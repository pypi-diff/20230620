# Comparing `tmp/nonebot-plugin-all4one-0.1.0a2.tar.gz` & `tmp/nonebot-plugin-all4one-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-all4one-0.1.0a2.tar", last modified: Sun Mar 12 14:53:24 2023, max compression
+gzip compressed data, was "nonebot-plugin-all4one-0.1.0a3.tar", last modified: Tue Jun 20 14:59:23 2023, max compression
```

## Comparing `nonebot-plugin-all4one-0.1.0a2.tar` & `nonebot-plugin-all4one-0.1.0a3.tar`

### file list

```diff
@@ -1,31 +1,29 @@
--rw-r--r--   0        0        0    34523 2023-02-20 05:07:57.986890 nonebot-plugin-all4one-0.1.0a2/LICENSE
--rw-r--r--   0        0        0     2615 2023-03-08 11:16:09.748161 nonebot-plugin-all4one-0.1.0a2/README.md
--rw-r--r--   0        0        0     1296 2023-02-20 10:36:13.945476 nonebot-plugin-all4one-0.1.0a2/nonebot_plugin_all4one/__init__.py
--rw-r--r--   0        0        0      212 2023-02-20 05:07:57.986890 nonebot-plugin-all4one-0.1.0a2/nonebot_plugin_all4one/config.py
--rw-r--r--   0        0        0     4267 2023-03-03 15:08:14.531599 nonebot-plugin-all4one-0.1.0a2/nonebot_plugin_all4one/database/__init__.py
--rw-r--r--   0        0        0    17841 2023-03-09 03:59:16.620255 nonebot-plugin-all4one-0.1.0a2/nonebot_plugin_all4one/middlewares/__init__.py
--rw-r--r--   0        0        0     2577 2023-03-09 03:59:16.620255 nonebot-plugin-all4one-0.1.0a2/nonebot_plugin_all4one/middlewares/console.py
--rw-r--r--   0        0        0    14650 2023-03-09 03:59:16.623589 nonebot-plugin-all4one-0.1.0a2/nonebot_plugin_all4one/middlewares/onebot/v11.py
--rw-r--r--   0        0        0     3947 2023-03-11 07:54:31.359718 nonebot-plugin-all4one-0.1.0a2/nonebot_plugin_all4one/middlewares/onebot/v12.py
--rw-r--r--   0        0        0    19081 2023-03-12 14:43:48.015962 nonebot-plugin-all4one-0.1.0a2/nonebot_plugin_all4one/middlewares/qqguild.py
--rw-r--r--   0        0        0    13430 2023-03-11 07:54:31.363051 nonebot-plugin-all4one-0.1.0a2/nonebot_plugin_all4one/middlewares/telegram.py
--rw-r--r--   0        0        0     1120 2023-03-03 10:21:33.572655 nonebot-plugin-all4one-0.1.0a2/nonebot_plugin_all4one/migrations/6e6321bc6c48_init_db.py
--rw-r--r--   0        0        0      982 2023-03-03 10:21:33.572655 nonebot-plugin-all4one-0.1.0a2/nonebot_plugin_all4one/migrations/d0a1d19f3408_.py
--rw-r--r--   0        0        0    20002 2023-03-12 14:43:48.022629 nonebot-plugin-all4one-0.1.0a2/nonebot_plugin_all4one/onebotimpl/__init__.py
--rw-r--r--   0        0        0     1340 2023-02-28 15:31:28.882568 nonebot-plugin-all4one-0.1.0a2/nonebot_plugin_all4one/onebotimpl/config.py
--rw-r--r--   0        0        0      955 2023-03-03 10:21:33.572655 nonebot-plugin-all4one-0.1.0a2/nonebot_plugin_all4one/onebotimpl/utils.py
--rw-r--r--   0        0        0     1953 2023-03-12 14:51:28.739961 nonebot-plugin-all4one-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-26 11:16:56.602509 nonebot-plugin-all4one-0.1.0a2/tests/__init__.py
--rw-r--r--   0        0        0     2051 2023-03-08 06:59:18.958697 nonebot-plugin-all4one-0.1.0a2/tests/conftest.py
--rw-r--r--   0        0        0      969 2023-03-03 10:21:33.572655 nonebot-plugin-all4one-0.1.0a2/tests/database/test_database.py
--rw-r--r--   0        0        0      871 2023-03-04 04:30:42.494110 nonebot-plugin-all4one-0.1.0a2/tests/middlewares/onebot/events.json
--rw-r--r--   0        0        0     1047 2023-03-04 04:30:09.344112 nonebot-plugin-all4one-0.1.0a2/tests/middlewares/onebot/test_onebot_v11.py
--rw-r--r--   0        0        0      634 2023-03-11 07:54:31.363051 nonebot-plugin-all4one-0.1.0a2/tests/middlewares/onebot/test_onebot_v12.py
--rw-r--r--   0        0        0     1068 2023-02-26 11:16:56.602509 nonebot-plugin-all4one-0.1.0a2/tests/middlewares/qqguild/events.json
--rw-r--r--   0        0        0     1019 2023-03-03 14:40:58.460577 nonebot-plugin-all4one-0.1.0a2/tests/middlewares/qqguild/test_qqguild.py
--rw-r--r--   0        0        0     4272 2023-03-11 07:54:31.363051 nonebot-plugin-all4one-0.1.0a2/tests/middlewares/telegram/test_telegram.py
--rw-r--r--   0        0        0     7357 2023-03-03 14:31:45.176947 nonebot-plugin-all4one-0.1.0a2/tests/middlewares/telegram/updates.json
--rw-r--r--   0        0        0      365 2023-03-04 06:47:53.420417 nonebot-plugin-all4one-0.1.0a2/tests/onebotimpl/test_bot_connect.py
--rw-r--r--   0        0        0      870 2023-03-09 03:59:16.626922 nonebot-plugin-all4one-0.1.0a2/tests/onebotimpl/test_call_api.py
--rw-r--r--   0        0        0        0 2023-03-04 04:52:11.517387 nonebot-plugin-all4one-0.1.0a2/tests/onebotimpl/test_onebot_conn.py
--rw-r--r--   0        0        0     2891 1970-01-01 00:00:00.000000 nonebot-plugin-all4one-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-20 14:58:53.359576 nonebot-plugin-all4one-0.1.0a3/LICENSE
+-rw-r--r--   0        0        0     2538 2023-06-20 14:58:53.359576 nonebot-plugin-all4one-0.1.0a3/README.md
+-rw-r--r--   0        0        0     2193 2023-06-20 14:58:53.363577 nonebot-plugin-all4one-0.1.0a3/nonebot_plugin_all4one/__init__.py
+-rw-r--r--   0        0        0      212 2023-06-20 14:58:53.363577 nonebot-plugin-all4one-0.1.0a3/nonebot_plugin_all4one/config.py
+-rw-r--r--   0        0        0     4267 2023-06-20 14:58:53.363577 nonebot-plugin-all4one-0.1.0a3/nonebot_plugin_all4one/database/__init__.py
+-rw-r--r--   0        0        0      826 2023-06-20 14:58:53.363577 nonebot-plugin-all4one-0.1.0a3/nonebot_plugin_all4one/middlewares/__init__.py
+-rw-r--r--   0        0        0    17826 2023-06-20 14:58:53.363577 nonebot-plugin-all4one-0.1.0a3/nonebot_plugin_all4one/middlewares/base.py
+-rw-r--r--   0        0        0     2585 2023-06-20 14:58:53.363577 nonebot-plugin-all4one-0.1.0a3/nonebot_plugin_all4one/middlewares/console.py
+-rw-r--r--   0        0        0    14712 2023-06-20 14:58:53.363577 nonebot-plugin-all4one-0.1.0a3/nonebot_plugin_all4one/middlewares/onebot_v11.py
+-rw-r--r--   0        0        0    23737 2023-06-20 14:58:53.363577 nonebot-plugin-all4one-0.1.0a3/nonebot_plugin_all4one/middlewares/qqguild.py
+-rw-r--r--   0        0        0    13193 2023-06-20 14:58:53.363577 nonebot-plugin-all4one-0.1.0a3/nonebot_plugin_all4one/middlewares/telegram.py
+-rw-r--r--   0        0        0     1120 2023-06-20 14:58:53.363577 nonebot-plugin-all4one-0.1.0a3/nonebot_plugin_all4one/migrations/6e6321bc6c48_init_db.py
+-rw-r--r--   0        0        0      982 2023-06-20 14:58:53.363577 nonebot-plugin-all4one-0.1.0a3/nonebot_plugin_all4one/migrations/d0a1d19f3408_.py
+-rw-r--r--   0        0        0    20142 2023-06-20 14:58:53.363577 nonebot-plugin-all4one-0.1.0a3/nonebot_plugin_all4one/onebotimpl/__init__.py
+-rw-r--r--   0        0        0     1340 2023-06-20 14:58:53.363577 nonebot-plugin-all4one-0.1.0a3/nonebot_plugin_all4one/onebotimpl/config.py
+-rw-r--r--   0        0        0      955 2023-06-20 14:58:53.363577 nonebot-plugin-all4one-0.1.0a3/nonebot_plugin_all4one/onebotimpl/utils.py
+-rw-r--r--   0        0        0     2043 2023-06-20 14:58:53.367576 nonebot-plugin-all4one-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-20 14:58:53.367576 nonebot-plugin-all4one-0.1.0a3/tests/__init__.py
+-rw-r--r--   0        0        0     2006 2023-06-20 14:58:53.367576 nonebot-plugin-all4one-0.1.0a3/tests/conftest.py
+-rw-r--r--   0        0        0      969 2023-06-20 14:58:53.367576 nonebot-plugin-all4one-0.1.0a3/tests/database/test_database.py
+-rw-r--r--   0        0        0     1646 2023-06-20 14:58:53.367576 nonebot-plugin-all4one-0.1.0a3/tests/middlewares/onebot_v11/events.json
+-rw-r--r--   0        0        0     1412 2023-06-20 14:58:53.367576 nonebot-plugin-all4one-0.1.0a3/tests/middlewares/onebot_v11/test_onebot_v11.py
+-rw-r--r--   0        0        0     1446 2023-06-20 14:58:53.367576 nonebot-plugin-all4one-0.1.0a3/tests/middlewares/qqguild/events.json
+-rw-r--r--   0        0        0     1587 2023-06-20 14:58:53.367576 nonebot-plugin-all4one-0.1.0a3/tests/middlewares/qqguild/test_qqguild.py
+-rw-r--r--   0        0        0     4709 2023-06-20 14:58:53.367576 nonebot-plugin-all4one-0.1.0a3/tests/middlewares/telegram/test_telegram.py
+-rw-r--r--   0        0        0     7357 2023-06-20 14:58:53.367576 nonebot-plugin-all4one-0.1.0a3/tests/middlewares/telegram/updates.json
+-rw-r--r--   0        0        0      365 2023-06-20 14:58:53.367576 nonebot-plugin-all4one-0.1.0a3/tests/onebotimpl/test_bot_connect.py
+-rw-r--r--   0        0        0      870 2023-06-20 14:58:53.367576 nonebot-plugin-all4one-0.1.0a3/tests/onebotimpl/test_call_api.py
+-rw-r--r--   0        0        0     2814 1970-01-01 00:00:00.000000 nonebot-plugin-all4one-0.1.0a3/PKG-INFO
```

### Comparing `nonebot-plugin-all4one-0.1.0a2/LICENSE` & `nonebot-plugin-all4one-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-all4one-0.1.0a2/README.md` & `nonebot-plugin-all4one-0.1.0a3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -51,26 +51,25 @@
 blocked_plugins = ["echo"] # 在 block_event=False 时生效，可自定义处理流程中要中止的插件
 ```
 
 ## Feature
 
 ### OneBot
 
-- [x] HTTP 测试中
-- [x] HTTP Webhook 测试中
-- [x] 正向 WebSocket 测试中
+- [x] HTTP
+- [x] HTTP Webhook
+- [x] 正向 WebSocket
 - [x] 反向 WebSocket
 
 ### Middlewares
 
 - [x] Console
-- [x] OneBot V11 测试中
-- [x] OneBot V12
-- [x] Telegram 测试中
-- [x] QQ Guild [@he0119](https://github.com/he0119) 测试中
+- [x] OneBot V11
+- [x] Telegram
+- [x] QQ Guild [@he0119](https://github.com/he0119)
 - [ ] Kaiheila
 
 ## 相关链接
 
 - [nonebot-adapter-onebot](https://github.com/nonebot/adapter-onebot) 复用代码
 - [zhamao-robot/go-cqhttp-adapter-plugin](https://github.com/zhamao-robot/go-cqhttp-adapter-plugin) OneBot V11 -> V12 逻辑参考
 - [nonebot-plugin-params](https://github.com/iyume/nonebot-plugin-params) 灵感来源
```

### Comparing `nonebot-plugin-all4one-0.1.0a2/nonebot_plugin_all4one/database/__init__.py` & `nonebot-plugin-all4one-0.1.0a3/nonebot_plugin_all4one/database/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-all4one-0.1.0a2/nonebot_plugin_all4one/middlewares/__init__.py` & `nonebot-plugin-all4one-0.1.0a3/nonebot_plugin_all4one/middlewares/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,23 +27,14 @@
     BotStatus,
     MessageEvent,
     StatusUpdateMetaEvent,
 )
 
 from ..database import get_file, upload_file
 
-MIDDLEWARE_MAP = {
-    "Telegram": "telegram",
-    "Console": "console",
-    "QQ Guild": "qqguild",
-    "OneBot V12": "onebot.v12",
-    "OneBot V11": "onebot.v11",
-}
-
-
 _T = TypeVar("_T", bound=OneBotEvent)
 if TYPE_CHECKING:
 
     class _Queue(BaseQueue[_T]):
         pass
 
 else:
@@ -147,15 +138,17 @@
         if isinstance(event, BotEvent):
             event.self.user_id = "a4o@" + event.self.user_id
         if isinstance(event, StatusUpdateMetaEvent):
             for bot in event.status.bots:
                 bot.self.user_id = "a4o@" + bot.self.user_id
         if isinstance(event, MessageEvent):
             for msg in event.message:
-                if msg.type == "mention" and msg.data["user_id"] == self.self_id:
+                if msg.type == "reply" and msg.data["user_id"] == self.self_id:
+                    msg.data["user_id"] = "a4o@" + msg.data["user_id"]
+                elif msg.type == "mention" and msg.data["user_id"] == self.self_id:
                     msg.data["user_id"] = "a4o@" + msg.data["user_id"]
         return event
 
     @classmethod
     @abstractmethod
     def get_name(cls) -> str:
         """对应协议适配器的名称"""
```

### Comparing `nonebot-plugin-all4one-0.1.0a2/nonebot_plugin_all4one/middlewares/console.py` & `nonebot-plugin-all4one-0.1.0a3/nonebot_plugin_all4one/middlewares/console.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from nonebot.adapters.onebot.v12 import Message as OneBotMessage
 from nonebot.adapters.console.bot import Bot, Event, Message, MessageEvent
 from nonebot.adapters.onebot.v12 import MessageSegment as OneBotMessageSegment
 from nonebot.adapters.onebot.v12.event import (
     PrivateMessageEvent as OneBotPrivateMessageEvent,
 )
 
-from . import supported_action
-from . import Middleware as BaseMiddleware
+from .base import supported_action
+from .base import Middleware as BaseMiddleware
 
 
 class Middleware(BaseMiddleware):
     bot: Bot
 
     def __init__(self, bot: Bot):
         super().__init__(bot)
```

### Comparing `nonebot-plugin-all4one-0.1.0a2/nonebot_plugin_all4one/middlewares/onebot/v11.py` & `nonebot-plugin-all4one-0.1.0a3/nonebot_plugin_all4one/middlewares/onebot_v11.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,17 @@
     FriendAddNoticeEvent,
     GroupRecallNoticeEvent,
     FriendRecallNoticeEvent,
     GroupDecreaseNoticeEvent,
     GroupIncreaseNoticeEvent,
 )
 
-from .. import supported_action
-from .. import Middleware as BaseMiddleware
-from ...database import get_file, upload_file
+from .base import supported_action
+from ..database import get_file, upload_file
+from .base import Middleware as BaseMiddleware
 
 
 class Middleware(BaseMiddleware):
     bot: Bot
 
     async def _call_api(self, api: str, **kwargs: Any) -> Any:
         try:
@@ -85,14 +85,22 @@
         event_dict["id"] = uuid.uuid4().hex
         event_dict["type"] = event.post_type
         if not isinstance(event, MetaEvent):
             event_dict["self"] = self.get_bot_self().dict()
         if isinstance(event, MessageEvent):
             event_dict["detail_type"] = event.message_type
             event_dict["message"] = await self.to_onebot_message(event.original_message)
+            if event.reply:
+                event_dict["message"].insert(
+                    0,
+                    OneBotMessageSegment.reply(
+                        str(event.reply.message_id),
+                        user_id=str(event.reply.sender.user_id),
+                    ),
+                )
             event_dict["alt_message"] = event.raw_message
         elif isinstance(event, NoticeEvent):
             if isinstance(event, FriendRecallNoticeEvent):
                 event_dict["detail_type"] = "private_message_delete"
             elif isinstance(event, FriendAddNoticeEvent):
                 event_dict["detail_type"] = "friend_increase"
             elif isinstance(event, GroupIncreaseNoticeEvent):
@@ -168,20 +176,14 @@
                                 "",
                                 self.get_name(),
                                 segment.data["file"],
                             )
                         },
                     )
                 )
-            elif segment.type == "reply":
-                message_list.append(
-                    OneBotMessageSegment.reply(
-                        segment.data["id"], user_id=message["at", 0].data["qq"]
-                    )
-                )
         return OneBotMessage(message_list)
 
     async def from_onebot_message(self, message: OneBotMessage) -> Message:
         message_list = []
         for segment in message:
             if segment.type == "text":
                 message_list.append(MessageSegment.text(segment.data["text"]))
```

### Comparing `nonebot-plugin-all4one-0.1.0a2/nonebot_plugin_all4one/middlewares/telegram.py` & `nonebot-plugin-all4one-0.1.0a3/nonebot_plugin_all4one/middlewares/telegram.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,31 +4,29 @@
 from pydantic import parse_obj_as
 from nonebot.adapters.onebot.v12 import UnsupportedSegment
 from nonebot.adapters.telegram.message import File, Entity
 from nonebot.adapters.onebot.v12 import Event as OneBotEvent
 from nonebot.adapters.onebot.v12 import Adapter as OneBotAdapter
 from nonebot.adapters.onebot.v12 import Message as OneBotMessage
 from nonebot.adapters.telegram import Bot, Event, Adapter, Message
-from nonebot.adapters.telegram.model import Message as TelegramMessage
 from nonebot.adapters.onebot.v12 import MessageSegment as OneBotMessageSegment
 from nonebot.adapters.telegram.event import (
-    Chat,
     NoticeEvent,
     MessageEvent,
     ChannelPostEvent,
     GroupMessageEvent,
     NewChatMemberEvent,
     LeftChatMemberEvent,
     PrivateMessageEvent,
     ForumTopicMessageEvent,
 )
 
-from . import supported_action
-from . import Middleware as BaseMiddleware
+from .base import supported_action
 from ..database import get_file, upload_file
+from .base import Middleware as BaseMiddleware
 
 
 class Middleware(BaseMiddleware):
     bot: Bot
 
     @staticmethod
     def get_name():
@@ -45,15 +43,15 @@
         event_dict["type"] = type
         event_dict["self"] = self.get_bot_self().dict()
         if isinstance(event, MessageEvent):
             event_dict["time"] = event.date
             event_dict["detail_type"] = event.get_event_name().split(".")[1]
             event_dict["sub_type"] = ""
             event_dict["message_id"] = f"{event.chat.id}/{event.message_id}"
-            event_dict["message"] = await self.to_onebot_message(event.message)
+            event_dict["message"] = await self.to_onebot_message(event.original_message)
             event_dict["alt_message"] = str(event.message)
             if isinstance(event, PrivateMessageEvent):
                 event_dict["user_id"] = event.get_user_id()
             elif isinstance(event, ForumTopicMessageEvent):
                 event_dict["detail_type"] = "channel"
                 event_dict["guild_id"] = str(event.chat.id)
                 event_dict["channel_id"] = str(event.message_thread_id)
@@ -101,16 +99,21 @@
 
     async def to_onebot_message(self, message: Message) -> OneBotMessage:
         message_list = []
         for segment in message:
             if segment.type == "text":
                 message_list.append(OneBotMessageSegment.text(segment.data["text"]))
             elif segment.type == "mention":
+                if (user_name := segment.data["text"][1:]) == self.bot.username:
+                    message_list.append(OneBotMessageSegment.mention(self.bot.self_id))
+                else:
+                    message_list.append(OneBotMessageSegment.mention(user_name))
+            elif segment.type == "text_mention":
                 message_list.append(
-                    OneBotMessageSegment.mention(segment.data["text"][1:])
+                    OneBotMessageSegment.mention(str(segment.data["user"].id))
                 )
             elif isinstance(segment, Entity):
                 message_list.append(OneBotMessageSegment.text(str(segment)))
             elif segment.type == "photo":
                 message_list.append(OneBotMessageSegment.image(segment.data["file"]))
             elif segment.type in ("voice", "audio", "video"):
                 message_list.append(
@@ -129,33 +132,14 @@
                     Path(file.file_path).name,
                     self.get_platform(),
                     file.file_id,
                     url=f"https://api.telegram.org/file/bot{self.bot.bot_config.token}/{file.file_path}",
                 )
         return OneBotMessage(message_list)
 
-    async def send(
-        self,
-        chat_id: int,
-        message: Message,
-        message_thread_id: Optional[int] = None,
-        **kwargs,
-    ) -> Union[TelegramMessage, List[TelegramMessage]]:
-        class FakeEvent(Event):
-            chat: Chat
-
-        fake_event = FakeEvent(
-            **{
-                "chat": Chat(id=chat_id, type="private"),
-                "message_thread_id": message_thread_id,
-            }
-        )
-
-        return await self.bot.send(fake_event, message, **kwargs)
-
     @supported_action
     async def send_message(
         self,
         *,
         detail_type: Union[Literal["private", "group", "channel"], str],
         user_id: Optional[str] = None,
         group_id: Optional[str] = None,
@@ -204,24 +188,24 @@
 
         reply_to_message_id = None
         if message.count("reply"):
             reply_to_message_id = int(
                 message["reply", 0].data["message_id"].split("/")[1]
             )
 
-        result = await self.send(
+        result = await self.bot.send_to(
             int(chat_id),
             telegram_message,
             message_thread_id=int(channel_id) if channel_id else None,
             reply_to_message_id=reply_to_message_id,
             **kwargs,
         )
         if isinstance(result, list):
             result = result[0]
-        return {"message_id": str(result.message_id), "time": result.date}
+        return {"message_id": f"{chat_id}/{result.message_id}", "time": result.date}
 
     @supported_action
     async def delete_message(self, *, message_id: str, **kwargs: Any) -> None:
         await self.bot.delete_message(*map(int, message_id.split("/")))
 
     @supported_action
     async def get_self_info(
```

### Comparing `nonebot-plugin-all4one-0.1.0a2/nonebot_plugin_all4one/migrations/6e6321bc6c48_init_db.py` & `nonebot-plugin-all4one-0.1.0a3/nonebot_plugin_all4one/migrations/6e6321bc6c48_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-all4one-0.1.0a2/nonebot_plugin_all4one/migrations/d0a1d19f3408_.py` & `nonebot-plugin-all4one-0.1.0a3/nonebot_plugin_all4one/migrations/d0a1d19f3408_.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-all4one-0.1.0a2/nonebot_plugin_all4one/onebotimpl/__init__.py` & `nonebot-plugin-all4one-0.1.0a3/nonebot_plugin_all4one/onebotimpl/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 import uuid
 import asyncio
-import importlib
 from datetime import datetime
 from functools import partial
 from contextlib import asynccontextmanager
 from typing import (
     Any,
     Set,
     Dict,
@@ -427,14 +426,20 @@
                         logger.exception("HTTP Webhook Response action failed")
                 # 事件推送成功，并不做更多处理
                 elif resp.status_code == 204:
                     pass
                 # 事件推送失败
                 else:
                     logger.error(f"HTTP Webhook event push failed: {resp}")
+            except (NotImplementedError, TypeError):
+                logger.error(
+                    f"Current driver {self.driver.type} does not support http client"
+                )
+                middleware.queues.remove(queue)
+                break
             except Exception:
                 logger.exception("HTTP Webhook event push failed")
 
     async def _websocket_rev(
         self, middleware: Middleware, conn: WebsocketReverseConfig
     ) -> None:
         headers = {
@@ -475,47 +480,46 @@
                             "<y><bg #f8bbd0>WebSocket Closed</bg #f8bbd0></y>"
                         )
                     except Exception as e:
                         logger.opt(colors=True).exception(
                             "<r><bg #f8bbd0>Error while process data from websocket"
                             f"{escape_tag(str(conn.url))}. Trying to reconnect...</bg #f8bbd0></r>",
                         )
+            except (NotImplementedError, TypeError):
+                logger.error(
+                    f"Current driver {self.driver.type} does not support websocket server"
+                )
+                break
             except Exception as e:
                 logger.opt(colors=True).warning(
                     "<y><bg #f8bbd0>Error while setup websocket to "
                     f"{escape_tag(str(conn.url))}. Trying to reconnect...</bg #f8bbd0></y>",
                 )
             await asyncio.sleep(conn.reconnect_interval)
 
     def bot_disconnect(self, bot: Bot) -> None:
         if (middleware := self.middlewares.pop(bot.self_id, None)) is None:
             return
         for task in middleware.tasks:
             if not task.done():
                 task.cancel()
 
-    def import_middlewares(self, middlewares: Optional[Set[str]] = None):
+    def _register_middlewares(self, middlewares: Optional[Set[str]] = None):
         if middlewares is None:
             middlewares = set(self.driver._adapters.keys())
         for middleware in middlewares:
-            try:
-                if middleware in MIDDLEWARE_MAP:
-                    module = importlib.import_module(
-                        f"nonebot_plugin_all4one.middlewares.{MIDDLEWARE_MAP[middleware]}"
-                    )
-                    self.register_middleware(getattr(module, "Middleware"))
-                else:
-                    logger.error(f"Can not find middleware for Adapter {middleware}")
-            except Exception:
-                logger.exception(f"Can not load middleware for Adapter {middleware}:")
+            if middleware in MIDDLEWARE_MAP:
+                self.register_middleware(MIDDLEWARE_MAP[middleware])
+            else:
+                logger.error(f"Can not find middleware for Adapter {middleware}")
 
     def setup(self):
         @self.driver.on_startup
         async def _():
-            self.import_middlewares(self.config.middlewares)
+            self._register_middlewares(self.config.middlewares)
 
         @self.driver.on_shutdown
         async def _():
             for middleware in self.middlewares.values():
                 for task in middleware.tasks:
                     if not task.done():
                         task.cancel()
```

### Comparing `nonebot-plugin-all4one-0.1.0a2/nonebot_plugin_all4one/onebotimpl/config.py` & `nonebot-plugin-all4one-0.1.0a3/nonebot_plugin_all4one/onebotimpl/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-all4one-0.1.0a2/nonebot_plugin_all4one/onebotimpl/utils.py` & `nonebot-plugin-all4one-0.1.0a3/nonebot_plugin_all4one/onebotimpl/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-all4one-0.1.0a2/pyproject.toml` & `nonebot-plugin-all4one-0.1.0a3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [project]
 name = "nonebot-plugin-all4one"
-version = "0.1.0a2"
+version = "0.1.0a3"
 description = ""
 authors = [
     { name = "Jigsaw", email = "j1g5aw@foxmail.com" },
 ]
 dependencies = [
-    "nonebot2<3.0.0,>=2.0.0rc2",
-    "nonebot-adapter-onebot>=2.2.0",
-    "nonebot-plugin-datastore>=0.6.0a0",
+    "nonebot2<3.0.0,>=2.0.0",
+    "nonebot-adapter-onebot>=2.2.2",
+    "nonebot-plugin-datastore>=0.6.0",
 ]
 requires-python = ">=3.8,<4.0"
 readme = "README.md"
 
 [project.license]
 text = "AGPL-3.0-only"
 
 [project.optional-dependencies]
 telegram = [
-    "nonebot-adapter-telegram>=0.1.0b8",
+    "nonebot-adapter-telegram>=0.1.0b13",
 ]
 console = [
     "nonebot-adapter-console>=0.3.2",
 ]
 qqguild = [
     "nonebot-adapter-qqguild>=0.2.2",
 ]
@@ -41,22 +41,25 @@
     "websockets>=10.4",
     "uvicorn>=0.12.0,<0.21.0",
 ]
 adapters = [
     "nonebot-adapter-onebot @ git+https://github.com/nonebot/adapter-onebot.git",
     "nonebot-adapter-telegram @ git+https://github.com/nonebot/adapter-telegram.git",
     "nonebot-adapter-console @ git+https://github.com/nonebot/adapter-console.git",
-    "nonebot-adapter-qqguild>=0.2.2",
+    "nonebot-adapter-qqguild @ git+https://github.com/nonebot/adapter-qqguild.git",
 ]
 tests = [
     "nonebug>=0.3.1",
     "pytest-asyncio>=0.20.3",
     "pytest-cov>=4.0.0",
     "pytest-xdist>=3.2.0",
 ]
+impl = [
+    "nonebot-plugin-sentry>=0.2.2",
+]
 
 [tool.black]
 line-length = 88
 target-version = [
     "py38",
     "py39",
     "py310",
@@ -80,15 +83,15 @@
 all = false
 
 [tool.pyright]
 reportShadowedImports = false
 pythonVersion = "3.8"
 pythonPlatform = "All"
 extraPaths = [
-    "__pypackages__/3.8/lib/",
+    "__pypackages__/3.11/lib/",
 ]
 exclude = [
     "__pypackages__",
     "nonebot_plugin_all4one/migrations",
 ]
 
 [tool.pytest.ini_options]
```

### Comparing `nonebot-plugin-all4one-0.1.0a2/tests/conftest.py` & `nonebot-plugin-all4one-0.1.0a3/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,19 +23,14 @@
     driver = nonebot.get_driver()
     driver.register_adapter(OnebotV11Adapter)
     driver.register_adapter(OnebotV12Adapter)
     driver.register_adapter(QQGuildAdapter)
     driver.register_adapter(TelegramAdapter)
     driver.register_adapter(ConsoleAdapter)
 
-    nonebot.require("nonebot_plugin_all4one")
-    from nonebot_plugin_all4one import obimpl
-
-    obimpl.import_middlewares()
-
 
 @pytest.fixture
 def FakeMiddleware():
     from nonebot_plugin_all4one.middlewares import Middleware
 
     class FakeMiddleware(Middleware):
         @classmethod
@@ -48,25 +43,26 @@
         async def to_onebot_event(self, event):
             return []
 
     return FakeMiddleware
 
 
 @pytest.fixture
-async def app(nonebug_init: None, tmp_path: Path):
+async def app(nonebug_init: None, tmp_path: Path, monkeypatch: pytest.MonkeyPatch):
     nonebot.require("nonebot_plugin_all4one")
     from nonebot_plugin_datastore.db import init_db
     from nonebot_plugin_datastore import create_session
-    from nonebot_plugin_datastore.config import plugin_config
 
-    plugin_config.datastore_data_dir = tmp_path
+    import nonebot_plugin_all4one.database
 
     await init_db()
 
-    yield App()
+    with monkeypatch.context() as m:
+        m.setattr(nonebot_plugin_all4one.database, "FILE_PATH", tmp_path)
 
-    # 清空数据库
+        yield App()
 
+    # 清空数据库
     from nonebot_plugin_all4one.database import File
 
     async with create_session() as session:
         await session.execute(delete(File))
```

### Comparing `nonebot-plugin-all4one-0.1.0a2/tests/database/test_database.py` & `nonebot-plugin-all4one-0.1.0a3/tests/database/test_database.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-all4one-0.1.0a2/tests/middlewares/onebot/events.json` & `nonebot-plugin-all4one-0.1.0a3/tests/middlewares/onebot_v11/events.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {'insert': "[(2, OrderedDict([('_model', 'GroupMessageEvent'), ('self_id', 0), ('time', 0), "*

 * *           "('post_type', 'message'), ('message_type', 'group'), ('sub_type', 'normal'), "*

 * *           "('message_id', 1), ('user_id', 1), ('group_id', 1), ('message', '[CQ:reply,id=2] Test "*

 * *           "text'), ('raw_message', '[CQ:reply,id=2] Test text'), ('reply', OrderedDict([('group', "*

 * *           "True), ('group_id', 1), ('message_id', 2), ('real_id', 2), ('message_type', 'group'), "*

 * *           "('sender', Ord […]*

```diff
@@ -34,9 +34,46 @@
             "nickname": "Test",
             "sex": "unknown",
             "user_id": 1
         },
         "sub_type": "normal",
         "time": 0,
         "user_id": 1
+    },
+    {
+        "_model": "GroupMessageEvent",
+        "anonymous": null,
+        "font": 0,
+        "group_id": 1,
+        "message": "[CQ:reply,id=2] Test text",
+        "message_id": 1,
+        "message_type": "group",
+        "post_type": "message",
+        "raw_message": "[CQ:reply,id=2] Test text",
+        "reply": {
+            "group": true,
+            "group_id": 1,
+            "message": "",
+            "message_id": 2,
+            "message_type": "group",
+            "raw_message": "",
+            "real_id": 2,
+            "sender": {
+                "age": 0,
+                "nickname": "Test",
+                "sex": "unknown",
+                "user_id": 1
+            },
+            "time": 0
+        },
+        "self_id": 0,
+        "sender": {
+            "age": 0,
+            "nickname": "Test",
+            "sex": "unknown",
+            "user_id": 1
+        },
+        "sub_type": "normal",
+        "time": 0,
+        "user_id": 1
     }
 ]
```

### Comparing `nonebot-plugin-all4one-0.1.0a2/tests/middlewares/onebot/test_onebot_v11.py` & `nonebot-plugin-all4one-0.1.0a3/tests/middlewares/onebot_v11/test_onebot_v11.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from nonebug import App
 from nonebot.adapters.onebot.v11 import Bot, Adapter
 from nonebot.adapters.onebot.v12 import GroupMessageEvent, PrivateMessageEvent
 
 
 async def test_to_onebot_event(app: App):
-    from nonebot_plugin_all4one.middlewares.onebot.v11 import Middleware
+    from nonebot_plugin_all4one.middlewares.onebot_v11 import Middleware
 
     with (Path(__file__).parent / "events.json").open("r", encoding="utf8") as f:
         test_events = json.load(f)
 
     async with app.test_api() as ctx:
         bot = ctx.create_bot(base=Bot, self_id="0")
         middleware = Middleware(bot)
@@ -23,7 +23,15 @@
         assert event[0].message[0].type == "mention_all"
 
         event = Adapter.json_to_event(test_events[1])
         assert event
         event = await middleware.to_onebot_event(event)
         assert isinstance(event[0], GroupMessageEvent)
         assert event[0].message[0].type == "mention_all"
+
+        event = Adapter.json_to_event(test_events[2])
+        assert event
+        event = await middleware.to_onebot_event(event)
+        assert isinstance(event[0], GroupMessageEvent)
+        assert event[0].message[0].type == "reply"
+        assert event[0].message[0].data.get("message_id") == "2"
+        assert event[0].message[0].data.get("user_id") == "1"
```

### Comparing `nonebot-plugin-all4one-0.1.0a2/tests/middlewares/qqguild/events.json` & `nonebot-plugin-all4one-0.1.0a3/tests/middlewares/qqguild/events.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {'insert': "[(1, OrderedDict([('id', 222222222), ('guild_id', 11111111111111111111), ('name', "*

 * *           "'测试'), ('type', 0), ('sub_type', 0), ('position', None), ('parent_id', None), "*

 * *           "('owner_id', 22222222222222222222), ('private_type', 0), ('speak_permission', 1), "*

 * *           "('application_id', None), ('op_user_id', '22222222222222222222')]))]"}*

```diff
@@ -29,9 +29,23 @@
         "mentions": null,
         "message_reference": null,
         "reply": null,
         "seq": 644,
         "seq_in_channel": "644",
         "timestamp": "2023-02-26T13:23:59+08:00",
         "to_me": false
+    },
+    {
+        "application_id": null,
+        "guild_id": 11111111111111111111,
+        "id": 222222222,
+        "name": "\u6d4b\u8bd5",
+        "op_user_id": "22222222222222222222",
+        "owner_id": 22222222222222222222,
+        "parent_id": null,
+        "position": null,
+        "private_type": 0,
+        "speak_permission": 1,
+        "sub_type": 0,
+        "type": 0
     }
 ]
```

### Comparing `nonebot-plugin-all4one-0.1.0a2/tests/middlewares/telegram/test_telegram.py` & `nonebot-plugin-all4one-0.1.0a3/tests/middlewares/telegram/test_telegram.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import json
 from pathlib import Path
 
 from nonebug import App
+from nonebot.adapters.telegram import Bot, Event
 from nonebot.adapters.telegram.model import Chat
 from nonebot.adapters.telegram.model import Message
 from nonebot.adapters.telegram.config import BotConfig
 from nonebot.adapters.telegram.message import File, Entity
 from nonebot.adapters.onebot.v12 import PrivateMessageEvent
-from nonebot.adapters.telegram import Bot, Event, MessageSegment
 from nonebot.adapters.telegram.model import File as TelegramFile
 from nonebot.adapters.onebot.v12 import MessageSegment as OneBotMessageSegment
 
 bot_config = BotConfig(token="1234567890:ABCDEFGHIJKLMNOPQRSTUVWXYZABCDEFGHI")
 
 
 async def test_to_onebot_event(app: App):
     from nonebot_plugin_all4one.middlewares.telegram import Middleware
 
     with (Path(__file__).parent / "updates.json").open("r", encoding="utf8") as f:
         test_updates = json.load(f)
 
     async with app.test_api() as ctx:
-        bot = ctx.create_bot(base=Bot, self_id=bot_config)  # type:ignore
+        bot = ctx.create_bot(
+            base=Bot,
+            self_id=Bot.get_bot_id_by_token(bot_config.token),
+            config=bot_config,
+        )
         middleware = Middleware(bot)
 
         event = Event.parse_event(test_updates[0])
         event = await middleware.to_onebot_event(event)
         assert isinstance(event[0], PrivateMessageEvent)
 
         event = Event.parse_event(test_updates[3])
@@ -65,50 +69,60 @@
 
 
 async def test_send_message(app: App):
     from nonebot_plugin_all4one.database import upload_file
     from nonebot_plugin_all4one.middlewares.telegram import Middleware
 
     async with app.test_api() as ctx:
-        bot = ctx.create_bot(base=Bot, self_id=bot_config)  # type:ignore
-        middleware = Middleware(bot)
-
-        class FakeEvent(Event):
-            chat: Chat
-
-        fake_event = FakeEvent(
-            **{
-                "chat": Chat(id=1111, type="private"),
-                "message_thread_id": None,
-            }
+        bot = ctx.create_bot(
+            base=Bot,
+            self_id=Bot.get_bot_id_by_token(bot_config.token),
+            config=bot_config,
         )
+        middleware = Middleware(bot)
 
         file_id = await upload_file(
             name="test",
             data=b"test",
             src=middleware.get_platform(),
             src_id="test",
         )
-        ctx.should_call_send(
-            fake_event,
-            Entity.text("Test") + File.photo("test"),
-            Message(message_id=2222, date=1, chat=fake_event.chat),
-            reply_to_message_id=None,
+        ctx.should_call_api(
+            "send_photo",
+            {
+                "chat_id": 1111,
+                "message_thread_id": None,
+                "photo": "test",
+                "caption": "Test",
+                "caption_entities": None,
+                "disable_notification": None,
+                "protect_content": None,
+                "reply_to_message_id": None,
+                "allow_sending_without_reply": None,
+                "parse_mode": None,
+                "has_spoiler": None,
+                "reply_markup": None,
+            },
+            Message(message_id=2222, date=1, chat=Chat(type="private", id=1111)),
         )
         await middleware.send_message(
             detail_type="private",
             user_id="1111",
             message=OneBotMessageSegment.text("Test")
             + OneBotMessageSegment.image(file_id),
         )
 
 
 async def test_delete_message(app: App):
     from nonebot_plugin_all4one.middlewares.telegram import Middleware
 
     async with app.test_api() as ctx:
-        bot = ctx.create_bot(base=Bot, self_id=bot_config)  # type:ignore
+        bot = ctx.create_bot(
+            base=Bot,
+            self_id=Bot.get_bot_id_by_token(bot_config.token),
+            config=bot_config,
+        )
         middleware = Middleware(bot)
         ctx.should_call_api(
             "delete_message", {"chat_id": 1111, "message_id": 2222}, True
         )
         await middleware.delete_message(message_id="1111/2222")
```

### Comparing `nonebot-plugin-all4one-0.1.0a2/tests/middlewares/telegram/updates.json` & `nonebot-plugin-all4one-0.1.0a3/tests/middlewares/telegram/updates.json`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-all4one-0.1.0a2/tests/onebotimpl/test_call_api.py` & `nonebot-plugin-all4one-0.1.0a3/tests/onebotimpl/test_call_api.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-all4one-0.1.0a2/PKG-INFO` & `nonebot-plugin-all4one-0.1.0a3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-all4one
-Version: 0.1.0a2
+Version: 0.1.0a3
 License: AGPL-3.0-only
 Author-email: Jigsaw <j1g5aw@foxmail.com>
 Requires-Python: >=3.8,<4.0
 Provides-Extra: console
 Provides-Extra: qqguild
 Provides-Extra: telegram
 Description-Content-Type: text/markdown
@@ -62,26 +62,25 @@
 blocked_plugins = ["echo"] # 在 block_event=False 时生效，可自定义处理流程中要中止的插件
 ```
 
 ## Feature
 
 ### OneBot
 
-- [x] HTTP 测试中
-- [x] HTTP Webhook 测试中
-- [x] 正向 WebSocket 测试中
+- [x] HTTP
+- [x] HTTP Webhook
+- [x] 正向 WebSocket
 - [x] 反向 WebSocket
 
 ### Middlewares
 
 - [x] Console
-- [x] OneBot V11 测试中
-- [x] OneBot V12
-- [x] Telegram 测试中
-- [x] QQ Guild [@he0119](https://github.com/he0119) 测试中
+- [x] OneBot V11
+- [x] Telegram
+- [x] QQ Guild [@he0119](https://github.com/he0119)
 - [ ] Kaiheila
 
 ## 相关链接
 
 - [nonebot-adapter-onebot](https://github.com/nonebot/adapter-onebot) 复用代码
 - [zhamao-robot/go-cqhttp-adapter-plugin](https://github.com/zhamao-robot/go-cqhttp-adapter-plugin) OneBot V11 -> V12 逻辑参考
 - [nonebot-plugin-params](https://github.com/iyume/nonebot-plugin-params) 灵感来源
```

