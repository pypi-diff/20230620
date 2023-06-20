# Comparing `tmp/tomato-cooker-0.1.0.tar.gz` & `tmp/tomato-cooker-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomato-cooker-0.1.0.tar", last modified: Fri May 12 10:23:14 2023, max compression
+gzip compressed data, was "tomato-cooker-0.2.0.tar", last modified: Tue Jun 20 09:56:32 2023, max compression
```

## Comparing `tomato-cooker-0.1.0.tar` & `tomato-cooker-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:23:14.551118 tomato-cooker-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-12 10:23:14.551118 tomato-cooker-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 10:23:14.555117 tomato-cooker-0.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1555 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:23:14.547118 tomato-cooker-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/tests/test_grill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:23:14.547118 tomato-cooker-0.1.0/tomato_cooker/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/tomato_cooker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:23:14.551118 tomato-cooker-0.1.0/tomato_cooker/grill/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/tomato_cooker/grill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/tomato_cooker/grill/grill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:23:14.551118 tomato-cooker-0.1.0/tomato_cooker/models/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/tomato_cooker/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/tomato_cooker/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:23:14.551118 tomato-cooker-0.1.0/tomato_cooker/models/tomatic/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/tomato_cooker/models/tomatic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/tomato_cooker/models/tomatic/phone_grill.mzn
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/tomato_cooker/models/tomatic/tomatic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:23:14.551118 tomato-cooker-0.1.0/tomato_cooker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-12 10:23:03.000000 tomato-cooker-0.1.0/tomato_cooker/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 10:23:14.551118 tomato-cooker-0.1.0/tomato_cooker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-12 10:23:14.000000 tomato-cooker-0.1.0/tomato_cooker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-12 10:23:14.000000 tomato-cooker-0.1.0/tomato_cooker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:23:14.000000 tomato-cooker-0.1.0/tomato_cooker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-12 10:23:14.000000 tomato-cooker-0.1.0/tomato_cooker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-12 10:23:14.000000 tomato-cooker-0.1.0/tomato_cooker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 10:23:14.000000 tomato-cooker-0.1.0/tomato_cooker.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:56:32.978687 tomato-cooker-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-20 09:56:32.974687 tomato-cooker-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 09:56:32.978687 tomato-cooker-0.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1557 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:56:32.974687 tomato-cooker-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/tests/test_grill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:56:32.974687 tomato-cooker-0.2.0/tomato_cooker/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/tomato_cooker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:56:32.974687 tomato-cooker-0.2.0/tomato_cooker/grill/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/tomato_cooker/grill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/tomato_cooker/grill/grill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:56:32.974687 tomato-cooker-0.2.0/tomato_cooker/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/tomato_cooker/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/tomato_cooker/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:56:32.974687 tomato-cooker-0.2.0/tomato_cooker/models/tomatic/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/tomato_cooker/models/tomatic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/tomato_cooker/models/tomatic/phone_grill.mzn
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/tomato_cooker/models/tomatic/tomatic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:56:32.974687 tomato-cooker-0.2.0/tomato_cooker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-20 09:56:19.000000 tomato-cooker-0.2.0/tomato_cooker/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:56:32.974687 tomato-cooker-0.2.0/tomato_cooker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-20 09:56:32.000000 tomato-cooker-0.2.0/tomato_cooker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-20 09:56:32.000000 tomato-cooker-0.2.0/tomato_cooker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:56:32.000000 tomato-cooker-0.2.0/tomato_cooker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-20 09:56:32.000000 tomato-cooker-0.2.0/tomato_cooker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 09:56:32.000000 tomato-cooker-0.2.0/tomato_cooker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:56:32.000000 tomato-cooker-0.2.0/tomato_cooker.egg-info/zip-safe
```

### Comparing `tomato-cooker-0.1.0/LICENSE` & `tomato-cooker-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tomato-cooker-0.1.0/PKG-INFO` & `tomato-cooker-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomato-cooker
-Version: 0.1.0
+Version: 0.2.0
 Summary: Minizinc problem solver
 Home-page: https://github.com/Som-Energia/Som-Minizinc
 Author: Som Energia SCCL
 Author-email: info@somenergia.coop
 License: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -16,49 +16,52 @@
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: tests
 License-File: LICENSE
 
-# Som-MiniZinc
+# cooked-tomato
 
-### Hackathon held on 11-03-2022 about MiniZinc
+Timetable scheduler for phone attention turns in Som Energia
 
-This problem was previously solved at [https://github.com/Som-Energia/somenergia-tomatic/blob/master/tomatic/backtracker.py](https://github.com/Som-Energia/somenergia-tomatic/blob/master/tomatic/backtracker.py).
-With this library we want to solve the same problem using minizinc language and also open the possibility to extend the resolution of other similar problems.
+## History
+
+This project is the result of an internal Som Energia Hackathon held on 11-03-2022 about MiniZinc
+with the goal of reimplementing the previous solution based on a 
+[pruned backtracking](https://github.com/Som-Energia/somenergia-tomatic/blob/master/tomatic/backtracker.py).
 
 
 ### Prerequisites
 
 Before you begin, ensure you have met the following requirements:
+
 * You must have at least `python 3.8`. You can get this python version through `pyenv`. See more here -> https://github.com/pyenv/pyenv#installation
-* You should have installed `pipenv`. Instructions here -> https://pipenv.readthedocs.io/en/latest/#install-pipenv-today
 * You should have a `Linux/Mac` machine. Windows is not supported and we are not thinking in it.
-* Optionally, an user with sudo permissions
 
 ### Installation
 
 ```bash
-pip install git+https://github.com/Som-Energia/Som-Minizinc.git
+pip install cooked-tomato
 ```
 
-#### Usage
+### Usage
+
 ```python
 import asyncio
 from tomato_cooker.grill import GrillTomatoCooker
 from tomato_cooker.models import TomaticProblem, tomatic
 
 # define a problem
 tomatic_problem_params = {
-    "nPersones": 4,
-    "nLinies": 2,
-    "nSlots": 3,
+    "nPersons": 4,
+    "nLines": 2,
+    "nHours": 3,
     "nNingus": 1,
-    "nDies": 5,
+    "nDays": 5,
     "maxTorns": 2,
     "nTorns": [3, 3, 3, 3,],
     "indisponibilitats": [
         {1}, {1}, {2}, {1}, {1},
         {2}, {2}, {2}, {2}, {2},
         {3}, {3}, {2}, {3}, {3},
         {2}, {3}, {2}, {2}, {1},
@@ -73,29 +76,30 @@
 tomato_cooker = GrillTomatoCooker(tomatic.MODEL_DEFINITION_PATH, solvers)
 
 # Now, we can solve the problem
 solution = asyncio.run(tomato_cooker.cook(tomatic_problem))
 print(solution)
 ```
 
-#### Contribute
+### Contribute
 
 1. Fork the repository on GitHub.
 2. Set up your development setup
 ```bash
-$> pip install -e .
-$> pipenv install --dev
+$> pip install -e .[dev,tests]
 ```
 3. Run the tests to confirm they all pass on your system.
 ```bash
-$> pipenv run pytest
+$> pytest
 ```
 4. Make your change and run the entire test suite again and confirm that all tests pass including the ones you just added.
 5. Create us a GitHub Pull Request to the main repository’s master branch. GitHub Pull Requests are the expected method of code collaboration on this project.
 
-### Changes
+## Changes
+
 [Historic of changes.][changelog]
 
-### License
+## License
+
 This project uses the following license: [GNU AFFERO GENERAL PUBLIC LICENSE](LICENSE).
 
 [changelog]: CHANGELOG.md
```

### Comparing `tomato-cooker-0.1.0/README.md` & `tomato-cooker-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,45 @@
-# Som-MiniZinc
+# cooked-tomato
 
-### Hackathon held on 11-03-2022 about MiniZinc
+Timetable scheduler for phone attention turns in Som Energia
 
-This problem was previously solved at [https://github.com/Som-Energia/somenergia-tomatic/blob/master/tomatic/backtracker.py](https://github.com/Som-Energia/somenergia-tomatic/blob/master/tomatic/backtracker.py).
-With this library we want to solve the same problem using minizinc language and also open the possibility to extend the resolution of other similar problems.
+## History
+
+This project is the result of an internal Som Energia Hackathon held on 11-03-2022 about MiniZinc
+with the goal of reimplementing the previous solution based on a 
+[pruned backtracking](https://github.com/Som-Energia/somenergia-tomatic/blob/master/tomatic/backtracker.py).
 
 
 ### Prerequisites
 
 Before you begin, ensure you have met the following requirements:
+
 * You must have at least `python 3.8`. You can get this python version through `pyenv`. See more here -> https://github.com/pyenv/pyenv#installation
-* You should have installed `pipenv`. Instructions here -> https://pipenv.readthedocs.io/en/latest/#install-pipenv-today
 * You should have a `Linux/Mac` machine. Windows is not supported and we are not thinking in it.
-* Optionally, an user with sudo permissions
 
 ### Installation
 
 ```bash
-pip install git+https://github.com/Som-Energia/Som-Minizinc.git
+pip install cooked-tomato
 ```
 
-#### Usage
+### Usage
+
 ```python
 import asyncio
 from tomato_cooker.grill import GrillTomatoCooker
 from tomato_cooker.models import TomaticProblem, tomatic
 
 # define a problem
 tomatic_problem_params = {
-    "nPersones": 4,
-    "nLinies": 2,
-    "nSlots": 3,
+    "nPersons": 4,
+    "nLines": 2,
+    "nHours": 3,
     "nNingus": 1,
-    "nDies": 5,
+    "nDays": 5,
     "maxTorns": 2,
     "nTorns": [3, 3, 3, 3,],
     "indisponibilitats": [
         {1}, {1}, {2}, {1}, {1},
         {2}, {2}, {2}, {2}, {2},
         {3}, {3}, {2}, {3}, {3},
         {2}, {3}, {2}, {2}, {1},
@@ -51,29 +54,30 @@
 tomato_cooker = GrillTomatoCooker(tomatic.MODEL_DEFINITION_PATH, solvers)
 
 # Now, we can solve the problem
 solution = asyncio.run(tomato_cooker.cook(tomatic_problem))
 print(solution)
 ```
 
-#### Contribute
+### Contribute
 
 1. Fork the repository on GitHub.
 2. Set up your development setup
 ```bash
-$> pip install -e .
-$> pipenv install --dev
+$> pip install -e .[dev,tests]
 ```
 3. Run the tests to confirm they all pass on your system.
 ```bash
-$> pipenv run pytest
+$> pytest
 ```
 4. Make your change and run the entire test suite again and confirm that all tests pass including the ones you just added.
 5. Create us a GitHub Pull Request to the main repository’s master branch. GitHub Pull Requests are the expected method of code collaboration on this project.
 
-### Changes
+## Changes
+
 [Historic of changes.][changelog]
 
-### License
+## License
+
 This project uses the following license: [GNU AFFERO GENERAL PUBLIC LICENSE](LICENSE).
 
 [changelog]: CHANGELOG.md
```

### Comparing `tomato-cooker-0.1.0/setup.py` & `tomato-cooker-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 #!/usr/bin/env python
 from setuptools import find_packages, setup
 
-from tomato_cooker.__init__ import VERSION
+from tomato_cooker import VERSION
 
 readme = open("README.md").read()
 
-required = ["minizinc", "pyyaml"]
+required = [
+    "minizinc",
+    "pyyaml",
+]
 
 extras = {
     "dev": [
         "isort",
         "flake8",
         "black",
         "pre-commit",
```

### Comparing `tomato-cooker-0.1.0/tests/test_grill.py` & `tomato-cooker-0.2.0/tests/test_grill.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,93 +13,134 @@
     solver = GrillTomatoCooker(graellador_path, solvers)
 
     # Then returns a Solver instance
     assert isinstance(solver, GrillTomatoCooker)
 
 
 @pytest.mark.asyncio
-async def test__grid_tomato_cooker__cook(
+async def test__solution__well_formed(
     # given a solver
     tomato_cooker,
     # problem instance
     tomatic_instance,
 ):
     # When we start a new grid execution
     results = await tomato_cooker.cook(tomatic_instance)
 
     # Then a valid phone schedule is generated
-    assert len(results.solution.ocupacioSlot) == tomatic_instance.nDies
+    assert len(results.solution.ocupacioSlot) == tomatic_instance.nDays
     for day in results.solution.ocupacioSlot:
-        assert len(day) == tomatic_instance.nSlots
+        assert len(day) == tomatic_instance.nHours
         for slot in day:
             assert (
-                tomatic_instance.nLinies - tomatic_instance.nNingus
+                tomatic_instance.nLines - tomatic_instance.nNingus
                 <= len(slot)
-                <= tomatic_instance.nLinies
+                <= tomatic_instance.nLines
             )
 
 @pytest.mark.asyncio
-async def test__grid_tomato_cooker__cook__especial_one_day_two_consecutive_slots_same_person(
+async def test__multiple_turns_a_day__must_be_consecutive(
     # given a solver
     tomato_cooker,
     # problem instance
     tomatic_instance_one_day_three_people,
 ):
     # When we start a new grid execution
     results = await tomato_cooker.cook(tomatic_instance_one_day_three_people)
 
     # Then a valid phone schedule is generated
-    assert len(results.solution.ocupacioSlot) == tomatic_instance_one_day_three_people.nDies
+    assert len(results.solution.ocupacioSlot) == tomatic_instance_one_day_three_people.nDays
     for day in results.solution.ocupacioSlot:
-        assert len(day) == tomatic_instance_one_day_three_people.nSlots
+        assert len(day) == tomatic_instance_one_day_three_people.nHours
         for slot in day:
             assert (
-                tomatic_instance_one_day_three_people.nLinies - tomatic_instance_one_day_three_people.nNingus
+                tomatic_instance_one_day_three_people.nLines - tomatic_instance_one_day_three_people.nNingus
                 <= len(slot)
-                <= tomatic_instance_one_day_three_people.nLinies
+                <= tomatic_instance_one_day_three_people.nLines
             )
             assert (
-                1 in results.solution.ocupacioSlot[0][0]
+                'alice' in results.solution.ocupacioSlot[0][0]
             )
             assert (
-                2 in results.solution.ocupacioSlot[0][1] or
-                3 in results.solution.ocupacioSlot[0][1]
+                'bob' in results.solution.ocupacioSlot[0][1] or
+                'carol' in results.solution.ocupacioSlot[0][1]
             )
             assert (
-                2 in results.solution.ocupacioSlot[0][2] or
-                3 in results.solution.ocupacioSlot[0][2]
+                'bob' in results.solution.ocupacioSlot[0][2] or
+                'carol' in results.solution.ocupacioSlot[0][2]
             )
 
 @pytest.mark.asyncio
-async def test__grid_tomato_cooker__indisponibilities(
+async def test__busy_persons__not_in_result(
     # given a solver
     tomato_cooker,
     # problem instance
     tomatic_instance,
 ):
     # When we start a new grid execution
     results = await tomato_cooker.cook(tomatic_instance)
 
     # TODO: Have fun 🦄🌈
     for index, in_this_pony in enumerate(tomatic_instance.indisponibilitats):
-        person = index // tomatic_instance.nDies
-        day = index % tomatic_instance.nDies
+        person = index // tomatic_instance.nDays
+        day = index % tomatic_instance.nDays
         for little_pony in in_this_pony:
             assert person + 1 not in results.solution.ocupacioSlot[day][little_pony - 1]
 
 
 @pytest.mark.asyncio
-async def test__grid_tomato_cooker__preferences(
+async def test__forced_turns__included_in_resut(
     # given a solver
     tomato_cooker,
     # problem instance
-    tomatic_instance_with_preferences,
+    tomatic_instance,
+):
+    day=1
+    hour=4
+    person='C'
+    iperson = tomatic_instance.names.index(person)
+    idx=tomatic_instance.index(person=iperson, day=day)
+    tomatic_instance.forcedTurns[idx].add(hour)
+
+    # When we start a new grid execution
+    results = await tomato_cooker.cook(tomatic_instance)
+    assert person in results.solution.ocupacioSlot[day][hour-1]
+
+@pytest.mark.asyncio
+async def test__forced_turns__ignored_if_busy(
+    # given a solver
+    tomato_cooker,
+    # problem instance
+    tomatic_instance,
 ):
+    person = 'C'
+    day = 3 # dj
+    hour = 4
+    iperson = tomatic_instance.names.index(person)
+    idx=tomatic_instance.index(person=iperson, day=day)
+    tomatic_instance.forcedTurns[idx].add(hour)
+    tomatic_instance.indisponibilitats[idx].add(hour)
     # When we start a new grid execution
-    results = await tomato_cooker.cook(tomatic_instance_with_preferences)
+    results = await tomato_cooker.cook(tomatic_instance)
+
+    assert person not in results.solution.ocupacioSlot[day][hour-1]
+
+@pytest.mark.asyncio
+async def test__forced_turns__reduced_if_person_has_less_load(
+    # given a solver
+    tomato_cooker,
+    # problem instance
+    tomatic_instance_one_day_three_people,
+):
+    tomatic_instance = tomatic_instance_one_day_three_people
+    person = 'alice'
+    day = 0 # dl
+    hours = {1,2}
+    iperson = tomatic_instance.names.index(person)
+    idx=tomatic_instance.index(person=iperson, day=day)
+    tomatic_instance.forcedTurns[idx]=hours # 2 fixed torns
+    tomatic_instance.nTorns[iperson]=1 # load=1
+    tomatic_instance.indisponibilitats[idx]=set() # no indisponibility that day
+    # When we start a new grid execution
+    results = await tomato_cooker.cook(tomatic_instance)
 
-    # TODO: move your body 🕺
-    for index, prefe_dance in enumerate(tomatic_instance_with_preferences.preferencies):
-        person = index // tomatic_instance_with_preferences.nDies
-        day = index % tomatic_instance_with_preferences.nDies
-        for step in prefe_dance:
-            assert person + 1 in results.solution.ocupacioSlot[day][step - 1]
+    assert results.solution.ocupacioPersona[iperson][day].issubset(hours)
```

### Comparing `tomato-cooker-0.1.0/tomato_cooker/grill/grill.py` & `tomato-cooker-0.2.0/tomato_cooker/grill/grill.py`

 * *Files identical despite different names*

### Comparing `tomato-cooker-0.1.0/tomato_cooker/utils/__init__.py` & `tomato-cooker-0.2.0/tomato_cooker/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tomato-cooker-0.1.0/tomato_cooker.egg-info/PKG-INFO` & `tomato-cooker-0.2.0/tomato_cooker.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomato-cooker
-Version: 0.1.0
+Version: 0.2.0
 Summary: Minizinc problem solver
 Home-page: https://github.com/Som-Energia/Som-Minizinc
 Author: Som Energia SCCL
 Author-email: info@somenergia.coop
 License: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -16,49 +16,52 @@
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: tests
 License-File: LICENSE
 
-# Som-MiniZinc
+# cooked-tomato
 
-### Hackathon held on 11-03-2022 about MiniZinc
+Timetable scheduler for phone attention turns in Som Energia
 
-This problem was previously solved at [https://github.com/Som-Energia/somenergia-tomatic/blob/master/tomatic/backtracker.py](https://github.com/Som-Energia/somenergia-tomatic/blob/master/tomatic/backtracker.py).
-With this library we want to solve the same problem using minizinc language and also open the possibility to extend the resolution of other similar problems.
+## History
+
+This project is the result of an internal Som Energia Hackathon held on 11-03-2022 about MiniZinc
+with the goal of reimplementing the previous solution based on a 
+[pruned backtracking](https://github.com/Som-Energia/somenergia-tomatic/blob/master/tomatic/backtracker.py).
 
 
 ### Prerequisites
 
 Before you begin, ensure you have met the following requirements:
+
 * You must have at least `python 3.8`. You can get this python version through `pyenv`. See more here -> https://github.com/pyenv/pyenv#installation
-* You should have installed `pipenv`. Instructions here -> https://pipenv.readthedocs.io/en/latest/#install-pipenv-today
 * You should have a `Linux/Mac` machine. Windows is not supported and we are not thinking in it.
-* Optionally, an user with sudo permissions
 
 ### Installation
 
 ```bash
-pip install git+https://github.com/Som-Energia/Som-Minizinc.git
+pip install cooked-tomato
 ```
 
-#### Usage
+### Usage
+
 ```python
 import asyncio
 from tomato_cooker.grill import GrillTomatoCooker
 from tomato_cooker.models import TomaticProblem, tomatic
 
 # define a problem
 tomatic_problem_params = {
-    "nPersones": 4,
-    "nLinies": 2,
-    "nSlots": 3,
+    "nPersons": 4,
+    "nLines": 2,
+    "nHours": 3,
     "nNingus": 1,
-    "nDies": 5,
+    "nDays": 5,
     "maxTorns": 2,
     "nTorns": [3, 3, 3, 3,],
     "indisponibilitats": [
         {1}, {1}, {2}, {1}, {1},
         {2}, {2}, {2}, {2}, {2},
         {3}, {3}, {2}, {3}, {3},
         {2}, {3}, {2}, {2}, {1},
@@ -73,29 +76,30 @@
 tomato_cooker = GrillTomatoCooker(tomatic.MODEL_DEFINITION_PATH, solvers)
 
 # Now, we can solve the problem
 solution = asyncio.run(tomato_cooker.cook(tomatic_problem))
 print(solution)
 ```
 
-#### Contribute
+### Contribute
 
 1. Fork the repository on GitHub.
 2. Set up your development setup
 ```bash
-$> pip install -e .
-$> pipenv install --dev
+$> pip install -e .[dev,tests]
 ```
 3. Run the tests to confirm they all pass on your system.
 ```bash
-$> pipenv run pytest
+$> pytest
 ```
 4. Make your change and run the entire test suite again and confirm that all tests pass including the ones you just added.
 5. Create us a GitHub Pull Request to the main repository’s master branch. GitHub Pull Requests are the expected method of code collaboration on this project.
 
-### Changes
+## Changes
+
 [Historic of changes.][changelog]
 
-### License
+## License
+
 This project uses the following license: [GNU AFFERO GENERAL PUBLIC LICENSE](LICENSE).
 
 [changelog]: CHANGELOG.md
```

### Comparing `tomato-cooker-0.1.0/tomato_cooker.egg-info/SOURCES.txt` & `tomato-cooker-0.2.0/tomato_cooker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

