# Comparing `tmp/code_ocean_aux_tools-1.0.1.tar.gz` & `tmp/code_ocean_aux_tools-1.0.2.tar.gz`

## Comparing `code_ocean_aux_tools-1.0.1.tar` & `code_ocean_aux_tools-1.0.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/setup.py
--rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/index.html
--rwxr-xr-x   0        0        0   145343 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/search.js
--rwxr-xr-x   0        0        0    35405 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools.html
--rwxr-xr-x   0        0        0    64876 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/co_fasta.html
--rwxr-xr-x   0        0        0   137471 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/co_fastq.html
--rwxr-xr-x   0        0        0    95633 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/co_utils.html
--rwxr-xr-x   0        0        0    38262 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_cpu_count.html
--rwxr-xr-x   0        0        0    46146 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_dir_contents.html
--rwxr-xr-x   0        0        0    45020 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_fasta_file.html
--rwxr-xr-x   0        0        0    43404 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_fastq_pair.html
--rwxr-xr-x   0        0        0    44350 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_fwd_fastqs.html
--rwxr-xr-x   0        0        0    43368 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_groups.html
--rwxr-xr-x   0        0        0    77308 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_logger.html
--rwxr-xr-x   0        0        0    38284 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_pipeline_confirm.html
--rwxr-xr-x   0        0        0    43353 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_read_direction.html
--rwxr-xr-x   0        0        0    45190 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_read_pattern.html
--rwxr-xr-x   0        0        0    45128 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_read_prefix.html
--rwxr-xr-x   0        0        0    45408 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_rev_file.html
--rwxr-xr-x   0        0        0    43629 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/set_log_msg.html
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/__init__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/__init__.py
--rwxr-xr-x   0        0        0     2014 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/co_fasta.py
--rwxr-xr-x   0        0        0     7434 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/co_fastq.py
--rwxr-xr-x   0        0        0     4334 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/co_utils.py
--rwxr-xr-x   0        0        0      190 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/get_cpu_count.py
--rwxr-xr-x   0        0        0      716 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/get_dir_contents.py
--rwxr-xr-x   0        0        0      693 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/get_fasta_file.py
--rwxr-xr-x   0        0        0      515 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/get_fastq_pair.py
--rwxr-xr-x   0        0        0      573 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/get_fwd_fastqs.py
--rwxr-xr-x   0        0        0      503 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/get_groups.py
--rwxr-xr-x   0        0        0     3821 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/get_logger.py
--rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/get_pipeline_confirm.py
--rwxr-xr-x   0        0        0      534 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/get_read_direction.py
--rwxr-xr-x   0        0        0      641 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/get_read_pattern.py
--rwxr-xr-x   0        0        0      609 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/get_read_prefix.py
--rwxr-xr-x   0        0        0      633 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/get_rev_file.py
--rwxr-xr-x   0        0        0      556 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/set_log_msg.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/__init__.py
--rwxr-xr-x   0        0        0      200 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/conftest.py
--rwxr-xr-x   0        0        0      649 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/test_get_cpu_count.py
--rwxr-xr-x   0        0        0      664 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/test_get_dir_contents.py
--rwxr-xr-x   0        0        0     1781 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/test_get_fasta_file.py
--rwxr-xr-x   0        0        0      502 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/test_get_fwd_fastqs.py
--rwxr-xr-x   0        0        0      478 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/test_get_groups.py
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/test_get_pipeline_confirm.py
--rwxr-xr-x   0        0        0     1533 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/test_get_read_direction.py
--rwxr-xr-x   0        0        0     3356 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/test_get_read_pattern.py
--rwxr-xr-x   0        0        0     1330 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/test_get_read_prefix.py
--rwxr-xr-x   0        0        0     2175 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/test_get_rev_file.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/fixtures/__init__.py
--rwxr-xr-x   0        0        0      857 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/fixtures/dirs_of_files.py
--rwxr-xr-x   0        0        0      320 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/fixtures/fastq_file.py
--rwxr-xr-x   0        0        0      659 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/fixtures/sample_sheets.py
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/.gitignore
--rwxr-xr-x   0        0        0     1067 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/LICENSE
--rwxr-xr-x   0        0        0     3985 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/README.md
--rwxr-xr-x   0        0        0     1388 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/setup.py
+-rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/index.html
+-rwxr-xr-x   0        0        0   145343 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/search.js
+-rwxr-xr-x   0        0        0    35405 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools.html
+-rwxr-xr-x   0        0        0    64876 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/co_fasta.html
+-rwxr-xr-x   0        0        0   137471 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/co_fastq.html
+-rwxr-xr-x   0        0        0    95633 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/co_utils.html
+-rwxr-xr-x   0        0        0    38262 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_cpu_count.html
+-rwxr-xr-x   0        0        0    46146 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_dir_contents.html
+-rwxr-xr-x   0        0        0    45020 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_fasta_file.html
+-rwxr-xr-x   0        0        0    43404 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_fastq_pair.html
+-rwxr-xr-x   0        0        0    44350 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_fwd_fastqs.html
+-rwxr-xr-x   0        0        0    43368 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_groups.html
+-rwxr-xr-x   0        0        0    77308 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_logger.html
+-rwxr-xr-x   0        0        0    38284 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_pipeline_confirm.html
+-rwxr-xr-x   0        0        0    43353 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_read_direction.html
+-rwxr-xr-x   0        0        0    45190 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_read_pattern.html
+-rwxr-xr-x   0        0        0    45128 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_read_prefix.html
+-rwxr-xr-x   0        0        0    45408 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_rev_file.html
+-rwxr-xr-x   0        0        0    43629 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/docs/src/co_tools/set_log_msg.html
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/__init__.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/__init__.py
+-rwxr-xr-x   0        0        0     2028 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/co_fasta.py
+-rwxr-xr-x   0        0        0     7448 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/co_fastq.py
+-rwxr-xr-x   0        0        0     4363 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/co_utils.py
+-rwxr-xr-x   0        0        0      190 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/get_cpu_count.py
+-rwxr-xr-x   0        0        0      730 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/get_dir_contents.py
+-rwxr-xr-x   0        0        0      707 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/get_fasta_file.py
+-rwxr-xr-x   0        0        0      529 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/get_fastq_pair.py
+-rwxr-xr-x   0        0        0      587 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/get_fwd_fastqs.py
+-rwxr-xr-x   0        0        0      517 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/get_groups.py
+-rwxr-xr-x   0        0        0     3826 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/get_logger.py
+-rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/get_pipeline_confirm.py
+-rwxr-xr-x   0        0        0      548 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/get_read_direction.py
+-rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/get_read_pattern.py
+-rwxr-xr-x   0        0        0      623 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/get_read_prefix.py
+-rwxr-xr-x   0        0        0      647 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/get_rev_file.py
+-rwxr-xr-x   0        0        0      570 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/src/co_tools/set_log_msg.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/__init__.py
+-rwxr-xr-x   0        0        0      200 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/conftest.py
+-rwxr-xr-x   0        0        0      649 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/test_get_cpu_count.py
+-rwxr-xr-x   0        0        0      664 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/test_get_dir_contents.py
+-rwxr-xr-x   0        0        0     1781 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/test_get_fasta_file.py
+-rwxr-xr-x   0        0        0      502 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/test_get_fwd_fastqs.py
+-rwxr-xr-x   0        0        0      478 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/test_get_groups.py
+-rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/test_get_pipeline_confirm.py
+-rwxr-xr-x   0        0        0     1533 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/test_get_read_direction.py
+-rwxr-xr-x   0        0        0     3356 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/test_get_read_pattern.py
+-rwxr-xr-x   0        0        0     1330 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/test_get_read_prefix.py
+-rwxr-xr-x   0        0        0     2175 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/test_get_rev_file.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/fixtures/__init__.py
+-rwxr-xr-x   0        0        0      857 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/fixtures/dirs_of_files.py
+-rwxr-xr-x   0        0        0      320 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/fixtures/fastq_file.py
+-rwxr-xr-x   0        0        0      659 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/tests/fixtures/sample_sheets.py
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/.gitignore
+-rwxr-xr-x   0        0        0     1067 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/LICENSE
+-rwxr-xr-x   0        0        0     3985 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/README.md
+-rwxr-xr-x   0        0        0     1388 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.2/PKG-INFO
```

### Comparing `code_ocean_aux_tools-1.0.1/docs/search.js` & `code_ocean_aux_tools-1.0.2/docs/search.js`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/docs/src/co_tools.html` & `code_ocean_aux_tools-1.0.2/docs/src/co_tools.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/docs/src/co_tools/co_fasta.html` & `code_ocean_aux_tools-1.0.2/docs/src/co_tools/co_fasta.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/docs/src/co_tools/co_fastq.html` & `code_ocean_aux_tools-1.0.2/docs/src/co_tools/co_fastq.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/docs/src/co_tools/co_utils.html` & `code_ocean_aux_tools-1.0.2/docs/src/co_tools/co_utils.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_cpu_count.html` & `code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_cpu_count.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_dir_contents.html` & `code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_dir_contents.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_fasta_file.html` & `code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_fasta_file.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_fastq_pair.html` & `code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_fastq_pair.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_fwd_fastqs.html` & `code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_fwd_fastqs.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_groups.html` & `code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_groups.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_logger.html` & `code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_logger.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_pipeline_confirm.html` & `code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_pipeline_confirm.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_read_direction.html` & `code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_read_direction.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_read_pattern.html` & `code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_read_pattern.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_read_prefix.html` & `code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_read_prefix.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_rev_file.html` & `code_ocean_aux_tools-1.0.2/docs/src/co_tools/get_rev_file.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/docs/src/co_tools/set_log_msg.html` & `code_ocean_aux_tools-1.0.2/docs/src/co_tools/set_log_msg.html`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/src/co_tools/co_fasta.py` & `code_ocean_aux_tools-1.0.2/src/co_tools/co_fasta.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import re
 from glob import glob
 from pathlib import Path
 from pathlib import PurePath
 
-if os.getenv("CO_LOG").lower() == "true":
+if os.environ.get("CO_LOG", "false").lower() == "true":
     from .get_logger import LOGGER
 
     log = LOGGER
 else:
     import logging
 
     log = logging.getLogger(__name__)
```

### Comparing `code_ocean_aux_tools-1.0.1/src/co_tools/co_fastq.py` & `code_ocean_aux_tools-1.0.2/src/co_tools/co_fastq.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import re
 from glob import glob
 from pathlib import Path
 
-if os.getenv("CO_LOG").lower() == "true":
+if os.environ.get("CO_LOG", "false").lower() == "true":
     from .get_logger import LOGGER
 
     log = LOGGER
 else:
     import logging
 
     log = logging.getLogger(__name__)
```

### Comparing `code_ocean_aux_tools-1.0.1/src/co_tools/co_utils.py` & `code_ocean_aux_tools-1.0.2/src/co_tools/co_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 from glob import glob
 from multiprocessing import cpu_count
 from pathlib import Path
 
-if os.getenv("CO_LOG").lower() == "true":
+if os.environ.get("CO_LOG", "false").lower() == "true":
     from .get_logger import LOGGER
 
     log = LOGGER
 else:
     import logging
 
     log = logging.getLogger(__name__)
 
-co_cpus = os.getenv("CO_CPUS")
-aws_batch_job_id = os.getenv("AWS_BATCH_JOB_ID")
+co_cpus = os.environ.get("CO_CPUS")
+aws_batch_job_id = os.environ.get("AWS_BATCH_JOB_ID")
 
 
 def get_cpu_limit(co_cpus=co_cpus, aws_batch_job_id=aws_batch_job_id):
     """This function returns an integer corresponding to the number of cores
 
     Args:
         co_cpus (int, optional): _description_. Defaults to co_cpus.
@@ -102,15 +102,15 @@
 
 def is_pipeline():
     """This function lets confirms if code is executing in a pipeline
 
     Returns:
         int: Returns 1 if in a pipeline, 0 otherwise.
     """
-    return 1 if bool(os.getenv("AWS_BATCH_JOB_ID")) else 0
+    return 1 if bool(os.environ.get("AWS_BATCH_JOB_ID")) else 0
 
 
 def print_log_msg(msg=None, level="WARNING"):
     level = level.upper()
     if level == "DEBUG":
         return log.debug(msg)
     elif level == "INFO":
```

### Comparing `code_ocean_aux_tools-1.0.1/src/co_tools/get_dir_contents.py` & `code_ocean_aux_tools-1.0.2/src/co_tools/get_dir_contents.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 import os
 import sys
 
 from .co_utils import get_dir_contents
 
-if os.getenv("CO_LOG").lower() == "true":
+if os.environ.get("CO_LOG", "false").lower() == "true":
     from .get_logger import LOGGER
 
     log = LOGGER
 else:
     import logging
 
     log = logging.getLogger(__name__)
```

### Comparing `code_ocean_aux_tools-1.0.1/src/co_tools/get_fasta_file.py` & `code_ocean_aux_tools-1.0.2/src/co_tools/get_rev_file.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 #!/usr/bin/env python
 import os
 import sys
 
-from .co_fasta import find_fasta_file
+from .co_fastq import get_rev_file
 
-if os.getenv("CO_LOG").lower() == "true":
+if os.environ.get("CO_LOG", "false").lower() == "true":
     from .get_logger import LOGGER
 
     log = LOGGER
 else:
     import logging
 
     log = logging.getLogger(__name__)
 
 
 def main(argv=sys.argv):
+    log.debug(f"args: {sys.argv}")
     if len(argv) == 1:
-        log.warning(
-            "You failed to provide a search directory."
-            + " Will continue by searching in ../data"
-        )
-        print(find_fasta_file("../data"))
+        sys.exit(log.error("You failed to provide a filename"))
+    elif len(argv) == 2:
+        print(get_rev_file(argv[1]))
         return 0
     else:
-        log.info(f"Input dir to search for fasta file: {sys.argv[1]}")
-        print(find_fasta_file(sys.argv[1]))
+        print(get_rev_file(argv[1], argv[2]))
         return 0
 
 
 if __name__ == "__main__":
+    log.debug(f"args: {sys.argv}")
     sys.exit(main(sys.argv))
```

### Comparing `code_ocean_aux_tools-1.0.1/src/co_tools/get_fastq_pair.py` & `code_ocean_aux_tools-1.0.2/src/co_tools/get_fastq_pair.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 import os
 import sys
 
 from .co_fastq import get_fastq_pair
 
-if os.getenv("CO_LOG").lower() == "true":
+if os.environ.get("CO_LOG", "false").lower() == "true":
     from .get_logger import LOGGER
 
     log = LOGGER
 else:
     import logging
 
     log = logging.getLogger(__name__)
```

### Comparing `code_ocean_aux_tools-1.0.1/src/co_tools/get_fwd_fastqs.py` & `code_ocean_aux_tools-1.0.2/src/co_tools/get_fwd_fastqs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 import os
 import sys
 
 from .co_fastq import get_fwd_fastqs
 
-if os.getenv("CO_LOG").lower() == "true":
+if os.environ.get("CO_LOG", "false").lower() == "true":
     from .get_logger import LOGGER
 
     log = LOGGER
 else:
     import logging
 
     log = logging.getLogger(__name__)
```

### Comparing `code_ocean_aux_tools-1.0.1/src/co_tools/get_logger.py` & `code_ocean_aux_tools-1.0.2/src/co_tools/get_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import os
 
 LOGGER_DIR_PATH = "../results/co_logs"  # path to log directory
 co_computation_id = os.environ.get("CO_COMPUTATION_ID")
-aws_batch_job_id = os.getenv("AWS_BATCH_JOB_ID")
+aws_batch_job_id = os.environ.get("AWS_BATCH_JOB_ID")
 # name for the log file in ../results/co_logs
 LOGGER_FILE_NAME = co_computation_id if co_computation_id else aws_batch_job_id
 ENV_LEVEL = os.environ.get("CO_LOG_LEVEL")
 DEFAULT_LEVEL = "WARNING" if not ENV_LEVEL else ENV_LEVEL.upper()
 
 """
 Benefit to this logger is that it adds to each log entry a timestamp,
```

### Comparing `code_ocean_aux_tools-1.0.1/src/co_tools/get_read_direction.py` & `code_ocean_aux_tools-1.0.2/src/co_tools/get_read_pattern.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 #!/usr/bin/env python
 import os
 import sys
 
-from .co_fastq import get_read_direction
+from .co_fastq import get_read_pattern
 
-if os.getenv("CO_LOG").lower() == "true":
+if os.environ.get("CO_LOG", "false").lower() == "true":
     from .get_logger import LOGGER
 
     log = LOGGER
 else:
     import logging
 
     log = logging.getLogger(__name__)
 
 
 def main(argv=sys.argv):
     log.debug(f"args: {sys.argv}")
     if len(argv) == 1:
-        sys.exit("You failed to provide a file name")
-    print(get_read_direction(argv[1]))
+        sys.exit(log.error("You failed to provide a filename and direction"))
+    elif len(argv) == 2:
+        print(get_read_pattern(argv[1]))
+        return 0
+    print(get_read_pattern(argv[1], argv[2]))
     return 0
 
 
 if __name__ == "__main__":
     log.debug(f"args: {sys.argv}")
-    sys.exit(main(argv=sys.argv))
+    sys.exit(main(sys.argv))
```

### Comparing `code_ocean_aux_tools-1.0.1/src/co_tools/get_read_pattern.py` & `code_ocean_aux_tools-1.0.2/src/co_tools/get_read_prefix.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #!/usr/bin/env python
 import os
 import sys
 
-from .co_fastq import get_read_pattern
+from .co_fastq import get_prefix
 
-if os.getenv("CO_LOG").lower() == "true":
+if os.environ.get("CO_LOG", "false").lower() == "true":
     from .get_logger import LOGGER
 
     log = LOGGER
 else:
     import logging
 
     log = logging.getLogger(__name__)
 
 
 def main(argv=sys.argv):
     log.debug(f"args: {sys.argv}")
     if len(argv) == 1:
-        sys.exit(log.error("You failed to provide a filename and direction"))
+        sys.exit(log.error("You failed to provide a filename"))
     elif len(argv) == 2:
-        print(get_read_pattern(argv[1]))
+        print(get_prefix(argv[1]))
         return 0
-    print(get_read_pattern(argv[1], argv[2]))
+    print(get_prefix(argv[1], argv[2]))
     return 0
 
 
 if __name__ == "__main__":
     log.debug(f"args: {sys.argv}")
     sys.exit(main(sys.argv))
```

### Comparing `code_ocean_aux_tools-1.0.1/src/co_tools/get_read_prefix.py` & `code_ocean_aux_tools-1.0.2/src/co_tools/get_groups.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 #!/usr/bin/env python
 import os
 import sys
 
-from .co_fastq import get_prefix
+from .co_utils import get_groups
 
-if os.getenv("CO_LOG").lower() == "true":
+if os.environ.get("CO_LOG", "false").lower() == "true":
     from .get_logger import LOGGER
 
     log = LOGGER
 else:
     import logging
 
     log = logging.getLogger(__name__)
 
 
 def main(argv=sys.argv):
     log.debug(f"args: {sys.argv}")
-    if len(argv) == 1:
-        sys.exit(log.error("You failed to provide a filename"))
-    elif len(argv) == 2:
-        print(get_prefix(argv[1]))
+    if len(argv) > 1:
+        print(get_groups(argv[1]))
         return 0
-    print(get_prefix(argv[1], argv[2]))
+    print(get_groups())
     return 0
 
 
 if __name__ == "__main__":
     log.debug(f"args: {sys.argv}")
     sys.exit(main(sys.argv))
```

### Comparing `code_ocean_aux_tools-1.0.1/src/co_tools/get_rev_file.py` & `code_ocean_aux_tools-1.0.2/src/co_tools/get_fasta_file.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 #!/usr/bin/env python
 import os
 import sys
 
-from .co_fastq import get_rev_file
+from .co_fasta import find_fasta_file
 
-if os.getenv("CO_LOG").lower() == "true":
+if os.environ.get("CO_LOG", "false").lower() == "true":
     from .get_logger import LOGGER
 
     log = LOGGER
 else:
     import logging
 
     log = logging.getLogger(__name__)
 
 
 def main(argv=sys.argv):
-    log.debug(f"args: {sys.argv}")
     if len(argv) == 1:
-        sys.exit(log.error("You failed to provide a filename"))
-    elif len(argv) == 2:
-        print(get_rev_file(argv[1]))
+        log.warning(
+            "You failed to provide a search directory."
+            + " Will continue by searching in ../data"
+        )
+        print(find_fasta_file("../data"))
         return 0
     else:
-        print(get_rev_file(argv[1], argv[2]))
+        log.info(f"Input dir to search for fasta file: {sys.argv[1]}")
+        print(find_fasta_file(sys.argv[1]))
         return 0
 
 
 if __name__ == "__main__":
-    log.debug(f"args: {sys.argv}")
     sys.exit(main(sys.argv))
```

### Comparing `code_ocean_aux_tools-1.0.1/src/co_tools/set_log_msg.py` & `code_ocean_aux_tools-1.0.2/src/co_tools/set_log_msg.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 import os
 import sys
 
 from .co_utils import print_log_msg
 
-if os.getenv("CO_LOG").lower() == "true":
+if os.environ.get("CO_LOG", "false").lower() == "true":
     from .get_logger import LOGGER
 
     log = LOGGER
 else:
     import logging
 
     log = logging.getLogger(__name__)
```

### Comparing `code_ocean_aux_tools-1.0.1/tests/test_get_cpu_count.py` & `code_ocean_aux_tools-1.0.2/tests/test_get_cpu_count.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/tests/test_get_dir_contents.py` & `code_ocean_aux_tools-1.0.2/tests/test_get_dir_contents.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/tests/test_get_fasta_file.py` & `code_ocean_aux_tools-1.0.2/tests/test_get_fasta_file.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/tests/test_get_read_direction.py` & `code_ocean_aux_tools-1.0.2/tests/test_get_read_direction.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/tests/test_get_read_pattern.py` & `code_ocean_aux_tools-1.0.2/tests/test_get_read_pattern.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/tests/test_get_read_prefix.py` & `code_ocean_aux_tools-1.0.2/tests/test_get_read_prefix.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/tests/test_get_rev_file.py` & `code_ocean_aux_tools-1.0.2/tests/test_get_rev_file.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/tests/fixtures/dirs_of_files.py` & `code_ocean_aux_tools-1.0.2/tests/fixtures/dirs_of_files.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/tests/fixtures/sample_sheets.py` & `code_ocean_aux_tools-1.0.2/tests/fixtures/sample_sheets.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/LICENSE` & `code_ocean_aux_tools-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/README.md` & `code_ocean_aux_tools-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.1/pyproject.toml` & `code_ocean_aux_tools-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/co_tools"]
 
 [project]
 name = "Code_Ocean_Aux_Tools"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Frank Zappulla", email="frank@codeocean.com" },
 ]
 maintainers = [
     { name="Frank Zappulla", email="frank@codeocean.com" }
 ]
 description = "A suite of convenience tools for working with sequencing files and Code Ocean capsules."
```

### Comparing `code_ocean_aux_tools-1.0.1/PKG-INFO` & `code_ocean_aux_tools-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Code_Ocean_Aux_Tools
-Version: 1.0.1
+Version: 1.0.2
 Summary: A suite of convenience tools for working with sequencing files and Code Ocean capsules.
 Project-URL: Homepage, https://github.com/codeocean/co_aux_tools
 Project-URL: Bug Tracker, https://github.com/codeocean/co_aux_tools/issues
 Author-email: Frank Zappulla <frank@codeocean.com>
 Maintainer-email: Frank Zappulla <frank@codeocean.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

