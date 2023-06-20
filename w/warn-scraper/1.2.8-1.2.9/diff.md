# Comparing `tmp/warn-scraper-1.2.8.tar.gz` & `tmp/warn-scraper-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warn-scraper-1.2.8.tar", last modified: Sun Jul  3 23:35:48 2022, max compression
+gzip compressed data, was "warn-scraper-1.2.9.tar", last modified: Fri Jul  8 18:46:41 2022, max compression
```

## Comparing `warn-scraper-1.2.8.tar` & `warn-scraper-1.2.9.tar`

### file list

```diff
@@ -1,148 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 23:35:48.010334 warn-scraper-1.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 23:35:47.990333 warn-scraper-1.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 23:35:47.994334 warn-scraper-1.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     4962 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/.github/workflows/continuous-deployment.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1296 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3552 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     1841 2022-07-03 23:35:48.010334 warn-scraper-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/Pipfile
--rw-r--r--   0 runner    (1001) docker     (121)    85811 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 23:35:47.994334 warn-scraper-1.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 23:35:47.998334 warn-scraper-1.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)   894555 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/_static/R42693.pdf
--rw-r--r--   0 runner    (1001) docker     (121)   528620 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/_static/gao-03-1003.pdf
--rw-r--r--   0 runner    (1001) docker     (121)   184127 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/_static/releasing-actions-finished.png
--rw-r--r--   0 runner    (1001) docker     (121)   185718 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/_static/releasing-actions-start.png
--rw-r--r--   0 runner    (1001) docker     (121)   174370 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/_static/releasing-changelog-button.png
--rw-r--r--   0 runner    (1001) docker     (121)   177217 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/_static/releasing-changelog-entered.png
--rw-r--r--   0 runner    (1001) docker     (121)   129429 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/_static/releasing-draft-button.png
--rw-r--r--   0 runner    (1001) docker     (121)   170326 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/_static/releasing-name-release.png
--rw-r--r--   0 runner    (1001) docker     (121)   176171 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/_static/releasing-name-tag.png
--rw-r--r--   0 runner    (1001) docker     (121)   160943 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/_static/releasing-publish-button.png
--rw-r--r--   0 runner    (1001) docker     (121)   139063 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/_static/releasing-pypi.png
--rw-r--r--   0 runner    (1001) docker     (121)   115853 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/_static/releasing-release-published.png
--rw-r--r--   0 runner    (1001) docker     (121)   217800 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/_static/releasing-releases-button.png
--rw-r--r--   0 runner    (1001) docker     (121)   171004 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/_static/releasing-tag-button.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 23:35:47.998334 warn-scraper-1.2.8/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/_templates/sources.md.tmpl
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)    10377 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)     2721 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4416 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/releasing.md
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 23:35:48.002334 warn-scraper-1.2.8/docs/scrapers/
--rw-r--r--   0 runner    (1001) docker     (121)     1579 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/scrapers/al.md
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/scrapers/az.md
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/scrapers/ca.md
--rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/scrapers/co.md
--rw-r--r--   0 runner    (1001) docker     (121)      454 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/scrapers/dc.md
--rw-r--r--   0 runner    (1001) docker     (121)      744 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/scrapers/de.md
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/scrapers/ia.md
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/scrapers/in.md
--rw-r--r--   0 runner    (1001) docker     (121)     4308 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/scrapers/job_center.md
--rw-r--r--   0 runner    (1001) docker     (121)      997 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/scrapers/ks.md
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/scrapers/md.md
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/scrapers/me.md
--rw-r--r--   0 runner    (1001) docker     (121)     2032 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/scrapers/mo.md
--rw-r--r--   0 runner    (1001) docker     (121)     1973 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/scrapers/ny.md
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/scrapers/ok.md
--rw-r--r--   0 runner    (1001) docker     (121)     1496 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/scrapers/or.md
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/scrapers/sc.md
--rw-r--r--   0 runner    (1001) docker     (121)     3424 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/scrapers/tx.md
--rw-r--r--   0 runner    (1001) docker     (121)      430 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/scrapers/ut.md
--rw-r--r--   0 runner    (1001) docker     (121)      679 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/scrapers/va.md
--rw-r--r--   0 runner    (1001) docker     (121)      963 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/scrapers/vt.md
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/scrapers/wi.md
--rw-r--r--   0 runner    (1001) docker     (121)    10753 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/sources.md
--rw-r--r--   0 runner    (1001) docker     (121)     1363 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-07-03 23:35:48.010334 warn-scraper-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5353 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 23:35:48.002334 warn-scraper-1.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 23:35:48.002334 warn-scraper-1.2.8/tests/cassettes/
--rw-r--r--   0 runner    (1001) docker     (121)    48934 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/tests/cassettes/test_cached_detail_pages.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    34866 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/tests/cassettes/test_cached_search_results.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   209861 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/tests/cassettes/test_delete.yaml
--rw-r--r--   0 runner    (1001) docker     (121)   209861 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/tests/cassettes/test_iowa.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    33645 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/tests/cassettes/test_missing_detail_page_values.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16676 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/tests/cassettes/test_no_results.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    35299 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/tests/cassettes/test_paged_results.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    48760 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/tests/cassettes/test_scrape_integration.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     2156 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 23:35:48.002334 warn-scraper-1.2.8/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/tests/fixtures/2021_page_1.html
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/tests/fixtures/2021_page_2.html
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/tests/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (121)     4997 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/tests/test_job_center.py
--rw-r--r--   0 runner    (1001) docker     (121)     3506 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/tests/test_job_center_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/tests/test_openpyxl.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 23:35:48.006334 warn-scraper-1.2.8/warn/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5502 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     2019 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 23:35:48.006334 warn-scraper-1.2.8/warn/platforms/
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 23:35:48.006334 warn-scraper-1.2.8/warn/platforms/job_center/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/platforms/job_center/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/platforms/job_center/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)    10009 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/platforms/job_center/site.py
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/platforms/job_center/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     5436 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/platforms/job_center/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1894 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 23:35:48.010334 warn-scraper-1.2.8/warn/scrapers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1847 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/ak.py
--rw-r--r--   0 runner    (1001) docker     (121)     2240 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/al.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1222 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/az.py
--rw-r--r--   0 runner    (1001) docker     (121)     7262 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/ca.py
--rw-r--r--   0 runner    (1001) docker     (121)     4228 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/ct.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4021 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/dc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1316 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/de.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9429 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/fl.py
--rw-r--r--   0 runner    (1001) docker     (121)     3484 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/ga.py
--rw-r--r--   0 runner    (1001) docker     (121)     2087 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/ia.py
--rw-r--r--   0 runner    (1001) docker     (121)     4600 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/id.py
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/il.py
--rw-r--r--   0 runner    (1001) docker     (121)     2539 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/in.py
--rw-r--r--   0 runner    (1001) docker     (121)     1266 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/ks.py
--rw-r--r--   0 runner    (1001) docker     (121)     4222 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/ky.py
--rw-r--r--   0 runner    (1001) docker     (121)    12047 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/la.py
--rw-r--r--   0 runner    (1001) docker     (121)     2774 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/md.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1172 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/me.py
--rw-r--r--   0 runner    (1001) docker     (121)     3527 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/mi.py
--rw-r--r--   0 runner    (1001) docker     (121)     3469 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/mo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2294 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/mt.py
--rw-r--r--   0 runner    (1001) docker     (121)     4090 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/ne.py
--rw-r--r--   0 runner    (1001) docker     (121)     2231 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/nj.py
--rw-r--r--   0 runner    (1001) docker     (121)     3581 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/nm.py
--rw-r--r--   0 runner    (1001) docker     (121)     3545 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/ny.py
--rw-r--r--   0 runner    (1001) docker     (121)     5640 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/oh.py
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/ok.py
--rw-r--r--   0 runner    (1001) docker     (121)     1683 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/or.py
--rw-r--r--   0 runner    (1001) docker     (121)     1977 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/ri.py
--rw-r--r--   0 runner    (1001) docker     (121)     4736 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/sc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1904 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/sd.py
--rw-r--r--   0 runner    (1001) docker     (121)     4480 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/tn.py
--rw-r--r--   0 runner    (1001) docker     (121)     4351 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/tx.py
--rw-r--r--   0 runner    (1001) docker     (121)     1825 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/ut.py
--rw-r--r--   0 runner    (1001) docker     (121)     1554 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/va.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1186 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/vt.py
--rw-r--r--   0 runner    (1001) docker     (121)     4021 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/wa.py
--rw-r--r--   0 runner    (1001) docker     (121)     3531 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/scrapers/wi.py
--rw-r--r--   0 runner    (1001) docker     (121)     5200 2022-07-03 23:35:28.000000 warn-scraper-1.2.8/warn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 23:35:48.010334 warn-scraper-1.2.8/warn_scraper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1841 2022-07-03 23:35:47.000000 warn-scraper-1.2.8/warn_scraper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3214 2022-07-03 23:35:47.000000 warn-scraper-1.2.8/warn_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-03 23:35:47.000000 warn-scraper-1.2.8/warn_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-07-03 23:35:47.000000 warn-scraper-1.2.8/warn_scraper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-03 23:35:47.000000 warn-scraper-1.2.8/warn_scraper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-07-03 23:35:47.000000 warn-scraper-1.2.8/warn_scraper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-07-03 23:35:47.000000 warn-scraper-1.2.8/warn_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 18:46:41.814078 warn-scraper-1.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 18:46:41.794078 warn-scraper-1.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 18:46:41.794078 warn-scraper-1.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     4962 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/.github/workflows/continuous-deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1296 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3552 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)     1841 2022-07-08 18:46:41.814078 warn-scraper-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      615 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (121)    85811 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (121)      663 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 18:46:41.798078 warn-scraper-1.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      711 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 18:46:41.802078 warn-scraper-1.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)   894555 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/_static/R42693.pdf
+-rw-r--r--   0 runner    (1001) docker     (121)   528620 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/_static/gao-03-1003.pdf
+-rw-r--r--   0 runner    (1001) docker     (121)   184127 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/_static/releasing-actions-finished.png
+-rw-r--r--   0 runner    (1001) docker     (121)   185718 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/_static/releasing-actions-start.png
+-rw-r--r--   0 runner    (1001) docker     (121)   174370 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/_static/releasing-changelog-button.png
+-rw-r--r--   0 runner    (1001) docker     (121)   177217 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/_static/releasing-changelog-entered.png
+-rw-r--r--   0 runner    (1001) docker     (121)   129429 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/_static/releasing-draft-button.png
+-rw-r--r--   0 runner    (1001) docker     (121)   170326 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/_static/releasing-name-release.png
+-rw-r--r--   0 runner    (1001) docker     (121)   176171 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/_static/releasing-name-tag.png
+-rw-r--r--   0 runner    (1001) docker     (121)   160943 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/_static/releasing-publish-button.png
+-rw-r--r--   0 runner    (1001) docker     (121)   139063 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/_static/releasing-pypi.png
+-rw-r--r--   0 runner    (1001) docker     (121)   115853 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/_static/releasing-release-published.png
+-rw-r--r--   0 runner    (1001) docker     (121)   217800 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/_static/releasing-releases-button.png
+-rw-r--r--   0 runner    (1001) docker     (121)   171004 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/_static/releasing-tag-button.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 18:46:41.802078 warn-scraper-1.2.9/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (121)      829 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/_templates/sources.md.tmpl
+-rw-r--r--   0 runner    (1001) docker     (121)      492 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10377 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      800 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (121)     2721 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4416 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/releasing.md
+-rw-r--r--   0 runner    (1001) docker     (121)       51 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 18:46:41.806078 warn-scraper-1.2.9/docs/scrapers/
+-rw-r--r--   0 runner    (1001) docker     (121)     1579 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/scrapers/al.md
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/scrapers/az.md
+-rw-r--r--   0 runner    (1001) docker     (121)      213 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/scrapers/ca.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/scrapers/co.md
+-rw-r--r--   0 runner    (1001) docker     (121)      454 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/scrapers/dc.md
+-rw-r--r--   0 runner    (1001) docker     (121)      744 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/scrapers/de.md
+-rw-r--r--   0 runner    (1001) docker     (121)      198 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/scrapers/ia.md
+-rw-r--r--   0 runner    (1001) docker     (121)      785 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/scrapers/in.md
+-rw-r--r--   0 runner    (1001) docker     (121)     4308 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/scrapers/job_center.md
+-rw-r--r--   0 runner    (1001) docker     (121)      997 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/scrapers/ks.md
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/scrapers/md.md
+-rw-r--r--   0 runner    (1001) docker     (121)      965 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/scrapers/me.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2032 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/scrapers/mo.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1973 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/scrapers/ny.md
+-rw-r--r--   0 runner    (1001) docker     (121)      719 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/scrapers/ok.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1496 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/scrapers/or.md
+-rw-r--r--   0 runner    (1001) docker     (121)      240 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/scrapers/sc.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3424 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/scrapers/tx.md
+-rw-r--r--   0 runner    (1001) docker     (121)      430 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/scrapers/ut.md
+-rw-r--r--   0 runner    (1001) docker     (121)      679 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/scrapers/va.md
+-rw-r--r--   0 runner    (1001) docker     (121)      963 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/scrapers/vt.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/scrapers/wi.md
+-rw-r--r--   0 runner    (1001) docker     (121)    11024 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/sources.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1363 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2022-07-08 18:46:41.814078 warn-scraper-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     5353 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 18:46:41.806078 warn-scraper-1.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 18:46:41.806078 warn-scraper-1.2.9/tests/cassettes/
+-rw-r--r--   0 runner    (1001) docker     (121)    48934 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/tests/cassettes/test_cached_detail_pages.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    34866 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/tests/cassettes/test_cached_search_results.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)   209861 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/tests/cassettes/test_delete.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)   209861 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/tests/cassettes/test_iowa.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    33645 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/tests/cassettes/test_missing_detail_page_values.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16676 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/tests/cassettes/test_no_results.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    35299 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/tests/cassettes/test_paged_results.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    48760 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/tests/cassettes/test_scrape_integration.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     2156 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 18:46:41.806078 warn-scraper-1.2.9/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/tests/fixtures/2021_page_1.html
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/tests/fixtures/2021_page_2.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2122 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)      168 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/tests/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4997 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/tests/test_job_center.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3506 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/tests/test_job_center_cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/tests/test_openpyxl.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 18:46:41.810078 warn-scraper-1.2.9/warn/
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5502 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2019 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 18:46:41.810078 warn-scraper-1.2.9/warn/platforms/
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 18:46:41.810078 warn-scraper-1.2.9/warn/platforms/job_center/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/platforms/job_center/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/platforms/job_center/cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10009 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/platforms/job_center/site.py
+-rw-r--r--   0 runner    (1001) docker     (121)      414 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/platforms/job_center/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5436 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/platforms/job_center/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1894 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 18:46:41.814078 warn-scraper-1.2.9/warn/scrapers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1847 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/ak.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2240 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/al.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1222 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/az.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7262 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/ca.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5763 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/co.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4228 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/ct.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4021 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/dc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1316 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/de.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9429 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/fl.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3484 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/ga.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2087 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/ia.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4600 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/id.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/il.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2539 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/in.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1266 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/ks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4222 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/ky.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12047 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/la.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2774 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/md.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1172 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/me.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3527 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/mi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3469 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/mo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2294 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/mt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4090 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/ne.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2231 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/nj.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3581 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/nm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3545 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/ny.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5640 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/oh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/ok.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1683 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/or.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1977 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/ri.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4736 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/sc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1904 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/sd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4480 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/tn.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4351 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/tx.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1825 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/ut.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1554 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/va.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1186 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/vt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4021 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/wa.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3531 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/scrapers/wi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5200 2022-07-08 18:46:24.000000 warn-scraper-1.2.9/warn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-08 18:46:41.814078 warn-scraper-1.2.9/warn_scraper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1841 2022-07-08 18:46:41.000000 warn-scraper-1.2.9/warn_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3234 2022-07-08 18:46:41.000000 warn-scraper-1.2.9/warn_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-08 18:46:41.000000 warn-scraper-1.2.9/warn_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-07-08 18:46:41.000000 warn-scraper-1.2.9/warn_scraper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-08 18:46:41.000000 warn-scraper-1.2.9/warn_scraper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-07-08 18:46:41.000000 warn-scraper-1.2.9/warn_scraper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-07-08 18:46:41.000000 warn-scraper-1.2.9/warn_scraper.egg-info/top_level.txt
```

### Comparing `warn-scraper-1.2.8/.github/workflows/continuous-deployment.yml` & `warn-scraper-1.2.9/.github/workflows/continuous-deployment.yml`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/.gitignore` & `warn-scraper-1.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/.pre-commit-config.yaml` & `warn-scraper-1.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/LICENSE` & `warn-scraper-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/Makefile` & `warn-scraper-1.2.9/Makefile`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/PKG-INFO` & `warn-scraper-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warn-scraper
-Version: 1.2.8
+Version: 1.2.9
 Summary: Command-line interface for downloading WARN Act notices of qualified plant closings and mass layoffs from state government websites
 Home-page: https://github.com/biglocalnews/warn-scraper
 Author: Big Local News
 License: Apache 2.0 license
 Project-URL: Documentation, https://warn-scraper.readthedocs.io
 Project-URL: Maintainer, https://github.com/biglocalnews
 Project-URL: Source, https://github.com/biglocalnews/warn-scraper
```

### Comparing `warn-scraper-1.2.8/Pipfile` & `warn-scraper-1.2.9/Pipfile`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/Pipfile.lock` & `warn-scraper-1.2.9/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/README.md` & `warn-scraper-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/Makefile` & `warn-scraper-1.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/_static/R42693.pdf` & `warn-scraper-1.2.9/docs/_static/R42693.pdf`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/_static/gao-03-1003.pdf` & `warn-scraper-1.2.9/docs/_static/gao-03-1003.pdf`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/_static/releasing-actions-finished.png` & `warn-scraper-1.2.9/docs/_static/releasing-actions-finished.png`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/_static/releasing-actions-start.png` & `warn-scraper-1.2.9/docs/_static/releasing-actions-start.png`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/_static/releasing-changelog-button.png` & `warn-scraper-1.2.9/docs/_static/releasing-changelog-button.png`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/_static/releasing-changelog-entered.png` & `warn-scraper-1.2.9/docs/_static/releasing-changelog-entered.png`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/_static/releasing-draft-button.png` & `warn-scraper-1.2.9/docs/_static/releasing-draft-button.png`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/_static/releasing-name-release.png` & `warn-scraper-1.2.9/docs/_static/releasing-name-release.png`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/_static/releasing-name-tag.png` & `warn-scraper-1.2.9/docs/_static/releasing-name-tag.png`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/_static/releasing-publish-button.png` & `warn-scraper-1.2.9/docs/_static/releasing-publish-button.png`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/_static/releasing-pypi.png` & `warn-scraper-1.2.9/docs/_static/releasing-pypi.png`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/_static/releasing-release-published.png` & `warn-scraper-1.2.9/docs/_static/releasing-release-published.png`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/_static/releasing-releases-button.png` & `warn-scraper-1.2.9/docs/_static/releasing-releases-button.png`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/_static/releasing-tag-button.png` & `warn-scraper-1.2.9/docs/_static/releasing-tag-button.png`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/_templates/sources.md.tmpl` & `warn-scraper-1.2.9/docs/_templates/sources.md.tmpl`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/contributing.rst` & `warn-scraper-1.2.9/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/index.rst` & `warn-scraper-1.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/make.bat` & `warn-scraper-1.2.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/reference.rst` & `warn-scraper-1.2.9/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/releasing.md` & `warn-scraper-1.2.9/docs/releasing.md`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/scrapers/al.md` & `warn-scraper-1.2.9/docs/scrapers/al.md`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/scrapers/az.md` & `warn-scraper-1.2.9/docs/scrapers/az.md`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/scrapers/co.md` & `warn-scraper-1.2.9/docs/scrapers/co.md`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/scrapers/de.md` & `warn-scraper-1.2.9/docs/scrapers/de.md`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/scrapers/in.md` & `warn-scraper-1.2.9/docs/scrapers/in.md`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/scrapers/job_center.md` & `warn-scraper-1.2.9/docs/scrapers/job_center.md`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/scrapers/ks.md` & `warn-scraper-1.2.9/docs/scrapers/ks.md`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/scrapers/me.md` & `warn-scraper-1.2.9/docs/scrapers/me.md`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/scrapers/mo.md` & `warn-scraper-1.2.9/docs/scrapers/mo.md`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/scrapers/ny.md` & `warn-scraper-1.2.9/docs/scrapers/ny.md`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/scrapers/ok.md` & `warn-scraper-1.2.9/docs/scrapers/ok.md`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/scrapers/or.md` & `warn-scraper-1.2.9/docs/scrapers/or.md`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/scrapers/tx.md` & `warn-scraper-1.2.9/docs/scrapers/tx.md`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/scrapers/va.md` & `warn-scraper-1.2.9/docs/scrapers/va.md`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/scrapers/vt.md` & `warn-scraper-1.2.9/docs/scrapers/vt.md`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/scrapers/wi.md` & `warn-scraper-1.2.9/docs/scrapers/wi.md`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/docs/sources.md` & `warn-scraper-1.2.9/docs/sources.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Sources
 
-There are currently scrapers for 38 of America's 56 states and territories.
+There are currently scrapers for 39 of America's 56 states and territories.
 
 | State | Source | Docs | Authors | Tags |
 | :---- | :----: | :--: | :------ | :--- |
 |[Alabama](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/al.py)|[🔗](https://www.madeinalabama.com/warn-list/)|[📃](scrapers/al.md)|[Dilcia19](https://github.com/Dilcia19), [zstumgoren](https://github.com/zstumgoren)|html|
 |[Alaska](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/ak.py)|[🔗](https://jobs.alaska.gov/RR/WARN_notices.htm)||[Dilcia19](https://github.com/Dilcia19), [zstumgoren](https://github.com/zstumgoren)|html|
 |[Arizona](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/az.py)|[🔗](https://www.azjobconnection.gov/search/warn_lookups/new)|[📃](scrapers/az.md)|[Dilcia19](https://github.com/Dilcia19), [zstumgoren](https://github.com/zstumgoren)|jobcenter|
 |[California](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/ca.py)|[🔗](https://edd.ca.gov/en/Jobs_and_Training/Layoff_Services_WARN)|[📃](scrapers/ca.md)|[Dilcia19](https://github.com/Dilcia19), [ydoc5212](https://github.com/ydoc5212), [zstumgoren](https://github.com/zstumgoren)|excel, html, pdf|
+|[Colorado](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/co.py)|[🔗](https://cdle.colorado.gov/employers/layoff-separations/layoff-warn-list)|[📃](scrapers/co.md)|[anikasikka](https://github.com/anikasikka)|html|
 |[Connecticut](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/ct.py)|[🔗](https://www.ctdol.state.ct.us/progsupt/bussrvce/warnreports/warnreports.htm)||[Dilcia19](https://github.com/Dilcia19), [stucka](https://github.com/stucka), [zstumgoren](https://github.com/zstumgoren)|html|
 |[Delaware](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/de.py)|[🔗](https://joblink.delaware.gov/search/warn_lookups/new)|[📃](scrapers/de.md)|[Dilcia19](https://github.com/Dilcia19), [zstumgoren](https://github.com/zstumgoren)|jobcenter|
 |[Florida](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/fl.py)|[🔗](http://floridajobs.org/office-directory/division-of-workforce-services/workforce-programs/reemployment-and-emergency-assistance-coordination-team-react/warn-notices)||[Dilcia19](https://github.com/Dilcia19), [shallotly](https://github.com/shallotly), [zstumgoren](https://github.com/zstumgoren)|html, pdf|
 |[Georgia](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/ga.py)|[🔗](https://www.dol.state.ga.us/public/es/warn/searchwarns/list)||[chriszs](https://github.com/chriszs)|html|
 |[Idaho](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/id.py)|[🔗](https://www.labor.idaho.gov/dnn/Businesses/Layoff-Assistance#2)||[chriszs](https://github.com/chriszs)|pdf|
 |[Illinois](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/il.py)|[🔗](https://www2.illinois.gov/dceo/WorkforceDevelopment/warn/Pages/default.aspx)||[chriszs](https://github.com/chriszs)|excel, html|
 |[Indiana](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/in.py)|[🔗](https://www.in.gov/dwd/2567.htm)|[📃](scrapers/in.md)|[Dilcia19](https://github.com/Dilcia19), [zstumgoren](https://github.com/zstumgoren)|html|
@@ -23,15 +24,15 @@
 |[Maryland](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/md.py)|[🔗](http://www.dllr.state.md.us/employment/warn.shtml)|[📃](scrapers/md.md)|[Dilcia19](https://github.com/Dilcia19), [shallotly](https://github.com/shallotly), [zstumgoren](https://github.com/zstumgoren)|html|
 |[Michigan](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/mi.py)|[🔗](https://milmi.org/warn/)||[anikasikka](https://github.com/anikasikka)|html, pdf|
 |[Missouri](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/mo.py)|[🔗](https://jobs.mo.gov/content/2022-warn-notices)|[📃](scrapers/mo.md)|[Dilcia19](https://github.com/Dilcia19), [shallotly](https://github.com/shallotly), [zstumgoren](https://github.com/zstumgoren)|html|
 |[Montana](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/mt.py)|[🔗](https://wsd.dli.mt.gov/wioa/related-links/warn-notice-page)||[ydoc5212](https://github.com/ydoc5212), [zstumgoren](https://github.com/zstumgoren)|excel, html|
 |[Nebraska](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/ne.py)|[🔗](https://dol.nebraska.gov/ReemploymentServices/LayoffServices/LayoffsAndDownsizingWARN)||[Dilcia19](https://github.com/Dilcia19), [zstumgoren](https://github.com/zstumgoren)|html|
 |[New Jersey](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/nj.py)|[🔗](https://www.nj.gov/labor/employer-services/warn/)||[Dilcia19](https://github.com/Dilcia19), [palewire](https://github.com/palewire), [zstumgoren](https://github.com/zstumgoren)|html|
 |[New Mexico](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/nm.py)|[🔗](https://www.dws.state.nm.us/Rapid-Response)||[chriszs](https://github.com/chriszs)|pdf|
-|[New York](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/ny.py)|[🔗](https://dol.ny.gov/warn-notices)|[📃](scrapers/ny.md)|[Dilcia19](https://github.com/Dilcia19), [ydoc5212](https://github.com/ydoc5212), [zstumgoren](https://github.com/zstumgoren)|excel, historical|
+|[New York](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/ny.py)|[🔗](https://dol.ny.gov/warn-notices)|[📃](scrapers/ny.md)|[Dilcia19](https://github.com/Dilcia19), [palewire](https://github.com/palewire), [ydoc5212](https://github.com/ydoc5212), [zstumgoren](https://github.com/zstumgoren)|excel, historical|
 |[Ohio](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/oh.py)|[🔗](https://jfs.ohio.gov/warn/index.stm)||[Dilcia19](https://github.com/Dilcia19), [chriszs](https://github.com/chriszs), [zstumgoren](https://github.com/zstumgoren)|html, pdf|
 |[Oklahoma](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/ok.py)|[🔗](https://okjobmatch.com/search/warn_lookups/new)|[📃](scrapers/ok.md)|[Dilcia19](https://github.com/Dilcia19), [zstumgoren](https://github.com/zstumgoren)|jobcenter|
 |[Oregon](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/or.py)|[🔗](https://ccwd.hecc.oregon.gov/Layoff/WARN)|[📃](scrapers/or.md)|[Dilcia19](https://github.com/Dilcia19), [ydoc5212](https://github.com/ydoc5212), [zstumgoren](https://github.com/zstumgoren)|excel, historical|
 |[Rhode Island](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/ri.py)|[🔗](https://dlt.ri.gov/employers/worker-adjustment-and-retraining-notification-warn)||[Dilcia19](https://github.com/Dilcia19), [chriszs](https://github.com/chriszs), [ydoc5212](https://github.com/ydoc5212), [zstumgoren](https://github.com/zstumgoren)|excel|
 |[South Carolina](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/sc.py)|[🔗](https://scworks.org/employer/employer-programs/at-risk-of-closing/layoff-notification-reports)|[📃](scrapers/sc.md)|[palewire](https://github.com/palewire)|html, pdf|
 |[South Dakota](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/sd.py)|[🔗](https://dlr.sd.gov/workforce_services/businesses/warn_notices.aspx)||[Dilcia19](https://github.com/Dilcia19), [ydoc5212](https://github.com/ydoc5212), [zstumgoren](https://github.com/zstumgoren)|html|
 |[Tennessee](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/tn.py)|[🔗](https://www.tn.gov/workforce/general-resources/major-publications0/major-publications-redirect/reports.html)||[anikasikka](https://github.com/anikasikka)|html, pdf|
@@ -42,18 +43,17 @@
 |[Washington](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/wa.py)|[🔗](https://esd.wa.gov/about-employees/WARN)||[Dilcia19](https://github.com/Dilcia19), [zstumgoren](https://github.com/zstumgoren)|html|
 |[Wisconsin](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/wi.py)|[🔗](https://dwd.wisconsin.gov/dislocatedworker/warn/)|[📃](scrapers/wi.md)|[Dilcia19](https://github.com/Dilcia19), [ydoc5212](https://github.com/ydoc5212), [zstumgoren](https://github.com/zstumgoren)|html|
 |[District of Columbia](https://github.com/biglocalnews/warn-scraper/blob/main/warn/scrapers/dc.py)|[🔗](https://does.dc.gov/page/industry-closings-and-layoffs-warn-notifications-2022)|[📃](scrapers/dc.md)|[Dilcia19](https://github.com/Dilcia19), [shallotly](https://github.com/shallotly), [zstumgoren](https://github.com/zstumgoren)|html|
 
 
 ## To do
 
-These 18 areas need a scraper:
+These 17 areas need a scraper:
 
 - Arkansas
-- Colorado
 - Hawaii
 - Massachusetts
 - Minnesota
 - Mississippi
 - Nevada
 - New Hampshire
 - North Carolina
```

### Comparing `warn-scraper-1.2.8/docs/usage.md` & `warn-scraper-1.2.9/docs/usage.md`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/setup.py` & `warn-scraper-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/tests/cassettes/test_cached_detail_pages.yaml` & `warn-scraper-1.2.9/tests/cassettes/test_cached_detail_pages.yaml`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/tests/cassettes/test_cached_search_results.yaml` & `warn-scraper-1.2.9/tests/cassettes/test_cached_search_results.yaml`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/tests/cassettes/test_delete.yaml` & `warn-scraper-1.2.9/tests/cassettes/test_delete.yaml`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/tests/cassettes/test_iowa.yaml` & `warn-scraper-1.2.9/tests/cassettes/test_iowa.yaml`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/tests/cassettes/test_missing_detail_page_values.yaml` & `warn-scraper-1.2.9/tests/cassettes/test_missing_detail_page_values.yaml`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/tests/cassettes/test_no_results.yaml` & `warn-scraper-1.2.9/tests/cassettes/test_no_results.yaml`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/tests/cassettes/test_paged_results.yaml` & `warn-scraper-1.2.9/tests/cassettes/test_paged_results.yaml`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/tests/cassettes/test_scrape_integration.yaml` & `warn-scraper-1.2.9/tests/cassettes/test_scrape_integration.yaml`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/tests/conftest.py` & `warn-scraper-1.2.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/tests/test_cache.py` & `warn-scraper-1.2.9/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/tests/test_job_center.py` & `warn-scraper-1.2.9/tests/test_job_center.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/tests/test_job_center_cache.py` & `warn-scraper-1.2.9/tests/test_job_center_cache.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/cache.py` & `warn-scraper-1.2.9/warn/cache.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/cli.py` & `warn-scraper-1.2.9/warn/cli.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/platforms/job_center/cache.py` & `warn-scraper-1.2.9/warn/platforms/job_center/cache.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/platforms/job_center/site.py` & `warn-scraper-1.2.9/warn/platforms/job_center/site.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/platforms/job_center/utils.py` & `warn-scraper-1.2.9/warn/platforms/job_center/utils.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/runner.py` & `warn-scraper-1.2.9/warn/runner.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/ak.py` & `warn-scraper-1.2.9/warn/scrapers/ak.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/al.py` & `warn-scraper-1.2.9/warn/scrapers/al.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/az.py` & `warn-scraper-1.2.9/warn/scrapers/az.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/ca.py` & `warn-scraper-1.2.9/warn/scrapers/ca.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/ct.py` & `warn-scraper-1.2.9/warn/scrapers/ct.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/dc.py` & `warn-scraper-1.2.9/warn/scrapers/dc.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/de.py` & `warn-scraper-1.2.9/warn/scrapers/de.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/fl.py` & `warn-scraper-1.2.9/warn/scrapers/fl.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/ga.py` & `warn-scraper-1.2.9/warn/scrapers/ga.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/ia.py` & `warn-scraper-1.2.9/warn/scrapers/ia.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/id.py` & `warn-scraper-1.2.9/warn/scrapers/id.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/il.py` & `warn-scraper-1.2.9/warn/scrapers/il.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/in.py` & `warn-scraper-1.2.9/warn/scrapers/in.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/ks.py` & `warn-scraper-1.2.9/warn/scrapers/ks.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/ky.py` & `warn-scraper-1.2.9/warn/scrapers/ky.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/la.py` & `warn-scraper-1.2.9/warn/scrapers/la.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/md.py` & `warn-scraper-1.2.9/warn/scrapers/md.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/me.py` & `warn-scraper-1.2.9/warn/scrapers/me.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/mi.py` & `warn-scraper-1.2.9/warn/scrapers/mi.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/mo.py` & `warn-scraper-1.2.9/warn/scrapers/mo.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/mt.py` & `warn-scraper-1.2.9/warn/scrapers/mt.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/ne.py` & `warn-scraper-1.2.9/warn/scrapers/ne.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/nj.py` & `warn-scraper-1.2.9/warn/scrapers/nj.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/nm.py` & `warn-scraper-1.2.9/warn/scrapers/nm.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/ny.py` & `warn-scraper-1.2.9/warn/scrapers/ny.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/oh.py` & `warn-scraper-1.2.9/warn/scrapers/oh.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/ok.py` & `warn-scraper-1.2.9/warn/scrapers/ok.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/or.py` & `warn-scraper-1.2.9/warn/scrapers/or.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/ri.py` & `warn-scraper-1.2.9/warn/scrapers/ri.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/sc.py` & `warn-scraper-1.2.9/warn/scrapers/sc.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/sd.py` & `warn-scraper-1.2.9/warn/scrapers/sd.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/tn.py` & `warn-scraper-1.2.9/warn/scrapers/tn.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/tx.py` & `warn-scraper-1.2.9/warn/scrapers/tx.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/ut.py` & `warn-scraper-1.2.9/warn/scrapers/ut.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/va.py` & `warn-scraper-1.2.9/warn/scrapers/va.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/vt.py` & `warn-scraper-1.2.9/warn/scrapers/vt.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/wa.py` & `warn-scraper-1.2.9/warn/scrapers/wa.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/scrapers/wi.py` & `warn-scraper-1.2.9/warn/scrapers/wi.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn/utils.py` & `warn-scraper-1.2.9/warn/utils.py`

 * *Files identical despite different names*

### Comparing `warn-scraper-1.2.8/warn_scraper.egg-info/PKG-INFO` & `warn-scraper-1.2.9/warn_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warn-scraper
-Version: 1.2.8
+Version: 1.2.9
 Summary: Command-line interface for downloading WARN Act notices of qualified plant closings and mass layoffs from state government websites
 Home-page: https://github.com/biglocalnews/warn-scraper
 Author: Big Local News
 License: Apache 2.0 license
 Project-URL: Documentation, https://warn-scraper.readthedocs.io
 Project-URL: Maintainer, https://github.com/biglocalnews
 Project-URL: Source, https://github.com/biglocalnews/warn-scraper
```

### Comparing `warn-scraper-1.2.8/warn_scraper.egg-info/SOURCES.txt` & `warn-scraper-1.2.9/warn_scraper.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 warn/platforms/job_center/urls.py
 warn/platforms/job_center/utils.py
 warn/scrapers/__init__.py
 warn/scrapers/ak.py
 warn/scrapers/al.py
 warn/scrapers/az.py
 warn/scrapers/ca.py
+warn/scrapers/co.py
 warn/scrapers/ct.py
 warn/scrapers/dc.py
 warn/scrapers/de.py
 warn/scrapers/fl.py
 warn/scrapers/ga.py
 warn/scrapers/ia.py
 warn/scrapers/id.py
```

