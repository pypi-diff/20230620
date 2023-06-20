# Comparing `tmp/autora-experiment-runner-recruitment-manager-prolific-1.0.0a4.tar.gz` & `tmp/autora-experiment-runner-recruitment-manager-prolific-1.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-experiment-runner-recruitment-manager-prolific-1.0.0a4.tar", last modified: Mon Jun 12 21:42:41 2023, max compression
+gzip compressed data, was "autora-experiment-runner-recruitment-manager-prolific-1.0.0a5.tar", last modified: Tue Jun 20 12:28:23 2023, max compression
```

## Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a4.tar` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:42:41.303547 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:42:41.299547 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:42:41.299547 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-12 21:42:26.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-12 21:42:26.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-12 21:42:26.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-12 21:42:41.303547 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-12 21:42:26.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:42:41.299547 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-06-12 21:42:26.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-12 21:42:26.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:42:41.299547 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-12 21:42:26.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-12 21:42:26.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:42:41.299547 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-12 21:42:26.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-12 21:42:26.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-12 21:42:26.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 21:42:41.303547 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:42:41.299547 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:42:41.299547 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:42:41.299547 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/src/autora/experiment_runner/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:42:41.299547 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/src/autora/experiment_runner/recruitment_manager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:42:41.299547 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/src/autora/experiment_runner/recruitment_manager/prolific/
--rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-06-12 21:42:26.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:42:41.303547 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-12 21:42:41.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-12 21:42:41.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:42:41.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-12 21:42:41.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-12 21:42:41.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:42:41.303547 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-12 21:42:26.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:42:26.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-12 21:42:26.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/tests/test_recruitment_manager_prolific.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:28:23.979215 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:28:23.975215 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:28:23.975215 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-20 12:28:11.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-20 12:28:11.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-20 12:28:11.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-20 12:28:23.979215 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-20 12:28:11.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:28:23.979215 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-06-20 12:28:11.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-20 12:28:11.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:28:23.979215 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-20 12:28:11.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-20 12:28:11.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:28:23.979215 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-20 12:28:11.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-20 12:28:11.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-20 12:28:11.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 12:28:23.979215 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:28:23.975215 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:28:23.975215 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:28:23.975215 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/src/autora/experiment_runner/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:28:23.975215 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/src/autora/experiment_runner/recruitment_manager/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:28:23.979215 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/src/autora/experiment_runner/recruitment_manager/prolific/
+-rw-r--r--   0 runner    (1001) docker     (123)    13393 2023-06-20 12:28:11.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:28:23.979215 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-20 12:28:23.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-20 12:28:23.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 12:28:23.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-20 12:28:23.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 12:28:23.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:28:23.979215 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-20 12:28:11.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:28:11.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 12:28:11.000000 autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/tests/test_recruitment_manager_prolific.py
```

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/.github/workflows/python-publish.yml` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/.gitignore` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/.pre-commit-config.yaml` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/PKG-INFO` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-recruitment-manager-prolific
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: AutoRA Prolific Recruitment Manager provides functionality to recruit participants via Prolific to set up an experiment runner for AutoRA
 Author-email: Kevin Phan <kphan@princeton.edu>, Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experiment-runner-recruitment-manager-prolific
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/README.md` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/README.md`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/docs/Basic Usage.ipynb` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/mkdocs/base.yml` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/pyproject.toml` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/src/autora/experiment_runner/recruitment_manager/prolific/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,86 @@
 import random
 import string
 from typing import Any, List
 import requests
 import json
 
 
+def __get_request_results(url, headers):
+    # Fetch all submissions using pagination
+    all_submissions = []
+
+    while True:
+        response = requests.get(url, headers=headers)
+        data = response.json()
+
+        if "results" in data:
+            all_submissions.extend(data["results"])
+
+        next_page = data.get("next_page")
+        if next_page:
+            url = next_page
+        else:
+            break
+    return all_submissions
+
+
+def __get_request_results_id(url, headers):
+    page = 1  # Start with the first page
+    results_per_page = 50  # Specify the number of results per page
+
+    # Concatenate all submissions
+    all_submissions = []
+
+    while True:
+        response = requests.get(
+            url,
+            headers=headers,
+
+        )
+        data = response.json()
+        url = data['_links']['next']['href']
+        # Concatenate the JSON object from the response
+        all_submissions.extend(data.get("results", []))
+
+        # Check if there are no more results
+        if url is None:
+            break
+
+    return all_submissions
+
+
 def _list_studies(prolific_token: str):
     """
     Returns list of all studies on Prolific account.
     """
-    studies = requests.get(
+    studies = __get_request_results(
         "https://api.prolific.co/api/v1/studies/",
-        headers={"Authorization": f"Token {prolific_token}"},
+        {"Authorization": f"Token {prolific_token}"},
     )
-    return studies.json()
+    return studies
 
 
 def _studies_from_name(study_name: str, prolific_token: str):
     """
     Returns the ids and status of studies with a given the name.
     """
-    lst = _list_studies(prolific_token)['results']
+    lst = _list_studies(prolific_token)
     return [{'id': s['id'], 'status': s['status']} for s in lst if s['name'] == study_name]
 
 
 def _is_study_uncompleted(study_name: str, prolific_token: str):
     """
     Returns true if there is alread a study with the name that is not completed
     """
     lst = _studies_from_name(study_name, prolific_token)
     incomplete_lst = [s for s in lst if s['status'] != 'COMPLETED']
     return len(incomplete_lst) > 0
 
 
-# def _get_id_from_name(study_name: str, prolific_token: str):
-#     """
-#     Returns the id of a study given its name.
-#     """
-#     lst = _list_studies(prolific_token)["results"]
-#     for s in lst:
-#         if s["name"] == study_name:
-#             return s["id"]
-#     return ""
-
-
 def _update_study(study_id: str, prolific_token: str, **kwargs) -> bool:
     """
     Updates the parameters of a given study.
     If a study is already published, only internal_name
     and total_available_places can be updated.
     """
     study = requests.patch(
@@ -85,34 +118,24 @@
         "places_taken",
         "status",
         "number_of_submissions",
     ]
     return dict((key, value) for key, value in study.items() if key in keys_to_include)
 
 
-# def increase_participant_count(
-#         study_name: str, prolific_token: str, increment: int = 1
-# ) -> bool:
-#     """
-#     Increase participants on prolific to collect data for a new cycle
-#
-#     Args:
-#         study_name: name of the study as given in prolific
-#         increment: number of participants to recruit for this cycle
-#         prolific_token: a prolific api token
-#     Returns:
-#         Returns True if participants got increased
-#     """
-#     study_id = _get_id_from_name(study_name, prolific_token)
-#     available_places = _retrieve_study(study_id, prolific_token)[
-#         "total_available_places"
-#     ]
-#     return _update_study(
-#         study_id, prolific_token, total_available_places=available_places + increment
-#     )
+def _append_url_variable(url, variable):
+    """
+    appends an url variable if not already in url
+    """
+    if variable not in url:
+        if '?' in url:
+            url += f'&{variable}'
+        else:
+            url += f'?{variable}'
+    return url
 
 
 def setup_study(
         name: str,
         description: str,
         external_study_url: str,
         estimated_completion_time: int,
@@ -173,15 +196,15 @@
             nationality_eligibility,
             vision_eligibility,
             language_eligibility,
         ]
     if _is_study_uncompleted(name, prolific_token):
         print('ERROR: There is a study with this name that is not completed. Can not proceed.')
         return
-    previous_studies = _list_studies(prolific_token)["results"]
+    previous_studies = _list_studies(prolific_token)
     excludes = [
         {"name": s["name"], "id": s["id"]}
         for s in previous_studies
         if s["name"] in exclude_studies
     ]
     if excludes is not []:
         eligibility_requirements += [EligibilityOptions.previous_studies(excludes)]
@@ -192,14 +215,16 @@
     if completion_code == "":
         completion_code = "".join(
             random.choices(string.ascii_letters + string.digits, k=6)
         )
     if reward == 0:
         reward = round(20 * estimated_completion_time)  # 12$ per hour / 20¢ per minute
 
+    external_study_url = _append_url_variable(external_study_url, 'PROLIFIC_PID={{%PROLIFIC_PID%}}')
+
     # packages function parameters into dictionary
     data = locals()
 
     data["completion_code_action"] = "AUTOMATICALLY_APPROVE"
     study = requests.post(
         "https://api.prolific.co/api/v1/studies/",
         headers={"Authorization": f"Token {prolific_token}"},
@@ -237,15 +262,14 @@
     )
     if study.status_code != 400:
         print(study.json())
         return False
     return True
 
 
-# number_of_submissions
 def pause_study(study_id: str, prolific_token: str):
     """
     Pauses the study
     """
     return _update_study_status(study_id, "PAUSE", prolific_token)
 
 
@@ -260,23 +284,18 @@
     """
     Publish the study
     """
     return _update_study_status(study_id, "PUBLISH", prolific_token)
 
 
 def _get_submissions(study_id: str, prolific_token: str):
-    study = requests.get(
+    study = __get_request_results_id(
         f"https://api.prolific.co/api/v1/studies/{study_id}/submissions/",
-        headers={"Authorization": f"Token {prolific_token}"},
-
-    )
-    if study.status_code != 200:
-        print(study.json())
-        return False
-    return study.json()['results']
+        {"Authorization": f"Token {prolific_token}"})
+    return study
 
 
 def _get_participants_by_status(study_id: str, prolific_token: str, status: str):
     results = _get_submissions(study_id, prolific_token)
     return [d['participant_id'] for d in results if d["status"] == status]
 
 
@@ -284,14 +303,18 @@
     return _get_participants_by_status(study_id, prolific_token, 'AWAITING REVIEW')
 
 
 def get_participants_returned(study_id: str, prolific_token: str):
     return _get_participants_by_status(study_id, prolific_token, 'RETURNED')
 
 
+def get_participants_timed_out(study_id: str, prolific_token: str):
+    return _get_participants_by_status(study_id, prolific_token, 'TIMED OUT')
+
+
 def approve_all(study_id: str, prolific_token: str):
     awaiting_review = get_participants_awaiting_review(study_id, prolific_token)
     data = {"study_id": study_id,
             "participant_ids": awaiting_review
             }
     study = requests.post(
         f"https://api.prolific.co/api/v1/submissions/bulk-approve/",
```

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experiment-runner-recruitment-manager-prolific
-Version: 1.0.0a4
+Version: 1.0.0a5
 Summary: AutoRA Prolific Recruitment Manager provides functionality to recruit participants via Prolific to set up an experiment runner for AutoRA
 Author-email: Kevin Phan <kphan@princeton.edu>, Younes Strittmatter <younes_strittmatter@brown.edu>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experiment-runner-recruitment-manager-prolific
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/src/autora_experiment_runner_recruitment_manager_prolific.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-experiment-runner-recruitment-manager-prolific-1.0.0a4/tests/README.md` & `autora-experiment-runner-recruitment-manager-prolific-1.0.0a5/tests/README.md`

 * *Files identical despite different names*

