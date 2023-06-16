# Comparing `tmp/villa-0.2.0.tar.gz` & `tmp/villa-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "villa-0.2.0.tar", max compression
+gzip compressed data, was "villa-0.3.0.tar", max compression
```

## Comparing `villa-0.2.0.tar` & `villa-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1062 2023-06-12 15:23:36.018385 villa-0.2.0/LICENSE
--rw-r--r--   0        0        0     2844 2023-06-12 15:23:36.018385 villa-0.2.0/README.md
--rw-r--r--   0        0        0     1034 2023-06-12 15:23:36.018385 villa-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      285 2023-06-12 15:23:36.018385 villa-0.2.0/villa/__init__.py
--rw-r--r--   0        0        0    38490 2023-06-12 15:23:36.018385 villa-0.2.0/villa/bot.py
--rw-r--r--   0        0        0     8160 2023-06-12 15:23:36.018385 villa-0.2.0/villa/event.py
--rw-r--r--   0        0        0      473 2023-06-12 15:23:36.022385 villa-0.2.0/villa/exception.py
--rw-r--r--   0        0        0     1504 2023-06-12 15:23:36.022385 villa-0.2.0/villa/log.py
--rw-r--r--   0        0        0    16316 2023-06-12 15:23:36.022385 villa-0.2.0/villa/message.py
--rw-r--r--   0        0        0     9982 2023-06-12 15:23:36.022385 villa-0.2.0/villa/models.py
--rw-r--r--   0        0        0      935 2023-06-12 15:23:36.022385 villa-0.2.0/villa/store.py
--rw-r--r--   0        0        0      822 2023-06-12 15:23:36.022385 villa-0.2.0/villa/typing.py
--rw-r--r--   0        0        0      995 2023-06-12 15:23:36.022385 villa-0.2.0/villa/utils.py
--rw-r--r--   0        0        0     3796 1970-01-01 00:00:00.000000 villa-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-16 13:41:35.807920 villa-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2844 2023-06-16 13:41:35.807920 villa-0.3.0/README.md
+-rw-r--r--   0        0        0     1034 2023-06-16 13:41:35.807920 villa-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      285 2023-06-16 13:41:35.807920 villa-0.3.0/villa/__init__.py
+-rw-r--r--   0        0        0    40237 2023-06-16 13:41:35.807920 villa-0.3.0/villa/bot.py
+-rw-r--r--   0        0        0     8160 2023-06-16 13:41:35.807920 villa-0.3.0/villa/event.py
+-rw-r--r--   0        0        0      473 2023-06-16 13:41:35.807920 villa-0.3.0/villa/exception.py
+-rw-r--r--   0        0        0     1504 2023-06-16 13:41:35.807920 villa-0.3.0/villa/log.py
+-rw-r--r--   0        0        0    16803 2023-06-16 13:41:35.807920 villa-0.3.0/villa/message.py
+-rw-r--r--   0        0        0    10411 2023-06-16 13:41:35.807920 villa-0.3.0/villa/models.py
+-rw-r--r--   0        0        0      935 2023-06-16 13:41:35.807920 villa-0.3.0/villa/store.py
+-rw-r--r--   0        0        0      822 2023-06-16 13:41:35.807920 villa-0.3.0/villa/typing.py
+-rw-r--r--   0        0        0      995 2023-06-16 13:41:35.807920 villa-0.3.0/villa/utils.py
+-rw-r--r--   0        0        0     3796 1970-01-01 00:00:00.000000 villa-0.3.0/PKG-INFO
```

### Comparing `villa-0.2.0/LICENSE` & `villa-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `villa-0.2.0/README.md` & `villa-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `villa-0.2.0/pyproject.toml` & `villa-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "villa"
-version = "0.2.0"
+version = "0.3.0"
 description = "米游社大别野Bot Python SDK。MiHoYo Villa Bot Python SDK."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/villa-py"
 repository = "https://github.com/CMHopeSunshine/villa-py"
 documentation = "https://github.com/CMHopeSunshine/villa-py"
```

### Comparing `villa-0.2.0/villa/bot.py` & `villa-0.3.0/villa/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .models import *
 from .message import Message
 from .exception import ActionFailed
 from .message import MessageSegment
 from .log import logger, _log_patcher
 from .utils import run_sync, escape_tag
 from .message import Link as LinkSegment
+from .message import Post as PostSegment
 from .message import Text as TextSegment
 from .message import Image as ImageSegment
 from .store import get_app, get_bot, store_bot
 from .message import RoomLink as RoomLinkSegment
 from .typing import T_Func, T_Handler, EventHandler
 from .message import MentionAll as MentionAllSegment
 from .message import MentionUser as MentionUserSegment
@@ -81,15 +82,15 @@
     def description(self) -> str:
         """Bot 介绍"""
         if self.bot_info is None:
             raise ValueError(f"Bot {self.bot_id} not connected")
         return self.bot_info.template.desc
 
     @property
-    def current_villa_id(self) -> str:
+    def current_villa_id(self) -> int:
         """Bot 最后收到的事件的大别野 ID"""
         if self.bot_info is None:
             raise ValueError(f"Bot {self.bot_id} not connected")
         return self.bot_info.villa_id
 
     def on_event(
         self, *event_type: Type[Event], block: bool = False, priority: int = 1
@@ -270,20 +271,26 @@
         返回:
             str: 消息 ID
         """
         if isinstance(message, str):
             message = MessageSegment.text(message)
         if isinstance(message, MessageSegment):
             message = Message(message)
-        content = await self._parse_message_content(message)
+        content_info = await self._parse_message_content(message)
+        if isinstance(content_info.content, TextMessageContent):
+            object_name = "MHY:Text"
+        elif isinstance(content_info.content, ImageMessageContent):
+            object_name = "MHY:Image"
+        else:
+            object_name = "MHY:Post"
         return await self.send_message(
             villa_id=villa_id,
             room_id=room_id,
-            object_name="MHY:Text",
-            msg_content=content,
+            object_name=object_name,
+            msg_content=content_info.json(by_alias=True, exclude_none=True),
         )
 
     async def check_member_bot_access_token(
         self, token: str, villa_id: Optional[int] = None
     ) -> CheckMemberBotAccessTokenReturn:
         """校验用户机器人访问凭证，并返回用户信息
 
@@ -752,15 +759,15 @@
         """
         return MemberRoleDetail.parse_obj(
             (
                 await self._request(
                     "GET",
                     "getMemberRoleInfo",
                     villa_id,
-                    json={"id": role_id},
+                    json={"role_id": role_id},
                 )
             )["role"]
         )
 
     async def get_villa_member_roles(self, villa_id: int) -> List[MemberRoleDetail]:
         """获取大别野下所有身份组
 
@@ -956,42 +963,47 @@
             )
 
     async def _parse_message_content(self, message: Message) -> MessageContentInfo:
         """解析消息内容"""
         if quote := message["quote", 0]:
             quote = QuoteInfo(**quote.dict())
 
-        if images_msg := (message["image"] or None):
+        if images_msg := (message["image"] or None):  # type: ignore
             images_msg: List[ImageSegment]
             images = [
                 Image(
                     url=seg.url,
                     size=ImageSize(width=seg.width, height=seg.height)
                     if seg.width and seg.height
                     else None,
                     file_size=seg.file_size,
                 )
                 for seg in images_msg
             ]
         else:
             images = None
+        if posts_msg := (message["post"] or None):  # type: ignore
+            posts_msg: List[PostSegment]
+            post_ids = [seg.post_id for seg in posts_msg]
+        else:
+            post_ids = None
         cal_len = lambda x: len(x.encode("utf-16")) // 2 - 1
         message_text = ""
         message_offset = 0
         entities: List[TextEntity] = []
         mentioned = MentionedInfo(type=MentionType.PART)
-        for seg in message:
+        for seg in message:  # type: ignore
             try:
-                if seg.type in ("quote", "image"):
+                if seg.type in ("quote", "image", "post"):
                     continue
                 if isinstance(seg, TextSegment):
                     seg_text = seg.content
                     length = cal_len(seg_text)
                 elif isinstance(seg, MentionAllSegment):
-                    seg_text = f"@{seg.data['show_text']} "
+                    seg_text = f"@{seg.show_text} "
                     length = cal_len(seg_text)
                     entities.append(
                         TextEntity(
                             offset=message_offset,
                             length=length,
                             entity=MentionedAll(show_text=seg.show_text),
                         )
@@ -1047,31 +1059,58 @@
                 else:
                     seg: LinkSegment
                     seg_text = seg.show_text
                     length = cal_len(seg_text)
                     entities.append(
                         TextEntity(
                             offset=message_offset,
-                            length=seg_text,
+                            length=length,
                             entity=Link(url=seg.url, show_text=seg.show_text),
                         )
                     )
                 message_offset += length
                 message_text += seg_text
             except Exception as e:
                 logger.opt(exception=e).warning("error when parse message content")
 
-        # 不能单独只发图片而没有其他文本内容
-        if images and not message_text:
-            message_text = "\u200B"
-
         if not (mentioned.type == MentionType.ALL and mentioned.user_id_list):
             mentioned = None
+
+        if not (message_text or entities):
+            if images:
+                if len(images) > 1:
+                    logger.warning(
+                        "Sending multiple images in one message will not be visible on the web side!"
+                    )
+                    content = TextMessageContent(text="\u200B", images=images)
+                else:
+                    content = ImageMessageContent(**images[0].dict())
+            elif post_ids:
+                if len(post_ids) > 1:
+                    logger.opt(colors=True).warning(
+                        f"Only support one post in one message, so use the last one <m>{post_ids[-1]}</m>!"
+                    )
+                content = PostMessageContent(post_id=post_ids[-1])
+            else:
+                raise ValueError("message content is empty")
+        else:
+            if images and message_text:
+                logger.warning(
+                    "When a message is accompanied by text and image, image will not visible on the web side!"
+                )
+            if post_ids and message_text:
+                logger.warning(
+                    "When a message is accompanied by text and post, post will not visible!"
+                )
+            content = TextMessageContent(
+                text=message_text, entities=entities, images=images
+            )
+
         return MessageContentInfo(
-            content=MessageContent(text=message_text, entities=entities, images=images),
+            content=content,
             mentionedInfo=mentioned,
             quote=quote,
         )
 
     def run(
         self,
         host: str = "127.0.0.1",
```

### Comparing `villa-0.2.0/villa/event.py` & `villa-0.3.0/villa/event.py`

 * *Files identical despite different names*

### Comparing `villa-0.2.0/villa/log.py` & `villa-0.3.0/villa/log.py`

 * *Files identical despite different names*

### Comparing `villa-0.2.0/villa/message.py` & `villa-0.3.0/villa/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     "mention_user",
     "mention_all",
     "mention_robot",
     "room_link",
     "link",
     "image",
     "quote",
+    "post",
 ]
 
 
 class MessageSegment(ABC, BaseModel):
     type: MessageType
     """消息段基类"""
 
@@ -42,14 +43,18 @@
         return RoomLink(villa_id=villa_id, room_id=room_id)
 
     @staticmethod
     def link(url: str, show_text: Optional[str] = None) -> "Link":
         return Link(url=url, show_text=show_text or url)
 
     @staticmethod
+    def post(post_id: str) -> "Post":
+        return Post(post_id=post_id)
+
+    @staticmethod
     def image(
         url: str,
         width: Optional[int] = None,
         height: Optional[int] = None,
         file_size: Optional[int] = None,
     ) -> "Image":
         return Image(url=url, width=width, height=height, file_size=file_size)
@@ -142,14 +147,21 @@
     type: Literal["quote"] = "quote"
     quoted_message_id: str
     quoted_message_send_time: int
     original_message_id: str
     original_message_send_time: int
 
 
+class Post(MessageSegment):
+    """帖子消息段"""
+
+    type: Literal["post"] = "post"
+    post_id: str
+
+
 class Message(BaseModel):
     __root__: List[MessageSegment] = Field(default_factory=list)
 
     def __init__(
         self,
         message: Union[
             str, MessageSegment, Iterable[MessageSegment], "Message", None
@@ -294,14 +306,26 @@
                 quoted_message_send_time=message_send_time,
                 original_message_id=message_id,
                 original_message_send_time=message_send_time,
             )
         )
         return self
 
+    def post(self, post_id: str) -> Self:
+        """帖子转发消息
+
+        参数:
+            post_id: 帖子ID
+
+        返回:
+            Self: 消息对象
+        """
+        self.__root__.append(Post(post_id=post_id))
+        return self
+
     def insert(self, index: int, segment: Union[str, MessageSegment]):
         """在指定位置插入消息段
 
         参数:
             index: 插入位置
             segment: 消息段
 
@@ -576,14 +600,15 @@
             "mention_user",
             "mention_all",
             "mention_robot",
             "room_link",
             "link",
             "image",
             "quote",
+            "post",
         ):
             if arg2 is None:
                 return Message([seg for seg in self.__root__ if seg.type == arg1])
             elif isinstance(arg2, int):
                 try:
                     return [seg for seg in self.__root__ if seg.type == arg1][arg2]
                 except IndexError:
```

### Comparing `villa-0.2.0/villa/models.py` & `villa-0.3.0/villa/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,20 +184,35 @@
 
 class Image(BaseModel):
     url: str
     size: Optional[ImageSize] = None
     file_size: Optional[int] = None
 
 
-class MessageContent(BaseModel):
+class PostMessageContent(BaseModel):
+    post_id: str
+
+    @validator("post_id")
+    def __deal_post_id(cls, v: str):
+        s = v.split("/")[-1]
+        if s.isdigit():
+            return s
+        raise ValueError(f"Invalid post_id: {v}, post_id must be a number.")
+
+
+class TextMessageContent(BaseModel):
     text: str
     entities: List[TextEntity] = Field(default_factory=list)
     images: Optional[List[Image]] = None
 
 
+class ImageMessageContent(Image):
+    pass
+
+
 class MentionedInfo(BaseModel):
     type: MentionType
     user_id_list: List[str] = Field(default_factory=list, alias="userIdList")
 
 
 class QuoteInfo(BaseModel):
     quoted_message_id: str
@@ -227,15 +242,15 @@
     action_type: int
     bot_msg_id: str
     client: str
     rong_sdk_version: str
 
 
 class MessageContentInfo(BaseModel):
-    content: MessageContent
+    content: Union[TextMessageContent, ImageMessageContent, PostMessageContent]
     mentioned_info: Optional[MentionedInfo] = Field(None, alias="mentionedInfo")
     quote: Optional[QuoteInfo] = None
     user: Optional[User] = None
     trace: Optional[Trace] = None
 
 
 # 房间部分
@@ -420,15 +435,17 @@
     "MentionType",
     "MentionedRobot",
     "MentionedUser",
     "MentionedAll",
     "VillaRoomLink",
     "Link",
     "TextEntity",
-    "MessageContent",
+    "TextMessageContent",
+    "ImageMessageContent",
+    "PostMessageContent",
     "MentionedInfo",
     "QuoteInfo",
     "User",
     "Trace",
     "ImageSize",
     "Image",
     "MessageContentInfo",
```

### Comparing `villa-0.2.0/villa/store.py` & `villa-0.3.0/villa/store.py`

 * *Files identical despite different names*

### Comparing `villa-0.2.0/villa/typing.py` & `villa-0.3.0/villa/typing.py`

 * *Files identical despite different names*

### Comparing `villa-0.2.0/villa/utils.py` & `villa-0.3.0/villa/utils.py`

 * *Files identical despite different names*

### Comparing `villa-0.2.0/PKG-INFO` & `villa-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: villa
-Version: 0.2.0
+Version: 0.3.0
 Summary: 米游社大别野Bot Python SDK。MiHoYo Villa Bot Python SDK.
 Home-page: https://github.com/CMHopeSunshine/villa-py
 License: MIT
 Keywords: mihoyo,bot,villa
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
```

