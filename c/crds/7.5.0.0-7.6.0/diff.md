# Comparing `tmp/crds-7.5.0.0.tar.gz` & `tmp/crds-7.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/crds-7.5.0.0.tar", last modified: Wed May  6 12:53:13 2020, max compression
+gzip compressed data, was "dist/crds-7.6.0.tar", last modified: Wed Sep  2 13:39:42 2020, max compression
```

## Comparing `crds-7.5.0.0.tar` & `crds-7.6.0.tar`

### file list

```diff
@@ -1,1124 +1,1139 @@
-drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-06 12:53:13.275297 crds-7.5.0.0/
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       99 2020-05-04 16:42:34.000000 crds-7.5.0.0/MANIFEST.in
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     7678 2020-05-06 12:53:13.275505 crds-7.5.0.0/PKG-INFO
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     5681 2020-05-04 16:42:34.000000 crds-7.5.0.0/README.rst
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3029 2020-05-04 16:42:34.000000 crds-7.5.0.0/TESTING
--rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)      523 2020-05-04 16:42:34.000000 crds-7.5.0.0/clean
-drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-06 12:53:12.538512 crds-7.5.0.0/crds/
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3966 2020-05-05 02:57:32.000000 crds-7.5.0.0/crds/__init__.py
-drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-06 12:53:12.545319 crds-7.5.0.0/crds/bestrefs/
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      159 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/bestrefs/__init__.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      441 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/bestrefs/__main__.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    53328 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/bestrefs/bestrefs.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    18932 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/bestrefs/headers.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    23707 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/bestrefs/table_effects.py
-drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-06 12:53:12.553082 crds-7.5.0.0/crds/certify/
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      126 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/certify/__init__.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      329 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/certify/__main__.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    55112 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/certify/certify.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2140 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/certify/check_sha1sum.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    12850 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/certify/generic_tpn.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     5069 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/certify/mapping_parser.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    17166 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/certify/reftypes.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    14084 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/certify/validator_helpers.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    34006 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/certify/validators.py
-drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-06 12:53:12.555652 crds-7.5.0.0/crds/client/
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      339 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/client/__init__.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    38378 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/client/api.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     8589 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/client/proxy.py
-drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-06 12:53:12.574712 crds-7.5.0.0/crds/core/
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/core/__init__.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    39694 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/core/cmdline.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    57115 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/core/config.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      332 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/core/constants.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     9468 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/core/crds_cache_locking.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     7669 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/core/custom_dict.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    10351 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/core/exceptions.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      160 2020-05-05 02:57:32.000000 crds-7.5.0.0/crds/core/git_version.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    32574 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/core/heavy_client.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    17702 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/core/log.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     5631 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/core/mapping_verifier.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    10401 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/core/naming.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    13406 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/core/pysh.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      476 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/core/python23.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    85346 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/core/rmap.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)   114953 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/core/selectors.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     7929 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/core/substitutions.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    16639 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/core/timestamp.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    42479 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/core/utils.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     5431 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/data_file.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    47714 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/diff.py
-drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-06 12:53:12.584631 crds-7.5.0.0/crds/hst/
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1692 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/__init__.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/__main__.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    10668 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/acs.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      624 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/acs_common.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    11375 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/acs_v1.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     6024 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/acs_v2.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/cos.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    24548 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/locate.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/nicmos.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     7920 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/siname.py
-drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-06 12:53:12.707083 crds-7.5.0.0/crds/hst/specs/
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      528 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/acs_atodtab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      538 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/acs_biasfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      450 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/acs_bpixtab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      528 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/acs_ccdtab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      494 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/acs_cfltfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      551 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/acs_crrejtab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      447 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/acs_d2imfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      498 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/acs_darkfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      834 2020-05-05 20:47:17.000000 crds-7.5.0.0/crds/hst/specs/acs_dfltfile.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      458 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/acs_dgeofile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      534 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/acs_drkcfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      517 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/acs_flshfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      510 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/acs_idctab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      453 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/acs_imphttab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      531 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/acs_lfltfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      469 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/acs_mdriztab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      463 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/acs_mlintab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      448 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/acs_npolfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      440 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/acs_oscntab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      428 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/acs_pctetab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      759 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/acs_pfltfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      472 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/acs_shadfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      651 2020-05-05 20:47:17.000000 crds-7.5.0.0/crds/hst/specs/acs_snkcfile.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      477 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/acs_spottab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    99374 2020-05-05 20:47:22.000000 crds-7.5.0.0/crds/hst/specs/combined_specs.json
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      510 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/cos_badttab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      461 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/cos_bpixtab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      463 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/cos_brftab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      520 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/cos_brsttab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      449 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/cos_deadtab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      848 2020-05-05 20:47:17.000000 crds-7.5.0.0/crds/hst/specs/cos_dgeofile.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      519 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/cos_disptab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      437 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/cos_flatfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      568 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/cos_fluxtab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      462 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/cos_geofile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      444 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/cos_gsagtab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      449 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/cos_hvtab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      529 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/cos_lamptab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      482 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/cos_phatab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      524 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/cos_proftab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      692 2020-05-05 20:47:17.000000 crds-7.5.0.0/crds/hst/specs/cos_spottab.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      570 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/cos_spwcstab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      547 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/hst/specs/cos_tdstab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      514 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/cos_tracetab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      552 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/cos_twozxtab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      525 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/cos_walktab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      491 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/cos_wcptab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      530 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/cos_xtractab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      882 2020-05-05 20:47:17.000000 crds-7.5.0.0/crds/hst/specs/cos_xwlkfile.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      882 2020-05-05 20:47:17.000000 crds-7.5.0.0/crds/hst/specs/cos_ywlkfile.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      396 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/nicmos_backtab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      488 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/nicmos_darkfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      415 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/nicmos_flatfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      430 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/nicmos_idctab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      430 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/nicmos_illmfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      399 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/nicmos_maskfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      417 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/nicmos_nlinfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      426 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/nicmos_noisfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      389 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/nicmos_pedsbtab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      413 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/nicmos_phottab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      404 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/nicmos_pmodfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      403 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/nicmos_pmskfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      420 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/nicmos_rnlcortb.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      405 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/nicmos_saacntab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      401 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/nicmos_saadfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      438 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/nicmos_tdffile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      424 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/nicmos_tempfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      414 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/nicmos_zprattab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      456 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_apdestab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      432 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_apertab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      465 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_biasfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      495 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_bpixtab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      479 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_ccdtab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      501 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_cdstab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      466 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_crrejtab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      489 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_darkfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      491 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_disptab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      503 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_echsctab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      519 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_exstab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      529 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_gactab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      487 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_halotab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      484 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_idctab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      444 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_imphttab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      500 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_inangtab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      494 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_lamptab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      559 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_lfltfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      435 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_mlintab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      514 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_mofftab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      517 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_pctab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      569 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_pfltfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      482 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_phottab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      498 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_riptab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      523 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_sdctab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      485 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_sptrctab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      522 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_srwtab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      446 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_tdctab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      468 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_tdstab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      492 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_teltab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      473 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_wcptab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      509 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/stis_xtractab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      825 2020-05-05 20:47:17.000000 crds-7.5.0.0/crds/hst/specs/synphot_thermal.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      834 2020-05-05 20:47:17.000000 crds-7.5.0.0/crds/hst/specs/synphot_thruput.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      753 2020-05-05 20:47:17.000000 crds-7.5.0.0/crds/hst/specs/synphot_tmctab.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      778 2020-05-05 20:47:17.000000 crds-7.5.0.0/crds/hst/specs/synphot_tmgtab.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      751 2020-05-05 20:47:17.000000 crds-7.5.0.0/crds/hst/specs/synphot_tmttab.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      532 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfc3_atodtab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      670 2020-05-05 20:47:17.000000 crds-7.5.0.0/crds/hst/specs/wfc3_biacfile.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      521 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfc3_biasfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      478 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfc3_bpixtab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      518 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfc3_ccdtab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      561 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfc3_crrejtab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      451 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfc3_d2imfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      653 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfc3_darkfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      547 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfc3_dfltfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      674 2020-05-05 20:47:17.000000 crds-7.5.0.0/crds/hst/specs/wfc3_drkcfile.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      535 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfc3_flshfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      492 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfc3_idctab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      490 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfc3_imphttab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      463 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfc3_lfltfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      488 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfc3_mdriztab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      452 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfc3_nlinfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      465 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfc3_npolfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      458 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfc3_oscntab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      645 2020-05-05 20:47:17.000000 crds-7.5.0.0/crds/hst/specs/wfc3_pctetab.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      591 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfc3_pfltfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      476 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfc3_shadfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      659 2020-05-05 20:47:17.000000 crds-7.5.0.0/crds/hst/specs/wfc3_snkcfile.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      431 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfpc2_atodfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      401 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfpc2_biasfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      412 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfpc2_darkfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      433 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfpc2_dgeofile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      456 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfpc2_flatfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      478 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfpc2_idctab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      396 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfpc2_maskfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      434 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfpc2_offtab.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      422 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfpc2_shadfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      402 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/specs/wfpc2_wf4tfile.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/stis.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    12747 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/substitutions.dat
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/synphot.py
-drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-06 12:53:12.990604 crds-7.5.0.0/crds/hst/tpns/
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      636 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_a2d.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      837 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_a2d_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1879 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_bia.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2007 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_bia_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      723 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_bpx.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      932 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_bpx_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      796 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/hst/tpns/acs_ccd.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      862 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_ccd_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      889 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_cfl.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1421 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_cfl_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      505 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_crr.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      708 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_crr_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      560 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_csp.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      763 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_csp_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2757 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_cte.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1145 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_cte_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      730 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_d2i.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      995 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_d2i_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      861 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_dfl.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      937 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_dfl_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      796 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_dkc.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1084 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_dkc_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      635 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_drk.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      846 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_drk_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1311 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_dxy.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1649 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_dxy_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      672 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_fls.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      885 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_fls_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1275 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_idc.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1461 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_idc_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1193 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_imp.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1002 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_imp_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1147 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_lfl.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1445 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_lfl_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      464 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_lin.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      684 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_lin_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      488 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_mdz.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      688 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_mdz_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1679 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_npl.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1920 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_npl_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      482 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_osc.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      749 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_osc_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1564 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_pfl.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1851 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_pfl_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      476 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_shd.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      684 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_shd_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      573 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_snk.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      834 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/acs_snk_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1909 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_1dx.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2045 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_1dx_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1356 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_2zx.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1541 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_2zx_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      837 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_badt.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1092 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_badt_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      728 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_bpix.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      974 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_bpix_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      775 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_brf.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1023 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_brf_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      820 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_burst.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1078 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_burst_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      777 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_dead.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1032 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_dead_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      401 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_dgeo.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      685 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_dgeo_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1710 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_disp.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1962 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_disp_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1107 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_flat.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1367 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_flat_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      727 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_geo.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      969 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_geo_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1141 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_gsag.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1101 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_gsag_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      948 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_hv.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1033 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_hv_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1642 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_lamp.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1898 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_lamp_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      885 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_pha.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1125 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_pha_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1791 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_phot.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2039 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_phot_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1341 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_profile.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1481 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_profile_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1170 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_spot.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      938 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_spot_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1637 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_spwcs.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1880 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_spwcs_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1090 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/hst/tpns/cos_tds.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1351 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/hst/tpns/cos_tds_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1337 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_trace.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1473 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_trace_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      868 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_walk.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1146 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_walk_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      987 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_wcp.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1247 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_wcp_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      421 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_xwalk.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      690 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_xwalk_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      421 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_ywalk.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      690 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/cos_ywalk_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1155 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/foc_bac.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1047 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/foc_bac_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1536 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/foc_blm.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1244 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/foc_blm_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      762 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/foc_cuni.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1085 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/foc_cuni_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1536 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/foc_geo.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1424 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/foc_geo_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1436 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/foc_itf.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1235 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/foc_itf_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1006 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/foc_lsf.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1018 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/foc_lsf_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1371 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/foc_sde.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1080 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/foc_sde_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1462 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/foc_uni.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1125 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/foc_uni_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1700 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ais.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1188 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ais_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1200 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_bac.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1041 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_bac_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      921 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccg2.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      995 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccg2_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      723 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccs0.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1137 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccs0_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      652 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccs1.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1076 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccs1_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      752 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccs2.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1154 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccs2_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      654 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccs3.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1002 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccs3_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1101 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccs4.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1114 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccs4_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      821 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccs5.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1203 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccs5_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1261 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccs6.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1291 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccs6_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      564 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccs7.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1002 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccs7_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      609 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccs8.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1002 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccs8_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      652 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccs9.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1076 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccs9_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      509 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccsa.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      957 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccsa_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1036 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccsb.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1158 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccsb_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      705 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccsc.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1084 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccsc_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      697 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccsd.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1076 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccsd_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      748 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccse.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      952 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccse_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1239 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccsf.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      952 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ccsf_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1001 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ddt.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1001 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ddt_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1595 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_flt.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1328 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_flt_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1556 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ivs.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1346 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ivs_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1073 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_lsf.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      788 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_lsf_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1280 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_pcp.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1197 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_pcp_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1198 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_psf.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1037 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_psf_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1540 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_qin.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1406 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_qin_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1435 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ret.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1150 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/fos_ret_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1088 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_abs.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1032 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_abs_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      692 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccr1.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1027 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccr1_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      872 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccr2.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      995 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccr2_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1547 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccr3.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      995 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccr3_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      595 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccr4.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1033 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccr4_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      775 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccr5.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1033 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccr5_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1900 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccr6.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1033 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccr6_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      910 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccr7.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1033 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccr7_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      741 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccr8.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1114 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccr8_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      685 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccr9.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1068 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccr9_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      730 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccra.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1033 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccra_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      782 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccrb.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1110 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccrb_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2350 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccrc.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1033 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccrc_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      737 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccrd.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      995 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccrd_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      590 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccre.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      957 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_ccre_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1048 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_dio.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      994 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_dio_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1141 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_net.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1032 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_net_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1255 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_phc.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1032 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_phc_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1041 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_qin.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      994 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_qin_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1008 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_saa.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      956 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_saa_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      422 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_scoffc.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      957 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_scoffc_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1345 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_vig.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1032 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hrs_vig_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      490 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hsp_ccp0.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      993 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hsp_ccp0_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1310 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hsp_ccp1.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1059 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hsp_ccp1_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1228 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hsp_ccp2.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1026 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hsp_ccp2_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1228 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hsp_ccp3.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1024 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hsp_ccp3_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1269 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hsp_ccp4.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1028 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hsp_ccp4_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1310 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hsp_ccp5.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1060 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hsp_ccp5_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      490 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hsp_ccp6.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1024 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hsp_ccp6_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1228 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hsp_ccp7.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1026 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hsp_ccp7_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      613 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hsp_ccp8.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1061 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hsp_ccp8_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      490 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hsp_ccp9.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1028 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/hsp_ccp9_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1357 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_bkg.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1675 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_bkg_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1111 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_drk.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1443 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_drk_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1333 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_flt.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1675 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_flt_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      715 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_idc.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1057 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_idc_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1359 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_ilm.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1675 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_ilm_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      662 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_lin.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1004 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_lin_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      662 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_msk.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1004 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_msk_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      715 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_nlc.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1057 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_nlc_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      756 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_noi.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1096 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_noi_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      745 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_pht.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      956 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_pht_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      845 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_pmd.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1057 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_pmd_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      715 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_pmk.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1057 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_pmk_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      614 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_psb.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      956 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_psb_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      614 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_scn.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      956 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_scn_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      715 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_sdk.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1057 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_sdk_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      913 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_tdd.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1004 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_tdd_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1415 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_tdf.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1675 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_tdf_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      656 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_zpr.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      998 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/nic_zpr_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1733 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_1dt.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2127 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_1dt_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2807 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_1dx.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3183 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_1dx_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      774 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_a2d.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1109 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_a2d_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      970 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_any_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1738 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_apd.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2069 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_apd_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1743 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_apt.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2069 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_apt_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      765 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_bia.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1033 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_bia_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      680 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_bpx.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      988 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_bpx_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      923 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_ccd.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1226 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_ccd_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      761 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_cds.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1011 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_cds_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      753 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_crr.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1009 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_crr_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      686 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_dfl.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      988 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_dfl_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      794 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_drk.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1100 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_drk_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1862 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_dsp.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2251 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_dsp_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      761 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_ech.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1011 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_ech_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      770 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_exs.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1011 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_exs_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2825 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_gac.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3181 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_gac_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      748 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_hal.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1011 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_hal_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1861 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_iac.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2292 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_iac_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1118 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_idc.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1206 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_idc_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1622 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_imp.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1013 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_imp_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3230 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_lfl.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3353 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_lfl_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      681 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_lin.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      984 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_lin_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      630 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_lmp.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      922 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_lmp_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1705 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_moc.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2099 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_moc_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3235 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_pct.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3530 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_pct_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3256 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_pfl.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3550 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_pfl_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1932 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_pht.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2367 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_pht_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1049 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_rip.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1311 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_rip_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1873 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_sdc.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2127 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_sdc_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1067 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_srw.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1311 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_srw_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      679 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_ssc.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      970 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_ssc_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      704 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_ssd.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      988 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_ssd_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      668 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_tdc.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1023 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_tdc_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1099 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_tds.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1435 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_tds_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      680 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_tel.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      943 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_tel_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      905 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_wcp.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1160 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/stis_wcp_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1116 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/hst/tpns/synphot_syn.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1116 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/hst/tpns/synphot_syn_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      924 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/synphot_th.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      924 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/synphot_th_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      834 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/synphot_tmc.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      822 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/synphot_tmc_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      939 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/synphot_tmg.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      939 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/synphot_tmg_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      968 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/synphot_tmt.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      953 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/synphot_tmt_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      602 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_a2d.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      802 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_a2d_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1612 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_bia.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1962 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_bia_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1213 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_bic.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1441 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_bic_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      640 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_bpx.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      852 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_bpx_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      814 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_ccd.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1017 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_ccd_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      497 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_crr.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      715 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_crr_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2466 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_cte.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      839 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_cte_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      733 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_d2i.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      997 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_d2i_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      540 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_dfl.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      753 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_dfl_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1404 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_dkc.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1525 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_dkc_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      726 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_drk.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      944 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_drk_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      700 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_fls.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      952 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_fls_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      663 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_idc.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      855 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_idc_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1282 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_imp.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      999 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_imp_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      562 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_lfl.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      765 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_lfl_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      680 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_lin.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1004 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_lin_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      485 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_mdz.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      685 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_mdz_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      809 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_npl.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1050 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_npl_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      572 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_osc.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      840 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_osc_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      565 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_pfl.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      765 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_pfl_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      474 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_shd.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      682 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_shd_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      592 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_snk.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      839 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfc3_snk_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1861 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfp_a2d.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1152 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfp_a2d_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1247 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfp_bas.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1152 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfp_bas_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1391 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfp_dfl.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1230 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfp_dfl_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1425 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfp_dqf.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1230 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfp_dqf_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2061 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfp_drk.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1230 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfp_drk_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1391 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfp_flt.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1230 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfp_flt_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1394 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfp_msk.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1230 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfp_msk_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      825 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfp_phot.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1175 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfp_phot_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1391 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfp_prf.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1230 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfp_prf_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2126 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfp_psf.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1217 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfp_psf_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1392 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfp_spg.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1230 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wfp_spg_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1271 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wp2_a2d.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1090 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wp2_a2d_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1229 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wp2_bas.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1049 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wp2_bas_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1297 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wp2_dqf.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1163 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wp2_dqf_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1280 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wp2_drk.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1090 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wp2_drk_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      511 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wp2_dxy.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      743 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wp2_dxy_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1409 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wp2_flt.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1077 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wp2_flt_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      781 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wp2_idc.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      958 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wp2_idc_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1223 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wp2_msk.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1040 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wp2_msk_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      676 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wp2_off.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      958 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wp2_off_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      922 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wp2_phot.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1035 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wp2_phot_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2241 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wp2_psf.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1268 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wp2_shd.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1078 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wp2_shd_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      973 2020-05-04 16:42:34.000000 crds-7.5.0.0/crds/hst/tpns/wp2_w4t.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1018 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/hst/tpns/wp2_w4t_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     8420 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/hst/wfc3.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    12771 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/hst/wfpc2.py
-drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-06 12:53:12.996219 crds-7.5.0.0/crds/io/
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/io/__init__.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    13890 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/io/abstract.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2054 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/io/asdf.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     4891 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/io/factory.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    10076 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/io/fits.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     6350 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/io/geis.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      815 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/io/json.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3408 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/io/tables.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      841 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/io/yaml.py
-drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-06 12:53:13.009122 crds-7.5.0.0/crds/jwst/
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      975 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/__init__.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/__main__.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/fgs.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     9007 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/gen_system_crdscfg.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    27238 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/jwst_system_crdscfg_b7.1.1.yaml
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    28294 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/jwst_system_crdscfg_b7.1.3.yaml
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    27329 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/jwst_system_crdscfg_b7.1.yaml
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    29137 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/jwst_system_crdscfg_b7.2.yaml
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    35563 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/jwst_system_crdscfg_b7.3.yaml
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    36866 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/jwst_system_crdscfg_b7.4.yaml
--rw-r--r--   0 eisenham  (1009) STSCI\science  (1031)    35961 2020-05-04 21:54:20.000000 crds-7.5.0.0/crds/jwst/jwst_system_crdscfg_b7.5.yaml
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    33748 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/jwst_system_crdscfg_b7.yaml
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    24052 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/locate.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/miri.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/nircam.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/niriss.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/nirspec.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    17192 2020-05-04 21:57:20.000000 crds-7.5.0.0/crds/jwst/pipeline.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     9344 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/schema.py
-drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-06 12:53:13.101085 crds-7.5.0.0/crds/jwst/specs/
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      198 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/all_all.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      258 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/all_dark.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      231 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/all_gain.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      244 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/all_ipc.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      268 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/all_photom.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      316 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/all_rscd.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      300 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/all_throughput.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      280 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/all_trappars.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)   143906 2020-05-05 20:47:23.000000 crds-7.5.0.0/crds/jwst/specs/combined_specs.json
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1161 2020-05-05 20:47:20.000000 crds-7.5.0.0/crds/jwst/specs/fgs_abvegaoffset.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      220 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/fgs_all.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      506 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/fgs_amplifier.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3888 2020-05-05 20:47:20.000000 crds-7.5.0.0/crds/jwst/specs/fgs_apcorr.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      449 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/fgs_area.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      459 2020-05-05 20:47:20.000000 crds-7.5.0.0/crds/jwst/specs/fgs_dark.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      610 2020-05-05 20:47:21.000000 crds-7.5.0.0/crds/jwst/specs/fgs_distortion.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      434 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/fgs_drizpars.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      453 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/fgs_flat.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      462 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/fgs_gain.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      472 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/fgs_ipc.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      498 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/fgs_linearity.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      472 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/fgs_mask.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      469 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/fgs_persat.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      473 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/fgs_photom.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      488 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/fgs_readnoise.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      325 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/fgs_regions.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      471 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/fgs_saturation.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      355 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/fgs_specwcs.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      506 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/fgs_superbias.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      490 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/fgs_trapdensity.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      478 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/fgs_trappars.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      361 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/fgs_wcsregions.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1163 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/miri_abvegaoffset.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      211 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/miri_all.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      508 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/miri_amplifier.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3938 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/miri_apcorr.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      480 2020-05-05 20:47:21.000000 crds-7.5.0.0/crds/jwst/specs/miri_area.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      603 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/miri_cubepar.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      492 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/miri_dark.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      640 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/miri_distortion.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      436 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/miri_drizpars.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      559 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/miri_extract1d.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      661 2020-05-05 20:47:17.000000 crds-7.5.0.0/crds/jwst/specs/miri_filteroffset.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      531 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/miri_flat.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      508 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/miri_fringe.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      464 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/miri_gain.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      474 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/miri_ipc.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      491 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/miri_lastframe.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      501 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/miri_linearity.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      448 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/miri_mask.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      552 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/miri_pathloss.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      522 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/miri_persat.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      535 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/miri_photom.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      662 2020-05-05 20:47:21.000000 crds-7.5.0.0/crds/jwst/specs/miri_psfmask.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      490 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/miri_readnoise.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      677 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/miri_regions.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      655 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/miri_reset.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      580 2020-05-05 20:47:20.000000 crds-7.5.0.0/crds/jwst/specs/miri_resol.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      615 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/miri_rscd.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      474 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/miri_saturation.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      846 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/miri_specwcs.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      473 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/miri_straymask.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      543 2020-05-05 20:47:20.000000 crds-7.5.0.0/crds/jwst/specs/miri_trapdensity.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      531 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/miri_trappars.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      693 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/miri_tsophot.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      757 2020-05-05 20:47:20.000000 crds-7.5.0.0/crds/jwst/specs/miri_v2v3.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      598 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/miri_wavelengthrange.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      737 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/miri_wcsregions.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1167 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/nircam_abvegaoffset.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      219 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nircam_all.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      512 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nircam_amplifier.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3906 2020-05-05 20:47:20.000000 crds-7.5.0.0/crds/jwst/specs/nircam_apcorr.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      509 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/nircam_area.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      496 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nircam_dark.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      704 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/nircam_distortion.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      440 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nircam_drizpars.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      708 2020-05-05 20:47:20.000000 crds-7.5.0.0/crds/jwst/specs/nircam_filteroffset.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      495 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nircam_flat.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      468 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nircam_gain.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      478 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nircam_ipc.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      507 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nircam_linearity.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      478 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nircam_mask.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      475 2020-05-05 20:47:17.000000 crds-7.5.0.0/crds/jwst/specs/nircam_persat.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      561 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nircam_photom.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      670 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/nircam_psfmask.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      494 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nircam_readnoise.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      331 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nircam_regions.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      480 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nircam_saturation.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      802 2020-05-05 20:47:21.000000 crds-7.5.0.0/crds/jwst/specs/nircam_specwcs.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      361 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nircam_specwcs.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      512 2020-05-05 20:47:20.000000 crds-7.5.0.0/crds/jwst/specs/nircam_superbias.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      496 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/nircam_trapdensity.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      484 2020-05-05 20:47:20.000000 crds-7.5.0.0/crds/jwst/specs/nircam_trappars.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      703 2020-05-05 20:47:20.000000 crds-7.5.0.0/crds/jwst/specs/nircam_tsophot.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      609 2020-05-05 20:47:20.000000 crds-7.5.0.0/crds/jwst/specs/nircam_wavelengthrange.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      367 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nircam_wcsregions.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      701 2020-05-05 20:47:20.000000 crds-7.5.0.0/crds/jwst/specs/nircam_wfssbkg.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1167 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/niriss_abvegaoffset.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      219 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/niriss_all.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      512 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/niriss_amplifier.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3906 2020-05-05 20:47:17.000000 crds-7.5.0.0/crds/jwst/specs/niriss_apcorr.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      509 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/niriss_area.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      472 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/niriss_dark.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      554 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/niriss_distortion.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      440 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/niriss_drizpars.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      563 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/niriss_extract1d.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      465 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/niriss_flat.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      468 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/niriss_gain.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      478 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/niriss_ipc.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      507 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/niriss_linearity.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      454 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/niriss_mask.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      587 2020-05-05 20:47:20.000000 crds-7.5.0.0/crds/jwst/specs/niriss_pathloss.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      475 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/niriss_persat.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      539 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/niriss_photom.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      494 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/niriss_readnoise.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      331 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/niriss_regions.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      480 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/niriss_saturation.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1085 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/niriss_specwcs.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      512 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/niriss_superbias.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      513 2020-05-05 20:47:21.000000 crds-7.5.0.0/crds/jwst/specs/niriss_throughput.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      496 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/niriss_trapdensity.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      484 2020-05-05 20:47:17.000000 crds-7.5.0.0/crds/jwst/specs/niriss_trappars.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      609 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/niriss_wavelengthrange.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      367 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/niriss_wcsregions.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      700 2020-05-05 20:47:20.000000 crds-7.5.0.0/crds/jwst/specs/niriss_wfssbkg.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      223 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_all.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      514 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_amplifier.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3904 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_apcorr.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      572 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_area.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      551 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_badshutter.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      741 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_barshadow.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      559 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_camera.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      573 2020-05-05 20:47:20.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_collimator.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      762 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_cubepar.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      498 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_dark.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      562 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_dflat.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      641 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_disperser.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      529 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_distortion.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      442 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_drizpars.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      565 2020-05-05 20:47:20.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_extract1d.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      587 2020-05-05 20:47:21.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_fflat.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      517 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_flat.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      642 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_fore.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      569 2020-05-05 20:47:20.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_fpa.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      470 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_gain.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      538 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_ifufore.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      538 2020-05-05 20:47:21.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_ifupost.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      548 2020-05-05 20:47:17.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_ifuslicer.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      480 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_ipc.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      510 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_linearity.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      480 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_mask.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      571 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_msa.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      663 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_msaoper.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      582 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_ote.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      558 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_pathloss.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      477 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_persat.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      513 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_photom.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      496 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_readnoise.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      613 2020-05-05 20:47:20.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_refpix.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      872 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_regions.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      483 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_saturation.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      644 2020-05-05 20:47:20.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_sflat.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      679 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_specwcs.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      514 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_superbias.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      498 2020-05-05 20:47:20.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_trapdensity.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      486 2020-05-05 20:47:19.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_trappars.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      568 2020-05-05 20:47:21.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_wavecorr.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      606 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_wavelengthrange.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      369 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/specs/nirspec_wcsregions.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      561 2020-05-05 20:47:18.000000 crds-7.5.0.0/crds/jwst/specs/system_calver.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      612 2020-05-05 20:47:20.000000 crds-7.5.0.0/crds/jwst/specs/system_crdscfg.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      638 2020-05-05 20:47:20.000000 crds-7.5.0.0/crds/jwst/specs/system_datalvl.rmap
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        3 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/substitutions.dat
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       52 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/system.py
-drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-06 12:53:13.177637 crds-7.5.0.0/crds/jwst/tpns/
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2754 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/all_all.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2754 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/all_all_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      715 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/all_dark.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      715 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/all_dark_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       37 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/all_gain.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      459 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/all_ipc.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       67 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/all_photom.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      348 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/all_throughput.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      749 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/all_trappars.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1840 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/fgs_all.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1840 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/fgs_all_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      552 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/jwst/tpns/fgs_apcorr.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      276 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/fgs_area.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      521 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/fgs_dark.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       37 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/fgs_distortion.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      185 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/fgs_flat.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      120 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/fgs_gain.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       35 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/fgs_linearity.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       30 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/fgs_mask.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       76 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/fgs_persat.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/fgs_photom.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      150 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/fgs_readnoise.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      282 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/fgs_saturation.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      186 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/fgs_superbias.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       76 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/fgs_trapdensity.tpn
-drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-06 12:53:13.197285 crds-7.5.0.0/crds/jwst/tpns/includes/
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1104 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/jwst/tpns/includes/apcorr.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      971 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/miri_dq_array.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      824 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/miri_dq_def_array.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      482 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/miri_err_array.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      796 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/miri_sci_array_both.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       81 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/miri_sci_array_norefpix.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       81 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/miri_sci_array_refpix.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1592 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/miri_subarray_both.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       56 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/miri_subarray_norefpix.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      134 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/miri_subarray_refpix.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      412 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/nir_dq_array.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      827 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/nir_dq_def_array.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      455 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/nir_err_array.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      372 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/nir_linearity.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      261 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/nir_mask.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      582 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/nir_opt_err_array.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      626 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/nir_photom.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1707 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/nir_sci_array_both.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      239 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/nir_sci_array_norefpix.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      235 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/nir_sci_array_refpix.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3236 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/nir_subarray.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      755 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/nir_subarray_baseline.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      934 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/nirspec_dq_array.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      529 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/nirspec_err_array.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      562 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/nirspec_opt_err_array.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1922 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/nirspec_sci_array_both.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       91 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/nirspec_sci_array_norefpix.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       91 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/nirspec_sci_array_refpix.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1540 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/includes/nirspec_sci_array_striped.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      747 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/jwst/tpns/includes/nirspec_subarray_baseline.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1830 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/jwst/tpns/miri_all.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1830 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/jwst/tpns/miri_all_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      354 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/miri_area.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      243 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/miri_cubepar.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      312 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/miri_dark.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       45 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/miri_distortion.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      197 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/miri_flat.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      324 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/miri_fringe.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      129 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/miri_gain.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      154 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/miri_lastframe.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1192 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/miri_linearity.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      262 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/miri_mask.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/miri_photom.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      153 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/miri_psfmask.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      159 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/miri_readnoise.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      364 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/miri_reset.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3264 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/jwst/tpns/miri_rscd.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      292 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/miri_saturation.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       44 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/miri_specwcs.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      308 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/miri_straymask.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      457 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/miri_tsophot.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3046 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nircam_all.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3046 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nircam_all_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      707 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/jwst/tpns/nircam_apcorr.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      276 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nircam_area.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      298 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nircam_dark.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       37 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nircam_distortion.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      187 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nircam_flat.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      120 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nircam_gain.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       36 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nircam_linearity.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       31 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nircam_mask.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       76 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nircam_persat.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nircam_photom.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      233 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nircam_psfmask.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      150 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nircam_readnoise.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      283 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nircam_saturation.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      186 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nircam_superbias.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       76 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nircam_trapdensity.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      459 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nircam_tsophot.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      384 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nircam_wfssbkg.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1243 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/niriss_all.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1243 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/niriss_all_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      535 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/jwst/tpns/niriss_apcorr.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      276 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/niriss_area.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      298 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/niriss_dark.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       37 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/niriss_distortion.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      185 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/niriss_flat.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      120 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/niriss_gain.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       36 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/niriss_linearity.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       31 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/niriss_mask.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      234 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/niriss_pathloss.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       76 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/niriss_persat.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        1 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/niriss_photom.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      150 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/niriss_readnoise.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      283 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/niriss_saturation.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       34 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/niriss_specwcs.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      186 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/niriss_superbias.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       76 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/niriss_trapdensity.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      384 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/niriss_wfssbkg.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1714 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nirspec_all.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1714 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nirspec_all_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1196 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/jwst/tpns/nirspec_apcorr.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1770 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nirspec_area.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1235 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nirspec_barshadow.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      229 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nirspec_cubepar.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      456 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nirspec_dark.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1364 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nirspec_dflat.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       37 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nirspec_distortion.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3246 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nirspec_fflat.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      226 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nirspec_gain.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      455 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nirspec_linearity.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      285 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nirspec_mask.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      637 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nirspec_pathloss.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      105 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nirspec_persat.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nirspec_photom.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      255 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nirspec_readnoise.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      795 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nirspec_refpix.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      442 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nirspec_saturation.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1718 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nirspec_sflat.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      301 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nirspec_superbias.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      107 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/jwst/tpns/nirspec_trapdensity.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    32752 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/list.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    16584 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/matches.py
-drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-06 12:53:13.204498 crds-7.5.0.0/crds/misc/
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/misc/__init__.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1827 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/misc/cal_pipelines.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     7449 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/misc/check_archive.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2789 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/misc/datalvl.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    11250 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/misc/get_synphot.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    26044 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/misc/query_affected.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     6349 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/misc/sql.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     8902 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/misc/uniqname.py
-drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-06 12:53:13.208224 crds-7.5.0.0/crds/refactoring/
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/refactoring/__init__.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     5012 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/refactoring/checksum.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     7815 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/refactoring/newcontext.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    10334 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/refactoring/refactor.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    33947 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/refactoring/refactor2.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    32384 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/rowdiff.py
-drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-06 12:53:13.213108 crds-7.5.0.0/crds/submit/
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      176 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/submit/__init__.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      205 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/submit/__main__.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3026 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/submit/background.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     5774 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/submit/monitor.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    14408 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/submit/rc_submit.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    16924 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/submit/submit.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     8877 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/submit/web.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    36425 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/sync.py
-drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-06 12:53:13.238863 crds-7.5.0.0/crds/tests/
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      237 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/__init__.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      514 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/compare_pickles.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1440 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/profile_bestrefs.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      892 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/profile_pickling.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     8336 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/test_bad_files.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    26773 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/tests/test_bestrefs.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3435 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/test_build6.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)   123303 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/tests/test_certify.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2051 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/test_check_archive.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     9101 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/test_checksum.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    10602 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/tests/test_cmdline.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     4125 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/test_config.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    41724 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/test_diff.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    11689 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/test_heavy_client.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    13957 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/test_io.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    27576 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/test_list.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     4743 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/tests/test_locking.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3845 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/tests/test_matches.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3579 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/test_newcontext.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     6585 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/test_or_bars.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     7557 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/test_refactor.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    16166 2020-05-04 16:42:38.000000 crds-7.5.0.0/crds/tests/test_reftypes.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    33929 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/test_rmap.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    10768 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/test_rowdiff.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    50865 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/test_special.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     9724 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/test_submit.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    12230 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/test_substitutions.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     4751 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/test_sync.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    29836 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/test_synphot_hst.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     5289 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/test_table_effects.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     5431 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/test_uniqname.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2956 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tests/test_uses.py
-drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-06 12:53:13.242754 crds-7.5.0.0/crds/tobs/
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      733 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tobs/__init__.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tobs/__main__.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    11292 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tobs/locate.py
-drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-06 12:53:13.243825 crds-7.5.0.0/crds/tobs/specs/
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      749 2020-05-05 20:47:23.000000 crds-7.5.0.0/crds/tobs/specs/combined_specs.json
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      437 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tobs/specs/tinstr_tfilekind.spec
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        3 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tobs/substitutions.dat
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    23945 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tobs/tests.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      123 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tobs/tinstr.py
-drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-06 12:53:13.245305 crds-7.5.0.0/crds/tobs/tpns/
--rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)      531 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tobs/tpns/tinstr_tfk.tpn
--rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)      531 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/tobs/tpns/tinstr_tfk_ld.tpn
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     6352 2020-05-04 16:42:35.000000 crds-7.5.0.0/crds/uses.py
-drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-06 12:53:12.541577 crds-7.5.0.0/crds.egg-info/
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     7678 2020-05-06 12:53:12.000000 crds-7.5.0.0/crds.egg-info/PKG-INFO
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    33038 2020-05-06 12:53:12.000000 crds-7.5.0.0/crds.egg-info/SOURCES.txt
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        1 2020-05-06 12:53:12.000000 crds-7.5.0.0/crds.egg-info/dependency_links.txt
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        1 2020-05-06 12:53:12.000000 crds-7.5.0.0/crds.egg-info/not-zip-safe
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      269 2020-05-06 12:53:12.000000 crds-7.5.0.0/crds.egg-info/requires.txt
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        5 2020-05-06 12:53:12.000000 crds-7.5.0.0/crds.egg-info/top_level.txt
-drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-06 12:53:13.266673 crds-7.5.0.0/envs/
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      336 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/crds-readonly.csh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      404 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/crds-tests.csh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      414 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/crds-tests.sh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2408 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/env-forwarded.csh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2373 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/env-local.csh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2457 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/hst-crds-dev.csh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2456 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/hst-crds-dev.sh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2388 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/hst-crds-ops.csh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2387 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/hst-crds-ops.sh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2379 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/hst-crds-readonly.csh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2378 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/hst-crds-readonly.sh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2394 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/hst-crds-test.csh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2393 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/hst-crds-test.sh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      124 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/hst-serverless.csh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2412 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/jwst-crds-b5it.csh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2412 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/jwst-crds-b6it.csh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2410 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/jwst-crds-bit.csh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2407 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/jwst-crds-bit.sh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2410 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/jwst-crds-cit.csh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2407 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/jwst-crds-cit.sh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2410 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/jwst-crds-dev.csh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2409 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/jwst-crds-dev.sh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2410 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/jwst-crds-dit.csh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2409 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/jwst-crds-dit.sh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2389 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/jwst-crds-ops.csh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2388 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/jwst-crds-ops.sh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2390 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/jwst-crds-readonly.csh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2389 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/jwst-crds-readonly.sh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2395 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/jwst-crds-test.csh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2398 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/jwst-crds-test.sh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      125 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/jwst-serverless.csh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      935 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/s3.sh
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      263 2020-05-04 16:42:35.000000 crds-7.5.0.0/envs/un-s3.sh
--rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)     2292 2020-05-04 16:42:35.000000 crds-7.5.0.0/install
-drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-05-06 12:53:13.274847 crds-7.5.0.0/scripts/
--rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)     2748 2020-05-04 16:42:35.000000 crds-7.5.0.0/scripts/crds
--rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)      281 2020-05-04 16:42:35.000000 crds-7.5.0.0/scripts/crds_cached_context
--rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)     1299 2020-05-04 16:42:35.000000 crds-7.5.0.0/scripts/crds_check_cache
--rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)     1676 2020-05-04 16:42:35.000000 crds-7.5.0.0/scripts/crds_dataset_capture
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1233 2020-05-04 16:42:35.000000 crds-7.5.0.0/scripts/crds_jwst_serverless_pipeline_env.csh
--rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)     4199 2020-05-04 16:42:35.000000 crds-7.5.0.0/scripts/crds_repair_cache
--rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)       71 2020-05-04 16:42:35.000000 crds-7.5.0.0/scripts/crds_s3_get
--rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)      902 2020-05-04 16:42:35.000000 crds-7.5.0.0/scripts/crds_unique
--rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)     5566 2020-05-04 16:42:35.000000 crds-7.5.0.0/scripts/cron_sync
--rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)      846 2020-05-04 16:42:35.000000 crds-7.5.0.0/scripts/custom_query_affected_datasets
--rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)     1348 2020-05-04 16:42:35.000000 crds-7.5.0.0/scripts/pipeline_bestref
--rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)      197 2020-05-04 16:42:35.000000 crds-7.5.0.0/scripts/query_affected_datasets
--rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)      530 2020-05-04 16:42:35.000000 crds-7.5.0.0/scripts/remote_cache_init
--rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)     1607 2020-05-04 16:42:35.000000 crds-7.5.0.0/scripts/safe_bestrefs
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      364 2020-05-06 12:53:13.276194 crds-7.5.0.0/setup.cfg
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3083 2020-05-05 02:57:32.000000 crds-7.5.0.0/setup.py
--rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1224 2020-05-04 16:42:35.000000 crds-7.5.0.0/setup_data.py
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:42.873893 crds-7.6.0/
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       99 2020-09-02 13:20:07.000000 crds-7.6.0/MANIFEST.in
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     7700 2020-09-02 13:39:42.874144 crds-7.6.0/PKG-INFO
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     5681 2020-09-02 13:20:07.000000 crds-7.6.0/README.rst
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3029 2020-09-02 13:20:07.000000 crds-7.6.0/TESTING
+-rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)      523 2020-09-02 13:20:07.000000 crds-7.6.0/clean
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:41.797171 crds-7.6.0/crds/
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3964 2020-09-02 13:24:37.000000 crds-7.6.0/crds/__init__.py
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:41.810274 crds-7.6.0/crds/bestrefs/
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      159 2020-09-02 13:20:07.000000 crds-7.6.0/crds/bestrefs/__init__.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      441 2020-09-02 13:20:07.000000 crds-7.6.0/crds/bestrefs/__main__.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    53328 2020-09-02 13:20:07.000000 crds-7.6.0/crds/bestrefs/bestrefs.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    18932 2020-09-02 13:20:07.000000 crds-7.6.0/crds/bestrefs/headers.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    23707 2020-09-02 13:20:07.000000 crds-7.6.0/crds/bestrefs/table_effects.py
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:41.817947 crds-7.6.0/crds/certify/
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      141 2020-09-02 13:20:12.000000 crds-7.6.0/crds/certify/__init__.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      329 2020-09-02 13:20:07.000000 crds-7.6.0/crds/certify/__main__.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    55134 2020-09-02 13:20:12.000000 crds-7.6.0/crds/certify/certify.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2140 2020-09-02 13:20:07.000000 crds-7.6.0/crds/certify/check_sha1sum.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    12850 2020-09-02 13:20:07.000000 crds-7.6.0/crds/certify/generic_tpn.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     5069 2020-09-02 13:20:07.000000 crds-7.6.0/crds/certify/mapping_parser.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    17166 2020-09-02 13:20:12.000000 crds-7.6.0/crds/certify/reftypes.py
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:41.820579 crds-7.6.0/crds/certify/validators/
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3000 2020-09-02 13:20:12.000000 crds-7.6.0/crds/certify/validators/__init__.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    33053 2020-09-02 13:20:12.000000 crds-7.6.0/crds/certify/validators/core.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    14084 2020-09-02 13:20:12.000000 crds-7.6.0/crds/certify/validators/helpers.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     8172 2020-09-02 13:20:12.000000 crds-7.6.0/crds/certify/validators/synphot.py
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:41.824866 crds-7.6.0/crds/client/
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      339 2020-09-02 13:20:07.000000 crds-7.6.0/crds/client/__init__.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    38378 2020-09-02 13:20:07.000000 crds-7.6.0/crds/client/api.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     8589 2020-09-02 13:20:07.000000 crds-7.6.0/crds/client/proxy.py
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:41.844465 crds-7.6.0/crds/core/
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:20:07.000000 crds-7.6.0/crds/core/__init__.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    39694 2020-09-02 13:20:07.000000 crds-7.6.0/crds/core/cmdline.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    57115 2020-09-02 13:20:07.000000 crds-7.6.0/crds/core/config.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      332 2020-09-02 13:20:07.000000 crds-7.6.0/crds/core/constants.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     9468 2020-09-02 13:20:07.000000 crds-7.6.0/crds/core/crds_cache_locking.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     7669 2020-09-02 13:20:07.000000 crds-7.6.0/crds/core/custom_dict.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    10351 2020-09-02 13:20:07.000000 crds-7.6.0/crds/core/exceptions.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      158 2020-09-02 13:24:37.000000 crds-7.6.0/crds/core/git_version.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    32574 2020-09-02 13:20:12.000000 crds-7.6.0/crds/core/heavy_client.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    17702 2020-09-02 13:20:07.000000 crds-7.6.0/crds/core/log.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     5631 2020-09-02 13:20:07.000000 crds-7.6.0/crds/core/mapping_verifier.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    10401 2020-09-02 13:20:07.000000 crds-7.6.0/crds/core/naming.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    13406 2020-09-02 13:20:07.000000 crds-7.6.0/crds/core/pysh.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      476 2020-09-02 13:20:07.000000 crds-7.6.0/crds/core/python23.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    85346 2020-09-02 13:20:12.000000 crds-7.6.0/crds/core/rmap.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)   114953 2020-09-02 13:20:07.000000 crds-7.6.0/crds/core/selectors.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     7929 2020-09-02 13:20:07.000000 crds-7.6.0/crds/core/substitutions.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    16639 2020-09-02 13:20:07.000000 crds-7.6.0/crds/core/timestamp.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    42479 2020-09-02 13:20:07.000000 crds-7.6.0/crds/core/utils.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     5431 2020-09-02 13:20:12.000000 crds-7.6.0/crds/data_file.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    47714 2020-09-02 13:20:07.000000 crds-7.6.0/crds/diff.py
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:41.855738 crds-7.6.0/crds/hst/
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1692 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/__init__.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/__main__.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    10668 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/acs.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      624 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/acs_common.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    11375 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/acs_v1.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     6024 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/acs_v2.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/cos.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    24556 2020-09-02 13:20:12.000000 crds-7.6.0/crds/hst/locate.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/nicmos.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     7920 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/siname.py
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:41.946700 crds-7.6.0/crds/hst/specs/
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      528 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/acs_atodtab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      538 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/acs_biasfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      450 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/acs_bpixtab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      528 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/acs_ccdtab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      494 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/acs_cfltfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      551 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/acs_crrejtab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      447 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/acs_d2imfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      498 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/acs_darkfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      834 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/acs_dfltfile.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      458 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/acs_dgeofile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      534 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/acs_drkcfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      517 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/acs_flshfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      510 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/acs_idctab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      453 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/acs_imphttab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      531 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/acs_lfltfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      469 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/acs_mdriztab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      463 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/acs_mlintab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      448 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/acs_npolfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      440 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/acs_oscntab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      428 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/acs_pctetab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      759 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/acs_pfltfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      472 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/acs_shadfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      651 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/acs_snkcfile.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      477 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/acs_spottab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)   100318 2020-09-02 13:20:12.000000 crds-7.6.0/crds/hst/specs/combined_specs.json
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      510 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/cos_badttab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      461 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/cos_bpixtab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      463 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/cos_brftab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      520 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/cos_brsttab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      449 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/cos_deadtab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      848 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/cos_dgeofile.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      519 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/cos_disptab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      437 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/cos_flatfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      568 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/cos_fluxtab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      462 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/cos_geofile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      444 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/cos_gsagtab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      449 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/cos_hvtab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      529 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/cos_lamptab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      482 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/cos_phatab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      524 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/cos_proftab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      692 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/cos_spottab.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      570 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/cos_spwcstab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      547 2020-09-02 13:20:12.000000 crds-7.6.0/crds/hst/specs/cos_tdstab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      514 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/cos_tracetab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      552 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/cos_twozxtab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      525 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/cos_walktab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      491 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/cos_wcptab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      530 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/cos_xtractab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      882 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/cos_xwlkfile.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      882 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/cos_ywlkfile.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      396 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/nicmos_backtab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      488 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/nicmos_darkfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      415 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/nicmos_flatfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      430 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/nicmos_idctab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      430 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/nicmos_illmfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      399 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/nicmos_maskfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      417 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/nicmos_nlinfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      426 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/nicmos_noisfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      389 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/nicmos_pedsbtab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      413 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/nicmos_phottab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      404 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/nicmos_pmodfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      403 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/nicmos_pmskfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      420 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/nicmos_rnlcortb.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      405 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/nicmos_saacntab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      401 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/nicmos_saadfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      438 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/nicmos_tdffile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      424 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/nicmos_tempfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      414 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/nicmos_zprattab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      456 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_apdestab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      432 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_apertab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      465 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_biasfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      495 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_bpixtab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      479 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_ccdtab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      501 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_cdstab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      466 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_crrejtab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      489 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_darkfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      491 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_disptab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      503 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_echsctab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      519 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_exstab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      529 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_gactab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      487 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_halotab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      484 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_idctab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      444 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_imphttab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      500 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_inangtab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      494 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_lamptab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      559 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_lfltfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      435 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_mlintab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      514 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_mofftab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      517 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_pctab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      569 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_pfltfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      482 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_phottab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      498 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_riptab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      523 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_sdctab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      485 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_sptrctab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      522 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_srwtab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      446 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_tdctab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      468 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_tdstab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      492 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_teltab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      473 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_wcptab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      509 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/stis_xtractab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      736 2020-09-02 13:20:12.000000 crds-7.6.0/crds/hst/specs/synphot_obsmodes.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      825 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/synphot_thermal.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      834 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/synphot_thruput.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      753 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/synphot_tmctab.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      778 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/synphot_tmgtab.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      751 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/synphot_tmttab.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      532 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfc3_atodtab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      670 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfc3_biacfile.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      521 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfc3_biasfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      478 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfc3_bpixtab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      518 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfc3_ccdtab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      561 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfc3_crrejtab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      451 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfc3_d2imfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      653 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfc3_darkfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      547 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfc3_dfltfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      674 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfc3_drkcfile.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      535 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfc3_flshfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      492 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfc3_idctab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      490 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfc3_imphttab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      463 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfc3_lfltfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      488 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfc3_mdriztab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      452 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfc3_nlinfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      465 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfc3_npolfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      458 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfc3_oscntab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      645 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfc3_pctetab.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      591 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfc3_pfltfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      476 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfc3_shadfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      659 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfc3_snkcfile.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      431 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfpc2_atodfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      401 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfpc2_biasfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      412 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfpc2_darkfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      433 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfpc2_dgeofile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      456 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfpc2_flatfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      478 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfpc2_idctab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      396 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfpc2_maskfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      434 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfpc2_offtab.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      422 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfpc2_shadfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      402 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/specs/wfpc2_wf4tfile.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/stis.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    12747 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/substitutions.dat
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/synphot.py
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:42.569536 crds-7.6.0/crds/hst/tpns/
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      636 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_a2d.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      837 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_a2d_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1879 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_bia.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2007 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_bia_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      723 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_bpx.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      932 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_bpx_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      796 2020-09-02 13:20:12.000000 crds-7.6.0/crds/hst/tpns/acs_ccd.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      862 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_ccd_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      889 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_cfl.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1421 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_cfl_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      505 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_crr.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      708 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_crr_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      560 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_csp.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      763 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_csp_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2757 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_cte.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1145 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_cte_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      730 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_d2i.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      995 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_d2i_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      861 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_dfl.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      937 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_dfl_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      796 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_dkc.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1084 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_dkc_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      635 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_drk.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      846 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_drk_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1311 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_dxy.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1649 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_dxy_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      672 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_fls.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      885 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_fls_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1275 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_idc.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1461 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_idc_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1193 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_imp.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1002 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_imp_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1147 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_lfl.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1445 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_lfl_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      464 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_lin.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      684 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_lin_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      488 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_mdz.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      688 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_mdz_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1679 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_npl.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1920 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_npl_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      482 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_osc.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      749 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_osc_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1564 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_pfl.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1851 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_pfl_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      476 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_shd.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      684 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_shd_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      573 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_snk.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      834 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/acs_snk_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1909 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_1dx.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2045 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_1dx_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1356 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_2zx.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1541 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_2zx_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      837 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_badt.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1092 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_badt_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      728 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_bpix.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      974 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_bpix_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      775 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_brf.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1023 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_brf_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      820 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_burst.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1078 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_burst_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      777 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_dead.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1032 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_dead_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      401 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_dgeo.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      685 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_dgeo_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1710 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_disp.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1962 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_disp_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1107 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_flat.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1367 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_flat_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      727 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_geo.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      969 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_geo_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1141 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_gsag.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1101 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_gsag_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      948 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_hv.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1033 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_hv_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1642 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_lamp.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1898 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_lamp_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      885 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_pha.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1125 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_pha_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1791 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_phot.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2039 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_phot_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1341 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_profile.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1481 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_profile_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1170 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_spot.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      938 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_spot_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1637 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_spwcs.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1880 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_spwcs_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1090 2020-09-02 13:20:12.000000 crds-7.6.0/crds/hst/tpns/cos_tds.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1351 2020-09-02 13:20:12.000000 crds-7.6.0/crds/hst/tpns/cos_tds_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1337 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_trace.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1473 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_trace_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      868 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_walk.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1146 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_walk_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      987 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_wcp.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1247 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_wcp_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      421 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_xwalk.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      690 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_xwalk_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      421 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_ywalk.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      690 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/cos_ywalk_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1155 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/foc_bac.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1047 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/foc_bac_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1536 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/foc_blm.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1244 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/foc_blm_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      762 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/foc_cuni.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1085 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/foc_cuni_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1536 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/foc_geo.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1424 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/foc_geo_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1436 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/foc_itf.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1235 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/foc_itf_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1006 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/foc_lsf.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1018 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/foc_lsf_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1371 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/foc_sde.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1080 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/foc_sde_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1462 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/foc_uni.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1125 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/foc_uni_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1700 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ais.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1188 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ais_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1200 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_bac.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1041 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_bac_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      921 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccg2.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      995 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccg2_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      723 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccs0.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1137 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccs0_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      652 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccs1.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1076 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccs1_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      752 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccs2.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1154 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccs2_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      654 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccs3.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1002 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccs3_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1101 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccs4.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1114 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccs4_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      821 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccs5.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1203 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccs5_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1261 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccs6.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1291 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccs6_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      564 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccs7.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1002 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccs7_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      609 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccs8.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1002 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccs8_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      652 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccs9.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1076 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccs9_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      509 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccsa.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      957 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccsa_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1036 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccsb.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1158 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccsb_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      705 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccsc.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1084 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccsc_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      697 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccsd.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1076 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccsd_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      748 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccse.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      952 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccse_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1239 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccsf.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      952 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ccsf_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1001 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ddt.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1001 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ddt_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1595 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_flt.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1328 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_flt_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1556 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ivs.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1346 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ivs_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1073 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_lsf.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      788 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_lsf_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1280 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_pcp.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1197 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_pcp_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1198 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_psf.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1037 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_psf_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1540 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_qin.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1406 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_qin_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1435 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ret.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1150 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/fos_ret_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1088 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_abs.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1032 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_abs_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      692 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccr1.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1027 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccr1_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      872 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccr2.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      995 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccr2_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1547 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccr3.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      995 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccr3_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      595 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccr4.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1033 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccr4_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      775 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccr5.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1033 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccr5_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1900 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccr6.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1033 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccr6_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      910 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccr7.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1033 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccr7_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      741 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccr8.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1114 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccr8_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      685 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccr9.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1068 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccr9_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      730 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccra.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1033 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccra_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      782 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccrb.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1110 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccrb_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2350 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccrc.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1033 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccrc_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      737 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccrd.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      995 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccrd_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      590 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccre.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      957 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_ccre_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1048 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_dio.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      994 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_dio_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1141 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_net.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1032 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_net_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1255 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_phc.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1032 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_phc_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1041 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_qin.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      994 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_qin_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1008 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_saa.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      956 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_saa_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      422 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_scoffc.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      957 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_scoffc_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1345 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_vig.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1032 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hrs_vig_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      490 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hsp_ccp0.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      993 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hsp_ccp0_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1310 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hsp_ccp1.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1059 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hsp_ccp1_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1228 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hsp_ccp2.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1026 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hsp_ccp2_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1228 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hsp_ccp3.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1024 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hsp_ccp3_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1269 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hsp_ccp4.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1028 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hsp_ccp4_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1310 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hsp_ccp5.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1060 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hsp_ccp5_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      490 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hsp_ccp6.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1024 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hsp_ccp6_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1228 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hsp_ccp7.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1026 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hsp_ccp7_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      613 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hsp_ccp8.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1061 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hsp_ccp8_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      490 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hsp_ccp9.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1028 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/hsp_ccp9_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1357 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_bkg.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1675 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_bkg_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1111 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_drk.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1443 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_drk_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1333 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_flt.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1675 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_flt_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      715 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_idc.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1057 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_idc_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1359 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_ilm.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1675 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_ilm_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      662 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_lin.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1004 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_lin_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      662 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_msk.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1004 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_msk_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      715 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_nlc.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1057 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_nlc_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      756 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_noi.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1096 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_noi_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      745 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_pht.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      956 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_pht_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      845 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_pmd.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1057 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_pmd_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      715 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_pmk.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1057 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_pmk_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      614 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_psb.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      956 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_psb_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      614 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_scn.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      956 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_scn_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      715 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_sdk.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1057 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_sdk_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      913 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_tdd.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1004 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_tdd_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1415 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_tdf.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1675 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_tdf_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      656 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_zpr.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      998 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/nic_zpr_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1733 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_1dt.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2127 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_1dt_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2807 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_1dx.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3183 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_1dx_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      774 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_a2d.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1109 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_a2d_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      970 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_any_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1738 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_apd.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2069 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_apd_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1743 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_apt.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2069 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_apt_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      765 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_bia.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1033 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_bia_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      680 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_bpx.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      988 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_bpx_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      923 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_ccd.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1226 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_ccd_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      761 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_cds.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1011 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_cds_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      753 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_crr.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1009 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_crr_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      686 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_dfl.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      988 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_dfl_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      794 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_drk.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1100 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_drk_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1862 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_dsp.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2251 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_dsp_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      761 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_ech.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1011 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_ech_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      770 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_exs.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1011 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_exs_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2825 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_gac.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3181 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_gac_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      748 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_hal.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1011 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_hal_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1861 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_iac.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2292 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_iac_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1118 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_idc.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1206 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_idc_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1622 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_imp.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1013 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_imp_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3230 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_lfl.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3353 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_lfl_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      681 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_lin.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      984 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_lin_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      630 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_lmp.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      922 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_lmp_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1705 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_moc.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2099 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_moc_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3235 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_pct.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3530 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_pct_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3256 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_pfl.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3550 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_pfl_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1932 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_pht.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2367 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_pht_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1049 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_rip.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1311 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_rip_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1873 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_sdc.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2127 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_sdc_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1067 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_srw.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1311 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_srw_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      679 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_ssc.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      970 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_ssc_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      704 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_ssd.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      988 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_ssd_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      668 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_tdc.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1023 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_tdc_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1099 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_tds.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1435 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_tds_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      680 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_tel.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      943 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_tel_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      905 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_wcp.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1160 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/stis_wcp_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      695 2020-09-02 13:20:12.000000 crds-7.6.0/crds/hst/tpns/synphot_obs.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      695 2020-09-02 13:20:12.000000 crds-7.6.0/crds/hst/tpns/synphot_obs_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1111 2020-09-02 13:20:12.000000 crds-7.6.0/crds/hst/tpns/synphot_syn.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1111 2020-09-02 13:20:12.000000 crds-7.6.0/crds/hst/tpns/synphot_syn_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1105 2020-09-02 13:20:12.000000 crds-7.6.0/crds/hst/tpns/synphot_th.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1105 2020-09-02 13:20:12.000000 crds-7.6.0/crds/hst/tpns/synphot_th_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1055 2020-09-02 13:20:12.000000 crds-7.6.0/crds/hst/tpns/synphot_tmc.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1055 2020-09-02 13:20:12.000000 crds-7.6.0/crds/hst/tpns/synphot_tmc_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1587 2020-09-02 13:20:12.000000 crds-7.6.0/crds/hst/tpns/synphot_tmg.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1587 2020-09-02 13:20:12.000000 crds-7.6.0/crds/hst/tpns/synphot_tmg_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1189 2020-09-02 13:20:12.000000 crds-7.6.0/crds/hst/tpns/synphot_tmt.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1189 2020-09-02 13:20:12.000000 crds-7.6.0/crds/hst/tpns/synphot_tmt_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      602 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_a2d.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      802 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_a2d_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1612 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_bia.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1962 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_bia_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1213 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_bic.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1441 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_bic_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      640 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_bpx.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      852 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_bpx_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      814 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_ccd.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1017 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_ccd_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      497 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_crr.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      715 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_crr_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2466 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_cte.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      839 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_cte_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      733 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_d2i.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      997 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_d2i_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      540 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_dfl.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      753 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_dfl_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1404 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_dkc.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1525 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_dkc_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      726 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_drk.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      944 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_drk_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      700 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_fls.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      952 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_fls_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      663 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_idc.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      855 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_idc_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1282 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_imp.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      999 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_imp_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      562 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_lfl.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      765 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_lfl_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      680 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_lin.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1004 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_lin_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      485 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_mdz.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      685 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_mdz_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      809 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_npl.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1050 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_npl_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      572 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_osc.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      840 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_osc_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      565 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_pfl.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      765 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_pfl_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      474 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_shd.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      682 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_shd_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      592 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_snk.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      839 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfc3_snk_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1861 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfp_a2d.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1152 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfp_a2d_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1247 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfp_bas.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1152 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfp_bas_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1391 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfp_dfl.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1230 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfp_dfl_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1425 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfp_dqf.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1230 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfp_dqf_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2061 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfp_drk.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1230 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfp_drk_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1391 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfp_flt.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1230 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfp_flt_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1394 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfp_msk.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1230 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfp_msk_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      825 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfp_phot.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1175 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfp_phot_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1391 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfp_prf.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1230 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfp_prf_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2126 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfp_psf.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1217 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfp_psf_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1392 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfp_spg.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1230 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wfp_spg_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1271 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_a2d.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1090 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_a2d_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1229 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_bas.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1049 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_bas_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1297 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_dqf.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1163 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_dqf_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1280 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_drk.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1090 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_drk_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      511 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_dxy.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      743 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_dxy_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1409 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_flt.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1077 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_flt_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      781 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_idc.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      958 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_idc_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1223 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_msk.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1040 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_msk_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      676 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_off.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      958 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_off_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      922 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_phot.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1035 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_phot_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2241 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_psf.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1268 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_shd.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1078 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_shd_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      973 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_w4t.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1018 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/tpns/wp2_w4t_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     8420 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/wfc3.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    12771 2020-09-02 13:20:07.000000 crds-7.6.0/crds/hst/wfpc2.py
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:42.575449 crds-7.6.0/crds/io/
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:20:07.000000 crds-7.6.0/crds/io/__init__.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    13890 2020-09-02 13:20:12.000000 crds-7.6.0/crds/io/abstract.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2054 2020-09-02 13:20:12.000000 crds-7.6.0/crds/io/asdf.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     4891 2020-09-02 13:20:07.000000 crds-7.6.0/crds/io/factory.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    10076 2020-09-02 13:20:12.000000 crds-7.6.0/crds/io/fits.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     6350 2020-09-02 13:20:07.000000 crds-7.6.0/crds/io/geis.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      815 2020-09-02 13:20:07.000000 crds-7.6.0/crds/io/json.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3408 2020-09-02 13:20:07.000000 crds-7.6.0/crds/io/tables.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      841 2020-09-02 13:20:07.000000 crds-7.6.0/crds/io/yaml.py
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:42.598427 crds-7.6.0/crds/jwst/
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      975 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/__init__.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/__main__.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/fgs.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     9007 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/gen_system_crdscfg.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    27238 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/jwst_system_crdscfg_b7.1.1.yaml
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    28294 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/jwst_system_crdscfg_b7.1.3.yaml
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    27329 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/jwst_system_crdscfg_b7.1.yaml
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    29137 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/jwst_system_crdscfg_b7.2.yaml
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    35563 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/jwst_system_crdscfg_b7.3.yaml
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    36866 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/jwst_system_crdscfg_b7.4.yaml
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    35961 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/jwst_system_crdscfg_b7.5.yaml
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    36205 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/jwst_system_crdscfg_b7.6.yaml
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    33748 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/jwst_system_crdscfg_b7.yaml
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    24052 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/locate.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/miri.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/nircam.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/niriss.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/nirspec.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    17241 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/pipeline.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     9356 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/schema.py
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:42.711682 crds-7.6.0/crds/jwst/specs/
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      198 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/all_all.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      258 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/all_dark.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      231 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/all_gain.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      244 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/all_ipc.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      268 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/all_photom.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      316 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/all_rscd.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      300 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/all_throughput.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      280 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/all_trappars.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)   145939 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/specs/combined_specs.json
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1161 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/specs/fgs_abvegaoffset.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      220 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/fgs_all.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      506 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/fgs_amplifier.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3888 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/specs/fgs_apcorr.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      449 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/fgs_area.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      459 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/fgs_dark.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      610 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/fgs_distortion.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      434 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/fgs_drizpars.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      453 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/fgs_flat.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      462 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/fgs_gain.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      472 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/fgs_ipc.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      498 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/fgs_linearity.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      472 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/fgs_mask.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      469 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/fgs_persat.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      473 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/fgs_photom.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      488 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/fgs_readnoise.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      325 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/fgs_regions.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      471 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/fgs_saturation.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      355 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/fgs_specwcs.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      506 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/fgs_superbias.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      490 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/fgs_trapdensity.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      478 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/fgs_trappars.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      361 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/fgs_wcsregions.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1163 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/specs/miri_abvegaoffset.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      211 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_all.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      508 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_amplifier.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3938 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/specs/miri_apcorr.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      480 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_area.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      603 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/specs/miri_cubepar.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      492 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_dark.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      640 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_distortion.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      436 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_drizpars.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      559 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_extract1d.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      661 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_filteroffset.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      531 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_flat.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      508 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_fringe.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      464 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_gain.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      474 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_ipc.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      491 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_lastframe.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      501 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_linearity.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      448 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_mask.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      552 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_pathloss.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      522 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_persat.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      535 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_photom.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      662 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_psfmask.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      490 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_readnoise.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      677 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_regions.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      655 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_reset.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      580 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_resol.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      615 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_rscd.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      474 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_saturation.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      846 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_specwcs.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      473 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_straymask.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      543 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_trapdensity.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      531 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_trappars.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      693 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_tsophot.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      757 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_v2v3.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      598 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_wavelengthrange.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      737 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/miri_wcsregions.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1167 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/specs/nircam_abvegaoffset.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      219 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_all.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      512 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_amplifier.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3906 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/specs/nircam_apcorr.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      509 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_area.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      496 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_dark.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      704 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_distortion.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      440 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_drizpars.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      708 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/specs/nircam_filteroffset.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      495 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_flat.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      468 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_gain.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      478 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_ipc.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      507 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_linearity.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      478 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_mask.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      475 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_persat.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      561 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_photom.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      670 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_psfmask.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      494 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_readnoise.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      331 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_regions.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      480 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_saturation.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      802 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_specwcs.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      361 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_specwcs.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      512 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_superbias.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      496 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_trapdensity.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      484 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_trappars.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      703 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_tsophot.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      609 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_wavelengthrange.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      367 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_wcsregions.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      701 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nircam_wfssbkg.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1167 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/specs/niriss_abvegaoffset.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      219 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_all.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      512 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_amplifier.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3906 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/specs/niriss_apcorr.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      509 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_area.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      472 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_dark.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      554 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_distortion.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      440 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_drizpars.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      563 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_extract1d.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      465 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_flat.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      468 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_gain.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      478 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_ipc.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      507 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_linearity.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      454 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_mask.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      574 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/specs/niriss_pars-image2pipeline.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      587 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_pathloss.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      475 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_persat.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      539 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_photom.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      494 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_readnoise.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      331 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_regions.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      480 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_saturation.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1085 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_specwcs.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      512 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_superbias.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      513 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_throughput.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      496 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_trapdensity.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      484 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_trappars.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      609 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_wavelengthrange.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      367 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_wcsregions.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      700 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/niriss_wfssbkg.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      223 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_all.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      514 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_amplifier.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3904 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/specs/nirspec_apcorr.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      572 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_area.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      551 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_badshutter.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      741 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_barshadow.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      559 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_camera.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      573 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_collimator.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      762 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_cubepar.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      498 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_dark.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      562 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_dflat.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      641 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_disperser.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      529 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_distortion.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      442 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_drizpars.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      565 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_extract1d.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      587 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_fflat.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      517 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_flat.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      642 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_fore.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      569 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_fpa.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      470 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_gain.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      538 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_ifufore.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      538 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_ifupost.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      548 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_ifuslicer.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      480 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_ipc.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      510 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_linearity.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      480 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_mask.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      571 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_msa.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      663 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_msaoper.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      582 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_ote.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      629 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/specs/nirspec_pars-spec2pipeline.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      558 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_pathloss.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      477 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_persat.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      513 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_photom.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      496 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_readnoise.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      613 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_refpix.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      872 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_regions.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      483 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_saturation.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      644 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_sflat.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      679 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_specwcs.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      514 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_superbias.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      498 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_trapdensity.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      486 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_trappars.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      568 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_wavecorr.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      606 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_wavelengthrange.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      369 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/nirspec_wcsregions.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      561 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/system_calver.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      612 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/system_crdscfg.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      638 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/specs/system_datalvl.rmap
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        3 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/substitutions.dat
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       52 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/system.py
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:42.768955 crds-7.6.0/crds/jwst/tpns/
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2754 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/all_all.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2754 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/all_all_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      715 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/all_dark.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      715 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/all_dark_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       37 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/all_gain.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      459 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/all_ipc.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       67 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/all_photom.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      348 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/all_throughput.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      749 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/all_trappars.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1840 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/fgs_all.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1840 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/fgs_all_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      552 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/tpns/fgs_apcorr.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      276 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/fgs_area.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      521 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/fgs_dark.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       37 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/fgs_distortion.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      185 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/fgs_flat.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      120 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/fgs_gain.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       35 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/fgs_linearity.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       30 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/fgs_mask.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       76 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/fgs_persat.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/fgs_photom.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      150 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/fgs_readnoise.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      282 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/fgs_saturation.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      186 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/fgs_superbias.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       76 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/fgs_trapdensity.tpn
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:42.781704 crds-7.6.0/crds/jwst/tpns/includes/
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1104 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/tpns/includes/apcorr.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      971 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/miri_dq_array.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      824 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/miri_dq_def_array.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      482 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/miri_err_array.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      796 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/miri_sci_array_both.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       81 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/miri_sci_array_norefpix.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       81 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/miri_sci_array_refpix.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1592 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/miri_subarray_both.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       56 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/miri_subarray_norefpix.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      134 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/miri_subarray_refpix.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      412 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/nir_dq_array.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      827 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/nir_dq_def_array.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      455 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/nir_err_array.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      372 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/nir_linearity.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      261 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/nir_mask.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      582 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/nir_opt_err_array.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      626 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/nir_photom.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1707 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/nir_sci_array_both.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      239 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/nir_sci_array_norefpix.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      235 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/nir_sci_array_refpix.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3236 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/nir_subarray.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      755 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/nir_subarray_baseline.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      934 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/nirspec_dq_array.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      529 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/nirspec_err_array.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      562 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/nirspec_opt_err_array.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1922 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/nirspec_sci_array_both.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       91 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/nirspec_sci_array_norefpix.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       91 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/nirspec_sci_array_refpix.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1540 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/includes/nirspec_sci_array_striped.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      747 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/tpns/includes/nirspec_subarray_baseline.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1830 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/tpns/miri_all.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1830 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/tpns/miri_all_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      354 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/miri_area.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      243 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/miri_cubepar.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      312 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/miri_dark.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       45 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/miri_distortion.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      197 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/miri_flat.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      324 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/miri_fringe.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      129 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/miri_gain.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      154 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/miri_lastframe.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1192 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/miri_linearity.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      262 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/miri_mask.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/miri_photom.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      153 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/miri_psfmask.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      159 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/miri_readnoise.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      364 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/miri_reset.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3264 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/tpns/miri_rscd.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      292 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/miri_saturation.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       44 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/miri_specwcs.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      308 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/miri_straymask.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      457 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/miri_tsophot.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3046 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nircam_all.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3046 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nircam_all_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      707 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/tpns/nircam_apcorr.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      276 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nircam_area.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      298 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nircam_dark.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       37 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nircam_distortion.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      187 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nircam_flat.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      120 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nircam_gain.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       36 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nircam_linearity.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       31 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nircam_mask.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       76 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nircam_persat.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nircam_photom.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      233 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nircam_psfmask.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      150 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nircam_readnoise.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      283 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nircam_saturation.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      186 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nircam_superbias.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       76 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nircam_trapdensity.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      459 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nircam_tsophot.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      384 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nircam_wfssbkg.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1243 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/niriss_all.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1243 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/niriss_all_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      535 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/tpns/niriss_apcorr.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      276 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/niriss_area.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      298 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/niriss_dark.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       37 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/niriss_distortion.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      185 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/niriss_flat.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      120 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/niriss_gain.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       36 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/niriss_linearity.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       31 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/niriss_mask.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      234 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/niriss_pathloss.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       76 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/niriss_persat.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        1 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/niriss_photom.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      150 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/niriss_readnoise.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      283 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/niriss_saturation.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       34 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/niriss_specwcs.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      186 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/niriss_superbias.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       76 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/niriss_trapdensity.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      384 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/niriss_wfssbkg.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1714 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nirspec_all.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1714 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nirspec_all_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1196 2020-09-02 13:20:12.000000 crds-7.6.0/crds/jwst/tpns/nirspec_apcorr.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1770 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nirspec_area.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1235 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nirspec_barshadow.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      229 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nirspec_cubepar.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      456 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nirspec_dark.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1364 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nirspec_dflat.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)       37 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nirspec_distortion.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3246 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nirspec_fflat.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      226 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nirspec_gain.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      455 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nirspec_linearity.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      285 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nirspec_mask.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      637 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nirspec_pathloss.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      105 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nirspec_persat.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nirspec_photom.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      255 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nirspec_readnoise.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      795 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nirspec_refpix.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      442 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nirspec_saturation.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1718 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nirspec_sflat.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      301 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nirspec_superbias.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      107 2020-09-02 13:20:07.000000 crds-7.6.0/crds/jwst/tpns/nirspec_trapdensity.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    32752 2020-09-02 13:20:12.000000 crds-7.6.0/crds/list.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    16584 2020-09-02 13:20:07.000000 crds-7.6.0/crds/matches.py
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:42.784783 crds-7.6.0/crds/misc/
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:20:07.000000 crds-7.6.0/crds/misc/__init__.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1827 2020-09-02 13:20:07.000000 crds-7.6.0/crds/misc/cal_pipelines.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     7449 2020-09-02 13:20:07.000000 crds-7.6.0/crds/misc/check_archive.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2789 2020-09-02 13:20:07.000000 crds-7.6.0/crds/misc/datalvl.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    11248 2020-09-02 13:20:12.000000 crds-7.6.0/crds/misc/get_synphot.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    26044 2020-09-02 13:20:12.000000 crds-7.6.0/crds/misc/query_affected.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     6349 2020-09-02 13:20:07.000000 crds-7.6.0/crds/misc/sql.py
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:42.786812 crds-7.6.0/crds/misc/synphot/
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      258 2020-09-02 13:20:12.000000 crds-7.6.0/crds/misc/synphot/__init__.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    13746 2020-09-02 13:20:12.000000 crds-7.6.0/crds/misc/synphot/integration_tests.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     6382 2020-09-02 13:20:12.000000 crds-7.6.0/crds/misc/synphot/lookup_generator.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     8744 2020-09-02 13:20:12.000000 crds-7.6.0/crds/misc/synphot/utils.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     8902 2020-09-02 13:20:07.000000 crds-7.6.0/crds/misc/uniqname.py
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:42.788985 crds-7.6.0/crds/refactoring/
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:20:07.000000 crds-7.6.0/crds/refactoring/__init__.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     5012 2020-09-02 13:20:07.000000 crds-7.6.0/crds/refactoring/checksum.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     7815 2020-09-02 13:20:07.000000 crds-7.6.0/crds/refactoring/newcontext.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    10334 2020-09-02 13:20:07.000000 crds-7.6.0/crds/refactoring/refactor.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    33947 2020-09-02 13:20:07.000000 crds-7.6.0/crds/refactoring/refactor2.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    32384 2020-09-02 13:20:07.000000 crds-7.6.0/crds/rowdiff.py
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:42.793371 crds-7.6.0/crds/submit/
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      176 2020-09-02 13:20:07.000000 crds-7.6.0/crds/submit/__init__.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      205 2020-09-02 13:20:07.000000 crds-7.6.0/crds/submit/__main__.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3026 2020-09-02 13:20:07.000000 crds-7.6.0/crds/submit/background.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     5774 2020-09-02 13:20:07.000000 crds-7.6.0/crds/submit/monitor.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    14408 2020-09-02 13:20:07.000000 crds-7.6.0/crds/submit/rc_submit.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    16924 2020-09-02 13:20:07.000000 crds-7.6.0/crds/submit/submit.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     8877 2020-09-02 13:20:07.000000 crds-7.6.0/crds/submit/web.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    36425 2020-09-02 13:20:07.000000 crds-7.6.0/crds/sync.py
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:42.818099 crds-7.6.0/crds/tests/
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      237 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/__init__.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      514 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/compare_pickles.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1440 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/profile_bestrefs.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      892 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/profile_pickling.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     8336 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/test_bad_files.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    26773 2020-09-02 13:20:12.000000 crds-7.6.0/crds/tests/test_bestrefs.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3435 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/test_build6.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)   128512 2020-09-02 13:20:12.000000 crds-7.6.0/crds/tests/test_certify.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2051 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/test_check_archive.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     9101 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/test_checksum.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    10602 2020-09-02 13:20:12.000000 crds-7.6.0/crds/tests/test_cmdline.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     4125 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/test_config.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    41724 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/test_diff.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    11689 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/test_heavy_client.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    13957 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/test_io.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    27576 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/test_list.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     4743 2020-09-02 13:20:12.000000 crds-7.6.0/crds/tests/test_locking.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3845 2020-09-02 13:20:12.000000 crds-7.6.0/crds/tests/test_matches.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3579 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/test_newcontext.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     6585 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/test_or_bars.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     7557 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/test_refactor.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    16189 2020-09-02 13:20:12.000000 crds-7.6.0/crds/tests/test_reftypes.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    33929 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/test_rmap.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    10768 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/test_rowdiff.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    50865 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/test_special.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     9724 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/test_submit.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    12230 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/test_substitutions.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     4751 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/test_sync.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    37869 2020-09-02 13:20:12.000000 crds-7.6.0/crds/tests/test_synphot_hst.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1527 2020-09-02 13:20:12.000000 crds-7.6.0/crds/tests/test_synphot_lookup_generator.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     5289 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/test_table_effects.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     5431 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/test_uniqname.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2956 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tests/test_uses.py
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:42.820399 crds-7.6.0/crds/tobs/
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      733 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tobs/__init__.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tobs/__main__.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    11292 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tobs/locate.py
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:42.821105 crds-7.6.0/crds/tobs/specs/
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      749 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tobs/specs/combined_specs.json
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      437 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tobs/specs/tinstr_tfilekind.spec
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        3 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tobs/substitutions.dat
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    23945 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tobs/tests.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      123 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tobs/tinstr.py
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:42.821895 crds-7.6.0/crds/tobs/tpns/
+-rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)      531 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tobs/tpns/tinstr_tfk.tpn
+-rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)      531 2020-09-02 13:20:07.000000 crds-7.6.0/crds/tobs/tpns/tinstr_tfk_ld.tpn
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     6352 2020-09-02 13:20:07.000000 crds-7.6.0/crds/uses.py
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:41.807273 crds-7.6.0/crds.egg-info/
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     7700 2020-09-02 13:39:41.000000 crds-7.6.0/crds.egg-info/PKG-INFO
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)    33529 2020-09-02 13:39:41.000000 crds-7.6.0/crds.egg-info/SOURCES.txt
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        1 2020-09-02 13:39:41.000000 crds-7.6.0/crds.egg-info/dependency_links.txt
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        1 2020-09-02 13:22:22.000000 crds-7.6.0/crds.egg-info/not-zip-safe
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      290 2020-09-02 13:39:41.000000 crds-7.6.0/crds.egg-info/requires.txt
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)        5 2020-09-02 13:39:41.000000 crds-7.6.0/crds.egg-info/top_level.txt
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:42.866170 crds-7.6.0/envs/
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      336 2020-09-02 13:20:07.000000 crds-7.6.0/envs/crds-readonly.csh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      404 2020-09-02 13:20:07.000000 crds-7.6.0/envs/crds-tests.csh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      414 2020-09-02 13:20:07.000000 crds-7.6.0/envs/crds-tests.sh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2408 2020-09-02 13:20:07.000000 crds-7.6.0/envs/env-forwarded.csh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2373 2020-09-02 13:20:07.000000 crds-7.6.0/envs/env-local.csh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2457 2020-09-02 13:20:07.000000 crds-7.6.0/envs/hst-crds-dev.csh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2456 2020-09-02 13:20:07.000000 crds-7.6.0/envs/hst-crds-dev.sh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2388 2020-09-02 13:20:07.000000 crds-7.6.0/envs/hst-crds-ops.csh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2387 2020-09-02 13:20:07.000000 crds-7.6.0/envs/hst-crds-ops.sh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2379 2020-09-02 13:20:07.000000 crds-7.6.0/envs/hst-crds-readonly.csh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2378 2020-09-02 13:20:07.000000 crds-7.6.0/envs/hst-crds-readonly.sh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2394 2020-09-02 13:20:07.000000 crds-7.6.0/envs/hst-crds-test.csh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2393 2020-09-02 13:20:07.000000 crds-7.6.0/envs/hst-crds-test.sh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      124 2020-09-02 13:20:07.000000 crds-7.6.0/envs/hst-serverless.csh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2412 2020-09-02 13:20:07.000000 crds-7.6.0/envs/jwst-crds-b5it.csh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2412 2020-09-02 13:20:07.000000 crds-7.6.0/envs/jwst-crds-b6it.csh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2410 2020-09-02 13:20:07.000000 crds-7.6.0/envs/jwst-crds-bit.csh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2407 2020-09-02 13:20:07.000000 crds-7.6.0/envs/jwst-crds-bit.sh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2410 2020-09-02 13:20:07.000000 crds-7.6.0/envs/jwst-crds-cit.csh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2407 2020-09-02 13:20:07.000000 crds-7.6.0/envs/jwst-crds-cit.sh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2410 2020-09-02 13:20:07.000000 crds-7.6.0/envs/jwst-crds-dev.csh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2409 2020-09-02 13:20:07.000000 crds-7.6.0/envs/jwst-crds-dev.sh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2410 2020-09-02 13:20:07.000000 crds-7.6.0/envs/jwst-crds-dit.csh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2409 2020-09-02 13:20:07.000000 crds-7.6.0/envs/jwst-crds-dit.sh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2389 2020-09-02 13:20:07.000000 crds-7.6.0/envs/jwst-crds-ops.csh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2388 2020-09-02 13:20:07.000000 crds-7.6.0/envs/jwst-crds-ops.sh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2390 2020-09-02 13:20:07.000000 crds-7.6.0/envs/jwst-crds-readonly.csh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2389 2020-09-02 13:20:07.000000 crds-7.6.0/envs/jwst-crds-readonly.sh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2395 2020-09-02 13:20:07.000000 crds-7.6.0/envs/jwst-crds-test.csh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     2398 2020-09-02 13:20:07.000000 crds-7.6.0/envs/jwst-crds-test.sh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      125 2020-09-02 13:20:07.000000 crds-7.6.0/envs/jwst-serverless.csh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      935 2020-09-02 13:20:07.000000 crds-7.6.0/envs/s3.sh
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      263 2020-09-02 13:20:07.000000 crds-7.6.0/envs/un-s3.sh
+-rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)     2292 2020-09-02 13:20:07.000000 crds-7.6.0/install
+drwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)        0 2020-09-02 13:39:42.873176 crds-7.6.0/scripts/
+-rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)     2748 2020-09-02 13:20:07.000000 crds-7.6.0/scripts/crds
+-rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)      281 2020-09-02 13:20:07.000000 crds-7.6.0/scripts/crds_cached_context
+-rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)     1299 2020-09-02 13:20:07.000000 crds-7.6.0/scripts/crds_check_cache
+-rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)     1676 2020-09-02 13:20:07.000000 crds-7.6.0/scripts/crds_dataset_capture
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1233 2020-09-02 13:20:07.000000 crds-7.6.0/scripts/crds_jwst_serverless_pipeline_env.csh
+-rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)     4199 2020-09-02 13:20:07.000000 crds-7.6.0/scripts/crds_repair_cache
+-rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)       71 2020-09-02 13:20:07.000000 crds-7.6.0/scripts/crds_s3_get
+-rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)      902 2020-09-02 13:20:07.000000 crds-7.6.0/scripts/crds_unique
+-rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)     5566 2020-09-02 13:20:07.000000 crds-7.6.0/scripts/cron_sync
+-rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)      846 2020-09-02 13:20:07.000000 crds-7.6.0/scripts/custom_query_affected_datasets
+-rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)     1348 2020-09-02 13:20:07.000000 crds-7.6.0/scripts/pipeline_bestref
+-rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)      197 2020-09-02 13:20:07.000000 crds-7.6.0/scripts/query_affected_datasets
+-rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)      530 2020-09-02 13:20:07.000000 crds-7.6.0/scripts/remote_cache_init
+-rwxrwxr-x   0 eisenham  (1009) STSCI\science  (1031)     1607 2020-09-02 13:20:07.000000 crds-7.6.0/scripts/safe_bestrefs
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)      362 2020-09-02 13:39:42.875115 crds-7.6.0/setup.cfg
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     3295 2020-09-02 13:24:37.000000 crds-7.6.0/setup.py
+-rw-rw-r--   0 eisenham  (1009) STSCI\science  (1031)     1224 2020-09-02 13:20:07.000000 crds-7.6.0/setup_data.py
```

### Comparing `crds-7.5.0.0/PKG-INFO` & `crds-7.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crds
-Version: 7.5.0.0
+Version: 7.6.0
 Summary: Calibration Reference Data System,  HST/JWST reference file management
 Home-page: https://hst-crds.stsci.edu
 Author: Todd Miller
 Author-email: jmiller@stsci.edu
 License: BSD
 Description: ====
         CRDS
@@ -177,7 +177,8 @@
 Provides: crds
 Provides-Extra: jwst
 Provides-Extra: submission
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: aws
+Provides-Extra: synphot
```

### Comparing `crds-7.5.0.0/README.rst` & `crds-7.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/TESTING` & `crds-7.6.0/TESTING`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/clean` & `crds-7.6.0/clean`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/__init__.py` & `crds-7.6.0/crds/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import warnings
 
 warnings.filterwarnings(
     "ignore", ".*found in sys.modules after import of package.*")
 
 # ============================================================================
 
-__version__ = "7.5.0.0"   # XXXX  see also ../setup.cfg
-__rationale__ = "JWST DMS 7.5, May2020 Release #1"
+__version__ = "7.6.0"   # XXXX  see also ../setup.cfg
+__rationale__ = "JWST DMS 7.6, Sep2020 Release #1"
 
 __all__ = [
     "getrecommendations",
     "getreferences",
     "assign_bestrefs",
     "get_pickled_mapping",
     "get_symbolic_mapping",
```

### Comparing `crds-7.5.0.0/crds/bestrefs/bestrefs.py` & `crds-7.6.0/crds/bestrefs/bestrefs.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/bestrefs/headers.py` & `crds-7.6.0/crds/bestrefs/headers.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/bestrefs/table_effects.py` & `crds-7.6.0/crds/bestrefs/table_effects.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/certify/certify.py` & `crds-7.6.0/crds/certify/certify.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
 
     def get_validators(self):
         """Given a reference file `filename`,  return the observatory specific
         list of Validators used to check that reference file type.
         """
         # Get the cache key for this filetype.
-        checkers = validators.get_validators(self.observatory, self.filename)
+        checkers = validators.get_validators(self.observatory, self.filename, context=self.context)
         checkers = self.set_rmap_parkeys_to_required(checkers)
         return checkers
 
     def set_rmap_parkeys_to_required(self, checkers):
         """Mutate copies of `checkers` so that any specified by the rmap parkey are required."""
         parkeys = set(self.get_rmap_parkeys())
         vlist = []
```

### Comparing `crds-7.5.0.0/crds/certify/check_sha1sum.py` & `crds-7.6.0/crds/certify/check_sha1sum.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/certify/generic_tpn.py` & `crds-7.6.0/crds/certify/generic_tpn.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/certify/mapping_parser.py` & `crds-7.6.0/crds/certify/mapping_parser.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/certify/reftypes.py` & `crds-7.6.0/crds/certify/reftypes.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/certify/validator_helpers.py` & `crds-7.6.0/crds/certify/validators/helpers.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/certify/validators.py` & `crds-7.6.0/crds/certify/validators/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-"""This module defines replacement functionality for the CDBS "certify" program
-used to check parameter values in .fits reference files.   It verifies that FITS
-files define required parameters and that they have legal values.
-"""
 import os
 import re
 import copy
 import abc
 
 # ============================================================================
 
@@ -15,17 +11,18 @@
 
 from crds.core import log, utils, timestamp, selectors, config
 from crds.core.exceptions import MissingKeywordError, IllegalKeywordError
 from crds.core.exceptions import TpnDefinitionError, RequiredConditionError
 from crds.core.exceptions import BadKernelSumError, BadKernelCenterPixelTooSmall
 from crds.io import tables
 from crds import data_file
+from crds.certify import generic_tpn
+from crds.certify.generic_tpn import TpnInfo # generic TpnInfo code
 
-from . import generic_tpn, validator_helpers
-from .generic_tpn import TpnInfo   # generic TpnInfo code
+from . import helpers as validator_helpers
 
 # ============================================================================
 
 def array_name(rootname):
     """Given the `rootname` for an array,  return the name of the array used
     in Validator expressions.
 
@@ -46,17 +43,18 @@
 
 # ============================================================================
 
 class Validator:
     """Validator is an Abstract class that applies TpnInfo objects to reference files.  Each
     Validator handles a single constraint defined in a .tpn file.
     """
-    def __init__(self, info):
+    def __init__(self, info, context=None):
         self.info = info
         self.name = info.name
+        self.context = context
         self._presence_condition_code = None
 
         if self.info.datatype not in generic_tpn.TpnInfo.datatypes:
             raise ValueError("Bad TPN datatype field " + repr(self.info.presence))
 
         if not (self.info.presence in generic_tpn.TpnInfo.presences or
                 self.conditionally_required):
@@ -639,14 +637,45 @@
     # Next reject strings with quotes in them,  or lower case or mixed case
     no_quotes = [key for key in candidates if re.match(r"^[A-Z0-9_\.]+$", key)]
     no_dots = [key.split(".")[0] for key in no_quotes]
     no_numbers = [key for key in no_dots if not re.match(r"\d+", key)]
     no_underscores = [key for key in no_numbers if key != "_"]
     return no_underscores
 
+# ----------------------------------------------------------------------------
+
+class ColumnExpressionValidator(Validator):
+    """Value is an expression on the column value that must evaluate to True."""
+
+    def __init__(self, info, *args, **keys):
+        super(ColumnExpressionValidator, self).__init__(info, *args, **keys)
+        self._expr = info.values[0]
+        self._expr_code = compile(self._expr, repr(self.info), "eval")
+
+    def check_value(self, filename, value):
+        if value in [None, "UNDEFINED"]: # missing optional or excluded keyword
+            return True
+        value = self.condition(value)
+
+        try:
+            satisfied = eval(self._expr_code, {"VALUE": value}, self._eval_namespace)
+        except Exception as exc:
+            raise RequiredConditionError("Failed checking constraint", repr(self._expr), ":", str(exc))
+
+        if not satisfied:
+            raise RequiredConditionError("Constraint", str(self._expr), "is not satisfied.")
+        elif satisfied == "W":  # from warn_only() helper
+            log.warning("Constraint", str(self._expr), "is not satisfied.")
+            satisfied = True
+
+        return satisfied
+
+    def check_header(self, filename, header):
+        return True
+
 # ---------------------------------------------------------------------------
 
 class KernelunityValidator(Validator):
     """Ensure that every image in the specified array as a sum() near 1.0"""
     def _check_value(self, *args, **keys):
         return True
 
@@ -756,57 +785,7 @@
         crds_name = value
         if "$" in value: # remove IRAF-style path prefix from SYNPHOT TMC and TMT filename column values
             crds_name = crds_name.split("$")[-1]
         if "[" in value: # split off HDU index trailer,  or SYNPHOT parameterization trailer
             crds_name = crds_name.split("[")[0]
         log.verbose("Conditioned filepath", repr(value), "to", repr(crds_name))
         return crds_name
-
-
-# ----------------------------------------------------------------------------
-
-def validator(info):
-    """Given TpnInfo object `info`, construct and return a Validator for it."""
-    if len(info.values) == 1 and len(info.values[0]) and \
-        info.values[0][0] == "&":
-        # This block handles &-types like &PEDIGREE and &SYBDATE
-        # only called on static TPN infos.
-        class_name = info.values[0][1:].capitalize() + "Validator"
-        rval = eval(class_name)(info)
-    elif info.datatype == "C":
-        rval = CharacterValidator(info)
-    elif info.datatype == "R":
-        rval = RealValidator(info)
-    elif info.datatype == "D":
-        rval = DoubleValidator(info)
-    elif info.datatype == "I":
-        rval = IntValidator(info)
-    elif info.datatype == "L":
-        rval = LogicalValidator(info)
-    elif info.datatype == "X":
-        rval = ExpressionValidator(info)
-    else:
-        raise ValueError("Unimplemented datatype " + repr(info.datatype))
-    return rval
-
-# ============================================================================
-
-def get_validators(observatory, refpath):
-    """Given `observatory` and a path to a reference file `refpath`,  load the
-    corresponding validators that define individual constraints that reference
-    should satisfy.
-    """
-    tpns = get_reffile_tpninfos(observatory, refpath)
-    checkers = [validator(x) for x in tpns]
-    log.verbose("Validators for", repr(refpath), "("+str(len(checkers))+"):\n", log.PP(checkers), verbosity=65)
-    return checkers
-
-def get_reffile_tpninfos(observatory, refpath):
-    """Load just the TpnInfo objects for `observatory` and the given `refpath`.
-    This entails both "class" TpnInfo's from CDBS as well as TpnInfo objects
-    derived from the JWST data models.
-    """
-    locator = utils.get_locator_module(observatory)
-    instrument, filekind = locator.get_file_properties(refpath)
-    tpns = list(locator.get_all_tpninfos(instrument, filekind, "tpn"))
-    tpns.extend(locator.get_extra_tpninfos(refpath))
-    return tpns
```

### Comparing `crds-7.5.0.0/crds/client/api.py` & `crds-7.6.0/crds/client/api.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/client/proxy.py` & `crds-7.6.0/crds/client/proxy.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/core/cmdline.py` & `crds-7.6.0/crds/core/cmdline.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/core/config.py` & `crds-7.6.0/crds/core/config.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/core/crds_cache_locking.py` & `crds-7.6.0/crds/core/crds_cache_locking.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/core/custom_dict.py` & `crds-7.6.0/crds/core/custom_dict.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/core/exceptions.py` & `crds-7.6.0/crds/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/core/heavy_client.py` & `crds-7.6.0/crds/core/heavy_client.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/core/log.py` & `crds-7.6.0/crds/core/log.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/core/mapping_verifier.py` & `crds-7.6.0/crds/core/mapping_verifier.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/core/naming.py` & `crds-7.6.0/crds/core/naming.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/core/pysh.py` & `crds-7.6.0/crds/core/pysh.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/core/rmap.py` & `crds-7.6.0/crds/core/rmap.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/core/selectors.py` & `crds-7.6.0/crds/core/selectors.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/core/substitutions.py` & `crds-7.6.0/crds/core/substitutions.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/core/timestamp.py` & `crds-7.6.0/crds/core/timestamp.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/core/utils.py` & `crds-7.6.0/crds/core/utils.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/data_file.py` & `crds-7.6.0/crds/data_file.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/diff.py` & `crds-7.6.0/crds/diff.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/__init__.py` & `crds-7.6.0/crds/hst/__init__.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/acs.py` & `crds-7.6.0/crds/hst/acs.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/acs_common.py` & `crds-7.6.0/crds/hst/acs_common.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/acs_v1.py` & `crds-7.6.0/crds/hst/acs_v1.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/acs_v2.py` & `crds-7.6.0/crds/hst/acs_v2.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/locate.py` & `crds-7.6.0/crds/hst/locate.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,15 +314,15 @@
                           "for", repr(ref))
             if filekind != filekind2:
                 log.error("Inconsistent filekinds", repr(filekind), "vs.", repr(filekind2),
                           "for", repr(ref))
 
             for pmap_name in reversed(sorted(rmap.list_mappings("*.pmap", observatory="hst"))):
 
-                r = certify.find_governing_rmap(pmap_name, ref)
+                r = certify.certify.find_governing_rmap(pmap_name, ref)
 
                 if not r:
                     continue
 
                 if r.instrument != instrument:
                     log.error("Rmap instrument", repr(r.instrument),
                               "inconsistent with name derived instrument", repr(instrument), "for", repr(ref), "in", repr(pmap_name))
```

### Comparing `crds-7.5.0.0/crds/hst/siname.py` & `crds-7.6.0/crds/hst/siname.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/acs_atodtab.spec` & `crds-7.6.0/crds/hst/specs/acs_atodtab.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/acs_biasfile.spec` & `crds-7.6.0/crds/hst/specs/acs_biasfile.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/acs_ccdtab.spec` & `crds-7.6.0/crds/hst/specs/acs_ccdtab.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/acs_crrejtab.spec` & `crds-7.6.0/crds/hst/specs/acs_crrejtab.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/acs_dfltfile.rmap` & `crds-7.6.0/crds/hst/specs/acs_dfltfile.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/acs_drkcfile.spec` & `crds-7.6.0/crds/hst/specs/acs_drkcfile.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/acs_flshfile.spec` & `crds-7.6.0/crds/hst/specs/acs_flshfile.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/acs_lfltfile.spec` & `crds-7.6.0/crds/hst/specs/acs_lfltfile.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/acs_pfltfile.spec` & `crds-7.6.0/crds/hst/specs/acs_pfltfile.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/acs_snkcfile.rmap` & `crds-7.6.0/crds/hst/specs/acs_snkcfile.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/combined_specs.json` & `crds-7.6.0/crds/hst/specs/combined_specs.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9880952380952381%*

 * *Differences: {"'synphot'": "{'obsmodes': OrderedDict([('classes', ['Match']), ('derived_from', 'Initial hand "*

 * *              "made version 2020-03-25.'), ('extra_keys', []), ('file_ext', '.fits'), ('filekind', "*

 * *              "'OBSMODES'), ('filetype', 'CROBSMODELIST'), ('instrument', 'SYNPHOT'), ('ld_tpn', "*

 * *              "'synphot_obs_ld.tpn'), ('mapping', 'REFERENCE'), ('name', 'synphot_obsmodes.rmap'), "*

 * *              "('observatory', 'HST'), ('parkey', [[]]), ('reffile_format', 'TABLE'), "*

 * *              "('reffile_ […]*

```diff
@@ -2148,14 +2148,43 @@
                 "OPT_ELEM",
                 "CENWAVE",
                 "SPORDER"
             ]
         }
     },
     "synphot": {
+        "obsmodes": {
+            "classes": [
+                "Match"
+            ],
+            "derived_from": "Initial hand made version 2020-03-25.",
+            "extra_keys": [],
+            "file_ext": ".fits",
+            "filekind": "OBSMODES",
+            "filetype": "CROBSMODELIST",
+            "instrument": "SYNPHOT",
+            "ld_tpn": "synphot_obs_ld.tpn",
+            "mapping": "REFERENCE",
+            "name": "synphot_obsmodes.rmap",
+            "observatory": "HST",
+            "parkey": [
+                []
+            ],
+            "reffile_format": "TABLE",
+            "reffile_required": "YES",
+            "reffile_switch": "NONE",
+            "rmap_omit": "True",
+            "sha1sum": "2ccb22fa1a9794eabf46e02ed05e0a6eee16fe78",
+            "suffix": "obs",
+            "text_descr": "Observing Modes Table",
+            "tpn": "synphot_obs.tpn",
+            "unique_rowkeys": [
+                "OBSMODE"
+            ]
+        },
         "thermal": {
             "classes": [
                 "Match"
             ],
             "comment_parkeys": [
                 "DATE",
                 "DESCRIP"
```

### Comparing `crds-7.5.0.0/crds/hst/specs/cos_brsttab.spec` & `crds-7.6.0/crds/hst/specs/cos_brsttab.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/cos_dgeofile.rmap` & `crds-7.6.0/crds/hst/specs/cos_dgeofile.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/cos_disptab.spec` & `crds-7.6.0/crds/hst/specs/cos_disptab.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/cos_fluxtab.spec` & `crds-7.6.0/crds/hst/specs/cos_fluxtab.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/cos_lamptab.spec` & `crds-7.6.0/crds/hst/specs/cos_lamptab.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/cos_proftab.spec` & `crds-7.6.0/crds/hst/specs/cos_proftab.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/cos_spottab.rmap` & `crds-7.6.0/crds/hst/specs/cos_spottab.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/cos_spwcstab.spec` & `crds-7.6.0/crds/hst/specs/cos_spwcstab.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/cos_tdstab.spec` & `crds-7.6.0/crds/hst/specs/cos_tdstab.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/cos_tracetab.spec` & `crds-7.6.0/crds/hst/specs/cos_tracetab.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/cos_twozxtab.spec` & `crds-7.6.0/crds/hst/specs/cos_twozxtab.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/cos_walktab.spec` & `crds-7.6.0/crds/hst/specs/cos_walktab.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/cos_xtractab.spec` & `crds-7.6.0/crds/hst/specs/cos_xtractab.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/cos_xwlkfile.rmap` & `crds-7.6.0/crds/hst/specs/cos_xwlkfile.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/cos_ywlkfile.rmap` & `crds-7.6.0/crds/hst/specs/cos_ywlkfile.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/stis_exstab.spec` & `crds-7.6.0/crds/hst/specs/stis_exstab.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/stis_gactab.spec` & `crds-7.6.0/crds/hst/specs/stis_gactab.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/stis_lfltfile.spec` & `crds-7.6.0/crds/hst/specs/stis_lfltfile.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/stis_mofftab.spec` & `crds-7.6.0/crds/hst/specs/stis_mofftab.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/stis_pctab.spec` & `crds-7.6.0/crds/hst/specs/stis_pctab.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/stis_pfltfile.spec` & `crds-7.6.0/crds/hst/specs/stis_pfltfile.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/stis_sdctab.spec` & `crds-7.6.0/crds/hst/specs/stis_sdctab.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/stis_srwtab.spec` & `crds-7.6.0/crds/hst/specs/stis_srwtab.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/synphot_thermal.rmap` & `crds-7.6.0/crds/hst/specs/synphot_thermal.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/synphot_thruput.rmap` & `crds-7.6.0/crds/hst/specs/synphot_thruput.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/synphot_tmctab.rmap` & `crds-7.6.0/crds/hst/specs/synphot_tmctab.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/synphot_tmgtab.rmap` & `crds-7.6.0/crds/hst/specs/synphot_tmgtab.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/synphot_tmttab.rmap` & `crds-7.6.0/crds/hst/specs/synphot_tmttab.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/wfc3_atodtab.spec` & `crds-7.6.0/crds/hst/specs/wfc3_atodtab.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/wfc3_biacfile.rmap` & `crds-7.6.0/crds/hst/specs/wfc3_biacfile.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/wfc3_biasfile.spec` & `crds-7.6.0/crds/hst/specs/wfc3_biasfile.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/wfc3_ccdtab.spec` & `crds-7.6.0/crds/hst/specs/wfc3_ccdtab.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/wfc3_crrejtab.spec` & `crds-7.6.0/crds/hst/specs/wfc3_crrejtab.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/wfc3_darkfile.spec` & `crds-7.6.0/crds/hst/specs/wfc3_darkfile.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/wfc3_dfltfile.spec` & `crds-7.6.0/crds/hst/specs/wfc3_dfltfile.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/wfc3_drkcfile.rmap` & `crds-7.6.0/crds/hst/specs/wfc3_drkcfile.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/wfc3_flshfile.spec` & `crds-7.6.0/crds/hst/specs/wfc3_flshfile.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/wfc3_pctetab.rmap` & `crds-7.6.0/crds/hst/specs/wfc3_pctetab.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/wfc3_pfltfile.spec` & `crds-7.6.0/crds/hst/specs/wfc3_pfltfile.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/specs/wfc3_snkcfile.rmap` & `crds-7.6.0/crds/hst/specs/wfc3_snkcfile.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/substitutions.dat` & `crds-7.6.0/crds/hst/substitutions.dat`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_a2d.tpn` & `crds-7.6.0/crds/hst/tpns/acs_a2d.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_a2d_ld.tpn` & `crds-7.6.0/crds/hst/tpns/acs_a2d_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_bia.tpn` & `crds-7.6.0/crds/hst/tpns/acs_bia.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_bia_ld.tpn` & `crds-7.6.0/crds/hst/tpns/acs_bia_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_bpx.tpn` & `crds-7.6.0/crds/hst/tpns/acs_bpx.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_bpx_ld.tpn` & `crds-7.6.0/crds/hst/tpns/acs_bpx_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_ccd.tpn` & `crds-7.6.0/crds/hst/tpns/acs_ccd.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_ccd_ld.tpn` & `crds-7.6.0/crds/hst/tpns/acs_ccd_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_cfl.tpn` & `crds-7.6.0/crds/hst/tpns/acs_cfl.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_cfl_ld.tpn` & `crds-7.6.0/crds/hst/tpns/acs_cfl_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_crr_ld.tpn` & `crds-7.6.0/crds/hst/tpns/acs_crr_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_csp.tpn` & `crds-7.6.0/crds/hst/tpns/acs_csp.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_csp_ld.tpn` & `crds-7.6.0/crds/hst/tpns/acs_csp_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_cte.tpn` & `crds-7.6.0/crds/hst/tpns/acs_cte.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_cte_ld.tpn` & `crds-7.6.0/crds/hst/tpns/acs_cte_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_d2i.tpn` & `crds-7.6.0/crds/hst/tpns/acs_d2i.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_d2i_ld.tpn` & `crds-7.6.0/crds/hst/tpns/acs_d2i_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_dfl.tpn` & `crds-7.6.0/crds/hst/tpns/acs_dfl.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_dfl_ld.tpn` & `crds-7.6.0/crds/hst/tpns/acs_dfl_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_dkc.tpn` & `crds-7.6.0/crds/hst/tpns/acs_dkc.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_dkc_ld.tpn` & `crds-7.6.0/crds/hst/tpns/acs_dkc_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_drk.tpn` & `crds-7.6.0/crds/hst/tpns/acs_drk.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_drk_ld.tpn` & `crds-7.6.0/crds/hst/tpns/acs_drk_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_dxy.tpn` & `crds-7.6.0/crds/hst/tpns/acs_dxy.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_dxy_ld.tpn` & `crds-7.6.0/crds/hst/tpns/acs_dxy_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_fls.tpn` & `crds-7.6.0/crds/hst/tpns/acs_fls.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_fls_ld.tpn` & `crds-7.6.0/crds/hst/tpns/acs_fls_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_idc.tpn` & `crds-7.6.0/crds/hst/tpns/acs_idc.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_idc_ld.tpn` & `crds-7.6.0/crds/hst/tpns/acs_idc_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_imp.tpn` & `crds-7.6.0/crds/hst/tpns/acs_imp.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_imp_ld.tpn` & `crds-7.6.0/crds/hst/tpns/acs_imp_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_lfl.tpn` & `crds-7.6.0/crds/hst/tpns/acs_lfl.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_lfl_ld.tpn` & `crds-7.6.0/crds/hst/tpns/acs_lfl_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_lin_ld.tpn` & `crds-7.6.0/crds/hst/tpns/acs_lin_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_mdz_ld.tpn` & `crds-7.6.0/crds/hst/tpns/acs_mdz_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_npl.tpn` & `crds-7.6.0/crds/hst/tpns/acs_npl.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_npl_ld.tpn` & `crds-7.6.0/crds/hst/tpns/acs_npl_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_osc_ld.tpn` & `crds-7.6.0/crds/hst/tpns/acs_osc_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_pfl.tpn` & `crds-7.6.0/crds/hst/tpns/acs_pfl.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_pfl_ld.tpn` & `crds-7.6.0/crds/hst/tpns/acs_pfl_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_shd_ld.tpn` & `crds-7.6.0/crds/hst/tpns/acs_shd_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_snk.tpn` & `crds-7.6.0/crds/hst/tpns/acs_snk.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/acs_snk_ld.tpn` & `crds-7.6.0/crds/hst/tpns/acs_snk_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_1dx.tpn` & `crds-7.6.0/crds/hst/tpns/cos_1dx.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_1dx_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_1dx_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_2zx.tpn` & `crds-7.6.0/crds/hst/tpns/cos_2zx.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_2zx_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_2zx_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_badt.tpn` & `crds-7.6.0/crds/hst/tpns/cos_badt.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_badt_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_badt_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_bpix.tpn` & `crds-7.6.0/crds/hst/tpns/cos_bpix.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_bpix_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_bpix_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_brf.tpn` & `crds-7.6.0/crds/hst/tpns/cos_brf.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_brf_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_brf_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_burst.tpn` & `crds-7.6.0/crds/hst/tpns/cos_burst.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_burst_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_burst_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_dead.tpn` & `crds-7.6.0/crds/hst/tpns/cos_dead.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_dead_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_dead_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_dgeo_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_dgeo_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_disp.tpn` & `crds-7.6.0/crds/hst/tpns/cos_disp.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_disp_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_disp_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_flat.tpn` & `crds-7.6.0/crds/hst/tpns/cos_flat.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_flat_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_flat_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_geo.tpn` & `crds-7.6.0/crds/hst/tpns/cos_geo.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_geo_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_geo_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_gsag.tpn` & `crds-7.6.0/crds/hst/tpns/cos_gsag.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_gsag_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_gsag_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_hv.tpn` & `crds-7.6.0/crds/hst/tpns/cos_hv.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_hv_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_hv_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_lamp.tpn` & `crds-7.6.0/crds/hst/tpns/cos_lamp.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_lamp_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_lamp_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_pha.tpn` & `crds-7.6.0/crds/hst/tpns/cos_pha.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_pha_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_pha_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_phot.tpn` & `crds-7.6.0/crds/hst/tpns/cos_phot.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_phot_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_phot_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_profile.tpn` & `crds-7.6.0/crds/hst/tpns/cos_profile.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_profile_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_profile_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_spot.tpn` & `crds-7.6.0/crds/hst/tpns/cos_spot.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_spot_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_spot_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_spwcs.tpn` & `crds-7.6.0/crds/hst/tpns/cos_spwcs.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_spwcs_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_spwcs_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_tds.tpn` & `crds-7.6.0/crds/hst/tpns/cos_tds.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_tds_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_tds_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_trace.tpn` & `crds-7.6.0/crds/hst/tpns/cos_trace.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_trace_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_trace_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_walk.tpn` & `crds-7.6.0/crds/hst/tpns/cos_walk.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_walk_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_walk_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_wcp.tpn` & `crds-7.6.0/crds/hst/tpns/cos_wcp.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_wcp_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_wcp_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_xwalk_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_xwalk_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/cos_ywalk_ld.tpn` & `crds-7.6.0/crds/hst/tpns/cos_ywalk_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/foc_bac.tpn` & `crds-7.6.0/crds/hst/tpns/foc_bac.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/foc_bac_ld.tpn` & `crds-7.6.0/crds/hst/tpns/foc_bac_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/foc_blm.tpn` & `crds-7.6.0/crds/hst/tpns/foc_blm.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/foc_blm_ld.tpn` & `crds-7.6.0/crds/hst/tpns/foc_blm_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/foc_cuni.tpn` & `crds-7.6.0/crds/hst/tpns/foc_cuni.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/foc_cuni_ld.tpn` & `crds-7.6.0/crds/hst/tpns/foc_cuni_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/foc_geo.tpn` & `crds-7.6.0/crds/hst/tpns/foc_geo.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/foc_geo_ld.tpn` & `crds-7.6.0/crds/hst/tpns/foc_geo_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/foc_itf.tpn` & `crds-7.6.0/crds/hst/tpns/foc_itf.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/foc_itf_ld.tpn` & `crds-7.6.0/crds/hst/tpns/foc_itf_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/foc_lsf.tpn` & `crds-7.6.0/crds/hst/tpns/foc_lsf.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/foc_lsf_ld.tpn` & `crds-7.6.0/crds/hst/tpns/foc_lsf_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/foc_sde.tpn` & `crds-7.6.0/crds/hst/tpns/foc_sde.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/foc_sde_ld.tpn` & `crds-7.6.0/crds/hst/tpns/foc_sde_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/foc_uni.tpn` & `crds-7.6.0/crds/hst/tpns/foc_uni.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/foc_uni_ld.tpn` & `crds-7.6.0/crds/hst/tpns/foc_uni_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ais.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ais.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ais_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ais_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_bac.tpn` & `crds-7.6.0/crds/hst/tpns/fos_bac.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_bac_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_bac_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccg2.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccg2.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccg2_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccg2_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccs0.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccs0.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccs0_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccs0_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccs1.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccs1.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccs1_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccs1_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccs2.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccs2.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccs2_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccs2_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccs3.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccs3.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccs3_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccs3_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccs4.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccs4.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccs4_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccs4_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccs5.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccs5.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccs5_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccs5_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccs6.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccs6.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccs6_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccs6_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccs7.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccs7.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccs7_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccs7_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccs8.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccs8.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccs8_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccs8_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccs9.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccs9.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccs9_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccs9_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccsa_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccsa_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccsb.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccsb.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccsb_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccsb_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccsc.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccsc.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccsc_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccsc_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccsd.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccsd.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccsd_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccsd_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccse.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccse.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccse_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccse_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccsf.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccsf.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ccsf_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ccsf_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ddt.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ddt.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ddt_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ddt_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_flt.tpn` & `crds-7.6.0/crds/hst/tpns/fos_flt.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_flt_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_flt_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ivs.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ivs.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ivs_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ivs_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_lsf.tpn` & `crds-7.6.0/crds/hst/tpns/fos_lsf.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_lsf_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_lsf_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_pcp.tpn` & `crds-7.6.0/crds/hst/tpns/fos_pcp.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_pcp_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_pcp_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_psf.tpn` & `crds-7.6.0/crds/hst/tpns/fos_psf.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_psf_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_psf_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_qin.tpn` & `crds-7.6.0/crds/hst/tpns/fos_qin.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_qin_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_qin_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ret.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ret.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/fos_ret_ld.tpn` & `crds-7.6.0/crds/hst/tpns/fos_ret_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_abs.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_abs.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_abs_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_abs_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccr1.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccr1.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccr1_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccr1_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccr2.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccr2.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccr2_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccr2_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccr3.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccr3.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccr3_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccr3_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccr4.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccr4.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccr4_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccr4_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccr5.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccr5.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccr5_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccr5_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccr6.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccr6.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccr6_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccr6_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccr7.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccr7.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccr7_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccr7_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccr8.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccr8.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccr8_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccr8_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccr9.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccr9.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccr9_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccr9_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccra.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccra.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccra_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccra_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccrb.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccrb.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccrb_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccrb_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccrc.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccrc.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccrc_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccrc_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccrd.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccrd.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccrd_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccrd_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccre.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccre.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_ccre_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_ccre_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_dio.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_dio.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_dio_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_dio_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_net.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_net.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_net_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_net_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_phc.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_phc.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_phc_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_phc_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_qin.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_qin.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_qin_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_qin_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_saa.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_saa.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_saa_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_saa_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_scoffc_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_scoffc_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_vig.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_vig.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hrs_vig_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hrs_vig_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hsp_ccp0_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hsp_ccp0_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hsp_ccp1.tpn` & `crds-7.6.0/crds/hst/tpns/hsp_ccp1.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hsp_ccp1_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hsp_ccp1_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hsp_ccp2.tpn` & `crds-7.6.0/crds/hst/tpns/hsp_ccp2.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hsp_ccp2_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hsp_ccp2_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hsp_ccp3.tpn` & `crds-7.6.0/crds/hst/tpns/hsp_ccp3.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hsp_ccp3_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hsp_ccp3_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hsp_ccp4.tpn` & `crds-7.6.0/crds/hst/tpns/hsp_ccp4.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hsp_ccp4_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hsp_ccp4_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hsp_ccp5.tpn` & `crds-7.6.0/crds/hst/tpns/hsp_ccp5.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hsp_ccp5_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hsp_ccp5_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hsp_ccp6_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hsp_ccp6_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hsp_ccp7.tpn` & `crds-7.6.0/crds/hst/tpns/hsp_ccp7.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hsp_ccp7_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hsp_ccp7_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hsp_ccp8.tpn` & `crds-7.6.0/crds/hst/tpns/hsp_ccp8.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hsp_ccp8_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hsp_ccp8_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/hsp_ccp9_ld.tpn` & `crds-7.6.0/crds/hst/tpns/hsp_ccp9_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_bkg.tpn` & `crds-7.6.0/crds/hst/tpns/nic_bkg.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_bkg_ld.tpn` & `crds-7.6.0/crds/hst/tpns/nic_bkg_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_drk.tpn` & `crds-7.6.0/crds/hst/tpns/nic_drk.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_drk_ld.tpn` & `crds-7.6.0/crds/hst/tpns/nic_drk_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_flt.tpn` & `crds-7.6.0/crds/hst/tpns/nic_flt.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_flt_ld.tpn` & `crds-7.6.0/crds/hst/tpns/nic_flt_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_idc.tpn` & `crds-7.6.0/crds/hst/tpns/nic_idc.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_idc_ld.tpn` & `crds-7.6.0/crds/hst/tpns/nic_idc_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_ilm.tpn` & `crds-7.6.0/crds/hst/tpns/nic_ilm.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_ilm_ld.tpn` & `crds-7.6.0/crds/hst/tpns/nic_ilm_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_lin.tpn` & `crds-7.6.0/crds/hst/tpns/nic_lin.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_lin_ld.tpn` & `crds-7.6.0/crds/hst/tpns/nic_lin_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_msk.tpn` & `crds-7.6.0/crds/hst/tpns/nic_msk.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_msk_ld.tpn` & `crds-7.6.0/crds/hst/tpns/nic_msk_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_nlc.tpn` & `crds-7.6.0/crds/hst/tpns/nic_nlc.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_nlc_ld.tpn` & `crds-7.6.0/crds/hst/tpns/nic_nlc_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_noi.tpn` & `crds-7.6.0/crds/hst/tpns/nic_noi.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_noi_ld.tpn` & `crds-7.6.0/crds/hst/tpns/nic_noi_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_pht.tpn` & `crds-7.6.0/crds/hst/tpns/nic_pht.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_pht_ld.tpn` & `crds-7.6.0/crds/hst/tpns/nic_pht_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_pmd.tpn` & `crds-7.6.0/crds/hst/tpns/nic_pmd.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_pmd_ld.tpn` & `crds-7.6.0/crds/hst/tpns/nic_pmd_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_pmk.tpn` & `crds-7.6.0/crds/hst/tpns/nic_pmk.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_pmk_ld.tpn` & `crds-7.6.0/crds/hst/tpns/nic_pmk_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_psb.tpn` & `crds-7.6.0/crds/hst/tpns/nic_psb.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_psb_ld.tpn` & `crds-7.6.0/crds/hst/tpns/nic_psb_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_scn.tpn` & `crds-7.6.0/crds/hst/tpns/nic_scn.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_scn_ld.tpn` & `crds-7.6.0/crds/hst/tpns/nic_scn_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_sdk.tpn` & `crds-7.6.0/crds/hst/tpns/nic_sdk.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_sdk_ld.tpn` & `crds-7.6.0/crds/hst/tpns/nic_sdk_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_tdd.tpn` & `crds-7.6.0/crds/hst/tpns/nic_tdd.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_tdd_ld.tpn` & `crds-7.6.0/crds/hst/tpns/nic_tdd_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_tdf.tpn` & `crds-7.6.0/crds/hst/tpns/nic_tdf.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_tdf_ld.tpn` & `crds-7.6.0/crds/hst/tpns/nic_tdf_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_zpr.tpn` & `crds-7.6.0/crds/hst/tpns/nic_zpr.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/nic_zpr_ld.tpn` & `crds-7.6.0/crds/hst/tpns/nic_zpr_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_1dt.tpn` & `crds-7.6.0/crds/hst/tpns/stis_1dt.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_1dt_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_1dt_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_1dx.tpn` & `crds-7.6.0/crds/hst/tpns/stis_1dx.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_1dx_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_1dx_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_a2d.tpn` & `crds-7.6.0/crds/hst/tpns/stis_a2d.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_a2d_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_a2d_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_any_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_any_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_apd.tpn` & `crds-7.6.0/crds/hst/tpns/stis_apd.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_apd_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_apd_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_apt.tpn` & `crds-7.6.0/crds/hst/tpns/stis_apt.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_apt_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_apt_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_bia.tpn` & `crds-7.6.0/crds/hst/tpns/stis_bia.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_bia_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_bia_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_bpx.tpn` & `crds-7.6.0/crds/hst/tpns/stis_bpx.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_bpx_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_bpx_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_ccd.tpn` & `crds-7.6.0/crds/hst/tpns/stis_ccd.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_ccd_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_ccd_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_cds.tpn` & `crds-7.6.0/crds/hst/tpns/stis_cds.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_cds_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_cds_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_crr.tpn` & `crds-7.6.0/crds/hst/tpns/stis_crr.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_crr_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_crr_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_dfl.tpn` & `crds-7.6.0/crds/hst/tpns/stis_dfl.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_dfl_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_dfl_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_drk.tpn` & `crds-7.6.0/crds/hst/tpns/stis_drk.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_drk_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_drk_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_dsp.tpn` & `crds-7.6.0/crds/hst/tpns/stis_dsp.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_dsp_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_dsp_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_ech.tpn` & `crds-7.6.0/crds/hst/tpns/stis_ech.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_ech_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_ech_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_exs.tpn` & `crds-7.6.0/crds/hst/tpns/stis_exs.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_exs_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_exs_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_gac.tpn` & `crds-7.6.0/crds/hst/tpns/stis_gac.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_gac_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_gac_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_hal.tpn` & `crds-7.6.0/crds/hst/tpns/stis_hal.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_hal_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_hal_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_iac.tpn` & `crds-7.6.0/crds/hst/tpns/stis_iac.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_iac_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_iac_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_idc.tpn` & `crds-7.6.0/crds/hst/tpns/stis_idc.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_idc_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_idc_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_imp.tpn` & `crds-7.6.0/crds/hst/tpns/stis_imp.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_imp_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_imp_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_lfl.tpn` & `crds-7.6.0/crds/hst/tpns/stis_lfl.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_lfl_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_lfl_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_lin.tpn` & `crds-7.6.0/crds/hst/tpns/stis_lin.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_lin_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_lin_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_lmp.tpn` & `crds-7.6.0/crds/hst/tpns/stis_lmp.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_lmp_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_lmp_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_moc.tpn` & `crds-7.6.0/crds/hst/tpns/stis_moc.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_moc_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_moc_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_pct.tpn` & `crds-7.6.0/crds/hst/tpns/stis_pct.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_pct_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_pct_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_pfl.tpn` & `crds-7.6.0/crds/hst/tpns/stis_pfl.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_pfl_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_pfl_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_pht.tpn` & `crds-7.6.0/crds/hst/tpns/stis_pht.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_pht_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_pht_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_rip.tpn` & `crds-7.6.0/crds/hst/tpns/stis_rip.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_rip_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_rip_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_sdc.tpn` & `crds-7.6.0/crds/hst/tpns/stis_sdc.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_sdc_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_sdc_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_srw.tpn` & `crds-7.6.0/crds/hst/tpns/stis_srw.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_srw_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_srw_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_ssc.tpn` & `crds-7.6.0/crds/hst/tpns/stis_ssc.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_ssc_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_ssc_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_ssd.tpn` & `crds-7.6.0/crds/hst/tpns/stis_ssd.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_ssd_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_ssd_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_tdc.tpn` & `crds-7.6.0/crds/hst/tpns/stis_tdc.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_tdc_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_tdc_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_tds.tpn` & `crds-7.6.0/crds/hst/tpns/stis_tds.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_tds_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_tds_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_tel.tpn` & `crds-7.6.0/crds/hst/tpns/stis_tel.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_tel_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_tel_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_wcp.tpn` & `crds-7.6.0/crds/hst/tpns/stis_wcp.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/stis_wcp_ld.tpn` & `crds-7.6.0/crds/hst/tpns/stis_wcp_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/synphot_syn.tpn` & `crds-7.6.0/crds/hst/tpns/wp2_drk_ld.tpn`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 # Template file used by certify to check reference files
 # Some fields may be abbreviated to their first character:
 #
 # keytype = (Header|Group|Column)
 # datatype = (Integer|Real|Logical|Double|Character)
 # presence = (Optional|Required)
 #
-# 05/17/2007 58081  MSwam  change PEDIGREE validation by request
-#
 # NAME          KEYTYPE  DATATYPE  PRESENCE VALUES
 #--------------------------------------------------------------------------
-DBTABLE             H        C         R    CRTHROUGHPUT
-USEAFTER            H        C         R    &SYBDATE
-INSTRUME            H        C         R
+FILE_NAME	    H        C         R
+USEAFTER_DATE       H        C         R    &SYBDATE
+OPUS_FLAG           H        C         R    Y,N
+COMPARISON_FILE     H        C         R    
 COMMENT             H        C         R
-HISTORY             H        C         R
-COMPNAME            H        C         R
-DESCRIP             H        C         R
-PEDIGREE            H        C         W    &PEDIGREE
-DATE                H        C         R
-
-WAVELENGTH      C        R             R
-THROUGHPUT      C        R             W
-
-# Warn when the first and last throughput values are not both equal to 0:
-EXT1            D        X             R    (warn_only((EXT1_ARRAY.DATA.field("THROUGHPUT")[[0,-1]]==0.0).all()))
+INSTRUMENT	    H	     C	       R    WFPC2
+REFERENCE_FILE_TYPE H        C         R    DRK
+CHANGE_LEVEL        C        C         R    TRIVIAL,MODERATE,SEVERE
+PEDIGREE	    C        C	       R    INFLIGHT,GROUND,MODEL,DUMMY
+OBSERVATION_BEGIN_DATE  C    C         O    &SYBDATE
+OBSERVATION_END_DATE    C    C         O    &SYBDATE
+COMMENT             C        C         P
+MODE		    C	     C	       R    FULL,AREA
+SERIALS		    C	     C	       R    ON,OFF
+ATODGAIN	    C	     R	       R    7.00000:15.0000
```

### Comparing `crds-7.5.0.0/crds/hst/tpns/synphot_syn_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wp2_w4t.tpn`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 # Template file used by certify to check reference files
 # Some fields may be abbreviated to their first character:
 #
 # keytype = (Header|Group|Column)
 # datatype = (Integer|Real|Logical|Double|Character)
 # presence = (Optional|Required)
 #
-# 05/17/2007 58081  MSwam  change PEDIGREE validation by request
-#
 # NAME          KEYTYPE  DATATYPE  PRESENCE VALUES
 #--------------------------------------------------------------------------
-DBTABLE             H        C         R    CRTHROUGHPUT
+DATATYPE            H        C         R    REAL*4
+NAXIS               H        I         R    2
+GCOUNT              H        I         R    4
+INSTRUME            H        C         R    WFPC2
+FILETYPE            H        C         R    W4T
 USEAFTER            H        C         R    &SYBDATE
-INSTRUME            H        C         R
-COMMENT             H        C         R
-HISTORY             H        C         R
-COMPNAME            H        C         R
-DESCRIP             H        C         R
-PEDIGREE            H        C         W    &PEDIGREE
-DATE                H        C         R
-
-WAVELENGTH      C        R             R
-THROUGHPUT      C        R             W
-
-# Warn when the first and last throughput values are not both equal to 0:
-EXT1            D        X             R    (warn_only((EXT1_ARRAY.DATA.field("THROUGHPUT")[[0,-1]]==0.0).all()))
+IMAGETYP            H        C         R    SPECIAL,CDBS
+CDBSFILE            H        C         R    W4T
+PEDIGREE            H        C         R    &PEDIGREE
+DESCRIP             H        C         R    
+ATODGAIN            H        R         R    7.00000:15.0000
+DETECTOR            G        I         R    1:4
```

### Comparing `crds-7.5.0.0/crds/hst/tpns/synphot_th.tpn` & `crds-7.6.0/crds/hst/tpns/synphot_th.tpn`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,19 @@
 # NAME          KEYTYPE  DATATYPE  PRESENCE VALUES
 #--------------------------------------------------------------------------
 DBTABLE             H        C         R    CRTHERMAL
 USEAFTER            H        C         R    &SYBDATE
 INSTRUME            H        C         R
 COMMENT             H        C         R
 HISTORY             H        C         R
+
 COMPNAME            H        C         R
+COMPNAME            H        X         R    ((len(COMPNAME)>0)and(len(COMPNAME)<=18)and(COMPNAME==COMPNAME.lower()))
+
 DESCRIP             H        C         R
 DATE                H        C         R
 PEDIGREE            H        C         W    &PEDIGREE
 
 WAVELENGTH          C        R         R
 EMISSIVITY          C        R         W
+
+EXT1                D        X         R    &SYNPHOT_THERMAL
```

### Comparing `crds-7.5.0.0/crds/hst/tpns/synphot_th_ld.tpn` & `crds-7.6.0/crds/hst/tpns/synphot_th_ld.tpn`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,19 @@
 # NAME          KEYTYPE  DATATYPE  PRESENCE VALUES
 #--------------------------------------------------------------------------
 DBTABLE             H        C         R    CRTHERMAL
 USEAFTER            H        C         R    &SYBDATE
 INSTRUME            H        C         R
 COMMENT             H        C         R
 HISTORY             H        C         R
+
 COMPNAME            H        C         R
+COMPNAME            H        X         R    ((len(COMPNAME)>0)and(len(COMPNAME)<=18)and(COMPNAME==COMPNAME.lower()))
+
 DESCRIP             H        C         R
 DATE                H        C         R
 PEDIGREE            H        C         W    &PEDIGREE
 
 WAVELENGTH          C        R         R
 EMISSIVITY          C        R         W
+
+EXT1                D        X         R    &SYNPHOT_THERMAL
```

### Comparing `crds-7.5.0.0/crds/hst/tpns/synphot_tmc.tpn` & `crds-7.6.0/crds/hst/tpns/synphot_tmc.tpn`

 * *Files 21% similar despite different names*

```diff
@@ -11,11 +11,17 @@
 INSTRUME            H        C         R    HST,SYNPHOT
 DBTABLE             H        C         R    CRCOMPLIST
 DESCRIP             H        C         R
 COMMENT             H        C         R
 HISTORY             H        C         R
 
 TIME                C        C         R
+
 COMPNAME            C        C         R
-FILENAME            C        C         W   &FileExists
+COMPNAME            C        X         R    ((len(VALUE)>0)and(VALUE==VALUE.lower()))
+
+FILENAME            C        C         R
+FILENAME            C        X         R    ((len(VALUE)>0)and(VALUE==VALUE.lower()))
+
 COMMENT             C        C         R
 
+EXT1                D        X         R    &SYNPHOT_LOOKUP
```

### Comparing `crds-7.5.0.0/crds/hst/tpns/synphot_tmc_ld.tpn` & `crds-7.6.0/crds/hst/tpns/synphot_obs.tpn`

 * *Files 14% similar despite different names*

```diff
@@ -4,18 +4,14 @@
 # keytype = (Header|Group|Column)
 # datatype = (Integer|Real|Logical|Double|Character)
 # presence = (Optional|Required)
 #
 # NAME          KEYTYPE  DATATYPE  PRESENCE VALUES
 #--------------------------------------------------------------------------
 USEAFTER            H        C         R    &SYBDATE
-INSTRUME            H        C         R    HST,SYNPHOT
-DBTABLE             H        C         R    CRCOMPLIST
+INSTRUME            H        C         R    SYNPHOT
+DBTABLE             H        C         R    CROBSMODELIST
 DESCRIP             H        C         R
 COMMENT             H        C         R
 HISTORY             H        C         R
 
-TIME                C        C         R
-COMPNAME            C        C         R
-FILENAME            C        C         R  
-COMMENT             C        C         R
-
+OBSMODE             C        C         R
```

### Comparing `crds-7.5.0.0/crds/hst/tpns/synphot_tmg.tpn` & `crds-7.6.0/crds/hst/tpns/synphot_tmc_ld.tpn`

 * *Files 14% similar despite different names*

```diff
@@ -5,20 +5,23 @@
 # datatype = (Integer|Real|Logical|Double|Character)
 # presence = (Optional|Required)
 #
 # NAME          KEYTYPE  DATATYPE  PRESENCE VALUES
 #--------------------------------------------------------------------------
 USEAFTER            H        C         R    &SYBDATE
 INSTRUME            H        C         R    HST,SYNPHOT
-DBTABLE             H        C         R    CRGRAPH
+DBTABLE             H        C         R    CRCOMPLIST
 DESCRIP             H        C         R
-GENERATI            H        I         R
 COMMENT             H        C         R
 HISTORY             H        C         R
 
+TIME                C        C         R
+
 COMPNAME            C        C         R
-INNODE	            C        I         R
-OUTNODE             C        I         R
-KEYWORD             C        C         R
-THCOMPNAME          C        C         R
+COMPNAME            C        X         R    ((len(VALUE)>0)and(VALUE==VALUE.lower()))
+
+FILENAME            C        C         R
+FILENAME            C        X         R    ((len(VALUE)>0)and(VALUE==VALUE.lower()))
+
 COMMENT             C        C         R
 
+EXT1                D        X         R    &SYNPHOT_LOOKUP
```

### Comparing `crds-7.5.0.0/crds/hst/tpns/synphot_tmg_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_lin.tpn`

 * *Files 20% similar despite different names*

```diff
@@ -3,22 +3,13 @@
 #
 # keytype = (Header|Group|Column)
 # datatype = (Integer|Real|Logical|Double|Character)
 # presence = (Optional|Required)
 #
 # NAME          KEYTYPE  DATATYPE  PRESENCE VALUES
 #--------------------------------------------------------------------------
-USEAFTER            H        C         R    &SYBDATE
-INSTRUME            H        C         R    HST,SYNPHOT
-DBTABLE             H        C         R    CRGRAPH
+INSTRUME            H        C         R    WFC3
+FILETYPE            H        C         R    "LINEARITY COEFFICIENTS"
+DETECTOR            H        C         R    IR
+PEDIGREE            H        C         R    &PEDIGREE
 DESCRIP             H        C         R
-GENERATI            H        I         R
-COMMENT             H        C         R
-HISTORY             H        C         R
-
-COMPNAME            C        C         R
-INNODE	            C        I         R
-OUTNODE             C        I         R
-KEYWORD             C        C         R
-THCOMPNAME          C        C         R
-COMMENT             C        C         R
-
+USEAFTER            H        C         R    &SYBDATE
```

### Comparing `crds-7.5.0.0/crds/hst/tpns/synphot_tmt.tpn` & `crds-7.6.0/crds/hst/tpns/wp2_idc.tpn`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 # Template file used by certify to check reference files
 # Some fields may be abbreviated to their first character:
 #
 # keytype = (Header|Group|Column)
 # datatype = (Integer|Real|Logical|Double|Character)
 # presence = (Optional|Required)
 #
-# 05/17/2007 58081  MSwam  change PEDIGREE validation by request
+# 07/08/04 51069  MSwam   first version
 #
 # NAME          KEYTYPE  DATATYPE  PRESENCE VALUES
 #--------------------------------------------------------------------------
+INSTRUME            H        C         R    WFPC2
+FILETYPE            H        C         R    "DISTORTION COEFFICIENTS"
 USEAFTER            H        C         R    &SYBDATE
-INSTRUME            H        C         R    HST,SYNPHOT
-DBTABLE             H        C         R    CRTHERMLIST
-COMMENT             H        C         R
-HISTORY             H        C         R
-DESCRIP             H        C         R
 PEDIGREE            H        C         R    &PEDIGREE
-
-TIME                C        C         R    &SYBDATE
-COMPNAME            C        C         R
-FILENAME            C        C         W    &FileExists
-COMMENT             C        C         R
+NORDER              H        I         R
+DETCHIP             C        I         R    1,2,3,4
+DIRECTION           C        C         R    FORWARD
```

### Comparing `crds-7.5.0.0/crds/hst/tpns/synphot_tmt_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wp2_phot.tpn`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # Template file used by certify to check reference files
 # Some fields may be abbreviated to their first character:
 #
 # keytype = (Header|Group|Column)
 # datatype = (Integer|Real|Logical|Double|Character)
 # presence = (Optional|Required)
 #
-# 05/17/2007 58081  MSwam  change PEDIGREE validation by request
-#
 # NAME          KEYTYPE  DATATYPE  PRESENCE VALUES
 #--------------------------------------------------------------------------
-USEAFTER            H        C         R    &SYBDATE
-INSTRUME            H        C         R    HST,SYNPHOT
-DBTABLE             H        C         R    CRTHERMLIST
-COMMENT             H        C         R
-HISTORY             H        C         R
-DESCRIP             H        C         R
-PEDIGREE            H        C         R    &PEDIGREE
-
-TIME                C        C         R    &SYBDATE
-COMPNAME            C        C         R
-FILENAME            C        C         R
-COMMENT             C        C         R
+DETECTOR            C        I         R    1:4
+USEAFTER       H        C         R    &SYBDATE
+MODE                C        C         R    FULL,AREA
+GAIN                C        C         R    
+BUNIT               C        C         R    
+FILTNAM1            C        C         R    
+FILTNAM2            C        C         R    
+PHOTMODE            C        C         R    
+PHOTFLAM            C        R         R    
+PHOTZPT             C        R         R    
+PHOTPLAM            C        R         R    
+PHOTBW              C        R         R
```

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_a2d.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_a2d.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_a2d_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_a2d_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_bia.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_bia.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_bia_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_bia_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_bic.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_bic.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_bic_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_bic_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_bpx.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_bpx.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_bpx_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_bpx_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_ccd.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_ccd.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_ccd_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_ccd_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_crr_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_crr_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_cte.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_cte.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_cte_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_cte_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_d2i.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_d2i.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_d2i_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_d2i_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_dfl.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_dfl.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_dfl_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_dfl_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_dkc.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_dkc.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_dkc_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_dkc_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_drk.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_drk.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_drk_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_drk_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_fls.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_fls.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_fls_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_fls_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_idc.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_idc.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_idc_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_idc_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_imp.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_imp.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_imp_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_imp_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_lfl.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_lfl.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_lfl_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_lfl_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_lin.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_npl.tpn`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 # Template file used by certify to check reference files
 # Some fields may be abbreviated to their first character:
 #
 # keytype = (Header|Group|Column)
 # datatype = (Integer|Real|Logical|Double|Character)
 # presence = (Optional|Required)
 #
-# NAME          KEYTYPE  DATATYPE  PRESENCE VALUES
-#--------------------------------------------------------------------------
-INSTRUME            H        C         R    WFC3
-FILETYPE            H        C         R    "LINEARITY COEFFICIENTS"
-DETECTOR            H        C         R    IR
-PEDIGREE            H        C         R    &PEDIGREE
-DESCRIP             H        C         R
-USEAFTER            H        C         R    &SYBDATE
+# History:
+# 09/01/11  MSwam  69084   first version
+#
+# NAME  KEYTYPE  DATATYPE       PRESENCE        VALUES
+#----------------------------------------------------------
+INSTRUME        H       C       R       WFC3
+FILETYPE        H       C       R       "DXY GRID"
+DETECTOR        H       C       R       UVIS
+TELESCOP        H       C       R       HST
+OBSTYPE         H       C       R       IMAGING
+FILTER          H       C       R
+USEAFTER        H       C       R       &SYBDATE
+PEDIGREE        H       C       R       &PEDIGREE
+DESCRIP         H       C       R
```

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_lin_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_lin_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_mdz_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_mdz_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_npl.tpn` & `crds-7.6.0/crds/hst/tpns/wp2_w4t_ld.tpn`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Template file used by certify to check reference files
 # Some fields may be abbreviated to their first character:
 #
 # keytype = (Header|Group|Column)
 # datatype = (Integer|Real|Logical|Double|Character)
 # presence = (Optional|Required)
 #
-# History:
-# 09/01/11  MSwam  69084   first version
-#
-# NAME  KEYTYPE  DATATYPE       PRESENCE        VALUES
-#----------------------------------------------------------
-INSTRUME        H       C       R       WFC3
-FILETYPE        H       C       R       "DXY GRID"
-DETECTOR        H       C       R       UVIS
-TELESCOP        H       C       R       HST
-OBSTYPE         H       C       R       IMAGING
-FILTER          H       C       R
-USEAFTER        H       C       R       &SYBDATE
-PEDIGREE        H       C       R       &PEDIGREE
-DESCRIP         H       C       R
+# NAME          KEYTYPE  DATATYPE  PRESENCE VALUES
+#--------------------------------------------------------------------------
+FILE_NAME	    H        C         R
+USEAFTER_DATE       H        C         R    &SYBDATE
+OPUS_FLAG           H        C         R    Y,N
+COMPARISON_FILE     H        C         R    
+COMMENT             H        C         R
+INSTRUMENT	    H	     C	       R    WFPC2
+REFERENCE_FILE_TYPE H        C         R    W4T
+ATODGAIN            C        R         R    7.00000:15.0000
+CHANGE_LEVEL        C        C         R    TRIVIAL,MODERATE,SEVERE
+PEDIGREE	    C        C	       R    INFLIGHT,GROUND,MODEL,DUMMY
+OBSERVATION_BEGIN_DATE  C    C         O    &SYBDATE
+OBSERVATION_END_DATE    C    C         O    &SYBDATE
+COMMENT             C        C         P
```

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_npl_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_npl_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_osc.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_osc.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_osc_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_osc_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_pfl.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_pfl.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_pfl_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_pfl_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_shd_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_shd_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_snk.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_snk.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfc3_snk_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfc3_snk_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfp_a2d.tpn` & `crds-7.6.0/crds/hst/tpns/wfp_a2d.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfp_a2d_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfp_a2d_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfp_bas.tpn` & `crds-7.6.0/crds/hst/tpns/wfp_bas.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfp_bas_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfp_bas_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfp_dfl.tpn` & `crds-7.6.0/crds/hst/tpns/wfp_dfl.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfp_dfl_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfp_dfl_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfp_dqf.tpn` & `crds-7.6.0/crds/hst/tpns/wfp_dqf.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfp_dqf_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfp_dqf_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfp_drk.tpn` & `crds-7.6.0/crds/hst/tpns/wfp_drk.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfp_drk_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfp_drk_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfp_flt.tpn` & `crds-7.6.0/crds/hst/tpns/wfp_flt.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfp_flt_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfp_flt_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfp_msk.tpn` & `crds-7.6.0/crds/hst/tpns/wfp_msk.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfp_msk_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfp_msk_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfp_phot.tpn` & `crds-7.6.0/crds/hst/tpns/wfp_phot.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfp_phot_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfp_phot_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfp_prf.tpn` & `crds-7.6.0/crds/hst/tpns/wfp_prf.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfp_prf_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfp_prf_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfp_psf.tpn` & `crds-7.6.0/crds/hst/tpns/wfp_psf.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfp_psf_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfp_psf_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfp_spg.tpn` & `crds-7.6.0/crds/hst/tpns/wfp_spg.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wfp_spg_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wfp_spg_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wp2_a2d.tpn` & `crds-7.6.0/crds/hst/tpns/wp2_a2d.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wp2_a2d_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wp2_a2d_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wp2_bas.tpn` & `crds-7.6.0/crds/hst/tpns/wp2_bas.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wp2_bas_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wp2_bas_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wp2_dqf.tpn` & `crds-7.6.0/crds/hst/tpns/wp2_dqf.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wp2_dqf_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wp2_dqf_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wp2_drk.tpn` & `crds-7.6.0/crds/hst/tpns/wp2_drk.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wp2_drk_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wp2_msk_ld.tpn`

 * *Files 16% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 #--------------------------------------------------------------------------
 FILE_NAME	    H        C         R
 USEAFTER_DATE       H        C         R    &SYBDATE
 OPUS_FLAG           H        C         R    Y,N
 COMPARISON_FILE     H        C         R    
 COMMENT             H        C         R
 INSTRUMENT	    H	     C	       R    WFPC2
-REFERENCE_FILE_TYPE H        C         R    DRK
+REFERENCE_FILE_TYPE H        C         R    MSK
 CHANGE_LEVEL        C        C         R    TRIVIAL,MODERATE,SEVERE
 PEDIGREE	    C        C	       R    INFLIGHT,GROUND,MODEL,DUMMY
 OBSERVATION_BEGIN_DATE  C    C         O    &SYBDATE
 OBSERVATION_END_DATE    C    C         O    &SYBDATE
 COMMENT             C        C         P
 MODE		    C	     C	       R    FULL,AREA
 SERIALS		    C	     C	       R    ON,OFF
-ATODGAIN	    C	     R	       R    7.00000:15.0000
```

### Comparing `crds-7.5.0.0/crds/hst/tpns/wp2_dxy_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wp2_dxy_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wp2_flt.tpn` & `crds-7.6.0/crds/hst/tpns/wp2_flt.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wp2_flt_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wp2_flt_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wp2_idc.tpn` & `crds-7.6.0/crds/hst/tpns/wp2_off.tpn`

 * *Files 15% similar despite different names*

```diff
@@ -6,13 +6,11 @@
 # presence = (Optional|Required)
 #
 # 07/08/04 51069  MSwam   first version
 #
 # NAME          KEYTYPE  DATATYPE  PRESENCE VALUES
 #--------------------------------------------------------------------------
 INSTRUME            H        C         R    WFPC2
-FILETYPE            H        C         R    "DISTORTION COEFFICIENTS"
+FILETYPE            H        C         R    "CHIP OFFSET"
 USEAFTER            H        C         R    &SYBDATE
 PEDIGREE            H        C         R    &PEDIGREE
-NORDER              H        I         R
 DETCHIP             C        I         R    1,2,3,4
-DIRECTION           C        C         R    FORWARD
```

### Comparing `crds-7.5.0.0/crds/hst/tpns/wp2_idc_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wp2_idc_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wp2_msk.tpn` & `crds-7.6.0/crds/hst/tpns/wp2_msk.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wp2_msk_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wp2_off_ld.tpn`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,13 @@
 #--------------------------------------------------------------------------
 FILE_NAME	    H        C         R
 USEAFTER_DATE       H        C         R    &SYBDATE
 OPUS_FLAG           H        C         R    Y,N
 COMPARISON_FILE     H        C         R    
 COMMENT             H        C         R
 INSTRUMENT	    H	     C	       R    WFPC2
-REFERENCE_FILE_TYPE H        C         R    MSK
+REFERENCE_FILE_TYPE H        C         R    OFF
 CHANGE_LEVEL        C        C         R    TRIVIAL,MODERATE,SEVERE
 PEDIGREE	    C        C	       R    INFLIGHT,GROUND,MODEL,DUMMY
 OBSERVATION_BEGIN_DATE  C    C         O    &SYBDATE
 OBSERVATION_END_DATE    C    C         O    &SYBDATE
 COMMENT             C        C         P
-MODE		    C	     C	       R    FULL,AREA
-SERIALS		    C	     C	       R    ON,OFF
```

### Comparing `crds-7.5.0.0/crds/hst/tpns/wp2_off.tpn` & `crds-7.6.0/crds/hst/tpns/wp2_phot_ld.tpn`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 # Template file used by certify to check reference files
 # Some fields may be abbreviated to their first character:
 #
 # keytype = (Header|Group|Column)
 # datatype = (Integer|Real|Logical|Double|Character)
 # presence = (Optional|Required)
 #
-# 07/08/04 51069  MSwam   first version
-#
 # NAME          KEYTYPE  DATATYPE  PRESENCE VALUES
 #--------------------------------------------------------------------------
-INSTRUME            H        C         R    WFPC2
-FILETYPE            H        C         R    "CHIP OFFSET"
-USEAFTER            H        C         R    &SYBDATE
-PEDIGREE            H        C         R    &PEDIGREE
-DETCHIP             C        I         R    1,2,3,4
+FILE_NAME	    H        C         R
+USEAFTER_DATE       H        C         R    &SYBDATE
+OPUS_FLAG           H        C         R    Y,N
+COMPARISON_FILE     H        C         R    
+COMMENT             H        C         R
+INSTRUMENT	    H	     C	       R    WFPC2
+REFERENCE_FILE_TYPE H        C         R    PHOT
+CHANGE_LEVEL        C        C         R    TRIVIAL,MODERATE,SEVERE
+PEDIGREE	    C        C	       R    INFLIGHT,GROUND,MODEL,DUMMY
+OBSERVATION_BEGIN_DATE  C    C         O    &SYBDATE
+OBSERVATION_END_DATE    C    C         O    &SYBDATE
+COMMENT             C        C         P
+MODE		    C	     C	       R    FULL,AREA
+PHOTMODE	    C	     C	       R
```

### Comparing `crds-7.5.0.0/crds/hst/tpns/wp2_off_ld.tpn` & `crds-7.6.0/crds/hst/tpns/wp2_shd_ld.tpn`

 * *Files 8% similar despite different names*

```diff
@@ -9,13 +9,16 @@
 #--------------------------------------------------------------------------
 FILE_NAME	    H        C         R
 USEAFTER_DATE       H        C         R    &SYBDATE
 OPUS_FLAG           H        C         R    Y,N
 COMPARISON_FILE     H        C         R    
 COMMENT             H        C         R
 INSTRUMENT	    H	     C	       R    WFPC2
-REFERENCE_FILE_TYPE H        C         R    OFF
+REFERENCE_FILE_TYPE H        C         R    SHD
 CHANGE_LEVEL        C        C         R    TRIVIAL,MODERATE,SEVERE
 PEDIGREE	    C        C	       R    INFLIGHT,GROUND,MODEL,DUMMY
 OBSERVATION_BEGIN_DATE  C    C         O    &SYBDATE
 OBSERVATION_END_DATE    C    C         O    &SYBDATE
 COMMENT             C        C         P
+MODE		    C	     C	       R    FULL,AREA
+SERIALS		    C	     C	       R    ON,OFF
+SHUTTER		    C	     C	       R    A,B
```

### Comparing `crds-7.5.0.0/crds/hst/tpns/wp2_psf.tpn` & `crds-7.6.0/crds/hst/tpns/wp2_psf.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wp2_shd.tpn` & `crds-7.6.0/crds/hst/tpns/wp2_shd.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/tpns/wp2_w4t.tpn` & `crds-7.6.0/crds/jwst/tpns/all_dark.tpn`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 # Template file used by certify to check reference files
 # Some fields may be abbreviated to their first character:
 #
 # keytype = (Header|Group|Column)
 # datatype = (Integer|Real|Logical|Double|Character)
 # presence = (Optional|Required)
 #
-# NAME          KEYTYPE  DATATYPE  PRESENCE VALUES
-#--------------------------------------------------------------------------
-DATATYPE            H        C         R    REAL*4
-NAXIS               H        I         R    2
-GCOUNT              H        I         R    4
-INSTRUME            H        C         R    WFPC2
-FILETYPE            H        C         R    W4T
-USEAFTER            H        C         R    &SYBDATE
-IMAGETYP            H        C         R    SPECIAL,CDBS
-CDBSFILE            H        C         R    W4T
-PEDIGREE            H        C         R    &PEDIGREE
-DESCRIP             H        C         R    
-ATODGAIN            H        R         R    7.00000:15.0000
-DETECTOR            G        I         R    1:4
+# NAME  KEYTYPE  DATATYPE   PRESENCE    VALUES
+#----------------------------------------------------------
+META.SUBARRAY.NAME          X   X   R   (not(META_SUBARRAY_NAME)in(['GENERIC','N/A']))
+META.EXPOSURE.NFRAMES       H   I   R  
+META.EXPOSURE.GROUPGAP      H   I   R   
+META.EXPOSURE.NGROUPS       H   I   R                  
+
+# SCI     A     X      R    (ndim(SCI_ARRAY,3))
+# ERR     A     X      O    (ndim(ERR_ARRAY,3))
+# DQ      A     X      O    (ndim(DQ_ARRAY,2))
```

### Comparing `crds-7.5.0.0/crds/hst/wfc3.py` & `crds-7.6.0/crds/hst/wfc3.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/hst/wfpc2.py` & `crds-7.6.0/crds/hst/wfpc2.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/io/abstract.py` & `crds-7.6.0/crds/io/abstract.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/io/asdf.py` & `crds-7.6.0/crds/io/asdf.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/io/factory.py` & `crds-7.6.0/crds/io/factory.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/io/fits.py` & `crds-7.6.0/crds/io/fits.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/io/geis.py` & `crds-7.6.0/crds/io/geis.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/io/json.py` & `crds-7.6.0/crds/io/json.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/io/tables.py` & `crds-7.6.0/crds/io/tables.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/io/yaml.py` & `crds-7.6.0/crds/io/yaml.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/__init__.py` & `crds-7.6.0/crds/jwst/__init__.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/gen_system_crdscfg.py` & `crds-7.6.0/crds/jwst/gen_system_crdscfg.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/jwst_system_crdscfg_b7.1.1.yaml` & `crds-7.6.0/crds/jwst/jwst_system_crdscfg_b7.1.1.yaml`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/jwst_system_crdscfg_b7.1.3.yaml` & `crds-7.6.0/crds/jwst/jwst_system_crdscfg_b7.1.3.yaml`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/jwst_system_crdscfg_b7.1.yaml` & `crds-7.6.0/crds/jwst/jwst_system_crdscfg_b7.1.yaml`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/jwst_system_crdscfg_b7.2.yaml` & `crds-7.6.0/crds/jwst/jwst_system_crdscfg_b7.2.yaml`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/jwst_system_crdscfg_b7.3.yaml` & `crds-7.6.0/crds/jwst/jwst_system_crdscfg_b7.3.yaml`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/jwst_system_crdscfg_b7.4.yaml` & `crds-7.6.0/crds/jwst/jwst_system_crdscfg_b7.4.yaml`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/jwst_system_crdscfg_b7.5.yaml` & `crds-7.6.0/crds/jwst/jwst_system_crdscfg_b7.5.yaml`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/jwst_system_crdscfg_b7.yaml` & `crds-7.6.0/crds/jwst/jwst_system_crdscfg_b7.yaml`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/locate.py` & `crds-7.6.0/crds/jwst/locate.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/pipeline.py` & `crds-7.6.0/crds/jwst/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,15 +237,16 @@
     ('0.9.0', "jwst_system_crdscfg_b7.1.yaml"),
     ('0.9.1', "jwst_system_crdscfg_b7.1.1.yaml"),
     ('0.9.3', "jwst_system_crdscfg_b7.1.3.yaml"),
     ('0.10.0', "jwst_system_crdscfg_b7.2.yaml"),
     ('0.13.0', "jwst_system_crdscfg_b7.3.yaml"),
     ('0.13.8', "jwst_system_crdscfg_b7.4.yaml"),
     ('0.16.0', "jwst_system_crdscfg_b7.5.yaml"),
-    ('999.0.0', "jwst_system_crdscfg_b7.5.yaml"),   # latest backstop
+    ('0.17.0', "jwst_system_crdscfg_b7.6.yaml"),
+    ('999.0.0', "jwst_system_crdscfg_b7.6.yaml"),   # latest backstop
 ]
 
 def _get_config_refpath(context, cal_ver):
     """Given CRDS `context` and calibration s/w version `cal_ver`,  identify the applicable
     SYSTEM CRDSCFG reference file, cache it, and return the file path.
     """
     context = _get_missing_context(context)
```

### Comparing `crds-7.5.0.0/crds/jwst/schema.py` & `crds-7.6.0/crds/jwst/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # ====================================================================================
 
 # from jwst import datamodels   # deferred
 # from . import locate  # deferred
 
 import crds
 from crds.core import log, utils, heavy_client, config
-from crds.certify import TpnInfo
+from crds.certify.generic_tpn import TpnInfo
 
 # ====================================================================================
 
 INSTR_PREFIX = {
     "fgs" : "FGS_",
     "miri" : "MIR_",
     "nircam" : "NRC_",
```

### Comparing `crds-7.5.0.0/crds/jwst/specs/combined_specs.json` & `crds-7.6.0/crds/jwst/specs/combined_specs.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9959496442255062%*

 * *Differences: {"'niriss'": "{'pars-image2pipeline': OrderedDict([('derived_from', 'Hand made 2020-08-18'), "*

 * *             "('extra_keys', None), ('file_ext', '.asdf'), ('filekind', 'pars-image2pipeline'), "*

 * *             "('filetype', 'PARS-IMAGE2PIPELINE'), ('instrument', 'NIRISS'), ('ld_tpn', "*

 * *             "'niriss_pars-image2pipeline_ld.tpn'), ('mapping', 'REFERENCE'), ('name', "*

 * *             "'jwst_niriss_pars-image2pipeline.rmap'), ('observatory', 'JWST'), ('parkey', "*

 * *             "[['META.EXPOSURE.TYPE'], ['META.O […]*

```diff
@@ -2597,14 +2597,40 @@
             ],
             "sha1sum": "5ecad4ace0d22f271aad88f0138bfb0e43c3e4a7",
             "suffix": "mask",
             "text_descr": "Bad Pixel Mask",
             "tpn": "niriss_mask.tpn",
             "unique_rowkeys": null
         },
+        "pars-image2pipeline": {
+            "derived_from": "Hand made 2020-08-18",
+            "extra_keys": null,
+            "file_ext": ".asdf",
+            "filekind": "pars-image2pipeline",
+            "filetype": "PARS-IMAGE2PIPELINE",
+            "instrument": "NIRISS",
+            "ld_tpn": "niriss_pars-image2pipeline_ld.tpn",
+            "mapping": "REFERENCE",
+            "name": "jwst_niriss_pars-image2pipeline.rmap",
+            "observatory": "JWST",
+            "parkey": [
+                [
+                    "META.EXPOSURE.TYPE"
+                ],
+                [
+                    "META.OBSERVATION.DATE",
+                    "META.OBSERVATION.TIME"
+                ]
+            ],
+            "sha1sum": "36566118852d56882dc425fe69859233b4656402",
+            "suffix": "pars-image2pipeline",
+            "text_descr": "Image2Pipeline runtime parameters",
+            "tpn": "niriss_pars-image2pipeline.tpn",
+            "unique_rowkeys": null
+        },
         "pathloss": {
             "classes": [
                 "Match",
                 "UseAfter"
             ],
             "derived_from": "Hand made 2016-10-20",
             "extra_keys": null,
@@ -3700,14 +3726,42 @@
             },
             "sha1sum": "ed707f0f08e062c6e93838af65f9c7f79b600b18",
             "suffix": "ote",
             "text_descr": "Transform through the Optical Telescope Element",
             "tpn": "nirspec_ote.tpn",
             "unique_rowkeys": null
         },
+        "pars-spec2pipeline": {
+            "derived_from": "Hand made 2020-06-19",
+            "extra_keys": null,
+            "file_ext": ".asdf",
+            "filekind": "pars-spec2pipeline",
+            "filetype": "PARS-SPEC2PIPELINE",
+            "instrument": "NIRSPEC",
+            "ld_tpn": "nirspec_pars-spec2pipeline_ld.tpn",
+            "mapping": "REFERENCE",
+            "name": "jwst_nirspec_pars-spec2pipeline.rmap",
+            "observatory": "JWST",
+            "parkey": [
+                [
+                    "META.EXPOSURE.TYPE",
+                    "META.INSTRUMENT.LAMP_MODE",
+                    "META.INSTRUMENT.LAMP_STATE"
+                ],
+                [
+                    "META.OBSERVATION.DATE",
+                    "META.OBSERVATION.TIME"
+                ]
+            ],
+            "sha1sum": "d4575df2ab497212b01ba3bf09965839d34c79f1",
+            "suffix": "pars-spec2pipeline",
+            "text_descr": "Spec2Pipeline runtime parameters",
+            "tpn": "nirspec_pars-spec2pipeline.tpn",
+            "unique_rowkeys": null
+        },
         "pathloss": {
             "classes": [
                 "Match",
                 "UseAfter"
             ],
             "derived_from": "Hand made 2016-10-20",
             "extra_keys": null,
```

### Comparing `crds-7.5.0.0/crds/jwst/specs/fgs_abvegaoffset.rmap` & `crds-7.6.0/crds/jwst/specs/fgs_abvegaoffset.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/fgs_apcorr.rmap` & `crds-7.6.0/crds/jwst/specs/fgs_apcorr.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/fgs_distortion.rmap` & `crds-7.6.0/crds/jwst/specs/fgs_distortion.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/miri_abvegaoffset.rmap` & `crds-7.6.0/crds/jwst/specs/miri_abvegaoffset.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/miri_apcorr.rmap` & `crds-7.6.0/crds/jwst/specs/miri_apcorr.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/miri_cubepar.rmap` & `crds-7.6.0/crds/jwst/specs/miri_cubepar.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/miri_distortion.spec` & `crds-7.6.0/crds/jwst/specs/miri_distortion.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/miri_extract1d.rmap` & `crds-7.6.0/crds/jwst/specs/miri_extract1d.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/miri_filteroffset.rmap` & `crds-7.6.0/crds/jwst/specs/miri_filteroffset.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/miri_flat.spec` & `crds-7.6.0/crds/jwst/specs/miri_flat.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/miri_pathloss.rmap` & `crds-7.6.0/crds/jwst/specs/miri_pathloss.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/miri_persat.rmap` & `crds-7.6.0/crds/jwst/specs/miri_persat.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/miri_photom.spec` & `crds-7.6.0/crds/jwst/specs/miri_photom.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/miri_psfmask.rmap` & `crds-7.6.0/crds/jwst/specs/miri_psfmask.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/miri_regions.spec` & `crds-7.6.0/crds/jwst/specs/miri_regions.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/miri_reset.rmap` & `crds-7.6.0/crds/jwst/specs/miri_reset.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/miri_resol.rmap` & `crds-7.6.0/crds/jwst/specs/miri_resol.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/miri_rscd.rmap` & `crds-7.6.0/crds/jwst/specs/miri_rscd.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/miri_specwcs.spec` & `crds-7.6.0/crds/jwst/specs/miri_specwcs.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/miri_trapdensity.rmap` & `crds-7.6.0/crds/jwst/specs/miri_trapdensity.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/miri_trappars.rmap` & `crds-7.6.0/crds/jwst/specs/miri_trappars.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/miri_tsophot.rmap` & `crds-7.6.0/crds/jwst/specs/miri_tsophot.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/miri_v2v3.rmap` & `crds-7.6.0/crds/jwst/specs/miri_v2v3.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/miri_wavelengthrange.rmap` & `crds-7.6.0/crds/jwst/specs/miri_wavelengthrange.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/miri_wcsregions.spec` & `crds-7.6.0/crds/jwst/specs/miri_wcsregions.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nircam_abvegaoffset.rmap` & `crds-7.6.0/crds/jwst/specs/nircam_abvegaoffset.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nircam_amplifier.spec` & `crds-7.6.0/crds/jwst/specs/nircam_amplifier.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nircam_apcorr.rmap` & `crds-7.6.0/crds/jwst/specs/nircam_apcorr.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nircam_distortion.rmap` & `crds-7.6.0/crds/jwst/specs/nircam_distortion.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nircam_filteroffset.rmap` & `crds-7.6.0/crds/jwst/specs/nircam_filteroffset.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nircam_photom.spec` & `crds-7.6.0/crds/jwst/specs/nircam_photom.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nircam_psfmask.rmap` & `crds-7.6.0/crds/jwst/specs/nircam_psfmask.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nircam_specwcs.rmap` & `crds-7.6.0/crds/jwst/specs/nircam_specwcs.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nircam_superbias.rmap` & `crds-7.6.0/crds/jwst/specs/nircam_superbias.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nircam_tsophot.rmap` & `crds-7.6.0/crds/jwst/specs/nircam_tsophot.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nircam_wavelengthrange.rmap` & `crds-7.6.0/crds/jwst/specs/nircam_wavelengthrange.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nircam_wfssbkg.rmap` & `crds-7.6.0/crds/jwst/specs/nircam_wfssbkg.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/niriss_abvegaoffset.rmap` & `crds-7.6.0/crds/jwst/specs/niriss_abvegaoffset.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/niriss_amplifier.spec` & `crds-7.6.0/crds/jwst/specs/niriss_amplifier.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/niriss_apcorr.rmap` & `crds-7.6.0/crds/jwst/specs/niriss_apcorr.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/niriss_distortion.rmap` & `crds-7.6.0/crds/jwst/specs/niriss_distortion.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/niriss_extract1d.rmap` & `crds-7.6.0/crds/jwst/specs/niriss_extract1d.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/niriss_pathloss.rmap` & `crds-7.6.0/crds/jwst/specs/niriss_pathloss.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/niriss_photom.spec` & `crds-7.6.0/crds/jwst/specs/niriss_photom.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/niriss_specwcs.rmap` & `crds-7.6.0/crds/jwst/specs/niriss_specwcs.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/niriss_superbias.rmap` & `crds-7.6.0/crds/jwst/specs/niriss_superbias.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/niriss_throughput.rmap` & `crds-7.6.0/crds/jwst/specs/niriss_throughput.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/niriss_wavelengthrange.rmap` & `crds-7.6.0/crds/jwst/specs/niriss_wavelengthrange.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/niriss_wfssbkg.rmap` & `crds-7.6.0/crds/jwst/specs/niriss_wfssbkg.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_amplifier.spec` & `crds-7.6.0/crds/jwst/specs/nirspec_amplifier.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_apcorr.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_apcorr.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_area.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_area.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_badshutter.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_badshutter.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_barshadow.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_barshadow.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_camera.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_camera.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_collimator.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_collimator.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_cubepar.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_cubepar.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_dflat.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_dflat.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_disperser.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_disperser.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_distortion.spec` & `crds-7.6.0/crds/jwst/specs/nirspec_distortion.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_extract1d.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_extract1d.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_fflat.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_fflat.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_flat.spec` & `crds-7.6.0/crds/jwst/specs/nirspec_flat.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_fore.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_fore.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_fpa.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_fpa.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_ifufore.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_ifufore.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_ifupost.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_ifupost.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_ifuslicer.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_ifuslicer.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_msa.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_msa.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_msaoper.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_msaoper.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_ote.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_ote.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_pathloss.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_pathloss.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_photom.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_photom.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_refpix.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_refpix.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_regions.spec` & `crds-7.6.0/crds/jwst/specs/nirspec_regions.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_sflat.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_sflat.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_specwcs.spec` & `crds-7.6.0/crds/jwst/specs/nirspec_specwcs.spec`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_superbias.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_superbias.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_wavecorr.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_wavecorr.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/nirspec_wavelengthrange.rmap` & `crds-7.6.0/crds/jwst/specs/nirspec_wavelengthrange.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/system_calver.rmap` & `crds-7.6.0/crds/jwst/specs/system_calver.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/system_crdscfg.rmap` & `crds-7.6.0/crds/jwst/specs/system_crdscfg.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/specs/system_datalvl.rmap` & `crds-7.6.0/crds/jwst/specs/system_datalvl.rmap`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/all_all.tpn` & `crds-7.6.0/crds/jwst/tpns/all_all.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/all_all_ld.tpn` & `crds-7.6.0/crds/jwst/tpns/all_all_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/all_dark.tpn` & `crds-7.6.0/crds/jwst/tpns/all_dark_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/all_trappars.tpn` & `crds-7.6.0/crds/jwst/tpns/all_trappars.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/fgs_all.tpn` & `crds-7.6.0/crds/jwst/tpns/fgs_all.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/fgs_all_ld.tpn` & `crds-7.6.0/crds/jwst/tpns/fgs_all_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/fgs_apcorr.tpn` & `crds-7.6.0/crds/jwst/tpns/fgs_apcorr.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/fgs_dark.tpn` & `crds-7.6.0/crds/jwst/tpns/fgs_dark.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/includes/apcorr.tpn` & `crds-7.6.0/crds/jwst/tpns/includes/apcorr.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/includes/miri_dq_array.tpn` & `crds-7.6.0/crds/jwst/tpns/includes/miri_dq_array.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/includes/miri_dq_def_array.tpn` & `crds-7.6.0/crds/jwst/tpns/includes/miri_dq_def_array.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/includes/miri_sci_array_both.tpn` & `crds-7.6.0/crds/jwst/tpns/includes/miri_sci_array_both.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/includes/miri_subarray_both.tpn` & `crds-7.6.0/crds/jwst/tpns/includes/miri_subarray_both.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/includes/nir_dq_def_array.tpn` & `crds-7.6.0/crds/jwst/tpns/includes/nir_dq_def_array.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/includes/nir_opt_err_array.tpn` & `crds-7.6.0/crds/jwst/tpns/includes/nir_opt_err_array.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/includes/nir_photom.tpn` & `crds-7.6.0/crds/jwst/tpns/includes/nir_photom.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/includes/nir_sci_array_both.tpn` & `crds-7.6.0/crds/jwst/tpns/includes/nir_sci_array_both.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/includes/nir_subarray.tpn` & `crds-7.6.0/crds/jwst/tpns/includes/nir_subarray.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/includes/nir_subarray_baseline.tpn` & `crds-7.6.0/crds/jwst/tpns/includes/nir_subarray_baseline.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/includes/nirspec_dq_array.tpn` & `crds-7.6.0/crds/jwst/tpns/includes/nirspec_dq_array.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/includes/nirspec_err_array.tpn` & `crds-7.6.0/crds/jwst/tpns/includes/nirspec_err_array.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/includes/nirspec_opt_err_array.tpn` & `crds-7.6.0/crds/jwst/tpns/includes/nirspec_opt_err_array.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/includes/nirspec_sci_array_both.tpn` & `crds-7.6.0/crds/jwst/tpns/includes/nirspec_sci_array_both.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/includes/nirspec_sci_array_striped.tpn` & `crds-7.6.0/crds/jwst/tpns/includes/nirspec_sci_array_striped.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/includes/nirspec_subarray_baseline.tpn` & `crds-7.6.0/crds/jwst/tpns/includes/nirspec_subarray_baseline.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/miri_all.tpn` & `crds-7.6.0/crds/jwst/tpns/miri_all.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/miri_all_ld.tpn` & `crds-7.6.0/crds/jwst/tpns/miri_all_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/miri_linearity.tpn` & `crds-7.6.0/crds/jwst/tpns/miri_linearity.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/miri_rscd.tpn` & `crds-7.6.0/crds/jwst/tpns/miri_rscd.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/nircam_all.tpn` & `crds-7.6.0/crds/jwst/tpns/nircam_all.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/nircam_all_ld.tpn` & `crds-7.6.0/crds/jwst/tpns/nircam_all_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/nircam_apcorr.tpn` & `crds-7.6.0/crds/jwst/tpns/nircam_apcorr.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/niriss_all.tpn` & `crds-7.6.0/crds/jwst/tpns/niriss_all.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/niriss_all_ld.tpn` & `crds-7.6.0/crds/jwst/tpns/niriss_all_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/niriss_apcorr.tpn` & `crds-7.6.0/crds/jwst/tpns/niriss_apcorr.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/nirspec_all.tpn` & `crds-7.6.0/crds/jwst/tpns/nirspec_all.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/nirspec_all_ld.tpn` & `crds-7.6.0/crds/jwst/tpns/nirspec_all_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/nirspec_apcorr.tpn` & `crds-7.6.0/crds/jwst/tpns/nirspec_apcorr.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/nirspec_area.tpn` & `crds-7.6.0/crds/jwst/tpns/nirspec_area.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/nirspec_barshadow.tpn` & `crds-7.6.0/crds/jwst/tpns/nirspec_barshadow.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/nirspec_dflat.tpn` & `crds-7.6.0/crds/jwst/tpns/nirspec_dflat.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/nirspec_fflat.tpn` & `crds-7.6.0/crds/jwst/tpns/nirspec_fflat.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/nirspec_pathloss.tpn` & `crds-7.6.0/crds/jwst/tpns/nirspec_pathloss.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/nirspec_refpix.tpn` & `crds-7.6.0/crds/jwst/tpns/nirspec_refpix.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/jwst/tpns/nirspec_sflat.tpn` & `crds-7.6.0/crds/jwst/tpns/nirspec_sflat.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/list.py` & `crds-7.6.0/crds/list.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/matches.py` & `crds-7.6.0/crds/matches.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/misc/cal_pipelines.py` & `crds-7.6.0/crds/misc/cal_pipelines.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/misc/check_archive.py` & `crds-7.6.0/crds/misc/check_archive.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/misc/datalvl.py` & `crds-7.6.0/crds/misc/datalvl.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/misc/get_synphot.py` & `crds-7.6.0/crds/misc/get_synphot.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
         references  = rmap.reference_names()
         assert len(references) == 1, \
             "More than one '%s' reference name mentioned in '%s'." % \
             (synname, rmap.name)
         tab_name = references[0]
 
         # rmap object locate() not module function.
-        tab_path = config.locate_file(tab_name)
+        tab_path = rmap.locate_file(tab_name)
 
         # CRDS abstract table object nominally from HDU 1
         table = tables.tables(tab_path)[0]
 
         fileinfo = {}
         for syn_name in table.columns["FILENAME"]:
```

### Comparing `crds-7.5.0.0/crds/misc/query_affected.py` & `crds-7.6.0/crds/misc/query_affected.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/misc/sql.py` & `crds-7.6.0/crds/misc/sql.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/misc/uniqname.py` & `crds-7.6.0/crds/misc/uniqname.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/refactoring/checksum.py` & `crds-7.6.0/crds/refactoring/checksum.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/refactoring/newcontext.py` & `crds-7.6.0/crds/refactoring/newcontext.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/refactoring/refactor.py` & `crds-7.6.0/crds/refactoring/refactor.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/refactoring/refactor2.py` & `crds-7.6.0/crds/refactoring/refactor2.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/rowdiff.py` & `crds-7.6.0/crds/rowdiff.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/submit/background.py` & `crds-7.6.0/crds/submit/background.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/submit/monitor.py` & `crds-7.6.0/crds/submit/monitor.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/submit/rc_submit.py` & `crds-7.6.0/crds/submit/rc_submit.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/submit/submit.py` & `crds-7.6.0/crds/submit/submit.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/submit/web.py` & `crds-7.6.0/crds/submit/web.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/sync.py` & `crds-7.6.0/crds/sync.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/compare_pickles.py` & `crds-7.6.0/crds/tests/compare_pickles.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/profile_bestrefs.py` & `crds-7.6.0/crds/tests/profile_bestrefs.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/profile_pickling.py` & `crds-7.6.0/crds/tests/profile_pickling.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_bad_files.py` & `crds-7.6.0/crds/tests/test_bad_files.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_bestrefs.py` & `crds-7.6.0/crds/tests/test_bestrefs.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_build6.py` & `crds-7.6.0/crds/tests/test_build6.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_certify.py` & `crds-7.6.0/crds/tests/test_certify.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import doctest
 from pprint import pprint as pp
 
 # ==================================================================================
 import numpy as np
 
-from nose.tools import assert_raises, assert_true
+from nose.tools import assert_raises, assert_true, assert_false
 
 # ==================================================================================
 
 from crds.core import utils, log, exceptions
 from crds import client
 from crds import data_file
 from crds import certify
@@ -247,15 +247,15 @@
 """
 
 def certify_interpret_fitsverify():
     """
     >>> doctest.ELLIPSIS_MARKER = '-ignore-'
     >>> old_state = test_config.setup(url="https://jwst-serverless-mode.stsci.edu")
 
-    >>> certify.interpret_fitsverify_output(1, INTERPRET_FITSVERIFY)  # doctest: +ELLIPSIS
+    >>> certify.certify.interpret_fitsverify_output(1, INTERPRET_FITSVERIFY)  # doctest: +ELLIPSIS
     CRDS - INFO -  >>
     CRDS - INFO -  >> Running fitsverify.
     CRDS - INFO -  >>
     CRDS - INFO -  >>               fitsverify -ignore- (CFITSIO -ignore-)
     CRDS - INFO -  >>               --------------------------------
     CRDS - INFO -  >>
     CRDS - INFO -  >>
@@ -289,15 +289,15 @@
     CRDS - INFO -  >>  1                          Primary Array    0         0
     CRDS - INFO -  >>  2                          Binary Table     2         1
     CRDS - INFO -  >>
     CRDS - INFO -  >> Verification found 2 warning(s) and 0 error(s). ****
     CRDS - INFO -  Fitsverify returned a NONZERO COMMAND LINE ERROR STATUS.
     CRDS - ERROR -  Fitsverify output contains errors or warnings CRDS recategorizes as ERRORs.
 
-    >>> certify.interpret_fitsverify_output(1, INTERPRET_FITSVERIFY2)  # doctest: +ELLIPSIS
+    >>> certify.certify.interpret_fitsverify_output(1, INTERPRET_FITSVERIFY2)  # doctest: +ELLIPSIS
     CRDS - INFO -  >>
     CRDS - INFO -  >>               fitsverify -ignore- (CFITSIO -ignore-)
     CRDS - INFO -  >>               --------------------------------
     CRDS - INFO -  >>
     CRDS - INFO -  >>
     CRDS - INFO -  >> File: jwst_nircam_photom_nrcalong.fits
     CRDS - INFO -  >>
@@ -340,15 +340,15 @@
     CRDS - INFO -  >>  2     PHOTOM (1)           Binary Table     0         0
     CRDS - INFO -  >>  3     ASDF                 Image Array      0         1
     CRDS - INFO -  >>
     CRDS - INFO -  >> **** Verification found 0 warning(s) and 1 error(s). ****
     CRDS - INFO -  Fitsverify returned a NONZERO COMMAND LINE ERROR STATUS.
     CRDS - INFO -  Fitsverify output contains errors or warnings CRDS recategorizes as INFOs.
 
-    >>> certify.interpret_fitsverify_output(0, "")
+    >>> certify.certify.interpret_fitsverify_output(0, "")
 
     >>> test_config.cleanup(old_state)
     >>> doctest.ELLIPSIS_MARKER = '...'
     """
 
 def certify_dump_provenance_fits():
     """
@@ -709,15 +709,15 @@
     >>> generic_tpn.load_all_type_constraints("hst")
     >>> test_config.cleanup(old_state)
     """
 
 def certify_validator_bad_presence_condition():
     """
     >>> old_state = test_config.setup(url="https://hst-crds-serverless.stsci.edu", observatory="hst")
-    >>> info = certify.TpnInfo('DETECTOR','H','C', '(Q='BAR')', ('WFC','HRC','SBC'))
+    >>> info = generic_tpn.TpnInfo('DETECTOR','H','C', '(Q='BAR')', ('WFC','HRC','SBC'))
     Traceback (most recent call last):
     ...
     SyntaxError: invalid syntax
     >>> test_config.cleanup(old_state)
     """
 
 def certify_JsonCertify_valid():
@@ -822,28 +822,28 @@
     CRDS - INFO -  Adding checksum for 'data/hst_cos_tdstab_duplicate.rmap'
     CRDS - ERROR -  Duplicate entry at selector ('FUV', 'SPECTROSCOPIC') = UseAfter vs. UseAfter
     >>> test_config.cleanup(old_state)
     """
 
 def undefined_expr_identifiers():
     """Some TpnInfos include Python expressions either to make them apply conditionally or to
-    implement and expression constraint.   validators.expr_identifiers() scans a Tpn header
+    implement and expression constraint.   validators.core.expr_identifiers() scans a Tpn header
     expression for the header keywords upon which it depends.   This enables CRDS To short
     circuit checks for which critical keywords are not defined at all.
 
-    >>> validators.expr_identifiers("((EXP_TYPE)in(['NRS_MSASPEC','NRS_FIXEDSLIT','NRS_BRIGHTOBJ','NRS_IFU']))")
+    >>> validators.core.expr_identifiers("((EXP_TYPE)in(['NRS_MSASPEC','NRS_FIXEDSLIT','NRS_BRIGHTOBJ','NRS_IFU']))")
     ['EXP_TYPE']
 
-    >>> validators.expr_identifiers("nir_filter(INSTRUME,REFTYPE,EXP_TYPE)")
+    >>> validators.core.expr_identifiers("nir_filter(INSTRUME,REFTYPE,EXP_TYPE)")
     ['INSTRUME', 'REFTYPE', 'EXP_TYPE']
 
-    >>> validators.expr_identifiers("(len(SCI_ARRAY.SHAPE)==2)")
+    >>> validators.core.expr_identifiers("(len(SCI_ARRAY.SHAPE)==2)")
     ['SCI_ARRAY']
 
-    >>> validators.expr_identifiers("(True)")
+    >>> validators.core.expr_identifiers("(True)")
     []
     """
 
 def load_nirspec_staturation_tpn_lines():
     """Print out the outcome of various .tpn directives like "replace" and
     "include" and reuse of generic files.
 
@@ -1305,651 +1305,726 @@
     def tearDown(self, *args, **keys):
         super(TestCertify, self).tearDown(*args, **keys)
         log.set_exception_trap(self._old_debug)
 
     # ------------------------------------------------------------------------------
 
     def test_validator_bad_presence(self):
-        tinfo = certify.TpnInfo('DETECTOR','H','C','Q', ('WFC','HRC','SBC'))
-        assert_raises(ValueError, certify.validator, tinfo)
+        tinfo = generic_tpn.TpnInfo('DETECTOR','H','C','Q', ('WFC','HRC','SBC'))
+        assert_raises(ValueError, validators.validator, tinfo)
 
     def test_validator_bad_keytype(self):
-        tinfo = certify.TpnInfo('DETECTOR','Q','C','R', ('WFC','HRC','SBC'))
-        assert_raises(ValueError, certify.validator, tinfo)
+        tinfo = generic_tpn.TpnInfo('DETECTOR','Q','C','R', ('WFC','HRC','SBC'))
+        assert_raises(ValueError, validators.validator, tinfo)
 
     def test_character_validator_file_good(self):
-        tinfo = certify.TpnInfo('DETECTOR','H','C','R', ('WFC','HRC','SBC'))
-        cval = certify.validator(tinfo)
-        assert_true(isinstance(cval, certify.CharacterValidator))
+        tinfo = generic_tpn.TpnInfo('DETECTOR','H','C','R', ('WFC','HRC','SBC'))
+        cval = validators.validator(tinfo)
+        assert_true(isinstance(cval, validators.core.CharacterValidator))
         header = {"DETECTOR": "HRC"}
         cval.check(self.data('acs_new_idc.fits'), header)
 
     def test_character_validator_bad(self):
-        tinfo = certify.TpnInfo('DETECTOR','H','C','R', ('WFC','HRC','SBC'))
-        cval = certify.validator(tinfo)
-        assert_true(isinstance(cval, certify.CharacterValidator))
+        tinfo = generic_tpn.TpnInfo('DETECTOR','H','C','R', ('WFC','HRC','SBC'))
+        cval = validators.validator(tinfo)
+        assert_true(isinstance(cval, validators.core.CharacterValidator))
         header = {"DETECTOR" : "WFD" }
         assert_raises(ValueError, cval.check, "foo.fits", header)
 
     def test_character_validator_missing_required(self):
-        tinfo = certify.TpnInfo('DETECTOR','H','C','R', ('WFC','HRC','SBC'))
-        cval = certify.validator(tinfo)
-        assert_true(isinstance(cval, certify.CharacterValidator))
+        tinfo = generic_tpn.TpnInfo('DETECTOR','H','C','R', ('WFC','HRC','SBC'))
+        cval = validators.validator(tinfo)
+        assert_true(isinstance(cval, validators.core.CharacterValidator))
         header = {"DETECTOR" : "WFD" }
         assert_raises(ValueError, cval.check, "foo.fits", header)
 
     def test_character_validator_optional_bad(self):
-        tinfo = certify.TpnInfo('DETECTOR','H','C','O', ('WFC','HRC','SBC'))
-        cval = certify.validator(tinfo)
-        assert_true(isinstance(cval, certify.CharacterValidator))
+        tinfo = generic_tpn.TpnInfo('DETECTOR','H','C','O', ('WFC','HRC','SBC'))
+        cval = validators.validator(tinfo)
+        assert_true(isinstance(cval, validators.core.CharacterValidator))
         header = {"DETECTOR" : "WFD" }
         assert_raises(ValueError, cval.check, "foo.fits", header)
 
     def test_character_validator_optional_missing(self):
-        tinfo = certify.TpnInfo('DETECTOR','H','C','O', ('WFC','HRC','SBC'))
-        cval = certify.validator(tinfo)
-        assert_true(isinstance(cval, certify.CharacterValidator))
+        tinfo = generic_tpn.TpnInfo('DETECTOR','H','C','O', ('WFC','HRC','SBC'))
+        cval = validators.validator(tinfo)
+        assert_true(isinstance(cval, validators.core.CharacterValidator))
         header = {"DETECTR" : "WFC" }
         cval.check("foo.fits", header)
 
     # ------------------------------------------------------------------------------
 
     def test_logical_validator_good(self):
-        tinfo = certify.TpnInfo('ROKIN','H','L','R',())
-        cval = certify.validator(tinfo)
-        assert_true(isinstance(cval, certify.LogicalValidator))
+        tinfo = generic_tpn.TpnInfo('ROKIN','H','L','R',())
+        cval = validators.validator(tinfo)
+        assert_true(isinstance(cval, validators.core.LogicalValidator))
         header= {"ROKIN": "F"}
         cval.check("foo.fits", header)
         header= {"ROKIN": "T"}
         cval.check("foo.fits", header)
 
     def test_logical_validator_bad(self):
-        tinfo = certify.TpnInfo('ROKIN','H','L','R',())
-        cval = certify.validator(tinfo)
-        assert_true(isinstance(cval, certify.LogicalValidator))
+        tinfo = generic_tpn.TpnInfo('ROKIN','H','L','R',())
+        cval = validators.validator(tinfo)
+        assert_true(isinstance(cval, validators.core.LogicalValidator))
         header = {"ROKIN" : "True"}
         assert_raises(ValueError, cval.check, "foo.fits", header)
         header = {"ROKIN" : "False"}
         assert_raises(ValueError, cval.check, "foo.fits", header)
         header = {"ROKIN" : "1"}
         assert_raises(ValueError, cval.check, "foo.fits", header)
         header = {"ROKIN" : "0"}
         assert_raises(ValueError, cval.check, "foo.fits", header)
 
     # ------------------------------------------------------------------------------
 
     def test_integer_validator_bad_format(self):
-        info = certify.TpnInfo('READPATT', 'H', 'I', 'R', ('FOO',))
-        assert_raises(ValueError, certify.validator, info)
-        info = certify.TpnInfo('READPATT', 'H', 'I', 'R', ('1.0','2.0'))
-        assert_raises(ValueError, certify.validator, info)
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'I', 'R', ('FOO',))
+        assert_raises(ValueError, validators.validator, info)
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'I', 'R', ('1.0','2.0'))
+        assert_raises(ValueError, validators.validator, info)
 
     def test_integer_validator_bad_float(self):
-        info = certify.TpnInfo('READPATT', 'H', 'I', 'R', ('1','2'))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.IntValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'I', 'R', ('1','2'))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.IntValidator))
         header = {"READPATT": "1.9"}
         assert_raises(ValueError, cval.check, "foo.fits", header)
 
     def test_integer_validator_bad_value(self):
-        info = certify.TpnInfo('READPATT', 'H', 'I', 'R', ('1','2','3'))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.IntValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'I', 'R', ('1','2','3'))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.IntValidator))
         header = {"READPATT": "4"}
         assert_raises(ValueError, cval.check, "foo.fits", header)
 
     def test_integer_validator_good(self):
-        info = certify.TpnInfo('READPATT', 'H', 'I', 'R', ('1','2','3'))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.IntValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'I', 'R', ('1','2','3'))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.IntValidator))
         header = {"READPATT": "2"}
         cval.check("foo.fits", header)
 
     def test_integer_validator_range_good(self):
-        info = certify.TpnInfo('READPATT', 'H', 'I', 'R', ("1:40",))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.IntValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'I', 'R', ("1:40",))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.IntValidator))
         header = {"READPATT": "39"}
         cval.check("foo.fits", header)
 
     def test_integer_validator_range_bad(self):
-        info = certify.TpnInfo('READPATT', 'H', 'I', 'R', ("1:40",))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.IntValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'I', 'R', ("1:40",))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.IntValidator))
         header = {"READPATT": "41"}
         assert_raises(ValueError, cval.check, "foo.fits", header)
 
     def test_integer_validator_range_boundary_good(self):
-        info = certify.TpnInfo('READPATT', 'H', 'I', 'R', ("1:40",))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.IntValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'I', 'R', ("1:40",))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.IntValidator))
         header = {"READPATT": "40"}
         cval.check("foo.fits", header)
 
     def test_integer_validator_range_format_bad(self):
-        info = certify.TpnInfo('READPATT', 'H', 'I', 'R', ("1:40",))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.IntValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'I', 'R', ("1:40",))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.IntValidator))
         header = {"READPATT": "40.3"}
         assert_raises(ValueError, cval.check, "foo.fits", header)
-        info = certify.TpnInfo('READPATT', 'H', 'I', 'R', ("x:40",))
-        assert_raises(ValueError, certify.validator, info)
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'I', 'R', ("x:40",))
+        assert_raises(ValueError, validators.validator, info)
 
     # ------------------------------------------------------------------------------
 
     def test_real_validator_bad_format(self):
-        info = certify.TpnInfo('READPATT', 'H', 'R', 'R', ('FOO',))
-        assert_raises(ValueError, certify.validator, info)
-        info = certify.TpnInfo('READPATT', 'H', 'R', 'R', ('x.0','2.0'))
-        assert_raises(ValueError, certify.validator, info)
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'R', 'R', ('FOO',))
+        assert_raises(ValueError, validators.validator, info)
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'R', 'R', ('x.0','2.0'))
+        assert_raises(ValueError, validators.validator, info)
 
     def test_real_validator_bad_value(self):
-        info = certify.TpnInfo('READPATT', 'H', 'R', 'R', ('1.1','2.2','3.3'))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.RealValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'R', 'R', ('1.1','2.2','3.3'))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.RealValidator))
         header = {"READPATT": "3.2"}
         assert_raises(ValueError, cval.check, "foo.fits", header)
 
     def test_real_validator_good(self):
-        info = certify.TpnInfo('READPATT', 'H', 'R', 'R', ('1.0','2.1','3.0'))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.RealValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'R', 'R', ('1.0','2.1','3.0'))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.RealValidator))
         header = {"READPATT": "2.1"}
         cval.check("foo.fits", header)
 
     def test_real_validator_range_good(self):
-        info = certify.TpnInfo('READPATT', 'H', 'R', 'R', ("1.5:40.2",))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.RealValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'R', 'R', ("1.5:40.2",))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.RealValidator))
         header = {"READPATT": "40.1"}
         cval.check("foo.fits", header)
 
     def test_real_validator_range_bad(self):
-        info = certify.TpnInfo('READPATT', 'H', 'R', 'R', ("1.5:40.2",))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.RealValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'R', 'R', ("1.5:40.2",))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.RealValidator))
         header = {"READPATT": "40.21"}
         assert_raises(ValueError, cval.check, "foo.fits", header)
 
     def test_real_validator_range_boundary_good(self):
-        info = certify.TpnInfo('READPATT', 'H', 'R', 'R', ("1.4:40.1",))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.RealValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'R', 'R', ("1.4:40.1",))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.RealValidator))
         header = {"READPATT": "40.1"}
         cval.check("foo.fits", header)
 
     def test_real_validator_range_format_bad(self):
-        info = certify.TpnInfo('READPATT', 'H', 'R', 'R', ("1.5:40.2",))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.RealValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'R', 'R', ("1.5:40.2",))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.RealValidator))
         header = {"READPATT": "40.x"}
         assert_raises(ValueError, cval.check, "foo.fits", header)
-        info = certify.TpnInfo('READPATT', 'H', 'R', 'R', ("1.x:40.2",))
-        assert_raises(ValueError, certify.validator, info)
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'R', 'R', ("1.x:40.2",))
+        assert_raises(ValueError, validators.validator, info)
 
     def test_real_validator_float_zero(self):
-        info = certify.TpnInfo('READPATT', 'H', 'R', 'R', ('1','0.0'))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.RealValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'R', 'R', ('1','0.0'))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.RealValidator))
         header = {"READPATT": "0.0001"}
         assert_raises(ValueError, cval.check, "foo.fits", header)
 
     def test_real_validator_float_zero_zero(self):
-        info = certify.TpnInfo('READPATT', 'H', 'R', 'R', ('1','0.0'))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.RealValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'R', 'R', ('1','0.0'))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.RealValidator))
         header = {"READPATT": "0.0003"}
         assert_raises(ValueError, cval.check, "foo.fits", header)
 
     def test_real_validator_range_inf_good(self):
-        info = certify.TpnInfo('READPATT', 'H', 'R', 'R', ("5.5:inf",))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.RealValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'R', 'R', ("5.5:inf",))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.RealValidator))
         header = {"READPATT": "100000.0"}
         cval.check("foo.fits", header)
 
     def test_real_validator_range_inf_bad(self):
-        info = certify.TpnInfo('READPATT', 'H', 'R', 'R', ("5.5:inf",))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.RealValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'R', 'R', ("5.5:inf",))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.RealValidator))
         header = {"READPATT": "5.4"}
         assert_raises(ValueError, cval.check, "foo.fits", header)
 
     # ------------------------------------------------------------------------------
 
     def test_double_validator_bad_format(self):
-        info = certify.TpnInfo('READPATT', 'H', 'D', 'R', ('FOO',))
-        assert_raises(ValueError, certify.validator, info)
-        info = certify.TpnInfo('READPATT', 'H', 'D', 'R', ('x.0','2.0'))
-        assert_raises(ValueError, certify.validator, info)
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'D', 'R', ('FOO',))
+        assert_raises(ValueError, validators.validator, info)
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'D', 'R', ('x.0','2.0'))
+        assert_raises(ValueError, validators.validator, info)
 
     def test_double_validator_bad_value(self):
-        info = certify.TpnInfo('READPATT', 'H', 'D', 'R', ('1.1','2.2','3.3'))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.DoubleValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'D', 'R', ('1.1','2.2','3.3'))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.DoubleValidator))
         header = {"READPATT": "3.2"}
         assert_raises(ValueError, cval.check, "foo.fits", header)
 
     def test_double_validator_good(self):
-        info = certify.TpnInfo('READPATT', 'H', 'D', 'R', ('1.0','2.1','3.0'))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.DoubleValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'D', 'R', ('1.0','2.1','3.0'))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.DoubleValidator))
         header = {"READPATT": "2.1"}
         cval.check("foo.fits", header)
 
     def test_double_validator_range_good(self):
-        info = certify.TpnInfo('READPATT', 'H', 'D', 'R', ("1.5:40.2",))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.DoubleValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'D', 'R', ("1.5:40.2",))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.DoubleValidator))
         header = {"READPATT": "40.1"}
         cval.check("foo.fits", header)
 
     def test_double_validator_range_bad(self):
-        info = certify.TpnInfo('READPATT', 'H', 'D', 'R', ("1.5:40.2",))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.DoubleValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'D', 'R', ("1.5:40.2",))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.DoubleValidator))
         header = {"READPATT": "40.21"}
         assert_raises(ValueError, cval.check, "foo.fits", header)
 
     def test_double_validator_range_boundary_good(self):
-        info = certify.TpnInfo('READPATT', 'H', 'D', 'R', ("1.4:40.1",))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.DoubleValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'D', 'R', ("1.4:40.1",))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.DoubleValidator))
         header = {"READPATT": "40.1"}
         cval.check("foo.fits", header)
 
     def test_double_validator_range_format_bad(self):
-        info = certify.TpnInfo('READPATT', 'H', 'D', 'R', ("1.5:40.2",))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.DoubleValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'D', 'R', ("1.5:40.2",))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.DoubleValidator))
         header = {"READPATT": "40.x"}
         assert_raises(ValueError, cval.check, "foo.fits", header)
-        info = certify.TpnInfo('READPATT', 'H', 'D', 'R', ("1.x:40.2",))
-        assert_raises(ValueError, certify.validator, info)
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'D', 'R', ("1.x:40.2",))
+        assert_raises(ValueError, validators.validator, info)
 
     def test_double_validator_range_inf_good(self):
-        info = certify.TpnInfo('READPATT', 'H', 'D', 'R', ("5.5:inf",))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.DoubleValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'D', 'R', ("5.5:inf",))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.DoubleValidator))
         header = {"READPATT": "100000.0"}
         cval.check("foo.fits", header)
 
     def test_double_validator_range_inf_bad(self):
-        info = certify.TpnInfo('READPATT', 'H', 'D', 'R', ("5.5:inf",))
-        cval = certify.validator(info)
-        assert_true(isinstance(cval, certify.DoubleValidator))
+        info = generic_tpn.TpnInfo('READPATT', 'H', 'D', 'R', ("5.5:inf",))
+        cval = validators.validator(info)
+        assert_true(isinstance(cval, validators.core.DoubleValidator))
         header = {"READPATT": "5.4"}
         assert_raises(ValueError, cval.check, "foo.fits", header)
 
     # ------------------------------------------------------------------------------
 
     def test_expression_validator_passes(self):
-        tinfo = certify.TpnInfo('DETECTOR','X','X','R', ('((DETECTOR==\'FOO\')and(SUBARRAY==\'BAR\'))',))
-        cval = certify.validator(tinfo)
-        assert_true(isinstance(cval, certify.ExpressionValidator))
+        tinfo = generic_tpn.TpnInfo('DETECTOR','X','X','R', ('((DETECTOR==\'FOO\')and(SUBARRAY==\'BAR\'))',))
+        cval = validators.validator(tinfo)
+        assert_true(isinstance(cval, validators.core.ExpressionValidator))
         header = { "DETECTOR":"FOO", "SUBARRAY":"BAR" }
         cval.check("foo.fits", header)
 
     def test_expression_validator_fails(self):
-        tinfo = certify.TpnInfo('DETECTOR','X','X','R', ('((DETECTOR=="FOO")and(SUBARRAY=="BAR"))',))
-        cval = certify.validator(tinfo)
-        assert_true(isinstance(cval, certify.ExpressionValidator))
+        tinfo = generic_tpn.TpnInfo('DETECTOR','X','X','R', ('((DETECTOR=="FOO")and(SUBARRAY=="BAR"))',))
+        cval = validators.validator(tinfo)
+        assert_true(isinstance(cval, validators.core.ExpressionValidator))
         header = { "DETECTOR":"FOO", "SUBARRAY":"BA" }
-        assert_raises(certify.RequiredConditionError, cval.check, "foo.fits", header)
+        assert_raises(validators.core.RequiredConditionError, cval.check, "foo.fits", header)
 
     def test_expression_validator_bad_format(self):
         # typical subtle expression error, "=" vs. "=="
-        tinfo = certify.TpnInfo('DETECTOR','X','X','R', ('((DETECTOR="FOO")and(SUBARRAY=="BAR"))',))
-        assert_raises(SyntaxError, certify.validator, tinfo)
+        tinfo = generic_tpn.TpnInfo('DETECTOR','X','X','R', ('((DETECTOR="FOO")and(SUBARRAY=="BAR"))',))
+        assert_raises(SyntaxError, validators.validator, tinfo)
+
+    # ------------------------------------------------------------------------------
+
+    def test_column_expression_validator_passes(self):
+        tinfo = generic_tpn.TpnInfo('DETCHIP', 'C', 'X', 'R', ('(VALUE%2==1)',))
+        cval = validators.validator(tinfo)
+        assert_true(isinstance(cval, validators.core.ColumnExpressionValidator))
+        cval.check(self.data('acs_new_idc.fits'), {})
+
+    def test_column_expression_validator_fails(self):
+        tinfo = generic_tpn.TpnInfo('DETCHIP', 'C', 'X', 'R', ('(VALUE%2==0)',))
+        cval = validators.validator(tinfo)
+        assert_raises(exceptions.RequiredConditionError, cval.check, self.data('acs_new_idc.fits'), {})
+
+    def test_column_expression_validator_header_variable(self):
+        tinfo = generic_tpn.TpnInfo('DETCHIP', 'C', 'X', 'R', ('(DETECTOR=="FOO")',))
+        cval = validators.validator(tinfo)
+        header = { "DETECTOR": "FOO" }
+        assert_raises(exceptions.RequiredConditionError, cval.check, self.data('acs_new_idc.fits'), header)
+
+    # ------------------------------------------------------------------------------
+
+    def test_synphot_graph_validator_passes(self):
+        tinfo = generic_tpn.TpnInfo('EXT1', 'D', 'X', 'R', ('&SYNPHOT_GRAPH',))
+        cval = validators.validator(tinfo)
+        assert_true(isinstance(cval, validators.synphot.SynphotGraphValidator))
+        assert_true(cval.check(self.data('hst_synphot_tmg_connected.fits'), {}))
+
+    def test_synphot_graph_validator_fails(self):
+        tinfo = generic_tpn.TpnInfo('EXT1', 'D', 'X', 'R', ('&SYNPHOT_GRAPH',))
+        cval = validators.validator(tinfo)
+        assert_false(cval.check(self.data('hst_synphot_tmg_disconnected.fits'), {}))
+
+    # ------------------------------------------------------------------------------
+
+    def test_synphot_lookup_validator_passes(self):
+        tinfo = generic_tpn.TpnInfo('EXT1', 'D', 'X', 'R', ('&SYNPHOT_LOOKUP',))
+        cval = validators.validator(tinfo)
+        assert_true(isinstance(cval, validators.synphot.SynphotLookupValidator))
+        assert_true(cval.check(self.data('hst_synphot_tmc_passes.fits'), {}))
+
+    def test_synphot_lookup_validator_fails(self):
+        tinfo = generic_tpn.TpnInfo('EXT1', 'D', 'X', 'R', ('&SYNPHOT_LOOKUP',))
+        cval = validators.validator(tinfo)
+        assert_false(cval.check(self.data('hst_synphot_tmc_bad_filename.fits'), {}))
+
+    # ------------------------------------------------------------------------------
+
+    def test_synphot_throughput_validator_passes(self):
+        tinfo = generic_tpn.TpnInfo('EXT1', 'D', 'X', 'R', ('&SYNPHOT_THROUGHPUT',))
+        cval = validators.validator(tinfo, context="hst_0787.pmap")
+        assert_true(isinstance(cval, validators.synphot.SynphotThroughputValidator))
+        header = { "COMPNAME": "acs_f555w_hrc"}
+        assert_true(cval.check(self.data('acs_f555w_hrc_007_syn.fits'), header))
+
+    def test_synphot_throughput_validator_fails(self):
+        tinfo = generic_tpn.TpnInfo('EXT1', 'D', 'X', 'R', ('&SYNPHOT_THROUGHPUT',))
+        cval = validators.validator(tinfo, context="hst_0787.pmap")
+        header = { "COMPNAME": "acs_f555w_hrc"}
+        assert_false(cval.check(self.data('acs_f555w_hrc_006_syn.fits'), header))
+
+    # ------------------------------------------------------------------------------
+
+    def test_synphot_thermal_validator_passes(self):
+        tinfo = generic_tpn.TpnInfo('EXT1', 'D', 'X', 'R', ('&SYNPHOT_THERMAL',))
+        cval = validators.validator(tinfo, context="hst_0787.pmap")
+        assert_true(isinstance(cval, validators.synphot.SynphotThermalValidator))
+        header = { "COMPNAME": "wfc3_ir_g141_src"}
+        assert_true(cval.check(self.data('wfc3_ir_g141_src_999_th.fits'), header))
+
+    def test_synphot_thermal_validator_fails(self):
+        tinfo = generic_tpn.TpnInfo('EXT1', 'D', 'X', 'R', ('&SYNPHOT_THERMAL',))
+        cval = validators.validator(tinfo, context="hst_0787.pmap")
+        header = { "COMPNAME": "wfc3_ir_g141_src"}
+        assert_false(cval.check(self.data('wfc3_ir_g141_src_003_th.fits'), header))
 
     # ------------------------------------------------------------------------------
 
     def test_conditionally_required_bad_format(self):
         # typical subtle expression error, "=" vs. "=="
-        tinfo = certify.TpnInfo('DETECTOR','X', 'X', '(SUBARRAY="BAR")', ("FOO","BAR","BAZ"))
-        assert_raises(SyntaxError, certify.validator, tinfo)
+        tinfo = generic_tpn.TpnInfo('DETECTOR','X', 'X', '(SUBARRAY="BAR")', ("FOO","BAR","BAZ"))
+        assert_raises(SyntaxError, validators.validator, tinfo)
 
     def test_conditionally_required_good(self):
         # typical subtle expression error, "=" vs. "=="
-        tinfo = certify.TpnInfo('DETECTOR','H', 'C', '(SUBARRAY=="BAR")', ("FOO","BAR","BAZ"))
-        cval = certify.validator(tinfo)
+        tinfo = generic_tpn.TpnInfo('DETECTOR','H', 'C', '(SUBARRAY=="BAR")', ("FOO","BAR","BAZ"))
+        cval = validators.validator(tinfo)
         header = { "DETECTOR" : "FOO", "SUBARRAY":"BAR" }
         cval.check("foo.fits", header)
 
     def test_conditionally_required_bad(self):
         # typical subtle expression error, "=" vs. "=="
-        tinfo = certify.TpnInfo('DETECTOR','H', 'C', '(SUBARRAY=="BAR")', ("FOO","BAR","BAZ"))
-        checker = certify.validator(tinfo)
+        tinfo = generic_tpn.TpnInfo('DETECTOR','H', 'C', '(SUBARRAY=="BAR")', ("FOO","BAR","BAZ"))
+        checker = validators.validator(tinfo)
         header = { "DETECTOR" : "FRODO", "SUBARRAY":"BAR" }
         assert_raises(ValueError, checker.check, "foo.fits", header)
 
     def test_conditionally_not_required(self):
         # typical subtle expression error, "=" vs. "=="
-        tinfo = certify.TpnInfo('DETECTOR','H', 'C', '(SUBARRAY=="BAR")', ("FOO","BAR","BAZ"))
-        checker = certify.validator(tinfo)
+        tinfo = generic_tpn.TpnInfo('DETECTOR','H', 'C', '(SUBARRAY=="BAR")', ("FOO","BAR","BAZ"))
+        checker = validators.validator(tinfo)
         header = { "DETECTOR" : "FRODO", "SUBARRAY":"BAZ" }
         checker.check("foo.fits", header)
 
     def test_not_conditionally_required(self):
         # typical subtle expression error, "=" vs. "=="
-        info = certify.TpnInfo('DETECTOR','H', 'C', 'R', ("FOO","BAR","BAZ"))
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('DETECTOR','H', 'C', 'R', ("FOO","BAR","BAZ"))
+        checker = validators.validator(info)
         assert_true(not checker.conditionally_required)  #
 
     def test_conditional_warning_true_present(self):
-        info = certify.TpnInfo('PIXAR_SR', 'H', 'R', "(warning(not(('MRS')in(EXP_TYPE))))", ())
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PIXAR_SR', 'H', 'R', "(warning(not(('MRS')in(EXP_TYPE))))", ())
+        checker = validators.validator(info)
         assert_true(checker.conditionally_required)
         header = {"EXP_TYPE":"MIR_LRS-FIXEDSLIT", "PIXAR_SR":"999.0"}
         assert_true(checker.is_applicable(header)=='W')  #
         checker.handle_missing(header)
 
     def test_conditional_warning_true_absent(self):
-        info = certify.TpnInfo('PIXAR_SR', 'H', 'R', "(warning(not(('MRS')in(EXP_TYPE))))", ())
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PIXAR_SR', 'H', 'R', "(warning(not(('MRS')in(EXP_TYPE))))", ())
+        checker = validators.validator(info)
         assert_true(checker.conditionally_required)
         header = {"EXP_TYPE":"MIR_LRS-FIXEDSLIT", "PIXAR_SR":"999.0"}
         assert_true(checker.is_applicable(header)=='W')  #
         checker.handle_missing(header)
 
     def test_conditional_warning_false_present(self):
-        info = certify.TpnInfo('PIXAR_SR', 'H', 'R', "(warning(not(('MRS')in(EXP_TYPE))))", ())
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PIXAR_SR', 'H', 'R', "(warning(not(('MRS')in(EXP_TYPE))))", ())
+        checker = validators.validator(info)
         assert_true(checker.conditionally_required)
         header = {"EXP_TYPE":"MIR_FLAT-MRS", "PIXAR_SR":"999.0"}
         assert_true(checker.is_applicable(header)==False)  #
         checker.handle_missing(header)
 
     def test_conditional_warning_false_absent(self):
-        info = certify.TpnInfo('PIXAR_SR', 'H', 'R', "(warning(not(('MRS')in(EXP_TYPE))))", ())
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PIXAR_SR', 'H', 'R', "(warning(not(('MRS')in(EXP_TYPE))))", ())
+        checker = validators.validator(info)
         assert_true(checker.conditionally_required)
         header = {"EXP_TYPE":"MIR_FLAT-MRS"}
         assert_true(checker.is_applicable(header)==False)  #
         checker.handle_missing(header)
 
     def test_conditional_optional_true_present(self):
-        info = certify.TpnInfo('PIXAR_SR', 'H', 'R', "(optional(not(('MRS')in(EXP_TYPE))))", ())
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PIXAR_SR', 'H', 'R', "(optional(not(('MRS')in(EXP_TYPE))))", ())
+        checker = validators.validator(info)
         assert_true(checker.conditionally_required)
         header = {"EXP_TYPE":"MIR_LRS-FIXEDSLIT", "PIXAR_SR":"999.0"}
         assert_true(checker.is_applicable(header)=='O')  #
         checker.handle_missing(header)
 
     def test_conditional_optional_true_absent(self):
-        info = certify.TpnInfo('PIXAR_SR', 'H', 'R', "(optional(not(('MRS')in(EXP_TYPE))))", ())
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PIXAR_SR', 'H', 'R', "(optional(not(('MRS')in(EXP_TYPE))))", ())
+        checker = validators.validator(info)
         assert_true(checker.conditionally_required)
         header = {"EXP_TYPE":"MIR_LRS-FIXEDSLIT"}
         assert_true(checker.is_applicable(header)=='O')  #
         checker.handle_missing(header)
 
     def test_conditional_optional_false_present(self):
-        info = certify.TpnInfo('PIXAR_SR', 'H', 'R', "(optional(not(('MRS')in(EXP_TYPE))))", ())
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PIXAR_SR', 'H', 'R', "(optional(not(('MRS')in(EXP_TYPE))))", ())
+        checker = validators.validator(info)
         assert_true(checker.conditionally_required)
         header = {"EXP_TYPE":"MIR_FLAT-MRS", "PIXAR_SR":"999.0"}
         assert_true(checker.is_applicable(header)==False)  #
         checker.handle_missing(header)
 
     def test_conditional_optional_false_absent(self):
-        info = certify.TpnInfo('PIXAR_SR', 'H', 'R', "(optional(not(('MRS')in(EXP_TYPE))))", ())
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PIXAR_SR', 'H', 'R', "(optional(not(('MRS')in(EXP_TYPE))))", ())
+        checker = validators.validator(info)
         assert_true(checker.conditionally_required)
         header = {"EXP_TYPE":"MIR_FLAT-MRS"}
         assert_true(checker.is_applicable(header)==False)  #
         checker.handle_missing(header)
 
     def test_tpn_bad_presence(self):
         try:
-            certify.TpnInfo('DETECTOR','H', 'C', 'Q', ("FOO","BAR","BAZ"))
+            generic_tpn.TpnInfo('DETECTOR','H', 'C', 'Q', ("FOO","BAR","BAZ"))
         except ValueError as exc:
             assert_true("presence" in str(exc), "Wrong exception for test_tpn_bad_presence")
 
     def test_tpn_bad_group_keytype(self):
-        info = certify.TpnInfo('DETECTOR','G', 'C', 'R', ("FOO","BAR","BAZ"))
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('DETECTOR','G', 'C', 'R', ("FOO","BAR","BAZ"))
+        checker = validators.validator(info)
         warns = log.warnings()
         checker.check("test.fits", {"DETECTOR":"FOO"})
         new_warns = log.warnings()
         assert_true(new_warns - warns >= 1, "No warning issued for unsupported group .tpn constraint type.")
 
     def test_tpn_repr(self):
         # typical subtle expression error, "=" vs. "=="
-        info = certify.TpnInfo('DETECTOR','H', 'C', 'R', ("FOO","BAR","BAZ"))
-        repr(certify.Validator(info))
+        info = generic_tpn.TpnInfo('DETECTOR','H', 'C', 'R', ("FOO","BAR","BAZ"))
+        repr(validators.validator(info))
 
     def test_tpn_check_value_method_not_implemented(self):
         # typical subtle expression error, "=" vs. "=="
-        info = certify.TpnInfo('DETECTOR','H', 'C', 'R', ("FOO","BAR","BAZ"))
-        checker = certify.Validator(info)
+        info = generic_tpn.TpnInfo('DETECTOR','H', 'C', 'R', ("FOO","BAR","BAZ"))
+        checker = validators.core.Validator(info)
         assert_raises(NotImplementedError, checker.check, "test.fits", header={"DETECTOR":"FOO"})
 
     def test_tpn_handle_missing(self):
         # typical subtle expression error, "=" vs. "=="
-        info = certify.TpnInfo('DETECTOR','H', 'C', 'W', ("FOO","BAR","BAZ"))
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('DETECTOR','H', 'C', 'W', ("FOO","BAR","BAZ"))
+        checker = validators.validator(info)
         assert_true(checker.handle_missing(header={"READPATT":"FOO"}) == "UNDEFINED")
-        info = certify.TpnInfo('DETECTOR','H', 'C', 'S', ("FOO","BAR","BAZ"))
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('DETECTOR','H', 'C', 'S', ("FOO","BAR","BAZ"))
+        checker = validators.validator(info)
         assert_true(checker.handle_missing(header={"READPATT":"FOO"}) == "UNDEFINED")
-        info = certify.TpnInfo('DETECTOR','H', 'C', 'F', ("FOO","BAR","BAZ"))
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('DETECTOR','H', 'C', 'F', ("FOO","BAR","BAZ"))
+        checker = validators.validator(info)
         assert_true(checker.handle_missing(header={"READPATT":"FOO"}) == "UNDEFINED")
 
     def test_tpn_handle_missing_conditional(self):
         # typical subtle expression error, "=" vs. "=="
-        info = certify.TpnInfo('DETECTOR','H', 'C', "(READPATT=='FOO')", ("FOO","BAR","BAZ"))
-        checker = certify.validator(info)
-        assert_raises(certify.MissingKeywordError, checker.handle_missing, header={"READPATT":"FOO"})
+        info = generic_tpn.TpnInfo('DETECTOR','H', 'C', "(READPATT=='FOO')", ("FOO","BAR","BAZ"))
+        checker = validators.validator(info)
+        assert_raises(exceptions.MissingKeywordError, checker.handle_missing, header={"READPATT":"FOO"})
         assert_true(checker.handle_missing(header={"READPATT":"BAR"}) == "UNDEFINED")
 
 
     def test_missing_column_validator(self):
-        info = certify.TpnInfo('FOO','C', 'C', 'R', ("X","Y","Z"))
-        checker = certify.validator(info)
-        assert_raises(certify.MissingKeywordError, checker.check, self.data("v8q14451j_idc.fits"),
+        info = generic_tpn.TpnInfo('FOO','C', 'C', 'R', ("X","Y","Z"))
+        checker = validators.validator(info)
+        assert_raises(exceptions.MissingKeywordError, checker.check, self.data("v8q14451j_idc.fits"),
                       header={"DETECTOR":"IRRELEVANT"})
 
     def test_tpn_excluded_keyword(self):
         # typical subtle expression error, "=" vs. "=="
-        info = certify.TpnInfo('DETECTOR','H', 'C', 'E', ())
-        checker = certify.validator(info)
-        assert_raises(certify.IllegalKeywordError, checker.check, "test.fits", {"DETECTOR":"SHOULDNT_DEFINE"})
+        info = generic_tpn.TpnInfo('DETECTOR','H', 'C', 'E', ())
+        checker = validators.validator(info)
+        assert_raises(exceptions.IllegalKeywordError, checker.check, "test.fits", {"DETECTOR":"SHOULDNT_DEFINE"})
 
     def test_tpn_not_value(self):
         # typical subtle expression error, "=" vs. "=="
-        info = certify.TpnInfo('SUBARRAY','H', 'C', 'R', ["NOT_GENERIC"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('SUBARRAY','H', 'C', 'R', ["NOT_GENERIC"])
+        checker = validators.validator(info)
         assert_raises(ValueError, checker.check, "test.fits", {"SUBARRAY":"GENERIC"})
 
     def test_tpn_or_bar_value(self):
         # typical subtle expression error, "=" vs. "=="
-        info = certify.TpnInfo('DETECTOR','H', 'C', 'R', ["THIS","THAT","OTHER"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('DETECTOR','H', 'C', 'R', ["THIS","THAT","OTHER"])
+        checker = validators.validator(info)
         checker.check("test.fits", {"DETECTOR":"THAT|THIS"})
 
-        info = certify.TpnInfo('DETECTOR','H', 'C', 'R', ["THAT","OTHER"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('DETECTOR','H', 'C', 'R', ["THAT","OTHER"])
+        checker = validators.validator(info)
         assert_raises(ValueError, checker.check, "test.fits", {"DETECTOR":"THAT|THIS"})
 
     def test_tpn_esoteric_value(self):
         # typical subtle expression error, "=" vs. "=="
-        info = certify.TpnInfo('DETECTOR','H', 'C', 'R', ["([abc]+)","BETWEEN_300_400","#OTHER#"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('DETECTOR','H', 'C', 'R', ["([abc]+)","BETWEEN_300_400","#OTHER#"])
+        checker = validators.validator(info)
         checker.check("test.fits", {"DETECTOR":"([abc]+)"})
         assert_raises(ValueError, checker.check, "test.fits", {"DETECTOR": "([def]+)"})
 
-        info = certify.TpnInfo('DETECTOR','H', 'C', 'R', ["{.*1234}","BETWEEN_300_400","#OTHER#"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('DETECTOR','H', 'C', 'R', ["{.*1234}","BETWEEN_300_400","#OTHER#"])
+        checker = validators.validator(info)
         checker.check("test.fits", {"DETECTOR":"{.*1234}"})
 
-        info = certify.TpnInfo('DETECTOR','H', 'C', 'R', ["(THIS)","BETWEEN_300_400","#OTHER#"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('DETECTOR','H', 'C', 'R', ["(THIS)","BETWEEN_300_400","#OTHER#"])
+        checker = validators.validator(info)
         checker.check("test.fits", {"DETECTOR":"BETWEEN_300_400"})
 
-        info = certify.TpnInfo('DETECTOR','H', 'C', 'R', ["# >1 and <37 #","BETWEEN_300_400","#OTHER#"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('DETECTOR','H', 'C', 'R', ["# >1 and <37 #","BETWEEN_300_400","#OTHER#"])
+        checker = validators.validator(info)
         checker.check("test.fits", {"DETECTOR":"# >1 and <37 #"})
 
         # This demos synatax/check for "NOT FOO" in rmap match tuples
-        info = certify.TpnInfo('DETECTOR','H', 'C', 'R', ["NOT_FOO","BETWEEN_300_400","#OTHER#"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('DETECTOR','H', 'C', 'R', ["NOT_FOO","BETWEEN_300_400","#OTHER#"])
+        checker = validators.validator(info)
         checker.check("test.fits", {"DETECTOR":"NOT_FOO"})
 
     def test_tpn_pedigree_missing(self):
-        info = certify.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
-        checker = certify.validator(info)
-        assert_raises(certify.MissingKeywordError,
+        info = generic_tpn.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
+        checker = validators.validator(info)
+        assert_raises(exceptions.MissingKeywordError,
             checker.check, "test.fits", {"DETECTOR":"This is a test"})
 
     def test_tpn_pedigree_dummy(self):
-        info = certify.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
+        checker = validators.validator(info)
         checker.check("test.fits", {"PEDIGREE":"DUMMY"})
 
     def test_tpn_pedigree_ground(self):
-        info = certify.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
+        checker = validators.validator(info)
         checker.check("test.fits", {"PEDIGREE":"GROUND"})
 
     def test_tpn_pedigree_simulation(self):
-        info = certify.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
+        checker = validators.validator(info)
         checker.check("test.fits", {"PEDIGREE":"SIMULATION"})
 
     def test_tpn_pedigree_bad_leading(self):
-        info = certify.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
+        checker = validators.validator(info)
         assert_raises(ValueError, checker.check, "test.fits", {"PEDIGREE":"xDUMMY"})
 
     def test_tpn_pedigree_bad_trailing(self):
         # typical subtle expression error, "=" vs. "=="
-        info = certify.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
+        checker = validators.validator(info)
         assert_raises(ValueError, checker.check, "test.fits", {"PEDIGREE":"DUMMYxyz"})
 
     def test_tpn_pedigree_inflight_no_date(self):
-        info = certify.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
+        checker = validators.validator(info)
         assert_raises(ValueError, checker.check, "test.fits", {"PEDIGREE":"INFLIGHT"})
 
     def test_tpn_pedigree_equal_start_stop(self):
-        info = certify.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
+        checker = validators.validator(info)
         checker.check("test.fits", {"PEDIGREE":"INFLIGHT 02/01/2017 02/01/2017"})
 
     def test_tpn_pedigree_bad_datetime_order(self):
-        info = certify.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
+        checker = validators.validator(info)
         assert_raises(ValueError, checker.check, "test.fits", {"PEDIGREE":"INFLIGHT 2017-01-02 2017-01-01"})
 
     def test_tpn_pedigree_good_datetime_slash(self):
-        info = certify.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
+        checker = validators.validator(info)
         checker.check("test.fits", {"PEDIGREE":"INFLIGHT 02/01/2017 03/01/2017"})
 
     def test_tpn_pedigree_bad_datetime_slash(self):
-        info = certify.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
+        checker = validators.validator(info)
         assert_raises(ValueError, checker.check, "test.fits", {"PEDIGREE":"INFLIGHT 02/25/2017 03/01/2017"})
 
     def test_tpn_pedigree_good_datetime_dash(self):
-        info = certify.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
+        checker = validators.validator(info)
         checker.check("test.fits", {"PEDIGREE":"INFLIGHT 2017-01-01 2017-01-02"})
 
     def test_tpn_pedigree_bad_datetime_dash(self):
-        info = certify.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
+        checker = validators.validator(info)
         assert_raises(ValueError, checker.check, "test.fits", {"PEDIGREE":"INFLIGHT 2017-01-01 01-02-2017"})
 
     def test_tpn_pedigree_bad_datetime_dash_dash(self):
-        info = certify.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
+        checker = validators.validator(info)
         assert_raises(ValueError, checker.check, "test.fits", {"PEDIGREE":"INFLIGHT 2017-01-01 - 2017-01-02"})
 
     def test_tpn_pedigree_bad_datetime_format_1(self):
-        info = certify.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
+        checker = validators.validator(info)
         assert_raises(ValueError, checker.check, "test.fits",
                       {"PEDIGREE":"INFLIGHT 2017-01-01 - 2017-01-02 -"})
 
     def test_tpn_pedigree_bad_datetime_format_2(self):
-        info = certify.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
+        checker = validators.validator(info)
         assert_raises(ValueError, checker.check,
                       "test.fits", {"PEDIGREE":"INFLIGHT 2017-01-01 - 2017/01/02"})
 
     def test_tpn_pedigree_bad_datetime_format_3(self):
-        info = certify.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PEDIGREE','H', 'C', 'R', ["&PEDIGREE"])
+        checker = validators.validator(info)
         assert_raises(ValueError, checker.check,
                       "test.fits", {"PEDIGREE":"INFLIGHT 2017-01-01T00:00:00 2017-01-02"})
 
     def test_tpn_jwstpedigree_dashdate(self):
-        info = certify.TpnInfo('PEDIGREE','H', 'C', 'R', ["&JWSTPEDIGREE"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PEDIGREE','H', 'C', 'R', ["&JWSTPEDIGREE"])
+        checker = validators.validator(info)
         checker.check(
             "test.fits", {"PEDIGREE":"INFLIGHT 2017-01-01 2017-01-02"})
 
     def test_tpn_jwstpedigree_ground_dates(self):
-        info = certify.TpnInfo('PEDIGREE','H', 'C', 'R', ["&JWSTPEDIGREE"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PEDIGREE','H', 'C', 'R', ["&JWSTPEDIGREE"])
+        checker = validators.validator(info)
         assert_raises(
             ValueError, checker.check, "test.fits",
             {"PEDIGREE":"GROUND 2018-01-01 2018-01-25"})
 
     def test_tpn_jwstpedigree_nodate_format_3(self):
-        info = certify.TpnInfo('PEDIGREE','H', 'C', 'R', ["&JWSTPEDIGREE"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PEDIGREE','H', 'C', 'R', ["&JWSTPEDIGREE"])
+        checker = validators.validator(info)
         assert_raises(
             ValueError, checker.check, "test.fits", {"PEDIGREE":"INFLIGHT"})
 
     def test_tpn_jwstpedigree_missing_format_3(self):
-        info = certify.TpnInfo('PEDIGREE','H', 'C', 'R', ["&JWSTPEDIGREE"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PEDIGREE','H', 'C', 'R', ["&JWSTPEDIGREE"])
+        checker = validators.validator(info)
         assert_raises(
-            certify.MissingKeywordError, checker.check, "test.fits", {})
+            exceptions.MissingKeywordError, checker.check, "test.fits", {})
 
     def test_tpn_jwstpedigree_no_model_3(self):
-        info = certify.TpnInfo('PEDIGREE','H', 'C', 'R', ["&JWSTPEDIGREE"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PEDIGREE','H', 'C', 'R', ["&JWSTPEDIGREE"])
+        checker = validators.validator(info)
         assert_raises(
             ValueError, checker.check, "test.fits", {"PEDIGREE":"MODEL"})
 
     def test_tpn_pedigree_missing_column(self):
-        info = certify.TpnInfo('PEDIGREE','C', 'C', 'R', ["&PEDIGREE"])
-        checker = certify.validator(info)
-        assert_raises(certify.MissingKeywordError, checker.check_column, "data/x2i1559gl_wcp.fits", {})
+        info = generic_tpn.TpnInfo('PEDIGREE','C', 'C', 'R', ["&PEDIGREE"])
+        checker = validators.validator(info)
+        assert_raises(exceptions.MissingKeywordError, checker.check_column, "data/x2i1559gl_wcp.fits", {})
 
     def test_tpn_pedigree_ok_column(self):
-        info = certify.TpnInfo('PEDIGREE','C', 'C', 'R', ["&PEDIGREE"])
-        checker = certify.validator(info)
+        info = generic_tpn.TpnInfo('PEDIGREE','C', 'C', 'R', ["&PEDIGREE"])
+        checker = validators.validator(info)
         header = data_file.get_header(self.data("16j16005o_apd.fits"))
         checker.check_column("data/16j16005o_apd.fits", header)
 
 # ------------------------------------------------------------------------------
 
     def test_sybdate_validator(self):
-        tinfo = certify.TpnInfo('USEAFTER','H','C','R',('&SYBDATE',))
-        cval = certify.validator(tinfo)
-        assert_true(isinstance(cval,certify.SybdateValidator))
+        tinfo = generic_tpn.TpnInfo('USEAFTER','H','C','R',('&SYBDATE',))
+        cval = validators.validator(tinfo)
+        assert_true(isinstance(cval,validators.core.SybdateValidator))
         header = data_file.get_header(self.data("acs_new_idc.fits"))
         cval.check(self.data('acs_new_idc.fits'), header)
 
     def test_slashdate_validator(self):
-        tinfo = certify.TpnInfo('USEAFTER','H','C','R',('&SLASHDATE',))
-        checker = certify.validator(tinfo)
+        tinfo = generic_tpn.TpnInfo('USEAFTER','H','C','R',('&SLASHDATE',))
+        checker = validators.validator(tinfo)
         checker.check("test.fits", {"USEAFTER":"25/12/2016"})
         assert_raises(ValueError, checker.check, "test.fits", {"USEAFTER":"2017-12-25"})
 
     def test_Anydate_validator(self):
-        tinfo = certify.TpnInfo('USEAFTER','H','C','R',('&ANYDATE',))
-        checker = certify.validator(tinfo)
+        tinfo = generic_tpn.TpnInfo('USEAFTER','H','C','R',('&ANYDATE',))
+        checker = validators.validator(tinfo)
         checker.check("test.fits", {"USEAFTER":"25/12/2016"})
         checker.check("test.fits", {"USEAFTER":"Mar 21 2001 12:00:00 am"})
         assert_raises(ValueError, checker.check, "test.fits", {"USEAFTER":"2017-01-01T00:00:00.000"})
         assert_raises(ValueError, checker.check, "test.fits", {"USEAFTER":"12-25-2017"})
         assert_raises(ValueError, checker.check, "test.fits", {"USEAFTER":"Mxx 21 2001 01:00:00 PM"})
         assert_raises(ValueError, checker.check, "test.fits", {"USEAFTER":"35/12/20117"})
 
@@ -2021,30 +2096,30 @@
                                                [ 0.0316    ,  0.88160002,  0.0316    ],
                                                [ 0.        ,  0.0276    ,  0.        ]], dtype='float32'),
                                 'DATA_TYPE': 'float32',
                                 'EXTENSION': 1,
                                 'KIND': 'IMAGE',
                                 'SHAPE': (3, 3)})
                 }
-        info = certify.TpnInfo('SCI','D','X','R',('&KernelUnity',))
-        checker = certify.KernelunityValidator(info)
+        info = generic_tpn.TpnInfo('SCI','D','X','R',('&KernelUnity',))
+        checker = validators.core.KernelunityValidator(info)
         checker.check("test.fits", header)
 
     def test_certify_kernel_unity_validator_bad(self):
         header = {'SCI_ARRAY': utils.Struct({'COLUMN_NAMES': None,
                                 'DATA': np.array([[ 0.        ,  0.0276    ,  0.        ],
                                                [ 0.0316    ,  0.88160002 + 1e-6,  0.0316    ],
                                                [ 0.        ,  0.0276    ,  0.        ]], dtype='float32'),
                                 'DATA_TYPE': 'float32',
                                 'EXTENSION': 1,
                                 'KIND': 'IMAGE',
                                 'SHAPE': (3, 3)})
                 }
-        info = certify.TpnInfo('SCI','D','X','R',('&KernelUnity',))
-        checker = certify.KernelunityValidator(info)
+        info = generic_tpn.TpnInfo('SCI','D','X','R',('&KernelUnity',))
+        checker = validators.core.KernelunityValidator(info)
         assert_raises(exceptions.BadKernelSumError, checker.check, "test.fits", header)
 
 
 # ==================================================================================
 
 def main():
     """Run module tests,  for now just doctests only."""
```

### Comparing `crds-7.5.0.0/crds/tests/test_check_archive.py` & `crds-7.6.0/crds/tests/test_check_archive.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_checksum.py` & `crds-7.6.0/crds/tests/test_checksum.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_cmdline.py` & `crds-7.6.0/crds/tests/test_cmdline.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_config.py` & `crds-7.6.0/crds/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_diff.py` & `crds-7.6.0/crds/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_heavy_client.py` & `crds-7.6.0/crds/tests/test_heavy_client.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_io.py` & `crds-7.6.0/crds/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_list.py` & `crds-7.6.0/crds/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_locking.py` & `crds-7.6.0/crds/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_matches.py` & `crds-7.6.0/crds/tests/test_matches.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_newcontext.py` & `crds-7.6.0/crds/tests/test_newcontext.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_or_bars.py` & `crds-7.6.0/crds/tests/test_or_bars.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_refactor.py` & `crds-7.6.0/crds/tests/test_refactor.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_reftypes.py` & `crds-7.6.0/crds/tests/test_reftypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,16 +242,16 @@
     def tearDown(self, *args, **keys):
         super(TestReftypes, self).tearDown(*args, **keys)
         log.set_exception_trap(self._old_debug)
 
     # ------------------------------------------------------------------------------
 
     def test_validator_bad_presence(self):
-        #         tinfo = certify.TpnInfo('DETECTOR','H','C','Q', ('WFC','HRC','SBC'))
-        #         assert_raises(ValueError, certify.validator, tinfo)
+        #         tinfo = certify.generic_tpn.TpnInfo('DETECTOR','H','C','Q', ('WFC','HRC','SBC'))
+        #         assert_raises(ValueError, certify.validators.validator, tinfo)
         pass
 
 # ==================================================================================
 
 def main():
     """Run module tests,  for now just doctests only."""
     import unittest
```

### Comparing `crds-7.5.0.0/crds/tests/test_rmap.py` & `crds-7.6.0/crds/tests/test_rmap.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_rowdiff.py` & `crds-7.6.0/crds/tests/test_rowdiff.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_special.py` & `crds-7.6.0/crds/tests/test_special.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_submit.py` & `crds-7.6.0/crds/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_substitutions.py` & `crds-7.6.0/crds/tests/test_substitutions.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_sync.py` & `crds-7.6.0/crds/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_table_effects.py` & `crds-7.6.0/crds/tests/test_table_effects.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_uniqname.py` & `crds-7.6.0/crds/tests/test_uniqname.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tests/test_uses.py` & `crds-7.6.0/crds/tests/test_uses.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tobs/__init__.py` & `crds-7.6.0/crds/tobs/__init__.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tobs/locate.py` & `crds-7.6.0/crds/tobs/locate.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tobs/specs/combined_specs.json` & `crds-7.6.0/crds/tobs/specs/combined_specs.json`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tobs/tests.py` & `crds-7.6.0/crds/tobs/tests.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tobs/tpns/tinstr_tfk.tpn` & `crds-7.6.0/crds/tobs/tpns/tinstr_tfk.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/tobs/tpns/tinstr_tfk_ld.tpn` & `crds-7.6.0/crds/tobs/tpns/tinstr_tfk_ld.tpn`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds/uses.py` & `crds-7.6.0/crds/uses.py`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/crds.egg-info/PKG-INFO` & `crds-7.6.0/crds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crds
-Version: 7.5.0.0
+Version: 7.6.0
 Summary: Calibration Reference Data System,  HST/JWST reference file management
 Home-page: https://hst-crds.stsci.edu
 Author: Todd Miller
 Author-email: jmiller@stsci.edu
 License: BSD
 Description: ====
         CRDS
@@ -177,7 +177,8 @@
 Provides: crds
 Provides-Extra: jwst
 Provides-Extra: submission
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: docs
 Provides-Extra: aws
+Provides-Extra: synphot
```

### Comparing `crds-7.5.0.0/crds.egg-info/SOURCES.txt` & `crds-7.6.0/crds.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,18 @@
 crds/certify/__init__.py
 crds/certify/__main__.py
 crds/certify/certify.py
 crds/certify/check_sha1sum.py
 crds/certify/generic_tpn.py
 crds/certify/mapping_parser.py
 crds/certify/reftypes.py
-crds/certify/validator_helpers.py
-crds/certify/validators.py
+crds/certify/validators/__init__.py
+crds/certify/validators/core.py
+crds/certify/validators/helpers.py
+crds/certify/validators/synphot.py
 crds/client/__init__.py
 crds/client/api.py
 crds/client/proxy.py
 crds/core/__init__.py
 crds/core/cmdline.py
 crds/core/config.py
 crds/core/constants.py
@@ -167,14 +169,15 @@
 crds/hst/specs/stis_sptrctab.spec
 crds/hst/specs/stis_srwtab.spec
 crds/hst/specs/stis_tdctab.spec
 crds/hst/specs/stis_tdstab.spec
 crds/hst/specs/stis_teltab.spec
 crds/hst/specs/stis_wcptab.spec
 crds/hst/specs/stis_xtractab.spec
+crds/hst/specs/synphot_obsmodes.rmap
 crds/hst/specs/synphot_thermal.rmap
 crds/hst/specs/synphot_thruput.rmap
 crds/hst/specs/synphot_tmctab.rmap
 crds/hst/specs/synphot_tmgtab.rmap
 crds/hst/specs/synphot_tmttab.rmap
 crds/hst/specs/wfc3_atodtab.spec
 crds/hst/specs/wfc3_biacfile.rmap
@@ -545,14 +548,16 @@
 crds/hst/tpns/stis_tdc_ld.tpn
 crds/hst/tpns/stis_tds.tpn
 crds/hst/tpns/stis_tds_ld.tpn
 crds/hst/tpns/stis_tel.tpn
 crds/hst/tpns/stis_tel_ld.tpn
 crds/hst/tpns/stis_wcp.tpn
 crds/hst/tpns/stis_wcp_ld.tpn
+crds/hst/tpns/synphot_obs.tpn
+crds/hst/tpns/synphot_obs_ld.tpn
 crds/hst/tpns/synphot_syn.tpn
 crds/hst/tpns/synphot_syn_ld.tpn
 crds/hst/tpns/synphot_th.tpn
 crds/hst/tpns/synphot_th_ld.tpn
 crds/hst/tpns/synphot_tmc.tpn
 crds/hst/tpns/synphot_tmc_ld.tpn
 crds/hst/tpns/synphot_tmg.tpn
@@ -666,14 +671,15 @@
 crds/jwst/jwst_system_crdscfg_b7.1.1.yaml
 crds/jwst/jwst_system_crdscfg_b7.1.3.yaml
 crds/jwst/jwst_system_crdscfg_b7.1.yaml
 crds/jwst/jwst_system_crdscfg_b7.2.yaml
 crds/jwst/jwst_system_crdscfg_b7.3.yaml
 crds/jwst/jwst_system_crdscfg_b7.4.yaml
 crds/jwst/jwst_system_crdscfg_b7.5.yaml
+crds/jwst/jwst_system_crdscfg_b7.6.yaml
 crds/jwst/jwst_system_crdscfg_b7.yaml
 crds/jwst/locate.py
 crds/jwst/miri.py
 crds/jwst/nircam.py
 crds/jwst/niriss.py
 crds/jwst/nirspec.py
 crds/jwst/pipeline.py
@@ -787,14 +793,15 @@
 crds/jwst/specs/niriss_drizpars.spec
 crds/jwst/specs/niriss_extract1d.rmap
 crds/jwst/specs/niriss_flat.spec
 crds/jwst/specs/niriss_gain.spec
 crds/jwst/specs/niriss_ipc.spec
 crds/jwst/specs/niriss_linearity.spec
 crds/jwst/specs/niriss_mask.spec
+crds/jwst/specs/niriss_pars-image2pipeline.rmap
 crds/jwst/specs/niriss_pathloss.rmap
 crds/jwst/specs/niriss_persat.rmap
 crds/jwst/specs/niriss_photom.spec
 crds/jwst/specs/niriss_readnoise.spec
 crds/jwst/specs/niriss_regions.spec
 crds/jwst/specs/niriss_saturation.spec
 crds/jwst/specs/niriss_specwcs.rmap
@@ -830,14 +837,15 @@
 crds/jwst/specs/nirspec_ifuslicer.rmap
 crds/jwst/specs/nirspec_ipc.spec
 crds/jwst/specs/nirspec_linearity.spec
 crds/jwst/specs/nirspec_mask.spec
 crds/jwst/specs/nirspec_msa.rmap
 crds/jwst/specs/nirspec_msaoper.rmap
 crds/jwst/specs/nirspec_ote.rmap
+crds/jwst/specs/nirspec_pars-spec2pipeline.rmap
 crds/jwst/specs/nirspec_pathloss.rmap
 crds/jwst/specs/nirspec_persat.rmap
 crds/jwst/specs/nirspec_photom.rmap
 crds/jwst/specs/nirspec_readnoise.spec
 crds/jwst/specs/nirspec_refpix.rmap
 crds/jwst/specs/nirspec_regions.spec
 crds/jwst/specs/nirspec_saturation.spec
@@ -992,14 +1000,18 @@
 crds/misc/cal_pipelines.py
 crds/misc/check_archive.py
 crds/misc/datalvl.py
 crds/misc/get_synphot.py
 crds/misc/query_affected.py
 crds/misc/sql.py
 crds/misc/uniqname.py
+crds/misc/synphot/__init__.py
+crds/misc/synphot/integration_tests.py
+crds/misc/synphot/lookup_generator.py
+crds/misc/synphot/utils.py
 crds/refactoring/__init__.py
 crds/refactoring/checksum.py
 crds/refactoring/newcontext.py
 crds/refactoring/refactor.py
 crds/refactoring/refactor2.py
 crds/submit/__init__.py
 crds/submit/__main__.py
@@ -1033,14 +1045,15 @@
 crds/tests/test_rmap.py
 crds/tests/test_rowdiff.py
 crds/tests/test_special.py
 crds/tests/test_submit.py
 crds/tests/test_substitutions.py
 crds/tests/test_sync.py
 crds/tests/test_synphot_hst.py
+crds/tests/test_synphot_lookup_generator.py
 crds/tests/test_table_effects.py
 crds/tests/test_uniqname.py
 crds/tests/test_uses.py
 crds/tobs/__init__.py
 crds/tobs/__main__.py
 crds/tobs/locate.py
 crds/tobs/substitutions.dat
```

### Comparing `crds-7.5.0.0/envs/env-forwarded.csh` & `crds-7.6.0/envs/env-forwarded.csh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/env-local.csh` & `crds-7.6.0/envs/env-local.csh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/hst-crds-dev.csh` & `crds-7.6.0/envs/hst-crds-dev.csh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/hst-crds-dev.sh` & `crds-7.6.0/envs/hst-crds-dev.sh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/hst-crds-ops.csh` & `crds-7.6.0/envs/hst-crds-ops.csh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/hst-crds-ops.sh` & `crds-7.6.0/envs/hst-crds-ops.sh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/hst-crds-readonly.csh` & `crds-7.6.0/envs/hst-crds-readonly.csh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/hst-crds-readonly.sh` & `crds-7.6.0/envs/hst-crds-readonly.sh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/hst-crds-test.csh` & `crds-7.6.0/envs/hst-crds-test.csh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/hst-crds-test.sh` & `crds-7.6.0/envs/hst-crds-test.sh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/jwst-crds-b5it.csh` & `crds-7.6.0/envs/jwst-crds-b5it.csh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/jwst-crds-b6it.csh` & `crds-7.6.0/envs/jwst-crds-b6it.csh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/jwst-crds-bit.csh` & `crds-7.6.0/envs/jwst-crds-bit.csh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/jwst-crds-bit.sh` & `crds-7.6.0/envs/jwst-crds-bit.sh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/jwst-crds-cit.csh` & `crds-7.6.0/envs/jwst-crds-cit.csh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/jwst-crds-cit.sh` & `crds-7.6.0/envs/jwst-crds-cit.sh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/jwst-crds-dev.csh` & `crds-7.6.0/envs/jwst-crds-dev.csh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/jwst-crds-dev.sh` & `crds-7.6.0/envs/jwst-crds-dev.sh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/jwst-crds-dit.csh` & `crds-7.6.0/envs/jwst-crds-dit.csh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/jwst-crds-dit.sh` & `crds-7.6.0/envs/jwst-crds-dit.sh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/jwst-crds-ops.csh` & `crds-7.6.0/envs/jwst-crds-ops.csh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/jwst-crds-ops.sh` & `crds-7.6.0/envs/jwst-crds-ops.sh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/jwst-crds-readonly.csh` & `crds-7.6.0/envs/jwst-crds-readonly.csh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/jwst-crds-readonly.sh` & `crds-7.6.0/envs/jwst-crds-readonly.sh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/jwst-crds-test.csh` & `crds-7.6.0/envs/jwst-crds-test.csh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/jwst-crds-test.sh` & `crds-7.6.0/envs/jwst-crds-test.sh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/envs/s3.sh` & `crds-7.6.0/envs/s3.sh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/install` & `crds-7.6.0/install`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/scripts/crds` & `crds-7.6.0/scripts/crds`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/scripts/crds_check_cache` & `crds-7.6.0/scripts/crds_check_cache`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/scripts/crds_dataset_capture` & `crds-7.6.0/scripts/crds_dataset_capture`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/scripts/crds_jwst_serverless_pipeline_env.csh` & `crds-7.6.0/scripts/crds_jwst_serverless_pipeline_env.csh`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/scripts/crds_repair_cache` & `crds-7.6.0/scripts/crds_repair_cache`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/scripts/crds_unique` & `crds-7.6.0/scripts/crds_unique`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/scripts/cron_sync` & `crds-7.6.0/scripts/cron_sync`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/scripts/custom_query_affected_datasets` & `crds-7.6.0/scripts/custom_query_affected_datasets`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/scripts/pipeline_bestref` & `crds-7.6.0/scripts/pipeline_bestref`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/scripts/remote_cache_init` & `crds-7.6.0/scripts/remote_cache_init`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/scripts/safe_bestrefs` & `crds-7.6.0/scripts/safe_bestrefs`

 * *Files identical despite different names*

### Comparing `crds-7.5.0.0/setup.py` & `crds-7.6.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,38 +7,42 @@
 import setuptools
 
 setup_pars = {
     "packages" : [
         'crds',
         'crds.bestrefs',
         'crds.certify',
+        'crds.certify.validators',
         'crds.client',
         'crds.core',
         'crds.io',
         'crds.submit',
 
         'crds.misc',
+        'crds.misc.synphot',
         'crds.refactoring',
 
         'crds.hst',
         'crds.jwst',
         'crds.tobs',
 
         'crds.tests',
         ],
     "package_dir" : {
         'crds' : 'crds',
         'crds.bestrefs' : 'crds/bestrefs',
         'crds.certify' : 'crds/certify',
+        'crds.certify.validators' : 'crds/certify/validators',
         'crds.client' : 'crds/client',
         'crds.core' : 'crds/core',
         'crds.io' : 'crds/io',
         'crds.submit' : 'crds/submit',
 
         'crds.misc' : 'crds/misc',
+        'crds.misc.synphot' : 'crds/misc/synphot',
         'crds.refactoring' : 'crds/refactoring',
 
         'crds.hst' : 'crds/hst',
         'crds.jwst' : 'crds/jwst',
         'crds.tobs' : 'crds/tobs',
 
         'crds.tests' : 'crds/tests',
@@ -80,15 +84,15 @@
 
 TEST_DEPS = ["lockfile", "mock", "nose", "pytest", "pylint", "flake8", "bandit",]
 
 SUBMISSION_DEPS = ["requests", "lxml", "parsley"]
 
 setup(name="crds",
       provides=["crds"],
-      version = '7.5.0.0',
+      version = '7.6.0',
       description="Calibration Reference Data System,  HST/JWST reference file management",
       long_description=open('README.rst').read(),
       author="Todd Miller",
       author_email="jmiller@stsci.edu",
       url="https://hst-crds.stsci.edu",
       license="BSD",
       install_requires=["astropy", "numpy", "filelock"] + SUBMISSION_DEPS,
@@ -96,14 +100,15 @@
           "jwst": ["jwst"],
           "submission": ["requests", "lxml", "parsley"],
           "dev" : ["ipython","jupyterlab","ansible","helm",
                    "nose-cprof", "coverage"],
           "test" : TEST_DEPS,
           "docs" : ["sphinx","sphinx_rtd_theme","docutils"],
           "aws" : ["boto3","awscli"],
+          "synphot": ["stsynphot"],
       },
       tests_require=TEST_DEPS,
       zip_safe=False,
       classifiers=[
           'Intended Audience :: Science/Research',
           'License :: OSI Approved :: BSD License',
           'Operating System :: POSIX :: Linux',
```

### Comparing `crds-7.5.0.0/setup_data.py` & `crds-7.6.0/setup_data.py`

 * *Files identical despite different names*

