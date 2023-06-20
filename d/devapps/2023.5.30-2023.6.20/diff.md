# Comparing `tmp/devapps-2023.5.30.tar.gz` & `tmp/devapps-2023.6.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devapps-2023.5.30.tar", max compression
+gzip compressed data, was "devapps-2023.6.20.tar", max compression
```

## Comparing `devapps-2023.5.30.tar` & `devapps-2023.6.20.tar`

### file list

```diff
@@ -1,145 +1,148 @@
--rw-r--r--   0        0        0     1323 2022-05-05 20:54:49.110883 devapps-2023.5.30/LICENSE
--rw-r--r--   0        0        0      992 2023-05-30 21:05:51.406637 devapps-2023.5.30/README.md
--rw-r--r--   0        0        0     5914 2023-05-30 21:05:36.291436 devapps-2023.5.30/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-22 14:30:25.715938 devapps-2023.5.30/src/ax/utils/__init__.py
--rw-r--r--   0        0        0       28 2023-03-22 14:30:25.715938 devapps-2023.5.30/src/ax/utils/ax_tree/__init__.py
--rwxr-xr-x   0        0        0    88440 2023-03-22 14:30:25.716939 devapps-2023.5.30/src/ax/utils/ax_tree/_ax_tree.so
--rw-r--r--   0        0        0    10033 2023-03-22 14:30:25.716939 devapps-2023.5.30/src/ax/utils/ax_tree/ax_tree.py
--rwxr-xr-x   0        0        0      491 2023-05-17 15:36:04.919861 devapps-2023.5.30/src/devapp/__init__.py
--rwxr-xr-x   0        0        0    19220 2023-05-17 15:36:04.919861 devapps-2023.5.30/src/devapp/app.py
--rwxr-xr-x   0        0        0        0 2023-05-17 15:36:04.919861 devapps-2023.5.30/src/devapp/app_token/__init__.py
--rwxr-xr-x   0        0        0     1201 2023-05-17 15:36:04.920861 devapps-2023.5.30/src/devapp/app_token/create_tokens.py
--rwxr-xr-x   0        0        0     2230 2023-05-17 15:36:04.920861 devapps-2023.5.30/src/devapp/app_token/read_tokens.py
--rwxr-xr-x   0        0        0      151 2023-05-17 15:36:04.921861 devapps-2023.5.30/src/devapp/app_token/verify_token
--rwxr-xr-x   0        0        0      297 2023-05-17 15:36:04.921861 devapps-2023.5.30/src/devapp/components/__init__.py
--rwxr-xr-x   0        0        0     6980 2023-05-17 15:36:04.921861 devapps-2023.5.30/src/devapp/components/cloudfoundry.py
--rwxr-xr-x   0        0        0     5956 2023-05-17 15:36:04.922861 devapps-2023.5.30/src/devapp/components/gitlab.py
--rwxr-xr-x   0        0        0     4828 2023-05-17 15:36:04.922861 devapps-2023.5.30/src/devapp/components/gitlab_runner.py
--rwxr-xr-x   0        0        0      150 2023-05-17 15:36:04.922861 devapps-2023.5.30/src/devapp/da.py
--rwxr-xr-x   0        0        0     1321 2023-05-17 15:36:04.922861 devapps-2023.5.30/src/devapp/dev_mode.py
--rwxr-xr-x   0        0        0     1636 2023-05-17 15:36:04.923861 devapps-2023.5.30/src/devapp/gevent_patched.py
--rwxr-xr-x   0        0        0     1549 2023-05-17 15:36:04.923861 devapps-2023.5.30/src/devapp/layer.py
--rwxr-xr-x   0        0        0      188 2023-05-17 15:36:04.923861 devapps-2023.5.30/src/devapp/lib/README.md
--rwxr-xr-x   0        0        0        0 2023-05-17 15:36:04.923861 devapps-2023.5.30/src/devapp/lib/__init__.py
--rwxr-xr-x   0        0        0   123141 2023-05-17 15:36:04.924861 devapps-2023.5.30/src/devapp/lib/sh.py
--rwxr-xr-x   0        0        0     2343 2023-05-17 15:36:04.925861 devapps-2023.5.30/src/devapp/load.py
--rwxr-xr-x   0        0        0      655 2023-05-17 15:36:04.925861 devapps-2023.5.30/src/devapp/logo
--rwxr-xr-x   0        0        0     1671 2023-05-17 15:36:04.925861 devapps-2023.5.30/src/devapp/max.py
--rw-r--r--   0        0        0     1933 2023-05-17 15:36:04.925861 devapps-2023.5.30/src/devapp/operations/resources.py
--rwxr-xr-x   0        0        0     1551 2023-05-17 15:36:04.926861 devapps-2023.5.30/src/devapp/plugins/dev_devapp/personal_development_sandbox/__init__.py
--rwxr-xr-x   0        0        0     6445 2023-05-17 15:36:04.926861 devapps-2023.5.30/src/devapp/plugins/dev_devapp/repo_sym_links.py
--rw-r--r--   0        0        0     3090 2023-05-17 15:36:04.926861 devapps-2023.5.30/src/devapp/plugins/ops_devapp/arch/resource_install.py
--rw-r--r--   0        0        0     4577 2023-05-17 15:36:04.926861 devapps-2023.5.30/src/devapp/plugins/ops_devapp/arch/resource_run.py
--rw-r--r--   0        0        0     8983 2023-05-17 15:36:04.927861 devapps-2023.5.30/src/devapp/plugins/ops_devapp/arch/resources.py.dis
--rw-r--r--   0        0        0      671 2023-05-17 15:36:04.927861 devapps-2023.5.30/src/devapp/plugins/ops_devapp/arch/resources_list.py
--rw-r--r--   0        0        0      879 2023-05-17 15:36:04.927861 devapps-2023.5.30/src/devapp/plugins/ops_devapp/arch/wait_for_port.py
--rwxr-xr-x   0        0        0     8688 2023-05-17 15:36:04.927861 devapps-2023.5.30/src/devapp/plugins/ops_devapp/container_build.py
--rwxr-xr-x   0        0        0    10257 2023-05-17 15:36:04.928861 devapps-2023.5.30/src/devapp/plugins/ops_devapp/container_pull.py
--rwxr-xr-x   0        0        0    28013 2023-05-17 15:36:04.928861 devapps-2023.5.30/src/devapp/plugins/ops_devapp/fs_build.py
--rwxr-xr-x   0        0        0    13318 2023-05-17 15:36:04.928861 devapps-2023.5.30/src/devapp/plugins/ops_devapp/infra_aws_cloud/__init__.py
--rwxr-xr-x   0        0        0     9232 2023-05-17 15:36:04.929861 devapps-2023.5.30/src/devapp/plugins/ops_devapp/infra_digital_ocean/__init__.py
--rwxr-xr-x   0        0        0    12668 2023-05-17 15:36:04.929861 devapps-2023.5.30/src/devapp/plugins/ops_devapp/infra_hetzner_cloud/__init__.py
--rwxr-xr-x   0        0        0     8750 2023-05-17 15:36:04.929861 devapps-2023.5.30/src/devapp/plugins/ops_devapp/kubectl/__init__.py
--rwxr-xr-x   0        0        0     2975 2023-05-17 15:36:04.930861 devapps-2023.5.30/src/devapp/plugins/ops_devapp/life_cycle.py
--rw-r--r--   0        0        0     1573 2023-05-17 15:36:04.930861 devapps-2023.5.30/src/devapp/plugins/ops_devapp/log_view.py
--rwxr-xr-x   0        0        0     2140 2023-05-18 08:36:34.543057 devapps-2023.5.30/src/devapp/plugins/ops_devapp/pkgs.py
--rwxr-xr-x   0        0        0    12954 2023-05-30 21:03:47.819991 devapps-2023.5.30/src/devapp/plugins/ops_devapp/project/__init__.py
--rw-r--r--   0        0        0     9960 2023-05-17 15:36:04.930861 devapps-2023.5.30/src/devapp/plugins/ops_devapp/project/devinstall/__init__.py
--rw-r--r--   0        0        0     4994 2023-05-17 15:36:04.931861 devapps-2023.5.30/src/devapp/plugins/ops_devapp/run.py
--rwxr-xr-x   0        0        0    28235 2023-05-17 15:36:04.931861 devapps-2023.5.30/src/devapp/run.py
--rwxr-xr-x   0        0        0    25984 2023-05-17 15:36:04.931861 devapps-2023.5.30/src/devapp/spec/build.py
--rwxr-xr-x   0        0        0     2929 2023-05-17 15:36:04.932861 devapps-2023.5.30/src/devapp/spec/find_paths_in_fs_components.py
--rwxr-xr-x   0        0        0    16176 2023-05-17 15:36:04.932861 devapps-2023.5.30/src/devapp/spec/fs_components.py
--rwxr-xr-x   0        0        0     1715 2023-05-17 15:36:04.933861 devapps-2023.5.30/src/devapp/spec/links.py
--rwxr-xr-x   0        0        0     2481 2023-05-17 15:36:04.933861 devapps-2023.5.30/src/devapp/spec/os_tools.py
--rwxr-xr-x   0        0        0     7913 2023-05-17 15:36:04.933861 devapps-2023.5.30/src/devapp/spec/templ.py
--rwxr-xr-x   0        0        0     1600 2023-05-17 15:36:04.933861 devapps-2023.5.30/src/devapp/spec/templates/unit
--rwxr-xr-x   0        0        0     7586 2023-05-17 15:36:04.934861 devapps-2023.5.30/src/devapp/spec/tools.py
--rwxr-xr-x   0        0        0    30671 2023-05-17 15:36:04.934861 devapps-2023.5.30/src/devapp/t
--rw-r--r--   0        0        0     3559 2023-05-17 15:36:04.934861 devapps-2023.5.30/src/devapp/testing/auto_docs.py
--rw-r--r--   0        0        0      443 2023-05-17 15:36:04.935861 devapps-2023.5.30/src/devapp/tests/test_unit_devapp.py
--rwxr-xr-x   0        0        0    13808 2023-05-17 15:36:04.935861 devapps-2023.5.30/src/devapp/third/rpl
--rwxr-xr-x   0        0        0    50010 2023-05-17 15:36:04.936861 devapps-2023.5.30/src/devapp/tools/__init__.py
--rw-r--r--   0        0        0     4025 2023-05-17 15:36:04.936861 devapps-2023.5.30/src/devapp/tools/flag.py
--rw-r--r--   0        0        0      731 2023-05-17 15:36:04.936861 devapps-2023.5.30/src/devapp/tools/http.py
--rw-r--r--   0        0        0    35701 2023-05-17 15:36:04.936861 devapps-2023.5.30/src/devapp/tools/infra/__init__.py
--rw-r--r--   0        0        0    16618 2023-05-17 15:36:04.937861 devapps-2023.5.30/src/devapp/tools/infra/actions.py
--rw-r--r--   0        0        0     3089 2023-05-17 15:36:04.937861 devapps-2023.5.30/src/devapp/tools/infra/playbooks/000:functions.sh
--rwxr-xr-x   0        0        0      375 2023-05-17 15:36:04.937861 devapps-2023.5.30/src/devapp/tools/infra/playbooks/001:add_sudo_user.sh
--rwxr-xr-x   0        0        0     1521 2023-05-17 15:36:04.938861 devapps-2023.5.30/src/devapp/tools/infra/playbooks/1000:k_hello_world1.sh
--rwxr-xr-x   0        0        0      448 2023-05-17 15:36:04.938861 devapps-2023.5.30/src/devapp/tools/infra/playbooks/100:docker.sh
--rwxr-xr-x   0        0        0      324 2023-05-17 15:36:04.938861 devapps-2023.5.30/src/devapp/tools/infra/playbooks/200:tools.sh
--rwxr-xr-x   0        0        0      760 2023-05-17 15:36:04.938861 devapps-2023.5.30/src/devapp/tools/infra/playbooks/300:dns.sh
--rwxr-xr-x   0        0        0     4375 2023-05-17 15:36:04.938861 devapps-2023.5.30/src/devapp/tools/infra/playbooks/500:k3s.sh
--rwxr-xr-x   0        0        0      943 2023-05-17 15:36:04.939861 devapps-2023.5.30/src/devapp/tools/infra/playbooks/501:kind.sh
--rwxr-xr-x   0        0        0    17210 2023-05-17 15:36:04.939861 devapps-2023.5.30/src/devapp/tools/infra/playbooks/502:k3s.sh
--rw-r--r--   0        0        0      276 2023-05-17 15:36:04.939861 devapps-2023.5.30/src/devapp/tools/infra/playbooks/510:label_workers.sh
--rwxr-xr-x   0        0        0      661 2023-05-17 15:36:04.940861 devapps-2023.5.30/src/devapp/tools/infra/playbooks/600:longhorn.sh
--rw-r--r--   0        0        0     1737 2023-05-17 15:36:04.941861 devapps-2023.5.30/src/devapp/tools/infra/playbooks/800:kube_hypermodern.sh
--rw-r--r--   0        0        0    26850 2023-05-17 15:36:04.942861 devapps-2023.5.30/src/devapp/tools/old.py
--rw-r--r--   0        0        0     4415 2023-05-17 15:36:04.942861 devapps-2023.5.30/src/devapp/tools/plugin.py
--rw-r--r--   0        0        0    27592 2023-05-30 20:16:25.156128 devapps-2023.5.30/src/devapp/tools/resource.py
--rw-r--r--   0        0        0     1861 2023-05-17 15:36:04.942861 devapps-2023.5.30/src/devapp/tools/times.py
--rwxr-xr-x   0        0        0        0 2023-05-17 15:36:04.943861 devapps-2023.5.30/src/devapp/utils/__init__.py
--rwxr-xr-x   0        0        0    15787 2023-05-17 15:36:04.943861 devapps-2023.5.30/src/devapp/utils/os_.py
--rwxr-xr-x   0        0        0     1871 2023-05-17 15:36:04.943861 devapps-2023.5.30/src/devapp/utils/py_source_env.py
--rwxr-xr-x   0        0        0     9335 2023-05-17 15:36:04.944861 devapps-2023.5.30/src/devapp/utils/rx_tools.py
--rwxr-xr-x   0        0        0    11529 2023-05-17 15:36:04.944861 devapps-2023.5.30/src/devapp/utils/vault.py
--rwxr-xr-x   0        0        0     2107 2023-05-17 15:36:04.944861 devapps-2023.5.30/src/devapp/utils/watch_dog.py
--rwxr-xr-x   0        0        0        0 2023-03-22 14:30:25.734938 devapps-2023.5.30/src/mdvl/__init__.py
--rwxr-xr-x   0        0        0    20402 2023-05-02 08:41:56.784342 devapps-2023.5.30/src/mdvl/mdvl.py
--rwxr-xr-x   0        0        0     2317 2023-03-22 14:30:25.735939 devapps-2023.5.30/src/mdvl/tools.py
--rwxr-xr-x   0        0        0      519 2023-05-17 15:36:04.945861 devapps-2023.5.30/src/structlogging/__init__.py
--rwxr-xr-x   0        0        0     1559 2023-05-17 15:36:04.945861 devapps-2023.5.30/src/structlogging/adapters.py
--rwxr-xr-x   0        0        0       88 2023-05-17 15:36:04.946861 devapps-2023.5.30/src/structlogging/common.py
--rwxr-xr-x   0        0        0     5503 2023-05-17 15:36:04.946861 devapps-2023.5.30/src/structlogging/config.py
--rwxr-xr-x   0        0        0     1618 2023-05-17 15:36:04.946861 devapps-2023.5.30/src/structlogging/formatters.py
--rwxr-xr-x   0        0        0     2640 2023-05-17 15:36:04.946861 devapps-2023.5.30/src/structlogging/processors.py
--rwxr-xr-x   0        0        0     5472 2023-05-17 15:36:04.946861 devapps-2023.5.30/src/structlogging/renderers.py
--rwxr-xr-x   0        0        0    11172 2023-05-17 15:36:04.947861 devapps-2023.5.30/src/structlogging/sl.py
--rw-r--r--   0        0        0     4022 2023-05-17 15:36:04.947861 devapps-2023.5.30/src/structlogging/stacktrace.py
--rwxr-xr-x   0        0        0     1355 2023-05-17 15:36:04.947861 devapps-2023.5.30/src/structlogging/tests/test_structlogging.py
--rwxr-xr-x   0        0        0      886 2023-05-02 12:47:20.254964 devapps-2023.5.30/src/theming/__init__.py
--rwxr-xr-x   0        0        0    14865 2023-05-02 12:47:20.254964 devapps-2023.5.30/src/theming/absl_color_help.py
--rwxr-xr-x   0        0        0     4345 2023-05-02 12:47:20.255964 devapps-2023.5.30/src/theming/ansi2html.py
--rwxr-xr-x   0        0        0    11888 2023-05-02 12:47:20.255964 devapps-2023.5.30/src/theming/ansi2html.sh
--rwxr-xr-x   0        0        0     3030 2023-05-02 12:47:20.255964 devapps-2023.5.30/src/theming/ansistrm.py
--rwxr-xr-x   0        0        0    10066 2023-05-02 12:47:20.255964 devapps-2023.5.30/src/theming/ax_xml.py
--rwxr-xr-x   0        0        0    10495 2023-05-02 12:47:20.255964 devapps-2023.5.30/src/theming/camel_snake.py
--rwxr-xr-x   0        0        0     7517 2023-05-02 12:47:20.256964 devapps-2023.5.30/src/theming/charting.py
--rwxr-xr-x   0        0        0     3392 2023-05-02 12:47:20.256964 devapps-2023.5.30/src/theming/colorhilite.py
--rwxr-xr-x   0        0        0     1113 2023-05-02 12:47:20.256964 devapps-2023.5.30/src/theming/filesize/README.txt
--rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.256964 devapps-2023.5.30/src/theming/filesize/__init__.py
--rwxr-xr-x   0        0        0     2549 2023-05-02 12:47:20.256964 devapps-2023.5.30/src/theming/filesize/filesize.py
--rwxr-xr-x   0        0        0     3756 2023-05-02 12:47:20.257964 devapps-2023.5.30/src/theming/formatters.py
--rw-r--r--   0        0        0     3807 2023-05-02 12:47:20.257964 devapps-2023.5.30/src/theming/formatting/markdown.py
--rw-r--r--   0        0        0     1241 2023-05-02 12:47:20.257964 devapps-2023.5.30/src/theming/formatting/viz_sequence.py
--rwxr-xr-x   0        0        0     3410 2023-05-02 12:47:20.257964 devapps-2023.5.30/src/theming/html_tools.py
--rwxr-xr-x   0        0        0    11409 2023-05-02 12:47:20.257964 devapps-2023.5.30/src/theming/inflect.py
--rwxr-xr-x   0        0        0      460 2023-05-02 12:47:20.258964 devapps-2023.5.30/src/theming/msgs.py
--rwxr-xr-x   0        0        0     9864 2023-05-02 12:47:20.258964 devapps-2023.5.30/src/theming/pretty_print.py
--rwxr-xr-x   0        0        0    55699 2023-05-02 12:47:20.258964 devapps-2023.5.30/src/theming/tablepretty.py
--rwxr-xr-x   0        0        0    13998 2023-05-02 12:47:20.259964 devapps-2023.5.30/src/theming/term.py
--rwxr-xr-x   0        0        0     1468 2023-05-02 12:47:20.259964 devapps-2023.5.30/src/theming/term_struct_hilite.py
--rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.259964 devapps-2023.5.30/src/theming/test
--rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.259964 devapps-2023.5.30/src/theming/tests/__init__.py
--rwxr-xr-x   0        0        0     9454 2023-05-02 12:47:20.260964 devapps-2023.5.30/src/theming/tests/test_text_formatting.py
--rwxr-xr-x   0        0        0     1063 2023-05-02 12:47:20.260964 devapps-2023.5.30/src/theming/tracebacks.py
--rwxr-xr-x   0        0        0     3011 2023-05-02 12:47:20.260964 devapps-2023.5.30/src/theming/unicode_chars.py
--rwxr-xr-x   0        0        0    23138 2023-03-23 18:50:41.169018 devapps-2023.5.30/src/tree_builder/__init__.py
--rwxr-xr-x   0        0        0    19864 2023-03-23 18:50:41.169018 devapps-2023.5.30/src/tree_builder/arch/__init__.py.bak
--rwxr-xr-x   0        0        0     7762 2023-03-23 18:50:41.169018 devapps-2023.5.30/src/tree_builder/arch/links.py.bak
--rwxr-xr-x   0        0        0    11455 2023-03-23 18:50:41.169018 devapps-2023.5.30/src/tree_builder/arch/o.py
--rwxr-xr-x   0        0        0    19872 2023-03-23 18:50:41.170018 devapps-2023.5.30/src/tree_builder/arch/old
--rwxr-xr-x   0        0        0    10911 2023-03-23 18:50:41.170018 devapps-2023.5.30/src/tree_builder/arch/olinit
--rwxr-xr-x   0        0        0    11597 2023-03-23 18:50:41.170018 devapps-2023.5.30/src/tree_builder/arch/oo
--rwxr-xr-x   0        0        0      154 2023-03-23 18:50:41.170018 devapps-2023.5.30/src/tree_builder/arch/py2.py
--rwxr-xr-x   0        0        0     7968 2023-03-23 18:50:41.170018 devapps-2023.5.30/src/tree_builder/arch/render.py.bak
--rwxr-xr-x   0        0        0     2078 2023-03-23 18:50:41.170018 devapps-2023.5.30/src/tree_builder/chrome_reload.sh
--rwxr-xr-x   0        0        0     5502 2023-03-23 18:50:41.170018 devapps-2023.5.30/src/tree_builder/delivery2.py
--rwxr-xr-x   0        0        0    10773 2023-03-23 18:50:41.171018 devapps-2023.5.30/src/tree_builder/links.py
--rwxr-xr-x   0        0        0      218 2023-03-23 18:50:41.171018 devapps-2023.5.30/src/tree_builder/py3.py
--rwxr-xr-x   0        0        0     8028 2023-03-23 18:50:41.171018 devapps-2023.5.30/src/tree_builder/render.py
--rwxr-xr-x   0        0        0       21 2023-03-23 18:50:41.171018 devapps-2023.5.30/src/tree_builder/version.py
--rw-r--r--   0        0        0     3038 2023-05-30 21:05:54.041867 devapps-2023.5.30/setup.py
--rw-r--r--   0        0        0     1805 2023-05-30 21:05:54.042127 devapps-2023.5.30/PKG-INFO
+-rw-r--r--   0        0        0     1323 2022-05-05 20:54:49.110883 devapps-2023.6.20/LICENSE
+-rw-r--r--   0        0        0      992 2023-06-20 14:21:54.336663 devapps-2023.6.20/README.md
+-rw-r--r--   0        0        0     5914 2023-06-20 14:21:38.025659 devapps-2023.6.20/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-22 14:30:25.715938 devapps-2023.6.20/src/ax/utils/__init__.py
+-rw-r--r--   0        0        0       28 2023-03-22 14:30:25.715938 devapps-2023.6.20/src/ax/utils/ax_tree/__init__.py
+-rwxr-xr-x   0        0        0    88440 2023-03-22 14:30:25.716939 devapps-2023.6.20/src/ax/utils/ax_tree/_ax_tree.so
+-rw-r--r--   0        0        0    10033 2023-03-22 14:30:25.716939 devapps-2023.6.20/src/ax/utils/ax_tree/ax_tree.py
+-rwxr-xr-x   0        0        0      491 2023-05-17 15:36:04.919861 devapps-2023.6.20/src/devapp/__init__.py
+-rwxr-xr-x   0        0        0    19220 2023-05-17 15:36:04.919861 devapps-2023.6.20/src/devapp/app.py
+-rwxr-xr-x   0        0        0        0 2023-05-17 15:36:04.919861 devapps-2023.6.20/src/devapp/app_token/__init__.py
+-rwxr-xr-x   0        0        0     1201 2023-05-17 15:36:04.920861 devapps-2023.6.20/src/devapp/app_token/create_tokens.py
+-rwxr-xr-x   0        0        0     2230 2023-05-17 15:36:04.920861 devapps-2023.6.20/src/devapp/app_token/read_tokens.py
+-rwxr-xr-x   0        0        0      151 2023-05-17 15:36:04.921861 devapps-2023.6.20/src/devapp/app_token/verify_token
+-rwxr-xr-x   0        0        0      297 2023-05-17 15:36:04.921861 devapps-2023.6.20/src/devapp/components/__init__.py
+-rwxr-xr-x   0        0        0     6980 2023-05-17 15:36:04.921861 devapps-2023.6.20/src/devapp/components/cloudfoundry.py
+-rwxr-xr-x   0        0        0     5956 2023-05-17 15:36:04.922861 devapps-2023.6.20/src/devapp/components/gitlab.py
+-rwxr-xr-x   0        0        0     4828 2023-05-17 15:36:04.922861 devapps-2023.6.20/src/devapp/components/gitlab_runner.py
+-rwxr-xr-x   0        0        0      150 2023-05-17 15:36:04.922861 devapps-2023.6.20/src/devapp/da.py
+-rwxr-xr-x   0        0        0     1321 2023-05-17 15:36:04.922861 devapps-2023.6.20/src/devapp/dev_mode.py
+-rwxr-xr-x   0        0        0     1636 2023-05-17 15:36:04.923861 devapps-2023.6.20/src/devapp/gevent_patched.py
+-rwxr-xr-x   0        0        0     1549 2023-05-17 15:36:04.923861 devapps-2023.6.20/src/devapp/layer.py
+-rwxr-xr-x   0        0        0      188 2023-05-17 15:36:04.923861 devapps-2023.6.20/src/devapp/lib/README.md
+-rwxr-xr-x   0        0        0        0 2023-05-17 15:36:04.923861 devapps-2023.6.20/src/devapp/lib/__init__.py
+-rwxr-xr-x   0        0        0   123141 2023-05-17 15:36:04.924861 devapps-2023.6.20/src/devapp/lib/sh.py
+-rwxr-xr-x   0        0        0     2343 2023-05-17 15:36:04.925861 devapps-2023.6.20/src/devapp/load.py
+-rwxr-xr-x   0        0        0      655 2023-05-17 15:36:04.925861 devapps-2023.6.20/src/devapp/logo
+-rwxr-xr-x   0        0        0     1671 2023-05-17 15:36:04.925861 devapps-2023.6.20/src/devapp/max.py
+-rw-r--r--   0        0        0     1933 2023-05-17 15:36:04.925861 devapps-2023.6.20/src/devapp/operations/resources.py
+-rwxr-xr-x   0        0        0     1551 2023-05-17 15:36:04.926861 devapps-2023.6.20/src/devapp/plugins/dev_devapp/personal_development_sandbox/__init__.py
+-rwxr-xr-x   0        0        0     6445 2023-05-17 15:36:04.926861 devapps-2023.6.20/src/devapp/plugins/dev_devapp/repo_sym_links.py
+-rw-r--r--   0        0        0     3090 2023-05-17 15:36:04.926861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/arch/resource_install.py
+-rw-r--r--   0        0        0     4577 2023-05-17 15:36:04.926861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/arch/resource_run.py
+-rw-r--r--   0        0        0     8983 2023-05-17 15:36:04.927861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/arch/resources.py.dis
+-rw-r--r--   0        0        0      671 2023-05-17 15:36:04.927861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/arch/resources_list.py
+-rw-r--r--   0        0        0      879 2023-05-17 15:36:04.927861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/arch/wait_for_port.py
+-rwxr-xr-x   0        0        0     8688 2023-05-17 15:36:04.927861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/container_build.py
+-rwxr-xr-x   0        0        0    10257 2023-05-17 15:36:04.928861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/container_pull.py
+-rwxr-xr-x   0        0        0    28013 2023-05-17 15:36:04.928861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/fs_build.py
+-rwxr-xr-x   0        0        0    13318 2023-05-17 15:36:04.928861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/infra_aws_cloud/__init__.py
+-rwxr-xr-x   0        0        0     9232 2023-05-17 15:36:04.929861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/infra_digital_ocean/__init__.py
+-rwxr-xr-x   0        0        0    12668 2023-05-17 15:36:04.929861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/infra_hetzner_cloud/__init__.py
+-rwxr-xr-x   0        0        0     8750 2023-05-17 15:36:04.929861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/kubectl/__init__.py
+-rwxr-xr-x   0        0        0     2975 2023-05-17 15:36:04.930861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/life_cycle.py
+-rw-r--r--   0        0        0     1573 2023-05-17 15:36:04.930861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/log_view.py
+-rwxr-xr-x   0        0        0     2140 2023-05-18 08:36:34.543057 devapps-2023.6.20/src/devapp/plugins/ops_devapp/pkgs.py
+-rwxr-xr-x   0        0        0    12996 2023-05-31 11:31:49.834517 devapps-2023.6.20/src/devapp/plugins/ops_devapp/project/__init__.py
+-rw-r--r--   0        0        0     9960 2023-05-17 15:36:04.930861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/project/devinstall/__init__.py
+-rw-r--r--   0        0        0     4994 2023-05-17 15:36:04.931861 devapps-2023.6.20/src/devapp/plugins/ops_devapp/run.py
+-rwxr-xr-x   0        0        0     7865 2023-06-16 15:07:07.410741 devapps-2023.6.20/src/devapp/plugins/ops_devapp/system/__init__.py
+-rw-r--r--   0        0        0     2649 2023-06-16 16:56:09.507836 devapps-2023.6.20/src/devapp/plugins/ops_devapp/system/templates/inst_base.sh
+-rw-r--r--   0        0        0     2657 2023-06-16 16:00:30.337863 devapps-2023.6.20/src/devapp/plugins/ops_devapp/system/tools.py
+-rwxr-xr-x   0        0        0    28235 2023-05-17 15:36:04.931861 devapps-2023.6.20/src/devapp/run.py
+-rwxr-xr-x   0        0        0    25984 2023-05-17 15:36:04.931861 devapps-2023.6.20/src/devapp/spec/build.py
+-rwxr-xr-x   0        0        0     2929 2023-05-17 15:36:04.932861 devapps-2023.6.20/src/devapp/spec/find_paths_in_fs_components.py
+-rwxr-xr-x   0        0        0    16176 2023-05-17 15:36:04.932861 devapps-2023.6.20/src/devapp/spec/fs_components.py
+-rwxr-xr-x   0        0        0     1715 2023-05-17 15:36:04.933861 devapps-2023.6.20/src/devapp/spec/links.py
+-rwxr-xr-x   0        0        0     2481 2023-05-17 15:36:04.933861 devapps-2023.6.20/src/devapp/spec/os_tools.py
+-rwxr-xr-x   0        0        0     7913 2023-05-17 15:36:04.933861 devapps-2023.6.20/src/devapp/spec/templ.py
+-rwxr-xr-x   0        0        0     1600 2023-05-17 15:36:04.933861 devapps-2023.6.20/src/devapp/spec/templates/unit
+-rwxr-xr-x   0        0        0     7586 2023-05-17 15:36:04.934861 devapps-2023.6.20/src/devapp/spec/tools.py
+-rwxr-xr-x   0        0        0    30671 2023-05-17 15:36:04.934861 devapps-2023.6.20/src/devapp/t
+-rw-r--r--   0        0        0     3559 2023-05-17 15:36:04.934861 devapps-2023.6.20/src/devapp/testing/auto_docs.py
+-rw-r--r--   0        0        0      443 2023-05-17 15:36:04.935861 devapps-2023.6.20/src/devapp/tests/test_unit_devapp.py
+-rwxr-xr-x   0        0        0    13808 2023-05-17 15:36:04.935861 devapps-2023.6.20/src/devapp/third/rpl
+-rwxr-xr-x   0        0        0    50126 2023-06-16 15:44:29.254501 devapps-2023.6.20/src/devapp/tools/__init__.py
+-rw-r--r--   0        0        0     4025 2023-05-17 15:36:04.936861 devapps-2023.6.20/src/devapp/tools/flag.py
+-rw-r--r--   0        0        0      731 2023-05-17 15:36:04.936861 devapps-2023.6.20/src/devapp/tools/http.py
+-rw-r--r--   0        0        0    35701 2023-05-17 15:36:04.936861 devapps-2023.6.20/src/devapp/tools/infra/__init__.py
+-rw-r--r--   0        0        0    16618 2023-05-17 15:36:04.937861 devapps-2023.6.20/src/devapp/tools/infra/actions.py
+-rw-r--r--   0        0        0     3089 2023-05-17 15:36:04.937861 devapps-2023.6.20/src/devapp/tools/infra/playbooks/000:functions.sh
+-rwxr-xr-x   0        0        0      375 2023-05-17 15:36:04.937861 devapps-2023.6.20/src/devapp/tools/infra/playbooks/001:add_sudo_user.sh
+-rwxr-xr-x   0        0        0     1521 2023-05-17 15:36:04.938861 devapps-2023.6.20/src/devapp/tools/infra/playbooks/1000:k_hello_world1.sh
+-rwxr-xr-x   0        0        0      448 2023-05-17 15:36:04.938861 devapps-2023.6.20/src/devapp/tools/infra/playbooks/100:docker.sh
+-rwxr-xr-x   0        0        0      324 2023-05-17 15:36:04.938861 devapps-2023.6.20/src/devapp/tools/infra/playbooks/200:tools.sh
+-rwxr-xr-x   0        0        0      760 2023-05-17 15:36:04.938861 devapps-2023.6.20/src/devapp/tools/infra/playbooks/300:dns.sh
+-rwxr-xr-x   0        0        0     4375 2023-05-17 15:36:04.938861 devapps-2023.6.20/src/devapp/tools/infra/playbooks/500:k3s.sh
+-rwxr-xr-x   0        0        0      943 2023-05-17 15:36:04.939861 devapps-2023.6.20/src/devapp/tools/infra/playbooks/501:kind.sh
+-rwxr-xr-x   0        0        0    17210 2023-05-17 15:36:04.939861 devapps-2023.6.20/src/devapp/tools/infra/playbooks/502:k3s.sh
+-rw-r--r--   0        0        0      276 2023-05-17 15:36:04.939861 devapps-2023.6.20/src/devapp/tools/infra/playbooks/510:label_workers.sh
+-rwxr-xr-x   0        0        0      661 2023-05-17 15:36:04.940861 devapps-2023.6.20/src/devapp/tools/infra/playbooks/600:longhorn.sh
+-rw-r--r--   0        0        0     1737 2023-05-17 15:36:04.941861 devapps-2023.6.20/src/devapp/tools/infra/playbooks/800:kube_hypermodern.sh
+-rw-r--r--   0        0        0    26850 2023-05-17 15:36:04.942861 devapps-2023.6.20/src/devapp/tools/old.py
+-rw-r--r--   0        0        0     4415 2023-05-17 15:36:04.942861 devapps-2023.6.20/src/devapp/tools/plugin.py
+-rw-r--r--   0        0        0    27729 2023-06-12 11:18:59.001038 devapps-2023.6.20/src/devapp/tools/resource.py
+-rw-r--r--   0        0        0     1861 2023-05-17 15:36:04.942861 devapps-2023.6.20/src/devapp/tools/times.py
+-rwxr-xr-x   0        0        0        0 2023-05-17 15:36:04.943861 devapps-2023.6.20/src/devapp/utils/__init__.py
+-rwxr-xr-x   0        0        0    15787 2023-05-17 15:36:04.943861 devapps-2023.6.20/src/devapp/utils/os_.py
+-rwxr-xr-x   0        0        0     1871 2023-05-17 15:36:04.943861 devapps-2023.6.20/src/devapp/utils/py_source_env.py
+-rwxr-xr-x   0        0        0     9335 2023-05-17 15:36:04.944861 devapps-2023.6.20/src/devapp/utils/rx_tools.py
+-rwxr-xr-x   0        0        0    11529 2023-05-17 15:36:04.944861 devapps-2023.6.20/src/devapp/utils/vault.py
+-rwxr-xr-x   0        0        0     2134 2023-06-20 09:40:12.936499 devapps-2023.6.20/src/devapp/utils/watch_dog.py
+-rwxr-xr-x   0        0        0        0 2023-03-22 14:30:25.734938 devapps-2023.6.20/src/mdvl/__init__.py
+-rwxr-xr-x   0        0        0    20402 2023-05-02 08:41:56.784342 devapps-2023.6.20/src/mdvl/mdvl.py
+-rwxr-xr-x   0        0        0     2317 2023-03-22 14:30:25.735939 devapps-2023.6.20/src/mdvl/tools.py
+-rwxr-xr-x   0        0        0      519 2023-05-17 15:36:04.945861 devapps-2023.6.20/src/structlogging/__init__.py
+-rwxr-xr-x   0        0        0     1559 2023-05-17 15:36:04.945861 devapps-2023.6.20/src/structlogging/adapters.py
+-rwxr-xr-x   0        0        0       88 2023-05-17 15:36:04.946861 devapps-2023.6.20/src/structlogging/common.py
+-rwxr-xr-x   0        0        0     5503 2023-05-17 15:36:04.946861 devapps-2023.6.20/src/structlogging/config.py
+-rwxr-xr-x   0        0        0     1618 2023-05-17 15:36:04.946861 devapps-2023.6.20/src/structlogging/formatters.py
+-rwxr-xr-x   0        0        0     2640 2023-05-17 15:36:04.946861 devapps-2023.6.20/src/structlogging/processors.py
+-rwxr-xr-x   0        0        0     5472 2023-05-17 15:36:04.946861 devapps-2023.6.20/src/structlogging/renderers.py
+-rwxr-xr-x   0        0        0    11172 2023-05-17 15:36:04.947861 devapps-2023.6.20/src/structlogging/sl.py
+-rw-r--r--   0        0        0     4022 2023-05-17 15:36:04.947861 devapps-2023.6.20/src/structlogging/stacktrace.py
+-rwxr-xr-x   0        0        0     1355 2023-05-17 15:36:04.947861 devapps-2023.6.20/src/structlogging/tests/test_structlogging.py
+-rwxr-xr-x   0        0        0      886 2023-05-02 12:47:20.254964 devapps-2023.6.20/src/theming/__init__.py
+-rwxr-xr-x   0        0        0    14865 2023-05-02 12:47:20.254964 devapps-2023.6.20/src/theming/absl_color_help.py
+-rwxr-xr-x   0        0        0     4345 2023-05-02 12:47:20.255964 devapps-2023.6.20/src/theming/ansi2html.py
+-rwxr-xr-x   0        0        0    11888 2023-05-02 12:47:20.255964 devapps-2023.6.20/src/theming/ansi2html.sh
+-rwxr-xr-x   0        0        0     3030 2023-05-02 12:47:20.255964 devapps-2023.6.20/src/theming/ansistrm.py
+-rwxr-xr-x   0        0        0    10066 2023-05-02 12:47:20.255964 devapps-2023.6.20/src/theming/ax_xml.py
+-rwxr-xr-x   0        0        0    10495 2023-05-02 12:47:20.255964 devapps-2023.6.20/src/theming/camel_snake.py
+-rwxr-xr-x   0        0        0     7517 2023-05-02 12:47:20.256964 devapps-2023.6.20/src/theming/charting.py
+-rwxr-xr-x   0        0        0     3392 2023-05-02 12:47:20.256964 devapps-2023.6.20/src/theming/colorhilite.py
+-rwxr-xr-x   0        0        0     1113 2023-05-02 12:47:20.256964 devapps-2023.6.20/src/theming/filesize/README.txt
+-rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.256964 devapps-2023.6.20/src/theming/filesize/__init__.py
+-rwxr-xr-x   0        0        0     2549 2023-05-02 12:47:20.256964 devapps-2023.6.20/src/theming/filesize/filesize.py
+-rwxr-xr-x   0        0        0     3756 2023-05-02 12:47:20.257964 devapps-2023.6.20/src/theming/formatters.py
+-rw-r--r--   0        0        0     3807 2023-05-02 12:47:20.257964 devapps-2023.6.20/src/theming/formatting/markdown.py
+-rw-r--r--   0        0        0     1241 2023-05-02 12:47:20.257964 devapps-2023.6.20/src/theming/formatting/viz_sequence.py
+-rwxr-xr-x   0        0        0     3410 2023-05-02 12:47:20.257964 devapps-2023.6.20/src/theming/html_tools.py
+-rwxr-xr-x   0        0        0    11409 2023-05-02 12:47:20.257964 devapps-2023.6.20/src/theming/inflect.py
+-rwxr-xr-x   0        0        0      460 2023-05-02 12:47:20.258964 devapps-2023.6.20/src/theming/msgs.py
+-rwxr-xr-x   0        0        0     9864 2023-05-02 12:47:20.258964 devapps-2023.6.20/src/theming/pretty_print.py
+-rwxr-xr-x   0        0        0    55699 2023-05-02 12:47:20.258964 devapps-2023.6.20/src/theming/tablepretty.py
+-rwxr-xr-x   0        0        0    13998 2023-05-02 12:47:20.259964 devapps-2023.6.20/src/theming/term.py
+-rwxr-xr-x   0        0        0     1468 2023-05-02 12:47:20.259964 devapps-2023.6.20/src/theming/term_struct_hilite.py
+-rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.259964 devapps-2023.6.20/src/theming/test
+-rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.259964 devapps-2023.6.20/src/theming/tests/__init__.py
+-rwxr-xr-x   0        0        0     9454 2023-05-02 12:47:20.260964 devapps-2023.6.20/src/theming/tests/test_text_formatting.py
+-rwxr-xr-x   0        0        0     1063 2023-05-02 12:47:20.260964 devapps-2023.6.20/src/theming/tracebacks.py
+-rwxr-xr-x   0        0        0     3011 2023-05-02 12:47:20.260964 devapps-2023.6.20/src/theming/unicode_chars.py
+-rwxr-xr-x   0        0        0    23138 2023-03-23 18:50:41.169018 devapps-2023.6.20/src/tree_builder/__init__.py
+-rwxr-xr-x   0        0        0    19864 2023-03-23 18:50:41.169018 devapps-2023.6.20/src/tree_builder/arch/__init__.py.bak
+-rwxr-xr-x   0        0        0     7762 2023-03-23 18:50:41.169018 devapps-2023.6.20/src/tree_builder/arch/links.py.bak
+-rwxr-xr-x   0        0        0    11455 2023-03-23 18:50:41.169018 devapps-2023.6.20/src/tree_builder/arch/o.py
+-rwxr-xr-x   0        0        0    19872 2023-03-23 18:50:41.170018 devapps-2023.6.20/src/tree_builder/arch/old
+-rwxr-xr-x   0        0        0    10911 2023-03-23 18:50:41.170018 devapps-2023.6.20/src/tree_builder/arch/olinit
+-rwxr-xr-x   0        0        0    11597 2023-03-23 18:50:41.170018 devapps-2023.6.20/src/tree_builder/arch/oo
+-rwxr-xr-x   0        0        0      154 2023-03-23 18:50:41.170018 devapps-2023.6.20/src/tree_builder/arch/py2.py
+-rwxr-xr-x   0        0        0     7968 2023-03-23 18:50:41.170018 devapps-2023.6.20/src/tree_builder/arch/render.py.bak
+-rwxr-xr-x   0        0        0     2078 2023-03-23 18:50:41.170018 devapps-2023.6.20/src/tree_builder/chrome_reload.sh
+-rwxr-xr-x   0        0        0     5502 2023-03-23 18:50:41.170018 devapps-2023.6.20/src/tree_builder/delivery2.py
+-rwxr-xr-x   0        0        0    10773 2023-03-23 18:50:41.171018 devapps-2023.6.20/src/tree_builder/links.py
+-rwxr-xr-x   0        0        0      218 2023-03-23 18:50:41.171018 devapps-2023.6.20/src/tree_builder/py3.py
+-rwxr-xr-x   0        0        0     8028 2023-03-23 18:50:41.171018 devapps-2023.6.20/src/tree_builder/render.py
+-rwxr-xr-x   0        0        0       21 2023-03-23 18:50:41.171018 devapps-2023.6.20/src/tree_builder/version.py
+-rw-r--r--   0        0        0     3129 2023-06-20 14:21:57.163617 devapps-2023.6.20/setup.py
+-rw-r--r--   0        0        0     1805 2023-06-20 14:21:57.163899 devapps-2023.6.20/PKG-INFO
```

### Comparing `devapps-2023.5.30/LICENSE` & `devapps-2023.6.20/LICENSE`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/README.md` & `devapps-2023.6.20/README.md`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/pyproject.toml` & `devapps-2023.6.20/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "devapps"
-version = "2023.05.30"
+version = "2023.06.20"
 description = "Apps - End to End."
 authors = ["Gunther Klessinger <g_kle_ss_ing_er@gmx.de>"]
 license = "BSD"
 readme = "README.md"
 repository = "https://github.com/AXGKl/devapps"
 homepage = "https://axgkl.github.io/devapps"
 keywords = []
```

### Comparing `devapps-2023.5.30/src/ax/utils/ax_tree/_ax_tree.so` & `devapps-2023.6.20/src/ax/utils/ax_tree/_ax_tree.so`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/ax/utils/ax_tree/ax_tree.py` & `devapps-2023.6.20/src/ax/utils/ax_tree/ax_tree.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/app.py` & `devapps-2023.6.20/src/devapp/app.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/app_token/create_tokens.py` & `devapps-2023.6.20/src/devapp/app_token/create_tokens.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/app_token/read_tokens.py` & `devapps-2023.6.20/src/devapp/app_token/read_tokens.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/components/cloudfoundry.py` & `devapps-2023.6.20/src/devapp/components/cloudfoundry.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/components/gitlab.py` & `devapps-2023.6.20/src/devapp/components/gitlab.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/components/gitlab_runner.py` & `devapps-2023.6.20/src/devapp/components/gitlab_runner.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/dev_mode.py` & `devapps-2023.6.20/src/devapp/dev_mode.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/gevent_patched.py` & `devapps-2023.6.20/src/devapp/gevent_patched.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/layer.py` & `devapps-2023.6.20/src/devapp/layer.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/lib/sh.py` & `devapps-2023.6.20/src/devapp/lib/sh.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/load.py` & `devapps-2023.6.20/src/devapp/load.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/logo` & `devapps-2023.6.20/src/devapp/logo`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/max.py` & `devapps-2023.6.20/src/devapp/max.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/operations/resources.py` & `devapps-2023.6.20/src/devapp/operations/resources.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/plugins/dev_devapp/personal_development_sandbox/__init__.py` & `devapps-2023.6.20/src/devapp/plugins/dev_devapp/personal_development_sandbox/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/plugins/dev_devapp/repo_sym_links.py` & `devapps-2023.6.20/src/devapp/plugins/dev_devapp/repo_sym_links.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/plugins/ops_devapp/arch/resource_install.py` & `devapps-2023.6.20/src/devapp/plugins/ops_devapp/arch/resource_install.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/plugins/ops_devapp/arch/resource_run.py` & `devapps-2023.6.20/src/devapp/plugins/ops_devapp/arch/resource_run.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/plugins/ops_devapp/arch/resources.py.dis` & `devapps-2023.6.20/src/devapp/plugins/ops_devapp/arch/resources.py.dis`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/plugins/ops_devapp/arch/resources_list.py` & `devapps-2023.6.20/src/devapp/plugins/ops_devapp/arch/resources_list.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/plugins/ops_devapp/arch/wait_for_port.py` & `devapps-2023.6.20/src/devapp/plugins/ops_devapp/arch/wait_for_port.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/plugins/ops_devapp/container_build.py` & `devapps-2023.6.20/src/devapp/plugins/ops_devapp/container_build.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/plugins/ops_devapp/container_pull.py` & `devapps-2023.6.20/src/devapp/plugins/ops_devapp/container_pull.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/plugins/ops_devapp/fs_build.py` & `devapps-2023.6.20/src/devapp/plugins/ops_devapp/fs_build.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/plugins/ops_devapp/infra_aws_cloud/__init__.py` & `devapps-2023.6.20/src/devapp/plugins/ops_devapp/infra_aws_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/plugins/ops_devapp/infra_digital_ocean/__init__.py` & `devapps-2023.6.20/src/devapp/plugins/ops_devapp/infra_digital_ocean/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/plugins/ops_devapp/infra_hetzner_cloud/__init__.py` & `devapps-2023.6.20/src/devapp/plugins/ops_devapp/infra_hetzner_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/plugins/ops_devapp/kubectl/__init__.py` & `devapps-2023.6.20/src/devapp/plugins/ops_devapp/kubectl/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/plugins/ops_devapp/life_cycle.py` & `devapps-2023.6.20/src/devapp/plugins/ops_devapp/life_cycle.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/plugins/ops_devapp/log_view.py` & `devapps-2023.6.20/src/devapp/plugins/ops_devapp/log_view.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/plugins/ops_devapp/pkgs.py` & `devapps-2023.6.20/src/devapp/plugins/ops_devapp/pkgs.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/plugins/ops_devapp/project/__init__.py` & `devapps-2023.6.20/src/devapp/plugins/ops_devapp/project/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,14 @@
     #         d = False
     class force_reinstall:
         n = 'Do not only install resources detected uninstalled but reinstall all'
         d = False
 
     class init_at:
         n = 'Set up project in given directory. env vars / relative dirs supported. Sets install action implicitly'
-        d = '.'
 
     class dev_install:
         n = 'Set the project up in developer mode - incl. make and poetry file machinery'
         d = False
 
     class init_create_all_units:
         n = 'If set we create unit files for ALL service type resources'
@@ -262,24 +261,27 @@
     if d:
         app.info('Disabled (only via -irm)', resources=[i.name for i in d])
     [rscs.remove(r) for r in list(rscs) if r in d]
     return rscs
 
 
 def run():
-    if FLG.init_resource_match or FLG.init_at:
+
+    if FLG.install or FLG.init_resource_match or FLG.init_at:
         # backwards compat
+        FLG.init_at = FLG.init_at or '.'
         FLG.list = False
         FLG.install = True
 
     if FLG.list_resources_files or FLG.list:
         rscs = get_matching_resources()
         app.info('Listing Defined Resources')
         app.info('details', json=rscs_dicts(rscs))
         return [r for r in rscs]
+
     m = FLG.delete_all_matching_service_unit_files
     if m:
         return do(delete_all_matching_service_unit_files, match=m)
 
     if FLG.edit_matching_resource_file:
         return start_editor()
```

### Comparing `devapps-2023.5.30/src/devapp/plugins/ops_devapp/project/devinstall/__init__.py` & `devapps-2023.6.20/src/devapp/plugins/ops_devapp/project/devinstall/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/plugins/ops_devapp/run.py` & `devapps-2023.6.20/src/devapp/plugins/ops_devapp/run.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/run.py` & `devapps-2023.6.20/src/devapp/run.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/spec/build.py` & `devapps-2023.6.20/src/devapp/spec/build.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/spec/find_paths_in_fs_components.py` & `devapps-2023.6.20/src/devapp/spec/find_paths_in_fs_components.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/spec/fs_components.py` & `devapps-2023.6.20/src/devapp/spec/fs_components.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/spec/links.py` & `devapps-2023.6.20/src/devapp/spec/links.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/spec/os_tools.py` & `devapps-2023.6.20/src/devapp/spec/os_tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/spec/templ.py` & `devapps-2023.6.20/src/devapp/spec/templ.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/spec/templates/unit` & `devapps-2023.6.20/src/devapp/spec/templates/unit`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/spec/tools.py` & `devapps-2023.6.20/src/devapp/spec/tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/t` & `devapps-2023.6.20/src/devapp/t`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/testing/auto_docs.py` & `devapps-2023.6.20/src/devapp/testing/auto_docs.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/third/rpl` & `devapps-2023.6.20/src/devapp/third/rpl`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/tools/__init__.py` & `devapps-2023.6.20/src/devapp/tools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -663,14 +663,17 @@
 def download_file(url, local_filename, auto_extract=True):
     """auto extract works for exe types like hugo.tar.gz -> contains in same dir the hugo binary.
     if the .tar.gz is containing a bin dir then the user should rather not say type
     is 'exe' but type is archive or so
     """
     import requests
     from devapp.app import app
+    local_filename = abspath(local_filename)
+    d = dirname(local_filename)
+    os.makedirs(d, exist_ok=True)
 
     app.info('Downloading', url=url, to=local_filename)
     r = requests.get(url, stream=True)
     arch, fn = None, local_filename
     if auto_extract:
         for k in archives:
             if url.endswith(k):
@@ -1351,15 +1354,15 @@
 
     TODO: other formats than pyproject.toml
 
     """
 
     config, dir_home, fn_cfg = {}, None, None
 
-    def root(no_fail=False):
+    def root(no_fail=False)->str:
         # r = FLG.project_directory or os.environ.get('project_directory')
         # if r:
         #     if not exists(r):
         #         from devapp.app import app
 
         #         os.makedirs(r)
         #         os.system('cd "%s"; git init' % r)
```

### Comparing `devapps-2023.5.30/src/devapp/tools/flag.py` & `devapps-2023.6.20/src/devapp/tools/flag.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/tools/http.py` & `devapps-2023.6.20/src/devapp/tools/http.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/tools/infra/__init__.py` & `devapps-2023.6.20/src/devapp/tools/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/tools/infra/actions.py` & `devapps-2023.6.20/src/devapp/tools/infra/actions.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/tools/infra/playbooks/000:functions.sh` & `devapps-2023.6.20/src/devapp/tools/infra/playbooks/000:functions.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/tools/infra/playbooks/1000:k_hello_world1.sh` & `devapps-2023.6.20/src/devapp/tools/infra/playbooks/1000:k_hello_world1.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/tools/infra/playbooks/300:dns.sh` & `devapps-2023.6.20/src/devapp/tools/infra/playbooks/300:dns.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/tools/infra/playbooks/500:k3s.sh` & `devapps-2023.6.20/src/devapp/tools/infra/playbooks/500:k3s.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/tools/infra/playbooks/501:kind.sh` & `devapps-2023.6.20/src/devapp/tools/infra/playbooks/501:kind.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/tools/infra/playbooks/502:k3s.sh` & `devapps-2023.6.20/src/devapp/tools/infra/playbooks/502:k3s.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/tools/infra/playbooks/600:longhorn.sh` & `devapps-2023.6.20/src/devapp/tools/infra/playbooks/600:longhorn.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/tools/infra/playbooks/800:kube_hypermodern.sh` & `devapps-2023.6.20/src/devapp/tools/infra/playbooks/800:kube_hypermodern.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/tools/old.py` & `devapps-2023.6.20/src/devapp/tools/old.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/tools/plugin.py` & `devapps-2023.6.20/src/devapp/tools/plugin.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/tools/resource.py` & `devapps-2023.6.20/src/devapp/tools/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,34 @@
     exists,
     repl_dollar_var_with_env_val,
     dirname,
     write_file,
     read_file,
 )
 
+
+class S:
+    """state"""
+
+    is_mamba = True
+    rscs_defined = None  # from resource_list
+    pkg_cmd = None
+    rsc_modified = False
+    name_to_func = {}
+    conda_prefix = None  # env vars replaced
+    fs_dir = None  # filesystem install dest
+    constants = {}
+    rsc_dirs = {}
+
+
 # mamba support hack
 MRP = os.environ.get('MAMBA_ROOT_PREFIX')
 CP = os.environ.get('CONDA_PREFIX', '').split('/envs/')[0]
 if CP:
+    S.is_mamba = CP == MRP
     MRP = CP
 
 os.environ['CONDA_PREFIX'] = CP
 
 
 T_unit = """
 [Unit]
@@ -55,27 +71,14 @@
 
 # _MATCH_ (auto created %(ctime)s) 
 """
 unit_match = 'DevApp Unit'
 T_unit = T_unit.replace('_MATCH_', unit_match)
 
 
-class S:
-    """state"""
-
-    rscs_defined = None  # from resource_list
-    pkg_cmd = None
-    rsc_modified = False
-    name_to_func = {}
-    conda_prefix = None  # env vars replaced
-    fs_dir = None  # filesystem install dest
-    constants = {}
-    rsc_dirs = {}
-
-
 def add_const(key, val, skip_exists=True):
     """import order matters, i.e. 4A's flows file will overrule lc-py"""
     v = S.constants.get(key)
     if v is not None:
         app.warn('Overwriting constant %s' % key, have=v, new=val)
     S.constants[key] = val
 
@@ -542,34 +545,35 @@
 
     class Conda:
         def conda_env(rsc):
             D = S.conda_prefix
 
             # return False if not dp else all([exists(dp + '/' + p) for p in rsc.provides])
             if not exists(D + '/bin/'):
+                app.warn('Conda base not fully installed')
                 do(Install.Conda.base, location=D)
 
             if str(rsc.path).startswith(D):
                 return app.debug('already installed - skipping', rsc=rsc)
 
             env = g(rsc, 'conda_env', rsc.name)
             ctx = dict(D=D, name=env, yes=interactive())
             mamba = os.environ.get('MAMBA_EXE')
             # if os.system('type micromamba') == 0 or 1:
-            if mamba and MRP:
+            if S.is_mamba and mamba and MRP:
                 ctx['conda'] = mamba
                 # FIXME: The activate during docker build is a problem in micromamba which runs as subprocess
                 # Better create the env via micromamba create -n foo -f <yaml file> first
                 cmd = [
                     '%(conda)s create %(yes)s -n "%(name)s"',
                     f'. "{MRP}/etc/profile.d/micromamba.sh"',
                     'micromamba activate "%(name)s"',
                 ]
 
-            elif mamba:
+            elif S.is_mamba and mamba:
                 ctx['conda'] = mamba
                 # FIXME: The activate during docker build is a problem in micromamba which runs as subprocess
                 # Better create the env via micromamba create -n foo -f <yaml file> first
                 cmd = [
                     '%(conda)s create %(yes)s -n "%(name)s"',
                     'eval "$(%(conda)s shell hook --shell=bash)"',
                     '%(conda)s activate "%(name)s"',
```

### Comparing `devapps-2023.5.30/src/devapp/tools/times.py` & `devapps-2023.6.20/src/devapp/tools/times.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/utils/os_.py` & `devapps-2023.6.20/src/devapp/utils/os_.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/utils/py_source_env.py` & `devapps-2023.6.20/src/devapp/utils/py_source_env.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/utils/rx_tools.py` & `devapps-2023.6.20/src/devapp/utils/rx_tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/utils/vault.py` & `devapps-2023.6.20/src/devapp/utils/vault.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/devapp/utils/watch_dog.py` & `devapps-2023.6.20/src/devapp/utils/watch_dog.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
             out(WD + f'Matching event: {event.event_type}  path : {event.src_path} {_}')
             try:
                 os.kill(int(pid), sig)
             except:
                 pass
             if sig != signal_handled:
                 out(WD + 'Exitting watchdog')
+                die[0] = 1
                 sys.exit(0)
 
     o, h = Observer(), H()
     if isinstance(match, str):
         h.match = match
     else:
         raise Exception('spec not supported')
```

### Comparing `devapps-2023.5.30/src/mdvl/mdvl.py` & `devapps-2023.6.20/src/mdvl/mdvl.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/mdvl/tools.py` & `devapps-2023.6.20/src/mdvl/tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/structlogging/__init__.py` & `devapps-2023.6.20/src/structlogging/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/structlogging/adapters.py` & `devapps-2023.6.20/src/structlogging/adapters.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/structlogging/config.py` & `devapps-2023.6.20/src/structlogging/config.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/structlogging/formatters.py` & `devapps-2023.6.20/src/structlogging/formatters.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/structlogging/processors.py` & `devapps-2023.6.20/src/structlogging/processors.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/structlogging/renderers.py` & `devapps-2023.6.20/src/structlogging/renderers.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/structlogging/sl.py` & `devapps-2023.6.20/src/structlogging/sl.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/structlogging/stacktrace.py` & `devapps-2023.6.20/src/structlogging/stacktrace.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/structlogging/tests/test_structlogging.py` & `devapps-2023.6.20/src/structlogging/tests/test_structlogging.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/theming/__init__.py` & `devapps-2023.6.20/src/theming/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/theming/absl_color_help.py` & `devapps-2023.6.20/src/theming/absl_color_help.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/theming/ansi2html.py` & `devapps-2023.6.20/src/theming/ansi2html.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/theming/ansi2html.sh` & `devapps-2023.6.20/src/theming/ansi2html.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/theming/ansistrm.py` & `devapps-2023.6.20/src/theming/ansistrm.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/theming/ax_xml.py` & `devapps-2023.6.20/src/theming/ax_xml.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/theming/camel_snake.py` & `devapps-2023.6.20/src/theming/camel_snake.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/theming/charting.py` & `devapps-2023.6.20/src/theming/charting.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/theming/colorhilite.py` & `devapps-2023.6.20/src/theming/colorhilite.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/theming/filesize/README.txt` & `devapps-2023.6.20/src/theming/filesize/README.txt`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/theming/filesize/filesize.py` & `devapps-2023.6.20/src/theming/filesize/filesize.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/theming/formatters.py` & `devapps-2023.6.20/src/theming/formatters.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/theming/formatting/markdown.py` & `devapps-2023.6.20/src/theming/formatting/markdown.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/theming/formatting/viz_sequence.py` & `devapps-2023.6.20/src/theming/formatting/viz_sequence.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/theming/html_tools.py` & `devapps-2023.6.20/src/theming/html_tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/theming/inflect.py` & `devapps-2023.6.20/src/theming/inflect.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/theming/pretty_print.py` & `devapps-2023.6.20/src/theming/pretty_print.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/theming/tablepretty.py` & `devapps-2023.6.20/src/theming/tablepretty.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/theming/term.py` & `devapps-2023.6.20/src/theming/term.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/theming/term_struct_hilite.py` & `devapps-2023.6.20/src/theming/term_struct_hilite.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/theming/tests/test_text_formatting.py` & `devapps-2023.6.20/src/theming/tests/test_text_formatting.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/theming/tracebacks.py` & `devapps-2023.6.20/src/theming/tracebacks.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/theming/unicode_chars.py` & `devapps-2023.6.20/src/theming/unicode_chars.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/tree_builder/__init__.py` & `devapps-2023.6.20/src/tree_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/tree_builder/arch/__init__.py.bak` & `devapps-2023.6.20/src/tree_builder/arch/__init__.py.bak`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/tree_builder/arch/links.py.bak` & `devapps-2023.6.20/src/tree_builder/arch/links.py.bak`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/tree_builder/arch/o.py` & `devapps-2023.6.20/src/tree_builder/arch/o.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/tree_builder/arch/old` & `devapps-2023.6.20/src/tree_builder/arch/old`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/tree_builder/arch/olinit` & `devapps-2023.6.20/src/tree_builder/arch/olinit`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/tree_builder/arch/oo` & `devapps-2023.6.20/src/tree_builder/arch/oo`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/tree_builder/arch/render.py.bak` & `devapps-2023.6.20/src/tree_builder/arch/render.py.bak`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/tree_builder/chrome_reload.sh` & `devapps-2023.6.20/src/tree_builder/chrome_reload.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/tree_builder/delivery2.py` & `devapps-2023.6.20/src/tree_builder/delivery2.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/tree_builder/links.py` & `devapps-2023.6.20/src/tree_builder/links.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/src/tree_builder/render.py` & `devapps-2023.6.20/src/tree_builder/render.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.30/setup.py` & `devapps-2023.6.20/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
  'devapp.plugins.ops_devapp.arch',
  'devapp.plugins.ops_devapp.infra_aws_cloud',
  'devapp.plugins.ops_devapp.infra_digital_ocean',
  'devapp.plugins.ops_devapp.infra_hetzner_cloud',
  'devapp.plugins.ops_devapp.kubectl',
  'devapp.plugins.ops_devapp.project',
  'devapp.plugins.ops_devapp.project.devinstall',
+ 'devapp.plugins.ops_devapp.system',
  'devapp.spec',
  'devapp.testing',
  'devapp.tests',
  'devapp.tools',
  'devapp.tools.infra',
  'devapp.utils',
  'mdvl',
@@ -38,14 +39,15 @@
  'theming.tests',
  'tree_builder',
  'tree_builder.arch']
 
 package_data = \
 {'': ['*'],
  'devapp': ['third/*'],
+ 'devapp.plugins.ops_devapp.system': ['templates/*'],
  'devapp.spec': ['templates/*'],
  'devapp.tools.infra': ['playbooks/*']}
 
 install_requires = \
 ['absl-py',
  'inflection',
  'jsondiff',
@@ -60,15 +62,15 @@
                      'dev = devapp.tools.plugin:main',
                      'fui = interactive.cli:main',
                      'myapp = devapp.tools.plugin:main',
                      'ops = devapp.tools.plugin:main']}
 
 setup_kwargs = {
     'name': 'devapps',
-    'version': '2023.5.30',
+    'version': '2023.6.20',
     'description': 'Apps - End to End.',
     'long_description': '# devapps\n\n\n<!-- badges -->\n[![docs pages][docs pages_img]][docs pages] [![gh-ci][gh-ci_img]][gh-ci] [![pkg][pkg_img]][pkg] [![code_style][code_style_img]][code_style] \n\n[docs pages]: https://axgkl.github.io/devapps/\n[docs pages_img]: https://axgkl.github.io/devapps/img/badge_docs.svg\n[gh-ci]: https://github.com/AXGKl/devapps/actions/workflows/ci.yml\n[gh-ci_img]: https://github.com/AXGKl/devapps/actions/workflows/ci.yml/badge.svg\n[pkg]: https://pypi.com/\n[pkg_img]: https://axgkl.github.io/devapps/img/badge_pypi.svg\n[code_style]: https://pypi.org/project/axblack/\n[code_style_img]: https://axgkl.github.io/devapps/img/badge_axblack.svg\n<!-- badges -->\n\n\nEnabler repo for dev *and* ops friendly apps, in a normalized way.\n\nIncludes:\n\n- logging (structlog)\n- cli flags handling (abseil, with addons)\n- docutools (mkdocs-material)\n- project setup\n- (test) resources management, including daemons and container filesystem layers\n\nand more.\n\n\n\n\nDocumentation: https://axgkl.github.io/devapps/',
     'author': 'Gunther Klessinger',
     'author_email': 'g_kle_ss_ing_er@gmx.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://axgkl.github.io/devapps',
```

### Comparing `devapps-2023.5.30/PKG-INFO` & `devapps-2023.6.20/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devapps
-Version: 2023.5.30
+Version: 2023.6.20
 Summary: Apps - End to End.
 Home-page: https://axgkl.github.io/devapps
 License: BSD
 Author: Gunther Klessinger
 Author-email: g_kle_ss_ing_er@gmx.de
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
```

