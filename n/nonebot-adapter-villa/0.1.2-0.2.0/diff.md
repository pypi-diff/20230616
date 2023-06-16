# Comparing `tmp/nonebot_adapter_villa-0.1.2.tar.gz` & `tmp/nonebot_adapter_villa-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_villa-0.1.2.tar", max compression
+gzip compressed data, was "nonebot_adapter_villa-0.2.0.tar", max compression
```

## Comparing `nonebot_adapter_villa-0.1.2.tar` & `nonebot_adapter_villa-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1062 2023-06-09 04:10:10.722784 nonebot_adapter_villa-0.1.2/LICENSE
--rw-r--r--   0        0        0     4154 2023-06-09 04:10:10.722784 nonebot_adapter_villa-0.1.2/README.md
--rw-r--r--   0        0        0      235 2023-06-09 04:10:10.722784 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/__init__.py
--rw-r--r--   0        0        0     4668 2023-06-09 04:10:10.722784 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/adapter.py
--rw-r--r--   0        0        0      114 2023-06-09 04:10:10.722784 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/api/__init__.py
--rw-r--r--   0        0        0     3247 2023-06-09 04:10:10.722784 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/api/cilent.pyi
--rw-r--r--   0        0        0     4109 2023-06-09 04:10:10.722784 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/api/client.py
--rw-r--r--   0        0        0    13301 2023-06-09 04:10:10.722784 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/api/handle.py
--rw-r--r--   0        0        0     9952 2023-06-09 04:10:10.722784 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/api/models.py
--rw-r--r--   0        0        0     1514 2023-06-09 04:10:10.722784 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/api/request.py
--rw-r--r--   0        0        0    11473 2023-06-09 04:10:10.722784 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/bot.py
--rw-r--r--   0        0        0      263 2023-06-09 04:10:10.722784 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/config.py
--rw-r--r--   0        0        0     8936 2023-06-09 04:10:10.726785 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/event.py
--rw-r--r--   0        0        0     1755 2023-06-09 04:10:10.726785 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/exception.py
--rw-r--r--   0        0        0     6279 2023-06-09 04:10:10.726785 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/message.py
--rw-r--r--   0        0        0       76 2023-06-09 04:10:10.726785 nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/utils.py
--rw-r--r--   0        0        0     1134 2023-06-09 04:10:10.726785 nonebot_adapter_villa-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5055 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-16 14:06:25.691916 nonebot_adapter_villa-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5070 2023-06-16 14:06:25.691916 nonebot_adapter_villa-0.2.0/README.md
+-rw-r--r--   0        0        0      235 2023-06-16 14:06:25.691916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/__init__.py
+-rw-r--r--   0        0        0     4668 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/adapter.py
+-rw-r--r--   0        0        0      114 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/api/__init__.py
+-rw-r--r--   0        0        0     2905 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/api/cilent.pyi
+-rw-r--r--   0        0        0     3714 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/api/client.py
+-rw-r--r--   0        0        0    12434 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/api/handle.py
+-rw-r--r--   0        0        0    10411 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/api/models.py
+-rw-r--r--   0        0        0     1514 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/api/request.py
+-rw-r--r--   0        0        0    12230 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/bot.py
+-rw-r--r--   0        0        0      263 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/config.py
+-rw-r--r--   0        0        0     8936 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/event.py
+-rw-r--r--   0        0        0     1755 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/exception.py
+-rw-r--r--   0        0        0     6704 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/message.py
+-rw-r--r--   0        0        0       76 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/utils.py
+-rw-r--r--   0        0        0     1134 2023-06-16 14:06:25.695916 nonebot_adapter_villa-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5971 1970-01-01 00:00:00.000000 nonebot_adapter_villa-0.2.0/PKG-INFO
```

### Comparing `nonebot_adapter_villa-0.1.2/LICENSE` & `nonebot_adapter_villa-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.1.2/README.md` & `nonebot_adapter_villa-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -4,17 +4,25 @@
 
 <div align="center">
 
 # NoneBot-Adapter-Villa
 
 _✨ 大别野 协议适配 ✨_
 
+<a href="https://cdn.jsdelivr.net/gh/CMHopeSunshine/nonebot-adapter-villa@master/LICENSE">
+  <img src="https://img.shields.io/github/license/CMHopeSunshine/nonebot-adapter-villa" alt="license">
+</a>
 <img src="https://img.shields.io/pypi/v/nonebot-adapter-villa" alt="version">
 <img src="https://img.shields.io/badge/Python-3.8+-yellow" alt="python">
-<a href="https://cdn.jsdelivr.net/gh/CMHopeSunshine/nonebot-adapter-villa@master/LICENSE"><img src="https://img.shields.io/github/license/CMHopeSunshine/nonebot-adapter-villa" alt="license"></a>
+<a href="https://pypi.python.org/pypi/nonebot-adapter-villa">
+  <img src="https://img.shields.io/pypi/dm/nonebot-adapter-villa" alt="pypi download">
+</a>
+<a href="https://wakatime.com/badge/user/eed3f89c-5d65-46e6-ab19-78dcc4b62b3f/project/838e7f55-f8b8-49ff-aec0-29ad264931cf">
+  <img src="https://wakatime.com/badge/user/eed3f89c-5d65-46e6-ab19-78dcc4b62b3f/project/838e7f55-f8b8-49ff-aec0-29ad264931cf.svg" alt="wakatime">
+</a>
 
 </div>
 
 ## 安装
 
 在`NoneBot2`项目目录下使用脚手架安装：
 
@@ -34,15 +42,15 @@
 
 ```dotenv
 DRIVER=~fastapi+~httpx
 ```
 
 ### VILLA_BOTS
 
-配置机器人帐号列表，每个bot有3个必填配置，在大别野官方机器人开发者社区(别野ID: OpenVilla)申请时获得，
+配置机器人帐号列表，每个bot有3个必填配置，在大别野[官方机器人开发者社区](https://dby.miyoushe.com/chat/463/20020)(别野ID: OpenVilla)申请时获得，
 
 - bot_id: 机器人id，以`bot_`开头
 - bot_secret: 机器人密钥
 - callback_url: http回调地址，例如申请bot时给的回调地址是`http://域名/your/callback/url`，那么配置里的`callback_url`填写`/your/callback/url`
   例如：
 
 ```dotenv
@@ -55,14 +63,16 @@
   }
 ]
 '
 ```
 
 ## 示例
 
+> 注意，当前大别野只能接收到有@Bot(在哪个位置皆可)的消息事件，且不能有多个@(即使是@两次Bot都不行)
+
 ### 消息段展示
 
 以下是一个简单的插件示例，展示各种消息段：
 
 ```python
 from nonebot import on_command
 from nonebot.params import CommandArg
@@ -87,19 +97,24 @@
             msg += MessageSegment.room_link(event.villa_id, event.room_id)
         elif arg == "链接":
             msg += MessageSegment.link("https://www.miyoushe.com/ys/article/39670307", show_text="这是链接")
             # 使用link的话链接能够点击进行跳转，使用text的话不能点击
             # show_text是指链接显示的文字，但在当前版本Web端大别野会无法正常跳转，最好不使用该参数
         elif arg == "图片":
             msg += MessageSegment.image("https://www.miyoushe.com/_nuxt/img/miHoYo_Game.2457753.png")
-            # 暂时只支持url图片，但在当前版本web端无法显示图片，待官方后续修复
+            # 暂时只支持url图片
+            # 如果在单次消息中，发送多张图片或者与其他消息段拼接，那么将无法在web端显示出来
+            # 所以建议每张图片单独发送
+        elif arg == "帖子":
+            msg += MessageSegment.post("https://www.miyoushe.com/ys/article/40391314")
+            # 帖子消息段只能单独发送，和其他消息段拼接时将被无视
     await matcher.finish(msg)
 ```
 
-使用命令`@bot /发送 艾特我 艾特bot 文字 房间 链接 图片`时，bot会回复`@你的名字 @bot的名字 文字 #房间名 这是链接 图片内容`
+使用命令`@bot /发送 艾特我 艾特bot 文字 房间 链接`时，bot会回复`@你的名字 @bot的名字 文字 #房间名 这是链接`
 
 
 ## 交流和反馈
 
 目前无论是大别野Bot还是本适配器都在测试开发中，如遇问题请提出issue，感谢支持！
 
 也欢迎来我的大别野【尘世闲游】进行交流：
```

#### html2text {}

```diff
@@ -1,47 +1,53 @@
                             [nonebot-adapter-villa]
- # NoneBot-Adapter-Villa _â¨ å¤§å«é åè®®éé â¨_ [version] [python]
-                                   [license]
+ # NoneBot-Adapter-Villa _â¨ å¤§å«é åè®®éé â¨_ [license] [version]
+                      [python] [pypi_download] [wakatime]
 ## å®è£ å¨`NoneBot2`é¡¹ç®ç®å½ä¸ä½¿ç¨èææ¶å®è£ï¼ ``` nb adapter
 install nonebot-adapter-villa ``` ## éç½® ä¿®æ¹ NoneBot éç½®æä»¶ `.env`
 æè `.env.*`ã ### Driver
 æ¬ééå¨åæ¶éè¦`ReverseDriver`å`ForwardDriver`ï¼åè [driver]
 (https://v2.nonebot.dev/docs/next/advanced/
 driver#%E9%A9%B1%E5%8A%A8%E5%99%A8%E7%B1%BB%E5%9E%8B) éç½®é¡¹ã ä¾å¦ï¼
 ```dotenv DRIVER=~fastapi+~httpx ``` ### VILLA_BOTS
-éç½®æºå¨äººå¸å·åè¡¨ï¼æ¯ä¸ªbotæ3ä¸ªå¿å¡«éç½®ï¼å¨å¤§å«éå®æ¹æºå¨äººå¼åèç¤¾åº
+éç½®æºå¨äººå¸å·åè¡¨ï¼æ¯ä¸ªbotæ3ä¸ªå¿å¡«éç½®ï¼å¨å¤§å«é
+[å®æ¹æºå¨äººå¼åèç¤¾åº](https://dby.miyoushe.com/chat/463/20020)
 (å«éID: OpenVilla)ç³è¯·æ¶è·å¾ï¼ - bot_id: æºå¨äººidï¼ä»¥`bot_`å¼å¤´
 - bot_secret: æºå¨äººå¯é¥ - callback_url:
 httpåè°å°åï¼ä¾å¦ç³è¯·botæ¶ç»çåè°å°åæ¯`http://åå/your/
 callback/url`ï¼é£ä¹éç½®éç`callback_url`å¡«å`/your/callback/url`
 ä¾å¦ï¼ ```dotenv VILLA_BOTS=' [ { "bot_id": "bot_123456789", "bot_secret":
-"abc123def456", "callback_url": "/your/callback/url" } ] ' ``` ## ç¤ºä¾ ###
-æ¶æ¯æ®µå±ç¤º ä»¥ä¸æ¯ä¸ä¸ªç®åçæä»¶ç¤ºä¾ï¼å±ç¤ºåç§æ¶æ¯æ®µï¼
-```python from nonebot import on_command from nonebot.params import CommandArg
-from nonebot.adapters.villa import Bot, SendMessageEvent, Message,
-MessageSegment matcher = on_command('åé') @matcher.handle() async def
-matcher_handler(bot: Bot, event: SendMessageEvent, cmd_arg: Message =
-CommandArg()): msg = Message() args = cmd_arg.extract_plain_text().strip
-().split(' ') for arg in args: if arg == "è¾ç¹æ": msg +=
-MessageSegment.mention_user(event.villa_id, event.from_user_id) elif arg ==
-"è¾ç¹bot": msg += MessageSegment.mention_robot(bot.self_id, bot.nickname)
-elif arg == "æå­": msg += MessageSegment.text("æå­") #
-è¡¨æä¹æ¯ç¨textæ¥åéï¼ä»¥[è¡¨æå]æ ¼å¼ï¼ä¾å¦MessageSegment.text
-("[ç±å¿]") elif arg == "æ¿é´": msg += MessageSegment.room_link
-(event.villa_id, event.room_id) elif arg == "é¾æ¥": msg +=
-MessageSegment.link("https://www.miyoushe.com/ys/article/39670307",
-show_text="è¿æ¯é¾æ¥") #
+"abc123def456", "callback_url": "/your/callback/url" } ] ' ``` ## ç¤ºä¾ >
+æ³¨æï¼å½åå¤§å«éåªè½æ¥æ¶å°æ@Bot
+(å¨åªä¸ªä½ç½®çå¯)çæ¶æ¯äºä»¶ï¼ä¸ä¸è½æå¤ä¸ª@
+(å³ä½¿æ¯@ä¸¤æ¬¡Boté½ä¸è¡) ### æ¶æ¯æ®µå±ç¤º
+ä»¥ä¸æ¯ä¸ä¸ªç®åçæä»¶ç¤ºä¾ï¼å±ç¤ºåç§æ¶æ¯æ®µï¼ ```python from
+nonebot import on_command from nonebot.params import CommandArg from
+nonebot.adapters.villa import Bot, SendMessageEvent, Message, MessageSegment
+matcher = on_command('åé') @matcher.handle() async def matcher_handler(bot:
+Bot, event: SendMessageEvent, cmd_arg: Message = CommandArg()): msg = Message()
+args = cmd_arg.extract_plain_text().strip().split(' ') for arg in args: if arg
+== "è¾ç¹æ": msg += MessageSegment.mention_user(event.villa_id,
+event.from_user_id) elif arg == "è¾ç¹bot": msg +=
+MessageSegment.mention_robot(bot.self_id, bot.nickname) elif arg == "æå­":
+msg += MessageSegment.text("æå­") # è¡¨æä¹æ¯ç¨textæ¥åéï¼ä»¥
+[è¡¨æå]æ ¼å¼ï¼ä¾å¦MessageSegment.text("[ç±å¿]") elif arg == "æ¿é´":
+msg += MessageSegment.room_link(event.villa_id, event.room_id) elif arg ==
+"é¾æ¥": msg += MessageSegment.link("https://www.miyoushe.com/ys/article/
+39670307", show_text="è¿æ¯é¾æ¥") #
 ä½¿ç¨linkçè¯é¾æ¥è½å¤ç¹å»è¿è¡è·³è½¬ï¼ä½¿ç¨textçè¯ä¸è½ç¹å» #
 show_textæ¯æé¾æ¥æ¾ç¤ºçæå­ï¼ä½å¨å½åçæ¬Webç«¯å¤§å«éä¼æ æ³æ­£å¸¸è·³è½¬ï¼æå¥½ä¸ä½¿ç¨è¯¥åæ°
 elif arg == "å¾ç": msg += MessageSegment.image("https://www.miyoushe.com/
-_nuxt/img/miHoYo_Game.2457753.png") #
-ææ¶åªæ¯æurlå¾çï¼ä½å¨å½åçæ¬webç«¯æ æ³æ¾ç¤ºå¾çï¼å¾å®æ¹åç»­ä¿®å¤
+_nuxt/img/miHoYo_Game.2457753.png") # ææ¶åªæ¯æurlå¾ç #
+å¦æå¨åæ¬¡æ¶æ¯ä¸­ï¼åéå¤å¼ å¾çæèä¸å¶ä»æ¶æ¯æ®µæ¼æ¥ï¼é£ä¹å°æ æ³å¨webç«¯æ¾ç¤ºåºæ¥
+# æä»¥å»ºè®®æ¯å¼ å¾çåç¬åé elif arg == "å¸å­": msg +=
+MessageSegment.post("https://www.miyoushe.com/ys/article/40391314") #
+å¸å­æ¶æ¯æ®µåªè½åç¬åéï¼åå¶ä»æ¶æ¯æ®µæ¼æ¥æ¶å°è¢«æ è§
 await matcher.finish(msg) ``` ä½¿ç¨å½ä»¤`@bot /åé è¾ç¹æ è¾ç¹bot
-æå­ æ¿é´ é¾æ¥ å¾ç`æ¶ï¼botä¼åå¤`@ä½ çåå­ @botçåå­
-æå­ #æ¿é´å è¿æ¯é¾æ¥ å¾çåå®¹` ## äº¤æµååé¦
+æå­ æ¿é´ é¾æ¥`æ¶ï¼botä¼åå¤`@ä½ çåå­ @botçåå­ æå­
+#æ¿é´å è¿æ¯é¾æ¥` ## äº¤æµååé¦
 ç®åæ è®ºæ¯å¤§å«éBotè¿æ¯æ¬ééå¨é½å¨æµè¯å¼åä¸­ï¼å¦éé®é¢è¯·æåºissueï¼æè°¢æ¯æï¼
 ä¹æ¬¢è¿æ¥æçå¤§å«éãå°ä¸é²æ¸¸ãè¿è¡äº¤æµï¼ - å¤§å«éID:
 wgiJNaUï¼å¯æç´¢å å¥ - [Webç«¯é¾æ¥](https://dby.miyoushe.com/chat/1047/
 21652)ï¼ç®åä»PCç«¯å¯è®¿é® ## ç¸å³é¡¹ç® - [NoneBot2](https://
 github.com/nonebot/nonebot2): éå¸¸å¥½ç¨çPythonè·¨å¹³å°æºå¨äººæ¡æ¶ï¼
 - [villa-py](https://github.com/CMHopeSunshine/villa-py): å¤§å«é Bot Python
 SDKã
```

### Comparing `nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/adapter.py` & `nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/api/cilent.pyi` & `nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/api/cilent.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union, Literal
+from typing import List, Union
 
 from .models import *
 
 class ApiClient:
     async def check_member_bot_access_token(
         self, *, villa_id: int, token: str
     ) -> CheckMemberBotAccessTokenReturn: ...
@@ -35,24 +35,14 @@
     async def create_group(self, *, villa_id: int, group_name: str) -> int: ...
     async def edit_group(
         self, *, villa_id: int, group_id: int, group_name: str
     ) -> None: ...
     async def delete_group(self, *, villa_id: int, group_id: int) -> None: ...
     async def get_group_list(self, *, villa_id: int) -> List[Group]: ...
     async def sort_group_list(self, *, villa_id: int, group_ids: List[int]) -> None: ...
-    async def create_room(
-        self,
-        *,
-        villa_id: int,
-        room_name: str,
-        room_type: Union[Literal[1, 2, 3], CreateRoomType],
-        group_id: int,
-        room_default_notify_type: Union[Literal[1, 2], CreateRoomDefaultNotifyType],
-        send_msg_auth_range: SendMsgAuthRange,
-    ) -> Room: ...
     async def edit_room(
         self, *, villa_id: int, room_id: int, room_name: str
     ) -> None: ...
     async def delete_room(self, *, villa_id: int, room_id: int) -> None: ...
     async def get_room(self, *, villa_id: int, room_id: int) -> Room: ...
     async def get_villa_group_room_list(self, *, villa_id: int) -> GroupRoom: ...
     async def sort_room_list(
```

### Comparing `nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/api/client.py` & `nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/api/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, List, Union, Literal
+from typing import TYPE_CHECKING, List, Union
 
 from .models import *
 
 if TYPE_CHECKING:
 
     class ApiClient:
         async def check_member_bot_access_token(
@@ -63,26 +63,14 @@
 
         async def get_group_list(self, *, villa_id: int) -> List[Group]:
             ...
 
         async def sort_group_list(self, *, villa_id: int, group_ids: List[int]) -> None:
             ...
 
-        async def create_room(
-            self,
-            *,
-            villa_id: int,
-            room_name: str,
-            room_type: Union[Literal[1, 2, 3], CreateRoomType],
-            group_id: int,
-            room_default_notify_type: Union[Literal[1, 2], CreateRoomDefaultNotifyType],
-            send_msg_auth_range: SendMsgAuthRange,
-        ) -> Room:
-            ...
-
         async def edit_room(
             self, *, villa_id: int, room_id: int, room_name: str
         ) -> None:
             ...
 
         async def delete_room(self, *, villa_id: int, room_id: int) -> None:
             ...
```

### Comparing `nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/api/handle.py` & `nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/api/handle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, List, Union, Literal
+from typing import TYPE_CHECKING, List, Union
 
 from pydantic import parse_obj_as
 from nonebot.drivers import Request
 
 from .models import *
 from .request import _request
 
@@ -186,39 +186,14 @@
         url=adapter.base_url / "vila/api/bot/platform/sortGroupList",
         headers=bot.get_authorization_header(villa_id),
         json={"villa_id": villa_id, "group_ids": group_ids},
     )
     await _request(adapter, bot, request)
 
 
-async def _create_room(
-    adapter: "Adapter",
-    bot: "Bot",
-    villa_id: int,
-    room_name: str,
-    room_type: Union[Literal[1, 2, 3], CreateRoomType],
-    group_id: int,
-    room_default_notify_type: Union[Literal[1, 2], CreateRoomDefaultNotifyType],
-    send_msg_auth_range: SendMsgAuthRange,
-) -> Room:
-    request = Request(
-        method="POST",
-        url=adapter.base_url / "vila/api/bot/platform/createRoom",
-        headers=bot.get_authorization_header(villa_id),
-        json={
-            "room_name": room_name,
-            "room_type": room_type,
-            "group_id": group_id,
-            "room_default_notify_type": room_default_notify_type,
-            "send_msg_auth_range": send_msg_auth_range.dict(),
-        },
-    )
-    return parse_obj_as(Room, (await _request(adapter, bot, request))["room"])
-
-
 async def _edit_room(
     adapter: "Adapter", bot: "Bot", villa_id: int, room_id: int, room_name: str
 ) -> None:
     request = Request(
         method="POST",
         url=adapter.base_url / "vila/api/bot/platform/editRoom",
         headers=bot.get_authorization_header(villa_id),
@@ -341,15 +316,15 @@
 async def _get_member_role_info(
     adapter: "Adapter", bot: "Bot", villa_id: int, role_id: int
 ) -> MemberRoleDetail:
     request = Request(
         method="GET",
         url=adapter.base_url / "vila/api/bot/platform/getMemberRoleInfo",
         headers=bot.get_authorization_header(villa_id),
-        json={"id": role_id},
+        json={"role_id": role_id},
     )
     return parse_obj_as(
         MemberRoleDetail, (await _request(adapter, bot, request))["role"]
     )
 
 
 async def _get_villa_member_roles(
@@ -405,15 +380,14 @@
     "recall_message": _recall_message,
     "send_message": _send_message,
     "create_group": _create_group,
     "edit_group": _edit_group,
     "delete_group": _delete_group,
     "get_group_list": _get_group_list,
     "sort_group_list": _sort_group_list,
-    "create_room": _create_room,
     "edit_room": _edit_room,
     "delete_room": _delete_room,
     "get_room": _get_room,
     "get_villa_group_room_list": _get_villa_group_room_list,
     "sort_room_list": _sort_room_list,
     "operate_member_to_role": _operate_member_to_role,
     "create_member_role": _create_member_role,
```

### Comparing `nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/api/models.py` & `nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/api/models.py`

 * *Files 3% similar despite different names*

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
-    entities: List[TextEntity]
+    entities: List[TextEntity] = Field(default_factory=list)
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

### Comparing `nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/api/request.py` & `nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/api/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/bot.py` & `nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/bot.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,18 @@
     MentionType,
     MentionedAll,
     RobotCommand,
     MentionedInfo,
     MentionedUser,
     VillaRoomLink,
     MentionedRobot,
-    MessageContent,
     MessageContentInfo,
+    PostMessageContent,
+    TextMessageContent,
+    ImageMessageContent,
 )
 
 if TYPE_CHECKING:
     from .adapter import Adapter
 
 
 async def _check_reply(bot: "Bot", event: SendMessageEvent):
@@ -193,19 +195,24 @@
         if mention_sender:
             message.insert(
                 0, MessageSegment.mention_user(event.villa_id, event.from_user_id)
             )
         if reply_message:
             message += MessageSegment.quote(event.msg_uid, event.send_at)
         content_info = await self.parse_message_content(message)
+        if isinstance(content_info.content, TextMessageContent):
+            object_name = "MHY:Text"
+        elif isinstance(content_info.content, ImageMessageContent):
+            object_name = "MHY:Image"
+        else:
+            object_name = "MHY:Post"
         return await self.send_message(
             villa_id=event.villa_id,
             room_id=event.room_id,
-            object_name="MHY:Text",
-            # object_name="MHY:Image" if content_info.content.images else "MHY:Text",
+            object_name=object_name,
             msg_content=content_info.json(by_alias=True, exclude_none=True),
         )
 
     async def parse_message_content(self, message: Message) -> MessageContentInfo:
         """将适配器的Message对象转为大别野发送所需要的MessageContentInfo对象
 
         参数:
@@ -231,22 +238,26 @@
                     else None,
                     file_size=seg.data["file_size"],
                 )
                 for seg in images_msg
             ]
         else:
             images = None
+        if posts_msg := (message["post"] or None):
+            post_ids: Optional[List[str]] = [seg.data["post_id"] for seg in posts_msg]
+        else:
+            post_ids = None
         cal_len = lambda x: len(x.encode("utf-16")) // 2 - 1
         message_text = ""
         message_offset = 0
         entities: List[TextEntity] = []
         mentioned = MentionedInfo(type=MentionType.PART)
         for seg in message:
             try:
-                if seg.type in ("quote", "image"):
+                if seg.type in ("quote", "image", "post"):
                     continue
                 if seg.type == "text":
                     seg_text = seg.data["text"]
                     length = cal_len(seg_text)
                 elif seg.type == "mention_all":
                     seg_text = f"@{seg.data['show_text']} "
                     length = cal_len(seg_text)
@@ -303,15 +314,15 @@
                             entity=VillaRoomLink(
                                 villa_id=str(seg.data["villa_id"]),
                                 room_id=str(seg.data["room_id"]),
                                 room_name=room.room_name,
                             ),
                         )
                     )
-                elif seg.type == "link":
+                else:
                     seg_text = seg.data["show_text"]
                     length = cal_len(seg_text)
                     entities.append(
                         TextEntity(
                             offset=message_offset,
                             length=length,
                             entity=Link(
@@ -320,18 +331,30 @@
                         )
                     )
                 message_offset += length
                 message_text += seg_text
             except Exception as e:
                 log("WARNING", "error when parse message content", e)
 
-        # 不能单独只发图片而没有其他文本内容，塞一个零宽度空格
-        if images and not message_text:
-            message_text = "\u200B"
-
         if not (mentioned.type == MentionType.ALL and mentioned.user_id_list):
             mentioned = None
+
+        if not (message_text or entities):
+            if images:
+                if len(images) > 1:
+                    content = TextMessageContent(text="\u200B", images=images)
+                else:
+                    content = ImageMessageContent(**images[-1].dict())
+            elif post_ids:
+                content = PostMessageContent(post_id=post_ids[-1])
+            else:
+                raise ValueError("message content is empty")
+        else:
+            content = TextMessageContent(
+                text=message_text, entities=entities, images=images
+            )
+
         return MessageContentInfo(
-            content=MessageContent(text=message_text, entities=entities, images=images),
+            content=content,
             mentionedInfo=mentioned,
             quote=quote,  # type: ignore
         )
```

### Comparing `nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/event.py` & `nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/exception.py` & `nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_villa-0.1.2/nonebot/adapters/villa/message.py` & `nonebot_adapter_villa-0.2.0/nonebot/adapters/villa/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,14 +138,26 @@
             ImageSegment: 消息段对象
         """
         return ImageSegment(
             "image",
             {"url": url, "width": width, "height": height, "file_size": file_size},
         )
 
+    @staticmethod
+    def post(post_id: str) -> "PostSegment":
+        """帖子转发消息段
+
+        参数:
+            post_id: 帖子ID
+
+        返回:
+            PostSegment: 消息段对象
+        """
+        return PostSegment("post", {"post_id": post_id})
+
 
 class TextSegment(MessageSegment):
     @overrides(MessageSegment)
     def __str__(self) -> str:
         return escape_tag(self.data["text"])
 
 
@@ -187,14 +199,20 @@
 
 class QuoteSegment(MessageSegment):
     @overrides(MessageSegment)
     def __str__(self) -> str:
         return f"<Quote:msg_id={self.data['msg_id']}>"
 
 
+class PostSegment(MessageSegment):
+    @overrides(MessageSegment)
+    def __str__(self) -> str:
+        return f"<Post:post_id={self.data['post_id']}>"
+
+
 class Message(BaseMessage[MessageSegment]):
     @classmethod
     @overrides(BaseMessage)
     def get_segment_class(cls) -> Type[MessageSegment]:
         return MessageSegment
 
     @overrides(BaseMessage)
```

### Comparing `nonebot_adapter_villa-0.1.2/pyproject.toml` & `nonebot_adapter_villa-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-villa"
-version = "0.1.2"
+version = "0.2.0"
 description = "NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2."
 authors = ["CMHopeSunshine <277073121@qq.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 repository = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
 documentation = "https://github.com/CMHopeSunshine/nonebot-adapter-villa"
```

### Comparing `nonebot_adapter_villa-0.1.2/PKG-INFO` & `nonebot_adapter_villa-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-villa
-Version: 0.1.2
+Version: 0.2.0
 Summary: NoneBot2米游社大别野Bot适配器。MiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa
 License: MIT
 Keywords: nonebot,mihoyo,bot
 Author: CMHopeSunshine
 Author-email: 277073121@qq.com
 Requires-Python: >=3.8,<4.0
@@ -25,17 +25,25 @@
 
 <div align="center">
 
 # NoneBot-Adapter-Villa
 
 _✨ 大别野 协议适配 ✨_
 
+<a href="https://cdn.jsdelivr.net/gh/CMHopeSunshine/nonebot-adapter-villa@master/LICENSE">
+  <img src="https://img.shields.io/github/license/CMHopeSunshine/nonebot-adapter-villa" alt="license">
+</a>
 <img src="https://img.shields.io/pypi/v/nonebot-adapter-villa" alt="version">
 <img src="https://img.shields.io/badge/Python-3.8+-yellow" alt="python">
-<a href="https://cdn.jsdelivr.net/gh/CMHopeSunshine/nonebot-adapter-villa@master/LICENSE"><img src="https://img.shields.io/github/license/CMHopeSunshine/nonebot-adapter-villa" alt="license"></a>
+<a href="https://pypi.python.org/pypi/nonebot-adapter-villa">
+  <img src="https://img.shields.io/pypi/dm/nonebot-adapter-villa" alt="pypi download">
+</a>
+<a href="https://wakatime.com/badge/user/eed3f89c-5d65-46e6-ab19-78dcc4b62b3f/project/838e7f55-f8b8-49ff-aec0-29ad264931cf">
+  <img src="https://wakatime.com/badge/user/eed3f89c-5d65-46e6-ab19-78dcc4b62b3f/project/838e7f55-f8b8-49ff-aec0-29ad264931cf.svg" alt="wakatime">
+</a>
 
 </div>
 
 ## 安装
 
 在`NoneBot2`项目目录下使用脚手架安装：
 
@@ -55,15 +63,15 @@
 
 ```dotenv
 DRIVER=~fastapi+~httpx
 ```
 
 ### VILLA_BOTS
 
-配置机器人帐号列表，每个bot有3个必填配置，在大别野官方机器人开发者社区(别野ID: OpenVilla)申请时获得，
+配置机器人帐号列表，每个bot有3个必填配置，在大别野[官方机器人开发者社区](https://dby.miyoushe.com/chat/463/20020)(别野ID: OpenVilla)申请时获得，
 
 - bot_id: 机器人id，以`bot_`开头
 - bot_secret: 机器人密钥
 - callback_url: http回调地址，例如申请bot时给的回调地址是`http://域名/your/callback/url`，那么配置里的`callback_url`填写`/your/callback/url`
   例如：
 
 ```dotenv
@@ -76,14 +84,16 @@
   }
 ]
 '
 ```
 
 ## 示例
 
+> 注意，当前大别野只能接收到有@Bot(在哪个位置皆可)的消息事件，且不能有多个@(即使是@两次Bot都不行)
+
 ### 消息段展示
 
 以下是一个简单的插件示例，展示各种消息段：
 
 ```python
 from nonebot import on_command
 from nonebot.params import CommandArg
@@ -108,19 +118,24 @@
             msg += MessageSegment.room_link(event.villa_id, event.room_id)
         elif arg == "链接":
             msg += MessageSegment.link("https://www.miyoushe.com/ys/article/39670307", show_text="这是链接")
             # 使用link的话链接能够点击进行跳转，使用text的话不能点击
             # show_text是指链接显示的文字，但在当前版本Web端大别野会无法正常跳转，最好不使用该参数
         elif arg == "图片":
             msg += MessageSegment.image("https://www.miyoushe.com/_nuxt/img/miHoYo_Game.2457753.png")
-            # 暂时只支持url图片，但在当前版本web端无法显示图片，待官方后续修复
+            # 暂时只支持url图片
+            # 如果在单次消息中，发送多张图片或者与其他消息段拼接，那么将无法在web端显示出来
+            # 所以建议每张图片单独发送
+        elif arg == "帖子":
+            msg += MessageSegment.post("https://www.miyoushe.com/ys/article/40391314")
+            # 帖子消息段只能单独发送，和其他消息段拼接时将被无视
     await matcher.finish(msg)
 ```
 
-使用命令`@bot /发送 艾特我 艾特bot 文字 房间 链接 图片`时，bot会回复`@你的名字 @bot的名字 文字 #房间名 这是链接 图片内容`
+使用命令`@bot /发送 艾特我 艾特bot 文字 房间 链接`时，bot会回复`@你的名字 @bot的名字 文字 #房间名 这是链接`
 
 
 ## 交流和反馈
 
 目前无论是大别野Bot还是本适配器都在测试开发中，如遇问题请提出issue，感谢支持！
 
 也欢迎来我的大别野【尘世闲游】进行交流：
```

#### html2text {}

```diff
@@ -1,60 +1,66 @@
-Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.1.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-adapter-villa Version: 0.2.0 Summary:
 NoneBot2ç±³æ¸¸ç¤¾å¤§å«éBotééå¨ãMiHoYo Villa Bot adapter for nonebot2.
 Home-page: https://github.com/CMHopeSunshine/nonebot-adapter-villa License: MIT
 Keywords: nonebot,mihoyo,bot Author: CMHopeSunshine Author-email:
 277073121@qq.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: nonebot2
 (>=2.0.0-beta.3,<3.0.0) Project-URL: Documentation, https://github.com/
 CMHopeSunshine/nonebot-adapter-villa Project-URL: Repository, https://
 github.com/CMHopeSunshine/nonebot-adapter-villa Description-Content-Type: text/
 markdown
                             [nonebot-adapter-villa]
- # NoneBot-Adapter-Villa _â¨ å¤§å«é åè®®éé â¨_ [version] [python]
-                                   [license]
+ # NoneBot-Adapter-Villa _â¨ å¤§å«é åè®®éé â¨_ [license] [version]
+                      [python] [pypi_download] [wakatime]
 ## å®è£ å¨`NoneBot2`é¡¹ç®ç®å½ä¸ä½¿ç¨èææ¶å®è£ï¼ ``` nb adapter
 install nonebot-adapter-villa ``` ## éç½® ä¿®æ¹ NoneBot éç½®æä»¶ `.env`
 æè `.env.*`ã ### Driver
 æ¬ééå¨åæ¶éè¦`ReverseDriver`å`ForwardDriver`ï¼åè [driver]
 (https://v2.nonebot.dev/docs/next/advanced/
 driver#%E9%A9%B1%E5%8A%A8%E5%99%A8%E7%B1%BB%E5%9E%8B) éç½®é¡¹ã ä¾å¦ï¼
 ```dotenv DRIVER=~fastapi+~httpx ``` ### VILLA_BOTS
-éç½®æºå¨äººå¸å·åè¡¨ï¼æ¯ä¸ªbotæ3ä¸ªå¿å¡«éç½®ï¼å¨å¤§å«éå®æ¹æºå¨äººå¼åèç¤¾åº
+éç½®æºå¨äººå¸å·åè¡¨ï¼æ¯ä¸ªbotæ3ä¸ªå¿å¡«éç½®ï¼å¨å¤§å«é
+[å®æ¹æºå¨äººå¼åèç¤¾åº](https://dby.miyoushe.com/chat/463/20020)
 (å«éID: OpenVilla)ç³è¯·æ¶è·å¾ï¼ - bot_id: æºå¨äººidï¼ä»¥`bot_`å¼å¤´
 - bot_secret: æºå¨äººå¯é¥ - callback_url:
 httpåè°å°åï¼ä¾å¦ç³è¯·botæ¶ç»çåè°å°åæ¯`http://åå/your/
 callback/url`ï¼é£ä¹éç½®éç`callback_url`å¡«å`/your/callback/url`
 ä¾å¦ï¼ ```dotenv VILLA_BOTS=' [ { "bot_id": "bot_123456789", "bot_secret":
-"abc123def456", "callback_url": "/your/callback/url" } ] ' ``` ## ç¤ºä¾ ###
-æ¶æ¯æ®µå±ç¤º ä»¥ä¸æ¯ä¸ä¸ªç®åçæä»¶ç¤ºä¾ï¼å±ç¤ºåç§æ¶æ¯æ®µï¼
-```python from nonebot import on_command from nonebot.params import CommandArg
-from nonebot.adapters.villa import Bot, SendMessageEvent, Message,
-MessageSegment matcher = on_command('åé') @matcher.handle() async def
-matcher_handler(bot: Bot, event: SendMessageEvent, cmd_arg: Message =
-CommandArg()): msg = Message() args = cmd_arg.extract_plain_text().strip
-().split(' ') for arg in args: if arg == "è¾ç¹æ": msg +=
-MessageSegment.mention_user(event.villa_id, event.from_user_id) elif arg ==
-"è¾ç¹bot": msg += MessageSegment.mention_robot(bot.self_id, bot.nickname)
-elif arg == "æå­": msg += MessageSegment.text("æå­") #
-è¡¨æä¹æ¯ç¨textæ¥åéï¼ä»¥[è¡¨æå]æ ¼å¼ï¼ä¾å¦MessageSegment.text
-("[ç±å¿]") elif arg == "æ¿é´": msg += MessageSegment.room_link
-(event.villa_id, event.room_id) elif arg == "é¾æ¥": msg +=
-MessageSegment.link("https://www.miyoushe.com/ys/article/39670307",
-show_text="è¿æ¯é¾æ¥") #
+"abc123def456", "callback_url": "/your/callback/url" } ] ' ``` ## ç¤ºä¾ >
+æ³¨æï¼å½åå¤§å«éåªè½æ¥æ¶å°æ@Bot
+(å¨åªä¸ªä½ç½®çå¯)çæ¶æ¯äºä»¶ï¼ä¸ä¸è½æå¤ä¸ª@
+(å³ä½¿æ¯@ä¸¤æ¬¡Boté½ä¸è¡) ### æ¶æ¯æ®µå±ç¤º
+ä»¥ä¸æ¯ä¸ä¸ªç®åçæä»¶ç¤ºä¾ï¼å±ç¤ºåç§æ¶æ¯æ®µï¼ ```python from
+nonebot import on_command from nonebot.params import CommandArg from
+nonebot.adapters.villa import Bot, SendMessageEvent, Message, MessageSegment
+matcher = on_command('åé') @matcher.handle() async def matcher_handler(bot:
+Bot, event: SendMessageEvent, cmd_arg: Message = CommandArg()): msg = Message()
+args = cmd_arg.extract_plain_text().strip().split(' ') for arg in args: if arg
+== "è¾ç¹æ": msg += MessageSegment.mention_user(event.villa_id,
+event.from_user_id) elif arg == "è¾ç¹bot": msg +=
+MessageSegment.mention_robot(bot.self_id, bot.nickname) elif arg == "æå­":
+msg += MessageSegment.text("æå­") # è¡¨æä¹æ¯ç¨textæ¥åéï¼ä»¥
+[è¡¨æå]æ ¼å¼ï¼ä¾å¦MessageSegment.text("[ç±å¿]") elif arg == "æ¿é´":
+msg += MessageSegment.room_link(event.villa_id, event.room_id) elif arg ==
+"é¾æ¥": msg += MessageSegment.link("https://www.miyoushe.com/ys/article/
+39670307", show_text="è¿æ¯é¾æ¥") #
 ä½¿ç¨linkçè¯é¾æ¥è½å¤ç¹å»è¿è¡è·³è½¬ï¼ä½¿ç¨textçè¯ä¸è½ç¹å» #
 show_textæ¯æé¾æ¥æ¾ç¤ºçæå­ï¼ä½å¨å½åçæ¬Webç«¯å¤§å«éä¼æ æ³æ­£å¸¸è·³è½¬ï¼æå¥½ä¸ä½¿ç¨è¯¥åæ°
 elif arg == "å¾ç": msg += MessageSegment.image("https://www.miyoushe.com/
-_nuxt/img/miHoYo_Game.2457753.png") #
-ææ¶åªæ¯æurlå¾çï¼ä½å¨å½åçæ¬webç«¯æ æ³æ¾ç¤ºå¾çï¼å¾å®æ¹åç»­ä¿®å¤
+_nuxt/img/miHoYo_Game.2457753.png") # ææ¶åªæ¯æurlå¾ç #
+å¦æå¨åæ¬¡æ¶æ¯ä¸­ï¼åéå¤å¼ å¾çæèä¸å¶ä»æ¶æ¯æ®µæ¼æ¥ï¼é£ä¹å°æ æ³å¨webç«¯æ¾ç¤ºåºæ¥
+# æä»¥å»ºè®®æ¯å¼ å¾çåç¬åé elif arg == "å¸å­": msg +=
+MessageSegment.post("https://www.miyoushe.com/ys/article/40391314") #
+å¸å­æ¶æ¯æ®µåªè½åç¬åéï¼åå¶ä»æ¶æ¯æ®µæ¼æ¥æ¶å°è¢«æ è§
 await matcher.finish(msg) ``` ä½¿ç¨å½ä»¤`@bot /åé è¾ç¹æ è¾ç¹bot
-æå­ æ¿é´ é¾æ¥ å¾ç`æ¶ï¼botä¼åå¤`@ä½ çåå­ @botçåå­
-æå­ #æ¿é´å è¿æ¯é¾æ¥ å¾çåå®¹` ## äº¤æµååé¦
+æå­ æ¿é´ é¾æ¥`æ¶ï¼botä¼åå¤`@ä½ çåå­ @botçåå­ æå­
+#æ¿é´å è¿æ¯é¾æ¥` ## äº¤æµååé¦
 ç®åæ è®ºæ¯å¤§å«éBotè¿æ¯æ¬ééå¨é½å¨æµè¯å¼åä¸­ï¼å¦éé®é¢è¯·æåºissueï¼æè°¢æ¯æï¼
 ä¹æ¬¢è¿æ¥æçå¤§å«éãå°ä¸é²æ¸¸ãè¿è¡äº¤æµï¼ - å¤§å«éID:
 wgiJNaUï¼å¯æç´¢å å¥ - [Webç«¯é¾æ¥](https://dby.miyoushe.com/chat/1047/
 21652)ï¼ç®åä»PCç«¯å¯è®¿é® ## ç¸å³é¡¹ç® - [NoneBot2](https://
 github.com/nonebot/nonebot2): éå¸¸å¥½ç¨çPythonè·¨å¹³å°æºå¨äººæ¡æ¶ï¼
 - [villa-py](https://github.com/CMHopeSunshine/villa-py): å¤§å«é Bot Python
 SDKã
```

