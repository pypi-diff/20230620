# Comparing `tmp/netbox_software-0.1.4.tar.gz` & `tmp/netbox_software-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_software-0.1.4.tar", max compression
+gzip compressed data, was "netbox_software-0.1.5.tar", max compression
```

## Comparing `netbox_software-0.1.4.tar` & `netbox_software-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,32 @@
--rw-r--r--   0        0        0    11357 2023-06-20 09:07:55.621872 netbox_software-0.1.4/LICENSE
--rw-r--r--   0        0        0     3420 2023-06-20 09:07:55.621872 netbox_software-0.1.4/README.md
--rw-r--r--   0        0        0      636 2023-06-20 10:07:37.388282 netbox_software-0.1.4/netbox_software/__init__.py
--rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.1.4/netbox_software/api/__init__.py
--rw-r--r--   0        0        0     3513 2023-06-20 09:54:33.064309 netbox_software-0.1.4/netbox_software/api/serializers.py
--rw-r--r--   0        0        0      399 2023-06-20 09:54:33.084309 netbox_software-0.1.4/netbox_software/api/urls.py
--rw-r--r--   0        0        0     1076 2023-06-20 09:54:33.056309 netbox_software-0.1.4/netbox_software/api/views.py
--rw-r--r--   0        0        0     1672 2023-06-20 09:54:33.036309 netbox_software-0.1.4/netbox_software/filtersets.py
--rw-r--r--   0        0        0     3975 2023-06-20 10:07:37.384282 netbox_software-0.1.4/netbox_software/forms.py
--rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.1.4/netbox_software/migrations/__init__.py
--rw-r--r--   0        0        0     4395 2023-06-20 10:04:20.725280 netbox_software-0.1.4/netbox_software/models.py
--rw-r--r--   0        0        0     2299 2023-06-20 09:07:55.625872 netbox_software-0.1.4/netbox_software/navigation.py
--rw-r--r--   0        0        0     1029 2023-06-20 09:54:33.080309 netbox_software-0.1.4/netbox_software/search.py
--rw-r--r--   0        0        0     2857 2023-06-20 09:54:33.060309 netbox_software-0.1.4/netbox_software/tables.py
--rw-r--r--   0        0        0     2133 2023-06-20 09:54:33.040309 netbox_software-0.1.4/netbox_software/template_content.py
--rw-r--r--   0        0        0     1539 2023-06-20 09:07:55.629872 netbox_software-0.1.4/netbox_software/templates/netbox_software/devicesoftware.html
--rw-r--r--   0        0        0      689 2023-06-20 09:07:55.629872 netbox_software-0.1.4/netbox_software/templates/netbox_software/devicesoftware_edit.html
--rw-r--r--   0        0        0     2230 2023-06-20 09:07:55.629872 netbox_software-0.1.4/netbox_software/templates/netbox_software/devicesoftware_include.html
--rw-r--r--   0        0        0      650 2023-06-20 09:07:55.629872 netbox_software-0.1.4/netbox_software/templates/netbox_software/software_edit.html
--rw-r--r--   0        0        0      663 2023-06-20 09:55:48.277457 netbox_software-0.1.4/netbox_software/templates/netbox_software/softwaretype.html
--rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.1.4/netbox_software/templates/netbox_software/softwaretype_edit.html
--rw-r--r--   0        0        0      674 2023-06-20 09:55:20.813038 netbox_software-0.1.4/netbox_software/templates/netbox_software/vendor.html
--rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.1.4/netbox_software/templates/netbox_software/vendor_edit.html
--rw-r--r--   0        0        0     1603 2023-06-20 09:07:55.629872 netbox_software-0.1.4/netbox_software/templates/netbox_software/virtualmachinesoftware.html
--rw-r--r--   0        0        0      697 2023-06-20 09:07:55.629872 netbox_software-0.1.4/netbox_software/templates/netbox_software/virtualmachinesoftware_edit.html
--rw-r--r--   0        0        0     2372 2023-06-20 09:07:55.629872 netbox_software-0.1.4/netbox_software/templates/netbox_software/virtualmachinesoftware_include.html
--rw-r--r--   0        0        0     2994 2023-06-20 09:54:33.052309 netbox_software-0.1.4/netbox_software/urls.py
--rw-r--r--   0        0        0     4297 2023-06-20 09:54:33.044309 netbox_software-0.1.4/netbox_software/views.py
--rw-r--r--   0        0        0      318 2023-06-20 10:07:37.380282 netbox_software-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 netbox_software-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-20 09:07:55.621872 netbox_software-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3420 2023-06-20 09:07:55.621872 netbox_software-0.1.5/README.md
+-rw-r--r--   0        0        0      636 2023-06-20 11:07:52.786908 netbox_software-0.1.5/netbox_software/__init__.py
+-rw-r--r--   0        0        0      616 2023-06-19 13:55:08.848877 netbox_software-0.1.5/netbox_software/admin.py
+-rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.1.5/netbox_software/api/__init__.py
+-rw-r--r--   0        0        0     3459 2023-06-20 10:54:23.034743 netbox_software-0.1.5/netbox_software/api/serializers.py
+-rw-r--r--   0        0        0      399 2023-06-20 09:54:33.084309 netbox_software-0.1.5/netbox_software/api/urls.py
+-rw-r--r--   0        0        0     1076 2023-06-20 09:54:33.056309 netbox_software-0.1.5/netbox_software/api/views.py
+-rw-r--r--   0        0        0     1705 2023-06-20 11:07:06.570213 netbox_software-0.1.5/netbox_software/filtersets.py
+-rw-r--r--   0        0        0     3975 2023-06-20 10:07:37.384282 netbox_software-0.1.5/netbox_software/forms.py
+-rw-r--r--   0        0        0     5261 2023-06-20 10:12:28.772709 netbox_software-0.1.5/netbox_software/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-20 09:07:55.625872 netbox_software-0.1.5/netbox_software/migrations/__init__.py
+-rw-r--r--   0        0        0     4395 2023-06-20 10:04:20.725280 netbox_software-0.1.5/netbox_software/models.py
+-rw-r--r--   0        0        0     2299 2023-06-20 09:07:55.625872 netbox_software-0.1.5/netbox_software/navigation.py
+-rw-r--r--   0        0        0     1029 2023-06-20 09:54:33.080309 netbox_software-0.1.5/netbox_software/search.py
+-rw-r--r--   0        0        0     2857 2023-06-20 09:54:33.060309 netbox_software-0.1.5/netbox_software/tables.py
+-rw-r--r--   0        0        0     2133 2023-06-20 09:54:33.040309 netbox_software-0.1.5/netbox_software/template_content.py
+-rw-r--r--   0        0        0     1539 2023-06-20 10:19:00.886666 netbox_software-0.1.5/netbox_software/templates/netbox_software/devicesoftware.html
+-rw-r--r--   0        0        0      693 2023-06-20 10:19:13.746862 netbox_software-0.1.5/netbox_software/templates/netbox_software/devicesoftware_edit.html
+-rw-r--r--   0        0        0     2230 2023-06-20 10:19:00.870666 netbox_software-0.1.5/netbox_software/templates/netbox_software/devicesoftware_include.html
+-rw-r--r--   0        0        0      650 2023-06-20 10:19:00.878666 netbox_software-0.1.5/netbox_software/templates/netbox_software/software_edit.html
+-rw-r--r--   0        0        0      663 2023-06-20 09:55:48.277457 netbox_software-0.1.5/netbox_software/templates/netbox_software/softwaretype.html
+-rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.1.5/netbox_software/templates/netbox_software/softwaretype_edit.html
+-rw-r--r--   0        0        0      674 2023-06-20 09:55:20.813038 netbox_software-0.1.5/netbox_software/templates/netbox_software/vendor.html
+-rw-r--r--   0        0        0      487 2023-06-20 09:56:36.178188 netbox_software-0.1.5/netbox_software/templates/netbox_software/vendor_edit.html
+-rw-r--r--   0        0        0     1603 2023-06-20 10:19:00.894666 netbox_software-0.1.5/netbox_software/templates/netbox_software/virtualmachinesoftware.html
+-rw-r--r--   0        0        0      697 2023-06-20 10:19:00.898666 netbox_software-0.1.5/netbox_software/templates/netbox_software/virtualmachinesoftware_edit.html
+-rw-r--r--   0        0        0     2372 2023-06-20 10:19:00.890666 netbox_software-0.1.5/netbox_software/templates/netbox_software/virtualmachinesoftware_include.html
+-rw-r--r--   0        0        0     2994 2023-06-20 09:54:33.052309 netbox_software-0.1.5/netbox_software/urls.py
+-rw-r--r--   0        0        0     4297 2023-06-20 09:54:33.044309 netbox_software-0.1.5/netbox_software/views.py
+-rw-r--r--   0        0        0      318 2023-06-20 11:07:52.778908 netbox_software-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 netbox_software-0.1.5/PKG-INFO
```

### Comparing `netbox_software-0.1.4/LICENSE` & `netbox_software-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.4/README.md` & `netbox_software-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.4/netbox_software/__init__.py` & `netbox_software-0.1.5/netbox_software/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from extras.plugins import PluginConfig
 
 
 class NetboxSoftware(PluginConfig):
     name = 'netbox_software'
     verbose_name = 'Установленное ПО'
     description = 'Manage device software in Netbox'
-    version = '0.1.4'
+    version = '0.1.5'
     author = 'Ilya Zakharov'
     author_email = 'me@izakharov.ru'
     min_version = '3.2.0'
     base_url = 'software'
     default_settings = {
         "enable_navigation_menu": True,
         "enable_device_software": True,
```

### Comparing `netbox_software-0.1.4/netbox_software/api/serializers.py` & `netbox_software-0.1.5/netbox_software/api/serializers.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,27 +4,23 @@
 from ..models import DeviceSoftware, VirtualMachineSoftware, SoftwareType, Vendor
 from dcim.api.nested_serializers import NestedDeviceSerializer
 from virtualization.api.nested_serializers import NestedVirtualMachineSerializer
 
 
 # Vendor Serializer
 class VendorSerializer(NetBoxModelSerializer):
-    url = serializers.HyperlinkedIdentityField(
-        view_name='plugins-api:netbox_software-api:vendor-detail'
-    )
+    url = serializers.HyperlinkedIdentityField(view_name='plugins-api:netbox_software-api:vendor-detail')
 
     class Meta:
         model = Vendor
         fields = ('id', 'url', 'display', 'name', 'comments', 'custom_fields', 'created', 'last_updated',)
 
 
 class NestedVendorSerializer(WritableNestedSerializer):
-    url = serializers.HyperlinkedIdentityField(
-        view_name='plugins-api:netbox_software-api:vendor-detail'
-    )
+    url = serializers.HyperlinkedIdentityField(view_name='plugins-api:netbox_software-api:vendor-detail')
 
     class Meta:
         model = Vendor
         fields = ('id', 'url', 'display', 'name',)
 
 
 # Vendor Serializer
@@ -46,14 +42,15 @@
     class Meta:
         model = SoftwareType
         fields = ('id', 'url', 'display', 'name',)
 
 
 # Device Software Serializer
 class DeviceSoftwareSerializer(NetBoxModelSerializer):
+
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_software-api:devicesoftware-detail'
     )
     device = NestedDeviceSerializer()
     software_type = NestedSoftwareTypeSerializer()
     vendor = NestedVendorSerializer()
     class Meta:
@@ -66,15 +63,15 @@
 
 class NestedDeviceSoftwareSerializer(WritableNestedSerializer):
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_software-api:devicesoftware-detail'
     )
     class Meta:
         model = DeviceSoftware
-        fields = ('id', 'url', 'display', 'name', 'software_type', 'vendor', 'version',)
+        fields = ('id', 'url', 'display', 'name', 'version',)
 
 
 # Virtual Machine Software Serializer
 class VirtualMachineSoftwareSerializer(NetBoxModelSerializer):
 
     url = serializers.HyperlinkedIdentityField(
         view_name='plugins-api:netbox_software-api:virtualmachinesoftware-detail'
```

### Comparing `netbox_software-0.1.4/netbox_software/api/views.py` & `netbox_software-0.1.5/netbox_software/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.4/netbox_software/filtersets.py` & `netbox_software-0.1.5/netbox_software/filtersets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,42 @@
+import django_filters
 from netbox.filtersets import NetBoxModelFilterSet
-from .models import DeviceSoftware, VirtualMachineSoftware
+from .models import DeviceSoftware, VirtualMachineSoftware, SoftwareType, Vendor
 from django.db.models import Q
 
 
 class VendorFilterSet(NetBoxModelFilterSet):
     class Meta:
-        model = DeviceSoftware
+        model = Vendor
         fields = ('id', 'name',)
 
     def search(self, queryset, name, value):
         if not value.strip():
             return queryset
         return queryset.filter(
             Q(name__icontains=value) |
             Q(comments__icontains=value)
         )
 
 
 class SoftwareTypeFilterSet(NetBoxModelFilterSet):
     class Meta:
-        model = DeviceSoftware
+        model = SoftwareType
         fields = ('id', 'name',)
 
     def search(self, queryset, name, value):
         if not value.strip():
             return queryset
         return queryset.filter(
             Q(name__icontains=value) |
             Q(comments__icontains=value)
         )
 
 
 class DeviceSoftwareFilterSet(NetBoxModelFilterSet):
-
     class Meta:
         model = DeviceSoftware
         fields = ('id', 'name', 'software_type', 'device', 'vendor')
 
     def search(self, queryset, name, value):
         if not value.strip():
             return queryset
```

### Comparing `netbox_software-0.1.4/netbox_software/forms.py` & `netbox_software-0.1.5/netbox_software/forms.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.4/netbox_software/models.py` & `netbox_software-0.1.5/netbox_software/models.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.4/netbox_software/navigation.py` & `netbox_software-0.1.5/netbox_software/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.4/netbox_software/search.py` & `netbox_software-0.1.5/netbox_software/search.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.4/netbox_software/tables.py` & `netbox_software-0.1.5/netbox_software/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.4/netbox_software/template_content.py` & `netbox_software-0.1.5/netbox_software/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.4/netbox_software/templates/netbox_software/devicesoftware.html` & `netbox_software-0.1.5/netbox_software/templates/netbox_software/devicesoftware.html`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             </tr>
             <tr>
               <th scope="row">Наименование</th>
               <td><a href="{{ object.software.url }}" target="_blank">{{ object.name }}</a></td>
             </tr>
             <tr>
               <th scope="row">Источник</th>
-              <td>{{ object.source|placeholder }}</tr>
+              <td>{{ object.vendor|placeholder }}</tr>
             <tr>
               <th scope="row">Версия</th>
               <td>{{ object.version|placeholder }}</tr>
           </table>
         </div>
       </div>
       {% include 'inc/panels/custom_fields.html' %}
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% extends 'generic/object.html' %} {% load helpers %} {% block content %}
 ** ÐÐ ÑÑÑÑÐ¾Ð¹ÑÑÐ²Ð° **
 ÐÐ°Ð·Ð²Ð°Ð½�{{ object.name|placeholder }}
 Ð£ÑÑÑÐ¾Ð¹�{{_object.device_}}
 Ð¢Ð¸Ð¿ ÐÐ    {% badge object.get_software_type_display
                          bg_color=object.get_software_type_color %}
 ÐÐ°Ð¸Ð¼ÐµÐ½�{{_object.name_}}¸Ðµ
-ÐÑÑÐ¾ÑÐ½�{{ object.source|placeholder }}
+ÐÑÑÐ¾ÑÐ½�{{ object.vendor|placeholder }}
 ÐÐµÑÑÐ¸Ñ {{ object.version|placeholder }}
 {% include 'inc/panels/custom_fields.html' %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
 {% endblock content %}
```

### Comparing `netbox_software-0.1.4/netbox_software/templates/netbox_software/devicesoftware_edit.html` & `netbox_software-0.1.5/netbox_software/templates/netbox_software/devicesoftware_edit.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-{% extends 'generic/object_edit.html' %}
+/p  {% extends 'generic/object_edit.html' %}
 {% load static %}
 {% load form_helpers %}
 {% load helpers %}
 
 {% block form %}
     <div class="field-group my-5">
       {% render_field form.name %}
 
       <div class="field-group my-1">
         {% render_field form.software_type %}
-        {% render_field form.source %}
+        {% render_field form.vendor %}
         {% render_field form.version %}
         {% render_field form.device %}
 
         <div class="field-group my-5">
             <div class="row mb-2">
               <h5 class="text-center">Комментарии</h5>
             </div>
```

### Comparing `netbox_software-0.1.4/netbox_software/templates/netbox_software/devicesoftware_include.html` & `netbox_software-0.1.5/netbox_software/templates/netbox_software/devicesoftware_include.html`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             <th></th>
         </tr>
         {% for software in device_software %}
         <tr>
             <td>
                 {{ software.name }}
             </td>
-            <td>{{ software.source }}</td>
+            <td>{{ software.vendor }}</td>
             <td>{{ software.version }}</td>
             <td>{% badge software.get_software_type_display bg_color=software.get_software_type_color %}</td>
             <td class="text-end noprint">
                 <a href="{% url 'plugins:netbox_software:devicesoftware' pk=software.pk %}"
                    class="btn btn-primary btn-sm lh-1" title="Просмотреть">
                     <i class="mdi mdi-book" aria-hidden="true"></i>
                   </a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% load helpers %}
 ** ÐÐ ÑÑÑÑÐ¾Ð¹ÑÑÐ²Ð° **
 {% if device_software %}
 ÐÐ°Ð·Ð²�Ð¸ÑÑÐ¾�Ð²ÐµÑÑ�Ð¢Ð¸Ð¿
                  {                {                {% badge
 {{ software.name {                {                software.get_software_type_display
-}}               software.source  software.version bg_color=software.get_software_type_color
+}}               software.vendor  software.version bg_color=software.get_software_type_color
                  }}               }}               %}
 {% else %}
 ÐÐµÑ
 {% endif %}
  ÐÐ¾Ð±Ð°Ð²Ð¸ÑÑ_ÐÐ
```

### Comparing `netbox_software-0.1.4/netbox_software/templates/netbox_software/software_edit.html` & `netbox_software-0.1.5/netbox_software/templates/netbox_software/software_edit.html`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 {% block form %}
     <div class="field-group my-5">
       {% render_field form.name %}
 
       <div class="field-group my-1">
         {% render_field form.software_type %}
-        {% render_field form.source %}
+        {% render_field form.vendor %}
         {% render_field form.version %}
 
         <div class="field-group my-5">
             <div class="row mb-2">
               <h5 class="text-center">Комментарии</h5>
             </div>
             {% render_field form.comments %}
```

### Comparing `netbox_software-0.1.4/netbox_software/templates/netbox_software/softwaretype.html` & `netbox_software-0.1.5/netbox_software/templates/netbox_software/softwaretype.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.4/netbox_software/templates/netbox_software/vendor.html` & `netbox_software-0.1.5/netbox_software/templates/netbox_software/vendor.html`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.4/netbox_software/templates/netbox_software/virtualmachinesoftware.html` & `netbox_software-0.1.5/netbox_software/templates/netbox_software/virtualmachinesoftware.html`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             </tr>
             <tr>
               <th scope="row">Наименование</th>
               <td><a href="{{ object.software.url }}" target="_blank">{{ object.name }}</a></td>
             </tr>
             <tr>
               <th scope="row">Источник</th>
-              <td>{{ object.source|placeholder }}</tr>
+              <td>{{ object.vendor|placeholder }}</tr>
             <tr>
               <th scope="row">Версия</th>
               <td>{{ object.version|placeholder }}</tr>
           </table>
         </div>
       </div>
       {% include 'inc/panels/custom_fields.html' %}
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% extends 'generic/object.html' %} {% load helpers %} {% block content %}
 ** ÐÐ Ð²Ð¸ÑÑÑÐ°Ð»ÑÐ½ÑÑ Ð¼Ð°ÑÐ¸Ð½ **
 ÐÐ°Ð·Ð²Ð°Ð½Ð¸Ðµ    {{ object.name|placeholder }}
 ÐÐ¸ÑÑÑÐ°Ð»ÑÐ½{{_object.virtual_machine_}}�Ð°
 Ð¢Ð¸Ð¿ ÐÐ               {% badge object.get_software_type_display
                                     bg_color=object.get_software_type_color %}
 ÐÐ°Ð¸Ð¼ÐµÐ½Ð¾Ð²Ð°{{_object.name_}}
-ÐÑÑÐ¾ÑÐ½Ð¸Ðº    {{ object.source|placeholder }}
+ÐÑÑÐ¾ÑÐ½Ð¸Ðº    {{ object.vendor|placeholder }}
 ÐÐµÑÑÐ¸Ñ            {{ object.version|placeholder }}
 {% include 'inc/panels/custom_fields.html' %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
 {% endblock content %}
```

### Comparing `netbox_software-0.1.4/netbox_software/templates/netbox_software/virtualmachinesoftware_edit.html` & `netbox_software-0.1.5/netbox_software/templates/netbox_software/virtualmachinesoftware_edit.html`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 {% block form %}
     <div class="field-group my-5">
       {% render_field form.name %}
 
       <div class="field-group my-1">
         {% render_field form.software_type %}
-        {% render_field form.source %}
+        {% render_field form.vendor %}
         {% render_field form.version %}
         {% render_field form.virtual_machine %}
         <div class="field-group my-5">
             <div class="row mb-2">
               <h5 class="text-center">Комментарии</h5>
             </div>
             {% render_field form.comments %}
```

### Comparing `netbox_software-0.1.4/netbox_software/templates/netbox_software/virtualmachinesoftware_include.html` & `netbox_software-0.1.5/netbox_software/templates/netbox_software/virtualmachinesoftware_include.html`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             <th></th>
         </tr>
         {% for software in virtual_machine_software %}
         <tr>
             <td>
                 {{ software.name }}
             </td>
-            <td>{{ software.source }}</td>
+            <td>{{ software.vendor }}</td>
             <td>{{ software.version }}</td>
             <td>{% badge software.get_software_type_display bg_color=software.get_software_type_color %}</td>
             <td class="text-end noprint">
                 <a href="{% url 'plugins:netbox_software:virtualmachinesoftware' pk=software.pk %}"
                    class="btn btn-primary btn-sm lh-1" title="Просмотреть">
                     <i class="mdi mdi-book" aria-hidden="true"></i>
                   </a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% load helpers %}
 ** ÐÐ Ð²Ð¸ÑÑÑÐ°Ð»ÑÐ½ÑÑ Ð¼Ð°ÑÐ¸Ð½ **
 {% if virtual_machine_software %}
 ÐÐ°Ð·Ð²�Ð Ð°Ð·ÑÐ°Ð�ÐÐµÑÑ�Ð¢Ð¸Ð¿
                                         {                {% badge
-{{ software.name {{ software.source }}  {                software.get_software_type_display
+{{ software.name {{ software.vendor }}  {                software.get_software_type_display
 }}                                      software.version bg_color=software.get_software_type_color
                                         }}               %}
 {% else %}
 ÐÐµÑ
 {% endif %}
  ÐÐ¾Ð±Ð°Ð²Ð¸ÑÑ_ÐÐ
```

### Comparing `netbox_software-0.1.4/netbox_software/urls.py` & `netbox_software-0.1.5/netbox_software/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.4/netbox_software/views.py` & `netbox_software-0.1.5/netbox_software/views.py`

 * *Files identical despite different names*

### Comparing `netbox_software-0.1.4/PKG-INFO` & `netbox_software-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-software
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: izakharov
 Author-email: ilya.zakharov@domrf.ru
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

