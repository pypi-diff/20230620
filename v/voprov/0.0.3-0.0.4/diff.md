# Comparing `tmp/voprov-0.0.3.tar.gz` & `tmp/voprov-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voprov-0.0.3.tar", last modified: Tue May  2 09:41:57 2023, max compression
+gzip compressed data, was "voprov-0.0.4.tar", last modified: Tue Jun 20 08:41:46 2023, max compression
```

## Comparing `voprov-0.0.3.tar` & `voprov-0.0.4.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:41:57.992111 voprov-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-02 09:41:42.000000 voprov-0.0.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-02 09:41:42.000000 voprov-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-02 09:41:57.992111 voprov-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-02 09:41:42.000000 voprov-0.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 09:41:57.996111 voprov-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-02 09:41:42.000000 voprov-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:41:57.992111 voprov-0.0.3/voprov/
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:41:57.992111 voprov-0.0.3/voprov/models/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/models/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)   105183 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/models/voprovConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (123)    13687 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/models/voprovDescriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/models/voprovRelations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:41:57.992111 voprov-0.0.3/voprov/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11514 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/serializers/provjson.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/serializers/provn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9987 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/serializers/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:41:57.992111 voprov-0.0.3/voprov/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/visualization/dot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-02 09:41:42.000000 voprov-0.0.3/voprov/visualization/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 09:41:57.992111 voprov-0.0.3/voprov.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-02 09:41:57.000000 voprov-0.0.3/voprov.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-02 09:41:57.000000 voprov-0.0.3/voprov.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:41:57.000000 voprov-0.0.3/voprov.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 09:41:57.000000 voprov-0.0.3/voprov.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-02 09:41:57.000000 voprov-0.0.3/voprov.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 09:41:57.000000 voprov-0.0.3/voprov.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:41:46.631804 voprov-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-20 08:41:38.000000 voprov-0.0.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-20 08:41:38.000000 voprov-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-20 08:41:46.631804 voprov-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-20 08:41:38.000000 voprov-0.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 08:41:46.631804 voprov-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-20 08:41:38.000000 voprov-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:41:46.627804 voprov-0.0.4/voprov/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-20 08:41:38.000000 voprov-0.0.4/voprov/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:41:46.627804 voprov-0.0.4/voprov/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-20 08:41:38.000000 voprov-0.0.4/voprov/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-06-20 08:41:38.000000 voprov-0.0.4/voprov/models/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113827 2023-06-20 08:41:38.000000 voprov-0.0.4/voprov/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-20 08:41:38.000000 voprov-0.0.4/voprov/models/voprovConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13687 2023-06-20 08:41:38.000000 voprov-0.0.4/voprov/models/voprovDescriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-20 08:41:38.000000 voprov-0.0.4/voprov/models/voprovRelations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:41:46.627804 voprov-0.0.4/voprov/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-20 08:41:38.000000 voprov-0.0.4/voprov/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11514 2023-06-20 08:41:38.000000 voprov-0.0.4/voprov/serializers/provjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-20 08:41:38.000000 voprov-0.0.4/voprov/serializers/provn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-06-20 08:41:38.000000 voprov-0.0.4/voprov/serializers/voyaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9987 2023-06-20 08:41:38.000000 voprov-0.0.4/voprov/serializers/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:41:46.631804 voprov-0.0.4/voprov/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-20 08:41:38.000000 voprov-0.0.4/voprov/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-06-20 08:41:38.000000 voprov-0.0.4/voprov/visualization/dot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-20 08:41:38.000000 voprov-0.0.4/voprov/visualization/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-06-20 08:41:38.000000 voprov-0.0.4/voprov/visualization/plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:41:46.627804 voprov-0.0.4/voprov.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-20 08:41:46.000000 voprov-0.0.4/voprov.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-20 08:41:46.000000 voprov-0.0.4/voprov.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 08:41:46.000000 voprov-0.0.4/voprov.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 08:41:46.000000 voprov-0.0.4/voprov.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-20 08:41:46.000000 voprov-0.0.4/voprov.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 08:41:46.000000 voprov-0.0.4/voprov.egg-info/top_level.txt
```

### Comparing `voprov-0.0.3/LICENSE` & `voprov-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `voprov-0.0.3/PKG-INFO` & `voprov-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voprov
-Version: 0.0.3
+Version: 0.0.4
 Summary: A library for IVOA Provenance Data Model supporting PROV-JSON, PROV-XML and PROV-N
 Home-page: https://github.com/sanguillon/voprov/
 Author: Benjamin Parciany
 Author-email: benjamin.parciany@obspm.fr
 License: MIT
 Keywords: provenance,graph,model,VOPROV,provenance-dm,PROVENANCE-DM,PROV-JSON,JSON,PROV-XML,PROV-N
 Classifier: Development Status :: 4 - Beta
```

### Comparing `voprov-0.0.3/README.rst` & `voprov-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `voprov-0.0.3/setup.py` & `voprov-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 test_requirements = [
     'pydot>=1.2.0'
 ]
 
 setup(
     name='voprov',
-    version='0.0.3',
+    version='0.0.4',
     description='A library for IVOA Provenance Data Model supporting PROV-JSON, '
                 'PROV-XML and PROV-N',
     long_description=readme,
     author='Benjamin Parciany',
     author_email='benjamin.parciany@obspm.fr',
     url='https://github.com/sanguillon/voprov/',
     packages=find_packages(),
```

### Comparing `voprov-0.0.3/voprov/__init__.py` & `voprov-0.0.4/voprov/__init__.py`

 * *Files identical despite different names*

### Comparing `voprov-0.0.3/voprov/models/constants.py` & `voprov-0.0.4/voprov/models/constants.py`

 * *Files identical despite different names*

### Comparing `voprov-0.0.3/voprov/models/model.py` & `voprov-0.0.4/voprov/models/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import io
 import itertools
 import os
 import logging
 import shutil
 import tempfile
 import dateutil.parser
+import requests
 from prov.model import (ProvException, ProvDocument, ProvBundle, ProvActivity,
                         ProvUsage, ProvAgent, ProvGeneration, ProvAssociation, ProvEntity,
                         ProvCommunication, ProvStart, ProvEnd, ProvInvalidation, ProvDerivation,
                         ProvAttribution, ProvDelegation, ProvInfluence, ProvSpecialization,
                         ProvAlternate, ProvMention, ProvMembership,
                         PROV_REC_CLS, DEFAULT_NAMESPACES, NamespaceManager, first)
 from urllib.parse import urlparse
@@ -183,14 +184,23 @@
             bundle = ProvBundle()
 
         entity = ProvEntity(bundle, self.identifier, self.attributes)
         entity.add_asserted_type(self._prov_type)  # self.__class__.__name__)
 
         return bundle.add_record(entity)
 
+    def add_agent(self, identifier, name=None, type=None, comment=None, email=None, affiliation=None, phone=None,
+              address=None, url=None, other_attributes=None):
+        """add an agent to an entity"""
+        agent = self._bundle.agent(identifier, name, type, comment, email, affiliation, phone,
+              address, url, other_attributes)
+        self._bundle.wasAttributedTo(self, agent)
+        self._bundle.unified()
+        return agent
+
 
 class VOProvValueEntity(VOProvEntity):
     """Class for VOProv Value Entity"""
     _prov_type = VOPROV_VALUE_ENTITY
 
     def set_value(self, value):
         """Set a value for this entity.
@@ -364,21 +374,62 @@
             if value:
                 for super_formal in super(VOProvActivity, self).FORMAL_ATTRIBUTES:
                     if local_part is super_formal.localpart:
                         activity.add_attributes({super_formal: value})
                         break
         return bundle.add_record(activity)
 
-    def add_parameter(self, idbundle, idparam, nameparam, valueparam):
+    def add_parameter(self, idparam, nameparam, valueparam, parameterDescription=None, other_attributes=None):
         """add a parameter to an activity"""
+        idbundle = "#configuration#" + self.identifier._str.replace(":", "#")
         if self._bundle.valid_qualified_name(idbundle) not in self._bundle._bundles:
             bundle_config = self._bundle.bundle(idbundle)
-            param = bundle_config.parameter(idparam, nameparam, valueparam)
-            self._bundle.wasConfiguredBy(self, param)
-
+        else:
+            bundle_config = self._bundle._bundles[self._bundle.valid_qualified_name(idbundle)]
+        param = bundle_config.parameter(idparam, nameparam, valueparam, parameterDescription, other_attributes)
+        self._bundle.wasConfiguredBy(self, param)
+        self._bundle.unified_relations()
+        return param
+
+    def add_configFile(self, idfile, namefile, locationfile, comment=None, configFileDescription=None,
+                       other_attributes=None):
+        """add a configuration file to an activity"""
+        idbundle = "#configuration#" + self.identifier._str.replace(":", "#")
+        if self._bundle.valid_qualified_name(idbundle) not in self._bundle._bundles:
+            bundle_config = self._bundle.bundle(idbundle)
+        else:
+            bundle_config = self._bundle._bundles[self._bundle.valid_qualified_name(idbundle)]
+        file = bundle_config.configFile(idfile, namefile, locationfile, comment, configFileDescription, other_attributes)
+        self._bundle.wasConfiguredBy(self, file, 'ConfigFile')
+        return file
+
+    def add_agent(self, identifier, name=None, type=None, comment=None, email=None, affiliation=None, phone=None,
+                  address=None, url=None, other_attributes=None):
+        """add an agent to an activity"""
+        agent = self._bundle.agent(identifier, name, type, comment, email, affiliation, phone,
+                                   address, url, other_attributes)
+        self._bundle.wasAssociatedWith(self, agent)
+        self._bundle.unified()
+        return agent
+
+    def add_used_entity(self, identifier, name=None, location=None, generatedAtTime=None, invalidatedAtTime=None,
+               comment=None, entityDescription=None, other_attributes=None, time=None, attributes=None):
+        """add a used entity to an activity"""
+        entity = self._bundle.entity(identifier, name, location, generatedAtTime, invalidatedAtTime,
+               comment, entityDescription, other_attributes)
+        self.used(entity, time, attributes)
+        return entity
+
+    def add_generated_entity(self, identifier, name=None, location=None, generatedAtTime=None, invalidatedAtTime=None,
+               comment=None, entityDescription=None, other_attributes=None, time=None, attributes=None):
+        """add a generated entity to an activity"""
+        entity = self._bundle.entity(identifier, name, location, generatedAtTime, invalidatedAtTime,
+               comment, entityDescription, other_attributes)
+        entity.wasGeneratedBy(self, time, attributes)
+        return entity
 
 class VOProvAgent(ProvAgent):
     """Adaptation of Prov Agent class"""
     _prov_type = VOPROV_AGENT
 
     def set_name(self, name):
         """Set the name of this activity.
@@ -915,27 +966,28 @@
         self.add_namespaces(namespaces)
 
 
 class VOProvBundle(ProvBundle):
     """Adaptation of prov bundle to VOProv Bundle"""
 
     def __init__(self, records=None, identifier=None, namespaces=None,
-                 document=None):
+                 document=None, label=""):
         """
         Constructor.
 
         :param records: Optional iterable of records to add to the bundle
             (default: None).
         :param identifier: Optional identifier of the bundle (default: None).
         :param namespaces: Optional iterable of :py:class:`~prov.identifier.Namespace`s
             to set the document up with (default: None).
         :param document: Optional document to add to the bundle (default: None).
         """
         #  Initializing bundle-specific attributes
         super(VOProvBundle, self).__init__(records, identifier, namespaces, document)
+        self.label = label
         self._namespaces = VOProvNamespaceManager(
             namespaces,
             parent=(document._namespaces if document is not None else None)
         )
 
     def unified(self):
         """
@@ -1176,15 +1228,15 @@
                                         attribute is set, the value string can be interpreted by this valueType.
         :param parameterDescription:    Description object or identifier.
         :param other_attributes:        Optional other attributes as a dictionary or list
                                         of tuples to be added to the record optionally (default: None).
         """
         if parameterDescription is not None:
             self.description(identifier, parameterDescription)
-        return self.new_record(VOPROV_CONFIGURATION_PARAMETER, identifier, {
+        return self.new_record(VOPROV_CONFIGURATION_PARAMETER   , identifier, {
             VOPROV_ATTR_NAME: name,
             VOPROV_ATTR_VALUE: value,
             PROV_LABEL: name + " = " + value
         }, other_attributes)
 
     def agent(self, identifier, name=None, type=None, comment=None, email=None, affiliation=None, phone=None,
               address=None, url=None, other_attributes=None):
@@ -2051,14 +2103,90 @@
             VOPROV_REFERENCE_RELATION, identifier, {
                 VOPROV_ATTR_REFERENCED: referenced,
                 VOPROV_ATTR_REFERRER: referrer
             },
             None
         )
 
+    def add_activity_description(self, iddescription, namedescription, version = None, description = None,
+                                 docurl = None, type = None, subtype = None, other_attributes = None):
+        """add a description to an activity"""
+        idbundle = '#description#' + iddescription.replace(":", "#")
+        if self.valid_qualified_name(idbundle) not in self._bundles:
+            bundle_description = self.bundle(idbundle)
+        else:
+            bundle_description = self._bundles[self.valid_qualified_name(idbundle)]
+        return bundle_description.activityDescription(iddescription, namedescription, version, description, docurl, type,
+                                               subtype, other_attributes)
+
+    def add_usage_description(self, identifier, activityDescription, role, description=None, type=None,
+                         multiplicity=None, entityDescription=None, other_attributes=None):
+        """add a description to a usage"""
+        idbundle = '#description#' + activityDescription.replace(":", "#")
+        if self.valid_qualified_name(idbundle) not in self._bundles:
+            bundle_description = self.bundle(idbundle)
+        else:
+            bundle_description = self._bundles[self.valid_qualified_name(idbundle)]
+        return bundle_description.usageDescription(identifier, activityDescription, role, description, type, multiplicity,
+                                               entityDescription, other_attributes)
+
+    def add_generation_description(self, identifier, activityDescription, role, description=None, type=None,
+                              multiplicity=None, entityDescription=None, other_attributes=None):
+        """add a description to a generation"""
+        idbundle = '#description#' + activityDescription.replace(":", "#")
+        if self.valid_qualified_name(idbundle) not in self._bundles:
+            bundle_description = self.bundle(idbundle)
+        else:
+            bundle_description = self._bundles[self.valid_qualified_name(idbundle)]
+        return bundle_description.generationDescription(identifier, activityDescription, role, description, type, multiplicity,
+                                               entityDescription, other_attributes)
+
+    def add_parameter_description(self, identifier, activityDescription, name, valueType, description=None, unit=None,
+                             ucd=None, utype=None, min=None, max=None, options=None, default=None,
+                             other_attributes=None):
+        """add a description to a parameter"""
+        idbundle = '#description#' + activityDescription.replace(":", "#")
+        if self.valid_qualified_name(idbundle) not in self._bundles:
+            bundle_description = self.bundle(idbundle)
+        else:
+            bundle_description = self._bundles[self.valid_qualified_name(idbundle)]
+        return bundle_description.parameterDescription(identifier, activityDescription, name, valueType, description, unit,
+                                               ucd, utype, min, max, options, default, other_attributes)
+
+    def add_one_step(self, onestep):
+        if 'activityDescription' in onestep:
+            self.add_activity_description(onestep['activityDescription'], onestep['activityDescriptionName'])
+            act = self.activity(onestep['activity'], activityDescription=onestep['activityDescription'])
+        else:
+            act = self.activity(onestep['activity'])
+        used = act.add_used_entity(onestep['used'])
+        generated = act.add_generated_entity(onestep['generated'])
+        if 'agentUsedEntity' in onestep:
+            used.add_agent(onestep['agentUsedEntity'])
+        if 'agentGeneratedEntity' in onestep:
+            generated.add_agent(onestep['agentGeneratedEntity'])
+        if 'agentActivity' in onestep:
+            act.add_agent(onestep['agentActivity'])
+        if 'usedEntityDescription' in onestep:
+            self.add_entity_description(used, onestep['usedEntityDescription'], onestep['usedEntityDescriptionName'])
+            if 'usageDescription' in onestep and 'usageRole' in onestep and 'activityDescription' in onestep:
+                self.add_usage_description(onestep['usageDescription'], onestep['activityDescription'], onestep['usageRole'],
+                                           entityDescription=onestep['usedEntityDescription'])
+        if 'generatedEntityDescription' in onestep:
+            self.add_entity_description(generated, onestep['generatedEntityDescription'], onestep['generatedEntityDescriptionName'])
+            if 'generationDescription' in onestep and 'generationRole' in onestep and 'activityDescription' in onestep:
+                self.add_generation_description(onestep['generationDescription'], onestep['activityDescription'], onestep['generationRole'],
+                                                entityDescription=onestep['generatedEntityDescription'])
+        if 'idParameter' in onestep and 'nameParameter' in onestep and 'valueParameter' in onestep:
+            act.add_parameter(onestep['idParameter'], onestep['nameParameter'], onestep['valueParameter'])
+
+    def get_from_provsap(self, url):
+        r = requests.get(url)
+        return r.json()
+
     # update alias of prov function
     wasGeneratedBy = generation
     used = usage
     wasAttributedTo = attribution
     wasAssociatedWith = association
     wasStartedBy = start
     wasEndedBy = end
@@ -2078,14 +2206,16 @@
     # alias for voprov's function
     isDescribedBy = description
     isRelatedTo = relate
     wasConfiguredBy = configuration
     hadReference = reference
 
 
+
+
 class VOProvDocument(ProvDocument, VOProvBundle):
     """Adaptation of prov document to VOProvenance Document."""
 
     def __init__(self, records=None, namespaces=None):
         """
         Constructor.
 
@@ -2354,14 +2484,19 @@
         if source is not None:
             if hasattr(source, "read"):
                 return serializer.deserialize(source, **args)
             else:
                 with open(source) as f:
                     return serializer.deserialize(f, **args)
 
+    def add_entity_description(self, identity, iddescription, name, description=None, docurl=None, type=None, other_attributes=None):
+        """add a description to an entity"""
+        description = self.entityDescription(iddescription, name, description, docurl, type, other_attributes)
+        self.description(identity, iddescription)
+
 
 #  adding voprov class to the prov class mappings
 PROV_REC_CLS.update({
     # link prov class to their voprov representation
     VOPROV_ENTITY: VOProvEntity,
     VOPROV_ACTIVITY: VOProvActivity,
     VOPROV_AGENT: VOProvAgent,
```

### Comparing `voprov-0.0.3/voprov/models/voprovConfigurations.py` & `voprov-0.0.4/voprov/models/voprovConfigurations.py`

 * *Files identical despite different names*

### Comparing `voprov-0.0.3/voprov/models/voprovDescriptions.py` & `voprov-0.0.4/voprov/models/voprovDescriptions.py`

 * *Files identical despite different names*

### Comparing `voprov-0.0.3/voprov/models/voprovRelations.py` & `voprov-0.0.4/voprov/models/voprovRelations.py`

 * *Files identical despite different names*

### Comparing `voprov-0.0.3/voprov/serializers/__init__.py` & `voprov-0.0.4/voprov/serializers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,20 +25,22 @@
     @staticmethod
     def load_serializers():
         """Loads all available serializers into the registry."""
         from voprov.serializers.provjson import VOProvJSONSerializer
         from voprov.serializers.provn import VOProvNSerializer
         from voprov.serializers.xml import VOProvXMLSerializer
         from prov.serializers.provrdf import ProvRDFSerializer
+        from voprov.serializers.voyaml import VOProvYAMLSerializer
 
         Registry.serializers = {
             'json': VOProvJSONSerializer,
             'rdf': ProvRDFSerializer,
             'provn': VOProvNSerializer,
-            'xml': VOProvXMLSerializer
+            'xml': VOProvXMLSerializer,
+            'yaml': VOProvYAMLSerializer
         }
 
 
 def get(format_name):
     """
     Returns the serializer class for the specified format. Raises a DoNotExist
     """
```

### Comparing `voprov-0.0.3/voprov/serializers/provjson.py` & `voprov-0.0.4/voprov/serializers/provjson.py`

 * *Files identical despite different names*

### Comparing `voprov-0.0.3/voprov/serializers/provn.py` & `voprov-0.0.4/voprov/serializers/provn.py`

 * *Files identical despite different names*

### Comparing `voprov-0.0.3/voprov/serializers/xml.py` & `voprov-0.0.4/voprov/serializers/xml.py`

 * *Files identical despite different names*

### Comparing `voprov-0.0.3/voprov/visualization/dot.py` & `voprov-0.0.4/voprov/visualization/dot.py`

 * *Files identical despite different names*

### Comparing `voprov-0.0.3/voprov/visualization/graph.py` & `voprov-0.0.4/voprov/visualization/graph.py`

 * *Files identical despite different names*

### Comparing `voprov-0.0.3/voprov.egg-info/PKG-INFO` & `voprov-0.0.4/voprov.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voprov
-Version: 0.0.3
+Version: 0.0.4
 Summary: A library for IVOA Provenance Data Model supporting PROV-JSON, PROV-XML and PROV-N
 Home-page: https://github.com/sanguillon/voprov/
 Author: Benjamin Parciany
 Author-email: benjamin.parciany@obspm.fr
 License: MIT
 Keywords: provenance,graph,model,VOPROV,provenance-dm,PROVENANCE-DM,PROV-JSON,JSON,PROV-XML,PROV-N
 Classifier: Development Status :: 4 - Beta
```

### Comparing `voprov-0.0.3/voprov.egg-info/SOURCES.txt` & `voprov-0.0.4/voprov.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,11 +14,13 @@
 voprov/models/model.py
 voprov/models/voprovConfigurations.py
 voprov/models/voprovDescriptions.py
 voprov/models/voprovRelations.py
 voprov/serializers/__init__.py
 voprov/serializers/provjson.py
 voprov/serializers/provn.py
+voprov/serializers/voyaml.py
 voprov/serializers/xml.py
 voprov/visualization/__init__.py
 voprov/visualization/dot.py
-voprov/visualization/graph.py
+voprov/visualization/graph.py
+voprov/visualization/plotly.py
```

