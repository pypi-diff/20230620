# Comparing `tmp/domain-admin-1.4.1.tar.gz` & `tmp/domain-admin-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domain-admin-1.4.1.tar", last modified: Tue Jun 20 02:46:01 2023, max compression
+gzip compressed data, was "domain-admin-1.4.2.tar", last modified: Tue Jun 20 02:57:00 2023, max compression
```

## Comparing `domain-admin-1.4.1.tar` & `domain-admin-1.4.2.tar`

### file list

```diff
@@ -1,263 +1,263 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.032127 domain-admin-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-20 02:45:49.000000 domain-admin-1.4.1/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-06-20 02:45:49.000000 domain-admin-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-06-20 02:46:01.032127 domain-admin-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-06-20 02:45:49.000000 domain-admin-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.008127 domain-admin-1.4.1/domain_admin/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.008127 domain-admin-1.4.1/domain_admin/api/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/api/address_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/api/cert_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/api/domain_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/api/domain_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/api/group_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/api/ip_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/api/log_scheduler_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/api/notify_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/api/system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/api/whois_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.008127 domain-admin-1.4.1/domain_admin/config/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/config/default_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/config/env_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.008127 domain-admin-1.4.1/domain_admin/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/enums/config_key_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/enums/event_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/enums/notify_type_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/enums/status_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/enums/version_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.012127 domain-admin-1.4.1/domain_admin/migrate/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/migrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/migrate/migrate_102_to_103.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/migrate/migrate_106_to_110.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/migrate/migrate_110_to_1212.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/migrate/migrate_1212_to_1213.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/migrate/migrate_1213_to_131.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/migrate/migrate_136_to_140_alpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/migrate/migrate_140_alpha_to_140.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/migrate/migrate_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.012127 domain-admin-1.4.1/domain_admin/model/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/model/address_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/model/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/model/cache_domain_info_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/model/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/model/domain_info_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/model/domain_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/model/group_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/model/log_scheduler_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/model/notify_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/model/system_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/model/user_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/model/version_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.012127 domain-admin-1.4.1/domain_admin/public/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.012127 domain-admin-1.4.1/domain_admin/public/.git/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/FETCH_HEAD
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/HEAD
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/config
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-06-20 02:45:58.000000 domain-admin-1.4.1/domain_admin/public/.git/description
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-06-20 02:45:58.000000 domain-admin-1.4.1/domain_admin/public/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-06-20 02:45:58.000000 domain-admin-1.4.1/domain_admin/public/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-06-20 02:45:58.000000 domain-admin-1.4.1/domain_admin/public/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-06-20 02:45:58.000000 domain-admin-1.4.1/domain_admin/public/.git/hooks/post-update.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-06-20 02:45:58.000000 domain-admin-1.4.1/domain_admin/public/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-06-20 02:45:58.000000 domain-admin-1.4.1/domain_admin/public/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-06-20 02:45:58.000000 domain-admin-1.4.1/domain_admin/public/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-06-20 02:45:58.000000 domain-admin-1.4.1/domain_admin/public/.git/hooks/pre-push.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-06-20 02:45:58.000000 domain-admin-1.4.1/domain_admin/public/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-06-20 02:45:58.000000 domain-admin-1.4.1/domain_admin/public/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-06-20 02:45:58.000000 domain-admin-1.4.1/domain_admin/public/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-06-20 02:45:58.000000 domain-admin-1.4.1/domain_admin/public/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-06-20 02:45:58.000000 domain-admin-1.4.1/domain_admin/public/.git/hooks/update.sample
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/index
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/info/
--rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-06-20 02:45:58.000000 domain-admin-1.4.1/domain_admin/public/.git/info/exclude
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/logs/HEAD
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.004127 domain-admin-1.4.1/domain_admin/public/.git/logs/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/logs/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/logs/refs/heads/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.004127 domain-admin-1.4.1/domain_admin/public/.git/logs/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/logs/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/logs/refs/remotes/origin/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.004127 domain-admin-1.4.1/domain_admin/public/.git/objects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/objects/1c/
--r--r--r--   0 runner    (1001) docker     (123)      175 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/1c/f3da1e24b61c3c2c098a44ee5104015360b15b
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/objects/1d/
--r--r--r--   0 runner    (1001) docker     (123)    10075 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/1d/5380125d8b56c0426f9651cb8fb148b47a4c27
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/objects/20/
--r--r--r--   0 runner    (1001) docker     (123)      151 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/20/ac4f105a4a0c8be8e9f4e00e224cad538ad2e8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/objects/21/
--r--r--r--   0 runner    (1001) docker     (123)       61 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/21/00bd7d2219a26827cc80aa37fe72fcb303bb50
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/objects/39/
--r--r--r--   0 runner    (1001) docker     (123)    63323 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/39/f04d3540ee3fad6d43a9831763d9eba45d0573
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/objects/3c/
--r--r--r--   0 runner    (1001) docker     (123)     3081 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/objects/40/
--r--r--r--   0 runner    (1001) docker     (123)      229 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/40/60293e2ea143c10233675d3b2a12c7df256566
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/objects/49/
--r--r--r--   0 runner    (1001) docker     (123)      662 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/49/9cb6596b56d599852473fb85c29c53040e2f78
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/objects/4c/
--r--r--r--   0 runner    (1001) docker     (123)      462 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/4c/f467f38c990e812a5d7ecdca9745a8babd037f
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/objects/50/
--r--r--r--   0 runner    (1001) docker     (123)     1428 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/50/0fd27e2e6061799cce3e7e6ed602915082a659
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/objects/57/
--r--r--r--   0 runner    (1001) docker     (123)       70 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/57/55d0c159b607a0a5978e25659b818536dd0a76
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/objects/5b/
--r--r--r--   0 runner    (1001) docker     (123)    62564 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/5b/1c488a74d8c3493cec2a99903972521902b410
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/objects/5f/
--r--r--r--   0 runner    (1001) docker     (123)      530 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/objects/61/
--r--r--r--   0 runner    (1001) docker     (123)      222 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/61/e848827cf28154fabcfa3f31472b070c9329b0
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/objects/6a/
--r--r--r--   0 runner    (1001) docker     (123)      475 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/6a/55c88c046e7a748569f99f406ff272d2bf51cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/objects/6d/
--r--r--r--   0 runner    (1001) docker     (123)      612 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/objects/74/
--r--r--r--   0 runner    (1001) docker     (123)     6220 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/74/38a8b40596320051c82f62e00d1906c2d755d8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/objects/7a/
--r--r--r--   0 runner    (1001) docker     (123)   279768 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/7a/b699b6eea6b7e3d3c0130b97bdca0def787fef
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/objects/81/
--r--r--r--   0 runner    (1001) docker     (123)      640 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/81/51e81a1838d6c47c21cdefbf26ecc9f5755db6
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/objects/8b/
--r--r--r--   0 runner    (1001) docker     (123)    41901 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/8b/19737c31c38191351e2550ceba02f876fb253a
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/objects/93/
--r--r--r--   0 runner    (1001) docker     (123)     4057 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/93/01be1310745fa1bd0a1929236eeaf354873706
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/objects/95/
--r--r--r--   0 runner    (1001) docker     (123)     1738 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/95/c5323cc849308100d0409fdf506006828df9eb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/objects/a2/
--r--r--r--   0 runner    (1001) docker     (123)    77211 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/a2/709cde362f916eadaacfc27c47d0220dd4705c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.016127 domain-admin-1.4.1/domain_admin/public/.git/objects/a5/
--r--r--r--   0 runner    (1001) docker     (123)     3174 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/a5/4d5e8c9407e7b569a1a8a7e3436fdcc7cffec3
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.020127 domain-admin-1.4.1/domain_admin/public/.git/objects/ac/
--r--r--r--   0 runner    (1001) docker     (123)     8218 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/ac/b525d308d4833452f2159639607c0e10ac52e7
--r--r--r--   0 runner    (1001) docker     (123)     8018 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/ac/be31715261348534f51c95789f87d880bd018a
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.020127 domain-admin-1.4.1/domain_admin/public/.git/objects/b1/
--r--r--r--   0 runner    (1001) docker     (123)     4499 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/b1/c8fbd3728133a504f21a506ab5dff37409451f
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.020127 domain-admin-1.4.1/domain_admin/public/.git/objects/bb/
--r--r--r--   0 runner    (1001) docker     (123)     1026 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/objects/bb/9a94723f92fe51c9842c5c6baf60f9ca2b2e36
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.004127 domain-admin-1.4.1/domain_admin/public/.git/refs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.020127 domain-admin-1.4.1/domain_admin/public/.git/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/refs/heads/dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.004127 domain-admin-1.4.1/domain_admin/public/.git/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.020127 domain-admin-1.4.1/domain_admin/public/.git/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/.git/refs/remotes/origin/dist
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-20 02:45:58.000000 domain-admin-1.4.1/domain_admin/public/.git/shallow
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.020127 domain-admin-1.4.1/domain_admin/public/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/css/ConditionFilterGroup.a91875e6.css
--rw-r--r--   0 runner    (1001) docker     (123)   328824 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/css/index.483612c5.css
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/css/index.f0377688.css
--rwxr-xr-x   0 runner    (1001) docker     (123)    15406 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.024127 domain-admin-1.4.1/domain_admin/public/js/
--rw-r--r--   0 runner    (1001) docker     (123)    21298 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/js/ConditionFilterGroup.bbd10def.js
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/js/ConnectStatus.3d8a0270.js
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/js/SelectGroup.0f7c084d.js
--rw-r--r--   0 runner    (1001) docker     (123)   195335 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/js/element-icon.ade3aa7e.js
--rw-r--r--   0 runner    (1001) docker     (123)   749550 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/js/element-plus.dcbfaaa8.js
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/js/index.050f1ae2.js
--rw-r--r--   0 runner    (1001) docker     (123)    27059 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/js/index.2d4c528a.js
--rw-r--r--   0 runner    (1001) docker     (123)   239631 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/js/index.3c22ca57.js
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/js/index.83d13e8b.js
--rw-r--r--   0 runner    (1001) docker     (123)    14298 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/js/index.888df730.js
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/js/index.bf2c4fd4.js
--rw-r--r--   0 runner    (1001) docker     (123)    26679 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/js/index.bff8f0b2.js
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/js/index.c44ca8f1.js
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/js/index.cfa94de3.js
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/js/validator.0c34c3e7.js
--rw-r--r--   0 runner    (1001) docker     (123)    23389 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/js/vendor-lib.4c56f242.js
--rw-r--r--   0 runner    (1001) docker     (123)    94202 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/js/vendor-vue.edbe275b.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.024127 domain-admin-1.4.1/domain_admin/public/svg/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-20 02:45:59.000000 domain-admin-1.4.1/domain_admin/public/svg/logo.184a2d7d.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.024127 domain-admin-1.4.1/domain_admin/router/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/router/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/router/api_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/router/permission.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.028127 domain-admin-1.4.1/domain_admin/service/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/service/async_task_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/service/auth_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/service/cache_domain_info_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/service/domain_info_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/service/domain_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/service/email_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/service/file_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/service/global_data_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/service/group_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/service/notify_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/service/render_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/service/scheduler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/service/system_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/service/token_service.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/service/user_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/service/version_service.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/service/work_weixin_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.028127 domain-admin-1.4.1/domain_admin/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/templates/cert-email.html
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/templates/cert-export.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/templates/domain-email.html
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/templates/domain-export.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.028127 domain-admin-1.4.1/domain_admin/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/bcrypt_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.028127 domain-admin-1.4.1/domain_admin/utils/cert_util/
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/cert_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/cert_util/cert_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/cert_util/cert_consts.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/cert_util/cert_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/cert_util/cert_openssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/cert_util/cert_openssl_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/cert_util/cert_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/cert_util/cert_socket_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/datetime_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/domain_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/email_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/file_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.028127 domain-admin-1.4.1/domain_admin/utils/flask_ext/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/flask_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/flask_ext/api_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/flask_ext/app_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/flask_ext/flask_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/flask_ext/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/flask_ext/http_code_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.032127 domain-admin-1.4.1/domain_admin/utils/flask_ext/json/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/flask_ext/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/flask_ext/json/default.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/flask_ext/json/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/flask_ext/json/json_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/flask_ext/register.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/flask_ext/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/ip_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/json_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.032127 domain-admin-1.4.1/domain_admin/utils/peewee_ext/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/peewee_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/peewee_ext/model_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/secret_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/text_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/time_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.032127 domain-admin-1.4.1/domain_admin/utils/whois_util/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/whois_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/whois_util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/whois_util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    25896 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/whois_util/whois-servers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/whois_util/whois_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/utils/work_weixin_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       60 2023-06-20 02:45:49.000000 domain-admin-1.4.1/domain_admin/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.008127 domain-admin-1.4.1/domain_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-06-20 02:46:00.000000 domain-admin-1.4.1/domain_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-06-20 02:46:00.000000 domain-admin-1.4.1/domain_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 02:46:00.000000 domain-admin-1.4.1/domain_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-20 02:46:00.000000 domain-admin-1.4.1/domain_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 02:46:00.000000 domain-admin-1.4.1/domain_admin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 02:46:00.000000 domain-admin-1.4.1/domain_admin.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:46:01.032127 domain-admin-1.4.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-20 02:45:49.000000 domain-admin-1.4.1/requirements/production.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 02:46:01.032127 domain-admin-1.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1928 2023-06-20 02:45:49.000000 domain-admin-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.406464 domain-admin-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-20 02:56:44.000000 domain-admin-1.4.2/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      417 2023-06-20 02:56:44.000000 domain-admin-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-06-20 02:57:00.406464 domain-admin-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-06-20 02:56:44.000000 domain-admin-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.382464 domain-admin-1.4.2/domain_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.386464 domain-admin-1.4.2/domain_admin/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/api/address_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/api/cert_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14230 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/api/domain_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/api/domain_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/api/group_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/api/ip_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/api/log_scheduler_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/api/notify_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/api/system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/api/whois_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.386464 domain-admin-1.4.2/domain_admin/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/config/default_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/config/env_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.386464 domain-admin-1.4.2/domain_admin/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/enums/config_key_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/enums/event_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/enums/notify_type_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/enums/status_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/enums/version_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.386464 domain-admin-1.4.2/domain_admin/migrate/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/migrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/migrate/migrate_102_to_103.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/migrate/migrate_106_to_110.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/migrate/migrate_110_to_1212.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/migrate/migrate_1212_to_1213.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/migrate/migrate_1213_to_131.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/migrate/migrate_136_to_140_alpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/migrate/migrate_140_alpha_to_140.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/migrate/migrate_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.386464 domain-admin-1.4.2/domain_admin/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/model/address_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/model/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/model/cache_domain_info_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/model/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/model/domain_info_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/model/domain_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/model/group_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/model/log_scheduler_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/model/notify_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/model/system_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/model/user_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/model/version_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.386464 domain-admin-1.4.2/domain_admin/public/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.390464 domain-admin-1.4.2/domain_admin/public/.git/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/FETCH_HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/config
+-rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/description
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.390464 domain-admin-1.4.2/domain_admin/public/.git/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      478 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4726 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/hooks/post-update.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1643 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      416 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1374 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4898 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2783 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/hooks/update.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.390464 domain-admin-1.4.2/domain_admin/public/.git/info/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/info/exclude
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.390464 domain-admin-1.4.2/domain_admin/public/.git/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/logs/HEAD
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.378464 domain-admin-1.4.2/domain_admin/public/.git/logs/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.390464 domain-admin-1.4.2/domain_admin/public/.git/logs/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/logs/refs/heads/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.378464 domain-admin-1.4.2/domain_admin/public/.git/logs/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.390464 domain-admin-1.4.2/domain_admin/public/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/logs/refs/remotes/origin/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.382464 domain-admin-1.4.2/domain_admin/public/.git/objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.390464 domain-admin-1.4.2/domain_admin/public/.git/objects/1c/
+-r--r--r--   0 runner    (1001) docker     (123)      175 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/1c/f3da1e24b61c3c2c098a44ee5104015360b15b
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.390464 domain-admin-1.4.2/domain_admin/public/.git/objects/1d/
+-r--r--r--   0 runner    (1001) docker     (123)    10075 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/1d/5380125d8b56c0426f9651cb8fb148b47a4c27
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.390464 domain-admin-1.4.2/domain_admin/public/.git/objects/20/
+-r--r--r--   0 runner    (1001) docker     (123)      151 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/20/ac4f105a4a0c8be8e9f4e00e224cad538ad2e8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.390464 domain-admin-1.4.2/domain_admin/public/.git/objects/21/
+-r--r--r--   0 runner    (1001) docker     (123)       61 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/21/00bd7d2219a26827cc80aa37fe72fcb303bb50
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.390464 domain-admin-1.4.2/domain_admin/public/.git/objects/39/
+-r--r--r--   0 runner    (1001) docker     (123)    63323 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/39/f04d3540ee3fad6d43a9831763d9eba45d0573
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.390464 domain-admin-1.4.2/domain_admin/public/.git/objects/3c/
+-r--r--r--   0 runner    (1001) docker     (123)     3081 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.390464 domain-admin-1.4.2/domain_admin/public/.git/objects/40/
+-r--r--r--   0 runner    (1001) docker     (123)      229 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/40/60293e2ea143c10233675d3b2a12c7df256566
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.390464 domain-admin-1.4.2/domain_admin/public/.git/objects/49/
+-r--r--r--   0 runner    (1001) docker     (123)      662 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/49/9cb6596b56d599852473fb85c29c53040e2f78
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.390464 domain-admin-1.4.2/domain_admin/public/.git/objects/4c/
+-r--r--r--   0 runner    (1001) docker     (123)      462 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/4c/f467f38c990e812a5d7ecdca9745a8babd037f
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.390464 domain-admin-1.4.2/domain_admin/public/.git/objects/50/
+-r--r--r--   0 runner    (1001) docker     (123)     1428 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/50/0fd27e2e6061799cce3e7e6ed602915082a659
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.390464 domain-admin-1.4.2/domain_admin/public/.git/objects/57/
+-r--r--r--   0 runner    (1001) docker     (123)       70 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/57/55d0c159b607a0a5978e25659b818536dd0a76
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.390464 domain-admin-1.4.2/domain_admin/public/.git/objects/5b/
+-r--r--r--   0 runner    (1001) docker     (123)    62564 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/5b/1c488a74d8c3493cec2a99903972521902b410
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.390464 domain-admin-1.4.2/domain_admin/public/.git/objects/5f/
+-r--r--r--   0 runner    (1001) docker     (123)      530 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.390464 domain-admin-1.4.2/domain_admin/public/.git/objects/61/
+-r--r--r--   0 runner    (1001) docker     (123)      222 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/61/e848827cf28154fabcfa3f31472b070c9329b0
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.390464 domain-admin-1.4.2/domain_admin/public/.git/objects/6a/
+-r--r--r--   0 runner    (1001) docker     (123)      475 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/6a/55c88c046e7a748569f99f406ff272d2bf51cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.390464 domain-admin-1.4.2/domain_admin/public/.git/objects/6d/
+-r--r--r--   0 runner    (1001) docker     (123)      612 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.390464 domain-admin-1.4.2/domain_admin/public/.git/objects/74/
+-r--r--r--   0 runner    (1001) docker     (123)     6220 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/74/38a8b40596320051c82f62e00d1906c2d755d8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.390464 domain-admin-1.4.2/domain_admin/public/.git/objects/7a/
+-r--r--r--   0 runner    (1001) docker     (123)   279768 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/7a/b699b6eea6b7e3d3c0130b97bdca0def787fef
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.394464 domain-admin-1.4.2/domain_admin/public/.git/objects/81/
+-r--r--r--   0 runner    (1001) docker     (123)      640 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/81/51e81a1838d6c47c21cdefbf26ecc9f5755db6
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.394464 domain-admin-1.4.2/domain_admin/public/.git/objects/8b/
+-r--r--r--   0 runner    (1001) docker     (123)    41901 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/8b/19737c31c38191351e2550ceba02f876fb253a
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.394464 domain-admin-1.4.2/domain_admin/public/.git/objects/93/
+-r--r--r--   0 runner    (1001) docker     (123)     4057 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/93/01be1310745fa1bd0a1929236eeaf354873706
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.394464 domain-admin-1.4.2/domain_admin/public/.git/objects/95/
+-r--r--r--   0 runner    (1001) docker     (123)     1738 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/95/c5323cc849308100d0409fdf506006828df9eb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.394464 domain-admin-1.4.2/domain_admin/public/.git/objects/a2/
+-r--r--r--   0 runner    (1001) docker     (123)    77211 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/a2/709cde362f916eadaacfc27c47d0220dd4705c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.394464 domain-admin-1.4.2/domain_admin/public/.git/objects/a5/
+-r--r--r--   0 runner    (1001) docker     (123)     3174 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/a5/4d5e8c9407e7b569a1a8a7e3436fdcc7cffec3
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.394464 domain-admin-1.4.2/domain_admin/public/.git/objects/ac/
+-r--r--r--   0 runner    (1001) docker     (123)     8218 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/ac/b525d308d4833452f2159639607c0e10ac52e7
+-r--r--r--   0 runner    (1001) docker     (123)     8018 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/ac/be31715261348534f51c95789f87d880bd018a
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.394464 domain-admin-1.4.2/domain_admin/public/.git/objects/b1/
+-r--r--r--   0 runner    (1001) docker     (123)     4499 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/b1/c8fbd3728133a504f21a506ab5dff37409451f
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.394464 domain-admin-1.4.2/domain_admin/public/.git/objects/bb/
+-r--r--r--   0 runner    (1001) docker     (123)     1026 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/objects/bb/9a94723f92fe51c9842c5c6baf60f9ca2b2e36
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.382464 domain-admin-1.4.2/domain_admin/public/.git/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.394464 domain-admin-1.4.2/domain_admin/public/.git/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/refs/heads/dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.382464 domain-admin-1.4.2/domain_admin/public/.git/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.394464 domain-admin-1.4.2/domain_admin/public/.git/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/.git/refs/remotes/origin/dist
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-20 02:56:57.000000 domain-admin-1.4.2/domain_admin/public/.git/shallow
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.394464 domain-admin-1.4.2/domain_admin/public/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/css/ConditionFilterGroup.a91875e6.css
+-rw-r--r--   0 runner    (1001) docker     (123)   328824 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/css/index.483612c5.css
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/css/index.f0377688.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15406 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.398464 domain-admin-1.4.2/domain_admin/public/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    21298 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/js/ConditionFilterGroup.bbd10def.js
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/js/ConnectStatus.3d8a0270.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/js/SelectGroup.0f7c084d.js
+-rw-r--r--   0 runner    (1001) docker     (123)   195335 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/js/element-icon.ade3aa7e.js
+-rw-r--r--   0 runner    (1001) docker     (123)   749550 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/js/element-plus.dcbfaaa8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/js/index.050f1ae2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27059 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/js/index.2d4c528a.js
+-rw-r--r--   0 runner    (1001) docker     (123)   239631 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/js/index.3c22ca57.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/js/index.83d13e8b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14298 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/js/index.888df730.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/js/index.bf2c4fd4.js
+-rw-r--r--   0 runner    (1001) docker     (123)    26679 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/js/index.bff8f0b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/js/index.c44ca8f1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/js/index.cfa94de3.js
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/js/validator.0c34c3e7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23389 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/js/vendor-lib.4c56f242.js
+-rw-r--r--   0 runner    (1001) docker     (123)    94202 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/js/vendor-vue.edbe275b.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.398464 domain-admin-1.4.2/domain_admin/public/svg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-20 02:56:58.000000 domain-admin-1.4.2/domain_admin/public/svg/logo.184a2d7d.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.398464 domain-admin-1.4.2/domain_admin/router/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/router/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/router/api_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/router/permission.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.398464 domain-admin-1.4.2/domain_admin/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/service/async_task_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/service/auth_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/service/cache_domain_info_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/service/domain_info_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15506 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/service/domain_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/service/email_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/service/file_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/service/global_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/service/group_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/service/notify_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/service/render_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/service/scheduler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/service/system_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/service/token_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/service/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5049 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/service/version_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/service/work_weixin_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.402464 domain-admin-1.4.2/domain_admin/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/templates/cert-email.html
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/templates/cert-export.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/templates/domain-email.html
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/templates/domain-export.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.402464 domain-admin-1.4.2/domain_admin/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/bcrypt_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.402464 domain-admin-1.4.2/domain_admin/utils/cert_util/
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/cert_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/cert_util/cert_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/cert_util/cert_consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/cert_util/cert_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/cert_util/cert_openssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/cert_util/cert_openssl_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/cert_util/cert_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/cert_util/cert_socket_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/datetime_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/domain_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/email_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/file_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.402464 domain-admin-1.4.2/domain_admin/utils/flask_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/flask_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/flask_ext/api_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/flask_ext/app_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/flask_ext/flask_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/flask_ext/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/flask_ext/http_code_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.402464 domain-admin-1.4.2/domain_admin/utils/flask_ext/json/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/flask_ext/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/flask_ext/json/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/flask_ext/json/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/flask_ext/json/json_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/flask_ext/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/flask_ext/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/ip_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/json_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.402464 domain-admin-1.4.2/domain_admin/utils/peewee_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/peewee_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/peewee_ext/model_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/secret_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/text_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/time_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.402464 domain-admin-1.4.2/domain_admin/utils/whois_util/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/whois_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/whois_util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/whois_util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25896 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/whois_util/whois-servers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/whois_util/whois_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/utils/work_weixin_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       60 2023-06-20 02:56:44.000000 domain-admin-1.4.2/domain_admin/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.382464 domain-admin-1.4.2/domain_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11296 2023-06-20 02:57:00.000000 domain-admin-1.4.2/domain_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-06-20 02:57:00.000000 domain-admin-1.4.2/domain_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 02:57:00.000000 domain-admin-1.4.2/domain_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-20 02:57:00.000000 domain-admin-1.4.2/domain_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 02:57:00.000000 domain-admin-1.4.2/domain_admin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 02:57:00.000000 domain-admin-1.4.2/domain_admin.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 02:57:00.406464 domain-admin-1.4.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-20 02:56:44.000000 domain-admin-1.4.2/requirements/production.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 02:57:00.406464 domain-admin-1.4.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1928 2023-06-20 02:56:44.000000 domain-admin-1.4.2/setup.py
```

### Comparing `domain-admin-1.4.1/LICENSE` & `domain-admin-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/PKG-INFO` & `domain-admin-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domain-admin
-Version: 1.4.1
+Version: 1.4.2
 Summary: a domain ssl cert admin
 Home-page: https://github.com/mouday/domain-admin
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Keywords: domain ssl cert
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `domain-admin-1.4.1/README.md` & `domain-admin-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/api/address_api.py` & `domain-admin-1.4.2/domain_admin/api/address_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/api/auth_api.py` & `domain-admin-1.4.2/domain_admin/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/api/domain_api.py` & `domain-admin-1.4.2/domain_admin/api/domain_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
     current_user_id = g.user_id
 
     domain_id = request.json['id']
 
     # domain_service.check_permission_and_get_row(domain_id, current_user_id)
 
     DomainModel.delete().where(
-        DomainModel.domain_id == domain_id,
+        DomainModel.id == domain_id,
         DomainModel.user_id == current_user_id,
     ).execute()
 
     # 同时移除主机信息
     AddressModel.delete().where(
         AddressModel.domain_id == domain_id
     ).execute()
```

### Comparing `domain-admin-1.4.1/domain_admin/api/domain_info_api.py` & `domain-admin-1.4.2/domain_admin/api/domain_info_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/api/group_api.py` & `domain-admin-1.4.2/domain_admin/api/group_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/api/log_scheduler_api.py` & `domain-admin-1.4.2/domain_admin/api/log_scheduler_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/api/notify_api.py` & `domain-admin-1.4.2/domain_admin/api/notify_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/api/system_api.py` & `domain-admin-1.4.2/domain_admin/api/system_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/api/user_api.py` & `domain-admin-1.4.2/domain_admin/api/user_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/config/default_config.py` & `domain-admin-1.4.2/domain_admin/config/default_config.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/enums/config_key_enum.py` & `domain-admin-1.4.2/domain_admin/enums/config_key_enum.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/enums/version_enum.py` & `domain-admin-1.4.2/domain_admin/enums/version_enum.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/log.py` & `domain-admin-1.4.2/domain_admin/log.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/main.py` & `domain-admin-1.4.2/domain_admin/main.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/migrate/migrate_102_to_103.py` & `domain-admin-1.4.2/domain_admin/migrate/migrate_102_to_103.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/migrate/migrate_106_to_110.py` & `domain-admin-1.4.2/domain_admin/migrate/migrate_106_to_110.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/migrate/migrate_110_to_1212.py` & `domain-admin-1.4.2/domain_admin/migrate/migrate_110_to_1212.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/migrate/migrate_1212_to_1213.py` & `domain-admin-1.4.2/domain_admin/migrate/migrate_1212_to_1213.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/migrate/migrate_1213_to_131.py` & `domain-admin-1.4.2/domain_admin/migrate/migrate_1213_to_131.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/migrate/migrate_136_to_140_alpha.py` & `domain-admin-1.4.2/domain_admin/migrate/migrate_136_to_140_alpha.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/migrate/migrate_140_alpha_to_140.py` & `domain-admin-1.4.2/domain_admin/migrate/migrate_140_alpha_to_140.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/migrate/migrate_common.py` & `domain-admin-1.4.2/domain_admin/migrate/migrate_common.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/model/address_model.py` & `domain-admin-1.4.2/domain_admin/model/address_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/model/base_model.py` & `domain-admin-1.4.2/domain_admin/model/base_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/model/cache_domain_info_model.py` & `domain-admin-1.4.2/domain_admin/model/cache_domain_info_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/model/database.py` & `domain-admin-1.4.2/domain_admin/model/database.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/model/domain_info_model.py` & `domain-admin-1.4.2/domain_admin/model/domain_info_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/model/domain_model.py` & `domain-admin-1.4.2/domain_admin/model/domain_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/model/group_model.py` & `domain-admin-1.4.2/domain_admin/model/group_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/model/log_scheduler_model.py` & `domain-admin-1.4.2/domain_admin/model/log_scheduler_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/model/notify_model.py` & `domain-admin-1.4.2/domain_admin/model/notify_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/model/system_model.py` & `domain-admin-1.4.2/domain_admin/model/system_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/model/user_model.py` & `domain-admin-1.4.2/domain_admin/model/user_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/model/version_model.py` & `domain-admin-1.4.2/domain_admin/model/version_model.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/hooks/commit-msg.sample` & `domain-admin-1.4.2/domain_admin/public/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/hooks/fsmonitor-watchman.sample` & `domain-admin-1.4.2/domain_admin/public/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/hooks/pre-commit.sample` & `domain-admin-1.4.2/domain_admin/public/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/hooks/pre-push.sample` & `domain-admin-1.4.2/domain_admin/public/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/hooks/pre-rebase.sample` & `domain-admin-1.4.2/domain_admin/public/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/hooks/pre-receive.sample` & `domain-admin-1.4.2/domain_admin/public/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/hooks/prepare-commit-msg.sample` & `domain-admin-1.4.2/domain_admin/public/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/hooks/push-to-checkout.sample` & `domain-admin-1.4.2/domain_admin/public/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/hooks/update.sample` & `domain-admin-1.4.2/domain_admin/public/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/objects/1d/5380125d8b56c0426f9651cb8fb148b47a4c27` & `domain-admin-1.4.2/domain_admin/public/.git/objects/1d/5380125d8b56c0426f9651cb8fb148b47a4c27`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/objects/39/f04d3540ee3fad6d43a9831763d9eba45d0573` & `domain-admin-1.4.2/domain_admin/public/.git/objects/39/f04d3540ee3fad6d43a9831763d9eba45d0573`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949` & `domain-admin-1.4.2/domain_admin/public/.git/objects/3c/0f2e923566dc74d04e67d46d8b722923ed1949`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/objects/49/9cb6596b56d599852473fb85c29c53040e2f78` & `domain-admin-1.4.2/domain_admin/public/.git/objects/49/9cb6596b56d599852473fb85c29c53040e2f78`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/objects/50/0fd27e2e6061799cce3e7e6ed602915082a659` & `domain-admin-1.4.2/domain_admin/public/.git/objects/50/0fd27e2e6061799cce3e7e6ed602915082a659`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/objects/5b/1c488a74d8c3493cec2a99903972521902b410` & `domain-admin-1.4.2/domain_admin/public/.git/objects/5b/1c488a74d8c3493cec2a99903972521902b410`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34` & `domain-admin-1.4.2/domain_admin/public/.git/objects/5f/a7faf700c98850aa96022ab07af6a07b854f34`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc` & `domain-admin-1.4.2/domain_admin/public/.git/objects/6d/15191314c9b832ac41056a30bf0bf6533a29dc`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/objects/74/38a8b40596320051c82f62e00d1906c2d755d8` & `domain-admin-1.4.2/domain_admin/public/.git/objects/74/38a8b40596320051c82f62e00d1906c2d755d8`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/objects/7a/b699b6eea6b7e3d3c0130b97bdca0def787fef` & `domain-admin-1.4.2/domain_admin/public/.git/objects/7a/b699b6eea6b7e3d3c0130b97bdca0def787fef`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/objects/81/51e81a1838d6c47c21cdefbf26ecc9f5755db6` & `domain-admin-1.4.2/domain_admin/public/.git/objects/81/51e81a1838d6c47c21cdefbf26ecc9f5755db6`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/objects/8b/19737c31c38191351e2550ceba02f876fb253a` & `domain-admin-1.4.2/domain_admin/public/.git/objects/8b/19737c31c38191351e2550ceba02f876fb253a`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/objects/93/01be1310745fa1bd0a1929236eeaf354873706` & `domain-admin-1.4.2/domain_admin/public/.git/objects/93/01be1310745fa1bd0a1929236eeaf354873706`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/objects/95/c5323cc849308100d0409fdf506006828df9eb` & `domain-admin-1.4.2/domain_admin/public/.git/objects/95/c5323cc849308100d0409fdf506006828df9eb`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/objects/a2/709cde362f916eadaacfc27c47d0220dd4705c` & `domain-admin-1.4.2/domain_admin/public/.git/objects/a2/709cde362f916eadaacfc27c47d0220dd4705c`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/objects/a5/4d5e8c9407e7b569a1a8a7e3436fdcc7cffec3` & `domain-admin-1.4.2/domain_admin/public/.git/objects/a5/4d5e8c9407e7b569a1a8a7e3436fdcc7cffec3`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/objects/ac/b525d308d4833452f2159639607c0e10ac52e7` & `domain-admin-1.4.2/domain_admin/public/.git/objects/ac/b525d308d4833452f2159639607c0e10ac52e7`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/objects/ac/be31715261348534f51c95789f87d880bd018a` & `domain-admin-1.4.2/domain_admin/public/.git/objects/ac/be31715261348534f51c95789f87d880bd018a`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/objects/b1/c8fbd3728133a504f21a506ab5dff37409451f` & `domain-admin-1.4.2/domain_admin/public/.git/objects/b1/c8fbd3728133a504f21a506ab5dff37409451f`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/.git/objects/bb/9a94723f92fe51c9842c5c6baf60f9ca2b2e36` & `domain-admin-1.4.2/domain_admin/public/.git/objects/bb/9a94723f92fe51c9842c5c6baf60f9ca2b2e36`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/css/ConditionFilterGroup.a91875e6.css` & `domain-admin-1.4.2/domain_admin/public/css/ConditionFilterGroup.a91875e6.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/css/index.483612c5.css` & `domain-admin-1.4.2/domain_admin/public/css/index.483612c5.css`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/favicon.ico` & `domain-admin-1.4.2/domain_admin/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/index.html` & `domain-admin-1.4.2/domain_admin/public/index.html`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/js/ConditionFilterGroup.bbd10def.js` & `domain-admin-1.4.2/domain_admin/public/js/ConditionFilterGroup.bbd10def.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/js/ConnectStatus.3d8a0270.js` & `domain-admin-1.4.2/domain_admin/public/js/ConnectStatus.3d8a0270.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/js/SelectGroup.0f7c084d.js` & `domain-admin-1.4.2/domain_admin/public/js/SelectGroup.0f7c084d.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/js/element-icon.ade3aa7e.js` & `domain-admin-1.4.2/domain_admin/public/js/element-icon.ade3aa7e.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/js/element-plus.dcbfaaa8.js` & `domain-admin-1.4.2/domain_admin/public/js/element-plus.dcbfaaa8.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/js/index.050f1ae2.js` & `domain-admin-1.4.2/domain_admin/public/js/index.050f1ae2.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/js/index.2d4c528a.js` & `domain-admin-1.4.2/domain_admin/public/js/index.2d4c528a.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/js/index.3c22ca57.js` & `domain-admin-1.4.2/domain_admin/public/js/index.3c22ca57.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/js/index.83d13e8b.js` & `domain-admin-1.4.2/domain_admin/public/js/index.83d13e8b.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/js/index.888df730.js` & `domain-admin-1.4.2/domain_admin/public/js/index.888df730.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/js/index.bf2c4fd4.js` & `domain-admin-1.4.2/domain_admin/public/js/index.bf2c4fd4.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/js/index.bff8f0b2.js` & `domain-admin-1.4.2/domain_admin/public/js/index.bff8f0b2.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/js/index.c44ca8f1.js` & `domain-admin-1.4.2/domain_admin/public/js/index.c44ca8f1.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/js/index.cfa94de3.js` & `domain-admin-1.4.2/domain_admin/public/js/index.cfa94de3.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/js/vendor-lib.4c56f242.js` & `domain-admin-1.4.2/domain_admin/public/js/vendor-lib.4c56f242.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/js/vendor-vue.edbe275b.js` & `domain-admin-1.4.2/domain_admin/public/js/vendor-vue.edbe275b.js`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/public/svg/logo.184a2d7d.svg` & `domain-admin-1.4.2/domain_admin/public/svg/logo.184a2d7d.svg`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/router/api_map.py` & `domain-admin-1.4.2/domain_admin/router/api_map.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/router/permission.py` & `domain-admin-1.4.2/domain_admin/router/permission.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/service/auth_service.py` & `domain-admin-1.4.2/domain_admin/service/auth_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/service/cache_domain_info_service.py` & `domain-admin-1.4.2/domain_admin/service/cache_domain_info_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/service/domain_info_service.py` & `domain-admin-1.4.2/domain_admin/service/domain_info_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/service/domain_service.py` & `domain-admin-1.4.2/domain_admin/service/domain_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/service/email_service.py` & `domain-admin-1.4.2/domain_admin/service/email_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/service/file_service.py` & `domain-admin-1.4.2/domain_admin/service/file_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/service/notify_service.py` & `domain-admin-1.4.2/domain_admin/service/notify_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/service/scheduler_service.py` & `domain-admin-1.4.2/domain_admin/service/scheduler_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/service/system_service.py` & `domain-admin-1.4.2/domain_admin/service/system_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/service/token_service.py` & `domain-admin-1.4.2/domain_admin/service/token_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/service/version_service.py` & `domain-admin-1.4.2/domain_admin/service/version_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/service/work_weixin_service.py` & `domain-admin-1.4.2/domain_admin/service/work_weixin_service.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/templates/cert-email.html` & `domain-admin-1.4.2/domain_admin/templates/cert-email.html`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/templates/domain-email.html` & `domain-admin-1.4.2/domain_admin/templates/domain-email.html`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/utils/bcrypt_util.py` & `domain-admin-1.4.2/domain_admin/utils/bcrypt_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/utils/cert_util/__init__.py` & `domain-admin-1.4.2/domain_admin/utils/cert_util/__init__.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/utils/cert_util/cert_common.py` & `domain-admin-1.4.2/domain_admin/utils/cert_util/cert_common.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/utils/cert_util/cert_openssl.py` & `domain-admin-1.4.2/domain_admin/utils/cert_util/cert_openssl.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/utils/cert_util/cert_openssl_v2.py` & `domain-admin-1.4.2/domain_admin/utils/cert_util/cert_openssl_v2.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/utils/cert_util/cert_socket.py` & `domain-admin-1.4.2/domain_admin/utils/cert_util/cert_socket.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/utils/cert_util/cert_socket_v2.py` & `domain-admin-1.4.2/domain_admin/utils/cert_util/cert_socket_v2.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/utils/datetime_util.py` & `domain-admin-1.4.2/domain_admin/utils/datetime_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/utils/domain_util.py` & `domain-admin-1.4.2/domain_admin/utils/domain_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/utils/email_util.py` & `domain-admin-1.4.2/domain_admin/utils/email_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/utils/flask_ext/api_result.py` & `domain-admin-1.4.2/domain_admin/utils/flask_ext/api_result.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/utils/flask_ext/app_exception.py` & `domain-admin-1.4.2/domain_admin/utils/flask_ext/app_exception.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/utils/flask_ext/flask_app.py` & `domain-admin-1.4.2/domain_admin/utils/flask_ext/flask_app.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/utils/flask_ext/handler.py` & `domain-admin-1.4.2/domain_admin/utils/flask_ext/handler.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/utils/ip_util.py` & `domain-admin-1.4.2/domain_admin/utils/ip_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/utils/json_util.py` & `domain-admin-1.4.2/domain_admin/utils/json_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/utils/peewee_ext/model_util.py` & `domain-admin-1.4.2/domain_admin/utils/peewee_ext/model_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/utils/text_util.py` & `domain-admin-1.4.2/domain_admin/utils/text_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/utils/time_util.py` & `domain-admin-1.4.2/domain_admin/utils/time_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/utils/whois_util/config.py` & `domain-admin-1.4.2/domain_admin/utils/whois_util/config.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/utils/whois_util/util.py` & `domain-admin-1.4.2/domain_admin/utils/whois_util/util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/utils/whois_util/whois-servers.txt` & `domain-admin-1.4.2/domain_admin/utils/whois_util/whois-servers.txt`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/utils/whois_util/whois_util.py` & `domain-admin-1.4.2/domain_admin/utils/whois_util/whois_util.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin/utils/work_weixin_api.py` & `domain-admin-1.4.2/domain_admin/utils/work_weixin_api.py`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/domain_admin.egg-info/PKG-INFO` & `domain-admin-1.4.2/domain_admin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domain-admin
-Version: 1.4.1
+Version: 1.4.2
 Summary: a domain ssl cert admin
 Home-page: https://github.com/mouday/domain-admin
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Keywords: domain ssl cert
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `domain-admin-1.4.1/domain_admin.egg-info/SOURCES.txt` & `domain-admin-1.4.2/domain_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `domain-admin-1.4.1/setup.py` & `domain-admin-1.4.2/setup.py`

 * *Files identical despite different names*

