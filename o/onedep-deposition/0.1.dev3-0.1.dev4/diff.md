# Comparing `tmp/onedep_deposition-0.1.dev3.tar.gz` & `tmp/onedep_deposition-0.1.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onedep_deposition-0.1.dev3.tar", last modified: Mon Jun 19 15:36:28 2023, max compression
+gzip compressed data, was "onedep_deposition-0.1.dev4.tar", last modified: Mon Jun 19 17:12:56 2023, max compression
```

## Comparing `onedep_deposition-0.1.dev3.tar` & `onedep_deposition-0.1.dev4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-19 15:36:28.005573 onedep_deposition-0.1.dev3/
--rw-r--r--   0 peisach    (502) staff       (20)      552 2023-06-13 13:04:02.000000 onedep_deposition-0.1.dev3/LICENSE
--rw-r--r--   0 peisach    (502) staff       (20)     5174 2023-06-19 15:36:28.005145 onedep_deposition-0.1.dev3/PKG-INFO
--rw-r--r--   0 peisach    (502) staff       (20)     4641 2023-06-17 15:30:45.000000 onedep_deposition-0.1.dev3/README.md
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-19 15:36:28.000415 onedep_deposition-0.1.dev3/onedep_deposition/
--rw-r--r--   0 peisach    (502) staff       (20)       25 2023-06-19 15:35:51.000000 onedep_deposition-0.1.dev3/onedep_deposition/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-19 15:36:28.004556 onedep_deposition-0.1.dev3/onedep_deposition/cli/
--rw-r--r--   0 peisach    (502) staff       (20)        0 2023-06-17 17:42:03.000000 onedep_deposition-0.1.dev3/onedep_deposition/cli/__init__.py
--rw-r--r--   0 peisach    (502) staff       (20)    12124 2023-06-19 15:35:16.000000 onedep_deposition-0.1.dev3/onedep_deposition/cli/cli.py
--rw-r--r--   0 peisach    (502) staff       (20)    16794 2023-06-17 16:20:15.000000 onedep_deposition-0.1.dev3/onedep_deposition/constants.py
--rw-r--r--   0 peisach    (502) staff       (20)    14441 2023-06-19 14:33:49.000000 onedep_deposition-0.1.dev3/onedep_deposition/deposit_api.py
--rw-r--r--   0 peisach    (502) staff       (20)     9006 2023-06-15 13:32:19.000000 onedep_deposition-0.1.dev3/onedep_deposition/enum.py
--rw-r--r--   0 peisach    (502) staff       (20)      159 2023-06-08 16:58:15.000000 onedep_deposition-0.1.dev3/onedep_deposition/exceptions.py
--rw-r--r--   0 peisach    (502) staff       (20)    12948 2023-06-19 15:35:41.000000 onedep_deposition-0.1.dev3/onedep_deposition/models.py
--rw-r--r--   0 peisach    (502) staff       (20)     5810 2023-06-19 15:34:56.000000 onedep_deposition-0.1.dev3/onedep_deposition/rest_adapter.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-19 15:36:28.003656 onedep_deposition-0.1.dev3/onedep_deposition.egg-info/
--rw-r--r--   0 peisach    (502) staff       (20)     5174 2023-06-19 15:36:27.000000 onedep_deposition-0.1.dev3/onedep_deposition.egg-info/PKG-INFO
--rw-r--r--   0 peisach    (502) staff       (20)      557 2023-06-19 15:36:27.000000 onedep_deposition-0.1.dev3/onedep_deposition.egg-info/SOURCES.txt
--rw-r--r--   0 peisach    (502) staff       (20)        1 2023-06-19 15:36:27.000000 onedep_deposition-0.1.dev3/onedep_deposition.egg-info/dependency_links.txt
--rw-r--r--   0 peisach    (502) staff       (20)       68 2023-06-19 15:36:27.000000 onedep_deposition-0.1.dev3/onedep_deposition.egg-info/entry_points.txt
--rw-r--r--   0 peisach    (502) staff       (20)       15 2023-06-19 15:36:27.000000 onedep_deposition-0.1.dev3/onedep_deposition.egg-info/requires.txt
--rw-r--r--   0 peisach    (502) staff       (20)       18 2023-06-19 15:36:27.000000 onedep_deposition-0.1.dev3/onedep_deposition.egg-info/top_level.txt
--rw-r--r--   0 peisach    (502) staff       (20)     1039 2023-06-17 17:50:36.000000 onedep_deposition-0.1.dev3/pyproject.toml
--rw-r--r--   0 peisach    (502) staff       (20)       38 2023-06-19 15:36:28.005741 onedep_deposition-0.1.dev3/setup.cfg
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-19 17:12:56.280950 onedep_deposition-0.1.dev4/
+-rw-r--r--   0 peisach    (502) staff       (20)      552 2023-06-13 13:04:02.000000 onedep_deposition-0.1.dev4/LICENSE
+-rw-r--r--   0 peisach    (502) staff       (20)     5174 2023-06-19 17:12:56.280637 onedep_deposition-0.1.dev4/PKG-INFO
+-rw-r--r--   0 peisach    (502) staff       (20)     4641 2023-06-17 15:30:45.000000 onedep_deposition-0.1.dev4/README.md
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-19 17:12:56.275981 onedep_deposition-0.1.dev4/onedep_deposition/
+-rw-r--r--   0 peisach    (502) staff       (20)       25 2023-06-19 17:12:23.000000 onedep_deposition-0.1.dev4/onedep_deposition/__init__.py
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-19 17:12:56.280084 onedep_deposition-0.1.dev4/onedep_deposition/cli/
+-rw-r--r--   0 peisach    (502) staff       (20)        0 2023-06-17 17:42:03.000000 onedep_deposition-0.1.dev4/onedep_deposition/cli/__init__.py
+-rw-r--r--   0 peisach    (502) staff       (20)    12301 2023-06-19 17:09:13.000000 onedep_deposition-0.1.dev4/onedep_deposition/cli/cli.py
+-rw-r--r--   0 peisach    (502) staff       (20)    16794 2023-06-17 16:20:15.000000 onedep_deposition-0.1.dev4/onedep_deposition/constants.py
+-rw-r--r--   0 peisach    (502) staff       (20)    14894 2023-06-19 17:09:13.000000 onedep_deposition-0.1.dev4/onedep_deposition/deposit_api.py
+-rw-r--r--   0 peisach    (502) staff       (20)     9006 2023-06-15 13:32:19.000000 onedep_deposition-0.1.dev4/onedep_deposition/enum.py
+-rw-r--r--   0 peisach    (502) staff       (20)      159 2023-06-08 16:58:15.000000 onedep_deposition-0.1.dev4/onedep_deposition/exceptions.py
+-rw-r--r--   0 peisach    (502) staff       (20)    12847 2023-06-19 17:09:13.000000 onedep_deposition-0.1.dev4/onedep_deposition/models.py
+-rw-r--r--   0 peisach    (502) staff       (20)     5810 2023-06-19 15:34:56.000000 onedep_deposition-0.1.dev4/onedep_deposition/rest_adapter.py
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-19 17:12:56.279155 onedep_deposition-0.1.dev4/onedep_deposition.egg-info/
+-rw-r--r--   0 peisach    (502) staff       (20)     5174 2023-06-19 17:12:56.000000 onedep_deposition-0.1.dev4/onedep_deposition.egg-info/PKG-INFO
+-rw-r--r--   0 peisach    (502) staff       (20)      557 2023-06-19 17:12:56.000000 onedep_deposition-0.1.dev4/onedep_deposition.egg-info/SOURCES.txt
+-rw-r--r--   0 peisach    (502) staff       (20)        1 2023-06-19 17:12:56.000000 onedep_deposition-0.1.dev4/onedep_deposition.egg-info/dependency_links.txt
+-rw-r--r--   0 peisach    (502) staff       (20)       68 2023-06-19 17:12:56.000000 onedep_deposition-0.1.dev4/onedep_deposition.egg-info/entry_points.txt
+-rw-r--r--   0 peisach    (502) staff       (20)       15 2023-06-19 17:12:56.000000 onedep_deposition-0.1.dev4/onedep_deposition.egg-info/requires.txt
+-rw-r--r--   0 peisach    (502) staff       (20)       18 2023-06-19 17:12:56.000000 onedep_deposition-0.1.dev4/onedep_deposition.egg-info/top_level.txt
+-rw-r--r--   0 peisach    (502) staff       (20)     1039 2023-06-17 17:50:36.000000 onedep_deposition-0.1.dev4/pyproject.toml
+-rw-r--r--   0 peisach    (502) staff       (20)       38 2023-06-19 17:12:56.281105 onedep_deposition-0.1.dev4/setup.cfg
```

### Comparing `onedep_deposition-0.1.dev3/LICENSE` & `onedep_deposition-0.1.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev3/PKG-INFO` & `onedep_deposition-0.1.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onedep_deposition
-Version: 0.1.dev3
+Version: 0.1.dev4
 Summary: Package for wrapping the OneDep deposition API services
 Author-email: Neli Jose da Fonseca Junior <neli@ebi.ac.uk>
 License: apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `onedep_deposition-0.1.dev3/README.md` & `onedep_deposition-0.1.dev4/README.md`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev3/onedep_deposition/cli/cli.py` & `onedep_deposition-0.1.dev4/onedep_deposition/cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,14 +84,18 @@
             raise click.BadParameter("Invalid experiment subtype, options are: helical, single, subtomogram, tomography")
     if not email:
         raise click.BadParameter("Email is required")
     if not re.match(r'^[\w\.-]+@[\w\.-]+\.\w+$', email):
         raise click.BadParameter("Invalid email")
     if len(users) == 0:
         raise click.BadParameter("At least one user is required")
+    else:
+        for orcid in users:
+            if not re.match(r'^\d{4}-\d{4}-\d{4}-\d{3}[\dX]$', orcid):
+                raise click.BadParameter(f"Invalid ORCID: {orcid}")
     if related_bmrb:
         if not re.match(r'^\d+$', related_bmrb):
             raise click.BadParameter("Invalid BMRB code")
     if related_emdb:
         if not re.match(r'^EMD-\d{4,5}$', related_emdb):
             raise click.BadParameter("Invalid EMDB code")
     country = get_country_enum(country_string)
```

### Comparing `onedep_deposition-0.1.dev3/onedep_deposition/constants.py` & `onedep_deposition-0.1.dev4/onedep_deposition/constants.py`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev3/onedep_deposition/deposit_api.py` & `onedep_deposition-0.1.dev4/onedep_deposition/deposit_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,14 +60,15 @@
             data["password"] = password
 
         # If a hostname was not given in the class constructor, get one from the country
         if not self.given_hostname:
             self._rest_adapter.hostname = self._get_site_from_country(country)
 
         response = self._rest_adapter.post("depositions/new", data=data)
+        response.data["dep_id"] = response.data.pop("id")
         deposit = Deposit(**response.data)
         return deposit
 
     def create_em_deposition(self, email: str, users: List[str], country: Country, subtype: Union[EMSubType, str],  # pylint: disable=unused-argument
                              related_emdb: str = None, password: str = "", **kwargs) -> Deposit:
         """
         Create an EM deposition
@@ -170,14 +171,15 @@
         """
         Get deposition from ID
         :param dep_id: Deposition ID
         :return: Deposit
         """
         try:
             response = self._rest_adapter.get(f"depositions/{dep_id}")
+            response.data['dep_id'] = response.data.pop('id')
             deposit = Deposit(**response.data)
         except DepositApiException as e:
             if e.status_code == 404:
                 return None
             else:
                 raise
 
@@ -187,27 +189,29 @@
         """
         Get all depositions from an user
         :return: List[Deposit]
         """
         depositions = []
         response = self._rest_adapter.get("depositions/")
         for deposition_json in response.data["items"]:
+            deposition_json['dep_id'] = deposition_json.pop('id')
             deposition = Deposit(**deposition_json)
             depositions.append(deposition)
         return depositions
 
     def get_users(self, dep_id: str):
         """
         Get users from deposition
         :param dep_id:
         :return: Depositor
         """
         users = []
         response = self._rest_adapter.get(f"depositions/{dep_id}/users/")
         for user_json in response.data:
+            user_json["user_id"] = user_json.pop("id")
             user = Depositor(**user_json)
             users.append(user)
         return users
 
     def add_user(self, dep_id: str, orcid: Union[List, str]) -> List[Depositor]:
         """
         Grant access from given users to deposition
@@ -220,14 +224,15 @@
         if type(orcid) == str:
             data.append({'orcid': orcid})
         elif type(orcid) == list:
             for orcid_id in orcid:
                 data.append({'orcid': orcid_id})
         response = self._rest_adapter.post(f"depositions/{dep_id}/users/", data=data)
         for user_json in response.data:
+            user_json["user_id"] = user_json.pop("id")
             users.append(Depositor(**user_json))
 
         return users
 
     def remove_user(self, dep_id: str, orcid: str):
         """
         Remove access from an user to a deposition
@@ -271,14 +276,15 @@
                     self.remove_file(dep_id, file.id)
 
         with open(file_path, "rb") as fp:
             files["file"] = (file_name, fp, mime_type)
 
             response = self._rest_adapter.post(f"depositions/{dep_id}/files/", data=data, files=files, content_type="")
             response.data["file_type"] = response.data.pop("type")
+            response.data["file_id"] = response.data.pop("id")
 
             return DepositedFile(**response.data)
 
     def get_files(self, dep_id: str) -> DepositedFilesSet:
         """
         Get all files in deposition
         :param dep_id: Deposition ID
@@ -300,15 +306,18 @@
     def get_status(self, dep_id: str) -> DepositStatus:
         """
         Return the deposition status
         :param dep_id: Deposition ID
         :return: Status
         """
         response = self._rest_adapter.get(f"depositions/{dep_id}/status")
-        status = DepositStatus(**response.data)
+        try:
+            status = DepositStatus(**response.data)
+        except TypeError:
+            status = DepositError(**response.data)
         return status
 
     def process(self, dep_id: str, voxel: List = None, copy_from_id: str = None, copy_contact: bool = False,
                 copy_authors: bool = False, copy_citation: bool = False, copy_grant: bool = False,
                 copy_em_exp_data: bool = False):
         """
         Trigger file processing
```

### Comparing `onedep_deposition-0.1.dev3/onedep_deposition/enum.py` & `onedep_deposition-0.1.dev4/onedep_deposition/enum.py`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev3/onedep_deposition/models.py` & `onedep_deposition-0.1.dev4/onedep_deposition/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 class Experiment:
     """Class representing an experiment"""
     def __init__(self, exp_type: Union[ExperimentType, str], subtype: Union[EMSubType, str] = None,
                  related_emdb: str = None, related_bmrb: str = None):
         """
         Constructor for Experiment
-        :param type:
+        :param exp_type:
         :param subtype:
         :param related_emdb:
         :param related_bmrb:
         """
         self._type = None
         self._subtype = None
         self._related_emdb = str(related_emdb) if related_emdb is not None else None
@@ -130,16 +130,15 @@
 
     def __str__(self):
         return f"CODE: {self._code}, MESSAGE: {self._message}\nEXTRAS: {self._extras}"
 
 
 class Deposit:
     """Class representing an deposit"""
-    # TODO: Replace id for dep_id
-    def __init__(self, email: str, id: str, entry_id: str, title: str, created: str, last_login: str, site: str,  # pylint: disable=redefined-builtin
+    def __init__(self, email: str, dep_id: str, entry_id: str, title: str, created: str, last_login: str, site: str,
                  status: Status, experiments: List = None, errors: List = None, site_url: str = None):
         """
         Constructor for Deposit
         :param email:
         :param dep_id:
         :param entry_id:
         :param title:
@@ -148,15 +147,15 @@
         :param site:
         :param status:
         :param experiments:
         :param errors:
         :param site_url
         """
         self._email = str(email)
-        self._id = str(id)
+        self._id = str(dep_id)
         self._entry_id = str(entry_id)
         self._title = str(title)
         self._created = datetime.fromisoformat(created)
         self._last_login = datetime.fromisoformat(last_login)
         self._site = str(site)
         self._status = getattr(Status, status)
         self._experiments = []
@@ -234,43 +233,42 @@
             json_object['errors'].append(error.json())
 
         return json_object
 
 
 class Depositor:
     """Class representing a depositor"""
-    # TODO: Replace id for dep_id
-    def __init__(self, orcid: str, id: int, full_name: str, last_login: str = None, date_joined: str = None,  # pylint: disable=redefined-builtin
+    def __init__(self, orcid: str, user_id: int, full_name: str, last_login: str = None, date_joined: str = None,
                  depositions: List[Deposit] = None):
         """Constructor for depositor
         :param orcid:
-        :param id:
+        :param user_id:
         :param full_name:
         :param last_login:
         :param date_joined:
         :param depositions:
         """
         self._orcid = str(orcid)
-        self._id = int(id)
+        self._user_id = int(user_id)
         self._full_name = str(full_name)
         self._last_login = datetime.fromisoformat(last_login) if last_login else None
         self._date_joined = datetime.fromisoformat(date_joined) if date_joined else None
         self._depositions = []
 
         if depositions:
             for deposition in depositions:
                 self._depositions.append(**deposition)
 
     @property
     def orcid(self) -> str:
         return self._orcid
 
     @property
-    def id(self) -> int:
-        return self._id
+    def user_id(self) -> int:
+        return self._user_id
 
     @property
     def full_name(self) -> str:
         return self._full_name
 
     @property
     def last_login(self) -> datetime:
@@ -281,41 +279,40 @@
         return self._date_joined
 
     @property
     def depositions(self) -> List[Deposit]:
         return self._depositions
 
     def __str__(self):
-        return f"Name: {self._full_name} [{self._id}]\nORCID: {self._orcid}\nDate joined: {self._date_joined}\nLast login: {self._last_login}\nDepositions: {self._depositions}"
+        return f"Name: {self._full_name} [{self._user_id}]\nORCID: {self._orcid}\nDate joined: {self._date_joined}\nLast login: {self._last_login}\nDepositions: {self._depositions}"
 
     def json(self):
         json_object = self.__dict__.copy()
         json_object = {key[1:]: value for key, value in json_object.items() if value is not None}
         json_object["depositions"] = []
 
         for deposition in self._depositions:
             json_object["depositions"].append(deposition.json())
 
         return json_object
 
 
 class DepositedFile:
     """Class representing a deposited file"""
-    # TODO: Replace id for dep_id
-    def __init__(self, id: int, created: str, name: str, file_type: Union[str, FileType], errors: List[str] = None,  # pylint: disable=redefined-builtin
+    def __init__(self, file_id: int, created: str, name: str, file_type: Union[str, FileType], errors: List[str] = None,
                  warnings: List[str] = None):
         """Constructor for deposited file
-        :param id:
+        :param file_id:
         :param created:
         :param name:
         :param file_type:
         :param errors:
         :param warnings:
         """
-        self._id = int(id)
+        self._id = int(file_id)
         self._name = str(name)
 
         date_format = "%A, %B %d, %Y %H:%M:%S"
         self._created = datetime.strptime(created, date_format)
 
         if isinstance(file_type, str):
             self._type = FileType(file_type)
@@ -332,15 +329,15 @@
         message += "\nWARNINGS:\n"
         for warning in self._warnings:
             message += f"  -{warning}\n"
 
         return message
 
     @property
-    def id(self) -> int:
+    def file_id(self) -> int:
         return self._id
 
     @property
     def created(self) -> datetime:
         return self._created
 
     @property
@@ -370,14 +367,15 @@
         self._errors = [DepositError(**error) for error in errors if error != ""] if errors else []
         self._warnings = [DepositError(**warning) for warning in warnings if warning != ""] if errors else []
 
         self.__current_index = 0
 
         for file in files:
             file["file_type"] = file.pop("type")
+            file["file_id"] = file.pop("id")
             self._files.append(DepositedFile(**file))
 
     def __getitem__(self, index):
         return self._files[index]
 
     def __len__(self):
         return len(self._files)
```

### Comparing `onedep_deposition-0.1.dev3/onedep_deposition/rest_adapter.py` & `onedep_deposition-0.1.dev4/onedep_deposition/rest_adapter.py`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev3/onedep_deposition.egg-info/PKG-INFO` & `onedep_deposition-0.1.dev4/onedep_deposition.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onedep-deposition
-Version: 0.1.dev3
+Version: 0.1.dev4
 Summary: Package for wrapping the OneDep deposition API services
 Author-email: Neli Jose da Fonseca Junior <neli@ebi.ac.uk>
 License: apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `onedep_deposition-0.1.dev3/onedep_deposition.egg-info/SOURCES.txt` & `onedep_deposition-0.1.dev4/onedep_deposition.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev3/pyproject.toml` & `onedep_deposition-0.1.dev4/pyproject.toml`

 * *Files identical despite different names*

