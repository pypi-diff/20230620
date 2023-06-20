# Comparing `tmp/pygaps-4.4.2.tar.gz` & `tmp/pygaps-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygaps-4.4.2.tar", last modified: Tue Oct 11 22:47:15 2022, max compression
+gzip compressed data, was "pygaps-4.5.0.tar", last modified: Tue Jun 20 00:28:02 2023, max compression
```

## Comparing `pygaps-4.4.2.tar` & `pygaps-4.5.0.tar`

### file list

```diff
@@ -1,353 +1,355 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.937990 pygaps-4.4.2/
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-10-11 22:47:02.000000 pygaps-4.4.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.897987 pygaps-4.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.897987 pygaps-4.4.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-10-11 22:47:02.000000 pygaps-4.4.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      791 2022-10-11 22:47:02.000000 pygaps-4.4.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-10-11 22:47:02.000000 pygaps-4.4.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.897987 pygaps-4.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     3627 2022-10-11 22:47:02.000000 pygaps-4.4.2/.github/workflows/CI.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-10-11 22:47:02.000000 pygaps-4.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-10-11 22:47:02.000000 pygaps-4.4.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-10-11 22:47:02.000000 pygaps-4.4.2/.release.info
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-10-11 22:47:02.000000 pygaps-4.4.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)    18040 2022-10-11 22:47:02.000000 pygaps-4.4.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-10-11 22:47:02.000000 pygaps-4.4.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (121)     2709 2022-10-11 22:47:02.000000 pygaps-4.4.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-10-11 22:47:02.000000 pygaps-4.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     9115 2022-10-11 22:47:15.937990 pygaps-4.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7785 2022-10-11 22:47:02.000000 pygaps-4.4.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.897987 pygaps-4.4.2/ci/
--rw-r--r--   0 runner    (1001) docker     (121)     3181 2022-10-11 22:47:02.000000 pygaps-4.4.2/ci/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.897987 pygaps-4.4.2/ci/ci_old/
--rw-r--r--   0 runner    (1001) docker     (121)     3884 2022-10-11 22:47:02.000000 pygaps-4.4.2/ci/ci_old/appveyor-download.py
--rw-r--r--   0 runner    (1001) docker     (121)     3600 2022-10-11 22:47:02.000000 pygaps-4.4.2/ci/ci_old/appveyor-with-compiler.cmd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.897987 pygaps-4.4.2/ci/ci_old/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     5173 2022-10-11 22:47:02.000000 pygaps-4.4.2/ci/ci_old/templates/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2067 2022-10-11 22:47:02.000000 pygaps-4.4.2/ci/ci_old/templates/appveyor.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2995 2022-10-11 22:47:02.000000 pygaps-4.4.2/ci/ci_old/windows-conda-bootstrap.ps1
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.897987 pygaps-4.4.2/ci/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     2016 2022-10-11 22:47:02.000000 pygaps-4.4.2/ci/templates/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.897987 pygaps-4.4.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.889986 pygaps-4.4.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.897987 pygaps-4.4.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (121)      977 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.897987 pygaps-4.4.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)      326 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6912 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/docutils.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.905987 pygaps-4.4.2/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    47803 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/alphas.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   188676 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/area_calcs.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/characterisation.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.905987 pygaps-4.4.2/docs/examples/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.909988 pygaps-4.4.2/docs/examples/data/calorimetry/
--rw-r--r--   0 runner    (1001) docker     (121)     4423 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/calorimetry/HKUST-1(Cu) KRICT.json
--rw-r--r--   0 runner    (1001) docker     (121)     5354 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/calorimetry/Takeda 5A Test CO2.json
--rw-r--r--   0 runner    (1001) docker     (121)  4546254 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/calorimetry/data.csv
--rw-r--r--   0 runner    (1001) docker     (121)     1346 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/calorimetry/header.csv
--rw-r--r--   0 runner    (1001) docker     (121)    13668 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/carbon_x1_n2.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.909988 pygaps-4.4.2/docs/examples/data/characterisation/
--rw-r--r--   0 runner    (1001) docker     (121)     7214 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/characterisation/MCM-41 N2 77.355.json
--rw-r--r--   0 runner    (1001) docker     (121)    10942 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/characterisation/NaY N2 77.355.json
--rw-r--r--   0 runner    (1001) docker     (121)     4810 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/characterisation/SiO2 N2 77.355.json
--rw-r--r--   0 runner    (1001) docker     (121)    13631 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/characterisation/Takeda 5A N2 77.355.json
--rw-r--r--   0 runner    (1001) docker     (121)    11636 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/characterisation/UiO-66(Zr) N2 77.355.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.909988 pygaps-4.4.2/docs/examples/data/iast/
--rw-r--r--   0 runner    (1001) docker     (121)     2159 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/iast/MOF-5(Zn) - IAST - C2H6.json
--rw-r--r--   0 runner    (1001) docker     (121)     2786 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/iast/MOF-5(Zn) - IAST - CH4.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.909988 pygaps-4.4.2/docs/examples/data/isosteric/
--rw-r--r--   0 runner    (1001) docker     (121)     5001 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/isosteric/BAX 1500 - Isosteric Heat - 298.json
--rw-r--r--   0 runner    (1001) docker     (121)     4338 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/isosteric/BAX 1500 - Isosteric Heat - 323.json
--rw-r--r--   0 runner    (1001) docker     (121)     3999 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/isosteric/BAX 1500 - Isosteric Heat - 348.json
--rw-r--r--   0 runner    (1001) docker     (121)     4426 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/isotherm.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.893987 pygaps-4.4.2/docs/examples/data/parsing/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.913988 pygaps-4.4.2/docs/examples/data/parsing/aif/
--rw-r--r--   0 runner    (1001) docker     (121)     3505 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/aif/ar_test_77k.aif
--rw-r--r--   0 runner    (1001) docker     (121)     2187 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/aif/dmof_C2H6_298k.aif
--rw-r--r--   0 runner    (1001) docker     (121)     1452 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/aif/dut-8_etoh_298k.aif
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.893987 pygaps-4.4.2/docs/examples/data/parsing/commercial/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.913988 pygaps-4.4.2/docs/examples/data/parsing/commercial/3p/
--rw-r--r--   0 runner    (1001) docker     (121)  1637702 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/commercial/3p/MOF_N2_77K.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/commercial/3p/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.913988 pygaps-4.4.2/docs/examples/data/parsing/commercial/bel/
--rw-r--r--   0 runner    (1001) docker     (121)     4451 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/commercial/bel/DUT-13-CH4-190K.DAT
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/commercial/bel/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.913988 pygaps-4.4.2/docs/examples/data/parsing/commercial/mic/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/commercial/mic/README.txt
--rw-r--r--   0 runner    (1001) docker     (121)    59904 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/commercial/mic/Sample_C.xls
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.913988 pygaps-4.4.2/docs/examples/data/parsing/commercial/qnt/
--rw-r--r--   0 runner    (1001) docker     (121)    10413 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/commercial/qnt/DUT-6_N2_77K (Raw Analysis Data).txt
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/commercial/qnt/README
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.913988 pygaps-4.4.2/docs/examples/data/parsing/commercial/smsdvs/
--rw-r--r--   0 runner    (1001) docker     (121)    26372 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/commercial/smsdvs/13X water 30c.xlsx
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/commercial/smsdvs/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.913988 pygaps-4.4.2/docs/examples/data/parsing/csv/
--rw-r--r--   0 runner    (1001) docker     (121)     1480 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/csv/HKUST-1(Cu) CO2 303.0.csv
--rw-r--r--   0 runner    (1001) docker     (121)     1765 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/csv/MCM-41 N2 77.0.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.913988 pygaps-4.4.2/docs/examples/data/parsing/excel/
--rw-r--r--   0 runner    (1001) docker     (121)     9728 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/excel/HKUST-1(Cu) CO2 303.0.xls
--rw-r--r--   0 runner    (1001) docker     (121)     9728 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/excel/MCM-41 N2 77.0.xls
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.917988 pygaps-4.4.2/docs/examples/data/parsing/json/
--rw-r--r--   0 runner    (1001) docker     (121)    21354 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/json/AC Ar 77.json
--rw-r--r--   0 runner    (1001) docker     (121)     5458 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/json/AC BAX1500 butane 298.json
--rw-r--r--   0 runner    (1001) docker     (121)     8807 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/json/DUT-8 EtOH 298.json
--rw-r--r--   0 runner    (1001) docker     (121)     4939 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/json/HKUST-1(Cu) CO2 303.json
--rw-r--r--   0 runner    (1001) docker     (121)     7754 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/json/MCM-41 N2 77.json
--rw-r--r--   0 runner    (1001) docker     (121)    17168 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/json/SURF N2 77.json
--rw-r--r--   0 runner    (1001) docker     (121)    12498 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/json/UiO-66(Zr) N2 77.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.917988 pygaps-4.4.2/docs/examples/data/parsing/nist/
--rw-r--r--   0 runner    (1001) docker     (121)    12189 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/data/parsing/nist/nist_iso.json
--rw-r--r--   0 runner    (1001) docker     (121)    37594 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/database.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    82587 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/dr_da_plots.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   129960 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/iast.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     4499 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/import.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    93919 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/initial_enthalpy.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   124568 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/initial_henryc.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    83406 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/inspection.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    70175 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/isosteric_enthalpy.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   226257 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/modelling.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   107509 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/novel.png
--rw-r--r--   0 runner    (1001) docker     (121)    35882 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/parsing.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   370212 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/plotting.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   399127 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/psd.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   385374 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    54786 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/test.png
--rw-r--r--   0 runner    (1001) docker     (121)    69242 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/examples/tplot.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   324341 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)    12304 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/favicon.png
--rw-r--r--   0 runner    (1001) docker     (121)     5472 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/favicon.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.917988 pygaps-4.4.2/docs/figures/
--rw-r--r--   0 runner    (1001) docker     (121)    56681 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/figures/SMS-Logo.jpg
--rw-r--r--   0 runner    (1001) docker     (121)    81047 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/figures/db_schema.png
--rw-r--r--   0 runner    (1001) docker     (121)    33195 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/figures/svp_graph.png
--rw-r--r--   0 runner    (1001) docker     (121)    52666 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/figures/vle_graph.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.917988 pygaps-4.4.2/docs/files/
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/files/isotherm.aif
--rw-r--r--   0 runner    (1001) docker     (121)     1684 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/files/isotherm.csv
--rw-r--r--   0 runner    (1001) docker     (121)     4458 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/files/isotherm.json
--rw-r--r--   0 runner    (1001) docker     (121)     9728 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/files/isotherm.xls
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/indices.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1881 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)   104930 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)     6313 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.917988 pygaps-4.4.2/docs/manual/
--rw-r--r--   0 runner    (1001) docker     (121)     6727 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/manual/adsorbate.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/manual/characterisation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/manual/eqstate.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3518 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/manual/iast.rst
--rw-r--r--   0 runner    (1001) docker     (121)      932 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/manual/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    23793 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/manual/isotherm.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4639 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/manual/material.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8656 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/manual/modelling.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8483 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/manual/parsing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/manual/parsing_modes.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/manual/plotting.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2469 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/manual/sqlitedb.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7519 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/manual/units.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.921989 pygaps-4.4.2/docs/reference/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.921989 pygaps-4.4.2/docs/reference/characterisation/
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/reference/characterisation/alphas_plot.rst
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/reference/characterisation/area_bet.rst
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/reference/characterisation/area_lang.rst
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/reference/characterisation/dubinin.rst
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/reference/characterisation/initial_enth.rst
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/reference/characterisation/initial_hk.rst
--rw-r--r--   0 runner    (1001) docker     (121)      136 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/reference/characterisation/isosteric_enth.rst
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/reference/characterisation/psd_kernel.rst
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/reference/characterisation/psd_meso.rst
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/reference/characterisation/psd_micro.rst
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/reference/characterisation/t_plot.rst
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/reference/characterisation/thickness_models.rst
--rw-r--r--   0 runner    (1001) docker     (121)      466 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/reference/characterisation.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.921989 pygaps-4.4.2/docs/reference/core/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/reference/core/adsorbate.rst
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/reference/core/isotherms.rst
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/reference/core/material.rst
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/reference/core.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1691 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/reference/fitting.rst
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/reference/iast.rst
--rw-r--r--   0 runner    (1001) docker     (121)      547 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      549 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/reference/parsing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      573 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/reference/plotting.rst
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/reference/units.rst
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/reference/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-10-11 22:47:02.000000 pygaps-4.4.2/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4670 2022-10-11 22:47:02.000000 pygaps-4.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2310 2022-10-11 22:47:15.941990 pygaps-4.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.893987 pygaps-4.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.921989 pygaps-4.4.2/src/pygaps/
--rw-r--r--   0 runner    (1001) docker     (121)     2181 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-11 22:47:15.000000 pygaps-4.4.2/src/pygaps/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.925989 pygaps-4.4.2/src/pygaps/characterisation/
--rw-r--r--   0 runner    (1001) docker     (121)      798 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/characterisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14609 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/characterisation/alphas_plots.py
--rw-r--r--   0 runner    (1001) docker     (121)    12764 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/characterisation/area_bet.py
--rw-r--r--   0 runner    (1001) docker     (121)    10555 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/characterisation/area_lang.py
--rw-r--r--   0 runner    (1001) docker     (121)    13065 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/characterisation/dr_da_plots.py
--rw-r--r--   0 runner    (1001) docker     (121)    14871 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/characterisation/initial_enth.py
--rw-r--r--   0 runner    (1001) docker     (121)     4763 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/characterisation/initial_henry.py
--rw-r--r--   0 runner    (1001) docker     (121)     7942 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/characterisation/isosteric_enth.py
--rw-r--r--   0 runner    (1001) docker     (121)     2880 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/characterisation/models_hk.py
--rw-r--r--   0 runner    (1001) docker     (121)     7732 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/characterisation/models_kelvin.py
--rw-r--r--   0 runner    (1001) docker     (121)     5688 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/characterisation/models_thickness.py
--rw-r--r--   0 runner    (1001) docker     (121)    13569 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/characterisation/psd_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)    32546 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/characterisation/psd_meso.py
--rw-r--r--   0 runner    (1001) docker     (121)    46537 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/characterisation/psd_micro.py
--rw-r--r--   0 runner    (1001) docker     (121)    12294 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/characterisation/t_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.925989 pygaps-4.4.2/src/pygaps/cli/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4934 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.925989 pygaps-4.4.2/src/pygaps/core/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20249 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/core/adsorbate.py
--rw-r--r--   0 runner    (1001) docker     (121)    16422 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/core/baseisotherm.py
--rw-r--r--   0 runner    (1001) docker     (121)     4982 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/core/material.py
--rw-r--r--   0 runner    (1001) docker     (121)    39421 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/core/modelisotherm.py
--rw-r--r--   0 runner    (1001) docker     (121)    49496 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/core/pointisotherm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.925989 pygaps-4.4.2/src/pygaps/data/
--rw-r--r--   0 runner    (1001) docker     (121)     2019 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3918 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/data/adsorbate_props.json
--rw-r--r--   0 runner    (1001) docker     (121)    85533 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/data/adsorbates.json
--rw-r--r--   0 runner    (1001) docker     (121)   212992 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/data/default.db
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.925989 pygaps-4.4.2/src/pygaps/data/kernels/
--rw-r--r--   0 runner    (1001) docker     (121)   164433 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/data/kernels/DFT-N2-77K-carbon-slit.csv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/data/kernels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.925989 pygaps-4.4.2/src/pygaps/data/stdiso/
--rw-r--r--   0 runner    (1001) docker     (121)     2628 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/data/stdiso/Cabot BP280 carbon black.csv
--rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/data/stdiso/LiChrospher Si-1000 silica.csv
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/data/stdiso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.929989 pygaps-4.4.2/src/pygaps/graphing/
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/graphing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18942 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/graphing/calc_graphs.py
--rw-r--r--   0 runner    (1001) docker     (121)     5070 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/graphing/iast_graphs.py
--rw-r--r--   0 runner    (1001) docker     (121)    19063 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/graphing/isotherm_graphs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2896 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/graphing/labels.py
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/graphing/model_graphs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/graphing/mpl_styles.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.929989 pygaps-4.4.2/src/pygaps/iast/
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/iast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24673 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/iast/pgiast.py
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.929989 pygaps-4.4.2/src/pygaps/modelling/
--rw-r--r--   0 runner    (1001) docker     (121)     5290 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/modelling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9589 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/modelling/base_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     6367 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/modelling/bet.py
--rw-r--r--   0 runner    (1001) docker     (121)     4720 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/modelling/da.py
--rw-r--r--   0 runner    (1001) docker     (121)     4512 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/modelling/dr.py
--rw-r--r--   0 runner    (1001) docker     (121)     4623 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/modelling/dslangmuir.py
--rw-r--r--   0 runner    (1001) docker     (121)     5720 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/modelling/fhvst.py
--rw-r--r--   0 runner    (1001) docker     (121)     3964 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/modelling/freundlich.py
--rw-r--r--   0 runner    (1001) docker     (121)     3739 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/modelling/gab.py
--rw-r--r--   0 runner    (1001) docker     (121)     3607 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/modelling/henry.py
--rw-r--r--   0 runner    (1001) docker     (121)     4988 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/modelling/jensenseaton.py
--rw-r--r--   0 runner    (1001) docker     (121)     5292 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/modelling/langmuir.py
--rw-r--r--   0 runner    (1001) docker     (121)     4318 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/modelling/quadratic.py
--rw-r--r--   0 runner    (1001) docker     (121)     4511 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/modelling/temkinapprox.py
--rw-r--r--   0 runner    (1001) docker     (121)     3429 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/modelling/toth.py
--rw-r--r--   0 runner    (1001) docker     (121)     5044 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/modelling/tslangmuir.py
--rw-r--r--   0 runner    (1001) docker     (121)     8006 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/modelling/virial.py
--rw-r--r--   0 runner    (1001) docker     (121)     5941 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/modelling/wvst.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.929989 pygaps-4.4.2/src/pygaps/parsing/
--rw-r--r--   0 runner    (1001) docker     (121)     2347 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12543 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/parsing/aif.py
--rw-r--r--   0 runner    (1001) docker     (121)     6895 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/parsing/csv.py
--rw-r--r--   0 runner    (1001) docker     (121)    10222 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/parsing/excel.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/parsing/isodb.py
--rw-r--r--   0 runner    (1001) docker     (121)     8235 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/parsing/json.py
--rw-r--r--   0 runner    (1001) docker     (121)    36732 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/parsing/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.933989 pygaps-4.4.2/src/pygaps/units/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12153 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/units/converter_mode.py
--rw-r--r--   0 runner    (1001) docker     (121)     1869 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/units/converter_unit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.933989 pygaps-4.4.2/src/pygaps/utilities/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/utilities/coolprop_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      842 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/utilities/hashgen.py
--rw-r--r--   0 runner    (1001) docker     (121)     2113 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/utilities/isotherm_interpolator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4678 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/utilities/math_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)      753 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/utilities/pygaps_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     2634 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/utilities/python_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/utilities/sqlite_db_creator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4334 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/utilities/sqlite_db_pragmas.py
--rw-r--r--   0 runner    (1001) docker     (121)     4718 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/utilities/sqlite_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     3754 2022-10-11 22:47:02.000000 pygaps-4.4.2/src/pygaps/utilities/string_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.921989 pygaps-4.4.2/src/pygaps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9115 2022-10-11 22:47:15.000000 pygaps-4.4.2/src/pygaps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10029 2022-10-11 22:47:15.000000 pygaps-4.4.2/src/pygaps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-11 22:47:15.000000 pygaps-4.4.2/src/pygaps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-10-11 22:47:15.000000 pygaps-4.4.2/src/pygaps.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      430 2022-10-11 22:47:15.000000 pygaps-4.4.2/src/pygaps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-11 22:47:15.000000 pygaps-4.4.2/src/pygaps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-11 22:47:15.000000 pygaps-4.4.2/src/pygaps.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.933989 pygaps-4.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.933989 pygaps-4.4.2/tests/characterisation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/characterisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3978 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/characterisation/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4118 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/characterisation/test_alphas_plots.py
--rw-r--r--   0 runner    (1001) docker     (121)     3768 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/characterisation/test_area_bet.py
--rw-r--r--   0 runner    (1001) docker     (121)     3307 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/characterisation/test_area_langmuir.py
--rw-r--r--   0 runner    (1001) docker     (121)     3330 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/characterisation/test_dr_da_plots.py
--rw-r--r--   0 runner    (1001) docker     (121)     3338 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/characterisation/test_initial_enthalpy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3396 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/characterisation/test_initial_henry.py
--rw-r--r--   0 runner    (1001) docker     (121)     2759 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/characterisation/test_isosteric_enthalpy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1365 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/characterisation/test_models_hk.py
--rw-r--r--   0 runner    (1001) docker     (121)     3738 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/characterisation/test_models_kelvin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1971 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/characterisation/test_models_thickness.py
--rw-r--r--   0 runner    (1001) docker     (121)     2683 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/characterisation/test_psd_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     3123 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/characterisation/test_psd_meso.py
--rw-r--r--   0 runner    (1001) docker     (121)     5623 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/characterisation/test_psd_micro.py
--rw-r--r--   0 runner    (1001) docker     (121)     2985 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/characterisation/test_t_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.933989 pygaps-4.4.2/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3377 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/cli/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     4804 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.937990 pygaps-4.4.2/tests/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3785 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/core/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     5492 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/core/test_adsorbate.py
--rw-r--r--   0 runner    (1001) docker     (121)     5385 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/core/test_baseisotherm.py
--rw-r--r--   0 runner    (1001) docker     (121)     2498 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/core/test_material.py
--rw-r--r--   0 runner    (1001) docker     (121)     9407 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/core/test_modelisotherm.py
--rw-r--r--   0 runner    (1001) docker     (121)    20169 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/core/test_pointisotherm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.937990 pygaps-4.4.2/tests/graphing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/graphing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/graphing/test_calc_graphs.py
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/graphing/test_iast_graphs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/graphing/test_iso_graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.937990 pygaps-4.4.2/tests/modelling/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/modelling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9117 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/modelling/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     4545 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/modelling/test_models_isotherm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.937990 pygaps-4.4.2/tests/parsing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/parsing/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3096 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/parsing/test_aif.py
--rw-r--r--   0 runner    (1001) docker     (121)     3752 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/parsing/test_csv.py
--rw-r--r--   0 runner    (1001) docker     (121)     2399 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/parsing/test_excel.py
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/parsing/test_isodb.py
--rw-r--r--   0 runner    (1001) docker     (121)     2587 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/parsing/test_json.py
--rw-r--r--   0 runner    (1001) docker     (121)     9408 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/parsing/test_sqlite_db.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.937990 pygaps-4.4.2/tests/prediction/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/prediction/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     8148 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/prediction/test_iast.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.937990 pygaps-4.4.2/tests/utilities/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8672 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/utilities/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1431 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/utilities/test_coolprop_interaction.py
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/utilities/test_python_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     1303 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/utilities/test_sqlite_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/utilities/test_string_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:15.937990 pygaps-4.4.2/tests/utilities/tst/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/utilities/tst/1.tst
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-11 22:47:02.000000 pygaps-4.4.2/tests/utilities/tst/2.tst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.404965 pygaps-4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-20 00:27:51.000000 pygaps-4.5.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.364965 pygaps-4.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.368965 pygaps-4.5.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-20 00:27:51.000000 pygaps-4.5.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-20 00:27:51.000000 pygaps-4.5.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-20 00:27:51.000000 pygaps-4.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.368965 pygaps-4.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-20 00:27:51.000000 pygaps-4.5.0/.github/workflows/CI.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-20 00:27:51.000000 pygaps-4.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-20 00:27:51.000000 pygaps-4.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-20 00:27:51.000000 pygaps-4.5.0/.release.info
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-20 00:27:51.000000 pygaps-4.5.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-06-20 00:27:51.000000 pygaps-4.5.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-20 00:27:51.000000 pygaps-4.5.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-20 00:27:51.000000 pygaps-4.5.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 00:27:51.000000 pygaps-4.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-06-20 00:28:02.404965 pygaps-4.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-06-20 00:27:51.000000 pygaps-4.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.368965 pygaps-4.5.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-20 00:27:51.000000 pygaps-4.5.0/ci/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.368965 pygaps-4.5.0/ci/ci_old/
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-06-20 00:27:51.000000 pygaps-4.5.0/ci/ci_old/appveyor-download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-20 00:27:51.000000 pygaps-4.5.0/ci/ci_old/appveyor-with-compiler.cmd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.368965 pygaps-4.5.0/ci/ci_old/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-20 00:27:51.000000 pygaps-4.5.0/ci/ci_old/templates/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-20 00:27:51.000000 pygaps-4.5.0/ci/ci_old/templates/appveyor.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-20 00:27:51.000000 pygaps-4.5.0/ci/ci_old/windows-conda-bootstrap.ps1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.368965 pygaps-4.5.0/ci/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-20 00:27:51.000000 pygaps-4.5.0/ci/templates/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.368965 pygaps-4.5.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.360965 pygaps-4.5.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.368965 pygaps-4.5.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.368965 pygaps-4.5.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/docutils.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.376965 pygaps-4.5.0/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47803 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/alphas.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   188676 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/area_calcs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/characterisation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.376965 pygaps-4.5.0/docs/examples/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.380965 pygaps-4.5.0/docs/examples/data/calorimetry/
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/calorimetry/HKUST-1(Cu) KRICT.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/calorimetry/Takeda 5A Test CO2.json
+-rw-r--r--   0 runner    (1001) docker     (123)  4546254 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/calorimetry/data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/calorimetry/header.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13668 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/carbon_x1_n2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.380965 pygaps-4.5.0/docs/examples/data/characterisation/
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/characterisation/MCM-41 N2 77.355.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/characterisation/NaY N2 77.355.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/characterisation/SiO2 N2 77.355.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/characterisation/Takeda 5A N2 77.355.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/characterisation/UiO-66(Zr) N2 77.355.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.380965 pygaps-4.5.0/docs/examples/data/iast/
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/iast/MOF-5(Zn) - IAST - C2H6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/iast/MOF-5(Zn) - IAST - CH4.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.380965 pygaps-4.5.0/docs/examples/data/isosteric/
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/isosteric/BAX 1500 - Isosteric Heat - 298.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/isosteric/BAX 1500 - Isosteric Heat - 323.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/isosteric/BAX 1500 - Isosteric Heat - 348.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/isotherm.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.364965 pygaps-4.5.0/docs/examples/data/parsing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.380965 pygaps-4.5.0/docs/examples/data/parsing/aif/
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/aif/ar_test_77k.aif
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/aif/dmof_C2H6_298k.aif
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/aif/dut-8_etoh_298k.aif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.364965 pygaps-4.5.0/docs/examples/data/parsing/commercial/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.384965 pygaps-4.5.0/docs/examples/data/parsing/commercial/3p/
+-rw-r--r--   0 runner    (1001) docker     (123)  1637702 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/commercial/3p/MOF_N2_77K.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/commercial/3p/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.384965 pygaps-4.5.0/docs/examples/data/parsing/commercial/bel/
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/commercial/bel/DUT-13-CH4-190K.DAT
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/commercial/bel/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.384965 pygaps-4.5.0/docs/examples/data/parsing/commercial/mic/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/commercial/mic/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    59904 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/commercial/mic/Sample_C.xls
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.384965 pygaps-4.5.0/docs/examples/data/parsing/commercial/qnt/
+-rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/commercial/qnt/DUT-6_N2_77K (Raw Analysis Data).txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/commercial/qnt/README
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.384965 pygaps-4.5.0/docs/examples/data/parsing/commercial/smsdvs/
+-rw-r--r--   0 runner    (1001) docker     (123)    26372 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/commercial/smsdvs/13X water 30c.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/commercial/smsdvs/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.384965 pygaps-4.5.0/docs/examples/data/parsing/csv/
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/csv/HKUST-1(Cu) CO2 303.0.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/csv/MCM-41 N2 77.0.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.384965 pygaps-4.5.0/docs/examples/data/parsing/excel/
+-rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/excel/HKUST-1(Cu) CO2 303.0.xls
+-rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/excel/MCM-41 N2 77.0.xls
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.384965 pygaps-4.5.0/docs/examples/data/parsing/json/
+-rw-r--r--   0 runner    (1001) docker     (123)    21354 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/json/AC Ar 77.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/json/AC BAX1500 butane 298.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/json/DUT-8 EtOH 298.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/json/HKUST-1(Cu) CO2 303.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/json/MCM-41 N2 77.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17168 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/json/SURF N2 77.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12498 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/json/UiO-66(Zr) N2 77.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.384965 pygaps-4.5.0/docs/examples/data/parsing/nist/
+-rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/parsing/nist/nist_iso.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.384965 pygaps-4.5.0/docs/examples/data/whittaker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/data/whittaker/whittaker_iso_1.aiff
+-rw-r--r--   0 runner    (1001) docker     (123)    37594 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/database.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   145262 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/dr_da_plots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   253359 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/enthalpy_sorption.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   129960 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/iast.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/import.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    94038 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/initial_enthalpy.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   124568 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/initial_henryc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    83406 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/inspection.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   380720 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/modelling.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   107509 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/novel.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35978 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/parsing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   370417 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/plotting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   399127 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/psd.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   621812 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    54786 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)    69242 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/examples/tplot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   324341 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/favicon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.384965 pygaps-4.5.0/docs/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)    56681 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/figures/SMS-Logo.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    81047 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/figures/db_schema.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33195 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/figures/svp_graph.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52666 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/figures/vle_graph.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.384965 pygaps-4.5.0/docs/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/files/isotherm.aif
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/files/isotherm.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/files/isotherm.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/files/isotherm.xls
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/indices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   104930 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.388965 pygaps-4.5.0/docs/manual/
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/manual/adsorbate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/manual/characterisation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/manual/eqstate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/manual/iast.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/manual/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    23793 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/manual/isotherm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/manual/material.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/manual/modelling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/manual/parsing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/manual/parsing_modes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/manual/plotting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/manual/sqlitedb.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/manual/units.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.388965 pygaps-4.5.0/docs/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.388965 pygaps-4.5.0/docs/reference/characterisation/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/reference/characterisation/alphas_plot.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/reference/characterisation/area_bet.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/reference/characterisation/area_lang.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/reference/characterisation/dubinin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/reference/characterisation/enthalpy_sorption.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/reference/characterisation/initial_hk.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/reference/characterisation/psd_kernel.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/reference/characterisation/psd_meso.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/reference/characterisation/psd_micro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/reference/characterisation/t_plot.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/reference/characterisation/thickness_models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/reference/characterisation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.388965 pygaps-4.5.0/docs/reference/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/reference/core/adsorbate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/reference/core/isotherms.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/reference/core/material.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/reference/core.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/reference/fitting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/reference/iast.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/reference/parsing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/reference/plotting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/reference/units.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/reference/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-20 00:27:51.000000 pygaps-4.5.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-06-20 00:27:51.000000 pygaps-4.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-20 00:28:02.404965 pygaps-4.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.364965 pygaps-4.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.388965 pygaps-4.5.0/src/pygaps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 00:28:02.000000 pygaps-4.5.0/src/pygaps/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.392965 pygaps-4.5.0/src/pygaps/characterisation/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/characterisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14609 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/characterisation/alphas_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/characterisation/area_bet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/characterisation/area_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13200 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/characterisation/dr_da_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/characterisation/enth_sorp_whittaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14871 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/characterisation/initial_enth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/characterisation/initial_henry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7955 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/characterisation/isosteric_enth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/characterisation/models_hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/characterisation/models_kelvin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/characterisation/models_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/characterisation/psd_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32546 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/characterisation/psd_meso.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46537 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/characterisation/psd_micro.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12294 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/characterisation/t_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.392965 pygaps-4.5.0/src/pygaps/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.392965 pygaps-4.5.0/src/pygaps/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28277 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/core/adsorbate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16422 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/core/baseisotherm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/core/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39421 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/core/modelisotherm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49496 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/core/pointisotherm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.392965 pygaps-4.5.0/src/pygaps/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/data/adsorbate_props.json
+-rw-r--r--   0 runner    (1001) docker     (123)    85533 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/data/adsorbates.json
+-rw-r--r--   0 runner    (1001) docker     (123)   212992 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/data/default.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.392965 pygaps-4.5.0/src/pygaps/data/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)   164433 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/data/kernels/DFT-N2-77K-carbon-slit.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.392965 pygaps-4.5.0/src/pygaps/data/stdiso/
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/data/stdiso/Cabot BP280 carbon black.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/data/stdiso/LiChrospher Si-1000 silica.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.396965 pygaps-4.5.0/src/pygaps/graphing/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/graphing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18987 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/graphing/calc_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/graphing/iast_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19063 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/graphing/isotherm_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/graphing/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/graphing/model_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/graphing/mpl_styles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.396965 pygaps-4.5.0/src/pygaps/iast/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/iast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24673 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/iast/pgiast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.396965 pygaps-4.5.0/src/pygaps/modelling/
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/modelling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/modelling/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/modelling/bet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/modelling/da.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/modelling/dr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/modelling/dslangmuir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/modelling/fhvst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/modelling/freundlich.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/modelling/gab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/modelling/henry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/modelling/jensenseaton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/modelling/langmuir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/modelling/quadratic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/modelling/temkinapprox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/modelling/toth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/modelling/tslangmuir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/modelling/virial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/modelling/wvst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.396965 pygaps-4.5.0/src/pygaps/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13630 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/parsing/aif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/parsing/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/parsing/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/parsing/isodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/parsing/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36732 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/parsing/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.396965 pygaps-4.5.0/src/pygaps/units/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12174 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/units/converter_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/units/converter_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.400965 pygaps-4.5.0/src/pygaps/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/utilities/coolprop_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/utilities/hashgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/utilities/isotherm_interpolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/utilities/math_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/utilities/pygaps_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/utilities/python_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/utilities/sqlite_db_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/utilities/sqlite_db_pragmas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/utilities/sqlite_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-20 00:27:51.000000 pygaps-4.5.0/src/pygaps/utilities/string_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.388965 pygaps-4.5.0/src/pygaps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-06-20 00:28:02.000000 pygaps-4.5.0/src/pygaps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-06-20 00:28:02.000000 pygaps-4.5.0/src/pygaps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 00:28:02.000000 pygaps-4.5.0/src/pygaps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 00:28:02.000000 pygaps-4.5.0/src/pygaps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-20 00:28:02.000000 pygaps-4.5.0/src/pygaps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 00:28:02.000000 pygaps-4.5.0/src/pygaps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 00:28:01.000000 pygaps-4.5.0/src/pygaps.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.400965 pygaps-4.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.400965 pygaps-4.5.0/tests/characterisation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/characterisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/characterisation/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/characterisation/test_alphas_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/characterisation/test_area_bet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/characterisation/test_area_langmuir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/characterisation/test_dr_da_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/characterisation/test_enth_sorp_clausclap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/characterisation/test_enth_sorp_whittaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/characterisation/test_initial_enthalpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/characterisation/test_initial_henry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/characterisation/test_models_hk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/characterisation/test_models_kelvin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/characterisation/test_models_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/characterisation/test_psd_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/characterisation/test_psd_meso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/characterisation/test_psd_micro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/characterisation/test_t_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.400965 pygaps-4.5.0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/cli/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.400965 pygaps-4.5.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/core/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/core/test_adsorbate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/core/test_baseisotherm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/core/test_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/core/test_modelisotherm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20160 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/core/test_pointisotherm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.404965 pygaps-4.5.0/tests/graphing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/graphing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/graphing/test_calc_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/graphing/test_iast_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/graphing/test_iso_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.404965 pygaps-4.5.0/tests/modelling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/modelling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/modelling/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/modelling/test_models_isotherm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.404965 pygaps-4.5.0/tests/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/parsing/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/parsing/test_aif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/parsing/test_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/parsing/test_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/parsing/test_isodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/parsing/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/parsing/test_sqlite_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.404965 pygaps-4.5.0/tests/prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/prediction/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/prediction/test_iast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.404965 pygaps-4.5.0/tests/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/utilities/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/utilities/test_coolprop_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/utilities/test_python_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/utilities/test_sqlite_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/utilities/test_string_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:28:02.404965 pygaps-4.5.0/tests/utilities/tst/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/utilities/tst/1.tst
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 00:27:51.000000 pygaps-4.5.0/tests/utilities/tst/2.tst
```

### Comparing `pygaps-4.4.2/.github/ISSUE_TEMPLATE/bug_report.md` & `pygaps-4.5.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/.github/ISSUE_TEMPLATE/feature_request.md` & `pygaps-4.5.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/.github/workflows/CI.yaml` & `pygaps-4.5.0/.github/workflows/CI.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 on:
   [push, pull_request, workflow_dispatch]
 
 jobs:
   linting-checks:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python 3.8
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: 3.8
         cache: 'pip'
         cache-dependency-path: '**/setup.cfg'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade setuptools
@@ -26,17 +26,17 @@
         isort --verbose --check-only --diff src tests
         flake8 src tests
         # pylint src tests
 
   docs-build:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python 3.8
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: 3.8
         cache: 'pip'
         cache-dependency-path: |
           setup.cfg
           docs/conf.py
     - name: Install dependencies
@@ -58,18 +58,18 @@
     defaults:
       run:
         shell: bash -l {0}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
-        python-version : ['3.7', '3.8', '3.9', '3.10']
+        python-version : ['3.7', '3.8', '3.9', '3.10', '3.11']
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
 
     - name: Set up Conda
       uses: conda-incubator/setup-miniconda@v2
       with:
         python-version: ${{ matrix.python-version }}
         activate-environment: test
 
@@ -101,18 +101,18 @@
 
   build-publish:
       runs-on: ubuntu-latest
       needs: [linting-checks, docs-build, unit-tests]
       if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
 
       steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
       - name: Set up Python 3.x
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: '3.x'
 
       - name: Install dependencies
         run: |
           python -m pip install build
           python -m pip install --upgrade setuptools wheel
```

### Comparing `pygaps-4.4.2/.gitignore` & `pygaps-4.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/.readthedocs.yaml` & `pygaps-4.5.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/.release.info` & `pygaps-4.5.0/.release.info`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/CHANGELOG.rst` & `pygaps-4.5.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 
 Changelog
 =========
 
+4.5.0 (2023-06-20)
+
+* Added a new function that calculates the enthalpy of adsorption using a method
+  proposed by Whittaker et al in `pygaps.characterisation.enth_sorp_whittaker`.
+  Thanks to L Scott Blankenship for contribution!
+* Updated AIF parser to latest version. Thanks to Jack Evans for contribution.
+* Refactored DR/DA calculations.
+* Docs updating to fix issue #42
+* Added data types to excel output parsing to fix edge cases where these were not
+  correctly parsed.
+* Testing correctly on Python 3.11.
+* Fixed various accumulating issues and bugs and deprecations.
+
 4.4.0 (2022-09-03)
 ------------------
 
 * Drop python 3.6
 * Parsing of instrument files is now spun off into
   a separate package for ease of maintenance.
   See: https://github.com/AIF-development-team/adsorption-file-parser
```

### Comparing `pygaps-4.4.2/CITATION.cff` & `pygaps-4.5.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/CONTRIBUTING.rst` & `pygaps-4.5.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/LICENSE` & `pygaps-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/PKG-INFO` & `pygaps-4.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygaps
-Version: 4.4.2
+Version: 4.5.0
 Summary: A framework for processing adsorption data for porous materials.
 Home-page: https://github.com/pauliacomi/pygaps
 Author: Paul Iacomi
 Author-email: mail@pauliacomi.com
 License: MIT license
 Project-URL: Documentation, https://pygaps.readthedocs.io
 Project-URL: Source Code, https://github.com/pauliacomi/pygaps
```

### Comparing `pygaps-4.4.2/README.rst` & `pygaps-4.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/ci/bootstrap.py` & `pygaps-4.5.0/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/ci/ci_old/appveyor-download.py` & `pygaps-4.5.0/ci/ci_old/appveyor-download.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/ci/ci_old/appveyor-with-compiler.cmd` & `pygaps-4.5.0/ci/ci_old/appveyor-with-compiler.cmd`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/ci/ci_old/templates/.travis.yml` & `pygaps-4.5.0/ci/ci_old/templates/.travis.yml`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/ci/ci_old/templates/appveyor.yml` & `pygaps-4.5.0/ci/ci_old/templates/appveyor.yml`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/ci/ci_old/windows-conda-bootstrap.ps1` & `pygaps-4.5.0/ci/ci_old/windows-conda-bootstrap.ps1`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/ci/templates/pyproject.toml` & `pygaps-4.5.0/ci/templates/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/_static/css/custom.css` & `pygaps-4.5.0/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/conf.py` & `pygaps-4.5.0/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,25 +99,26 @@
 # github badges being stored on another server
 suppress_warnings = [
     'image.nonlocal_uri',
 ]
 
 # External links
 extlinks = {
-    'issue': ('https://github.com/pauliacomi/pygaps/issues/%s', '#'),
-    'pr': ('https://github.com/pauliacomi/pygaps/pull/%s', 'PR #'),
+    'issue': ('https://github.com/pauliacomi/pygaps/issues/%s', '#%s'),
+    'pr': ('https://github.com/pauliacomi/pygaps/pull/%s', 'PR #%s'),
 }
 
 linkcheck_timeout = 3
 linkcheck_retries = 2
 linkcheck_ignore = [
     r'https://github.com/pauliacomi/pygaps/compare/.+',
     r'https://requires.io/.+',
     r'https://twitter.com/.+',
     r'https://www.coolprop.org/.+',
+    r'https://doi.org/.+',
 ]
 
 # Checking for internal links
 nitpicky = True
 nitpick_ignore = [
     ('py:class', 'numpy.ndarray'),
     ('py:class', 'pandas.core.frame.DataFrame'),
```

### Comparing `pygaps-4.4.2/docs/examples/alphas.ipynb` & `pygaps-4.5.0/docs/examples/alphas.ipynb`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/area_calcs.ipynb` & `pygaps-4.5.0/docs/examples/area_calcs.ipynb`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/calorimetry/HKUST-1(Cu) KRICT.json` & `pygaps-4.5.0/docs/examples/data/calorimetry/HKUST-1(Cu) KRICT.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/calorimetry/Takeda 5A Test CO2.json` & `pygaps-4.5.0/docs/examples/data/calorimetry/Takeda 5A Test CO2.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/calorimetry/data.csv` & `pygaps-4.5.0/docs/examples/data/calorimetry/data.csv`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/calorimetry/header.csv` & `pygaps-4.5.0/docs/examples/data/calorimetry/header.csv`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/carbon_x1_n2.json` & `pygaps-4.5.0/docs/examples/data/carbon_x1_n2.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/characterisation/MCM-41 N2 77.355.json` & `pygaps-4.5.0/docs/examples/data/characterisation/MCM-41 N2 77.355.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/characterisation/NaY N2 77.355.json` & `pygaps-4.5.0/docs/examples/data/characterisation/NaY N2 77.355.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/characterisation/SiO2 N2 77.355.json` & `pygaps-4.5.0/docs/examples/data/characterisation/SiO2 N2 77.355.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/characterisation/Takeda 5A N2 77.355.json` & `pygaps-4.5.0/docs/examples/data/characterisation/Takeda 5A N2 77.355.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/characterisation/UiO-66(Zr) N2 77.355.json` & `pygaps-4.5.0/docs/examples/data/characterisation/UiO-66(Zr) N2 77.355.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/iast/MOF-5(Zn) - IAST - C2H6.json` & `pygaps-4.5.0/docs/examples/data/iast/MOF-5(Zn) - IAST - C2H6.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/iast/MOF-5(Zn) - IAST - CH4.json` & `pygaps-4.5.0/docs/examples/data/iast/MOF-5(Zn) - IAST - CH4.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/isosteric/BAX 1500 - Isosteric Heat - 298.json` & `pygaps-4.5.0/docs/examples/data/isosteric/BAX 1500 - Isosteric Heat - 298.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/isosteric/BAX 1500 - Isosteric Heat - 323.json` & `pygaps-4.5.0/docs/examples/data/isosteric/BAX 1500 - Isosteric Heat - 323.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/isosteric/BAX 1500 - Isosteric Heat - 348.json` & `pygaps-4.5.0/docs/examples/data/isosteric/BAX 1500 - Isosteric Heat - 348.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/isotherm.json` & `pygaps-4.5.0/docs/examples/data/isotherm.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/parsing/aif/ar_test_77k.aif` & `pygaps-4.5.0/docs/examples/data/parsing/aif/ar_test_77k.aif`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 data_data_raw2aifv005
-_audit_aif_version 1.0
+_audit_aif_version 'd546195'
 _exptl_operator 'Volodymyr'
 _exptl_date 2020-06-03T00:00:00
 _exptl_instrument 'BEL 00218'
 _exptl_adsorptive Ar
 _exptl_temperature 87.00
-_exptl_sample_mass 0.14320
-_sample_id 'aus der BOX'
-_sample_material_id 'unknown'
+_adsnt_sample_mass 0.14320
+_adsnt_sample_id 'aus der BOX'
+_adsnt_material_id 'unknown'
 _units_temperature K
 _units_pressure kPa
 _units_mass g
 _units_loading 'ml(STP) g-1'
 
 loop_
 _adsorp_pressure
```

### Comparing `pygaps-4.4.2/docs/examples/data/parsing/aif/dmof_C2H6_298k.aif` & `pygaps-4.5.0/docs/examples/data/parsing/aif/dmof_C2H6_298k.aif`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 data_data_raw2aifv005
-_audit_aif_version 1.0
+_audit_aif_version 'd546195'
 _exptl_operator 'single gas'
 _exptl_date 2019-08-19T00:00:00
 _exptl_instrument 'BEL VC-05'
 _exptl_adsorptive C2H6
 _exptl_temperature 298.15
-_exptl_sample_mass 0.817
-_sample_id '[Zn2(tm-bdc)2(dabco)]'
-_sample_material_id 'DMOF'
+_adsnt_sample_mass 0.817
+_adsnt_sample_id '[Zn2(tm-bdc)2(dabco)]'
+_adsnt_material_id 'DMOF'
 _units_temperature K
 _units_pressure kPa
 _units_mass g
 _units_loading 'cm^3(STP) g^-1'
 
 loop_
 _adsorp_pressure
```

### Comparing `pygaps-4.4.2/docs/examples/data/parsing/aif/dut-8_etoh_298k.aif` & `pygaps-4.5.0/docs/examples/data/parsing/aif/dut-8_etoh_298k.aif`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 data_data_raw2aifv005
-_audit_aif_version 1.0
+_audit_aif_version 'd546195'
 _exptl_operator 'Leila'
 _exptl_date 2020-10-19T00:00:00
 _exptl_instrument 'BEL 00348'
 _exptl_adsorptive C2H5OH
 _exptl_temperature 298.00
-_exptl_sample_mass 0.02460
-_sample_id 'LA-133_DUT-8(Zn)_isp_cp_EtOH_298K'
-_sample_material_id 'DUT-8'
+_adsnt_sample_mass 0.02460
+_adsnt_sample_id 'LA-133_DUT-8(Zn)_isp_cp_EtOH_298K'
+_adsnt_material_id 'DUT-8'
 _units_temperature K
 _units_pressure kPa
 _units_mass g
 _units_loading 'ml(STP) g-1'
 
 loop_
 _adsorp_pressure
```

### Comparing `pygaps-4.4.2/docs/examples/data/parsing/commercial/3p/MOF_N2_77K.xlsx` & `pygaps-4.5.0/docs/examples/data/parsing/commercial/3p/MOF_N2_77K.xlsx`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/parsing/commercial/bel/DUT-13-CH4-190K.DAT` & `pygaps-4.5.0/docs/examples/data/parsing/commercial/bel/DUT-13-CH4-190K.DAT`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/parsing/commercial/mic/Sample_C.xls` & `pygaps-4.5.0/docs/examples/data/parsing/commercial/mic/Sample_C.xls`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/parsing/commercial/qnt/DUT-6_N2_77K (Raw Analysis Data).txt` & `pygaps-4.5.0/docs/examples/data/parsing/commercial/qnt/DUT-6_N2_77K (Raw Analysis Data).txt`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/parsing/commercial/smsdvs/13X water 30c.xlsx` & `pygaps-4.5.0/docs/examples/data/parsing/commercial/smsdvs/13X water 30c.xlsx`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/parsing/csv/HKUST-1(Cu) CO2 303.0.csv` & `pygaps-4.5.0/docs/examples/data/parsing/csv/HKUST-1(Cu) CO2 303.0.csv`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/parsing/csv/MCM-41 N2 77.0.csv` & `pygaps-4.5.0/docs/examples/data/parsing/csv/MCM-41 N2 77.0.csv`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/parsing/excel/HKUST-1(Cu) CO2 303.0.xls` & `pygaps-4.5.0/docs/examples/data/parsing/excel/HKUST-1(Cu) CO2 303.0.xls`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/parsing/excel/MCM-41 N2 77.0.xls` & `pygaps-4.5.0/docs/examples/data/parsing/excel/MCM-41 N2 77.0.xls`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/parsing/json/AC Ar 77.json` & `pygaps-4.5.0/docs/examples/data/parsing/json/AC Ar 77.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/parsing/json/AC BAX1500 butane 298.json` & `pygaps-4.5.0/docs/examples/data/parsing/json/AC BAX1500 butane 298.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/parsing/json/DUT-8 EtOH 298.json` & `pygaps-4.5.0/docs/examples/data/parsing/json/DUT-8 EtOH 298.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/parsing/json/HKUST-1(Cu) CO2 303.json` & `pygaps-4.5.0/docs/examples/data/parsing/json/HKUST-1(Cu) CO2 303.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/parsing/json/MCM-41 N2 77.json` & `pygaps-4.5.0/docs/examples/data/parsing/json/MCM-41 N2 77.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/parsing/json/SURF N2 77.json` & `pygaps-4.5.0/docs/examples/data/parsing/json/SURF N2 77.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/parsing/json/UiO-66(Zr) N2 77.json` & `pygaps-4.5.0/docs/examples/data/parsing/json/UiO-66(Zr) N2 77.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/data/parsing/nist/nist_iso.json` & `pygaps-4.5.0/docs/examples/data/parsing/nist/nist_iso.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/database.ipynb` & `pygaps-4.5.0/docs/examples/database.ipynb`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/iast.ipynb` & `pygaps-4.5.0/docs/examples/iast.ipynb`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/import.ipynb` & `pygaps-4.5.0/docs/examples/import.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9420093795093796%*

 * *Differences: {"'cells'": "{insert: [(10, OrderedDict([('cell_type', 'code'), ('execution_count', None), "*

 * *            "('metadata', OrderedDict()), ('outputs', []), ('source', "*

 * *            "['isotherms_enth_whittaker_paths = list(Path(json_path / "*

 * *            '\\\'whittaker\\\').rglob("*.aiff"))\\n\', \'isotherms_enth_whittaker = [\\n\', \'    '*

 * *            "pgp.isotherm_from_aif(filepath)\\n', '    for filepath in "*

 * *            "isotherms_enth_whittaker_paths\\n', ']'])]))]}",*

 * * "'metadata'": "{'kernelspec': {'display […]*

```diff
@@ -143,31 +143,49 @@
                 "isotherms_isosteric_paths = list(Path(json_path / 'isosteric').rglob(\"*.json\"))\n",
                 "isotherms_isosteric = [\n",
                 "    pgp.isotherm_from_json(filepath)\n",
                 "    for filepath in isotherms_isosteric_paths\n",
                 "]\n",
                 "print('Selected', len(isotherms_isosteric), 'isotherms for isosteric enthalpy calculation')"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "isotherms_enth_whittaker_paths = list(Path(json_path / 'whittaker').rglob(\"*.aiff\"))\n",
+                "isotherms_enth_whittaker = [\n",
+                "    pgp.isotherm_from_aif(filepath)\n",
+                "    for filepath in isotherms_enth_whittaker_paths\n",
+                "]"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "sci",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.9.13"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "bb92cfc77ebe3751b7fb3df8620ceb006227daaf69256df93b17635e0b7c66c1"
+            }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `pygaps-4.4.2/docs/examples/initial_enthalpy.ipynb` & `pygaps-4.5.0/docs/examples/initial_enthalpy.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9533730158730158%*

 * *Differences: {"'metadata'": "{'kernelspec': {'display_name': 'sci'}, 'language_info': {'version': '3.9.13'}, "*

 * *               "'vscode': OrderedDict([('interpreter', OrderedDict([('hash', "*

 * *               "'bb92cfc77ebe3751b7fb3df8620ceb006227daaf69256df93b17635e0b7c66c1')]))])}"}*

```diff
@@ -314,27 +314,32 @@
                 "res = pgc.initial_enthalpy_comp(isotherm, 'enthalpy', verbose=True)\n",
                 "plt.show()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "sci",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.9.13"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "bb92cfc77ebe3751b7fb3df8620ceb006227daaf69256df93b17635e0b7c66c1"
+            }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `pygaps-4.4.2/docs/examples/initial_henryc.ipynb` & `pygaps-4.5.0/docs/examples/initial_henryc.ipynb`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/inspection.ipynb` & `pygaps-4.5.0/docs/examples/inspection.ipynb`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/novel.png` & `pygaps-4.5.0/docs/examples/novel.png`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/parsing.ipynb` & `pygaps-4.5.0/docs/examples/parsing.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984203296703297%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, '%matplotlib inline\\n'), (1, '\\n')]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.9.13 (main, Oct 13 2022, 21:23:06) [MSC v.1916 64 "*

 * *               "bit (AMD64)]'}}"}*

```diff
@@ -17,14 +17,16 @@
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
+                "%matplotlib inline\n",
+                "\n",
                 "from pathlib import Path\n",
                 "import pygaps.parsing as pgp\n",
                 "\n",
                 "# Get directory paths\n",
                 "base_path = Path.cwd() / 'data' / 'parsing'\n",
                 "\n",
                 "# Find files\n",
@@ -383,15 +385,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.12"
+            "version": "3.9.13 (main, Oct 13 2022, 21:23:06) [MSC v.1916 64 bit (AMD64)]"
         },
         "vscode": {
             "interpreter": {
                 "hash": "bb92cfc77ebe3751b7fb3df8620ceb006227daaf69256df93b17635e0b7c66c1"
             }
         }
     },
```

### Comparing `pygaps-4.4.2/docs/examples/plotting.ipynb` & `pygaps-4.5.0/docs/examples/plotting.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9531646825396826%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, '%matplotlib inline\\n')]}}}",*

 * * "'metadata'": "{'kernelspec': {'display_name': 'sci'}, 'language_info': {'version': '3.9.13 "*

 * *               "(main, Oct 13 2022, 21:23:06) [MSC v.1916 64 bit (AMD64)]'}, 'vscode': "*

 * *               "OrderedDict([('interpreter', OrderedDict([('hash', "*

 * *               "'bb92cfc77ebe3751b7fb3df8620ceb006227daaf69256df93b17635e0b7c66c1')]))])}"}*

```diff
@@ -26,14 +26,15 @@
                         "Selected 2 room temperature calorimetry isotherms\n",
                         "Selected 2 isotherms for IAST calculation\n",
                         "Selected 3 isotherms for isosteric enthalpy calculation\n"
                     ]
                 }
             ],
             "source": [
+                "%matplotlib inline\n",
                 "%run import.ipynb\n",
                 "import matplotlib.pyplot as plt"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -431,27 +432,32 @@
                 ")\n",
                 "ax.set_title(\"Only desorption branch\")"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "sci",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.7"
+            "version": "3.9.13 (main, Oct 13 2022, 21:23:06) [MSC v.1916 64 bit (AMD64)]"
+        },
+        "vscode": {
+            "interpreter": {
+                "hash": "bb92cfc77ebe3751b7fb3df8620ceb006227daaf69256df93b17635e0b7c66c1"
+            }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `pygaps-4.4.2/docs/examples/psd.ipynb` & `pygaps-4.5.0/docs/examples/psd.ipynb`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/test.png` & `pygaps-4.5.0/docs/examples/test.png`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/examples/tplot.ipynb` & `pygaps-4.5.0/docs/examples/tplot.ipynb`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/favicon.ico` & `pygaps-4.5.0/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/favicon.png` & `pygaps-4.5.0/docs/favicon.png`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/favicon.svg` & `pygaps-4.5.0/docs/favicon.svg`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/figures/SMS-Logo.jpg` & `pygaps-4.5.0/docs/figures/SMS-Logo.jpg`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/figures/db_schema.png` & `pygaps-4.5.0/docs/figures/db_schema.png`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/figures/svp_graph.png` & `pygaps-4.5.0/docs/figures/svp_graph.png`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/figures/vle_graph.png` & `pygaps-4.5.0/docs/figures/vle_graph.png`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/files/isotherm.aif` & `pygaps-4.5.0/docs/files/isotherm.aif`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 data_830a707e2c95c8db400979a9cba7c92d
-_audit_aif_version 1.0
+_audit_aif_version 'd546195'
 _audit_creation_method pyGAPS
 _exptl_adsorptive 'carbon dioxide'
 _exptl_temperature 303.0
-_sample_material_id 'HKUST-1(Cu)'
+_adsnt_material_id 'HKUST-1(Cu)'
 _exptl_operator 'PI'
 _exptl_date '2010-05-21 00:00:00'
 _exptl_instrument 'device1'
-_exptl_activation_temperature '150.0'
-_sample_id 'KRICT'
+_adsnt_degas_temperature '150.0'
+_adsnt_sample_id 'KRICT'
 _units_temperature K
 _units_pressure bar
 _units_loading mmol/g
 _pygaps_iso_type 'calorimetry'
 _pygaps_project 'ACRONYM'
 _pygaps_comment 'a comment'
```

### Comparing `pygaps-4.4.2/docs/files/isotherm.csv` & `pygaps-4.5.0/docs/files/isotherm.csv`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/files/isotherm.json` & `pygaps-4.5.0/docs/files/isotherm.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/files/isotherm.xls` & `pygaps-4.5.0/docs/files/isotherm.xls`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/installation.rst` & `pygaps-4.5.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/logo.png` & `pygaps-4.5.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/logo.svg` & `pygaps-4.5.0/docs/logo.svg`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/manual/adsorbate.rst` & `pygaps-4.5.0/docs/manual/adsorbate.rst`

 * *Files 8% similar despite different names*

```diff
@@ -117,20 +117,25 @@
 
 The :class:`~pygaps.core.adsorbate.Adsorbate` class has methods which allow the
 properties of the adsorbate to be either calculated using the CoolProp or
 REFPROP backend or retrieved as a string from the internal dictionary. The
 properties which can be calculated are:
 
 - Molar mass: :meth:`~pygaps.core.adsorbate.Adsorbate.molar_mass`.
+- Triple point pressure: :meth:`~pygaps.core.adsorbate.Adsorbate.p_triple`.
+- Triple point temperature: :meth:`~pygaps.core.adsorbate.Adsorbate.t_triple`.
+- Critical point pressure: :meth:`~pygaps.core.adsorbate.Adsorbate.p_critical`.
+- Critical point temperature: :meth:`~pygaps.core.adsorbate.Adsorbate.t_critical`.
 - Saturation pressure: :meth:`~pygaps.core.adsorbate.Adsorbate.saturation_pressure`.
 - Surface tension: :meth:`~pygaps.core.adsorbate.Adsorbate.surface_tension`.
 - Liquid density: :meth:`~pygaps.core.adsorbate.Adsorbate.liquid_density`.
 - Molar liquid density: :meth:`~pygaps.core.adsorbate.Adsorbate.liquid_molar_density`.
 - Gas density: :meth:`~pygaps.core.adsorbate.Adsorbate.gas_density`.
 - Molar gas density: :meth:`~pygaps.core.adsorbate.Adsorbate.gas_molar_density`.
+- Enthalpy of vaporisation: :meth:`~pygaps.core.adsorbate.Adsorbate.enthalpy_vaporisation`.
 - Enthalpy of liquefaction: :meth:`~pygaps.core.adsorbate.Adsorbate.enthalpy_liquefaction`.
 
 For example, for the :class:`~pygaps.core.adsorbate.Adsorbate` created above, to
 get the vapour pressure at 25 degrees in bar.
 
 .. code:: python
 
@@ -153,19 +158,19 @@
 
     my_adsorbate.saturation_pressure(298, calculate=False)
     >> 2.2              # Value in the `properties` dictionary
 
 For calculations of other properties, the
 `CoolProp backend <https://www.coolprop.org/coolprop/wrappers/Python/index.html>`__
 can be accessed directly using the ``backend`` property. To calculate the
-critical temperature for example.
+reducing temperature for example.
 
 .. code:: python
 
-    my_adsorbate.backend.T_critical()
+    my_adsorbate.backend.T_reducing()
 
 
 .. _adsorbate-manual-manage:
 
 Adsorbate management
 --------------------
```

### Comparing `pygaps-4.4.2/docs/manual/characterisation.rst` & `pygaps-4.5.0/docs/manual/characterisation.rst`

 * *Files 6% similar despite different names*

```diff
@@ -14,38 +14,41 @@
 The framework currently provides the following functionality for material
 characterisation:
 
 - BET surface area :mod:`~pygaps.characterisation.area_bet`
 - Langmuir surface area :mod:`~pygaps.characterisation.area_lang`
 - The t-plot method :mod:`~pygaps.characterisation.t_plots`
 - The :math:`\alpha_s` method :mod:`~pygaps.characterisation.alphas_plots`
-- Pore size distribution (PSD) calculations
+- Pore size distribution (PSD):
 
   - Mesoporous PSD calculations function
     :meth:`~pygaps.characterisation.psd_meso.psd_mesoporous` with the module
     containing the individual model references:
     :mod:`pygaps.characterisation.psd_meso`
   - Microporous PSD calculations function
     :meth:`~pygaps.characterisation.psd_micro.psd_microporous` with the module
     containing the individual model references:
     :mod:`~pygaps.characterisation.psd_micro`
   - Kernel fitting PSD functions, like DFT
     :meth:`~pygaps.characterisation.psd_kernel.psd_dft` with the module
     containing the individual model references:
     :mod:`~pygaps.characterisation.psd_kernel`
 
-- Isosteric enthalpy of adsorption calculations
-  :meth:`~pygaps.characterisation.isosteric_enth`
+- Enthalpy of adsorption determination:
+
+  - Isosteric enthalpy through the Clausius-Clapeyron method (multiple isotherms
+    at different temperatures): :meth:`~pygaps.characterisation.isosteric_enth`
+  - Isosteric enthalpy through the Whittaker method (from a model fit to an
+    isotherm): :meth:`~pygaps.characterisation.enth_sorp_whittaker`
+
 - Dubinin-Radushevitch and Dubinin-Astakov plots
   (:meth:`~pygaps.characterisation.dr_da_plots.dr_plot`,
   :meth:`~pygaps.characterisation.dr_da_plots.da_plot`)
 - Initial Henry constant calculation
   :mod:`~pygaps.characterisation.initial_henry`
-- Initial enthalpy of adsorption calculation (from isotherms with enthalpy data)
-  :mod:`~pygaps.characterisation.initial_enth`
 
 More info about each function and its usage can be found on their respective
 page.
 
 .. caution::
 
     Before using the provided characterisation functions, make sure you are
```

### Comparing `pygaps-4.4.2/docs/manual/eqstate.rst` & `pygaps-4.5.0/docs/manual/eqstate.rst`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/manual/iast.rst` & `pygaps-4.5.0/docs/manual/iast.rst`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/manual/index.rst` & `pygaps-4.5.0/docs/manual/index.rst`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/manual/isotherm.rst` & `pygaps-4.5.0/docs/manual/isotherm.rst`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/manual/material.rst` & `pygaps-4.5.0/docs/manual/material.rst`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/manual/modelling.rst` & `pygaps-4.5.0/docs/manual/modelling.rst`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/manual/parsing.rst` & `pygaps-4.5.0/docs/manual/parsing.rst`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/manual/plotting.rst` & `pygaps-4.5.0/docs/manual/plotting.rst`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/manual/sqlitedb.rst` & `pygaps-4.5.0/docs/manual/sqlitedb.rst`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/manual/units.rst` & `pygaps-4.5.0/docs/manual/units.rst`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/reference/fitting.rst` & `pygaps-4.5.0/docs/reference/fitting.rst`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/reference/index.rst` & `pygaps-4.5.0/docs/reference/index.rst`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/reference/parsing.rst` & `pygaps-4.5.0/docs/reference/parsing.rst`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/reference/plotting.rst` & `pygaps-4.5.0/docs/reference/plotting.rst`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/docs/reference/utilities.rst` & `pygaps-4.5.0/docs/reference/utilities.rst`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/pyproject.toml` & `pygaps-4.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -127,25 +127,27 @@
 legacy_tox_ini = """
 [tox]
 isolated_build = True
 envlist =
     clean,
     check,
     docs,
+    py311-cover,
     py310-cover,
     py36-cover,
     py37-cover,
     py38-cover,
     py39-cover,
     report
 
 [testenv]
 wheel = true
 basepython =
     bootstrap: python
+    py311: {env:TOXPYTHON:python3.11-cover}
     py310: {env:TOXPYTHON:python3.10-cover}
     py36: {env:TOXPYTHON:python3.6-cover}
     py37: {env:TOXPYTHON:python3.7-cover}
     py38: {env:TOXPYTHON:python3.8-cover}
     py39: {env:TOXPYTHON:python3.9-cover}
     {docs,spell,clean,check,report,codecov}: {env:TOXPYTHON:python3}
 setenv =
```

### Comparing `pygaps-4.4.2/setup.cfg` & `pygaps-4.5.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -29,25 +29,25 @@
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering :: Physics
 	Topic :: Scientific/Engineering :: Chemistry
 
 [options]
 package_dir = 
 	=src
-packages = find:
+packages = find_namespace:
 python_requires = >=3.7
 zip_safe = True
 include_package_data = True
 tests_require = 
 	pytest
 	pytest-cov
 	coverage[toml]
 	nose
 install_requires = 
-	adsorption-file-parser >= 0.2.2
+	adsorption-file-parser >= 0.2.6
 	numpy >= 1.16.5
 	scipy >= 1.5
 	pandas >= 1.1
 	matplotlib >= 3.3
 	coolprop >= 6.0
 	xlrd >= 1.1
 	xlwt >= 1.3
@@ -57,17 +57,15 @@
 	importlib_resources; python_version < "3.9"
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 * = *.txt, *.rst
-pygaps.data = *
-pygaps.data.kernels = *.csv
-pygaps.data.stdiso = *.csv
+pygaps.data = *, **
 
 [options.entry_points]
 console_scripts = 
 	pygaps = pygaps.cli:main
 
 [options.extras_require]
 dev =
```

### Comparing `pygaps-4.4.2/src/pygaps/__init__.py` & `pygaps-4.5.0/src/pygaps/__init__.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/characterisation/__init__.py` & `pygaps-4.5.0/src/pygaps/characterisation/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .alphas_plots import alpha_s_raw
 from .area_bet import area_BET
 from .area_bet import area_BET_raw
 from .area_lang import area_langmuir
 from .area_lang import area_langmuir_raw
 from .dr_da_plots import da_plot
 from .dr_da_plots import dr_plot
+from .enth_sorp_whittaker import enthalpy_sorption_whittaker
 from .initial_enth import initial_enthalpy_comp
 from .initial_enth import initial_enthalpy_point
 from .initial_henry import initial_henry_slope
 from .initial_henry import initial_henry_virial
 from .isosteric_enth import isosteric_enthalpy
 from .isosteric_enth import isosteric_enthalpy_raw
 from .psd_kernel import psd_dft
```

### Comparing `pygaps-4.4.2/src/pygaps/characterisation/alphas_plots.py` & `pygaps-4.5.0/src/pygaps/characterisation/alphas_plots.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/characterisation/area_bet.py` & `pygaps-4.5.0/src/pygaps/characterisation/area_bet.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/characterisation/area_lang.py` & `pygaps-4.5.0/src/pygaps/characterisation/area_lang.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/characterisation/dr_da_plots.py` & `pygaps-4.5.0/src/pygaps/characterisation/dr_da_plots.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,30 +67,33 @@
 
     .. math::
 
         V_{ads} = V_{t} \exp\Big[\Big(\frac{\Delta G}{\varepsilon}\Big)^{2}\Big]
 
     Here :math:`\Delta G` is the change in Gibbs free energy
     :math:`\Delta G = - RT \ln(p_0/p)` and :math:`\varepsilon`
-    is a characteristic energy of adsorption.
+    is a characteristic energy of adsorption. Substituting:
+
+    .. math::
+
+        V_{ads} = V_{t} - e^{-\Big(\frac{RT}{\varepsilon}\Big)^2 \ln^2{\frac{p_0}{p}}} = V_{t} - e^{-D \ln^2{\frac{p_0}{p}}}
 
     If an experimental isotherm is consistent with the DR model,
     the equation can be used to obtain the total pore volume
-    and energy of adsorption. The DR equation is first linearised:
+    and energy of adsorption. The DR equation is linearised:
 
     .. math::
 
-        \log_{10}{V_{ads}} = \log_{10}{V_{t}} -
-        \ln10\Big(\frac{RT}{\varepsilon}\Big)^2 \Big[\log_{10}{\frac{p_0}{p}}\Big]^2
+        \ln{V_{ads}} = \ln{V_{t}} - \Big(\frac{RT}{\varepsilon}\Big)^2 \ln^2{\Big[\frac{p_0}{p}}\Big]
 
     Isotherm loading is converted to volume adsorbed by
     assuming that the density of the adsorbed phase is equal to
     bulk liquid density at the isotherm temperature.
-    Afterwards :math:`\log_{10}{V_{ads}}` is plotted
-    against :math:`\log^2_{10}{p_0/p}`,
+    Afterwards :math:`\ln{V_{ads}}` is plotted
+    against :math:`\ln^2{p_0/p}`,
     and fitted with a best-fit line. The intercept of this
     line can be used to calculate the total pore volume,
     while the slope is proportional to the characteristic
     energy of adsorption :math:`\varepsilon`.
 
     References
     ----------
@@ -169,30 +172,33 @@
         V_{ads} = V_{t} \exp\Big[\Big(\frac{\Delta G}{\varepsilon}\Big)^{n}\Big]
 
     Here :math:`\Delta G` is the change in Gibbs free energy
     :math:`\Delta G = - RT \ln(p_0/p)` and :math:`\varepsilon`
     is a characteristic energy of adsorption.
     The exponent :math:`n` is a fitting coefficient, often taken between
     1 (described as surface adsorption) and 3 (micropore adsorption).
-    The exponent can also be related to surface heterogeneity.
+    The exponent can also be related to surface heterogeneity.  Substituting:
+
+    .. math::
+
+        V_{ads} = V_{t} - e^{-\Big(\frac{RT}{\varepsilon}\Big)^n \ln^n{\frac{p_0}{p}}} = V_{t} - e^{-D \ln^n{\frac{p_0}{p}}}
 
     If an experimental isotherm is consistent with the DA model,
     the equation can be used to obtain the total pore volume
     and energy of adsorption. The DA equation is first linearised:
 
     .. math::
 
-        \log_{10}{V_{ads}} = \log_{10}{V_{t}} -
-        (\ln10)^{n-1}\Big(\frac{RT}{\varepsilon}\Big)^n \Big[\log_{10}{\frac{p_0}{p}}\Big]^n
+        \ln{V_{ads}} = \ln{V_{t}} - \Big(\frac{RT}{\varepsilon}\Big)^n \ln^n{\Big[\frac{p_0}{p}}\Big]
 
     Isotherm loading is converted to volume adsorbed by
     assuming that the density of the adsorbed phase is equal to
     bulk liquid density at the isotherm temperature.
-    Afterwards :math:`\log_{10}{V_{ads}}` is plotted
-    against :math:`\log^n_{10}{p_0/p}`,
+    Afterwards :math:`\ln{V_{ads}}` is plotted
+    against :math:`\ln^n{p_0/p}`,
     and fitted with a best-fit line. The intercept of this
     line can be used to calculate the total pore volume,
     while the slope is proportional to the characteristic
     energy of adsorption :math:`\varepsilon`.
 
     References
     ----------
@@ -380,31 +386,30 @@
         if not res.success:
             raise CalculationError("""Could not obtain a linear fit on the data provided.""")
         exp = res.x
 
     slope, intercept, corr_coef = dr_fit(exp, ret=True)
 
     # Calculate final result values
-    microp_volume = 10**intercept
-    potential = (-numpy.log(10)**(exp - 1) *
-                 (constants.gas_constant * iso_temp)**(exp) / slope)**(1 / exp) / 1000
+    microp_volume = numpy.exp(intercept)
+    potential = (constants.gas_constant * iso_temp) / (-slope)**(1 / exp) / 1000
 
     return (
         microp_volume,
         potential,
         exp,
         slope,
         intercept,
         minimum,
         maximum,
         corr_coef,
     )
 
 
 def log_v_adj(loading, molar_mass, liquid_density):
-    """Base 10 logarithm of volumetric uptake."""
-    return numpy.log10(loading * molar_mass / liquid_density)
+    """Log of volumetric uptake."""
+    return numpy.log(loading * molar_mass / liquid_density)
 
 
 def log_p_exp(pressure, exp):
-    """Base 10 logarithm of p_0/p raised to the DA exponent."""
-    return (-numpy.log10(pressure))**exp
+    """Log of p_0/p raised to the DA exponent."""
+    return (-numpy.log(pressure))**exp
```

### Comparing `pygaps-4.4.2/src/pygaps/characterisation/initial_enth.py` & `pygaps-4.5.0/src/pygaps/characterisation/initial_enth.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/characterisation/initial_henry.py` & `pygaps-4.5.0/src/pygaps/characterisation/initial_henry.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/characterisation/isosteric_enth.py` & `pygaps-4.5.0/src/pygaps/characterisation/isosteric_enth.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 def isosteric_enthalpy(
     isotherms: "list[PointIsotherm | ModelIsotherm]",
     loading_points: list = None,
     branch: str = 'ads',
     verbose: bool = False,
 ):
     r"""
-    Calculate the isosteric enthalpy of adsorption using several isotherms
-    recorded at different temperatures on the same material and the
-    Clausius-Clapeyron equation.
+
+    Calculate the isosteric enthalpy of adsorption (in kJ/mol) by applying
+    Clausius-Clapeyron equation to several isotherms recorded at different
+    temperatures on the same material.
 
     Parameters
     ----------
     isotherms : list[PointIsotherms | ModelIsotherm]
         The isotherms to use in calculation of the isosteric enthalpy. They should all
         be measured on the same material.
     loading_points : list[float], optional
@@ -36,15 +37,15 @@
         Whether to print out extra information and generate a graph.
 
     Returns
     -------
     result_dict : dict
         A dictionary with the isosteric enthalpies per loading, with the form:
 
-        - ``isosteric_enthalpy`` (array) : the isosteric enthalpy of adsorption in kj/mmol
+        - ``isosteric_enthalpy`` (array) : the isosteric enthalpy of adsorption in kJ/mol
         - ``loading`` (array) : the loading for each point of the isosteric enthalpy, in mmol
         - ``slopes`` (array) : the exact log(p) vs 1/T slope for each point
         - ``correlation`` (array) : correlation coefficient for each point
         - ``std_errors`` (array) : estimated standard errors for each point
 
     Raises
     ------
```

### Comparing `pygaps-4.4.2/src/pygaps/characterisation/models_hk.py` & `pygaps-4.5.0/src/pygaps/characterisation/models_hk.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/characterisation/models_kelvin.py` & `pygaps-4.5.0/src/pygaps/characterisation/models_kelvin.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/characterisation/models_thickness.py` & `pygaps-4.5.0/src/pygaps/characterisation/models_thickness.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/characterisation/psd_kernel.py` & `pygaps-4.5.0/src/pygaps/characterisation/psd_kernel.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,21 +361,22 @@
     if path in _LOADED:
         return _LOADED[path]
 
     with open(path, encoding="utf8") as fp:
         raw_kernel = pandas.read_csv(fp, index_col=0)
 
     # add a 0 in the dataframe for interpolation between lowest values
-    raw_kernel = raw_kernel.append(
+    raw_kernel = pandas.concat([
         pandas.DataFrame(
-            [0 for col in raw_kernel.columns],
-            index=raw_kernel.columns,
-            columns=[0],
-        ).transpose()
-    )
+            [[0 for col in raw_kernel.columns]],
+            index=[0],
+            columns=raw_kernel.columns,
+        ),
+        raw_kernel,
+    ])
 
     kernel = {}
     for pore_size in raw_kernel:
         interpolator = interpolate.interp1d(
             raw_kernel[pore_size].index, raw_kernel[pore_size].values, kind='cubic'
         )
```

### Comparing `pygaps-4.4.2/src/pygaps/characterisation/psd_meso.py` & `pygaps-4.5.0/src/pygaps/characterisation/psd_meso.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/characterisation/psd_micro.py` & `pygaps-4.5.0/src/pygaps/characterisation/psd_micro.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/characterisation/t_plots.py` & `pygaps-4.5.0/src/pygaps/characterisation/t_plots.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/cli/cli.py` & `pygaps-4.5.0/src/pygaps/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/core/adsorbate.py` & `pygaps-4.5.0/src/pygaps/core/adsorbate.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from pygaps.units.converter_unit import _PRESSURE_UNITS
 from pygaps.units.converter_unit import c_unit
 from pygaps.utilities.coolprop_utilities import CP
 from pygaps.utilities.coolprop_utilities import thermodynamic_backend
 from pygaps.utilities.exceptions import CalculationError
 from pygaps.utilities.exceptions import ParameterError
 
+# TODO: units in the prop dictionary and from coolprop do not always match (e.g. p_critical)
+
 
 class Adsorbate():
     """
     An unified class descriptor for an adsorbate.
 
     Its purpose is to expose properties such as adsorbate name,
     and formula, as well as physical properties, such as molar mass
@@ -38,28 +40,38 @@
         A chemical formula for the adsorbate in LaTeX form: He/N_{2}/C_{2}H_{4} etc.
     backend_name : str
         Used for integration with CoolProp/REFPROP. For a list of names
         look at the CoolProp `list of fluids
         <http://www.coolprop.org/fluid_properties/PurePseudoPure.html#list-of-fluids>`_
     molar_mass : float
         Custom value for molar mass (otherwise obtained through CoolProp).
+    p_triple : float
+        Custom value for triple point pressure (otherwise obtained through CoolProp).
+    t_triple : float
+        Custom value for triple point temperature (otherwise obtained through CoolProp).
+    p_critical : float
+        Custom value for critical point pressure (otherwise obtained through CoolProp).
+    t_critical : float
+        Custom value for critical point temperature (otherwise obtained through CoolProp).
     saturation_pressure : float
         Custom value for saturation pressure (otherwise obtained through CoolProp).
     surface_tension : float
         Custom value for surface tension (otherwise obtained through CoolProp).
     liquid_density : float
         Custom value for liquid density (otherwise obtained through CoolProp).
     liquid_molar_density : float
         Custom value for liquid molar density (otherwise obtained through CoolProp).
     gas_density : float
         Custom value for gas density (otherwise obtained through CoolProp).
     gas_molar_density : float
         Custom value for gas molar density (otherwise obtained through CoolProp).
+    enthalpy_vaporisation : float
+        Custom value for enthalpy of vaporisation/liquefaction (otherwise obtained through CoolProp).
     enthalpy_liquefaction : float
-        Custom value for enthalpy of liquefaction (otherwise obtained through CoolProp).
+        Custom value for enthalpy of vaporisation/liquefaction (otherwise obtained through CoolProp).
 
     Notes
     -----
     The members of the properties dictionary are left at the discretion of the
     user, to keep the class extensible. There are, however, some unique
     properties which are used by calculations in other modules listed in the
     other parameters section above.
@@ -321,21 +333,198 @@
                 _warn_reading_params(err)
                 return self.molar_mass(calculate=False)
         try:
             return self.get_prop("molar_mass")
         except ParameterError as err:
             _raise_calculation_error(err)
 
-    def pressure_saturation(self, temp, unit=None, calculate: bool = True) -> float:
-        """Alias for saturation_pressure"""
+    def p_triple(self, calculate: bool = True) -> float:
+        """
+        Return the triple point pressure, in Pa.
+
+        Parameters
+        ----------
+        calculate : bool, optional
+            Whether to calculate the property or look it up in the properties
+            dictionary, default - True.
+
+        Returns
+        -------
+        float
+            Triple point pressure in Pa.
+
+        Raises
+        ------
+        ``ParameterError``
+            If the calculation is not requested and the property does not exist
+            in the class dictionary.
+        ``CalculationError``
+            If it cannot be calculated, due to a physical reason.
+        """
+        if calculate:
+            try:
+                # For some reason coolprop does not implement a python
+                # wrapper for P_triple, so we are directly calling the propsSI function
+                # TODO: this will not work for REFPROP
+                return CP.CoolProp.PropsSI('PTRIPLE', self.backend_name)
+            except BaseException as err:
+                _warn_reading_params(err)
+                return self.p_triple(calculate=False)
+        try:
+            return self.get_prop("p_triple") * 1e5
+        except ParameterError as err:
+            _raise_calculation_error(err)
+
+    def t_triple(self, calculate: bool = True) -> float:
+        """
+        Return the triple point temperature, in K.
+
+        Parameters
+        ----------
+        calculate : bool, optional
+            Whether to calculate the property or look it up in the properties
+            dictionary, default - True.
+
+        Returns
+        -------
+        float
+            Triple point temperature in K.
+
+        Raises
+        ------
+        ``ParameterError``
+            If the calculation is not requested and the property does not exist
+            in the class dictionary.
+        ``CalculationError``
+            If it cannot be calculated, due to a physical reason.
+        """
+        if calculate:
+            try:
+                return self.backend.Ttriple()
+            except BaseException as err:
+                _warn_reading_params(err)
+                return self.t_triple(calculate=False)
+        try:
+            return self.get_prop("t_triple")
+        except ParameterError as err:
+            _raise_calculation_error(err)
+
+    def p_critical(self, calculate: bool = True) -> float:
+        """
+        Return the critical point pressure, in Pa.
+
+        Parameters
+        ----------
+        calculate : bool, optional
+            Whether to calculate the property or look it up in the properties
+            dictionary, default - True.
+
+        Returns
+        -------
+        float
+            Critical point pressure in Pa.
+
+        Raises
+        ------
+        ``ParameterError``
+            If the calculation is not requested and the property does not exist
+            in the class dictionary.
+        ``CalculationError``
+            If it cannot be calculated, due to a physical reason.
+        """
+        if calculate:
+            try:
+                return self.backend.p_critical()
+            except BaseException as err:
+                _warn_reading_params(err)
+                return self.p_critical(calculate=False)
+        try:
+            return self.get_prop("p_critical") * 1e5
+        except ParameterError as err:
+            _raise_calculation_error(err)
+
+    def t_critical(self, calculate: bool = True) -> float:
+        """
+        Return the critical point temperature, in K.
+
+        Parameters
+        ----------
+        calculate : bool, optional
+            Whether to calculate the property or look it up in the properties
+            dictionary, default - True.
+
+        Returns
+        -------
+        float
+            Critical point temperature in K.
+
+        Raises
+        ------
+        ``ParameterError``
+            If the calculation is not requested and the property does not exist
+            in the class dictionary.
+        ``CalculationError``
+            If it cannot be calculated, due to a physical reason.
+        """
+        if calculate:
+            try:
+                return self.backend.T_critical()
+            except BaseException as err:
+                _warn_reading_params(err)
+                return self.t_critical(calculate=False)
+        try:
+            return self.get_prop("t_critical")
+        except ParameterError as err:
+            _raise_calculation_error(err)
+
+    def pressure_saturation(
+        self,
+        temp: float,
+        unit: str = None,
+        calculate: bool = True,
+    ) -> float:
+        """
+        Get the saturation pressure at a particular temperature, in desired unit (default Pa).
+
+        Alias for 'saturation_pressure'
+
+        Parameters
+        ----------
+        temp : float
+            Temperature at which the pressure is desired in K.
+        unit : str
+            Unit in which to return the saturation pressure.
+            If not specifies defaults to Pascal.
+        calculate : bool, optional
+            Whether to calculate the property or look it up in the properties
+            dictionary, default - True.
+
+        Returns
+        -------
+        float
+            Pressure in unit requested.
+
+        Raises
+        ------
+        ``ParameterError``
+            If the calculation is not requested and the property does not exist
+            in the class dictionary.
+        ``CalculationError``
+            If it cannot be calculated, due to a physical reason.
+        """
         return self.saturation_pressure(temp, unit, calculate)
 
-    def saturation_pressure(self, temp, unit=None, calculate: bool = True) -> float:
+    def saturation_pressure(
+        self,
+        temp: float,
+        unit: str = None,
+        calculate: bool = True,
+    ) -> float:
         """
-        Get the saturation pressure at a particular temperature.
+        Get the saturation pressure at a particular temperature, in desired unit (default Pa).
 
         Parameters
         ----------
         temp : float
             Temperature at which the pressure is desired in K.
         unit : str
             Unit in which to return the saturation pressure.
@@ -372,17 +561,21 @@
             return sat_p
 
         try:
             return self.get_prop("saturation_pressure")
         except ParameterError as err:
             _raise_calculation_error(err)
 
-    def surface_tension(self, temp, calculate: bool = True) -> float:
+    def surface_tension(
+        self,
+        temp: float,
+        calculate: bool = True,
+    ) -> float:
         """
-        Get the surface tension at a particular temperature.
+        Get the surface tension at a particular temperature, in mN/m.
 
         Parameters
         ----------
         temp : float
             Temperature at which the surface_tension is desired in K.
         calculate : bool, optional
             Whether to calculate the property or look it up in the properties
@@ -413,17 +606,21 @@
                 return self.surface_tension(temp, calculate=False)
 
         try:
             return self.get_prop("surface_tension")
         except ParameterError as err:
             _raise_calculation_error(err)
 
-    def liquid_density(self, temp, calculate: bool = True) -> float:
+    def liquid_density(
+        self,
+        temp: float,
+        calculate: bool = True,
+    ) -> float:
         """
-        Get the liquid density at a particular temperature.
+        Get the liquid density at a particular temperature, in g/cm3.
 
         Parameters
         ----------
         temp : float
             Temperature at which the liquid density is desired in K.
         calculate : bool, optional.
             Whether to calculate the property or look it up in the properties
@@ -453,17 +650,21 @@
                 return self.liquid_density(temp, calculate=False)
 
         try:
             return self.get_prop("liquid_density")
         except ParameterError as err:
             _raise_calculation_error(err)
 
-    def liquid_molar_density(self, temp, calculate: bool = True) -> float:
+    def liquid_molar_density(
+        self,
+        temp: float,
+        calculate: bool = True,
+    ) -> float:
         """
-        Get the liquid molar density at a particular temperature.
+        Get the liquid molar density at a particular temperature, in mol/cm3.
 
         Parameters
         ----------
         temp : float
             Temperature at which the liquid density is desired in K.
         calculate : bool, optional.
             Whether to calculate the property or look it up in the properties
@@ -493,17 +694,21 @@
                 return self.liquid_molar_density(temp, calculate=False)
 
         try:
             return self.get_prop("liquid_molar_density")
         except ParameterError as err:
             _raise_calculation_error(err)
 
-    def gas_density(self, temp, calculate: bool = True) -> float:
+    def gas_density(
+        self,
+        temp: float,
+        calculate: bool = True,
+    ) -> float:
         """
-        Get the gas molar density at a particular temperature.
+        Get the gas molar density at a particular temperature, in g/cm3.
 
         Parameters
         ----------
         temp : float
             Temperature at which the gas density is desired in K.
         calculate : bool, optional.
             Whether to calculate the property or look it up in the properties
@@ -533,17 +738,21 @@
                 return self.gas_density(temp, calculate=False)
 
         try:
             return self.get_prop("gas_density")
         except ParameterError as err:
             _raise_calculation_error(err)
 
-    def gas_molar_density(self, temp, calculate: bool = True) -> float:
+    def gas_molar_density(
+        self,
+        temp: float,
+        calculate: bool = True,
+    ) -> float:
         """
-        Get the gas density at a particular temperature.
+        Get the gas density at a particular temperature, in mol/cm3.
 
         Parameters
         ----------
         temp : float
             Temperature at which the gas density is desired in K.
         calculate : bool, optional.
             Whether to calculate the property or look it up in the properties
@@ -573,17 +782,55 @@
                 return self.gas_molar_density(temp, calculate=False)
 
         try:
             return self.get_prop("gas_molar_density")
         except ParameterError as err:
             _raise_calculation_error(err)
 
-    def enthalpy_liquefaction(self, temp, calculate: bool = True) -> float:
+    def enthalpy_vaporisation(
+        self,
+        temp: float = None,
+        press: float = None,
+        calculate: bool = True,
+    ) -> float:
         """
-        Get the enthalpy of liquefaction at a particular temperature.
+        Get the enthalpy of vaporisation at a particular temperature, in kJ/mol.
+
+        Parameters
+        ----------
+        temp : float
+            Temperature at which the enthalpy of vaporisation is desired, in K.
+        calculate : bool, optional
+            Whether to calculate the property or look it up in the properties
+            dictionary, default - True.
+
+        Returns
+        -------
+        float
+            Enthalpy of vaporisation in kJ/mol.
+
+        Raises
+        ------
+        ``ParameterError``
+            If the calculation is not requested and the property does not exist
+            in the class dictionary.
+        ``CalculationError``
+            If it cannot be calculated, due to a physical reason.
+
+        """
+        return self.enthalpy_liquefaction(temp, press, calculate)
+
+    def enthalpy_liquefaction(
+        self,
+        temp: float = None,
+        press: float = None,
+        calculate: bool = True,
+    ) -> float:
+        """
+        Get the enthalpy of liquefaction at a particular temperature, in kJ/mol.
 
         Parameters
         ----------
         temp : float
             Temperature at which the enthalpy of liquefaction is desired, in K.
         calculate : bool, optional
             Whether to calculate the property or look it up in the properties
@@ -600,20 +847,32 @@
             If the calculation is not requested and the property does not exist
             in the class dictionary.
         ``CalculationError``
             If it cannot be calculated, due to a physical reason.
 
         """
         if calculate:
+            if temp and press:
+                raise CalculationError(
+                    "Can only specify one intensive variable, either temperature or pressure."
+                )
             try:
                 state = self.backend
-                state.update(CP.QT_INPUTS, 0.0, temp)
-                h_liq = state.hmolar()
-                state.update(CP.QT_INPUTS, 1.0, temp)
-                h_vap = state.hmolar()
+                if temp:
+                    state.update(CP.QT_INPUTS, 0.0, temp)
+                    h_liq = state.hmolar()
+                    state.update(CP.QT_INPUTS, 1.0, temp)
+                    h_vap = state.hmolar()
+                elif press:
+                    state.update(CP.PQ_INPUTS, press, 0.0)
+                    h_liq = state.hmolar()
+                    state.update(CP.PQ_INPUTS, press, 1.0)
+                    h_vap = state.hmolar()
+                else:
+                    raise CalculationError("Neither pressure nor temperature specified.")
                 return (h_vap - h_liq) / 1000
             except BaseException as err:
                 _warn_reading_params(err)
                 return self.enthalpy_liquefaction(temp, calculate=False)
 
         try:
             return self.get_prop("enthalpy_liquefaction")
```

### Comparing `pygaps-4.4.2/src/pygaps/core/baseisotherm.py` & `pygaps-4.5.0/src/pygaps/core/baseisotherm.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/core/material.py` & `pygaps-4.5.0/src/pygaps/core/material.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/core/modelisotherm.py` & `pygaps-4.5.0/src/pygaps/core/modelisotherm.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/core/pointisotherm.py` & `pygaps-4.5.0/src/pygaps/core/pointisotherm.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/data/__init__.py` & `pygaps-4.5.0/src/pygaps/data/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,18 +46,18 @@
 
 # TODO These methods actually WILL not work if there's a Zip file or
 # any other package
 # The reasoning is that we are using importlib_resources correctly, then
 # switching back to a path based approach with the dictionary.
 
 # Locations for fitting kernels
-_kernel_res = importlib_resources_files('pygaps.data.kernels')
+_kernel_res = importlib_resources_files('pygaps.data') / "kernels"
 KERNELS = {
     'DFT-N2-77K-carbon-slit': _kernel_res / 'DFT-N2-77K-carbon-slit.csv',
 }
 
 # Locations for standard isotherms
-_stdiso_res = importlib_resources_files('pygaps.data.stdiso')
+_stdiso_res = importlib_resources_files('pygaps.data') / "stdiso"
 STANDARD_ISOTHERMS = {
     "SiO2_JKO": _stdiso_res / "LiChrospher Si-1000 silica.csv",
     "CB_KJG": _stdiso_res / "Cabot BP280 carbon black.csv",
 }
```

### Comparing `pygaps-4.4.2/src/pygaps/data/adsorbate_props.json` & `pygaps-4.5.0/src/pygaps/data/adsorbate_props.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/data/adsorbates.json` & `pygaps-4.5.0/src/pygaps/data/adsorbates.json`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/data/default.db` & `pygaps-4.5.0/src/pygaps/data/default.db`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/data/kernels/DFT-N2-77K-carbon-slit.csv` & `pygaps-4.5.0/src/pygaps/data/kernels/DFT-N2-77K-carbon-slit.csv`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/data/stdiso/Cabot BP280 carbon black.csv` & `pygaps-4.5.0/src/pygaps/data/stdiso/Cabot BP280 carbon black.csv`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/data/stdiso/LiChrospher Si-1000 silica.csv` & `pygaps-4.5.0/src/pygaps/data/stdiso/LiChrospher Si-1000 silica.csv`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/graphing/calc_graphs.py` & `pygaps-4.5.0/src/pygaps/graphing/calc_graphs.py`

 * *Files 1% similar despite different names*

```diff
@@ -625,14 +625,17 @@
         own styling if desired.
 
     """
     # Generate the figure if needed
     if ax is None:
         _, ax = plt.subplots()
 
+    if exp != 2:
+        exp = 'n'
+
     with mpl.rc_context(POINTS_MUTED):
         ax.plot(
             log_n_p0p,
             logv,
             label='all points',
         )
     with mpl.rc_context(POINTS_HIGHLIGHTED):
@@ -645,16 +648,16 @@
         ax.plot(
             log_n_p0p,
             slope * log_n_p0p + intercept,
             color='black',
             label='model fit',
         )
 
-    ax.set_xlabel('log $p^0/p$')
-    ax.set_ylabel('log $V/V_0$')
+    ax.set_xlabel(fr'$ln^{exp}\ p^0/p$')
+    ax.set_ylabel(r'$ln\ V/V_0$')
     ax.legend()
 
     return ax
 
 
 @mpl.rc_context(BASE_STYLE)
 def virial_plot(
```

### Comparing `pygaps-4.4.2/src/pygaps/graphing/iast_graphs.py` & `pygaps-4.5.0/src/pygaps/graphing/iast_graphs.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/graphing/isotherm_graphs.py` & `pygaps-4.5.0/src/pygaps/graphing/isotherm_graphs.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/graphing/labels.py` & `pygaps-4.5.0/src/pygaps/graphing/labels.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/graphing/model_graphs.py` & `pygaps-4.5.0/src/pygaps/graphing/model_graphs.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/graphing/mpl_styles.py` & `pygaps-4.5.0/src/pygaps/graphing/mpl_styles.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,71 @@
 """Contains global style dictionaries for matplotlib to be applied."""
 
+import typing as t
+
 #: Markers used in plotting.
-ISO_MARKERS = ('o', 's', 'D', 'P', '*', '<', '>', 'X', 'v', '^')
+ISO_MARKERS: "tuple[str]" = ('o', 's', 'D', 'P', '*', '<', '>', 'X', 'v', '^')
 #: Colors used in main (y1) plotting.
-Y1_COLORS = ('#003f5c', '#58508d', '#bc5090', '#ff6361', '#ffa600')
+Y1_COLORS: "tuple[str]" = ('#003f5c', '#58508d', '#bc5090', '#ff6361', '#ffa600')
 #: Colors used in secondary (y2) plotting.
-Y2_COLORS = ("#0082bd", "#8674c5", "#d15d9e", "#ea5e59", "#ca8300")
+Y2_COLORS: "tuple[str]" = ("#0082bd", "#8674c5", "#d15d9e", "#ea5e59", "#ca8300")
 
 #: Style applied to ALL matplotlib figures in pygaps.
-BASE_STYLE = {
+BASE_STYLE: "dict[str, t.Any]" = {
     'legend.frameon': False,
 }
 
 #: Style applied to Isotherm figures.
-ISO_STYLE = {
+ISO_STYLE: "dict[str, t.Any]" = {
     'figure.figsize': (6, 6),
     'axes.titlesize': 20,
     'axes.titley': 1.01,
     'axes.labelsize': 15,
     'xtick.labelsize': 13,
     'ytick.labelsize': 13,
     'lines.linewidth': 1.5,
     'lines.markersize': 5,
     'legend.handlelength': 2,
     'legend.fontsize': 11,
     'image.aspect': 'equal'
 }
 
 #: Style component to generate "muted/unselected" points.
-POINTS_MUTED = {
+POINTS_MUTED: "dict[str, t.Any]" = {
     "lines.linestyle": 'none',
     "lines.marker": 'o',
     "lines.markerfacecolor": 'none',
     "lines.markeredgecolor": 'grey',
     "lines.markersize": 5,
     "lines.markeredgewidth": 1.5,
 }
 
 #: Style component to generate "highlighted/elected" points.
-POINTS_HIGHLIGHTED = {
+POINTS_HIGHLIGHTED: "dict[str, t.Any]" = {
     "lines.linestyle": 'none',
     "lines.marker": 'o',
     "lines.markeredgecolor": 'r',
     "lines.markerfacecolor": 'r',
     "lines.markersize": 5,
 }
 
 #: Style component to generate "single important" points.
-POINTS_IMPORTANT = {
+POINTS_IMPORTANT: "dict[str, t.Any]" = {
     "lines.linestyle": 'none',
     "lines.marker": 'X',
     "lines.markeredgecolor": 'k',
     "lines.markerfacecolor": 'k',
     "lines.markersize": 10,
 }
 
 #: Style component to generate a line fitted through points.
-LINE_FIT = {
+LINE_FIT: "dict[str, t.Any]" = {
     "lines.linestyle": '--',
     "lines.marker": '',
 }
 
 #: Style component to apply to error bars.
-LINE_ERROR = {
+LINE_ERROR: "dict[str, t.Any]" = {
     "lines.linestyle": '--',
     "lines.marker": 'o',
     "lines.markersize": 3,
 }
```

### Comparing `pygaps-4.4.2/src/pygaps/iast/pgiast.py` & `pygaps-4.5.0/src/pygaps/iast/pgiast.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/modelling/__init__.py` & `pygaps-4.5.0/src/pygaps/modelling/__init__.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/modelling/base_model.py` & `pygaps-4.5.0/src/pygaps/modelling/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,18 +232,18 @@
 
         param_names = list(self.params)
         guess = numpy.array([param_guess[p] for p in param_names])
         bounds = [[self.param_bounds[p][0] for p in param_names],
                   [self.param_bounds[p][1] for p in param_names]]
 
         if self.calculates == "loading":
-            fit_func_base = lambda p, l: self.loading(p) - l
+            fit_func_base = lambda pr, ld: self.loading(pr) - ld
             model_range = self.loading_range[1] - self.loading_range[0]
         elif self.calculates == "pressure":
-            fit_func_base = lambda p, l: self.pressure(l) - p
+            fit_func_base = lambda pr, ld: self.pressure(ld) - pr
             model_range = self.pressure_range[1] - self.pressure_range[0]
 
         def fit_func(x, pressure, loading):
             for i, _ in enumerate(param_names):
                 self.params[param_names[i]] = x[i]
             return fit_func_base(pressure, loading)
```

### Comparing `pygaps-4.4.2/src/pygaps/modelling/bet.py` & `pygaps-4.5.0/src/pygaps/modelling/bet.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/modelling/da.py` & `pygaps-4.5.0/src/pygaps/modelling/da.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/modelling/dr.py` & `pygaps-4.5.0/src/pygaps/modelling/dr.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/modelling/dslangmuir.py` & `pygaps-4.5.0/src/pygaps/modelling/dslangmuir.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/modelling/fhvst.py` & `pygaps-4.5.0/src/pygaps/modelling/fhvst.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/modelling/freundlich.py` & `pygaps-4.5.0/src/pygaps/modelling/freundlich.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/modelling/gab.py` & `pygaps-4.5.0/src/pygaps/modelling/gab.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/modelling/henry.py` & `pygaps-4.5.0/src/pygaps/modelling/henry.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/modelling/jensenseaton.py` & `pygaps-4.5.0/src/pygaps/modelling/jensenseaton.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/modelling/langmuir.py` & `pygaps-4.5.0/src/pygaps/modelling/langmuir.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/modelling/quadratic.py` & `pygaps-4.5.0/src/pygaps/modelling/quadratic.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,18 @@
     is convex at low pressures but changes concavity as it saturates, yielding
     an S-shape. The S-shape can be explained by adsorbate-adsorbate attractive
     forces; the initial convexity is due to a cooperative
     effect of adsorbate-adsorbate attractions aiding in the recruitment of
     additional adsorbate molecules [#]_.
 
     The parameter :math:`K_a` can be interpreted as the Langmuir constant; the
-    strength of the adsorbate-adsorbate attractive forces is embedded in :math:`K_b`.
-    It is often useful in systems where the
-    energy of guest-guest interactions is actually higher than
-    the energy of adsorption, such as when adsorbing water
-    on a hydrophobic surface.
+    strength of the adsorbate-adsorbate attractive forces is embedded in
+    :math:`K_b`. It is often useful in systems where the energy of guest-guest
+    interactions is actually higher than the energy of adsorption, such as when
+    adsorbing water on a hydrophobic surface.
 
     References
     ----------
     .. [#]  T. L. Hill, An introduction to statistical thermodynamics, Dover
        Publications, 1986.
 
     """
```

### Comparing `pygaps-4.4.2/src/pygaps/modelling/temkinapprox.py` & `pygaps-4.5.0/src/pygaps/modelling/temkinapprox.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/modelling/toth.py` & `pygaps-4.5.0/src/pygaps/modelling/toth.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/modelling/tslangmuir.py` & `pygaps-4.5.0/src/pygaps/modelling/tslangmuir.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/modelling/virial.py` & `pygaps-4.5.0/src/pygaps/modelling/virial.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/modelling/wvst.py` & `pygaps-4.5.0/src/pygaps/modelling/wvst.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/parsing/__init__.py` & `pygaps-4.5.0/src/pygaps/parsing/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,19 @@
 
     meta, data = read(path, manufacturer, fmt, **options)
     data = pandas.DataFrame(data)
 
     meta['loading_key'] = 'loading'
     meta['pressure_key'] = 'pressure'
 
+    # Quantachrome files are parsed in cc, must convert per unit mass
+    if manufacturer == 'qnt' and fmt == 'txt-raw':
+        mass = meta['material_mass']
+        data['loading'] = [ld / mass for ld in data['loading']]
+
     # TODO pyGAPS does not yet handle saturation pressure recorded at each point
     # Therefore, we use the relative pressure column as our true pressure,
     # ignoring the absolute pressure column
     if 'pressure_relative' in data.columns:
         data['pressure'] = data['pressure_relative']
         data = data.drop('pressure_relative', axis=1)
         meta['pressure_mode'] = 'relative'
```

### Comparing `pygaps-4.4.2/src/pygaps/parsing/aif.py` & `pygaps-4.5.0/src/pygaps/parsing/aif.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,26 +22,26 @@
 from pygaps.core.modelisotherm import ModelIsotherm
 from pygaps.core.pointisotherm import PointIsotherm
 from pygaps.modelling import model_from_dict
 from pygaps.parsing import _PARSER_PRECISION
 from pygaps.utilities.exceptions import ParsingError
 from pygaps.utilities.string_utilities import cast_string
 
-_parser_version = "1.0"
+_parser_version = "d546195"
 
 _META_DICT = {
     '_exptl_temperature': {
         'text': 'temperature',
         'type': float
     },
     '_exptl_adsorptive': {
         'text': 'adsorbate',
         'type': str
     },
-    '_sample_material_id': {
+    '_adsnt_material_id': {
         'text': 'material',
         'type': str
     },
     '_exptl_operator': {
         'text': 'user',
         'type': str
     },
@@ -49,27 +49,27 @@
         'text': 'date',
         'type': str
     },
     '_exptl_instrument': {
         'text': 'instrument',
         'type': str
     },
-    '_exptl_sample_mass': {
+    '_adsnt_sample_mass': {
         'text': 'material_mass',
         'type': float
     },
     '_units_mass': {
         'text': 'material_mass_unit',
         'type': str
     },
-    '_exptl_activation_temperature': {
+    '_adsnt_degas_temperature': {
         'text': 'activation_temperature',
         'type': float
     },
-    '_sample_id': {
+    '_adsnt_sample_id': {
         'text': 'material_batch',
         'type': str
     },
 }
 _DATA_DICT = {
     'pressure': 'pressure',
     'p0': 'pressure_saturation',
@@ -78,14 +78,34 @@
 }
 _UNITS_DICT = [
     "_units_pressure",
     "_units_loading",
     "_units_mass",
     "_units_temperature",
 ]
+# This dictionary contains old keys that are no longer used
+# but are still present in some AIF files
+_META_DICT_OLD = {
+    '_sample_material_id': {
+        'text': 'material',
+        'type': str
+    },
+    '_exptl_sample_mass': {
+        'text': 'material_mass',
+        'type': float
+    },
+    '_exptl_activation_temperature': {
+        'text': 'activation_temperature',
+        'type': float
+    },
+    '_sample_id': {
+        'text': 'material_batch',
+        'type': str
+    },
+}
 
 
 def isotherm_to_aif(isotherm: PointIsotherm, path: str = None):
     """
     Convert isotherm into an AIF representation [#]_.
 
     If the path is specified, the isotherm is saved as a file,
@@ -128,15 +148,15 @@
     # write metadata
     block.set_pair('_audit_aif_version', _parser_version)
     block.set_pair('_audit_creation_method', 'pyGAPS')
 
     # required pygaps data
     block.set_pair('_exptl_adsorptive', f"\'{iso_dict.pop('adsorbate')}\'")
     block.set_pair('_exptl_temperature', f"{iso_dict.pop('temperature')}")
-    block.set_pair('_sample_material_id', f"\'{iso_dict.pop('material')}\'")
+    block.set_pair('_adsnt_material_id', f"\'{iso_dict.pop('material')}\'")
 
     # other possible specs
     for key, val in _META_DICT.items():
         if val['text'] in iso_dict:
             block.set_pair(key, f"\'{iso_dict.pop(val['text'])}\'")
 
     # units
@@ -234,20 +254,24 @@
                 "The `path/string` is invalid or does not exist. "
             ) from ex
 
     block = aif.sole_block()
     raw_dict = {}
 
     # read version
-    version = block.find_value('_audit_aif_version').strip("'")
-    if not version or float(version.strip("'")) < float(_parser_version):
+    version = block.find_value('_audit_aif_version')
+    try_other_version = False
+    if not version or version.strip("'") != (_parser_version):
         logger.warning(
             f"The file version is {version} while the parser uses version {_parser_version}. "
             "Strange things might happen, so double check your data."
         )
+        try_other_version = True
+    else:
+        version = version.strip("'")
 
     # creation method (excluded if created in pygaps)
     cmethod = block.find_value('_audit_creation_method')
     if cmethod and cmethod.strip("'") != "pyGAPS":
         raw_dict["_audit_creation_method"] = cmethod.strip("'")
 
     # read data and metadata through sequential iteration
@@ -260,18 +284,29 @@
     for item in block:
         # metadata handling
         if item.pair is not None:
             key, val = item.pair
             val = val.strip("'")
 
             if key in _META_DICT:
-                raw_dict[_META_DICT[key]['text']] = _META_DICT[key]['type'](val)
+                try:
+                    raw_dict[_META_DICT[key]['text']] = _META_DICT[key]['type'](val)
+                except ValueError:
+                    logger.warning(
+                        f"""Could not parse parameter {_META_DICT[key]['text']}, currently {val}"""
+                    )
             elif key.startswith('_pygaps_'):
                 raw_dict[key[8:]] = cast_string(val)
             elif key not in excluded:
+                if try_other_version:
+                    if key in _META_DICT_OLD:
+                        try:
+                            raw_dict[_META_DICT_OLD[key]['text']] = _META_DICT_OLD[key]['type'](val)
+                        except ValueError:
+                            pass
                 raw_dict[key] = cast_string(val)
 
         # data handling
         elif item.loop is not None:
             loop = item.loop
             loop_data = block.find(loop.tags)
```

### Comparing `pygaps-4.4.2/src/pygaps/parsing/csv.py` & `pygaps-4.5.0/src/pygaps/parsing/csv.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/parsing/excel.py` & `pygaps-4.5.0/src/pygaps/parsing/excel.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,14 +136,18 @@
 
         # We get data and replace adsorption terminology
         data = isotherm.data_raw.copy()
         data['branch'] = data['branch'].replace(0, 'ads').replace(1, 'des')
 
         columns = [isotherm.pressure_key, isotherm.loading_key, 'branch'] + isotherm.other_keys
 
+        # Write data types
+        for col_index, heading in enumerate(isotherm.other_keys):
+            sht.write(data_row - 1, col_index + 3, data[heading].dtype.name)
+
         # Write all data
         for col_index, heading in enumerate(columns):
             sht.write(data_row, col_index, heading)
             for row_index, datapoint in enumerate(data[heading]):
                 sht.write(data_row + row_index + 1, col_index, datapoint)
 
     elif isinstance(isotherm, ModelIsotherm):
@@ -244,25 +248,34 @@
             if point == '':
                 break
             final_row += 1
 
         # read the data in
         header_col = 0
         headers = []
+        dtypes = {}
         experiment_data = {}
         while header_col < sht.ncols:
             header = sht.cell(header_row, header_col).value
             if header == '':
                 break
+            # read header, data, and dtype
             headers.append(header)
             experiment_data[header] = [
                 sht.cell(i, header_col).value for i in range(start_row, final_row)
             ]
+            # read the data type
+            # only read the data type if it is not a pressure, loading or branch
+            if header_col > 2:
+                dtype = sht.cell(header_row - 1, header_col).value
+                if dtype != '':
+                    dtypes[header] = dtype
             header_col += 1
-        data = pandas.DataFrame(experiment_data).convert_dtypes()
+        data = pandas.DataFrame(experiment_data)
+        data = data.astype(dtypes)
 
         raw_dict['pressure_key'] = headers[0]
         raw_dict['loading_key'] = headers[1]
 
         # process isotherm branches if they exist
         if 'branch' in data.columns:
             data['branch'] = data['branch'].apply(lambda x: 0 if x == 'ads' else 1)
```

### Comparing `pygaps-4.4.2/src/pygaps/parsing/isodb.py` & `pygaps-4.5.0/src/pygaps/parsing/isodb.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Interaction with the NIST ISODB."""
 
 from pygaps import logger
 from pygaps.parsing.json import isotherm_from_json
+from pygaps.utilities.exceptions import ParsingError
 
 _ISODB_API = "https://adsorption.nist.gov/isodb/api"
 
 
 def isotherm_from_isodb(filename):
     """
     Load an isotherm from the NIST ISODB.
@@ -32,8 +33,13 @@
         logger.warning('Connection timeout')
         return None
 
     except requests.exceptions.ConnectionError:
         logger.warning('Connection error')
         return None
 
-    return isotherm_from_json(resp.text, fmt="NIST")
+    try:
+        return isotherm_from_json(resp.text, fmt="NIST")
+
+    except ParsingError:
+        logger.warning('Could not parse isotherm. Check if the service is up.')
+        return None
```

### Comparing `pygaps-4.4.2/src/pygaps/parsing/json.py` & `pygaps-4.5.0/src/pygaps/parsing/json.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/parsing/sqlite.py` & `pygaps-4.5.0/src/pygaps/parsing/sqlite.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/units/converter_mode.py` & `pygaps-4.5.0/src/pygaps/units/converter_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,15 @@
                 sign = -1
 
         return (
             value * _LOADING_MODE[_basis_from][_unit_from] * factor * constant**sign /
             _LOADING_MODE[_basis_to][_unit_to]
         )
 
-    elif unit_to and unit_from != unit_to:
+    if unit_to and unit_from != unit_to:
         return c_unit(_LOADING_MODE[basis_from], value, unit_from, unit_to)
 
     return value
 
 
 def c_material(
     value: float,
@@ -328,16 +328,17 @@
     """
     _check_basis(basis_from, _MATERIAL_MODE, 'material')
     _check_basis(basis_to, _MATERIAL_MODE, 'material')
 
     if basis_from != basis_to:
 
         if (basis_from in ['percent', 'fraction'] or basis_to in ['percent', 'fraction']):
-            ParameterError(
-                "If you want to convert to/from fraction/percent, convert using loading, not adsorbate."
+            raise ParameterError(
+                "If you want to convert to/from fraction/percent,"
+                " convert using loading, not adsorbate."
             )
 
         _check_unit(unit_to, _MATERIAL_MODE[basis_to], 'material')
         _check_unit(unit_from, _MATERIAL_MODE[basis_from], 'material')
 
         constant = 1
         sign = 1
@@ -365,15 +366,15 @@
                 sign = -1
 
         return (
             value / _MATERIAL_MODE[basis_from][unit_from] / constant**sign *
             _MATERIAL_MODE[basis_to][unit_to]
         )
 
-    elif unit_to and unit_from != unit_to:
+    if unit_to and unit_from != unit_to:
         return c_unit(_MATERIAL_MODE[basis_from], value, unit_from, unit_to, sign=-1)
 
     return value
 
 
 def c_temperature(
     value: float,
```

### Comparing `pygaps-4.4.2/src/pygaps/units/converter_unit.py` & `pygaps-4.5.0/src/pygaps/units/converter_unit.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/utilities/coolprop_utilities.py` & `pygaps-4.5.0/src/pygaps/utilities/coolprop_utilities.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/utilities/hashgen.py` & `pygaps-4.5.0/src/pygaps/utilities/hashgen.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/utilities/isotherm_interpolator.py` & `pygaps-4.5.0/src/pygaps/utilities/isotherm_interpolator.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,45 +26,49 @@
         Determine which kind of interpolation is done between the
         datapoints.
     interp_fill : str, optional
         The parameter passed to the scipy.interpolate.interp1d function
         to determine what to do outside data bounds.
 
     """
-
     def __init__(
         self,
         known_data,
         interp_data,
         interp_branch='ads',
         interp_kind='linear',
         interp_fill=None,
     ):
-        """Instantiate."""
+        # Instantiate
         # The branch the internal interpolator is on.
         self.interp_branch = interp_branch
         # The kind of interpolator in the internal interpolator.
         self.interp_kind = interp_kind
         # Value of loading to assume beyond highest pressure in the data.
         self.interp_fill = interp_fill
 
         # The actual interpolator. This is generated
         # the first time it is needed to make calculations faster.
         if known_data is None:
             return
 
+        # Create the interpolator
         if interp_fill is None:
             self.interp_fun = interp1d(
-                known_data, interp_data, kind=interp_kind
+                known_data,
+                interp_data,
+                kind=interp_kind,
             )
+        # If we want to extrapolate, we need to use a different
+        # interpolator.
         else:
             self.interp_fun = interp1d(
                 known_data,
                 interp_data,
                 kind=interp_kind,
                 fill_value=interp_fill,
                 bounds_error=False
             )
 
     def __call__(self, data):
-        """Override direct call."""
+        """Override direct call to return interpolated data."""
         return self.interp_fun(data)
```

### Comparing `pygaps-4.4.2/src/pygaps/utilities/math_utilities.py` & `pygaps-4.5.0/src/pygaps/utilities/math_utilities.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/utilities/pygaps_utilities.py` & `pygaps-4.5.0/src/pygaps/utilities/pygaps_utilities.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/utilities/python_utilities.py` & `pygaps-4.5.0/src/pygaps/utilities/python_utilities.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/utilities/sqlite_db_creator.py` & `pygaps-4.5.0/src/pygaps/utilities/sqlite_db_creator.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,24 +20,31 @@
         Print out extra information.
 
     """
     for pragma in PRAGMAS:
         db_execute_general(pragma, path, verbose=verbose)
 
     # Get json files
-    import importlib.resources as importlib_resources
+    try:
+        from importlib.resources import files as ir_files
+    except ImportError:
+        # TODO Deprecation after PY<3.9
+        # Use backported `importlib_resources`.
+        from importlib_resources import files as ir_files
 
     # Get and upload adsorbate property types
-    ads_props_json = importlib_resources.read_text('pygaps.data', 'adsorbate_props.json')
+    ads_props_json = ir_files('pygaps.data').joinpath('adsorbate_props.json').read_text(
+        encoding='utf8'
+    )
     ads_props = json.loads(ads_props_json)
     for ap_type in ads_props:
         pgp_sqlite.adsorbate_property_type_to_db(ap_type, db_path=path, verbose=verbose)
 
     # Get and upload adsorbates
-    ads_json = importlib_resources.read_text('pygaps.data', 'adsorbates.json')
+    ads_json = ir_files('pygaps.data').joinpath('adsorbates.json').read_text(encoding='utf8')
     adsorbates = json.loads(ads_json)
     for ads in adsorbates:
         pgp_sqlite.adsorbate_to_db(pygaps.Adsorbate(**ads), db_path=path, verbose=verbose)
 
     # Upload standard isotherm types
     pgp_sqlite.isotherm_type_to_db({'type': 'isotherm'}, db_path=path)
     pgp_sqlite.isotherm_type_to_db({'type': 'pointisotherm'}, db_path=path)
```

### Comparing `pygaps-4.4.2/src/pygaps/utilities/sqlite_db_pragmas.py` & `pygaps-4.5.0/src/pygaps/utilities/sqlite_db_pragmas.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/utilities/sqlite_utilities.py` & `pygaps-4.5.0/src/pygaps/utilities/sqlite_utilities.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps/utilities/string_utilities.py` & `pygaps-4.5.0/src/pygaps/utilities/string_utilities.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/src/pygaps.egg-info/PKG-INFO` & `pygaps-4.5.0/src/pygaps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygaps
-Version: 4.4.2
+Version: 4.5.0
 Summary: A framework for processing adsorption data for porous materials.
 Home-page: https://github.com/pauliacomi/pygaps
 Author: Paul Iacomi
 Author-email: mail@pauliacomi.com
 License: MIT license
 Project-URL: Documentation, https://pygaps.readthedocs.io
 Project-URL: Source Code, https://github.com/pauliacomi/pygaps
```

### Comparing `pygaps-4.4.2/src/pygaps.egg-info/SOURCES.txt` & `pygaps-4.5.0/src/pygaps.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,21 +40,21 @@
 docs/_templates/layout.html
 docs/examples/__init__.py
 docs/examples/alphas.ipynb
 docs/examples/area_calcs.ipynb
 docs/examples/characterisation.rst
 docs/examples/database.ipynb
 docs/examples/dr_da_plots.ipynb
+docs/examples/enthalpy_sorption.ipynb
 docs/examples/iast.ipynb
 docs/examples/import.ipynb
 docs/examples/index.rst
 docs/examples/initial_enthalpy.ipynb
 docs/examples/initial_henryc.ipynb
 docs/examples/inspection.ipynb
-docs/examples/isosteric_enthalpy.ipynb
 docs/examples/modelling.ipynb
 docs/examples/novel.png
 docs/examples/parsing.ipynb
 docs/examples/plotting.ipynb
 docs/examples/psd.ipynb
 docs/examples/quickstart.ipynb
 docs/examples/test.png
@@ -96,14 +96,15 @@
 docs/examples/data/parsing/json/AC BAX1500 butane 298.json
 docs/examples/data/parsing/json/DUT-8 EtOH 298.json
 docs/examples/data/parsing/json/HKUST-1(Cu) CO2 303.json
 docs/examples/data/parsing/json/MCM-41 N2 77.json
 docs/examples/data/parsing/json/SURF N2 77.json
 docs/examples/data/parsing/json/UiO-66(Zr) N2 77.json
 docs/examples/data/parsing/nist/nist_iso.json
+docs/examples/data/whittaker/whittaker_iso_1.aiff
 docs/figures/SMS-Logo.jpg
 docs/figures/db_schema.png
 docs/figures/svp_graph.png
 docs/figures/vle_graph.png
 docs/files/isotherm.aif
 docs/files/isotherm.csv
 docs/files/isotherm.json
@@ -130,17 +131,16 @@
 docs/reference/plotting.rst
 docs/reference/units.rst
 docs/reference/utilities.rst
 docs/reference/characterisation/alphas_plot.rst
 docs/reference/characterisation/area_bet.rst
 docs/reference/characterisation/area_lang.rst
 docs/reference/characterisation/dubinin.rst
-docs/reference/characterisation/initial_enth.rst
+docs/reference/characterisation/enthalpy_sorption.rst
 docs/reference/characterisation/initial_hk.rst
-docs/reference/characterisation/isosteric_enth.rst
 docs/reference/characterisation/psd_kernel.rst
 docs/reference/characterisation/psd_meso.rst
 docs/reference/characterisation/psd_micro.rst
 docs/reference/characterisation/t_plot.rst
 docs/reference/characterisation/thickness_models.rst
 docs/reference/core/adsorbate.rst
 docs/reference/core/isotherms.rst
@@ -156,14 +156,15 @@
 src/pygaps.egg-info/top_level.txt
 src/pygaps.egg-info/zip-safe
 src/pygaps/characterisation/__init__.py
 src/pygaps/characterisation/alphas_plots.py
 src/pygaps/characterisation/area_bet.py
 src/pygaps/characterisation/area_lang.py
 src/pygaps/characterisation/dr_da_plots.py
+src/pygaps/characterisation/enth_sorp_whittaker.py
 src/pygaps/characterisation/initial_enth.py
 src/pygaps/characterisation/initial_henry.py
 src/pygaps/characterisation/isosteric_enth.py
 src/pygaps/characterisation/models_hk.py
 src/pygaps/characterisation/models_kelvin.py
 src/pygaps/characterisation/models_thickness.py
 src/pygaps/characterisation/psd_kernel.py
@@ -179,18 +180,16 @@
 src/pygaps/core/modelisotherm.py
 src/pygaps/core/pointisotherm.py
 src/pygaps/data/__init__.py
 src/pygaps/data/adsorbate_props.json
 src/pygaps/data/adsorbates.json
 src/pygaps/data/default.db
 src/pygaps/data/kernels/DFT-N2-77K-carbon-slit.csv
-src/pygaps/data/kernels/__init__.py
 src/pygaps/data/stdiso/Cabot BP280 carbon black.csv
 src/pygaps/data/stdiso/LiChrospher Si-1000 silica.csv
-src/pygaps/data/stdiso/__init__.py
 src/pygaps/graphing/__init__.py
 src/pygaps/graphing/calc_graphs.py
 src/pygaps/graphing/iast_graphs.py
 src/pygaps/graphing/isotherm_graphs.py
 src/pygaps/graphing/labels.py
 src/pygaps/graphing/model_graphs.py
 src/pygaps/graphing/mpl_styles.py
@@ -234,23 +233,25 @@
 src/pygaps/utilities/python_utilities.py
 src/pygaps/utilities/sqlite_db_creator.py
 src/pygaps/utilities/sqlite_db_pragmas.py
 src/pygaps/utilities/sqlite_utilities.py
 src/pygaps/utilities/string_utilities.py
 tests/__init__.py
 tests/conftest.py
+tests/test_utils.py
 tests/characterisation/__init__.py
 tests/characterisation/conftest.py
 tests/characterisation/test_alphas_plots.py
 tests/characterisation/test_area_bet.py
 tests/characterisation/test_area_langmuir.py
 tests/characterisation/test_dr_da_plots.py
+tests/characterisation/test_enth_sorp_clausclap.py
+tests/characterisation/test_enth_sorp_whittaker.py
 tests/characterisation/test_initial_enthalpy.py
 tests/characterisation/test_initial_henry.py
-tests/characterisation/test_isosteric_enthalpy.py
 tests/characterisation/test_models_hk.py
 tests/characterisation/test_models_kelvin.py
 tests/characterisation/test_models_thickness.py
 tests/characterisation/test_psd_kernel.py
 tests/characterisation/test_psd_meso.py
 tests/characterisation/test_psd_micro.py
 tests/characterisation/test_t_plots.py
```

### Comparing `pygaps-4.4.2/tests/characterisation/conftest.py` & `pygaps-4.5.0/tests/characterisation/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 """
 
 from pathlib import Path
 
 DATA_PATH = Path(__file__).parent.parent.parent / 'docs' / 'examples' / 'data'
 DATA_N77_PATH = DATA_PATH / 'characterisation'
 DATA_ISOSTERIC_PATH = DATA_PATH / 'isosteric'
+DATA_WHITTAKER_PATH = DATA_PATH / 'whittaker'
 DATA_CALO_PATH = DATA_PATH / 'calorimetry'
 
 DATA = {
     'MCM-41': {
         'file': 'MCM-41 N2 77.355.json',
         'bet_area': 350.0,
         'bet_area_s': 350.0,
@@ -122,7 +123,14 @@
         'ienth': 27,
     },
     'Takeda 5A': {
         'file': 'Takeda 5A Test CO2.json',
         'ienth': 35,
     },
 }
+
+DATA_WHITTAKER = {
+    'example1': {
+        'file': 'whittaker_iso_1.aiff',
+        'ref_enth': 16.08745,
+    }
+}
```

### Comparing `pygaps-4.4.2/tests/characterisation/test_alphas_plots.py` & `pygaps-4.5.0/tests/characterisation/test_alphas_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 
 Functions are tested against pre-calculated values on real isotherms.
 All pre-calculated data for characterisation can be found in the
 /.conftest file together with the other isotherm parameters.
 """
 
 import pytest
-from matplotlib.testing.decorators import cleanup
 from numpy import isclose
 
 import pygaps
 import pygaps.characterisation.alphas_plots as als
 import pygaps.parsing.json as pgpj
 import pygaps.utilities.exceptions as pgEx
 
+from ..test_utils import mpl_cleanup
 from .conftest import DATA
 from .conftest import DATA_N77_PATH
 
 
 @pytest.mark.characterisation
 class TestAlphaSPlot():
     """Test alpha-s calculation."""
@@ -101,14 +101,14 @@
         err_absolute_volume = 0.01  # units
 
         assert isclose(results[-1].get('adsorbed_volume'), 0, err_relative, err_absolute_area)
         assert isclose(
             results[-1].get('area'), sample['s_as_area'], err_relative, err_absolute_volume
         )
 
-    @cleanup
+    @mpl_cleanup
     def test_alphas_output(self):
         """Test verbosity."""
         sample = DATA['MCM-41']
         filepath = DATA_N77_PATH / sample['file']
         isotherm = pgpj.isotherm_from_json(filepath)
         als.alpha_s(isotherm, isotherm, verbose=True)
```

### Comparing `pygaps-4.4.2/tests/characterisation/test_area_bet.py` & `pygaps-4.5.0/tests/characterisation/test_area_bet.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 Functions are tested against pre-calculated values on real isotherms.
 All pre-calculated data for characterisation can be found in the
 /.conftest file together with the other isotherm parameters.
 """
 import logging
 
 import pytest
-from matplotlib.testing.decorators import cleanup
 from numpy import isclose
 from numpy import linspace
 
 import pygaps.characterisation.area_bet as ab
 import pygaps.parsing.json as pgpj
 import pygaps.utilities.exceptions as pgEx
 
+from ..test_utils import mpl_cleanup
 from .conftest import DATA
 from .conftest import DATA_N77_PATH
 
 
 @pytest.mark.characterisation
 class TestAreaBET():
     """Tests BET surface area calculations."""
@@ -103,14 +103,14 @@
             area = ab.area_BET(isotherm, branch="des").get("area")
         assert caplog.records
 
         err_relative = 0.1  # 10 percent
         err_absolute = 0.1  # 0.1 m2
         assert isclose(area, sample['bet_area_des'], err_relative, err_absolute)
 
-    @cleanup
+    @mpl_cleanup
     def test_area_BET_output(self):
         """Test verbosity."""
         sample = DATA['MCM-41']
         filepath = DATA_N77_PATH / sample['file']
         isotherm = pgpj.isotherm_from_json(filepath)
         ab.area_BET(isotherm, verbose=True)
```

### Comparing `pygaps-4.4.2/tests/characterisation/test_area_langmuir.py` & `pygaps-4.5.0/tests/characterisation/test_area_langmuir.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 
 Functions are tested against pre-calculated values on real isotherms.
 All pre-calculated data for characterisation can be found in the
 /.conftest file together with the other isotherm parameters.
 """
 
 import pytest
-from matplotlib.testing.decorators import cleanup
 from numpy import isclose
 from numpy import linspace
 
 import pygaps.characterisation.area_lang as al
 import pygaps.parsing.json as pgpj
 import pygaps.utilities.exceptions as pgEx
 
+from ..test_utils import mpl_cleanup
 from .conftest import DATA
 from .conftest import DATA_N77_PATH
 
 
 @pytest.mark.characterisation
 class TestAreaLangmuir():
     """Tests Langmuir surface area calculations."""
@@ -87,14 +87,14 @@
 
         area = al.area_langmuir(isotherm, branch="des").get("area")
 
         err_relative = 0.1  # 10 percent
         err_absolute = 0.1  # 0.1 m2
         assert isclose(area, sample['langmuir_area'], err_relative, err_absolute)
 
-    @cleanup
+    @mpl_cleanup
     def test_area_langmuir_output(self):
         """Test verbosity."""
         sample = DATA['MCM-41']
         filepath = DATA_N77_PATH / sample['file']
         isotherm = pgpj.isotherm_from_json(filepath)
         al.area_langmuir(isotherm, verbose=True)
```

### Comparing `pygaps-4.4.2/tests/characterisation/test_dr_da_plots.py` & `pygaps-4.5.0/tests/characterisation/test_dr_da_plots.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 
 Functions are tested against pre-calculated values on real isotherms.
 All pre-calculated data for characterisation can be found in the
 /.conftest file together with the other isotherm parameters.
 """
 
 import pytest
-from matplotlib.testing.decorators import cleanup
 from numpy import isclose
 
 import pygaps.characterisation.dr_da_plots as drda
 import pygaps.parsing.json as pgpj
 import pygaps.utilities.exceptions as pgEx
 
+from ..test_utils import mpl_cleanup
 from .conftest import DATA
 from .conftest import DATA_N77_PATH
 
 
 @pytest.mark.characterisation
 class TestDAPlot():
     """Tests DA and DR plots."""
@@ -82,14 +82,14 @@
 
             err_relative = 0.05  # 5 percent
             err_absolute = 0.01  # 0.01 cm3/g
 
             assert isclose(da_vol, sample['da_volume'], err_relative, err_absolute)
             assert isclose(da_pot, sample['da_potential'], err_relative, err_absolute)
 
-    @cleanup
+    @mpl_cleanup
     def test_da_output(self):
         """Test verbosity."""
         sample = DATA['Takeda 5A']
         filepath = DATA_N77_PATH / sample['file']
         isotherm = pgpj.isotherm_from_json(filepath)
         drda.da_plot(isotherm, verbose=True)
```

### Comparing `pygaps-4.4.2/tests/characterisation/test_initial_enthalpy.py` & `pygaps-4.5.0/tests/characterisation/test_initial_enthalpy.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 
 Functions are tested against pre-calculated values on real isotherms.
 All pre-calculated data for characterisation can be found in the
 /.conftest file together with the other isotherm parameters.
 """
 
 import pytest
-from matplotlib.testing.decorators import cleanup
 from numpy import isclose
 
 import pygaps.characterisation.initial_enth as ie
 import pygaps.parsing as pgp
 import pygaps.utilities.exceptions as pgEx
 
+from ..test_utils import mpl_cleanup
 from .conftest import DATA_CALO
 from .conftest import DATA_CALO_PATH
 
 
 @pytest.mark.characterisation
 class TestInitialEnthalpyPoint():
     """Test point initial enthalpy methods."""
@@ -37,23 +37,22 @@
     @pytest.mark.parametrize('sample', [sample for sample in DATA_CALO])
     def test_ienthalpy_point(self, sample):
         """The point method."""
         sample = DATA_CALO[sample]
         filepath = DATA_CALO_PATH / sample['file']
         isotherm = pgp.isotherm_from_json(filepath)
 
-        ienth_poly = ie.initial_enthalpy_point(isotherm, 'enthalpy'
-                                               ).get('initial_enthalpy')
+        ienth_poly = ie.initial_enthalpy_point(isotherm, 'enthalpy').get('initial_enthalpy')
 
         err_relative = 0.1  # 10 percent
         err_absolute = 1  #
 
         assert isclose(ienth_poly, sample['ienth'], err_relative, err_absolute)
 
-    @cleanup
+    @mpl_cleanup
     def test_ienthalpy_point_output(self):
         """Test verbosity."""
         sample = DATA_CALO['Takeda 5A']
         filepath = DATA_CALO_PATH / sample['file']
         isotherm = pgp.isotherm_from_json(filepath)
         ie.initial_enthalpy_point(isotherm, 'enthalpy', verbose=True)
 
@@ -71,22 +70,21 @@
     @pytest.mark.parametrize('sample', [sample for sample in DATA_CALO])
     def test_ienthalpy_comb(self, sample):
         """The combined polynomial method"""
         sample = DATA_CALO[sample]
         filepath = DATA_CALO_PATH / sample['file']
         isotherm = pgp.isotherm_from_json(filepath)
 
-        ienth_poly = ie.initial_enthalpy_comp(isotherm, 'enthalpy'
-                                              ).get('initial_enthalpy')
+        ienth_poly = ie.initial_enthalpy_comp(isotherm, 'enthalpy').get('initial_enthalpy')
 
         err_relative = 0.1  # 10 percent
         err_absolute = 1  #
 
         assert isclose(ienth_poly, sample['ienth'], err_relative, err_absolute)
 
-    @cleanup
+    @mpl_cleanup
     def test_ienthalpy_comb_output(self):
         """Test verbosity."""
         sample = DATA_CALO['Takeda 5A']
         filepath = DATA_CALO_PATH / sample['file']
         isotherm = pgp.isotherm_from_json(filepath)
         ie.initial_enthalpy_comp(isotherm, 'enthalpy', verbose=True)
```

### Comparing `pygaps-4.4.2/tests/characterisation/test_initial_henry.py` & `pygaps-4.5.0/tests/characterisation/test_initial_henry.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 
 Functions are tested against pre-calculated values on real isotherms.
 All pre-calculated data for characterisation can be found in the
 /.conftest file together with the other isotherm parameters.
 """
 
 import pytest
-from matplotlib.testing.decorators import cleanup
 from numpy import isclose
 
 import pygaps.characterisation.initial_henry as ih
 import pygaps.parsing as pgp
 import pygaps.utilities.exceptions as pgEx
 
+from ..test_utils import mpl_cleanup
 from .conftest import DATA
 from .conftest import DATA_N77_PATH
 
 
 @pytest.mark.characterisation
 class TestInitialHenry():
     """Test all initial henry methods."""
@@ -37,33 +37,29 @@
             isotherm = pgp.isotherm_from_json(filepath)
 
             ihenry_slope = ih.initial_henry_slope(isotherm, max_adjrms=0.01)
 
             err_relative = 0.1  # 10 percent
             err_absolute = 10  #
 
-            assert isclose(
-                ihenry_slope, sample['Khi_slope'], err_relative, err_absolute
-            )
+            assert isclose(ihenry_slope, sample['Khi_slope'], err_relative, err_absolute)
 
     def test_ihenry_slope_limits(self):
         """Test introducing limits in the initial slope method."""
         sample = DATA['SiO2']
         filepath = DATA_N77_PATH / sample['file']
         isotherm = pgp.isotherm_from_json(filepath)
         ih.initial_henry_slope(isotherm, max_adjrms=0.01, p_limits=[0, 0.2])
         ih.initial_henry_slope(isotherm, max_adjrms=0.01, p_limits=[0.2, None])
         ih.initial_henry_slope(isotherm, max_adjrms=0.01, l_limits=[5, None])
 
         with pytest.raises(pgEx.ParameterError):
-            ih.initial_henry_slope(
-                isotherm, max_adjrms=0.01, l_limits=[25, None]
-            )
+            ih.initial_henry_slope(isotherm, max_adjrms=0.01, l_limits=[25, None])
 
-    @cleanup
+    @mpl_cleanup
     def test_ihenry_slope_verbose(self):
         """Test verbosity."""
         sample = DATA['MCM-41']
         filepath = DATA_N77_PATH / sample['file']
         isotherm = pgp.isotherm_from_json(filepath)
         ih.initial_henry_slope(isotherm, verbose=True)
 
@@ -78,18 +74,16 @@
             isotherm = pgp.isotherm_from_json(filepath)
 
             ihenry_virial = ih.initial_henry_virial(isotherm)
 
             err_relative = 0.1  # 10 percent
             err_absolute = 10  #
 
-            assert isclose(
-                ihenry_virial, sample['Khi_virial'], err_relative, err_absolute
-            )
+            assert isclose(ihenry_virial, sample['Khi_virial'], err_relative, err_absolute)
 
-    @cleanup
+    @mpl_cleanup
     def test_ihenry_virial_verbose(self):
         """Test verbosity."""
         sample = DATA['SiO2']
         filepath = DATA_N77_PATH / sample['file']
         isotherm = pgp.isotherm_from_json(filepath)
         ih.initial_henry_virial(isotherm, verbose=True)
```

### Comparing `pygaps-4.4.2/tests/characterisation/test_isosteric_enthalpy.py` & `pygaps-4.5.0/tests/characterisation/test_enth_sorp_clausclap.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 
 Functions are tested against pre-calculated values on real isotherms.
 All pre-calculated data for characterisation can be found in the
 /.conftest file together with the other isotherm parameters.
 """
 
 import pytest
-from matplotlib.testing.decorators import cleanup
 from numpy import average
 from numpy import isclose
 
 import pygaps.characterisation.isosteric_enth as ie
 import pygaps.parsing as pgp
 import pygaps.utilities.exceptions as pgEx
 
+from ..test_utils import mpl_cleanup
 from .conftest import DATA_ISOSTERIC
 from .conftest import DATA_ISOSTERIC_PATH
 
 
 @pytest.mark.characterisation
 class TestIsostericEnthalpy():
     """Tests isosteric enthalpy calculations."""
@@ -61,15 +61,15 @@
             isotherm = pgp.isotherm_from_json(filepath)
             isotherms.append(isotherm)
 
         result_dict = ie.isosteric_enthalpy(isotherms)
 
         assert isclose(average(result_dict['isosteric_enthalpy']), 29, 0.5)
 
-    @cleanup
+    @mpl_cleanup
     def test_iso_enthalpy_output(self):
         """Test verbosity."""
         isotherms = []
 
         for sample in DATA_ISOSTERIC:
             filepath = DATA_ISOSTERIC_PATH / DATA_ISOSTERIC[sample]['file']
             isotherm = pgp.isotherm_from_json(filepath)
```

### Comparing `pygaps-4.4.2/tests/characterisation/test_models_hk.py` & `pygaps-4.5.0/tests/characterisation/test_models_hk.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/tests/characterisation/test_models_kelvin.py` & `pygaps-4.5.0/tests/characterisation/test_models_kelvin.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/tests/characterisation/test_models_thickness.py` & `pygaps-4.5.0/tests/characterisation/test_models_thickness.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/tests/characterisation/test_psd_kernel.py` & `pygaps-4.5.0/tests/characterisation/test_psd_kernel.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 versus stored values.
 All pre-calculated data for characterisation can be found in the
 /.conftest file together with the other isotherm parameters.
 """
 
 import numpy as np
 import pytest
-from matplotlib.testing.decorators import cleanup
 
 import pygaps.characterisation.psd_kernel as psdk
 import pygaps.parsing as pgp
 import pygaps.utilities.exceptions as pgEx
 
+from ..test_utils import mpl_cleanup
 from .conftest import DATA
 from .conftest import DATA_N77_PATH
 
 
 @pytest.mark.characterisation
 class TestPSDKernel():
     """Test pore size distribution calculation."""
@@ -63,14 +63,14 @@
             err_relative = 0.05  # 5 percent
             err_absolute = 0.01  # 0.01
 
             assert np.isclose(
                 principal_peak, sample['psd_micro_pore_size'], err_relative, err_absolute
             )
 
-    @cleanup
+    @mpl_cleanup
     def test_psd_dft_verbose(self):
         """Test verbosity."""
         sample = DATA['MCM-41']
         filepath = DATA_N77_PATH / sample['file']
         isotherm = pgp.isotherm_from_json(filepath)
         psdk.psd_dft(isotherm, verbose=True)
```

### Comparing `pygaps-4.4.2/tests/characterisation/test_psd_meso.py` & `pygaps-4.5.0/tests/characterisation/test_psd_meso.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 versus a stored value, with a margin of error.
 All pre-calculated data for characterisation can be found in
 the /.conftest file together with the other isotherm parameters.
 """
 
 import numpy as np
 import pytest
-from matplotlib.testing.decorators import cleanup
 
 import pygaps.characterisation.psd_meso as pmes
 import pygaps.parsing as pgp
 import pygaps.utilities.exceptions as pgEx
 
+from ..test_utils import mpl_cleanup
 from .conftest import DATA
 from .conftest import DATA_N77_PATH
 
 
 @pytest.mark.characterisation
 class TestPSDMeso():
     """Test mesopore size distribution calculation."""
@@ -74,14 +74,14 @@
             err_relative = 0.05  # 5 percent
             err_absolute = 0.01  # 0.01
 
             assert np.isclose(
                 principal_peak, sample['psd_meso_pore_size'], err_relative, err_absolute
             )
 
-    @cleanup
+    @mpl_cleanup
     def test_psd_meso_verbose(self):
         """Test verbosity."""
         sample = DATA['MCM-41']
         filepath = DATA_N77_PATH / sample['file']
         isotherm = pgp.isotherm_from_json(filepath)
         pmes.psd_mesoporous(isotherm, verbose=True)
```

### Comparing `pygaps-4.4.2/tests/characterisation/test_psd_micro.py` & `pygaps-4.5.0/tests/characterisation/test_psd_micro.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 versus stored values.
 All pre-calculated data for characterisation can be found in the
 /.conftest file together with the other isotherm parameters.
 """
 
 import numpy as np
 import pytest
-from matplotlib.testing.decorators import cleanup
 
 import pygaps.characterisation.psd_micro as pmic
 import pygaps.parsing as pgp
 import pygaps.utilities.exceptions as pgEx
 from pygaps.characterisation.models_hk import PROPERTIES_CARBON
 
+from ..test_utils import mpl_cleanup
 from .conftest import DATA
 from .conftest import DATA_N77_PATH
 
 N2_PROPS = {
     'molecular_diameter': 0.3,
     'polarizability': 0.0017403,
     'magnetic_susceptibility': 3.6e-08,
@@ -63,17 +63,15 @@
 
         assert np.isclose(pmic._N_over_RT(77), 9.40645E+20)
 
         km_ads = 1.23E-13
         km_mat = 4.91E-13
 
         assert np.isclose(pmic._kirkwood_muller_dispersion_ads(1, 1), km_ads)
-        assert np.isclose(
-            pmic._kirkwood_muller_dispersion_mat(1, 1, 2, 2), km_mat
-        )
+        assert np.isclose(pmic._kirkwood_muller_dispersion_mat(1, 1, 2, 2), km_mat)
         {'polarizability': 1, 'magnetic_susceptibility': 1}
 
         disp_dict = pmic._dispersion_from_dict({
             'polarizability': 1,
             'magnetic_susceptibility': 1
         }, {
             'polarizability': 2,
@@ -81,89 +79,69 @@
         })
         assert np.isclose(disp_dict[0], km_ads)
         assert np.isclose(disp_dict[1], km_mat)
 
     def test_psd_micro_solvers(self):
         """Check the HK and HK-CY solvers"""
 
-        assert np.isclose(
-            pmic._solve_hk([1], lambda x: np.log(x), 0.5, 1)[0], 1
-        )
+        assert np.isclose(pmic._solve_hk([1], lambda x: np.log(x), 0.5, 1)[0], 1)
 
         assert np.isclose(
-            pmic._solve_hk_cy([1.463017], np.array([0.5, 1]),
-                              lambda x: np.log(x), 0.5, 1)[0], 1, 0.001
+            pmic._solve_hk_cy([1.463017], np.array([0.5, 1]), lambda x: np.log(x), 0.5, 1)[0], 1,
+            0.001
         )
 
     def test_psd_micro_hk(self):
         """Test H-K psd model with blank arrays"""
 
         x = [0.001, 0.002]
         y = [1, 2]
 
         pmic.psd_horvath_kawazoe(x, y, 77, 'slit', N2_PROPS, PROPERTIES_CARBON)
-        pmic.psd_horvath_kawazoe(
-            x, x, 77, 'cylinder', N2_PROPS, PROPERTIES_CARBON
-        )
-        pmic.psd_horvath_kawazoe(
-            x, x, 77, 'sphere', N2_PROPS, PROPERTIES_CARBON
-        )
-        pmic.psd_horvath_kawazoe(
-            x, x, 77, 'slit', N2_PROPS, PROPERTIES_CARBON, use_cy=True
-        )
+        pmic.psd_horvath_kawazoe(x, x, 77, 'cylinder', N2_PROPS, PROPERTIES_CARBON)
+        pmic.psd_horvath_kawazoe(x, x, 77, 'sphere', N2_PROPS, PROPERTIES_CARBON)
+        pmic.psd_horvath_kawazoe(x, x, 77, 'slit', N2_PROPS, PROPERTIES_CARBON, use_cy=True)
 
     def test_psd_micro_ry(self):
         """Test H-K psd model with blank arrays"""
 
         x = [0.001, 0.002]
         y = [1, 2]
 
-        pmic.psd_horvath_kawazoe_ry(
-            x, y, 77, 'slit', N2_PROPS, PROPERTIES_CARBON
-        )
-        pmic.psd_horvath_kawazoe_ry(
-            x, x, 77, 'cylinder', N2_PROPS, PROPERTIES_CARBON
-        )
+        pmic.psd_horvath_kawazoe_ry(x, y, 77, 'slit', N2_PROPS, PROPERTIES_CARBON)
+        pmic.psd_horvath_kawazoe_ry(x, x, 77, 'cylinder', N2_PROPS, PROPERTIES_CARBON)
 
-        pmic.psd_horvath_kawazoe_ry(
-            x, x, 77, 'sphere', N2_PROPS, PROPERTIES_CARBON
-        )
+        pmic.psd_horvath_kawazoe_ry(x, x, 77, 'sphere', N2_PROPS, PROPERTIES_CARBON)
 
-        pmic.psd_horvath_kawazoe_ry(
-            x, x, 77, 'slit', N2_PROPS, PROPERTIES_CARBON, use_cy=True
-        )
+        pmic.psd_horvath_kawazoe_ry(x, x, 77, 'slit', N2_PROPS, PROPERTIES_CARBON, use_cy=True)
 
     @pytest.mark.parametrize('sample', [sample for sample in DATA])
     def test_psd_micro(self, sample):
         """Test psd calculation with several model isotherms"""
         sample = DATA[sample]
         # exclude datasets where it is not applicable
         if sample.get('psd_micro_pore_size', None):
 
             filepath = DATA_N77_PATH / sample['file']
             isotherm = pgp.isotherm_from_json(filepath)
 
-            result_dict = pmic.psd_microporous(
-                isotherm, psd_model='HK', pore_geometry='slit'
-            )
+            result_dict = pmic.psd_microporous(isotherm, psd_model='HK', pore_geometry='slit')
 
             loc = np.where(
-                result_dict['pore_distribution'] ==
-                max(result_dict['pore_distribution'])
+                result_dict['pore_distribution'] == max(result_dict['pore_distribution'])
             )
             principal_peak = result_dict['pore_widths'][loc]
 
             err_relative = 0.05  # 5 percent
             err_absolute = 0.01  # 0.01
 
             assert np.isclose(
-                principal_peak, sample['psd_micro_pore_size'], err_relative,
-                err_absolute
+                principal_peak, sample['psd_micro_pore_size'], err_relative, err_absolute
             )
 
-    @cleanup
+    @mpl_cleanup
     def test_psd_micro_verbose(self):
         """Test verbosity."""
         sample = DATA['MCM-41']
         filepath = DATA_N77_PATH / sample['file']
         isotherm = pgp.isotherm_from_json(filepath)
         pmic.psd_microporous(isotherm, verbose=True)
```

### Comparing `pygaps-4.4.2/tests/characterisation/test_t_plots.py` & `pygaps-4.5.0/tests/characterisation/test_t_plots.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 
 Functions are tested against pre-calculated values on real isotherms.
 All pre-calculated data for characterisation can be found in the
 /.conftest file together with the other isotherm parameters.
 """
 
 import pytest
-from matplotlib.testing.decorators import cleanup
 from numpy import isclose
 
 import pygaps.characterisation.t_plots as pt
 import pygaps.parsing as pgp
 import pygaps.utilities.exceptions as pgEx
 
+from ..test_utils import mpl_cleanup
 from .conftest import DATA
 from .conftest import DATA_N77_PATH
 
 
 @pytest.mark.characterisation
 class TestTPlot():
     """Tests t-plot calculations."""
@@ -77,14 +77,14 @@
             results[-1].get('adsorbed_volume'), sample['t_pore_volume'], err_relative,
             err_absolute_area
         )
         assert isclose(
             results[-1].get('area'), sample['s_t_area'], err_relative, err_absolute_volume
         )
 
-    @cleanup
+    @mpl_cleanup
     def test_t_plot_output(self):
         """Test verbosity."""
         sample = DATA['MCM-41']
         filepath = DATA_N77_PATH / sample['file']
         isotherm = pgp.isotherm_from_json(filepath)
         pt.t_plot(isotherm, 'Halsey', verbose=True)
```

### Comparing `pygaps-4.4.2/tests/cli/test_cli.py` & `pygaps-4.5.0/tests/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/tests/conftest.py` & `pygaps-4.5.0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,18 +142,19 @@
         'molar_mass': 28.01348,
         'cross_sectional_area': 0.162,
         'molecular_diameter': 0.3,
         'polarizability': 1.76E-3,
         'magnetic_susceptibility': 3.6E-8,
         'dipole_moment': 0.0,
         'quadrupole_moment': 1.52,
-        't_critical': 77.355,
-        'p_critical': 34.0,
-        'rhomolar_critical': 11.2,
+        't_critical': 126.2,
+        'p_critical': 33.95,
         't_triple': 63.1,
+        'p_triple': 0.1252,
+        'rhomolar_critical': 11.2,
         # properties for 1atm/ 77k
         'gas_density': 0.00461214,
         'liquid_density': 0.806,
         'surface_density': 6.71e18,
         'surface_tension': 8.8796,
         'saturation_pressure': 101325,
         'enthalpy_liquefaction': 5.5796,
```

### Comparing `pygaps-4.4.2/tests/core/conftest.py` & `pygaps-4.5.0/tests/core/conftest.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/tests/core/test_adsorbate.py` & `pygaps-4.5.0/tests/core/test_adsorbate.py`

 * *Files 9% similar despite different names*

```diff
@@ -70,14 +70,15 @@
         """Check standard adsorbates can be found."""
         ads = pygaps.Adsorbate.find('N2')
         assert ads == 'N2'
         assert ads == 'nitrogen'
         assert ads == 'Nitrogen'
 
     def test_adsorbate_formula(self):
+        """Check that formula is correctly latexed."""
         ads = pygaps.Adsorbate.find('N2')
         assert ads.formula == 'N_{2}'
         ads = pygaps.Adsorbate.find('D4')
         assert ads.formula == 'octamethylcyclotetrasiloxane'
 
     def test_adsorbate_get_properties(self, adsorbate_data, basic_adsorbate):
         """Check if properties of a adsorbate can be located."""
@@ -87,24 +88,37 @@
 
         name = basic_adsorbate.properties.pop('backend_name')
         with pytest.raises(ParameterError):
             name = basic_adsorbate.backend_name
         basic_adsorbate.properties['backend_name'] = name
 
     def test_adsorbate_fallback(self):
+        """Check if fallback to properties dictionary works."""
         ads = pygaps.Adsorbate("test")
         ads.properties["molar_mass"] = 142
         assert ads.molar_mass() == 142
 
     @pytest.mark.parametrize('calculated', [True, False])
     def test_adsorbate_named_props(self, adsorbate_data, basic_adsorbate, calculated):
+        """Test all named properties, both calculated and not."""
         temp = 77.355
         assert basic_adsorbate.molar_mass(calculated) == pytest.approx(
             adsorbate_data.get('molar_mass'), 0.001
         )
+        assert basic_adsorbate.t_triple(calculated
+                                        ) == pytest.approx(adsorbate_data.get('t_triple'), 0.001)
+        assert basic_adsorbate.p_triple(calculated) == pytest.approx(
+            adsorbate_data.get('p_triple') * 1e5, 0.001
+        )
+        assert basic_adsorbate.t_critical(calculated) == pytest.approx(
+            adsorbate_data.get('t_critical'), 0.001
+        )
+        assert basic_adsorbate.p_critical(calculated) == pytest.approx(
+            adsorbate_data.get('p_critical') * 1e5, 0.001
+        )
         assert basic_adsorbate.saturation_pressure(temp, calculate=calculated) == pytest.approx(
             adsorbate_data.get('saturation_pressure'), 0.001
         )
         assert basic_adsorbate.surface_tension(temp, calculate=calculated) == pytest.approx(
             adsorbate_data.get('surface_tension'), 0.001
         )
         assert basic_adsorbate.liquid_density(temp, calculate=calculated) == pytest.approx(
@@ -114,14 +128,15 @@
             adsorbate_data.get('gas_density'), 0.001
         )
         assert basic_adsorbate.enthalpy_liquefaction(temp, calculate=calculated) == pytest.approx(
             adsorbate_data.get('enthalpy_liquefaction'), 0.001
         )
 
     def test_adsorbate_miss_named_props(self):
+        """Test warning/error if properties cannot be calculated + are missing."""
         temp = 77.355
         ads = pygaps.Adsorbate(name='temp')
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             with pytest.raises(CalculationError):
                 ads.molar_mass()
             with pytest.raises(CalculationError):
```

### Comparing `pygaps-4.4.2/tests/core/test_baseisotherm.py` & `pygaps-4.5.0/tests/core/test_baseisotherm.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/tests/core/test_material.py` & `pygaps-4.5.0/tests/core/test_material.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/tests/core/test_modelisotherm.py` & `pygaps-4.5.0/tests/core/test_modelisotherm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Tests relating to the ModelIsotherm class."""
 
 import pandas
 import pytest
-from matplotlib.testing.decorators import cleanup
 from pandas.testing import assert_series_equal
 
 import pygaps
 import pygaps.modelling as pgm
 import pygaps.parsing as pgp
 import pygaps.utilities.exceptions as pgEx
 
 from ..characterisation.conftest import DATA
 from ..characterisation.conftest import DATA_N77_PATH
+from ..test_utils import mpl_cleanup
 from .conftest import LOADING_AT_PARAM
 from .conftest import LOADING_PARAM
 from .conftest import PRESSURE_AT_PARAM
 from .conftest import PRESSURE_PARAM
 
 
 @pytest.mark.core
@@ -37,72 +37,52 @@
             'adsorbate': 'nitrogen',
             'temperature': 77,
         }
 
         pressure = [1, 2, 3, 4, 5, 3, 2]
         loading = [1, 2, 3, 4, 5, 3, 2]
 
-        isotherm_data = pandas.DataFrame({
-            'pressure': pressure,
-            'loading': loading
-        })
+        isotherm_data = pandas.DataFrame({'pressure': pressure, 'loading': loading})
 
         # regular creation
-        pygaps.ModelIsotherm(
-            pressure=pressure,
-            loading=loading,
-            model='Henry',
-            **isotherm_param
-        )
+        pygaps.ModelIsotherm(pressure=pressure, loading=loading, model='Henry', **isotherm_param)
 
         # regular creation, DataFrame
-        pygaps.ModelIsotherm(
-            isotherm_data=isotherm_data, model='Henry', **isotherm_param
-        )
+        pygaps.ModelIsotherm(isotherm_data=isotherm_data, model='Henry', **isotherm_param)
 
         # regular creation, desorption
         pygaps.ModelIsotherm(
-            isotherm_data=isotherm_data,
-            model='Henry',
-            branch='des',
-            **isotherm_param
+            isotherm_data=isotherm_data, model='Henry', branch='des', **isotherm_param
         )
 
         # regular creation, guessed parameters
         pygaps.ModelIsotherm(
-            isotherm_data=isotherm_data,
-            model='Henry',
-            param_guess={'K': 1.0},
-            **isotherm_param
+            isotherm_data=isotherm_data, model='Henry', param_guess={'K': 1.0}, **isotherm_param
         )
 
         # regular creation, with bounds
         pygaps.ModelIsotherm(
             isotherm_data=isotherm_data,
             model='Henry',
             param_guess={'K': 1.0},
             param_bounds={'K': [0, 100]},
             **isotherm_param
         )
 
         # Missing pressure/loading
         with pytest.raises(pgEx.ParameterError):
-            pygaps.ModelIsotherm(
-                pressure=pressure, loading=None, **isotherm_param
-            )
+            pygaps.ModelIsotherm(pressure=pressure, loading=None, **isotherm_param)
 
         # Missing model
         with pytest.raises(pgEx.ParameterError):
             pygaps.ModelIsotherm(isotherm_data=isotherm_data, **isotherm_param)
 
         # Wrong model
         with pytest.raises(pgEx.ParameterError):
-            pygaps.ModelIsotherm(
-                isotherm_data=isotherm_data, model='Wrong', **isotherm_param
-            )
+            pygaps.ModelIsotherm(isotherm_data=isotherm_data, model='Wrong', **isotherm_param)
 
         # Wrong branch
         with pytest.raises(pgEx.ParameterError):
             pygaps.ModelIsotherm(
                 isotherm_data=isotherm_data,
                 model='Henry',
                 branch='random',
@@ -116,20 +96,15 @@
                 param_guess={'K9': 'woof'},
                 **isotherm_param
             )
 
     def test_isotherm_create_from_model(self, basic_isotherm):
         """Check isotherm can be created from a model."""
         model = pygaps.modelling.get_isotherm_model('Henry')
-        pygaps.ModelIsotherm(
-            model=model,
-            material='Test',
-            temperature=303,
-            adsorbate='nitrogen'
-        )
+        pygaps.ModelIsotherm(model=model, material='Test', temperature=303, adsorbate='nitrogen')
 
     def test_isotherm_create_from_isotherm(self, basic_isotherm):
         """Check isotherm can be created from Isotherm."""
         pygaps.ModelIsotherm.from_isotherm(
             basic_isotherm,
             isotherm_data=pandas.DataFrame({
                 'pressure': [1, 2, 3, 4, 5, 3, 2],
@@ -145,44 +120,37 @@
         with pytest.raises(pgEx.ParameterError):
             pygaps.ModelIsotherm.from_pointisotherm(basic_pointisotherm)
         pygaps.ModelIsotherm.from_pointisotherm(
             basic_pointisotherm,
             model='Henry',
         )
 
-    @cleanup
-    @pytest.mark.parametrize(
-        'file, ', [(data['file']) for data in list(DATA.values())]
-    )
+    @mpl_cleanup
+    @pytest.mark.parametrize('file, ', [(data['file']) for data in list(DATA.values())])
     def test_isotherm_create_guess(self, file):
         """Check isotherm can be guessed from PointIsotherm."""
 
         filepath = DATA_N77_PATH / file
         isotherm = pgp.isotherm_from_json(filepath)
 
-        pygaps.ModelIsotherm.from_pointisotherm(
-            isotherm, model='guess', verbose=True
-        )
+        pygaps.ModelIsotherm.from_pointisotherm(isotherm, model='guess', verbose=True)
 
-        pygaps.ModelIsotherm.from_pointisotherm(
-            isotherm, model=['Henry', 'Langmuir'], verbose=True
-        )
+        pygaps.ModelIsotherm.from_pointisotherm(isotherm, model=['Henry', 'Langmuir'], verbose=True)
 
         with pytest.raises(pgEx.ParameterError):
             pygaps.ModelIsotherm.from_pointisotherm(
                 isotherm, model=['Henry', 'DummyModel'], verbose=True
             )
 
     ##########################
 
     @pytest.mark.parametrize(
         'expected, parameters',
         [
-            pytest.param(1, {'branch': 'des'},
-                         marks=pytest.mark.xfail),  # Wrong branch
+            pytest.param(1, {'branch': 'des'}, marks=pytest.mark.xfail),  # Wrong branch
         ] + PRESSURE_PARAM
     )
     def test_isotherm_ret_pressure(
         self,
         use_adsorbate,
         basic_modelisotherm,
         expected,
@@ -202,16 +170,15 @@
         assert basic_modelisotherm.pressure(5, indexed=True).equals(
             pandas.Series([1.0, 2.25, 3.5, 4.75, 6.0], name='loading')
         )
 
     @pytest.mark.parametrize(
         'expected, parameters',
         [
-            pytest.param(1, {'branch': 'des'},
-                         marks=pytest.mark.xfail),  # Wrong branch
+            pytest.param(1, {'branch': 'des'}, marks=pytest.mark.xfail),  # Wrong branch
         ] + LOADING_PARAM
     )
     def test_isotherm_ret_loading(
         self,
         use_material,
         use_adsorbate,
         basic_modelisotherm,
@@ -226,25 +193,23 @@
 
     def test_isotherm_ret_loading_indexed(
         self,
         basic_modelisotherm,
     ):
         """Indexed option specified."""
         assert_series_equal(
-            basic_modelisotherm.loading(5, indexed=True),
-            pandas.Series([1.0, 2.25, 3.5, 4.75, 6.0])
+            basic_modelisotherm.loading(5, indexed=True), pandas.Series([1.0, 2.25, 3.5, 4.75, 6.0])
         )
 
     ##########################
 
     @pytest.mark.parametrize(
         'inp, expected, parameters',
         [
-            pytest.param(1, 1, {'branch': 'des'},
-                         marks=pytest.mark.xfail),  # Wrong branch
+            pytest.param(1, 1, {'branch': 'des'}, marks=pytest.mark.xfail),  # Wrong branch
         ] + PRESSURE_AT_PARAM
     )
     def test_isotherm_ret_pressure_at(
         self,
         use_material,
         use_adsorbate,
         basic_modelisotherm,
@@ -257,16 +222,15 @@
             inp,
             **parameters,
         ) == pytest.approx(expected, 1e-5)
 
     @pytest.mark.parametrize(
         'inp, expected, parameters',
         [
-            pytest.param(1, 1, {'branch': 'des'},
-                         marks=pytest.mark.xfail),  # Wrong branch
+            pytest.param(1, 1, {'branch': 'des'}, marks=pytest.mark.xfail),  # Wrong branch
         ] + LOADING_AT_PARAM
     )
     def test_isotherm_ret_loading_at(
         self,
         use_material,
         use_adsorbate,
         basic_modelisotherm,
@@ -280,33 +244,31 @@
             **parameters,
         ) == pytest.approx(expected, 1e-5)
 
     @pytest.mark.parametrize(
         'inp, expected, parameters',
         [
             (1, 1, dict()),
-            pytest.param(1, 1, {'branch': 'des'},
-                         marks=pytest.mark.xfail),  # Wrong branch
+            pytest.param(1, 1, {'branch': 'des'}, marks=pytest.mark.xfail),  # Wrong branch
             (100000, 1, dict(pressure_unit='Pa')),
             (0.5, 3.89137, dict(pressure_mode='relative')),
         ]
     )
     def test_isotherm_spreading_pressure_at(
         self,
         use_adsorbate,
         basic_modelisotherm,
         inp,
         parameters,
         expected,
     ):
         """Check the ModelIsotherm spreading pressure calculation."""
-        assert basic_modelisotherm.spreading_pressure_at(
-            inp, **parameters
-        ) == pytest.approx(expected, 1e-5)
+        assert basic_modelisotherm.spreading_pressure_at(inp, **parameters
+                                                         ) == pytest.approx(expected, 1e-5)
 
-    @cleanup
+    @mpl_cleanup
     def test_isotherm_print_parameters(self, basic_modelisotherm):
         """Checks isotherm can print its own info."""
 
         print(basic_modelisotherm)
         basic_modelisotherm.plot()
         basic_modelisotherm.print_info()
```

### Comparing `pygaps-4.4.2/tests/core/test_pointisotherm.py` & `pygaps-4.5.0/tests/core/test_pointisotherm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Tests relating to the PointIsotherm class."""
 
 import pandas
 import pytest
-from matplotlib.testing.decorators import cleanup
 from pandas.testing import assert_series_equal
 
 import pygaps
 import pygaps.utilities.exceptions as pgEx
 
+from ..test_utils import mpl_cleanup
 from .conftest import LOADING_AT_PARAM
 from .conftest import LOADING_PARAM
 from .conftest import PRESSURE_AT_PARAM
 from .conftest import PRESSURE_PARAM
 
 
 @pytest.mark.core
@@ -612,14 +612,14 @@
         assert (basic_pointisotherm.loading()[0] == pytest.approx(10, 0.001))
         # Convert from mmol/mol to mmol/g
         basic_pointisotherm.convert_material(basis_to='mass', unit_to='g')
         assert (basic_pointisotherm.loading()[0] == pytest.approx(1, 0.001))
 
     ##########################
 
-    @cleanup
+    @mpl_cleanup
     def test_isotherm_print_parameters(self, basic_pointisotherm):
         """Check isotherm can print its own info."""
 
         print(basic_pointisotherm)
         basic_pointisotherm.plot()
         basic_pointisotherm.print_info()
```

### Comparing `pygaps-4.4.2/tests/graphing/test_calc_graphs.py` & `pygaps-4.5.0/tests/graphing/test_calc_graphs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 """
 Tests calculation graphs such as PSD/t_plot/BET etc
 """
 
 import pytest
-from matplotlib.testing.decorators import cleanup
 
 import pygaps.graphing.calc_graphs as graphing
 
+from ..test_utils import mpl_cleanup
+
 
 @pytest.mark.graphing
 class TestCalcGraphs():
     """Tests all calculation graphs"""
-    @cleanup
+    @mpl_cleanup
     def test_bet_graph(self):
         """Test BET graph"""
 
         pressure = [0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7]
         bet_points = [0.1, 0.15, 0.2, 0.25, 0.3, 0.35, 0.4]
         min_p = 2
         max_p = 6
         slope = 0.5
         intercept = 0.01
         mono_p = 0.33
         mono_bet = 0.23
 
-        graphing.bet_plot(
-            pressure, bet_points, min_p, max_p, slope, intercept, mono_p,
-            mono_bet
-        )
+        graphing.bet_plot(pressure, bet_points, min_p, max_p, slope, intercept, mono_p, mono_bet)
 
-    @cleanup
+    @mpl_cleanup
     def test_roq_graph(self):
         """Test Rouquerol graph"""
 
         pressure = [0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7]
         roq_points = [0.1, 0.15, 0.2, 0.25, 0.3, 0.35, 0.4]
         min_p = 2
         max_p = 6
```

### Comparing `pygaps-4.4.2/tests/graphing/test_iast_graphs.py` & `pygaps-4.5.0/tests/graphing/test_iast_graphs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 """Tests IAST graphs."""
 
 import pytest
-from matplotlib.testing.decorators import cleanup
 
 import pygaps.graphing.iast_graphs as graphing
 
+from ..test_utils import mpl_cleanup
+
 
 @pytest.mark.graphing
 class TestIASTGraphs():
     """Test all IAST graphs."""
-    @cleanup
+    @mpl_cleanup
     def test_svp_graph(self):
         """Test svp graph."""
 
         pressure = [0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7]
         selectivity = [0.5, 0.5, 0.6, 0.6, 0.7, 0.8, 1.0]
         fraction = 0.3
 
-        graphing.plot_iast_svp(
-            pressure, selectivity, 'CO2', 'CH4', fraction, 'bar'
-        )
+        graphing.plot_iast_svp(pressure, selectivity, 'CO2', 'CH4', fraction, 'bar')
 
-    @cleanup
+    @mpl_cleanup
     def test_vle_graph(self):
         """Test vle graph."""
 
         x_data = [0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7]
         y_data = [0.1, 0.3, 0.4, 0.5, 0.6, 0.7, 0.7]
         pressure = 2
```

### Comparing `pygaps-4.4.2/tests/graphing/test_iso_graphs.py` & `pygaps-4.5.0/tests/graphing/test_iso_graphs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,85 +1,86 @@
 """
 Tests for the isotherm graphs
 """
 
 import pytest
-from matplotlib.testing.decorators import cleanup
 
 from pygaps.graphing.isotherm_graphs import plot_iso
 
+from ..test_utils import mpl_cleanup
+
 
 @pytest.mark.graphing
 class TestIsothermGraphs():
     """Tests regular isotherm graphs"""
-    @cleanup
+    @mpl_cleanup
     def test_basic_plot(self, basic_pointisotherm):
         plot_iso(basic_pointisotherm)
 
-    @cleanup
+    @mpl_cleanup
     def test_multi_plot(self, basic_pointisotherm):
         plot_iso([
             basic_pointisotherm,
             basic_pointisotherm,
             basic_pointisotherm,
         ])
 
-    @cleanup
+    @mpl_cleanup
     def test_data_plot(self, basic_pointisotherm):
         plot_iso(
             basic_pointisotherm,
             x_data='pressure',
             y1_data='loading',
             y2_data='enthalpy',
         )
         plot_iso(
             basic_pointisotherm,
             x_data='loading',
             y1_data='enthalpy',
         )
 
-    @cleanup
+    @mpl_cleanup
     def test_branch_plot(self, basic_pointisotherm):
         plot_iso(basic_pointisotherm, branch='ads')
         plot_iso(basic_pointisotherm, branch='des')
         plot_iso(basic_pointisotherm, branch='all')
 
-    @cleanup
+    @mpl_cleanup
     def test_convert_plot(self, use_adsorbate, basic_pointisotherm):
         plot_iso(basic_pointisotherm, pressure_unit='Pa')
         plot_iso(basic_pointisotherm, loading_unit='mol')
         plot_iso(basic_pointisotherm, pressure_mode='relative')
 
-    @cleanup
+    @mpl_cleanup
     def test_range_plot(self, basic_pointisotherm):
         plot_iso(basic_pointisotherm, x_range=(0, 4))
         plot_iso(basic_pointisotherm, x_range=(0, None))
         plot_iso(basic_pointisotherm, y1_range=(3, None))
         plot_iso(basic_pointisotherm, y1_range=(3, None))
         plot_iso(basic_pointisotherm, y2_range=(3, 100))
         plot_iso(basic_pointisotherm, y2_range=(None, 10))
 
-    @cleanup
+    @mpl_cleanup
     def test_log_plot(self, basic_pointisotherm):
         plot_iso(basic_pointisotherm, logx=True)
         plot_iso(basic_pointisotherm, logy1=True)
         plot_iso(basic_pointisotherm, logy2=True)
 
-    @cleanup
+    @mpl_cleanup
     def test_color_plot(self, basic_pointisotherm):
         plot_iso(basic_pointisotherm, color=False)
         plot_iso(basic_pointisotherm, color=3)
         plot_iso(basic_pointisotherm, color=['red'])
 
-    @cleanup
+    @mpl_cleanup
     def test_marker_plot(self, basic_pointisotherm):
         plot_iso(basic_pointisotherm, marker=False)
         plot_iso(basic_pointisotherm, marker=3)
         plot_iso(basic_pointisotherm, marker=['o'])
 
-    @cleanup
+    @mpl_cleanup
     def test_style_plot(self, basic_pointisotherm):
         plot_iso(basic_pointisotherm, y1_line_style=dict(linewidth=5))
 
-    @cleanup
+    @mpl_cleanup
     def test_legend_plot(self, basic_pointisotherm):
         plot_iso(basic_pointisotherm, lgd_keys=['material', 'temperature'])
```

### Comparing `pygaps-4.4.2/tests/modelling/conftest.py` & `pygaps-4.5.0/tests/modelling/conftest.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/tests/modelling/test_models_isotherm.py` & `pygaps-4.5.0/tests/modelling/test_models_isotherm.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/tests/parsing/test_aif.py` & `pygaps-4.5.0/tests/parsing/test_aif.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/tests/parsing/test_csv.py` & `pygaps-4.5.0/tests/parsing/test_csv.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/tests/parsing/test_excel.py` & `pygaps-4.5.0/tests/parsing/test_excel.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/tests/parsing/test_json.py` & `pygaps-4.5.0/tests/parsing/test_json.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/tests/parsing/test_sqlite_db.py` & `pygaps-4.5.0/tests/parsing/test_sqlite_db.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/tests/prediction/test_iast.py` & `pygaps-4.5.0/tests/prediction/test_iast.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 /.conftest file together with the other isotherm parameters.
 """
 
 import logging
 
 import numpy
 import pytest
-from matplotlib.testing.decorators import cleanup
 
 import pygaps
 import pygaps.iast.pgiast as pgi
 import pygaps.parsing as pgp
 import pygaps.utilities.exceptions as pgEx
 
+from ..test_utils import mpl_cleanup
 from .conftest import DATA_IAST
 from .conftest import DATA_IAST_PATH
 
 
 @pytest.fixture()
 def load_iast():
     """A fixture which loads files from the disk."""
@@ -90,15 +90,15 @@
         gas_fraction = [0.5, 0.5]
         adsorbed_fractions = [0.2833, 0.7167]
 
         loadings = pgi.iast_point_fraction(load_iast_models, gas_fraction, 1)
 
         assert numpy.isclose(adsorbed_fractions[0], loadings[0], 0.001)
 
-    @cleanup
+    @mpl_cleanup
     def test_iast_verbose(self, load_iast):
         """Test verbosity."""
         pgi.iast_point_fraction(load_iast, [0.5, 0.5], 1, verbose=True)
 
 
 @pytest.mark.modelling
 class TestReverseIAST():
@@ -152,15 +152,15 @@
         gas_fraction, actual_loading = pgi.reverse_iast(load_iast_models, ideal_ads_fraction, 1)
 
         actual_ads_fraction = actual_loading / numpy.sum(actual_loading)
 
         assert numpy.isclose(ideal_gas_fraction[0], gas_fraction[0], atol=0.1)
         assert numpy.isclose(ideal_ads_fraction[0], actual_ads_fraction[0], atol=0.05)
 
-    @cleanup
+    @mpl_cleanup
     def test_reverse_iast_verbose(self, load_iast):
         """Test verbosity."""
         pgi.reverse_iast(load_iast, [0.23064, 0.76936], 1, verbose=True)
 
 
 @pytest.mark.modelling
 class TestIASTVLE():
@@ -196,15 +196,15 @@
         y_data = result_dict['y']
 
         dev = sum(y_data - x_data)
         expected_dev = 8.8
 
         assert numpy.isclose(dev, expected_dev, atol=0.1)
 
-    @cleanup
+    @mpl_cleanup
     def test_iast_vle_verbose(self, load_iast):
         """Test verbosity."""
         pgi.iast_binary_vle(load_iast, 1, verbose=True)
 
 
 @pytest.mark.modelling
 class TestIASTSVP():
@@ -242,12 +242,12 @@
         result_dict = pgi.iast_binary_svp(load_iast_models, [0.5, 0.5], rng)
 
         expected_avg = 0.13
         avg = numpy.average(result_dict['selectivity'])
 
         assert numpy.isclose(avg, expected_avg, atol=0.01)
 
-    @cleanup
+    @mpl_cleanup
     def test_iast_vle_verbose(self, load_iast):
         """Test verbosity."""
         rng = numpy.linspace(0.01, 10, 30)
         pgi.iast_binary_svp(load_iast, [0.5, 0.5], rng, verbose=True)
```

### Comparing `pygaps-4.4.2/tests/utilities/test_converter.py` & `pygaps-4.5.0/tests/utilities/test_converter.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/tests/utilities/test_coolprop_interaction.py` & `pygaps-4.5.0/tests/utilities/test_coolprop_interaction.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/tests/utilities/test_python_utilities.py` & `pygaps-4.5.0/tests/utilities/test_python_utilities.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/tests/utilities/test_sqlite_utilities.py` & `pygaps-4.5.0/tests/utilities/test_sqlite_utilities.py`

 * *Files identical despite different names*

### Comparing `pygaps-4.4.2/tests/utilities/test_string_utilities.py` & `pygaps-4.5.0/tests/utilities/test_string_utilities.py`

 * *Files identical despite different names*

