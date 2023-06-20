# Comparing `tmp/aiida_nanotech_empa-1.0.0b2.tar.gz` & `tmp/aiida_nanotech_empa-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_nanotech_empa-1.0.0b2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiida_nanotech_empa-1.0.0b3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida_nanotech_empa-1.0.0b2.tar` & `aiida_nanotech_empa-1.0.0b3.tar`

### file list

```diff
@@ -1,121 +1,118 @@
--rw-r--r--   0        0        0       13 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/.codecov.yml
--rw-r--r--   0        0        0       33 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/.coveragerc
--rw-r--r--   0        0        0       52 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/.flake8
--rw-r--r--   0        0        0      200 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/.github/install_cp2k.sh
--rw-r--r--   0        0        0      289 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/.github/install_qe.sh
--rw-r--r--   0        0        0     1737 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      795 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/.github/workflows/publish.yml
--rw-r--r--   0        0        0      135 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/.gitignore
--rw-r--r--   0        0        0     1628 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1075 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/LICENSE
--rw-r--r--   0        0        0     2277 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/README.md
--rw-r--r--   0        0        0      189 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/__init__.py
--rw-r--r--   0        0        0       51 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/helpers.py
--rw-r--r--   0        0        0      273 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/parsers/__init__.py
--rw-r--r--   0        0        0     9867 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/parsers/cp2k_gw_parser.py
--rw-r--r--   0        0        0     4846 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/parsers/cp2k_neb_parser.py
--rw-r--r--   0        0        0     2542 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/parsers/cubegen_pymol_parser.py
--rw-r--r--   0        0        0     1678 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/parsers/gaussian_casscf_parser.py
--rw-r--r--   0        0        0     1379 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/parsers/pp_parser.py
--rw-r--r--   0        0        0      230 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/plugins/__init__.py
--rw-r--r--   0        0        0     3023 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/plugins/afm.py
--rw-r--r--   0        0        0     2951 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/plugins/hrstm.py
--rw-r--r--   0        0        0     3542 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/plugins/overlap.py
--rw-r--r--   0        0        0     2863 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/plugins/stm.py
--rw-r--r--   0        0        0      168 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/schedulers/__init__.py
--rw-r--r--   0        0        0     1523 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/schedulers/lsf_ethz_euler.py
--rw-r--r--   0        0        0     1599 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/schedulers/slurm_ethz_euler.py
--rw-r--r--   0        0        0        0 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/__init__.py
--rw-r--r--   0        0        0    15829 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/analyze_structure.py
--rw-r--r--   0        0        0     1375 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/common_utils.py
--rw-r--r--   0        0        0     2736 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/cube_utils.py
--rw-r--r--   0        0        0     9994 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/gaussian_wcs_postprocess.py
--rw-r--r--   0        0        0    10034 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/igor.py
--rw-r--r--   0        0        0     5427 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/pymol_render.py
--rw-r--r--   0        0        0     8561 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/stm_tools.py
--rw-r--r--   0        0        0      103 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/version.py
--rw-r--r--   0        0        0        0 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/__init__.py
--rw-r--r--   0        0        0     1147 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/__init__.py
--rw-r--r--   0        0        0    11867 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/adsorbed_gw_ic_workchain.py
--rw-r--r--   0        0        0     6154 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/afm_workchain.py
--rw-r--r--   0        0        0    31717 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/cp2k_utils.py
--rw-r--r--   0        0        0     2627 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/ALL_POTENTIALS
--rw-r--r--   0        0        0     2333 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/BASIS_DEFAULT
--rw-r--r--   0        0        0   136047 2023-06-16 13:42:28.627694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/BASIS_MOLOPT
--rw-r--r--   0        0        0   114564 2023-06-16 13:42:28.627694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/GW_BASIS_SET
--rw-r--r--   0        0        0   172445 2023-06-16 13:42:28.627694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/K_GW_BASIS
--rw-r--r--   0        0        0   135825 2023-06-16 13:42:28.627694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/POTENTIAL
--rw-r--r--   0        0        0      378 2023-06-16 13:42:28.627694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/POTENTIALS_DEFAULT
--rw-r--r--   0        0        0   154582 2023-06-16 13:42:28.627694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/RI_HFX_BASIS_all
--rw-r--r--   0        0        0     8000 2023-06-16 13:42:28.627694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/atomic_kinds.yml
--rw-r--r--   0        0        0    10869 2023-06-16 13:42:28.627694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_2pp.ini
--rw-r--r--   0        0        0    10601 2023-06-16 13:42:28.627694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_pp.ini
--rw-r--r--   0        0        0  1959318 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/dftd3.dat
--rw-r--r--   0        0        0     9698 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/diag_workchain.py
--rw-r--r--   0        0        0    13166 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/fragment_separation.py
--rw-r--r--   0        0        0     7700 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/geo_opt_workchain.py
--rw-r--r--   0        0        0     5666 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/hrstm_workchain.py
--rw-r--r--   0        0        0    11952 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/molecule_gw_workchain.py
--rw-r--r--   0        0        0     6348 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/molecule_opt_gw_workchain.py
--rw-r--r--   0        0        0     9953 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/neb_workchain.py
--rw-r--r--   0        0        0     4169 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/orbitals_workchain.py
--rw-r--r--   0        0        0     6973 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/pdos_workchain.py
--rw-r--r--   0        0        0     5592 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/phonons_workchain.py
--rw-r--r--   0        0        0     1252 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/cell_opt_protocol.yml
--rw-r--r--   0        0        0    12253 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/geo_opt_protocol.yml
--rw-r--r--   0        0        0    11446 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/gw_protocols.yml
--rw-r--r--   0        0        0     7983 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/neb_protocol.yml
--rw-r--r--   0        0        0     9918 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/phonons_protocol.yml
--rw-r--r--   0        0        0     1966 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/scf_diag_protocol.yml
--rw-r--r--   0        0        0     7603 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/scf_ot_protocol.yml
--rw-r--r--   0        0        0    14942 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/replica_workchain.py
--rw-r--r--   0        0        0     4369 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/stm_workchain.py
--rw-r--r--   0        0        0      812 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/__init__.py
--rw-r--r--   0        0        0     9185 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/casscf_series_workchain.py
--rw-r--r--   0        0        0     8919 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/casscf_workchain.py
--rw-r--r--   0        0        0     6083 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/common.py
--rw-r--r--   0        0        0     6708 2023-06-16 13:42:28.639694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/constr_opt_chain_workchain.py
--rw-r--r--   0        0        0     7953 2023-06-16 13:42:28.639694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/delta_scf_workchain.py
--rw-r--r--   0        0        0     5234 2023-06-16 13:42:28.639694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/hf_mp2_workchain.py
--rw-r--r--   0        0        0    11073 2023-06-16 13:42:28.639694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/natorb_workchain.py
--rw-r--r--   0        0        0    12134 2023-06-16 13:42:28.639694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/relax_workchain.py
--rw-r--r--   0        0        0    11760 2023-06-16 13:42:28.639694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/scf_workchain.py
--rw-r--r--   0        0        0    11519 2023-06-16 13:42:28.639694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/spin_workchain.py
--rw-r--r--   0        0        0       80 2023-06-16 13:42:28.639694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/qe/__init__.py
--rw-r--r--   0        0        0    22418 2023-06-16 13:42:28.639694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/qe/nanoribbon.py
--rw-r--r--   0        0        0     3369 2023-06-16 13:42:28.639694 aiida_nanotech_empa-1.0.0b2/conftest.py
--rw-r--r--   0        0        0       96 2023-06-16 13:42:28.639694 aiida_nanotech_empa-1.0.0b2/examples/__init__.py
--rw-r--r--   0        0        0   921233 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/data/sssp_minimal/C.upf
--rw-r--r--   0        0        0   366195 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/data/sssp_minimal/H.upf
--rw-r--r--   0        0        0       13 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/.gitignore
--rwxr-xr-x   0        0        0     9833 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/aa
--rw-r--r--   0        0        0      558 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/benzene-diradical.xyz
--rw-r--r--   0        0        0      402 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/c2h2.xyz
--rw-r--r--   0        0        0      422 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/c2h2_no_spin.xyz
--rw-r--r--   0        0        0     2959 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/c2h2_on_au111.xyz
--rw-r--r--   0        0        0      467 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/c2h2_spin.xyz
--rw-r--r--   0        0        0      572 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/c2h4.xyz
--rw-r--r--   0        0        0     2533 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_ads_gw_ic.py
--rw-r--r--   0        0        0     5271 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_afm.py
--rw-r--r--   0        0        0     3527 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_diag.py
--rw-r--r--   0        0        0     3702 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_fragment_separation.py
--rw-r--r--   0        0        0     4654 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_geo_opt.py
--rw-r--r--   0        0        0     3177 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_gw.py
--rw-r--r--   0        0        0     5825 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_hrstm.py
--rw-r--r--   0        0        0     1934 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_mol_opt_gw.py
--rw-r--r--   0        0        0     6194 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_neb.py
--rw-r--r--   0        0        0     3893 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_orb.py
--rw-r--r--   0        0        0     4486 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_pdos.py
--rw-r--r--   0        0        0     3057 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_phonons.py
--rw-r--r--   0        0        0     3163 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_replica_chain.py
--rw-r--r--   0        0        0     3831 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_stm.py
--rw-r--r--   0        0        0     2145 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_gaussian_casscf.py
--rw-r--r--   0        0        0     1393 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_gaussian_spin.py
--rw-r--r--   0        0        0     2776 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_nanoribbon.py
--rw-r--r--   0        0        0      251 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/h2.xyz
--rw-r--r--   0        0        0     2483 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/h2_on_au111.xyz
--rw-r--r--   0        0        0     1568 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/h2_on_hbn.xyz
--rw-r--r--   0        0        0      679 2023-06-16 13:42:28.647694 aiida_nanotech_empa-1.0.0b2/examples/workflows/si_bulk.xyz
--rw-r--r--   0        0        0     4743 2023-06-16 13:42:28.647694 aiida_nanotech_empa-1.0.0b2/pyproject.toml
--rw-r--r--   0        0        0      253 2023-06-16 13:42:28.647694 aiida_nanotech_empa-1.0.0b2/pytest.ini
--rw-r--r--   0        0        0     3610 1970-01-01 00:00:00.000000 aiida_nanotech_empa-1.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0       13 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/.codecov.yml
+-rw-r--r--   0        0        0       33 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/.coveragerc
+-rw-r--r--   0        0        0       52 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/.flake8
+-rw-r--r--   0        0        0      200 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/.github/install_cp2k.sh
+-rw-r--r--   0        0        0      289 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/.github/install_qe.sh
+-rw-r--r--   0        0        0     1737 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      795 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      135 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/.gitignore
+-rw-r--r--   0        0        0     1628 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1075 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/LICENSE
+-rw-r--r--   0        0        0     2277 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/README.md
+-rw-r--r--   0        0        0      189 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/__init__.py
+-rw-r--r--   0        0        0       51 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/helpers.py
+-rw-r--r--   0        0        0      273 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/parsers/__init__.py
+-rw-r--r--   0        0        0     9867 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/parsers/cp2k_gw_parser.py
+-rw-r--r--   0        0        0     4846 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/parsers/cp2k_neb_parser.py
+-rw-r--r--   0        0        0     2542 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/parsers/cubegen_pymol_parser.py
+-rw-r--r--   0        0        0     1678 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/parsers/gaussian_casscf_parser.py
+-rw-r--r--   0        0        0     1379 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/parsers/pp_parser.py
+-rw-r--r--   0        0        0      230 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/plugins/__init__.py
+-rw-r--r--   0        0        0     3023 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/plugins/afm.py
+-rw-r--r--   0        0        0     2951 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/plugins/hrstm.py
+-rw-r--r--   0        0        0     3542 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/plugins/overlap.py
+-rw-r--r--   0        0        0     2863 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/plugins/stm.py
+-rw-r--r--   0        0        0      168 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/schedulers/__init__.py
+-rw-r--r--   0        0        0     1523 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/schedulers/lsf_ethz_euler.py
+-rw-r--r--   0        0        0     1599 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/schedulers/slurm_ethz_euler.py
+-rw-r--r--   0        0        0        0 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/utils/__init__.py
+-rw-r--r--   0        0        0    15829 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/utils/analyze_structure.py
+-rw-r--r--   0        0        0     1375 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/utils/common_utils.py
+-rw-r--r--   0        0        0     2736 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/utils/cube_utils.py
+-rw-r--r--   0        0        0     9994 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/utils/gaussian_wcs_postprocess.py
+-rw-r--r--   0        0        0    10034 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/utils/igor.py
+-rw-r--r--   0        0        0     5427 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/utils/pymol_render.py
+-rw-r--r--   0        0        0     8561 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/utils/stm_tools.py
+-rw-r--r--   0        0        0      103 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/version.py
+-rw-r--r--   0        0        0        0 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/__init__.py
+-rw-r--r--   0        0        0     1147 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/__init__.py
+-rw-r--r--   0        0        0    11867 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/adsorbed_gw_ic_workchain.py
+-rw-r--r--   0        0        0     6154 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/afm_workchain.py
+-rw-r--r--   0        0        0    31717 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/cp2k_utils.py
+-rw-r--r--   0        0        0     2627 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/data/ALL_POTENTIALS
+-rw-r--r--   0        0        0     2333 2023-06-20 15:03:53.220860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/data/BASIS_DEFAULT
+-rw-r--r--   0        0        0   136047 2023-06-20 15:03:53.224860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/data/BASIS_MOLOPT
+-rw-r--r--   0        0        0   114564 2023-06-20 15:03:53.224860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/data/GW_BASIS_SET
+-rw-r--r--   0        0        0   172445 2023-06-20 15:03:53.224860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/data/K_GW_BASIS
+-rw-r--r--   0        0        0   135825 2023-06-20 15:03:53.224860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/data/POTENTIAL
+-rw-r--r--   0        0        0      378 2023-06-20 15:03:53.224860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/data/POTENTIALS_DEFAULT
+-rw-r--r--   0        0        0   154582 2023-06-20 15:03:53.224860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/data/RI_HFX_BASIS_all
+-rw-r--r--   0        0        0     8000 2023-06-20 15:03:53.224860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/data/atomic_kinds.yml
+-rw-r--r--   0        0        0    10869 2023-06-20 15:03:53.224860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_2pp.ini
+-rw-r--r--   0        0        0    10601 2023-06-20 15:03:53.224860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_pp.ini
+-rw-r--r--   0        0        0  1959318 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/data/dftd3.dat
+-rw-r--r--   0        0        0     9698 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/diag_workchain.py
+-rw-r--r--   0        0        0    13166 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/fragment_separation.py
+-rw-r--r--   0        0        0     7700 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/geo_opt_workchain.py
+-rw-r--r--   0        0        0     5666 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/hrstm_workchain.py
+-rw-r--r--   0        0        0    11952 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/molecule_gw_workchain.py
+-rw-r--r--   0        0        0     6348 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/molecule_opt_gw_workchain.py
+-rw-r--r--   0        0        0     9953 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/neb_workchain.py
+-rw-r--r--   0        0        0     4169 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/orbitals_workchain.py
+-rw-r--r--   0        0        0     6973 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/pdos_workchain.py
+-rw-r--r--   0        0        0     5592 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/phonons_workchain.py
+-rw-r--r--   0        0        0     1252 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/protocols/cell_opt_protocol.yml
+-rw-r--r--   0        0        0    12253 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/protocols/geo_opt_protocol.yml
+-rw-r--r--   0        0        0    11446 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/protocols/gw_protocols.yml
+-rw-r--r--   0        0        0     7983 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/protocols/neb_protocol.yml
+-rw-r--r--   0        0        0     9918 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/protocols/phonons_protocol.yml
+-rw-r--r--   0        0        0     1966 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/protocols/scf_diag_protocol.yml
+-rw-r--r--   0        0        0     7603 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/protocols/scf_ot_protocol.yml
+-rw-r--r--   0        0        0    14942 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/replica_workchain.py
+-rw-r--r--   0        0        0     4369 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/stm_workchain.py
+-rw-r--r--   0        0        0      812 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/gaussian/__init__.py
+-rw-r--r--   0        0        0     9185 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/gaussian/casscf_series_workchain.py
+-rw-r--r--   0        0        0     8919 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/gaussian/casscf_workchain.py
+-rw-r--r--   0        0        0     6083 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/gaussian/common.py
+-rw-r--r--   0        0        0     6708 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/gaussian/constr_opt_chain_workchain.py
+-rw-r--r--   0        0        0     7953 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/gaussian/delta_scf_workchain.py
+-rw-r--r--   0        0        0     5234 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/gaussian/hf_mp2_workchain.py
+-rw-r--r--   0        0        0    11073 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/gaussian/natorb_workchain.py
+-rw-r--r--   0        0        0    12134 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/gaussian/relax_workchain.py
+-rw-r--r--   0        0        0    11760 2023-06-20 15:03:53.232860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/gaussian/scf_workchain.py
+-rw-r--r--   0        0        0    11519 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/gaussian/spin_workchain.py
+-rw-r--r--   0        0        0       80 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/qe/__init__.py
+-rw-r--r--   0        0        0    22418 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/qe/nanoribbon.py
+-rw-r--r--   0        0        0     3071 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/conftest.py
+-rw-r--r--   0        0        0       13 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/.gitignore
+-rwxr-xr-x   0        0        0     9833 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/aa
+-rw-r--r--   0        0        0      558 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/benzene-diradical.xyz
+-rw-r--r--   0        0        0      402 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/c2h2.xyz
+-rw-r--r--   0        0        0      422 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/c2h2_no_spin.xyz
+-rw-r--r--   0        0        0     2959 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/c2h2_on_au111.xyz
+-rw-r--r--   0        0        0      467 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/c2h2_spin.xyz
+-rw-r--r--   0        0        0      572 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/c2h4.xyz
+-rw-r--r--   0        0        0     2533 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_ads_gw_ic.py
+-rw-r--r--   0        0        0     5271 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_afm.py
+-rw-r--r--   0        0        0     3527 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_diag.py
+-rw-r--r--   0        0        0     3702 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_fragment_separation.py
+-rw-r--r--   0        0        0     4654 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_geo_opt.py
+-rw-r--r--   0        0        0     3177 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_gw.py
+-rw-r--r--   0        0        0     5825 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_hrstm.py
+-rw-r--r--   0        0        0     1934 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_mol_opt_gw.py
+-rw-r--r--   0        0        0     6194 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_neb.py
+-rw-r--r--   0        0        0     3893 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_orb.py
+-rw-r--r--   0        0        0     4486 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_pdos.py
+-rw-r--r--   0        0        0     3057 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_phonons.py
+-rw-r--r--   0        0        0     3163 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_replica_chain.py
+-rw-r--r--   0        0        0     3831 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_stm.py
+-rw-r--r--   0        0        0     2145 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/example_gaussian_casscf.py
+-rw-r--r--   0        0        0     1393 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/example_gaussian_spin.py
+-rw-r--r--   0        0        0     2862 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/example_nanoribbon.py
+-rw-r--r--   0        0        0      251 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/h2.xyz
+-rw-r--r--   0        0        0     2483 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/h2_on_au111.xyz
+-rw-r--r--   0        0        0     1568 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/h2_on_hbn.xyz
+-rw-r--r--   0        0        0      679 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/examples/workflows/si_bulk.xyz
+-rw-r--r--   0        0        0     4742 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0      253 2023-06-20 15:03:53.236860 aiida_nanotech_empa-1.0.0b3/pytest.ini
+-rw-r--r--   0        0        0     3609 1970-01-01 00:00:00.000000 aiida_nanotech_empa-1.0.0b3/PKG-INFO
```

### Comparing `aiida_nanotech_empa-1.0.0b2/.github/workflows/ci.yml` & `aiida_nanotech_empa-1.0.0b3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/.github/workflows/publish.yml` & `aiida_nanotech_empa-1.0.0b3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/.pre-commit-config.yaml` & `aiida_nanotech_empa-1.0.0b3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/LICENSE` & `aiida_nanotech_empa-1.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/README.md` & `aiida_nanotech_empa-1.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/parsers/cp2k_gw_parser.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/parsers/cp2k_gw_parser.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/parsers/cp2k_neb_parser.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/parsers/cp2k_neb_parser.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/parsers/cubegen_pymol_parser.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/parsers/cubegen_pymol_parser.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/parsers/gaussian_casscf_parser.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/parsers/gaussian_casscf_parser.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/parsers/pp_parser.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/parsers/pp_parser.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/plugins/afm.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/plugins/afm.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/plugins/hrstm.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/plugins/hrstm.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/plugins/overlap.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/plugins/overlap.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/plugins/stm.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/plugins/stm.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/schedulers/lsf_ethz_euler.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/schedulers/lsf_ethz_euler.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/schedulers/slurm_ethz_euler.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/schedulers/slurm_ethz_euler.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/analyze_structure.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/utils/analyze_structure.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/common_utils.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/cube_utils.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/utils/cube_utils.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/gaussian_wcs_postprocess.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/utils/gaussian_wcs_postprocess.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/igor.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/utils/igor.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/pymol_render.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/utils/pymol_render.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/stm_tools.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/utils/stm_tools.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/__init__.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/adsorbed_gw_ic_workchain.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/adsorbed_gw_ic_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/afm_workchain.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/afm_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/cp2k_utils.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/cp2k_utils.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/ALL_POTENTIALS` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/data/ALL_POTENTIALS`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/BASIS_DEFAULT` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/data/BASIS_DEFAULT`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/BASIS_MOLOPT` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/data/BASIS_MOLOPT`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/GW_BASIS_SET` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/data/GW_BASIS_SET`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/K_GW_BASIS` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/data/K_GW_BASIS`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/POTENTIAL` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/data/POTENTIAL`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/RI_HFX_BASIS_all` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/data/RI_HFX_BASIS_all`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/atomic_kinds.yml` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/data/atomic_kinds.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_2pp.ini` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_2pp.ini`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_pp.ini` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_pp.ini`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/dftd3.dat` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/data/dftd3.dat`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/diag_workchain.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/diag_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/fragment_separation.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/fragment_separation.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/geo_opt_workchain.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/geo_opt_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/hrstm_workchain.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/hrstm_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/molecule_gw_workchain.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/molecule_gw_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/molecule_opt_gw_workchain.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/molecule_opt_gw_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/neb_workchain.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/neb_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/orbitals_workchain.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/orbitals_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/pdos_workchain.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/pdos_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/phonons_workchain.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/phonons_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/cell_opt_protocol.yml` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/protocols/cell_opt_protocol.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/geo_opt_protocol.yml` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/protocols/geo_opt_protocol.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/gw_protocols.yml` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/protocols/gw_protocols.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/neb_protocol.yml` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/protocols/neb_protocol.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/phonons_protocol.yml` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/protocols/phonons_protocol.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/scf_diag_protocol.yml` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/protocols/scf_diag_protocol.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/scf_ot_protocol.yml` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/protocols/scf_ot_protocol.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/replica_workchain.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/replica_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/stm_workchain.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/cp2k/stm_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/__init__.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/gaussian/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/casscf_series_workchain.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/gaussian/casscf_series_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/casscf_workchain.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/gaussian/casscf_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/common.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/gaussian/common.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/constr_opt_chain_workchain.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/gaussian/constr_opt_chain_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/delta_scf_workchain.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/gaussian/delta_scf_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/hf_mp2_workchain.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/gaussian/hf_mp2_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/natorb_workchain.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/gaussian/natorb_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/relax_workchain.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/gaussian/relax_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/scf_workchain.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/gaussian/scf_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/spin_workchain.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/gaussian/spin_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/qe/nanoribbon.py` & `aiida_nanotech_empa-1.0.0b3/aiida_nanotech_empa/workflows/qe/nanoribbon.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/conftest.py` & `aiida_nanotech_empa-1.0.0b3/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 """pytest fixtures for simplified testing."""
-import os
-import pathlib
 import shutil
+import subprocess
 
 import pytest
 from aiida.common import exceptions
 from aiida.orm import Code, Computer, QueryBuilder
-from aiida.plugins import GroupFactory
 
 pytest_plugins = ["aiida.manage.tests.pytest_fixtures"]
 
-SSSP_DIR = os.path.join(
-    os.path.dirname(os.path.abspath(__file__)), "examples/data/sssp_minimal"
-)
-
 
 @pytest.fixture(scope="session", autouse=True)
 def setup_sssp_pseudos(aiida_profile):
     """Create an SSSP pseudo potential family from scratch."""
-    aiida_profile.clear_profile()
-    sssp_family = GroupFactory("pseudo.family.sssp")
-    label = "SSSP/1.1/PBE/efficiency"
-    # label = 'SSSP_modified'
-    my_path = pathlib.Path(SSSP_DIR)
-    family = sssp_family.create_from_folder(my_path, label)
-    family.store()
-    # return family
+    subprocess.run(
+        [
+            "aiida-pseudo",
+            "install",
+            "sssp",
+            "-p",
+            "efficiency",
+            "-x",
+            "PBE",
+            "-v",
+            "1.2",
+        ]
+    )
 
 
 @pytest.fixture
 def fixture_localhost(aiida_localhost):
     """Return a localhost `Computer`."""
     localhost = aiida_localhost
     localhost.set_default_mpiprocs_per_machine(1)
@@ -87,17 +86,14 @@
             code.set_append_text(append_text)
 
         return code.store()
 
     return get_code
 
 
-# --------------------------------------------------------------------------------------
-
-
 @pytest.fixture(scope="function")
 def qe_pw_code(local_code_factory):
     return local_code_factory("quantumespresso.pw", "pw.x")
 
 
 @pytest.fixture(scope="function")
 def qe_pp_code(local_code_factory):
```

### Comparing `aiida_nanotech_empa-1.0.0b2/examples/workflows/aa` & `aiida_nanotech_empa-1.0.0b3/examples/workflows/aa`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/examples/workflows/benzene-diradical.xyz` & `aiida_nanotech_empa-1.0.0b3/examples/workflows/benzene-diradical.xyz`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/examples/workflows/c2h2_on_au111.xyz` & `aiida_nanotech_empa-1.0.0b3/examples/workflows/c2h2_on_au111.xyz`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/examples/workflows/c2h4.xyz` & `aiida_nanotech_empa-1.0.0b3/examples/workflows/c2h4.xyz`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_ads_gw_ic.py` & `aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_ads_gw_ic.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_afm.py` & `aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_afm.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_diag.py` & `aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_diag.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_fragment_separation.py` & `aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_fragment_separation.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_geo_opt.py` & `aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_geo_opt.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_gw.py` & `aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_gw.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_hrstm.py` & `aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_hrstm.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_mol_opt_gw.py` & `aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_mol_opt_gw.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_neb.py` & `aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_neb.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_orb.py` & `aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_orb.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_pdos.py` & `aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_pdos.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_phonons.py` & `aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_phonons.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_replica_chain.py` & `aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_replica_chain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_stm.py` & `aiida_nanotech_empa-1.0.0b3/examples/workflows/example_cp2k_stm.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_gaussian_casscf.py` & `aiida_nanotech_empa-1.0.0b3/examples/workflows/example_gaussian_casscf.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_gaussian_spin.py` & `aiida_nanotech_empa-1.0.0b3/examples/workflows/example_gaussian_spin.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_nanoribbon.py` & `aiida_nanotech_empa-1.0.0b3/examples/workflows/example_nanoribbon.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,103 +1,107 @@
-import os
+import pathlib
 
-from aiida.engine import run_get_node
-from aiida.orm import Bool, Float, Int, Str, load_code
-from aiida.plugins import DataFactory, WorkflowFactory
-from ase.io import read
+import ase.io
+import click
+from aiida import engine, orm, plugins
 
 from aiida_nanotech_empa.utils.cube_utils import cube_from_qe_pp_arraydata
 
 # AiiDA classes.
-StructureData = DataFactory("core.structure")
-NanoribbonWorkChain = WorkflowFactory("nanotech_empa.nanoribbon")
+NanoribbonWorkChain = plugins.WorkflowFactory("nanotech_empa.nanoribbon")
 
-DATA_DIR = os.path.dirname(os.path.abspath(__file__))
-OUTPUT_DIR = os.path.dirname(os.path.abspath(__file__))
+DATA_DIR = pathlib.Path(__file__).parent.absolute()
+OUTPUT_DIR = pathlib.Path(__file__).parent.absolute()
 
 
 def _example_nanoribbon(
     opt_cell, qe_pw_code, qe_pp_code, qe_projwfc_code, geo_file, description
 ):
     builder = NanoribbonWorkChain.get_builder()
 
     # Calculation settings.
-    builder.optimize_cell = Bool(opt_cell)
-    builder.max_kpoints = Int(2)
-    builder.precision = Float(0.0)
+    builder.optimize_cell = orm.Bool(opt_cell)
+    builder.max_kpoints = orm.Int(2)
+    builder.precision = orm.Float(0.0)
 
     # Resources.
-    builder.max_nodes = Int(1)
-    builder.mem_node = Int(32)
+    builder.max_nodes = orm.Int(1)
+    builder.mem_node = orm.Int(32)
 
     # Codes.
     builder.pw_code = qe_pw_code
     builder.pp_code = qe_pp_code
     builder.projwfc_code = qe_projwfc_code
 
     # Inputs
-    builder.structure = StructureData(ase=read(geo_file))
-    # builder.pseudo_family = Str("SSSP_modified")
-    builder.pseudo_family = Str(
-        "SSSP/1.1/PBE/efficiency"
+    builder.structure = orm.StructureData(ase=ase.io.read(geo_file))
+    # builder.pseudo_family = orm.Str("SSSP_modified")
+    builder.pseudo_family = orm.Str(
+        "SSSP/1.2/PBE/efficiency"
     )  # It requires aiida-pseudo install sssp!
 
     # Metadata
     builder.metadata = {
         "description": description,
         "label": "NanoribbonWorkChain",
     }
 
-    _, node = run_get_node(builder)
+    _, node = engine.run_get_node(builder)
 
     assert node.is_finished_ok
 
     if "spin_density_arraydata" in node.outputs:
         cube = cube_from_qe_pp_arraydata(node.outputs.spin_density_arraydata)
-        cube.write_cube_file(os.path.join(OUTPUT_DIR, "spin.cube"))
+        cube.write_cube_file(OUTPUT_DIR / "spin.cube")
         print("Wrote spin.cube!")
 
 
 def example_nanoribbon_no_spin(qe_pw_code, qe_pp_code, qe_projwfc_code):
     _example_nanoribbon(
         True,
         qe_pw_code,
         qe_pp_code,
         qe_projwfc_code,
-        os.path.join(DATA_DIR, "c2h2_no_spin.xyz"),
+        DATA_DIR / "c2h2_no_spin.xyz",
         "Test calculation no spin",
     )
 
 
 def example_nanoribbon_spin(qe_pw_code, qe_pp_code, qe_projwfc_code):
     _example_nanoribbon(
         True,
         qe_pw_code,
         qe_pp_code,
         qe_projwfc_code,
-        os.path.join(DATA_DIR, "c2h2_spin.xyz"),
+        DATA_DIR / "c2h2_spin.xyz",
         "Test calculation spin",
     )
 
 
 def example_nanoribbon_no_cell(qe_pw_code, qe_pp_code, qe_projwfc_code):
     _example_nanoribbon(
         False,
         qe_pw_code,
         qe_pp_code,
         qe_projwfc_code,
-        os.path.join(DATA_DIR, "c2h2_no_spin.xyz"),
+        DATA_DIR / "c2h2_no_spin.xyz",
         "Test calculation no cell opt",
     )
 
 
-if __name__ == "__main__":
+@click.command("cli")
+@click.argument("pw_code", default="pw@localhost")
+@click.argument("pp_code", default="pp@localhost")
+@click.argument("projwfc_code", default="projwfc@localhost")
+def run_all(pw_code, pp_code, projwfc_code):
     set_of_codes = (
-        load_code("pw@localhost"),
-        load_code("pp@localhost"),
-        load_code("projwfc@localhost"),
+        orm.load_code(pw_code),
+        orm.load_code(pp_code),
+        orm.load_code(projwfc_code),
     )
     example_nanoribbon_no_cell(*set_of_codes)
-
     example_nanoribbon_no_spin(*set_of_codes)
-
     example_nanoribbon_spin(*set_of_codes)
+
+
+if __name__ == "__main__":
+    run_all()
```

### Comparing `aiida_nanotech_empa-1.0.0b2/examples/workflows/h2_on_au111.xyz` & `aiida_nanotech_empa-1.0.0b3/examples/workflows/h2_on_au111.xyz`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/examples/workflows/h2_on_hbn.xyz` & `aiida_nanotech_empa-1.0.0b3/examples/workflows/h2_on_hbn.xyz`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/examples/workflows/si_bulk.xyz` & `aiida_nanotech_empa-1.0.0b3/examples/workflows/si_bulk.xyz`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b2/pyproject.toml` & `aiida_nanotech_empa-1.0.0b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering",
 ]
 requires-python = ">=3.8"
 dependencies = [
     "aiida-core~=2.2",
-    "aiida-quantumespresso~=4.1",
+    "aiida-quantumespresso<4.3",
     "aiida-pseudo~=1.0",
     "aiida-cp2k~=2.0",
     "ase~=3.21",
     "aiida-gaussian~=2.0",
     "pillow>=8.0.0",
     "more-itertools",
 ]
@@ -86,15 +86,15 @@
 "nanotech_empa.cp2k.phonons" = "aiida_nanotech_empa.workflows.cp2k:Cp2kPhononsWorkChain"
 
 
 [project.entry-points."aiida.schedulers"]
 slurm_ethz_euler = "aiida_nanotech_empa.schedulers:ETHZEulerSlurmScheduler"
 
 [tool.bumpver]
-current_version = "v1.0.0b2"
+current_version = "v1.0.0b3"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Bump version {old_version} -> {new_version}."
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `aiida_nanotech_empa-1.0.0b2/PKG-INFO` & `aiida_nanotech_empa-1.0.0b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-nanotech-empa
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: AiiDA plugins and workflows developed at nanotech@surfaces group from Empa.
 Author: nanotech@surfaces
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
 Classifier: Intended Audience :: Science/Research
@@ -12,15 +12,15 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: aiida-core~=2.2
-Requires-Dist: aiida-quantumespresso~=4.1
+Requires-Dist: aiida-quantumespresso<4.3
 Requires-Dist: aiida-pseudo~=1.0
 Requires-Dist: aiida-cp2k~=2.0
 Requires-Dist: ase~=3.21
 Requires-Dist: aiida-gaussian~=2.0
 Requires-Dist: pillow>=8.0.0
 Requires-Dist: more-itertools
 Requires-Dist: pgtest~=1.3.1 ; extra == "dev"
```

