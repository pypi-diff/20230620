# Comparing `tmp/sqlalchemy_celery_beat-0.6.0.tar.gz` & `tmp/sqlalchemy_celery_beat-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_celery_beat-0.6.0.tar", last modified: Tue Jun 20 07:57:12 2023, max compression
+gzip compressed data, was "sqlalchemy_celery_beat-0.6.1.tar", last modified: Tue Jun 20 14:58:41 2023, max compression
```

## Comparing `sqlalchemy_celery_beat-0.6.0.tar` & `sqlalchemy_celery_beat-0.6.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 07:57:12.961323 sqlalchemy_celery_beat-0.6.0/
--rw-rw-rw-   0        0        0     1093 2023-06-15 09:28:10.000000 sqlalchemy_celery_beat-0.6.0/LICENSE
--rw-rw-rw-   0        0        0    10599 2023-06-20 07:57:12.960348 sqlalchemy_celery_beat-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     9627 2023-06-20 07:42:22.000000 sqlalchemy_celery_beat-0.6.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-20 07:57:12.961323 sqlalchemy_celery_beat-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     3156 2023-06-20 07:55:14.000000 sqlalchemy_celery_beat-0.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 07:57:12.919325 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/
--rw-rw-rw-   0        0        0      455 2023-06-20 07:55:05.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/__init__.py
--rw-rw-rw-   0        0        0     1317 2023-06-15 13:54:09.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/clockedschedule.py
--rw-rw-rw-   0        0        0    20425 2023-06-20 07:52:42.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/models.py
--rw-rw-rw-   0        0        0    16354 2023-06-20 07:52:42.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/schedulers.py
--rw-rw-rw-   0        0        0     4171 2023-06-19 07:50:11.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/session.py
--rw-rw-rw-   0        0        0     1323 2023-06-15 13:53:44.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/time_utils.py
--rw-rw-rw-   0        0        0     2766 2023-06-20 02:26:17.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/tzcrontab.py
-drwxrwxrwx   0        0        0        0 2023-06-20 07:57:12.957372 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat.egg-info/
--rw-rw-rw-   0        0        0    10599 2023-06-20 07:57:12.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      603 2023-06-20 07:57:12.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 07:57:12.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-06-20 07:57:12.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-15 17:41:10.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-06-20 07:57:12.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-06-20 07:57:12.000000 sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 14:58:41.586999 sqlalchemy_celery_beat-0.6.1/
+-rw-rw-rw-   0        0        0     1093 2023-06-15 09:28:10.000000 sqlalchemy_celery_beat-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0    10599 2023-06-20 14:58:41.585999 sqlalchemy_celery_beat-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9627 2023-06-20 07:42:22.000000 sqlalchemy_celery_beat-0.6.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-20 14:58:41.586999 sqlalchemy_celery_beat-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     3156 2023-06-20 14:58:25.000000 sqlalchemy_celery_beat-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:58:41.554001 sqlalchemy_celery_beat-0.6.1/sqlalchemy_celery_beat/
+-rw-rw-rw-   0        0        0      455 2023-06-20 14:58:15.000000 sqlalchemy_celery_beat-0.6.1/sqlalchemy_celery_beat/__init__.py
+-rw-rw-rw-   0        0        0     1317 2023-06-15 13:54:09.000000 sqlalchemy_celery_beat-0.6.1/sqlalchemy_celery_beat/clockedschedule.py
+-rw-rw-rw-   0        0        0    21047 2023-06-20 14:53:43.000000 sqlalchemy_celery_beat-0.6.1/sqlalchemy_celery_beat/models.py
+-rw-rw-rw-   0        0        0    16319 2023-06-20 14:40:58.000000 sqlalchemy_celery_beat-0.6.1/sqlalchemy_celery_beat/schedulers.py
+-rw-rw-rw-   0        0        0     4171 2023-06-19 07:50:11.000000 sqlalchemy_celery_beat-0.6.1/sqlalchemy_celery_beat/session.py
+-rw-rw-rw-   0        0        0     1323 2023-06-20 12:52:02.000000 sqlalchemy_celery_beat-0.6.1/sqlalchemy_celery_beat/time_utils.py
+-rw-rw-rw-   0        0        0     2766 2023-06-20 02:26:17.000000 sqlalchemy_celery_beat-0.6.1/sqlalchemy_celery_beat/tzcrontab.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:58:41.584000 sqlalchemy_celery_beat-0.6.1/sqlalchemy_celery_beat.egg-info/
+-rw-rw-rw-   0        0        0    10599 2023-06-20 14:58:41.000000 sqlalchemy_celery_beat-0.6.1/sqlalchemy_celery_beat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      603 2023-06-20 14:58:41.000000 sqlalchemy_celery_beat-0.6.1/sqlalchemy_celery_beat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 14:58:41.000000 sqlalchemy_celery_beat-0.6.1/sqlalchemy_celery_beat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-06-20 14:58:41.000000 sqlalchemy_celery_beat-0.6.1/sqlalchemy_celery_beat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-15 17:41:10.000000 sqlalchemy_celery_beat-0.6.1/sqlalchemy_celery_beat.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-06-20 14:58:41.000000 sqlalchemy_celery_beat-0.6.1/sqlalchemy_celery_beat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-20 14:58:41.000000 sqlalchemy_celery_beat-0.6.1/sqlalchemy_celery_beat.egg-info/top_level.txt
```

### Comparing `sqlalchemy_celery_beat-0.6.0/LICENSE` & `sqlalchemy_celery_beat-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.6.0/PKG-INFO` & `sqlalchemy_celery_beat-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy_celery_beat
-Version: 0.6.0
+Version: 0.6.1
 Summary: A Scheduler Based SQLalchemy For Celery
 Home-page: https://github.com/farahats9/sqlalchemy-celery-beat
 Author: Mohamed Farahat
 Author-email: farahats9@yahoo.com
 License: MIT
 Keywords: celery scheduler sqlalchemy beat
 Platform: any
```

### Comparing `sqlalchemy_celery_beat-0.6.0/README.md` & `sqlalchemy_celery_beat-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.6.0/setup.py` & `sqlalchemy_celery_beat-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 setup(
     name="sqlalchemy_celery_beat",
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.6.0",
+    version="0.6.1",
     # The project's main homepage.
     url="https://github.com/farahats9/sqlalchemy-celery-beat",
     # Choose your license
 
     license='MIT',
 
     description="A Scheduler Based SQLalchemy For Celery",
```

### Comparing `sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/clockedschedule.py` & `sqlalchemy_celery_beat-0.6.1/sqlalchemy_celery_beat/clockedschedule.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/models.py` & `sqlalchemy_celery_beat-0.6.1/sqlalchemy_celery_beat/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     from zoneinfo import available_timezones
 except ImportError:
     from backports.zoneinfo import available_timezones
 import enum
 import sqlalchemy as sa
 from celery import schedules
 from celery.utils.log import get_logger
+from celery.utils.time import maybe_make_aware, make_aware
 from sqlalchemy import event
 from sqlalchemy.future import Connection
 from sqlalchemy.orm import (Session, backref, foreign, relationship, remote,
                             validates)
 from sqlalchemy.sql import insert, select, update
 
 from .clockedschedule import clocked
@@ -44,34 +45,34 @@
     MINUTES = 'minutes'
     SECONDS = 'seconds'
     MICROSECONDS = 'microseconds'
 
 
 class SolarEvent(str, enum.Enum):
     DAWN_ASTRONOMICAL = 'dawn_astronomical'
-    DAWN_CIVIL = 'dawn_civil'
     DAWN_NAUTICAL = 'dawn_nautical'
-    DUSK_ASTRONOMICAL = 'dusk_astronomical'
-    DUSK_CIVIL = 'dusk_civil'
-    DUSK_NAUTICAL = 'dusk_nautical'
-    SOLAR_NOON = 'solar_noon'
+    DAWN_CIVIL = 'dawn_civil'
     SUNRISE = 'sunrise'
+    SOLAR_NOON = 'solar_noon'
     SUNSET = 'sunset'
+    DUSK_CIVIL = 'dusk_civil'
+    DUSK_NAUTICAL = 'dusk_nautical'
+    DUSK_ASTRONOMICAL = 'dusk_astronomical'
 
 
 class PeriodicTaskChanged(ModelBase, ModelMixin):
     """Helper table for tracking updates to periodic tasks."""
     __table_args__ = {
         'sqlite_autoincrement': False,
         'schema': 'celery_schema'
     }
 
     id = sa.Column(sa.Integer, primary_key=True)
     last_update = sa.Column(
-        sa.DateTime(timezone=True), nullable=False, default=dt.datetime.now)
+        sa.DateTime(timezone=True), nullable=False, default=lambda: maybe_make_aware(dt.datetime.utcnow()))
 
     @classmethod
     def changed(cls, mapper, connection, target):
         """
         :param mapper: the Mapper which is the target of this event
         :param connection: the Connection being used
         :param target: the mapped instance being persisted
@@ -87,19 +88,19 @@
         :param target: the mapped instance being persisted
         """
         logger.info('Database last time set to now')
         s = connection.execute(select(PeriodicTaskChanged).
                                where(PeriodicTaskChanged.id == 1).limit(1))
         if not s:
             s = connection.execute(insert(PeriodicTaskChanged),
-                                   last_update=dt.datetime.now())
+                                   last_update=maybe_make_aware(dt.datetime.utcnow()))
         else:
             s = connection.execute(update(PeriodicTaskChanged).
                                    where(PeriodicTaskChanged.id == 1).
-                                   values(last_update=dt.datetime.now()))
+                                   values(last_update=maybe_make_aware(dt.datetime.utcnow())))
 
     @classmethod
     def update_from_session(cls, session: Session, commit: bool = True):
         """
         :param session: the Session to use
         :param commit: commit the session if set to true
         """
@@ -164,14 +165,18 @@
                          doc='Priority',
                          comment='Priority Number between 0 and 255. '
                          'Supported by: RabbitMQ, Redis (priority reversed, 0 is highest).')
     expires = sa.Column(sa.DateTime(timezone=True),
                         doc='Expires Datetime',
                         comment='Datetime after which the schedule will no longer '
                         'trigger the task to run')
+    expire_seconds = sa.Column(sa.Integer,
+                               doc='Expires timedelta with seconds',
+                               comment='Timedelta with seconds which the schedule will no longer '
+                               'trigger the task to run')
 
     one_off = sa.Column(sa.Boolean(), default=False, nullable=False,
                         doc='One-off Task',
                         comment='If True, the schedule will only run the task a single time')
     start_time = sa.Column(sa.DateTime(timezone=True),
                            doc='Start Datetime',
                            comment='Datetime when the schedule should begin '
@@ -183,15 +188,16 @@
                             comment='Datetime that the schedule last triggered the task to run. ')
     total_run_count = sa.Column(sa.Integer(), nullable=False, default=0,
                                 doc='Total Run Count',
                                 comment='Running count of how many times the schedule '
                                 'has triggered the task')
 
     date_changed = sa.Column(sa.DateTime(timezone=True),
-                             default=dt.datetime.now, onupdate=dt.datetime.now,
+                             default=lambda: maybe_make_aware(dt.datetime.utcnow()),
+                             onupdate=lambda: maybe_make_aware(dt.datetime.utcnow()),
                              doc='Last Modified',
                              comment='Datetime that this PeriodicTask was last modified')
     description = sa.Column(sa.Text(), default='', doc='Description',
                             comment='Detailed description about the details of this Periodic Task')
 
     no_changes = False
 
@@ -220,26 +226,24 @@
             self.discriminator = value.discriminator
             setattr(self, "model_%s" % value.discriminator, value)
 
     @staticmethod
     def before_insert_or_update(mapper, connection, target):
         if target.enabled and isinstance(target.schedule_model, ClockedSchedule) and not target.one_off:
             raise ValueError("one_off must be True for clocked schedule")
+        if target.expire_seconds is not None and target.expires:
+            raise ValueError('Only one can be set, in expires and expire_seconds')
 
     def __repr__(self):
         fmt = '{0.name}: {0.schedule_model}'
         return fmt.format(self)
 
     @property
-    def task_name(self):
-        return self.task
-
-    @task_name.setter
-    def task_name(self, value):
-        self.task = value
+    def expires_(self):
+        return self.expires or self.expire_seconds
 
     @property
     def schedule(self):
         if self.schedule_model:
             return self.schedule_model.schedule
         raise ValueError('{} schedule is None!'.format(self.name))
 
@@ -432,15 +436,15 @@
             session.commit()
         return model
 
     @staticmethod
     def before_insert_or_update(mapper, connection, target):
         try:
             # Test the object to make sure it is valid before saving to DB
-            CrontabSchedule.aware_crontab(target).remaining_estimate(dt.datetime.now())
+            CrontabSchedule.aware_crontab(target).remaining_estimate(dt.datetime.utcnow())
         except Exception as exc:
             raise ValueError(f"Could not parse cron values: {str(exc)}") from exc
 
     @validates('timezone')
     def validate_crontab(self, key, value):
         if value not in available_timezones():
             raise ValueError(f'Timezone "{value}"  is not found in available timezones')
@@ -487,15 +491,15 @@
 
     @property
     def schedule(self):
         return schedules.solar(
             self.event,
             self.latitude,
             self.longitude,
-            nowfun=dt.datetime.now
+            nowfun=lambda: maybe_make_aware(dt.datetime.utcnow())
         )
 
     @classmethod
     def from_schedule(cls, session, schedule):
         spec = {
             'event': schedule.event,
             'latitude': schedule.lat,
```

### Comparing `sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/schedulers.py` & `sqlalchemy_celery_beat-0.6.1/sqlalchemy_celery_beat/schedulers.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,16 +56,15 @@
         self.app = app or current_app._get_current_object()
         self.Session = Session
         self.name = model.name
         self.task = model.task
         try:
             self.schedule = model.schedule
             logger.debug('schedule: {}'.format(self.schedule))
-        except Exception as e:
-            logger.error(e)
+        except Exception:
             logger.error(
                 'Disabling schedule %s that was removed from database',
                 self.name,
             )
             self._disable(model)
 
         try:
@@ -75,21 +74,27 @@
             logger.exception(
                 'Removing schedule %s for argument deseralization error: %r',
                 self.name, exc,
             )
             self._disable(model)
 
         self.options = {}
-        for option in ['queue', 'exchange', 'routing_key', 'expires',
-                       'priority']:
+        for option in ['queue', 'exchange', 'routing_key', 'priority']:
             value = getattr(model, option)
             if value is None:
                 continue
             self.options[option] = value
 
+        expires = getattr(model, 'expires_', None)
+        if expires:
+            if isinstance(expires, dt.datetime):
+                self.options['expires'] = maybe_make_aware(expires).astimezone(self.app.timezone)
+            else:
+                self.options['expires'] = expires
+
         self.options['headers'] = loads(model.headers or '{}')
         self.options['periodic_task_name'] = model.name
 
         self.total_run_count = model.total_run_count
         self.model = model
 
         if not model.last_run_at:
@@ -102,20 +107,15 @@
                 model.last_run_at = model.last_run_at \
                     - dt.timedelta(days=365 * 30)
 
         self.last_run_at = model.last_run_at
 
         # Because the last_run_at read from the database may not have time zone information,
         # so time zone information must be added here
-        self.last_run_at = self.last_run_at.replace(tzinfo=self.app.timezone)
-
-        # self.options['expires']
-        # if 'expires' in self.options:
-        #     expires = self.options['expires']
-        #     self.options['expires'] = expires.replace(tzinfo=self.app.timezone)
+        self.last_run_at = maybe_make_aware(self.last_run_at).astimezone(self.app.timezone)
 
     def _disable(self, model):
         model.no_changes = True
         self.model.enabled = self.enabled = model.enabled = False
         session = self.Session()
         with session_cleanup(session):
             session.add(model)
@@ -126,16 +126,15 @@
         if not self.model.enabled:
             # 5 second delay for re-enable.
             return schedules.schedstate(False, 5.0)
 
         # START DATE: only run after the `start_time`, if one exists.
         if self.model.start_time is not None:
             now = maybe_make_aware(self._default_now())
-            start_time = self.model.start_time.replace(
-                tzinfo=self.app.timezone)
+            start_time = maybe_make_aware(self.model.start_time)
             if now < start_time:
                 # The datetime is before the start date - don't run.
                 delay = math.ceil(
                     (start_time - now).total_seconds()
                 )
                 return schedules.schedstate(False, delay)
 
@@ -146,27 +145,25 @@
             self.model.total_run_count = 0  # Reset
             self.model.no_changes = False  # Mark the model entry as changed
             save_fields = ('enabled',)   # the additional fields to save
             self.save(save_fields)
 
             return schedules.schedstate(False, NEVER_CHECK_TIMEOUT)  # Don't recheck
 
+        # tz = self.app.timezone
+        # last_run_at_in_tz = maybe_make_aware(self.last_run_at).astimezone(tz)
+        # return self.schedule.is_due(last_run_at_in_tz)
         return self.schedule.is_due(self.last_run_at)
 
     def _default_now(self):
-        now = self.app.now()
-        # The PyTZ datetime must be localised for the Django-Celery-Beat
-        # scheduler to work. Keep in mind that timezone arithmatic
-        # with a localized timezone may be inaccurate.
-        # return now.tzinfo.localize(now.replace(tzinfo=None))
-        return now.replace(tzinfo=self.app.timezone)
+        now = maybe_make_aware(dt.datetime.utcnow())
+        return now
 
     def __next__(self):
-        # should be use `self._default_now()` or `self.app.now()` ?
-        self.model.last_run_at = self.app.now()
+        self.model.last_run_at = self._default_now()
         self.model.total_run_count += 1
         self.model.no_changes = True
         return self.__class__(self.model, Session=self.Session)
     next = __next__  # for 2to3
 
     def save(self, fields=tuple()):
         """
@@ -243,30 +240,32 @@
             kwargs=dumps(kwargs or {}),
             **cls._unpack_options(**options or {})
         )
         return entry
 
     @classmethod
     def _unpack_options(cls, queue=None, exchange=None, routing_key=None,
-                        priority=None, one_off=None, expires=None, **kwargs):
+                        priority=None, headers=None, one_off=True,
+                        expire_seconds=None, expires=None, start_time=None,
+                        ):
         data = {
             'queue': queue,
             'exchange': exchange,
             'routing_key': routing_key,
             'priority': priority,
+            'headers': dumps(headers or {}),
             'one_off': one_off,
+            'start_time': start_time,
+            'expire_seconds': expire_seconds,
         }
         if expires:
             if isinstance(expires, int):
-                expires = dt.datetime.utcnow() + dt.timedelta(seconds=expires)
-            elif isinstance(expires, dt.datetime):
-                pass
-            else:
-                raise ValueError('expires value error')
-            data['expires'] = expires
+                data['expire_seconds'] = expires
+            elif isinstance(expires, dt.timedelta):
+                data['expires'] = dt.datetime.utcnow() + expires
         return data
 
     def __repr__(self):
         return '<ModelEntry: {0} {1}(*{2}, **{3}) {4}>'.format(
             safe_str(self.name), self.task, safe_repr(self.args),
             safe_repr(self.kwargs), self.schedule,
         )
@@ -396,15 +395,15 @@
     def install_default_entries(self, data):
         entries = {}
         if self.app.conf.result_expires:
             entries.setdefault(
                 'celery.backend_cleanup', {
                     'task': 'celery.backend_cleanup',
                     'schedule': schedules.crontab('0', '4', '*'),
-                    'options': {'expires': 12 * 3600},
+                    'options': {'expire_seconds': 12 * 3600},
                 },
             )
         self.update_from_dict(entries)
 
     def schedules_equal(self, *args, **kwargs):
         if self._heap_invalidated:
             self._heap_invalidated = False
```

### Comparing `sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/session.py` & `sqlalchemy_celery_beat-0.6.1/sqlalchemy_celery_beat/session.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/time_utils.py` & `sqlalchemy_celery_beat-0.6.1/sqlalchemy_celery_beat/time_utils.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat/tzcrontab.py` & `sqlalchemy_celery_beat-0.6.1/sqlalchemy_celery_beat/tzcrontab.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat.egg-info/PKG-INFO` & `sqlalchemy_celery_beat-0.6.1/sqlalchemy_celery_beat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-celery-beat
-Version: 0.6.0
+Version: 0.6.1
 Summary: A Scheduler Based SQLalchemy For Celery
 Home-page: https://github.com/farahats9/sqlalchemy-celery-beat
 Author: Mohamed Farahat
 Author-email: farahats9@yahoo.com
 License: MIT
 Keywords: celery scheduler sqlalchemy beat
 Platform: any
```

### Comparing `sqlalchemy_celery_beat-0.6.0/sqlalchemy_celery_beat.egg-info/SOURCES.txt` & `sqlalchemy_celery_beat-0.6.1/sqlalchemy_celery_beat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

