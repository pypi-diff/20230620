# Comparing `tmp/stig_edit-1.0.1.tar.gz` & `tmp/stig_edit-1.0.5.tar.gz`

## Comparing `stig_edit-1.0.1.tar` & `stig_edit-1.0.5.tar`

### file list

```diff
@@ -1,9 +1,13 @@
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 stig_edit-1.0.1/src/stig_edit/__init__.py
--rwxr-xr-x   0        0        0      977 2020-02-02 00:00:00.000000 stig_edit-1.0.1/src/stig_edit/checks.py
--rwxr-xr-x   0        0        0     3681 2020-02-02 00:00:00.000000 stig_edit-1.0.1/src/stig_edit/ckl_editor.py
--rwxr-xr-x   0        0        0  2134108 2020-02-02 00:00:00.000000 stig_edit-1.0.1/tests/test.ckl
--rwxr-xr-x   0        0        0      705 2020-02-02 00:00:00.000000 stig_edit-1.0.1/tests/test_main.py
--rwxr-xr-x   0        0        0     1086 2020-02-02 00:00:00.000000 stig_edit-1.0.1/LICENSE
--rwxr-xr-x   0        0        0     7678 2020-02-02 00:00:00.000000 stig_edit-1.0.1/README.md
--rwxr-xr-x   0        0        0      625 2020-02-02 00:00:00.000000 stig_edit-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     8081 2020-02-02 00:00:00.000000 stig_edit-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    21235 2020-02-02 00:00:00.000000 stig_edit-1.0.5/.pylintrc
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 stig_edit-1.0.5/.github/workflows/merge.yml
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 stig_edit-1.0.5/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 stig_edit-1.0.5/stig_edit/__init__.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 stig_edit-1.0.5/stig_edit/ckl_editor.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 stig_edit-1.0.5/stig_edit/handler.py
+-rw-r--r--   0        0        0  2134120 2020-02-02 00:00:00.000000 stig_edit-1.0.5/tests/test.ckl
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 stig_edit-1.0.5/tests/test_stig_edit.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 stig_edit-1.0.5/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 stig_edit-1.0.5/LICENSE
+-rw-r--r--   0        0        0     5865 2020-02-02 00:00:00.000000 stig_edit-1.0.5/README.md
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 stig_edit-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 stig_edit-1.0.5/PKG-INFO
```

### Comparing `stig_edit-1.0.1/tests/test.ckl` & `stig_edit-1.0.5/tests/test.ckl`

 * *Files 0% similar despite different names*

#### Comparing `stig_edit-1.0.1/tests/test.ckl` & `stig_edit-1.0.5/tests/test.ckl`

```diff
@@ -347,15 +347,15 @@
         <STIG_DATA>
           <VULN_ATTRIBUTE>CCI_REF</VULN_ATTRIBUTE>
           <ATTRIBUTE_DATA>CCI-000366</ATTRIBUTE_DATA>
         </STIG_DATA>
         <STATUS>Not_Reviewed</STATUS>
         <FINDING_DETAILS>Server was patched.
 This is not a finding</FINDING_DETAILS>
-        <COMMENTS>No Comment.</COMMENTS>
+        <COMMENTS>This is a test comment.</COMMENTS>
         <SEVERITY_OVERRIDE/>
         <SEVERITY_JUSTIFICATION/>
       </VULN>
       <VULN>
         <STIG_DATA>
           <VULN_ATTRIBUTE>Vuln_Num</VULN_ATTRIBUTE>
           <ATTRIBUTE_DATA>V-230223</ATTRIBUTE_DATA>
```

### Comparing `stig_edit-1.0.1/LICENSE` & `stig_edit-1.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 FourHole
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 FourHole
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `stig_edit-1.0.1/README.md` & `stig_edit-1.0.5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -51,71 +51,31 @@
 import ckl_editor
 print(ckl_editor.read_target_data("test.ckl"))
 ```
     
 
 ---
 
-### **load_vkey_data**(*filename*)
-
-This module loads all available vkeys that can be passed to the *write_vkey_data()* module to ensure that you do not try to edit a vkey that does not exists in the stig file you are parsing. 
-
-You should run this before running the *write_vkey_data()* module or use it as an input into it.
-
-| Parameters        | Description                                               | Examples         | Required |
-|:------------------|:----------------------------------------------------------|:-----------------|:---------|
-| filename          | Filename of CKL file to parse.                            | testfile.txt     | yes
-
-#### Example
-```python
-import ckl_editor
-
-vkeylist = ckl_editor.load_vkey_data("test.ckl")
-```
-
----
-
-### **load_target_data**(*file_name*)
-
-This is used to load all of the available target data for the STIG.
-
-You should run this before running the *write_target_data()* or use it as an input into it
-
-| Parameters        | Description                                               | Examples         | Required |
-|:------------------|:----------------------------------------------------------|:-----------------|:---------|
-| filename          | Filename of CKL file to parse.                            | testfile.txt     | yes
-
-#### Example
-```python
-import ckl_editor
-
-target_values=ckl_editor.load_target_data("test.ckl")
-```
----
-
 ### **write_target_data**(*file_name*, *key*, *value*, *target_list*)
 
 This module can write to any of the Target Data fields shown in the *Editable Fields/Target Data* section. Note the values because some fields must match a list of predefined values or the STIG Viewer will not be able to open the file.
 
 Before running this module, you need to run the *load_target_data()* module and use that as the input for target_list. 
 
 | Parameters        | Description                                               | Examples         | Required |
 |:------------------|:----------------------------------------------------------|:-----------------|:---------|
 | filename          | Filename of CKL file to parse.                            | testfile.txt     | yes      
 | key               | Target field name that you want to edit                   | ROLE             | yes      
 | value             | The value that you want to set the target field to        | Workstation      | yes      
-| target_list       | The list of editable targets from *load_target_data()*    | load_target_data("test.txt")| yes
 
 #### Example
 ```python
 import ckl_editor
 
-target_values=ckl_editor.load_target_data("test.ckl")
-
-ckl_editor.write_target_data(file_name="test.ckl", key="ROLE", value="Member Server",target_list=target_values)
+ckl_editor.write_target_data(file_name="test.ckl", key="ROLE", value="Member Server")
 ```
 
 ---
 
 ### **write_vkey_data**(*file_name*, *key*, *status*, *finding_details*, *comments*, *vkeylist*)
 
 This module can write status, finding_details, and comments to any vkey that exists in your CKL file. It will error out if the vkey does not exists. Some of the fileds such as status have a list of predefined values you must use or the STIG Viewer will not be able to open the file.
@@ -125,18 +85,15 @@
 | Parameters        | Description                                            | Examples         | Required |
 |:------------------|:-------------------------------------------------------|:-----------------|:---------|
 | filename          | Filename of CKL file to parse.                         | testfile.txt     | yes      
 | key               | The vkey that you want to edit in the checklist        | V-230222         | yes      
 | status            | The value that you want to set the status to.          | NotAFinding      | yes     
 | finding_details   | Any information you want to put in the finding details | The check returned no results.| yes   
 | comments          | Any information you want to put in the comments        | Fixed on July 4, 1776 | yes    
-| vkeylist          | The list of editable vkeys from *load_vkey_data()*     | load_vkey_data("test.txt")| yes
 
 ```python
 import ckl_editor
 
-vkeylist = ckl_editor.load_vkey_data("test.ckl")
-
-ckl_editor.write_vkey_data(file_name="test.ckl", key="V-230222", status="Not_Reviewed", finding_details="Server was patched.\nThis is not a finding", comments="No Comment.", vkeylist=vkeylist)
+ckl_editor.write_vkey_data(file_name="test.ckl", key="V-230222", status="Not_Reviewed", finding_details="Server was patched.\nThis is not a finding", comments="No Comment.")
 ```
 
 ---
```

### Comparing `stig_edit-1.0.1/pyproject.toml` & `stig_edit-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "stig_edit"
-version = "1.0.1"
+version = "1.0.5"
 authors = [
   { name="fourhole", email="fourhole7@gmail.com" },
 ]
 description = "A small package that allows you to easily edit STIG (CKL files) quickly."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `stig_edit-1.0.1/PKG-INFO` & `stig_edit-1.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stig_edit
-Version: 1.0.1
+Version: 1.0.5
 Summary: A small package that allows you to easily edit STIG (CKL files) quickly.
 Project-URL: Homepage, https://github.com/FourHole/stig_edit
 Project-URL: Bug Tracker, https://github.com/FourHole/stig_edit/issues
 Author-email: fourhole <fourhole7@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -65,71 +65,31 @@
 import ckl_editor
 print(ckl_editor.read_target_data("test.ckl"))
 ```
     
 
 ---
 
-### **load_vkey_data**(*filename*)
-
-This module loads all available vkeys that can be passed to the *write_vkey_data()* module to ensure that you do not try to edit a vkey that does not exists in the stig file you are parsing. 
-
-You should run this before running the *write_vkey_data()* module or use it as an input into it.
-
-| Parameters        | Description                                               | Examples         | Required |
-|:------------------|:----------------------------------------------------------|:-----------------|:---------|
-| filename          | Filename of CKL file to parse.                            | testfile.txt     | yes
-
-#### Example
-```python
-import ckl_editor
-
-vkeylist = ckl_editor.load_vkey_data("test.ckl")
-```
-
----
-
-### **load_target_data**(*file_name*)
-
-This is used to load all of the available target data for the STIG.
-
-You should run this before running the *write_target_data()* or use it as an input into it
-
-| Parameters        | Description                                               | Examples         | Required |
-|:------------------|:----------------------------------------------------------|:-----------------|:---------|
-| filename          | Filename of CKL file to parse.                            | testfile.txt     | yes
-
-#### Example
-```python
-import ckl_editor
-
-target_values=ckl_editor.load_target_data("test.ckl")
-```
----
-
 ### **write_target_data**(*file_name*, *key*, *value*, *target_list*)
 
 This module can write to any of the Target Data fields shown in the *Editable Fields/Target Data* section. Note the values because some fields must match a list of predefined values or the STIG Viewer will not be able to open the file.
 
 Before running this module, you need to run the *load_target_data()* module and use that as the input for target_list. 
 
 | Parameters        | Description                                               | Examples         | Required |
 |:------------------|:----------------------------------------------------------|:-----------------|:---------|
 | filename          | Filename of CKL file to parse.                            | testfile.txt     | yes      
 | key               | Target field name that you want to edit                   | ROLE             | yes      
 | value             | The value that you want to set the target field to        | Workstation      | yes      
-| target_list       | The list of editable targets from *load_target_data()*    | load_target_data("test.txt")| yes
 
 #### Example
 ```python
 import ckl_editor
 
-target_values=ckl_editor.load_target_data("test.ckl")
-
-ckl_editor.write_target_data(file_name="test.ckl", key="ROLE", value="Member Server",target_list=target_values)
+ckl_editor.write_target_data(file_name="test.ckl", key="ROLE", value="Member Server")
 ```
 
 ---
 
 ### **write_vkey_data**(*file_name*, *key*, *status*, *finding_details*, *comments*, *vkeylist*)
 
 This module can write status, finding_details, and comments to any vkey that exists in your CKL file. It will error out if the vkey does not exists. Some of the fileds such as status have a list of predefined values you must use or the STIG Viewer will not be able to open the file.
@@ -139,18 +99,15 @@
 | Parameters        | Description                                            | Examples         | Required |
 |:------------------|:-------------------------------------------------------|:-----------------|:---------|
 | filename          | Filename of CKL file to parse.                         | testfile.txt     | yes      
 | key               | The vkey that you want to edit in the checklist        | V-230222         | yes      
 | status            | The value that you want to set the status to.          | NotAFinding      | yes     
 | finding_details   | Any information you want to put in the finding details | The check returned no results.| yes   
 | comments          | Any information you want to put in the comments        | Fixed on July 4, 1776 | yes    
-| vkeylist          | The list of editable vkeys from *load_vkey_data()*     | load_vkey_data("test.txt")| yes
 
 ```python
 import ckl_editor
 
-vkeylist = ckl_editor.load_vkey_data("test.ckl")
-
-ckl_editor.write_vkey_data(file_name="test.ckl", key="V-230222", status="Not_Reviewed", finding_details="Server was patched.\nThis is not a finding", comments="No Comment.", vkeylist=vkeylist)
+ckl_editor.write_vkey_data(file_name="test.ckl", key="V-230222", status="Not_Reviewed", finding_details="Server was patched.\nThis is not a finding", comments="No Comment.")
 ```
 
 ---
```

