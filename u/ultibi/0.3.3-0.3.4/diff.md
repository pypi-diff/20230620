# Comparing `tmp/ultibi-0.3.3.tar.gz` & `tmp/ultibi-0.3.4.tar.gz`

## Comparing `ultibi-0.3.3.tar` & `ultibi-0.3.4.tar`

### file list

```diff
@@ -1,153 +1,153 @@
--rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 ultibi-0.3.3/local_dependencies/ultibi_server/Cargo.toml
--rw-r--r--   0     1001      123      219 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_server/build.rs
--rw-r--r--   0     1001      123       35 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_server/src/api/mod.rs
--rw-r--r--   0     1001      123      754 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_server/src/api/open_api.rs
--rw-r--r--   0     1001      123     6651 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_server/src/api/routers.rs
--rw-r--r--   0     1001      123     1264 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_server/src/app.rs
--rw-r--r--   0     1001      123     2593 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_server/src/helpers.rs
--rw-r--r--   0     1001      123     1432 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_server/src/lib.rs
--rw-r--r--   0     1001      123      433 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_server/src/visual.rs
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 ultibi-0.3.3/local_dependencies/ultibi/Cargo.toml
--rw-r--r--   0     1001      123        0 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi/README.md
--rw-r--r--   0     1001      123       73 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi/src/lib.rs
--rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 ultibi-0.3.3/local_dependencies/ultibi_core/Cargo.toml
--rw-r--r--   0     1001      123     2031 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/add_row.rs
--rw-r--r--   0     1001      123     3486 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/aggregations.rs
--rw-r--r--   0     1001      123      654 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/cache.rs
--rw-r--r--   0     1001      123     4244 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/datarequest.rs
--rw-r--r--   0     1001      123     9751 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/dataset.rs
--rw-r--r--   0     1001      123     1782 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/datasource/acquire.rs
--rw-r--r--   0     1001      123     2059 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/datasource/awss3.rs
--rw-r--r--   0     1001      123     5329 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/datasource/helpers.rs
--rw-r--r--   0     1001      123     7509 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/datasource/mod.rs
--rw-r--r--   0     1001      123      700 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/errors.rs
--rw-r--r--   0     1001      123    10956 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/execution/execute_agg.rs
--rw-r--r--   0     1001      123     4594 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs
--rw-r--r--   0     1001      123      464 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/execution/mod.rs
--rw-r--r--   0     1001      123     2663 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/filters.rs
--rw-r--r--   0     1001      123       18 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/helpers/mod.rs
--rw-r--r--   0     1001      123      545 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/helpers/searches.rs
--rw-r--r--   0     1001      123      375 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/lib.rs
--rw-r--r--   0     1001      123    11996 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/measure.rs
--rw-r--r--   0     1001      123     5459 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/overrides.rs
--rw-r--r--   0     1001      123      230 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/prelude.rs
--rw-r--r--   0     1001      123       64 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/reports/mod.rs
--rw-r--r--   0     1001      123     1178 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/src/reports/report.rs
--rw-r--r--   0     1001      123     1884 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/add_row.rs
--rw-r--r--   0     1001      123      741 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/agg_request.rs
--rw-r--r--   0     1001      123     1543 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/aggregations.rs
--rw-r--r--   0     1001      123        1 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/cache.rs
--rw-r--r--   0     1001      123     2067 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/common/mod.rs
--rw-r--r--   0     1001      123       95 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/data/bad_config.toml
--rw-r--r--   0     1001      123      553 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/data/bad_config2.toml
--rw-r--r--   0     1001      123      116 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/data/test_config.toml
--rw-r--r--   0     1001      123      354 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/data/testset.csv
--rw-r--r--   0     1001      123     1250 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/datasource.rs
--rw-r--r--   0     1001      123     3115 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/dependants.rs
--rw-r--r--   0     1001      123     1485 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/filters.rs
--rw-r--r--   0     1001      123        1 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/ultibi_core/tests/overrides.rs
--rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 ultibi-0.3.3/local_dependencies/frtb_engine/Cargo.toml
--rw-r--r--   0     1001      123      481 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/README.md
--rw-r--r--   0     1001      123    14931 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/data/frtb/Delta.csv
--rw-r--r--   0     1001      123      541 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv
--rw-r--r--   0     1001      123     2160 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/data/frtb/datasource_config.toml
--rw-r--r--   0     1001      123      159 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/data/frtb/hms.csv
--rw-r--r--   0     1001      123      177 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/data/frtb/vega_risk_weights.csv
--rw-r--r--   0     1001      123    20066 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/calc_params.rs
--rw-r--r--   0     1001      123       25 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/docs/mod.rs
--rw-r--r--   0     1001      123     1226 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/docs/optional_params.rs
--rw-r--r--   0     1001      123     1424 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/drc/common.rs
--rw-r--r--   0     1001      123    11840 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs
--rw-r--r--   0     1001      123     9483 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs
--rw-r--r--   0     1001      123     7606 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/drc/drc_weights.rs
--rw-r--r--   0     1001      123       96 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/drc/mod.rs
--rw-r--r--   0     1001      123      787 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/drc/totals.rs
--rw-r--r--   0     1001      123     4811 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/helpers.rs
--rw-r--r--   0     1001      123     8968 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/lib.rs
--rw-r--r--   0     1001      123     3780 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/measures.rs
--rw-r--r--   0     1001      123      188 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/prelude.rs
--rw-r--r--   0     1001      123    26516 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/risk_weights.rs
--rw-r--r--   0     1001      123     5408 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/risk_weights_crr2.rs
--rw-r--r--   0     1001      123     5268 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/rrao/mod.rs
--rw-r--r--   0     1001      123     1374 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/buckets.rs
--rw-r--r--   0     1001      123    14177 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs
--rw-r--r--   0     1001      123    13866 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs
--rw-r--r--   0     1001      123       64 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/commodity/mod.rs
--rw-r--r--   0     1001      123     3699 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs
--rw-r--r--   0     1001      123     7432 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs
--rw-r--r--   0     1001      123    29827 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/common.rs
--rw-r--r--   0     1001      123     9793 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/common_curv.rs
--rw-r--r--   0     1001      123    19318 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs
--rw-r--r--   0     1001      123    17703 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs
--rw-r--r--   0     1001      123       64 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_nonsec/mod.rs
--rw-r--r--   0     1001      123     3841 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs
--rw-r--r--   0     1001      123    11803 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs
--rw-r--r--   0     1001      123    15617 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs
--rw-r--r--   0     1001      123    12459 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs
--rw-r--r--   0     1001      123       64 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/mod.rs
--rw-r--r--   0     1001      123     2904 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs
--rw-r--r--   0     1001      123     8782 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs
--rw-r--r--   0     1001      123    15261 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs
--rw-r--r--   0     1001      123    13479 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs
--rw-r--r--   0     1001      123       64 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/mod.rs
--rw-r--r--   0     1001      123     2988 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs
--rw-r--r--   0     1001      123     8063 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs
--rw-r--r--   0     1001      123    17052 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs
--rw-r--r--   0     1001      123    10900 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/equity/delta.rs
--rw-r--r--   0     1001      123       64 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/equity/mod.rs
--rw-r--r--   0     1001      123     2162 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/equity/totals.rs
--rw-r--r--   0     1001      123    10428 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/equity/vega.rs
--rw-r--r--   0     1001      123    14289 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs
--rw-r--r--   0     1001      123    11992 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/fx/delta.rs
--rw-r--r--   0     1001      123       64 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/fx/mod.rs
--rw-r--r--   0     1001      123     2162 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/fx/totals.rs
--rw-r--r--   0     1001      123    10166 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/fx/vega.rs
--rw-r--r--   0     1001      123    14030 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs
--rw-r--r--   0     1001      123    21887 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/girr/delta.rs
--rw-r--r--   0     1001      123       64 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/girr/mod.rs
--rw-r--r--   0     1001      123     2295 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/girr/totals.rs
--rw-r--r--   0     1001      123    15657 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/girr/vega.rs
--rw-r--r--   0     1001      123      221 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/mod.rs
--rw-r--r--   0     1001      123     5170 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/totals.rs
--rw-r--r--   0     1001      123    28643 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/statics.rs
--rw-r--r--   0     1001      123      753 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/totals.rs
--rw-r--r--   0     1001      123     1881 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/src/validate.rs
--rw-r--r--   0     1001      123     1756 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/tests/common/mod.rs
--rw-r--r--   0     1001      123     1486 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/tests/dependant.rs
--rw-r--r--   0     1001      123     4487 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/tests/drc.rs
--rw-r--r--   0     1001      123      420 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/tests/rrao.rs
--rw-r--r--   0     1001      123    18903 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/tests/sbm.rs
--rw-r--r--   0     1001      123      744 2023-06-10 15:44:32.000000 ultibi-0.3.3/local_dependencies/frtb_engine/tests/sbm_totals.rs
--rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 ultibi-0.3.3/Cargo.toml
--rw-r--r--   0     1001      123      728 2023-06-10 15:44:32.000000 ultibi-0.3.3/.gitignore
--rw-r--r--   0     1001      123     5183 2023-06-10 15:44:32.000000 ultibi-0.3.3/LICENSE
--rw-r--r--   0     1001      123     2403 2023-06-10 15:44:32.000000 ultibi-0.3.3/Makefile
--rw-r--r--   0     1001      123     5565 2023-06-10 15:44:32.000000 ultibi-0.3.3/README.md
--rw-r--r--   0     1001      123     1559 2023-06-10 15:44:32.000000 ultibi-0.3.3/example.py
--rw-r--r--   0     1001      123     2104 2023-06-10 15:44:32.000000 ultibi-0.3.3/pyproject.toml
--rw-r--r--   0     1001      123       36 2023-06-10 15:44:32.000000 ultibi-0.3.3/requirements-lint.txt
--rw-r--r--   0     1001      123      307 2023-06-10 15:44:32.000000 ultibi-0.3.3/requirements.txt
--rw-r--r--   0     1001      123     3842 2023-06-10 15:44:32.000000 ultibi-0.3.3/src/calculator.rs
--rw-r--r--   0     1001      123       48 2023-06-10 15:44:32.000000 ultibi-0.3.3/src/conversions/mod.rs
--rw-r--r--   0     1001      123     3542 2023-06-10 15:44:32.000000 ultibi-0.3.3/src/conversions/series.rs
--rw-r--r--   0     1001      123     3049 2023-06-10 15:44:32.000000 ultibi-0.3.3/src/conversions/wrappers.rs
--rw-r--r--   0     1001      123     7737 2023-06-10 15:44:32.000000 ultibi-0.3.3/src/dataset.rs
--rw-r--r--   0     1001      123     3303 2023-06-10 15:44:32.000000 ultibi-0.3.3/src/errors.rs
--rw-r--r--   0     1001      123      693 2023-06-10 15:44:32.000000 ultibi-0.3.3/src/filter.rs
--rw-r--r--   0     1001      123     2021 2023-06-10 15:44:32.000000 ultibi-0.3.3/src/lib.rs
--rw-r--r--   0     1001      123     2521 2023-06-10 15:44:32.000000 ultibi-0.3.3/src/measure.rs
--rw-r--r--   0     1001      123     1353 2023-06-10 15:44:32.000000 ultibi-0.3.3/src/requests.rs
--rw-r--r--   0     1001      123     1762 2023-06-10 15:44:32.000000 ultibi-0.3.3/tests/data/datasource_config.toml
--rw-r--r--   0     1001      123     4042 2023-06-10 15:44:32.000000 ultibi-0.3.3/tests/docs/run_doc_examples.py
--rw-r--r--   0     1001      123      591 2023-06-10 15:44:32.000000 ultibi-0.3.3/tests/unit/test_compute.py
--rw-r--r--   0     1001      123     1507 2023-06-10 15:44:32.000000 ultibi-0.3.3/tests/unit/test_ds.py
--rw-r--r--   0     1001      123     2658 2023-06-10 15:44:32.000000 ultibi-0.3.3/tests/unit/test_measure.py
--rw-r--r--   0     1001      123      848 2023-06-10 15:44:32.000000 ultibi-0.3.3/ultibi/__init__.py
--rw-r--r--   0     1001      123     1060 2023-06-10 15:44:32.000000 ultibi-0.3.3/ultibi/internals/__init__.py
--rw-r--r--   0     1001      123     6733 2023-06-10 15:44:32.000000 ultibi-0.3.3/ultibi/internals/dataset.py
--rw-r--r--   0     1001      123     3131 2023-06-10 15:44:32.000000 ultibi-0.3.3/ultibi/internals/filters.py
--rw-r--r--   0     1001      123     5200 2023-06-10 15:44:32.000000 ultibi-0.3.3/ultibi/internals/measure.py
--rw-r--r--   0     1001      123     2950 2023-06-10 15:44:32.000000 ultibi-0.3.3/ultibi/internals/requests.py
--rw-r--r--   0     1001      123        0 2023-06-10 15:44:32.000000 ultibi-0.3.3/ultibi/rust_module/__init__.py
--rw-r--r--   0        0        0   100879 2023-06-10 15:47:51.000000 ultibi-0.3.3/Cargo.lock
--rw-r--r--   0        0        0     6488 1970-01-01 00:00:00.000000 ultibi-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      914 1970-01-01 00:00:00.000000 ultibi-0.3.4/local_dependencies/frtb_engine/Cargo.toml
+-rw-r--r--   0     1001      123      481 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/README.md
+-rw-r--r--   0     1001      123    14931 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/data/frtb/Delta.csv
+-rw-r--r--   0     1001      123      541 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv
+-rw-r--r--   0     1001      123     2160 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/data/frtb/datasource_config.toml
+-rw-r--r--   0     1001      123      159 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/data/frtb/hms.csv
+-rw-r--r--   0     1001      123      177 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/data/frtb/vega_risk_weights.csv
+-rw-r--r--   0     1001      123    20066 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/calc_params.rs
+-rw-r--r--   0     1001      123       25 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/docs/mod.rs
+-rw-r--r--   0     1001      123     1226 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/docs/optional_params.rs
+-rw-r--r--   0     1001      123     1424 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/drc/common.rs
+-rw-r--r--   0     1001      123    11840 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs
+-rw-r--r--   0     1001      123     9483 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs
+-rw-r--r--   0     1001      123     7606 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/drc/drc_weights.rs
+-rw-r--r--   0     1001      123       96 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/drc/mod.rs
+-rw-r--r--   0     1001      123      787 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/drc/totals.rs
+-rw-r--r--   0     1001      123     4811 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/helpers.rs
+-rw-r--r--   0     1001      123     8968 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/lib.rs
+-rw-r--r--   0     1001      123     3780 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/measures.rs
+-rw-r--r--   0     1001      123      188 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/prelude.rs
+-rw-r--r--   0     1001      123    26516 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/risk_weights.rs
+-rw-r--r--   0     1001      123     5408 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/risk_weights_crr2.rs
+-rw-r--r--   0     1001      123     5268 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/rrao/mod.rs
+-rw-r--r--   0     1001      123     1374 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/buckets.rs
+-rw-r--r--   0     1001      123    14177 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs
+-rw-r--r--   0     1001      123    13866 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs
+-rw-r--r--   0     1001      123       64 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/commodity/mod.rs
+-rw-r--r--   0     1001      123     3699 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs
+-rw-r--r--   0     1001      123     7432 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs
+-rw-r--r--   0     1001      123    29827 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/common.rs
+-rw-r--r--   0     1001      123     9793 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/common_curv.rs
+-rw-r--r--   0     1001      123    19318 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs
+-rw-r--r--   0     1001      123    17703 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs
+-rw-r--r--   0     1001      123       64 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_nonsec/mod.rs
+-rw-r--r--   0     1001      123     3841 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs
+-rw-r--r--   0     1001      123    11803 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs
+-rw-r--r--   0     1001      123    15617 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs
+-rw-r--r--   0     1001      123    12459 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs
+-rw-r--r--   0     1001      123       64 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/mod.rs
+-rw-r--r--   0     1001      123     2904 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs
+-rw-r--r--   0     1001      123     8782 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs
+-rw-r--r--   0     1001      123    15261 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs
+-rw-r--r--   0     1001      123    13479 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs
+-rw-r--r--   0     1001      123       64 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/mod.rs
+-rw-r--r--   0     1001      123     2988 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs
+-rw-r--r--   0     1001      123     8063 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs
+-rw-r--r--   0     1001      123    17052 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs
+-rw-r--r--   0     1001      123    10900 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/equity/delta.rs
+-rw-r--r--   0     1001      123       64 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/equity/mod.rs
+-rw-r--r--   0     1001      123     2162 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/equity/totals.rs
+-rw-r--r--   0     1001      123    10428 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/equity/vega.rs
+-rw-r--r--   0     1001      123    14289 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs
+-rw-r--r--   0     1001      123    11992 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/fx/delta.rs
+-rw-r--r--   0     1001      123       64 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/fx/mod.rs
+-rw-r--r--   0     1001      123     2162 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/fx/totals.rs
+-rw-r--r--   0     1001      123    10166 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/fx/vega.rs
+-rw-r--r--   0     1001      123    14030 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs
+-rw-r--r--   0     1001      123    21887 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/girr/delta.rs
+-rw-r--r--   0     1001      123       64 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/girr/mod.rs
+-rw-r--r--   0     1001      123     2295 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/girr/totals.rs
+-rw-r--r--   0     1001      123    15657 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/girr/vega.rs
+-rw-r--r--   0     1001      123      221 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/mod.rs
+-rw-r--r--   0     1001      123     5170 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/totals.rs
+-rw-r--r--   0     1001      123    28643 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/statics.rs
+-rw-r--r--   0     1001      123      753 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/totals.rs
+-rw-r--r--   0     1001      123     1881 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/src/validate.rs
+-rw-r--r--   0     1001      123     1756 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/tests/common/mod.rs
+-rw-r--r--   0     1001      123     1486 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/tests/dependant.rs
+-rw-r--r--   0     1001      123     4487 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/tests/drc.rs
+-rw-r--r--   0     1001      123      420 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/tests/rrao.rs
+-rw-r--r--   0     1001      123    18903 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/tests/sbm.rs
+-rw-r--r--   0     1001      123      744 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/frtb_engine/tests/sbm_totals.rs
+-rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 ultibi-0.3.4/local_dependencies/ultibi_server/Cargo.toml
+-rw-r--r--   0     1001      123      219 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_server/build.rs
+-rw-r--r--   0     1001      123       35 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_server/src/api/mod.rs
+-rw-r--r--   0     1001      123      754 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_server/src/api/open_api.rs
+-rw-r--r--   0     1001      123     6651 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_server/src/api/routers.rs
+-rw-r--r--   0     1001      123     1264 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_server/src/app.rs
+-rw-r--r--   0     1001      123     2593 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_server/src/helpers.rs
+-rw-r--r--   0     1001      123     1432 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_server/src/lib.rs
+-rw-r--r--   0     1001      123      433 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_server/src/visual.rs
+-rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 ultibi-0.3.4/local_dependencies/ultibi/Cargo.toml
+-rw-r--r--   0     1001      123        0 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi/README.md
+-rw-r--r--   0     1001      123       73 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi/src/lib.rs
+-rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 ultibi-0.3.4/local_dependencies/ultibi_core/Cargo.toml
+-rw-r--r--   0     1001      123     2031 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/add_row.rs
+-rw-r--r--   0     1001      123     3486 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/aggregations.rs
+-rw-r--r--   0     1001      123      654 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/cache.rs
+-rw-r--r--   0     1001      123     4244 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/datarequest.rs
+-rw-r--r--   0     1001      123     9751 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/dataset.rs
+-rw-r--r--   0     1001      123     1782 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/datasource/acquire.rs
+-rw-r--r--   0     1001      123     2059 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/datasource/awss3.rs
+-rw-r--r--   0     1001      123     5329 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/datasource/helpers.rs
+-rw-r--r--   0     1001      123     7509 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/datasource/mod.rs
+-rw-r--r--   0     1001      123      700 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/errors.rs
+-rw-r--r--   0     1001      123    10956 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/execution/execute_agg.rs
+-rw-r--r--   0     1001      123     4594 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs
+-rw-r--r--   0     1001      123      464 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/execution/mod.rs
+-rw-r--r--   0     1001      123     2663 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/filters.rs
+-rw-r--r--   0     1001      123       18 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/helpers/mod.rs
+-rw-r--r--   0     1001      123      545 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/helpers/searches.rs
+-rw-r--r--   0     1001      123      375 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/lib.rs
+-rw-r--r--   0     1001      123    11996 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/measure.rs
+-rw-r--r--   0     1001      123     5459 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/overrides.rs
+-rw-r--r--   0     1001      123      230 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/prelude.rs
+-rw-r--r--   0     1001      123       64 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/reports/mod.rs
+-rw-r--r--   0     1001      123     1178 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/src/reports/report.rs
+-rw-r--r--   0     1001      123     1884 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/add_row.rs
+-rw-r--r--   0     1001      123      741 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/agg_request.rs
+-rw-r--r--   0     1001      123     1543 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/aggregations.rs
+-rw-r--r--   0     1001      123        1 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/cache.rs
+-rw-r--r--   0     1001      123     2067 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/common/mod.rs
+-rw-r--r--   0     1001      123       95 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/data/bad_config.toml
+-rw-r--r--   0     1001      123      553 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/data/bad_config2.toml
+-rw-r--r--   0     1001      123      116 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/data/test_config.toml
+-rw-r--r--   0     1001      123      354 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/data/testset.csv
+-rw-r--r--   0     1001      123     1250 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/datasource.rs
+-rw-r--r--   0     1001      123     3115 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/dependants.rs
+-rw-r--r--   0     1001      123     1485 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/filters.rs
+-rw-r--r--   0     1001      123        1 2023-06-20 17:50:17.000000 ultibi-0.3.4/local_dependencies/ultibi_core/tests/overrides.rs
+-rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 ultibi-0.3.4/Cargo.toml
+-rw-r--r--   0     1001      123      728 2023-06-20 17:50:17.000000 ultibi-0.3.4/.gitignore
+-rw-r--r--   0     1001      123     5183 2023-06-20 17:50:17.000000 ultibi-0.3.4/LICENSE
+-rw-r--r--   0     1001      123     2403 2023-06-20 17:50:17.000000 ultibi-0.3.4/Makefile
+-rw-r--r--   0     1001      123     5565 2023-06-20 17:50:17.000000 ultibi-0.3.4/README.md
+-rw-r--r--   0     1001      123     1559 2023-06-20 17:50:17.000000 ultibi-0.3.4/example.py
+-rw-r--r--   0     1001      123     2104 2023-06-20 17:50:17.000000 ultibi-0.3.4/pyproject.toml
+-rw-r--r--   0     1001      123       36 2023-06-20 17:50:17.000000 ultibi-0.3.4/requirements-lint.txt
+-rw-r--r--   0     1001      123      307 2023-06-20 17:50:17.000000 ultibi-0.3.4/requirements.txt
+-rw-r--r--   0     1001      123     3842 2023-06-20 17:50:17.000000 ultibi-0.3.4/src/calculator.rs
+-rw-r--r--   0     1001      123       48 2023-06-20 17:50:17.000000 ultibi-0.3.4/src/conversions/mod.rs
+-rw-r--r--   0     1001      123     3542 2023-06-20 17:50:17.000000 ultibi-0.3.4/src/conversions/series.rs
+-rw-r--r--   0     1001      123     3049 2023-06-20 17:50:17.000000 ultibi-0.3.4/src/conversions/wrappers.rs
+-rw-r--r--   0     1001      123     7737 2023-06-20 17:50:17.000000 ultibi-0.3.4/src/dataset.rs
+-rw-r--r--   0     1001      123     3303 2023-06-20 17:50:17.000000 ultibi-0.3.4/src/errors.rs
+-rw-r--r--   0     1001      123      693 2023-06-20 17:50:17.000000 ultibi-0.3.4/src/filter.rs
+-rw-r--r--   0     1001      123     2021 2023-06-20 17:50:17.000000 ultibi-0.3.4/src/lib.rs
+-rw-r--r--   0     1001      123     2521 2023-06-20 17:50:17.000000 ultibi-0.3.4/src/measure.rs
+-rw-r--r--   0     1001      123     1353 2023-06-20 17:50:17.000000 ultibi-0.3.4/src/requests.rs
+-rw-r--r--   0     1001      123     1762 2023-06-20 17:50:17.000000 ultibi-0.3.4/tests/data/datasource_config.toml
+-rw-r--r--   0     1001      123     4042 2023-06-20 17:50:17.000000 ultibi-0.3.4/tests/docs/run_doc_examples.py
+-rw-r--r--   0     1001      123      591 2023-06-20 17:50:17.000000 ultibi-0.3.4/tests/unit/test_compute.py
+-rw-r--r--   0     1001      123     1507 2023-06-20 17:50:17.000000 ultibi-0.3.4/tests/unit/test_ds.py
+-rw-r--r--   0     1001      123     2658 2023-06-20 17:50:17.000000 ultibi-0.3.4/tests/unit/test_measure.py
+-rw-r--r--   0     1001      123      848 2023-06-20 17:50:17.000000 ultibi-0.3.4/ultibi/__init__.py
+-rw-r--r--   0     1001      123     1060 2023-06-20 17:50:17.000000 ultibi-0.3.4/ultibi/internals/__init__.py
+-rw-r--r--   0     1001      123     6733 2023-06-20 17:50:17.000000 ultibi-0.3.4/ultibi/internals/dataset.py
+-rw-r--r--   0     1001      123     3131 2023-06-20 17:50:17.000000 ultibi-0.3.4/ultibi/internals/filters.py
+-rw-r--r--   0     1001      123     5200 2023-06-20 17:50:17.000000 ultibi-0.3.4/ultibi/internals/measure.py
+-rw-r--r--   0     1001      123     2950 2023-06-20 17:50:17.000000 ultibi-0.3.4/ultibi/internals/requests.py
+-rw-r--r--   0     1001      123        0 2023-06-20 17:50:17.000000 ultibi-0.3.4/ultibi/rust_module/__init__.py
+-rw-r--r--   0        0        0   100635 2023-06-20 17:54:29.000000 ultibi-0.3.4/Cargo.lock
+-rw-r--r--   0        0        0     6488 1970-01-01 00:00:00.000000 ultibi-0.3.4/PKG-INFO
```

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_server/Cargo.toml` & `ultibi-0.3.4/local_dependencies/ultibi_server/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ultibi_server"
-version= "0.3.3"
+version= "0.3.4"
 edition = "2021"
 publish = true
 license-file= "LICENSE"
 description= "Ultibi is a BI tool for no code data analysis"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_server/src/api/open_api.rs` & `ultibi-0.3.4/local_dependencies/ultibi_server/src/api/open_api.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_server/src/api/routers.rs` & `ultibi-0.3.4/local_dependencies/ultibi_server/src/api/routers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_server/src/app.rs` & `ultibi-0.3.4/local_dependencies/ultibi_server/src/app.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_server/src/helpers.rs` & `ultibi-0.3.4/local_dependencies/ultibi_server/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_server/src/lib.rs` & `ultibi-0.3.4/local_dependencies/ultibi_server/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/Cargo.toml` & `ultibi-0.3.4/local_dependencies/ultibi_core/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ultibi_core"
-version= "0.3.3"
+version= "0.3.4"
 edition = "2021"
 publish = true
 license-file= "LICENSE"
 description= "Ultibi is a BI tool for no code data analysis"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
```

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/src/add_row.rs` & `ultibi-0.3.4/local_dependencies/ultibi_core/src/add_row.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/src/aggregations.rs` & `ultibi-0.3.4/local_dependencies/ultibi_core/src/aggregations.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/src/cache.rs` & `ultibi-0.3.4/local_dependencies/ultibi_core/src/cache.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/src/datarequest.rs` & `ultibi-0.3.4/local_dependencies/ultibi_core/src/datarequest.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/src/dataset.rs` & `ultibi-0.3.4/local_dependencies/ultibi_core/src/dataset.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/src/datasource/acquire.rs` & `ultibi-0.3.4/local_dependencies/ultibi_core/src/datasource/acquire.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/src/datasource/awss3.rs` & `ultibi-0.3.4/local_dependencies/ultibi_core/src/datasource/awss3.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/src/datasource/helpers.rs` & `ultibi-0.3.4/local_dependencies/ultibi_core/src/datasource/helpers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/src/datasource/mod.rs` & `ultibi-0.3.4/local_dependencies/ultibi_core/src/datasource/mod.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/src/errors.rs` & `ultibi-0.3.4/local_dependencies/ultibi_core/src/errors.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/src/execution/execute_agg.rs` & `ultibi-0.3.4/local_dependencies/ultibi_core/src/execution/execute_agg.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs` & `ultibi-0.3.4/local_dependencies/ultibi_core/src/execution/execute_agg_with_cache.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/src/filters.rs` & `ultibi-0.3.4/local_dependencies/ultibi_core/src/filters.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/src/helpers/searches.rs` & `ultibi-0.3.4/local_dependencies/ultibi_core/src/helpers/searches.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/src/measure.rs` & `ultibi-0.3.4/local_dependencies/ultibi_core/src/measure.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/src/overrides.rs` & `ultibi-0.3.4/local_dependencies/ultibi_core/src/overrides.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/src/reports/report.rs` & `ultibi-0.3.4/local_dependencies/ultibi_core/src/reports/report.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/tests/add_row.rs` & `ultibi-0.3.4/local_dependencies/ultibi_core/tests/add_row.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/tests/agg_request.rs` & `ultibi-0.3.4/local_dependencies/ultibi_core/tests/agg_request.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/tests/aggregations.rs` & `ultibi-0.3.4/local_dependencies/ultibi_core/tests/aggregations.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/tests/common/mod.rs` & `ultibi-0.3.4/local_dependencies/ultibi_core/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/tests/data/bad_config2.toml` & `ultibi-0.3.4/local_dependencies/ultibi_core/tests/data/bad_config2.toml`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/tests/datasource.rs` & `ultibi-0.3.4/local_dependencies/ultibi_core/tests/datasource.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/tests/dependants.rs` & `ultibi-0.3.4/local_dependencies/ultibi_core/tests/dependants.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/ultibi_core/tests/filters.rs` & `ultibi-0.3.4/local_dependencies/ultibi_core/tests/filters.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/Cargo.toml` & `ultibi-0.3.4/local_dependencies/frtb_engine/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "frtb_engine"
-version= "0.3.3"
+version= "0.3.4"
 edition = "2021"
 publish = false
 license-file= "LICENSE"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
```

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/data/frtb/Delta.csv` & `ultibi-0.3.4/local_dependencies/frtb_engine/data/frtb/Delta.csv`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv` & `ultibi-0.3.4/local_dependencies/frtb_engine/data/frtb/TradeAttributes.csv`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/data/frtb/datasource_config.toml` & `ultibi-0.3.4/local_dependencies/frtb_engine/data/frtb/datasource_config.toml`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/calc_params.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/calc_params.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/docs/optional_params.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/docs/optional_params.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/drc/common.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/drc/common.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/drc/drc_nonsec.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/drc/drc_secnonctp.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/drc/drc_weights.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/drc/drc_weights.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/drc/totals.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/drc/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/helpers.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/lib.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/measures.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/measures.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/risk_weights.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/risk_weights.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/risk_weights_crr2.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/risk_weights_crr2.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/rrao/mod.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/rrao/mod.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/buckets.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/buckets.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/commodity/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/commodity/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/commodity/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/commodity/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/common.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/common.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/common_curv.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/common_curv.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_nonsec/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_nonsec/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_nonsec/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_nonsec/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_ctp/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/csr_sec_nonctp/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/equity/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/equity/delta.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/equity/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/equity/totals.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/equity/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/equity/vega.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/equity/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/fx/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/fx/delta.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/fx/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/fx/totals.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/fx/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/fx/vega.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/fx/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/girr/curvature.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/girr/delta.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/girr/delta.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/girr/totals.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/girr/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/girr/vega.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/girr/vega.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/sbm/totals.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/sbm/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/statics.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/statics.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/totals.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/src/validate.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/src/validate.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/tests/common/mod.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/tests/dependant.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/tests/dependant.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/tests/drc.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/tests/drc.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/tests/sbm.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/tests/sbm.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/local_dependencies/frtb_engine/tests/sbm_totals.rs` & `ultibi-0.3.4/local_dependencies/frtb_engine/tests/sbm_totals.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/Cargo.toml` & `ultibi-0.3.4/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyultima"
-version= "0.3.3"
+version= "0.3.4"
 edition = "2021"
 publish = false
 repository= "https://github.com/ultima-ib/ultima/"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "ultibi"
```

### Comparing `ultibi-0.3.3/.gitignore` & `ultibi-0.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/LICENSE` & `ultibi-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/Makefile` & `ultibi-0.3.4/Makefile`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/README.md` & `ultibi-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/example.py` & `ultibi-0.3.4/example.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/pyproject.toml` & `ultibi-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/src/calculator.rs` & `ultibi-0.3.4/src/calculator.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/src/conversions/series.rs` & `ultibi-0.3.4/src/conversions/series.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/src/conversions/wrappers.rs` & `ultibi-0.3.4/src/conversions/wrappers.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/src/dataset.rs` & `ultibi-0.3.4/src/dataset.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/src/errors.rs` & `ultibi-0.3.4/src/errors.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/src/filter.rs` & `ultibi-0.3.4/src/filter.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/src/lib.rs` & `ultibi-0.3.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/src/measure.rs` & `ultibi-0.3.4/src/measure.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/src/requests.rs` & `ultibi-0.3.4/src/requests.rs`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/tests/data/datasource_config.toml` & `ultibi-0.3.4/tests/data/datasource_config.toml`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/tests/docs/run_doc_examples.py` & `ultibi-0.3.4/tests/docs/run_doc_examples.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/tests/unit/test_compute.py` & `ultibi-0.3.4/tests/unit/test_compute.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/tests/unit/test_ds.py` & `ultibi-0.3.4/tests/unit/test_ds.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/tests/unit/test_measure.py` & `ultibi-0.3.4/tests/unit/test_measure.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/ultibi/__init__.py` & `ultibi-0.3.4/ultibi/__init__.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/ultibi/internals/__init__.py` & `ultibi-0.3.4/ultibi/internals/__init__.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/ultibi/internals/dataset.py` & `ultibi-0.3.4/ultibi/internals/dataset.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/ultibi/internals/filters.py` & `ultibi-0.3.4/ultibi/internals/filters.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/ultibi/internals/measure.py` & `ultibi-0.3.4/ultibi/internals/measure.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/ultibi/internals/requests.py` & `ultibi-0.3.4/ultibi/internals/requests.py`

 * *Files identical despite different names*

### Comparing `ultibi-0.3.3/Cargo.lock` & `ultibi-0.3.4/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -939,28 +939,28 @@
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
 name = "clap"
-version = "4.3.3"
+version = "4.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca8f255e4b8027970e78db75e78831229c9815fdbfa67eb1a1b777a62e24b4a0"
+checksum = "2686c4115cb0810d9a984776e197823d08ec94f176549a89a9efded477c456dc"
 dependencies = [
  "clap_builder",
  "clap_derive",
  "once_cell",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.3.3"
+version = "4.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "acd4f3c17c83b0ba34ffbc4f8bbd74f079413f747f84a6f89292f138057e36ab"
+checksum = "2e53afce1efce6ed1f633cf0e57612fe51db54a1ee4fd8f8503d078fe02d69ae"
 dependencies = [
  "anstream",
  "anstyle",
  "bitflags",
  "clap_lex",
  "strsim",
 ]
@@ -1032,17 +1032,17 @@
 name = "core-foundation-sys"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.7"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
+checksum = "03e69e28e9f7f77debdedbaafa2866e1de9ba56df55a8bd7cfc724c25a09987c"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32c"
 version = "0.6.3"
@@ -1080,30 +1080,30 @@
  "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.14"
+version = "0.9.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46bd5f3f85273295a9d14aedfb86f6aadbff6d8f5295c4a9edb08e819dcf5695"
+checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "memoffset 0.8.0",
+ "memoffset",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.15"
+version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
+checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crossterm"
 version = "0.26.1"
@@ -1118,17 +1118,17 @@
  "signal-hook",
  "signal-hook-mio",
  "winapi",
 ]
 
 [[package]]
 name = "crossterm_winapi"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2ae1b35a484aa10e07fe0638d02301c5ad24de82d310ccbd2f3693da5f09bf1c"
+checksum = "acdd7c62a3665c7f6830a51635d9ac9b23ed385797f70a83bb8bafe9c572ab2b"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "crypto-common"
 version = "0.1.6"
@@ -1353,15 +1353,15 @@
 checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "frtb_engine"
-version = "0.3.3"
+version = "0.3.4"
 dependencies = [
  "log",
  "ndarray",
  "once_cell",
  "polars",
  "rayon",
  "serde",
@@ -1797,17 +1797,17 @@
 checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
-version = "0.3.63"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2f37a4a5928311ac501dee68b3c7613a1037d0edb30c8e5427bd832d55d1b790"
+checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "language-tags"
 version = "0.3.2"
@@ -1947,17 +1947,17 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.18"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "lz4"
 version = "1.24.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e9e2dd86df36ce760a60f6ff6ad526f7ba1f14ba0356f8254fb6905e6494df1"
 dependencies = [
@@ -2010,23 +2010,14 @@
 checksum = "83faa42c0a078c393f6b29d5db232d8be22776a891f8f56e5284faee4a20b327"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
-dependencies = [
- "autocfg",
-]
-
-[[package]]
-name = "memoffset"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
@@ -2640,15 +2631,15 @@
 version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
- "memoffset 0.9.0",
+ "memoffset",
  "parking_lot 0.12.1",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
@@ -2693,15 +2684,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyultima"
-version = "0.3.3"
+version = "0.3.4"
 dependencies = [
  "ciborium",
  "frtb_engine",
  "once_cell",
  "polars",
  "polars-arrow",
  "pyo3",
@@ -2933,17 +2924,17 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.37.19"
+version = "0.37.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
+checksum = "b96e891d04aa506a6d1f318d2771bcb1c7dfda84e126660ace067c9b474bb2c0"
 dependencies = [
  "bitflags",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.48.0",
@@ -3067,17 +3058,17 @@
  "proc-macro2",
  "quote",
  "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.96"
+version = "1.0.97"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
+checksum = "bdf3bf93142acad5821c99197022e170842cdbc1c30482b98750c688c640842a"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -3110,17 +3101,17 @@
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
 name = "sha2"
-version = "0.10.6"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
+checksum = "479fb9d862239e610720565ca91403019f2f00410f1864c5aa7479b950a76ed8"
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
@@ -3322,15 +3313,15 @@
  "redox_syscall 0.3.5",
  "rustix",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "template_drivers"
-version = "0.3.3"
+version = "0.3.4"
 dependencies = [
  "actix-files",
  "actix-web",
  "actix-web-httpauth",
  "actix-web-static-files",
  "anyhow",
  "clap",
@@ -3592,17 +3583,17 @@
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.24"
+version = "0.1.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
+checksum = "8803eee176538f94ae9a14b55b2804eb7e1441f8210b1c31290b3bccdccff73b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.18",
 ]
 
 [[package]]
@@ -3624,23 +3615,23 @@
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "ultibi"
-version = "0.3.3"
+version = "0.3.4"
 dependencies = [
  "ultibi_core",
  "ultibi_server",
 ]
 
 [[package]]
 name = "ultibi_core"
-version = "0.3.3"
+version = "0.3.4"
 dependencies = [
  "aws-config",
  "aws-sdk-s3",
  "dashmap",
  "derivative",
  "futures",
  "once_cell",
@@ -3652,15 +3643,15 @@
  "tokio",
  "toml",
  "utoipa",
 ]
 
 [[package]]
 name = "ultibi_server"
-version = "0.3.3"
+version = "0.3.4"
 dependencies = [
  "actix-web",
  "actix-web-static-files",
  "anyhow",
  "dotenv",
  "log",
  "mime",
@@ -3745,55 +3736,55 @@
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "utoipa"
 version = "3.3.0"
-source = "git+https://github.com/juhaku/utoipa#f8c6d07ef699d4fd6d3eeddfb55d6955d89af0f6"
+source = "git+https://github.com/juhaku/utoipa#1774bb708c15dafcf34f28c0ec8b5b093dece7a9"
 dependencies = [
  "indexmap",
  "serde",
  "serde_json",
  "utoipa-gen",
 ]
 
 [[package]]
 name = "utoipa-gen"
 version = "3.3.0"
-source = "git+https://github.com/juhaku/utoipa#f8c6d07ef699d4fd6d3eeddfb55d6955d89af0f6"
+source = "git+https://github.com/juhaku/utoipa#1774bb708c15dafcf34f28c0ec8b5b093dece7a9"
 dependencies = [
  "lazy_static",
  "proc-macro-error",
  "proc-macro2",
  "quote",
  "regex",
  "syn 2.0.18",
 ]
 
 [[package]]
 name = "utoipa-swagger-ui"
 version = "3.1.3"
-source = "git+https://github.com/juhaku/utoipa#f8c6d07ef699d4fd6d3eeddfb55d6955d89af0f6"
+source = "git+https://github.com/juhaku/utoipa#1774bb708c15dafcf34f28c0ec8b5b093dece7a9"
 dependencies = [
  "actix-web",
  "mime_guess",
  "regex",
  "rust-embed",
  "serde",
  "serde_json",
  "utoipa",
  "zip",
 ]
 
 [[package]]
 name = "uuid"
-version = "1.3.3"
+version = "1.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "345444e32442451b267fc254ae85a209c64be56d2890e601a0c37ff0c3c5ecd2"
+checksum = "0fa2982af2eec27de306107c027578ff7f423d65f7250e40ce0fea8f45248b81"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "vcpkg"
 version = "0.2.15"
@@ -3814,19 +3805,18 @@
 dependencies = [
  "same-file",
  "winapi-util",
 ]
 
 [[package]]
 name = "want"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ce8a968cb1cd110d136ff8b819a556d6fb6d919363c61534f6860c7eb172ba0"
+checksum = "bfa7760aed19e106de2c7c0b581b509f2f25d3dacaf737cb82ac61bc6d760b0e"
 dependencies = [
- "log",
  "try-lock",
 ]
 
 [[package]]
 name = "wasi"
 version = "0.10.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -3836,77 +3826,77 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5bba0e8cb82ba49ff4e229459ff22a191bbe9a1cb3a341610c9c33efc27ddf73"
+checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "19b04bc93f9d6bdee709f6bd2118f57dd6679cf1176a1af464fca3ab0d66d8fb"
+checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
  "syn 2.0.18",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.36"
+version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2d1985d03709c53167ce907ff394f5316aa22cb4e12761295c5dc57dacb6297e"
+checksum = "c02dbc21516f9f1f04f187958890d7e6026df8d16540b7ad9492bc34a67cea03"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14d6b024f1a526bb0234f52840389927257beb670610081360e5a03c5df9c258"
+checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e128beba882dd1eb6200e1dc92ae6c5dbaa4311aa7bb211ca035779e5efc39f8"
+checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.18",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed9d5b4305409d1fc9482fee2d7f9bcbf24b3972bf59817ef757e23982242a93"
+checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
 
 [[package]]
 name = "wasm-timer"
 version = "0.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be0ecb0db480561e9a7642b5d3e4187c128914e58aa84330b9493e3eb68c5e7f"
 dependencies = [
@@ -3917,17 +3907,17 @@
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
 ]
 
 [[package]]
 name = "web-sys"
-version = "0.3.63"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3bdd9ef4e984da1187bf8110c5cf5b845fbc87a23602cdf912386a76fcd3a7c2"
+checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "webpki"
@@ -4100,17 +4090,17 @@
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "winnow"
-version = "0.4.6"
+version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61de7bac303dc551fe038e2b3cef0f571087a47571ea6e79a87692ac99b99699"
+checksum = "ca0ace3845f0d96209f0375e6d367e3eb87eb65d27d445bdc9f1843a26f39448"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winreg"
 version = "0.10.1"
```

### Comparing `ultibi-0.3.3/PKG-INFO` & `ultibi-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultibi
-Version: 0.3.3
+Version: 0.3.4
 Classifier: Programming Language :: Rust
 Classifier: License :: Free for non-commercial use
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,17 +12,17 @@
 Requires-Dist: pyarrow
 License-File: LICENSE
 Summary: Flexible DataFrame Operations via UI
 Keywords: dataframe,visualization,aggregation,calculation,chart,data,dataviz,pivot-table,frtb,risk
 Author-email: Anatoly Bugakov <anatoly@ultimabi.uk>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Homepage, https://ultimabi.uk/
 Project-URL: Repository, https://github.com/ultima-ib/ultibi-frtb-book
 Project-URL: Documentation, https://ultimabi.uk/ultibi-frtb-book/
-Project-URL: Homepage, https://ultimabi.uk/
 
 <br>
 
 <p align="center">
     <a href="https://ultimabi.uk/" target="_blank">
     <img width="900" src="https://ultima-bi.s3.eu-west-2.amazonaws.com/imgs/logo.png" alt="Ultima Logo">
     </a>
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: ultibi Version: 0.3.3 Classifier: Programming
+Metadata-Version: 2.1 Name: ultibi Version: 0.3.4 Classifier: Programming
 Language :: Rust Classifier: License :: Free for non-commercial use Classifier:
 Topic :: Scientific/Engineering Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: polars Requires-Dist: pyarrow License-File: LICENSE Summary:
 Flexible DataFrame Operations via UI Keywords:
 dataframe,visualization,aggregation,calculation,chart,data,dataviz,pivot-
 table,frtb,risk Author-email: Anatoly Bugakov
 ultimabi.uk> Requires-Python: >=3.7 Description-Content-Type: text/markdown;
-charset=UTF-8; variant=GFM Project-URL: Repository, https://github.com/ultima-
-ib/ultibi-frtb-book Project-URL: Documentation, https://ultimabi.uk/ultibi-
-frtb-book/ Project-URL: Homepage, https://ultimabi.uk/
+charset=UTF-8; variant=GFM Project-URL: Homepage, https://ultimabi.uk/ Project-
+URL: Repository, https://github.com/ultima-ib/ultibi-frtb-book Project-URL:
+Documentation, https://ultimabi.uk/ultibi-frtb-book/
                                  [Ultima_Logo]
 
                     **** the ultimate data analytics tool
          for no code visualisation and collaborative exploration. ****
          **** Present easier.   Dig deeper.   Review together.   ****
 # The Ultimate BI tool With `Ultibi` you can turn your `DataFrame` into a pivot
 table with a UI and share it across organisation. You can also define measures
```

