# Comparing `tmp/canvasrobot-0.6.1.tar.gz` & `tmp/canvasrobot-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canvasrobot-0.6.1.tar", max compression
+gzip compressed data, was "canvasrobot-0.7.0.tar", max compression
```

## Comparing `canvasrobot-0.6.1.tar` & `canvasrobot-0.7.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      229 2023-01-05 13:29:04.133543 canvasrobot-0.6.1/README.md
--rw-r--r--   0        0        0      338 2023-05-01 21:47:36.875391 canvasrobot-0.6.1/canvasrobot/__init__.py
--rw-r--r--   0        0        0    65809 2023-05-01 21:38:40.606868 canvasrobot-0.6.1/canvasrobot/canvas_robot.py
--rw-r--r--   0        0        0    10381 2023-03-30 08:46:30.991283 canvasrobot-0.6.1/canvasrobot/canvas_robot_model.py
--rw-r--r--   0        0        0      402 2023-03-09 18:01:08.232782 canvasrobot-0.6.1/canvasrobot/entities/__init__.py
--rw-r--r--   0        0        0     1099 2023-03-09 17:33:17.174768 canvasrobot-0.6.1/canvasrobot/entities/course.py
--rw-r--r--   0        0        0      663 2023-03-09 17:33:17.175051 canvasrobot-0.6.1/canvasrobot/entities/guest.py
--rw-r--r--   0        0        0     1017 2023-03-09 17:33:17.175104 canvasrobot-0.6.1/canvasrobot/entities/quiz.py
--rw-r--r--   0        0        0     2182 2023-03-09 17:42:32.613135 canvasrobot-0.6.1/canvasrobot/entities/user.py
--rw-r--r--   0        0        0      687 2023-05-01 21:47:36.871925 canvasrobot-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      998 1970-01-01 00:00:00.000000 canvasrobot-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      229 2023-01-05 13:29:04.133543 canvasrobot-0.7.0/README.md
+-rw-r--r--   0        0        0      336 2023-06-20 11:08:01.804453 canvasrobot-0.7.0/canvasrobot/__init__.py
+-rw-r--r--   0        0        0    70069 2023-06-20 11:02:11.302391 canvasrobot-0.7.0/canvasrobot/canvasrobot.py
+-rw-r--r--   0        0        0    10766 2023-06-06 12:14:27.990182 canvasrobot-0.7.0/canvasrobot/canvasrobot_model.py
+-rw-r--r--   0        0        0      402 2023-03-09 18:01:08.232782 canvasrobot-0.7.0/canvasrobot/entities/__init__.py
+-rw-r--r--   0        0        0     1113 2023-05-10 09:19:06.275056 canvasrobot-0.7.0/canvasrobot/entities/course.py
+-rw-r--r--   0        0        0      663 2023-03-09 17:33:17.175051 canvasrobot-0.7.0/canvasrobot/entities/guest.py
+-rw-r--r--   0        0        0        0 2023-05-24 15:41:21.895635 canvasrobot-0.7.0/canvasrobot/entities/py.typed
+-rw-r--r--   0        0        0     1017 2023-03-09 17:33:17.175104 canvasrobot-0.7.0/canvasrobot/entities/quiz.py
+-rw-r--r--   0        0        0     2182 2023-03-09 17:42:32.613135 canvasrobot-0.7.0/canvasrobot/entities/user.py
+-rw-r--r--   0        0        0      749 2023-06-20 11:07:03.522945 canvasrobot-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      998 1970-01-01 00:00:00.000000 canvasrobot-0.7.0/PKG-INFO
```

### Comparing `canvasrobot-0.6.1/canvasrobot/canvas_robot.py` & `canvasrobot-0.7.0/canvasrobot/canvasrobot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,69 @@
+from typing import Optional, Union, Any
 import io
 import json
 import mimetypes
-import osstatus
+import os
 import re
 import time
 from collections import namedtuple
 from datetime import datetime
+import logging
+import binascii
 
 import attrs
 from attrs import define, asdict
-import canvasapi
+import canvasapi  # type: ignore
 import requests
-import logging
 
-from rich.logging import RichHandler
+# from functools import lru_cache
+try:  # type: ignore
+    from pymemcache import serde  # type: ignore
+    from pymemcache.client import base  # type: ignore
+
+    MEMCACHED: Union[base.Client, bool] = True
+except ImportError:
+    print("No memcaching")
+    MEMCACHED = False
+#  from rich.logging import RichHandler
 from rich.progress import track
-from canvasapi.course import Course
-from canvasapi.util import combine_kwargs
-from openpyxl.styles import NamedStyle, Font, PatternFill, Alignment
-from openpyxl.utils import get_column_letter
-from openpyxl.workbook import Workbook
-from openpyxl.worksheet.dimensions import ColumnDimension, DimensionHolder
-
-from .canvas_robot_model import AC_YEAR, NEXT_YEAR, ENROLLMENT_TYPES, \
-    EDUCATIONS, COMMUNITIES, LocalDAL, CanvasConfig, EXAMINATION_FOLDER
-from .entities import User, QuestionDTO, CourseMetadata, Grade, ExaminationDTO, Stats
+from canvasapi.course import Course  # type: ignore
+from openpyxl.styles import NamedStyle, Font, PatternFill, Alignment  # type: ignore
+from canvasapi.util import combine_kwargs  # type: ignore
+from openpyxl.utils import get_column_letter  # type: ignore
+from openpyxl.workbook import Workbook  # type: ignore
+from openpyxl.worksheet.dimensions import ColumnDimension, DimensionHolder  # type: ignore
+from socket import gaierror, timeout
+from .canvasrobot_model import (AC_YEAR, NEXT_YEAR, ENROLLMENT_TYPES,  # type: ignore
+                                 EDUCATIONS, COMMUNITIES, LocalDAL, CanvasConfig,
+                                 EXAMINATION_FOLDER)  # type: ignore
+from .entities import User, QuestionDTO, CourseMetadata, Grade, ExaminationDTO, \
+    Stats  # type: ignore
 
 logging.getLogger("canvasapi").setLevel(logging.WARNING)
 # we don't need the info messages
 # from this library
 
-logging.basicConfig(
-    level=logging.INFO,
-    format="%(asctime)s [%(levelname)s] %(message)s",
-    handlers=[
-        logging.FileHandler("canvasrobot.log"),
-        RichHandler()
-        # logging.StreamHandler(sys.stdout)
-    ]
-)
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
 
 
 
 # noinspection PyProtectedMember
+
+
 def file_update(file, **kwargs):
     """
         Updates a file.
         :calls: `PUT /api/v1/files/:id \
         <https://canvas.instructure.com/doc/api/files.html#method.files.update>`_
         :rtype: :class:`canvasapi.file.File`
         """
     response = file._requester.request(
-        "PUT", "files/{}".format(file.id), _kwargs=combine_kwargs(**kwargs)
+            "PUT", "files/{}".format(file.id), _kwargs=combine_kwargs(**kwargs)
     )
 
     if "name" in response.json():
         response.set_attributes(response.json())
 
     return canvasapi.file.File(file._requester, response.json())
 
@@ -67,67 +75,223 @@
 
 
 class DibsaRetrieveError(Error):
     """Raised when connection to Dibsa or retrieval failed"""
     pass
 
 
-
+# noinspection PyClassHasNoInit
 @define
 class LabelType:
     label: str
     field_type: str
 
 
+# noinspection PyClassHasNoInit
 @define
 class Profile:
     login_id: str
     id: int
     name: str
     short_name: str
     sortable_name: str
     avatar_url: str
     title: str
-    bio: any  # can be N
+    bio: Optional[str]  # can be N
     primary_email: str
     integration_id: str
     time_zone: str
     locale: str
     # effective_locale str)
     # calendar str)
     # lti_user_id str)
 
 
+if MEMCACHED:
+    try:
+        MEMCACHED = base.Client(('localhost', 11211),
+                                connect_timeout=1,
+                                timeout=0.2,
+                                serde=serde.pickle_serde)
+        result = MEMCACHED.set('canvasbot', 'Running')
+        running = MEMCACHED.get('canvasrobot')
+    except (ConnectionRefusedError, gaierror, timeout):
+        MEMCACHED = False
+
+
+# noinspection PyCallingNonCallable,GrazieInspection
+
+
+def course_metadata_memcached(course_id, canvas, ignore_assignment_names):
+    def get_md():
+        course = canvas.get_course(course_id)
+        modules = course.get_modules()
+        nr_modules = len(list(modules))
+        nr_module_items = 0
+        nr_ext_urls = 0
+        for module in modules:
+            module_items = module.get_module_items()
+            item_count_ext_url = filter(lambda i: i.type == "ext_url", module_items)
+            nr_ext_urls += len(list(item_count_ext_url))
+            nr_module_items += module.items_count
+        pages = course.get_pages()
+        pages = filter(lambda p: p.title[0:3] != 'UVT', pages)
+        nr_pages = len(list(pages))
+        assignments = course.get_assignments()
+        assignments_summary = "Assignments:\n"
+        examinations = []
+        for assignment in assignments:
+            if assignment.name not in ignore_assignment_names:
+                assignments_summary += f"{assignment.name}"
+                examination = ExaminationDTO(course_id,
+                                             course.name,
+                                             assignment.name)
+
+                examinations.append(examination)
+            else:
+                assignments_summary += f"ignored: {assignment.name}"
+                # if show_all else ""
 
-# noinspection PyTypeChecker,PyUnresolvedReferences,PyCallingNonCallable
+            submissions_summary = ""
+            submissions = assignment.get_submissions()
+            # try:
+            for idx, submission in enumerate(submissions, start=1):
+                if assignment.name not in ignore_assignment_names:
+                    if submission.submission_type == "online_upload":
+
+                        originality_str = (f"{submission.has_originality_report}"
+                                           if hasattr(submission,
+                                                      'has_originality_report')
+                                           else "no Originality Report!")
+                        submissions_summary += (f"({idx}. "
+                                                f"{submission.submission_type}) "
+                                                f"graded "
+                                                f"{submission.grade} at "
+                                                f"{submission.graded_at}. "
+                                                f"Checked for plagiarism: "
+                                                f"{originality_str}\n"
+                                                )
+                    else:
+                        submissions_summary += (f"({idx}. "
+                                                f"{submission.submission_type}) "
+                                                f"graded "
+                                                f"{submission.grade} at "
+                                                f"{submission.graded_at}\n")
+            assignments_summary += f"\n{submissions_summary}"
+        nr_assignments = len(list(assignments))
+        quizzes = course.get_quizzes()
+        nr_quizzes = len(list(quizzes))
+        files = course.get_files()
+        nr_files = len(list(files))
+        # check for uploaded examination files
+        examinations_summary = ""
+        examination_files = 0
+        examination_folder_found = False
+        for file in files:
+            folder = course.get_folder(file.folder_id)
+            if f"/{EXAMINATION_FOLDER}" in folder.full_name:
+                examination_folder_found = True
+                examination_files += 1
+                examinations_summary += f"{file.display_name}\n"
+        if examination_files == 0:
+            if examination_folder_found:
+                examinations_summary += (f"No examination files in "
+                                         f"folder {EXAMINATION_FOLDER}\n")
+            else:
+                examinations_summary += f"No folder {EXAMINATION_FOLDER}\n"
+        else:
+            examinations_summary += (f"\nTotal: {examination_files} "
+                                     f"examination files"
+                                     f"in {EXAMINATION_FOLDER}")
+        # was this working earlier 2.2.0 ?
+        # try:
+        #    collaborations = course.get_collaborations()
+        #    list_of_cols = [c for c in collaborations]
+        #    nr_collaborations = len(list_of_collaborations)
+        # except TypeError:
+        #    nr_collaborations = None
+        md = CourseMetadata(nr_modules=nr_modules,
+                            nr_module_items=nr_module_items,
+                            nr_pages=nr_pages,
+                            nr_assignments=nr_assignments,
+                            nr_quizzes=nr_quizzes,
+                            nr_files=nr_files,
+                            assignments_summary=assignments_summary,
+                            examinations_summary=examinations_summary,
+                            examination_records=examinations
+                            )
+        return md
+
+    if MEMCACHED:
+        memc_key = f"{course_id}{hash(ignore_assignment_names)}"
+        md = MEMCACHED.get(memc_key)
+        if md:
+            return md
+        MEMCACHED.set(memc_key, md := get_md())
+        return md
+    return get_md()
+
+
+# noinspection PyTypeChecker
 class CanvasRobot(object):
-    db: callable
+    """" uses caching since """
+    db: Any
     TOT_WEIGHT: int = 100
-    year: int = AC_YEAR
-    def __init__(self, reset_api_keys=False, years_back = 0, msg_queue=None):
-        self.year = AC_YEAR - years_back
-        self.queue = msg_queue
+    _year: int = AC_YEAR  # the current academic year
+
+    def __init__(self,
+                 reset_api_keys: bool = False,
+                 msg_queue=None,
+                 console=None, # optional Rich console
+                 is_testing: bool = False,
+                 db_folder: str = "",
+                 fake_migrate_all: bool = False):
+        self.queue = msg_queue # for async use in tkinter
+        self.console = console # for commandline use
+
+        db_folder = db_folder or os.path.join(os.getcwd(), 'databases')
+        self.db = LocalDAL(is_testing=is_testing,
+                           fake_migrate_all=fake_migrate_all,
+                           folder=db_folder)
+
         config = CanvasConfig(reset_api_keys=reset_api_keys)
         self.canvas = canvasapi.Canvas(config.url, config.api_key)
+        if not self.canvas:
+            logger.error("login Canvas failed")
+            exit(1)
         self.admin = self.canvas.get_account(config.admin_id) if config.admin_id \
             else None
-        db_path = os.path.join(os.getcwd(),'databases')
-        if not os.path.exists(db_path):
-            # Create a new directory because it does not exist
-            os.makedirs(db_path)
-        self.db = LocalDAL()
         self.teacher_ids = self.lookup_teachers_db()
+
         self.internal_id = None
-        logging.info("Canvasrobot started")
-        self.errors = []
-        self.actions = []
+        self.errors: list[str] = []
+        self.actions: list[str] = []
+        logger.info("Canvasrobot instance created")
+
+    @property
+    def year(self):
+        return self._year
+
+    @year.setter
+    def year(self, year):
+        self._year = year
+
+    @property
+    def full_ac_year(self):
+        return f"{self._year}-{self._year+1}"
 
     def add_to_queue(self, msg, value):
         if self.queue:
-            self.queue.put((msg,value))
+            self.queue.put((msg, value))
+
+    def add_message(self, msg, value):
+        if self.queue:
+            self.queue.put((msg, value))
+        if self.console:
+            self.console.print(f"{msg}:{value=}" if value else msg)
     def lookup_teachers_db(self):
         db = self.db
         teachers = db((db.course2user.role == 'T') &
                       (db.course2user.user == db.user.id)).select(db.user.user_id,
                                                                   distinct=True)
         teacher_ids = [teacher.user_id for teacher in teachers]
         return teacher_ids
@@ -139,15 +303,17 @@
 
     def get_courses(self, enrollment_type: str = "teacher"):
         """"
         :enrollment_type 'teacher'(default), 'student','ta', 'observer' 'designer'
         :returns canvas courses for current user in role"""
         return self.canvas.get_courses(enrollment_type=enrollment_type)
 
-    def get_courses_in_account(self, by_teachers: list=None, this_year=True):
+    def get_courses_in_account(self,
+                               by_teachers: Optional[list] = None,
+                               this_year=True):
         """
         get all course in account here use_is has the role/type [enrollment_type]
         :param by_teachers: list of teacher id's
         :param this_year: True=filter courses to include only the current year
         :returns list of courses
         """
         assert self.admin, "No (sub) admin account provided"
@@ -171,24 +337,24 @@
         return self.canvas.get_user(user_id)
 
     @staticmethod
     def create_profile(profile_dict):
         try:
             profile = Profile(**profile_dict)
         except TypeError as e:
-            logging.error(f"attribute needs to be added to Profile class: {e}")
+            logger.error(f"attribute needs to be added to Profile class: {e}")
             raise
         return profile
 
     def get_user_profile_id(self, user_id: int):
         user = self.get_user(user_id)
         profile = self.create_profile(user.get_profile())
         return user, profile
 
-    def get_user_profile_anr(self, anr: str):
+    def get_user_profile_anr(self, anr):
         user = self.canvas.get_user(anr, 'sis_user_id')
         profile = self.create_profile(user.get_profile())
         return user, profile
 
     def is_teacher_canvas(self, user):
         """":param user """
         role_teacher = ENROLLMENT_TYPES['teacher']
@@ -214,130 +380,30 @@
             module_items = page.get_module_items()
             print("page module_items:{}".format(module_items))
             for item in module_items:
                 print(item.c)
             # print("There are {} modules in page".format(len(page)))
         return
 
-    def course_metadata(self, course_id, examination_names=None, show_candidates=False):
+    def course_metadata(self, course_id, ignore_assignment_names):
         """
         return dict with metadata of this course
         as a dict.
+        ignore the submissions of assigments present in ignore_assignment_names
+        the others are reported in assignments_summary
         :returns md: CourseMetadata"""
-        examination_names = examination_names or []
-        course = self.get_course(course_id)
-        modules = course.get_modules()
-
-        nr_modules = len(list(modules))
-        nr_module_items = 0
-        nr_ext_urls = 0
-        for module in modules:
-            # print(dir(module))
-            # print("page:{}".format(module))
-            module_items = module.get_module_items()
-            # print("page module_items:{}".format(module_items))
-            # for item in module_items:
-            #    print(item.type)
-            item_count_ext_url = filter(lambda i: i.type == "ext_url", module_items)
-            nr_ext_urls += len(list(item_count_ext_url))
-            nr_module_items += module.items_count
-        pages = course.get_pages()
-        pages = filter(lambda p: p.title[0:3] != 'UVT', pages)
-        nr_pages = len(list(pages))
-        assignments = course.get_assignments()
-        assignments_summary = "Assignments:\n"
-        examination_candidates = []
-        for assignment in assignments:
-            if assignment.name in examination_names:
-                assignments_summary += f"Examination assignment: {assignment.name}"
-            else:
-                assignments_summary += f"Examination candidate: {assignment.name}" \
-                    if show_candidates else ""
-
-                candidate = ExaminationDTO(course_id,
-                                           course.name,
-                                           assignment.name)
-
-                examination_candidates.append(candidate)
-            submissions_summary = ""
-            submissions = assignment.get_submissions()
-            try:
-                for idx, submission in enumerate(submissions, start=1):
-                    if assignment.name in examination_names:
-                        if submission.submission_type == "online_upload":
-
-                            originality_str = (f"{submission.has_originality_report}"
-                            if hasattr(submission, 'has_originality_report')
-                            else "no has_originality_report attribute!\n")
-                            submissions_summary += (f"({idx}. "
-                                                    f"{submission.submission_type}) "
-                                                    f"graded "
-                                                    f"{submission.grade} at "
-                                                    f"{submission.graded_at}. "
-                                                    f"Checked for plagiarism: "
-                                                    f"{originality_str}\n"
-                                                    )
-                        else:
-                            submissions_summary+=(f"({idx}. "
-                                                  f"{submission.submission_type}) "
-                                                  f"graded "
-                                                  f"{submission.grade} at "
-                                                  f"{submission.graded_at}\n")
-            except BaseException as exc:
-                logging.exception(f"In Course:{course_id} {course.name} "
-                                  f"Assignment {assignment.name} "
-                                  f"Submission nr {idx} "
-                                  f"type{submission.type} {exc}")
-                raise
-
-
-            assignments_summary+=f"\n{submissions_summary}"
-        nr_assignments = len(list(assignments))
-        quizzes = course.get_quizzes()
-        nr_quizzes = len(list(quizzes))
-        files = course.get_files()
-        nr_files = len(list(files))
-        # check for uploaded examination files
-        examinations_summary = ""
-        examination_files = 0
-        for file in files:
-            folder = course.get_folder(file.folder_id)
-            if f"/{EXAMINATION_FOLDER}" in folder.full_name:
-                examination_files+=1
-                examinations_summary+=f"\n{file.display_name}"
-        if examination_files == 0:
-            examinations_summary += (f"\nNo examination files in "
-                                     f"folder {EXAMINATION_FOLDER}")
-        else:
-            examinations_summary += (f"\nTotal: {examination_files} "
-                                     f"examination files")
-        # was this working earlier 2.2.0 ?
-        # try:
-        #    collaborations = course.get_collaborations()
-        #    list_of_cols = [c for c in collaborations]
-        #    nr_collaborations = len(list_of_collaborations)
-        # except TypeError:
-        #    nr_collaborations = None
-        md = CourseMetadata(nr_modules=nr_modules,
-                            nr_module_items=nr_module_items,
-                            nr_pages=nr_pages,
-                            nr_assignments=nr_assignments,
-                            nr_quizzes=nr_quizzes,
-                            nr_files=nr_files,
-                            assignments_summary=assignments_summary,
-                            examinations_summary=examinations_summary,
-                            examination_candidates=examination_candidates
-                            )
-        # examination_candidates: collect to create a canonical list
-        return md
+        ignore_assignment_names = ignore_assignment_names or []
+        result = course_metadata_memcached(course_id, self.canvas,
+                                           frozenset(ignore_assignment_names))
+        return result
 
     def enroll_in_course(self,
                          search: str,
                          course_id: int,
-                         username: str,
+                         username,
                          enrollment_type: str) -> str:
         if search:
             try:
                 course = self.get_course_using_osiris_id(search)
             except canvasapi.exceptions.ResourceDoesNotExist:
                 return f"Course {search} not found in Canvas"
         else:
@@ -363,28 +429,24 @@
         """"":returns list of all TST course canvas course """
 
         def cur_year_active(course):
             """ filter function"""
             return (str(course.sis_course_id)[:4] == str(self.year) and
                     not course.name.endswith('conclude'))
 
-        def set_id_to_course_id(course):
-            course.id = course.course_id
-            return course
-
         if from_db:
             db = self.db
             courses = db(
-                (db.course.ac_year == self.year)).select(db.course.ALL)
+                    (db.course.ac_year == self.year)).select(db.course.ALL)
             # map(set_id_to_course_id, courses)
         else:
             courses = self.admin.get_courses()
             courses = filter(cur_year_active, courses)
-        # for index, c in enumerate(courses):
-        #     print(index, c.name)
+            logger.info("Create filtered list")
+            courses = list(courses)
         return courses
 
     def get_course_using_osiris_id(self, osiris_id):
         """
         :returns first TST course with sisid starting with
         osiris_id in selected  year"""
         for course in self.admin.get_courses():
@@ -398,15 +460,15 @@
         db = self.db
         rows = db((db.course.course_code == osiris_id) &
                   (db.course.ac_year == self.year)).select(db.course.course_id)
         if rows:
             return rows[0].course_id
         return 0
 
-    def search_user(self, search_name: str, email: str = None):
+    def search_user(self, search_name: str, email: str = ""):
         """
         :param search_name:
         :param email to search on email
         try search name as a login, then the email if supplied otherwise use
         """
         try:
             user = self.canvas.get_user(search_name, 'sis_login_id')
@@ -447,31 +509,31 @@
             raise DibsaRetrieveError(f"unable to decode student data "
                                      f"of {c_name} from Dibsa @ {url} due to {e}")
 
         return result
 
     def get_students_for_community(self, c_id):
 
-        community_edu_ids = {'banl': ['banl', 'pm-ma', 'pm-ulo'],  # nl
-                             'bauk': ['bauk', 'pm-macs'],  # uk
-                             'ma': ['ma'],
-                             'ulo': ['ulo'],
-                             'macs': ['macs'],
+        community_edu_ids = {'banl'    : ['banl', 'pm-ma', 'pm-ulo'],  # nl
+                             'bauk'    : ['bauk', 'pm-macs'],  # uk
+                             'ma'      : ['ma'],
+                             'ulo'     : ['ulo'],
+                             'macs'    : ['macs'],
                              'acskills': [edu.lower() for edu in EDUCATIONS]
                              }
         # edu_ids = [edu.lower() for edu in EDUCATIONS]
         # if c_id == 'acskills' else  if c_id == 'banl' else [c_id]
         edu_ids = community_edu_ids[c_id]
         students_dibsa = []
         students_canvas = []
         for edu_id in edu_ids:
             try:
                 students_dibsa += self.get_students_dibsa(edu_id.upper())
             except DibsaRetrieveError as e:
-                logging.error(e)
+                logger.error(e)
                 raise
         for student in students_dibsa:
             username = student['username']
             user = self.search_user(username)
             if not user:
                 continue
             students_canvas.append(user)
@@ -497,15 +559,15 @@
         except (canvasapi.exceptions.BadRequest,
                 canvasapi.exceptions.Conflict):
             self.errors.append(f'User {user.name} not added to {course.name}')
         else:
             self.actions.append(f"{user.name} added to {course.name} as {role}")
         return
 
-    def add_observer_to_education(self, user, edu_id, report_only=False):
+    def add_observer_to_education(self, user):
         """ add user as an observer to all courses of an education"""
         # todo: select courses using membership of education using osiris ids
         print(user)
         # idea: filter course of an education using db
         for course in self.admin.get_courses():
             # only insert/update course if current year
             if str(course.sis_course_id)[:4] != str(self.year):
@@ -549,25 +611,25 @@
         from os.path import expanduser
 
         path = os.path.join(expanduser('~'), 'Downloads', filename + '.csv')
         db = self.db
         try:
             ofile = open(path, "rU")
         except IOError as e:
-            logging.error("{} {} not found".format(e.message, path))
+            logger.error("{} {} not found".format(e.message, path))
             raise
         else:
             reader = csv.reader(ofile, delimiter=';', quotechar='"')
             header = reader.next()
-            logging.debug(header)
+            logger.debug(header)
             # db(db.teacher.id > 0).delete()
             db(db.course2teacher.id > 0).delete()
-            # refresh all course2teacher couplings
+            # refresh all course_teacher couplings
             for row in reader:
-                logging.debug(row)
+                logger.debug(row)
                 assert len(row) == 7, "Error {0} fields!".format(len(row))
                 teacher_names = row[2].replace(' (T)',
                                                '').replace(' (U)',
                                                            '').replace(' en ',
                                                                        ', ').split(', ')
                 # phases = row[4].split(', ')
                 course_id = db.course.update_or_insert(db.course.course_base == row[0],
@@ -578,15 +640,15 @@
                                                        phase=row[4],
                                                        department=row[5],
                                                        memo=row[6])
                 if not course_id:  # must be there
                     course_id = db(db.course.course_base ==
                                    row[0]).select(db.course.id)[0].id
                 else:
-                    logging.info("course added")
+                    logger.info("course added")
                 for t_name in teacher_names:
                     teacher_id = db.teacher.update_or_insert(db.teacher.name == t_name,
                                                              name=t_name)
                     if not teacher_id:
                         teacher_id = db(db.teacher.name ==
                                         t_name).select(db.teacher.id)[0].id
                     db.course2teacher.insert(course=course_id,
@@ -639,18 +701,18 @@
         else:
             assert self.internal_id
         # we need the primary key
         try:
             bbcourse_id = db(db.bbcourse.bb_id ==
                              self.internal_id).select(db.bbcourse.id).first().id
         except AttributeError:
-            logging.info(f'course_id {self.internal_id} not found in our database!')
+            logger.info(f'course_id {self.internal_id} not found in our database!')
             return -1
 
-        logging.info(f'updating users for course_id {bbcourse_id}')
+        logger.info(f'updating users for course_id {bbcourse_id}')
         # show overview enrolled users
         self.execute_command('enrolled_users', self.internal_id)
         # assumes course is selected
         count = 0
         count_students = 0
         # connect user to this course in db
         db.commit()
@@ -671,18 +733,18 @@
                                  db.course.nr_assignments,
                                  orderby=db.course.id)
         labels = [c.course_id for c in courses]
         features = [(c.nr_modules,
                      c.nr_module_items,
                      c.nr_pages,
                      c.nr_assignments) for c in courses]
-        columns = ("nrModules", "nrModuleItems", ",nrPAges", "nr_assignments")
+        columns = ("nrModules", "nrModuleItems", ",nrPages", "nr_assignments")
         return features, labels, columns
 
-    def get_bbcourses(self, single_course=None):
+    def get_bbcourses(self, single_course: str = ""):
         """ for all courses: get coursename and other fields from db
         :param single_course: used for testing
         :return: rows/list of dicts """
 
         db = self.db  # cosmetic reasons
         suffix = '-{}-'.format(self.year)
         qry = db.bbcourse.course_suffix.contains(suffix)
@@ -705,43 +767,42 @@
                                                        count,
                                                        groupby=db.bbcourse.name,
                                                        orderby=db.bbcourse.name)
         for row in rows:
             row.count = row[count]
         return rows
 
-    def update_all_file_urls(self, max_courses=None, single_course=None):
-        # type: (int, string) -> string
+    def update_all_file_urls(self, max_courses: int = 0, single_course=None) -> str:
         """ for all courses harvest the attachments/files urls from Bb
         :param single_course: for testing
         :param max_courses:
         :returns list of found files
         """
         courses = self.get_bbcourses(single_course=single_course)
-        logging.info("{} courses to scan".format(len(courses)))
+        logger.info("{} courses to scan".format(len(courses)))
 
-        total_files = []
+        total_files: Optional[list] = []
         for count, course in enumerate(courses):
             if max_courses and count == max_courses:
-                logging.info("Stopped after {} courses".format(max_courses))
+                logger.info("Stopped after {} courses".format(max_courses))
                 break
-            logging.info("{}/{}:{}".format(count + 1, len(courses), course.name))
-            self.goto(course.bb_id)
-            areas = self.get_areas()  # top level areas (menu buttons)
-            logging.info("#{} areas#".format(len(areas)))
-            for area in areas:
-                self.goto_area(area)  # select content area
-                bb_files = self.get_files_from_area(level=0, area_name=area.name)
-                # above function is recursive
-                logging.info("{} files#".format(len(bb_files)))
-                # test_file_name = bb_files[0].fname
-                self.update_documents(bb_files)  # record data files in database
-                total_files += bb_files
+            logger.info("{}/{}:{}".format(count + 1, len(courses), course.name))
+            self.get_course(course.id)  # check this!
+            # areas = self.get_areas()  # top level areas (menu buttons)
+            # logger.info("#{} areas#".format(len(areas)))
+            # for area in areas:
+            #     self.goto_area(area)  # select content area
+            #     bb_files = self.get_files_from_area(level=0, area_name=area.name)
+            #     # above function is recursive
+            #     logger.info("{} files#".format(len(bb_files)))
+            #     # test_file_name = bb_files[0].fname
+            #     self.update_documents(bb_files)  # record data files in database
+            #     total_files += bb_files
         return "{} courses scanned {} files found".format(len(courses),
-                                                          len(total_files))
+                                                          len(total_files) if total_files else 0)
 
     # the delegates ---
     # noinspection PyRedeclaration
     def make_enroll_file(self, courseid):
         self.db.make_enroll_file(courseid)
 
     def _check_bb(self, suffix=NEXT_YEAR):
@@ -771,31 +832,31 @@
                 else:
                     db.bbdocument.update_or_insert(db.bbdocument.url == c_file.url,
                                                    url=c_file.url,
                                                    name=c_file.name,
                                                    bbcourse_id=bbcourse_id,
                                                    area=c_file.area_name)
             except Exception as e:
-                logging.error(
-                    "'{0}' error in update_documents() while inserting "
-                    "'{1}' in table Document".format(e, c_file.name))
+                logger.error(
+                        "'{0}' error in update_documents() while inserting "
+                        "'{1}' in table Document".format(e, c_file.name))
             else:
                 db.commit()
 
     def get_list_of_documents(self):
         """ get documents/attachments from db als a list
         """
         db = self.db
         suffix = '-{}-'.format(self.year)
         try:
             items = db((db.bbcourse.course_suffix.contains(suffix)) &
                        (db.bbdocument.bbcourse_id ==
                         db.bbcourse.id)).select(db.bbdocument.ALL)
         except Exception as e:
-            logging.error("*{0} error in get_list_of_ documents() "
+            logger.error("*{0} error in get_list_of_ documents() "
                           "while selecting documents*".format(e))
             return []
         else:
             return items
 
     # noinspection PyUnresolvedReferences
     def download_documents_localfs(self):
@@ -830,114 +891,144 @@
                 counters.ok += 1
             else:
                 counters.failed += 1
             db(db.bbdocument.id == item.id).update(http_status=status)
         db.commit()
         return counters
 
-    def get_examinations_from_database(self, candidate=False):
+    def get_examinations_from_database(self,
+                                       single_course=None,
+                                       orderby=None,
+                                       candidate=False):
+        """ get all assignments/examinations in the current year
+        """
         db = self.db
         # include the NULL values
-        qry = ((db.course.ac_year==self.year)&
-               (db.examination.course==db.course.course_id)& # join examination courses
-               (db.examination.candidate==
-                candidate)) if candidate else ((db.course.ac_year==self.year)&
-                                               (db.examination.course==db.course.course_id))
-        records = db( qry ).select(db.examination.ALL)
+        if single_course:
+            qry = ((db.course.course_id == single_course) &
+                   (db.examination.course == db.course.course_id) &  # join examination courses
+                   (db.examination.candidate ==
+                    candidate)) \
+                if candidate else ((db.course.course_id == single_course) &
+                                   (db.examination.course == db.course.course_id))
+        else:
+            qry = ((db.course.ac_year == self.year) &
+                   (db.examination.course == db.course.course_id) &  # join examination courses
+                   (db.examination.candidate ==
+                    candidate)) if candidate else ((db.course.ac_year == self.year) &
+                                                   (db.examination.course == db.course.course_id))
+        orderby = orderby or db.course.course_code
+        records = db(qry).select(db.examination.id,
+                                 db.examination.course,
+                                 db.examination.course_name,
+                                 db.examination.name,
+                                 db.examination.ignore,
+                                 db.course.course_code,
+                                 db.course.course_id,
+                                 orderby=orderby)
         return records
+
     def get_courses_from_database(self,
                                   skip_courses_without_students=False,
-                                  add_list=None,
                                   qry=None,
                                   orderby=None,
                                   fields=None):
         db = self.db
         if skip_courses_without_students:
-            cur_qry = (db.course.nr_students>0) &(db.course.ac_year==self.year)
+            cur_qry = (db.course.nr_students > 0) & (db.course.ac_year == self.year)
         else:
-            cur_qry = (db.course.ac_year==self.year)
-
+            cur_qry = (db.course.ac_year == self.year)
 
         if qry:
             cur_qry = cur_qry & qry
 
-
         fields = fields or db.course.ALL
-        orderby=orderby or db.course.course_code
-        records = db(cur_qry).select(db.course.ALL,
+        orderby = orderby or db.course.course_code
+        try:
+            records = db(cur_qry).select(fields,
                                      orderby=orderby)
+        except binascii.Error:
+            logger.exception("Wrong content in image field?")
+        else:
+            return records
 
-        return records
-    def get_course_from_database(self,course_id):
+    def get_course_from_database(self, course_id):
         db = self.db
-        record = db(db.course.course_id==
+        record = db(db.course.course_id ==
                     course_id).select(db.course.ALL).first()
         return record
-    def delete_course_from_database(self,course_id):
+
+    def delete_course_from_database(self, course_id):
         db = self.db
-        result = db(db.course.course_id==course_id).delete()
+        result = db(db.course.course_id == course_id).delete()
+        result2 = db(db.examination.course == course_id).delete()
         db.commit()
-        return result
+        return result and result2
 
-    def update_record_db(self, search_field, search_id, table ,field, value):
+    def update_record_db(self, qry, field, value):
 
         db = self.db
         ud_fields = {field: value}
-        #row = db(db[table][search_field] == search_id).select()
-        #row2 = db(db.course.course_id == search_id).select()
-        db(db[table][search_field] == search_id).update(**ud_fields)
+        # row = db(db[table][search_field] == search_id).select()
+        # row2 = db(db.course.course_id == search_id).select()
+        # db(db[table][search_field] == search_id).update(**ud_fields)
+        db(qry).update(**ud_fields)
         db.commit()
 
     # noinspection PyUnusedLocal
     def update_database_from_canvas(self,
                                     single_course=None,
                                     single_course_osiris_id=None,
                                     max_number=None,
                                     stop_list=None):
         """
             Using the canvasapi to read the TST courses for the selected year
-            (or a single course using canvas cours_id or osiris id) and
+            (or a single course using canvas course_id or the siris id) and
             - record internal_id course_id, fname and instructors in the
             table course
             - put teacher details in table user
             - collects info about assignments in assignment_summary
             - collects info about examinations in examination_summary
             - reports new tentamination candidates
             :return number of added/updated rows
             """
 
         db = self.db
-        msg= f'open course(s) for year {self.year} - {self.year+1}'
-        self.add_to_queue(msg, None)
-        logging.info(msg)
+        msg = f'Open single course {single_course}' \
+            if single_course \
+            else f'open course(s) for year {self.year} - {self.year + 1}'
+        self.add_message(msg, None)
+        logger.info(msg)
         num_rows = 0
         if single_course_osiris_id:
-            courses= [self.get_course_using_osiris_id(single_course_osiris_id)]
+            courses = [self.get_course_using_osiris_id(single_course_osiris_id)]
         elif single_course:
             courses = [self.get_course(single_course)]
         else:
             courses = self.admin.get_courses()
 
         num_courses = len(list(courses))
         max_number = max_number or num_courses
 
-        for idx,course in enumerate(courses):
-            self.add_to_queue("<Progress>", (course.name,idx,num_courses))
+        for idx, course in enumerate(courses):
+            self.add_message("<Progress>", (course.name, idx, num_courses))
 
             # only insert/update course if current year unless single_course
             if (str(course.sis_course_id)[:4] != str(self.year)
-                    or course.name.endswith('conclude')) and not single_course:
+                or course.name.endswith('conclude')) \
+                    and not (single_course or single_course_osiris_id):
                 continue
             if course.name in (stop_list or []):
                 continue
             if idx > max_number:
                 break
-            logging.debug("course: {}".format(course.name))  # course
-            students = course.get_users(enrollment_type="student")
-            nr_students=len(list(students))
+            logger.debug("course: {}".format(course.name))  # course
+            students = course.get_users(enrollment_type="student", )
+            # remove student with name=='Test Student'
+            nr_students = len(list(filter(lambda s: s.name != 'Test student', list(students))))
             teachers = course.get_users(enrollment_type="teacher")
             teachers_ids = []
             for teacher in teachers:
                 if not hasattr(teacher, 'login_id'):
                     continue
                 # print(teacher.name)
                 first_name, last_name, prefix = self.parse_sortable_name(teacher)
@@ -960,26 +1051,28 @@
                 teacher_logins = [teacher.login_id for teacher in teachers
                                   if hasattr(teacher, 'login_id')]
                 teacher_names = [teacher.name for teacher in teachers
                                  if hasattr(teacher, 'login_id')]
             except AttributeError as e:
                 msg = (f"skipped teacher of {course.name} "
                        f"[{course.id}] due to {e}")
-                logging.warning(msg)
+                logger.warning(msg)
                 continue
-            logging.info("instructors: {0}".format(teacher_logins))  # instructors
+            logger.info("instructors: {0}".format(teacher_logins))  # instructors
 
             inserted_id = None
             format_str = "%Y-%m-%dT%H:%M:%SZ"
             creation_date = datetime.strptime(course.created_at, format_str)
+            ignore_examinations = self.get_examinations_from_database(single_course=single_course)
+            # filter: we need only our course.id with candidate False
+            ignore_examination_names = [row.name for row in ignore_examinations
+                                        if (row.course == course.id and row.ignore)]
+            md = self.course_metadata(course.id, frozenset(ignore_examination_names))
+
             course_id = None
-            examinations = self.get_examinations_from_database(candidate=False)
-            canonical_examination_names = [row.name for row in examinations
-                                           if (row.course==course.id and not row.candidate)]
-            md = self.course_metadata(course.id, canonical_examination_names)
             try:
                 course_id = db.course.update_or_insert(db.course.course_id == course.id,
                                                        course_id=course.id,
                                                        # status=course.workflow_state,
                                                        course_code=course.course_code.split('-')[0],
                                                        sis_code=course.sis_course_id,
                                                        # year course_code and suffixes
@@ -988,47 +1081,48 @@
                                                        ac_year=self.year,
                                                        nr_students=nr_students,
                                                        nr_modules=md.nr_modules,
                                                        nr_module_items=md.nr_module_items,
                                                        nr_pages=md.nr_pages,
                                                        nr_assignments=md.nr_assignments,
                                                        nr_quizzes=md.nr_quizzes,
-                                                       assignments_summary= md.assignments_summary,
-                                                       examinations_summary = md.examinations_summary,
+                                                       assignments_summary=md.assignments_summary,
+                                                       examinations_summary=md.examinations_summary,
                                                        teachers=teacher_logins,
                                                        teachers_names=teacher_names)
+                db.commit()  # really needed here??
             except Exception as e:
                 err = f"{e} error inserting {course.name}"
-                self.add_to_queue("<InsertError>", err)
-                logging.exception(err)
+                self.add_message("<InsertError>", err)
+                logger.exception(err)
                 raise
-            if course_id:
+            if course_id:  # a new course has been inserted in the db
                 db(db.course.id == inserted_id).update(status=2)
             else:
                 course_id = db(db.course.course_id == course.id).select().first().id
-            for cand in md.examination_candidates:
+            for item in md.examination_records:
                 # candidate is True if course_name in examination_list else False
-                db.examination.update_or_insert((db.examination.course ==
-                                                 cand.course_id)&
-                                                 (db.examination.name == cand.name),
-                                                 course=cand.course_id,
-                                                 course_name=cand.course_name,
-                                                 name=cand.name,
-                                                )
+                _ = db.examination.update_or_insert((db.examination.course ==
+                                                     item.course_id) &
+                                                    (db.examination.name == item.name),
+                                                    course=item.course_id,
+                                                    course_name=item.course_name,
+                                                    name=item.name
+                                                    )
             for user_id in teachers_ids:
                 db.course2user.update_or_insert((db.course2user.course == course_id) &
                                                 (db.course2user.user == user_id),
                                                 course=course_id,
                                                 user=user_id,
                                                 role='T')
 
             db.commit()
             num_rows += 1
 
-        self.add_to_queue("<Done>",
+        self.add_message("<Done>",
                           (f"Update db from Canvas "
                            f"{single_course or max_number or 'All courses'}"))
         return num_rows
 
     def is_user_valid(self, userinfo):
         """"":param userinfo (dict or named tuple or Storage with attributes id, login_id)
              :returns True for invalid user, detail"""
@@ -1142,107 +1236,108 @@
         Goyvaert, Samuel (Sam)
         Wieringen, Archibald (H.M.J.)
         """
 
         assert ", " in user.sortable_name, "sortable_name should contain comma"
         source = user.sortable_name
         pat = re.compile(
-            r'(?P<last_name>[\w \-]+), (?P<first_name>\w+)\s?((\((?P<first_name_par>\w+)\))|'
-            r'(\((?P<init>[\w.]+.)\)))?(\s*(?P<prefix>\w+))?')
+                r'(?P<last_name>[\w \-]+), (?P<first_name>\w+)\s?((\((?P<first_name_par>\w+)\))|'
+                r'(\((?P<init>[\w.]+.)\)))?(\s*(?P<prefix>\w+))?')
         d = re.match(pat, source)
         if not d:
             print("!!!Failed parsing!!!")
 
         return d['first_name_par'] or d['first_name'], d['prefix'] or '', d['last_name']
 
     def download_file(self, url=None, fname=None):
         """download a file to static folder from url
         :param fname: local file to write to
         :param url: remote url to fetch file from
         """
         filename = 'static/' + fname.strip()
-        logging.info("creating file %s for %s" % (filename, url))
+        logger.info("creating file %s for %s" % (filename, url))
         # convert to fname/value pairs
         cookies = {}
         for cookie in self.cookies:
             cookies[str(cookie['fname'])] = cookie['value']
         with open(filename, 'wb') as outfile:
             r = requests.get(url, cookies=cookies, stream=True)
             if r.status_code == 200:
                 for block in r.iter_content(1024):
                     if not block:
                         break
                     outfile.write(block)
             else:
-                logging.info("html error %s" % r.status_code)
+                logger.info("html error %s" % r.status_code)
         return r.status_code
 
     def transfer_file_to_server(self, url=None, fname=None):
         """download a file to uploads folder from external url using a temporary buffer
         :param fname: original name of file
         :param url: remote url to fetch file from
         """
         db = self.db
         filename = fname.strip()
-        logging.debug("creating transfer buffer %s for %s" % (filename, url))
+        logger.debug("creating transfer buffer %s for %s" % (filename, url))
         # convert to fname/value pairs
         cookies = {}
         for cookie in self.cookies:
             cookies[str(cookie['fname'])] = cookie['value']
         #
-        logging.info("cookies %s for %s" % (cookies, url))
+        logger.info("cookies %s for %s" % (cookies, url))
         with io.BytesIO() as outfile:
             try:
                 r = requests.get(url, cookies=cookies, stream=True)
             except requests.exceptions.RequestException as e:
-                logging.error("couldn't get {} from file {} due to {}".format(filename,
+                logger.error("couldn't get {} from file {} due to {}".format(filename,
                                                                               url,
                                                                               e.message))
                 return None
 
             if r.status_code == 200:
                 self.receive_file(db, filename, outfile, r, url)
             else:
-                logging.info("html response {} url is now {}".format(r.status_code, r.url))
+                logger.info("html response {} url is now {}".format(r.status_code,
+                                                                    r.url))
                 # try again with redirected url (we assume redirection)
                 r = requests.get(r.url, cookies=cookies, stream=True)
                 if r.status_code == 200:
                     self.receive_file(db, filename, outfile, r, url)
                 else:
-                    logging.error('Failed {0}'.format(r))
+                    logger.error('Failed {0}'.format(r))
 
         return r.status_code
 
     @staticmethod
     def receive_file(db, filename, outfile, r, url):
-        logging.debug('Start receiving file in buffer')
+        logger.debug('Start receiving file in buffer')
         for block in r.iter_content(1024):
             if not block:
-                logging.debug('.')
+                logger.debug('.')
                 break
             outfile.write(block)
         outfile.seek(0)  # rewind
         content_type = r.headers['content-type']
         full_filename = 'undef'
         try:
             full_filename = filename + mimetypes.guess_extension(content_type) or ''
             thisfile = db.bbdocument.bbfile.store(outfile, full_filename)
         except TypeError as e:
             msg = "unable to store {} with content-type {} {}".format(filename,
                                                                       content_type,
                                                                       e.message)
-            logging.error(msg)
+            logger.error(msg)
         except IOError as e:
             msg = "unable to store {} based on {} and {} {}".format(full_filename,
                                                                     filename,
                                                                     content_type,
                                                                     e.message)
-            logging.error(msg)
+            logger.error(msg)
         else:
-            logging.info("{} should be in uploads folder...".format(full_filename))
+            logger.info("{} should be in uploads folder...".format(full_filename))
             db(db.bbdocument.url == url).update(bbfile=thisfile)
             db.commit()
 
     def course_grades(self, c_id):
         course = self.get_course(c_id)
         enrollments = course.get_enrollments()
         grades = []
@@ -1265,33 +1360,33 @@
         course, grades = self.course_grades(c_id)
 
         labels_and_types = [LabelType(label='stud_id', field_type='string'),
                             LabelType(label='stud_name', field_type='string'),
                             LabelType(label='score', field_type='percentage'),
                             LabelType(label='grade', field_type='grade')]
         styles = {
-            # list below is not complete
-            # see https://www.web2pyref.com/reference/field-type-database-field-types
-            'datetime': NamedStyle(name='date', number_format='yyyy-mm-dd'),
-            'id': NamedStyle(name='int', number_format='#,##0'),
-            'integer': NamedStyle(name='int', number_format='#,##0'),
-            'price': NamedStyle(name='money', font=Font(italic=True),
-                                fill=PatternFill(fill_type='solid', fgColor='404040'),
-                                number_format=u'[$\u20ac-1] #,##0.00 '),  # unicode for €
-            'double': NamedStyle(name='double', number_format='#0.000000'),
-            'grade': NamedStyle(name='grade', number_format='#0.00'),
-            'percentage': NamedStyle(name='score', number_format='#0.00'),
-            'string': NamedStyle(name='std',
-                                 alignment=Alignment(horizontal='left',
-                                                     vertical='bottom',
-                                                     text_rotation=0,
-                                                     wrap_text=False,
-                                                     shrink_to_fit=False,
-                                                     indent=0)),
-            'text': None
+                # list below is not complete
+                # see https://www.web2pyref.com/reference/field-type-database-field-types
+                'datetime'  : NamedStyle(name='date', number_format='yyyy-mm-dd'),
+                'id'        : NamedStyle(name='int', number_format='#,##0'),
+                'integer'   : NamedStyle(name='int', number_format='#,##0'),
+                'price'     : NamedStyle(name='money', font=Font(italic=True),
+                                         fill=PatternFill(fill_type='solid', fgColor='404040'),
+                                         number_format=u'[$\u20ac-1] #,##0.00 '),  # unicode for €
+                'double'    : NamedStyle(name='double', number_format='#0.000000'),
+                'grade'     : NamedStyle(name='grade', number_format='#0.00'),
+                'percentage': NamedStyle(name='score', number_format='#0.00'),
+                'string'    : NamedStyle(name='std',
+                                         alignment=Alignment(horizontal='left',
+                                                             vertical='bottom',
+                                                             text_rotation=0,
+                                                             wrap_text=False,
+                                                             shrink_to_fit=False,
+                                                             indent=0)),
+                'text'      : None
         }
 
         dest_filename = f'TST {course}.xlsx'
         wb = Workbook()
         ws = wb.active
         ws.page_setup.orientation = ws.ORIENTATION_LANDSCAPE
         ws.page_setup.paperSize = ws.PAPERSIZE_A4
@@ -1341,15 +1436,15 @@
         :param course_id:
         :param title:
         :param quiz_type:
         :return: msg, quiz_id
         """
         course: Course = self.get_course(course_id)
         quiz = course.create_quiz(dict(title=title, quiz_type=quiz_type))
-        logging.debug(f"{course.name} now contains {quiz}")
+        logger.debug(f"{course.name} now contains {quiz}")
         return quiz.id
 
     def create_question(self,
                         course_id: int,
                         quiz_id: int,
                         question_dto: QuestionDTO) -> int:
         """
@@ -1357,15 +1452,15 @@
         :param quiz_id:
         :param question_dto:
         :return: msg, quiz_question_id
         """
         course = self.get_course(course_id)
         quiz = course.get_quiz(quiz_id)
         quiz_question = quiz.create_question(question=asdict(question_dto))
-        logging.debug(f"{quiz} now contains {quiz_question}")
+        logger.debug(f"{quiz} now contains {quiz_question}")
         return quiz_question.id
         # return f"{quiz} now contains {quiz_question}", quiz_question.id
 
     def create_quizzes_from_data(self,
                                  course_id: int,
                                  question_format="Question {}.",
                                  data=None,
@@ -1387,17 +1482,17 @@
                    f"should contain {{}} als placeholder")
             ValueError(msg)
 
         stats = Stats()
 
         total_questions = 0
         for _, questions in data:
-            total_questions+=len(questions)
+            total_questions += len(questions)
 
-        for quiz_name, questions in track(data): # for non-gui progress
+        for quiz_name, questions in track(data):  # for non-gui progress
 
             quiz_id = self.create_quiz(course_id=course_id,
                                        title=quiz_name,
                                        quiz_type="practice_quiz")
             stats.quiz_ids.append(quiz_id)
             for index, (question_text, answers) in enumerate(questions, start=1):
                 # answers_asdict = [asdict(answer) for answer in answers]
@@ -1405,63 +1500,69 @@
                                            question_text=question_text,
                                            answers=answers)
                 question_id = self.create_question(course_id=course_id,
                                                    quiz_id=quiz_id,
                                                    question_dto=question_dto)
                 stats.question_ids.append(question_id)
             if gui_root:
-                gui_queue.put(index/total_questions)
+                gui_queue.put(index / total_questions)
                 gui_root.event_generate('<<CreateQuizzes:Progress>>')
 
         if gui_root:
             gui_root.event_generate('<<CreateQuizzes:Done>>')
 
         return stats
 
-
     def get_course_tab_by_label(self, course_id: int, label: str):
         course = self.get_course(course_id)
         for tab in course.get_tabs():
             if tab.label == label:
                 return tab
 
     def create_folder_in_course_files(self, course_id: int, foldername: str):
+        """
+        :param foldername:
+        :param course_id:
+        in course with 'course_id' create a folder 'foldername'"""
         course = self.get_course(course_id)
 
         foldernames = [f.full_name for f in course.get_folders()]
         if f"course files/{foldername}" in foldernames:
-            logging.info(f"No action needed: Folder '(course) files/{foldername}' "
-                         f"already in ({course_id})")
+            logger.info(f"No action needed: Folder '(course) files/{foldername}' "
+                         f"already in ({course_id=})")
             return -1
         folder_id = course.create_folder(foldername,
                                          parent_folder_path='/',
                                          locked=True)
-        logging.info(f"Folder '(course) files/{foldername}' should be created now")
+        logger.info(f"Folder '(course) files/{foldername}' should be created now in ({course_id=})")
         return folder_id
 
     def create_folder_in_all_courses(self, foldername):
+
         for course in track(self.get_all_active_tst_courses(from_db=False),
-                            description="All current courses..."):
+                            description="All current courses...",
+                            console=self.console):
             self.create_folder_in_course_files(course.id, foldername)
 
     def unpublish_subfolder_in_all_courses(self,
                                            foldername: str,
                                            files_too: bool = False,
                                            check_only: bool = False):
         for course in track(self.get_all_active_tst_courses(from_db=False),
                             description=(f"Checking all current"
                                          f" courses for folder '{foldername}'..." if check_only
-                            else f"Unpublish all published folder {foldername}...")):
+                            else f"Unpublish all published folder {foldername}..."),
+                            console=self.console):
             if course.name.endswith("_conclude"):
                 continue
-            # logging.info(course.name)
+            # logger.info(course.name)
             self.unpublish_folderitems_in_course(course.id,
-                                                             foldername,
-                                                             files_too,
-                                                             check_only)
+                                                 foldername,
+                                                 files_too,
+                                                 check_only)
 
     def unpublish_folderitems_in_course(self, course_id: int,
                                         foldername: str,
                                         files_too: bool = False,
                                         check_only: bool = False):
         """
         :param check_only: only show publication status no change
@@ -1477,68 +1578,68 @@
             nonlocal folder_changes
             nonlocal file_changes
             nonlocal course_id
             for folder in file_or_folder.get_folders():
                 if not folder.locked:
                     folder.update(locked=True)
                     folder_changes += 1
-                    logging.info(f"Corrected: Folder '{folder.full_name}' "
+                    logger.info(f"Corrected: Folder '{folder.full_name}' "
                                  f"is now unpublished!")
                 unpublish_items(folder)
             for file in file_or_folder.get_files():
                 if not file.locked:
                     if not check_only:
                         file_update(file, locked=True)
-                        logging.info(f"Corrected: File '{file.display_name}' in {foldername} "
+                        logger.info(f"Corrected: File '{file.display_name}' in {foldername} "
                                      f"is now unpublished")
                         file_changes += 1
                     else:
-                        logging.warning(f"File '{file.display_name}' in {foldername} is published!")
+                        logger.warning(f"File '{file.display_name}' in {foldername} is published!")
 
         # files_folder = 'course files'
         course_ids_missing_folder = []
         course = self.get_course(course_id)
         folders = course.get_folders()
         for folder in folders:  # paginated
             if folder.full_name == foldername:
                 files_tab = self.get_course_tab_by_label(course_id, "Files") or \
                             self.get_course_tab_by_label(course_id, "Bestanden")
                 try:
                     if files_tab.visibility == "public":
-                        logging.warning(f"Files folder of {course.name}"
+                        logger.warning(f"Files folder of {course.name}"
                                         f" ({course.id}) is visible")
                         # files_tab.visibility = "admins" # ! no change  without teachers approval!
                 except AttributeError:
-                    logging.warning(f"Files tab visibility of {course.name} {course_id} missing")
+                    logger.warning(f"Files tab visibility of {course.name} {course_id} missing")
 
                 # folder_id = folder.id
                 if not folder.locked:
                     if not check_only:
                         folder.update(locked=True)
                         folder_changes += 1
-                        logging.info(
-                            f"Folder '{foldername}' is now unpublished"
-                            f" in course {course.name}")
+                        logger.info(
+                                f"Folder '{foldername}' is now unpublished"
+                                f" in course {course.name}")
                     else:
-                        logging.warning(f"Folder '{foldername}' is published "
+                        logger.warning(f"Folder '{foldername}' is published "
                                         f"in course {course.name}({course.id})!")
                 else:
-                    logging.debug(
-                        f"Folder '{foldername}' was already "
-                        f"unpublished/locked in course {course.name}")
+                    logger.debug(
+                            f"Folder '{foldername}' was already "
+                            f"unpublished/locked in course {course.name}")
                 if files_too:
                     unpublish_items(folder)
                     # for f in folder.get_files():
                     #    if not f.locked:
-                    #        logging.warning(f"{f.filename} is published!")
+                    #        logger.warning(f"{f.filename} is published!")
                 break
         else:
-            logging.info(f"Folder '{foldername}' not found in {course.name}")
+            logger.info(f"Folder '{foldername}' not found in {course.name}")
             course_ids_missing_folder.append(course_id)
 
         for course_id in course_ids_missing_folder:
-            logging.info(f"Folder '{foldername}' not found in {course_id}")
+            logger.info(f"Folder '{foldername}' not found in {course_id}")
         return folder_changes, file_changes
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `canvasrobot-0.6.1/canvasrobot/canvas_robot_model.py` & `canvasrobot-0.7.0/canvasrobot/canvasrobot_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 from datetime import datetime
 import os
-
-#try:
-#    from gluon import DAL, Field, XML, HTML
-#    from gluon.storage import Storage
-#except ImportError:
-from pydal import DAL, Field, validators
+from pydal import DAL, Field, validators  # type: ignore
 import yaml
 import logging
 import logging.config
 
 from attrs import define
 import keyring
 # for UI use rich of tkinter
@@ -49,14 +44,15 @@
         for field in self.api_fields:
             value = self.get_value(field["msg"], field["key"])
             self.__setattr__(field["key"], value)
 
     def get_value(self, msg, entry):
         value = keyring.get_password(self.namespace, entry)
         if value in (None, ""):
+            # noinspection PyTypeChecker
             value = simpledialog.askstring("Input",
                                            msg,
                                            parent=self.app_window) \
                 if self.app_window else Prompt.ask(msg)
             keyring.set_password(self.namespace, entry, value)
             value = keyring.get_password(self.namespace, entry)
         return value
@@ -111,14 +107,15 @@
 AC_YEAR = now.year - 1 if now.month < 8 else now.year
 LAST_YEAR = '-{0}-{1}'.format(AC_YEAR - 1, AC_YEAR)
 THIS_YEAR = '-{0}-{1}'.format(AC_YEAR, AC_YEAR + 1)
 NEXT_YEAR = '-{0}-{1}'.format(AC_YEAR + 1, AC_YEAR + 2)
 
 EXAMINATION_FOLDER = "Tentamens"
 
+
 def load_config(default_path='ca_robot.yaml'):
     """
     Setup configuration:
     using yaml config from
     :param default_path:
     """
     path = default_path
@@ -134,22 +131,22 @@
                                     "O": "Observer",
                                     "PS": "Proctorio Surveillant",
                                     "S": "Student"})
 
 
 # noinspection PyCallingNonCallable,PyProtectedMember
 class LocalDAL(DAL):
-    def __init__(self, is_testing=False):
+    def __init__(self, is_testing=False, fake_migrate_all=False, folder="databases"):
         url = 'sqlite://testing.sqlite' if is_testing else 'sqlite://storage.sqlite'
         super(LocalDAL, self).__init__(url,
-                                       folder='databases',
+                                       folder=folder,
                                        migrate=True,
                                        migrate_enabled=True,
                                        fake_migrate=False,
-                                       fake_migrate_all=False)
+                                       fake_migrate_all=fake_migrate_all)
         self.define_table('course',
                           Field('course_id', 'integer'),
                           Field('course_code', 'string'),
                           Field('sis_code', 'string'),
                           Field('ac_year', 'string'),
                           Field('name', 'string'),
                           Field('creation_date', 'date'),
@@ -166,29 +163,34 @@
                           # Field('nr_collaborations', 'integer'),
                           Field('nr_ext_urls', 'integer'),
                           Field('assignments_summary', 'string'),
                           Field('examinations_summary', 'string'),
                           Field('examinations_ok', 'boolean', default=False),
                           Field('examinations_findings', 'string'),
                           Field('examinations_details_osiris', 'string'),
+                          Field('gradebook', 'upload', uploadfield='gradebook_file'),
+                          Field('gradebook_file', 'blob'),
                           singular='LMS course',
                           plural='LMS courses',
                           format='%(name)s[%(teacher_names)s]')
 
-        # to record a controlled set of names referring to examination assigments
+        # To record a controlled set of names referring to examination assigments
+        # We override the (sound) pyDAL principle to use course->id as reference
+        # because we need the canvas course_id for browserlinks
+        # Note that Pydal create a foreign key to course->id we need to change using DBrowser
         self.define_table('examination',
                           Field('course',
                                 'reference course',
                                 requires=validators.IS_IN_DB(self, 'course.course_id',
                                                              self.course._format)),
-                          Field('course_name', 'string'), # a bit redundant
+                          Field('course_name', 'string'),  # a bit redundant
                           Field('name', 'string'),
-                          Field('candidate', 'boolean',
-                                label="Only Examination when False",
-                                default=True),
+                          Field('ignore', 'boolean',
+                                label="Skip unused/unusable assignments",
+                                default=False),
                           format='%(name)s',
                           singular='Examination name',
                           plural='Examination names')
 
         self.define_table('user',
                           Field('user_id', 'integer'),
                           Field('username', 'string'),
@@ -221,15 +223,15 @@
 
         self.define_table('submission',
                           Field('submission_id', 'integer'),
                           Field('assigment_id', 'integer'),
                           Field('course_id', 'integer'),
                           Field('user_id', 'integer'),
                           Field('submission_type', 'string'),
-                          Field('url','string'),
+                          Field('url', 'string'),
                           Field('grade', 'string'),
                           Field('graded_at', 'string'),
                           format='%(submission_id)s-%(assigment_id)s %(user_id)s',
                           singular='Submission',
                           plural='Submissions')
 
         self.define_table('document',
```

### Comparing `canvasrobot-0.6.1/canvasrobot/entities/course.py` & `canvasrobot-0.7.0/canvasrobot/entities/course.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,36 +26,36 @@
 
 @define
 class SearchTextInCourseDTO:
     course_id: int = 0
     course: str = ""
     search: str = ""
 
+@define
+class ExaminationDTO:
+    course_id: int
+    course_name: str
+    name:str
 
 @define
 class CourseMetadata:
     nr_modules: int
     nr_module_items: int
     nr_pages: int
     nr_assignments: int
     nr_quizzes: int
     nr_files: int
     assignments_summary: str
     examinations_summary: str
-    examination_candidates: str
+    examination_records: list[ExaminationDTO]
     # nr_collaborations: int
 
     # #ext_urls: int
     # avr_len_assignments: int
 
 @define
 class Grade:
     stud_name: str
     stud_id: str
     final_score: float
     final_grade: float
 
-@define
-class ExaminationDTO:
-    course_id: int
-    course_name: str
-    name:str
```

### Comparing `canvasrobot-0.6.1/canvasrobot/entities/guest.py` & `canvasrobot-0.7.0/canvasrobot/entities/guest.py`

 * *Files identical despite different names*

### Comparing `canvasrobot-0.6.1/canvasrobot/entities/quiz.py` & `canvasrobot-0.7.0/canvasrobot/entities/quiz.py`

 * *Files identical despite different names*

### Comparing `canvasrobot-0.6.1/canvasrobot/entities/user.py` & `canvasrobot-0.7.0/canvasrobot/entities/user.py`

 * *Files identical despite different names*

### Comparing `canvasrobot-0.6.1/pyproject.toml` & `canvasrobot-0.7.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "canvasrobot"
-version = "0.6.1"
+version = "0.7.0"
 description = "Library which uses Canvasapi https://canvasapi.readthedocs.io/en/stable/getting-started.html to provide a CanvasRobot class."
 authors = ["Nico de Groot <ndegroot0@gmail.com>",]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0.0"
 requests = "~=2.28.1"
@@ -14,17 +14,21 @@
 pydal = "*"
 rich = "*"
 toml = "*"
 keyring = "*"
 
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.3"
+pytest = "*"
 mock = "*"
 pylint = "*"
 ruff = "*"
-#
+pymemcache = "*"
+mypy = "*"
+types-requests = "*"
+types-pyyaml = "*"
+
 [tool.poetry_bumpversion.file."canvasrobot/__init__.py"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `canvasrobot-0.6.1/PKG-INFO` & `canvasrobot-0.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvasrobot
-Version: 0.6.1
+Version: 0.7.0
 Summary: Library which uses Canvasapi https://canvasapi.readthedocs.io/en/stable/getting-started.html to provide a CanvasRobot class.
 Author: Nico de Groot
 Author-email: ndegroot0@gmail.com
 Requires-Python: >=3.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

