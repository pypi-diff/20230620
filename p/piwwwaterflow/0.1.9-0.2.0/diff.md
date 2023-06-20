# Comparing `tmp/piwwwaterflow-0.1.9.tar.gz` & `tmp/piwwwaterflow-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piwwwaterflow-0.1.9.tar", last modified: Sat Jun 17 14:35:08 2023, max compression
+gzip compressed data, was "piwwwaterflow-0.2.0.tar", last modified: Tue Jun 20 07:30:24 2023, max compression
```

## Comparing `piwwwaterflow-0.1.9.tar` & `piwwwaterflow-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:08.734823 piwwwaterflow-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-17 14:35:08.734823 piwwwaterflow-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:08.730823 piwwwaterflow-0.1.9/piwwwaterflow/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:08.730823 piwwwaterflow-0.1.9/piwwwaterflow/static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/static/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:08.730823 piwwwaterflow-0.1.9/piwwwaterflow/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/static/css/iepngfix.htc
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/static/css/view.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:08.734823 piwwwaterflow-0.1.9/piwwwaterflow/static/img/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/static/img/blank.gif
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/static/img/bottom.png
--rw-r--r--   0 runner    (1001) docker     (123)    33683 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/static/img/icon-256.png
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/static/img/icon-32.png
--rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/static/img/piwaterflow.svg
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/static/img/play.png
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/static/img/shadow.gif
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/static/img/top.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:08.734823 piwwwaterflow-0.1.9/piwwwaterflow/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)    10461 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/static/js/code.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:08.734823 piwwwaterflow-0.1.9/piwwwaterflow/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/templates/form.html
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/webservice.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/piwwwaterflow/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:08.730823 piwwwaterflow-0.1.9/piwwwaterflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-17 14:35:08.000000 piwwwaterflow-0.1.9/piwwwaterflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-17 14:35:08.000000 piwwwaterflow-0.1.9/piwwwaterflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 14:35:08.000000 piwwwaterflow-0.1.9/piwwwaterflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-17 14:35:08.000000 piwwwaterflow-0.1.9/piwwwaterflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-17 14:35:08.000000 piwwwaterflow-0.1.9/piwwwaterflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 14:35:08.734823 piwwwaterflow-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 14:35:08.734823 piwwwaterflow-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-17 14:34:55.000000 piwwwaterflow-0.1.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:30:24.686527 piwwwaterflow-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-20 07:30:24.686527 piwwwaterflow-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:30:24.682527 piwwwaterflow-0.2.0/piwwwaterflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:30:24.686527 piwwwaterflow-0.2.0/piwwwaterflow/static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/static/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:30:24.686527 piwwwaterflow-0.2.0/piwwwaterflow/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/static/css/iepngfix.htc
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/static/css/view.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:30:24.686527 piwwwaterflow-0.2.0/piwwwaterflow/static/img/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/static/img/blank.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/static/img/bottom.png
+-rw-r--r--   0 runner    (1001) docker     (123)    33683 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/static/img/icon-256.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/static/img/icon-32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10541 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/static/img/piwaterflow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/static/img/play.png
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/static/img/shadow.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/static/img/top.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:30:24.686527 piwwwaterflow-0.2.0/piwwwaterflow/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    11612 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/static/js/code.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:30:24.686527 piwwwaterflow-0.2.0/piwwwaterflow/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/templates/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/webservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/piwwwaterflow/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:30:24.686527 piwwwaterflow-0.2.0/piwwwaterflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-20 07:30:24.000000 piwwwaterflow-0.2.0/piwwwaterflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-20 07:30:24.000000 piwwwaterflow-0.2.0/piwwwaterflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 07:30:24.000000 piwwwaterflow-0.2.0/piwwwaterflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-20 07:30:24.000000 piwwwaterflow-0.2.0/piwwwaterflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-20 07:30:24.000000 piwwwaterflow-0.2.0/piwwwaterflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 07:30:24.686527 piwwwaterflow-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:30:24.686527 piwwwaterflow-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 07:30:12.000000 piwwwaterflow-0.2.0/tests/__init__.py
```

### Comparing `piwwwaterflow-0.1.9/PKG-INFO` & `piwwwaterflow-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwwwaterflow
-Version: 0.1.9
+Version: 0.2.0
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwwwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # piwwwaterflow
         Flask/Gunicorn Webservice for piwaterflow system
```

### Comparing `piwwwaterflow-0.1.9/piwwwaterflow/static/css/iepngfix.htc` & `piwwwaterflow-0.2.0/piwwwaterflow/static/css/iepngfix.htc`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.9/piwwwaterflow/static/css/view.css` & `piwwwaterflow-0.2.0/piwwwaterflow/static/css/view.css`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.9/piwwwaterflow/static/img/icon-256.png` & `piwwwaterflow-0.2.0/piwwwaterflow/static/img/icon-256.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.9/piwwwaterflow/static/img/icon-32.png` & `piwwwaterflow-0.2.0/piwwwaterflow/static/img/icon-32.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.9/piwwwaterflow/static/img/piwaterflow.svg` & `piwwwaterflow-0.2.0/piwwwaterflow/static/img/piwaterflow.svg`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.9/piwwwaterflow/static/img/play.png` & `piwwwaterflow-0.2.0/piwwwaterflow/static/img/play.png`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.9/piwwwaterflow/static/js/code.js` & `piwwwaterflow-0.2.0/piwwwaterflow/static/js/code.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,9 @@
 var forceTriggersEnabled = true
 
-var socket = io();
-
 function _setEnableForceTriggers(enable) {
     forceTriggersEnabled = enable
 }
 
 function getProgramName(index) {
     return document.getElementById('program' + (index + 1) + 'trigger').textContent
 }
@@ -82,41 +80,37 @@
             return original.replaceAt(start, 10, 'Tomorrow')
         } else {
             return original
         }
     }
 }
 
-socket.on('connect', function() {
-    update(true);
-});
-
-socket.on('disconnect', function() {
-    //document.cookie = "token=; expires=Thu, 01 Jan 1970 00:00:00 UTC; ";
-    location.reload();
-});
+update(true);
 
 setInterval("update(false);", 30000);
 
 function update(first_time) {
-    socket.emit('service_request', function service(response) {
-        // Version label update
+    let requestservice = new XMLHttpRequest();
+    // Add timestamp to avoid caching
+    requestservice.open('GET', '/service?' + (new Date()).getTime());
+    requestservice.responseType = 'json';
+    requestservice.onload = function() {
         var versionlabel = document.getElementById('version');
-        frontend = response.version_frontend
-        backend = response.version_backend
+        frontend = requestservice.response.version_frontend
+        backend = requestservice.response.version_backend
         versionlabel.textContent = `PiWaterflow ${frontend} (Backend ${backend})`
 
         // Status line update
         now = new Date()
         formattedNow = _datestringFromDate(now).slice(0, 10)
         tomorrow = new Date(now.getTime())
         tomorrow.setDate(now.getDate() + 1)
         formattedTomorrow = _datestringFromDate(tomorrow).slice(0, 10)
 
-        lastlooptime = new Date(response.lastlooptime)
+        lastlooptime = new Date(requestservice.response.lastlooptime)
 
         formattedLastLoopDate = _datestringFromDate(lastlooptime)
 
         // Remove date info, if its today... and keep only time info
         if (formattedLastLoopDate.slice(0, 10) == formattedNow)
             formattedLastLoopDate = formattedLastLoopDate.slice(11, )
 
@@ -132,15 +126,15 @@
         }
 
         // Log textarea update
         logtextarea = document.getElementById("log");
         atbottom = ((logtextarea.scrollHeight - logtextarea.scrollTop) <= logtextarea.clientHeight);
 
         var newlines = "";
-        var lines = response.log.split('\n');
+        var lines = requestservice.response.log.split('\n');
 
         for (var i = 0; i < lines.length; i++) {
             if (lines[i].slice(20, 24) == 'Next') {
                 newstring = _readableDay(lines[i], 34, 44, formattedNow, formattedTomorrow)
                 newstring = _readableDay(newstring, 0, 10, formattedNow, formattedTomorrow)
             } else {
                 newstring = _readableDay(lines[i], 0, 10, formattedNow, formattedTomorrow)
@@ -149,22 +143,22 @@
         }
 
         logtextarea.value = newlines;
         if (atbottom)
             logtextarea.scrollTop = logtextarea.scrollHeight;
 
         // Stop button update
-        if (response.stop == false)
+        if (requestservice.response.stop == false)
             document.getElementById('stop').disabled = false
         else
             document.getElementById('stop').disabled = true
 
         // Force triggers update
         _resetForceTriggers();
-        var forcedObj = response.forced;
+        var forcedObj = requestservice.response.forced;
         if (forcedObj != null) {
             _setEnableForceTriggers(false);
 
             if (forcedObj.type == 'program') {
                 if (forcedObj.value == 0)
                     _activateForceTrigger("program1trigger");
                 else
@@ -176,15 +170,15 @@
                     _activateForceTrigger("valve2trigger");
             }
         } else {
             _setEnableForceTriggers(true)
         }
 
         // Controls update
-        var configObj = response.config;
+        var configObj = requestservice.response.config;
         if (configObj != null) {
             time1 = document.getElementById("time1");
             if (!time1.changed)
                 time1.value = configObj.programs[0].start_time;
             valve11 = document.getElementById("valve11");
             if (!valve11.changed)
                 valve11.value = configObj.programs[0].valves[0].time
@@ -215,50 +209,81 @@
                 document.getElementById('valve1trigger').textContent = configObj.programs[0].valves[0].name;
                 document.getElementById('valve2trigger').textContent = configObj.programs[0].valves[1].name;
 
                 saveCurrentValues();
                 refreshSaveButton();
             }
         }
-    });
+    };
+    requestservice.send();
 }
 
 function forceProgram(control, program_forced) {
     if (forceTriggersEnabled && confirm("Are you sure you want to force program?.")) {
-        socket.emit('force', {
-            'type': 'program',
-            'value': program_forced
-        });
+        let requestservice = new XMLHttpRequest();
+        requestservice.open('POST', '/force');
+        requestservice.responseType = 'text';
+        requestservice.onload = function() {
+            if (requestservice.response == 'false') {
+
+            }
+        }
+        var data = new FormData();
+        data.append('type', 'program');
+        data.append('value', program_forced);
+
+        requestservice.send(data);
+
         control.style.color = '#22FF22'
         _setEnableForceTriggers(false)
     } else {
         control.checked = false
     }
 }
 
 function forceValve(control, valve_forced) {
     if (forceTriggersEnabled && confirm("Are you sure you want to force valve?.")) {
-        socket.emit('force', {
-            'type': 'valve',
-            'value': valve_forced
-        });
+        let requestservice = new XMLHttpRequest();
+        requestservice.open('POST', '/force');
+        requestservice.responseType = 'text';
+        requestservice.onload = function() {
+            if (requestservice.response == 'false') {
+
+            }
+        }
+        var data = new FormData();
+        data.append('type', 'valve');
+        data.append('value', valve_forced);
+
+        requestservice.send(data);
         control.style.color = '#22FF22'
         _setEnableForceTriggers(false)
     } else {
         control.checked = false
     }
 }
 
 function stopWaterflow(button) {
-    socket.emit('stop');
+    let requestservice = new XMLHttpRequest();
+    requestservice.open('POST', '/stop');
+    requestservice.send();
     button.disabled = true;
 }
 
 function save(button) {
-    socket.emit('save', [{
+    let requestservice = new XMLHttpRequest();
+    requestservice.open('POST', '/force');
+    requestservice.responseType = 'text';
+    requestservice.onload = function() {
+        if (requestservice.response == 'false') {
+
+        }
+    }
+    var data = new FormData();
+    data.append('save', [{
         'name': getProgramName(0),
         'time': document.getElementById("time1").value,
         'valves': [{
             'name': getValveName(0),
             'time': parseInt(document.getElementById("valve11").value)
         }, {
             'name': getValveName(1),
@@ -279,8 +304,9 @@
     }], function ack(result) {
         if (result) {
             saveCurrentValues();
             refreshSaveButton();
             button.disabled = true;
         }
     });
+    requestservice.send();
 }
```

### Comparing `piwwwaterflow-0.1.9/piwwwaterflow/templates/form.html` & `piwwwaterflow-0.2.0/piwwwaterflow/templates/form.html`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.9/piwwwaterflow/webservice.py` & `piwwwaterflow-0.2.0/piwwwaterflow/webservice.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """ Webservice to control and manage the piwaterflow loop """
 from datetime import datetime
 
 from flask import Flask, render_template, request
 from flask_compress import Compress
-from flask_socketio import SocketIO
 from importlib_metadata import version, PackageNotFoundError
 
 from piwaterflow import Waterflow
 from log_mgr import Logger, LoggerMode
 from revproxy_auth import RevProxyAuth
 
 
@@ -20,21 +19,23 @@
         self.logger.info("Launching piwwwaterflow...")
         self.waterflow = Waterflow()
 
         self.app = Flask(__name__,  template_folder=template_folder, static_folder=static_folder)
 
         self.revproxy_auth = RevProxyAuth(self.app, root_class='piwwwaterflow')
 
-        self.app.add_url_rule('/', 'index', self.waterflow_endpoint, methods=['GET', 'POST'])
+        self.app.add_url_rule('/', 'waterflow', self.waterflow_endpoint, methods=['GET', 'POST'])
+
+        self.app.add_url_rule('/service', 'service', self.on_service_request, methods=['GET'])
+        self.app.add_url_rule('/force', 'force', self.on_force, methods=['GET', 'POST'])
+        self.app.add_url_rule('/stop', 'stop', self.on_stop, methods=['GET', 'POST'])
+        self.app.add_url_rule('/save', 'save', self.on_save, methods=['POST'])
+
         Compress(self.app)
-        self.socketio = SocketIO(self.app, cors_allowed_origins='*')
-        self.socketio.on_event('service_request', self.on_service_request)
-        self.socketio.on_event('force', self.on_force)
-        self.socketio.on_event('stop', self.on_stop)
-        self.socketio.on_event('save', self.on_save)
+        self.waterflow = Waterflow()
 
     @classmethod
     def class_name(cls):
         """ class name """
         return "piwwwaterflow"
 
     def get_app(self):
@@ -42,16 +43,15 @@
         Returns:
             WSGI app:
         """
         return self.app
 
     def run(self):
         """ Run function """
-        # self.app.run()
-        self.socketio.run(self.app)
+        self.app.run()
 
     def waterflow_endpoint(self):
         """ Main endpoint that returns the main page for piwaterflow
         Returns:
             response: The main html content
         """
         return self.revproxy_auth.get_auth_response(request, lambda : render_template('form.html'))
@@ -93,31 +93,41 @@
 
     def on_force(self, data: dict):
         """ On force action request
         Args:
             data (dict): 'type': Must be 'valve' or 'program'
                          'value': Must be the index of the program or value to be forced
         """
-        print(f'Force requested... {data}')
-        type_force = data['type']
-        value_force = data['value']
-        self.waterflow.force(type_force, value_force)
+        if request.method == 'POST':
+            print(f'Force requested... {data}')
+            type_force = request.form.get['type']
+            value_force = request.form.get['value']
+            self.waterflow.force(type_force, value_force)
+        else:
+            forced_data = self.waterflow.get_forced_info()
+            return forced_data
+            # return json.dumps(forced_data)
 
     def on_stop(self):
         """ Event to stop current operation """
-        print('Stop requested...')
-        self.waterflow.stop()
+        if request.method == 'POST':
+            print('Stop requested...')
+            self.waterflow.stop()
+        else:
+            stop_requested = self.waterflow.stop_requested()
+            return "true" if stop_requested else "false"
 
-    def on_save(self, data):
+    def on_save(self):
         """ Event to save the changes in the watering system schedulling
         Args:
             data (dict): Information about the required schedulling
         Returns:
             bool: If everything went ok
         """
+        data = request.form.get['save']
         parsed_config = self.waterflow.config.get_dict_copy()
         for program, update in zip(parsed_config['programs'], data):
             self._change_program(program, update)
 
         self.waterflow.update_config(programs=parsed_config['programs'])
         return True
```

### Comparing `piwwwaterflow-0.1.9/piwwwaterflow/wsgi.py` & `piwwwaterflow-0.2.0/piwwwaterflow/wsgi.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """ WSGI entry point """
 from pathlib import Path
 import os
 
 from piwwwaterflow import PiWWWaterflowService
 
-def create_service():
+def _create_service():
     """ Instantiation of the webservice
     Returns:
        Webservice class instantiated
     """
     templates_path = os.path.join(Path(__file__).parent.resolve(), 'templates')
     static_path = os.path.join(Path(__file__).parent.resolve(), 'static')
     return PiWWWaterflowService(template_folder=templates_path, static_folder=static_path)
 
 def create_app():
     """ Creates a WSGI standard callable function
     Returns:
         WSGI app provided by the PiWWWaterflowService/Flask
     """
-    wtf_service = create_service()
+    wtf_service = _create_service()
     return wtf_service.get_app()
 
 # __main__ used for standalone execution (debugging). For WSGI call, the "wsgi:create_app()" function should be called
 if __name__ == '__main__':
-    service = create_service()
-    service.socketio.run(service.app, host='0.0.0.0', port=5000, debug=True, use_reloader=False)
+    service = create_app()
+    service.run()
```

### Comparing `piwwwaterflow-0.1.9/piwwwaterflow.egg-info/PKG-INFO` & `piwwwaterflow-0.2.0/piwwwaterflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwwwaterflow
-Version: 0.1.9
+Version: 0.2.0
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwwwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # piwwwaterflow
         Flask/Gunicorn Webservice for piwaterflow system
```

### Comparing `piwwwaterflow-0.1.9/piwwwaterflow.egg-info/SOURCES.txt` & `piwwwaterflow-0.2.0/piwwwaterflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piwwwaterflow-0.1.9/setup.py` & `piwwwaterflow-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="piwwwaterflow",
-    version="0.1.9",
+    version="0.2.0",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Raspberry Pi Waterflow resilient system",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/piwwwaterflow",
     packages=setuptools.find_packages(),
@@ -24,12 +24,12 @@
     install_requires=[
         'Flask>=1.1.2',
         'flask-compress>=1.9.0',
         'importlib-metadata>=4.5.0',
         'python-socketio>=5.8.0',
         'flask-socketio>=5.3.3',
         'eventlet==0.30.2', # Exact version required 0.30.2
-        'piwaterflow>=0.5.11',
+        'piwaterflow>=0.6.0',
         'revproxy_auth>=0.1.7'
     ],
     python_requires='>=3.6',
 )
```

