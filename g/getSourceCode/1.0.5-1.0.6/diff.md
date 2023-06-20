# Comparing `tmp/getSourceCode-1.0.5.tar.gz` & `tmp/getSourceCode-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getSourceCode-1.0.5.tar", last modified: Tue Apr 25 15:28:56 2023, max compression
+gzip compressed data, was "getSourceCode-1.0.6.tar", last modified: Tue Jun 20 12:54:19 2023, max compression
```

## Comparing `getSourceCode-1.0.5.tar` & `getSourceCode-1.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 15:28:56.891213 getSourceCode-1.0.5/
--rw-rw-rw-   0        0        0     7236 2023-04-25 15:28:56.890212 getSourceCode-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     5614 2023-04-10 08:16:44.000000 getSourceCode-1.0.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-25 15:28:56.871693 getSourceCode-1.0.5/getSourceCode/
--rw-rw-rw-   0        0        0    28916 2023-04-25 15:27:34.000000 getSourceCode-1.0.5/getSourceCode/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 15:28:56.887215 getSourceCode-1.0.5/getSourceCode.egg-info/
--rw-rw-rw-   0        0        0     7236 2023-04-25 15:28:56.000000 getSourceCode-1.0.5/getSourceCode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-04-25 15:28:56.000000 getSourceCode-1.0.5/getSourceCode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 15:28:56.000000 getSourceCode-1.0.5/getSourceCode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-25 15:28:56.000000 getSourceCode-1.0.5/getSourceCode.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-04-25 15:28:56.000000 getSourceCode-1.0.5/getSourceCode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 15:28:56.891213 getSourceCode-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      505 2023-04-25 15:28:48.000000 getSourceCode-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:54:19.077324 getSourceCode-1.0.6/
+-rw-rw-rw-   0        0        0     7243 2023-06-20 12:54:19.076315 getSourceCode-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5621 2023-04-25 15:30:55.000000 getSourceCode-1.0.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-20 12:54:19.062685 getSourceCode-1.0.6/getSourceCode/
+-rw-rw-rw-   0        0        0    28924 2023-06-20 12:52:03.000000 getSourceCode-1.0.6/getSourceCode/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:54:19.073324 getSourceCode-1.0.6/getSourceCode.egg-info/
+-rw-rw-rw-   0        0        0     7243 2023-06-20 12:54:18.000000 getSourceCode-1.0.6/getSourceCode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-06-20 12:54:18.000000 getSourceCode-1.0.6/getSourceCode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 12:54:18.000000 getSourceCode-1.0.6/getSourceCode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-20 12:54:18.000000 getSourceCode-1.0.6/getSourceCode.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-06-20 12:54:18.000000 getSourceCode-1.0.6/getSourceCode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 12:54:19.077324 getSourceCode-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      505 2023-06-20 12:53:44.000000 getSourceCode-1.0.6/setup.py
```

### Comparing `getSourceCode-1.0.5/PKG-INFO` & `getSourceCode-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: getSourceCode
-Version: 1.0.5
+Version: 1.0.6
 Summary: Simple way to get contract source code.
 Home-page: https://hxzy.me
 Author: hxzy
 Author-email: hxzy0220@gmail.com
 License: UNKNOWN
 Description: getSourceCode
         =============
@@ -25,15 +25,15 @@
         
             avax-testnet|arbi-testnet|poly-testnet
         
             bsc-testnet|heco-testnet|ftm-testnet
         
             Goerli|Kovan|Rinkeby|Ropsten
         
-            moonbase|boba-testnet
+            moonbase|boba-testnet|gnosis
         
         Get code by tx only supports:
         
         ::
         
             BSC|ETH|BOBA|ARBI|HECO
```

### Comparing `getSourceCode-1.0.5/README.rst` & `getSourceCode-1.0.6/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     avax-testnet|arbi-testnet|poly-testnet
 
     bsc-testnet|heco-testnet|ftm-testnet
 
     Goerli|Kovan|Rinkeby|Ropsten
 
-    moonbase|boba-testnet
+    moonbase|boba-testnet|gnosis
 
 Get code by tx only supports:
 
 ::
 
     BSC|ETH|BOBA|ARBI|HECO
```

### Comparing `getSourceCode-1.0.5/getSourceCode/__init__.py` & `getSourceCode-1.0.6/getSourceCode/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -430,27 +430,29 @@
     global contractIndex
     if "ContractName" not in result.keys():
         return
     try:
         index = 0
         isMultiFile = False
         contractName = result['ContractName']
+
+        print(contractName)
         saveInfo(address, contractName)
         sourceCode = result['SourceCode'].replace("\r\n", "\n")
         if sourceCode.find('.sol":{"content":') != -1:
             isMultiFile = True
         if "\"language\":" in sourceCode or isMultiFile:
             contractFolder = contractName
             mkdir(contractFolder)
             if not isMultiFile:
                 sourceCode = json.loads(sourceCode[1:-1])['sources']
             else:
                 sourceCode = json.loads(sourceCode)
             for key in sourceCode.keys():
-                contractName = key.split(".")[0] + ".sol"
+                contractName = key
                 while os.path.exists(contractFolder + "//" + contractName):
                     contractName = key.split(".")[0] + "_{}".format(index) + ".sol"
                     index += 1
                 index = 0
                 mkdir(os.path.split(contractFolder + "//" + contractName)[0])
                 with open(contractFolder + "//" + contractName, "w+", encoding='utf-8') as fw:
                     fw.write(sourceCode[key]["content"].replace('\r\n', '\n'))
```

### Comparing `getSourceCode-1.0.5/getSourceCode.egg-info/PKG-INFO` & `getSourceCode-1.0.6/getSourceCode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: getSourceCode
-Version: 1.0.5
+Version: 1.0.6
 Summary: Simple way to get contract source code.
 Home-page: https://hxzy.me
 Author: hxzy
 Author-email: hxzy0220@gmail.com
 License: UNKNOWN
 Description: getSourceCode
         =============
@@ -25,15 +25,15 @@
         
             avax-testnet|arbi-testnet|poly-testnet
         
             bsc-testnet|heco-testnet|ftm-testnet
         
             Goerli|Kovan|Rinkeby|Ropsten
         
-            moonbase|boba-testnet
+            moonbase|boba-testnet|gnosis
         
         Get code by tx only supports:
         
         ::
         
             BSC|ETH|BOBA|ARBI|HECO
```

