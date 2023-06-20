# Comparing `tmp/manabi-0.7.1.tar.gz` & `tmp/manabi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manabi-0.7.1.tar", max compression
+gzip compressed data, was "manabi-1.0.0.tar", max compression
```

## Comparing `manabi-0.7.1.tar` & `manabi-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     2037 2022-12-02 12:27:52.630976 manabi-0.7.1/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2022-11-10 12:16:37.030438 manabi-0.7.1/LICENSE
--rw-r--r--   0        0        0     2058 2022-11-10 12:16:37.030438 manabi-0.7.1/README.md
--rw-r--r--   0        0        0     1388 2022-11-11 11:40:01.080197 manabi-0.7.1/manabi/__init__.py
--rw-r--r--   0        0        0     4316 2022-11-10 12:16:37.030438 manabi-0.7.1/manabi/auth.py
--rw-r--r--   0        0        0     2407 2022-11-10 12:16:37.033772 manabi-0.7.1/manabi/filesystem.py
--rw-r--r--   0        0        0     8768 2022-12-02 12:22:49.562130 manabi-0.7.1/manabi/lock.py
--rw-r--r--   0        0        0     2730 2022-11-10 12:16:37.033772 manabi-0.7.1/manabi/log.py
--rw-r--r--   0        0        0     3839 2022-11-10 12:16:37.033772 manabi-0.7.1/manabi/token.py
--rw-r--r--   0        0        0     2166 2022-11-10 12:16:37.033772 manabi-0.7.1/manabi/util.py
--rw-r--r--   0        0        0        0 2022-11-10 12:16:37.033772 manabi-0.7.1/manabi_django/manabi_migrations/__init__.py
--rw-r--r--   0        0        0      165 2022-11-10 12:16:37.033772 manabi-0.7.1/manabi_django/manabi_migrations/apps.py
--rw-r--r--   0        0        0      532 2022-11-10 12:16:37.033772 manabi-0.7.1/manabi_django/manabi_migrations/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-11-10 12:16:37.033772 manabi-0.7.1/manabi_django/manabi_migrations/migrations/__init__.py
--rw-r--r--   0        0        0      200 2022-11-10 12:16:37.033772 manabi-0.7.1/manabi_django/manabi_migrations/models.py
--rw-r--r--   0        0        0     2130 2022-12-02 12:23:35.710143 manabi-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     3047 1970-01-01 00:00:00.000000 manabi-0.7.1/setup.py
--rw-r--r--   0        0        0     3356 1970-01-01 00:00:00.000000 manabi-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     2519 2023-06-20 12:52:14.834699 manabi-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2023-05-31 17:06:59.165102 manabi-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5260 2023-06-19 16:02:10.707837 manabi-1.0.0/README.md
+-rw-r--r--   0        0        0     1372 2023-06-15 12:40:23.020940 manabi-1.0.0/manabi/__init__.py
+-rw-r--r--   0        0        0     4300 2023-06-16 14:47:50.897983 manabi-1.0.0/manabi/auth.py
+-rw-r--r--   0        0        0     3471 2023-06-19 16:02:10.707837 manabi-1.0.0/manabi/filesystem.py
+-rw-r--r--   0        0        0    10021 2023-06-15 12:40:23.020940 manabi-1.0.0/manabi/lock.py
+-rw-r--r--   0        0        0     2681 2023-06-15 12:40:23.020940 manabi-1.0.0/manabi/log.py
+-rw-r--r--   0        0        0      273 2023-06-15 12:40:23.020940 manabi-1.0.0/manabi/mypy_fix.py
+-rw-r--r--   0        0        0     4401 2023-06-16 14:27:26.837088 manabi-1.0.0/manabi/token.py
+-rw-r--r--   0        0        0      410 2023-06-09 10:43:33.248961 manabi-1.0.0/manabi/type_alias.py
+-rw-r--r--   0        0        0     2763 2023-06-19 16:02:10.707837 manabi-1.0.0/manabi/util.py
+-rw-r--r--   0        0        0        0 2023-05-31 17:07:00.845155 manabi-1.0.0/manabi_django/manabi_migrations/__init__.py
+-rw-r--r--   0        0        0      165 2023-05-31 17:07:00.845155 manabi-1.0.0/manabi_django/manabi_migrations/apps.py
+-rw-r--r--   0        0        0      532 2023-05-31 17:07:00.845155 manabi-1.0.0/manabi_django/manabi_migrations/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-31 17:07:00.845155 manabi-1.0.0/manabi_django/manabi_migrations/migrations/__init__.py
+-rw-r--r--   0        0        0      200 2023-05-31 17:07:00.845155 manabi-1.0.0/manabi_django/manabi_migrations/models.py
+-rw-r--r--   0        0        0     2428 2023-06-20 12:34:52.252687 manabi-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6510 1970-01-01 00:00:00.000000 manabi-1.0.0/PKG-INFO
```

### Comparing `manabi-0.7.1/CHANGELOG.md` & `manabi-1.0.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.0.0 (2023-06-20)
+
+### Feature
+* feat(hook): add pre_write_hook ([`4de0ad6`](https://github.com/projectcaluma/manabi/commit/4de0ad65b95bbd0be5fa19ed986660233fcd6b6c))
+
+### Fix
+* fix: fuzzying found relative urls like '..' ([`e74b263`](https://github.com/projectcaluma/manabi/commit/e74b2638f9413b339988dea52eb2b8747262a2dc))
+
+### Feature
+* feat(hook): add payload to token ([`7679f9d`](https://github.com/projectcaluma/manabi/commit/7679f9d2d1a87fd933c5af109bfb1ec244a0c480))
+
 ## v0.7.1 (2022-12-02)
 
 ### Fix
 * **postgres:** Reconnect on OperationalError too ([`c6f587f`](https://github.com/projectcaluma/manabi/commit/c6f587f6b855d8053536f99a6cc6afe654e44eb9))
 
 ## v0.7.0 (2022-11-11)
```

### Comparing `manabi-0.7.1/LICENSE` & `manabi-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `manabi-0.7.1/manabi/__init__.py` & `manabi-1.0.0/manabi/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from wsgidav import http_authenticator  # type: ignore
-from wsgidav.http_authenticator import HTTPAuthenticator  # type: ignore
-from wsgidav.wsgidav_app import WsgiDAVApp  # type: ignore
+from wsgidav import http_authenticator
+from wsgidav.http_authenticator import HTTPAuthenticator
+from wsgidav.wsgidav_app import WsgiDAVApp
 
 from .auth import ManabiAuthenticator
 
 
 class ManabiDAVApp(WsgiDAVApp):
     def __init__(self, config):
         super().__init__(config)
-        self.lock_manager._lock = config["lock_storage"]._lock
+        self.lock_manager._lock = config["lock_storage"]._lock  # type: ignore
 
 
 class MetaFakeHTTPAuthenticator(type(http_authenticator.HTTPAuthenticator)):  # type: ignore
     def __instancecheck__(cls, instance):
         return isinstance(instance, HTTPAuthenticator) or isinstance(
             instance, ManabiAuthenticator
         )
@@ -27,15 +27,15 @@
 # Instead of accepting an override for HTTPAuthenticator as for everything else, wsgidav
 # just expects a class extending HTTPAuthenticator in the middleware_stack.
 # wsgidav grabs that class out of the middleware_stack.
 #
 # Using a metaclass is slightly less intrusive than just replacing HTTPAuthenticator
 # with ManabiAuthenticator. If http_authenticator.HTTPAuthenticator is created it is
 # still a HTTPAuthenticator.
-http_authenticator.HTTPAuthenticator = FakeHTTPAuthenticator
+http_authenticator.HTTPAuthenticator = FakeHTTPAuthenticator  # type: ignore
 
 
 def keygen() -> None:
     from .util import to_string
 
     with open("/dev/random", "rb") as f:
         print(to_string(f.read(32)))
```

### Comparing `manabi-0.7.1/manabi/auth.py` & `manabi-1.0.0/manabi/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from functools import partial
 from http.cookies import SimpleCookie
 from typing import Any, Callable, Dict, List
 from unittest.mock import MagicMock
 
-from wsgidav.mw.base_mw import BaseMiddleware  # type: ignore
+from wsgidav.mw.base_mw import BaseMiddleware
 
 from .token import Config, State, Token
 from .util import AppInfo, get_rfc1123_time, set_cookie
 
 _error_message_403 = """
 <html>
     <head><title>403 Forbidden</title></head>
```

### Comparing `manabi-0.7.1/manabi/lock.py` & `manabi-1.0.0/manabi/lock.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,79 @@
 import fcntl
 import json
 import shelve
 import threading
 import traceback
 import weakref
+from abc import ABC, abstractmethod
 from collections.abc import MutableMapping
 from pathlib import Path
+from typing import Callable
 
 import psycopg2.extensions
 from psycopg2 import InterfaceError, OperationalError, connect
-from wsgidav.lock_man.lock_storage import LockStorageDict  # type: ignore
-from wsgidav.util import get_module_logger  # type: ignore
+from psycopg2.extensions import connection as PsycopgConnection
+from wsgidav.lock_man.lock_storage import LockStorageDict
+from wsgidav.util import get_module_logger
 
 _logger = get_module_logger(__name__)
 
 
 class ManabiTimeoutMixin:
+    _max_timeout: float = 0
+
+    @property
+    def max_timeout(self) -> float:
+        return self._max_timeout
+
+    @max_timeout.setter
+    def max_timeout(self, value: float) -> None:
+        if value <= 0:
+            raise ValueError("max_timeout must be a positive integer.")
+        self._max_timeout = value
+
     def set_timeout(self, lock):
         max_timeout = self.max_timeout
         timeout = lock.get("timeout")
 
         if not timeout:
             lock["timeout"] = max_timeout
         else:
             if timeout > max_timeout:
                 lock["timeout"] = max_timeout
 
 
-class ManabiContextLockMixin:
+class ManabiContextLockMixin(ABC):
+    @abstractmethod
+    def acquire(self):
+        pass
+
+    @abstractmethod
+    def release(self):
+        pass
+
     def __enter__(self):
         self.acquire()
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.release()
 
 
 class ManabiShelfLock(ManabiContextLockMixin):
-    def __init__(self, storage_path, storage_object):
+    _storage_object: Callable[[], "ManabiShelfLockLockStorage"]
+
+    def __init__(self, storage_path, storage_object: "ManabiShelfLockLockStorage"):
         self._storage_path = storage_path
-        self._storage_object = weakref.ref(storage_object)
+        # type manually checked
+        self._storage_object = weakref.ref(storage_object)  # type: ignore
         self._semaphore = 0
         self._lock_file = open(f"{storage_path}.lock", "wb+")
         self._fd = self._lock_file.fileno()
         self.acquire_write = self.acquire_read = self.acquire
-        self._id = None
+        self._id = -1
 
     def acquire(self):
         tid = threading.get_ident()
         if self._id and self._id != tid:
             _logger.error("Do not use from multiple threads")
         self._id = tid
         if self._semaphore == 0:
@@ -63,26 +89,28 @@
             )
         if self._id and self._id != tid:
             _logger.error("Do not use from multiple threads")
         self._id = tid
         self._semaphore -= 1
         if self._semaphore == 0:
             storage_object = self._storage_object()
-            storage_object._dict.close()
-            storage_object._dict = None
+            if storage_object._dict is not None:
+                storage_object._dict.close()
+                storage_object._dict = None
             fcntl.flock(self._fd, fcntl.LOCK_UN)
         self._id = threading.get_ident()
 
 
 class ManabiShelfLockLockStorage(LockStorageDict, ManabiTimeoutMixin):
     def __init__(self, refresh: float, storage: Path):
         super().__init__()
         self.max_timeout = refresh / 2
         self._storage = storage
-        self._lock = ManabiShelfLock(storage, self)
+        # this is a cast
+        self._lock: ManabiShelfLock = ManabiShelfLock(storage, self)  # type:ignore
 
     def open(self):
         pass
 
     def close(self):
         pass
 
@@ -115,49 +143,57 @@
                 include_root=include_root,
                 include_children=include_children,
                 token_only=token_only,
             )
 
 
 class ManabiPostgresLock(ManabiContextLockMixin):
-    def __init__(self, storage):
+    _storage_object: Callable[[], "ManabiDbLockStorage"]
+
+    def __init__(self, storage_object: "ManabiDbLockStorage"):
         self._id = None
-        self.storage = weakref.ref(storage)
+        # type manually checked
+        self._storage_object = weakref.ref(storage_object)  # type: ignore
         self.acquire_write = self.acquire_read = self.acquire
         self._semaphore = 0
-        self._id = None
+        self._id = -1
 
     def acquire(self):
         tid = threading.get_ident()
         if self._id and self._id != tid:
             _logger.error("Do not use from multiple threads")
         self._id = tid
         if self._semaphore == 0:
             _logger.info(f"{tid} acquire")
-            self.storage().execute("LOCK TABLE manabi_lock IN ACCESS EXCLUSIVE MODE")
+            self._storage_object().execute(
+                "LOCK TABLE manabi_lock IN ACCESS EXCLUSIVE MODE"
+            )
         self._semaphore += 1
 
     def release(self):
         tid = threading.get_ident()
         if self._semaphore == 0:
             _logger.error(
                 f"Inconsistent use of lock. {''.join(traceback.format_stack())}"
             )
         if self._id and self._id != tid:
             _logger.error("Do not use from multiple threads")
         self._id = tid
         self._semaphore -= 1
         if self._semaphore == 0:
             _logger.info(f"{tid} release")
-            self.storage()._connection.commit()
+            self._storage_object()._connection.commit()
 
 
 class ManabiPostgresDict(MutableMapping):
-    def __init__(self, storage, lock):
-        self.storage = weakref.ref(storage)
+    _storage_object: Callable[[], "ManabiDbLockStorage"]
+
+    def __init__(self, storage_object: "ManabiDbLockStorage", lock):
+        # type manually checked
+        self._storage_object = weakref.ref(storage_object)  # type: ignore
         self._lock = lock
 
     @staticmethod
     def decode_lock(lock):
         if "owner" in lock:
             owner = lock["owner"]
             if isinstance(owner, bytes):
@@ -168,80 +204,82 @@
         if "owner" in lock:
             owner = lock["owner"]
             if "manabi_was_bytes" in owner:
                 lock["owner"] = owner["manabi_was_bytes"].encode("UTF-8")
 
     def cleanup(self):
         with self._lock:
-            self.storage().execute("DELETE FROM manabi_lock;")
+            self._storage_object().execute("DELETE FROM manabi_lock;")
 
     def __len__(self):
         with self._lock:
-            cursor = self.storage().execute("SELECT count(*) FROM manabi_lock")
+            cursor = self._storage_object().execute("SELECT count(*) FROM manabi_lock")
             return int(cursor.fetchone()[0])
 
     def __iter__(self):
         with self._lock:
-            cursor = self.storage().execute("SELECT token FROM manabi_lock")
+            cursor = self._storage_object().execute("SELECT token FROM manabi_lock")
             for token in cursor.fetchall():
                 yield token[0]
 
     def __delitem__(self, token):
         with self._lock:
-            self.storage().execute(
+            self._storage_object().execute(
                 "DELETE FROM manabi_lock WHERE token = %s", (str(token),)
             )
 
     def __contains__(self, token):
         with self._lock:
-            cursor = self.storage().execute(
+            cursor = self._storage_object().execute(
                 "SELECT 1 FROM manabi_lock WHERE token = %s", (str(token),)
             )
             if cursor.fetchone() is None:
                 return False
             else:
                 return True
 
     def __setitem__(self, token, lock):
         with self._lock:
             self.decode_lock(lock)
             json_lock = json.dumps(lock)
-            self.storage().execute(
+            self._storage_object().execute(
                 """
                     INSERT INTO manabi_lock(token, data) VALUES (%(token)s, %(data)s)
                         ON CONFLICT(token) DO
                         UPDATE SET data = %(data)s WHERE manabi_lock.token = %(token)s
                 """,
                 {
                     "token": token,
                     "data": json_lock,
                 },
             )
 
     def __getitem__(self, token):
         with self._lock:
-            cursor = self.storage().execute(
+            cursor = self._storage_object().execute(
                 "SELECT data FROM manabi_lock WHERE token = %s", (str(token),)
             )
             lock = cursor.fetchone()
             if lock is None:
                 raise KeyError(f"{token} not found")
             lock = lock[0]
             self.encode_lock(lock)
             return lock
 
 
 class ManabiDbLockStorage(LockStorageDict, ManabiTimeoutMixin):
+    _connection: PsycopgConnection
+
     def __init__(self, refresh: float, postgres_dsn: str):
         super().__init__()
         self._postgres_dsn = postgres_dsn
         self.max_timeout = refresh / 2
-        self._connection = None
         self.connect()
-        self._lock = ManabiPostgresLock(self)
+        # this is a cast
+        self._lock: ManabiPostgresLock = ManabiPostgresLock(self)  # type: ignore
         self._dict = ManabiPostgresDict(self, self._lock)
 
     def connect(self):
         try:
             if self._connection:
                 # it the connecton failed, this might cause an exception, we do not care.
                 self._connection.close()
```

### Comparing `manabi-0.7.1/manabi/log.py` & `manabi-1.0.0/manabi/log.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 from functools import partial
 from typing import Any, Callable, Dict, List, Tuple
 
-from wsgidav.mw.base_mw import BaseMiddleware  # type: ignore
-from wsgidav.util import (  # type: ignore
-    SubAppStartResponse,
-    get_module_logger,
-    init_logging,
-)
+from wsgidav.mw.base_mw import BaseMiddleware
+from wsgidav.util import SubAppStartResponse, get_module_logger, init_logging
 
 _logger = get_module_logger(__name__)
 
 
 class HeaderLogger(BaseMiddleware):
     def logger(
         self,
```

### Comparing `manabi-0.7.1/manabi/token.py` & `manabi-1.0.0/manabi/token.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import calendar
 import struct
 from datetime import datetime
 from enum import Enum
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Tuple, Union
 
+import umsgpack  # type: ignore
 from attr import Factory, dataclass
 from branca import Branca  # type: ignore
 
+from .type_alias import OptionalProp, PropType
 from .util import cattrib, from_string
 
 
 def now() -> int:
     return calendar.timegm(datetime.utcnow().timetuple())
 
 
@@ -53,14 +55,15 @@
     invalid = 4, "the token is not valid, authentication failed"
 
 
 @dataclass
 class Token:
     key: Key = cattrib(Key)
     path: Optional[Path] = cattrib(Path, default=None)
+    payload: OptionalProp = cattrib(OptionalProp, default=None)
     timestamp: Optional[int] = cattrib(
         int, default=Factory(lambda: now()), optional=True
     )
     ciphertext: str = cattrib(str, default=None)
 
     def as_url(self) -> str:
         if self.path is None:
@@ -72,37 +75,42 @@
         return f"/{self.path}"
 
     def encode(self) -> str:
         if self.path is None:
             raise ValueError("path may not be None")
         if self.timestamp is None:
             self.timestamp = now()
-        self.ciphertext = _encode(self.key.data, str(self.path), self.timestamp)
+        self.ciphertext = _encode(
+            self.key.data,
+            str(self.path),
+            self.payload,
+            self.timestamp,
+        )
         return self.ciphertext
 
     @classmethod
-    def from_token(cls, token: "Token", timestamp: int = None) -> "Token":
+    def from_token(cls, token: "Token", timestamp: Optional[int] = None) -> "Token":
         if timestamp is None:
-            return cls(token.key, token.path, now())
+            return cls(token.key, token.path, token.payload, now())
         else:
-            return cls(token.key, token.path, timestamp)
+            return cls(token.key, token.path, token.payload, timestamp)
 
     @classmethod
     def from_ciphertext(cls, key: Key, ciphertext: str) -> "Token":
         assert ciphertext
         branca = Branca(key.data)
         try:
             timestamp = branca.timestamp(ciphertext)
         except (struct.error, ValueError):
             return cls(key, None, None)
         try:
-            token_path = Path(branca.decode(ciphertext).decode("UTF-8"))
+            token_path, token_payload = _decode(branca, ciphertext)
         except RuntimeError:
             return cls(key, None, timestamp)
-        return cls(key, token_path, timestamp, ciphertext)
+        return cls(key, token_path, token_payload, timestamp, ciphertext)
 
     def check(self, ttl: Optional[int] = None) -> State:
         if self.path is None or self.timestamp is None:
             return State.invalid
         if ttl is not None:
             future = self.timestamp + ttl
             past = self.timestamp - 1
@@ -116,17 +124,31 @@
     def refresh(self, ttl: TTL) -> State:
         return self.check(ttl.refresh)
 
     def initial(self, ttl: TTL) -> State:
         return self.check(ttl.initial)
 
 
-def _encode(key: bytes, path: str, now: Optional[int] = None) -> str:
+def _encode(
+    key: bytes,
+    path: str,
+    payload: OptionalProp = None,
+    now: Optional[int] = None,
+) -> str:
     f = Branca(key)
-    p = path.encode("UTF-8")
+    p = umsgpack.packb((path.encode("UTF-8"), payload))
     ciphertext = f.encode(p, now)
     return ciphertext
 
 
-def _decode(key: bytes, ciphertext: str, ttl=None) -> str:
-    f = Branca(key)
-    return f.decode(ciphertext, ttl).decode("UTF-8")
+def _decode(
+    key: Union[bytes, Branca],
+    ciphertext: str,
+    ttl=None,
+) -> Tuple[Path, PropType]:
+    if isinstance(key, Branca):
+        f = key
+    else:
+        f = Branca(key)
+    tpb, token_payload = umsgpack.unpackb(f.decode(ciphertext, ttl))
+    token_path = tpb.decode("UTF-8")
+    return Path(token_path), token_payload
```

### Comparing `manabi-0.7.1/manabi/util.py` & `manabi-1.0.0/manabi/util.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,65 @@
 import calendar
+import threading
 from datetime import datetime
 from email.utils import formatdate
 from http.cookies import SimpleCookie
 from inspect import getsource
 from typing import Any, Callable, Dict, List, Optional, Tuple, cast
 
 import base62  # type: ignore
+import requests
 from attr import attrib, dataclass
 
+from .type_alias import TypeType
+
+_local_session = threading.local()
+
+
+def requests_session() -> requests.Session:
+    """Wsgidav uses threading, lets get a session per thread."""
+    local_dict = _local_session.__dict__
+    session = local_dict.get("session")
+    if not session:
+        local_dict["session"] = session = requests.Session()
+    return session
+
 
 def cattrib(
-    attrib_type: Optional[type] = None,
+    attrib_type: Optional[TypeType] = None,
     check: Optional[Callable] = None,
     optional: bool = False,
     **kwargs,
 ):
     if "default" in kwargs and kwargs["default"] is None:
         optional = True
 
     def handler(object, attribute, value):
         if value is None and optional:
             return value
-        if attrib_type is not None and not isinstance(value, attrib_type):
+        # Some python versions cannot do the check assume True
+        is_inst = True
+        try:
+            if attrib_type is not None:
+                is_inst = isinstance(value, attrib_type)
+        except TypeError:
+            pass
+        if not is_inst:
             raise TypeError(
                 f"{attribute.name} ({type(value)}) is not of type {attrib_type}"
             )
         if check and not check(value):
             source = getsource(check).strip()
             raise ValueError(f"check failed: {source}")
         return value
 
     return attrib(validator=handler, on_setattr=handler, **kwargs)
 
 
-def get_rfc1123_time(secs: float = None) -> str:
+def get_rfc1123_time(secs: Optional[float] = None) -> str:
     """Return <secs> in rfc 1123 date/time format (pass secs=None for current date)."""
     return formatdate(timeval=secs, localtime=False, usegmt=True)
 
 
 def to_string(data: bytes) -> str:
     return base62.encodebytes(data)
```

### Comparing `manabi-0.7.1/manabi_django/manabi_migrations/migrations/0001_initial.py` & `manabi-1.0.0/manabi_django/manabi_migrations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `manabi-0.7.1/pyproject.toml` & `manabi-1.0.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "manabi"
-version = "0.7.1"
+version = "1.0.0"
 description = "Provide WebDAV access for documents."
 homepage = "https://github.com/projectcaluma/manabi"
 repository = "https://github.com/projectcaluma/manabi"
 authors = ["Adfinis AG"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 classifiers = [
@@ -26,42 +26,46 @@
 ]
 packages = [
     { include = "manabi" },
     { include = "manabi_migrations", from = "manabi_django" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.8.1"
 WsgiDAV = "^4.0.2"
 pybranca = "^0.5.0"
-pybase62 = "^0.5.0"
-attrs = "^22.1.0"
+pybase62 = "^1.0.0"
+attrs = "^23.1.0"
 django = "^3.2.15"
 psycopg2-binary = "^2.9.3"
+u-msgpack-python = "^2.8.0"
 
-[tool.poetry.dev-dependencies]
-black = "22.8.0"
-cheroot = "8.6.0"
-flake8 = "5.0.4"
-flake8-bugbear = "22.9.23"
-flake8-debugger = "4.1.2"
-flake8-docstrings = "1.6.0"
-flake8-isort = "4.2.0"
-flake8-string-format = "0.3.0"
-flake8-tuple = "0.4.1"
-hypothesis = "6.54.6"
-isort = "5.10.1"
-mypy = "0.981"
-pdbpp = "0.10.3"
-pytest = "7.1.3"
-python-language-server = "0.36.2"
-python-semantic-release = "7.32.0"
-requests = "2.28.1"
-types-psycopg2 = "2.9.21"
-types-requests = "2.28.11"
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+cheroot = "^10.0.0"
+flake8 = "^6.0.0"
+flake8-bugbear = "^23.5.9"
+flake8-debugger = "^4.1.2"
+flake8-docstrings = "^1.7.0"
+flake8-isort = "^6.0.0"
+flake8-string-format = "^0.3.0"
+flake8-tuple = "^0.4.1"
+hypothesis = "^6.54.6"
+mypy = "^1.3.0"
+pdbpp = "^0.10.3"
+pytest = "^7.3.1"
+python-semantic-release = "^7.32.0"
+requests = "^2.28.1"
+types-psycopg2 = "^2.9.21"
+types-requests = "^2.28.11"
+python-lsp-server = "^1.7.3"
+python-lsp-black = "^1.3.0"
+python-lsp-isort = "^0.1"
+flake8-pyproject = "^1.2.3"
+requests-mock = "^1.11.0"
 
 [tool.isort]
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 combine_as_imports = true
 line_length = 88
@@ -72,13 +76,30 @@
 major_on_zero = false
 upload_to_repository = true
 upload_to_release = true
 build_command = "poetry build"
 commit_subject = "chore(release): v{version}"
 commit_author = "github-actions <github-actions@github.com>"
 
-# No flake8 pyproject support yet, please edit .flake8
+[tool.mypy]
+check_untyped_defs = true
+
+[tool.flake8]
+ignore = """
+    E501,
+    D100,
+    D101,
+    D102,
+    D103,
+    D104,
+    D105,
+    D106,
+    D107,
+    W503
+    E203,
+"""
+max_line_length = 88
+doctests = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
-
+build-backend = "poetry.core.masonry.api"
```

