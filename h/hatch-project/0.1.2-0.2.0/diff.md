# Comparing `tmp/hatch_project-0.1.2.tar.gz` & `tmp/hatch_project-0.2.0.tar.gz`

## Comparing `hatch_project-0.1.2.tar` & `hatch_project-0.2.0.tar`

### file list

```diff
@@ -1,767 +1,1898 @@
--rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 hatch_project-0.1.2/requirements.txt
--rwxr-xr-x   0        0        0       74 2020-02-02 00:00:00.000000 hatch_project-0.1.2/uninstall.txt
--rwxr-xr-x   0        0        0      248 2020-02-02 00:00:00.000000 hatch_project-0.1.2/uninstall2.txt
--rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/pyvenv.cfg
--rwxr-xr-x   0        0        0     9033 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/bin/Activate.ps1
--rwxr-xr-x   0        0        0     2030 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/bin/activate
--rwxr-xr-x   0        0        0      956 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/bin/activate.csh
--rwxr-xr-x   0        0        0     2098 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/bin/activate.fish
--rwxr-xr-x   0        0        0      301 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/bin/normalizer
--rwxr-xr-x   0        0        0      278 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/bin/pip
--rwxr-xr-x   0        0        0      278 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/bin/pip3
--rwxr-xr-x   0        0        0      278 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/bin/pip3.10
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/bin/python -> python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/bin/python3 -> /home/kenno/.pyenv/versions/3.10.0/bin/python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/bin/python3.10 -> python3
--rwxr-xr-x   0        0        0      152 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/distutils-precedence.pth
--rwxr-xr-x   0        0        0     3688 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/_distutils_hack/__init__.py
--rwxr-xr-x   0        0        0       44 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/_distutils_hack/override.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/beautifulsoup4-4.12.2.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     3556 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/beautifulsoup4-4.12.2.dist-info/METADATA
--rwxr-xr-x   0        0        0     5623 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/beautifulsoup4-4.12.2.dist-info/RECORD
--rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/beautifulsoup4-4.12.2.dist-info/WHEEL
--rwxr-xr-x   0        0        0     2176 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/beautifulsoup4-4.12.2.dist-info/licenses/AUTHORS
--rwxr-xr-x   0        0        0     1441 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/beautifulsoup4-4.12.2.dist-info/licenses/LICENSE
--rwxr-xr-x   0        0        0    33822 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/__init__.py
--rwxr-xr-x   0        0        0    10077 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/css.py
--rwxr-xr-x   0        0        0    41158 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/dammit.py
--rwxr-xr-x   0        0        0     7195 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/diagnose.py
--rwxr-xr-x   0        0        0    92716 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/element.py
--rwxr-xr-x   0        0        0     7184 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/formatter.py
--rwxr-xr-x   0        0        0    24393 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/builder/__init__.py
--rwxr-xr-x   0        0        0    19078 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/builder/_html5lib.py
--rwxr-xr-x   0        0        0    14919 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/builder/_htmlparser.py
--rwxr-xr-x   0        0        0    14904 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/builder/_lxml.py
--rwxr-xr-x   0        0        0    48391 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/__init__.py
--rwxr-xr-x   0        0        0     1115 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/test_builder.py
--rwxr-xr-x   0        0        0     5114 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/test_builder_registry.py
--rwxr-xr-x   0        0        0    17279 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/test_css.py
--rwxr-xr-x   0        0        0    15451 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/test_dammit.py
--rwxr-xr-x   0        0        0     1127 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/test_docs.py
--rwxr-xr-x   0        0        0     2377 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/test_element.py
--rwxr-xr-x   0        0        0     4148 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/test_formatter.py
--rwxr-xr-x   0        0        0     3637 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/test_fuzz.py
--rwxr-xr-x   0        0        0     8322 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/test_html5lib.py
--rwxr-xr-x   0        0        0     6256 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/test_htmlparser.py
--rwxr-xr-x   0        0        0     7635 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/test_lxml.py
--rwxr-xr-x   0        0        0     5081 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/test_navigablestring.py
--rwxr-xr-x   0        0        0    14274 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/test_pageelement.py
--rwxr-xr-x   0        0        0    19877 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/test_soup.py
--rwxr-xr-x   0        0        0     9016 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/test_tag.py
--rwxr-xr-x   0        0        0    48129 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/test_tree.py
--rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-4818336571064320.testcase
--rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-4999465949331456.testcase
--rwxr-xr-x   0        0        0    19469 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5167584867909632.testcase
--rwxr-xr-x   0        0        0        5 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5703933063462912.testcase
--rwxr-xr-x   0        0        0       35 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5843991618256896.testcase
--rwxr-xr-x   0        0        0    51495 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-5984173902397440.testcase
--rwxr-xr-x   0        0        0    10380 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6124268085182464.testcase
--rwxr-xr-x   0        0        0       19 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6241471367348224.testcase
--rwxr-xr-x   0        0        0     3546 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6450958476902400.testcase
--rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/fuzz/clusterfuzz-testcase-minimized-bs4_fuzzer-6600557255327744.testcase
--rwxr-xr-x   0        0        0     2607 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/tests/fuzz/crash-0d306a50c8ed8bcd0785b67000fcd5dea1d33f08.testcase
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4-0.0.1.dist-info/INSTALLER
--rwxr-xr-x   0        0        0      919 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4-0.0.1.dist-info/METADATA
--rwxr-xr-x   0        0        0      368 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4-0.0.1.dist-info/RECORD
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4-0.0.1.dist-info/WHEEL
--rwxr-xr-x   0        0        0        1 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4-0.0.1.dist-info/top_level.txt
--rwxr-xr-x   0        0        0       94 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/certifi/__init__.py
--rwxr-xr-x   0        0        0      243 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/certifi/__main__.py
--rwxr-xr-x   0        0        0   278952 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/certifi/cacert.pem
--rwxr-xr-x   0        0        0     4219 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/certifi/core.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/certifi/py.typed
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1052 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/LICENSE
--rwxr-xr-x   0        0        0     2190 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/METADATA
--rwxr-xr-x   0        0        0     1009 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/RECORD
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/WHEEL
--rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/top_level.txt
--rwxr-xr-x   0        0        0     1549 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/__init__.py
--rwxr-xr-x   0        0        0    18624 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/api.py
--rwxr-xr-x   0        0        0    12554 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/cd.py
--rwxr-xr-x   0        0        0    19101 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/constant.py
--rwxr-xr-x   0        0        0     2071 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/legacy.py
--rwxr-xr-x   0        0        0    17496 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/md.cpython-310-x86_64-linux-gnu.so
--rwxr-xr-x   0        0        0    18258 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/md.py
--rwxr-xr-x   0        0        0   424312 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/md__mypyc.cpython-310-x86_64-linux-gnu.so
--rwxr-xr-x   0        0        0    11492 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/models.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/py.typed
--rwxr-xr-x   0        0        0    11544 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/utils.py
--rwxr-xr-x   0        0        0       79 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/version.py
--rwxr-xr-x   0        0        0    20069 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/assets/__init__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/cli/__init__.py
--rwxr-xr-x   0        0        0     9744 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/cli/normalizer.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1070 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/LICENSE
--rwxr-xr-x   0        0        0    30983 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/METADATA
--rwxr-xr-x   0        0        0     2798 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/RECORD
--rwxr-xr-x   0        0        0      152 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/WHEEL
--rwxr-xr-x   0        0        0       76 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/entry_points.txt
--rwxr-xr-x   0        0        0       19 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/top_level.txt
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/hatch_project/__about__.py
--rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/hatch_project/__init__.py
--rwxr-xr-x   0        0        0      545 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/hatch_project/scraping.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/hatch_project-0.1.1.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1479 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/hatch_project-0.1.1.dist-info/METADATA
--rwxr-xr-x   0        0        0      933 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/hatch_project-0.1.1.dist-info/RECORD
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/hatch_project-0.1.1.dist-info/REQUESTED
--rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/hatch_project-0.1.1.dist-info/WHEEL
--rwxr-xr-x   0        0        0     1101 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/hatch_project-0.1.1.dist-info/licenses/LICENSE.txt
--rwxr-xr-x   0        0        0      849 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/idna/__init__.py
--rwxr-xr-x   0        0        0     3374 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/idna/codec.py
--rwxr-xr-x   0        0        0      321 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/idna/compat.py
--rwxr-xr-x   0        0        0    12950 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/idna/core.py
--rwxr-xr-x   0        0        0    44375 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/idna/idnadata.py
--rwxr-xr-x   0        0        0     1881 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/idna/intranges.py
--rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/idna/package_data.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/idna/py.typed
--rwxr-xr-x   0        0        0   206539 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/idna/uts46data.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/idna-3.4.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1523 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/idna-3.4.dist-info/LICENSE.md
--rwxr-xr-x   0        0        0     9830 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/idna-3.4.dist-info/METADATA
--rwxr-xr-x   0        0        0     1378 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/idna-3.4.dist-info/RECORD
--rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/idna-3.4.dist-info/WHEEL
--rwxr-xr-x   0        0        0      370 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/__init__.py
--rwxr-xr-x   0        0        0     1229 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/__main__.py
--rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/py.typed
--rwxr-xr-x   0        0        0      592 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/__init__.py
--rwxr-xr-x   0        0        0    10415 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/build_env.py
--rwxr-xr-x   0        0        0    10245 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/cache.py
--rwxr-xr-x   0        0        0    14128 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/configuration.py
--rwxr-xr-x   0        0        0    13567 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/exceptions.py
--rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/main.py
--rwxr-xr-x   0        0        0     7246 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/pyproject.py
--rwxr-xr-x   0        0        0     6671 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/self_outdated_check.py
--rwxr-xr-x   0        0        0    12100 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/wheel_builder.py
--rwxr-xr-x   0        0        0      136 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/cli/__init__.py
--rwxr-xr-x   0        0        0     6562 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/cli/autocompletion.py
--rwxr-xr-x   0        0        0     7810 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/cli/base_command.py
--rwxr-xr-x   0        0        0    29292 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/cli/cmdoptions.py
--rwxr-xr-x   0        0        0      787 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/cli/command_context.py
--rwxr-xr-x   0        0        0     2542 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/cli/main.py
--rwxr-xr-x   0        0        0     2701 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/cli/main_parser.py
--rwxr-xr-x   0        0        0    11080 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/cli/parser.py
--rwxr-xr-x   0        0        0     8550 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/cli/progress_bars.py
--rwxr-xr-x   0        0        0    17001 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/cli/req_command.py
--rwxr-xr-x   0        0        0     5233 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/cli/spinners.py
--rwxr-xr-x   0        0        0      122 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/cli/status_codes.py
--rwxr-xr-x   0        0        0     3888 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/__init__.py
--rwxr-xr-x   0        0        0     7453 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/cache.py
--rwxr-xr-x   0        0        0     1617 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/check.py
--rwxr-xr-x   0        0        0     3005 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/completion.py
--rwxr-xr-x   0        0        0     9228 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/configuration.py
--rwxr-xr-x   0        0        0     6851 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/debug.py
--rwxr-xr-x   0        0        0     5088 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/download.py
--rwxr-xr-x   0        0        0     2869 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/freeze.py
--rwxr-xr-x   0        0        0     1719 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/hash.py
--rwxr-xr-x   0        0        0     1173 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/help.py
--rwxr-xr-x   0        0        0     4920 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/index.py
--rwxr-xr-x   0        0        0    28243 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/install.py
--rwxr-xr-x   0        0        0    12090 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/list.py
--rwxr-xr-x   0        0        0     5707 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/search.py
--rwxr-xr-x   0        0        0     8208 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/show.py
--rwxr-xr-x   0        0        0     3580 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/uninstall.py
--rwxr-xr-x   0        0        0     6365 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/wheel.py
--rwxr-xr-x   0        0        0      879 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/distributions/__init__.py
--rwxr-xr-x   0        0        0     1244 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/distributions/base.py
--rwxr-xr-x   0        0        0      667 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/distributions/installed.py
--rwxr-xr-x   0        0        0     3957 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/distributions/sdist.py
--rwxr-xr-x   0        0        0     1217 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/distributions/wheel.py
--rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/index/__init__.py
--rwxr-xr-x   0        0        0    18179 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/index/collector.py
--rwxr-xr-x   0        0        0    37120 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/index/package_finder.py
--rwxr-xr-x   0        0        0     6781 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/index/sources.py
--rwxr-xr-x   0        0        0    11584 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/locations/__init__.py
--rwxr-xr-x   0        0        0     6040 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/locations/_distutils.py
--rwxr-xr-x   0        0        0     8137 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/locations/_sysconfig.py
--rwxr-xr-x   0        0        0     1631 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/locations/base.py
--rwxr-xr-x   0        0        0     1624 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/metadata/__init__.py
--rwxr-xr-x   0        0        0     8170 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/metadata/base.py
--rwxr-xr-x   0        0        0     5353 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py
--rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/models/__init__.py
--rwxr-xr-x   0        0        0      977 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/models/candidate.py
--rwxr-xr-x   0        0        0     6482 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/models/direct_url.py
--rwxr-xr-x   0        0        0     2641 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/models/format_control.py
--rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/models/index.py
--rwxr-xr-x   0        0        0    10227 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/models/link.py
--rwxr-xr-x   0        0        0      769 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/models/scheme.py
--rwxr-xr-x   0        0        0     4600 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/models/search_scope.py
--rwxr-xr-x   0        0        0     1923 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/models/selection_prefs.py
--rwxr-xr-x   0        0        0     3981 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/models/target_python.py
--rwxr-xr-x   0        0        0     3633 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/models/wheel.py
--rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/network/__init__.py
--rwxr-xr-x   0        0        0    11961 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/network/auth.py
--rwxr-xr-x   0        0        0     2169 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/network/cache.py
--rwxr-xr-x   0        0        0     6200 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/network/download.py
--rwxr-xr-x   0        0        0     7825 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/network/lazy_wheel.py
--rwxr-xr-x   0        0        0    17036 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/network/session.py
--rwxr-xr-x   0        0        0     4155 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/network/utils.py
--rwxr-xr-x   0        0        0     1851 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/network/xmlrpc.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/operations/__init__.py
--rwxr-xr-x   0        0        0     5448 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/operations/check.py
--rwxr-xr-x   0        0        0    10833 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/operations/freeze.py
--rwxr-xr-x   0        0        0    25503 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/operations/prepare.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/operations/build/__init__.py
--rwxr-xr-x   0        0        0     1200 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/operations/build/metadata.py
--rwxr-xr-x   0        0        0     1991 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rwxr-xr-x   0        0        0     1144 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/operations/build/wheel.py
--rwxr-xr-x   0        0        0     3337 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/operations/install/__init__.py
--rwxr-xr-x   0        0        0     1443 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py
--rwxr-xr-x   0        0        0     4537 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/operations/install/legacy.py
--rwxr-xr-x   0        0        0    30269 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/operations/install/wheel.py
--rwxr-xr-x   0        0        0     2925 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/req/__init__.py
--rwxr-xr-x   0        0        0    16300 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/req/constructors.py
--rwxr-xr-x   0        0        0    17936 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/req/req_file.py
--rwxr-xr-x   0        0        0    32517 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/req/req_install.py
--rwxr-xr-x   0        0        0     7762 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/req/req_set.py
--rwxr-xr-x   0        0        0     4312 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/req/req_tracker.py
--rwxr-xr-x   0        0        0    24450 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/req/req_uninstall.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/resolution/__init__.py
--rwxr-xr-x   0        0        0      575 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/resolution/base.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/resolution/legacy/__init__.py
--rwxr-xr-x   0        0        0    18005 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rwxr-xr-x   0        0        0     5434 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py
--rwxr-xr-x   0        0        0    19397 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rwxr-xr-x   0        0        0    27559 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rwxr-xr-x   0        0        0     5427 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rwxr-xr-x   0        0        0     8617 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rwxr-xr-x   0        0        0     2669 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rwxr-xr-x   0        0        0     5621 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rwxr-xr-x   0        0        0    10795 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/__init__.py
--rwxr-xr-x   0        0        0     1053 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/_log.py
--rwxr-xr-x   0        0        0     1220 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/appdirs.py
--rwxr-xr-x   0        0        0     1947 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/compat.py
--rwxr-xr-x   0        0        0     5622 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/datetime.py
--rwxr-xr-x   0        0        0     3304 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/deprecation.py
--rwxr-xr-x   0        0        0     3073 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py
--rwxr-xr-x   0        0        0     1291 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/distutils_args.py
--rwxr-xr-x   0        0        0     1205 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/encoding.py
--rwxr-xr-x   0        0        0     1082 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/entrypoints.py
--rwxr-xr-x   0        0        0     6075 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/filesystem.py
--rwxr-xr-x   0        0        0      789 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/filetypes.py
--rwxr-xr-x   0        0        0     3262 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/glibc.py
--rwxr-xr-x   0        0        0     5332 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/hashes.py
--rwxr-xr-x   0        0        0      846 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/inject_securetransport.py
--rwxr-xr-x   0        0        0    12735 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/logging.py
--rwxr-xr-x   0        0        0    24472 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/misc.py
--rwxr-xr-x   0        0        0     1376 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/models.py
--rwxr-xr-x   0        0        0     2989 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/packaging.py
--rwxr-xr-x   0        0        0     3325 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/parallel.py
--rwxr-xr-x   0        0        0     1146 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/pkg_resources.py
--rwxr-xr-x   0        0        0     5220 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/setuptools_build.py
--rwxr-xr-x   0        0        0    10324 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/subprocess.py
--rwxr-xr-x   0        0        0     8210 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/temp_dir.py
--rwxr-xr-x   0        0        0     9317 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/unpacking.py
--rwxr-xr-x   0        0        0     1863 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/urls.py
--rwxr-xr-x   0        0        0     3675 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/virtualenv.py
--rwxr-xr-x   0        0        0     6479 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/wheel.py
--rwxr-xr-x   0        0        0      611 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/vcs/__init__.py
--rwxr-xr-x   0        0        0     3058 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/vcs/bazaar.py
--rwxr-xr-x   0        0        0    17853 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/vcs/git.py
--rwxr-xr-x   0        0        0     5234 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/vcs/mercurial.py
--rwxr-xr-x   0        0        0    12195 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/vcs/subversion.py
--rwxr-xr-x   0        0        0    23998 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py
--rwxr-xr-x   0        0        0     4814 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/__init__.py
--rwxr-xr-x   0        0        0    26540 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/appdirs.py
--rwxr-xr-x   0        0        0    44858 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distro.py
--rwxr-xr-x   0        0        0   280501 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pyparsing.py
--rwxr-xr-x   0        0        0    35547 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/six.py
--rwxr-xr-x   0        0        0      386 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/vendor.txt
--rwxr-xr-x   0        0        0      313 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/__init__.py
--rwxr-xr-x   0        0        0     1352 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rwxr-xr-x   0        0        0     5015 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py
--rwxr-xr-x   0        0        0      844 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py
--rwxr-xr-x   0        0        0      724 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/compat.py
--rwxr-xr-x   0        0        0    14525 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py
--rwxr-xr-x   0        0        0     2613 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rwxr-xr-x   0        0        0     4205 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rwxr-xr-x   0        0        0     7279 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py
--rwxr-xr-x   0        0        0      719 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rwxr-xr-x   0        0        0     4299 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rwxr-xr-x   0        0        0      889 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/certifi/__init__.py
--rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/certifi/__main__.py
--rwxr-xr-x   0        0        0   259465 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem
--rwxr-xr-x   0        0        0     2916 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/certifi/core.py
--rwxr-xr-x   0        0        0     3354 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/__init__.py
--rwxr-xr-x   0        0        0    31640 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/big5freq.py
--rwxr-xr-x   0        0        0     1804 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/big5prober.py
--rwxr-xr-x   0        0        0     9644 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py
--rwxr-xr-x   0        0        0     3946 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rwxr-xr-x   0        0        0     5255 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py
--rwxr-xr-x   0        0        0     3678 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rwxr-xr-x   0        0        0     1236 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/compat.py
--rwxr-xr-x   0        0        0     1904 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py
--rwxr-xr-x   0        0        0     1737 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/enums.py
--rwxr-xr-x   0        0        0     4051 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/escprober.py
--rwxr-xr-x   0        0        0    10756 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/escsm.py
--rwxr-xr-x   0        0        0     3841 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py
--rwxr-xr-x   0        0        0    13741 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py
--rwxr-xr-x   0        0        0     1795 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py
--rwxr-xr-x   0        0        0    32008 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py
--rwxr-xr-x   0        0        0     1793 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py
--rwxr-xr-x   0        0        0    20998 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py
--rwxr-xr-x   0        0        0     1800 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py
--rwxr-xr-x   0        0        0    14130 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py
--rwxr-xr-x   0        0        0    26102 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py
--rwxr-xr-x   0        0        0    19876 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py
--rwxr-xr-x   0        0        0   110347 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rwxr-xr-x   0        0        0   103969 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rwxr-xr-x   0        0        0   103159 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rwxr-xr-x   0        0        0   107148 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rwxr-xr-x   0        0        0   136898 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rwxr-xr-x   0        0        0   107695 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py
--rwxr-xr-x   0        0        0   100329 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rwxr-xr-x   0        0        0     5515 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py
--rwxr-xr-x   0        0        0     3504 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rwxr-xr-x   0        0        0     2066 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rwxr-xr-x   0        0        0    26053 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py
--rwxr-xr-x   0        0        0     6281 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rwxr-xr-x   0        0        0     4392 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rwxr-xr-x   0        0        0     3866 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py
--rwxr-xr-x   0        0        0    12789 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py
--rwxr-xr-x   0        0        0     2848 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/version.py
--rwxr-xr-x   0        0        0        2 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/cli/__init__.py
--rwxr-xr-x   0        0        0     2831 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rwxr-xr-x   0        0        0    19784 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py
--rwxr-xr-x   0        0        0      245 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/colorama/__init__.py
--rwxr-xr-x   0        0        0     2624 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/colorama/ansi.py
--rwxr-xr-x   0        0        0    10775 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py
--rwxr-xr-x   0        0        0     1995 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/colorama/initialise.py
--rwxr-xr-x   0        0        0     5556 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/colorama/win32.py
--rwxr-xr-x   0        0        0     6607 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/colorama/winterm.py
--rwxr-xr-x   0        0        0      604 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/__init__.py
--rwxr-xr-x   0        0        0    42528 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/compat.py
--rwxr-xr-x   0        0        0    52398 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/database.py
--rwxr-xr-x   0        0        0    21248 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/index.py
--rwxr-xr-x   0        0        0    53265 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/locators.py
--rwxr-xr-x   0        0        0    15204 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/manifest.py
--rwxr-xr-x   0        0        0     4474 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/markers.py
--rwxr-xr-x   0        0        0    40167 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/metadata.py
--rwxr-xr-x   0        0        0    11178 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/resources.py
--rwxr-xr-x   0        0        0    17671 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/scripts.py
--rwxr-xr-x   0        0        0    96768 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/t32.exe
--rwxr-xr-x   0        0        0   105984 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/t64.exe
--rwxr-xr-x   0        0        0    69523 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/util.py
--rwxr-xr-x   0        0        0    24247 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/version.py
--rwxr-xr-x   0        0        0    90112 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/w32.exe
--rwxr-xr-x   0        0        0    99840 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/w64.exe
--rwxr-xr-x   0        0        0    44118 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/wheel.py
--rwxr-xr-x   0        0        0      280 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/_backport/__init__.py
--rwxr-xr-x   0        0        0     1012 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/_backport/misc.py
--rwxr-xr-x   0        0        0    26471 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/_backport/shutil.py
--rwxr-xr-x   0        0        0     2701 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/_backport/sysconfig.cfg
--rwxr-xr-x   0        0        0    27640 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/_backport/sysconfig.py
--rwxr-xr-x   0        0        0    95235 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/_backport/tarfile.py
--rwxr-xr-x   0        0        0     1195 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/__init__.py
--rwxr-xr-x   0        0        0    17017 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_ihatexml.py
--rwxr-xr-x   0        0        0    33271 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_inputstream.py
--rwxr-xr-x   0        0        0    78775 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_tokenizer.py
--rwxr-xr-x   0        0        0     5090 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_utils.py
--rwxr-xr-x   0        0        0    86410 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/constants.py
--rwxr-xr-x   0        0        0   119981 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/html5parser.py
--rwxr-xr-x   0        0        0    16168 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/serializer.py
--rwxr-xr-x   0        0        0      114 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_trie/__init__.py
--rwxr-xr-x   0        0        0     1053 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_trie/_base.py
--rwxr-xr-x   0        0        0     1842 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_trie/py.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/__init__.py
--rwxr-xr-x   0        0        0      948 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py
--rwxr-xr-x   0        0        0      298 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/base.py
--rwxr-xr-x   0        0        0     3018 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/inject_meta_charset.py
--rwxr-xr-x   0        0        0     3736 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/lint.py
--rwxr-xr-x   0        0        0    10795 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/optionaltags.py
--rwxr-xr-x   0        0        0    27813 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/sanitizer.py
--rwxr-xr-x   0        0        0     1252 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/whitespace.py
--rwxr-xr-x   0        0        0      709 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treeadapters/__init__.py
--rwxr-xr-x   0        0        0     1769 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treeadapters/genshi.py
--rwxr-xr-x   0        0        0     1826 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treeadapters/sax.py
--rwxr-xr-x   0        0        0     3680 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/__init__.py
--rwxr-xr-x   0        0        0    14982 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/base.py
--rwxr-xr-x   0        0        0     9164 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/dom.py
--rwxr-xr-x   0        0        0    13179 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/etree.py
--rwxr-xr-x   0        0        0    15158 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py
--rwxr-xr-x   0        0        0     5873 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/__init__.py
--rwxr-xr-x   0        0        0     7728 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/base.py
--rwxr-xr-x   0        0        0     1456 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/dom.py
--rwxr-xr-x   0        0        0     4682 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/etree.py
--rwxr-xr-x   0        0        0     6572 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py
--rwxr-xr-x   0        0        0     2378 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/genshi.py
--rwxr-xr-x   0        0        0      893 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/idna/__init__.py
--rwxr-xr-x   0        0        0     3570 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/idna/codec.py
--rwxr-xr-x   0        0        0      376 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/idna/compat.py
--rwxr-xr-x   0        0        0    13235 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/idna/core.py
--rwxr-xr-x   0        0        0    44400 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/idna/idnadata.py
--rwxr-xr-x   0        0        0     1991 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/idna/intranges.py
--rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/idna/package_data.py
--rwxr-xr-x   0        0        0   210287 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/idna/uts46data.py
--rwxr-xr-x   0        0        0     1172 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/msgpack/__init__.py
--rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/msgpack/_version.py
--rwxr-xr-x   0        0        0     1129 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py
--rwxr-xr-x   0        0        0     6281 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/msgpack/ext.py
--rwxr-xr-x   0        0        0    39113 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/msgpack/fallback.py
--rwxr-xr-x   0        0        0      687 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/packaging/__about__.py
--rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/packaging/__init__.py
--rwxr-xr-x   0        0        0    11789 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py
--rwxr-xr-x   0        0        0     4514 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py
--rwxr-xr-x   0        0        0     1696 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/packaging/_structures.py
--rwxr-xr-x   0        0        0     8791 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/packaging/markers.py
--rwxr-xr-x   0        0        0     4822 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/packaging/requirements.py
--rwxr-xr-x   0        0        0    31792 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/packaging/specifiers.py
--rwxr-xr-x   0        0        0    16198 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/packaging/tags.py
--rwxr-xr-x   0        0        0     4336 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/packaging/utils.py
--rwxr-xr-x   0        0        0    15169 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/packaging/version.py
--rwxr-xr-x   0        0        0      136 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pep517/__init__.py
--rwxr-xr-x   0        0        0     3596 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pep517/build.py
--rwxr-xr-x   0        0        0     6303 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pep517/check.py
--rwxr-xr-x   0        0        0     4213 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pep517/colorlog.py
--rwxr-xr-x   0        0        0     1113 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pep517/compat.py
--rwxr-xr-x   0        0        0     1173 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pep517/dirtools.py
--rwxr-xr-x   0        0        0     6283 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pep517/envbuild.py
--rwxr-xr-x   0        0        0     2555 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pep517/meta.py
--rwxr-xr-x   0        0        0    13629 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pep517/wrappers.py
--rwxr-xr-x   0        0        0      580 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/__init__.py
--rwxr-xr-x   0        0        0    11182 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/_in_process.py
--rwxr-xr-x   0        0        0   111573 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py
--rwxr-xr-x   0        0        0      585 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pkg_resources/py31compat.py
--rwxr-xr-x   0        0        0     5034 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/progress/__init__.py
--rwxr-xr-x   0        0        0     2945 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/progress/bar.py
--rwxr-xr-x   0        0        0     1413 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/progress/counter.py
--rwxr-xr-x   0        0        0     1423 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/progress/spinner.py
--rwxr-xr-x   0        0        0     5267 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/__init__.py
--rwxr-xr-x   0        0        0      455 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/__version__.py
--rwxr-xr-x   0        0        0     1138 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py
--rwxr-xr-x   0        0        0    22081 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/adapters.py
--rwxr-xr-x   0        0        0     6561 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/api.py
--rwxr-xr-x   0        0        0    10512 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/auth.py
--rwxr-xr-x   0        0        0      483 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/certs.py
--rwxr-xr-x   0        0        0     2121 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/compat.py
--rwxr-xr-x   0        0        0    18979 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/cookies.py
--rwxr-xr-x   0        0        0     3377 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/exceptions.py
--rwxr-xr-x   0        0        0     4104 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/help.py
--rwxr-xr-x   0        0        0      791 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/hooks.py
--rwxr-xr-x   0        0        0    35890 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/models.py
--rwxr-xr-x   0        0        0      711 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/packages.py
--rwxr-xr-x   0        0        0    30949 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/sessions.py
--rwxr-xr-x   0        0        0     4311 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/status_codes.py
--rwxr-xr-x   0        0        0     3110 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/structures.py
--rwxr-xr-x   0        0        0    32407 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/utils.py
--rwxr-xr-x   0        0        0      563 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py
--rwxr-xr-x   0        0        0     5762 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/resolvelib/providers.py
--rwxr-xr-x   0        0        0     1401 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py
--rwxr-xr-x   0        0        0    17698 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py
--rwxr-xr-x   0        0        0     4959 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/resolvelib/structs.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rwxr-xr-x   0        0        0      162 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rwxr-xr-x   0        0        0    18774 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/__init__.py
--rwxr-xr-x   0        0        0     3406 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py
--rwxr-xr-x   0        0        0     2012 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/_utils.py
--rwxr-xr-x   0        0        0     1542 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/after.py
--rwxr-xr-x   0        0        0     1417 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/before.py
--rwxr-xr-x   0        0        0     1966 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py
--rwxr-xr-x   0        0        0     1426 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/nap.py
--rwxr-xr-x   0        0        0     6858 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/retry.py
--rwxr-xr-x   0        0        0     2886 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/stop.py
--rwxr-xr-x   0        0        0     2204 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rwxr-xr-x   0        0        0     6882 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/wait.py
--rwxr-xr-x   0        0        0      236 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tomli/__init__.py
--rwxr-xr-x   0        0        0    23118 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tomli/_parser.py
--rwxr-xr-x   0        0        0     2764 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tomli/_re.py
--rwxr-xr-x   0        0        0     2848 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/__init__.py
--rwxr-xr-x   0        0        0    11148 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/_collections.py
--rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/_version.py
--rwxr-xr-x   0        0        0    19293 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/connection.py
--rwxr-xr-x   0        0        0    38198 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py
--rwxr-xr-x   0        0        0     8540 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py
--rwxr-xr-x   0        0        0     8853 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/fields.py
--rwxr-xr-x   0        0        0     2538 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/filepost.py
--rwxr-xr-x   0        0        0    20299 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py
--rwxr-xr-x   0        0        0     6155 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/request.py
--rwxr-xr-x   0        0        0    29024 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/response.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rwxr-xr-x   0        0        0      993 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rwxr-xr-x   0        0        0    11348 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rwxr-xr-x   0        0        0     4668 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rwxr-xr-x   0        0        0    17402 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rwxr-xr-x   0        0        0    35356 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rwxr-xr-x   0        0        0     7313 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rwxr-xr-x   0        0        0    18168 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rwxr-xr-x   0        0        0    14304 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rwxr-xr-x   0        0        0    35743 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rwxr-xr-x   0        0        0     1468 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rwxr-xr-x   0        0        0      951 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py
--rwxr-xr-x   0        0        0     5839 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py
--rwxr-xr-x   0        0        0     1204 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py
--rwxr-xr-x   0        0        0     5070 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py
--rwxr-xr-x   0        0        0     1660 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py
--rwxr-xr-x   0        0        0      520 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/queue.py
--rwxr-xr-x   0        0        0     4266 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/request.py
--rwxr-xr-x   0        0        0     3617 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/response.py
--rwxr-xr-x   0        0        0    21993 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py
--rwxr-xr-x   0        0        0    17672 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rwxr-xr-x   0        0        0     7152 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rwxr-xr-x   0        0        0    10271 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py
--rwxr-xr-x   0        0        0    14479 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/url.py
--rwxr-xr-x   0        0        0     5557 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py
--rwxr-xr-x   0        0        0    10921 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/webencodings/__init__.py
--rwxr-xr-x   0        0        0     9210 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/webencodings/labels.py
--rwxr-xr-x   0        0        0     1364 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py
--rwxr-xr-x   0        0        0     6716 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/webencodings/tests.py
--rwxr-xr-x   0        0        0     4632 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip-21.2.3.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1110 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip-21.2.3.dist-info/LICENSE.txt
--rwxr-xr-x   0        0        0     4165 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip-21.2.3.dist-info/METADATA
--rwxr-xr-x   0        0        0    62024 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip-21.2.3.dist-info/RECORD
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip-21.2.3.dist-info/REQUESTED
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip-21.2.3.dist-info/WHEEL
--rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip-21.2.3.dist-info/entry_points.txt
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip-21.2.3.dist-info/top_level.txt
--rwxr-xr-x   0        0        0   108202 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/__init__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/__init__.py
--rwxr-xr-x   0        0        0    24701 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/appdirs.py
--rwxr-xr-x   0        0        0   232056 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/pyparsing.py
--rwxr-xr-x   0        0        0      736 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rwxr-xr-x   0        0        0      562 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rwxr-xr-x   0        0        0     1128 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_compat.py
--rwxr-xr-x   0        0        0     2022 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rwxr-xr-x   0        0        0     1812 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_typing.py
--rwxr-xr-x   0        0        0     9518 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/markers.py
--rwxr-xr-x   0        0        0     4929 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rwxr-xr-x   0        0        0    31944 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rwxr-xr-x   0        0        0    24067 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/tags.py
--rwxr-xr-x   0        0        0     1811 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/utils.py
--rwxr-xr-x   0        0        0    15470 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/version.py
--rwxr-xr-x   0        0        0     2362 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/extern/__init__.py
--rwxr-xr-x   0        0        0      104 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/tests/data/my-test-package-source/setup.py
--rwxr-xr-x   0        0        0     4963 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/__init__.py
--rwxr-xr-x   0        0        0      435 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/__version__.py
--rwxr-xr-x   0        0        0     1495 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/_internal_utils.py
--rwxr-xr-x   0        0        0    19553 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/adapters.py
--rwxr-xr-x   0        0        0     6449 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/api.py
--rwxr-xr-x   0        0        0    10187 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/auth.py
--rwxr-xr-x   0        0        0      429 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/certs.py
--rwxr-xr-x   0        0        0     1451 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/compat.py
--rwxr-xr-x   0        0        0    18560 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/cookies.py
--rwxr-xr-x   0        0        0     3811 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/exceptions.py
--rwxr-xr-x   0        0        0     3875 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/help.py
--rwxr-xr-x   0        0        0      733 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/hooks.py
--rwxr-xr-x   0        0        0    35223 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/models.py
--rwxr-xr-x   0        0        0      957 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/packages.py
--rwxr-xr-x   0        0        0    30373 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/sessions.py
--rwxr-xr-x   0        0        0     4235 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/status_codes.py
--rwxr-xr-x   0        0        0     2912 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/structures.py
--rwxr-xr-x   0        0        0    33448 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/utils.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests-2.31.0.dist-info/INSTALLER
--rwxr-xr-x   0        0        0    10142 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests-2.31.0.dist-info/LICENSE
--rwxr-xr-x   0        0        0     4634 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests-2.31.0.dist-info/METADATA
--rwxr-xr-x   0        0        0     2761 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests-2.31.0.dist-info/RECORD
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests-2.31.0.dist-info/WHEEL
--rwxr-xr-x   0        0        0        9 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests-2.31.0.dist-info/top_level.txt
--rwxr-xr-x   0        0        0     7681 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/__init__.py
--rwxr-xr-x   0        0        0      218 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_deprecation_warning.py
--rwxr-xr-x   0        0        0     2392 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_imp.py
--rwxr-xr-x   0        0        0     7077 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/archive_util.py
--rwxr-xr-x   0        0        0    10280 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/build_meta.py
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/cli-32.exe
--rwxr-xr-x   0        0        0    74752 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/cli-64.exe
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/cli.exe
--rwxr-xr-x   0        0        0    22279 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/config.py
--rwxr-xr-x   0        0        0      949 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/dep_util.py
--rwxr-xr-x   0        0        0     5474 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/depends.py
--rwxr-xr-x   0        0        0    42591 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/dist.py
--rwxr-xr-x   0        0        0      524 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/errors.py
--rwxr-xr-x   0        0        0     1684 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/extension.py
--rwxr-xr-x   0        0        0     4873 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/glob.py
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/gui-32.exe
--rwxr-xr-x   0        0        0    75264 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/gui-64.exe
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/gui.exe
--rwxr-xr-x   0        0        0     3567 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/installer.py
--rwxr-xr-x   0        0        0      812 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/launch.py
--rwxr-xr-x   0        0        0     2335 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/lib2to3_ex.py
--rwxr-xr-x   0        0        0     5217 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/monkey.py
--rwxr-xr-x   0        0        0    50561 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/msvc.py
--rwxr-xr-x   0        0        0     3093 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/namespaces.py
--rwxr-xr-x   0        0        0    39886 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/package_index.py
--rwxr-xr-x   0        0        0      245 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/py34compat.py
--rwxr-xr-x   0        0        0    14151 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/sandbox.py
--rwxr-xr-x   0        0        0      218 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/script (dev).tmpl
--rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/script.tmpl
--rwxr-xr-x   0        0        0      941 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/unicode_utils.py
--rwxr-xr-x   0        0        0      144 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/version.py
--rwxr-xr-x   0        0        0     8288 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/wheel.py
--rwxr-xr-x   0        0        0      714 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/windows_support.py
--rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/__init__.py
--rwxr-xr-x   0        0        0    20813 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/_msvccompiler.py
--rwxr-xr-x   0        0        0     8572 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/archive_util.py
--rwxr-xr-x   0        0        0    14894 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/bcppcompiler.py
--rwxr-xr-x   0        0        0    47607 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/ccompiler.py
--rwxr-xr-x   0        0        0    18079 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/cmd.py
--rwxr-xr-x   0        0        0     4827 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/config.py
--rwxr-xr-x   0        0        0     8876 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/core.py
--rwxr-xr-x   0        0        0    16938 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/cygwinccompiler.py
--rwxr-xr-x   0        0        0      139 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/debug.py
--rwxr-xr-x   0        0        0     3491 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/dep_util.py
--rwxr-xr-x   0        0        0     7778 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/dir_util.py
--rwxr-xr-x   0        0        0    50421 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/dist.py
--rwxr-xr-x   0        0        0     3577 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/errors.py
--rwxr-xr-x   0        0        0    10515 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/extension.py
--rwxr-xr-x   0        0        0    17784 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/fancy_getopt.py
--rwxr-xr-x   0        0        0     8148 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/file_util.py
--rwxr-xr-x   0        0        0    13407 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/filelist.py
--rwxr-xr-x   0        0        0     1969 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/log.py
--rwxr-xr-x   0        0        0    30453 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/msvc9compiler.py
--rwxr-xr-x   0        0        0    23540 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/msvccompiler.py
--rwxr-xr-x   0        0        0      455 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/py35compat.py
--rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/py38compat.py
--rwxr-xr-x   0        0        0     3498 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/spawn.py
--rwxr-xr-x   0        0        0    21349 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/sysconfig.py
--rwxr-xr-x   0        0        0    12483 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/text_file.py
--rwxr-xr-x   0        0        0    14957 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/unixccompiler.py
--rwxr-xr-x   0        0        0    23185 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/util.py
--rwxr-xr-x   0        0        0    12514 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/version.py
--rwxr-xr-x   0        0        0     5133 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/versionpredicate.py
--rwxr-xr-x   0        0        0      799 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/__init__.py
--rwxr-xr-x   0        0        0     5562 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/bdist.py
--rwxr-xr-x   0        0        0     4913 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rwxr-xr-x   0        0        0    35579 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_msi.py
--rwxr-xr-x   0        0        0    21537 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rwxr-xr-x   0        0        0    16030 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_wininst.py
--rwxr-xr-x   0        0        0     5773 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/build.py
--rwxr-xr-x   0        0        0     8022 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/build_clib.py
--rwxr-xr-x   0        0        0    31720 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/build_ext.py
--rwxr-xr-x   0        0        0    17190 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/build_py.py
--rwxr-xr-x   0        0        0     6232 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/build_scripts.py
--rwxr-xr-x   0        0        0     5637 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/check.py
--rwxr-xr-x   0        0        0     2776 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/clean.py
--rwxr-xr-x   0        0        0    13117 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/config.py
--rwxr-xr-x   0        0        0    27488 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/install.py
--rwxr-xr-x   0        0        0     2822 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/install_data.py
--rwxr-xr-x   0        0        0     2603 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/install_egg_info.py
--rwxr-xr-x   0        0        0     1298 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/install_headers.py
--rwxr-xr-x   0        0        0     8397 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/install_lib.py
--rwxr-xr-x   0        0        0     2017 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/install_scripts.py
--rwxr-xr-x   0        0        0      671 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/py37compat.py
--rwxr-xr-x   0        0        0    11712 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/register.py
--rwxr-xr-x   0        0        0    19005 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/sdist.py
--rwxr-xr-x   0        0        0     7597 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/upload.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/__init__.py
--rwxr-xr-x   0        0        0    15130 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/ordered_set.py
--rwxr-xr-x   0        0        0   232056 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/pyparsing.py
--rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rwxr-xr-x   0        0        0   117968 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/more.py
--rwxr-xr-x   0        0        0    16256 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rwxr-xr-x   0        0        0      736 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/__about__.py
--rwxr-xr-x   0        0        0      562 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/__init__.py
--rwxr-xr-x   0        0        0     1128 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/_compat.py
--rwxr-xr-x   0        0        0     2022 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/_structures.py
--rwxr-xr-x   0        0        0     1812 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/_typing.py
--rwxr-xr-x   0        0        0     9509 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/markers.py
--rwxr-xr-x   0        0        0     4917 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/requirements.py
--rwxr-xr-x   0        0        0    31944 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/specifiers.py
--rwxr-xr-x   0        0        0    24067 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/tags.py
--rwxr-xr-x   0        0        0     1811 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/utils.py
--rwxr-xr-x   0        0        0    15470 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/version.py
--rwxr-xr-x   0        0        0      217 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/__init__.py
--rwxr-xr-x   0        0        0     2381 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/alias.py
--rwxr-xr-x   0        0        0    16604 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/bdist_egg.py
--rwxr-xr-x   0        0        0      900 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/bdist_rpm.py
--rwxr-xr-x   0        0        0     4415 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/build_clib.py
--rwxr-xr-x   0        0        0    13212 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/build_ext.py
--rwxr-xr-x   0        0        0     8930 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/build_py.py
--rwxr-xr-x   0        0        0     8045 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/develop.py
--rwxr-xr-x   0        0        0      960 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/dist_info.py
--rwxr-xr-x   0        0        0    85308 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/easy_install.py
--rwxr-xr-x   0        0        0    25335 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/egg_info.py
--rwxr-xr-x   0        0        0     4705 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/install.py
--rwxr-xr-x   0        0        0     2203 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/install_egg_info.py
--rwxr-xr-x   0        0        0     3875 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/install_lib.py
--rwxr-xr-x   0        0        0     2593 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/install_scripts.py
--rwxr-xr-x   0        0        0      628 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/launcher manifest.xml
--rwxr-xr-x   0        0        0     4946 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/py36compat.py
--rwxr-xr-x   0        0        0      468 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/register.py
--rwxr-xr-x   0        0        0     2128 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/rotate.py
--rwxr-xr-x   0        0        0      658 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/saveopts.py
--rwxr-xr-x   0        0        0     5967 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/sdist.py
--rwxr-xr-x   0        0        0     5051 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/setopt.py
--rwxr-xr-x   0        0        0     9490 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/test.py
--rwxr-xr-x   0        0        0      462 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/upload.py
--rwxr-xr-x   0        0        0     7218 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/upload_docs.py
--rwxr-xr-x   0        0        0     2407 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/extern/__init__.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools-57.4.0.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     1050 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools-57.4.0.dist-info/LICENSE
--rwxr-xr-x   0        0        0     4908 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools-57.4.0.dist-info/METADATA
--rwxr-xr-x   0        0        0    23214 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools-57.4.0.dist-info/RECORD
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools-57.4.0.dist-info/REQUESTED
--rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools-57.4.0.dist-info/WHEEL
--rwxr-xr-x   0        0        0     2869 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools-57.4.0.dist-info/entry_points.txt
--rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools-57.4.0.dist-info/top_level.txt
--rwxr-xr-x   0        0        0     4630 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/soupsieve/__init__.py
--rwxr-xr-x   0        0        0     6842 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/soupsieve/__meta__.py
--rwxr-xr-x   0        0        0    58152 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/soupsieve/css_match.py
--rwxr-xr-x   0        0        0    47063 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/soupsieve/css_parser.py
--rwxr-xr-x   0        0        0    10337 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/soupsieve/css_types.py
--rwxr-xr-x   0        0        0     4053 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/soupsieve/pretty.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/soupsieve/py.typed
--rwxr-xr-x   0        0        0     3374 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/soupsieve/util.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/soupsieve-2.4.1.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     4731 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/soupsieve-2.4.1.dist-info/METADATA
--rwxr-xr-x   0        0        0     1383 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/soupsieve-2.4.1.dist-info/RECORD
--rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/soupsieve-2.4.1.dist-info/WHEEL
--rwxr-xr-x   0        0        0     1096 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/soupsieve-2.4.1.dist-info/licenses/LICENSE.md
--rwxr-xr-x   0        0        0     5283 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/__init__.py
--rwxr-xr-x   0        0        0     5651 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/_base_connection.py
--rwxr-xr-x   0        0        0    15561 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/_collections.py
--rwxr-xr-x   0        0        0     7756 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/_request_methods.py
--rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/_version.py
--rwxr-xr-x   0        0        0    33622 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/connection.py
--rwxr-xr-x   0        0        0    42961 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/connectionpool.py
--rwxr-xr-x   0        0        0     9385 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/exceptions.py
--rwxr-xr-x   0        0        0    11026 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/fields.py
--rwxr-xr-x   0        0        0     2395 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/filepost.py
--rwxr-xr-x   0        0        0    22648 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/poolmanager.py
--rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/py.typed
--rwxr-xr-x   0        0        0    40092 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/response.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/contrib/__init__.py
--rwxr-xr-x   0        0        0    19437 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/contrib/pyopenssl.py
--rwxr-xr-x   0        0        0    34121 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/contrib/securetransport.py
--rwxr-xr-x   0        0        0     7715 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/contrib/socks.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/contrib/_securetransport/__init__.py
--rwxr-xr-x   0        0        0    14452 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/contrib/_securetransport/bindings.py
--rwxr-xr-x   0        0        0    16220 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/contrib/_securetransport/low_level.py
--rwxr-xr-x   0        0        0     1051 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/__init__.py
--rwxr-xr-x   0        0        0     4462 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/connection.py
--rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/proxy.py
--rwxr-xr-x   0        0        0     8111 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/request.py
--rwxr-xr-x   0        0        0     3374 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/response.py
--rwxr-xr-x   0        0        0    18374 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/retry.py
--rwxr-xr-x   0        0        0    18860 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/ssl_.py
--rwxr-xr-x   0        0        0     5812 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/ssl_match_hostname.py
--rwxr-xr-x   0        0        0     9045 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/ssltransport.py
--rwxr-xr-x   0        0        0    10529 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/timeout.py
--rwxr-xr-x   0        0        0    15213 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/url.py
--rwxr-xr-x   0        0        0     1146 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/util.py
--rwxr-xr-x   0        0        0     4423 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/wait.py
--rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3-2.0.3.dist-info/INSTALLER
--rwxr-xr-x   0        0        0     6591 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3-2.0.3.dist-info/METADATA
--rwxr-xr-x   0        0        0     4877 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3-2.0.3.dist-info/RECORD
--rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3-2.0.3.dist-info/WHEEL
--rwxr-xr-x   0        0        0     1093 2020-02-02 00:00:00.000000 hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3-2.0.3.dist-info/licenses/LICENSE.txt
--rwxr-xr-x   0        0        0       55 2020-02-02 00:00:00.000000 hatch_project-0.1.2/src/__init__.py
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 hatch_project-0.1.2/src/hatch_project/__about__.py
--rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 hatch_project-0.1.2/src/hatch_project/__init__.py
--rwxr-xr-x   0        0        0      545 2020-02-02 00:00:00.000000 hatch_project-0.1.2/src/hatch_project/scraping.py
--rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 hatch_project-0.1.2/tests/__init__.py
--rwxr-xr-x   0        0        0      955 2020-02-02 00:00:00.000000 hatch_project-0.1.2/tests/test_scraping.py
--rwxr-xr-x   0        0        0     1101 2020-02-02 00:00:00.000000 hatch_project-0.1.2/LICENSE.txt
--rwxr-xr-x   0        0        0      513 2020-02-02 00:00:00.000000 hatch_project-0.1.2/README.md
--rwxr-xr-x   0        0        0     3343 2020-02-02 00:00:00.000000 hatch_project-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 hatch_project-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 hatch_project-0.2.0/requirements.txt
+-rwxr-xr-x   0        0        0       74 2020-02-02 00:00:00.000000 hatch_project-0.2.0/uninstall.txt
+-rwxr-xr-x   0        0        0      406 2020-02-02 00:00:00.000000 hatch_project-0.2.0/uninstall2.txt
+-rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/pyvenv.cfg
+-rwxr-xr-x   0        0        0     9033 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/Activate.ps1
+-rwxr-xr-x   0        0        0     2030 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/activate
+-rwxr-xr-x   0        0        0      956 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/activate.csh
+-rwxr-xr-x   0        0        0     2098 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/activate.fish
+-rwxr-xr-x   0        0        0      273 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/docutils
+-rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/keyring
+-rwxr-xr-x   0        0        0      277 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/markdown-it
+-rwxr-xr-x   0        0        0      301 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/normalizer
+-rwxr-xr-x   0        0        0      278 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/pip
+-rwxr-xr-x   0        0        0      278 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/pip3
+-rwxr-xr-x   0        0        0      278 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/pip3.10
+-rwxr-xr-x   0        0        0      275 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/pkginfo
+-rwxr-xr-x   0        0        0      272 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/pygmentize
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/python -> python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/python3 -> /home/kenno/.pyenv/versions/3.10.0/bin/python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/python3.10 -> python3
+-rwxr-xr-x   0        0        0      659 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/rst2html.py
+-rwxr-xr-x   0        0        0      781 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/rst2html4.py
+-rwxr-xr-x   0        0        0     1116 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/rst2html5.py
+-rwxr-xr-x   0        0        0      858 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/rst2latex.py
+-rwxr-xr-x   0        0        0      681 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/rst2man.py
+-rwxr-xr-x   0        0        0      847 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/rst2odt.py
+-rwxr-xr-x   0        0        0      653 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0        0        0      666 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/rst2pseudoxml.py
+-rwxr-xr-x   0        0        0      702 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/rst2s5.py
+-rwxr-xr-x   0        0        0      938 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/rst2xetex.py
+-rwxr-xr-x   0        0        0      667 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/rst2xml.py
+-rwxr-xr-x   0        0        0      735 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/rstpep2html.py
+-rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/bin/twine
+-rwxr-xr-x   0        0        0   983760 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/_cffi_backend.cpython-310-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0      152 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/distutils-precedence.pth
+-rwxr-xr-x   0        0        0    34549 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/six.py
+-rwxr-xr-x   0        0        0     9974 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/Pygments-2.15.1.dist-info/AUTHORS
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/Pygments-2.15.1.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1331 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/Pygments-2.15.1.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     2451 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/Pygments-2.15.1.dist-info/METADATA
+-rwxr-xr-x   0        0        0    42567 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/Pygments-2.15.1.dist-info/RECORD
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/Pygments-2.15.1.dist-info/WHEEL
+-rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/Pygments-2.15.1.dist-info/entry_points.txt
+-rwxr-xr-x   0        0        0        9 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/Pygments-2.15.1.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/SecretStorage-3.3.3.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1504 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/SecretStorage-3.3.3.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     4027 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/SecretStorage-3.3.3.dist-info/METADATA
+-rwxr-xr-x   0        0        0     1540 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/SecretStorage-3.3.3.dist-info/RECORD
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/SecretStorage-3.3.3.dist-info/WHEEL
+-rwxr-xr-x   0        0        0       14 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/SecretStorage-3.3.3.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0     3688 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/_distutils_hack/__init__.py
+-rwxr-xr-x   0        0        0       44 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/_distutils_hack/override.py
+-rwxr-xr-x   0        0        0     3649 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/__init__.py
+-rwxr-xr-x   0        0        0      752 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/callbacks.py
+-rwxr-xr-x   0        0        0     2526 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/css_sanitizer.py
+-rwxr-xr-x   0        0        0    22779 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/html5lib_shim.py
+-rwxr-xr-x   0        0        0    22350 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/linkifier.py
+-rwxr-xr-x   0        0        0       50 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/parse_shim.py
+-rwxr-xr-x   0        0        0    21934 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/sanitizer.py
+-rwxr-xr-x   0        0        0     2160 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/README.rst
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/__init__.py
+-rwxr-xr-x   0        0        0    39023 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/parse.py
+-rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/parse.py.SHA256SUM
+-rwxr-xr-x   0        0        0      184 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/vendor.txt
+-rwxr-xr-x   0        0        0      453 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/vendor_install.sh
+-rwxr-xr-x   0        0        0     1143 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/__init__.py
+-rwxr-xr-x   0        0        0    16728 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/_ihatexml.py
+-rwxr-xr-x   0        0        0    32300 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/_inputstream.py
+-rwxr-xr-x   0        0        0    77028 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/_tokenizer.py
+-rwxr-xr-x   0        0        0     4919 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/_utils.py
+-rwxr-xr-x   0        0        0    83464 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/constants.py
+-rwxr-xr-x   0        0        0   117174 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/html5parser.py
+-rwxr-xr-x   0        0        0    15747 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/serializer.py
+-rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/_trie/__init__.py
+-rwxr-xr-x   0        0        0     1013 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/_trie/_base.py
+-rwxr-xr-x   0        0        0     1763 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/_trie/py.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/filters/__init__.py
+-rwxr-xr-x   0        0        0      919 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/filters/alphabeticalattributes.py
+-rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/filters/base.py
+-rwxr-xr-x   0        0        0     2945 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/filters/inject_meta_charset.py
+-rwxr-xr-x   0        0        0     3631 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/filters/lint.py
+-rwxr-xr-x   0        0        0    10588 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/filters/optionaltags.py
+-rwxr-xr-x   0        0        0    26885 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/filters/sanitizer.py
+-rwxr-xr-x   0        0        0     1214 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/filters/whitespace.py
+-rwxr-xr-x   0        0        0      650 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/treeadapters/__init__.py
+-rwxr-xr-x   0        0        0     1715 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/treeadapters/genshi.py
+-rwxr-xr-x   0        0        0     1776 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/treeadapters/sax.py
+-rwxr-xr-x   0        0        0     3592 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/treebuilders/__init__.py
+-rwxr-xr-x   0        0        0    14553 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/treebuilders/base.py
+-rwxr-xr-x   0        0        0     8925 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/treebuilders/dom.py
+-rwxr-xr-x   0        0        0    12824 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/treebuilders/etree.py
+-rwxr-xr-x   0        0        0    14754 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/treebuilders/etree_lxml.py
+-rwxr-xr-x   0        0        0     5719 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/treewalkers/__init__.py
+-rwxr-xr-x   0        0        0     7476 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/treewalkers/base.py
+-rwxr-xr-x   0        0        0     1413 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/treewalkers/dom.py
+-rwxr-xr-x   0        0        0     4539 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/treewalkers/etree.py
+-rwxr-xr-x   0        0        0     6345 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/treewalkers/etree_lxml.py
+-rwxr-xr-x   0        0        0     2309 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib/treewalkers/genshi.py
+-rwxr-xr-x   0        0        0      983 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib-1.1.dist-info/AUTHORS.rst
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib-1.1.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1084 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib-1.1.dist-info/LICENSE
+-rwxr-xr-x   0        0        0    16076 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib-1.1.dist-info/METADATA
+-rwxr-xr-x   0        0        0     3486 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib-1.1.dist-info/RECORD
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib-1.1.dist-info/REQUESTED
+-rwxr-xr-x   0        0        0      110 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib-1.1.dist-info/WHEEL
+-rwxr-xr-x   0        0        0        9 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/_vendor/html5lib-1.1.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach-6.0.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0      569 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach-6.0.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0    29799 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach-6.0.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0     8498 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach-6.0.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach-6.0.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0        7 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach-6.0.0.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0       94 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/certifi/__init__.py
+-rwxr-xr-x   0        0        0      243 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/certifi/__main__.py
+-rwxr-xr-x   0        0        0   278952 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/certifi/cacert.pem
+-rwxr-xr-x   0        0        0     4219 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/certifi/core.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/certifi/py.typed
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1052 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     2190 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/METADATA
+-rwxr-xr-x   0        0        0     1009 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/RECORD
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/WHEEL
+-rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0      513 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi/__init__.py
+-rwxr-xr-x   0        0        0     3908 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi/_cffi_errors.h
+-rwxr-xr-x   0        0        0    14800 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi/_cffi_include.h
+-rwxr-xr-x   0        0        0    17680 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi/_embedding.h
+-rwxr-xr-x   0        0        0    42064 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi/api.py
+-rwxr-xr-x   0        0        0    42454 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi/backend_ctypes.py
+-rwxr-xr-x   0        0        0     5724 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi/cffi_opcode.py
+-rwxr-xr-x   0        0        0     2689 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi/commontypes.py
+-rwxr-xr-x   0        0        0    44231 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi/cparser.py
+-rwxr-xr-x   0        0        0      877 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi/error.py
+-rwxr-xr-x   0        0        0     4046 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi/ffiplatform.py
+-rwxr-xr-x   0        0        0      747 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi/lock.py
+-rwxr-xr-x   0        0        0    21768 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi/model.py
+-rwxr-xr-x   0        0        0     5976 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi/parse_c_type.h
+-rwxr-xr-x   0        0        0     4374 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi/pkgconfig.py
+-rwxr-xr-x   0        0        0    64598 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi/recompiler.py
+-rwxr-xr-x   0        0        0     8931 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi/setuptools_ext.py
+-rwxr-xr-x   0        0        0    43320 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi/vengine_cpy.py
+-rwxr-xr-x   0        0        0    26684 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi/vengine_gen.py
+-rwxr-xr-x   0        0        0    11253 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi/verifier.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi-1.15.1.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1294 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi-1.15.1.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     1144 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi-1.15.1.dist-info/METADATA
+-rwxr-xr-x   0        0        0     2913 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi-1.15.1.dist-info/RECORD
+-rwxr-xr-x   0        0        0      152 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi-1.15.1.dist-info/WHEEL
+-rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi-1.15.1.dist-info/entry_points.txt
+-rwxr-xr-x   0        0        0       19 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cffi-1.15.1.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0     1549 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/__init__.py
+-rwxr-xr-x   0        0        0    18624 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/api.py
+-rwxr-xr-x   0        0        0    12554 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/cd.py
+-rwxr-xr-x   0        0        0    19101 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/constant.py
+-rwxr-xr-x   0        0        0     2071 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/legacy.py
+-rwxr-xr-x   0        0        0    17496 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/md.cpython-310-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0    18258 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/md.py
+-rwxr-xr-x   0        0        0   424312 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/md__mypyc.cpython-310-x86_64-linux-gnu.so
+-rwxr-xr-x   0        0        0    11492 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/models.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/py.typed
+-rwxr-xr-x   0        0        0    11544 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/utils.py
+-rwxr-xr-x   0        0        0       79 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/version.py
+-rwxr-xr-x   0        0        0    20069 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/assets/__init__.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/cli/__init__.py
+-rwxr-xr-x   0        0        0     9744 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/cli/normalizer.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1070 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0    30983 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0     2798 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0      152 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0       76 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/entry_points.txt
+-rwxr-xr-x   0        0        0       19 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0      445 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/__about__.py
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/__init__.py
+-rwxr-xr-x   0        0        0     1118 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/exceptions.py
+-rwxr-xr-x   0        0        0     6886 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/fernet.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/py.typed
+-rwxr-xr-x   0        0        0     4018 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/utils.py
+-rwxr-xr-x   0        0        0      455 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/__init__.py
+-rwxr-xr-x   0        0        0    14441 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/_oid.py
+-rwxr-xr-x   0        0        0      361 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/backends/__init__.py
+-rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/backends/openssl/__init__.py
+-rwxr-xr-x   0        0        0    15967 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/backends/openssl/aead.py
+-rwxr-xr-x   0        0        0    73231 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/backends/openssl/backend.py
+-rwxr-xr-x   0        0        0    10358 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/backends/openssl/ciphers.py
+-rwxr-xr-x   0        0        0     3035 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/backends/openssl/cmac.py
+-rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/backends/openssl/decode_asn1.py
+-rwxr-xr-x   0        0        0    11474 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/backends/openssl/ec.py
+-rwxr-xr-x   0        0        0    21825 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/backends/openssl/rsa.py
+-rwxr-xr-x   0        0        0     2190 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/backends/openssl/utils.py
+-rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/bindings/__init__.py
+-rwxr-xr-x   0        0        0 13408352 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/bindings/_rust.abi3.so
+-rwxr-xr-x   0        0        0      981 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/bindings/_rust/__init__.pyi
+-rwxr-xr-x   0        0        0      230 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/bindings/_rust/_openssl.pyi
+-rwxr-xr-x   0        0        0      592 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/bindings/_rust/asn1.pyi
+-rwxr-xr-x   0        0        0      640 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/bindings/_rust/exceptions.pyi
+-rwxr-xr-x   0        0        0      905 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/bindings/_rust/ocsp.pyi
+-rwxr-xr-x   0        0        0      460 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/bindings/_rust/pkcs7.pyi
+-rwxr-xr-x   0        0        0     1878 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/bindings/_rust/x509.pyi
+-rwxr-xr-x   0        0        0      970 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/bindings/_rust/openssl/__init__.pyi
+-rwxr-xr-x   0        0        0      896 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/bindings/_rust/openssl/dh.pyi
+-rwxr-xr-x   0        0        0      764 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/bindings/_rust/openssl/dsa.pyi
+-rwxr-xr-x   0        0        0      629 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/bindings/_rust/openssl/ed25519.pyi
+-rwxr-xr-x   0        0        0      603 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/bindings/_rust/openssl/ed448.pyi
+-rwxr-xr-x   0        0        0      573 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/bindings/_rust/openssl/hashes.pyi
+-rwxr-xr-x   0        0        0      662 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/bindings/_rust/openssl/hmac.pyi
+-rwxr-xr-x   0        0        0      544 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/bindings/_rust/openssl/kdf.pyi
+-rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/bindings/_rust/openssl/poly1305.pyi
+-rwxr-xr-x   0        0        0      616 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/bindings/_rust/openssl/x25519.pyi
+-rwxr-xr-x   0        0        0      590 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/bindings/_rust/openssl/x448.pyi
+-rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/bindings/openssl/__init__.py
+-rwxr-xr-x   0        0        0     9098 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/bindings/openssl/_conditional.py
+-rwxr-xr-x   0        0        0     6696 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/bindings/openssl/binding.py
+-rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/__init__.py
+-rwxr-xr-x   0        0        0      532 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/_asymmetric.py
+-rwxr-xr-x   0        0        0     1093 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/_cipheralgorithm.py
+-rwxr-xr-x   0        0        0     5216 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/_serialization.py
+-rwxr-xr-x   0        0        0     2065 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/cmac.py
+-rwxr-xr-x   0        0        0      422 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/constant_time.py
+-rwxr-xr-x   0        0        0     5115 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/hashes.py
+-rwxr-xr-x   0        0        0      423 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/hmac.py
+-rwxr-xr-x   0        0        0     5678 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/keywrap.py
+-rwxr-xr-x   0        0        0     6242 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/padding.py
+-rwxr-xr-x   0        0        0      355 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/poly1305.py
+-rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/asymmetric/__init__.py
+-rwxr-xr-x   0        0        0     7013 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/asymmetric/dh.py
+-rwxr-xr-x   0        0        0     8263 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/asymmetric/dsa.py
+-rwxr-xr-x   0        0        0    12867 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/asymmetric/ec.py
+-rwxr-xr-x   0        0        0     3489 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/asymmetric/ed25519.py
+-rwxr-xr-x   0        0        0     3440 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/asymmetric/ed448.py
+-rwxr-xr-x   0        0        0     2717 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/asymmetric/padding.py
+-rwxr-xr-x   0        0        0    11623 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/asymmetric/rsa.py
+-rwxr-xr-x   0        0        0     2996 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/asymmetric/types.py
+-rwxr-xr-x   0        0        0      790 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/asymmetric/utils.py
+-rwxr-xr-x   0        0        0     3437 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/asymmetric/x25519.py
+-rwxr-xr-x   0        0        0     3358 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/asymmetric/x448.py
+-rwxr-xr-x   0        0        0      680 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/ciphers/__init__.py
+-rwxr-xr-x   0        0        0    12067 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/ciphers/aead.py
+-rwxr-xr-x   0        0        0     5000 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/ciphers/algorithms.py
+-rwxr-xr-x   0        0        0     8286 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/ciphers/base.py
+-rwxr-xr-x   0        0        0     8361 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/ciphers/modes.py
+-rwxr-xr-x   0        0        0      750 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/kdf/__init__.py
+-rwxr-xr-x   0        0        0     3726 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/kdf/concatkdf.py
+-rwxr-xr-x   0        0        0     3045 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/kdf/hkdf.py
+-rwxr-xr-x   0        0        0     9232 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/kdf/kbkdf.py
+-rwxr-xr-x   0        0        0     2012 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/kdf/pbkdf2.py
+-rwxr-xr-x   0        0        0     2354 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/kdf/scrypt.py
+-rwxr-xr-x   0        0        0     2002 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/kdf/x963kdf.py
+-rwxr-xr-x   0        0        0     1653 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/serialization/__init__.py
+-rwxr-xr-x   0        0        0     1986 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/serialization/base.py
+-rwxr-xr-x   0        0        0     6767 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/serialization/pkcs12.py
+-rwxr-xr-x   0        0        0     7392 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/serialization/pkcs7.py
+-rwxr-xr-x   0        0        0    50088 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/serialization/ssh.py
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/twofactor/__init__.py
+-rwxr-xr-x   0        0        0     3010 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/twofactor/hotp.py
+-rwxr-xr-x   0        0        0     1473 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/hazmat/primitives/twofactor/totp.py
+-rwxr-xr-x   0        0        0     7870 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/x509/__init__.py
+-rwxr-xr-x   0        0        0    35677 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/x509/base.py
+-rwxr-xr-x   0        0        0     2261 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/x509/certificate_transparency.py
+-rwxr-xr-x   0        0        0    68365 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/x509/extensions.py
+-rwxr-xr-x   0        0        0     7868 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/x509/general_name.py
+-rwxr-xr-x   0        0        0    14855 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/x509/name.py
+-rwxr-xr-x   0        0        0    18534 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/x509/ocsp.py
+-rwxr-xr-x   0        0        0      829 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography/x509/oid.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography-41.0.1.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography-41.0.1.dist-info/LICENSE
+-rwxr-xr-x   0        0        0    11360 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography-41.0.1.dist-info/LICENSE.APACHE
+-rwxr-xr-x   0        0        0     1532 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography-41.0.1.dist-info/LICENSE.BSD
+-rwxr-xr-x   0        0        0     5175 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography-41.0.1.dist-info/METADATA
+-rwxr-xr-x   0        0        0    15245 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography-41.0.1.dist-info/RECORD
+-rwxr-xr-x   0        0        0      148 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography-41.0.1.dist-info/WHEEL
+-rwxr-xr-x   0        0        0       13 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/cryptography-41.0.1.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0    10293 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/__init__.py
+-rwxr-xr-x   0        0        0     3625 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/__main__.py
+-rwxr-xr-x   0        0        0    33045 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/core.py
+-rwxr-xr-x   0        0        0     3961 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/examples.py
+-rwxr-xr-x   0        0        0    40002 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/frontend.py
+-rwxr-xr-x   0        0        0    23958 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/io.py
+-rwxr-xr-x   0        0        0    81006 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/nodes.py
+-rwxr-xr-x   0        0        0    56956 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/statemachine.py
+-rwxr-xr-x   0        0        0     2921 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/__init__.py
+-rwxr-xr-x   0        0        0     1831 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/af.py
+-rwxr-xr-x   0        0        0     1943 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/ar.py
+-rwxr-xr-x   0        0        0     1912 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/ca.py
+-rwxr-xr-x   0        0        0     1900 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/cs.py
+-rwxr-xr-x   0        0        0     1856 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/da.py
+-rwxr-xr-x   0        0        0     1728 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/de.py
+-rwxr-xr-x   0        0        0     1854 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/en.py
+-rwxr-xr-x   0        0        0     1931 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/eo.py
+-rwxr-xr-x   0        0        0     1906 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/es.py
+-rwxr-xr-x   0        0        0     1958 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/fa.py
+-rwxr-xr-x   0        0        0     1964 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/fi.py
+-rwxr-xr-x   0        0        0     1831 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/fr.py
+-rwxr-xr-x   0        0        0     1990 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/gl.py
+-rwxr-xr-x   0        0        0     2692 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/he.py
+-rwxr-xr-x   0        0        0     1814 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/it.py
+-rwxr-xr-x   0        0        0     1890 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/ja.py
+-rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/ko.py
+-rwxr-xr-x   0        0        0     1919 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/lt.py
+-rwxr-xr-x   0        0        0     1851 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/lv.py
+-rwxr-xr-x   0        0        0     1871 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/nl.py
+-rwxr-xr-x   0        0        0     1866 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/pl.py
+-rwxr-xr-x   0        0        0     1929 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/pt_br.py
+-rwxr-xr-x   0        0        0     2070 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/ru.py
+-rwxr-xr-x   0        0        0     1832 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/sk.py
+-rwxr-xr-x   0        0        0     1863 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/sv.py
+-rwxr-xr-x   0        0        0     2062 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/uk.py
+-rwxr-xr-x   0        0        0     1974 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/zh_cn.py
+-rwxr-xr-x   0        0        0     2742 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/languages/zh_tw.py
+-rwxr-xr-x   0        0        0     3724 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/__init__.py
+-rwxr-xr-x   0        0        0     1765 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/commonmark_wrapper.py
+-rwxr-xr-x   0        0        0      445 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/null.py
+-rwxr-xr-x   0        0        0     5426 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/recommonmark_wrapper.py
+-rwxr-xr-x   0        0        0    15954 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/__init__.py
+-rwxr-xr-x   0        0        0    16119 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/roles.py
+-rwxr-xr-x   0        0        0   132550 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/states.py
+-rwxr-xr-x   0        0        0    20912 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/tableparser.py
+-rwxr-xr-x   0        0        0    14652 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/directives/__init__.py
+-rwxr-xr-x   0        0        0     2405 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/directives/admonitions.py
+-rwxr-xr-x   0        0        0     9883 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/directives/body.py
+-rwxr-xr-x   0        0        0      695 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/directives/html.py
+-rwxr-xr-x   0        0        0     6799 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/directives/images.py
+-rwxr-xr-x   0        0        0    26302 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/directives/misc.py
+-rwxr-xr-x   0        0        0     4247 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/directives/parts.py
+-rwxr-xr-x   0        0        0      831 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/directives/references.py
+-rwxr-xr-x   0        0        0    23825 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/directives/tables.py
+-rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/README.txt
+-rwxr-xr-x   0        0        0    10925 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isoamsa.txt
+-rwxr-xr-x   0        0        0     7242 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isoamsb.txt
+-rwxr-xr-x   0        0        0     1723 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isoamsc.txt
+-rwxr-xr-x   0        0        0     6721 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isoamsn.txt
+-rwxr-xr-x   0        0        0     3825 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isoamso.txt
+-rwxr-xr-x   0        0        0    11763 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isoamsr.txt
+-rwxr-xr-x   0        0        0     3101 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isobox.txt
+-rwxr-xr-x   0        0        0     4241 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isocyr1.txt
+-rwxr-xr-x   0        0        0     1882 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isocyr2.txt
+-rwxr-xr-x   0        0        0      869 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isodia.txt
+-rwxr-xr-x   0        0        0     3010 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isogrk1.txt
+-rwxr-xr-x   0        0        0     1705 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isogrk2.txt
+-rwxr-xr-x   0        0        0     2880 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isogrk3.txt
+-rwxr-xr-x   0        0        0     3035 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isogrk4-wide.txt
+-rwxr-xr-x   0        0        0      372 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isogrk4.txt
+-rwxr-xr-x   0        0        0     4397 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isolat1.txt
+-rwxr-xr-x   0        0        0     8466 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isolat2.txt
+-rwxr-xr-x   0        0        0     3334 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isomfrk-wide.txt
+-rwxr-xr-x   0        0        0      519 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isomfrk.txt
+-rwxr-xr-x   0        0        0     1931 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isomopf-wide.txt
+-rwxr-xr-x   0        0        0      639 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isomopf.txt
+-rwxr-xr-x   0        0        0     3231 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isomscr-wide.txt
+-rwxr-xr-x   0        0        0      776 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isomscr.txt
+-rwxr-xr-x   0        0        0     4066 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isonum.txt
+-rwxr-xr-x   0        0        0     4613 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isopub.txt
+-rwxr-xr-x   0        0        0     9726 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/isotech.txt
+-rwxr-xr-x   0        0        0    45428 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/mmlalias.txt
+-rwxr-xr-x   0        0        0     9010 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/mmlextra-wide.txt
+-rwxr-xr-x   0        0        0     6800 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/mmlextra.txt
+-rwxr-xr-x   0        0        0     1036 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/s5defs.txt
+-rwxr-xr-x   0        0        0     6112 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/xhtml1-lat1.txt
+-rwxr-xr-x   0        0        0     1945 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/xhtml1-special.txt
+-rwxr-xr-x   0        0        0     7028 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/include/xhtml1-symbol.txt
+-rwxr-xr-x   0        0        0     1222 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/__init__.py
+-rwxr-xr-x   0        0        0     3727 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/af.py
+-rwxr-xr-x   0        0        0     3051 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/ar.py
+-rwxr-xr-x   0        0        0     4406 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/ca.py
+-rwxr-xr-x   0        0        0     4808 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/cs.py
+-rwxr-xr-x   0        0        0     3719 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/da.py
+-rwxr-xr-x   0        0        0     3547 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/de.py
+-rwxr-xr-x   0        0        0     3514 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/en.py
+-rwxr-xr-x   0        0        0     3825 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/eo.py
+-rwxr-xr-x   0        0        0     4158 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/es.py
+-rwxr-xr-x   0        0        0     3171 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/fa.py
+-rwxr-xr-x   0        0        0     3526 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/fi.py
+-rwxr-xr-x   0        0        0     3782 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/fr.py
+-rwxr-xr-x   0        0        0     3632 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/gl.py
+-rwxr-xr-x   0        0        0     3641 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/he.py
+-rwxr-xr-x   0        0        0     3322 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/it.py
+-rwxr-xr-x   0        0        0     3776 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/ja.py
+-rwxr-xr-x   0        0        0     3377 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/ko.py
+-rwxr-xr-x   0        0        0     3519 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/lt.py
+-rwxr-xr-x   0        0        0     3376 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/lv.py
+-rwxr-xr-x   0        0        0     3761 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/nl.py
+-rwxr-xr-x   0        0        0     3443 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/pl.py
+-rwxr-xr-x   0        0        0     3960 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/pt_br.py
+-rwxr-xr-x   0        0        0     3398 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/ru.py
+-rwxr-xr-x   0        0        0     3947 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/sk.py
+-rwxr-xr-x   0        0        0     3261 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/sv.py
+-rwxr-xr-x   0        0        0     3441 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/uk.py
+-rwxr-xr-x   0        0        0     3925 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/zh_cn.py
+-rwxr-xr-x   0        0        0     5160 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/parsers/rst/languages/zh_tw.py
+-rwxr-xr-x   0        0        0     3520 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/readers/__init__.py
+-rwxr-xr-x   0        0        0     1607 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/readers/doctree.py
+-rwxr-xr-x   0        0        0     1523 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/readers/pep.py
+-rwxr-xr-x   0        0        0     2324 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/readers/standalone.py
+-rwxr-xr-x   0        0        0     6870 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/transforms/__init__.py
+-rwxr-xr-x   0        0        0     2151 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/transforms/components.py
+-rwxr-xr-x   0        0        0    21371 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/transforms/frontmatter.py
+-rwxr-xr-x   0        0        0     4873 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/transforms/misc.py
+-rwxr-xr-x   0        0        0     6912 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/transforms/parts.py
+-rwxr-xr-x   0        0        0    11111 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/transforms/peps.py
+-rwxr-xr-x   0        0        0    36819 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/transforms/references.py
+-rwxr-xr-x   0        0        0    12548 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/transforms/universal.py
+-rwxr-xr-x   0        0        0     3057 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/transforms/writer_aux.py
+-rwxr-xr-x   0        0        0    29382 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/utils/__init__.py
+-rwxr-xr-x   0        0        0     4920 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/utils/code_analyzer.py
+-rwxr-xr-x   0        0        0     8105 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/utils/error_reporting.py
+-rwxr-xr-x   0        0        0     5747 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/utils/punctuation_chars.py
+-rwxr-xr-x   0        0        0     2695 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/utils/roman.py
+-rwxr-xr-x   0        0        0    38972 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/utils/smartquotes.py
+-rwxr-xr-x   0        0        0     6260 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/utils/urischemes.py
+-rwxr-xr-x   0        0        0     1825 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/utils/math/__init__.py
+-rwxr-xr-x   0        0        0    51496 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/utils/math/latex2mathml.py
+-rwxr-xr-x   0        0        0   107993 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/utils/math/math2html.py
+-rwxr-xr-x   0        0        0     6760 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/utils/math/tex2mathml_extern.py
+-rwxr-xr-x   0        0        0    37497 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/utils/math/tex2unichar.py
+-rwxr-xr-x   0        0        0    18393 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/utils/math/unichar2tex.py
+-rwxr-xr-x   0        0        0     4945 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/__init__.py
+-rwxr-xr-x   0        0        0    70896 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/_html_base.py
+-rwxr-xr-x   0        0        0     6763 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/docutils_xml.py
+-rwxr-xr-x   0        0        0    36654 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/manpage.py
+-rwxr-xr-x   0        0        0      568 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/null.py
+-rwxr-xr-x   0        0        0     1032 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/pseudoxml.py
+-rwxr-xr-x   0        0        0    37675 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/html4css1/__init__.py
+-rwxr-xr-x   0        0        0     7219 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/html4css1/html4css1.css
+-rwxr-xr-x   0        0        0      114 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/html4css1/template.txt
+-rwxr-xr-x   0        0        0    16718 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/html5_polyglot/__init__.py
+-rwxr-xr-x   0        0        0     6261 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/html5_polyglot/math.css
+-rwxr-xr-x   0        0        0     7388 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/html5_polyglot/minimal.css
+-rwxr-xr-x   0        0        0     7749 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/html5_polyglot/plain.css
+-rwxr-xr-x   0        0        0    11895 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/html5_polyglot/responsive.css
+-rwxr-xr-x   0        0        0      114 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/html5_polyglot/template.txt
+-rwxr-xr-x   0        0        0    12023 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/html5_polyglot/tuftig.css
+-rwxr-xr-x   0        0        0   137132 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/latex2e/__init__.py
+-rwxr-xr-x   0        0        0      422 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/latex2e/default.tex
+-rwxr-xr-x   0        0        0     5472 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/latex2e/docutils.sty
+-rwxr-xr-x   0        0        0      480 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/latex2e/titlepage.tex
+-rwxr-xr-x   0        0        0      424 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/latex2e/titlingpage.tex
+-rwxr-xr-x   0        0        0      672 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/latex2e/xelatex.tex
+-rwxr-xr-x   0        0        0   132358 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/odf_odt/__init__.py
+-rwxr-xr-x   0        0        0     2142 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/odf_odt/prepstyles.py
+-rwxr-xr-x   0        0        0     4681 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/odf_odt/pygmentsformatter.py
+-rwxr-xr-x   0        0        0    16500 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/odf_odt/styles.odt
+-rwxr-xr-x   0        0        0     3505 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/pep_html/__init__.py
+-rwxr-xr-x   0        0        0     6367 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/pep_html/pep.css
+-rwxr-xr-x   0        0        0     1001 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/pep_html/template.txt
+-rwxr-xr-x   0        0        0    14517 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/s5_html/__init__.py
+-rwxr-xr-x   0        0        0      278 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/s5_html/themes/README.txt
+-rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/s5_html/themes/big-black/__base__
+-rwxr-xr-x   0        0        0      910 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/s5_html/themes/big-black/framing.css
+-rwxr-xr-x   0        0        0     3605 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/s5_html/themes/big-black/pretty.css
+-rwxr-xr-x   0        0        0      905 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/s5_html/themes/big-white/framing.css
+-rwxr-xr-x   0        0        0     3565 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/s5_html/themes/big-white/pretty.css
+-rwxr-xr-x   0        0        0     1002 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/s5_html/themes/default/framing.css
+-rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/s5_html/themes/default/opera.css
+-rwxr-xr-x   0        0        0      648 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/s5_html/themes/default/outline.css
+-rwxr-xr-x   0        0        0     4383 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/s5_html/themes/default/pretty.css
+-rwxr-xr-x   0        0        0      818 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/s5_html/themes/default/print.css
+-rwxr-xr-x   0        0        0      450 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/s5_html/themes/default/s5-core.css
+-rwxr-xr-x   0        0        0      283 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/s5_html/themes/default/slides.css
+-rwxr-xr-x   0        0        0    15801 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/s5_html/themes/default/slides.js
+-rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/s5_html/themes/medium-black/__base__
+-rwxr-xr-x   0        0        0     4029 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/s5_html/themes/medium-black/pretty.css
+-rwxr-xr-x   0        0        0      943 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/s5_html/themes/medium-white/framing.css
+-rwxr-xr-x   0        0        0     3989 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/s5_html/themes/medium-white/pretty.css
+-rwxr-xr-x   0        0        0       40 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/s5_html/themes/small-black/__base__
+-rwxr-xr-x   0        0        0     4028 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/s5_html/themes/small-black/pretty.css
+-rwxr-xr-x   0        0        0      940 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/s5_html/themes/small-white/framing.css
+-rwxr-xr-x   0        0        0     3999 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/s5_html/themes/small-white/pretty.css
+-rwxr-xr-x   0        0        0     5736 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/writers/xetex/__init__.py
+-rwxr-xr-x   0        0        0     6292 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils-0.20.1.dist-info/COPYING.txt
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils-0.20.1.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     2817 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils-0.20.1.dist-info/METADATA
+-rwxr-xr-x   0        0        0    28169 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils-0.20.1.dist-info/RECORD
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils-0.20.1.dist-info/WHEEL
+-rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils-0.20.1.dist-info/entry_points.txt
+-rwxr-xr-x   0        0        0        9 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils-0.20.1.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0      849 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/idna/__init__.py
+-rwxr-xr-x   0        0        0     3374 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/idna/codec.py
+-rwxr-xr-x   0        0        0      321 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/idna/compat.py
+-rwxr-xr-x   0        0        0    12950 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/idna/core.py
+-rwxr-xr-x   0        0        0    44375 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/idna/idnadata.py
+-rwxr-xr-x   0        0        0     1881 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/idna/intranges.py
+-rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/idna/package_data.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/idna/py.typed
+-rwxr-xr-x   0        0        0   206539 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/idna/uts46data.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/idna-3.4.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1523 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/idna-3.4.dist-info/LICENSE.md
+-rwxr-xr-x   0        0        0     9830 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/idna-3.4.dist-info/METADATA
+-rwxr-xr-x   0        0        0     1378 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/idna-3.4.dist-info/RECORD
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/idna-3.4.dist-info/WHEEL
+-rwxr-xr-x   0        0        0    30724 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/importlib_metadata/__init__.py
+-rwxr-xr-x   0        0        0     2454 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/importlib_metadata/_adapters.py
+-rwxr-xr-x   0        0        0      743 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/importlib_metadata/_collections.py
+-rwxr-xr-x   0        0        0     1735 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/importlib_metadata/_compat.py
+-rwxr-xr-x   0        0        0     2895 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/importlib_metadata/_functools.py
+-rwxr-xr-x   0        0        0     2068 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/importlib_metadata/_itertools.py
+-rwxr-xr-x   0        0        0     1615 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/importlib_metadata/_meta.py
+-rwxr-xr-x   0        0        0     1098 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/importlib_metadata/_py39compat.py
+-rwxr-xr-x   0        0        0     2166 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/importlib_metadata/_text.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/importlib_metadata/py.typed
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/importlib_metadata-6.7.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0    11358 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/importlib_metadata-6.7.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     4878 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/importlib_metadata-6.7.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0     1961 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/importlib_metadata-6.7.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/importlib_metadata-6.7.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0       19 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/importlib_metadata-6.7.0.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jaraco/classes/__init__.py
+-rwxr-xr-x   0        0        0     1464 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jaraco/classes/ancestry.py
+-rwxr-xr-x   0        0        0     1853 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jaraco/classes/meta.py
+-rwxr-xr-x   0        0        0     3996 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jaraco/classes/properties.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jaraco.classes-3.2.3.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1050 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jaraco.classes-3.2.3.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     2943 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jaraco.classes-3.2.3.dist-info/METADATA
+-rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jaraco.classes-3.2.3.dist-info/RECORD
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jaraco.classes-3.2.3.dist-info/WHEEL
+-rwxr-xr-x   0        0        0        7 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jaraco.classes-3.2.3.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0      408 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/__init__.py
+-rwxr-xr-x   0        0        0     4933 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/auth.py
+-rwxr-xr-x   0        0        0     4054 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/bindgen.py
+-rwxr-xr-x   0        0        0     1817 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/bus.py
+-rwxr-xr-x   0        0        0     8140 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/bus_messages.py
+-rwxr-xr-x   0        0        0     5056 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/fds.py
+-rwxr-xr-x   0        0        0    19119 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/low_level.py
+-rwxr-xr-x   0        0        0     2827 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/routing.py
+-rwxr-xr-x   0        0        0     7979 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/wrappers.py
+-rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/io/__init__.py
+-rwxr-xr-x   0        0        0     7622 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/io/asyncio.py
+-rwxr-xr-x   0        0        0    12290 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/io/blocking.py
+-rwxr-xr-x   0        0        0     2696 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/io/common.py
+-rwxr-xr-x   0        0        0     9391 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/io/threading.py
+-rwxr-xr-x   0        0        0    14848 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/io/trio.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/io/tests/__init__.py
+-rwxr-xr-x   0        0        0     2730 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/io/tests/conftest.py
+-rwxr-xr-x   0        0        0     2636 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/io/tests/test_asyncio.py
+-rwxr-xr-x   0        0        0     2967 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/io/tests/test_blocking.py
+-rwxr-xr-x   0        0        0     2699 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/io/tests/test_threading.py
+-rwxr-xr-x   0        0        0     3892 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/io/tests/test_trio.py
+-rwxr-xr-x   0        0        0       79 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/io/tests/utils.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/tests/__init__.py
+-rwxr-xr-x   0        0        0     4575 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/tests/secrets_introspect.xml
+-rwxr-xr-x   0        0        0      611 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/tests/test_auth.py
+-rwxr-xr-x   0        0        0     1098 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/tests/test_bindgen.py
+-rwxr-xr-x   0        0        0      847 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/tests/test_bus.py
+-rwxr-xr-x   0        0        0     3228 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/tests/test_bus_messages.py
+-rwxr-xr-x   0        0        0     1821 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/tests/test_fds.py
+-rwxr-xr-x   0        0        0     2554 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/tests/test_low_level.py
+-rwxr-xr-x   0        0        0      959 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney/tests/test_routing.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney-0.8.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1081 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney-0.8.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     1280 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney-0.8.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0     4517 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney-0.8.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/jeepney-0.8.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/__init__.py
+-rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/__main__.py
+-rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/_compat.py
+-rwxr-xr-x   0        0        0     3886 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/_properties_compat.py
+-rwxr-xr-x   0        0        0     8100 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/backend.py
+-rwxr-xr-x   0        0        0      451 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/backend_complete.zsh
+-rwxr-xr-x   0        0        0     4400 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/cli.py
+-rwxr-xr-x   0        0        0     1324 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/completion.py
+-rwxr-xr-x   0        0        0     5593 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/core.py
+-rwxr-xr-x   0        0        0     1593 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/credentials.py
+-rwxr-xr-x   0        0        0      752 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/devpi_client.py
+-rwxr-xr-x   0        0        0     1430 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/errors.py
+-rwxr-xr-x   0        0        0     1231 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/http.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/py.typed
+-rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/py312compat.py
+-rwxr-xr-x   0        0        0     4692 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/backends/SecretService.py
+-rwxr-xr-x   0        0        0     5814 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/backends/Windows.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/backends/__init__.py
+-rwxr-xr-x   0        0        0     2173 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/backends/chainer.py
+-rwxr-xr-x   0        0        0      929 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/backends/fail.py
+-rwxr-xr-x   0        0        0     5830 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/backends/kwallet.py
+-rwxr-xr-x   0        0        0     5982 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/backends/libsecret.py
+-rwxr-xr-x   0        0        0      453 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/backends/null.py
+-rwxr-xr-x   0        0        0     2689 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/backends/macOS/__init__.py
+-rwxr-xr-x   0        0        0     4341 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/backends/macOS/api.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/testing/__init__.py
+-rwxr-xr-x   0        0        0     6598 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/testing/backend.py
+-rwxr-xr-x   0        0        0     1918 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/testing/util.py
+-rwxr-xr-x   0        0        0      868 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/util/__init__.py
+-rwxr-xr-x   0        0        0     2215 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring/util/platform_.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring-24.0.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1023 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring-24.0.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0    20511 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring-24.0.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0     4555 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring-24.0.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring-24.0.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0      334 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring-24.0.0.dist-info/entry_points.txt
+-rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/keyring-24.0.0.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/__init__.py
+-rwxr-xr-x   0        0        0      246 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/_compat.py
+-rwxr-xr-x   0        0        0     2364 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/_punycode.py
+-rwxr-xr-x   0        0        0    12772 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/main.py
+-rwxr-xr-x   0        0        0     3911 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/parser_block.py
+-rwxr-xr-x   0        0        0     1010 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/parser_core.py
+-rwxr-xr-x   0        0        0     4997 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/parser_inline.py
+-rwxr-xr-x   0        0        0     2446 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/port.yaml
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/py.typed
+-rwxr-xr-x   0        0        0     9970 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/renderer.py
+-rwxr-xr-x   0        0        0     9199 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/ruler.py
+-rwxr-xr-x   0        0        0     6439 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/token.py
+-rwxr-xr-x   0        0        0    11421 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/tree.py
+-rwxr-xr-x   0        0        0     5365 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/utils.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/cli/__init__.py
+-rwxr-xr-x   0        0        0     2901 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/cli/parse.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/common/__init__.py
+-rwxr-xr-x   0        0        0      156 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/common/entities.py
+-rwxr-xr-x   0        0        0      932 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/common/html_blocks.py
+-rwxr-xr-x   0        0        0      929 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/common/html_re.py
+-rwxr-xr-x   0        0        0     2568 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/common/normalize_url.py
+-rwxr-xr-x   0        0        0    10728 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/common/utils.py
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/helpers/__init__.py
+-rwxr-xr-x   0        0        0     1977 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/helpers/parse_link_destination.py
+-rwxr-xr-x   0        0        0     1036 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/helpers/parse_link_label.py
+-rwxr-xr-x   0        0        0     1425 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/helpers/parse_link_title.py
+-rwxr-xr-x   0        0        0      970 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/presets/__init__.py
+-rwxr-xr-x   0        0        0     2868 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/presets/commonmark.py
+-rwxr-xr-x   0        0        0     1810 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/presets/default.py
+-rwxr-xr-x   0        0        0     2112 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/presets/zero.py
+-rwxr-xr-x   0        0        0      553 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_block/__init__.py
+-rwxr-xr-x   0        0        0     8887 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_block/blockquote.py
+-rwxr-xr-x   0        0        0      859 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_block/code.py
+-rwxr-xr-x   0        0        0     2537 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_block/fence.py
+-rwxr-xr-x   0        0        0     1746 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_block/heading.py
+-rwxr-xr-x   0        0        0     1226 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_block/hr.py
+-rwxr-xr-x   0        0        0     2721 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_block/html_block.py
+-rwxr-xr-x   0        0        0     2625 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_block/lheading.py
+-rwxr-xr-x   0        0        0     9668 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_block/list.py
+-rwxr-xr-x   0        0        0     1818 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_block/paragraph.py
+-rwxr-xr-x   0        0        0     6168 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_block/reference.py
+-rwxr-xr-x   0        0        0     8422 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_block/state_block.py
+-rwxr-xr-x   0        0        0     6987 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_block/table.py
+-rwxr-xr-x   0        0        0      394 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_core/__init__.py
+-rwxr-xr-x   0        0        0      372 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_core/block.py
+-rwxr-xr-x   0        0        0      325 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_core/inline.py
+-rwxr-xr-x   0        0        0     5141 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_core/linkify.py
+-rwxr-xr-x   0        0        0      402 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_core/normalize.py
+-rwxr-xr-x   0        0        0     3470 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_core/replacements.py
+-rwxr-xr-x   0        0        0     7443 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_core/smartquotes.py
+-rwxr-xr-x   0        0        0      570 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_core/state_core.py
+-rwxr-xr-x   0        0        0     1172 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_core/text_join.py
+-rwxr-xr-x   0        0        0      696 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_inline/__init__.py
+-rwxr-xr-x   0        0        0     2079 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_inline/autolink.py
+-rwxr-xr-x   0        0        0     2037 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_inline/backticks.py
+-rwxr-xr-x   0        0        0     4851 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_inline/balance_pairs.py
+-rwxr-xr-x   0        0        0     3123 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_inline/emphasis.py
+-rwxr-xr-x   0        0        0     1651 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_inline/entity.py
+-rwxr-xr-x   0        0        0     1658 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_inline/escape.py
+-rwxr-xr-x   0        0        0     1493 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_inline/fragments_join.py
+-rwxr-xr-x   0        0        0     1130 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_inline/html_inline.py
+-rwxr-xr-x   0        0        0     4135 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_inline/image.py
+-rwxr-xr-x   0        0        0     4318 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_inline/link.py
+-rwxr-xr-x   0        0        0     1704 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_inline/linkify.py
+-rwxr-xr-x   0        0        0     1296 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_inline/newline.py
+-rwxr-xr-x   0        0        0     5101 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_inline/state_inline.py
+-rwxr-xr-x   0        0        0     3214 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_inline/strikethrough.py
+-rwxr-xr-x   0        0        0      901 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it/rules_inline/text.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it_py-3.0.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1078 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE.markdown-it
+-rwxr-xr-x   0        0        0     6940 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it_py-3.0.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0    10827 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it_py-3.0.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it_py-3.0.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0       58 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it_py-3.0.0.dist-info/entry_points.txt
+-rwxr-xr-x   0        0        0      547 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/mdurl/__init__.py
+-rwxr-xr-x   0        0        0     3004 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/mdurl/_decode.py
+-rwxr-xr-x   0        0        0     2602 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/mdurl/_encode.py
+-rwxr-xr-x   0        0        0      626 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/mdurl/_format.py
+-rwxr-xr-x   0        0        0    11374 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/mdurl/_parse.py
+-rwxr-xr-x   0        0        0      284 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/mdurl/_url.py
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/mdurl/py.typed
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/mdurl-0.1.2.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     2338 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/mdurl-0.1.2.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     1638 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/mdurl-0.1.2.dist-info/METADATA
+-rwxr-xr-x   0        0        0     1152 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/mdurl-0.1.2.dist-info/RECORD
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/mdurl-0.1.2.dist-info/WHEEL
+-rwxr-xr-x   0        0        0      148 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/more_itertools/__init__.py
+-rwxr-xr-x   0        0        0       43 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/more_itertools/__init__.pyi
+-rwxr-xr-x   0        0        0   134968 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/more_itertools/more.py
+-rwxr-xr-x   0        0        0    20105 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/more_itertools/more.pyi
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/more_itertools/py.typed
+-rwxr-xr-x   0        0        0    25416 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/more_itertools/recipes.py
+-rwxr-xr-x   0        0        0     4056 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/more_itertools/recipes.pyi
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/more_itertools-9.1.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1053 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/more_itertools-9.1.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0    32271 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/more_itertools-9.1.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0     1158 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/more_itertools-9.1.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/more_itertools-9.1.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0      370 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/__init__.py
+-rwxr-xr-x   0        0        0     1229 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/__main__.py
+-rwxr-xr-x   0        0        0      290 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/py.typed
+-rwxr-xr-x   0        0        0      592 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/__init__.py
+-rwxr-xr-x   0        0        0    10415 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/build_env.py
+-rwxr-xr-x   0        0        0    10245 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/cache.py
+-rwxr-xr-x   0        0        0    14128 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/configuration.py
+-rwxr-xr-x   0        0        0    13567 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/exceptions.py
+-rwxr-xr-x   0        0        0      364 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/main.py
+-rwxr-xr-x   0        0        0     7246 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/pyproject.py
+-rwxr-xr-x   0        0        0     6671 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/self_outdated_check.py
+-rwxr-xr-x   0        0        0    12100 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/wheel_builder.py
+-rwxr-xr-x   0        0        0      136 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/cli/__init__.py
+-rwxr-xr-x   0        0        0     6562 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/cli/autocompletion.py
+-rwxr-xr-x   0        0        0     7810 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/cli/base_command.py
+-rwxr-xr-x   0        0        0    29292 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/cli/cmdoptions.py
+-rwxr-xr-x   0        0        0      787 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/cli/command_context.py
+-rwxr-xr-x   0        0        0     2542 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/cli/main.py
+-rwxr-xr-x   0        0        0     2701 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/cli/main_parser.py
+-rwxr-xr-x   0        0        0    11080 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/cli/parser.py
+-rwxr-xr-x   0        0        0     8550 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/cli/progress_bars.py
+-rwxr-xr-x   0        0        0    17001 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/cli/req_command.py
+-rwxr-xr-x   0        0        0     5233 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/cli/spinners.py
+-rwxr-xr-x   0        0        0      122 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/cli/status_codes.py
+-rwxr-xr-x   0        0        0     3888 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/__init__.py
+-rwxr-xr-x   0        0        0     7453 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/cache.py
+-rwxr-xr-x   0        0        0     1617 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/check.py
+-rwxr-xr-x   0        0        0     3005 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/completion.py
+-rwxr-xr-x   0        0        0     9228 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/configuration.py
+-rwxr-xr-x   0        0        0     6851 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/debug.py
+-rwxr-xr-x   0        0        0     5088 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/download.py
+-rwxr-xr-x   0        0        0     2869 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/freeze.py
+-rwxr-xr-x   0        0        0     1719 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/hash.py
+-rwxr-xr-x   0        0        0     1173 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/help.py
+-rwxr-xr-x   0        0        0     4920 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/index.py
+-rwxr-xr-x   0        0        0    28243 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/install.py
+-rwxr-xr-x   0        0        0    12090 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/list.py
+-rwxr-xr-x   0        0        0     5707 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/search.py
+-rwxr-xr-x   0        0        0     8208 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/show.py
+-rwxr-xr-x   0        0        0     3580 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/uninstall.py
+-rwxr-xr-x   0        0        0     6365 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/wheel.py
+-rwxr-xr-x   0        0        0      879 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/distributions/__init__.py
+-rwxr-xr-x   0        0        0     1244 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/distributions/base.py
+-rwxr-xr-x   0        0        0      667 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/distributions/installed.py
+-rwxr-xr-x   0        0        0     3957 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/distributions/sdist.py
+-rwxr-xr-x   0        0        0     1217 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/distributions/wheel.py
+-rwxr-xr-x   0        0        0       32 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/index/__init__.py
+-rwxr-xr-x   0        0        0    18179 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/index/collector.py
+-rwxr-xr-x   0        0        0    37120 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/index/package_finder.py
+-rwxr-xr-x   0        0        0     6781 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/index/sources.py
+-rwxr-xr-x   0        0        0    11584 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/locations/__init__.py
+-rwxr-xr-x   0        0        0     6040 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/locations/_distutils.py
+-rwxr-xr-x   0        0        0     8137 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/locations/_sysconfig.py
+-rwxr-xr-x   0        0        0     1631 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/locations/base.py
+-rwxr-xr-x   0        0        0     1624 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/metadata/__init__.py
+-rwxr-xr-x   0        0        0     8170 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/metadata/base.py
+-rwxr-xr-x   0        0        0     5353 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/models/__init__.py
+-rwxr-xr-x   0        0        0      977 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/models/candidate.py
+-rwxr-xr-x   0        0        0     6482 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/models/direct_url.py
+-rwxr-xr-x   0        0        0     2641 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/models/format_control.py
+-rwxr-xr-x   0        0        0     1090 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/models/index.py
+-rwxr-xr-x   0        0        0    10227 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/models/link.py
+-rwxr-xr-x   0        0        0      769 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/models/scheme.py
+-rwxr-xr-x   0        0        0     4600 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/models/search_scope.py
+-rwxr-xr-x   0        0        0     1923 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/models/selection_prefs.py
+-rwxr-xr-x   0        0        0     3981 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/models/target_python.py
+-rwxr-xr-x   0        0        0     3633 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/models/wheel.py
+-rwxr-xr-x   0        0        0       52 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/network/__init__.py
+-rwxr-xr-x   0        0        0    11961 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/network/auth.py
+-rwxr-xr-x   0        0        0     2169 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/network/cache.py
+-rwxr-xr-x   0        0        0     6200 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/network/download.py
+-rwxr-xr-x   0        0        0     7825 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/network/lazy_wheel.py
+-rwxr-xr-x   0        0        0    17036 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/network/session.py
+-rwxr-xr-x   0        0        0     4155 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/network/utils.py
+-rwxr-xr-x   0        0        0     1851 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/network/xmlrpc.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/operations/__init__.py
+-rwxr-xr-x   0        0        0     5448 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/operations/check.py
+-rwxr-xr-x   0        0        0    10833 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/operations/freeze.py
+-rwxr-xr-x   0        0        0    25503 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/operations/prepare.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/operations/build/__init__.py
+-rwxr-xr-x   0        0        0     1200 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/operations/build/metadata.py
+-rwxr-xr-x   0        0        0     1991 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rwxr-xr-x   0        0        0     1144 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/operations/build/wheel.py
+-rwxr-xr-x   0        0        0     3337 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/operations/install/__init__.py
+-rwxr-xr-x   0        0        0     1443 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rwxr-xr-x   0        0        0     4537 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/operations/install/legacy.py
+-rwxr-xr-x   0        0        0    30269 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/operations/install/wheel.py
+-rwxr-xr-x   0        0        0     2925 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/req/__init__.py
+-rwxr-xr-x   0        0        0    16300 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/req/constructors.py
+-rwxr-xr-x   0        0        0    17936 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/req/req_file.py
+-rwxr-xr-x   0        0        0    32517 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/req/req_install.py
+-rwxr-xr-x   0        0        0     7762 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/req/req_set.py
+-rwxr-xr-x   0        0        0     4312 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/req/req_tracker.py
+-rwxr-xr-x   0        0        0    24450 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/req/req_uninstall.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/resolution/__init__.py
+-rwxr-xr-x   0        0        0      575 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/resolution/base.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rwxr-xr-x   0        0        0    18005 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rwxr-xr-x   0        0        0     5434 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rwxr-xr-x   0        0        0    19397 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rwxr-xr-x   0        0        0    27559 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rwxr-xr-x   0        0        0     5427 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rwxr-xr-x   0        0        0     8617 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rwxr-xr-x   0        0        0     2669 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rwxr-xr-x   0        0        0     5621 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rwxr-xr-x   0        0        0    10795 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/__init__.py
+-rwxr-xr-x   0        0        0     1053 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/_log.py
+-rwxr-xr-x   0        0        0     1220 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/appdirs.py
+-rwxr-xr-x   0        0        0     1947 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/compat.py
+-rwxr-xr-x   0        0        0     5622 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/datetime.py
+-rwxr-xr-x   0        0        0     3304 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/deprecation.py
+-rwxr-xr-x   0        0        0     3073 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rwxr-xr-x   0        0        0     1291 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/distutils_args.py
+-rwxr-xr-x   0        0        0     1205 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/encoding.py
+-rwxr-xr-x   0        0        0     1082 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/entrypoints.py
+-rwxr-xr-x   0        0        0     6075 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/filesystem.py
+-rwxr-xr-x   0        0        0      789 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/filetypes.py
+-rwxr-xr-x   0        0        0     3262 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/glibc.py
+-rwxr-xr-x   0        0        0     5332 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/hashes.py
+-rwxr-xr-x   0        0        0      846 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/inject_securetransport.py
+-rwxr-xr-x   0        0        0    12735 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/logging.py
+-rwxr-xr-x   0        0        0    24472 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/misc.py
+-rwxr-xr-x   0        0        0     1376 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/models.py
+-rwxr-xr-x   0        0        0     2989 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/packaging.py
+-rwxr-xr-x   0        0        0     3325 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/parallel.py
+-rwxr-xr-x   0        0        0     1146 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/pkg_resources.py
+-rwxr-xr-x   0        0        0     5220 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/setuptools_build.py
+-rwxr-xr-x   0        0        0    10324 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/subprocess.py
+-rwxr-xr-x   0        0        0     8210 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/temp_dir.py
+-rwxr-xr-x   0        0        0     9317 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/unpacking.py
+-rwxr-xr-x   0        0        0     1863 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/urls.py
+-rwxr-xr-x   0        0        0     3675 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/virtualenv.py
+-rwxr-xr-x   0        0        0     6479 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/wheel.py
+-rwxr-xr-x   0        0        0      611 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/vcs/__init__.py
+-rwxr-xr-x   0        0        0     3058 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/vcs/bazaar.py
+-rwxr-xr-x   0        0        0    17853 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/vcs/git.py
+-rwxr-xr-x   0        0        0     5234 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/vcs/mercurial.py
+-rwxr-xr-x   0        0        0    12195 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/vcs/subversion.py
+-rwxr-xr-x   0        0        0    23998 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py
+-rwxr-xr-x   0        0        0     4814 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/__init__.py
+-rwxr-xr-x   0        0        0    26540 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/appdirs.py
+-rwxr-xr-x   0        0        0    44858 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distro.py
+-rwxr-xr-x   0        0        0   280501 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pyparsing.py
+-rwxr-xr-x   0        0        0    35547 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/six.py
+-rwxr-xr-x   0        0        0      386 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/vendor.txt
+-rwxr-xr-x   0        0        0      313 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rwxr-xr-x   0        0        0     1352 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rwxr-xr-x   0        0        0     5015 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rwxr-xr-x   0        0        0      844 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py
+-rwxr-xr-x   0        0        0      724 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/compat.py
+-rwxr-xr-x   0        0        0    14525 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py
+-rwxr-xr-x   0        0        0     2613 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rwxr-xr-x   0        0        0     4205 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rwxr-xr-x   0        0        0     7279 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rwxr-xr-x   0        0        0      719 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rwxr-xr-x   0        0        0     4299 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rwxr-xr-x   0        0        0      889 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/certifi/__init__.py
+-rwxr-xr-x   0        0        0      267 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/certifi/__main__.py
+-rwxr-xr-x   0        0        0   259465 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem
+-rwxr-xr-x   0        0        0     2916 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/certifi/core.py
+-rwxr-xr-x   0        0        0     3354 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/__init__.py
+-rwxr-xr-x   0        0        0    31640 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/big5freq.py
+-rwxr-xr-x   0        0        0     1804 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/big5prober.py
+-rwxr-xr-x   0        0        0     9644 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py
+-rwxr-xr-x   0        0        0     3946 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rwxr-xr-x   0        0        0     5255 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py
+-rwxr-xr-x   0        0        0     3678 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rwxr-xr-x   0        0        0     1236 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/compat.py
+-rwxr-xr-x   0        0        0     1904 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py
+-rwxr-xr-x   0        0        0     1737 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/enums.py
+-rwxr-xr-x   0        0        0     4051 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/escprober.py
+-rwxr-xr-x   0        0        0    10756 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/escsm.py
+-rwxr-xr-x   0        0        0     3841 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rwxr-xr-x   0        0        0    13741 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rwxr-xr-x   0        0        0     1795 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py
+-rwxr-xr-x   0        0        0    32008 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rwxr-xr-x   0        0        0     1793 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py
+-rwxr-xr-x   0        0        0    20998 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rwxr-xr-x   0        0        0     1800 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rwxr-xr-x   0        0        0    14130 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rwxr-xr-x   0        0        0    26102 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py
+-rwxr-xr-x   0        0        0    19876 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py
+-rwxr-xr-x   0        0        0   110347 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rwxr-xr-x   0        0        0   103969 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rwxr-xr-x   0        0        0   103159 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rwxr-xr-x   0        0        0   107148 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rwxr-xr-x   0        0        0   136898 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rwxr-xr-x   0        0        0   107695 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rwxr-xr-x   0        0        0   100329 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rwxr-xr-x   0        0        0     5515 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py
+-rwxr-xr-x   0        0        0     3504 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rwxr-xr-x   0        0        0     2066 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rwxr-xr-x   0        0        0    26053 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py
+-rwxr-xr-x   0        0        0     6281 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rwxr-xr-x   0        0        0     4392 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rwxr-xr-x   0        0        0     3866 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py
+-rwxr-xr-x   0        0        0    12789 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py
+-rwxr-xr-x   0        0        0     2848 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py
+-rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/version.py
+-rwxr-xr-x   0        0        0        2 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rwxr-xr-x   0        0        0     2831 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rwxr-xr-x   0        0        0    19784 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rwxr-xr-x   0        0        0      245 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/colorama/__init__.py
+-rwxr-xr-x   0        0        0     2624 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/colorama/ansi.py
+-rwxr-xr-x   0        0        0    10775 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rwxr-xr-x   0        0        0     1995 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/colorama/initialise.py
+-rwxr-xr-x   0        0        0     5556 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/colorama/win32.py
+-rwxr-xr-x   0        0        0     6607 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/colorama/winterm.py
+-rwxr-xr-x   0        0        0      604 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/__init__.py
+-rwxr-xr-x   0        0        0    42528 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/compat.py
+-rwxr-xr-x   0        0        0    52398 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/database.py
+-rwxr-xr-x   0        0        0    21248 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/index.py
+-rwxr-xr-x   0        0        0    53265 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/locators.py
+-rwxr-xr-x   0        0        0    15204 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/manifest.py
+-rwxr-xr-x   0        0        0     4474 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/markers.py
+-rwxr-xr-x   0        0        0    40167 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/metadata.py
+-rwxr-xr-x   0        0        0    11178 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/resources.py
+-rwxr-xr-x   0        0        0    17671 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/scripts.py
+-rwxr-xr-x   0        0        0    96768 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/t32.exe
+-rwxr-xr-x   0        0        0   105984 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/t64.exe
+-rwxr-xr-x   0        0        0    69523 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/util.py
+-rwxr-xr-x   0        0        0    24247 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/version.py
+-rwxr-xr-x   0        0        0    90112 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/w32.exe
+-rwxr-xr-x   0        0        0    99840 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/w64.exe
+-rwxr-xr-x   0        0        0    44118 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/wheel.py
+-rwxr-xr-x   0        0        0      280 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/_backport/__init__.py
+-rwxr-xr-x   0        0        0     1012 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/_backport/misc.py
+-rwxr-xr-x   0        0        0    26471 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/_backport/shutil.py
+-rwxr-xr-x   0        0        0     2701 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/_backport/sysconfig.cfg
+-rwxr-xr-x   0        0        0    27640 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/_backport/sysconfig.py
+-rwxr-xr-x   0        0        0    95235 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/_backport/tarfile.py
+-rwxr-xr-x   0        0        0     1195 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/__init__.py
+-rwxr-xr-x   0        0        0    17017 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_ihatexml.py
+-rwxr-xr-x   0        0        0    33271 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_inputstream.py
+-rwxr-xr-x   0        0        0    78775 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_tokenizer.py
+-rwxr-xr-x   0        0        0     5090 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_utils.py
+-rwxr-xr-x   0        0        0    86410 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/constants.py
+-rwxr-xr-x   0        0        0   119981 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/html5parser.py
+-rwxr-xr-x   0        0        0    16168 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/serializer.py
+-rwxr-xr-x   0        0        0      114 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_trie/__init__.py
+-rwxr-xr-x   0        0        0     1053 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_trie/_base.py
+-rwxr-xr-x   0        0        0     1842 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_trie/py.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/__init__.py
+-rwxr-xr-x   0        0        0      948 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py
+-rwxr-xr-x   0        0        0      298 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/base.py
+-rwxr-xr-x   0        0        0     3018 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/inject_meta_charset.py
+-rwxr-xr-x   0        0        0     3736 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/lint.py
+-rwxr-xr-x   0        0        0    10795 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/optionaltags.py
+-rwxr-xr-x   0        0        0    27813 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/sanitizer.py
+-rwxr-xr-x   0        0        0     1252 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/whitespace.py
+-rwxr-xr-x   0        0        0      709 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treeadapters/__init__.py
+-rwxr-xr-x   0        0        0     1769 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treeadapters/genshi.py
+-rwxr-xr-x   0        0        0     1826 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treeadapters/sax.py
+-rwxr-xr-x   0        0        0     3680 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/__init__.py
+-rwxr-xr-x   0        0        0    14982 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/base.py
+-rwxr-xr-x   0        0        0     9164 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/dom.py
+-rwxr-xr-x   0        0        0    13179 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/etree.py
+-rwxr-xr-x   0        0        0    15158 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py
+-rwxr-xr-x   0        0        0     5873 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/__init__.py
+-rwxr-xr-x   0        0        0     7728 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/base.py
+-rwxr-xr-x   0        0        0     1456 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/dom.py
+-rwxr-xr-x   0        0        0     4682 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/etree.py
+-rwxr-xr-x   0        0        0     6572 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py
+-rwxr-xr-x   0        0        0     2378 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/genshi.py
+-rwxr-xr-x   0        0        0      893 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/idna/__init__.py
+-rwxr-xr-x   0        0        0     3570 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/idna/codec.py
+-rwxr-xr-x   0        0        0      376 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/idna/compat.py
+-rwxr-xr-x   0        0        0    13235 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/idna/core.py
+-rwxr-xr-x   0        0        0    44400 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/idna/idnadata.py
+-rwxr-xr-x   0        0        0     1991 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/idna/intranges.py
+-rwxr-xr-x   0        0        0       23 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/idna/package_data.py
+-rwxr-xr-x   0        0        0   210287 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/idna/uts46data.py
+-rwxr-xr-x   0        0        0     1172 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/msgpack/__init__.py
+-rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/msgpack/_version.py
+-rwxr-xr-x   0        0        0     1129 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py
+-rwxr-xr-x   0        0        0     6281 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/msgpack/ext.py
+-rwxr-xr-x   0        0        0    39113 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/msgpack/fallback.py
+-rwxr-xr-x   0        0        0      687 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/packaging/__about__.py
+-rwxr-xr-x   0        0        0      522 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/packaging/__init__.py
+-rwxr-xr-x   0        0        0    11789 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py
+-rwxr-xr-x   0        0        0     4514 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py
+-rwxr-xr-x   0        0        0     1696 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/packaging/_structures.py
+-rwxr-xr-x   0        0        0     8791 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/packaging/markers.py
+-rwxr-xr-x   0        0        0     4822 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/packaging/requirements.py
+-rwxr-xr-x   0        0        0    31792 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/packaging/specifiers.py
+-rwxr-xr-x   0        0        0    16198 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/packaging/tags.py
+-rwxr-xr-x   0        0        0     4336 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/packaging/utils.py
+-rwxr-xr-x   0        0        0    15169 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/packaging/version.py
+-rwxr-xr-x   0        0        0      136 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pep517/__init__.py
+-rwxr-xr-x   0        0        0     3596 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pep517/build.py
+-rwxr-xr-x   0        0        0     6303 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pep517/check.py
+-rwxr-xr-x   0        0        0     4213 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pep517/colorlog.py
+-rwxr-xr-x   0        0        0     1113 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pep517/compat.py
+-rwxr-xr-x   0        0        0     1173 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pep517/dirtools.py
+-rwxr-xr-x   0        0        0     6283 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pep517/envbuild.py
+-rwxr-xr-x   0        0        0     2555 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pep517/meta.py
+-rwxr-xr-x   0        0        0    13629 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pep517/wrappers.py
+-rwxr-xr-x   0        0        0      580 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/__init__.py
+-rwxr-xr-x   0        0        0    11182 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/_in_process.py
+-rwxr-xr-x   0        0        0   111573 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rwxr-xr-x   0        0        0      585 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pkg_resources/py31compat.py
+-rwxr-xr-x   0        0        0     5034 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/progress/__init__.py
+-rwxr-xr-x   0        0        0     2945 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/progress/bar.py
+-rwxr-xr-x   0        0        0     1413 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/progress/counter.py
+-rwxr-xr-x   0        0        0     1423 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/progress/spinner.py
+-rwxr-xr-x   0        0        0     5267 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/__init__.py
+-rwxr-xr-x   0        0        0      455 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/__version__.py
+-rwxr-xr-x   0        0        0     1138 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py
+-rwxr-xr-x   0        0        0    22081 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/adapters.py
+-rwxr-xr-x   0        0        0     6561 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/api.py
+-rwxr-xr-x   0        0        0    10512 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/auth.py
+-rwxr-xr-x   0        0        0      483 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/certs.py
+-rwxr-xr-x   0        0        0     2121 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/compat.py
+-rwxr-xr-x   0        0        0    18979 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/cookies.py
+-rwxr-xr-x   0        0        0     3377 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/exceptions.py
+-rwxr-xr-x   0        0        0     4104 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/help.py
+-rwxr-xr-x   0        0        0      791 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/hooks.py
+-rwxr-xr-x   0        0        0    35890 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/models.py
+-rwxr-xr-x   0        0        0      711 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/packages.py
+-rwxr-xr-x   0        0        0    30949 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/sessions.py
+-rwxr-xr-x   0        0        0     4311 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/status_codes.py
+-rwxr-xr-x   0        0        0     3110 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/structures.py
+-rwxr-xr-x   0        0        0    32407 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/utils.py
+-rwxr-xr-x   0        0        0      563 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py
+-rwxr-xr-x   0        0        0     5762 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/resolvelib/providers.py
+-rwxr-xr-x   0        0        0     1401 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py
+-rwxr-xr-x   0        0        0    17698 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rwxr-xr-x   0        0        0     4959 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/resolvelib/structs.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rwxr-xr-x   0        0        0      162 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rwxr-xr-x   0        0        0    18774 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/__init__.py
+-rwxr-xr-x   0        0        0     3406 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rwxr-xr-x   0        0        0     2012 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/_utils.py
+-rwxr-xr-x   0        0        0     1542 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/after.py
+-rwxr-xr-x   0        0        0     1417 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/before.py
+-rwxr-xr-x   0        0        0     1966 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rwxr-xr-x   0        0        0     1426 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/nap.py
+-rwxr-xr-x   0        0        0     6858 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/retry.py
+-rwxr-xr-x   0        0        0     2886 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/stop.py
+-rwxr-xr-x   0        0        0     2204 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rwxr-xr-x   0        0        0     6882 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/wait.py
+-rwxr-xr-x   0        0        0      236 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tomli/__init__.py
+-rwxr-xr-x   0        0        0    23118 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tomli/_parser.py
+-rwxr-xr-x   0        0        0     2764 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tomli/_re.py
+-rwxr-xr-x   0        0        0     2848 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/__init__.py
+-rwxr-xr-x   0        0        0    11148 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/_collections.py
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/_version.py
+-rwxr-xr-x   0        0        0    19293 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/connection.py
+-rwxr-xr-x   0        0        0    38198 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py
+-rwxr-xr-x   0        0        0     8540 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py
+-rwxr-xr-x   0        0        0     8853 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/fields.py
+-rwxr-xr-x   0        0        0     2538 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/filepost.py
+-rwxr-xr-x   0        0        0    20299 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rwxr-xr-x   0        0        0     6155 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/request.py
+-rwxr-xr-x   0        0        0    29024 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/response.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rwxr-xr-x   0        0        0      993 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+-rwxr-xr-x   0        0        0    11348 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rwxr-xr-x   0        0        0     4668 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rwxr-xr-x   0        0        0    17402 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rwxr-xr-x   0        0        0    35356 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rwxr-xr-x   0        0        0     7313 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rwxr-xr-x   0        0        0    18168 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rwxr-xr-x   0        0        0    14304 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rwxr-xr-x   0        0        0      113 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/__init__.py
+-rwxr-xr-x   0        0        0    35743 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rwxr-xr-x   0        0        0     1468 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rwxr-xr-x   0        0        0      951 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py
+-rwxr-xr-x   0        0        0     5839 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py
+-rwxr-xr-x   0        0        0     1204 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rwxr-xr-x   0        0        0     5070 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py
+-rwxr-xr-x   0        0        0     1660 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rwxr-xr-x   0        0        0      520 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/queue.py
+-rwxr-xr-x   0        0        0     4266 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/request.py
+-rwxr-xr-x   0        0        0     3617 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/response.py
+-rwxr-xr-x   0        0        0    21993 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py
+-rwxr-xr-x   0        0        0    17672 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rwxr-xr-x   0        0        0     7152 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rwxr-xr-x   0        0        0    10271 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rwxr-xr-x   0        0        0    14479 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/url.py
+-rwxr-xr-x   0        0        0     5557 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py
+-rwxr-xr-x   0        0        0    10921 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/webencodings/__init__.py
+-rwxr-xr-x   0        0        0     9210 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/webencodings/labels.py
+-rwxr-xr-x   0        0        0     1364 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py
+-rwxr-xr-x   0        0        0     6716 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/webencodings/tests.py
+-rwxr-xr-x   0        0        0     4632 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip-21.2.3.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1110 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip-21.2.3.dist-info/LICENSE.txt
+-rwxr-xr-x   0        0        0     4165 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip-21.2.3.dist-info/METADATA
+-rwxr-xr-x   0        0        0    62024 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip-21.2.3.dist-info/RECORD
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip-21.2.3.dist-info/REQUESTED
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip-21.2.3.dist-info/WHEEL
+-rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip-21.2.3.dist-info/entry_points.txt
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip-21.2.3.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0   108202 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/__init__.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/__init__.py
+-rwxr-xr-x   0        0        0    24701 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/appdirs.py
+-rwxr-xr-x   0        0        0   232056 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/pyparsing.py
+-rwxr-xr-x   0        0        0      736 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/__about__.py
+-rwxr-xr-x   0        0        0      562 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rwxr-xr-x   0        0        0     1128 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_compat.py
+-rwxr-xr-x   0        0        0     2022 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rwxr-xr-x   0        0        0     1812 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_typing.py
+-rwxr-xr-x   0        0        0     9518 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rwxr-xr-x   0        0        0     4929 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rwxr-xr-x   0        0        0    31944 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rwxr-xr-x   0        0        0    24067 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rwxr-xr-x   0        0        0     1811 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rwxr-xr-x   0        0        0    15470 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/version.py
+-rwxr-xr-x   0        0        0     2362 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/extern/__init__.py
+-rwxr-xr-x   0        0        0      104 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/tests/data/my-test-package-source/setup.py
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/__init__.py
+-rwxr-xr-x   0        0        0      357 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/__init__.pyi
+-rwxr-xr-x   0        0        0     1198 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/bdist.py
+-rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/bdist.pyi
+-rwxr-xr-x   0        0        0     7415 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/commandline.py
+-rwxr-xr-x   0        0        0     1088 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/commandline.pyi
+-rwxr-xr-x   0        0        0     1577 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/develop.py
+-rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/develop.pyi
+-rwxr-xr-x   0        0        0     4627 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/distribution.py
+-rwxr-xr-x   0        0        0     1691 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/distribution.pyi
+-rwxr-xr-x   0        0        0      518 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/index.py
+-rwxr-xr-x   0        0        0      223 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/index.pyi
+-rwxr-xr-x   0        0        0     2492 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/installed.py
+-rwxr-xr-x   0        0        0      323 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/installed.pyi
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/py.typed
+-rwxr-xr-x   0        0        0     2347 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/sdist.py
+-rwxr-xr-x   0        0        0      396 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/sdist.pyi
+-rwxr-xr-x   0        0        0     1786 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/utils.py
+-rwxr-xr-x   0        0        0      175 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/utils.pyi
+-rwxr-xr-x   0        0        0     1586 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/wheel.py
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/wheel.pyi
+-rwxr-xr-x   0        0        0     1342 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/tests/__init__.py
+-rwxr-xr-x   0        0        0     2279 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/tests/test_bdist.py
+-rwxr-xr-x   0        0        0    11722 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/tests/test_commandline.py
+-rwxr-xr-x   0        0        0      831 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/tests/test_develop.py
+-rwxr-xr-x   0        0        0    19377 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/tests/test_distribution.py
+-rwxr-xr-x   0        0        0     2636 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/tests/test_index.py
+-rwxr-xr-x   0        0        0     5460 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/tests/test_installed.py
+-rwxr-xr-x   0        0        0     5481 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/tests/test_sdist.py
+-rwxr-xr-x   0        0        0     6835 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/tests/test_utils.py
+-rwxr-xr-x   0        0        0     4443 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo/tests/test_wheel.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo-1.9.6.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1084 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo-1.9.6.dist-info/LICENSE.txt
+-rwxr-xr-x   0        0        0    10807 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo-1.9.6.dist-info/METADATA
+-rwxr-xr-x   0        0        0     4168 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo-1.9.6.dist-info/RECORD
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo-1.9.6.dist-info/WHEEL
+-rwxr-xr-x   0        0        0       54 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo-1.9.6.dist-info/entry_points.txt
+-rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkginfo-1.9.6.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0     2815 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pycparser/__init__.py
+-rwxr-xr-x   0        0        0    10555 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pycparser/_ast_gen.py
+-rwxr-xr-x   0        0        0     1039 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pycparser/_build_tables.py
+-rwxr-xr-x   0        0        0     4255 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pycparser/_c_ast.cfg
+-rwxr-xr-x   0        0        0     5691 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pycparser/ast_transforms.py
+-rwxr-xr-x   0        0        0    31445 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pycparser/c_ast.py
+-rwxr-xr-x   0        0        0    17772 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pycparser/c_generator.py
+-rwxr-xr-x   0        0        0    17167 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pycparser/c_lexer.py
+-rwxr-xr-x   0        0        0    73680 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pycparser/c_parser.py
+-rwxr-xr-x   0        0        0     8504 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pycparser/lextab.py
+-rwxr-xr-x   0        0        0     4875 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pycparser/plyparser.py
+-rwxr-xr-x   0        0        0   205652 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pycparser/yacctab.py
+-rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pycparser/ply/__init__.py
+-rwxr-xr-x   0        0        0    33282 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pycparser/ply/cpp.py
+-rwxr-xr-x   0        0        0     3177 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pycparser/ply/ctokens.py
+-rwxr-xr-x   0        0        0    42918 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pycparser/ply/lex.py
+-rwxr-xr-x   0        0        0   137323 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pycparser/ply/yacc.py
+-rwxr-xr-x   0        0        0     2251 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pycparser/ply/ygen.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pycparser-2.21.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1536 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pycparser-2.21.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     1108 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pycparser-2.21.dist-info/METADATA
+-rwxr-xr-x   0        0        0     2793 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pycparser-2.21.dist-info/RECORD
+-rwxr-xr-x   0        0        0      110 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pycparser-2.21.dist-info/WHEEL
+-rwxr-xr-x   0        0        0       10 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pycparser-2.21.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0     2959 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/__init__.py
+-rwxr-xr-x   0        0        0      348 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/__main__.py
+-rwxr-xr-x   0        0        0    23530 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/cmdline.py
+-rwxr-xr-x   0        0        0     1697 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/console.py
+-rwxr-xr-x   0        0        0     1938 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/filter.py
+-rwxr-xr-x   0        0        0     4154 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/formatter.py
+-rwxr-xr-x   0        0        0    34541 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexer.py
+-rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/modeline.py
+-rwxr-xr-x   0        0        0     2579 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/plugin.py
+-rwxr-xr-x   0        0        0     3072 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/regexopt.py
+-rwxr-xr-x   0        0        0     3092 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/scanner.py
+-rwxr-xr-x   0        0        0     6816 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/sphinxext.py
+-rwxr-xr-x   0        0        0     6245 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/style.py
+-rwxr-xr-x   0        0        0     6184 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/token.py
+-rwxr-xr-x   0        0        0    63223 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/unistring.py
+-rwxr-xr-x   0        0        0    10230 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/util.py
+-rwxr-xr-x   0        0        0    40338 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/filters/__init__.py
+-rwxr-xr-x   0        0        0     5388 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/formatters/__init__.py
+-rwxr-xr-x   0        0        0     4176 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/formatters/_mapping.py
+-rwxr-xr-x   0        0        0     3290 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/formatters/bbcode.py
+-rwxr-xr-x   0        0        0     5070 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/formatters/groff.py
+-rwxr-xr-x   0        0        0    35574 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/formatters/html.py
+-rwxr-xr-x   0        0        0    21914 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/formatters/img.py
+-rwxr-xr-x   0        0        0     4945 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/formatters/irc.py
+-rwxr-xr-x   0        0        0    19303 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/formatters/latex.py
+-rwxr-xr-x   0        0        0     5025 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/formatters/other.py
+-rwxr-xr-x   0        0        0     2200 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/formatters/pangomarkup.py
+-rwxr-xr-x   0        0        0     4990 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/formatters/rtf.py
+-rwxr-xr-x   0        0        0     7299 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/formatters/svg.py
+-rwxr-xr-x   0        0        0     4626 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/formatters/terminal.py
+-rwxr-xr-x   0        0        0    11717 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/formatters/terminal256.py
+-rwxr-xr-x   0        0        0    12082 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/__init__.py
+-rwxr-xr-x   0        0        0     1543 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_ada_builtins.py
+-rwxr-xr-x   0        0        0    27287 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_asy_builtins.py
+-rwxr-xr-x   0        0        0    13994 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_cl_builtins.py
+-rwxr-xr-x   0        0        0   105182 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_cocoa_builtins.py
+-rwxr-xr-x   0        0        0    18414 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_csound_builtins.py
+-rwxr-xr-x   0        0        0    12446 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_css_builtins.py
+-rwxr-xr-x   0        0        0    11883 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_julia_builtins.py
+-rwxr-xr-x   0        0        0   134510 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_lasso_builtins.py
+-rwxr-xr-x   0        0        0   108094 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_lilypond_builtins.py
+-rwxr-xr-x   0        0        0     8116 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_lua_builtins.py
+-rwxr-xr-x   0        0        0    65633 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_mapping.py
+-rwxr-xr-x   0        0        0    24713 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_mql_builtins.py
+-rwxr-xr-x   0        0        0    25842 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_mysql_builtins.py
+-rwxr-xr-x   0        0        0    49398 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_openedge_builtins.py
+-rwxr-xr-x   0        0        0   107930 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_php_builtins.py
+-rwxr-xr-x   0        0        0    13355 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_postgres_builtins.py
+-rwxr-xr-x   0        0        0    12595 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_qlik_builtins.py
+-rwxr-xr-x   0        0        0    32564 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_scheme_builtins.py
+-rwxr-xr-x   0        0        0    52413 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_scilab_builtins.py
+-rwxr-xr-x   0        0        0    26781 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_sourcemod_builtins.py
+-rwxr-xr-x   0        0        0    13445 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_stan_builtins.py
+-rwxr-xr-x   0        0        0    27227 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_stata_builtins.py
+-rwxr-xr-x   0        0        0    15460 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_tsql_builtins.py
+-rwxr-xr-x   0        0        0     1658 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_usd_builtins.py
+-rwxr-xr-x   0        0        0     4225 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_vbscript_builtins.py
+-rwxr-xr-x   0        0        0    57066 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/_vim_builtins.py
+-rwxr-xr-x   0        0        0    11676 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/actionscript.py
+-rwxr-xr-x   0        0        0     5320 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/ada.py
+-rwxr-xr-x   0        0        0      876 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/agile.py
+-rwxr-xr-x   0        0        0     9873 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/algebra.py
+-rwxr-xr-x   0        0        0     2606 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/ambient.py
+-rwxr-xr-x   0        0        0     1670 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/amdgpu.py
+-rwxr-xr-x   0        0        0     4177 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/ampl.py
+-rwxr-xr-x   0        0        0    30766 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/apdlexer.py
+-rwxr-xr-x   0        0        0     3405 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/apl.py
+-rwxr-xr-x   0        0        0    11469 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/archetype.py
+-rwxr-xr-x   0        0        0     3565 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/arrow.py
+-rwxr-xr-x   0        0        0    11417 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/arturo.py
+-rwxr-xr-x   0        0        0     1621 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/asc.py
+-rwxr-xr-x   0        0        0    41243 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/asm.py
+-rwxr-xr-x   0        0        0    19815 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/automation.py
+-rwxr-xr-x   0        0        0     3021 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/bare.py
+-rwxr-xr-x   0        0        0    27923 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/basic.py
+-rwxr-xr-x   0        0        0     1652 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/bdd.py
+-rwxr-xr-x   0        0        0     3211 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/berry.py
+-rwxr-xr-x   0        0        0     4723 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/bibtex.py
+-rwxr-xr-x   0        0        0     3915 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/boa.py
+-rwxr-xr-x   0        0        0    28112 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/business.py
+-rwxr-xr-x   0        0        0    17791 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/c_cpp.py
+-rwxr-xr-x   0        0        0    29206 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/c_like.py
+-rwxr-xr-x   0        0        0     2175 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/capnproto.py
+-rwxr-xr-x   0        0        0     3231 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/carbon.py
+-rwxr-xr-x   0        0        0     5182 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/cddl.py
+-rwxr-xr-x   0        0        0     5157 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/chapel.py
+-rwxr-xr-x   0        0        0     6395 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/clean.py
+-rwxr-xr-x   0        0        0     3156 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/comal.py
+-rwxr-xr-x   0        0        0     1407 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/compiled.py
+-rwxr-xr-x   0        0        0    42338 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/configs.py
+-rwxr-xr-x   0        0        0     4148 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/console.py
+-rwxr-xr-x   0        0        0     1390 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/cplint.py
+-rwxr-xr-x   0        0        0    15756 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/crystal.py
+-rwxr-xr-x   0        0        0    16994 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/csound.py
+-rwxr-xr-x   0        0        0    25322 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/css.py
+-rwxr-xr-x   0        0        0     9875 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/d.py
+-rwxr-xr-x   0        0        0     4607 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/dalvik.py
+-rwxr-xr-x   0        0        0    26940 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/data.py
+-rwxr-xr-x   0        0        0     8099 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/dax.py
+-rwxr-xr-x   0        0        0     4020 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/devicetree.py
+-rwxr-xr-x   0        0        0     5278 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/diff.py
+-rwxr-xr-x   0        0        0    37623 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/dotnet.py
+-rwxr-xr-x   0        0        0    36774 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/dsls.py
+-rwxr-xr-x   0        0        0    10380 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/dylan.py
+-rwxr-xr-x   0        0        0     6372 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/ecl.py
+-rwxr-xr-x   0        0        0     2690 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/eiffel.py
+-rwxr-xr-x   0        0        0     3152 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/elm.py
+-rwxr-xr-x   0        0        0     6370 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/elpi.py
+-rwxr-xr-x   0        0        0     4742 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/email.py
+-rwxr-xr-x   0        0        0    19170 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/erlang.py
+-rwxr-xr-x   0        0        0    10396 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/esoteric.py
+-rwxr-xr-x   0        0        0     3273 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/ezhil.py
+-rwxr-xr-x   0        0        0    19531 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/factor.py
+-rwxr-xr-x   0        0        0    10197 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/fantom.py
+-rwxr-xr-x   0        0        0     9646 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/felix.py
+-rwxr-xr-x   0        0        0     1621 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/fift.py
+-rwxr-xr-x   0        0        0     2668 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/floscript.py
+-rwxr-xr-x   0        0        0     7194 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/forth.py
+-rwxr-xr-x   0        0        0    10336 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/fortran.py
+-rwxr-xr-x   0        0        0    26212 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/foxpro.py
+-rwxr-xr-x   0        0        0    26914 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/freefem.py
+-rwxr-xr-x   0        0        0     3622 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/func.py
+-rwxr-xr-x   0        0        0      674 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/functional.py
+-rwxr-xr-x   0        0        0     3732 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/futhark.py
+-rwxr-xr-x   0        0        0      826 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/gcodelexer.py
+-rwxr-xr-x   0        0        0     7543 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/gdscript.py
+-rwxr-xr-x   0        0        0     3761 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/go.py
+-rwxr-xr-x   0        0        0     7980 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/grammar_notation.py
+-rwxr-xr-x   0        0        0     3861 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/graph.py
+-rwxr-xr-x   0        0        0    39026 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/graphics.py
+-rwxr-xr-x   0        0        0     1935 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/graphviz.py
+-rwxr-xr-x   0        0        0     3991 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/gsql.py
+-rwxr-xr-x   0        0        0    32898 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/haskell.py
+-rwxr-xr-x   0        0        0    30976 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/haxe.py
+-rwxr-xr-x   0        0        0    22520 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/hdl.py
+-rwxr-xr-x   0        0        0     3603 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/hexdump.py
+-rwxr-xr-x   0        0        0    19879 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/html.py
+-rwxr-xr-x   0        0        0    15450 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/idl.py
+-rwxr-xr-x   0        0        0    30631 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/igor.py
+-rwxr-xr-x   0        0        0     3136 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/inferno.py
+-rwxr-xr-x   0        0        0    13178 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/installers.py
+-rwxr-xr-x   0        0        0    57119 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/int_fiction.py
+-rwxr-xr-x   0        0        0     1906 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/iolang.py
+-rwxr-xr-x   0        0        0     4854 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/j.py
+-rwxr-xr-x   0        0        0    62859 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/javascript.py
+-rwxr-xr-x   0        0        0     2059 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/jmespath.py
+-rwxr-xr-x   0        0        0     3701 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/jslt.py
+-rwxr-xr-x   0        0        0     5635 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/jsonnet.py
+-rwxr-xr-x   0        0        0    11646 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/julia.py
+-rwxr-xr-x   0        0        0    72929 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/jvm.py
+-rwxr-xr-x   0        0        0    11406 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/kuin.py
+-rwxr-xr-x   0        0        0     9753 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/lilypond.py
+-rwxr-xr-x   0        0        0   144039 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/lisp.py
+-rwxr-xr-x   0        0        0    31914 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/macaulay2.py
+-rwxr-xr-x   0        0        0     7618 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/make.py
+-rwxr-xr-x   0        0        0    58129 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/markup.py
+-rwxr-xr-x   0        0        0      676 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/math.py
+-rwxr-xr-x   0        0        0   132852 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/matlab.py
+-rwxr-xr-x   0        0        0     2716 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/maxima.py
+-rwxr-xr-x   0        0        0     4337 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/meson.py
+-rwxr-xr-x   0        0        0     7538 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/mime.py
+-rwxr-xr-x   0        0        0    13846 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/minecraft.py
+-rwxr-xr-x   0        0        0     4604 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/mips.py
+-rwxr-xr-x   0        0        0    35324 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/ml.py
+-rwxr-xr-x   0        0        0    13524 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/modeling.py
+-rwxr-xr-x   0        0        0    53073 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/modula2.py
+-rwxr-xr-x   0        0        0     6290 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/monte.py
+-rwxr-xr-x   0        0        0     9187 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/mosel.py
+-rwxr-xr-x   0        0        0    63962 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/ncl.py
+-rwxr-xr-x   0        0        0     6416 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/nimrod.py
+-rwxr-xr-x   0        0        0     2726 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/nit.py
+-rwxr-xr-x   0        0        0     4015 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/nix.py
+-rwxr-xr-x   0        0        0     4169 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/oberon.py
+-rwxr-xr-x   0        0        0    22961 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/objective.py
+-rwxr-xr-x   0        0        0     2982 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/ooc.py
+-rwxr-xr-x   0        0        0     1744 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/other.py
+-rwxr-xr-x   0        0        0     2720 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/parasail.py
+-rwxr-xr-x   0        0        0    25904 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/parsers.py
+-rwxr-xr-x   0        0        0    30880 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/pascal.py
+-rwxr-xr-x   0        0        0     8146 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/pawn.py
+-rwxr-xr-x   0        0        0    39170 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/perl.py
+-rwxr-xr-x   0        0        0    23252 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/phix.py
+-rwxr-xr-x   0        0        0    13040 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/php.py
+-rwxr-xr-x   0        0        0     1975 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/pointless.py
+-rwxr-xr-x   0        0        0     3244 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/pony.py
+-rwxr-xr-x   0        0        0    12677 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/praat.py
+-rwxr-xr-x   0        0        0     1156 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/procfile.py
+-rwxr-xr-x   0        0        0    12351 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/prolog.py
+-rwxr-xr-x   0        0        0     4715 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/promql.py
+-rwxr-xr-x   0        0        0    53376 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/python.py
+-rwxr-xr-x   0        0        0     6932 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/q.py
+-rwxr-xr-x   0        0        0     3665 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/qlik.py
+-rwxr-xr-x   0        0        0     6072 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/qvt.py
+-rwxr-xr-x   0        0        0     6185 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/r.py
+-rwxr-xr-x   0        0        0    15790 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/rdf.py
+-rwxr-xr-x   0        0        0    18248 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/rebol.py
+-rwxr-xr-x   0        0        0     2902 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/resource.py
+-rwxr-xr-x   0        0        0     5056 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/ride.py
+-rwxr-xr-x   0        0        0     1128 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/rita.py
+-rwxr-xr-x   0        0        0     1973 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/rnc.py
+-rwxr-xr-x   0        0        0     1962 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/roboconf.py
+-rwxr-xr-x   0        0        0    18449 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/robotframework.py
+-rwxr-xr-x   0        0        0    22775 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/ruby.py
+-rwxr-xr-x   0        0        0     8216 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/rust.py
+-rwxr-xr-x   0        0        0     9400 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/sas.py
+-rwxr-xr-x   0        0        0     4645 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/savi.py
+-rwxr-xr-x   0        0        0     2239 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/scdoc.py
+-rwxr-xr-x   0        0        0    70014 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/scripting.py
+-rwxr-xr-x   0        0        0     1986 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/sgf.py
+-rwxr-xr-x   0        0        0    36466 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/shell.py
+-rwxr-xr-x   0        0        0     2441 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/sieve.py
+-rwxr-xr-x   0        0        0     8482 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/slash.py
+-rwxr-xr-x   0        0        0     7206 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/smalltalk.py
+-rwxr-xr-x   0        0        0     2660 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/smithy.py
+-rwxr-xr-x   0        0        0     2773 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/smv.py
+-rwxr-xr-x   0        0        0     2732 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/snobol.py
+-rwxr-xr-x   0        0        0     3127 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/solidity.py
+-rwxr-xr-x   0        0        0     3330 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/sophia.py
+-rwxr-xr-x   0        0        0     3414 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/special.py
+-rwxr-xr-x   0        0        0     2733 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/spice.py
+-rwxr-xr-x   0        0        0    42086 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/sql.py
+-rwxr-xr-x   0        0        0     1693 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/srcinfo.py
+-rwxr-xr-x   0        0        0     6416 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/stata.py
+-rwxr-xr-x   0        0        0     3698 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/supercollider.py
+-rwxr-xr-x   0        0        0     2639 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/tal.py
+-rwxr-xr-x   0        0        0     5513 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/tcl.py
+-rwxr-xr-x   0        0        0     3523 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/teal.py
+-rwxr-xr-x   0        0        0    72610 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/templates.py
+-rwxr-xr-x   0        0        0     9719 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/teraterm.py
+-rwxr-xr-x   0        0        0    10767 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/testing.py
+-rwxr-xr-x   0        0        0     1029 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/text.py
+-rwxr-xr-x   0        0        0     7609 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/textedit.py
+-rwxr-xr-x   0        0        0    15192 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/textfmts.py
+-rwxr-xr-x   0        0        0    20157 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/theorem.py
+-rwxr-xr-x   0        0        0     4228 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/thingsdb.py
+-rwxr-xr-x   0        0        0     1377 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/tlb.py
+-rwxr-xr-x   0        0        0    10457 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/tnt.py
+-rwxr-xr-x   0        0        0     1474 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/trafficscript.py
+-rwxr-xr-x   0        0        0     8207 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/typoscript.py
+-rwxr-xr-x   0        0        0     8956 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/ul4.py
+-rwxr-xr-x   0        0        0    18512 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/unicon.py
+-rwxr-xr-x   0        0        0     6037 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/urbi.py
+-rwxr-xr-x   0        0        0     3513 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/usd.py
+-rwxr-xr-x   0        0        0     7273 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/varnish.py
+-rwxr-xr-x   0        0        0     3885 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/verification.py
+-rwxr-xr-x   0        0        0      894 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/web.py
+-rwxr-xr-x   0        0        0     5699 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/webassembly.py
+-rwxr-xr-x   0        0        0    10517 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/webidl.py
+-rwxr-xr-x   0        0        0    40549 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/webmisc.py
+-rwxr-xr-x   0        0        0    11920 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/wgsl.py
+-rwxr-xr-x   0        0        0     4018 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/whiley.py
+-rwxr-xr-x   0        0        0     4021 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/wowtoc.py
+-rwxr-xr-x   0        0        0     3239 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/wren.py
+-rwxr-xr-x   0        0        0     1920 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/x10.py
+-rwxr-xr-x   0        0        0      902 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/xorg.py
+-rwxr-xr-x   0        0        0     4500 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/yang.py
+-rwxr-xr-x   0        0        0     3953 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/lexers/zig.py
+-rwxr-xr-x   0        0        0     3676 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/__init__.py
+-rwxr-xr-x   0        0        0      705 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/abap.py
+-rwxr-xr-x   0        0        0     2216 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/algol.py
+-rwxr-xr-x   0        0        0     2231 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/algol_nu.py
+-rwxr-xr-x   0        0        0     4443 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/arduino.py
+-rwxr-xr-x   0        0        0     2096 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/autumn.py
+-rwxr-xr-x   0        0        0     1514 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/borland.py
+-rwxr-xr-x   0        0        0     1308 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/bw.py
+-rwxr-xr-x   0        0        0     2730 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/colorful.py
+-rwxr-xr-x   0        0        0     2488 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/default.py
+-rwxr-xr-x   0        0        0     3314 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/dracula.py
+-rwxr-xr-x   0        0        0     2439 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/emacs.py
+-rwxr-xr-x   0        0        0     2502 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/friendly.py
+-rwxr-xr-x   0        0        0     2707 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/friendly_grayscale.py
+-rwxr-xr-x   0        0        0     1274 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/fruity.py
+-rwxr-xr-x   0        0        0     3481 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/gh_dark.py
+-rwxr-xr-x   0        0        0     3230 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/gruvbox.py
+-rwxr-xr-x   0        0        0      692 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/igor.py
+-rwxr-xr-x   0        0        0     2302 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/inkpot.py
+-rwxr-xr-x   0        0        0     2016 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/lilypond.py
+-rwxr-xr-x   0        0        0     3117 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/lovelace.py
+-rwxr-xr-x   0        0        0     2350 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/manni.py
+-rwxr-xr-x   0        0        0     4083 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/material.py
+-rwxr-xr-x   0        0        0     5063 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/monokai.py
+-rwxr-xr-x   0        0        0     2703 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/murphy.py
+-rwxr-xr-x   0        0        0     1948 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/native.py
+-rwxr-xr-x   0        0        0     5244 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/nord.py
+-rwxr-xr-x   0        0        0     1664 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/onedark.py
+-rwxr-xr-x   0        0        0     5526 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/paraiso_dark.py
+-rwxr-xr-x   0        0        0     5530 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/paraiso_light.py
+-rwxr-xr-x   0        0        0     2425 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/pastie.py
+-rwxr-xr-x   0        0        0     2128 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/perldoc.py
+-rwxr-xr-x   0        0        0     2432 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/rainbow_dash.py
+-rwxr-xr-x   0        0        0      874 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/rrt.py
+-rwxr-xr-x   0        0        0     1393 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/sas.py
+-rwxr-xr-x   0        0        0     4078 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/solarized.py
+-rwxr-xr-x   0        0        0      770 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/staroffice.py
+-rwxr-xr-x   0        0        0     1198 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/stata_dark.py
+-rwxr-xr-x   0        0        0     1227 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/stata_light.py
+-rwxr-xr-x   0        0        0     7039 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/tango.py
+-rwxr-xr-x   0        0        0     1885 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/trac.py
+-rwxr-xr-x   0        0        0     1922 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/vim.py
+-rwxr-xr-x   0        0        0     1026 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/vs.py
+-rwxr-xr-x   0        0        0     1453 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/xcode.py
+-rwxr-xr-x   0        0        0     2148 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/pygments/styles/zenburn.py
+-rwxr-xr-x   0        0        0     1119 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/readme_renderer/__about__.py
+-rwxr-xr-x   0        0        0      573 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/readme_renderer/__init__.py
+-rwxr-xr-x   0        0        0     2622 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/readme_renderer/__main__.py
+-rwxr-xr-x   0        0        0     4290 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/readme_renderer/clean.py
+-rwxr-xr-x   0        0        0     3595 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/readme_renderer/markdown.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/readme_renderer/py.typed
+-rwxr-xr-x   0        0        0     4460 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/readme_renderer/rst.py
+-rwxr-xr-x   0        0        0      823 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/readme_renderer/txt.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/readme_renderer-40.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     9694 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/readme_renderer-40.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     2670 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/readme_renderer-40.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0     1561 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/readme_renderer-40.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/readme_renderer-40.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0       16 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/readme_renderer-40.0.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0     4963 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/__init__.py
+-rwxr-xr-x   0        0        0      435 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/__version__.py
+-rwxr-xr-x   0        0        0     1495 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/_internal_utils.py
+-rwxr-xr-x   0        0        0    19553 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/adapters.py
+-rwxr-xr-x   0        0        0     6449 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/api.py
+-rwxr-xr-x   0        0        0    10187 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/auth.py
+-rwxr-xr-x   0        0        0      429 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/certs.py
+-rwxr-xr-x   0        0        0     1451 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/compat.py
+-rwxr-xr-x   0        0        0    18560 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/cookies.py
+-rwxr-xr-x   0        0        0     3811 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/exceptions.py
+-rwxr-xr-x   0        0        0     3875 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/help.py
+-rwxr-xr-x   0        0        0      733 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/hooks.py
+-rwxr-xr-x   0        0        0    35223 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/models.py
+-rwxr-xr-x   0        0        0      957 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/packages.py
+-rwxr-xr-x   0        0        0    30373 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/sessions.py
+-rwxr-xr-x   0        0        0     4235 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/status_codes.py
+-rwxr-xr-x   0        0        0     2912 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/structures.py
+-rwxr-xr-x   0        0        0    33448 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/utils.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests-2.31.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0    10142 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests-2.31.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     4634 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests-2.31.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0     2761 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests-2.31.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests-2.31.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0        9 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests-2.31.0.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0     1188 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/__init__.py
+-rwxr-xr-x   0        0        0     9260 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/_compat.py
+-rwxr-xr-x   0        0        0      695 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/exceptions.py
+-rwxr-xr-x   0        0        0     3102 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/sessions.py
+-rwxr-xr-x   0        0        0     4044 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/streaming_iterator.py
+-rwxr-xr-x   0        0        0      370 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/adapters/__init__.py
+-rwxr-xr-x   0        0        0     7539 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/adapters/appengine.py
+-rwxr-xr-x   0        0        0     1404 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/adapters/fingerprint.py
+-rwxr-xr-x   0        0        0     1396 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/adapters/host_header_ssl.py
+-rwxr-xr-x   0        0        0     4789 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/adapters/socket_options.py
+-rwxr-xr-x   0        0        0     2608 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/adapters/source.py
+-rwxr-xr-x   0        0        0     2399 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/adapters/ssl.py
+-rwxr-xr-x   0        0        0     7854 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/adapters/x509.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/auth/__init__.py
+-rwxr-xr-x   0        0        0      910 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/auth/_digest_auth_compat.py
+-rwxr-xr-x   0        0        0     4944 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/auth/guess.py
+-rwxr-xr-x   0        0        0     4407 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/auth/handler.py
+-rwxr-xr-x   0        0        0     3706 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/auth/http_proxy_digest.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/cookies/__init__.py
+-rwxr-xr-x   0        0        0      213 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/cookies/forgetful.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/downloadutils/__init__.py
+-rwxr-xr-x   0        0        0     6024 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/downloadutils/stream.py
+-rwxr-xr-x   0        0        0     4365 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/downloadutils/tee.py
+-rwxr-xr-x   0        0        0      854 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/multipart/__init__.py
+-rwxr-xr-x   0        0        0     4861 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/multipart/decoder.py
+-rwxr-xr-x   0        0        0    20769 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/multipart/encoder.py
+-rwxr-xr-x   0        0        0     3213 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/threaded/__init__.py
+-rwxr-xr-x   0        0        0     6628 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/threaded/pool.py
+-rwxr-xr-x   0        0        0     1465 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/threaded/thread.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/utils/__init__.py
+-rwxr-xr-x   0        0        0     2558 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/utils/deprecated.py
+-rwxr-xr-x   0        0        0     6522 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/utils/dump.py
+-rwxr-xr-x   0        0        0     3233 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/utils/formdata.py
+-rwxr-xr-x   0        0        0     4524 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt/utils/user_agent.py
+-rwxr-xr-x   0        0        0      986 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt-1.0.0.dist-info/AUTHORS.rst
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt-1.0.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0      596 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt-1.0.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0    14638 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt-1.0.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0     6078 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt-1.0.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0      110 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt-1.0.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0       18 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests_toolbelt-1.0.0.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0     1565 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rfc3986/__init__.py
+-rwxr-xr-x   0        0        0    13297 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rfc3986/_mixin.py
+-rwxr-xr-x   0        0        0     9048 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rfc3986/abnf_regexp.py
+-rwxr-xr-x   0        0        0     3862 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rfc3986/api.py
+-rwxr-xr-x   0        0        0    12709 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rfc3986/builder.py
+-rwxr-xr-x   0        0        0     1620 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rfc3986/compat.py
+-rwxr-xr-x   0        0        0     3614 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rfc3986/exceptions.py
+-rwxr-xr-x   0        0        0     5477 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rfc3986/iri.py
+-rwxr-xr-x   0        0        0     4114 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rfc3986/misc.py
+-rwxr-xr-x   0        0        0     5261 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rfc3986/normalizers.py
+-rwxr-xr-x   0        0        0    14599 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rfc3986/parseresult.py
+-rwxr-xr-x   0        0        0     5183 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rfc3986/uri.py
+-rwxr-xr-x   0        0        0    13676 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rfc3986/validators.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rfc3986-2.0.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0      564 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rfc3986-2.0.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     6630 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rfc3986-2.0.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0     2085 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rfc3986-2.0.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0      110 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rfc3986-2.0.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0        8 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rfc3986-2.0.0.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0     6066 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/__init__.py
+-rwxr-xr-x   0        0        0     8334 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/__main__.py
+-rwxr-xr-x   0        0        0    10096 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/_cell_widths.py
+-rwxr-xr-x   0        0        0   140235 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/_emoji_codes.py
+-rwxr-xr-x   0        0        0     1064 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/_emoji_replace.py
+-rwxr-xr-x   0        0        0     2100 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/_export_format.py
+-rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/_extension.py
+-rwxr-xr-x   0        0        0      799 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/_fileno.py
+-rwxr-xr-x   0        0        0     9695 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/_inspect.py
+-rwxr-xr-x   0        0        0     3213 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/_log_render.py
+-rwxr-xr-x   0        0        0     1236 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/_loop.py
+-rwxr-xr-x   0        0        0     1387 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/_null_file.py
+-rwxr-xr-x   0        0        0     7063 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/_palettes.py
+-rwxr-xr-x   0        0        0      423 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/_pick.py
+-rwxr-xr-x   0        0        0     5460 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/_ratio.py
+-rwxr-xr-x   0        0        0    19919 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/_spinners.py
+-rwxr-xr-x   0        0        0      351 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/_stack.py
+-rwxr-xr-x   0        0        0      417 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/_timer.py
+-rwxr-xr-x   0        0        0    22784 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/_win32_console.py
+-rwxr-xr-x   0        0        0     1902 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/_windows.py
+-rwxr-xr-x   0        0        0     2759 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/_windows_renderer.py
+-rwxr-xr-x   0        0        0     1840 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/_wrap.py
+-rwxr-xr-x   0        0        0      878 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/abc.py
+-rwxr-xr-x   0        0        0    10320 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/align.py
+-rwxr-xr-x   0        0        0     6906 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/ansi.py
+-rwxr-xr-x   0        0        0     3264 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/bar.py
+-rwxr-xr-x   0        0        0     9794 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/box.py
+-rwxr-xr-x   0        0        0     4509 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/cells.py
+-rwxr-xr-x   0        0        0    18224 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/color.py
+-rwxr-xr-x   0        0        0     1054 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/color_triplet.py
+-rwxr-xr-x   0        0        0     7131 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/columns.py
+-rwxr-xr-x   0        0        0    99146 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/console.py
+-rwxr-xr-x   0        0        0     1288 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/constrain.py
+-rwxr-xr-x   0        0        0     5497 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/containers.py
+-rwxr-xr-x   0        0        0     6606 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/control.py
+-rwxr-xr-x   0        0        0     8046 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/default_styles.py
+-rwxr-xr-x   0        0        0      924 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/diagnose.py
+-rwxr-xr-x   0        0        0     2465 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/emoji.py
+-rwxr-xr-x   0        0        0      642 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/errors.py
+-rwxr-xr-x   0        0        0     1683 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/file_proxy.py
+-rwxr-xr-x   0        0        0     2508 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/filesize.py
+-rwxr-xr-x   0        0        0     9584 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/highlighter.py
+-rwxr-xr-x   0        0        0     5020 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/json.py
+-rwxr-xr-x   0        0        0     3228 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/jupyter.py
+-rwxr-xr-x   0        0        0    13947 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/layout.py
+-rwxr-xr-x   0        0        0    14273 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/live.py
+-rwxr-xr-x   0        0        0     3655 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/live_render.py
+-rwxr-xr-x   0        0        0    11891 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/logging.py
+-rwxr-xr-x   0        0        0    26245 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/markdown.py
+-rwxr-xr-x   0        0        0     8174 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/markup.py
+-rwxr-xr-x   0        0        0     5305 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/measure.py
+-rwxr-xr-x   0        0        0     4958 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/padding.py
+-rwxr-xr-x   0        0        0      828 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/pager.py
+-rwxr-xr-x   0        0        0     3288 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/palette.py
+-rwxr-xr-x   0        0        0    10574 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/panel.py
+-rwxr-xr-x   0        0        0    35816 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/pretty.py
+-rwxr-xr-x   0        0        0    59694 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/progress.py
+-rwxr-xr-x   0        0        0     8165 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/progress_bar.py
+-rwxr-xr-x   0        0        0    11291 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/prompt.py
+-rwxr-xr-x   0        0        0     1367 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/protocol.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/py.typed
+-rwxr-xr-x   0        0        0      166 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/region.py
+-rwxr-xr-x   0        0        0     4419 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/repr.py
+-rwxr-xr-x   0        0        0     4590 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/rule.py
+-rwxr-xr-x   0        0        0     2831 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/scope.py
+-rwxr-xr-x   0        0        0     1579 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/screen.py
+-rwxr-xr-x   0        0        0    24211 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/segment.py
+-rwxr-xr-x   0        0        0     4339 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/spinner.py
+-rwxr-xr-x   0        0        0     4425 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/status.py
+-rwxr-xr-x   0        0        0    27073 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/style.py
+-rwxr-xr-x   0        0        0     1234 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/styled.py
+-rwxr-xr-x   0        0        0    35065 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/syntax.py
+-rwxr-xr-x   0        0        0    39648 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/table.py
+-rwxr-xr-x   0        0        0     3370 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/terminal_theme.py
+-rwxr-xr-x   0        0        0    45513 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/text.py
+-rwxr-xr-x   0        0        0     3777 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/theme.py
+-rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/themes.py
+-rwxr-xr-x   0        0        0    29532 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/traceback.py
+-rwxr-xr-x   0        0        0     9109 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich/tree.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich-13.4.2.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1056 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich-13.4.2.dist-info/LICENSE
+-rwxr-xr-x   0        0        0    18837 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich-13.4.2.dist-info/METADATA
+-rwxr-xr-x   0        0        0     9650 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich-13.4.2.dist-info/RECORD
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/rich-13.4.2.dist-info/WHEEL
+-rwxr-xr-x   0        0        0     3364 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/secretstorage/__init__.py
+-rwxr-xr-x   0        0        0     9436 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/secretstorage/collection.py
+-rwxr-xr-x   0        0        0      807 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/secretstorage/defines.py
+-rwxr-xr-x   0        0        0     2578 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/secretstorage/dhcrypto.py
+-rwxr-xr-x   0        0        0     1655 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/secretstorage/exceptions.py
+-rwxr-xr-x   0        0        0     5813 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/secretstorage/item.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/secretstorage/py.typed
+-rwxr-xr-x   0        0        0     6755 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/secretstorage/util.py
+-rwxr-xr-x   0        0        0     7681 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/__init__.py
+-rwxr-xr-x   0        0        0      218 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_deprecation_warning.py
+-rwxr-xr-x   0        0        0     2392 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_imp.py
+-rwxr-xr-x   0        0        0     7077 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/archive_util.py
+-rwxr-xr-x   0        0        0    10280 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/build_meta.py
+-rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/cli-32.exe
+-rwxr-xr-x   0        0        0    74752 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/cli-64.exe
+-rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/cli.exe
+-rwxr-xr-x   0        0        0    22279 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/config.py
+-rwxr-xr-x   0        0        0      949 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/dep_util.py
+-rwxr-xr-x   0        0        0     5474 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/depends.py
+-rwxr-xr-x   0        0        0    42591 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/dist.py
+-rwxr-xr-x   0        0        0      524 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/errors.py
+-rwxr-xr-x   0        0        0     1684 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/extension.py
+-rwxr-xr-x   0        0        0     4873 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/glob.py
+-rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/gui-32.exe
+-rwxr-xr-x   0        0        0    75264 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/gui-64.exe
+-rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/gui.exe
+-rwxr-xr-x   0        0        0     3567 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/installer.py
+-rwxr-xr-x   0        0        0      812 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/launch.py
+-rwxr-xr-x   0        0        0     2335 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/lib2to3_ex.py
+-rwxr-xr-x   0        0        0     5217 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/monkey.py
+-rwxr-xr-x   0        0        0    50561 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/msvc.py
+-rwxr-xr-x   0        0        0     3093 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/namespaces.py
+-rwxr-xr-x   0        0        0    39886 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/package_index.py
+-rwxr-xr-x   0        0        0      245 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/py34compat.py
+-rwxr-xr-x   0        0        0    14151 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/sandbox.py
+-rwxr-xr-x   0        0        0      218 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/script (dev).tmpl
+-rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/script.tmpl
+-rwxr-xr-x   0        0        0      941 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/unicode_utils.py
+-rwxr-xr-x   0        0        0      144 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/version.py
+-rwxr-xr-x   0        0        0     8288 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/wheel.py
+-rwxr-xr-x   0        0        0      714 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/windows_support.py
+-rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/__init__.py
+-rwxr-xr-x   0        0        0    20813 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/_msvccompiler.py
+-rwxr-xr-x   0        0        0     8572 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/archive_util.py
+-rwxr-xr-x   0        0        0    14894 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/bcppcompiler.py
+-rwxr-xr-x   0        0        0    47607 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/ccompiler.py
+-rwxr-xr-x   0        0        0    18079 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/cmd.py
+-rwxr-xr-x   0        0        0     4827 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/config.py
+-rwxr-xr-x   0        0        0     8876 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/core.py
+-rwxr-xr-x   0        0        0    16938 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rwxr-xr-x   0        0        0      139 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/debug.py
+-rwxr-xr-x   0        0        0     3491 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/dep_util.py
+-rwxr-xr-x   0        0        0     7778 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/dir_util.py
+-rwxr-xr-x   0        0        0    50421 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/dist.py
+-rwxr-xr-x   0        0        0     3577 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/errors.py
+-rwxr-xr-x   0        0        0    10515 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/extension.py
+-rwxr-xr-x   0        0        0    17784 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/fancy_getopt.py
+-rwxr-xr-x   0        0        0     8148 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/file_util.py
+-rwxr-xr-x   0        0        0    13407 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/filelist.py
+-rwxr-xr-x   0        0        0     1969 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/log.py
+-rwxr-xr-x   0        0        0    30453 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/msvc9compiler.py
+-rwxr-xr-x   0        0        0    23540 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/msvccompiler.py
+-rwxr-xr-x   0        0        0      455 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/py35compat.py
+-rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/py38compat.py
+-rwxr-xr-x   0        0        0     3498 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/spawn.py
+-rwxr-xr-x   0        0        0    21349 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/sysconfig.py
+-rwxr-xr-x   0        0        0    12483 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/text_file.py
+-rwxr-xr-x   0        0        0    14957 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/unixccompiler.py
+-rwxr-xr-x   0        0        0    23185 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/util.py
+-rwxr-xr-x   0        0        0    12514 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/version.py
+-rwxr-xr-x   0        0        0     5133 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/versionpredicate.py
+-rwxr-xr-x   0        0        0      799 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/__init__.py
+-rwxr-xr-x   0        0        0     5562 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/bdist.py
+-rwxr-xr-x   0        0        0     4913 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rwxr-xr-x   0        0        0    35579 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_msi.py
+-rwxr-xr-x   0        0        0    21537 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rwxr-xr-x   0        0        0    16030 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_wininst.py
+-rwxr-xr-x   0        0        0     5773 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/build.py
+-rwxr-xr-x   0        0        0     8022 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/build_clib.py
+-rwxr-xr-x   0        0        0    31720 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/build_ext.py
+-rwxr-xr-x   0        0        0    17190 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/build_py.py
+-rwxr-xr-x   0        0        0     6232 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/build_scripts.py
+-rwxr-xr-x   0        0        0     5637 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/check.py
+-rwxr-xr-x   0        0        0     2776 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/clean.py
+-rwxr-xr-x   0        0        0    13117 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/config.py
+-rwxr-xr-x   0        0        0    27488 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/install.py
+-rwxr-xr-x   0        0        0     2822 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/install_data.py
+-rwxr-xr-x   0        0        0     2603 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rwxr-xr-x   0        0        0     1298 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/install_headers.py
+-rwxr-xr-x   0        0        0     8397 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/install_lib.py
+-rwxr-xr-x   0        0        0     2017 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/install_scripts.py
+-rwxr-xr-x   0        0        0      671 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/py37compat.py
+-rwxr-xr-x   0        0        0    11712 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/register.py
+-rwxr-xr-x   0        0        0    19005 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/sdist.py
+-rwxr-xr-x   0        0        0     7597 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/upload.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/__init__.py
+-rwxr-xr-x   0        0        0    15130 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/ordered_set.py
+-rwxr-xr-x   0        0        0   232056 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/pyparsing.py
+-rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rwxr-xr-x   0        0        0   117968 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/more.py
+-rwxr-xr-x   0        0        0    16256 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rwxr-xr-x   0        0        0      736 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/__about__.py
+-rwxr-xr-x   0        0        0      562 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/__init__.py
+-rwxr-xr-x   0        0        0     1128 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/_compat.py
+-rwxr-xr-x   0        0        0     2022 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/_structures.py
+-rwxr-xr-x   0        0        0     1812 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/_typing.py
+-rwxr-xr-x   0        0        0     9509 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/markers.py
+-rwxr-xr-x   0        0        0     4917 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/requirements.py
+-rwxr-xr-x   0        0        0    31944 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rwxr-xr-x   0        0        0    24067 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/tags.py
+-rwxr-xr-x   0        0        0     1811 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/utils.py
+-rwxr-xr-x   0        0        0    15470 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/version.py
+-rwxr-xr-x   0        0        0      217 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/__init__.py
+-rwxr-xr-x   0        0        0     2381 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/alias.py
+-rwxr-xr-x   0        0        0    16604 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/bdist_egg.py
+-rwxr-xr-x   0        0        0      900 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/bdist_rpm.py
+-rwxr-xr-x   0        0        0     4415 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/build_clib.py
+-rwxr-xr-x   0        0        0    13212 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/build_ext.py
+-rwxr-xr-x   0        0        0     8930 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/build_py.py
+-rwxr-xr-x   0        0        0     8045 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/develop.py
+-rwxr-xr-x   0        0        0      960 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/dist_info.py
+-rwxr-xr-x   0        0        0    85308 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/easy_install.py
+-rwxr-xr-x   0        0        0    25335 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/egg_info.py
+-rwxr-xr-x   0        0        0     4705 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/install.py
+-rwxr-xr-x   0        0        0     2203 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/install_egg_info.py
+-rwxr-xr-x   0        0        0     3875 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/install_lib.py
+-rwxr-xr-x   0        0        0     2593 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/install_scripts.py
+-rwxr-xr-x   0        0        0      628 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/launcher manifest.xml
+-rwxr-xr-x   0        0        0     4946 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/py36compat.py
+-rwxr-xr-x   0        0        0      468 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/register.py
+-rwxr-xr-x   0        0        0     2128 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/rotate.py
+-rwxr-xr-x   0        0        0      658 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/saveopts.py
+-rwxr-xr-x   0        0        0     5967 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/sdist.py
+-rwxr-xr-x   0        0        0     5051 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/setopt.py
+-rwxr-xr-x   0        0        0     9490 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/test.py
+-rwxr-xr-x   0        0        0      462 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/upload.py
+-rwxr-xr-x   0        0        0     7218 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/upload_docs.py
+-rwxr-xr-x   0        0        0     2407 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/extern/__init__.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools-57.4.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1050 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools-57.4.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     4908 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools-57.4.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0    23214 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools-57.4.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools-57.4.0.dist-info/REQUESTED
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools-57.4.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0     2869 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools-57.4.0.dist-info/entry_points.txt
+-rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools-57.4.0.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/six-1.16.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1066 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/six-1.16.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     1795 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/six-1.16.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0      561 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/six-1.16.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0      110 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/six-1.16.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/six-1.16.0.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0     1343 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/twine/__init__.py
+-rwxr-xr-x   0        0        0     1475 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/twine/__main__.py
+-rwxr-xr-x   0        0        0     3129 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/twine/auth.py
+-rwxr-xr-x   0        0        0     3738 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/twine/cli.py
+-rwxr-xr-x   0        0        0     3814 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/twine/exceptions.py
+-rwxr-xr-x   0        0        0    11024 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/twine/package.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/twine/py.typed
+-rwxr-xr-x   0        0        0     8713 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/twine/repository.py
+-rwxr-xr-x   0        0        0    12269 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/twine/settings.py
+-rwxr-xr-x   0        0        0    10867 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/twine/utils.py
+-rwxr-xr-x   0        0        0     3049 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/twine/wheel.py
+-rwxr-xr-x   0        0        0     1795 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/twine/wininst.py
+-rwxr-xr-x   0        0        0     1802 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/twine/commands/__init__.py
+-rwxr-xr-x   0        0        0     5727 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/twine/commands/check.py
+-rwxr-xr-x   0        0        0     2904 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/twine/commands/register.py
+-rwxr-xr-x   0        0        0     7469 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/twine/commands/upload.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/twine-4.0.2.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     9695 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/twine-4.0.2.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     3259 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/twine-4.0.2.dist-info/METADATA
+-rwxr-xr-x   0        0        0     2645 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/twine-4.0.2.dist-info/RECORD
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/twine-4.0.2.dist-info/REQUESTED
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/twine-4.0.2.dist-info/WHEEL
+-rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/twine-4.0.2.dist-info/entry_points.txt
+-rwxr-xr-x   0        0        0        6 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/twine-4.0.2.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0     5283 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/__init__.py
+-rwxr-xr-x   0        0        0     5651 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/_base_connection.py
+-rwxr-xr-x   0        0        0    15561 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/_collections.py
+-rwxr-xr-x   0        0        0     7756 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/_request_methods.py
+-rwxr-xr-x   0        0        0       98 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/_version.py
+-rwxr-xr-x   0        0        0    33622 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/connection.py
+-rwxr-xr-x   0        0        0    42961 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/connectionpool.py
+-rwxr-xr-x   0        0        0     9385 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/exceptions.py
+-rwxr-xr-x   0        0        0    11026 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/fields.py
+-rwxr-xr-x   0        0        0     2395 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/filepost.py
+-rwxr-xr-x   0        0        0    22648 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/poolmanager.py
+-rwxr-xr-x   0        0        0       93 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/py.typed
+-rwxr-xr-x   0        0        0    40092 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/response.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/contrib/__init__.py
+-rwxr-xr-x   0        0        0    19437 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/contrib/pyopenssl.py
+-rwxr-xr-x   0        0        0    34121 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/contrib/securetransport.py
+-rwxr-xr-x   0        0        0     7715 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/contrib/socks.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/contrib/_securetransport/__init__.py
+-rwxr-xr-x   0        0        0    14452 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/contrib/_securetransport/bindings.py
+-rwxr-xr-x   0        0        0    16220 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/contrib/_securetransport/low_level.py
+-rwxr-xr-x   0        0        0     1051 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/__init__.py
+-rwxr-xr-x   0        0        0     4462 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/connection.py
+-rwxr-xr-x   0        0        0     1148 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/proxy.py
+-rwxr-xr-x   0        0        0     8111 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/request.py
+-rwxr-xr-x   0        0        0     3374 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/response.py
+-rwxr-xr-x   0        0        0    18374 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/retry.py
+-rwxr-xr-x   0        0        0    18860 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/ssl_.py
+-rwxr-xr-x   0        0        0     5812 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/ssl_match_hostname.py
+-rwxr-xr-x   0        0        0     9045 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/ssltransport.py
+-rwxr-xr-x   0        0        0    10529 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/timeout.py
+-rwxr-xr-x   0        0        0    15213 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/url.py
+-rwxr-xr-x   0        0        0     1146 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/util.py
+-rwxr-xr-x   0        0        0     4423 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/wait.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3-2.0.3.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     6591 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3-2.0.3.dist-info/METADATA
+-rwxr-xr-x   0        0        0     4877 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3-2.0.3.dist-info/RECORD
+-rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3-2.0.3.dist-info/WHEEL
+-rwxr-xr-x   0        0        0     1093 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3-2.0.3.dist-info/licenses/LICENSE.txt
+-rwxr-xr-x   0        0        0    10579 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/webencodings/__init__.py
+-rwxr-xr-x   0        0        0     8979 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/webencodings/labels.py
+-rwxr-xr-x   0        0        0     1305 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/webencodings/mklabels.py
+-rwxr-xr-x   0        0        0     6563 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/webencodings/tests.py
+-rwxr-xr-x   0        0        0     4307 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/webencodings/x_user_defined.py
+-rwxr-xr-x   0        0        0     1039 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/webencodings-0.5.1.dist-info/DESCRIPTION.rst
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/webencodings-0.5.1.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     2063 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/webencodings-0.5.1.dist-info/METADATA
+-rwxr-xr-x   0        0        0     1296 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/webencodings-0.5.1.dist-info/RECORD
+-rwxr-xr-x   0        0        0      110 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/webencodings-0.5.1.dist-info/WHEEL
+-rwxr-xr-x   0        0        0     1092 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/webencodings-0.5.1.dist-info/metadata.json
+-rwxr-xr-x   0        0        0       13 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/webencodings-0.5.1.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0    10676 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/zipp/__init__.py
+-rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/zipp/py310compat.py
+-rwxr-xr-x   0        0        0        4 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/zipp-3.15.0.dist-info/INSTALLER
+-rwxr-xr-x   0        0        0     1050 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/zipp-3.15.0.dist-info/LICENSE
+-rwxr-xr-x   0        0        0     3735 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/zipp-3.15.0.dist-info/METADATA
+-rwxr-xr-x   0        0        0      710 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/zipp-3.15.0.dist-info/RECORD
+-rwxr-xr-x   0        0        0       92 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/zipp-3.15.0.dist-info/WHEEL
+-rwxr-xr-x   0        0        0        5 2020-02-02 00:00:00.000000 hatch_project-0.2.0/.test/lib/python3.10/site-packages/zipp-3.15.0.dist-info/top_level.txt
+-rwxr-xr-x   0        0        0       55 2020-02-02 00:00:00.000000 hatch_project-0.2.0/src/__init__.py
+-rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 hatch_project-0.2.0/src/hatch_project/__about__.py
+-rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 hatch_project-0.2.0/src/hatch_project/__init__.py
+-rwxr-xr-x   0        0        0      545 2020-02-02 00:00:00.000000 hatch_project-0.2.0/src/hatch_project/scraping.py
+-rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 hatch_project-0.2.0/tests/__init__.py
+-rwxr-xr-x   0        0        0      955 2020-02-02 00:00:00.000000 hatch_project-0.2.0/tests/test_scraping.py
+-rwxr-xr-x   0        0        0     1101 2020-02-02 00:00:00.000000 hatch_project-0.2.0/LICENSE.txt
+-rwxr-xr-x   0        0        0      513 2020-02-02 00:00:00.000000 hatch_project-0.2.0/README.md
+-rwxr-xr-x   0        0        0     3343 2020-02-02 00:00:00.000000 hatch_project-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 hatch_project-0.2.0/PKG-INFO
```

### Comparing `hatch_project-0.1.2/.test/bin/Activate.ps1` & `hatch_project-0.2.0/.test/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/bin/activate` & `hatch_project-0.2.0/.test/bin/activate`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/bin/activate.csh` & `hatch_project-0.2.0/.test/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/bin/activate.fish` & `hatch_project-0.2.0/.test/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/_distutils_hack/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/_distutils_hack/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/beautifulsoup4-4.12.2.dist-info/licenses/LICENSE` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/more_itertools-9.1.0.dist-info/LICENSE`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,19 @@
-Beautiful Soup is made available under the MIT license:
+Copyright (c) 2012 Erik Rose
 
- Copyright (c) Leonard Richardson
-
- Permission is hereby granted, free of charge, to any person obtaining
- a copy of this software and associated documentation files (the
- "Software"), to deal in the Software without restriction, including
- without limitation the rights to use, copy, modify, merge, publish,
- distribute, sublicense, and/or sell copies of the Software, and to
- permit persons to whom the Software is furnished to do so, subject to
- the following conditions:
-
- The above copyright notice and this permission notice shall be
- included in all copies or substantial portions of the Software.
-
- THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
- EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
- MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
- NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
- BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
- ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
- CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
- SOFTWARE.
-
-Beautiful Soup incorporates code from the html5lib library, which is
-also made available under the MIT license. Copyright (c) James Graham
-and other contributors
-
-Beautiful Soup has an optional dependency on the soupsieve library,
-which is also made available under the MIT license. Copyright (c)
-Isaac Muse
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+of the Software, and to permit persons to whom the Software is furnished to do
+so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/element.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/docutils/nodes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,2430 +1,2315 @@
-# Use of this source code is governed by the MIT license.
-__license__ = "MIT"
+# $Id: nodes.py 9310 2022-12-17 12:17:32Z milde $
+# Author: David Goodger <goodger@python.org>
+# Maintainer: docutils-develop@lists.sourceforge.net
+# Copyright: This module has been placed in the public domain.
+
+"""
+Docutils document tree element class library.
+
+Classes in CamelCase are abstract base classes or auxiliary classes. The one
+exception is `Text`, for a text (PCDATA) node; uppercase is used to
+differentiate from element classes.  Classes in lower_case_with_underscores
+are element classes, matching the XML element generic identifiers in the DTD_.
+
+The position of each node (the level at which it can occur) is significant and
+is represented by abstract base classes (`Root`, `Structural`, `Body`,
+`Inline`, etc.).  Certain transformations will be easier because we can use
+``isinstance(node, base_class)`` to determine the position of the node in the
+hierarchy.
 
-try:
-    from collections.abc import Callable # Python 3.6
-except ImportError as e:
-    from collections import Callable
+.. _DTD: https://docutils.sourceforge.io/docs/ref/docutils.dtd
+"""
+
+__docformat__ = 'reStructuredText'
+
+from collections import Counter
 import re
 import sys
 import warnings
+import unicodedata
+# import xml.dom.minidom as dom # -> conditional import in Node.asdom()
+#                                    and document.asdom()
+
+# import docutils.transforms # -> conditional import in document.__init__()
+
+
+# ==============================
+#  Functional Node Base Classes
+# ==============================
+
+class Node:
+    """Abstract base class of nodes in a document tree."""
+
+    parent = None
+    """Back-reference to the Node immediately containing this Node."""
 
-from bs4.css import CSS
-from bs4.formatter import (
-    Formatter,
-    HTMLFormatter,
-    XMLFormatter,
-)
-
-DEFAULT_OUTPUT_ENCODING = "utf-8"
-
-nonwhitespace_re = re.compile(r"\S+")
-
-# NOTE: This isn't used as of 4.7.0. I'm leaving it for a little bit on
-# the off chance someone imported it for their own use.
-whitespace_re = re.compile(r"\s+")
+    source = None
+    """Path or description of the input source which generated this Node."""
+
+    line = None
+    """The line number (1-based) of the beginning of this Node in `source`."""
+
+    _document = None
 
-def _alias(attr):
-    """Alias one attribute name to another for backward compatibility"""
     @property
-    def alias(self):
-        return getattr(self, attr)
+    def document(self):
+        """Return the `document` root node of the tree containing this Node.
+        """
+        try:
+            return self._document or self.parent.document
+        except AttributeError:
+            return None
 
-    @alias.setter
-    def alias(self):
-        return setattr(self, attr)
-    return alias
-
-
-# These encodings are recognized by Python (so PageElement.encode
-# could theoretically support them) but XML and HTML don't recognize
-# them (so they should not show up in an XML or HTML document as that
-# document's encoding).
-#
-# If an XML document is encoded in one of these encodings, no encoding
-# will be mentioned in the XML declaration. If an HTML document is
-# encoded in one of these encodings, and the HTML document has a
-# <meta> tag that mentions an encoding, the encoding will be given as
-# the empty string.
-#
-# Source:
-# https://docs.python.org/3/library/codecs.html#python-specific-encodings
-PYTHON_SPECIFIC_ENCODINGS = set([
-    "idna",
-    "mbcs",
-    "oem",
-    "palmos",
-    "punycode",
-    "raw_unicode_escape",
-    "undefined",
-    "unicode_escape",
-    "raw-unicode-escape",
-    "unicode-escape",
-    "string-escape",
-    "string_escape",
-])
-
-
-class NamespacedAttribute(str):
-    """A namespaced string (e.g. 'xml:lang') that remembers the namespace
-    ('xml') and the name ('lang') that were used to create it.
-    """
-
-    def __new__(cls, prefix, name=None, namespace=None):
-        if not name:
-            # This is the default namespace. Its name "has no value"
-            # per https://www.w3.org/TR/xml-names/#defaulting
-            name = None
-
-        if not name:
-            obj = str.__new__(cls, prefix)
-        elif not prefix:
-            # Not really namespaced.
-            obj = str.__new__(cls, name)
-        else:
-            obj = str.__new__(cls, prefix + ":" + name)
-        obj.prefix = prefix
-        obj.name = name
-        obj.namespace = namespace
-        return obj
+    @document.setter
+    def document(self, value):
+        self._document = value
 
-class AttributeValueWithCharsetSubstitution(str):
-    """A stand-in object for a character encoding specified in HTML."""
+    def __bool__(self):
+        """
+        Node instances are always true, even if they're empty.  A node is more
+        than a simple container.  Its boolean "truth" does not depend on
+        having one or more subnodes in the doctree.
 
-class CharsetMetaAttributeValue(AttributeValueWithCharsetSubstitution):
-    """A generic stand-in for the value of a meta tag's 'charset' attribute.
+        Use `len()` to check node length.
+        """
+        return True
 
-    When Beautiful Soup parses the markup '<meta charset="utf8">', the
-    value of the 'charset' attribute will be one of these objects.
-    """
+    def asdom(self, dom=None):
+        """Return a DOM **fragment** representation of this Node."""
+        if dom is None:
+            import xml.dom.minidom as dom
+        domroot = dom.Document()
+        return self._dom_node(domroot)
+
+    def pformat(self, indent='    ', level=0):
+        """
+        Return an indented pseudo-XML representation, for test purposes.
+
+        Override in subclasses.
+        """
+        raise NotImplementedError
+
+    def copy(self):
+        """Return a copy of self."""
+        raise NotImplementedError
+
+    def deepcopy(self):
+        """Return a deep copy of self (also copying children)."""
+        raise NotImplementedError
+
+    def astext(self):
+        """Return a string representation of this Node."""
+        raise NotImplementedError
+
+    def setup_child(self, child):
+        child.parent = self
+        if self.document:
+            child.document = self.document
+            if child.source is None:
+                child.source = self.document.current_source
+            if child.line is None:
+                child.line = self.document.current_line
+
+    def walk(self, visitor):
+        """
+        Traverse a tree of `Node` objects, calling the
+        `dispatch_visit()` method of `visitor` when entering each
+        node.  (The `walkabout()` method is similar, except it also
+        calls the `dispatch_departure()` method before exiting each
+        node.)
+
+        This tree traversal supports limited in-place tree
+        modifications.  Replacing one node with one or more nodes is
+        OK, as is removing an element.  However, if the node removed
+        or replaced occurs after the current node, the old node will
+        still be traversed, and any new nodes will not.
+
+        Within ``visit`` methods (and ``depart`` methods for
+        `walkabout()`), `TreePruningException` subclasses may be raised
+        (`SkipChildren`, `SkipSiblings`, `SkipNode`, `SkipDeparture`).
+
+        Parameter `visitor`: A `NodeVisitor` object, containing a
+        ``visit`` implementation for each `Node` subclass encountered.
+
+        Return true if we should stop the traversal.
+        """
+        stop = False
+        visitor.document.reporter.debug(
+            'docutils.nodes.Node.walk calling dispatch_visit for %s'
+            % self.__class__.__name__)
+        try:
+            try:
+                visitor.dispatch_visit(self)
+            except (SkipChildren, SkipNode):
+                return stop
+            except SkipDeparture:           # not applicable; ignore
+                pass
+            children = self.children
+            try:
+                for child in children[:]:
+                    if child.walk(visitor):
+                        stop = True
+                        break
+            except SkipSiblings:
+                pass
+        except StopTraversal:
+            stop = True
+        return stop
+
+    def walkabout(self, visitor):
+        """
+        Perform a tree traversal similarly to `Node.walk()` (which
+        see), except also call the `dispatch_departure()` method
+        before exiting each node.
+
+        Parameter `visitor`: A `NodeVisitor` object, containing a
+        ``visit`` and ``depart`` implementation for each `Node`
+        subclass encountered.
+
+        Return true if we should stop the traversal.
+        """
+        call_depart = True
+        stop = False
+        visitor.document.reporter.debug(
+            'docutils.nodes.Node.walkabout calling dispatch_visit for %s'
+            % self.__class__.__name__)
+        try:
+            try:
+                visitor.dispatch_visit(self)
+            except SkipNode:
+                return stop
+            except SkipDeparture:
+                call_depart = False
+            children = self.children
+            try:
+                for child in children[:]:
+                    if child.walkabout(visitor):
+                        stop = True
+                        break
+            except SkipSiblings:
+                pass
+        except SkipChildren:
+            pass
+        except StopTraversal:
+            stop = True
+        if call_depart:
+            visitor.document.reporter.debug(
+                'docutils.nodes.Node.walkabout calling dispatch_departure '
+                'for %s' % self.__class__.__name__)
+            visitor.dispatch_departure(self)
+        return stop
+
+    def _fast_findall(self, cls):
+        """Return iterator that only supports instance checks."""
+        if isinstance(self, cls):
+            yield self
+        for child in self.children:
+            yield from child._fast_findall(cls)
 
-    def __new__(cls, original_value):
-        obj = str.__new__(cls, original_value)
-        obj.original_value = original_value
-        return obj
+    def _superfast_findall(self):
+        """Return iterator that doesn't check for a condition."""
+        # This is different from ``iter(self)`` implemented via
+        # __getitem__() and __len__() in the Element subclass,
+        # which yields only the direct children.
+        yield self
+        for child in self.children:
+            yield from child._superfast_findall()
+
+    def traverse(self, condition=None, include_self=True, descend=True,
+                 siblings=False, ascend=False):
+        """Return list of nodes following `self`.
+
+        For looping, Node.findall() is faster and more memory efficient.
+        """
+        # traverse() may be eventually removed:
+        warnings.warn('nodes.Node.traverse() is obsoleted by Node.findall().',
+                      PendingDeprecationWarning, stacklevel=2)
+        return list(self.findall(condition, include_self, descend,
+                                 siblings, ascend))
+
+    def findall(self, condition=None, include_self=True, descend=True,
+                siblings=False, ascend=False):
+        """
+        Return an iterator yielding nodes following `self`:
+
+        * self (if `include_self` is true)
+        * all descendants in tree traversal order (if `descend` is true)
+        * the following siblings (if `siblings` is true) and their
+          descendants (if also `descend` is true)
+        * the following siblings of the parent (if `ascend` is true) and
+          their descendants (if also `descend` is true), and so on.
+
+        If `condition` is not None, the iterator yields only nodes
+        for which ``condition(node)`` is true.  If `condition` is a
+        node class ``cls``, it is equivalent to a function consisting
+        of ``return isinstance(node, cls)``.
+
+        If `ascend` is true, assume `siblings` to be true as well.
+
+        If the tree structure is modified during iteration, the result
+        is undefined.
+
+        For example, given the following tree::
+
+            <paragraph>
+                <emphasis>      <--- emphasis.traverse() and
+                    <strong>    <--- strong.traverse() are called.
+                        Foo
+                    Bar
+                <reference name="Baz" refid="baz">
+                    Baz
+
+        Then tuple(emphasis.traverse()) equals ::
+
+            (<emphasis>, <strong>, <#text: Foo>, <#text: Bar>)
+
+        and list(strong.traverse(ascend=True) equals ::
+
+            [<strong>, <#text: Foo>, <#text: Bar>, <reference>, <#text: Baz>]
+        """
+        if ascend:
+            siblings = True
+        # Check for special argument combinations that allow using an
+        # optimized version of traverse()
+        if include_self and descend and not siblings:
+            if condition is None:
+                yield from self._superfast_findall()
+                return
+            elif isinstance(condition, type):
+                yield from self._fast_findall(condition)
+                return
+        # Check if `condition` is a class (check for TypeType for Python
+        # implementations that use only new-style classes, like PyPy).
+        if isinstance(condition, type):
+            node_class = condition
+
+            def condition(node, node_class=node_class):
+                return isinstance(node, node_class)
+
+        if include_self and (condition is None or condition(self)):
+            yield self
+        if descend and len(self.children):
+            for child in self:
+                yield from child.findall(condition=condition,
+                                         include_self=True, descend=True,
+                                         siblings=False, ascend=False)
+        if siblings or ascend:
+            node = self
+            while node.parent:
+                index = node.parent.index(node)
+                # extra check since Text nodes have value-equality
+                while node.parent[index] is not node:
+                    index = node.parent.index(node, index + 1)
+                for sibling in node.parent[index+1:]:
+                    yield from sibling.findall(
+                        condition=condition,
+                        include_self=True, descend=descend,
+                        siblings=False, ascend=False)
+                if not ascend:
+                    break
+                else:
+                    node = node.parent
 
-    def encode(self, encoding):
-        """When an HTML document is being encoded to a given encoding, the
-        value of a meta tag's 'charset' is the name of the encoding.
+    def next_node(self, condition=None, include_self=False, descend=True,
+                  siblings=False, ascend=False):
         """
-        if encoding in PYTHON_SPECIFIC_ENCODINGS:
-            return ''
-        return encoding
+        Return the first node in the iterator returned by findall(),
+        or None if the iterable is empty.
+
+        Parameter list is the same as of traverse.  Note that `include_self`
+        defaults to False, though.
+        """
+        try:
+            return next(self.findall(condition, include_self,
+                                     descend, siblings, ascend))
+        except StopIteration:
+            return None
 
 
-class ContentMetaAttributeValue(AttributeValueWithCharsetSubstitution):
-    """A generic stand-in for the value of a meta tag's 'content' attribute.
+class reprunicode(str):
+    """
+    Deprecated backwards compatibility stub. Use the standard `str` instead.
+    """
+    def __init__(self, s):
+        warnings.warn('nodes.reprunicode() is not required with Python 3'
+                      ' and will be removed in Docutils 0.21 or later.',
+                      DeprecationWarning, stacklevel=2)
+        super().__init__()
 
-    When Beautiful Soup parses the markup:
-     <meta http-equiv="content-type" content="text/html; charset=utf8">
 
-    The value of the 'content' attribute will be one of these objects.
+def ensure_str(s):
+    """
+    Deprecated backwards compatibility stub returning `s`.
     """
+    warnings.warn('nodes.ensure_str() is not required with Python 3'
+                  ' and will be removed in Docutils 0.21 or later.',
+                  DeprecationWarning, stacklevel=2)
+    return s
 
-    CHARSET_RE = re.compile(r"((^|;)\s*charset=)([^;]*)", re.M)
 
-    def __new__(cls, original_value):
-        match = cls.CHARSET_RE.search(original_value)
-        if match is None:
-            # No substitution necessary.
-            return str.__new__(str, original_value)
+# definition moved here from `utils` to avoid circular import dependency
+def unescape(text, restore_backslashes=False, respect_whitespace=False):
+    """
+    Return a string with nulls removed or restored to backslashes.
+    Backslash-escaped spaces are also removed.
+    """
+    # `respect_whitespace` is ignored (since introduction 2016-12-16)
+    if restore_backslashes:
+        return text.replace('\x00', '\\')
+    else:
+        for sep in ['\x00 ', '\x00\n', '\x00']:
+            text = ''.join(text.split(sep))
+        return text
 
-        obj = str.__new__(cls, original_value)
-        obj.original_value = original_value
-        return obj
 
-    def encode(self, encoding):
-        if encoding in PYTHON_SPECIFIC_ENCODINGS:
+class Text(Node, str):
+
+    """
+    Instances are terminal nodes (leaves) containing text only; no child
+    nodes or attributes.  Initialize by passing a string to the constructor.
+
+    Access the raw (null-escaped) text with ``str(<instance>)``
+    and unescaped text with ``<instance>.astext()``.
+    """
+
+    tagname = '#text'
+
+    children = ()
+    """Text nodes have no children, and cannot have children."""
+
+    def __new__(cls, data, rawsource=None):
+        """Assert that `data` is not an array of bytes
+        and warn if the deprecated `rawsource` argument is used.
+        """
+        if isinstance(data, bytes):
+            raise TypeError('expecting str data, not bytes')
+        if rawsource is not None:
+            warnings.warn('nodes.Text: initialization argument "rawsource" '
+                          'is ignored and will be removed in Docutils 2.0.',
+                          DeprecationWarning, stacklevel=2)
+        return str.__new__(cls, data)
+
+    def shortrepr(self, maxlen=18):
+        data = self
+        if len(data) > maxlen:
+            data = data[:maxlen-4] + ' ...'
+        return '<%s: %r>' % (self.tagname, str(data))
+
+    def __repr__(self):
+        return self.shortrepr(maxlen=68)
+
+    def _dom_node(self, domroot):
+        return domroot.createTextNode(str(self))
+
+    def astext(self):
+        return str(unescape(self))
+
+    def copy(self):
+        return self.__class__(str(self))
+
+    def deepcopy(self):
+        return self.copy()
+
+    def pformat(self, indent='    ', level=0):
+        try:
+            if self.document.settings.detailed:
+                tag = '%s%s' % (indent*level, '<#text>')
+                lines = (indent*(level+1) + repr(line)
+                         for line in self.splitlines(True))
+                return '\n'.join((tag, *lines)) + '\n'
+        except AttributeError:
+            pass
+        indent = indent * level
+        lines = [indent+line for line in self.astext().splitlines()]
+        if not lines:
             return ''
-        def rewrite(match):
-            return match.group(1) + encoding
-        return self.CHARSET_RE.sub(rewrite, self.original_value)
+        return '\n'.join(lines) + '\n'
+
+    # rstrip and lstrip are used by substitution definitions where
+    # they are expected to return a Text instance, this was formerly
+    # taken care of by UserString.
+
+    def rstrip(self, chars=None):
+        return self.__class__(str.rstrip(self, chars))
 
+    def lstrip(self, chars=None):
+        return self.__class__(str.lstrip(self, chars))
 
-class PageElement(object):
-    """Contains the navigational information for some part of the page:
-    that is, its current location in the parse tree.
 
-    NavigableString, Tag, etc. are all subclasses of PageElement.
+class Element(Node):
+
     """
+    `Element` is the superclass to all specific elements.
 
-    # In general, we can't tell just by looking at an element whether
-    # it's contained in an XML document or an HTML document. But for
-    # Tags (q.v.) we can store this information at parse time.
-    known_xml = None
+    Elements contain attributes and child nodes.
+    They can be described as a cross between a list and a dictionary.
 
-    def setup(self, parent=None, previous_element=None, next_element=None,
-              previous_sibling=None, next_sibling=None):
-        """Sets up the initial relations between this element and
-        other elements.
+    Elements emulate dictionaries for external [#]_ attributes, indexing by
+    attribute name (a string). To set the attribute 'att' to 'value', do::
 
-        :param parent: The parent of this element.
+        element['att'] = 'value'
 
-        :param previous_element: The element parsed immediately before
-            this one.
+    .. [#] External attributes correspond to the XML element attributes.
+       From its `Node` superclass, Element also inherits "internal"
+       class attributes that are accessed using the standard syntax, e.g.
+       ``element.parent``.
 
-        :param next_element: The element parsed immediately before
-            this one.
+    There are two special attributes: 'ids' and 'names'.  Both are
+    lists of unique identifiers: 'ids' conform to the regular expression
+    ``[a-z](-?[a-z0-9]+)*`` (see the make_id() function for rationale and
+    details). 'names' serve as user-friendly interfaces to IDs; they are
+    case- and whitespace-normalized (see the fully_normalize_name() function).
 
-        :param previous_sibling: The most recently encountered element
-            on the same level of the parse tree as this one.
+    Elements emulate lists for child nodes (element nodes and/or text
+    nodes), indexing by integer.  To get the first child node, use::
 
-        :param previous_sibling: The next element to be encountered
-            on the same level of the parse tree as this one.
-        """
-        self.parent = parent
+        element[0]
 
-        self.previous_element = previous_element
-        if previous_element is not None:
-            self.previous_element.next_element = self
+    to iterate over the child nodes (without descending), use::
 
-        self.next_element = next_element
-        if self.next_element is not None:
-            self.next_element.previous_element = self
+        for child in element:
+            ...
 
-        self.next_sibling = next_sibling
-        if self.next_sibling is not None:
-            self.next_sibling.previous_sibling = self
+    Elements may be constructed using the ``+=`` operator.  To add one new
+    child node to element, do::
 
-        if (previous_sibling is None
-            and self.parent is not None and self.parent.contents):
-            previous_sibling = self.parent.contents[-1]
+        element += node
 
-        self.previous_sibling = previous_sibling
-        if previous_sibling is not None:
-            self.previous_sibling.next_sibling = self
+    This is equivalent to ``element.append(node)``.
 
-    def format_string(self, s, formatter):
-        """Format the given string using the given formatter.
+    To add a list of multiple child nodes at once, use the same ``+=``
+    operator::
 
-        :param s: A string.
-        :param formatter: A Formatter object, or a string naming one of the standard formatters.
-        """
-        if formatter is None:
-            return s
-        if not isinstance(formatter, Formatter):
-            formatter = self.formatter_for_name(formatter)
-        output = formatter.substitute(s)
-        return output
+        element += [node1, node2]
 
-    def formatter_for_name(self, formatter):
-        """Look up or create a Formatter for the given identifier,
-        if necessary.
+    This is equivalent to ``element.extend([node1, node2])``.
+    """
 
-        :param formatter: Can be a Formatter object (used as-is), a
-            function (used as the entity substitution hook for an
-            XMLFormatter or HTMLFormatter), or a string (used to look
-            up an XMLFormatter or HTMLFormatter in the appropriate
-            registry.
-        """
-        if isinstance(formatter, Formatter):
-            return formatter
-        if self._is_xml:
-            c = XMLFormatter
-        else:
-            c = HTMLFormatter
-        if isinstance(formatter, Callable):
-            return c(entity_substitution=formatter)
-        return c.REGISTRY[formatter]
+    basic_attributes = ('ids', 'classes', 'names', 'dupnames')
+    """Tuple of attributes which are defined for every Element-derived class
+    instance and can be safely transferred to a different node."""
 
-    @property
-    def _is_xml(self):
-        """Is this element part of an XML tree or an HTML tree?
+    local_attributes = ('backrefs',)
+    """Tuple of class-specific attributes that should not be copied with the
+    standard attributes when replacing a node.
 
-        This is used in formatter_for_name, when deciding whether an
-        XMLFormatter or HTMLFormatter is more appropriate. It can be
-        inefficient, but it should be called very rarely.
-        """
-        if self.known_xml is not None:
-            # Most of the time we will have determined this when the
-            # document is parsed.
-            return self.known_xml
-
-        # Otherwise, it's likely that this element was created by
-        # direct invocation of the constructor from within the user's
-        # Python code.
-        if self.parent is None:
-            # This is the top-level object. It should have .known_xml set
-            # from tree creation. If not, take a guess--BS is usually
-            # used on HTML markup.
-            return getattr(self, 'is_xml', False)
-        return self.parent._is_xml
-
-    nextSibling = _alias("next_sibling")  # BS3
-    previousSibling = _alias("previous_sibling")  # BS3
-
-    default = object()
-    def _all_strings(self, strip=False, types=default):
-        """Yield all strings of certain classes, possibly stripping them.
+    NOTE: Derived classes should override this value to prevent any of its
+    attributes being copied by adding to the value in its parent class."""
 
-        This is implemented differently in Tag and NavigableString.
-        """
-        raise NotImplementedError()
+    list_attributes = basic_attributes + local_attributes
+    """Tuple of attributes that are automatically initialized to empty lists
+    for all nodes."""
 
-    @property
-    def stripped_strings(self):
-        """Yield all strings in this PageElement, stripping them first.
+    known_attributes = list_attributes + ('source',)
+    """Tuple of attributes that are known to the Element base class."""
 
-        :yield: A sequence of stripped strings.
-        """
-        for string in self._all_strings(True):
-            yield string
+    tagname = None
+    """The element generic identifier. If None, it is set as an instance
+    attribute to the name of the class."""
 
-    def get_text(self, separator="", strip=False,
-                 types=default):
-        """Get all child strings of this PageElement, concatenated using the
-        given separator.
-
-        :param separator: Strings will be concatenated using this separator.
-
-        :param strip: If True, strings will be stripped before being
-            concatenated.
-
-        :param types: A tuple of NavigableString subclasses. Any
-            strings of a subclass not found in this list will be
-            ignored. Although there are exceptions, the default
-            behavior in most cases is to consider only NavigableString
-            and CData objects. That means no comments, processing
-            instructions, etc.
-
-        :return: A string.
-        """
-        return separator.join([s for s in self._all_strings(
-                    strip, types=types)])
-    getText = get_text
-    text = property(get_text)
-
-    def replace_with(self, *args):
-        """Replace this PageElement with one or more PageElements, keeping the
-        rest of the tree the same.
-
-        :param args: One or more PageElements.
-        :return: `self`, no longer part of the tree.
-        """
-        if self.parent is None:
-            raise ValueError(
-                "Cannot replace one element with another when the "
-                "element to be replaced is not part of a tree.")
-        if len(args) == 1 and args[0] is self:
-            return
-        if any(x is self.parent for x in args):
-            raise ValueError("Cannot replace a Tag with its parent.")
-        old_parent = self.parent
-        my_index = self.parent.index(self)
-        self.extract(_self_index=my_index)
-        for idx, replace_with in enumerate(args, start=my_index):
-            old_parent.insert(idx, replace_with)
-        return self
-    replaceWith = replace_with  # BS3
+    child_text_separator = '\n\n'
+    """Separator for child nodes, used by `astext()` method."""
 
-    def unwrap(self):
-        """Replace this PageElement with its contents.
+    def __init__(self, rawsource='', *children, **attributes):
+        self.rawsource = rawsource
+        """The raw text from which this element was constructed.
 
-        :return: `self`, no longer part of the tree.
+        NOTE: some elements do not set this value (default '').
         """
-        my_parent = self.parent
-        if self.parent is None:
-            raise ValueError(
-                "Cannot replace an element with its contents when that"
-                "element is not part of a tree.")
-        my_index = self.parent.index(self)
-        self.extract(_self_index=my_index)
-        for child in reversed(self.contents[:]):
-            my_parent.insert(my_index, child)
-        return self
-    replace_with_children = unwrap
-    replaceWithChildren = unwrap  # BS3
 
-    def wrap(self, wrap_inside):
-        """Wrap this PageElement inside another one.
+        self.children = []
+        """List of child nodes (elements and/or `Text`)."""
 
-        :param wrap_inside: A PageElement.
-        :return: `wrap_inside`, occupying the position in the tree that used
-           to be occupied by `self`, and with `self` inside it.
-        """
-        me = self.replace_with(wrap_inside)
-        wrap_inside.append(me)
-        return wrap_inside
-
-    def extract(self, _self_index=None):
-        """Destructively rips this element out of the tree.
-
-        :param _self_index: The location of this element in its parent's
-           .contents, if known. Passing this in allows for a performance
-           optimization.
-
-        :return: `self`, no longer part of the tree.
-        """
-        if self.parent is not None:
-            if _self_index is None:
-                _self_index = self.parent.index(self)
-            del self.parent.contents[_self_index]
-
-        #Find the two elements that would be next to each other if
-        #this element (and any children) hadn't been parsed. Connect
-        #the two.
-        last_child = self._last_descendant()
-        next_element = last_child.next_element
-
-        if (self.previous_element is not None and
-            self.previous_element is not next_element):
-            self.previous_element.next_element = next_element
-        if next_element is not None and next_element is not self.previous_element:
-            next_element.previous_element = self.previous_element
-        self.previous_element = None
-        last_child.next_element = None
-
-        self.parent = None
-        if (self.previous_sibling is not None
-            and self.previous_sibling is not self.next_sibling):
-            self.previous_sibling.next_sibling = self.next_sibling
-        if (self.next_sibling is not None
-            and self.next_sibling is not self.previous_sibling):
-            self.next_sibling.previous_sibling = self.previous_sibling
-        self.previous_sibling = self.next_sibling = None
-        return self
+        self.extend(children)           # maintain parent info
 
-    def _last_descendant(self, is_initialized=True, accept_self=True):
-        """Finds the last element beneath this object to be parsed.
+        self.attributes = {}
+        """Dictionary of attribute {name: value}."""
 
-        :param is_initialized: Has `setup` been called on this PageElement
-            yet?
-        :param accept_self: Is `self` an acceptable answer to the question?
-        """
-        if is_initialized and self.next_sibling is not None:
-            last_child = self.next_sibling.previous_element
+        # Initialize list attributes.
+        for att in self.list_attributes:
+            self.attributes[att] = []
+
+        for att, value in attributes.items():
+            att = att.lower()
+            if att in self.list_attributes:
+                # mutable list; make a copy for this node
+                self.attributes[att] = value[:]
+            else:
+                self.attributes[att] = value
+
+        if self.tagname is None:
+            self.tagname = self.__class__.__name__
+
+    def _dom_node(self, domroot):
+        element = domroot.createElement(self.tagname)
+        for attribute, value in self.attlist():
+            if isinstance(value, list):
+                value = ' '.join(serial_escape('%s' % (v,)) for v in value)
+            element.setAttribute(attribute, '%s' % value)
+        for child in self.children:
+            element.appendChild(child._dom_node(domroot))
+        return element
+
+    def __repr__(self):
+        data = ''
+        for c in self.children:
+            data += c.shortrepr()
+            if len(data) > 60:
+                data = data[:56] + ' ...'
+                break
+        if self['names']:
+            return '<%s "%s": %s>' % (self.__class__.__name__,
+                                      '; '.join(self['names']), data)
         else:
-            last_child = self
-            while isinstance(last_child, Tag) and last_child.contents:
-                last_child = last_child.contents[-1]
-        if not accept_self and last_child is self:
-            last_child = None
-        return last_child
-    # BS3: Not part of the API!
-    _lastRecursiveChild = _last_descendant
-
-    def insert(self, position, new_child):
-        """Insert a new PageElement in the list of this PageElement's children.
-
-        This works the same way as `list.insert`.
-
-        :param position: The numeric position that should be occupied
-           in `self.children` by the new PageElement.
-        :param new_child: A PageElement.
-        """
-        if new_child is None:
-            raise ValueError("Cannot insert None into a tag.")
-        if new_child is self:
-            raise ValueError("Cannot insert a tag into itself.")
-        if (isinstance(new_child, str)
-            and not isinstance(new_child, NavigableString)):
-            new_child = NavigableString(new_child)
-
-        from bs4 import BeautifulSoup
-        if isinstance(new_child, BeautifulSoup):
-            # We don't want to end up with a situation where one BeautifulSoup
-            # object contains another. Insert the children one at a time.
-            for subchild in list(new_child.contents):
-                self.insert(position, subchild)
-                position += 1
-            return
-        position = min(position, len(self.contents))
-        if hasattr(new_child, 'parent') and new_child.parent is not None:
-            # We're 'inserting' an element that's already one
-            # of this object's children.
-            if new_child.parent is self:
-                current_index = self.index(new_child)
-                if current_index < position:
-                    # We're moving this element further down the list
-                    # of this object's children. That means that when
-                    # we extract this element, our target index will
-                    # jump down one.
-                    position -= 1
-            new_child.extract()
-
-        new_child.parent = self
-        previous_child = None
-        if position == 0:
-            new_child.previous_sibling = None
-            new_child.previous_element = self
+            return '<%s: %s>' % (self.__class__.__name__, data)
+
+    def shortrepr(self):
+        if self['names']:
+            return '<%s "%s"...>' % (self.__class__.__name__,
+                                     '; '.join(self['names']))
         else:
-            previous_child = self.contents[position - 1]
-            new_child.previous_sibling = previous_child
-            new_child.previous_sibling.next_sibling = new_child
-            new_child.previous_element = previous_child._last_descendant(False)
-        if new_child.previous_element is not None:
-            new_child.previous_element.next_element = new_child
-
-        new_childs_last_element = new_child._last_descendant(False)
-
-        if position >= len(self.contents):
-            new_child.next_sibling = None
-
-            parent = self
-            parents_next_sibling = None
-            while parents_next_sibling is None and parent is not None:
-                parents_next_sibling = parent.next_sibling
-                parent = parent.parent
-                if parents_next_sibling is not None:
-                    # We found the element that comes next in the document.
-                    break
-            if parents_next_sibling is not None:
-                new_childs_last_element.next_element = parents_next_sibling
+            return '<%s...>' % self.tagname
+
+    def __str__(self):
+        if self.children:
+            return '%s%s%s' % (self.starttag(),
+                               ''.join(str(c) for c in self.children),
+                               self.endtag())
+        else:
+            return self.emptytag()
+
+    def starttag(self, quoteattr=None):
+        # the optional arg is used by the docutils_xml writer
+        if quoteattr is None:
+            quoteattr = pseudo_quoteattr
+        parts = [self.tagname]
+        for name, value in self.attlist():
+            if value is None:           # boolean attribute
+                parts.append('%s="True"' % name)
+                continue
+            if isinstance(value, list):
+                values = [serial_escape('%s' % (v,)) for v in value]
+                value = ' '.join(values)
             else:
-                # The last element of this tag is the last element in
-                # the document.
-                new_childs_last_element.next_element = None
+                value = str(value)
+            value = quoteattr(value)
+            parts.append('%s=%s' % (name, value))
+        return '<%s>' % ' '.join(parts)
+
+    def endtag(self):
+        return '</%s>' % self.tagname
+
+    def emptytag(self):
+        attributes = ('%s="%s"' % (n, v) for n, v in self.attlist())
+        return '<%s/>' % ' '.join((self.tagname, *attributes))
+
+    def __len__(self):
+        return len(self.children)
+
+    def __contains__(self, key):
+        # Test for both, children and attributes with operator ``in``.
+        if isinstance(key, str):
+            return key in self.attributes
+        return key in self.children
+
+    def __getitem__(self, key):
+        if isinstance(key, str):
+            return self.attributes[key]
+        elif isinstance(key, int):
+            return self.children[key]
+        elif isinstance(key, slice):
+            assert key.step in (None, 1), 'cannot handle slice with stride'
+            return self.children[key.start:key.stop]
         else:
-            next_child = self.contents[position]
-            new_child.next_sibling = next_child
-            if new_child.next_sibling is not None:
-                new_child.next_sibling.previous_sibling = new_child
-            new_childs_last_element.next_element = next_child
-
-        if new_childs_last_element.next_element is not None:
-            new_childs_last_element.next_element.previous_element = new_childs_last_element
-        self.contents.insert(position, new_child)
-
-    def append(self, tag):
-        """Appends the given PageElement to the contents of this one.
-
-        :param tag: A PageElement.
-        """
-        self.insert(len(self.contents), tag)
-
-    def extend(self, tags):
-        """Appends the given PageElements to this one's contents.
-
-        :param tags: A list of PageElements. If a single Tag is
-            provided instead, this PageElement's contents will be extended
-            with that Tag's contents.
-        """
-        if isinstance(tags, Tag):
-            tags = tags.contents
-        if isinstance(tags, list):
-            # Moving items around the tree may change their position in
-            # the original list. Make a list that won't change.
-            tags = list(tags)
-        for tag in tags:
-            self.append(tag)
-
-    def insert_before(self, *args):
-        """Makes the given element(s) the immediate predecessor of this one.
-
-        All the elements will have the same parent, and the given elements
-        will be immediately before this one.
-
-        :param args: One or more PageElements.
-        """
-        parent = self.parent
-        if parent is None:
-            raise ValueError(
-                "Element has no parent, so 'before' has no meaning.")
-        if any(x is self for x in args):
-                raise ValueError("Can't insert an element before itself.")
-        for predecessor in args:
-            # Extract first so that the index won't be screwed up if they
-            # are siblings.
-            if isinstance(predecessor, PageElement):
-                predecessor.extract()
-            index = parent.index(self)
-            parent.insert(index, predecessor)
-
-    def insert_after(self, *args):
-        """Makes the given element(s) the immediate successor of this one.
-
-        The elements will have the same parent, and the given elements
-        will be immediately after this one.
-
-        :param args: One or more PageElements.
-        """
-        # Do all error checking before modifying the tree.
-        parent = self.parent
-        if parent is None:
-            raise ValueError(
-                "Element has no parent, so 'after' has no meaning.")
-        if any(x is self for x in args):
-            raise ValueError("Can't insert an element after itself.")
-
-        offset = 0
-        for successor in args:
-            # Extract first so that the index won't be screwed up if they
-            # are siblings.
-            if isinstance(successor, PageElement):
-                successor.extract()
-            index = parent.index(self)
-            parent.insert(index+1+offset, successor)
-            offset += 1
-
-    def find_next(self, name=None, attrs={}, string=None, **kwargs):
-        """Find the first PageElement that matches the given criteria and
-        appears later in the document than this PageElement.
-
-        All find_* methods take a common set of arguments. See the online
-        documentation for detailed explanations.
-
-        :param name: A filter on tag name.
-        :param attrs: A dictionary of filters on attribute values.
-        :param string: A filter for a NavigableString with specific text.
-        :kwargs: A dictionary of filters on attribute values.
-        :return: A PageElement.
-        :rtype: bs4.element.Tag | bs4.element.NavigableString
-        """
-        return self._find_one(self.find_all_next, name, attrs, string, **kwargs)
-    findNext = find_next  # BS3
-
-    def find_all_next(self, name=None, attrs={}, string=None, limit=None,
-                    **kwargs):
-        """Find all PageElements that match the given criteria and appear
-        later in the document than this PageElement.
-
-        All find_* methods take a common set of arguments. See the online
-        documentation for detailed explanations.
-
-        :param name: A filter on tag name.
-        :param attrs: A dictionary of filters on attribute values.
-        :param string: A filter for a NavigableString with specific text.
-        :param limit: Stop looking after finding this many results.
-        :kwargs: A dictionary of filters on attribute values.
-        :return: A ResultSet containing PageElements.
-        """
-        _stacklevel = kwargs.pop('_stacklevel', 2)
-        return self._find_all(name, attrs, string, limit, self.next_elements,
-                              _stacklevel=_stacklevel+1, **kwargs)
-    findAllNext = find_all_next  # BS3
-
-    def find_next_sibling(self, name=None, attrs={}, string=None, **kwargs):
-        """Find the closest sibling to this PageElement that matches the
-        given criteria and appears later in the document.
-
-        All find_* methods take a common set of arguments. See the
-        online documentation for detailed explanations.
-
-        :param name: A filter on tag name.
-        :param attrs: A dictionary of filters on attribute values.
-        :param string: A filter for a NavigableString with specific text.
-        :kwargs: A dictionary of filters on attribute values.
-        :return: A PageElement.
-        :rtype: bs4.element.Tag | bs4.element.NavigableString
-        """
-        return self._find_one(self.find_next_siblings, name, attrs, string,
-                             **kwargs)
-    findNextSibling = find_next_sibling  # BS3
-
-    def find_next_siblings(self, name=None, attrs={}, string=None, limit=None,
-                           **kwargs):
-        """Find all siblings of this PageElement that match the given criteria
-        and appear later in the document.
-
-        All find_* methods take a common set of arguments. See the online
-        documentation for detailed explanations.
-
-        :param name: A filter on tag name.
-        :param attrs: A dictionary of filters on attribute values.
-        :param string: A filter for a NavigableString with specific text.
-        :param limit: Stop looking after finding this many results.
-        :kwargs: A dictionary of filters on attribute values.
-        :return: A ResultSet of PageElements.
-        :rtype: bs4.element.ResultSet
-        """
-        _stacklevel = kwargs.pop('_stacklevel', 2)
-        return self._find_all(
-            name, attrs, string, limit,
-            self.next_siblings, _stacklevel=_stacklevel+1, **kwargs
-        )
-    findNextSiblings = find_next_siblings   # BS3
-    fetchNextSiblings = find_next_siblings  # BS2
-
-    def find_previous(self, name=None, attrs={}, string=None, **kwargs):
-        """Look backwards in the document from this PageElement and find the
-        first PageElement that matches the given criteria.
-
-        All find_* methods take a common set of arguments. See the online
-        documentation for detailed explanations.
-
-        :param name: A filter on tag name.
-        :param attrs: A dictionary of filters on attribute values.
-        :param string: A filter for a NavigableString with specific text.
-        :kwargs: A dictionary of filters on attribute values.
-        :return: A PageElement.
-        :rtype: bs4.element.Tag | bs4.element.NavigableString
-        """
-        return self._find_one(
-            self.find_all_previous, name, attrs, string, **kwargs)
-    findPrevious = find_previous  # BS3
-
-    def find_all_previous(self, name=None, attrs={}, string=None, limit=None,
-                        **kwargs):
-        """Look backwards in the document from this PageElement and find all
-        PageElements that match the given criteria.
-
-        All find_* methods take a common set of arguments. See the online
-        documentation for detailed explanations.
-
-        :param name: A filter on tag name.
-        :param attrs: A dictionary of filters on attribute values.
-        :param string: A filter for a NavigableString with specific text.
-        :param limit: Stop looking after finding this many results.
-        :kwargs: A dictionary of filters on attribute values.
-        :return: A ResultSet of PageElements.
-        :rtype: bs4.element.ResultSet
-        """
-        _stacklevel = kwargs.pop('_stacklevel', 2)
-        return self._find_all(
-            name, attrs, string, limit, self.previous_elements,
-            _stacklevel=_stacklevel+1, **kwargs
-        )
-    findAllPrevious = find_all_previous  # BS3
-    fetchPrevious = find_all_previous    # BS2
-
-    def find_previous_sibling(self, name=None, attrs={}, string=None, **kwargs):
-        """Returns the closest sibling to this PageElement that matches the
-        given criteria and appears earlier in the document.
-
-        All find_* methods take a common set of arguments. See the online
-        documentation for detailed explanations.
-
-        :param name: A filter on tag name.
-        :param attrs: A dictionary of filters on attribute values.
-        :param string: A filter for a NavigableString with specific text.
-        :kwargs: A dictionary of filters on attribute values.
-        :return: A PageElement.
-        :rtype: bs4.element.Tag | bs4.element.NavigableString
-        """
-        return self._find_one(self.find_previous_siblings, name, attrs, string,
-                             **kwargs)
-    findPreviousSibling = find_previous_sibling  # BS3
-
-    def find_previous_siblings(self, name=None, attrs={}, string=None,
-                               limit=None, **kwargs):
-        """Returns all siblings to this PageElement that match the
-        given criteria and appear earlier in the document.
-
-        All find_* methods take a common set of arguments. See the online
-        documentation for detailed explanations.
-
-        :param name: A filter on tag name.
-        :param attrs: A dictionary of filters on attribute values.
-        :param string: A filter for a NavigableString with specific text.
-        :param limit: Stop looking after finding this many results.
-        :kwargs: A dictionary of filters on attribute values.
-        :return: A ResultSet of PageElements.
-        :rtype: bs4.element.ResultSet
-        """
-        _stacklevel = kwargs.pop('_stacklevel', 2)
-        return self._find_all(
-            name, attrs, string, limit,
-            self.previous_siblings, _stacklevel=_stacklevel+1, **kwargs
-        )
-    findPreviousSiblings = find_previous_siblings   # BS3
-    fetchPreviousSiblings = find_previous_siblings  # BS2
-
-    def find_parent(self, name=None, attrs={}, **kwargs):
-        """Find the closest parent of this PageElement that matches the given
-        criteria.
-
-        All find_* methods take a common set of arguments. See the online
-        documentation for detailed explanations.
-
-        :param name: A filter on tag name.
-        :param attrs: A dictionary of filters on attribute values.
-        :kwargs: A dictionary of filters on attribute values.
-
-        :return: A PageElement.
-        :rtype: bs4.element.Tag | bs4.element.NavigableString
-        """
-        # NOTE: We can't use _find_one because findParents takes a different
-        # set of arguments.
-        r = None
-        l = self.find_parents(name, attrs, 1, _stacklevel=3, **kwargs)
-        if l:
-            r = l[0]
-        return r
-    findParent = find_parent  # BS3
-
-    def find_parents(self, name=None, attrs={}, limit=None, **kwargs):
-        """Find all parents of this PageElement that match the given criteria.
-
-        All find_* methods take a common set of arguments. See the online
-        documentation for detailed explanations.
-
-        :param name: A filter on tag name.
-        :param attrs: A dictionary of filters on attribute values.
-        :param limit: Stop looking after finding this many results.
-        :kwargs: A dictionary of filters on attribute values.
-
-        :return: A PageElement.
-        :rtype: bs4.element.Tag | bs4.element.NavigableString
-        """
-        _stacklevel = kwargs.pop('_stacklevel', 2)
-        return self._find_all(name, attrs, None, limit, self.parents,
-                              _stacklevel=_stacklevel+1, **kwargs)
-    findParents = find_parents   # BS3
-    fetchParents = find_parents  # BS2
+            raise TypeError('element index must be an integer, a slice, or '
+                            'an attribute name string')
 
-    @property
-    def next(self):
-        """The PageElement, if any, that was parsed just after this one.
+    def __setitem__(self, key, item):
+        if isinstance(key, str):
+            self.attributes[str(key)] = item
+        elif isinstance(key, int):
+            self.setup_child(item)
+            self.children[key] = item
+        elif isinstance(key, slice):
+            assert key.step in (None, 1), 'cannot handle slice with stride'
+            for node in item:
+                self.setup_child(node)
+            self.children[key.start:key.stop] = item
+        else:
+            raise TypeError('element index must be an integer, a slice, or '
+                            'an attribute name string')
 
-        :return: A PageElement.
-        :rtype: bs4.element.Tag | bs4.element.NavigableString
-        """
-        return self.next_element
+    def __delitem__(self, key):
+        if isinstance(key, str):
+            del self.attributes[key]
+        elif isinstance(key, int):
+            del self.children[key]
+        elif isinstance(key, slice):
+            assert key.step in (None, 1), 'cannot handle slice with stride'
+            del self.children[key.start:key.stop]
+        else:
+            raise TypeError('element index must be an integer, a simple '
+                            'slice, or an attribute name string')
 
-    @property
-    def previous(self):
-        """The PageElement, if any, that was parsed just before this one.
+    def __add__(self, other):
+        return self.children + other
 
-        :return: A PageElement.
-        :rtype: bs4.element.Tag | bs4.element.NavigableString
-        """
-        return self.previous_element
+    def __radd__(self, other):
+        return other + self.children
+
+    def __iadd__(self, other):
+        """Append a node or a list of nodes to `self.children`."""
+        if isinstance(other, Node):
+            self.append(other)
+        elif other is not None:
+            self.extend(other)
+        return self
 
-    #These methods do the real heavy lifting.
-
-    def _find_one(self, method, name, attrs, string, **kwargs):
-        r = None
-        l = method(name, attrs, string, 1, _stacklevel=4, **kwargs)
-        if l:
-            r = l[0]
-        return r
-
-    def _find_all(self, name, attrs, string, limit, generator, **kwargs):
-        "Iterates over a generator looking for things that match."
-        _stacklevel = kwargs.pop('_stacklevel', 3)
-
-        if string is None and 'text' in kwargs:
-            string = kwargs.pop('text')
-            warnings.warn(
-                "The 'text' argument to find()-type methods is deprecated. Use 'string' instead.",
-                DeprecationWarning, stacklevel=_stacklevel
-            )
+    def astext(self):
+        return self.child_text_separator.join(
+                   [child.astext() for child in self.children])
+
+    def non_default_attributes(self):
+        atts = {}
+        for key, value in self.attributes.items():
+            if self.is_not_default(key):
+                atts[key] = value
+        return atts
+
+    def attlist(self):
+        return sorted(self.non_default_attributes().items())
+
+    def get(self, key, failobj=None):
+        return self.attributes.get(key, failobj)
+
+    def hasattr(self, attr):
+        return attr in self.attributes
+
+    def delattr(self, attr):
+        if attr in self.attributes:
+            del self.attributes[attr]
+
+    def setdefault(self, key, failobj=None):
+        return self.attributes.setdefault(key, failobj)
+
+    has_key = hasattr
+
+    def get_language_code(self, fallback=''):
+        """Return node's language tag.
+
+        Look iteratively in self and parents for a class argument
+        starting with ``language-`` and return the remainder of it
+        (which should be a `BCP49` language tag) or the `fallback`.
+        """
+        for cls in self.get('classes', []):
+            if cls.startswith('language-'):
+                return cls[9:]
+        try:
+            return self.parent.get_language(fallback)
+        except AttributeError:
+            return fallback
+
+    def append(self, item):
+        self.setup_child(item)
+        self.children.append(item)
+
+    def extend(self, item):
+        for node in item:
+            self.append(node)
+
+    def insert(self, index, item):
+        if isinstance(item, Node):
+            self.setup_child(item)
+            self.children.insert(index, item)
+        elif item is not None:
+            self[index:index] = item
+
+    def pop(self, i=-1):
+        return self.children.pop(i)
+
+    def remove(self, item):
+        self.children.remove(item)
+
+    def index(self, item, start=0, stop=sys.maxsize):
+        return self.children.index(item, start, stop)
+
+    def previous_sibling(self):
+        """Return preceding sibling node or ``None``."""
+        try:
+            i = self.parent.index(self)
+        except (AttributeError):
+            return None
+        return self.parent[i-1] if i > 0 else None
 
-        if isinstance(name, SoupStrainer):
-            strainer = name
+    def is_not_default(self, key):
+        if self[key] == [] and key in self.list_attributes:
+            return 0
         else:
-            strainer = SoupStrainer(name, attrs, string, **kwargs)
+            return 1
 
-        if string is None and not limit and not attrs and not kwargs:
-            if name is True or name is None:
-                # Optimization to find all tags.
-                result = (element for element in generator
-                          if isinstance(element, Tag))
-                return ResultSet(strainer, result)
-            elif isinstance(name, str):
-                # Optimization to find all tags with a given name.
-                if name.count(':') == 1:
-                    # This is a name with a prefix. If this is a namespace-aware document,
-                    # we need to match the local name against tag.name. If not,
-                    # we need to match the fully-qualified name against tag.name.
-                    prefix, local_name = name.split(':', 1)
-                else:
-                    prefix = None
-                    local_name = name
-                result = (element for element in generator
-                          if isinstance(element, Tag)
-                          and (
-                              element.name == name
-                          ) or (
-                              element.name == local_name
-                              and (prefix is None or element.prefix == prefix)
-                          )
-                )
-                return ResultSet(strainer, result)
-        results = ResultSet(strainer)
-        while True:
-            try:
-                i = next(generator)
-            except StopIteration:
-                break
-            if i:
-                found = strainer.search(i)
-                if found:
-                    results.append(found)
-                    if limit and len(results) >= limit:
-                        break
-        return results
+    def update_basic_atts(self, dict_):
+        """
+        Update basic attributes ('ids', 'names', 'classes',
+        'dupnames', but not 'source') from node or dictionary `dict_`.
+        """
+        if isinstance(dict_, Node):
+            dict_ = dict_.attributes
+        for att in self.basic_attributes:
+            self.append_attr_list(att, dict_.get(att, []))
 
-    #These generators can be used to navigate starting from both
-    #NavigableStrings and Tags.
-    @property
-    def next_elements(self):
-        """All PageElements that were parsed after this one.
+    def append_attr_list(self, attr, values):
+        """
+        For each element in values, if it does not exist in self[attr], append
+        it.
 
-        :yield: A sequence of PageElements.
+        NOTE: Requires self[attr] and values to be sequence type and the
+        former should specifically be a list.
         """
-        i = self.next_element
-        while i is not None:
-            yield i
-            i = i.next_element
+        # List Concatenation
+        for value in values:
+            if value not in self[attr]:
+                self[attr].append(value)
 
-    @property
-    def next_siblings(self):
-        """All PageElements that are siblings of this one but were parsed
-        later.
-
-        :yield: A sequence of PageElements.
-        """
-        i = self.next_sibling
-        while i is not None:
-            yield i
-            i = i.next_sibling
+    def coerce_append_attr_list(self, attr, value):
+        """
+        First, convert both self[attr] and value to a non-string sequence
+        type; if either is not already a sequence, convert it to a list of one
+        element.  Then call append_attr_list.
 
-    @property
-    def previous_elements(self):
-        """All PageElements that were parsed before this one.
+        NOTE: self[attr] and value both must not be None.
+        """
+        # List Concatenation
+        if not isinstance(self.get(attr), list):
+            self[attr] = [self[attr]]
+        if not isinstance(value, list):
+            value = [value]
+        self.append_attr_list(attr, value)
 
-        :yield: A sequence of PageElements.
+    def replace_attr(self, attr, value, force=True):
         """
-        i = self.previous_element
-        while i is not None:
-            yield i
-            i = i.previous_element
+        If self[attr] does not exist or force is True or omitted, set
+        self[attr] to value, otherwise do nothing.
+        """
+        # One or the other
+        if force or self.get(attr) is None:
+            self[attr] = value
 
-    @property
-    def previous_siblings(self):
-        """All PageElements that are siblings of this one but were parsed
-        earlier.
-
-        :yield: A sequence of PageElements.
-        """
-        i = self.previous_sibling
-        while i is not None:
-            yield i
-            i = i.previous_sibling
+    def copy_attr_convert(self, attr, value, replace=True):
+        """
+        If attr is an attribute of self, set self[attr] to
+        [self[attr], value], otherwise set self[attr] to value.
 
-    @property
-    def parents(self):
-        """All PageElements that are parents of this PageElement.
+        NOTE: replace is not used by this function and is kept only for
+              compatibility with the other copy functions.
+        """
+        if self.get(attr) is not value:
+            self.coerce_append_attr_list(attr, value)
 
-        :yield: A sequence of PageElements.
+    def copy_attr_coerce(self, attr, value, replace):
+        """
+        If attr is an attribute of self and either self[attr] or value is a
+        list, convert all non-sequence values to a sequence of 1 element and
+        then concatenate the two sequence, setting the result to self[attr].
+        If both self[attr] and value are non-sequences and replace is True or
+        self[attr] is None, replace self[attr] with value. Otherwise, do
+        nothing.
         """
-        i = self.parent
-        while i is not None:
-            yield i
-            i = i.parent
+        if self.get(attr) is not value:
+            if isinstance(self.get(attr), list) or \
+               isinstance(value, list):
+                self.coerce_append_attr_list(attr, value)
+            else:
+                self.replace_attr(attr, value, replace)
 
-    @property
-    def decomposed(self):
-        """Check whether a PageElement has been decomposed.
+    def copy_attr_concatenate(self, attr, value, replace):
+        """
+        If attr is an attribute of self and both self[attr] and value are
+        lists, concatenate the two sequences, setting the result to
+        self[attr].  If either self[attr] or value are non-sequences and
+        replace is True or self[attr] is None, replace self[attr] with value.
+        Otherwise, do nothing.
+        """
+        if self.get(attr) is not value:
+            if isinstance(self.get(attr), list) and \
+               isinstance(value, list):
+                self.append_attr_list(attr, value)
+            else:
+                self.replace_attr(attr, value, replace)
 
-        :rtype: bool
+    def copy_attr_consistent(self, attr, value, replace):
+        """
+        If replace is True or self[attr] is None, replace self[attr] with
+        value.  Otherwise, do nothing.
         """
-        return getattr(self, '_decomposed', False) or False
-   
-    # Old non-property versions of the generators, for backwards
-    # compatibility with BS3.
-    def nextGenerator(self):
-        return self.next_elements
+        if self.get(attr) is not value:
+            self.replace_attr(attr, value, replace)
+
+    def update_all_atts(self, dict_, update_fun=copy_attr_consistent,
+                        replace=True, and_source=False):
+        """
+        Updates all attributes from node or dictionary `dict_`.
+
+        Appends the basic attributes ('ids', 'names', 'classes',
+        'dupnames', but not 'source') and then, for all other attributes in
+        dict_, updates the same attribute in self.  When attributes with the
+        same identifier appear in both self and dict_, the two values are
+        merged based on the value of update_fun.  Generally, when replace is
+        True, the values in self are replaced or merged with the values in
+        dict_; otherwise, the values in self may be preserved or merged.  When
+        and_source is True, the 'source' attribute is included in the copy.
+
+        NOTE: When replace is False, and self contains a 'source' attribute,
+              'source' is not replaced even when dict_ has a 'source'
+              attribute, though it may still be merged into a list depending
+              on the value of update_fun.
+        NOTE: It is easier to call the update-specific methods then to pass
+              the update_fun method to this function.
+        """
+        if isinstance(dict_, Node):
+            dict_ = dict_.attributes
+
+        # Include the source attribute when copying?
+        if and_source:
+            filter_fun = self.is_not_list_attribute
+        else:
+            filter_fun = self.is_not_known_attribute
 
-    def nextSiblingGenerator(self):
-        return self.next_siblings
+        # Copy the basic attributes
+        self.update_basic_atts(dict_)
 
-    def previousGenerator(self):
-        return self.previous_elements
+        # Grab other attributes in dict_ not in self except the
+        # (All basic attributes should be copied already)
+        for att in filter(filter_fun, dict_):
+            update_fun(self, att, dict_[att], replace)
+
+    def update_all_atts_consistantly(self, dict_, replace=True,
+                                     and_source=False):
+        """
+        Updates all attributes from node or dictionary `dict_`.
+
+        Appends the basic attributes ('ids', 'names', 'classes',
+        'dupnames', but not 'source') and then, for all other attributes in
+        dict_, updates the same attribute in self.  When attributes with the
+        same identifier appear in both self and dict_ and replace is True, the
+        values in self are replaced with the values in dict_; otherwise, the
+        values in self are preserved.  When and_source is True, the 'source'
+        attribute is included in the copy.
+
+        NOTE: When replace is False, and self contains a 'source' attribute,
+              'source' is not replaced even when dict_ has a 'source'
+              attribute, though it may still be merged into a list depending
+              on the value of update_fun.
+        """
+        self.update_all_atts(dict_, Element.copy_attr_consistent, replace,
+                             and_source)
+
+    def update_all_atts_concatenating(self, dict_, replace=True,
+                                      and_source=False):
+        """
+        Updates all attributes from node or dictionary `dict_`.
+
+        Appends the basic attributes ('ids', 'names', 'classes',
+        'dupnames', but not 'source') and then, for all other attributes in
+        dict_, updates the same attribute in self.  When attributes with the
+        same identifier appear in both self and dict_ whose values aren't each
+        lists and replace is True, the values in self are replaced with the
+        values in dict_; if the values from self and dict_ for the given
+        identifier are both of list type, then the two lists are concatenated
+        and the result stored in self; otherwise, the values in self are
+        preserved.  When and_source is True, the 'source' attribute is
+        included in the copy.
+
+        NOTE: When replace is False, and self contains a 'source' attribute,
+              'source' is not replaced even when dict_ has a 'source'
+              attribute, though it may still be merged into a list depending
+              on the value of update_fun.
+        """
+        self.update_all_atts(dict_, Element.copy_attr_concatenate, replace,
+                             and_source)
+
+    def update_all_atts_coercion(self, dict_, replace=True,
+                                 and_source=False):
+        """
+        Updates all attributes from node or dictionary `dict_`.
+
+        Appends the basic attributes ('ids', 'names', 'classes',
+        'dupnames', but not 'source') and then, for all other attributes in
+        dict_, updates the same attribute in self.  When attributes with the
+        same identifier appear in both self and dict_ whose values are both
+        not lists and replace is True, the values in self are replaced with
+        the values in dict_; if either of the values from self and dict_ for
+        the given identifier are of list type, then first any non-lists are
+        converted to 1-element lists and then the two lists are concatenated
+        and the result stored in self; otherwise, the values in self are
+        preserved.  When and_source is True, the 'source' attribute is
+        included in the copy.
+
+        NOTE: When replace is False, and self contains a 'source' attribute,
+              'source' is not replaced even when dict_ has a 'source'
+              attribute, though it may still be merged into a list depending
+              on the value of update_fun.
+        """
+        self.update_all_atts(dict_, Element.copy_attr_coerce, replace,
+                             and_source)
+
+    def update_all_atts_convert(self, dict_, and_source=False):
+        """
+        Updates all attributes from node or dictionary `dict_`.
+
+        Appends the basic attributes ('ids', 'names', 'classes',
+        'dupnames', but not 'source') and then, for all other attributes in
+        dict_, updates the same attribute in self.  When attributes with the
+        same identifier appear in both self and dict_ then first any non-lists
+        are converted to 1-element lists and then the two lists are
+        concatenated and the result stored in self; otherwise, the values in
+        self are preserved.  When and_source is True, the 'source' attribute
+        is included in the copy.
+
+        NOTE: When replace is False, and self contains a 'source' attribute,
+              'source' is not replaced even when dict_ has a 'source'
+              attribute, though it may still be merged into a list depending
+              on the value of update_fun.
+        """
+        self.update_all_atts(dict_, Element.copy_attr_convert,
+                             and_source=and_source)
+
+    def clear(self):
+        self.children = []
+
+    def replace(self, old, new):
+        """Replace one child `Node` with another child or children."""
+        index = self.index(old)
+        if isinstance(new, Node):
+            self.setup_child(new)
+            self[index] = new
+        elif new is not None:
+            self[index:index+1] = new
+
+    def replace_self(self, new):
+        """
+        Replace `self` node with `new`, where `new` is a node or a
+        list of nodes.
+        """
+        update = new
+        if not isinstance(new, Node):
+            # `new` is a list; update first child.
+            try:
+                update = new[0]
+            except IndexError:
+                update = None
+        if isinstance(update, Element):
+            update.update_basic_atts(self)
+        else:
+            # `update` is a Text node or `new` is an empty list.
+            # Assert that we aren't losing any attributes.
+            for att in self.basic_attributes:
+                assert not self[att], \
+                       'Losing "%s" attribute: %s' % (att, self[att])
+        self.parent.replace(self, new)
+
+    def first_child_matching_class(self, childclass, start=0, end=sys.maxsize):
+        """
+        Return the index of the first child whose class exactly matches.
+
+        Parameters:
+
+        - `childclass`: A `Node` subclass to search for, or a tuple of `Node`
+          classes. If a tuple, any of the classes may match.
+        - `start`: Initial index to check.
+        - `end`: Initial index to *not* check.
+        """
+        if not isinstance(childclass, tuple):
+            childclass = (childclass,)
+        for index in range(start, min(len(self), end)):
+            for c in childclass:
+                if isinstance(self[index], c):
+                    return index
+        return None
 
-    def previousSiblingGenerator(self):
-        return self.previous_siblings
+    def first_child_not_matching_class(self, childclass, start=0,
+                                       end=sys.maxsize):
+        """
+        Return the index of the first child whose class does *not* match.
+
+        Parameters:
+
+        - `childclass`: A `Node` subclass to skip, or a tuple of `Node`
+          classes. If a tuple, none of the classes may match.
+        - `start`: Initial index to check.
+        - `end`: Initial index to *not* check.
+        """
+        if not isinstance(childclass, tuple):
+            childclass = (childclass,)
+        for index in range(start, min(len(self), end)):
+            for c in childclass:
+                if isinstance(self.children[index], c):
+                    break
+            else:
+                return index
+        return None
+
+    def pformat(self, indent='    ', level=0):
+        tagline = '%s%s\n' % (indent*level, self.starttag())
+        childreps = (c.pformat(indent, level+1) for c in self.children)
+        return ''.join((tagline, *childreps))
+
+    def copy(self):
+        obj = self.__class__(rawsource=self.rawsource, **self.attributes)
+        obj._document = self._document
+        obj.source = self.source
+        obj.line = self.line
+        return obj
+
+    def deepcopy(self):
+        copy = self.copy()
+        copy.extend([child.deepcopy() for child in self.children])
+        return copy
+
+    def set_class(self, name):
+        """Add a new class to the "classes" attribute."""
+        warnings.warn('docutils.nodes.Element.set_class() is deprecated; '
+                      ' and will be removed in Docutils 0.21 or later.'
+                      "Append to Element['classes'] list attribute directly",
+                      DeprecationWarning, stacklevel=2)
+        assert ' ' not in name
+        self['classes'].append(name.lower())
+
+    def note_referenced_by(self, name=None, id=None):
+        """Note that this Element has been referenced by its name
+        `name` or id `id`."""
+        self.referenced = 1
+        # Element.expect_referenced_by_* dictionaries map names or ids
+        # to nodes whose ``referenced`` attribute is set to true as
+        # soon as this node is referenced by the given name or id.
+        # Needed for target propagation.
+        by_name = getattr(self, 'expect_referenced_by_name', {}).get(name)
+        by_id = getattr(self, 'expect_referenced_by_id', {}).get(id)
+        if by_name:
+            assert name is not None
+            by_name.referenced = 1
+        if by_id:
+            assert id is not None
+            by_id.referenced = 1
+
+    @classmethod
+    def is_not_list_attribute(cls, attr):
+        """
+        Returns True if and only if the given attribute is NOT one of the
+        basic list attributes defined for all Elements.
+        """
+        return attr not in cls.list_attributes
 
-    def parentGenerator(self):
-        return self.parents
+    @classmethod
+    def is_not_known_attribute(cls, attr):
+        """
+        Returns True if and only if the given attribute is NOT recognized by
+        this class.
+        """
+        return attr not in cls.known_attributes
 
 
-class NavigableString(str, PageElement):
-    """A Python Unicode string that is part of a parse tree.
+class TextElement(Element):
 
-    When Beautiful Soup parses the markup <b>penguin</b>, it will
-    create a NavigableString for the string "penguin".
     """
+    An element which directly contains text.
 
-    PREFIX = ''
-    SUFFIX = ''
+    Its children are all `Text` or `Inline` subclass nodes.  You can
+    check whether an element's context is inline simply by checking whether
+    its immediate parent is a `TextElement` instance (including subclasses).
+    This is handy for nodes like `image` that can appear both inline and as
+    standalone body elements.
 
-    def __new__(cls, value):
-        """Create a new NavigableString.
+    If passing children to `__init__()`, make sure to set `text` to
+    ``''`` or some other suitable value.
+    """
 
-        When unpickling a NavigableString, this method is called with
-        the string in DEFAULT_OUTPUT_ENCODING. That encoding needs to be
-        passed in to the superclass's __new__ or the superclass won't know
-        how to handle non-ASCII characters.
-        """
-        if isinstance(value, str):
-            u = str.__new__(cls, value)
-        else:
-            u = str.__new__(cls, value, DEFAULT_OUTPUT_ENCODING)
-        u.setup()
-        return u
-
-    def __deepcopy__(self, memo, recursive=False):
-        """A copy of a NavigableString has the same contents and class
-        as the original, but it is not connected to the parse tree.
-
-        :param recursive: This parameter is ignored; it's only defined
-           so that NavigableString.__deepcopy__ implements the same
-           signature as Tag.__deepcopy__.
-        """
-        return type(self)(self)
-
-    def __copy__(self):
-        """A copy of a NavigableString can only be a deep copy, because
-        only one PageElement can occupy a given place in a parse tree.
-        """
-        return self.__deepcopy__({})
-
-    def __getnewargs__(self):
-        return (str(self),)
-
-    def __getattr__(self, attr):
-        """text.string gives you text. This is for backwards
-        compatibility for Navigable*String, but for CData* it lets you
-        get the string without the CData wrapper."""
-        if attr == 'string':
-            return self
+    child_text_separator = ''
+    """Separator for child nodes, used by `astext()` method."""
+
+    def __init__(self, rawsource='', text='', *children, **attributes):
+        if text != '':
+            textnode = Text(text)
+            Element.__init__(self, rawsource, textnode, *children,
+                             **attributes)
         else:
-            raise AttributeError(
-                "'%s' object has no attribute '%s'" % (
-                    self.__class__.__name__, attr))
+            Element.__init__(self, rawsource, *children, **attributes)
 
-    def output_ready(self, formatter="minimal"):
-        """Run the string through the provided formatter.
 
-        :param formatter: A Formatter object, or a string naming one of the standard formatters.
-        """
-        output = self.format_string(self, formatter)
-        return self.PREFIX + output + self.SUFFIX
+class FixedTextElement(TextElement):
 
-    @property
-    def name(self):
-        """Since a NavigableString is not a Tag, it has no .name.
+    """An element which directly contains preformatted text."""
 
-        This property is implemented so that code like this doesn't crash
-        when run on a mixture of Tag and NavigableString objects:
-            [x.name for x in tag.children]
-        """
-        return None
+    def __init__(self, rawsource='', text='', *children, **attributes):
+        TextElement.__init__(self, rawsource, text, *children, **attributes)
+        self.attributes['xml:space'] = 'preserve'
 
-    @name.setter
-    def name(self, name):
-        """Prevent NavigableString.name from ever being set."""
-        raise AttributeError("A NavigableString cannot be given a name.")
-
-    def _all_strings(self, strip=False, types=PageElement.default):
-        """Yield all strings of certain classes, possibly stripping them.
-
-        This makes it easy for NavigableString to implement methods
-        like get_text() as conveniences, creating a consistent
-        text-extraction API across all PageElements.
-
-        :param strip: If True, all strings will be stripped before being
-            yielded.
-
-        :param types: A tuple of NavigableString subclasses. If this
-            NavigableString isn't one of those subclasses, the
-            sequence will be empty. By default, the subclasses
-            considered are NavigableString and CData objects. That
-            means no comments, processing instructions, etc.
-
-        :yield: A sequence that either contains this string, or is empty.
-
-        """
-        if types is self.default:
-            # This is kept in Tag because it's full of subclasses of
-            # this class, which aren't defined until later in the file.
-            types = Tag.DEFAULT_INTERESTING_STRING_TYPES
-
-        # Do nothing if the caller is looking for specific types of
-        # string, and we're of a different type.
-        #
-        # We check specific types instead of using isinstance(self,
-        # types) because all of these classes subclass
-        # NavigableString. Anyone who's using this feature probably
-        # wants generic NavigableStrings but not other stuff.
-        my_type = type(self)
-        if types is not None:
-            if isinstance(types, type):
-                # Looking for a single type.
-                if my_type is not types:
-                    return
-            elif my_type not in types:
-                # Looking for one of a list of types.
-                return
 
-        value = self
-        if strip:
-            value = value.strip()
-        if len(value) > 0:
-            yield value
-    strings = property(_all_strings)
+# ========
+#  Mixins
+# ========
 
-class PreformattedString(NavigableString):
-    """A NavigableString not subject to the normal formatting rules.
+class Resolvable:
 
-    This is an abstract class used for special kinds of strings such
-    as comments (the Comment class) and CDATA blocks (the CData
-    class).
-    """
+    resolved = 0
 
-    PREFIX = ''
-    SUFFIX = ''
 
-    def output_ready(self, formatter=None):
-        """Make this string ready for output by adding any subclass-specific
-            prefix or suffix.
+class BackLinkable:
 
-        :param formatter: A Formatter object, or a string naming one
-            of the standard formatters. The string will be passed into the
-            Formatter, but only to trigger any side effects: the return
-            value is ignored.
+    def add_backref(self, refid):
+        self['backrefs'].append(refid)
 
-        :return: The string, with any subclass-specific prefix and
-           suffix added on.
-        """
-        if formatter is not None:
-            ignore = self.format_string(self, formatter)
-        return self.PREFIX + self + self.SUFFIX
 
-class CData(PreformattedString):
-    """A CDATA block."""
-    PREFIX = '<![CDATA['
-    SUFFIX = ']]>'
+# ====================
+#  Element Categories
+# ====================
 
-class ProcessingInstruction(PreformattedString):
-    """A SGML processing instruction."""
+class Root:
+    pass
 
-    PREFIX = '<?'
-    SUFFIX = '>'
 
-class XMLProcessingInstruction(ProcessingInstruction):
-    """An XML processing instruction."""
-    PREFIX = '<?'
-    SUFFIX = '?>'
+class Titular:
+    pass
 
-class Comment(PreformattedString):
-    """An HTML or XML comment."""
-    PREFIX = '<!--'
-    SUFFIX = '-->'
 
+class PreBibliographic:
+    """Category of Node which may occur before Bibliographic Nodes."""
 
-class Declaration(PreformattedString):
-    """An XML declaration."""
-    PREFIX = '<?'
-    SUFFIX = '?>'
 
+class Bibliographic:
+    pass
 
-class Doctype(PreformattedString):
-    """A document type declaration."""
-    @classmethod
-    def for_name_and_ids(cls, name, pub_id, system_id):
-        """Generate an appropriate document type declaration for a given
-        public ID and system ID.
 
-        :param name: The name of the document's root element, e.g. 'html'.
-        :param pub_id: The Formal Public Identifier for this document type,
-            e.g. '-//W3C//DTD XHTML 1.1//EN'
-        :param system_id: The system identifier for this document type,
-            e.g. 'http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd'
+class Decorative(PreBibliographic):
+    pass
 
-        :return: A Doctype.
-        """
-        value = name or ''
-        if pub_id is not None:
-            value += ' PUBLIC "%s"' % pub_id
-            if system_id is not None:
-                value += ' "%s"' % system_id
-        elif system_id is not None:
-            value += ' SYSTEM "%s"' % system_id
 
-        return Doctype(value)
+class Structural:
+    pass
 
-    PREFIX = '<!DOCTYPE '
-    SUFFIX = '>\n'
 
+class Body:
+    pass
 
-class Stylesheet(NavigableString):
-    """A NavigableString representing an stylesheet (probably
-    CSS).
 
-    Used to distinguish embedded stylesheets from textual content.
-    """
+class General(Body):
     pass
 
 
-class Script(NavigableString):
-    """A NavigableString representing an executable script (probably
-    Javascript).
+class Sequential(Body):
+    """List-like elements."""
 
-    Used to distinguish executable code from textual content.
-    """
-    pass
 
+class Admonition(Body): pass
 
-class TemplateString(NavigableString):
-    """A NavigableString representing a string found inside an HTML
-    template embedded in a larger document.
 
-    Used to distinguish such strings from the main body of the document.
-    """
+class Special(Body):
+    """Special internal body elements."""
+
+
+class Invisible(PreBibliographic):
+    """Internal elements that don't appear in output."""
+
+
+class Part:
     pass
 
 
-class RubyTextString(NavigableString):
-    """A NavigableString representing the contents of the <rt> HTML
-    element.
+class Inline:
+    pass
 
-    https://dev.w3.org/html5/spec-LC/text-level-semantics.html#the-rt-element
 
-    Can be used to distinguish such strings from the strings they're
-    annotating.
-    """
+class Referential(Resolvable):
     pass
 
 
-class RubyParenthesisString(NavigableString):
-    """A NavigableString representing the contents of the <rp> HTML
-    element.
+class Targetable(Resolvable):
+
+    referenced = 0
+
+    indirect_reference_name = None
+    """Holds the whitespace_normalized_name (contains mixed case) of a target.
+    Required for MoinMoin/reST compatibility."""
+
+
+class Labeled:
+    """Contains a `label` as its first element."""
+
+
+# ==============
+#  Root Element
+# ==============
+
+class document(Root, Structural, Element):
 
-    https://dev.w3.org/html5/spec-LC/text-level-semantics.html#the-rp-element
     """
-    pass
+    The document root element.
+
+    Do not instantiate this class directly; use
+    `docutils.utils.new_document()` instead.
+    """
+
+    def __init__(self, settings, reporter, *args, **kwargs):
+        Element.__init__(self, *args, **kwargs)
+
+        self.current_source = None
+        """Path to or description of the input source being processed."""
+
+        self.current_line = None
+        """Line number (1-based) of `current_source`."""
+
+        self.settings = settings
+        """Runtime settings data record."""
+
+        self.reporter = reporter
+        """System message generator."""
+
+        self.indirect_targets = []
+        """List of indirect target nodes."""
+
+        self.substitution_defs = {}
+        """Mapping of substitution names to substitution_definition nodes."""
+
+        self.substitution_names = {}
+        """Mapping of case-normalized substitution names to case-sensitive
+        names."""
+
+        self.refnames = {}
+        """Mapping of names to lists of referencing nodes."""
+
+        self.refids = {}
+        """Mapping of ids to lists of referencing nodes."""
+
+        self.nameids = {}
+        """Mapping of names to unique id's."""
+
+        self.nametypes = {}
+        """Mapping of names to hyperlink type (boolean: True => explicit,
+        False => implicit."""
+
+        self.ids = {}
+        """Mapping of ids to nodes."""
+
+        self.footnote_refs = {}
+        """Mapping of footnote labels to lists of footnote_reference nodes."""
+
+        self.citation_refs = {}
+        """Mapping of citation labels to lists of citation_reference nodes."""
+
+        self.autofootnotes = []
+        """List of auto-numbered footnote nodes."""
+
+        self.autofootnote_refs = []
+        """List of auto-numbered footnote_reference nodes."""
 
+        self.symbol_footnotes = []
+        """List of symbol footnote nodes."""
 
-class Tag(PageElement):
-    """Represents an HTML or XML tag that is part of a parse tree, along
-    with its attributes and contents.
-
-    When Beautiful Soup parses the markup <b>penguin</b>, it will
-    create a Tag object representing the <b> tag.
-    """
-
-    def __init__(self, parser=None, builder=None, name=None, namespace=None,
-                 prefix=None, attrs=None, parent=None, previous=None,
-                 is_xml=None, sourceline=None, sourcepos=None,
-                 can_be_empty_element=None, cdata_list_attributes=None,
-                 preserve_whitespace_tags=None,
-                 interesting_string_types=None,
-                 namespaces=None
-    ):
-        """Basic constructor.
-
-        :param parser: A BeautifulSoup object.
-        :param builder: A TreeBuilder.
-        :param name: The name of the tag.
-        :param namespace: The URI of this Tag's XML namespace, if any.
-        :param prefix: The prefix for this Tag's XML namespace, if any.
-        :param attrs: A dictionary of this Tag's attribute values.
-        :param parent: The PageElement to use as this Tag's parent.
-        :param previous: The PageElement that was parsed immediately before
-            this tag.
-        :param is_xml: If True, this is an XML tag. Otherwise, this is an
-            HTML tag.
-        :param sourceline: The line number where this tag was found in its
-            source document.
-        :param sourcepos: The character position within `sourceline` where this
-            tag was found.
-        :param can_be_empty_element: If True, this tag should be
-            represented as <tag/>. If False, this tag should be represented
-            as <tag></tag>.
-        :param cdata_list_attributes: A list of attributes whose values should
-            be treated as CDATA if they ever show up on this tag.
-        :param preserve_whitespace_tags: A list of tag names whose contents
-            should have their whitespace preserved.
-        :param interesting_string_types: This is a NavigableString
-            subclass or a tuple of them. When iterating over this
-            Tag's strings in methods like Tag.strings or Tag.get_text,
-            these are the types of strings that are interesting enough
-            to be considered. The default is to consider
-            NavigableString and CData the only interesting string
-            subtypes.
-        :param namespaces: A dictionary mapping currently active
-            namespace prefixes to URIs. This can be used later to
-            construct CSS selectors.
+        self.symbol_footnote_refs = []
+        """List of symbol footnote_reference nodes."""
+
+        self.footnotes = []
+        """List of manually-numbered footnote nodes."""
+
+        self.citations = []
+        """List of citation nodes."""
+
+        self.autofootnote_start = 1
+        """Initial auto-numbered footnote number."""
+
+        self.symbol_footnote_start = 0
+        """Initial symbol footnote symbol index."""
+
+        self.id_counter = Counter()
+        """Numbers added to otherwise identical IDs."""
+
+        self.parse_messages = []
+        """System messages generated while parsing."""
+
+        self.transform_messages = []
+        """System messages generated while applying transforms."""
+
+        import docutils.transforms
+        self.transformer = docutils.transforms.Transformer(self)
+        """Storage for transforms to be applied to this document."""
+
+        self.include_log = []
+        """The current source's parents (to detect inclusion loops)."""
+
+        self.decoration = None
+        """Document's `decoration` node."""
+
+        self._document = self
+
+    def __getstate__(self):
         """
-        if parser is None:
-            self.parser_class = None
-        else:
-            # We don't actually store the parser object: that lets extracted
-            # chunks be garbage-collected.
-            self.parser_class = parser.__class__
-        if name is None:
-            raise ValueError("No value provided for new tag's name.")
-        self.name = name
-        self.namespace = namespace
-        self._namespaces = namespaces or {}
-        self.prefix = prefix
-        if ((not builder or builder.store_line_numbers)
-            and (sourceline is not None or sourcepos is not None)):
-            self.sourceline = sourceline
-            self.sourcepos = sourcepos
-        if attrs is None:
-            attrs = {}
-        elif attrs:
-            if builder is not None and builder.cdata_list_attributes:
-                attrs = builder._replace_cdata_list_attribute_values(
-                    self.name, attrs)
+        Return dict with unpicklable references removed.
+        """
+        state = self.__dict__.copy()
+        state['reporter'] = None
+        state['transformer'] = None
+        return state
+
+    def asdom(self, dom=None):
+        """Return a DOM representation of this document."""
+        if dom is None:
+            import xml.dom.minidom as dom
+        domroot = dom.Document()
+        domroot.appendChild(self._dom_node(domroot))
+        return domroot
+
+    def set_id(self, node, msgnode=None, suggested_prefix=''):
+        if node['ids']:
+            # register and check for duplicates
+            for id in node['ids']:
+                self.ids.setdefault(id, node)
+                if self.ids[id] is not node:
+                    msg = self.reporter.severe('Duplicate ID: "%s".' % id)
+                    if msgnode is not None:
+                        msgnode += msg
+            return id
+        # generate and set id
+        id_prefix = self.settings.id_prefix
+        auto_id_prefix = self.settings.auto_id_prefix
+        base_id = ''
+        id = ''
+        for name in node['names']:
+            if id_prefix:
+                # allow names starting with numbers if `id_prefix`
+                base_id = make_id('x'+name)[1:]
             else:
-                attrs = dict(attrs)
+                base_id = make_id(name)
+            # TODO: normalize id-prefix? (would make code simpler)
+            id = id_prefix + base_id
+            if base_id and id not in self.ids:
+                break
         else:
-            attrs = dict(attrs)
+            if base_id and auto_id_prefix.endswith('%'):
+                # disambiguate name-derived ID
+                # TODO: remove second condition after announcing change
+                prefix = id + '-'
+            else:
+                prefix = id_prefix + auto_id_prefix
+                if prefix.endswith('%'):
+                    prefix = '%s%s-' % (prefix[:-1],
+                                        suggested_prefix
+                                        or make_id(node.tagname))
+            while True:
+                self.id_counter[prefix] += 1
+                id = '%s%d' % (prefix, self.id_counter[prefix])
+                if id not in self.ids:
+                    break
+        node['ids'].append(id)
+        self.ids[id] = node
+        return id
+
+    def set_name_id_map(self, node, id, msgnode=None, explicit=None):
+        """
+        `self.nameids` maps names to IDs, while `self.nametypes` maps names to
+        booleans representing hyperlink type (True==explicit,
+        False==implicit).  This method updates the mappings.
+
+        The following state transition table shows how `self.nameids` items
+        ("id") and `self.nametypes` items ("type") change with new input
+        (a call to this method), and what actions are performed
+        ("implicit"-type system messages are INFO/1, and
+        "explicit"-type system messages are ERROR/3):
+
+        ====  =====  ========  ========  =======  ====  =====  =====
+         Old State    Input          Action        New State   Notes
+        -----------  --------  -----------------  -----------  -----
+        id    type   new type  sys.msg.  dupname  id    type
+        ====  =====  ========  ========  =======  ====  =====  =====
+        -     -      explicit  -         -        new   True
+        -     -      implicit  -         -        new   False
+        -     False  explicit  -         -        new   True
+        old   False  explicit  implicit  old      new   True
+        -     True   explicit  explicit  new      -     True
+        old   True   explicit  explicit  new,old  -     True   [#]_
+        -     False  implicit  implicit  new      -     False
+        old   False  implicit  implicit  new,old  -     False
+        -     True   implicit  implicit  new      -     True
+        old   True   implicit  implicit  new      old   True
+        ====  =====  ========  ========  =======  ====  =====  =====
+
+        .. [#] Do not clear the name-to-id map or invalidate the old target if
+           both old and new targets are external and refer to identical URIs.
+           The new target is invalidated regardless.
+        """
+        for name in tuple(node['names']):
+            if name in self.nameids:
+                self.set_duplicate_name_id(node, id, name, msgnode, explicit)
+                # attention: modifies node['names']
+            else:
+                self.nameids[name] = id
+                self.nametypes[name] = explicit
 
-        # If possible, determine ahead of time whether this tag is an
-        # XML tag.
-        if builder:
-            self.known_xml = builder.is_xml
+    def set_duplicate_name_id(self, node, id, name, msgnode, explicit):
+        old_id = self.nameids[name]
+        old_explicit = self.nametypes[name]
+        self.nametypes[name] = old_explicit or explicit
+        if explicit:
+            if old_explicit:
+                level = 2
+                if old_id is not None:
+                    old_node = self.ids[old_id]
+                    if 'refuri' in node:
+                        refuri = node['refuri']
+                        if (old_node['names']
+                            and 'refuri' in old_node
+                            and old_node['refuri'] == refuri):
+                            level = 1   # just inform if refuri's identical
+                    if level > 1:
+                        dupname(old_node, name)
+                        self.nameids[name] = None
+                msg = self.reporter.system_message(
+                    level, 'Duplicate explicit target name: "%s".' % name,
+                    backrefs=[id], base_node=node)
+                if msgnode is not None:
+                    msgnode += msg
+                dupname(node, name)
+            else:
+                self.nameids[name] = id
+                if old_id is not None:
+                    old_node = self.ids[old_id]
+                    dupname(old_node, name)
         else:
-            self.known_xml = is_xml
-        self.attrs = attrs
-        self.contents = []
-        self.setup(parent, previous)
-        self.hidden = False
-
-        if builder is None:
-            # In the absence of a TreeBuilder, use whatever values were
-            # passed in here. They're probably None, unless this is a copy of some
-            # other tag.
-            self.can_be_empty_element = can_be_empty_element
-            self.cdata_list_attributes = cdata_list_attributes
-            self.preserve_whitespace_tags = preserve_whitespace_tags
-            self.interesting_string_types = interesting_string_types
+            if old_id is not None and not old_explicit:
+                self.nameids[name] = None
+                old_node = self.ids[old_id]
+                dupname(old_node, name)
+            dupname(node, name)
+        if not explicit or (not old_explicit and old_id is not None):
+            msg = self.reporter.info(
+                'Duplicate implicit target name: "%s".' % name,
+                backrefs=[id], base_node=node)
+            if msgnode is not None:
+                msgnode += msg
+
+    def has_name(self, name):
+        return name in self.nameids
+
+    # "note" here is an imperative verb: "take note of".
+    def note_implicit_target(self, target, msgnode=None):
+        id = self.set_id(target, msgnode)
+        self.set_name_id_map(target, id, msgnode, explicit=False)
+
+    def note_explicit_target(self, target, msgnode=None):
+        id = self.set_id(target, msgnode)
+        self.set_name_id_map(target, id, msgnode, explicit=True)
+
+    def note_refname(self, node):
+        self.refnames.setdefault(node['refname'], []).append(node)
+
+    def note_refid(self, node):
+        self.refids.setdefault(node['refid'], []).append(node)
+
+    def note_indirect_target(self, target):
+        self.indirect_targets.append(target)
+        if target['names']:
+            self.note_refname(target)
+
+    def note_anonymous_target(self, target):
+        self.set_id(target)
+
+    def note_autofootnote(self, footnote):
+        self.set_id(footnote)
+        self.autofootnotes.append(footnote)
+
+    def note_autofootnote_ref(self, ref):
+        self.set_id(ref)
+        self.autofootnote_refs.append(ref)
+
+    def note_symbol_footnote(self, footnote):
+        self.set_id(footnote)
+        self.symbol_footnotes.append(footnote)
+
+    def note_symbol_footnote_ref(self, ref):
+        self.set_id(ref)
+        self.symbol_footnote_refs.append(ref)
+
+    def note_footnote(self, footnote):
+        self.set_id(footnote)
+        self.footnotes.append(footnote)
+
+    def note_footnote_ref(self, ref):
+        self.set_id(ref)
+        self.footnote_refs.setdefault(ref['refname'], []).append(ref)
+        self.note_refname(ref)
+
+    def note_citation(self, citation):
+        self.citations.append(citation)
+
+    def note_citation_ref(self, ref):
+        self.set_id(ref)
+        self.citation_refs.setdefault(ref['refname'], []).append(ref)
+        self.note_refname(ref)
+
+    def note_substitution_def(self, subdef, def_name, msgnode=None):
+        name = whitespace_normalize_name(def_name)
+        if name in self.substitution_defs:
+            msg = self.reporter.error(
+                      'Duplicate substitution definition name: "%s".' % name,
+                      base_node=subdef)
+            if msgnode is not None:
+                msgnode += msg
+            oldnode = self.substitution_defs[name]
+            dupname(oldnode, name)
+        # keep only the last definition:
+        self.substitution_defs[name] = subdef
+        # case-insensitive mapping:
+        self.substitution_names[fully_normalize_name(name)] = name
+
+    def note_substitution_ref(self, subref, refname):
+        subref['refname'] = whitespace_normalize_name(refname)
+
+    def note_pending(self, pending, priority=None):
+        self.transformer.add_pending(pending, priority)
+
+    def note_parse_message(self, message):
+        self.parse_messages.append(message)
+
+    def note_transform_message(self, message):
+        self.transform_messages.append(message)
+
+    def note_source(self, source, offset):
+        self.current_source = source
+        if offset is None:
+            self.current_line = offset
         else:
-            # Set up any substitutions for this tag, such as the charset in a META tag.
-            builder.set_up_substitutions(self)
+            self.current_line = offset + 1
 
-            # Ask the TreeBuilder whether this tag might be an empty-element tag.
-            self.can_be_empty_element = builder.can_be_empty_element(name)
+    def copy(self):
+        obj = self.__class__(self.settings, self.reporter,
+                             **self.attributes)
+        obj.source = self.source
+        obj.line = self.line
+        return obj
 
-            # Keep track of the list of attributes of this tag that
-            # might need to be treated as a list.
-            #
-            # For performance reasons, we store the whole data structure
-            # rather than asking the question of every tag. Asking would
-            # require building a new data structure every time, and
-            # (unlike can_be_empty_element), we almost never need
-            # to check this.
-            self.cdata_list_attributes = builder.cdata_list_attributes
-
-            # Keep track of the names that might cause this tag to be treated as a
-            # whitespace-preserved tag.
-            self.preserve_whitespace_tags = builder.preserve_whitespace_tags
-
-            if self.name in builder.string_containers:
-                # This sort of tag uses a special string container
-                # subclass for most of its strings. When we ask the
-                self.interesting_string_types = builder.string_containers[self.name]
+    def get_decoration(self):
+        if not self.decoration:
+            self.decoration = decoration()
+            index = self.first_child_not_matching_class((Titular, meta))
+            if index is None:
+                self.append(self.decoration)
             else:
-                self.interesting_string_types = self.DEFAULT_INTERESTING_STRING_TYPES
+                self.insert(index, self.decoration)
+        return self.decoration
 
-    parserClass = _alias("parser_class")  # BS3
 
-    def __deepcopy__(self, memo, recursive=True):
-        """A deepcopy of a Tag is a new Tag, unconnected to the parse tree.
-        Its contents are a copy of the old Tag's contents.
-        """
-        clone = self._clone()
-
-        if recursive:
-            # Clone this tag's descendants recursively, but without
-            # making any recursive function calls.
-            tag_stack = [clone]
-            for event, element in self._event_stream(self.descendants):
-                if event is Tag.END_ELEMENT_EVENT:
-                    # Stop appending incoming Tags to the Tag that was
-                    # just closed.
-                    tag_stack.pop()
-                else:
-                    descendant_clone = element.__deepcopy__(
-                        memo, recursive=False
-                    )
-                    # Add to its parent's .contents
-                    tag_stack[-1].append(descendant_clone)
-
-                    if event is Tag.START_ELEMENT_EVENT:
-                        # Add the Tag itself to the stack so that its
-                        # children will be .appended to it.
-                        tag_stack.append(descendant_clone)
-        return clone
-
-    def __copy__(self):
-        """A copy of a Tag must always be a deep copy, because a Tag's
-        children can only have one parent at a time.
-        """
-        return self.__deepcopy__({})
-
-    def _clone(self):
-        """Create a new Tag just like this one, but with no
-        contents and unattached to any parse tree.
-
-        This is the first step in the deepcopy process.
-        """
-        clone = type(self)(
-            None, self.builder, self.name, self.namespace,
-            self.prefix, self.attrs, is_xml=self._is_xml,
-            sourceline=self.sourceline, sourcepos=self.sourcepos,
-            can_be_empty_element=self.can_be_empty_element,
-            cdata_list_attributes=self.cdata_list_attributes,
-            preserve_whitespace_tags=self.preserve_whitespace_tags,
-            interesting_string_types=self.interesting_string_types
-        )
-        for attr in ('can_be_empty_element', 'hidden'):
-            setattr(clone, attr, getattr(self, attr))
-        return clone
-    
-    @property
-    def is_empty_element(self):
-        """Is this tag an empty-element tag? (aka a self-closing tag)
+# ================
+#  Title Elements
+# ================
 
-        A tag that has contents is never an empty-element tag.
+class title(Titular, PreBibliographic, TextElement): pass
+class subtitle(Titular, PreBibliographic, TextElement): pass
+class rubric(Titular, TextElement): pass
 
-        A tag that has no contents may or may not be an empty-element
-        tag. It depends on the builder used to create the tag. If the
-        builder has a designated list of empty-element tags, then only
-        a tag whose name shows up in that list is considered an
-        empty-element tag.
 
-        If the builder has no designated list of empty-element tags,
-        then any tag with no contents is an empty-element tag.
-        """
-        return len(self.contents) == 0 and self.can_be_empty_element
-    isSelfClosing = is_empty_element  # BS3
+# ==================
+#  Meta-Data Element
+# ==================
 
-    @property
-    def string(self):
-        """Convenience property to get the single string within this
-        PageElement.
-
-        TODO It might make sense to have NavigableString.string return
-        itself.
-
-        :return: If this element has a single string child, return
-         value is that string. If this element has one child tag,
-         return value is the 'string' attribute of the child tag,
-         recursively. If this element is itself a string, has no
-         children, or has more than one child, return value is None.
-        """
-        if len(self.contents) != 1:
-            return None
-        child = self.contents[0]
-        if isinstance(child, NavigableString):
-            return child
-        return child.string
-
-    @string.setter
-    def string(self, string):
-        """Replace this PageElement's contents with `string`."""
-        self.clear()
-        self.append(string.__class__(string))
-
-    DEFAULT_INTERESTING_STRING_TYPES = (NavigableString, CData)
-    def _all_strings(self, strip=False, types=PageElement.default):
-        """Yield all strings of certain classes, possibly stripping them.
-
-        :param strip: If True, all strings will be stripped before being
-            yielded.
-
-        :param types: A tuple of NavigableString subclasses. Any strings of
-            a subclass not found in this list will be ignored. By
-            default, the subclasses considered are the ones found in
-            self.interesting_string_types. If that's not specified,
-            only NavigableString and CData objects will be
-            considered. That means no comments, processing
-            instructions, etc.
+class meta(PreBibliographic, Element):
+    """Container for "invisible" bibliographic data, or meta-data."""
 
-        :yield: A sequence of strings.
 
-        """
-        if types is self.default:
-            types = self.interesting_string_types
+# ========================
+#  Bibliographic Elements
+# ========================
 
-        for descendant in self.descendants:
-            if (types is None and not isinstance(descendant, NavigableString)):
-                continue
-            descendant_type = type(descendant)
-            if isinstance(types, type):
-                if descendant_type is not types:
-                    # We're not interested in strings of this type.
-                    continue
-            elif types is not None and descendant_type not in types:
-                # We're not interested in strings of this type.
-                continue
-            if strip:
-                descendant = descendant.strip()
-                if len(descendant) == 0:
-                    continue
-            yield descendant
-    strings = property(_all_strings)
-
-    def decompose(self):
-        """Recursively destroys this PageElement and its children.
-
-        This element will be removed from the tree and wiped out; so
-        will everything beneath it.
-
-        The behavior of a decomposed PageElement is undefined and you
-        should never use one for anything, but if you need to _check_
-        whether an element has been decomposed, you can use the
-        `decomposed` property.
-        """
-        self.extract()
-        i = self
-        while i is not None:
-            n = i.next_element
-            i.__dict__.clear()
-            i.contents = []
-            i._decomposed = True
-            i = n
-
-    def clear(self, decompose=False):
-        """Wipe out all children of this PageElement by calling extract()
-           on them.
-
-        :param decompose: If this is True, decompose() (a more
-            destructive method) will be called instead of extract().
-        """
-        if decompose:
-            for element in self.contents[:]:
-                if isinstance(element, Tag):
-                    element.decompose()
-                else:
-                    element.extract()
-        else:
-            for element in self.contents[:]:
-                element.extract()
+class docinfo(Bibliographic, Element): pass
+class author(Bibliographic, TextElement): pass
+class authors(Bibliographic, Element): pass
+class organization(Bibliographic, TextElement): pass
+class address(Bibliographic, FixedTextElement): pass
+class contact(Bibliographic, TextElement): pass
+class version(Bibliographic, TextElement): pass
+class revision(Bibliographic, TextElement): pass
+class status(Bibliographic, TextElement): pass
+class date(Bibliographic, TextElement): pass
+class copyright(Bibliographic, TextElement): pass
 
-    def smooth(self):
-        """Smooth out this element's children by consolidating consecutive
-        strings.
-
-        This makes pretty-printed output look more natural following a
-        lot of operations that modified the tree.
-        """
-        # Mark the first position of every pair of children that need
-        # to be consolidated.  Do this rather than making a copy of
-        # self.contents, since in most cases very few strings will be
-        # affected.
-        marked = []
-        for i, a in enumerate(self.contents):
-            if isinstance(a, Tag):
-                # Recursively smooth children.
-                a.smooth()
-            if i == len(self.contents)-1:
-                # This is the last item in .contents, and it's not a
-                # tag. There's no chance it needs any work.
-                continue
-            b = self.contents[i+1]
-            if (isinstance(a, NavigableString)
-                and isinstance(b, NavigableString)
-                and not isinstance(a, PreformattedString)
-                and not isinstance(b, PreformattedString)
-            ):
-                marked.append(i)
-
-        # Go over the marked positions in reverse order, so that
-        # removing items from .contents won't affect the remaining
-        # positions.
-        for i in reversed(marked):
-            a = self.contents[i]
-            b = self.contents[i+1]
-            b.extract()
-            n = NavigableString(a+b)
-            a.replace_with(n)
-
-    def index(self, element):
-        """Find the index of a child by identity, not value.
-
-        Avoids issues with tag.contents.index(element) getting the
-        index of equal elements.
-
-        :param element: Look for this PageElement in `self.contents`.
-        """
-        for i, child in enumerate(self.contents):
-            if child is element:
-                return i
-        raise ValueError("Tag.index: element not in tag")
-
-    def get(self, key, default=None):
-        """Returns the value of the 'key' attribute for the tag, or
-        the value given for 'default' if it doesn't have that
-        attribute."""
-        return self.attrs.get(key, default)
-
-    def get_attribute_list(self, key, default=None):
-        """The same as get(), but always returns a list.
-
-        :param key: The attribute to look for.
-        :param default: Use this value if the attribute is not present
-            on this PageElement.
-        :return: A list of values, probably containing only a single
-            value.
-        """
-        value = self.get(key, default)
-        if not isinstance(value, list):
-            value = [value]
-        return value
 
-    def has_attr(self, key):
-        """Does this PageElement have an attribute with the given name?"""
-        return key in self.attrs
+# =====================
+#  Decorative Elements
+# =====================
 
-    def __hash__(self):
-        return str(self).__hash__()
+class decoration(Decorative, Element):
 
-    def __getitem__(self, key):
-        """tag[key] returns the value of the 'key' attribute for the Tag,
-        and throws an exception if it's not there."""
-        return self.attrs[key]
-
-    def __iter__(self):
-        "Iterating over a Tag iterates over its contents."
-        return iter(self.contents)
+    def get_header(self):
+        if not len(self.children) or not isinstance(self.children[0], header):
+            self.insert(0, header())
+        return self.children[0]
 
-    def __len__(self):
-        "The length of a Tag is the length of its list of contents."
-        return len(self.contents)
+    def get_footer(self):
+        if not len(self.children) or not isinstance(self.children[-1], footer):
+            self.append(footer())
+        return self.children[-1]
 
-    def __contains__(self, x):
-        return x in self.contents
 
-    def __bool__(self):
-        "A tag is non-None even if it has no contents."
-        return True
+class header(Decorative, Element): pass
+class footer(Decorative, Element): pass
 
-    def __setitem__(self, key, value):
-        """Setting tag[key] sets the value of the 'key' attribute for the
-        tag."""
-        self.attrs[key] = value
 
-    def __delitem__(self, key):
-        "Deleting tag[key] deletes all 'key' attributes for the tag."
-        self.attrs.pop(key, None)
+# =====================
+#  Structural Elements
+# =====================
 
-    def __call__(self, *args, **kwargs):
-        """Calling a Tag like a function is the same as calling its
-        find_all() method. Eg. tag('a') returns a list of all the A tags
-        found within this tag."""
-        return self.find_all(*args, **kwargs)
-
-    def __getattr__(self, tag):
-        """Calling tag.subtag is the same as calling tag.find(name="subtag")"""
-        #print("Getattr %s.%s" % (self.__class__, tag))
-        if len(tag) > 3 and tag.endswith('Tag'):
-            # BS3: soup.aTag -> "soup.find("a")
-            tag_name = tag[:-3]
-            warnings.warn(
-                '.%(name)sTag is deprecated, use .find("%(name)s") instead. If you really were looking for a tag called %(name)sTag, use .find("%(name)sTag")' % dict(
-                    name=tag_name
-                ),
-                DeprecationWarning, stacklevel=2
-            )
-            return self.find(tag_name)
-        # We special case contents to avoid recursion.
-        elif not tag.startswith("__") and not tag == "contents":
-            return self.find(tag)
-        raise AttributeError(
-            "'%s' object has no attribute '%s'" % (self.__class__, tag))
-
-    def __eq__(self, other):
-        """Returns true iff this Tag has the same name, the same attributes,
-        and the same contents (recursively) as `other`."""
-        if self is other:
-            return True
-        if (not hasattr(other, 'name') or
-            not hasattr(other, 'attrs') or
-            not hasattr(other, 'contents') or
-            self.name != other.name or
-            self.attrs != other.attrs or
-            len(self) != len(other)):
-            return False
-        for i, my_child in enumerate(self.contents):
-            if my_child != other.contents[i]:
-                return False
-        return True
+class section(Structural, Element): pass
 
-    def __ne__(self, other):
-        """Returns true iff this Tag is not identical to `other`,
-        as defined in __eq__."""
-        return not self == other
-
-    def __repr__(self, encoding="unicode-escape"):
-        """Renders this PageElement as a string.
-
-        :param encoding: The encoding to use (Python 2 only).
-            TODO: This is now ignored and a warning should be issued
-            if a value is provided.
-        :return: A (Unicode) string.
-        """
-        # "The return value must be a string object", i.e. Unicode
-        return self.decode()
-
-    def __unicode__(self):
-        """Renders this PageElement as a Unicode string."""
-        return self.decode()
-
-    __str__ = __repr__ = __unicode__
-
-    def encode(self, encoding=DEFAULT_OUTPUT_ENCODING,
-               indent_level=None, formatter="minimal",
-               errors="xmlcharrefreplace"):
-        """Render a bytestring representation of this PageElement and its
-        contents.
-
-        :param encoding: The destination encoding.
-        :param indent_level: Each line of the rendering will be
-           indented this many levels. (The formatter decides what a
-           'level' means in terms of spaces or other characters
-           output.) Used internally in recursive calls while
-           pretty-printing.
-        :param formatter: A Formatter object, or a string naming one of
-            the standard formatters.
-        :param errors: An error handling strategy such as
-            'xmlcharrefreplace'. This value is passed along into
-            encode() and its value should be one of the constants
-            defined by Python.
-        :return: A bytestring.
-
-        """
-        # Turn the data structure into Unicode, then encode the
-        # Unicode.
-        u = self.decode(indent_level, encoding, formatter)
-        return u.encode(encoding, errors)
-
-    def decode(self, indent_level=None,
-               eventual_encoding=DEFAULT_OUTPUT_ENCODING,
-               formatter="minimal",
-               iterator=None):
-        pieces = []
-        # First off, turn a non-Formatter `formatter` into a Formatter
-        # object. This will stop the lookup from happening over and
-        # over again.
-        if not isinstance(formatter, Formatter):
-            formatter = self.formatter_for_name(formatter)
-
-        if indent_level is True:
-            indent_level = 0
-
-        # The currently active tag that put us into string literal
-        # mode. Until this element is closed, children will be treated
-        # as string literals and not pretty-printed. String literal
-        # mode is turned on immediately after this tag begins, and
-        # turned off immediately before it's closed. This means there
-        # will be whitespace before and after the tag itself.
-        string_literal_tag = None
-
-        for event, element in self._event_stream(iterator):
-            if event in (Tag.START_ELEMENT_EVENT, Tag.EMPTY_ELEMENT_EVENT):
-                piece = element._format_tag(
-                    eventual_encoding, formatter, opening=True
-                )
-            elif event is Tag.END_ELEMENT_EVENT:
-                piece = element._format_tag(
-                    eventual_encoding, formatter, opening=False
-                )
-                if indent_level is not None:
-                    indent_level -= 1
-            else:
-                piece = element.output_ready(formatter)
 
-            # Now we need to apply the 'prettiness' -- extra
-            # whitespace before and/or after this tag. This can get
-            # complicated because certain tags, like <pre> and
-            # <script>, can't be prettified, since adding whitespace would
-            # change the meaning of the content.
-
-            # The default behavior is to add whitespace before and
-            # after an element when string literal mode is off, and to
-            # leave things as they are when string literal mode is on.
-            if string_literal_tag:
-                indent_before = indent_after = False
-            else:
-                indent_before = indent_after = True
+class topic(Structural, Element):
 
-            # The only time the behavior is more complex than that is
-            # when we encounter an opening or closing tag that might
-            # put us into or out of string literal mode.
-            if (event is Tag.START_ELEMENT_EVENT
-                and not string_literal_tag
-                and not element._should_pretty_print()):
-                    # We are about to enter string literal mode. Add
-                    # whitespace before this tag, but not after. We
-                    # will stay in string literal mode until this tag
-                    # is closed.
-                    indent_before = True
-                    indent_after = False
-                    string_literal_tag = element
-            elif (event is Tag.END_ELEMENT_EVENT
-                  and element is string_literal_tag):
-                # We are about to exit string literal mode by closing
-                # the tag that sent us into that mode. Add whitespace
-                # after this tag, but not before.
-                indent_before = False
-                indent_after = True
-                string_literal_tag = None
-
-            # Now we know whether to add whitespace before and/or
-            # after this element.
-            if indent_level is not None:
-                if (indent_before or indent_after):
-                    if isinstance(element, NavigableString):
-                        piece = piece.strip()
-                    if piece:
-                        piece = self._indent_string(
-                            piece, indent_level, formatter,
-                            indent_before, indent_after
-                        )
-                if event == Tag.START_ELEMENT_EVENT:
-                    indent_level += 1
-            pieces.append(piece)
-        return "".join(pieces)
-
-    # Names for the different events yielded by _event_stream
-    START_ELEMENT_EVENT = object()
-    END_ELEMENT_EVENT = object()
-    EMPTY_ELEMENT_EVENT = object()
-    STRING_ELEMENT_EVENT = object()
-
-    def _event_stream(self, iterator=None):
-        """Yield a sequence of events that can be used to reconstruct the DOM
-        for this element.
-
-        This lets us recreate the nested structure of this element
-        (e.g. when formatting it as a string) without using recursive
-        method calls.
-
-        This is similar in concept to the SAX API, but it's a simpler
-        interface designed for internal use. The events are different
-        from SAX and the arguments associated with the events are Tags
-        and other Beautiful Soup objects.
-
-        :param iterator: An alternate iterator to use when traversing
-         the tree.
-        """
-        tag_stack = []
-
-        iterator = iterator or self.self_and_descendants
-
-        for c in iterator:
-            # If the parent of the element we're about to yield is not
-            # the tag currently on the stack, it means that the tag on
-            # the stack closed before this element appeared.
-            while tag_stack and c.parent != tag_stack[-1]:
-                now_closed_tag = tag_stack.pop()
-                yield Tag.END_ELEMENT_EVENT, now_closed_tag
-
-            if isinstance(c, Tag):
-                if c.is_empty_element:
-                    yield Tag.EMPTY_ELEMENT_EVENT, c
-                else:
-                    yield Tag.START_ELEMENT_EVENT, c
-                    tag_stack.append(c)
-                    continue
+    """
+    Topics are terminal, "leaf" mini-sections, like block quotes with titles,
+    or textual figures.  A topic is just like a section, except that it has no
+    subsections, and it doesn't have to conform to section placement rules.
+
+    Topics are allowed wherever body elements (list, table, etc.) are allowed,
+    but only at the top level of a section or document.  Topics cannot nest
+    inside topics, sidebars, or body elements; you can't have a topic inside a
+    table, list, block quote, etc.
+    """
+
+
+class sidebar(Structural, Element):
+
+    """
+    Sidebars are like miniature, parallel documents that occur inside other
+    documents, providing related or reference material.  A sidebar is
+    typically offset by a border and "floats" to the side of the page; the
+    document's main text may flow around it.  Sidebars can also be likened to
+    super-footnotes; their content is outside of the flow of the document's
+    main text.
+
+    Sidebars are allowed wherever body elements (list, table, etc.) are
+    allowed, but only at the top level of a section or document.  Sidebars
+    cannot nest inside sidebars, topics, or body elements; you can't have a
+    sidebar inside a table, list, block quote, etc.
+    """
+
+
+class transition(Structural, Element): pass
+
+
+# ===============
+#  Body Elements
+# ===============
+
+class paragraph(General, TextElement): pass
+class compound(General, Element): pass
+class container(General, Element): pass
+class bullet_list(Sequential, Element): pass
+class enumerated_list(Sequential, Element): pass
+class list_item(Part, Element): pass
+class definition_list(Sequential, Element): pass
+class definition_list_item(Part, Element): pass
+class term(Part, TextElement): pass
+class classifier(Part, TextElement): pass
+class definition(Part, Element): pass
+class field_list(Sequential, Element): pass
+class field(Part, Element): pass
+class field_name(Part, TextElement): pass
+class field_body(Part, Element): pass
+
+
+class option(Part, Element):
+
+    child_text_separator = ''
+
+
+class option_argument(Part, TextElement):
+
+    def astext(self):
+        return self.get('delimiter', ' ') + TextElement.astext(self)
+
+
+class option_group(Part, Element):
+
+    child_text_separator = ', '
+
+
+class option_list(Sequential, Element): pass
+
+
+class option_list_item(Part, Element):
+
+    child_text_separator = '  '
+
+
+class option_string(Part, TextElement): pass
+class description(Part, Element): pass
+class literal_block(General, FixedTextElement): pass
+class doctest_block(General, FixedTextElement): pass
+class math_block(General, FixedTextElement): pass
+class line_block(General, Element): pass
+
+
+class line(Part, TextElement):
+
+    indent = None
+
+
+class block_quote(General, Element): pass
+class attribution(Part, TextElement): pass
+class attention(Admonition, Element): pass
+class caution(Admonition, Element): pass
+class danger(Admonition, Element): pass
+class error(Admonition, Element): pass
+class important(Admonition, Element): pass
+class note(Admonition, Element): pass
+class tip(Admonition, Element): pass
+class hint(Admonition, Element): pass
+class warning(Admonition, Element): pass
+class admonition(Admonition, Element): pass
+class comment(Special, Invisible, FixedTextElement): pass
+class substitution_definition(Special, Invisible, TextElement): pass
+class target(Special, Invisible, Inline, TextElement, Targetable): pass
+class footnote(General, BackLinkable, Element, Labeled, Targetable): pass
+class citation(General, BackLinkable, Element, Labeled, Targetable): pass
+class label(Part, TextElement): pass
+class figure(General, Element): pass
+class caption(Part, TextElement): pass
+class legend(Part, Element): pass
+class table(General, Element): pass
+class tgroup(Part, Element): pass
+class colspec(Part, Element): pass
+class thead(Part, Element): pass
+class tbody(Part, Element): pass
+class row(Part, Element): pass
+class entry(Part, Element): pass
+
+
+class system_message(Special, BackLinkable, PreBibliographic, Element):
+
+    """
+    System message element.
+
+    Do not instantiate this class directly; use
+    ``document.reporter.info/warning/error/severe()`` instead.
+    """
+
+    def __init__(self, message=None, *children, **attributes):
+        rawsource = attributes.pop('rawsource', '')
+        if message:
+            p = paragraph('', message)
+            children = (p,) + children
+        try:
+            Element.__init__(self, rawsource, *children, **attributes)
+        except:  # noqa  catchall
+            print('system_message: children=%r' % (children,))
+            raise
+
+    def astext(self):
+        line = self.get('line', '')
+        return '%s:%s: (%s/%s) %s' % (self['source'], line, self['type'],
+                                      self['level'], Element.astext(self))
+
+
+class pending(Special, Invisible, Element):
+
+    """
+    The "pending" element is used to encapsulate a pending operation: the
+    operation (transform), the point at which to apply it, and any data it
+    requires.  Only the pending operation's location within the document is
+    stored in the public document tree (by the "pending" object itself); the
+    operation and its data are stored in the "pending" object's internal
+    instance attributes.
+
+    For example, say you want a table of contents in your reStructuredText
+    document.  The easiest way to specify where to put it is from within the
+    document, with a directive::
+
+        .. contents::
+
+    But the "contents" directive can't do its work until the entire document
+    has been parsed and possibly transformed to some extent.  So the directive
+    code leaves a placeholder behind that will trigger the second phase of its
+    processing, something like this::
+
+        <pending ...public attributes...> + internal attributes
+
+    Use `document.note_pending()` so that the
+    `docutils.transforms.Transformer` stage of processing can run all pending
+    transforms.
+    """
+
+    def __init__(self, transform, details=None,
+                 rawsource='', *children, **attributes):
+        Element.__init__(self, rawsource, *children, **attributes)
+
+        self.transform = transform
+        """The `docutils.transforms.Transform` class implementing the pending
+        operation."""
+
+        self.details = details or {}
+        """Detail data (dictionary) required by the pending operation."""
+
+    def pformat(self, indent='    ', level=0):
+        internals = ['.. internal attributes:',
+                     '     .transform: %s.%s' % (self.transform.__module__,
+                                                 self.transform.__name__),
+                     '     .details:']
+        details = sorted(self.details.items())
+        for key, value in details:
+            if isinstance(value, Node):
+                internals.append('%7s%s:' % ('', key))
+                internals.extend(['%9s%s' % ('', line)
+                                  for line in value.pformat().splitlines()])
+            elif (value
+                  and isinstance(value, list)
+                  and isinstance(value[0], Node)):
+                internals.append('%7s%s:' % ('', key))
+                for v in value:
+                    internals.extend(['%9s%s' % ('', line)
+                                      for line in v.pformat().splitlines()])
             else:
-                yield Tag.STRING_ELEMENT_EVENT, c
+                internals.append('%7s%s: %r' % ('', key, value))
+        return (Element.pformat(self, indent, level)
+                + ''.join(('    %s%s\n' % (indent * level, line))
+                          for line in internals))
+
+    def copy(self):
+        obj = self.__class__(self.transform, self.details, self.rawsource,
+                             **self.attributes)
+        obj._document = self._document
+        obj.source = self.source
+        obj.line = self.line
+        return obj
 
-        while tag_stack:
-            now_closed_tag = tag_stack.pop()
-            yield Tag.END_ELEMENT_EVENT, now_closed_tag
-
-    def _indent_string(self, s, indent_level, formatter,
-                       indent_before, indent_after):
-        """Add indentation whitespace before and/or after a string.
-
-        :param s: The string to amend with whitespace.
-        :param indent_level: The indentation level; affects how much
-           whitespace goes before the string.
-        :param indent_before: Whether or not to add whitespace
-           before the string.
-        :param indent_after: Whether or not to add whitespace
-           (a newline) after the string.
-        """
-        space_before = ''
-        if indent_before and indent_level:
-            space_before = (formatter.indent * indent_level)
-
-        space_after = ''
-        if indent_after:
-            space_after = "\n"
-
-        return space_before + s + space_after
-
-    def _format_tag(self, eventual_encoding, formatter, opening):
-        # A tag starts with the < character (see below).
-
-        # Then the / character, if this is a closing tag.
-        closing_slash = ''
-        if not opening:
-            closing_slash = '/'
-
-        # Then an optional namespace prefix.
-        prefix = ''
-        if self.prefix:
-            prefix = self.prefix + ":"
-
-        # Then a list of attribute values, if this is an opening tag.
-        attribute_string = ''
-        if opening:
-            attributes = formatter.attributes(self)
-            attrs = []
-            for key, val in attributes:
-                if val is None:
-                    decoded = key
-                else:
-                    if isinstance(val, list) or isinstance(val, tuple):
-                        val = ' '.join(val)
-                    elif not isinstance(val, str):
-                        val = str(val)
-                    elif (
-                            isinstance(val, AttributeValueWithCharsetSubstitution)
-                            and eventual_encoding is not None
-                    ):
-                        val = val.encode(eventual_encoding)
-
-                    text = formatter.attribute_value(val)
-                    decoded = (
-                        str(key) + '='
-                        + formatter.quoted_attribute_value(text))
-                attrs.append(decoded)
-            if attrs:
-                attribute_string = ' ' + ' '.join(attrs)
-
-        # Then an optional closing slash (for a void element in an
-        # XML document).
-        void_element_closing_slash = ''
-        if self.is_empty_element:
-            void_element_closing_slash = formatter.void_element_close_prefix or ''
-
-        # Put it all together.
-        return '<' + closing_slash + prefix + self.name + attribute_string + void_element_closing_slash + '>'
-
-    def _should_pretty_print(self, indent_level=1):
-        """Should this tag be pretty-printed?
-
-        Most of them should, but some (such as <pre> in HTML
-        documents) should not.
-        """
-        return (
-            indent_level is not None
-            and (
-                not self.preserve_whitespace_tags
-                or self.name not in self.preserve_whitespace_tags
-            )
-        )
-
-    def prettify(self, encoding=None, formatter="minimal"):
-        """Pretty-print this PageElement as a string.
-
-        :param encoding: The eventual encoding of the string. If this is None,
-            a Unicode string will be returned.
-        :param formatter: A Formatter object, or a string naming one of
-            the standard formatters.
-        :return: A Unicode string (if encoding==None) or a bytestring
-            (otherwise).
-        """
-        if encoding is None:
-            return self.decode(True, formatter=formatter)
-        else:
-            return self.encode(encoding, True, formatter=formatter)
 
-    def decode_contents(self, indent_level=None,
-                       eventual_encoding=DEFAULT_OUTPUT_ENCODING,
-                       formatter="minimal"):
-        """Renders the contents of this tag as a Unicode string.
-
-        :param indent_level: Each line of the rendering will be
-           indented this many levels. (The formatter decides what a
-           'level' means in terms of spaces or other characters
-           output.) Used internally in recursive calls while
-           pretty-printing.
-
-        :param eventual_encoding: The tag is destined to be
-           encoded into this encoding. decode_contents() is _not_
-           responsible for performing that encoding. This information
-           is passed in so that it can be substituted in if the
-           document contains a <META> tag that mentions the document's
-           encoding.
-
-        :param formatter: A Formatter object, or a string naming one of
-            the standard Formatters.
-
-        """
-        return self.decode(indent_level, eventual_encoding, formatter,
-                           iterator=self.descendants)
-
-    def encode_contents(
-        self, indent_level=None, encoding=DEFAULT_OUTPUT_ENCODING,
-        formatter="minimal"):
-        """Renders the contents of this PageElement as a bytestring.
-
-        :param indent_level: Each line of the rendering will be
-           indented this many levels. (The formatter decides what a
-           'level' means in terms of spaces or other characters
-           output.) Used internally in recursive calls while
-           pretty-printing.
-
-        :param eventual_encoding: The bytestring will be in this encoding.
-
-        :param formatter: A Formatter object, or a string naming one of
-            the standard Formatters.
-
-        :return: A bytestring.
-        """
-        contents = self.decode_contents(indent_level, encoding, formatter)
-        return contents.encode(encoding)
-
-    # Old method for BS3 compatibility
-    def renderContents(self, encoding=DEFAULT_OUTPUT_ENCODING,
-                       prettyPrint=False, indentLevel=0):
-        """Deprecated method for BS3 compatibility."""
-        if not prettyPrint:
-            indentLevel = None
-        return self.encode_contents(
-            indent_level=indentLevel, encoding=encoding)
-
-    #Soup methods
-
-    def find(self, name=None, attrs={}, recursive=True, string=None,
-             **kwargs):
-        """Look in the children of this PageElement and find the first
-        PageElement that matches the given criteria.
-
-        All find_* methods take a common set of arguments. See the online
-        documentation for detailed explanations.
-
-        :param name: A filter on tag name.
-        :param attrs: A dictionary of filters on attribute values.
-        :param recursive: If this is True, find() will perform a
-            recursive search of this PageElement's children. Otherwise,
-            only the direct children will be considered.
-        :param limit: Stop looking after finding this many results.
-        :kwargs: A dictionary of filters on attribute values.
-        :return: A PageElement.
-        :rtype: bs4.element.Tag | bs4.element.NavigableString
-        """
-        r = None
-        l = self.find_all(name, attrs, recursive, string, 1, _stacklevel=3,
-                          **kwargs)
-        if l:
-            r = l[0]
-        return r
-    findChild = find #BS2
-
-    def find_all(self, name=None, attrs={}, recursive=True, string=None,
-                 limit=None, **kwargs):
-        """Look in the children of this PageElement and find all
-        PageElements that match the given criteria.
-
-        All find_* methods take a common set of arguments. See the online
-        documentation for detailed explanations.
-
-        :param name: A filter on tag name.
-        :param attrs: A dictionary of filters on attribute values.
-        :param recursive: If this is True, find_all() will perform a
-            recursive search of this PageElement's children. Otherwise,
-            only the direct children will be considered.
-        :param limit: Stop looking after finding this many results.
-        :kwargs: A dictionary of filters on attribute values.
-        :return: A ResultSet of PageElements.
-        :rtype: bs4.element.ResultSet
-        """
-        generator = self.descendants
-        if not recursive:
-            generator = self.children
-        _stacklevel = kwargs.pop('_stacklevel', 2)
-        return self._find_all(name, attrs, string, limit, generator,
-                              _stacklevel=_stacklevel+1, **kwargs)
-    findAll = find_all       # BS3
-    findChildren = find_all  # BS2
+class raw(Special, Inline, PreBibliographic, FixedTextElement):
 
-    #Generator methods
-    @property
-    def children(self):
-        """Iterate over all direct children of this PageElement.
+    """
+    Raw data that is to be passed untouched to the Writer.
+    """
+
+
+# =================
+#  Inline Elements
+# =================
+
+class emphasis(Inline, TextElement): pass
+class strong(Inline, TextElement): pass
+class literal(Inline, TextElement): pass
+class reference(General, Inline, Referential, TextElement): pass
+class footnote_reference(Inline, Referential, TextElement): pass
+class citation_reference(Inline, Referential, TextElement): pass
+class substitution_reference(Inline, TextElement): pass
+class title_reference(Inline, TextElement): pass
+class abbreviation(Inline, TextElement): pass
+class acronym(Inline, TextElement): pass
+class superscript(Inline, TextElement): pass
+class subscript(Inline, TextElement): pass
+class math(Inline, TextElement): pass
+
+
+class image(General, Inline, Element):
+
+    def astext(self):
+        return self.get('alt', '')
+
+
+class inline(Inline, TextElement): pass
+class problematic(Inline, TextElement): pass
+class generated(Inline, TextElement): pass
+
+
+# ========================================
+#  Auxiliary Classes, Functions, and Data
+# ========================================
+
+node_class_names = """
+    Text
+    abbreviation acronym address admonition attention attribution author
+        authors
+    block_quote bullet_list
+    caption caution citation citation_reference classifier colspec comment
+        compound contact container copyright
+    danger date decoration definition definition_list definition_list_item
+        description docinfo doctest_block document
+    emphasis entry enumerated_list error
+    field field_body field_list field_name figure footer
+        footnote footnote_reference
+    generated
+    header hint
+    image important inline
+    label legend line line_block list_item literal literal_block
+    math math_block meta
+    note
+    option option_argument option_group option_list option_list_item
+        option_string organization
+    paragraph pending problematic
+    raw reference revision row rubric
+    section sidebar status strong subscript substitution_definition
+        substitution_reference subtitle superscript system_message
+    table target tbody term tgroup thead tip title title_reference topic
+        transition
+    version
+    warning""".split()
+"""A list of names of all concrete Node subclasses."""
+
+
+class NodeVisitor:
+
+    """
+    "Visitor" pattern [GoF95]_ abstract superclass implementation for
+    document tree traversals.
+
+    Each node class has corresponding methods, doing nothing by
+    default; override individual methods for specific and useful
+    behaviour.  The `dispatch_visit()` method is called by
+    `Node.walk()` upon entering a node.  `Node.walkabout()` also calls
+    the `dispatch_departure()` method before exiting a node.
+
+    The dispatch methods call "``visit_`` + node class name" or
+    "``depart_`` + node class name", resp.
+
+    This is a base class for visitors whose ``visit_...`` & ``depart_...``
+    methods must be implemented for *all* compulsory node types encountered
+    (such as for `docutils.writers.Writer` subclasses).
+    Unimplemented methods will raise exceptions (except for optional nodes).
+
+    For sparse traversals, where only certain node types are of interest, use
+    subclass `SparseNodeVisitor` instead.  When (mostly or entirely) uniform
+    processing is desired, subclass `GenericNodeVisitor`.
+
+    .. [GoF95] Gamma, Helm, Johnson, Vlissides. *Design Patterns: Elements of
+       Reusable Object-Oriented Software*. Addison-Wesley, Reading, MA, USA,
+       1995.
+    """
+
+    optional = ('meta',)
+    """
+    Tuple containing node class names (as strings).
 
-        :yield: A sequence of PageElements.
+    No exception will be raised if writers do not implement visit
+    or departure functions for these node classes.
+
+    Used to ensure transitional compatibility with existing 3rd-party writers.
+    """
+
+    def __init__(self, document):
+        self.document = document
+
+    def dispatch_visit(self, node):
+        """
+        Call self."``visit_`` + node class name" with `node` as
+        parameter.  If the ``visit_...`` method does not exist, call
+        self.unknown_visit.
         """
-        # return iter() to make the purpose of the method clear
-        return iter(self.contents)  # XXX This seems to be untested.
+        node_name = node.__class__.__name__
+        method = getattr(self, 'visit_' + node_name, self.unknown_visit)
+        self.document.reporter.debug(
+            'docutils.nodes.NodeVisitor.dispatch_visit calling %s for %s'
+            % (method.__name__, node_name))
+        return method(node)
 
-    @property
-    def self_and_descendants(self):
-        """Iterate over this PageElement and its children in a
-        breadth-first sequence.
+    def dispatch_departure(self, node):
+        """
+        Call self."``depart_`` + node class name" with `node` as
+        parameter.  If the ``depart_...`` method does not exist, call
+        self.unknown_departure.
+        """
+        node_name = node.__class__.__name__
+        method = getattr(self, 'depart_' + node_name, self.unknown_departure)
+        self.document.reporter.debug(
+            'docutils.nodes.NodeVisitor.dispatch_departure calling %s for %s'
+            % (method.__name__, node_name))
+        return method(node)
 
-        :yield: A sequence of PageElements.
+    def unknown_visit(self, node):
         """
-        if not self.hidden:
-            yield self
-        for i in self.descendants:
-            yield i
+        Called when entering unknown `Node` types.
 
-    @property
-    def descendants(self):
-        """Iterate over all children of this PageElement in a
-        breadth-first sequence.
+        Raise an exception unless overridden.
+        """
+        if (self.document.settings.strict_visitor
+            or node.__class__.__name__ not in self.optional):
+            raise NotImplementedError(
+                '%s visiting unknown node type: %s'
+                % (self.__class__, node.__class__.__name__))
+
+    def unknown_departure(self, node):
+        """
+        Called before exiting unknown `Node` types.
 
-        :yield: A sequence of PageElements.
+        Raise exception unless overridden.
         """
-        if not len(self.contents):
-            return
-        stopNode = self._last_descendant().next_element
-        current = self.contents[0]
-        while current is not stopNode:
-            yield current
-            current = current.next_element
+        if (self.document.settings.strict_visitor
+            or node.__class__.__name__ not in self.optional):
+            raise NotImplementedError(
+                '%s departing unknown node type: %s'
+                % (self.__class__, node.__class__.__name__))
 
-    # CSS selector code
-    def select_one(self, selector, namespaces=None, **kwargs):
-        """Perform a CSS selection operation on the current element.
 
-        :param selector: A CSS selector.
+class SparseNodeVisitor(NodeVisitor):
 
-        :param namespaces: A dictionary mapping namespace prefixes
-           used in the CSS selector to namespace URIs. By default,
-           Beautiful Soup will use the prefixes it encountered while
-           parsing the document.
+    """
+    Base class for sparse traversals, where only certain node types are of
+    interest.  When ``visit_...`` & ``depart_...`` methods should be
+    implemented for *all* node types (such as for `docutils.writers.Writer`
+    subclasses), subclass `NodeVisitor` instead.
+    """
 
-        :param kwargs: Keyword arguments to be passed into Soup Sieve's
-           soupsieve.select() method.
 
-        :return: A Tag.
-        :rtype: bs4.element.Tag
-        """
-        return self.css.select_one(selector, namespaces, **kwargs)
+class GenericNodeVisitor(NodeVisitor):
 
-    def select(self, selector, namespaces=None, limit=None, **kwargs):
-        """Perform a CSS selection operation on the current element.
+    """
+    Generic "Visitor" abstract superclass, for simple traversals.
 
-        This uses the SoupSieve library.
+    Unless overridden, each ``visit_...`` method calls `default_visit()`, and
+    each ``depart_...`` method (when using `Node.walkabout()`) calls
+    `default_departure()`. `default_visit()` (and `default_departure()`) must
+    be overridden in subclasses.
+
+    Define fully generic visitors by overriding `default_visit()` (and
+    `default_departure()`) only. Define semi-generic visitors by overriding
+    individual ``visit_...()`` (and ``depart_...()``) methods also.
 
-        :param selector: A string containing a CSS selector.
+    `NodeVisitor.unknown_visit()` (`NodeVisitor.unknown_departure()`) should
+    be overridden for default behavior.
+    """
 
-        :param namespaces: A dictionary mapping namespace prefixes
-           used in the CSS selector to namespace URIs. By default,
-           Beautiful Soup will use the prefixes it encountered while
-           parsing the document.
+    def default_visit(self, node):
+        """Override for generic, uniform traversals."""
+        raise NotImplementedError
 
-        :param limit: After finding this number of results, stop looking.
+    def default_departure(self, node):
+        """Override for generic, uniform traversals."""
+        raise NotImplementedError
 
-        :param kwargs: Keyword arguments to be passed into SoupSieve's
-           soupsieve.select() method.
 
-        :return: A ResultSet of Tags.
-        :rtype: bs4.element.ResultSet
-        """
-        return self.css.select(selector, namespaces, limit, **kwargs)
+def _call_default_visit(self, node):
+    self.default_visit(node)
 
-    @property
-    def css(self):
-        """Return an interface to the CSS selector API."""
-        return CSS(self)
-
-    # Old names for backwards compatibility
-    def childGenerator(self):
-        """Deprecated generator."""
-        return self.children
-
-    def recursiveChildGenerator(self):
-        """Deprecated generator."""
-        return self.descendants
-
-    def has_key(self, key):
-        """Deprecated method. This was kind of misleading because has_key()
-        (attributes) was different from __in__ (contents).
-
-        has_key() is gone in Python 3, anyway.
-        """
-        warnings.warn(
-            'has_key is deprecated. Use has_attr(key) instead.',
-            DeprecationWarning, stacklevel=2
-        )
-        return self.has_attr(key)
-
-# Next, a couple classes to represent queries and their results.
-class SoupStrainer(object):
-    """Encapsulates a number of ways of matching a markup element (tag or
-    string).
-
-    This is primarily used to underpin the find_* methods, but you can
-    create one yourself and pass it in as `parse_only` to the
-    `BeautifulSoup` constructor, to parse a subset of a large
-    document.
-    """
-
-    def __init__(self, name=None, attrs={}, string=None, **kwargs):
-        """Constructor.
-
-        The SoupStrainer constructor takes the same arguments passed
-        into the find_* methods. See the online documentation for
-        detailed explanations.
-
-        :param name: A filter on tag name.
-        :param attrs: A dictionary of filters on attribute values.
-        :param string: A filter for a NavigableString with specific text.
-        :kwargs: A dictionary of filters on attribute values.
-        """
-        if string is None and 'text' in kwargs:
-            string = kwargs.pop('text')
-            warnings.warn(
-                "The 'text' argument to the SoupStrainer constructor is deprecated. Use 'string' instead.",
-                DeprecationWarning, stacklevel=2
-            )
-
-        self.name = self._normalize_search_value(name)
-        if not isinstance(attrs, dict):
-            # Treat a non-dict value for attrs as a search for the 'class'
-            # attribute.
-            kwargs['class'] = attrs
-            attrs = None
-
-        if 'class_' in kwargs:
-            # Treat class_="foo" as a search for the 'class'
-            # attribute, overriding any non-dict value for attrs.
-            kwargs['class'] = kwargs['class_']
-            del kwargs['class_']
-
-        if kwargs:
-            if attrs:
-                attrs = attrs.copy()
-                attrs.update(kwargs)
-            else:
-                attrs = kwargs
-        normalized_attrs = {}
-        for key, value in list(attrs.items()):
-            normalized_attrs[key] = self._normalize_search_value(value)
-
-        self.attrs = normalized_attrs
-        self.string = self._normalize_search_value(string)
-
-        # DEPRECATED but just in case someone is checking this.
-        self.text = self.string
-
-    def _normalize_search_value(self, value):
-        # Leave it alone if it's a Unicode string, a callable, a
-        # regular expression, a boolean, or None.
-        if (isinstance(value, str) or isinstance(value, Callable) or hasattr(value, 'match')
-            or isinstance(value, bool) or value is None):
-            return value
-
-        # If it's a bytestring, convert it to Unicode, treating it as UTF-8.
-        if isinstance(value, bytes):
-            return value.decode("utf8")
-
-        # If it's listlike, convert it into a list of strings.
-        if hasattr(value, '__iter__'):
-            new_value = []
-            for v in value:
-                if (hasattr(v, '__iter__') and not isinstance(v, bytes)
-                    and not isinstance(v, str)):
-                    # This is almost certainly the user's mistake. In the
-                    # interests of avoiding infinite loops, we'll let
-                    # it through as-is rather than doing a recursive call.
-                    new_value.append(v)
-                else:
-                    new_value.append(self._normalize_search_value(v))
-            return new_value
 
-        # Otherwise, convert it into a Unicode string.
-        # The unicode(str()) thing is so this will do the same thing on Python 2
-        # and Python 3.
-        return str(str(value))
+def _call_default_departure(self, node):
+    self.default_departure(node)
 
-    def __str__(self):
-        """A human-readable representation of this SoupStrainer."""
-        if self.string:
-            return self.string
-        else:
-            return "%s|%s" % (self.name, self.attrs)
 
-    def search_tag(self, markup_name=None, markup_attrs={}):
-        """Check whether a Tag with the given name and attributes would
-        match this SoupStrainer.
-
-        Used prospectively to decide whether to even bother creating a Tag
-        object.
-
-        :param markup_name: A tag name as found in some markup.
-        :param markup_attrs: A dictionary of attributes as found in some markup.
-
-        :return: True if the prospective tag would match this SoupStrainer;
-            False otherwise.
-        """
-        found = None
-        markup = None
-        if isinstance(markup_name, Tag):
-            markup = markup_name
-            markup_attrs = markup
-
-        if isinstance(self.name, str):
-            # Optimization for a very common case where the user is
-            # searching for a tag with one specific name, and we're
-            # looking at a tag with a different name.
-            if markup and not markup.prefix and self.name != markup.name:
-                 return False
-
-        call_function_with_tag_data = (
-            isinstance(self.name, Callable)
-            and not isinstance(markup_name, Tag))
-
-        if ((not self.name)
-            or call_function_with_tag_data
-            or (markup and self._matches(markup, self.name))
-            or (not markup and self._matches(markup_name, self.name))):
-            if call_function_with_tag_data:
-                match = self.name(markup_name, markup_attrs)
-            else:
-                match = True
-                markup_attr_map = None
-                for attr, match_against in list(self.attrs.items()):
-                    if not markup_attr_map:
-                        if hasattr(markup_attrs, 'get'):
-                            markup_attr_map = markup_attrs
-                        else:
-                            markup_attr_map = {}
-                            for k, v in markup_attrs:
-                                markup_attr_map[k] = v
-                    attr_value = markup_attr_map.get(attr)
-                    if not self._matches(attr_value, match_against):
-                        match = False
-                        break
-            if match:
-                if markup:
-                    found = markup
-                else:
-                    found = markup_name
-        if found and self.string and not self._matches(found.string, self.string):
-            found = None
-        return found
-
-    # For BS3 compatibility.
-    searchTag = search_tag
-
-    def search(self, markup):
-        """Find all items in `markup` that match this SoupStrainer.
-
-        Used by the core _find_all() method, which is ultimately
-        called by all find_* methods.
-
-        :param markup: A PageElement or a list of them.
-        """
-        # print('looking for %s in %s' % (self, markup))
-        found = None
-        # If given a list of items, scan it for a text element that
-        # matches.
-        if hasattr(markup, '__iter__') and not isinstance(markup, (Tag, str)):
-            for element in markup:
-                if isinstance(element, NavigableString) \
-                       and self.search(element):
-                    found = element
-                    break
-        # If it's a Tag, make sure its name or attributes match.
-        # Don't bother with Tags if we're searching for text.
-        elif isinstance(markup, Tag):
-            if not self.string or self.name or self.attrs:
-                found = self.search_tag(markup)
-        # If it's text, make sure the text matches.
-        elif isinstance(markup, NavigableString) or \
-                 isinstance(markup, str):
-            if not self.name and not self.attrs and self._matches(markup, self.string):
-                found = markup
-        else:
-            raise Exception(
-                "I don't know how to match against a %s" % markup.__class__)
-        return found
-
-    def _matches(self, markup, match_against, already_tried=None):
-        # print(u"Matching %s against %s" % (markup, match_against))
-        result = False
-        if isinstance(markup, list) or isinstance(markup, tuple):
-            # This should only happen when searching a multi-valued attribute
-            # like 'class'.
-            for item in markup:
-                if self._matches(item, match_against):
-                    return True
-            # We didn't match any particular value of the multivalue
-            # attribute, but maybe we match the attribute value when
-            # considered as a string.
-            if self._matches(' '.join(markup), match_against):
-                return True
-            return False
-
-        if match_against is True:
-            # True matches any non-None value.
-            return markup is not None
-
-        if isinstance(match_against, Callable):
-            return match_against(markup)
-
-        # Custom callables take the tag as an argument, but all
-        # other ways of matching match the tag name as a string.
-        original_markup = markup
-        if isinstance(markup, Tag):
-            markup = markup.name
-
-        # Ensure that `markup` is either a Unicode string, or None.
-        markup = self._normalize_search_value(markup)
-
-        if markup is None:
-            # None matches None, False, an empty string, an empty list, and so on.
-            return not match_against
-
-        if (hasattr(match_against, '__iter__')
-            and not isinstance(match_against, str)):
-            # We're asked to match against an iterable of items.
-            # The markup must be match at least one item in the
-            # iterable. We'll try each one in turn.
-            #
-            # To avoid infinite recursion we need to keep track of
-            # items we've already seen.
-            if not already_tried:
-                already_tried = set()
-            for item in match_against:
-                if item.__hash__:
-                    key = item
-                else:
-                    key = id(item)
-                if key in already_tried:
-                    continue
-                else:
-                    already_tried.add(key)
-                    if self._matches(original_markup, item, already_tried):
-                        return True
-            else:
-                return False
+def _nop(self, node):
+    pass
+
+
+def _add_node_class_names(names):
+    """Save typing with dynamic assignments:"""
+    for _name in names:
+        setattr(GenericNodeVisitor, "visit_" + _name, _call_default_visit)
+        setattr(GenericNodeVisitor, "depart_" + _name, _call_default_departure)
+        setattr(SparseNodeVisitor, 'visit_' + _name, _nop)
+        setattr(SparseNodeVisitor, 'depart_' + _name, _nop)
+
 
-        # Beyond this point we might need to run the test twice: once against
-        # the tag's name and once against its prefixed name.
-        match = False
-
-        if not match and isinstance(match_against, str):
-            # Exact string match
-            match = markup == match_against
-
-        if not match and hasattr(match_against, 'search'):
-            # Regexp match
-            return match_against.search(markup)
-
-        if (not match
-            and isinstance(original_markup, Tag)
-            and original_markup.prefix):
-            # Try the whole thing again with the prefixed tag name.
-            return self._matches(
-                original_markup.prefix + ':' + original_markup.name, match_against
-            )
-
-        return match
-
-
-class ResultSet(list):
-    """A ResultSet is just a list that keeps track of the SoupStrainer
-    that created it."""
-    def __init__(self, source, result=()):
-        """Constructor.
-
-        :param source: A SoupStrainer.
-        :param result: A list of PageElements.
-        """
-        super(ResultSet, self).__init__(result)
-        self.source = source
-
-    def __getattr__(self, key):
-        """Raise a helpful exception to explain a common code fix."""
-        raise AttributeError(
-            "ResultSet object has no attribute '%s'. You're probably treating a list of elements like a single element. Did you call find_all() when you meant to call find()?" % key
-        )
+_add_node_class_names(node_class_names)
+
+
+class TreeCopyVisitor(GenericNodeVisitor):
+
+    """
+    Make a complete copy of a tree or branch, including element attributes.
+    """
+
+    def __init__(self, document):
+        GenericNodeVisitor.__init__(self, document)
+        self.parent_stack = []
+        self.parent = []
+
+    def get_tree_copy(self):
+        return self.parent[0]
+
+    def default_visit(self, node):
+        """Copy the current node, and make it the new acting parent."""
+        newnode = node.copy()
+        self.parent.append(newnode)
+        self.parent_stack.append(self.parent)
+        self.parent = newnode
+
+    def default_departure(self, node):
+        """Restore the previous acting parent."""
+        self.parent = self.parent_stack.pop()
+
+
+class TreePruningException(Exception):
+
+    """
+    Base class for `NodeVisitor`-related tree pruning exceptions.
+
+    Raise subclasses from within ``visit_...`` or ``depart_...`` methods
+    called from `Node.walk()` and `Node.walkabout()` tree traversals to prune
+    the tree traversed.
+    """
+
+
+class SkipChildren(TreePruningException):
+
+    """
+    Do not visit any children of the current node.  The current node's
+    siblings and ``depart_...`` method are not affected.
+    """
+
+
+class SkipSiblings(TreePruningException):
+
+    """
+    Do not visit any more siblings (to the right) of the current node.  The
+    current node's children and its ``depart_...`` method are not affected.
+    """
+
+
+class SkipNode(TreePruningException):
+
+    """
+    Do not visit the current node's children, and do not call the current
+    node's ``depart_...`` method.
+    """
+
+
+class SkipDeparture(TreePruningException):
+
+    """
+    Do not call the current node's ``depart_...`` method.  The current node's
+    children and siblings are not affected.
+    """
+
+
+class NodeFound(TreePruningException):
+
+    """
+    Raise to indicate that the target of a search has been found.  This
+    exception must be caught by the client; it is not caught by the traversal
+    code.
+    """
+
+
+class StopTraversal(TreePruningException):
+
+    """
+    Stop the traversal altogether.  The current node's ``depart_...`` method
+    is not affected.  The parent nodes ``depart_...`` methods are also called
+    as usual.  No other nodes are visited.  This is an alternative to
+    NodeFound that does not cause exception handling to trickle up to the
+    caller.
+    """
+
+
+def make_id(string):
+    """
+    Convert `string` into an identifier and return it.
+
+    Docutils identifiers will conform to the regular expression
+    ``[a-z](-?[a-z0-9]+)*``.  For CSS compatibility, identifiers (the "class"
+    and "id" attributes) should have no underscores, colons, or periods.
+    Hyphens may be used.
+
+    - The `HTML 4.01 spec`_ defines identifiers based on SGML tokens:
+
+          ID and NAME tokens must begin with a letter ([A-Za-z]) and may be
+          followed by any number of letters, digits ([0-9]), hyphens ("-"),
+          underscores ("_"), colons (":"), and periods (".").
+
+    - However the `CSS1 spec`_ defines identifiers based on the "name" token,
+      a tighter interpretation ("flex" tokenizer notation; "latin1" and
+      "escape" 8-bit characters have been replaced with entities)::
+
+          unicode     \\[0-9a-f]{1,4}
+          latin1      [&iexcl;-&yuml;]
+          escape      {unicode}|\\[ -~&iexcl;-&yuml;]
+          nmchar      [-a-z0-9]|{latin1}|{escape}
+          name        {nmchar}+
+
+    The CSS1 "nmchar" rule does not include underscores ("_"), colons (":"),
+    or periods ("."), therefore "class" and "id" attributes should not contain
+    these characters. They should be replaced with hyphens ("-"). Combined
+    with HTML's requirements (the first character must be a letter; no
+    "unicode", "latin1", or "escape" characters), this results in the
+    ``[a-z](-?[a-z0-9]+)*`` pattern.
+
+    .. _HTML 4.01 spec: https://www.w3.org/TR/html401
+    .. _CSS1 spec: https://www.w3.org/TR/REC-CSS1
+    """
+    id = string.lower()
+    id = id.translate(_non_id_translate_digraphs)
+    id = id.translate(_non_id_translate)
+    # get rid of non-ascii characters.
+    # 'ascii' lowercase to prevent problems with turkish locale.
+    id = unicodedata.normalize(
+            'NFKD', id).encode('ascii', 'ignore').decode('ascii')
+    # shrink runs of whitespace and replace by hyphen
+    id = _non_id_chars.sub('-', ' '.join(id.split()))
+    id = _non_id_at_ends.sub('', id)
+    return str(id)
+
+
+_non_id_chars = re.compile('[^a-z0-9]+')
+_non_id_at_ends = re.compile('^[-0-9]+|-+$')
+_non_id_translate = {
+    0x00f8: 'o',       # o with stroke
+    0x0111: 'd',       # d with stroke
+    0x0127: 'h',       # h with stroke
+    0x0131: 'i',       # dotless i
+    0x0142: 'l',       # l with stroke
+    0x0167: 't',       # t with stroke
+    0x0180: 'b',       # b with stroke
+    0x0183: 'b',       # b with topbar
+    0x0188: 'c',       # c with hook
+    0x018c: 'd',       # d with topbar
+    0x0192: 'f',       # f with hook
+    0x0199: 'k',       # k with hook
+    0x019a: 'l',       # l with bar
+    0x019e: 'n',       # n with long right leg
+    0x01a5: 'p',       # p with hook
+    0x01ab: 't',       # t with palatal hook
+    0x01ad: 't',       # t with hook
+    0x01b4: 'y',       # y with hook
+    0x01b6: 'z',       # z with stroke
+    0x01e5: 'g',       # g with stroke
+    0x0225: 'z',       # z with hook
+    0x0234: 'l',       # l with curl
+    0x0235: 'n',       # n with curl
+    0x0236: 't',       # t with curl
+    0x0237: 'j',       # dotless j
+    0x023c: 'c',       # c with stroke
+    0x023f: 's',       # s with swash tail
+    0x0240: 'z',       # z with swash tail
+    0x0247: 'e',       # e with stroke
+    0x0249: 'j',       # j with stroke
+    0x024b: 'q',       # q with hook tail
+    0x024d: 'r',       # r with stroke
+    0x024f: 'y',       # y with stroke
+}
+_non_id_translate_digraphs = {
+    0x00df: 'sz',      # ligature sz
+    0x00e6: 'ae',      # ae
+    0x0153: 'oe',      # ligature oe
+    0x0238: 'db',      # db digraph
+    0x0239: 'qp',      # qp digraph
+}
+
+
+def dupname(node, name):
+    node['dupnames'].append(name)
+    node['names'].remove(name)
+    # Assume that this method is referenced, even though it isn't; we
+    # don't want to throw unnecessary system_messages.
+    node.referenced = 1
+
+
+def fully_normalize_name(name):
+    """Return a case- and whitespace-normalized name."""
+    return ' '.join(name.lower().split())
+
+
+def whitespace_normalize_name(name):
+    """Return a whitespace-normalized name."""
+    return ' '.join(name.split())
+
+
+def serial_escape(value):
+    """Escape string values that are elements of a list, for serialization."""
+    return value.replace('\\', r'\\').replace(' ', r'\ ')
+
+
+def pseudo_quoteattr(value):
+    """Quote attributes for pseudo-xml"""
+    return '"%s"' % value
```

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/bs4/builder/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/bleach/html5lib_shim.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,631 +1,741 @@
-# Use of this source code is governed by the MIT license.
-__license__ = "MIT"
+# flake8: noqa
+"""
+Shim module between Bleach and html5lib. This makes it easier to upgrade the
+html5lib library without having to change a lot of code.
+"""
 
-from collections import defaultdict
-import itertools
 import re
+import string
 import warnings
-import sys
-from bs4.element import (
-    CharsetMetaAttributeValue,
-    ContentMetaAttributeValue,
-    RubyParenthesisString,
-    RubyTextString,
-    Stylesheet,
-    Script,
-    TemplateString,
-    nonwhitespace_re
+
+# ignore html5lib deprecation warnings to use bleach; we are bleach
+# apply before we import submodules that import html5lib
+warnings.filterwarnings(
+    "ignore",
+    message="html5lib's sanitizer is deprecated",
+    category=DeprecationWarning,
+    module="bleach._vendor.html5lib",
+)
+
+from bleach._vendor.html5lib import (  # noqa: E402 module level import not at top of file
+    HTMLParser,
+    getTreeWalker,
+)
+from bleach._vendor.html5lib import (
+    constants,
+)  # noqa: E402 module level import not at top of file
+from bleach._vendor.html5lib.constants import (  # noqa: E402 module level import not at top of file
+    namespaces,
+    prefixes,
+)
+from bleach._vendor.html5lib.constants import (
+    _ReparseException as ReparseException,
+)  # noqa: E402 module level import not at top of file
+from bleach._vendor.html5lib.filters.base import (
+    Filter,
+)  # noqa: E402 module level import not at top of file
+from bleach._vendor.html5lib.filters.sanitizer import (
+    allowed_protocols,
+    allowed_css_properties,
+    allowed_svg_properties,
+    attr_val_is_uri,
+    svg_attr_val_allows_ref,
+    svg_allow_local_href,
+)  # noqa: E402 module level import not at top of file
+from bleach._vendor.html5lib.filters.sanitizer import (
+    Filter as SanitizerFilter,
+)  # noqa: E402 module level import not at top of file
+from bleach._vendor.html5lib._inputstream import (
+    HTMLInputStream,
+)  # noqa: E402 module level import not at top of file
+from bleach._vendor.html5lib.serializer import (
+    escape,
+    HTMLSerializer,
+)  # noqa: E402 module level import not at top of file
+from bleach._vendor.html5lib._tokenizer import (
+    attributeMap,
+    HTMLTokenizer,
+)  # noqa: E402 module level import not at top of file
+from bleach._vendor.html5lib._trie import (
+    Trie,
+)  # noqa: E402 module level import not at top of file
+
+
+#: Map of entity name to expanded entity
+ENTITIES = constants.entities
+
+#: Trie of html entity string -> character representation
+ENTITIES_TRIE = Trie(ENTITIES)
+
+#: Token type constants--these never change
+TAG_TOKEN_TYPES = {
+    constants.tokenTypes["StartTag"],
+    constants.tokenTypes["EndTag"],
+    constants.tokenTypes["EmptyTag"],
+}
+TAG_TOKEN_TYPE_START = constants.tokenTypes["StartTag"]
+TAG_TOKEN_TYPE_END = constants.tokenTypes["EndTag"]
+TAG_TOKEN_TYPE_CHARACTERS = constants.tokenTypes["Characters"]
+TAG_TOKEN_TYPE_PARSEERROR = constants.tokenTypes["ParseError"]
+
+
+#: List of valid HTML tags, from WHATWG HTML Living Standard as of 2018-10-17
+#: https://html.spec.whatwg.org/multipage/indices.html#elements-3
+HTML_TAGS = frozenset(
+    (
+        "a",
+        "abbr",
+        "address",
+        "area",
+        "article",
+        "aside",
+        "audio",
+        "b",
+        "base",
+        "bdi",
+        "bdo",
+        "blockquote",
+        "body",
+        "br",
+        "button",
+        "canvas",
+        "caption",
+        "cite",
+        "code",
+        "col",
+        "colgroup",
+        "data",
+        "datalist",
+        "dd",
+        "del",
+        "details",
+        "dfn",
+        "dialog",
+        "div",
+        "dl",
+        "dt",
+        "em",
+        "embed",
+        "fieldset",
+        "figcaption",
+        "figure",
+        "footer",
+        "form",
+        "h1",
+        "h2",
+        "h3",
+        "h4",
+        "h5",
+        "h6",
+        "head",
+        "header",
+        "hgroup",
+        "hr",
+        "html",
+        "i",
+        "iframe",
+        "img",
+        "input",
+        "ins",
+        "kbd",
+        "keygen",
+        "label",
+        "legend",
+        "li",
+        "link",
+        "map",
+        "mark",
+        "menu",
+        "meta",
+        "meter",
+        "nav",
+        "noscript",
+        "object",
+        "ol",
+        "optgroup",
+        "option",
+        "output",
+        "p",
+        "param",
+        "picture",
+        "pre",
+        "progress",
+        "q",
+        "rp",
+        "rt",
+        "ruby",
+        "s",
+        "samp",
+        "script",
+        "section",
+        "select",
+        "slot",
+        "small",
+        "source",
+        "span",
+        "strong",
+        "style",
+        "sub",
+        "summary",
+        "sup",
+        "table",
+        "tbody",
+        "td",
+        "template",
+        "textarea",
+        "tfoot",
+        "th",
+        "thead",
+        "time",
+        "title",
+        "tr",
+        "track",
+        "u",
+        "ul",
+        "var",
+        "video",
+        "wbr",
+    )
+)
+
+
+#: List of block level HTML tags, as per https://github.com/mozilla/bleach/issues/369
+#: from mozilla on 2019.07.11
+#: https://developer.mozilla.org/en-US/docs/Web/HTML/Block-level_elements#Elements
+HTML_TAGS_BLOCK_LEVEL = frozenset(
+    (
+        "address",
+        "article",
+        "aside",
+        "blockquote",
+        "details",
+        "dialog",
+        "dd",
+        "div",
+        "dl",
+        "dt",
+        "fieldset",
+        "figcaption",
+        "figure",
+        "footer",
+        "form",
+        "h1",
+        "h2",
+        "h3",
+        "h4",
+        "h5",
+        "h6",
+        "header",
+        "hgroup",
+        "hr",
+        "li",
+        "main",
+        "nav",
+        "ol",
+        "p",
+        "pre",
+        "section",
+        "table",
+        "ul",
+    )
 )
 
-__all__ = [
-    'HTMLTreeBuilder',
-    'SAXTreeBuilder',
-    'TreeBuilder',
-    'TreeBuilderRegistry',
-    ]
-
-# Some useful features for a TreeBuilder to have.
-FAST = 'fast'
-PERMISSIVE = 'permissive'
-STRICT = 'strict'
-XML = 'xml'
-HTML = 'html'
-HTML_5 = 'html5'
-
-class XMLParsedAsHTMLWarning(UserWarning):
-    """The warning issued when an HTML parser is used to parse
-    XML that is not XHTML.
-    """
-    MESSAGE = """It looks like you're parsing an XML document using an HTML parser. If this really is an HTML document (maybe it's XHTML?), you can ignore or filter this warning. If it's XML, you should know that using an XML parser will be more reliable. To parse this document as XML, make sure you have the lxml package installed, and pass the keyword argument `features="xml"` into the BeautifulSoup constructor."""
 
+class InputStreamWithMemory:
+    """Wraps an HTMLInputStream to remember characters since last <
+
+    This wraps existing HTMLInputStream classes to keep track of the stream
+    since the last < which marked an open tag state.
 
-class TreeBuilderRegistry(object):
-    """A way of looking up TreeBuilder subclasses by their name or by desired
-    features.
     """
-    
-    def __init__(self):
-        self.builders_for_feature = defaultdict(list)
-        self.builders = []
 
-    def register(self, treebuilder_class):
-        """Register a treebuilder based on its advertised features.
+    def __init__(self, inner_stream):
+        self._inner_stream = inner_stream
+        self.reset = self._inner_stream.reset
+        self.position = self._inner_stream.position
+        self._buffer = []
+
+    @property
+    def errors(self):
+        return self._inner_stream.errors
+
+    @property
+    def charEncoding(self):
+        return self._inner_stream.charEncoding
+
+    @property
+    def changeEncoding(self):
+        return self._inner_stream.changeEncoding
+
+    def char(self):
+        c = self._inner_stream.char()
+        # char() can return None if EOF, so ignore that
+        if c:
+            self._buffer.append(c)
+        return c
+
+    def charsUntil(self, characters, opposite=False):
+        chars = self._inner_stream.charsUntil(characters, opposite=opposite)
+        self._buffer.extend(list(chars))
+        return chars
+
+    def unget(self, char):
+        if self._buffer:
+            self._buffer.pop(-1)
+        return self._inner_stream.unget(char)
+
+    def get_tag(self):
+        """Returns the stream history since last '<'
+
+        Since the buffer starts at the last '<' as as seen by tagOpenState(),
+        we know that everything from that point to when this method is called
+        is the "tag" that is being tokenized.
+
+        """
+        return "".join(self._buffer)
+
+    def start_tag(self):
+        """Resets stream history to just '<'
+
+        This gets called by tagOpenState() which marks a '<' that denotes an
+        open tag. Any time we see that, we reset the buffer.
+
+        """
+        self._buffer = ["<"]
+
+
+class BleachHTMLTokenizer(HTMLTokenizer):
+    """Tokenizer that doesn't consume character entities"""
+
+    def __init__(self, consume_entities=False, **kwargs):
+        super().__init__(**kwargs)
+
+        self.consume_entities = consume_entities
+
+        # Wrap the stream with one that remembers the history
+        self.stream = InputStreamWithMemory(self.stream)
+
+        # Remember the last token emitted; needed for block element spacing
+        self.emitted_last_token = None
+
+    def __iter__(self):
+        last_error_token = None
+
+        for token in super().__iter__():
+            if last_error_token is not None:
+                if (
+                    last_error_token["data"] == "invalid-character-in-attribute-name"
+                    and token["type"] in TAG_TOKEN_TYPES
+                    and token.get("data")
+                ):
+                    # token["data"] is an html5lib attributeMap
+                    # (OrderedDict 3.7+ and dict otherwise)
+                    # of attr name to attr value
+                    #
+                    # Remove attribute names that have ', " or < in them
+                    # because those characters are invalid for attribute names.
+                    token["data"] = attributeMap(
+                        (attr_name, attr_value)
+                        for attr_name, attr_value in token["data"].items()
+                        if (
+                            '"' not in attr_name
+                            and "'" not in attr_name
+                            and "<" not in attr_name
+                        )
+                    )
+                    last_error_token = None
+                    yield token
+
+                elif (
+                    last_error_token["data"] == "expected-closing-tag-but-got-char"
+                    and self.parser.tags is not None
+                    and token["data"].lower().strip() not in self.parser.tags
+                ):
+                    # We've got either a malformed tag or a pseudo-tag or
+                    # something that html5lib wants to turn into a malformed
+                    # comment which Bleach clean() will drop so we interfere
+                    # with the token stream to handle it more correctly.
+                    #
+                    # If this is an allowed tag, it's malformed and we just let
+                    # the html5lib parser deal with it--we don't enter into this
+                    # block.
+                    #
+                    # If this is not an allowed tag, then we convert it to
+                    # characters and it'll get escaped in the sanitizer.
+                    token["data"] = self.stream.get_tag()
+                    token["type"] = TAG_TOKEN_TYPE_CHARACTERS
+
+                    last_error_token = None
+                    yield token
+
+                elif token["type"] == TAG_TOKEN_TYPE_PARSEERROR:
+                    # If the token is a parse error, then let the last_error_token
+                    # go, and make token the new last_error_token
+                    yield last_error_token
+                    last_error_token = token
 
-        :param treebuilder_class: A subclass of Treebuilder. its .features
-           attribute should list its features.
-        """
-        for feature in treebuilder_class.features:
-            self.builders_for_feature[feature].insert(0, treebuilder_class)
-        self.builders.insert(0, treebuilder_class)
-
-    def lookup(self, *features):
-        """Look up a TreeBuilder subclass with the desired features.
-
-        :param features: A list of features to look for. If none are
-            provided, the most recently registered TreeBuilder subclass
-            will be used.
-        :return: A TreeBuilder subclass, or None if there's no
-            registered subclass with all the requested features.
-        """
-        if len(self.builders) == 0:
-            # There are no builders at all.
-            return None
+                else:
+                    yield last_error_token
+                    yield token
+                    last_error_token = None
+
+                continue
+
+            # If the token is a ParseError, we hold on to it so we can get the
+            # next token and potentially fix it.
+            if token["type"] == TAG_TOKEN_TYPE_PARSEERROR:
+                last_error_token = token
+                continue
+
+            yield token
+
+        if last_error_token:
+            if last_error_token["data"] == "eof-in-tag-name":
+                # Handle the case where the text being parsed ends with <
+                # followed by a series of characters. It's treated as a tag
+                # name that abruptly ends, but we should treat that like
+                # character data
+                yield {
+                    "type": TAG_TOKEN_TYPE_CHARACTERS,
+                    "data": "<" + self.currentToken["name"],
+                }
+            else:
+                yield last_error_token
+
+    def consumeEntity(self, allowedChar=None, fromAttribute=False):
+        # If this tokenizer is set to consume entities, then we can let the
+        # superclass do its thing.
+        if self.consume_entities:
+            return super().consumeEntity(allowedChar, fromAttribute)
+
+        # If this tokenizer is set to not consume entities, then we don't want
+        # to consume and convert them, so this overrides the html5lib tokenizer's
+        # consumeEntity so that it's now a no-op.
+        #
+        # However, when that gets called, it's consumed an &, so we put that back in
+        # the stream.
+        if fromAttribute:
+            self.currentToken["data"][-1][1] += "&"
+
+        else:
+            self.tokenQueue.append({"type": TAG_TOKEN_TYPE_CHARACTERS, "data": "&"})
 
-        if len(features) == 0:
-            # They didn't ask for any features. Give them the most
-            # recently registered builder.
-            return self.builders[0]
-
-        # Go down the list of features in order, and eliminate any builders
-        # that don't match every feature.
-        features = list(features)
-        features.reverse()
-        candidates = None
-        candidate_set = None
-        while len(features) > 0:
-            feature = features.pop()
-            we_have_the_feature = self.builders_for_feature.get(feature, [])
-            if len(we_have_the_feature) > 0:
-                if candidates is None:
-                    candidates = we_have_the_feature
-                    candidate_set = set(candidates)
+    def tagOpenState(self):
+        # This state marks a < that is either a StartTag, EndTag, EmptyTag,
+        # or ParseError. In all cases, we want to drop any stream history
+        # we've collected so far and we do that by calling start_tag() on
+        # the input stream wrapper.
+        self.stream.start_tag()
+        return super().tagOpenState()
+
+    def emitCurrentToken(self):
+        token = self.currentToken
+
+        if (
+            self.parser.tags is not None
+            and token["type"] in TAG_TOKEN_TYPES
+            and token["name"].lower() not in self.parser.tags
+        ):
+            # If this is a start/end/empty tag for a tag that's not in our
+            # allowed list, then it gets stripped or escaped. In both of these
+            # cases it gets converted to a Characters token.
+            if self.parser.strip:
+                if (
+                    self.emitted_last_token
+                    and token["type"] == TAG_TOKEN_TYPE_START
+                    and token["name"].lower() in HTML_TAGS_BLOCK_LEVEL
+                ):
+                    # If this is a block level tag we're stripping, we drop it
+                    # for a newline because that's what a browser would parse
+                    # it as
+                    new_data = "\n"
                 else:
-                    # Eliminate any candidates that don't have this feature.
-                    candidate_set = candidate_set.intersection(
-                        set(we_have_the_feature))
-
-        # The only valid candidates are the ones in candidate_set.
-        # Go through the original list of candidates and pick the first one
-        # that's in candidate_set.
-        if candidate_set is None:
-            return None
-        for candidate in candidates:
-            if candidate in candidate_set:
-                return candidate
-        return None
+                    # For all other things being stripped, we throw in an empty
+                    # string token
+                    new_data = ""
+
+            else:
+                # If we're escaping the token, we want to escape the exact
+                # original string. Since tokenizing also normalizes data
+                # and this is a tag-like thing, we've lost some information.
+                # So we go back through the stream to get the original
+                # string and use that.
+                new_data = self.stream.get_tag()
+
+            new_token = {"type": TAG_TOKEN_TYPE_CHARACTERS, "data": new_data}
+
+            self.currentToken = self.emitted_last_token = new_token
+            self.tokenQueue.append(new_token)
+            self.state = self.dataState
+            return
 
-# The BeautifulSoup class will take feature lists from developers and use them
-# to look up builders in this registry.
-builder_registry = TreeBuilderRegistry()
-
-class TreeBuilder(object):
-    """Turn a textual document into a Beautiful Soup object tree."""
-
-    NAME = "[Unknown tree builder]"
-    ALTERNATE_NAMES = []
-    features = []
-
-    is_xml = False
-    picklable = False
-    empty_element_tags = None # A tag will be considered an empty-element
-                              # tag when and only when it has no contents.
-    
-    # A value for these tag/attribute combinations is a space- or
-    # comma-separated list of CDATA, rather than a single CDATA.
-    DEFAULT_CDATA_LIST_ATTRIBUTES = defaultdict(list)
-
-    # Whitespace should be preserved inside these tags.
-    DEFAULT_PRESERVE_WHITESPACE_TAGS = set()
-
-    # The textual contents of tags with these names should be
-    # instantiated with some class other than NavigableString.
-    DEFAULT_STRING_CONTAINERS = {}
-    
-    USE_DEFAULT = object()
-
-    # Most parsers don't keep track of line numbers.
-    TRACKS_LINE_NUMBERS = False
-    
-    def __init__(self, multi_valued_attributes=USE_DEFAULT,
-                 preserve_whitespace_tags=USE_DEFAULT,
-                 store_line_numbers=USE_DEFAULT,
-                 string_containers=USE_DEFAULT,
-    ):
-        """Constructor.
+        self.emitted_last_token = self.currentToken
+        super().emitCurrentToken()
 
-        :param multi_valued_attributes: If this is set to None, the
-         TreeBuilder will not turn any values for attributes like
-         'class' into lists. Setting this to a dictionary will
-         customize this behavior; look at DEFAULT_CDATA_LIST_ATTRIBUTES
-         for an example.
-
-         Internally, these are called "CDATA list attributes", but that
-         probably doesn't make sense to an end-user, so the argument name
-         is `multi_valued_attributes`.
-
-        :param preserve_whitespace_tags: A list of tags to treat
-         the way <pre> tags are treated in HTML. Tags in this list
-         are immune from pretty-printing; their contents will always be
-         output as-is.
-
-        :param string_containers: A dictionary mapping tag names to
-        the classes that should be instantiated to contain the textual
-        contents of those tags. The default is to use NavigableString
-        for every tag, no matter what the name. You can override the
-        default by changing DEFAULT_STRING_CONTAINERS.
-
-        :param store_line_numbers: If the parser keeps track of the
-         line numbers and positions of the original markup, that
-         information will, by default, be stored in each corresponding
-         `Tag` object. You can turn this off by passing
-         store_line_numbers=False. If the parser you're using doesn't 
-         keep track of this information, then setting store_line_numbers=True
-         will do nothing.
-        """
-        self.soup = None
-        if multi_valued_attributes is self.USE_DEFAULT:
-            multi_valued_attributes = self.DEFAULT_CDATA_LIST_ATTRIBUTES
-        self.cdata_list_attributes = multi_valued_attributes
-        if preserve_whitespace_tags is self.USE_DEFAULT:
-            preserve_whitespace_tags = self.DEFAULT_PRESERVE_WHITESPACE_TAGS
-        self.preserve_whitespace_tags = preserve_whitespace_tags
-        if store_line_numbers == self.USE_DEFAULT:
-            store_line_numbers = self.TRACKS_LINE_NUMBERS
-        self.store_line_numbers = store_line_numbers 
-        if string_containers == self.USE_DEFAULT:
-            string_containers = self.DEFAULT_STRING_CONTAINERS
-        self.string_containers = string_containers
-        
-    def initialize_soup(self, soup):
-        """The BeautifulSoup object has been initialized and is now
-        being associated with the TreeBuilder.
 
-        :param soup: A BeautifulSoup object.
-        """
-        self.soup = soup
-        
-    def reset(self):
-        """Do any work necessary to reset the underlying parser
-        for a new document.
+class BleachHTMLParser(HTMLParser):
+    """Parser that uses BleachHTMLTokenizer"""
 
-        By default, this does nothing.
+    def __init__(self, tags, strip, consume_entities, **kwargs):
         """
-        pass
-
-    def can_be_empty_element(self, tag_name):
-        """Might a tag with this name be an empty-element tag?
+        :arg tags: set of allowed tags--everything else is either stripped or
+            escaped; if None, then this doesn't look at tags at all
+        :arg strip: whether to strip disallowed tags (True) or escape them (False);
+            if tags=None, then this doesn't have any effect
+        :arg consume_entities: whether to consume entities (default behavior) or
+            leave them as is when tokenizing (BleachHTMLTokenizer-added behavior)
 
-        The final markup may or may not actually present this tag as
-        self-closing.
+        """
+        self.tags = (
+            frozenset((tag.lower() for tag in tags)) if tags is not None else None
+        )
+        self.strip = strip
+        self.consume_entities = consume_entities
+        super().__init__(**kwargs)
 
-        For instance: an HTMLBuilder does not consider a <p> tag to be
-        an empty-element tag (it's not in
-        HTMLBuilder.empty_element_tags). This means an empty <p> tag
-        will be presented as "<p></p>", not "<p/>" or "<p>".
-
-        The default implementation has no opinion about which tags are
-        empty-element tags, so a tag will be presented as an
-        empty-element tag if and only if it has no children.
-        "<foo></foo>" will become "<foo/>", and "<foo>bar</foo>" will
-        be left alone.
+    def _parse(
+        self, stream, innerHTML=False, container="div", scripting=True, **kwargs
+    ):
+        # set scripting=True to parse <noscript> as though JS is enabled to
+        # match the expected context in browsers
+        #
+        # https://html.spec.whatwg.org/multipage/scripting.html#the-noscript-element
+        #
+        # Override HTMLParser so we can swap out the tokenizer for our own.
+        self.innerHTMLMode = innerHTML
+        self.container = container
+        self.scripting = scripting
+        self.tokenizer = BleachHTMLTokenizer(
+            stream=stream, consume_entities=self.consume_entities, parser=self, **kwargs
+        )
+        self.reset()
 
-        :param tag_name: The name of a markup tag.
-        """
-        if self.empty_element_tags is None:
-            return True
-        return tag_name in self.empty_element_tags
-    
-    def feed(self, markup):
-        """Run some incoming markup through some parsing process,
-        populating the `BeautifulSoup` object in self.soup.
+        try:
+            self.mainLoop()
+        except ReparseException:
+            self.reset()
+            self.mainLoop()
 
-        This method is not implemented in TreeBuilder; it must be
-        implemented in subclasses.
 
-        :return: None.
-        """
-        raise NotImplementedError()
+def convert_entity(value):
+    """Convert an entity (minus the & and ; part) into what it represents
 
-    def prepare_markup(self, markup, user_specified_encoding=None,
-                       document_declared_encoding=None, exclude_encodings=None):
-        """Run any preliminary steps necessary to make incoming markup
-        acceptable to the parser.
-
-        :param markup: Some markup -- probably a bytestring.
-        :param user_specified_encoding: The user asked to try this encoding.
-        :param document_declared_encoding: The markup itself claims to be
-            in this encoding. NOTE: This argument is not used by the
-            calling code and can probably be removed.
-        :param exclude_encodings: The user asked _not_ to try any of
-            these encodings.
-
-        :yield: A series of 4-tuples:
-         (markup, encoding, declared encoding,
-          has undergone character replacement)
-
-         Each 4-tuple represents a strategy for converting the
-         document to Unicode and parsing it. Each strategy will be tried 
-         in turn.
-
-         By default, the only strategy is to parse the markup
-         as-is. See `LXMLTreeBuilderForXML` and
-         `HTMLParserTreeBuilder` for implementations that take into
-         account the quirks of particular parsers.
-        """
-        yield markup, None, None, False
+    This handles numeric, hex, and text entities.
 
-    def test_fragment_to_document(self, fragment):
-        """Wrap an HTML fragment to make it look like a document.
+    :arg value: the string (minus the ``&`` and ``;`` part) to convert
 
-        Different parsers do this differently. For instance, lxml
-        introduces an empty <head> tag, and html5lib
-        doesn't. Abstracting this away lets us write simple tests
-        which run HTML fragments through the parser and compare the
-        results against other HTML fragments.
+    :returns: unicode character or None if it's an ambiguous ampersand that
+        doesn't match a character entity
 
-        This method should not be used outside of tests.
+    """
+    if value[0] == "#":
+        if len(value) < 2:
+            return None
 
-        :param fragment: A string -- fragment of HTML.
-        :return: A string -- a full HTML document.
-        """
-        return fragment
+        if value[1] in ("x", "X"):
+            # hex-encoded code point
+            int_as_string, base = value[2:], 16
+        else:
+            # decimal code point
+            int_as_string, base = value[1:], 10
 
-    def set_up_substitutions(self, tag):
-        """Set up any substitutions that will need to be performed on 
-        a `Tag` when it's output as a string.
+        if int_as_string == "":
+            return None
 
-        By default, this does nothing. See `HTMLTreeBuilder` for a
-        case where this is used.
+        code_point = int(int_as_string, base)
+        if 0 < code_point < 0x110000:
+            return chr(code_point)
+        else:
+            return None
 
-        :param tag: A `Tag`
-        :return: Whether or not a substitution was performed.
-        """
-        return False
+    return ENTITIES.get(value, None)
 
-    def _replace_cdata_list_attribute_values(self, tag_name, attrs):
-        """When an attribute value is associated with a tag that can
-        have multiple values for that attribute, convert the string
-        value to a list of strings.
 
-        Basically, replaces class="foo bar" with class=["foo", "bar"]
+def convert_entities(text):
+    """Converts all found entities in the text
 
-        NOTE: This method modifies its input in place.
+    :arg text: the text to convert entities in
 
-        :param tag_name: The name of a tag.
-        :param attrs: A dictionary containing the tag's attributes.
-           Any appropriate attribute values will be modified in place.
-        """
-        if not attrs:
-            return attrs
-        if self.cdata_list_attributes:
-            universal = self.cdata_list_attributes.get('*', [])
-            tag_specific = self.cdata_list_attributes.get(
-                tag_name.lower(), None)
-            for attr in list(attrs.keys()):
-                if attr in universal or (tag_specific and attr in tag_specific):
-                    # We have a "class"-type attribute whose string
-                    # value is a whitespace-separated list of
-                    # values. Split it into a list.
-                    value = attrs[attr]
-                    if isinstance(value, str):
-                        values = nonwhitespace_re.findall(value)
-                    else:
-                        # html5lib sometimes calls setAttributes twice
-                        # for the same tag when rearranging the parse
-                        # tree. On the second call the attribute value
-                        # here is already a list.  If this happens,
-                        # leave the value alone rather than trying to
-                        # split it again.
-                        values = value
-                    attrs[attr] = values
-        return attrs
-    
-class SAXTreeBuilder(TreeBuilder):
-    """A Beautiful Soup treebuilder that listens for SAX events.
+    :returns: unicode text with converted entities
 
-    This is not currently used for anything, but it demonstrates
-    how a simple TreeBuilder would work.
     """
+    if "&" not in text:
+        return text
 
-    def feed(self, markup):
-        raise NotImplementedError()
+    new_text = []
+    for part in next_possible_entity(text):
+        if not part:
+            continue
 
-    def close(self):
-        pass
+        if part.startswith("&"):
+            entity = match_entity(part)
+            if entity is not None:
+                converted = convert_entity(entity)
 
-    def startElement(self, name, attrs):
-        attrs = dict((key[1], value) for key, value in list(attrs.items()))
-        #print("Start %s, %r" % (name, attrs))
-        self.soup.handle_starttag(name, attrs)
+                # If it's not an ambiguous ampersand, then replace with the
+                # unicode character. Otherwise, we leave the entity in.
+                if converted is not None:
+                    new_text.append(converted)
+                    remainder = part[len(entity) + 2 :]
+                    if part:
+                        new_text.append(remainder)
+                    continue
 
-    def endElement(self, name):
-        #print("End %s" % name)
-        self.soup.handle_endtag(name)
+        new_text.append(part)
 
-    def startElementNS(self, nsTuple, nodeName, attrs):
-        # Throw away (ns, nodeName) for now.
-        self.startElement(nodeName, attrs)
+    return "".join(new_text)
 
-    def endElementNS(self, nsTuple, nodeName):
-        # Throw away (ns, nodeName) for now.
-        self.endElement(nodeName)
-        #handler.endElementNS((ns, node.nodeName), node.nodeName)
 
-    def startPrefixMapping(self, prefix, nodeValue):
-        # Ignore the prefix for now.
-        pass
+def match_entity(stream):
+    """Returns first entity in stream or None if no entity exists
 
-    def endPrefixMapping(self, prefix):
-        # Ignore the prefix for now.
-        # handler.endPrefixMapping(prefix)
-        pass
+    Note: For Bleach purposes, entities must start with a "&" and end with a
+    ";". This ignores ambiguous character entities that have no ";" at the end.
 
-    def characters(self, content):
-        self.soup.handle_data(content)
+    :arg stream: the character stream
 
-    def startDocument(self):
-        pass
+    :returns: the entity string without "&" or ";" if it's a valid character
+        entity; ``None`` otherwise
 
-    def endDocument(self):
-        pass
+    """
+    # Nix the & at the beginning
+    if stream[0] != "&":
+        raise ValueError('Stream should begin with "&"')
+
+    stream = stream[1:]
+
+    stream = list(stream)
+    possible_entity = ""
+    end_characters = "<&=;" + string.whitespace
+
+    # Handle number entities
+    if stream and stream[0] == "#":
+        possible_entity = "#"
+        stream.pop(0)
+
+        if stream and stream[0] in ("x", "X"):
+            allowed = "0123456789abcdefABCDEF"
+            possible_entity += stream.pop(0)
+        else:
+            allowed = "0123456789"
 
+        # FIXME(willkg): Do we want to make sure these are valid number
+        # entities? This doesn't do that currently.
+        while stream and stream[0] not in end_characters:
+            c = stream.pop(0)
+            if c not in allowed:
+                break
+            possible_entity += c
 
-class HTMLTreeBuilder(TreeBuilder):
-    """This TreeBuilder knows facts about HTML.
+        if possible_entity and stream and stream[0] == ";":
+            return possible_entity
+        return None
 
-    Such as which tags are empty-element tags.
-    """
+    # Handle character entities
+    while stream and stream[0] not in end_characters:
+        c = stream.pop(0)
+        possible_entity += c
+        if not ENTITIES_TRIE.has_keys_with_prefix(possible_entity):
+            # If it's not a prefix, then it's not an entity and we're
+            # out
+            return None
 
-    empty_element_tags = set([
-        # These are from HTML5.
-        'area', 'base', 'br', 'col', 'embed', 'hr', 'img', 'input', 'keygen', 'link', 'menuitem', 'meta', 'param', 'source', 'track', 'wbr',
-        
-        # These are from earlier versions of HTML and are removed in HTML5.
-        'basefont', 'bgsound', 'command', 'frame', 'image', 'isindex', 'nextid', 'spacer'
-    ])
-
-    # The HTML standard defines these as block-level elements. Beautiful
-    # Soup does not treat these elements differently from other elements,
-    # but it may do so eventually, and this information is available if
-    # you need to use it.
-    block_elements = set(["address", "article", "aside", "blockquote", "canvas", "dd", "div", "dl", "dt", "fieldset", "figcaption", "figure", "footer", "form", "h1", "h2", "h3", "h4", "h5", "h6", "header", "hr", "li", "main", "nav", "noscript", "ol", "output", "p", "pre", "section", "table", "tfoot", "ul", "video"])
+    if possible_entity and stream and stream[0] == ";":
+        return possible_entity
 
-    # These HTML tags need special treatment so they can be
-    # represented by a string class other than NavigableString.
-    #
-    # For some of these tags, it's because the HTML standard defines
-    # an unusual content model for them. I made this list by going
-    # through the HTML spec
-    # (https://html.spec.whatwg.org/#metadata-content) and looking for
-    # "metadata content" elements that can contain strings.
-    #
-    # The Ruby tags (<rt> and <rp>) are here despite being normal
-    # "phrasing content" tags, because the content they contain is
-    # qualitatively different from other text in the document, and it
-    # can be useful to be able to distinguish it.
-    #
-    # TODO: Arguably <noscript> could go here but it seems
-    # qualitatively different from the other tags.
-    DEFAULT_STRING_CONTAINERS = {
-        'rt' : RubyTextString,
-        'rp' : RubyParenthesisString,
-        'style': Stylesheet,
-        'script': Script,
-        'template': TemplateString,
-    }    
-    
-    # The HTML standard defines these attributes as containing a
-    # space-separated list of values, not a single value. That is,
-    # class="foo bar" means that the 'class' attribute has two values,
-    # 'foo' and 'bar', not the single value 'foo bar'.  When we
-    # encounter one of these attributes, we will parse its value into
-    # a list of values if possible. Upon output, the list will be
-    # converted back into a string.
-    DEFAULT_CDATA_LIST_ATTRIBUTES = {
-        "*" : ['class', 'accesskey', 'dropzone'],
-        "a" : ['rel', 'rev'],
-        "link" :  ['rel', 'rev'],
-        "td" : ["headers"],
-        "th" : ["headers"],
-        "td" : ["headers"],
-        "form" : ["accept-charset"],
-        "object" : ["archive"],
-
-        # These are HTML5 specific, as are *.accesskey and *.dropzone above.
-        "area" : ["rel"],
-        "icon" : ["sizes"],
-        "iframe" : ["sandbox"],
-        "output" : ["for"],
-        }
-
-    DEFAULT_PRESERVE_WHITESPACE_TAGS = set(['pre', 'textarea'])
-
-    def set_up_substitutions(self, tag):
-        """Replace the declared encoding in a <meta> tag with a placeholder,
-        to be substituted when the tag is output to a string.
-
-        An HTML document may come in to Beautiful Soup as one
-        encoding, but exit in a different encoding, and the <meta> tag
-        needs to be changed to reflect this.
+    return None
 
-        :param tag: A `Tag`
-        :return: Whether or not a substitution was performed.
-        """
-        # We are only interested in <meta> tags
-        if tag.name != 'meta':
-            return False
-
-        http_equiv = tag.get('http-equiv')
-        content = tag.get('content')
-        charset = tag.get('charset')
-
-        # We are interested in <meta> tags that say what encoding the
-        # document was originally in. This means HTML 5-style <meta>
-        # tags that provide the "charset" attribute. It also means
-        # HTML 4-style <meta> tags that provide the "content"
-        # attribute and have "http-equiv" set to "content-type".
-        #
-        # In both cases we will replace the value of the appropriate
-        # attribute with a standin object that can take on any
-        # encoding.
-        meta_encoding = None
-        if charset is not None:
-            # HTML 5 style:
-            # <meta charset="utf8">
-            meta_encoding = charset
-            tag['charset'] = CharsetMetaAttributeValue(charset)
-
-        elif (content is not None and http_equiv is not None
-              and http_equiv.lower() == 'content-type'):
-            # HTML 4 style:
-            # <meta http-equiv="content-type" content="text/html; charset=utf8">
-            tag['content'] = ContentMetaAttributeValue(content)
-
-        return (meta_encoding is not None)
-
-class DetectsXMLParsedAsHTML(object):
-    """A mixin class for any class (a TreeBuilder, or some class used by a
-    TreeBuilder) that's in a position to detect whether an XML
-    document is being incorrectly parsed as HTML, and issue an
-    appropriate warning.
-
-    This requires being able to observe an incoming processing
-    instruction that might be an XML declaration, and also able to
-    observe tags as they're opened. If you can't do that for a given
-    TreeBuilder, there's a less reliable implementation based on
-    examining the raw markup.
-    """
 
-    # Regular expression for seeing if markup has an <html> tag.
-    LOOKS_LIKE_HTML = re.compile("<[^ +]html", re.I)
-    LOOKS_LIKE_HTML_B = re.compile(b"<[^ +]html", re.I)
-
-    XML_PREFIX = '<?xml'
-    XML_PREFIX_B = b'<?xml'
-    
-    @classmethod
-    def warn_if_markup_looks_like_xml(cls, markup):
-        """Perform a check on some markup to see if it looks like XML
-        that's not XHTML. If so, issue a warning.
+AMP_SPLIT_RE = re.compile("(&)")
 
-        This is much less reliable than doing the check while parsing,
-        but some of the tree builders can't do that.
 
-        :return: True if the markup looks like non-XHTML XML, False
-        otherwise.
-        """
-        if isinstance(markup, bytes):
-            prefix = cls.XML_PREFIX_B
-            looks_like_html = cls.LOOKS_LIKE_HTML_B
-        else:
-            prefix = cls.XML_PREFIX
-            looks_like_html = cls.LOOKS_LIKE_HTML
-        
-        if (markup is not None
-            and markup.startswith(prefix)
-            and not looks_like_html.search(markup[:500])
-        ):
-            cls._warn()
-            return True
-        return False
-
-    @classmethod
-    def _warn(cls):
-        """Issue a warning about XML being parsed as HTML."""
-        warnings.warn(
-            XMLParsedAsHTMLWarning.MESSAGE, XMLParsedAsHTMLWarning
-        )
-        
-    def _initialize_xml_detector(self):
-        """Call this method before parsing a document."""
-        self._first_processing_instruction = None
-        self._root_tag = None
-       
-    def _document_might_be_xml(self, processing_instruction):
-        """Call this method when encountering an XML declaration, or a
-        "processing instruction" that might be an XML declaration.
-        """
-        if (self._first_processing_instruction is not None
-            or self._root_tag is not None):
-            # The document has already started. Don't bother checking
-            # anymore.
-            return
+def next_possible_entity(text):
+    """Takes a text and generates a list of possible entities
 
-        self._first_processing_instruction = processing_instruction
+    :arg text: the text to look at
 
-        # We won't know until we encounter the first tag whether or
-        # not this is actually a problem.
-        
-    def _root_tag_encountered(self, name):
-        """Call this when you encounter the document's root tag.
+    :returns: generator where each part (except the first) starts with an
+        "&"
 
-        This is where we actually check whether an XML document is
-        being incorrectly parsed as HTML, and issue the warning.
-        """
-        if self._root_tag is not None:
-            # This method was incorrectly called multiple times. Do
-            # nothing.
-            return
+    """
+    for i, part in enumerate(AMP_SPLIT_RE.split(text)):
+        if i == 0:
+            yield part
+        elif i % 2 == 0:
+            yield "&" + part
 
-        self._root_tag = name
-        if (name != 'html' and self._first_processing_instruction is not None
-            and self._first_processing_instruction.lower().startswith('xml ')):
-            # We encountered an XML declaration and then a tag other
-            # than 'html'. This is a reliable indicator that a
-            # non-XHTML document is being parsed as XML.
-            self._warn()
-
-    
-def register_treebuilders_from(module):
-    """Copy TreeBuilders from the given module into this module."""
-    this_module = sys.modules[__name__]
-    for name in module.__all__:
-        obj = getattr(module, name)
-
-        if issubclass(obj, TreeBuilder):
-            setattr(this_module, name, obj)
-            this_module.__all__.append(name)
-            # Register the builder while we're at it.
-            this_module.builder_registry.register(obj)
-
-class ParserRejectedMarkup(Exception):
-    """An Exception to be raised when the underlying parser simply
-    refuses to parse the given markup.
+
+class BleachHTMLSerializer(HTMLSerializer):
+    """HTMLSerializer that undoes & -> &amp; in attributes and sets
+    escape_rcdata to True
     """
-    def __init__(self, message_or_exception):
-        """Explain why the parser rejected the given markup, either
-        with a textual explanation or another exception.
-        """
-        if isinstance(message_or_exception, Exception):
-            e = message_or_exception
-            message_or_exception = "%s: %s" % (e.__class__.__name__, str(e))
-        super(ParserRejectedMarkup, self).__init__(message_or_exception)
-            
-# Builders are registered in reverse order of priority, so that custom
-# builder registrations will take precedence. In general, we want lxml
-# to take precedence over html5lib, because it's faster. And we only
-# want to use HTMLParser as a last resort.
-from . import _htmlparser
-register_treebuilders_from(_htmlparser)
-try:
-    from . import _html5lib
-    register_treebuilders_from(_html5lib)
-except ImportError:
-    # They don't have html5lib installed.
-    pass
-try:
-    from . import _lxml
-    register_treebuilders_from(_lxml)
-except ImportError:
-    # They don't have lxml installed.
-    pass
+
+    # per the HTMLSerializer.__init__ docstring:
+    #
+    # Whether to escape characters that need to be
+    # escaped within normal elements within rcdata elements such as
+    # style.
+    #
+    escape_rcdata = True
+
+    def escape_base_amp(self, stoken):
+        """Escapes just bare & in HTML attribute values"""
+        # First, undo escaping of &. We need to do this because html5lib's
+        # HTMLSerializer expected the tokenizer to consume all the character
+        # entities and convert them to their respective characters, but the
+        # BleachHTMLTokenizer doesn't do that. For example, this fixes
+        # &amp;entity; back to &entity; .
+        stoken = stoken.replace("&amp;", "&")
+
+        # However, we do want all bare & that are not marking character
+        # entities to be changed to &amp;, so let's do that carefully here.
+        for part in next_possible_entity(stoken):
+            if not part:
+                continue
+
+            if part.startswith("&"):
+                entity = match_entity(part)
+                # Only leave entities in that are not ambiguous. If they're
+                # ambiguous, then we escape the ampersand.
+                if entity is not None and convert_entity(entity) is not None:
+                    yield f"&{entity};"
+
+                    # Length of the entity plus 2--one for & at the beginning
+                    # and one for ; at the end
+                    part = part[len(entity) + 2 :]
+                    if part:
+                        yield part
+                    continue
+
+            yield part.replace("&", "&amp;")
+
+    def serialize(self, treewalker, encoding=None):
+        """Wrap HTMLSerializer.serialize and conver & to &amp; in attribute values
+
+        Note that this converts & to &amp; in attribute values where the & isn't
+        already part of an unambiguous character entity.
+
+        """
+        in_tag = False
+        after_equals = False
+
+        for stoken in super().serialize(treewalker, encoding):
+            if in_tag:
+                if stoken == ">":
+                    in_tag = False
+
+                elif after_equals:
+                    if stoken != '"':
+                        yield from self.escape_base_amp(stoken)
+
+                        after_equals = False
+                        continue
+
+                elif stoken == "=":
+                    after_equals = True
+
+                yield stoken
+            else:
+                if stoken.startswith("<"):
+                    in_tag = True
+                yield stoken
```

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/certifi/cacert.pem` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/certifi/core.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/certifi/core.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/LICENSE` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/METADATA` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/RECORD` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/api.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/api.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/cd.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/cd.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/constant.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/constant.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/legacy.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/legacy.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/md.cpython-310-x86_64-linux-gnu.so` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/md.cpython-310-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/md.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/md.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/md__mypyc.cpython-310-x86_64-linux-gnu.so` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/md__mypyc.cpython-310-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/models.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/models.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/utils.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/utils.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/assets/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer/cli/normalizer.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer/cli/normalizer.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/LICENSE` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/METADATA` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/RECORD` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/hatch_project/scraping.py` & `hatch_project-0.2.0/src/hatch_project/scraping.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/hatch_project-0.1.1.dist-info/METADATA` & `hatch_project-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-project
-Version: 0.1.1
+Version: 0.2.0
 Project-URL: Documentation, https://github.com/unknown/hatch-project#readme
 Project-URL: Issues, https://github.com/unknown/hatch-project/issues
 Project-URL: Source, https://github.com/unknown/hatch-project
 Author-email: Kenno-Warise <wariken0523@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/hatch_project-0.1.1.dist-info/licenses/LICENSE.txt` & `hatch_project-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/idna/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/idna/codec.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/idna/codec.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/idna/core.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/idna/core.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/idna/idnadata.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/idna/intranges.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/idna/uts46data.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/idna-3.4.dist-info/LICENSE.md` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/idna-3.4.dist-info/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/idna-3.4.dist-info/METADATA` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/idna-3.4.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/idna-3.4.dist-info/RECORD` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/idna-3.4.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/__main__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/build_env.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/cache.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/configuration.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/exceptions.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/pyproject.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/self_outdated_check.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/wheel_builder.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/cli/autocompletion.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/cli/base_command.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/cli/cmdoptions.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/cli/command_context.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/cli/main.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/cli/main_parser.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/cli/parser.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/cli/progress_bars.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/cli/req_command.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/cli/spinners.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/cache.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/check.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/completion.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/configuration.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/debug.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/download.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/freeze.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/hash.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/help.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/index.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/install.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/list.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/search.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/show.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/uninstall.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/commands/wheel.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/distributions/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/distributions/base.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/distributions/installed.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/distributions/sdist.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/distributions/wheel.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/index/collector.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/index/package_finder.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/index/sources.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/locations/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/locations/_distutils.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/locations/_sysconfig.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/locations/base.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/metadata/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/metadata/base.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/models/candidate.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/models/direct_url.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/models/format_control.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/models/index.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/models/link.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/models/scheme.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/models/search_scope.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/models/selection_prefs.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/models/target_python.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/models/wheel.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/network/auth.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/network/cache.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/network/download.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/network/lazy_wheel.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/network/session.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/network/utils.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/network/xmlrpc.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/operations/check.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/operations/freeze.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/operations/prepare.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/operations/build/metadata.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/operations/build/wheel.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/operations/install/legacy.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/operations/install/legacy.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/operations/install/wheel.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/req/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/req/constructors.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/req/req_file.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/req/req_install.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/req/req_set.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/req/req_tracker.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/req/req_tracker.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/req/req_uninstall.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/resolution/base.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/_log.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/appdirs.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/compat.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/deprecation.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/distutils_args.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/distutils_args.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/encoding.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/entrypoints.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/filesystem.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/filetypes.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/glibc.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/hashes.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/inject_securetransport.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/logging.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/misc.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/models.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/packaging.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/parallel.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/pkg_resources.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/setuptools_build.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/subprocess.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/temp_dir.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/unpacking.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/urls.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/virtualenv.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/utils/wheel.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/vcs/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/vcs/bazaar.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/vcs/git.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/vcs/mercurial.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/vcs/subversion.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/appdirs.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distro.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distro.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pyparsing.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/six.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/compat.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/certifi/core.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/big5freq.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/big5prober.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/compat.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/compat.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/enums.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/escprober.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/escsm.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/colorama/ansi.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/colorama/initialise.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/colorama/win32.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/colorama/winterm.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/compat.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/database.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/index.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/locators.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/manifest.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/markers.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/metadata.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/resources.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/scripts.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/t32.exe` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/t32.exe`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/t64.exe` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/t64.exe`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/util.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/version.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/w32.exe` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/w32.exe`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/w64.exe` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/w64.exe`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/wheel.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/_backport/misc.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/_backport/misc.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/_backport/shutil.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/_backport/shutil.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/_backport/sysconfig.cfg` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/_backport/sysconfig.cfg`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/_backport/sysconfig.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/_backport/sysconfig.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/distlib/_backport/tarfile.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/distlib/_backport/tarfile.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_ihatexml.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_ihatexml.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_inputstream.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_inputstream.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_tokenizer.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_utils.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_utils.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/constants.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/constants.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/html5parser.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/html5parser.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/serializer.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/serializer.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_trie/_base.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_trie/_base.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_trie/py.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/_trie/py.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/inject_meta_charset.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/inject_meta_charset.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/lint.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/lint.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/optionaltags.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/optionaltags.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/sanitizer.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/sanitizer.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/whitespace.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/whitespace.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treeadapters/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treeadapters/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treeadapters/genshi.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treeadapters/genshi.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treeadapters/sax.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treeadapters/sax.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/base.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/base.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/dom.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/dom.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/etree.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/etree.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/base.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/base.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/dom.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/dom.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/etree.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/etree.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/genshi.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/genshi.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/idna/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/idna/codec.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/idna/core.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/idna/idnadata.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/idna/intranges.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/idna/uts46data.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/msgpack/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/msgpack/ext.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/msgpack/fallback.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/packaging/__about__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/packaging/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/packaging/_structures.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/packaging/markers.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/packaging/requirements.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/packaging/specifiers.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/packaging/tags.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/packaging/utils.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/packaging/version.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pep517/build.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pep517/build.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pep517/check.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pep517/check.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pep517/colorlog.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pep517/colorlog.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pep517/compat.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pep517/compat.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pep517/dirtools.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pep517/dirtools.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pep517/envbuild.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pep517/envbuild.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pep517/meta.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pep517/meta.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pep517/wrappers.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pep517/wrappers.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/_in_process.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/pkg_resources/py31compat.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/progress/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/progress/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/progress/bar.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/progress/bar.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/progress/counter.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/progress/counter.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/progress/spinner.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/progress/spinner.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/adapters.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/api.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/auth.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/compat.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/cookies.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/exceptions.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/help.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/hooks.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/models.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/packages.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/sessions.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/status_codes.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/structures.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/requests/utils.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/resolvelib/providers.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/resolvelib/structs.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/_utils.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/after.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/before.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/nap.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/retry.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/stop.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/wait.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tomli/_parser.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/tomli/_re.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/_collections.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/connection.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/fields.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/filepost.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/request.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/response.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/ssl_match_hostname/_implementation.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/queue.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/queue.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/request.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/response.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/url.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/webencodings/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/webencodings/labels.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/webencodings/tests.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip-21.2.3.dist-info/LICENSE.txt` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip-21.2.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip-21.2.3.dist-info/METADATA` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip-21.2.3.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pip-21.2.3.dist-info/RECORD` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pip-21.2.3.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/appdirs.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/pyparsing.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/__about__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_compat.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_compat.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_structures.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_typing.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_typing.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/markers.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/tags.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/utils.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/version.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/pkg_resources/extern/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/_internal_utils.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/adapters.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/api.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/api.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/auth.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/auth.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/compat.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/compat.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/cookies.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/exceptions.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/help.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/help.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/hooks.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/models.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/models.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/packages.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/packages.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/sessions.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/status_codes.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/structures.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/structures.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests/utils.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests/utils.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests-2.31.0.dist-info/LICENSE` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests-2.31.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests-2.31.0.dist-info/METADATA` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests-2.31.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/requests-2.31.0.dist-info/RECORD` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/requests-2.31.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_imp.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_imp.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/archive_util.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/archive_util.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/build_meta.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/cli-32.exe` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/cli-32.exe`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/cli-64.exe` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/cli-64.exe`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/cli.exe` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/cli.exe`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/config.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/config.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/dep_util.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/depends.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/depends.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/dist.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/dist.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/errors.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/errors.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/extension.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/glob.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/glob.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/gui-32.exe` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/gui-32.exe`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/gui-64.exe` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/gui-64.exe`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/gui.exe` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/gui.exe`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/installer.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/installer.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/launch.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/launch.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/lib2to3_ex.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/lib2to3_ex.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/monkey.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/monkey.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/msvc.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/msvc.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/namespaces.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/namespaces.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/package_index.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/package_index.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/sandbox.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/sandbox.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/unicode_utils.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/wheel.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/wheel.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/windows_support.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/_msvccompiler.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/_msvccompiler.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/archive_util.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/archive_util.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/bcppcompiler.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/bcppcompiler.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/ccompiler.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/ccompiler.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/cmd.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/cmd.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/config.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/config.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/core.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/core.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/cygwinccompiler.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/cygwinccompiler.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/dep_util.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/dep_util.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/dir_util.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/dir_util.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/dist.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/dist.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/errors.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/errors.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/extension.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/extension.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/fancy_getopt.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/fancy_getopt.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/file_util.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/file_util.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/filelist.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/filelist.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/log.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/log.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/msvc9compiler.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/msvccompiler.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/msvccompiler.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/spawn.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/spawn.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/sysconfig.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/sysconfig.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/text_file.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/text_file.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/unixccompiler.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/unixccompiler.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/util.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/util.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/version.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/version.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/versionpredicate.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/versionpredicate.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/bdist.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/bdist.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_dumb.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_dumb.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_msi.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_msi.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_rpm.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_wininst.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_wininst.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/build.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/build.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/build_clib.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/build_ext.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/build_py.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/build_py.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/build_scripts.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/build_scripts.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/check.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/check.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/clean.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/clean.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/config.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/config.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/install.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/install.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/install_data.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/install_data.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/install_egg_info.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/install_headers.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/install_headers.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/install_lib.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/install_scripts.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/py37compat.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/py37compat.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/register.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/register.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/sdist.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/sdist.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_distutils/command/upload.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_distutils/command/upload.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/ordered_set.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/ordered_set.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/pyparsing.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/more.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/__about__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/_compat.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/_compat.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/_structures.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/_typing.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/_typing.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/markers.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/requirements.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/specifiers.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/tags.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/utils.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/version.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/alias.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/alias.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/bdist_egg.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/bdist_rpm.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/build_clib.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/build_ext.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/build_py.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/build_py.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/develop.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/develop.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/dist_info.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/easy_install.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/easy_install.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/egg_info.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/install.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/install_egg_info.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/install_lib.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/install_scripts.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/launcher manifest.xml` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/py36compat.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/py36compat.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/rotate.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/rotate.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/saveopts.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/sdist.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/sdist.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/setopt.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/setopt.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/test.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/test.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/command/upload_docs.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools/extern/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools-57.4.0.dist-info/LICENSE` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/jaraco.classes-3.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools-57.4.0.dist-info/METADATA` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools-57.4.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools-57.4.0.dist-info/RECORD` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools-57.4.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/setuptools-57.4.0.dist-info/entry_points.txt` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/setuptools-57.4.0.dist-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/soupsieve-2.4.1.dist-info/licenses/LICENSE.md` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/markdown_it_py-3.0.0.dist-info/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018 - 2023 Isaac Muse <isaacmuse@gmail.com>
+Copyright (c) 2020 ExecutableBookProject
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/_base_connection.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/_base_connection.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/_collections.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/_request_methods.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/_request_methods.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/connection.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/connectionpool.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/exceptions.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/fields.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/filepost.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/poolmanager.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/response.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/contrib/pyopenssl.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/contrib/securetransport.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/contrib/socks.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/contrib/_securetransport/bindings.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/contrib/_securetransport/low_level.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/__init__.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/connection.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/proxy.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/request.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/response.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/retry.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/ssl_.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/ssl_match_hostname.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/ssltransport.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/timeout.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/url.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/util.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/util.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3/util/wait.py` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3-2.0.3.dist-info/METADATA` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3-2.0.3.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3-2.0.3.dist-info/RECORD` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3-2.0.3.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/.test/lib/python3.10/site-packages/urllib3-2.0.3.dist-info/licenses/LICENSE.txt` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/urllib3-2.0.3.dist-info/licenses/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/tests/test_scraping.py` & `hatch_project-0.2.0/tests/test_scraping.py`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/LICENSE.txt` & `hatch_project-0.2.0/.test/lib/python3.10/site-packages/six-1.16.0.dist-info/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,18 @@
-MIT License
+Copyright (c) 2010-2020 Benjamin Peterson
 
-Copyright (c) 2023-present Kenno-Warise <wariken0523@gmail.com>
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions:
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
 
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `hatch_project-0.1.2/README.md` & `hatch_project-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `hatch_project-0.1.2/pyproject.toml` & `hatch_project-0.2.0/pyproject.toml`

 * *Files identical despite different names*

