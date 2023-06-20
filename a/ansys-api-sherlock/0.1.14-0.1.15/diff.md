# Comparing `tmp/ansys-api-sherlock-0.1.14.tar.gz` & `tmp/ansys-api-sherlock-0.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-api-sherlock-0.1.14.tar", last modified: Mon Jun 12 14:07:28 2023, max compression
+gzip compressed data, was "ansys-api-sherlock-0.1.15.tar", last modified: Tue Jun 20 14:29:19 2023, max compression
```

## Comparing `ansys-api-sherlock-0.1.14.tar` & `ansys-api-sherlock-0.1.15.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:07:28.270333 ansys-api-sherlock-0.1.14/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-12 14:07:28.270333 ansys-api-sherlock-0.1.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 14:07:28.270333 ansys-api-sherlock-0.1.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:07:28.270333 ansys-api-sherlock-0.1.14/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:07:28.270333 ansys-api-sherlock-0.1.14/src/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:07:28.270333 ansys-api-sherlock-0.1.14/src/ansys/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:07:28.270333 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:07:28.270333 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/
--rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockAnalysisService.proto
--rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockCommonService.proto
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockLayerService.proto
--rw-r--r--   0 runner    (1001) docker     (123)    27755 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockLifeCycleService.proto
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockModelService.proto
--rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockPartsService.proto
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockProjectService.proto
--rw-r--r--   0 runner    (1001) docker     (123)    13290 2023-06-12 14:07:11.000000 ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockStackupService.proto
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 14:07:28.270333 ansys-api-sherlock-0.1.14/src/ansys_api_sherlock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-12 14:07:28.000000 ansys-api-sherlock-0.1.14/src/ansys_api_sherlock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-12 14:07:28.000000 ansys-api-sherlock-0.1.14/src/ansys_api_sherlock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 14:07:28.000000 ansys-api-sherlock-0.1.14/src/ansys_api_sherlock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-12 14:07:28.000000 ansys-api-sherlock-0.1.14/src/ansys_api_sherlock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-12 14:07:28.000000 ansys-api-sherlock-0.1.14/src/ansys_api_sherlock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-12 14:07:28.000000 ansys-api-sherlock-0.1.14/src/ansys_api_sherlock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:29:19.321219 ansys-api-sherlock-0.1.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-20 14:29:00.000000 ansys-api-sherlock-0.1.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-20 14:29:19.321219 ansys-api-sherlock-0.1.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-20 14:29:00.000000 ansys-api-sherlock-0.1.15/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-20 14:29:00.000000 ansys-api-sherlock-0.1.15/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 14:29:19.321219 ansys-api-sherlock-0.1.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-20 14:29:00.000000 ansys-api-sherlock-0.1.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:29:19.317219 ansys-api-sherlock-0.1.15/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:29:19.317219 ansys-api-sherlock-0.1.15/src/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:29:19.317219 ansys-api-sherlock-0.1.15/src/ansys/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:29:19.321219 ansys-api-sherlock-0.1.15/src/ansys/api/sherlock/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 14:29:00.000000 ansys-api-sherlock-0.1.15/src/ansys/api/sherlock/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-20 14:29:00.000000 ansys-api-sherlock-0.1.15/src/ansys/api/sherlock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:29:00.000000 ansys-api-sherlock-0.1.15/src/ansys/api/sherlock/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:29:19.321219 ansys-api-sherlock-0.1.15/src/ansys/api/sherlock/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)    14708 2023-06-20 14:29:00.000000 ansys-api-sherlock-0.1.15/src/ansys/api/sherlock/v0/SherlockAnalysisService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-06-20 14:29:00.000000 ansys-api-sherlock-0.1.15/src/ansys/api/sherlock/v0/SherlockCommonService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-06-20 14:29:00.000000 ansys-api-sherlock-0.1.15/src/ansys/api/sherlock/v0/SherlockLayerService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    27755 2023-06-20 14:29:00.000000 ansys-api-sherlock-0.1.15/src/ansys/api/sherlock/v0/SherlockLifeCycleService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-06-20 14:29:00.000000 ansys-api-sherlock-0.1.15/src/ansys/api/sherlock/v0/SherlockModelService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-06-20 14:29:00.000000 ansys-api-sherlock-0.1.15/src/ansys/api/sherlock/v0/SherlockPartsService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-06-20 14:29:00.000000 ansys-api-sherlock-0.1.15/src/ansys/api/sherlock/v0/SherlockProjectService.proto
+-rw-r--r--   0 runner    (1001) docker     (123)    13290 2023-06-20 14:29:00.000000 ansys-api-sherlock-0.1.15/src/ansys/api/sherlock/v0/SherlockStackupService.proto
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:29:19.321219 ansys-api-sherlock-0.1.15/src/ansys_api_sherlock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-20 14:29:19.000000 ansys-api-sherlock-0.1.15/src/ansys_api_sherlock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-20 14:29:19.000000 ansys-api-sherlock-0.1.15/src/ansys_api_sherlock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:29:19.000000 ansys-api-sherlock-0.1.15/src/ansys_api_sherlock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 14:29:19.000000 ansys-api-sherlock-0.1.15/src/ansys_api_sherlock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 14:29:19.000000 ansys-api-sherlock-0.1.15/src/ansys_api_sherlock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 14:29:19.000000 ansys-api-sherlock-0.1.15/src/ansys_api_sherlock.egg-info/top_level.txt
```

### Comparing `ansys-api-sherlock-0.1.14/LICENSE` & `ansys-api-sherlock-0.1.15/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.14/PKG-INFO` & `ansys-api-sherlock-0.1.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-sherlock
-Version: 0.1.14
-Summary: Autogenerated python gRPC interface package for ansys-api-sherlock, built on 14:07:28 on 12 June 2023
+Version: 0.1.15
+Summary: Autogenerated python gRPC interface package for ansys-api-sherlock, built on 14:29:19 on 20 June 2023
 Home-page: https://github.com/ansys/ansys-api-sherlock
 Author: ANSYS, Inc.
 Author-email: support@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ansys-api-sherlock-0.1.14/README.md` & `ansys-api-sherlock-0.1.15/README.md`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.14/setup.py` & `ansys-api-sherlock-0.1.15/setup.py`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockAnalysisService.proto` & `ansys-api-sherlock-0.1.15/src/ansys/api/sherlock/v0/SherlockAnalysisService.proto`

 * *Files 17% similar despite different names*

```diff
@@ -76,17 +76,17 @@
   	optional string harmonicVibeDamping = 4;			// Modal Damping Ratio(s).
   	optional bool partValidationEnabled = 5;			// Flag indicating if part validation should be performed.
   	optional bool requireMaterialAssignmentEnabled = 6;	// Flag indicating if material assignment is required.
   	optional double analysisTemp = 7;					// Temperature.
   	optional string analysisTempUnits = 8; 				// Temperature units.
   	optional string forceModelRebuild = 9;				// Model Creation. Valid values are "FORCE" or "AUTO"
   	optional bool filterByEventFrequency = 10;			// Flag indicating if harmonic results outside selected event range are imported.
-  	optional double naturalFreqMin = 11;				// Min Frequency. For NX Nastran analysis only.
+  	optional uint32 naturalFreqMin = 11;				// Min Frequency. For NX Nastran analysis only.
   	optional string naturalFreqMinUnits = 12;			// Min Frequency units. For NX Nastran analysis only.
-  	optional double naturalFreqMax = 13;				// Max Frequency. For NX Nastran analysis only.
+  	optional uint32 naturalFreqMax = 13;				// Max Frequency. For NX Nastran analysis only.
   	optional string naturalFreqMaxUnits = 14;			// Max Frequency units. For NX Nastran analysis only.
   	optional bool reuseModalAnalysis = 15;				// Reuse Natural Frequency. For NX Nastran analysis only.
   }
   
   repeated HarmonicVibe harmonicVibeProperties = 2;
 }
 
@@ -236,14 +236,48 @@
     string pcbMaxVerticalUnits			= 10;	// The length units for the maximum vertical mesh size.
     bool quadsPreferred					= 11;	// Indicates that the meshing engine should attempt to generate quad-shaped elements when creating the mesh.
   }
   
   repeated Analysis analyses	= 3;
 }
 
+message UpdateMechanicalShockPropsRequest {
+  string project = 1;										// Project name.
+  
+  message MechanicalShock {
+	string ccaName = 1; 									// CCA name for which the mechanical properties are set.
+	optional ModelSource modelSource = 2;					// Default is GENERATED.
+	optional int32 shockResultCount = 3;					// Mechanical Shock Result Count.
+	optional double criticalShockStrain = 4;				// Critical Shock Strain.
+	optional string criticalShockStrainUnits = 5;			// Critical Shock Strain units.
+	optional bool partValidationEnabled = 6;				// Flag indicating if part validation should be performed.
+	optional bool requireMaterialAssignmentEnabled = 7;		// Flag indicating if material assignment is required.
+	optional string forceModelRebuild = 8;					// Model Creation. Valid values are "FORCE" or "AUTO"
+	optional uint32 naturalFreqMin = 9;						// Min Frequency.
+	optional string naturalFreqMinUnits = 10;				// Min Frequency units.
+	optional uint32 naturalFreqMax = 11;					// Max Frequency.
+	optional string naturalFreqMaxUnits = 12;				// Max Frequency units.
+	optional double analysisTemp = 13;						// Temperature.
+	optional string analysisTempUnits = 14;					// Temperature units.
+  }
+  
+  repeated MechanicalShock mechanicalShockProperties = 2;
+}
+
+/**
+ * Request to list the valid Mechanical shock input fields for the provided model source and user configuration.
+ */
+message GetMechanicalShockInputFieldsRequest {
+  optional ModelSource modelSource = 1;	// Optional model source. Default: GENERATED
+}
+
+message GetMechanicalShockInputFieldsResponse {
+  repeated string fieldName = 1;
+}
+
 service SherlockAnalysisService {
   // Runs one or more Sherlock analysis.
   rpc runAnalysis(RunAnalysisRequest) returns (ReturnCode);
   
   // Run Sherlock strain map analysis.
   rpc runStrainMapAnalysis(RunStrainMapAnalysisRequest) returns (ReturnCode);
   
@@ -255,14 +289,20 @@
   
   // Returns the list of valid Random Vibe input fields for the provided model source and user configuration.
   rpc getRandomVibeInputFields(GetRandomVibeInputFieldsRequest) returns (GetRandomVibeInputFieldsResponse);
   
   // Updates the analysis properties for Random Vibe analysis.
   rpc updateRandomVibeProps(UpdateRandomVibePropsRequest) returns (ReturnCode);
   
+  // Returns the list of valid Mechanical Shock input fields for the provided model source and user configuration.
+  rpc getMechanicalShockInputFields(GetMechanicalShockInputFieldsRequest) returns (GetMechanicalShockInputFieldsResponse);
+ 
+  // Updates the analysis properties for Mechanical Shock analysis.
+  rpc updateMechanicalShockProps(UpdateMechanicalShockPropsRequest) returns (ReturnCode);
+  
   // Returns the list of valid Natural Frequency property fields given the user configuration.
   rpc getNaturalFrequencyInputFields(GetNaturalFrequencyInputFieldsRequest) returns (GetNaturalFrequencyInputFieldsResponse);
   
   // Updates the analysis properties for Natural Frequency analysis.
   rpc updateNaturalFrequencyProps(UpdateNaturalFrequencyPropsRequest) returns (ReturnCode);
   
   // Updates the analysis properties for Thermal Mech analysis
```

### Comparing `ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockCommonService.proto` & `ansys-api-sherlock-0.1.15/src/ansys/api/sherlock/v0/SherlockCommonService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockLayerService.proto` & `ansys-api-sherlock-0.1.15/src/ansys/api/sherlock/v0/SherlockLayerService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockLifeCycleService.proto` & `ansys-api-sherlock-0.1.15/src/ansys/api/sherlock/v0/SherlockLifeCycleService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockModelService.proto` & `ansys-api-sherlock-0.1.15/src/ansys/api/sherlock/v0/SherlockModelService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockPartsService.proto` & `ansys-api-sherlock-0.1.15/src/ansys/api/sherlock/v0/SherlockPartsService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockProjectService.proto` & `ansys-api-sherlock-0.1.15/src/ansys/api/sherlock/v0/SherlockProjectService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.14/src/ansys/api/sherlock/v0/SherlockStackupService.proto` & `ansys-api-sherlock-0.1.15/src/ansys/api/sherlock/v0/SherlockStackupService.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-sherlock-0.1.14/src/ansys_api_sherlock.egg-info/PKG-INFO` & `ansys-api-sherlock-0.1.15/src/ansys_api_sherlock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ansys-api-sherlock
-Version: 0.1.14
-Summary: Autogenerated python gRPC interface package for ansys-api-sherlock, built on 14:07:28 on 12 June 2023
+Version: 0.1.15
+Summary: Autogenerated python gRPC interface package for ansys-api-sherlock, built on 14:29:19 on 20 June 2023
 Home-page: https://github.com/ansys/ansys-api-sherlock
 Author: ANSYS, Inc.
 Author-email: support@ansys.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ansys-api-sherlock-0.1.14/src/ansys_api_sherlock.egg-info/SOURCES.txt` & `ansys-api-sherlock-0.1.15/src/ansys_api_sherlock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

