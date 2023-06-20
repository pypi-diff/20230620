# Comparing `tmp/troubadix-23.6.1.tar.gz` & `tmp/troubadix-23.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troubadix-23.6.1.tar", max compression
+gzip compressed data, was "troubadix-23.6.2.tar", max compression
```

## Comparing `troubadix-23.6.1.tar` & `troubadix-23.6.2.tar`

### file list

```diff
@@ -1,195 +1,195 @@
--rw-r--r--   0        0        0    35149 2023-06-20 11:25:25.268133 troubadix-23.6.1/LICENSE
--rw-r--r--   0        0        0     2730 2023-06-20 11:25:25.268133 troubadix-23.6.1/README.md
--rw-r--r--   0        0        0     2516 2023-06-20 11:25:25.272133 troubadix-23.6.1/pyproject.toml
--rw-r--r--   0        0        0      716 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/__init__.py
--rw-r--r--   0        0        0      716 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/helper/__init__.py
--rw-r--r--   0        0        0     8416 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/helper/test_linguistic_exception_handler.py
--rw-r--r--   0        0        0     1940 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/helper/test_patterns.py
--rw-r--r--   0        0        0     2396 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/__init__.py
--rw-r--r--   0        0        0     1012 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/fail.nasl
--rw-r--r--   0        0        0     1291 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/fail2.nasl
--rw-r--r--   0        0        0     2100 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test.nasl
--rw-r--r--   0        0        0     2450 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_badwords.py
--rw-r--r--   0        0        0     5109 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_copyright_text.py
--rw-r--r--   0        0        0     6961 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_copyright_year.py
--rw-r--r--   0        0        0     5004 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_creation_date.py
--rw-r--r--   0        0        0     5881 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_cve_format.py
--rw-r--r--   0        0        0     4914 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_cvss_format.py
--rw-r--r--   0        0        0     8970 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_dependencies.py
--rw-r--r--   0        0        0     5808 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_dependency_category_order.py
--rw-r--r--   0        0        0     5589 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_deprecated_dependency.py
--rw-r--r--   0        0        0     4545 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_deprecated_functions.py
--rw-r--r--   0        0        0     2394 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_double_end_points.py
--rw-r--r--   0        0        0     3504 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_duplicate_oid.py
--rw-r--r--   0        0        0     4686 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_duplicated_script_tags.py
--rw-r--r--   0        0        0     3906 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_encoding.py
--rw-r--r--   0        0        0     1982 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_files/fail_bad_new_line.nasl
--rw-r--r--   0        0        0      246 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_files/fail_badwords.nasl
--rw-r--r--   0        0        0     1979 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_files/fail_name_and_copyright_newline.nasl
--rw-r--r--   0        0        0     1965 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_files/fail_name_newline.nasl
--rwxr-xr-x   0        0        0     1012 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_files/fail_permissions.nasl
--rw-r--r--   0        0        0      150 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_files/fail_spelling.nasl
--rw-r--r--   0        0        0     2213 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/fail.nasl
--rw-r--r--   0        0        0      246 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/fail_badwords.nasl
--rw-r--r--   0        0        0     1990 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl
--rw-r--r--   0        0        0     1987 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl
--rw-r--r--   0        0        0     2134 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl
--rw-r--r--   0        0        0     1023 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/runner/fail.nasl
--rw-r--r--   0        0        0     1302 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl
--rw-r--r--   0        0        0     2122 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/runner/test.nasl
--rw-r--r--   0        0        0     2119 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl
--rw-r--r--   0        0        0     1023 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/test.inc
--rw-r--r--   0        0        0     2122 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/test.nasl
--rw-r--r--   0        0        0     2976 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/nasl/warning.nasl
--rw-r--r--   0        0        0     1012 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/ok_permissions.nasl
--rw-r--r--   0        0        0     2100 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/test_oid.nasl
--rw-r--r--   0        0        0     4548 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_forking_nasl_functions.py
--rw-r--r--   0        0        0     2271 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_get_kb_on_services.py
--rw-r--r--   0        0        0     9438 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_grammar.py
--rw-r--r--   0        0        0     6936 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_http_links_in_tags.py
--rw-r--r--   0        0        0     4730 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_illegal_characters.py
--rw-r--r--   0        0        0     5965 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_log_messages.py
--rw-r--r--   0        0        0     6174 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_malformed_dependencies.py
--rw-r--r--   0        0        0    21051 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_misplaced_compare_in_if.py
--rw-r--r--   0        0        0     3585 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_missing_desc_exit.py
--rw-r--r--   0        0        0     3101 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_missing_tag_solution.py
--rw-r--r--   0        0        0     4688 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_newlines.py
--rw-r--r--   0        0        0    40813 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_overlong_script_tags.py
--rw-r--r--   0        0        0     4294 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_prod_svc_detect_in_vulnvt.py
--rw-r--r--   0        0        0     4594 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_qod.py
--rw-r--r--   0        0        0     5844 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_reporting_consistency.py
--rw-r--r--   0        0        0     3371 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_script_add_preference_type.py
--rw-r--r--   0        0        0     2353 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_script_calls_empty_values.py
--rw-r--r--   0        0        0     2799 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_script_calls_recommended.py
--rw-r--r--   0        0        0     2650 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_script_category.py
--rw-r--r--   0        0        0     3469 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_script_copyright.py
--rw-r--r--   0        0        0     3877 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_script_family.py
--rw-r--r--   0        0        0     3079 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_script_tag_form.py
--rw-r--r--   0        0        0     6010 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_script_tag_whitespaces.py
--rw-r--r--   0        0        0     3313 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_script_tags_mandatory.py
--rw-r--r--   0        0        0     4858 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_script_version_and_last_modification_tags.py
--rw-r--r--   0        0        0     3016 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_script_xref_form.py
--rw-r--r--   0        0        0     2189 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_script_xref_url.py
--rw-r--r--   0        0        0     6599 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_security_messages.py
--rw-r--r--   0        0        0     3021 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_set_get_kb_calls.py
--rw-r--r--   0        0        0     7260 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_solution_text.py
--rw-r--r--   0        0        0     3306 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_solution_type.py
--rw-r--r--   0        0        0     2827 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_spelling.py
--rw-r--r--   0        0        0     1813 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_tabs.py
--rw-r--r--   0        0        0     6297 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_todo_tbd.py
--rw-r--r--   0        0        0     2398 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_trailing_spaces_tabs.py
--rw-r--r--   0        0        0     3868 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_using_display.py
--rw-r--r--   0        0        0    24134 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_valid_oid.py
--rw-r--r--   0        0        0     4154 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_valid_script_tag_names.py
--rw-r--r--   0        0        0     1947 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_vt_file_permissions.py
--rw-r--r--   0        0        0     5189 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_vt_placement.py
--rw-r--r--   0        0        0      716 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/__init__.py
--rw-r--r--   0        0        0      716 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/changed_packages/__init__.py
--rw-r--r--   0        0        0      716 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/changed_packages/markers/__init__.py
--rw-r--r--   0        0        0     3075 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py
--rw-r--r--   0        0        0     2620 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/changed_packages/markers/test_added_release.py
--rw-r--r--   0        0        0     1792 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py
--rw-r--r--   0        0        0     3258 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/changed_packages/markers/test_changed_update.py
--rw-r--r--   0        0        0     3584 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py
--rw-r--r--   0        0        0     3780 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/changed_packages/test_changed_packages.py
--rw-r--r--   0        0        0     2427 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/changed_packages/test_package.py
--rw-r--r--   0        0        0     2977 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/test_changed_cves.py
--rw-r--r--   0        0        0     2952 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/test_changed_oid.py
--rw-r--r--   0        0        0     3962 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/test_last_modification.py
--rw-r--r--   0        0        0     7347 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/test_no_solution.py
--rw-r--r--   0        0        0     6293 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/test_version_updated.py
--rw-r--r--   0        0        0     4768 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/test_argparser.py
--rw-r--r--   0        0        0     3947 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/test_helper.py
--rw-r--r--   0        0        0     3671 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/test_naslinter.py
--rw-r--r--   0        0        0     3399 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/test_reporter.py
--rw-r--r--   0        0        0     2517 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/test_results.py
--rw-r--r--   0        0        0    17972 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/test_runner.py
--rw-r--r--   0        0        0      716 2023-06-20 11:25:25.276133 troubadix-23.6.1/troubadix/__init__.py
--rw-r--r--   0        0        0      103 2023-06-20 11:25:25.276133 troubadix-23.6.1/troubadix/__version__.py
--rw-r--r--   0        0        0     6999 2023-06-20 11:25:25.276133 troubadix-23.6.1/troubadix/argparser.py
--rw-r--r--   0        0        0      338 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/codespell/codespell.additions
--rw-r--r--   0        0        0   124190 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/codespell/codespell.exclude
--rw-r--r--   0        0        0      756 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/codespell/codespell.ignore
--rw-r--r--   0        0        0     1061 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/helper/__init__.py
--rw-r--r--   0        0        0     3105 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/helper/helper.py
--rw-r--r--   0        0        0     6811 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/helper/linguistic_exception_handler.py
--rw-r--r--   0        0        0     9370 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/helper/patterns.py
--rw-r--r--   0        0        0     3508 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugin.py
--rw-r--r--   0        0        0     7013 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/__init__.py
--rw-r--r--   0        0        0     4166 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/badwords.py
--rw-r--r--   0        0        0     3583 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/copyright_text.py
--rw-r--r--   0        0        0     3334 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/copyright_year.py
--rw-r--r--   0        0        0     3357 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/creation_date.py
--rw-r--r--   0        0        0     3400 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/cve_format.py
--rw-r--r--   0        0        0     2309 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/cvss_format.py
--rw-r--r--   0        0        0     4456 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/dependencies.py
--rw-r--r--   0        0        0     7316 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/dependency_category_order.py
--rw-r--r--   0        0        0     4137 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/deprecated_dependency.py
--rw-r--r--   0        0        0     2568 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/deprecated_functions.py
--rw-r--r--   0        0        0     2509 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/double_end_points.py
--rw-r--r--   0        0        0     2652 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/duplicate_oid.py
--rw-r--r--   0        0        0     3179 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/duplicated_script_tags.py
--rw-r--r--   0        0        0     2090 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/encoding.py
--rw-r--r--   0        0        0     6014 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/forking_nasl_functions.py
--rw-r--r--   0        0        0     3401 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/get_kb_on_services.py
--rw-r--r--   0        0        0     8348 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/grammar.py
--rw-r--r--   0        0        0     7157 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/http_links_in_tags.py
--rw-r--r--   0        0        0     4406 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/illegal_characters.py
--rw-r--r--   0        0        0     2960 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/log_messages.py
--rw-r--r--   0        0        0     3000 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/malformed_dependencies.py
--rw-r--r--   0        0        0     5330 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/misplaced_compare_in_if.py
--rw-r--r--   0        0        0     2411 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/missing_desc_exit.py
--rw-r--r--   0        0        0     2828 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/missing_tag_solution.py
--rw-r--r--   0        0        0     2788 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/newlines.py
--rw-r--r--   0        0        0     2373 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/overlong_script_tags.py
--rw-r--r--   0        0        0     4584 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/prod_svc_detect_in_vulnvt.py
--rw-r--r--   0        0        0     3790 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/qod.py
--rw-r--r--   0        0        0     4043 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/reporting_consistency.py
--rw-r--r--   0        0        0     3193 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/script_add_preference_type.py
--rw-r--r--   0        0        0     2512 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/script_calls_empty_values.py
--rw-r--r--   0        0        0     3137 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/script_calls_recommended.py
--rw-r--r--   0        0        0     2184 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/script_category.py
--rw-r--r--   0        0        0     2310 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/script_copyright.py
--rw-r--r--   0        0        0     4023 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/script_family.py
--rw-r--r--   0        0        0     1773 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/script_tag_form.py
--rw-r--r--   0        0        0     2172 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/script_tag_whitespaces.py
--rw-r--r--   0        0        0     2630 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/script_tags_mandatory.py
--rw-r--r--   0        0        0     7026 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/script_version_and_last_modification_tags.py
--rw-r--r--   0        0        0     1848 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/script_xref_form.py
--rw-r--r--   0        0        0     2875 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/script_xref_url.py
--rw-r--r--   0        0        0     4708 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/security_messages.py
--rw-r--r--   0        0        0     3415 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/set_get_kb_calls.py
--rw-r--r--   0        0        0     5852 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/solution_text.py
--rw-r--r--   0        0        0     2602 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/solution_type.py
--rw-r--r--   0        0        0     9557 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/spelling.py
--rw-r--r--   0        0        0     1319 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/tabs.py
--rw-r--r--   0        0        0     1733 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/todo_tbd.py
--rw-r--r--   0        0        0     2049 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/trailing_spaces_tabs.py
--rw-r--r--   0        0        0     4046 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/using_display.py
--rw-r--r--   0        0        0    16627 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/valid_oid.py
--rw-r--r--   0        0        0     3447 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/valid_script_tag_names.py
--rw-r--r--   0        0        0     3285 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/variable_assigned_in_if.py
--rw-r--r--   0        0        0     1521 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/vt_file_permissions.py
--rw-r--r--   0        0        0     2800 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/vt_placement.py
--rw-r--r--   0        0        0     9176 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/reporter.py
--rw-r--r--   0        0        0     2632 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/results.py
--rw-r--r--   0        0        0     5172 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/runner.py
--rw-r--r--   0        0        0       22 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/standalone_plugins/__init__.py
--rw-r--r--   0        0        0     4145 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/allowed_rev_diff.py
--rw-r--r--   0        0        0     2921 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/changed_cves.py
--rw-r--r--   0        0        0     4074 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/changed_oid.py
--rw-r--r--   0        0        0     5742 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/changed_packages.py
--rw-r--r--   0        0        0      923 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/__init__.py
--rw-r--r--   0        0        0     1797 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py
--rw-r--r--   0        0        0     1486 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/added_release.py
--rw-r--r--   0        0        0     1124 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py
--rw-r--r--   0        0        0     1952 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/changed_update.py
--rw-r--r--   0        0        0     1632 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py
--rw-r--r--   0        0        0     1278 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/marker.py
--rw-r--r--   0        0        0     2743 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/package.py
--rw-r--r--   0        0        0     1028 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/common.py
--rw-r--r--   0        0        0     4616 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/last_modification.py
--rw-r--r--   0        0        0     8463 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/no_solution.py
--rw-r--r--   0        0        0     4263 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/version_updated.py
--rw-r--r--   0        0        0     6045 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/troubadix.py
--rw-r--r--   0        0        0     3971 1970-01-01 00:00:00.000000 troubadix-23.6.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-20 14:44:19.581933 troubadix-23.6.2/LICENSE
+-rw-r--r--   0        0        0     2730 2023-06-20 14:44:19.581933 troubadix-23.6.2/README.md
+-rw-r--r--   0        0        0     2516 2023-06-20 14:44:19.585933 troubadix-23.6.2/pyproject.toml
+-rw-r--r--   0        0        0      716 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/__init__.py
+-rw-r--r--   0        0        0      716 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/helper/__init__.py
+-rw-r--r--   0        0        0     8416 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/helper/test_linguistic_exception_handler.py
+-rw-r--r--   0        0        0     1940 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/helper/test_patterns.py
+-rw-r--r--   0        0        0     2396 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/__init__.py
+-rw-r--r--   0        0        0     1012 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/fail.nasl
+-rw-r--r--   0        0        0     1291 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/fail2.nasl
+-rw-r--r--   0        0        0     2100 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test.nasl
+-rw-r--r--   0        0        0     2450 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_badwords.py
+-rw-r--r--   0        0        0     5109 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_copyright_text.py
+-rw-r--r--   0        0        0     6961 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_copyright_year.py
+-rw-r--r--   0        0        0     5004 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_creation_date.py
+-rw-r--r--   0        0        0     5881 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_cve_format.py
+-rw-r--r--   0        0        0     4914 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_cvss_format.py
+-rw-r--r--   0        0        0     8970 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_dependencies.py
+-rw-r--r--   0        0        0     5808 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_dependency_category_order.py
+-rw-r--r--   0        0        0     5589 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_deprecated_dependency.py
+-rw-r--r--   0        0        0     4545 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_deprecated_functions.py
+-rw-r--r--   0        0        0     2394 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_double_end_points.py
+-rw-r--r--   0        0        0     3504 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_duplicate_oid.py
+-rw-r--r--   0        0        0     4686 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_duplicated_script_tags.py
+-rw-r--r--   0        0        0     3906 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_encoding.py
+-rw-r--r--   0        0        0     1982 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/fail_bad_new_line.nasl
+-rw-r--r--   0        0        0      246 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/fail_badwords.nasl
+-rw-r--r--   0        0        0     1979 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/fail_name_and_copyright_newline.nasl
+-rw-r--r--   0        0        0     1965 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/fail_name_newline.nasl
+-rwxr-xr-x   0        0        0     1012 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/fail_permissions.nasl
+-rw-r--r--   0        0        0      150 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/fail_spelling.nasl
+-rw-r--r--   0        0        0     2213 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/fail.nasl
+-rw-r--r--   0        0        0      246 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/fail_badwords.nasl
+-rw-r--r--   0        0        0     1990 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl
+-rw-r--r--   0        0        0     1987 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl
+-rw-r--r--   0        0        0     2134 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl
+-rw-r--r--   0        0        0     1023 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/runner/fail.nasl
+-rw-r--r--   0        0        0     1302 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl
+-rw-r--r--   0        0        0     2122 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/runner/test.nasl
+-rw-r--r--   0        0        0     2119 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl
+-rw-r--r--   0        0        0     1023 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/test.inc
+-rw-r--r--   0        0        0     2122 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/test.nasl
+-rw-r--r--   0        0        0     2976 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/nasl/warning.nasl
+-rw-r--r--   0        0        0     1012 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/ok_permissions.nasl
+-rw-r--r--   0        0        0     2100 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_files/test_oid.nasl
+-rw-r--r--   0        0        0     4548 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_forking_nasl_functions.py
+-rw-r--r--   0        0        0     2271 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_get_kb_on_services.py
+-rw-r--r--   0        0        0     9438 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_grammar.py
+-rw-r--r--   0        0        0     6936 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_http_links_in_tags.py
+-rw-r--r--   0        0        0     4730 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_illegal_characters.py
+-rw-r--r--   0        0        0     5965 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_log_messages.py
+-rw-r--r--   0        0        0     6174 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_malformed_dependencies.py
+-rw-r--r--   0        0        0    21051 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_misplaced_compare_in_if.py
+-rw-r--r--   0        0        0     3585 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_missing_desc_exit.py
+-rw-r--r--   0        0        0     3101 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_missing_tag_solution.py
+-rw-r--r--   0        0        0     4688 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_newlines.py
+-rw-r--r--   0        0        0    40813 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_overlong_script_tags.py
+-rw-r--r--   0        0        0     4294 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_prod_svc_detect_in_vulnvt.py
+-rw-r--r--   0        0        0     4594 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_qod.py
+-rw-r--r--   0        0        0     5844 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_reporting_consistency.py
+-rw-r--r--   0        0        0     3371 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_script_add_preference_type.py
+-rw-r--r--   0        0        0     2353 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_script_calls_empty_values.py
+-rw-r--r--   0        0        0     2799 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_script_calls_recommended.py
+-rw-r--r--   0        0        0     2650 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_script_category.py
+-rw-r--r--   0        0        0     3469 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_script_copyright.py
+-rw-r--r--   0        0        0     3877 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_script_family.py
+-rw-r--r--   0        0        0     3079 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_script_tag_form.py
+-rw-r--r--   0        0        0     6010 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_script_tag_whitespaces.py
+-rw-r--r--   0        0        0     3313 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_script_tags_mandatory.py
+-rw-r--r--   0        0        0     4858 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_script_version_and_last_modification_tags.py
+-rw-r--r--   0        0        0     3016 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_script_xref_form.py
+-rw-r--r--   0        0        0     2189 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_script_xref_url.py
+-rw-r--r--   0        0        0     6599 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_security_messages.py
+-rw-r--r--   0        0        0     3021 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_set_get_kb_calls.py
+-rw-r--r--   0        0        0     7260 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_solution_text.py
+-rw-r--r--   0        0        0     3306 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_solution_type.py
+-rw-r--r--   0        0        0     2827 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_spelling.py
+-rw-r--r--   0        0        0     1813 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_tabs.py
+-rw-r--r--   0        0        0     6297 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_todo_tbd.py
+-rw-r--r--   0        0        0     2398 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_trailing_spaces_tabs.py
+-rw-r--r--   0        0        0     3868 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_using_display.py
+-rw-r--r--   0        0        0    24134 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_valid_oid.py
+-rw-r--r--   0        0        0     4154 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_valid_script_tag_names.py
+-rw-r--r--   0        0        0     1947 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_vt_file_permissions.py
+-rw-r--r--   0        0        0     5189 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/plugins/test_vt_placement.py
+-rw-r--r--   0        0        0      716 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/standalone_plugins/__init__.py
+-rw-r--r--   0        0        0      716 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/standalone_plugins/changed_packages/__init__.py
+-rw-r--r--   0        0        0      716 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/standalone_plugins/changed_packages/markers/__init__.py
+-rw-r--r--   0        0        0     3075 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py
+-rw-r--r--   0        0        0     2620 2023-06-20 14:44:19.585933 troubadix-23.6.2/tests/standalone_plugins/changed_packages/markers/test_added_release.py
+-rw-r--r--   0        0        0     1792 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py
+-rw-r--r--   0        0        0     3258 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/standalone_plugins/changed_packages/markers/test_changed_update.py
+-rw-r--r--   0        0        0     3584 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py
+-rw-r--r--   0        0        0     3780 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/standalone_plugins/changed_packages/test_changed_packages.py
+-rw-r--r--   0        0        0     2427 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/standalone_plugins/changed_packages/test_package.py
+-rw-r--r--   0        0        0     2977 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/standalone_plugins/test_changed_cves.py
+-rw-r--r--   0        0        0     2952 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/standalone_plugins/test_changed_oid.py
+-rw-r--r--   0        0        0     3962 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/standalone_plugins/test_last_modification.py
+-rw-r--r--   0        0        0     7347 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/standalone_plugins/test_no_solution.py
+-rw-r--r--   0        0        0     6293 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/standalone_plugins/test_version_updated.py
+-rw-r--r--   0        0        0     4768 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/test_argparser.py
+-rw-r--r--   0        0        0     3947 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/test_helper.py
+-rw-r--r--   0        0        0     3671 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/test_naslinter.py
+-rw-r--r--   0        0        0     3399 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/test_reporter.py
+-rw-r--r--   0        0        0     2517 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/test_results.py
+-rw-r--r--   0        0        0    17972 2023-06-20 14:44:19.589933 troubadix-23.6.2/tests/test_runner.py
+-rw-r--r--   0        0        0      716 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/__init__.py
+-rw-r--r--   0        0        0      103 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/__version__.py
+-rw-r--r--   0        0        0     6999 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/argparser.py
+-rw-r--r--   0        0        0      338 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/codespell/codespell.additions
+-rw-r--r--   0        0        0   124978 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/codespell/codespell.exclude
+-rw-r--r--   0        0        0      756 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/codespell/codespell.ignore
+-rw-r--r--   0        0        0     1061 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/helper/__init__.py
+-rw-r--r--   0        0        0     3105 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/helper/helper.py
+-rw-r--r--   0        0        0     6811 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/helper/linguistic_exception_handler.py
+-rw-r--r--   0        0        0     9370 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/helper/patterns.py
+-rw-r--r--   0        0        0     3508 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugin.py
+-rw-r--r--   0        0        0     7013 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/__init__.py
+-rw-r--r--   0        0        0     4166 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/badwords.py
+-rw-r--r--   0        0        0     3583 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/copyright_text.py
+-rw-r--r--   0        0        0     3334 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/copyright_year.py
+-rw-r--r--   0        0        0     3357 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/creation_date.py
+-rw-r--r--   0        0        0     3400 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/cve_format.py
+-rw-r--r--   0        0        0     2309 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/cvss_format.py
+-rw-r--r--   0        0        0     4456 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/dependencies.py
+-rw-r--r--   0        0        0     7316 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/dependency_category_order.py
+-rw-r--r--   0        0        0     4137 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/deprecated_dependency.py
+-rw-r--r--   0        0        0     2568 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/deprecated_functions.py
+-rw-r--r--   0        0        0     2509 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/double_end_points.py
+-rw-r--r--   0        0        0     2652 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/duplicate_oid.py
+-rw-r--r--   0        0        0     3179 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/duplicated_script_tags.py
+-rw-r--r--   0        0        0     2090 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/encoding.py
+-rw-r--r--   0        0        0     6014 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/forking_nasl_functions.py
+-rw-r--r--   0        0        0     3401 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/get_kb_on_services.py
+-rw-r--r--   0        0        0     8566 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/grammar.py
+-rw-r--r--   0        0        0     7157 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/http_links_in_tags.py
+-rw-r--r--   0        0        0     4406 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/illegal_characters.py
+-rw-r--r--   0        0        0     2960 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/log_messages.py
+-rw-r--r--   0        0        0     3000 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/malformed_dependencies.py
+-rw-r--r--   0        0        0     5330 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/misplaced_compare_in_if.py
+-rw-r--r--   0        0        0     2411 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/missing_desc_exit.py
+-rw-r--r--   0        0        0     2828 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/missing_tag_solution.py
+-rw-r--r--   0        0        0     2788 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/newlines.py
+-rw-r--r--   0        0        0     2373 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/overlong_script_tags.py
+-rw-r--r--   0        0        0     4584 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/prod_svc_detect_in_vulnvt.py
+-rw-r--r--   0        0        0     3790 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/qod.py
+-rw-r--r--   0        0        0     4043 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/reporting_consistency.py
+-rw-r--r--   0        0        0     3193 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/script_add_preference_type.py
+-rw-r--r--   0        0        0     2512 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/script_calls_empty_values.py
+-rw-r--r--   0        0        0     3137 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/script_calls_recommended.py
+-rw-r--r--   0        0        0     2184 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/script_category.py
+-rw-r--r--   0        0        0     2310 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/script_copyright.py
+-rw-r--r--   0        0        0     4023 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/script_family.py
+-rw-r--r--   0        0        0     1773 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/script_tag_form.py
+-rw-r--r--   0        0        0     2172 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/script_tag_whitespaces.py
+-rw-r--r--   0        0        0     2630 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/script_tags_mandatory.py
+-rw-r--r--   0        0        0     7026 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/script_version_and_last_modification_tags.py
+-rw-r--r--   0        0        0     1848 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/script_xref_form.py
+-rw-r--r--   0        0        0     2875 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/script_xref_url.py
+-rw-r--r--   0        0        0     4708 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/security_messages.py
+-rw-r--r--   0        0        0     3415 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/set_get_kb_calls.py
+-rw-r--r--   0        0        0     5852 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/solution_text.py
+-rw-r--r--   0        0        0     2602 2023-06-20 14:44:19.589933 troubadix-23.6.2/troubadix/plugins/solution_type.py
+-rw-r--r--   0        0        0     9557 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/plugins/spelling.py
+-rw-r--r--   0        0        0     1319 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/plugins/tabs.py
+-rw-r--r--   0        0        0     1733 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/plugins/todo_tbd.py
+-rw-r--r--   0        0        0     2049 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/plugins/trailing_spaces_tabs.py
+-rw-r--r--   0        0        0     4046 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/plugins/using_display.py
+-rw-r--r--   0        0        0    16627 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/plugins/valid_oid.py
+-rw-r--r--   0        0        0     3447 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/plugins/valid_script_tag_names.py
+-rw-r--r--   0        0        0     3285 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/plugins/variable_assigned_in_if.py
+-rw-r--r--   0        0        0     1521 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/plugins/vt_file_permissions.py
+-rw-r--r--   0        0        0     2800 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/plugins/vt_placement.py
+-rw-r--r--   0        0        0     9176 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/reporter.py
+-rw-r--r--   0        0        0     2632 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/results.py
+-rw-r--r--   0        0        0     5172 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/runner.py
+-rw-r--r--   0        0        0       22 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/__init__.py
+-rw-r--r--   0        0        0     4145 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/allowed_rev_diff.py
+-rw-r--r--   0        0        0     2921 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/changed_cves.py
+-rw-r--r--   0        0        0     4074 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/changed_oid.py
+-rw-r--r--   0        0        0     5742 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/changed_packages.py
+-rw-r--r--   0        0        0      923 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/__init__.py
+-rw-r--r--   0        0        0     1797 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py
+-rw-r--r--   0        0        0     1486 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/added_release.py
+-rw-r--r--   0        0        0     1124 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py
+-rw-r--r--   0        0        0     1952 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/changed_update.py
+-rw-r--r--   0        0        0     1632 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py
+-rw-r--r--   0        0        0     1278 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/marker.py
+-rw-r--r--   0        0        0     2743 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/package.py
+-rw-r--r--   0        0        0     1028 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/common.py
+-rw-r--r--   0        0        0     4616 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/last_modification.py
+-rw-r--r--   0        0        0     8463 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/no_solution.py
+-rw-r--r--   0        0        0     4263 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/standalone_plugins/version_updated.py
+-rw-r--r--   0        0        0     6045 2023-06-20 14:44:19.593933 troubadix-23.6.2/troubadix/troubadix.py
+-rw-r--r--   0        0        0     3971 1970-01-01 00:00:00.000000 troubadix-23.6.2/PKG-INFO
```

### Comparing `troubadix-23.6.1/LICENSE` & `troubadix-23.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/README.md` & `troubadix-23.6.2/README.md`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/pyproject.toml` & `troubadix-23.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "troubadix"
-version = "23.6.1"
+version = "23.6.2"
 description = "A linting and QA check tool for NASL files"
 authors = ["Greenbone <info@greenbone.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/greenbone/troubadix"
 homepage = "https://github.com/greenbone/troubadix"
```

### Comparing `troubadix-23.6.1/tests/__init__.py` & `troubadix-23.6.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/helper/__init__.py` & `troubadix-23.6.2/tests/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/helper/test_linguistic_exception_handler.py` & `troubadix-23.6.2/tests/helper/test_linguistic_exception_handler.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/helper/test_patterns.py` & `troubadix-23.6.2/tests/helper/test_patterns.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/__init__.py` & `troubadix-23.6.2/tests/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/fail.nasl` & `troubadix-23.6.2/tests/plugins/fail.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/fail2.nasl` & `troubadix-23.6.2/tests/plugins/fail2.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test.nasl` & `troubadix-23.6.2/tests/plugins/test.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_badwords.py` & `troubadix-23.6.2/tests/plugins/test_badwords.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_copyright_text.py` & `troubadix-23.6.2/tests/plugins/test_copyright_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_copyright_year.py` & `troubadix-23.6.2/tests/plugins/test_copyright_year.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_creation_date.py` & `troubadix-23.6.2/tests/plugins/test_creation_date.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_cve_format.py` & `troubadix-23.6.2/tests/plugins/test_cve_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_cvss_format.py` & `troubadix-23.6.2/tests/plugins/test_cvss_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_dependencies.py` & `troubadix-23.6.2/tests/plugins/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_dependency_category_order.py` & `troubadix-23.6.2/tests/plugins/test_dependency_category_order.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_deprecated_dependency.py` & `troubadix-23.6.2/tests/plugins/test_deprecated_dependency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_deprecated_functions.py` & `troubadix-23.6.2/tests/plugins/test_deprecated_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_double_end_points.py` & `troubadix-23.6.2/tests/plugins/test_double_end_points.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_duplicate_oid.py` & `troubadix-23.6.2/tests/plugins/test_duplicate_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_duplicated_script_tags.py` & `troubadix-23.6.2/tests/plugins/test_duplicated_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_encoding.py` & `troubadix-23.6.2/tests/plugins/test_encoding.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_files/fail_bad_new_line.nasl` & `troubadix-23.6.2/tests/plugins/test_files/fail_bad_new_line.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_files/fail_name_and_copyright_newline.nasl` & `troubadix-23.6.2/tests/plugins/test_files/fail_name_and_copyright_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_files/fail_name_newline.nasl` & `troubadix-23.6.2/tests/plugins/test_files/fail_name_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_files/fail_permissions.nasl` & `troubadix-23.6.2/tests/plugins/test_files/fail_permissions.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/fail.nasl` & `troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/fail.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl` & `troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl` & `troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl` & `troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/runner/fail.nasl` & `troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/runner/fail.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl` & `troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/runner/test.nasl` & `troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/runner/test.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl` & `troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/test.inc` & `troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/test.inc`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/test.nasl` & `troubadix-23.6.2/tests/plugins/test_files/nasl/21.04/test.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_files/nasl/warning.nasl` & `troubadix-23.6.2/tests/plugins/test_files/nasl/warning.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_files/ok_permissions.nasl` & `troubadix-23.6.2/tests/plugins/test_files/ok_permissions.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_files/test_oid.nasl` & `troubadix-23.6.2/tests/plugins/test_files/test_oid.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_forking_nasl_functions.py` & `troubadix-23.6.2/tests/plugins/test_forking_nasl_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_get_kb_on_services.py` & `troubadix-23.6.2/tests/plugins/test_get_kb_on_services.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_grammar.py` & `troubadix-23.6.2/tests/plugins/test_grammar.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_http_links_in_tags.py` & `troubadix-23.6.2/tests/plugins/test_http_links_in_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_illegal_characters.py` & `troubadix-23.6.2/tests/plugins/test_illegal_characters.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_log_messages.py` & `troubadix-23.6.2/tests/plugins/test_log_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_malformed_dependencies.py` & `troubadix-23.6.2/tests/plugins/test_malformed_dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_misplaced_compare_in_if.py` & `troubadix-23.6.2/tests/plugins/test_misplaced_compare_in_if.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_missing_desc_exit.py` & `troubadix-23.6.2/tests/plugins/test_missing_desc_exit.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_missing_tag_solution.py` & `troubadix-23.6.2/tests/plugins/test_missing_tag_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_newlines.py` & `troubadix-23.6.2/tests/plugins/test_newlines.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_overlong_script_tags.py` & `troubadix-23.6.2/tests/plugins/test_overlong_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_prod_svc_detect_in_vulnvt.py` & `troubadix-23.6.2/tests/plugins/test_prod_svc_detect_in_vulnvt.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_qod.py` & `troubadix-23.6.2/tests/plugins/test_qod.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_reporting_consistency.py` & `troubadix-23.6.2/tests/plugins/test_reporting_consistency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_script_add_preference_type.py` & `troubadix-23.6.2/tests/plugins/test_script_add_preference_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_script_calls_empty_values.py` & `troubadix-23.6.2/tests/plugins/test_script_calls_empty_values.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_script_calls_recommended.py` & `troubadix-23.6.2/tests/plugins/test_script_calls_recommended.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_script_category.py` & `troubadix-23.6.2/tests/plugins/test_script_category.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_script_copyright.py` & `troubadix-23.6.2/tests/plugins/test_script_copyright.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_script_family.py` & `troubadix-23.6.2/tests/plugins/test_script_family.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_script_tag_form.py` & `troubadix-23.6.2/tests/plugins/test_script_tag_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_script_tag_whitespaces.py` & `troubadix-23.6.2/tests/plugins/test_script_tag_whitespaces.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_script_tags_mandatory.py` & `troubadix-23.6.2/tests/plugins/test_script_tags_mandatory.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_script_version_and_last_modification_tags.py` & `troubadix-23.6.2/tests/plugins/test_script_version_and_last_modification_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_script_xref_form.py` & `troubadix-23.6.2/tests/plugins/test_script_xref_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_script_xref_url.py` & `troubadix-23.6.2/tests/plugins/test_script_xref_url.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_security_messages.py` & `troubadix-23.6.2/tests/plugins/test_security_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_set_get_kb_calls.py` & `troubadix-23.6.2/tests/plugins/test_set_get_kb_calls.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_solution_text.py` & `troubadix-23.6.2/tests/plugins/test_solution_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_solution_type.py` & `troubadix-23.6.2/tests/plugins/test_solution_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_spelling.py` & `troubadix-23.6.2/tests/plugins/test_spelling.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_tabs.py` & `troubadix-23.6.2/tests/plugins/test_tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_todo_tbd.py` & `troubadix-23.6.2/tests/plugins/test_todo_tbd.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_trailing_spaces_tabs.py` & `troubadix-23.6.2/tests/plugins/test_trailing_spaces_tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_using_display.py` & `troubadix-23.6.2/tests/plugins/test_using_display.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_valid_oid.py` & `troubadix-23.6.2/tests/plugins/test_valid_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_valid_script_tag_names.py` & `troubadix-23.6.2/tests/plugins/test_valid_script_tag_names.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_vt_file_permissions.py` & `troubadix-23.6.2/tests/plugins/test_vt_file_permissions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/plugins/test_vt_placement.py` & `troubadix-23.6.2/tests/plugins/test_vt_placement.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/standalone_plugins/__init__.py` & `troubadix-23.6.2/tests/standalone_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/standalone_plugins/changed_packages/__init__.py` & `troubadix-23.6.2/tests/standalone_plugins/changed_packages/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/standalone_plugins/changed_packages/markers/__init__.py` & `troubadix-23.6.2/tests/standalone_plugins/changed_packages/markers/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py` & `troubadix-23.6.2/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/standalone_plugins/changed_packages/markers/test_added_release.py` & `troubadix-23.6.2/tests/standalone_plugins/changed_packages/markers/test_added_release.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py` & `troubadix-23.6.2/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/standalone_plugins/changed_packages/markers/test_changed_update.py` & `troubadix-23.6.2/tests/standalone_plugins/changed_packages/markers/test_changed_update.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py` & `troubadix-23.6.2/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/standalone_plugins/changed_packages/test_changed_packages.py` & `troubadix-23.6.2/tests/standalone_plugins/changed_packages/test_changed_packages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/standalone_plugins/changed_packages/test_package.py` & `troubadix-23.6.2/tests/standalone_plugins/changed_packages/test_package.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/standalone_plugins/test_changed_cves.py` & `troubadix-23.6.2/tests/standalone_plugins/test_changed_cves.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/standalone_plugins/test_changed_oid.py` & `troubadix-23.6.2/tests/standalone_plugins/test_changed_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/standalone_plugins/test_last_modification.py` & `troubadix-23.6.2/tests/standalone_plugins/test_last_modification.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/standalone_plugins/test_no_solution.py` & `troubadix-23.6.2/tests/standalone_plugins/test_no_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/standalone_plugins/test_version_updated.py` & `troubadix-23.6.2/tests/standalone_plugins/test_version_updated.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/test_argparser.py` & `troubadix-23.6.2/tests/test_argparser.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/test_helper.py` & `troubadix-23.6.2/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/test_naslinter.py` & `troubadix-23.6.2/tests/test_naslinter.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/test_reporter.py` & `troubadix-23.6.2/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/test_results.py` & `troubadix-23.6.2/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/tests/test_runner.py` & `troubadix-23.6.2/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/__init__.py` & `troubadix-23.6.2/troubadix/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/argparser.py` & `troubadix-23.6.2/troubadix/argparser.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/codespell/codespell.exclude` & `troubadix-23.6.2/troubadix/codespell/codespell.exclude`

 * *Files 0% similar despite different names*

```diff
@@ -142,14 +142,15 @@
 btrfs: add hel... [Please see the references for more information on the vulnerabilities]");
 - Btrfs: Avoid trucating page or punching hole in a already existed hole
 - Btrfs: delete chunk allocation attemp when setting block group ro.
 - Btrfs: explictly delete unused block groups in close_ctree and
   bu = eregmatch(pattern: "Build ([0-9]+)", string: banner);
     build = bu[1];
 buil... [Please see the references for more information on the vulnerabilities]");
+Bui Quang Minh discovered that the XDP socket implementation in the Linux
   Business RV042 Dual WAN VPN Routers and Cisco Small Business RV042G Dual Gigabit WAN VPN Routers could allow
   Business RV340, RV340W, RV345, and RV345P Dual WAN Gigabit VPN Routers could allow an unauthenticated, remote
 can: gs_usb: fix endianess problem with candleLight fi... [Please see the references for more information on the vulnerabilities]");
 can: gs_usb: fix endianess problem with candleLight firmware (git-fixes).
 #  CARD8    byteOrder (66 'B'=MSB, 108 'l'=LSB)
   carefully crafted GIF or IFF ILBM file, the application could crash
 CAS authentication protocol, did not encode tickets before adding them
@@ -169,14 +170,15 @@
 "chage --inactive <DAYS> <USER> for existing users.';
 # Charles Thier <cthier@thethiers.net>
         check_matches = re.finditer('[^\r\n]*[#]+[ ]*([Tt]hunderbird|[Ss]ea[Mm]onkey|[Hh]ot[Ff]ix|[Ff]irefox|[Pp]ower[Pp]oint( Viewer)?)[ ]*[Cc]heck[^\r\n]*\n', text)
 China_Internet_Network_Information_Center_EV_Certificates_Ro ot:2.4.72.159.0.1.crt (server auth)
 China_Internet_Network_Information_Center_EV_Certificates_Ro ot:2.4.72.159.0.1.crt server auth
 Christian Loos discovered an information disclosure flaw which may reveal RSS feeds URLs, and thus ticket data.
 Christian Loos discovered a remote denial of service vulnerability, exploitable via the email gateway and affecting any installation which accepts mail from untrusted sources. Depending on RT's logging configuration, a remote attacker can take advantage of this flaw to cause CPU and excessive disk usage.
+chunks in CAF audio files. If a user or automated system were tricked into
   Cisco ACI Multi-Site Orchestrator (MSO) to send a specific API request to a managed Cisco APIC or
 # Cisco TelePresence TC and TE Software Multiple Security Vulnerabilities
 Claus Jorgensen reported that a text input box can be pre-filled with a filename and then turned into a file-upload control, allowing a malicious website to steal any local file whose name they can guess. [MFSA-2006-23]
 Claus Wahlers reported that random images from GPU memory
   Clemens Huebner and Kevin Stange discovered that Pidgin incorrectly handled
                clen +
   clen = "567";
@@ -339,14 +341,15 @@
 (FATE#313309) The ipset userland utility will be published seperately to support this feature.
 (FATE#314441). A seperate hyper-v package will be published to support this feature.
   feature for Cisco Nexus 9000 Series Fabric Switches in Application Centric Infrastructure (ACI)
   feature is available to ensure that nobody can gain remote access to the modem (via the WAN/DSL interface).
 # Fedora Update for tre FEDORA-2016-0a952a3bc0
 # Fedora Update for tre FEDORA-2016-0ff6c3d84b
 # Fedora Update for tre FEDORA-2016-cd09eab674
+files. If a user were tricked into opening a specially-crafted CAF file, a
   files to potentially execute code and it is tracked by the Mitre CVE
   file_xml = '\t\t<file_item' + status + ' xmlns="http://oval.mitre.org/XMLSchema/' +
 Fixed a bug where Podman could not run containers usin... [Please see the references for more information on the vulnerabilities]");
 Fixed an issue with version missmatch (bsc#1162224).
 Fixed a regression in regards to the 'edge' comand line flag
   * fixed FILS to and RSNE into (Re)Association Response frames
 Fixed utf8 handling in perldoc by useing 'term' instead of 'man'
@@ -509,14 +512,15 @@
   it was added support for Cirrus Logic CS420x HDA codec, Wacom driver
 It was discovered that a buffer overflow in IFF ILBM image parsing
 It was discovered that the HSA Linux kernel driver for AMD GPU devices did
 It was discovered that the JULI logging component did not restrict its target path, resulting in potential denial of service through file overwrites.
 It was discovered that the PEAK-System Technik USB driver in the Linux
 It was discovered that the PEAK-System Technik USB driver in the ... [Please see the references for more information on the vulnerabilities]");
   It was discovered that the SBNI WAN driver did not correctly check for the
+It was discovered that WavPack incorrectly handled certain CAF files.
 It was found that 389 Directory Server was vulnerable to a flaw in which the default ACI (Access Control Instructions) could be read by an anonymous user. This could lead to leakage of sensitive information.
 It was found that if a Non-Maskable Interrupt (NMI) occurred immediately after a SYSCALL call or before a SYSRET call with the user RSP pointing to the NMI IST stack, the kernel could skip that NMI.(CVE-2015-3291)
  James Troup discovered that snap did not properly manage the permissions for
   James web admin endpoints to a public WAN (Internet) / public LAN without authentication.");
 Jan-Ivar Bruaroey, Jesse Ruderman, Markus Stange, Olli Pettay, Ehsan
  javax/security/auth/Subject/doAs/NestedActions.java fails if extra
 "jave",
@@ -648,14 +652,15 @@
 ofproto/bond: fix interal flow leak of tcp-balance bond
   of the Cisco Small Business RV340, RV340W, RV345, and RV345P Dual WAN Gigabit VPN Routers could
  of the CPU microcode packages, delivered in seperate updates.
   of user-supplied input processed by Steam In-Home Streaming (IHS) Discovery
   of Wiesemann & Theis GmbH W&T OPC Server for Windows.");
 Ohter bug fixes:
       # on e.g. newer releases of the NAM appliance we're even getting an 403/forbidden
+opening a specially crafted CAF audio file, an attacker could execute
 Openswan. Note that Portage will force a move for Super-FreeS/WAN users to
 or CAS service provider is enable and the administrator has chosen to store
 or potentially have unspecified futher impact.
   os_register_and_report( os:"Cisco NAM", cpe:"cpe:/o:cisco:prime_network_analysis_module_firmware", banner_type:BANNER_TYPE, port:port, proto:"udp", banner:sysdesc, desc:SCRIPT_DESC, runs_key:"unixoide" );
                'oval-common-schema.xsd http://oval.mitre.org/XMLSchema/oval-system-characteristics-5#linux linux-system-characteristics-schema.xsd">\n\n' );
                        '//oval.mitre.org/XMLSchema/oval-system-characteristi' +
                'oval-system-characteristics-schema.xsd http://oval.mitre.org/XMLSchema/oval-common-5 ',
@@ -845,23 +850,26 @@
   script_tag(name:"insight", value:"A security feature bypass exists in Azure SSH Keypairs, due to a change in the provisioning logic for some Linux images that use cloud-init, aka 'Azure SSH Keypairs Security Feature Bypass Vulnerability'.(CVE-2019-0816)");
   script_tag(name:"insight", value:"A vulnerability in processing IPv6 ND packets originating from subscribers
   script_tag(name:"insight", value:"A vulnerability in the implementation of the Short Message Service (SMS) handling functionality of Cisco IOS Software and Cisco IOS XE Software could allow an unauthenticated, remote attacker to trigger a denial of service (DoS) condition on an affected device. The vulnerability is due to improper processing of SMS protocol data units (PDUs) that are encoded with a special character set. An attacker could exploit this vulnerability by sending a malicious SMS message to an affected device. A successful exploit could allow the attacker to cause the wireless WAN (WWAN) cellular interface module on an affected device to crash, resulting in a DoS condition that would require manual intervention to restore normal operating conditions. (CVE-2019-1747)
   script_tag(name:"insight", value:"A vulnerability in the implementation of the Short Message Service (SMS) handling functionality of Cisco IOS Software and Cisco IOS XE Software could allow an unauthenticated, remote attacker to trigger a denial of service (DoS) condition on an affected device. The vulnerability is due to improper processing of SMS protocol data units (PDUs) that are encoded with a special character set. An attacker could exploit this vulnerability by sending a malicious SMS message to an affected device. A successful exploit could allow the attacker to cause the wireless WAN (WWAN) cellular interface module on an affected device to crash, resulting in a DoS condition that would require manual intervention to restore normal operating conditions. (CVE-2019-1747)");
   script_tag(name:"insight", value:"A vulnerability in the implementation of the Short Message Service (SMS) handling functionality of Cisco IOS Software and Cisco IOS XE Software could allow an unauthenticated, remote attacker to trigger a denial of service (DoS) condition on an affected device. The vulnerability is due to improper processing of SMS protocol data units (PDUs) that are encoded with a special character set. An attacker could exploit this vulnerability by sending a malicious SMS message to an affected device. A successful exploit could allow the attacker to cause the wireless WAN (WWAN) cellular interface module on an affected device to crash, resulting in a DoS condition that would require manual intervention to restore normal operating conditions.(CVE-2019-1747)
   script_tag(name:"insight", value:"A vulnerability in the Network Access Manager (NAM) of Cisco
   script_tag(name:"insight", value:"A vulnerability was found in Linux kernel. There is an information leak in file 'sound/core/timer.c' of the latest mainline Linux kernel, the stack object tread has a total size of 32 bytes. It contains a 8-bytes padding, which is not initialized but sent to user via copy_to_user(), resulting a kernel leak.(CVE-2016-4569)
+  script_tag(name:"insight", value:"Benjamin Smedberg, Bob Clary, Jesse Ruderman, and Josh Aas discovered
+  script_tag(name:"insight", value:"Bui Quang Minh discovered that libxml2 did not properly process XPath
   script_tag(name:"insight", value:"Calle Dybedahl discovered a bug in lyskom-server which could result in
   script_tag(name:"insight", value:"Calle Dybedahl discovered a bug in lyskom-server which could result in a denial of service where an unauthenticated user could cause the server to become unresponsive as it processes a large query.
   script_tag(name:"insight", value:"Cisco TelePresence TC and TE Software are prone to
   script_tag(name:"insight", value:"_core_/plugins/medias in SPIP allows remote authenticated authors to inject
   script_tag(name:"insight", value:"Crafted data - channels per frame value - in CAF files enables remote
   script_tag(name:"insight", value:"Erik Sjoelund discovered that a race condition in the stap tool shipped by Systemtap, an instrumentation system for Linux 2.6, allows local privilege escalation for members of the stapusr group.
   script_tag(name:"insight", value:"FreeS/WAN, Openswan, strongSwan and Super-FreeS/WAN contain two bugs when
   script_tag(name:"insight", value:"In Apache::Session::Browseable before 1.3.6, validity of the X.509 certificate is not checked by default when connecting to remote LDAP backends, because the default configuration of the Net::LDAPS module for Perl is used.
   script_tag(name:"insight", value:"It was discovered that a specially-crafted packet sent to the racoon ipsec key exchange server could cause a tunnel to crash, resulting in a denial of service.
+  script_tag(name:"insight", value:"It was discovered that the VLC CAF demuxer incorrectly handled certain
   script_tag(name:"insight", value:"James Troup discovered that MAAS stored RabbitMQ
   script_tag(name:"insight", value:"James Troup discovered that MAAS stored RabbitMQ authentication
   script_tag(name:"insight", value:"James Troup discovered that snap did not properly manage the permissions for
   script_tag(name:"insight", value:"Javantea discovered a NULL pointer dereference flaw in racoon, the Internet Key Exchange daemon of ipsec-tools. A remote attacker can use this flaw to cause the IKE daemon to crash via specially crafted UDP packets, resulting in a denial of service.
   script_tag(name:"insight", value:"Jesse Hertz and Tim Newsham discovered
   script_tag(name:"insight", value:"Jesse Hertz and Tim Newsham discovered that
   script_tag(name:"insight", value:"Juraj Somorovsky, Robert Merget and Nimrod Aviram discovered a padding oracle attack in OpenSSL.
@@ -872,14 +880,15 @@
   script_tag(name:"insight", value:"Multiple flaws are due to errors in MS-MMS, RTPS, RTPS2, Mount, AMPQ, ACN,
   script_tag(name:"insight", value:"Multiple flaws are due to errors in RELOAD, MPLS Echo, CSN.1, HART/IP and TCP
   script_tag(name:"insight", value:"Multiple flaws are present due to errors in Liquify save mesh, Sharpen,
   script_tag(name:"insight", value:"Multiple vulnerabilities were discovered in nd, a command-line WebDAV
   script_tag(name:"insight", value:"Multiple vulnerabilities were discovered in nd, a command-line WebDAV interface, whereby long strings received from the remote server could overflow fixed-length buffers. This vulnerability could be exploited by a remote attacker in control of a malicious WebDAV server to execute arbitrary code if the server was accessed by a vulnerable version of nd.
   script_tag(name:"insight", value:"Multiple vulnerabilities were discovered in the dissectors for the MS-MMS, RTPS, RTPS2, Mount, ACN, CIMD and DTLS protocols, which could result in denial of service or the execution of arbitrary code.
   script_tag(name:"insight", value:"Ning Zhang & Amin Tora discovered that the mod_dav module
+  script_tag(name:"insight", value:"Robert Merget, Marcus Brinkmann, Nimrod Aviram, and Juraj Somorovsky
   script_tag(name:"insight", value:"Robert Merget, Marcus Brinkmann, Nimrod Aviram, and Juraj Somorovsky discovered that certain Diffie-Hellman ciphersuites in the TLS specification and implemented by OpenSSL contained a flaw. A remote attacker could possibly use this issue to eavesdrop on encrypted communications. This was fixed in this update by disabling the insecure ciphersuites.
   script_tag(name:"insight", value:"Several remote vulnerabilities have been discovered in racoon, the Internet Key Exchange daemon of ipsec-tools. The Common Vulnerabilities and Exposures project identifies the following problems:
   script_tag(name:"insight", value:"Several vulnerabilities have been discovered in phpCAS, a CAS client
   script_tag(name:"insight", value:"Simo Sorce discovered that a NULL pointer dereference existed in
   script_tag(name:"insight", value:"Stan Hu discovered that kramdown, a pure Ruby Markdown parser and converter, performed insufficient namespace validation of Rouge syntax highlighting formatters.
   script_tag(name:"insight", value:"The http_request_split_value function in request.c in lighttpd before 1.4.32 allows remote attackers to cause a denial of service (infinite loop) via a request with a header containing an empty token, as demonstrated using the 'Connection: TE,,Keep-Alive' header.");
   script_tag(name:"insight", value:"The Internet Key Exchange version 1 (IKEv1) implementation in racoon from ipsec-tools, IPsec tools for Linux, try to dereference a NULL pointer under certain conditions which allows a remote attacker to cause a denial of service.
```

### Comparing `troubadix-23.6.1/troubadix/codespell/codespell.ignore` & `troubadix-23.6.2/troubadix/codespell/codespell.ignore`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/helper/__init__.py` & `troubadix-23.6.2/troubadix/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/helper/helper.py` & `troubadix-23.6.2/troubadix/helper/helper.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/helper/linguistic_exception_handler.py` & `troubadix-23.6.2/troubadix/helper/linguistic_exception_handler.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/helper/patterns.py` & `troubadix-23.6.2/troubadix/helper/patterns.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugin.py` & `troubadix-23.6.2/troubadix/plugin.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/__init__.py` & `troubadix-23.6.2/troubadix/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/badwords.py` & `troubadix-23.6.2/troubadix/plugins/badwords.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/copyright_text.py` & `troubadix-23.6.2/troubadix/plugins/copyright_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/copyright_year.py` & `troubadix-23.6.2/troubadix/plugins/copyright_year.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/creation_date.py` & `troubadix-23.6.2/troubadix/plugins/creation_date.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/cve_format.py` & `troubadix-23.6.2/troubadix/plugins/cve_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/cvss_format.py` & `troubadix-23.6.2/troubadix/plugins/cvss_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/dependencies.py` & `troubadix-23.6.2/troubadix/plugins/dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/dependency_category_order.py` & `troubadix-23.6.2/troubadix/plugins/dependency_category_order.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/deprecated_dependency.py` & `troubadix-23.6.2/troubadix/plugins/deprecated_dependency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/deprecated_functions.py` & `troubadix-23.6.2/troubadix/plugins/deprecated_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/double_end_points.py` & `troubadix-23.6.2/troubadix/plugins/double_end_points.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/duplicate_oid.py` & `troubadix-23.6.2/troubadix/plugins/duplicate_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/duplicated_script_tags.py` & `troubadix-23.6.2/troubadix/plugins/duplicated_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/encoding.py` & `troubadix-23.6.2/troubadix/plugins/encoding.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/forking_nasl_functions.py` & `troubadix-23.6.2/troubadix/plugins/forking_nasl_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/get_kb_on_services.py` & `troubadix-23.6.2/troubadix/plugins/get_kb_on_services.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/grammar.py` & `troubadix-23.6.2/troubadix/plugins/grammar.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,18 @@
         r"\s+a\s+(page|client|report|few)\s+requests",
         re.IGNORECASE,
     ),
     # From 2021/mozilla/gb_mozilla_firefox_mfsa_2012-63_lin.nasl
     TextCheck("when an element with a 'requiredFeatures' attribute"),
     # e.g. Multiple Products $something Vulnerability
     PatternCheck(r"Multiple\s+Products.+Vulnerability", re.IGNORECASE),
+    # From 2009/ubuntu/gb_ubuntu_USN_592_1.nasl:
+    # The default has been changed to prompt the user each time a website
+    # requests a client certificate.
+    TextCheck("a website requests a client certificate"),
 ]
 
 
 def get_grammer_pattern() -> re.Pattern:
     return re.compile(
         r".*("
         r"refer\s+(the\s+)?Reference|"
```

### Comparing `troubadix-23.6.1/troubadix/plugins/http_links_in_tags.py` & `troubadix-23.6.2/troubadix/plugins/http_links_in_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/illegal_characters.py` & `troubadix-23.6.2/troubadix/plugins/illegal_characters.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/log_messages.py` & `troubadix-23.6.2/troubadix/plugins/log_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/malformed_dependencies.py` & `troubadix-23.6.2/troubadix/plugins/malformed_dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/misplaced_compare_in_if.py` & `troubadix-23.6.2/troubadix/plugins/misplaced_compare_in_if.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/missing_desc_exit.py` & `troubadix-23.6.2/troubadix/plugins/missing_desc_exit.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/missing_tag_solution.py` & `troubadix-23.6.2/troubadix/plugins/missing_tag_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/newlines.py` & `troubadix-23.6.2/troubadix/plugins/newlines.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/overlong_script_tags.py` & `troubadix-23.6.2/troubadix/plugins/overlong_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/prod_svc_detect_in_vulnvt.py` & `troubadix-23.6.2/troubadix/plugins/prod_svc_detect_in_vulnvt.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/qod.py` & `troubadix-23.6.2/troubadix/plugins/qod.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/reporting_consistency.py` & `troubadix-23.6.2/troubadix/plugins/reporting_consistency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/script_add_preference_type.py` & `troubadix-23.6.2/troubadix/plugins/script_add_preference_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/script_calls_empty_values.py` & `troubadix-23.6.2/troubadix/plugins/script_calls_empty_values.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/script_calls_recommended.py` & `troubadix-23.6.2/troubadix/plugins/script_calls_recommended.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/script_category.py` & `troubadix-23.6.2/troubadix/plugins/script_category.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/script_copyright.py` & `troubadix-23.6.2/troubadix/plugins/script_copyright.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/script_family.py` & `troubadix-23.6.2/troubadix/plugins/script_family.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/script_tag_form.py` & `troubadix-23.6.2/troubadix/plugins/script_tag_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/script_tag_whitespaces.py` & `troubadix-23.6.2/troubadix/plugins/script_tag_whitespaces.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/script_tags_mandatory.py` & `troubadix-23.6.2/troubadix/plugins/script_tags_mandatory.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/script_version_and_last_modification_tags.py` & `troubadix-23.6.2/troubadix/plugins/script_version_and_last_modification_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/script_xref_form.py` & `troubadix-23.6.2/troubadix/plugins/script_xref_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/script_xref_url.py` & `troubadix-23.6.2/troubadix/plugins/script_xref_url.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/security_messages.py` & `troubadix-23.6.2/troubadix/plugins/security_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/set_get_kb_calls.py` & `troubadix-23.6.2/troubadix/plugins/set_get_kb_calls.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/solution_text.py` & `troubadix-23.6.2/troubadix/plugins/solution_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/solution_type.py` & `troubadix-23.6.2/troubadix/plugins/solution_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/spelling.py` & `troubadix-23.6.2/troubadix/plugins/spelling.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/tabs.py` & `troubadix-23.6.2/troubadix/plugins/tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/todo_tbd.py` & `troubadix-23.6.2/troubadix/plugins/todo_tbd.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/trailing_spaces_tabs.py` & `troubadix-23.6.2/troubadix/plugins/trailing_spaces_tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/using_display.py` & `troubadix-23.6.2/troubadix/plugins/using_display.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/valid_oid.py` & `troubadix-23.6.2/troubadix/plugins/valid_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/valid_script_tag_names.py` & `troubadix-23.6.2/troubadix/plugins/valid_script_tag_names.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/variable_assigned_in_if.py` & `troubadix-23.6.2/troubadix/plugins/variable_assigned_in_if.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/vt_file_permissions.py` & `troubadix-23.6.2/troubadix/plugins/vt_file_permissions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/plugins/vt_placement.py` & `troubadix-23.6.2/troubadix/plugins/vt_placement.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/reporter.py` & `troubadix-23.6.2/troubadix/reporter.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/results.py` & `troubadix-23.6.2/troubadix/results.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/runner.py` & `troubadix-23.6.2/troubadix/runner.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/standalone_plugins/allowed_rev_diff.py` & `troubadix-23.6.2/troubadix/standalone_plugins/allowed_rev_diff.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/standalone_plugins/changed_cves.py` & `troubadix-23.6.2/troubadix/standalone_plugins/changed_cves.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/standalone_plugins/changed_oid.py` & `troubadix-23.6.2/troubadix/standalone_plugins/changed_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/changed_packages.py` & `troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/changed_packages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/__init__.py` & `troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py` & `troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/added_release.py` & `troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/added_release.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py` & `troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/changed_update.py` & `troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/changed_update.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py` & `troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/marker.py` & `troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/marker/marker.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/package.py` & `troubadix-23.6.2/troubadix/standalone_plugins/changed_packages/package.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/standalone_plugins/common.py` & `troubadix-23.6.2/troubadix/standalone_plugins/common.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/standalone_plugins/last_modification.py` & `troubadix-23.6.2/troubadix/standalone_plugins/last_modification.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/standalone_plugins/no_solution.py` & `troubadix-23.6.2/troubadix/standalone_plugins/no_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/standalone_plugins/version_updated.py` & `troubadix-23.6.2/troubadix/standalone_plugins/version_updated.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/troubadix/troubadix.py` & `troubadix-23.6.2/troubadix/troubadix.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.1/PKG-INFO` & `troubadix-23.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troubadix
-Version: 23.6.1
+Version: 23.6.2
 Summary: A linting and QA check tool for NASL files
 Home-page: https://github.com/greenbone/troubadix
 License: GPL-3.0-or-later
 Author: Greenbone
 Author-email: info@greenbone.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

