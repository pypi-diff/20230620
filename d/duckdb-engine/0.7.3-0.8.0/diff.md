# Comparing `tmp/duckdb_engine-0.7.3.tar.gz` & `tmp/duckdb_engine-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckdb_engine-0.7.3.tar", max compression
+gzip compressed data, was "duckdb_engine-0.8.0.tar", max compression
```

## Comparing `duckdb_engine-0.7.3.tar` & `duckdb_engine-0.8.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1076 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/LICENSE.txt
--rw-r--r--   0        0        0     5953 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/README.md
--rw-r--r--   0        0        0        4 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/7210af19145ec2a8
--rw-r--r--   0        0        0        1 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/bec021b4f368e306
--rw-r--r--   0        0        0    20688 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz
--rw-r--r--   0        0        0    11629 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/__init__.py
--rw-r--r--   0        0        0      985 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/config.py
--rw-r--r--   0        0        0        0 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/conftest.py
--rw-r--r--   0        0        0     2198 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/datatypes.py
--rw-r--r--   0        0        0        0 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/py.typed
--rw-r--r--   0        0        0        0 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/tests/__init__.py
--rw-r--r--   0        0        0     1042 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/tests/snapshots/__init__.py
--rw-r--r--   0        0        0      338 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/tests/snapshots/snap_test_basic.py
--rw-r--r--   0        0        0    10426 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/tests/test_basic.py
--rw-r--r--   0        0        0     3185 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/tests/test_datatypes.py
--rw-r--r--   0        0        0      948 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/tests/test_ibis.py
--rw-r--r--   0        0        0      455 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/tests/test_integration.py
--rw-r--r--   0        0        0     3946 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/tests/test_pandas.py
--rw-r--r--   0        0        0      257 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/duckdb_engine/tests/util.py
--rw-r--r--   0        0        0     1370 2023-05-19 14:15:32.534209 duckdb_engine-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     6867 1970-01-01 00:00:00.000000 duckdb_engine-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     5953 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/README.md
+-rw-r--r--   0        0        0        4 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/7210af19145ec2a8
+-rw-r--r--   0        0        0        1 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/.hypothesis/examples/f024fc7dfe5f1878/bec021b4f368e306
+-rw-r--r--   0        0        0    20688 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz
+-rw-r--r--   0        0        0    11754 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/__init__.py
+-rw-r--r--   0        0        0     1096 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/config.py
+-rw-r--r--   0        0        0        0 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/conftest.py
+-rw-r--r--   0        0        0     5731 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/datatypes.py
+-rw-r--r--   0        0        0        0 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/py.typed
+-rw-r--r--   0        0        0        0 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/tests/__init__.py
+-rw-r--r--   0        0        0     1209 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/tests/snapshots/__init__.py
+-rw-r--r--   0        0        0      338 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/tests/snapshots/snap_test_basic.py
+-rw-r--r--   0        0        0    11218 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/tests/test_basic.py
+-rw-r--r--   0        0        0     4016 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/tests/test_datatypes.py
+-rw-r--r--   0        0        0      948 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/tests/test_ibis.py
+-rw-r--r--   0        0        0     1740 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/tests/test_integration.py
+-rw-r--r--   0        0        0     3946 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/tests/test_pandas.py
+-rw-r--r--   0        0        0      257 2023-06-20 15:20:50.022194 duckdb_engine-0.8.0/duckdb_engine/tests/util.py
+-rw-r--r--   0        0        0     1403 2023-06-20 15:20:50.026194 duckdb_engine-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     6867 1970-01-01 00:00:00.000000 duckdb_engine-0.8.0/PKG-INFO
```

### Comparing `duckdb_engine-0.7.3/LICENSE.txt` & `duckdb_engine-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.3/README.md` & `duckdb_engine-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.3/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz` & `duckdb_engine-0.8.0/duckdb_engine/.hypothesis/unicode_data/12.1.0/charmap.json.gz`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.3/duckdb_engine/__init__.py` & `duckdb_engine-0.8.0/duckdb_engine/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from sqlalchemy.dialects.postgresql.psycopg2 import PGDialect_psycopg2
 from sqlalchemy.engine.default import DefaultDialect
 from sqlalchemy.engine.url import URL
 
 from .config import apply_config, get_core_config
 from .datatypes import ISCHEMA_NAMES, register_extension_types
 
-__version__ = "0.7.3"
+__version__ = "0.8.0"
 
 if TYPE_CHECKING:
     from sqlalchemy.base import Connection
     from sqlalchemy.engine.interfaces import _IndexDict
 
 
 register_extension_types()
@@ -192,15 +192,16 @@
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         kwargs["use_native_hstore"] = False
         super().__init__(*args, **kwargs)
 
     def connect(self, *cargs: Any, **cparams: Any) -> "Connection":
         core_keys = get_core_config()
         preload_extensions = cparams.pop("preload_extensions", [])
-        config = cparams.get("config", {})
+        config = cparams.setdefault("config", {})
+        config.update(cparams.pop("url_config", {}))
 
         ext = {k: config.pop(k) for k in list(config) if k not in core_keys}
 
         conn = duckdb.connect(*cargs, **cparams)
 
         for extension in preload_extensions:
             conn.execute(f"LOAD {extension}")
@@ -277,15 +278,17 @@
         index_warning()
         return []
 
     def initialize(self, connection: "Connection") -> None:
         DefaultDialect.initialize(self, connection)
 
     def create_connect_args(self, url: URL) -> Tuple[tuple, dict]:
-        return (), url.translate_connect_args(database="database")
+        opts = url.translate_connect_args(database="database")
+        opts["url_config"] = dict(url.query)
+        return (), opts
 
     @classmethod
     def import_dbapi(cls: Type["Dialect"]) -> Type[DBAPI]:
         return cls.dbapi()
 
     def do_executemany(
         self, cursor: Any, statement: Any, parameters: Any, context: Optional[Any] = ...
```

### Comparing `duckdb_engine-0.7.3/duckdb_engine/config.py` & `duckdb_engine-0.8.0/duckdb_engine/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 @lru_cache()
 def get_core_config() -> Set[str]:
     rows = (
         duckdb.connect(":memory:")
         .execute("SELECT name FROM duckdb_settings()")
         .fetchall()
     )
-    return {name for name, in rows}
+    # special case for motherduck here - they accept this config at extension load time
+    return {name for name, in rows} | {"motherduck_token"}
 
 
 def apply_config(
     dialect: Dialect,
     conn: duckdb.DuckDBPyConnection,
     ext: Dict[str, Union[str, int, bool]],
 ) -> None:
```

### Comparing `duckdb_engine-0.7.3/duckdb_engine/tests/conftest.py` & `duckdb_engine-0.8.0/duckdb_engine/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,23 @@
+import warnings
 from functools import wraps
 from typing import Any, Callable, TypeVar
 
 from pytest import fixture, raises
 from sqlalchemy import create_engine
 from sqlalchemy.dialects import registry  # type: ignore
 from sqlalchemy.engine import Engine
 from sqlalchemy.orm import Session, sessionmaker
 from typing_extensions import ParamSpec
 
+warnings.filterwarnings(
+    "ignore",
+    "distutils Version classes are deprecated. Use packaging.version instead.",
+    DeprecationWarning,
+)
 P = ParamSpec("P")
 
 FuncT = TypeVar("FuncT", bound=Callable[..., Any])
 
 
 @fixture
 def engine() -> Engine:
```

### Comparing `duckdb_engine-0.7.3/duckdb_engine/tests/test_basic.py` & `duckdb_engine-0.8.0/duckdb_engine/tests/test_basic.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,14 +177,15 @@
     assert views == ["test"]
 
     views = engine.dialect.get_view_names(con, schema="scheme")
     assert views == ["schema_test"]
 
 
 @mark.skipif(os.uname().machine == "aarch64", reason="not supported on aarch64")
+@mark.remote_data
 def test_preload_extension() -> None:
     duckdb.default_connection.execute("INSTALL httpfs")
     engine = create_engine(
         "duckdb:///",
         connect_args={
             "preload_extensions": ["httpfs"],
             "config": {"s3_region": "ap-southeast-2", "s3_use_ssl": True},
@@ -359,14 +360,41 @@
         DBAPIError,
         match='Cannot execute statement of type "CREATE" (on database "test" which is attached )?in read-only mode!',
     ):
         with eng.connect() as conn:
             conn.execute(text("create table hello2 (i int)"))
 
 
+def test_url_config() -> None:
+    eng = create_engine("duckdb:///:memory:?worker_threads=123")
+
+    with eng.connect() as conn:
+        res = conn.execute(text("select current_setting('worker_threads')"))
+        row = res.first()
+        assert row is not None
+        assert row[0] == 123
+
+
+def test_url_config_and_dict_config() -> None:
+    eng = create_engine(
+        "duckdb:///:memory:?worker_threads=123",
+        connect_args={"config": {"memory_limit": "500mb"}},
+    )
+
+    with eng.connect() as conn:
+        res = conn.execute(
+            text(
+                "select current_setting('worker_threads'), current_setting('memory_limit')"
+            )
+        )
+        row = res.first()
+        assert row is not None
+        assert row == (123, "500.0MB")
+
+
 def test_do_ping(tmp_path: Path, caplog: LogCaptureFixture) -> None:
     engine = create_engine(
         "duckdb:///" + str(tmp_path / "db"), pool_pre_ping=True, pool_size=1
     )
 
     logger = cast(logging.Logger, engine.pool.logger)  # type: ignore
     logger.setLevel(logging.DEBUG)
```

### Comparing `duckdb_engine-0.7.3/duckdb_engine/tests/test_datatypes.py` & `duckdb_engine-0.8.0/duckdb_engine/tests/test_datatypes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import warnings
 from typing import Type
 from uuid import uuid4
 
 import duckdb
 from pytest import importorskip, mark
-from sqlalchemy import Column, Integer, MetaData, Table, inspect, text
+from sqlalchemy import Column, Integer, MetaData, String, Table, inspect, text
 from sqlalchemy.dialects.postgresql import UUID
 from sqlalchemy.engine import Engine
 from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy.orm import Session
 from sqlalchemy.sql import sqltypes
 from sqlalchemy.types import JSON
 
-from ..datatypes import types
+from ..datatypes import Map, Struct, types
 
 
 @mark.parametrize("coltype", types)
 def test_unsigned_integer_type(
     engine: Engine, session: Session, coltype: Type[Integer]
 ) -> None:
     Base = declarative_base()
@@ -110,7 +110,33 @@
             if name.endswith("_enum") and duckdb.__version__ < "0.7.1":  # type: ignore[attr-defined]
                 continue
             if "array" in name or "struct" in name or "map" in name:
                 assert col.type == sqltypes.NULLTYPE, name
             else:
                 assert col.type != sqltypes.NULLTYPE, name
         assert not capture
+
+
+def test_nested_types(engine: Engine, session: Session) -> None:
+    importorskip("duckdb", "0.5.0")  # nested types require at least duckdb 0.5.0
+    base = declarative_base()
+
+    class Entry(base):
+        __tablename__ = "test_struct"
+
+        id = Column(Integer, primary_key=True, default=0)
+        struct = Column(Struct(fields={"name": String}))
+        map = Column(Map(String, Integer))
+        # union = Column(Union(fields={"name": String, "age": Integer}))
+
+    base.metadata.create_all(bind=engine)
+
+    struct_data = {"name": "Edgar"}
+    map_data = {"one": 1, "two": 2}
+
+    session.add(Entry(struct=struct_data, map=map_data))  # type: ignore[call-arg]
+    session.commit()
+
+    result = session.query(Entry).one()
+
+    assert result.struct == struct_data
+    assert result.map == map_data
```

### Comparing `duckdb_engine-0.7.3/duckdb_engine/tests/test_ibis.py` & `duckdb_engine-0.8.0/duckdb_engine/tests/test_ibis.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.3/duckdb_engine/tests/test_pandas.py` & `duckdb_engine-0.8.0/duckdb_engine/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `duckdb_engine-0.7.3/pyproject.toml` & `duckdb_engine-0.8.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "duckdb_engine"
-version = "0.7.3"
+version = "0.8.0"
 description = "SQLAlchemy driver for duckdb"
 authors = ["Elliana <me@mause.me>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Mause/duckdb_engine"
 
 [tool.poetry.urls]
@@ -20,26 +20,26 @@
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 pre-commit = "^2.21.0"
 pdbpp = "^0.10.3"
 mypy = "^1.3"
 hypothesis = "^6.75.2"
 pandas = "^1"
-jupysql = "^0.7.4"
+jupysql = "^0.7.8"
 sqlalchemy = {version="^1.3.19", extras=['mypy']}
 pytest-cov = {extras = ["coverage"], version = "^4.0.0"}
 snapshottest = "^0.6.0"
+pytest-remotedata = "^0.4.0"
 
 [tool.poetry.plugins."sqlalchemy.dialects"]
 duckdb = "duckdb_engine:Dialect"
 
 [tool.pytest.ini_options]
-addopts = "--hypothesis-show-statistics"
+addopts = "--hypothesis-show-statistics --strict --strict-markers"
 xfail_strict = true
-strict_markers = true
 
 [tool.mypy]
 ignore_missing_imports = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 check_untyped_defs = true
```

### Comparing `duckdb_engine-0.7.3/PKG-INFO` & `duckdb_engine-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckdb-engine
-Version: 0.7.3
+Version: 0.8.0
 Summary: SQLAlchemy driver for duckdb
 Home-page: https://github.com/Mause/duckdb_engine
 License: MIT
 Author: Elliana
 Author-email: me@mause.me
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
```

