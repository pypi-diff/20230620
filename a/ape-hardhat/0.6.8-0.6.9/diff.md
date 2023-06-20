# Comparing `tmp/ape-hardhat-0.6.8.tar.gz` & `tmp/ape-hardhat-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-hardhat-0.6.8.tar", last modified: Tue Jun 13 16:30:52 2023, max compression
+gzip compressed data, was "ape-hardhat-0.6.9.tar", last modified: Tue Jun 20 21:27:43 2023, max compression
```

## Comparing `ape-hardhat-0.6.8.tar` & `ape-hardhat-0.6.9.tar`

### file list

```diff
@@ -1,137 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:30:52.686029 ape-hardhat-0.6.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:30:52.666029 ape-hardhat-0.6.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:30:52.666029 ape-hardhat-0.6.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:30:52.670029 ape-hardhat-0.6.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-13 16:30:52.686029 ape-hardhat-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:30:52.670029 ape-hardhat-0.6.8/ape_hardhat/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/ape_hardhat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/ape_hardhat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    28332 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/ape_hardhat/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/ape_hardhat/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 16:30:52.000000 ape-hardhat-0.6.8/ape_hardhat/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:30:52.670029 ape-hardhat-0.6.8/ape_hardhat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-13 16:30:52.000000 ape-hardhat-0.6.8/ape_hardhat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-06-13 16:30:52.000000 ape-hardhat-0.6.8/ape_hardhat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:30:52.000000 ape-hardhat-0.6.8/ape_hardhat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:30:52.000000 ape-hardhat-0.6.8/ape_hardhat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-13 16:30:52.000000 ape-hardhat-0.6.8/ape_hardhat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 16:30:52.000000 ape-hardhat-0.6.8/ape_hardhat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/hardhat.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-13 16:30:52.686029 ape-hardhat-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:30:52.670029 ape-hardhat-0.6.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:30:52.666029 ape-hardhat-0.6.8/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:30:52.666029 ape-hardhat-0.6.8/tests/data/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:30:52.666029 ape-hardhat-0.6.8/tests/data/contracts/ethereum/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:30:52.674029 ape-hardhat-0.6.8/tests/data/contracts/ethereum/local/
--rw-r--r--   0 runner    (1001) docker     (123)    28685 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/local/contract_a.json
--rw-r--r--   0 runner    (1001) docker     (123)    27534 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/local/contract_b.json
--rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/local/contract_c.json
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/local/has_error.json
--rw-r--r--   0 runner    (1001) docker     (123)    45606 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/local/reverts_contract.json
--rw-r--r--   0 runner    (1001) docker     (123)    33356 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/local/solidity_contract.json
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/local/sub_reverts_contract.json
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/local/token_a.json
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/local/token_b.json
--rw-r--r--   0 runner    (1001) docker     (123)    28197 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/local/vyper_contract.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:30:52.666029 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:30:52.682029 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
--rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json
--rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json
--rw-r--r--   0 runner    (1001) docker     (123)    17042 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json
--rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4a672a16dEf4BAa3907BBF6f43C868297b111e5B.json
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json
--rw-r--r--   0 runner    (1001) docker     (123)    19792 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json
--rw-r--r--   0 runner    (1001) docker     (123)    44429 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json
--rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json
--rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json
--rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json
--rw-r--r--   0 runner    (1001) docker     (123)    14160 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json
--rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
--rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:30:52.682029 ape-hardhat-0.6.8/tests/data/python/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/python/pytest_test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/python/pytest_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:30:52.686029 ape-hardhat-0.6.8/tests/data/sources/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/sources/HasError.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/sources/RevertsContractVy.vy
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/sources/SubRevertsVy.vy
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/sources/TokenA.vy
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/sources/TokenB.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:30:52.686029 ape-hardhat-0.6.8/tests/data/sources/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/data/sources/interfaces/ISubRevertsVy.vy
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/expected_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)     9091 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/test_fork_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/test_gas_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-13 16:29:24.000000 ape-hardhat-0.6.8/tests/test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:43.083670 ape-hardhat-0.6.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:43.059670 ape-hardhat-0.6.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:43.063670 ape-hardhat-0.6.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:43.063670 ape-hardhat-0.6.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-06-20 21:27:43.083670 ape-hardhat-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:43.063670 ape-hardhat-0.6.9/ape_hardhat/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/ape_hardhat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/ape_hardhat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32258 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/ape_hardhat/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/ape_hardhat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 21:27:41.000000 ape-hardhat-0.6.9/ape_hardhat/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:43.067670 ape-hardhat-0.6.9/ape_hardhat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-06-20 21:27:42.000000 ape-hardhat-0.6.9/ape_hardhat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-06-20 21:27:42.000000 ape-hardhat-0.6.9/ape_hardhat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 21:27:42.000000 ape-hardhat-0.6.9/ape_hardhat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 21:27:42.000000 ape-hardhat-0.6.9/ape_hardhat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-20 21:27:42.000000 ape-hardhat-0.6.9/ape_hardhat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 21:27:42.000000 ape-hardhat-0.6.9/ape_hardhat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-20 21:27:43.087670 ape-hardhat-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:43.067670 ape-hardhat-0.6.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:43.059670 ape-hardhat-0.6.9/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:43.055670 ape-hardhat-0.6.9/tests/data/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:43.055670 ape-hardhat-0.6.9/tests/data/contracts/ethereum/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:43.071670 ape-hardhat-0.6.9/tests/data/contracts/ethereum/local/
+-rw-r--r--   0 runner    (1001) docker     (123)    28685 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/local/contract_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)    27534 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/local/contract_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/local/contract_c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/local/has_error.json
+-rw-r--r--   0 runner    (1001) docker     (123)    45606 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/local/reverts_contract.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33356 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/local/solidity_contract.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/local/sub_reverts_contract.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/local/token_a.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/local/token_b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28197 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/local/vyper_contract.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:43.055670 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:43.083670 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7438 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17042 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x4a672a16dEf4BAa3907BBF6f43C868297b111e5B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19792 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json
+-rw-r--r--   0 runner    (1001) docker     (123)    44429 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15942 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14160 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:43.083670 ape-hardhat-0.6.9/tests/data/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/python/pytest_test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/python/pytest_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:43.083670 ape-hardhat-0.6.9/tests/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/sources/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/sources/RevertsContractVy.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/sources/SubRevertsVy.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/sources/TokenA.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/sources/TokenB.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:27:43.083670 ape-hardhat-0.6.9/tests/data/sources/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/data/sources/interfaces/ISubRevertsVy.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/expected_traces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/test_fork_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/test_gas_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-20 21:26:32.000000 ape-hardhat-0.6.9/tests/test_trace.py
```

### Comparing `ape-hardhat-0.6.8/.github/ISSUE_TEMPLATE/bug.md` & `ape-hardhat-0.6.9/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/.github/ISSUE_TEMPLATE/feature.md` & `ape-hardhat-0.6.9/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/.github/ISSUE_TEMPLATE/work-item.md` & `ape-hardhat-0.6.9/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/.github/release-drafter.yml` & `ape-hardhat-0.6.9/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/.github/workflows/codeql.yml` & `ape-hardhat-0.6.9/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/.github/workflows/commit.yaml` & `ape-hardhat-0.6.9/.github/workflows/commit.yaml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/.github/workflows/prtitle.yaml` & `ape-hardhat-0.6.9/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/.github/workflows/publish.yaml` & `ape-hardhat-0.6.9/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/.github/workflows/stale-prs.yml` & `ape-hardhat-0.6.9/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/.github/workflows/test.yaml` & `ape-hardhat-0.6.9/.github/workflows/test.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         - name: Setup Node
           uses: actions/setup-node@v3
           with:
               node-version: '16'
 
         - name: Install Node Dependencies
-          run: npm install --save-dev hardhat
+          run: pushd tests && npm install --save-dev hardhat && popd
 
         - name: Run Async Tests
           run: pytest -m "not fork and not manual and not fuzzing"
 
         - name: Run Sync Tests
           # Only run forked-network tests if not from a forked repo (Else it always fails)
           if: github.event.pull_request.head.repo.full_name == github.repository
```

### Comparing `ape-hardhat-0.6.8/.gitignore` & `ape-hardhat-0.6.9/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/.pre-commit-config.yaml` & `ape-hardhat-0.6.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/CONTRIBUTING.md` & `ape-hardhat-0.6.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/LICENSE` & `ape-hardhat-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/PKG-INFO` & `ape-hardhat-0.6.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-hardhat
-Version: 0.6.8
+Version: 0.6.9
 Summary: ape-hardhat: Ape network provider for Hardhat
 Home-page: https://github.com/ApeWorX/ape-hardhat
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -126,14 +126,25 @@
         enable_hardhat_deployments: true
 ```
 
 ```bash
 ape plugins install alchemy
 ```
 
+## Remote Hardhat Node
+
+To connect to a Hardhat node, set up your config like this:
+
+```yaml
+hardhat:
+  host: https://hardhat.example.com
+```
+
+Now, instead of launching a local process, it will attempt to connect to the remote Hardhat node and use this plugin as the ape interace.
+
 ## Custom Hardhat Config File
 
 By default, Ape generates and uses a basic config file for starting up a Hardhat node and having the same test accounts that Ape expects.
 To avoid conflict with other pre-existing Hardhat config files, Ape generates one in `$HOME/.ape/hardhat` and always refers to that one.
 To use a different one, such as the one in your local project instead, add the following to your `ape-config.yaml`:
 
 ```yaml
```

### Comparing `ape-hardhat-0.6.8/README.md` & `ape-hardhat-0.6.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -97,14 +97,25 @@
         enable_hardhat_deployments: true
 ```
 
 ```bash
 ape plugins install alchemy
 ```
 
+## Remote Hardhat Node
+
+To connect to a Hardhat node, set up your config like this:
+
+```yaml
+hardhat:
+  host: https://hardhat.example.com
+```
+
+Now, instead of launching a local process, it will attempt to connect to the remote Hardhat node and use this plugin as the ape interace.
+
 ## Custom Hardhat Config File
 
 By default, Ape generates and uses a basic config file for starting up a Hardhat node and having the same test accounts that Ape expects.
 To avoid conflict with other pre-existing Hardhat config files, Ape generates one in `$HOME/.ape/hardhat` and always refers to that one.
 To use a different one, such as the one in your local project instead, add the following to your `ape-config.yaml`:
 
 ```yaml
```

### Comparing `ape-hardhat-0.6.8/ape_hardhat/__init__.py` & `ape-hardhat-0.6.9/ape_hardhat/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/ape_hardhat/exceptions.py` & `ape-hardhat-0.6.9/ape_hardhat/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/ape_hardhat/provider.py` & `ape-hardhat-0.6.9/ape_hardhat/provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     TransactionAPI,
     UpstreamProvider,
     Web3Provider,
 )
 from ape.exceptions import (
     ContractLogicError,
     OutOfGasError,
-    ProviderError,
     RPCTimeoutError,
     SubprocessError,
     TransactionError,
     VirtualMachineError,
 )
 from ape.logging import logger
 from ape.types import AddressType, CallTreeNode, ContractCode, SnapshotID, TraceFrame
@@ -39,14 +38,15 @@
 from pydantic import BaseModel, Field
 from web3 import HTTPProvider, Web3
 from web3.exceptions import ExtraDataLengthError
 from web3.gas_strategies.rpc import rpc_gas_price_strategy
 from web3.middleware import geth_poa_middleware
 from web3.middleware.validation import MAX_EXTRADATA_LENGTH
 from web3.types import TxParams
+from yarl import URL
 
 from .exceptions import HardhatNotInstalledError, HardhatProviderError, HardhatSubprocessError
 
 EPHEMERAL_PORTS_START = 49152
 EPHEMERAL_PORTS_END = 60999
 DEFAULT_PORT = 8545
 HARDHAT_CHAIN_ID = 31337
@@ -161,16 +161,28 @@
     upstream_provider: Optional[str] = None
     block_number: Optional[int] = None
     enable_hardhat_deployments: bool = False
 
 
 class HardhatNetworkConfig(PluginConfig):
     port: Optional[Union[int, Literal["auto"]]] = DEFAULT_PORT
+    """Depreciated. Use ``host`` config."""
+
+    host: Optional[Union[str, Literal["auto"]]] = None
+    """The host address or ``"auto"`` to use localhost with a random port (with attempts)."""
+
+    manage_process: bool = True
+    """
+    If ``True`` and the host is local and Hardhat is not running, will attempt to start.
+    Defaults to ``True``. If ``host`` is remote, will not be able to start.
+    """
+
     request_timeout: int = 30
     fork_request_timeout: int = 300
+    process_attempts: int = 5
 
     hardhat_config_file: Optional[Path] = None
     """
     Optionally specify a Hardhat config file to use
     (in the case when you don't wish to use the one Ape creates).
     Note: If you do this, you may need to ensure its settings
     matches Ape's.
@@ -186,16 +198,17 @@
 
 
 def _call(*args):
     return call([*args], stderr=PIPE, stdout=PIPE, stdin=PIPE)
 
 
 class HardhatProvider(SubprocessProvider, Web3Provider, TestProviderAPI):
-    port: Optional[int] = None
+    _host: Optional[str] = None
     attempted_ports: List[int] = []
+    _did_warn_wrong_node = False
 
     # Will get set to False if notices not installed correctly.
     # However, will still attempt to connect and only raise
     # if failed to connect. This is because sometimes Hardhat may still work,
     # such when running via `pytester`.
     _detected_correct_install: bool = True
 
@@ -216,19 +229,27 @@
         return "Hardhat node"
 
     @property
     def timeout(self) -> int:
         return self.config.request_timeout
 
     @property
+    def _clean_uri(self) -> str:
+        return str(URL(self.uri).with_user(None).with_password(None))
+
+    @property
+    def _port(self) -> Optional[int]:
+        return URL(self.uri).port
+
+    @property
     def chain_id(self) -> int:
         return self.web3.eth.chain_id if hasattr(self.web3, "eth") else HARDHAT_CHAIN_ID
 
-    @property
-    def npx_bin(self) -> str:
+    @cached_property
+    def node_bin(self) -> str:
         npx = shutil.which("npx")
         suffix = "See ape-hardhat README for install steps."
         if not npx:
             raise HardhatSubprocessError(f"Could not locate `npx` executable. {suffix}")
 
         elif _call(npx, "--version") != 0:
             raise HardhatSubprocessError(f"`npm` executable returned error code. {suffix}.")
@@ -250,40 +271,69 @@
             self._detected_correct_install = False
             return npx
 
         data = json.loads(install_result)
 
         # This actually ensures it is installed.
         self._detected_correct_install = "hardhat" in data.get("dependencies", {})
-        return npx
+        node = shutil.which("node")
+        if not node:
+            raise HardhatSubprocessError(f"Could not locate `node` executable. {suffix}")
+
+        return node
 
     @property
     def project_folder(self) -> Path:
         return self.config_manager.PROJECT_FOLDER
 
     @property
     def uri(self) -> str:
-        if not self.port:
-            raise HardhatProviderError("Can't build URI before `connect()` is called.")
-
-        return f"http://127.0.0.1:{self.port}"
+        if self._host is not None:
+            return self._host
+        if config_host := self.config.host:
+            if config_host == "auto":
+                self._host = "auto"
+                return self._host
+
+            if not config_host.startswith("http"):
+                if "127.0.0.1" in config_host or "localhost" in config_host:
+                    self._host = f"http://{config_host}"
+                else:
+                    self._host = f"https://{config_host}"
+            else:
+                self._host = config_host
+            if "127.0.0.1" in config_host or "localhost" in config_host:
+                host_without_http = self._host[7:]
+                if ":" not in host_without_http:
+                    self._host = f"{self._host}:{DEFAULT_PORT}"
+        else:
+            self._host = f"http://127.0.0.1:{DEFAULT_PORT}"
+        return self._host
 
     @property
     def priority_fee(self) -> int:
         """
         Priority fee not needed in development network.
         """
         return 0
 
     @property
     def is_connected(self) -> bool:
+        if self._host in ("auto", None):
+            # Hasn't tried yet.
+            return False
+
         self._set_web3()
         return self._web3 is not None
 
     @property
+    def bin_path(self) -> Path:
+        return self.project_folder / "node_modules" / ".bin" / "hardhat"
+
+    @property
     def hardhat_config_file(self) -> Path:
         if self.config.hardhat_config_file and self.config.hardhat_config_file.is_dir():
             path = self.config.hardhat_config_file / DEFAULT_HARDHAT_CONFIG_FILE_NAME
         elif self.config.hardhat_config_file:
             path = self.config.hardhat_config_file
         else:
             path = self.config_manager.DATA_FOLDER / "hardhat" / DEFAULT_HARDHAT_CONFIG_FILE_NAME
@@ -327,64 +377,97 @@
         """
 
         _validate_hardhat_config_file(
             self.hardhat_config_file, self.mnemonic, self.number_of_accounts
         )
 
         # NOTE: Must set port before calling 'super().connect()'.
-        if not self.port:
-            self.port = self.provider_settings.get("port", self.config.port)
+        warning = "`port` setting is depreciated. Please use `host` key that includes the port."
+
+        if "port" in self.provider_settings:
+            # TODO: Can remove after 0.7.
+            logger.warning(warning)
+            self._host = f"http://127.0.0.1:{self.provider_settings['port']}"
+
+        elif self.config.port != DEFAULT_PORT and self.config.host is not None:
+            raise HardhatProviderError(
+                "Cannot use depreciated `port` field with `host`."
+                "Place `port` at end of `host` instead."
+            )
+
+        elif self.config.port != DEFAULT_PORT:
+            # We only get here if the user configured a port without a host,
+            # the old way of doing it. TODO: Can remove after 0.7.
+            logger.warning(warning)
+            if self.config.port not in (None, "auto"):
+                self._host = f"http://127.0.0.1:{self.config.port}"
+            else:
+                # This will trigger selecting a random port on localhost and trying.
+                self._host = "auto"
+
+        elif "host" in self.provider_settings:
+            self._host = self.provider_settings["host"]
+
+        elif self._host is None:
+            self._host = self.uri
 
         if self.is_connected:
             # Connects to already running process
             self._start()
-        else:
+        elif self.config.manage_process:
             # Only do base-process setup if not connecting to already-running process
             super().connect()
 
-            if self.port:
+            if self._host:
                 self._set_web3()
                 if not self._web3:
                     self._start()
                 else:
-                    # The user configured a port and the hardhat process was already running.
+                    # The user configured a host and the hardhat process was already running.
                     logger.info(
-                        f"Connecting to existing '{self.process_name}' at port '{self.port}'."
+                        f"Connecting to existing '{self.process_name}' at host '{self._clean_uri}'."
                     )
             else:
                 for _ in range(self.config.process_attempts):
                     try:
                         self._start()
                         break
                     except HardhatNotInstalledError:
                         # Is a sub-class of `HardhatSubprocessError` but we to still raise
                         # so we don't keep retrying.
                         raise
                     except SubprocessError as exc:
                         logger.info("Retrying Hardhat subprocess startup: %r", exc)
-                        self.port = None
+                        self._host = None
+        else:
+            raise HardhatProviderError(
+                f"Failed to connect to remote Hardhat node at {self._clean_uri}`"
+            )
 
     def _set_web3(self):
-        if not self.port:
+        if not self._host:
             return
 
         self._web3 = _create_web3(self.uri, self.timeout)
         if not self._web3.is_connected():
             self._web3 = None
             return
 
         # Verify is actually a Hardhat provider,
         # or else skip it to possibly try another port.
         client_version = self._web3.client_version.lower()
         if "hardhat" in client_version:
             self._web3.eth.set_gas_price_strategy(rpc_gas_price_strategy)
-        else:
-            raise ProviderError(
-                f"Port '{self.port}' already in use by another process that isn't a Hardhat node."
+        elif self._port is not None:
+            raise HardhatProviderError(
+                f"A process that is not a Hardhat node is running at host {self._clean_uri}."
             )
+        else:
+            # Not sure if possible to get here.
+            raise HardhatProviderError("Failed to start Hardhat process.")
 
         def check_poa(block_id) -> bool:
             try:
                 block = self.web3.eth.get_block(block_id)
             except ExtraDataLengthError:
                 return True
             else:
@@ -394,58 +477,74 @@
                 )
 
         # Handle if using PoA Hardhat
         if any(map(check_poa, (0, "latest"))):
             self._web3.middleware_onion.inject(geth_poa_middleware, layer=0)
 
     def _start(self):
-        use_random_port = self.port == "auto"
+        use_random_port = self._host == "auto"
         if use_random_port:
-            self.port = None
+            self._host = None
 
-            if DEFAULT_PORT not in self.attempted_ports and not use_random_port:
-                self.port = DEFAULT_PORT
-            else:
+            if DEFAULT_PORT not in self.attempted_ports:
+                self._host = f"http://127.0.0.1:{DEFAULT_PORT}"
+
+            # Pick a random port
+            port = random.randint(EPHEMERAL_PORTS_START, EPHEMERAL_PORTS_END)
+            max_attempts = 25
+            attempts = 0
+            while port in self.attempted_ports:
                 port = random.randint(EPHEMERAL_PORTS_START, EPHEMERAL_PORTS_END)
-                max_attempts = 25
-                attempts = 0
-                while port in self.attempted_ports:
-                    port = random.randint(EPHEMERAL_PORTS_START, EPHEMERAL_PORTS_END)
-                    attempts += 1
-                    if attempts == max_attempts:
-                        ports_str = ", ".join([str(p) for p in self.attempted_ports])
-                        raise HardhatProviderError(
-                            f"Unable to find an available port. Ports tried: {ports_str}"
-                        )
+                attempts += 1
+                if attempts == max_attempts:
+                    ports_str = ", ".join([str(p) for p in self.attempted_ports])
+                    raise HardhatProviderError(
+                        f"Unable to find an available port. Ports tried: {ports_str}"
+                    )
 
-                self.port = port
+            self.attempted_ports.append(port)
+            self._host = f"http://127.0.0.1:{port}"
+
+        elif self._host is not None and ":" in self._host and self._port is not None:
+            # Append the one and only port to the attempted ports list, for honest keeping.
+            self.attempted_ports.append(self._port)
+
+        else:
+            self._host = f"http://127.0.0.1:{DEFAULT_PORT}"
 
-        self.attempted_ports.append(self.port)
         try:
             self.start()
         except RPCTimeoutError as err:
             if not self._detected_correct_install:
                 raise HardhatNotInstalledError() from err
 
             raise  # RPCTimeoutError
 
     def disconnect(self):
         self._web3 = None
-        self.port = None
+        self._host = None
         super().disconnect()
 
     def build_command(self) -> List[str]:
+        # Run `node` on the actual binary.
+        # This allows the process mgmt to function and prevents dangling nodes.
+        if not self.bin_path.is_file():
+            raise HardhatSubprocessError("Unable to find Hardhat binary. Is it installed?")
+
+        return self._get_command()
+
+    def _get_command(self) -> List[str]:
         return [
-            self.npx_bin,
-            "hardhat",
+            self.node_bin,
+            str(self.bin_path),
             "node",
             "--hostname",
             "127.0.0.1",
             "--port",
-            str(self.port),
+            f"{self._port or DEFAULT_PORT}",
             "--config",
             str(self.hardhat_config_file),
         ]
 
     def set_block_gas_limit(self, gas_limit: int) -> bool:
         return self._make_request("evm_setBlockGasLimit", [hex(gas_limit)]) is True
 
@@ -728,29 +827,29 @@
                 logger.error(
                     f"Upstream provider '{self._upstream_provider.name}' "
                     f"missing Geth PoA middleware."
                 )
                 self._upstream_provider.web3.middleware_onion.inject(geth_poa_middleware, layer=0)
                 upstream_genesis_block_hash = self._upstream_provider.get_block(0).hash
             else:
-                raise ProviderError(f"Unable to get genesis block: {err}.") from err
+                raise HardhatProviderError(f"Unable to get genesis block: {err}.") from err
 
         self._upstream_provider.disconnect()
 
         if self.get_block(0).hash != upstream_genesis_block_hash:
             logger.warning(
                 "Upstream network has mismatching genesis block. "
                 "This could be an issue with hardhat."
             )
 
     def build_command(self) -> List[str]:
         if not self.fork_url:
             raise HardhatProviderError("Upstream provider does not have a ``connection_str``.")
 
-        if self.fork_url.replace("localhost", "127.0.0.1") == self.uri:
+        if self.fork_url.replace("localhost", "127.0.0.1").replace("http://", "") == self.uri:
             raise HardhatProviderError(
                 "Invalid upstream-fork URL. Can't be same as local Hardhat node."
             )
 
         cmd = super().build_command()
         cmd.extend(("--fork", self.fork_url))
```

### Comparing `ape-hardhat-0.6.8/ape_hardhat.egg-info/PKG-INFO` & `ape-hardhat-0.6.9/ape_hardhat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-hardhat
-Version: 0.6.8
+Version: 0.6.9
 Summary: ape-hardhat: Ape network provider for Hardhat
 Home-page: https://github.com/ApeWorX/ape-hardhat
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -126,14 +126,25 @@
         enable_hardhat_deployments: true
 ```
 
 ```bash
 ape plugins install alchemy
 ```
 
+## Remote Hardhat Node
+
+To connect to a Hardhat node, set up your config like this:
+
+```yaml
+hardhat:
+  host: https://hardhat.example.com
+```
+
+Now, instead of launching a local process, it will attempt to connect to the remote Hardhat node and use this plugin as the ape interace.
+
 ## Custom Hardhat Config File
 
 By default, Ape generates and uses a basic config file for starting up a Hardhat node and having the same test accounts that Ape expects.
 To avoid conflict with other pre-existing Hardhat config files, Ape generates one in `$HOME/.ape/hardhat` and always refers to that one.
 To use a different one, such as the one in your local project instead, add the following to your `ape-config.yaml`:
 
 ```yaml
```

### Comparing `ape-hardhat-0.6.8/ape_hardhat.egg-info/SOURCES.txt` & `ape-hardhat-0.6.9/ape_hardhat.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 .gitignore
 .mdformat.toml
 .pre-commit-config.yaml
 CONTRIBUTING.md
 LICENSE
 README.md
-hardhat.config.js
 pyproject.toml
 setup.cfg
 setup.py
 .github/PULL_REQUEST_TEMPLATE.md
 .github/release-drafter.yml
 .github/ISSUE_TEMPLATE/bug.md
 .github/ISSUE_TEMPLATE/feature.md
```

### Comparing `ape-hardhat-0.6.8/ape_hardhat.egg-info/requires.txt` & `ape-hardhat-0.6.9/ape_hardhat.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-eth-ape<0.7,>=0.6.9
+eth-ape<0.7,>=0.6.11
 evm-trace
 hexbytes
 web3
 chompjs<2,>=1.1.9
+yarl<2,>=1.9.2
 
 [dev]
 pytest>=6.0
 pytest-mock
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
@@ -19,30 +20,30 @@
 types-setuptools
 types-requests
 flake8<7,>=6.0.0
 isort<6,>=5.10.1
 mdformat>=0.7.16
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
-Sphinx<4,>=3.4.3
-sphinx_rtd_theme<1,>=0.1.9
+Sphinx<7,>=6.1.3
+sphinx_rtd_theme<2,>=1.2.0
 towncrier<20,>=19.2.0
 setuptools
 setuptools-scm
 wheel
 twine
 commitizen
 pre-commit
 pytest-watch
 IPython
 ipdb
 
 [doc]
-Sphinx<4,>=3.4.3
-sphinx_rtd_theme<1,>=0.1.9
+Sphinx<7,>=6.1.3
+sphinx_rtd_theme<2,>=1.2.0
 towncrier<20,>=19.2.0
 
 [lint]
 black<24,>=23.3.0
 mypy<1,>=0.991
 types-PyYAML
 types-setuptools
```

### Comparing `ape-hardhat-0.6.8/pyproject.toml` & `ape-hardhat-0.6.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/setup.py` & `ape-hardhat-0.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
         "flake8>=6.0.0,<7",  # Style linter
         "isort>=5.10.1,<6",  # Import sorting linter
         "mdformat>=0.7.16",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
     ],
     "doc": [
-        "Sphinx>=3.4.3,<4",  # Documentation generator
-        "sphinx_rtd_theme>=0.1.9,<1",  # Readthedocs.org theme
+        "Sphinx>=6.1.3,<7",  # Documentation generator
+        "sphinx_rtd_theme>=1.2.0,<2",  # Readthedocs.org theme
         "towncrier>=19.2.0, <20",  # Generate release notes
     ],
     "release": [  # `release` GitHub Action job uses this
         "setuptools",  # Installation tool
         "setuptools-scm",  # Installation tool
         "wheel",  # Packaging tool
         "twine",  # Package upload tool
@@ -67,19 +67,20 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-hardhat",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.6.9,<0.7",
+        "eth-ape>=0.6.11,<0.7",
         "evm-trace",  # Use same version as eth-ape
         "hexbytes",  # Use same version as eth-ape
         "web3",  # Use same version as eth-ape
         "chompjs>=1.1.9,<2",  # To help parse hardhat files
+        "yarl>=1.9.2,<2",
     ],
     python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=["ape_hardhat"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
```

### Comparing `ape-hardhat-0.6.8/tests/ape-config.yaml` & `ape-hardhat-0.6.9/tests/ape-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/conftest.py` & `ape-hardhat-0.6.9/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -199,28 +199,28 @@
 def mainnet_fork_port():
     return MAINNET_FORK_PORT
 
 
 @pytest.fixture
 def mainnet_fork_provider(name, networks, mainnet_fork_port):
     with networks.ethereum["mainnet-fork"].use_provider(
-        name, provider_settings={"port": mainnet_fork_port}
+        name, provider_settings={"host": f"http://127.0.0.1:{mainnet_fork_port}"}
     ) as provider:
         yield provider
 
 
 @pytest.fixture
 def goerli_fork_port():
     return GOERLI_FORK_PORT
 
 
 @pytest.fixture
 def goerli_fork_provider(name, networks, goerli_fork_port):
     with networks.ethereum.goerli_fork.use_provider(
-        name, provider_settings={"port": goerli_fork_port}
+        name, provider_settings={"host": f"http://127.0.0.1:{goerli_fork_port}"}
     ) as provider:
         yield provider
 
 
 @pytest.fixture(scope="session")
 def temp_config(config):
     @contextmanager
```

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/local/contract_a.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/local/contract_a.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/local/contract_b.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/local/contract_b.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/local/contract_c.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/local/contract_c.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/local/has_error.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/local/has_error.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/local/reverts_contract.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/local/reverts_contract.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/local/solidity_contract.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/local/solidity_contract.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/local/sub_reverts_contract.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/local/sub_reverts_contract.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/local/token_a.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/local/token_a.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/local/token_b.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/local/token_b.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/local/vyper_contract.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/local/vyper_contract.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x0000000000b3F879cb30FE243b4Dfee438691c04.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x00c47B2Ac6C298d33DCd53Adb48F3d678BD0E561.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x0C3F8Df27e1A00b47653fDE878D68D35F00714C0.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x0c212728e3cDb57ED62DdFCa917Fe7DF17A63979.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x1111111254fb6c44bAC0beD2854e76F90643097d.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x197E90f9FAD81970bA7976f33CbD77088E5D7cf7.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x1b14E8D511c9A4395425314f849bD737BAF8208F.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x1c27Be6D7146eb9273DB1d22Eb860b9E85854EEa.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x24a42fD28C976A61Df5D00D0599C34c4f90748c8.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x2F0b23f53734252Bda2277357e97e1517d6B042A.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x2a17c35FF147b32f13F19F2E311446eEB02503F3.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x338f7e5d19d9953b76dD81446B142C2D9fE03482.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x35A18000230DA775CAc24873d00Ff85BccdeD550.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x35D1b3F3D7966A1DFe207aa4514C12a259A0492B.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x398eC7346DcD622eDc5ae82352F02bE94C62d119.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x3Ba0319533C578527aE69BF7fA2D289F20B9B55c.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x3d9819210A31b4961b30EF54bE2aeD79B9c9Cd3B.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x3dfd23A6c5E8BbcFc9581d2E864a68feb6a076d3.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x4031064525292eaeb0dAE34Bbf5759E85CdE09Ad.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x4BA1f38427b33B8ab7Bb0490200dAE1F1C36823F.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x4D728A4496e4De35f218D5A214366bde3a62B51C.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x4Ddc2D193948926D02f9B1fE9e1daa0718270ED5.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x533c8844bA1922b88d892aCA090df0cC0c292F1b.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x5766067108e534419ce13F05899bC3E3F4344948.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x597C52281b31B9d949a9D8fEbA08F7A2530a965e.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x5c55B921f590a89C1Ebe84dF170E655a82b62126.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x5d3a536E4D6DbD6114cc1Ead35777bAB948E3643.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x5ef30b9986345249bc32d8928B7ee64DE9435E39.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x61935CbDd02287B511119DDb11Aeb42F1593b7Ef.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x637726f8b08a7ABE3aE3aCaB01A80E2d8ddeF77B.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x6B175474E89094C44Da98b954EedeAC495271d0F.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x6D252BaEa75459Ed0077410613c5f6e51cAb4750.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x72B886d09C117654aB7dA13A14d603001dE0B777.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x77924185CF0cbB2Ae0b746A0086A065d6875b0a5.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x7b5e3521a049C8fF88e6349f33044c6Cc33c113c.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x88e6A0c2dDD26FEEb64F039a2c41296FcB3f5640.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x922018674c12a7F0D394ebEEf9B58F186CdE13c1.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x95E6F48254609A6ee006F7D493c8e5fB97094ceF.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x9759A6Ac90977b93B58547b4A71c78317f391A28.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0x976aa93ca5Aaa569109f4267589c619a097f001D.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xA4d2D85d84F86F4a91A9974a5e76C8257B17e8bA.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xA950524441892A31ebddF91d3cEEFa04Bf454466.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xC47b7094F378e54347e281AaB170E8ccA69d880A.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xE3d9988F676457123C5fD01297605efdD0Cba1ae.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xF14f0648435CF34f8bC800d4E71FF0Ba15bC52dD.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xFB564da37B41b2F6B6EDcc3e56FbF523bD9F2012.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xa2327a938Febf5FEC13baCFb16Ae10EcBc4cbDCF.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xa26e80e7Dea86279c6d778D702Cc413E6CFfA777.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xaa1A02671440Be41545D83BDDfF2bf2488628C10.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xb67F15159e1C60d7E5f5b60316c4588b014c61fa.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xbB8bE4772fAA655C255309afc3c5207aA7b896Fd.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xc00e94Cb662C3520282E6f5717214004A7f26888.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xdAC17F958D2ee523a2206206994597C13D831ec7.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xe800542e56208aC5c496A57926FA7647ed8E5f07.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xeAC99f8Fb1996AeB153E8cF0842908973a48C66F.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xf650C3d88D12dB855b8bf7D11Be6C55A4e07dCC9.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json` & `ape-hardhat-0.6.9/tests/data/contracts/ethereum/mainnet/contract_types/0xfeD941d39905B23D6FAf02C8301d40bD4834E27F.json`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/python/pytest_tests.py` & `ape-hardhat-0.6.9/tests/data/python/pytest_tests.py`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/sources/RevertsContractVy.vy` & `ape-hardhat-0.6.9/tests/data/sources/RevertsContractVy.vy`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/sources/TokenA.vy` & `ape-hardhat-0.6.9/tests/data/sources/TokenA.vy`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/data/sources/TokenB.vy` & `ape-hardhat-0.6.9/tests/data/sources/TokenB.vy`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/expected_traces.py` & `ape-hardhat-0.6.9/tests/expected_traces.py`

 * *Files identical despite different names*

### Comparing `ape-hardhat-0.6.8/tests/test_fork_provider.py` & `ape-hardhat-0.6.9/tests/test_fork_provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,39 +18,42 @@
     return owner.deploy(contract_container)
 
 
 @pytest.mark.fork
 def test_multiple_providers(
     name, networks, connected_provider, mainnet_fork_port, goerli_fork_port
 ):
+    default_host = "http://127.0.0.1:8545"
     assert networks.active_provider.name == name
     assert networks.active_provider.network.name == LOCAL_NETWORK_NAME
-    assert networks.active_provider.port == 8545
+    assert networks.active_provider.uri == default_host
+    mainnet_fork_host = f"http://127.0.0.1:{mainnet_fork_port}"
 
     with networks.ethereum.mainnet_fork.use_provider(
-        name, provider_settings={"port": mainnet_fork_port}
+        name, provider_settings={"host": mainnet_fork_host}
     ):
         assert networks.active_provider.name == name
         assert networks.active_provider.network.name == "mainnet-fork"
-        assert networks.active_provider.port == mainnet_fork_port
+        assert networks.active_provider.uri == mainnet_fork_host
+        goerli_fork_host = f"http://127.0.0.1:{goerli_fork_port}"
 
         with networks.ethereum.goerli_fork.use_provider(
-            name, provider_settings={"port": goerli_fork_port}
+            name, provider_settings={"host": goerli_fork_host}
         ):
             assert networks.active_provider.name == name
             assert networks.active_provider.network.name == "goerli-fork"
-            assert networks.active_provider.port == goerli_fork_port
+            assert networks.active_provider.uri == goerli_fork_host
 
         assert networks.active_provider.name == name
         assert networks.active_provider.network.name == "mainnet-fork"
-        assert networks.active_provider.port == mainnet_fork_port
+        assert networks.active_provider.uri == mainnet_fork_host
 
     assert networks.active_provider.name == name
     assert networks.active_provider.network.name == LOCAL_NETWORK_NAME
-    assert networks.active_provider.port == 8545
+    assert networks.active_provider.uri == default_host
 
 
 @pytest.mark.parametrize("network", [k for k in NETWORKS.keys()])
 def test_fork_config(name, config, network):
     plugin_config = config.get_config(name)
     network_config = plugin_config["fork"].get("ethereum", {}).get(network, {})
     assert network_config.get("upstream_provider") == "alchemy", "config not registered"
@@ -149,14 +152,15 @@
         mainnet_fork_contract_instance.setNumber(10, sender=mainnet_fork_contract_instance)
 
 
 @pytest.mark.fork
 def test_transaction_unknown_contract_as_sender(accounts, mainnet_fork_provider):
     account = "0xFEB4acf3df3cDEA7399794D0869ef76A6EfAff52"
     multi_sig = accounts[account]
+    multi_sig.balance += accounts.conversion_manager.convert("1000 ETH", int)
     receipt = multi_sig.transfer(accounts[0], "100 gwei")
     assert not receipt.failed
 
 
 @pytest.mark.fork
 def test_get_receipt(mainnet_fork_provider, mainnet_fork_contract_instance, owner):
     receipt = mainnet_fork_contract_instance.setAddress(owner.address, sender=owner)
@@ -218,15 +222,15 @@
         provider = HardhatForkProvider(
             name=name,
             network=network_api,
             request_header={},
             data_folder=Path("."),
             provider_settings={},
         )
-        provider.port = port
+        provider._host = f"http://127.0.0.1:{port}"
         actual = provider.build_command()
         expected = [
             name,
             "node",
             "--hostname",
             "127.0.0.1",
             "--port",
```

### Comparing `ape-hardhat-0.6.8/tests/test_gas_report.py` & `ape-hardhat-0.6.9/tests/test_gas_report.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,17 +17,17 @@
   transfer +\d +\d+ + \d+ + \d+ + \d+
 """
 EXPECTED_GAS_REPORT = rf"""
  +TestContractVy Gas
 
   Method +Times called +Min. +Max. +Mean +Median
  ─+
+  fooAndBar +\d +\d+ + \d+ + \d+ + \d+
   myNumber +\d +\d+ + \d+ + \d+ + \d+
   setNumber +\d +\d+ + \d+ + \d+ + \d+
-  fooAndBar +\d +\d+ + \d+ + \d+ + \d+
 
  +TokenA Gas
 
   Method +Times called +Min. +Max. +Mean +Median
  ─+
   balanceOf +\d +\d+ + \d+ + \d+ + \d+
   transfer +\d +\d+ + \d+ + \d+ + \d+
```

### Comparing `ape-hardhat-0.6.8/tests/test_provider.py` & `ape-hardhat-0.6.9/tests/test_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,61 +1,65 @@
 import tempfile
 from pathlib import Path
 
 import pytest
+import requests
 from ape.api import ReceiptAPI
 from ape.api.accounts import ImpersonatedAccount
 from ape.contracts import ContractContainer
 from ape.exceptions import ContractLogicError
 from ape.pytest.contextmanagers import RevertsContextManager as reverts
 from ape.types import CallTreeNode, TraceFrame
 from evm_trace import CallType
 from hexbytes import HexBytes
 
-from ape_hardhat.exceptions import HardhatNotInstalledError, HardhatProviderError
+from ape_hardhat.exceptions import HardhatNotInstalledError, HardhatSubprocessError
 from ape_hardhat.provider import HARDHAT_CHAIN_ID
 
 TEST_WALLET_ADDRESS = "0xD9b7fdb3FC0A0Aa3A507dCf0976bc23D49a9C7A3"
 
 
 def test_instantiation(disconnected_provider, name):
     assert disconnected_provider.name == name
 
 
 def test_connect_and_disconnect(disconnected_provider):
     # Use custom port to prevent connecting to a port used in another test.
 
-    disconnected_provider.port = 8555
+    disconnected_provider._host = "http://127.0.0.1:8555"
     disconnected_provider.connect()
+    uri = f"{disconnected_provider.uri}/eth_getClientVersion"
+    response = requests.get(uri)
+    response.raise_for_status()
 
     try:
         assert disconnected_provider.is_connected
         assert disconnected_provider.chain_id == HARDHAT_CHAIN_ID
     finally:
         disconnected_provider.disconnect()
 
     assert not disconnected_provider.is_connected
     assert disconnected_provider.process is None
 
+    # Proof it is really disconnected.
+    with pytest.raises(Exception):
+        requests.get(uri)
+
 
 def test_gas_price(connected_provider):
     gas_price = connected_provider.gas_price
     assert gas_price > 1
 
 
 def test_uri_disconnected(disconnected_provider):
-    with pytest.raises(
-        HardhatProviderError, match=r"Can't build URI before `connect\(\)` is called\."
-    ):
-        _ = disconnected_provider.uri
+    assert disconnected_provider.uri == "http://127.0.0.1:8545"
 
 
 def test_uri(connected_provider):
-    expected_uri = f"http://127.0.0.1:{connected_provider.port}"
-    assert expected_uri in connected_provider.uri
+    assert connected_provider.uri in connected_provider.uri
 
 
 def test_set_block_gas_limit(connected_provider):
     gas_limit = connected_provider.get_block("latest").gas_limit
     assert connected_provider.set_block_gas_limit(gas_limit) is True
 
 
@@ -246,20 +250,32 @@
         error_contract.withdraw(sender=account)
 
     # Before, this would fail because there would not be an associated txn
     # because the account is impersonated.
     assert err.value.txn.txn_hash.startswith("0x")
 
 
+@pytest.mark.parametrize("host", ("https://example.com", "example.com"))
+def test_host(temp_config, networks, host):
+    data = {"hardhat": {"host": host}}
+    with temp_config(data):
+        provider = networks.ethereum.local.get_provider("hardhat")
+        assert provider.uri == "https://example.com"
+
+
 def test_use_different_config(temp_config, networks):
     data = {"hardhat": {"hardhat_config_file": "./hardhat.config.ts"}}
     with temp_config(data):
         provider = networks.ethereum.local.get_provider("hardhat")
         assert provider.hardhat_config_file.name == "hardhat.config.ts"
-        assert "--config" in provider.build_command()
+        assert "--config" in provider._get_command()
+
+        with pytest.raises(HardhatSubprocessError):
+            # This raises because Hardhat is not installed in the temp project.
+            provider.build_command()
 
 
 def test_connect_when_hardhat_not_installed(networks, mock_web3, install_detection_fail):
     """
     Verifies that if both Hardhat is sensed to not be installed correctly
     and Web3 doesn't connect, you get the custom error about installing
     Hardhat in the project.
```

### Comparing `ape-hardhat-0.6.8/tests/test_trace.py` & `ape-hardhat-0.6.9/tests/test_trace.py`

 * *Files identical despite different names*

