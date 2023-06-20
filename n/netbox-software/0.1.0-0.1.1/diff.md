# Comparing `tmp/netbox_software-0.1.0.tar.gz` & `tmp/netbox_software-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_software-0.1.0.tar", max compression
+gzip compressed data, was "netbox_software-0.1.1.tar", max compression
```

## Comparing `netbox_software-0.1.0.tar` & `netbox_software-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,37 @@
--rw-r--r--   0        0        0    11357 2023-03-15 12:38:12.327212 netbox_software-0.1.0/LICENSE
--rw-r--r--   0        0        0     3420 2023-04-06 15:18:35.573875 netbox_software-0.1.0/README.md
--rw-r--r--   0        0        0      477 2023-04-06 13:29:54.486735 netbox_software-0.1.0/netbox_software/__init__.py
--rw-r--r--   0        0        0        0 2023-03-15 12:38:12.335212 netbox_software-0.1.0/netbox_software/api/__init__.py
--rw-r--r--   0        0        0     1073 2023-04-06 15:07:25.559695 netbox_software-0.1.0/netbox_software/api/serializers.py
--rw-r--r--   0        0        0      211 2023-04-06 15:07:25.571695 netbox_software-0.1.0/netbox_software/api/urls.py
--rw-r--r--   0        0        0      362 2023-04-06 15:07:25.563695 netbox_software-0.1.0/netbox_software/api/views.py
--rw-r--r--   0        0        0      504 2023-04-06 14:17:14.437496 netbox_software-0.1.0/netbox_software/filtersets.py
--rw-r--r--   0        0        0     1149 2023-04-06 14:17:14.413496 netbox_software-0.1.0/netbox_software/forms.py
--rw-r--r--   0        0        0     1537 2023-04-06 15:22:47.597705 netbox_software-0.1.0/netbox_software/migrations/0001_initial.py
--rw-r--r--   0        0        0      828 2023-04-06 15:07:25.571695 netbox_software-0.1.0/netbox_software/migrations/0002_alter_devicesoftware_options_and_more.py
--rw-r--r--   0        0        0        0 2023-03-15 12:38:12.335212 netbox_software-0.1.0/netbox_software/migrations/__init__.py
--rw-r--r--   0        0        0     1966 2023-04-06 14:17:14.409496 netbox_software-0.1.0/netbox_software/models.py
--rw-r--r--   0        0        0     1365 2023-04-06 14:17:14.397495 netbox_software-0.1.0/netbox_software/navigation.py
--rw-r--r--   0        0        0      436 2023-04-06 14:17:14.441496 netbox_software-0.1.0/netbox_software/search.py
--rw-r--r--   0        0        0      885 2023-04-06 14:29:26.996585 netbox_software-0.1.0/netbox_software/tables.py
--rw-r--r--   0        0        0     1093 2023-04-06 14:29:27.000585 netbox_software-0.1.0/netbox_software/template_content.py
--rw-r--r--   0        0        0     1539 2023-04-06 14:37:14.751838 netbox_software-0.1.0/netbox_software/templates/netbox_software/devicesoftware.html
--rw-r--r--   0        0        0      689 2023-04-06 14:47:25.961431 netbox_software-0.1.0/netbox_software/templates/netbox_software/devicesoftware_edit.html
--rw-r--r--   0        0        0     2223 2023-04-06 15:07:25.567695 netbox_software-0.1.0/netbox_software/templates/netbox_software/devicesoftware_include.html
--rw-r--r--   0        0        0      689 2023-04-06 15:07:25.563695 netbox_software-0.1.0/netbox_software/templates/netbox_software/software_edit.html
--rw-r--r--   0        0        0      850 2023-04-06 14:17:14.413496 netbox_software-0.1.0/netbox_software/urls.py
--rw-r--r--   0        0        0     1190 2023-04-06 14:17:14.405496 netbox_software-0.1.0/netbox_software/views.py
--rw-r--r--   0        0        0      318 2023-04-07 06:34:41.491754 netbox_software-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 netbox_software-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-15 12:38:12.327212 netbox_software-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3420 2023-04-06 15:18:35.573875 netbox_software-0.1.1/README.md
+-rw-r--r--   0        0        0      636 2023-06-20 08:54:35.545661 netbox_software-0.1.1/netbox_software/__init__.py
+-rw-r--r--   0        0        0      616 2023-06-19 13:55:08.848877 netbox_software-0.1.1/netbox_software/admin.py
+-rw-r--r--   0        0        0        0 2023-03-15 12:38:12.335212 netbox_software-0.1.1/netbox_software/api/__init__.py
+-rw-r--r--   0        0        0      149 2023-05-03 14:16:11.985814 netbox_software-0.1.1/netbox_software/api/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2291 2023-05-03 14:16:11.989815 netbox_software-0.1.1/netbox_software/api/__pycache__/serializers.cpython-310.pyc
+-rw-r--r--   0        0        0      452 2023-05-03 14:16:11.985814 netbox_software-0.1.1/netbox_software/api/__pycache__/urls.cpython-310.pyc
+-rw-r--r--   0        0        0      952 2023-05-03 14:16:11.989815 netbox_software-0.1.1/netbox_software/api/__pycache__/views.cpython-310.pyc
+-rw-r--r--   0        0        0     2116 2023-04-11 13:07:45.497532 netbox_software-0.1.1/netbox_software/api/serializers.py
+-rw-r--r--   0        0        0      293 2023-04-11 13:07:45.489532 netbox_software-0.1.1/netbox_software/api/urls.py
+-rw-r--r--   0        0        0      654 2023-04-11 13:07:45.493532 netbox_software-0.1.1/netbox_software/api/views.py
+-rw-r--r--   0        0        0      940 2023-04-11 13:14:52.527217 netbox_software-0.1.1/netbox_software/filtersets.py
+-rw-r--r--   0        0        0     3237 2023-06-19 14:07:22.839519 netbox_software-0.1.1/netbox_software/forms.py
+-rw-r--r--   0        0        0     5165 2023-06-19 14:48:40.521604 netbox_software-0.1.1/netbox_software/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-03-15 12:38:12.335212 netbox_software-0.1.1/netbox_software/migrations/__init__.py
+-rw-r--r--   0        0        0     1493 2023-05-03 14:16:14.621854 netbox_software-0.1.1/netbox_software/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0        0        0      912 2023-05-03 14:16:14.621854 netbox_software-0.1.1/netbox_software/migrations/__pycache__/0002_alter_devicesoftware_options_and_more.cpython-310.pyc
+-rw-r--r--   0        0        0      834 2023-05-03 14:16:14.621854 netbox_software-0.1.1/netbox_software/migrations/__pycache__/0003_alter_devicesoftware_options_and_more.cpython-310.pyc
+-rw-r--r--   0        0        0     1748 2023-05-03 14:16:14.621854 netbox_software-0.1.1/netbox_software/migrations/__pycache__/0004_virtualmachinesoftware.cpython-310.pyc
+-rw-r--r--   0        0        0      156 2023-05-03 14:16:14.617853 netbox_software-0.1.1/netbox_software/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4528 2023-06-19 14:46:32.247472 netbox_software-0.1.1/netbox_software/models.py
+-rw-r--r--   0        0        0     2299 2023-04-11 12:56:21.905069 netbox_software-0.1.1/netbox_software/navigation.py
+-rw-r--r--   0        0        0      697 2023-04-11 12:56:21.917069 netbox_software-0.1.1/netbox_software/search.py
+-rw-r--r--   0        0        0     1749 2023-04-11 12:56:21.909069 netbox_software-0.1.1/netbox_software/tables.py
+-rw-r--r--   0        0        0     2134 2023-04-11 13:31:53.564251 netbox_software-0.1.1/netbox_software/template_content.py
+-rw-r--r--   0        0        0     1539 2023-04-06 14:37:14.751838 netbox_software-0.1.1/netbox_software/templates/netbox_software/devicesoftware.html
+-rw-r--r--   0        0        0      689 2023-04-06 14:47:25.961431 netbox_software-0.1.1/netbox_software/templates/netbox_software/devicesoftware_edit.html
+-rw-r--r--   0        0        0     2230 2023-04-07 08:21:07.678785 netbox_software-0.1.1/netbox_software/templates/netbox_software/devicesoftware_include.html
+-rw-r--r--   0        0        0      650 2023-04-11 13:29:02.496416 netbox_software-0.1.1/netbox_software/templates/netbox_software/software_edit.html
+-rw-r--r--   0        0        0     1603 2023-04-11 12:56:21.909069 netbox_software-0.1.1/netbox_software/templates/netbox_software/virtualmachinesoftware.html
+-rw-r--r--   0        0        0      697 2023-04-11 13:07:45.485532 netbox_software-0.1.1/netbox_software/templates/netbox_software/virtualmachinesoftware_edit.html
+-rw-r--r--   0        0        0     2372 2023-04-11 14:14:34.161980 netbox_software-0.1.1/netbox_software/templates/netbox_software/virtualmachinesoftware_include.html
+-rw-r--r--   0        0        0     1762 2023-04-11 12:56:21.921069 netbox_software-0.1.1/netbox_software/urls.py
+-rw-r--r--   0        0        0     2346 2023-04-11 13:11:06.688023 netbox_software-0.1.1/netbox_software/views.py
+-rw-r--r--   0        0        0      318 2023-06-20 08:55:18.882312 netbox_software-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 netbox_software-0.1.1/PKG-INFO
```

### Comparing `netbox_software-0.1.0/LICENSE` & `netbox_software-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.0/README.md` & `netbox_software-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.0/netbox_software/api/serializers.py` & `netbox_software-0.1.1/netbox_software/api/serializers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from rest_framework import serializers
 
 from netbox.api.serializers import NetBoxModelSerializer, WritableNestedSerializer
-from ..models import DeviceSoftware
+from ..models import DeviceSoftware, VirtualMachineSoftware
 from dcim.api.nested_serializers import NestedDeviceSerializer
+from virtualization.api.nested_serializers import NestedVirtualMachineSerializer
 
 
 # Device Software Serializer
 class DeviceSoftwareSerializer(NetBoxModelSerializer):
 
     url = serializers.HyperlinkedIdentityField(
-        view_name='plugins-api:netboxsoftware-api:devicesoftware-detail'
+        view_name='plugins-api:netbox_software-api:devicesoftware-detail'
     )
 
     device = NestedDeviceSerializer()
 
     class Meta:
         model = DeviceSoftware
         fields = (
@@ -21,15 +22,45 @@
             'custom_fields', 'created', 'last_updated',
         )
 
 
 class NestedDeviceSoftwareSerializer(WritableNestedSerializer):
 
     url = serializers.HyperlinkedIdentityField(
-        view_name='plugins-api:netboxsoftware-api:devicesoftware-detail'
+        view_name='plugins-api:netbox_software-api:devicesoftware-detail'
     )
 
     class Meta:
         model = DeviceSoftware
         fields = (
             'id', 'url', 'display', 'name', 'software_type', 'source', 'version',
         )
+
+
+# Virtual Machine Software Serializer
+class VirtualMachineSoftwareSerializer(NetBoxModelSerializer):
+
+    url = serializers.HyperlinkedIdentityField(
+        view_name='plugins-api:netbox_software-api:virtualmachinesoftware-detail'
+    )
+
+    virtual_machine = NestedVirtualMachineSerializer()
+
+    class Meta:
+        model = VirtualMachineSoftware
+        fields = (
+            'id', 'url', 'display', 'name', 'software_type', 'source', 'version', 'virtual_machine', 'comments', 'tags',
+            'custom_fields', 'created', 'last_updated',
+        )
+
+
+class NestedVirtualMachineSoftwareSerializer(WritableNestedSerializer):
+
+    url = serializers.HyperlinkedIdentityField(
+        view_name='plugins-api:netbox_software-api:virtualmachinesoftware-detail'
+    )
+
+    class Meta:
+        model = VirtualMachineSoftware
+        fields = (
+            'id', 'url', 'display', 'name', 'software_type', 'source', 'version',
+        )
```

### Comparing `netbox_software-0.1.0/netbox_software/tables.py` & `netbox_software-0.1.1/netbox_software/tables.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,53 @@
 import django_tables2 as tables
 
 from netbox.tables import NetBoxTable, columns
-from .models import DeviceSoftware
-
+from .models import DeviceSoftware, VirtualMachineSoftware
 
 DEVICE_SOFTWARE_LINK = """
 {% if record %}
     <a href="{% url 'plugins:netbox_software:devicesoftware' pk=record.pk %}">{% firstof record.name record.name %}</a>
 {% endif %}
 """
 
+VIRTUAL_MACHINE_SOFTWARE_LINK = """
+{% if record %}
+    <a href="{% url 'plugins:netbox_software:virtualmachinesoftware' pk=record.pk %}">
+    {% firstof record.name record.name %}</a>
+{% endif %}
+"""
+
 
 class DeviceSoftwareTable(NetBoxTable):
     name = tables.TemplateColumn(template_code=DEVICE_SOFTWARE_LINK)
     software_type = columns.ChoiceFieldColumn()
     device = tables.Column(
         linkify=True
     )
 
     tags = columns.TagColumn(
         url_name='dcim:sitegroup_list'
     )
 
     class Meta(NetBoxTable.Meta):
         model = DeviceSoftware
-        fields = ('pk', 'id', 'name', 'software_type',  'source', 'version', 'device', 'comments', 'actions',
+        fields = ('pk', 'id', 'name', 'software_type', 'source', 'version', 'device', 'comments', 'actions',
                   'created', 'last_updated', 'tags')
         default_columns = ('name', 'software_type', 'device', 'tags')
+
+
+class VirtualMachineSoftwareTable(NetBoxTable):
+    name = tables.TemplateColumn(template_code=VIRTUAL_MACHINE_SOFTWARE_LINK)
+    software_type = columns.ChoiceFieldColumn()
+    virtual_machine = tables.Column(
+        linkify=True
+    )
+
+    tags = columns.TagColumn(
+        url_name='dcim:sitegroup_list'
+    )
+
+    class Meta(NetBoxTable.Meta):
+        model = VirtualMachineSoftware
+        fields = ('pk', 'id', 'name', 'software_type', 'source', 'version', 'virtual_machine', 'comments', 'actions',
+                  'created', 'last_updated', 'tags')
+        default_columns = ('name', 'software_type', 'virtual_machine', 'tags')
```

### Comparing `netbox_software-0.1.0/netbox_software/template_content.py` & `netbox_software-0.1.1/netbox_software/template_content.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from extras.plugins import PluginTemplateExtension
 from django.conf import settings
-from .models import DeviceSoftware
+from .models import DeviceSoftware, VirtualMachineSoftware
 
 plugin_settings = settings.PLUGINS_CONFIG.get('netbox_software', {})
 
 
 class DeviceSoftwareList(PluginTemplateExtension):
     model = 'dcim.device'
 
@@ -23,8 +23,30 @@
             return self.render('netbox_software/devicesoftware_include.html', extra_context={
                 'device_software': DeviceSoftware.objects.filter(device=self.context['object']),
             })
         else:
             return ""
 
 
-template_extensions = [DeviceSoftwareList]
+class VirtualMachineSoftwareList(PluginTemplateExtension):
+    model = 'virtualization.virtualmachine'
+
+    def left_page(self):
+        if plugin_settings.get('enable_virtual-machine_software') and plugin_settings.get('virtual-machine_software_location') == 'left':
+
+            return self.render('netbox_software/virtualmachinesoftware_include.html', extra_context={
+                'virtual_machine_software': VirtualMachineSoftware.objects.filter(virtual_machine=self.context['object']),
+            })
+        else:
+            return ""
+
+    def right_page(self):
+        if plugin_settings.get('enable_virtual-machine_software') and plugin_settings.get('virtual-machine_software_location') == 'right':
+
+            return self.render('netbox_software/virtualmachinesoftware_include.html', extra_context={
+                'virtual_machine_software': VirtualMachineSoftware.objects.filter(virtual_machine=self.context['object']),
+            })
+        else:
+            return ""
+
+
+template_extensions = [DeviceSoftwareList, VirtualMachineSoftwareList]
```

### Comparing `netbox_software-0.1.0/netbox_software/templates/netbox_software/devicesoftware.html` & `netbox_software-0.1.1/netbox_software/templates/netbox_software/devicesoftware.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.0/netbox_software/templates/netbox_software/devicesoftware_edit.html` & `netbox_software-0.1.1/netbox_software/templates/netbox_software/devicesoftware_edit.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.0/netbox_software/templates/netbox_software/devicesoftware_include.html` & `netbox_software-0.1.1/netbox_software/templates/netbox_software/devicesoftware_include.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% load helpers %}
 
 <div class="card">
 <h5 class="card-header">
-    Документы
+    ПО устройства
 </h5>
 <div class="card-body">
 {% if device_software %}
     <table class="table table-hover">
         <tr>
             <th>Название</th>
             <th>источник</th>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {% load helpers %}
-** ÐÐ¾ÐºÑÐ¼ÐµÐ½ÑÑ **
+** ÐÐ ÑÑÑÑÐ¾Ð¹ÑÑÐ²Ð° **
 {% if device_software %}
 ÐÐ°Ð·Ð²�Ð¸ÑÑÐ¾�Ð²ÐµÑÑ�Ð¢Ð¸Ð¿
                  {                {                {% badge
 {{ software.name {                {                software.get_software_type_display
 }}               software.source  software.version bg_color=software.get_software_type_color
                  }}               }}               %}
 {% else %}
```

### Comparing `netbox_software-0.1.0/netbox_software/templates/netbox_software/software_edit.html` & `netbox_software-0.1.1/netbox_software/templates/netbox_software/software_edit.html`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,14 @@
     <div class="field-group my-5">
       {% render_field form.name %}
 
       <div class="field-group my-1">
         {% render_field form.software_type %}
         {% render_field form.source %}
         {% render_field form.version %}
-        {% render_field form.device %}
 
         <div class="field-group my-5">
             <div class="row mb-2">
               <h5 class="text-center">Комментарии</h5>
             </div>
             {% render_field form.comments %}
         </div>
```

### Comparing `netbox_software-0.1.0/netbox_software/views.py` & `netbox_software-0.1.1/netbox_software/views.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,13 +18,40 @@
 
 
 class DeviceSoftwareEditView(PermissionRequiredMixin, generic.ObjectEditView):
     permission_required = ('dcim.view_site', 'dcim.view_device')
     queryset = models.DeviceSoftware.objects.all()
     form = forms.DeviceSoftwareForm
 
-    template_name = 'netbox_documents/devicesoftware_edit.html'
+    template_name = 'netbox_software/devicesoftware_edit.html'
 
 
 class DeviceSoftwareDeleteView(PermissionRequiredMixin, generic.ObjectDeleteView):
     permission_required = ('dcim.view_site', 'dcim.view_device')
     queryset = models.DeviceSoftware.objects.all()
+
+
+### VirtualMachineSoftware
+class VirtualMachineSoftwareView(PermissionRequiredMixin, generic.ObjectView):
+    permission_required = ('dcim.view_site', 'dcim.view_device')
+    queryset = models.VirtualMachineSoftware.objects.all()
+
+
+class VirtualMachineSoftwareListView(PermissionRequiredMixin, generic.ObjectListView):
+    permission_required = ('dcim.view_site', 'dcim.view_device')
+    queryset = models.VirtualMachineSoftware.objects.all()
+    table = tables.VirtualMachineSoftwareTable
+    filterset = filtersets.VirtualMachineSoftwareFilterSet
+    filterset_form = forms.VirtualMachineSoftwareFilterForm
+
+
+class VirtualMachineSoftwareEditView(PermissionRequiredMixin, generic.ObjectEditView):
+    permission_required = ('dcim.view_site', 'dcim.view_device')
+    queryset = models.VirtualMachineSoftware.objects.all()
+    form = forms.VirtualMachineSoftwareForm
+
+    template_name = 'netbox_software/virtualmachinesoftware_edit.html'
+
+
+class VirtualMachineSoftwareDeleteView(PermissionRequiredMixin, generic.ObjectDeleteView):
+    permission_required = ('dcim.view_site', 'dcim.view_device')
+    queryset = models.VirtualMachineSoftware.objects.all()
```

### Comparing `netbox_software-0.1.0/PKG-INFO` & `netbox_software-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-software
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: izakharov
 Author-email: ilya.zakharov@domrf.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

