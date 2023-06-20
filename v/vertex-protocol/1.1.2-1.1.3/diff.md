# Comparing `tmp/vertex_protocol-1.1.2.tar.gz` & `tmp/vertex_protocol-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertex_protocol-1.1.2.tar", max compression
+gzip compressed data, was "vertex_protocol-1.1.3.tar", max compression
```

## Comparing `vertex_protocol-1.1.2.tar` & `vertex_protocol-1.1.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     3337 2023-06-19 14:36:59.082668 vertex_protocol-1.1.2/README.md
--rw-r--r--   0        0        0     1664 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/__init__.py
--rw-r--r--   0        0        0     6634 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/client/__init__.py
--rw-r--r--   0        0        0      580 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/client/apis/__init__.py
--rw-r--r--   0        0        0     1394 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/client/apis/base.py
--rw-r--r--   0        0        0     1108 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/client/apis/market/__init__.py
--rw-r--r--   0        0        0     3404 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/client/apis/market/execute.py
--rw-r--r--   0        0        0    10101 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/client/apis/market/query.py
--rw-r--r--   0        0        0      746 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/client/apis/perp/__init__.py
--rw-r--r--   0        0        0     1438 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/client/apis/perp/query.py
--rw-r--r--   0        0        0     1027 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/client/apis/spot/__init__.py
--rw-r--r--   0        0        0     1191 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/client/apis/spot/base.py
--rw-r--r--   0        0        0     4782 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/client/apis/spot/execute.py
--rw-r--r--   0        0        0     2964 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/client/apis/spot/query.py
--rw-r--r--   0        0        0     1307 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/client/apis/subaccount/__init__.py
--rw-r--r--   0        0        0     2023 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/client/apis/subaccount/execute.py
--rw-r--r--   0        0        0     3193 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/client/apis/subaccount/query.py
--rw-r--r--   0        0        0     2554 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/client/context.py
--rw-r--r--   0        0        0     8264 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/contracts/__init__.py
--rw-r--r--   0        0        0    11702 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/contracts/abis/Endpoint.json
--rw-r--r--   0        0        0    55374 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/contracts/abis/FQuerier.json
--rw-r--r--   0        0        0    16980 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/contracts/abis/IClearinghouse.json
--rw-r--r--   0        0        0     3385 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/contracts/abis/IERC20.json
--rw-r--r--   0        0        0     4723 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/contracts/abis/IEndpoint.json
--rw-r--r--   0        0        0    13112 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/contracts/abis/IOffchainBook.json
--rw-r--r--   0        0        0    21812 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/contracts/abis/IPerpEngine.json
--rw-r--r--   0        0        0     8410 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/contracts/abis/IProductEngine.json
--rw-r--r--   0        0        0    18858 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/contracts/abis/ISpotEngine.json
--rw-r--r--   0        0        0     5698 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/contracts/abis/MockERC20.json
--rw-r--r--   0        0        0     1013 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json
--rw-r--r--   0        0        0      993 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json
--rw-r--r--   0        0        0      908 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/contracts/deployments/deployment.test.json
--rw-r--r--   0        0        0      426 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/contracts/eip712/__init__.py
--rw-r--r--   0        0        0     1189 2023-06-19 14:36:59.086668 vertex_protocol-1.1.2/vertex_protocol/contracts/eip712/domain.py
--rw-r--r--   0        0        0     2484 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/contracts/eip712/sign.py
--rw-r--r--   0        0        0     4636 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/contracts/eip712/types.py
--rw-r--r--   0        0        0     1526 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/contracts/loader.py
--rw-r--r--   0        0        0     2747 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/contracts/types.py
--rw-r--r--   0        0        0     1127 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/engine_client/__init__.py
--rw-r--r--   0        0        0    18498 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/engine_client/execute.py
--rw-r--r--   0        0        0    11206 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/engine_client/query.py
--rw-r--r--   0        0        0     5739 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/engine_client/types/__init__.py
--rw-r--r--   0        0        0    18440 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/engine_client/types/execute.py
--rw-r--r--   0        0        0     3429 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/engine_client/types/models.py
--rw-r--r--   0        0        0     9841 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/engine_client/types/query.py
--rw-r--r--   0        0        0      926 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/indexer_client/__init__.py
--rw-r--r--   0        0        0    11233 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/indexer_client/query.py
--rw-r--r--   0        0        0     2979 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/indexer_client/types/__init__.py
--rw-r--r--   0        0        0     5625 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/indexer_client/types/models.py
--rw-r--r--   0        0        0    12117 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/indexer_client/types/query.py
--rw-r--r--   0        0        0      933 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/utils/__init__.py
--rw-r--r--   0        0        0      341 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/utils/backend.py
--rw-r--r--   0        0        0     5301 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/utils/bytes32.py
--rw-r--r--   0        0        0       99 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/utils/enum.py
--rw-r--r--   0        0        0     1136 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/utils/exceptions.py
--rw-r--r--   0        0        0     1094 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/utils/expiration.py
--rw-r--r--   0        0        0      927 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/utils/math.py
--rw-r--r--   0        0        0     2089 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/utils/model.py
--rw-r--r--   0        0        0      753 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/utils/nonce.py
--rw-r--r--   0        0        0      503 2023-06-19 14:36:59.090668 vertex_protocol-1.1.2/vertex_protocol/utils/subaccount.py
--rw-r--r--   0        0        0     4119 1970-01-01 00:00:00.000000 vertex_protocol-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3337 2023-06-20 02:41:13.736585 vertex_protocol-1.1.3/README.md
+-rw-r--r--   0        0        0     1664 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/__init__.py
+-rw-r--r--   0        0        0     6634 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/__init__.py
+-rw-r--r--   0        0        0      580 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/__init__.py
+-rw-r--r--   0        0        0     1394 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/base.py
+-rw-r--r--   0        0        0     1108 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/market/__init__.py
+-rw-r--r--   0        0        0     3404 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/market/execute.py
+-rw-r--r--   0        0        0    10101 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/market/query.py
+-rw-r--r--   0        0        0      746 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/perp/__init__.py
+-rw-r--r--   0        0        0     1438 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/perp/query.py
+-rw-r--r--   0        0        0     1027 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/spot/__init__.py
+-rw-r--r--   0        0        0     1191 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/spot/base.py
+-rw-r--r--   0        0        0     4782 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/spot/execute.py
+-rw-r--r--   0        0        0     2964 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/spot/query.py
+-rw-r--r--   0        0        0     1307 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/subaccount/__init__.py
+-rw-r--r--   0        0        0     2023 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/subaccount/execute.py
+-rw-r--r--   0        0        0     3193 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/apis/subaccount/query.py
+-rw-r--r--   0        0        0     2554 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/client/context.py
+-rw-r--r--   0        0        0     8264 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/__init__.py
+-rw-r--r--   0        0        0    11702 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/abis/Endpoint.json
+-rw-r--r--   0        0        0    55374 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/abis/FQuerier.json
+-rw-r--r--   0        0        0    16980 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/abis/IClearinghouse.json
+-rw-r--r--   0        0        0     3385 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/abis/IERC20.json
+-rw-r--r--   0        0        0     4723 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/abis/IEndpoint.json
+-rw-r--r--   0        0        0    13112 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/abis/IOffchainBook.json
+-rw-r--r--   0        0        0    21812 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/abis/IPerpEngine.json
+-rw-r--r--   0        0        0     8410 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/abis/IProductEngine.json
+-rw-r--r--   0        0        0    18858 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/abis/ISpotEngine.json
+-rw-r--r--   0        0        0     5698 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/abis/MockERC20.json
+-rw-r--r--   0        0        0     1013 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json
+-rw-r--r--   0        0        0      993 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json
+-rw-r--r--   0        0        0      908 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/deployments/deployment.test.json
+-rw-r--r--   0        0        0      426 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/eip712/__init__.py
+-rw-r--r--   0        0        0     1189 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/eip712/domain.py
+-rw-r--r--   0        0        0     2484 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/eip712/sign.py
+-rw-r--r--   0        0        0     4636 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/eip712/types.py
+-rw-r--r--   0        0        0     1526 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/loader.py
+-rw-r--r--   0        0        0     2747 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/contracts/types.py
+-rw-r--r--   0        0        0     1127 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/engine_client/__init__.py
+-rw-r--r--   0        0        0    18498 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/engine_client/execute.py
+-rw-r--r--   0        0        0    11206 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/engine_client/query.py
+-rw-r--r--   0        0        0     5739 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/engine_client/types/__init__.py
+-rw-r--r--   0        0        0    18440 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/engine_client/types/execute.py
+-rw-r--r--   0        0        0     3429 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/engine_client/types/models.py
+-rw-r--r--   0        0        0     9841 2023-06-20 02:41:13.740585 vertex_protocol-1.1.3/vertex_protocol/engine_client/types/query.py
+-rw-r--r--   0        0        0      926 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/indexer_client/__init__.py
+-rw-r--r--   0        0        0    11233 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/indexer_client/query.py
+-rw-r--r--   0        0        0     2979 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/indexer_client/types/__init__.py
+-rw-r--r--   0        0        0     5625 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/indexer_client/types/models.py
+-rw-r--r--   0        0        0    12117 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/indexer_client/types/query.py
+-rw-r--r--   0        0        0      933 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/utils/__init__.py
+-rw-r--r--   0        0        0      341 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/utils/backend.py
+-rw-r--r--   0        0        0     5301 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/utils/bytes32.py
+-rw-r--r--   0        0        0       99 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/utils/enum.py
+-rw-r--r--   0        0        0     1136 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/utils/exceptions.py
+-rw-r--r--   0        0        0     1094 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/utils/expiration.py
+-rw-r--r--   0        0        0      927 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/utils/math.py
+-rw-r--r--   0        0        0     2089 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/utils/model.py
+-rw-r--r--   0        0        0      863 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/utils/nonce.py
+-rw-r--r--   0        0        0      503 2023-06-20 02:41:13.744585 vertex_protocol-1.1.3/vertex_protocol/utils/subaccount.py
+-rw-r--r--   0        0        0     4119 1970-01-01 00:00:00.000000 vertex_protocol-1.1.3/PKG-INFO
```

### Comparing `vertex_protocol-1.1.2/README.md` & `vertex_protocol-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/pyproject.toml` & `vertex_protocol-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vertex-protocol"
-version = "1.1.2"
+version = "1.1.3"
 description = "Vertex Protocol SDK"
 authors = ["Jeury Mejia <jeury@vertexprotocol.com>"]
 homepage = "https://vertexprotocol.com/"
 maintainers = [
   "Frank Jia <frank@vertexprotocol.com>",
   "Clark Oh-Willeke <clark@vertexprotocol.com>"
 ]
```

### Comparing `vertex_protocol-1.1.2/vertex_protocol/client/__init__.py` & `vertex_protocol-1.1.3/vertex_protocol/client/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/client/apis/__init__.py` & `vertex_protocol-1.1.3/vertex_protocol/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/client/apis/base.py` & `vertex_protocol-1.1.3/vertex_protocol/client/apis/base.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/client/apis/market/__init__.py` & `vertex_protocol-1.1.3/vertex_protocol/client/apis/market/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/client/apis/market/execute.py` & `vertex_protocol-1.1.3/vertex_protocol/client/apis/market/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/client/apis/market/query.py` & `vertex_protocol-1.1.3/vertex_protocol/client/apis/market/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/client/apis/perp/__init__.py` & `vertex_protocol-1.1.3/vertex_protocol/client/apis/perp/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/client/apis/perp/query.py` & `vertex_protocol-1.1.3/vertex_protocol/client/apis/perp/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/client/apis/spot/__init__.py` & `vertex_protocol-1.1.3/vertex_protocol/client/apis/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/client/apis/spot/base.py` & `vertex_protocol-1.1.3/vertex_protocol/client/apis/spot/base.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/client/apis/spot/execute.py` & `vertex_protocol-1.1.3/vertex_protocol/client/apis/spot/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/client/apis/spot/query.py` & `vertex_protocol-1.1.3/vertex_protocol/client/apis/spot/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/client/apis/subaccount/__init__.py` & `vertex_protocol-1.1.3/vertex_protocol/client/apis/subaccount/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/client/apis/subaccount/execute.py` & `vertex_protocol-1.1.3/vertex_protocol/client/apis/subaccount/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/client/apis/subaccount/query.py` & `vertex_protocol-1.1.3/vertex_protocol/client/apis/subaccount/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/client/context.py` & `vertex_protocol-1.1.3/vertex_protocol/client/context.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/contracts/__init__.py` & `vertex_protocol-1.1.3/vertex_protocol/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/contracts/abis/Endpoint.json` & `vertex_protocol-1.1.3/vertex_protocol/contracts/abis/Endpoint.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/contracts/abis/FQuerier.json` & `vertex_protocol-1.1.3/vertex_protocol/contracts/abis/FQuerier.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/contracts/abis/IClearinghouse.json` & `vertex_protocol-1.1.3/vertex_protocol/contracts/abis/IClearinghouse.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/contracts/abis/IERC20.json` & `vertex_protocol-1.1.3/vertex_protocol/contracts/abis/IERC20.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/contracts/abis/IEndpoint.json` & `vertex_protocol-1.1.3/vertex_protocol/contracts/abis/IEndpoint.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/contracts/abis/IOffchainBook.json` & `vertex_protocol-1.1.3/vertex_protocol/contracts/abis/IOffchainBook.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/contracts/abis/IPerpEngine.json` & `vertex_protocol-1.1.3/vertex_protocol/contracts/abis/IPerpEngine.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/contracts/abis/IProductEngine.json` & `vertex_protocol-1.1.3/vertex_protocol/contracts/abis/IProductEngine.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/contracts/abis/ISpotEngine.json` & `vertex_protocol-1.1.3/vertex_protocol/contracts/abis/ISpotEngine.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/contracts/abis/MockERC20.json` & `vertex_protocol-1.1.3/vertex_protocol/contracts/abis/MockERC20.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json` & `vertex_protocol-1.1.3/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json` & `vertex_protocol-1.1.3/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/contracts/deployments/deployment.test.json` & `vertex_protocol-1.1.3/vertex_protocol/contracts/deployments/deployment.test.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/contracts/eip712/domain.py` & `vertex_protocol-1.1.3/vertex_protocol/contracts/eip712/domain.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/contracts/eip712/sign.py` & `vertex_protocol-1.1.3/vertex_protocol/contracts/eip712/sign.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/contracts/eip712/types.py` & `vertex_protocol-1.1.3/vertex_protocol/contracts/eip712/types.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/contracts/loader.py` & `vertex_protocol-1.1.3/vertex_protocol/contracts/loader.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/contracts/types.py` & `vertex_protocol-1.1.3/vertex_protocol/contracts/types.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/engine_client/__init__.py` & `vertex_protocol-1.1.3/vertex_protocol/engine_client/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/engine_client/execute.py` & `vertex_protocol-1.1.3/vertex_protocol/engine_client/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/engine_client/query.py` & `vertex_protocol-1.1.3/vertex_protocol/engine_client/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/engine_client/types/__init__.py` & `vertex_protocol-1.1.3/vertex_protocol/engine_client/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/engine_client/types/execute.py` & `vertex_protocol-1.1.3/vertex_protocol/engine_client/types/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/engine_client/types/models.py` & `vertex_protocol-1.1.3/vertex_protocol/engine_client/types/models.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/engine_client/types/query.py` & `vertex_protocol-1.1.3/vertex_protocol/engine_client/types/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/indexer_client/__init__.py` & `vertex_protocol-1.1.3/vertex_protocol/indexer_client/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/indexer_client/query.py` & `vertex_protocol-1.1.3/vertex_protocol/indexer_client/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/indexer_client/types/__init__.py` & `vertex_protocol-1.1.3/vertex_protocol/indexer_client/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/indexer_client/types/models.py` & `vertex_protocol-1.1.3/vertex_protocol/indexer_client/types/models.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/indexer_client/types/query.py` & `vertex_protocol-1.1.3/vertex_protocol/indexer_client/types/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/utils/__init__.py` & `vertex_protocol-1.1.3/vertex_protocol/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/utils/bytes32.py` & `vertex_protocol-1.1.3/vertex_protocol/utils/bytes32.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/utils/exceptions.py` & `vertex_protocol-1.1.3/vertex_protocol/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/utils/expiration.py` & `vertex_protocol-1.1.3/vertex_protocol/utils/expiration.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/utils/math.py` & `vertex_protocol-1.1.3/vertex_protocol/utils/math.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/utils/model.py` & `vertex_protocol-1.1.3/vertex_protocol/utils/model.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.2/vertex_protocol/utils/nonce.py` & `vertex_protocol-1.1.3/vertex_protocol/utils/nonce.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional
-import time
+from datetime import timezone, datetime, timedelta
 import random
 
 
 def gen_order_nonce(
     recv_time_ms: Optional[int] = None, random_int: Optional[int] = None
 ) -> int:
     """
@@ -14,12 +14,14 @@
 
         random_int (int, optional): An integer for the nonce. Defaults to a random integer between 0 and 999.
 
     Returns:
         int: The generated order nonce.
     """
     if recv_time_ms is None:
-        recv_time_ms = (int(time.time()) + 90) * 1000
+        recv_time_ms = int(
+            (datetime.now(tz=timezone.utc) + timedelta(seconds=90)).timestamp() * 1000
+        )
     if random_int is None:
         random_int = random.randint(0, 999)
 
     return (recv_time_ms << 20) + random_int
```

### Comparing `vertex_protocol-1.1.2/PKG-INFO` & `vertex_protocol-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertex-protocol
-Version: 1.1.2
+Version: 1.1.3
 Summary: Vertex Protocol SDK
 Home-page: https://vertexprotocol.com/
 Keywords: vertex protocol,vertex sdk,vertex protocol api
 Author: Jeury Mejia
 Author-email: jeury@vertexprotocol.com
 Maintainer: Frank Jia
 Maintainer-email: frank@vertexprotocol.com
```

