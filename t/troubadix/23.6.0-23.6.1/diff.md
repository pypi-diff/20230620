# Comparing `tmp/troubadix-23.6.0.tar.gz` & `tmp/troubadix-23.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troubadix-23.6.0.tar", max compression
+gzip compressed data, was "troubadix-23.6.1.tar", max compression
```

## Comparing `troubadix-23.6.0.tar` & `troubadix-23.6.1.tar`

### file list

```diff
@@ -1,195 +1,195 @@
--rw-r--r--   0        0        0    35149 2023-06-15 12:27:39.519142 troubadix-23.6.0/LICENSE
--rw-r--r--   0        0        0     2730 2023-06-15 12:27:39.519142 troubadix-23.6.0/README.md
--rw-r--r--   0        0        0     2516 2023-06-15 12:27:39.523142 troubadix-23.6.0/pyproject.toml
--rw-r--r--   0        0        0      716 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/__init__.py
--rw-r--r--   0        0        0      716 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/helper/__init__.py
--rw-r--r--   0        0        0     8416 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/helper/test_linguistic_exception_handler.py
--rw-r--r--   0        0        0     1940 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/helper/test_patterns.py
--rw-r--r--   0        0        0     2396 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/__init__.py
--rw-r--r--   0        0        0     1012 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/fail.nasl
--rw-r--r--   0        0        0     1291 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/fail2.nasl
--rw-r--r--   0        0        0     2100 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test.nasl
--rw-r--r--   0        0        0     2061 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_badwords.py
--rw-r--r--   0        0        0     5109 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_copyright_text.py
--rw-r--r--   0        0        0     6961 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_copyright_year.py
--rw-r--r--   0        0        0     5004 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_creation_date.py
--rw-r--r--   0        0        0     5881 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_cve_format.py
--rw-r--r--   0        0        0     4914 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_cvss_format.py
--rw-r--r--   0        0        0     8970 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_dependencies.py
--rw-r--r--   0        0        0     5808 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_dependency_category_order.py
--rw-r--r--   0        0        0     5589 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_deprecated_dependency.py
--rw-r--r--   0        0        0     4545 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_deprecated_functions.py
--rw-r--r--   0        0        0     2394 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_double_end_points.py
--rw-r--r--   0        0        0     3504 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_duplicate_oid.py
--rw-r--r--   0        0        0     4686 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_duplicated_script_tags.py
--rw-r--r--   0        0        0     3906 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_encoding.py
--rw-r--r--   0        0        0     1982 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_files/fail_bad_new_line.nasl
--rw-r--r--   0        0        0      246 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_files/fail_badwords.nasl
--rw-r--r--   0        0        0     1979 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_files/fail_name_and_copyright_newline.nasl
--rw-r--r--   0        0        0     1965 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_files/fail_name_newline.nasl
--rwxr-xr-x   0        0        0     1012 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_files/fail_permissions.nasl
--rw-r--r--   0        0        0      150 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_files/fail_spelling.nasl
--rw-r--r--   0        0        0     2213 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_files/nasl/21.04/fail.nasl
--rw-r--r--   0        0        0      246 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_files/nasl/21.04/fail_badwords.nasl
--rw-r--r--   0        0        0     1990 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl
--rw-r--r--   0        0        0     1987 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl
--rw-r--r--   0        0        0     2134 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl
--rw-r--r--   0        0        0     1023 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_files/nasl/21.04/runner/fail.nasl
--rw-r--r--   0        0        0     1302 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl
--rw-r--r--   0        0        0     2122 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_files/nasl/21.04/runner/test.nasl
--rw-r--r--   0        0        0     2119 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl
--rw-r--r--   0        0        0     1023 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_files/nasl/21.04/test.inc
--rw-r--r--   0        0        0     2122 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_files/nasl/21.04/test.nasl
--rw-r--r--   0        0        0     2976 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_files/nasl/warning.nasl
--rw-r--r--   0        0        0     1012 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_files/ok_permissions.nasl
--rw-r--r--   0        0        0     2100 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_files/test_oid.nasl
--rw-r--r--   0        0        0     4548 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_forking_nasl_functions.py
--rw-r--r--   0        0        0     2271 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_get_kb_on_services.py
--rw-r--r--   0        0        0     9438 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_grammar.py
--rw-r--r--   0        0        0     6936 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_http_links_in_tags.py
--rw-r--r--   0        0        0     4730 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_illegal_characters.py
--rw-r--r--   0        0        0     5965 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_log_messages.py
--rw-r--r--   0        0        0     6174 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_malformed_dependencies.py
--rw-r--r--   0        0        0    21051 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_misplaced_compare_in_if.py
--rw-r--r--   0        0        0     3585 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_missing_desc_exit.py
--rw-r--r--   0        0        0     3101 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_missing_tag_solution.py
--rw-r--r--   0        0        0     4688 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_newlines.py
--rw-r--r--   0        0        0    40813 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_overlong_script_tags.py
--rw-r--r--   0        0        0     4294 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_prod_svc_detect_in_vulnvt.py
--rw-r--r--   0        0        0     4594 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_qod.py
--rw-r--r--   0        0        0     5844 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_reporting_consistency.py
--rw-r--r--   0        0        0     3371 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_script_add_preference_type.py
--rw-r--r--   0        0        0     2353 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_script_calls_empty_values.py
--rw-r--r--   0        0        0     2799 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_script_calls_recommended.py
--rw-r--r--   0        0        0     2650 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_script_category.py
--rw-r--r--   0        0        0     3469 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_script_copyright.py
--rw-r--r--   0        0        0     3877 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_script_family.py
--rw-r--r--   0        0        0     3079 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_script_tag_form.py
--rw-r--r--   0        0        0     6010 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_script_tag_whitespaces.py
--rw-r--r--   0        0        0     3313 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_script_tags_mandatory.py
--rw-r--r--   0        0        0     4858 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_script_version_and_last_modification_tags.py
--rw-r--r--   0        0        0     3016 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_script_xref_form.py
--rw-r--r--   0        0        0     2189 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_script_xref_url.py
--rw-r--r--   0        0        0     6599 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_security_messages.py
--rw-r--r--   0        0        0     3021 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_set_get_kb_calls.py
--rw-r--r--   0        0        0     7260 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_solution_text.py
--rw-r--r--   0        0        0     3306 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_solution_type.py
--rw-r--r--   0        0        0     2827 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_spelling.py
--rw-r--r--   0        0        0     1813 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_tabs.py
--rw-r--r--   0        0        0     6297 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_todo_tbd.py
--rw-r--r--   0        0        0     2398 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_trailing_spaces_tabs.py
--rw-r--r--   0        0        0     3868 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_using_display.py
--rw-r--r--   0        0        0    24134 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_valid_oid.py
--rw-r--r--   0        0        0     4154 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_valid_script_tag_names.py
--rw-r--r--   0        0        0     1947 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_vt_file_permissions.py
--rw-r--r--   0        0        0     5189 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/plugins/test_vt_placement.py
--rw-r--r--   0        0        0      716 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/standalone_plugins/__init__.py
--rw-r--r--   0        0        0      716 2023-06-15 12:27:39.523142 troubadix-23.6.0/tests/standalone_plugins/changed_packages/__init__.py
--rw-r--r--   0        0        0      716 2023-06-15 12:27:39.527142 troubadix-23.6.0/tests/standalone_plugins/changed_packages/markers/__init__.py
--rw-r--r--   0        0        0     3075 2023-06-15 12:27:39.527142 troubadix-23.6.0/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py
--rw-r--r--   0        0        0     2620 2023-06-15 12:27:39.527142 troubadix-23.6.0/tests/standalone_plugins/changed_packages/markers/test_added_release.py
--rw-r--r--   0        0        0     1792 2023-06-15 12:27:39.527142 troubadix-23.6.0/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py
--rw-r--r--   0        0        0     3258 2023-06-15 12:27:39.527142 troubadix-23.6.0/tests/standalone_plugins/changed_packages/markers/test_changed_update.py
--rw-r--r--   0        0        0     3584 2023-06-15 12:27:39.527142 troubadix-23.6.0/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py
--rw-r--r--   0        0        0     3780 2023-06-15 12:27:39.527142 troubadix-23.6.0/tests/standalone_plugins/changed_packages/test_changed_packages.py
--rw-r--r--   0        0        0     2427 2023-06-15 12:27:39.527142 troubadix-23.6.0/tests/standalone_plugins/changed_packages/test_package.py
--rw-r--r--   0        0        0     2977 2023-06-15 12:27:39.527142 troubadix-23.6.0/tests/standalone_plugins/test_changed_cves.py
--rw-r--r--   0        0        0     2952 2023-06-15 12:27:39.527142 troubadix-23.6.0/tests/standalone_plugins/test_changed_oid.py
--rw-r--r--   0        0        0     3962 2023-06-15 12:27:39.527142 troubadix-23.6.0/tests/standalone_plugins/test_last_modification.py
--rw-r--r--   0        0        0     7347 2023-06-15 12:27:39.527142 troubadix-23.6.0/tests/standalone_plugins/test_no_solution.py
--rw-r--r--   0        0        0     6293 2023-06-15 12:27:39.527142 troubadix-23.6.0/tests/standalone_plugins/test_version_updated.py
--rw-r--r--   0        0        0     4768 2023-06-15 12:27:39.527142 troubadix-23.6.0/tests/test_argparser.py
--rw-r--r--   0        0        0     3947 2023-06-15 12:27:39.527142 troubadix-23.6.0/tests/test_helper.py
--rw-r--r--   0        0        0     3671 2023-06-15 12:27:39.527142 troubadix-23.6.0/tests/test_naslinter.py
--rw-r--r--   0        0        0     3399 2023-06-15 12:27:39.527142 troubadix-23.6.0/tests/test_reporter.py
--rw-r--r--   0        0        0     2517 2023-06-15 12:27:39.527142 troubadix-23.6.0/tests/test_results.py
--rw-r--r--   0        0        0    17972 2023-06-15 12:27:39.527142 troubadix-23.6.0/tests/test_runner.py
--rw-r--r--   0        0        0      716 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/__init__.py
--rw-r--r--   0        0        0      103 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/__version__.py
--rw-r--r--   0        0        0     6999 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/argparser.py
--rw-r--r--   0        0        0      338 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/codespell/codespell.additions
--rw-r--r--   0        0        0   125386 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/codespell/codespell.exclude
--rw-r--r--   0        0        0      756 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/codespell/codespell.ignore
--rw-r--r--   0        0        0     1061 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/helper/__init__.py
--rw-r--r--   0        0        0     3105 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/helper/helper.py
--rw-r--r--   0        0        0     6811 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/helper/linguistic_exception_handler.py
--rw-r--r--   0        0        0     9370 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/helper/patterns.py
--rw-r--r--   0        0        0     3508 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugin.py
--rw-r--r--   0        0        0     7013 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/__init__.py
--rw-r--r--   0        0        0     3633 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/badwords.py
--rw-r--r--   0        0        0     3583 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/copyright_text.py
--rw-r--r--   0        0        0     3334 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/copyright_year.py
--rw-r--r--   0        0        0     3357 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/creation_date.py
--rw-r--r--   0        0        0     3400 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/cve_format.py
--rw-r--r--   0        0        0     2309 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/cvss_format.py
--rw-r--r--   0        0        0     4456 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/dependencies.py
--rw-r--r--   0        0        0     7316 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/dependency_category_order.py
--rw-r--r--   0        0        0     4137 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/deprecated_dependency.py
--rw-r--r--   0        0        0     2568 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/deprecated_functions.py
--rw-r--r--   0        0        0     2509 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/double_end_points.py
--rw-r--r--   0        0        0     2652 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/duplicate_oid.py
--rw-r--r--   0        0        0     3179 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/duplicated_script_tags.py
--rw-r--r--   0        0        0     2090 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/encoding.py
--rw-r--r--   0        0        0     6014 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/forking_nasl_functions.py
--rw-r--r--   0        0        0     3401 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/get_kb_on_services.py
--rw-r--r--   0        0        0     8348 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/grammar.py
--rw-r--r--   0        0        0     7157 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/http_links_in_tags.py
--rw-r--r--   0        0        0     4406 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/illegal_characters.py
--rw-r--r--   0        0        0     2960 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/log_messages.py
--rw-r--r--   0        0        0     3000 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/malformed_dependencies.py
--rw-r--r--   0        0        0     5330 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/misplaced_compare_in_if.py
--rw-r--r--   0        0        0     2411 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/missing_desc_exit.py
--rw-r--r--   0        0        0     2828 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/missing_tag_solution.py
--rw-r--r--   0        0        0     2788 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/newlines.py
--rw-r--r--   0        0        0     2373 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/overlong_script_tags.py
--rw-r--r--   0        0        0     4584 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/prod_svc_detect_in_vulnvt.py
--rw-r--r--   0        0        0     3790 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/qod.py
--rw-r--r--   0        0        0     4043 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/reporting_consistency.py
--rw-r--r--   0        0        0     3193 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/script_add_preference_type.py
--rw-r--r--   0        0        0     2512 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/script_calls_empty_values.py
--rw-r--r--   0        0        0     3137 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/script_calls_recommended.py
--rw-r--r--   0        0        0     2184 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/script_category.py
--rw-r--r--   0        0        0     2310 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/script_copyright.py
--rw-r--r--   0        0        0     4023 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/script_family.py
--rw-r--r--   0        0        0     1773 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/script_tag_form.py
--rw-r--r--   0        0        0     2172 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/script_tag_whitespaces.py
--rw-r--r--   0        0        0     2630 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/script_tags_mandatory.py
--rw-r--r--   0        0        0     7026 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/script_version_and_last_modification_tags.py
--rw-r--r--   0        0        0     1848 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/script_xref_form.py
--rw-r--r--   0        0        0     2875 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/script_xref_url.py
--rw-r--r--   0        0        0     4708 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/security_messages.py
--rw-r--r--   0        0        0     3415 2023-06-15 12:27:39.527142 troubadix-23.6.0/troubadix/plugins/set_get_kb_calls.py
--rw-r--r--   0        0        0     5852 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/plugins/solution_text.py
--rw-r--r--   0        0        0     2602 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/plugins/solution_type.py
--rw-r--r--   0        0        0     9557 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/plugins/spelling.py
--rw-r--r--   0        0        0     1319 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/plugins/tabs.py
--rw-r--r--   0        0        0     1733 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/plugins/todo_tbd.py
--rw-r--r--   0        0        0     2049 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/plugins/trailing_spaces_tabs.py
--rw-r--r--   0        0        0     4046 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/plugins/using_display.py
--rw-r--r--   0        0        0    16627 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/plugins/valid_oid.py
--rw-r--r--   0        0        0     3447 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/plugins/valid_script_tag_names.py
--rw-r--r--   0        0        0     3285 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/plugins/variable_assigned_in_if.py
--rw-r--r--   0        0        0     1521 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/plugins/vt_file_permissions.py
--rw-r--r--   0        0        0     2800 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/plugins/vt_placement.py
--rw-r--r--   0        0        0     9176 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/reporter.py
--rw-r--r--   0        0        0     2632 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/results.py
--rw-r--r--   0        0        0     5172 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/runner.py
--rw-r--r--   0        0        0       22 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/standalone_plugins/__init__.py
--rw-r--r--   0        0        0     4145 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/standalone_plugins/allowed_rev_diff.py
--rw-r--r--   0        0        0     2921 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/standalone_plugins/changed_cves.py
--rw-r--r--   0        0        0     4074 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/standalone_plugins/changed_oid.py
--rw-r--r--   0        0        0     5742 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/standalone_plugins/changed_packages/changed_packages.py
--rw-r--r--   0        0        0      923 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/standalone_plugins/changed_packages/marker/__init__.py
--rw-r--r--   0        0        0     1797 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py
--rw-r--r--   0        0        0     1486 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/standalone_plugins/changed_packages/marker/added_release.py
--rw-r--r--   0        0        0     1124 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py
--rw-r--r--   0        0        0     1952 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/standalone_plugins/changed_packages/marker/changed_update.py
--rw-r--r--   0        0        0     1632 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py
--rw-r--r--   0        0        0     1278 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/standalone_plugins/changed_packages/marker/marker.py
--rw-r--r--   0        0        0     2743 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/standalone_plugins/changed_packages/package.py
--rw-r--r--   0        0        0     1028 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/standalone_plugins/common.py
--rw-r--r--   0        0        0     4616 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/standalone_plugins/last_modification.py
--rw-r--r--   0        0        0     8463 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/standalone_plugins/no_solution.py
--rw-r--r--   0        0        0     4263 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/standalone_plugins/version_updated.py
--rw-r--r--   0        0        0     6045 2023-06-15 12:27:39.531142 troubadix-23.6.0/troubadix/troubadix.py
--rw-r--r--   0        0        0     3971 1970-01-01 00:00:00.000000 troubadix-23.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-20 11:25:25.268133 troubadix-23.6.1/LICENSE
+-rw-r--r--   0        0        0     2730 2023-06-20 11:25:25.268133 troubadix-23.6.1/README.md
+-rw-r--r--   0        0        0     2516 2023-06-20 11:25:25.272133 troubadix-23.6.1/pyproject.toml
+-rw-r--r--   0        0        0      716 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/__init__.py
+-rw-r--r--   0        0        0      716 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/helper/__init__.py
+-rw-r--r--   0        0        0     8416 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/helper/test_linguistic_exception_handler.py
+-rw-r--r--   0        0        0     1940 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/helper/test_patterns.py
+-rw-r--r--   0        0        0     2396 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/__init__.py
+-rw-r--r--   0        0        0     1012 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/fail.nasl
+-rw-r--r--   0        0        0     1291 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/fail2.nasl
+-rw-r--r--   0        0        0     2100 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test.nasl
+-rw-r--r--   0        0        0     2450 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_badwords.py
+-rw-r--r--   0        0        0     5109 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_copyright_text.py
+-rw-r--r--   0        0        0     6961 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_copyright_year.py
+-rw-r--r--   0        0        0     5004 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_creation_date.py
+-rw-r--r--   0        0        0     5881 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_cve_format.py
+-rw-r--r--   0        0        0     4914 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_cvss_format.py
+-rw-r--r--   0        0        0     8970 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_dependencies.py
+-rw-r--r--   0        0        0     5808 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_dependency_category_order.py
+-rw-r--r--   0        0        0     5589 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_deprecated_dependency.py
+-rw-r--r--   0        0        0     4545 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_deprecated_functions.py
+-rw-r--r--   0        0        0     2394 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_double_end_points.py
+-rw-r--r--   0        0        0     3504 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_duplicate_oid.py
+-rw-r--r--   0        0        0     4686 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_duplicated_script_tags.py
+-rw-r--r--   0        0        0     3906 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_encoding.py
+-rw-r--r--   0        0        0     1982 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_files/fail_bad_new_line.nasl
+-rw-r--r--   0        0        0      246 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_files/fail_badwords.nasl
+-rw-r--r--   0        0        0     1979 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_files/fail_name_and_copyright_newline.nasl
+-rw-r--r--   0        0        0     1965 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_files/fail_name_newline.nasl
+-rwxr-xr-x   0        0        0     1012 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_files/fail_permissions.nasl
+-rw-r--r--   0        0        0      150 2023-06-20 11:25:25.272133 troubadix-23.6.1/tests/plugins/test_files/fail_spelling.nasl
+-rw-r--r--   0        0        0     2213 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/fail.nasl
+-rw-r--r--   0        0        0      246 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/fail_badwords.nasl
+-rw-r--r--   0        0        0     1990 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl
+-rw-r--r--   0        0        0     1987 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl
+-rw-r--r--   0        0        0     2134 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl
+-rw-r--r--   0        0        0     1023 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/runner/fail.nasl
+-rw-r--r--   0        0        0     1302 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl
+-rw-r--r--   0        0        0     2122 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/runner/test.nasl
+-rw-r--r--   0        0        0     2119 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl
+-rw-r--r--   0        0        0     1023 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/test.inc
+-rw-r--r--   0        0        0     2122 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/test.nasl
+-rw-r--r--   0        0        0     2976 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/nasl/warning.nasl
+-rw-r--r--   0        0        0     1012 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/ok_permissions.nasl
+-rw-r--r--   0        0        0     2100 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_files/test_oid.nasl
+-rw-r--r--   0        0        0     4548 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_forking_nasl_functions.py
+-rw-r--r--   0        0        0     2271 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_get_kb_on_services.py
+-rw-r--r--   0        0        0     9438 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_grammar.py
+-rw-r--r--   0        0        0     6936 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_http_links_in_tags.py
+-rw-r--r--   0        0        0     4730 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_illegal_characters.py
+-rw-r--r--   0        0        0     5965 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_log_messages.py
+-rw-r--r--   0        0        0     6174 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_malformed_dependencies.py
+-rw-r--r--   0        0        0    21051 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_misplaced_compare_in_if.py
+-rw-r--r--   0        0        0     3585 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_missing_desc_exit.py
+-rw-r--r--   0        0        0     3101 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_missing_tag_solution.py
+-rw-r--r--   0        0        0     4688 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_newlines.py
+-rw-r--r--   0        0        0    40813 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_overlong_script_tags.py
+-rw-r--r--   0        0        0     4294 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_prod_svc_detect_in_vulnvt.py
+-rw-r--r--   0        0        0     4594 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_qod.py
+-rw-r--r--   0        0        0     5844 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_reporting_consistency.py
+-rw-r--r--   0        0        0     3371 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_script_add_preference_type.py
+-rw-r--r--   0        0        0     2353 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_script_calls_empty_values.py
+-rw-r--r--   0        0        0     2799 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_script_calls_recommended.py
+-rw-r--r--   0        0        0     2650 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_script_category.py
+-rw-r--r--   0        0        0     3469 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_script_copyright.py
+-rw-r--r--   0        0        0     3877 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_script_family.py
+-rw-r--r--   0        0        0     3079 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_script_tag_form.py
+-rw-r--r--   0        0        0     6010 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_script_tag_whitespaces.py
+-rw-r--r--   0        0        0     3313 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_script_tags_mandatory.py
+-rw-r--r--   0        0        0     4858 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_script_version_and_last_modification_tags.py
+-rw-r--r--   0        0        0     3016 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_script_xref_form.py
+-rw-r--r--   0        0        0     2189 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_script_xref_url.py
+-rw-r--r--   0        0        0     6599 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_security_messages.py
+-rw-r--r--   0        0        0     3021 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_set_get_kb_calls.py
+-rw-r--r--   0        0        0     7260 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_solution_text.py
+-rw-r--r--   0        0        0     3306 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_solution_type.py
+-rw-r--r--   0        0        0     2827 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_spelling.py
+-rw-r--r--   0        0        0     1813 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_tabs.py
+-rw-r--r--   0        0        0     6297 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_todo_tbd.py
+-rw-r--r--   0        0        0     2398 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_trailing_spaces_tabs.py
+-rw-r--r--   0        0        0     3868 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_using_display.py
+-rw-r--r--   0        0        0    24134 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_valid_oid.py
+-rw-r--r--   0        0        0     4154 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_valid_script_tag_names.py
+-rw-r--r--   0        0        0     1947 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_vt_file_permissions.py
+-rw-r--r--   0        0        0     5189 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/plugins/test_vt_placement.py
+-rw-r--r--   0        0        0      716 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/__init__.py
+-rw-r--r--   0        0        0      716 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/changed_packages/__init__.py
+-rw-r--r--   0        0        0      716 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/changed_packages/markers/__init__.py
+-rw-r--r--   0        0        0     3075 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py
+-rw-r--r--   0        0        0     2620 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/changed_packages/markers/test_added_release.py
+-rw-r--r--   0        0        0     1792 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py
+-rw-r--r--   0        0        0     3258 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/changed_packages/markers/test_changed_update.py
+-rw-r--r--   0        0        0     3584 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py
+-rw-r--r--   0        0        0     3780 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/changed_packages/test_changed_packages.py
+-rw-r--r--   0        0        0     2427 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/changed_packages/test_package.py
+-rw-r--r--   0        0        0     2977 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/test_changed_cves.py
+-rw-r--r--   0        0        0     2952 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/test_changed_oid.py
+-rw-r--r--   0        0        0     3962 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/test_last_modification.py
+-rw-r--r--   0        0        0     7347 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/test_no_solution.py
+-rw-r--r--   0        0        0     6293 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/standalone_plugins/test_version_updated.py
+-rw-r--r--   0        0        0     4768 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/test_argparser.py
+-rw-r--r--   0        0        0     3947 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/test_helper.py
+-rw-r--r--   0        0        0     3671 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/test_naslinter.py
+-rw-r--r--   0        0        0     3399 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/test_reporter.py
+-rw-r--r--   0        0        0     2517 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/test_results.py
+-rw-r--r--   0        0        0    17972 2023-06-20 11:25:25.276133 troubadix-23.6.1/tests/test_runner.py
+-rw-r--r--   0        0        0      716 2023-06-20 11:25:25.276133 troubadix-23.6.1/troubadix/__init__.py
+-rw-r--r--   0        0        0      103 2023-06-20 11:25:25.276133 troubadix-23.6.1/troubadix/__version__.py
+-rw-r--r--   0        0        0     6999 2023-06-20 11:25:25.276133 troubadix-23.6.1/troubadix/argparser.py
+-rw-r--r--   0        0        0      338 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/codespell/codespell.additions
+-rw-r--r--   0        0        0   124190 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/codespell/codespell.exclude
+-rw-r--r--   0        0        0      756 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/codespell/codespell.ignore
+-rw-r--r--   0        0        0     1061 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/helper/__init__.py
+-rw-r--r--   0        0        0     3105 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/helper/helper.py
+-rw-r--r--   0        0        0     6811 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/helper/linguistic_exception_handler.py
+-rw-r--r--   0        0        0     9370 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/helper/patterns.py
+-rw-r--r--   0        0        0     3508 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugin.py
+-rw-r--r--   0        0        0     7013 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/__init__.py
+-rw-r--r--   0        0        0     4166 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/badwords.py
+-rw-r--r--   0        0        0     3583 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/copyright_text.py
+-rw-r--r--   0        0        0     3334 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/copyright_year.py
+-rw-r--r--   0        0        0     3357 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/creation_date.py
+-rw-r--r--   0        0        0     3400 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/cve_format.py
+-rw-r--r--   0        0        0     2309 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/cvss_format.py
+-rw-r--r--   0        0        0     4456 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/dependencies.py
+-rw-r--r--   0        0        0     7316 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/dependency_category_order.py
+-rw-r--r--   0        0        0     4137 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/deprecated_dependency.py
+-rw-r--r--   0        0        0     2568 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/deprecated_functions.py
+-rw-r--r--   0        0        0     2509 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/double_end_points.py
+-rw-r--r--   0        0        0     2652 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/duplicate_oid.py
+-rw-r--r--   0        0        0     3179 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/duplicated_script_tags.py
+-rw-r--r--   0        0        0     2090 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/encoding.py
+-rw-r--r--   0        0        0     6014 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/forking_nasl_functions.py
+-rw-r--r--   0        0        0     3401 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/get_kb_on_services.py
+-rw-r--r--   0        0        0     8348 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/grammar.py
+-rw-r--r--   0        0        0     7157 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/http_links_in_tags.py
+-rw-r--r--   0        0        0     4406 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/illegal_characters.py
+-rw-r--r--   0        0        0     2960 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/log_messages.py
+-rw-r--r--   0        0        0     3000 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/malformed_dependencies.py
+-rw-r--r--   0        0        0     5330 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/misplaced_compare_in_if.py
+-rw-r--r--   0        0        0     2411 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/missing_desc_exit.py
+-rw-r--r--   0        0        0     2828 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/missing_tag_solution.py
+-rw-r--r--   0        0        0     2788 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/newlines.py
+-rw-r--r--   0        0        0     2373 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/overlong_script_tags.py
+-rw-r--r--   0        0        0     4584 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/prod_svc_detect_in_vulnvt.py
+-rw-r--r--   0        0        0     3790 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/qod.py
+-rw-r--r--   0        0        0     4043 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/reporting_consistency.py
+-rw-r--r--   0        0        0     3193 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/script_add_preference_type.py
+-rw-r--r--   0        0        0     2512 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/script_calls_empty_values.py
+-rw-r--r--   0        0        0     3137 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/script_calls_recommended.py
+-rw-r--r--   0        0        0     2184 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/script_category.py
+-rw-r--r--   0        0        0     2310 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/script_copyright.py
+-rw-r--r--   0        0        0     4023 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/script_family.py
+-rw-r--r--   0        0        0     1773 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/script_tag_form.py
+-rw-r--r--   0        0        0     2172 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/script_tag_whitespaces.py
+-rw-r--r--   0        0        0     2630 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/script_tags_mandatory.py
+-rw-r--r--   0        0        0     7026 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/script_version_and_last_modification_tags.py
+-rw-r--r--   0        0        0     1848 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/script_xref_form.py
+-rw-r--r--   0        0        0     2875 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/script_xref_url.py
+-rw-r--r--   0        0        0     4708 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/security_messages.py
+-rw-r--r--   0        0        0     3415 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/set_get_kb_calls.py
+-rw-r--r--   0        0        0     5852 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/solution_text.py
+-rw-r--r--   0        0        0     2602 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/solution_type.py
+-rw-r--r--   0        0        0     9557 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/spelling.py
+-rw-r--r--   0        0        0     1319 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/tabs.py
+-rw-r--r--   0        0        0     1733 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/todo_tbd.py
+-rw-r--r--   0        0        0     2049 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/trailing_spaces_tabs.py
+-rw-r--r--   0        0        0     4046 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/using_display.py
+-rw-r--r--   0        0        0    16627 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/valid_oid.py
+-rw-r--r--   0        0        0     3447 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/valid_script_tag_names.py
+-rw-r--r--   0        0        0     3285 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/variable_assigned_in_if.py
+-rw-r--r--   0        0        0     1521 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/vt_file_permissions.py
+-rw-r--r--   0        0        0     2800 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/plugins/vt_placement.py
+-rw-r--r--   0        0        0     9176 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/reporter.py
+-rw-r--r--   0        0        0     2632 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/results.py
+-rw-r--r--   0        0        0     5172 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/runner.py
+-rw-r--r--   0        0        0       22 2023-06-20 11:25:25.280133 troubadix-23.6.1/troubadix/standalone_plugins/__init__.py
+-rw-r--r--   0        0        0     4145 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/allowed_rev_diff.py
+-rw-r--r--   0        0        0     2921 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/changed_cves.py
+-rw-r--r--   0        0        0     4074 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/changed_oid.py
+-rw-r--r--   0        0        0     5742 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/changed_packages.py
+-rw-r--r--   0        0        0      923 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/__init__.py
+-rw-r--r--   0        0        0     1797 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py
+-rw-r--r--   0        0        0     1486 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/added_release.py
+-rw-r--r--   0        0        0     1124 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py
+-rw-r--r--   0        0        0     1952 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/changed_update.py
+-rw-r--r--   0        0        0     1632 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py
+-rw-r--r--   0        0        0     1278 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/marker.py
+-rw-r--r--   0        0        0     2743 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/package.py
+-rw-r--r--   0        0        0     1028 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/common.py
+-rw-r--r--   0        0        0     4616 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/last_modification.py
+-rw-r--r--   0        0        0     8463 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/no_solution.py
+-rw-r--r--   0        0        0     4263 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/standalone_plugins/version_updated.py
+-rw-r--r--   0        0        0     6045 2023-06-20 11:25:25.284133 troubadix-23.6.1/troubadix/troubadix.py
+-rw-r--r--   0        0        0     3971 1970-01-01 00:00:00.000000 troubadix-23.6.1/PKG-INFO
```

### Comparing `troubadix-23.6.0/LICENSE` & `troubadix-23.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/README.md` & `troubadix-23.6.1/README.md`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/pyproject.toml` & `troubadix-23.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "troubadix"
-version = "23.6.0"
+version = "23.6.1"
 description = "A linting and QA check tool for NASL files"
 authors = ["Greenbone <info@greenbone.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/greenbone/troubadix"
 homepage = "https://github.com/greenbone/troubadix"
```

### Comparing `troubadix-23.6.0/tests/__init__.py` & `troubadix-23.6.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/helper/__init__.py` & `troubadix-23.6.1/tests/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/helper/test_linguistic_exception_handler.py` & `troubadix-23.6.1/tests/helper/test_linguistic_exception_handler.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/helper/test_patterns.py` & `troubadix-23.6.1/tests/helper/test_patterns.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/__init__.py` & `troubadix-23.6.1/tests/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/fail.nasl` & `troubadix-23.6.1/tests/plugins/fail.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/fail2.nasl` & `troubadix-23.6.1/tests/plugins/fail2.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test.nasl` & `troubadix-23.6.1/tests/plugins/test.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_badwords.py` & `troubadix-23.6.1/tests/plugins/test_badwords.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,7 +56,20 @@
             nasl_file=path, lines=content.splitlines()
         )
 
         plugin = CheckBadwords(fake_context)
         results = list(plugin.run())
 
         self.assertEqual(len(results), 0)
+
+    def test_exception_ok(self):
+        path = Path("some/include.inc")
+        content = '# HostDetails/NVT                 => "1.2.3.4"'
+
+        fake_context = self.create_file_plugin_context(
+            nasl_file=path, lines=content.splitlines()
+        )
+
+        plugin = CheckBadwords(fake_context)
+        results = list(plugin.run())
+
+        self.assertEqual(len(results), 0)
```

### Comparing `troubadix-23.6.0/tests/plugins/test_copyright_text.py` & `troubadix-23.6.1/tests/plugins/test_copyright_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_copyright_year.py` & `troubadix-23.6.1/tests/plugins/test_copyright_year.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_creation_date.py` & `troubadix-23.6.1/tests/plugins/test_creation_date.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_cve_format.py` & `troubadix-23.6.1/tests/plugins/test_cve_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_cvss_format.py` & `troubadix-23.6.1/tests/plugins/test_cvss_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_dependencies.py` & `troubadix-23.6.1/tests/plugins/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_dependency_category_order.py` & `troubadix-23.6.1/tests/plugins/test_dependency_category_order.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_deprecated_dependency.py` & `troubadix-23.6.1/tests/plugins/test_deprecated_dependency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_deprecated_functions.py` & `troubadix-23.6.1/tests/plugins/test_deprecated_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_double_end_points.py` & `troubadix-23.6.1/tests/plugins/test_double_end_points.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_duplicate_oid.py` & `troubadix-23.6.1/tests/plugins/test_duplicate_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_duplicated_script_tags.py` & `troubadix-23.6.1/tests/plugins/test_duplicated_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_encoding.py` & `troubadix-23.6.1/tests/plugins/test_encoding.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_files/fail_bad_new_line.nasl` & `troubadix-23.6.1/tests/plugins/test_files/fail_bad_new_line.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_files/fail_name_and_copyright_newline.nasl` & `troubadix-23.6.1/tests/plugins/test_files/fail_name_and_copyright_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_files/fail_name_newline.nasl` & `troubadix-23.6.1/tests/plugins/test_files/fail_name_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_files/fail_permissions.nasl` & `troubadix-23.6.1/tests/plugins/test_files/fail_permissions.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_files/nasl/21.04/fail.nasl` & `troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/fail.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl` & `troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/fail_name_and_copyright_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl` & `troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/fail_name_newline.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl` & `troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/fail_solution_template.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_files/nasl/21.04/runner/fail.nasl` & `troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/runner/fail.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl` & `troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/runner/fail2.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_files/nasl/21.04/runner/test.nasl` & `troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/runner/test.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl` & `troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/runner/test_valid_oid.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_files/nasl/21.04/test.inc` & `troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/test.inc`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_files/nasl/21.04/test.nasl` & `troubadix-23.6.1/tests/plugins/test_files/nasl/21.04/test.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_files/nasl/warning.nasl` & `troubadix-23.6.1/tests/plugins/test_files/nasl/warning.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_files/ok_permissions.nasl` & `troubadix-23.6.1/tests/plugins/test_files/ok_permissions.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_files/test_oid.nasl` & `troubadix-23.6.1/tests/plugins/test_files/test_oid.nasl`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_forking_nasl_functions.py` & `troubadix-23.6.1/tests/plugins/test_forking_nasl_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_get_kb_on_services.py` & `troubadix-23.6.1/tests/plugins/test_get_kb_on_services.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_grammar.py` & `troubadix-23.6.1/tests/plugins/test_grammar.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_http_links_in_tags.py` & `troubadix-23.6.1/tests/plugins/test_http_links_in_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_illegal_characters.py` & `troubadix-23.6.1/tests/plugins/test_illegal_characters.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_log_messages.py` & `troubadix-23.6.1/tests/plugins/test_log_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_malformed_dependencies.py` & `troubadix-23.6.1/tests/plugins/test_malformed_dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_misplaced_compare_in_if.py` & `troubadix-23.6.1/tests/plugins/test_misplaced_compare_in_if.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_missing_desc_exit.py` & `troubadix-23.6.1/tests/plugins/test_missing_desc_exit.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_missing_tag_solution.py` & `troubadix-23.6.1/tests/plugins/test_missing_tag_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_newlines.py` & `troubadix-23.6.1/tests/plugins/test_newlines.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_overlong_script_tags.py` & `troubadix-23.6.1/tests/plugins/test_overlong_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_prod_svc_detect_in_vulnvt.py` & `troubadix-23.6.1/tests/plugins/test_prod_svc_detect_in_vulnvt.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_qod.py` & `troubadix-23.6.1/tests/plugins/test_qod.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_reporting_consistency.py` & `troubadix-23.6.1/tests/plugins/test_reporting_consistency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_script_add_preference_type.py` & `troubadix-23.6.1/tests/plugins/test_script_add_preference_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_script_calls_empty_values.py` & `troubadix-23.6.1/tests/plugins/test_script_calls_empty_values.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_script_calls_recommended.py` & `troubadix-23.6.1/tests/plugins/test_script_calls_recommended.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_script_category.py` & `troubadix-23.6.1/tests/plugins/test_script_category.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_script_copyright.py` & `troubadix-23.6.1/tests/plugins/test_script_copyright.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_script_family.py` & `troubadix-23.6.1/tests/plugins/test_script_family.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_script_tag_form.py` & `troubadix-23.6.1/tests/plugins/test_script_tag_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_script_tag_whitespaces.py` & `troubadix-23.6.1/tests/plugins/test_script_tag_whitespaces.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_script_tags_mandatory.py` & `troubadix-23.6.1/tests/plugins/test_script_tags_mandatory.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_script_version_and_last_modification_tags.py` & `troubadix-23.6.1/tests/plugins/test_script_version_and_last_modification_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_script_xref_form.py` & `troubadix-23.6.1/tests/plugins/test_script_xref_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_script_xref_url.py` & `troubadix-23.6.1/tests/plugins/test_script_xref_url.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_security_messages.py` & `troubadix-23.6.1/tests/plugins/test_security_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_set_get_kb_calls.py` & `troubadix-23.6.1/tests/plugins/test_set_get_kb_calls.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_solution_text.py` & `troubadix-23.6.1/tests/plugins/test_solution_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_solution_type.py` & `troubadix-23.6.1/tests/plugins/test_solution_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_spelling.py` & `troubadix-23.6.1/tests/plugins/test_spelling.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_tabs.py` & `troubadix-23.6.1/tests/plugins/test_tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_todo_tbd.py` & `troubadix-23.6.1/tests/plugins/test_todo_tbd.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_trailing_spaces_tabs.py` & `troubadix-23.6.1/tests/plugins/test_trailing_spaces_tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_using_display.py` & `troubadix-23.6.1/tests/plugins/test_using_display.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_valid_oid.py` & `troubadix-23.6.1/tests/plugins/test_valid_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_valid_script_tag_names.py` & `troubadix-23.6.1/tests/plugins/test_valid_script_tag_names.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_vt_file_permissions.py` & `troubadix-23.6.1/tests/plugins/test_vt_file_permissions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/plugins/test_vt_placement.py` & `troubadix-23.6.1/tests/plugins/test_vt_placement.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/standalone_plugins/__init__.py` & `troubadix-23.6.1/tests/standalone_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/standalone_plugins/changed_packages/__init__.py` & `troubadix-23.6.1/tests/standalone_plugins/changed_packages/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/standalone_plugins/changed_packages/markers/__init__.py` & `troubadix-23.6.1/tests/standalone_plugins/changed_packages/markers/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py` & `troubadix-23.6.1/tests/standalone_plugins/changed_packages/markers/test_added_epoch.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/standalone_plugins/changed_packages/markers/test_added_release.py` & `troubadix-23.6.1/tests/standalone_plugins/changed_packages/markers/test_added_release.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py` & `troubadix-23.6.1/tests/standalone_plugins/changed_packages/markers/test_added_udeb.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/standalone_plugins/changed_packages/markers/test_changed_update.py` & `troubadix-23.6.1/tests/standalone_plugins/changed_packages/markers/test_changed_update.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py` & `troubadix-23.6.1/tests/standalone_plugins/changed_packages/markers/test_dropped_architecture.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/standalone_plugins/changed_packages/test_changed_packages.py` & `troubadix-23.6.1/tests/standalone_plugins/changed_packages/test_changed_packages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/standalone_plugins/changed_packages/test_package.py` & `troubadix-23.6.1/tests/standalone_plugins/changed_packages/test_package.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/standalone_plugins/test_changed_cves.py` & `troubadix-23.6.1/tests/standalone_plugins/test_changed_cves.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/standalone_plugins/test_changed_oid.py` & `troubadix-23.6.1/tests/standalone_plugins/test_changed_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/standalone_plugins/test_last_modification.py` & `troubadix-23.6.1/tests/standalone_plugins/test_last_modification.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/standalone_plugins/test_no_solution.py` & `troubadix-23.6.1/tests/standalone_plugins/test_no_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/standalone_plugins/test_version_updated.py` & `troubadix-23.6.1/tests/standalone_plugins/test_version_updated.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/test_argparser.py` & `troubadix-23.6.1/tests/test_argparser.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/test_helper.py` & `troubadix-23.6.1/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/test_naslinter.py` & `troubadix-23.6.1/tests/test_naslinter.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/test_reporter.py` & `troubadix-23.6.1/tests/test_reporter.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/test_results.py` & `troubadix-23.6.1/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/tests/test_runner.py` & `troubadix-23.6.1/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/__init__.py` & `troubadix-23.6.1/troubadix/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/argparser.py` & `troubadix-23.6.1/troubadix/argparser.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/codespell/codespell.exclude` & `troubadix-23.6.1/troubadix/codespell/codespell.exclude`

 * *Files 2% similar despite different names*

```diff
@@ -8,28 +8,31 @@
 # 00000008 To ensure that entries are kept unique and ordered
 # 000300Dedected burute force atack from your ip adress   <--- alternative response
     '000300Dedected burute force atack from your ip adress' >< r ||
 # 00: 33 20 2d 2d 36 20 42 61 64 20 52 65 71 75 65 73    3 --6 Bad Reques
 # 0x00:  00 11 49 6E 76 61 6C 69 64 20 63 6F 6D 6D 61 6E    ..Invalid comman
 # 0x00:  01 67 65 74 6E 61 6D 65 69 6E 66 6F 3A 20 54 65    .getnameinfo: Te
 # 0x0010:  73 65 72 20 20 20 20 20 20 48 6F 73 74 28 73 29    ser      Host(s)
+# 0x0020:  0D 0A 46 72 6F 6D 3A 20 3C 73 69 70 3A 6D 69 73    ..From: <sip:mis
 # 0x00E0:  74 65 20 69 6E 64 65 78 20 69 68 61 76 65 20 64    te index ihave d
 # 0x00F0:  75 70 6C 69 63 61 74 65 20 6D 69 6D 65 20 66 6F    uplicate mime fo
 # 0x01D0:  45 20 63 6F 6D 6D 61 6E 64 20 72 65 63 65 69 76    E command receiv
                    0x02,			# ByteOrder (little endian)
 # 0x10:  70 65 63 69 66 69 65 64 20 75 73 65 72 2E 0D 0A    pecified user...
 # 0x20:  64 79 0D 0A 45 52 52 4F 52 20 43 6F 6D 6D 61 6E    dy..ERROR Comman
 # 0x20:  6D 65 73 73 61 67 65 2E 48 61 6E 64 73 68 61 6B    message.Handshak
 # 0x50:  72 6F 2E 70 72 6F 64 75 63 74 2E 64 65 76 69 63    ro.product.devic
 # 0x50:  A1 37 43 6F 6E 6E 65 63 74 69 6F 6E 20 66 72 6F    .7Connection fro
 #0x60:  AC 13 28 D3 B3 A5 BA F0 FD D6 FA 22 BF 4D F2 4D    ..(........".M.M
   10001 from WAN (if port-forwarding is enabled to allow remote configuration, then it is a good
                      1047, "WIT",
                      1153, "Alga Automacao e controle LTDA",
                      1212, "HSA Systems",
+                     1289, "HMS/BU Ewon",
+                     1638, "Hach",
 2007-11-08  Tim Brown <timb@openvas.org>
 2008-02-20  Tim Brown <timb@openvas.org>
 2008-09-10  Tim Brown <timb@openvas.org>
 2008-09-14  Tim Brown <timb@openvas.org>
 2008-09-15  Tim Brown <timb@openvas.org>
 2008-09-18  Tim Brown <timb@openvas.org>
 2008-10-12  Tim Brown <timb@openvas.org>
@@ -51,14 +54,15 @@
                      419, "GERBI & FASE S.p.A.(Fase Saldatura)",
   # 50: 4d 4c 20 5b 0a 20 20 20 3c 21 45 4c 45 4d 45 4e    ML [.   <!ELEMEN
 # 50: 4d 4c 20 5b 0a 20 20 20 3c 21 45 4c 45 4d 45 4e    ML [.   <!ELEMEN
   # 50: 65 63 74 20 65 6e 76 65 6c 6f 70 65 20 76 61 63 ect envelope vac
 # 50: 65 63 74 20 65 6e 76 65 6c 6f 70 65 20 76 61 63 ect envelope vac
                           52, "HART Device",
  6-4c-4/01 00000411 Atom X series Readded what missing in last
+                     798, "TE Connectivity",
                           "84:BA:3B","Canon",
                      879, "PULS GmbH",
 8930 was added, Dell Inspiron Mini 9 HDA sound support was added, CIFS
                      902, "Defontaine Groupe",
                      961, "Varian Vacuum Technologies",
 '-a always,exit -F arch=b32 -S creat -S open -S openat -S truncate -S ftruncate -F exit=-EACCES -F auid>=1000 -F auid!=4294967295 -k access',
 '-a always,exit -F arch=b32 -S creat -S open -S openat -S truncate -S ftruncate -F exit=-EPERM -F auid>=1000 -F auid!=4294967295 -k access');
@@ -110,14 +114,16 @@
 An input validation issue was addressed with improved memory handling. This issue is fixed in macOS Big Sur 11.1, Security Update 2020-001 Catalina, Security Update 2020-007 Mojave. A malicious application may be able to read restricted memory.(CVE-2020-10001)");
 An issue was discovered in Linux: KVM through Improper handling of VM_IO<pipe>VM_PFNMAP vmas in KVM can bypass RO checks and can lead to pages being freed while still accessible by the VMM and guest. This allows users with the ability to start and control a VM to read/write random pages of memory and can result in local privilege escalation.(CVE-2021-22543)
 Application Centric Infrastructure (ACI) could allow an unauthenticated, adjacent attacker to cause a denial of
   Application Centric Infrastructure (ACI) mode could allow an authenticated, local attacker to
   Application Centric Infrastructure (ACI) Mode could allow an unauthenticated, remote attacker to
 Ari Kauppi from Synopsys Ltd discovered that the NFSv2 and NFSv3 server implementations do not properly handle payload bounds checking of WRITE requests. A remote attacker with write access to a NFS mount can take advantage of this flaw to read chunks of arbitrary memory from both kernel-space and user-space.
   - arm64: ptrace: Avoid setting compat FPR to garbage if get_user fails
+  - arm: pxa: add the number of DMA requestor lines (bnc#1012382).
+  - arm: pxa: fix the number of DMA requestor lines (bnc#1012382).
  ascii art thats show the arcs between that start and end points of
   as demonstrated using the Connection: TE, , Keep-Alive header.");
 - A seperate sblim-sfcb-openssl1 package was added to the SECURITY Module.
   as the original reporter of CVE-2010-1168, and Tim Bunce and Rafal
   Autoloader '%{pear_phpdir}/CAS/Autoload.php'<semicolon>");
 "bakup\n",
                           base:"cpe:/a:cas:commserver_ua:", expr:"^([0-9.]+)", insloc:location, regService:"smb-login", regPort:0);
@@ -271,14 +277,16 @@
 CVE-2020-1945: Fixed an inseure temorary file vulnerability which could
 CVE-2020-26117: Server certificates were stored as certiticate
 CVE-2020-29481: Fixed an issue which could have allowd to new domains to
 CVE-2020-36158: Fixed an issue wich might have allowed a remote
 CVE-2020-5208: Fixed multiple remote code executtion vulnerabilities
 CVE-2020-8492: Fixed a regular expression in urrlib that was prone to
 CVE-2021-30004: Fixed an issue where forging attacks might have occured
+"DataArchivingService/webcontent/aas",
+  "/DataArchivingService/webcontent/aas/aas_store.jsp");
   David Bloom and Jordi Chancel discovered that Firefox did not always
 David Bloom and Jordi Chancel discovered that Firefox did not always
   David Bloom and Jordi Chancel discovered that Thunderbird did not always
 David Bloom and Jordi Chancel discovered that Thunderbird did not always
 David Miller and Jan Lieskovsky discovered issues with the virtual address range checking of mmaped regions on the sparc architecture that may be exploited by local users to cause a denial of service.
 David Watson reported an issue in the open()/creat() system calls
 David Watson reported an issue in the open()/creat() system calls which, under certain conditions, can be exploited by local users to obtain the privileges of a group for which they are not a member.
@@ -294,26 +302,25 @@
 "developement\n",
 # |/dev/hda|ST3160021A|UNK|*||/dev/hdc|???|ERR|*||/dev/hdg|Maxtor 6B200P0|UNK|*||/dev/hdh|Maxtor 6Y160P0|38|C|
   die aktuellste Ergaenzungslieferung bezieht. Titel und Inhalt koennen sich bei einer
 Die Standard-Anforderung 'A7: Lokale Sicherheitsrichtlinien' beschreibt, dass und welche
                           dir + "/ans/ans.pl?p=../../../../../usr/bin/id|&blah" ) ) {
  * Disable all weak EXPORT ciphers by default. These can be reenabled if
 disable, or enable CAs causing various denial of service problems with
+  display debugging information to the requestor. It is recommended that such debug information be
 distrust all of DigiNotar's CAs. In this update, this is done in the
  (divide-by-zero error and QEMU process crash) via a larg... [Please see the references for more information on the vulnerabilities]");
   # <div style="float: right; margin-top: 5px; margin-right: 5px;">Rev. 1.04.06&nbsp;&nbsp;&nbsp;&nbsp;Bulid. 20150226142928 </div>
   # <div style="float: right; margin-top: 5px; margin-right: 5px;">Rev. 1.04.07&nbsp;&nbsp;&nbsp;&nbsp;Bulid. 20150925151332 </div>
  Docker compatability (#3340)
 - Don't discard stap probe note sections on aarch64 (#1225091)
 drbd: Avoid Clang warning about pointless switch statment (bsc#1051510).
 - drm/i915: Add Reenable Timer to turn Hotplug Detection back on (v4)
         egrep( string:ret, pattern:"^#?\s*-+\s*[Mm]ore\s*-+", icase:FALSE ) # nb: Huawei VRP (Yunshan)
  eliptic curve parameters were not sufficiently validated during
-  else if (AUDITLOGDAEMON_START =~ ".*Datei oder Verzeichnis nicht gefunden.*" ||  AUDITLOGDAEMON_START =~ ".*No such file or directory.*")  AUDITLOGDAEMON_START = "no audit.log";
-  else if (AUDITLOG_DATETIME =~ ".*Datei oder Verzeichnis nicht gefunden.*" ||  AUDITLOG_DATETIME =~ ".*No such file or directory.*")  AUDITLOGDATETIME_LAST = "no audit.log";
   } else if("diese Vorgabe muss manuell ueberprueft werden" >< tolower(status)) {
   else if( svc == "agobot.fo" )
 Enable log information of starting/stoping services. (bsc#1144923,
 Engineering (TE) tunnel's physical source interface is not propagated to hardware after the adjacency is lost.
   eSpace IAD, eSpace U1981 and eSpace USM.");
   establishment of the Cisco Nexus 9000 Series Application Centric Infrastructure (ACI) Mode Switch
   exact-width integer types int{N}_t and uint{N}_t.
@@ -406,49 +413,41 @@
  hypervisor crash leading to a Denial of Servce. (XSA-203, bsc#1014300,
 i40e: Fix kernel oops whe... [Please see the references for more information on the vulnerabilities]");
   ie_reg_version_id = 'oval:org.mitre.oval:obj:247';
     iexplore_file_id = 'oval:org.mitre.oval:obj:16';
     if(!appName || appName !~ "CAS.CommServerUA") continue;
     if(!appName || appName !~ "ICS Generic HART") continue;
 If a session backend is set to Apache::Session::LDAP or Apache::Session::Browseable::LDAP, then the complete fix involves upgrading the corresponding Apache::Session module (libapache-session-ldap-perl resp. libapache-session-browseable-perl) to 0.4-1+deb10u1 (or >=0.5) resp. 1.3.0-1+deb10u1 (or >=1.3.8). See related advisories DLA-3284-1 and DLA-3285-1 for details.
-  if (AUDITCONF =~ ".*Datei oder Verzeichnis nicht gefunden.*" ||  AUDITCONF =~ ".*No such file or directory.*") AUDITCONF = "no auditd.conf";
-  if (AUDITRULES =~ ".*Datei oder Verzeichnis nicht gefunden.*" ||  AUDITRULES =~ ".*No such file or directory.*") AUDITRULES = "no audit.rules";
-  if (AUDITSTATUS =~ ".*Datei oder Verzeichnis nicht gefunden.*" ||  AUDITSTATUS =~ ".*No such file or directory.*") AUDITSTATUS = "no auditctl";
 if( banner =~ " (A\. A\. Milne|Albert Einstein|Anonimo|Antico proverbio cinese|Autor desconocido|Charles Dickens|Francisco de Quevedo y Villegas|George Bernard Shaw|Jaime Balmes|Johann Wolfgang von Goethe|Jil Sander|Juana de Asbaje|Konfucius|Lord Philip Chesterfield|Montaigne|Petrarca|Ralph Waldo Emerson|Seneca|Syrus|Werner von Siemens)" ||
 if(!banner = get_kb_item("shttp/" + port + "/banner"))
 if (banner =~ "Huawei TE[0-9]0") {
 if( banner =~ "(MD|BU)-" ) {
   if( ( buf =~ "<title>GLPI - Authentification" || buf =~ "<title>GLPI - Authentication" ) && ( buf =~ "Powered By Indepnet" ||
 if( "CONEXANT SYSTEMS, INC." >< r &&
 if( "CONEXANT SYSTEMS, INC" >< r && "ACCESS RUNNER ADSL CONSOLE PORT" >< r && "LOGON PASSWORD" >< r ) {
 if( cpe =~ "^cpe:/o:huawei:te(3|4|5|6)0_firmware" ) {
   if( ">CrawlTrack informations<" >< rcvRes ) {
-    if (cryptdisks =~ ".*Datei oder Verzeichnis nicht gefunden.*" ||  cryptdisks =~ ".*No such file or directory.*") cryptdisks = "none";
-    if (crypttab =~ ".*Datei oder Verzeichnis nicht gefunden.*" ||  crypttab =~ ".*No such file or directory.*") crypttab = "none";
-  if (devaudio =~ ".*Datei oder Verzeichnis nicht gefunden.*" ||  devaudio =~ ".*No such file or directory.*") devaudio = "no audio";
 if( ect = egrep( pattern:"^Expect-CT\s*:", string:banner, icase:TRUE ) )
   if( ect_on_http )  report += '\nECT-Header:\n\n' + ect;
 if( egrep( pattern:"RTSP/1\.0 505( Protocol | RTSP | )Version [nN]ot [sS]upported", string:r ) ) {
+    if( egrep( pattern:"^[Ss]erver\s*:\s*AAS", string:banner, icase:FALSE ) ) {
+if(egrep(pattern: "^[Ss]erver\s*:\s*AAS", string: banner, icase: FALSE)) {
 if( found = egrep( string:dir_recv, pattern:"^(c:\\te?mp|/var/spool/cron|/etc/crontabs|/etc|/proc|/tmp)", icase:TRUE ) ) {
     if( fpr[0] == "[" ) {
-    if (fstab =~ ".*Datei oder Verzeichnis nicht gefunden.*" ||  fstab =~ ".*No such file or directory.*") cryptdisks = "none";
-if (fstab =~ ".*Datei oder Verzeichnis nicht gefunden.*" ||  fstab =~ ".*No such file or directory.*") fstab = "none";
 if(http_vuln_check(port:port, url:'/hag/pages/toolbox.htm',pattern:"<title>Advanced Setup", extra_check:make_list("WAN Configuration","ADSL Status"))) {
 if(http_vuln_check(port:port, url:url, pattern:"Current Configuration", extra_check:make_list("System Description","System Software Version","network parms"))) {
   if(http_vuln_check(port:port, url:url, pattern:"Password found\. Loging in\.\.\.<script>")) {
 if (http_vuln_check(port: port, url: url, pattern: "<title>WAN Setup", check_header: TRUE)) {
   if( "Huawei TE" >< banner ) {
   if( ! iif || ! ip || ! ip6 ) {
     if(in_array(search:"ro", array:options_list)){
   if (!isnull(bu[1]))
   if(!isnull(res = isdpkgvuln(pkg:"nd", ver:"0.5.0-1woody1", rls:"DEB3.0"))) {
   if(!isnull(res = isrpmvuln(pkg:"libell", rpm:"libell~0.26~1.fc31", rls:"FC31"))) {
 if( "Login successed" >< recv ) {
-  if (lssendmailcnf =~ ".*Datei oder Verzeichnis nicht gefunden.*" || lssendmailcnf =~ ".*No such file or directory.*"){
-      if (lsstatusfile =~ ".*Datei oder Verzeichnis nicht gefunden.*" ||  lsstatusfile =~ ".*No such file or directory.*") lsstatusfile = "nofile";
   If-Match, If-None-Match, If-Range, If-Unmodified-Since, Max-Forwards, TE, Host)");
 if( ( model =~ '^RP200' || model =~ '^TE[3456]0' ) && revcomp( a: version, b: "v600r006c00spc500" ) < 0) {
 if( model =~ '^TE[3456]0' && revcomp( a: version, b: "v600r006c00spc500" ) < 0 ) {
   if (mountd =~ 'program 100005 version . ready and waiting' || mountd =~ 'Program 100005 Version . ist bereit und wartet') mountd = "true";
   if( "NAM application image" >< show_ver )
   if (nfsd =~ 'program 100003 version . ready and waiting' || nfsd =~ 'Program 100003 Version . ist bereit und wartet') nfsd = "true";
                     if "nvd.nist.gov/vuln/detail/CVE-" in match.group(2) or "cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-" in match.group(2):
@@ -467,24 +466,18 @@
 if ((res = ispkgvuln(pkg:"app-admin/lsat", unaffected: make_list(), vulnerable: make_list("le 0.9.2"))) != NULL) {
   if ((res = isrpmvuln(pkg:"tre", rpm:"tre~0.8.0~18.20140228gitc2f5d13.fc23", rls:"FC23")) != NULL)
   if ((res = isrpmvuln(pkg:"tre", rpm:"tre~0.8.0~18.20140228gitc2f5d13.fc24", rls:"FC24")) != NULL)
   if ((res = isrpmvuln(pkg:"tre", rpm:"tre~0.8.0~18.20140228gitc2f5d13.fc25", rls:"FC25")) != NULL)
   if( ! res || res !~ "^HTTP/1\.[01] 200" || ( "/themes/" >!< res && "/datas/" >!< res && "/rss.php" >!< res ) )
 if(res =~ "<span>[Ss]arix&[Tt]rade;</span>" && res =~ "<span>Copyright\s*&copy;\s*[0-9]+-[0-9]+,\s*[Pp][Ee][Ll][Cc][Oo]\s*&middot;"
 if( res && "WAN SETTINGS" >< res && "value='3G Interface" >< res && "menu.html" >< res &&
-if (secretstdb =~ ".*Datei oder Verzeichnis nicht gefunden.*" ||  secretstdb =~ ".*No such file or directory.*") secretstdb = "none";
 if( "Server: Boa" >!< banner || ( "AirLive" >!< banner && banner !~ "(WL|MD|BU|POE)-") )
-if (smbconf =~ ".*Datei oder Verzeichnis nicht gefunden.*" ||  smbconf =~ ".*No such file or directory.*") smbconf = "none";
-if (smbpasswd =~ ".*Datei oder Verzeichnis nicht gefunden.*" ||  smbpasswd =~ ".*No such file or directory.*") smbpasswd = "none";
   if(strlen(res) && "nonexistant" >< res && "XJ004CSS" >< res) {
 if ("<title>Cisco NFVIS</title>" >< res && 'content="Xenon Boostrap Admin Panel"' >< res) {
 if ("<title>COMfortel</title>" >< res && "/statics/script/pageChallenge.js" >< res) {
-if (usbbus =~ ".*Datei oder Verzeichnis nicht gefunden.*" ||  usbbus =~ ".*No such file or directory.*" ) usbbus = "none";
-if (usbmodules =~ ".*Datei oder Verzeichnis nicht gefunden.*" ||  usbmodules =~ ".*No such file or directory.*" ) usbmodules = "none";
-if (usbstorage =~ ".*Datei oder Verzeichnis nicht gefunden.*" ||  usbstorage =~ ".*No such file or directory.*" || usbstorage =~ "cat: .* /sys/kernel/debug/usb/devices:.*") usbstorage = "none";
 If you disable this policy setting, transcripting of PowerShell-based applications is disabled by
 If you enable this policy setting, Windows PowerShell will enable transcripting for Windows
 	Ignore root CAs.
   iif = ssh_cmd( socket:sock, cmd:'nft list ruleset | awk \'/hook input/,/}/\' | grep \'iif "lo" accept\'', nosh:TRUE, return_errors:FALSE );
  image. This occured because of a lack of proper validation that cached
   Imaging and Communications in Medicine (DICOM) service accessible from a public WAN (Internet) /
   Imaging and Communications in Medicine (DICOM) web viewer accessible from a public WAN (Internet)
@@ -508,14 +501,15 @@
 invalid parameters for the GOST block cipher, which allows remote
   inventory fields and via the 'All softwares' search form for the 'Software name' field.");
  * iscsiadm: Optimize the the verification of mode paramters
   issue. Upstream acknowledges Tim Zingelman as the original reporter.
  It could have occured with FUSE requests. (bnc#1133190)
 item[count]     = "Norton.Thar";
 item = "EnableTranscripting";
+  - it is [mis]configured in that it does not return '404 Not Found' error codes when a non-existent
   it was added support for Cirrus Logic CS420x HDA codec, Wacom driver
 It was discovered that a buffer overflow in IFF ILBM image parsing
 It was discovered that the HSA Linux kernel driver for AMD GPU devices did
 It was discovered that the JULI logging component did not restrict its target path, resulting in potential denial of service through file overwrites.
 It was discovered that the PEAK-System Technik USB driver in the Linux
 It was discovered that the PEAK-System Technik USB driver in the ... [Please see the references for more information on the vulnerabilities]");
   It was discovered that the SBNI WAN driver did not correctly check for the
@@ -583,14 +577,15 @@
 # Mesosphere Marathon Web UI Public WAN (Internet) Accessible
     "Metastasio (Ipermestra)" >< banner || '"\r\nAnonimo' >< banner || banner =~ '^"[^"]+" *Autor desconocido[ \t\r\n]*$' || "/usr/games/fortune: not found" >< banner ||
     "Metastasio (Ipermestra)" >< r || '"\r\nAnonimo' >< r || r =~ '^"[^"]+" *Autor desconocido[ \t\r\n]*$' ) {
  MFSA 2012-27 / CVE-2012-0474: Security researchers Jordi Chancel and Eddy Bordi reported that they could short-circuit page loads to show the address of a different site than what is ... [Please see the references for more information on the vulnerabilities]");
  MFSA 2012-75 / CVE-2012-3984: Security researcher David Bloom of Cue discovered that 'select' elements are always-on-top chromeless windows and that navigation away from a page with an active 'select' menu does not remove this window.When another menu is opened programmatically on a new page, the original 'select' menu can be retained and arbitrary HTML content within it rendered, allowing an attacker to cover arbitrary portions of the new page through absolute positioning/scrolling, leading to spoofing attacks. Security researcher Jordi Chancel found a variation that would allow for click-jacking attacks was well.
  MFSA 2013-23 / CVE-2013-0765: Mozilla developer Boris Zbarsky reported that in some circumstances a wrapped WebIDL object can be wrapped multiple times, overwriting the existing wrapp... [Please see the references for more information on the vulnerabilities]");
  MFSA 2013-54 / CVE-2013-1692: Security researcher Johnathan Kuskos reported that Firefox is sending data in the body of XMLHttpRequest (XHR) HEAD requests, which goes agains the XHR specification. This can potentially be used for Cross-Site Request Forgery (CSRF) attacks against sites which do not distinguish between HEAD and POST requests.
+  (mis)configured in this way can periodically send packets with spoofed source address to keep the rate limiting
   * missing capability checks were found in the SBNI WAN driver which could
 ML^Q8<TQ^+LTL*)6UG-,[V6-;N*W*79^&[ND/.DM''*U8D?Q:.'+%RB;S$!.'
 MM]7>[YM~GC^@?_WK0@W/F>UDL^Q8<TQ^+LTL*)6UG-,[V6-;N*W*79^&[ND/
 MN*W*79^&[ND/.DM''*U8D?Q:.'+%RB;S$!.'6['*(;8>~A:>&GO>&&M7/36X
   model = "TE Unknown Model";
   mod = eregmatch(pattern: "Huawei (TE[0-9]0)", string: banner);
     mod = eregmatch( pattern:"var Model(Nmae|Name) = '(EDR-[^']+)';", string:buf );
@@ -767,14 +762,16 @@
   script_add_preference(name:"Report about unrechable Hosts", type:"checkbox", value:"no", id:6);
   script_add_preference(name:"Value", type:"entry", value:"O:BAG:BAD:(A;;RC;;;BA)", id:1);
   script_copyright("Copyright (C) 2005 Charles Thier");
   script_copyright("Copyright (C) 2008 E-Soft Inc. http://www.securityspace.com & Tim Brown");
   script_copyright("Copyright (C) 2008 Tim Brown and Vlatko Kosturjak");
   script_copyright("Copyright (C) 2009 Tim Brown");
   script_copyright("(c) Tim Brown and Portcullis Computer Security Ltd, 2008");
+  script_mandatory_keys("AAS/banner");
+  script_mandatory_keys("aas/detected");
   script_mandatory_keys("Jasig CAS server/Installed");
   script_mandatory_keys("shttp/detected");
   script_mandatory_keys("telnet/huawei/te/detected");
   script_name("AIDA64 <= 6.25.5400 SEH Buffer Overflow Vulnerability");
   script_name("Apache James Server Web Admin Public WAN (Internet) / Public LAN Accessible without Authentication");
   script_name("Apache JServ Protocol (AJP) Public WAN (Internet) / Public LAN Accessible");
   script_name("CAS CommServer UA Version Detection (Windows)");
@@ -1011,29 +1008,33 @@
     send(socket:soc,data:string("ALLO ",buff,"\r\n"));
 send(socket: soc, data: triggerD);
 "|SER",
   Series Fabric Switches in Application-Centric Infrastructure (ACI) Mode could allow an
   Series VPN Routers version 1.0.00.15 and earlier and RV340 Series Dual WAN Gigabit VPN Routers
        '    </ser>\r\n' +
        '    <ser>\r\n' +
+    # Server: AAS/<someversion>
   server accessible from a public WAN (Internet) / public LAN.");
   # Server: WebLogic Server 10.3.6.0.171017 PSU Patch for BUG26519424 TUE SEP 12 18:34:42 IST 2017
   service accessible from a public WAN (Internet) / public LAN.
   service accessible from a public WAN (Internet) / public LAN.");
   service_register( port:port, proto:"agobot.fo" );
     service_report( port:port, svc:"agobot.fo", banner:banner );
  SessionTicket extention and ECDHE-ECDSA (bsc#1015499).
+  set_kb_item(name: "aas/detected", value: TRUE);
+  set_kb_item(name: "aas/http/detected", value: TRUE);
     set_kb_item(name:"cas/commserver_ua/win/detected", value:TRUE);
     set_kb_item( name:"Jasig CAS server/Installed", value:TRUE );
   set_kb_item(name:"shttp/detected", value:TRUE);
   set_kb_item(name:"shttp/" + port + "/banner", value:banner);
   set_kb_item(name:"shttp/" + port + "/detected", value:TRUE);
     set_kb_item( name:"telnet/huawei/te/detected", value:TRUE );
 set_kb_item(name:"WMI/Antivir/UptoDate", value:AntiVir_UpDate);
     set_kb_item( name:"www/" + port + "/cas", value:version );
+set_mandatory_key( key:"AAS", regex:"^Server\s*:\s*AAS", banner:banner );
   several Nettle signature verification functions (GOST DSA, EDDSA & ECDSA) result in the Elliptic
 Several other fixes for pg_dump, which includ... [Please see the references for more information on the vulnerabilities]");
  + Short curcuit the conditional for identifying the sysconfig renderer.
   SICWEB web interface accessible from a public WAN (Internet) / public LAN and with auto-logon
 # Siemens, SIMATIC NET, RUGGEDCOM RM1224 NAM, 6GK6 108-4AM00-2DA2, HW: Version 1, FW: Version V04.01.02, SVPH8159590
 Simo Sorce discovered that Samba clients always requested
   Simo Sorce discovered that the MIT krb5 Key Distribution Center (KDC)
@@ -1244,28 +1245,30 @@
  value of divider greater than ba... [Please see the references for more information on the vulnerabilities]");
             variable_get_set = re.search('[^#](\n[ ]*#+ ?([Vv]ulnerable [Uu][Rr][Ll]|[GgSs]et|[Ss]end[s]?( (the |a )?[Rr]equest)? [Aa]nd [Rr]eceive|[Ff]etch|[Oo]pen ([Tt]he )?(UDP|udp|TCP|tcp)? ?[Ss]ocket|[Cc]los(e|ing) ([Tt]he )?(FTP|Telnet|SSH)? ?[Ss]ocket|[Cc]heck|[Ii]terate|[Tt]ry|[Cc]onfirm|[Cc]onstruct|[Bb]uild|[Gg]rep|[Rr]egister|[Cc]onstant|[Ww]indows|[Ll]inux]|[Tt]raversal_files\(\) [Ff]unction [Rr]eturns [Dd]ictionary|[Ww]ait|[Ss]leep)[s]?(ing)?(ed)?(ation)?[^\r\n]*)', text)
         variable_get_set = re.search('[^#](\n[ ]*#+ ?([Vv]ulnerable [Uu][Rr][Ll]|[GgSs]et|[Ss]end[s]?( (the |a )?[Rr]equest)? [Aa]nd [Rr]eceive|[Ff]etch|[Oo]pen ([Tt]he )?(UDP|udp|TCP|tcp)? ?[Ss]ocket|[Cc]los(e|ing) ([Tt]he )?(FTP|Telnet|SSH)? ?[Ss]ocket|[Cc]heck|[Ii]terate|[Tt]ry|[Cc]onfirm|[Cc]onstruct|[Bb]uild|[Gg]rep|[Rr]egister|[Cc]onstant|[Ww]indows|[Ll]inux]|[Tt]raversal_files\(\) [Ff]unction [Rr]eturns [Dd]ictionary|[Ww]ait|[Ss]leep)[s]?(ing)?(ed)?(ation)?[^\r\n]*)', text)
 Vegard Nossum reported an issue with the UNIX socket garbage collector. Local users can consume all of LOWMEM and decrease system performance by overloading the system with inflight sockets.
   vers = eregmatch( pattern:"mandr(iva|ake).*inux ?(enterprise server)? release ([0-9.]+)", string:rls, icase:TRUE );
   vers = eregmatch(pattern: ">Rev\. ([0-9.]+)([^<]+Bu(li|il)d\. ([0-9]+))?", string: res);
       version = eregmatch( pattern:"Powered by.*ANG(</a>)? ([0-9.]+)", string:res );
+  version = eregmatch(string: banner, pattern: "^[Ss]erver\s*:\s*AAS/([0-9.]+)", icase: FALSE);
 version of nd.
   vers = ssh_get_bin_version(full_prog_name:file, version_argv:"--version", ver_pattern:"Kerberos 5 [Rr]elease ([0-9.]+)", sock:sock);
  + vfs_recycle: Prevent flooding the log if we're called on non-existant
     vgx_file_id = 'oval:org.mitre.oval:obj:308';
     vgx_file_variable_id = 'oval:org.mitre.oval:var:209';
 via crafted description chunks in a CAF audio file, leading to a
   vulnerability by flooding an adjacent IOS XE device with specific ND messages.");
   vulnerability by sending crafted IPv6 Neighbor Discovery (ND) packets to an affected device for
 vuln_url = "/olt/Login.do/../../olt/UploadFileUpload.do";
 # WAN Emulator Remote Command Execution Vulnerabilities
        && '">WAN IP<' >< res && '">LAN IP<' >< res ) {
     # WAN Miniport (IPv6)|5|(null)|(null)
 Wan-Teh Chang as the original reporters of CVE-2013-5607.
   web-based interface for Cisco Small Business RV320 and RV325 Dual Gigabit WAN VPN Routers could
+  webcontent/aas/aas_store.jsp.");
 Wen Guanxing discovered that PCRE incorrectly handled certain regular
 Wen Xu and Po-Ning Tseng discovered that btrfs file system implementation
 Wen Xu and Po-Ning Tseng discovered that the btrfs filesystem
 Wen Xu and wushi of KeenTeam discovered that users allowed to create
 Wen Xu discovered an integer overflow issue in the Angle library.
 Wen Xu discovered an out-of-bounds read issue in the v8 library.
 Wen Xu discovered a use-after-free flaw in the Linux kernel's ipv4 ping
@@ -1288,14 +1291,15 @@
   which ultimately allows for overwriting Structured Exception Handler (SEH) addresses and the
   Wide Area Network (WAN) Settings and 'addURLFilter', 'addHostFilter'
 will execute user defined network requests to both WAN and LAN clients. A remote unauthenticated attacker can use
     win32k_file_id = 'oval:org.mitre.oval:obj:570';
     win32k_file_variable_id = 'oval:org.mitre.oval:var:200';
     winsrv_file_id = 'oval:org.mitre.oval:obj:1382';
     winsrv_file_variable_id = 'oval:org.mitre.oval:var:200';
+  withheld from the requestor.");
 With this update, the ACI check is stopped when the ACI is going to be
 "/wls-wsat/CoordinatorPortType11", "weblogic\.wsee\.wstx\.wsat\.v1[01]\.endpoint\.CoordinatorPort",
 "/wls-wsat/CoordinatorPortType", "weblogic\.wsee\.wstx\.wsat\.v1[01]\.endpoint\.CoordinatorPort",
 "/wls-wsat/ParticipantPortType11", "weblogic\.wsee\.wstx\.wsat\.v1[01]\.endpoint\.ParticipantPort",
 "/wls-wsat/ParticipantPortType", "weblogic\.wsee\.wstx\.wsat\.v1[01]\.endpoint\.ParticipantPort",
 "/wls-wsat/RegistrationPortTypeRPC11", "weblogic\.wsee\.wstx\.wsc\.v1[01]\.endpoint\.RegistrationPort");
 "/wls-wsat/RegistrationPortTypeRPC", "weblogic\.wsee\.wstx\.wsc\.v1[01]\.endpoint\.RegistrationPort",
```

### Comparing `troubadix-23.6.0/troubadix/codespell/codespell.ignore` & `troubadix-23.6.1/troubadix/codespell/codespell.ignore`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/helper/__init__.py` & `troubadix-23.6.1/troubadix/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/helper/helper.py` & `troubadix-23.6.1/troubadix/helper/helper.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/helper/linguistic_exception_handler.py` & `troubadix-23.6.1/troubadix/helper/linguistic_exception_handler.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/helper/patterns.py` & `troubadix-23.6.1/troubadix/helper/patterns.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugin.py` & `troubadix-23.6.1/troubadix/plugin.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/__init__.py` & `troubadix-23.6.1/troubadix/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/badwords.py` & `troubadix-23.6.1/troubadix/plugins/badwords.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,20 @@
 # hexstr(openvas) = '6f70656e766173'
 DEFAULT_BADWORDS = [
     "cracker",
     "openvas",
     "OpenVAS",
     "4f70656e564153",
     "6f70656e766173",
+    # nb:
+    # - VT should be used instead
+    # - using a space before/after to make the check a little bit more strict
+    # - this could be made less strict later once the whole feed is "clean"
+    "NVT ",
+    " NVT",
 ]
 
 _IGNORE_FILES = [
     "gb_openvas",
     "gb_gsa_",
     "http_func.inc",
     "misc_func.inc",
@@ -75,14 +81,16 @@
     "OpenVAS / Greenbone Vulnerability Manager",
     "openvas_1808149858",
     "evil.zip -> openvas.jsp",
     'url = "/openvas.jsp";',
     'if( "OpenVAS RCE Test" >< buf )',
     'the file "/openvas.jsp" was created',
     "/var/lib/openvas/plugins/",
+    "INVT ",  # INVT Electric VT Designer
+    "HostDetails/NVT",  # Can't be changed right now...
 ]
 
 STARTS_WITH_EXCEPTIONS = [
     "# OpenVAS Vulnerability Test",
     "# OpenVAS Include File",
     "  script_",
     "# $Id: ",
@@ -116,13 +124,18 @@
                         for start in STARTS_WITH_EXCEPTIONS
                     )
                     and not any(
                         nasl_file.name == filename and value in line
                         for filename, value in COMBINED
                     )
                 ):
+                    report = f"Badword in line {i:5}: {line}"
+                    if "NVT" in line:
+                        report += (
+                            '\nNote/Hint: Please use the term "VT" instead.'
+                        )
                     yield LinterError(
-                        f"Badword in line {i:5}: {line}",
+                        report,
                         plugin=self.name,
                         file=nasl_file,
                         line=i,
                     )
```

### Comparing `troubadix-23.6.0/troubadix/plugins/copyright_text.py` & `troubadix-23.6.1/troubadix/plugins/copyright_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/copyright_year.py` & `troubadix-23.6.1/troubadix/plugins/copyright_year.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/creation_date.py` & `troubadix-23.6.1/troubadix/plugins/creation_date.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/cve_format.py` & `troubadix-23.6.1/troubadix/plugins/cve_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/cvss_format.py` & `troubadix-23.6.1/troubadix/plugins/cvss_format.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/dependencies.py` & `troubadix-23.6.1/troubadix/plugins/dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/dependency_category_order.py` & `troubadix-23.6.1/troubadix/plugins/dependency_category_order.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/deprecated_dependency.py` & `troubadix-23.6.1/troubadix/plugins/deprecated_dependency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/deprecated_functions.py` & `troubadix-23.6.1/troubadix/plugins/deprecated_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/double_end_points.py` & `troubadix-23.6.1/troubadix/plugins/double_end_points.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/duplicate_oid.py` & `troubadix-23.6.1/troubadix/plugins/duplicate_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/duplicated_script_tags.py` & `troubadix-23.6.1/troubadix/plugins/duplicated_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/encoding.py` & `troubadix-23.6.1/troubadix/plugins/encoding.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/forking_nasl_functions.py` & `troubadix-23.6.1/troubadix/plugins/forking_nasl_functions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/get_kb_on_services.py` & `troubadix-23.6.1/troubadix/plugins/get_kb_on_services.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/grammar.py` & `troubadix-23.6.1/troubadix/plugins/grammar.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/http_links_in_tags.py` & `troubadix-23.6.1/troubadix/plugins/http_links_in_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/illegal_characters.py` & `troubadix-23.6.1/troubadix/plugins/illegal_characters.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/log_messages.py` & `troubadix-23.6.1/troubadix/plugins/log_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/malformed_dependencies.py` & `troubadix-23.6.1/troubadix/plugins/malformed_dependencies.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/misplaced_compare_in_if.py` & `troubadix-23.6.1/troubadix/plugins/misplaced_compare_in_if.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/missing_desc_exit.py` & `troubadix-23.6.1/troubadix/plugins/missing_desc_exit.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/missing_tag_solution.py` & `troubadix-23.6.1/troubadix/plugins/missing_tag_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/newlines.py` & `troubadix-23.6.1/troubadix/plugins/newlines.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/overlong_script_tags.py` & `troubadix-23.6.1/troubadix/plugins/overlong_script_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/prod_svc_detect_in_vulnvt.py` & `troubadix-23.6.1/troubadix/plugins/prod_svc_detect_in_vulnvt.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/qod.py` & `troubadix-23.6.1/troubadix/plugins/qod.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/reporting_consistency.py` & `troubadix-23.6.1/troubadix/plugins/reporting_consistency.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/script_add_preference_type.py` & `troubadix-23.6.1/troubadix/plugins/script_add_preference_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/script_calls_empty_values.py` & `troubadix-23.6.1/troubadix/plugins/script_calls_empty_values.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/script_calls_recommended.py` & `troubadix-23.6.1/troubadix/plugins/script_calls_recommended.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/script_category.py` & `troubadix-23.6.1/troubadix/plugins/script_category.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/script_copyright.py` & `troubadix-23.6.1/troubadix/plugins/script_copyright.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/script_family.py` & `troubadix-23.6.1/troubadix/plugins/script_family.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/script_tag_form.py` & `troubadix-23.6.1/troubadix/plugins/script_tag_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/script_tag_whitespaces.py` & `troubadix-23.6.1/troubadix/plugins/script_tag_whitespaces.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/script_tags_mandatory.py` & `troubadix-23.6.1/troubadix/plugins/script_tags_mandatory.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/script_version_and_last_modification_tags.py` & `troubadix-23.6.1/troubadix/plugins/script_version_and_last_modification_tags.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/script_xref_form.py` & `troubadix-23.6.1/troubadix/plugins/script_xref_form.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/script_xref_url.py` & `troubadix-23.6.1/troubadix/plugins/script_xref_url.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/security_messages.py` & `troubadix-23.6.1/troubadix/plugins/security_messages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/set_get_kb_calls.py` & `troubadix-23.6.1/troubadix/plugins/set_get_kb_calls.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/solution_text.py` & `troubadix-23.6.1/troubadix/plugins/solution_text.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/solution_type.py` & `troubadix-23.6.1/troubadix/plugins/solution_type.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/spelling.py` & `troubadix-23.6.1/troubadix/plugins/spelling.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/tabs.py` & `troubadix-23.6.1/troubadix/plugins/tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/todo_tbd.py` & `troubadix-23.6.1/troubadix/plugins/todo_tbd.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/trailing_spaces_tabs.py` & `troubadix-23.6.1/troubadix/plugins/trailing_spaces_tabs.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/using_display.py` & `troubadix-23.6.1/troubadix/plugins/using_display.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/valid_oid.py` & `troubadix-23.6.1/troubadix/plugins/valid_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/valid_script_tag_names.py` & `troubadix-23.6.1/troubadix/plugins/valid_script_tag_names.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/variable_assigned_in_if.py` & `troubadix-23.6.1/troubadix/plugins/variable_assigned_in_if.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/vt_file_permissions.py` & `troubadix-23.6.1/troubadix/plugins/vt_file_permissions.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/plugins/vt_placement.py` & `troubadix-23.6.1/troubadix/plugins/vt_placement.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/reporter.py` & `troubadix-23.6.1/troubadix/reporter.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/results.py` & `troubadix-23.6.1/troubadix/results.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/runner.py` & `troubadix-23.6.1/troubadix/runner.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/standalone_plugins/allowed_rev_diff.py` & `troubadix-23.6.1/troubadix/standalone_plugins/allowed_rev_diff.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/standalone_plugins/changed_cves.py` & `troubadix-23.6.1/troubadix/standalone_plugins/changed_cves.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/standalone_plugins/changed_oid.py` & `troubadix-23.6.1/troubadix/standalone_plugins/changed_oid.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/standalone_plugins/changed_packages/changed_packages.py` & `troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/changed_packages.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/standalone_plugins/changed_packages/marker/__init__.py` & `troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/__init__.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py` & `troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/added_epoch.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/standalone_plugins/changed_packages/marker/added_release.py` & `troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/added_release.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py` & `troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/added_udeb.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/standalone_plugins/changed_packages/marker/changed_update.py` & `troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/changed_update.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py` & `troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/dropped_architecture.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/standalone_plugins/changed_packages/marker/marker.py` & `troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/marker/marker.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/standalone_plugins/changed_packages/package.py` & `troubadix-23.6.1/troubadix/standalone_plugins/changed_packages/package.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/standalone_plugins/common.py` & `troubadix-23.6.1/troubadix/standalone_plugins/common.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/standalone_plugins/last_modification.py` & `troubadix-23.6.1/troubadix/standalone_plugins/last_modification.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/standalone_plugins/no_solution.py` & `troubadix-23.6.1/troubadix/standalone_plugins/no_solution.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/standalone_plugins/version_updated.py` & `troubadix-23.6.1/troubadix/standalone_plugins/version_updated.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/troubadix/troubadix.py` & `troubadix-23.6.1/troubadix/troubadix.py`

 * *Files identical despite different names*

### Comparing `troubadix-23.6.0/PKG-INFO` & `troubadix-23.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troubadix
-Version: 23.6.0
+Version: 23.6.1
 Summary: A linting and QA check tool for NASL files
 Home-page: https://github.com/greenbone/troubadix
 License: GPL-3.0-or-later
 Author: Greenbone
 Author-email: info@greenbone.net
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

