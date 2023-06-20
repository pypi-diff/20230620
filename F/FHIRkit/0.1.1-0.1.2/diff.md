# Comparing `tmp/FHIRkit-0.1.1.tar.gz` & `tmp/FHIRkit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FHIRkit-0.1.1.tar", last modified: Tue Jun 13 08:27:43 2023, max compression
+gzip compressed data, was "FHIRkit-0.1.2.tar", last modified: Tue Jun 20 06:34:32 2023, max compression
```

## Comparing `FHIRkit-0.1.1.tar` & `FHIRkit-0.1.2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 charlottedevlieghere   (501) staff       (20)        0 2023-06-13 08:27:43.160193 FHIRkit-0.1.1/
-drwxr-xr-x   0 charlottedevlieghere   (501) staff       (20)        0 2023-06-13 08:27:43.131153 FHIRkit-0.1.1/FHIRkit.egg-info/
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2476 2023-06-13 08:27:43.000000 FHIRkit-0.1.1/FHIRkit.egg-info/PKG-INFO
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1696 2023-06-13 08:27:43.000000 FHIRkit-0.1.1/FHIRkit.egg-info/SOURCES.txt
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)        1 2023-06-13 08:27:43.000000 FHIRkit-0.1.1/FHIRkit.egg-info/dependency_links.txt
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)       23 2023-06-13 08:27:43.000000 FHIRkit-0.1.1/FHIRkit.egg-info/requires.txt
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)       13 2023-06-13 08:27:43.000000 FHIRkit-0.1.1/FHIRkit.egg-info/top_level.txt
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1094 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/LICENSE.md
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2476 2023-06-13 08:27:43.159877 FHIRkit-0.1.1/PKG-INFO
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2029 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/README.md
-drwxr-xr-x   0 charlottedevlieghere   (501) staff       (20)        0 2023-06-13 08:27:43.149657 FHIRkit-0.1.1/fhirkit/
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      519 2022-12-22 10:38:55.000000 FHIRkit-0.1.1/fhirkit/AllergyIntolerance.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     4080 2023-04-10 09:45:08.000000 FHIRkit-0.1.1/fhirkit/BaseModel.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1774 2022-12-22 10:38:55.000000 FHIRkit-0.1.1/fhirkit/Bundle.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      291 2023-06-13 07:52:05.000000 FHIRkit-0.1.1/fhirkit/CarePlan.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      275 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/CareTeam.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1806 2023-01-15 15:30:45.000000 FHIRkit-0.1.1/fhirkit/ClinicalImpression.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     5490 2023-06-13 07:52:07.000000 FHIRkit-0.1.1/fhirkit/CodeSystem.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2722 2023-01-27 09:58:51.000000 FHIRkit-0.1.1/fhirkit/Composition.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      381 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/CompositionValueSet.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     5527 2023-02-17 17:20:01.000000 FHIRkit-0.1.1/fhirkit/Condition.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1020 2023-04-27 13:46:13.000000 FHIRkit-0.1.1/fhirkit/Coverage.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      269 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/Device.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1614 2023-01-13 16:13:41.000000 FHIRkit-0.1.1/fhirkit/DiagnosticReport.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      302 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/DocumentReference.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     8049 2023-02-17 17:20:01.000000 FHIRkit-0.1.1/fhirkit/Encounter.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      287 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/ImagingStudy.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      287 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/Immunization.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1591 2022-10-20 12:40:00.000000 FHIRkit-0.1.1/fhirkit/Location.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      281 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/Medication.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      337 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/MedicationAdministration.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      302 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/MedicationRequest.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      322 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/MedicationStatement.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     3658 2023-06-13 07:52:05.000000 FHIRkit-0.1.1/fhirkit/Observation.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1286 2022-10-24 13:24:49.000000 FHIRkit-0.1.1/fhirkit/OperationOutcome.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2440 2023-05-22 08:57:29.000000 FHIRkit-0.1.1/fhirkit/Organization.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2120 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/Parameter.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     3496 2023-04-13 07:10:47.000000 FHIRkit-0.1.1/fhirkit/Patient.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2547 2023-02-17 17:20:01.000000 FHIRkit-0.1.1/fhirkit/Practitioner.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     3791 2023-02-17 17:20:01.000000 FHIRkit-0.1.1/fhirkit/PractitionerRole.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     5966 2023-04-10 09:33:00.000000 FHIRkit-0.1.1/fhirkit/Procedure.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      281 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/Provenance.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2943 2023-05-22 08:59:19.000000 FHIRkit-0.1.1/fhirkit/Resource.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2828 2023-02-17 17:19:01.000000 FHIRkit-0.1.1/fhirkit/Server.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)    10578 2023-04-13 07:11:11.000000 FHIRkit-0.1.1/fhirkit/SimpleFHIRStore.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      293 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/SupplyDelivery.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      650 2022-12-22 10:38:55.000000 FHIRkit-0.1.1/fhirkit/TerminologyServer.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     6228 2023-06-13 07:52:07.000000 FHIRkit-0.1.1/fhirkit/ValueSet.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1842 2023-06-13 07:52:05.000000 FHIRkit-0.1.1/fhirkit/__init__.py
-drwxr-xr-x   0 charlottedevlieghere   (501) staff       (20)        0 2023-06-13 08:27:43.154351 FHIRkit-0.1.1/fhirkit/choice_type/
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)       83 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/choice_type/__init__.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     5630 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/choice_type/choice_type.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1207 2022-12-22 10:38:55.000000 FHIRkit-0.1.1/fhirkit/choice_type/validators.py
-drwxr-xr-x   0 charlottedevlieghere   (501) staff       (20)        0 2023-06-13 08:27:43.155946 FHIRkit-0.1.1/fhirkit/elements/
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1583 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/elements/Timing.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      926 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/elements/UsageContext.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)       90 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/elements/__init__.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)    10875 2023-06-13 07:52:07.000000 FHIRkit-0.1.1/fhirkit/elements/elements.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1075 2023-02-17 17:20:01.000000 FHIRkit-0.1.1/fhirkit/metadata_types.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      495 2022-12-22 10:38:55.000000 FHIRkit-0.1.1/fhirkit/parse.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     7228 2023-05-22 08:59:19.000000 FHIRkit-0.1.1/fhirkit/primitive_datatypes.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)  2467556 2023-06-13 08:03:49.000000 FHIRkit-0.1.1/fhirkit/r4.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)  3105532 2023-06-13 07:52:07.000000 FHIRkit-0.1.1/fhirkit/r5.py
-drwxr-xr-x   0 charlottedevlieghere   (501) staff       (20)        0 2023-06-13 08:27:43.157372 FHIRkit-0.1.1/fhirkit/snomed/
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     4697 2023-02-17 17:19:01.000000 FHIRkit-0.1.1/fhirkit/snomed/ValueSet.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      125 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/snomed/__init__.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)       35 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/fhirkit/snomed/consts.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1648 2023-01-13 08:53:58.000000 FHIRkit-0.1.1/fhirkit/snomed/elements.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     8174 2023-02-17 17:19:01.000000 FHIRkit-0.1.1/fhirkit/snomed/terminology.py
-drwxr-xr-x   0 charlottedevlieghere   (501) staff       (20)        0 2023-06-13 08:27:43.158329 FHIRkit-0.1.1/fhirkit/tiro/
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)       34 2023-01-13 08:55:47.000000 FHIRkit-0.1.1/fhirkit/tiro/__init__.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      583 2023-01-20 15:20:02.000000 FHIRkit-0.1.1/fhirkit/tiro/elements.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      336 2023-06-13 07:52:07.000000 FHIRkit-0.1.1/pyproject.toml
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)       38 2023-06-13 08:27:43.160268 FHIRkit-0.1.1/setup.cfg
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      664 2023-06-13 08:27:32.000000 FHIRkit-0.1.1/setup.py
-drwxr-xr-x   0 charlottedevlieghere   (501) staff       (20)        0 2023-06-13 08:27:43.159403 FHIRkit-0.1.1/test/
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)        0 2023-02-17 17:19:01.000000 FHIRkit-0.1.1/test/__init__.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      262 2023-02-20 09:07:12.000000 FHIRkit-0.1.1/test/test_meta.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      455 2022-10-14 12:32:43.000000 FHIRkit-0.1.1/test/test_observation.py
--rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      483 2022-12-22 10:38:55.000000 FHIRkit-0.1.1/test/test_reference.py
+drwxr-xr-x   0 charlottedevlieghere   (501) staff       (20)        0 2023-06-20 06:34:32.918336 FHIRkit-0.1.2/
+drwxr-xr-x   0 charlottedevlieghere   (501) staff       (20)        0 2023-06-20 06:34:32.897861 FHIRkit-0.1.2/FHIRkit.egg-info/
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2476 2023-06-20 06:34:32.000000 FHIRkit-0.1.2/FHIRkit.egg-info/PKG-INFO
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1696 2023-06-20 06:34:32.000000 FHIRkit-0.1.2/FHIRkit.egg-info/SOURCES.txt
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)        1 2023-06-20 06:34:32.000000 FHIRkit-0.1.2/FHIRkit.egg-info/dependency_links.txt
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)       23 2023-06-20 06:34:32.000000 FHIRkit-0.1.2/FHIRkit.egg-info/requires.txt
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)       13 2023-06-20 06:34:32.000000 FHIRkit-0.1.2/FHIRkit.egg-info/top_level.txt
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1094 2022-10-14 12:32:43.000000 FHIRkit-0.1.2/LICENSE.md
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2476 2023-06-20 06:34:32.918103 FHIRkit-0.1.2/PKG-INFO
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2029 2022-10-14 12:32:43.000000 FHIRkit-0.1.2/README.md
+drwxr-xr-x   0 charlottedevlieghere   (501) staff       (20)        0 2023-06-20 06:34:32.912697 FHIRkit-0.1.2/fhirkit/
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      519 2022-12-22 10:38:55.000000 FHIRkit-0.1.2/fhirkit/AllergyIntolerance.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     4080 2023-04-10 09:45:08.000000 FHIRkit-0.1.2/fhirkit/BaseModel.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1774 2022-12-22 10:38:55.000000 FHIRkit-0.1.2/fhirkit/Bundle.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      291 2023-06-13 07:52:05.000000 FHIRkit-0.1.2/fhirkit/CarePlan.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      275 2022-10-14 12:32:43.000000 FHIRkit-0.1.2/fhirkit/CareTeam.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1806 2023-01-15 15:30:45.000000 FHIRkit-0.1.2/fhirkit/ClinicalImpression.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     5490 2023-06-13 07:52:07.000000 FHIRkit-0.1.2/fhirkit/CodeSystem.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2722 2023-01-27 09:58:51.000000 FHIRkit-0.1.2/fhirkit/Composition.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      381 2022-10-14 12:32:43.000000 FHIRkit-0.1.2/fhirkit/CompositionValueSet.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     5527 2023-02-17 17:20:01.000000 FHIRkit-0.1.2/fhirkit/Condition.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1020 2023-04-27 13:46:13.000000 FHIRkit-0.1.2/fhirkit/Coverage.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      269 2022-10-14 12:32:43.000000 FHIRkit-0.1.2/fhirkit/Device.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1614 2023-01-13 16:13:41.000000 FHIRkit-0.1.2/fhirkit/DiagnosticReport.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      302 2022-10-14 12:32:43.000000 FHIRkit-0.1.2/fhirkit/DocumentReference.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     8049 2023-02-17 17:20:01.000000 FHIRkit-0.1.2/fhirkit/Encounter.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      287 2022-10-14 12:32:43.000000 FHIRkit-0.1.2/fhirkit/ImagingStudy.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      287 2022-10-14 12:32:43.000000 FHIRkit-0.1.2/fhirkit/Immunization.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1591 2022-10-20 12:40:00.000000 FHIRkit-0.1.2/fhirkit/Location.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      281 2022-10-14 12:32:43.000000 FHIRkit-0.1.2/fhirkit/Medication.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      337 2022-10-14 12:32:43.000000 FHIRkit-0.1.2/fhirkit/MedicationAdministration.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      302 2022-10-14 12:32:43.000000 FHIRkit-0.1.2/fhirkit/MedicationRequest.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      322 2022-10-14 12:32:43.000000 FHIRkit-0.1.2/fhirkit/MedicationStatement.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     3658 2023-06-13 07:52:05.000000 FHIRkit-0.1.2/fhirkit/Observation.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1286 2022-10-24 13:24:49.000000 FHIRkit-0.1.2/fhirkit/OperationOutcome.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2440 2023-05-22 08:57:29.000000 FHIRkit-0.1.2/fhirkit/Organization.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2120 2022-10-14 12:32:43.000000 FHIRkit-0.1.2/fhirkit/Parameter.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     3496 2023-04-13 07:10:47.000000 FHIRkit-0.1.2/fhirkit/Patient.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2547 2023-02-17 17:20:01.000000 FHIRkit-0.1.2/fhirkit/Practitioner.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     3791 2023-02-17 17:20:01.000000 FHIRkit-0.1.2/fhirkit/PractitionerRole.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     5966 2023-04-10 09:33:00.000000 FHIRkit-0.1.2/fhirkit/Procedure.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      281 2022-10-14 12:32:43.000000 FHIRkit-0.1.2/fhirkit/Provenance.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2943 2023-05-22 08:59:19.000000 FHIRkit-0.1.2/fhirkit/Resource.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     2828 2023-02-17 17:19:01.000000 FHIRkit-0.1.2/fhirkit/Server.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)    10578 2023-04-13 07:11:11.000000 FHIRkit-0.1.2/fhirkit/SimpleFHIRStore.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      293 2022-10-14 12:32:43.000000 FHIRkit-0.1.2/fhirkit/SupplyDelivery.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      650 2022-12-22 10:38:55.000000 FHIRkit-0.1.2/fhirkit/TerminologyServer.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     6228 2023-06-13 07:52:07.000000 FHIRkit-0.1.2/fhirkit/ValueSet.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1842 2023-06-13 07:52:05.000000 FHIRkit-0.1.2/fhirkit/__init__.py
+drwxr-xr-x   0 charlottedevlieghere   (501) staff       (20)        0 2023-06-20 06:34:32.915239 FHIRkit-0.1.2/fhirkit/choice_type/
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)       83 2022-10-14 12:32:43.000000 FHIRkit-0.1.2/fhirkit/choice_type/__init__.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     5630 2022-10-14 12:32:43.000000 FHIRkit-0.1.2/fhirkit/choice_type/choice_type.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1207 2022-12-22 10:38:55.000000 FHIRkit-0.1.2/fhirkit/choice_type/validators.py
+drwxr-xr-x   0 charlottedevlieghere   (501) staff       (20)        0 2023-06-20 06:34:32.915808 FHIRkit-0.1.2/fhirkit/elements/
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1583 2022-10-14 12:32:43.000000 FHIRkit-0.1.2/fhirkit/elements/Timing.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      926 2022-10-14 12:32:43.000000 FHIRkit-0.1.2/fhirkit/elements/UsageContext.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)       90 2022-10-14 12:32:43.000000 FHIRkit-0.1.2/fhirkit/elements/__init__.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)    10875 2023-06-13 07:52:07.000000 FHIRkit-0.1.2/fhirkit/elements/elements.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1075 2023-02-17 17:20:01.000000 FHIRkit-0.1.2/fhirkit/metadata_types.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      495 2022-12-22 10:38:55.000000 FHIRkit-0.1.2/fhirkit/parse.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     7228 2023-05-22 08:59:19.000000 FHIRkit-0.1.2/fhirkit/primitive_datatypes.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)  2467556 2023-06-13 08:03:49.000000 FHIRkit-0.1.2/fhirkit/r4.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)  3105532 2023-06-13 07:52:07.000000 FHIRkit-0.1.2/fhirkit/r5.py
+drwxr-xr-x   0 charlottedevlieghere   (501) staff       (20)        0 2023-06-20 06:34:32.916635 FHIRkit-0.1.2/fhirkit/snomed/
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     4697 2023-02-17 17:19:01.000000 FHIRkit-0.1.2/fhirkit/snomed/ValueSet.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      125 2022-10-14 12:32:43.000000 FHIRkit-0.1.2/fhirkit/snomed/__init__.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)       35 2022-10-14 12:32:43.000000 FHIRkit-0.1.2/fhirkit/snomed/consts.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     1648 2023-01-13 08:53:58.000000 FHIRkit-0.1.2/fhirkit/snomed/elements.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)     8174 2023-02-17 17:19:01.000000 FHIRkit-0.1.2/fhirkit/snomed/terminology.py
+drwxr-xr-x   0 charlottedevlieghere   (501) staff       (20)        0 2023-06-20 06:34:32.917231 FHIRkit-0.1.2/fhirkit/tiro/
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)       34 2023-01-13 08:55:47.000000 FHIRkit-0.1.2/fhirkit/tiro/__init__.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      583 2023-01-20 15:20:02.000000 FHIRkit-0.1.2/fhirkit/tiro/elements.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      336 2023-06-20 06:34:29.000000 FHIRkit-0.1.2/pyproject.toml
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)       38 2023-06-20 06:34:32.918390 FHIRkit-0.1.2/setup.cfg
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      664 2023-06-20 06:34:31.000000 FHIRkit-0.1.2/setup.py
+drwxr-xr-x   0 charlottedevlieghere   (501) staff       (20)        0 2023-06-20 06:34:32.917855 FHIRkit-0.1.2/test/
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)        0 2023-02-17 17:19:01.000000 FHIRkit-0.1.2/test/__init__.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      262 2023-02-20 09:07:12.000000 FHIRkit-0.1.2/test/test_meta.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      455 2022-10-14 12:32:43.000000 FHIRkit-0.1.2/test/test_observation.py
+-rw-r--r--   0 charlottedevlieghere   (501) staff       (20)      483 2022-12-22 10:38:55.000000 FHIRkit-0.1.2/test/test_reference.py
```

### Comparing `FHIRkit-0.1.1/FHIRkit.egg-info/PKG-INFO` & `FHIRkit-0.1.2/FHIRkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FHIRkit
-Version: 0.1.1
+Version: 0.1.2
 Summary: Toolkit to handle FHIR Resources in a more efficient, pythonic way.
 Home-page: 
 Author: 
 Author-email: 
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Healthcare Industry
```

### Comparing `FHIRkit-0.1.1/FHIRkit.egg-info/SOURCES.txt` & `FHIRkit-0.1.2/FHIRkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/LICENSE.md` & `FHIRkit-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/PKG-INFO` & `FHIRkit-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FHIRkit
-Version: 0.1.1
+Version: 0.1.2
 Summary: Toolkit to handle FHIR Resources in a more efficient, pythonic way.
 Home-page: 
 Author: 
 Author-email: 
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Healthcare Industry
```

### Comparing `FHIRkit-0.1.1/README.md` & `FHIRkit-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/AllergyIntolerance.py` & `FHIRkit-0.1.2/fhirkit/AllergyIntolerance.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/BaseModel.py` & `FHIRkit-0.1.2/fhirkit/BaseModel.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/Bundle.py` & `FHIRkit-0.1.2/fhirkit/Bundle.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/ClinicalImpression.py` & `FHIRkit-0.1.2/fhirkit/ClinicalImpression.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/CodeSystem.py` & `FHIRkit-0.1.2/fhirkit/CodeSystem.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/Composition.py` & `FHIRkit-0.1.2/fhirkit/Composition.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/Condition.py` & `FHIRkit-0.1.2/fhirkit/Condition.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/Coverage.py` & `FHIRkit-0.1.2/fhirkit/Coverage.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/DiagnosticReport.py` & `FHIRkit-0.1.2/fhirkit/DiagnosticReport.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/Encounter.py` & `FHIRkit-0.1.2/fhirkit/Encounter.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/Location.py` & `FHIRkit-0.1.2/fhirkit/Location.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/Observation.py` & `FHIRkit-0.1.2/fhirkit/Observation.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/OperationOutcome.py` & `FHIRkit-0.1.2/fhirkit/OperationOutcome.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/Organization.py` & `FHIRkit-0.1.2/fhirkit/Organization.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/Parameter.py` & `FHIRkit-0.1.2/fhirkit/Parameter.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/Patient.py` & `FHIRkit-0.1.2/fhirkit/Patient.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/Practitioner.py` & `FHIRkit-0.1.2/fhirkit/Practitioner.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/PractitionerRole.py` & `FHIRkit-0.1.2/fhirkit/PractitionerRole.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/Procedure.py` & `FHIRkit-0.1.2/fhirkit/Procedure.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/Resource.py` & `FHIRkit-0.1.2/fhirkit/Resource.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/Server.py` & `FHIRkit-0.1.2/fhirkit/Server.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/SimpleFHIRStore.py` & `FHIRkit-0.1.2/fhirkit/SimpleFHIRStore.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/TerminologyServer.py` & `FHIRkit-0.1.2/fhirkit/TerminologyServer.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/ValueSet.py` & `FHIRkit-0.1.2/fhirkit/ValueSet.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/__init__.py` & `FHIRkit-0.1.2/fhirkit/__init__.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/choice_type/choice_type.py` & `FHIRkit-0.1.2/fhirkit/choice_type/choice_type.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/choice_type/validators.py` & `FHIRkit-0.1.2/fhirkit/choice_type/validators.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/elements/Timing.py` & `FHIRkit-0.1.2/fhirkit/elements/Timing.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/elements/UsageContext.py` & `FHIRkit-0.1.2/fhirkit/elements/UsageContext.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/elements/elements.py` & `FHIRkit-0.1.2/fhirkit/elements/elements.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/metadata_types.py` & `FHIRkit-0.1.2/fhirkit/metadata_types.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/primitive_datatypes.py` & `FHIRkit-0.1.2/fhirkit/primitive_datatypes.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/r4.py` & `FHIRkit-0.1.2/fhirkit/r4.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/r5.py` & `FHIRkit-0.1.2/fhirkit/r5.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/snomed/ValueSet.py` & `FHIRkit-0.1.2/fhirkit/snomed/ValueSet.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/snomed/elements.py` & `FHIRkit-0.1.2/fhirkit/snomed/elements.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/snomed/terminology.py` & `FHIRkit-0.1.2/fhirkit/snomed/terminology.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/fhirkit/tiro/elements.py` & `FHIRkit-0.1.2/fhirkit/tiro/elements.py`

 * *Files identical despite different names*

### Comparing `FHIRkit-0.1.1/setup.py` & `FHIRkit-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "Intended Audience :: Healthcare Industry",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
 setup(
     name="FHIRkit",
-    version="0.1.1",
+    version="0.1.2",
     description="Toolkit to handle FHIR Resources in a more efficient, pythonic way.",
     long_description=open("README.md").read(),
     url="",
     author="",
     author_email="",
     license="MIT",
     classifiers=classifiers,
```

