# Comparing `tmp/z_units-0.1.0.tar.gz` & `tmp/z_units-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z_units-0.1.0.tar", last modified: Mon May 22 15:24:41 2023, max compression
+gzip compressed data, was "z_units-0.1.1.tar", last modified: Tue Jun 20 15:41:23 2023, max compression
```

## Comparing `z_units-0.1.0.tar` & `z_units-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,20 @@
--rw-r--r--   0        0        0     1067 2023-05-17 13:45:43.661931 z_units-0.1.0/LICENSE
--rw-r--r--   0        0        0      350 2023-05-22 14:19:24.345214 z_units-0.1.0/README.md
--rw-r--r--   0        0        0      417 2023-05-22 15:24:41.911885 z_units-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       39 2023-05-18 13:31:12.554551 z_units-0.1.0/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-05-18 13:31:12.554551 z_units-0.1.0/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2023-05-18 13:31:12.554551 z_units-0.1.0/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0     1309 2023-05-18 13:31:25.444673 z_units-0.1.0/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-05-18 13:31:25.444673 z_units-0.1.0/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2022-10-05 15:38:26.023471 z_units-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0    18595 2023-05-18 13:45:37.916016 z_units-0.1.0/tests/test_quantity.py
--rw-r--r--   0        0        0        0 2023-05-17 13:33:52.991704 z_units-0.1.0/z_units/__init__.py
--rw-r--r--   0        0        0     4969 2023-05-17 14:40:42.035615 z_units-0.1.0/z_units/quantity.py
--rw-r--r--   0        0        0    19989 2023-05-17 14:37:33.585421 z_units-0.1.0/z_units/unit.py
--rw-r--r--   0        0        0     9232 2022-10-05 15:38:47.112694 z_units-0.1.0/z_units/unit_registry.py
--rw-r--r--   0        0        0      992 2023-05-17 14:37:33.596422 z_units-0.1.0/z_units/util.py
--rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 z_units-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-17 13:45:43.661931 z_units-0.1.1/LICENSE
+-rw-r--r--   0        0        0      739 2023-06-20 15:09:52.178275 z_units-0.1.1/README.md
+-rw-r--r--   0        0        0      482 2023-06-20 15:41:23.750115 z_units-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-05-18 13:31:12.554551 z_units-0.1.1/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2023-05-18 13:31:12.554551 z_units-0.1.1/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2023-05-18 13:31:12.554551 z_units-0.1.1/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2023-06-13 15:10:39.946194 z_units-0.1.1/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     1339 2023-06-20 15:32:51.630557 z_units-0.1.1/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2023-06-20 15:32:51.630557 z_units-0.1.1/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2022-10-05 15:38:26.023471 z_units-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0    18855 2023-05-27 13:51:23.872491 z_units-0.1.1/tests/test_quantity.py
+-rw-r--r--   0        0        0      369 2023-06-14 16:10:41.774469 z_units-0.1.1/tests/test_unit.py
+-rw-r--r--   0        0        0       66 2023-06-20 15:09:52.184275 z_units-0.1.1/z_units/__init__.py
+-rw-r--r--   0        0        0     1099 2023-06-20 15:09:52.182275 z_units-0.1.1/z_units/config.py
+-rw-r--r--   0        0        0       93 2023-05-27 13:51:23.872491 z_units-0.1.1/z_units/constant.py
+-rw-r--r--   0        0        0     4785 2023-05-30 13:53:30.266379 z_units-0.1.1/z_units/quantity.py
+-rw-r--r--   0        0        0    21352 2023-06-14 16:13:18.996833 z_units-0.1.1/z_units/unit.py
+-rw-r--r--   0        0        0     9232 2023-06-02 15:07:02.749962 z_units-0.1.1/z_units/unit_registry.py
+-rw-r--r--   0        0        0      992 2023-05-17 14:37:33.596422 z_units-0.1.1/z_units/util.py
+-rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 z_units-0.1.1/PKG-INFO
```

### Comparing `z_units-0.1.0/LICENSE` & `z_units-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `z_units-0.1.0/tests/.pytest_cache/v/cache/nodeids` & `z_units-0.1.1/tests/.pytest_cache/v/cache/nodeids`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9696969696969697%*

 * *Differences: {'insert': "[(32, 'test_unit.py::test_unit')]"}*

```diff
@@ -26,9 +26,10 @@
     "test_quantity.py::test_surface_tension",
     "test_quantity.py::test_temperature",
     "test_quantity.py::test_thermal_conductivity",
     "test_quantity.py::test_time",
     "test_quantity.py::test_velocity",
     "test_quantity.py::test_viscosity",
     "test_quantity.py::test_volume",
-    "test_quantity.py::test_volume_flow"
+    "test_quantity.py::test_volume_flow",
+    "test_unit.py::test_unit"
 ]
```

### Comparing `z_units-0.1.0/tests/test_quantity.py` & `z_units-0.1.1/tests/test_quantity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from math import isclose
 
 from z_units import quantity as q
+from z_units.config import set_local_atmospheric_pressure, set_standard_temperature
 
 
 def test_length():
     x = q.Length(1)
     assert x.unit.symbol == 'm'
     assert x.unit == x.base_unit
     assert isclose(x.to('km').value, 1e-3, rel_tol=1e-4)
@@ -81,14 +82,16 @@
     assert x.unit == x.base_unit
     assert isclose(x.to('mol').value, 1e3, rel_tol=1e-4)
     assert isclose(x.to('Nm3').value, 22.414, rel_tol=1e-4)
     assert isclose(x.to('Sm3').value, 24.055149, rel_tol=1e-4)
     assert isclose(x.to('SCF').value, 836.56108, rel_tol=1e-4)
     assert isclose(x.to('MSCF').value, 836.56108e-3, rel_tol=1e-4)
     assert isclose(x.to('MMSCF').value, 836.56108e-6, rel_tol=1e-4)
+    set_standard_temperature(0)
+    assert isclose(x.to('Sm3').value, x.to('Nm3').value)
 
 
 def test_energy():
     x = q.Energy(1)
     assert x.unit.symbol == 'kJ'
     assert x.unit == x.base_unit
     assert isclose(x.to('J').value, 1e3, rel_tol=1e-4)
@@ -165,14 +168,16 @@
     assert isclose(x.to('psig').value, -0.19218, rel_tol=1e-4)
     assert isclose(x.to('lbf/ft2_g').value, -27.673, rel_tol=1e-4)
     assert isclose(x.to('torr_g').value, -9.9385, rel_tol=1e-4)
     assert isclose(x.to('mmHg_0C_g').value, -9.9385, rel_tol=1e-4)
     assert isclose(x.to('inHg_32F_g').value, -0.39127, rel_tol=1e-4)
     assert isclose(x.to('inHg_60F_g').value, -0.39237, rel_tol=1e-4)
     assert isclose(q.Pressure(1, 'MPag').to('psi').value, 159.73368651, rel_tol=1e-4)
+    set_local_atmospheric_pressure(50)
+    assert isclose(x.to('kPag').value, 50)
 
 
 def test_volume_flow():
     v = q.VolumeFlow(1)
     assert v.unit.symbol == 'm3/s'
     assert v.base_unit.symbol == v.unit.symbol
     assert isclose(v.to('m3/h').value, 3600, rel_tol=1e-6)
```

### Comparing `z_units-0.1.0/z_units/quantity.py` & `z_units-0.1.1/z_units/quantity.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,20 +22,14 @@
     def to(self, unit_symbol: str):
         if self.value is None:
             return None
         ref_value = self._unit.to_base_unit(self.value)
         value = self.unit_registry.get_unit(unit_symbol).from_base_unit(ref_value)
         return self.__class__(value, unit_symbol)
 
-    # def to_base(self):
-    #     if self.value is None:
-    #         return None
-    #     value = self._unit.to_base_unit(self.value)
-    #     return self.__class__(value)
-
     @property
     def unit_registry(self) -> UnitRegistry:
         return self.get_unit_registry()
 
     def get_unit_registry(self):
         return UnitRegistry(reg.dimensionless)
```

### Comparing `z_units-0.1.0/z_units/unit.py` & `z_units-0.1.1/z_units/unit.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,60 @@
+import numbers
 import re
+from typing import Union, Callable
 
-# 1 atmosphere (kPa)
+from .config import get_local_atmospheric_pressure, get_standard_temperature
 from .util import multi_replace
-
-ATM = 101.325
-# gravitational acceleration: in m/s**2
-G = 9.80665
-
-
-def format_symbol_short(symbol: str) -> str:
-    if symbol:
-        return multi_replace(symbol, {
-            '**': '',
-            '*': '-',
-            '(': '',
-            ')': '',
-        })
-
-    return symbol
-
-
-def format_symbol_defined(symbol: str) -> str:
-    if symbol:
-        return re.sub(r'(\*{2}|\*|/)', r' \g<0> ', symbol)
-
-    return symbol
+from . import constant
 
 
 class Unit:
     """
-    A class used to represent a Unit.
+    Class used to represent a Unit.
 
     For unit conversion, units belong to same 'family' (unit set)
     shall be converted from/to one 'base unit' as reference.
-    Creation: unit = Unit(name[, factor])
+
+    Creation: unit = Unit(name[, factor, offset])
+
     name: str
-        the hysys-style name(symbol) of the unit,
+        the quick style name(symbol) of the unit,
         example: 'kg/s', 'm3/s', 'kJ/mol-C'
-        Simple form used to represent definition, as bellow:
+
+        Simple form used to represent definition, as:
         'm3' = 'm**3', 'mol-C' = 'mol*C'
-    factor: numeric valve
-        conversion factor for converting this unit to base unit,
-        unit * factor = base unit
+
+    factor, offset: numeric value or function,
+        for converting this unit to base unit.
+
+        unit * factor + offset = base unit
+
     If unit conversion is nonlinear, to_base_unit() & from_base_unit()
-    have to be overridden
+    have to be overridden.
+
     Example: kilometer = Unit('km', factor=1e3)
-    meter is base unit
 
-    Attributes
+    Which meter is base unit
+
+    Property
     ----------
     symbol: str
-        the hysys-style name(symbol) of the unit.
+        the quick style name(symbol) of the unit.
+
+    factor: float
+        factor value
+
+    offset: float
+        offset value
     """
 
-    def __init__(self, symbol: str, factor: float = 1, offset: float = 0):
+    def __init__(self, symbol: str, factor: Union[float, Callable] = 1, offset: Union[float, Callable] = 0):
         self._symbol = symbol.replace(' ', '')
-        self.factor = factor
-        self.offset = offset
+        self._factor = factor
+        self._offset = offset
 
     def to_base_unit(self, value: float):
         """
         Convert value from this unit to base unit
         :param value: numerical value
         :return: converted value
         """
@@ -71,33 +65,81 @@
         Convert value from base unit to this unit
         :param value: numerical valve
         :return: converted valve
         """
         return (value - self.offset) / self.factor
 
     @property
-    def symbol_short(self):
+    def quick_style(self):
         """
-        Used for indexing
-        :return:
+        The default style, used for indexing
+
+        Quick Style Convention:
+
+        * No space separator
+        * Power:    x ** y -> xy
+        * Multiply: x * y  -> x-y
+        * Parentheses will be omitted:  x / (y * z) -> x/y-z
+
+        Examples:
+
+            m ** 2 -> m2
+            m * s -> m-s
+            kJ / (C * kg) -> kJ/C-kg
+
+        :return: quick style symbol in str
         """
-        return format_symbol_short(self._symbol)
+        if self._symbol:
+            return multi_replace(self._symbol, {
+                '**': '',
+                '*': '-',
+                '(': '',
+                ')': '',
+            })
+
+        return self._symbol
 
     @property
-    def symbol_defined(self):
-        return format_symbol_defined(self._symbol)
+    def defined_style(self):
+        """
+        Defined Style shows formula
+        :return: defined style symbol in str
+        """
+        if self._symbol:
+            return re.sub(r'(\*{2}|\*|/)', r' \g<0> ', self._symbol)
+
+        return self._symbol
 
     @property
     def symbol(self):
-        return self.symbol_short
+        return self.quick_style
+
+    @property
+    def factor(self):
+        if callable(self._factor):
+            return self._factor()
+
+        return self._factor
+
+    @property
+    def offset(self):
+        if callable(self._offset):
+            return self._offset()
+
+        return self._offset
 
     def __repr__(self):
-        return f"<Unit('{self.symbol}')>"
+        return f"<Unit('{self}')>"
+
+    def __format__(self, format_spec=''):
+        if format_spec.startswith('q'):
+            return self.quick_style
+        if format_spec.startswith('d'):
+            return self.defined_style
 
-    def __str__(self):
         return self.symbol
 
 
 class BaseUnit(Unit):
     """
     A class used to represent Base Unit.
 
@@ -176,24 +218,25 @@
 pound = Unit('lb', factor=0.45359237)
 
 # force, N
 newton = BaseUnit('N')
 kilogram_meter_per_second_squared = Unit('kg*m/s**2', factor=1)
 kilo_newton = Unit('kN', factor=1e3)
 dyne = Unit('dyn', factor=1e-5)
-kilogram_force = Unit('kgf', factor=G)
-tonne_force = Unit('tonf', factor=tonne.factor * G)
-pound_force = Unit('lbf', factor=pound.factor * G)
+kilogram_force = Unit('kgf', factor=constant.G)
+tonne_force = Unit('tonf', factor=tonne.factor * constant.G)
+pound_force = Unit('lbf', factor=pound.factor * constant.G)
 
 # substance, kmol
 kilomole = BaseUnit('kmol')
 mole = Unit('mol', factor=1e-3)
 normal_cubic_meter = Unit('Nm**3', factor=1 / 22.414)
 # @20 degC
-standard_cubic_meter = Unit('Sm**3', factor=normal_cubic_meter.factor * 273.15 / (273.15 + 20))
+standard_cubic_meter = Unit('Sm**3',
+                            factor=lambda: normal_cubic_meter.factor * 273.15 / (273.15 + get_standard_temperature()))
 # scf is @60 degF, so some math need to be done
 T_60F_inK = kelvin.from_base_unit(fahrenheit.to_base_unit(60))
 T_0C_inK = kelvin.from_base_unit(0)
 standard_cubic_foot = Unit('SCF', factor=normal_cubic_meter.factor * cubic_foot.factor * T_0C_inK / T_60F_inK)
 kilo_standard_cubic_foot = Unit('MSCF', factor=1e3 * standard_cubic_foot.factor)
 million_standard_cubic_foot = Unit('MMSCF', factor=1e6 * standard_cubic_foot.factor)
 
@@ -207,49 +250,50 @@
 calorie = Unit('cal', factor=4.184e-3)
 kilocalorie = Unit('kcal', factor=1e3 * calorie.factor)
 megacalorie = Unit('Mcal', factor=1e6 * calorie.factor)
 gigacalorie = Unit('Gcal', factor=1e9 * calorie.factor)
 million_kilocalorie = Unit('MMkcal', factor=1e6 * kilocalorie.factor)
 british_thermal_unit = Unit('Btu', factor=1.055056)
 million_british_thermal_unit = Unit('MMBtu', factor=1e6 * british_thermal_unit.factor)
-# pound_force_foot = Unit('lbf*ft', factor=1.355818e-3)
 pound_force_foot = Unit('lbf*ft', factor=1e-3 * pound_force.factor * foot.factor)
 
 # delta temperature
 delta_celsius = BaseUnit('C')
 delta_kelvin = Unit('K', factor=1)
 delta_rankine = Unit('R', factor=5 / 9)
 delta_fahrenheit = Unit('F', factor=5 / 9)
 
 # pressure base unit
 kilopascal = BaseUnit('kPa')
 megapascal = Unit('MPa', factor=1e3)
 bar = Unit('bar', factor=1e2)
 millibar = Unit('mbar', factor=0.1)
 pascal = Unit('Pa', factor=1e-3)
-atm = Unit('atm', factor=ATM)
+atm = Unit('atm', factor=constant.ATM)
 kg_force_per_square_centimeter = Unit('kgf/cm**2', factor=1e-3 * kilogram_force.factor / square_centimeter.factor)
 # psi = Unit('psi', factor=6.894757)
 psi = Unit('psi', factor=1e-3 * pound_force.factor / square_inch.factor)
 pound_force_per_square_foot = Unit('lbf/ft**2', factor=1e-3 * pound_force.factor / square_foot.factor)
 torr = Unit('torr', factor=101.325 / 760)
 mm_Hg = Unit('mmHg_0C', factor=torr.factor)
 inch_Hg = Unit('inHg_32F', factor=3.386389)
 inch_Hg_60F = Unit('inHg_60F', factor=3.37685)
-kilopascal_gauge = Unit('kPag', offset=ATM)
-megapascal_gauge = Unit('MPag', factor=megapascal.factor, offset=ATM)
-bar_gauge = Unit('barg', factor=bar.factor, offset=ATM)
-millibar_gauge = Unit('mbarg', factor=millibar.factor, offset=ATM)
-kg_force_per_square_centimeter_gauge = Unit('kgf/cm**2_g', factor=kg_force_per_square_centimeter.factor, offset=ATM)
-psi_gauge = Unit('psig', factor=psi.factor, offset=ATM)
-pound_force_per_square_foot_gauge = Unit('lbf/ft**2_g', factor=pound_force_per_square_foot.factor, offset=ATM)
-torr_gauge = Unit('torr_g', factor=torr.factor, offset=ATM)
-mm_Hg_gauge = Unit('mmHg_0C_g', factor=mm_Hg.factor, offset=ATM)
-inch_Hg_gauge = Unit('inHg_32F_g', factor=inch_Hg.factor, offset=ATM)
-inch_Hg_60F_gauge = Unit('inHg_60F_g', factor=inch_Hg_60F.factor, offset=ATM)
+kilopascal_gauge = Unit('kPag', offset=get_local_atmospheric_pressure)
+megapascal_gauge = Unit('MPag', factor=megapascal.factor, offset=get_local_atmospheric_pressure)
+bar_gauge = Unit('barg', factor=bar.factor, offset=get_local_atmospheric_pressure)
+millibar_gauge = Unit('mbarg', factor=millibar.factor, offset=get_local_atmospheric_pressure)
+kg_force_per_square_centimeter_gauge = Unit('kgf/cm**2_g', factor=kg_force_per_square_centimeter.factor,
+                                            offset=get_local_atmospheric_pressure)
+psi_gauge = Unit('psig', factor=psi.factor, offset=get_local_atmospheric_pressure)
+pound_force_per_square_foot_gauge = Unit('lbf/ft**2_g', factor=pound_force_per_square_foot.factor,
+                                         offset=get_local_atmospheric_pressure)
+torr_gauge = Unit('torr_g', factor=torr.factor, offset=get_local_atmospheric_pressure)
+mm_Hg_gauge = Unit('mmHg_0C_g', factor=mm_Hg.factor, offset=get_local_atmospheric_pressure)
+inch_Hg_gauge = Unit('inHg_32F_g', factor=inch_Hg.factor, offset=get_local_atmospheric_pressure)
+inch_Hg_60F_gauge = Unit('inHg_60F_g', factor=inch_Hg_60F.factor, offset=get_local_atmospheric_pressure)
 
 # molar flow, base: kmol/s
 kilomole_per_second = BaseUnit('kmol/s')
 kilomole_per_hour = Unit('kmol/h', factor=1 / hour.factor)
 kilomole_per_minute = Unit('kmol/min', factor=1 / minute.factor)
 normal_cubic_meter_per_hour = Unit('Nm**3/h', factor=normal_cubic_meter.factor / hour.factor)
 normal_cubic_meter_per_day = Unit('Nm**3/d', factor=normal_cubic_meter.factor / day.factor)
@@ -343,19 +387,18 @@
 calorie_per_mole_celsius = Unit('cal/(mol*C)', factor=calorie.factor / mole.factor)
 calorie_per_mole_kelvin = Unit('cal/(mol*K)', factor=calorie.factor / mole.factor)
 calorie_per_kilomole_celsius = Unit('cal/(kmol*C)', factor=calorie.factor / kilomole.factor)
 calorie_per_kilomole_kelvin = Unit('cal/(kmol*K)', factor=calorie.factor / kilomole.factor)
 
 # thermal conductivity, W/m-K
 watt_per_meter_kelvin = BaseUnit('W/(m*K)')
-# Btu_per_hour_foot_fahrenheit = Unit('Btu/(h*ft*F)', factor=1.730735)
 Btu_per_hour_foot_fahrenheit = Unit('Btu/(h*ft*F)', factor=1e3 * british_thermal_unit.factor / (
             hour.factor * foot.factor * delta_fahrenheit.factor))
-kilocalorie_per_meter_hour_celsuis = Unit('kcal/(m*h*C)', factor=1e3 * kilocalorie.factor / hour.factor)
-calorie_per_centimeter_second_celsuis = Unit('cal/(cm*s*C)', factor=1e3 * calorie.factor / centimeter.factor)
+kilocalorie_per_meter_hour_celsius = Unit('kcal/(m*h*C)', factor=1e3 * kilocalorie.factor / hour.factor)
+calorie_per_centimeter_second_celsius = Unit('cal/(cm*s*C)', factor=1e3 * calorie.factor / centimeter.factor)
 
 # viscosity, cP
 centipoise = BaseUnit('cP')
 millipoise = Unit('mP', factor=0.1)
 micropoise = Unit('microP', factor=1e-3 * millipoise.factor)
 poise = Unit('P', factor=100)
 pascal_second = Unit('Pa-s', factor=1000)
@@ -365,29 +408,29 @@
 
 # surface tension, dyne/cm
 dyne_per_centimeter = BaseUnit('dyne/cm')
 dyn_per_centimeter = Unit('dyn/cm', factor=1)
 pound_force_per_foot = Unit('lbf/ft', factor=1e3 * pound_force.factor / foot.factor)
 
 # mass capacity, kJ/kg-C
-kilojoule_per_gram_celsuis = Unit('kJ/(g*C)', factor=kilojoule.factor / gram.factor)
+kilojoule_per_gram_celsius = Unit('kJ/(g*C)', factor=kilojoule.factor / gram.factor)
 kilojoule_per_gram_kelvin = Unit('kJ/(g*K)', factor=kilojoule.factor / gram.factor)
-kilojoule_per_kilogram_celsuis = BaseUnit('kJ/(kg*C)')
+kilojoule_per_kilogram_celsius = BaseUnit('kJ/(kg*C)')
 kilojoule_per_kilogram_kelvin = Unit('kJ/(kg*K)', factor=1)
-joule_per_gram_celsuis = Unit('J/(g*C)', factor=1)
+joule_per_gram_celsius = Unit('J/(g*C)', factor=1)
 joule_per_gram_kelvin = Unit('J/(g*K)', factor=1)
-joule_per_kilogram_celsuis = Unit('J/(kg*C)', factor=joule.factor / kilogram.factor)
+joule_per_kilogram_celsius = Unit('J/(kg*C)', factor=joule.factor / kilogram.factor)
 joule_per_kilogram_kelvin = Unit('J/(kg*K)', factor=joule.factor / kilogram.factor)
-kilocalorie_per_gram_celsuis = Unit('kcal/(g*C)', factor=kilocalorie.factor / gram.factor)
+kilocalorie_per_gram_celsius = Unit('kcal/(g*C)', factor=kilocalorie.factor / gram.factor)
 kilocalorie_per_gram_kelvin = Unit('kcal/(g*K)', factor=kilocalorie.factor / gram.factor)
-kilocalorie_per_kilogram_celsuis = Unit('kcal/(kg*C)', factor=kilocalorie.factor / kilogram.factor)
+kilocalorie_per_kilogram_celsius = Unit('kcal/(kg*C)', factor=kilocalorie.factor / kilogram.factor)
 kilocalorie_per_kilogram_kelvin = Unit('kcal/(kg*K)', factor=kilocalorie.factor / kilogram.factor)
-calorie_per_gram_celsuis = Unit('cal/(g*C)', factor=calorie.factor / gram.factor)
+calorie_per_gram_celsius = Unit('cal/(g*C)', factor=calorie.factor / gram.factor)
 calorie_per_gram_kelvin = Unit('cal/(g*K)', factor=calorie.factor / gram.factor)
-calorie_per_kilogram_celsuis = Unit('cal/(kg*C)', factor=calorie.factor / kilogram.factor)
+calorie_per_kilogram_celsius = Unit('cal/(kg*C)', factor=calorie.factor / kilogram.factor)
 calorie_per_kilogram_kelvin = Unit('cal/(kg*K)', factor=calorie.factor / kilogram.factor)
 
 # mass density, kg/m3
 kilogram_per_cubic_meter = BaseUnit('kg/m**3')
 gram_per_liter = Unit('g/L', factor=gram.factor / liter.factor)
 gram_per_cubic_centimeter = Unit('g/cm**3', factor=gram.factor / cubic_centimeter.factor)
 gram_per_milliliter = Unit('g/mL', factor=gram.factor / milliliter.factor)
```

### Comparing `z_units-0.1.0/z_units/unit_registry.py` & `z_units-0.1.1/z_units/unit_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,16 +284,16 @@
 ])
 
 molar_entropy = molar_heat_capacity
 
 thermal_conductivity = UnitRegistry([
     u.watt_per_meter_kelvin,
     u.Btu_per_hour_foot_fahrenheit,
-    u.kilocalorie_per_meter_hour_celsuis,
-    u.calorie_per_centimeter_second_celsuis
+    u.kilocalorie_per_meter_hour_celsius,
+    u.calorie_per_centimeter_second_celsius
 ])
 
 viscosity = UnitRegistry([
     u.centipoise,
     u.millipoise,
     u.micropoise,
     u.poise,
@@ -306,29 +306,29 @@
 surface_tension = UnitRegistry([
     u.dyne_per_centimeter,
     u.dyn_per_centimeter,
     u.pound_force_per_foot
 ])
 
 mass_heat_capacity = UnitRegistry([
-    u.kilojoule_per_gram_celsuis,
+    u.kilojoule_per_gram_celsius,
     u.kilojoule_per_gram_kelvin,
-    u.kilojoule_per_kilogram_celsuis,
+    u.kilojoule_per_kilogram_celsius,
     u.kilojoule_per_kilogram_kelvin,
-    u.joule_per_gram_celsuis,
+    u.joule_per_gram_celsius,
     u.joule_per_gram_kelvin,
-    u.joule_per_kilogram_celsuis,
+    u.joule_per_kilogram_celsius,
     u.joule_per_kilogram_kelvin,
-    u.kilocalorie_per_gram_celsuis,
+    u.kilocalorie_per_gram_celsius,
     u.kilocalorie_per_gram_kelvin,
-    u.kilocalorie_per_kilogram_celsuis,
+    u.kilocalorie_per_kilogram_celsius,
     u.kilocalorie_per_kilogram_kelvin,
-    u.calorie_per_gram_celsuis,
+    u.calorie_per_gram_celsius,
     u.calorie_per_gram_kelvin,
-    u.calorie_per_kilogram_celsuis,
+    u.calorie_per_kilogram_celsius,
     u.calorie_per_kilogram_kelvin
 ])
 
 mass_density = UnitRegistry([
     u.kilogram_per_cubic_meter,
     u.gram_per_liter,
     u.gram_per_cubic_centimeter,
```

### Comparing `z_units-0.1.0/z_units/util.py` & `z_units-0.1.1/z_units/util.py`

 * *Files identical despite different names*

