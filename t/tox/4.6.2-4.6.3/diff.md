# Comparing `tmp/tox-4.6.2.tar.gz` & `tmp/tox-4.6.3.tar.gz`

## Comparing `tox-4.6.2.tar` & `tox-4.6.3.tar`

### file list

```diff
@@ -1,221 +1,221 @@
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 tox-4.6.2/tox.ini
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/__init__.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/__main__.py
--rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/provision.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/py.typed
--rw-r--r--   0        0        0    19660 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/pytest.py
--rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/report.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/run.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/__init__.py
--rw-r--r--   0        0        0     6570 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/main.py
--rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/of_type.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/set_env.py
--rw-r--r--   0        0        0     9990 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/sets.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/cli/__init__.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/cli/env_var.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/cli/ini.py
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/cli/parse.py
--rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/cli/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/loader/__init__.py
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/loader/api.py
--rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/loader/convert.py
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/loader/memory.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/loader/section.py
--rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/loader/str_convert.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/loader/stringify.py
--rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/loader/ini/__init__.py
--rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/loader/ini/factor.py
--rw-r--r--   0        0        0    13404 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/loader/ini/replace.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/source/__init__.py
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/source/api.py
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/source/discover.py
--rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/source/ini.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/source/ini_section.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/source/legacy_toml.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/source/setup_cfg.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/config/source/tox_ini.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/execute/__init__.py
--rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/execute/api.py
--rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/execute/pep517_backend.py
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/execute/request.py
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/execute/stream.py
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/execute/util.py
--rw-r--r--   0        0        0    14099 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/execute/local_sub_process/__init__.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/execute/local_sub_process/read_via_thread.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/execute/local_sub_process/read_via_thread_unix.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/execute/local_sub_process/read_via_thread_windows.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/journal/__init__.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/journal/env.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/journal/main.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/plugin/__init__.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/plugin/inline.py
--rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/plugin/manager.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/plugin/spec.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/__init__.py
--rw-r--r--   0        0        0    18474 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/env_select.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/__init__.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/depends.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/devenv.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/exec_.py
--rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/legacy.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/list_env.py
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/quickstart.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/show_config.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/version_flag.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/run/__init__.py
--rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/run/common.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/run/parallel.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/run/sequential.py
--rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/session/cmd/run/single.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/__init__.py
--rw-r--r--   0        0        0    20287 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/api.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/errors.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/info.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/installer.py
--rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/package.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/register.py
--rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/runner.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/__init__.py
--rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/api.py
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/package.py
--rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/pip/__init__.py
--rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/pip/pip_install.py
--rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/pip/req_file.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/pip/req/__init__.py
--rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/pip/req/args.py
--rw-r--r--   0        0        0    19762 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/pip/req/file.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/pip/req/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/virtual_env/__init__.py
--rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/virtual_env/api.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/virtual_env/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/virtual_env/package/__init__.py
--rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/virtual_env/package/cmd_builder.py
--rw-r--r--   0        0        0    17905 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/virtual_env/package/pyproject.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/tox_env/python/virtual_env/package/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/util/__init__.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/util/ci.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/util/cpu.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/util/file_view.py
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/util/graph.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/util/path.py
--rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 tox-4.6.2/src/tox/util/spinner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/__init__.py
--rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 tox-4.6.2/tests/conftest.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 tox-4.6.2/tests/test_call_modes.py
--rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 tox-4.6.2/tests/test_provision.py
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 tox-4.6.2/tests/test_report.py
--rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 tox-4.6.2/tests/test_run.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 tox-4.6.2/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/__init__.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/conftest.py
--rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/test_main.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/test_of_types.py
--rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/test_set_env.py
--rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/test_sets.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/test_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/cli/__init__.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/cli/conftest.py
--rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/cli/test_cli_env_var.py
--rw-r--r--   0        0        0     7422 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/cli/test_cli_ini.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/cli/test_parse.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/cli/test_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/__init__.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/test_loader.py
--rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/test_memory_loader.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/test_section.py
--rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/test_str_convert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/__init__.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/conftest.py
--rw-r--r--   0        0        0     6501 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/test_factor.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/test_ini_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/replace/__init__.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/replace/conftest.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/replace/test_replace.py
--rw-r--r--   0        0        0     7230 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/replace/test_replace_env_var.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/replace/test_replace_os_pathsep.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/replace/test_replace_os_sep.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/replace/test_replace_posargs.py
--rw-r--r--   0        0        0     8310 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/replace/test_replace_tox_env.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/loader/ini/replace/test_replace_tty.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/source/__init__.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/source/test_discover.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/source/test_legacy_toml.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/source/test_setup_cfg.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 tox-4.6.2/tests/config/source/test_source_ini.py
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 tox-4.6.2/tests/demo_pkg_inline/build.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tox-4.6.2/tests/demo_pkg_inline/pyproject.toml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 tox-4.6.2/tests/demo_pkg_setuptools/pyproject.toml
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tox-4.6.2/tests/demo_pkg_setuptools/setup.cfg
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 tox-4.6.2/tests/demo_pkg_setuptools/demo_pkg_setuptools/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/execute/__init__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tox-4.6.2/tests/execute/conftest.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tox-4.6.2/tests/execute/test_request.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tox-4.6.2/tests/execute/test_stream.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/execute/local_subprocess/__init__.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 tox-4.6.2/tests/execute/local_subprocess/bad_process.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 tox-4.6.2/tests/execute/local_subprocess/local_subprocess_sigint.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 tox-4.6.2/tests/execute/local_subprocess/test_execute_util.py
--rw-r--r--   0        0        0    14176 2020-02-02 00:00:00.000000 tox-4.6.2/tests/execute/local_subprocess/test_local_subprocess.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 tox-4.6.2/tests/execute/local_subprocess/tty_check.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/journal/__init__.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 tox-4.6.2/tests/journal/test_main_journal.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tox-4.6.2/tests/plugin/conftest.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 tox-4.6.2/tests/plugin/test_inline.py
--rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 tox-4.6.2/tests/plugin/test_plugin.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 tox-4.6.2/tests/plugin/test_plugin_custom_config_set.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/pytest_/__init__.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 tox-4.6.2/tests/pytest_/test_init.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/__init__.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/test_env_select.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/test_session_common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/__init__.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/test_depends.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/test_devenv.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/test_exec_.py
--rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/test_legacy.py
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/test_list_envs.py
--rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/test_parallel.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/test_quickstart.py
--rw-r--r--   0        0        0    18755 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/test_sequential.py
--rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/test_show_config.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/test_state.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/run/__init__.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 tox-4.6.2/tests/session/cmd/run/test_common.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/__init__.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/test_api.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/test_info.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/test_register.py
--rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/test_tox_env_api.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/test_tox_env_runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/__init__.py
--rw-r--r--   0        0        0     9327 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/test_python_api.py
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/test_python_runner.py
--rw-r--r--   0        0        0    17085 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/pip/test_pip_install.py
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/pip/test_req_file.py
--rw-r--r--   0        0        0    22171 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/pip/req/test_file.py
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/test-pkg/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/virtual_env/__init__.py
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/virtual_env/test_setuptools.py
--rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/virtual_env/test_virtualenv_api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/virtual_env/package/__init__.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/virtual_env/package/conftest.py
--rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py
--rw-r--r--   0        0        0    11235 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/virtual_env/package/test_package_pyproject.py
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 tox-4.6.2/tests/tox_env/python/virtual_env/package/test_python_package_util.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 tox-4.6.2/tests/type_check/add_config_container_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.2/tests/util/__init__.py
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 tox-4.6.2/tests/util/test_ci.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 tox-4.6.2/tests/util/test_cpu.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 tox-4.6.2/tests/util/test_graph.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tox-4.6.2/tests/util/test_path.py
--rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 tox-4.6.2/tests/util/test_spinner.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tox-4.6.2/.gitignore
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox-4.6.2/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 tox-4.6.2/README.md
--rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 tox-4.6.2/pyproject.toml
--rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 tox-4.6.2/PKG-INFO
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 tox-4.6.3/tox.ini
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/__init__.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/__main__.py
+-rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/provision.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/py.typed
+-rw-r--r--   0        0        0    19660 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/pytest.py
+-rw-r--r--   0        0        0     8283 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/report.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/run.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/__init__.py
+-rw-r--r--   0        0        0     6570 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/main.py
+-rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/of_type.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/set_env.py
+-rw-r--r--   0        0        0     9990 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/sets.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/cli/__init__.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/cli/env_var.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/cli/ini.py
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/cli/parse.py
+-rw-r--r--   0        0        0    13738 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/cli/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/loader/__init__.py
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/loader/api.py
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/loader/convert.py
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/loader/memory.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/loader/section.py
+-rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/loader/str_convert.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/loader/stringify.py
+-rw-r--r--   0        0        0     3966 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/loader/ini/__init__.py
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/loader/ini/factor.py
+-rw-r--r--   0        0        0    13404 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/loader/ini/replace.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/source/__init__.py
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/source/api.py
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/source/discover.py
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/source/ini.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/source/ini_section.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/source/legacy_toml.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/source/setup_cfg.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/config/source/tox_ini.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/execute/__init__.py
+-rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/execute/api.py
+-rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/execute/pep517_backend.py
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/execute/request.py
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/execute/stream.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/execute/util.py
+-rw-r--r--   0        0        0    14099 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/execute/local_sub_process/__init__.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/execute/local_sub_process/read_via_thread.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/execute/local_sub_process/read_via_thread_unix.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/execute/local_sub_process/read_via_thread_windows.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/journal/__init__.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/journal/env.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/journal/main.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/plugin/__init__.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/plugin/inline.py
+-rw-r--r--   0        0        0     3702 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/plugin/manager.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/plugin/spec.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/__init__.py
+-rw-r--r--   0        0        0    18474 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/env_select.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/__init__.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/depends.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/devenv.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/exec_.py
+-rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/legacy.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/list_env.py
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/quickstart.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/show_config.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/version_flag.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/run/__init__.py
+-rw-r--r--   0        0        0    17515 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/run/common.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/run/parallel.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/run/sequential.py
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/session/cmd/run/single.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/__init__.py
+-rw-r--r--   0        0        0    20287 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/api.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/errors.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/info.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/installer.py
+-rw-r--r--   0        0        0     3636 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/package.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/register.py
+-rw-r--r--   0        0        0     7824 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/runner.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/__init__.py
+-rw-r--r--   0        0        0    10989 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/api.py
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/package.py
+-rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/pip/__init__.py
+-rw-r--r--   0        0        0    10567 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/pip/pip_install.py
+-rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/pip/req_file.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/pip/req/__init__.py
+-rw-r--r--   0        0        0     4319 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/pip/req/args.py
+-rw-r--r--   0        0        0    19762 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/pip/req/file.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/pip/req/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/virtual_env/__init__.py
+-rw-r--r--   0        0        0     6453 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/virtual_env/api.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/virtual_env/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/virtual_env/package/__init__.py
+-rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/virtual_env/package/cmd_builder.py
+-rw-r--r--   0        0        0    18379 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/virtual_env/package/pyproject.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/tox_env/python/virtual_env/package/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/util/__init__.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/util/ci.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/util/cpu.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/util/file_view.py
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/util/graph.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/util/path.py
+-rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 tox-4.6.3/src/tox/util/spinner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/__init__.py
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 tox-4.6.3/tests/conftest.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 tox-4.6.3/tests/test_call_modes.py
+-rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 tox-4.6.3/tests/test_provision.py
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 tox-4.6.3/tests/test_report.py
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 tox-4.6.3/tests/test_run.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 tox-4.6.3/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/__init__.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/conftest.py
+-rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/test_main.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/test_of_types.py
+-rw-r--r--   0        0        0     5828 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/test_set_env.py
+-rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/test_sets.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/test_types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/cli/__init__.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/cli/conftest.py
+-rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/cli/test_cli_env_var.py
+-rw-r--r--   0        0        0     7422 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/cli/test_cli_ini.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/cli/test_parse.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/cli/test_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/__init__.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/test_loader.py
+-rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/test_memory_loader.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/test_section.py
+-rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/test_str_convert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/__init__.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/conftest.py
+-rw-r--r--   0        0        0     6501 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/test_factor.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/test_ini_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/replace/__init__.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/replace/conftest.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/replace/test_replace.py
+-rw-r--r--   0        0        0     7230 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/replace/test_replace_env_var.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/replace/test_replace_os_pathsep.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/replace/test_replace_os_sep.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/replace/test_replace_posargs.py
+-rw-r--r--   0        0        0     8310 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/replace/test_replace_tox_env.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/loader/ini/replace/test_replace_tty.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/source/__init__.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/source/test_discover.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/source/test_legacy_toml.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/source/test_setup_cfg.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 tox-4.6.3/tests/config/source/test_source_ini.py
+-rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 tox-4.6.3/tests/demo_pkg_inline/build.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tox-4.6.3/tests/demo_pkg_inline/pyproject.toml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 tox-4.6.3/tests/demo_pkg_setuptools/pyproject.toml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tox-4.6.3/tests/demo_pkg_setuptools/setup.cfg
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 tox-4.6.3/tests/demo_pkg_setuptools/demo_pkg_setuptools/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/execute/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 tox-4.6.3/tests/execute/conftest.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 tox-4.6.3/tests/execute/test_request.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tox-4.6.3/tests/execute/test_stream.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/execute/local_subprocess/__init__.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 tox-4.6.3/tests/execute/local_subprocess/bad_process.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 tox-4.6.3/tests/execute/local_subprocess/local_subprocess_sigint.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 tox-4.6.3/tests/execute/local_subprocess/test_execute_util.py
+-rw-r--r--   0        0        0    14176 2020-02-02 00:00:00.000000 tox-4.6.3/tests/execute/local_subprocess/test_local_subprocess.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 tox-4.6.3/tests/execute/local_subprocess/tty_check.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/journal/__init__.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 tox-4.6.3/tests/journal/test_main_journal.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tox-4.6.3/tests/plugin/conftest.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 tox-4.6.3/tests/plugin/test_inline.py
+-rw-r--r--   0        0        0     9176 2020-02-02 00:00:00.000000 tox-4.6.3/tests/plugin/test_plugin.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 tox-4.6.3/tests/plugin/test_plugin_custom_config_set.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/pytest_/__init__.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 tox-4.6.3/tests/pytest_/test_init.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/__init__.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/test_env_select.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/test_session_common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/__init__.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/test_depends.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/test_devenv.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/test_exec_.py
+-rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/test_legacy.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/test_list_envs.py
+-rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/test_parallel.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/test_quickstart.py
+-rw-r--r--   0        0        0    18755 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/test_sequential.py
+-rw-r--r--   0        0        0    11254 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/test_show_config.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/test_state.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/run/__init__.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 tox-4.6.3/tests/session/cmd/run/test_common.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/__init__.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/test_api.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/test_info.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/test_register.py
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/test_tox_env_api.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/test_tox_env_runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/__init__.py
+-rw-r--r--   0        0        0     9327 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/test_python_api.py
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/test_python_runner.py
+-rw-r--r--   0        0        0    17085 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/pip/test_pip_install.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/pip/test_req_file.py
+-rw-r--r--   0        0        0    22171 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/pip/req/test_file.py
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/test-pkg/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/virtual_env/__init__.py
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/virtual_env/test_setuptools.py
+-rw-r--r--   0        0        0     6603 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/virtual_env/test_virtualenv_api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/virtual_env/package/__init__.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/virtual_env/package/conftest.py
+-rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py
+-rw-r--r--   0        0        0    11285 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/virtual_env/package/test_package_pyproject.py
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 tox-4.6.3/tests/tox_env/python/virtual_env/package/test_python_package_util.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 tox-4.6.3/tests/type_check/add_config_container_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox-4.6.3/tests/util/__init__.py
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 tox-4.6.3/tests/util/test_ci.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 tox-4.6.3/tests/util/test_cpu.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 tox-4.6.3/tests/util/test_graph.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 tox-4.6.3/tests/util/test_path.py
+-rw-r--r--   0        0        0     5150 2020-02-02 00:00:00.000000 tox-4.6.3/tests/util/test_spinner.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tox-4.6.3/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox-4.6.3/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 tox-4.6.3/README.md
+-rw-r--r--   0        0        0     5335 2020-02-02 00:00:00.000000 tox-4.6.3/pyproject.toml
+-rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 tox-4.6.3/PKG-INFO
```

### Comparing `tox-4.6.2/tox.ini` & `tox-4.6.3/tox.ini`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/provision.py` & `tox-4.6.3/src/tox/provision.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/pytest.py` & `tox-4.6.3/src/tox/pytest.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/report.py` & `tox-4.6.3/src/tox/report.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/run.py` & `tox-4.6.3/src/tox/run.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/config/main.py` & `tox-4.6.3/src/tox/config/main.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/config/of_type.py` & `tox-4.6.3/src/tox/config/of_type.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/config/set_env.py` & `tox-4.6.3/src/tox/config/set_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/config/sets.py` & `tox-4.6.3/src/tox/config/sets.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/config/types.py` & `tox-4.6.3/src/tox/config/types.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/config/cli/env_var.py` & `tox-4.6.3/src/tox/config/cli/env_var.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/config/cli/ini.py` & `tox-4.6.3/src/tox/config/cli/ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/config/cli/parse.py` & `tox-4.6.3/src/tox/config/cli/parse.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/config/cli/parser.py` & `tox-4.6.3/src/tox/config/cli/parser.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/config/loader/api.py` & `tox-4.6.3/src/tox/config/loader/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/config/loader/convert.py` & `tox-4.6.3/src/tox/config/loader/convert.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/config/loader/memory.py` & `tox-4.6.3/src/tox/config/loader/memory.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/config/loader/section.py` & `tox-4.6.3/src/tox/config/loader/section.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/config/loader/str_convert.py` & `tox-4.6.3/src/tox/config/loader/str_convert.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/config/loader/stringify.py` & `tox-4.6.3/src/tox/config/loader/stringify.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/config/loader/ini/__init__.py` & `tox-4.6.3/src/tox/config/loader/ini/__init__.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/config/loader/ini/factor.py` & `tox-4.6.3/src/tox/config/loader/ini/factor.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/config/loader/ini/replace.py` & `tox-4.6.3/src/tox/config/loader/ini/replace.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/config/source/api.py` & `tox-4.6.3/src/tox/config/source/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/config/source/discover.py` & `tox-4.6.3/src/tox/config/source/discover.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/config/source/ini.py` & `tox-4.6.3/src/tox/config/source/ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/config/source/ini_section.py` & `tox-4.6.3/src/tox/config/source/ini_section.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/config/source/legacy_toml.py` & `tox-4.6.3/src/tox/config/source/legacy_toml.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/config/source/setup_cfg.py` & `tox-4.6.3/src/tox/config/source/setup_cfg.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/execute/api.py` & `tox-4.6.3/src/tox/execute/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/execute/pep517_backend.py` & `tox-4.6.3/src/tox/execute/pep517_backend.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/execute/request.py` & `tox-4.6.3/src/tox/execute/request.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/execute/stream.py` & `tox-4.6.3/src/tox/execute/stream.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/execute/util.py` & `tox-4.6.3/src/tox/execute/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/execute/local_sub_process/__init__.py` & `tox-4.6.3/src/tox/execute/local_sub_process/__init__.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/execute/local_sub_process/read_via_thread.py` & `tox-4.6.3/src/tox/execute/local_sub_process/read_via_thread.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/execute/local_sub_process/read_via_thread_unix.py` & `tox-4.6.3/src/tox/execute/local_sub_process/read_via_thread_unix.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/execute/local_sub_process/read_via_thread_windows.py` & `tox-4.6.3/src/tox/execute/local_sub_process/read_via_thread_windows.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/journal/env.py` & `tox-4.6.3/src/tox/journal/env.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/journal/main.py` & `tox-4.6.3/src/tox/journal/main.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/plugin/__init__.py` & `tox-4.6.3/src/tox/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/plugin/inline.py` & `tox-4.6.3/src/tox/plugin/inline.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/plugin/manager.py` & `tox-4.6.3/src/tox/plugin/manager.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/plugin/spec.py` & `tox-4.6.3/src/tox/plugin/spec.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/session/env_select.py` & `tox-4.6.3/src/tox/session/env_select.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/session/state.py` & `tox-4.6.3/src/tox/session/state.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/session/cmd/depends.py` & `tox-4.6.3/src/tox/session/cmd/depends.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/session/cmd/devenv.py` & `tox-4.6.3/src/tox/session/cmd/devenv.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/session/cmd/exec_.py` & `tox-4.6.3/src/tox/session/cmd/exec_.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/session/cmd/legacy.py` & `tox-4.6.3/src/tox/session/cmd/legacy.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/session/cmd/list_env.py` & `tox-4.6.3/src/tox/session/cmd/list_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/session/cmd/quickstart.py` & `tox-4.6.3/src/tox/session/cmd/quickstart.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/session/cmd/show_config.py` & `tox-4.6.3/src/tox/session/cmd/show_config.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/session/cmd/version_flag.py` & `tox-4.6.3/src/tox/session/cmd/version_flag.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/session/cmd/run/common.py` & `tox-4.6.3/src/tox/session/cmd/run/common.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/session/cmd/run/parallel.py` & `tox-4.6.3/src/tox/session/cmd/run/parallel.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/session/cmd/run/sequential.py` & `tox-4.6.3/src/tox/session/cmd/run/sequential.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/session/cmd/run/single.py` & `tox-4.6.3/src/tox/session/cmd/run/single.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/tox_env/api.py` & `tox-4.6.3/src/tox/tox_env/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/tox_env/info.py` & `tox-4.6.3/src/tox/tox_env/info.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/tox_env/installer.py` & `tox-4.6.3/src/tox/tox_env/installer.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/tox_env/package.py` & `tox-4.6.3/src/tox/tox_env/package.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/tox_env/register.py` & `tox-4.6.3/src/tox/tox_env/register.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/tox_env/runner.py` & `tox-4.6.3/src/tox/tox_env/runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/tox_env/util.py` & `tox-4.6.3/src/tox/tox_env/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/tox_env/python/api.py` & `tox-4.6.3/src/tox/tox_env/python/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/tox_env/python/package.py` & `tox-4.6.3/src/tox/tox_env/python/package.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/tox_env/python/runner.py` & `tox-4.6.3/src/tox/tox_env/python/runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/tox_env/python/pip/pip_install.py` & `tox-4.6.3/src/tox/tox_env/python/pip/pip_install.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/tox_env/python/pip/req_file.py` & `tox-4.6.3/src/tox/tox_env/python/pip/req_file.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/tox_env/python/pip/req/args.py` & `tox-4.6.3/src/tox/tox_env/python/pip/req/args.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/tox_env/python/pip/req/file.py` & `tox-4.6.3/src/tox/tox_env/python/pip/req/file.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/tox_env/python/pip/req/util.py` & `tox-4.6.3/src/tox/tox_env/python/pip/req/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/tox_env/python/virtual_env/api.py` & `tox-4.6.3/src/tox/tox_env/python/virtual_env/api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/tox_env/python/virtual_env/runner.py` & `tox-4.6.3/src/tox/tox_env/python/virtual_env/runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/tox_env/python/virtual_env/package/cmd_builder.py` & `tox-4.6.3/src/tox/tox_env/python/virtual_env/package/cmd_builder.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/tox_env/python/virtual_env/package/pyproject.py` & `tox-4.6.3/src/tox/tox_env/python/virtual_env/package/pyproject.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import logging
 import os
 import sys
 from collections import defaultdict
 from contextlib import contextmanager
+from itertools import chain
 from pathlib import Path
 from threading import RLock
 from typing import TYPE_CHECKING, Any, Dict, Generator, Iterator, NoReturn, Optional, Sequence, cast
 
 from cachetools import cached
 from packaging.requirements import Requirement
 from pyproject_api import BackendFailed, CmdStatus, Frontend
@@ -93,14 +94,15 @@
 class Pep517VirtualEnvPackager(PythonPackageToxEnv, VirtualEnv):
     """local file system python virtual environment via the virtualenv package."""
 
     def __init__(self, create_args: ToxEnvCreateArgs) -> None:
         super().__init__(create_args)
         self._frontend_: Pep517VirtualEnvFrontend | None = None
         self.builds: defaultdict[str, list[EnvConfigSet]] = defaultdict(list)
+        self.call_require_hooks: set[str] = set()
         self._distribution_meta: PathDistribution | None = None
         self._package_dependencies: list[Requirement] | None = None
         self._package_name: str | None = None
         self._pkg_lock = RLock()  # can build only one package at a time
         self.root = self.conf["package_root"]
         self._package_paths: set[Path] = set()
 
@@ -146,29 +148,31 @@
         if meta_folder.exists() and tuple(meta_folder.iterdir()):
             return meta_folder
         return None
 
     def register_run_env(self, run_env: RunToxEnv) -> Generator[tuple[str, str], PackageToxEnv, None]:
         yield from super().register_run_env(run_env)
         build_type = run_env.conf["package"]
+        self.call_require_hooks.add(build_type)
         self.builds[build_type].append(run_env.conf)
 
     def _setup_env(self) -> None:
         super()._setup_env()
-        if "editable" in self.builds:
+        if "sdist" in self.call_require_hooks or "external" in self.call_require_hooks:
+            self._setup_build_requires("sdist")
+        if "wheel" in self.call_require_hooks:
+            self._setup_build_requires("wheel")
+        if "editable" in self.call_require_hooks:
             if not self._frontend.optional_hooks["build_editable"]:
                 raise BuildEditableNotSupportedError
-            build_requires = self._frontend.get_requires_for_build_editable().requires
-            self._install(build_requires, PythonPackageToxEnv.__name__, "requires_for_build_editable")
-        if "wheel" in self.builds:
-            build_requires = self._frontend.get_requires_for_build_wheel().requires
-            self._install(build_requires, PythonPackageToxEnv.__name__, "requires_for_build_wheel")
-        if "sdist" in self.builds or "external" in self.builds:
-            build_requires = self._frontend.get_requires_for_build_sdist().requires
-            self._install(build_requires, PythonPackageToxEnv.__name__, "requires_for_build_sdist")
+            self._setup_build_requires("editable")
+
+    def _setup_build_requires(self, of_type: str) -> None:
+        requires = getattr(self._frontend, f"get_requires_for_build_{of_type}")().requires
+        self._install(requires, PythonPackageToxEnv.__name__, f"requires_for_build_{of_type}")
 
     def _teardown(self) -> None:
         executor = self._frontend.backend_executor
         if executor is not None:  # pragma: no branch
             try:
                 if executor.is_alive:
                     self._frontend._send("_exit")  # try first on amicable shutdown  # noqa: SLF001
@@ -183,26 +187,28 @@
         super()._teardown()
 
     def perform_packaging(self, for_env: EnvConfigSet) -> list[Package]:
         """Build the package to install."""
         try:
             deps = self._load_deps(for_env)
         except BuildEditableNotSupportedError:
+            self.call_require_hooks.remove("editable")
             targets = [e for e in self.builds.pop("editable") if e["package"] == "editable"]
             names = ", ".join(sorted({t.env_name for t in targets if t.env_name}))
 
             logging.error(  # noqa: TRY400
                 "package config for %s is editable, however the build backend %s does not support PEP-660, falling "
                 "back to editable-legacy - change your configuration to it",
                 names,
                 cast(Pep517VirtualEnvFrontend, self._frontend_).backend,
             )
             for env in targets:
                 env._defined["package"].value = "editable-legacy"  # type: ignore[attr-defined]  # noqa: SLF001
                 self.builds["editable-legacy"].append(env)
+            self._run_state["setup"] = False  # force setup again as we need to provision wheel to get dependencies
             deps = self._load_deps(for_env)
         of_type: str = for_env["package"]
         if of_type == "editable-legacy":
             self.setup()
             deps = [*self.requires(), *self._frontend.get_requires_for_build_sdist().requires, *deps]
             package: Package = EditableLegacyPackage(self.core["tox_root"], deps)  # the folder itself is the package
         elif of_type == "sdist":
@@ -305,20 +311,21 @@
                 self._ensure_meta_present(for_env)
                 self._package_name = cast(PathDistribution, self._distribution_meta).metadata["Name"]
         return self._package_name
 
     def _ensure_meta_present(self, for_env: EnvConfigSet) -> None:
         if self._distribution_meta is not None:  # pragma: no branch
             return  # pragma: no cover
+        # even if we don't build a wheel we need the requirements for it should we want to build its metadata
+        target = "editable" if for_env["package"] == "editable" else "wheel"
+        self.call_require_hooks.add(target)
+
         self.setup()
-        end = self._frontend
-        if for_env["package"] == "editable":
-            dist_info = end.prepare_metadata_for_build_editable(self.meta_folder, self._wheel_config_settings).metadata
-        else:
-            dist_info = end.prepare_metadata_for_build_wheel(self.meta_folder, self._wheel_config_settings).metadata
+        hook = getattr(self._frontend, f"prepare_metadata_for_build_{target}")
+        dist_info = hook(self.meta_folder, self._wheel_config_settings).metadata
         self._distribution_meta = Distribution.at(str(dist_info))
 
     @property
     def _wheel_config_settings(self) -> ConfigSettings | None:
         return {"--build-option": []}
 
     def requires(self) -> tuple[Requirement, ...]:
@@ -328,20 +335,24 @@
 class Pep517VirtualEnvFrontend(Frontend):
     def __init__(self, root: Path, env: Pep517VirtualEnvPackager) -> None:
         super().__init__(*Frontend.create_args_from_folder(root))
         self._tox_env = env
         self._backend_executor_: LocalSubProcessPep517Executor | None = None
         into: dict[str, Any] = {}
 
-        for build_type in ("editable", "sdist", "wheel"):  # wrap build methods in a cache wrapper
+        for hook in chain(
+            (f"get_requires_for_build_{build_type}" for build_type in ["editable", "wheel", "sdist"]),
+            (f"prepare_metadata_for_build_{build_type}" for build_type in ["editable", "wheel"]),
+            (f"build_{build_type}" for build_type in ["editable", "wheel", "sdist"]),
+        ):  # wrap build methods in a cache wrapper
 
-            def key(*args: Any, bound_return: str = build_type, **kwargs: Any) -> str:  # noqa: ARG001
+            def key(*args: Any, bound_return: str = hook, **kwargs: Any) -> str:  # noqa: ARG001
                 return bound_return
 
-            setattr(self, f"build_{build_type}", cached(into, key=key)(getattr(self, f"build_{build_type}")))
+            setattr(self, hook, cached(into, key=key)(getattr(self, hook)))
 
     @property
     def backend_cmd(self) -> Sequence[str]:
         return ["python", *self.backend_args]
 
     def _send(self, cmd: str, **kwargs: Any) -> tuple[Any, str, str]:
         try:
```

### Comparing `tox-4.6.2/src/tox/tox_env/python/virtual_env/package/util.py` & `tox-4.6.3/src/tox/tox_env/python/virtual_env/package/util.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/util/ci.py` & `tox-4.6.3/src/tox/util/ci.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/util/file_view.py` & `tox-4.6.3/src/tox/util/file_view.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/util/graph.py` & `tox-4.6.3/src/tox/util/graph.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/util/path.py` & `tox-4.6.3/src/tox/util/path.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/src/tox/util/spinner.py` & `tox-4.6.3/src/tox/util/spinner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/conftest.py` & `tox-4.6.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/test_provision.py` & `tox-4.6.3/tests/test_provision.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/test_report.py` & `tox-4.6.3/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/test_run.py` & `tox-4.6.3/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/test_version.py` & `tox-4.6.3/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/test_main.py` & `tox-4.6.3/tests/config/test_main.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/test_of_types.py` & `tox-4.6.3/tests/config/test_of_types.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/test_set_env.py` & `tox-4.6.3/tests/config/test_set_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/test_sets.py` & `tox-4.6.3/tests/config/test_sets.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/test_types.py` & `tox-4.6.3/tests/config/test_types.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/cli/conftest.py` & `tox-4.6.3/tests/config/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/cli/test_cli_env_var.py` & `tox-4.6.3/tests/config/cli/test_cli_env_var.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/cli/test_cli_ini.py` & `tox-4.6.3/tests/config/cli/test_cli_ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/cli/test_parse.py` & `tox-4.6.3/tests/config/cli/test_parse.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/cli/test_parser.py` & `tox-4.6.3/tests/config/cli/test_parser.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/loader/test_loader.py` & `tox-4.6.3/tests/config/loader/test_loader.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/loader/test_memory_loader.py` & `tox-4.6.3/tests/config/loader/test_memory_loader.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/loader/test_section.py` & `tox-4.6.3/tests/config/loader/test_section.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/loader/test_str_convert.py` & `tox-4.6.3/tests/config/loader/test_str_convert.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/loader/ini/conftest.py` & `tox-4.6.3/tests/config/loader/ini/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/loader/ini/test_factor.py` & `tox-4.6.3/tests/config/loader/ini/test_factor.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/loader/ini/test_ini_loader.py` & `tox-4.6.3/tests/config/loader/ini/test_ini_loader.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/loader/ini/replace/conftest.py` & `tox-4.6.3/tests/config/loader/ini/replace/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/loader/ini/replace/test_replace.py` & `tox-4.6.3/tests/config/loader/ini/replace/test_replace.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/loader/ini/replace/test_replace_env_var.py` & `tox-4.6.3/tests/config/loader/ini/replace/test_replace_env_var.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/loader/ini/replace/test_replace_os_sep.py` & `tox-4.6.3/tests/config/loader/ini/replace/test_replace_os_sep.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/loader/ini/replace/test_replace_posargs.py` & `tox-4.6.3/tests/config/loader/ini/replace/test_replace_posargs.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/loader/ini/replace/test_replace_tox_env.py` & `tox-4.6.3/tests/config/loader/ini/replace/test_replace_tox_env.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/loader/ini/replace/test_replace_tty.py` & `tox-4.6.3/tests/config/loader/ini/replace/test_replace_tty.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/source/test_discover.py` & `tox-4.6.3/tests/config/source/test_discover.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/source/test_setup_cfg.py` & `tox-4.6.3/tests/config/source/test_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/config/source/test_source_ini.py` & `tox-4.6.3/tests/config/source/test_source_ini.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/demo_pkg_inline/build.py` & `tox-4.6.3/tests/demo_pkg_inline/build.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/execute/test_request.py` & `tox-4.6.3/tests/execute/test_request.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/execute/local_subprocess/bad_process.py` & `tox-4.6.3/tests/execute/local_subprocess/bad_process.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/execute/local_subprocess/local_subprocess_sigint.py` & `tox-4.6.3/tests/execute/local_subprocess/local_subprocess_sigint.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/execute/local_subprocess/test_execute_util.py` & `tox-4.6.3/tests/execute/local_subprocess/test_execute_util.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/execute/local_subprocess/test_local_subprocess.py` & `tox-4.6.3/tests/execute/local_subprocess/test_local_subprocess.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/journal/test_main_journal.py` & `tox-4.6.3/tests/journal/test_main_journal.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/plugin/test_inline.py` & `tox-4.6.3/tests/plugin/test_inline.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/plugin/test_plugin.py` & `tox-4.6.3/tests/plugin/test_plugin.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/plugin/test_plugin_custom_config_set.py` & `tox-4.6.3/tests/plugin/test_plugin_custom_config_set.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/pytest_/test_init.py` & `tox-4.6.3/tests/pytest_/test_init.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/session/test_env_select.py` & `tox-4.6.3/tests/session/test_env_select.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/session/test_session_common.py` & `tox-4.6.3/tests/session/test_session_common.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/session/cmd/test_depends.py` & `tox-4.6.3/tests/session/cmd/test_depends.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/session/cmd/test_devenv.py` & `tox-4.6.3/tests/session/cmd/test_devenv.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/session/cmd/test_exec_.py` & `tox-4.6.3/tests/session/cmd/test_exec_.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/session/cmd/test_legacy.py` & `tox-4.6.3/tests/session/cmd/test_legacy.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/session/cmd/test_list_envs.py` & `tox-4.6.3/tests/session/cmd/test_list_envs.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/session/cmd/test_parallel.py` & `tox-4.6.3/tests/session/cmd/test_parallel.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/session/cmd/test_quickstart.py` & `tox-4.6.3/tests/session/cmd/test_quickstart.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/session/cmd/test_sequential.py` & `tox-4.6.3/tests/session/cmd/test_sequential.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/session/cmd/test_show_config.py` & `tox-4.6.3/tests/session/cmd/test_show_config.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/session/cmd/test_state.py` & `tox-4.6.3/tests/session/cmd/test_state.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/session/cmd/run/test_common.py` & `tox-4.6.3/tests/session/cmd/run/test_common.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/tox_env/test_api.py` & `tox-4.6.3/tests/tox_env/test_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/tox_env/test_register.py` & `tox-4.6.3/tests/tox_env/test_register.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/tox_env/test_tox_env_api.py` & `tox-4.6.3/tests/tox_env/test_tox_env_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/tox_env/test_tox_env_runner.py` & `tox-4.6.3/tests/tox_env/test_tox_env_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,13 +20,14 @@
     execute_calls = proj.patch_execute(lambda r: 0 if "install" in r.run_id else None)
     result = proj.run("r", "--sdistonly")
     result.assert_success()
 
     expected_calls = [
         (".pkg", "_optional_hooks"),
         (".pkg", "get_requires_for_build_sdist"),
+        (".pkg", "get_requires_for_build_wheel"),
         (".pkg", "build_wheel"),
         (".pkg", "build_sdist"),
         (".pkg", "_exit"),
     ]
     found_calls = [(i[0][0].conf.name, i[0][3].run_id) for i in execute_calls.call_args_list]
     assert found_calls == expected_calls
```

### Comparing `tox-4.6.2/tests/tox_env/python/test_python_api.py` & `tox-4.6.3/tests/tox_env/python/test_python_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/tox_env/python/test_python_runner.py` & `tox-4.6.3/tests/tox_env/python/test_python_runner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/tox_env/python/pip/test_pip_install.py` & `tox-4.6.3/tests/tox_env/python/pip/test_pip_install.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/tox_env/python/pip/test_req_file.py` & `tox-4.6.3/tests/tox_env/python/pip/test_req_file.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/tox_env/python/pip/req/test_file.py` & `tox-4.6.3/tests/tox_env/python/pip/req/test_file.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/tox_env/python/virtual_env/test_setuptools.py` & `tox-4.6.3/tests/tox_env/python/virtual_env/test_setuptools.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/tox_env/python/virtual_env/test_virtualenv_api.py` & `tox-4.6.3/tests/tox_env/python/virtual_env/test_virtualenv_api.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/tox_env/python/virtual_env/package/conftest.py` & `tox-4.6.3/tests/tox_env/python/virtual_env/package/conftest.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py` & `tox-4.6.3/tests/tox_env/python/virtual_env/package/test_package_cmd_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,16 @@
     result.assert_success()
     calls = [(i[0][0].conf.name, i[0][3].run_id, i[0][3].cmd[5:]) for i in execute_calls.call_args_list]
     deps = ["black>=3", "colorama>=0.4.3", "flake8", "platformdirs>=2.1", "sphinx-rtd-theme<1,>=0.4.3", "sphinx>=3"]
     assert calls == [
         (".pkg_external_sdist_meta", "install_requires", ["setuptools", "wheel"]),
         (".pkg_external_sdist_meta", "_optional_hooks", []),
         (".pkg_external_sdist_meta", "get_requires_for_build_sdist", []),
+        (".pkg_external_sdist_meta", "get_requires_for_build_wheel", []),  # required before prepare_metadata*
+        (".pkg_external_sdist_meta", "install_requires_for_build_wheel", ["wheel"]),
         (".pkg_external_sdist_meta", "prepare_metadata_for_build_wheel", []),
         ("py", "install_package_deps", deps),
         ("py", "install_package", ["--force-reinstall", "--no-deps", str(pkg_with_extras_project_sdist)]),
         (".pkg_external_sdist_meta", "_exit", []),
     ]
```

### Comparing `tox-4.6.2/tests/tox_env/python/virtual_env/package/test_package_pyproject.py` & `tox-4.6.3/tests/tox_env/python/virtual_env/package/test_package_pyproject.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,14 +209,15 @@
     execute_calls = proj.patch_execute(lambda r: 0 if "install" in r.run_id else None)
     result = proj.run("r", "--notest")
     result.assert_success()
 
     expected_calls = [
         (".pkg", "_optional_hooks"),
         (".pkg", "get_requires_for_build_sdist"),
+        (".pkg", "get_requires_for_build_wheel"),
         (".pkg", "build_wheel"),
         (".pkg", "build_sdist"),
         ("py", "install_package_deps"),
         ("py", "install_package"),
         (".pkg", "_exit"),
     ]
     found_calls = [(i[0][0].conf.name, i[0][3].run_id) for i in execute_calls.call_args_list]
@@ -235,18 +236,18 @@
         ".pkg: package config for a, b is editable, however the build backend build does not support PEP-660, "
         "falling back to editable-legacy - change your configuration to it"
     )
     assert warning in result.out.splitlines()
 
     expected_calls = [
         (".pkg", "_optional_hooks"),
+        (".pkg", "get_requires_for_build_wheel"),
         (".pkg", "build_wheel"),
         (".pkg", "get_requires_for_build_sdist"),
         ("a", "install_package"),
-        (".pkg", "get_requires_for_build_sdist"),
         ("b", "install_package"),
         (".pkg", "_exit"),
     ]
     found_calls = [(i[0][0].conf.name, i[0][3].run_id) for i in execute_calls.call_args_list]
     assert found_calls == expected_calls
```

### Comparing `tox-4.6.2/tests/tox_env/python/virtual_env/package/test_python_package_util.py` & `tox-4.6.3/tests/tox_env/python/virtual_env/package/test_python_package_util.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/util/test_ci.py` & `tox-4.6.3/tests/util/test_ci.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/util/test_cpu.py` & `tox-4.6.3/tests/util/test_cpu.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/util/test_graph.py` & `tox-4.6.3/tests/util/test_graph.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/tests/util/test_spinner.py` & `tox-4.6.3/tests/util/test_spinner.py`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/LICENSE` & `tox-4.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/README.md` & `tox-4.6.3/README.md`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/pyproject.toml` & `tox-4.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tox-4.6.2/PKG-INFO` & `tox-4.6.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox
-Version: 4.6.2
+Version: 4.6.3
 Summary: tox is a generic virtualenv management and test command line tool
 Project-URL: Documentation, https://tox.wiki
 Project-URL: Homepage, http://tox.readthedocs.org
 Project-URL: Release Notes, https://tox.wiki/en/latest/changelog.html
 Project-URL: Source, https://github.com/tox-dev/tox
 Project-URL: Tracker, https://github.com/tox-dev/tox/issues
 Author-email: Bernát Gábor <gaborjbernat@gmail.com>
```

