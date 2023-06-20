# Comparing `tmp/netbox_plugin_prometheus_sd-0.6.3.tar.gz` & `tmp/netbox_plugin_prometheus_sd-0.7.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_plugin_prometheus_sd-0.6.3.tar", max compression
+gzip compressed data, was "netbox_plugin_prometheus_sd-0.7.0rc1.tar", max compression
```

## Comparing `netbox_plugin_prometheus_sd-0.6.3.tar` & `netbox_plugin_prometheus_sd-0.7.0rc1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1069 2023-04-12 09:59:26.361881 netbox_plugin_prometheus_sd-0.6.3/LICENSE
--rw-r--r--   0        0        0     3918 2023-04-12 09:59:26.361881 netbox_plugin_prometheus_sd-0.6.3/README.md
--rw-r--r--   0        0        0      488 2023-04-12 09:59:26.365882 netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/__init__.py
--rw-r--r--   0        0        0        0 2023-04-12 09:59:26.365882 netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/api/__init__.py
--rw-r--r--   0        0        0     3891 2023-04-12 09:59:26.365882 netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/api/serializers.py
--rw-r--r--   0        0        0      321 2023-04-12 09:59:26.365882 netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/api/urls.py
--rw-r--r--   0        0        0     4005 2023-04-12 09:59:26.365882 netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/api/utils.py
--rw-r--r--   0        0        0     2545 2023-04-12 09:59:26.365882 netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/api/views.py
--rw-r--r--   0        0        0       50 2023-04-12 09:59:26.365882 netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/tests/__init__.py
--rw-r--r--   0        0        0     2764 2023-04-12 09:59:26.365882 netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/tests/test_api.py
--rwxr-xr-x   0        0        0     8825 2023-04-12 09:59:26.365882 netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/tests/test_serializers.py
--rw-r--r--   0        0        0     3817 2023-04-12 09:59:26.365882 netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/tests/utils.py
--rw-r--r--   0        0        0      617 2023-04-12 09:59:41.394267 netbox_plugin_prometheus_sd-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     4523 1970-01-01 00:00:00.000000 netbox_plugin_prometheus_sd-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-20 08:59:14.242869 netbox_plugin_prometheus_sd-0.7.0rc1/LICENSE
+-rw-r--r--   0        0        0     4788 2023-06-20 08:59:14.242869 netbox_plugin_prometheus_sd-0.7.0rc1/README.md
+-rw-r--r--   0        0        0      488 2023-06-20 08:59:14.246870 netbox_plugin_prometheus_sd-0.7.0rc1/netbox_prometheus_sd/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 08:59:14.246870 netbox_plugin_prometheus_sd-0.7.0rc1/netbox_prometheus_sd/api/__init__.py
+-rw-r--r--   0        0        0     6098 2023-06-20 08:59:14.246870 netbox_plugin_prometheus_sd-0.7.0rc1/netbox_prometheus_sd/api/serializers.py
+-rw-r--r--   0        0        0      321 2023-06-20 08:59:14.246870 netbox_plugin_prometheus_sd-0.7.0rc1/netbox_prometheus_sd/api/urls.py
+-rw-r--r--   0        0        0     4440 2023-06-20 08:59:14.246870 netbox_plugin_prometheus_sd-0.7.0rc1/netbox_prometheus_sd/api/utils.py
+-rw-r--r--   0        0        0     2888 2023-06-20 08:59:14.246870 netbox_plugin_prometheus_sd-0.7.0rc1/netbox_prometheus_sd/api/views.py
+-rw-r--r--   0        0        0       50 2023-06-20 08:59:14.246870 netbox_plugin_prometheus_sd-0.7.0rc1/netbox_prometheus_sd/tests/__init__.py
+-rw-r--r--   0        0        0     2862 2023-06-20 08:59:14.246870 netbox_plugin_prometheus_sd-0.7.0rc1/netbox_prometheus_sd/tests/test_api.py
+-rwxr-xr-x   0        0        0    10872 2023-06-20 08:59:14.246870 netbox_plugin_prometheus_sd-0.7.0rc1/netbox_prometheus_sd/tests/test_serializers.py
+-rw-r--r--   0        0        0     6439 2023-06-20 08:59:14.246870 netbox_plugin_prometheus_sd-0.7.0rc1/netbox_prometheus_sd/tests/utils.py
+-rw-r--r--   0        0        0      620 2023-06-20 08:59:27.563092 netbox_plugin_prometheus_sd-0.7.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     5396 1970-01-01 00:00:00.000000 netbox_plugin_prometheus_sd-0.7.0rc1/PKG-INFO
```

### Comparing `netbox_plugin_prometheus_sd-0.6.3/LICENSE` & `netbox_plugin_prometheus_sd-0.7.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_plugin_prometheus_sd-0.6.3/README.md` & `netbox_plugin_prometheus_sd-0.7.0rc1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 Provide Prometheus http_sd compatible API Endpoint with data from Netbox.
 
 HTTP SD is a new feature in Prometheus 2.28.0 that allows hosts to be found via a URL instead of just files.
 This plugin implements API endpoints in Netbox to make devices, IPs and virtual machines available to Prometheus.
 
 ## Compatibility
 
-We aim to support the latest major versions of Netbox. For now we Support Netbox `2.11`, `3.0`, `3.1`, `3.2` and `3.3` including bugfix versions.
+We aim to support the latest major versions of Netbox. For now we Support Netbox `3.2`, `3.3`, `3.4` and `3.5` including bugfix versions.
+Check the `.github/workflows/ci.yml` pipeline for the current tested builds. Other versions may work, but we do not test them explicitly.
 All relevant target versions are tested in CI. Have a look at the Github Actions definition for the current build targets.
 
 ## Installation
 
 The plugin is available as a Python package in pypi and can be installed with pip
 
     pip install netbox-plugin-prometheus-sd
@@ -41,14 +42,39 @@
 
 ```
 GET        /api/plugins/prometheus-sd/devices/              Get a list of devices in a prometheus compatible format
 GET        /api/plugins/prometheus-sd/virtual-machines/     Get a list of vms in a prometheus compatible format
 GET        /api/plugins/prometheus-sd/ip-addresses/         Get a list of ip in a prometheus compatible format
 ```
 
+### Config context
+
+The plugin can also discover extra config to inject in the HTTP SD JSON from the config context of the devices/virtual machines.
+If you have a `prometheus-plugin-prometheus-sd` entry in your config context with the following schema it will be automatically picked up:
+
+```
+prometheus-plugin-prometheus-sd:
+  - metrics_path: /not/metrics
+    port: 4242
+    scheme: https
+  - port: 4243
+```
+
+This allow you to configure those values directly into netbox instead of doing that inside the Prometheus
+config and filtering each scenario by a specific tag for instance.
+
+If there is only one entry you can also use this form:
+
+```
+prometheus-plugin-prometheus-sd:
+  metrics_path: /not/metrics
+  port: 4242
+  scheme: https
+```
+
 ### Example
 
 A working example on how to use this plugin with Prometheus is located at the `example` folder. Netbox content is created by using Netbox docker initializers.
 
 The demo data doesn't make sense, but they are good enough for demonstrating how to configure Prometheus and get demo data to Prometheus service discovery.
 
 Go to the `example` folder and run `docker-compose up`. Prometheus should get available on `http://localhost:9090`.
```

### Comparing `netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/api/views.py` & `netbox_plugin_prometheus_sd-0.7.0rc1/netbox_prometheus_sd/api/views.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 from ipam.models import IPAddress
 from virtualization.models import VirtualMachine
 from dcim.models.devices import Device
 
-# The base ViewSet has been renamed, this try-except helps to support
-# Both < 3.2 and the newer 3.2+ Versions:
-# https://github.com/netbox-community/netbox/commit/bbdeae0ed9bcc06fb96ffa2970272e1a3447448c
-try:
-    from netbox.api.viewsets import NetBoxModelViewSet
+# pylint: disable=ungrouped-imports
+try:  # Netbox >= 3.5
+    from netbox.api.viewsets import BaseViewSet
+    from netbox.api.viewsets.mixins import CustomFieldsMixin
+    from rest_framework.mixins import ListModelMixin
+    # Netbox MosdelViewSet with list only
+    class NetboxPrometheusSDModelViewSet( # pylint: disable=too-many-ancestors
+        CustomFieldsMixin,
+        ListModelMixin,
+        BaseViewSet):
+        pass
 except ImportError:
-    from extras.api.views import CustomFieldModelViewSet as NetBoxModelViewSet
+    try: #  3.2 >= Netbox < 3.5
+        from netbox.api.viewsets import NetBoxModelViewSet as NetboxPrometheusSDModelViewSet
+    except ImportError: # Netbox < 3.2
+        from extras.api.views import CustomFieldModelViewSet as NetboxPrometheusSDModelViewSet
 
 # Filtersets have been renamed, we support both
 # https://github.com/netbox-community/netbox/commit/1024782b9e0abb48f6da65f8248741227d53dbed#diff-d9224204dab475bbe888868c02235b8ef10f07c9201c45c90804d395dc161c40
-# pylint: disable=ungrouped-imports
 try:
     from ipam.filtersets import IPAddressFilterSet
     from dcim.filtersets import DeviceFilterSet
     from virtualization.filtersets import VirtualMachineFilterSet
 except ImportError:
     from ipam.filters import IPAddressFilterSet
     from dcim.filters import DeviceFilterSet
@@ -27,16 +35,17 @@
 from .serializers import (
     PrometheusIPAddressSerializer,
     PrometheusDeviceSerializer,
     PrometheusVirtualMachineSerializer,
 )
 
 
+
 class VirtualMachineViewSet(
-    NetBoxModelViewSet
+    NetboxPrometheusSDModelViewSet
 ):  # pylint: disable=too-many-ancestors
     queryset = VirtualMachine.objects.prefetch_related(
         "cluster__site",
         "role",
         "tenant",
         "platform",
         "primary_ip4",
@@ -47,15 +56,15 @@
 
     )
     filterset_class = VirtualMachineFilterSet
     serializer_class = PrometheusVirtualMachineSerializer
     pagination_class = None
 
 
-class DeviceViewSet(NetBoxModelViewSet):  # pylint: disable=too-many-ancestors
+class DeviceViewSet(NetboxPrometheusSDModelViewSet):  # pylint: disable=too-many-ancestors
     queryset = Device.objects.prefetch_related(
         "device_type__manufacturer",
         "device_role",
         "tenant",
         "platform",
         "site",
         "location",
@@ -67,12 +76,12 @@
         "tags",
     )
     filterset_class = DeviceFilterSet
     serializer_class = PrometheusDeviceSerializer
     pagination_class = None
 
 
-class IPAddressViewSet(NetBoxModelViewSet):  # pylint: disable=too-many-ancestors
+class IPAddressViewSet(NetboxPrometheusSDModelViewSet):  # pylint: disable=too-many-ancestors
     queryset = IPAddress.objects.prefetch_related("tenant", "tags")
     serializer_class = PrometheusIPAddressSerializer
     filterset_class = IPAddressFilterSet
     pagination_class = None
```

### Comparing `netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/tests/test_api.py` & `netbox_plugin_prometheus_sd-0.7.0rc1/netbox_prometheus_sd/tests/test_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,15 +57,16 @@
 
         resp = self.client.get("/api/plugins/prometheus-sd/virtual-machines/")
         self.assertEqual(resp.status_code, status.HTTP_200_OK)
         data = json.loads(resp.content)
 
         self.assertIsNotNone(data[0]["targets"])
         self.assertIsNotNone(data[0]["labels"])
-        self.assertEqual(len(data), 60)
+        # Full vm contains two entry in the config context so we have to double the number of vm
+        self.assertEqual(len(data), 120)
 
     def test_endpoint_ip_address(self):
         """Ensure ip address endpoint returns a valid response"""
 
         for i in range(60):
             utils.build_full_ip(address=f"10.10.10.{i}/24")
```

### Comparing `netbox_plugin_prometheus_sd-0.6.3/netbox_prometheus_sd/tests/test_serializers.py` & `netbox_plugin_prometheus_sd-0.7.0rc1/netbox_prometheus_sd/tests/test_serializers.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from . import utils
 
 
 class PrometheusVirtualMachineSerializerTests(TestCase):
     def test_vm_minimal_to_target(self):
 
         instance = utils.build_minimal_vm("vm-01.example.com")
-        data = PrometheusVirtualMachineSerializer(instance=instance).data
+        data = PrometheusVirtualMachineSerializer(many=True, instance=[instance]).data[0]
 
         self.assertEqual(data["targets"], ["vm-01.example.com"])
         self.assertDictContainsSubset({"__meta_netbox_id": str(instance.id)}, data["labels"])
         self.assertDictContainsSubset(
             {"__meta_netbox_model": "VirtualMachine"}, data["labels"]
         )
         self.assertDictContainsSubset(
@@ -28,90 +28,101 @@
         )
         self.assertDictContainsSubset(
             {"__meta_netbox_cluster_type": "On Prem"}, data["labels"]
         )
 
     def test_vm_full_to_target(self):
         instance = utils.build_vm_full("vm-full-01.example.com")
-        data = PrometheusVirtualMachineSerializer(instance=instance).data
+        data_list = PrometheusVirtualMachineSerializer(many=True, instance=[instance]).data
 
-        self.assertEqual(data["targets"], ["vm-full-01.example.com"])
-        self.assertDictContainsSubset({"__meta_netbox_id": str(instance.id)}, data["labels"])
-        self.assertDictContainsSubset(
-            {"__meta_netbox_model": "VirtualMachine"}, data["labels"]
-        )
-        self.assertDictContainsSubset(
-            {"__meta_netbox_status": "active"}, data["labels"]
-        )
-        self.assertDictContainsSubset(
-            {"__meta_netbox_tenant": "Acme Corp."}, data["labels"]
-        )
-        self.assertDictContainsSubset(
-            {"__meta_netbox_tenant_slug": "acme"}, data["labels"]
-        )
-        self.assertDictContainsSubset(
-            {"__meta_netbox_site": "Campus A"}, data["labels"]
-        )
-        self.assertDictContainsSubset(
-            {"__meta_netbox_site_slug": "campus-a"}, data["labels"]
-        )
-        self.assertDictContainsSubset({"__meta_netbox_role": "VM"}, data["labels"])
-        self.assertDictContainsSubset({"__meta_netbox_role_slug": "vm"}, data["labels"])
-        self.assertDictContainsSubset(
-            {"__meta_netbox_platform": "Ubuntu 20.04"}, data["labels"]
-        )
-        self.assertDictContainsSubset(
-            {"__meta_netbox_platform_slug": "ubuntu-20.04"}, data["labels"]
-        )
-        self.assertDictContainsSubset(
-            {"__meta_netbox_primary_ip": "2001:db8:1701::2"}, data["labels"]
-        )
-        self.assertDictContainsSubset(
-            {"__meta_netbox_primary_ip4": "192.168.0.1"}, data["labels"]
-        )
+        self.assertEqual(data_list[0]["targets"], ["vm-full-01.example.com:4242"])
         self.assertDictContainsSubset(
-            {"__meta_netbox_primary_ip6": "2001:db8:1701::2"}, data["labels"]
+            {"__metrics__path__": "/not/metrics"}, data_list[0]["labels"]
         )
         self.assertDictContainsSubset(
-            {"__meta_netbox_custom_field_simple": "Foobar 123"}, data["labels"]
-        )
-        self.assertDictContainsSubset(
-            {"__meta_netbox_custom_field_int": "42"}, data["labels"]
-        )
-        self.assertDictContainsSubset(
-            {"__meta_netbox_custom_field_bool": "True"}, data["labels"]
-        )
-        self.assertDictContainsSubset(
-            {"__meta_netbox_custom_field_json": "{'foo': ['bar', 'baz']}"},
-            data["labels"],
-        )
-        self.assertDictContainsSubset(
-            {"__meta_netbox_custom_field_multi_selection": "['foo', 'baz']"},
-            data["labels"],
-        )
-        self.assertDictContainsSubset(
-            {
-                "__meta_netbox_custom_field_contact":
-                "[{'id': 1, 'url': 'http://localhost:8000/api/tenancy/contacts/1/', 'display': 'Foo', 'name': 'Foo'}]"
-            },
-            data["labels"],
-        )
-        self.assertDictContainsSubset(
-            {
-                "__meta_netbox_custom_field_text_long": "This is\r\na  pretty\r\nlog\r\nText"
-            },
-            data["labels"],
+            {"__scheme__": "https"}, data_list[0]["labels"]
         )
+        self.assertEqual(data_list[0]["targets"], ["vm-full-01.example.com:4242"])
+
+        self.assertEqual(data_list[1]["targets"], ["vm-full-01.example.com:4243"])
+        for data in data_list:
+            self.assertDictContainsSubset({"__meta_netbox_id": str(instance.id)}, data["labels"])
+            self.assertDictContainsSubset(
+                {"__meta_netbox_model": "VirtualMachine"}, data["labels"]
+            )
+            self.assertDictContainsSubset(
+                {"__meta_netbox_status": "active"}, data["labels"]
+            )
+            self.assertDictContainsSubset(
+                {"__meta_netbox_tenant": "Acme Corp."}, data["labels"]
+            )
+            self.assertDictContainsSubset(
+                {"__meta_netbox_tenant_slug": "acme"}, data["labels"]
+            )
+            self.assertDictContainsSubset(
+                {"__meta_netbox_site": "Campus A"}, data["labels"]
+            )
+            self.assertDictContainsSubset(
+                {"__meta_netbox_site_slug": "campus-a"}, data["labels"]
+            )
+            self.assertDictContainsSubset({"__meta_netbox_role": "VM"}, data["labels"])
+            self.assertDictContainsSubset({"__meta_netbox_role_slug": "vm"}, data["labels"])
+            self.assertDictContainsSubset(
+                {"__meta_netbox_platform": "Ubuntu 20.04"}, data["labels"]
+            )
+            self.assertDictContainsSubset(
+                {"__meta_netbox_platform_slug": "ubuntu-20.04"}, data["labels"]
+            )
+            self.assertDictContainsSubset(
+                {"__meta_netbox_primary_ip": "2001:db8:1701::2"}, data["labels"]
+            )
+            self.assertDictContainsSubset(
+                {"__meta_netbox_primary_ip4": "192.168.0.1"}, data["labels"]
+            )
+            self.assertDictContainsSubset(
+                {"__meta_netbox_primary_ip6": "2001:db8:1701::2"}, data["labels"]
+            )
+            self.assertDictContainsSubset(
+                {"__meta_netbox_custom_field_simple": "Foobar 123"}, data["labels"]
+            )
+            self.assertDictContainsSubset(
+                {"__meta_netbox_custom_field_int": "42"}, data["labels"]
+            )
+            self.assertDictContainsSubset(
+                {"__meta_netbox_custom_field_bool": "True"}, data["labels"]
+            )
+            self.assertDictContainsSubset(
+                {"__meta_netbox_custom_field_json": "{'foo': ['bar', 'baz']}"},
+                data["labels"],
+            )
+            self.assertDictContainsSubset(
+                {"__meta_netbox_custom_field_multi_selection": "['foo', 'baz']"},
+                data["labels"],
+            )
+            self.assertDictContainsSubset(
+                {
+                    "__meta_netbox_custom_field_contact":
+                    "[{'id': 1, 'url': 'http://localhost:8000/api/tenancy/contacts/1/',"
+                        + " 'display': 'Foo', 'name': 'Foo'}]"
+                },
+                data["labels"],
+            )
+            self.assertDictContainsSubset(
+                {
+                    "__meta_netbox_custom_field_text_long":
+                    "This is\r\na  pretty\r\nlog\r\nText"
+                },
+                data["labels"],
+            )
 
 
 class PrometheusDeviceSerializerTests(TestCase):
     def test_device_minimal_to_target(self):
-
         instance = utils.build_minimal_device("firewall-01")
-        data = PrometheusDeviceSerializer(instance=instance).data
+        data = PrometheusDeviceSerializer(many=True, instance=[instance]).data[0]
 
         self.assertEqual(data["targets"], ["firewall-01"])
         self.assertDictContainsSubset({"__meta_netbox_id": str(instance.id)}, data["labels"])
         self.assertDictContainsSubset({"__meta_netbox_model": "Device"}, data["labels"])
         self.assertDictContainsSubset(
             {"__meta_netbox_role": "Firewall"}, data["labels"]
         )
@@ -125,17 +136,41 @@
             {"__meta_netbox_device_type_slug": "srx"}, data["labels"]
         )
         self.assertDictContainsSubset({"__meta_netbox_site": "Site"}, data["labels"])
         self.assertDictContainsSubset(
             {"__meta_netbox_site_slug": "site"}, data["labels"]
         )
 
+    def test_device_config_context_no_array(self):
+        instance = utils.build_device_config_context_no_array("firewall-no-array-01")
+        data = PrometheusDeviceSerializer(many=True, instance=[instance]).data[0]
+
+        self.assertEqual(data["targets"], ["firewall-no-array-01:4242"])
+
+    def test_device_config_context_invalid_1(self):
+        instance = utils.build_device_config_context_invalid_1("firewall-invalid-01")
+        data = PrometheusDeviceSerializer(many=True, instance=[instance]).data[0]
+
+        self.assertEqual(data["targets"], ["firewall-invalid-01"])
+
+    def test_device_config_context_invalid_2(self):
+        instance = utils.build_device_config_context_invalid_2("firewall-invalid-02")
+        data = PrometheusDeviceSerializer(many=True, instance=[instance]).data[0]
+
+        self.assertEqual(data["targets"], ["firewall-invalid-02"])
+
+    def test_device_config_context_mix_valid_invalid(self):
+        instance = utils.build_device_config_context_mix_invalid_valid("firewall-valid-invalid-01")
+        data = PrometheusDeviceSerializer(many=True, instance=[instance]).data[0]
+
+        self.assertEqual(data["targets"], ["firewall-valid-invalid-01:4242"])
+
     def test_device_full_to_target(self):
         instance = utils.build_device_full("firewall-full-01")
-        data = PrometheusDeviceSerializer(instance=instance).data
+        data = PrometheusDeviceSerializer(many=True, instance=[instance]).data[0]
 
         self.assertEqual(data["targets"], ["firewall-full-01"])
         self.assertDictContainsSubset({"__meta_netbox_id": str(instance.id)}, data["labels"])
         self.assertDictContainsSubset({"__meta_netbox_model": "Device"}, data["labels"])
         self.assertDictContainsSubset(
             {"__meta_netbox_platform": "Junos"}, data["labels"]
         )
@@ -162,30 +197,30 @@
             {"__meta_netbox_custom_field_simple": "Foobar 123"}, data["labels"]
         )
 
 
 class PrometheusIPAddressSerializerTests(TestCase):
     def test_ip_minimal_to_target(self):
         instance = utils.build_minimal_ip("10.10.10.10/24")
-        data = PrometheusIPAddressSerializer(instance=instance).data
+        data = PrometheusIPAddressSerializer(many=True, instance=[instance]).data[0]
 
         self.assertEqual(data["targets"], ["10.10.10.10"])
         self.assertDictContainsSubset({"__meta_netbox_id": str(instance.id)}, data["labels"])
         self.assertDictContainsSubset(
             {"__meta_netbox_status": "active"}, data["labels"]
         )
         self.assertDictContainsSubset(
             {"__meta_netbox_model": "IPAddress"}, data["labels"]
         )
 
     def test_ip_full_to_target(self):
         instance = utils.build_full_ip(
             address="10.10.10.10/24", dns_name="foo.example.com"
         )
-        data = PrometheusIPAddressSerializer(instance=instance).data
+        data = PrometheusIPAddressSerializer(many=True, instance=[instance]).data[0]
 
         self.assertEqual(
             data["targets"],
             ["foo.example.com"],
             "IP with DNS name should use DNS name as target",
         )
         self.assertDictContainsSubset({"__meta_netbox_id": str(instance.id)}, data["labels"])
```

### Comparing `netbox_plugin_prometheus_sd-0.6.3/pyproject.toml` & `netbox_plugin_prometheus_sd-0.7.0rc1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "netbox-plugin-prometheus-sd"
-version = "0.6.3" # placeholder
+version = "0.7.0rc1" # placeholder
 description = "A Netbox plugin to provide Netbox entires to Prometheus HTTP service discovery"
 authors = ["Felix Peters <felix.peters@breuninger.de>"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     { include = "netbox_prometheus_sd" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3"
-invoke = "^2.0.0"
-pylint = "^2.17.2"
+invoke = "^2.1.3"
+pylint = "^2.17.4"
 pylint-django = "^2.5.3"
-yamllint = "^1.30.0"
+yamllint = "^1.32.0"
 typed-ast = "^1.5.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `netbox_plugin_prometheus_sd-0.6.3/PKG-INFO` & `netbox_plugin_prometheus_sd-0.7.0rc1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-plugin-prometheus-sd
-Version: 0.6.3
+Version: 0.7.0rc1
 Summary: A Netbox plugin to provide Netbox entires to Prometheus HTTP service discovery
 License: MIT
 Author: Felix Peters
 Author-email: felix.peters@breuninger.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -23,15 +23,16 @@
 Provide Prometheus http_sd compatible API Endpoint with data from Netbox.
 
 HTTP SD is a new feature in Prometheus 2.28.0 that allows hosts to be found via a URL instead of just files.
 This plugin implements API endpoints in Netbox to make devices, IPs and virtual machines available to Prometheus.
 
 ## Compatibility
 
-We aim to support the latest major versions of Netbox. For now we Support Netbox `2.11`, `3.0`, `3.1`, `3.2` and `3.3` including bugfix versions.
+We aim to support the latest major versions of Netbox. For now we Support Netbox `3.2`, `3.3`, `3.4` and `3.5` including bugfix versions.
+Check the `.github/workflows/ci.yml` pipeline for the current tested builds. Other versions may work, but we do not test them explicitly.
 All relevant target versions are tested in CI. Have a look at the Github Actions definition for the current build targets.
 
 ## Installation
 
 The plugin is available as a Python package in pypi and can be installed with pip
 
     pip install netbox-plugin-prometheus-sd
@@ -57,14 +58,39 @@
 
 ```
 GET        /api/plugins/prometheus-sd/devices/              Get a list of devices in a prometheus compatible format
 GET        /api/plugins/prometheus-sd/virtual-machines/     Get a list of vms in a prometheus compatible format
 GET        /api/plugins/prometheus-sd/ip-addresses/         Get a list of ip in a prometheus compatible format
 ```
 
+### Config context
+
+The plugin can also discover extra config to inject in the HTTP SD JSON from the config context of the devices/virtual machines.
+If you have a `prometheus-plugin-prometheus-sd` entry in your config context with the following schema it will be automatically picked up:
+
+```
+prometheus-plugin-prometheus-sd:
+  - metrics_path: /not/metrics
+    port: 4242
+    scheme: https
+  - port: 4243
+```
+
+This allow you to configure those values directly into netbox instead of doing that inside the Prometheus
+config and filtering each scenario by a specific tag for instance.
+
+If there is only one entry you can also use this form:
+
+```
+prometheus-plugin-prometheus-sd:
+  metrics_path: /not/metrics
+  port: 4242
+  scheme: https
+```
+
 ### Example
 
 A working example on how to use this plugin with Prometheus is located at the `example` folder. Netbox content is created by using Netbox docker initializers.
 
 The demo data doesn't make sense, but they are good enough for demonstrating how to configure Prometheus and get demo data to Prometheus service discovery.
 
 Go to the `example` folder and run `docker-compose up`. Prometheus should get available on `http://localhost:9090`.
```

