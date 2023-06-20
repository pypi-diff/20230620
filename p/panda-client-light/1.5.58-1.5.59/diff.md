# Comparing `tmp/panda_client_light-1.5.58-py2.py3-none-any.whl.zip` & `tmp/panda_client_light-1.5.59-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 155683 bytes, number of entries: 36
+Zip file size: 155883 bytes, number of entries: 36
 -rw-r--r--  2.0 unx    63390 b- defN 20-Feb-02 00:00 pandaclient/AthenaUtils.py
 -rw-r--r--  2.0 unx     2276 b- defN 20-Feb-02 00:00 pandaclient/BookConfig.py
 -rwxr-xr-x  2.0 unx    32382 b- defN 20-Feb-02 00:00 pandaclient/BookGUI.py
--rwxr-xr-x  2.0 unx    62375 b- defN 20-Feb-02 00:00 pandaclient/Client.py
+-rwxr-xr-x  2.0 unx    64164 b- defN 20-Feb-02 00:00 pandaclient/Client.py
 -rwxr-xr-x  2.0 unx     3118 b- defN 20-Feb-02 00:00 pandaclient/FileSpec.py
 -rw-r--r--  2.0 unx     3468 b- defN 20-Feb-02 00:00 pandaclient/Group_argparse.py
 -rwxr-xr-x  2.0 unx    27030 b- defN 20-Feb-02 00:00 pandaclient/JobSpec.py
 -rw-r--r--  2.0 unx    13691 b- defN 20-Feb-02 00:00 pandaclient/LocalJobSpec.py
 -rw-r--r--  2.0 unx    11007 b- defN 20-Feb-02 00:00 pandaclient/LocalJobsetSpec.py
 -rw-r--r--  2.0 unx    10225 b- defN 20-Feb-02 00:00 pandaclient/MiscUtils.py
 -rw-r--r--  2.0 unx    15025 b- defN 20-Feb-02 00:00 pandaclient/MyproxyUtils.py
@@ -28,11 +28,11 @@
 -rw-r--r--  2.0 unx     4163 b- defN 20-Feb-02 00:00 pandaclient/localSpecs.py
 -rw-r--r--  2.0 unx    10226 b- defN 20-Feb-02 00:00 pandaclient/openidc_utils.py
 -rw-r--r--  2.0 unx    10528 b- defN 20-Feb-02 00:00 pandaclient/panda_api.py
 -rw-r--r--  2.0 unx     4975 b- defN 20-Feb-02 00:00 pandaclient/panda_gui.py
 -rw-r--r--  2.0 unx     4025 b- defN 20-Feb-02 00:00 pandaclient/panda_jupyter.py
 -rw-r--r--  2.0 unx     7280 b- defN 20-Feb-02 00:00 pandaclient/pcontainer_core.py
 -rw-r--r--  2.0 unx     4281 b- defN 20-Feb-02 00:00 pandaclient/queryPandaMonUtils.py
-?rw-r--r--  2.0 unx      894 b- defN 20-Feb-02 00:00 panda_client_light-1.5.58.dist-info/METADATA
-?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 panda_client_light-1.5.58.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2992 b- defN 20-Feb-02 00:00 panda_client_light-1.5.58.dist-info/RECORD
-36 files, 657781 bytes uncompressed, 150963 bytes compressed:  77.0%
+?rw-r--r--  2.0 unx      894 b- defN 20-Feb-02 00:00 panda_client_light-1.5.59.dist-info/METADATA
+?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 panda_client_light-1.5.59.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2992 b- defN 20-Feb-02 00:00 panda_client_light-1.5.59.dist-info/RECORD
+36 files, 659570 bytes uncompressed, 151163 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -93,17 +93,17 @@
 
 Filename: pandaclient/pcontainer_core.py
 Comment: 
 
 Filename: pandaclient/queryPandaMonUtils.py
 Comment: 
 
-Filename: panda_client_light-1.5.58.dist-info/METADATA
+Filename: panda_client_light-1.5.59.dist-info/METADATA
 Comment: 
 
-Filename: panda_client_light-1.5.58.dist-info/WHEEL
+Filename: panda_client_light-1.5.59.dist-info/WHEEL
 Comment: 
 
-Filename: panda_client_light-1.5.58.dist-info/RECORD
+Filename: panda_client_light-1.5.59.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pandaclient/Client.py

```diff
@@ -1959,7 +1959,63 @@
             'dataset_types': dataset_types}
     status, output = curl.post(url, data, is_json=True)
     if status != 0:
         return EC_Failed, output
     if output is None:
         return EC_Failed, 'server side error'
     return 0, output
+
+
+# get status of events
+def get_events_status(ids, verbose=False):
+    """Get status of events
+       args:
+          ids: a list of {'task_id': ..., 'panda_id': ...}
+          verbose: True to see verbose message
+       returns:
+          status code
+             0: communication succeeded to the panda server
+           255: communication failure
+          a dictionary of {panda_id: [{event_range_id: status}, ...], ...}
+    """
+    # instantiate curl
+    curl = _Curl()
+    curl.sslCert = _x509()
+    curl.sslKey  = _x509()
+    curl.verbose = verbose
+    # execute
+    url = baseURLSSL + '/get_events_status'
+    data = {'ids': json.dumps(ids)}
+    status, output = curl.post(url, data, is_json=True)
+    if status != 0:
+        return EC_Failed, output
+    if output is None:
+        return EC_Failed, 'server side error'
+    return 0, output
+
+
+# update events
+def update_events(events, verbose=False):
+    """Update events
+       args:
+          events: a list of {'eventRangeID': ..., 'eventStatus': ..., 'errorCode': <optional>}
+          verbose: True to see verbose message
+       returns:
+          status code
+             0: communication succeeded to the panda server
+           255: communication failure
+          a dictionary of {'Returns': a list of returns when updating events, 'Command': commands to jobs, 'StatusCode': 0 for OK})
+    """
+    # instantiate curl
+    curl = _Curl()
+    curl.sslCert = _x509()
+    curl.sslKey  = _x509()
+    curl.verbose = verbose
+    # execute
+    url = baseURLSSL + '/updateEventRanges'
+    data = {'eventRanges': json.dumps(events)}
+    status, output = curl.post(url, data, is_json=True)
+    if status != 0:
+        return EC_Failed, output
+    if output is None:
+        return EC_Failed, 'server side error'
+    return 0, output
```

## pandaclient/PandaToolsPkgInfo.py

```diff
@@ -1 +1 @@
-release_version = "1.5.58"
+release_version = "1.5.59"
```

## Comparing `panda_client_light-1.5.58.dist-info/METADATA` & `panda_client_light-1.5.59.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda-client-light
-Version: 1.5.58
+Version: 1.5.59
 Summary: Lightweight PanDA Client Package installed on PanDA server
 Project-URL: Homepage, https://panda-wms.readthedocs.io/en/latest/
 Author-email: PanDA Team <atlas-adc-panda@cern.ch>
 License-Expression: Apache-2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

## Comparing `panda_client_light-1.5.58.dist-info/RECORD` & `panda_client_light-1.5.59.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 pandaclient/AthenaUtils.py,sha256=KQDQqZ0kfw9jLfkFpgqw68jYlZFKVPedFKmSq8P8lbY,63390
 pandaclient/BookConfig.py,sha256=wM6KSkYDV7Jg-_M5GYckkvI1eysE1Q6U9RFwblmL-BQ,2276
 pandaclient/BookGUI.py,sha256=iM-EyioT5zb_6sECFtjxk_OSE0NZizsN1d46bj7IyYY,32382
-pandaclient/Client.py,sha256=4MlUbkMH7syF4VnkFf2pwsiwK316TN135thN47D3LJs,62375
+pandaclient/Client.py,sha256=xwlzQzX63Mrmqyjg-BvNatPnjU8upjqWFAc_6OEzLBU,64164
 pandaclient/FileSpec.py,sha256=1AMnagDrGZhnIBl4nMVTMASCdvwZoD4cs5weqmCeiwM,3118
 pandaclient/Group_argparse.py,sha256=Pn2qJEH3X_-nOvigsRteFHnWrQSxGPJ8GmTmCX3xR5o,3468
 pandaclient/JobSpec.py,sha256=wMZLot1W_-mnkOtRzXkpBcRA7acVa0ggujaDgj_vUuo,27030
 pandaclient/LocalJobSpec.py,sha256=rVMgk4KVhMY1hjWnsaIL9cWVAZMEKVOnE4vQqz7cHWU,13691
 pandaclient/LocalJobsetSpec.py,sha256=nYQMhKrbCtzm68ZWnEXCs_-mWvATm9XClm514aJ-7cU,11007
 pandaclient/MiscUtils.py,sha256=SQWcqhHOW_tmahjb1zbO62zP-uBcB51SJB4ERyYtt5Y,10225
 pandaclient/MyproxyUtils.py,sha256=7eNIdr6Vt8phcW5FVbt5mZ10I4tZH0n-xAuKBk-GcQI,15025
 pandaclient/PBookCore.py,sha256=134Ubc_RG2SMjmgeNs6s_op-3zpyFFOcNLMqd89f8bs,17679
 pandaclient/PBookScript.py,sha256=zgH4LHQeXkyeM1rxtQ64KN0lFDM3wAqpsRf5QVYzp_I,19506
 pandaclient/PLogger.py,sha256=1R0xMlWsHLdptyb-ewt_o6NVveK07ENmKBoE-NKtyJw,1167
-pandaclient/PandaToolsPkgInfo.py,sha256=_8zoi0uLENvrPC8mHYJ9yXgm7VNeKVTKigp5jrkF-W8,27
+pandaclient/PandaToolsPkgInfo.py,sha256=RsqS2_Hfqg42DVrq0QlwtO01b-s4sn1wTgMi6G1N72U,27
 pandaclient/ParseJobXML.py,sha256=GWdiTXhRZOVIqxUT4laZZ13WQ5HZs4V2PgichtyQ4Ec,15441
 pandaclient/PathenaScript.py,sha256=2KCZMps7gDhkFFJA0vE1f1eS5XBLQl42UwXciIphu3A,104912
 pandaclient/PchainScript.py,sha256=JuDJoegkS82Yggo7_szQVEuePgYp5NHp-_vmxOPovW8,11704
 pandaclient/PcontainerScript.py,sha256=J7EiyUfBmMPHXvdwbPE7t9redP6JhdWmCZa3Yg27fRQ,247
 pandaclient/PdbUtils.py,sha256=TNsmCb___D1JevvocLWMUUKajA10Zo62VjdqDx4-Law,24834
 pandaclient/PhpoScript.py,sha256=SgAFlX4VJSx24A4z4fH6sTwka1CJD2_CAbOxrgVXrwU,27474
 pandaclient/PrunScript.py,sha256=lRGKiskp0USbXv9q4-z3BXLplOnzp4UXjW95QQs9xwU,104663
@@ -27,10 +27,10 @@
 pandaclient/localSpecs.py,sha256=Cx9ZNTaOvFIWbk_u9f7Xg9s_4zJdhyksAeMWNwHKbt0,4163
 pandaclient/openidc_utils.py,sha256=nV4cq1n9jDgGXn8FqoERBDHDnFEJMTYuZ7HqIbWKqaU,10226
 pandaclient/panda_api.py,sha256=eNLVvzBiqjANFbqED_AX-K3UI7tASl0fHml8SAMuIkw,10528
 pandaclient/panda_gui.py,sha256=5nW5RsYaXuDcgsxj8SCXvnrZrC117bg70OBZRXqjIvY,4975
 pandaclient/panda_jupyter.py,sha256=buiC8kGSA_KCaZ9TF6XLbfi0hwHi9d6_npDXitRlkCA,4025
 pandaclient/pcontainer_core.py,sha256=k_HjWhLtGPVtnRgK1yaMzEY0XgiBz3XHZt-rVoLf04c,7280
 pandaclient/queryPandaMonUtils.py,sha256=7NqvwjMAgpJC9re4qKe7W6Zn9E7CRzyL1yHmp9yndsg,4281
-panda_client_light-1.5.58.dist-info/METADATA,sha256=xSrL5eHrqn9AIUlUGyUSty-_saseTbUb2OybfxMxMi0,894
-panda_client_light-1.5.58.dist-info/WHEEL,sha256=z6xSPN0Mo_h_NAjjk0VNneWjIiXMjAF_l8uGkjgc2-A,105
-panda_client_light-1.5.58.dist-info/RECORD,,
+panda_client_light-1.5.59.dist-info/METADATA,sha256=_65WipDhp2CybvdHFp3hvOwJ5CTtMwowlEueeucB_qc,894
+panda_client_light-1.5.59.dist-info/WHEEL,sha256=fagL_Tj29mg80flwlxJNW45nBDbboxF04Tnbc_jt3Bg,105
+panda_client_light-1.5.59.dist-info/RECORD,,
```

