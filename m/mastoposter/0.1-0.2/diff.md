# Comparing `tmp/mastoposter-0.1.tar.gz` & `tmp/mastoposter-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mastoposter-0.1.tar", last modified: Tue May  9 15:46:50 2023, max compression
+gzip compressed data, was "mastoposter-0.2.tar", last modified: Fri Jun 16 21:55:17 2023, max compression
```

## Comparing `mastoposter-0.1.tar` & `mastoposter-0.2.tar`

### file list

```diff
@@ -1,28 +1,37 @@
--rw-r--r--   0        0        0       42 2022-10-11 06:28:03.114718 mastoposter-0.1/.dockerignore
--rw-r--r--   0        0        0       70 2023-05-08 15:04:53.166981 mastoposter-0.1/.gitignore
--rw-r--r--   0        0        0      219 2022-10-11 06:28:03.114718 mastoposter-0.1/Dockerfile
--rw-r--r--   0        0        0    35149 2023-05-08 15:04:53.166981 mastoposter-0.1/LICENSE
--rw-r--r--   0        0        0    10101 2023-05-08 15:04:53.166981 mastoposter-0.1/README.md
--rw-r--r--   0        0        0     5096 2023-03-05 06:02:37.750142 mastoposter-0.1/config.ini
--rw-r--r--   0        0        0     3074 2023-05-09 15:46:11.877142 mastoposter-0.1/mastoposter/__init__.py
--rw-r--r--   0        0        0     4468 2023-05-08 15:04:53.166981 mastoposter-0.1/mastoposter/__main__.py
--rw-r--r--   0        0        0     1798 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/filters/__init__.py
--rw-r--r--   0        0        0     2676 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/filters/base.py
--rw-r--r--   0        0        0     1661 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/filters/boost.py
--rw-r--r--   0        0        0     2431 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/filters/combined.py
--rw-r--r--   0        0        0     2090 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/filters/media.py
--rw-r--r--   0        0        0     1946 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/filters/mention.py
--rw-r--r--   0        0        0     1411 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/filters/spoiler.py
--rw-r--r--   0        0        0     2493 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/filters/text.py
--rw-r--r--   0        0        0     1266 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/filters/visibility.py
--rw-r--r--   0        0        0      967 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/integrations/__init__.py
--rw-r--r--   0        0        0     1113 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/integrations/base.py
--rw-r--r--   0        0        0     4021 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/integrations/discord/__init__.py
--rw-r--r--   0        0        0     2535 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/integrations/discord/types.py
--rw-r--r--   0        0        0     9834 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/integrations/telegram.py
--rw-r--r--   0        0        0     2236 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/sources.py
--rw-r--r--   0        0        0    10407 2023-05-08 15:04:53.170314 mastoposter-0.1/mastoposter/types.py
--rw-r--r--   0        0        0     8486 2023-05-09 15:42:36.239241 mastoposter-0.1/mastoposter/utils.py
--rw-r--r--   0        0        0      882 2023-05-08 15:04:53.170314 mastoposter-0.1/pyproject.toml
--rw-r--r--   0        0        0      246 2022-11-05 08:05:19.598221 mastoposter-0.1/requirements.txt
--rw-r--r--   0        0        0    10842 1970-01-01 00:00:00.000000 mastoposter-0.1/PKG-INFO
+-rw-r--r--   0        0        0       42 2023-06-16 20:17:57.513860 mastoposter-0.2/.dockerignore
+-rw-r--r--   0        0        0      371 2023-06-16 20:17:57.513860 mastoposter-0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0       70 2023-06-16 20:17:57.513860 mastoposter-0.2/.gitignore
+-rw-r--r--   0        0        0      219 2023-06-16 20:17:57.513860 mastoposter-0.2/Dockerfile
+-rw-r--r--   0        0        0    35149 2023-06-16 20:17:57.513860 mastoposter-0.2/LICENSE
+-rw-r--r--   0        0        0    10101 2023-06-16 20:17:57.513860 mastoposter-0.2/README.md
+-rw-r--r--   0        0        0     5096 2023-06-16 20:17:57.517193 mastoposter-0.2/config.ini
+-rw-r--r--   0        0        0      924 2023-06-16 20:17:57.517193 mastoposter-0.2/contrib/mastoposter.initd
+-rw-r--r--   0        0        0      962 2023-06-16 20:17:57.517193 mastoposter-0.2/contrib/mastoposter.service
+-rw-r--r--   0        0        0     3115 2023-06-16 21:54:33.383397 mastoposter-0.2/mastoposter/__init__.py
+-rw-r--r--   0        0        0     4918 2023-06-16 20:17:57.517193 mastoposter-0.2/mastoposter/__main__.py
+-rw-r--r--   0        0        0     1798 2023-06-16 20:17:57.517193 mastoposter-0.2/mastoposter/filters/__init__.py
+-rw-r--r--   0        0        0     2676 2023-06-16 20:17:57.517193 mastoposter-0.2/mastoposter/filters/base.py
+-rw-r--r--   0        0        0     1661 2023-06-16 20:17:57.517193 mastoposter-0.2/mastoposter/filters/boost.py
+-rw-r--r--   0        0        0     2431 2023-06-16 20:17:57.517193 mastoposter-0.2/mastoposter/filters/combined.py
+-rw-r--r--   0        0        0     2090 2023-06-16 20:17:57.517193 mastoposter-0.2/mastoposter/filters/media.py
+-rw-r--r--   0        0        0     1946 2023-06-16 20:17:57.517193 mastoposter-0.2/mastoposter/filters/mention.py
+-rw-r--r--   0        0        0     1411 2023-06-16 20:17:57.517193 mastoposter-0.2/mastoposter/filters/spoiler.py
+-rw-r--r--   0        0        0     2493 2023-06-16 20:17:57.520526 mastoposter-0.2/mastoposter/filters/text.py
+-rw-r--r--   0        0        0     1266 2023-06-16 20:17:57.520526 mastoposter-0.2/mastoposter/filters/visibility.py
+-rw-r--r--   0        0        0      967 2023-06-16 20:17:57.520526 mastoposter-0.2/mastoposter/integrations/__init__.py
+-rw-r--r--   0        0        0     1113 2023-06-16 20:17:57.520526 mastoposter-0.2/mastoposter/integrations/base.py
+-rw-r--r--   0        0        0     3995 2023-06-16 20:17:57.520526 mastoposter-0.2/mastoposter/integrations/discord/__init__.py
+-rw-r--r--   0        0        0     2535 2023-06-16 20:17:57.520526 mastoposter-0.2/mastoposter/integrations/discord/types.py
+-rw-r--r--   0        0        0     9859 2023-06-16 20:17:57.520526 mastoposter-0.2/mastoposter/integrations/telegram.py
+-rw-r--r--   0        0        0     2236 2023-06-16 20:17:57.520526 mastoposter-0.2/mastoposter/sources.py
+-rw-r--r--   0        0        0     3024 2023-06-16 20:17:57.520526 mastoposter-0.2/mastoposter/text/__init__.py
+-rw-r--r--   0        0        0     1243 2023-06-16 20:17:57.520526 mastoposter-0.2/mastoposter/text/__main__.py
+-rw-r--r--   0        0        0     2970 2023-06-16 20:17:57.520526 mastoposter-0.2/mastoposter/text/html.py
+-rw-r--r--   0        0        0     2128 2023-06-16 20:17:57.520526 mastoposter-0.2/mastoposter/text/markdown.py
+-rw-r--r--   0        0        0     1963 2023-06-16 20:17:57.523860 mastoposter-0.2/mastoposter/text/plain.py
+-rw-r--r--   0        0        0    10389 2023-06-16 20:17:57.523860 mastoposter-0.2/mastoposter/types.py
+-rw-r--r--   0        0        0     1299 2023-06-16 20:17:57.523860 mastoposter-0.2/mastoposter/utils.py
+-rw-r--r--   0        0        0     1178 2023-06-16 20:17:57.523860 mastoposter-0.2/pyproject.toml
+-rw-r--r--   0        0        0      246 2023-06-16 20:17:57.523860 mastoposter-0.2/requirements.txt
+-rw-r--r--   0        0        0     6617 2023-06-16 20:17:57.523860 mastoposter-0.2/tests/test_text_utils.py
+-rw-r--r--   0        0        0    10895 1970-01-01 00:00:00.000000 mastoposter-0.2/PKG-INFO
```

### Comparing `mastoposter-0.1/LICENSE` & `mastoposter-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mastoposter-0.1/README.md` & `mastoposter-0.2/README.md`

 * *Files identical despite different names*

### Comparing `mastoposter-0.1/config.ini` & `mastoposter-0.2/config.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-[DEFAULT]
-# Number of retries in case request fails. Applies globally
-# Can be changed on per-module basis
-http-retries = 5
-
 [main]
 # This is a list of output modules. Each module should be defined in section,
 # named "module/MODULENAME". Space-separated list of strings.
 modules = telegram
 
 # Mastodon instance to grab posts from
 instance = mastodon.example.org
 
 # Mastodon user token.
-# Required permissions: read:statuses read:lists
+# Required permissions: read:accounts read:statuses read:lists
 # You can get your token by creating application in
 # ${instance}/settings/applications
 token = blahblah
 
 # Your user ID.
 # Doesn't necessarily yours, it can be any user's ID, but that user should be
 # on the list for crossposter to find it.
@@ -34,14 +29,18 @@
 
 # Should we automatically reconnect to the streaming socket?
 # That option exists because it's not really a big deal when crossposter runs
 # as a service and restarts automatically by the service manager.
 auto-reconnect = yes
 reconnect-delay = 1.0
 
+# Number of retries in case request fails. Applies globally
+# Can be changed on per-module basis
+http-retries = 5
+
 # Example Telegram integration. You can use it as a template
 [module/telegram]
 type = telegram
 
 # Telegram Bot API token. There's plenty of guides how to obtain one.
 # https://core.telegram.org/bots#3-how-do-i-create-a-bot
 token = 12345:blahblah
@@ -105,15 +104,15 @@
 ;mode = include
 
 ;# Text content filter
 ;[filter/content]
 ;type = content
 ;# Mode of the filter.
 ;# "regexp" requires "regexp" property and should contain... A RegExp
-;# "hashtag" should contain space-separated list of tags
+;# "tag" should contain space-separated list of tags
 ;mode = regexp
 ;# Regular expression pattern to be matched
 ;regexp = ^x-no-repost
 ;# List of tags
 ; tags = maids artspam
 
 ;# Spoiler text filter
```

#### html2text {}

```diff
@@ -1,35 +1,36 @@
-[DEFAULT] # Number of retries in case request fails. Applies globally # Can be
-changed on per-module basis http-retries = 5 [main] # This is a list of output
-modules. Each module should be defined in section, # named "module/MODULENAME".
-Space-separated list of strings. modules = telegram # Mastodon instance to grab
-posts from instance = mastodon.example.org # Mastodon user token. # Required
-permissions: read:statuses read:lists # You can get your token by creating
+[main] # This is a list of output modules. Each module should be defined in
+section, # named "module/MODULENAME". Space-separated list of strings. modules
+= telegram # Mastodon instance to grab posts from instance =
+mastodon.example.org # Mastodon user token. # Required permissions: read:
+accounts read:statuses read:lists # You can get your token by creating
 application in # ${instance}/settings/applications token = blahblah # Your user
 ID. # Doesn't necessarily yours, it can be any user's ID, but that user should
 be # on the list for crossposter to find it. # Setting it to "auto" will just
 grab yours instead. Don't worry about it # EXCEPT if you're using Pleroma.
 Check #11 issue for more details: # https://github.com/hatkidchan/mastoposter/
 issues/11 user = auto # Mastodon user list ID. AGAIN, UNFORTUNATELY, there is
 no way to reliably use # streaming API to get all of your posts. Using home
 timeline is unreliable and # does not always include boosts, same with public:
 local # So, create a list, add yourself here, and put its ID here (it should be
 in # address bar while you have that list open) list = 1 # Should we
 automatically reconnect to the streaming socket? # That option exists because
 it's not really a big deal when crossposter runs # as a service and restarts
 automatically by the service manager. auto-reconnect = yes reconnect-delay =
-1.0 # Example Telegram integration. You can use it as a template [module/
-telegram] type = telegram # Telegram Bot API token. There's plenty of guides
-how to obtain one. # https://core.telegram.org/bots#3-how-do-i-create-a-bot
-token = 12345:blahblah # Telegram channel/chat ID or name. Also can be just a
-regular user. # You can use @showjsonbot to obtain your channel ID, or just use
-its # username, if it is public chat = @username # Should we make posts silent?
-# https://core.telegram.org/bots/api#sendmessage `disable_notification` silent
-= true # Jinja2 template string for the post. Works only in Telegram. # This is
-the default template, not specifying that property at all will result # in this
+1.0 # Number of retries in case request fails. Applies globally # Can be
+changed on per-module basis http-retries = 5 # Example Telegram integration.
+You can use it as a template [module/telegram] type = telegram # Telegram Bot
+API token. There's plenty of guides how to obtain one. # https://
+core.telegram.org/bots#3-how-do-i-create-a-bot token = 12345:blahblah #
+Telegram channel/chat ID or name. Also can be just a regular user. # You can
+use @showjsonbot to obtain your channel ID, or just use its # username, if it
+is public chat = @username # Should we make posts silent? # https://
+core.telegram.org/bots/api#sendmessage `disable_notification` silent = true #
+Jinja2 template string for the post. Works only in Telegram. # This is the
+default template, not specifying that property at all will result # in this
 string (probably) # Pay attention to 4 spaces in the empty line, I think it's
 required template = {% if status.reblog %}Boost from {
 {status.reblog.account.name}} {% endif %}{% if
 status.reblog_or_status.spoiler_text %}{{status.reblog_or_status.spoiler_text}}
 {% endif %}{{ status.reblog_or_status.content_flathtml }}{% if
 status.reblog_or_status.spoiler_text %}{% endif %} Link_to_post # Discord
 integration [module/discord] type = discord # Webhook URL with the `?wait=true`
@@ -47,15 +48,15 @@
 @name@* @*@* ;# Media filter. Only posts with some specific media content are
 triggered ;[filter/media] ;type = media ;# space-separated list of media types
 to be checked ;valid-media = image video gifv audio unknown ;# mode of the
 filter itself ;# "include" means "there should be at least one media of any
 type listed" ;# "exclude" means "there shouldn't be anything from that list" ;#
 "only" allows only media from the list to be sent ;mode = include ;# Text
 content filter ;[filter/content] ;type = content ;# Mode of the filter. ;#
-"regexp" requires "regexp" property and should contain... A RegExp ;# "hashtag"
+"regexp" requires "regexp" property and should contain... A RegExp ;# "tag"
 should contain space-separated list of tags ;mode = regexp ;# Regular
 expression pattern to be matched ;regexp = ^x-no-repost ;# List of tags ; tags
 = maids artspam ;# Spoiler text filter ;# Will be matched if spoiler matches
 some regexp ;# (use ^.+$ to check for any spoiler) ;[filter/spoiler] ;type =
 spoiler ;regexp = ^CW: ;# Visibility filter. ;# Only posts with specific
 visibility will be matched ;[filter/visibility] ;type = visibility ;# Space-
 separated list of visibilities ;# NOTE: `direct` visibility is always ignored
```

### Comparing `mastoposter-0.1/mastoposter/__init__.py` & `mastoposter-0.2/mastoposter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,18 @@
 from mastoposter.integrations import (
     DiscordIntegration,
     FilteredIntegration,
     TelegramIntegration,
 )
 from mastoposter.types import Status
 
-__version__ = "0.1"
-__description__ = "Mastodon to [anything] reposter"
+__version__ = "0.2"
+__description__ = (
+    "Configurable reposter from Mastodon-compatible Fediverse servers"
+)
 
 logger = getLogger()
 
 
 def load_integrations_from(config: ConfigParser) -> List[FilteredIntegration]:
     modules: List[FilteredIntegration] = []
     for module_name in config.get("main", "modules").split():
```

### Comparing `mastoposter-0.1/mastoposter/__main__.py` & `mastoposter-0.2/mastoposter/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,32 +9,40 @@
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 """
+from argparse import ArgumentParser
 from asyncio import run
 from configparser import ConfigParser, ExtendedInterpolation
 from logging import (
     INFO,
     Formatter,
     Logger,
     StreamHandler,
     getLevelName,
     getLogger,
 )
-from sys import argv, stdout
-from mastoposter import execute_integrations, load_integrations_from
-from mastoposter.integrations import FilteredIntegration
-from mastoposter.sources import websocket_source
+from os import getenv
+from sys import stdout
 from typing import AsyncGenerator, Callable, List
-from mastoposter.types import Account, Status
+
 from httpx import Client, HTTPTransport
 
+from mastoposter import (
+    execute_integrations,
+    load_integrations_from,
+    __version__,
+    __description__,
+)
+from mastoposter.integrations import FilteredIntegration
+from mastoposter.sources import websocket_source
+from mastoposter.types import Account, Status
 from mastoposter.utils import normalize_config
 
 
 WSOCK_TEMPLATE = "wss://{instance}/api/v1/streaming"
 VERIFY_CREDS_TEMPLATE = "https://{instance}/api/v1/accounts/verify_credentials"
 
 logger = getLogger()
@@ -88,21 +96,30 @@
         ):
             logger.info(
                 "Skipping post %s because it's a reply to another person",
                 status.uri,
             )
             continue
 
-        await execute_integrations(status, drains)
+        logger.info(await execute_integrations(status, drains))
 
 
-def main(config_path: str = argv[1]):
-    conf = ConfigParser(interpolation=ExtendedInterpolation())
-    conf.read(config_path)
+def main():
+    parser = ArgumentParser(prog="mastoposter", description=__description__)
+    parser.add_argument(
+        "config", nargs="?", default=getenv("MASTOPOSTER_CONFIG_FILE")
+    )
+    parser.add_argument("-v", action="version", version=__version__)
+    args = parser.parse_args()
 
+    if not args.config:
+        raise RuntimeError("No config file. Aborting")
+
+    conf = ConfigParser(interpolation=ExtendedInterpolation())
+    conf.read(args.config)
     init_logger(getLevelName(conf["main"].get("loglevel", "INFO")))
     normalize_config(conf)
 
     modules: List[FilteredIntegration] = load_integrations_from(conf)
     retries: int = conf["main"].getint("http-retries", 5)
 
     logger.info("Loaded %d integrations", len(modules))
```

### Comparing `mastoposter-0.1/mastoposter/filters/__init__.py` & `mastoposter-0.2/mastoposter/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0.1/mastoposter/filters/base.py` & `mastoposter-0.2/mastoposter/filters/base.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0.1/mastoposter/filters/boost.py` & `mastoposter-0.2/mastoposter/filters/boost.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0.1/mastoposter/filters/combined.py` & `mastoposter-0.2/mastoposter/filters/combined.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0.1/mastoposter/filters/media.py` & `mastoposter-0.2/mastoposter/filters/media.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0.1/mastoposter/filters/mention.py` & `mastoposter-0.2/mastoposter/filters/mention.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0.1/mastoposter/filters/spoiler.py` & `mastoposter-0.2/mastoposter/filters/spoiler.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0.1/mastoposter/filters/text.py` & `mastoposter-0.2/mastoposter/filters/text.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0.1/mastoposter/filters/visibility.py` & `mastoposter-0.2/mastoposter/filters/visibility.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0.1/mastoposter/integrations/__init__.py` & `mastoposter-0.2/mastoposter/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0.1/mastoposter/integrations/base.py` & `mastoposter-0.2/mastoposter/integrations/base.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0.1/mastoposter/integrations/discord/__init__.py` & `mastoposter-0.2/mastoposter/integrations/discord/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
     async def execute_webhook(
         self,
         content: Optional[str] = None,
         username: Optional[str] = None,
         avatar_url: Optional[str] = None,
         embeds: Optional[List[DiscordEmbed]] = None,
-    ) -> dict:
+    ) -> None:
         async with AsyncClient(
             transport=AsyncHTTPTransport(retries=self.retries)
         ) as c:
             json = {
                 "content": content,
                 "username": username,
                 "avatar_url": avatar_url,
@@ -61,15 +61,14 @@
             result = (
                 await c.post(
                     self.webhook,
                     json=json,
                 )
             ).json()
             logger.debug("Result: %r", result)
-            return result
 
     async def __call__(self, status: Status) -> Optional[str]:
         source = status.reblog or status
         embeds: List[DiscordEmbed] = []
 
         text = source.content_markdown
         if source.spoiler_text:
```

### Comparing `mastoposter-0.1/mastoposter/integrations/discord/types.py` & `mastoposter-0.2/mastoposter/integrations/discord/types.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0.1/mastoposter/integrations/telegram.py` & `mastoposter-0.2/mastoposter/integrations/telegram.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,15 +184,15 @@
                 logger.warning(
                     "attachment %r is not in %r",
                     attachment.type,
                     MEDIA_COMPATIBILITY,
                 )
                 continue
 
-            if attachment.type not in allowed_medias:
+            if attachment.type not in allowed_medias or len(media_list) >= 10:
                 unused.append(attachment)
                 continue
 
             allowed_medias &= MEDIA_COMPATIBILITY[attachment.type]
 
             media_list.append(
                 {
```

### Comparing `mastoposter-0.1/mastoposter/sources.py` & `mastoposter-0.2/mastoposter/sources.py`

 * *Files identical despite different names*

### Comparing `mastoposter-0.1/mastoposter/types.py` & `mastoposter-0.2/mastoposter/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 """
 from dataclasses import dataclass, field, fields
 from datetime import datetime
 from typing import Any, Callable, Optional, List, Literal, TypeVar
 
 from bs4 import BeautifulSoup
 
-from mastoposter.utils import node_to_html, node_to_markdown, node_to_plaintext
+from mastoposter.text import node_process
 
 
 def _date(val: str) -> datetime:
     return datetime.fromisoformat(val.rstrip("Z"))
 
 
 T = TypeVar("T")
@@ -351,22 +351,22 @@
 
     @property
     def link(self) -> str:
         return self.account.url + "/" + str(self.id)
 
     @property
     def content_flathtml(self) -> str:
-        return node_to_html(
-            BeautifulSoup(self.content, features="lxml")
+        return node_process(
+            BeautifulSoup(self.content, features="lxml"), "html"
         ).rstrip()
 
     @property
     def content_markdown(self) -> str:
-        return node_to_markdown(
-            BeautifulSoup(self.content, features="lxml")
+        return node_process(
+            BeautifulSoup(self.content, features="lxml"), "markdown"
         ).rstrip()
 
     @property
     def content_plaintext(self) -> str:
-        return node_to_plaintext(
-            BeautifulSoup(self.content, features="lxml")
+        return node_process(
+            BeautifulSoup(self.content, features="lxml"), "plain"
         ).rstrip()
```

### Comparing `mastoposter-0.1/pyproject.toml` & `mastoposter-0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,52 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "mastoposter"
+description = "Configurable reposter from Mastodon-compatible Fediverse servers"
 authors = [
     {name = "hatkidchan", email = "hatkidchan@gmail.com"}
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "Environment :: No Input/Output (Daemon)",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Topic :: Communications",
     "Topic :: Internet :: WWW/HTTP"
 ]
 keywords = ["mastodon", "discord", "telegram"]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
     "Jinja2",
-    "beautifulsoup4",
+    "beautifulsoup4[lxml]",
     "emoji",
     "httpx",
     "websockets"
 ]
-dynamic = ["version", "description"]
+dynamic = ["version"]
+
+[project.optional-dependencies]
+test = [
+    "pytest"
+]
 
 [project.urls]
 Source = "https://github.com/hatkidchan/mastoposter"
 
 [project.scripts]
 mastoposter = "mastoposter.__main__:main"
 
 [tool.flit.sdist]
-include = ["config.ini"]
+include = ["config.ini", "contrib/*"]
+
+[tool.black]
+line-length = 79
+target-version = ['py37', 'py38']
+
+[tool.mypy]
+warn_return_any = true
+warn_unused_configs = true
+check_untyped_defs = true
```

### Comparing `mastoposter-0.1/PKG-INFO` & `mastoposter-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: mastoposter
-Version: 0.1
-Summary: mastoposter - configurable reposter from Mastodon-compatible Fediverse servers
+Version: 0.2
+Summary: Configurable reposter from Mastodon-compatible Fediverse servers
 Keywords: mastodon,discord,telegram
 Author-email: hatkidchan <hatkidchan@gmail.com>
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Topic :: Communications
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: Jinja2
-Requires-Dist: beautifulsoup4
+Requires-Dist: beautifulsoup4[lxml]
 Requires-Dist: emoji
 Requires-Dist: httpx
 Requires-Dist: websockets
+Requires-Dist: pytest ; extra == "test"
 Project-URL: Source, https://github.com/hatkidchan/mastoposter
+Provides-Extra: test
 
 # mastoposter - easy-to-use mastodon-to-[everything] reposter
 
 Mastoposter is a simple zero-headache* service that forwards your toots from any
 Mastodon-compatible Fediverse software (Pleroma also works\*\*!) to any of your
 other services! For now it supports only Discord webhooks and Telegram, but it
 can be easily extended to support pretty much anything!
```

