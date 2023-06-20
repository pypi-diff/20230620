# Comparing `tmp/sqlalchemy_celery_beat-0.5.1.tar.gz` & `tmp/sqlalchemy_celery_beat-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_celery_beat-0.5.1.tar", last modified: Sun Jun 18 04:43:57 2023, max compression
+gzip compressed data, was "sqlalchemy_celery_beat-0.6.0.tar", last modified: Tue Jun 20 07:57:12 2023, max compression
```

## Comparing `sqlalchemy_celery_beat-0.5.1.tar` & `sqlalchemy_celery_beat-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 04:43:57.417286 sqlalchemy_celery_beat-0.5.1/
--rw-rw-rw-   0        0        0     1093 2023-06-15 09:28:10.000000 sqlalchemy_celery_beat-0.5.1/LICENSE
--rw-rw-rw-   0        0        0    10573 2023-06-18 04:43:57.416284 sqlalchemy_celery_beat-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     9602 2023-06-18 04:42:43.000000 sqlalchemy_celery_beat-0.5.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-18 04:43:57.417286 sqlalchemy_celery_beat-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     3138 2023-06-18 04:43:11.000000 sqlalchemy_celery_beat-0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 04:43:57.380286 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/
--rw-rw-rw-   0        0        0      455 2023-06-18 04:43:14.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/__init__.py
--rw-rw-rw-   0        0        0     1317 2023-06-15 13:54:09.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/clockedschedule.py
--rw-rw-rw-   0        0        0    12367 2023-06-18 04:28:22.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/models.py
--rw-rw-rw-   0        0        0    16270 2023-06-18 03:12:47.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/schedulers.py
--rw-rw-rw-   0        0        0     4171 2023-06-18 04:09:09.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/session.py
--rw-rw-rw-   0        0        0     1323 2023-06-15 13:53:44.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/time_utils.py
--rw-rw-rw-   0        0        0     2766 2023-06-15 09:08:15.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/tzcrontab.py
-drwxrwxrwx   0        0        0        0 2023-06-18 04:43:57.414284 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat.egg-info/
--rw-rw-rw-   0        0        0    10573 2023-06-18 04:43:57.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      603 2023-06-18 04:43:57.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 04:43:57.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-06-18 04:43:57.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-15 17:41:10.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-06-18 04:43:57.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-06-18 04:43:57.000000 sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 07:57:12.961323 sqlalchemy_celery_beat-0.6.0/
+-rw-rw-rw-   0        0        0     1093 2023-06-15 09:28:10.000000 sqlalchemy_celery_beat-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0    10599 2023-06-20 07:57:12.960348 sqlalchemy_celery_beat-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9627 2023-06-20 07:42:22.000000 sqlalchemy_celery_beat-0.6.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-20 07:57:12.961323 sqlalchemy_celery_beat-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     3156 2023-06-20 07:55:14.000000 sqlalchemy_celery_beat-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:57:12.919325 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/
+-rw-rw-rw-   0        0        0      455 2023-06-20 07:55:05.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/__init__.py
+-rw-rw-rw-   0        0        0     1317 2023-06-15 13:54:09.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/clockedschedule.py
+-rw-rw-rw-   0        0        0    20425 2023-06-20 07:52:42.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/models.py
+-rw-rw-rw-   0        0        0    16354 2023-06-20 07:52:42.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/schedulers.py
+-rw-rw-rw-   0        0        0     4171 2023-06-19 07:50:11.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/session.py
+-rw-rw-rw-   0        0        0     1323 2023-06-15 13:53:44.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/time_utils.py
+-rw-rw-rw-   0        0        0     2766 2023-06-20 02:26:17.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/tzcrontab.py
+drwxrwxrwx   0        0        0        0 2023-06-20 07:57:12.957372 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat.egg-info/
+-rw-rw-rw-   0        0        0    10599 2023-06-20 07:57:12.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      603 2023-06-20 07:57:12.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 07:57:12.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-06-20 07:57:12.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-15 17:41:10.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-06-20 07:57:12.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-20 07:57:12.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat.egg-info/top_level.txt
```

### Comparing `sqlalchemy_celery_beat-0.5.1/LICENSE` & `sqlalchemy_celery_beat-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.5.1/PKG-INFO` & `sqlalchemy_celery_beat-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy_celery_beat
-Version: 0.5.1
+Version: 0.6.0
 Summary: A Scheduler Based SQLalchemy For Celery
 Home-page: https://github.com/farahats9/sqlalchemy-celery-beat
 Author: Mohamed Farahat
 Author-email: farahats9@yahoo.com
 License: MIT
 Keywords: celery scheduler sqlalchemy beat
 Platform: any
@@ -291,15 +291,16 @@
 
         $ celery -A [project-name] beat -l info --scheduler sqlalchemy_celery_beat.schedulers:DatabaseScheduler
 
 ## Working on adding the following features
 
 - ✅ Add `ClockedSchedule` model
 - ✅ Implement a generic foreign key
-- More robust attribute validation on models
+- ✅ More robust attribute validation on models
+- Add more examples
 - Add Tests
 - Support for Async drivers like asyncpg and psycopg3 async mode
 - Use Alembic migrations
 
 Any help with the tasks above or feedback is appreciated 🙂
 
 ## Acknowledgments
```

### Comparing `sqlalchemy_celery_beat-0.5.1/README.md` & `sqlalchemy_celery_beat-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,16 @@
 
         $ celery -A [project-name] beat -l info --scheduler sqlalchemy_celery_beat.schedulers:DatabaseScheduler
 
 ## Working on adding the following features
 
 - ✅ Add `ClockedSchedule` model
 - ✅ Implement a generic foreign key
-- More robust attribute validation on models
+- ✅ More robust attribute validation on models
+- Add more examples
 - Add Tests
 - Support for Async drivers like asyncpg and psycopg3 async mode
 - Use Alembic migrations
 
 Any help with the tasks above or feedback is appreciated 🙂
 
 ## Acknowledgments
```

### Comparing `sqlalchemy_celery_beat-0.5.1/setup.py` & `sqlalchemy_celery_beat-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 setup(
     name="sqlalchemy_celery_beat",
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.5.1",
+    version="0.6.0",
     # The project's main homepage.
     url="https://github.com/farahats9/sqlalchemy-celery-beat",
     # Choose your license
 
     license='MIT',
 
     description="A Scheduler Based SQLalchemy For Celery",
@@ -80,11 +80,12 @@
         'celery.beat_schedulers': [
             'sqlalchemy = sqlalchemy_celery_beat.schedulers:DatabaseScheduler',
         ],
     },
     install_requires=[
         'celery>=5.0',
         'sqlalchemy>=1.4',
-        'tzdata'
+        'tzdata',
+        'ephem'
     ],
     zip_safe=False,
 )
```

### Comparing `sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/clockedschedule.py` & `sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/clockedschedule.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/models.py` & `sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/models.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,67 @@
 # coding=utf-8
 # The generic foreign key is implemented after this example:
 # https://docs.sqlalchemy.org/en/20/_modules/examples/generic_associations/generic_fk.html
+import re
 import datetime as dt
 from typing import Any
 from zoneinfo import ZoneInfo
-
+try:
+    from zoneinfo import available_timezones
+except ImportError:
+    from backports.zoneinfo import available_timezones
+import enum
 import sqlalchemy as sa
 from celery import schedules
 from celery.utils.log import get_logger
-from sqlalchemy import event, func
+from sqlalchemy import event
 from sqlalchemy.future import Connection
 from sqlalchemy.orm import (Session, backref, foreign, relationship, remote,
                             validates)
 from sqlalchemy.sql import insert, select, update
 
 from .clockedschedule import clocked
 from .session import ModelBase
 from .tzcrontab import TzAwareCrontab
 
 logger = get_logger('sqlalchemy_celery_beat.models')
 
 
-def cronexp(field):
-    """Representation of cron expression."""
-    return field and str(field).replace(' ', '') or '*'
-
-
 class ModelMixin(object):
 
     @classmethod
     def create(cls, **kw):
         return cls(**kw)
 
     def update(self, **kw):
         for attr, value in kw.items():
             setattr(self, attr, value)
         return self
 
 
+class Period(str, enum.Enum):
+    DAYS = 'days'
+    HOURS = 'hours'
+    MINUTES = 'minutes'
+    SECONDS = 'seconds'
+    MICROSECONDS = 'microseconds'
+
+
+class SolarEvent(str, enum.Enum):
+    DAWN_ASTRONOMICAL = 'dawn_astronomical'
+    DAWN_CIVIL = 'dawn_civil'
+    DAWN_NAUTICAL = 'dawn_nautical'
+    DUSK_ASTRONOMICAL = 'dusk_astronomical'
+    DUSK_CIVIL = 'dusk_civil'
+    DUSK_NAUTICAL = 'dusk_nautical'
+    SOLAR_NOON = 'solar_noon'
+    SUNRISE = 'sunrise'
+    SUNSET = 'sunset'
+
+
 class PeriodicTaskChanged(ModelBase, ModelMixin):
     """Helper table for tracking updates to periodic tasks."""
     __table_args__ = {
         'sqlite_autoincrement': False,
         'schema': 'celery_schema'
     }
 
@@ -93,47 +113,98 @@
         periodic_tasks = session.query(PeriodicTaskChanged).get(1)
         if periodic_tasks:
             return periodic_tasks.last_update
 
 
 class PeriodicTask(ModelBase, ModelMixin):
 
+    __table_args__ = (
+        sa.CheckConstraint(sa.column('priority').between(0, 255)),
+        {
+            'sqlite_autoincrement': True,
+            'schema': 'celery_schema'
+        }
+    )
+
     id = sa.Column(sa.Integer, primary_key=True, autoincrement=True)
     # name
-    name = sa.Column(sa.String(255), unique=True)
+    name = sa.Column(sa.String(255), unique=True, nullable=False,
+                     doc='Name',
+                     comment='Short Description For This Task')
     # task name
-    task = sa.Column(sa.String(255))
-
-    args = sa.Column(sa.Text(), default='[]')
-    kwargs = sa.Column(sa.Text(), default='{}')
+    task = sa.Column(sa.String(255), nullable=False,
+                     doc='Task Name',
+                     comment='The Name of the Celery Task that Should be Run.  '
+                     '(Example: "proj.tasks.import_contacts")')
+
+    args = sa.Column(sa.Text(), default='[]', nullable=False,
+                     doc='Positional Arguments',
+                     comment='JSON encoded positional arguments '
+                     '(Example: ["arg1", "arg2"])')
+    kwargs = sa.Column(sa.Text(), default='{}', nullable=False,
+                       doc='Keyword Arguments',
+                       comment='JSON encoded keyword arguments '
+                       '(Example: {"argument": "value"})')
     # queue for celery
-    queue = sa.Column(sa.String(255))
+    queue = sa.Column(sa.String(255),
+                      doc='Queue Override',
+                      comment='Queue defined in CELERY_TASK_QUEUES. '
+                      'Leave None for default queuing.')
     # exchange for celery
-    exchange = sa.Column(sa.String(255))
+    exchange = sa.Column(sa.String(255), doc='Exchange',
+                         comment='Override Exchange for low-level AMQP routing')
     # routing_key for celery
-    routing_key = sa.Column(sa.String(255))
-    priority = sa.Column(sa.Integer())
-    expires = sa.Column(sa.DateTime(timezone=True))
-
-    one_off = sa.Column(sa.Boolean(), default=False)
-    start_time = sa.Column(sa.DateTime(timezone=True))
-    enabled = sa.Column(sa.Boolean(), default=True)
-    last_run_at = sa.Column(sa.DateTime(timezone=True))
-    total_run_count = sa.Column(sa.Integer(), nullable=False, default=0)
+    routing_key = sa.Column(sa.String(255), doc='Routing Key',
+                            comment='Override Routing Key for low-level AMQP routing')
+    headers = sa.Column(sa.Text,
+                        default='{}',
+                        doc='AMQP Message Headers',
+                        comment='JSON encoded message headers for the AMQP message.',
+                        )
+    priority = sa.Column(sa.Integer(),
+                         doc='Priority',
+                         comment='Priority Number between 0 and 255. '
+                         'Supported by: RabbitMQ, Redis (priority reversed, 0 is highest).')
+    expires = sa.Column(sa.DateTime(timezone=True),
+                        doc='Expires Datetime',
+                        comment='Datetime after which the schedule will no longer '
+                        'trigger the task to run')
+
+    one_off = sa.Column(sa.Boolean(), default=False, nullable=False,
+                        doc='One-off Task',
+                        comment='If True, the schedule will only run the task a single time')
+    start_time = sa.Column(sa.DateTime(timezone=True),
+                           doc='Start Datetime',
+                           comment='Datetime when the schedule should begin '
+                           'triggering the task to run')
+    enabled = sa.Column(sa.Boolean(), default=True, nullable=False,
+                        doc='Enabled',
+                        comment='Set to False to disable the schedule')
+    last_run_at = sa.Column(sa.DateTime(timezone=True), doc='Last Run Datetime',
+                            comment='Datetime that the schedule last triggered the task to run. ')
+    total_run_count = sa.Column(sa.Integer(), nullable=False, default=0,
+                                doc='Total Run Count',
+                                comment='Running count of how many times the schedule '
+                                'has triggered the task')
 
     date_changed = sa.Column(sa.DateTime(timezone=True),
-                             default=dt.datetime.now, onupdate=dt.datetime.now)
-    description = sa.Column(sa.Text(), default='')
+                             default=dt.datetime.now, onupdate=dt.datetime.now,
+                             doc='Last Modified',
+                             comment='Datetime that this PeriodicTask was last modified')
+    description = sa.Column(sa.Text(), default='', doc='Description',
+                            comment='Detailed description about the details of this Periodic Task')
 
     no_changes = False
 
-    discriminator = sa.Column(sa.String(50), nullable=False)
+    discriminator = sa.Column(sa.String(20), nullable=False, doc='Schedule Name',
+                              comment='Lower case name of the schedule class. ')
     """Refers to the type of parent."""
 
-    schedule_id = sa.Column(sa.Integer(), nullable=False)
+    schedule_id = sa.Column(sa.Integer(), nullable=False, doc='Schedule ID',
+                            comment='ID of the schedule model object. ')
     """Refers to the primary key of the parent.
 
     This could refer to any table.
     """
     @property
     def schedule_model(self):
         """Provides in-Python access to the "parent" by choosing
@@ -145,17 +216,17 @@
     @schedule_model.setter
     def schedule_model(self, value):
         if value is not None:
             self.schedule_id = value.id
             self.discriminator = value.discriminator
             setattr(self, "model_%s" % value.discriminator, value)
 
-    @classmethod
-    def validate_before_insert(cls, mapper, connection, target):
-        if isinstance(target.schedule_model, ClockedSchedule) and not target.one_off:
+    @staticmethod
+    def before_insert_or_update(mapper, connection, target):
+        if target.enabled and isinstance(target.schedule_model, ClockedSchedule) and not target.one_off:
             raise ValueError("one_off must be True for clocked schedule")
 
     def __repr__(self):
         fmt = '{0.name}: {0.schedule_model}'
         return fmt.format(self)
 
     @property
@@ -210,24 +281,37 @@
         return self.__class__.__name__.lower()
 
     class_.discriminator = get_discriminator
 
 
 class IntervalSchedule(ScheduleModel, ModelBase):
 
-    DAYS = 'days'
-    HOURS = 'hours'
-    MINUTES = 'minutes'
-    SECONDS = 'seconds'
-    MICROSECONDS = 'microseconds'
+    __table_args__ = (
+        sa.CheckConstraint(sa.column('every') >= 1),
+        {
+            'sqlite_autoincrement': True,
+            'schema': 'celery_schema'
+        }
+    )
 
     id = sa.Column(sa.Integer, primary_key=True, autoincrement=True)
 
-    every = sa.Column(sa.Integer, nullable=False)
-    period = sa.Column(sa.String(24))
+    every = sa.Column(
+        sa.Integer,
+        nullable=False,
+        doc='Number of Periods',
+        comment='Number of interval periods to wait before '
+        'running the task again'
+    )
+    period = sa.Column(
+        sa.Enum(Period, values_callable=lambda obj: [e.value for e in obj]),
+        nullable=False,
+        doc='Interval Period',
+        comment='The type of period between task runs (Example: days)'
+    )
 
     def __repr__(self):
         if self.every == 1:
             return 'every {0}'.format(self.period_singular)
         return 'every {0} {1}'.format(self.every, self.period)
 
     @property
@@ -235,15 +319,15 @@
         return schedules.schedule(
             dt.timedelta(**{self.period: self.every}),
             # nowfun=lambda: make_aware(now())
             # nowfun=dt.datetime.now
         )
 
     @classmethod
-    def from_schedule(cls, session, schedule, period=SECONDS):
+    def from_schedule(cls, session, schedule, period=Period.SECONDS):
         every = max(schedule.run_every.total_seconds(), 0)
         model = session.query(IntervalSchedule).filter_by(
             every=every, period=period).first()
         if not model:
             model = cls(every=every, period=period)
             session.add(model)
             session.commit()
@@ -253,66 +337,157 @@
     def period_singular(self):
         return self.period[:-1]
 
 
 class CrontabSchedule(ScheduleModel, ModelBase):
 
     id = sa.Column(sa.Integer, primary_key=True, autoincrement=True)
-    minute = sa.Column(sa.String(60 * 4), default='*')
-    hour = sa.Column(sa.String(24 * 4), default='*')
-    day_of_week = sa.Column(sa.String(64), default='*')
-    day_of_month = sa.Column(sa.String(31 * 4), default='*')
-    month_of_year = sa.Column(sa.String(64), default='*')
-    timezone = sa.Column(sa.String(64), default='UTC')
+    minute = sa.Column(
+        sa.String(60 * 4),
+        nullable=False,
+        default='*',
+        doc='Minute(s)',
+        comment='Cron Minutes to Run. Use "*" for "all". (Example: "0,30")'
+    )
+    hour = sa.Column(
+        sa.String(24 * 4),
+        nullable=False,
+        default='*',
+        doc='Hour(s)',
+        comment='Cron Hours to Run. Use "*" for "all". (Example: "8,20")'
+    )
+    day_of_week = sa.Column(
+        sa.String(64),
+        nullable=False,
+        default='*',
+        doc='Day(s) Of The Week',
+        comment='Cron Days Of The Week to Run. Use "*" for "all", Sunday '
+        'is 0 or 7, Monday is 1. (Example: "0,5")'
+    )
+    day_of_month = sa.Column(
+        sa.String(31 * 4),
+        nullable=False,
+        default='*',
+        doc='Day(s) Of The Month',
+        comment='Cron Days Of The Month to Run. Use "*" for "all". '
+        '(Example: "1,15")'
+    )
+    month_of_year = sa.Column(
+        sa.String(64),
+        nullable=False,
+        default='*',
+        doc='Month(s) Of The Year',
+        comment='Cron Months (1-12) Of The Year to Run. Use "*" for "all". '
+        '(Example: "1,12")'
+    )
+    timezone = sa.Column(
+        sa.String(64),
+        nullable=False,
+        default='UTC',
+        doc='Cron Timezone',
+        comment='Timezone to Run the Cron Schedule on. Default is UTC.'
+    )
 
     def __repr__(self):
         return '{0} {1} {2} {3} {4} (m/h/d/dM/MY) {5}'.format(
-            cronexp(self.minute), cronexp(self.hour),
-            cronexp(self.day_of_week), cronexp(self.day_of_month),
-            cronexp(self.month_of_year), str(self.timezone)
+            self.cronexp(self.minute), self.cronexp(self.hour),
+            self.cronexp(self.day_of_week), self.cronexp(self.day_of_month),
+            self.cronexp(self.month_of_year), str(self.timezone)
         )
 
-    @property
-    def schedule(self):
+    @staticmethod
+    def aware_crontab(obj):
         return TzAwareCrontab(
-            minute=self.minute,
-            hour=self.hour, day_of_week=self.day_of_week,
-            day_of_month=self.day_of_month,
-            month_of_year=self.month_of_year,
-            tz=ZoneInfo(self.timezone)
+            minute=obj.minute,
+            hour=obj.hour, day_of_week=obj.day_of_week,
+            day_of_month=obj.day_of_month,
+            month_of_year=obj.month_of_year,
+            tz=ZoneInfo(obj.timezone)
         )
 
+    @property
+    def schedule(self):
+        return self.aware_crontab(self)
+
+    @staticmethod
+    def cronexp(value):
+        return value and re.sub(r"[\s\[\]\{\}]", '', str(value))
+
     @classmethod
     def from_schedule(cls, session, schedule):
         spec = {
-            'minute': schedule._orig_minute,
-            'hour': schedule._orig_hour,
-            'day_of_week': schedule._orig_day_of_week,
-            'day_of_month': schedule._orig_day_of_month,
-            'month_of_year': schedule._orig_month_of_year,
+            'minute': cls.cronexp(schedule._orig_minute),
+            'hour': cls.cronexp(schedule._orig_hour),
+            'day_of_week': cls.cronexp(schedule._orig_day_of_week),
+            'day_of_month': cls.cronexp(schedule._orig_day_of_month),
+            'month_of_year': cls.cronexp(schedule._orig_month_of_year),
         }
         if schedule.tz:
             spec.update({
                 'timezone': schedule.tz.key
             })
         model = session.query(CrontabSchedule).filter_by(**spec).first()
         if not model:
             model = cls(**spec)
             session.add(model)
             session.commit()
         return model
 
+    @staticmethod
+    def before_insert_or_update(mapper, connection, target):
+        try:
+            # Test the object to make sure it is valid before saving to DB
+            CrontabSchedule.aware_crontab(target).remaining_estimate(dt.datetime.now())
+        except Exception as exc:
+            raise ValueError(f"Could not parse cron values: {str(exc)}") from exc
+
+    @validates('timezone')
+    def validate_crontab(self, key, value):
+        if value not in available_timezones():
+            raise ValueError(f'Timezone "{value}"  is not found in available timezones')
+        return value
+
+    @validates('minute', 'hour', 'day_of_week', 'day_of_month', 'month_of_year')
+    def validate_values(self, key, value):
+        value = self.cronexp(value)
+        return value
+
 
 class SolarSchedule(ScheduleModel, ModelBase):
 
+    __table_args__ = (
+        sa.UniqueConstraint('event', 'latitude', 'longitude'),
+        sa.CheckConstraint(sa.column('latitude').between(-90, 90)),
+        sa.CheckConstraint(sa.column('longitude').between(-180, 180)),
+        {
+            'sqlite_autoincrement': True,
+            'schema': 'celery_schema'
+        }
+    )
+
     id = sa.Column(sa.Integer, primary_key=True, autoincrement=True)
 
-    event = sa.Column(sa.String(24))
-    latitude = sa.Column(sa.Float())
-    longitude = sa.Column(sa.Float())
+    event = sa.Column(
+        sa.Enum(SolarEvent, values_callable=lambda obj: [e.value for e in obj]),
+        nullable=False,
+        doc='Solar Event',
+        comment='The type of solar event when the job should run'
+    )
+    latitude = sa.Column(
+        sa.Numeric(precision=9, scale=6, decimal_return_scale=6, asdecimal=False),
+        nullable=False,
+        doc='Latitude',
+        comment='Run the task when the event happens at this latitude'
+    )
+    longitude = sa.Column(
+        sa.Numeric(precision=9, scale=6, decimal_return_scale=6, asdecimal=False),
+        nullable=False,
+        doc='Longitude',
+        comment='Run the task when the event happens at this longitude'
+    )
 
     @property
     def schedule(self):
         return schedules.solar(
             self.event,
             self.latitude,
             self.longitude,
@@ -360,14 +535,30 @@
         model = session.query(ClockedSchedule).filter_by(**spec).first()
         if not model:
             model = cls(**spec)
             session.add(model)
             session.commit()
         return model
 
+    def strip_ms(self):
+        """ Convenience function to remove microseconds,
+        this should help reduce number of clockedschedules in DB
+        if you have too many.
+        ex:
+            s = ClockedSchedule(clocked_time=datetime.now() + timedelta(hours=1))
+            # now your clocked_time looks like this: 2023-06-19 03:20:23.807020
+            s.strip_ms()
+            # now your clocked_time looks like this: 2023-06-19 03:20:23.000000
+            session.add(s)
+        """
+        self.clocked_time = self.clocked_time.replace(microsecond=0)
+
 
 event.listen(PeriodicTask, 'after_insert', PeriodicTaskChanged.update_changed)
 event.listen(PeriodicTask, 'after_delete', PeriodicTaskChanged.update_changed)
 event.listen(PeriodicTask, 'after_update', PeriodicTaskChanged.changed)
-event.listen(PeriodicTask, 'before_insert', PeriodicTask.validate_before_insert)
+event.listen(PeriodicTask, 'before_insert', PeriodicTask.before_insert_or_update)
+event.listen(PeriodicTask, 'before_update', PeriodicTask.before_insert_or_update)
 event.listen(ScheduleModel, 'after_delete', PeriodicTaskChanged.update_changed, propagate=True)
 event.listen(ScheduleModel, 'after_update', PeriodicTaskChanged.update_changed, propagate=True)
+event.listen(CrontabSchedule, 'before_insert', CrontabSchedule.before_insert_or_update)
+event.listen(CrontabSchedule, 'before_update', CrontabSchedule.before_insert_or_update)
```

### Comparing `sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/schedulers.py` & `sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/schedulers.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     )
     save_fields = ['last_run_at', 'total_run_count', 'no_changes']
 
     def __init__(self, model, Session, app=None, **kw):
         """Initialize the model entry."""
         self.app = app or current_app._get_current_object()
         self.Session = Session
-        self.model = model
         self.name = model.name
         self.task = model.task
         try:
             self.schedule = model.schedule
             logger.debug('schedule: {}'.format(self.schedule))
         except Exception as e:
             logger.error(e)
@@ -83,30 +82,33 @@
         for option in ['queue', 'exchange', 'routing_key', 'expires',
                        'priority']:
             value = getattr(model, option)
             if value is None:
                 continue
             self.options[option] = value
 
+        self.options['headers'] = loads(model.headers or '{}')
+        self.options['periodic_task_name'] = model.name
+
         self.total_run_count = model.total_run_count
-        self.enabled = model.enabled
+        self.model = model
 
         if not model.last_run_at:
             model.last_run_at = self._default_now()
             # if last_run_at is not set and
             # model.start_time last_run_at should be in way past.
             # This will trigger the job to run at start_time
             # and avoid the heap block.
             if self.model.start_time:
                 model.last_run_at = model.last_run_at \
                     - dt.timedelta(days=365 * 30)
 
         self.last_run_at = model.last_run_at
 
-        # Because the last_run_at read from the database may not have time zone information, 
+        # Because the last_run_at read from the database may not have time zone information,
         # so time zone information must be added here
         self.last_run_at = self.last_run_at.replace(tzinfo=self.app.timezone)
 
         # self.options['expires']
         # if 'expires' in self.options:
         #     expires = self.options['expires']
         #     self.options['expires'] = expires.replace(tzinfo=self.app.timezone)
```

### Comparing `sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/session.py` & `sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/session.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/time_utils.py` & `sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/time_utils.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat/tzcrontab.py` & `sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/tzcrontab.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat.egg-info/PKG-INFO` & `sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-celery-beat
-Version: 0.5.1
+Version: 0.6.0
 Summary: A Scheduler Based SQLalchemy For Celery
 Home-page: https://github.com/farahats9/sqlalchemy-celery-beat
 Author: Mohamed Farahat
 Author-email: farahats9@yahoo.com
 License: MIT
 Keywords: celery scheduler sqlalchemy beat
 Platform: any
@@ -291,15 +291,16 @@
 
         $ celery -A [project-name] beat -l info --scheduler sqlalchemy_celery_beat.schedulers:DatabaseScheduler
 
 ## Working on adding the following features
 
 - ✅ Add `ClockedSchedule` model
 - ✅ Implement a generic foreign key
-- More robust attribute validation on models
+- ✅ More robust attribute validation on models
+- Add more examples
 - Add Tests
 - Support for Async drivers like asyncpg and psycopg3 async mode
 - Use Alembic migrations
 
 Any help with the tasks above or feedback is appreciated 🙂
 
 ## Acknowledgments
```

### Comparing `sqlalchemy_celery_beat-0.5.1/sqlalchemy_celery_beat.egg-info/SOURCES.txt` & `sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

