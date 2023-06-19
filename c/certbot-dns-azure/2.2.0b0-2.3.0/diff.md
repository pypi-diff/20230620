# Comparing `tmp/certbot-dns-azure-2.2.0b0.tar.gz` & `tmp/certbot-dns-azure-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-dns-azure-2.2.0b0.tar", last modified: Tue May 16 20:29:37 2023, max compression
+gzip compressed data, was "certbot-dns-azure-2.3.0.tar", last modified: Mon Jun 19 22:14:54 2023, max compression
```

## Comparing `certbot-dns-azure-2.2.0b0.tar` & `certbot-dns-azure-2.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:29:37.536460 certbot-dns-azure-2.2.0b0/
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-16 20:29:37.536460 certbot-dns-azure-2.2.0b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:29:37.532460 certbot-dns-azure-2.2.0b0/certbot_dns_azure/
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:29:37.532460 certbot-dns-azure-2.2.0b0/certbot_dns_azure/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15391 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure/_internal/dns_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:29:37.532460 certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-16 20:29:37.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-16 20:29:37.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:29:37.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-16 20:29:37.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-16 20:29:37.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 20:29:37.000000 certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:29:37.532460 certbot-dns-azure-2.2.0b0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-16 20:29:37.536460 certbot-dns-azure-2.2.0b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:29:37.532460 certbot-dns-azure-2.2.0b0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-05-16 20:29:34.000000 certbot-dns-azure-2.2.0b0/tests/dns_azure_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:14:54.885394 certbot-dns-azure-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-06-19 22:14:47.000000 certbot-dns-azure-2.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-19 22:14:47.000000 certbot-dns-azure-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-19 22:14:54.885394 certbot-dns-azure-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-19 22:14:47.000000 certbot-dns-azure-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:14:54.885394 certbot-dns-azure-2.3.0/certbot_dns_azure/
+-rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-06-19 22:14:47.000000 certbot-dns-azure-2.3.0/certbot_dns_azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:14:54.885394 certbot-dns-azure-2.3.0/certbot_dns_azure/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-19 22:14:47.000000 certbot-dns-azure-2.3.0/certbot_dns_azure/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15828 2023-06-19 22:14:47.000000 certbot-dns-azure-2.3.0/certbot_dns_azure/_internal/dns_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:14:54.885394 certbot-dns-azure-2.3.0/certbot_dns_azure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-19 22:14:54.000000 certbot-dns-azure-2.3.0/certbot_dns_azure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-19 22:14:54.000000 certbot-dns-azure-2.3.0/certbot_dns_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 22:14:54.000000 certbot-dns-azure-2.3.0/certbot_dns_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-19 22:14:54.000000 certbot-dns-azure-2.3.0/certbot_dns_azure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-19 22:14:54.000000 certbot-dns-azure-2.3.0/certbot_dns_azure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-19 22:14:54.000000 certbot-dns-azure-2.3.0/certbot_dns_azure.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:14:54.885394 certbot-dns-azure-2.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-19 22:14:47.000000 certbot-dns-azure-2.3.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-19 22:14:47.000000 certbot-dns-azure-2.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-19 22:14:47.000000 certbot-dns-azure-2.3.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-06-19 22:14:47.000000 certbot-dns-azure-2.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-19 22:14:47.000000 certbot-dns-azure-2.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-19 22:14:47.000000 certbot-dns-azure-2.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 22:14:47.000000 certbot-dns-azure-2.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-19 22:14:54.885394 certbot-dns-azure-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-19 22:14:47.000000 certbot-dns-azure-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 22:14:54.885394 certbot-dns-azure-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    15566 2023-06-19 22:14:47.000000 certbot-dns-azure-2.3.0/tests/dns_azure_test.py
```

### Comparing `certbot-dns-azure-2.2.0b0/LICENSE.txt` & `certbot-dns-azure-2.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-azure-2.2.0b0/PKG-INFO` & `certbot-dns-azure-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-azure
-Version: 2.2.0b0
+Version: 2.3.0
 Summary: Azure DNS Authenticator plugin for Certbot
 Home-page: https://github.com/binkhq/certbot-dns-azure
 Author: Terry Cain
 Author-email: opensource@bink.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `certbot-dns-azure-2.2.0b0/README.md` & `certbot-dns-azure-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `certbot-dns-azure-2.2.0b0/certbot_dns_azure/__init__.py` & `certbot-dns-azure-2.3.0/certbot_dns_azure/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,14 +77,26 @@
    dns_azure_msi_system_assigned = true
 
    dns_azure_environment = "AzurePublicCloud"
 
    dns_azure_zone1 = example.com:/subscriptions/c135abce-d87d-48df-936c-15596c6968a5/resourceGroups/dns1
    dns_azure_zone2 = example.org:/subscriptions/99800903-fb14-4992-9aff-12eaf2744622/resourceGroups/dns2
 
+.. code-block:: ini
+   :name: certbot_azure_cli.ini
+   :caption: Example config file using Azure CLI credentials:
+
+   dns_azure_use_cli_credentials = true
+
+   dns_azure_environment = "AzurePublicCloud"
+
+   dns_azure_zone1 = example.com:/subscriptions/c135abce-d87d-48df-936c-15596c6968a5/resourceGroups/dns1
+   dns_azure_zone2 = example.org:/subscriptions/99800903-fb14-4992-9aff-12eaf2744622/resourceGroups/dns2
+
+
 The path to this file can be provided interactively or using the
 ``--dns-azure-config`` command-line argument. Certbot records the path
 to this file for use during renewal, but does not store the file's contents.
 
 .. caution::
    You should protect these API credentials as you would the password to your
    Azure account. Users who can read this file can use these credentials
@@ -189,15 +201,15 @@
 .. code-block:: ini
     :name: certbot_azure_moresecure.ini
     :caption: Example configuration snippet for individual record permissions
 
     dns_azure_zone1 = test.foo.com:/subscriptions/c135abce-d87d-48df-936c-15596c6968a/resourceGroups/dns1/providers/Microsoft.Network/dnszones/foo.com/TXT/_acme-validation.test
 
 This will override the zone to foo.com (which ``test`` is already in) and the validation record (though it's overridden to the same thing) but now
-it wont delete said validation record.
+it will not delete said validation record.
 
 
 Generic Certbot Examples
 ------------------------
 
 .. code-block:: bash
    :caption: To acquire a certificate for ``example.com``
```

### Comparing `certbot-dns-azure-2.2.0b0/certbot_dns_azure/_internal/dns_azure.py` & `certbot-dns-azure-2.3.0/certbot_dns_azure/_internal/dns_azure.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os import getenv
 from typing import Dict, Tuple
 
 from azure.mgmt.dns import DnsManagementClient
 from azure.mgmt.dns.models import RecordSet, TxtRecord
 from azure.core.exceptions import HttpResponseError
 from azure.core.utils import CaseInsensitiveDict
-from azure.identity import ClientSecretCredential, ManagedIdentityCredential, CertificateCredential
+from azure.identity import ClientSecretCredential, ManagedIdentityCredential, CertificateCredential, AzureCliCredential
 
 from certbot import errors
 from certbot.plugins import dns_common
 
 logger = logging.getLogger(__name__)
 logging.getLogger('azure').setLevel(logging.WARNING)
 
@@ -68,19 +68,22 @@
         sp_certificate_path = credentials.conf('sp_certificate_path')
         tenant_id = credentials.conf('tenant_id')
         has_sp = all((sp_client_id, any((sp_client_secret, sp_certificate_path)), tenant_id))
 
         msi_client_id = credentials.conf('msi_client_id')
         msi_system_assigned = credentials.conf('msi_system_assigned')
 
-        if not any((has_sp, msi_system_assigned, msi_client_id)):
+        use_azure_cli_creds = credentials.conf('use_cli_credentials')
+
+        if not any((has_sp, msi_system_assigned, msi_client_id, use_azure_cli_creds)):
             raise errors.PluginError('{}: No authentication methods have been '
                                      'configured for Azure DNS. Either configure '
-                                     'a service principal or system/user assigned '
-                                     'managed identity'.format(credentials.confobj.filename))
+                                     'a service principal, system/user assigned '
+                                     'managed identity or configure the use of '
+                                     'azure cli credentials'.format(credentials.confobj.filename))
 
         has_zone_mapping = any((key for key in credentials.confobj.keys() if 'azure_zone' in key))
 
         if not has_zone_mapping:
             raise errors.PluginError('{}: At least one zone mapping needs to be provided,'
                                      ' e.g dns_azure_zone1 = DOMAIN:DNS_ZONE_RESOURCE_GROUP_ID'
                                      ''.format(credentials.confobj.filename))
@@ -122,24 +125,28 @@
 
         # Figure out which credential type we're going to use
         sp_client_id = valid_creds.conf('sp_client_id')
         sp_client_secret = valid_creds.conf('sp_client_secret')
         sp_certificate_path = valid_creds.conf('sp_certificate_path')
         tenant_id = valid_creds.conf('tenant_id')
         msi_client_id = valid_creds.conf('msi_client_id')
+        use_azure_cli_creds = valid_creds.conf('use_cli_credentials')
 
         self.credential = self._get_azure_credentials(
-            sp_client_id, sp_client_secret, sp_certificate_path, tenant_id, msi_client_id, self._aad_endpoint
+            sp_client_id, sp_client_secret, sp_certificate_path, tenant_id, msi_client_id, use_azure_cli_creds, self._aad_endpoint
         )
 
     @staticmethod
-    def _get_azure_credentials(client_id=None, client_secret=None, certificate_path=None, tenant_id=None, msi_client_id=None, aad_endpoint=None):
+    def _get_azure_credentials(client_id=None, client_secret=None, certificate_path=None, tenant_id=None, msi_client_id=None,
+                               use_azure_cli_creds=None, aad_endpoint=None):
         has_sp = all((client_id, client_secret, tenant_id))
         has_sp_cert = all((client_id, certificate_path, tenant_id))
-        if has_sp:
+        if use_azure_cli_creds:
+            return AzureCliCredential(tenant_id=tenant_id)
+        elif has_sp:
             return ClientSecretCredential(
                 client_id=client_id,
                 client_secret=client_secret,
                 tenant_id=tenant_id,
                 authority=aad_endpoint
             )
         elif has_sp_cert:
```

### Comparing `certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/PKG-INFO` & `certbot-dns-azure-2.3.0/certbot_dns_azure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-azure
-Version: 2.2.0b0
+Version: 2.3.0
 Summary: Azure DNS Authenticator plugin for Certbot
 Home-page: https://github.com/binkhq/certbot-dns-azure
 Author: Terry Cain
 Author-email: opensource@bink.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
```

### Comparing `certbot-dns-azure-2.2.0b0/certbot_dns_azure.egg-info/SOURCES.txt` & `certbot-dns-azure-2.3.0/certbot_dns_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certbot-dns-azure-2.2.0b0/docs/Makefile` & `certbot-dns-azure-2.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `certbot-dns-azure-2.2.0b0/docs/conf.py` & `certbot-dns-azure-2.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `certbot-dns-azure-2.2.0b0/docs/index.rst` & `certbot-dns-azure-2.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `certbot-dns-azure-2.2.0b0/docs/make.bat` & `certbot-dns-azure-2.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `certbot-dns-azure-2.2.0b0/setup.py` & `certbot-dns-azure-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages
 from setuptools import setup
 
-version = '2.2.0b0'
+version = '2.3.0'
 
 # azure-mgmt-dns is still the old style SDK, so will change dramatically
 # when they refactor, most notably the credential parts
 install_requires = [
     'azure-identity>=1.11.0',
     'azure-mgmt-dns>=8.0.0',
     'setuptools>=41.6.0',
```

### Comparing `certbot-dns-azure-2.2.0b0/tests/dns_azure_test.py` & `certbot-dns-azure-2.3.0/tests/dns_azure_test.py`

 * *Files identical despite different names*

