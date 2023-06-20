# Comparing `tmp/windkit-0.6.1.tar.gz` & `tmp/windkit-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windkit-0.6.1.tar", last modified: Thu Mar 16 11:56:45 2023, max compression
+gzip compressed data, was "windkit-0.6.2.tar", last modified: Tue Jun 20 10:08:22 2023, max compression
```

## Comparing `windkit-0.6.1.tar` & `windkit-0.6.2.tar`

### file list

```diff
@@ -1,149 +1,150 @@
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-03-16 11:56:45.611014 windkit-0.6.1/
--rw-rw-r--   0 neil      (1000) neil      (1000)      461 2023-01-31 04:56:55.000000 windkit-0.6.1/.gitignore
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-03-16 11:56:45.555014 windkit-0.6.1/.gitlab/
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-03-16 11:56:45.559014 windkit-0.6.1/.gitlab/merge_request_templates/
--rw-rw-r--   0 neil      (1000) neil      (1000)      491 2023-01-31 04:56:55.000000 windkit-0.6.1/.gitlab/merge_request_templates/default.md
--rw-rw-r--   0 neil      (1000) neil      (1000)    12309 2023-03-14 11:45:01.000000 windkit-0.6.1/.gitlab-ci.yml
--rw-rw-r--   0 neil      (1000) neil      (1000)     1058 2023-03-14 11:45:01.000000 windkit-0.6.1/.pre-commit-config.yaml
--rw-rw-r--   0 neil      (1000) neil      (1000)     1261 2023-01-31 04:56:55.000000 windkit-0.6.1/.pylintrc
--rw-rw-r--   0 neil      (1000) neil      (1000)    12296 2023-03-16 11:51:20.000000 windkit-0.6.1/CHANGELOG.md
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-03-16 11:56:45.559014 windkit-0.6.1/CI_helper_scripts/
--rwxrwxr-x   0 neil      (1000) neil      (1000)      624 2023-01-31 04:56:55.000000 windkit-0.6.1/CI_helper_scripts/post_build_test_nix.sh
--rwxrwxr-x   0 neil      (1000) neil      (1000)      680 2023-01-31 04:56:55.000000 windkit-0.6.1/CI_helper_scripts/post_build_test_win.sh
--rw-rw-r--   0 neil      (1000) neil      (1000)     1523 2023-01-31 04:56:55.000000 windkit-0.6.1/LICENSE
--rw-rw-r--   0 neil      (1000) neil      (1000)      149 2023-02-14 09:38:21.000000 windkit-0.6.1/MANIFEST.in
--rw-rw-r--   0 neil      (1000) neil      (1000)     4045 2023-03-16 11:56:45.611014 windkit-0.6.1/PKG-INFO
--rw-rw-r--   0 neil      (1000) neil      (1000)     3428 2023-03-16 11:55:52.000000 windkit-0.6.1/README-Internal.md
--rw-rw-r--   0 neil      (1000) neil      (1000)     3537 2023-01-31 04:56:55.000000 windkit-0.6.1/README.md
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-03-16 11:56:45.567014 windkit-0.6.1/docs/
--rw-rw-r--   0 neil      (1000) neil      (1000)       82 2023-01-31 04:56:55.000000 windkit-0.6.1/docs/.dockerignore
--rw-rw-r--   0 neil      (1000) neil      (1000)       11 2023-01-31 04:56:55.000000 windkit-0.6.1/docs/.gitignore
--rw-rw-r--   0 neil      (1000) neil      (1000)      108 2023-01-31 04:56:55.000000 windkit-0.6.1/docs/Dockerfile
--rw-rw-r--   0 neil      (1000) neil      (1000)     7042 2023-01-31 04:56:55.000000 windkit-0.6.1/docs/Makefile
--rw-rw-r--   0 neil      (1000) neil      (1000)      559 2023-01-31 04:56:55.000000 windkit-0.6.1/docs/docker-compose.yml
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-03-16 11:56:45.555014 windkit-0.6.1/docs/legacy/
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-03-16 11:56:45.567014 windkit-0.6.1/docs/legacy/dev/
--rw-rw-r--   0 neil      (1000) neil      (1000)     2228 2023-01-31 04:56:55.000000 windkit-0.6.1/docs/legacy/dev/dev-git.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)     1759 2023-01-31 04:56:55.000000 windkit-0.6.1/docs/legacy/dev/dev-intro.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)     2208 2023-01-31 04:56:55.000000 windkit-0.6.1/docs/legacy/dev/dev-pytest.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)     1418 2023-01-31 04:56:55.000000 windkit-0.6.1/docs/legacy/dev/dev-sphinx.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)      239 2023-01-31 04:56:55.000000 windkit-0.6.1/docs/nginx.conf
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-03-16 11:56:45.575014 windkit-0.6.1/docs/source/
--rw-rw-r--   0 neil      (1000) neil      (1000)     9713 2023-01-31 04:56:55.000000 windkit-0.6.1/docs/source/WAsP.bib
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-03-16 11:56:45.555014 windkit-0.6.1/docs/source/_templates/
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-03-16 11:56:45.579014 windkit-0.6.1/docs/source/_templates/autosummary/
--rw-rw-r--   0 neil      (1000) neil      (1000)      585 2023-01-31 04:56:55.000000 windkit-0.6.1/docs/source/_templates/autosummary/class.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)      693 2023-01-31 04:56:55.000000 windkit-0.6.1/docs/source/_templates/autosummary/module.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)     9885 2023-03-14 11:45:01.000000 windkit-0.6.1/docs/source/conf.py
--rw-rw-r--   0 neil      (1000) neil      (1000)      125 2023-03-14 11:45:01.000000 windkit-0.6.1/docs/source/development_roadmap.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)     1358 2023-03-14 11:45:01.000000 windkit-0.6.1/docs/source/index.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)     4567 2023-01-31 04:56:55.000000 windkit-0.6.1/docs/source/installation.rst
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-03-16 11:56:45.579014 windkit-0.6.1/docs/source/io/
--rw-rw-r--   0 neil      (1000) neil      (1000)     4014 2023-03-14 11:45:01.000000 windkit-0.6.1/docs/source/io/io.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)      241 2023-01-31 04:56:55.000000 windkit-0.6.1/docs/source/map_conversion.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)       66 2023-01-31 04:56:55.000000 windkit-0.6.1/docs/source/map_conversion_examples_nb.nblink
--rw-rw-r--   0 neil      (1000) neil      (1000)      439 2023-01-31 04:56:55.000000 windkit-0.6.1/docs/source/plotting.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)      301 2023-01-31 04:56:55.000000 windkit-0.6.1/docs/source/plotting_examples.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)       53 2023-01-31 04:56:55.000000 windkit-0.6.1/docs/source/plotting_examples_nb.nblink
--rw-rw-r--   0 neil      (1000) neil      (1000)    10214 2023-01-31 04:56:55.000000 windkit-0.6.1/docs/source/plotting_user_guide.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)      127 2023-03-14 11:45:01.000000 windkit-0.6.1/docs/source/release_notes.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)     4794 2023-01-31 04:56:55.000000 windkit-0.6.1/docs/source/topographic_data.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)     3232 2023-01-31 04:56:55.000000 windkit-0.6.1/docs/source/wind_climate_objects.rst
--rw-rw-r--   0 neil      (1000) neil      (1000)     5859 2023-01-31 04:56:55.000000 windkit-0.6.1/docs/source/windkit.rst
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-03-16 11:56:45.583014 windkit-0.6.1/env/
--rw-rw-r--   0 neil      (1000) neil      (1000)      498 2023-01-31 04:56:55.000000 windkit-0.6.1/env/Dockerfile.api
--rw-rw-r--   0 neil      (1000) neil      (1000)     1209 2023-03-14 11:45:01.000000 windkit-0.6.1/env/Dockerfile.ci
--rw-rw-r--   0 neil      (1000) neil      (1000)      421 2023-01-31 04:56:55.000000 windkit-0.6.1/env/Dockerfile.miniconda
--rw-rw-r--   0 neil      (1000) neil      (1000)      187 2023-03-14 11:45:01.000000 windkit-0.6.1/env/Makefile
--rw-rw-r--   0 neil      (1000) neil      (1000)      891 2023-03-14 11:45:01.000000 windkit-0.6.1/env/conda-linux-64.lock
--rw-rw-r--   0 neil      (1000) neil      (1000)    35182 2023-01-31 04:56:55.000000 windkit-0.6.1/env/conda-osx-64.lock
--rw-rw-r--   0 neil      (1000) neil      (1000)    42058 2023-02-14 09:38:21.000000 windkit-0.6.1/env/conda-win-64.lock
--rw-rw-r--   0 neil      (1000) neil      (1000)     1692 2023-02-14 09:38:21.000000 windkit-0.6.1/env/create_locks.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     1066 2023-03-14 11:45:01.000000 windkit-0.6.1/env/dev_env.yaml
--rw-rw-r--   0 neil      (1000) neil      (1000)      186 2023-02-14 09:38:21.000000 windkit-0.6.1/env/pywasp.cfg
--rw-rw-r--   0 neil      (1000) neil      (1000)      653 2023-02-14 09:38:21.000000 windkit-0.6.1/env/pywasp_env.yml
--rw-rw-r--   0 neil      (1000) neil      (1000)      470 2023-02-14 09:38:21.000000 windkit-0.6.1/env/pywaspio_env.yml
--rw-rw-r--   0 neil      (1000) neil      (1000)       78 2023-02-14 09:38:21.000000 windkit-0.6.1/env/windkit.ini
--rw-rw-r--   0 neil      (1000) neil      (1000)      441 2023-02-07 11:47:48.000000 windkit-0.6.1/pyproject.toml
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-03-16 11:56:45.583014 windkit-0.6.1/recipe/
--rw-rw-r--   0 neil      (1000) neil      (1000)      667 2023-03-14 11:45:01.000000 windkit-0.6.1/recipe/meta.yaml
--rw-rw-r--   0 neil      (1000) neil      (1000)      962 2023-03-16 11:56:45.611014 windkit-0.6.1/setup.cfg
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-03-16 11:56:45.599014 windkit-0.6.1/windkit/
--rw-rw-r--   0 neil      (1000) neil      (1000)     1020 2023-03-14 11:45:01.000000 windkit-0.6.1/windkit/__init__.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     1726 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/_errors.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     8505 2023-03-14 11:45:01.000000 windkit-0.6.1/windkit/_rvea_xml.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     2179 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/_validate.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    11639 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/_vectormap_gml.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     5008 2023-03-14 11:45:01.000000 windkit-0.6.1/windkit/_vectormap_helpers.py
--rw-rw-r--   0 neil      (1000) neil      (1000)      160 2023-03-16 11:56:45.000000 windkit-0.6.1/windkit/_version.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    37804 2023-02-14 09:38:21.000000 windkit-0.6.1/windkit/all_vars.json
--rw-rw-r--   0 neil      (1000) neil      (1000)    32058 2023-02-14 09:38:21.000000 windkit-0.6.1/windkit/binned_wind_climate.py
--rw-rw-r--   0 neil      (1000) neil      (1000)      155 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/config.py
--rw-rw-r--   0 neil      (1000) neil      (1000)      981 2023-02-14 09:38:21.000000 windkit-0.6.1/windkit/data_structures.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     1110 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/elevation_map.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    17220 2023-03-14 11:45:01.000000 windkit-0.6.1/windkit/empty.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    21529 2023-03-14 11:45:01.000000 windkit-0.6.1/windkit/generalized_wind_climate.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     1131 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/geospatial_imports.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     9775 2023-02-14 09:38:21.000000 windkit-0.6.1/windkit/get_map.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     8201 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/landcover.py
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-03-16 11:56:45.603014 windkit-0.6.1/windkit/landcovertables/
--rw-rw-r--   0 neil      (1000) neil      (1000)     1943 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/landcovertables/CGLS-LC100.json
--rw-rw-r--   0 neil      (1000) neil      (1000)     5736 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/landcovertables/CORINE.json
--rw-rw-r--   0 neil      (1000) neil      (1000)     2643 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/landcovertables/Globcover.json
--rw-rw-r--   0 neil      (1000) neil      (1000)     1315 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/landcovertables/MODIS.json
--rw-rw-r--   0 neil      (1000) neil      (1000)      883 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/landcovertables/WorldCover.json
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-03-16 11:56:45.603014 windkit-0.6.1/windkit/map_conversion/
--rw-rw-r--   0 neil      (1000) neil      (1000)        0 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/map_conversion/__init__.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     1757 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/map_conversion/helper_functions.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    24213 2023-03-14 11:45:01.000000 windkit-0.6.1/windkit/map_conversion/lines2poly.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    21612 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/map_conversion/poly2lines.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    12972 2023-03-14 11:45:01.000000 windkit-0.6.1/windkit/map_file_header_to_epsg.json
--rw-rw-r--   0 neil      (1000) neil      (1000)    15852 2023-02-14 09:38:21.000000 windkit-0.6.1/windkit/metadata.py
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-03-16 11:56:45.603014 windkit-0.6.1/windkit/plot/
--rw-rw-r--   0 neil      (1000) neil      (1000)      889 2023-02-14 09:38:21.000000 windkit-0.6.1/windkit/plot/__init__.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     1237 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/plot/_colormaps.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     3859 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/plot/_helpers.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     8517 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/plot/color.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    16579 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/plot/histogram.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     2605 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/plot/landcover_map.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    13441 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/plot/operational_curves.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     4040 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/plot/raster_plot.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     5476 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/plot/roughness_rose.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     4306 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/plot/vertical_profile.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     8993 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/plot/wind_rose.py
--rw-rw-r--   0 neil      (1000) neil      (1000)      981 2023-02-14 09:38:21.000000 windkit-0.6.1/windkit/plot/wind_turbine.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    12330 2023-02-14 09:38:21.000000 windkit-0.6.1/windkit/raster_map.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     1096 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/roughness_map.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     4708 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/sector.py
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-03-16 11:56:45.611014 windkit-0.6.1/windkit/spatial/
--rw-rw-r--   0 neil      (1000) neil      (1000)     1684 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/spatial/README.md
--rw-rw-r--   0 neil      (1000) neil      (1000)     1433 2023-03-14 11:45:01.000000 windkit-0.6.1/windkit/spatial/__init__.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     5989 2023-02-14 09:38:21.000000 windkit-0.6.1/windkit/spatial/_bbox.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     4003 2023-03-14 11:45:01.000000 windkit-0.6.1/windkit/spatial/_crs.py
--rw-rw-r--   0 neil      (1000) neil      (1000)      754 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/spatial/_cuboid.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     1432 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/spatial/_dimensions.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     4676 2023-02-14 09:38:21.000000 windkit-0.6.1/windkit/spatial/_interpolation.py
--rw-rw-r--   0 neil      (1000) neil      (1000)      775 2023-02-14 09:38:21.000000 windkit-0.6.1/windkit/spatial/_latitude.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     8724 2023-03-14 11:45:01.000000 windkit-0.6.1/windkit/spatial/_point.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    19130 2023-02-14 09:38:21.000000 windkit-0.6.1/windkit/spatial/_raster.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     7062 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/spatial/_struct.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     4062 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/spatial/_utm.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     2808 2023-02-14 09:38:21.000000 windkit-0.6.1/windkit/spatial/_vector.py
--rw-rw-r--   0 neil      (1000) neil      (1000)      300 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/spatial/_vertical.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     2530 2023-02-14 09:38:21.000000 windkit-0.6.1/windkit/spatial/decorators.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    25848 2023-03-14 11:45:01.000000 windkit-0.6.1/windkit/spatial/spatial.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     3694 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/time_series_wind_climate.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    18741 2023-03-14 11:45:01.000000 windkit-0.6.1/windkit/vector_map.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    11843 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/weibull.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    19416 2023-02-14 09:38:21.000000 windkit-0.6.1/windkit/weibull_wind_climate.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     3870 2023-01-31 04:56:55.000000 windkit-0.6.1/windkit/wind.py
--rw-rw-r--   0 neil      (1000) neil      (1000)     3611 2023-02-14 09:38:21.000000 windkit-0.6.1/windkit/wind_climate.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    22640 2023-03-14 11:45:01.000000 windkit-0.6.1/windkit/wind_turbine.py
--rw-rw-r--   0 neil      (1000) neil      (1000)    21523 2023-03-14 11:45:01.000000 windkit-0.6.1/windkit/workspace.py
-drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-03-16 11:56:45.599014 windkit-0.6.1/windkit.egg-info/
--rw-rw-r--   0 neil      (1000) neil      (1000)     4045 2023-03-16 11:56:45.000000 windkit-0.6.1/windkit.egg-info/PKG-INFO
--rw-rw-r--   0 neil      (1000) neil      (1000)     3368 2023-03-16 11:56:45.000000 windkit-0.6.1/windkit.egg-info/SOURCES.txt
--rw-rw-r--   0 neil      (1000) neil      (1000)        1 2023-03-16 11:56:45.000000 windkit-0.6.1/windkit.egg-info/dependency_links.txt
--rw-rw-r--   0 neil      (1000) neil      (1000)       63 2023-03-16 11:56:45.000000 windkit-0.6.1/windkit.egg-info/entry_points.txt
--rw-rw-r--   0 neil      (1000) neil      (1000)      244 2023-03-16 11:56:45.000000 windkit-0.6.1/windkit.egg-info/requires.txt
--rw-rw-r--   0 neil      (1000) neil      (1000)        8 2023-03-16 11:56:45.000000 windkit-0.6.1/windkit.egg-info/top_level.txt
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:22.022385 windkit-0.6.2/
+-rw-rw-r--   0 neil      (1000) neil      (1000)      461 2023-01-31 04:56:55.000000 windkit-0.6.2/.gitignore
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:21.986385 windkit-0.6.2/.gitlab/
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:21.998385 windkit-0.6.2/.gitlab/merge_request_templates/
+-rw-rw-r--   0 neil      (1000) neil      (1000)      491 2023-01-31 04:56:55.000000 windkit-0.6.2/.gitlab/merge_request_templates/default.md
+-rw-rw-r--   0 neil      (1000) neil      (1000)    12309 2023-03-14 11:45:01.000000 windkit-0.6.2/.gitlab-ci.yml
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1058 2023-03-14 11:45:01.000000 windkit-0.6.2/.pre-commit-config.yaml
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1261 2023-01-31 04:56:55.000000 windkit-0.6.2/.pylintrc
+-rw-rw-r--   0 neil      (1000) neil      (1000)    14505 2023-06-20 10:07:06.000000 windkit-0.6.2/CHANGELOG.md
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:21.998385 windkit-0.6.2/CI_helper_scripts/
+-rwxrwxr-x   0 neil      (1000) neil      (1000)      624 2023-01-31 04:56:55.000000 windkit-0.6.2/CI_helper_scripts/post_build_test_nix.sh
+-rwxrwxr-x   0 neil      (1000) neil      (1000)      680 2023-01-31 04:56:55.000000 windkit-0.6.2/CI_helper_scripts/post_build_test_win.sh
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1523 2023-01-31 04:56:55.000000 windkit-0.6.2/LICENSE
+-rw-rw-r--   0 neil      (1000) neil      (1000)      149 2023-02-14 09:38:21.000000 windkit-0.6.2/MANIFEST.in
+-rw-rw-r--   0 neil      (1000) neil      (1000)     4045 2023-06-20 10:08:22.022385 windkit-0.6.2/PKG-INFO
+-rw-rw-r--   0 neil      (1000) neil      (1000)     2634 2023-06-20 05:48:52.000000 windkit-0.6.2/README-Internal.md
+-rw-rw-r--   0 neil      (1000) neil      (1000)     3537 2023-01-31 04:56:55.000000 windkit-0.6.2/README.md
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:21.998385 windkit-0.6.2/docs/
+-rw-rw-r--   0 neil      (1000) neil      (1000)       82 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/.dockerignore
+-rw-rw-r--   0 neil      (1000) neil      (1000)       11 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/.gitignore
+-rw-rw-r--   0 neil      (1000) neil      (1000)      108 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/Dockerfile
+-rw-rw-r--   0 neil      (1000) neil      (1000)     7042 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/Makefile
+-rw-rw-r--   0 neil      (1000) neil      (1000)      559 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/docker-compose.yml
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:21.986385 windkit-0.6.2/docs/legacy/
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:21.998385 windkit-0.6.2/docs/legacy/dev/
+-rw-rw-r--   0 neil      (1000) neil      (1000)     2228 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/legacy/dev/dev-git.rst
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1759 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/legacy/dev/dev-intro.rst
+-rw-rw-r--   0 neil      (1000) neil      (1000)     2208 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/legacy/dev/dev-pytest.rst
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1418 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/legacy/dev/dev-sphinx.rst
+-rw-rw-r--   0 neil      (1000) neil      (1000)      239 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/nginx.conf
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:22.002385 windkit-0.6.2/docs/source/
+-rw-rw-r--   0 neil      (1000) neil      (1000)     9713 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/WAsP.bib
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:21.990385 windkit-0.6.2/docs/source/_templates/
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:22.002385 windkit-0.6.2/docs/source/_templates/autosummary/
+-rw-rw-r--   0 neil      (1000) neil      (1000)      585 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/_templates/autosummary/class.rst
+-rw-rw-r--   0 neil      (1000) neil      (1000)      693 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/_templates/autosummary/module.rst
+-rw-rw-r--   0 neil      (1000) neil      (1000)     9885 2023-03-14 11:45:01.000000 windkit-0.6.2/docs/source/conf.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)      125 2023-03-14 11:45:01.000000 windkit-0.6.2/docs/source/development_roadmap.rst
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1358 2023-03-14 11:45:01.000000 windkit-0.6.2/docs/source/index.rst
+-rw-rw-r--   0 neil      (1000) neil      (1000)     4567 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/installation.rst
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:22.002385 windkit-0.6.2/docs/source/io/
+-rw-rw-r--   0 neil      (1000) neil      (1000)     4014 2023-03-14 11:45:01.000000 windkit-0.6.2/docs/source/io/io.rst
+-rw-rw-r--   0 neil      (1000) neil      (1000)      241 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/map_conversion.rst
+-rw-rw-r--   0 neil      (1000) neil      (1000)       66 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/map_conversion_examples_nb.nblink
+-rw-rw-r--   0 neil      (1000) neil      (1000)      439 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/plotting.rst
+-rw-rw-r--   0 neil      (1000) neil      (1000)      301 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/plotting_examples.rst
+-rw-rw-r--   0 neil      (1000) neil      (1000)       53 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/plotting_examples_nb.nblink
+-rw-rw-r--   0 neil      (1000) neil      (1000)    10214 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/plotting_user_guide.rst
+-rw-rw-r--   0 neil      (1000) neil      (1000)      127 2023-03-14 11:45:01.000000 windkit-0.6.2/docs/source/release_notes.rst
+-rw-rw-r--   0 neil      (1000) neil      (1000)     4794 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/topographic_data.rst
+-rw-rw-r--   0 neil      (1000) neil      (1000)     3232 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/wind_climate_objects.rst
+-rw-rw-r--   0 neil      (1000) neil      (1000)     5859 2023-01-31 04:56:55.000000 windkit-0.6.2/docs/source/windkit.rst
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:22.006385 windkit-0.6.2/env/
+-rw-rw-r--   0 neil      (1000) neil      (1000)      498 2023-01-31 04:56:55.000000 windkit-0.6.2/env/Dockerfile.api
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1209 2023-03-14 11:45:01.000000 windkit-0.6.2/env/Dockerfile.ci
+-rw-rw-r--   0 neil      (1000) neil      (1000)      421 2023-01-31 04:56:55.000000 windkit-0.6.2/env/Dockerfile.miniconda
+-rw-rw-r--   0 neil      (1000) neil      (1000)      187 2023-03-14 11:45:01.000000 windkit-0.6.2/env/Makefile
+-rw-rw-r--   0 neil      (1000) neil      (1000)      891 2023-06-20 05:48:25.000000 windkit-0.6.2/env/conda-linux-64.lock
+-rw-rw-r--   0 neil      (1000) neil      (1000)    35182 2023-01-31 04:56:55.000000 windkit-0.6.2/env/conda-osx-64.lock
+-rw-rw-r--   0 neil      (1000) neil      (1000)    42058 2023-02-14 09:38:21.000000 windkit-0.6.2/env/conda-win-64.lock
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1692 2023-02-14 09:38:21.000000 windkit-0.6.2/env/create_locks.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1066 2023-03-14 11:45:01.000000 windkit-0.6.2/env/dev_env.yaml
+-rw-rw-r--   0 neil      (1000) neil      (1000)      186 2023-02-14 09:38:21.000000 windkit-0.6.2/env/pywasp.cfg
+-rw-rw-r--   0 neil      (1000) neil      (1000)      653 2023-02-14 09:38:21.000000 windkit-0.6.2/env/pywasp_env.yml
+-rw-rw-r--   0 neil      (1000) neil      (1000)      470 2023-02-14 09:38:21.000000 windkit-0.6.2/env/pywaspio_env.yml
+-rw-rw-r--   0 neil      (1000) neil      (1000)       78 2023-02-14 09:38:21.000000 windkit-0.6.2/env/windkit.ini
+-rw-rw-r--   0 neil      (1000) neil      (1000)      441 2023-02-07 11:47:48.000000 windkit-0.6.2/pyproject.toml
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:22.006385 windkit-0.6.2/recipe/
+-rw-rw-r--   0 neil      (1000) neil      (1000)      667 2023-03-14 11:45:01.000000 windkit-0.6.2/recipe/meta.yaml
+-rw-rw-r--   0 neil      (1000) neil      (1000)      962 2023-06-20 10:08:22.022385 windkit-0.6.2/setup.cfg
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:22.014385 windkit-0.6.2/windkit/
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1153 2023-06-20 05:48:25.000000 windkit-0.6.2/windkit/__init__.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1726 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/_errors.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     8505 2023-03-14 11:45:01.000000 windkit-0.6.2/windkit/_rvea_xml.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     2179 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/_validate.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)    11639 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/_vectormap_gml.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     5008 2023-03-14 11:45:01.000000 windkit-0.6.2/windkit/_vectormap_helpers.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)      160 2023-06-20 10:08:21.000000 windkit-0.6.2/windkit/_version.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)    37804 2023-02-14 09:38:21.000000 windkit-0.6.2/windkit/all_vars.json
+-rw-rw-r--   0 neil      (1000) neil      (1000)    32058 2023-02-14 09:38:21.000000 windkit-0.6.2/windkit/binned_wind_climate.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     4910 2023-06-20 05:48:25.000000 windkit-0.6.2/windkit/cfd.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)      155 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/config.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1030 2023-06-20 05:48:25.000000 windkit-0.6.2/windkit/data_structures.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1110 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/elevation_map.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)    17220 2023-06-20 05:27:05.000000 windkit-0.6.2/windkit/empty.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)    21529 2023-03-14 11:45:01.000000 windkit-0.6.2/windkit/generalized_wind_climate.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1131 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/geospatial_imports.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     9775 2023-02-14 09:38:21.000000 windkit-0.6.2/windkit/get_map.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     8201 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/landcover.py
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:22.018385 windkit-0.6.2/windkit/landcovertables/
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1943 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/landcovertables/CGLS-LC100.json
+-rw-rw-r--   0 neil      (1000) neil      (1000)     5736 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/landcovertables/CORINE.json
+-rw-rw-r--   0 neil      (1000) neil      (1000)     2643 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/landcovertables/Globcover.json
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1315 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/landcovertables/MODIS.json
+-rw-rw-r--   0 neil      (1000) neil      (1000)      883 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/landcovertables/WorldCover.json
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:22.018385 windkit-0.6.2/windkit/map_conversion/
+-rw-rw-r--   0 neil      (1000) neil      (1000)        0 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/map_conversion/__init__.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1757 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/map_conversion/helper_functions.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)    24213 2023-03-14 11:45:01.000000 windkit-0.6.2/windkit/map_conversion/lines2poly.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)    21612 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/map_conversion/poly2lines.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)    12972 2023-03-14 11:45:01.000000 windkit-0.6.2/windkit/map_file_header_to_epsg.json
+-rw-rw-r--   0 neil      (1000) neil      (1000)    16270 2023-06-20 05:48:25.000000 windkit-0.6.2/windkit/metadata.py
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:22.018385 windkit-0.6.2/windkit/plot/
+-rw-rw-r--   0 neil      (1000) neil      (1000)      889 2023-02-14 09:38:21.000000 windkit-0.6.2/windkit/plot/__init__.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1237 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/plot/_colormaps.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     3859 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/plot/_helpers.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     8517 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/plot/color.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)    16579 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/plot/histogram.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     2605 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/plot/landcover_map.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)    13441 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/plot/operational_curves.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     4040 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/plot/raster_plot.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     5476 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/plot/roughness_rose.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     5569 2023-06-20 05:48:25.000000 windkit-0.6.2/windkit/plot/vertical_profile.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     8993 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/plot/wind_rose.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)      981 2023-02-14 09:38:21.000000 windkit-0.6.2/windkit/plot/wind_turbine.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)    12330 2023-02-14 09:38:21.000000 windkit-0.6.2/windkit/raster_map.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1096 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/roughness_map.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     4708 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/sector.py
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:22.022385 windkit-0.6.2/windkit/spatial/
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1684 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/spatial/README.md
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1433 2023-03-14 11:45:01.000000 windkit-0.6.2/windkit/spatial/__init__.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     5989 2023-02-14 09:38:21.000000 windkit-0.6.2/windkit/spatial/_bbox.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     4003 2023-03-14 11:45:01.000000 windkit-0.6.2/windkit/spatial/_crs.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)      754 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/spatial/_cuboid.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     1432 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/spatial/_dimensions.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     4676 2023-02-14 09:38:21.000000 windkit-0.6.2/windkit/spatial/_interpolation.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)      775 2023-02-14 09:38:21.000000 windkit-0.6.2/windkit/spatial/_latitude.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     8724 2023-03-14 11:45:01.000000 windkit-0.6.2/windkit/spatial/_point.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)    19130 2023-05-16 14:34:54.000000 windkit-0.6.2/windkit/spatial/_raster.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     7062 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/spatial/_struct.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     4062 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/spatial/_utm.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     2808 2023-02-14 09:38:21.000000 windkit-0.6.2/windkit/spatial/_vector.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)      300 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/spatial/_vertical.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     2530 2023-02-14 09:38:21.000000 windkit-0.6.2/windkit/spatial/decorators.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)    25867 2023-06-20 05:48:25.000000 windkit-0.6.2/windkit/spatial/spatial.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)    13485 2023-06-20 05:48:25.000000 windkit-0.6.2/windkit/time_series_wind_climate.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)    18766 2023-06-20 05:48:25.000000 windkit-0.6.2/windkit/vector_map.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)    11843 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/weibull.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)    21666 2023-06-20 06:55:20.000000 windkit-0.6.2/windkit/weibull_wind_climate.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     3870 2023-01-31 04:56:55.000000 windkit-0.6.2/windkit/wind.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)     3611 2023-02-14 09:38:21.000000 windkit-0.6.2/windkit/wind_climate.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)    22640 2023-03-14 11:45:01.000000 windkit-0.6.2/windkit/wind_turbine.py
+-rw-rw-r--   0 neil      (1000) neil      (1000)    21523 2023-03-14 11:45:01.000000 windkit-0.6.2/windkit/workspace.py
+drwxrwxr-x   0 neil      (1000) neil      (1000)        0 2023-06-20 10:08:22.014385 windkit-0.6.2/windkit.egg-info/
+-rw-rw-r--   0 neil      (1000) neil      (1000)     4045 2023-06-20 10:08:21.000000 windkit-0.6.2/windkit.egg-info/PKG-INFO
+-rw-rw-r--   0 neil      (1000) neil      (1000)     3383 2023-06-20 10:08:21.000000 windkit-0.6.2/windkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 neil      (1000) neil      (1000)        1 2023-06-20 10:08:21.000000 windkit-0.6.2/windkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 neil      (1000) neil      (1000)       63 2023-06-20 10:08:21.000000 windkit-0.6.2/windkit.egg-info/entry_points.txt
+-rw-rw-r--   0 neil      (1000) neil      (1000)      244 2023-06-20 10:08:21.000000 windkit-0.6.2/windkit.egg-info/requires.txt
+-rw-rw-r--   0 neil      (1000) neil      (1000)        8 2023-06-20 10:08:21.000000 windkit-0.6.2/windkit.egg-info/top_level.txt
```

### Comparing `windkit-0.6.1/.gitlab-ci.yml` & `windkit-0.6.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/.pre-commit-config.yaml` & `windkit-0.6.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/.pylintrc` & `windkit-0.6.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/CHANGELOG.md` & `windkit-0.6.2/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,45 @@
 # Changelog
 
 All major changes are listed here.
 
-## 0.6.1
+## 0.6.2 (2023-06-20)
 
 ### New Features
 
+#### New file reading functions
+
+* `windkit.read_timeseries_from_pandas` and `windkit.read_timeseries_from_csv` build a time-series wind climate `xarray.Dataset` from time-series data in tabular form, either a `pandas` Dataframe or a `csv` file. The functions attempt to auto-detect the wind speed and wind direction columns based on a standard list of names if they are not provided.
+* `windkit.read_cfdres` reads a WAsP CFD `.cfdres` file into an `xarray.Dataset` structure.
+
+#### Detection of CRS from WAsP .map files
+
+* `windkit.read_vector_map` and by extension `windkit.read_elevation_map` and `windkit.read_roughness_map` now try to detect CRS information from the header of WAsP `.map` files, which can be added using recent versions of the WAsP MapEditor. In case there is a problem (e.g. wrong format) it will raise an error.
+
+#### Updates to vertical profile plotting
+
+* `windkit.plot.vertical_profile` Function now works for data arrays without their attributes set. If the height coordinate does not have attributes, `Height [m]` will be used for the y-axis. If the data variable to plot does not have attributes, `DataArray.name` will be used for the x-axis. 
+* `windkit.plot.vertical_profile` no longer allows plotting of objects with a `time` coordinate. This is due to performance limitations when plotting potentially thousands of points when a time-series object is passed.
+
+### Breaking changes
+
+* When creating a file using `windkit.to_rsffile` and `windkit.to_wrgfile` or reading a file using `wk.read_rsffile` and `wk.read_wrgfile`, the elevation variable has been renamed from `elevation` to `site_elev`. This now matches the variable name used in PyWAsP. 
+
+### Changes
+
+* `windkit.spatial.nearest_points` will issue a warning instead of a `ValueError` when it is used on datasets with geographical coordinates.
+* `windkit.to_rsffile` and `windkit.to_wrgfile` calculate necessary parameters met_fields, "power_density", "combined_A", "combined_k", and "wspd", from a wwc if they aren't included.
+
+### Bug Fixes
+
+* Fixed a formatting bug in `wk.to_rsffile` and `wk.to_wrgfile` that resulted in incorrect column widths.
+
+## 0.6.1 (2023-03-16)
+
+### New Features
 * `windkit.wtg_cp` function returns the power_coefficient for given wind speeds from an wind turbine generator.
 * Added lookup table to convert WAsP Map Editor named projections to EPSG codes. This allows for projection to be autodetected from some GWC files.
 
 ### Breaking changes
 
 * Removed `coords` from `windkit.read_gwc`. Instead you should use the separate `west_east`, `south_north`, and `height` arguments. Also removed `**kwargs`, as there was only a single option `header`, which is now its own argument.
 
@@ -24,15 +54,15 @@
 * Allow projections that don't have an EPSG code to be added using `windkit.spatial.add_crs`.
 * Scalar spatial datasets would fail in `windkit.spatial.count_spatial_points`.
 * Ensured that `wk.Workspace.get_gwc` could parse GWC objects from WAsP 12.7 and 12.8 workspaces.
 * Fixed bug in `windkit.spatial.to_stacked_point`, where the order of the `west_east` and `south_north` coordinates would be flipped from expected. This caused an issue when converting to `point` and then back to `stacked_point`.
 * Prevent creation of NaN values for some curves when using `windkit.read_wtg` to read ``.wtg`` files with different modes and different wind speed tables.
 * Bug fix in `wind_climate._is_bwc` where an exception was not properly caught.
 
-## 0.6.0
+## 0.6.0 (2023-01-29)
 
 Several new features in this release including support for Wind Turbines, the ability to convert roughness lines to roughness polygons, and the ability to read PWC files. Several important bug fixes also added.
 
 ### New Features
 
 #### Support for wind turbines and AEP data
```

### Comparing `windkit-0.6.1/CI_helper_scripts/post_build_test_nix.sh` & `windkit-0.6.2/CI_helper_scripts/post_build_test_nix.sh`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/CI_helper_scripts/post_build_test_win.sh` & `windkit-0.6.2/CI_helper_scripts/post_build_test_win.sh`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/LICENSE` & `windkit-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/PKG-INFO` & `windkit-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windkit
-Version: 0.6.1
+Version: 0.6.2
 Summary: WindKit provides core functionalities for working with wind resource data
 Home-page: https://docs-wasp.ramtt.xyz/windkit
 Author: DTU Wind Energy
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `windkit-0.6.1/README-Internal.md` & `windkit-0.6.2/README-Internal.md`

 * *Files 20% similar despite different names*

```diff
@@ -24,61 +24,43 @@
 
 ```sh
 export SETUPTOOLS_SCM_PRETEND_VERSION=<version>
 export TWINE_USERNAME=__token__
 export TWINE_PASSWORD=<global-token> # global token can be found in bitwarden under pypi, username wasp
 
 # Create build environment
-mamba create -n build boa build python=3.9 twine setuptools_scm
+mamba create -n build boa build python=3.9 twine setuptools_scm conda-verify
 conda activate build
 
 # install the package such that the above version code (in SETUPTOOLS_SCM_PRETEND_VERSION) will be written to the dist package that is uplaoded to pypi
-pip install --no-deps -e .
+pip install -e .
 
 # Build & deploy Pypi
 rm -r dist
 python -m build
 python3 -m twine upload dist/*
 
 # Build & deploy conda
 # This cannot be done from a submodule folder, windkit must be cloned in a different folder.
 rm -r conda_build
 export VERSION=<version>
 time conda mambabuild -c https://conda.windenergy.dtu.dk/channel/open --output-folder conda_build  ./recipe
 
-scp conda_build/*/*.tar.bz2 VIND-pWEBext01:~/.
-ssh VIND-pWEBext01
-  sudo mv *.tar.bz2 /mnt/data/external/rw/conda-channel/basic_auth_node_server/conda/open/noarch/.
-  sudo chown 1000:1000 /mnt/data/external/rw/conda-channel/basic_auth_node_server/conda/open/noarch/*.tar.bz2
-  # This may be running on any of the VIND-pWEBext machines. For now ping neda@dtu.dk to carry out these steps.
-  docker exec -it production_conda-channel_ci_deploy_storage /bin/bash
-    su conda_deploy
-    conda index ~/repos/open/
+rsync -auPv conda_build/ VIND-pWASPInt01:~/.
+ssh VIND-pWASPInt01
+  sudo rsync --ignore-existing -tprm --include=*/ --include=*.tar.bz2 --exclude=* conda_build/ /mnt/data/external/rw/conda-channel/basic_auth_node_server/conda/open/
+  sudo chown -R 1000:1000 /mnt/data/external/rw/conda-channel/basic_auth_node_server/conda/
   # To check whether it worked correctly, go to  https://conda.windenergy.dtu.dk/channel/open/noarch/
 ```
 
 ### Build and deploy docs
 
 Make sure you have an environment with all sphinx related dependencies.
 
 
 ```sh
 cd docs
 make clean
 make html
 # Copy to the machine
-rsync -avP --delete build/html VIND-pWEBext01:/web/static-documentation/setup_files/windkit_docs/windkit/
-
-ssh VIND-pWEBext01
-  cd /web/static-documentation/setup_files/windkit_docs/
-  #login with your dtu username and password
-  docker login registry.windenergy.dtu.dk
-  docker build -t registry.windenergy.dtu.dk/ram-tech-team/dockerhub-private/docs_windkit:0.5.1 .
-  docker push registry.windenergy.dtu.dk/ram-tech-team/dockerhub-private/docs_windkit:0.5.1
-
-  #update docker compose yaml
-  cd /web/static-documentation/
-  # edit docker-compose.yml to update docs_windkit image tag.
-  # run docker stack deploy
-  docker stack deploy -c docker-compose.yml static_project_documentation --with-registry-auth
-
+rsync -auPv --delete build/html VIND-pWASPint01:/mnt/data/external/ro/web_documentation/windkit
 ```
```

### Comparing `windkit-0.6.1/README.md` & `windkit-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/docs/Makefile` & `windkit-0.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/docs/docker-compose.yml` & `windkit-0.6.2/docs/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/docs/legacy/dev/dev-git.rst` & `windkit-0.6.2/docs/legacy/dev/dev-git.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/docs/legacy/dev/dev-intro.rst` & `windkit-0.6.2/docs/legacy/dev/dev-intro.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/docs/legacy/dev/dev-pytest.rst` & `windkit-0.6.2/docs/legacy/dev/dev-pytest.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/docs/legacy/dev/dev-sphinx.rst` & `windkit-0.6.2/docs/legacy/dev/dev-sphinx.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/docs/source/WAsP.bib` & `windkit-0.6.2/docs/source/WAsP.bib`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/docs/source/_templates/autosummary/class.rst` & `windkit-0.6.2/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/docs/source/_templates/autosummary/module.rst` & `windkit-0.6.2/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/docs/source/conf.py` & `windkit-0.6.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/docs/source/index.rst` & `windkit-0.6.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/docs/source/installation.rst` & `windkit-0.6.2/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/docs/source/io/io.rst` & `windkit-0.6.2/docs/source/io/io.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/docs/source/plotting_user_guide.rst` & `windkit-0.6.2/docs/source/plotting_user_guide.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/docs/source/topographic_data.rst` & `windkit-0.6.2/docs/source/topographic_data.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/docs/source/wind_climate_objects.rst` & `windkit-0.6.2/docs/source/wind_climate_objects.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/docs/source/windkit.rst` & `windkit-0.6.2/docs/source/windkit.rst`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/env/Dockerfile.ci` & `windkit-0.6.2/env/Dockerfile.ci`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/env/conda-linux-64.lock` & `windkit-0.6.2/env/conda-linux-64.lock`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/env/conda-osx-64.lock` & `windkit-0.6.2/env/conda-osx-64.lock`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/env/conda-win-64.lock` & `windkit-0.6.2/env/conda-win-64.lock`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/env/create_locks.py` & `windkit-0.6.2/env/create_locks.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/env/dev_env.yaml` & `windkit-0.6.2/env/dev_env.yaml`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/env/pywasp_env.yml` & `windkit-0.6.2/env/pywasp_env.yml`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/recipe/meta.yaml` & `windkit-0.6.2/recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/setup.cfg` & `windkit-0.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/__init__.py` & `windkit-0.6.2/windkit/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .binned_wind_climate import *
 from .generalized_wind_climate import *
 from .landcover import LandCoverTable
 from .raster_map import *
 from .vector_map import *
 from .roughness_map import read_roughness_map
 from .elevation_map import read_elevation_map
+from .cfd import read_cfdres
 from .empty import *
 from .weibull_wind_climate import *
 from .wind import (
     wind_speed,
     wind_direction,
     wind_speed_and_direction,
     wind_vectors,
@@ -28,10 +29,13 @@
     wtg_ct,
     WindTurbines,
 )
 from .workspace import Workspace
 from .weibull import *
 from .wind_climate import mean_windspeed, power_density
 from . import plot  # Order of imports matters
-
+from .time_series_wind_climate import (
+    read_timeseries_from_csv,
+    read_timeseries_from_pandas,
+)
 from .map_conversion.lines2poly import lines2poly
 from .map_conversion.poly2lines import poly2lines
```

### Comparing `windkit-0.6.1/windkit/_errors.py` & `windkit-0.6.2/windkit/_errors.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/_rvea_xml.py` & `windkit-0.6.2/windkit/_rvea_xml.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/_validate.py` & `windkit-0.6.2/windkit/_validate.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/_vectormap_gml.py` & `windkit-0.6.2/windkit/_vectormap_gml.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/_vectormap_helpers.py` & `windkit-0.6.2/windkit/_vectormap_helpers.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/all_vars.json` & `windkit-0.6.2/windkit/all_vars.json`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/binned_wind_climate.py` & `windkit-0.6.2/windkit/binned_wind_climate.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/data_structures.py` & `windkit-0.6.2/windkit/data_structures.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     LINCOM_WIND_LEVEL = "LINCOM Wind Level"
     LINCOM_WIND_POINT = "LINCOM Wind Point"
     V50_GUMBEL = "V50 Gumbel"
     MAP_TYPE = "Rastermap"
     MET = "Met fields"
     SPECTRUM = "Spectrum/spectral Correction Factor"
     TOPO_EFFECTS = "Topographic effects"
+    TOPO_CFD_EFFECTS = "Topographic CFD effects"
     WEIB = "Weibull Wind Climate"
     WASP_SITE_COND = "WAsP site conditions"
     LINCOM_GEWC = "LINCOM GEWC"
     TS = "Time Series Wind Climate"
     WTG = "Wind Turbine Generator"
     AEP = "Anual Energy Production"
     WF_FLOW_MAP = "Wind Farm Flow Map"
```

### Comparing `windkit-0.6.1/windkit/elevation_map.py` & `windkit-0.6.2/windkit/elevation_map.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/empty.py` & `windkit-0.6.2/windkit/empty.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/generalized_wind_climate.py` & `windkit-0.6.2/windkit/generalized_wind_climate.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/geospatial_imports.py` & `windkit-0.6.2/windkit/geospatial_imports.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/get_map.py` & `windkit-0.6.2/windkit/get_map.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/landcover.py` & `windkit-0.6.2/windkit/landcover.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/landcovertables/CGLS-LC100.json` & `windkit-0.6.2/windkit/landcovertables/CGLS-LC100.json`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/landcovertables/CORINE.json` & `windkit-0.6.2/windkit/landcovertables/CORINE.json`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/landcovertables/Globcover.json` & `windkit-0.6.2/windkit/landcovertables/Globcover.json`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/landcovertables/MODIS.json` & `windkit-0.6.2/windkit/landcovertables/MODIS.json`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/landcovertables/WorldCover.json` & `windkit-0.6.2/windkit/landcovertables/WorldCover.json`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/map_conversion/helper_functions.py` & `windkit-0.6.2/windkit/map_conversion/helper_functions.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/map_conversion/lines2poly.py` & `windkit-0.6.2/windkit/map_conversion/lines2poly.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/map_conversion/poly2lines.py` & `windkit-0.6.2/windkit/map_conversion/poly2lines.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/map_file_header_to_epsg.json` & `windkit-0.6.2/windkit/map_file_header_to_epsg.json`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/metadata.py` & `windkit-0.6.2/windkit/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,14 +292,25 @@
     "roughness_turnings": ALL_VARS_META["roughness_turnings"],
     "dirrix": ALL_VARS_META["dirrix"],
     "site_elev": ALL_VARS_META["elevation"],
     "rix": ALL_VARS_META["rix"],
     "object_type": DataStructures.TOPO_EFFECTS.value,
 }
 
+
+_TOPO_CFD_EFFECTS_ATTRS = {
+    "z0meso": ALL_VARS_META["z0meso"],
+    "cfd_speedups": ALL_VARS_META["cfd_speedups"],
+    "cfd_turnings": ALL_VARS_META["cfd_turnings"],
+    "cfd_turbulence_intensity": ALL_VARS_META["cfd_turbulence_intensity"],
+    "cfd_flow_inclination": ALL_VARS_META["cfd_flow_inclination"],
+    "site_elev": ALL_VARS_META["elevation"],
+    "object_type": DataStructures.TOPO_CFD_EFFECTS.value,
+}
+
 # this is the basic data structure returned by
 # a WAsP downscaling, in WAsP GUI often referred
 # to as the pwc (predicted wind climate)
 _WEIB_ATTRS = {
     "A": ALL_VARS_META["weib_A"],
     "k": ALL_VARS_META["weib_k"],
     "wdfreq": ALL_VARS_META["wdfreq"],
```

### Comparing `windkit-0.6.1/windkit/plot/__init__.py` & `windkit-0.6.2/windkit/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/plot/_colormaps.py` & `windkit-0.6.2/windkit/plot/_colormaps.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/plot/_helpers.py` & `windkit-0.6.2/windkit/plot/_helpers.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/plot/color.py` & `windkit-0.6.2/windkit/plot/color.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/plot/histogram.py` & `windkit-0.6.2/windkit/plot/histogram.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/plot/landcover_map.py` & `windkit-0.6.2/windkit/plot/landcover_map.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/plot/operational_curves.py` & `windkit-0.6.2/windkit/plot/operational_curves.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/plot/raster_plot.py` & `windkit-0.6.2/windkit/plot/raster_plot.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/plot/roughness_rose.py` & `windkit-0.6.2/windkit/plot/roughness_rose.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/plot/vertical_profile.py` & `windkit-0.6.2/windkit/plot/vertical_profile.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # (c) 2022 DTU Wind Energy
 """
 Vertical profile plotting
 """
 
-
+from .._errors import PlottingAttrsError, WindkitError
 from ._helpers import (
     HAS_PLOTLY,
     check_plotting_attrs,
     missing_arguments,
     requires_plotly,
 )
 
@@ -15,30 +15,30 @@
     import plotly.express as px
 
 
 def vertical_profile(
     da_meas=None, da_pred=None, color_bwc="red", color_wwc="dodgerblue"
 ):
     """Plots the vertical profile of the dataArray or dataArrays introduced. If
-    two dataArrays are given, one should represent mesured/observed data (as the one
+    two dataArrays are given, one should represent measured/observed data (as the one
     represented in a binned wind climate) and the other predicted/generalized
     data (as the one represented in a weibull wind climate). The function will
     plot both vertical profiles to compare.
     If one dataArray is give, the function plots its vertical profile.
 
     Parameters
     ----------
     da_meas : xarray.DataArray
-        WindKit DataArray representing a mesured/observed vertical profile data.
+        WindKit DataArray representing a measured/observed vertical profile data.
 
     da_pred : xarray.DataArray
         WindKit DataArray representing a predicted/generalized vertical profile data.
 
     color_bwc :  str, optional
-        Sets the color of the mesured/observed vertical profile plot.
+        Sets the color of the measured/observed vertical profile plot.
         Strings should define valid CSS-colors.
         By default is defined as "red".
 
     color_wwc :  str, optional
         Sets the color of the predicted/generalized vertical profile plot.
         Strings should define valid CSS-colors.
         By default is defined as "dodgerblue".
@@ -48,14 +48,21 @@
     plotly.graph_objects.Figure
         Plotly figure for display, additional modification, or output
 
     """
     requires_plotly()
 
     if da_meas is not None and da_pred is not None:
+        if (
+            "time" in da_meas.reset_coords().coords
+            or "time" in da_pred.reset_coords().coords
+        ):
+            raise WindkitError(
+                "DataArray is a timeseries and cannot be plotted as a vertical profile."
+            )
         da_meas = da_meas.squeeze()
         df_bwc = da_meas.to_dataframe().reset_index().dropna()
         da_pred = da_pred.squeeze()
         df_wwc = da_pred.to_dataframe().reset_index().dropna()
 
         plot_bwc_dict = {
             "x": da_meas.name,
@@ -67,57 +74,82 @@
             "x": da_pred.name,
             "y": "height",
             "custom_data": [da_pred.name, "height"],
             "color_discrete_sequence": [color_wwc],
         }
 
         for da in [da_meas, da_pred]:
-            xaxes_title = check_plotting_attrs(da)
-            yaxes_title = check_plotting_attrs(da["height"])
+            try:
+                xaxes_title = check_plotting_attrs(da)
+            except PlottingAttrsError:
+                xaxes_title = da.name
+            try:
+                yaxes_title = check_plotting_attrs(da["height"])
+            except PlottingAttrsError:
+                yaxes_title = "Height [m]"
 
         fig = px.scatter(df_bwc, **plot_bwc_dict)
-        fig["data"][0]["name"] = "Mesured"
+        fig["data"][0]["name"] = "Measured"
         fig["data"][0]["showlegend"] = True
 
         fig2 = px.line(df_wwc, **plot_wwc_dict)
         fig2["data"][0]["name"] = "Predicted"
         fig2["data"][0]["showlegend"] = True
         fig.add_trace(fig2.data[0])
 
     elif da_meas is not None and da_pred is None:
+        if "time" in da_meas.reset_coords().coords:
+            raise WindkitError(
+                "DataArray is a timeseries and cannot be plotted as a vertical profile."
+            )
         da_meas = da_meas.squeeze()
         df_bwc = da_meas.to_dataframe().reset_index().dropna()
 
         plot_bwc_dict = {
             "x": da_meas.name,
             "y": "height",
             "custom_data": [da_meas.name, "height"],
             "color_discrete_sequence": [color_bwc],
         }
 
-        xaxes_title = check_plotting_attrs(da_meas)
-        yaxes_title = check_plotting_attrs(da_meas["height"])
+        try:
+            xaxes_title = check_plotting_attrs(da_meas)
+        except PlottingAttrsError:
+            xaxes_title = da_meas.name
+        try:
+            yaxes_title = check_plotting_attrs(da_meas["height"])
+        except PlottingAttrsError:
+            yaxes_title = "Height [m]"
 
         fig = px.scatter(df_bwc, **plot_bwc_dict)
-        fig["data"][0]["name"] = "Mesured"
+        fig["data"][0]["name"] = "Measured"
         fig["data"][0]["showlegend"] = True
 
     elif da_meas is None and da_pred is not None:
+        if "time" in da_pred.reset_coords().coords:
+            raise WindkitError(
+                "DataArray is a timeseries and cannot be plotted as a vertical profile."
+            )
         da_pred = da_pred.squeeze()
         df_wwc = da_pred.to_dataframe().reset_index().dropna()
 
         plot_wwc_dict = {
             "x": da_pred.name,
             "y": "height",
             "custom_data": [da_pred.name, "height"],
             "color_discrete_sequence": [color_wwc],
         }
-
-        xaxes_title = check_plotting_attrs(da_pred)
-        yaxes_title = check_plotting_attrs(da_pred["height"])
+        try:
+            xaxes_title = check_plotting_attrs(da_pred)
+        except PlottingAttrsError:
+            xaxes_title = da_pred.name
+        try:
+            yaxes_title = check_plotting_attrs(da_pred["height"])
+        except PlottingAttrsError:
+            yaxes_title = "Height [m]"
 
         fig = px.line(df_wwc, **plot_wwc_dict)
         fig["data"][0]["name"] = "Predicted"
         fig["data"][0]["showlegend"] = True
 
     else:
         missing_arguments("vertical_profile()", ["da_bwc", "da_wwc"])
```

### Comparing `windkit-0.6.1/windkit/plot/wind_rose.py` & `windkit-0.6.2/windkit/plot/wind_rose.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/plot/wind_turbine.py` & `windkit-0.6.2/windkit/plot/wind_turbine.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/raster_map.py` & `windkit-0.6.2/windkit/raster_map.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/roughness_map.py` & `windkit-0.6.2/windkit/roughness_map.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/sector.py` & `windkit-0.6.2/windkit/sector.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/spatial/README.md` & `windkit-0.6.2/windkit/spatial/README.md`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/spatial/__init__.py` & `windkit-0.6.2/windkit/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/spatial/_bbox.py` & `windkit-0.6.2/windkit/spatial/_bbox.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/spatial/_crs.py` & `windkit-0.6.2/windkit/spatial/_crs.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/spatial/_cuboid.py` & `windkit-0.6.2/windkit/spatial/_cuboid.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/spatial/_dimensions.py` & `windkit-0.6.2/windkit/spatial/_dimensions.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/spatial/_interpolation.py` & `windkit-0.6.2/windkit/spatial/_interpolation.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/spatial/_latitude.py` & `windkit-0.6.2/windkit/spatial/_latitude.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/spatial/_point.py` & `windkit-0.6.2/windkit/spatial/_point.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/spatial/_raster.py` & `windkit-0.6.2/windkit/spatial/_raster.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/spatial/_struct.py` & `windkit-0.6.2/windkit/spatial/_struct.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/spatial/_utm.py` & `windkit-0.6.2/windkit/spatial/_utm.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/spatial/_vector.py` & `windkit-0.6.2/windkit/spatial/_vector.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/spatial/decorators.py` & `windkit-0.6.2/windkit/spatial/decorators.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/spatial/spatial.py` & `windkit-0.6.2/windkit/spatial/spatial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # (c) 2022 DTU Wind Energy
 """
 Public interface to all of the spatial tools in WindKit
 """
 import logging
+import warnings
 
 import numpy as np
 import pyproj
 import xarray as xr
 from scipy.spatial import KDTree
 
 from windkit.geospatial_imports import is_GeoDataFrame, is_GeoSeries
@@ -721,16 +722,16 @@
 
     Returns
     -------
     xr.Dataset
         ds but with the nearest points provided in ds_target (i.e. ds will have the shape of ds_target)
     """
     if get_crs(ds).is_geographic or get_crs(ds_target).is_geographic:
-        raise ValueError(
-            "Can only do nearest neighbour lookup in metric coordinate systems!"
+        warnings.warn(
+            "You are doing nearest neighbour lookup in non metric coordinate systems!"
         )
     if get_crs(ds) != get_crs(ds_target):
         raise ValueError("Datasets must have the same coordinate system!")
 
     # stack so that we also work with point structure
     ds = spatial_stack(ds)
```

### Comparing `windkit-0.6.1/windkit/vector_map.py` & `windkit-0.6.2/windkit/vector_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,17 +93,18 @@
     map_type_code = _MAP_TYPE_CODES[map_type]
     if map_type == "landmask":
         map_type_code = _MAP_TYPE_CODES["roughness"]
 
     #############
     # Handle CRS
     #############
-    # TODO: Add CRS autodetection from header
     if crs is None:
-        raise ValueError("""'crs' cannot be detected from file""")
+        crs = _crs_from_map_file(filename)
+        if crs is None:
+            raise ValueError("""'crs' cannot be detected from file""")
 
     with open(filename, "r", newline="\r\n") as fobj:
         # Read 4 header lines into a single string
         for _ in range(4):
             metadata += fobj.readline()
 
         # Process remaining data
```

### Comparing `windkit-0.6.1/windkit/weibull.py` & `windkit-0.6.2/windkit/weibull.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/weibull_wind_climate.py` & `windkit-0.6.2/windkit/weibull_wind_climate.py`

 * *Files 5% similar despite different names*

```diff
@@ -163,86 +163,91 @@
         structure (dimensions south_north, west_east, height).
 
     Returns
     -------
     wwc: xarray.Dataset
         Weibull wind climate dataset.
     """
+    if crs is None:
+        raise ValueError("crs must be specified")
 
     has_wrg_header = _has_wrg_header(resource_file)
     nsec = _infer_resource_file_nsec(resource_file, skip_first=has_wrg_header)
 
     df = pd.read_fwf(
         resource_file,
         widths=tuple([10, 10, 10, 8, 5, 5, 6, 15, 3] + [4, 4, 5] * nsec),
         header=None,
         skiprows=int(has_wrg_header),
     )
 
     header = [
-        "Name",
+        "name",
         "west_east",
         "south_north",
-        "elevation",
+        "site_elev",
         "height",
         "A_combined",
         "k_combined",
         "power_density",
         "nsec",
     ]
 
     for i in range(1, nsec + 1):
         header += f"f_{i} A_{i} k_{i}".split()
 
     df.columns = header
 
     can_be_raster = _raster._can_be_raster(df["west_east"], df["south_north"])
 
-    df = df.set_index(["Name"])
+    df = df.set_index(["name"])
 
     wwc = df.to_xarray()
 
-    wwc = wwc.assign_coords(point=(("Name",), np.arange(len(df.index))))
-    wwc = wwc.swap_dims({"Name": "point"})
+    wwc = wwc.assign_coords(point=(("name",), np.arange(len(df.index))))
+    wwc = wwc.swap_dims({"name": "point"})
     wwc = wwc.assign_coords(
         west_east=(("point",), wwc.west_east.values),
         south_north=(("point",), wwc.south_north.values),
         height=(("point",), wwc.height.values),
     )
 
     knames = [f"k_{sec}" for sec in range(1, nsec + 1)]
     Anames = [f"A_{sec}" for sec in range(1, nsec + 1)]
     fnames = [f"f_{sec}" for sec in range(1, nsec + 1)]
 
     wwc["k"] = xr.concat([wwc[n] for n in knames], dim="sector")
     wwc["A"] = xr.concat([wwc[n] for n in Anames], dim="sector")
     wwc["wdfreq"] = xr.concat([wwc[n] for n in fnames], dim="sector")
 
-    wwc["elevation"] = wwc["elevation"].astype(np.float64)
+    wwc["site_elev"] = wwc["site_elev"].astype(np.float64)
     wwc["k"] = wwc["k"] / 100.0
     wwc["A"] = wwc["A"] / 10.0
     wwc["wdfreq"] = wwc["wdfreq"] / wwc["wdfreq"].sum(dim="sector")
 
     wwc = wwc.drop_vars(
         ["nsec"]
-        + [f"k_{sec}" for sec in range(1, nsec + 1)]
-        + [f"A_{sec}" for sec in range(1, nsec + 1)]
         + [f"f_{sec}" for sec in range(1, nsec + 1)]
+        + [f"A_{sec}" for sec in range(1, nsec + 1)]
+        + [f"k_{sec}" for sec in range(1, nsec + 1)]
     )
 
     wwc = add_crs(wwc, crs)
     wdcenters = create_sector_coords(nsec)
     wwc = wwc.assign_coords(**wdcenters.coords)
 
     if (not can_be_raster) and to_cuboid:
         logging.warning(
             "_read_resource_file: Data cannot be converted to raster, returning point."
         )
     if can_be_raster and to_cuboid:
         wwc = to_raster(wwc)
+        if "elevation" in wwc.data_vars:
+            wwc["elevation"] = wwc["elevation"].isel(height=0)
+
     wwc = update_var_attrs(wwc, _WEIB_ATTRS)
     return update_history(wwc)
 
 
 def read_rsffile(rsffile, crs=None, to_cuboid=False, **kwargs):
     """Reads .rsf file into a weibull wind climate dataset.
 
@@ -334,65 +339,141 @@
 def _to_resource_file(wwc, rsffile, wrg_header=False):
     """Write weibull wind climate dataset to a resource file (.rsf or .wrg).
 
     Parameters
     ----------
     wwc : xarray.Dataset
         Weibull wind climate xarray dataset.
-    rsffile: str
+
+    rsffile : str
         Path to resource file
+
+    wrg_header : bool
+        If True, the WRG header will be added to the file.
+        Requires a cuboid dataset.
+
     """
 
-    # TODO: 2. make sure sum of written values sum to 100 or 1000
-    # order = ['Name', 'west_east', 'south_north', 'elevation',
-    #          'height', 'A_combined', 'k_combined', 'power_density', 'nsec']
+    # Check if wwc has unsupported dimensions
+    approved_dims = [
+        "sector",
+        "point",
+        "stacked_point",
+        "south_north",
+        "west_east",
+        "height",
+    ]
+    if any([dim not in approved_dims for dim in wwc.dims]):
+        raise ValueError(
+            f"Unsupported dimensions in wwc: {wwc.dims}. "
+            f"Supported dimensions: {approved_dims}"
+        )
+
     wwc_cp = wwc.copy()
 
     if wrg_header:
         if not is_cuboid(wwc):
             raise ValueError("WWC must be a 'cuboid' to add WRG header!")
         header = _wrg_header(wwc)
 
-    # The code below this line works if these vars are deleted. It was like that
-    # originally.
-    wwc_cp = wwc_cp.drop_vars(["sector", "sector_ceil", "sector_floor", "crs"])
+    # I feel like it would be cleaner to throw a key error or we always
+    # return the parameters required from `downscale()`. But adding the vars
+    # as needed works as well.
+    if "A_combined" not in wwc_cp.data_vars:
+        wwc_cp[["A_combined", "k_combined"]] = weibull_combined(wwc_cp)
+    if "wspd" not in wwc_cp.data_vars:
+        wwc_cp["wspd"] = wwc_mean_windspeed(wwc_cp)
+    if "power_density" not in wwc_cp.data_vars:
+        try:
+            air_dens = wwc_cp["air_density"]
+        except KeyError:
+            air_dens = 1.225
+        wwc_cp["power_density"] = wwc_power_density(wwc_cp, air_dens)
+
+    # remove unneeded vars
+    wwc_cp = wwc_cp.drop_vars(
+        ["sector", "sector_ceil", "sector_floor", "crs"], errors="ignore"
+    )
 
+    nsec = wwc_cp.dims["sector"]
     wwc_cp["A"] = (wwc_cp["A"] * 10.0).astype(np.int16)
     wwc_cp["k"] = (wwc_cp["k"] * 100.0).astype(np.int16)
     wwc_cp["wdfreq"] = (wwc_cp["wdfreq"] * 1000.0).astype(np.int16)
+    wwc_cp["site_elev"] = wwc_cp["site_elev"].astype(np.int16)
+    wwc_cp["nsec"] = xr.full_like(wwc_cp["site_elev"], nsec, dtype=np.int16)
 
-    df = wwc_cp["elevation"].to_dataframe().reset_index()
-    new_columns = ["point", "Name", "west_east", "south_north", "elevation", "height"]
-    df = df.reindex(columns=new_columns)
-
-    df = df.merge(wwc_cp["A_combined"].to_dataframe().reset_index())
-    df = df.merge(wwc_cp["k_combined"].to_dataframe().reset_index())
-    df = df.merge(wwc_cp["power_density"].to_dataframe().reset_index())
-    df.loc[:, "nsec"] = wwc_cp.dims["sector"]
-
-    freq_sec = list(wwc_cp["wdfreq"].groupby("sector"))
-    A_sec = list(wwc_cp["A"].groupby("sector"))
-    k_sec = list(wwc_cp["k"].groupby("sector"))
-
-    for isec in range(wwc_cp.dims["sector"]):
-        wdfreq = freq_sec[isec][1].to_dataframe(name=f"wdfreq_{isec+1}").reset_index()
-        A = A_sec[isec][1].to_dataframe(name=f"A_{isec+1}").reset_index()
-        k = k_sec[isec][1].to_dataframe(name=f"k_{isec+1}").reset_index()
-        df = df.merge(wdfreq).merge(A).merge(k)
+    # select variables that do not depend on wind direction sector
+    vars = [
+        "name",
+        "west_east",
+        "south_north",
+        "site_elev",
+        "height",
+        "A_combined",
+        "k_combined",
+        "power_density",
+        "nsec",
+    ]
+
+    df = wwc_cp[
+        ["site_elev", "A_combined", "k_combined", "power_density", "nsec"]
+    ].to_dataframe()
+
+    if "name" not in df.columns:
+        df["name"] = "GridPoint"  # insert text column at first position
+
+    # select variables that depend on wind direction sector
+    sec_vars = [str((var, sec)) for sec in range(nsec) for var in ["wdfreq", "A", "k"]]
+    df_sec = wwc_cp[["wdfreq", "A", "k"]].to_dataframe()
+    df_sec = df_sec.pivot_table(
+        index=df.index.names, columns="sector", values=["wdfreq", "A", "k"]
+    )
+
+    # merge all-sector and sectorwise values
+    df_total = (
+        pd.concat([df, df_sec], axis=1)
+        .reset_index()
+        .drop(["point", "stacked_point"], axis=1, errors="ignore")
+    )  # concat combined and sectorwise values
+    # transform all column names to string to make it compatible with pandas 1.4
+    df_total.columns = [str(x) for x in df_total.columns]
+    df_total = df_total[vars + sec_vars]  # select vars in correct order
 
-    df = df.drop(columns=["point"])
-    nsec = int(df["nsec"].values[0])
     widths_offset = tuple([9, 9, 9, 7, 4, 4, 5, 14, 2] + [3, 3, 4] * nsec)
-    str_list = df.to_string(
+
+    formatters = [
+        lambda x: f"{x:>9}",  # name
+        lambda x: f"{x:>9.1f}",  # west_east
+        lambda x: f"{x:>9.1f}",  # south_north
+        lambda x: f"{x:>7.0f}",  # elevation
+        lambda x: f"{x:>4.1f}",  # height
+        lambda x: f"{x:>4.2f}",  # A_combined
+        lambda x: f"{x:>5.3f}",  # k_combined
+        lambda x: f"{x:>14.0f}",  # power_density
+        lambda x: f"{x:>2}",  # nsec
+    ]
+
+    for isec in range(nsec):
+        formatters.extend(
+            [
+                lambda x: f"{x:>3}",  # wdfreq
+                lambda x: f"{x:>3}",  # A
+                lambda x: f"{x:>4}",  # k
+            ]
+        )
+
+    str_list = df_total.to_string(
         header=False,
         index=False,
         index_names=False,
         col_space=widths_offset,
+        formatters=formatters,
         justify="left",
     )
+
     with open(rsffile, "w", newline="\r\n") as text_file:
         if wrg_header:
             text_file.write(header + "\n")
         text_file.write(str_list)
 
 
 def to_rsffile(wwc, rsffile, wrg_header=False):
@@ -443,29 +524,29 @@
     """
 
     def _rename_var(var):
         """
         Function to rename WAsP variable names to short hand name
         """
         _rename = {
-            "Flow inclination": "flow_inc",
-            "Mean speed": "ws_mean",
-            "Meso roughness": "meso_rgh",
-            "Obstacles speed": "obst_spd",
-            "Orographic speed": "orog_spd",
-            "Orographic turn": "orog_trn",
+            "Flow inclination": "flow_inclination",
+            "Mean speed": "wspd",
+            "Meso roughness": "z0meso",
+            "Obstacles speed": "obstacle_speedups",
+            "Orographic speed": "orographic_speedups",
+            "Orographic turn": "orographic_turnings",
             "Power density": "power_density",
             "RIX": "rix",
-            "Roughness changes": "rgh_change",
-            "Roughness speed": "rgh_spd",
+            "Roughness changes": "nrch",
+            "Roughness speed": "roughness_speedups",
             "Sector frequency": "wdfreq",
-            "Turbulence intensity": "tke",
+            "Turbulence intensity": "turbulence_intensity",
             "Weibull-A": "A",
             "Weibull-k": "k",
-            "Elevation": "elevation",
+            "Elevation": "site_elev",
         }
 
         return _rename[var]
 
     def _read_grd_data(filename):
         def _parse_line_floats(f):
             return [float(i) for i in f.readline().strip().split()]
@@ -509,20 +590,20 @@
         values = values[..., np.newaxis]
 
         if not meta["sector"].lower() == "all":
             dims += ["sector"]
             coords["sector"] = [int(meta["sector"])]
             values = values[..., np.newaxis]
         else:
-            if meta["var"] != "elevation":
+            if meta["var"] != "site_elev":
                 meta["var"] = meta["var"] + "_combined"
 
         da = xr.DataArray(values, dims=dims, coords=coords, name=meta["var"])
 
-        if da.name == "elevation":
+        if da.name == "site_elev":
             da = da.isel(height=0, drop=True)
 
         return da
 
     if not isinstance(grdfiles, list):
         grdfiles = [grdfiles]
```

### Comparing `windkit-0.6.1/windkit/wind.py` & `windkit-0.6.2/windkit/wind.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/wind_climate.py` & `windkit-0.6.2/windkit/wind_climate.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/wind_turbine.py` & `windkit-0.6.2/windkit/wind_turbine.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit/workspace.py` & `windkit-0.6.2/windkit/workspace.py`

 * *Files identical despite different names*

### Comparing `windkit-0.6.1/windkit.egg-info/PKG-INFO` & `windkit-0.6.2/windkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windkit
-Version: 0.6.1
+Version: 0.6.2
 Summary: WindKit provides core functionalities for working with wind resource data
 Home-page: https://docs-wasp.ramtt.xyz/windkit
 Author: DTU Wind Energy
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `windkit-0.6.1/windkit.egg-info/SOURCES.txt` & `windkit-0.6.2/windkit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 windkit/_rvea_xml.py
 windkit/_validate.py
 windkit/_vectormap_gml.py
 windkit/_vectormap_helpers.py
 windkit/_version.py
 windkit/all_vars.json
 windkit/binned_wind_climate.py
+windkit/cfd.py
 windkit/config.py
 windkit/data_structures.py
 windkit/elevation_map.py
 windkit/empty.py
 windkit/generalized_wind_climate.py
 windkit/geospatial_imports.py
 windkit/get_map.py
```

