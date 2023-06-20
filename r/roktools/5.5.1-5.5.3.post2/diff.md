# Comparing `tmp/roktools-5.5.1-py2.py3-none-any.whl.zip` & `tmp/roktools-5.5.3.post2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 20981 bytes, number of entries: 17
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-17 17:18 roktools/__init__.py
+Zip file size: 20937 bytes, number of entries: 17
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-20 12:14 roktools/__init__.py
 -rw-r--r--  2.0 unx     4641 b- defN 23-May-29 14:14 roktools/cl.py
 -rw-r--r--  2.0 unx      400 b- defN 23-May-29 14:14 roktools/file.py
 -rw-r--r--  2.0 unx    33542 b- defN 23-May-29 14:14 roktools/geodetic.py
 -rw-r--r--  2.0 unx     1479 b- defN 23-May-29 14:14 roktools/logger.py
 -rw-r--r--  2.0 unx     3613 b- defN 23-May-29 14:14 roktools/rinex.py
 -rw-r--r--  2.0 unx      861 b- defN 23-May-29 14:14 roktools/stats.py
 -rw-r--r--  2.0 unx     1580 b- defN 23-May-29 14:14 roktools/tensorial.py
--rw-r--r--  2.0 unx     9644 b- defN 23-Jun-17 17:17 roktools/time.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-17 17:18 roktools/gnss/__init__.py
--rw-r--r--  2.0 unx     1722 b- defN 23-May-29 14:14 roktools/gnss/types.py
--rw-rw-rw-  2.0 unx     1067 b- defN 23-Jun-17 17:18 roktools-5.5.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2604 b- defN 23-Jun-17 17:18 roktools-5.5.1.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-17 17:18 roktools-5.5.1.dist-info/WHEEL
--rw-r--r--  2.0 unx      127 b- defN 23-Jun-17 17:18 roktools-5.5.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-17 17:18 roktools-5.5.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1314 b- defN 23-Jun-17 17:18 roktools-5.5.1.dist-info/RECORD
-17 files, 62713 bytes uncompressed, 18845 bytes compressed:  70.0%
+-rw-r--r--  2.0 unx     8792 b- defN 23-Jun-20 12:13 roktools/time.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-20 12:14 roktools/gnss/__init__.py
+-rw-r--r--  2.0 unx     1769 b- defN 23-Jun-20 12:13 roktools/gnss/types.py
+-rw-rw-rw-  2.0 unx     1067 b- defN 23-Jun-20 12:14 roktools-5.5.3.post2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2683 b- defN 23-Jun-20 12:14 roktools-5.5.3.post2.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-20 12:14 roktools-5.5.3.post2.dist-info/WHEEL
+-rw-r--r--  2.0 unx      127 b- defN 23-Jun-20 12:14 roktools-5.5.3.post2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-20 12:14 roktools-5.5.3.post2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1350 b- defN 23-Jun-20 12:14 roktools-5.5.3.post2.dist-info/RECORD
+17 files, 62023 bytes uncompressed, 18729 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: roktools/gnss/__init__.py
 Comment: 
 
 Filename: roktools/gnss/types.py
 Comment: 
 
-Filename: roktools-5.5.1.dist-info/LICENSE
+Filename: roktools-5.5.3.post2.dist-info/LICENSE
 Comment: 
 
-Filename: roktools-5.5.1.dist-info/METADATA
+Filename: roktools-5.5.3.post2.dist-info/METADATA
 Comment: 
 
-Filename: roktools-5.5.1.dist-info/WHEEL
+Filename: roktools-5.5.3.post2.dist-info/WHEEL
 Comment: 
 
-Filename: roktools-5.5.1.dist-info/entry_points.txt
+Filename: roktools-5.5.3.post2.dist-info/entry_points.txt
 Comment: 
 
-Filename: roktools-5.5.1.dist-info/top_level.txt
+Filename: roktools-5.5.3.post2.dist-info/top_level.txt
 Comment: 
 
-Filename: roktools-5.5.1.dist-info/RECORD
+Filename: roktools-5.5.3.post2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## roktools/time.py

```diff
@@ -3,37 +3,26 @@
 import math
 import enum
 from typing import List, Tuple
 import numpy as np
 WeekTow = namedtuple('WeekTow', 'week tow day_of_week')
 
 
-class TimeScale(enum.Enum):
-    GPS = enum.auto()
-    UTC = enum.auto()
-
-def get_gps_leapseconds(utc_date:datetime.date) -> datetime.timedelta:
-
-    if utc_date >= datetime.date(2017, 1, 1): return datetime.timedelta(seconds=18)
-    elif utc_date >= datetime.date(2015, 7, 1): return datetime.timedelta(seconds=17)
-    elif utc_date >= datetime.date(2012, 7, 1): return datetime.timedelta(seconds=16)
-    elif utc_date >= datetime.date(2009, 1, 1): return datetime.timedelta(seconds=15)
-    elif utc_date >= datetime.date(2006, 1, 1): return datetime.timedelta(seconds=14)
-    elif utc_date >= datetime.date(1999, 1, 1): return datetime.timedelta(seconds=13)
-
-    raise ValueError('No Leap second information for epochs prior to 1999-01-01')
-
-
-
 GPS_TIME_START = datetime.datetime(1980, 1, 6, 0, 0, 0)
 J2000_TIME_START = datetime.datetime(2000, 1, 1, 12, 0, 0)
 SECONDS_IN_DAY = 24 * 60 * 60
 SECONDS_IN_WEEK = 86400 * 7
 GPS_AS_J2000 = -630763200
 
+
+class TimeScale(enum.Enum):
+    GPS = enum.auto()
+    UTC = enum.auto()
+
+
 class Timespan:
     def __init__(self, start: datetime.datetime, end: datetime.datetime):
         self.start = start
         self.end = end
 
     def __str__(self):
         return f"{self.start} - {self.end}"
@@ -63,62 +52,63 @@
         start = max(self.start, other.start)
         end = min(self.end, other.end)
         return Timespan(start, end)
 
     def __repr__(self) -> str:
         return self.__str__
 
-def to_week_tow(epoch: datetime.datetime, time_scale: TimeScale= TimeScale.GPS, apply_leap_seconds:bool = False) -> WeekTow:
+
+def get_gps_leapseconds(utc_date:datetime.date) -> datetime.timedelta:
+
+    if utc_date >= datetime.date(2017, 1, 1): return datetime.timedelta(seconds=18)
+    elif utc_date >= datetime.date(2015, 7, 1): return datetime.timedelta(seconds=17)
+    elif utc_date >= datetime.date(2012, 7, 1): return datetime.timedelta(seconds=16)
+    elif utc_date >= datetime.date(2009, 1, 1): return datetime.timedelta(seconds=15)
+    elif utc_date >= datetime.date(2006, 1, 1): return datetime.timedelta(seconds=14)
+    elif utc_date >= datetime.date(1999, 1, 1): return datetime.timedelta(seconds=13)
+
+    raise ValueError('No Leap second information for epochs prior to 1999-01-01')
+
+
+def to_week_tow(epoch: datetime.datetime) -> WeekTow:
     """
     Convert from datetime to GPS week
 
-    >>> to_week_tow(datetime.datetime(1980, 1, 6), TimeScale.UTC)
-    WeekTow(week=0, tow=0.0, day_of_week=0)
-    >>> to_week_tow(datetime.datetime(2005, 1, 28, 13, 30), TimeScale.GPS, apply_leap_seconds = True)
+    >>> to_week_tow(datetime.datetime(2005, 1, 28, 13, 30))
     WeekTow(week=1307, tow=480613.0, day_of_week=5)
 
     Conversion method based on algorithm provided in this link
     http://www.novatel.com/support/knowledge-and-learning/published-papers-and-documents/unit-conversions/
     """
 
     timedelta = epoch - GPS_TIME_START
-    leap_delta = datetime.timedelta(0)
-    if apply_leap_seconds and time_scale == TimeScale.GPS:
-        leap_delta = get_gps_leapseconds(epoch.date())
+    leap_delta = get_gps_leapseconds(epoch.date())
+
     gpsw = int(timedelta.days / 7)
     day = timedelta.days - 7 * gpsw
     tow = timedelta.microseconds * 1e-6 + timedelta.seconds + day * SECONDS_IN_DAY + leap_delta.total_seconds()
 
     return WeekTow(gpsw, tow, day)
 
 
-# ------------------------------------------------------------------------------
-
-def from_week_tow(week: int, tow: float, time_scale: TimeScale=TimeScale.GPS, apply_leap_seconds:bool = False) -> datetime.datetime:
+def from_week_tow(week: int, tow: float) -> datetime.datetime:
     """
     Convert from datetime to GPS week
 
-    >>> from_week_tow(0, 0.0, TimeScale.UTC)
-    datetime.datetime(1980, 1, 6, 0, 0)
-    >>> from_week_tow(1307, 480600.0, TimeScale.UTC)
-    datetime.datetime(2005, 1, 28, 13, 30)
-    >>> from_week_tow(1307, 480613.0, TimeScale.GPS)
+    >>> from_week_tow(1307, 480613.0)
     datetime.datetime(2005, 1, 28, 13, 30)
 
     """
     delta = datetime.timedelta(weeks=week, seconds=tow)
-
     gps_epoch = GPS_TIME_START + delta
-
-    leap_delta = datetime.timedelta(0)
-    if apply_leap_seconds or time_scale == TimeScale.GPS:
-        leap_delta = -get_gps_leapseconds(gps_epoch.date())
+    leap_delta = -get_gps_leapseconds(gps_epoch.date())
 
     return gps_epoch + leap_delta
 
+
 def weektow_to_datetime(tow: float, week: int) -> datetime.datetime:
     import warnings
     warnings.warn("This function will be replaced by 'from_week_tow'", DeprecationWarning, stacklevel=2)
     return from_week_tow(week, tow)
 
 
 def weektow_to_j2000(tow: float, week: int) -> float:
@@ -137,23 +127,24 @@
 
     # Rebase seconds from GPS start origin to J2000 start origin
     j2000s += GPS_AS_J2000
 
     return j2000s
 
 
-def to_j2000(epoch: datetime.datetime, time_scale:TimeScale = TimeScale.GPS) -> float:
+def to_j2000(epoch: datetime.datetime) -> float:
     """
     Convert from datetime toj2000 seconds
 
-    >>> to_j2000(datetime.datetime(2005, 1, 28, 13, 30), TimeScale.UTC)
-    160191000.0
+    >>> to_j2000(datetime.datetime(2005, 1, 28, 13, 30, 0, 100001))
+    160191000.100001
     """
-    week_tow = to_week_tow(epoch, time_scale)
-    return weektow_to_j2000(week_tow.tow, week_tow.week)
+
+    return (epoch - J2000_TIME_START).total_seconds()
+    
 
 def from_j2000(j2000s: int, fraction_of_seconds: float = 0.0) -> datetime.datetime:
     """
     Convert from J2000 epoch to datetime
 
     >>> from_j2000(160191000)
     datetime.datetime(2005, 1, 28, 13, 30)
```

## roktools/gnss/types.py

```diff
@@ -1,13 +1,15 @@
 from enum import Enum
 from dataclasses import dataclass
 
 class ConstellationId(Enum):
     GPS : str = 'G' 
     GALILEO : str = 'E'
+    BEIDOU : str = 'C'
+    GLONASS : str = 'R'
     
     
 class ChannelCode(Enum):
     c_1C : str = "1C"
     c_5Q : str = "5Q"
```

## Comparing `roktools-5.5.1.dist-info/LICENSE` & `roktools-5.5.3.post2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `roktools-5.5.1.dist-info/METADATA` & `roktools-5.5.3.post2.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roktools
-Version: 5.5.1
+Version: 5.5.3.post2
 Summary: Set of tools used in internal Rokubun projects
 Home-page: https://www.rokubun.cat
 Author: Àlex López, Miquel García
 Author-email: alex.lopez@rokubun.cat, miquel.garcia@rokubun.cat
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -18,20 +18,22 @@
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
 Requires-Dist: setuptools (>=8.0)
 Requires-Dist: numpy (~=1.21)
 Provides-Extra: all
 Requires-Dist: pytest ; extra == 'all'
 Requires-Dist: pytest-mocha ; extra == 'all'
+Requires-Dist: tox ; extra == 'all'
 Provides-Extra: lint
 Requires-Dist: flake8 ; extra == 'lint'
 Requires-Dist: tox (==3.27.1) ; extra == 'lint'
 Provides-Extra: test
 Requires-Dist: pytest ; extra == 'test'
 Requires-Dist: pytest-mocha ; extra == 'test'
+Requires-Dist: tox ; extra == 'test'
 
 # pyrok-tools
 
 Python tools used in internal Rokubun projects. This repository contains the following modules:
 
 - `logger`, a module that extends basic Python logging
 - `geodetic`, to perform basic geodetic transformation (Cartesian to Geodetic,
```

## Comparing `roktools-5.5.1.dist-info/RECORD` & `roktools-5.5.3.post2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 roktools/cl.py,sha256=LuRhDicv8eJAxvI7gbnG7RnOiRmEtyuUKg-nNcJlL1U,4641
 roktools/file.py,sha256=hJuPUBGz7MC600sfvOgwa2Md4uSHr10iChrW36sAeRQ,400
 roktools/geodetic.py,sha256=dxSoPxxooEyeKyEQqGfcb1WYmH9-Hl-kREtQu9kHpE4,33542
 roktools/logger.py,sha256=4kvcTWXPoiG-MlyP6B330l4Fu7MfCuDjuIlIiLA8f1Y,1479
 roktools/rinex.py,sha256=74IU4Nw-KKiAW1mTJd3UZYPH83oFQHppsfBejE8RH_Q,3613
 roktools/stats.py,sha256=I-XJdwktJIZgO7BIaEZYyGXQOpWBRLQCMStzRfmLvJk,861
 roktools/tensorial.py,sha256=RZ8-9Z926mQigYX9S0tjAa068jUMu5JkBElXLSLbYDY,1580
-roktools/time.py,sha256=WMSVJQolZYkk8XSqKgHWJsVGrYsNDsRk9xOul82HpOo,9644
+roktools/time.py,sha256=9hEAAl-q8DxJuef28dSCtfdJU4sgz-tAf-bpnXyYVNc,8792
 roktools/gnss/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-roktools/gnss/types.py,sha256=6g-Hp2HcGGwbhP-tlGoZlah0sJkcMQ3y7e-j9NKAa3I,1722
-roktools-5.5.1.dist-info/LICENSE,sha256=Wwany6RAAZ9vVHjFLA9KBJ0HE77d52s2NOUA1CPAEug,1067
-roktools-5.5.1.dist-info/METADATA,sha256=sVsYG6BC6Yf9bbqIwaC28kkZXR7B55r2h-eMn5rYh0g,2604
-roktools-5.5.1.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-roktools-5.5.1.dist-info/entry_points.txt,sha256=tqrJvPDvOGCSWlRebEVLccLeFL5t-VHWC2aIoBNaZLA,127
-roktools-5.5.1.dist-info/top_level.txt,sha256=0RQjCH-RrFWM5YvdqifHlQ9EqtA2tdgtUb7tVuWzFDE,9
-roktools-5.5.1.dist-info/RECORD,,
+roktools/gnss/types.py,sha256=ecRfonSn66LV5wQNexvbZPb_kClQxC1uvJcBY2HgoTk,1769
+roktools-5.5.3.post2.dist-info/LICENSE,sha256=Wwany6RAAZ9vVHjFLA9KBJ0HE77d52s2NOUA1CPAEug,1067
+roktools-5.5.3.post2.dist-info/METADATA,sha256=EXonOgkZ9JYtbJ0RFRIe5yKOR1SKOSuZA5ICOLZCZ7U,2683
+roktools-5.5.3.post2.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+roktools-5.5.3.post2.dist-info/entry_points.txt,sha256=tqrJvPDvOGCSWlRebEVLccLeFL5t-VHWC2aIoBNaZLA,127
+roktools-5.5.3.post2.dist-info/top_level.txt,sha256=0RQjCH-RrFWM5YvdqifHlQ9EqtA2tdgtUb7tVuWzFDE,9
+roktools-5.5.3.post2.dist-info/RECORD,,
```

