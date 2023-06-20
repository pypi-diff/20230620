# Comparing `tmp/databento_dbn-0.6.1-cp39-none-win_amd64.whl.zip` & `tmp/databento_dbn-0.7.0-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 544968 bytes, number of entries: 8
--rw-r--r--  4.6 unx     2990 b- defN 23-Jun-02 19:02 databento_dbn-0.6.1.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 23-Jun-02 19:02 databento_dbn-0.6.1.dist-info/WHEEL
--rw-r--r--  4.6 unx     9868 b- defN 23-Jun-02 19:02 databento_dbn-0.6.1.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx      135 b- defN 23-Jun-02 19:02 databento_dbn/__init__.py
--rw-r--r--  4.6 unx    37132 b- defN 23-Jun-02 19:02 databento_dbn/__init__.pyi
--rw-r--r--  4.6 unx        0 b- defN 23-Jun-02 19:02 databento_dbn/py.typed
--rwxr-xr-x  4.6 unx  1553920 b- defN 23-Jun-02 19:02 databento_dbn/databento_dbn.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      679 b- defN 23-Jun-02 19:02 databento_dbn-0.6.1.dist-info/RECORD
-8 files, 1604818 bytes uncompressed, 543780 bytes compressed:  66.1%
+Zip file size: 559738 bytes, number of entries: 8
+-rw-r--r--  4.6 unx     3052 b- defN 23-Jun-20 17:37 databento_dbn-0.7.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 23-Jun-20 17:37 databento_dbn-0.7.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     9868 b- defN 23-Jun-20 17:37 databento_dbn-0.7.0.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx      135 b- defN 23-Jun-20 17:37 databento_dbn/__init__.py
+-rw-r--r--  4.6 unx    37101 b- defN 23-Jun-20 17:37 databento_dbn/__init__.pyi
+-rw-r--r--  4.6 unx        0 b- defN 23-Jun-20 17:37 databento_dbn/py.typed
+-rwxr-xr-x  4.6 unx  1616384 b- defN 23-Jun-20 17:37 databento_dbn/databento_dbn.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      679 b- defN 23-Jun-20 17:37 databento_dbn-0.7.0.dist-info/RECORD
+8 files, 1667313 bytes uncompressed, 558550 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: databento_dbn-0.6.1.dist-info/METADATA
+Filename: databento_dbn-0.7.0.dist-info/METADATA
 Comment: 
 
-Filename: databento_dbn-0.6.1.dist-info/WHEEL
+Filename: databento_dbn-0.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: databento_dbn-0.6.1.dist-info/license_files/LICENSE
+Filename: databento_dbn-0.7.0.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: databento_dbn/__init__.py
 Comment: 
 
 Filename: databento_dbn/__init__.pyi
 Comment: 
 
 Filename: databento_dbn/py.typed
 Comment: 
 
 Filename: databento_dbn/databento_dbn.cp39-win_amd64.pyd
 Comment: 
 
-Filename: databento_dbn-0.6.1.dist-info/RECORD
+Filename: databento_dbn-0.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## databento_dbn/__init__.pyi

```diff
@@ -1,20 +1,19 @@
-"""Type stubs for databento_dbn."""
+# ruff: noqa: PYI021 PYI053
+from __future__ import annotations
+
+from collections.abc import Sequence
 from typing import (
     Any,
     BinaryIO,
-    Dict,
-    List,
-    Optional,
-    Sequence,
     SupportsBytes,
-    Tuple,
     Union,
 )
 
+
 _DBNRecord = Union[
     Metadata,
     MBOMsg,
     MBP1Msg,
     MBP10Msg,
     OHLCVMsg,
     TradeMsg,
@@ -28,15 +27,15 @@
 
 class Metadata(SupportsBytes):
     """
     Information about the data contained in a DBN file or stream. DBN requires
     the Metadata to be included at the start of the encoded data.
 
     See Also
-    ---------
+    --------
     decode_metadata
     encode_metadata
 
     """
 
     def __bytes__(self) -> bytes: ...
     def __eq__(self, other) -> bool: ...
@@ -58,22 +57,22 @@
 
         Returns
         -------
         str
 
         """
     @property
-    def schema(self) -> Optional[str]:
+    def schema(self) -> str | None:
         """
         The data record schema. Specifies which record type is stored in the
         Zstd-compressed DBN file.
 
         Returns
         -------
-        Optional[str]
+        str | None
 
         """
     @property
     def start(self) -> int:
         """
         The UNIX nanosecond timestamp of the query start, or the first record
         if the file was split.
@@ -101,21 +100,21 @@
 
         Returns
         -------
         int
 
         """
     @property
-    def stype_in(self) -> Optional[str]:
+    def stype_in(self) -> str | None:
         """
         The input symbology type to map from.
 
         Returns
         -------
-        Optional[str]
+        str | None
 
         """
     @property
     def stype_out(self) -> str:
         """
         The output symbology type to map to.
 
@@ -132,58 +131,58 @@
 
         Returns
         -------
         bool
 
         """
     @property
-    def symbols(self) -> List[str]:
+    def symbols(self) -> list[str]:
         """
         The original query input symbols from the request.
 
         Returns
         -------
-        List[str]
+        list[str]
 
         """
     @property
-    def partial(self) -> List[str]:
+    def partial(self) -> list[str]:
         """
         Symbols that did not resolve for at least one day in the query time
         range.
 
         Returns
         -------
-        List[str]
+        list[str]
 
         """
     @property
-    def not_found(self) -> List[str]:
+    def not_found(self) -> list[str]:
         """
         Symbols that did not resolve for any day in the query time range.
 
         Returns
         -------
-        List[str]
+        list[str]
 
         """
     @property
-    def mappings(self) -> Dict[str, List[Dict[str, Any]]]:
+    def mappings(self) -> dict[str, list[dict[str, Any]]]:
         """
         Symbol mappings containing a native symbol and its mapping intervals.
 
         Returns
         -------
-        Dict[str, List[Dict[str, Any]]]:
+        dict[str, list[dict[str, Any]]]:
 
         """
     @classmethod
-    def decode(cls, data: bytes) -> "Metadata":
+    def decode(cls, data: bytes) -> Metadata:
         """
-        Decodes the given Python `bytes` to `Metadata`. Returns a `Metadata`
+        Decode the given Python `bytes` to `Metadata`. Returns a `Metadata`
         object with all the DBN metadata attributes.
 
         Parameters
         ----------
         data : bytes
             The bytes to decode from.
 
@@ -195,15 +194,15 @@
         ------
         ValueError
             When a Metadata instance cannot be parsed from `data`.
 
         """
     def encode(self) -> bytes:
         """
-        Encodes the Metadata to bytes.
+        Encode the Metadata to bytes.
 
         Returns
         -------
         bytes
 
         Raises
         ------
@@ -349,22 +348,22 @@
 
         Returns
         -------
         int
 
         """
     @property
-    def ts_out(self) -> Optional[int]:
+    def ts_out(self) -> int | None:
         """
         The live gateway send timestamp expressed as number of nanoseconds since
         the UNIX epoch.
 
         Returns
         -------
-        Optional[int]
+        int | None
 
         """
 
 class _MBOBase:
     """Base for market-by-order messages."""
 
     @property
@@ -643,39 +642,39 @@
 
     """
 
 class MBP1Msg(Record, _MBPBase):
     """Market by price implementation with a known book depth of 1."""
 
     @property
-    def levels(self) -> List[BidAskPair]:
+    def levels(self) -> list[BidAskPair]:
         """
         The top of the order book.
 
         Returns
         -------
-        List[BidAskPair]
+        list[BidAskPair]
 
         Notes
         -----
         MBP1Msg contains 1 level of BidAskPair.
 
         """
 
 class MBP10Msg(Record, _MBPBase):
     """Market by price implementation with a known book depth of 10."""
 
     @property
-    def levels(self) -> List[BidAskPair]:
+    def levels(self) -> list[BidAskPair]:
         """
         The top 10 levels.
 
         Returns
         -------
-        List[BidAskPair]
+        list[BidAskPair]
 
         Notes
         -----
         MBP10Msg contains 10 levels of BidAskPairs.
 
         """
 
@@ -1683,15 +1682,16 @@
         -------
         str
 
         """
 
 class SymbolMappingMsg(Record):
     """A symbol mapping message which maps a symbol of one `SType` to
-    another."""
+    another.
+    """
 
     @property
     def stype_in_symbol(self) -> str:
         """
         The input symbol.
 
         Returns
@@ -1772,21 +1772,21 @@
         Returns
         -------
         bytes
 
         """
     def decode(
         self,
-    ) -> List[_DBNRecord]:
+    ) -> list[_DBNRecord]:
         """
         Decode the buffered data into DBN records.
 
         Returns
         -------
-        List[DBNRecord]
+        list[DBNRecord]
 
         Raises
         ------
         ValueError
             When the decoding fails.
 
         See Also
@@ -1811,31 +1811,31 @@
         decode
 
         """
 
 def update_encoded_metadata(
     file: BinaryIO,
     start: int,
-    end: Optional[int] = None,
-    limit: Optional[int] = None,
+    end: int | None = None,
+    limit: int | None = None,
 ) -> None:
     """
-    Updates existing fields that have already been written to the given file.
+    Update existing fields that have already been written to the given file.
 
     Parameters
     ----------
     file : BinaryIO
         The file handle to update.
     start : int
         The UNIX nanosecond timestamp of the query start, or the
         first record if the file was split.
-    end : Optional[int]
+    end : int | None
         The UNIX nanosecond timestamp of the query end, or the
         last record if the file was split.
-    limit : Optional[int]
+    limit : int | None
         The optional maximum number of records for the query.
 
     Raises
     ------
     ValueError
         When the file update fails.
 
@@ -1846,18 +1846,18 @@
     compression: str,
     dataset: str,
     schema: str,
     start: int,
     stype_in: str,
     stype_out: str,
     records: Sequence[Record],
-    end: Optional[int] = None,
+    end: int | None = None,
 ) -> None:
     """
-    Encodes the given data in the DBN encoding and writes it to `file`.
+    Encode the given data in the DBN encoding and writes it to `file`.
 
     Parameters
     ----------
     file : BinaryIO
         The file handle to update.
     compression : str
         The DBN compression format.
@@ -1870,15 +1870,15 @@
         first record if the file was split.
     stype_in : str
         The input symbology type to map from.
     stype_out : str
         The output symbology type to map to.
     records : Sequence[object]
         A sequence of DBN record objects.
-    end : Optional[int]
+    end : int | None
         The UNIX nanosecond timestamp of the query end, or the
         last record if the file was split.
 
     Raises
     ------
     ValueError
         When any of the enum arguments cannot be converted to their Rust equivalents.
```

## Comparing `databento_dbn-0.6.1.dist-info/METADATA` & `databento_dbn-0.7.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: databento-dbn
-Version: 0.6.1
+Version: 0.7.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Python bindings for encoding and decoding Databento Binary Encoding (DBN)
 Author: Databento <support@databento.com>
 Author-email: Databento <support@databento.com>
 License: Apache-2.0
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/databento/dbn
 
 # databento-dbn
 
 [![build](https://github.com/databento/dbn/actions/workflows/build.yaml/badge.svg)](https://github.com/databento/dbn/actions/workflows/build.yaml)
+![python](https://img.shields.io/badge/python-3.8+-blue.svg)
 ![license](https://img.shields.io/github/license/databento/dbn?color=blue)
 [![pypi-version](https://img.shields.io/pypi/v/databento_dbn)](https://pypi.org/project/databento-dbn)
 
 Python bindings for the `dbn` Rust library.
 Used by the [Databento Python client library](https://github.com/databento/databento-python).
 
 Using this library is for advanced users and is not fully documented or supported.
```

## Comparing `databento_dbn-0.6.1.dist-info/license_files/LICENSE` & `databento_dbn-0.7.0.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

