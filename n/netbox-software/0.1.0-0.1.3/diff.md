# Comparing `tmp/netbox_software-0.1.0.tar.gz` & `tmp/netbox_software-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_software-0.1.0.tar", max compression
+gzip compressed data, was "netbox_software-0.1.3.tar", max compression
```

## Comparing `netbox_software-0.1.0.tar` & `netbox_software-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,30 @@
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
+-rw-r--r--   0        0        0    11357 2023-06-20 09:07:55.621872 netbox_software-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3420 2023-06-20 09:07:55.621872 netbox_software-0.1.3/README.md
+-rw-r--r--   0        0        0      636 2023-06-20 10:04:58.469856 netbox_software-0.1.3/netbox_software/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.1.3/netbox_software/api/__init__.py
+-rw-r--r--   0        0        0     3513 2023-06-20 09:54:33.064309 netbox_software-0.1.3/netbox_software/api/serializers.py
+-rw-r--r--   0        0        0      399 2023-06-20 09:54:33.084309 netbox_software-0.1.3/netbox_software/api/urls.py
+-rw-r--r--   0        0        0     1076 2023-06-20 09:54:33.056309 netbox_software-0.1.3/netbox_software/api/views.py
+-rw-r--r--   0        0        0     1672 2023-06-20 09:54:33.036309 netbox_software-0.1.3/netbox_software/filtersets.py
+-rw-r--r--   0        0        0     3998 2023-06-20 09:54:33.072309 netbox_software-0.1.3/netbox_software/forms.py
+-rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.1.3/netbox_software/migrations/__init__.py
+-rw-r--r--   0        0        0     4395 2023-06-20 10:04:20.725280 netbox_software-0.1.3/netbox_software/models.py
+-rw-r--r--   0        0        0     2299 2023-06-20 09:07:55.625872 netbox_software-0.1.3/netbox_software/navigation.py
+-rw-r--r--   0        0        0     1029 2023-06-20 09:54:33.080309 netbox_software-0.1.3/netbox_software/search.py
+-rw-r--r--   0        0        0     2857 2023-06-20 09:54:33.060309 netbox_software-0.1.3/netbox_software/tables.py
+-rw-r--r--   0        0        0     2133 2023-06-20 09:54:33.040309 netbox_software-0.1.3/netbox_software/template_content.py
+-rw-r--r--   0        0        0     1539 2023-06-20 09:07:55.629872 netbox_software-0.1.3/netbox_software/templates/netbox_software/devicesoftware.html
+-rw-r--r--   0        0        0      689 2023-06-20 09:07:55.629872 netbox_software-0.1.3/netbox_software/templates/netbox_software/devicesoftware_edit.html
+-rw-r--r--   0        0        0     2230 2023-06-20 09:07:55.629872 netbox_software-0.1.3/netbox_software/templates/netbox_software/devicesoftware_include.html
+-rw-r--r--   0        0        0      650 2023-06-20 09:07:55.629872 netbox_software-0.1.3/netbox_software/templates/netbox_software/software_edit.html
+-rw-r--r--   0        0        0      663 2023-06-20 09:55:48.277457 netbox_software-0.1.3/netbox_software/templates/netbox_software/softwaretype.html
+-rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.1.3/netbox_software/templates/netbox_software/softwaretype_edit.html
+-rw-r--r--   0        0        0      674 2023-06-20 09:55:20.813038 netbox_software-0.1.3/netbox_software/templates/netbox_software/vendor.html
+-rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.1.3/netbox_software/templates/netbox_software/vendor_edit.html
+-rw-r--r--   0        0        0     1603 2023-06-20 09:07:55.629872 netbox_software-0.1.3/netbox_software/templates/netbox_software/virtualmachinesoftware.html
+-rw-r--r--   0        0        0      697 2023-06-20 09:07:55.629872 netbox_software-0.1.3/netbox_software/templates/netbox_software/virtualmachinesoftware_edit.html
+-rw-r--r--   0        0        0     2372 2023-06-20 09:07:55.629872 netbox_software-0.1.3/netbox_software/templates/netbox_software/virtualmachinesoftware_include.html
+-rw-r--r--   0        0        0     2994 2023-06-20 09:54:33.052309 netbox_software-0.1.3/netbox_software/urls.py
+-rw-r--r--   0        0        0     4297 2023-06-20 09:54:33.044309 netbox_software-0.1.3/netbox_software/views.py
+-rw-r--r--   0        0        0      318 2023-06-20 10:04:58.465856 netbox_software-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 netbox_software-0.1.3/PKG-INFO
```

### Comparing `netbox_software-0.1.0/LICENSE` & `netbox_software-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.0/README.md` & `netbox_software-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.0/netbox_software/template_content.py` & `netbox_software-0.1.3/netbox_software/template_content.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from extras.plugins import PluginTemplateExtension
 from django.conf import settings
-from .models import DeviceSoftware
+from .models import DeviceSoftware, VirtualMachineSoftware
 
 plugin_settings = settings.PLUGINS_CONFIG.get('netbox_software', {})
 
 
 class DeviceSoftwareList(PluginTemplateExtension):
     model = 'dcim.device'
-
     def left_page(self):
         if plugin_settings.get('enable_device_software') and plugin_settings.get('device_software_location') == 'left':
 
             return self.render('netbox_software/devicesoftware_include.html', extra_context={
                 'device_software': DeviceSoftware.objects.filter(device=self.context['object']),
             })
         else:
@@ -23,8 +22,30 @@
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

### Comparing `netbox_software-0.1.0/netbox_software/templates/netbox_software/devicesoftware.html` & `netbox_software-0.1.3/netbox_software/templates/netbox_software/devicesoftware.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.0/netbox_software/templates/netbox_software/devicesoftware_edit.html` & `netbox_software-0.1.3/netbox_software/templates/netbox_software/devicesoftware_edit.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.0/netbox_software/templates/netbox_software/devicesoftware_include.html` & `netbox_software-0.1.3/netbox_software/templates/netbox_software/devicesoftware_include.html`

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

### Comparing `netbox_software-0.1.0/netbox_software/templates/netbox_software/software_edit.html` & `netbox_software-0.1.3/netbox_software/templates/netbox_software/software_edit.html`

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

### Comparing `netbox_software-0.1.0/PKG-INFO` & `netbox_software-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-software
-Version: 0.1.0
+Version: 0.1.3
 Summary: 
 Author: izakharov
 Author-email: ilya.zakharov@domrf.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

