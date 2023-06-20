# Comparing `tmp/proton-api-client-0.0.3.tar.gz` & `tmp/proton-api-client-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proton-api-client-0.0.3.tar", last modified: Mon Jun 19 18:31:40 2023, max compression
+gzip compressed data, was "proton-api-client-0.0.4.tar", last modified: Tue Jun 20 20:28:57 2023, max compression
```

## Comparing `proton-api-client-0.0.3.tar` & `proton-api-client-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-19 18:31:40.758439 proton-api-client-0.0.3/
--rw-r--r--   0 x         (1000) x         (1000)    35149 2023-06-19 17:50:26.000000 proton-api-client-0.0.3/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)     1135 2023-06-19 18:31:40.758439 proton-api-client-0.0.3/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      747 2023-06-19 18:31:17.000000 proton-api-client-0.0.3/README.md
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-19 18:31:40.758439 proton-api-client-0.0.3/proton/
--rw-r--r--   0 x         (1000) x         (1000)      156 2023-06-19 17:57:18.000000 proton-api-client-0.0.3/proton/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)     9059 2023-06-19 18:23:32.000000 proton-api-client-0.0.3/proton/_ctsrp.py
--rw-r--r--   0 x         (1000) x         (1000)     4077 2023-06-19 18:23:32.000000 proton-api-client-0.0.3/proton/_pysrp.py
--rw-r--r--   0 x         (1000) x         (1000)     4711 2023-06-19 17:57:55.000000 proton-api-client-0.0.3/proton/client.py
--rw-r--r--   0 x         (1000) x         (1000)     2134 2023-06-19 18:15:31.000000 proton-api-client-0.0.3/proton/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     2174 2023-06-19 17:57:18.000000 proton-api-client-0.0.3/proton/helpers.py
--rw-r--r--   0 x         (1000) x         (1000)     1537 2023-06-19 18:15:31.000000 proton-api-client-0.0.3/proton/login.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-19 18:31:40.758439 proton-api-client-0.0.3/proton_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     1135 2023-06-19 18:31:40.000000 proton-api-client-0.0.3/proton_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      354 2023-06-19 18:31:40.000000 proton-api-client-0.0.3/proton_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-19 18:31:40.000000 proton-api-client-0.0.3/proton_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       59 2023-06-19 18:31:40.000000 proton-api-client-0.0.3/proton_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        7 2023-06-19 18:31:40.000000 proton-api-client-0.0.3/proton_api_client.egg-info/top_level.txt
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-19 18:31:40.758439 proton-api-client-0.0.3/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)     1655 2023-06-19 18:31:17.000000 proton-api-client-0.0.3/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-20 20:28:57.305162 proton-api-client-0.0.4/
+-rw-r--r--   0 x         (1000) x         (1000)    35149 2023-06-19 17:50:26.000000 proton-api-client-0.0.4/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)     1173 2023-06-20 20:28:57.305162 proton-api-client-0.0.4/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      784 2023-06-20 20:28:15.000000 proton-api-client-0.0.4/README.md
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-20 20:28:57.305162 proton-api-client-0.0.4/proton/
+-rw-r--r--   0 x         (1000) x         (1000)      156 2023-06-19 17:57:18.000000 proton-api-client-0.0.4/proton/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)     9059 2023-06-19 18:23:32.000000 proton-api-client-0.0.4/proton/_ctsrp.py
+-rw-r--r--   0 x         (1000) x         (1000)     3881 2023-06-20 20:05:33.000000 proton-api-client-0.0.4/proton/_pysrp.py
+-rw-r--r--   0 x         (1000) x         (1000)     4921 2023-06-20 20:28:15.000000 proton-api-client-0.0.4/proton/client.py
+-rw-r--r--   0 x         (1000) x         (1000)     2188 2023-06-20 19:43:36.000000 proton-api-client-0.0.4/proton/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     2017 2023-06-20 20:20:29.000000 proton-api-client-0.0.4/proton/helpers.py
+-rw-r--r--   0 x         (1000) x         (1000)     1537 2023-06-19 18:15:31.000000 proton-api-client-0.0.4/proton/login.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-20 20:28:57.305162 proton-api-client-0.0.4/proton_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)     1173 2023-06-20 20:28:57.000000 proton-api-client-0.0.4/proton_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      354 2023-06-20 20:28:57.000000 proton-api-client-0.0.4/proton_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-20 20:28:57.000000 proton-api-client-0.0.4/proton_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       59 2023-06-20 20:28:57.000000 proton-api-client-0.0.4/proton_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        7 2023-06-20 20:28:57.000000 proton-api-client-0.0.4/proton_api_client.egg-info/top_level.txt
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-20 20:28:57.305162 proton-api-client-0.0.4/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)     1669 2023-06-20 20:28:15.000000 proton-api-client-0.0.4/setup.py
```

### Comparing `proton-api-client-0.0.3/LICENSE` & `proton-api-client-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.3/PKG-INFO` & `proton-api-client-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proton-api-client
-Version: 0.0.3
+Version: 0.0.4
 Summary: Proton Mail API
 Home-page: https://github.com/trevorhobenshield/proton-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: proton api client async search automation bot scrape mail email
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
@@ -22,30 +22,36 @@
 username, password = ..., ...
 proton = ProtonMail(username, password)
 
 passphrase = 'myPass'
 pk = 'privatekey.hotmale@proton.me-6fdhskjgfd7s98gdgre87gregrjdhrgd7897g898.asc'
 proton.gpg_import(pk, passphrase=passphrase)
 
+
+sessions = proton.sessions()
+
 salts = proton.salts()
 
 users = proton.users()
 
 inbox = proton.inbox()
 
-conversation_id = inbox['Conversations'][0]['ID']
-conversation = proton.decrypt_conversation(conversation_id)
+cid = inbox['Conversations'][0]['ID']
+conversation = proton.decrypt_conversation(cid)
 
 decrypted_inbox = proton.inbox_decrypted()
 
 user_settings = proton.user_settings()
 
 mail_settings = proton.mail_settings()
 
 calendar_settings = proton.calendar_settings()
 
 timezones = proton.timezones()
 
 addresses = proton.addresses()
 
 info = proton.info()
+
+proton.revoke_all_sessions()
+
 ```
```

### Comparing `proton-api-client-0.0.3/proton/_ctsrp.py` & `proton-api-client-0.0.4/proton/_ctsrp.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.3/proton/_pysrp.py` & `proton-api-client-0.0.4/proton/_pysrp.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,57 +12,57 @@
 a,b  Secret ephemeral values
 A,B  Public ephemeral values
 x    Private key (derived from p and s)
 v    Password verifier
 """
 
 from .constants import SRP_LEN_BYTES, SALT_LEN_BYTES
-from .helpers import pm_hash, bytes_to_long, custom_hash, get_random_of_length, hash_password, long_to_bytes
+from .helpers import pm_hash, b2l, hash_custom, randl, hash_password, l2b
 
 
 def get_ng(n_bin: bytes, g_hex: bytes) -> tuple[int, int]:
-    return bytes_to_long(n_bin), int(g_hex, 16)
+    return b2l(n_bin), int(g_hex, 16)
 
 
 def hash_k(hash_class: callable, g: int, modulus: int, width: int) -> int:
     h = hash_class()
     h.update(g.to_bytes(width, 'little'))
     h.update(modulus.to_bytes(width, 'little'))
-    return bytes_to_long(h.digest())
+    return b2l(h.digest())
 
 
 def calc_x(hash_class: callable, salt: bytes, password: str, modulus: int) -> int:
-    mod = long_to_bytes(modulus, SRP_LEN_BYTES)
+    mod = l2b(modulus, SRP_LEN_BYTES)
     exp = hash_password(hash_class, password, salt, mod)
-    return bytes_to_long(exp)
+    return b2l(exp)
 
 
 def calc_client_proof(hash_class: callable, A: int, B: int, K: bytes) -> bytes:
     h = hash_class()
-    h.update(long_to_bytes(A, SRP_LEN_BYTES))
-    h.update(long_to_bytes(B, SRP_LEN_BYTES))
+    h.update(l2b(A, SRP_LEN_BYTES))
+    h.update(l2b(B, SRP_LEN_BYTES))
     h.update(K)
     return h.digest()
 
 
 def calc_server_proof(hash_class: callable, A: int, M: bytes, K: bytes) -> bytes:
     h = hash_class()
-    h.update(long_to_bytes(A, SRP_LEN_BYTES))
+    h.update(l2b(A, SRP_LEN_BYTES))
     h.update(M)
     h.update(K)
     return h.digest()
 
 
 class User(object):
     def __init__(self, password: str, n_bin: bytes, g_hex: bytes = b"2"):
         self.p = password
         self.hash_class = pm_hash
         self.N, self.g = get_ng(n_bin, g_hex)
         self.k = hash_k(self.hash_class, self.g, self.N, SRP_LEN_BYTES)
-        self.a = get_random_of_length(32)
+        self.a = randl(32)
         self.A = pow(self.g, self.a, self.N)
         self.expected_server_proof = None
         self._authenticated = False
         self.bytes_s = None
         self.v = None
         self.M = None
         self.K = None
@@ -71,45 +71,44 @@
         self.u = None
         self.x = None
 
     def authenticated(self) -> bool:
         return self._authenticated
 
     def get_ephemeral_secret(self) -> bytes:
-        return long_to_bytes(self.a, SRP_LEN_BYTES)
+        return l2b(self.a, SRP_LEN_BYTES)
 
     def get_session_key(self) -> bytes | None:
         return self.K if self._authenticated else None
 
     def get_challenge(self) -> bytes:
-        return long_to_bytes(self.A, SRP_LEN_BYTES)
-
+        return l2b(self.A, SRP_LEN_BYTES)
 
     def process_challenge(self, bytes_s: bytes, bytes_server_challenge: bytes) -> bytes | None:
         """ Returns M or None if SRP-6a safety check is violated """
         self.bytes_s = bytes_s
-        self.B = bytes_to_long(bytes_server_challenge)
+        self.B = b2l(bytes_server_challenge)
         # SRP-6a safety check
         if (self.B % self.N) == 0:
             return None
-        self.u = custom_hash(self.hash_class, self.A, self.B)
+        self.u = hash_custom(self.hash_class, self.A, self.B)
         # SRP-6a safety check
         if self.u == 0:
             return None
         self.x = calc_x(self.hash_class, self.bytes_s, self.p, self.N)
         self.v = pow(self.g, self.x, self.N)
         self.S = pow((self.B - self.k * self.v), (self.a + self.u * self.x), self.N)
-        self.K = long_to_bytes(self.S, SRP_LEN_BYTES)
+        self.K = l2b(self.S, SRP_LEN_BYTES)
         self.M = calc_client_proof(self.hash_class, self.A, self.B, self.K)  # noqa
         self.expected_server_proof = calc_server_proof(self.hash_class, self.A, self.M, self.K)
         return self.M
 
     def verify_session(self, server_proof: bytes) -> None:
         if self.expected_server_proof == server_proof:
             self._authenticated = True
 
     def compute_v(self, bytes_s: bytes = None) -> tuple[bytes, bytes]:
-        self.bytes_s = long_to_bytes(
-            get_random_of_length(SALT_LEN_BYTES),
+        self.bytes_s = l2b(
+            randl(SALT_LEN_BYTES),
             SALT_LEN_BYTES) if bytes_s is None else bytes_s
         self.x = calc_x(self.hash_class, self.bytes_s, self.p, self.N)
-        return self.bytes_s, long_to_bytes(pow(self.g, self.x, self.N), SRP_LEN_BYTES)
+        return self.bytes_s, l2b(pow(self.g, self.x, self.N), SRP_LEN_BYTES)
```

### Comparing `proton-api-client-0.0.3/proton/client.py` & `proton-api-client-0.0.4/proton/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from subprocess import Popen, PIPE
 
 import gnupg
 from selectolax.lexbor import LexborHTMLParser
 from tqdm import tqdm
 
+from .constants import PM_APP_VERSION_ACCOUNT
 from .login import login
 
 
 class ProtonMail:
     def __init__(self, username: str, password: str, gpg_passphrase: str = None):
         self.gpg = gnupg.GPG()
         self.gpg_passphrase = gpg_passphrase
@@ -18,14 +19,24 @@
 
     def salts(self):
         return self.client.get(f'{self.account_api}/core/v4/keys/salts').json()
 
     def users(self):
         return self.client.get(f'{self.account_api}/core/v4/users').json()
 
+    def sessions(self):
+        return self.client.get(f'{self.account_api}/auth/v4/sessions').json()
+
+    def info(self):
+        headers = dict(self.client.headers) | {'x-pm-appversion': PM_APP_VERSION_ACCOUNT}
+        return self.client.post(f'{self.account_api}/core/v4/auth/info', headers=headers).json()
+
+    def revoke_all_sessions(self):
+        self.client.delete(f'{self.account_api}/auth/v4/sessions')
+
     def gpg_import(self, fname: str, passphrase: str = None):
         self.gpg.import_keys_file(fname, passphrase=passphrase or self.gpg_passphrase)
 
     def gpg_decrypt(self, data: str, passphrase: str = None) -> str:
         return self.gpg.decrypt(data, passphrase=passphrase or self.gpg_passphrase).data.decode()
 
     def gpg_clean(self) -> list[dict]:
@@ -66,30 +77,25 @@
     def addresses(self, params: dict = None) -> dict:
         params = params or {
             'Page': 0,
             'PageSize': 150,  # max page size
         }
         return self.client.get(f'{self.api}/core/v4/addresses', params=params).json()
 
-    def info(self):
-        headers = dict(self.client.headers) | {'x-pm-appversion': 'web-account@5.0.35.1'}
-        return self.client.post(f'{self.account_api}/core/v4/auth/info', headers=headers).json()
-
     def inbox_decrypted(self, params: dict = None):
         """
         just testing things out - move into smaller and different functions
         """
         params = params or {
             'Page': 0,
             'PageSize': 150,  # max page size
             'LabelID': 0,
             'Sort': 'Time',
             'Desc': 1,
-            # 'Limit': 100,
-            # 'Attachments': 1, # only get messages with attachments
+            # 'Attachments': 1,  ## filter attachments
         }
         inbox = self.client.get(f"{self.api}/mail/v4/conversations", params=params).json()
         conversation_ids = [x.get('ID') for x in inbox.get('Conversations')]
 
         conversations_data = []
         for cid in conversation_ids:
             conversations_data.append(self.client.get(f"{self.api}/mail/v4/conversations/{cid}").json())
```

### Comparing `proton-api-client-0.0.3/proton/constants.py` & `proton-api-client-0.0.4/proton/constants.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 VERSION = "0.7.1"
-PM_APP_VERSION = 'web-mail@5.0.23.1'
-PM_API_VERSION = 4
+PM_APP_VERSION_MAIL = 'web-mail@5.0.23.1'
+PM_APP_VERSION_ACCOUNT = 'web-account@5.0.35.2'
+PM_API_VERSION = '4'
 SRP_LEN_BYTES = 256
 SALT_LEN_BYTES = 10
-
 DEFAULT_TIMEOUT = (3.05, 27)
 
 DEFAULT_HEADERS = {
     'authority': 'account.proton.me',
     'accept': 'application/vnd.protonmail.v1+json',
     'accept-language': 'en-GB,en;q=0.9',
     'content-type': 'application/json',
     'origin': 'https://account.proton.me',
     'referer': 'https://account.proton.me',
     'user-agent': 'Mozilla/5.0 (X11; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/113.0',
-    'x-pm-appversion': PM_APP_VERSION,
-    'x-pm-apiversion': f'{PM_API_VERSION}',
+    'x-pm-appversion': PM_APP_VERSION_MAIL,
+    'x-pm-apiversion': PM_API_VERSION,
 }
 
 DNS_HOSTS = [
     "https://dns11.quad9.net/dns-query",
     "https://dns.google/dns-query"
 ]
 ENCODED_URLS = [
```

### Comparing `proton-api-client-0.0.3/proton/helpers.py` & `proton-api-client-0.0.4/proton/helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import base64
 import hashlib
 import os
-import time
 from pathlib import Path
 
 import bcrypt
 import orjson
 
 from .constants import SRP_LEN_BYTES
 
@@ -28,53 +27,50 @@
         ])
 
 
 def pm_hash(b: bytes = b''):
     return PMHash(b)
 
 
-def bcrypt_b64_encode(s: bytes) -> bytes:
+def bcrypt_b64encode(s: bytes) -> bytes:
     bcrypt_base64 = b'./ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789'
     std_base64chars = b'ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/'
     s = base64.b64encode(s)
     return s.translate(bytes.maketrans(std_base64chars, bcrypt_base64))
 
 
 def hash_password(hash_class: callable, password: str, salt: bytes, modulus: bytes) -> bytes:
     salt = (salt + b'protonmail')[:16]
-    salt = bcrypt_b64_encode(salt)[:22]
+    salt = bcrypt_b64encode(salt)[:22]
     hashed = bcrypt.hashpw(password, b'$2y$10$' + salt)
     return hash_class(hashed + modulus).digest()
 
 
-def bytes_to_long(s: bytes) -> int:
+def b2l(s: bytes) -> int:
     return int.from_bytes(s, 'little')
 
 
-def long_to_bytes(n: int, nbytes: int) -> bytes:
+def l2b(n: int, nbytes: int) -> bytes:
     return n.to_bytes(nbytes, 'little')
 
 
-def get_random(nbytes: int) -> int:
-    return bytes_to_long(os.urandom(nbytes))
+def rand(nbytes: int) -> int:
+    return b2l(os.urandom(nbytes))
 
 
-def get_random_of_length(nbytes: int) -> int:
+def randl(nbytes: int) -> int:
     offset = (nbytes * 8) - 1
-    return get_random(nbytes) | (1 << offset)
+    return rand(nbytes) | (1 << offset)
 
 
-def custom_hash(hash_class: callable, *args) -> int:
+def hash_custom(hash_class: callable, *args) -> int:
     h = hash_class()
-    for s in args:
-        if s is not None:
-            data = long_to_bytes(s, SRP_LEN_BYTES) if isinstance(s, int) else s
-            h.update(data)
-    return bytes_to_long(h.digest())
+    for s in filter(None, args):
+        h.update(l2b(s, SRP_LEN_BYTES) if isinstance(s, int) else s)
+    return b2l(h.digest())
 
 
 def dump(path: str, **kwargs):
     fname, data = list(kwargs.items())[0]
     out = Path(path)
     out.mkdir(exist_ok=True, parents=True)
-    (out / f'{fname}_{time.time_ns()}.json').write_bytes(
-        orjson.dumps(data, option=orjson.OPT_INDENT_2 | orjson.OPT_SORT_KEYS))
+    (out / f'{fname}.json').write_bytes(orjson.dumps(data, option=orjson.OPT_INDENT_2 | orjson.OPT_SORT_KEYS))
```

### Comparing `proton-api-client-0.0.3/proton/login.py` & `proton-api-client-0.0.4/proton/login.py`

 * *Files identical despite different names*

### Comparing `proton-api-client-0.0.3/proton_api_client.egg-info/PKG-INFO` & `proton-api-client-0.0.4/proton_api_client.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proton-api-client
-Version: 0.0.3
+Version: 0.0.4
 Summary: Proton Mail API
 Home-page: https://github.com/trevorhobenshield/proton-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: proton api client async search automation bot scrape mail email
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
@@ -22,30 +22,36 @@
 username, password = ..., ...
 proton = ProtonMail(username, password)
 
 passphrase = 'myPass'
 pk = 'privatekey.hotmale@proton.me-6fdhskjgfd7s98gdgre87gregrjdhrgd7897g898.asc'
 proton.gpg_import(pk, passphrase=passphrase)
 
+
+sessions = proton.sessions()
+
 salts = proton.salts()
 
 users = proton.users()
 
 inbox = proton.inbox()
 
-conversation_id = inbox['Conversations'][0]['ID']
-conversation = proton.decrypt_conversation(conversation_id)
+cid = inbox['Conversations'][0]['ID']
+conversation = proton.decrypt_conversation(cid)
 
 decrypted_inbox = proton.inbox_decrypted()
 
 user_settings = proton.user_settings()
 
 mail_settings = proton.mail_settings()
 
 calendar_settings = proton.calendar_settings()
 
 timezones = proton.timezones()
 
 addresses = proton.addresses()
 
 info = proton.info()
+
+proton.revoke_all_sessions()
+
 ```
```

### Comparing `proton-api-client-0.0.3/setup.py` & `proton-api-client-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'orjson',
     'httpx',
     'tqdm',
 ]
 
 setup(
     name='proton-api-client',
-    version='0.0.3',
+    version='0.0.4',
     python_requires='>=3.10.10',
     description='Proton Mail API',
     long_description=dedent('''
     
     ### Proton Mail API
     
     #### Examples
@@ -29,36 +29,42 @@
     username, password = ..., ...
     proton = ProtonMail(username, password)
     
     passphrase = 'myPass'
     pk = 'privatekey.hotmale@proton.me-6fdhskjgfd7s98gdgre87gregrjdhrgd7897g898.asc'
     proton.gpg_import(pk, passphrase=passphrase)
     
-    salts = proton.salts()
     
+    sessions = proton.sessions()
+
+    salts = proton.salts()
+
     users = proton.users()
-    
+
     inbox = proton.inbox()
-    
-    conversation_id = inbox['Conversations'][0]['ID']
-    conversation = proton.decrypt_conversation(conversation_id)
-    
+
+    cid = inbox['Conversations'][0]['ID']
+    conversation = proton.decrypt_conversation(cid)
+
     decrypted_inbox = proton.inbox_decrypted()
-    
+
     user_settings = proton.user_settings()
-    
+
     mail_settings = proton.mail_settings()
-    
+
     calendar_settings = proton.calendar_settings()
-    
+
     timezones = proton.timezones()
-    
+
     addresses = proton.addresses()
-    
+
     info = proton.info()
+
+    proton.revoke_all_sessions()
+    
     ```
     '''),
     long_description_content_type='text/markdown',
     author='Trevor Hobenshield',
     author_email='trevorhobenshield@gmail.com',
     url='https://github.com/trevorhobenshield/proton-api-client',
     install_requires=install_requires,
```

