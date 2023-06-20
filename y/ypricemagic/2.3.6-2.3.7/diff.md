# Comparing `tmp/ypricemagic-2.3.6.tar.gz` & `tmp/ypricemagic-2.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ypricemagic-2.3.6.tar", last modified: Mon Jun 19 14:23:51 2023, max compression
+gzip compressed data, was "ypricemagic-2.3.7.tar", last modified: Tue Jun 20 14:03:21 2023, max compression
```

## Comparing `ypricemagic-2.3.6.tar` & `ypricemagic-2.3.7.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.030897 ypricemagic-2.3.6/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/.env.sample
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.018897 ypricemagic-2.3.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.022897 ypricemagic-2.3.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3229 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-06-19 14:23:51.030897 ypricemagic-2.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      776 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-19 14:23:51.030897 ypricemagic-2.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.022897 ypricemagic-2.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.022897 ypricemagic-2.3.6/tests/classes/
--rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/tests/classes/test_erc20.py
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/tests/classes/test_singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.022897 ypricemagic-2.3.6/tests/prices/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/tests/prices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.022897 ypricemagic-2.3.6/tests/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/tests/prices/dex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/tests/prices/dex/test_balancer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/tests/prices/dex/test_uniswap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.022897 ypricemagic-2.3.6/tests/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/tests/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6458 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/tests/prices/lending/test_aave.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/tests/prices/lending/test_compound.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.022897 ypricemagic-2.3.6/tests/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/tests/prices/stable_swap/test_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/tests/prices/test_chainlink.py
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/tests/prices/test_gearbox.py
--rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/tests/prices/test_magic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/tests/prices/test_popsicle.py
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/tests/prices/test_synthetix.py
--rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/tests/prices/test_yearn.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.022897 ypricemagic-2.3.6/tests/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/tests/prices/tokenized_fund/test_piedao.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.022897 ypricemagic-2.3.6/tests/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/tests/prices/utils/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/tests/test_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.022897 ypricemagic-2.3.6/y/
--rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.022897 ypricemagic-2.3.6/y/classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7773 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/classes/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/classes/singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)    10017 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    20162 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/contracts.py
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/convert.py
--rw-r--r--   0 runner    (1001) docker     (122)      576 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/erc20.py
--rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.022897 ypricemagic-2.3.6/y/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)     6400 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/interfaces/ERC20.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.022897 ypricemagic-2.3.6/y/interfaces/balancer/
--rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/interfaces/balancer/WeightedPool.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/interfaces/balancer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.026897 ypricemagic-2.3.6/y/interfaces/compound/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/interfaces/compound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32517 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/interfaces/compound/unitroller.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.026897 ypricemagic-2.3.6/y/interfaces/curve/
--rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/interfaces/curve/CurveRegistry.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/interfaces/curve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/interfaces/multicall2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.026897 ypricemagic-2.3.6/y/interfaces/uniswap/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/interfaces/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/interfaces/uniswap/factoryv2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/interfaces/uniswap/quoterv3.py
--rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/networks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.026897 ypricemagic-2.3.6/y/prices/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/band.py
--rw-r--r--   0 runner    (1001) docker     (122)    19868 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/chainlink.py
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/convex.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.026897 ypricemagic-2.3.6/y/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/dex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.026897 ypricemagic-2.3.6/y/prices/dex/balancer/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/dex/balancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/dex/balancer/balancer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6669 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/dex/balancer/v1.py
--rw-r--r--   0 runner    (1001) docker     (122)    10744 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/dex/balancer/v2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/dex/genericamm.py
--rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/dex/mooniswap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.026897 ypricemagic-2.3.6/y/prices/dex/uniswap/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/dex/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6370 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/dex/uniswap/uniswap.py
--rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/dex/uniswap/v1.py
--rw-r--r--   0 runner    (1001) docker     (122)    23293 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/dex/uniswap/v2.py
--rw-r--r--   0 runner    (1001) docker     (122)    12588 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/dex/uniswap/v2_forks.py
--rw-r--r--   0 runner    (1001) docker     (122)     3949 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/dex/uniswap/v3.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.026897 ypricemagic-2.3.6/y/prices/eth_derivs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/eth_derivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/eth_derivs/creth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/eth_derivs/wsteth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2940 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/gearbox.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.026897 ypricemagic-2.3.6/y/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6880 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/lending/aave.py
--rw-r--r--   0 runner    (1001) docker     (122)    10528 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/lending/compound.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/lending/ib.py
--rw-r--r--   0 runner    (1001) docker     (122)    11264 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/magic.py
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/one_to_one.py
--rw-r--r--   0 runner    (1001) docker     (122)     2490 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/popsicle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.026897 ypricemagic-2.3.6/y/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/stable_swap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/stable_swap/belt.py
--rw-r--r--   0 runner    (1001) docker     (122)    22296 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/stable_swap/curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/stable_swap/ellipsis.py
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/stable_swap/froyo.py
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/stable_swap/mstablefeederpool.py
--rw-r--r--   0 runner    (1001) docker     (122)     3259 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/stable_swap/saddle.py
--rw-r--r--   0 runner    (1001) docker     (122)     3887 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/synthetix.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.026897 ypricemagic-2.3.6/y/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/tokenized_fund/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/tokenized_fund/basketdao.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/tokenized_fund/gelato.py
--rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/tokenized_fund/piedao.py
--rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/tokenized_fund/tokensets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.030897 ypricemagic-2.3.6/y/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4650 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/utils/buckets.py
--rw-r--r--   0 runner    (1001) docker     (122)     8555 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/utils/sense_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     8174 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/utils/ypriceapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     5853 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/prices/yearn.py
--rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.030897 ypricemagic-2.3.6/y/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/utils/client.py
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/utils/dank_mids.py
--rw-r--r--   0 runner    (1001) docker     (122)     7970 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/utils/events.py
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/utils/fakes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/utils/middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)    11228 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/utils/multicall.py
--rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/y/utils/raw_calls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.030897 ypricemagic-2.3.6/ypricemagic/
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/ypricemagic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-06-19 14:23:40.000000 ypricemagic-2.3.6/ypricemagic/magic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:23:51.030897 ypricemagic-2.3.6/ypricemagic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-06-19 14:23:50.000000 ypricemagic-2.3.6/ypricemagic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-06-19 14:23:50.000000 ypricemagic-2.3.6/ypricemagic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-19 14:23:50.000000 ypricemagic-2.3.6/ypricemagic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-06-19 14:23:50.000000 ypricemagic-2.3.6/ypricemagic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-19 14:23:50.000000 ypricemagic-2.3.6/ypricemagic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.815879 ypricemagic-2.3.7/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/.env.sample
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.803879 ypricemagic-2.3.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3229 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-06-20 14:03:21.815879 ypricemagic-2.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      776 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-20 14:03:21.815879 ypricemagic-2.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/tests/classes/
+-rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/classes/test_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/classes/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/tests/prices/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/tests/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/dex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/dex/test_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/dex/test_uniswap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/tests/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6458 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/lending/test_aave.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/lending/test_compound.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/tests/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/stable_swap/test_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/test_chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/test_gearbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/test_magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/test_popsicle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/test_synthetix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/test_yearn.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/tests/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/tokenized_fund/test_piedao.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/tests/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/utils/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/test_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/y/
+-rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/y/classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7773 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/classes/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/classes/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10017 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20385 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      576 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/erc20.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/y/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     6400 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/interfaces/ERC20.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/y/interfaces/balancer/
+-rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/interfaces/balancer/WeightedPool.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/interfaces/balancer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/y/interfaces/compound/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/interfaces/compound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32517 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/interfaces/compound/unitroller.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/y/interfaces/curve/
+-rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/interfaces/curve/CurveRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/interfaces/curve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/interfaces/multicall2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.811879 ypricemagic-2.3.7/y/interfaces/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/interfaces/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/interfaces/uniswap/factoryv2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/interfaces/uniswap/quoterv3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/networks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.811879 ypricemagic-2.3.7/y/prices/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/band.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19868 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/convex.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.811879 ypricemagic-2.3.7/y/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.811879 ypricemagic-2.3.7/y/prices/dex/balancer/
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/balancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/balancer/balancer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6669 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/balancer/v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10744 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/balancer/v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/genericamm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/mooniswap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.811879 ypricemagic-2.3.7/y/prices/dex/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6370 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/uniswap/uniswap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/uniswap/v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23293 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/uniswap/v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12588 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/uniswap/v2_forks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3949 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/uniswap/v3.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.811879 ypricemagic-2.3.7/y/prices/eth_derivs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/eth_derivs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/eth_derivs/creth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/eth_derivs/wsteth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2940 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/gearbox.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.811879 ypricemagic-2.3.7/y/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6880 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/lending/aave.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10528 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/lending/compound.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/lending/ib.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11264 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/one_to_one.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2490 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/popsicle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.811879 ypricemagic-2.3.7/y/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/stable_swap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/stable_swap/belt.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22296 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/stable_swap/curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/stable_swap/ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/stable_swap/froyo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/stable_swap/mstablefeederpool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3259 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/stable_swap/saddle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3887 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.811879 ypricemagic-2.3.7/y/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/tokenized_fund/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/tokenized_fund/basketdao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/tokenized_fund/gelato.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/tokenized_fund/piedao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/tokenized_fund/tokensets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.815879 ypricemagic-2.3.7/y/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4650 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/utils/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8555 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/utils/sense_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8174 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/utils/ypriceapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5853 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/yearn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.815879 ypricemagic-2.3.7/y/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/utils/dank_mids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7970 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/utils/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/utils/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/utils/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11228 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/utils/multicall.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/utils/raw_calls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.815879 ypricemagic-2.3.7/ypricemagic/
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/ypricemagic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/ypricemagic/magic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.815879 ypricemagic-2.3.7/ypricemagic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-06-20 14:03:21.000000 ypricemagic-2.3.7/ypricemagic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-06-20 14:03:21.000000 ypricemagic-2.3.7/ypricemagic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-20 14:03:21.000000 ypricemagic-2.3.7/ypricemagic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-06-20 14:03:21.000000 ypricemagic-2.3.7/ypricemagic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-20 14:03:21.000000 ypricemagic-2.3.7/ypricemagic.egg-info/top_level.txt
```

### Comparing `ypricemagic-2.3.6/.github/workflows/codeql-analysis.yml` & `ypricemagic-2.3.7/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/.github/workflows/pytest.yaml` & `ypricemagic-2.3.7/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/.github/workflows/release.yaml` & `ypricemagic-2.3.7/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/LICENSE.txt` & `ypricemagic-2.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/README.md` & `ypricemagic-2.3.7/README.md`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/setup.py` & `ypricemagic-2.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/tests/classes/test_erc20.py` & `ypricemagic-2.3.7/tests/classes/test_erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/tests/classes/test_singleton.py` & `ypricemagic-2.3.7/tests/classes/test_singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/tests/fixtures.py` & `ypricemagic-2.3.7/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/tests/prices/dex/test_uniswap.py` & `ypricemagic-2.3.7/tests/prices/dex/test_uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/tests/prices/lending/test_aave.py` & `ypricemagic-2.3.7/tests/prices/lending/test_aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/tests/prices/lending/test_compound.py` & `ypricemagic-2.3.7/tests/prices/lending/test_compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/tests/prices/test_chainlink.py` & `ypricemagic-2.3.7/tests/prices/test_chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/tests/prices/test_magic.py` & `ypricemagic-2.3.7/tests/prices/test_magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/tests/prices/test_popsicle.py` & `ypricemagic-2.3.7/tests/prices/test_popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/tests/prices/test_synthetix.py` & `ypricemagic-2.3.7/tests/prices/test_synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/tests/prices/test_yearn.py` & `ypricemagic-2.3.7/tests/prices/test_yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/tests/prices/utils/test_buckets.py` & `ypricemagic-2.3.7/tests/prices/utils/test_buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/__init__.py` & `ypricemagic-2.3.7/y/__init__.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/classes/common.py` & `ypricemagic-2.3.7/y/classes/common.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/classes/singleton.py` & `ypricemagic-2.3.7/y/classes/singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/constants.py` & `ypricemagic-2.3.7/y/constants.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/contracts.py` & `ypricemagic-2.3.7/y/contracts.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,18 @@
             raise ContractNotFound(f"{address} is not a contract.")
 
         with _contract_lock:
             # autofetch-sources: false
             # Try to fetch the contract from the local sqlite db.
             try:
                 super().__init__(address, owner=owner)
-                self.verified = True
+                try:
+                    self.verified = True
+                except AttributeError:
+                    logger.warning(f'`Contract("{address}").verified` property will not be usable due to the contract having a `verified` method in its ABI.')
             # This error happens on occasion, it comes from brownie's compiling process. But we shoulnd't be using that anyway. Check config.
             except IndexError as e:
                 if str(e) == "pop from an empty deque":
                     raise CompilerError("y.Contract objects work best when we bypass compilers. In this case, it will *only* work when we bypass. Please ensure autofetch_sources=False in your brownie-config.yaml and rerun your script.")
                 raise e
             # If we don't already have the contract in the db, we'll try to fetch it from the explorer.
             except ValueError as e:
```

### Comparing `ypricemagic-2.3.6/y/datatypes.py` & `ypricemagic-2.3.7/y/datatypes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/decorators.py` & `ypricemagic-2.3.7/y/decorators.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/erc20.py` & `ypricemagic-2.3.7/y/erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/exceptions.py` & `ypricemagic-2.3.7/y/exceptions.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/interfaces/ERC20.py` & `ypricemagic-2.3.7/y/interfaces/ERC20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/interfaces/balancer/WeightedPool.py` & `ypricemagic-2.3.7/y/interfaces/balancer/WeightedPool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/interfaces/compound/unitroller.py` & `ypricemagic-2.3.7/y/interfaces/compound/unitroller.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/interfaces/curve/CurveRegistry.py` & `ypricemagic-2.3.7/y/interfaces/curve/CurveRegistry.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/interfaces/multicall2.py` & `ypricemagic-2.3.7/y/interfaces/multicall2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/interfaces/uniswap/factoryv2.py` & `ypricemagic-2.3.7/y/interfaces/uniswap/factoryv2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/interfaces/uniswap/quoterv3.py` & `ypricemagic-2.3.7/y/interfaces/uniswap/quoterv3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/networks.py` & `ypricemagic-2.3.7/y/networks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/band.py` & `ypricemagic-2.3.7/y/prices/band.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/chainlink.py` & `ypricemagic-2.3.7/y/prices/chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/convex.py` & `ypricemagic-2.3.7/y/prices/convex.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/dex/balancer/balancer.py` & `ypricemagic-2.3.7/y/prices/dex/balancer/balancer.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/dex/balancer/v1.py` & `ypricemagic-2.3.7/y/prices/dex/balancer/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/dex/balancer/v2.py` & `ypricemagic-2.3.7/y/prices/dex/balancer/v2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/dex/genericamm.py` & `ypricemagic-2.3.7/y/prices/dex/genericamm.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/dex/mooniswap.py` & `ypricemagic-2.3.7/y/prices/dex/mooniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/dex/uniswap/uniswap.py` & `ypricemagic-2.3.7/y/prices/dex/uniswap/uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/dex/uniswap/v1.py` & `ypricemagic-2.3.7/y/prices/dex/uniswap/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/dex/uniswap/v2.py` & `ypricemagic-2.3.7/y/prices/dex/uniswap/v2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/dex/uniswap/v2_forks.py` & `ypricemagic-2.3.7/y/prices/dex/uniswap/v2_forks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/dex/uniswap/v3.py` & `ypricemagic-2.3.7/y/prices/dex/uniswap/v3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/eth_derivs/creth.py` & `ypricemagic-2.3.7/y/prices/eth_derivs/creth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/eth_derivs/wsteth.py` & `ypricemagic-2.3.7/y/prices/eth_derivs/wsteth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/gearbox.py` & `ypricemagic-2.3.7/y/prices/gearbox.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/lending/aave.py` & `ypricemagic-2.3.7/y/prices/lending/aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/lending/compound.py` & `ypricemagic-2.3.7/y/prices/lending/compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/lending/ib.py` & `ypricemagic-2.3.7/y/prices/lending/ib.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/magic.py` & `ypricemagic-2.3.7/y/prices/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/one_to_one.py` & `ypricemagic-2.3.7/y/prices/one_to_one.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/popsicle.py` & `ypricemagic-2.3.7/y/prices/popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/stable_swap/belt.py` & `ypricemagic-2.3.7/y/prices/stable_swap/belt.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/stable_swap/curve.py` & `ypricemagic-2.3.7/y/prices/stable_swap/curve.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/stable_swap/ellipsis.py` & `ypricemagic-2.3.7/y/prices/stable_swap/ellipsis.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/stable_swap/froyo.py` & `ypricemagic-2.3.7/y/prices/stable_swap/froyo.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/stable_swap/mstablefeederpool.py` & `ypricemagic-2.3.7/y/prices/stable_swap/mstablefeederpool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/stable_swap/saddle.py` & `ypricemagic-2.3.7/y/prices/stable_swap/saddle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/synthetix.py` & `ypricemagic-2.3.7/y/prices/synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/tokenized_fund/basketdao.py` & `ypricemagic-2.3.7/y/prices/tokenized_fund/basketdao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/tokenized_fund/gelato.py` & `ypricemagic-2.3.7/y/prices/tokenized_fund/gelato.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/tokenized_fund/piedao.py` & `ypricemagic-2.3.7/y/prices/tokenized_fund/piedao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/tokenized_fund/tokensets.py` & `ypricemagic-2.3.7/y/prices/tokenized_fund/tokensets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/utils/buckets.py` & `ypricemagic-2.3.7/y/prices/utils/buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/utils/sense_check.py` & `ypricemagic-2.3.7/y/prices/utils/sense_check.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/utils/ypriceapi.py` & `ypricemagic-2.3.7/y/prices/utils/ypriceapi.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/prices/yearn.py` & `ypricemagic-2.3.7/y/prices/yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/time.py` & `ypricemagic-2.3.7/y/time.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/utils/client.py` & `ypricemagic-2.3.7/y/utils/client.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/utils/events.py` & `ypricemagic-2.3.7/y/utils/events.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/utils/fakes.py` & `ypricemagic-2.3.7/y/utils/fakes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/utils/logging.py` & `ypricemagic-2.3.7/y/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/utils/middleware.py` & `ypricemagic-2.3.7/y/utils/middleware.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/utils/multicall.py` & `ypricemagic-2.3.7/y/utils/multicall.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/y/utils/raw_calls.py` & `ypricemagic-2.3.7/y/utils/raw_calls.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/ypricemagic/magic.py` & `ypricemagic-2.3.7/ypricemagic/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.6/ypricemagic.egg-info/SOURCES.txt` & `ypricemagic-2.3.7/ypricemagic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

