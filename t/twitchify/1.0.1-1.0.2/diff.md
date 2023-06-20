# Comparing `tmp/twitchify-1.0.1.tar.gz` & `tmp/twitchify-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitchify-1.0.1.tar", last modified: Tue Jun 20 17:08:01 2023, max compression
+gzip compressed data, was "twitchify-1.0.2.tar", last modified: Tue Jun 20 19:21:00 2023, max compression
```

## Comparing `twitchify-1.0.1.tar` & `twitchify-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 17:08:01.172967 twitchify-1.0.1/
--rw-rw-rw-   0        0        0     1747 2023-06-20 17:08:01.171968 twitchify-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1380 2023-06-20 16:26:45.000000 twitchify-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-20 17:08:01.172967 twitchify-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      896 2023-06-20 17:07:45.000000 twitchify-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:08:01.144984 twitchify-1.0.1/twitch/
--rw-rw-rw-   0        0        0     1328 2023-06-20 15:33:19.000000 twitchify-1.0.1/twitch/__init__.py
--rw-rw-rw-   0        0        0     5241 2023-06-20 15:29:57.000000 twitchify-1.0.1/twitch/channel.py
--rw-rw-rw-   0        0        0     7468 2023-06-20 15:19:57.000000 twitchify-1.0.1/twitch/client.py
--rw-rw-rw-   0        0        0     3352 2023-06-20 15:24:23.000000 twitchify-1.0.1/twitch/errors.py
--rw-rw-rw-   0        0        0    11170 2023-06-20 15:27:41.000000 twitchify-1.0.1/twitch/gateway.py
--rw-rw-rw-   0        0        0     7491 2023-06-20 00:35:39.000000 twitchify-1.0.1/twitch/goals.py
--rw-rw-rw-   0        0        0    15095 2023-06-20 15:27:41.000000 twitchify-1.0.1/twitch/http.py
--rw-rw-rw-   0        0        0     2171 2023-06-20 00:12:07.000000 twitchify-1.0.1/twitch/message.py
--rw-rw-rw-   0        0        0     3729 2023-06-20 00:35:40.000000 twitchify-1.0.1/twitch/moderation.py
--rw-rw-rw-   0        0        0     6566 2023-06-20 00:35:39.000000 twitchify-1.0.1/twitch/reward.py
--rw-rw-rw-   0        0        0    13751 2023-06-20 01:23:10.000000 twitchify-1.0.1/twitch/state.py
--rw-rw-rw-   0        0        0     3970 2023-06-20 00:35:40.000000 twitchify-1.0.1/twitch/stream.py
--rw-rw-rw-   0        0        0     7761 2023-06-20 00:35:40.000000 twitchify-1.0.1/twitch/survey.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:08:01.149982 twitchify-1.0.1/twitch/types/
--rw-rw-rw-   0        0        0     2137 2023-06-20 00:12:07.000000 twitchify-1.0.1/twitch/types/gateway.py
--rw-rw-rw-   0        0        0     1414 2023-06-20 00:12:07.000000 twitchify-1.0.1/twitch/types/http.py
--rw-rw-rw-   0        0        0     1306 2023-06-20 00:12:07.000000 twitchify-1.0.1/twitch/types/message.py
--rw-rw-rw-   0        0        0     2701 2023-06-20 00:12:07.000000 twitchify-1.0.1/twitch/types/user.py
--rw-rw-rw-   0        0        0     5701 2023-06-20 00:35:40.000000 twitchify-1.0.1/twitch/user.py
--rw-rw-rw-   0        0        0     5432 2023-06-20 01:19:01.000000 twitchify-1.0.1/twitch/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 17:08:01.169968 twitchify-1.0.1/twitchify.egg-info/
--rw-rw-rw-   0        0        0     1747 2023-06-20 17:08:01.000000 twitchify-1.0.1/twitchify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      529 2023-06-20 17:08:01.000000 twitchify-1.0.1/twitchify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 17:08:01.000000 twitchify-1.0.1/twitchify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-20 17:08:01.000000 twitchify-1.0.1/twitchify.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-20 17:08:01.000000 twitchify-1.0.1/twitchify.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 19:21:00.113165 twitchify-1.0.2/
+-rw-rw-rw-   0        0        0     2532 2023-06-20 19:21:00.112164 twitchify-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1543 2023-06-20 18:44:54.000000 twitchify-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-20 19:21:00.114163 twitchify-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1586 2023-06-20 18:37:36.000000 twitchify-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:21:00.046204 twitchify-1.0.2/twitch/
+-rw-rw-rw-   0        0        0     1328 2023-06-20 18:30:54.000000 twitchify-1.0.2/twitch/__init__.py
+-rw-rw-rw-   0        0        0     5241 2023-06-20 15:29:57.000000 twitchify-1.0.2/twitch/channel.py
+-rw-rw-rw-   0        0        0     7468 2023-06-20 19:08:00.000000 twitchify-1.0.2/twitch/client.py
+-rw-rw-rw-   0        0        0     3352 2023-06-20 15:24:23.000000 twitchify-1.0.2/twitch/errors.py
+-rw-rw-rw-   0        0        0    11104 2023-06-20 19:08:00.000000 twitchify-1.0.2/twitch/gateway.py
+-rw-rw-rw-   0        0        0     7814 2023-06-20 19:08:00.000000 twitchify-1.0.2/twitch/goals.py
+-rw-rw-rw-   0        0        0    15033 2023-06-20 19:08:00.000000 twitchify-1.0.2/twitch/http.py
+-rw-rw-rw-   0        0        0     2287 2023-06-20 19:08:00.000000 twitchify-1.0.2/twitch/message.py
+-rw-rw-rw-   0        0        0     3737 2023-06-20 19:08:00.000000 twitchify-1.0.2/twitch/moderation.py
+-rw-rw-rw-   0        0        0     6740 2023-06-20 19:08:00.000000 twitchify-1.0.2/twitch/reward.py
+-rw-rw-rw-   0        0        0    14007 2023-06-20 19:09:24.000000 twitchify-1.0.2/twitch/state.py
+-rw-rw-rw-   0        0        0     3986 2023-06-20 19:09:24.000000 twitchify-1.0.2/twitch/stream.py
+-rw-rw-rw-   0        0        0     7761 2023-06-20 00:35:40.000000 twitchify-1.0.2/twitch/survey.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:21:00.057198 twitchify-1.0.2/twitch/types/
+-rw-rw-rw-   0        0        0     2137 2023-06-20 00:12:07.000000 twitchify-1.0.2/twitch/types/gateway.py
+-rw-rw-rw-   0        0        0     1414 2023-06-20 00:12:07.000000 twitchify-1.0.2/twitch/types/http.py
+-rw-rw-rw-   0        0        0     1306 2023-06-20 00:12:07.000000 twitchify-1.0.2/twitch/types/message.py
+-rw-rw-rw-   0        0        0     2701 2023-06-20 00:12:07.000000 twitchify-1.0.2/twitch/types/user.py
+-rw-rw-rw-   0        0        0     5709 2023-06-20 19:09:24.000000 twitchify-1.0.2/twitch/user.py
+-rw-rw-rw-   0        0        0     5129 2023-06-20 18:37:37.000000 twitchify-1.0.2/twitch/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:21:00.109165 twitchify-1.0.2/twitchify.egg-info/
+-rw-rw-rw-   0        0        0     2532 2023-06-20 19:20:59.000000 twitchify-1.0.2/twitchify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      529 2023-06-20 19:20:59.000000 twitchify-1.0.2/twitchify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 19:20:59.000000 twitchify-1.0.2/twitchify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-06-20 19:20:59.000000 twitchify-1.0.2/twitchify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-20 19:20:59.000000 twitchify-1.0.2/twitchify.egg-info/top_level.txt
```

### Comparing `twitchify-1.0.1/PKG-INFO` & `twitchify-1.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,37 @@
-Metadata-Version: 2.1
-Name: twitchify
-Version: 1.0.1
-Summary: A Python Twitch API wrapper
-Home-page: https://github.com/mrsnifo/twitchify
-Author: Snifo
-Author-email: Snifo@mail.com
-License: MIT
-Project-URL: Issue tracker, https://github.com/mrsnifo/twitchify/issues
-Platform: UNKNOWN
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-
 # Twitchify
 
 ---
+
 [![Discord](https://img.shields.io/discord/938786168592547880)](https://discord.gg/hH4ZkNg6cA)
-[![PyPI Version](https://img.shields.io/pypi/v/twitchify.svg)](https://pypi.org/project/twitchify)
+[![PyPI Version](https://img.shields.io/pypi/v/twitchify)](https://pypi.org/project/twitchify)
 ![Python versions](https://img.shields.io/pypi/pyversions/twitchify)
 
-Twitchify is a Python library that provides a lightweight and extensible Twitch API wrapper with support for WebSocket EventSub.
-
-**Note**: Twitchify currently supports EventSub only.
+Python library for Twitch's WebSocket **EventSub** integration
 
 ## Features
-
-- WebSocket EventSub support for real-time Twitch event notifications.
-- Easy-to-use interfaces for accessing Twitch resources.
+- Comprehensive support for WebSocket EventSub, providing real-time Twitch event notifications.
+- User-friendly interfaces for seamless integration.
+- Built-in support for type hinting, ensuring code clarity and maintainability.
 
 ## Installation
 
 You can install Twitchify using pip:
 
 ```shell
 # Windows
 py -3 -m pip install -U twitchify
 
 # Linux/macOS
 python3 -m pip install -U twitchify
 ```
 
+## Documentation
+Please refer to the [Events Documentation](https://github.com/MrSniFo/Twitchify/blob/main/docs/EVENTS.md) for detailed information on handling events with Twitchify.
+
 ## Quick Example
 ```python
 from twitch import Client
 from twitch.user import Follower
 
 client = Client(client_id="CLIENT ID HERE")
 
@@ -57,10 +46,9 @@
 @client.event
 async def on_follow(user: Follower):
     """
     Event handler triggered when a user follows the channel.
     """
     print("%s just followed you!" % user.display_name)
 
-client.run( access_token="USER ACCESS TOKEN HERE")
+client.run(access_token="USER ACCESS TOKEN HERE")
 ```
-
```

### Comparing `twitchify-1.0.1/twitch/__init__.py` & `twitchify-1.0.2/twitch/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,14 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 __title__ = 'Twitchify'
-__version__ = '1.0.0'
+__version__ = '1.0.2'
 __license__ = 'MIT License'
 __author__ = 'Snifo'
 __email__ = 'Snifo@mail.com'
 __github__ = 'https://github.com/mrsnifo/twitchify'
 
 from .client import Client
```

### Comparing `twitchify-1.0.1/twitch/channel.py` & `twitchify-1.0.2/twitch/channel.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.0.1/twitch/client.py` & `twitchify-1.0.2/twitch/client.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -126,28 +126,28 @@
         :param access_token: The access token for authentication.
         :param refresh_token: The refresh token for refreshing the access token, if applicable.
         """
         # Setup logger
         setup_logging()
         if self.loop is None:
             self.loop = asyncio.get_running_loop()
-        self.dispatch('connect')
         # Validating the access key and opening a new session.
         validation = await self._http.open_session(access_token=access_token, refresh_token=refresh_token)
         # Retrieving the client.
         self._connection.broadcaster = await self._http.get_client()
         # Creating an EventSub websocket.
         EventSub = EventSubWebSocket(http=self._http, connection=self._connection,
                                      loop=self.loop,
                                      events=self._sub_events)
         # Creating tasks.
         tasks = [
             self.loop.create_task(self._http.Refresher(expires_in=validation['expires_in']),
                                   name="Twitchify:Refresher")
         ]
+        self.dispatch('connect')
         # Makes sure that there are events to subscribe to.
         if len(EventSub.subscriptions) >= 1:
             tasks.append(self.loop.create_task(EventSub.connect(), name="Twitchify:EventSub"))
 
         await asyncio.gather(*tasks)
 
     async def start(self, access_token: str, refresh_token: Optional[str] = None) -> None:
```

### Comparing `twitchify-1.0.1/twitch/errors.py` & `twitchify-1.0.2/twitch/errors.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.0.1/twitch/gateway.py` & `twitchify-1.0.2/twitch/gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,25 +30,23 @@
 
 # Libraries
 from asyncio import wait_for, sleep, TimeoutError, AbstractEventLoop
 from json import JSONDecodeError
 from aiohttp import WSMsgType
 
 from typing import TYPE_CHECKING
-
 if TYPE_CHECKING:
     from .types.eventsub.subscriptions import SubscriptionPayload
     from typing import Optional, List, Dict, Any
     from aiohttp import ClientWebSocketResponse
     from .state import ConnectionState
     from .http import HTTPClient
     from .types.gateway import *
 
 import logging
-
 _logger = logging.getLogger(__name__)
 
 
 class WsReconnect(Exception):
     """
     Reconnect to a new websocket.
     """
@@ -59,15 +57,15 @@
 
 class EventSubWebSocket:
     DEFAULT_URL = 'wss://eventsub.wss.twitch.tv/ws'
 
     __slots__ = ('_http', '__connection', '__loop', 'subscriptions', '_ready', '_keep_alive', '_ws', '_ws_switch',
                  'session_id', 'retry_count')
 
-    def __init__(self, *, http: HTTPClient, connection: ConnectionState, loop, events: List[str]):
+    def __init__(self, *, http: HTTPClient, connection: ConnectionState, loop, events: List[str]) -> None:
         """
         Initialize the EventSubWebSocket.
 
         :param http:
          The HTTP client for making API requests.
 
         :param events:
@@ -198,15 +196,14 @@
                         self._ws_switch = None
                     else:
                         # Subscribing to events.
                         task = self._http.subscribe(user_id=self.__connection.broadcaster.id,
                                                     session_id=_session['id'],
                                                     subscriptions=self.subscriptions)
                         self.__loop.create_task(task, name='Twitchify:Subscriptions')
-                        await self.__connection.parse(event='ready')
                     if _session['id'] != self.session_id:
                         if self.session_id is not None:
                             _logger.debug('A new WebSocket Session has been detected ID: %s', _session['id'])
                         self.session_id = _session['id']
                     # KeepAlive timeout.
                     self._keep_alive = _session['keepalive_timeout_seconds']
```

### Comparing `twitchify-1.0.1/twitch/goals.py` & `twitchify-1.0.2/twitch/goals.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,159 +33,162 @@
     from .types.eventsub import hypertrain as ht
     from .types.eventsub import charity as ch
     from typing import Optional, Union, List
     from .types.eventsub import goal as gl
     from datetime import datetime
 
 
-
-class CharityInfo:
+class _CharityInfo:
     """
     Information about a charity.
     """
+    __slots__ = ('name', 'description', 'logo', 'website')
 
-    def __init__(self, charity: ch.SpecificCharity):
+    def __init__(self, charity: ch.SpecificCharity) -> None:
         self.name: str = charity['charity_name']
-        self.description: Optional[str] = charity.get('charity_description')
+        self.description: Optional[str] = charity.get('charity_description')  # Beta
         self.logo: str = charity['charity_logo']
-        self.website: Optional[str] = charity.get('charity_website')
+        self.website: Optional[str] = charity.get('charity_website')  # Beta
+
+    def __repr__(self) -> str:
+        return f'<_CharityInfo name={self.name} description={self.description}>'
 
 
 class _CharityAmount:
     """
     Represents an amount with its value and currency.
     """
     __slots__ = ('value', 'currency')
 
-    def __init__(self, *, amount: ch.Amount):
+    def __init__(self, *, amount: ch.Amount) -> None:
         self.value: float = (amount['value'] / 10 ** amount['decimal_places'])
         self.currency: str = amount['currency']
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'<_Amount value={self.value} currency={self.currency}>'
 
 
 class Charity:
     """
     Represents a channel charity.
     """
     __slots__ = ('id', 'charity', 'current_amount', 'target_amount', '_started_at', '_stopped_at')
 
-    def __init__(self, charity: Union[ch.Start, ch.Progress, ch.Stop]):
+    def __init__(self, charity: Union[ch.Start, ch.Progress, ch.Stop]) -> None:
         self.id: str = charity['id']
-        self.charity: CharityInfo = CharityInfo(charity=charity)
+        self.charity: _CharityInfo = _CharityInfo(charity=charity)
         self.current_amount: _CharityAmount = _CharityAmount(amount=charity['current_amount'])
         self.target_amount: _CharityAmount = _CharityAmount(amount=charity['target_amount'])
         self._started_at: Optional[str] = charity.get('started_at')
         self._stopped_at: Optional[str] = charity.get('stopped_at')
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'<Charity id={self.id} current_amount={self.current_amount.__repr__()}>'
 
 
 class Donation:
     """
     Represents a donation made to a charity.
     """
     __slots__ = ('id', 'charity', 'user', 'amount')
 
-    def __init__(self, donation: ch.Donation):
+    def __init__(self, donation: ch.Donation) -> None:
         self.id: str = donation['id']
-        self.charity: CharityInfo = CharityInfo(charity=donation)
+        self.charity: _CharityInfo = _CharityInfo(charity=donation)
         self.user: User = User(user=donation)
         self.amount: _CharityAmount = _CharityAmount(amount=donation['amount'])
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'<Donation id={self.id} user={self.user.__repr__()} amount={self.amount.__repr__()}>'
 
 
 class _GoalAmount:
     """
     Represents the amount and type of goal.
     """
 
-    def __init__(self, goal: gl.Goal):
+    def __init__(self, goal: gl.Goal) -> None:
         self.value: int = goal['current_amount']
         self.type: str = goal['type']
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'<_GoalAmount value={self.value} type={self.type}>'
 
 
 class Goal:
     """
     Represents a channel goal.
     """
     __slots__ = ('id', 'description', 'amount', 'started_at', 'is_achieved', '_ended_at')
 
-    def __init__(self, goal: Union[gl.Begin, gl.Progress, gl.End]):
+    def __init__(self, goal: Union[gl.Begin, gl.Progress, gl.End]) -> None:
         self.id: str = goal['id']
         self.description: str = goal['description']
         self.amount: _GoalAmount = _GoalAmount(goal=goal)
         self.started_at: datetime = parse_rfc3339_timestamp(timestamp=goal['started_at'])
         self.is_achieved: bool = goal.get('is_achieved') or False
         self._ended_at: Optional[str] = goal.get('ended_at')
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'<Goal id={self.id} amount={self.amount.__repr__()} started_at={self.started_at}>'
 
 
 class _Contributor:
     """
     Hyper train top contributor.
     """
     __slots__ = ('user', 'type', 'total')
 
-    def __init__(self, *, contributor: ht.Contributor):
+    def __init__(self, *, contributor: ht.Contributor) -> None:
         self.user: User = User(user=contributor)
         self.type: str = contributor['type']
         self.total: int = contributor['total']
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'<_Contributor user={self.user.__repr__()} total={self.total} type={self.type}>'
 
 
 class Train:
     """
     Hyper train progress.
     """
     __slots__ = ('progress', 'goal', 'expires_at', '_last_contribution')
 
-    def __init__(self, train: ht.Begin):
+    def __init__(self, train: ht.Begin) -> None:
         self.goal: int = train['goal']
         self.progress: int = train['progress']
         self.expires_at: datetime = parse_rfc3339_timestamp(timestamp=train['expires_at'])
         self._last_contribution: List[ht.Contributor] = train['last_contribution']
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'<_Train goal={self.goal} progress={self.progress} expires_at={self.expires_at}>'
 
     @property
     def last_contribution(self) -> List[_Contributor]:
         return [_Contributor(contributor=c) for c in self._last_contribution]
 
 
 class HyperTrain:
     """
     Represents a channel Hyper Train.
     """
     __slots__ = ('__hypertrain', 'id', 'total', 'level', '_top_contributions', 'started_at', '_ended_at',
                  '_cooldown_ends_at')
 
-    def __init__(self, hypertrain: Union[ht.Begin, ht.Progress, ht.End]):
+    def __init__(self, hypertrain: Union[ht.Begin, ht.Progress, ht.End]) -> None:
         self.__hypertrain = hypertrain
         self.id: str = hypertrain['id']
         self.level: int = hypertrain['level']
         self.total: int = hypertrain['total']
         self._top_contributions: List[ht.Contributor] = hypertrain['top_contributions']
         self.started_at: datetime = parse_rfc3339_timestamp(timestamp=hypertrain['started_at'])
         self._ended_at: Optional[str] = hypertrain.get('ended_at')
         self._cooldown_ends_at: Optional[str] = hypertrain.get('cooldown_ends_at')
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'<HyperTrain id={self.id} level={self.level} total={self.total}>'
 
     @property
     def top_contributions(self) -> List[_Contributor]:
         return [_Contributor(contributor=c) for c in self._top_contributions]
 
     @property
```

### Comparing `twitchify-1.0.1/twitch/http.py` & `twitchify-1.0.2/twitch/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,25 +40,24 @@
 if TYPE_CHECKING:
     from .types.eventsub.subscriptions import SubscriptionPayload
     from aiohttp import ClientWebSocketResponse
     from .types.http import Validate, Refresh
     from .state import ConnectionState
     from typing import Optional, List
 
-
 import logging
 _logger = logging.getLogger(__name__)
 
 
 class Route:
     BASE_ROUTE: str = 'https://api.twitch.tv/helix/'
 
     __slots__ = ('method', 'url')
 
-    def __init__(self, method: str, path: Optional[str] = None, url: Optional[str] = None):
+    def __init__(self, method: str, path: Optional[str] = None, url: Optional[str] = None) -> None:
         """
         Initialize a Route object.
 
         :param method:
          The HTTP method of the route.
         :param path:
          The path of the route.
@@ -81,15 +80,15 @@
 
 class HTTPClient:
     """Serves as an HTTP client responsible for sending HTTP requests to the Twitch API."""
 
     __slots__ = ('__connection', '_client_id', '_client_secret', '__session', '_session_lock', '_user_agent',
                  '_refresh_token')
 
-    def __init__(self, *, connection: ConnectionState, client_id: str, client_secret: Optional[str]):
+    def __init__(self, *, connection: ConnectionState, client_id: str, client_secret: Optional[str]) -> None:
         """
         Initialize the HTTPClient object.
         """
         self.__connection = connection
         self._client_id = client_id
         self._client_secret = client_secret
         self.__session: Optional[ClientSession] = None
@@ -232,16 +231,14 @@
                     _logger.debug('Generating a new access token to refresh the existing one.')
                     route = Route(method='POST', url='https://id.twitch.tv/oauth2/token')
                     refresh: Refresh = await self.request(route=route, params=params)
                     # Updating the session headers.
                     self.__session.headers.update({'Authorization': f'Bearer {refresh["access_token"]}'})
                     _logger.debug('Session headers have been successfully updated with the new access token.')
                     await self.__connection.parse(event='refresh_token', data=refresh)
-                    # todo In connections...
-                    # self.core.dispatch('refresh_token', refresh['access_token'])
                     return refresh
         return None
 
     async def _validate_token(self, *, generate: bool = False) -> Validate:
         """
         Validating access token.
 
@@ -361,14 +358,15 @@
                 route = Route(method='POST', path='eventsub/subscriptions')
                 await self.request(route=route, json=data)
             except Forbidden:
                 raise Forbidden('Subscription `%s` is missing proper authorization' % subscription['name'])
             except BadRequest:
                 raise SubscriptionError(subscription=subscription['name'],
                                         version=subscription['version'])
+        await self.__connection.parse(event='ready')
 
     async def get_client(self) -> Broadcaster:
         """
         Retrieves the user with the associated access token.
 
         :return:
          The Broadcaster.
```

### Comparing `twitchify-1.0.1/twitch/message.py` & `twitchify-1.0.2/twitch/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,41 +21,46 @@
 FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
+
 if TYPE_CHECKING:
     from .types import message as msg
     from typing import List, Optional
 
 
 class Emote:
     """
     Represents a message emote.
     """
-    def __init__(self, *, emote: msg.Emote):
+    __slots__ = ('id', 'begin', 'end')
+
+    def __init__(self, *, emote: msg.Emote) -> None:
         self.id: str = emote['id']
         self.begin: int = emote['begin']
         self.end: int = emote['end']
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'<Emote id={self.id} begin={self.begin} end={self.end}>'
 
 
 class Message:
     """
     Represents a chat message.
     """
-    def __init__(self, *, message: msg.Message):
+    __slots__ = ('content', '_emotes')
+
+    def __init__(self, *, message: msg.Message) -> None:
         self.content: str = message['text']
         self._emotes: List[msg.Emote] = message['emotes']
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f'<Message message={self.content}>'
 
     def __str__(self) -> str:
         return self.content
 
     @property
     def emotes(self) -> Optional[List[Emote]]:
```

### Comparing `twitchify-1.0.1/twitch/moderation.py` & `twitchify-1.0.2/twitch/moderation.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
 class ShieldMode:
     """
     Represents a channel Shield Mode.
     """
     __slots__ = ('moderator', '_started_at', '_ended_at')
 
-    def __init__(self, mode: Union[md.ShieldModeBegin, md.ShieldModeEnd]):
+    def __init__(self, mode: Union[md.ShieldModeBegin, md.ShieldModeEnd]) -> None:
         self.moderator: User = User(user=mode, prefix='moderator_user')
         self._started_at: Optional[str] = mode.get('started_at')
         self._ended_at: Optional[str] = mode.get('ended_at')
 
     def __repr__(self) -> str:
         return f'<UnBan moderator={self.moderator} _started_at={self._started_at} _ended_at={self._ended_at}>'
```

### Comparing `twitchify-1.0.1/twitch/reward.py` & `twitchify-1.0.2/twitch/reward.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,41 +38,41 @@
 class _Image:
     """
     Represents a custom image for a reward.
     """
 
     __slots__ = ('url_1x', 'url_2x', 'url_4x')
 
-    def __init__(self, *, image: rd.Image):
+    def __init__(self, *, image: rd.Image) -> None:
         self.url_1x: str = image['url_1x']
         self.url_2x: str = image['url_2x']
         self.url_4x: str = image['url_4x']
 
 
 class _OptionalImage:
     """
     Represents an optional custom image for a reward.
     """
 
     __slots__ = ('url_1x', 'url_2x', 'url_4x')
 
-    def __init__(self, *, image: rd.OptionalImage):
+    def __init__(self, *, image: rd.OptionalImage) -> None:
         self.url_1x: Optional[str] = image['url_1x']
         self.url_2x: Optional[str] = image['url_2x']
         self.url_4x: Optional[str] = image['url_4x']
 
 
 class _MaxValue:
     """
     Represents a maximum value setting for a reward.
     """
 
     __slots__ = ('is_enabled', 'value')
 
-    def __init__(self, *, data: rd.MaxValue):
+    def __init__(self, *, data: rd.MaxValue) -> None:
         self.is_enabled: bool = data['is_enabled']
         self.value: int = data['value']
 
 
 class _MaxCooldown:
     """
     Represents a maximum cooldown setting for a reward.
@@ -173,24 +173,26 @@
 
     def __init__(self, reward: rd.BaseReward):
         self.id: str = reward['id']
         self.title: str = reward['title']
         self.cost: int = reward['cost']
         self.description: str = reward['prompt']
 
+    def __repr__(self) -> str:
+        return f'<_Reward id={self.id} title={self.title} cost={self.cost}>'
+
 
 class Redemption:
     """
     Represents a reward redemption.
     """
     __slots__ = ('id', 'user', 'status', 'reward', 'redeemed_at')
 
-    def __init__(self, redemption: rd.Redemption):
+    def __init__(self, redemption: rd.Redemption) -> None:
         self.id: str = redemption['id']
         self.user: User = User(user=redemption)
         self.status: str = redemption['status']
         self.reward: _Reward = _Reward(reward=redemption['reward'])
         self.redeemed_at: datetime = parse_rfc3339_timestamp(timestamp=redemption['redeemed_at'])
 
     def __repr__(self) -> str:
-        return f'<Redemption id={self.id} user={self.user} status={self.status}>'
-
+        return f'<Redemption id={self.id} user={self.user} reward={self.reward.__repr__()} status={self.status}>'
```

### Comparing `twitchify-1.0.1/twitch/state.py` & `twitchify-1.0.2/twitch/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,53 +31,53 @@
 from .moderation import Ban, UnBan, ShieldMode
 from .stream import Online, Offline, Shoutout
 from .reward import Reward, Redemption
 from .survey import Poll, Prediction
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
+    from typing import Optional, Dict, Callable, Any
     from .types.http import Refresh
     from .types.eventsub import (
         channel as chl,
         moderation as md,
         reward as rd,
         poll as pl,
         prediction as pd,
         charity as ch,
         goal as gl,
         hypertrain as ht,
         stream as sm,
         user as us)
-    from typing import Optional, Dict, Callable, Any
 
 import logging
 _logger = logging.getLogger(__name__)
 
 
 class ConnectionState:
     """
-    Represents the state of the connection to the Twitch API.
+    Represents the state of the connection.
     """
 
-    def __init__(self, dispatcher: Callable[..., Any]):
+    def __init__(self, dispatcher: Callable[..., Any]) -> None:
         self.broadcaster: Optional[Broadcaster] = None
         self._dispatch: Callable[..., Any] = dispatcher
 
     async def parse(self, event: str, data: Optional[Dict[str, Any]] = None) -> None:
         """
         Parse an event and dispatch it to the appropriate handler.
         """
         try:
             parse = self.__getattribute__('parse_' + event.replace('.', '_'))
             if data is None:
                 await parse()
             else:
                 await parse(data)
-        except AttributeError:
-            _logger.error(f'Failed to parse event: {event}')
+        except Exception as error:
+            _logger.error(f'Failed to parse event: {event}, {error}')
 
     async def parse_ready(self) -> None:
         """
         Parse ready event.
         """
         self._dispatch('ready')
 
@@ -377,8 +377,13 @@
         self._dispatch('stream_offline', _stream)
 
     async def parse_user_update(self, data: us.Update) -> None:
         """
         Parse a user update event.
         """
         _update = Update(update=data)
+        # Updating the broadcaster
+        self.broadcaster.name = _update.name
+        self.broadcaster.display_name = _update.display_name
+        self.broadcaster._description = _update.description
+        self.broadcaster.email = _update.email
         self._dispatch('user_update', _update)
```

### Comparing `twitchify-1.0.1/twitch/stream.py` & `twitchify-1.0.2/twitch/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 class Online:
     """
     Represents an online stream.
     """
     __slots__ = ('user', 'id', 'type', 'started_at')
 
-    def __init__(self, stream: sm.Online):
+    def __init__(self, stream: sm.Online) -> None:
         self.user: User = User(user=stream, prefix='broadcaster_user')
         self.id: str = stream['id']
         self.type: str = stream['type']
         self.started_at: datetime = parse_rfc3339_timestamp(timestamp=stream['started_at'])
 
     def __repr__(self) -> str:
         return f'<Online user={self.user} id={self.id} type={self.type} started_at={self.started_at}>'
@@ -97,12 +97,12 @@
 
 class Offline:
     """
     Represents an offline stream.
     """
     __slots__ = 'user'
 
-    def __init__(self, stream: sm.Offline):
+    def __init__(self, stream: sm.Offline) -> None:
         self.user: User = User(user=stream, prefix='broadcaster_user')
 
     def __repr__(self) -> str:
         return f'<Offline user={self.user}>'
```

### Comparing `twitchify-1.0.1/twitch/survey.py` & `twitchify-1.0.2/twitch/survey.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.0.1/twitch/types/gateway.py` & `twitchify-1.0.2/twitch/types/gateway.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.0.1/twitch/types/http.py` & `twitchify-1.0.2/twitch/types/http.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.0.1/twitch/types/message.py` & `twitchify-1.0.2/twitch/types/message.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.0.1/twitch/types/user.py` & `twitchify-1.0.2/twitch/types/user.py`

 * *Files identical despite different names*

### Comparing `twitchify-1.0.1/twitch/user.py` & `twitchify-1.0.2/twitch/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 class Update(User):
     """
     Represents a user updated his information.
     """
     __slots__ = ('description', 'email', 'email_verified')
 
-    def __init__(self, *, update: us.Update):
+    def __init__(self, *, update: us.Update) -> None:
         super().__init__(user=update)
         self.description: str = update['description']
         self.email: Optional[str] = update.get('email')  # Requires user:read:email scope
         self.email_verified: bool = update['email_verified']
 
     def __repr__(self) -> str:
         return f'<Update user={super().__repr__()} description={self.description} email={self.email}>'
```

### Comparing `twitchify-1.0.1/twitch/utils.py` & `twitchify-1.0.2/twitch/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 # Core
 from .types.eventsub.subscriptions import Subscriptions
 
 # Libraries
 from datetime import datetime
 import json
-import re
 import logging
 
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from .types.eventsub.subscriptions import SubscriptionPayload
     from typing import Optional, List
 try:
@@ -123,28 +122,14 @@
 
     :return:
      The parsed timestamp as a datetime object.
     """
     return datetime.fromisoformat(timestamp)
 
 
-def is_valid(login: str) -> bool:
-    """
-    Checks if a login is valid.
-
-    :param login:
-     The login to be checked.
-
-    :return:
-     True if the login is valid, False otherwise.
-    """
-    pattern = r"^[a-z0-9_]{1,25}$"
-    return not not re.match(pattern, login)
-
-
 class ColoredFormatter(logging.Formatter):
     """
     Setup chat formatter for logger
     """
     COLORS = {
         'DEBUG': '\033[36m',  # Cyan
         'INFO': '\033[37m',  # White
@@ -164,15 +149,14 @@
 def setup_logging() -> logging.getLogger:
     """
     Setup logger
     """
     formatter = ColoredFormatter('%(message)s')
     handler = logging.StreamHandler()
     handler.setFormatter(formatter)
-
     logger = logging.getLogger()
     logger.addHandler(handler)
     logger.setLevel(logging.INFO)
     return logger
 
 
 def get_subscriptions(*, events: List[str]) -> List[SubscriptionPayload]:
```

### Comparing `twitchify-1.0.1/twitchify.egg-info/SOURCES.txt` & `twitchify-1.0.2/twitchify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

