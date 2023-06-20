# Comparing `tmp/firefly_exchange_client-0.3.2.tar.gz` & `tmp/firefly_exchange_client-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firefly_exchange_client-0.3.2.tar", last modified: Fri Jun 16 22:30:55 2023, max compression
+gzip compressed data, was "firefly_exchange_client-0.4.0.tar", last modified: Tue Jun 20 13:22:18 2023, max compression
```

## Comparing `firefly_exchange_client-0.3.2.tar` & `firefly_exchange_client-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:30:55.903680 firefly_exchange_client-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-16 22:30:55.903680 firefly_exchange_client-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 22:30:55.903680 firefly_exchange_client-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:30:55.899680 firefly_exchange_client-0.3.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:30:55.899680 firefly_exchange_client-0.3.2/src/firefly_exchange_client/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/api_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    36559 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    83581 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/contract_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/enumerations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/onboarding_signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/order_signer.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/signer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/socket_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/sockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-06-16 22:30:46.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 22:30:55.903680 firefly_exchange_client-0.3.2/src/firefly_exchange_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-16 22:30:55.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-16 22:30:55.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 22:30:55.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 22:30:55.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-16 22:30:55.000000 firefly_exchange_client-0.3.2/src/firefly_exchange_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:22:18.182067 firefly_exchange_client-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-06-20 13:22:18.182067 firefly_exchange_client-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 13:22:18.182067 firefly_exchange_client-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:22:18.178067 firefly_exchange_client-0.4.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:22:18.182067 firefly_exchange_client-0.4.0/src/firefly_exchange_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/api_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37256 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83581 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/contract_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/enumerations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/onboarding_signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/order_signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/signer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/socket_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/sockets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-06-20 13:22:08.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:22:18.182067 firefly_exchange_client-0.4.0/src/firefly_exchange_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-06-20 13:22:18.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-20 13:22:18.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:22:18.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-20 13:22:18.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 13:22:18.000000 firefly_exchange_client-0.4.0/src/firefly_exchange_client.egg-info/top_level.txt
```

### Comparing `firefly_exchange_client-0.3.2/LICENSE` & `firefly_exchange_client-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.2/PKG-INFO` & `firefly_exchange_client-0.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: firefly_exchange_client
-Version: 0.3.2
-Summary: Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts
-Project-URL: Homepage, https://github.com/fireflyprotocol/firefly_exchange_client
-Project-URL: Bug Reports, https://github.com/fireflyprotocol/firefly_exchange_client/issues
-Project-URL: Source, https://github.com/fireflyprotocol/firefly_exchange_client/
-Keywords: firefly,exchange,decentralized,perpetuals,blockchain
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Firefly Client Library
 
 [<img alt="Firefly logo" src="https://raw.githubusercontent.com/fireflyprotocol/firefly_exchange_client/main/res/banner.png" />](#)
 
 <div align="center">
 
 ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/fireflyprotocol/firefly_exchange_client/publish_to_pypi.yml)
@@ -96,15 +84,45 @@
 
 if __name__ == "__main__":
   loop = asyncio.new_event_loop()
   loop.run_until_complete(main())
   loop.close()
 ```
 
-​
+**Read-only Initialization:**
+Firefly-client can also be initialized in `read-only` mode, below is the example:
+```python
+from config import TEST_ACCT_KEY, TEST_NETWORK
+from firefly_exchange_client import FireflyClient, Networks
+from pprint import pprint
+import asyncio
+
+async def main():
+  # initialize client without providing private_key
+  client = FireflyClient(
+      True, # agree to terms and conditions
+      Networks[TEST_NETWORK], # network to connect with
+      )
+
+  # Initializing client for the private key provided. The second argument api_token is optional
+  await client.init(True,"54b0bfafc9a48728f76e52848a716e96d490263392e3959c2d44f05dea960761") 
+
+  # close aio http connection
+  await client.apis.close_session()
+  await client.dmsApi.close_session()
+
+  pprint(data)
+
+if __name__ == "__main__":
+  loop = asyncio.new_event_loop()
+  loop.run_until_complete(main())
+  loop.close()
+```
+​Here is the [list](https://docs.bluefin.io/8/2.readonly-access-data) of APIs that can be accessed in `read-only` mode.
+
 **Placing Orders:**
 
 ```python
 from config import TEST_ACCT_KEY, TEST_NETWORK
 from firefly_exchange_client import FireflyClient, Networks, MARKET_SYMBOLS, ORDER_SIDE, ORDER_TYPE, OrderSignatureRequest
 import asyncio
```

### Comparing `firefly_exchange_client-0.3.2/README.md` & `firefly_exchange_client-0.4.0/src/firefly_exchange_client.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: firefly-exchange-client
+Version: 0.4.0
+Summary: Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts
+Project-URL: Homepage, https://github.com/fireflyprotocol/firefly_exchange_client
+Project-URL: Bug Reports, https://github.com/fireflyprotocol/firefly_exchange_client/issues
+Project-URL: Source, https://github.com/fireflyprotocol/firefly_exchange_client/
+Keywords: firefly,exchange,decentralized,perpetuals,blockchain
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Firefly Client Library
 
 [<img alt="Firefly logo" src="https://raw.githubusercontent.com/fireflyprotocol/firefly_exchange_client/main/res/banner.png" />](#)
 
 <div align="center">
 
 ![GitHub Workflow Status (with branch)](https://img.shields.io/github/actions/workflow/status/fireflyprotocol/firefly_exchange_client/publish_to_pypi.yml)
@@ -84,15 +96,45 @@
 
 if __name__ == "__main__":
   loop = asyncio.new_event_loop()
   loop.run_until_complete(main())
   loop.close()
 ```
 
-​
+**Read-only Initialization:**
+Firefly-client can also be initialized in `read-only` mode, below is the example:
+```python
+from config import TEST_ACCT_KEY, TEST_NETWORK
+from firefly_exchange_client import FireflyClient, Networks
+from pprint import pprint
+import asyncio
+
+async def main():
+  # initialize client without providing private_key
+  client = FireflyClient(
+      True, # agree to terms and conditions
+      Networks[TEST_NETWORK], # network to connect with
+      )
+
+  # Initializing client for the private key provided. The second argument api_token is optional
+  await client.init(True,"54b0bfafc9a48728f76e52848a716e96d490263392e3959c2d44f05dea960761") 
+
+  # close aio http connection
+  await client.apis.close_session()
+  await client.dmsApi.close_session()
+
+  pprint(data)
+
+if __name__ == "__main__":
+  loop = asyncio.new_event_loop()
+  loop.run_until_complete(main())
+  loop.close()
+```
+​Here is the [list](https://docs.bluefin.io/8/2.readonly-access-data) of APIs that can be accessed in `read-only` mode.
+
 **Placing Orders:**
 
 ```python
 from config import TEST_ACCT_KEY, TEST_NETWORK
 from firefly_exchange_client import FireflyClient, Networks, MARKET_SYMBOLS, ORDER_SIDE, ORDER_TYPE, OrderSignatureRequest
 import asyncio
```

### Comparing `firefly_exchange_client-0.3.2/pyproject.toml` & `firefly_exchange_client-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "firefly_exchange_client"
-version = "0.3.2"
+version = "0.4.0"
 description = "Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["firefly", "exchange", "decentralized", "perpetuals", "blockchain"]
 dependencies = [
   'web3 ~= 5.31.3',
   'requests ~= 2.28.1',
```

### Comparing `firefly_exchange_client-0.3.2/src/firefly_exchange_client/api_service.py` & `firefly_exchange_client-0.4.0/src/firefly_exchange_client/api_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .interfaces import *
 
 
 class APIService():
     def __init__(self, url):
         self.server_url = url
         self.auth_token = None
+        self.api_token = None
         self.client = aiohttp.ClientSession()
 
     async def close_session(self):
         if self.client is not None:
             return await self.client.close()
 
     async def get(self, service_url, query={}, auth_required=False):
@@ -24,15 +25,19 @@
         url = self._create_url(service_url)
 
         response = None
         if auth_required:
             response = await self.client.get(
                 url,
                 params=query,
-                headers={'Authorization': 'Bearer {}'.format(self.auth_token)})
+                headers={
+                    'Authorization': 'Bearer {}'.format(self.auth_token) if self.auth_token else '',
+                    'x-api-token': self.api_token or ''
+                }
+            )
         else:
             response = await self.client.get(url, params=query)
 
         try:
             if response.status != 503:  # checking for service unavailitbility
                 return await response.json()
             else:
```

### Comparing `firefly_exchange_client-0.3.2/src/firefly_exchange_client/client.py` & `firefly_exchange_client-0.4.0/src/firefly_exchange_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,33 +10,35 @@
 from .enumerations import *
 from .websocket_client import WebsocketClient
 
 from eth_account import Account
 from eth_utils import to_wei, from_wei
 
 class FireflyClient:
-    def __init__(self, are_terms_accepted, network, private_key):
+    def __init__(self, are_terms_accepted, network, private_key=""):
         self.are_terms_accepted = are_terms_accepted
         self.network = network
         self.w3 = self._connect_w3(self.network["url"])
-        self.account = Account.from_key(private_key)
+        if private_key != "":
+            self.account = Account.from_key(private_key)
         self.apis = APIService(self.network["apiGateway"])
         self.dmsApi = APIService(self.network["dmsURL"])
         self.socket = Sockets(self.network["socketURL"])
         self.webSocketClient = WebsocketClient(self.network["webSocketURL"])
         self.contracts = Contracts()
         self.order_signers = {}
         self.onboarding_signer = OnboardingSigner()
         
             
-    async def init(self, user_onboarding=True):
+    async def init(self, user_onboarding=True, api_token=""):
         """
             Initialize the client.
             Inputs:
                 user_onboarding (bool, optional): If set to true onboards the user address to exchange and gets authToken. Defaults to True.
+                api_token(string, optional): API token to initialize client in read-only mode 
         """
         self.contracts.contract_addresses = await self.get_contract_addresses()
 
         if "error" in self.contracts.contract_addresses:
             raise Exception("Error initializing client: {}".format(self.contracts.contract_addresses["error"]))
 
         # adding auxiliaryContracts to contracts class
@@ -44,15 +46,21 @@
             self.add_contract(name=i,address=j)
         
         # contracts pertaining to markets
         for k, v in self.contracts.contract_addresses.items():
             if 'PERP' in k:
                 self.add_contract(name="Perpetual",address=v["Perpetual"], market=k)
 
-        if user_onboarding:
+        if api_token:
+            self.apis.api_token = api_token
+            # for socket
+            self.socket.set_api_token(api_token)
+            self.webSocketClient.set_api_token(api_token)
+        # In case of api_token received, user onboarding is not done
+        elif user_onboarding:
             self.apis.auth_token = await self.onboard_user()
             self.dmsApi.auth_token = self.apis.auth_token
             self.socket.set_token(self.apis.auth_token)
             self.webSocketClient.set_token(self.apis.auth_token)
 
 
     async def onboard_user(self, token:str=None):
@@ -750,14 +758,23 @@
 
     def get_public_address(self):
         """
             Returns the user account public address
         """
         return self.account.address
 
+    async def generate_readonly_token(self):
+        """
+            Returns a read-only token generated for authenticated user.
+        """
+        return await self.apis.post(
+            SERVICE_URLS["USER"]["GENERATE_READONLY_TOKEN"],
+            {},
+            True
+        )
     async def get_orders(self,params:GetOrderRequest):
         """
             Returns a list of orders.
             Inputs:
                 params(GetOrderRequest): params required to query orders (e.g. symbol,statuses) 
             Returns:
                 list: a list of orders
```

### Comparing `firefly_exchange_client-0.3.2/src/firefly_exchange_client/constants.py` & `firefly_exchange_client-0.4.0/src/firefly_exchange_client/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
     "MASTER_INFO": "/masterInfo",
     "FUNDING_RATE":"/fundingRate"
   },
   "USER": {
     "USER_POSITIONS": "/userPosition",
     "USER_TRADES": "/userTrades",
     "ORDERS": "/orders",
+    "GENERATE_READONLY_TOKEN": "/generateReadOnlyToken",
     "ACCOUNT": "/account",
     "USER_TRANSACTION_HISTORY": "/userTransactionHistory",
     "AUTHORIZE": "/authorize",
     "ADJUST_LEVERAGE": "/account/adjustLeverage",
     "FUND_GAS": "/account/fundGas",
     "TRANSFER_HISTORY": "/userTransferHistory",
     "FUNDING_HISTORY": "/userFundingHistory",
```

### Comparing `firefly_exchange_client-0.3.2/src/firefly_exchange_client/contract_abis.py` & `firefly_exchange_client-0.4.0/src/firefly_exchange_client/contract_abis.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.2/src/firefly_exchange_client/contracts.py` & `firefly_exchange_client-0.4.0/src/firefly_exchange_client/contracts.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.2/src/firefly_exchange_client/enumerations.py` & `firefly_exchange_client-0.4.0/src/firefly_exchange_client/enumerations.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,14 +77,16 @@
     MARKET_DATA_UPDATE = "MarketDataUpdate"
     RECENT_TRADES = "RecentTrades"
     ORDERBOOK_UPDATE = "OrderbookUpdate"
     ADJUST_MARGIN = "AdjustMargin"
     MARKET_HEALTH = "MarketHealth"
     EXCHANGE_HEALTH = "ExchangeHealth"
     ORDER_UPDATE = "OrderUpdate"
+    ORDER_SENT_FOR_SETTLEMENT = "OrderSettlementUpdate"
+    ORDER_REQUEUE_UPDATE = "OrderRequeueUpdate"
     ORDER_CANCELLATION = "OrderCancelled"
     POSITION_UPDATE = "PositionUpdate"
     USER_TRADE = "UserTrade"
     USER_TRANSACTION = "UserTransaction"
     ACCOUNT_DATA = "AccountDataUpdate"
```

### Comparing `firefly_exchange_client-0.3.2/src/firefly_exchange_client/interfaces.py` & `firefly_exchange_client-0.4.0/src/firefly_exchange_client/interfaces.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.2/src/firefly_exchange_client/onboarding_signer.py` & `firefly_exchange_client-0.4.0/src/firefly_exchange_client/onboarding_signer.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.2/src/firefly_exchange_client/order_signer.py` & `firefly_exchange_client-0.4.0/src/firefly_exchange_client/order_signer.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.2/src/firefly_exchange_client/signer.py` & `firefly_exchange_client-0.4.0/src/firefly_exchange_client/signer.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.2/src/firefly_exchange_client/socket_manager.py` & `firefly_exchange_client-0.4.0/src/firefly_exchange_client/socket_manager.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.2/src/firefly_exchange_client/sockets.py` & `firefly_exchange_client-0.4.0/src/firefly_exchange_client/sockets.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,164 +1,175 @@
 import socketio
 from .enumerations import MARKET_SYMBOLS, SOCKET_EVENTS
 
 sio = socketio.Client()
-      
+
+
 class Sockets:
-    callbacks={}
+    callbacks = {}
+
     def __init__(self, url, timeout=10, token=None) -> None:
-        self.url = url  
+        self.url = url
         self.timeout = timeout
         self.token = token
-        return 
+        self.api_token = ""
+        return
 
     def _establish_connection(self):
         """
             Connects to the desired url
         """
         try:
-            sio.connect(self.url,wait_timeout=self.timeout,transports=["websocket"])
+            sio.connect(self.url, wait_timeout=self.timeout,
+                        transports=["websocket"])
             return True
         except:
             return False
 
     def set_token(self, token):
         """
             Sets default user token
             Inputs:
                 - token (user auth token): firefly onboarding token.
         """
         self.token = token
 
+    def set_api_token(self, token):
+        """
+            Sets default user token
+            Inputs:
+                - token (user auth token): firefly onboarding token.
+        """
+        self.api_token = token
+
     async def open(self):
         """
             opens socket instance connection
         """
         self.connection_established = self._establish_connection()
         if not self.connection_established:
             await self.close()
-            raise(Exception("Failed to connect to Host: {}".format(self.url)))
+            raise (Exception("Failed to connect to Host: {}".format(self.url)))
         return
-        
 
     async def close(self):
         """
             closes the socket instance connection
         """
         sio.disconnect()
-        return 
+        return
 
     @sio.on("*")
-    def listener(event,data):
+    def listener(event, data):
         """
             Listens to all events emitted by the server
         """
         try:
             if event in Sockets.callbacks.keys():
                 Sockets.callbacks[event](data)
             elif "default" in Sockets.callbacks.keys():
-                Sockets.callbacks["default"]({"event":event,"data":data})
+                Sockets.callbacks["default"]({"event": event, "data": data})
             else:
                 pass
         except:
             pass
-        return 
+        return
 
-    async def listen(self,event,callback):
+    async def listen(self, event, callback):
         """
             Assigns callbacks to desired events
         """
         Sockets.callbacks[event] = callback
-        return 
+        return
 
-    async def subscribe_global_updates_by_symbol(self,symbol: MARKET_SYMBOLS):
+    async def subscribe_global_updates_by_symbol(self, symbol: MARKET_SYMBOLS):
         """
             Allows user to subscribe to global updates for the desired symbol.
             Inputs:
                 - symbol: market symbol of market user wants global updates for. (e.g. DOT-PERP)
         """
         try:
             if not self.connection_established:
-                raise Exception("Socket connection is established, invoke socket.open()")
+                raise Exception(
+                    "Socket connection is established, invoke socket.open()")
 
-            resp = sio.call('SUBSCRIBE',[
-            {
-                "e": SOCKET_EVENTS.GLOBAL_UPDATES_ROOM.value,
-                "p": symbol.value,
-            },
+            resp = sio.call('SUBSCRIBE', [
+                {
+                    "e": SOCKET_EVENTS.GLOBAL_UPDATES_ROOM.value,
+                    "p": symbol.value,
+                },
             ])
             return resp["success"]
         except Exception as e:
             print("Error: ", e)
             return False
 
-    async def unsubscribe_global_updates_by_symbol(self,symbol: MARKET_SYMBOLS):
+    async def unsubscribe_global_updates_by_symbol(self, symbol: MARKET_SYMBOLS):
         """
             Allows user to unsubscribe to global updates for the desired symbol.
                 Inputs:
                     - symbol: market symbol of market user wants to remove global updates for. (e.g. DOT-PERP)
         """
         try:
             if not self.connection_established:
-                return False 
-            
+                return False
+
             resp = sio.call('UNSUBSCRIBE', [
-            {
-                "e": SOCKET_EVENTS.GLOBAL_UPDATES_ROOM.value,
-                "p": symbol.value,
-            },
+                {
+                    "e": SOCKET_EVENTS.GLOBAL_UPDATES_ROOM.value,
+                    "p": symbol.value,
+                },
             ])
 
             return resp["success"]
         except Exception as e:
-            print(e) 
+            print(e)
             return False
 
-    async def subscribe_user_update_by_token(self, parent_account: str=None, user_token: str=None) -> bool:
+    async def subscribe_user_update_by_token(self, parent_account: str = None, user_token: str = None) -> bool:
         """
             Allows user to subscribe to their account updates.
             Inputs:
                 - parent_account(str): address of parent account. Only whitelisted 
                   sub-account can listen to its parent account position updates
                 - token(str): auth token generated when onboarding on firefly
         """
         try:
             if not self.connection_established:
                 return False
-              
+
             resp = sio.call("SUBSCRIBE", [
-            {
-                "e": SOCKET_EVENTS.USER_UPDATES_ROOM.value,
-                'pa': parent_account,
-                "t": self.token if user_token == None else user_token,
-            },
+                {
+                    "e": SOCKET_EVENTS.USER_UPDATES_ROOM.value,
+                    'pa': parent_account,
+                    "t": self.token if user_token == None else user_token,
+                    "rt": self.api_token
+                },
             ])
 
             return resp["success"]
         except Exception as e:
-            print(e) 
+            print(e)
             return False
 
-    async def unsubscribe_user_update_by_token(self, parent_account: str=None, user_token:str=None): 
+    async def unsubscribe_user_update_by_token(self, parent_account: str = None, user_token: str = None):
         """
             Allows user to unsubscribe to their account updates.
             Inputs:
                 - parent_account(str): address of parent account. Only for sub-accounts
                 - token: auth token generated when onboarding on firefly
         """
         try:
             if not self.connection_established:
                 return False
-              
+
             resp = sio.call("UNSUBSCRIBE", [
-            {
-                "e": SOCKET_EVENTS.USER_UPDATES_ROOM.value,
-                'pa': parent_account,
-                "t": self.token if user_token == None else user_token,
-            },
+                {
+                    "e": SOCKET_EVENTS.USER_UPDATES_ROOM.value,
+                    'pa': parent_account,
+                    "t": self.token if user_token == None else user_token,
+                    "rt": self.api_token
+                },
             ])
             return resp["success"]
         except:
             return False
-
-    
-
```

### Comparing `firefly_exchange_client-0.3.2/src/firefly_exchange_client/utilities.py` & `firefly_exchange_client-0.4.0/src/firefly_exchange_client/utilities.py`

 * *Files identical despite different names*

### Comparing `firefly_exchange_client-0.3.2/src/firefly_exchange_client/websocket_client.py` & `firefly_exchange_client-0.4.0/src/firefly_exchange_client/websocket_client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 import json
 import logging
 from .socket_manager import SocketManager
 from .enumerations import MARKET_SYMBOLS, SOCKET_EVENTS
 
+
 class WebsocketClient:
     def __init__(
         self,
         stream_url,
         token=None,
+        api_token=None,
         logger=None,
     ):
         if not logger:
             logger = logging.getLogger(__name__)
         self.logger = logger
         self.token = token
+        self.api_token = api_token
         self.stream_url = stream_url
-        self.callbacks={}
+        self.callbacks = {}
 
     def initialize_socket(
         self,
         on_open,
         on_close=None,
         on_error=None,
         on_ping=None,
         on_pong=None,
         logger=None,
     ):
-        self.socket_manager =  SocketManager(
+        self.socket_manager = SocketManager(
             self.stream_url,
             on_message=self.listener,
             on_open=on_open,
             on_close=on_close,
             on_error=on_error,
             on_ping=on_ping,
             on_pong=on_pong,
@@ -38,131 +41,142 @@
         )
 
         # start the thread
         self.socket_manager.create_ws_connection()
         self.logger.debug("WebSocket Client started.")
         self.socket_manager.start()
 
-
     def set_token(self, token):
         """
             Sets default user token
             Inputs:
                 - token (user auth token): firefly onboarding token.
         """
         self.token = token
-    
-    def listen(self,event,callback):
+
+    def set_api_token(self, token):
+        """
+            Sets default user token
+            Inputs:
+                - token (user auth token): firefly onboarding token.
+        """
+        self.api_token = token
+
+    def listen(self, event, callback):
         """
             Assigns callbacks to desired events
         """
         self.callbacks[event] = callback
-        return 
+        return
 
     def send(self, message: dict):
         self.socket_manager.send_message(json.dumps(message))
 
-    def subscribe_global_updates_by_symbol(self,symbol: MARKET_SYMBOLS):
+    def subscribe_global_updates_by_symbol(self, symbol: MARKET_SYMBOLS):
         """
             Allows user to subscribe to global updates for the desired symbol.
             Inputs:
                 - symbol: market symbol of market user wants global updates for. (e.g. DOT-PERP)
         """
         try:
             if not self.socket_manager.ws.connected:
-                raise Exception("Socket connection is established, invoke socket.open()")
+                raise Exception(
+                    "Socket connection is established, invoke socket.open()")
 
-            self.socket_manager.send_message(json.dumps(['SUBSCRIBE',[
+            self.socket_manager.send_message(json.dumps(['SUBSCRIBE', [
                 {
                     "e": SOCKET_EVENTS.GLOBAL_UPDATES_ROOM.value,
                     "p": symbol.value,
                 },
-                ]]))
+            ]]))
             return True
         except Exception:
             return False
 
-    def unsubscribe_global_updates_by_symbol(self,symbol: MARKET_SYMBOLS):
+    def unsubscribe_global_updates_by_symbol(self, symbol: MARKET_SYMBOLS):
         """
             Allows user to unsubscribe to global updates for the desired symbol.
                 Inputs:
                     - symbol: market symbol of market user wants to remove global updates for. (e.g. DOT-PERP)
         """
         try:
             if not self.socket_manager.ws.connected:
-                return False 
-            
+                return False
+
             self.socket_manager.send_message(json.dumps((['UNSUBSCRIBE', [
-            {
-                "e": SOCKET_EVENTS.GLOBAL_UPDATES_ROOM.value,
-                "p": symbol.value,
-            },
+                {
+                    "e": SOCKET_EVENTS.GLOBAL_UPDATES_ROOM.value,
+                    "p": symbol.value,
+                },
             ]])))
             return True
         except:
             return False
 
-    def subscribe_user_update_by_token(self, user_token: str=None):
+    def subscribe_user_update_by_token(self, user_token: str = None):
         """
             Allows user to subscribe to their account updates.
             Inputs:
                 - token(str): auth token generated when onboarding on firefly
         """
         try:
             if not self.socket_manager.ws.connected:
                 return False
-              
+
             self.socket_manager.send_message(json.dumps((["SUBSCRIBE", [
-            {
-                "e": SOCKET_EVENTS.USER_UPDATES_ROOM.value,
-                "t": self.token if user_token == None else user_token,
-            },
+                {
+                    "e": SOCKET_EVENTS.USER_UPDATES_ROOM.value,
+                    "t": self.token if user_token == None else user_token,
+                    "rt": self.api_token
+                },
             ]])))
             return True
         except:
             return False
 
-    def unsubscribe_user_update_by_token(self, user_token:str=None): 
+    def unsubscribe_user_update_by_token(self, user_token: str = None):
         """
             Allows user to unsubscribe to their account updates.
             Inputs:
                 - token: auth token generated when onboarding on firefly
         """
         try:
             if not self.socket_manager.ws.connected:
                 return False
-              
+
             self.socket_manager.send_message(json.dumps((["UNSUBSCRIBE", [
-            {
-                "e": SOCKET_EVENTS.USER_UPDATES_ROOM.value,
-                "t": self.token if user_token == None else user_token,
-            },
+                {
+                    "e": SOCKET_EVENTS.USER_UPDATES_ROOM.value,
+                    "t": self.token if user_token == None else user_token,
+                    "rt": self.api_token
+                },
             ]])))
             return True
         except:
             return False
 
     def ping(self):
         self.logger.debug("Sending ping to WebSocket Server")
         self.socket_manager.ping()
 
     def stop(self, id=None):
         self.socket_manager.close()
         # self.socket_manager.join()
 
-    def listener(self,_, message):
+    def listener(self, _, message):
         """
             Listens to all events emitted by the server
         """
         data = json.loads(message)
         event_name = data["eventName"]
         try:
             if event_name in self.callbacks:
                 callback = self.callbacks[event_name]
                 callback(data["data"])
             elif "default" in self.callbacks.keys():
-                self.callbacks["default"]({"event":event_name,"data":data["data"]})
+                self.callbacks["default"](
+                    {"event": event_name, "data": data["data"]})
             else:
                 pass
         except:
             pass
-        return 
+        return
```

### Comparing `firefly_exchange_client-0.3.2/src/firefly_exchange_client.egg-info/PKG-INFO` & `firefly_exchange_client-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: firefly-exchange-client
-Version: 0.3.2
+Name: firefly_exchange_client
+Version: 0.4.0
 Summary: Library to interact with firefly exchange protocol including its off-chain api-gateway and on-chain contracts
 Project-URL: Homepage, https://github.com/fireflyprotocol/firefly_exchange_client
 Project-URL: Bug Reports, https://github.com/fireflyprotocol/firefly_exchange_client/issues
 Project-URL: Source, https://github.com/fireflyprotocol/firefly_exchange_client/
 Keywords: firefly,exchange,decentralized,perpetuals,blockchain
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -96,15 +96,45 @@
 
 if __name__ == "__main__":
   loop = asyncio.new_event_loop()
   loop.run_until_complete(main())
   loop.close()
 ```
 
-​
+**Read-only Initialization:**
+Firefly-client can also be initialized in `read-only` mode, below is the example:
+```python
+from config import TEST_ACCT_KEY, TEST_NETWORK
+from firefly_exchange_client import FireflyClient, Networks
+from pprint import pprint
+import asyncio
+
+async def main():
+  # initialize client without providing private_key
+  client = FireflyClient(
+      True, # agree to terms and conditions
+      Networks[TEST_NETWORK], # network to connect with
+      )
+
+  # Initializing client for the private key provided. The second argument api_token is optional
+  await client.init(True,"54b0bfafc9a48728f76e52848a716e96d490263392e3959c2d44f05dea960761") 
+
+  # close aio http connection
+  await client.apis.close_session()
+  await client.dmsApi.close_session()
+
+  pprint(data)
+
+if __name__ == "__main__":
+  loop = asyncio.new_event_loop()
+  loop.run_until_complete(main())
+  loop.close()
+```
+​Here is the [list](https://docs.bluefin.io/8/2.readonly-access-data) of APIs that can be accessed in `read-only` mode.
+
 **Placing Orders:**
 
 ```python
 from config import TEST_ACCT_KEY, TEST_NETWORK
 from firefly_exchange_client import FireflyClient, Networks, MARKET_SYMBOLS, ORDER_SIDE, ORDER_TYPE, OrderSignatureRequest
 import asyncio
```

### Comparing `firefly_exchange_client-0.3.2/src/firefly_exchange_client.egg-info/SOURCES.txt` & `firefly_exchange_client-0.4.0/src/firefly_exchange_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

