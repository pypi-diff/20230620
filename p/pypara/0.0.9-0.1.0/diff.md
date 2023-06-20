# Comparing `tmp/pypara-0.0.9.tar.gz` & `tmp/pypara-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypara-0.0.9.tar", last modified: Tue Jul 17 05:53:52 2018, max compression
+gzip compressed data, was "pypara-0.1.0.tar", last modified: Tue Jun 20 05:30:12 2023, max compression
```

## Comparing `pypara-0.0.9.tar` & `pypara-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,36 @@
-drwxr-xr-x   0 vst       (1000) vst       (1000)        0 2018-07-17 05:53:52.000000 pypara-0.0.9/
-drwxr-xr-x   0 vst       (1000) vst       (1000)        0 2018-07-17 05:53:52.000000 pypara-0.0.9/pypara/
--rw-r--r--   0 vst       (1000) vst       (1000)    23927 2018-07-17 03:31:48.000000 pypara-0.0.9/pypara/currencies.py
--rw-r--r--   0 vst       (1000) vst       (1000)    24168 2018-07-17 03:31:48.000000 pypara-0.0.9/pypara/dcc.py
--rw-r--r--   0 vst       (1000) vst       (1000)       61 2018-07-17 03:32:28.000000 pypara-0.0.9/pypara/__init__.py
--rw-r--r--   0 vst       (1000) vst       (1000)    37963 2018-07-17 03:31:48.000000 pypara-0.0.9/pypara/monetary.py
--rw-r--r--   0 vst       (1000) vst       (1000)     5823 2018-07-17 03:31:48.000000 pypara-0.0.9/pypara/exchange.py
--rw-r--r--   0 vst       (1000) vst       (1000)     1241 2018-07-17 03:31:48.000000 pypara-0.0.9/pypara/generic.py
--rw-r--r--   0 vst       (1000) vst       (1000)       39 2018-04-27 06:33:32.000000 pypara-0.0.9/MANIFEST.in
--rw-r--r--   0 vst       (1000) vst       (1000)      115 2018-07-17 05:53:52.000000 pypara-0.0.9/setup.cfg
--rw-r--r--   0 vst       (1000) vst       (1000)      965 2018-04-27 06:33:32.000000 pypara-0.0.9/README.rst
-drwxr-xr-x   0 vst       (1000) vst       (1000)        0 2018-07-17 05:53:52.000000 pypara-0.0.9/pypara.egg-info/
--rw-r--r--   0 vst       (1000) vst       (1000)       37 2018-07-17 05:53:52.000000 pypara-0.0.9/pypara.egg-info/requires.txt
--rw-r--r--   0 vst       (1000) vst       (1000)        1 2018-04-30 04:48:26.000000 pypara-0.0.9/pypara.egg-info/not-zip-safe
--rw-r--r--   0 vst       (1000) vst       (1000)      341 2018-07-17 05:53:52.000000 pypara-0.0.9/pypara.egg-info/SOURCES.txt
--rw-r--r--   0 vst       (1000) vst       (1000)        1 2018-07-17 05:53:52.000000 pypara-0.0.9/pypara.egg-info/dependency_links.txt
--rw-r--r--   0 vst       (1000) vst       (1000)     1812 2018-07-17 05:53:52.000000 pypara-0.0.9/pypara.egg-info/PKG-INFO
--rw-r--r--   0 vst       (1000) vst       (1000)        7 2018-07-17 05:53:52.000000 pypara-0.0.9/pypara.egg-info/top_level.txt
--rw-r--r--   0 vst       (1000) vst       (1000)     1469 2018-04-27 06:33:32.000000 pypara-0.0.9/LICENSE.txt
--rw-r--r--   0 vst       (1000) vst       (1000)     1842 2018-07-17 03:33:38.000000 pypara-0.0.9/setup.py
--rw-r--r--   0 vst       (1000) vst       (1000)     1812 2018-07-17 05:53:52.000000 pypara-0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:30:12.598204 pypara-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-20 05:29:11.000000 pypara-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-20 05:30:12.598204 pypara-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-20 05:29:11.000000 pypara-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:30:12.598204 pypara-0.1.0/pypara/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-20 05:29:11.000000 pypara-0.1.0/pypara/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:30:12.598204 pypara-0.1.0/pypara/accounting/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-20 05:29:11.000000 pypara-0.1.0/pypara/accounting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10880 2023-06-20 05:29:11.000000 pypara-0.1.0/pypara/accounting/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-20 05:29:11.000000 pypara-0.1.0/pypara/accounting/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-06-20 05:29:11.000000 pypara-0.1.0/pypara/accounting/journaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-20 05:29:11.000000 pypara-0.1.0/pypara/accounting/ledger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:30:12.598204 pypara-0.1.0/pypara/commons/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 05:29:11.000000 pypara-0.1.0/pypara/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-20 05:29:11.000000 pypara-0.1.0/pypara/commons/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-20 05:29:11.000000 pypara-0.1.0/pypara/commons/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-20 05:29:11.000000 pypara-0.1.0/pypara/commons/guid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-06-20 05:29:11.000000 pypara-0.1.0/pypara/commons/numbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30750 2023-06-20 05:29:11.000000 pypara-0.1.0/pypara/commons/zeitgeist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25197 2023-06-20 05:29:11.000000 pypara-0.1.0/pypara/currencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32609 2023-06-20 05:29:11.000000 pypara-0.1.0/pypara/dcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-20 05:29:11.000000 pypara-0.1.0/pypara/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58668 2023-06-20 05:29:11.000000 pypara-0.1.0/pypara/monetary.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 05:29:11.000000 pypara-0.1.0/pypara/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:30:12.598204 pypara-0.1.0/pypara.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-20 05:30:12.000000 pypara-0.1.0/pypara.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-20 05:30:12.000000 pypara-0.1.0/pypara.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 05:30:12.000000 pypara-0.1.0/pypara.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-20 05:30:12.000000 pypara-0.1.0/pypara.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 05:30:12.000000 pypara-0.1.0/pypara.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-06-20 05:29:11.000000 pypara-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 05:30:12.598204 pypara-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:30:12.598204 pypara-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-20 05:29:11.000000 pypara-0.1.0/tests/test_currencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20343 2023-06-20 05:29:11.000000 pypara-0.1.0/tests/test_monetary_money.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-06-20 05:29:11.000000 pypara-0.1.0/tests/test_monetary_price.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pypara-0.0.9/pypara/currencies.py` & `pypara-0.1.0/pypara/currencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,31 @@
+"""
+This module provides currency definitions and related functionality.
+"""
+
+__all__ = ["Currencies", "Currency", "CurrencyLookupError", "CurrencyRegistry", "CurrencyType"]
+
 from collections import OrderedDict
+from dataclasses import dataclass
 from decimal import Decimal
 from enum import Enum
-from typing import Dict, List, Tuple, Optional, Type, Any, Callable, NamedTuple
+from typing import Any, Callable, Dict, List, Optional, Tuple, Type
 
-from .generic import MaxPrecisionQuantizer, ProgrammingError, make_quantizer
+from .commons.errors import ProgrammingError
+from .commons.numbers import ZERO, MaxPrecisionQuantizer, make_quantizer
 
 
 class CurrencyLookupError(LookupError):
     """
     Provides a currency lookup error.
+
+    >>> raise CurrencyLookupError("XYZ")
+    Traceback (most recent call last):
+    ...
+    pypara.currencies.CurrencyLookupError: Currency identified by code 'XYZ' does not exist
     """
 
     def __init__(self, code: str) -> None:
         """
         Initializes a currency lookup error.
         """
         ## Keep the code:
@@ -33,23 +46,26 @@
     #: Defines precious metals currency type.
     METAL = "Precious Metal"
 
     #: Defines crypto currency type.
     CRYPTO = "Crypto Currency"
 
     #: Defines alternative currency type.
-    ALTERNATIVE = "Alernative"
+    ALTERNATIVE = "Alternative"
 
 
-class Currency(NamedTuple):
+@dataclass(frozen=True, order=True)
+class Currency:
     """
-    Defines currency value object model which is extending ISO 4217 to embrace other currency types.
+    Defines currency value object model which is extending ISO 4217 to embrace
+    other currency types.
 
-    Note that you should not call :class:`Currency` constructor directly, but instead use the :method:`Currency.build`.
-    :method:`Currency.build` is responsible of performing some checks before creating the currency.
+    Note that you should not call :class:`Currency` constructor directly, but
+    instead use the :func:`Currency.of`. :func:`Currency.of` is responsible of
+    performing some checks before creating the currency.
 
     Try with USD:
 
     >>> USD = Currency.of("USD", "US Dollars", 2, CurrencyType.MONEY)
     >>> USD.quantize(Decimal("1.005"))
     Decimal('1.00')
     >>> USD.quantize(Decimal("1.015"))
@@ -104,37 +120,36 @@
     #: Defines the pre-computed, cached hash.
     hashcache: int
 
     def __eq__(self, other: Any) -> bool:
         """
         Checks if the `self` and `other` are same currencies.
         """
-        ## TODO: Can we optimise this without any changes in the semantics?
-        return other.__class__ == Currency and self[5] == other[5]  # type: ignore
+        return isinstance(other, Currency) and self.hashcache == other.hashcache
 
     def __hash__(self) -> int:
         """
         Returns the pre-computed and cached hash.
         """
-        return self[5]
+        return self.hashcache
 
     def quantize(self, qty: Decimal) -> Decimal:
         """
         Quantizes the decimal ``qty`` wrt to ccy's minor units fraction. Note that
         the [ROUND HALF TO EVEN](https://en.wikipedia.org/wiki/Rounding) method
         is used for rounding purposes.
 
         **Note** that the HALF-TO-EVEN method is inherited from the default decimal context instead of
         explicitly passing it. Therefore, if call-site application is making changes to the default
         context, the rounding method may not be HALF-TO-EVEN anymore.
         """
-        return qty.quantize(self[4])
+        return qty.quantize(self.quantizer)
 
     @classmethod
-    def of(cls, code: str, name: str, decimals: int, type: CurrencyType) -> "Currency":
+    def of(cls, code: str, name: str, decimals: int, ctype: CurrencyType) -> "Currency":
         """
         Attempts to create a currency instance and returns it.
         """
         ## Check the code:
         ProgrammingError.passert(isinstance(code, str), "Currency code must be a string")
         ProgrammingError.passert(code.isalpha(), "Currency code must contain only alphabetic characters")
         ProgrammingError.passert(code.isupper(), "Currency code must be all uppercase")
@@ -145,29 +160,29 @@
         ProgrammingError.passert(not (name.startswith(" ") or name.endswith(" ")), "Trim the currency name")
 
         ## Check the decimals:
         ProgrammingError.passert(isinstance(decimals, int), "Number of decimals must be an integer")
         ProgrammingError.passert(decimals >= -1, "Number of decimals can not be less than -1")
 
         ## Check the type:
-        ProgrammingError.passert(isinstance(type, CurrencyType), "Currency Type must be of type `CurrencyType`")
+        ProgrammingError.passert(isinstance(ctype, CurrencyType), "Currency Type must be of type `CurrencyType`")
 
         ## Define the quantizer:
         if decimals > 0:
             quantizer = make_quantizer(decimals)
         elif decimals < 0:
             quantizer = MaxPrecisionQuantizer
         else:
-            quantizer = Decimal("0")
+            quantizer = ZERO
 
         ## By now, we should have all required instance attributes. However, we want to compute and cache the hash.
-        hashcode = hash((code, name, decimals, type, quantizer))
+        hashcode = hash((code, name, decimals, ctype, quantizer))
 
         ## Done, create the currency object and return:
-        return Currency(code, name, decimals, type, quantizer, hashcode)
+        return Currency(code, name, decimals, ctype, quantizer, hashcode)
 
 
 class CurrencyRegistry:
     """
     Defines a currency registry model.
 
     >>> "USD" in Currencies
@@ -191,23 +206,23 @@
     True
     >>> assert len(Currencies) == len(Currencies.all)
     >>> assert Currencies.codes == [currency.code for currency in Currencies.all]
     >>> assert Currencies.codenames == [(currency.code, currency.name) for currency in Currencies.all]
     """
 
     #: Defines the singleton instance.
-    __instance = None  # type: CurrencyRegistry
+    __instance: "CurrencyRegistry" = None  # type: ignore
 
     def __new__(cls) -> "CurrencyRegistry":
         """
         Creates the singleton instance, or returns the existing one.
         """
         ## Do we have the singleton instance?
         if CurrencyRegistry.__instance is None:
-            ## Nope, not yet. Creat one:
+            ## Nope, not yet. Create one:
             CurrencyRegistry.__instance = object.__new__(cls)
 
         ## Return the singleton instance.
         return CurrencyRegistry.__instance
 
     def __init__(self) -> None:
         """
@@ -242,28 +257,34 @@
         """
         Exits the registry population context and performs some finalization tasks.
         """
         ## Re-sort the registry:
         self.__registry = OrderedDict([(c.code, c) for c in sorted(self.__registry.values(), key=lambda x: x.code)])
 
         ## Re-sort currencies buffer:
-        self.__currencies = [c for c in self.__registry.values()]
+        self.__currencies = list(self.__registry.values())
 
         ## Re-sort the currency codes buffer:
         self.__codes = [c.code for c in self.__currencies]
 
         ## Re-sort the choices buffer
         self.__codenames = [(c.code, c.name) for c in self.__currencies]
 
         ## Close the context:
         self.__ctx_open = False
 
     def __register(self, currency: Currency) -> None:
         """
         Attempts to add the currency to the registry.
+
+        >>> with Currencies as register:
+        ...    register(Currency.of("AED", "UAE Dirham", 2, CurrencyType.MONEY))
+        Traceback (most recent call last):
+        ...
+        ValueError: Currency AED is already registered.
         """
         ## Check of the registry population context is open:
         if not self.__ctx_open:
             ## Nope, raise error:
             raise ProgrammingError("Can not create currencies outside registry context.")
 
         ## Check if the currency is already added:
@@ -284,27 +305,34 @@
         Checks if a given currency code is available.
         """
         return code in self.__registry
 
     def __getitem__(self, code: str) -> Currency:
         """
         Returns the currency identified by the code or raises lookup error.
+
+        >>> Currencies["USD"].code
+        'USD'
+        >>> Currencies["NON-EXISTING"].code
+        Traceback (most recent call last):
+        ...
+        pypara.currencies.CurrencyLookupError: Currency identified by code 'NON-EXISTING' does not exist
         """
         try:
             return self.__registry[code]
         except KeyError:
             raise CurrencyLookupError(code)
 
     def has(self, code: str) -> bool:
         """
         Indicates if the code is a valid currency code.
         """
         return code in self.__registry
 
-    def get(self, code: str, default: Optional[Currency]=None) -> Optional[Currency]:
+    def get(self, code: str, default: Optional[Currency] = None) -> Optional[Currency]:
         """
         Returns the currency for the given code.
 
         Note that if the code is not a valid currency code, a currency lookup error is raised.
         """
         return self.__registry.get(code, default)
 
@@ -341,15 +369,15 @@
     register(Currency.of("ALL", "Lek", 2, CurrencyType.MONEY))
     register(Currency.of("AMD", "Armenian Dram", 2, CurrencyType.MONEY))
     register(Currency.of("ANG", "Netherlands Antillean Guilder", 2, CurrencyType.MONEY))
     register(Currency.of("AOA", "Kwanza", 2, CurrencyType.MONEY))
     register(Currency.of("ARS", "Argentine Peso", 2, CurrencyType.MONEY))
     register(Currency.of("AUD", "Australian Dollar", 2, CurrencyType.MONEY))
     register(Currency.of("AWG", "Aruban Florin", 2, CurrencyType.MONEY))
-    register(Currency.of("AZN", "Azerbaijanian Manat", 2, CurrencyType.MONEY))
+    register(Currency.of("AZN", "Azerbaijani Manat", 2, CurrencyType.MONEY))
     register(Currency.of("BAM", "Convertible Mark", 2, CurrencyType.MONEY))
     register(Currency.of("BBD", "Barbados Dollar", 2, CurrencyType.MONEY))
     register(Currency.of("BCH", "Bitcoin Cash", -1, CurrencyType.CRYPTO))
     register(Currency.of("BDT", "Taka", 2, CurrencyType.MONEY))
     register(Currency.of("BGN", "Bulgarian Lev", 2, CurrencyType.MONEY))
     register(Currency.of("BHD", "Bahraini Dinar", 3, CurrencyType.MONEY))
     register(Currency.of("BIF", "Burundi Franc", 0, CurrencyType.MONEY))
@@ -358,15 +386,15 @@
     register(Currency.of("BOB", "Boliviano", 2, CurrencyType.MONEY))
     register(Currency.of("BOV", "Mvdol", 2, CurrencyType.MONEY))
     register(Currency.of("BRL", "Brazilian Real", 2, CurrencyType.MONEY))
     register(Currency.of("BSD", "Bahamian Dollar", 2, CurrencyType.MONEY))
     register(Currency.of("BTC", "Bitcoin", -1, CurrencyType.CRYPTO))
     register(Currency.of("BTN", "Ngultrum", 2, CurrencyType.MONEY))
     register(Currency.of("BWP", "Pula", 2, CurrencyType.MONEY))
-    register(Currency.of("BYR", "Belarussian Ruble", 0, CurrencyType.MONEY))
+    register(Currency.of("BYR", "Belarusian Ruble", 0, CurrencyType.MONEY))
     register(Currency.of("BZD", "Belize Dollar", 2, CurrencyType.MONEY))
     register(Currency.of("CAD", "Canadian Dollar", 2, CurrencyType.MONEY))
     register(Currency.of("CDF", "Congolese Franc", 2, CurrencyType.MONEY))
     register(Currency.of("CHE", "WIR Euro", 2, CurrencyType.MONEY))
     register(Currency.of("CHF", "Swiss Franc", 2, CurrencyType.MONEY))
     register(Currency.of("CHW", "WIR Franc", 2, CurrencyType.MONEY))
     register(Currency.of("CLF", "Unidad de Fomento", 4, CurrencyType.MONEY))
@@ -374,19 +402,20 @@
     register(Currency.of("CNH", "Yuan Renminbi (Off-shore)", 2, CurrencyType.MONEY))
     register(Currency.of("CNY", "Yuan Renminbi", 2, CurrencyType.MONEY))
     register(Currency.of("COP", "Colombian Peso", 2, CurrencyType.MONEY))
     register(Currency.of("COU", "Unidad de Valor Real", 2, CurrencyType.MONEY))
     register(Currency.of("CRC", "Costa Rican Colon", 2, CurrencyType.MONEY))
     register(Currency.of("CUC", "Peso Convertible", 2, CurrencyType.MONEY))
     register(Currency.of("CUP", "Cuban Peso", 2, CurrencyType.MONEY))
-    register(Currency.of("CVE", "Cabo Verde Escudo", 2, CurrencyType.MONEY))
+    register(Currency.of("CVE", "Cape Verdean Escudo", 2, CurrencyType.MONEY))
     register(Currency.of("CZK", "Czech Koruna", 2, CurrencyType.MONEY))
     register(Currency.of("DASH", "Dash", -1, CurrencyType.CRYPTO))
     register(Currency.of("DJF", "Djibouti Franc", 0, CurrencyType.MONEY))
     register(Currency.of("DKK", "Danish Krone", 2, CurrencyType.MONEY))
+    register(Currency.of("DOGE", "Dogecoin", -1, CurrencyType.CRYPTO))
     register(Currency.of("DOP", "Dominican Peso", 2, CurrencyType.MONEY))
     register(Currency.of("DZD", "Algerian Dinar", 2, CurrencyType.MONEY))
     register(Currency.of("EGP", "Egyptian Pound", 2, CurrencyType.MONEY))
     register(Currency.of("EOS", "EOSIO", -1, CurrencyType.CRYPTO))
     register(Currency.of("ERN", "Nakfa", 2, CurrencyType.MONEY))
     register(Currency.of("ETB", "Ethiopian Birr", 2, CurrencyType.MONEY))
     register(Currency.of("ETC", "Ethereum Classic", -1, CurrencyType.CRYPTO))
@@ -424,14 +453,15 @@
     register(Currency.of("KPW", "North Korean Won", 2, CurrencyType.MONEY))
     register(Currency.of("KRW", "Won", 0, CurrencyType.MONEY))
     register(Currency.of("KWD", "Kuwaiti Dinar", 3, CurrencyType.MONEY))
     register(Currency.of("KYD", "Cayman Islands Dollar", 2, CurrencyType.MONEY))
     register(Currency.of("KZT", "Tenge", 2, CurrencyType.MONEY))
     register(Currency.of("LAK", "Kip", 2, CurrencyType.MONEY))
     register(Currency.of("LBP", "Lebanese Pound", 2, CurrencyType.MONEY))
+    register(Currency.of("LINK", "Chainlink", -1, CurrencyType.CRYPTO))
     register(Currency.of("LKR", "Sri Lanka Rupee", 2, CurrencyType.MONEY))
     register(Currency.of("LRD", "Liberian Dollar", 2, CurrencyType.MONEY))
     register(Currency.of("LSL", "Loti", 2, CurrencyType.MONEY))
     register(Currency.of("LTC", "Litecoin", -1, CurrencyType.CRYPTO))
     register(Currency.of("LYD", "Libyan Dinar", 3, CurrencyType.MONEY))
     register(Currency.of("MAD", "Moroccan Dirham", 2, CurrencyType.MONEY))
     register(Currency.of("MDL", "Moldovan Leu", 2, CurrencyType.MONEY))
@@ -494,25 +524,28 @@
     register(Currency.of("TWD", "New Taiwan Dollar", 2, CurrencyType.MONEY))
     register(Currency.of("TZS", "Tanzanian Shilling", 2, CurrencyType.MONEY))
     register(Currency.of("UAH", "Hryvnia", 2, CurrencyType.MONEY))
     register(Currency.of("UGX", "Uganda Shilling", 0, CurrencyType.MONEY))
     register(Currency.of("USD", "US Dollar", 2, CurrencyType.MONEY))
     register(Currency.of("USN", "US Dollar (Next day)", 2, CurrencyType.MONEY))
     register(Currency.of("UYI", "Uruguay Peso en Unidades Indexadas", 0, CurrencyType.MONEY))
-    register(Currency.of("UYU", "Peso Uruguayo", 2, CurrencyType.MONEY))
+    register(Currency.of("UYU", "Uruguayan Peso", 2, CurrencyType.MONEY))
     register(Currency.of("UZS", "Uzbekistan Sum", 2, CurrencyType.MONEY))
     register(Currency.of("VEF", "Bolivar", 2, CurrencyType.MONEY))
     register(Currency.of("VND", "Dong", 0, CurrencyType.MONEY))
     register(Currency.of("VUV", "Vatu", 0, CurrencyType.MONEY))
     register(Currency.of("WST", "Tala", 2, CurrencyType.MONEY))
+    register(Currency.of("XAF", "Central African CFA Franc BCEAO", 2, CurrencyType.MONEY))
     register(Currency.of("XAG", "Silver", -1, CurrencyType.METAL))
     register(Currency.of("XAU", "Gold", -1, CurrencyType.METAL))
     register(Currency.of("XCD", "East Caribbean Dollar", 2, CurrencyType.MONEY))
+    register(Currency.of("XLC", "Ethereum Lite Cash", -1, CurrencyType.CRYPTO))
     register(Currency.of("XLM", "Stellar", -1, CurrencyType.CRYPTO))
     register(Currency.of("XMR", "Monero", -1, CurrencyType.CRYPTO))
+    register(Currency.of("XOF", "West African CFA Franc BCEAO", 2, CurrencyType.MONEY))
     register(Currency.of("XPD", "Palladium", -1, CurrencyType.METAL))
     register(Currency.of("XPT", "Platinum", -1, CurrencyType.METAL))
     register(Currency.of("XRP", "Ripple", -1, CurrencyType.CRYPTO))
     register(Currency.of("XSU", "Sucre", -1, CurrencyType.MONEY))
     register(Currency.of("XUA", "ADB Unit of Account", -1, CurrencyType.MONEY))
     register(Currency.of("YER", "Yemeni Rial", 2, CurrencyType.MONEY))
     register(Currency.of("ZAR", "Rand", 2, CurrencyType.MONEY))
```

### Comparing `pypara-0.0.9/pypara/dcc.py` & `pypara-0.1.0/pypara/dcc.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,28 @@
+"""
+This module provides day-count convention definitions and functionality.
+"""
+
+__all__ = ["DCC", "DCCRegistry"]
+
 import calendar
 import datetime
 from decimal import Decimal
-from typing import Dict, Callable, Set, Optional, List, Iterable, NamedTuple
+from itertools import chain
+from typing import Callable, Dict, Iterable, List, NamedTuple, Optional, Set, Union
 
-from pypara.currencies import Currency, Currencies
-from pypara.generic import Date
-from pypara.monetary import Money
+from dateutil.relativedelta import relativedelta
+
+from .commons.numbers import ONE, ZERO
+from .commons.zeitgeist import Date
+from .currencies import Currencies, Currency
+from .monetary import Money
 
 #: Defines a type alias for day count fraction calculation functions.
-DCFC = Callable[[Date, Date, Date], Decimal]
+DCFC = Callable[[Date, Date, Date, Optional[Decimal]], Decimal]
 
 
 def _as_ccys(codes: Set[str]) -> Set[Currency]:
     """
     Converts a set of currency codes to a set of currencies.
     """
     return {Currencies[c] for c in codes}
@@ -22,16 +32,16 @@
     """
     Returns a generator of dates falling into range within the given period (``end`` is exclusive).
 
     :param start: The start date of the period.
     :param end: The end date of the period.
     :return: A generator of dates.
     """
-    for i in range((end - start).days):
-        yield start + datetime.timedelta(days=i)
+    for d in range((end - start).days):
+        yield start + datetime.timedelta(days=d)
 
 
 def _get_actual_day_count(start: Date, end: Date) -> int:
     """
     Counts the actual number of days in the given period.
 
     :param start: The start date of the period.
@@ -70,51 +80,220 @@
 def _is_last_day_of_month(date: Date) -> bool:
     """
     Indicates if the date is the last day of the month.
     """
     return date.day == calendar.monthrange(date.year, date.month)[1]
 
 
+def _last_payment_date(start: Date, asof: Date, frequency: Union[int, Decimal], eom: Optional[int] = None) -> Date:
+    """
+    Returns the last coupon payment date.
+
+    >>> _last_payment_date(datetime.date(2014,  1,  1), datetime.date(2015, 12, 31), 1)
+    datetime.date(2015, 1, 1)
+
+    >>> _last_payment_date(datetime.date(2015,  1,  1), datetime.date(2015, 12, 31), 1)
+    datetime.date(2015, 1, 1)
+
+    >>> _last_payment_date(datetime.date(2014,  1,  1), datetime.date(2015, 12, 31), 2)
+    datetime.date(2015, 7, 1)
+
+    >>> _last_payment_date(datetime.date(2014,  1,  1), datetime.date(2015,  8, 31), 2)
+    datetime.date(2015, 7, 1)
+
+    >>> _last_payment_date(datetime.date(2014,  1,  1), datetime.date(2015,  4, 30), 2)
+    datetime.date(2015, 1, 1)
+
+    >>> _last_payment_date(datetime.date(2014,  6,  1), datetime.date(2015,  4, 30), 1)
+    datetime.date(2014, 6, 1)
+
+    >>> _last_payment_date(datetime.date(2008,  7,  7), datetime.date(2015, 10,  6), 4)
+    datetime.date(2015, 7, 7)
+
+    >>> _last_payment_date(datetime.date(2014, 12,  9), datetime.date(2015, 12,  4), 1)
+    datetime.date(2014, 12, 9)
+
+    >>> _last_payment_date(datetime.date(2012, 12, 15), datetime.date(2016,  1,  6), 2)
+    datetime.date(2015, 12, 15)
+
+    >>> _last_payment_date(datetime.date(2012, 12, 15), datetime.date(2015, 12, 31), 2)
+    datetime.date(2015, 12, 15)
+    """
+    ## Make sure that we have eom:
+    eom = eom or start.day
+
+    ## Get the starting month:
+    s_month = start.month
+
+    ## Get the period:
+    period = int(12 / frequency)
+
+    ## Get the current day, month and year:
+    c_day, c_month, c_year = asof.day, asof.month, asof.year
+
+    ## Get the payment schedule:
+    schedule = sorted([i > 0 and i or 12 for i in sorted([(i + s_month) % 12 for i in range(0, 12, period)])])
+
+    ## Filter out previous:
+    future = [month for month in schedule if (month < c_month) or (month == c_month and eom <= c_day)]
+
+    ## Get the previous month and year:
+    p_year, p_month = (c_year, future[-1]) if future else (c_year - 1, schedule[-1])
+
+    ## Return the date:
+    if p_year < 1 or p_month < 1 or eom < 1:
+        return start
+
+    ## Construct and return the date safely:
+    return _construct_date(p_year, p_month, eom)
+
+
+def _next_payment_date(start: Date, frequency: Union[int, Decimal], eom: Optional[int] = None) -> Date:
+    """
+    Returns the last coupon payment date.
+
+    >>> _next_payment_date(datetime.date(2014,  1,  1), 1, None)
+    datetime.date(2015, 1, 1)
+
+    >>> _next_payment_date(datetime.date(2014,  1,  1), 1, 15)
+    datetime.date(2015, 1, 15)
+    """
+    ## Get the number of months to move forward:
+    months = int(12 / frequency)
+
+    ## Find the next date:
+    nextdate = start + relativedelta(months=months)
+
+    ## Do we have any end of month?
+    if eom:
+        try:
+            nextdate = nextdate.replace(day=eom)
+        except ValueError:
+            pass
+
+    ## Done, return:
+    return nextdate
+
+
+def _construct_date(year: int, month: int, day: int) -> Date:
+    """
+    Constructs and returns date safely.
+    """
+    if year <= 0 or month <= 0 or day <= 0:
+        raise ValueError("year, month and day must be greater than 0.")
+    try:
+        return datetime.date(year, month, day)
+    except ValueError as exc:
+        if str(exc) == "day is out of range for month":
+            return _construct_date(year, month, day - 1)
+        else:
+            raise exc
+
+
 class DCC(NamedTuple):
     """
     Defines a day count convention model.
     """
 
     #: Defines the name of the day count convention.
     name: str
 
     #: Defines a set of alternative names of the day count convention.
     altnames: Set[str]
 
     #: Defines a set of currencies which are known to use this convention by default.
     currencies: Set[Currency]
 
-    #: Defines the day count fraction calculation function.
-    calculate_fraction: DCFC
+    #: Defines the day count fraction calculation method function.
+    calculate_fraction_method: DCFC
+
+    def calculate_fraction(self, start: Date, asof: Date, end: Date, freq: Optional[Decimal] = None) -> Decimal:
+        """
+        Calculates the day count fraction based on the underlying methodology after performing some general checks.
+        """
+        ## Checks if dates are provided properly:
+        if not start <= asof <= end:
+            ## Nope, return 0:
+            return ZERO
 
-    def __call__(self, principal: Money, rate: Decimal, start: Date, asof: Date, end: Optional[Date]=None) -> Money:
+        ## Cool, we can proceed with calculation based on the methodology:
+        return self[3](start, asof, end, freq)
+
+    def calculate_daily_fraction(self, start: Date, asof: Date, end: Date, freq: Optional[Decimal] = None) -> Decimal:
         """
-        Calculates the interest for the given schedule.
+        Calculates daily fraction.
         """
-        return principal * rate * self[3](start, asof, end or asof)
+        ## Get t-1 for asof:
+        asof_minus_1 = asof - datetime.timedelta(days=1)
+
+        ## Get the yesterday's factor:
+        if asof_minus_1 < start:
+            yfact = ZERO
+        else:
+            yfact = self.calculate_fraction_method(start, asof_minus_1, end, freq)
+
+        ## Get today's factor:
+        tfact = self.calculate_fraction_method(start, asof, end, freq)
+
+        ## Get the factor and return:
+        return tfact - yfact
+
+    def interest(
+        self,
+        principal: Money,
+        rate: Decimal,
+        start: Date,
+        asof: Date,
+        end: Optional[Date] = None,
+        freq: Optional[Decimal] = None,
+    ) -> Money:
+        """
+        Calculates the accrued interest.
+        """
+        return principal * rate * self.calculate_fraction(start, asof, end or asof, freq)
+
+    def coupon(
+        self,
+        principal: Money,
+        rate: Decimal,
+        start: Date,
+        asof: Date,
+        end: Date,
+        freq: Union[int, Decimal],
+        eom: Optional[int] = None,
+    ) -> Money:
+        """
+        Calculates the accrued interest for the coupon payment.
+
+        This method is primarily used for bond coupon accruals which assumes the start date to be the first of regular
+        payment schedules.
+        """
+        ## Find the previous and next payment dates:
+        prevdate = _last_payment_date(start, asof, freq, eom)
+        nextdate = _next_payment_date(prevdate, freq, eom)
+
+        ## Calculate the interest and return:
+        return self.interest(principal, rate, prevdate, asof, nextdate, Decimal(freq))
 
 
 class DCCRegistryMachinery:
     """
     Provides the day count registry model.
 
     >>> principal = Money.of(Currencies["USD"], Decimal(1000000), datetime.date.today())
     >>> start = datetime.date(2007, 12, 28)
     >>> end = datetime.date(2008, 2, 28)
     >>> rate = Decimal(0.01)
     >>> dcc = DCCRegistry.find("Act/Act")
     >>> round(dcc.calculate_fraction(start, end, end), 14)
     Decimal('0.16942884946478')
-    >>> dcc(principal, rate, start, end).qty
+    >>> dcc.interest(principal, rate, start, end, end).qty
     Decimal('1694.29')
+    >>> dcc.interest(principal, rate, end, start, start).qty
+    Decimal('0.00')
     """
 
     def __init__(self) -> None:
         """
         Initializes the registry.
         """
         ## Define the main registry buffer:
@@ -157,63 +336,119 @@
         """
         return self._buffer_main.get(name) or self._buffer_altn.get(name)
 
     def find(self, name: str) -> Optional[DCC]:
         """
         Attempts to find the day count convention by the given name.
 
-        Note that all day count conventions are registered under stripped, uppercased names. Therefore,
+        Note that all day count conventions are registered under stripped, uppercase names. Therefore,
         the implementation will first attempt to find by given name as is. If it can not find it, it will
         strip and uppercase the name and try to find it as such as a last resort.
         """
         return self._find_strict(name) or self._find_strict(name.strip().upper())
 
+    @property
+    def registry(self) -> List[DCC]:
+        """
+        Returns the main registry values.
+        """
+        return list(self._buffer_main.values())
+
+    @property
+    def table(self) -> Dict[str, DCC]:
+        """
+        Returns a lookup table for available day count conventions.
+
+        >>> for k in sorted(DCCRegistry.table.keys()):
+        ...     print(k)
+        30/360 European
+        30/360 German
+        30/360 ISDA
+        30/360 ISMA
+        30/360 US
+        30/360 US Municipal
+        30E+/360
+        30E/360
+        30E/360 ISDA
+        30S/360 Special German
+        30U/360
+        30US/360
+        360
+        365
+        Act/360
+        Act/365A
+        Act/365F
+        Act/365L
+        Act/Act
+        Act/Act (ICMA)
+        Act/Act (ISMA)
+        Actual/360
+        Actual/365 Actual
+        Actual/365 Fixed
+        Actual/365 Leap Year
+        Actual/365 No Leap Year
+        Actual/Actual
+        Actual/Actual (ICMA)
+        Actual/Actual (ISDA)
+        Bond Basis
+        English
+        Eurobond Basis
+        French
+        ISMA-99
+        NL/365
+        NL365
+        """
+        return dict(chain(self._buffer_main.items(), self._buffer_altn.items()))
+
 
 #: Defines the default DCC registry.
 DCCRegistry = DCCRegistryMachinery()
 
 
-def dcc(name: str, altnames: Optional[Set[str]]=None, ccys: Optional[Set[Currency]]=None) -> Callable[[DCFC], DCFC]:
+def dcc(name: str, altnames: Optional[Set[str]] = None, ccys: Optional[Set[Currency]] = None) -> Callable[[DCFC], DCFC]:
     """
     Registers a day count fraction calculator under the given names and alternative names (if any).
 
     :param name: The name of the day count convention.
     :param altnames: A set of alternative names of the day count convention, if any.
     :param ccys: A set of currencies which are known to use this convention by default, if any.
     :return: Registered day count fraction calculation function.
     """
+
     def register_and_return_dcfc(func: DCFC) -> DCFC:
         """
         Registers the given day count fraction calculator and returns it.
 
         :param func: Day count fraction calculation function to be registered.
         :return: Registered day count fraction calculation function.
         """
         ## Create the DCC instance:
-        dcc = DCC(name, altnames or set([]), ccys or set([]), func)
+        dcc = DCC(name, altnames or set(), ccys or set(), func)
 
         ## Attempt to register the DCC:
         DCCRegistry.register(dcc)
 
         ## Attach the dcc instance to the day count fraction calculation function (for whatever it is worth):
-        setattr(func, "__dcc", dcc)
+        setattr(func, "__dcc", dcc)  # noqa: B010
 
-        ## Done, return the function (if above statment did not raise any exceptions):
+        ## Done, return the function (if above statement did not raise any exceptions):
         return func
+
     return register_and_return_dcfc
 
 
 @dcc("Act/Act", {"Actual/Actual", "Actual/Actual (ISDA)"})
-def dcfc_act_act(start: Date, asof: Date, end: Date) -> Decimal:
+def dcfc_act_act(start: Date, asof: Date, end: Date, freq: Optional[Decimal] = None) -> Decimal:
     """
     Computes the day count fraction for "Act/Act" convention.
 
     :param start: The start date of the period.
     :param asof: The date which the day count fraction to be calculated as of.
     :param end: The end date of the period (a.k.a. termination date).
+    :param freq: The frequency of payments in a year.
     :return: Day count fraction.
 
     >>> ex1_start, ex1_asof = datetime.date(2007, 12, 28), datetime.date(2008, 2, 28)
     >>> ex2_start, ex2_asof = datetime.date(2007, 12, 28), datetime.date(2008, 2, 29)
     >>> ex3_start, ex3_asof = datetime.date(2007, 10, 31), datetime.date(2008, 11, 30)
     >>> ex4_start, ex4_asof = datetime.date(2008, 2, 1), datetime.date(2009, 5, 31)
     >>> round(dcfc_act_act(start=ex1_start, asof=ex1_asof, end=ex1_asof), 14)
@@ -241,17 +476,44 @@
             ## Nope, not a leap year:
             buffer[0] += 1
 
     ## Done, compute and return:
     return Decimal(buffer[0]) / Decimal(365) + Decimal(buffer[1]) / Decimal(366)
 
 
-@dcc("Act/360", {"Actual/360", "French", "360"},
-     _as_ccys({"AUD", "CAD", "CHF", "EUR", "USD", "DKK", "CZK", "HUF", "SEK", "IDR", "NOK", "JPY", "NZD", "THB"}))
-def dcfc_act_360(start: Date, asof: Date, end: Date) -> Decimal:
+@dcc("Act/Act (ICMA)", {"Actual/Actual (ICMA)", "ISMA-99", "Act/Act (ISMA)"})
+def dcfc_act_act_icma(start: Date, asof: Date, end: Date, freq: Optional[Decimal] = None) -> Decimal:
+    """
+    Computes the day count fraction for "Act/Act (ICMA)" convention.
+
+    :param start: The start date of the period.
+    :param asof: The date which the day count fraction to be calculated as of.
+    :param end: The end date of the period (a.k.a. termination date).
+    :return: Day count fraction.
+
+    >>> ex1_start, ex1_asof, ex1_end = datetime.date(2019, 3, 2), datetime.date(2019, 9, 10), datetime.date(2020, 3, 2)
+    >>> round(dcfc_act_act_icma(start=ex1_start, asof=ex1_asof, end=ex1_end), 10)
+    Decimal('0.5245901639')
+    """
+    ## Get the number of actual days:
+    p1 = Decimal(_get_actual_day_count(start, asof))
+
+    ## Get the number of days in the period:
+    p2 = Decimal(_get_actual_day_count(start, end))
+
+    ## Compute the ratio and return:
+    return p1 / p2 / Decimal(freq or ONE)
+
+
+@dcc(
+    "Act/360",
+    {"Actual/360", "French", "360"},
+    _as_ccys({"AUD", "CAD", "CHF", "EUR", "USD", "DKK", "CZK", "HUF", "SEK", "IDR", "NOK", "JPY", "NZD", "THB"}),
+)
+def dcfc_act_360(start: Date, asof: Date, end: Date, freq: Optional[Decimal] = None) -> Decimal:
     """
     Computes the day count fraction for "Act/360" convention.
 
     :param start: The start date of the period.
     :param end: The end date of the period.
     :return: Day count fraction.
 
@@ -268,15 +530,15 @@
     >>> round(dcfc_act_360(start=ex4_start, asof=ex4_asof, end=ex4_asof), 14)
     Decimal('1.34722222222222')
     """
     return _get_actual_day_count(start, asof) / Decimal(360)
 
 
 @dcc("Act/365F", {"Actual/365 Fixed", "English", "365"}, _as_ccys({"GBP", "HKD", "INR", "PLN", "SGD", "ZAR", "MYR"}))
-def dcfc_act_365_f(start: Date, asof: Date, end: Date) -> Decimal:
+def dcfc_act_365_f(start: Date, asof: Date, end: Date, freq: Optional[Decimal] = None) -> Decimal:
     """
     Computes the day count fraction for the "Act/365F" convention.
 
     :param start: The start date of the period.
     :param asof: The date which the day count fraction to be calculated as of.
     :param end: The end date of the period (a.k.a. termination date).
     :return: Day count fraction.
@@ -294,15 +556,15 @@
     >>> round(dcfc_act_365_f(start=ex4_start, asof=ex4_asof, end=ex4_asof), 14)
     Decimal('1.32876712328767')
     """
     return _get_actual_day_count(start, asof) / Decimal(365)
 
 
 @dcc("Act/365A", {"Actual/365 Actual"})
-def dcfc_act_365_a(start: Date, asof: Date, end: Date) -> Decimal:
+def dcfc_act_365_a(start: Date, asof: Date, end: Date, freq: Optional[Decimal] = None) -> Decimal:
     """
     Computes the day count fraction for the "Act/365A" convention.
 
     :param start: The start date of the period.
     :param asof: The date which the day count fraction to be calculated as of.
     :param end: The end date of the period (a.k.a. termination date).
     :return: Day count fraction.
@@ -320,15 +582,15 @@
     >>> round(dcfc_act_365_a(start=ex4_start, asof=ex4_asof, end=ex4_asof), 14)
     Decimal('1.32513661202186')
     """
     return _get_actual_day_count(start, asof) / Decimal(366 if _has_leap_day(start, asof) else 365)
 
 
 @dcc("Act/365L", {"Actual/365 Leap Year"})
-def dcfc_act_365_l(start: Date, asof: Date, end: Date) -> Decimal:
+def dcfc_act_365_l(start: Date, asof: Date, end: Date, freq: Optional[Decimal] = None) -> Decimal:
     """
     Computes the day count fraction for the "Act/365L" convention.
 
     :param start: The start date of the period.
     :param asof: The date which the day count fraction to be calculated as of.
     :param end: The end date of the period (a.k.a. termination date).
     :return: Day count fraction.
@@ -346,15 +608,15 @@
     >>> round(dcfc_act_365_l(start=ex4_start, asof=ex4_asof, end=ex4_asof), 14)
     Decimal('1.32876712328767')
     """
     return _get_actual_day_count(start, asof) / Decimal(366 if calendar.isleap(asof.year) else 365)
 
 
 @dcc("NL/365", {"Actual/365 No Leap Year", "NL365"})
-def dcfc_nl_365(start: Date, asof: Date, end: Date) -> Decimal:
+def dcfc_nl_365(start: Date, asof: Date, end: Date, freq: Optional[Decimal] = None) -> Decimal:
     """
     Computes the day count fraction for the "NL/365" convention.
 
     :param start: The start date of the period.
     :param asof: The date which the day count fraction to be calculated as of.
     :param end: The end date of the period (a.k.a. termination date).
     :return: Day count fraction.
@@ -372,15 +634,15 @@
     >>> round(dcfc_nl_365(start=ex4_start, asof=ex4_asof, end=ex4_asof), 14)
     Decimal('1.32602739726027')
     """
     return (_get_actual_day_count(start, asof) - (1 if _has_leap_day(start, asof) else 0)) / Decimal(365)
 
 
 @dcc("30/360 ISDA", {"30/360 US Municipal", "Bond Basis"})
-def dcfc_30_360_isda(start: Date, asof: Date, end: Date) -> Decimal:
+def dcfc_30_360_isda(start: Date, asof: Date, end: Date, freq: Optional[Decimal] = None) -> Decimal:
     """
     Computes the day count fraction for the "30/360 ISDA" convention.
 
     :param start: The start date of the period.
     :param asof: The date which the day count fraction to be calculated as of.
     :param end: The end date of the period (a.k.a. termination date).
     :return: Day count fraction.
@@ -410,15 +672,15 @@
     nod = (asof.day - start.day) + 30 * (asof.month - start.month) + 360 * (asof.year - start.year)
 
     ## Done, compute and return the day count fraction:
     return nod / Decimal(360)
 
 
 @dcc("30E/360", {"30/360 ISMA", "30/360 European", "30S/360 Special German", "Eurobond Basis"})
-def dcfc_30_e_360(start: Date, asof: Date, end: Date) -> Decimal:
+def dcfc_30_e_360(start: Date, asof: Date, end: Date, freq: Optional[Decimal] = None) -> Decimal:
     """
     Computes the day count fraction for the "30E/360" convention.
 
     :param start: The start date of the period.
     :param asof: The date which the day count fraction to be calculated as of.
     :param end: The end date of the period (a.k.a. termination date).
     :return: Day count fraction.
@@ -448,15 +710,15 @@
     nod = (asof.day - start.day) + 30 * (asof.month - start.month) + 360 * (asof.year - start.year)
 
     ## Done, compute and return the day count fraction:
     return nod / Decimal(360)
 
 
 @dcc("30E+/360")
-def dcfc_30_e_plus_360(start: Date, asof: Date, end: Date) -> Decimal:
+def dcfc_30_e_plus_360(start: Date, asof: Date, end: Date, freq: Optional[Decimal] = None) -> Decimal:
     """
     Computes the day count fraction for the "30E+/360" convention.
 
     :param start: The start date of the period.
     :param asof: The date which the day count fraction to be calculated as of.
     :param end: The end date of the period (a.k.a. termination date).
     :return: Day count fraction.
@@ -487,15 +749,15 @@
     nod = (asof.day - start.day) + 30 * (asof.month - start.month) + 360 * (asof.year - start.year)
 
     ## Done, compute and return the day count fraction:
     return nod / Decimal(360)
 
 
 @dcc("30/360 German", {"30E/360 ISDA"})
-def dcfc_30_360_german(start: Date, asof: Date, end: Date) -> Decimal:
+def dcfc_30_360_german(start: Date, asof: Date, end: Date, freq: Optional[Decimal] = None) -> Decimal:
     """
     Computes the day count fraction.
 
     :param start: The start date of the period.
     :param asof: The date which the day count fraction to be calculated as of.
     :param end: The end date of the period (a.k.a. termination date).
     :return: Day count fraction.
@@ -529,15 +791,15 @@
     nod = (d2 - d1) + 30 * (asof.month - start.month) + 360 * (asof.year - start.year)
 
     ## Done, compute and return the day count fraction:
     return nod / Decimal(360)
 
 
 @dcc("30/360 US", {"30U/360", "30US/360"})
-def dcfc_30_360_us(start: Date, asof: Date, end: Date) -> Decimal:
+def dcfc_30_360_us(start: Date, asof: Date, end: Date, freq: Optional[Decimal] = None) -> Decimal:
     """
     Computes the day count fraction for the "30/360 US" convention.
 
     :param start: The start date of the period.
     :param asof: The date which the day count fraction to be calculated as of.
     :param end: The end date of the period (a.k.a. termination date).
     :return: Day count fraction.
@@ -565,15 +827,15 @@
         d1 = 30
 
         ## Shall we change the d2, too?
         if _is_last_day_of_month(asof):
             d2 = 30
 
     ## Revisit d2:
-    if d2 == 31 and (d1 == 30 or d1 == 31):
+    if d2 == 31 and (d1 in {30, 31}):
         d2 = 30
 
     ## Revisit d1:
     if d1 == 31:
         d1 = 30
 
     ## Compute number of days:
```

### Comparing `pypara-0.0.9/pypara/monetary.py` & `pypara-0.1.0/pypara/monetary.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,302 +1,552 @@
-from abc import abstractmethod
-from decimal import Decimal, InvalidOperation, DivisionByZero
-from typing import Any, Optional, NamedTuple
-
-from pypara.currencies import Currency
-from pypara.exchange import FXRateService, FXRateLookupError
-from pypara.generic import Date, Numeric, ProgrammingError
+"""
+This module provides definitions and functionality related to encoding monetary
+values and operating on them.
+"""
+
+__all__ = [
+    "IncompatibleCurrencyError",
+    "MonetaryOperationException",
+    "Money",
+    "NoMoney",
+    "NoPrice",
+    "NoneMoney",
+    "NonePrice",
+    "Price",
+    "SomeMoney",
+    "SomePrice",
+]
+
+from abc import ABC, abstractmethod
+from decimal import Decimal, DivisionByZero, InvalidOperation
+from typing import TYPE_CHECKING, Any, Callable, NamedTuple, Optional, TypeVar, Union, overload
+
+from .commons.errors import ProgrammingError
+from .commons.numbers import ZERO, Numeric
+from .commons.zeitgeist import Date
+from .currencies import Currency
+from .exchange import FXRateLookupError, FXRateService
+
+if TYPE_CHECKING:
+    from typing_extensions import TypeGuard
+else:
+    try:
+        from typing import TypeGuard
+    except ImportError:
+        from typing_extensions import TypeGuard
 
 
 class IncompatibleCurrencyError(ValueError):
     """
-    Provides an exception indicating that there is an attempt for performing monetary operations
-    with incompatible currencies.
+    Provides an exception indicating that there is an attempt for performing
+    monetary operations with incompatible currencies.
     """
 
-    def __init__(self, ccy1: Currency, ccy2: Currency, operation: str="<Unspecified>") -> None:
+    def __init__(self, ccy1: Currency, ccy2: Currency, operation: str = "<Unspecified>") -> None:
         """
         Initializes an incompatible currency error message.
         """
-        ## Keep sloys:
+        ## Keep slots:
         self.ccy1 = ccy1
         self.ccy2 = ccy2
         self.operation = operation
 
         ## Call super:
         super().__init__(f"{ccy1.code} vs {ccy2.code} are incompatible for operation '{operation}'.")
 
 
 class MonetaryOperationException(TypeError):
     """
-    Provides an exception that a certain monetary operation can not be carried on.
+    Provides an exception that a certain monetary operation can not be carried
+    on.
     """
-    pass
 
-###########################
-# BEGIN DEFINITION: Money #
-###########################
 
+_T = TypeVar("_T")
 
-class Money:
+
+class Money(ABC):
     """
     Provides an abstract money model and its semantics.
     """
 
     ## No need for slots.
     __slots__ = ()
 
-    #: Defines the *undefined* money object as a singleton.
-    NA: "Money"
+    @property
+    @abstractmethod
+    def defined(self) -> bool:
+        """
+        Indicates that the money is a *defined* monetary value.
 
-    #: Returns the currency of the money object, if defined.
-    #:
-    #: Note that a :class:`TypeError` is raised if call-site attempts to access this property of an undefined money.
-    ccy: Currency
-
-    #: Returns the quantity of the money object, if defined.
-    #:
-    #: Note that a :class:`TypeError` is raised if call-site attempts to access this property of an undefined money.
-    qty: Decimal
-
-    #: Returns the value date of the money object, if defined.
-    #:
-    #: Note that a :class:`TypeError` is raised if call-site attempts to access this property of an undefined money.
-    dov: Date
+        >>> from pypara.currencies import Currencies
+        >>> Money.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1)).defined
+        True
+        >>> Money.na().defined
+        False
+        """
 
-    #: Indicates that the money is a *defined* monetary value.
-    defined: bool  # noqa: E704
+    @property
+    @abstractmethod
+    def undefined(self) -> bool:
+        """
+        Indicates that the money is a *undefined* monetary value.
 
-    #: Indicates that the money is an *undefined* monetary value.
-    undefined: bool
+        >>> from pypara.currencies import Currencies
+        >>> Money.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1)).undefined
+        False
+        >>> Money.na().undefined
+        True
+        """
 
     @abstractmethod
     def is_equal(self, other: Any) -> bool:
         """
         Checks the equality of two money objects.
 
         In particular:
 
         1. ``True`` if ``other`` is a money object **and** all slots are same.
         2. ``False`` otherwise.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def as_boolean(self) -> bool:
         """
         Returns the logical representation of the money object.
 
         In particular:
 
         1. ``False`` if money is *undefined* **or** money quantity is ``zero``.
         2. ``True`` otherwise.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def as_float(self) -> float:
         """
-        Returns the quantity as a ``float`` if *defined*, raises class:`MonetaryOperationException` otherwise.
+        Returns the quantity as a ``float`` if *defined*, raises
+        :class:`MonetaryOperationException` otherwise.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def as_integer(self) -> int:
         """
-        Returns the quantity as an ``int`` if *defined*, raises class:`MonetaryOperationException` otherwise.
+        Returns the quantity as an ``int`` if *defined*, raises
+        :class:`MonetaryOperationException` otherwise.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def abs(self) -> "Money":
         """
         Returns the absolute money if *defined*, itself otherwise.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def negative(self) -> "Money":
         """
-        Negates the quantity of the monetary value if *defined*, itself otherwise.
+        Negates the quantity of the monetary value if *defined*, itself
+        otherwise.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def positive(self) -> "Money":
         """
         Returns same monetary value if *defined*, itself otherwise.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def round(self, ndigits: int = 0) -> "Money":
         """
-        Rounds the quantity of the monetary value to ``ndigits`` by using ``HALF_EVEN`` method if *defined*, itself
-        otherwise.
+        Rounds the quantity of the monetary value to ``ndigits`` by using
+        ``HALF_EVEN`` method if *defined*, itself otherwise.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def add(self, other: "Money") -> "Money":
         """
         Performs monetary addition on the money object and the given ``other`` money object.
 
-        Note that::
+        Note that:
 
         1. Raises :class:`IncompatibleCurrencyError` if currencies do not match.
         2. If any of the operands are undefined, returns the other one conveniently.
         3. Dates are carried forward as a result of addition of two defined money objects.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def scalar_add(self, other: Numeric) -> "Money":
         """
         Performs scalar addition on the quantity of the money.
 
         Note that undefined money object is returned as is.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def subtract(self, other: "Money") -> "Money":
         """
-        Performs monetary subtraction on the money object and the given ``other`` money object.
+        Performs monetary subtraction on the money object and the given
+        ``other`` money object.
 
-        Note that::
+        Note that:
 
         1. Raises :class:`IncompatibleCurrencyError` if currencies do not match.
-        2. If any of the operands are undefined, returns the other one conveniently.
-        3. Dates are carried forward as a result of addition of two defined money objects.
+        2. If any of the operands are undefined, returns the other one
+           conveniently.
+        3. Dates are carried forward as a result of addition of two defined
+           money objects.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def scalar_subtract(self, other: Numeric) -> "Money":
         """
         Performs scalar subtraction on the quantity of the money.
 
         Note that undefined money object is returned as is.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def multiply(self, other: Numeric) -> "Money":
         """
         Performs scalar multiplication.
 
         Note that undefined money object is returned as is.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def divide(self, other: Numeric) -> "Money":
         """
-        Performs ordinary division on the money object if *defined*, itself otherwise.
+        Performs ordinary division on the money object if *defined*, itself
+        otherwise.
 
         Note that division by zero yields an undefined money object.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def floor_divide(self, other: Numeric) -> "Money":
         """
-        Performs floor division on the money object if *defined*, itself otherwise.
+        Performs floor division on the money object if *defined*, itself
+        otherwise.
 
         Note that division by zero yields an undefined money object.
-
         """
-        raise NotImplementedError
 
     @abstractmethod
     def lt(self, other: "Money") -> bool:
         """
         Applies "less than" comparison against ``other`` money.
 
-        Note that::
+        Note that:
 
-        1. Undefined money objects are always less than ``other`` if ``other`` is not undefined, and
-        2. :class:`IncompatibleCurrencyError` is raised when comparing two defined money objects with different
-        currencies.
+        1. Undefined money objects are always less than ``other`` if ``other``
+           is not undefined, and
+        2. :class:`IncompatibleCurrencyError` is raised when comparing two
+           defined money objects with different currencies.
         """
-        pass
 
     @abstractmethod
     def lte(self, other: "Money") -> bool:
         """
         Applies "less than or equal to" comparison against ``other`` money.
 
-        Note that::
+        Note that:
 
-        1. Undefined money objects are always less than or equal to ``other``, and
-        2. :class:`IncompatibleCurrencyError` is raised when comparing two defined money objects with different
-        currencies.
+        1. Undefined money objects are always less than or equal to ``other``,
+           and
+        2. :class:`IncompatibleCurrencyError` is raised when comparing two
+           defined money objects with different currencies.
         """
-        pass
 
     @abstractmethod
     def gt(self, other: "Money") -> bool:
         """
         Applies "greater than" comparison against ``other`` money.
 
-        Note that::
+        Note that:
 
         1. Undefined money objects are never greater than ``other``,
-        2. Defined money objects are always greater than ``other`` if other is undefined, and
-        3. :class:`IncompatibleCurrencyError` is raised when comparing two defined money objects with different
-        currencies.
+        2. Defined money objects are always greater than ``other`` if other is
+           undefined, and
+        3. :class:`IncompatibleCurrencyError` is raised when comparing two
+           defined money objects with different currencies.
         """
-        pass
 
     @abstractmethod
     def gte(self, other: "Money") -> bool:
         """
         Applies "greater than or equal to" comparison against ``other`` money.
 
-        Note that::
+        Note that:
 
-        1. Undefined money objects are never greater than or equal to ``other`` if ``other`` is defined,
-        2. Undefined money objects are greater than or equal to ``other`` if ``other is undefined, and
-        3. :class:`IncompatibleCurrencyError` is raised when comparing two defined money objects with different
-        currencies.
+        1. Undefined money objects are never greater than or equal to ``other``
+           if ``other`` is defined,
+        2. Undefined money objects are greater than or equal to ``other`` if
+           ``other`` is undefined, and
+        3. :class:`IncompatibleCurrencyError` is raised when comparing two
+           defined money objects with different currencies.
+        """
+
+    @abstractmethod
+    def or_else(self, e: Callable[[], "Money"]) -> "Money":
+        """
+        Returns itself if the monetary value is defined, the value of the given
+        combinator otherwise.
+
+        >>> from pypara.currencies import Currencies
+        >>> fallback = Money.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1))
+        >>> somemoney = Money.of(Currencies["EUR"], Decimal('2'), Date(2019, 1, 2))
+        >>> nonemoney = Money.of(None, Decimal('1'), None)
+        >>> somemoney.or_else(lambda: fallback) is somemoney
+        True
+        >>> nonemoney.or_else(lambda: fallback) is fallback
+        True
+        """
+
+    @abstractmethod
+    def fmap(self, f: Callable[["SomeMoney"], "Money"]) -> "Money":
+        """
+        Consumes a given function that consumes a defined monetary value and
+        applies to the value if defined, and returns its value, undefined
+        monetary value otherwise.
+
+        >>> import datetime
+        >>> from pypara.currencies import Currencies
+        >>> somemoney = Money.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1))
+        >>> new = somemoney.fmap(lambda x: Money.of(x.ccy, x.qty + Decimal('1'), x.dov + datetime.timedelta(days=10)))
+        >>> new.ccy.code
+        'USD'
+        >>> new.qty
+        Decimal('2.00')
+        >>> new.dov
+        datetime.date(2019, 1, 11)
+        >>> nonemoney = Money.of(None, Decimal('1'), None)
+        >>> nonemoney.fmap(lambda sm: Money.of(sm.ccy, sm.qty + Decimal('1'), sm.dov)) is Money.na()
+        True
+        """
+
+    @abstractmethod
+    def dimap(self, f: Callable[["SomeMoney"], _T], e: Callable[[], _T]) -> _T:
+        """
+        Consumes a given function that consumes a defined monetary value and
+        applies to the value if defined, and returns its value, the result of
+        the application of the given combinator otherwise.
+
+        >>> from pypara.currencies import Currencies
+        >>> somemoney = Money.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1))
+        >>> somemoney.dimap(lambda x: x.ccy.code, lambda: "EUR")
+        'USD'
+        >>> nonemoney = Money.of(None, Decimal('1'), None)
+        >>> nonemoney.dimap(lambda x: x.ccy.code, lambda: "EUR")
+        'EUR'
         """
-        pass
 
     @abstractmethod
     def with_ccy(self, ccy: Currency) -> "Money":
         """
-        Creates a new money object with the given currency if money is *defined*, returns itself otherwise.
+        Creates a new money object with the given currency if money is
+        *defined*, returns itself otherwise.
         """
-        pass
 
     @abstractmethod
     def with_qty(self, qty: Decimal) -> "Money":
         """
-        Creates a new money object with the given quantity if money is *defined*, returns itself otherwise.
+        Creates a new money object with the given quantity if money is
+        *defined*, returns itself otherwise.
         """
-        pass
 
     @abstractmethod
     def with_dov(self, dov: Date) -> "Money":
         """
-        Creates a new money object with the given value date if money is *defined*, returns itself otherwise.
+        Creates a new money object with the given value date if money is
+        *defined*, returns itself otherwise.
+        """
+
+    @abstractmethod
+    def ccy_or(self, default: Currency) -> Currency:
+        """
+        Returns the ``ccy`` if the monetary value is *defined*, ``default``
+        otherwise.
+
+        >>> from pypara.currencies import Currencies
+        >>> somemoney = Money.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1))
+        >>> somemoney.ccy_or(Currencies["EUR"]).code
+        'USD'
+        >>> nonemoney = Money.of(Currencies["USD"], None, None)
+        >>> nonemoney.ccy_or(Currencies["EUR"]).code
+        'EUR'
+        """
+
+    @abstractmethod
+    def ccy_or_none(self) -> Optional[Currency]:
+        """
+        Returns the ``ccy`` if the monetary value is *defined*, ``None``
+        otherwise.
+
+        >>> from pypara.currencies import Currencies
+        >>> somemoney = Money.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1))
+        >>> somemoney.ccy_or_none().code
+        'USD'
+        >>> nonemoney = Money.of(Currencies["USD"], None, None)
+        >>> nonemoney.ccy_or_none() is None
+        True
+        """
+
+    @abstractmethod
+    def qty_or(self, default: Decimal) -> Decimal:
+        """
+        Returns the ``qty`` if the monetary value is *defined*, ``default`` otherwise.
+
+        >>> from pypara.currencies import Currencies
+        >>> somemoney = Money.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1))
+        >>> somemoney.qty_or(Decimal(0))
+        Decimal('1.00')
+        >>> nonemoney = Money.of(None, Decimal('1'), None)
+        >>> nonemoney.qty_or(Decimal(0))
+        Decimal('0')
+        """
+
+    @abstractmethod
+    def qty_or_zero(self) -> Decimal:
+        """
+        Returns the ``qty`` if the monetary value is *defined*, ``0`` otherwise.
+
+        >>> from pypara.currencies import Currencies
+        >>> somemoney = Money.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1))
+        >>> somemoney.qty_or_zero()
+        Decimal('1.00')
+        >>> nonemoney = Money.of(None, Decimal('1'), None)
+        >>> nonemoney.qty_or_zero()
+        Decimal('0')
+        """
+
+    @abstractmethod
+    def qty_or_none(self) -> Optional[Decimal]:
+        """
+        Returns the ``qty`` if the monetary value is *defined*, ``None`` otherwise.
+
+        >>> from pypara.currencies import Currencies
+        >>> somemoney = Money.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1))
+        >>> somemoney.qty_or_none()
+        Decimal('1.00')
+        >>> nonemoney = Money.of(None, Decimal('1'), None)
+        >>> nonemoney.qty_or_none() is None
+        True
+        """
+
+    @abstractmethod
+    def qty_or_else(self, e: Callable[[], _T]) -> Union[Decimal, _T]:
+        """
+        Returns the ``qty`` if the monetary value is *defined*, the value of the
+        call of provided combinator otherwise.
+
+        >>> from pypara.currencies import Currencies
+        >>> somemoney = Money.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1))
+        >>> somemoney.qty_or_else(lambda: Decimal('42'))
+        Decimal('1.00')
+        >>> somemoney.qty_or_else(lambda: True)
+        Decimal('1.00')
+        >>> nonemoney = Money.of(None, Decimal('1'), None)
+        >>> nonemoney.qty_or_else(lambda: Decimal('42'))
+        Decimal('42')
+        >>> nonemoney.qty_or_else(lambda: False)
+        False
+        """
+
+    @abstractmethod
+    def qty_map(self, f: Callable[[Decimal], _T], e: Callable[[], _T]) -> _T:
+        """
+        Applies the given function to the ``qty`` and returns the result if the
+        monetary value is *defined*, returns the value of the call of provided
+        combinator otherwise.
+
+        >>> from pypara.currencies import Currencies
+        >>> somemoney = Money.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1))
+        >>> somemoney.qty_map(lambda x: x + Decimal('1'), lambda: Decimal('42'))
+        Decimal('2.00')
+        >>> nonemoney = Money.of(None, Decimal('1'), None)
+        >>> nonemoney.qty_map(lambda x: x + Decimal('1'), lambda: Decimal('42'))
+        Decimal('42')
+        """
+
+    @abstractmethod
+    def dov_or(self, default: Date) -> Date:
+        """
+        Returns the ``dov`` if the monetary value is *defined*, ``default`` otherwise.
+
+        >>> from pypara.currencies import Currencies
+        >>> somemoney = Money.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1))
+        >>> somemoney.dov_or(Date(2001, 1, 1))
+        datetime.date(2019, 1, 1)
+        >>> nonemoney = Money.of(None, None, Date(2019, 1, 1))
+        >>> nonemoney.dov_or(Date(2001, 1, 1))
+        datetime.date(2001, 1, 1)
+        """
+
+    @abstractmethod
+    def dov_or_none(self) -> Optional[Date]:
+        """
+        Returns the ``dov`` if the monetary value is *defined*, ``None``
+        otherwise.
+
+        >>> from pypara.currencies import Currencies
+        >>> somemoney = Money.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1))
+        >>> somemoney.dov_or_none()
+        datetime.date(2019, 1, 1)
+        >>> nonemoney = Money.of(None, None, Date(2019, 1, 1))
+        >>> nonemoney.dov_or_none() is None
+        True
         """
-        pass
 
     @abstractmethod
     def convert(self, to: Currency, asof: Optional[Date] = None, strict: bool = False) -> "Money":
         """
         Converts the monetary value from one currency to another.
 
-        Raises :class:`FXRateLookupError` if no foreign exchange rate can be found for conversion.
+        Raises :class:`FXRateLookupError` if no foreign exchange rate can be
+        found for conversion.
 
         Note that we will carry the date forward as per ``asof`` date.
         """
-        raise NotImplementedError
+
+    @classmethod
+    def na(cls) -> "Money":
+        """
+        Undefined money instance.
+
+        >>> Money.na().defined
+        False
+        >>> Money.na().undefined
+        True
+        """
+        return NoMoney
+
+    @staticmethod
+    def is_none(x: "Money") -> TypeGuard["NoneMoney"]:
+        """
+        Type guard for undefined money instances.
+
+        >>> from pypara.currencies import Currencies
+        >>> Money.is_none(Money.na())
+        True
+        >>> Money.is_none(Money.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1)))
+        False
+        """
+        return x.undefined
+
+    @staticmethod
+    def is_some(x: "Money") -> TypeGuard["SomeMoney"]:
+        """
+        Type guard for defined money instances.
+
+        >>> from pypara.currencies import Currencies
+        >>> Money.is_some(Money.na())
+        False
+        >>> Money.is_some(Money.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1)))
+        True
+        """
+        return x.defined
 
     @classmethod
     def of(cls, ccy: Optional[Currency], qty: Optional[Decimal], dov: Optional[Date]) -> "Money":
         """
         Provides a factory method to create a new money object in a safe manner.
         """
         if qty is None or ccy is None or dov is None:
@@ -305,95 +555,109 @@
 
     @property
     @abstractmethod
     def price(self) -> "Price":
         """
         Returns the price representation of the money object.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def __bool__(self) -> bool:
-        pass
+        ...
 
     @abstractmethod
     def __eq__(self, other: Any) -> bool:
-        pass
+        ...
 
     @abstractmethod
     def __abs__(self) -> "Money":
-        pass
+        ...
 
     @abstractmethod
     def __float__(self) -> float:
-        pass
+        ...
 
     @abstractmethod
     def __int__(self) -> int:
-        pass
+        ...
 
-    @abstractmethod
-    def __round__(self, ndigits: int = 0) -> "Money":
-        pass
+    @overload
+    def __round__(self) -> int:
+        ...
+
+    @overload
+    def __round__(self, ndigits: None) -> int:
+        ...
+
+    @overload
+    def __round__(self, ndigits: int) -> "Money":
+        ...
+
+    def __round__(self, ndigits: Optional[int] = 0) -> Union["Money", int]:
+        return self.round(ndigits or 0)
 
     @abstractmethod
     def __neg__(self) -> "Money":
-        pass
+        ...
 
     @abstractmethod
     def __pos__(self) -> "Money":
-        pass
+        ...
 
     @abstractmethod
     def __add__(self, other: "Money") -> "Money":
-        pass
+        ...
 
     @abstractmethod
     def __sub__(self, other: "Money") -> "Money":
-        pass
+        ...
 
     @abstractmethod
     def __mul__(self, other: Numeric) -> "Money":
-        pass
+        ...
 
     @abstractmethod
     def __truediv__(self, other: Numeric) -> "Money":
-        pass
+        ...
 
     @abstractmethod
     def __floordiv__(self, other: Numeric) -> "Money":
-        pass
+        ...
 
     @abstractmethod
     def __lt__(self, other: "Money") -> bool:
-        pass
+        ...
 
     @abstractmethod
     def __le__(self, other: "Money") -> bool:
-        pass
+        ...
 
     @abstractmethod
     def __gt__(self, other: "Money") -> bool:
-        pass
+        ...
 
     @abstractmethod
     def __ge__(self, other: "Money") -> bool:
-        pass
+        ...
 
 
-class SomeMoney(Money, NamedTuple("SomeMoney", [("ccy", Currency), ("qty", Decimal), ("dov", Date)])):  # type: ignore
+class SomeMoney(Money, NamedTuple("SomeMoney", [("ccy", Currency), ("qty", Decimal), ("dov", Date)])):
     """
     Provides a *defined* money object model.
     """
 
     __slots__ = ()
 
-    defined = True
+    @property
+    def defined(self) -> bool:
+        return True
 
-    undefined = False
+    @property
+    def undefined(self) -> bool:
+        return False
 
     def is_equal(self, other: Any) -> bool:
         return other.__class__ is SomeMoney and tuple(self) == tuple(other)
 
     def as_boolean(self) -> bool:
         return self[1].__bool__()
 
@@ -413,110 +677,158 @@
 
     def positive(self) -> "Money":
         c, q, d = self
         return SomeMoney(c, q.__pos__(), d)
 
     def round(self, ndigits: int = 0) -> "Money":
         c, q, d = self
-        dec = c[2]
-        return SomeMoney(c, q.__round__(ndigits if ndigits < dec else dec), d)  # type: ignore
+        dec = c.decimals
+        return SomeMoney(c, q.__round__(ndigits if ndigits < dec else dec), d)
 
     def add(self, other: "Money") -> "Money":
         if other.undefined:
             return self
 
+        c1: Currency
+        q1: Decimal
+        d1: Date
+        c2: Currency
+        q2: Decimal
+        d2: Date
         c1, q1, d1 = self
         c2, q2, d2 = other  # type: ignore
 
         if c1 != c2:
             raise IncompatibleCurrencyError(ccy1=c1, ccy2=c2, operation="addition")
 
         return SomeMoney(c1, q1 + q2, d1 if d1 > d2 else d2)
 
     def scalar_add(self, other: Numeric) -> "Money":
         ## TODO: **try** not casting other to Decimal.
         c, q, d = self
-        return SomeMoney(c, (q + Decimal(other)).quantize(c[4]), d)
+        return SomeMoney(c, (q + Decimal(other)).quantize(c.quantizer), d)
 
     def subtract(self, other: "Money") -> "Money":
         if other.undefined:
             return self
 
+        c1: Currency
+        q1: Decimal
+        d1: Date
+        c2: Currency
+        q2: Decimal
+        d2: Date
         c1, q1, d1 = self
         c2, q2, d2 = other  # type: ignore
 
         if c1 != c2:
             raise IncompatibleCurrencyError(ccy1=c1, ccy2=c2, operation="subtraction")
 
         return SomeMoney(c1, q1 - q2, d1 if d1 > d2 else d2)
 
     def scalar_subtract(self, other: Numeric) -> "Money":
         ## TODO: **try** not casting other to Decimal.
         c, q, d = self
-        return SomeMoney(c, (q - Decimal(other)).quantize(c[4]), d)
+        return SomeMoney(c, (q - Decimal(other)).quantize(c.quantizer), d)
 
     def multiply(self, other: Numeric) -> "Money":
         ## TODO: **try** not casting other to Decimal.
         c, q, d = self
-        return SomeMoney(c, (q * Decimal(other)).quantize(c[4]), d)
+        return SomeMoney(c, (q * Decimal(other)).quantize(c.quantizer), d)
 
     def divide(self, other: Numeric) -> "Money":
         ## TODO: **try** not casting other to Decimal.
         try:
             c, q, d = self
-            return SomeMoney(c, (q / Decimal(other)).quantize(c[4]), d)
-        except (InvalidOperation, DivisionByZero) as ex:
+            return SomeMoney(c, (q / Decimal(other)).quantize(c.quantizer), d)
+        except (InvalidOperation, DivisionByZero):
             return NoMoney
 
     def floor_divide(self, other: Numeric) -> "Money":
         ## TODO: **try** not casting other to Decimal.
         try:
             c, q, d = self
-            return SomeMoney(c, (q // Decimal(other)).quantize(c[4]), d)
-        except (InvalidOperation, DivisionByZero) as ex:
+            return SomeMoney(c, (q // Decimal(other)).quantize(c.quantizer), d)
+        except (InvalidOperation, DivisionByZero):
             return NoMoney
 
     def lt(self, other: "Money") -> bool:
-        if other.undefined:
+        if not isinstance(other, SomeMoney):
             return False
         elif self.ccy != other.ccy:
-            raise IncompatibleCurrencyError(ccy1=self.ccy, ccy2=other.ccy, operation="< comparision")
+            raise IncompatibleCurrencyError(ccy1=self.ccy, ccy2=other.ccy, operation="< comparison")
         return self.qty < other.qty
 
     def lte(self, other: "Money") -> bool:
-        if other.undefined:
+        if not isinstance(other, SomeMoney):
             return False
         elif self.ccy != other.ccy:
-            raise IncompatibleCurrencyError(ccy1=self.ccy, ccy2=other.ccy, operation="<= comparision")
+            raise IncompatibleCurrencyError(ccy1=self.ccy, ccy2=other.ccy, operation="<= comparison")
         return self.qty <= other.qty
 
     def gt(self, other: "Money") -> bool:
-        if other.undefined:
+        if not isinstance(other, SomeMoney):
             return True
         elif self.ccy != other.ccy:
-            raise IncompatibleCurrencyError(ccy1=self.ccy, ccy2=other.ccy, operation="> comparision")
+            raise IncompatibleCurrencyError(ccy1=self.ccy, ccy2=other.ccy, operation="> comparison")
         return self.qty > other.qty
 
     def gte(self, other: "Money") -> bool:
-        if other.undefined:
+        if not isinstance(other, SomeMoney):
             return True
         elif self.ccy != other.ccy:
-            raise IncompatibleCurrencyError(ccy1=self.ccy, ccy2=other.ccy, operation=">= comparision")
+            raise IncompatibleCurrencyError(ccy1=self.ccy, ccy2=other.ccy, operation=">= comparison")
         return self.qty >= other.qty
 
+    def or_else(self, e: Callable[[], "Money"]) -> "Money":
+        return self
+
+    def fmap(self, f: Callable[["SomeMoney"], "Money"]) -> "Money":
+        return f(self)
+
+    def dimap(self, f: Callable[["SomeMoney"], _T], e: Callable[[], _T]) -> _T:
+        return f(self)
+
     def with_ccy(self, ccy: Currency) -> "Money":
         return SomeMoney(ccy, self[1], self[2])
 
     def with_qty(self, qty: Decimal) -> "Money":
         c, q, d = self
-        return SomeMoney(c, qty.quantize(c[4]), d)
+        return SomeMoney(c, qty.quantize(c.quantizer), d)
 
     def with_dov(self, dov: Date) -> "Money":
         return SomeMoney(self[0], self[1], dov)
 
+    def ccy_or(self, default: Currency) -> Currency:
+        return self[0]
+
+    def ccy_or_none(self) -> Optional[Currency]:
+        return self[0]
+
+    def qty_or(self, default: Decimal) -> Decimal:
+        return self[1]
+
+    def qty_or_zero(self) -> Decimal:
+        return self[1]
+
+    def qty_or_none(self) -> Optional[Decimal]:
+        return self[1]
+
+    def qty_or_else(self, e: Callable[[], _T]) -> Union[Decimal, _T]:
+        return self[1]
+
+    def qty_map(self, f: Callable[[Decimal], _T], e: Callable[[], _T]) -> _T:
+        return f(self[1])
+
+    def dov_or(self, default: Date) -> Date:
+        return self[2]
+
+    def dov_or_none(self) -> Optional[Date]:
+        return self[2]
+
     def convert(self, to: Currency, asof: Optional[Date] = None, strict: bool = False) -> "Money":
         ## Get slots:
         ccy, qty, dov = self
 
         ## Get date of conversion:
         asof = asof or dov
 
@@ -536,15 +848,15 @@
                 ## Yep:
                 raise FXRateLookupError(ccy, to, asof)
             else:
                 ## Just return NA:
                 return NoMoney
 
         ## Compute and return:
-        return SomeMoney(to, (qty * rate.value).quantize(to[4]), asof)
+        return SomeMoney(to, (qty * rate.value).quantize(to.quantizer), asof)
 
     @property
     def price(self) -> "Price":
         return SomePrice(*self)
 
     __bool__ = as_boolean
 
@@ -552,46 +864,47 @@
 
     __abs__ = abs
 
     __float__ = as_float
 
     __int__ = as_integer
 
-    __round__ = round
-
     __neg__ = negative
 
     __pos__ = positive
 
-    __add__ = add
+    __add__ = add  # type: ignore
 
     __sub__ = subtract
 
-    __mul__ = multiply
+    __mul__ = multiply  # type: ignore
 
     __truediv__ = divide
 
     __floordiv__ = floor_divide
 
-    __lt__ = lt
+    __lt__ = lt  # type: ignore
 
-    __le__ = lte
+    __le__ = lte  # type: ignore
 
-    __gt__ = gt
+    __gt__ = gt  # type: ignore
 
-    __ge__ = gte
+    __ge__ = gte  # type: ignore
 
 
 class NoneMoney(Money):
-
     __slots__ = ()
 
-    defined = False
+    @property
+    def defined(self) -> bool:
+        return False
 
-    undefined = True
+    @property
+    def undefined(self) -> bool:
+        return True
 
     def as_boolean(self) -> bool:
         return False
 
     def is_equal(self, other: Any) -> bool:
         return other.__class__ is NoneMoney
 
@@ -642,23 +955,59 @@
 
     def gt(self, other: "Money") -> bool:
         return False
 
     def gte(self, other: "Money") -> bool:
         return other.undefined
 
+    def or_else(self, e: Callable[[], "Money"]) -> "Money":
+        return e()
+
+    def fmap(self, f: Callable[["SomeMoney"], "Money"]) -> "Money":
+        return self
+
+    def dimap(self, f: Callable[["SomeMoney"], _T], e: Callable[[], _T]) -> _T:
+        return e()
+
     def with_ccy(self, ccy: Currency) -> "Money":
         return self
 
     def with_qty(self, qty: Decimal) -> "Money":
         return self
 
     def with_dov(self, dov: Date) -> "Money":
         return self
 
+    def ccy_or(self, default: Currency) -> Currency:
+        return default
+
+    def ccy_or_none(self) -> Optional[Currency]:
+        return None
+
+    def qty_or(self, default: Decimal) -> Decimal:
+        return default
+
+    def qty_or_zero(self) -> Decimal:
+        return ZERO
+
+    def qty_or_none(self) -> Optional[Decimal]:
+        return None
+
+    def qty_or_else(self, e: Callable[[], _T]) -> Union[Decimal, _T]:
+        return e()
+
+    def qty_map(self, f: Callable[[Decimal], _T], e: Callable[[], _T]) -> _T:
+        return e()
+
+    def dov_or(self, default: Date) -> Date:
+        return default
+
+    def dov_or_none(self) -> Optional[Date]:
+        return None
+
     def convert(self, to: Currency, asof: Optional[Date] = None, strict: bool = False) -> "Money":
         return self
 
     @property
     def price(self) -> "Price":
         return NoPrice
 
@@ -668,16 +1017,14 @@
 
     __abs__ = abs
 
     __float__ = as_float
 
     __int__ = as_integer
 
-    __round__ = round
-
     __neg__ = negative
 
     __pos__ = positive
 
     __add__ = add
 
     __sub__ = subtract
@@ -693,388 +1040,623 @@
     __le__ = lte
 
     __gt__ = gt
 
     __ge__ = gte
 
 
-## Define and attach undefined money singleton.
-Money.NA = NoMoney = NoneMoney()
+#: Undefined money instance.
+NoMoney = NoneMoney()
 
-#########################
-# END DEFINITION: Money #
-#########################
 
-###########################
-# BEGIN DEFINITION: Price #
-###########################
-
-
-class Price:
+class Price(ABC):
     """
     Provides an abstract price model and its semantics.
     """
 
     ## No need for slots.
     __slots__ = ()
 
-    #: Defines the *undefined* price object as a singleton.
-    NA: "Price"
+    @property
+    @abstractmethod
+    def defined(self) -> bool:
+        """
+        Indicates that the price is a *defined* monetary value.
 
-    #: Returns the currency of the price object, if defined.
-    #:
-    #: Note that a :class:`TypeError` is raised if call-site attempts to access this property of an undefined price.
-    ccy: Currency
-
-    #: Returns the quantity of the price object, if defined.
-    #:
-    #: Note that a :class:`TypeError` is raised if call-site attempts to access this property of an undefined price.
-    qty: Decimal
-
-    #: Returns the value date of the price object, if defined.
-    #:
-    #: Note that a :class:`TypeError` is raised if call-site attempts to access this property of an undefined price.
-    dov: Date
+        >>> from pypara.currencies import Currencies
+        >>> Price.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1)).defined
+        True
+        >>> Price.na().defined
+        False
+        """
 
-    #: Indicates that the price is a *defined* monetary value.
-    defined: bool  # noqa: E704
+    @property
+    @abstractmethod
+    def undefined(self) -> bool:
+        """
+        Indicates that the price is a *undefined* monetary value.
 
-    #: Indicates that the price is an *undefined* monetary value.
-    undefined: bool
+        >>> from pypara.currencies import Currencies
+        >>> Price.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1)).undefined
+        False
+        >>> Price.na().undefined
+        True
+        """
 
     @abstractmethod
     def is_equal(self, other: Any) -> bool:
         """
         Checks the equality of two price objects.
 
         In particular:
 
         1. ``True`` if ``other`` is a price object **and** all slots are same.
         2. ``False`` otherwise.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def as_boolean(self) -> bool:
         """
         Returns the logical representation of the price object.
 
         In particular:
 
         1. ``False`` if price is *undefined* **or** price quantity is ``zero``.
         2. ``True`` otherwise.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def as_float(self) -> float:
         """
-        Returns the quantity as a ``float`` if *defined*, raises class:`MonetaryOperationException` otherwise.
+        Returns the quantity as a ``float`` if *defined*, raises
+        class:`MonetaryOperationException` otherwise.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def as_integer(self) -> int:
         """
-        Returns the quantity as an ``int`` if *defined*, raises class:`MonetaryOperationException` otherwise.
+        Returns the quantity as an ``int`` if *defined*, raises
+        class:`MonetaryOperationException` otherwise.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def abs(self) -> "Price":
         """
         Returns the absolute price if *defined*, itself otherwise.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def negative(self) -> "Price":
         """
-        Negates the quantity of the monetary value if *defined*, itself otherwise.
+        Negates the quantity of the monetary value if *defined*, itself
+        otherwise.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def positive(self) -> "Price":
         """
         Returns same monetary value if *defined*, itself otherwise.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def round(self, ndigits: int = 0) -> "Price":
         """
-        Rounds the quantity of the monetary value to ``ndigits`` by using ``HALF_EVEN`` method if *defined*, itself
-        otherwise.
+        Rounds the quantity of the monetary value to ``ndigits`` by using
+        ``HALF_EVEN`` method if *defined*, itself otherwise.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def add(self, other: "Price") -> "Price":
         """
-        Performs monetary addition on the price object and the given ``other`` price object.
+        Performs monetary addition on the price object and the given ``other``
+        price object.
 
-        Note that::
+        Note that:
 
         1. Raises :class:`IncompatibleCurrencyError` if currencies do not match.
-        2. If any of the operands are undefined, returns the other one conveniently.
-        3. Dates are carried forward as a result of addition of two defined price objects.
+        2. If any of the operands are undefined, returns the other one
+           conveniently.
+        3. Dates are carried forward as a result of addition of two defined
+           price objects.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def scalar_add(self, other: Numeric) -> "Price":
         """
         Performs scalar addition on the quantity of the price.
 
         Note that undefined price object is returned as is.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def subtract(self, other: "Price") -> "Price":
         """
-        Performs monetary subtraction on the price object and the given ``other`` price object.
+        Performs monetary subtraction on the price object and the given
+        ``other`` price object.
 
-        Note that::
+        Note that:
 
         1. Raises :class:`IncompatibleCurrencyError` if currencies do not match.
-        2. If any of the operands are undefined, returns the other one conveniently.
-        3. Dates are carried forward as a result of addition of two defined price objects.
+        2. If any of the operands are undefined, returns the other one
+           conveniently.
+        3. Dates are carried forward as a result of addition of two defined
+           price objects.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def scalar_subtract(self, other: Numeric) -> "Price":
         """
         Performs scalar subtraction on the quantity of the price.
 
         Note that undefined price object is returned as is.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def multiply(self, other: Numeric) -> "Price":
         """
         Performs scalar multiplication.
 
         Note that undefined price object is returned as is.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def times(self, other: Numeric) -> "Money":
         """
         Performs monetary multiplication operation.
 
         Note that undefined price object is returned as is.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def divide(self, other: Numeric) -> "Price":
         """
-        Performs ordinary division on the price object if *defined*, itself otherwise.
+        Performs ordinary division on the price object if *defined*, itself
+        otherwise.
 
         Note that division by zero yields an undefined price object.
         """
-        raise NotImplementedError
 
     @abstractmethod
     def floor_divide(self, other: Numeric) -> "Price":
         """
-        Performs floor division on the price object if *defined*, itself otherwise.
+        Performs floor division on the price object if *defined*, itself
+        otherwise.
 
         Note that division by zero yields an undefined price object.
 
         """
-        raise NotImplementedError
 
     @abstractmethod
     def lt(self, other: "Price") -> bool:
         """
         Applies "less than" comparison against ``other`` price.
 
-        Note that::
+        Note that:
 
-        1. Undefined price objects are always less than ``other`` if ``other`` is not undefined, and
-        2. :class:`IncompatibleCurrencyError` is raised when comparing two defined price objects with different
-        currencies.
+        1. Undefined price objects are always less than ``other`` if ``other``
+           is not undefined, and
+        2. :class:`IncompatibleCurrencyError` is raised when comparing two
+           defined price objects with different currencies.
         """
-        pass
 
     @abstractmethod
     def lte(self, other: "Price") -> bool:
         """
         Applies "less than or equal to" comparison against ``other`` price.
 
-        Note that::
+        Note that:
 
-        1. Undefined price objects are always less than or equal to ``other``, and
-        2. :class:`IncompatibleCurrencyError` is raised when comparing two defined price objects with different
-        currencies.
+        1. Undefined price objects are always less than or equal to ``other``,
+           and
+        2. :class:`IncompatibleCurrencyError` is raised when comparing two
+           defined price objects with different currencies.
         """
-        pass
 
     @abstractmethod
     def gt(self, other: "Price") -> bool:
         """
         Applies "greater than" comparison against ``other`` price.
 
-        Note that::
+        Note that:
 
         1. Undefined price objects are never greater than ``other``,
-        2. Defined price objects are always greater than ``other`` if other is undefined, and
-        3. :class:`IncompatibleCurrencyError` is raised when comparing two defined price objects with different
-        currencies.
+        2. Defined price objects are always greater than ``other`` if other is
+           undefined, and
+        3. :class:`IncompatibleCurrencyError` is raised when comparing two
+           defined price objects with different currencies.
         """
-        pass
 
     @abstractmethod
     def gte(self, other: "Price") -> bool:
         """
         Applies "greater than or equal to" comparison against ``other`` price.
 
-        Note that::
+        Note that:
 
-        1. Undefined price objects are never greater than or equal to ``other`` if ``other`` is defined,
-        2. Undefined price objects are greater than or equal to ``other`` if ``other is undefined, and
-        3. :class:`IncompatibleCurrencyError` is raised when comparing two defined price objects with different
-        currencies.
+        1. Undefined price objects are never greater than or equal to ``other``
+           if ``other`` is defined,
+        2. Undefined price objects are greater than or equal to ``other`` if
+           ``other`` is undefined, and
+        3. :class:`IncompatibleCurrencyError` is raised when comparing two
+           defined price objects with different currencies.
+        """
+
+    @abstractmethod
+    def or_else(self, e: Callable[[], "Price"]) -> "Price":
+        """
+        Returns itself if the monetary value is defined, the value of the given
+        combinator otherwise.
+
+        >>> from pypara.currencies import Currencies
+        >>> fallback = Price.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1))
+        >>> someprice = Price.of(Currencies["EUR"], Decimal('2'), Date(2019, 1, 2))
+        >>> noneprice = Price.of(None, Decimal('1'), None)
+        >>> someprice.or_else(lambda: fallback) is someprice
+        True
+        >>> noneprice.or_else(lambda: fallback) is fallback
+        True
+        """
+
+    @abstractmethod
+    def fmap(self, f: Callable[["SomePrice"], "Price"]) -> "Price":
+        """
+        Consumes a given function that consumes a defined monetary value and
+        applies to the value if defined, and returns its value, undefined
+        monetary value otherwise.
+
+        >>> import datetime
+        >>> from pypara.currencies import Currencies
+        >>> someprice = Price.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1))
+        >>> new = someprice.fmap(lambda x: Price.of(x.ccy, x.qty + Decimal('1'), x.dov + datetime.timedelta(days=10)))
+        >>> new.ccy.code
+        'USD'
+        >>> new.qty
+        Decimal('2')
+        >>> new.dov
+        datetime.date(2019, 1, 11)
+        >>> noneprice = Price.of(None, Decimal('1'), None)
+        >>> noneprice.fmap(lambda sp: Price.of(sp.ccy, sp.qty + Decimal('1'), sp.dov)) is Price.na()
+        True
+        """
+
+    @abstractmethod
+    def dimap(self, f: Callable[["SomePrice"], _T], e: Callable[[], _T]) -> _T:
+        """
+        Consumes a given function that consumes a defined monetary value and
+        applies to the value if defined, and returns its value, the result of
+        the application of the given combinator otherwise.
+
+        >>> from pypara.currencies import Currencies
+        >>> someprice = Price.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1))
+        >>> someprice.dimap(lambda x: x.ccy.code, lambda: "EUR")
+        'USD'
+        >>> noneprice = Price.of(None, Decimal('1'), None)
+        >>> noneprice.dimap(lambda x: x.ccy.code, lambda: "EUR")
+        'EUR'
         """
-        pass
 
     @abstractmethod
     def with_ccy(self, ccy: Currency) -> "Price":
         """
-        Creates a new price object with the given currency if price is *defined*, returns itself otherwise.
+        Creates a new price object with the given currency if price is
+        *defined*, returns itself otherwise.
         """
-        pass
 
     @abstractmethod
     def with_qty(self, qty: Decimal) -> "Price":
         """
-        Creates a new price object with the given quantity if price is *defined*, returns itself otherwise.
+        Creates a new price object with the given quantity if price is
+        *defined*, returns itself otherwise.
         """
-        pass
 
     @abstractmethod
     def with_dov(self, dov: Date) -> "Price":
         """
         Creates a new price object with the given value date if price is *defined*, returns itself otherwise.
         """
-        pass
+
+    @abstractmethod
+    def ccy_or(self, default: Currency) -> Currency:
+        """
+        Returns the ``ccy`` if the monetary value is *defined*, ``default``
+        otherwise.
+
+        >>> from pypara.currencies import Currencies
+        >>> someprice = Price.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1))
+        >>> someprice.ccy_or(Currencies["EUR"]).code
+        'USD'
+        >>> someprice = Price.of(Currencies["USD"], None, None)
+        >>> someprice.ccy_or(Currencies["EUR"]).code
+        'EUR'
+        """
+
+    @abstractmethod
+    def ccy_or_none(self) -> Optional[Currency]:
+        """
+        Returns the ``ccy`` if the monetary value is *defined*, ``None``
+        otherwise.
+
+        >>> from pypara.currencies import Currencies
+        >>> someprice = Price.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1))
+        >>> someprice.ccy_or_none().code
+        'USD'
+        >>> someprice = Price.of(Currencies["USD"], None, None)
+        >>> someprice.ccy_or_none() is None
+        True
+        """
+
+    @abstractmethod
+    def qty_or(self, default: Decimal) -> Decimal:
+        """
+        Returns the ``qty`` if the monetary value is *defined*, ``default``
+        otherwise.
+
+        >>> from pypara.currencies import Currencies
+        >>> someprice = Price.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1))
+        >>> someprice.qty_or(Decimal(0))
+        Decimal('1')
+        >>> noneprice = Price.of(None, Decimal('1'), None)
+        >>> noneprice.qty_or(Decimal(0))
+        Decimal('0')
+        """
+
+    @abstractmethod
+    def qty_or_zero(self) -> Decimal:
+        """
+        Returns the ``qty`` if the monetary value is *defined*, ``0``
+        otherwise.
+
+        >>> from pypara.currencies import Currencies
+        >>> someprice = Price.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1))
+        >>> someprice.qty_or_zero()
+        Decimal('1')
+        >>> noneprice = Price.of(None, Decimal('1'), None)
+        >>> noneprice.qty_or_zero()
+        Decimal('0')
+        """
+
+    @abstractmethod
+    def qty_or_none(self) -> Optional[Decimal]:
+        """
+        Returns the ``qty`` if the monetary value is *defined*, ``None``
+        otherwise.
+
+        >>> from pypara.currencies import Currencies
+        >>> someprice = Price.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1))
+        >>> someprice.qty_or_none()
+        Decimal('1')
+        >>> noneprice = Price.of(None, Decimal('1'), None)
+        >>> noneprice.qty_or_none() is None
+        True
+        """
+
+    @abstractmethod
+    def qty_or_else(self, e: Callable[[], _T]) -> Union[Decimal, _T]:
+        """
+        Returns the ``qty`` if the monetary value is *defined*, the value of the
+        call of provided combinator otherwise.
+
+        >>> from pypara.currencies import Currencies
+        >>> someprice = Price.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1))
+        >>> someprice.qty_or_else(lambda: Decimal('42'))
+        Decimal('1')
+        >>> someprice.qty_or_else(lambda: True)
+        Decimal('1')
+        >>> noneprice = Price.of(None, Decimal('1'), None)
+        >>> noneprice.qty_or_else(lambda: Decimal('42'))
+        Decimal('42')
+        >>> noneprice.qty_or_else(lambda: False)
+        False
+        """
+
+    @abstractmethod
+    def qty_map(self, f: Callable[[Decimal], _T], e: Callable[[], _T]) -> _T:
+        """
+        Applies the given function to the ``qty`` and returns the result if the
+        monetary value is *defined*, returns the value of the call of provided
+        combinator otherwise.
+
+        >>> from pypara.currencies import Currencies
+        >>> someprice = Price.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1))
+        >>> someprice.qty_map(lambda x: x + Decimal('1'), lambda: Decimal('42'))
+        Decimal('2')
+        >>> noneprice = Price.of(None, Decimal('1'), None)
+        >>> noneprice.qty_map(lambda x: x + Decimal('1'), lambda: Decimal('42'))
+        Decimal('42')
+        """
+
+    @abstractmethod
+    def dov_or(self, default: Date) -> Date:
+        """
+        Returns the ``dov`` if the monetary value is *defined*, ``default``
+        otherwise.
+
+        >>> from pypara.currencies import Currencies
+        >>> someprice = Price.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1))
+        >>> someprice.dov_or(Date(2001, 1, 1))
+        datetime.date(2019, 1, 1)
+        >>> noneprice = Price.of(None, None, Date(2019, 1, 1))
+        >>> noneprice.dov_or(Date(2001, 1, 1))
+        datetime.date(2001, 1, 1)
+        """
+
+    @abstractmethod
+    def dov_or_none(self) -> Optional[Date]:
+        """
+        Returns the ``dov`` if the monetary value is *defined*, ``None``
+        otherwise.
+
+        >>> from pypara.currencies import Currencies
+        >>> someprice = Price.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1))
+        >>> someprice.dov_or_none()
+        datetime.date(2019, 1, 1)
+        >>> noneprice = Price.of(None, None, Date(2019, 1, 1))
+        >>> noneprice.dov_or_none() is None
+        True
+        """
 
     @abstractmethod
     def convert(self, to: Currency, asof: Optional[Date] = None, strict: bool = False) -> "Price":
         """
         Converts the monetary value from one currency to another.
 
-        Raises :class:`FXRateLookupError` if no foreign exchange rate can be found for conversion.
+        Raises :class:`FXRateLookupError` if no foreign exchange rate can be
+        found for conversion.
 
         Note that we will carry the date forward as per ``asof`` date.
         """
-        raise NotImplementedError
 
     @property
     @abstractmethod
     def money(self) -> Money:
         """
         Returns the money representation of the price object.
         """
-        raise NotImplementedError
+
+    @classmethod
+    def na(cls) -> "Price":
+        """
+        Undefined price instance.
+
+        >>> Price.na().defined
+        False
+        >>> Price.na().undefined
+        True
+        """
+        return NoPrice
+
+    @staticmethod
+    def is_none(x: "Price") -> TypeGuard["NonePrice"]:
+        """
+        Type guard for undefined price instances.
+
+        >>> from pypara.currencies import Currencies
+        >>> Price.is_none(Price.na())
+        True
+        >>> Price.is_none(Price.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1)))
+        False
+        """
+        return x.undefined
+
+    @staticmethod
+    def is_some(x: "Price") -> TypeGuard["SomePrice"]:
+        """
+        Type guard for defined price instances.
+
+        >>> from pypara.currencies import Currencies
+        >>> Price.is_some(Price.na())
+        False
+        >>> Price.is_some(Price.of(Currencies["USD"], Decimal('1'), Date(2019, 1, 1)))
+        True
+        """
+        return x.defined
 
     @classmethod
     def of(cls, ccy: Optional[Currency], qty: Optional[Decimal], dov: Optional[Date]) -> "Price":
         """
         Provides a factory method to create a new price object in a safe manner.
         """
         if qty is None or ccy is None or dov is None:
             return NoPrice
         return SomePrice(ccy, qty, dov)
 
     @abstractmethod
     def __bool__(self) -> bool:
-        pass
+        ...
 
     @abstractmethod
     def __eq__(self, other: Any) -> bool:
-        pass
+        ...
 
     @abstractmethod
     def __abs__(self) -> "Price":
-        pass
+        ...
 
     @abstractmethod
     def __float__(self) -> float:
-        pass
+        ...
 
     @abstractmethod
     def __int__(self) -> int:
-        pass
+        ...
 
-    @abstractmethod
-    def __round__(self, ndigits: int = 0) -> "Price":
-        pass
+    @overload
+    def __round__(self) -> int:
+        ...
+
+    @overload
+    def __round__(self, ndigits: None) -> int:
+        ...
+
+    @overload
+    def __round__(self, ndigits: int) -> "Price":
+        ...
+
+    def __round__(self, ndigits: Optional[int] = 0) -> Union["Price", int]:
+        return self.round(ndigits or 0)
 
     @abstractmethod
     def __neg__(self) -> "Price":
-        pass
+        ...
 
     @abstractmethod
     def __pos__(self) -> "Price":
-        pass
+        ...
 
     @abstractmethod
     def __add__(self, other: "Price") -> "Price":
-        pass
+        ...
 
     @abstractmethod
     def __sub__(self, other: "Price") -> "Price":
-        pass
+        ...
 
     @abstractmethod
     def __mul__(self, other: Numeric) -> "Price":
-        pass
+        ...
 
     @abstractmethod
     def __truediv__(self, other: Numeric) -> "Price":
-        pass
+        ...
 
     @abstractmethod
     def __floordiv__(self, other: Numeric) -> "Price":
-        pass
+        ...
 
     @abstractmethod
     def __lt__(self, other: "Price") -> bool:
-        pass
+        ...
 
     @abstractmethod
     def __le__(self, other: "Price") -> bool:
-        pass
+        ...
 
     @abstractmethod
     def __gt__(self, other: "Price") -> bool:
-        pass
+        ...
 
     @abstractmethod
     def __ge__(self, other: "Price") -> bool:
-        pass
+        ...
 
 
-class SomePrice(Price, NamedTuple("SomePrice", [("ccy", Currency), ("qty", Decimal), ("dov", Date)])):  # type: ignore
+class SomePrice(Price, NamedTuple("SomePrice", [("ccy", Currency), ("qty", Decimal), ("dov", Date)])):
     """
     Provides a *defined* price object model.
     """
 
     __slots__ = ()
 
-    defined = True
+    @property
+    def defined(self) -> bool:
+        return True
 
-    undefined = False
+    @property
+    def undefined(self) -> bool:
+        return False
 
     def is_equal(self, other: Any) -> bool:
         return other.__class__ is SomePrice and tuple(self) == tuple(other)
 
     def as_boolean(self) -> bool:
         return self.qty.__bool__()
 
@@ -1094,20 +1676,26 @@
 
     def positive(self) -> "Price":
         c, q, d = self
         return SomePrice(c, q.__pos__(), d)
 
     def round(self, ndigits: int = 0) -> "Price":
         c, q, d = self
-        return SomePrice(c, q.__round__(ndigits), d)  # type: ignore
+        return SomePrice(c, q.__round__(ndigits), d)
 
     def add(self, other: "Price") -> "Price":
         if other.undefined:
             return self
 
+        c1: Currency
+        q1: Decimal
+        d1: Date
+        c2: Currency
+        q2: Decimal
+        d2: Date
         c1, q1, d1 = self
         c2, q2, d2 = other  # type: ignore
 
         if c1 != c2:
             raise IncompatibleCurrencyError(ccy1=c1, ccy2=c2, operation="addition")
 
         return SomePrice(c1, q1 + q2, d1 if d1 > d2 else d2)
@@ -1117,14 +1705,20 @@
         c, q, d = self
         return SomePrice(c, q + Decimal(other), d)
 
     def subtract(self, other: "Price") -> "Price":
         if other.undefined:
             return self
 
+        c1: Currency
+        q1: Decimal
+        d1: Date
+        c2: Currency
+        q2: Decimal
+        d2: Date
         c1, q1, d1 = self
         c2, q2, d2 = other  # type: ignore
 
         if c1 != c2:
             raise IncompatibleCurrencyError(ccy1=c1, ccy2=c2, operation="subtraction")
 
         return SomePrice(c1, q1 - q2, d1 if d1 > d2 else d2)
@@ -1137,69 +1731,105 @@
     def multiply(self, other: Numeric) -> "Price":
         ## TODO: **try** not casting other to Decimal.
         c, q, d = self
         return SomePrice(c, q * Decimal(other), d)
 
     def times(self, other: Numeric) -> "Money":
         c, q, d = self
-        return SomeMoney(c, (q * Decimal(other)).quantize(c[4]), self.dov)
+        return SomeMoney(c, (q * Decimal(other)).quantize(c.quantizer), self.dov)
 
     def divide(self, other: Numeric) -> "Price":
         ## TODO: **try** not casting other to Decimal.
         try:
             c, q, d = self
             return SomePrice(c, q / Decimal(other), d)
-        except (InvalidOperation, DivisionByZero) as ex:
+        except (InvalidOperation, DivisionByZero):
             return NoPrice
 
     def floor_divide(self, other: Numeric) -> "Price":
         ## TODO: **try** not casting other to Decimal.
         try:
             c, q, d = self
             return SomePrice(c, q // Decimal(other), d)
-        except (InvalidOperation, DivisionByZero) as ex:
+        except (InvalidOperation, DivisionByZero):
             return NoPrice
 
     def lt(self, other: "Price") -> bool:
-        if other.undefined:
+        if not isinstance(other, SomePrice):
             return False
         elif self.ccy != other.ccy:
-            raise IncompatibleCurrencyError(ccy1=self.ccy, ccy2=other.ccy, operation="< comparision")
+            raise IncompatibleCurrencyError(ccy1=self.ccy, ccy2=other.ccy, operation="< comparison")
         return self.qty < other.qty
 
     def lte(self, other: "Price") -> bool:
-        if other.undefined:
+        if not isinstance(other, SomePrice):
             return False
         elif self.ccy != other.ccy:
-            raise IncompatibleCurrencyError(ccy1=self.ccy, ccy2=other.ccy, operation="<= comparision")
+            raise IncompatibleCurrencyError(ccy1=self.ccy, ccy2=other.ccy, operation="<= comparison")
         return self.qty <= other.qty
 
     def gt(self, other: "Price") -> bool:
-        if other.undefined:
+        if not isinstance(other, SomePrice):
             return True
         elif self.ccy != other.ccy:
-            raise IncompatibleCurrencyError(ccy1=self.ccy, ccy2=other.ccy, operation="> comparision")
+            raise IncompatibleCurrencyError(ccy1=self.ccy, ccy2=other.ccy, operation="> comparison")
         return self.qty > other.qty
 
     def gte(self, other: "Price") -> bool:
-        if other.undefined:
+        if not isinstance(other, SomePrice):
             return True
         elif self.ccy != other.ccy:
-            raise IncompatibleCurrencyError(ccy1=self.ccy, ccy2=other.ccy, operation=">= comparision")
+            raise IncompatibleCurrencyError(ccy1=self.ccy, ccy2=other.ccy, operation=">= comparison")
         return self.qty >= other.qty
 
+    def or_else(self, e: Callable[[], "Price"]) -> "Price":
+        return self
+
+    def fmap(self, f: Callable[["SomePrice"], "Price"]) -> "Price":
+        return f(self)
+
+    def dimap(self, f: Callable[["SomePrice"], _T], e: Callable[[], _T]) -> _T:
+        return f(self)
+
     def with_ccy(self, ccy: Currency) -> "Price":
         return SomePrice(ccy, self[1], self[2])
 
     def with_qty(self, qty: Decimal) -> "Price":
         return SomePrice(self[0], qty, self[2])
 
     def with_dov(self, dov: Date) -> "Price":
         return SomePrice(self[0], self[1], dov)
 
+    def ccy_or(self, default: Currency) -> Currency:
+        return self[0]
+
+    def ccy_or_none(self) -> Optional[Currency]:
+        return self[0]
+
+    def qty_or(self, default: Decimal) -> Decimal:
+        return self[1]
+
+    def qty_or_zero(self) -> Decimal:
+        return self[1]
+
+    def qty_or_none(self) -> Optional[Decimal]:
+        return self[1]
+
+    def qty_or_else(self, e: Callable[[], _T]) -> Union[Decimal, _T]:
+        return self[1]
+
+    def qty_map(self, f: Callable[[Decimal], _T], e: Callable[[], _T]) -> _T:
+        return f(self[1])
+
+    def dov_or(self, default: Date) -> Date:
+        return self[2]
+
+    def dov_or_none(self) -> Optional[Date]:
+        return self[2]
+
     def convert(self, to: Currency, asof: Optional[Date] = None, strict: bool = False) -> "Price":
         ## Get slots:
         ccy, qty, dov = self
 
         ## Get date of conversion:
         asof = asof or dov
 
@@ -1224,58 +1854,59 @@
 
         ## Compute and return:
         return SomePrice(to, qty * rate.value, asof)
 
     @property
     def money(self) -> Money:
         c, q, d = self
-        return SomeMoney(c, q.quantize(c[4]), d)
+        return SomeMoney(c, q.quantize(c.quantizer), d)
 
     __bool__ = as_boolean
 
     __eq__ = is_equal
 
     __abs__ = abs
 
     __float__ = as_float
 
     __int__ = as_integer
 
-    __round__ = round
-
     __neg__ = negative
 
     __pos__ = positive
 
-    __add__ = add
+    __add__ = add  # type: ignore
 
     __sub__ = subtract
 
-    __mul__ = multiply
+    __mul__ = multiply  # type: ignore
 
     __truediv__ = divide
 
     __floordiv__ = floor_divide
 
-    __lt__ = lt
+    __lt__ = lt  # type: ignore
 
-    __le__ = lte
+    __le__ = lte  # type: ignore
 
-    __gt__ = gt
+    __gt__ = gt  # type: ignore
 
-    __ge__ = gte
+    __ge__ = gte  # type: ignore
 
 
 class NonePrice(Price):
-
     __slots__ = ()
 
-    defined = False
+    @property
+    def defined(self) -> bool:
+        return False
 
-    undefined = True
+    @property
+    def undefined(self) -> bool:
+        return True
 
     def as_boolean(self) -> bool:
         return False
 
     def is_equal(self, other: Any) -> bool:
         return other.__class__ is NonePrice
 
@@ -1329,40 +1960,76 @@
 
     def gt(self, other: "Price") -> bool:
         return False
 
     def gte(self, other: "Price") -> bool:
         return other.undefined
 
+    def or_else(self, e: Callable[[], "Price"]) -> "Price":
+        return e()
+
+    def fmap(self, f: Callable[["SomePrice"], "Price"]) -> "Price":
+        return self
+
+    def dimap(self, f: Callable[["SomePrice"], _T], e: Callable[[], _T]) -> _T:
+        return e()
+
     def with_ccy(self, ccy: Currency) -> "Price":
         return self
 
     def with_qty(self, qty: Decimal) -> "Price":
         return self
 
     def with_dov(self, dov: Date) -> "Price":
         return self
 
+    def ccy_or(self, default: Currency) -> Currency:
+        return default
+
+    def ccy_or_none(self) -> Optional[Currency]:
+        return None
+
+    def qty_or(self, default: Decimal) -> Decimal:
+        return default
+
+    def qty_or_zero(self) -> Decimal:
+        return ZERO
+
+    def qty_or_none(self) -> Optional[Decimal]:
+        return None
+
+    def qty_or_else(self, e: Callable[[], _T]) -> Union[Decimal, _T]:
+        return e()
+
+    def qty_map(self, f: Callable[[Decimal], _T], e: Callable[[], _T]) -> _T:
+        return e()
+
+    def dov_or(self, default: Date) -> Date:
+        return default
+
+    def dov_or_none(self) -> Optional[Date]:
+        return None
+
     def convert(self, to: Currency, asof: Optional[Date] = None, strict: bool = False) -> "Price":
         return self
 
-    money = NoMoney
+    @property
+    def money(self) -> Money:
+        return NoMoney
 
     __bool__ = as_boolean
 
     __eq__ = is_equal
 
     __abs__ = abs
 
     __float__ = as_float
 
     __int__ = as_integer
 
-    __round__ = round
-
     __neg__ = negative
 
     __pos__ = positive
 
     __add__ = add
 
     __sub__ = subtract
@@ -1378,13 +2045,9 @@
     __le__ = lte
 
     __gt__ = gt
 
     __ge__ = gte
 
 
-## Define and attach undefined price singleton.
-Price.NA = NoPrice = NonePrice()
-
-#########################
-# END DEFINITION: Price #
-#########################
+#: Undefined price instance.
+NoPrice = NonePrice()
```

### Comparing `pypara-0.0.9/pypara/exchange.py` & `pypara-0.1.0/pypara/exchange.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,20 @@
+"""
+This module provides definitions and functionality related to foreign-exchange conversions.
+"""
+
+__all__ = ["FXRate", "FXRateLookupError", "FXRateService"]
+
 from abc import ABCMeta, abstractmethod
 from decimal import Decimal
-from typing import Optional, Tuple, Iterable, NamedTuple
+from typing import Iterable, NamedTuple, Optional, Tuple
 
+from .commons.numbers import ONE, ZERO
+from .commons.zeitgeist import Date
 from .currencies import Currency
-from .generic import Date
 
 
 class FXRateLookupError(LookupError):
     """
     Provides an exception indicating that the foreign exchange rate is not found.
     """
 
@@ -24,15 +31,15 @@
         super().__init__(f"Foreign exchange rate for {ccy1}/{ccy2} not found as of {asof}")
 
 
 class FXRate(NamedTuple):
     """
     Defines a foreign exchange (FX) rate model.
 
-    Note that the constructor of this class is not safe: It does not check input. :method:`FXRate.of`, on the
+    Note that the constructor of this class is not safe: It does not check input. :func:`FXRate.of`, on the
     other hand provides a safer way of creating :class:`FXRate` instances.
 
     **Implementation Note:**
 
     I wanted to use an immutable, compact object model with fast creation and property access. Options were
     tweaked plain-vanilla Python class, NamedTuple and dataclasses.
 
@@ -105,19 +112,19 @@
             raise ValueError("CCY/2 must be of type `Currency`.")
         if not isinstance(ccy1, Currency):
             raise ValueError("FX rate value must be of type `Decimal`.")
         if not isinstance(ccy1, Currency):
             raise ValueError("FX rate date must be of type `date`.")
 
         ## Check the value:
-        if value <= 0:
+        if value <= ZERO:
             raise ValueError("FX rate value can not be equal to or less than `zero`.")
 
         ## Check consistency:
-        if ccy1 == ccy2 and value != 1:
+        if ccy1 == ccy2 and value != ONE:
             raise ValueError("FX rate to the same currency must be `one`.")
 
         ## Create and return the FX rate instance:
         return cls(ccy1, ccy2, date, value)
 
 
 class FXRateService(metaclass=ABCMeta):
@@ -128,29 +135,27 @@
     #: Defines the default foreign exchange rate service for the runtime.
     default: Optional["FXRateService"] = None  # noqa: E704
 
     #: Defines an FX rate query tuple.
     TQuery = Tuple[Currency, Currency, Date]
 
     @abstractmethod
-    def query(self, ccy1: Currency, ccy2: Currency, asof: Date, strict: bool=False) -> Optional[FXRate]:
+    def query(self, ccy1: Currency, ccy2: Currency, asof: Date, strict: bool = False) -> Optional[FXRate]:
         """
         Returns the foreign exchange rate of a given currency pair as of a given date.
 
         :param ccy1: The first currency of foreign exchange rate.
         :param ccy2: The second currency of foreign exchange rate.
         :param asof: Temporal dimension the foreign exchange rate is effective as of.
         :param strict: Indicates if we should raise a lookup error if that the foreign exchange rate can not be found.
-        :return: The foreign exhange rate as a :class:`Decimal` instance or None.
+        :return: The foreign exchange rate as a :class:`Decimal` instance or None.
         """
-        pass
 
     @abstractmethod
-    def queries(self, queries: Iterable[TQuery], strict: bool=False) -> Iterable[Optional[FXRate]]:
+    def queries(self, queries: Iterable[TQuery], strict: bool = False) -> Iterable[Optional[FXRate]]:
         """
         Returns foreign exchange rates for a given collection of currency pairs and dates.
 
         :param queries: An iterable of :class:`Currency`, :class:`Currency` and :class:`Temporal` tuples.
         :param strict: Indicates if we should raise a lookup error if that the foreign exchange rate can not be found.
         :return: An iterable of rates.
         """
-        pass
```

### Comparing `pypara-0.0.9/pypara/generic.py` & `pypara-0.1.0/pypara/commons/errors.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,33 @@
-import datetime
-from decimal import Decimal
-from typing import Optional, Union
+"""
+This module provides common error definitions and routines for :py:mod:`pypara`.
+"""
+
+__all__ = ["ProgrammingError"]
+
+from typing import Optional
 
 
 class ProgrammingError(Exception):
     """
     Provides a programming error exception.
 
-    The rationale for this exception is to raise them whenever we rely on metaprogramming and
-    the programmer has introduced a statement which breaks the coherence of the domain logic.
+    The rationale for this exception is to raise them whenever we rely on meta-programming and the programmer has
+    introduced a statement which breaks the coherence of the domain logic.
     """
 
     @classmethod
-    def passert(cls, condition: bool, message: Optional[str]) -> None:
+    def passert(cls, condition: bool, message: Optional[str] = None) -> None:
         """
-        Raises a `ProgrammingError` if the condition is false.
+        Raises a :py:class:`ProgrammingError` if the condition is ``False``.
+
+        :param condition: Indicates if the expectation is fulfilled.
+        :param message: Message of the error to be raised in case that the condition is not met.
+        :raises ProgrammingError: In case that the condition is ``False``.
+
+        >>> ProgrammingError.passert(1 == 0)
+        Traceback (most recent call last):
+        ...
+        pypara.commons.errors.ProgrammingError: Broken coherence. Check your code against domain logic to fix it.
         """
         if not condition:
             raise cls(message or "Broken coherence. Check your code against domain logic to fix it.")
-
-
-def make_quantizer(precision: int) -> Decimal:
-    """
-    Creates a quantifier as per the given precision.
-    """
-    return Decimal(f"0.{''.join(['0' * precision])}")
-
-
-#: Defines a type alias for acceptable numeric values.
-Numeric = Union[Decimal, int, float]
-
-#: Defines an alias for the temporal dimension of :mod:`pypara` implementation.
-Date = datetime.date
-
-#: Defines the maximum precision of the monetary values and operations.
-MaxPrecision: int = 12
-
-#: Defines the maximum precision quantifier.
-MaxPrecisionQuantizer: Decimal = make_quantizer(MaxPrecision)
```

### Comparing `pypara-0.0.9/LICENSE.txt` & `pypara-0.1.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (2017) Vehbi Sinan Tunalioglu
+Copyright (2017-2023) Vehbi Sinan Tunalioglu
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
 
 1. Redistributions of source code must retain the above copyright
 notice, this list of conditions and the following disclaimer.
```

