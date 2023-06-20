# Comparing `tmp/carculator_truck-0.3.9.tar.gz` & `tmp/carculator_truck-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carculator_truck-0.3.9.tar", last modified: Mon May  8 16:35:35 2023, max compression
+gzip compressed data, was "carculator_truck-0.4.0.tar", last modified: Tue Jun 20 08:30:42 2023, max compression
```

## Comparing `carculator_truck-0.3.9.tar` & `carculator_truck-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:35:35.814892 carculator_truck-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-05-08 16:35:35.814892 carculator_truck-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:35:35.810892 carculator_truck-0.3.9/carculator_truck/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/carculator_truck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/carculator_truck/background_systems.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:35:35.814892 carculator_truck-0.3.9/carculator_truck/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1445083 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/carculator_truck/data/default_parameters.json
--rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/carculator_truck/data/extra_parameters.json
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/carculator_truck/data/payloads.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/carculator_truck/driving_cycles.py
--rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/carculator_truck/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    35059 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/carculator_truck/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/carculator_truck/truck_input_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:35:35.810892 carculator_truck-0.3.9/carculator_truck.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-05-08 16:35:35.000000 carculator_truck-0.3.9/carculator_truck.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-08 16:35:35.000000 carculator_truck-0.3.9/carculator_truck.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:35:35.000000 carculator_truck-0.3.9/carculator_truck.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-08 16:35:35.000000 carculator_truck-0.3.9/carculator_truck.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-08 16:35:35.000000 carculator_truck-0.3.9/carculator_truck.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 16:35:35.814892 carculator_truck-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:35:35.814892 carculator_truck-0.3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/tests/test_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-05-08 16:35:27.000000 carculator_truck-0.3.9/tests/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:30:42.258970 carculator_truck-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-20 08:30:32.000000 carculator_truck-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-06-20 08:30:42.258970 carculator_truck-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-06-20 08:30:32.000000 carculator_truck-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:30:42.254970 carculator_truck-0.4.0/carculator_truck/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-20 08:30:32.000000 carculator_truck-0.4.0/carculator_truck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-06-20 08:30:32.000000 carculator_truck-0.4.0/carculator_truck/background_systems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:30:42.258970 carculator_truck-0.4.0/carculator_truck/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1445083 2023-06-20 08:30:32.000000 carculator_truck-0.4.0/carculator_truck/data/default_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-06-20 08:30:32.000000 carculator_truck-0.4.0/carculator_truck/data/extra_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-20 08:30:32.000000 carculator_truck-0.4.0/carculator_truck/data/payloads.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-20 08:30:32.000000 carculator_truck-0.4.0/carculator_truck/driving_cycles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-06-20 08:30:32.000000 carculator_truck-0.4.0/carculator_truck/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35036 2023-06-20 08:30:32.000000 carculator_truck-0.4.0/carculator_truck/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-20 08:30:32.000000 carculator_truck-0.4.0/carculator_truck/truck_input_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:30:42.254970 carculator_truck-0.4.0/carculator_truck.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-06-20 08:30:42.000000 carculator_truck-0.4.0/carculator_truck.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-20 08:30:42.000000 carculator_truck-0.4.0/carculator_truck.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 08:30:42.000000 carculator_truck-0.4.0/carculator_truck.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-20 08:30:42.000000 carculator_truck-0.4.0/carculator_truck.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 08:30:42.000000 carculator_truck-0.4.0/carculator_truck.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 08:30:42.258970 carculator_truck-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-20 08:30:32.000000 carculator_truck-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:30:42.258970 carculator_truck-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-06-20 08:30:32.000000 carculator_truck-0.4.0/tests/test_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-20 08:30:32.000000 carculator_truck-0.4.0/tests/test_model.py
```

### Comparing `carculator_truck-0.3.9/LICENSE` & `carculator_truck-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `carculator_truck-0.3.9/PKG-INFO` & `carculator_truck-0.4.0/carculator_truck.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: carculator_truck
-Version: 0.3.9
+Name: carculator-truck
+Version: 0.4.0
 Summary: Prospective environmental and economic life cycle assessmentof medium and heavy goods vehicles
 Home-page: https://github.com/romainsacchi/carculator_truck
 Author: Romain Sacchi <romain.sacchi@psi.ch>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, Paul Scherrer Institut
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: carculator_truck Version: 0.3.9 Summary:
+Metadata-Version: 2.1 Name: carculator-truck Version: 0.4.0 Summary:
 Prospective environmental and economic life cycle assessmentof medium and heavy
 goods vehicles Home-page: https://github.com/romainsacchi/carculator_truck
 Author: Romain Sacchi
 sacchi@psi.ch> License: BSD 3-Clause License Copyright (c) 2020, Paul Scherrer
 Institut Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: *
 Redistributions of source code must retain the above copyright notice, this
```

### Comparing `carculator_truck-0.3.9/README.md` & `carculator_truck-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `carculator_truck-0.3.9/carculator_truck/__init__.py` & `carculator_truck-0.4.0/carculator_truck/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 
 .. autosummary::
     :toctree: _autosummary
 
 
 """
 
-_all_ = (
+__all__ = (
     "TruckInputParameters",
     "fill_xarray_from_input_parameters",
     "TruckModel",
     "InventoryTruck",
     "get_driving_cycle",
 )
 
 # library version
-__version__ = (0, 3, 9)
+__version__ = (0, 4, 0)
 
 from pathlib import Path
 
 DATA_DIR = Path(__file__).resolve().parent / "data"
 
 from carculator_utils.array import fill_xarray_from_input_parameters
```

### Comparing `carculator_truck-0.3.9/carculator_truck/background_systems.py` & `carculator_truck-0.4.0/carculator_truck/background_systems.py`

 * *Files identical despite different names*

### Comparing `carculator_truck-0.3.9/carculator_truck/data/default_parameters.json` & `carculator_truck-0.4.0/carculator_truck/data/default_parameters.json`

 * *Files identical despite different names*

### Comparing `carculator_truck-0.3.9/carculator_truck/data/extra_parameters.json` & `carculator_truck-0.4.0/carculator_truck/data/extra_parameters.json`

 * *Files identical despite different names*

### Comparing `carculator_truck-0.3.9/carculator_truck/data/payloads.yaml` & `carculator_truck-0.4.0/carculator_truck/data/payloads.yaml`

 * *Files identical despite different names*

### Comparing `carculator_truck-0.3.9/carculator_truck/inventory.py` & `carculator_truck-0.4.0/carculator_truck/inventory.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     """
 
     def fill_in_A_matrix(self):
         """
         Fill-in the A matrix. Does not return anything. Modifies in place.
         Shape of the A matrix (values, products, activities).
 
-        :param array: :attr:`array` from :class:`CarModel` class
+        :attr:`array` from :class:`CarModel` class
         """
 
         # Glider/Frame
         self.A[
             :,
             self.find_input_indices(("frame, blanks and saddle, for lorry",)),
             self.find_input_indices(("Truck, ",)),
```

### Comparing `carculator_truck-0.3.9/carculator_truck/model.py` & `carculator_truck-0.4.0/carculator_truck/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,41 +25,39 @@
 
 class TruckModel(VehicleModel):
 
     """
     This class represents the entirety of the vehicles considered, with useful attributes, such as an array that stores
     all the vehicles parameters.
 
-    :ivar array: multi-dimensional numpy-like array that contains parameters' value(s)
+    :ivar array: multidimensional numpy-like array that contains parameters' value(s)
     :vartype array: xarray.DataArray
     :ivar mappings: Dictionary with names correspondence
     :vartype mappings: dict
     :ivar ecm: instance of :class:`EnergyConsumptionModel` class for a given driving cycle
     :vartype ecm: coarse.energy_consumption.EnergyConsumptionModel
 
     """
 
     def set_all(self, electric_utility_factor: float = None):
         """
         This method runs a series of other methods to obtain the tank-to-wheel energy requirement,
         efficiency of the vehicle, costs, etc.
 
         :meth:`set_component_masses()`, :meth:`set_vehicle_masses()` and :meth:`set_power_parameters()` and
-         :meth:`set_energy_stored_properties` relate to one another.
+        :meth:`set_energy_stored_properties` relate to one another.
         `powertrain_mass` depends on `power`, `curb_mass` is affected by changes in `powertrain_mass`,
-        `combustion engine mass`, `electric engine mass`. `energy battery mass` is influenced
-        by the `curb mass` but also
+        `combustion engine mass`, `electric engine mass`. `energy battery mass` is influencedby the `curb mass` but also
         by the `target range` the truck has. `power` is also varying with `curb_mass`.
 
         The current solution is to loop through the methods until the change in payload between
-        two iterations is
-        inferior to 0.1%. It is then assumed that the trucks are correctly sized.
-
-        :returns: Does not return anything. Modifies ``self.array`` in place.
+        two iterations is inferior to 0.1%. It is then assumed that the trucks are correctly sized.
 
+        :param electric_utility_factor: the share of km driven in battery-depleting mode over the required range autonomy
+        :return: Does not return anything. Modifies ``self.array`` in place.
         """
 
         diff = 1.0
 
         self["is_compliant"] = True
         self["is_available"] = True
 
@@ -103,14 +101,20 @@
             self.set_power_battery_properties()
             self.set_vehicle_masses()
 
             diff = (self["available payload"].sum().values - old_payload) / self[
                 "available payload"
             ].sum()
 
+        self["cargo mass"] = np.clip(self["cargo mass"], 0, self["available payload"])
+
+        self["capacity utilization"] = np.clip(
+            (self["cargo mass"] / self["available payload"]), 0, 1
+        )
+
         self.adjust_cost()
 
         self.set_electric_utility_factor(electric_utility_factor)
         self.set_electricity_consumption()
         self.set_costs()
         self.set_particulates_emission()
         self.set_noise_emissions()
@@ -163,15 +167,14 @@
                     dict(size=s, parameter="kilometers per year")
                 ] = annual_mileage[cycle][s]
 
     def adjust_cost(self):
         """
         This method adjusts costs of energy storage over time, to correct for the overly optimistic linear
         interpolation between years.
-
         """
 
         n_iterations = self.array.shape[-1]
         n_year = len(self.array.year.values)
 
         # If uncertainty is not considered, teh cost factor equals 1.
         # Otherwise, a variability of +/-30% is added.
@@ -269,15 +272,14 @@
             energy_storage.update(self.energy_storage)
 
         self.energy_storage = energy_storage
 
     def override_range(self):
         """
         Set storage size or range for each powertrain.
-        :return:
         """
 
         target_ranges = {
             "Urban delivery": 150,
             "Regional delivery": 400,
             "Long haul": 800,
         }
@@ -312,15 +314,14 @@
 
     def calculate_ttw_energy(self):
         """
         This method calculates the energy required to operate
         auxiliary services as well as to move the vehicle.
         The sum is stored under the parameter label "TtW energy"
         in :attr:`self.array`.
-
         """
 
         self.energy = self.ecm.motive_energy_per_km(
             driving_mass=self["driving mass"],
             rr_coef=self["rolling resistance coefficient"],
             drag_coef=self["aerodynamic drag coefficient"],
             frontal_area=self["frontal area"],
@@ -395,25 +396,24 @@
         self["auxiliary energy"] = (
             self.energy.sel(parameter="auxiliary energy").sum(dim="second").values
             / distance.values
         ).T
 
     def set_battery_fuel_cell_replacements(self):
         """
-        This methods calculates the number of replacement batteries needed
+        These methods calculates the number of replacement batteries needed
         to match the vehicle lifetime. Given the chemistry used,
         the cycle life is known. Given the lifetime kilometers and
         the kilometers per charge, the number of charge cycles can be inferred.
 
         If the battery lifetime surpasses the vehicle lifetime,
         100% of the burden of the battery production is allocated to the vehicle.
         Also, the number of replacement is rounded up.
         This means that the entirety of the battery replacement is allocated
         to the vehicle (and not to its potential second life).
-
         """
         # Number of replacement of battery is rounded *up*
 
         _ = lambda array: np.where(array == 0, 1, array)
 
         self["battery lifetime replacements"] = np.clip(
             (
@@ -454,21 +454,19 @@
             )
         ) * (self["fuel cell lifetime hours"] > 0)
 
     def set_vehicle_masses(self):
         """
         Define ``curb mass``, ``driving mass``, and ``cargo mass``.
 
-            * `curb mass <https://en.wikipedia.org/wiki/Curb_weight>`__ is the mass of the vehicle and fuel, without people or cargo.
-            * ``cargo mass`` is the mass of the cargo and passengers.
-            * ``driving mass`` is the ``curb mass`` plus ``cargo mass``.
-
-        .. note::
-            driving mass = cargo mass + driving mass
+        * `curb mass <https://en.wikipedia.org/wiki/Curb_weight>`__ is the mass of the vehicle and fuel, without people or cargo.
+        * ``cargo mass`` is the mass of the cargo and passengers.
+        * ``driving mass`` is the ``curb mass`` plus ``cargo mass``.
 
+        .. note:: driving mass = cargo mass + driving mass
         """
 
         # Base components, common to all powertrains
         base_components = [
             "glider base mass",
             "suspension mass",
             "braking system mass",
@@ -516,20 +514,14 @@
 
         self["available payload"] = (
             self["gross mass"]
             - self["curb mass"]
             - (self["average passengers"] * self["average passenger mass"])
         )
 
-        self["cargo mass"] = np.clip(self["cargo mass"], 0, self["available payload"])
-
-        self["capacity utilization"] = np.clip(
-            (self["cargo mass"] / self["available payload"]), 0, 1
-        )
-
     def set_component_masses(self):
         self["combustion engine mass"] = (
             self["combustion power"] * self["engine mass per power"]
             + self["engine fixed mass"]
         )
         self["electric engine mass"] = np.clip(
             (24.56 * np.exp(0.0078 * self["electric power"])), 0, 600
@@ -542,19 +534,16 @@
         self["inverter mass"] = (
             self["electric power"] * self["inverter mass per power"]
             + self["inverter fix mass"]
         )
 
     def set_electric_utility_factor(self, uf: float = None) -> None:
         """
-        The electric utility factor
-        is the share of km driven in battery-depleting mode
-        over the required range autonomy.
-        Scania's PHEV tractor can drive 60 km in electric mode
-        :return:
+        The electric utility factor is the share of km driven in battery-depleting mode
+        over the required range autonomy. Scania's PHEV tractor can drive 60 km in electric mode
         """
         if "PHEV-e" in self.array.coords["powertrain"].values:
             range = (
                 self.array.loc[
                     dict(parameter="electric energy stored", powertrain="PHEV-e")
                 ]
                 * self.array.loc[dict(parameter="battery DoD", powertrain="PHEV-e")]
@@ -577,17 +566,15 @@
                 self.array.loc[
                     dict(powertrain="PHEV-e", parameter="electric utility factor")
                 ] = uf
 
     def set_energy_stored_properties(self):
         """
         First, fuel mass is defined. It is dependent on the range required.
-        Then batteries are sized, depending on the range
-        required and the energy consumption.
-        :return:
+        Then batteries are sized, depending on the range required and the energy consumption.
         """
 
         _ = lambda x: np.where(x == 0, 1, x)
         _nz = lambda x: np.where(x < 1, 1, x)
 
         self.set_average_lhv()
 
@@ -844,21 +831,21 @@
             + self["insurance cost"]
             + self["toll cost"]
             + self["amortised component replacement cost"]
         )
 
     def calculate_cost_impacts(self, sensitivity=False, scope=None):
         """
-        This method returns an array with cost values per vehicle-km, sub-divided into the following groups:
+        This method returns an array with cost values per vehicle-km, subdivided into the following groups:
 
-            * Purchase
-            * Maintentance
-            * Component replacement
-            * Energy
-            * Total cost of ownership
+        * Purchase
+        * Maintenance
+        * Component replacement
+        * Energy
+        * Total cost of ownership
 
         :return: A xarray array with cost information per vehicle-km
         :rtype: xarray.core.dataarray.DataArray
         """
 
         if scope is None:
             scope = {
```

### Comparing `carculator_truck-0.3.9/carculator_truck/truck_input_parameters.py` & `carculator_truck-0.4.0/carculator_truck/truck_input_parameters.py`

 * *Files identical despite different names*

### Comparing `carculator_truck-0.3.9/carculator_truck.egg-info/PKG-INFO` & `carculator_truck-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: carculator-truck
-Version: 0.3.9
+Name: carculator_truck
+Version: 0.4.0
 Summary: Prospective environmental and economic life cycle assessmentof medium and heavy goods vehicles
 Home-page: https://github.com/romainsacchi/carculator_truck
 Author: Romain Sacchi <romain.sacchi@psi.ch>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, Paul Scherrer Institut
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: carculator-truck Version: 0.3.9 Summary:
+Metadata-Version: 2.1 Name: carculator_truck Version: 0.4.0 Summary:
 Prospective environmental and economic life cycle assessmentof medium and heavy
 goods vehicles Home-page: https://github.com/romainsacchi/carculator_truck
 Author: Romain Sacchi
 sacchi@psi.ch> License: BSD 3-Clause License Copyright (c) 2020, Paul Scherrer
 Institut Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: *
 Redistributions of source code must retain the above copyright notice, this
```

### Comparing `carculator_truck-0.3.9/carculator_truck.egg-info/SOURCES.txt` & `carculator_truck-0.4.0/carculator_truck.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `carculator_truck-0.3.9/setup.py` & `carculator_truck-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         for filename in filenames:
             paths.append(os.path.join("..", path, filename))
     return paths
 
 
 setup(
     name="carculator_truck",
-    version="0.3.9",
+    version="0.4.0",
     packages=packages,
     author="Romain Sacchi <romain.sacchi@psi.ch>",
     license=open("LICENSE").read(),
     package_data={
         "carculator_truck": package_files(os.path.join("carculator_truck", "data"))
     },
     install_requires=["carculator_utils", "prettytable"],
```

### Comparing `carculator_truck-0.3.9/tests/test_inventory.py` & `carculator_truck-0.4.0/tests/test_inventory.py`

 * *Files identical despite different names*

### Comparing `carculator_truck-0.3.9/tests/test_model.py` & `carculator_truck-0.4.0/tests/test_model.py`

 * *Files identical despite different names*

