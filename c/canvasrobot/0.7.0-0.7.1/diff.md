# Comparing `tmp/canvasrobot-0.7.0.tar.gz` & `tmp/canvasrobot-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canvasrobot-0.7.0.tar", max compression
+gzip compressed data, was "canvasrobot-0.7.1.tar", max compression
```

## Comparing `canvasrobot-0.7.0.tar` & `canvasrobot-0.7.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      229 2023-01-05 13:29:04.133543 canvasrobot-0.7.0/README.md
--rw-r--r--   0        0        0      336 2023-06-20 11:08:01.804453 canvasrobot-0.7.0/canvasrobot/__init__.py
--rw-r--r--   0        0        0    70069 2023-06-20 11:02:11.302391 canvasrobot-0.7.0/canvasrobot/canvasrobot.py
--rw-r--r--   0        0        0    10766 2023-06-06 12:14:27.990182 canvasrobot-0.7.0/canvasrobot/canvasrobot_model.py
--rw-r--r--   0        0        0      402 2023-03-09 18:01:08.232782 canvasrobot-0.7.0/canvasrobot/entities/__init__.py
--rw-r--r--   0        0        0     1113 2023-05-10 09:19:06.275056 canvasrobot-0.7.0/canvasrobot/entities/course.py
--rw-r--r--   0        0        0      663 2023-03-09 17:33:17.175051 canvasrobot-0.7.0/canvasrobot/entities/guest.py
--rw-r--r--   0        0        0        0 2023-05-24 15:41:21.895635 canvasrobot-0.7.0/canvasrobot/entities/py.typed
--rw-r--r--   0        0        0     1017 2023-03-09 17:33:17.175104 canvasrobot-0.7.0/canvasrobot/entities/quiz.py
--rw-r--r--   0        0        0     2182 2023-03-09 17:42:32.613135 canvasrobot-0.7.0/canvasrobot/entities/user.py
--rw-r--r--   0        0        0      749 2023-06-20 11:07:03.522945 canvasrobot-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      998 1970-01-01 00:00:00.000000 canvasrobot-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     2283 2023-06-20 12:11:20.754863 canvasrobot-0.7.1/README.md
+-rw-r--r--   0        0        0      336 2023-06-20 12:11:20.740593 canvasrobot-0.7.1/canvasrobot/__init__.py
+-rw-r--r--   0        0        0    70054 2023-06-20 12:11:20.751801 canvasrobot-0.7.1/canvasrobot/canvasrobot.py
+-rw-r--r--   0        0        0    10766 2023-06-06 12:14:27.990182 canvasrobot-0.7.1/canvasrobot/canvasrobot_model.py
+-rw-r--r--   0        0        0      402 2023-03-09 18:01:08.232782 canvasrobot-0.7.1/canvasrobot/entities/__init__.py
+-rw-r--r--   0        0        0     1113 2023-05-10 09:19:06.275056 canvasrobot-0.7.1/canvasrobot/entities/course.py
+-rw-r--r--   0        0        0      663 2023-03-09 17:33:17.175051 canvasrobot-0.7.1/canvasrobot/entities/guest.py
+-rw-r--r--   0        0        0        0 2023-05-24 15:41:21.895635 canvasrobot-0.7.1/canvasrobot/entities/py.typed
+-rw-r--r--   0        0        0     1017 2023-03-09 17:33:17.175104 canvasrobot-0.7.1/canvasrobot/entities/quiz.py
+-rw-r--r--   0        0        0     2182 2023-03-09 17:42:32.613135 canvasrobot-0.7.1/canvasrobot/entities/user.py
+-rw-r--r--   0        0        0      749 2023-06-20 12:28:56.421649 canvasrobot-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     3064 1970-01-01 00:00:00.000000 canvasrobot-0.7.1/PKG-INFO
```

### Comparing `canvasrobot-0.7.0/canvasrobot/canvasrobot.py` & `canvasrobot-0.7.1/canvasrobot/canvasrobot.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,18 +43,15 @@
 # we don't need the info messages
 # from this library
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 
-
 # noinspection PyProtectedMember
-
-
 def file_update(file, **kwargs):
     """
         Updates a file.
         :calls: `PUT /api/v1/files/:id \
         <https://canvas.instructure.com/doc/api/files.html#method.files.update>`_
         :rtype: :class:`canvasapi.file.File`
         """
@@ -421,15 +418,15 @@
 
         try:
             course.enroll_user(user, enrollment_type)
         except Exception as e:
             return f"Enroll of {user} in {course} as {enrollment_type} failed:{e}"
         return f"Enrolled {user} in {course} as {enrollment_type}"
 
-    def get_all_active_tst_courses(self, from_db=True):
+    def get_all_active_courses(self, from_db=True):
         """"":returns list of all TST course canvas course """
 
         def cur_year_active(course):
             """ filter function"""
             return (str(course.sis_course_id)[:4] == str(self.year) and
                     not course.name.endswith('conclude'))
 
@@ -1534,24 +1531,24 @@
                                          parent_folder_path='/',
                                          locked=True)
         logger.info(f"Folder '(course) files/{foldername}' should be created now in ({course_id=})")
         return folder_id
 
     def create_folder_in_all_courses(self, foldername):
 
-        for course in track(self.get_all_active_tst_courses(from_db=False),
+        for course in track(self.get_all_active_courses(from_db=False),
                             description="All current courses...",
                             console=self.console):
             self.create_folder_in_course_files(course.id, foldername)
 
     def unpublish_subfolder_in_all_courses(self,
                                            foldername: str,
                                            files_too: bool = False,
                                            check_only: bool = False):
-        for course in track(self.get_all_active_tst_courses(from_db=False),
+        for course in track(self.get_all_active_courses(from_db=False),
                             description=(f"Checking all current"
                                          f" courses for folder '{foldername}'..." if check_only
                             else f"Unpublish all published folder {foldername}..."),
                             console=self.console):
             if course.name.endswith("_conclude"):
                 continue
             # logger.info(course.name)
```

### Comparing `canvasrobot-0.7.0/canvasrobot/canvasrobot_model.py` & `canvasrobot-0.7.1/canvasrobot/canvasrobot_model.py`

 * *Files identical despite different names*

### Comparing `canvasrobot-0.7.0/canvasrobot/entities/course.py` & `canvasrobot-0.7.1/canvasrobot/entities/course.py`

 * *Files identical despite different names*

### Comparing `canvasrobot-0.7.0/canvasrobot/entities/guest.py` & `canvasrobot-0.7.1/canvasrobot/entities/guest.py`

 * *Files identical despite different names*

### Comparing `canvasrobot-0.7.0/canvasrobot/entities/quiz.py` & `canvasrobot-0.7.1/canvasrobot/entities/quiz.py`

 * *Files identical despite different names*

### Comparing `canvasrobot-0.7.0/canvasrobot/entities/user.py` & `canvasrobot-0.7.1/canvasrobot/entities/user.py`

 * *Files identical despite different names*

### Comparing `canvasrobot-0.7.0/pyproject.toml` & `canvasrobot-0.7.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "canvasrobot"
-version = "0.7.0"
+version = "0.7.1"
 description = "Library which uses Canvasapi https://canvasapi.readthedocs.io/en/stable/getting-started.html to provide a CanvasRobot class."
 authors = ["Nico de Groot <ndegroot0@gmail.com>",]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0.0"
-requests = "~=2.28.1"
-pyaml = "^21.10.1"
-canvasapi = "~=3.0.0"
-openpyxl = "^3.0.10"
+openpyxl = "^3.0"
 pydal = "*"
-rich = "*"
 toml = "*"
 keyring = "*"
+requests = "^2.31.0"
+pyaml = "^23.5.9"
+rich = "^13.4.2"
+canvasapi = "^3.2.0"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 mock = "*"
 pylint = "*"
 ruff = "*"
```

