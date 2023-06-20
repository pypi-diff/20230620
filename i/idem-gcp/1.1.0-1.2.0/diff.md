# Comparing `tmp/idem_gcp-1.1.0.tar.gz` & `tmp/idem_gcp-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem_gcp-1.1.0.tar", last modified: Wed Jun  7 13:38:27 2023, max compression
+gzip compressed data, was "idem_gcp-1.2.0.tar", last modified: Tue Jun 20 07:50:38 2023, max compression
```

## Comparing `idem_gcp-1.1.0.tar` & `idem_gcp-1.2.0.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.408869 idem_gcp-1.1.0/
--rw-r--r--   0 root         (0) root         (0)    11342 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7881 2023-06-07 13:38:27.408869 idem_gcp-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6761 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/acct/gcp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/acct/gcp/contracts/
--rw-r--r--   0 root         (0) root         (0)      603 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/acct/gcp/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)     2375 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/acct/gcp/service_account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/autogen/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/autogen/gcp/
--rw-r--r--   0 root         (0) root         (0)     9958 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/autogen/gcp/schema_parser.py
--rw-r--r--   0 root         (0) root         (0)       75 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/autogen/init.py
--rw-r--r--   0 root         (0) root         (0)     1749 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/exec/gcp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.400869 idem_gcp-1.1.0/idem_gcp/exec/gcp/cloudkms/
--rw-r--r--   0 root         (0) root         (0)     4101 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/cloudkms/crypto_key.py
--rw-r--r--   0 root         (0) root         (0)    10239 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/cloudkms/crypto_key_version.py
--rw-r--r--   0 root         (0) root         (0)     4092 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/cloudkms/import_job.py
--rw-r--r--   0 root         (0) root         (0)     3759 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/cloudkms/key_ring.py
--rw-r--r--   0 root         (0) root         (0)     2737 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/cloudkms/location.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.400869 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/
--rw-r--r--   0 root         (0) root         (0)     6946 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/accelerator_type.py
--rw-r--r--   0 root         (0) root         (0)     5866 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/backend_service.py
--rw-r--r--   0 root         (0) root         (0)    16748 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/disk.py
--rw-r--r--   0 root         (0) root         (0)     7479 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/disk_type.py
--rw-r--r--   0 root         (0) root         (0)     6938 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/firewall.py
--rw-r--r--   0 root         (0) root         (0)    10946 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/forwarding_rule.py
--rw-r--r--   0 root         (0) root         (0)     5200 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/health_check.py
--rw-r--r--   0 root         (0) root         (0)     5925 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/image.py
--rw-r--r--   0 root         (0) root         (0)    49424 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/instance.py
--rw-r--r--   0 root         (0) root         (0)    17133 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/instance_group.py
--rw-r--r--   0 root         (0) root         (0)     4958 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/machine_image.py
--rw-r--r--   0 root         (0) root         (0)     6819 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/machine_type.py
--rw-r--r--   0 root         (0) root         (0)    15742 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/network.py
--rw-r--r--   0 root         (0) root         (0)     7311 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/node_template.py
--rw-r--r--   0 root         (0) root         (0)     5977 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/reservation.py
--rw-r--r--   0 root         (0) root         (0)     6275 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/resource_policy.py
--rw-r--r--   0 root         (0) root         (0)     7766 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     6381 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/subnetwork.py
--rw-r--r--   0 root         (0) root         (0)     5810 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/target_pool.py
--rw-r--r--   0 root         (0) root         (0)     5619 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/zone.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.400869 idem_gcp-1.1.0/idem_gcp/exec/gcp/contracts/
--rw-r--r--   0 root         (0) root         (0)      501 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/contracts/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/exec/gcp/iam/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.400869 idem_gcp-1.1.0/idem_gcp/exec/gcp/iam/projects/
--rw-r--r--   0 root         (0) root         (0)     9330 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/iam/projects/service_account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.400869 idem_gcp-1.1.0/idem_gcp/exec/gcp/iam/projects/service_accounts/
--rw-r--r--   0 root         (0) root         (0)     7914 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/iam/projects/service_accounts/key.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.400869 idem_gcp-1.1.0/idem_gcp/exec/gcp/storage/
--rw-r--r--   0 root         (0) root         (0)     4382 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp/storage/bucket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.400869 idem_gcp-1.1.0/idem_gcp/exec/gcp_api/
--rw-r--r--   0 root         (0) root         (0)     1073 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/exec/gcp_api/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.400869 idem_gcp-1.1.0/idem_gcp/helpers/
--rw-r--r--   0 root         (0) root         (0)      834 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/helpers/exc.py
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/helpers/log.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/helpers/returns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/metadata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/metadata/gcp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/metadata/gcp/cloudkms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/metadata/gcp/cloudkms/projects/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.400869 idem_gcp-1.1.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/
--rw-r--r--   0 root         (0) root         (0)      187 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.400869 idem_gcp-1.1.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.400869 idem_gcp-1.1.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/
--rw-r--r--   0 root         (0) root         (0)      204 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/crypto_key_versions.py
--rw-r--r--   0 root         (0) root         (0)      244 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.400869 idem_gcp-1.1.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/import_jobs/
--rw-r--r--   0 root         (0) root         (0)      244 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/import_jobs/init.py
--rw-r--r--   0 root         (0) root         (0)      220 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.404869 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/
--rw-r--r--   0 root         (0) root         (0)      183 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/accelerator_type.py
--rw-r--r--   0 root         (0) root         (0)      236 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/backend_service.py
--rw-r--r--   0 root         (0) root         (0)      238 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/disk.py
--rw-r--r--   0 root         (0) root         (0)      270 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/disk_type.py
--rw-r--r--   0 root         (0) root         (0)      147 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/firewall.py
--rw-r--r--   0 root         (0) root         (0)      182 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/forwarding_rule.py
--rw-r--r--   0 root         (0) root         (0)      165 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/global_operation.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/health_check.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/image.py
--rw-r--r--   0 root         (0) root         (0)      153 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/instance.py
--rw-r--r--   0 root         (0) root         (0)      174 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/instance_group.py
--rw-r--r--   0 root         (0) root         (0)      165 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/machine_image.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/machine_type.py
--rw-r--r--   0 root         (0) root         (0)      143 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/network.py
--rw-r--r--   0 root         (0) root         (0)      175 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/node_template.py
--rw-r--r--   0 root         (0) root         (0)      204 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/region_backend_service.py
--rw-r--r--   0 root         (0) root         (0)      175 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/region_operation.py
--rw-r--r--   0 root         (0) root         (0)      165 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/reservation.py
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/resource_policy.py
--rw-r--r--   0 root         (0) root         (0)      100 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/snapshot.py
--rw-r--r--   0 root         (0) root         (0)      116 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/subnetwork.py
--rw-r--r--   0 root         (0) root         (0)      184 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/target_pool.py
--rw-r--r--   0 root         (0) root         (0)      124 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/zone.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/compute/zone_operation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/metadata/gcp/iam/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.404869 idem_gcp-1.1.0/idem_gcp/metadata/gcp/iam/projects/
--rw-r--r--   0 root         (0) root         (0)      170 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/iam/projects/service_account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.404869 idem_gcp-1.1.0/idem_gcp/metadata/gcp/iam/projects/service_accounts/
--rw-r--r--   0 root         (0) root         (0)      183 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/iam/projects/service_accounts/key.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.404869 idem_gcp-1.1.0/idem_gcp/metadata/gcp/storage/
--rw-r--r--   0 root         (0) root         (0)      219 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/storage/bucket.py
--rw-r--r--   0 root         (0) root         (0)      224 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/metadata/gcp/storage/objectAccessControls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.404869 idem_gcp-1.1.0/idem_gcp/resources/
--rw-r--r--   0 root         (0) root         (0)    22734 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/resources/properties.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.404869 idem_gcp-1.1.0/idem_gcp/states/gcp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.404869 idem_gcp-1.1.0/idem_gcp/states/gcp/cloudkms/
--rw-r--r--   0 root         (0) root         (0)    22050 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/cloudkms/crypto_key.py
--rw-r--r--   0 root         (0) root         (0)    28486 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/cloudkms/crypto_key_version.py
--rw-r--r--   0 root         (0) root         (0)    15728 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/cloudkms/import_job.py
--rw-r--r--   0 root         (0) root         (0)     7639 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/cloudkms/key_ring.py
--rw-r--r--   0 root         (0) root         (0)     2544 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/cloudkms/location.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.404869 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/
--rw-r--r--   0 root         (0) root         (0)    80631 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/backend_service.py
--rw-r--r--   0 root         (0) root         (0)    26659 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/disk.py
--rw-r--r--   0 root         (0) root         (0)    18532 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/firewall.py
--rw-r--r--   0 root         (0) root         (0)    27433 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/forwarding_rule.py
--rw-r--r--   0 root         (0) root         (0)    35690 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/health_check.py
--rw-r--r--   0 root         (0) root         (0)    19067 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/image.py
--rw-r--r--   0 root         (0) root         (0)    89687 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/instance.py
--rw-r--r--   0 root         (0) root         (0)    13388 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/instance_group.py
--rw-r--r--   0 root         (0) root         (0)    14687 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/machine_image.py
--rw-r--r--   0 root         (0) root         (0)    22166 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/network.py
--rw-r--r--   0 root         (0) root         (0)     6028 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/node_template.py
--rw-r--r--   0 root         (0) root         (0)     6068 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/reservation.py
--rw-r--r--   0 root         (0) root         (0)    14696 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/resource_policy.py
--rw-r--r--   0 root         (0) root         (0)    17125 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/snapshot.py
--rw-r--r--   0 root         (0) root         (0)    20411 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/subnetwork.py
--rw-r--r--   0 root         (0) root         (0)     8550 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/compute/target_pool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/states/gcp/iam/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.404869 idem_gcp-1.1.0/idem_gcp/states/gcp/iam/projects/
--rw-r--r--   0 root         (0) root         (0)    11923 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/iam/projects/service_account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.404869 idem_gcp-1.1.0/idem_gcp/states/gcp/iam/projects/service_accounts/
--rw-r--r--   0 root         (0) root         (0)     9632 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/iam/projects/service_accounts/key.py
--rw-r--r--   0 root         (0) root         (0)      144 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.404869 idem_gcp-1.1.0/idem_gcp/states/gcp/recursive_contracts/
--rw-r--r--   0 root         (0) root         (0)    15853 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/recursive_contracts/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.404869 idem_gcp-1.1.0/idem_gcp/states/gcp/storage/
--rw-r--r--   0 root         (0) root         (0)    40592 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/states/gcp/storage/bucket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.408869 idem_gcp-1.1.0/idem_gcp/tool/gcp/
--rw-r--r--   0 root         (0) root         (0)     1800 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/case.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.408869 idem_gcp-1.1.0/idem_gcp/tool/gcp/cloudkms/
--rw-r--r--   0 root         (0) root         (0)     5296 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/cloudkms/crypto_key_version_utils.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/cloudkms/patch.py
--rw-r--r--   0 root         (0) root         (0)     3953 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/comment_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.408869 idem_gcp-1.1.0/idem_gcp/tool/gcp/compute/
--rw-r--r--   0 root         (0) root         (0)     9834 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/compute/disk.py
--rw-r--r--   0 root         (0) root         (0)    11892 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/compute/instance.py
--rw-r--r--   0 root         (0) root         (0)      722 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/compute/instance_group.py
--rw-r--r--   0 root         (0) root         (0)     5276 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/compute/network.py
--rw-r--r--   0 root         (0) root         (0)      537 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/compute/subnetwork.py
--rw-r--r--   0 root         (0) root         (0)     4000 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/conversion_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.408869 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/
--rw-r--r--   0 root         (0) root         (0)     1116 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/exec_context.py
--rw-r--r--   0 root         (0) root         (0)      533 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/exec_param.py
--rw-r--r--   0 root         (0) root         (0)     1544 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/generic_exec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.408869 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/post_exec/
--rw-r--r--   0 root         (0) root         (0)      704 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/post_exec/item_getter.py
--rw-r--r--   0 root         (0) root         (0)     2771 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/post_exec/operation_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.408869 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/pre_exec/
--rw-r--r--   0 root         (0) root         (0)     1547 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/pre_exec/function_getter.py
--rw-r--r--   0 root         (0) root         (0)      522 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/pre_exec/parameter_sanitizer.py
--rw-r--r--   0 root         (0) root         (0)     1284 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/pre_exec/resource_id_extractor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.408869 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/recursive_contracts/
--rw-r--r--   0 root         (0) root         (0)      244 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/recursive_contracts/init.py
--rw-r--r--   0 root         (0) root         (0)      309 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/scope.py
--rw-r--r--   0 root         (0) root         (0)     1519 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/hub_resolver.py
--rw-r--r--   0 root         (0) root         (0)    21776 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/init.py
--rw-r--r--   0 root         (0) root         (0)     5614 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/operation_utils.py
--rw-r--r--   0 root         (0) root         (0)     1923 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/policy.py
--rw-r--r--   0 root         (0) root         (0)    18555 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/resolver.py
--rw-r--r--   0 root         (0) root         (0)    18698 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/resource_prop_utils.py
--rw-r--r--   0 root         (0) root         (0)     1530 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/sanitizers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.408869 idem_gcp-1.1.0/idem_gcp/tool/gcp/schema/
--rw-r--r--   0 root         (0) root         (0)      874 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/schema/finding.py
--rw-r--r--   0 root         (0) root         (0)     1845 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/schema/results_collector.py
--rw-r--r--   0 root         (0) root         (0)     2725 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/schema/schema_compatibility_checker.py
--rw-r--r--   0 root         (0) root         (0)     1283 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/schema/schema_naming_checker.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/schema/scm_utils.py
--rw-r--r--   0 root         (0) root         (0)      597 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/session.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/state_comparison_utils.py
--rw-r--r--   0 root         (0) root         (0)     2556 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/state_operation_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.408869 idem_gcp-1.1.0/idem_gcp/tool/gcp/storage/
--rw-r--r--   0 root         (0) root         (0)     2334 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/storage/bucket.py
--rw-r--r--   0 root         (0) root         (0)    19738 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/idem_gcp/tool/gcp/utils.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-07 13:38:26.000000 idem_gcp-1.1.0/idem_gcp/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 13:38:27.396869 idem_gcp-1.1.0/idem_gcp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7881 2023-06-07 13:38:27.000000 idem_gcp-1.1.0/idem_gcp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6140 2023-06-07 13:38:27.000000 idem_gcp-1.1.0/idem_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 13:38:27.000000 idem_gcp-1.1.0/idem_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-07 13:38:27.000000 idem_gcp-1.1.0/idem_gcp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      251 2023-06-07 13:38:27.000000 idem_gcp-1.1.0/idem_gcp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-07 13:38:27.000000 idem_gcp-1.1.0/idem_gcp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-07 13:38:27.408869 idem_gcp-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3303 2023-06-07 13:38:12.000000 idem_gcp-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.147737 idem_gcp-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)    11342 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7881 2023-06-20 07:50:38.147737 idem_gcp-1.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6761 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/acct/gcp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/acct/gcp/contracts/
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/acct/gcp/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/acct/gcp/service_account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/autogen/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/autogen/gcp/
+-rw-r--r--   0 root         (0) root         (0)     9958 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/autogen/gcp/schema_parser.py
+-rw-r--r--   0 root         (0) root         (0)       75 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/autogen/init.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/exec/gcp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/exec/gcp/cloudkms/
+-rw-r--r--   0 root         (0) root         (0)     4101 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/cloudkms/crypto_key.py
+-rw-r--r--   0 root         (0) root         (0)    10239 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/cloudkms/crypto_key_version.py
+-rw-r--r--   0 root         (0) root         (0)     4092 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/cloudkms/import_job.py
+-rw-r--r--   0 root         (0) root         (0)     3759 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/cloudkms/key_ring.py
+-rw-r--r--   0 root         (0) root         (0)     2737 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/cloudkms/location.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/
+-rw-r--r--   0 root         (0) root         (0)     6946 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/accelerator_type.py
+-rw-r--r--   0 root         (0) root         (0)     5866 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/backend_service.py
+-rw-r--r--   0 root         (0) root         (0)    16748 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/disk.py
+-rw-r--r--   0 root         (0) root         (0)     7479 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/disk_type.py
+-rw-r--r--   0 root         (0) root         (0)     6938 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/firewall.py
+-rw-r--r--   0 root         (0) root         (0)    10946 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/forwarding_rule.py
+-rw-r--r--   0 root         (0) root         (0)     5200 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/health_check.py
+-rw-r--r--   0 root         (0) root         (0)     5925 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/image.py
+-rw-r--r--   0 root         (0) root         (0)    49424 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/instance.py
+-rw-r--r--   0 root         (0) root         (0)    17133 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/instance_group.py
+-rw-r--r--   0 root         (0) root         (0)     4958 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/machine_image.py
+-rw-r--r--   0 root         (0) root         (0)     6819 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/machine_type.py
+-rw-r--r--   0 root         (0) root         (0)    15742 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/network.py
+-rw-r--r--   0 root         (0) root         (0)     7311 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/node_template.py
+-rw-r--r--   0 root         (0) root         (0)     5977 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/reservation.py
+-rw-r--r--   0 root         (0) root         (0)     6275 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/resource_policy.py
+-rw-r--r--   0 root         (0) root         (0)     7766 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     6381 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/subnetwork.py
+-rw-r--r--   0 root         (0) root         (0)     5810 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/target_pool.py
+-rw-r--r--   0 root         (0) root         (0)     5619 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/zone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/exec/gcp/contracts/
+-rw-r--r--   0 root         (0) root         (0)      501 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/contracts/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/exec/gcp/iam/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/exec/gcp/iam/projects/
+-rw-r--r--   0 root         (0) root         (0)     9330 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/iam/projects/service_account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/exec/gcp/iam/projects/service_accounts/
+-rw-r--r--   0 root         (0) root         (0)     7914 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/iam/projects/service_accounts/key.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/exec/gcp/storage/
+-rw-r--r--   0 root         (0) root         (0)     4382 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/storage/bucket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/exec/gcp_api/
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp_api/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/helpers/
+-rw-r--r--   0 root         (0) root         (0)      834 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/helpers/exc.py
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/helpers/log.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/helpers/returns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/metadata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/metadata/gcp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/metadata/gcp/cloudkms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/metadata/gcp/cloudkms/projects/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/
+-rw-r--r--   0 root         (0) root         (0)      187 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/
+-rw-r--r--   0 root         (0) root         (0)      204 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/crypto_key_versions.py
+-rw-r--r--   0 root         (0) root         (0)      244 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/import_jobs/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/import_jobs/init.py
+-rw-r--r--   0 root         (0) root         (0)      220 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.143737 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/
+-rw-r--r--   0 root         (0) root         (0)      183 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/accelerator_type.py
+-rw-r--r--   0 root         (0) root         (0)      236 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/backend_service.py
+-rw-r--r--   0 root         (0) root         (0)      238 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/disk.py
+-rw-r--r--   0 root         (0) root         (0)      270 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/disk_type.py
+-rw-r--r--   0 root         (0) root         (0)      147 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/firewall.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/forwarding_rule.py
+-rw-r--r--   0 root         (0) root         (0)      165 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/global_operation.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/health_check.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/image.py
+-rw-r--r--   0 root         (0) root         (0)      153 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/instance.py
+-rw-r--r--   0 root         (0) root         (0)      174 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/instance_group.py
+-rw-r--r--   0 root         (0) root         (0)      165 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/machine_image.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/machine_type.py
+-rw-r--r--   0 root         (0) root         (0)      143 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/network.py
+-rw-r--r--   0 root         (0) root         (0)      175 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/node_template.py
+-rw-r--r--   0 root         (0) root         (0)      204 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/region_backend_service.py
+-rw-r--r--   0 root         (0) root         (0)      175 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/region_operation.py
+-rw-r--r--   0 root         (0) root         (0)      165 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/reservation.py
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/resource_policy.py
+-rw-r--r--   0 root         (0) root         (0)      100 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)      116 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/subnetwork.py
+-rw-r--r--   0 root         (0) root         (0)      184 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/target_pool.py
+-rw-r--r--   0 root         (0) root         (0)      124 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/zone.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/zone_operation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/metadata/gcp/iam/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.143737 idem_gcp-1.2.0/idem_gcp/metadata/gcp/iam/projects/
+-rw-r--r--   0 root         (0) root         (0)      170 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/iam/projects/service_account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.143737 idem_gcp-1.2.0/idem_gcp/metadata/gcp/iam/projects/service_accounts/
+-rw-r--r--   0 root         (0) root         (0)      183 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/iam/projects/service_accounts/key.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.143737 idem_gcp-1.2.0/idem_gcp/metadata/gcp/storage/
+-rw-r--r--   0 root         (0) root         (0)      219 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/storage/bucket.py
+-rw-r--r--   0 root         (0) root         (0)      224 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/storage/objectAccessControls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.143737 idem_gcp-1.2.0/idem_gcp/resources/
+-rw-r--r--   0 root         (0) root         (0)    22702 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/resources/properties.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.143737 idem_gcp-1.2.0/idem_gcp/states/gcp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.143737 idem_gcp-1.2.0/idem_gcp/states/gcp/cloudkms/
+-rw-r--r--   0 root         (0) root         (0)    30514 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/cloudkms/crypto_key.py
+-rw-r--r--   0 root         (0) root         (0)    29172 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/cloudkms/crypto_key_version.py
+-rw-r--r--   0 root         (0) root         (0)    16925 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/cloudkms/import_job.py
+-rw-r--r--   0 root         (0) root         (0)     7655 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/cloudkms/key_ring.py
+-rw-r--r--   0 root         (0) root         (0)     2549 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/cloudkms/location.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.143737 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/
+-rw-r--r--   0 root         (0) root         (0)    81756 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/backend_service.py
+-rw-r--r--   0 root         (0) root         (0)    29638 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/disk.py
+-rw-r--r--   0 root         (0) root         (0)    18544 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/firewall.py
+-rw-r--r--   0 root         (0) root         (0)    27526 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/forwarding_rule.py
+-rw-r--r--   0 root         (0) root         (0)    35507 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/health_check.py
+-rw-r--r--   0 root         (0) root         (0)    24598 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/image.py
+-rw-r--r--   0 root         (0) root         (0)    89505 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/instance.py
+-rw-r--r--   0 root         (0) root         (0)    13426 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/instance_group.py
+-rw-r--r--   0 root         (0) root         (0)    14791 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/machine_image.py
+-rw-r--r--   0 root         (0) root         (0)    22275 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/network.py
+-rw-r--r--   0 root         (0) root         (0)     6821 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/node_template.py
+-rw-r--r--   0 root         (0) root         (0)     8342 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/reservation.py
+-rw-r--r--   0 root         (0) root         (0)    14697 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/resource_policy.py
+-rw-r--r--   0 root         (0) root         (0)    17272 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    20407 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/subnetwork.py
+-rw-r--r--   0 root         (0) root         (0)     8557 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/target_pool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/states/gcp/iam/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.143737 idem_gcp-1.2.0/idem_gcp/states/gcp/iam/projects/
+-rw-r--r--   0 root         (0) root         (0)    12073 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/iam/projects/service_account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.143737 idem_gcp-1.2.0/idem_gcp/states/gcp/iam/projects/service_accounts/
+-rw-r--r--   0 root         (0) root         (0)     9632 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/iam/projects/service_accounts/key.py
+-rw-r--r--   0 root         (0) root         (0)      144 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.143737 idem_gcp-1.2.0/idem_gcp/states/gcp/recursive_contracts/
+-rw-r--r--   0 root         (0) root         (0)    15877 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/recursive_contracts/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.143737 idem_gcp-1.2.0/idem_gcp/states/gcp/storage/
+-rw-r--r--   0 root         (0) root         (0)    41239 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/storage/bucket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.147737 idem_gcp-1.2.0/idem_gcp/tool/gcp/
+-rw-r--r--   0 root         (0) root         (0)     1800 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/case.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.147737 idem_gcp-1.2.0/idem_gcp/tool/gcp/cloudkms/
+-rw-r--r--   0 root         (0) root         (0)     5296 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/cloudkms/crypto_key_version_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/cloudkms/patch.py
+-rw-r--r--   0 root         (0) root         (0)     3953 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/comment_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.147737 idem_gcp-1.2.0/idem_gcp/tool/gcp/compute/
+-rw-r--r--   0 root         (0) root         (0)     9834 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/compute/disk.py
+-rw-r--r--   0 root         (0) root         (0)    11892 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/compute/instance.py
+-rw-r--r--   0 root         (0) root         (0)      722 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/compute/instance_group.py
+-rw-r--r--   0 root         (0) root         (0)     5276 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/compute/network.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/compute/subnetwork.py
+-rw-r--r--   0 root         (0) root         (0)     4000 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/conversion_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.147737 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/exec_context.py
+-rw-r--r--   0 root         (0) root         (0)      533 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/exec_param.py
+-rw-r--r--   0 root         (0) root         (0)     1544 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/generic_exec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.147737 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/post_exec/
+-rw-r--r--   0 root         (0) root         (0)      704 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/post_exec/item_getter.py
+-rw-r--r--   0 root         (0) root         (0)     2771 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/post_exec/operation_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.147737 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/pre_exec/
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/pre_exec/function_getter.py
+-rw-r--r--   0 root         (0) root         (0)      522 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/pre_exec/parameter_sanitizer.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/pre_exec/resource_id_extractor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.147737 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/recursive_contracts/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/recursive_contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)      309 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/scope.py
+-rw-r--r--   0 root         (0) root         (0)     1519 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/hub_resolver.py
+-rw-r--r--   0 root         (0) root         (0)    21776 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/init.py
+-rw-r--r--   0 root         (0) root         (0)     5614 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/operation_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/policy.py
+-rw-r--r--   0 root         (0) root         (0)    18555 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/resolver.py
+-rw-r--r--   0 root         (0) root         (0)    18698 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/resource_prop_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/sanitizers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.147737 idem_gcp-1.2.0/idem_gcp/tool/gcp/schema/
+-rw-r--r--   0 root         (0) root         (0)      874 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/schema/finding.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/schema/results_collector.py
+-rw-r--r--   0 root         (0) root         (0)     2725 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/schema/schema_compatibility_checker.py
+-rw-r--r--   0 root         (0) root         (0)     1283 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/schema/schema_naming_checker.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/schema/scm_utils.py
+-rw-r--r--   0 root         (0) root         (0)      597 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/session.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/state_comparison_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/state_operation_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.147737 idem_gcp-1.2.0/idem_gcp/tool/gcp/storage/
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/storage/bucket.py
+-rw-r--r--   0 root         (0) root         (0)    19738 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/utils.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-20 07:50:37.000000 idem_gcp-1.2.0/idem_gcp/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7881 2023-06-20 07:50:38.000000 idem_gcp-1.2.0/idem_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6140 2023-06-20 07:50:38.000000 idem_gcp-1.2.0/idem_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 07:50:38.000000 idem_gcp-1.2.0/idem_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-20 07:50:38.000000 idem_gcp-1.2.0/idem_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      251 2023-06-20 07:50:38.000000 idem_gcp-1.2.0/idem_gcp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-20 07:50:38.000000 idem_gcp-1.2.0/idem_gcp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-20 07:50:38.147737 idem_gcp-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3303 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/setup.py
```

### Comparing `idem_gcp-1.1.0/LICENSE` & `idem_gcp-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/PKG-INFO` & `idem_gcp-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem_gcp
-Version: 1.1.0
+Version: 1.2.0
 Summary: GCP Cloud Provider for Idem
 Home-page: https://gitlab.com/vmware/idem/idem-gcp
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/idem/idem-gcp
 Project-URL: Issue tracker, https://gitlab.com/vmware/idem/idem-gcp/-/issues
```

### Comparing `idem_gcp-1.1.0/README.rst` & `idem_gcp-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/acct/gcp/contracts/init.py` & `idem_gcp-1.2.0/idem_gcp/acct/gcp/contracts/init.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/acct/gcp/service_account.py` & `idem_gcp-1.2.0/idem_gcp/acct/gcp/service_account.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/autogen/gcp/schema_parser.py` & `idem_gcp-1.2.0/idem_gcp/autogen/gcp/schema_parser.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/conf.py` & `idem_gcp-1.2.0/idem_gcp/conf.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/cloudkms/crypto_key.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/cloudkms/crypto_key.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/cloudkms/crypto_key_version.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/cloudkms/crypto_key_version.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/cloudkms/import_job.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/cloudkms/import_job.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/cloudkms/key_ring.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/cloudkms/key_ring.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/cloudkms/location.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/cloudkms/location.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/accelerator_type.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/accelerator_type.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/backend_service.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/backend_service.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/disk.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/disk.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/disk_type.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/disk_type.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/firewall.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/firewall.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/forwarding_rule.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/forwarding_rule.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/health_check.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/health_check.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/image.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/image.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/instance.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/instance.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/instance_group.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/instance_group.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/machine_image.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/machine_image.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/machine_type.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/machine_type.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/network.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/network.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/node_template.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/node_template.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/reservation.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/reservation.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/resource_policy.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/resource_policy.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/snapshot.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/snapshot.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/subnetwork.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/subnetwork.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/target_pool.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/target_pool.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/compute/zone.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/zone.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/iam/projects/service_account.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/iam/projects/service_account.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/iam/projects/service_accounts/key.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/iam/projects/service_accounts/key.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp/storage/bucket.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp/storage/bucket.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/exec/gcp_api/init.py` & `idem_gcp-1.2.0/idem_gcp/exec/gcp_api/init.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/helpers/exc.py` & `idem_gcp-1.2.0/idem_gcp/helpers/exc.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/helpers/log.py` & `idem_gcp-1.2.0/idem_gcp/helpers/log.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/helpers/returns.py` & `idem_gcp-1.2.0/idem_gcp/helpers/returns.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/resources/properties.yaml` & `idem_gcp-1.2.0/idem_gcp/resources/properties.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -315,23 +315,21 @@
     - requestId
 #    body
     - name
     - autoCreateSubnetworks
     - description
     - enableUlaInternalIpv6
     - internalIpv6Range
-    - IPv4Range
     - mtu
     - networkFirewallPolicyEnforcementOrder
     - routingConfig
     - peerings
   update:
     - enableUlaInternalIpv6
     - internalIpv6Range
-    - IPv4Range
     - mtu
     - networkFirewallPolicyEnforcementOrder
     - routingConfig
     - peerings
   readonly_return_props:
     - id
   delete:
```

### Comparing `idem_gcp-1.1.0/idem_gcp/states/gcp/cloudkms/crypto_key.py` & `idem_gcp-1.2.0/idem_gcp/states/gcp/cloudkms/import_job.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,249 +1,214 @@
-"""State module for managing Cloud Key Management Service crypto keys."""
+"""State module for managing Cloud Key Management Service import job."""
 from dataclasses import field
 from dataclasses import make_dataclass
 from typing import Any
 from typing import Dict
 from typing import List
 
 __contracts__ = ["resource"]
-RESOURCE_TYPE = "cloudkms.crypto_key"
-RESOURCE_TYPE_FULL = "cloudkms.projects.locations.key_rings.crypto_keys"
-GCP_RESOURCE_TYPE_FULL = "gcp.cloudkms.crypto_key"
+RESOURCE_TYPE = "cloudkms.import_jobs"
+RESOURCE_TYPE_FULL = "cloudkms.projects.locations.key_rings.import_jobs"
+GCP_RESOURCE_TYPE_FULL = "gcp.cloudkms.import_jobs"
 
 
 async def present(
     hub,
     ctx,
     name: str,
-    crypto_key_id: str = None,
+    import_method: str,
+    protection_level: str,
+    import_job_id: str = None,
     project_id: str = None,
     location_id: str = None,
     key_ring_id: str = None,
-    primary: make_dataclass(
-        "CryptoKeyVersion",
+    create_time: str = None,
+    generate_time: str = None,
+    expire_time: str = None,
+    expire_event_time: str = None,
+    job_state: str = None,
+    public_key: str = None,
+    attestation: make_dataclass(
+        "KeyOperationAttestation",
         [
-            ("name", str),
-            ("state", str, field(default=None)),
-            ("protection_level", str, field(default=None)),
-            ("algorithm", str, field(default=None)),
+            ("format", str, field(default=None)),
+            ("content", str, field(default=None)),
             (
-                "attestation",
+                "cert_chains",
                 make_dataclass(
-                    "KeyOperationAttestation",
+                    "CertificateChains",
                     [
-                        ("format", str, field(default=None)),
-                        ("content", str, field(default=None)),
+                        ("cavium_certs", List[str], field(default=None)),
                         (
-                            "cert_chains",
-                            make_dataclass(
-                                "CertificateChains",
-                                [
-                                    ("cavium_certs", List[str], field(default=None)),
-                                    (
-                                        "google_card_certs",
-                                        List[str],
-                                        field(default=None),
-                                    ),
-                                    (
-                                        "google_partition_certs",
-                                        List[str],
-                                        field(default=None),
-                                    ),
-                                ],
-                            ),
+                            "google_card_certs",
+                            List[str],
+                            field(default=None),
+                        ),
+                        (
+                            "google_partition_certs",
+                            List[str],
                             field(default=None),
                         ),
                     ],
                 ),
                 field(default=None),
             ),
-            ("create_time", str, field(default=None)),
-            ("generate_time", str, field(default=None)),
-            ("destroy_time", str, field(default=None)),
-            ("destroy_event_time", str, field(default=None)),
-            ("import_job", str, field(default=None)),
-            ("import_time", str, field(default=None)),
-            ("import_failure_reason", str, field(default=None)),
-            (
-                "external_protection_level_options",
-                make_dataclass(
-                    "ExternalProtectionLevelOptions",
-                    [
-                        ("external_key_uri", str, field(default=None)),
-                        ("ekm_connection_key_path", str, field(default=None)),
-                    ],
-                ),
-                field(default=None),
-            ),
-            ("reimport_eligible", bool, field(default=None)),
-        ],
-    ) = None,
-    purpose: str = None,
-    create_time: str = None,
-    next_rotation_time: str = None,
-    version_template: make_dataclass(
-        "CryptoKeyVersionTemplate",
-        [
-            ("protection_level", str, field(default=None)),
-            ("algorithm", str, field(default=None)),
         ],
     ) = None,
-    labels: Dict[str, str] = None,
-    import_only: bool = None,
-    destroy_scheduled_duration: str = None,
-    crypto_key_backend: str = None,
-    rotation_period: str = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
-    r"""Create or update a `CryptoKey`_ within a `KeyRing`_.
-
-    `CryptoKey.purpose`_ and `CryptoKey.version_template.algorithm`_ are required for a new `CryptoKey`_.
+    """Create a new `ImportJob`_ within a `KeyRing`_.
 
     Args:
         name(str):
             Idem name.
 
-        crypto_key_id(str, Optional):
-            Crypto key id.
+        import_job_id(str, Optional):
+            Import job id. It must be unique within a KeyRing and match the regular expression ``[a-zA-Z0-9_-]{1,63}``
 
         project_id(str, Optional):
             Project Id of the new crypto key.
 
         location_id(str, Optional):
             Location Id of the new crypto key.
 
         key_ring_id(str, Optional):
             Keyring Id of the new crypto key.
 
-        primary(Dict[str, Any], Optional):
-            A copy of the "primary" CryptoKeyVersion that will be used by cryptoKeys.encrypt when this
-            CryptoKey is given in EncryptRequest.name. Keys with purpose ENCRYPT_DECRYPT may have a primary. For other keys,
-            this field will be omitted. To update the primary key provide only `primary.name = new_resource_id`. All
-            other CryptoKeyVersion are output only.
+        import_method(str):
+            Immutable. The wrapping method to be used for incoming key material. See `ImportMethod`_.
 
-        purpose(str, Optional):
-            Immutable. The immutable purpose of this CryptoKey.
+        protection_level(str):
+            Immutable. The protection level of the `ImportJob`_. This must match the `protectionLevel`_ of the
+            `versionTemplate`_ on the `CryptoKey`_ you attempt to import into.
 
         create_time(str, Optional):
-            Output only. The time at which this CryptoKey was created. A timestamp in RFC3339 UTC "Zulu" format, with
-            nanosecond resolution and up to nine fractional digits. Examples: "2014-10-02T15:01:23Z" and
-            "2014-10-02T15:01:23.045123456Z".
-
-        next_rotation_time(str, Optional):
-            At nextRotationTime, the Key Management Service will automatically:
-
-            - Create a new version of this CryptoKey.
-            - Mark the new version as primary.
-
-            Key rotations performed manually via cryptoKeyVersions.create and cryptoKeys.updatePrimaryVersion do not
-            affect nextRotationTime. Keys with purpose ENCRYPT_DECRYPT support automatic rotation. For other keys, this
-            field must be omitted. A timestamp in RFC3339 UTC "Zulu" format, with nanosecond resolution and up to nine
-            fractional digits. Examples: "2014-10-02T15:01:23Z" and "2014-10-02T15:01:23.045123456Z".
-
-        version_template(Dict[str, Any], Optional):
-            A template describing settings for new CryptoKeyVersion instances. The properties of new CryptoKeyVersion
-            instances created by either cryptoKeyVersions.create or auto-rotation are controlled by this template.
-
-        labels(Dict[str, str], Optional):
-            Labels with user-defined metadata. For more information, see `Labeling Keys`_.
-
-        import_only(bool, Optional):
-            Immutable. Whether this key may contain imported versions only.
-
-        destroy_scheduled_duration(str, Optional):
-            Immutable. The period of time that versions of this key spend in the DESTROY_SCHEDULED state before
-            transitioning to DESTROYED. If not specified at creation time, the default duration is 24 hours. A duration
-            in seconds with up to nine fractional digits, terminated by 's'. Example: "3.5s".
-
-        crypto_key_backend(str, Optional):
-            Immutable. The resource name of the backend environment where the key material for all CryptoKeyVersions
-            associated with this `CryptoKey`_ reside and where all related cryptographic operations are performed. Only
-            applicable if `CryptoKeyVersions`_ have a `ProtectionLevel`_ of
-            [EXTERNAL_VPC][CryptoKeyVersion.ProtectionLevel.EXTERNAL_VPC], with the resource name in the format
-            `projects/\\*/locations/\\*/ekmConnections/\\*`. Note, this list is non-exhaustive and may apply to additional
-            `ProtectionLevels`_ in the future.
-
-        rotation_period(str, Optional):
-            next_rotation_time will be advanced by this period when the service automatically rotates a key.
-            Must be at least 24 hours and at most 876,000 hours.
+            Output only. The time at which this `ImportJob`_ was created.
+
+            A timestamp in RFC3339 UTC "Zulu" format, with nanosecond resolution and up to nine fractional digits.
+            Examples: "2014-10-02T15:01:23Z" and "2014-10-02T15:01:23.045123456Z".
+
+        generate_time(str, Optional):
+            Output only. The time this `ImportJob`_'s key material was generated.
+
+            A timestamp in RFC3339 UTC "Zulu" format, with nanosecond resolution and up to nine fractional digits.
+            Examples: "2014-10-02T15:01:23Z" and "2014-10-02T15:01:23.045123456Z".
+
+        expire_time(str, Optional):
+            Output only. The time at which this `ImportJob`_ is scheduled for expiration and can no longer be used to
+            import key material.
+
+            A timestamp in RFC3339 UTC "Zulu" format, with nanosecond resolution and up to nine fractional digits.
+            Examples: "2014-10-02T15:01:23Z" and "2014-10-02T15:01:23.045123456Z".
+
+        expire_event_time(str, Optional):
+            Output only. The time this `ImportJob`_ expired. Only present if `state`_ is `EXPIRED`_.
+
+            A timestamp in RFC3339 UTC "Zulu" format, with nanosecond resolution and up to nine fractional digits.
+            Examples: "2014-10-02T15:01:23Z" and "2014-10-02T15:01:23.045123456Z".
+
+        job_state(str, Optional):
+            Output only. The current state of the `ImportJob`_, indicating if it can be used.
+
+        public_key(str, Optional):
+            Output only. The public key with which to wrap key material prior to import. Only returned if `state`_ is
+             `ACTIVE`_.
+
+        attestation(Dict[str, Any], Optional):
+            Output only. Statement that was generated and signed by the key creator (for example, an HSM) at key
+            creation time. Use this statement to verify attributes of the key as stored on the HSM, independently
+            of Google. Only present if the chosen ImportMethod is one with a protection level of HSM.
+
+            * format(str, Optional):
+                Output only. The format of the attestation data.
+                Enum type. Allowed values:
+                    "ATTESTATION_FORMAT_UNSPECIFIED"
+                    "CAVIUM_V1_COMPRESSED"
+                    "CAVIUM_V2_COMPRESSED"
+
+            * content(str, Optional):
+                Output only. The attestation data provided by the HSM when the key operation was performed.
+
+            * cert_chains(Dict[str, Any], Optional):
+                Output only. The certificate chains needed to validate the attestation.
+                Certificate chains needed to verify the attestation. Certificates in chains are PEM-encoded
+                and are ordered based on https://tools.ietf.org/html/rfc5246#section-7.4.2.
 
-            If rotation_period is set, next_rotation_time must also be set. Keys
-            with purpose ENCRYPT_DECRYPT support automatic rotation. For other keys, this field must be omitted.
+                * cavium_certs(list[str], Optional):
+                    Cavium certificate chain corresponding to the attestation.
 
-            A duration in seconds with up to nine fractional digits, terminated by 's'. Example: "3.5s".
+                * google_card_certs(list[str], Optional):
+                    Google card certificate chain corresponding to the attestation.
+
+                * google_partition_certs(list[str], Optional):
+                    Google partition certificate chain corresponding to the attestation.
 
         resource_id(str, Optional): Idem resource id. Formatted as
 
-            `projects/{project_id}/locations/{location_id}/keyRings/{key_ring_id}/cryptoKeys/{crypto_key_id}`
+            `projects/{project_id}/locations/{location_id}/keyRings/{key_ring_id}/importJobs/{import_job_id}`
 
-    .. _CryptoKey: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.cryptoKeys#CryptoKey
+    .. _ImportJob: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.importJobs#ImportJob
     .. _KeyRing: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings#KeyRing
-    .. _CryptoKey.purpose: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.cryptoKeys#CryptoKey.FIELDS.purpose
-    .. _CryptoKey.version_template.algorithm: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.cryptoKeys#CryptoKeyVersionTemplate.FIELDS.algorithm
     .. _Labeling Keys: https://cloud.google.com/kms/docs/labeling-keys
-    .. _CryptoKeyVersions: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.cryptoKeys.cryptoKeyVersions#CryptoKeyVersion
     .. _ProtectionLevel: https://cloud.google.com/kms/docs/reference/rest/v1/ProtectionLevel
-    .. _ProtectionLevels: https://cloud.google.com/kms/docs/reference/rest/v1/ProtectionLevel
+    .. _ImportMethod: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.importJobs#ImportMethod
+    .. _CryptoKey: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.cryptoKeys#CryptoKey
+    .. _versionTemplate: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.cryptoKeys#CryptoKey.FIELDS.version_template
+    .. _protectionLevel: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.cryptoKeys#CryptoKeyVersionTemplate.FIELDS.protection_level
+    .. _state: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.importJobs#ImportJob.FIELDS.state
+    .. _EXPIRED: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.importJobs#ImportJobState.ENUM_VALUES.EXPIRED
+    .. _ACTIVE: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.importJobs#ImportJobState.ENUM_VALUES.ACTIVE
+    .. _ImportMethod: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.importJobs#ImportMethod
+    .. _HSM: https://cloud.google.com/kms/docs/reference/rest/v1/ProtectionLevel#ENUM_VALUES.HSM
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
 
-            crypto_key_present:
-              gcp.cloudkms.crypto_key.present:
-              - primary:
-                  name: projects/project-name/locations/us-east1/keyRings/key-ring/cryptoKeys/key-1/cryptoKeyVersions/1
-              - purpose: ENCRYPT_DECRYPT
-              - labels:
-                  lbl_key_1: lbl-value-1
-              - version_template:
-                  algorithm: GOOGLE_SYMMETRIC_ENCRYPTION
-                  protection_level: SOFTWARE
-              - destroy_scheduled_duration: 86400s
-              - rotation_period: 31500001s
-              - next_rotation_time: "2024-10-02T15:01:23Z"
-              - resource_id: projects/project-name/locations/us-east1/keyRings/key-ring/cryptoKeys/key-1
-              - project_id: project-name
-              - location_id: us-east1
-              - key_ring_id: key-ring
-              - crypto_key_id: key-1
+            import_job_present:
+              gcp.cloudkms.import_job.present:
+                - import_method: RSA_OAEP_4096_SHA256
+                - protection_level: SOFTWARE
+                - project_id: project-name
+                - location_id: us-east1
+                - key_ring_id: key-ring-id
+                - import_job_id: import-job-id
+
     """
     result = {
         "result": True,
         "old_state": None,
         "new_state": None,
         "name": name,
         "comment": [],
     }
 
-    get_resource_only_with_resource_id = hub.OPT.idem.get(
-        "get_resource_only_with_resource_id", False
-    )
-
     if hub.tool.gcp.resource_prop_utils.properties_mismatch_resource_id(
         RESOURCE_TYPE_FULL,
         resource_id,
         {
             "project_id": project_id,
             "location_id": location_id,
             "key_ring_id": key_ring_id,
-            "crypto_key_id": crypto_key_id,
+            "import_job_id": import_job_id,
         },
     ):
         result["comment"].append(
             hub.tool.gcp.comment_utils.properties_mismatch_resource_id_comment(
                 RESOURCE_TYPE_FULL, name
             )
         )
 
+    get_resource_only_with_resource_id = hub.OPT.idem.get(
+        "get_resource_only_with_resource_id", False
+    )
     if resource_id:
-        old_get_ret = await hub.exec.gcp.cloudkms.crypto_key.get(
+        old_get_ret = await hub.exec.gcp.cloudkms.import_job.get(
             ctx, resource_id=resource_id
         )
 
         if not old_get_ret["result"] or (
             not old_get_ret["ret"] and get_resource_only_with_resource_id
         ):
             result["result"] = False
@@ -254,213 +219,127 @@
     elif not get_resource_only_with_resource_id:
         resource_id = hub.tool.gcp.resource_prop_utils.construct_resource_id(
             RESOURCE_TYPE_FULL,
             {
                 "project_id": project_id,
                 "location_id": location_id,
                 "key_ring_id": key_ring_id,
-                "crypto_key_id": crypto_key_id,
+                "import_job_id": import_job_id,
             },
         )
-        old_get_ret = await hub.exec.gcp.cloudkms.crypto_key.get(
+        old_get_ret = await hub.exec.gcp.cloudkms.import_job.get(
             ctx, resource_id=resource_id
         )
 
         if not old_get_ret["result"]:
             result["result"] = False
             result["comment"] += old_get_ret["comment"]
             return result
 
         if old_get_ret["ret"]:
             result["old_state"] = old_get_ret["ret"]
 
-    if not result["old_state"]:
-        resource_body = {
-            "purpose": purpose,
-            "next_rotation_time": next_rotation_time,
-            "version_template": version_template,
-            "labels": labels,
-            "import_only": import_only,
-            "destroy_scheduled_duration": destroy_scheduled_duration,
-            "crypto_key_backend": crypto_key_backend,
-            "rotation_period": rotation_period,
-        }
-    else:
-        resource_body = {
-            "next_rotation_time": next_rotation_time,
-            "version_template": version_template,
-            "labels": hub.tool.gcp.cloudkms.patch.merge_labels(
-                labels, result["old_state"].get("labels")
-            ),
-            "rotation_period": rotation_period,
-        }
-
-    resource_body = {k: v for (k, v) in resource_body.items() if v is not None}
-
     if result["old_state"]:
         resource_id = result["old_state"].get("resource_id", None)
-        update_mask = hub.tool.gcp.cloudkms.patch.calc_update_mask(
-            resource_body, result["old_state"]
+        els = hub.tool.gcp.resource_prop_utils.get_elements_from_resource_id(
+            RESOURCE_TYPE_FULL, resource_id
         )
-        if (
-            primary
-            and primary.get("name")
-            and primary["name"]
-            != (result["old_state"].get("primary") or {}).get("name")
-        ):
-            update_primary_version = True
-        else:
-            update_primary_version = False
-
-        if ctx["test"]:
-            if update_mask or update_primary_version:
-                result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
-                    {**result["old_state"], **resource_body}
-                )
-                result["comment"].append(
-                    hub.tool.gcp.comment_utils.would_update_comment(
-                        GCP_RESOURCE_TYPE_FULL, resource_id
-                    )
-                )
-            else:
+        if project_id and location_id and key_ring_id and import_job_id:
+            if (
+                els.get("project_id") != project_id
+                or els.get("location_id") != location_id
+                or els.get("key_ring_id") != key_ring_id
+                or els.get("import_job_id") != import_job_id
+            ):
+                result["result"] = False
                 result["comment"].append(
-                    hub.tool.gcp.comment_utils.up_to_date_comment(
-                        GCP_RESOURCE_TYPE_FULL, resource_id
+                    hub.tool.gcp.comment_utils.non_updatable_properties_comment(
+                        "gcp.cloudkms.import_job",
+                        resource_id,
+                        ["project_id", "location_id", "key_ring_id", "import_job_id"],
                     )
                 )
-            return result
+                return result
 
-        els = hub.tool.gcp.resource_prop_utils.get_elements_from_resource_id(
-            RESOURCE_TYPE_FULL, resource_id
-        )
         if (
-            els.get("project_id") != project_id
-            or els.get("location_id") != location_id
-            or els.get("key_ring_id") != key_ring_id
-            or els.get("crypto_key_id") != crypto_key_id
+            result["old_state"].get("import_method") != import_method
+            or result["old_state"].get("protection_level") != protection_level
         ):
             result["result"] = False
             result["comment"].append(
-                hub.tool.gcp.comment_utils.non_updatable_properties_comment(
-                    GCP_RESOURCE_TYPE_FULL,
-                    resource_id,
-                    ["project_id", "location_id", "key_ring_id", "crypto_key_id"],
+                hub.tool.gcp.comment_utils.no_resource_update_comment(
+                    "gcp.cloudkms.import_job", resource_id
                 )
             )
-            return result
-
-        if update_mask:
-            update_ret = await hub.exec.gcp_api.client.cloudkms.projects.locations.key_rings.crypto_keys.patch(
-                ctx, name_=resource_id, updateMask=update_mask, body=resource_body
+        else:
+            result["comment"].append(
+                hub.tool.gcp.comment_utils.already_exists_comment(
+                    "gcp.cloudkms.import_job", resource_id
+                )
             )
-            if not update_ret["result"]:
-                result["result"] = False
-                result["comment"] += update_ret["comment"]
-                return result
+            result["new_state"] = result["old_state"]
+
+        return result
 
-            result["new_state"] = {
+    resource_body = {
+        "importMethod": import_method,
+        "protectionLevel": protection_level,
+    }
+
+    if ctx["test"]:
+        result["comment"].append(
+            hub.tool.gcp.comment_utils.would_create_comment(
+                "gcp.cloudkms.import_job", resource_id
+            )
+        )
+        result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
+            {
+                "resource_id": resource_id,
                 "name": name,
                 "project_id": project_id,
                 "location_id": location_id,
                 "key_ring_id": key_ring_id,
-                "crypto_key_id": crypto_key_id,
-                **update_ret["ret"],
+                "import_job_id": import_job_id,
+                **resource_body,
             }
+        )
+        return result
 
-        if update_primary_version:
-            els = hub.tool.gcp.resource_prop_utils.get_elements_from_resource_id(
-                "cloudkms.projects.locations.key_rings.crypto_keys.crypto_key_versions",
-                primary["name"],
-            )
-            update_version_ret = await hub.exec.gcp_api.client.cloudkms.projects.locations.key_rings.crypto_keys.updatePrimaryVersion(
-                ctx,
-                name_=resource_id,
-                body={"cryptoKeyVersionId": els["crypto_key_version_id"]},
-            )
-            if not update_version_ret["result"]:
-                result["result"] = False
-                result["comment"] += update_version_ret["comment"]
-                return result
-
-            result["new_state"] = {
-                "name": name,
+    create_ret = await hub.exec.gcp_api.client.cloudkms.projects.locations.key_rings.import_jobs.create(
+        ctx,
+        parent=hub.tool.gcp.resource_prop_utils.construct_resource_id(
+            "cloudkms.projects.locations.key_rings",
+            {
                 "project_id": project_id,
                 "location_id": location_id,
                 "key_ring_id": key_ring_id,
-                "crypto_key_id": crypto_key_id,
-                "primary": update_version_ret["ret"]["primary"],
-            }
+            },
+        ),
+        body=resource_body,
+        import_job_id=import_job_id,
+    )
 
-        if update_mask or update_primary_version:
-            result["comment"].append(
-                hub.tool.gcp.comment_utils.update_comment(
-                    GCP_RESOURCE_TYPE_FULL, resource_id
-                )
-            )
-        else:
-            result["comment"].append(
-                hub.tool.gcp.comment_utils.up_to_date_comment(
-                    GCP_RESOURCE_TYPE_FULL, resource_id
-                )
-            )
+    if not create_ret["result"]:
+        result["result"] = False
+        result["comment"] += create_ret["comment"]
         return result
-
-    else:
-        if ctx["test"]:
-            result["comment"].append(
-                hub.tool.gcp.comment_utils.would_create_comment(
-                    GCP_RESOURCE_TYPE_FULL, name
-                )
-            )
-            result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
-                {
-                    "resource_id": resource_id,
-                    "name": name,
-                    "project_id": project_id,
-                    "location_id": location_id,
-                    "key_ring_id": key_ring_id,
-                    "crypto_key_id": crypto_key_id,
-                    **resource_body,
-                }
-            )
-            return result
-
-        create_ret = await hub.exec.gcp_api.client.cloudkms.projects.locations.key_rings.crypto_keys.create(
-            ctx,
-            parent=hub.tool.gcp.resource_prop_utils.construct_resource_id(
-                "cloudkms.projects.locations.key_rings",
-                {
-                    "project_id": project_id,
-                    "location_id": location_id,
-                    "key_ring_id": key_ring_id,
-                },
-            ),
-            body=resource_body,
-            crypto_key_id=crypto_key_id,
-            skip_initial_version_creation=False,
+    result["comment"].append(
+        hub.tool.gcp.comment_utils.create_comment(
+            "gcp.cloudkms.import_job", resource_id
         )
-        if not create_ret["result"]:
-            result["result"] = False
-            result["comment"] += create_ret["comment"]
-            return result
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.create_comment(
-                GCP_RESOURCE_TYPE_FULL, resource_id
-            )
-        )
-        result["new_state"] = {
-            "name": name,
-            "project_id": project_id,
-            "location_id": location_id,
-            "key_ring_id": key_ring_id,
-            "crypto_key_id": crypto_key_id,
-            **create_ret["ret"],
-        }
-        result["old_state"] = {}
-        return result
+    )
+    result["new_state"] = {
+        "name": name,
+        "project_id": project_id,
+        "location_id": location_id,
+        "key_ring_id": key_ring_id,
+        "import_job_id": import_job_id,
+        **create_ret["ret"],
+    }
+    return result
 
 
 async def absent(hub, ctx, name: str) -> Dict[str, Any]:
     """Absent is not supported for this resource.
 
     Args:
         name(str):
@@ -477,34 +356,34 @@
             }
     """
     return {
         "name": name,
         "result": False,
         "comment": [
             hub.tool.gcp.comment_utils.no_resource_delete_comment(
-                GCP_RESOURCE_TYPE_FULL
+                "gcp.cloudkms.import_job"
             )
         ],
         "old_state": None,
         "new_state": None,
     }
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
     """Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
-    Retrieve the list of available crypto keys.
+    Retrieve the list of available import jobs.
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: bash
 
-            $ idem describe gcp.cloudkms.crypto_key
+            $ idem describe gcp.cloudkms.import_job
     """
     result = {}
 
     locations = await hub.exec.gcp.cloudkms.location.list(
         ctx, project=ctx.acct.project_id
     )
     if not locations["result"]:
@@ -519,39 +398,41 @@
         )
         if not key_rings["result"]:
             hub.log.warning(
                 f"Could not list gcp.cloudkms.key_ring in {location['location_id']} {key_rings['comment']}"
             )
         else:
             for key_ring in key_rings["ret"]:
-                crypto_keys = await hub.exec.gcp.cloudkms.crypto_key.list(
+                import_jobs = await hub.exec.gcp.cloudkms.import_job.list(
                     ctx, key_ring=key_ring["resource_id"]
                 )
-                if not crypto_keys["result"]:
+                if not import_jobs["result"]:
                     hub.log.debug(
-                        f"Could not describe gcp.cloudkms.crypto_key in {key_ring['resource_id']} {key_rings['comment']}"
+                        f"Could not describe gcp.cloudkms.import_job in {key_ring['resource_id']} {key_rings['comment']}"
                     )
                 else:
-                    for crypto_key in crypto_keys["ret"]:
-                        resource_id = crypto_key["resource_id"]
+                    for import_job in import_jobs["ret"]:
+                        resource_id = import_job["resource_id"]
                         result[resource_id] = {
-                            "gcp.cloudkms.crypto_key.present": [
+                            "gcp.cloudkms.import_job.present": [
                                 {parameter_key: parameter_value}
-                                for parameter_key, parameter_value in crypto_key.items()
+                                if parameter_key != "state"
+                                else {"job_state": parameter_value}
+                                for parameter_key, parameter_value in import_job.items()
                             ]
                         }
                         els = hub.tool.gcp.resource_prop_utils.get_elements_from_resource_id(
                             RESOURCE_TYPE_FULL,
                             resource_id,
                         )
-                        p = result[resource_id]["gcp.cloudkms.crypto_key.present"]
+                        p = result[resource_id]["gcp.cloudkms.import_job.present"]
                         p.append({"project_id": els["project_id"]})
                         p.append({"location_id": els["location_id"]})
                         p.append({"key_ring_id": els["key_ring_id"]})
-                        p.append({"crypto_key_id": els["crypto_key_id"]})
+                        p.append({"import_job_id": els["import_job_id"]})
 
     return result
 
 
 def is_pending(hub, ret: dict, state: str = None, **pending_kwargs) -> bool:
     """Default implemented for each module."""
     return hub.tool.gcp.utils.is_pending(ret=ret, state=state, **pending_kwargs)
```

### Comparing `idem_gcp-1.1.0/idem_gcp/states/gcp/cloudkms/crypto_key_version.py` & `idem_gcp-1.2.0/idem_gcp/states/gcp/cloudkms/crypto_key_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,23 @@
             A timestamp in RFC3339 UTC "Zulu" format, with nanosecond resolution and up to nine fractional digits.
             Examples: "2014-10-02T15:01:23Z" and "2014-10-02T15:01:23.045123456Z".
 
         import_job(str, Optional):
             Output only. The name of the `ImportJob`_ used in the most recent import of this `CryptoKeyVersion`_. Only
             present if the underlying key material was imported.
 
+        external_protection_level_options(ExternalProtectionLevelOptions, Optional):
+            ExternalProtectionLevelOptions stores a group of additional fields for configuring a CryptoKeyVersion that are specific to the EXTERNAL protection level and EXTERNAL_VPC protection levels.
+            * external_key_uri(str, Optional):
+                The URI for an external resource that this CryptoKeyVersion represents.
+
+            * ekm_connection_key_path(str, Optional):
+                The path to the external key material on the EKM when using EkmConnection e.g.,
+                "v0/my/key". Set this field instead of external_key_uri when using an EkmConnection.
+
         resource_id(str, Optional): Idem resource id. Formatted as
 
             `projects/{project_id}/locations/{location_id}/keyRings/{key_ring_id}/cryptoKeys/{crypto_key_id}/cryptoKeyVersions/{crypto_key_version_id}`
 
         key_material(str, Optional): Base64 encoded key material. If this parameter is present will be attempted `import`_
             of the key material in the `CryptoKeyVersion`_ specified by the resource_id or in a new `CryptoKeyVersion`_
             if resource_id is missing. `import`_ requires also project_id, location_id, key_ring_id, crypto_key_id,
@@ -511,17 +520,18 @@
 
         key_ring_id(str, Optional):
             Keyring Id of the new crypto key version.
 
         crypto_key_id(str, Optional):
             Cryptokey Id of the new crypto key version.
 
-        resource_id(str, Optional): Idem resource id. Formatted as
-
+        resource_id(str, Optional):
+            Idem resource id. Formatted as
             `projects/{project_id}/locations/{location_id}/keyRings/{key_ring_id}/cryptoKeys/{crypto_key_id}/cryptoKeyVersions/{crypto_key_version_id}`
+
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
 
             {% set project_id = 'tango-gcp' %}
```

### Comparing `idem_gcp-1.1.0/idem_gcp/states/gcp/cloudkms/import_job.py` & `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/instance_group.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,414 +1,352 @@
-"""State module for managing Cloud Key Management Service import job."""
+"""State module for managing InstanceGroups."""
+
+__contracts__ = ["resource"]
+
 from dataclasses import field
 from dataclasses import make_dataclass
 from typing import Any
 from typing import Dict
 from typing import List
 
+from idem_gcp.tool.gcp.state_operation_utils import StateOperations
+from idem_gcp.tool.gcp.utils import zonal_absent
+
+# prevent commit hook from removing the import
+absent = zonal_absent
+
 __contracts__ = ["resource"]
-RESOURCE_TYPE = "cloudkms.import_jobs"
-RESOURCE_TYPE_FULL = "cloudkms.projects.locations.key_rings.import_jobs"
-GCP_RESOURCE_TYPE_FULL = "gcp.cloudkms.import_jobs"
 
 
 async def present(
     hub,
     ctx,
-    name: str,
-    import_method: str,
-    protection_level: str,
-    import_job_id: str = None,
-    project_id: str = None,
-    location_id: str = None,
-    key_ring_id: str = None,
-    create_time: str = None,
-    generate_time: str = None,
-    expire_time: str = None,
-    expire_event_time: str = None,
-    job_state: str = None,
-    public_key: str = None,
-    attestation: make_dataclass(
-        "KeyOperationAttestation",
-        [
-            ("format", str, field(default=None)),
-            ("content", str, field(default=None)),
-            (
-                "cert_chains",
-                make_dataclass(
-                    "CertificateChains",
-                    [
-                        ("cavium_certs", List[str], field(default=None)),
-                        (
-                            "google_card_certs",
-                            List[str],
-                            field(default=None),
-                        ),
-                        (
-                            "google_partition_certs",
-                            List[str],
-                            field(default=None),
-                        ),
-                    ],
-                ),
-                field(default=None),
-            ),
-        ],
-    ) = None,
+    name: str = None,
+    zone: str = None,
+    project: str = None,
+    description: str = None,
+    fingerprint: str = None,
+    subnetwork: str = None,
+    network: str = None,
+    named_ports: List[
+        make_dataclass(
+            "NamedPort",
+            [("name", str, field(default=None)), ("port", int, field(default=None))],
+        )
+    ] = None,
+    request_id: str = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
-    """Create a new `ImportJob`_ within a `KeyRing`_.
+    r"""Create or update an instance group.
+
+    Creates an instance group in the specified project using the parameters that are included in the request.
 
     Args:
         name(str):
-            Idem name.
-
-        import_job_id(str, Optional):
-            Import job id. It must be unique within a KeyRing and match the regular expression ``[a-zA-Z0-9_-]{1,63}``
-
-        project_id(str, Optional):
-            Project Id of the new crypto key.
-
-        location_id(str, Optional):
-            Location Id of the new crypto key.
-
-        key_ring_id(str, Optional):
-            Keyring Id of the new crypto key.
-
-        import_method(str):
-            Immutable. The wrapping method to be used for incoming key material. See `ImportMethod`_.
-
-        protection_level(str):
-            Immutable. The protection level of the `ImportJob`_. This must match the `protectionLevel`_ of the
-            `versionTemplate`_ on the `CryptoKey`_ you attempt to import into.
+            An Idem name of the resource.
 
-        create_time(str, Optional):
-            Output only. The time at which this `ImportJob`_ was created.
+        description(str, Optional):
+            An optional description of this resource. Provide this property when you create the resource. Defaults to None.
 
-            A timestamp in RFC3339 UTC "Zulu" format, with nanosecond resolution and up to nine fractional digits.
-            Examples: "2014-10-02T15:01:23Z" and "2014-10-02T15:01:23.045123456Z".
+        zone(str):
+            The name of the zone where the instance group is located.
 
-        generate_time(str, Optional):
-            Output only. The time this `ImportJob`_'s key material was generated.
+        fingerprint(str, Optional):
+            The fingerprint of the named ports. The system uses this fingerprint to detect conflicts when multiple users change the named ports concurrently. Defaults to None.
 
-            A timestamp in RFC3339 UTC "Zulu" format, with nanosecond resolution and up to nine fractional digits.
-            Examples: "2014-10-02T15:01:23Z" and "2014-10-02T15:01:23.045123456Z".
+        network(str, Optional):
+            The URL of the network to which all instances in the instance group belong. If your instance has multiple network interfaces, then the network and subnetwork fields only refer to the network and subnet used by your primary interface (nic0). Defaults to None.
 
-        expire_time(str, Optional):
-            Output only. The time at which this `ImportJob`_ is scheduled for expiration and can no longer be used to
-            import key material.
+        subnetwork(str, Optional):
+            The URL of the subnetwork to which all instances in the instance group belong. If your instance has multiple network interfaces, then the network and subnetwork fields only refer to the network and subnet used by your primary interface (nic0). Defaults to None.
 
-            A timestamp in RFC3339 UTC "Zulu" format, with nanosecond resolution and up to nine fractional digits.
-            Examples: "2014-10-02T15:01:23Z" and "2014-10-02T15:01:23.045123456Z".
+        named_ports(List[Dict[str, Any]], Optional):
+            Assigns a name to a port number. For example: {name: "http", port: 80} This allows the system to reference ports by the assigned name instead of a port number. Named ports can also contain multiple ports. For example: [{name: "app1", port: 8080}, {name: "app1", port: 8081}, {name: "app2", port: 8082}] Named ports apply to all instances in this instance group. . Defaults to None.
+                * name(str, Optional):
+                    The name for this named port. The name must be 1-63 characters long, and comply with RFC1035.
+                * port(int, Optional):
+                    The port number, which can be a value between 1 and 65535.
 
-        expire_event_time(str, Optional):
-            Output only. The time this `ImportJob`_ expired. Only present if `state`_ is `EXPIRED`_.
+        project(str):
+            Project ID for this request.
 
-            A timestamp in RFC3339 UTC "Zulu" format, with nanosecond resolution and up to nine fractional digits.
-            Examples: "2014-10-02T15:01:23Z" and "2014-10-02T15:01:23.045123456Z".
+        request_id(str, Optional):
+            An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000). Defaults to None.
 
-        job_state(str, Optional):
-            Output only. The current state of the `ImportJob`_, indicating if it can be used.
-
-        public_key(str, Optional):
-            Output only. The public key with which to wrap key material prior to import. Only returned if `state`_ is
-             `ACTIVE`_.
-
-        attestation(Dict[str, Any], Optional):
-            Output only. Statement that was generated and signed by the key creator (for example, an HSM) at key
-            creation time. Use this statement to verify attributes of the key as stored on the HSM, independently of
-            Google. Only present if the chosen `ImportMethod`_ is one with a protection level of `HSM`_.
-
-        resource_id(str, Optional): Idem resource id. Formatted as
-
-            `projects/{project_id}/locations/{location_id}/keyRings/{key_ring_id}/importJobs/{import_job_id}`
-
-    .. _ImportJob: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.importJobs#ImportJob
-    .. _KeyRing: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings#KeyRing
-    .. _Labeling Keys: https://cloud.google.com/kms/docs/labeling-keys
-    .. _ProtectionLevel: https://cloud.google.com/kms/docs/reference/rest/v1/ProtectionLevel
-    .. _ImportMethod: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.importJobs#ImportMethod
-    .. _CryptoKey: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.cryptoKeys#CryptoKey
-    .. _versionTemplate: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.cryptoKeys#CryptoKey.FIELDS.version_template
-    .. _protectionLevel: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.cryptoKeys#CryptoKeyVersionTemplate.FIELDS.protection_level
-    .. _state: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.importJobs#ImportJob.FIELDS.state
-    .. _EXPIRED: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.importJobs#ImportJobState.ENUM_VALUES.EXPIRED
-    .. _ACTIVE: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.importJobs#ImportJobState.ENUM_VALUES.ACTIVE
-    .. _ImportMethod: https://cloud.google.com/kms/docs/reference/rest/v1/projects.locations.keyRings.importJobs#ImportMethod
-    .. _HSM: https://cloud.google.com/kms/docs/reference/rest/v1/ProtectionLevel#ENUM_VALUES.HSM
+        resource_id(str, Optional):
+            An identifier of the resource in the provider. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
 
-            import_job_present:
-              gcp.cloudkms.import_job.present:
-                - import_method: RSA_OAEP_4096_SHA256
-                - protection_level: SOFTWARE
-                - project_id: project-name
-                - location_id: us-east1
-                - key_ring_id: key-ring-id
-                - import_job_id: import-job-id
-
+            resource_is_present:
+              gcp.compute.instance_groups.present:
+                - name: value
+                - zone: value
+                - project: value
+                - instance_group: value
     """
     result = {
         "result": True,
         "old_state": None,
         "new_state": None,
         "name": name,
         "comment": [],
     }
 
-    if hub.tool.gcp.resource_prop_utils.properties_mismatch_resource_id(
-        RESOURCE_TYPE_FULL,
-        resource_id,
-        {
-            "project_id": project_id,
-            "location_id": location_id,
-            "key_ring_id": key_ring_id,
-            "import_job_id": import_job_id,
-        },
-    ):
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.properties_mismatch_resource_id_comment(
-                RESOURCE_TYPE_FULL, name
-            )
-        )
+    project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
-    get_resource_only_with_resource_id = hub.OPT.idem.get(
-        "get_resource_only_with_resource_id", False
-    )
-    if resource_id:
-        old_get_ret = await hub.exec.gcp.cloudkms.import_job.get(
-            ctx, resource_id=resource_id
-        )
+    if ctx.get("wrapper_result"):
+        result = ctx.get("wrapper_result")
 
-        if not old_get_ret["result"] or (
-            not old_get_ret["ret"] and get_resource_only_with_resource_id
-        ):
-            result["result"] = False
-            result["comment"] += old_get_ret["comment"]
-            return result
+    resource_body = {
+        "description": description,
+        "zone": zone,
+        "name": name,
+        "named_ports": named_ports,
+        "network": network,
+        "subnetwork": subnetwork,
+    }
 
-        result["old_state"] = old_get_ret["ret"]
-    elif not get_resource_only_with_resource_id:
-        resource_id = hub.tool.gcp.resource_prop_utils.construct_resource_id(
-            RESOURCE_TYPE_FULL,
-            {
-                "project_id": project_id,
-                "location_id": location_id,
-                "key_ring_id": key_ring_id,
-                "import_job_id": import_job_id,
-            },
-        )
-        old_get_ret = await hub.exec.gcp.cloudkms.import_job.get(
-            ctx, resource_id=resource_id
+    resource_body = {k: v for (k, v) in resource_body.items() if v is not None}
+    operation = None
+    if result["old_state"]:
+        resource_id = result["old_state"].get("resource_id", None)
+        resource_body["resource_id"] = resource_id
+
+        # The fingerprint is required upon an update operation but in the time of creation the
+        # resource still do not have fingerprint so, we cannot make it a required param for present method.
+        resource_body["fingerprint"] = fingerprint or result["old_state"].get(
+            "fingerprint"
         )
 
-        if not old_get_ret["result"]:
-            result["result"] = False
-            result["comment"] += old_get_ret["comment"]
-            return result
+        # A dictionary of additional operations to perform on the object identified by the key
+        # the values are tuples with the first element - the method to call, the second element - arguments,
+        # third - the property is required in the end result
+        patch_operations_dict = {
+            "named_ports": (
+                hub.tool.gcp.compute.instance_group.update_named_ports,
+                (ctx, result["old_state"], named_ports),
+                True,
+            ),
+        }
 
-        if old_get_ret["ret"]:
-            result["old_state"] = old_get_ret["ret"]
+        state_operations = StateOperations(
+            hub, "compute.instance_group", patch_operations_dict, result, resource_body
+        )
 
-    if result["old_state"]:
-        resource_id = result["old_state"].get("resource_id", None)
-        els = hub.tool.gcp.resource_prop_utils.get_elements_from_resource_id(
-            RESOURCE_TYPE_FULL, resource_id
+        changes = hub.tool.gcp.utils.compare_states(
+            result["old_state"],
+            {
+                **resource_body,
+            },
+            "compute.instance_group",
+            additional_exclude_paths=list(patch_operations_dict.keys()),
         )
-        if project_id and location_id and key_ring_id and import_job_id:
-            if (
-                els.get("project_id") != project_id
-                or els.get("location_id") != location_id
-                or els.get("key_ring_id") != key_ring_id
-                or els.get("import_job_id") != import_job_id
-            ):
+
+        if changes:
+            changed_non_updatable_properties = (
+                hub.tool.gcp.resource_prop_utils.get_changed_non_updatable_properties(
+                    "compute.instance_group", changes
+                )
+            )
+            if changed_non_updatable_properties:
                 result["result"] = False
                 result["comment"].append(
                     hub.tool.gcp.comment_utils.non_updatable_properties_comment(
-                        "gcp.cloudkms.import_job",
-                        resource_id,
-                        ["project_id", "location_id", "key_ring_id", "import_job_id"],
+                        "gcp.compute.instance_group",
+                        name,
+                        changed_non_updatable_properties,
                     )
                 )
+                result["new_state"] = result["old_state"]
                 return result
 
-        if (
-            result["old_state"].get("import_method") != import_method
-            or result["old_state"].get("protection_level") != protection_level
-        ):
-            result["result"] = False
+        if not changes and not any(state_operations.changed_properties_dict.values()):
             result["comment"].append(
-                hub.tool.gcp.comment_utils.no_resource_update_comment(
-                    "gcp.cloudkms.import_job", resource_id
+                hub.tool.gcp.comment_utils.up_to_date_comment(
+                    "gcp.compute.instance_group", name
                 )
             )
-        else:
+            result["new_state"] = result["old_state"]
+            return result
+
+        if ctx["test"]:
             result["comment"].append(
-                hub.tool.gcp.comment_utils.already_exists_comment(
-                    "gcp.cloudkms.import_job", resource_id
+                hub.tool.gcp.comment_utils.would_update_comment(
+                    "gcp.compute.instance_group", name
                 )
             )
-            result["new_state"] = result["old_state"]
+            result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
+                resource_body
+            )
+            return result
 
-        return result
+        state_operations_ret = await state_operations.run_operations()
 
-    resource_body = {
-        "importMethod": import_method,
-        "protectionLevel": protection_level,
-    }
+        if not state_operations_ret["result"] or not state_operations_ret.get(
+            "new_state"
+        ):
+            result["result"] = False
+            result["comment"] += state_operations_ret["comment"]
+            return result
 
-    if ctx["test"]:
+        result["new_state"] = state_operations_ret["new_state"]
         result["comment"].append(
-            hub.tool.gcp.comment_utils.would_create_comment(
-                "gcp.cloudkms.import_job", resource_id
+            hub.tool.gcp.comment_utils.update_comment(
+                "gcp.compute.instance_group", name
             )
         )
-        result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
-            {
-                "resource_id": resource_id,
-                "name": name,
-                "project_id": project_id,
-                "location_id": location_id,
-                "key_ring_id": key_ring_id,
-                "import_job_id": import_job_id,
-                **resource_body,
-            }
-        )
         return result
 
-    create_ret = await hub.exec.gcp_api.client.cloudkms.projects.locations.key_rings.import_jobs.create(
-        ctx,
-        parent=hub.tool.gcp.resource_prop_utils.construct_resource_id(
-            "cloudkms.projects.locations.key_rings",
-            {
-                "project_id": project_id,
-                "location_id": location_id,
-                "key_ring_id": key_ring_id,
-            },
-        ),
-        body=resource_body,
-        import_job_id=import_job_id,
-    )
+    else:
+        # Create for test
+        if ctx.get("test", False):
+            result["comment"].append(
+                hub.tool.gcp.comment_utils.would_create_comment(
+                    "gcp.compute.instance_group", name
+                )
+            )
+            result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
+                resource_body
+            )
+            result["new_state"][
+                "resource_id"
+            ] = hub.tool.gcp.resource_prop_utils.construct_resource_id(
+                "compute.instance_group", {**locals(), "instanceGroup": name}
+            )
+            return result
 
-    if not create_ret["result"]:
-        result["result"] = False
-        result["comment"] += create_ret["comment"]
-        return result
-    result["comment"].append(
-        hub.tool.gcp.comment_utils.create_comment(
-            "gcp.cloudkms.import_job", resource_id
+        # Create
+        create_ret = await hub.exec.gcp_api.client.compute.instance_group.insert(
+            ctx,
+            name=name,
+            project=project,
+            zone=zone,
+            request_id=request_id,
+            body=resource_body,
         )
-    )
-    result["new_state"] = {
-        "name": name,
-        "project_id": project_id,
-        "location_id": location_id,
-        "key_ring_id": key_ring_id,
-        "import_job_id": import_job_id,
-        **create_ret["ret"],
-    }
+        if not create_ret["result"] or not create_ret["ret"]:
+            result["result"] = False
+            if create_ret["comment"] and next(
+                (
+                    comment
+                    for comment in create_ret["comment"]
+                    if "alreadyExists" in comment
+                ),
+                None,
+            ):
+                result["comment"].append(
+                    hub.tool.gcp.comment_utils.already_exists_comment(
+                        "gcp.compute.instance_group", name
+                    )
+                )
+            else:
+                result["comment"] += create_ret["comment"]
+            return result
+
+        if hub.tool.gcp.operation_utils.is_operation(create_ret["ret"]):
+            operation = create_ret["ret"]
+
+    if operation:
+        operation_id = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
+            operation.get("selfLink"), "compute.zone_operation"
+        )
+        result["rerun_data"] = {
+            "operation_id": operation_id,
+            "old_state": result["old_state"],
+        }
+
     return result
 
 
-async def absent(hub, ctx, name: str) -> Dict[str, Any]:
-    """Absent is not supported for this resource.
+async def absent(
+    hub,
+    ctx,
+    name: str = None,
+    project: str = None,
+    zone: str = None,
+    request_id: str = None,
+    resource_id: str = None,
+) -> Dict[str, Any]:
+    r"""Deletes the specified instance group.
+
+    The instances in the group are not deleted. Note that instance group must not belong to a backend service. Read Deleting an instance group for more information.
 
     Args:
         name(str):
-            Idem name
+            An Idem name of the resource.
+
+        project(str):
+            Project ID for this request.
+
+        request_id(str, Optional):
+            An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000). Defaults to None.
+
+        zone(str):
+            The name of the zone where the instance group is located.
+
+        resource_id(str, Optional):
+            An identifier of the resource in the provider. Defaults to None.
 
     Returns:
-        .. code-block:: json
+        Dict[str, Any]
 
-            {
-                "result": False,
-                "comment": "...",
-                "old_state": None,
-                "new_state": None,
-            }
+
+    Examples:
+        .. code-block:: sls
+
+            resource_is_absent:
+              gcp.compute.instance_groups.absent:
+                - name: value
+                - project: value
+                - instance_group: value
+                - zone: value
     """
-    return {
-        "name": name,
-        "result": False,
-        "comment": [
-            hub.tool.gcp.comment_utils.no_resource_delete_comment(
-                "gcp.cloudkms.import_job"
-            )
-        ],
-        "old_state": None,
-        "new_state": None,
-    }
+    # the method is handled via the recursive_contracts->call_absent
+    raise NotImplementedError
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
-    """Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
+    r"""Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
-    Retrieve the list of available import jobs.
+    Retrieves the list of zonal instance group resources contained within the specified zone. For managed instance groups, use the instanceGroupManagers or regionInstanceGroupManagers methods instead.
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: bash
 
-            $ idem describe gcp.cloudkms.import_job
+            $ idem describe gcp.compute.instance_groups
     """
     result = {}
 
-    locations = await hub.exec.gcp.cloudkms.location.list(
+    describe_ret = await hub.exec.gcp.compute.instance_group.list(
         ctx, project=ctx.acct.project_id
     )
-    if not locations["result"]:
-        hub.log.warning(
-            f"Could not list gcp.cloudkms.crypto_key in {ctx.acct.project_id} {locations['comment']}"
+
+    if not describe_ret["result"]:
+        hub.log.debug(
+            f"Could not describe gcp.compute.instance_group {describe_ret['comment']}"
         )
         return {}
 
-    for location in locations["ret"]:
-        key_rings = await hub.exec.gcp.cloudkms.key_ring.list(
-            ctx, location=location["resource_id"]
-        )
-        if not key_rings["result"]:
-            hub.log.warning(
-                f"Could not list gcp.cloudkms.key_ring in {location['location_id']} {key_rings['comment']}"
-            )
-        else:
-            for key_ring in key_rings["ret"]:
-                import_jobs = await hub.exec.gcp.cloudkms.import_job.list(
-                    ctx, key_ring=key_ring["resource_id"]
-                )
-                if not import_jobs["result"]:
-                    hub.log.debug(
-                        f"Could not describe gcp.cloudkms.import_job in {key_ring['resource_id']} {key_rings['comment']}"
-                    )
-                else:
-                    for import_job in import_jobs["ret"]:
-                        resource_id = import_job["resource_id"]
-                        result[resource_id] = {
-                            "gcp.cloudkms.import_job.present": [
-                                {parameter_key: parameter_value}
-                                if parameter_key != "state"
-                                else {"job_state": parameter_value}
-                                for parameter_key, parameter_value in import_job.items()
-                            ]
-                        }
-                        els = hub.tool.gcp.resource_prop_utils.get_elements_from_resource_id(
-                            RESOURCE_TYPE_FULL,
-                            resource_id,
-                        )
-                        p = result[resource_id]["gcp.cloudkms.import_job.present"]
-                        p.append({"project_id": els["project_id"]})
-                        p.append({"location_id": els["location_id"]})
-                        p.append({"key_ring_id": els["key_ring_id"]})
-                        p.append({"import_job_id": els["import_job_id"]})
+    for resource in describe_ret["ret"]:
+        resource_id = resource.get("resource_id")
+
+        result[resource_id] = {
+            "gcp.compute.instance_group.present": [
+                {parameter_key: parameter_value}
+                for parameter_key, parameter_value in resource.items()
+            ]
+        }
 
     return result
 
 
 def is_pending(hub, ret: dict, state: str = None, **pending_kwargs) -> bool:
     """Default implemented for each module."""
     return hub.tool.gcp.utils.is_pending(ret=ret, state=state, **pending_kwargs)
```

### Comparing `idem_gcp-1.1.0/idem_gcp/states/gcp/cloudkms/key_ring.py` & `idem_gcp-1.2.0/idem_gcp/states/gcp/cloudkms/key_ring.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,29 +16,28 @@
     project_id: str = None,
     location_id: str = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
     """Create a new KeyRing in a given Project and Location.
 
     Args:
-        name(str:
+        name(str):
             Idem name.
 
         key_ring_id(str, Optional):
             Key ring id.
 
-        project_id(str, Optional:
+        project_id(str, Optional):
             Project id.
 
         location_id(str, Optional):
             Location id.
 
-        resource_id:
+        resource_id(str, Optional):
             Idem resource id. Formatted as
-
             `projects/{project_id}/locations/{location_id}/keyRings/{key_ring_id}`
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
```

### Comparing `idem_gcp-1.1.0/idem_gcp/states/gcp/cloudkms/location.py` & `idem_gcp-1.2.0/idem_gcp/states/gcp/cloudkms/location.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     hub,
     ctx,
     name: str,
 ) -> Dict[str, Any]:
     """Present operation is not supported for this resource.
 
     Args:
-        name:
+        name(str):
             Idem name.
 
     Returns:
         .. code-block:: json
 
             {
                 "result": False,
```

### Comparing `idem_gcp-1.1.0/idem_gcp/states/gcp/compute/backend_service.py` & `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/backend_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,42 +270,51 @@
             Fingerprint of this resource. A hash of the contents stored in this object. This field is used in optimistic locking. This field will be ignored when inserting a BackendService. An up-to-date fingerprint must be provided in order to update the BackendService, otherwise the request will fail with error 412 conditionNotMet. To see the latest fingerprint, make a get() request to retrieve a BackendService. Defaults to None.
 
         health_checks(List[str], Optional):
             The list of URLs to the healthChecks, httpHealthChecks (legacy), or httpsHealthChecks (legacy) resource for health checking this backend service. Not all backend services support legacy health checks. See Load balancer guide. Currently, at most one health check can be specified for each backend service. Backend services with instance group or zonal NEG backends must have a health check. Backend services with internet or serverless NEG backends must not have a health check. Defaults to None.
 
         locality_lb_policy(str, Optional):
             The load balancing algorithm used within the scope of the locality. The possible values are: - ROUND_ROBIN: This is a simple policy in which each healthy backend is selected in round robin order. This is the default. - LEAST_REQUEST: An O(1) algorithm which selects two random healthy hosts and picks the host which has fewer active requests. - RING_HASH: The ring/modulo hash load balancer implements consistent hashing to backends. The algorithm has the property that the addition/removal of a host from a set of N hosts only affects 1/N of the requests. - RANDOM: The load balancer selects a random healthy host. - ORIGINAL_DESTINATION: Backend host is selected based on the client connection metadata, i.e., connections are opened to the same address as the destination address of the incoming connection before the connection was redirected to the load balancer. - MAGLEV: used as a drop in replacement for the ring hash load balancer. Maglev is not as stable as ring hash but has faster table lookup build times and host selection times. For more information about Maglev, see https://ai.google/research/pubs/pub44824 This field is applicable to either: - A regional backend service with the service_protocol set to HTTP, HTTPS, or HTTP2, and load_balancing_scheme set to INTERNAL_MANAGED. - A global backend service with the load_balancing_scheme set to INTERNAL_SELF_MANAGED. If sessionAffinity is not NONE, and this field is not set to MAGLEV or RING_HASH, session affinity settings will not take effect. Only ROUND_ROBIN and RING_HASH are supported when the backend service is referenced by a URL map that is bound to target gRPC proxy that has validateForProxyless field set to true.
-                Enum type. Allowed values:
+            Enum type. Allowed values:
                 "INVALID_LB_POLICY"
                 "LEAST_REQUEST" - An O(1) algorithm which selects two random healthy hosts and picks the host which has fewer active requests.
                 "MAGLEV" - This algorithm implements consistent hashing to backends. Maglev can be used as a drop in replacement for the ring hash load balancer. Maglev is not as stable as ring hash but has faster table lookup build times and host selection times. For more information about Maglev, see https://ai.google/research/pubs/pub44824
                 "ORIGINAL_DESTINATION" - Backend host is selected based on the client connection metadata, i.e., connections are opened to the same address as the destination address of the incoming connection before the connection was redirected to the load balancer.
                 "RANDOM" - The load balancer selects a random healthy host.
                 "RING_HASH" - The ring/modulo hash load balancer implements consistent hashing to backends. The algorithm has the property that the addition/removal of a host from a set of N hosts only affects 1/N of the requests.
                 "ROUND_ROBIN" - This is a simple policy in which each healthy backend is selected in round robin order. This is the default. Defaults to None.
 
-        circuit_breakers(Dict[str, Any], Optional): CircuitBreakers: Settings controlling the volume of requests, connections and retries to this backend service. Defaults to None.
+        circuit_breakers(Dict[str, Any], Optional):
+            CircuitBreakers: Settings controlling the volume of requests, connections and retries to this backend service. Defaults to None.
 
-            * max_requests_per_connection (int, Optional): Maximum requests for a single connection to the backend service. This parameter is respected by both the HTTP/1.1 and HTTP/2 implementations. If not specified, there is no limit. Setting this parameter to 1 will effectively disable keep alive. Not supported when the backend service is referenced by a URL map that is bound to target gRPC proxy that has validateForProxyless field set to true.
-            * max_connections (int, Optional): The maximum number of connections to the backend service. If not specified, there is no limit. Not supported when the backend service is referenced by a URL map that is bound to target gRPC proxy that has validateForProxyless field set to true.
-            * max_requests (int, Optional): The maximum number of parallel requests that allowed to the backend service. If not specified, there is no limit.
-            * max_retries (int, Optional): The maximum number of parallel retries allowed to the backend cluster. If not specified, the default is 1. Not supported when the backend service is referenced by a URL map that is bound to target gRPC proxy that has validateForProxyless field set to true.
-            * max_pending_requests (int, Optional): The maximum number of pending requests allowed to the backend service. If not specified, there is no limit. Not supported when the backend service is referenced by a URL map that is bound to target gRPC proxy that has validateForProxyless field set to true.
+            * max_requests_per_connection(int, Optional):
+                Maximum requests for a single connection to the backend service. This parameter is respected by both the HTTP/1.1 and HTTP/2 implementations. If not specified, there is no limit. Setting this parameter to 1 will effectively disable keep alive. Not supported when the backend service is referenced by a URL map that is bound to target gRPC proxy that has validateForProxyless field set to true.
+            * max_connections(int, Optional):
+                The maximum number of connections to the backend service. If not specified, there is no limit. Not supported when the backend service is referenced by a URL map that is bound to target gRPC proxy that has validateForProxyless field set to true.
+            * max_requests (int, Optional):
+                The maximum number of parallel requests that allowed to the backend service. If not specified, there is no limit.
+            * max_retries (int, Optional):
+                The maximum number of parallel retries allowed to the backend cluster. If not specified, the default is 1. Not supported when the backend service is referenced by a URL map that is bound to target gRPC proxy that has validateForProxyless field set to true.
+            * max_pending_requests (int, Optional):
+                The maximum number of pending requests allowed to the backend service. If not specified, there is no limit. Not supported when the backend service is referenced by a URL map that is bound to target gRPC proxy that has validateForProxyless field set to true.
 
         failover_policy(Dict[str, Any], Optional):
             Requires at least one backend instance group to be defined as a backup (failover) backend. For load balancers that have configurable failover: [Internal TCP/UDP Load Balancing](https://cloud.google.com/load-balancing/docs/internal/failover-overview) and [external TCP/UDP Load Balancing](https://cloud.google.com/load-balancing/docs/network/networklb-failover-overview).
             BackendServiceFailoverPolicy: For load balancers that have configurable failover: [Internal TCP/UDP Load Balancing](https://cloud.google.com/load-balancing/docs/internal/failover-overview) and [external TCP/UDP Load Balancing](https://cloud.google.com/load-balancing/docs/network/networklb-failover-overview). On failover or failback, this field indicates whether connection draining will be honored. Google Cloud has a fixed connection draining timeout of 10 minutes. A setting of true terminates existing TCP connections to the active pool during failover and failback, immediately draining traffic. A setting of false allows existing TCP connections to persist, even on VMs no longer in the active pool, for up to the duration of the connection draining timeout (10 minutes). Defaults to None.
 
-            * drop_traffic_if_unhealthy (bool, Optional): If set to true, connections to the load balancer are dropped when all primary and all backup backend VMs are unhealthy.If set to false, connections are distributed among all primary VMs when all primary and all backup backend VMs are unhealthy. For load balancers that have configurable failover: [Internal TCP/UDP Load Balancing](https://cloud.google.com/load-balancing/docs/internal/failover-overview) and [external TCP/UDP Load Balancing](https://cloud.google.com/load-balancing/docs/network/networklb-failover-overview). The default is false.
-            * disable_connection_drain_on_failover (bool, Optional): This can be set to true only if the protocol is TCP. The default is false.
-            * failover_ratio (float, Optional): The value of the field must be in the range [0, 1]. If the value is 0, the load balancer performs a failover when the number of healthy primary VMs equals zero. For all other values, the load balancer performs a failover when the total number of healthy primary VMs is less than this ratio. For load balancers that have configurable failover: [Internal TCP/UDP Load Balancing](https://cloud.google.com/load-balancing/docs/internal/failover-overview) and [external TCP/UDP Load Balancing](https://cloud.google.com/load-balancing/docs/network/networklb-failover-overview).
+            * drop_traffic_if_unhealthy (bool, Optional):
+                If set to true, connections to the load balancer are dropped when all primary and all backup backend VMs are unhealthy.If set to false, connections are distributed among all primary VMs when all primary and all backup backend VMs are unhealthy. For load balancers that have configurable failover: [Internal TCP/UDP Load Balancing](https://cloud.google.com/load-balancing/docs/internal/failover-overview) and [external TCP/UDP Load Balancing](https://cloud.google.com/load-balancing/docs/network/networklb-failover-overview). The default is false.
+            * disable_connection_drain_on_failover (bool, Optional):
+                This can be set to true only if the protocol is TCP. The default is false.
+            * failover_ratio (float, Optional):
+                The value of the field must be in the range [0, 1]. If the value is 0, the load balancer performs a failover when the number of healthy primary VMs equals zero. For all other values, the load balancer performs a failover when the total number of healthy primary VMs is less than this ratio. For load balancers that have configurable failover: [Internal TCP/UDP Load Balancing](https://cloud.google.com/load-balancing/docs/internal/failover-overview) and [external TCP/UDP Load Balancing](https://cloud.google.com/load-balancing/docs/network/networklb-failover-overview).
 
         protocol(str, Optional):
             The protocol this BackendService uses to communicate with backends. Possible values are HTTP, HTTPS, HTTP2, TCP, SSL, UDP or GRPC. depending on the chosen load balancer or Traffic Director configuration. Refer to the documentation for the load balancers or for Traffic Director for more information. Must be set to GRPC when the backend service is referenced by a URL map that is bound to target gRPC proxy.
-                Enum type. Allowed values:
+            Enum type. Allowed values:
                 "GRPC" - gRPC (available for Traffic Director).
                 "HTTP"
                 "HTTP2" - HTTP/2 with SSL.
                 "HTTPS"
                 "SSL" - TCP proxying with SSL.
                 "TCP" - TCP proxying or TCP pass-through.
                 "UDP" - UDP.
@@ -315,95 +324,130 @@
 
         network(str, Optional): The URL of the network to which this backend service belongs. This field can only be specified when the load balancing scheme is set to INTERNAL. Defaults to None.
 
         cdn_policy(Dict[str, Any], Optional):
             Cloud CDN configuration for this BackendService. Only available for specified load balancer types.
             BackendServiceCdnPolicy: Message containing Cloud CDN configuration for a backend service. Defaults to None.
 
-            * request_coalescing (bool, Optional): If true then Cloud CDN will combine multiple concurrent cache fill requests into a small number of requests to the origin.
-            * default_ttl (int, Optional): Specifies the default TTL for cached content served by this origin for responses that do not have an existing valid TTL (max-age or s-max-age). Setting a TTL of "0" means "always revalidate". The value of defaultTTL cannot be set to a value greater than that of maxTTL, but can be equal. When the cacheMode is set to FORCE_CACHE_ALL, the defaultTTL will overwrite the TTL set in all responses. The maximum allowed value is 31,622,400s (1 year), noting that infrequently accessed objects may be evicted from the cache before the defined TTL.
-            * bypass_cache_on_request_headers (List[Dict[str, Any]], Optional): Bypass the cache when the specified request headers are matched - e.g. Pragma or Authorization headers. Up to 5 headers can be specified. The cache is bypassed for all cdnPolicy.cacheMode settings.
-                * header_name (str, Optional): The header field name to match on when bypassing cache. Values are case-insensitive.
+            * request_coalescing (bool, Optional):
+                If true then Cloud CDN will combine multiple concurrent cache fill requests into a small number of requests to the origin.
+            * default_ttl (int, Optional):
+                Specifies the default TTL for cached content served by this origin for responses that do not have an existing valid TTL (max-age or s-max-age). Setting a TTL of "0" means "always revalidate". The value of defaultTTL cannot be set to a value greater than that of maxTTL, but can be equal. When the cacheMode is set to FORCE_CACHE_ALL, the defaultTTL will overwrite the TTL set in all responses. The maximum allowed value is 31,622,400s (1 year), noting that infrequently accessed objects may be evicted from the cache before the defined TTL.
+            * bypass_cache_on_request_headers (List[Dict[str, Any]], Optional):
+                Bypass the cache when the specified request headers are matched - e.g. Pragma or Authorization headers. Up to 5 headers can be specified. The cache is bypassed for all cdnPolicy.cacheMode settings.
+
+                * header_name (str, Optional):
+                    The header field name to match on when bypassing cache. Values are case-insensitive.
             * cache_mode (str, Optional):
                 Specifies the cache setting for all responses from this backend. The possible values are: USE_ORIGIN_HEADERS Requires the origin to set valid caching headers to cache content. Responses without these headers will not be cached at Google's edge, and will require a full trip to the origin on every request, potentially impacting performance and increasing load on the origin server. FORCE_CACHE_ALL Cache all content, ignoring any "private", "no-store" or "no-cache" directives in Cache-Control response headers. Warning: this may result in Cloud CDN caching private, per-user (user identifiable) content. CACHE_ALL_STATIC Automatically cache static content, including common image formats, media (video and audio), and web assets (JavaScript and CSS). Requests and responses that are marked as uncacheable, as well as dynamic content (including HTML), will not be cached.
-                    Enum type. Allowed values:
+                Enum type. Allowed values:
                     "CACHE_ALL_STATIC" - Automatically cache static content, including common image formats, media (video and audio), and web assets (JavaScript and CSS). Requests and responses that are marked as uncacheable, as well as dynamic content (including HTML), will not be cached.
                     "FORCE_CACHE_ALL" - Cache all content, ignoring any "private", "no-store" or "no-cache" directives in Cache-Control response headers. Warning: this may result in Cloud CDN caching private, per-user (user identifiable) content.
                     "INVALID_CACHE_MODE"
                     "USE_ORIGIN_HEADERS" - Requires the origin to set valid caching headers to cache content. Responses without these headers will not be cached at Google's edge, and will require a full trip to the origin on every request, potentially impacting performance and increasing load on the origin server.
 
-                * client_ttl (int, Optional): Specifies a separate client (e.g. browser client) maximum TTL. This is used to clamp the max-age (or Expires) value sent to the client. With FORCE_CACHE_ALL, the lesser of client_ttl and default_ttl is used for the response max-age directive, along with a "public" directive. For cacheable content in CACHE_ALL_STATIC mode, client_ttl clamps the max-age from the origin (if specified), or else sets the response max-age directive to the lesser of the client_ttl and default_ttl, and also ensures a "public" cache-control directive is present. If a client TTL is not specified, a default value (1 hour) will be used. The maximum allowed value is 31,622,400s (1 year).
-                * negative_caching (bool, Optional): Negative caching allows per-status code TTLs to be set, in order to apply fine-grained caching for common errors or redirects. This can reduce the load on your origin and improve end-user experience by reducing response latency. When the cache mode is set to CACHE_ALL_STATIC or USE_ORIGIN_HEADERS, negative caching applies to responses with the specified response code that lack any Cache-Control, Expires, or Pragma: no-cache directives. When the cache mode is set to FORCE_CACHE_ALL, negative caching applies to all responses with the specified response code, and override any caching headers. By default, Cloud CDN will apply the following default TTLs to these status codes: HTTP 300 (Multiple Choice), 301, 308 (Permanent Redirects): 10m HTTP 404 (Not Found), 410 (Gone), 451 (Unavailable For Legal Reasons): 120s HTTP 405 (Method Not Found), 421 (Misdirected Request), 501 (Not Implemented): 60s. These defaults can be overridden in negative_caching_policy.
-                * signed_url_cache_max_age_sec (str, Optional): Maximum number of seconds the response to a signed URL request will be considered fresh. After this time period, the response will be revalidated before being served. Defaults to 1hr (3600s). When serving responses to signed URL requests, Cloud CDN will internally behave as though all responses from this backend had a "Cache-Control: public, max-age=[TTL]" header, regardless of any existing Cache-Control header. The actual headers served in responses will not be altered.
-                * negative_caching_policy (List[Dict[str, Any]], Optional):
-                    Sets a cache TTL for the specified HTTP status code. negative_caching must be enabled to configure negative_caching_policy. Omitting the policy and leaving negative_caching enabled will use Cloud CDN's default cache TTLs. Note that when specifying an explicit negative_caching_policy, you should take care to specify a cache TTL for all response codes that you wish to cache. Cloud CDN will not apply any default negative caching when a policy exists.
-
-                    * ttl (int, Optional): The TTL (in seconds) for which to cache responses with the corresponding status code. The maximum allowed value is 1800s (30 minutes), noting that infrequently accessed objects may be evicted from the cache before the defined TTL.
-                    * code (int, Optional): The HTTP status code to define a TTL against. Only HTTP status codes 300, 301, 302, 307, 308, 404, 405, 410, 421, 451 and 501 are can be specified as values, and you cannot specify a status code more than once.
-                * cache_key_policy (Dict[str, Any], Optional):
-                    The CacheKeyPolicy for this CdnPolicy.
-                    CacheKeyPolicy: Message containing what to include in the cache key for a request for Cloud CDN.
-
-                    * include_named_cookies (List[str], Optional): Allows HTTP cookies (by name) to be used in the cache key. The name=value pair will be used in the cache key Cloud CDN generates.
-                    * include_host (bool, Optional): If true, requests to different hosts will be cached separately.
-                    * include_protocol (bool, Optional): If true, http and https requests will be cached separately.
-                    * query_string_blacklist (List[str], Optional): Names of query string parameters to exclude in cache keys. All other parameters will be included. Either specify query_string_whitelist or query_string_blacklist, not both. '&' and '=' will be percent encoded and not treated as delimiters.
-                    * include_query_string (bool, Optional): If true, include query string parameters in the cache key according to query_string_whitelist and query_string_blacklist. If neither is set, the entire query string will be included. If false, the query string will be excluded from the cache key entirely.
-                    * query_string_whitelist (List[str], Optional): Names of query string parameters to include in cache keys. All other parameters will be excluded. Either specify query_string_whitelist or query_string_blacklist, not both. '&' and '=' will be percent encoded and not treated as delimiters.
-                    * include_http_headers (List[str], Optional): Allows HTTP request headers (by name) to be used in the cache key.
-
-                * serve_while_stale (int, Optional):
-                    Serve existing content from the cache (if available) when revalidating content with the origin, or when an error is encountered when refreshing the cache. This setting defines the default "max-stale" duration for any cached responses that do not specify a max-stale directive. Stale responses that exceed the TTL configured here will not be served. The default limit (max-stale) is 86400s (1 day), which will allow stale content to be served up to this limit beyond the max-age (or s-max-age) of a cached response. The maximum allowed value is 604800 (1 week). Set this to zero (0) to disable serve-while-stale.
-                * max_ttl (int, Optional):
-                    Specifies the maximum allowed TTL for cached content served by this origin. Cache directives that attempt to set a max-age or s-maxage higher than this, or an Expires header more than maxTTL seconds in the future will be capped at the value of maxTTL, as if it were the value of an s-maxage Cache-Control directive. Headers sent to the client will not be modified. Setting a TTL of "0" means "always revalidate". The maximum allowed value is 31,622,400s (1 year), noting that infrequently accessed objects may be evicted from the cache before the defined TTL.
-                * signed_url_key_names (List[str], Optional):
-                    [Output Only] Names of the keys for signing request URLs.
+            * client_ttl (int, Optional):
+                Specifies a separate client (e.g. browser client) maximum TTL. This is used to clamp the max-age (or Expires) value sent to the client. With FORCE_CACHE_ALL, the lesser of client_ttl and default_ttl is used for the response max-age directive, along with a "public" directive. For cacheable content in CACHE_ALL_STATIC mode, client_ttl clamps the max-age from the origin (if specified), or else sets the response max-age directive to the lesser of the client_ttl and default_ttl, and also ensures a "public" cache-control directive is present. If a client TTL is not specified, a default value (1 hour) will be used. The maximum allowed value is 31,622,400s (1 year).
+            * negative_caching (bool, Optional):
+                Negative caching allows per-status code TTLs to be set, in order to apply fine-grained caching for common errors or redirects. This can reduce the load on your origin and improve end-user experience by reducing response latency. When the cache mode is set to CACHE_ALL_STATIC or USE_ORIGIN_HEADERS, negative caching applies to responses with the specified response code that lack any Cache-Control, Expires, or Pragma: no-cache directives. When the cache mode is set to FORCE_CACHE_ALL, negative caching applies to all responses with the specified response code, and override any caching headers. By default, Cloud CDN will apply the following default TTLs to these status codes: HTTP 300 (Multiple Choice), 301, 308 (Permanent Redirects): 10m HTTP 404 (Not Found), 410 (Gone), 451 (Unavailable For Legal Reasons): 120s HTTP 405 (Method Not Found), 421 (Misdirected Request), 501 (Not Implemented): 60s. These defaults can be overridden in negative_caching_policy.
+            * signed_url_cache_max_age_sec (str, Optional):
+                Maximum number of seconds the response to a signed URL request will be considered fresh. After this time period, the response will be revalidated before being served. Defaults to 1hr (3600s). When serving responses to signed URL requests, Cloud CDN will internally behave as though all responses from this backend had a "Cache-Control: public, max-age=[TTL]" header, regardless of any existing Cache-Control header. The actual headers served in responses will not be altered.
+
+            * negative_caching_policy (List[Dict[str, Any]], Optional):
+                Sets a cache TTL for the specified HTTP status code. negative_caching must be enabled to configure negative_caching_policy. Omitting the policy and leaving negative_caching enabled will use Cloud CDN's default cache TTLs. Note that when specifying an explicit negative_caching_policy, you should take care to specify a cache TTL for all response codes that you wish to cache. Cloud CDN will not apply any default negative caching when a policy exists.
+
+                * ttl (int, Optional):
+                    The TTL (in seconds) for which to cache responses with the corresponding status code. The maximum allowed value is 1800s (30 minutes), noting that infrequently accessed objects may be evicted from the cache before the defined TTL.
+                * code (int, Optional):
+                    The HTTP status code to define a TTL against. Only HTTP status codes 300, 301, 302, 307, 308, 404, 405, 410, 421, 451 and 501 are can be specified as values, and you cannot specify a status code more than once.
+            * cache_key_policy (Dict[str, Any], Optional):
+                The CacheKeyPolicy for this CdnPolicy.
+                CacheKeyPolicy: Message containing what to include in the cache key for a request for Cloud CDN.
+
+                    * include_named_cookies (List[str], Optional):
+                        Allows HTTP cookies (by name) to be used in the cache key. The name=value pair will be used in the cache key Cloud CDN generates.
+                    * include_host (bool, Optional):
+                        If true, requests to different hosts will be cached separately.
+                    * include_protocol (bool, Optional):
+                        If true, http and https requests will be cached separately.
+                    * query_string_blacklist (List[str], Optional):
+                        Names of query string parameters to exclude in cache keys. All other parameters will be included. Either specify query_string_whitelist or query_string_blacklist, not both. '&' and '=' will be percent encoded and not treated as delimiters.
+                    * include_query_string (bool, Optional):
+                        If true, include query string parameters in the cache key according to query_string_whitelist and query_string_blacklist. If neither is set, the entire query string will be included. If false, the query string will be excluded from the cache key entirely.
+                    * query_string_whitelist (List[str], Optional):
+                        Names of query string parameters to include in cache keys. All other parameters will be excluded. Either specify query_string_whitelist or query_string_blacklist, not both. '&' and '=' will be percent encoded and not treated as delimiters.
+                    * include_http_headers (List[str], Optional):
+                        Allows HTTP request headers (by name) to be used in the cache key.
+
+            * serve_while_stale (int, Optional):
+                Serve existing content from the cache (if available) when revalidating content with the origin, or when an error is encountered when refreshing the cache. This setting defines the default "max-stale" duration for any cached responses that do not specify a max-stale directive. Stale responses that exceed the TTL configured here will not be served. The default limit (max-stale) is 86400s (1 day), which will allow stale content to be served up to this limit beyond the max-age (or s-max-age) of a cached response. The maximum allowed value is 604800 (1 week). Set this to zero (0) to disable serve-while-stale.
+            * max_ttl (int, Optional):
+                Specifies the maximum allowed TTL for cached content served by this origin. Cache directives that attempt to set a max-age or s-maxage higher than this, or an Expires header more than maxTTL seconds in the future will be capped at the value of maxTTL, as if it were the value of an s-maxage Cache-Control directive. Headers sent to the client will not be modified. Setting a TTL of "0" means "always revalidate". The maximum allowed value is 31,622,400s (1 year), noting that infrequently accessed objects may be evicted from the cache before the defined TTL.
+            * signed_url_key_names (List[str], Optional):
+                [Output Only] Names of the keys for signing request URLs.
 
         log_config(Dict[str, Any], Optional):
             This field denotes the logging options for the load balancer traffic served by this backend service. If logging is enabled, logs will be exported to Stackdriver.
             BackendServiceLogConfig: The available logging options for the load balancer traffic served by this backend service. Defaults to None.
 
-            * enable (bool, Optional): Denotes whether to enable logging for the load balancer traffic served by this backend service. The default value is false.
-            * sample_rate (float, Optional): This field can only be specified if logging is enabled for this backend service. The value of the field must be in [0, 1]. This configures the sampling rate of requests to the load balancer where 1.0 means all logged requests are reported and 0.0 means no logged requests are reported. The default value is 1.0.
+            * enable (bool, Optional):
+                Denotes whether to enable logging for the load balancer traffic served by this backend service. The default value is false.
+            * sample_rate (float, Optional):
+                This field can only be specified if logging is enabled for this backend service. The value of the field must be in [0, 1]. This configures the sampling rate of requests to the load balancer where 1.0 means all logged requests are reported and 0.0 means no logged requests are reported. The default value is 1.0.
 
         security_settings(Dict[str, Any], Optional):
             This field specifies the security settings that apply to this backend service. This field is applicable to a global backend service with the load_balancing_scheme set to INTERNAL_SELF_MANAGED.
             SecuritySettings: The authentication and authorization settings for a BackendService. Defaults to None.
 
-            * client_tls_policy (str, Optional): Optional. A URL referring to a networksecurity.ClientTlsPolicy resource that describes how clients should authenticate with this service's backends. clientTlsPolicy only applies to a global BackendService with the loadBalancingScheme set to INTERNAL_SELF_MANAGED. If left blank, communications are not encrypted. Note: This field currently has no impact.
-            * subject_alt_names (List[str], Optional): Optional. A list of Subject Alternative Names (SANs) that the client verifies during a mutual TLS handshake with an server/endpoint for this BackendService. When the server presents its X.509 certificate to the client, the client inspects the certificate's subjectAltName field. If the field contains one of the specified values, the communication continues. Otherwise, it fails. This additional check enables the client to verify that the server is authorized to run the requested service. Note that the contents of the server certificate's subjectAltName field are configured by the Public Key Infrastructure which provisions server identities. Only applies to a global BackendService with loadBalancingScheme set to INTERNAL_SELF_MANAGED. Only applies when BackendService has an attached clientTlsPolicy with clientCertificate (mTLS mode). Note: This field currently has no impact.
+            * client_tls_policy (str, Optional):
+                Optional. A URL referring to a networksecurity.ClientTlsPolicy resource that describes how clients should authenticate with this service's backends. clientTlsPolicy only applies to a global BackendService with the loadBalancingScheme set to INTERNAL_SELF_MANAGED. If left blank, communications are not encrypted. Note: This field currently has no impact.
+            * subject_alt_names (List[str], Optional):
+                Optional. A list of Subject Alternative Names (SANs) that the client verifies during a mutual TLS handshake with an server/endpoint for this BackendService. When the server presents its X.509 certificate to the client, the client inspects the certificate's subjectAltName field. If the field contains one of the specified values, the communication continues. Otherwise, it fails. This additional check enables the client to verify that the server is authorized to run the requested service. Note that the contents of the server certificate's subjectAltName field are configured by the Public Key Infrastructure which provisions server identities. Only applies to a global BackendService with loadBalancingScheme set to INTERNAL_SELF_MANAGED. Only applies when BackendService has an attached clientTlsPolicy with clientCertificate (mTLS mode). Note: This field currently has no impact.
 
         backends(List[Dict[str, Any]], Optional):
             The list of backends that serve this BackendService. Defaults to None.
 
-            * max_connections (int, Optional): Defines a target maximum number of simultaneous connections. For usage guidelines, see Connection balancing mode and Utilization balancing mode. Not available if the backend's balancingMode is RATE.
-            * max_connections_per_instance (int, Optional): Defines a target maximum number of simultaneous connections. For usage guidelines, see Connection balancing mode and Utilization balancing mode. Not available if the backend's balancingMode is RATE.
-            * max_rate_per_endpoint (float, Optional): Defines a maximum target for requests per second (RPS). For usage guidelines, see Rate balancing mode and Utilization balancing mode. Not available if the backend's balancingMode is CONNECTION.
-            * max_utilization (float, Optional): Optional parameter to define a target capacity for the UTILIZATION balancing mode. The valid range is [0.0, 1.0]. For usage guidelines, see Utilization balancing mode.
-            * max_rate (int, Optional): Defines a maximum number of HTTP requests per second (RPS). For usage guidelines, see Rate balancing mode and Utilization balancing mode. Not available if the backend's balancingMode is CONNECTION.
-            * capacity_scaler (float, Optional): A multiplier applied to the backend's target capacity of its balancing mode. The default value is 1, which means the group serves up to 100% of its configured capacity (depending on balancingMode). A setting of 0 means the group is completely drained, offering 0% of its available capacity. The valid ranges are 0.0 and [0.1,1.0]. You cannot configure a setting larger than 0 and smaller than 0.1. You cannot configure a setting of 0 when there is only one backend attached to the backend service.
-            * group (str, Optional): The fully-qualified URL of an instance group or network endpoint group (NEG) resource. To determine what types of backends a load balancer supports, see the [Backend services overview](https://cloud.google.com/load-balancing/docs/backend-service#backends). You must use the *fully-qualified* URL (starting with https://www.googleapis.com/) to specify the instance group or NEG. Partial URLs are not supported.
+            * max_connections (int, Optional):
+                Defines a target maximum number of simultaneous connections. For usage guidelines, see Connection balancing mode and Utilization balancing mode. Not available if the backend's balancingMode is RATE.
+            * max_connections_per_instance (int, Optional):
+                Defines a target maximum number of simultaneous connections. For usage guidelines, see Connection balancing mode and Utilization balancing mode. Not available if the backend's balancingMode is RATE.
+            * max_rate_per_endpoint (float, Optional):
+                Defines a maximum target for requests per second (RPS). For usage guidelines, see Rate balancing mode and Utilization balancing mode. Not available if the backend's balancingMode is CONNECTION.
+            * max_utilization (float, Optional):
+                Optional parameter to define a target capacity for the UTILIZATION balancing mode. The valid range is [0.0, 1.0]. For usage guidelines, see Utilization balancing mode.
+            * max_rate (int, Optional):
+                Defines a maximum number of HTTP requests per second (RPS). For usage guidelines, see Rate balancing mode and Utilization balancing mode. Not available if the backend's balancingMode is CONNECTION.
+            * capacity_scaler (float, Optional):
+                A multiplier applied to the backend's target capacity of its balancing mode. The default value is 1, which means the group serves up to 100% of its configured capacity (depending on balancingMode). A setting of 0 means the group is completely drained, offering 0% of its available capacity. The valid ranges are 0.0 and [0.1,1.0]. You cannot configure a setting larger than 0 and smaller than 0.1. You cannot configure a setting of 0 when there is only one backend attached to the backend service.
+            * group (str, Optional):
+                The fully-qualified URL of an instance group or network endpoint group (NEG) resource. To determine what types of backends a load balancer supports, see the [Backend services overview](https://cloud.google.com/load-balancing/docs/backend-service#backends). You must use the *fully-qualified* URL (starting with https://www.googleapis.com/) to specify the instance group or NEG. Partial URLs are not supported.
             * balancing_mode (str, Optional):
                 Specifies how to determine whether the backend of a load balancer can handle additional traffic or is fully loaded. For usage guidelines, see Connection balancing mode. Backends must use compatible balancing modes. For more information, see Supported balancing modes and target capacity settings and Restrictions and guidance for instance groups. Note: Currently, if you use the API to configure incompatible balancing modes, the configuration might be accepted even though it has no impact and is ignored. Specifically, Backend.maxUtilization is ignored when Backend.balancingMode is RATE. In the future, this incompatible combination will be rejected.
-                    Enum type. Allowed values:
+                Enum type. Allowed values:
                     "CONNECTION" - Balance based on the number of simultaneous connections.
                     "RATE" - Balance based on requests per second (RPS).
                     "UTILIZATION" - Balance based on the backend utilization.
 
-                * failover (bool, Optional): This field designates whether this is a failover backend. More than one failover backend can be configured for a given BackendService.
-                * max_connections_per_endpoint (int, Optional): Defines a target maximum number of simultaneous connections. For usage guidelines, see Connection balancing mode and Utilization balancing mode. Not available if the backend's balancingMode is RATE.
-                * description (str, Optional): An optional description of this resource. Provide this property when you create the resource.
-                * max_rate_per_instance (float, Optional): Defines a maximum target for requests per second (RPS). For usage guidelines, see Rate balancing mode and Utilization balancing mode. Not available if the backend's balancingMode is CONNECTION.
+            * failover (bool, Optional):
+                This field designates whether this is a failover backend. More than one failover backend can be configured for a given BackendService.
+            * max_connections_per_endpoint (int, Optional):
+                Defines a target maximum number of simultaneous connections. For usage guidelines, see Connection balancing mode and Utilization balancing mode. Not available if the backend's balancingMode is RATE.
+            * description (str, Optional):
+                An optional description of this resource. Provide this property when you create the resource.
+            * max_rate_per_instance (float, Optional):
+                Defines a maximum target for requests per second (RPS). For usage guidelines, see Rate balancing mode and Utilization balancing mode. Not available if the backend's balancingMode is CONNECTION.
 
         max_stream_duration(Dict[str, Any], Optional):
             Specifies the default maximum duration (timeout) for streams to this service. Duration is computed from the beginning of the stream until the response has been completely processed, including all retries. A stream that does not complete in this duration is closed. If not specified, there will be no timeout limit, i.e. the maximum duration is infinite. This value can be overridden in the PathMatcher configuration of the UrlMap that references this backend service. This field is only allowed when the loadBalancingScheme of the backend service is INTERNAL_SELF_MANAGED.
             Duration: A Duration represents a fixed-length span of time represented as a count of seconds and fractions of seconds at nanosecond resolution. It is independent of any calendar and concepts like "day" or "month". Range is approximately 10,000 years. Defaults to None.
 
-            * nanos (int, Optional): Span of time that's a fraction of a second at nanosecond resolution. Durations less than one second are represented with a 0 `seconds` field and a positive `nanos` field. Must be from 0 to 999,999,999 inclusive.
-            * seconds (str, Optional): Span of time at a resolution of a second. Must be from 0 to 315,576,000,000 inclusive. Note: these bounds are computed from: 60 sec/min * 60 min/hr * 24 hr/day * 365.25 days/year * 10000 years
+            * nanos (int, Optional):
+                Span of time that's a fraction of a second at nanosecond resolution. Durations less than one second are represented with a 0 `seconds` field and a positive `nanos` field. Must be from 0 to 999,999,999 inclusive.
+            * seconds (str, Optional):
+                Span of time at a resolution of a second. Must be from 0 to 315,576,000,000 inclusive. Note: these bounds are computed from: 60 sec/min * 60 min/hr * 24 hr/day * 365.25 days/year * 10000 years
 
         subsetting(Dict[str, Any], Optional):
             Subsetting: Subsetting configuration for this BackendService. Currently this is applicable only for Internal TCP/UDP load balancing, Internal HTTP(S) load balancing and Traffic Director. Defaults to None.
 
             * policy (str, Optional):
                 Enum type. Allowed values:
                     "CONSISTENT_HASH_SUBSETTING" - Subsetting based on consistent hashing. For Traffic Director, the number of backends per backend group (the subset size) is based on the `subset_size` parameter. For Internal HTTP(S) load balancing, the number of backends per backend group (the subset size) is dynamically adjusted in two cases: - As the number of proxy instances participating in Internal HTTP(S) load balancing increases, the subset size decreases. - When the total number of backends in a network exceeds the capacity of a single proxy instance, subset sizes are reduced automatically for each service that has backend subsetting enabled.
@@ -414,142 +458,167 @@
         description(str, Optional): An optional description of this resource. Provide this property when you create the resource. Defaults to None.
 
         timeout_sec(int, Optional): The backend service timeout has a different meaning depending on the type of load balancer. For more information see, Backend service settings. The default is 30 seconds. The full range of timeout values allowed goes from 1 through 2,147,483,647 seconds. This value can be overridden in the PathMatcher configuration of the UrlMap that references this backend service. Not supported when the backend service is referenced by a URL map that is bound to target gRPC proxy that has validateForProxyless field set to true. Instead, use maxStreamDuration. Defaults to None.
 
         connection_draining(Dict[str, Any], Optional):
             ConnectionDraining: Message containing connection draining configuration. Defaults to None.
 
-            * draining_timeout_sec (int, Optional): Configures a duration timeout for existing requests on a removed backend instance. For supported load balancers and protocols, as described in Enabling connection draining.
+            * draining_timeout_sec (int, Optional):
+                Configures a duration timeout for existing requests on a removed backend instance. For supported load balancers and protocols, as described in Enabling connection draining.
 
         outlier_detection(Dict[str, Any], Optional):
                 Settings controlling the eviction of unhealthy hosts from the load balancing pool for the backend service. If not set, this feature is considered disabled. This field is applicable to either: - A regional backend service with the service_protocol set to HTTP, HTTPS, HTTP2, or GRPC, and load_balancing_scheme set to INTERNAL_MANAGED. - A global backend service with the load_balancing_scheme set to INTERNAL_SELF_MANAGED.
                 OutlierDetection: Settings controlling the eviction of unhealthy hosts from the load balancing pool for the backend service. Defaults to None.
 
                 * consecutive_errors (int, Optional):
                     Number of errors before a host is ejected from the connection pool. When the backend host is accessed over HTTP, a 5xx return code qualifies as an error. Defaults to 5. Not supported when the backend service is referenced by a URL map that is bound to target gRPC proxy that has validateForProxyless field set to true.
                 * base_ejection_time (Dict[str, Any], Optional):
                     The base time that a host is ejected for. The real ejection time is equal to the base ejection time multiplied by the number of times the host has been ejected. Defaults to 30000ms or 30s.
                     Duration: A Duration represents a fixed-length span of time represented as a count of seconds and fractions of seconds at nanosecond resolution. It is independent of any calendar and concepts like "day" or "month". Range is approximately 10,000 years.
 
-                    * nanos (int, Optional): Span of time that's a fraction of a second at nanosecond resolution. Durations less than one second are represented with a 0 `seconds` field and a positive `nanos` field. Must be from 0 to 999,999,999 inclusive.
-                    * seconds (str, Optional): Span of time at a resolution of a second. Must be from 0 to 315,576,000,000 inclusive. Note: these bounds are computed from: 60 sec/min * 60 min/hr * 24 hr/day * 365.25 days/year * 10000 years
-                * consecutive_gateway_failure (int, Optional): The number of consecutive gateway failures (502, 503, 504 status or connection errors that are mapped to one of those status codes) before a consecutive gateway failure ejection occurs. Defaults to 3. Not supported when the backend service is referenced by a URL map that is bound to target gRPC proxy that has validateForProxyless field set to true.
-                * enforcing_success_rate (int, Optional): The percentage chance that a host will be actually ejected when an outlier status is detected through success rate statistics. This setting can be used to disable ejection or to ramp it up slowly. Defaults to 100.
-                * enforcing_consecutive_gateway_failure (int, Optional): The percentage chance that a host will be actually ejected when an outlier status is detected through consecutive gateway failures. This setting can be used to disable ejection or to ramp it up slowly. Defaults to 100. Not supported when the backend service is referenced by a URL map that is bound to target gRPC proxy that has validateForProxyless field set to true.
-                * enforcing_consecutive_errors (int, Optional): The percentage chance that a host will be actually ejected when an outlier status is detected through consecutive 5xx. This setting can be used to disable ejection or to ramp it up slowly. Defaults to 0. Not supported when the backend service is referenced by a URL map that is bound to target gRPC proxy that has validateForProxyless field set to true.
-                * max_ejection_percent (int, Optional): Maximum percentage of hosts in the load balancing pool for the backend service that can be ejected. Defaults to 50%.
+                    * nanos (int, Optional):
+                        Span of time that's a fraction of a second at nanosecond resolution. Durations less than one second are represented with a 0 `seconds` field and a positive `nanos` field. Must be from 0 to 999,999,999 inclusive.
+                    * seconds (str, Optional):
+                        Span of time at a resolution of a second. Must be from 0 to 315,576,000,000 inclusive. Note: these bounds are computed from: 60 sec/min * 60 min/hr * 24 hr/day * 365.25 days/year * 10000 years
+                * consecutive_gateway_failure (int, Optional):
+                    The number of consecutive gateway failures (502, 503, 504 status or connection errors that are mapped to one of those status codes) before a consecutive gateway failure ejection occurs. Defaults to 3. Not supported when the backend service is referenced by a URL map that is bound to target gRPC proxy that has validateForProxyless field set to true.
+                * enforcing_success_rate (int, Optional):
+                    The percentage chance that a host will be actually ejected when an outlier status is detected through success rate statistics. This setting can be used to disable ejection or to ramp it up slowly. Defaults to 100.
+                * enforcing_consecutive_gateway_failure (int, Optional):
+                    The percentage chance that a host will be actually ejected when an outlier status is detected through consecutive gateway failures. This setting can be used to disable ejection or to ramp it up slowly. Defaults to 100. Not supported when the backend service is referenced by a URL map that is bound to target gRPC proxy that has validateForProxyless field set to true.
+                * enforcing_consecutive_errors (int, Optional):
+                    The percentage chance that a host will be actually ejected when an outlier status is detected through consecutive 5xx. This setting can be used to disable ejection or to ramp it up slowly. Defaults to 0. Not supported when the backend service is referenced by a URL map that is bound to target gRPC proxy that has validateForProxyless field set to true.
+                * max_ejection_percent (int, Optional):
+                    Maximum percentage of hosts in the load balancing pool for the backend service that can be ejected. Defaults to 50%.
                 * interval (Dict[str, Any], Optional):
                     Time interval between ejection analysis sweeps. This can result in both new ejections as well as hosts being returned to service. Defaults to 1 second.
                     Duration: A Duration represents a fixed-length span of time represented as a count of seconds and fractions of seconds at nanosecond resolution. It is independent of any calendar and concepts like "day" or "month". Range is approximately 10,000 years.
 
-                    * nanos (int, Optional): Span of time that's a fraction of a second at nanosecond resolution. Durations less than one second are represented with a 0 `seconds` field and a positive `nanos` field. Must be from 0 to 999,999,999 inclusive.
-                    * seconds (str, Optional): Span of time at a resolution of a second. Must be from 0 to 315,576,000,000 inclusive. Note: these bounds are computed from: 60 sec/min * 60 min/hr * 24 hr/day * 365.25 days/year * 10000 years
-                * success_rate_request_volume (int, Optional): The minimum number of total requests that must be collected in one interval (as defined by the interval duration above) to include this host in success rate based outlier detection. If the volume is lower than this setting, outlier detection via success rate statistics is not performed for that host. Defaults to 100.
-                * success_rate_stdev_factor (int, Optional): This factor is used to determine the ejection threshold for success rate outlier ejection. The ejection threshold is the difference between the mean success rate, and the product of this factor and the standard deviation of the mean success rate: mean - (stdev * success_rate_stdev_factor). This factor is divided by a thousand to get a double. That is, if the desired factor is 1.9, the runtime value should be 1900. Defaults to 1900.
-                * success_rate_minimum_hosts (int, Optional): The number of hosts in a cluster that must have enough request volume to detect success rate outliers. If the number of hosts is less than this setting, outlier detection via success rate statistics is not performed for any host in the cluster. Defaults to 5.
+                    * nanos (int, Optional):
+                        Span of time that's a fraction of a second at nanosecond resolution. Durations less than one second are represented with a 0 `seconds` field and a positive `nanos` field. Must be from 0 to 999,999,999 inclusive.
+                    * seconds (str, Optional):
+                        Span of time at a resolution of a second. Must be from 0 to 315,576,000,000 inclusive. Note: these bounds are computed from: 60 sec/min * 60 min/hr * 24 hr/day * 365.25 days/year * 10000 years
+                * success_rate_request_volume (int, Optional):
+                    The minimum number of total requests that must be collected in one interval (as defined by the interval duration above) to include this host in success rate based outlier detection. If the volume is lower than this setting, outlier detection via success rate statistics is not performed for that host. Defaults to 100.
+                * success_rate_stdev_factor (int, Optional):
+                    This factor is used to determine the ejection threshold for success rate outlier ejection. The ejection threshold is the difference between the mean success rate, and the product of this factor and the standard deviation of the mean success rate: mean - (stdev * success_rate_stdev_factor). This factor is divided by a thousand to get a double. That is, if the desired factor is 1.9, the runtime value should be 1900. Defaults to 1900.
+                * success_rate_minimum_hosts (int, Optional):
+                    The number of hosts in a cluster that must have enough request volume to detect success rate outliers. If the number of hosts is less than this setting, outlier detection via success rate statistics is not performed for any host in the cluster. Defaults to 5.
 
         enable_cdn(bool, Optional): If true, enables Cloud CDN for the backend service of an external HTTP(S) load balancer. Defaults to None.
 
         affinity_cookie_ttl_sec(int, Optional): Lifetime of cookies in seconds. This setting is applicable to external and internal HTTP(S) load balancers and Traffic Director and requires GENERATED_COOKIE or HTTP_COOKIE session affinity. If set to 0, the cookie is non-persistent and lasts only until the end of the browser session (or equivalent). The maximum allowed value is two weeks (1,209,600). Not supported when the backend service is referenced by a URL map that is bound to target gRPC proxy that has validateForProxyless field set to true. Defaults to None.
 
         connection_tracking_policy(Dict[str, Any], Optional):
             Connection Tracking configuration for this BackendService. Connection tracking policy settings are only available for Network Load Balancing and Internal TCP/UDP Load Balancing.
             BackendServiceConnectionTrackingPolicy: Connection Tracking configuration for this BackendService. Defaults to None.
 
             * idle_timeout_sec (int, Optional):
                 Specifies how long to keep a Connection Tracking entry while there is no matching traffic (in seconds). For Internal TCP/UDP Load Balancing: - The minimum (default) is 10 minutes and the maximum is 16 hours. - It can be set only if Connection Tracking is less than 5-tuple (i.e. Session Affinity is CLIENT_IP_NO_DESTINATION, CLIENT_IP or CLIENT_IP_PROTO, and Tracking Mode is PER_SESSION). For Network Load Balancer the default is 60 seconds. This option is not available publicly.
             * connection_persistence_on_unhealthy_backends (str, Optional):
                 Specifies connection persistence when backends are unhealthy. The default value is DEFAULT_FOR_PROTOCOL. If set to DEFAULT_FOR_PROTOCOL, the existing connections persist on unhealthy backends only for connection-oriented protocols (TCP and SCTP) and only if the Tracking Mode is PER_CONNECTION (default tracking mode) or the Session Affinity is configured for 5-tuple. They do not persist for UDP. If set to NEVER_PERSIST, after a backend becomes unhealthy, the existing connections on the unhealthy backend are never persisted on the unhealthy backend. They are always diverted to newly selected healthy backends (unless all backends are unhealthy). If set to ALWAYS_PERSIST, existing connections always persist on unhealthy backends regardless of protocol and session affinity. It is generally not recommended to use this mode overriding the default. For more details, see [Connection Persistence for Network Load Balancing](https://cloud.google.com/load-balancing/docs/network/networklb-backend-service#connection-persistence) and [Connection Persistence for Internal TCP/UDP Load Balancing](https://cloud.google.com/load-balancing/docs/internal#connection-persistence).
-                    Enum type. Allowed values:
+                Enum type. Allowed values:
                     "ALWAYS_PERSIST"
                     "DEFAULT_FOR_PROTOCOL"
                     "NEVER_PERSIST"
 
-                * enable_strong_affinity (bool, Optional):
-                    Enable Strong Session Affinity for Network Load Balancing. This option is not available publicly.
-                * tracking_mode (str, Optional):
-                    Specifies the key used for connection tracking. There are two options: - PER_CONNECTION: This is the default mode. The Connection Tracking is performed as per the Connection Key (default Hash Method) for the specific protocol. - PER_SESSION: The Connection Tracking is performed as per the configured Session Affinity. It matches the configured Session Affinity. For more details, see [Tracking Mode for Network Load Balancing](https://cloud.google.com/load-balancing/docs/network/networklb-backend-service#tracking-mode) and [Tracking Mode for Internal TCP/UDP Load Balancing](https://cloud.google.com/load-balancing/docs/internal#tracking-mode).
-                        Enum type. Allowed values:
-                        "INVALID_TRACKING_MODE"
-                        "PER_CONNECTION"
-                        "PER_SESSION"
+            * enable_strong_affinity (bool, Optional):
+                Enable Strong Session Affinity for Network Load Balancing. This option is not available publicly.
+            * tracking_mode (str, Optional):
+                Specifies the key used for connection tracking. There are two options: - PER_CONNECTION: This is the default mode. The Connection Tracking is performed as per the Connection Key (default Hash Method) for the specific protocol. - PER_SESSION: The Connection Tracking is performed as per the configured Session Affinity. It matches the configured Session Affinity. For more details, see [Tracking Mode for Network Load Balancing](https://cloud.google.com/load-balancing/docs/network/networklb-backend-service#tracking-mode) and [Tracking Mode for Internal TCP/UDP Load Balancing](https://cloud.google.com/load-balancing/docs/internal#tracking-mode).
+                Enum type. Allowed values:
+                    "INVALID_TRACKING_MODE"
+                    "PER_CONNECTION"
+                    "PER_SESSION"
 
         service_bindings(List[str], Optional): URLs of networkservices.ServiceBinding resources. Can only be set if load balancing scheme is INTERNAL_SELF_MANAGED. If set, lists of backends and health checks must be both empty. Defaults to None.
 
         load_balancing_scheme(str, Optional):
             Specifies the load balancer type. A backend service created for one type of load balancer cannot be used with another. For more information, refer to Choosing a load balancer.
-                Enum type. Allowed values:
+            Enum type. Allowed values:
                 "EXTERNAL" - Signifies that this will be used for external HTTP(S), SSL Proxy, TCP Proxy, or Network Load Balancing
                 "EXTERNAL_MANAGED" - Signifies that this will be used for External Managed HTTP(S) Load Balancing.
                 "INTERNAL" - Signifies that this will be used for Internal TCP/UDP Load Balancing.
                 "INTERNAL_MANAGED" - Signifies that this will be used for Internal HTTP(S) Load Balancing.
                 "INTERNAL_SELF_MANAGED" - Signifies that this will be used by Traffic Director.
                 "INVALID_LOAD_BALANCING_SCHEME". Defaults to None.
 
         compression_mode(str, Optional):
             Compress text responses using Brotli or gzip compression, based on the client's Accept-Encoding header.
-                Enum type. Allowed values:
+            Enum type. Allowed values:
                 "AUTOMATIC" - Automatically uses the best compression based on the Accept-Encoding header sent by the client.
                 "DISABLED" - Disables compression. Existing compressed responses cached by Cloud CDN will not be served to clients. Defaults to None.
 
         consistent_hash(Dict[str, Any], Optional):
             Consistent Hash-based load balancing can be used to provide soft session affinity based on HTTP headers, cookies or other properties. This load balancing policy is applicable only for HTTP connections. The affinity to a particular destination host will be lost when one or more hosts are added/removed from the destination service. This field specifies parameters that control consistent hashing. This field is only applicable when localityLbPolicy is set to MAGLEV or RING_HASH. This field is applicable to either: - A regional backend service with the service_protocol set to HTTP, HTTPS, or HTTP2, and load_balancing_scheme set to INTERNAL_MANAGED. - A global backend service with the load_balancing_scheme set to INTERNAL_SELF_MANAGED.
             ConsistentHashLoadBalancerSettings: This message defines settings for a consistent hash style load balancer. Defaults to None.
 
             * http_cookie (Dict[str, Any], Optional):
                 Hash is based on HTTP Cookie. This field describes a HTTP cookie that will be used as the hash key for the consistent hash load balancer. If the cookie is not present, it will be generated. This field is applicable if the sessionAffinity is set to HTTP_COOKIE. Not supported when the backend service is referenced by a URL map that is bound to target gRPC proxy that has validateForProxyless field set to true.
                 ConsistentHashLoadBalancerSettingsHttpCookie: The information about the HTTP Cookie on which the hash function is based for load balancing policies that use a consistent hash.
 
-                * name (str, Optional): Name of the cookie.
-                * path (str, Optional): Path to set for the cookie.
+                * name (str, Optional):
+                    Name of the cookie.
+                * path (str, Optional):
+                    Path to set for the cookie.
                 * ttl (Dict[str, Any], Optional):
                     Lifetime of the cookie.
                     Duration: A Duration represents a fixed-length span of time represented as a count of seconds and fractions of seconds at nanosecond resolution. It is independent of any calendar and concepts like "day" or "month". Range is approximately 10,000 years.
 
-                    * nanos (int, Optional): Span of time that's a fraction of a second at nanosecond resolution. Durations less than one second are represented with a 0 `seconds` field and a positive `nanos` field. Must be from 0 to 999,999,999 inclusive.
-                    * seconds (str, Optional): Span of time at a resolution of a second. Must be from 0 to 315,576,000,000 inclusive. Note: these bounds are computed from: 60 sec/min * 60 min/hr * 24 hr/day * 365.25 days/year * 10000 years
+                    * nanos (int, Optional):
+                        Span of time that's a fraction of a second at nanosecond resolution. Durations less than one second are represented with a 0 `seconds` field and a positive `nanos` field. Must be from 0 to 999,999,999 inclusive.
+                    * seconds (str, Optional):
+                        Span of time at a resolution of a second. Must be from 0 to 315,576,000,000 inclusive. Note: these bounds are computed from: 60 sec/min * 60 min/hr * 24 hr/day * 365.25 days/year * 10000 years
             * minimum_ring_size (str, Optional): The minimum number of virtual nodes to use for the hash ring. Defaults to 1024. Larger ring sizes result in more granular load distributions. If the number of hosts in the load balancing pool is larger than the ring size, each host will be assigned a single virtual node.
             * http_header_name (str, Optional): The hash based on the value of the specified header field. This field is applicable if the sessionAffinity is set to HEADER_FIELD.
 
         locality_lb_policies(List[Dict[str, Any]], Optional):
             A list of locality load balancing policies to be used in order of preference. Either the policy or the customPolicy field should be set. Overrides any value set in the localityLbPolicy field. localityLbPolicies is only supported when the BackendService is referenced by a URL Map that is referenced by a target gRPC proxy that has the validateForProxyless field set to true. Defaults to None.
 
-            * custom_policy (Dict[str, Any], Optional): BackendServiceLocalityLoadBalancingPolicyConfigCustomPolicy: The configuration for a custom policy implemented by the user and deployed with the client.
-                * name (str, Optional): Identifies the custom policy. The value should match the type the custom implementation is registered with on the gRPC clients. It should follow protocol buffer message naming conventions and include the full path (e.g. myorg.CustomLbPolicy). The maximum length is 256 characters. Note that specifying the same custom policy more than once for a backend is not a valid configuration and will be rejected.
-                * data (str, Optional): An optional, arbitrary JSON object with configuration data, understood by a locally installed custom policy implementation.
-            * policy (Dict[str, Any], Optional): BackendServiceLocalityLoadBalancingPolicyConfigPolicy: The configuration for a built-in load balancing policy.
+            * custom_policy (Dict[str, Any], Optional):
+             BackendServiceLocalityLoadBalancingPolicyConfigCustomPolicy: The configuration for a custom policy implemented by the user and deployed with the client.
+                * name (str, Optional):
+                    Identifies the custom policy. The value should match the type the custom implementation is registered with on the gRPC clients. It should follow protocol buffer message naming conventions and include the full path (e.g. myorg.CustomLbPolicy). The maximum length is 256 characters. Note that specifying the same custom policy more than once for a backend is not a valid configuration and will be rejected.
+                * data (str, Optional):
+                    An optional, arbitrary JSON object with configuration data, understood by a locally installed custom policy implementation.
+            * policy (Dict[str, Any], Optional):
+                BackendServiceLocalityLoadBalancingPolicyConfigPolicy: The configuration for a built-in load balancing policy.
                 * name (str, Optional):
                     The name of a locality load balancer policy to be used. The value should be one of the predefined ones as supported by localityLbPolicy, although at the moment only ROUND_ROBIN is supported. This field should only be populated when the customPolicy field is not used. Note that specifying the same policy more than once for a backend is not a valid configuration and will be rejected.
-                        Enum type. Allowed values:
+                    Enum type. Allowed values:
                         "INVALID_LB_POLICY"
                         "LEAST_REQUEST" - An O(1) algorithm which selects two random healthy hosts and picks the host which has fewer active requests.
                         "MAGLEV" - This algorithm implements consistent hashing to backends. Maglev can be used as a drop in replacement for the ring hash load balancer. Maglev is not as stable as ring hash but has faster table lookup build times and host selection times. For more information about Maglev, see https://ai.google/research/pubs/pub44824
                         "ORIGINAL_DESTINATION" - Backend host is selected based on the client connection metadata, i.e., connections are opened to the same address as the destination address of the incoming connection before the connection was redirected to the load balancer.
                         "RANDOM" - The load balancer selects a random healthy host.
                         "RING_HASH" - The ring/modulo hash load balancer implements consistent hashing to backends. The algorithm has the property that the addition/removal of a host from a set of N hosts only affects 1/N of the requests.
                         "ROUND_ROBIN" - This is a simple policy in which each healthy backend is selected in round robin order. This is the default.
 
         custom_request_headers(List[str], Optional): Headers that the load balancer adds to proxied requests. See [Creating custom headers](https://cloud.google.com/load-balancing/docs/custom-headers). Defaults to None.
 
         iap(Dict[str, Any], Optional):
             The configurations for Identity-Aware Proxy on this resource. Not available for Internal TCP/UDP Load Balancing and Network Load Balancing.
             BackendServiceIAP: Identity-Aware Proxy. Defaults to None.
 
-            * oauth2_client_id (str, Optional): OAuth2 client ID to use for the authentication flow.
-            * oauth2_client_secret (str, Optional): OAuth2 client secret to use for the authentication flow. For security reasons, this value cannot be retrieved via the API. Instead, the SHA-256 hash of the value is returned in the oauth2ClientSecretSha256 field. @InputOnly
-            * enabled (bool, Optional): Whether the serving infrastructure will authenticate and authorize all incoming requests. If true, the oauth2ClientId and oauth2ClientSecret fields must be non-empty.
-            * oauth2_client_secret_sha256 (str, Optional): [Output Only] SHA256 hash value for the field oauth2_client_secret above.
+            * oauth2_client_id (str, Optional):
+                OAuth2 client ID to use for the authentication flow.
+            * oauth2_client_secret (str, Optional):
+                OAuth2 client secret to use for the authentication flow. For security reasons, this value cannot be retrieved via the API. Instead, the SHA-256 hash of the value is returned in the oauth2ClientSecretSha256 field. @InputOnly
+            * enabled (bool, Optional):
+                Whether the serving infrastructure will authenticate and authorize all incoming requests. If true, the oauth2ClientId and oauth2ClientSecret fields must be non-empty.
+            * oauth2_client_secret_sha256 (str, Optional):
+                [Output Only] SHA256 hash value for the field oauth2_client_secret above.
 
         custom_response_headers(List[str], Optional): Headers that the load balancer adds to proxied responses. See [Creating custom headers](https://cloud.google.com/load-balancing/docs/custom-headers). Defaults to None.
 
         port_name(str, Optional): A named port on a backend instance group representing the port for communication to the backend VMs in that group. The named port must be [defined on each backend instance group](https://cloud.google.com/load-balancing/docs/backend-service#named_ports). This parameter has no meaning if the backends are NEGs. For Internal TCP/UDP Load Balancing and Network Load Balancing, omit port_name. Defaults to None.
 
         session_affinity(str, Optional):
             Type of session affinity to use. The default is NONE. Only NONE and HEADER_FIELD are supported when the backend service is referenced by a URL map that is bound to target gRPC proxy that has validateForProxyless field set to true. For more details, see: [Session Affinity](https://cloud.google.com/load-balancing/docs/backend-service#session_affinity).
-                Enum type. Allowed values:
+            Enum type. Allowed values:
                 "CLIENT_IP" - 2-tuple hash on packet's source and destination IP addresses. Connections from the same source IP address to the same destination IP address will be served by the same backend VM while that VM remains healthy.
                 "CLIENT_IP_NO_DESTINATION" - 1-tuple hash only on packet's source IP address. Connections from the same source IP address will be served by the same backend VM while that VM remains healthy. This option can only be used for Internal TCP/UDP Load Balancing.
                 "CLIENT_IP_PORT_PROTO" - 5-tuple hash on packet's source and destination IP addresses, IP protocol, and source and destination ports. Connections for the same IP protocol from the same source IP address and port to the same destination IP address and port will be served by the same backend VM while that VM remains healthy. This option cannot be used for HTTP(S) load balancing.
                 "CLIENT_IP_PROTO" - 3-tuple hash on packet's source and destination IP addresses, and IP protocol. Connections for the same IP protocol from the same source IP address to the same destination IP address will be served by the same backend VM while that VM remains healthy. This option cannot be used for HTTP(S) load balancing.
                 "GENERATED_COOKIE" - Hash based on a cookie generated by the L7 loadbalancer. Only valid for HTTP(S) load balancing.
                 "HEADER_FIELD" - The hash is based on a user specified header field.
                 "HTTP_COOKIE" - The hash is based on a user provided cookie.
@@ -761,18 +830,22 @@
     project: str = None,
     request_id: str = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
     r"""Deletes the specified BackendService resource.
 
     Args:
-        name(str): An Idem name of the resource.
-        request_id(str, Optional): An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000). Defaults to None.
-        project(str): Project ID for this request.
-        resource_id(str, Optional): An identifier of the resource in the provider. Defaults to None.
+        name(str):
+            An Idem name of the resource.
+        request_id(str, Optional):
+            An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000). Defaults to None.
+        project(str):
+            Project ID for this request.
+        resource_id(str, Optional):
+            An identifier of the resource in the provider. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
```

### Comparing `idem_gcp-1.1.0/idem_gcp/states/gcp/compute/disk.py` & `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/disk.py`

 * *Files 18% similar despite different names*

```diff
@@ -167,22 +167,18 @@
             Defaults to None.
 
         licenses(List[str], Optional):
             A list of publicly visible licenses. Reserved for Google's use.
             Defaults to None.
 
         guest_os_features(List[Dict[str, Any]], Optional):
-            A list of features to enable on the guest operating system. Applicable only for bootable images.
-            Read Enabling guest operating system features to see a list of available options.
-            Defaults to None.
-
-            * type (str, Optional):
-                The ID of a supported feature. To add multiple values,
-                use commas to separate values. Set to one or more of the following values:
+            A list of features to enable on the guest operating system. Applicable only for bootable images. Read Enabling guest operating system features to see a list of available options. Defaults to None.
 
+            * type(str, Optional):
+                The ID of a supported feature. To add multiple values, use commas to separate values. Set to one or more of the following values:
                 - VIRTIO_SCSI_MULTIQUEUE
                 - WINDOWS
                 - MULTI_IP_SUBNET
                 - UEFI_COMPATIBLE
                 - GVNIC
                 - SEV_CAPABLE
                 - SUSPEND_RESUME_COMPATIBLE
@@ -247,28 +243,37 @@
 
 
         source_image_encryption_key(Dict[str, Any], Optional):
             The customer-supplied encryption key of the source image.
             Required if the source image is protected by a customer-supplied encryption key.
             Defaults to None.
 
-            * raw_key(str, Optional)
-            * rsa_encrypted_key(str, Optional)
-            * kms_key_name(str, Optional)
-            * kms_key_service_account(str, Optional)
+            * raw_key(str, Optional):
+                Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
+            * rsa_encrypted_key(str, Optional):
+                Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
+            * kms_key_name(str, Optional):
+                The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
+            * kms_key_service_account(str, Optional):
+                The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/
 
         source_snapshot_encryption_key(Dict[str, Any], Optional):
             The customer-supplied encryption key of the source snapshot.
             Required if the source snapshot is protected by a customer-supplied encryption key.
             Defaults to None.
 
-            * raw_key(str, Optional)
-            * rsa_encrypted_key(str, Optional)
-            * kms_key_name(str, Optional)
-            * kms_key_service_account(str, Optional)
+            * raw_key(str, Optional):
+                Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
+            * rsa_encrypted_key(str, Optional):
+                Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
+            * kms_key_name(str, Optional):
+                The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
+            * kms_key_service_account(str, Optional):
+                The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/
+
 
         labels(Dict[str, Dict[str, str]], Optional):
             Labels to apply to this disk. These can be later modified by the setLabels method.
             Defaults to None.
 
         label_fingerprint(str, Optional):
             A fingerprint for the labels being applied to this disk,
@@ -325,22 +330,18 @@
             Defaults to None.
 
         architecture(str, Optional):
             The architecture of the disk. Valid values are ARM64 or X86_64.
             Defaults to None.
 
         params(Dict[str, Dict[str, str]], Optional):
-            Input only. [Input Only] Additional params passed with the request,
-            but not persisted as part of resource payload.
-            Defaults to None.
+            Input only. [Input Only] Additional params passed with the request, but not persisted as part of resource payload. Defaults to None.
 
-            * resourceManagerTags(Dict[str, str], Optional):
-                Resource manager tags to be bound to the disk. Tag keys and values have the same definition as
-                resource manager tags. Keys must be in the format `tagKeys/{tag_key_id}`, and values are in the format
-                `tagValues/456`. The field is ignored (both PUT & PATCH) when empty.
+            * resource_manager_tags(Dict[str, str], Optional):
+                Resource manager tags to be bound to the disk. Tag keys and values have the same definition as resource manager tags. Keys must be in the format `tagKeys/{tag_key_id}`, and values are in the format `tagValues/456`. The field is ignored (both PUT & PATCH) when empty.
 
         description(str, Optional):
             An optional description of this resource.
             Defaults to None.
 
         id(str, Optional): The unique identifier for the resource. This identifier is defined by the server. Read-only property
```

### Comparing `idem_gcp-1.1.0/idem_gcp/states/gcp/compute/firewall.py` & `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/firewall.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,40 +75,40 @@
             instance with service account listed in sourceServiceAccount. The connection does not need to match both
             fields for the firewall to apply. sourceServiceAccounts cannot be used at the same time as sourceTags or
             targetTags. Defaults to None.
         denied(List[Dict[str, Any]], Optional):
             The list of DENY rules specified by this firewall. Each rule specifies a protocol and port-range tuple that
             describes a denied connection. Defaults to None.
 
-            * ip_protocol (str, Optional): The IP protocol to which this rule applies. The protocol type is required when
-              creating a firewall rule. This value can either be one of the following well known protocol strings
+            * ip_protocol(str, Optional):
+                The IP protocol to which this rule applies. The protocol type is required when creating a firewall rule. This value can either be one of the following well known protocol strings
               (tcp, udp, icmp, esp, ah, ipip, sctp) or the IP protocol number.
-            * ports (list[str], Optional): An optional list of ports to which this rule applies. This field is only
-              applicable for the UDP or TCP protocol. Each entry must be either an integer or a range. If not specified,
-              this rule applies to connections through any port. Example inputs include: ["22"], ["80","443"], and
-              ["12345-12349"].
+            * ports(list[str], Optional):
+                An optional list of ports to which this rule applies. This field is only applicable for the UDP or TCP protocol. Each entry must be either an integer or a range. If not specified, this rule applies to connections through any port. Example inputs include: ["22"], ["80","443"], and ["12345-12349"].
         description(str, Optional):
             An optional description of this resource. Provide this field when you create the resource. Defaults to None.
         direction(str, Optional):
             Direction of traffic to which this firewall applies, either `INGRESS` or `EGRESS`. The default is `INGRESS`.
             For `EGRESS` traffic, you cannot specify the sourceTags fields. Defaults to None.
         destination_ranges(List[str], Optional):
             If destination ranges are specified, the firewall rule applies only to traffic that has destination IP
             address in these ranges. These ranges must be expressed in CIDR format. Both IPv4 and IPv6 are supported.
             Defaults to None.
         allowed(List[Dict[str, Any]], Optional):
             The list of ALLOW rules specified by this firewall. Each rule specifies a protocol and port-range tuple that
             describes a permitted connection. Defaults to None.
 
-            * ports (List[str], Optional): An optional list of ports to which this rule applies. This field is only
-              applicable for the UDP or TCP protocol. Each entry must be either an integer or a range. If not specified,
-              this rule applies to connections through any port. Example inputs include: ["22"], ["80","443"], and ["12345-12349"].
-            * ip_protocol (str, Optional): The IP protocol to which this rule applies. The protocol type is required when
-              creating a firewall rule. This value can either be one of the following well known protocol strings
-              (tcp, udp, icmp, esp, ah, ipip, sctp) or the IP protocol number.
+            * ports(List[str], Optional):
+                An optional list of ports to which this rule applies. This field is only applicable for the UDP or TCP protocol.
+                Each entry must be either an integer or a range. If not specified, this rule applies to connections through
+                any port. Example inputs include: ["22"], ["80","443"], and ["12345-12349"].
+            * ip_protocol(str, Optional):
+                The IP protocol to which this rule applies. The protocol type is required when
+                creating a firewall rule. This value can either be one of the following well known protocol strings
+                (tcp, udp, icmp, esp, ah, ipip, sctp) or the IP protocol number.
         disabled(bool, Optional):
             Denotes whether the firewall rule is disabled. When set to true, the firewall rule is not enforced and the
             network behaves as if it did not exist. If this is unspecified, the firewall rule will be enabled. Defaults to None.
         network(str, Optional):
             URL of the network resource for this firewall rule. If not specified when creating a firewall rule, the
             default network is used: global/networks/default If you choose to specify this field, you can specify the
             network as a full or partial URL. For example, the following are all valid
```

### Comparing `idem_gcp-1.1.0/idem_gcp/states/gcp/compute/forwarding_rule.py` & `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/forwarding_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,45 +99,48 @@
 
         fingerprint(str, Optional):
             Fingerprint of this resource. A hash of the contents stored in this object. This field is used in optimistic locking. This field will be ignored when inserting a ForwardingRule. Include the fingerprint in patch request to ensure that you do not overwrite changes that were applied from another concurrent request. To see the latest fingerprint, make a get() request to retrieve a ForwardingRule. Defaults to None.
 
         service_directory_registrations(List[Dict[str, Any]], Optional):
             Service Directory resources to register this forwarding rule with. Currently, only supports a single Service Directory resource. Defaults to None.
 
-            * service (str, Optional): Service Directory service to register the forwarding rule under.
-            * namespace (str, Optional): Service Directory namespace to register the forwarding rule under.
-            * service_directory_region (str, Optional): [Optional] Service Directory region to register this global forwarding rule under. Default to "us-central1". Only used for PSC for Google APIs. All PSC for Google APIs Forwarding Rules on the same network should use the same Service Directory region.
+            * service(str, Optional):
+                Service Directory service to register the forwarding rule under.
+            * namespace(str, Optional):
+                Service Directory namespace to register the forwarding rule under.
+            * service_directory_region(str, Optional):
+                [Optional] Service Directory region to register this global forwarding rule under. Default to "us-central1". Only used for PSC for Google APIs. All PSC for Google APIs Forwarding Rules on the same network should use the same Service Directory region.
 
         ip_protocol(str, Optional):
             The IP protocol to which this rule applies. For protocol forwarding, valid options are TCP, UDP, ESP, AH, SCTP, ICMP and L3_DEFAULT. The valid IP protocols are different for different load balancing products as described in [Load balancing features](https://cloud.google.com/load-balancing/docs/features#protocols_from_the_load_balancer_to_the_backends).
-                Enum type. Allowed values:
+            Enum type. Allowed values:
                 "AH"
                 "ESP"
                 "ICMP"
                 "L3_DEFAULT"
                 "SCTP"
                 "TCP"
                 "UDP". Defaults to None.
 
         target(str, Optional):
             The URL of the target resource to receive the matched traffic. For regional forwarding rules, this target must be in the same region as the forwarding rule. For global forwarding rules, this target must be a global load balancing resource. The forwarded traffic must be of a type appropriate to the target object. For more information, see the "Target" column in [Port specifications](https://cloud.google.com/load-balancing/docs/forwarding-rule-concepts#ip_address_specifications). For Private Service Connect forwarding rules that forward traffic to Google APIs, provide the name of a supported Google API bundle: - vpc-sc - APIs that support VPC Service Controls. - all-apis - All supported Google APIs. . Defaults to None.
 
         ip_version(str, Optional):
             The IP Version that will be used by this forwarding rule. Valid options are IPV4 or IPV6.
-                Enum type. Allowed values:
+            Enum type. Allowed values:
                 "IPV4"
                 "IPV6"
                 "UNSPECIFIED_VERSION". Defaults to None.
 
         is_mirroring_collector(bool, Optional):
             Indicates whether or not this load balancer can be used as a collector for packet mirroring. To prevent mirroring loops, instances behind this load balancer will not have their traffic mirrored even if a PacketMirroring rule applies to them. This can only be set to true for load balancers that have their loadBalancingScheme set to INTERNAL. Defaults to None.
 
         network_tier(str, Optional):
             This signifies the networking tier used for configuring this load balancer and can only take the following values: PREMIUM, STANDARD. For regional ForwardingRule, the valid values are PREMIUM and STANDARD. For GlobalForwardingRule, the valid value is PREMIUM. If this field is not specified, it is assumed to be PREMIUM. If IPAddress is specified, this value must be equal to the networkTier of the Address.
-                Enum type. Allowed values:
+            Enum type. Allowed values:
                 "FIXED_STANDARD" - Public internet quality with fixed bandwidth.
                 "PREMIUM" - High quality, Google-grade network tier, support for all networking products.
                 "STANDARD" - Public internet quality, only limited support for other networking products.
                 "STANDARD_OVERRIDES_FIXED_STANDARD" - (Output only) Temporary tier for FIXED_STANDARD when fixed standard tier is expired or not configured. Defaults to None.
 
         no_automate_dns_zone(bool, Optional):
             This is used in PSC consumer ForwardingRule to control whether it should try to auto-generate a DNS zone or not. Non-PSC forwarding rules do not use this field. Defaults to None.
@@ -146,52 +149,54 @@
             IP address for which this forwarding rule accepts traffic. When a client sends traffic to this IP address, the forwarding rule directs the traffic to the referenced target or backendService. While creating a forwarding rule, specifying an IPAddress is required under the following circumstances: - When the target is set to targetGrpcProxy and validateForProxyless is set to true, the IPAddress should be set to 0.0.0.0. - When the target is a Private Service Connect Google APIs bundle, you must specify an IPAddress. Otherwise, you can optionally specify an IP address that references an existing static (reserved) IP address resource. When omitted, Google Cloud assigns an ephemeral IP address. Use one of the following formats to specify an IP address while creating a forwarding rule: * IP address number, as in `100.1.2.3` * IPv6 address range, as in `2600:1234::/96` * Full resource URL, as in https://www.googleapis.com/compute/v1/projects/ project_id/regions/region/addresses/address-name * Partial URL or by name, as in: - projects/project_id/regions/region/addresses/address-name - regions/region/addresses/address-name - global/addresses/address-name - address-name The forwarding rule's target or backendService, and in most cases, also the loadBalancingScheme, determine the type of IP address that you can use. For detailed information, see [IP address specifications](https://cloud.google.com/load-balancing/docs/forwarding-rule-concepts#ip_address_specifications). When reading an IPAddress, the API always returns the IP address number. Defaults to None.
 
         network(str, Optional):
             This field is not used for external load balancing. For Internal TCP/UDP Load Balancing, this field identifies the network that the load balanced IP should belong to for this Forwarding Rule. If this field is not specified, the default network will be used. For Private Service Connect forwarding rules that forward traffic to Google APIs, a network must be provided. Defaults to None.
 
         psc_connection_status(str, Optional):
             Enum type. Allowed values:
-            "ACCEPTED" - The connection has been accepted by the producer.
-            "CLOSED" - The connection has been closed by the producer and will not serve traffic going forward.
-            "NEEDS_ATTENTION" - The connection has been accepted by the producer, but the producer needs to take further action before the forwarding rule can serve traffic.
-            "PENDING" - The connection is pending acceptance by the producer.
-            "REJECTED" - The connection has been rejected by the producer.
-            "STATUS_UNSPECIFIED". Defaults to None.
+                "ACCEPTED" - The connection has been accepted by the producer.
+                "CLOSED" - The connection has been closed by the producer and will not serve traffic going forward.
+                "NEEDS_ATTENTION" - The connection has been accepted by the producer, but the producer needs to take further action before the forwarding rule can serve traffic.
+                "PENDING" - The connection is pending acceptance by the producer.
+                "REJECTED" - The connection has been rejected by the producer.
+                "STATUS_UNSPECIFIED". Defaults to None.
 
         label_fingerprint(str, Optional):
             A fingerprint for the labels being applied to this resource, which is essentially a hash of the labels set used for optimistic locking. The fingerprint is initially generated by Compute Engine and changes after every request to modify or update labels. You must always provide an up-to-date fingerprint hash in order to update or change labels, otherwise the request will fail with error 412 conditionNotMet. To see the latest fingerprint, make a get() request to retrieve a ForwardingRule. Defaults to None.
 
         region(str):
             Name of the region scoping this request.
 
         subnetwork(str, Optional):
             This field identifies the subnetwork that the load balanced IP should belong to for this Forwarding Rule, used in internal load balancing and network load balancing with IPv6. If the network specified is in auto subnet mode, this field is optional. However, a subnetwork must be specified if the network is in custom subnet mode or when creating external forwarding rule with IPv6. Defaults to None.
 
         metadata_filters(List[Dict[str, Any]], Optional):
             Opaque filter criteria used by load balancer to restrict routing configuration to a limited set of xDS compliant clients. In their xDS requests to load balancer, xDS clients present node metadata. When there is a match, the relevant configuration is made available to those proxies. Otherwise, all the resources (e.g. TargetHttpProxy, UrlMap) referenced by the ForwardingRule are not visible to those proxies. For each metadataFilter in this list, if its filterMatchCriteria is set to MATCH_ANY, at least one of the filterLabels must match the corresponding label provided in the metadata. If its filterMatchCriteria is set to MATCH_ALL, then all of its filterLabels must match with corresponding labels provided in the metadata. If multiple metadataFilters are specified, all of them need to be satisfied in order to be considered a match. metadataFilters specified here will be applifed before those specified in the UrlMap that this ForwardingRule references. metadataFilters only applies to Loadbalancers that have their loadBalancingScheme set to INTERNAL_SELF_MANAGED. Defaults to None.
 
-            * filter_match_criteria (str, Optional):
+            * filter_match_criteria(str, Optional):
                 Specifies how individual filter label matches within the list of filterLabels and contributes toward the overall metadataFilter match. Supported values are: - MATCH_ANY: at least one of the filterLabels must have a matching label in the provided metadata. - MATCH_ALL: all filterLabels must have matching labels in the provided metadata.
-                    Enum type. Allowed values:
+                Enum type. Allowed values:
                     "MATCH_ALL" - Specifies that all filterLabels must match for the metadataFilter to be considered a match.
                     "MATCH_ANY" - Specifies that any filterLabel must match for the metadataFilter to be considered a match.
                     "NOT_SET" - Indicates that the match criteria was not set. A metadataFilter must never be created with this value.
 
-            * filter_labels (List[Dict[str, Any]], Optional): The list of label value pairs that must match labels in the provided metadata based on filterMatchCriteria This list must not be empty and can have at the most 64 entries.
-            * name (str, Optional): Name of metadata label. The name can have a maximum length of 1024 characters and must be at least 1 character long.
-            * value (str, Optional): The value of the label must match the specified value. value can have a maximum length of 1024 characters.
+            * filter_labels(List[Dict[str, Any]], Optional): The list of label value pairs that must match labels in the provided metadata based on filterMatchCriteria This list must not be empty and can have at the most 64 entries.
+                * name(str, Optional):
+                    Name of metadata label. The name can have a maximum length of 1024 characters and must be at least 1 character long.
+                * value(str, Optional):
+                    The value of the label must match the specified value. value can have a maximum length of 1024 characters.
         all_ports(bool, Optional):
             This field is used along with the backend_service field for Internal TCP/UDP Load Balancing or Network Load Balancing, or with the target field for internal and external TargetInstance. You can only use one of ports and port_range, or allPorts. The three are mutually exclusive. For TCP, UDP and SCTP traffic, packets addressed to any ports will be forwarded to the target or backendService. Defaults to None.
 
         service_label(str, Optional):
             An optional prefix to the service name for this Forwarding Rule. If specified, the prefix is the first label of the fully qualified service name. The label must be 1-63 characters long, and comply with RFC1035. Specifically, the label must be 1-63 characters long and match the regular expression `[a-z]([-a-z0-9]*[a-z0-9])?` which means the first character must be a lowercase letter, and all following characters must be a dash, lowercase letter, or digit, except the last character, which cannot be a dash. This field is only used for internal load balancing. Defaults to None.
 
         load_balancing_scheme(str, Optional):
             Specifies the forwarding rule type. For more information about forwarding rules, refer to Forwarding rule concepts.
-                Enum type. Allowed values:
+            Enum type. Allowed values:
                 "EXTERNAL"
                 "EXTERNAL_MANAGED"
                 "INTERNAL"
                 "INTERNAL_MANAGED"
                 "INTERNAL_SELF_MANAGED"
                 "INVALID". Defaults to None.
```

### Comparing `idem_gcp-1.1.0/idem_gcp/states/gcp/compute/health_check.py` & `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/health_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,127 +113,127 @@
 
         project(str):
             Project ID for this request.
 
         ssl_health_check(Dict[str, Any], Optional):
             Defaults to None.
 
-            * port_name (str, Optional):
+            * port_name(str, Optional):
                 Not supported.
 
-            * response (str, Optional):
+            * response(str, Optional):
                 Creates a content-based SSL health check. In addition to establishing a TCP connection and the TLS handshake, you can configure the health check to pass only when the backend sends this exact response ASCII string, up to 1024 bytes in length. For details, see: https://cloud.google.com/load-balancing/docs/health-check-concepts#criteria-protocol-ssl-tcp
 
-            * proxy_header (str, Optional):
+            * proxy_header(str, Optional):
                 Specifies the type of proxy header to append before sending data to the backend, either NONE or PROXY_V1. The default is NONE.
 
-            * port_specification (str, Optional):
+            * port_specification(str, Optional):
                 Specifies how a port is selected for health checking. Can be one of the following values: USE_FIXED_PORT: Specifies a port number explicitly using the port field in the health check. Supported by backend services for pass-through load balancers and backend services for proxy load balancers. Not supported by target pools. The health check supports all backends supported by the backend service provided the backend can be health checked. For example, GCE_VM_IP network endpoint groups, GCE_VM_IP_PORT network endpoint groups, and instance group backends. USE_NAMED_PORT: Not supported. USE_SERVING_PORT: Provides an indirect method of specifying the health check port by referring to the backend service. Only supported by backend services for proxy load balancers. Not supported by target pools. Not supported by backend services for pass-through load balancers. Supports all backends that can be health checked; for example, GCE_VM_IP_PORT network endpoint groups and instance group backends. For GCE_VM_IP_PORT network endpoint group backends, the health check uses the port number specified for each endpoint in the network endpoint group. For instance group backends, the health check uses the port number determined by looking up the backend service's named port in the instance group's list of named ports.
-                    Enum type. Allowed values:
-                        "USE_FIXED_PORT" - The port number in the health check's port is used for health checking. Applies to network endpoint group and instance group backends.
-                        "USE_NAMED_PORT" - Not supported.
-                        "USE_SERVING_PORT" - For network endpoint group backends, the health check uses the port number specified on each endpoint in the network endpoint group. For instance group backends, the health check uses the port number specified for the backend service's named port defined in the instance group's named ports.
+                Enum type. Allowed values:
+                    "USE_FIXED_PORT" - The port number in the health check's port is used for health checking. Applies to network endpoint group and instance group backends.
+                    "USE_NAMED_PORT" - Not supported.
+                    "USE_SERVING_PORT" - For network endpoint group backends, the health check uses the port number specified on each endpoint in the network endpoint group. For instance group backends, the health check uses the port number specified for the backend service's named port defined in the instance group's named ports.
 
-            * port (int, Optional):
+            * port(int, Optional):
                 The TCP port number to which the health check prober sends packets. The default value is 443. Valid values are 1 through 65535.
 
-            * request (str, Optional):
+            * request(str, Optional):
                 Instructs the health check prober to send this exact ASCII string, up to 1024 bytes in length, after establishing the TCP connection and SSL handshake.
 
         https_health_check(Dict[str, Any], Optional):
             Defaults to None.
 
-            * host (str, Optional):
+            * host(str, Optional):
                 The value of the host header in the HTTPS health check request. If left empty (default value), the host header is set to the destination IP address to which health check packets are sent. The destination IP address depends on the type of load balancer. For details, see: https://cloud.google.com/load-balancing/docs/health-check-concepts#hc-packet-dest
 
             * port_specification (str, Optional):
                 Specifies how a port is selected for health checking. Can be one of the following values: USE_FIXED_PORT: Specifies a port number explicitly using the port field in the health check. Supported by backend services for pass-through load balancers and backend services for proxy load balancers. Not supported by target pools. The health check supports all backends supported by the backend service provided the backend can be health checked. For example, GCE_VM_IP network endpoint groups, GCE_VM_IP_PORT network endpoint groups, and instance group backends. USE_NAMED_PORT: Not supported. USE_SERVING_PORT: Provides an indirect method of specifying the health check port by referring to the backend service. Only supported by backend services for proxy load balancers. Not supported by target pools. Not supported by backend services for pass-through load balancers. Supports all backends that can be health checked; for example, GCE_VM_IP_PORT network endpoint groups and instance group backends. For GCE_VM_IP_PORT network endpoint group backends, the health check uses the port number specified for each endpoint in the network endpoint group. For instance group backends, the health check uses the port number determined by looking up the backend service's named port in the instance group's list of named ports.
-                    Enum type. Allowed values:
-                        "USE_FIXED_PORT" - The port number in the health check's port is used for health checking. Applies to network endpoint group and instance group backends.
-                        "USE_NAMED_PORT" - Not supported.
-                        "USE_SERVING_PORT" - For network endpoint group backends, the health check uses the port number specified on each endpoint in the network endpoint group. For instance group backends, the health check uses the port number specified for the backend service's named port defined in the instance group's named ports.
+                Enum type. Allowed values:
+                    "USE_FIXED_PORT" - The port number in the health check's port is used for health checking. Applies to network endpoint group and instance group backends.
+                    "USE_NAMED_PORT" - Not supported.
+                    "USE_SERVING_PORT" - For network endpoint group backends, the health check uses the port number specified on each endpoint in the network endpoint group. For instance group backends, the health check uses the port number specified for the backend service's named port defined in the instance group's named ports.
 
             * port_name (str, Optional):
                 Not supported.
 
             * proxy_header (str, Optional):
                 Specifies the type of proxy header to append before sending data to the backend, either NONE or PROXY_V1. The default is NONE.
-                    Enum type. Allowed values:
-                        "NONE"
-                        "PROXY_V1"
+                Enum type. Allowed values:
+                    "NONE"
+                    "PROXY_V1"
 
             * request_path (str, Optional):
                 The request path of the HTTPS health check request. The default value is /.
 
             * port (int, Optional):
                 The TCP port number to which the health check prober sends packets. The default value is 443. Valid values are 1 through 65535.
 
             * response (str, Optional):
                 Creates a content-based HTTPS health check. In addition to the required HTTP 200 (OK) status code, you can configure the health check to pass only when the backend sends this specific ASCII response string within the first 1024 bytes of the HTTP response body. For details, see: https://cloud.google.com/load-balancing/docs/health-check-concepts#criteria-protocol-http
 
         type(str, Optional):
             Specifies the type of the healthCheck, either TCP, SSL, HTTP, HTTPS, HTTP2 or GRPC. Exactly one of the protocol-specific health check fields must be specified, which must match type field.
-                Enum type. Allowed values:
-                    "GRPC"
-                    "HTTP"
-                    "HTTP2"
-                    "HTTPS"
-                    "INVALID"
-                    "SSL"
-                    "TCP". Defaults to None.
+            Enum type. Allowed values:
+                "GRPC"
+                "HTTP"
+                "HTTP2"
+                "HTTPS"
+                "INVALID"
+                "SSL"
+                "TCP". Defaults to None.
 
         description(str, Optional):
             An optional description of this resource. Provide this property when you create the resource. Defaults to None.
 
         http2_health_check(Dict[str, Any], Optional):
             Defaults to None.
 
             * port_specification (str, Optional):
                 Specifies how a port is selected for health checking. Can be one of the following values: USE_FIXED_PORT: Specifies a port number explicitly using the port field in the health check. Supported by backend services for pass-through load balancers and backend services for proxy load balancers. Not supported by target pools. The health check supports all backends supported by the backend service provided the backend can be health checked. For example, GCE_VM_IP network endpoint groups, GCE_VM_IP_PORT network endpoint groups, and instance group backends. USE_NAMED_PORT: Not supported. USE_SERVING_PORT: Provides an indirect method of specifying the health check port by referring to the backend service. Only supported by backend services for proxy load balancers. Not supported by target pools. Not supported by backend services for pass-through load balancers. Supports all backends that can be health checked; for example, GCE_VM_IP_PORT network endpoint groups and instance group backends. For GCE_VM_IP_PORT network endpoint group backends, the health check uses the port number specified for each endpoint in the network endpoint group. For instance group backends, the health check uses the port number determined by looking up the backend service's named port in the instance group's list of named ports.
-                    Enum type. Allowed values:
-                        "USE_FIXED_PORT" - The port number in the health check's port is used for health checking. Applies to network endpoint group and instance group backends.
-                        "USE_NAMED_PORT" - Not supported.
-                        "USE_SERVING_PORT" - For network endpoint group backends, the health check uses the port number specified on each endpoint in the network endpoint group. For instance group backends, the health check uses the port number specified for the backend service's named port defined in the instance group's named ports.
+                Enum type. Allowed values:
+                    "USE_FIXED_PORT" - The port number in the health check's port is used for health checking. Applies to network endpoint group and instance group backends.
+                    "USE_NAMED_PORT" - Not supported.
+                    "USE_SERVING_PORT" - For network endpoint group backends, the health check uses the port number specified on each endpoint in the network endpoint group. For instance group backends, the health check uses the port number specified for the backend service's named port defined in the instance group's named ports.
 
             * port (int, Optional):
                 The TCP port number to which the health check prober sends packets. The default value is 443. Valid values are 1 through 65535.
 
             * port_name (str, Optional):
                 Not supported.
 
             * request_path (str, Optional):
                 The request path of the HTTP/2 health check request. The default value is /.
 
             * proxy_header (str, Optional):
                 Specifies the type of proxy header to append before sending data to the backend, either NONE or PROXY_V1. The default is NONE.
-                    Enum type. Allowed values:
-                        "NONE"
-                        "PROXY_V1"
+                Enum type. Allowed values:
+                    "NONE"
+                    "PROXY_V1"
 
             * response (str, Optional):
                 Creates a content-based HTTP/2 health check. In addition to the required HTTP 200 (OK) status code, you can configure the health check to pass only when the backend sends this specific ASCII response string within the first 1024 bytes of the HTTP response body. For details, see: https://cloud.google.com/load-balancing/docs/health-check-concepts#criteria-protocol-http
 
             * host (str, Optional):
                 The value of the host header in the HTTP/2 health check request. If left empty (default value), the host header is set to the destination IP address to which health check packets are sent. The destination IP address depends on the type of load balancer. For details, see: https://cloud.google.com/load-balancing/docs/health-check-concepts#hc-packet-dest
 
         tcp_health_check(Dict[str, Any], Optional):
             Defaults to None.
 
             * proxy_header (str, Optional):
                 Specifies the type of proxy header to append before sending data to the backend, either NONE or PROXY_V1. The default is NONE.
-                    Enum type. Allowed values:
-                        "NONE"
-                        "PROXY_V1"
+                Enum type. Allowed values:
+                    "NONE"
+                    "PROXY_V1"
 
             * port_specification (str, Optional):
                 Specifies how a port is selected for health checking. Can be one of the following values: USE_FIXED_PORT: Specifies a port number explicitly using the port field in the health check. Supported by backend services for pass-through load balancers and backend services for proxy load balancers. Not supported by target pools. The health check supports all backends supported by the backend service provided the backend can be health checked. For example, GCE_VM_IP network endpoint groups, GCE_VM_IP_PORT network endpoint groups, and instance group backends. USE_NAMED_PORT: Not supported. USE_SERVING_PORT: Provides an indirect method of specifying the health check port by referring to the backend service. Only supported by backend services for proxy load balancers. Not supported by target pools. Not supported by backend services for pass-through load balancers. Supports all backends that can be health checked; for example, GCE_VM_IP_PORT network endpoint groups and instance group backends. For GCE_VM_IP_PORT network endpoint group backends, the health check uses the port number specified for each endpoint in the network endpoint group. For instance group backends, the health check uses the port number determined by looking up the backend service's named port in the instance group's list of named ports.
-                    Enum type. Allowed values:
-                        "USE_FIXED_PORT" - The port number in the health check's port is used for health checking. Applies to network endpoint group and instance group backends.
-                        "USE_NAMED_PORT" - Not supported.
-                        "USE_SERVING_PORT" - For network endpoint group backends, the health check uses the port number specified on each endpoint in the network endpoint group. For instance group backends, the health check uses the port number specified for the backend service's named port defined in the instance group's named ports.
+                Enum type. Allowed values:
+                    "USE_FIXED_PORT" - The port number in the health check's port is used for health checking. Applies to network endpoint group and instance group backends.
+                    "USE_NAMED_PORT" - Not supported.
+                    "USE_SERVING_PORT" - For network endpoint group backends, the health check uses the port number specified on each endpoint in the network endpoint group. For instance group backends, the health check uses the port number specified for the backend service's named port defined in the instance group's named ports.
 
             * response (str, Optional):
                 Creates a content-based TCP health check. In addition to establishing a TCP connection, you can configure the health check to pass only when the backend sends this exact response ASCII string, up to 1024 bytes in length. For details, see: https://cloud.google.com/load-balancing/docs/health-check-concepts#criteria-protocol-ssl-tcp
             * request (str, Optional):
                 Instructs the health check prober to send this exact ASCII string, up to 1024 bytes in length, after establishing the TCP connection.
             * port_name (str, Optional):
                 Not supported.
@@ -257,18 +257,18 @@
                 Indicates whether or not to export logs. This is false by default, which means no health check logging will be done.
 
         grpc_health_check(Dict[str, Any], Optional):
             Defaults to None.
 
             * port_specification (str, Optional):
                 Specifies how a port is selected for health checking. Can be one of the following values: USE_FIXED_PORT: Specifies a port number explicitly using the port field in the health check. Supported by backend services for pass-through load balancers and backend services for proxy load balancers. Not supported by target pools. The health check supports all backends supported by the backend service provided the backend can be health checked. For example, GCE_VM_IP network endpoint groups, GCE_VM_IP_PORT network endpoint groups, and instance group backends. USE_NAMED_PORT: Not supported. USE_SERVING_PORT: Provides an indirect method of specifying the health check port by referring to the backend service. Only supported by backend services for proxy load balancers. Not supported by target pools. Not supported by backend services for pass-through load balancers. Supports all backends that can be health checked; for example, GCE_VM_IP_PORT network endpoint groups and instance group backends. For GCE_VM_IP_PORT network endpoint group backends, the health check uses the port number specified for each endpoint in the network endpoint group. For instance group backends, the health check uses the port number determined by looking up the backend service's named port in the instance group's list of named ports.
-                    Enum type. Allowed values:
-                        "USE_FIXED_PORT" - The port number in the health check's port is used for health checking. Applies to network endpoint group and instance group backends.
-                        "USE_NAMED_PORT" - Not supported.
-                        "USE_SERVING_PORT" - For network endpoint group backends, the health check uses the port number specified on each endpoint in the network endpoint group. For instance group backends, the health check uses the port number specified for the backend service's named port defined in the instance group's named ports.
+                Enum type. Allowed values:
+                    "USE_FIXED_PORT" - The port number in the health check's port is used for health checking. Applies to network endpoint group and instance group backends.
+                    "USE_NAMED_PORT" - Not supported.
+                    "USE_SERVING_PORT" - For network endpoint group backends, the health check uses the port number specified on each endpoint in the network endpoint group. For instance group backends, the health check uses the port number specified for the backend service's named port defined in the instance group's named ports.
 
             * grpc_service_name (str, Optional):
                 The gRPC service name for the health check. This field is optional. The value of grpc_service_name has the following meanings by convention: - Empty service_name means the overall status of all services at the backend. - Non-empty service_name means the health of that gRPC service, as defined by the owner of the service. The grpc_service_name can only be ASCII.
 
             * port_name (str, Optional):
                 Not supported.
 
@@ -288,27 +288,27 @@
                 The value of the host header in the HTTP health check request. If left empty (default value), the host header is set to the destination IP address to which health check packets are sent. The destination IP address depends on the type of load balancer. For details, see: https://cloud.google.com/load-balancing/docs/health-check-concepts#hc-packet-dest
 
             * response (str, Optional):
                 Creates a content-based HTTP health check. In addition to the required HTTP 200 (OK) status code, you can configure the health check to pass only when the backend sends this specific ASCII response string within the first 1024 bytes of the HTTP response body. For details, see: https://cloud.google.com/load-balancing/docs/health-check-concepts#criteria-protocol-http
 
             * port_specification (str, Optional):
                 Specifies how a port is selected for health checking. Can be one of the following values: USE_FIXED_PORT: Specifies a port number explicitly using the port field in the health check. Supported by backend services for pass-through load balancers and backend services for proxy load balancers. Also supported in legacy HTTP health checks for target pools. The health check supports all backends supported by the backend service provided the backend can be health checked. For example, GCE_VM_IP network endpoint groups, GCE_VM_IP_PORT network endpoint groups, and instance group backends. USE_NAMED_PORT: Not supported. USE_SERVING_PORT: Provides an indirect method of specifying the health check port by referring to the backend service. Only supported by backend services for proxy load balancers. Not supported by target pools. Not supported by backend services for pass-through load balancers. Supports all backends that can be health checked; for example, GCE_VM_IP_PORT network endpoint groups and instance group backends. For GCE_VM_IP_PORT network endpoint group backends, the health check uses the port number specified for each endpoint in the network endpoint group. For instance group backends, the health check uses the port number determined by looking up the backend service's named port in the instance group's list of named ports.
-                    Enum type. Allowed values:
-                        "USE_FIXED_PORT" - The port number in the health check's port is used for health checking. Applies to network endpoint group and instance group backends.
-                        "USE_NAMED_PORT" - Not supported.
-                        "USE_SERVING_PORT" - For network endpoint group backends, the health check uses the port number specified on each endpoint in the network endpoint group. For instance group backends, the health check uses the port number specified for the backend service's named port defined in the instance group's named ports.
+                Enum type. Allowed values:
+                    "USE_FIXED_PORT" - The port number in the health check's port is used for health checking. Applies to network endpoint group and instance group backends.
+                    "USE_NAMED_PORT" - Not supported.
+                    "USE_SERVING_PORT" - For network endpoint group backends, the health check uses the port number specified on each endpoint in the network endpoint group. For instance group backends, the health check uses the port number specified for the backend service's named port defined in the instance group's named ports.
 
             * port_name (str, Optional):
                 Not supported.
 
             * proxy_header (str, Optional):
                 Specifies the type of proxy header to append before sending data to the backend, either NONE or PROXY_V1. The default is NONE.
-                    Enum type. Allowed values:
-                        "NONE"
-                        "PROXY_V1"
+                Enum type. Allowed values:
+                    "NONE"
+                    "PROXY_V1"
 
         healthy_threshold(int, Optional):
             A so-far unhealthy instance will be marked healthy after this many consecutive successes. The default value is 2. Defaults to None.
 
         health_check(str):
             Name of the HealthCheck resource to return.
```

### Comparing `idem_gcp-1.1.0/idem_gcp/states/gcp/compute/image.py` & `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/image.py`

 * *Files 16% similar despite different names*

```diff
@@ -283,18 +283,22 @@
                 \"kms_key_service_account\":
                 \"name@project_id.iam.gserviceaccount.com/
 
         source_disk_encryption_key(Dict[str, Any], Optional):
             The customer-supplied encryption key of the source disk.
             Required if the source disk is protected by a customer-supplied encryption key."
 
-            * raw_key(str, Optional)
-            * rsa_encrypted_key(str, Optional)
-            * kms_key_name(str, Optional)
-            * kms_key_service_account(str, Optional)
+            * raw_key(str, Optional):
+                Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
+            * rsa_encrypted_key(str, Optional):
+                Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
+            * kms_key_name(str, Optional):
+                The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
+            * kms_key_service_account(str, Optional):
+                The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/
 
         labels(Dict[str, str], Optional):
             Labels to apply to this image. These can be later modified by the setLabels method.
 
         label_fingerprint(str, Optional):
             A fingerprint for the labels being applied to this image, which is essentially a hash of the labels
             used for optimistic locking. The fingerprint is initially generated by Compute Engine and changes after
@@ -302,15 +306,15 @@
             in order to update or change labels, otherwise the request will fail with error 412 conditionNotMet.
             To see the latest fingerprint, make a get() request to retrieve an image.
 
         guest_os_features(List[Dict[str, Any]], Optional):
             A list of features to enable on the guest operating system. Applicable only for bootable images.
             To see a list of available options, see the guestOSfeatures[].type parameter.
 
-            * type (str, Optional):
+            * type(str, Optional):
                 The ID of a supported feature. To add multiple values,
                 use commas to separate values. Set to one or more of the following values:
 
                 - VIRTIO_SCSI_MULTIQUEUE
                 - WINDOWS
                 - MULTI_IP_SUBNET
                 - UEFI_COMPATIBLE
@@ -337,18 +341,22 @@
             - The sourceImage URL
             - The sourceSnapshot URL
 
         source_image_encryption_key(Dict[str, Any], Optional):
             The customer-supplied encryption key of the source image.
             Required if the source image is protected by a customer-supplied encryption key.
 
-            * raw_key(str, Optional)
-            * rsa_encrypted_key(str, Optional)
-            * kms_key_name(str, Optional)
-            * kms_key_service_account(str, Optional)
+            * raw_key(str, Optional):
+                Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
+            * rsa_encrypted_key(str, Optional):
+                Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
+            * kms_key_name(str, Optional):
+                The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
+            * kms_key_service_account(str, Optional):
+                The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/
 
         source_snapshot(str, Optional):
             URL of the source snapshot used to create this image. The following are valid formats for the URL:
 
             - https://www.googleapis.com/compute/v1/projects/project_id/global/snapshots/snapshot_name
             - projects/project_id/global/snapshots/snapshot_name
 
@@ -359,50 +367,74 @@
             - The sourceImage URL
             - The sourceSnapshot URL
 
         source_snapshot_encryption_key(Dict[str, Any], Optional):
             The customer-supplied encryption key of the source snapshot.
             Required if the source snapshot is protected by a customer-supplied encryption key.
 
-            * raw_key(str, Optional)
-            * rsa_encrypted_key(str, Optional)
-            * kms_key_name(str, Optional)
-            * kms_key_service_account(str, Optional)
+            * raw_key(str, Optional):
+                Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
+            * rsa_encrypted_key(str, Optional):
+                Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
+            * kms_key_name(str, Optional):
+                The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
+            * kms_key_service_account(str, Optional):
+                The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/
 
         storage_locations(List[str], Optional):
             Cloud Storage bucket storage location of the image (regional or multi-regional).
 
         shielded_instance_initial_state(Dict[str, Any], Optional):
             Set the secure boot keys of shielded instance.
 
             * keks(List[Dict[str, Any]], Optional):
                 The Key Exchange Key (KEK).
 
-                * content(str, Optional):
-                    The raw content in the secure keys file.
                 * file_type(str, Optional):
                     The file type of source file.
-
-            * pk(Dict[str, Any], Optional):
-                The Platform Key (PK).
-
-                * content(str, Optional)
-                * file_type(str, Optional)
-
+                    Enum type. Allowed values:
+                        "BIN"
+                        "UNDEFINED"
+                        "X509"
+                * content(str, Optional):
+                    The raw content in the secure keys file.
             * dbs(List[Dict[str, Any]], Optional):
                 The Key Database (db).
 
-                * content(str, Optional)
-                * file_type(str, Optional)
+                * file_type (str, Optional):
+                    The file type of source file.
+                    Enum type. Allowed values:
+                        "BIN"
+                        "UNDEFINED"
+                        "X509"
+                * content (str, Optional):
+                    The raw content in the secure keys file.
 
-            * dbxs(List[Dict[str, Any]], Optional):
+            * dbxs (List[Dict[str, Any]], Optional):
                 The forbidden key database (dbx).
 
-                * content(str, Optional)
-                * file_type(str, Optional)
+                * file_type (str, Optional):
+                    The file type of source file.
+                    Enum type. Allowed values:
+                        "BIN"
+                        "UNDEFINED"
+                        "X509"
+                * content (str, Optional):
+                    The raw content in the secure keys file.
+            * pk (Dict[str, Any], Optional):
+                The Platform Key (PK).
+
+                * file_type (str, Optional):
+                    The file type of source file.
+                    Enum type. Allowed values:
+                        "BIN"
+                        "UNDEFINED"
+                        "X509"
+                * content (str, Optional):
+                    The raw content in the secure keys file.
 
         architecture(str, Optional):
             The architecture of the image. Valid values are ARM64 or X86_64.
 
     Returns:
         Dict[str, Any]
```

### Comparing `idem_gcp-1.1.0/idem_gcp/states/gcp/compute/instance.py` & `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -427,17 +427,17 @@
     Args:
         name(str):
             An Idem name of the resource.
 
         service_accounts(List[Dict[str, Any]], Optional):
             A list of service accounts, with their specified scopes, authorized for this instance. Only one service account per VM instance is supported. Service accounts generate access tokens that can be accessed through the metadata server and used to authenticate applications on the instance. See Service Accounts for more information. Defaults to None.
 
-            * scopes (List[str], Optional):
+            * scopes(List[str], Optional):
                 The list of scopes to be made available for this service account.
-            * email (str, Optional):
+            * email(str, Optional):
                 Email address of the service account.
 
         label_fingerprint(str, Optional):
             A fingerprint for this request, which is essentially a hash of the label's contents and used for optimistic locking. The fingerprint is initially generated by Compute Engine and changes after every request to modify or update labels. You must always provide an up-to-date fingerprint hash in order to update or change labels. To see the latest fingerprint, make get() request to the instance. Defaults to None.
 
         fingerprint(str, Optional):
             Specifies a fingerprint for this resource, which is essentially a hash of the instance's contents and used for optimistic locking. The fingerprint is initially generated by Compute Engine and changes after every request to modify or update the instance. You must always provide an up-to-date fingerprint hash in order to update the instance. To see the latest fingerprint, make get() request to the instance. Defaults to None.
@@ -466,47 +466,47 @@
                 URL of the VPC network resource for this instance. When creating an instance, if neither the network nor the subnetwork is specified, the default network global/networks/default is used. If the selected project doesn't have the default network, you must specify a network or subnet. If the network is not specified but the subnetwork is specified, the network is inferred. If you specify this property, you can specify the network as a full or partial URL. For example, the following are all valid URLs:
 
                 - https://www.googleapis.com/compute/v1/projects/project/global/networks/network
                 - projects/project/global/networks/network
                 - global/networks/default
             * stack_type (str, Optional):
                 The stack type for this network interface to identify whether the IPv6 feature is enabled or not. If not specified, IPV4_ONLY will be used. This field can be both set at instance creation and update network interface operations.
-                    Enum type. Allowed values:
-                        "IPV4_IPV6" - The network interface can have both IPv4 and IPv6 addresses.
-                        "IPV4_ONLY" - The network interface will be assigned IPv4 address.
+                Enum type. Allowed values:
+                    "IPV4_IPV6" - The network interface can have both IPv4 and IPv6 addresses.
+                    "IPV4_ONLY" - The network interface will be assigned IPv4 address.
             * name (str, Optional):
                 [Output Only] The name of the network interface, which is generated by the server. For a VM, the network interface uses the nicN naming format. Where N is a value between 0 and 7. The default interface value is nic0.
             * subnetwork (str, Optional):
                 The URL of the Subnetwork resource for this instance. If the network resource is in legacy mode, do not specify this field. If the network is in auto subnet mode, specifying the subnetwork is optional. If the network is in custom subnet mode, specifying the subnetwork is required. If you specify this field, you can specify the subnetwork as a full or partial URL. For example, the following are all valid URLs:
 
                 - https://www.googleapis.com/compute/v1/projects/project/regions/region/subnetworks/subnetwork
                 - regions/region/subnetworks/subnetwork
             * queue_count (int, Optional):
                 The networking queue count that's specified by users for the network interface. Both Rx and Tx queues will be set to this number. It'll be empty if not specified by the users.
             * ipv6_access_configs (List[Dict[str, Any]], Optional):
                 An array of IPv6 access configurations for this interface. Currently, only one IPv6 access config, DIRECT_IPV6, is supported. If there is no ipv6AccessConfig specified, then this instance will have no external IPv6 Internet access.
 
                 * network_tier (str, Optional):
                     This signifies the networking tier used for configuring this access configuration and can only take the following values: PREMIUM, STANDARD. If an AccessConfig is specified without a valid external IP address, an ephemeral IP will be created with this networkTier. If an AccessConfig with a valid external IP address is specified, it must match that of the networkTier associated with the Address resource owning that IP.
-                        Enum type. Allowed values:
+                    Enum type. Allowed values:
                         "FIXED_STANDARD" - Public internet quality with fixed bandwidth.
                         "PREMIUM" - High quality, Google-grade network tier, support for all networking products.
                         "STANDARD" - Public internet quality, only limited support for other networking products.
                         "STANDARD_OVERRIDES_FIXED_STANDARD" - (Output only) Temporary tier for FIXED_STANDARD when fixed standard tier is expired or not configured.
                 * external_ipv6_prefix_length (int, Optional):
                     The prefix length of the external IPv6 range.
                 * name (str, Optional):
                     The name of this access configuration. The default and recommended name is External NAT, but you can use any arbitrary string, such as My external IP or Network Access.
                 * kind (str, Optional):
                     [Output Only] Type of the resource. Always compute#accessConfig for access configs.
                 * external_ipv6 (str, Optional):
                     The first IPv6 address of the external IPv6 range associated with this instance, prefix length is stored in externalIpv6PrefixLength in ipv6AccessConfig. The field is output only, an IPv6 address from a subnetwork associated with the instance will be allocated dynamically.
                 * type (str, Optional):
                     The type of configuration. The default and only option is ONE_TO_ONE_NAT.
-                        Enum type. Allowed values:
+                    Enum type. Allowed values:
                         "DIRECT_IPV6"
                         "ONE_TO_ONE_NAT"
                 * set_public_ptr (bool, Optional):
                     Specifies whether a public DNS 'PTR' record should be created to map the external IP address of the instance to a DNS domain name. This field is not used in ipv6AccessConfig. A default PTR record will be created if the VM has external IPv6 range associated.
                 * public_ptr_domain_name (str, Optional):
                     The DNS domain name for the public PTR record. You can set this field only if the `setPublicPtr` field is enabled in accessConfig. If this field is unspecified in ipv6AccessConfig, a default PTR record will be createc for first IP in associated external IPv6 range.
                 * nat_ip (str, Optional):
@@ -522,47 +522,49 @@
                 * ip_cidr_range (str, Optional):
                     The IP alias ranges to allocate for this interface. This IP CIDR range must belong to the specified subnetwork and cannot contain IP addresses reserved by system or used by other network interfaces. This range may be a single IP address (such as 10.2.3.4), a netmask (such as /24) or a CIDR-formatted string (such as 10.1.2.0/24).
                 * subnetwork_range_name (str, Optional):
                     The name of a subnetwork secondary IP range from which to allocate an IP alias range. If not specified, the primary range of the subnetwork is used.
 
             * ipv6_access_type (str, Optional):
                 [Output Only] One of EXTERNAL, INTERNAL to indicate whether the IP can be accessed from the Internet. This field is always inherited from its subnetwork. Valid only if stackType is IPV4_IPV6.
-                    Enum type. Allowed values:
+                Enum type. Allowed values:
                     "EXTERNAL" - This network interface can have external IPv6.
                     "INTERNAL" - This network interface can have internal IPv6.
+
             * network_ip (str, Optional):
                 An IPv4 internal IP address to assign to the instance for this network interface. If not specified by the user, an unused internal IP is assigned by the system.
+
             * nic_type (str, Optional):
                 The type of vNIC to be used on this interface. This may be gVNIC or VirtioNet.
-                    Enum type. Allowed values:
+                Enum type. Allowed values:
                     "GVNIC" - GVNIC
                     "UNSPECIFIED_NIC_TYPE" - No type specified.
                     "VIRTIO_NET" - VIRTIO
 
             * access_configs (List[Dict[str, Any]], Optional):
                 An array of configurations for this interface. Currently, only one access config, ONE_TO_ONE_NAT, is supported. If there are no accessConfigs specified, then this instance will have no external internet access.
 
                 * network_tier (str, Optional):
                     This signifies the networking tier used for configuring this access configuration and can only take the following values: PREMIUM, STANDARD. If an AccessConfig is specified without a valid external IP address, an ephemeral IP will be created with this networkTier. If an AccessConfig with a valid external IP address is specified, it must match that of the networkTier associated with the Address resource owning that IP.
-                        Enum type. Allowed values:
+                    Enum type. Allowed values:
                         "FIXED_STANDARD" - Public internet quality with fixed bandwidth.
                         "PREMIUM" - High quality, Google-grade network tier, support for all networking products.
                         "STANDARD" - Public internet quality, only limited support for other networking products.
                         "STANDARD_OVERRIDES_FIXED_STANDARD" - (Output only) Temporary tier for FIXED_STANDARD when fixed standard tier is expired or not configured.
                 * external_ipv6_prefix_length (int, Optional):
                     The prefix length of the external IPv6 range.
                 * name (str, Optional):
                     The name of this access configuration. The default and recommended name is External NAT, but you can use any arbitrary string, such as My external IP or Network Access.
                 * kind (str, Optional):
                     [Output Only] Type of the resource. Always compute#accessConfig for access configs.
                 * external_ipv6 (str, Optional):
                     The first IPv6 address of the external IPv6 range associated with this instance, prefix length is stored in externalIpv6PrefixLength in ipv6AccessConfig. The field is output only, an IPv6 address from a subnetwork associated with the instance will be allocated dynamically.
                 * type (str, Optional):
                     The type of configuration. The default and only option is ONE_TO_ONE_NAT.
-                        Enum type. Allowed values:
+                    Enum type. Allowed values:
                         "DIRECT_IPV6"
                         "ONE_TO_ONE_NAT"
                 * set_public_ptr (bool, Optional):
                     Specifies whether a public DNS 'PTR' record should be created to map the external IP address of the instance to a DNS domain name. This field is not used in ipv6AccessConfig. A default PTR record will be created if the VM has external IPv6 range associated.
                 * public_ptr_domain_name (str, Optional):
                     The DNS domain name for the public PTR record. You can set this field only if the `setPublicPtr` field is enabled in accessConfig. If this field is unspecified in ipv6AccessConfig, a default PTR record will be createc for first IP in associated external IPv6 range.
                 * nat_ip (str, Optional):
@@ -577,23 +579,20 @@
         display_device(Dict[str, Any], Optional):
             Enables display device for the instance.
             DisplayDevice: A set of Display Device options. Defaults to None.
 
             * enable_display (bool, Optional):
                 Defines whether the instance has Display enabled.
 
-        source_machine_image(str, Optional):
-            Source machine image. Defaults to None.
-
         resource_policies(List[str], Optional):
             Resource policies applied to this instance. Defaults to None.
 
         status(str, Optional):
             The status of the instance. One of the following values: PROVISIONING, STAGING, RUNNING, STOPPING, SUSPENDING, SUSPENDED, REPAIRING, and TERMINATED. For more information about the status of the instance, see Instance life cycle.
-                Enum type. Allowed values:
+            Enum type. Allowed values:
                 "DEPROVISIONING" - The Nanny is halted and we are performing tear down tasks like network deprogramming, releasing quota, IP, tearing down disks etc.
                 "PROVISIONING" - Resources are being allocated for the instance.
                 "REPAIRING" - The instance is in repair.
                 "RUNNING" - The instance is running.
                 "STAGING" - All required resources have been allocated and the instance is being started.
                 "STOPPED" - The instance has stopped successfully.
                 "STOPPING" - The instance is currently stopping (either being deleted or killed).
@@ -608,65 +607,66 @@
             * fingerprint (str, Optional):
                 Specifies a fingerprint for this request, which is essentially a hash of the tags' contents and used for optimistic locking. The fingerprint is initially generated by Compute Engine and changes after every request to modify or update tags. You must always provide an up-to-date fingerprint hash in order to update or change tags. To see the latest fingerprint, make get() request to the instance.
             * items (List[str], Optional):
                 An array of tags. Each tag must be 1-63 characters long, and comply with RFC1035.
 
         key_revocation_action_type(str, Optional):
             KeyRevocationActionType of the instance. Supported options are "STOP" and "NONE". The default value is "NONE" if it is not specified.
-                Enum type. Allowed values:
+            Enum type. Allowed values:
                 "KEY_REVOCATION_ACTION_TYPE_UNSPECIFIED" - Default value. This value is unused.
                 "NONE" - Indicates user chose no operation.
                 "STOP" - Indicates user chose to opt for VM shutdown on key revocation. Defaults to None.
 
         scheduling(Dict[str, Any], Optional):
             Sets the scheduling options for this instance.
             Scheduling: Sets the scheduling options for an Instance. Defaults to None.
 
             * on_host_maintenance (str, Optional):
                 Defines the maintenance behavior for this instance. For standard instances, the default behavior is MIGRATE. For preemptible instances, the default and only possible behavior is TERMINATE. For more information, see Set VM host maintenance policy.
-                    Enum type. Allowed values:
+                Enum type. Allowed values:
                     "MIGRATE" - *[Default]* Allows Compute Engine to automatically migrate instances out of the way of maintenance events.
                     "TERMINATE" - Tells Compute Engine to terminate and (optionally) restart the instance away from the maintenance activity. If you would like your instance to be restarted, set the automaticRestart flag to true. Your instance may be restarted more than once, and it may be restarted outside the window of maintenance events.
             * preemptible (bool, Optional):
                 Defines whether the instance is preemptible. This can only be set during instance creation or while the instance is stopped and therefore, in a `TERMINATED` state. See Instance Life Cycle for more information on the possible instance states.
             * min_node_cpus (int, Optional):
                 The minimum number of virtual CPUs this instance will consume when running on a sole-tenant node.
             * automatic_restart (bool, Optional):
                 Specifies whether the instance should be automatically restarted if it is terminated by Compute Engine (not terminated by a user). You can only set the automatic restart option for standard instances. Preemptible instances cannot be automatically restarted. By default, this is set to true so an instance is automatically restarted if it is terminated by Compute Engine.
             * node_affinities (List[Dict[str, Any]], Optional):
                 A set of node affinity and anti-affinity configurations. Refer to Configuring node affinity for more information. Overrides reservationAffinity.
 
                 * operator (str, Optional):
                     Defines the operation of node selection. Valid operators are IN for affinity and NOT_IN for anti-affinity.
-                        Enum type. Allowed values:
+                    Enum type. Allowed values:
                         "IN" - Requires Compute Engine to seek for matched nodes.
                         "NOT_IN" - Requires Compute Engine to avoid certain nodes.
                         "OPERATOR_UNSPECIFIED"
+
                 * values (List[str], Optional):
                     Corresponds to the label values of Node resource.
                 * key (str, Optional):
                     Corresponds to the label key of Node resource.
 
             * instance_termination_action (str, Optional):
                 Specifies the termination action for the instance.
-                    Enum type. Allowed values:
+                Enum type. Allowed values:
                     "DELETE" - Delete the VM.
                     "INSTANCE_TERMINATION_ACTION_UNSPECIFIED" - Default value. This value is unused.
                     "STOP" - Stop the VM without storing in-memory content. default action.
             * provisioning_model (str, Optional):
                 Specifies the provisioning model of the instance.
-                    Enum type. Allowed values:
+                Enum type. Allowed values:
                     "SPOT" - Heavily discounted, no guaranteed runtime.
                     "STANDARD" - Standard provisioning with user controlled runtime, no discounts.
             * location_hint (str, Optional):
                 An opaque location hint used to place the instance close to other resources. This field is for use by internal tools that use the public API.
 
         private_ipv6_google_access(str, Optional):
             The private IPv6 google access type for the VM. If not specified, use INHERIT_FROM_SUBNETWORK as default.
-                Enum type. Allowed values:
+            Enum type. Allowed values:
                 "ENABLE_BIDIRECTIONAL_ACCESS_TO_GOOGLE" - Bidirectional private IPv6 access to/from Google services. If specified, the subnetwork who is attached to the instance's default network interface will be assigned an internal IPv6 prefix if it doesn't have before.
                 "ENABLE_OUTBOUND_VM_ACCESS_TO_GOOGLE" - Outbound private IPv6 access from VMs in this subnet to Google services. If specified, the subnetwork who is attached to the instance's default network interface will be assigned an internal IPv6 prefix if it doesn't have before.
                 "INHERIT_FROM_SUBNETWORK" - Each network interface inherits PrivateIpv6GoogleAccess from its subnetwork. Defaults to None.
 
         description(str, Optional):
             An optional description of this resource. Provide this property when you create the resource. Defaults to None.
 
@@ -718,15 +718,15 @@
             * boot (bool, Optional):
                 Indicates that this is a boot disk. The virtual machine will use the first partition of the disk for its root filesystem.
             * guest_os_features (List[Dict[str, Any]], Optional):
                 A list of features to enable on the guest operating system. Applicable only for bootable images. Read Enabling guest operating system features to see a list of available options.
 
                 * type (str, Optional):
                     The ID of a supported feature. To add multiple values, use commas to separate values. Set to one or more of the following values: - VIRTIO_SCSI_MULTIQUEUE - WINDOWS - MULTI_IP_SUBNET - UEFI_COMPATIBLE - GVNIC - SEV_CAPABLE - SUSPEND_RESUME_COMPATIBLE - SEV_SNP_CAPABLE For more information, see Enabling guest operating system features.
-                        Enum type. Allowed values:
+                    Enum type. Allowed values:
                         "FEATURE_TYPE_UNSPECIFIED"
                         "GVNIC"
                         "MULTI_IP_SUBNET"
                         "SECURE_BOOT"
                         "SEV_CAPABLE"
                         "UEFI_COMPATIBLE"
                         "VIRTIO_SCSI_MULTIQUEUE"
@@ -746,64 +746,64 @@
                     The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
                 * raw_key (str, Optional):
                     Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
             * force_attach (bool, Optional):
                 [Input Only] Whether to force attach the regional disk even if it's currently attached to another instance. If you try to force attach a zonal disk to an instance, you will receive an error.
             * architecture (str, Optional):
                 [Output Only] The architecture of the attached disk. Valid values are ARM64 or X86_64.
-                    Enum type. Allowed values:
+                Enum type. Allowed values:
                     "ARCHITECTURE_UNSPECIFIED" - Default value indicating Architecture is not set.
                     "ARM64" - Machines with architecture ARM64
                     "X86_64" - Machines with architecture X86_64
             * device_name (str, Optional):
                 Specifies a unique device name of your choice that is reflected into the /dev/disk/by-id/google-* tree of a Linux operating system running within the instance. This name can be used to reference the device for mounting, resizing, and so on, from within the instance. If not specified, the server chooses a default device name to apply to this disk, in the form persistent-disk-x, where x is a number assigned by Google Compute Engine. This field is only applicable for persistent disks.
             * shielded_instance_initial_state (Dict[str, Any], Optional):
                 [Output Only] shielded vm initial state stored on disk.
                 InitialStateConfig: Initial State for shielded instance, these are public keys which are safe to store in public
 
                 * keks (List[Dict[str, Any]], Optional):
                     The Key Exchange Key (KEK).
 
                     * file_type (str, Optional):
                         The file type of source file.
-                            Enum type. Allowed values:
+                        Enum type. Allowed values:
                             "BIN"
                             "UNDEFINED"
                             "X509"
                     * content (str, Optional):
                         The raw content in the secure keys file.
                 * dbs (List[Dict[str, Any]], Optional):
                     The Key Database (db).
 
                     * file_type (str, Optional):
                         The file type of source file.
-                            Enum type. Allowed values:
+                        Enum type. Allowed values:
                             "BIN"
                             "UNDEFINED"
                             "X509"
                     * content (str, Optional):
                         The raw content in the secure keys file.
 
                 * dbxs (List[Dict[str, Any]], Optional):
                     The forbidden key database (dbx).
 
                     * file_type (str, Optional):
                         The file type of source file.
-                            Enum type. Allowed values:
+                        Enum type. Allowed values:
                             "BIN"
                             "UNDEFINED"
                             "X509"
                     * content (str, Optional):
                         The raw content in the secure keys file.
                 * pk (Dict[str, Any], Optional):
                     The Platform Key (PK).
 
                     * file_type (str, Optional):
                         The file type of source file.
-                            Enum type. Allowed values:
+                        Enum type. Allowed values:
                             "BIN"
                             "UNDEFINED"
                             "X509"
                     * content (str, Optional):
                         The raw content in the secure keys file.
             * initialize_params (Dict[str, Any], Optional):
                 [Input Only] Specifies the parameters for a new disk that will be created alongside the new instance. Use initialization parameters to create boot disks or local SSDs attached to the new instance. This property is mutually exclusive with the source property; you can only define one or the other, but not both.
@@ -832,15 +832,15 @@
                         Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
                     * kms_key_name (str, Optional):
                         The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
                     * raw_key (str, Optional):
                         Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
                 * on_update_action (str, Optional):
                     Specifies which action to take on instance update with this disk. Default is to use the existing disk.
-                        Enum type. Allowed values:
+                    Enum type. Allowed values:
                         "RECREATE_DISK" - Always recreate the disk.
                         "RECREATE_DISK_IF_SOURCE_CHANGED" - Recreate the disk if source (image, snapshot) of this disk is different from source of existing disk.
                         "USE_EXISTING_DISK" - Use the existing disk, this is the default behaviour.
                 * source_snapshot_encryption_key (Dict[str, Any], Optional):
                     The customer-supplied encryption key of the source snapshot.
 
                     * kms_key_service_account (str, Optional):
@@ -852,15 +852,15 @@
                     * kms_key_name (str, Optional):
                         The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
                     * raw_key (str, Optional):
                         Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
 
                 * architecture (str, Optional):
                     The architecture of the attached disk. Valid values are arm64 or x86_64.
-                        Enum type. Allowed values:
+                    Enum type. Allowed values:
                         "ARCHITECTURE_UNSPECIFIED" - Default value indicating Architecture is not set.
                         "ARM64" - Machines with architecture ARM64
                         "X86_64" - Machines with architecture X86_64
                 * licenses (List[str], Optional):
                     A list of publicly visible licenses. Reserved for Google's use.
                 * labels (Dict[str, Any], Optional):
                     Labels to apply to this disk. These can be later modified by the disks.setLabels method. This field is only applicable for persistent disks.
@@ -873,40 +873,40 @@
 
             * kind (str, Optional):
                 [Output Only] Type of the resource. Always compute#attachedDisk for attached disks.
             * index (int, Optional):
                 [Output Only] A zero-based index to this disk, where 0 is reserved for the boot disk. If you have many disks attached to an instance, each disk would have a unique index number.
             * interface (str, Optional):
                 Specifies the disk interface to use for attaching this disk, which is either SCSI or NVME. For most machine types, the default is SCSI. Local SSDs can use either NVME or SCSI. In certain configurations, persistent disks can use NVMe. For more information, see About persistent disks.
-                    Enum type. Allowed values:
+                Enum type. Allowed values:
                     "NVME"
                     "SCSI"
             * licenses (List[str], Optional):
                 [Output Only] Any valid publicly visible licenses.
             * mode (str, Optional):
                 The mode in which to attach this disk, either READ_WRITE or READ_ONLY. If not specified, the default is to attach the disk in READ_WRITE mode.
-                    Enum type. Allowed values:
+                Enum type. Allowed values:
                     "READ_ONLY" - Attaches this disk in read-only mode. Multiple virtual machines can use a disk in read-only mode at a time.
                     "READ_WRITE" - *[Default]* Attaches this disk in read-write mode. Only one virtual machine at a time can be attached to a disk in read-write mode.
             * type (str, Optional):
                 Specifies the type of the disk, either SCRATCH or PERSISTENT. If not specified, the default is PERSISTENT.
-                    Enum type. Allowed values:
+                Enum type. Allowed values:
                     "PERSISTENT"
                     "SCRATCH"
 
         hostname(str, Optional):
             Specifies the hostname of the instance. The specified hostname must be RFC1035 compliant. If hostname is not specified, the default hostname is [INSTANCE_NAME].c.[PROJECT_ID].internal when using the global DNS, and [INSTANCE_NAME].[ZONE].c.[PROJECT_ID].internal when using zonal DNS. Defaults to None.
 
         network_performance_config(Dict[str, Any], Optional):
             Defaults to None.
 
             * total_egress_bandwidth_tier (str, Optional):
                 Enum type. Allowed values:
-                "DEFAULT"
-                "TIER_1"
+                    "DEFAULT"
+                    "TIER_1"
 
         params(Dict[str, Any], Optional):
             Input only. [Input Only] Additional params passed with the request, but not persisted as part of resource payload.
             InstanceParams: Additional instance params. Defaults to None.
 
             * resource_manager_tags (Dict[str, Any], Optional):
                 Resource manager tags to be bound to the instance. Tag keys and values have the same definition as resource manager tags. Keys must be in the format `tagKeys/{tag_key_id}`, and values are in the format `tagValues/456`. The field is ignored (both PUT & PATCH) when empty.
@@ -950,15 +950,15 @@
 
             * key (str, Optional):
                 Corresponds to the label key of a reservation resource. To target a SPECIFIC_RESERVATION by name, specify googleapis.com/reservation-name as the key and specify the name of your reservation as its value.
             * values (List[str], Optional):
                 Corresponds to the label values of a reservation resource. This can be either a name to a reservation in the same project or "projects/different-project/reservations/some-reservation-name" to target a shared reservation in the same zone but in a different project.
             * consume_reservation_type (str, Optional):
                 Specifies the type of reservation from which this instance can consume resources: ANY_RESERVATION (default), SPECIFIC_RESERVATION, or NO_RESERVATION. See Consuming reserved instances for examples.
-                    Enum type. Allowed values:
+                Enum type. Allowed values:
                     "ANY_RESERVATION" - Consume any allocation available.
                     "NO_RESERVATION" - Do not consume from any allocated capacity.
                     "SPECIFIC_RESERVATION" - Must consume from a specific reservation. Must specify key value fields for specifying the reservations.
                     "UNSPECIFIED"
 
         min_cpu_platform(str, Optional):
             Specifies a minimum CPU platform for the VM instance. Applicable values are the friendly names of CPU platforms, such as minCpuPlatform: "Intel Haswell" or minCpuPlatform: "Intel Sandy Bridge". Defaults to None.
@@ -975,15 +975,15 @@
             - https://www.googleapis.com/compute/v1/projects/project/global/instanceTemplates/instanceTemplate
             - projects/project/global/instanceTemplates/instanceTemplate
             - global/instanceTemplates/instanceTemplate
 
             Defaults to None.
 
         source_machine_image(str, Optional):
-            Specifies the machine image to use to create the instance. This field is optional. It can be a full or partial URL. Defaults to None. For example, the following are all valid URLs to a machine image:
+            Specifies the machine image to use to create the instance. This field is optional. It can be a full or partial URL. Defaults to None. For example, the following are all valid URLs to a machine image. Defaults to None.:
 
             - https://www.googleapis.com/compute/v1/projects/project/global/global/machineImages/machineImage
             - projects/project/global/global/machineImages/machineImage
             - global/machineImages/machineImage
 
         request_id(str, Optional):
             An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000). Defaults to None.
```

### Comparing `idem_gcp-1.1.0/idem_gcp/states/gcp/compute/instance_group.py` & `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/snapshot.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,346 +1,352 @@
-"""State module for managing InstanceGroups."""
-
+"""State module for managing Snapshots."""
 __contracts__ = ["resource"]
 
+from dataclasses import make_dataclass, field
+from typing import Dict, Any, List
+
 from dataclasses import field
 from dataclasses import make_dataclass
 from typing import Any
 from typing import Dict
 from typing import List
 
-from idem_gcp.tool.gcp.state_operation_utils import StateOperations
-from idem_gcp.tool.gcp.utils import zonal_absent
+from idem_gcp.tool.gcp.utils import global_absent
 
 # prevent commit hook from removing the import
-absent = zonal_absent
+absent = global_absent
 
 __contracts__ = ["resource"]
 
 
 async def present(
     hub,
     ctx,
-    name: str = None,
-    zone: str = None,
+    name: str,
     project: str = None,
+    resource_id: str = None,
+    source_disk: str = None,
+    storage_locations: List[str] = None,
+    location_hint: str = None,
+    label_fingerprint: str = None,
     description: str = None,
-    fingerprint: str = None,
-    subnetwork: str = None,
-    network: str = None,
-    named_ports: List[
-        make_dataclass(
-            "NamedPort",
-            [("name", str, field(default=None)), ("port", int, field(default=None))],
-        )
-    ] = None,
+    labels: Dict[str, Any] = None,
+    source_disk_encryption_key: make_dataclass(
+        "CustomerEncryptionKey",
+        [
+            ("kms_key_service_account", str, field(default=None)),
+            ("rsa_encrypted_key", str, field(default=None)),
+            ("kms_key_name", str, field(default=None)),
+            ("raw_key", str, field(default=None)),
+        ],
+    ) = None,
+    chain_name: str = None,
+    snapshot_type: str = None,
+    snapshot_encryption_key: make_dataclass(
+        "CustomerEncryptionKey",
+        [
+            ("kms_key_service_account", str, field(default=None)),
+            ("rsa_encrypted_key", str, field(default=None)),
+            ("kms_key_name", str, field(default=None)),
+            ("raw_key", str, field(default=None)),
+        ],
+    ) = None,
     request_id: str = None,
-    resource_id: str = None,
 ) -> Dict[str, Any]:
-    r"""Create or update an instance group.
+    r"""Creates a snapshot in the specified project using the data included in the request.
 
-    Creates an instance group in the specified project using the parameters that are included in the request.
+    For regular snapshot creation, consider using this method instead of disks.createSnapshot, as this method supports more features, such as creating snapshots in a project different from the source disk project.
 
     Args:
-        name(str):
-            An Idem name of the resource.
+        storage_locations(List[str], Optional):
+            Cloud Storage bucket storage location of the snapshot (regional or multi-regional). Defaults to None.
+
+        location_hint(str, Optional):
+            An opaque location hint used to place the snapshot close to other resources. This field is for use by internal tools that use the public API. Defaults to None.
+
+        label_fingerprint(str, Optional):
+            A fingerprint for the labels being applied to this snapshot, which is essentially a hash of the labels set used for optimistic locking. The fingerprint is initially generated by Compute Engine and changes after every request to modify or update labels. You must always provide an up-to-date fingerprint hash in order to update or change labels, otherwise the request will fail with error 412 conditionNotMet. To see the latest fingerprint, make a get() request to retrieve a snapshot. Defaults to None.
 
         description(str, Optional):
             An optional description of this resource. Provide this property when you create the resource. Defaults to None.
 
-        zone(str):
-            The name of the zone where the instance group is located.
-
-        fingerprint(str, Optional):
-            The fingerprint of the named ports. The system uses this fingerprint to detect conflicts when multiple users change the named ports concurrently. Defaults to None.
+        labels(Dict[str, Any], Optional):
+            Labels to apply to this snapshot. These can be later modified by the setLabels method. Label values may be empty. Defaults to None.
 
-        network(str, Optional):
-            The URL of the network to which all instances in the instance group belong. If your instance has multiple network interfaces, then the network and subnetwork fields only refer to the network and subnet used by your primary interface (nic0). Defaults to None.
+        source_disk_encryption_key(Dict[str, Any], Optional):
+            The customer-supplied encryption key of the source disk. Required if the source disk is protected by a customer-supplied encryption key. Defaults to None.
+            * kms_key_service_account(str, Optional):
+                The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/"
+            * sha256(str, Optional):
+                [Output only] The RFC 4648 base64 encoded SHA-256 hash of the customer-supplied encryption key that protects this resource.
+            * rsa_encrypted_key(str, Optional):
+                Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
+            * kms_key_name(str, Optional):
+                The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
+            * raw_key(str, Optional):
+                Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
+
+        source_disk(str, Optional):
+            The source disk used to create this snapshot. Defaults to None.
+
+        chain_name(str, Optional):
+            Creates the new snapshot in the snapshot chain labeled with the specified name. The chain name must be 1-63 characters long and comply with RFC1035. This is an uncommon option only for advanced service owners who needs to create separate snapshot chains, for example, for chargeback tracking. When you describe your snapshot resource, this field is visible only if it has a non-empty value. Defaults to None.
+
+        snapshot_type(str, Optional):
+            Indicates the type of the snapshot.
+            Enum type. Allowed values:
+                "ARCHIVE"
+                "STANDARD". Defaults to None.
+
+        snapshot_encryption_key(Dict[str, Any], Optional):
+            Encrypts the snapshot using a customer-supplied encryption key. After you encrypt a snapshot using a customer-supplied key, you must provide the same key if you use the snapshot later. For example, you must provide the encryption key when you create a disk from the encrypted snapshot in a future request. Customer-supplied encryption keys do not protect access to metadata of the snapshot. If you do not provide an encryption key when creating the snapshot, then the snapshot will be encrypted using an automatically generated key and you do not need to provide a key to use the snapshot later. Defaults to None.
+            * kms_key_service_account(str, Optional):
+                The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/"
+            * sha256 (str, Optional):
+                [Output only] The RFC 4648 base64 encoded SHA-256 hash of the customer-supplied encryption key that protects this resource.
+            * rsa_encrypted_key(str, Optional):
+                Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
+            * kms_key_name(str, Optional):
+                The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
+            * raw_key(str, Optional):
+                Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
 
-        subnetwork(str, Optional):
-            The URL of the subnetwork to which all instances in the instance group belong. If your instance has multiple network interfaces, then the network and subnetwork fields only refer to the network and subnet used by your primary interface (nic0). Defaults to None.
-
-        named_ports(List[Dict[str, Any]], Optional):
-            Assigns a name to a port number. For example: {name: "http", port: 80} This allows the system to reference ports by the assigned name instead of a port number. Named ports can also contain multiple ports. For example: [{name: "app1", port: 8080}, {name: "app1", port: 8081}, {name: "app2", port: 8082}] Named ports apply to all instances in this instance group. . Defaults to None.
-                * name (str, Optional): The name for this named port. The name must be 1-63 characters long, and comply with RFC1035.
-                * port (int, Optional): The port number, which can be a value between 1 and 65535.
+        request_id(str, Optional):
+            An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000). Defaults to None.
 
         project(str):
             Project ID for this request.
 
-        request_id(str, Optional):
-            An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000). Defaults to None.
+        name(str):
+            Name of the Snapshot resource to return.
 
         resource_id(str, Optional):
             An identifier of the resource in the provider. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
 
             resource_is_present:
-              gcp.compute.instance_groups.present:
+              gcp.compute.snapshot.present:
                 - name: value
-                - zone: value
                 - project: value
-                - instance_group: value
+                - snapshot: value
     """
     result = {
         "result": True,
         "old_state": None,
         "new_state": None,
         "name": name,
         "comment": [],
     }
 
     project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     if ctx.get("wrapper_result"):
         result = ctx.get("wrapper_result")
 
+    # to be autogenerated by pop-create based on insert/update props in properties.yaml
     resource_body = {
-        "description": description,
-        "zone": zone,
         "name": name,
-        "named_ports": named_ports,
-        "network": network,
-        "subnetwork": subnetwork,
+        "storage_locations": storage_locations,
+        "location_hint": location_hint,
+        "label_fingerprint": label_fingerprint,
+        "description": description,
+        "labels": labels,
+        "source_disk_encryption_key": source_disk_encryption_key,
+        "source_disk": source_disk,
+        "chain_name": chain_name,
+        "snapshot_type": snapshot_type,
+        "snapshot_encryption_key": snapshot_encryption_key,
     }
 
     resource_body = {k: v for (k, v) in resource_body.items() if v is not None}
     operation = None
-    if result["old_state"]:
-        resource_id = result["old_state"].get("resource_id", None)
-        resource_body["resource_id"] = resource_id
 
-        # The fingerprint is required upon an update operation but in the time of creation the
-        # resource still do not have fingerprint so, we cannot make it a required param for present method.
-        resource_body["fingerprint"] = fingerprint or result["old_state"].get(
-            "fingerprint"
-        )
-
-        # A dictionary of additional operations to perform on the object identified by the key
-        # the values are tuples with the first element - the method to call, the second element - arguments,
-        # third - the property is required in the end result
-        patch_operations_dict = {
-            "named_ports": (
-                hub.tool.gcp.compute.instance_group.update_named_ports,
-                (ctx, result["old_state"], named_ports),
-                True,
-            ),
-        }
-
-        state_operations = StateOperations(
-            hub, "compute.instance_group", patch_operations_dict, result, resource_body
-        )
+    if result["old_state"]:
+        resource_body["label_fingerprint"] = label_fingerprint or result[
+            "old_state"
+        ].get("label_fingerprint")
 
         changes = hub.tool.gcp.utils.compare_states(
             result["old_state"],
-            {
-                **resource_body,
-            },
-            "compute.instance_group",
-            additional_exclude_paths=list(patch_operations_dict.keys()),
+            {"resource_id": resource_id, **resource_body},
+            "compute.snapshot",
         )
 
-        if changes:
-            changed_non_updatable_properties = (
-                hub.tool.gcp.resource_prop_utils.get_changed_non_updatable_properties(
-                    "compute.instance_group", changes
+        # This check is necessary because "changes" does not detect label removal
+        are_labels_changed = (
+            labels is not None
+            and not (labels == {} and result["old_state"].get("labels") is None)
+            and result["old_state"].get("labels") != labels
+        )
+
+        if not changes and not are_labels_changed:
+            result["comment"].append(
+                hub.tool.gcp.comment_utils.up_to_date_comment(
+                    "gcp.compute.snapshot", name
                 )
             )
-            if changed_non_updatable_properties:
-                result["result"] = False
-                result["comment"].append(
-                    hub.tool.gcp.comment_utils.non_updatable_properties_comment(
-                        "gcp.compute.instance_group",
-                        name,
-                        changed_non_updatable_properties,
-                    )
-                )
-                result["new_state"] = result["old_state"]
-                return result
+            result["new_state"] = result["old_state"]
+            return result
+
+        changed_non_updatable_properties = (
+            hub.tool.gcp.resource_prop_utils.get_changed_non_updatable_properties(
+                "compute.snapshot", changes
+            )
+        )
 
-        if not changes and not any(state_operations.changed_properties_dict.values()):
+        if changed_non_updatable_properties:
+            result["result"] = False
             result["comment"].append(
-                hub.tool.gcp.comment_utils.up_to_date_comment(
-                    "gcp.compute.instance_group", name
+                hub.tool.gcp.comment_utils.non_updatable_properties_comment(
+                    "gcp.compute.snapshot",
+                    name,
+                    changed_non_updatable_properties,
                 )
             )
             result["new_state"] = result["old_state"]
             return result
 
-        if ctx["test"]:
+        if ctx.get("test", False):
             result["comment"].append(
                 hub.tool.gcp.comment_utils.would_update_comment(
-                    "gcp.compute.instance_group", name
+                    "gcp.compute.snapshot", name
                 )
             )
             result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
                 resource_body
             )
+            result["new_state"]["resource_id"] = resource_id
             return result
 
-        state_operations_ret = await state_operations.run_operations()
+        set_labels_body = {
+            "labels": labels,
+        }
+        if label_fingerprint:
+            set_labels_body.update(
+                {
+                    "label_fingerprint": label_fingerprint,
+                }
+            )
+        elif result["old_state"].get("label_fingerprint"):
+            set_labels_body.update(
+                {
+                    "label_fingerprint": result["old_state"].get("label_fingerprint"),
+                }
+            )
+
+        # the setLabels() method accepts "resource" as the name of the snapshot, so
+        # the resource_id is split into its properties ("project" and "snapshot") here to map "resource" to "snapshot
+        resource_id_props = (
+            hub.tool.gcp.resource_prop_utils.get_elements_from_resource_id(
+                "compute.snapshot", resource_id
+            )
+        )
+        update_ret = await hub.exec.gcp_api.client.compute.snapshot.setLabels(
+            ctx,
+            project=resource_id_props.get("project"),
+            resource=resource_id_props.get("snapshot"),
+            body=set_labels_body,
+        )
 
-        if not state_operations_ret["result"] or not state_operations_ret.get(
-            "new_state"
-        ):
+        if not update_ret["result"] or not update_ret["ret"]:
             result["result"] = False
-            result["comment"] += state_operations_ret["comment"]
+            result["comment"] += update_ret["comment"]
             return result
 
-        result["new_state"] = state_operations_ret["new_state"]
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.update_comment(
-                "gcp.compute.instance_group", name
-            )
-        )
-        return result
+        if hub.tool.gcp.operation_utils.is_operation(update_ret["ret"]):
+            operation = update_ret["ret"]
 
     else:
-        # Create for test
-        if ctx.get("test", False):
+        if ctx["test"]:
             result["comment"].append(
                 hub.tool.gcp.comment_utils.would_create_comment(
-                    "gcp.compute.instance_group", name
+                    "gcp.compute.snapshot", name
                 )
             )
             result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
                 resource_body
             )
-            result["new_state"][
-                "resource_id"
-            ] = hub.tool.gcp.resource_prop_utils.construct_resource_id(
-                "compute.instance_group", {**locals(), "instanceGroup": name}
-            )
+            result["new_state"]["resource_id"] = resource_id
             return result
 
         # Create
-        create_ret = await hub.exec.gcp_api.client.compute.instance_group.insert(
+        create_ret = await hub.exec.gcp_api.client.compute.snapshot.insert(
             ctx,
             name=name,
             project=project,
-            zone=zone,
             request_id=request_id,
             body=resource_body,
         )
-        if not create_ret["result"] or not create_ret["ret"]:
+        if not create_ret["result"]:
             result["result"] = False
             if create_ret["comment"] and next(
                 (
                     comment
                     for comment in create_ret["comment"]
                     if "alreadyExists" in comment
                 ),
                 None,
             ):
                 result["comment"].append(
                     hub.tool.gcp.comment_utils.already_exists_comment(
-                        "gcp.compute.instance_group", name
+                        "gcp.compute.snapshot", name
                     )
                 )
+                return result
             else:
                 result["comment"] += create_ret["comment"]
-            return result
 
-        if hub.tool.gcp.operation_utils.is_operation(create_ret["ret"]):
-            operation = create_ret["ret"]
+        if create_ret["ret"]:
+            if hub.tool.gcp.operation_utils.is_operation(create_ret["ret"]):
+                operation = create_ret["ret"]
 
     if operation:
         operation_id = hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-            operation.get("selfLink"), "compute.zone_operation"
+            operation.get("selfLink"), "compute.global_operation"
         )
         result["rerun_data"] = {
             "operation_id": operation_id,
             "old_state": result["old_state"],
         }
 
     return result
 
 
-async def absent(
-    hub,
-    ctx,
-    name: str = None,
-    project: str = None,
-    zone: str = None,
-    request_id: str = None,
-    resource_id: str = None,
-) -> Dict[str, Any]:
-    r"""Deletes the specified instance group.
-
-    The instances in the group are not deleted. Note that instance group must not belong to a backend service. Read Deleting an instance group for more information.
-
-    Args:
-        name(str):
-            An Idem name of the resource.
-
-        project(str):
-            Project ID for this request.
-
-        request_id(str, Optional):
-            An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000). Defaults to None.
-
-        zone(str):
-            The name of the zone where the instance group is located.
-
-        resource_id(str, Optional):
-            An identifier of the resource in the provider. Defaults to None.
-
-    Returns:
-        Dict[str, Any]
-
-
-    Examples:
-        .. code-block:: sls
-
-            resource_is_absent:
-              gcp.compute.instance_groups.absent:
-                - name: value
-                - project: value
-                - instance_group: value
-                - zone: value
-    """
-    # the method is handled via the recursive_contracts->call_absent
-    raise NotImplementedError
-
-
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
     r"""Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
-    Retrieves the list of zonal instance group resources contained within the specified zone. For managed instance groups, use the instanceGroupManagers or regionInstanceGroupManagers methods instead.
+    Retrieves the list of Snapshot resources contained within the specified project.
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: bash
 
-            $ idem describe gcp.compute.instance_groups
+            $ idem describe gcp.compute.snapshot
     """
     result = {}
 
-    describe_ret = await hub.exec.gcp.compute.instance_group.list(
+    describe_ret = await hub.exec.gcp.compute.snapshot.list(
         ctx, project=ctx.acct.project_id
     )
 
     if not describe_ret["result"]:
-        hub.log.debug(
-            f"Could not describe gcp.compute.instance_group {describe_ret['comment']}"
-        )
+        hub.log.debug(f"Could not describe snapshots {describe_ret['comment']}")
         return {}
 
     for resource in describe_ret["ret"]:
         resource_id = resource.get("resource_id")
-
         result[resource_id] = {
-            "gcp.compute.instance_group.present": [
+            "gcp.compute.snapshot.present": [
                 {parameter_key: parameter_value}
                 for parameter_key, parameter_value in resource.items()
             ]
         }
 
     return result
```

### Comparing `idem_gcp-1.1.0/idem_gcp/states/gcp/compute/machine_image.py` & `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/machine_image.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,42 +99,54 @@
                 - https://www.googleapis.com/compute/v1/projects/project/zones/zone/disks/disk
                 - projects/project/zones/zone/disks/disk
                 - zones/zone/disks/disk
 
             * disk_encryption_key(Dict[str, Any], Optional):
                 The customer-supplied encryption key of the source disk. Required if the source disk is protected by a customer-supplied encryption key.
 
-                * kms_key_service_account(str, Optional): The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/"
-                * rsa_encrypted_key(str, Optional): Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
-                * kms_key_name(str, Optional): The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
-                * raw_key(str, Optional): Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
+                * kms_key_service_account(str, Optional):
+                    The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/"
+                * rsa_encrypted_key(str, Optional):
+                    Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
+                * kms_key_name(str, Optional):
+                    The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
+                * raw_key(str, Optional):
+                    Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
 
         description(str, Optional):
             An optional description of this resource. Provide this property when you create the resource. Defaults to None.
 
         saved_disks(list[Dict[str, Any]], Optional):
             An array of Machine Image specific properties for disks attached to the source instance. Defaults to None.
 
-            * properties (Dict[str, Dict[str, Any]], Optional): An instance-attached disk resource.
-                * kind (str, Optional): [Output Only] Type of the resource. Always compute#savedDisk for attached disks.
-                * storageBytesStatus (str, Optional): [Output Only] An indicator whether storageBytes is in a stable state or it is being adjusted as a result of shared storage reallocation. This status can either be UPDATING, meaning the size of the snapshot is being updated, or UP_TO_DATE, meaning the size of the snapshot is up-to-date.
-                * architecture (str, Optional): [Output Only] The architecture of the attached disk.
-                * storageBytes (str, Optional): [Output Only] Size of the individual disk snapshot used by this machine image.
-                * sourceDisk (str, Optional): Specifies a URL of the disk attached to the source instance.
+            * kind(str, Optional):
+                [Output Only] Type of the resource. Always compute#savedDisk for attached disks.
+            * storage_bytes_status (str, Optional):
+                [Output Only] An indicator whether storageBytes is in a stable state or it is being adjusted as a result of shared storage reallocation. This status can either be UPDATING, meaning the size of the snapshot is being updated, or UP_TO_DATE, meaning the size of the snapshot is up-to-date.
+            * architecture(str, Optional):
+                [Output Only] The architecture of the attached disk.
+            * storage_bytes(str, Optional):
+                [Output Only] Size of the individual disk snapshot used by this machine image.
+            * source_disk(str, Optional):
+                Specifies a URL of the disk attached to the source instance.
 
         guest_flush(bool, Optional):
             [Input Only] Whether to attempt an application consistent machine image by informing the OS to prepare for the snapshot process. Defaults to None.
 
         machine_image_encryption_key(Dict[str, Any], Optional):
             Encrypts the machine image using a customer-supplied encryption key. After you encrypt a machine image using a customer-supplied key, you must provide the same key if you use the machine image later. For example, you must provide the encryption key when you create an instance from the encrypted machine image in a future request. Customer-supplied encryption keys do not protect access to metadata of the machine image. If you do not provide an encryption key when creating the machine image, then the machine image will be encrypted using an automatically generated key and you do not need to provide a key to use the machine image later. Defaults to None.
 
-            * kms_key_service_account(str, Optional): The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/"
-            * rsa_encrypted_key(str, Optional): Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
-            * kms_key_name(str, Optional): The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
-            * raw_key(str, Optional): Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
+            * kms_key_service_account(str, Optional):
+                The service account being used for the encryption request for the given KMS key. If absent, the Compute Engine default service account is used. For example: "kmsKeyServiceAccount": "name@project_id.iam.gserviceaccount.com/"
+            * rsa_encrypted_key(str, Optional):
+                Specifies an RFC 4648 base64 encoded, RSA-wrapped 2048-bit customer-supplied encryption key to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rsaEncryptedKey": "ieCx/NcW06PcT7Ep1X6LUTc/hLvUDYyzSZPPVCVPTVEohpeHASqC8uw5TzyO9U+Fka9JFH z0mBibXUInrC/jEk014kCK/NPjYgEMOyssZ4ZINPKxlUh2zn1bV+MCaTICrdmuSBTWlUUiFoD D6PYznLwh8ZNdaheCeZ8ewEXgFQ8V+sDroLaN3Xs3MDTXQEMMoNUXMCZEIpg9Vtp9x2oe==" The key must meet the following requirements before you can provide it to Compute Engine: 1. The key is wrapped using a RSA public key certificate provided by Google. 2. After being wrapped, the key must be encoded in RFC 4648 base64 encoding. Gets the RSA public key certificate provided by Google at: https://cloud-certs.storage.googleapis.com/google-cloud-csek-ingress.pem
+            * kms_key_name(str, Optional):
+                The name of the encryption key that is stored in Google Cloud KMS. For example: "kmsKeyName": "projects/kms_project_id/locations/region/keyRings/ key_region/cryptoKeys/key
+            * raw_key(str, Optional):
+                Specifies a 256-bit customer-supplied encryption key, encoded in RFC 4648 base64 to either encrypt or decrypt this resource. You can provide either the rawKey or the rsaEncryptedKey. For example: "rawKey": "SGVsbG8gZnJvbSBHb29nbGUgQ2xvdWQgUGxhdGZvcm0="
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
```

### Comparing `idem_gcp-1.1.0/idem_gcp/states/gcp/compute/network.py` & `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     resource_id: str = None,
     request_id: str = None,
     project: str = None,
     auto_create_subnetworks: bool = None,
     description: str = None,
     enable_ula_internal_ipv6: bool = None,
     internal_ipv6_range: str = None,
-    i_pv4_range: str = None,
     mtu: int = None,
     network_firewall_policy_enforcement_order: str = None,
     routing_config: make_dataclass(
         "NetworkRoutingConfig",
         [
             ("routing_mode", str, field(default=None)),
         ],
@@ -69,14 +68,21 @@
 
         project(str, Optional):
             Project ID for this request.
 
         routing_config(NetworkRoutingConfig, Optional):
             The network-level routing configuration for this network. Used by Cloud Router to determine what type of network-wide routing behavior to enforce. Defaults to None.
 
+            * routing_mode(str, Optional):
+                The network-wide routing mode to use. If set to REGIONAL, this network's Cloud Routers will only advertise routes with subnets of this network in the same
+                region as the router. If set to GLOBAL, this network's Cloud Routers will advertise routes with all subnets of this network, across regions.
+                Enum type. Allowed values:
+                    "GLOBAL"
+                    "REGIONAL"
+
         description(str, Optional):
             An optional description of this resource. Provide this field when you create the resource. Defaults to None.
 
         auto_create_subnetworks(bool, Optional):
             Must be set to create a VPC network. If not set, a legacy network is created. When set to true, the VPC network is created in auto mode. When set to false, the VPC network is created in custom mode. An auto mode VPC network starts with one subnet per region. Each subnet has a predetermined range as described in Auto mode VPC network IP ranges. For custom mode VPC networks, you can add subnets using the subnetworks insert method. Defaults to None.
 
         internal_ipv6_range(str, Optional):
@@ -84,17 +90,14 @@
 
         network_firewall_policy_enforcement_order(str, Optional):
             The network firewall policy enforcement order. Can be either AFTER_CLASSIC_FIREWALL or BEFORE_CLASSIC_FIREWALL. Defaults to AFTER_CLASSIC_FIREWALL if the field is not specified. Defaults to None.
 
         enable_ula_internal_ipv6(bool, Optional):
             Enable ULA internal ipv6 on this network. Enabling this feature will assign a /48 from google defined ULA prefix fd20::/20. . Defaults to None.
 
-        i_pv4_range(str, Optional):
-            Deprecated in favor of subnet mode networks. The range of internal addresses that are legal on this network. This range is a CIDR specification, for example: 192.168.0.0/16. Provided by the client when the network is created. Defaults to None.
-
         mtu(int, Optional):
             Maximum Transmission Unit in bytes. The minimum value for this field is 1300 and the maximum value is 8896. The suggested value is 1500, which is the default MTU used on the Internet, or 8896 if you want to use Jumbo frames. If unspecified, the value defaults to 1460. Defaults to None.
 
         resource_id(str, Optional):
             An identifier of the resource in the provider. Defaults to None.
 
         peerings(List[Dict[str, Any]], Optional):
@@ -106,15 +109,15 @@
                 This field will be deprecated soon. Use the exchange_subnet_routes field instead. Indicates whether full mesh connectivity is created and managed automatically between peered networks. Currently this field should always be true since Google Compute Engine will automatically create and manage subnetwork routes between two networks when peering state is ACTIVE.
             * network(str, Optional):
                 The URL of the peer network. It can be either full URL or partial URL. The peer network may belong to a different project. If the partial URL does not contain project, it is assumed that the peer network is in the same project as the current network.
             * name(str, Optional):
                 Name of this peering. Provided by the client when the peering is created. The name must comply with RFC1035. Specifically, the name must be 1-63 characters long and match regular expression `[a-z]([-a-z0-9]*[a-z0-9])?`. The first character must be a lowercase letter, and all the following characters must be a dash, lowercase letter, or digit, except the last character, which cannot be a dash.
             * state(str, Optional):
                 [Output Only] State for the peering, either `ACTIVE` or `INACTIVE`. The peering is `ACTIVE` when there's a matching configuration in the peer network.
-                    Enum type. Allowed values:
+                Enum type. Allowed values:
                     "ACTIVE" - Matching configuration exists on the peer.
                     "INACTIVE" - There is no matching configuration on the peer, including the case when peer does not exist.
             * peer_mtu(int, Optional):
                 Maximum Transmission Unit in bytes.
             * import_subnet_routes_with_public_ip(bool, Optional):
                 Whether subnet routes with public IP range are imported. The default value is false. IPv4 special-use ranges are always imported from peers and are not controlled by this field.
             * import_custom_routes(bool, Optional):
@@ -123,15 +126,15 @@
                 [Output Only] Details about the current state of the peering.
             * export_subnet_routes_with_public_ip(bool, Optional):
                 Whether subnet routes with public IP range are exported. The default value is true, all subnet routes are exported. IPv4 special-use ranges are always exported to peers and are not controlled by this field.
             * exchange_subnet_routes(bool, Optional):
                 Indicates whether full mesh connectivity is created and managed automatically between peered networks. Currently this field should always be true since Google Compute Engine will automatically create and manage subnetwork routes between two networks when peering state is ACTIVE.
             * stack_type(str, Optional):
                 Which IP version(s) of traffic and routes are allowed to be imported or exported between peer networks. The default value is IPV4_ONLY.
-                    Enum type. Allowed values:
+                Enum type. Allowed values:
                     "IPV4_IPV6" - This Peering will allow IPv4 traffic and routes to be exchanged. Additionally if the matching peering is IPV4_IPV6, IPv6 traffic and routes will be exchanged as well.
                     "IPV4_ONLY" - This Peering will only allow IPv4 traffic and routes to be exchanged, even if the matching peering is IPV4_IPV6.
 
         id(str, Optional): The unique identifier for the resource. This identifier is defined by the server. Read-only property
 
     Returns:
         Dict[str, Any]
@@ -253,15 +256,14 @@
 
     request_body = {
         "name": name,
         "description": description,
         "auto_create_subnetworks": auto_create_subnetworks,
         "enable_ula_internal_ipv6": enable_ula_internal_ipv6,
         "internal_ipv6_range": internal_ipv6_range,
-        "i_pv4_range": i_pv4_range,
         "mtu": mtu,
         "network_firewall_policy_enforcement_order": network_firewall_policy_enforcement_order,
         "routing_config": routing_config,
         "peerings": peerings,
         "id_": id_,
     }
```

### Comparing `idem_gcp-1.1.0/idem_gcp/states/gcp/compute/node_template.py` & `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/node_template.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             ],
         )
     ] = None,
     cpu_overcommit_type: str = None,
     server_binding: make_dataclass(
         "ServerBinding",
         [
-            ("type", str, field(default=None)),
+            ("type_", (str, "alias=type"), field(default=None)),
         ],
     ) = None,
     node_affinity_labels: Dict = None,
     node_type_flexibility: make_dataclass(
         "NodeTemplateNodeTypeFlexibility",
         [
             ("memory", str, field(default=None)),
@@ -48,16 +48,16 @@
             ("cpus", str, field(default=None)),
         ],
     ) = None,
     accelerators: List[
         make_dataclass(
             "AcceleratorConfig",
             [
-                ("acceleratorType", str, field(default=None)),
-                ("acceleratorCount", int, field(default=0)),
+                ("accelerator_type", str, field(default=None)),
+                ("accelerator_count", int, field(default=0)),
             ],
         )
     ] = None,
     node_type: str = None,
 ) -> Dict[str, Any]:
     r"""Creates a network in the specified project using the data included in the request.
 
@@ -76,29 +76,54 @@
 
         description(str, Optional):
             An optional description of this resource. Provide this field when you create the resource. Defaults to None.
 
         disks(List[LocalDisk], Optional):
             Local disk configurations.
 
+            * disk_count(int, Optional):
+                Specifies the number of such disks.
+            * disk_type(int, Optional):
+                Specifies the size of the disk in base-2 GB.
+            * disk_size_gb(str, Optional):
+                Specifies the desired di…k type and not its URL.
+
         cpu_overcommit_type(str, Optional):
             CPU overcommit.
 
         server_binding(ServerBinding, Optional):
             Sets the binding properties for the physical server. Valid values include: - *[Default]* RESTART_NODE_ON_ANY_SERVER: Restarts VMs on any available physical server - RESTART_NODE_ON_MINIMAL_SERVER: Restarts VMs on the same physical server whenever possible See Sole-tenant node options for more information.
 
-        node_affinity_labels({}, Optional):
+            * type(str, Optional):
+                Enum type. Allowed values:
+                    "RESTART_NODE_ON_ANY_SERVER"
+                    "RESTART_NODE_ON_MINIMAL_SERVERS"
+                    "SERVER_BINDING_TYPE_UNSPECIFIED"
+
+        node_affinity_labels(Dict[str, Any], Optional):
             Labels to use for node affinity, which will be used in instance scheduling.
 
         node_type_flexibility(NodeTemplateNodeTypeFlexibility, Optional):
-            The flexible properties of the desired node type. Node groups that use this node template will create nodes of a type that matches these properties. This field is mutually exclusive with the node_type property; you can only define one or the other, but not both.
+            Do not use. Instead, use the nodeType property.
+
+            * memory(str, Optional):
+                No description
+            * local_ssd(str, Optional):
+                No description
+            * cpus(str, Optional):
+                No description
 
         accelerators(List[AcceleratorConfig], Optional):
             A specification of the type and number of accelerator cards attached to the instance.
 
+            * accelerator_type(int, Optional):
+                The number of the guest …posed to this instance.
+            * accelerator_count(str, Optional):
+                Full or partial URL of t…t of accelerator types.
+
         node_type(str, Optional):
             The node type to use for nodes group that are created from this template.
 
         resource_id(str, Optional):
             An identifier of the resource in the provider. Defaults to None.
 
     Returns:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `idem_gcp-1.1.0/idem_gcp/states/gcp/compute/resource_policy.py` & `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/resource_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
                         ("max_retention_days", int, field(default=0)),
                         ("on_source_disk_delete", str, field(default=None)),
                     ],
                 ),
                 field(default=None),
             ),
             (
-                "snapshotProperties",
+                "snapshot_properties",
                 make_dataclass(
                     "ResourcePolicySnapshotSchedulePolicySnapshotProperties",
                     [
                         ("guest_flush", bool, field(default=False)),
                         ("chain_name", str, field(default=None)),
                         ("storage_locations", List[str], field(default=None)),
                         ("labels", Dict[str, str], field(default=None)),
```

### Comparing `idem_gcp-1.1.0/idem_gcp/states/gcp/compute/subnetwork.py` & `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/subnetwork.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,84 +84,86 @@
             An optional description of this resource. Provide this property when you create the resource. This field can be set only at resource creation time. Defaults to None.
 
         network(str, Optional):
             The URL of the network to which this subnetwork belongs, provided by the client when initially creating the subnetwork. This field can be set only at resource creation time. Defaults to None.
 
         stack_type(str, Optional):
             The stack type for the subnet. If set to IPV4_ONLY, new VMs in the subnet are assigned IPv4 addresses only. If set to IPV4_IPV6, new VMs in the subnet can be assigned both IPv4 and IPv6 addresses. If not specified, IPV4_ONLY is used. This field can be both set at resource creation time and updated using patch.
-                Enum type. Allowed values:
+            Enum type. Allowed values:
                 "IPV4_IPV6" - New VMs in this subnet can have both IPv4 and IPv6 addresses.
                 "IPV4_ONLY" - New VMs in this subnet will only be assigned IPv4 addresses. Defaults to None.
 
         log_config(Dict[str, Any], Optional):
             This field denotes the VPC flow logging options for this subnetwork. If logging is enabled, logs are exported to Cloud Logging.
             SubnetworkLogConfig: The available logging options for this subnetwork. Defaults to None.
 
-            * aggregation_interval (str, Optional):
+            * aggregation_interval(str, Optional):
                 Can only be specified if VPC flow logging for this subnetwork is enabled. Toggles the aggregation interval for collecting flow logs. Increasing the interval time will reduce the amount of generated flow logs for long lasting connections. Default is an interval of 5 seconds per connection.
-                    Enum type. Allowed values:
+                Enum type. Allowed values:
                     "INTERVAL_10_MIN"
                     "INTERVAL_15_MIN"
                     "INTERVAL_1_MIN"
                     "INTERVAL_30_SEC"
                     "INTERVAL_5_MIN"
                     "INTERVAL_5_SEC"
 
-            * filter_expr (str, Optional):
+            * filter_expr(str, Optional):
                 Can only be specified if VPC flow logs for this subnetwork is enabled. The filter expression is used to define which VPC flow logs should be exported to Cloud Logging.
 
-            * enable (bool, Optional):
+            * enable(bool, Optional):
                 Whether to enable flow logging for this subnetwork. If this field is not explicitly set, it will not appear in get listings. If not set the default behavior is determined by the org policy, if there is no org policy specified, then it will default to disabled.
 
-            * flow_sampling (float, Optional):
+            * flow_sampling(float, Optional):
                 Can only be specified if VPC flow logging for this subnetwork is enabled. The value of the field must be in [0, 1]. Set the sampling rate of VPC flow logs within the subnetwork where 1.0 means all collected logs are reported and 0.0 means no logs are reported. Default is 0.5 unless otherwise specified by the org policy, which means half of all collected logs are reported.
 
-            * metadata_fields (List[str], Optional):
+            * metadata_fields(List[str], Optional):
                 Can only be specified if VPC flow logs for this subnetwork is enabled and "metadata" was set to CUSTOM_METADATA.
 
-            * metadata (str, Optional):
+            * metadata(str, Optional):
                 Can only be specified if VPC flow logs for this subnetwork is enabled. Configures whether all, none or a subset of metadata fields should be added to the reported VPC flow logs. Default is EXCLUDE_ALL_METADATA.
-                    Enum type. Allowed values:
+                Enum type. Allowed values:
                     "CUSTOM_METADATA"
                     "EXCLUDE_ALL_METADATA"
                     "INCLUDE_ALL_METADATA"
 
         role(str, Optional):
             The role of subnetwork. Currently, this field is only used when purpose = INTERNAL_HTTPS_LOAD_BALANCER. The value can be set to ACTIVE or BACKUP. An ACTIVE subnetwork is one that is currently being used for Internal HTTP(S) Load Balancing. A BACKUP subnetwork is one that is ready to be promoted to ACTIVE or is currently draining. This field can be updated with a patch request.
-                Enum type. Allowed values:
+            Enum type. Allowed values:
                 "ACTIVE" - The ACTIVE subnet that is currently used.
                 "BACKUP" - The BACKUP subnet that could be promoted to ACTIVE. Defaults to None.
 
         ipv6_access_type(str, Optional):
             The access type of IPv6 address this subnet holds. It's immutable and can only be specified during creation or the first time the subnet is updated into IPV4_IPV6 dual stack.
-                Enum type. Allowed values:
+            Enum type. Allowed values:
                 "EXTERNAL" - VMs on this subnet will be assigned IPv6 addresses that are accessible via the Internet, as well as the VPC network.
                 "INTERNAL" - VMs on this subnet will be assigned IPv6 addresses that are only accessible over the VPC network. Defaults to None.
 
         fingerprint(str, Optional):
             Fingerprint of this resource. A hash of the contents stored in this object. This field is used in optimistic locking. This field will be ignored when inserting a Subnetwork. An up-to-date fingerprint must be provided in order to update the Subnetwork, otherwise the request will fail with error 412 conditionNotMet. To see the latest fingerprint, make a get() request to retrieve a Subnetwork. Defaults to None.
 
         secondary_ip_ranges(List[Dict[str, Any]], Optional):
             An array of configurations for secondary IP ranges for VM instances contained in this subnetwork. The primary IP of such VM must belong to the primary ipCidrRange of the subnetwork. The alias IPs may belong to either primary or secondary ranges. This field can be updated with a patch request. Defaults to None.
 
-            * ip_cidr_range (str, Optional): The range of IP addresses belonging to this subnetwork secondary range. Provide this property when you create the subnetwork. Ranges must be unique and non-overlapping with all primary and secondary IP ranges within a network. Only IPv4 is supported. The range can be any range listed in the Valid ranges list.
-            * range_name (str, Optional): The name associated with this subnetwork secondary range, used when adding an alias IP range to a VM instance. The name must be 1-63 characters long, and comply with RFC1035. The name must be unique within the subnetwork.
+            * ip_cidr_range(str, Optional):
+                The range of IP addresses belonging to this subnetwork secondary range. Provide this property when you create the subnetwork. Ranges must be unique and non-overlapping with all primary and secondary IP ranges within a network. Only IPv4 is supported. The range can be any range listed in the Valid ranges list.
+            * range_name(str, Optional):
+                The name associated with this subnetwork secondary range, used when adding an alias IP range to a VM instance. The name must be 1-63 characters long, and comply with RFC1035. The name must be unique within the subnetwork.
 
         purpose(str, Optional):
             The purpose of the resource. This field can be either PRIVATE_RFC_1918 or INTERNAL_HTTPS_LOAD_BALANCER. A subnetwork with purpose set to INTERNAL_HTTPS_LOAD_BALANCER is a user-created subnetwork that is reserved for Internal HTTP(S) Load Balancing. If unspecified, the purpose defaults to PRIVATE_RFC_1918. The enableFlowLogs field isn't supported with the purpose field set to INTERNAL_HTTPS_LOAD_BALANCER.
-                Enum type. Allowed values:
+            Enum type. Allowed values:
                 "INTERNAL_HTTPS_LOAD_BALANCER" - Subnet reserved for Internal HTTP(S) Load Balancing.
                 "PRIVATE" - Regular user created or automatically created subnet.
                 "PRIVATE_RFC_1918" - Regular user created or automatically created subnet.
                 "PRIVATE_SERVICE_CONNECT" - Subnetworks created for Private Service Connect in the producer network.
                 "REGIONAL_MANAGED_PROXY" - Subnetwork used for Regional Internal/External HTTP(S) Load Balancing. Defaults to None.
 
         private_ipv6_google_access(str, Optional):
             This field is for internal use. This field can be both set at resource creation time and updated using patch.
-                Enum type. Allowed values:
+            Enum type. Allowed values:
                 "DISABLE_GOOGLE_ACCESS" - Disable private IPv6 access to/from Google services.
                 "ENABLE_BIDIRECTIONAL_ACCESS_TO_GOOGLE" - Bidirectional private IPv6 access to/from Google services.
                 "ENABLE_OUTBOUND_VM_ACCESS_TO_GOOGLE" - Outbound private IPv6 access from VMs in this subnet to Google services. Defaults to None.
 
         ip_cidr_range(str, Optional):
             The range of internal addresses that are owned by this subnetwork. Provide this property when you create the subnetwork. For example, 10.0.0.0/8 or 100.64.0.0/10. Ranges must be unique and non-overlapping within a network. Only IPv4 is supported. This field is set at resource creation time. The range can be any range listed in the Valid ranges list. The range can be expanded after creation using expandIpCidrRange. Defaults to None.
```

### Comparing `idem_gcp-1.1.0/idem_gcp/states/gcp/compute/target_pool.py` & `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/target_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""State module for managing target tools."""
+"""State module for managing Target Pool."""
 from typing import Any
 from typing import Dict
 from typing import List
 
 __contracts__ = ["resource"]
 
 
@@ -20,24 +20,24 @@
     backup_pool: str = None,
     request_id: str = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
     r"""Creates a target pool in the specified project and region using the data included in the request.
 
     Args:
-        name (str):
+        name(str):
             An Idem name of the resource.
-        instances (List[str], Optional):
+        instances(List[str], Optional):
             A list of resource URLs to the virtual machine instances serving this pool. They must live in zones contained in the same region as this pool. Defaults to None.
-        session_affinity (str, Optional):
+        session_affinity(str, Optional):
             Session affinity option, must be one of the following values:
             NONE: Connections from the same client IP may go to any instance in the pool.
             CLIENT_IP: Connections from the same client IP will go to the same instance in the pool while that instance remains healthy.
             CLIENT_IP_PROTO: Connections from the same client IP with the same IP protocol will go to the same instance in the pool while that instance remains healthy.
-        description (str, Optional):
+        description(str, Optional):
             An optional description of this resource. Provide this property when you create the resource. Defaults to None.
         region(str, Optional):
             Name of the region scoping this request.
         failover_ratio(float, Optional):
             This field is applicable only when the containing target pool is serving a forwarding rule as the primary pool (i.e., not as a backup pool to some other target pool). The value of the field must be in [0, 1]. If set, backupPool must also be set. They together define the fallback behavior of the primary target pool: if the ratio of the healthy instances in the primary pool is at or below this number, traffic arriving at the load-balanced IP will be directed to the backup pool. In case where failoverRatio is not set or all the instances in the backup pool are unhealthy, the traffic will be directed back to the primary pool in the "force" mode, where traffic will be spread to the healthy instances with the best effort, or to all instances when no instance is healthy. Defaults to None.
         health_checks(List[str], Optional):
             The URL of the HttpHealthCheck resource. A member instance in this pool is considered healthy if and only if the health checks pass. Only legacy HttpHealthChecks are supported. Only one health check may be specified. Defaults to None.
@@ -90,22 +90,27 @@
     region: str = None,
     request_id: str = None,
     resource_id: str = None,
 ) -> Dict[str, Any]:
     r"""Deletes the specified target pool.
 
     Args:
-        name (str): An Idem name of the resource.
+        name(str):
+            An Idem name of the resource.
+
         project(str, Optional):
             Project ID for this request.
-        region (str, Optional):
+
+        region(str, Optional):
             Name of the region scoping this request.
-        request_id (str, Optional):
+
+        request_id(str, Optional):
             An optional request ID to identify requests. Specify a unique request ID so that if you must retry your request, the server will know to ignore the request if it has already been completed. For example, consider a situation where you make an initial request and the request times out. If you make the request again with the same request ID, the server can check if original operation with the same request ID was received, and if so, will ignore the second request. This prevents clients from accidentally creating duplicate commitments. The request ID must be a valid UUID with the exception that zero UUID is not supported ( 00000000-0000-0000-0000-000000000000). Defaults to None.
-        resource_id (str, Optional):
+
+        resource_id(str, Optional):
             An identifier of the resource in the provider. Defaults to None.
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
```

### Comparing `idem_gcp-1.1.0/idem_gcp/states/gcp/iam/projects/service_account.py` & `idem_gcp-1.2.0/idem_gcp/states/gcp/iam/projects/service_account.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,27 +23,48 @@
     etag: str = None,
     disabled: bool = None,
     oauth2_client_id: str = None,
 ) -> Dict[str, Any]:
     """Create or update a service account resource.
 
     Args:
-        name(str, Optional): The resource name of the service account.
-        resource_id(str, Optional): An identifier of the resource in the provider. Defaults to None.
-        project_id(str, Optional): A valid API project identifier.
-        account_id(str): Required on create. The account id that is used to generate the service account email address
-        and a stable unique id. It is unique within a project, must be 6-30 characters long, and match the regular
-        expression [a-z]([-a-z0-9]*[a-z0-9]) to comply with RFC1035.
-        display_name(str, Optional): A user-specified, human-readable name for the service account. The maximum length is 100 UTF-8 bytes.
-        description(str, Optional): A user-specified, human-readable description of the service account. The maximum length is 256 UTF-8 bytes.
-        unique_id(str, Optional): The unique, stable numeric ID for the service account.
-        email(str, Optional): The email address of the service account.
-        etag(str, Optional): A base64-encoded string.
-        disabled(str, Optional): Output only. Whether the service account is disabled.
-        oauth2_client_id(str, Optional): The OAuth 2.0 client ID for the service account.
+        name(str, Optional):
+            The resource name of the service account.
+
+        resource_id(str, Optional):
+            An identifier of the resource in the provider. Defaults to None.
+
+        project_id(str, Optional):
+            A valid API project identifier.
+
+        account_id(str):
+            Required on create. The account id that is used to generate the service account email address
+            and a stable unique id. It is unique within a project, must be 6-30 characters long, and match the regular
+            expression [a-z]([-a-z0-9]*[a-z0-9]) to comply with RFC1035.
+
+        display_name(str, Optional):
+            A user-specified, human-readable name for the service account. The maximum length is 100 UTF-8 bytes.
+
+        description(str, Optional):
+            A user-specified, human-readable description of the service account. The maximum length is 256 UTF-8 bytes.
+
+        unique_id(str, Optional):
+            The unique, stable numeric ID for the service account.
+
+        email(str, Optional):
+            The email address of the service account.
+
+        etag(str, Optional):
+            A base64-encoded string.
+
+        disabled(str, Optional):
+            Output only. Whether the service account is disabled.
+
+        oauth2_client_id(str, Optional):
+            The OAuth 2.0 client ID for the service account.
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
```

### Comparing `idem_gcp-1.1.0/idem_gcp/states/gcp/iam/projects/service_accounts/key.py` & `idem_gcp-1.2.0/idem_gcp/states/gcp/iam/projects/service_accounts/key.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/states/gcp/recursive_contracts/init.py` & `idem_gcp-1.2.0/idem_gcp/states/gcp/recursive_contracts/init.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,16 +263,18 @@
             If resource_id is NOT provided and cannot be constructed, then it is directly assumed that the
             resource does not exist in the Cloud. We then return then result["resutl"]=True and result["comment"]
             that the resource is already absent.
         2. Using resource_id check for resource existence by getting the resource current state from the Cloud.
             If the resource is found then delete it or return already absent comment.
 
     Args:
-        hub: The redistributed pop central hub. The root of the namespace that pop operates on.
-        ctx: Invocation context for this command.
+        hub:
+            The redistributed pop central hub. The root of the namespace that pop operates on.
+        ctx:
+            Invocation context for this command.
 
 
     Returns: The result of a resource deletion state.
 
     """
     state_ctx = ctx.kwargs.get("ctx")
     assert state_ctx, f"state context is missing: {state_ctx}"
```

### Comparing `idem_gcp-1.1.0/idem_gcp/states/gcp/storage/bucket.py` & `idem_gcp-1.2.0/idem_gcp/states/gcp/storage/bucket.py`

 * *Files 3% similar despite different names*

```diff
@@ -269,199 +269,257 @@
 
         user_project(str, Optional):
             The project to be billed for this request. Required for Requester Pays buckets. Defaults to None.
 
         billing(Dict[str, Any], Optional):
             The bucket's billing configuration. Defaults to None.
 
-            * requester_pays (bool, Optional):
+            * requester_pays(bool, Optional):
                 When set to true, Requester Pays is enabled for this bucket.
 
         cors(List[Dict[str, Any]], Optional):
             The bucket's Cross-Origin Resource Sharing (CORS) configuration. Defaults to None.
 
-            * max_age_seconds (int, Optional):
+            * max_age_seconds(int, Optional):
                 The value, in seconds, to return in the  Access-Control-Max-Age header used in preflight responses.
-            * method (List[str], Optional):
+            * method(List[str], Optional):
                 The list of HTTP methods on which to include CORS response headers, (GET, OPTIONS, POST, etc) Note: "*" is permitted in the list of methods, and means "any method".
-            * origin (List[str], Optional):
+            * origin(List[str], Optional):
                 The list of Origins eligible to receive CORS response headers. Note: "*" is permitted in the list of origins, and means "any Origin".
-            * response_header (List[str], Optional):
+            * response_header(List[str], Optional):
                 The list of HTTP headers other than the simple response headers to give permission for the user-agent to share across domains.
 
         custom_placement_config(Dict[str, Any], Optional):
             The bucket's custom placement configuration for Custom Dual Regions. Defaults to None.
 
-            * data_locations (List[str], Optional): The list of regional locations in which data is placed.
+            * data_locations(List[str], Optional):
+                The list of regional locations in which data is placed.
 
         default_event_based_hold(bool, Optional):
             The default value for event-based hold on newly created objects in this bucket. Event-based hold is a way to retain objects indefinitely until an event occurs, signified by the hold's release. After being released, such objects will be subject to bucket-level retention (if any). One sample use case of this flag is for banks to hold loan documents for at least 3 years after loan is paid in full. Here, bucket-level retention is 3 years and the event is loan being paid in full. In this example, these objects will be held intact for any number of years until the event has occurred (event-based hold on the object is released) and then 3 more years after that. That means retention duration of the objects begins from the moment event-based hold transitioned from true to false. Objects under event-based hold cannot be deleted, overwritten or archived until the hold is removed. Defaults to None.
 
         encryption(Dict[str, Any], Optional):
             Encryption configuration for a bucket. Defaults to None.
 
-            * default_kms_key_name (str, Optional):
+            * default_kms_key_name(str, Optional):
                 A Cloud KMS key that will be used to encrypt objects inserted into this bucket, if no encryption method is specified.
 
         iam_configuration(Dict[str, Any], Optional):
             The bucket's IAM configuration. Defaults to None.
 
-            * bucket_policy_only (Dict[str, Any], Optional):
+            * bucket_policy_only(Dict[str, Any], Optional):
                 The bucket's uniform bucket-level access configuration. The feature was formerly known as Bucket Policy Only. For backward compatibility, this field will be populated with identical information as the uniformBucketLevelAccess field. We recommend using the uniformBucketLevelAccess field to enable and disable the feature.
 
-                * enabled (bool, Optional):
+                * enabled(bool, Optional):
                     If set, access is controlled only by bucket-level or above IAM policies.
-                * locked_time (str, Optional):
+                * locked_time(str, Optional):
                     The deadline for changing iamConfiguration.bucketPolicyOnly.enabled from true to false in RFC 3339 format. iamConfiguration.bucketPolicyOnly.enabled may be changed from true to false until the locked time, after which the field is immutable.
-            * uniform_bucket_level_access (Dict[str, Any], Optional):
+            * uniform_bucket_level_access(Dict[str, Any], Optional):
                 The bucket's uniform bucket-level access configuration.
 
-                * enabled (bool, Optional):
+                * enabled(bool, Optional):
                     If set, access is controlled only by bucket-level or above IAM policies.
-                * locked_time (str, Optional):
+                * locked_time(str, Optional):
                     The deadline for changing iamConfiguration.uniformBucketLevelAccess.enabled from true to false in RFC 3339  format. iamConfiguration.uniformBucketLevelAccess.enabled may be changed from true to false until the locked time, after which the field is immutable.
-            * public_access_prevention (str, Optional):
+            * public_access_prevention(str, Optional):
                 The bucket's Public Access Prevention configuration. Currently, 'inherited' and 'enforced' are supported.
 
         labels(Dict[str, Any], Optional):
             User-provided labels, in key/value pairs. Defaults to None.
 
         lifecycle(Dict[str, Any], Optional):
             The bucket's lifecycle configuration. See lifecycle management for more information. Defaults to None.
 
-            * rule (List[Dict[str, Any]], Optional):
+            * rule(List[Dict[str, Any]], Optional):
                 A lifecycle management rule, which is made of an action to take and the condition(s) under which the action will be taken.
 
-                * action (Dict[str, Any], Optional):
+                * action(Dict[str, Any], Optional):
                     The action to take.
 
-                    * storage_class (str, Optional):
+                    * storage_class(str, Optional):
                         Target storage class. Required iff the type of the action is SetStorageClass.
-                    * type (str, Optional):
+                    * type(str, Optional):
                         Type of the action. Currently, only Delete, SetStorageClass, and AbortIncompleteMultipartUpload are supported.
-                * condition (Dict[str, Any], Optional):
+                * condition(Dict[str, Any], Optional):
                     The condition(s) under which the action will be taken.
 
-                    * age (int, Optional): Age of an object (in days). This condition is satisfied when an object reaches the specified age.
-                    * created_before (str, Optional): A date in RFC 3339 format with only the date part (for instance, "2013-01-15"). This condition is satisfied when an object is created before midnight of the specified date in UTC.
-                    * custom_time_before (str, Optional): A date in RFC 3339 format with only the date part (for instance, "2013-01-15"). This condition is satisfied when the custom time on an object is before this date in UTC.
-                    * days_since_custom_time (int, Optional): Number of days elapsed since the user-specified timestamp set on an object. The condition is satisfied if the days elapsed is at least this number. If no custom timestamp is specified on an object, the condition does not apply.
-                    * days_since_noncurrent_time (int, Optional): Number of days elapsed since the noncurrent timestamp of an object. The condition is satisfied if the days elapsed is at least this number. This condition is relevant only for versioned objects. The value of the field must be a nonnegative integer. If it's zero, the object version will become eligible for Lifecycle action as soon as it becomes noncurrent.
-                    * is_live (bool, Optional): Relevant only for versioned objects. If the value is true, this condition matches live objects; if the value is false, it matches archived objects.
-                    * matches_pattern (str, Optional): A regular expression that satisfies the RE2 syntax. This condition is satisfied when the name of the object matches the RE2 pattern. Note: This feature is currently in the "Early Access" launch stage and is only available to a whitelisted set of users; that means that this feature may be changed in backward-incompatible ways and that it is not guaranteed to be released.
-                    * matches_prefix (List[str], Optional): List of object name prefixes. This condition will be satisfied when at least one of the prefixes exactly matches the beginning of the object name.
-                    * matches_suffix (List[str], Optional): List of object name suffixes. This condition will be satisfied when at least one of the suffixes exactly matches the end of the object name.
-                    * matches_storage_class (List[str], Optional): Objects having any of the storage classes specified by this condition will be matched. Values include MULTI_REGIONAL, REGIONAL, NEARLINE, COLDLINE, ARCHIVE, STANDARD, and DURABLE_REDUCED_AVAILABILITY.
-                    * noncurrent_time_before (str, Optional): A date in RFC 3339 format with only the date part (for instance, "2013-01-15"). This condition is satisfied when the noncurrent time on an object is before this date in UTC. This condition is relevant only for versioned objects.
-                    * num_newer_versions (int, Optional): Relevant only for versioned objects. If the value is N, this condition is satisfied when there are at least N versions (including the live version) newer than this version of the object.
+                    * age(int, Optional):
+                        Age of an object (in days). This condition is satisfied when an object reaches the specified age.
+                    * created_before(str, Optional):
+                        A date in RFC 3339 format with only the date part (for instance, "2013-01-15"). This condition is satisfied when an object is created before midnight of the specified date in UTC.
+                    * custom_time_before(str, Optional):
+                        A date in RFC 3339 format with only the date part (for instance, "2013-01-15"). This condition is satisfied when the custom time on an object is before this date in UTC.
+                    * days_since_custom_time(int, Optional):
+                        Number of days elapsed since the user-specified timestamp set on an object. The condition is satisfied if the days elapsed is at least this number. If no custom timestamp is specified on an object, the condition does not apply.
+                    * days_since_noncurrent_time(int, Optional):
+                        Number of days elapsed since the noncurrent timestamp of an object. The condition is satisfied if the days elapsed is at least this number. This condition is relevant only for versioned objects. The value of the field must be a nonnegative integer. If it's zero, the object version will become eligible for Lifecycle action as soon as it becomes noncurrent.
+                    * is_live(bool, Optional):
+                        Relevant only for versioned objects. If the value is true, this condition matches live objects; if the value is false, it matches archived objects.
+                    * matches_pattern(str, Optional):
+                        A regular expression that satisfies the RE2 syntax. This condition is satisfied when the name of the object matches the RE2 pattern. Note: This feature is currently in the "Early Access" launch stage and is only available to a whitelisted set of users; that means that this feature may be changed in backward-incompatible ways and that it is not guaranteed to be released.
+                    * matches_prefix(List[str], Optional):
+                        List of object name prefixes. This condition will be satisfied when at least one of the prefixes exactly matches the beginning of the object name.
+                    * matches_suffix(List[str], Optional):
+                        List of object name suffixes. This condition will be satisfied when at least one of the suffixes exactly matches the end of the object name.
+                    * matches_storage_class(List[str], Optional):
+                        Objects having any of the storage classes specified by this condition will be matched. Values include MULTI_REGIONAL, REGIONAL, NEARLINE, COLDLINE, ARCHIVE, STANDARD, and DURABLE_REDUCED_AVAILABILITY.
+                    * noncurrent_time_before(str, Optional):
+                        A date in RFC 3339 format with only the date part (for instance, "2013-01-15"). This condition is satisfied when the noncurrent time on an object is before this date in UTC. This condition is relevant only for versioned objects.
+                    * num_newer_versions(int, Optional):
+                        Relevant only for versioned objects. If the value is N, this condition is satisfied when there are at least N versions (including the live version) newer than this version of the object.
+
         autoclass(Dict[str, Any], Optional):
             The bucket's Autoclass configuration. Defaults to None.
 
-            * enabled (bool, Optional):
+            * enabled(bool, Optional):
                 Whether or not Autoclass is enabled on this bucket
-            * toggle_time (str, Optional):
+            * toggle_time(str, Optional):
                 A date and time in RFC 3339 format representing the instant at which "enabled" was last toggled.
 
         location(str, Optional):
             The location of the bucket. Object data for objects in the bucket resides in physical storage within this region. Defaults to US. See the developer's guide for the authoritative list. Defaults to None.
 
         logging(Dict[str, Any], Optional):
             The bucket's logging configuration, which defines the destination bucket and optional name prefix for the current bucket's logs. Defaults to None.
 
-            * log_bucket (str, Optional):
+            * log_bucket(str, Optional):
                 The destination bucket where the current bucket's logs should be placed.
-            * log_object_prefix (str, Optional):
+            * log_object_prefix(str, Optional):
                 A prefix for log object names.
 
         retention_policy(Dict[str, Any], Optional):
             The bucket's retention policy. The retention policy enforces a minimum retention time for all objects contained in the bucket, based on their creation time. Any attempt to overwrite or delete objects younger than the retention period will result in a PERMISSION_DENIED error. An unlocked retention policy can be modified or removed from the bucket via a storage.buckets.update operation. A locked retention policy cannot be removed or shortened in duration for the lifetime of the bucket. Attempting to remove or decrease period of a locked retention policy will result in a PERMISSION_DENIED error. Defaults to None.
 
-            * is_locked (bool, Optional):
+            * is_locked(bool, Optional):
                 Locks the retention policy. Once locked, an object retention policy cannot be modified.
-            * retention_period (str, Optional):
+            * retention_period(str, Optional):
                 The duration in seconds that objects need to be retained. Retention duration must be greater than zero and less than 100 years. Note that enforcement of retention periods less than a day is not guaranteed. Such periods should only be used for testing purposes.
 
         rpo(str, Optional):
             The Recovery Point Objective (RPO) of this bucket. Set to ASYNC_TURBO to turn on Turbo Replication on a bucket. Defaults to None.
 
         storage_class(str, Optional):
             The bucket's default storage class, used whenever no storageClass is specified for a newly-created object. This defines how objects in the bucket are stored and determines the SLA and the cost of storage. Values include MULTI_REGIONAL, REGIONAL, STANDARD, NEARLINE, COLDLINE, ARCHIVE, and DURABLE_REDUCED_AVAILABILITY. If this value is not specified when the bucket is created, it will default to STANDARD. For more information, see storage classes. Defaults to None.
 
         versioning(Dict[str, Any], Optional):
             The bucket's versioning configuration. Defaults to None.
 
-            * enabled (bool, Optional):
+            * enabled(bool, Optional):
                 While set to true, versioning is fully enabled for this bucket.
 
         website(Dict[str, Any], Optional):
             The bucket's website configuration, controlling how the service behaves when accessing bucket contents as a web site. See the Static Website Examples for more information. Defaults to None.
 
-            * main_page_suffix (str, Optional):
+            * main_page_suffix(str, Optional):
                 If the requested object path is missing, the service will ensure the path has a trailing '/', append this suffix, and attempt to retrieve the resulting object. This allows the creation of index.html objects to represent directory pages.
-            * not_found_page (str, Optional):
+            * not_found_page(str, Optional):
                 If the requested object path is missing, and any mainPageSuffix object is missing, if applicable, the service will return the named object from this bucket as the content for a 404 Not Found result.
 
         metageneration(str, Optional):
             The metadata generation of this bucket. Read-only property
 
         if_metageneration_match(str, Optional):
             Makes the operation conditional on whether bucket's current metageneration matches the given value. Currently used only when locking retention policy
 
         acl(list[Dict[str, Any]], Optional):
             Access controls on the bucket. Defaults to None.
 
-            * bucket (str, Optional): [OutputOnly] The name of the bucket.
-            * domain (str, Optional): [OutputOnly] The domain associated with the entity, if any.
-            * email (str, Optional): [OutputOnly] The email address associated with the entity, if any.
-            * entity (str, Optional): The entity holding the permission, in one of the following forms:
+            * bucket(str, Optional):
+                [OutputOnly] The name of the bucket.
+
+            * domain(str, Optional):
+                [OutputOnly] The domain associated with the entity, if any.
+
+            * email(str, Optional):
+                [OutputOnly] The email address associated with the entity, if any.
+
+            * entity(str, Optional):
+                The entity holding the permission, in one of the following forms:
                 - user-userId
                 - user-email
                 - group-groupId
                 - group-email
                 - domain-domain
                 - project-team-projectId
                 - allUsers
                 - allAuthenticatedUsers Examples:
                 - The user liz@example.com would be user-liz@example.com.
                 - The group example@googlegroups.com would be group-example@googlegroups.com.
                 - To refer to all members of the Google Apps for Business domain example.com, the entity would be domain-example.com.
-            * entity_id (str, Optional): [OutputOnly] The ID for the entity, if any.
-            * etag (str, Optional): [OutputOnly] HTTP 1.1 Entity tag for the access-control entry.
-            * id (str, Optional): [OutputOnly] The ID of the access-control entry.
-            * kind (str, Optional): [OutputOnly] The kind of item this is. For bucket access control entries, this is always storage#bucketAccessControl.
-            * project_team (Dict[str, Any], Optional): [OutputOnly] The project team associated with the entity, if any.
-                * project_number (str, Optional): [OutputOnly] The project number.
-                * team (str, Optional): [OutputOnly] The team.
-            * role (str, Optional): The access permission for the entity.
-            * self_link (str, Optional): [OutputOnly] The link to this access-control entry.
+
+            * entity_id(str, Optional):
+                [OutputOnly] The ID for the entity, if any.
+
+            * etag(str, Optional):
+                [OutputOnly] HTTP 1.1 Entity tag for the access-control entry.
+
+            * id(str, Optional):
+                [OutputOnly] The ID of the access-control entry.
+
+            * kind(str, Optional):
+                [OutputOnly] The kind of item this is. For bucket access control entries, this is always storage#bucketAccessControl.
+
+            * project_team(Dict[str, Any], Optional):
+                [OutputOnly] The project team associated with the entity, if any.
+
+                * project_number(str, Optional):
+                    [OutputOnly] The project number.
+
+                * team(str, Optional):
+                    [OutputOnly] The team.
+
+            * role(str, Optional):
+                The access permission for the entity.
+
+            * self_link(str, Optional):
+                [OutputOnly] The link to this access-control entry.
 
         default_object_acl(list[Dict[str, Any]], Optional):
             Default access controls to apply to new objects when no ACL is provided. Defaults to None.
 
-            * domain (str, Optional): [OutputOnly] The domain associated with the entity, if any.
-            * email (str, Optional): [OutputOnly] The email address associated with the entity, if any.
-            * entity (str, Optional): The entity holding the permission, in one of the following forms:
+            * domain(str, Optional):
+                [OutputOnly] The domain associated with the entity, if any.
+
+            * email(str, Optional):
+                [OutputOnly] The email address associated with the entity, if any.
+
+            * entity(str, Optional):
+                The entity holding the permission, in one of the following forms:
                 - user-userId
                 - user-email
                 - group-groupId
                 - group-email
                 - domain-domain
                 - project-team-projectId
                 - allUsers
                 - allAuthenticatedUsers Examples:
                 - The user liz@example.com would be user-liz@example.com.
                 - The group example@googlegroups.com would be group-example@googlegroups.com.
                 - To refer to all members of the Google Apps for Business domain example.com, the entity would be domain-example.com.
-            * entity_id (str, Optional): [OutputOnly] The ID for the entity, if any.
-            * etag (str, Optional): [OutputOnly] HTTP 1.1 Entity tag for the access-control entry.
-            * kind (str, Optional): [OutputOnly] The kind of item this is. For object access control entries, this is always storage#objectAccessControl.
-            * project_team (Dict[str, Any], Optional): [OutputOnly] The project team associated with the entity, if any.
-                * project_number (str, Optional): [OutputOnly] The project number.
-                * team (str, Optional): [OutputOnly] The team.
-            * role (str, Optional): The access permission for the entity.
+
+            * entity_id(str, Optional):
+                [OutputOnly] The ID for the entity, if any.
+
+            * etag(str, Optional):
+                [OutputOnly] HTTP 1.1 Entity tag for the access-control entry.
+
+            * kind(str, Optional):
+                [OutputOnly] The kind of item this is. For object access control entries, this is always storage#objectAccessControl.
+
+            * project_team(Dict[str, Any], Optional):
+                [OutputOnly] The project team associated with the entity, if any.
+
+                * project_number(str, Optional):
+                    [OutputOnly] The project number.
+
+                * team(str, Optional):
+                    [OutputOnly] The team.
+
+            * role(str, Optional):
+                The access permission for the entity.
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
```

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/case.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/case.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/cloudkms/crypto_key_version_utils.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/cloudkms/crypto_key_version_utils.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/cloudkms/patch.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/cloudkms/patch.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/comment_utils.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/comment_utils.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/compute/disk.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/compute/disk.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/compute/instance.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/compute/instance.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/compute/instance_group.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/compute/instance_group.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/compute/network.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/compute/network.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/compute/subnetwork.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/compute/subnetwork.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/conversion_utils.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/exec_context.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/exec_context.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/exec_param.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/exec_param.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/generic_exec.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/generic_exec.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/post_exec/item_getter.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/post_exec/item_getter.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/post_exec/operation_processor.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/post_exec/operation_processor.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/pre_exec/function_getter.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/pre_exec/function_getter.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/pre_exec/parameter_sanitizer.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/pre_exec/parameter_sanitizer.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/generate/operators/pre_exec/resource_id_extractor.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/pre_exec/resource_id_extractor.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/hub_resolver.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/hub_resolver.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/init.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/init.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/operation_utils.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/operation_utils.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/policy.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/policy.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/resolver.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/resolver.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/resource_prop_utils.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/resource_prop_utils.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/sanitizers.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/sanitizers.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/schema/finding.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/schema/finding.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/schema/results_collector.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/schema/results_collector.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/schema/schema_compatibility_checker.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/schema/schema_compatibility_checker.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/schema/schema_naming_checker.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/schema/schema_naming_checker.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/schema/scm_utils.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/schema/scm_utils.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/session.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/session.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/state_comparison_utils.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/state_comparison_utils.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/state_operation_utils.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/state_operation_utils.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/storage/bucket.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/storage/bucket.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp/tool/gcp/utils.py` & `idem_gcp-1.2.0/idem_gcp/tool/gcp/utils.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/idem_gcp.egg-info/PKG-INFO` & `idem_gcp-1.2.0/idem_gcp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-gcp
-Version: 1.1.0
+Version: 1.2.0
 Summary: GCP Cloud Provider for Idem
 Home-page: https://gitlab.com/vmware/idem/idem-gcp
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/idem/idem-gcp
 Project-URL: Issue tracker, https://gitlab.com/vmware/idem/idem-gcp/-/issues
```

### Comparing `idem_gcp-1.1.0/idem_gcp.egg-info/SOURCES.txt` & `idem_gcp-1.2.0/idem_gcp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.1.0/setup.py` & `idem_gcp-1.2.0/setup.py`

 * *Files identical despite different names*

