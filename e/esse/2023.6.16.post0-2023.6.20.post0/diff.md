# Comparing `tmp/esse-2023.6.16.post0.tar.gz` & `tmp/esse-2023.6.20.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esse-2023.6.16.post0.tar", last modified: Fri Jun 16 01:20:31 2023, max compression
+gzip compressed data, was "esse-2023.6.20.post0.tar", last modified: Tue Jun 20 02:24:27 2023, max compression
```

## Comparing `esse-2023.6.16.post0.tar` & `esse-2023.6.20.post0.tar`

### file list

```diff
@@ -1,1263 +1,1263 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.772620 esse-2023.6.16.post0/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/.babelrc
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/.eslintrc.json
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.596617 esse-2023.6.16.post0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.628617 esse-2023.6.16.post0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-16 01:20:31.772620 esse-2023.6.16.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/build_schemas.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.632618 esse-2023.6.16.post0/example/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.632618 esse-2023.6.16.post0/example/core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.632618 esse-2023.6.16.post0/example/core/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/abstract/2d_data.json
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/abstract/2d_plot.json
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/abstract/3d_grid.json
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/abstract/3d_tensor.json
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/abstract/3d_vector_basis.json
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/abstract/point.json
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/abstract/vector.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.632618 esse-2023.6.16.post0/example/core/primitive/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/primitive/1d_data_series.json
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/primitive/3d_lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/primitive/array_of_3_booleans.json
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/primitive/array_of_3_numbers.json
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/primitive/array_of_ids.json
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/primitive/axis.json
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/primitive/scalar.json
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/primitive/string.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.632618 esse-2023.6.16.post0/example/core/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.636618 esse-2023.6.16.post0/example/core/reference/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/reference/experiment/condition.json
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/reference/experiment/location.json
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/reference/experiment.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.636618 esse-2023.6.16.post0/example/core/reference/literature/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/reference/literature/name.json
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/reference/literature/pages.json
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/reference/literature.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.636618 esse-2023.6.16.post0/example/core/reference/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/reference/modeling/exabyte.json
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/reference/modeling.json
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/reference.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.636618 esse-2023.6.16.post0/example/core/reusable/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/reusable/atomic_vectors.json
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/reusable/band_gap.json
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/reusable/energy.json
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/reusable/file_metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/core/reusable/object_storage_container_data.json
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/element.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.636618 esse-2023.6.16.post0/example/job/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/job/compute.json
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/job.json
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/material.json
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/method.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.636618 esse-2023.6.16.post0/example/methods_directory/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/methods_directory/local-orbital.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.636618 esse-2023.6.16.post0/example/methods_directory/pseudopotential/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/methods_directory/pseudopotential/dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.636618 esse-2023.6.16.post0/example/methods_directory/pseudopotential/file/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/methods_directory/pseudopotential/file/energy_cutoff.json
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/methods_directory/pseudopotential/file/exchange_correlation.json
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/methods_directory/pseudopotential/file/radii.json
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/methods_directory/pseudopotential/file.json
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/methods_directory/pseudopotential/precision.json
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/methods_directory/pseudopotential.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.636618 esse-2023.6.16.post0/example/methods_directory/regression/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/methods_directory/regression/data_per_feature.json
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/methods_directory/regression/dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.636618 esse-2023.6.16.post0/example/methods_directory/regression/kernel_ridge/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/methods_directory/regression/kernel_ridge/data_per_property.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.636618 esse-2023.6.16.post0/example/methods_directory/regression/linear/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/methods_directory/regression/linear/data_per_property.json
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/methods_directory/regression/precision.json
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/methods_directory/regression/precision_per_property.json
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/methods_directory/regression.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.636618 esse-2023.6.16.post0/example/model/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/model/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/model.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.600617 esse-2023.6.16.post0/example/models_directory/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.600617 esse-2023.6.16.post0/example/models_directory/pb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.636618 esse-2023.6.16.post0/example/models_directory/pb/qm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.640618 esse-2023.6.16.post0/example/models_directory/pb/qm/abin/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/models_directory/pb/qm/abin/configuration_interaction.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.640618 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.640618 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/dispersion_models_directory/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/dispersion_models_directory/dft_d.json
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/dispersion_models_directory/exchange_dipole.json
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/dispersion_models_directory/many_body_dispersion.json
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/dispersion_models_directory/non_local_correlation.json
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/dispersion_models_directory/tkatchenko_scheffler.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.640618 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/functional/component.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.640618 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/functional/components_directory/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/functional/components_directory/local_functional_lda.json
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/functional.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.640618 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/ksdft/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.640618 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/ksdft/double_hybrid/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.640618 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/ksdft/gga/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/ksdft/gga/functional.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.640618 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/ksdft/hybrid/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/ksdft/hybrid/functional.json
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.640618 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/ksdft/lda/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/ksdft/lda/functional.json
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/ksdft/lda.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.640618 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/ksdft/mgga/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/ksdft/mgga/functional.json
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/models_directory/pb/qm/dft/ksdft.json
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/models_directory/pb/qm/semp.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.600617 esse-2023.6.16.post0/example/models_directory/st/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.640618 esse-2023.6.16.post0/example/models_directory/st/det/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/models_directory/st/det/ml.json
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/new_model.json
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/project.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.640618 esse-2023.6.16.post0/example/properties_directory/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/electronic_configuration.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.640618 esse-2023.6.16.post0/example/properties_directory/elemental/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/elemental/atomic_radius.json
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/elemental/electronegativity.json
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/elemental/ionization_potential.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.644618 esse-2023.6.16.post0/example/properties_directory/non-scalar/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/non-scalar/band_gaps.json
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/non-scalar/band_structure.json
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/non-scalar/charge_density_profile.json
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/non-scalar/density_of_states.json
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/non-scalar/file_content.json
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/non-scalar/phonon_dispersions.json
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/non-scalar/phonon_dos.json
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/non-scalar/potential_profile.json
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/non-scalar/reaction_energy_profile.json
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/non-scalar/stress_tensor.json
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/non-scalar/total_energy_contributions.json
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/non-scalar/vibrational_spectrum.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.644618 esse-2023.6.16.post0/example/properties_directory/scalar/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/scalar/electron_affinity.json
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/scalar/fermi_energy.json
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/scalar/formation_energy.json
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/scalar/ionization_potential.json
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/scalar/pressure.json
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/scalar/reaction_energy_barrier.json
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/scalar/surface_energy.json
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/scalar/total_energy.json
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/scalar/total_force.json
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/scalar/valence_band_offset.json
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/scalar/zero_point_energy.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.648618 esse-2023.6.16.post0/example/properties_directory/structural/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/structural/atomic_forces.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.648618 esse-2023.6.16.post0/example/properties_directory/structural/basis/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/structural/basis/atomic_constraints.json
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/structural/basis/atomic_coordinate.json
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/structural/basis/atomic_coordinates.json
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/structural/basis/atomic_element.json
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/structural/basis/bonds.json
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/structural/basis.json
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/structural/density.json
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/structural/elemental_ratio.json
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/structural/inchi.json
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/structural/inchi_key.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.648618 esse-2023.6.16.post0/example/properties_directory/structural/lattice/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/structural/lattice/lattice_bravais.json
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/structural/lattice/lattice_vectors.json
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/structural/lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/structural/magnetic_moments.json
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/structural/molecular_pattern.json
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/structural/p-norm.json
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/structural/symmetry.json
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/structural/volume.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.604617 esse-2023.6.16.post0/example/properties_directory/workflow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.648618 esse-2023.6.16.post0/example/properties_directory/workflow/convergence/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/workflow/convergence/electronic.json
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/workflow/convergence/ionic.json
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/properties_directory/workflow/convergence/kpoint.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.648618 esse-2023.6.16.post0/example/property/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/property/best.json
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/property/raw.json
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/property/refined.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.648618 esse-2023.6.16.post0/example/software/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/software/application.json
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/software/executable.json
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/software/flavor.json
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/software/template.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.604617 esse-2023.6.16.post0/example/software_directory/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.648618 esse-2023.6.16.post0/example/software_directory/ml/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/software_directory/ml/exabyteml.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.604617 esse-2023.6.16.post0/example/software_directory/ml/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.652618 esse-2023.6.16.post0/example/software_directory/ml/unit/execution/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.652618 esse-2023.6.16.post0/example/software_directory/ml/unit/execution/evaluate/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/software_directory/ml/unit/execution/evaluate/cross-validate.json
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/software_directory/ml/unit/execution/initialize.json
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/software_directory/ml/unit/execution/score.json
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/software_directory/ml/unit/execution/train.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.604617 esse-2023.6.16.post0/example/software_directory/ml/unit/processing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.652618 esse-2023.6.16.post0/example/software_directory/ml/unit/processing/data_transformation/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/software_directory/ml/unit/processing/data_transformation/manipulation.json
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.652618 esse-2023.6.16.post0/example/software_directory/ml/unit/processing/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/software_directory/ml/unit/processing/feature_selection/filter_based.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.652618 esse-2023.6.16.post0/example/software_directory/modeling/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.652618 esse-2023.6.16.post0/example/software_directory/modeling/espresso/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/software_directory/modeling/espresso/arguments.json
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/software_directory/modeling/espresso.json
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/software_directory/modeling/nwchem.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.652618 esse-2023.6.16.post0/example/software_directory/modeling/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/software_directory/modeling/unit/execution.json
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/software_directory/modeling/vasp.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.652618 esse-2023.6.16.post0/example/software_directory/scripting/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/software_directory/scripting/jupyter-lab.json
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/software_directory/scripting/python.json
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/software_directory/scripting/shell.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.652618 esse-2023.6.16.post0/example/software_directory/scripting/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/software_directory/scripting/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.652618 esse-2023.6.16.post0/example/system/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/system/_material.json
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/system/_parent_job.json
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/system/_project.json
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/system/creator.json
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/system/entity_reference.json
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/system/file_source.json
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/system/message.json
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/system/owner.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.652618 esse-2023.6.16.post0/example/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/workflow/new_subworkflow.json
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/workflow/subworkflow.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.656618 esse-2023.6.16.post0/example/workflow/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/workflow/unit/assignment.json
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/workflow/unit/condition.json
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/workflow/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.656618 esse-2023.6.16.post0/example/workflow/unit/input/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/workflow/unit/input/_inputItemScope.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.656618 esse-2023.6.16.post0/example/workflow/unit/io/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/workflow/unit/io/api.json
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/workflow/unit/io/db.json
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/workflow/unit/io/object_storage.json
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/workflow/unit/io.json
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/workflow/unit/map.json
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/workflow/unit/processing.json
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/workflow/unit/reduce.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.656618 esse-2023.6.16.post0/example/workflow/unit/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/workflow/unit/runtime/runtime_items.json
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/workflow/unit.json
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/example/workflow.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.656618 esse-2023.6.16.post0/manifest/
--rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/manifest/dft_unit_functionals.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/manifest/functional_lookup_table.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/manifest/models.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/manifest/properties.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/npmignore
--rw-r--r--   0 runner    (1001) docker     (123)   269811 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      340 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/refactor.sh
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/requirements-dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1489 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/run-tests.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.656618 esse-2023.6.16.post0/schema/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.656618 esse-2023.6.16.post0/schema/core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.660618 esse-2023.6.16.post0/schema/core/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/abstract/2d_data.json
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/abstract/2d_plot.json
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/abstract/3d_grid.json
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/abstract/3d_tensor.json
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/abstract/3d_vector_basis.json
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/abstract/point.json
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/abstract/vector.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.660618 esse-2023.6.16.post0/schema/core/primitive/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/primitive/1d_data_series.json
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/primitive/3d_lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/primitive/array_of_3_booleans.json
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/primitive/array_of_3_numbers.json
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/primitive/array_of_ids.json
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/primitive/array_of_numbers.json
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/primitive/array_of_strings.json
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/primitive/axis.json
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/primitive/scalar.json
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/primitive/slugified_entry.json
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/primitive/slugified_entry_or_slug.json
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/primitive/string.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.660618 esse-2023.6.16.post0/schema/core/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/reference/exabyte.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.660618 esse-2023.6.16.post0/schema/core/reference/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/reference/experiment/condition.json
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/reference/experiment/location.json
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/reference/experiment.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.660618 esse-2023.6.16.post0/schema/core/reference/literature/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/reference/literature/name.json
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/reference/literature/pages.json
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/reference/literature.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.660618 esse-2023.6.16.post0/schema/core/reference/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/reference/modeling/exabyte.json
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/reference/modeling.json
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/reference.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.664618 esse-2023.6.16.post0/schema/core/reusable/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/reusable/atomic_scalars.json
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/reusable/atomic_strings.json
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/reusable/atomic_vectors.json
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/reusable/band_gap.json
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/reusable/energy.json
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/reusable/file_metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/core/reusable/object_storage_container_data.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.664618 esse-2023.6.16.post0/schema/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/definitions/units.json
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/element.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.664618 esse-2023.6.16.post0/schema/in_memory_entity/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/in_memory_entity/base.json
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/in_memory_entity/defaultable.json
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/in_memory_entity/named.json
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/in_memory_entity/named_defaultable.json
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/in_memory_entity/named_defaultable_has_metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/in_memory_entity/named_defaultable_runtime_items.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.664618 esse-2023.6.16.post0/schema/job/
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/job/compute.json
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/job.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.664618 esse-2023.6.16.post0/schema/material/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/material/conventional.json
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/material.json
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/method.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.664618 esse-2023.6.16.post0/schema/methods_directory/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/methods_directory/local-orbital.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.604617 esse-2023.6.16.post0/schema/methods_directory/local_orbital/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.664618 esse-2023.6.16.post0/schema/methods_directory/local_orbital/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/methods_directory/local_orbital/definitions/basis_sets.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.664618 esse-2023.6.16.post0/schema/methods_directory/pseudopotential/
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/methods_directory/pseudopotential/dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.668618 esse-2023.6.16.post0/schema/methods_directory/pseudopotential/file/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/methods_directory/pseudopotential/file/energy_cutoff.json
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/methods_directory/pseudopotential/file/exchange_correlation.json
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/methods_directory/pseudopotential/file/radii.json
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/methods_directory/pseudopotential/file.json
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/methods_directory/pseudopotential/precision.json
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/methods_directory/pseudopotential.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.668618 esse-2023.6.16.post0/schema/methods_directory/regression/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/methods_directory/regression/data.json
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/methods_directory/regression/data_per_feature.json
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/methods_directory/regression/dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.668618 esse-2023.6.16.post0/schema/methods_directory/regression/kernel_ridge/
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/methods_directory/regression/kernel_ridge/data_per_property.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.668618 esse-2023.6.16.post0/schema/methods_directory/regression/linear/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/methods_directory/regression/linear/data_per_property.json
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/methods_directory/regression/precision.json
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/methods_directory/regression/precision_per_property.json
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/methods_directory/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/methods_directory/unknown.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.668618 esse-2023.6.16.post0/schema/model/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/model/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/model/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/model/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/model.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.668618 esse-2023.6.16.post0/schema/models_directory/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/definitions.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.668618 esse-2023.6.16.post0/schema/models_directory/pb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.668618 esse-2023.6.16.post0/schema/models_directory/pb/qm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.668618 esse-2023.6.16.post0/schema/models_directory/pb/qm/abin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.672618 esse-2023.6.16.post0/schema/models_directory/pb/qm/abin/configuration_interaction/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/abin/configuration_interaction/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/abin/configuration_interaction/definitions.json
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/abin/configuration_interaction/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/abin/configuration_interaction/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/abin/configuration_interaction.json
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/abin/definitions.json
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/abin/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/abin.json
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/definitions.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.672618 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/
--rw-r--r--   0 runner    (1001) docker     (123)    36659 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dft_unit_functionals.json
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dft_unit_functionals_proto.json
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dispersion_model.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.672618 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/dft_d.json
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/exchange_dipole.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.672618 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_abin.json
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_empirical.json
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_abin.json
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_empirical.json
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/many_body_dispersion.json
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/non_local_correlation.json
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/tkatchenko_scheffler.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.672618 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/functional/component.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.672618 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/functional/components_directory/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/functional/components_directory/dispersion_correction.json
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/functional/components_directory/exact_exchange.json
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional.json
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional_gga.json
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional_lda.json
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional_mgga.json
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/functional/components_directory/mp2_correlation.json
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/functional/components_directory/range_separated_exchange.json
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/functional/definitions.json
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/functional/local_functional_components.json
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/functional.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.676618 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/definitions.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.676618 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/definitions.json
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.676618 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/gga/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/gga/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/gga/definitions.json
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/gga/functional.json
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/gga/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/gga/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/gga.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.680618 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/definitions.json
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/functional.json
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.680618 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/lda/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/lda/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/lda/definitions.json
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/lda/functional.json
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/lda/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/lda/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/lda.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.680618 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/definitions.json
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/functional.json
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/mgga.json
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft.json
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/dft.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.680618 esse-2023.6.16.post0/schema/models_directory/pb/qm/semp/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/semp/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/semp/definitions.json
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/semp/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/semp/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/semp.json
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb/qm.json
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/pb.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.680618 esse-2023.6.16.post0/schema/models_directory/st/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.680618 esse-2023.6.16.post0/schema/models_directory/st/det/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/st/det/ml.json
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/st/det.json
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/st.json
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/models_directory/unknown.json
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/new_model.json
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/project.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.680618 esse-2023.6.16.post0/schema/properties_directory/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/derived_properties.json
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/electronic_configuration.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.680618 esse-2023.6.16.post0/schema/properties_directory/elemental/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/elemental/atomic_radius.json
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/elemental/electronegativity.json
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/elemental/ionization_potential.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.684618 esse-2023.6.16.post0/schema/properties_directory/non-scalar/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/non-scalar/average_potential_profile.json
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/non-scalar/band_gaps.json
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/non-scalar/band_structure.json
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/non-scalar/charge_density_profile.json
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/non-scalar/density_of_states.json
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/non-scalar/file_content.json
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/non-scalar/phonon_dispersions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/non-scalar/phonon_dos.json
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/non-scalar/potential_profile.json
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/non-scalar/reaction_energy_profile.json
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/non-scalar/stress_tensor.json
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/non-scalar/total_energy_contributions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/non-scalar/vibrational_spectrum.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.684618 esse-2023.6.16.post0/schema/properties_directory/scalar/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/scalar/electron_affinity.json
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/scalar/fermi_energy.json
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/scalar/formation_energy.json
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/scalar/ionization_potential.json
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/scalar/pressure.json
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/scalar/reaction_energy_barrier.json
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/scalar/surface_energy.json
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/scalar/total_energy.json
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/scalar/total_force.json
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/scalar/valence_band_offset.json
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/scalar/zero_point_energy.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.688618 esse-2023.6.16.post0/schema/properties_directory/structural/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/structural/atomic_forces.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.688618 esse-2023.6.16.post0/schema/properties_directory/structural/basis/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/structural/basis/atomic_constraints.json
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/structural/basis/atomic_coordinate.json
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/structural/basis/atomic_coordinates.json
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/structural/basis/atomic_element.json
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/structural/basis/bonds.json
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/structural/basis.json
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/structural/density.json
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/structural/elemental_ratio.json
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/structural/inchi.json
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/structural/inchi_key.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.688618 esse-2023.6.16.post0/schema/properties_directory/structural/lattice/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/structural/lattice/lattice_bravais.json
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/structural/lattice/lattice_vectors.json
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/structural/lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/structural/magnetic_moments.json
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/structural/molecular_pattern.json
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/structural/p-norm.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.688618 esse-2023.6.16.post0/schema/properties_directory/structural/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/structural/patterns/functional_group.json
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/structural/patterns/ring.json
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/structural/patterns/special_bond.json
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/structural/symmetry.json
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/structural/volume.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.608617 esse-2023.6.16.post0/schema/properties_directory/workflow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.688618 esse-2023.6.16.post0/schema/properties_directory/workflow/convergence/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/workflow/convergence/electronic.json
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/workflow/convergence/ionic.json
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/properties_directory/workflow/convergence/kpoint.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.688618 esse-2023.6.16.post0/schema/property/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/property/best.json
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/property/raw.json
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/property/refined.json
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/property/source.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.688618 esse-2023.6.16.post0/schema/software/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software/application.json
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software/executable.json
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software/flavor.json
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software/template.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.612617 esse-2023.6.16.post0/schema/software_directory/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.688618 esse-2023.6.16.post0/schema/software_directory/ml/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software_directory/ml/exabyteml.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.688618 esse-2023.6.16.post0/schema/software_directory/ml/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.692618 esse-2023.6.16.post0/schema/software_directory/ml/unit/execution/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.692618 esse-2023.6.16.post0/schema/software_directory/ml/unit/execution/evaluate/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software_directory/ml/unit/execution/evaluate/cross-validate.json
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software_directory/ml/unit/execution/initialize.json
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software_directory/ml/unit/execution/score.json
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software_directory/ml/unit/execution/train.json
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software_directory/ml/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.692618 esse-2023.6.16.post0/schema/software_directory/ml/unit/processing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.692618 esse-2023.6.16.post0/schema/software_directory/ml/unit/processing/data_transformation/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software_directory/ml/unit/processing/data_transformation/manipulation.json
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software_directory/ml/unit/processing/data_transformation.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.692618 esse-2023.6.16.post0/schema/software_directory/ml/unit/processing/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software_directory/ml/unit/processing/feature_selection/filter_based.json
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software_directory/ml/unit/processing/feature_selection.json
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software_directory/ml/unit/processing.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.692618 esse-2023.6.16.post0/schema/software_directory/modeling/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.692618 esse-2023.6.16.post0/schema/software_directory/modeling/espresso/
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software_directory/modeling/espresso/arguments.json
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software_directory/modeling/espresso.json
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software_directory/modeling/nwchem.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.692618 esse-2023.6.16.post0/schema/software_directory/modeling/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software_directory/modeling/unit/execution.json
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software_directory/modeling/vasp.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.692618 esse-2023.6.16.post0/schema/software_directory/scripting/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software_directory/scripting/jupyter-lab.json
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software_directory/scripting/python.json
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software_directory/scripting/shell.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.692618 esse-2023.6.16.post0/schema/software_directory/scripting/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/software_directory/scripting/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.696618 esse-2023.6.16.post0/schema/system/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/_material.json
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/_parent_job.json
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/_project.json
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/bankable.json
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/creator.json
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/creator_account.json
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/database_source.json
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/defaultable.json
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/description.json
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/entity_reference.json
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/file_source.json
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/history.json
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/in_set.json
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/is_multi_material.json
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/is_outdated.json
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/job_extended.json
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/message.json
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/name.json
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/owner.json
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/schema_version.json
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/scope.json
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/set.json
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/sharing.json
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/soft_removable.json
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/status.json
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/timestampable.json
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/system/use_values.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.696618 esse-2023.6.16.post0/schema/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow/base_flow.json
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow/new_subworkflow.json
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow/subworkflow.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.700619 esse-2023.6.16.post0/schema/workflow/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow/unit/assertion.json
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow/unit/assignment.json
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow/unit/condition.json
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.700619 esse-2023.6.16.post0/schema/workflow/unit/input/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow/unit/input/_input.json
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow/unit/input/_inputItem.json
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow/unit/input/_inputItemId.json
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow/unit/input/_inputItemScope.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.700619 esse-2023.6.16.post0/schema/workflow/unit/io/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow/unit/io/api.json
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow/unit/io/db.json
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow/unit/io/object_storage.json
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow/unit/io.json
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow/unit/map.json
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow/unit/processing.json
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow/unit/reduce.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.700619 esse-2023.6.16.post0/schema/workflow/unit/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow/unit/runtime/_runtime_item_full_object.json
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow/unit/runtime/_runtime_item_name_object.json
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow/unit/runtime/_runtime_item_string.json
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow/unit/runtime/runtime_item.json
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow/unit/runtime/runtime_items.json
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow/unit.json
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/schema/workflow.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 01:20:31.772620 esse-2023.6.16.post0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.612617 esse-2023.6.16.post0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.612617 esse-2023.6.16.post0/src/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.700619 esse-2023.6.16.post0/src/js/esse/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/js/esse/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/js/esse/settings.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.700619 esse-2023.6.16.post0/src/js/esse/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/js/esse/tests/validate.js
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/js/esse/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.700619 esse-2023.6.16.post0/src/js/json_include/
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/js/json_include/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/js/json_include/settings.js
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/js/json_include/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.700619 esse-2023.6.16.post0/src/js/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/js/scripts/setSchemaIds.mjs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.612617 esse-2023.6.16.post0/src/py/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.704619 esse-2023.6.16.post0/src/py/esse/
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-16 01:20:31.000000 esse-2023.6.16.post0/src/py/esse/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.620617 esse-2023.6.16.post0/src/py/esse/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.704619 esse-2023.6.16.post0/src/py/esse/data/example/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.704619 esse-2023.6.16.post0/src/py/esse/data/example/core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.704619 esse-2023.6.16.post0/src/py/esse/data/example/core/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/abstract/2d_data.json
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/abstract/2d_plot.json
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/abstract/3d_grid.json
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/abstract/3d_tensor.json
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/abstract/3d_vector_basis.json
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/abstract/point.json
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/abstract/vector.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.708619 esse-2023.6.16.post0/src/py/esse/data/example/core/primitive/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/primitive/1d_data_series.json
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/primitive/3d_lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/primitive/array_of_3_booleans.json
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/primitive/array_of_3_numbers.json
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/primitive/array_of_ids.json
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/primitive/axis.json
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/primitive/scalar.json
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/primitive/string.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.708619 esse-2023.6.16.post0/src/py/esse/data/example/core/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.708619 esse-2023.6.16.post0/src/py/esse/data/example/core/reference/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/reference/experiment/condition.json
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/reference/experiment/location.json
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/reference/experiment.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.708619 esse-2023.6.16.post0/src/py/esse/data/example/core/reference/literature/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/reference/literature/name.json
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/reference/literature/pages.json
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/reference/literature.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.708619 esse-2023.6.16.post0/src/py/esse/data/example/core/reference/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/reference/modeling/exabyte.json
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/reference/modeling.json
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/reference.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.708619 esse-2023.6.16.post0/src/py/esse/data/example/core/reusable/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/reusable/atomic_vectors.json
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/reusable/band_gap.json
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/reusable/energy.json
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/reusable/file_metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/core/reusable/object_storage_container_data.json
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/element.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.708619 esse-2023.6.16.post0/src/py/esse/data/example/job/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/job/compute.json
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/job.json
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/material.json
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/method.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.708619 esse-2023.6.16.post0/src/py/esse/data/example/methods_directory/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/methods_directory/local-orbital.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.712619 esse-2023.6.16.post0/src/py/esse/data/example/methods_directory/pseudopotential/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/methods_directory/pseudopotential/dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.712619 esse-2023.6.16.post0/src/py/esse/data/example/methods_directory/pseudopotential/file/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/methods_directory/pseudopotential/file/energy_cutoff.json
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/methods_directory/pseudopotential/file/exchange_correlation.json
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/methods_directory/pseudopotential/file/radii.json
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/methods_directory/pseudopotential/file.json
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/methods_directory/pseudopotential/precision.json
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/methods_directory/pseudopotential.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.712619 esse-2023.6.16.post0/src/py/esse/data/example/methods_directory/regression/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/methods_directory/regression/data_per_feature.json
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/methods_directory/regression/dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.712619 esse-2023.6.16.post0/src/py/esse/data/example/methods_directory/regression/kernel_ridge/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/methods_directory/regression/kernel_ridge/data_per_property.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.712619 esse-2023.6.16.post0/src/py/esse/data/example/methods_directory/regression/linear/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/methods_directory/regression/linear/data_per_property.json
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/methods_directory/regression/precision.json
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/methods_directory/regression/precision_per_property.json
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/methods_directory/regression.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.712619 esse-2023.6.16.post0/src/py/esse/data/example/model/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/model/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/model.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.616617 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.612617 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.712619 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.712619 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/abin/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/abin/configuration_interaction.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.712619 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.712619 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/dispersion_models_directory/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/dispersion_models_directory/dft_d.json
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/dispersion_models_directory/exchange_dipole.json
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/dispersion_models_directory/many_body_dispersion.json
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/dispersion_models_directory/non_local_correlation.json
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/dispersion_models_directory/tkatchenko_scheffler.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.712619 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/functional/component.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.712619 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/functional/components_directory/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/functional/components_directory/local_functional_lda.json
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/functional.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.712619 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.712619 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/double_hybrid/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.712619 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/gga/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/gga/functional.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.716619 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/hybrid/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/hybrid/functional.json
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.716619 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/lda/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/lda/functional.json
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/lda.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.716619 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/mgga/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/mgga/functional.json
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft.json
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/semp.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.616617 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/st/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.716619 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/st/det/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/models_directory/st/det/ml.json
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/new_model.json
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/project.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.716619 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/electronic_configuration.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.716619 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/elemental/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/elemental/atomic_radius.json
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/elemental/electronegativity.json
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/elemental/ionization_potential.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.716619 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/non-scalar/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/non-scalar/band_gaps.json
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/non-scalar/band_structure.json
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/non-scalar/charge_density_profile.json
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/non-scalar/density_of_states.json
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/non-scalar/file_content.json
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/non-scalar/phonon_dispersions.json
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/non-scalar/phonon_dos.json
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/non-scalar/potential_profile.json
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/non-scalar/reaction_energy_profile.json
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/non-scalar/stress_tensor.json
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/non-scalar/total_energy_contributions.json
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/non-scalar/vibrational_spectrum.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.720619 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/scalar/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/scalar/electron_affinity.json
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/scalar/fermi_energy.json
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/scalar/formation_energy.json
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/scalar/ionization_potential.json
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/scalar/pressure.json
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/scalar/reaction_energy_barrier.json
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/scalar/surface_energy.json
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/scalar/total_energy.json
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/scalar/total_force.json
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/scalar/valence_band_offset.json
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/scalar/zero_point_energy.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.720619 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/structural/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/structural/atomic_forces.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.724619 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/structural/basis/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/structural/basis/atomic_constraints.json
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/structural/basis/atomic_coordinate.json
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/structural/basis/atomic_coordinates.json
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/structural/basis/atomic_element.json
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/structural/basis/bonds.json
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/structural/basis.json
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/structural/density.json
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/structural/elemental_ratio.json
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/structural/inchi.json
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/structural/inchi_key.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.724619 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/structural/lattice/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/structural/lattice/lattice_bravais.json
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/structural/lattice/lattice_vectors.json
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/structural/lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/structural/magnetic_moments.json
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/structural/molecular_pattern.json
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/structural/p-norm.json
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/structural/symmetry.json
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/structural/volume.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.616617 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/workflow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.724619 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/workflow/convergence/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/workflow/convergence/electronic.json
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/workflow/convergence/ionic.json
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/workflow/convergence/kpoint.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.724619 esse-2023.6.16.post0/src/py/esse/data/example/property/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/property/best.json
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/property/raw.json
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/property/refined.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.724619 esse-2023.6.16.post0/src/py/esse/data/example/software/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/software/application.json
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/software/executable.json
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/software/flavor.json
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/software/template.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.620617 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.724619 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/ml/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/ml/exabyteml.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.616617 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/ml/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.724619 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/ml/unit/execution/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.724619 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/ml/unit/execution/evaluate/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/ml/unit/execution/evaluate/cross-validate.json
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/ml/unit/execution/initialize.json
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/ml/unit/execution/score.json
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/ml/unit/execution/train.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.616617 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/ml/unit/processing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.724619 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/ml/unit/processing/data_transformation/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/ml/unit/processing/data_transformation/manipulation.json
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.724619 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/ml/unit/processing/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/ml/unit/processing/feature_selection/filter_based.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.728619 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/modeling/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.728619 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/modeling/espresso/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/modeling/espresso/arguments.json
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/modeling/espresso.json
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/modeling/nwchem.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.728619 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/modeling/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/modeling/unit/execution.json
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/modeling/vasp.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.728619 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/scripting/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/scripting/jupyter-lab.json
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/scripting/python.json
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/scripting/shell.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.728619 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/scripting/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/software_directory/scripting/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.728619 esse-2023.6.16.post0/src/py/esse/data/example/system/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/system/_material.json
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/system/_parent_job.json
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/system/_project.json
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/system/creator.json
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/system/entity_reference.json
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/system/file_source.json
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/system/message.json
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/system/owner.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.728619 esse-2023.6.16.post0/src/py/esse/data/example/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/workflow/new_subworkflow.json
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/workflow/subworkflow.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.728619 esse-2023.6.16.post0/src/py/esse/data/example/workflow/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/workflow/unit/assignment.json
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/workflow/unit/condition.json
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/workflow/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.728619 esse-2023.6.16.post0/src/py/esse/data/example/workflow/unit/input/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/workflow/unit/input/_inputItemScope.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.732619 esse-2023.6.16.post0/src/py/esse/data/example/workflow/unit/io/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/workflow/unit/io/api.json
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/workflow/unit/io/db.json
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/workflow/unit/io/object_storage.json
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/workflow/unit/io.json
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/workflow/unit/map.json
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/workflow/unit/processing.json
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/workflow/unit/reduce.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.732619 esse-2023.6.16.post0/src/py/esse/data/example/workflow/unit/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/workflow/unit/runtime/runtime_items.json
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/workflow/unit.json
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/example/workflow.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.732619 esse-2023.6.16.post0/src/py/esse/data/manifest/
--rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/manifest/dft_unit_functionals.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/manifest/functional_lookup_table.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/manifest/models.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/manifest/properties.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.732619 esse-2023.6.16.post0/src/py/esse/data/schema/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.732619 esse-2023.6.16.post0/src/py/esse/data/schema/core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.732619 esse-2023.6.16.post0/src/py/esse/data/schema/core/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/abstract/2d_data.json
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/abstract/2d_plot.json
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/abstract/3d_grid.json
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/abstract/3d_tensor.json
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/abstract/3d_vector_basis.json
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/abstract/point.json
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/abstract/vector.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.736619 esse-2023.6.16.post0/src/py/esse/data/schema/core/primitive/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/primitive/1d_data_series.json
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/primitive/3d_lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/primitive/array_of_3_booleans.json
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/primitive/array_of_3_numbers.json
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/primitive/array_of_ids.json
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/primitive/array_of_numbers.json
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/primitive/array_of_strings.json
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/primitive/axis.json
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/primitive/scalar.json
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/primitive/slugified_entry.json
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/primitive/slugified_entry_or_slug.json
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/primitive/string.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.736619 esse-2023.6.16.post0/src/py/esse/data/schema/core/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/reference/exabyte.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.736619 esse-2023.6.16.post0/src/py/esse/data/schema/core/reference/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/reference/experiment/condition.json
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/reference/experiment/location.json
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/reference/experiment.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.736619 esse-2023.6.16.post0/src/py/esse/data/schema/core/reference/literature/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/reference/literature/name.json
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/reference/literature/pages.json
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/reference/literature.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.736619 esse-2023.6.16.post0/src/py/esse/data/schema/core/reference/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/reference/modeling/exabyte.json
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/reference/modeling.json
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/reference.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.736619 esse-2023.6.16.post0/src/py/esse/data/schema/core/reusable/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/reusable/atomic_scalars.json
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/reusable/atomic_strings.json
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/reusable/atomic_vectors.json
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/reusable/band_gap.json
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/reusable/energy.json
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/reusable/file_metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/core/reusable/object_storage_container_data.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.736619 esse-2023.6.16.post0/src/py/esse/data/schema/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/definitions/units.json
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/element.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.740619 esse-2023.6.16.post0/src/py/esse/data/schema/in_memory_entity/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/in_memory_entity/base.json
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/in_memory_entity/defaultable.json
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/in_memory_entity/named.json
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/in_memory_entity/named_defaultable.json
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/in_memory_entity/named_defaultable_has_metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/in_memory_entity/named_defaultable_runtime_items.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.740619 esse-2023.6.16.post0/src/py/esse/data/schema/job/
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/job/compute.json
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/job.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.740619 esse-2023.6.16.post0/src/py/esse/data/schema/material/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/material/conventional.json
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/material.json
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/method.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.740619 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/local-orbital.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.620617 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/local_orbital/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.740619 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/local_orbital/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/local_orbital/definitions/basis_sets.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.740619 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/pseudopotential/
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/pseudopotential/dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.740619 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file/energy_cutoff.json
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file/exchange_correlation.json
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file/radii.json
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file.json
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/pseudopotential/precision.json
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/pseudopotential.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.740619 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/regression/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/regression/data.json
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/regression/data_per_feature.json
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/regression/dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.740619 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/regression/kernel_ridge/
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/regression/kernel_ridge/data_per_property.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.740619 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/regression/linear/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/regression/linear/data_per_property.json
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/regression/precision.json
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/regression/precision_per_property.json
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/unknown.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.740619 esse-2023.6.16.post0/src/py/esse/data/schema/model/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/model/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/model/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/model/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/model.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.744619 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/definitions.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.744619 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.744619 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.744619 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.744619 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/definitions.json
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction.json
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/definitions.json
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/abin.json
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/definitions.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.744619 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/
--rw-r--r--   0 runner    (1001) docker     (123)    36659 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dft_unit_functionals.json
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dft_unit_functionals_proto.json
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_model.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.744619 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/dft_d.json
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/exchange_dipole.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.748619 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_abin.json
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_empirical.json
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_abin.json
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_empirical.json
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/many_body_dispersion.json
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/non_local_correlation.json
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/tkatchenko_scheffler.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.748619 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/component.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.748619 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/dispersion_correction.json
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/exact_exchange.json
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional.json
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional_gga.json
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional_lda.json
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional_mgga.json
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/mp2_correlation.json
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/range_separated_exchange.json
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/definitions.json
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/local_functional_components.json
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.748619 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/definitions.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.752619 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/definitions.json
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.752619 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/definitions.json
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/functional.json
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.752619 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/definitions.json
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/functional.json
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.752619 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/definitions.json
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/functional.json
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.752619 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/definitions.json
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/functional.json
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga.json
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft.json
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.752619 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/semp/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/semp/augmentations.json
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/semp/definitions.json
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/semp/modifiers.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/semp/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/semp.json
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm.json
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.752619 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/st/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.752619 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/st/det/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/st/det/ml.json
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/st/det.json
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/st.json
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/unknown.json
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/new_model.json
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/project.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.756619 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/derived_properties.json
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/electronic_configuration.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.756619 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/elemental/
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/elemental/atomic_radius.json
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/elemental/electronegativity.json
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/elemental/ionization_potential.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.756619 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/average_potential_profile.json
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/band_gaps.json
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/band_structure.json
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/charge_density_profile.json
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/density_of_states.json
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/file_content.json
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/phonon_dispersions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/phonon_dos.json
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/potential_profile.json
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/reaction_energy_profile.json
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/stress_tensor.json
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/total_energy_contributions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/vibrational_spectrum.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.760619 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/scalar/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/scalar/electron_affinity.json
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/scalar/fermi_energy.json
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/scalar/formation_energy.json
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/scalar/ionization_potential.json
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/scalar/pressure.json
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/scalar/reaction_energy_barrier.json
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/scalar/surface_energy.json
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/scalar/total_energy.json
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/scalar/total_force.json
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/scalar/valence_band_offset.json
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/scalar/zero_point_energy.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.760619 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/atomic_forces.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.760619 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/basis/
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/basis/atomic_constraints.json
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/basis/atomic_coordinate.json
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/basis/atomic_coordinates.json
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/basis/atomic_element.json
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/basis/bonds.json
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/basis.json
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/density.json
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/elemental_ratio.json
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/inchi.json
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/inchi_key.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.760619 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/lattice/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/lattice/lattice_bravais.json
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/lattice/lattice_vectors.json
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/magnetic_moments.json
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/molecular_pattern.json
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/p-norm.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.760619 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/patterns/functional_group.json
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/patterns/ring.json
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/patterns/special_bond.json
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/symmetry.json
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/volume.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.624617 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/workflow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.760619 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/electronic.json
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/ionic.json
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/kpoint.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.764619 esse-2023.6.16.post0/src/py/esse/data/schema/property/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/property/best.json
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/property/raw.json
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/property/refined.json
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/property/source.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.764619 esse-2023.6.16.post0/src/py/esse/data/schema/software/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software/application.json
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software/executable.json
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software/flavor.json
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software/template.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.624617 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.764619 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/exabyteml.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.764619 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.764619 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.764619 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/evaluate/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/evaluate/cross-validate.json
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/initialize.json
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/score.json
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/train.json
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.764619 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.764619 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/data_transformation/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/data_transformation/manipulation.json
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/data_transformation.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.764619 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/feature_selection/filter_based.json
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/feature_selection.json
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/unit/processing.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.764619 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/modeling/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.764619 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/modeling/espresso/
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/modeling/espresso/arguments.json
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/modeling/espresso.json
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/modeling/nwchem.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.764619 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/modeling/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/modeling/unit/execution.json
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/modeling/vasp.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.764619 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/scripting/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/scripting/jupyter-lab.json
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/scripting/python.json
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/scripting/shell.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.764619 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/scripting/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/scripting/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.768620 esse-2023.6.16.post0/src/py/esse/data/schema/system/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/_material.json
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/_parent_job.json
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/_project.json
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/bankable.json
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/creator.json
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/creator_account.json
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/database_source.json
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/defaultable.json
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/description.json
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/entity_reference.json
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/file_source.json
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/history.json
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/in_set.json
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/is_multi_material.json
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/is_outdated.json
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/job_extended.json
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/message.json
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/name.json
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/owner.json
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/schema_version.json
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/scope.json
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/set.json
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/sharing.json
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/soft_removable.json
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/status.json
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/timestampable.json
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/system/use_values.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.772620 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/base_flow.json
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/new_subworkflow.json
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/subworkflow.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.772620 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/assertion.json
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/assignment.json
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/condition.json
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/execution.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.772620 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/input/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/input/_input.json
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/input/_inputItem.json
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/input/_inputItemId.json
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/input/_inputItemScope.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.772620 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/io/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/io/api.json
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/io/db.json
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/io/object_storage.json
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/io.json
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/map.json
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/processing.json
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/reduce.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.772620 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/runtime/_runtime_item_full_object.json
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/runtime/_runtime_item_name_object.json
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/runtime/_runtime_item_string.json
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/runtime/runtime_item.json
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/runtime/runtime_items.json
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit.json
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/data/schema/workflow.json
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/functionals.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.772620 esse-2023.6.16.post0/src/py/esse/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/tests/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-16 01:20:06.000000 esse-2023.6.16.post0/src/py/esse/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 01:20:31.704619 esse-2023.6.16.post0/src/py/esse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-16 01:20:31.000000 esse-2023.6.16.post0/src/py/esse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    55972 2023-06-16 01:20:31.000000 esse-2023.6.16.post0/src/py/esse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 01:20:31.000000 esse-2023.6.16.post0/src/py/esse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-16 01:20:31.000000 esse-2023.6.16.post0/src/py/esse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-16 01:20:31.000000 esse-2023.6.16.post0/src/py/esse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-16 01:20:31.000000 esse-2023.6.16.post0/src/py/esse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.350976 esse-2023.6.20.post0/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/.babelrc
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/.eslintrc.json
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.222976 esse-2023.6.20.post0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.250976 esse-2023.6.20.post0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-20 02:24:27.350976 esse-2023.6.20.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/build_schemas.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.250976 esse-2023.6.20.post0/example/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.250976 esse-2023.6.20.post0/example/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.250976 esse-2023.6.20.post0/example/core/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/abstract/2d_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/abstract/2d_plot.json
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/abstract/3d_grid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/abstract/3d_tensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/abstract/3d_vector_basis.json
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/abstract/point.json
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/abstract/vector.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.250976 esse-2023.6.20.post0/example/core/primitive/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/primitive/1d_data_series.json
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/primitive/3d_lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/primitive/array_of_3_booleans.json
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/primitive/array_of_3_numbers.json
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/primitive/array_of_ids.json
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/primitive/axis.json
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/primitive/scalar.json
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/primitive/string.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.254976 esse-2023.6.20.post0/example/core/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.254976 esse-2023.6.20.post0/example/core/reference/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/reference/experiment/condition.json
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/reference/experiment/location.json
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/reference/experiment.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.254976 esse-2023.6.20.post0/example/core/reference/literature/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/reference/literature/name.json
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/reference/literature/pages.json
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/reference/literature.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.254976 esse-2023.6.20.post0/example/core/reference/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/reference/modeling/exabyte.json
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/reference/modeling.json
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/reference.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.254976 esse-2023.6.20.post0/example/core/reusable/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/reusable/atomic_vectors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/reusable/band_gap.json
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/reusable/energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/reusable/file_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/core/reusable/object_storage_container_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/element.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.254976 esse-2023.6.20.post0/example/job/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/job/compute.json
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/job.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/material.json
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/method.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.254976 esse-2023.6.20.post0/example/methods_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/methods_directory/local-orbital.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.254976 esse-2023.6.20.post0/example/methods_directory/pseudopotential/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/methods_directory/pseudopotential/dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.254976 esse-2023.6.20.post0/example/methods_directory/pseudopotential/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/methods_directory/pseudopotential/file/energy_cutoff.json
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/methods_directory/pseudopotential/file/exchange_correlation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/methods_directory/pseudopotential/file/radii.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/methods_directory/pseudopotential/file.json
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/methods_directory/pseudopotential/precision.json
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/methods_directory/pseudopotential.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.254976 esse-2023.6.20.post0/example/methods_directory/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/methods_directory/regression/data_per_feature.json
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/methods_directory/regression/dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.254976 esse-2023.6.20.post0/example/methods_directory/regression/kernel_ridge/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/methods_directory/regression/kernel_ridge/data_per_property.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.254976 esse-2023.6.20.post0/example/methods_directory/regression/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/methods_directory/regression/linear/data_per_property.json
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/methods_directory/regression/precision.json
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/methods_directory/regression/precision_per_property.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/methods_directory/regression.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.254976 esse-2023.6.20.post0/example/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/model/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/model.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.226976 esse-2023.6.20.post0/example/models_directory/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.226976 esse-2023.6.20.post0/example/models_directory/pb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.254976 esse-2023.6.20.post0/example/models_directory/pb/qm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.254976 esse-2023.6.20.post0/example/models_directory/pb/qm/abin/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/models_directory/pb/qm/abin/configuration_interaction.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.254976 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.254976 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/dispersion_models_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/dispersion_models_directory/dft_d.json
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/dispersion_models_directory/exchange_dipole.json
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/dispersion_models_directory/many_body_dispersion.json
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/dispersion_models_directory/non_local_correlation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/dispersion_models_directory/tkatchenko_scheffler.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.254976 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/functional/component.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.258976 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/functional/components_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/functional/components_directory/local_functional_lda.json
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/functional.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.258976 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/ksdft/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.258976 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/ksdft/double_hybrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.258976 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/ksdft/gga/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/ksdft/gga/functional.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.258976 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/ksdft/hybrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/ksdft/hybrid/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.258976 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/ksdft/lda/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/ksdft/lda/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/ksdft/lda.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.258976 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/ksdft/mgga/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/ksdft/mgga/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/models_directory/pb/qm/dft/ksdft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/models_directory/pb/qm/semp.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.226976 esse-2023.6.20.post0/example/models_directory/st/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.258976 esse-2023.6.20.post0/example/models_directory/st/det/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/models_directory/st/det/ml.json
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/new_model.json
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/project.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.258976 esse-2023.6.20.post0/example/properties_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/electronic_configuration.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.258976 esse-2023.6.20.post0/example/properties_directory/elemental/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/elemental/atomic_radius.json
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/elemental/electronegativity.json
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/elemental/ionization_potential.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.258976 esse-2023.6.20.post0/example/properties_directory/non-scalar/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/non-scalar/band_gaps.json
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/non-scalar/band_structure.json
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/non-scalar/charge_density_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/non-scalar/density_of_states.json
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/non-scalar/file_content.json
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/non-scalar/phonon_dispersions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/non-scalar/phonon_dos.json
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/non-scalar/potential_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/non-scalar/reaction_energy_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/non-scalar/stress_tensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/non-scalar/total_energy_contributions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/non-scalar/vibrational_spectrum.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.258976 esse-2023.6.20.post0/example/properties_directory/scalar/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/scalar/electron_affinity.json
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/scalar/fermi_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/scalar/formation_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/scalar/ionization_potential.json
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/scalar/pressure.json
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/scalar/reaction_energy_barrier.json
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/scalar/surface_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/scalar/total_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/scalar/total_force.json
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/scalar/valence_band_offset.json
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/scalar/zero_point_energy.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.262976 esse-2023.6.20.post0/example/properties_directory/structural/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/structural/atomic_forces.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.262976 esse-2023.6.20.post0/example/properties_directory/structural/basis/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/structural/basis/atomic_constraints.json
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/structural/basis/atomic_coordinate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/structural/basis/atomic_coordinates.json
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/structural/basis/atomic_element.json
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/structural/basis/bonds.json
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/structural/basis.json
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/structural/density.json
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/structural/elemental_ratio.json
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/structural/inchi.json
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/structural/inchi_key.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.262976 esse-2023.6.20.post0/example/properties_directory/structural/lattice/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/structural/lattice/lattice_bravais.json
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/structural/lattice/lattice_vectors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/structural/lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/structural/magnetic_moments.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/structural/molecular_pattern.json
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/structural/p-norm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/structural/symmetry.json
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/structural/volume.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.230975 esse-2023.6.20.post0/example/properties_directory/workflow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.262976 esse-2023.6.20.post0/example/properties_directory/workflow/convergence/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/workflow/convergence/electronic.json
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/workflow/convergence/ionic.json
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/properties_directory/workflow/convergence/kpoint.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.262976 esse-2023.6.20.post0/example/property/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/property/best.json
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/property/raw.json
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/property/refined.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.262976 esse-2023.6.20.post0/example/software/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/software/application.json
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/software/executable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/software/flavor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/software/template.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.234976 esse-2023.6.20.post0/example/software_directory/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.262976 esse-2023.6.20.post0/example/software_directory/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/software_directory/ml/exabyteml.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.230975 esse-2023.6.20.post0/example/software_directory/ml/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.262976 esse-2023.6.20.post0/example/software_directory/ml/unit/execution/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.262976 esse-2023.6.20.post0/example/software_directory/ml/unit/execution/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/software_directory/ml/unit/execution/evaluate/cross-validate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/software_directory/ml/unit/execution/initialize.json
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/software_directory/ml/unit/execution/score.json
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/software_directory/ml/unit/execution/train.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.234976 esse-2023.6.20.post0/example/software_directory/ml/unit/processing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.262976 esse-2023.6.20.post0/example/software_directory/ml/unit/processing/data_transformation/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/software_directory/ml/unit/processing/data_transformation/manipulation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.262976 esse-2023.6.20.post0/example/software_directory/ml/unit/processing/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/software_directory/ml/unit/processing/feature_selection/filter_based.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.262976 esse-2023.6.20.post0/example/software_directory/modeling/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.262976 esse-2023.6.20.post0/example/software_directory/modeling/espresso/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/software_directory/modeling/espresso/arguments.json
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/software_directory/modeling/espresso.json
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/software_directory/modeling/nwchem.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.266976 esse-2023.6.20.post0/example/software_directory/modeling/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/software_directory/modeling/unit/execution.json
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/software_directory/modeling/vasp.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.266976 esse-2023.6.20.post0/example/software_directory/scripting/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/software_directory/scripting/jupyter-lab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/software_directory/scripting/python.json
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/software_directory/scripting/shell.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.266976 esse-2023.6.20.post0/example/software_directory/scripting/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/software_directory/scripting/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.266976 esse-2023.6.20.post0/example/system/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/system/_material.json
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/system/_parent_job.json
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/system/_project.json
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/system/creator.json
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/system/entity_reference.json
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/system/file_source.json
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/system/message.json
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/system/owner.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.266976 esse-2023.6.20.post0/example/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/workflow/new_subworkflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/workflow/subworkflow.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.266976 esse-2023.6.20.post0/example/workflow/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/workflow/unit/assignment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/workflow/unit/condition.json
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/workflow/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.266976 esse-2023.6.20.post0/example/workflow/unit/input/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/workflow/unit/input/_inputItemScope.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.266976 esse-2023.6.20.post0/example/workflow/unit/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/workflow/unit/io/api.json
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/workflow/unit/io/db.json
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/workflow/unit/io/object_storage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/workflow/unit/io.json
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/workflow/unit/map.json
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/workflow/unit/processing.json
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/workflow/unit/reduce.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.266976 esse-2023.6.20.post0/example/workflow/unit/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/workflow/unit/runtime/runtime_items.json
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/workflow/unit.json
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/example/workflow.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.266976 esse-2023.6.20.post0/manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/manifest/dft_unit_functionals.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/manifest/functional_lookup_table.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/manifest/models.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/manifest/properties.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/npmignore
+-rw-r--r--   0 runner    (1001) docker     (123)   269811 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      340 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/refactor.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/requirements-dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1489 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/run-tests.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.270976 esse-2023.6.20.post0/schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.270976 esse-2023.6.20.post0/schema/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.270976 esse-2023.6.20.post0/schema/core/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/abstract/2d_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/abstract/2d_plot.json
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/abstract/3d_grid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/abstract/3d_tensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/abstract/3d_vector_basis.json
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/abstract/point.json
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/abstract/vector.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.270976 esse-2023.6.20.post0/schema/core/primitive/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/primitive/1d_data_series.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/primitive/3d_lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/primitive/array_of_3_booleans.json
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/primitive/array_of_3_numbers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/primitive/array_of_ids.json
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/primitive/array_of_numbers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/primitive/array_of_strings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/primitive/axis.json
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/primitive/scalar.json
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/primitive/slugified_entry.json
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/primitive/slugified_entry_or_slug.json
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/primitive/string.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.270976 esse-2023.6.20.post0/schema/core/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/reference/exabyte.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.270976 esse-2023.6.20.post0/schema/core/reference/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/reference/experiment/condition.json
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/reference/experiment/location.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/reference/experiment.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.270976 esse-2023.6.20.post0/schema/core/reference/literature/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/reference/literature/name.json
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/reference/literature/pages.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/reference/literature.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.270976 esse-2023.6.20.post0/schema/core/reference/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/reference/modeling/exabyte.json
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/reference/modeling.json
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/reference.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.270976 esse-2023.6.20.post0/schema/core/reusable/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/reusable/atomic_scalars.json
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/reusable/atomic_strings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/reusable/atomic_vectors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/reusable/band_gap.json
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/reusable/energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/reusable/file_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/core/reusable/object_storage_container_data.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.274976 esse-2023.6.20.post0/schema/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/definitions/units.json
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/element.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.274976 esse-2023.6.20.post0/schema/in_memory_entity/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/in_memory_entity/base.json
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/in_memory_entity/defaultable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/in_memory_entity/named.json
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/in_memory_entity/named_defaultable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/in_memory_entity/named_defaultable_has_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/in_memory_entity/named_defaultable_runtime_items.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.274976 esse-2023.6.20.post0/schema/job/
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/job/compute.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/job.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.274976 esse-2023.6.20.post0/schema/material/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/material/conventional.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/material.json
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/method.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.274976 esse-2023.6.20.post0/schema/methods_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/methods_directory/local-orbital.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.234976 esse-2023.6.20.post0/schema/methods_directory/local_orbital/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.274976 esse-2023.6.20.post0/schema/methods_directory/local_orbital/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/methods_directory/local_orbital/definitions/basis_sets.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.274976 esse-2023.6.20.post0/schema/methods_directory/pseudopotential/
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/methods_directory/pseudopotential/dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.274976 esse-2023.6.20.post0/schema/methods_directory/pseudopotential/file/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/methods_directory/pseudopotential/file/energy_cutoff.json
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/methods_directory/pseudopotential/file/exchange_correlation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/methods_directory/pseudopotential/file/radii.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/methods_directory/pseudopotential/file.json
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/methods_directory/pseudopotential/precision.json
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/methods_directory/pseudopotential.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.274976 esse-2023.6.20.post0/schema/methods_directory/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/methods_directory/regression/data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/methods_directory/regression/data_per_feature.json
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/methods_directory/regression/dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.274976 esse-2023.6.20.post0/schema/methods_directory/regression/kernel_ridge/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/methods_directory/regression/kernel_ridge/data_per_property.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.274976 esse-2023.6.20.post0/schema/methods_directory/regression/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/methods_directory/regression/linear/data_per_property.json
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/methods_directory/regression/precision.json
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/methods_directory/regression/precision_per_property.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/methods_directory/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/methods_directory/unknown.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.274976 esse-2023.6.20.post0/schema/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/model/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/model/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/model/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/model.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.274976 esse-2023.6.20.post0/schema/models_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/definitions.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.274976 esse-2023.6.20.post0/schema/models_directory/pb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.278976 esse-2023.6.20.post0/schema/models_directory/pb/qm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.278976 esse-2023.6.20.post0/schema/models_directory/pb/qm/abin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.278976 esse-2023.6.20.post0/schema/models_directory/pb/qm/abin/configuration_interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/abin/configuration_interaction/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/abin/configuration_interaction/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/abin/configuration_interaction/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/abin/configuration_interaction/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/abin/configuration_interaction.json
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/abin/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/abin/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/abin.json
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/definitions.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.278976 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/
+-rw-r--r--   0 runner    (1001) docker     (123)    36659 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dft_unit_functionals.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dft_unit_functionals_proto.json
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dispersion_model.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.278976 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/dft_d.json
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/exchange_dipole.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.278976 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_abin.json
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_empirical.json
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_abin.json
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_empirical.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/many_body_dispersion.json
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/non_local_correlation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/tkatchenko_scheffler.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.278976 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/functional/component.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.278976 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/functional/components_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/functional/components_directory/dispersion_correction.json
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/functional/components_directory/exact_exchange.json
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional_gga.json
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional_lda.json
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional_mgga.json
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/functional/components_directory/mp2_correlation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/functional/components_directory/range_separated_exchange.json
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/functional/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/functional/local_functional_components.json
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/functional.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.282976 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/definitions.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.282976 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.282976 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/gga/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/gga/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/gga/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/gga/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/gga/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/gga/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/gga.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.282976 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.282976 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/lda/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/lda/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/lda/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/lda/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/lda/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/lda/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/lda.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.282976 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/mgga.json
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/dft.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.282976 esse-2023.6.20.post0/schema/models_directory/pb/qm/semp/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/semp/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/semp/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/semp/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/semp/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/semp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb/qm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/pb.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.282976 esse-2023.6.20.post0/schema/models_directory/st/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.282976 esse-2023.6.20.post0/schema/models_directory/st/det/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/st/det/ml.json
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/st/det.json
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/st.json
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/models_directory/unknown.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/new_model.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/project.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.282976 esse-2023.6.20.post0/schema/properties_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/derived_properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/electronic_configuration.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.286976 esse-2023.6.20.post0/schema/properties_directory/elemental/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/elemental/atomic_radius.json
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/elemental/electronegativity.json
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/elemental/ionization_potential.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.286976 esse-2023.6.20.post0/schema/properties_directory/non-scalar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/non-scalar/average_potential_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/non-scalar/band_gaps.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/non-scalar/band_structure.json
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/non-scalar/charge_density_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/non-scalar/density_of_states.json
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/non-scalar/file_content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/non-scalar/phonon_dispersions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/non-scalar/phonon_dos.json
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/non-scalar/potential_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/non-scalar/reaction_energy_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/non-scalar/stress_tensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/non-scalar/total_energy_contributions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/non-scalar/vibrational_spectrum.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.286976 esse-2023.6.20.post0/schema/properties_directory/scalar/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/scalar/electron_affinity.json
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/scalar/fermi_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/scalar/formation_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/scalar/ionization_potential.json
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/scalar/pressure.json
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/scalar/reaction_energy_barrier.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/scalar/surface_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/scalar/total_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/scalar/total_force.json
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/scalar/valence_band_offset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/scalar/zero_point_energy.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.286976 esse-2023.6.20.post0/schema/properties_directory/structural/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/structural/atomic_forces.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.290976 esse-2023.6.20.post0/schema/properties_directory/structural/basis/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/structural/basis/atomic_constraints.json
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/structural/basis/atomic_coordinate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/structural/basis/atomic_coordinates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/structural/basis/atomic_element.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/structural/basis/bonds.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/structural/basis.json
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/structural/density.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/structural/elemental_ratio.json
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/structural/inchi.json
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/structural/inchi_key.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.290976 esse-2023.6.20.post0/schema/properties_directory/structural/lattice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/structural/lattice/lattice_bravais.json
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/structural/lattice/lattice_vectors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/structural/lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/structural/magnetic_moments.json
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/structural/molecular_pattern.json
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/structural/p-norm.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.290976 esse-2023.6.20.post0/schema/properties_directory/structural/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/structural/patterns/functional_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/structural/patterns/ring.json
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/structural/patterns/special_bond.json
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/structural/symmetry.json
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/structural/volume.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.238976 esse-2023.6.20.post0/schema/properties_directory/workflow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.290976 esse-2023.6.20.post0/schema/properties_directory/workflow/convergence/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/workflow/convergence/electronic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/workflow/convergence/ionic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/properties_directory/workflow/convergence/kpoint.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.290976 esse-2023.6.20.post0/schema/property/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/property/best.json
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/property/raw.json
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/property/refined.json
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/property/source.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.290976 esse-2023.6.20.post0/schema/software/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software/application.json
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software/executable.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software/flavor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software/template.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.238976 esse-2023.6.20.post0/schema/software_directory/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.290976 esse-2023.6.20.post0/schema/software_directory/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software_directory/ml/exabyteml.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.290976 esse-2023.6.20.post0/schema/software_directory/ml/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.290976 esse-2023.6.20.post0/schema/software_directory/ml/unit/execution/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.290976 esse-2023.6.20.post0/schema/software_directory/ml/unit/execution/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software_directory/ml/unit/execution/evaluate/cross-validate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software_directory/ml/unit/execution/initialize.json
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software_directory/ml/unit/execution/score.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software_directory/ml/unit/execution/train.json
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software_directory/ml/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.290976 esse-2023.6.20.post0/schema/software_directory/ml/unit/processing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.290976 esse-2023.6.20.post0/schema/software_directory/ml/unit/processing/data_transformation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software_directory/ml/unit/processing/data_transformation/manipulation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software_directory/ml/unit/processing/data_transformation.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.290976 esse-2023.6.20.post0/schema/software_directory/ml/unit/processing/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software_directory/ml/unit/processing/feature_selection/filter_based.json
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software_directory/ml/unit/processing/feature_selection.json
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software_directory/ml/unit/processing.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.290976 esse-2023.6.20.post0/schema/software_directory/modeling/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.290976 esse-2023.6.20.post0/schema/software_directory/modeling/espresso/
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software_directory/modeling/espresso/arguments.json
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software_directory/modeling/espresso.json
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software_directory/modeling/nwchem.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.290976 esse-2023.6.20.post0/schema/software_directory/modeling/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software_directory/modeling/unit/execution.json
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software_directory/modeling/vasp.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.290976 esse-2023.6.20.post0/schema/software_directory/scripting/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software_directory/scripting/jupyter-lab.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software_directory/scripting/python.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software_directory/scripting/shell.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.290976 esse-2023.6.20.post0/schema/software_directory/scripting/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/software_directory/scripting/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.294976 esse-2023.6.20.post0/schema/system/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/_material.json
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/_parent_job.json
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/_project.json
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/bankable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/creator.json
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/creator_account.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/database_source.json
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/defaultable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/description.json
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/entity_reference.json
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/file_source.json
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/history.json
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/in_set.json
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/is_multi_material.json
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/is_outdated.json
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/job_extended.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/message.json
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/name.json
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/owner.json
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/schema_version.json
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/scope.json
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/set.json
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/sharing.json
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/soft_removable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/status.json
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/timestampable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/system/use_values.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.294976 esse-2023.6.20.post0/schema/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow/base_flow.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow/new_subworkflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow/subworkflow.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.294976 esse-2023.6.20.post0/schema/workflow/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow/unit/assertion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow/unit/assignment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow/unit/condition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.298976 esse-2023.6.20.post0/schema/workflow/unit/input/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow/unit/input/_input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow/unit/input/_inputItem.json
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow/unit/input/_inputItemId.json
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow/unit/input/_inputItemScope.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.298976 esse-2023.6.20.post0/schema/workflow/unit/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow/unit/io/api.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow/unit/io/db.json
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow/unit/io/object_storage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow/unit/io.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow/unit/map.json
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow/unit/processing.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow/unit/reduce.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.298976 esse-2023.6.20.post0/schema/workflow/unit/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow/unit/runtime/_runtime_item_full_object.json
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow/unit/runtime/_runtime_item_name_object.json
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow/unit/runtime/_runtime_item_string.json
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow/unit/runtime/runtime_item.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow/unit/runtime/runtime_items.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow/unit.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/schema/workflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 02:24:27.350976 esse-2023.6.20.post0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.238976 esse-2023.6.20.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.238976 esse-2023.6.20.post0/src/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.298976 esse-2023.6.20.post0/src/js/esse/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/js/esse/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/js/esse/settings.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.298976 esse-2023.6.20.post0/src/js/esse/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/js/esse/tests/validate.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/js/esse/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.298976 esse-2023.6.20.post0/src/js/json_include/
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/js/json_include/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/js/json_include/settings.js
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/js/json_include/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.298976 esse-2023.6.20.post0/src/js/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/js/scripts/setSchemaIds.mjs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.238976 esse-2023.6.20.post0/src/py/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.298976 esse-2023.6.20.post0/src/py/esse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-20 02:24:27.000000 esse-2023.6.20.post0/src/py/esse/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.242976 esse-2023.6.20.post0/src/py/esse/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.298976 esse-2023.6.20.post0/src/py/esse/data/example/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.298976 esse-2023.6.20.post0/src/py/esse/data/example/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.302976 esse-2023.6.20.post0/src/py/esse/data/example/core/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/abstract/2d_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/abstract/2d_plot.json
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/abstract/3d_grid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/abstract/3d_tensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/abstract/3d_vector_basis.json
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/abstract/point.json
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/abstract/vector.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.302976 esse-2023.6.20.post0/src/py/esse/data/example/core/primitive/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/primitive/1d_data_series.json
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/primitive/3d_lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/primitive/array_of_3_booleans.json
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/primitive/array_of_3_numbers.json
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/primitive/array_of_ids.json
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/primitive/axis.json
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/primitive/scalar.json
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/primitive/string.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.302976 esse-2023.6.20.post0/src/py/esse/data/example/core/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.302976 esse-2023.6.20.post0/src/py/esse/data/example/core/reference/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/reference/experiment/condition.json
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/reference/experiment/location.json
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/reference/experiment.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.302976 esse-2023.6.20.post0/src/py/esse/data/example/core/reference/literature/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/reference/literature/name.json
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/reference/literature/pages.json
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/reference/literature.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.302976 esse-2023.6.20.post0/src/py/esse/data/example/core/reference/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/reference/modeling/exabyte.json
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/reference/modeling.json
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/reference.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.302976 esse-2023.6.20.post0/src/py/esse/data/example/core/reusable/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/reusable/atomic_vectors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/reusable/band_gap.json
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/reusable/energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/reusable/file_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/core/reusable/object_storage_container_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/element.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.302976 esse-2023.6.20.post0/src/py/esse/data/example/job/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/job/compute.json
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/job.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/material.json
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/method.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.302976 esse-2023.6.20.post0/src/py/esse/data/example/methods_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/methods_directory/local-orbital.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.302976 esse-2023.6.20.post0/src/py/esse/data/example/methods_directory/pseudopotential/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/methods_directory/pseudopotential/dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.302976 esse-2023.6.20.post0/src/py/esse/data/example/methods_directory/pseudopotential/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/methods_directory/pseudopotential/file/energy_cutoff.json
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/methods_directory/pseudopotential/file/exchange_correlation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/methods_directory/pseudopotential/file/radii.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/methods_directory/pseudopotential/file.json
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/methods_directory/pseudopotential/precision.json
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/methods_directory/pseudopotential.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.306976 esse-2023.6.20.post0/src/py/esse/data/example/methods_directory/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/methods_directory/regression/data_per_feature.json
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/methods_directory/regression/dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.306976 esse-2023.6.20.post0/src/py/esse/data/example/methods_directory/regression/kernel_ridge/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/methods_directory/regression/kernel_ridge/data_per_property.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.306976 esse-2023.6.20.post0/src/py/esse/data/example/methods_directory/regression/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/methods_directory/regression/linear/data_per_property.json
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/methods_directory/regression/precision.json
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/methods_directory/regression/precision_per_property.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/methods_directory/regression.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.306976 esse-2023.6.20.post0/src/py/esse/data/example/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/model/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/model.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.242976 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.242976 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.306976 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.306976 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/abin/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/abin/configuration_interaction.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.306976 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.306976 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/dispersion_models_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/dispersion_models_directory/dft_d.json
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/dispersion_models_directory/exchange_dipole.json
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/dispersion_models_directory/many_body_dispersion.json
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/dispersion_models_directory/non_local_correlation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/dispersion_models_directory/tkatchenko_scheffler.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.306976 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/functional/component.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.306976 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/functional/components_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/functional/components_directory/local_functional_lda.json
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/functional.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.306976 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.306976 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/double_hybrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.306976 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/gga/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/gga/functional.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.306976 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/hybrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/hybrid/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.306976 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/lda/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/lda/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/lda.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.306976 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/mgga/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/mgga/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/semp.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.242976 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/st/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.306976 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/st/det/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/models_directory/st/det/ml.json
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/new_model.json
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/project.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.306976 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/electronic_configuration.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.306976 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/elemental/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/elemental/atomic_radius.json
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/elemental/electronegativity.json
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/elemental/ionization_potential.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.310976 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/non-scalar/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/non-scalar/band_gaps.json
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/non-scalar/band_structure.json
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/non-scalar/charge_density_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/non-scalar/density_of_states.json
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/non-scalar/file_content.json
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/non-scalar/phonon_dispersions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/non-scalar/phonon_dos.json
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/non-scalar/potential_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/non-scalar/reaction_energy_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/non-scalar/stress_tensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/non-scalar/total_energy_contributions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/non-scalar/vibrational_spectrum.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.310976 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/scalar/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/scalar/electron_affinity.json
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/scalar/fermi_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/scalar/formation_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/scalar/ionization_potential.json
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/scalar/pressure.json
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/scalar/reaction_energy_barrier.json
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/scalar/surface_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/scalar/total_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/scalar/total_force.json
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/scalar/valence_band_offset.json
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/scalar/zero_point_energy.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.310976 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/structural/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/structural/atomic_forces.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.310976 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/structural/basis/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/structural/basis/atomic_constraints.json
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/structural/basis/atomic_coordinate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/structural/basis/atomic_coordinates.json
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/structural/basis/atomic_element.json
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/structural/basis/bonds.json
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/structural/basis.json
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/structural/density.json
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/structural/elemental_ratio.json
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/structural/inchi.json
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/structural/inchi_key.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.310976 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/structural/lattice/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/structural/lattice/lattice_bravais.json
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/structural/lattice/lattice_vectors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/structural/lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/structural/magnetic_moments.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/structural/molecular_pattern.json
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/structural/p-norm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/structural/symmetry.json
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/structural/volume.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.242976 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/workflow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.310976 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/workflow/convergence/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/workflow/convergence/electronic.json
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/workflow/convergence/ionic.json
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/workflow/convergence/kpoint.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.310976 esse-2023.6.20.post0/src/py/esse/data/example/property/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/property/best.json
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/property/raw.json
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/property/refined.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.314976 esse-2023.6.20.post0/src/py/esse/data/example/software/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/software/application.json
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/software/executable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/software/flavor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/software/template.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.242976 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.314976 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/ml/exabyteml.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.242976 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/ml/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.314976 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/ml/unit/execution/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.314976 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/ml/unit/execution/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/ml/unit/execution/evaluate/cross-validate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/ml/unit/execution/initialize.json
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/ml/unit/execution/score.json
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/ml/unit/execution/train.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.242976 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/ml/unit/processing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.314976 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/ml/unit/processing/data_transformation/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/ml/unit/processing/data_transformation/manipulation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.314976 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/ml/unit/processing/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/ml/unit/processing/feature_selection/filter_based.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.314976 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/modeling/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.314976 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/modeling/espresso/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/modeling/espresso/arguments.json
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/modeling/espresso.json
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/modeling/nwchem.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.314976 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/modeling/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/modeling/unit/execution.json
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/modeling/vasp.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.314976 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/scripting/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/scripting/jupyter-lab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/scripting/python.json
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/scripting/shell.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.314976 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/scripting/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/software_directory/scripting/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.314976 esse-2023.6.20.post0/src/py/esse/data/example/system/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/system/_material.json
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/system/_parent_job.json
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/system/_project.json
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/system/creator.json
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/system/entity_reference.json
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/system/file_source.json
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/system/message.json
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/system/owner.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.314976 esse-2023.6.20.post0/src/py/esse/data/example/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/workflow/new_subworkflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/workflow/subworkflow.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.318976 esse-2023.6.20.post0/src/py/esse/data/example/workflow/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/workflow/unit/assignment.json
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/workflow/unit/condition.json
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/workflow/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.318976 esse-2023.6.20.post0/src/py/esse/data/example/workflow/unit/input/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/workflow/unit/input/_inputItemScope.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.318976 esse-2023.6.20.post0/src/py/esse/data/example/workflow/unit/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/workflow/unit/io/api.json
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/workflow/unit/io/db.json
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/workflow/unit/io/object_storage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/workflow/unit/io.json
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/workflow/unit/map.json
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/workflow/unit/processing.json
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/workflow/unit/reduce.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.318976 esse-2023.6.20.post0/src/py/esse/data/example/workflow/unit/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/workflow/unit/runtime/runtime_items.json
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/workflow/unit.json
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/example/workflow.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.318976 esse-2023.6.20.post0/src/py/esse/data/manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/manifest/dft_unit_functionals.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/manifest/functional_lookup_table.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/manifest/models.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/manifest/properties.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.318976 esse-2023.6.20.post0/src/py/esse/data/schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.318976 esse-2023.6.20.post0/src/py/esse/data/schema/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.318976 esse-2023.6.20.post0/src/py/esse/data/schema/core/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/abstract/2d_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/abstract/2d_plot.json
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/abstract/3d_grid.json
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/abstract/3d_tensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/abstract/3d_vector_basis.json
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/abstract/point.json
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/abstract/vector.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.322976 esse-2023.6.20.post0/src/py/esse/data/schema/core/primitive/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/primitive/1d_data_series.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/primitive/3d_lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/primitive/array_of_3_booleans.json
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/primitive/array_of_3_numbers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/primitive/array_of_ids.json
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/primitive/array_of_numbers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/primitive/array_of_strings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/primitive/axis.json
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/primitive/scalar.json
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/primitive/slugified_entry.json
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/primitive/slugified_entry_or_slug.json
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/primitive/string.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.322976 esse-2023.6.20.post0/src/py/esse/data/schema/core/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/reference/exabyte.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.322976 esse-2023.6.20.post0/src/py/esse/data/schema/core/reference/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/reference/experiment/condition.json
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/reference/experiment/location.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/reference/experiment.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.322976 esse-2023.6.20.post0/src/py/esse/data/schema/core/reference/literature/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/reference/literature/name.json
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/reference/literature/pages.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/reference/literature.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.322976 esse-2023.6.20.post0/src/py/esse/data/schema/core/reference/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/reference/modeling/exabyte.json
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/reference/modeling.json
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/reference.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.322976 esse-2023.6.20.post0/src/py/esse/data/schema/core/reusable/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/reusable/atomic_scalars.json
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/reusable/atomic_strings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/reusable/atomic_vectors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/reusable/band_gap.json
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/reusable/energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/reusable/file_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/core/reusable/object_storage_container_data.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.322976 esse-2023.6.20.post0/src/py/esse/data/schema/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/definitions/units.json
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/element.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.322976 esse-2023.6.20.post0/src/py/esse/data/schema/in_memory_entity/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/in_memory_entity/base.json
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/in_memory_entity/defaultable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/in_memory_entity/named.json
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/in_memory_entity/named_defaultable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/in_memory_entity/named_defaultable_has_metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/in_memory_entity/named_defaultable_runtime_items.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.322976 esse-2023.6.20.post0/src/py/esse/data/schema/job/
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/job/compute.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/job.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.322976 esse-2023.6.20.post0/src/py/esse/data/schema/material/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/material/conventional.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/material.json
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/method.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.322976 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/local-orbital.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.246976 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/local_orbital/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.322976 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/local_orbital/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/local_orbital/definitions/basis_sets.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.322976 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/pseudopotential/
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/pseudopotential/dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.326976 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file/energy_cutoff.json
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file/exchange_correlation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file/radii.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file.json
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/pseudopotential/precision.json
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/pseudopotential.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.326976 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/regression/data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/regression/data_per_feature.json
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/regression/dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.326976 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/regression/kernel_ridge/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/regression/kernel_ridge/data_per_property.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.326976 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/regression/linear/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/regression/linear/data_per_property.json
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/regression/precision.json
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/regression/precision_per_property.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/unknown.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.326976 esse-2023.6.20.post0/src/py/esse/data/schema/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/model/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/model/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/model/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/model.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.326976 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/definitions.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.326976 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.326976 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.326976 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.326976 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction.json
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/abin.json
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/definitions.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.326976 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/
+-rw-r--r--   0 runner    (1001) docker     (123)    36659 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dft_unit_functionals.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dft_unit_functionals_proto.json
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_model.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.330976 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/dft_d.json
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/exchange_dipole.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.330976 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_abin.json
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_empirical.json
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_abin.json
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_empirical.json
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/many_body_dispersion.json
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/non_local_correlation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/tkatchenko_scheffler.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.330976 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/component.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.330976 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/dispersion_correction.json
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/exact_exchange.json
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional_gga.json
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional_lda.json
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/local_functional_mgga.json
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/mp2_correlation.json
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/range_separated_exchange.json
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/local_functional_components.json
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.330976 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/definitions.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.330976 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.334976 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.334976 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.334976 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.334976 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/functional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga.json
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.334976 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/semp/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/semp/augmentations.json
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/semp/definitions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/semp/modifiers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/semp/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/semp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm.json
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.334976 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/st/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.334976 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/st/det/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/st/det/ml.json
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/st/det.json
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/st.json
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/unknown.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/new_model.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/project.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.334976 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/derived_properties.json
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/electronic_configuration.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.334976 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/elemental/
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/elemental/atomic_radius.json
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/elemental/electronegativity.json
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/elemental/ionization_potential.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.338976 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/average_potential_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/band_gaps.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/band_structure.json
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/charge_density_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/density_of_states.json
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/file_content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/phonon_dispersions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/phonon_dos.json
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/potential_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/reaction_energy_profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/stress_tensor.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/total_energy_contributions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/vibrational_spectrum.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.338976 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/scalar/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/scalar/electron_affinity.json
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/scalar/fermi_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/scalar/formation_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/scalar/ionization_potential.json
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/scalar/pressure.json
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/scalar/reaction_energy_barrier.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/scalar/surface_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/scalar/total_energy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/scalar/total_force.json
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/scalar/valence_band_offset.json
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/scalar/zero_point_energy.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.338976 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/atomic_forces.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.338976 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/basis/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/basis/atomic_constraints.json
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/basis/atomic_coordinate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/basis/atomic_coordinates.json
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/basis/atomic_element.json
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/basis/bonds.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/basis.json
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/density.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/elemental_ratio.json
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/inchi.json
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/inchi_key.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.338976 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/lattice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/lattice/lattice_bravais.json
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/lattice/lattice_vectors.json
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/magnetic_moments.json
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/molecular_pattern.json
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/p-norm.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.342976 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/patterns/
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/patterns/functional_group.json
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/patterns/ring.json
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/patterns/special_bond.json
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/symmetry.json
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/volume.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.246976 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/workflow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.342976 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/electronic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/ionic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/kpoint.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.342976 esse-2023.6.20.post0/src/py/esse/data/schema/property/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/property/best.json
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/property/raw.json
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/property/refined.json
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/property/source.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.342976 esse-2023.6.20.post0/src/py/esse/data/schema/software/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software/application.json
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software/executable.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software/flavor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software/template.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.246976 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.342976 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/exabyteml.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.342976 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.342976 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.342976 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/evaluate/cross-validate.json
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/initialize.json
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/score.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/train.json
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.342976 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.342976 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/data_transformation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/data_transformation/manipulation.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/data_transformation.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.342976 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/feature_selection/filter_based.json
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/feature_selection.json
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/unit/processing.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.342976 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/modeling/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.342976 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/modeling/espresso/
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/modeling/espresso/arguments.json
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/modeling/espresso.json
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/modeling/nwchem.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.342976 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/modeling/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/modeling/unit/execution.json
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/modeling/vasp.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.342976 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/scripting/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/scripting/jupyter-lab.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/scripting/python.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/scripting/shell.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.342976 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/scripting/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/scripting/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.346976 esse-2023.6.20.post0/src/py/esse/data/schema/system/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/_material.json
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/_parent_job.json
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/_project.json
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/bankable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/creator.json
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/creator_account.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/database_source.json
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/defaultable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/description.json
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/entity_reference.json
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/file_source.json
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/history.json
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/in_set.json
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/is_multi_material.json
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/is_outdated.json
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/job_extended.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/message.json
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/name.json
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/owner.json
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/schema_version.json
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/scope.json
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/set.json
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/sharing.json
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/soft_removable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/status.json
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/timestampable.json
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/system/use_values.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.346976 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/base_flow.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/new_subworkflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/subworkflow.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.346976 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/assertion.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/assignment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/condition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/execution.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.350976 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/input/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/input/_input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/input/_inputItem.json
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/input/_inputItemId.json
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/input/_inputItemScope.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.350976 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/io/api.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/io/db.json
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/io/object_storage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/io.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/map.json
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/processing.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/reduce.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.350976 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/runtime/_runtime_item_full_object.json
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/runtime/_runtime_item_name_object.json
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/runtime/_runtime_item_string.json
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/runtime/runtime_item.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/runtime/runtime_items.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/data/schema/workflow.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/functionals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.350976 esse-2023.6.20.post0/src/py/esse/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/tests/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-20 02:24:06.000000 esse-2023.6.20.post0/src/py/esse/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:24:27.298976 esse-2023.6.20.post0/src/py/esse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-20 02:24:27.000000 esse-2023.6.20.post0/src/py/esse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    55972 2023-06-20 02:24:27.000000 esse-2023.6.20.post0/src/py/esse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 02:24:27.000000 esse-2023.6.20.post0/src/py/esse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 02:24:27.000000 esse-2023.6.20.post0/src/py/esse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-20 02:24:27.000000 esse-2023.6.20.post0/src/py/esse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 02:24:27.000000 esse-2023.6.20.post0/src/py/esse.egg-info/top_level.txt
```

### Comparing `esse-2023.6.16.post0/.github/workflows/cicd.yml` & `esse-2023.6.20.post0/.github/workflows/cicd.yml`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,37 @@
 on: [push]
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.event.pull_request.number || github.ref }}
   cancel-in-progress: true
 
 jobs:
+  run-py-linter:
+    runs-on: ubuntu-20.04
+    strategy:
+      matrix:
+        python-version: [3.8.6]
+
+    steps:
+      - name: Checkout this repository
+        uses: actions/checkout@v3
+        with:
+          lfs: true
+
+      - name: Checkout actions repository
+        uses: actions/checkout@v3
+        with:
+          repository: Exabyte-io/actions
+          token: ${{ secrets.BOT_GITHUB_TOKEN }}
+          path: actions
+
+      - name: Run ruff linter
+        uses: ./actions/py/lint
+        with:
+          python-version: ${{ matrix.python-version }}
 
   run-py-tests:
     runs-on: ubuntu-20.04
     strategy:
       matrix:
         python-version: [3.6, 3.7, 3.8]
 
@@ -59,15 +82,15 @@
       
       - name: Run JS tests
         uses: ./actions/js/test
         with:
           node-version: ${{ matrix.node-version }}
 
   publish-js-package:
-    needs: [run-py-tests, run-js-tests]
+    needs: [run-py-linter, run-py-tests, run-js-tests]
     runs-on: ubuntu-latest
     if: github.ref_name == 'dev'
 
     steps:
       - name: Checkout this repository
         uses: actions/checkout@v2
         with:
```

### Comparing `esse-2023.6.16.post0/.gitignore` & `esse-2023.6.20.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/LICENSE.md` & `esse-2023.6.20.post0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/PKG-INFO` & `esse-2023.6.20.post0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esse
-Version: 2023.6.16.post0
+Version: 2023.6.20.post0
 Summary: Exabyte Source of Schemas and Examples
 Home-page: https://github.com/Exabyte-io/exabyte-esse
 Author: Exabyte Inc.
 Author-email: info@exabyte.io
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `esse-2023.6.16.post0/README.md` & `esse-2023.6.20.post0/README.md`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/job/compute.json` & `esse-2023.6.20.post0/example/job/compute.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/job.json` & `esse-2023.6.20.post0/example/job.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/material.json` & `esse-2023.6.20.post0/example/material.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/methods_directory/pseudopotential/file.json` & `esse-2023.6.20.post0/example/methods_directory/pseudopotential/file.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/methods_directory/regression.json` & `esse-2023.6.20.post0/example/methods_directory/regression.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/models_directory/pb/qm/abin/configuration_interaction.json` & `esse-2023.6.20.post0/example/models_directory/pb/qm/abin/configuration_interaction.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json` & `esse-2023.6.20.post0/example/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json` & `esse-2023.6.20.post0/example/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/models_directory/pb/qm/dft/ksdft/hybrid/functional.json` & `esse-2023.6.20.post0/example/models_directory/pb/qm/dft/ksdft/hybrid/functional.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json` & `esse-2023.6.20.post0/example/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/models_directory/pb/qm/dft/ksdft/lda.json` & `esse-2023.6.20.post0/example/models_directory/pb/qm/dft/ksdft/lda.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/models_directory/pb/qm/dft/ksdft.json` & `esse-2023.6.20.post0/example/models_directory/pb/qm/dft/ksdft.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/properties_directory/non-scalar/band_structure.json` & `esse-2023.6.20.post0/example/properties_directory/non-scalar/band_structure.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/properties_directory/non-scalar/density_of_states.json` & `esse-2023.6.20.post0/example/properties_directory/non-scalar/density_of_states.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/properties_directory/non-scalar/phonon_dispersions.json` & `esse-2023.6.20.post0/example/properties_directory/non-scalar/phonon_dispersions.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/properties_directory/non-scalar/phonon_dos.json` & `esse-2023.6.20.post0/example/properties_directory/non-scalar/phonon_dos.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/properties_directory/non-scalar/potential_profile.json` & `esse-2023.6.20.post0/example/properties_directory/non-scalar/potential_profile.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/properties_directory/non-scalar/reaction_energy_profile.json` & `esse-2023.6.20.post0/example/properties_directory/non-scalar/reaction_energy_profile.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/properties_directory/non-scalar/total_energy_contributions.json` & `esse-2023.6.20.post0/example/properties_directory/non-scalar/total_energy_contributions.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/properties_directory/structural/molecular_pattern.json` & `esse-2023.6.20.post0/example/properties_directory/structural/molecular_pattern.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/software_directory/ml/unit/execution/train.json` & `esse-2023.6.20.post0/example/software_directory/ml/unit/execution/train.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json` & `esse-2023.6.20.post0/example/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/system/file_source.json` & `esse-2023.6.20.post0/example/system/file_source.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/workflow/unit/execution.json` & `esse-2023.6.20.post0/example/workflow/unit/execution.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/workflow/unit/io/api.json` & `esse-2023.6.20.post0/example/workflow/unit/io/api.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/workflow/unit/io.json` & `esse-2023.6.20.post0/example/workflow/unit/io.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/example/workflow.json` & `esse-2023.6.20.post0/example/workflow.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/manifest/dft_unit_functionals.yaml` & `esse-2023.6.20.post0/manifest/dft_unit_functionals.yaml`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/manifest/functional_lookup_table.yaml` & `esse-2023.6.20.post0/manifest/functional_lookup_table.yaml`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/manifest/models.yaml` & `esse-2023.6.20.post0/manifest/models.yaml`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/manifest/properties.yaml` & `esse-2023.6.20.post0/manifest/properties.yaml`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/package-lock.json` & `esse-2023.6.20.post0/package-lock.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/package.json` & `esse-2023.6.20.post0/package.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/run-tests.sh` & `esse-2023.6.20.post0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/core/abstract/2d_plot.json` & `esse-2023.6.20.post0/schema/core/abstract/2d_plot.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/core/abstract/3d_vector_basis.json` & `esse-2023.6.20.post0/schema/core/abstract/3d_vector_basis.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/core/primitive/3d_lattice.json` & `esse-2023.6.20.post0/schema/core/primitive/3d_lattice.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/core/primitive/slugified_entry.json` & `esse-2023.6.20.post0/schema/core/primitive/slugified_entry.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/core/reference/exabyte.json` & `esse-2023.6.20.post0/schema/core/reference/exabyte.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/core/reference/experiment/condition.json` & `esse-2023.6.20.post0/schema/core/reference/experiment/condition.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/core/reference/experiment.json` & `esse-2023.6.20.post0/schema/core/reference/experiment.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/core/reference/literature.json` & `esse-2023.6.20.post0/schema/core/reference/literature.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/core/reference/modeling/exabyte.json` & `esse-2023.6.20.post0/schema/core/reference/modeling/exabyte.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/core/reusable/band_gap.json` & `esse-2023.6.20.post0/schema/core/reusable/band_gap.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/core/reusable/energy.json` & `esse-2023.6.20.post0/schema/core/reusable/energy.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/core/reusable/file_metadata.json` & `esse-2023.6.20.post0/schema/core/reusable/file_metadata.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/core/reusable/object_storage_container_data.json` & `esse-2023.6.20.post0/schema/core/reusable/object_storage_container_data.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/definitions/units.json` & `esse-2023.6.20.post0/schema/definitions/units.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/element.json` & `esse-2023.6.20.post0/schema/element.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/in_memory_entity/base.json` & `esse-2023.6.20.post0/schema/in_memory_entity/base.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/job/compute.json` & `esse-2023.6.20.post0/schema/job/compute.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/job.json` & `esse-2023.6.20.post0/schema/job.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/material.json` & `esse-2023.6.20.post0/schema/material.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/method.json` & `esse-2023.6.20.post0/schema/method.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/methods_directory/local-orbital.json` & `esse-2023.6.20.post0/schema/methods_directory/local-orbital.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/methods_directory/local_orbital/definitions/basis_sets.json` & `esse-2023.6.20.post0/schema/methods_directory/local_orbital/definitions/basis_sets.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/methods_directory/pseudopotential/dataset.json` & `esse-2023.6.20.post0/schema/methods_directory/pseudopotential/dataset.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/methods_directory/pseudopotential/file/energy_cutoff.json` & `esse-2023.6.20.post0/schema/methods_directory/pseudopotential/file/energy_cutoff.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/methods_directory/pseudopotential/file/radii.json` & `esse-2023.6.20.post0/schema/methods_directory/pseudopotential/file/radii.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/methods_directory/pseudopotential/file.json` & `esse-2023.6.20.post0/schema/methods_directory/pseudopotential/file.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/methods_directory/pseudopotential/precision.json` & `esse-2023.6.20.post0/schema/methods_directory/pseudopotential/precision.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/methods_directory/pseudopotential.json` & `esse-2023.6.20.post0/schema/methods_directory/pseudopotential.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/methods_directory/regression/dataset.json` & `esse-2023.6.20.post0/schema/methods_directory/regression/dataset.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/methods_directory/regression/kernel_ridge/data_per_property.json` & `esse-2023.6.20.post0/schema/methods_directory/regression/kernel_ridge/data_per_property.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/methods_directory/regression/linear/data_per_property.json` & `esse-2023.6.20.post0/schema/methods_directory/regression/linear/data_per_property.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/methods_directory/regression/precision_per_property.json` & `esse-2023.6.20.post0/schema/methods_directory/regression/precision_per_property.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/methods_directory/regression.json` & `esse-2023.6.20.post0/schema/methods_directory/regression.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/model.json` & `esse-2023.6.20.post0/schema/model.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/abin/configuration_interaction/modifiers.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/abin/configuration_interaction/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/abin/configuration_interaction/tags.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/abin/configuration_interaction/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/abin/configuration_interaction.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/abin/configuration_interaction.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/definitions.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/definitions.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dft_unit_functionals.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dft_unit_functionals.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dft_unit_functionals_proto.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dft_unit_functionals_proto.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dispersion_model.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dispersion_model.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/dft_d.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/dft_d.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/exchange_dipole.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/exchange_dipole.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_abin.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_abin.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_empirical.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_empirical.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_abin.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_abin.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_empirical.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_empirical.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/many_body_dispersion.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/many_body_dispersion.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/non_local_correlation.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/non_local_correlation.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/tkatchenko_scheffler.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/dispersion_models_directory/tkatchenko_scheffler.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/functional/component.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/functional/component.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/functional/components_directory/exact_exchange.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/functional/components_directory/exact_exchange.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/functional/components_directory/mp2_correlation.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/functional/components_directory/mp2_correlation.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/functional/components_directory/range_separated_exchange.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/functional/components_directory/range_separated_exchange.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/functional/definitions.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/functional/definitions.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/modifiers.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/tags.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/double_hybrid.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/gga/modifiers.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/gga/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/gga/tags.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/gga/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/gga.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/gga.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/functional.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/functional.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/modifiers.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/tags.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/hybrid.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/lda/modifiers.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/lda/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/lda/tags.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/lda/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/lda.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/lda.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/modifiers.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/tags.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/mgga/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/mgga.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/mgga.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/modifiers.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft/tags.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft/ksdft.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft/ksdft.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/dft.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/dft.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/pb/qm/semp.json` & `esse-2023.6.20.post0/schema/models_directory/pb/qm/semp.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/st/det/ml.json` & `esse-2023.6.20.post0/schema/models_directory/st/det/ml.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/models_directory/unknown.json` & `esse-2023.6.20.post0/schema/models_directory/unknown.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/new_model.json` & `esse-2023.6.20.post0/schema/new_model.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/project.json` & `esse-2023.6.20.post0/schema/project.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/derived_properties.json` & `esse-2023.6.20.post0/schema/properties_directory/derived_properties.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/elemental/ionization_potential.json` & `esse-2023.6.20.post0/schema/properties_directory/elemental/ionization_potential.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/non-scalar/average_potential_profile.json` & `esse-2023.6.20.post0/schema/properties_directory/non-scalar/average_potential_profile.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/non-scalar/band_gaps.json` & `esse-2023.6.20.post0/schema/properties_directory/non-scalar/band_gaps.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/non-scalar/band_structure.json` & `esse-2023.6.20.post0/schema/properties_directory/non-scalar/band_structure.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/non-scalar/charge_density_profile.json` & `esse-2023.6.20.post0/schema/properties_directory/non-scalar/charge_density_profile.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/non-scalar/density_of_states.json` & `esse-2023.6.20.post0/schema/properties_directory/non-scalar/density_of_states.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/non-scalar/file_content.json` & `esse-2023.6.20.post0/schema/properties_directory/non-scalar/file_content.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/non-scalar/phonon_dispersions.json` & `esse-2023.6.20.post0/schema/properties_directory/non-scalar/phonon_dispersions.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/non-scalar/phonon_dos.json` & `esse-2023.6.20.post0/schema/properties_directory/non-scalar/phonon_dos.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/non-scalar/potential_profile.json` & `esse-2023.6.20.post0/schema/properties_directory/non-scalar/potential_profile.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/non-scalar/reaction_energy_profile.json` & `esse-2023.6.20.post0/schema/properties_directory/non-scalar/reaction_energy_profile.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/non-scalar/total_energy_contributions.json` & `esse-2023.6.20.post0/schema/properties_directory/non-scalar/total_energy_contributions.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/non-scalar/vibrational_spectrum.json` & `esse-2023.6.20.post0/schema/properties_directory/non-scalar/vibrational_spectrum.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/structural/atomic_forces.json` & `esse-2023.6.20.post0/schema/properties_directory/structural/atomic_forces.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/structural/basis/atomic_coordinates.json` & `esse-2023.6.20.post0/schema/properties_directory/structural/basis/atomic_coordinates.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/structural/basis/atomic_element.json` & `esse-2023.6.20.post0/schema/properties_directory/structural/basis/atomic_element.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/structural/basis/bonds.json` & `esse-2023.6.20.post0/schema/properties_directory/structural/basis/bonds.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/structural/basis.json` & `esse-2023.6.20.post0/schema/properties_directory/structural/basis.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/structural/elemental_ratio.json` & `esse-2023.6.20.post0/schema/properties_directory/structural/elemental_ratio.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/structural/lattice/lattice_bravais.json` & `esse-2023.6.20.post0/schema/properties_directory/structural/lattice/lattice_bravais.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/structural/lattice/lattice_vectors.json` & `esse-2023.6.20.post0/schema/properties_directory/structural/lattice/lattice_vectors.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/structural/lattice.json` & `esse-2023.6.20.post0/schema/properties_directory/structural/lattice.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/structural/magnetic_moments.json` & `esse-2023.6.20.post0/schema/properties_directory/structural/magnetic_moments.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/structural/p-norm.json` & `esse-2023.6.20.post0/schema/properties_directory/structural/p-norm.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/structural/patterns/functional_group.json` & `esse-2023.6.20.post0/schema/properties_directory/structural/patterns/functional_group.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/structural/patterns/ring.json` & `esse-2023.6.20.post0/schema/properties_directory/structural/patterns/ring.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/structural/patterns/special_bond.json` & `esse-2023.6.20.post0/schema/properties_directory/structural/patterns/special_bond.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/structural/symmetry.json` & `esse-2023.6.20.post0/schema/properties_directory/structural/symmetry.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/workflow/convergence/electronic.json` & `esse-2023.6.20.post0/schema/properties_directory/workflow/convergence/electronic.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/workflow/convergence/ionic.json` & `esse-2023.6.20.post0/schema/properties_directory/workflow/convergence/ionic.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/properties_directory/workflow/convergence/kpoint.json` & `esse-2023.6.20.post0/schema/properties_directory/workflow/convergence/kpoint.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/property/raw.json` & `esse-2023.6.20.post0/schema/property/raw.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/property/refined.json` & `esse-2023.6.20.post0/schema/property/refined.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/property/source.json` & `esse-2023.6.20.post0/schema/property/source.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/software/application.json` & `esse-2023.6.20.post0/schema/software/application.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/software/executable.json` & `esse-2023.6.20.post0/schema/software/executable.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/software/flavor.json` & `esse-2023.6.20.post0/schema/software/flavor.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/software/template.json` & `esse-2023.6.20.post0/schema/software/template.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/software_directory/ml/exabyteml.json` & `esse-2023.6.20.post0/schema/software_directory/ml/exabyteml.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/software_directory/ml/unit/execution/evaluate/cross-validate.json` & `esse-2023.6.20.post0/schema/software_directory/ml/unit/execution/evaluate/cross-validate.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/software_directory/ml/unit/execution/initialize.json` & `esse-2023.6.20.post0/schema/software_directory/ml/unit/execution/initialize.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/software_directory/ml/unit/execution/train.json` & `esse-2023.6.20.post0/schema/software_directory/ml/unit/execution/train.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/software_directory/ml/unit/processing/data_transformation/manipulation.json` & `esse-2023.6.20.post0/schema/software_directory/ml/unit/processing/data_transformation/manipulation.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json` & `esse-2023.6.20.post0/schema/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/software_directory/ml/unit/processing/feature_selection/filter_based.json` & `esse-2023.6.20.post0/schema/software_directory/ml/unit/processing/feature_selection/filter_based.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/software_directory/modeling/espresso/arguments.json` & `esse-2023.6.20.post0/schema/software_directory/modeling/espresso/arguments.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/software_directory/modeling/espresso.json` & `esse-2023.6.20.post0/schema/software_directory/modeling/espresso.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/software_directory/modeling/nwchem.json` & `esse-2023.6.20.post0/schema/software_directory/modeling/nwchem.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/software_directory/modeling/vasp.json` & `esse-2023.6.20.post0/schema/software_directory/modeling/vasp.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/software_directory/scripting/jupyter-lab.json` & `esse-2023.6.20.post0/schema/software_directory/scripting/jupyter-lab.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/software_directory/scripting/python.json` & `esse-2023.6.20.post0/schema/software_directory/scripting/python.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/software_directory/scripting/shell.json` & `esse-2023.6.20.post0/schema/software_directory/scripting/shell.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/system/database_source.json` & `esse-2023.6.20.post0/schema/system/database_source.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/system/file_source.json` & `esse-2023.6.20.post0/schema/system/file_source.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/system/history.json` & `esse-2023.6.20.post0/schema/system/history.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/system/in_set.json` & `esse-2023.6.20.post0/schema/system/in_set.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/system/job_extended.json` & `esse-2023.6.20.post0/schema/system/job_extended.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/system/message.json` & `esse-2023.6.20.post0/schema/system/message.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/system/status.json` & `esse-2023.6.20.post0/schema/system/status.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/system/timestampable.json` & `esse-2023.6.20.post0/schema/system/timestampable.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/workflow/base_flow.json` & `esse-2023.6.20.post0/schema/workflow/base_flow.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/workflow/new_subworkflow.json` & `esse-2023.6.20.post0/schema/workflow/new_subworkflow.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/workflow/subworkflow.json` & `esse-2023.6.20.post0/schema/workflow/subworkflow.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/workflow/unit/assertion.json` & `esse-2023.6.20.post0/schema/workflow/unit/assertion.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/workflow/unit/assignment.json` & `esse-2023.6.20.post0/schema/workflow/unit/assignment.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/workflow/unit/condition.json` & `esse-2023.6.20.post0/schema/workflow/unit/condition.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/workflow/unit/execution.json` & `esse-2023.6.20.post0/schema/workflow/unit/execution.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/workflow/unit/input/_input.json` & `esse-2023.6.20.post0/schema/workflow/unit/input/_input.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/workflow/unit/input/_inputItem.json` & `esse-2023.6.20.post0/schema/workflow/unit/input/_inputItem.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/workflow/unit/input/_inputItemId.json` & `esse-2023.6.20.post0/schema/workflow/unit/input/_inputItemId.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/workflow/unit/input/_inputItemScope.json` & `esse-2023.6.20.post0/schema/workflow/unit/input/_inputItemScope.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/workflow/unit/io/api.json` & `esse-2023.6.20.post0/schema/workflow/unit/io/api.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/workflow/unit/io/db.json` & `esse-2023.6.20.post0/schema/workflow/unit/io/db.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/workflow/unit/io/object_storage.json` & `esse-2023.6.20.post0/schema/workflow/unit/io/object_storage.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/workflow/unit/io.json` & `esse-2023.6.20.post0/schema/workflow/unit/io.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/workflow/unit/map.json` & `esse-2023.6.20.post0/schema/workflow/unit/map.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/workflow/unit/processing.json` & `esse-2023.6.20.post0/schema/workflow/unit/processing.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/workflow/unit/reduce.json` & `esse-2023.6.20.post0/schema/workflow/unit/reduce.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/workflow/unit/runtime/runtime_items.json` & `esse-2023.6.20.post0/schema/workflow/unit/runtime/runtime_items.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/workflow/unit.json` & `esse-2023.6.20.post0/schema/workflow/unit.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/schema/workflow.json` & `esse-2023.6.20.post0/schema/workflow.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/setup.py` & `esse-2023.6.20.post0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,55 +6,53 @@
     files = []
     for root, dirs_, files_ in os.walk(path, followlinks=True):
         for file_ in files_:
             files.append(os.path.join(root, file_))
     return files
 
 
-with open('./README.md', 'r') as f:
+with open("./README.md", "r") as f:
     long_description = f.read()
 
 DIR = os.path.abspath(os.path.dirname(__file__))
 EXTRA_FILES = get_files_by_path(os.path.join(DIR, "example"))
 EXTRA_FILES.extend(get_files_by_path(os.path.join(DIR, "schema")))
 EXTRA_FILES.extend(get_files_by_path(os.path.join(DIR, "manifest")))
 
 setup(
-    name='esse',
-    setup_requires=['setuptools_scm'],
+    name="esse",
+    setup_requires=["setuptools_scm"],
     use_scm_version={
-        'version_scheme': 'post-release',
+        "version_scheme": "post-release",
     },
-    description='Exabyte Source of Schemas and Examples',
+    description="Exabyte Source of Schemas and Examples",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/Exabyte-io/exabyte-esse',
-    author='Exabyte Inc.',
-    author_email='info@exabyte.io',
-    packages=find_packages(where='src/py', exclude=['src/py/tests*']),
-    package_dir={'': 'src/py'},
-    package_data={'esse': [f.replace(DIR, "data") for f in EXTRA_FILES]},
+    long_description_content_type="text/markdown",
+    url="https://github.com/Exabyte-io/exabyte-esse",
+    author="Exabyte Inc.",
+    author_email="info@exabyte.io",
+    packages=find_packages(where="src/py", exclude=["src/py/tests*"]),
+    package_dir={"": "src/py"},
+    package_data={"esse": [f.replace(DIR, "data") for f in EXTRA_FILES]},
     install_requires=[
         "pyyaml>=4.2b1,<6",
         "jsonschema==2.6.0",
         "python-slugify==2.0.1",
-        "exabyte_json_include>=2020.10.19"
+        "exabyte_json_include>=2020.10.19",
     ],
     extras_require={
         "test": [
             "coverage[toml]>=5.3",
         ]
     },
     entry_points={
-        'console_scripts': [
-            'generate_dft_unit_functionals=esse.functionals:generate_dft_unit_functionals'
-        ],
+        "console_scripts": ["generate_dft_unit_functionals=esse.functionals:generate_dft_unit_functionals"],
     },
     python_requires=">=3.6",
     classifiers=[
-        'Programming Language :: Python',
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'Topic :: Software Development',
-        'License :: OSI Approved :: Apache Software License'
-    ]
+        "Programming Language :: Python",
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development",
+        "License :: OSI Approved :: Apache Software License",
+    ],
 )
```

### Comparing `esse-2023.6.16.post0/src/js/esse/index.js` & `esse-2023.6.20.post0/src/js/esse/index.js`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/js/esse/tests/validate.js` & `esse-2023.6.20.post0/src/js/esse/tests/validate.js`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/js/esse/utils.js` & `esse-2023.6.20.post0/src/js/esse/utils.js`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/js/json_include/index.js` & `esse-2023.6.20.post0/src/js/json_include/index.js`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/js/scripts/setSchemaIds.mjs` & `esse-2023.6.20.post0/src/js/scripts/setSchemaIds.mjs`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/__init__.py` & `esse-2023.6.20.post0/src/py/esse/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import jsonschema
 
 from esse.utils import parseIncludeReferenceStatementsByDir
 from esse.settings import SCHEMAS_DIR, EXAMPLES_DIR, PROPERTIES_MANIFEST
+
 # from esse.functionals import generate_dft_unit_functionals
 
 ## Note: We're disabling this for now to avoid a bug discovered in deployment - files are not necessarily writeable
 ## in the installed context, if the calling code is executed with a different user than the one that owns the install
 ## directory.  The function can be run manually with the `generate_dft_unit_functionals` command line script generated
 ## in setup.py when esse is installed.
 # generate_dft_unit_functionals()
```

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/job/compute.json` & `esse-2023.6.20.post0/src/py/esse/data/example/job/compute.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/job.json` & `esse-2023.6.20.post0/src/py/esse/data/example/job.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/material.json` & `esse-2023.6.20.post0/src/py/esse/data/example/material.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/methods_directory/pseudopotential/file.json` & `esse-2023.6.20.post0/src/py/esse/data/example/methods_directory/pseudopotential/file.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/methods_directory/regression.json` & `esse-2023.6.20.post0/src/py/esse/data/example/methods_directory/regression.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/abin/configuration_interaction.json` & `esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/abin/configuration_interaction.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json` & `esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json` & `esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/hybrid/functional.json` & `esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/hybrid/functional.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json` & `esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/lda.json` & `esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft/lda.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft.json` & `esse-2023.6.20.post0/src/py/esse/data/example/models_directory/pb/qm/dft/ksdft.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/non-scalar/band_structure.json` & `esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/non-scalar/band_structure.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/non-scalar/density_of_states.json` & `esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/non-scalar/density_of_states.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/non-scalar/phonon_dispersions.json` & `esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/non-scalar/phonon_dispersions.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/non-scalar/phonon_dos.json` & `esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/non-scalar/phonon_dos.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/non-scalar/potential_profile.json` & `esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/non-scalar/potential_profile.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/non-scalar/reaction_energy_profile.json` & `esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/non-scalar/reaction_energy_profile.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/non-scalar/total_energy_contributions.json` & `esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/non-scalar/total_energy_contributions.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/properties_directory/structural/molecular_pattern.json` & `esse-2023.6.20.post0/src/py/esse/data/example/properties_directory/structural/molecular_pattern.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/software_directory/ml/unit/execution/train.json` & `esse-2023.6.20.post0/src/py/esse/data/example/software_directory/ml/unit/execution/train.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json` & `esse-2023.6.20.post0/src/py/esse/data/example/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/system/file_source.json` & `esse-2023.6.20.post0/src/py/esse/data/example/system/file_source.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/workflow/unit/execution.json` & `esse-2023.6.20.post0/src/py/esse/data/example/workflow/unit/execution.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/workflow/unit/io/api.json` & `esse-2023.6.20.post0/src/py/esse/data/example/workflow/unit/io/api.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/workflow/unit/io.json` & `esse-2023.6.20.post0/src/py/esse/data/example/workflow/unit/io.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/example/workflow.json` & `esse-2023.6.20.post0/src/py/esse/data/example/workflow.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/manifest/dft_unit_functionals.yaml` & `esse-2023.6.20.post0/src/py/esse/data/manifest/dft_unit_functionals.yaml`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/manifest/functional_lookup_table.yaml` & `esse-2023.6.20.post0/src/py/esse/data/manifest/functional_lookup_table.yaml`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/manifest/models.yaml` & `esse-2023.6.20.post0/src/py/esse/data/manifest/models.yaml`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/manifest/properties.yaml` & `esse-2023.6.20.post0/src/py/esse/data/manifest/properties.yaml`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/core/abstract/2d_plot.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/core/abstract/2d_plot.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/core/abstract/3d_vector_basis.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/core/abstract/3d_vector_basis.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/core/primitive/3d_lattice.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/core/primitive/3d_lattice.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/core/primitive/slugified_entry.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/core/primitive/slugified_entry.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/core/reference/exabyte.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/core/reference/exabyte.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/core/reference/experiment/condition.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/core/reference/experiment/condition.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/core/reference/experiment.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/core/reference/experiment.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/core/reference/literature.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/core/reference/literature.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/core/reference/modeling/exabyte.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/core/reference/modeling/exabyte.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/core/reusable/band_gap.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/core/reusable/band_gap.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/core/reusable/energy.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/core/reusable/energy.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/core/reusable/file_metadata.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/core/reusable/file_metadata.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/core/reusable/object_storage_container_data.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/core/reusable/object_storage_container_data.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/definitions/units.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/definitions/units.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/element.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/element.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/in_memory_entity/base.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/in_memory_entity/base.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/job/compute.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/job/compute.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/job.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/job.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/material.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/material.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/method.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/method.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/local-orbital.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/local-orbital.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/local_orbital/definitions/basis_sets.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/local_orbital/definitions/basis_sets.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/pseudopotential/dataset.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/pseudopotential/dataset.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file/energy_cutoff.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file/energy_cutoff.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file/radii.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file/radii.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/pseudopotential/file.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/pseudopotential/precision.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/pseudopotential/precision.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/pseudopotential.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/pseudopotential.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/regression/dataset.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/regression/dataset.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/regression/kernel_ridge/data_per_property.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/regression/kernel_ridge/data_per_property.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/regression/linear/data_per_property.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/regression/linear/data_per_property.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/regression/precision_per_property.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/regression/precision_per_property.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/methods_directory/regression.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/methods_directory/regression.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/model.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/model.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/modifiers.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/tags.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/abin/configuration_interaction.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/definitions.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/definitions.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dft_unit_functionals.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dft_unit_functionals.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dft_unit_functionals_proto.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dft_unit_functionals_proto.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_model.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_model.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/dft_d.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/dft_d.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/exchange_dipole.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/exchange_dipole.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_abin.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_abin.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_empirical.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/intra_empirical.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_abin.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_abin.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_empirical.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/generalized/post_empirical.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/many_body_dispersion.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/many_body_dispersion.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/non_local_correlation.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/non_local_correlation.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/tkatchenko_scheffler.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/dispersion_models_directory/tkatchenko_scheffler.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/component.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/component.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/exact_exchange.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/exact_exchange.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/mp2_correlation.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/mp2_correlation.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/range_separated_exchange.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/components_directory/range_separated_exchange.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/definitions.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/functional/definitions.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/functional.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/modifiers.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/range_separated_functional.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/tags.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/double_hybrid.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/modifiers.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/tags.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/gga.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/functional.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/functional.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/modifiers.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/range_separated_functional.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/tags.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/hybrid.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/modifiers.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/tags.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/lda.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/modifiers.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/tags.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/mgga.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/modifiers.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/modifiers.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/tags.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft/tags.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft/ksdft.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/dft.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/dft.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/pb/qm/semp.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/pb/qm/semp.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/st/det/ml.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/st/det/ml.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/models_directory/unknown.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/models_directory/unknown.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/new_model.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/new_model.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/project.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/project.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/derived_properties.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/derived_properties.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/elemental/ionization_potential.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/elemental/ionization_potential.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/average_potential_profile.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/average_potential_profile.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/band_gaps.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/band_gaps.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/band_structure.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/band_structure.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/charge_density_profile.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/charge_density_profile.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/density_of_states.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/density_of_states.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/file_content.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/file_content.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/phonon_dispersions.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/phonon_dispersions.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/phonon_dos.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/phonon_dos.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/potential_profile.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/potential_profile.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/reaction_energy_profile.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/reaction_energy_profile.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/total_energy_contributions.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/total_energy_contributions.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/non-scalar/vibrational_spectrum.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/non-scalar/vibrational_spectrum.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/atomic_forces.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/atomic_forces.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/basis/atomic_coordinates.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/basis/atomic_coordinates.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/basis/atomic_element.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/basis/atomic_element.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/basis/bonds.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/basis/bonds.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/basis.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/basis.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/elemental_ratio.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/elemental_ratio.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/lattice/lattice_bravais.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/lattice/lattice_bravais.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/lattice/lattice_vectors.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/lattice/lattice_vectors.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/lattice.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/lattice.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/magnetic_moments.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/magnetic_moments.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/p-norm.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/p-norm.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/patterns/functional_group.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/patterns/functional_group.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/patterns/ring.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/patterns/ring.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/patterns/special_bond.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/patterns/special_bond.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/structural/symmetry.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/structural/symmetry.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/electronic.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/electronic.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/ionic.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/ionic.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/kpoint.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/properties_directory/workflow/convergence/kpoint.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/property/raw.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/property/raw.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/property/refined.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/property/refined.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/property/source.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/property/source.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/software/application.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/software/application.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/software/executable.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/software/executable.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/software/flavor.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/software/flavor.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/software/template.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/software/template.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/exabyteml.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/exabyteml.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/evaluate/cross-validate.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/evaluate/cross-validate.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/initialize.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/initialize.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/train.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/unit/execution/train.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/data_transformation/manipulation.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/data_transformation/manipulation.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/data_transformation/scale_and_reduce.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/feature_selection/filter_based.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/ml/unit/processing/feature_selection/filter_based.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/modeling/espresso/arguments.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/modeling/espresso/arguments.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/modeling/espresso.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/modeling/espresso.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/modeling/nwchem.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/modeling/nwchem.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/modeling/vasp.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/modeling/vasp.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/scripting/jupyter-lab.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/scripting/jupyter-lab.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/scripting/python.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/scripting/python.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/software_directory/scripting/shell.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/software_directory/scripting/shell.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/system/database_source.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/system/database_source.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/system/file_source.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/system/file_source.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/system/history.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/system/history.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/system/in_set.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/system/in_set.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/system/job_extended.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/system/job_extended.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/system/message.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/system/message.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/system/status.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/system/status.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/system/timestampable.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/system/timestampable.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/workflow/base_flow.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/workflow/base_flow.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/workflow/new_subworkflow.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/workflow/new_subworkflow.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/workflow/subworkflow.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/workflow/subworkflow.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/assertion.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/assertion.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/assignment.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/assignment.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/condition.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/condition.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/execution.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/execution.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/input/_input.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/input/_input.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/input/_inputItem.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/input/_inputItem.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/input/_inputItemId.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/input/_inputItemId.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/input/_inputItemScope.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/input/_inputItemScope.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/io/api.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/io/api.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/io/db.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/io/db.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/io/object_storage.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/io/object_storage.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/io.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/io.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/map.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/map.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/processing.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/processing.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/reduce.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/reduce.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit/runtime/runtime_items.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit/runtime/runtime_items.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/workflow/unit.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/workflow/unit.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/data/schema/workflow.json` & `esse-2023.6.20.post0/src/py/esse/data/schema/workflow.json`

 * *Files identical despite different names*

### Comparing `esse-2023.6.16.post0/src/py/esse/functionals.py` & `esse-2023.6.20.post0/src/py/esse/functionals.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from esse.utils import read_json_file, dump_json_file
 
 DIR = os.path.dirname(__file__)
 UNIT_FUNCTIONALS_PATH = os.path.join(DIR, "data/schema/models_directory/pb/qm/dft")
 PROTOTYPE_FILENAME = os.path.join(UNIT_FUNCTIONALS_PATH, "dft_unit_functionals_proto.json")
 UNIT_FILENAME = os.path.join(UNIT_FUNCTIONALS_PATH, "dft_unit_functionals.json")
 
-SCHEMA_WITH_PROPERTIES_TEMPLATE = Template("""{
+SCHEMA_WITH_PROPERTIES_TEMPLATE = Template(
+    """{
 "properties": {
     "name": {
         "enum": [
             "$name"
         ]
     },
     "slug": {
@@ -22,15 +23,17 @@
     },
     "type": {
         "enum": [
             "$type"
         ]
     }
 }
-}""")
+}"""
+)
+
 
 def generate_dft_unit_functionals():
     """
     Generate list of functionals suitable for validation by 'oneOf'.
 
     The targeted JSON file has a convoluted form which makes it inconvenient
     to read and prone to errors. Thus, it is generated automatically from
```

### Comparing `esse-2023.6.16.post0/src/py/esse/tests/validate.py` & `esse-2023.6.20.post0/src/py/esse/tests/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from esse.settings import SCHEMAS_DIR, EXAMPLES_DIR
 from esse.utils import parseIncludeReferenceStatements
 
 esse = ESSE()
 
 
 class TestCase(unittest.TestCase):
-
     def __init__(self, example_path):
         super(TestCase, self).__init__(methodName="runTest")
         self.example_path = example_path
         self.schema_path = self.example_path.replace(EXAMPLES_DIR, SCHEMAS_DIR)
 
     def runTest(self):
         schema = parseIncludeReferenceStatements(self.schema_path)
```

### Comparing `esse-2023.6.16.post0/src/py/esse/utils.py` & `esse-2023.6.20.post0/src/py/esse/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     Args:
         path_ (str): path to JSON file.
         content (dict): JSON file content.
         sort_keys (bool): whether to sort keys. Defaults to True.
     """
     with open(path_, "w+") as f:
-        f.write("".join((json.dumps(content, separators=(',', ': '), indent=4, sort_keys=sort_keys), "\n")))
+        f.write("".join((json.dumps(content, separators=(",", ": "), indent=4, sort_keys=sort_keys), "\n")))
 
 
 def refactor_examples():
     """
     Refactors examples:
         - fix space and indentation
         - sort keys
@@ -96,12 +96,14 @@
     """
     Slugifies the schema path and uses it as schema ID.
 
     Args:
         path_ (str): path to JSON file.
     """
     content = read_json_file(path_)
-    if not content.get("$schema"): return  # do not add ID to non-schema files
-    if content.get("schemaId"): del content["schemaId"]
-    schema_id = slugify(path_.replace("{}/".format(SCHEMAS_DIR), '').replace(".json", ""))
+    if not content.get("$schema"):
+        return  # do not add ID to non-schema files
+    if content.get("schemaId"):
+        del content["schemaId"]
+    schema_id = slugify(path_.replace("{}/".format(SCHEMAS_DIR), "").replace(".json", ""))
     content = OrderedDict(list(OrderedDict({"schemaId": schema_id}).items()) + list(content.items()))
     dump_json_file(path_, content, False)
```

### Comparing `esse-2023.6.16.post0/src/py/esse.egg-info/PKG-INFO` & `esse-2023.6.20.post0/src/py/esse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esse
-Version: 2023.6.16.post0
+Version: 2023.6.20.post0
 Summary: Exabyte Source of Schemas and Examples
 Home-page: https://github.com/Exabyte-io/exabyte-esse
 Author: Exabyte Inc.
 Author-email: info@exabyte.io
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `esse-2023.6.16.post0/src/py/esse.egg-info/SOURCES.txt` & `esse-2023.6.20.post0/src/py/esse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

