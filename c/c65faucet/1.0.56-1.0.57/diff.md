# Comparing `tmp/c65faucet-1.0.56.tar.gz` & `tmp/c65faucet-1.0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c65faucet-1.0.56.tar", last modified: Fri May 26 14:18:56 2023, max compression
+gzip compressed data, was "c65faucet-1.0.57.tar", last modified: Tue Jun 20 16:43:57 2023, max compression
```

## Comparing `c65faucet-1.0.56.tar` & `c65faucet-1.0.57.tar`

### file list

```diff
@@ -1,373 +1,373 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.300077 c65faucet-1.0.56/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-26 14:18:53.000000 c65faucet-1.0.56/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-26 14:18:53.000000 c65faucet-1.0.56/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-26 14:18:53.000000 c65faucet-1.0.56/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.236074 c65faucet-1.0.56/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-26 14:18:53.000000 c65faucet-1.0.56/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-26 14:18:53.000000 c65faucet-1.0.56/.github/renovate.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.240074 c65faucet-1.0.56/.github/workflows/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.240074 c65faucet-1.0.56/.github/workflows/disabled/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-26 14:18:53.000000 c65faucet-1.0.56/.github/workflows/disabled/periodic.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-26 14:18:53.000000 c65faucet-1.0.56/.github/workflows/disabled/release-debian.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-26 14:18:53.000000 c65faucet-1.0.56/.github/workflows/release-docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-26 14:18:53.000000 c65faucet-1.0.56/.github/workflows/release-python.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-26 14:18:53.000000 c65faucet-1.0.56/.github/workflows/tests-codecheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-05-26 14:18:53.000000 c65faucet-1.0.56/.github/workflows/tests-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-05-26 14:18:53.000000 c65faucet-1.0.56/.github/workflows/tests-integration.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-26 14:18:53.000000 c65faucet-1.0.56/.github/workflows/tests-unit.yml
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-26 14:18:53.000000 c65faucet-1.0.56/.github/workflows/tests-yaml-lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-26 14:18:53.000000 c65faucet-1.0.56/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-26 14:18:53.000000 c65faucet-1.0.56/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-26 14:18:53.000000 c65faucet-1.0.56/.renovaterc.json
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-26 14:18:56.000000 c65faucet-1.0.56/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-26 14:18:53.000000 c65faucet-1.0.56/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-26 14:18:56.000000 c65faucet-1.0.56/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-26 14:18:53.000000 c65faucet-1.0.56/Dockerfile.faucet
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-26 14:18:53.000000 c65faucet-1.0.56/Dockerfile.fuzz-config
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-26 14:18:53.000000 c65faucet-1.0.56/Dockerfile.fuzz-packet
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-26 14:18:53.000000 c65faucet-1.0.56/Dockerfile.gauge
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-26 14:18:53.000000 c65faucet-1.0.56/Dockerfile.tests
--rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-05-26 14:18:53.000000 c65faucet-1.0.56/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-26 14:18:53.000000 c65faucet-1.0.56/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-26 14:18:56.300077 c65faucet-1.0.56/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-26 14:18:53.000000 c65faucet-1.0.56/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.240074 c65faucet-1.0.56/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-26 14:18:53.000000 c65faucet-1.0.56/adapters/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.228074 c65faucet-1.0.56/adapters/vendors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.240074 c65faucet-1.0.56/adapters/vendors/faucetagent/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-26 14:18:53.000000 c65faucet-1.0.56/adapters/vendors/faucetagent/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-26 14:18:53.000000 c65faucet-1.0.56/adapters/vendors/faucetagent/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-26 14:18:53.000000 c65faucet-1.0.56/adapters/vendors/faucetagent/docker-compose.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      694 2023-05-26 14:18:53.000000 c65faucet-1.0.56/adapters/vendors/faucetagent/example_client.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1142 2023-05-26 14:18:53.000000 c65faucet-1.0.56/adapters/vendors/faucetagent/gencerts.sh
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-26 14:18:53.000000 c65faucet-1.0.56/adapters/vendors/faucetagent/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.244074 c65faucet-1.0.56/adapters/vendors/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-26 14:18:53.000000 c65faucet-1.0.56/adapters/vendors/rabbitmq/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-26 14:18:53.000000 c65faucet-1.0.56/adapters/vendors/rabbitmq/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-26 14:18:53.000000 c65faucet-1.0.56/adapters/vendors/rabbitmq/docker-compose-rabbitmq.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-26 14:18:53.000000 c65faucet-1.0.56/adapters/vendors/rabbitmq/docker-compose.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-26 14:18:53.000000 c65faucet-1.0.56/adapters/vendors/rabbitmq/example_consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.244074 c65faucet-1.0.56/adapters/vendors/rabbitmq/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-26 14:18:53.000000 c65faucet-1.0.56/adapters/vendors/rabbitmq/hooks/pre_build
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-05-26 14:18:53.000000 c65faucet-1.0.56/adapters/vendors/rabbitmq/rabbit.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 14:18:53.000000 c65faucet-1.0.56/adapters/vendors/rabbitmq/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-26 14:18:53.000000 c65faucet-1.0.56/adapters/vendors/rabbitmq/test_rabbit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.244074 c65faucet-1.0.56/c65faucet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-26 14:18:56.000000 c65faucet-1.0.56/c65faucet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-05-26 14:18:56.000000 c65faucet-1.0.56/c65faucet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:18:56.000000 c65faucet-1.0.56/c65faucet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-26 14:18:56.000000 c65faucet-1.0.56/c65faucet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:18:56.000000 c65faucet-1.0.56/c65faucet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-26 14:18:56.000000 c65faucet-1.0.56/c65faucet.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-26 14:18:56.000000 c65faucet-1.0.56/c65faucet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 14:18:56.000000 c65faucet-1.0.56/c65faucet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.248075 c65faucet-1.0.56/clib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:53.000000 c65faucet-1.0.56/clib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      540 2023-05-26 14:18:53.000000 c65faucet-1.0.56/clib/clib_mininet_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    35493 2023-05-26 14:18:53.000000 c65faucet-1.0.56/clib/clib_mininet_test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-05-26 14:18:53.000000 c65faucet-1.0.56/clib/clib_mininet_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    25032 2023-05-26 14:18:53.000000 c65faucet-1.0.56/clib/config_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-05-26 14:18:53.000000 c65faucet-1.0.56/clib/docker_host.py
--rw-r--r--   0 runner    (1001) docker     (123)    51086 2023-05-26 14:18:53.000000 c65faucet-1.0.56/clib/fakeoftable.py
--rw-r--r--   0 runner    (1001) docker     (123)   143186 2023-05-26 14:18:53.000000 c65faucet-1.0.56/clib/mininet_test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    34950 2023-05-26 14:18:53.000000 c65faucet-1.0.56/clib/mininet_test_base_topo.py
--rw-r--r--   0 runner    (1001) docker     (123)    30928 2023-05-26 14:18:53.000000 c65faucet-1.0.56/clib/mininet_test_topo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-05-26 14:18:53.000000 c65faucet-1.0.56/clib/mininet_test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-05-26 14:18:53.000000 c65faucet-1.0.56/clib/mininet_test_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-05-26 14:18:53.000000 c65faucet-1.0.56/clib/tcpdump_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)   118212 2023-05-26 14:18:53.000000 c65faucet-1.0.56/clib/valve_test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 14:18:53.000000 c65faucet-1.0.56/codecheck-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.252075 c65faucet-1.0.56/debian/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-26 14:18:53.000000 c65faucet-1.0.56/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-26 14:18:53.000000 c65faucet-1.0.56/debian/compat
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-26 14:18:53.000000 c65faucet-1.0.56/debian/control
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-26 14:18:53.000000 c65faucet-1.0.56/debian/copyright
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-26 14:18:53.000000 c65faucet-1.0.56/debian/faucet-all-in-one.install
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 14:18:53.000000 c65faucet-1.0.56/debian/faucet-docs.docs
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-26 14:18:53.000000 c65faucet-1.0.56/debian/faucet.default
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-26 14:18:53.000000 c65faucet-1.0.56/debian/faucet.install
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-26 14:18:53.000000 c65faucet-1.0.56/debian/faucet.postinst
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-26 14:18:53.000000 c65faucet-1.0.56/debian/faucet.service
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-26 14:18:53.000000 c65faucet-1.0.56/debian/gauge.default
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-26 14:18:53.000000 c65faucet-1.0.56/debian/gauge.install
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-26 14:18:53.000000 c65faucet-1.0.56/debian/gauge.postinst
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-26 14:18:53.000000 c65faucet-1.0.56/debian/gauge.service
--rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-05-26 14:18:53.000000 c65faucet-1.0.56/debian/rules
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.252075 c65faucet-1.0.56/debian/source/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 14:18:53.000000 c65faucet-1.0.56/debian/source/format
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-26 14:18:53.000000 c65faucet-1.0.56/debian/watch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.252075 c65faucet-1.0.56/docker/
--rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docker/fuzz_config.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docker/fuzz_packet.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1176 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docker/install-faucet.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1232 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docker/localtest.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      797 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docker/pip_deps.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docker/retrycmd.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     7205 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docker/runtests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      697 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docker/shard_tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docker-compose.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.256075 c65faucet-1.0.56/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.228074 c65faucet-1.0.56/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.256075 c65faucet-1.0.56/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/css/responsive-tables.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.256075 c65faucet-1.0.56/docs/_static/deployments/
--rw-r--r--   0 runner    (1001) docker     (123)    89120 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/deployments/ONF_Faucet_deploy1.png
--rw-r--r--   0 runner    (1001) docker     (123)   984943 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/deployments/nznog17-physical-network.jpg
--rw-r--r--   0 runner    (1001) docker     (123)  1106115 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/deployments/nznog17-virtual-network.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.260075 c65faucet-1.0.56/docs/_static/grafana-dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)    23629 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/grafana-dashboards/faucet_instrumentation.json
--rw-r--r--   0 runner    (1001) docker     (123)    22310 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/grafana-dashboards/faucet_inventory.json
--rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/grafana-dashboards/faucet_port_statistics.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.264075 c65faucet-1.0.56/docs/_static/images/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8466 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/images/8021X-conf-diagram.svg
--rw-r--r--   0 runner    (1001) docker     (123)    97737 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/images/faucet-architecture.svg
--rw-r--r--   0 runner    (1001) docker     (123)    23716 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/images/faucet-pipeline.png
--rw-r--r--   0 runner    (1001) docker     (123)    58351 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/images/faucet-pipeline.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/images/faucet-pipeline.txt
--rw-r--r--   0 runner    (1001) docker     (123)   136689 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/images/gauge-nznog17.png
--rw-r--r--   0 runner    (1001) docker     (123)   285918 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/images/gauge-snapshot1.png
--rw-r--r--   0 runner    (1001) docker     (123)   452164 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/images/gauge-snapshot2.png
--rw-r--r--   0 runner    (1001) docker     (123)   467326 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/images/gauge-snapshot3.png
--rw-r--r--   0 runner    (1001) docker     (123)    51732 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/images/tutorial-acls.svg
--rw-r--r--   0 runner    (1001) docker     (123)    77255 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/images/tutorial-bgp-routing.svg
--rw-r--r--   0 runner    (1001) docker     (123)    47652 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/images/tutorial-ivr.svg
--rw-r--r--   0 runner    (1001) docker     (123)   120062 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/images/tutorial-multi-root-stack.svg
--rw-r--r--   0 runner    (1001) docker     (123)    87114 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/images/tutorial-nfv-services.svg
--rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/images/tutorial-stack-loop.svg
--rw-r--r--   0 runner    (1001) docker     (123)    78230 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/images/tutorial-stack-tunnel.svg
--rw-r--r--   0 runner    (1001) docker     (123)    53594 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/images/tutorial-stack.svg
--rw-r--r--   0 runner    (1001) docker     (123)   109550 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/images/tutorial-stackwithivr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    59007 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/images/tutorial-static-routing.svg
--rw-r--r--   0 runner    (1001) docker     (123)   172474 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/images/tutorial-vlans.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.268075 c65faucet-1.0.56/docs/_static/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/tutorial/add_tagged_interface
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/tutorial/as_ns
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/tutorial/cleanup
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/tutorial/create_ns
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/tutorial/destroy_ns
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/_static/tutorial/inter_switch_link
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/architecture.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.268075 c65faucet-1.0.56/docs/autogen/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/autogen/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    40109 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14496 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/developer_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/external_resources.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/fuzzing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/monitoring.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.268075 c65faucet-1.0.56/docs/recipe_book/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/recipe_book/forwarding.rst
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/recipe_book/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/recipe_book/policy.rst
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/recipe_book/routing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.268075 c65faucet-1.0.56/docs/release_notes/
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/release_notes/1.7.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/release_notes/1.9.0.rst
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.268075 c65faucet-1.0.56/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.272076 c65faucet-1.0.56/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/tutorials/acls.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/tutorials/conntrack.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18441 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/tutorials/first_time.rst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17927 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/tutorials/nfv_services.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15268 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/tutorials/routing.rst
--rw-r--r--   0 runner    (1001) docker     (123)    30053 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/tutorials/stacking.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/tutorials/vlans.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.272076 c65faucet-1.0.56/docs/vendors/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.272076 c65faucet-1.0.56/docs/vendors/allied-telesis/
--rw-r--r--   0 runner    (1001) docker     (123)    14233 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/vendors/allied-telesis/README_Allied_Telesis.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.272076 c65faucet-1.0.56/docs/vendors/cisco/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9404 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/vendors/cisco/README_Cisco.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.272076 c65faucet-1.0.56/docs/vendors/hpe/
--rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/vendors/hpe/README_Aruba.rst
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/vendors/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.272076 c65faucet-1.0.56/docs/vendors/lagopus/
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/vendors/lagopus/README_Lagopus.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.272076 c65faucet-1.0.56/docs/vendors/northboundnetworks/
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/vendors/northboundnetworks/README_ZodiacFX.rst
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/vendors/northboundnetworks/README_ZodiacGX.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1292 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/vendors/northboundnetworks/conf-zodiac.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.272076 c65faucet-1.0.56/docs/vendors/noviflow/
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/vendors/noviflow/README_noviflow.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.272076 c65faucet-1.0.56/docs/vendors/ovs/
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/vendors/ovs/README_OVS-DPDK.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18223 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/vendors/ovs/faucet_ovs_test.png
--rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-05-26 14:18:53.000000 c65faucet-1.0.56/docs/vendors/ovs/faucet_testing_with_OVS_on_hardware.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.232074 c65faucet-1.0.56/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.272076 c65faucet-1.0.56/etc/default/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-26 14:18:53.000000 c65faucet-1.0.56/etc/default/faucet
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-26 14:18:53.000000 c65faucet-1.0.56/etc/default/gauge
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.276076 c65faucet-1.0.56/etc/faucet/
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-26 14:18:53.000000 c65faucet-1.0.56/etc/faucet/acls.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-26 14:18:53.000000 c65faucet-1.0.56/etc/faucet/faucet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-26 14:18:53.000000 c65faucet-1.0.56/etc/faucet/gauge.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-26 14:18:53.000000 c65faucet-1.0.56/etc/faucet/os_ken.conf
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-26 14:18:53.000000 c65faucet-1.0.56/etc/faucet/ryu.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.276076 c65faucet-1.0.56/etc/logrotate.d/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-26 14:18:53.000000 c65faucet-1.0.56/etc/logrotate.d/faucet
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-26 14:18:53.000000 c65faucet-1.0.56/etc/logrotate.d/gauge
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.276076 c65faucet-1.0.56/etc/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-26 14:18:53.000000 c65faucet-1.0.56/etc/prometheus/faucet.rules.yml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-26 14:18:53.000000 c65faucet-1.0.56/etc/prometheus/prometheus-docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-26 14:18:53.000000 c65faucet-1.0.56/etc/prometheus/prometheus.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.232074 c65faucet-1.0.56/etc/systemd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.276076 c65faucet-1.0.56/etc/systemd/system/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 14:18:53.000000 c65faucet-1.0.56/etc/systemd/system/faucet.service
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-26 14:18:53.000000 c65faucet-1.0.56/etc/systemd/system/gauge.service
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-26 14:18:53.000000 c65faucet-1.0.56/etc/systemd/system/prometheus.service
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.284076 c65faucet-1.0.56/faucet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5773 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35363 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/acl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2276 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/check_faucet_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    14246 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/config_parser_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    71188 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/dp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/faucet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/faucet_bgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/faucet_dot1x.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/faucet_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/faucet_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11424 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/faucet_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/faucet_pipeline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7755 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/fctl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/gauge.py
--rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/gauge_influx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/gauge_pollers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/gauge_prom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    31120 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/port.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/prom_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/router.py
--rw-r--r--   0 runner    (1001) docker     (123)    19588 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/tfm_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    73345 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/valve.py
--rw-r--r--   0 runner    (1001) docker     (123)    30131 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/valve_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/valve_coprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/valve_lldp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/valve_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    42091 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/valve_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/valve_of_old.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/valve_outonly.py
--rw-r--r--   0 runner    (1001) docker     (123)    28984 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/valve_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/valve_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    49835 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/valve_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/valve_ryuapp.py
--rw-r--r--   0 runner    (1001) docker     (123)    18431 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/valve_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/valve_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    30701 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/valve_switch_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)    52744 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/valve_switch_standalone.py
--rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/valve_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/valve_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    18634 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/valves_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    26043 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/vlan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-26 14:18:53.000000 c65faucet-1.0.56/faucet/watcher_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 14:18:53.000000 c65faucet-1.0.56/fuzz-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.284076 c65faucet-1.0.56/git-hook/
--rwxr-xr-x   0 runner    (1001) docker     (123)      456 2023-05-26 14:18:53.000000 c65faucet-1.0.56/git-hook/pre-commit
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-26 14:18:53.000000 c65faucet-1.0.56/helper-funcs
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-26 14:18:53.000000 c65faucet-1.0.56/hw_switch_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.284076 c65faucet-1.0.56/ofctl_rest/
--rw-r--r--   0 runner    (1001) docker     (123)    27150 2023-05-26 14:18:53.000000 c65faucet-1.0.56/ofctl_rest/ofctl_rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-05-26 14:18:53.000000 c65faucet-1.0.56/ofctl_rest/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-26 14:18:53.000000 c65faucet-1.0.56/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-26 14:18:56.300077 c65faucet-1.0.56/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3802 2023-05-26 14:18:53.000000 c65faucet-1.0.56/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-26 14:18:53.000000 c65faucet-1.0.56/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.284076 c65faucet-1.0.56/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.284076 c65faucet-1.0.56/tests/codecheck/
--rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/codecheck/flake8.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/codecheck/min_pylint.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/codecheck/pylint.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      342 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/codecheck/pytype.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      701 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/codecheck/src_files.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.232074 c65faucet-1.0.56/tests/generative/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.232074 c65faucet-1.0.56/tests/generative/fuzzer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.288076 c65faucet-1.0.56/tests/generative/fuzzer/config/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/config/config.dict
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.288076 c65faucet-1.0.56/tests/generative/fuzzer/config/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/config/examples/ex0
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/config/fuzz_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/config/generate_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.288076 c65faucet-1.0.56/tests/generative/fuzzer/packet/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/display_packet_crash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.292076 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/aoe.ex1
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/arp.ex1
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/arp.ex2
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/asap.ex1
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/asap.ex2
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/diameter.ex1
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/dns.ex1
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/dns.ex2
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/http.ex1
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/http.ex2
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/icmp.ex1
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/icmp.ex2
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/icmp.ex3
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/icmp.ex4
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/igmpv2.ex1
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/ipv4.ex1
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/ipv6.ex1
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/irc.ex1
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/irc.ex2
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/irc.ex3
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/lacp.ex1
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/msger.ex1
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/packet.dict
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/tcp.ex1
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/tcp.ex2
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/tcp.ex3
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/tcp.ex4
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/tcp.ex5
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/udp.ex1
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/udp.ex2
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/udp.ex3
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/udp.ex4
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/fake_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/fuzzer/packet/fuzz_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.292076 c65faucet-1.0.56/tests/generative/integration/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2304 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/integration/fault_tolerance_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    18304 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/integration/fault_tolerance_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.292076 c65faucet-1.0.56/tests/generative/unit/
--rwxr-xr-x   0 runner    (1001) docker     (123)    12779 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/generative/unit/test_topology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.292076 c65faucet-1.0.56/tests/integration/
--rwxr-xr-x   0 runner    (1001) docker     (123)      565 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/integration/mininet_main.py
--rw-r--r--   0 runner    (1001) docker     (123)   157767 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/integration/mininet_multidp_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)   308768 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/integration/mininet_tests.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      574 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/run_unit_tests.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      244 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/sysctls_for_tests.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.232074 c65faucet-1.0.56/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.296076 c65faucet-1.0.56/tests/unit/clib/
--rwxr-xr-x   0 runner    (1001) docker     (123)     8815 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/unit/clib/test_topo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.296076 c65faucet-1.0.56/tests/unit/faucet/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10401 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/unit/faucet/test_check_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   134114 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/unit/faucet/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6666 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/unit/faucet/test_fctl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1519 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/unit/faucet/test_main.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5773 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/unit/faucet/test_port.py
--rw-r--r--   0 runner    (1001) docker     (123)    31562 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/unit/faucet/test_valve.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    39651 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/unit/faucet/test_valve_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4960 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/unit/faucet/test_valve_dot1x.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5875 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/unit/faucet/test_valve_egress.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2968 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/unit/faucet/test_valve_of.py
--rw-r--r--   0 runner    (1001) docker     (123)   154810 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/unit/faucet/test_valve_stack.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2770 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/unit/faucet/test_valveapp_smoke.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9217 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/unit/faucet/test_vlan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.300077 c65faucet-1.0.56/tests/unit/gauge/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5590 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/unit/gauge/test_config_gauge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36917 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/unit/gauge/test_gauge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1516 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/unit/gauge/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:56.300077 c65faucet-1.0.56/tests/unit/packaging/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5501 2023-05-26 14:18:53.000000 c65faucet-1.0.56/tests/unit/packaging/test_packaging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.339960 c65faucet-1.0.57/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-20 16:43:54.000000 c65faucet-1.0.57/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 16:43:54.000000 c65faucet-1.0.57/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 16:43:54.000000 c65faucet-1.0.57/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.311960 c65faucet-1.0.57/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-20 16:43:54.000000 c65faucet-1.0.57/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-20 16:43:54.000000 c65faucet-1.0.57/.github/renovate.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.311960 c65faucet-1.0.57/.github/workflows/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.311960 c65faucet-1.0.57/.github/workflows/disabled/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-20 16:43:54.000000 c65faucet-1.0.57/.github/workflows/disabled/periodic.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-20 16:43:54.000000 c65faucet-1.0.57/.github/workflows/disabled/release-debian.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-06-20 16:43:54.000000 c65faucet-1.0.57/.github/workflows/release-docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-20 16:43:54.000000 c65faucet-1.0.57/.github/workflows/release-python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-06-20 16:43:54.000000 c65faucet-1.0.57/.github/workflows/tests-codecheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-20 16:43:54.000000 c65faucet-1.0.57/.github/workflows/tests-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-06-20 16:43:54.000000 c65faucet-1.0.57/.github/workflows/tests-integration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-20 16:43:54.000000 c65faucet-1.0.57/.github/workflows/tests-unit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-20 16:43:54.000000 c65faucet-1.0.57/.github/workflows/tests-yaml-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-20 16:43:54.000000 c65faucet-1.0.57/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-20 16:43:54.000000 c65faucet-1.0.57/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-20 16:43:54.000000 c65faucet-1.0.57/.renovaterc.json
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 16:43:57.000000 c65faucet-1.0.57/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-20 16:43:54.000000 c65faucet-1.0.57/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-20 16:43:57.000000 c65faucet-1.0.57/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-20 16:43:54.000000 c65faucet-1.0.57/Dockerfile.faucet
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-20 16:43:54.000000 c65faucet-1.0.57/Dockerfile.fuzz-config
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-20 16:43:54.000000 c65faucet-1.0.57/Dockerfile.fuzz-packet
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-20 16:43:54.000000 c65faucet-1.0.57/Dockerfile.gauge
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-20 16:43:54.000000 c65faucet-1.0.57/Dockerfile.tests
+-rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-06-20 16:43:54.000000 c65faucet-1.0.57/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-20 16:43:54.000000 c65faucet-1.0.57/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-20 16:43:57.339960 c65faucet-1.0.57/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-20 16:43:54.000000 c65faucet-1.0.57/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.311960 c65faucet-1.0.57/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-20 16:43:54.000000 c65faucet-1.0.57/adapters/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.303960 c65faucet-1.0.57/adapters/vendors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.311960 c65faucet-1.0.57/adapters/vendors/faucetagent/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-20 16:43:54.000000 c65faucet-1.0.57/adapters/vendors/faucetagent/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-20 16:43:54.000000 c65faucet-1.0.57/adapters/vendors/faucetagent/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-20 16:43:54.000000 c65faucet-1.0.57/adapters/vendors/faucetagent/docker-compose.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      694 2023-06-20 16:43:54.000000 c65faucet-1.0.57/adapters/vendors/faucetagent/example_client.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1142 2023-06-20 16:43:54.000000 c65faucet-1.0.57/adapters/vendors/faucetagent/gencerts.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 16:43:54.000000 c65faucet-1.0.57/adapters/vendors/faucetagent/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.311960 c65faucet-1.0.57/adapters/vendors/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-20 16:43:54.000000 c65faucet-1.0.57/adapters/vendors/rabbitmq/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-20 16:43:54.000000 c65faucet-1.0.57/adapters/vendors/rabbitmq/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-20 16:43:54.000000 c65faucet-1.0.57/adapters/vendors/rabbitmq/docker-compose-rabbitmq.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-20 16:43:54.000000 c65faucet-1.0.57/adapters/vendors/rabbitmq/docker-compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-20 16:43:54.000000 c65faucet-1.0.57/adapters/vendors/rabbitmq/example_consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.311960 c65faucet-1.0.57/adapters/vendors/rabbitmq/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-20 16:43:54.000000 c65faucet-1.0.57/adapters/vendors/rabbitmq/hooks/pre_build
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-06-20 16:43:54.000000 c65faucet-1.0.57/adapters/vendors/rabbitmq/rabbit.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 16:43:54.000000 c65faucet-1.0.57/adapters/vendors/rabbitmq/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-20 16:43:54.000000 c65faucet-1.0.57/adapters/vendors/rabbitmq/test_rabbit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.311960 c65faucet-1.0.57/c65faucet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-20 16:43:57.000000 c65faucet-1.0.57/c65faucet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-06-20 16:43:57.000000 c65faucet-1.0.57/c65faucet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:43:57.000000 c65faucet-1.0.57/c65faucet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-20 16:43:57.000000 c65faucet-1.0.57/c65faucet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:43:57.000000 c65faucet-1.0.57/c65faucet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-20 16:43:57.000000 c65faucet-1.0.57/c65faucet.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-20 16:43:57.000000 c65faucet-1.0.57/c65faucet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 16:43:57.000000 c65faucet-1.0.57/c65faucet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.315960 c65faucet-1.0.57/clib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:54.000000 c65faucet-1.0.57/clib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      540 2023-06-20 16:43:54.000000 c65faucet-1.0.57/clib/clib_mininet_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35493 2023-06-20 16:43:54.000000 c65faucet-1.0.57/clib/clib_mininet_test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-06-20 16:43:54.000000 c65faucet-1.0.57/clib/clib_mininet_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25032 2023-06-20 16:43:54.000000 c65faucet-1.0.57/clib/config_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-06-20 16:43:54.000000 c65faucet-1.0.57/clib/docker_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51086 2023-06-20 16:43:54.000000 c65faucet-1.0.57/clib/fakeoftable.py
+-rw-r--r--   0 runner    (1001) docker     (123)   143186 2023-06-20 16:43:54.000000 c65faucet-1.0.57/clib/mininet_test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34950 2023-06-20 16:43:54.000000 c65faucet-1.0.57/clib/mininet_test_base_topo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32302 2023-06-20 16:43:54.000000 c65faucet-1.0.57/clib/mininet_test_topo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-06-20 16:43:54.000000 c65faucet-1.0.57/clib/mininet_test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-06-20 16:43:54.000000 c65faucet-1.0.57/clib/mininet_test_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-06-20 16:43:54.000000 c65faucet-1.0.57/clib/tcpdump_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118212 2023-06-20 16:43:54.000000 c65faucet-1.0.57/clib/valve_test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-20 16:43:54.000000 c65faucet-1.0.57/codecheck-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.315960 c65faucet-1.0.57/debian/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-20 16:43:54.000000 c65faucet-1.0.57/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-20 16:43:54.000000 c65faucet-1.0.57/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-20 16:43:54.000000 c65faucet-1.0.57/debian/control
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-20 16:43:54.000000 c65faucet-1.0.57/debian/copyright
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-20 16:43:54.000000 c65faucet-1.0.57/debian/faucet-all-in-one.install
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 16:43:54.000000 c65faucet-1.0.57/debian/faucet-docs.docs
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-20 16:43:54.000000 c65faucet-1.0.57/debian/faucet.default
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-20 16:43:54.000000 c65faucet-1.0.57/debian/faucet.install
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-20 16:43:54.000000 c65faucet-1.0.57/debian/faucet.postinst
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-20 16:43:54.000000 c65faucet-1.0.57/debian/faucet.service
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-20 16:43:54.000000 c65faucet-1.0.57/debian/gauge.default
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 16:43:54.000000 c65faucet-1.0.57/debian/gauge.install
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-20 16:43:54.000000 c65faucet-1.0.57/debian/gauge.postinst
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-20 16:43:54.000000 c65faucet-1.0.57/debian/gauge.service
+-rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-06-20 16:43:54.000000 c65faucet-1.0.57/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.315960 c65faucet-1.0.57/debian/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 16:43:54.000000 c65faucet-1.0.57/debian/source/format
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-20 16:43:54.000000 c65faucet-1.0.57/debian/watch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.315960 c65faucet-1.0.57/docker/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docker/fuzz_config.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docker/fuzz_packet.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1176 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docker/install-faucet.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1232 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docker/localtest.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      797 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docker/pip_deps.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      220 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docker/retrycmd.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7205 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docker/runtests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      697 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docker/shard_tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docker-compose.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.319960 c65faucet-1.0.57/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docs/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.307960 c65faucet-1.0.57/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.319960 c65faucet-1.0.57/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docs/_static/css/responsive-tables.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.319960 c65faucet-1.0.57/docs/_static/deployments/
+-rw-r--r--   0 runner    (1001) docker     (123)    89120 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docs/_static/deployments/ONF_Faucet_deploy1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   984943 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docs/_static/deployments/nznog17-physical-network.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)  1106115 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docs/_static/deployments/nznog17-virtual-network.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.319960 c65faucet-1.0.57/docs/_static/grafana-dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)    23629 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docs/_static/grafana-dashboards/faucet_instrumentation.json
+-rw-r--r--   0 runner    (1001) docker     (123)    22310 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docs/_static/grafana-dashboards/faucet_inventory.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18566 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docs/_static/grafana-dashboards/faucet_port_statistics.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.323960 c65faucet-1.0.57/docs/_static/images/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8466 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docs/_static/images/8021X-conf-diagram.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    97737 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docs/_static/images/faucet-architecture.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23716 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docs/_static/images/faucet-pipeline.png
+-rw-r--r--   0 runner    (1001) docker     (123)    58351 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docs/_static/images/faucet-pipeline.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docs/_static/images/faucet-pipeline.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   136689 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docs/_static/images/gauge-nznog17.png
+-rw-r--r--   0 runner    (1001) docker     (123)   285918 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docs/_static/images/gauge-snapshot1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   452164 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docs/_static/images/gauge-snapshot2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   467326 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docs/_static/images/gauge-snapshot3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    51732 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docs/_static/images/tutorial-acls.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    77255 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docs/_static/images/tutorial-bgp-routing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    47652 2023-06-20 16:43:54.000000 c65faucet-1.0.57/docs/_static/images/tutorial-ivr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   120062 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/_static/images/tutorial-multi-root-stack.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    87114 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/_static/images/tutorial-nfv-services.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/_static/images/tutorial-stack-loop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    78230 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/_static/images/tutorial-stack-tunnel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    53594 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/_static/images/tutorial-stack.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   109550 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/_static/images/tutorial-stackwithivr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    59007 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/_static/images/tutorial-static-routing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   172474 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/_static/images/tutorial-vlans.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.323960 c65faucet-1.0.57/docs/_static/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/_static/tutorial/add_tagged_interface
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/_static/tutorial/as_ns
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/_static/tutorial/cleanup
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/_static/tutorial/create_ns
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/_static/tutorial/destroy_ns
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/_static/tutorial/inter_switch_link
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/architecture.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.323960 c65faucet-1.0.57/docs/autogen/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/autogen/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40109 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14496 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/developer_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/external_resources.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/fuzzing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/monitoring.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.327960 c65faucet-1.0.57/docs/recipe_book/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/recipe_book/forwarding.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/recipe_book/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/recipe_book/policy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/recipe_book/routing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.327960 c65faucet-1.0.57/docs/release_notes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/release_notes/1.7.0.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/release_notes/1.9.0.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.327960 c65faucet-1.0.57/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.327960 c65faucet-1.0.57/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/tutorials/acls.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/tutorials/conntrack.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18441 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/tutorials/first_time.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17927 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/tutorials/nfv_services.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15268 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/tutorials/routing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    30053 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/tutorials/stacking.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/tutorials/vlans.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.327960 c65faucet-1.0.57/docs/vendors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.327960 c65faucet-1.0.57/docs/vendors/allied-telesis/
+-rw-r--r--   0 runner    (1001) docker     (123)    14233 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/vendors/allied-telesis/README_Allied_Telesis.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.327960 c65faucet-1.0.57/docs/vendors/cisco/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9404 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/vendors/cisco/README_Cisco.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.327960 c65faucet-1.0.57/docs/vendors/hpe/
+-rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/vendors/hpe/README_Aruba.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/vendors/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.327960 c65faucet-1.0.57/docs/vendors/lagopus/
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/vendors/lagopus/README_Lagopus.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.327960 c65faucet-1.0.57/docs/vendors/northboundnetworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/vendors/northboundnetworks/README_ZodiacFX.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/vendors/northboundnetworks/README_ZodiacGX.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1292 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/vendors/northboundnetworks/conf-zodiac.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.327960 c65faucet-1.0.57/docs/vendors/noviflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/vendors/noviflow/README_noviflow.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.327960 c65faucet-1.0.57/docs/vendors/ovs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/vendors/ovs/README_OVS-DPDK.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18223 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/vendors/ovs/faucet_ovs_test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9332 2023-06-20 16:43:55.000000 c65faucet-1.0.57/docs/vendors/ovs/faucet_testing_with_OVS_on_hardware.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.307960 c65faucet-1.0.57/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.327960 c65faucet-1.0.57/etc/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-20 16:43:55.000000 c65faucet-1.0.57/etc/default/faucet
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-20 16:43:55.000000 c65faucet-1.0.57/etc/default/gauge
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.327960 c65faucet-1.0.57/etc/faucet/
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-06-20 16:43:55.000000 c65faucet-1.0.57/etc/faucet/acls.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-06-20 16:43:55.000000 c65faucet-1.0.57/etc/faucet/faucet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-20 16:43:55.000000 c65faucet-1.0.57/etc/faucet/gauge.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-20 16:43:55.000000 c65faucet-1.0.57/etc/faucet/os_ken.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-20 16:43:55.000000 c65faucet-1.0.57/etc/faucet/ryu.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.327960 c65faucet-1.0.57/etc/logrotate.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-20 16:43:55.000000 c65faucet-1.0.57/etc/logrotate.d/faucet
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-20 16:43:55.000000 c65faucet-1.0.57/etc/logrotate.d/gauge
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.327960 c65faucet-1.0.57/etc/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-20 16:43:55.000000 c65faucet-1.0.57/etc/prometheus/faucet.rules.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 16:43:55.000000 c65faucet-1.0.57/etc/prometheus/prometheus-docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-20 16:43:55.000000 c65faucet-1.0.57/etc/prometheus/prometheus.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.307960 c65faucet-1.0.57/etc/systemd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.327960 c65faucet-1.0.57/etc/systemd/system/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-20 16:43:55.000000 c65faucet-1.0.57/etc/systemd/system/faucet.service
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 16:43:55.000000 c65faucet-1.0.57/etc/systemd/system/gauge.service
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-20 16:43:55.000000 c65faucet-1.0.57/etc/systemd/system/prometheus.service
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.335960 c65faucet-1.0.57/faucet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5773 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35363 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/acl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2276 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/check_faucet_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14246 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/config_parser_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71188 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/dp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/faucet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10311 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/faucet_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/faucet_dot1x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/faucet_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/faucet_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11424 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/faucet_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/faucet_pipeline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7755 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/fctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/gauge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/gauge_influx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9969 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/gauge_pollers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/gauge_prom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31120 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/prom_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19588 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/tfm_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73345 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/valve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30131 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/valve_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/valve_coprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/valve_lldp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/valve_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42091 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/valve_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/valve_of_old.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/valve_outonly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28984 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/valve_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/valve_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49835 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/valve_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/valve_ryuapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18431 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/valve_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/valve_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30701 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/valve_switch_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52744 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/valve_switch_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/valve_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/valve_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18634 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/valves_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26043 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/vlan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-06-20 16:43:55.000000 c65faucet-1.0.57/faucet/watcher_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 16:43:55.000000 c65faucet-1.0.57/fuzz-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.335960 c65faucet-1.0.57/git-hook/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      456 2023-06-20 16:43:55.000000 c65faucet-1.0.57/git-hook/pre-commit
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-20 16:43:55.000000 c65faucet-1.0.57/helper-funcs
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-20 16:43:55.000000 c65faucet-1.0.57/hw_switch_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.335960 c65faucet-1.0.57/ofctl_rest/
+-rw-r--r--   0 runner    (1001) docker     (123)    27150 2023-06-20 16:43:55.000000 c65faucet-1.0.57/ofctl_rest/ofctl_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-06-20 16:43:55.000000 c65faucet-1.0.57/ofctl_rest/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-20 16:43:55.000000 c65faucet-1.0.57/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-20 16:43:57.343961 c65faucet-1.0.57/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3802 2023-06-20 16:43:55.000000 c65faucet-1.0.57/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-20 16:43:55.000000 c65faucet-1.0.57/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.335960 c65faucet-1.0.57/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.335960 c65faucet-1.0.57/tests/codecheck/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/codecheck/flake8.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/codecheck/min_pylint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/codecheck/pylint.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      342 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/codecheck/pytype.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      701 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/codecheck/src_files.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.307960 c65faucet-1.0.57/tests/generative/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.307960 c65faucet-1.0.57/tests/generative/fuzzer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.335960 c65faucet-1.0.57/tests/generative/fuzzer/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/config/config.dict
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.335960 c65faucet-1.0.57/tests/generative/fuzzer/config/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/config/examples/ex0
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/config/fuzz_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/config/generate_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.335960 c65faucet-1.0.57/tests/generative/fuzzer/packet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/display_packet_crash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.339960 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/aoe.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/arp.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/arp.ex2
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/asap.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/asap.ex2
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/diameter.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/dns.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/dns.ex2
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/http.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/http.ex2
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/icmp.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/icmp.ex2
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/icmp.ex3
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/icmp.ex4
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/igmpv2.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/ipv4.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/ipv6.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/irc.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/irc.ex2
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/irc.ex3
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/lacp.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/msger.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/packet.dict
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/tcp.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/tcp.ex2
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/tcp.ex3
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/tcp.ex4
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/tcp.ex5
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/udp.ex1
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/udp.ex2
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/udp.ex3
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/udp.ex4
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/fake_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/fuzzer/packet/fuzz_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.339960 c65faucet-1.0.57/tests/generative/integration/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2304 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/integration/fault_tolerance_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18304 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/integration/fault_tolerance_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.339960 c65faucet-1.0.57/tests/generative/unit/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12779 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/generative/unit/test_topology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.339960 c65faucet-1.0.57/tests/integration/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      565 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/integration/mininet_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)   157767 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/integration/mininet_multidp_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)   308530 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/integration/mininet_tests.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      574 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/run_unit_tests.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      244 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/sysctls_for_tests.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.307960 c65faucet-1.0.57/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.339960 c65faucet-1.0.57/tests/unit/clib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8815 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/unit/clib/test_topo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.339960 c65faucet-1.0.57/tests/unit/faucet/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10401 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/unit/faucet/test_check_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   134114 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/unit/faucet/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6666 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/unit/faucet/test_fctl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1519 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/unit/faucet/test_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5773 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/unit/faucet/test_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31562 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/unit/faucet/test_valve.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39651 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/unit/faucet/test_valve_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4960 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/unit/faucet/test_valve_dot1x.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5875 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/unit/faucet/test_valve_egress.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2968 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/unit/faucet/test_valve_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)   154810 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/unit/faucet/test_valve_stack.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2770 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/unit/faucet/test_valveapp_smoke.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9217 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/unit/faucet/test_vlan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.339960 c65faucet-1.0.57/tests/unit/gauge/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5590 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/unit/gauge/test_config_gauge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36917 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/unit/gauge/test_gauge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1516 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/unit/gauge/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:43:57.339960 c65faucet-1.0.57/tests/unit/packaging/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5501 2023-06-20 16:43:55.000000 c65faucet-1.0.57/tests/unit/packaging/test_packaging.py
```

### Comparing `c65faucet-1.0.56/.github/workflows/disabled/periodic.yml` & `c65faucet-1.0.57/.github/workflows/disabled/periodic.yml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/.github/workflows/disabled/release-debian.yml` & `c65faucet-1.0.57/.github/workflows/disabled/release-debian.yml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/.github/workflows/release-docker.yml` & `c65faucet-1.0.57/.github/workflows/release-docker.yml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/.github/workflows/release-python.yml` & `c65faucet-1.0.57/.github/workflows/release-python.yml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/.github/workflows/tests-codecheck.yml` & `c65faucet-1.0.57/.github/workflows/tests-codecheck.yml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/.github/workflows/tests-docs.yml` & `c65faucet-1.0.57/.github/workflows/tests-docs.yml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/.github/workflows/tests-integration.yml` & `c65faucet-1.0.57/.github/workflows/tests-integration.yml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/.github/workflows/tests-unit.yml` & `c65faucet-1.0.57/.github/workflows/tests-unit.yml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/.pylintrc` & `c65faucet-1.0.57/.pylintrc`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/CONTRIBUTING.rst` & `c65faucet-1.0.57/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/LICENSE` & `c65faucet-1.0.57/LICENSE`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/Makefile` & `c65faucet-1.0.57/Makefile`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/PKG-INFO` & `c65faucet-1.0.57/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c65faucet
-Version: 1.0.56
+Version: 1.0.57
 Summary: Faucet is an OpenFlow controller that implements a layer 2 and layer 3 switch.
 Home-page: https://faucet.nz
 Author: Faucet development team
 Author-email: faucetsdn@googlegroups.com
 License: Apache-2
 Keywords: openflow,openvswitch,ryu
 Platform: any
```

### Comparing `c65faucet-1.0.56/README.rst` & `c65faucet-1.0.57/README.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/adapters/vendors/faucetagent/Dockerfile` & `c65faucet-1.0.57/adapters/vendors/faucetagent/Dockerfile`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/adapters/vendors/faucetagent/README.rst` & `c65faucet-1.0.57/adapters/vendors/faucetagent/README.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/adapters/vendors/faucetagent/example_client.sh` & `c65faucet-1.0.57/adapters/vendors/faucetagent/example_client.sh`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/adapters/vendors/faucetagent/gencerts.sh` & `c65faucet-1.0.57/adapters/vendors/faucetagent/gencerts.sh`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/adapters/vendors/rabbitmq/Dockerfile` & `c65faucet-1.0.57/adapters/vendors/rabbitmq/Dockerfile`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/adapters/vendors/rabbitmq/README.rst` & `c65faucet-1.0.57/adapters/vendors/rabbitmq/README.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/adapters/vendors/rabbitmq/docker-compose.yaml` & `c65faucet-1.0.57/adapters/vendors/rabbitmq/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/adapters/vendors/rabbitmq/example_consumer.py` & `c65faucet-1.0.57/adapters/vendors/rabbitmq/example_consumer.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/adapters/vendors/rabbitmq/rabbit.py` & `c65faucet-1.0.57/adapters/vendors/rabbitmq/rabbit.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/adapters/vendors/rabbitmq/test_rabbit.py` & `c65faucet-1.0.57/adapters/vendors/rabbitmq/test_rabbit.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/c65faucet.egg-info/PKG-INFO` & `c65faucet-1.0.57/c65faucet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c65faucet
-Version: 1.0.56
+Version: 1.0.57
 Summary: Faucet is an OpenFlow controller that implements a layer 2 and layer 3 switch.
 Home-page: https://faucet.nz
 Author: Faucet development team
 Author-email: faucetsdn@googlegroups.com
 License: Apache-2
 Keywords: openflow,openvswitch,ryu
 Platform: any
```

### Comparing `c65faucet-1.0.56/c65faucet.egg-info/SOURCES.txt` & `c65faucet-1.0.57/c65faucet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/clib/clib_mininet_test.py` & `c65faucet-1.0.57/clib/clib_mininet_test.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/clib/clib_mininet_test_main.py` & `c65faucet-1.0.57/clib/clib_mininet_test_main.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/clib/clib_mininet_tests.py` & `c65faucet-1.0.57/clib/clib_mininet_tests.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/clib/config_generator.py` & `c65faucet-1.0.57/clib/config_generator.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/clib/docker_host.py` & `c65faucet-1.0.57/clib/docker_host.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/clib/fakeoftable.py` & `c65faucet-1.0.57/clib/fakeoftable.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/clib/mininet_test_base.py` & `c65faucet-1.0.57/clib/mininet_test_base.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/clib/mininet_test_base_topo.py` & `c65faucet-1.0.57/clib/mininet_test_base_topo.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/clib/mininet_test_topo.py` & `c65faucet-1.0.57/clib/mininet_test_topo.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         node2,
         port1=None,
         port2=None,
         intf_name1=None,
         intf_name2=None,
         addr1=None,
         addr2=None,
-        **params
+        **params,
     ):
         Link.__init__(
             self,
             node1,
             node2,
             port1=port1,
             port2=port2,
@@ -74,16 +74,47 @@
 
 
 class FaucetHost(Host):
     """Base Mininet Host class, for Mininet-based tests."""
 
     def __init__(self, *args, **kwargs):
         self.pid_files = []
+        # Isolate these directories in mininet container from host filesystem
+        kwargs["privateDirs"] = [
+            ("/etc/", "/var/tmp/mininet/%(name)s/etc"),
+            ("/var/log/", "/var/tmp/mininet/%(name)s/var/log"),
+            ("/run/", "/var/tmp/mininet/%(name)s/run"),
+            ("/var/run/", "/var/tmp/mininet/%(name)s/var/run"),
+        ]
         super().__init__(*args, **kwargs)
 
+    def mountPrivateDirs(self):
+        "Mount private directories"
+        for directory in self.privateDirs:
+            if isinstance(directory, tuple):
+                # mount given private directory
+                privateDir = directory[1] % self.__dict__
+                mountPoint = directory[0]
+                self.cmd(f"mkdir -p {privateDir}")
+                self.cmd(f"cp -aRT {mountPoint} {privateDir}")
+                self.cmd(f"mount --bind {privateDir} {mountPoint}")
+            else:
+                # mount temporary filesystem on directory
+                self.cmd(f"mkdir -p {directory}")
+                self.cmd(f"mount -n -t tmpfs tmpfs {directory}")
+
+    def unmountPrivateDirs(self):
+        "Unmount private directories"
+        for directory in self.privateDirs:
+            if isinstance(directory, tuple):
+                self.cmd(f"umount {directory[0]}")
+                self.cmd(f"rm -r {directory[1]}")
+            else:
+                self.cmd(f"umount {directory}")
+
     def startShell(self, mnopts=None):
         "Start a shell process for running commands"
         if self.shell:
             error("%s: shell is already running\n" % self.name)
             return
         # mnexec: (c)lose descriptors, (d)etach from tty,
         # (p)rint pid, and run in (n)amespace
@@ -605,15 +636,15 @@
     def __init__(
         self,
         name,
         tmpdir,
         controller_intf=None,
         controller_ipv6=False,
         cargs="",
-        **kwargs
+        **kwargs,
     ):
         self.name_no_pid = name
         name_with_pid = "%s-%u" % (name, os.getpid())
         self.tmpdir = tmpdir
         self.controller_intf = controller_intf
         self.controller_ipv6 = controller_ipv6
         self.cached_ryu_pid = None
@@ -811,30 +842,30 @@
         ctl_privkey,
         ctl_cert,
         ca_certs,
         ports_sock,
         prom_port,
         port,
         test_name,
-        **kwargs
+        **kwargs,
     ):
         self.prom_port = prom_port
         self.ofctl_port = mininet_test_util.find_free_port(ports_sock, test_name)
         env["OFCTL_PORT"] = str(self.ofctl_port)
         env["OFCTL_HOST"] = mininet_test_util.LOCALHOSTV6
         cargs = " ".join(self._tls_cargs(port, ctl_privkey, ctl_cert, ca_certs))
         super().__init__(
             name,
             tmpdir,
             controller_intf,
             controller_ipv6,
             cargs=cargs,
             command=self._command(env, name, " ".join(self.START_ARGS)),
             port=port,
-            **kwargs
+            **kwargs,
         )
 
     def listening(self):
         return (
             self.listen_port(self.ofctl_port)
             and self.listen_port(self.prom_port)
             and super().listening()
@@ -851,19 +882,19 @@
         controller_intf,
         controller_ipv6,
         env,
         ctl_privkey,
         ctl_cert,
         ca_certs,
         port,
-        **kwargs
+        **kwargs,
     ):
         super().__init__(
             name,
             tmpdir,
             controller_intf,
             controller_ipv6,
             cargs=self._tls_cargs(port, ctl_privkey, ctl_cert, ca_certs),
             command=self._command(env, name, "--gauge"),
             port=port,
-            **kwargs
+            **kwargs,
         )
```

### Comparing `c65faucet-1.0.56/clib/mininet_test_util.py` & `c65faucet-1.0.57/clib/mininet_test_util.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/clib/mininet_test_watcher.py` & `c65faucet-1.0.57/clib/mininet_test_watcher.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/clib/tcpdump_helper.py` & `c65faucet-1.0.57/clib/tcpdump_helper.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/clib/valve_test_lib.py` & `c65faucet-1.0.57/clib/valve_test_lib.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/debian/control` & `c65faucet-1.0.57/debian/control`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 Vcs-Browser: https://github.com/faucetsdn/faucet
 
 Package: python3-faucet
 Architecture: all
 Depends: python3-influxdb (>= 2.12.0),
          python3-networkx (>= 1.9),
          python3-pbr (>= 1.9),
-         python3-prometheus-client (>= 0.16.0), python3-prometheus-client (<< 0.16.1),
-         python3-ruamel.yaml (>= 0.17.26), python3-ruamel.yaml (<< 0.17.27),
+         python3-prometheus-client (>= 0.17.0), python3-prometheus-client (<< 0.17.1),
+         python3-ruamel.yaml (>= 0.17.31), python3-ruamel.yaml (<< 0.17.32),
          python3-os-ken (>= 2.6.0), python3-os-ken (<< 2.6.1),
          python3-beka (>= 0.4.2), python3-beka (<< 0.4.3),
          python3-chewie (>= 0.0.25), python3-chewie (<< 0.0.26),
          python3-pytricia (>= 1.0.0),
          python3:any (>= 3.8~),
          ${misc:Depends},
 Suggests: python-faucet-doc, faucet, gauge
```

### Comparing `c65faucet-1.0.56/debian/copyright` & `c65faucet-1.0.57/debian/copyright`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/debian/faucet.postinst` & `c65faucet-1.0.57/debian/faucet.postinst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/debian/gauge.postinst` & `c65faucet-1.0.57/debian/gauge.postinst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/debian/rules` & `c65faucet-1.0.57/debian/rules`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docker/fuzz_config.sh` & `c65faucet-1.0.57/docker/fuzz_config.sh`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docker/fuzz_packet.sh` & `c65faucet-1.0.57/docker/fuzz_packet.sh`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docker/install-faucet.sh` & `c65faucet-1.0.57/docker/install-faucet.sh`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docker/localtest.sh` & `c65faucet-1.0.57/docker/localtest.sh`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docker/pip_deps.sh` & `c65faucet-1.0.57/docker/pip_deps.sh`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docker/runtests.sh` & `c65faucet-1.0.57/docker/runtests.sh`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docker/shard_tests.sh` & `c65faucet-1.0.57/docker/shard_tests.sh`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docker-compose.yaml` & `c65faucet-1.0.57/docker-compose.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             - './etc/prometheus/faucet.rules.yml:/etc/prometheus/faucet.rules.yml'
         links:
             - faucet
             - gauge
 
     grafana:
         restart: always
-        image: 'grafana/grafana:9.5.2'
+        image: 'grafana/grafana:9.5.3'
         user: 'root'
         ports:
             - '3000:3000'
         volumes:
             - '${FAUCET_PREFIX}/opt/grafana:/var/lib/grafana'
         links:
             - influxdb
```

### Comparing `c65faucet-1.0.56/docs/Makefile` & `c65faucet-1.0.57/docs/Makefile`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/deployments/ONF_Faucet_deploy1.png` & `c65faucet-1.0.57/docs/_static/deployments/ONF_Faucet_deploy1.png`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/deployments/nznog17-physical-network.jpg` & `c65faucet-1.0.57/docs/_static/deployments/nznog17-physical-network.jpg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/deployments/nznog17-virtual-network.jpg` & `c65faucet-1.0.57/docs/_static/deployments/nznog17-virtual-network.jpg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/grafana-dashboards/faucet_instrumentation.json` & `c65faucet-1.0.57/docs/_static/grafana-dashboards/faucet_instrumentation.json`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/grafana-dashboards/faucet_inventory.json` & `c65faucet-1.0.57/docs/_static/grafana-dashboards/faucet_inventory.json`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/grafana-dashboards/faucet_port_statistics.json` & `c65faucet-1.0.57/docs/_static/grafana-dashboards/faucet_port_statistics.json`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/images/8021X-conf-diagram.svg` & `c65faucet-1.0.57/docs/_static/images/8021X-conf-diagram.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/images/faucet-architecture.svg` & `c65faucet-1.0.57/docs/_static/images/faucet-architecture.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/images/faucet-pipeline.png` & `c65faucet-1.0.57/docs/_static/images/faucet-pipeline.png`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/images/faucet-pipeline.svg` & `c65faucet-1.0.57/docs/_static/images/faucet-pipeline.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/images/faucet-pipeline.txt` & `c65faucet-1.0.57/docs/_static/images/faucet-pipeline.txt`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/images/gauge-nznog17.png` & `c65faucet-1.0.57/docs/_static/images/gauge-nznog17.png`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/images/gauge-snapshot1.png` & `c65faucet-1.0.57/docs/_static/images/gauge-snapshot1.png`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/images/gauge-snapshot2.png` & `c65faucet-1.0.57/docs/_static/images/gauge-snapshot2.png`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/images/gauge-snapshot3.png` & `c65faucet-1.0.57/docs/_static/images/gauge-snapshot3.png`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/images/tutorial-acls.svg` & `c65faucet-1.0.57/docs/_static/images/tutorial-acls.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/images/tutorial-bgp-routing.svg` & `c65faucet-1.0.57/docs/_static/images/tutorial-bgp-routing.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/images/tutorial-ivr.svg` & `c65faucet-1.0.57/docs/_static/images/tutorial-ivr.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/images/tutorial-multi-root-stack.svg` & `c65faucet-1.0.57/docs/_static/images/tutorial-multi-root-stack.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/images/tutorial-nfv-services.svg` & `c65faucet-1.0.57/docs/_static/images/tutorial-nfv-services.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/images/tutorial-stack-loop.svg` & `c65faucet-1.0.57/docs/_static/images/tutorial-stack-loop.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/images/tutorial-stack-tunnel.svg` & `c65faucet-1.0.57/docs/_static/images/tutorial-stack-tunnel.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/images/tutorial-stack.svg` & `c65faucet-1.0.57/docs/_static/images/tutorial-stack.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/images/tutorial-stackwithivr.svg` & `c65faucet-1.0.57/docs/_static/images/tutorial-stackwithivr.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/images/tutorial-static-routing.svg` & `c65faucet-1.0.57/docs/_static/images/tutorial-static-routing.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/images/tutorial-vlans.svg` & `c65faucet-1.0.57/docs/_static/images/tutorial-vlans.svg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/tutorial/cleanup` & `c65faucet-1.0.57/docs/_static/tutorial/cleanup`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/_static/tutorial/inter_switch_link` & `c65faucet-1.0.57/docs/_static/tutorial/inter_switch_link`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/architecture.rst` & `c65faucet-1.0.57/docs/architecture.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/conf.py` & `c65faucet-1.0.57/docs/conf.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/configuration.rst` & `c65faucet-1.0.57/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/developer_guide.rst` & `c65faucet-1.0.57/docs/developer_guide.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/external_resources.rst` & `c65faucet-1.0.57/docs/external_resources.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/fuzzing.rst` & `c65faucet-1.0.57/docs/fuzzing.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/installation.rst` & `c65faucet-1.0.57/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/intro.rst` & `c65faucet-1.0.57/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/monitoring.rst` & `c65faucet-1.0.57/docs/monitoring.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/release_notes/1.7.0.rst` & `c65faucet-1.0.57/docs/release_notes/1.7.0.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/release_notes/1.9.0.rst` & `c65faucet-1.0.57/docs/release_notes/1.9.0.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/testing.rst` & `c65faucet-1.0.57/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/tutorials/acls.rst` & `c65faucet-1.0.57/docs/tutorials/acls.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/tutorials/conntrack.rst` & `c65faucet-1.0.57/docs/tutorials/conntrack.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/tutorials/first_time.rst` & `c65faucet-1.0.57/docs/tutorials/first_time.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/tutorials/nfv_services.rst` & `c65faucet-1.0.57/docs/tutorials/nfv_services.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/tutorials/routing.rst` & `c65faucet-1.0.57/docs/tutorials/routing.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/tutorials/stacking.rst` & `c65faucet-1.0.57/docs/tutorials/stacking.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/tutorials/vlans.rst` & `c65faucet-1.0.57/docs/tutorials/vlans.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/vendors/allied-telesis/README_Allied_Telesis.rst` & `c65faucet-1.0.57/docs/vendors/allied-telesis/README_Allied_Telesis.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/vendors/cisco/README_Cisco.rst` & `c65faucet-1.0.57/docs/vendors/cisco/README_Cisco.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/vendors/hpe/README_Aruba.rst` & `c65faucet-1.0.57/docs/vendors/hpe/README_Aruba.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/vendors/lagopus/README_Lagopus.rst` & `c65faucet-1.0.57/docs/vendors/lagopus/README_Lagopus.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/vendors/northboundnetworks/README_ZodiacFX.rst` & `c65faucet-1.0.57/docs/vendors/northboundnetworks/README_ZodiacFX.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/vendors/northboundnetworks/README_ZodiacGX.rst` & `c65faucet-1.0.57/docs/vendors/northboundnetworks/README_ZodiacGX.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/vendors/northboundnetworks/conf-zodiac.sh` & `c65faucet-1.0.57/docs/vendors/northboundnetworks/conf-zodiac.sh`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/vendors/noviflow/README_noviflow.rst` & `c65faucet-1.0.57/docs/vendors/noviflow/README_noviflow.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/vendors/ovs/README_OVS-DPDK.rst` & `c65faucet-1.0.57/docs/vendors/ovs/README_OVS-DPDK.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/vendors/ovs/faucet_ovs_test.png` & `c65faucet-1.0.57/docs/vendors/ovs/faucet_ovs_test.png`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/docs/vendors/ovs/faucet_testing_with_OVS_on_hardware.rst` & `c65faucet-1.0.57/docs/vendors/ovs/faucet_testing_with_OVS_on_hardware.rst`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/etc/faucet/acls.yaml` & `c65faucet-1.0.57/etc/faucet/acls.yaml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/etc/faucet/faucet.yaml` & `c65faucet-1.0.57/etc/faucet/faucet.yaml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/etc/faucet/gauge.yaml` & `c65faucet-1.0.57/etc/faucet/gauge.yaml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/etc/prometheus/faucet.rules.yml` & `c65faucet-1.0.57/etc/prometheus/faucet.rules.yml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/etc/prometheus/prometheus.yml` & `c65faucet-1.0.57/etc/prometheus/prometheus.yml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/__main__.py` & `c65faucet-1.0.57/faucet/__main__.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/acl.py` & `c65faucet-1.0.57/faucet/acl.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/check_faucet_config.py` & `c65faucet-1.0.57/faucet/check_faucet_config.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/conf.py` & `c65faucet-1.0.57/faucet/conf.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/config_parser.py` & `c65faucet-1.0.57/faucet/config_parser.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/config_parser_util.py` & `c65faucet-1.0.57/faucet/config_parser_util.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/dp.py` & `c65faucet-1.0.57/faucet/dp.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/faucet.py` & `c65faucet-1.0.57/faucet/faucet.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/faucet_bgp.py` & `c65faucet-1.0.57/faucet/faucet_bgp.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/faucet_dot1x.py` & `c65faucet-1.0.57/faucet/faucet_dot1x.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/faucet_event.py` & `c65faucet-1.0.57/faucet/faucet_event.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/faucet_metrics.py` & `c65faucet-1.0.57/faucet/faucet_metrics.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/faucet_pipeline.py` & `c65faucet-1.0.57/faucet/faucet_pipeline.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/fctl.py` & `c65faucet-1.0.57/faucet/fctl.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/gauge.py` & `c65faucet-1.0.57/faucet/gauge.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/gauge_influx.py` & `c65faucet-1.0.57/faucet/gauge_influx.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/gauge_pollers.py` & `c65faucet-1.0.57/faucet/gauge_pollers.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/gauge_prom.py` & `c65faucet-1.0.57/faucet/gauge_prom.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/meter.py` & `c65faucet-1.0.57/faucet/meter.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/port.py` & `c65faucet-1.0.57/faucet/port.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/prom_client.py` & `c65faucet-1.0.57/faucet/prom_client.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/router.py` & `c65faucet-1.0.57/faucet/router.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/stack.py` & `c65faucet-1.0.57/faucet/stack.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/tfm_pipeline.py` & `c65faucet-1.0.57/faucet/tfm_pipeline.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/valve.py` & `c65faucet-1.0.57/faucet/valve.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/valve_acl.py` & `c65faucet-1.0.57/faucet/valve_acl.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/valve_coprocessor.py` & `c65faucet-1.0.57/faucet/valve_coprocessor.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/valve_lldp.py` & `c65faucet-1.0.57/faucet/valve_lldp.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/valve_manager_base.py` & `c65faucet-1.0.57/faucet/valve_manager_base.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/valve_of.py` & `c65faucet-1.0.57/faucet/valve_of.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/valve_of_old.py` & `c65faucet-1.0.57/faucet/valve_of_old.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/valve_outonly.py` & `c65faucet-1.0.57/faucet/valve_outonly.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/valve_packet.py` & `c65faucet-1.0.57/faucet/valve_packet.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/valve_pipeline.py` & `c65faucet-1.0.57/faucet/valve_pipeline.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/valve_route.py` & `c65faucet-1.0.57/faucet/valve_route.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/valve_ryuapp.py` & `c65faucet-1.0.57/faucet/valve_ryuapp.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/valve_stack.py` & `c65faucet-1.0.57/faucet/valve_stack.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/valve_switch.py` & `c65faucet-1.0.57/faucet/valve_switch.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/valve_switch_stack.py` & `c65faucet-1.0.57/faucet/valve_switch_stack.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/valve_switch_standalone.py` & `c65faucet-1.0.57/faucet/valve_switch_standalone.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/valve_table.py` & `c65faucet-1.0.57/faucet/valve_table.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/valve_util.py` & `c65faucet-1.0.57/faucet/valve_util.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/valves_manager.py` & `c65faucet-1.0.57/faucet/valves_manager.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/vlan.py` & `c65faucet-1.0.57/faucet/vlan.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/watcher.py` & `c65faucet-1.0.57/faucet/watcher.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/faucet/watcher_conf.py` & `c65faucet-1.0.57/faucet/watcher_conf.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/hw_switch_config.yaml` & `c65faucet-1.0.57/hw_switch_config.yaml`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/ofctl_rest/ofctl_rest.py` & `c65faucet-1.0.57/ofctl_rest/ofctl_rest.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/ofctl_rest/wsgi.py` & `c65faucet-1.0.57/ofctl_rest/wsgi.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/setup.cfg` & `c65faucet-1.0.57/setup.cfg`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/setup.py` & `c65faucet-1.0.57/setup.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/codecheck/src_files.sh` & `c65faucet-1.0.57/tests/codecheck/src_files.sh`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/generative/fuzzer/config/fuzz_config.py` & `c65faucet-1.0.57/tests/generative/fuzzer/config/fuzz_config.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/generative/fuzzer/config/generate_dict.py` & `c65faucet-1.0.57/tests/generative/fuzzer/config/generate_dict.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/generative/fuzzer/packet/display_packet_crash.py` & `c65faucet-1.0.57/tests/generative/fuzzer/packet/display_packet_crash.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/http.ex2` & `c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/http.ex2`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/icmp.ex1` & `c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/icmp.ex1`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/icmp.ex2` & `c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/icmp.ex2`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/ipv4.ex1` & `c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/ipv4.ex1`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/generative/fuzzer/packet/examples/msger.ex1` & `c65faucet-1.0.57/tests/generative/fuzzer/packet/examples/msger.ex1`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/generative/fuzzer/packet/fake_packet.py` & `c65faucet-1.0.57/tests/generative/fuzzer/packet/fake_packet.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/generative/fuzzer/packet/fuzz_packet.py` & `c65faucet-1.0.57/tests/generative/fuzzer/packet/fuzz_packet.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/generative/integration/fault_tolerance_main.py` & `c65faucet-1.0.57/tests/generative/integration/fault_tolerance_main.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/generative/integration/fault_tolerance_tests.py` & `c65faucet-1.0.57/tests/generative/integration/fault_tolerance_tests.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/generative/unit/test_topology.py` & `c65faucet-1.0.57/tests/generative/unit/test_topology.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/integration/mininet_main.py` & `c65faucet-1.0.57/tests/integration/mininet_main.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/integration/mininet_multidp_tests.py` & `c65faucet-1.0.57/tests/integration/mininet_multidp_tests.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/integration/mininet_tests.py` & `c65faucet-1.0.57/tests/integration/mininet_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -670,23 +670,18 @@
                 default_config = re.sub(listen_match, "", default_config)
                 default_site.seek(0)
                 default_site.write(default_config)
                 default_site.write(listen_config)
                 default_site.truncate()
         else:
             # Assume we are dealing with freeradius >=3 configuration
-            freerad_version = (
-                os.popen(r'freeradius -v | egrep -o -m 1 "Version ([0-9]\.[0.9])"')
-                .read()
-                .rstrip()
-            )
-            freerad_major_version = freerad_version.split(" ")[1]
             shutil.copytree(
-                "/etc/freeradius/%s/" % freerad_major_version,
+                "/etc/freeradius/3.0/",
                 "%s/freeradius" % self.tmpdir,
+                symlinks=True,
             )
             users_path = "%s/freeradius/mods-config/files/authorize" % self.tmpdir
 
             with open(
                 "%s/freeradius/sites-enabled/default" % self.tmpdir,
                 "r+",
                 encoding="utf-8",
```

### Comparing `c65faucet-1.0.56/tests/run_unit_tests.sh` & `c65faucet-1.0.57/tests/run_unit_tests.sh`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/unit/clib/test_topo.py` & `c65faucet-1.0.57/tests/unit/clib/test_topo.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/unit/faucet/test_check_config.py` & `c65faucet-1.0.57/tests/unit/faucet/test_check_config.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/unit/faucet/test_config.py` & `c65faucet-1.0.57/tests/unit/faucet/test_config.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/unit/faucet/test_fctl.py` & `c65faucet-1.0.57/tests/unit/faucet/test_fctl.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/unit/faucet/test_main.py` & `c65faucet-1.0.57/tests/unit/faucet/test_main.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/unit/faucet/test_port.py` & `c65faucet-1.0.57/tests/unit/faucet/test_port.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/unit/faucet/test_valve.py` & `c65faucet-1.0.57/tests/unit/faucet/test_valve.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/unit/faucet/test_valve_config.py` & `c65faucet-1.0.57/tests/unit/faucet/test_valve_config.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/unit/faucet/test_valve_dot1x.py` & `c65faucet-1.0.57/tests/unit/faucet/test_valve_dot1x.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/unit/faucet/test_valve_egress.py` & `c65faucet-1.0.57/tests/unit/faucet/test_valve_egress.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/unit/faucet/test_valve_of.py` & `c65faucet-1.0.57/tests/unit/faucet/test_valve_of.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/unit/faucet/test_valve_stack.py` & `c65faucet-1.0.57/tests/unit/faucet/test_valve_stack.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/unit/faucet/test_valveapp_smoke.py` & `c65faucet-1.0.57/tests/unit/faucet/test_valveapp_smoke.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/unit/faucet/test_vlan.py` & `c65faucet-1.0.57/tests/unit/faucet/test_vlan.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/unit/gauge/test_config_gauge.py` & `c65faucet-1.0.57/tests/unit/gauge/test_config_gauge.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/unit/gauge/test_gauge.py` & `c65faucet-1.0.57/tests/unit/gauge/test_gauge.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/unit/gauge/test_main.py` & `c65faucet-1.0.57/tests/unit/gauge/test_main.py`

 * *Files identical despite different names*

### Comparing `c65faucet-1.0.56/tests/unit/packaging/test_packaging.py` & `c65faucet-1.0.57/tests/unit/packaging/test_packaging.py`

 * *Files identical despite different names*

