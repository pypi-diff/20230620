# Comparing `tmp/adaptfx-0.2.0.tar.gz` & `tmp/adaptfx-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptfx-0.2.0.tar", last modified: Wed Feb  1 18:07:45 2023, max compression
+gzip compressed data, was "adaptfx-0.2.1.tar", last modified: Tue Jun 20 15:01:02 2023, max compression
```

## Comparing `adaptfx-0.2.0.tar` & `adaptfx-0.2.1.tar`

### file list

```diff
@@ -1,242 +1,253 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:07:45.768545 adaptfx-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:07:45.708545 adaptfx-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:07:45.712545 adaptfx-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-02-01 18:07:22.000000 adaptfx-0.2.0/.github/workflows/build_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-02-01 18:07:22.000000 adaptfx-0.2.0/.github/workflows/test_build_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-02-01 18:07:22.000000 adaptfx-0.2.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:07:45.740545 adaptfx-0.2.0/DVH_figures/
--rw-r--r--   0 runner    (1001) docker     (123)    63689 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-1_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    63799 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-1_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    63218 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-1_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    63680 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-1_4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    63526 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-1_5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    63629 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-1_planning.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    60284 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-2_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    62273 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-2_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    63071 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-2_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    61658 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-2_4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    62585 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-2_5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    62247 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-2_planning.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    59244 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-3_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    58497 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-3_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    58473 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-3_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    59402 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-3_4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    59147 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-3_5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    58547 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-3_planning.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    62463 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-4_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    61610 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-4_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    62992 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-4_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    62219 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-4_4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    61773 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-4_5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    61786 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-4_planning.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    62932 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-5_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    63582 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-5_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    62814 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-5_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    63360 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-5_4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    63320 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-5_5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    63871 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-5_planning.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    61632 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-6_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    61723 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-6_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    62637 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-6_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    63133 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-6_4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    63093 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-6_5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    62221 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient-6_planning.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    38726 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_10_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    38703 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_10_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    38653 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_10_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    38703 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_10_4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    38500 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_10_5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    38624 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_10_planning.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    35221 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_11_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    35135 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_11_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    35352 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_11_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    35314 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_11_4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    35317 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_11_5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    35907 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_11_planning.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    42579 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_12_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    42624 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_12_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    42527 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_12_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    42744 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_12_4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    42415 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_12_5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    42586 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_12_planning.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    40594 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_13_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    40240 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_13_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    40701 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_13_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    40888 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_13_4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    39722 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_13_5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    40631 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_13_planning.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    38905 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_14_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    39415 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_14_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    39287 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_14_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    38925 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_14_4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    39178 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_14_5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_14_planning.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    40098 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_15_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    39982 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_15_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    40318 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_15_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    39969 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_15_4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    40155 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_15_5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    40484 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_15_planning.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    40443 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_16_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    41486 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_16_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    40491 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_16_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    40012 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_16_4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    39806 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_16_5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    40145 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_16_planning.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    43437 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_7_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    43186 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_7_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    43407 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_7_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    43561 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_7_4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    43914 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_7_5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    43373 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_7_planning.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    35123 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_8_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    35730 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_8_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    35880 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_8_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    35133 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_8_4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    34844 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_8_5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    36410 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_8_planning.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    42437 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_9_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    41726 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_9_2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    41993 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_9_3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    42612 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_9_4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    42180 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_9_5.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    42012 2023-02-01 18:07:22.000000 adaptfx-0.2.0/DVH_figures/Patient_9_planning.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:07:45.740545 adaptfx-0.2.0/GUI/
--rw-r--r--   0 runner    (1001) docker     (123)    34724 2023-02-01 18:07:22.000000 adaptfx-0.2.0/GUI/2D_GUI.py
--rw-r--r--   0 runner    (1001) docker     (123)    29276 2023-02-01 18:07:22.000000 adaptfx-0.2.0/GUI/3D_GUI.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-02-01 18:07:22.000000 adaptfx-0.2.0/GUI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-02-01 18:07:22.000000 adaptfx-0.2.0/GUI/gamma_distribution_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-02-01 18:07:22.000000 adaptfx-0.2.0/GUI/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    23509 2023-02-01 18:07:22.000000 adaptfx-0.2.0/GUI/interpol2D_OAR.py
--rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-02-01 18:07:22.000000 adaptfx-0.2.0/GUI/interpol2D_OARminfrac.py
--rw-r--r--   0 runner    (1001) docker     (123)    25178 2023-02-01 18:07:22.000000 adaptfx-0.2.0/GUI/interpol2D_tumor.py
--rw-r--r--   0 runner    (1001) docker     (123)    28365 2023-02-01 18:07:22.000000 adaptfx-0.2.0/GUI/interpol3D.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-02-01 18:07:22.000000 adaptfx-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-02-01 18:07:22.000000 adaptfx-0.2.0/MANUAL.md
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-02-01 18:07:45.768545 adaptfx-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:07:45.764545 adaptfx-0.2.0/Patientdata_paper/
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_11_1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_11_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_11_3.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_11_4.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_11_5.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_11_planning.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_12_1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_12_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_12_3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19489 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_12_4.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19423 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_12_5.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19683 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_12_planning.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20145 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_13_1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19839 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_13_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20145 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_13_3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    22272 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_13_4.csv
--rw-r--r--   0 runner    (1001) docker     (123)    18367 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_13_5.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20193 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_13_planning.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_14_1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15436 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_14_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15275 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_14_3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15262 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_14_4.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_14_5.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_14_planning.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15095 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_15_1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14616 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_15_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15441 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_15_3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_15_4.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14927 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_15_5.csv
--rw-r--r--   0 runner    (1001) docker     (123)    15158 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_15_planning.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21741 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_16_1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21739 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_16_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21262 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_16_3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21044 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_16_4.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20991 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_16_5.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21268 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_16_planning.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_1_1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12543 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_1_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_1_3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13371 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_1_4.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_1_5.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_1_planning.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13251 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_2_1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_2_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_2_3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_2_4.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_2_5.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_2_planning.csv
--rw-r--r--   0 runner    (1001) docker     (123)    18440 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_3_1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    18394 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_3_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    18123 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_3_3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    18578 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_3_4.csv
--rw-r--r--   0 runner    (1001) docker     (123)    18356 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_3_5.csv
--rw-r--r--   0 runner    (1001) docker     (123)    17374 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_3_planning.csv
--rw-r--r--   0 runner    (1001) docker     (123)    17757 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_4_1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    16527 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_4_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    16451 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_4_3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    16688 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_4_4.csv
--rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_4_5.csv
--rw-r--r--   0 runner    (1001) docker     (123)    16343 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_4_planning.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_5_.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_5_1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_5_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14209 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_5_3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_5_4.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14071 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_5_5.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19593 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_6_1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19783 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_6_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19295 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_6_3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19028 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_6_4.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_6_5.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19293 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_6_planning.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14163 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_7_1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13853 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_7_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14351 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_7_3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_7_4.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14415 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_7_5.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_7_planning.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_8_1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_8_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_8_3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_8_4.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_8_5.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_8_planning.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19064 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_9_1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    18465 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_9_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    18708 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_9_3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19182 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_9_4.csv
--rw-r--r--   0 runner    (1001) docker     (123)    18567 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_9_5.csv
--rw-r--r--   0 runner    (1001) docker     (123)    18402 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/Patient_9_planning.csv
--rw-r--r--   0 runner    (1001) docker     (123)    22510 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/patient_10_1.csv
--rw-r--r--   0 runner    (1001) docker     (123)    23441 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/patient_10_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)    23092 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/patient_10_3.csv
--rw-r--r--   0 runner    (1001) docker     (123)    22730 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/patient_10_4.csv
--rw-r--r--   0 runner    (1001) docker     (123)    22386 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/patient_10_5.csv
--rw-r--r--   0 runner    (1001) docker     (123)    23081 2023-02-01 18:07:22.000000 adaptfx-0.2.0/Patientdata_paper/patient_10_planning.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-02-01 18:07:22.000000 adaptfx-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-02-01 18:07:22.000000 adaptfx-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-01 18:07:45.768545 adaptfx-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-01 18:07:22.000000 adaptfx-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:07:45.712545 adaptfx-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:07:45.764545 adaptfx-0.2.0/src/adaptfx/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-02-01 18:07:22.000000 adaptfx-0.2.0/src/adaptfx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-01 18:07:45.000000 adaptfx-0.2.0/src/adaptfx/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-02-01 18:07:22.000000 adaptfx-0.2.0/src/adaptfx/aft.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-02-01 18:07:22.000000 adaptfx-0.2.0/src/adaptfx/aft_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-02-01 18:07:22.000000 adaptfx-0.2.0/src/adaptfx/aft_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-02-01 18:07:22.000000 adaptfx-0.2.0/src/adaptfx/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-02-01 18:07:22.000000 adaptfx-0.2.0/src/adaptfx/maths.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-02-01 18:07:22.000000 adaptfx-0.2.0/src/adaptfx/planning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-02-01 18:07:22.000000 adaptfx-0.2.0/src/adaptfx/radiobiology.py
--rw-r--r--   0 runner    (1001) docker     (123)    12815 2023-02-01 18:07:22.000000 adaptfx-0.2.0/src/adaptfx/reinforce.py
--rw-r--r--   0 runner    (1001) docker     (123)    42308 2023-02-01 18:07:22.000000 adaptfx-0.2.0/src/adaptfx/reinforce_old.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-02-01 18:07:22.000000 adaptfx-0.2.0/src/adaptfx/visualiser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:07:45.768545 adaptfx-0.2.0/src/adaptfx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-02-01 18:07:45.000000 adaptfx-0.2.0/src/adaptfx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-02-01 18:07:45.000000 adaptfx-0.2.0/src/adaptfx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 18:07:45.000000 adaptfx-0.2.0/src/adaptfx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-01 18:07:45.000000 adaptfx-0.2.0/src/adaptfx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-01 18:07:45.000000 adaptfx-0.2.0/src/adaptfx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-01 18:07:45.000000 adaptfx-0.2.0/src/adaptfx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 18:07:45.768545 adaptfx-0.2.0/work/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-02-01 18:07:22.000000 adaptfx-0.2.0/work/frac_example.json
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-02-01 18:07:22.000000 adaptfx-0.2.0/work/oar_example.json
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-02-01 18:07:22.000000 adaptfx-0.2.0/work/testing.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:01:02.911055 adaptfx-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:01:02.875055 adaptfx-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:01:02.875055 adaptfx-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-20 15:00:44.000000 adaptfx-0.2.1/.github/workflows/build_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-20 15:00:44.000000 adaptfx-0.2.1/.github/workflows/test_build_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-20 15:00:44.000000 adaptfx-0.2.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:01:02.891055 adaptfx-0.2.1/DVH_figures/
+-rw-r--r--   0 runner    (1001) docker     (123)    63689 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-1_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    63799 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-1_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    63218 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-1_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    63680 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-1_4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    63526 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-1_5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    63629 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-1_planning.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    60284 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-2_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    62273 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-2_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    63071 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-2_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    61658 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-2_4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    62585 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-2_5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    62247 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-2_planning.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    59244 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-3_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    58497 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-3_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    58473 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-3_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    59402 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-3_4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    59147 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-3_5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    58547 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-3_planning.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    62463 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-4_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    61610 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-4_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    62992 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-4_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    62219 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-4_4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    61773 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-4_5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    61786 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-4_planning.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    62932 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-5_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    63582 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-5_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    62814 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-5_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    63360 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-5_4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    63320 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-5_5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    63871 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-5_planning.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    61632 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-6_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    61723 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-6_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    62637 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-6_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    63133 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-6_4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    63093 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-6_5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    62221 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient-6_planning.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    38726 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_10_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    38703 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_10_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    38653 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_10_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    38703 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_10_4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    38500 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_10_5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    38624 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_10_planning.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    35221 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_11_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    35135 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_11_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    35352 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_11_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    35314 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_11_4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    35317 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_11_5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    35907 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_11_planning.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    42579 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_12_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    42624 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_12_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    42527 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_12_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    42744 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_12_4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    42415 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_12_5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    42586 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_12_planning.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    40594 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_13_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    40240 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_13_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    40701 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_13_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    40888 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_13_4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    39722 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_13_5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    40631 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_13_planning.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    38905 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_14_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    39415 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_14_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    39287 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_14_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    38925 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_14_4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    39178 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_14_5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_14_planning.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    40098 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_15_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    39982 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_15_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    40318 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_15_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    39969 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_15_4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    40155 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_15_5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    40484 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_15_planning.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    40443 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_16_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    41486 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_16_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    40491 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_16_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    40012 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_16_4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    39806 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_16_5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    40145 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_16_planning.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    43437 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_7_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    43186 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_7_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    43407 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_7_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    43561 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_7_4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    43914 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_7_5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    43373 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_7_planning.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    35123 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_8_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    35730 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_8_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    35880 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_8_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    35133 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_8_4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    34844 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_8_5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    36410 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_8_planning.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    42437 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_9_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    41726 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_9_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    41993 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_9_3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    42612 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_9_4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    42180 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_9_5.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    42012 2023-06-20 15:00:44.000000 adaptfx-0.2.1/DVH_figures/Patient_9_planning.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:01:02.895055 adaptfx-0.2.1/GUI/
+-rw-r--r--   0 runner    (1001) docker     (123)    34724 2023-06-20 15:00:44.000000 adaptfx-0.2.1/GUI/2D_GUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29276 2023-06-20 15:00:44.000000 adaptfx-0.2.1/GUI/3D_GUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 15:00:44.000000 adaptfx-0.2.1/GUI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-20 15:00:44.000000 adaptfx-0.2.1/GUI/gamma_distribution_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-20 15:00:44.000000 adaptfx-0.2.1/GUI/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23509 2023-06-20 15:00:44.000000 adaptfx-0.2.1/GUI/interpol2D_OAR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-06-20 15:00:44.000000 adaptfx-0.2.1/GUI/interpol2D_OARminfrac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25178 2023-06-20 15:00:44.000000 adaptfx-0.2.1/GUI/interpol2D_tumor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28365 2023-06-20 15:00:44.000000 adaptfx-0.2.1/GUI/interpol3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-20 15:00:44.000000 adaptfx-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-06-20 15:00:44.000000 adaptfx-0.2.1/MANUAL.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11698 2023-06-20 15:01:02.911055 adaptfx-0.2.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:01:02.907055 adaptfx-0.2.1/Patientdata_paper/
+-rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_11_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_11_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_11_3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_11_4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_11_5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_11_planning.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_12_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_12_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_12_3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19489 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_12_4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19423 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_12_5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19683 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_12_planning.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20145 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_13_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19839 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_13_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20145 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_13_3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    22272 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_13_4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    18367 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_13_5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20193 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_13_planning.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_14_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15436 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_14_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15275 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_14_3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15262 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_14_4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_14_5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15006 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_14_planning.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15095 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_15_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14616 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_15_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15441 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_15_3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_15_4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14927 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_15_5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    15158 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_15_planning.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21741 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_16_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21739 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_16_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21262 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_16_3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21044 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_16_4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20991 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_16_5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21268 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_16_planning.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_1_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12543 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_1_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_1_3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13371 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_1_4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_1_5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_1_planning.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13251 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_2_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_2_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_2_3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_2_4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13109 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_2_5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_2_planning.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    18440 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_3_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    18394 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_3_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    18123 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_3_3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    18578 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_3_4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    18356 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_3_5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    17374 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_3_planning.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    17757 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_4_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    16527 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_4_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    16451 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_4_3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    16688 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_4_4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_4_5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    16343 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_4_planning.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_5_.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_5_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13928 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_5_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14209 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_5_3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_5_4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14071 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_5_5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19593 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_6_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19783 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_6_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19295 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_6_3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19028 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_6_4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_6_5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19293 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_6_planning.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14163 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_7_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13853 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_7_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14351 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_7_3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_7_4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14415 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_7_5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_7_planning.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_8_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_8_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_8_3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10366 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_8_4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10113 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_8_5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_8_planning.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19064 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_9_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    18465 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_9_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    18708 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_9_3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19182 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_9_4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    18567 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_9_5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    18402 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/Patient_9_planning.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    22510 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/patient_10_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    23441 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/patient_10_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    23092 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/patient_10_3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    22730 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/patient_10_4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    22386 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/patient_10_5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    23081 2023-06-20 15:00:44.000000 adaptfx-0.2.1/Patientdata_paper/patient_10_planning.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-06-20 15:00:44.000000 adaptfx-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-20 15:00:44.000000 adaptfx-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:01:02.911055 adaptfx-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-20 15:00:44.000000 adaptfx-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:01:02.875055 adaptfx-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:01:02.907055 adaptfx-0.2.1/src/adaptfx/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-20 15:00:44.000000 adaptfx-0.2.1/src/adaptfx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 15:01:02.000000 adaptfx-0.2.1/src/adaptfx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9254 2023-06-20 15:00:44.000000 adaptfx-0.2.1/src/adaptfx/aft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-20 15:00:44.000000 adaptfx-0.2.1/src/adaptfx/aft_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-06-20 15:00:44.000000 adaptfx-0.2.1/src/adaptfx/aft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-20 15:00:44.000000 adaptfx-0.2.1/src/adaptfx/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-06-20 15:00:44.000000 adaptfx-0.2.1/src/adaptfx/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-06-20 15:00:44.000000 adaptfx-0.2.1/src/adaptfx/planning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-20 15:00:44.000000 adaptfx-0.2.1/src/adaptfx/radiobiology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25391 2023-06-20 15:00:44.000000 adaptfx-0.2.1/src/adaptfx/reinforce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32803 2023-06-20 15:00:44.000000 adaptfx-0.2.1/src/adaptfx/reinforce_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-20 15:00:44.000000 adaptfx-0.2.1/src/adaptfx/visualiser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:01:02.907055 adaptfx-0.2.1/src/adaptfx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11698 2023-06-20 15:01:02.000000 adaptfx-0.2.1/src/adaptfx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-06-20 15:01:02.000000 adaptfx-0.2.1/src/adaptfx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:01:02.000000 adaptfx-0.2.1/src/adaptfx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-20 15:01:02.000000 adaptfx-0.2.1/src/adaptfx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 15:01:02.000000 adaptfx-0.2.1/src/adaptfx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 15:01:02.000000 adaptfx-0.2.1/src/adaptfx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:01:02.907055 adaptfx-0.2.1/src/adaptsim/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-20 15:00:44.000000 adaptfx-0.2.1/src/adaptsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-06-20 15:00:44.000000 adaptfx-0.2.1/src/adaptsim/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-20 15:00:44.000000 adaptfx-0.2.1/src/adaptsim/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-20 15:00:44.000000 adaptfx-0.2.1/src/adaptsim/visualiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-20 15:00:44.000000 adaptfx-0.2.1/src/adaptsim/visualiser_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:01:02.911055 adaptfx-0.2.1/work/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-20 15:00:44.000000 adaptfx-0.2.1/work/example_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-20 15:00:44.000000 adaptfx-0.2.1/work/example_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-20 15:00:44.000000 adaptfx-0.2.1/work/example_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-20 15:00:44.000000 adaptfx-0.2.1/work/example_3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-20 15:00:44.000000 adaptfx-0.2.1/work/example_4.json
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-20 15:00:44.000000 adaptfx-0.2.1/work/example_5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-20 15:00:44.000000 adaptfx-0.2.1/work/example_6.json
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-20 15:00:44.000000 adaptfx-0.2.1/work/example_7.json
```

### Comparing `adaptfx-0.2.0/.github/workflows/build_publish.yml` & `adaptfx-0.2.1/.github/workflows/build_publish.yml`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/.github/workflows/test_build_publish.yml` & `adaptfx-0.2.1/.github/workflows/test_build_publish.yml`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/.gitignore` & `adaptfx-0.2.1/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 
 # Translations
 *.mo
 *.pot
 
 # OS
 .DS_Store
+*.pdf
 
 # Django stuff:
 *.log
 local_settings.py
 db.sqlite3
 db.sqlite3-journal
```

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-1_1.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-1_1.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-1_2.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-1_2.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-1_3.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-1_3.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-1_4.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-1_4.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-1_5.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-1_5.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-1_planning.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-1_planning.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-2_1.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-2_1.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-2_2.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-2_2.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-2_3.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-2_3.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-2_4.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-2_4.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-2_5.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-2_5.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-2_planning.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-2_planning.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-3_1.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-3_1.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-3_2.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-3_2.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-3_3.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-3_3.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-3_4.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-3_4.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-3_5.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-3_5.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-3_planning.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-3_planning.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-4_1.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-4_1.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-4_2.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-4_2.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-4_3.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-4_3.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-4_4.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-4_4.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-4_5.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-4_5.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-4_planning.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-4_planning.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-5_1.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-5_1.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-5_2.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-5_2.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-5_3.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-5_3.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-5_4.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-5_4.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-5_5.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-5_5.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-5_planning.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-5_planning.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-6_1.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-6_1.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-6_2.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-6_2.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-6_3.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-6_3.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-6_4.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-6_4.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-6_5.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-6_5.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient-6_planning.jpg` & `adaptfx-0.2.1/DVH_figures/Patient-6_planning.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_10_1.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_10_1.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_10_2.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_10_2.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_10_3.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_10_3.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_10_4.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_10_4.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_10_5.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_10_5.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_10_planning.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_10_planning.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_11_1.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_11_1.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_11_2.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_11_2.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_11_3.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_11_3.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_11_4.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_11_4.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_11_5.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_11_5.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_11_planning.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_11_planning.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_12_1.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_12_1.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_12_2.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_12_2.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_12_3.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_12_3.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_12_4.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_12_4.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_12_5.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_12_5.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_12_planning.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_12_planning.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_13_1.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_13_1.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_13_2.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_13_2.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_13_3.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_13_3.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_13_4.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_13_4.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_13_5.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_13_5.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_13_planning.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_13_planning.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_14_1.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_14_1.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_14_2.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_14_2.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_14_3.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_14_3.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_14_4.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_14_4.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_14_5.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_14_5.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_14_planning.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_14_planning.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_15_1.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_15_1.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_15_2.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_15_2.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_15_3.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_15_3.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_15_4.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_15_4.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_15_5.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_15_5.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_15_planning.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_15_planning.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_16_1.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_16_1.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_16_2.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_16_2.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_16_3.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_16_3.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_16_4.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_16_4.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_16_5.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_16_5.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_16_planning.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_16_planning.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_7_1.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_7_1.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_7_2.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_7_2.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_7_3.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_7_3.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_7_4.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_7_4.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_7_5.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_7_5.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_7_planning.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_7_planning.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_8_1.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_8_1.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_8_2.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_8_2.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_8_3.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_8_3.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_8_4.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_8_4.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_8_5.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_8_5.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_8_planning.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_8_planning.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_9_1.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_9_1.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_9_2.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_9_2.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_9_3.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_9_3.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_9_4.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_9_4.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_9_5.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_9_5.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/DVH_figures/Patient_9_planning.jpg` & `adaptfx-0.2.1/DVH_figures/Patient_9_planning.jpg`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/GUI/2D_GUI.py` & `adaptfx-0.2.1/GUI/2D_GUI.py`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/GUI/3D_GUI.py` & `adaptfx-0.2.1/GUI/3D_GUI.py`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/GUI/gamma_distribution_preview.py` & `adaptfx-0.2.1/GUI/gamma_distribution_preview.py`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/GUI/helpers.py` & `adaptfx-0.2.1/GUI/helpers.py`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/GUI/interpol2D_OAR.py` & `adaptfx-0.2.1/GUI/interpol2D_OAR.py`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/GUI/interpol2D_OARminfrac.py` & `adaptfx-0.2.1/GUI/interpol2D_OARminfrac.py`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/GUI/interpol2D_tumor.py` & `adaptfx-0.2.1/GUI/interpol2D_tumor.py`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/GUI/interpol3D.py` & `adaptfx-0.2.1/GUI/interpol3D.py`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/LICENSE` & `adaptfx-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/MANUAL.md` & `adaptfx-0.2.1/MANUAL.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # The `adaptfx` manual
 
 ## Working tree
 
-One should perform calculations in a working folder e.g. `adaptfx/work`. There the instruction files can be specified by the user and `adaptfx` will automatically produce log files if the user wishes to.
+The package ships a CLI with which calculations can be performed which will be explained here. One should perform calculations in a working folder e.g. `adaptfx/work`. There the instruction files can be specified by the user and `adaptfx` will automatically produce log files if the user wishes to.
+
+The package also also provides a class that can be used in scripting mode. When using the package in scripts, a class creates an object with according attributes. To understand the attributes and behaviour of optimisation, read the doc-string of the `aft.py` script [here](src/adaptfx/aft.py)
 
 ## Format of the instruction file
 The user specifies following elements of the dictionary for the main entries: 
 - `"algorithm"`
 - `"debug"`
 - `"log"`
 - `"keys"`
@@ -90,15 +92,15 @@
 min_dose : float
     minimal physical doses to be delivered in one fraction.
     The doses are aimed at PTV 95.
     default: 0
 max_dose : float
     maximal physical doses to be delivered in one fraction.
     The doses are aimed at PTV 95. If -1 the dose is adapted to the
-    remaining dose tumor dose to be delivered or the remaining OAR dose 
+    remaining tumor BED to be delivered or the remaining OAR dose 
     allowed to be prescribed.
     default: -1
 ```
 
 ## Specific entries according to algorithm type
 
 ```
@@ -132,28 +134,90 @@
 sf_low : float
     lower bound of the possible sparing factors.
 sf_high : float
     upper bound of the possible sparing factors.
 sf_stepsize: float
     stepsize of the sparing factor stepsize.
 sf_prob_threshold': float
-    probability threshold of the sparing factor occuring.
+    probability threshold of the sparing factor occuring
+    which defines the range of sparing factors.
 inf_penalty : float
-    infinite penalty for certain undesired states.
+    define infinite penalty for undesired states
+    choose arbitrarily large compared to highest occuring reward.
 plot_policy : int
     starting from which fraction policy should be plotted.
 plot_values : int
     starting from which fraction value should be plotted.
 plot_remains : int
     starting from which fraction expected remaining number 
     of fractions should be plotted.
+plot_probability : int
+    flag if the probability distribution should be plotted
 ```
 
-# Example
+> :warning: Note:\
+> It is dangerous to use an upper and lower bound in `sf_low` and `sf_high`, as a truncated probability distribution may result that not accurately represents the environment model. Best is to set `sf_prob_threshold` to `1e-3` or lower or leave it at the default which is set at `1e-4`.
+
+## Note on Plots
+Policy, Value and Remaining number of fractions plots are calculated with the probability distribution in the fraction from which the plots should start. That is the value function that is known when iterating backwards through the fractions. E.g. the plotted policy starting to plot in the first fraction i.e `plot_policy = 1` and `prob_update = 0`  is the policy which is known throughout the treatment, when observing only the first sparing factor. In the case of probability updating e.g `prob_update = 1` the plotted policy is the optimal policy for the probability distribution known when observing the first sparing factor. As the probability distribution changes also future optimal policies change and one has to keep in mind only policy with the constant probability distribution from fraction `1` is plotted.
+
+Different is the probability plot: the probability is set for each fraction and updated with additional oberved sparing factors.
+
+# AFT CLI
 
-Outlined is an example instruction file for fraction minimisation. It simply is a `.json` that is translated into a python dictionary. An example can be found [here](work/oar_example.json)
+Outlined is an example instruction file for fraction minimisation. It simply is a `.json` that is translated into a python dictionary. An example can be found [here](work/example_0.json)
 
 This `.json` file can be called in with the CLI as:
 
 ```
 $ aft -f work/oar_example.json
+```
+
+# AST CLI
+There is also a second CLI that allows to plot sparing factors, policy functions, temporal Adaptive Fractionation Therapy etc.
+```
+$ ast [options] -f <simulation_file>
+```
+
+The entry for algorithm simulation type is
+
+```
+algorithm_simulation: histogram, fraction, single_state, all_state
+single_distance, single_patient, grid_distance, grid_fraction
+    allowed plots options
+keys_simulation: dict
+    simulation keys
+```
+
+```
+keys_simulation
+----------------
+# Histogram of applied AFT for sampled patients
+n_patients : float
+    stepsize of the actionspace.
+fixed_mean_sample : float
+    mean of sampled patient sparing factor
+fixed_std_sample : float
+    standard deviation of sampled patient sparing factor
+
+# Data related plots
+c_list : list
+    list of c parameters
+plot_index : int
+    which index to plot
+data_filepath : string
+    path to sparing factor file
+data_selection : list
+    two elements of header in sparing factor file
+data_row_hue : string
+    seaborn hue or row
+
+# Settings of plots
+figsize : list
+    two elements of size figure
+fontsize : float
+    fontsize of plots
+save : bool
+    boolean to instruct saving plot
+usetex : bool
+    boolean if TeX font should be used
 ```
```

### Comparing `adaptfx-0.2.0/PKG-INFO` & `adaptfx-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptfx
-Version: 0.2.0
+Version: 0.2.1
 Summary: Package for computing dose fractionation schemes in MR guided Adaptive Radiotherapy
 Author-email: Janic Tom Weber <janic.weber@uzh.ch>, Yoel Pérez Haas <yoel.perezhaas@uzh.ch>
 License: MIT
 Project-URL: source, https://github.com/openAFT/adaptfx
 Keywords: fractionation,adaptive radiotherapy,reinforcement-learning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -135,14 +135,18 @@
 ### GUI
 
 A last addition is made with graphical user interfaces that facilitate the use of the interpolation algorithms. There are two interfaces that can be run. In these interfaces all variables can be given to compute an adaptive fractionation plan for a patient. 
 
 > :warning: Note:\
 > The interfaces are not optimized, and thus it is not recommended using them to further develop extensions.
 
+### Reducing Number of Fractions
+
+For the 2D algorithms there exist the possibility to reduce number of fractions. A constant $c$ can be chosen which introduces a reward (or rather a cost) linear to the number of fractions used to finish the treatment. The cost is added to the immediate reward returned by the environment in the current fraction. There exist a simulative model helping to estimate what the constant $c$ should be chosen in order for the treatment to finish on some target number of fractions $n_{\text{targ}}$. The function can be found [here](src/adaptfx/radiobiology.py) in `c_calc`.
+
 ### Probability Updating
 
 The DP algorithm relies on a description of the environment to compute an optimal policy, in this case the probability distribution of the sparing factor $P(\delta)$, which we assume to be a Gaussian distribution truncated at $0$, with patient-specific parameters for mean and standard deviation. At the start of a treatment, only two sparing factors are available for that patient, from the planning scan and the first fraction. In each fraction, an additional sparing factor is measured, which can be used to calculate updated estimates $\mu_t$ and $\sigma_t$ for mean and standard deviation, respectively.
 
 #### No Updating
 
 In case where the probability is not updated the parameters $\mu_t$ and $\sigma_t$ of the normal distribution can be fixed.
@@ -184,20 +188,20 @@
       from _ctypes import Union, Structure, Array
 ImportError: No module named '_ctypes'
 ```
 
 **Solution:** with the specific package manager of the Linux distribution install `libffi-dev` development tool. E.g. in Fedora Linux and derivatives install this tool
 
 ```
-sudo dnf install libffi-devel
+$ sudo dnf install libffi-devel
 ```
 
 On Ubuntu:
 ```
-sudo apt install libffi-dev
+$ sudo apt install libffi-dev
 ```
 
 ### No GUI backend for `matplotlib`
 
 **Problem:** on Linux or MacOS it could be that once `aft` is run the plots are not shown and there is an error message:
 
 
@@ -206,27 +210,27 @@
   Could not find a version that satisfies the requirement tkinter (from versions: )
 No matching distribution found for tkinter
 ```
 
 **Solution:** on Fedora Linux and derivative distributions one could solve this by either installing python tkinter
 
 ```
-sudo dnf install python3-tkinter
+$ sudo dnf install python3-tkinter
 ```
 
 on Ubuntu
 
 ```
-sudo apt-get install python3-tk
+$ sudo apt-get install python3-tk
 ```
 
 **Solution:** on MacOS and Linux one could instead use `pip` to install `pyqt`
 
 ```
-pip install pyqt5
+$ pip install pyqt5
 ```
 
 
 ## References
 
 <a id="1">[1]</a>
 Yoel Samuel Pérez Haas et al.;
```

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_11_1.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_11_1.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_11_2.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_11_2.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_11_3.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_11_3.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_11_4.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_11_4.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_11_5.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_11_5.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_11_planning.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_11_planning.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_12_1.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_12_1.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_12_2.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_12_2.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_12_3.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_12_3.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_12_4.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_12_4.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_12_5.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_12_5.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_12_planning.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_12_planning.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_13_1.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_13_1.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_13_2.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_13_2.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_13_3.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_13_3.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_13_4.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_13_4.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_13_5.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_13_5.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_13_planning.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_13_planning.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_14_1.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_14_1.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_14_2.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_14_2.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_14_3.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_14_3.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_14_4.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_14_4.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_14_5.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_14_5.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_14_planning.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_14_planning.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_15_1.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_15_1.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_15_2.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_15_2.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_15_3.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_15_3.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_15_4.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_15_4.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_15_5.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_15_5.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_15_planning.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_15_planning.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_16_1.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_16_1.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_16_2.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_16_2.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_16_3.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_16_3.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_16_4.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_16_4.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_16_5.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_16_5.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_16_planning.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_16_planning.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_1_1.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_1_1.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_1_2.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_1_2.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_1_3.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_1_3.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_1_4.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_1_4.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_1_5.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_1_5.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_1_planning.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_1_planning.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_2_1.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_2_1.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_2_2.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_2_2.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_2_3.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_2_3.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_2_4.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_2_4.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_2_5.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_2_5.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_2_planning.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_2_planning.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_3_1.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_3_1.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_3_2.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_3_2.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_3_3.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_3_3.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_3_4.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_3_4.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_3_5.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_3_5.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_3_planning.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_3_planning.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_4_1.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_4_1.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_4_2.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_4_2.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_4_3.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_4_3.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_4_4.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_4_4.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_4_5.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_4_5.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_4_planning.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_4_planning.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_5_.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_5_.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_5_1.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_5_1.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_5_2.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_5_2.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_5_3.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_5_3.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_5_4.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_5_4.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_5_5.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_5_5.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_6_1.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_6_1.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_6_2.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_6_2.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_6_3.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_6_3.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_6_4.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_6_4.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_6_5.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_6_5.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_6_planning.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_6_planning.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_7_1.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_7_1.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_7_2.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_7_2.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_7_3.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_7_3.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_7_4.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_7_4.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_7_5.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_7_5.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_7_planning.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_7_planning.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_8_1.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_8_1.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_8_2.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_8_2.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_8_3.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_8_3.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_8_4.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_8_4.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_8_5.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_8_5.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_8_planning.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_8_planning.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_9_1.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_9_1.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_9_2.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_9_2.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_9_3.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_9_3.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_9_4.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_9_4.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_9_5.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_9_5.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/Patient_9_planning.csv` & `adaptfx-0.2.1/Patientdata_paper/Patient_9_planning.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/patient_10_1.csv` & `adaptfx-0.2.1/Patientdata_paper/patient_10_1.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/patient_10_2.csv` & `adaptfx-0.2.1/Patientdata_paper/patient_10_2.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/patient_10_3.csv` & `adaptfx-0.2.1/Patientdata_paper/patient_10_3.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/patient_10_4.csv` & `adaptfx-0.2.1/Patientdata_paper/patient_10_4.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/patient_10_5.csv` & `adaptfx-0.2.1/Patientdata_paper/patient_10_5.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/Patientdata_paper/patient_10_planning.csv` & `adaptfx-0.2.1/Patientdata_paper/patient_10_planning.csv`

 * *Files identical despite different names*

### Comparing `adaptfx-0.2.0/README.md` & `adaptfx-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -120,14 +120,18 @@
 ### GUI
 
 A last addition is made with graphical user interfaces that facilitate the use of the interpolation algorithms. There are two interfaces that can be run. In these interfaces all variables can be given to compute an adaptive fractionation plan for a patient. 
 
 > :warning: Note:\
 > The interfaces are not optimized, and thus it is not recommended using them to further develop extensions.
 
+### Reducing Number of Fractions
+
+For the 2D algorithms there exist the possibility to reduce number of fractions. A constant $c$ can be chosen which introduces a reward (or rather a cost) linear to the number of fractions used to finish the treatment. The cost is added to the immediate reward returned by the environment in the current fraction. There exist a simulative model helping to estimate what the constant $c$ should be chosen in order for the treatment to finish on some target number of fractions $n_{\text{targ}}$. The function can be found [here](src/adaptfx/radiobiology.py) in `c_calc`.
+
 ### Probability Updating
 
 The DP algorithm relies on a description of the environment to compute an optimal policy, in this case the probability distribution of the sparing factor $P(\delta)$, which we assume to be a Gaussian distribution truncated at $0$, with patient-specific parameters for mean and standard deviation. At the start of a treatment, only two sparing factors are available for that patient, from the planning scan and the first fraction. In each fraction, an additional sparing factor is measured, which can be used to calculate updated estimates $\mu_t$ and $\sigma_t$ for mean and standard deviation, respectively.
 
 #### No Updating
 
 In case where the probability is not updated the parameters $\mu_t$ and $\sigma_t$ of the normal distribution can be fixed.
@@ -169,20 +173,20 @@
       from _ctypes import Union, Structure, Array
 ImportError: No module named '_ctypes'
 ```
 
 **Solution:** with the specific package manager of the Linux distribution install `libffi-dev` development tool. E.g. in Fedora Linux and derivatives install this tool
 
 ```
-sudo dnf install libffi-devel
+$ sudo dnf install libffi-devel
 ```
 
 On Ubuntu:
 ```
-sudo apt install libffi-dev
+$ sudo apt install libffi-dev
 ```
 
 ### No GUI backend for `matplotlib`
 
 **Problem:** on Linux or MacOS it could be that once `aft` is run the plots are not shown and there is an error message:
 
 
@@ -191,27 +195,27 @@
   Could not find a version that satisfies the requirement tkinter (from versions: )
 No matching distribution found for tkinter
 ```
 
 **Solution:** on Fedora Linux and derivative distributions one could solve this by either installing python tkinter
 
 ```
-sudo dnf install python3-tkinter
+$ sudo dnf install python3-tkinter
 ```
 
 on Ubuntu
 
 ```
-sudo apt-get install python3-tk
+$ sudo apt-get install python3-tk
 ```
 
 **Solution:** on MacOS and Linux one could instead use `pip` to install `pyqt`
 
 ```
-pip install pyqt5
+$ pip install pyqt5
 ```
 
 
 ## References
 
 <a id="1">[1]</a>
 Yoel Samuel Pérez Haas et al.;
```

### Comparing `adaptfx-0.2.0/pyproject.toml` & `adaptfx-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,17 @@
     "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "numpy == 1.24.1",
     "scipy == 1.10.0",
     "matplotlib == 3.6.3",
-    "pyqt6 == 6.4.0"
+    "pyqt6 == 6.4.0",
+    "pandas==1.5.2",
+    "seaborn==0.12.2"
 ]
 dynamic = ["version"]
 
 [project.urls]
 source = "https://github.com/openAFT/adaptfx"
 
 
@@ -43,7 +45,8 @@
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["*"]
 
 [project.scripts]
 aft = "adaptfx.aft:main"
+ast = "adaptsim.ast:main"
```

### Comparing `adaptfx-0.2.0/src/adaptfx/__init__.py` & `adaptfx-0.2.1/src/adaptfx/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .aft_utils import *
 from .aft import RL_object
 from .maths import *
 from .planning import *
 from .radiobiology import *
 from .visualiser import *
 from .reinforce import *
-from .reinforce_old import *
+from .reinforce_old import max_tumor_bed_old, min_oar_bed_old, min_oar_max_tumor_old
 
 __all__ = ['bed_calc_matrix',
             'convert_to_physical',
             'multiple',
             'visualiser',
             'min_oar_bed',
             'min_n_frac',
```

### Comparing `adaptfx-0.2.0/src/adaptfx/aft_prompt.py` & `adaptfx-0.2.1/src/adaptfx/aft_prompt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 import sys
 import logging
-import os
+import adaptfx as afx
 
 prompt = 'AFT> '
 empty = ''
 
-def logging_init(filename, log, level):
+def logging_init(basename, log, level):
     """
     log initialisation to write to filename
 
     Parameters
     ----------
-    filename : string
-        filename of log file
+    basename : string
+        filename of log file without suffix
     log : bool
         if true store log to filename
     debug: bool
         if true log extensive message
 
     Returns
     -------
@@ -34,32 +34,15 @@
         log_level = logging.INFO
     elif level == 2:
         format_file = '%(asctime)s [%(levelname)s]: %(message)s'
         format_out = '[%(levelname)s]: %(message)s'
         log_level = logging.ERROR
     
     if log:
-        logfile_extension = "log"
-        # create logfile name
-        # get the basename before .json extension
-        basename = filename.rsplit('.')[0]
-        # search for existing filename ...
-        i = 1
-        while os.path.exists(f'{basename}_{i}.{logfile_extension}'):
-            # exponential search if many files exist
-            i *= 2
-        a, b = (i // 2, i)
-        while a+1 < b:
-            c = (a + b) // 2
-            if os.path.exists(f'{basename}_{c}.{logfile_extension}'):
-                a, b = (c, b)
-            else:
-                a, b = (a, c)
-        # ... end of search
-        log_filename = f'{basename}_{b}.{logfile_extension}'
+        log_filename = afx.create_name(basename, "log")
         logging.basicConfig(
             format=format_file,
             level=log_level, 
             datefmt='%d-%m-%Y %H:%M:%S',
             handlers=[
                 logging.FileHandler(log_filename),
                 logging.StreamHandler(sys.stdout)
```

### Comparing `adaptfx-0.2.0/src/adaptfx/constants.py` & `adaptfx-0.2.1/src/adaptfx/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # -*- coding: utf-8 -*-
 # log settings
-LOG_BOOL = 0
-LOG_BOOL_LIST = [0,1]
-LOG_LEVEL = 1
-LOG_LEVEL_LIST = [0,1,2]
+LOG_BOOL = 0            # no logging to file
+LOG_BOOL_LIST = [0,1]   # options for logging
+LOG_LEVEL = 1           # logging level middle
+LOG_LEVEL_LIST = [0,1,2]# options for logging level
 
 # dose, sf
 DOSE_STEPSIZE = 0.1
 STATE_STEPSIZE = 1
 SF_LOW = 0
 SF_HIGH = 1.7
 SF_STEPSIZE = 0.01
-SF_PROB_THRESHOLD = 1e-5
+SF_PROB_THRESHOLD = 1e-4
 INF_PENALTY = 1e4
 
 # keys
 ALPHA_BETA_TUMOR = 10
 ALPHA_BETA_OAR = 3
 
-FULL_DICT = {'number_of_fractions':None,
+# "None" are mandatory keys
+FULL_DICT = {'number_of_fractions': None,
         'fraction': 0,
         'sparing_factors': None,
-        'prob_update': 0,
+        'prob_update': None,
         'fixed_mean': None,
         'fixed_std': None,
         'shape': None,
         'scale': None,
         'shape_inv': None,
         'scale_inv': None,
         'tumor_goal': None,
@@ -46,14 +47,16 @@
         'sf_high': SF_HIGH,
         'sf_stepsize': SF_STEPSIZE,
         'sf_prob_threshold': SF_PROB_THRESHOLD,
         'inf_penalty': INF_PENALTY,
         'plot_policy': 0,
         'plot_values': 0,
         'plot_remains': 0,
+        'plot_probability': 0,
+        'save_plot': 0,
         }
 
 STANDARD_LIST = [
         'number_of_fractions',
         'fraction',
         'sparing_factors',
         'prob_update',
@@ -67,21 +70,22 @@
         'abn',
         'accumulated_oar_dose',
         'accumulated_tumor_dose',
         'min_dose',
         'max_dose',
         ]
 
+# define the list for each optimisation method
 OAR_LIST = STANDARD_LIST + ['tumor_goal']
 
-TUMOR_LIST = STANDARD_LIST + ['oar_limit']
+TUMOR_LIST = STANDARD_LIST + ['oar_limit', 'c']
 
 FRAC_LIST = STANDARD_LIST + ['tumor_goal', 'c']
 
 TUMOR_OAR_LIST = STANDARD_LIST + ['tumor_goal', 'oar_limit']
 
 KEY_DICT = {
         'oar': OAR_LIST, 'oar_old': OAR_LIST, 
         'tumor': TUMOR_LIST, 'tumor_old': TUMOR_LIST,
-        'frac': FRAC_LIST, 'frac_old': FRAC_LIST,
+        'frac': FRAC_LIST,
         'tumor_oar': TUMOR_OAR_LIST, 'tumor_oar_old': TUMOR_OAR_LIST
         }
```

### Comparing `adaptfx-0.2.0/src/adaptfx/maths.py` & `adaptfx-0.2.1/src/adaptfx/maths.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Returns
     -------
     scipy.stats._distn_infrastructure.rv_frozen
         distribution function
 
     """
     normal = truncnorm((low - mean) / std, (upp - mean) / std,
-                        loc=mean, scale=std)
+        loc=mean, scale=std)
 
     return normal
 
 def student_t(sf_observed, shape_inv, scale_inv):
     """
     Function for probability updating:
     Computes a posterior predictive sparing factor distribution
@@ -139,16 +139,16 @@
     # create sample sparing factor array
     sample_sf = np.arange(sf_low, sf_high + sf_stepsize, sf_stepsize)
     n_samples = len(sample_sf)
 
     # sum probability density from cumulative density function in interval
     # to get probability
     half_interval = sf_stepsize/2
-    upp_bound = (half_interval - sf_stepsize*1e-6) * np.ones(n_samples)
-    low_bound = half_interval * np.ones(n_samples)
+    upp_bound = (half_interval - sf_stepsize*1e-6)
+    low_bound = half_interval
     prob = X.cdf(sample_sf + upp_bound) - X.cdf(sample_sf - low_bound)
 
      # get rid of all probabilities below given threshold
     probability = prob[prob > probability_threshold]
     sf = sample_sf[prob > probability_threshold]
     return [sf, probability]
```

### Comparing `adaptfx-0.2.0/src/adaptfx/planning.py` & `adaptfx-0.2.1/src/adaptfx/planning.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,37 +18,48 @@
         keys = afx.DotDict(keys)
 
     if isinstance(sets, dict):
         # check if keys is a dictionary from manual user
         sets = afx.DotDict(sets)
 
     if keys.fraction != 0:
-        # if only a specific fraction should be calculated
-        fractions_list = np.array([keys.fraction])
-        physical_doses = np.zeros(1)
-        tumor_doses = np.zeros(1)
-        oar_doses = np.zeros(1)
+        # if only up to a specific fraction should be calculated
+        fractions_list = np.arange(1, keys.fraction + 1, 1)
+        physical_doses = np.zeros(keys.fraction)
+        tumor_doses = np.zeros(keys.fraction)
+        oar_doses = np.zeros(keys.fraction)
     else:
         # for calculation whole treatment in retrospect
         fractions_list = np.arange(1, keys.number_of_fractions + 1, 1)
         physical_doses = np.zeros(keys.number_of_fractions)
         tumor_doses = np.zeros(keys.number_of_fractions)
         oar_doses = np.zeros(keys.number_of_fractions)
+    
+    if sets.plot_probability:
+        # create lists for storing probability distribution
+        # note that the shape of probability distribution
+        # is 1) unknown and 2) non-constant --> use list
+        sf = []
+        pdf = []
 
+    # create array for keeping track of fractions
+    plot_numbering = np.arange(1, keys.number_of_fractions + 1, 1)
     first_tumor_dose = keys.accumulated_tumor_dose
     first_oar_dose = keys.accumulated_oar_dose
 
     output_whole = afx.DotDict({})
 
     for i, keys.fraction in enumerate(fractions_list):
         keys.sparing_factors_public = keys.sparing_factors[0 : keys.fraction + 1]
         if algorithm == 'oar':
             output = afx.min_oar_bed(keys, sets)
         elif algorithm == 'frac':
             output = afx.min_n_frac(keys, sets)
+        elif algorithm == 'tumor':
+            output = afx.max_tumor_bed(keys, sets)
             
         elif algorithm == 'oar_old':
             output = afx.min_oar_bed_old(keys, sets)
         elif algorithm == 'frac_old':
             output = afx.min_n_frac_old(keys, sets)
         elif algorithm == 'tumor_old':
             output = afx.max_tumor_bed_old(keys, sets)
@@ -62,26 +73,35 @@
         oar_doses[i] = output.oar_dose
 
         keys.accumulated_tumor_dose = np.nansum(tumor_doses) + first_tumor_dose
         keys.accumulated_oar_dose = np.nansum(oar_doses) + first_oar_dose
 
         # user specifies to plot policy number, if equal to fraction plot
         # if both zero than the user doesn't want to plot policy
+        if sets.plot_probability:
+            sf.append(list(output.probability.sf))
+            pdf.append(list(output.probability.pdf))
         if sets.plot_policy == keys.fraction:
             output_whole.policy = output.policy
-            output_whole.policy.fractions = fractions_list[sets.plot_policy - 1:]
+            output_whole.policy.fractions = plot_numbering[sets.plot_policy - 1:]
         if sets.plot_values == keys.fraction:
             output_whole.value = output.value
-            output_whole.value.fractions = fractions_list[sets.plot_values - 1:]
+            output_whole.value.fractions = plot_numbering[sets.plot_values - 1:]
         if sets.plot_remains == keys.fraction:
             output_whole.remains = output.remains
-            output_whole.remains.fractions = fractions_list[sets.plot_remains - 1:]
+            output_whole.remains.fractions = plot_numbering[sets.plot_remains - 1:]
 
     # store doses
     exponent = afx.find_exponent(sets.dose_stepsize) - 1
     [output_whole.physical_doses, output_whole.tumor_doses, output_whole.oar_doses] = np.around(
         [physical_doses, tumor_doses, oar_doses], -exponent)
     output_whole.oar_sum, output_whole.tumor_sum = np.around(
         [np.nansum(oar_doses), np.nansum(tumor_doses)], -exponent)
     output_whole.fractions_used = np.count_nonzero(~np.isnan(output_whole.physical_doses))
+    if sets.plot_probability:
+        # store probability distribution
+        output_whole.probability = {}
+        output_whole.probability.sf = sf
+        output_whole.probability.pdf = pdf
+        output_whole.probability.fractions = fractions_list
 
     return output_whole
```

### Comparing `adaptfx-0.2.0/src/adaptfx/reinforce.py` & `adaptfx-0.2.1/src/adaptfx/reinforce.py`

 * *Files 24% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     c = keys.c
     abt = keys.abt
     abn = keys.abn
     min_dose = keys.min_dose
     max_dose = keys.max_dose
     # ---------------------------------------------------------------------- #
     # check in which fraction data should be returned for plotting
+    probability_plot = 1 if sets.plot_probability else 0
     policy_plot = 1 if sets.plot_policy == fraction else 0
     values_plot = 1 if sets.plot_values == fraction else 0
     remains_plot = 1 if sets.plot_remains == fraction else 0
 
     # prepare distribution
     actual_sf = sparing_factors_public[fraction]
     if prob_update == 0:
@@ -129,19 +130,17 @@
             # state is the actual fraction to calculate
             # e.g. in the first fraction_state there is no prior dose delivered
             # and future_bedt is equal to bedt_space
             future_values_discrete = (values[fraction_index + 1] * prob).sum(axis=1)
             future_bedt = accumulated_tumor_dose + bedt_space
             future_bedt = np.where(future_bedt > tumor_goal, tumor_limit, future_bedt)
             c_penalties = np.where(np.round(future_bedt, -exp) < tumor_goal, -c, 0)
-            # for discrete matching
-            # future_values = future_values_discrete[np.where(np.isclose(bedt_states, future_bedt))]
             future_values = afx.interpolate(future_bedt, bedt_states, future_values_discrete)
             vs = -bedn_space + future_values + c_penalties
-            # argmax of vs along axis 0 to find best action fot the actual sf
+            # argmax of vs along axis 0 to find best action for the actual sf
             action_index = vs.argmax(axis=0)
 
             if policy_plot or values_plot or remains_plot:
                 # for the policy plot
                 future_bedt_full = bedt_states.reshape(n_bedt_states, 1) + bedt_space
                 future_bedt_full = np.where(future_bedt_full > tumor_goal, tumor_limit, future_bedt_full)
                 c_penalties_full = np.where(future_bedt_full < tumor_goal, -c, 0).reshape(n_bedt_states, n_action, 1)
@@ -183,21 +182,21 @@
             # this smooths out the penalties in underdose and overdose regions
             bedt_diff = np.round(bedt_states + last_bed_actions - tumor_goal, -exp)
             penalties = np.where(bedt_diff == 0, 0, -np.abs(bedt_diff) * sets.inf_penalty)
             # to each best action add the according penalties
             # penalties need to be reshaped for broadcasting
             vs = -last_bedn + penalties.reshape(n_bedt_states, 1)
             values[fraction_index] = vs
-            # ensure that for the goal reached the value/poliy is zero (min_dose)
+            # ensure that for the goal reached the value/policy is zero (min_dose)
             values[fraction_index][bedt_states==tumor_goal] = 0
 
             if policy_plot:
                 # policy calculation for each bedt, but sf is not considered
                 policy[fraction_index] += last_bed_actions.reshape(n_bedt_states, 1)
-                # ensure that for the goal reached the value/poliy is zero (min_dose)
+                # ensure that for the goal reached the value/policy is zero (min_dose)
                 policy[fraction_index][bedt_states==tumor_goal] = 0
 
         elif fraction_state != number_of_fractions:
             # every other state but the last
             # this calculates the value function in the future fractions
             future_values_discrete = (values[fraction_index + 1] * prob).sum(axis=1)
             # bedt_states is reshaped such that numpy broadcast leads to 2D array
@@ -206,15 +205,15 @@
             future_values = afx.interpolate(future_bedt, bedt_states, future_values_discrete)
             c_penalties = np.where(future_bedt < tumor_goal, -c, 0).reshape(n_bedt_states, n_action, 1)
             # dim(bedn_sf_space)=(1,n_action,n_sf),dim(future_values)=(n_states,n_action)
             # every row of values_penalties is transposed and copied n_sf times
             vs = -bedn_sf_space + future_values.reshape(n_bedt_states, n_action, 1) + c_penalties
             # check vs along the sf axis
             values[fraction_index] = vs.max(axis=1)
-            # ensure that for the goal reached the value/poliy is zero (min_dose)
+            # ensure that for the goal reached the value/policy is zero (min_dose)
             values[fraction_index][bedt_states==tumor_goal] = 0
 
             if policy_plot or remains_plot:
                 current_policy = bedt_space[vs.argmax(axis=1)]
                 # ensure that for the goal reached the value/policy is zero (min_dose)
                 current_policy[bedt_states == tumor_goal] = 0
                 future_remains_discrete = (remains[fraction_index + 1] * prob).sum(axis=1)
@@ -227,24 +226,270 @@
 
     output = afx.DotDict({})
 
     output.physical_dose = actionspace[action_index] if not finished else np.nan
     output.tumor_dose = bedt_space[action_index] if not finished else np.nan
     output.oar_dose = bedn_space[action_index] if not finished else np.nan
 
+    if probability_plot:
+        output.probability = {}
+        output.probability.sf = sf
+        output.probability.pdf = rv.pdf(sf)
+    if policy_plot:
+        output.policy = {}
+        output.policy.val = policy
+        output.policy.sf = sf
+        output.policy.states = bedt_states
+    if values_plot:
+        output.value = {}
+        output.value.val = values
+        output.value.sf = sf
+        output.value.states = bedt_states
+    if remains_plot:
+        output.remains = {}
+        output.remains.val = remains
+        output.remains.sf = sf
+        output.remains.states = bedt_states
+
+    return output
+
+
+def max_tumor_bed(keys, sets=afx.SETTING_DICT):
+    # check if keys is a dictionary from manual user
+    if isinstance(keys, dict):
+        keys = afx.DotDict(keys)
+
+    if isinstance(sets, dict):
+        sets = afx.DotDict(sets)
+
+    fraction = keys.fraction
+    number_of_fractions = keys.number_of_fractions
+    accumulated_oar_dose = keys.accumulated_oar_dose
+    sparing_factors_public = keys.sparing_factors_public
+    prob_update = keys.prob_update
+    fixed_mean = keys.fixed_mean
+    fixed_std = keys.fixed_std
+    shape = keys.shape
+    scale = keys.scale
+    shape_inv = keys.shape_inv
+    scale_inv = keys.scale_inv
+    oar_limit = keys.oar_limit
+    c = keys.c
+    abt = keys.abt
+    abn = keys.abn
+    min_dose = keys.min_dose
+    max_dose = keys.max_dose
+    # ---------------------------------------------------------------------- #
+    # check in which fraction data should be returned for plotting
+    probability_plot = 1 if sets.plot_probability else 0
+    policy_plot = 1 if sets.plot_policy == fraction else 0
+    values_plot = 1 if sets.plot_values == fraction else 0
+    remains_plot = 1 if sets.plot_remains == fraction else 0
+
+    # prepare distribution
+    actual_sf = sparing_factors_public[fraction]
+    if prob_update == 0:
+        # fixed normal distribution for sparing factor
+        mean = fixed_mean
+        std = fixed_std
+        rv = afx.truncated_normal(mean, std, sets.sf_low, sets.sf_high)
+    elif prob_update == 1:
+        # update normal distribution with gamma prior
+        mean = np.mean(sparing_factors_public)
+        std = afx.std_posterior(sparing_factors_public, shape, scale)
+        rv = afx.truncated_normal(mean, std, sets.sf_low, sets.sf_high)
+    elif prob_update == 2:
+        # update distribution with inverse-gamma prior
+        # posterior predictive distribution is student-t distribution
+        rv = afx.student_t(sparing_factors_public, shape_inv, scale_inv)
+    else:
+        afx.aft_error('invalid "prob_update" key was set', nme)
+    # initialise distribution from random variable (rv)
+    [sf, prob] = afx.sf_probdist(rv, sets.sf_low, sets.sf_high,
+        sets.sf_stepsize, sets.sf_prob_threshold)
+    n_sf = len(sf)
+
+    # actionspace
+    exp = afx.find_exponent(sets.dose_stepsize)
+    accumulated_oar_dose = np.round(accumulated_oar_dose, -exp)
+    remaining_bed = np.round(oar_limit - accumulated_oar_dose, -exp)
+    n_bedsteps = int(np.round(remaining_bed / sets.dose_stepsize, 0))
+    n_statesteps = int(np.round(remaining_bed / sets.state_stepsize, 0))
+
+    # automatic max_dose calculation
+    if max_dose == -1:
+        max_dose = remaining_bed
+    # Reduce max_dose to prohibit tumor_goal overshoot (efficiency)
+    max_dose = min(max_dose, remaining_bed)
+
+    # actionspace in bed dose
+    # pre calculation
+    bedn_space_pre = np.linspace(0, remaining_bed, n_bedsteps + 1)
+    actionspace_pre = afx.convert_to_physical(bedn_space_pre, abn, actual_sf)
+    bedt_space_pre = afx.bed_calc0(actionspace_pre, abt)
+    range_action = (bedn_space_pre >= min_dose) & (bedn_space_pre <= max_dose)
+    if range_action.any():
+        # check if actionspace is empty
+        bedn_space = bedn_space_pre[range_action]
+        actionspace = actionspace_pre[range_action]
+        bedt_space = bedt_space_pre[range_action]
+        n_action = len(bedn_space)
+        bedn_space_sf = np.zeros((1, n_sf)) + bedn_space.reshape(n_action, 1)
+        # bed_space to relate actionspace to oar- and tumor-dose
+        actionspace_sf = afx.convert_to_physical(bedn_space.reshape(n_action, 1), abn, sf)
+    else:
+        bedn_space_sf = np.zeros((1, n_sf)) + np.array([min_dose])
+        actionspace_sf = afx.convert_to_physical(bedn_space_sf, abn, sf)
+        n_action = 1
+    bedt_space_sf = afx.bed_calc0(actionspace_sf, abt)
+
+    # tumor bed states for tracking dose
+    oar_upper_bound = oar_limit + sets.state_stepsize
+    # include at least one more step for bedt
+    # define number of bed_dose steps to fulfill stepsize
+    bedn_states = np.linspace(accumulated_oar_dose,
+        oar_limit, n_statesteps + 1)
+    remaining_states = bedn_states - accumulated_oar_dose
+    n_bedn_states = len(bedn_states)
+    
+    # values matrix
+    # dim(values) = dim(policy) = fractions_remaining * bedt * sf
+    n_remaining_fractions = number_of_fractions - fraction
+    values = np.zeros((n_remaining_fractions + 1, n_bedn_states, n_sf))
+    if policy_plot or values_plot or remains_plot:
+        policy = np.zeros((n_remaining_fractions + 1, n_bedn_states, n_sf))
+        remains = np.zeros((n_remaining_fractions + 1, n_bedn_states, n_sf))
+    
+    finished = False
+    # ------------------------------------------------------------------------------------- #
+    remaining_fractions = np.arange(number_of_fractions, fraction - 1, -1)
+    remaining_index = remaining_fractions - fraction
+    # note that lowest fraction_state is one not zero
+    # and remaining_index counts in python indices
+    for fraction_index, fraction_state in zip(remaining_index, remaining_fractions):
+        if remaining_bed <= 0:
+            finished = True
+            break
+
+        elif fraction_state == fraction and fraction != number_of_fractions:
+            # state is the actual fraction to calculate
+            # e.g. in the first fraction_state there is no prior dose delivered
+            # and future_bedt is equal to bedt_space
+            future_values_discrete = (values[fraction_index + 1] * prob).sum(axis=1)
+            future_bedn = accumulated_oar_dose + bedn_space
+            future_bedn = np.where(future_bedn > oar_limit, oar_upper_bound, future_bedn)
+            c_penalties = np.where(np.round(future_bedn, -exp) < oar_limit, -c, 0)
+            future_values = afx.interpolate(future_bedn, bedn_states, future_values_discrete)
+            vs = bedt_space + future_values + c_penalties
+            # argmax of vs along axis 0 to find best action for the actual sf
+            action_index = vs.argmax(axis=0)
+
+            if policy_plot or values_plot or remains_plot:
+                # for the policy plot
+                future_bedn_full = bedn_states.reshape(n_bedn_states, 1, 1) + bedn_space_sf.reshape(1, n_action, n_sf)
+                future_bedn_full = np.where(future_bedn_full > oar_limit, oar_upper_bound, future_bedn_full)
+                c_penalties_full = np.where(future_bedn_full < oar_limit, -c, 0)
+                future_values_full = afx.interpolate(future_bedn_full, bedn_states, future_values_discrete)
+                vs_full = bedt_space_sf.reshape(1, n_action, n_sf) + future_values_full + c_penalties_full
+                # check vs along the sf axis
+                current_policy = bedn_space[vs_full.argmax(axis=1)]
+                # ensure that for the goal reached the value/policy is zero (min_dose)
+                current_policy[bedn_states == oar_limit] = 0
+                future_remains_discrete = (remains[fraction_index + 1] * prob).sum(axis=1)
+                future_bedn_opt = current_policy + bedn_states.reshape(n_bedn_states, 1)
+                future_remains = afx.interpolate(future_bedn_opt, bedn_states, future_remains_discrete)
+                current_remains = np.where((current_policy - remaining_states[::-1].reshape(n_bedn_states, 1)) >= 0, 0, 1)
+                # write to arrays
+                policy[fraction_index] = current_policy
+                values[fraction_index] = vs_full.max(axis=1)
+                remains[fraction_index] = current_remains + future_remains
+
+        elif fraction == number_of_fractions:
+            # in the last fraction value is not relevant
+            # max_dose is the already calculated remaining dose
+            # this should compensate the discretisation of the state space
+            action_index = np.abs(remaining_bed - bedn_space).argmin()
+            
+            if policy_plot:
+                policy[fraction_index][0] = bedn_space[action_index]
+
+        elif fraction_state == number_of_fractions:
+            # final state to initialise terminal reward
+            # dose remaining to be delivered, this is the actionspace in bedt
+            last_bed_actions = np.round(oar_limit - bedn_states, -exp)
+            # cut the actionspace to min and max dose constraints
+            last_bed_actions = np.where(last_bed_actions < min_dose, min_dose, last_bed_actions)
+            last_bed_actions = np.where(last_bed_actions > max_dose, max_dose, last_bed_actions)
+            last_bed_actions_reshaped = last_bed_actions.reshape(n_bedn_states, 1)
+            last_actions = afx.convert_to_physical(last_bed_actions_reshaped, abn, sf)
+            last_bedt = afx.bed_calc0(last_actions, abt)
+            # this smooths out the penalties in underdose and overdose regions
+            bedn_diff = np.round(bedn_states.reshape(n_bedn_states, 1) + last_bed_actions_reshaped - oar_limit, -exp)
+            penalties = np.where(bedn_diff == 0, 0, -np.abs(bedn_diff) * sets.inf_penalty)
+            # to each best action add the according penalties
+            # penalties need to be reshaped for broadcasting
+            vs = last_bedt + penalties
+            values[fraction_index] = vs
+            # ensure that for the goal reached the value/policy is zero (min_dose)
+            values[fraction_index][bedn_states==oar_limit] = 0
+
+            if policy_plot:
+                # policy calculation for each bedt, but sf is not considered
+                policy[fraction_index] += last_bed_actions_reshaped
+                # ensure that for the goal reached the value/policy is zero (min_dose)
+                policy[fraction_index][bedn_states==oar_limit] = 0
+
+        elif fraction_state != number_of_fractions:
+            # every other state but the last
+            # this calculates the value function in the future fractions
+            future_values_discrete = (values[fraction_index + 1] * prob).sum(axis=1)
+            # bedt_states is reshaped such that numpy broadcast leads to 2D array
+            future_bedn = bedn_states.reshape(n_bedn_states, 1, 1) + bedn_space_sf.reshape(1, n_action, n_sf)
+            future_bedn = np.where(future_bedn > oar_limit, oar_upper_bound, future_bedn)
+            future_values = afx.interpolate(future_bedn, bedn_states, future_values_discrete)
+            c_penalties = np.where(future_bedn < oar_limit, -c, 0)
+            # dim(bedn_sf_space)=(1,n_action,n_sf),dim(future_values)=(n_states,n_action)
+            # every row of values_penalties is transposed and copied n_sf times
+            vs = bedt_space_sf.reshape(1, n_action, n_sf) + future_values + c_penalties
+            # check vs along the sf axis
+            values[fraction_index] = vs.max(axis=1)
+            # ensure that for the goal reached the value/policy is zero (min_dose)
+            values[fraction_index][bedn_states==oar_limit] = 0
+
+            if policy_plot or remains_plot:
+                current_policy = bedn_space[vs.argmax(axis=1)]
+                # ensure that for the goal reached the value/policy is zero (min_dose)
+                current_policy[bedn_states == oar_limit] = 0
+                future_remains_discrete = (remains[fraction_index + 1] * prob).sum(axis=1)
+                future_bedn_opt = current_policy + bedn_states.reshape(n_bedn_states, 1)
+                future_remains = afx.interpolate(future_bedn_opt, bedn_states, future_remains_discrete)
+                current_remains = np.where((current_policy - remaining_states[::-1].reshape(n_bedn_states, 1)) >= 0, 0, 1)
+                # write to arrays
+                policy[fraction_index] = current_policy
+                remains[fraction_index] = current_remains + future_remains
+
+    output = afx.DotDict({})
+    output.physical_dose = actionspace[action_index] if not finished else np.nan
+    output.tumor_dose = bedt_space[action_index] if not finished else np.nan
+    output.oar_dose = bedn_space[action_index] if not finished else np.nan
+
+    if probability_plot:
+        output.probability = {}
+        output.probability.sf = sf
+        output.probability.pdf = rv.pdf(sf)
     if policy_plot:
         output.policy = {}
         output.policy.val = policy
         output.policy.sf = sf
-        output.policy.states = remaining_states
+        output.policy.states = bedn_states
     if values_plot:
         output.value = {}
         output.value.val = values
         output.value.sf = sf
-        output.value.states = remaining_states
+        output.value.states = bedn_states
     if remains_plot:
         output.remains = {}
         output.remains.val = remains
         output.remains.sf = sf
-        output.remains.states = remaining_states
+        output.remains.states = bedn_states
 
     return output
```

### Comparing `adaptfx-0.2.0/src/adaptfx/reinforce_old.py` & `adaptfx-0.2.1/src/adaptfx/reinforce_old.py`

 * *Files 12% similar despite different names*

```diff
@@ -61,34 +61,34 @@
 
 
 def min_oar_bed_old(keys, sets=SETTING_DICT):
     fraction = keys.fraction
     number_of_fractions = keys.number_of_fractions
     accumulated_tumor_dose = keys.accumulated_tumor_dose
     sparing_factors_public = keys.sparing_factors_public
-    alpha = keys.alpha
-    beta = keys.beta
+    shape = keys.shape
+    scale = keys.scale
     tumor_goal = keys.tumor_goal
     abt = keys.abt
     abn = keys.abn
     min_dose = keys.min_dose
     max_dose = keys.max_dose
-    fixed_prob = keys.fixed_prob
+    prob_update = keys.prob_update
     fixed_mean = keys.fixed_mean
     fixed_std = keys.fixed_std
     # ---------------------------------------------------------------------- #
     # check in which fraction policy should be returned
     policy_plot = 1 if sets.plot_policy == fraction else 0
 
-    if fixed_prob != 1:
+    if prob_update == 1:
         mean = np.mean(
             sparing_factors_public
         )  # extract the mean and std to setup the sparingfactor distribution
-        standard_deviation = std_posterior(sparing_factors_public, alpha, beta)
-    if fixed_prob == 1:
+        standard_deviation = std_posterior(sparing_factors_public, shape, scale)
+    elif prob_update == 0:
         mean = fixed_mean
         standard_deviation = fixed_std
     X = truncated_normal(mean, standard_deviation, sets.sf_low, sets.sf_high)
     bedt_states = np.arange(accumulated_tumor_dose, tumor_goal, 1)
     bedt_states = np.concatenate(
         (bedt_states, [tumor_goal, tumor_goal + 1])
     )  # add an extra step outside of our prescribed tumor dose which will be penalised to make sure that we aim at the prescribe tumor dose
@@ -220,228 +220,41 @@
     return output
 
 
 
 
 
 
-def min_n_frac_old(keys, sets=SETTING_DICT):
-    fraction = keys.fraction
-    number_of_fractions = keys.number_of_fractions
-    accumulated_tumor_dose = keys.accumulated_tumor_dose
-    sparing_factors_public = keys.sparing_factors_public
-    alpha = keys.alpha
-    beta = keys.beta
-    tumor_goal = keys.tumor_goal
-    c = keys.c
-    abt = keys.abt
-    abn = keys.abn
-    min_dose = keys.min_dose
-    max_dose = keys.max_dose
-    fixed_prob = keys.fixed_prob
-    fixed_mean = keys.fixed_mean
-    fixed_std = keys.fixed_std
-    # ---------------------------------------------------------------------- #
-    # check in which fraction policy should be returned
-    policy_plot = 1 if sets.plot_policy == fraction else 0
-
-    if fixed_prob != 1:
-        mean = np.mean(
-            sparing_factors_public
-        )  # extract the mean and std to setup the sparingfactor distribution
-        standard_deviation = std_posterior(sparing_factors_public, alpha, beta)
-    if fixed_prob == 1:
-        mean = fixed_mean
-        standard_deviation = fixed_std
-    X = truncated_normal(mean, standard_deviation, sets.sf_low, sets.sf_high)
-    bedt_states = np.arange(accumulated_tumor_dose, tumor_goal, 1)
-    bedt_states = np.concatenate(
-        (bedt_states, [tumor_goal, tumor_goal + 1])
-    )  # add an extra step outside of our prescribed tumor dose which will be penalised to make sure that we aim at the prescribe tumor dose
-    [sf, prob] = sf_probdist(X, sets.sf_low, sets.sf_high,
-        sets.sf_stepsize, sets.sf_prob_threshold)
-    # we prepare an empty values list and open an action space which is equal to all the dose numbers that can be given in one fraction
-    values = np.zeros(
-        (number_of_fractions - fraction, len(bedt_states), len(sf))
-    )  # 2d values list with first indice being the BED and second being the sf
-    max_physical_dose = convert_to_physical(tumor_goal, abt)
-    if max_dose == -1:
-        max_dose = max_physical_dose
-    elif max_dose > max_physical_dose:
-        # if the max dose is too large we lower it, so we dont needlessly check too many actions
-        max_dose = max_physical_dose
-    if min_dose > max_dose:
-        min_dose = max_dose - 0.1
-    actionspace = np.arange(min_dose, max_dose + 0.1, 0.1)
-    # now we set up the policy array which has len(BEDT)*len(sf)*len(actionspace) entries. We give each action the same probability to start with
-    policy = np.zeros((number_of_fractions - fraction, len(bedt_states), len(sf)))
-
-    for state, fraction_state in enumerate(
-        np.arange(number_of_fractions, fraction -1, -1)
-    ):
-        if (
-            state == number_of_fractions - 1 #fraction_state == 1
-        ):  # first state with no prior dose delivered so we dont loop through BEDT
-            bedn = bed_calc_matrix(
-                sparing_factors_public[-1], abn, actionspace
-            )  # calculate all delivered doses to the Normal tissues (the penalty)
-            future_bedt = bed_calc0(actionspace, abt)
-            future_values_func = interp1d(bedt_states, (values[state - 1] * prob).sum(axis=1))
-            future_values = future_values_func(
-                future_bedt
-            )  # for each action and sparing factor calculate the penalty of the action and add the future value we will only have as many future values as we have actions (not sparing dependent)
-            c_penalties = np.zeros(future_bedt.shape)
-            c_penalties[future_bedt < tumor_goal] = -c
-            vs = -bedn + c_penalties + future_values
-            policy4 = vs.argmax(axis=1)
-        elif (
-            accumulated_tumor_dose >= tumor_goal
-        ):
-            best_action = 0
-            last_BEDN = bed_calc0(best_action, abn, sparing_factors_public[-1])
-            policy4 = 0
-            break
-        elif (
-            fraction_state == fraction and fraction != number_of_fractions
-        ):  # actual fraction is first state to calculate
-            actionspace_clipped = actionspace[
-                0 : max_action(accumulated_tumor_dose, actionspace, tumor_goal) + 1
-            ]
-            bedn = bed_calc_matrix(sparing_factors_public[-1], abn, actionspace_clipped)
-            future_bedt = accumulated_tumor_dose + bed_calc0(actionspace_clipped, abt)
-            future_bedt[future_bedt > tumor_goal] = tumor_goal + 1
-            penalties = np.zeros(future_bedt.shape)
-            c_penalties = np.zeros(future_bedt.shape)
-            penalties[future_bedt > tumor_goal] = 0 #overdosing is indirectly penalised with BEDN
-            c_penalties[future_bedt < tumor_goal] = -c
-            future_values_func = interp1d(bedt_states, (values[state - 1] * prob).sum(axis=1))
-            future_values = future_values_func(
-                future_bedt
-            )  # for each action and sparing factor calculate the penalty of the action and add the future value we will only have as many future values as we have actions (not sparing dependent)
-            vs = -bedn + c_penalties + future_values + penalties
-            policy4 = vs.argmax(axis=1)
-        elif (
-            fraction == number_of_fractions
-        ):  # in this state no penalty has to be defined as the value is not relevant
-            best_action = convert_to_physical(tumor_goal-accumulated_tumor_dose, abt)
-            if accumulated_tumor_dose > tumor_goal:
-                best_action = 0
-            if best_action < min_dose:
-                best_action = min_dose
-            if best_action > max_dose:
-                best_action = max_dose
-            last_BEDN = bed_calc0(best_action, abn, sparing_factors_public[-1])
-            policy4 = best_action * 10
-        else:
-            future_value_prob = (values[state - 1] * prob).sum(axis=1)
-            future_values_func = interp1d(bedt_states, future_value_prob)
-            for tumor_index, tumor_value in enumerate(
-                bedt_states
-            ):  # this and the next for loop allow us to loop through all states
-                actionspace_clipped = actionspace[
-                    0 : max_action(tumor_value, actionspace, tumor_goal) + 1
-                ]  # we only allow the actions that do not overshoot
-                bedn = bed_calc_matrix(
-                    sf, abn, actionspace_clipped
-                )  # this one could be done outside of the loop and only the clipping would happen inside the loop.
-                bed = bed_calc_matrix(np.ones(len(sf)), abt, actionspace_clipped)
-                if state != 0 and tumor_value < tumor_goal:
-                    future_bedt = tumor_value + bed
-                    future_bedt[future_bedt > tumor_goal] = tumor_goal + 1
-                    future_values = future_values_func(
-                        future_bedt
-                    )  # for each action and sparing factor calculate the penalty of the action and add the future value we will only have as many future values as we have actions (not sparing dependent)
-                    c_penalties = np.zeros(future_bedt.shape)
-                    c_penalties[future_bedt < tumor_goal] = -c
-                    vs = -bedn + c_penalties + future_values
-                    if vs.size == 0:
-                        best_action = np.zeros(len(sf))
-                        valer = np.zeros(len(sf))
-                    else:
-                        best_action = actionspace_clipped[vs.argmax(axis=1)]
-                        valer = vs.max(axis=1)
-                elif tumor_value > tumor_goal: #calculate value for terminal case
-                    best_action = 0
-                    future_bedt = tumor_value
-                    valer = (
-                        + np.zeros(sf.shape)
-                    )  
-                else:  # last state no more further values to add
-                    best_action = convert_to_physical(tumor_goal-tumor_value, abt)
-                    if best_action > max_dose:
-                        best_action = max_dose
-                    if best_action < min_dose:
-                        best_action = min_dose
-                    last_BEDN = bed_calc0(best_action, abn, sf)
-                    future_bedt = tumor_value + bed_calc0(best_action, abt)
-                    underdose_penalty = 0
-                    overdose_penalty = 0
-                    if future_bedt < tumor_goal:
-                        underdose_penalty = -10000
-                    if future_bedt > tumor_goal:
-                        overdose_penalty = 0
-                    valer = (
-                        -last_BEDN
-                        + underdose_penalty * np.ones(sf.shape)
-                        + overdose_penalty * np.ones(sf.shape)
-                    )  # gives the value of each action for all sparing factors. elements 0-len(sparingfactors) are the Values for
-
-                policy[state][tumor_index] = best_action
-                values[state][tumor_index] = valer
-
-    if sets.plot_policy or sets.plot_value:
-        policy = np.concatenate([np.zeros((1, len(bedt_states), len(sf))), policy[::-1]])
-        values = np.concatenate([np.zeros((1, len(bedt_states), len(sf))), values[::-1]])
-    if fraction != number_of_fractions:
-        optimal_action = actionspace[policy4]
-    if fraction == number_of_fractions:
-        optimal_action = policy4 / 10
-    tumor_dose = bed_calc0(optimal_action, abt)
-    oar_dose = bed_calc0(optimal_action, abn, sparing_factors_public[-1])
-
-    output = DotDict({})
-
-    output.physical_dose = optimal_action
-    output.tumor_dose = tumor_dose
-    output.oar_dose = oar_dose
-    
-    return output
-
-
-
-
-
-
 
 def max_tumor_bed_old(keys, sets=SETTING_DICT):
     fraction = keys.fraction
     number_of_fractions = keys.number_of_fractions
-    accumulated_oar_dose = keys.accumulated_tumor_dose
+    accumulated_oar_dose = keys.accumulated_oar_dose
     sparing_factors_public = keys.sparing_factors_public
-    alpha = keys.alpha
-    beta = keys.beta
+    shape = keys.shape
+    scale = keys.scale
     oar_limit = keys.oar_limit
     abt = keys.abt
     abn = keys.abn
     min_dose = keys.min_dose
     max_dose = keys.max_dose
-    fixed_prob = keys.fixed_prob
+    prob_update = keys.prob_update
     fixed_mean = keys.fixed_mean
     fixed_std = keys.fixed_std
     # ---------------------------------------------------------------------- #
     # check in which fraction policy should be returned
     policy_plot = 1 if sets.plot_policy == fraction else 0
     
     actual_sparing = sparing_factors_public[-1]
-    if fixed_prob != 1:
+    if prob_update == 1:
         mean = np.mean(
             sparing_factors_public
         )  # extract the mean and std to setup the sparingfactor distribution
-        standard_deviation = std_posterior(sparing_factors_public, alpha, beta)
-    if fixed_prob == 1:
+        standard_deviation = std_posterior(sparing_factors_public, shape, scale)
+    elif prob_update == 0:
         mean = fixed_mean
         standard_deviation = fixed_std
     X = truncated_normal(mean, standard_deviation, sets.sf_low, sets.sf_high)
     [sf, prob] = sf_probdist(X, sets.sf_low, sets.sf_high,
         sets.sf_stepsize, sets.sf_prob_threshold)
 
     bedn = np.arange(accumulated_oar_dose, oar_limit + 1.6, 1)
@@ -630,35 +443,35 @@
 
 def min_oar_max_tumor_old(keys, sets=SETTING_DICT):
     fraction = keys.fraction
     number_of_fractions = keys.number_of_fractions
     accumulated_tumor_dose = keys.accumulated_tumor_dose
     accumulated_oar_dose = keys.accumulated_oar_dose
     sparing_factors_public = keys.sparing_factors_public
-    alpha = keys.alpha
-    beta = keys.beta
+    shape = keys.shape
+    scale = keys.scale
     tumor_goal = keys.tumor_goal
     oar_limit = keys.oar_limit
     abt = keys.abt
     abn = keys.abn
     min_dose = keys.min_dose
     max_dose = keys.max_dose
-    fixed_prob = keys.fixed_prob
+    prob_update = keys.prob_update
     fixed_mean = keys.fixed_mean
     fixed_std = keys.fixed_std
     # ---------------------------------------------------------------------- #
     # check in which fraction policy should be returned
     policy_plot = 1 if sets.plot_policy == fraction else 0
 
-    if fixed_prob != 1:
+    if prob_update == 1:
         mean = np.mean(
             sparing_factors_public
         )  # extract the mean and std to setup the sparingfactor distribution
-        standard_deviation = std_posterior(sparing_factors_public, alpha, beta)
-    if fixed_prob == 1:
+        standard_deviation = std_posterior(sparing_factors_public, shape, scale)
+    elif prob_update == 0:
         mean = fixed_mean
         standard_deviation = fixed_std
     X = truncated_normal(mean, standard_deviation, sets.sf_low, sets.sf_high)
     [sf, prob] = sf_probdist(X, sets.sf_low, sets.sf_high,
         sets.sf_stepsize, sets.sf_prob_threshold)
     underdosepenalty = 10
     print(accumulated_oar_dose, accumulated_tumor_dose)
```

### Comparing `adaptfx-0.2.0/src/adaptfx.egg-info/PKG-INFO` & `adaptfx-0.2.1/src/adaptfx.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptfx
-Version: 0.2.0
+Version: 0.2.1
 Summary: Package for computing dose fractionation schemes in MR guided Adaptive Radiotherapy
 Author-email: Janic Tom Weber <janic.weber@uzh.ch>, Yoel Pérez Haas <yoel.perezhaas@uzh.ch>
 License: MIT
 Project-URL: source, https://github.com/openAFT/adaptfx
 Keywords: fractionation,adaptive radiotherapy,reinforcement-learning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
@@ -135,14 +135,18 @@
 ### GUI
 
 A last addition is made with graphical user interfaces that facilitate the use of the interpolation algorithms. There are two interfaces that can be run. In these interfaces all variables can be given to compute an adaptive fractionation plan for a patient. 
 
 > :warning: Note:\
 > The interfaces are not optimized, and thus it is not recommended using them to further develop extensions.
 
+### Reducing Number of Fractions
+
+For the 2D algorithms there exist the possibility to reduce number of fractions. A constant $c$ can be chosen which introduces a reward (or rather a cost) linear to the number of fractions used to finish the treatment. The cost is added to the immediate reward returned by the environment in the current fraction. There exist a simulative model helping to estimate what the constant $c$ should be chosen in order for the treatment to finish on some target number of fractions $n_{\text{targ}}$. The function can be found [here](src/adaptfx/radiobiology.py) in `c_calc`.
+
 ### Probability Updating
 
 The DP algorithm relies on a description of the environment to compute an optimal policy, in this case the probability distribution of the sparing factor $P(\delta)$, which we assume to be a Gaussian distribution truncated at $0$, with patient-specific parameters for mean and standard deviation. At the start of a treatment, only two sparing factors are available for that patient, from the planning scan and the first fraction. In each fraction, an additional sparing factor is measured, which can be used to calculate updated estimates $\mu_t$ and $\sigma_t$ for mean and standard deviation, respectively.
 
 #### No Updating
 
 In case where the probability is not updated the parameters $\mu_t$ and $\sigma_t$ of the normal distribution can be fixed.
@@ -184,20 +188,20 @@
       from _ctypes import Union, Structure, Array
 ImportError: No module named '_ctypes'
 ```
 
 **Solution:** with the specific package manager of the Linux distribution install `libffi-dev` development tool. E.g. in Fedora Linux and derivatives install this tool
 
 ```
-sudo dnf install libffi-devel
+$ sudo dnf install libffi-devel
 ```
 
 On Ubuntu:
 ```
-sudo apt install libffi-dev
+$ sudo apt install libffi-dev
 ```
 
 ### No GUI backend for `matplotlib`
 
 **Problem:** on Linux or MacOS it could be that once `aft` is run the plots are not shown and there is an error message:
 
 
@@ -206,27 +210,27 @@
   Could not find a version that satisfies the requirement tkinter (from versions: )
 No matching distribution found for tkinter
 ```
 
 **Solution:** on Fedora Linux and derivative distributions one could solve this by either installing python tkinter
 
 ```
-sudo dnf install python3-tkinter
+$ sudo dnf install python3-tkinter
 ```
 
 on Ubuntu
 
 ```
-sudo apt-get install python3-tk
+$ sudo apt-get install python3-tk
 ```
 
 **Solution:** on MacOS and Linux one could instead use `pip` to install `pyqt`
 
 ```
-pip install pyqt5
+$ pip install pyqt5
 ```
 
 
 ## References
 
 <a id="1">[1]</a>
 Yoel Samuel Pérez Haas et al.;
```

### Comparing `adaptfx-0.2.0/src/adaptfx.egg-info/SOURCES.txt` & `adaptfx-0.2.1/src/adaptfx.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -221,10 +221,20 @@
 src/adaptfx/visualiser.py
 src/adaptfx.egg-info/PKG-INFO
 src/adaptfx.egg-info/SOURCES.txt
 src/adaptfx.egg-info/dependency_links.txt
 src/adaptfx.egg-info/entry_points.txt
 src/adaptfx.egg-info/requires.txt
 src/adaptfx.egg-info/top_level.txt
-work/frac_example.json
-work/oar_example.json
-work/testing.json
+src/adaptsim/__init__.py
+src/adaptsim/ast.py
+src/adaptsim/constants.py
+src/adaptsim/visualiser.py
+src/adaptsim/visualiser_data.py
+work/example_0.json
+work/example_1.json
+work/example_2.json
+work/example_3.json
+work/example_4.json
+work/example_5.json
+work/example_6.json
+work/example_7.json
```

### Comparing `adaptfx-0.2.0/work/frac_example.json` & `adaptfx-0.2.1/work/example_0.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9036931818181818%*

 * *Differences: {"'keys'": "{'sparing_factors': [0.946, 0.906, 0.905, 0.796, 0.868, 0.916, 0.954], 'prob_update': "*

 * *           "2, 'shape': 10.61, 'scale': 0.003, 'shape_inv': 2.27, 'scale_inv': 0.002, 'min_dose': "*

 * *           "4, 'max_dose': 14, 'c': 1.5}",*

 * * "'settings'": "{'sf_stepsize': 0.005, 'plot_remains': 0, 'plot_values': 0, 'plot_probability': 0, "*

 * *               "'save_plot': 0, delete: ['sf_low', 'sf_high', 'sf_prob_threshold']}"}*

```diff
@@ -1,40 +1,41 @@
 {
     "algorithm": "frac",
     "keys": {
         "accumulated_oar_dose": 0,
         "accumulated_tumor_dose": 0,
-        "c": 0,
+        "c": 1.5,
         "fixed_mean": 0.9,
         "fixed_std": 0.04,
         "fraction": 0,
-        "max_dose": -1,
-        "min_dose": 0,
+        "max_dose": 14,
+        "min_dose": 4,
         "number_of_fractions": 6,
-        "prob_update": 0,
-        "scale": "invalid",
-        "scale_inv": "invalid",
-        "shape": "invalid",
-        "shape_inv": "invalid",
+        "prob_update": 2,
+        "scale": 0.003,
+        "scale_inv": 0.002,
+        "shape": 10.61,
+        "shape_inv": 2.27,
         "sparing_factors": [
-            0.98,
-            0.97,
-            0.8,
-            0.83,
-            0.8,
-            0.85,
-            0.94
+            0.946,
+            0.906,
+            0.905,
+            0.796,
+            0.868,
+            0.916,
+            0.954
         ],
         "tumor_goal": 72
     },
     "level": 1,
     "log": 0,
     "settings": {
         "dose_stepsize": 0.5,
         "plot_policy": 1,
-        "sf_high": 1.1,
-        "sf_low": 0.7,
-        "sf_prob_threshold": 0,
-        "sf_stepsize": 0.01,
+        "plot_probability": 0,
+        "plot_remains": 0,
+        "plot_values": 0,
+        "save_plot": 0,
+        "sf_stepsize": 0.005,
         "state_stepsize": 0.5
     }
 }
```

### Comparing `adaptfx-0.2.0/work/oar_example.json` & `adaptfx-0.2.1/work/example_3.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9036931818181818%*

 * *Differences: {"'keys'": "{'sparing_factors': [0.946, 0.906, 0.905, 0.796, 0.868, 0.916, 0.954], 'fixed_mean': "*

 * *           "0.85, 'fixed_std': 0.1, 'shape': 10.61, 'scale': 0.003, 'shape_inv': 2.27, "*

 * *           "'scale_inv': 0.002, delete: ['c']}",*

 * * "'settings'": "{'sf_stepsize': 0.005, 'plot_remains': 0, 'plot_values': 0, 'plot_probability': 1, "*

 * *               "'save_plot': 0, delete: ['sf_low', 'sf_high', 'sf_prob_threshold']}"}*

```diff
@@ -1,40 +1,40 @@
 {
     "algorithm": "oar",
     "keys": {
         "accumulated_oar_dose": 0,
         "accumulated_tumor_dose": 0,
-        "c": 0,
-        "fixed_mean": 0.9,
-        "fixed_std": 0.04,
+        "fixed_mean": 0.85,
+        "fixed_std": 0.1,
         "fraction": 0,
         "max_dose": -1,
         "min_dose": 0,
         "number_of_fractions": 6,
         "prob_update": 0,
-        "scale": "invalid",
-        "scale_inv": "invalid",
-        "shape": "invalid",
-        "shape_inv": "invalid",
+        "scale": 0.003,
+        "scale_inv": 0.002,
+        "shape": 10.61,
+        "shape_inv": 2.27,
         "sparing_factors": [
-            0.98,
-            0.97,
-            0.8,
-            0.83,
-            0.8,
-            0.85,
-            0.94
+            0.946,
+            0.906,
+            0.905,
+            0.796,
+            0.868,
+            0.916,
+            0.954
         ],
         "tumor_goal": 72
     },
     "level": 1,
     "log": 0,
     "settings": {
         "dose_stepsize": 0.5,
         "plot_policy": 1,
-        "sf_high": 1.1,
-        "sf_low": 0.7,
-        "sf_prob_threshold": 0,
-        "sf_stepsize": 0.01,
+        "plot_probability": 1,
+        "plot_remains": 0,
+        "plot_values": 0,
+        "save_plot": 0,
+        "sf_stepsize": 0.005,
         "state_stepsize": 0.5
     }
 }
```

