# Comparing `tmp/kubemarine-0.18.0.tar.gz` & `tmp/kubemarine-0.18.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubemarine-0.18.0.tar", last modified: Fri Jun  2 11:14:55 2023, max compression
+gzip compressed data, was "kubemarine-0.18.1.tar", last modified: Mon Jun 19 10:32:52 2023, max compression
```

## Comparing `kubemarine-0.18.0.tar` & `kubemarine-0.18.1.tar`

### file list

```diff
@@ -1,241 +1,241 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.455617 kubemarine-0.18.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-02 11:14:41.000000 kubemarine-0.18.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      183 2023-06-02 11:14:41.000000 kubemarine-0.18.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    12413 2023-06-02 11:14:55.455617 kubemarine-0.18.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8986 2023-06-02 11:14:41.000000 kubemarine-0.18.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.427617 kubemarine-0.18.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)     1076 2023-06-02 11:14:41.000000 kubemarine-0.18.0/bin/kubemarine
--rw-r--r--   0 root         (0) root         (0)      657 2023-06-02 11:14:41.000000 kubemarine-0.18.0/bin/kubemarine.cmd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.431617 kubemarine-0.18.0/kubemarine/
--rw-r--r--   0 root         (0) root         (0)      603 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     8218 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/__main__.py
--rw-r--r--   0 root         (0) root         (0)    45051 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/admission.py
--rw-r--r--   0 root         (0) root         (0)     4862 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/apparmor.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/apt.py
--rw-r--r--   0 root         (0) root         (0)     4596 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/audit.py
--rw-r--r--   0 root         (0) root         (0)     2225 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/controlplane.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.431617 kubemarine-0.18.0/kubemarine/core/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2355 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/action.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/annotations.py
--rwxr-xr-x   0 root         (0) root         (0)    15520 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/cluster.py
--rw-r--r--   0 root         (0) root         (0)     4162 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/connections.py
--rwxr-xr-x   0 root         (0) root         (0)    23860 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/defaults.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/environment.py
--rw-r--r--   0 root         (0) root         (0)     5659 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/errors.py
--rw-r--r--   0 root         (0) root         (0)    16778 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/executor.py
--rwxr-xr-x   0 root         (0) root         (0)    18912 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/flow.py
--rwxr-xr-x   0 root         (0) root         (0)    41420 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/group.py
--rw-r--r--   0 root         (0) root         (0)    14424 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/log.py
--rw-r--r--   0 root         (0) root         (0)     1043 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/os.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/patch.py
--rw-r--r--   0 root         (0) root         (0)     8372 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/resources.py
--rw-r--r--   0 root         (0) root         (0)    15178 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/schema.py
--rw-r--r--   0 root         (0) root         (0)     2230 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/static.py
--rw-r--r--   0 root         (0) root         (0)     2110 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/summary.py
--rwxr-xr-x   0 root         (0) root         (0)    21325 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/utils.py
--rw-r--r--   0 root         (0) root         (0)     1671 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/core/yaml_merger.py
--rw-r--r--   0 root         (0) root         (0)     7067 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/coredns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.435617 kubemarine-0.18.0/kubemarine/cri/
--rw-r--r--   0 root         (0) root         (0)     2918 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/cri/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     6492 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/cri/containerd.py
--rwxr-xr-x   0 root         (0) root         (0)     3784 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/cri/docker.py
--rw-r--r--   0 root         (0) root         (0)    20072 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/demo.py
--rw-r--r--   0 root         (0) root         (0)     4664 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/etcd.py
--rw-r--r--   0 root         (0) root         (0)    10967 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/haproxy.py
--rw-r--r--   0 root         (0) root         (0)     2259 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/jinja.py
--rw-r--r--   0 root         (0) root         (0)     3437 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/k8s_certs.py
--rw-r--r--   0 root         (0) root         (0)    11269 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/keepalived.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.435617 kubemarine-0.18.0/kubemarine/kubernetes/
--rw-r--r--   0 root         (0) root         (0)    65136 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2189 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/kubernetes/daemonset.py
--rw-r--r--   0 root         (0) root         (0)     1753 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/kubernetes/deployment.py
--rw-r--r--   0 root         (0) root         (0)     3262 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/kubernetes/object.py
--rw-r--r--   0 root         (0) root         (0)     2132 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/kubernetes/replicaset.py
--rw-r--r--   0 root         (0) root         (0)     1977 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/kubernetes/statefulset.py
--rw-r--r--   0 root         (0) root         (0)     5780 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/kubernetes_accounts.py
--rw-r--r--   0 root         (0) root         (0)    29985 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/packages.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.435617 kubemarine-0.18.0/kubemarine/patches/
--rw-r--r--   0 root         (0) root         (0)     1126 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/patches/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/patches/software_upgrade.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.435617 kubemarine-0.18.0/kubemarine/plugins/
--rwxr-xr-x   0 root         (0) root         (0)    40081 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3769 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/builtin.py
--rwxr-xr-x   0 root         (0) root         (0)    14938 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/calico.py
--rw-r--r--   0 root         (0) root         (0)     4842 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/kubernetes_dashboard.py
--rw-r--r--   0 root         (0) root         (0)     5721 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/local_path_provisioner.py
--rw-r--r--   0 root         (0) root         (0)    16606 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/manifest.py
--rw-r--r--   0 root         (0) root         (0)    19568 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/nginx_ingress.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.439617 kubemarine-0.18.0/kubemarine/plugins/yaml/
--rw-r--r--   0 root         (0) root         (0)   222019 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml
--rw-r--r--   0 root         (0) root         (0)   239857 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml
--rw-r--r--   0 root         (0) root         (0)   243952 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)     7621 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml
--rw-r--r--   0 root         (0) root         (0)     7621 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml
--rw-r--r--   0 root         (0) root         (0)     2935 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15311 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15775 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml
--rw-r--r--   0 root         (0) root         (0)    15704 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.439617 kubemarine-0.18.0/kubemarine/procedures/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4919 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/add_node.py
--rwxr-xr-x   0 root         (0) root         (0)    20581 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/backup.py
--rwxr-xr-x   0 root         (0) root         (0)     2629 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/cert_renew.py
--rwxr-xr-x   0 root         (0) root         (0)    50185 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/check_iaas.py
--rwxr-xr-x   0 root         (0) root         (0)    72418 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/check_paas.py
--rwxr-xr-x   0 root         (0) root         (0)     5081 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/do.py
--rwxr-xr-x   0 root         (0) root         (0)    26620 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/install.py
--rwxr-xr-x   0 root         (0) root         (0)     1769 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/manage_psp.py
--rwxr-xr-x   0 root         (0) root         (0)     1667 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/manage_pss.py
--rwxr-xr-x   0 root         (0) root         (0)    14845 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/migrate_cri.py
--rw-r--r--   0 root         (0) root         (0)    19510 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/migrate_kubemarine.py
--rwxr-xr-x   0 root         (0) root         (0)     2380 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/reboot.py
--rwxr-xr-x   0 root         (0) root         (0)     6074 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/remove_node.py
--rwxr-xr-x   0 root         (0) root         (0)    13653 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/restore.py
--rwxr-xr-x   0 root         (0) root         (0)    11219 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/procedures/upgrade.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.439617 kubemarine-0.18.0/kubemarine/resources/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.443617 kubemarine-0.18.0/kubemarine/resources/configurations/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/configurations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.443617 kubemarine-0.18.0/kubemarine/resources/configurations/compatibility/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.443617 kubemarine-0.18.0/kubemarine/resources/configurations/compatibility/internal/
--rw-r--r--   0 root         (0) root         (0)     3605 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml
--rw-r--r--   0 root         (0) root         (0)     5037 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml
--rw-r--r--   0 root         (0) root         (0)     3849 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml
--rw-r--r--   0 root         (0) root         (0)     5903 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml
--rw-r--r--   0 root         (0) root         (0)     3020 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml
--rw-r--r--   0 root         (0) root         (0)    25005 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/configurations/defaults.yaml
--rw-r--r--   0 root         (0) root         (0)    10638 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/configurations/globals.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.443617 kubemarine-0.18.0/kubemarine/resources/drop_ins/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/drop_ins/__init__.py
--rw-r--r--   0 root         (0) root         (0)       25 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/drop_ins/haproxy.conf
--rw-r--r--   0 root         (0) root         (0)       25 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/drop_ins/keepalived.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.423617 kubemarine-0.18.0/kubemarine/resources/etalons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.443617 kubemarine-0.18.0/kubemarine/resources/etalons/patches/
--rw-r--r--   0 root         (0) root         (0)     1126 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/etalons/patches/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/etalons/patches/software_upgrade.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.443617 kubemarine-0.18.0/kubemarine/resources/psp/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/psp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/psp/anyuid.yaml
--rw-r--r--   0 root         (0) root         (0)     1923 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/psp/default.yaml
--rw-r--r--   0 root         (0) root         (0)     1618 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/psp/host-network.yaml
--rw-r--r--   0 root         (0) root         (0)     1204 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/psp/privileged.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.443617 kubemarine-0.18.0/kubemarine/resources/reports/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/reports/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1773 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/reports/check_report.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.447617 kubemarine-0.18.0/kubemarine/resources/schemas/
--rw-r--r--   0 root         (0) root         (0)      832 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/add_node.json
--rw-r--r--   0 root         (0) root         (0)     2651 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/backup.json
--rw-r--r--   0 root         (0) root         (0)     1038 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/cert_renew.json
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/check_paas.json
--rw-r--r--   0 root         (0) root         (0)     3142 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/cluster.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.447617 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.447617 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/common/
--rw-r--r--   0 root         (0) root         (0)      520 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/common/node_ref.json
--rw-r--r--   0 root         (0) root         (0)     1722 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/common/utils.json
--rw-r--r--   0 root         (0) root         (0)      615 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/gateway_node.json
--rw-r--r--   0 root         (0) root         (0)     4072 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/globals.json
--rw-r--r--   0 root         (0) root         (0)     1501 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/node.json
--rw-r--r--   0 root         (0) root         (0)     2217 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/node_defaults.json
--rw-r--r--   0 root         (0) root         (0)      575 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugin_defaults.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.447617 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/
--rw-r--r--   0 root         (0) root         (0)     4806 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/calico.json
--rw-r--r--   0 root         (0) root         (0)     1161 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.451617 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json
--rw-r--r--   0 root         (0) root         (0)      689 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json
--rw-r--r--   0 root         (0) root         (0)     3120 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json
--rw-r--r--   0 root         (0) root         (0)     1220 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json
--rw-r--r--   0 root         (0) root         (0)      606 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json
--rw-r--r--   0 root         (0) root         (0)     2265 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json
--rw-r--r--   0 root         (0) root         (0)     2498 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json
--rw-r--r--   0 root         (0) root         (0)     1780 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation.json
--rw-r--r--   0 root         (0) root         (0)     2901 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json
--rw-r--r--   0 root         (0) root         (0)     1628 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json
--rw-r--r--   0 root         (0) root         (0)     3201 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json
--rw-r--r--   0 root         (0) root         (0)      605 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins.json
--rw-r--r--   0 root         (0) root         (0)      749 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/procedures.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.451617 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/rbac/
--rw-r--r--   0 root         (0) root         (0)      661 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/rbac/account.json
--rw-r--r--   0 root         (0) root         (0)     3266 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json
--rw-r--r--   0 root         (0) root         (0)     3759 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/rbac/psp.json
--rw-r--r--   0 root         (0) root         (0)     2453 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/rbac/pss.json
--rw-r--r--   0 root         (0) root         (0)      709 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/rbac.json
--rw-r--r--   0 root         (0) root         (0)     1951 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/registry.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.451617 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/
--rw-r--r--   0 root         (0) root         (0)     1855 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/audit.json
--rw-r--r--   0 root         (0) root         (0)     9668 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/coredns.json
--rw-r--r--   0 root         (0) root         (0)     2645 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/cri.json
--rw-r--r--   0 root         (0) root         (0)      644 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json
--rw-r--r--   0 root         (0) root         (0)     1963 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/kernel_security.json
--rw-r--r--   0 root         (0) root         (0)     4856 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/kubeadm.json
--rw-r--r--   0 root         (0) root         (0)      628 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json
--rw-r--r--   0 root         (0) root         (0)     3035 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json
--rw-r--r--   0 root         (0) root         (0)     2898 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json
--rw-r--r--   0 root         (0) root         (0)      936 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/modprobe.json
--rw-r--r--   0 root         (0) root         (0)     2302 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/ntp.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.451617 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/packages/
--rw-r--r--   0 root         (0) root         (0)     4198 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/packages/associations.json
--rw-r--r--   0 root         (0) root         (0)     5144 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/packages.json
--rw-r--r--   0 root         (0) root         (0)      479 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/resolv.conf.json
--rw-r--r--   0 root         (0) root         (0)     1176 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/sysctl.json
--rw-r--r--   0 root         (0) root         (0)     3302 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/thirdparties.json
--rw-r--r--   0 root         (0) root         (0)     1881 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services.json
--rw-r--r--   0 root         (0) root         (0)     3130 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/definitions/vrrp_ip.json
--rw-r--r--   0 root         (0) root         (0)      757 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/manage_psp.json
--rw-r--r--   0 root         (0) root         (0)     1657 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/manage_pss.json
--rw-r--r--   0 root         (0) root         (0)     1608 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/migrate_cri.json
--rw-r--r--   0 root         (0) root         (0)     2885 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/migrate_kubemarine.json
--rw-r--r--   0 root         (0) root         (0)      798 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/reboot.json
--rw-r--r--   0 root         (0) root         (0)      872 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/remove_node.json
--rw-r--r--   0 root         (0) root         (0)     3365 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/restore.json
--rw-r--r--   0 root         (0) root         (0)     2775 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/schemas/upgrade.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.451617 kubemarine-0.18.0/kubemarine/resources/scripts/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/scripts/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      288 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/scripts/check_haproxy.sh
--rw-r--r--   0 root         (0) root         (0)     1206 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/scripts/check_url_availability.py
--rwxr-xr-x   0 root         (0) root         (0)     3996 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/scripts/etcdctl.sh
--rw-r--r--   0 root         (0) root         (0)     1499 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/resources/scripts/simple_tcp_listener.py
--rw-r--r--   0 root         (0) root         (0)     7984 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/selinux.py
--rw-r--r--   0 root         (0) root         (0)     3815 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/sysctl.py
--rw-r--r--   0 root         (0) root         (0)    26444 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.455617 kubemarine-0.18.0/kubemarine/templates/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)      667 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/admission.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     2259 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/haproxy.cfg.j2
--rw-r--r--   0 root         (0) root         (0)      714 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/keepalived.conf.j2
--rw-r--r--   0 root         (0) root         (0)     1126 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/kubelet.service.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.455617 kubemarine-0.18.0/kubemarine/templates/patches/
--rw-r--r--   0 root         (0) root         (0)      151 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/patches/control-plane-pod.json.j2
--rw-r--r--   0 root         (0) root         (0)       76 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/patches/kubelet.yaml.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.455617 kubemarine-0.18.0/kubemarine/templates/plugins/
--rw-r--r--   0 root         (0) root         (0)      604 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      879 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/calico-ippool.yaml.j2
--rw-r--r--   0 root         (0) root         (0)      286 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/calico-kube-controllers-metrics.yaml
--rw-r--r--   0 root         (0) root         (0)      245 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/calico-metrics.yaml
--rw-r--r--   0 root         (0) root         (0)      436 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/calico-rr.sh.j2
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/calico-rr.yaml.j2
--rw-r--r--   0 root         (0) root         (0)      136 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/calicoctl.cfg.j2
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/dashboard-ingress.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     8826 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     8905 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     2749 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/iperf3.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     5401 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2
--rw-r--r--   0 root         (0) root         (0)     9973 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2
--rw-r--r--   0 root         (0) root         (0)    17847 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2
--rw-r--r--   0 root         (0) root         (0)    11284 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/testsuite.py
--rw-r--r--   0 root         (0) root         (0)    17436 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/thirdparties.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/version
--rw-r--r--   0 root         (0) root         (0)     4843 2023-06-02 11:14:41.000000 kubemarine-0.18.0/kubemarine/yum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 11:14:55.431617 kubemarine-0.18.0/kubemarine.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12413 2023-06-02 11:14:55.000000 kubemarine-0.18.0/kubemarine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9113 2023-06-02 11:14:55.000000 kubemarine-0.18.0/kubemarine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 11:14:55.000000 kubemarine-0.18.0/kubemarine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-02 11:14:55.000000 kubemarine-0.18.0/kubemarine.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      278 2023-06-02 11:14:55.000000 kubemarine-0.18.0/kubemarine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-02 11:14:55.000000 kubemarine-0.18.0/kubemarine.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2554 2023-06-02 11:14:41.000000 kubemarine-0.18.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-02 11:14:55.455617 kubemarine-0.18.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1628 2023-06-02 11:14:41.000000 kubemarine-0.18.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.493515 kubemarine-0.18.1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-19 10:32:36.000000 kubemarine-0.18.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      183 2023-06-19 10:32:36.000000 kubemarine-0.18.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    12413 2023-06-19 10:32:52.493515 kubemarine-0.18.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8986 2023-06-19 10:32:36.000000 kubemarine-0.18.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.445515 kubemarine-0.18.1/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     1076 2023-06-19 10:32:36.000000 kubemarine-0.18.1/bin/kubemarine
+-rw-r--r--   0 root         (0) root         (0)      657 2023-06-19 10:32:36.000000 kubemarine-0.18.1/bin/kubemarine.cmd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.453515 kubemarine-0.18.1/kubemarine/
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     8218 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    45051 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/admission.py
+-rw-r--r--   0 root         (0) root         (0)     4862 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/apparmor.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/apt.py
+-rw-r--r--   0 root         (0) root         (0)     4596 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/audit.py
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/controlplane.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.457515 kubemarine-0.18.1/kubemarine/core/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/action.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/annotations.py
+-rwxr-xr-x   0 root         (0) root         (0)    15520 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/cluster.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/connections.py
+-rwxr-xr-x   0 root         (0) root         (0)    23860 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/defaults.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/environment.py
+-rw-r--r--   0 root         (0) root         (0)     5659 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    16778 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/executor.py
+-rwxr-xr-x   0 root         (0) root         (0)    18912 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/flow.py
+-rwxr-xr-x   0 root         (0) root         (0)    41420 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/group.py
+-rw-r--r--   0 root         (0) root         (0)    14424 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/log.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/os.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/patch.py
+-rw-r--r--   0 root         (0) root         (0)     8372 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/resources.py
+-rw-r--r--   0 root         (0) root         (0)    15178 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/schema.py
+-rw-r--r--   0 root         (0) root         (0)     2230 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/static.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/summary.py
+-rwxr-xr-x   0 root         (0) root         (0)    21325 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/core/yaml_merger.py
+-rw-r--r--   0 root         (0) root         (0)     7067 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/coredns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.457515 kubemarine-0.18.1/kubemarine/cri/
+-rw-r--r--   0 root         (0) root         (0)     2918 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/cri/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     6492 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/cri/containerd.py
+-rwxr-xr-x   0 root         (0) root         (0)     3784 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/cri/docker.py
+-rw-r--r--   0 root         (0) root         (0)    20072 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/demo.py
+-rw-r--r--   0 root         (0) root         (0)     4664 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/etcd.py
+-rw-r--r--   0 root         (0) root         (0)    10967 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/haproxy.py
+-rw-r--r--   0 root         (0) root         (0)     2259 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/jinja.py
+-rw-r--r--   0 root         (0) root         (0)     3437 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/k8s_certs.py
+-rw-r--r--   0 root         (0) root         (0)    11269 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/keepalived.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.457515 kubemarine-0.18.1/kubemarine/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)    65136 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/kubernetes/daemonset.py
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/kubernetes/deployment.py
+-rw-r--r--   0 root         (0) root         (0)     3262 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/kubernetes/object.py
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/kubernetes/replicaset.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/kubernetes/statefulset.py
+-rw-r--r--   0 root         (0) root         (0)     5780 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/kubernetes_accounts.py
+-rw-r--r--   0 root         (0) root         (0)    29985 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/packages.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.461515 kubemarine-0.18.1/kubemarine/patches/
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/patches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/patches/software_upgrade.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.461515 kubemarine-0.18.1/kubemarine/plugins/
+-rwxr-xr-x   0 root         (0) root         (0)    40081 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3769 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/builtin.py
+-rwxr-xr-x   0 root         (0) root         (0)    14938 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/calico.py
+-rw-r--r--   0 root         (0) root         (0)     4842 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/kubernetes_dashboard.py
+-rw-r--r--   0 root         (0) root         (0)     5721 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/local_path_provisioner.py
+-rw-r--r--   0 root         (0) root         (0)    16606 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/manifest.py
+-rw-r--r--   0 root         (0) root         (0)    19568 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/nginx_ingress.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.465515 kubemarine-0.18.1/kubemarine/plugins/yaml/
+-rw-r--r--   0 root         (0) root         (0)   222019 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   239857 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml
+-rw-r--r--   0 root         (0) root         (0)   243952 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     7621 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     7621 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15311 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15775 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml
+-rw-r--r--   0 root         (0) root         (0)    15704 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.469515 kubemarine-0.18.1/kubemarine/procedures/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4919 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/add_node.py
+-rwxr-xr-x   0 root         (0) root         (0)    20581 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/backup.py
+-rwxr-xr-x   0 root         (0) root         (0)     2629 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/cert_renew.py
+-rwxr-xr-x   0 root         (0) root         (0)    50185 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/check_iaas.py
+-rwxr-xr-x   0 root         (0) root         (0)    72418 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/check_paas.py
+-rwxr-xr-x   0 root         (0) root         (0)     5081 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/do.py
+-rwxr-xr-x   0 root         (0) root         (0)    26620 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/install.py
+-rwxr-xr-x   0 root         (0) root         (0)     1769 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/manage_psp.py
+-rwxr-xr-x   0 root         (0) root         (0)     1667 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/manage_pss.py
+-rwxr-xr-x   0 root         (0) root         (0)    14845 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/migrate_cri.py
+-rw-r--r--   0 root         (0) root         (0)    19510 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/migrate_kubemarine.py
+-rwxr-xr-x   0 root         (0) root         (0)     2380 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/reboot.py
+-rwxr-xr-x   0 root         (0) root         (0)     6074 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/remove_node.py
+-rwxr-xr-x   0 root         (0) root         (0)    13653 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/restore.py
+-rwxr-xr-x   0 root         (0) root         (0)    11219 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/procedures/upgrade.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.469515 kubemarine-0.18.1/kubemarine/resources/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.469515 kubemarine-0.18.1/kubemarine/resources/configurations/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/configurations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.469515 kubemarine-0.18.1/kubemarine/resources/configurations/compatibility/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.473515 kubemarine-0.18.1/kubemarine/resources/configurations/compatibility/internal/
+-rw-r--r--   0 root         (0) root         (0)     3826 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml
+-rw-r--r--   0 root         (0) root         (0)     5333 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/configurations/compatibility/internal/packages.yaml
+-rw-r--r--   0 root         (0) root         (0)     4067 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/configurations/compatibility/internal/plugins.yaml
+-rw-r--r--   0 root         (0) root         (0)     6255 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml
+-rw-r--r--   0 root         (0) root         (0)     3177 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml
+-rw-r--r--   0 root         (0) root         (0)    25005 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/configurations/defaults.yaml
+-rw-r--r--   0 root         (0) root         (0)    10638 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/configurations/globals.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.473515 kubemarine-0.18.1/kubemarine/resources/drop_ins/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/drop_ins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/drop_ins/haproxy.conf
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/drop_ins/keepalived.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.445515 kubemarine-0.18.1/kubemarine/resources/etalons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.473515 kubemarine-0.18.1/kubemarine/resources/etalons/patches/
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/etalons/patches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/etalons/patches/software_upgrade.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.473515 kubemarine-0.18.1/kubemarine/resources/psp/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/psp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/psp/anyuid.yaml
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/psp/default.yaml
+-rw-r--r--   0 root         (0) root         (0)     1618 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/psp/host-network.yaml
+-rw-r--r--   0 root         (0) root         (0)     1204 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/psp/privileged.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.473515 kubemarine-0.18.1/kubemarine/resources/reports/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/reports/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1773 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/reports/check_report.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.477515 kubemarine-0.18.1/kubemarine/resources/schemas/
+-rw-r--r--   0 root         (0) root         (0)      832 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/add_node.json
+-rw-r--r--   0 root         (0) root         (0)     2651 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/backup.json
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/cert_renew.json
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/check_paas.json
+-rw-r--r--   0 root         (0) root         (0)     3142 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/cluster.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.481515 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.481515 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/common/
+-rw-r--r--   0 root         (0) root         (0)      520 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/common/node_ref.json
+-rw-r--r--   0 root         (0) root         (0)     1722 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/common/utils.json
+-rw-r--r--   0 root         (0) root         (0)      615 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/gateway_node.json
+-rw-r--r--   0 root         (0) root         (0)     4072 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/globals.json
+-rw-r--r--   0 root         (0) root         (0)     1501 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/node.json
+-rw-r--r--   0 root         (0) root         (0)     2217 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/node_defaults.json
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugin_defaults.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.481515 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/
+-rw-r--r--   0 root         (0) root         (0)     4806 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/calico.json
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.485515 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json
+-rw-r--r--   0 root         (0) root         (0)      689 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/config.json
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/expect.json
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/helm.json
+-rw-r--r--   0 root         (0) root         (0)      606 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/python.json
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/shell.json
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/template.json
+-rw-r--r--   0 root         (0) root         (0)     1780 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation.json
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json
+-rw-r--r--   0 root         (0) root         (0)     3201 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json
+-rw-r--r--   0 root         (0) root         (0)      605 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins.json
+-rw-r--r--   0 root         (0) root         (0)      749 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/procedures.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.485515 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/rbac/
+-rw-r--r--   0 root         (0) root         (0)      661 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/rbac/account.json
+-rw-r--r--   0 root         (0) root         (0)     3266 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/rbac/account_defaults.json
+-rw-r--r--   0 root         (0) root         (0)     3759 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/rbac/psp.json
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/rbac/pss.json
+-rw-r--r--   0 root         (0) root         (0)      709 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/rbac.json
+-rw-r--r--   0 root         (0) root         (0)     1951 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/registry.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.485515 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/
+-rw-r--r--   0 root         (0) root         (0)     1855 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/audit.json
+-rw-r--r--   0 root         (0) root         (0)     9668 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/coredns.json
+-rw-r--r--   0 root         (0) root         (0)     2645 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/cri.json
+-rw-r--r--   0 root         (0) root         (0)      644 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/etc_hosts.json
+-rw-r--r--   0 root         (0) root         (0)     1963 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/kernel_security.json
+-rw-r--r--   0 root         (0) root         (0)     4856 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/kubeadm.json
+-rw-r--r--   0 root         (0) root         (0)      628 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json
+-rw-r--r--   0 root         (0) root         (0)     3035 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json
+-rw-r--r--   0 root         (0) root         (0)     2898 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/loadbalancer.json
+-rw-r--r--   0 root         (0) root         (0)      936 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/modprobe.json
+-rw-r--r--   0 root         (0) root         (0)     2302 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/ntp.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.485515 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/packages/
+-rw-r--r--   0 root         (0) root         (0)     4198 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/packages/associations.json
+-rw-r--r--   0 root         (0) root         (0)     5144 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/packages.json
+-rw-r--r--   0 root         (0) root         (0)      479 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/resolv.conf.json
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/sysctl.json
+-rw-r--r--   0 root         (0) root         (0)     3302 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/thirdparties.json
+-rw-r--r--   0 root         (0) root         (0)     1881 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services.json
+-rw-r--r--   0 root         (0) root         (0)     3130 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/definitions/vrrp_ip.json
+-rw-r--r--   0 root         (0) root         (0)      757 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/manage_psp.json
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/manage_pss.json
+-rw-r--r--   0 root         (0) root         (0)     1608 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/migrate_cri.json
+-rw-r--r--   0 root         (0) root         (0)     2885 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/migrate_kubemarine.json
+-rw-r--r--   0 root         (0) root         (0)      798 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/reboot.json
+-rw-r--r--   0 root         (0) root         (0)      872 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/remove_node.json
+-rw-r--r--   0 root         (0) root         (0)     3365 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/restore.json
+-rw-r--r--   0 root         (0) root         (0)     2775 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/schemas/upgrade.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.489515 kubemarine-0.18.1/kubemarine/resources/scripts/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/scripts/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      288 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/scripts/check_haproxy.sh
+-rw-r--r--   0 root         (0) root         (0)     1206 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/scripts/check_url_availability.py
+-rwxr-xr-x   0 root         (0) root         (0)     3996 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/scripts/etcdctl.sh
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/resources/scripts/simple_tcp_listener.py
+-rw-r--r--   0 root         (0) root         (0)     7984 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/selinux.py
+-rw-r--r--   0 root         (0) root         (0)     3815 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/sysctl.py
+-rw-r--r--   0 root         (0) root         (0)    26444 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.489515 kubemarine-0.18.1/kubemarine/templates/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      667 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/admission.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     2259 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/haproxy.cfg.j2
+-rw-r--r--   0 root         (0) root         (0)      714 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/keepalived.conf.j2
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/kubelet.service.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.489515 kubemarine-0.18.1/kubemarine/templates/patches/
+-rw-r--r--   0 root         (0) root         (0)      151 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/patches/control-plane-pod.json.j2
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/patches/kubelet.yaml.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.493515 kubemarine-0.18.1/kubemarine/templates/plugins/
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      879 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/calico-ippool.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)      286 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/calico-kube-controllers-metrics.yaml
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/calico-metrics.yaml
+-rw-r--r--   0 root         (0) root         (0)      436 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/calico-rr.sh.j2
+-rw-r--r--   0 root         (0) root         (0)      960 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/calico-rr.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)      136 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/calicoctl.cfg.j2
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/dashboard-ingress.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     8826 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     8905 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     2749 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/iperf3.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     5401 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/local-path-provisioner.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)     9973 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)    17847 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2
+-rw-r--r--   0 root         (0) root         (0)    11284 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/testsuite.py
+-rw-r--r--   0 root         (0) root         (0)    17436 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/thirdparties.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/version
+-rw-r--r--   0 root         (0) root         (0)     4843 2023-06-19 10:32:36.000000 kubemarine-0.18.1/kubemarine/yum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:32:52.453515 kubemarine-0.18.1/kubemarine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12413 2023-06-19 10:32:52.000000 kubemarine-0.18.1/kubemarine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9113 2023-06-19 10:32:52.000000 kubemarine-0.18.1/kubemarine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 10:32:52.000000 kubemarine-0.18.1/kubemarine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-19 10:32:52.000000 kubemarine-0.18.1/kubemarine.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      278 2023-06-19 10:32:52.000000 kubemarine-0.18.1/kubemarine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-19 10:32:52.000000 kubemarine-0.18.1/kubemarine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2554 2023-06-19 10:32:36.000000 kubemarine-0.18.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 10:32:52.493515 kubemarine-0.18.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-06-19 10:32:36.000000 kubemarine-0.18.1/setup.py
```

### Comparing `kubemarine-0.18.0/LICENSE` & `kubemarine-0.18.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/PKG-INFO` & `kubemarine-0.18.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubemarine
-Version: 0.18.0
+Version: 0.18.1
 Summary: Management tool for Kubernetes cluster deployment and maintenance
 Home-page: https://github.com/Netcracker/KubeMarine
 Author-email: Kubemarine Group <kubemarinegroup@netcracker.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Netcracker/KubeMarine
 Project-URL: Documentation, https://github.com/Netcracker/KubeMarine#documentation
 Project-URL: Issues, https://github.com/Netcracker/KubeMarine/issues/
@@ -33,36 +33,36 @@
 # Kubemarine
 
 Kubemarine is an open source, lightweight and powerful management tool built for end-to-end Kubernetes cluster deployment and maintenance. It is applicable for many purposes like simple and quick onboarding Kubernetes on local and production environments in different HA schemes depending on your aims, budget, and capabilities. Together with simplicity, Kubemarine can be a very flexible and customizable tool covering specific configurability cases on both deployment and maintenance stages. This library provides powerful CLI commands, as well as can be customized using a Python extension API.
 
 ## Highlights
 - Easy to use
 - Many procedures supported:
-  - [install](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#)
-  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#add-node-procedure)
-  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#remove-node-procedure)
-  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#upgrade-procedure)
-  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#backup-procedure)
-  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#restore-procedure)
-  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Kubecheck.md#iaas-procedure)
-  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Kubecheck.md#paas-procedure)
-  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#kubemarine-migration-procedure)
-  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#manage-psp-procedure)
-  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#manage-pss-procedure)
-  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#certificate-renew-procedure)
-  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#migration-cri-procedure)
-- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#configuration) for all operations, highly customizable
+  - [install](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#)
+  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#add-node-procedure)
+  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#remove-node-procedure)
+  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#upgrade-procedure)
+  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#backup-procedure)
+  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#restore-procedure)
+  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Kubecheck.md#iaas-procedure)
+  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Kubecheck.md#paas-procedure)
+  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#kubemarine-migration-procedure)
+  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#manage-psp-procedure)
+  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#manage-pss-procedure)
+  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#certificate-renew-procedure)
+  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#migration-cri-procedure)
+- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#configuration) for all operations, highly customizable
 - Default values of all parameters in configurations with a minimum of required parameters
-- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
-- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
-- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#custom-plugins-installation-procedures) support
-- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#installation-without-internet-resources) with private registries
-- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#dump-files)
+- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
+- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
+- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#custom-plugins-installation-procedures) support
+- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#installation-without-internet-resources) with private registries
+- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#dump-files)
 - Build supported as a package, container, and binary
-- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/PackageExtension.md)
+- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/PackageExtension.md)
 - Support different deployment schemes (all-in-one, mini-HA, HA, and so on)
 
 ## Kubemarine Binary Installation
 Proceed the following steps to install Kubemarine  on your environment:
 1. Download the binary file for your system from the latest [release](https://github.com/Netcracker/KubeMarine/releases)
 2. Move binary kubemarine to a separate folder 
 3. Now you can proceed to run Kubemarine! Try the following:
@@ -80,15 +80,15 @@
    ```bash
    python3 -m pip install --upgrade pip
    ```
    Windows:
    ```bash
    python -m pip install --upgrade pip
    ```
-1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#prerequisites-for-deployment-node).
+1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#prerequisites-for-deployment-node).
 1. Create and activate a [virtual environment](https://realpython.com/python-virtual-environments-a-primer/) if necessary.
 1. Install Kubemarine package.
 
    Linux / MacOS:
    ```bash
    python3 -m pip install kubemarine
    ```
@@ -99,15 +99,15 @@
 1. Now you can proceed to run Kubemarine! Try the following:
    ```bash
    kubemarine help
    ```
 
 
 ## Kubemarine Installation from Sources
-Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.18.0/README.md#kubemarine-package-installation).
+Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.18.1/README.md#kubemarine-package-installation).
 The exception is instead of installing the package from [PyPI](https://pypi.org/project/kubemarine/), do the following:
 1. [Download the latest release](https://github.com/netcracker/kubemarine/releases) or clone the repository:
    ```bash
    git clone https://github.com/netcracker/kubemarine.git
    ```
 1. Unpack the project from the archive if required:
    ```bash
@@ -128,24 +128,24 @@
    python -m pip install -e .
    ```
 1. Now you can proceed to run Kubemarine. Try the following:
     ```bash
     kubemarine help
     ```
 
-**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.18.0/Dockerfile) is also available.
+**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.18.1/Dockerfile) is also available.
 
 
 **Note:** Kubemarine debugging available via `kubemarine/__main__.py`.
 
 
 ## Running Cluster Installation
 To install a Kubernetes cluster using Kubemarine:
-1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
-1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.18.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
+1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#prerequisites-for-cluster-nodes).
+1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.18.1/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
    ```yaml
    node_defaults:
      keyfile: "/home/username/.ssh/id_rsa"
      username: "centos"
 
    vrrp_ips:
      - 192.168.0.250
@@ -173,42 +173,42 @@
    kubemarine install
    ```
 1. Check the health of the newly installed cluster:
    ```bash
    kubemarine check_paas
    ```
 
-For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.18.0/README.md#documentation).
+For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.18.1/README.md#documentation).
 
 ## Kubemarine Docker Installation
 To start, download the Kubmarine image ```docker pull ghcr.io/netcracker/kubemarine:main```
 
 Run Kubemarine from the container, for example:
    ```
    docker run -it --mount type=bind,source=/root/cluster.yaml,target=/opt/kubemarine/cluster.yaml --mount type=bind,source=/root/rsa_key,target=/opt/kubemarine/rsa_key kubemarine install -c /opt/kubemarine/cluster.yaml
    ```
    *Note*: Do not forget to pass the inventory file and connection key inside the container.
    For more execution details, refer to ["Installation of Kubernetes using CLI" guide on Github](https://github.com/Netcracker/kubemarine/blob/main/documentation/Installation.md#installation-of-kubernetes-using-cli).
 
 ## Documentation
 The following documents and tutorials are available:
-- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md)
-- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md)
-- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Troubleshooting.md)
-- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Kubecheck.md)
-- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Logging.md)
+- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md)
+- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md)
+- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Troubleshooting.md)
+- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Kubecheck.md)
+- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Logging.md)
 
 Also, check out the following inventory examples:
-- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.18.0/examples/cluster.yaml)
-- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.18.0/examples/procedure.yaml)
+- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.18.1/examples/cluster.yaml)
+- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.18.1/examples/procedure.yaml)
 
 ## Issues, Questions
 If you have any problems while working with Kubemarine, feel free to open a [new issue](https://github.com/netcracker/kubemarine/issues) or even
 [PR](https://github.com/netcracker/kubemarine/pulls) with related changes.
-Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.18.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
+Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.18.1/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
 
-In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.18.0/SECURITY.md)
+In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.18.1/SECURITY.md)
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/netcracker/kubemarine/releases).
 
 ## License
-[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.18.0/LICENSE)
+[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.18.1/LICENSE)
```

### Comparing `kubemarine-0.18.0/README.md` & `kubemarine-0.18.1/README.md`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/bin/kubemarine` & `kubemarine-0.18.1/bin/kubemarine`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/bin/kubemarine.cmd` & `kubemarine-0.18.1/bin/kubemarine.cmd`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/__init__.py` & `kubemarine-0.18.1/kubemarine/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/__main__.py` & `kubemarine-0.18.1/kubemarine/__main__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/admission.py` & `kubemarine-0.18.1/kubemarine/admission.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/apparmor.py` & `kubemarine-0.18.1/kubemarine/apparmor.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/apt.py` & `kubemarine-0.18.1/kubemarine/apt.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/audit.py` & `kubemarine-0.18.1/kubemarine/audit.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/controlplane.py` & `kubemarine-0.18.1/kubemarine/controlplane.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/core/__init__.py` & `kubemarine-0.18.1/kubemarine/core/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/core/action.py` & `kubemarine-0.18.1/kubemarine/core/action.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/core/annotations.py` & `kubemarine-0.18.1/kubemarine/core/annotations.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/core/cluster.py` & `kubemarine-0.18.1/kubemarine/core/cluster.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/core/connections.py` & `kubemarine-0.18.1/kubemarine/core/connections.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/core/defaults.py` & `kubemarine-0.18.1/kubemarine/core/defaults.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/core/environment.py` & `kubemarine-0.18.1/kubemarine/core/environment.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/core/errors.py` & `kubemarine-0.18.1/kubemarine/core/errors.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/core/executor.py` & `kubemarine-0.18.1/kubemarine/core/executor.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/core/flow.py` & `kubemarine-0.18.1/kubemarine/core/flow.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/core/group.py` & `kubemarine-0.18.1/kubemarine/core/group.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/core/log.py` & `kubemarine-0.18.1/kubemarine/core/log.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/core/os.py` & `kubemarine-0.18.1/kubemarine/core/os.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/core/patch.py` & `kubemarine-0.18.1/kubemarine/core/patch.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/core/resources.py` & `kubemarine-0.18.1/kubemarine/core/resources.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/core/schema.py` & `kubemarine-0.18.1/kubemarine/core/schema.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/core/static.py` & `kubemarine-0.18.1/kubemarine/core/static.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/core/summary.py` & `kubemarine-0.18.1/kubemarine/core/summary.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/core/utils.py` & `kubemarine-0.18.1/kubemarine/core/utils.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/core/yaml_merger.py` & `kubemarine-0.18.1/kubemarine/core/yaml_merger.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/coredns.py` & `kubemarine-0.18.1/kubemarine/coredns.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/cri/__init__.py` & `kubemarine-0.18.1/kubemarine/cri/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/cri/containerd.py` & `kubemarine-0.18.1/kubemarine/cri/containerd.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/cri/docker.py` & `kubemarine-0.18.1/kubemarine/cri/docker.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/demo.py` & `kubemarine-0.18.1/kubemarine/demo.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/etcd.py` & `kubemarine-0.18.1/kubemarine/etcd.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/haproxy.py` & `kubemarine-0.18.1/kubemarine/haproxy.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/jinja.py` & `kubemarine-0.18.1/kubemarine/jinja.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/k8s_certs.py` & `kubemarine-0.18.1/kubemarine/k8s_certs.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/keepalived.py` & `kubemarine-0.18.1/kubemarine/keepalived.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/kubernetes/__init__.py` & `kubemarine-0.18.1/kubemarine/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/kubernetes/daemonset.py` & `kubemarine-0.18.1/kubemarine/kubernetes/daemonset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/kubernetes/deployment.py` & `kubemarine-0.18.1/kubemarine/kubernetes/deployment.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/kubernetes/object.py` & `kubemarine-0.18.1/kubemarine/kubernetes/object.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/kubernetes/replicaset.py` & `kubemarine-0.18.1/kubemarine/kubernetes/replicaset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/kubernetes/statefulset.py` & `kubemarine-0.18.1/kubemarine/kubernetes/statefulset.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/kubernetes_accounts.py` & `kubemarine-0.18.1/kubemarine/kubernetes_accounts.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/packages.py` & `kubemarine-0.18.1/kubemarine/packages.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/patches/__init__.py` & `kubemarine-0.18.1/kubemarine/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/patches/software_upgrade.yaml` & `kubemarine-0.18.1/kubemarine/patches/software_upgrade.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/plugins/__init__.py` & `kubemarine-0.18.1/kubemarine/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/plugins/builtin.py` & `kubemarine-0.18.1/kubemarine/plugins/builtin.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/plugins/calico.py` & `kubemarine-0.18.1/kubemarine/plugins/calico.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/plugins/kubernetes_dashboard.py` & `kubemarine-0.18.1/kubemarine/plugins/kubernetes_dashboard.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/plugins/local_path_provisioner.py` & `kubemarine-0.18.1/kubemarine/plugins/local_path_provisioner.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/plugins/manifest.py` & `kubemarine-0.18.1/kubemarine/plugins/manifest.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/plugins/nginx_ingress.py` & `kubemarine-0.18.1/kubemarine/plugins/nginx_ingress.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml` & `kubemarine-0.18.1/kubemarine/plugins/yaml/calico-v3.22.2-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml` & `kubemarine-0.18.1/kubemarine/plugins/yaml/calico-v3.24.2-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml` & `kubemarine-0.18.1/kubemarine/plugins/yaml/calico-v3.25.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml` & `kubemarine-0.18.1/kubemarine/plugins/yaml/kubernetes-dashboard-v2.5.1-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml` & `kubemarine-0.18.1/kubemarine/plugins/yaml/kubernetes-dashboard-v2.7.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml` & `kubemarine-0.18.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.22-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml` & `kubemarine-0.18.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.23-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml` & `kubemarine-0.18.1/kubemarine/plugins/yaml/local-path-provisioner-v0.0.24-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml` & `kubemarine-0.18.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.2.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml` & `kubemarine-0.18.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.4.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml` & `kubemarine-0.18.1/kubemarine/plugins/yaml/nginx-ingress-controller-v1.7.0-original.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/procedures/__init__.py` & `kubemarine-0.18.1/kubemarine/procedures/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/procedures/add_node.py` & `kubemarine-0.18.1/kubemarine/procedures/add_node.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/procedures/backup.py` & `kubemarine-0.18.1/kubemarine/procedures/backup.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/procedures/cert_renew.py` & `kubemarine-0.18.1/kubemarine/procedures/cert_renew.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/procedures/check_iaas.py` & `kubemarine-0.18.1/kubemarine/procedures/check_iaas.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/procedures/check_paas.py` & `kubemarine-0.18.1/kubemarine/procedures/check_paas.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/procedures/do.py` & `kubemarine-0.18.1/kubemarine/procedures/do.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/procedures/install.py` & `kubemarine-0.18.1/kubemarine/procedures/install.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/procedures/manage_psp.py` & `kubemarine-0.18.1/kubemarine/procedures/manage_psp.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/procedures/manage_pss.py` & `kubemarine-0.18.1/kubemarine/procedures/manage_pss.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/procedures/migrate_cri.py` & `kubemarine-0.18.1/kubemarine/procedures/migrate_cri.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/procedures/migrate_kubemarine.py` & `kubemarine-0.18.1/kubemarine/procedures/migrate_kubemarine.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/procedures/reboot.py` & `kubemarine-0.18.1/kubemarine/procedures/reboot.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/procedures/remove_node.py` & `kubemarine-0.18.1/kubemarine/procedures/remove_node.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/procedures/restore.py` & `kubemarine-0.18.1/kubemarine/procedures/restore.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/procedures/upgrade.py` & `kubemarine-0.18.1/kubemarine/procedures/upgrade.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/__init__.py` & `kubemarine-0.18.1/kubemarine/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/configurations/__init__.py` & `kubemarine-0.18.1/kubemarine/resources/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml` & `kubemarine-0.18.1/kubemarine/resources/configurations/compatibility/internal/kubernetes_images.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,16 @@
     version: v1.21.5
   v1.21.12:
     version: v1.21.12
   v1.22.2:
     version: v1.22.2
   v1.22.9:
     version: v1.22.9
+  v1.23.1:
+    version: v1.23.1
   v1.23.6:
     version: v1.23.6
   v1.23.11:
     version: v1.23.11
   v1.23.17:
     version: v1.23.17
   v1.24.2:
@@ -38,14 +40,16 @@
     version: v1.21.5
   v1.21.12:
     version: v1.21.12
   v1.22.2:
     version: v1.22.2
   v1.22.9:
     version: v1.22.9
+  v1.23.1:
+    version: v1.23.1
   v1.23.6:
     version: v1.23.6
   v1.23.11:
     version: v1.23.11
   v1.23.17:
     version: v1.23.17
   v1.24.2:
@@ -69,14 +73,16 @@
     version: v1.21.5
   v1.21.12:
     version: v1.21.12
   v1.22.2:
     version: v1.22.2
   v1.22.9:
     version: v1.22.9
+  v1.23.1:
+    version: v1.23.1
   v1.23.6:
     version: v1.23.6
   v1.23.11:
     version: v1.23.11
   v1.23.17:
     version: v1.23.17
   v1.24.2:
@@ -100,14 +106,16 @@
     version: v1.21.5
   v1.21.12:
     version: v1.21.12
   v1.22.2:
     version: v1.22.2
   v1.22.9:
     version: v1.22.9
+  v1.23.1:
+    version: v1.23.1
   v1.23.6:
     version: v1.23.6
   v1.23.11:
     version: v1.23.11
   v1.23.17:
     version: v1.23.17
   v1.24.2:
@@ -131,14 +139,16 @@
     version: 3.4.1
   v1.21.12:
     version: 3.4.1
   v1.22.2:
     version: '3.5'
   v1.22.9:
     version: '3.5'
+  v1.23.1:
+    version: '3.6'
   v1.23.6:
     version: '3.6'
   v1.23.11:
     version: '3.6'
   v1.23.17:
     version: '3.6'
   v1.24.2:
@@ -162,14 +172,16 @@
     version: 3.4.13-0
   v1.21.12:
     version: 3.4.13-0
   v1.22.2:
     version: 3.5.0-0
   v1.22.9:
     version: 3.5.0-0
+  v1.23.1:
+    version: 3.5.1-0
   v1.23.6:
     version: 3.5.1-0
   v1.23.11:
     version: 3.5.1-0
   v1.23.17:
     version: 3.5.6-0
   v1.24.2:
@@ -193,14 +205,16 @@
     version: v1.8.0
   v1.21.12:
     version: v1.8.0
   v1.22.2:
     version: v1.8.4
   v1.22.9:
     version: v1.8.4
+  v1.23.1:
+    version: v1.8.6
   v1.23.6:
     version: v1.8.6
   v1.23.11:
     version: v1.8.6
   v1.23.17:
     version: v1.8.6
   v1.24.2:
```

### Comparing `kubemarine-0.18.0/kubemarine/resources/configurations/compatibility/internal/packages.yaml` & `kubemarine-0.18.1/kubemarine/resources/configurations/compatibility/internal/packages.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,18 @@
     version_rhel: 19.03*
     version_rhel8: 19.03*
     version_debian: 5:20.10.*
   v1.22.9:
     version_rhel: 19.03*
     version_rhel8: 19.03*
     version_debian: 5:20.10.*
+  v1.23.1:
+    version_rhel: 19.03*
+    version_rhel8: 19.03*
+    version_debian: 5:20.10.*
   v1.23.6:
     version_rhel: 19.03*
     version_rhel8: 19.03*
     version_debian: 5:20.10.*
   v1.23.11:
     version_rhel: 19.03*
     version_rhel8: 19.03*
@@ -72,14 +76,16 @@
     version_debian: 1.5.*
   v1.21.12:
     version_debian: 1.5.*
   v1.22.2:
     version_debian: 1.5.*
   v1.22.9:
     version_debian: 1.5.*
+  v1.23.1:
+    version_debian: 1.5.*
   v1.23.6:
     version_debian: 1.5.*
   v1.23.11:
     version_debian: 1.5.*
   v1.23.17:
     version_debian: 1.5.*
   v1.24.2:
@@ -113,14 +119,18 @@
     version_rhel: 1.6*
     version_rhel8: 1.6*
     version_debian: 1.5.*
   v1.22.9:
     version_rhel: 1.6*
     version_rhel8: 1.6*
     version_debian: 1.5.*
+  v1.23.1:
+    version_rhel: 1.6*
+    version_rhel8: 1.6*
+    version_debian: 1.5.*
   v1.23.6:
     version_rhel: 1.6*
     version_rhel8: 1.6*
     version_debian: 1.5.*
   v1.23.11:
     version_rhel: 1.6*
     version_rhel8: 1.6*
@@ -174,14 +184,18 @@
     version_rhel: 1.6.4*
     version_rhel8: "*"
     version_debian: "*"
   v1.22.9:
     version_rhel: 1.6.4*
     version_rhel8: "*"
     version_debian: "*"
+  v1.23.1:
+    version_rhel: 1.6.4*
+    version_rhel8: "*"
+    version_debian: "*"
   v1.23.6:
     version_rhel: 1.6.4*
     version_rhel8: "*"
     version_debian: "*"
   v1.23.11:
     version_rhel: 1.6.4*
     version_rhel8: "*"
```

### Comparing `kubemarine-0.18.0/kubemarine/resources/configurations/compatibility/internal/plugins.yaml` & `kubemarine-0.18.1/kubemarine/resources/configurations/compatibility/internal/plugins.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     version: v3.22.2
   v1.21.12:
     version: v3.22.2
   v1.22.2:
     version: v3.24.2
   v1.22.9:
     version: v3.24.2
+  v1.23.1:
+    version: v3.24.2
   v1.23.6:
     version: v3.24.2
   v1.23.11:
     version: v3.24.2
   v1.23.17:
     version: v3.24.2
   v1.24.2:
@@ -47,14 +49,17 @@
     webhook-version: v1.1.1
   v1.22.2:
     version: v1.2.0
     webhook-version: v1.1.1
   v1.22.9:
     version: v1.2.0
     webhook-version: v1.1.1
+  v1.23.1:
+    version: v1.2.0
+    webhook-version: v1.1.1
   v1.23.6:
     version: v1.2.0
     webhook-version: v1.1.1
   v1.23.11:
     version: v1.2.0
     webhook-version: v1.1.1
   v1.23.17:
@@ -93,14 +98,17 @@
     metrics-scraper-version: v1.0.7
   v1.22.2:
     version: v2.5.1
     metrics-scraper-version: v1.0.7
   v1.22.9:
     version: v2.5.1
     metrics-scraper-version: v1.0.7
+  v1.23.1:
+    version: v2.5.1
+    metrics-scraper-version: v1.0.7
   v1.23.6:
     version: v2.5.1
     metrics-scraper-version: v1.0.7
   v1.23.11:
     version: v2.5.1
     metrics-scraper-version: v1.0.7
   v1.23.17:
@@ -139,14 +147,17 @@
     busybox-version: 1.34.1
   v1.22.2:
     version: v0.0.22
     busybox-version: 1.34.1
   v1.22.9:
     version: v0.0.22
     busybox-version: 1.34.1
+  v1.23.1:
+    version: v0.0.22
+    busybox-version: 1.34.1
   v1.23.6:
     version: v0.0.22
     busybox-version: 1.34.1
   v1.23.11:
     version: v0.0.22
     busybox-version: 1.34.1
   v1.23.17:
```

### Comparing `kubemarine-0.18.0/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml` & `kubemarine-0.18.1/kubemarine/resources/configurations/compatibility/internal/thirdparties.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     sha1: 2ee056ac1d0b9c2289bdb03cb7bb0cd21ee29a8b
   v1.21.12:
     sha1: b566840ac2bd50d9c83165ac61331ba7998bf7ce
   v1.22.2:
     sha1: 190703cfe16ad00d0f91487d00bece9667cd5903
   v1.22.9:
     sha1: 33418daedfd3651ebcf5c0ab0c6c701764962e5d
+  v1.23.1:
+    sha1: ac147fd6a951670fe7414cee8b3cb1e6ac1d40d1
   v1.23.6:
     sha1: 90386507b3214adb6b2d4ed05a07e80f11f674d6
   v1.23.11:
     sha1: b93ff384df125429dcbeb18c2ea648168ae10c56
   v1.23.17:
     sha1: 0e805ff79d4099747bdf67d71d8acdc690e07e14
   v1.24.2:
@@ -39,14 +41,16 @@
     sha1: 61da22475b977cb678cca8cf7249bf727d72ee89
   v1.21.12:
     sha1: 45a50b60122f35505ecd08479be1ae232b0ac524
   v1.22.2:
     sha1: 41a2980963427a17c4fbce74aee6bb0bcf08b9ff
   v1.22.9:
     sha1: 21b4104937b65fdf0fdf9fbb57ff22a879b21e3f
+  v1.23.1:
+    sha1: 4a7e2e5f5e6b8e95efa52931786bc275a037bc50
   v1.23.6:
     sha1: 326110dcb62b66e69490d039b170682fb71c5560
   v1.23.11:
     sha1: 07769c846e4a83d59f9f34370c33be5cc163120b
   v1.23.17:
     sha1: 42bce3cef79c9bf2c787e2bcb923ef2528834e96
   v1.24.2:
@@ -70,14 +74,16 @@
     sha1: c4648e31ca16fb00e3826f8ab7c653da81eff367
   v1.21.12:
     sha1: 54a381297eb3a94ab968bb8bfff5f91e3d08805a
   v1.22.2:
     sha1: de9b5c2fe2faefc2b4a61adf6f89144d3f0a09b1
   v1.22.9:
     sha1: e4137d683b9f93211bb6d9fa155d0bb423e871c9
+  v1.23.1:
+    sha1: 4ceb8d046a2d8253495aa86d13f11e2eb29644fc
   v1.23.6:
     sha1: 65a24196b4cc9a3d2eafbd254b9d2d4add8ba152
   v1.23.11:
     sha1: 81643da0b975102cede136d39767cdc54f2b0aef
   v1.23.17:
     sha1: 7377f28047c9c468978199cf5b9e4e7cae0c4e78
   v1.24.2:
@@ -108,14 +114,17 @@
     sha1: b1e2c550480afe4250a34b0e4529eb38ae06973f
   v1.22.2:
     version: v3.24.2
     sha1: c4de7a203e5a3a942fdf130bc9ec180111fc2ab6
   v1.22.9:
     version: v3.24.2
     sha1: c4de7a203e5a3a942fdf130bc9ec180111fc2ab6
+  v1.23.1:
+    version: v3.24.2
+    sha1: c4de7a203e5a3a942fdf130bc9ec180111fc2ab6
   v1.23.6:
     version: v3.24.2
     sha1: c4de7a203e5a3a942fdf130bc9ec180111fc2ab6
   v1.23.11:
     version: v3.24.2
     sha1: c4de7a203e5a3a942fdf130bc9ec180111fc2ab6
   v1.23.17:
@@ -156,14 +165,17 @@
     sha1: 332001091d2e4523cbe8d97ab0f7bfbf4dfebda2
   v1.22.2:
     version: v1.23.0
     sha1: 332001091d2e4523cbe8d97ab0f7bfbf4dfebda2
   v1.22.9:
     version: v1.23.0
     sha1: 332001091d2e4523cbe8d97ab0f7bfbf4dfebda2
+  v1.23.1:
+    version: v1.23.0
+    sha1: 332001091d2e4523cbe8d97ab0f7bfbf4dfebda2
   v1.23.6:
     version: v1.23.0
     sha1: 332001091d2e4523cbe8d97ab0f7bfbf4dfebda2
   v1.23.11:
     version: v1.23.0
     sha1: 332001091d2e4523cbe8d97ab0f7bfbf4dfebda2
   v1.23.17:
```

### Comparing `kubemarine-0.18.0/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml` & `kubemarine-0.18.1/kubemarine/resources/configurations/compatibility/kubernetes_versions.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,20 @@
     crictl: v1.23.0
   v1.22.9:
     calico: v3.24.2
     nginx-ingress-controller: v1.2.0
     kubernetes-dashboard: v2.5.1
     local-path-provisioner: v0.0.22
     crictl: v1.23.0
+  v1.23.1:
+    calico: v3.24.2
+    nginx-ingress-controller: v1.2.0
+    kubernetes-dashboard: v2.5.1
+    local-path-provisioner: v0.0.22
+    crictl: v1.23.0
   v1.23.6:
     calico: v3.24.2
     nginx-ingress-controller: v1.2.0
     kubernetes-dashboard: v2.5.1
     local-path-provisioner: v0.0.22
     crictl: v1.23.0
   v1.23.11:
```

### Comparing `kubemarine-0.18.0/kubemarine/resources/configurations/defaults.yaml` & `kubemarine-0.18.1/kubemarine/resources/configurations/defaults.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/configurations/globals.yaml` & `kubemarine-0.18.1/kubemarine/resources/configurations/globals.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/drop_ins/__init__.py` & `kubemarine-0.18.1/kubemarine/resources/drop_ins/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/etalons/patches/__init__.py` & `kubemarine-0.18.1/kubemarine/resources/etalons/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/etalons/patches/software_upgrade.yaml` & `kubemarine-0.18.1/kubemarine/resources/etalons/patches/software_upgrade.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/psp/__init__.py` & `kubemarine-0.18.1/kubemarine/resources/psp/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/psp/anyuid.yaml` & `kubemarine-0.18.1/kubemarine/resources/psp/anyuid.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/psp/default.yaml` & `kubemarine-0.18.1/kubemarine/resources/psp/default.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/psp/host-network.yaml` & `kubemarine-0.18.1/kubemarine/resources/psp/host-network.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/psp/privileged.yaml` & `kubemarine-0.18.1/kubemarine/resources/psp/privileged.yaml`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/reports/__init__.py` & `kubemarine-0.18.1/kubemarine/resources/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/reports/check_report.css` & `kubemarine-0.18.1/kubemarine/resources/reports/check_report.css`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/add_node.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/add_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/backup.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/backup.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/cert_renew.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/cert_renew.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/cluster.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/cluster.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/common/node_ref.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/common/node_ref.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/common/utils.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/common/utils.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/gateway_node.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/gateway_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/globals.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/globals.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/node.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/node_defaults.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/node_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugin_defaults.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugin_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/calico.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/calico.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/generic_plugin.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/ansible.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/config.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/config.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/expect.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/expect.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/helm.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/helm.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/python.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/python.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/shell.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/shell.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation/template.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation/template.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/installation.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/installation.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/kubernetes-dashboard.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/local-path-provisioner.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins/nginx-ingress-controller.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/plugins.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/plugins.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/procedures.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/procedures.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/rbac/account.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/rbac/account.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/rbac/account_defaults.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/rbac/account_defaults.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/rbac/psp.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/rbac/psp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/rbac/pss.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/rbac/pss.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/rbac.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/rbac.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/registry.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/registry.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/audit.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/audit.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/coredns.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/coredns.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/cri.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/cri.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/etc_hosts.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/etc_hosts.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/kernel_security.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/kernel_security.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/kubeadm.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/kubeadm.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/kubeadm_kubelet.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/kubeadm_patches.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/loadbalancer.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/loadbalancer.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/modprobe.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/modprobe.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/ntp.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/ntp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/packages/associations.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/packages/associations.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/packages.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/packages.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/sysctl.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/sysctl.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services/thirdparties.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services/thirdparties.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/services.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/services.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/definitions/vrrp_ip.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/definitions/vrrp_ip.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/manage_psp.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/manage_psp.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/manage_pss.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/manage_pss.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/migrate_cri.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/migrate_cri.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/migrate_kubemarine.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/migrate_kubemarine.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/reboot.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/reboot.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/remove_node.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/remove_node.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/restore.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/restore.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/schemas/upgrade.json` & `kubemarine-0.18.1/kubemarine/resources/schemas/upgrade.json`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/scripts/__init__.py` & `kubemarine-0.18.1/kubemarine/resources/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/scripts/check_url_availability.py` & `kubemarine-0.18.1/kubemarine/resources/scripts/check_url_availability.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/scripts/etcdctl.sh` & `kubemarine-0.18.1/kubemarine/resources/scripts/etcdctl.sh`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/resources/scripts/simple_tcp_listener.py` & `kubemarine-0.18.1/kubemarine/resources/scripts/simple_tcp_listener.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/selinux.py` & `kubemarine-0.18.1/kubemarine/selinux.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/sysctl.py` & `kubemarine-0.18.1/kubemarine/sysctl.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/system.py` & `kubemarine-0.18.1/kubemarine/system.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/templates/__init__.py` & `kubemarine-0.18.1/kubemarine/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/templates/admission.yaml.j2` & `kubemarine-0.18.1/kubemarine/templates/admission.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/templates/haproxy.cfg.j2` & `kubemarine-0.18.1/kubemarine/templates/haproxy.cfg.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/templates/keepalived.conf.j2` & `kubemarine-0.18.1/kubemarine/templates/keepalived.conf.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/templates/kubelet.service.j2` & `kubemarine-0.18.1/kubemarine/templates/kubelet.service.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/templates/plugins/__init__.py` & `kubemarine-0.18.1/kubemarine/templates/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/templates/plugins/calico-ippool.yaml.j2` & `kubemarine-0.18.1/kubemarine/templates/plugins/calico-ippool.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/templates/plugins/calico-rr.yaml.j2` & `kubemarine-0.18.1/kubemarine/templates/plugins/calico-rr.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2` & `kubemarine-0.18.1/kubemarine/templates/plugins/dashboard-v2.5.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2` & `kubemarine-0.18.1/kubemarine/templates/plugins/dashboard-v2.7.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/templates/plugins/iperf3.yaml.j2` & `kubemarine-0.18.1/kubemarine/templates/plugins/iperf3.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/templates/plugins/local-path-provisioner.yaml.j2` & `kubemarine-0.18.1/kubemarine/templates/plugins/local-path-provisioner.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2` & `kubemarine-0.18.1/kubemarine/templates/plugins/nginx-ingress-controller-v1.2.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2` & `kubemarine-0.18.1/kubemarine/templates/plugins/nginx-ingress-controller-v1.4.yaml.j2`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/testsuite.py` & `kubemarine-0.18.1/kubemarine/testsuite.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/thirdparties.py` & `kubemarine-0.18.1/kubemarine/thirdparties.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine/yum.py` & `kubemarine-0.18.1/kubemarine/yum.py`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/kubemarine.egg-info/PKG-INFO` & `kubemarine-0.18.1/kubemarine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubemarine
-Version: 0.18.0
+Version: 0.18.1
 Summary: Management tool for Kubernetes cluster deployment and maintenance
 Home-page: https://github.com/Netcracker/KubeMarine
 Author-email: Kubemarine Group <kubemarinegroup@netcracker.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Netcracker/KubeMarine
 Project-URL: Documentation, https://github.com/Netcracker/KubeMarine#documentation
 Project-URL: Issues, https://github.com/Netcracker/KubeMarine/issues/
@@ -33,36 +33,36 @@
 # Kubemarine
 
 Kubemarine is an open source, lightweight and powerful management tool built for end-to-end Kubernetes cluster deployment and maintenance. It is applicable for many purposes like simple and quick onboarding Kubernetes on local and production environments in different HA schemes depending on your aims, budget, and capabilities. Together with simplicity, Kubemarine can be a very flexible and customizable tool covering specific configurability cases on both deployment and maintenance stages. This library provides powerful CLI commands, as well as can be customized using a Python extension API.
 
 ## Highlights
 - Easy to use
 - Many procedures supported:
-  - [install](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#)
-  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#add-node-procedure)
-  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#remove-node-procedure)
-  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#upgrade-procedure)
-  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#backup-procedure)
-  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#restore-procedure)
-  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Kubecheck.md#iaas-procedure)
-  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Kubecheck.md#paas-procedure)
-  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#kubemarine-migration-procedure)
-  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#manage-psp-procedure)
-  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#manage-pss-procedure)
-  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#certificate-renew-procedure)
-  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md#migration-cri-procedure)
-- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#configuration) for all operations, highly customizable
+  - [install](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#)
+  - [add_node](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#add-node-procedure)
+  - [remove_node](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#remove-node-procedure)
+  - [upgrade](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#upgrade-procedure)
+  - [backup](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#backup-procedure)
+  - [restore](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#restore-procedure)
+  - [check_iaas](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Kubecheck.md#iaas-procedure)
+  - [check_paas](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Kubecheck.md#paas-procedure)
+  - [migrate_kubemarine](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#kubemarine-migration-procedure)
+  - [manage_psp](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#manage-psp-procedure)
+  - [manage_pss](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#manage-pss-procedure)
+  - [cert_renew](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#certificate-renew-procedure)
+  - [migrate_cri](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md#migration-cri-procedure)
+- [Single cluster inventory](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#configuration) for all operations, highly customizable
 - Default values of all parameters in configurations with a minimum of required parameters
-- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
-- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
-- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#custom-plugins-installation-procedures) support
-- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#installation-without-internet-resources) with private registries
-- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#dump-files)
+- [Control planes balancing](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#full-ha-scheme) with external balancers and VRRP
+- Ability to [resume or skip specific task](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#tasks-list-redefinition) without re-running entire pipeline
+- [Pre-built plugins](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#predefined-plugins) out of the box and [custom plugins](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#custom-plugins-installation-procedures) support
+- Support for [executing in closed environments](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#installation-without-internet-resources) with private registries
+- Extended [logging](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Logging.md), configs [dumping](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#dump-files)
 - Build supported as a package, container, and binary
-- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/PackageExtension.md)
+- Package extension with [open extension API](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/PackageExtension.md)
 - Support different deployment schemes (all-in-one, mini-HA, HA, and so on)
 
 ## Kubemarine Binary Installation
 Proceed the following steps to install Kubemarine  on your environment:
 1. Download the binary file for your system from the latest [release](https://github.com/Netcracker/KubeMarine/releases)
 2. Move binary kubemarine to a separate folder 
 3. Now you can proceed to run Kubemarine! Try the following:
@@ -80,15 +80,15 @@
    ```bash
    python3 -m pip install --upgrade pip
    ```
    Windows:
    ```bash
    python -m pip install --upgrade pip
    ```
-1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#prerequisites-for-deployment-node).
+1. Ensure your environment meets the [Deployment Node Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#prerequisites-for-deployment-node).
 1. Create and activate a [virtual environment](https://realpython.com/python-virtual-environments-a-primer/) if necessary.
 1. Install Kubemarine package.
 
    Linux / MacOS:
    ```bash
    python3 -m pip install kubemarine
    ```
@@ -99,15 +99,15 @@
 1. Now you can proceed to run Kubemarine! Try the following:
    ```bash
    kubemarine help
    ```
 
 
 ## Kubemarine Installation from Sources
-Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.18.0/README.md#kubemarine-package-installation).
+Installation of Kubemarine from sources is mostly similar to [Kubemarine Package Installation](https://github.com/Netcracker/KubeMarine/blob/0.18.1/README.md#kubemarine-package-installation).
 The exception is instead of installing the package from [PyPI](https://pypi.org/project/kubemarine/), do the following:
 1. [Download the latest release](https://github.com/netcracker/kubemarine/releases) or clone the repository:
    ```bash
    git clone https://github.com/netcracker/kubemarine.git
    ```
 1. Unpack the project from the archive if required:
    ```bash
@@ -128,24 +128,24 @@
    python -m pip install -e .
    ```
 1. Now you can proceed to run Kubemarine. Try the following:
     ```bash
     kubemarine help
     ```
 
-**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.18.0/Dockerfile) is also available.
+**Note**: Building from [Dockerfile](https://github.com/Netcracker/KubeMarine/blob/0.18.1/Dockerfile) is also available.
 
 
 **Note:** Kubemarine debugging available via `kubemarine/__main__.py`.
 
 
 ## Running Cluster Installation
 To install a Kubernetes cluster using Kubemarine:
-1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#prerequisites-for-cluster-nodes).
-1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.18.0/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
+1. Prepare your VMs or bare-metal machines according to [Recommended Hardware Requirements](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#recommended-hardware-requirements) and the selected [Deployment Scheme](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#deployment-schemes). Make sure the nodes meet [Cluster Nodes Prerequisites](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#prerequisites-for-cluster-nodes).
+1. Create the `cluster.yaml` inventory file, and describe your environment. Make sure that all configurations are done. For more information, see [inventory configs available](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md#configuration) and [examples](https://github.com/Netcracker/KubeMarine/blob/0.18.1/examples/cluster.yaml). No need to enter all the parameters that are available, it is enough to specify the minimal identification data about the nodes where you want to install the cluster, for example:
    ```yaml
    node_defaults:
      keyfile: "/home/username/.ssh/id_rsa"
      username: "centos"
 
    vrrp_ips:
      - 192.168.0.250
@@ -173,42 +173,42 @@
    kubemarine install
    ```
 1. Check the health of the newly installed cluster:
    ```bash
    kubemarine check_paas
    ```
 
-For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.18.0/README.md#documentation).
+For more information, refer to the other [Kubemarine guides](https://github.com/Netcracker/KubeMarine/blob/0.18.1/README.md#documentation).
 
 ## Kubemarine Docker Installation
 To start, download the Kubmarine image ```docker pull ghcr.io/netcracker/kubemarine:main```
 
 Run Kubemarine from the container, for example:
    ```
    docker run -it --mount type=bind,source=/root/cluster.yaml,target=/opt/kubemarine/cluster.yaml --mount type=bind,source=/root/rsa_key,target=/opt/kubemarine/rsa_key kubemarine install -c /opt/kubemarine/cluster.yaml
    ```
    *Note*: Do not forget to pass the inventory file and connection key inside the container.
    For more execution details, refer to ["Installation of Kubernetes using CLI" guide on Github](https://github.com/Netcracker/kubemarine/blob/main/documentation/Installation.md#installation-of-kubernetes-using-cli).
 
 ## Documentation
 The following documents and tutorials are available:
-- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Installation.md)
-- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Maintenance.md)
-- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Troubleshooting.md)
-- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Kubecheck.md)
-- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.18.0/documentation/Logging.md)
+- [Installation](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Installation.md)
+- [Maintenance](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Maintenance.md)
+- [Troubleshooting](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Troubleshooting.md)
+- [Kubecheck](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Kubecheck.md)
+- [Logging](https://github.com/Netcracker/KubeMarine/blob/0.18.1/documentation/Logging.md)
 
 Also, check out the following inventory examples:
-- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.18.0/examples/cluster.yaml)
-- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.18.0/examples/procedure.yaml)
+- [cluster.yaml](https://github.com/Netcracker/KubeMarine/blob/0.18.1/examples/cluster.yaml)
+- [procedure.yaml](https://github.com/Netcracker/KubeMarine/blob/0.18.1/examples/procedure.yaml)
 
 ## Issues, Questions
 If you have any problems while working with Kubemarine, feel free to open a [new issue](https://github.com/netcracker/kubemarine/issues) or even
 [PR](https://github.com/netcracker/kubemarine/pulls) with related changes.
-Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.18.0/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
+Please follow the [Contribution Guide](https://github.com/Netcracker/KubeMarine/blob/0.18.1/CONTRIBUTING.md ) and the process outlined in the Stack Overflow [MCVE](https://stackoverflow.com/help/mcve) document.
 
-In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.18.0/SECURITY.md)
+In case of security concerns, please follow the [Security Reporting Process](https://github.com/Netcracker/KubeMarine/blob/0.18.1/SECURITY.md)
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/netcracker/kubemarine/releases).
 
 ## License
-[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.18.0/LICENSE)
+[Apache License 2.0](https://github.com/Netcracker/KubeMarine/blob/0.18.1/LICENSE)
```

### Comparing `kubemarine-0.18.0/kubemarine.egg-info/SOURCES.txt` & `kubemarine-0.18.1/kubemarine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kubemarine-0.18.0/pyproject.toml` & `kubemarine-0.18.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 Documentation = "https://github.com/Netcracker/KubeMarine#documentation"
 Issues = "https://github.com/Netcracker/KubeMarine/issues/"
 
 # To change version with automatic push and triggering of the release workflow use
 # 1. pip install bumpver
 # 2. bumpver update --set-version <new version>
 [tool.bumpver]
-current_version = "0.18.0"
+current_version = "0.18.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version to {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `kubemarine-0.18.0/setup.py` & `kubemarine-0.18.1/setup.py`

 * *Files identical despite different names*

