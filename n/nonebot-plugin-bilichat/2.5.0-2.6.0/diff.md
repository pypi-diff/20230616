# Comparing `tmp/nonebot_plugin_bilichat-2.5.0.tar.gz` & `tmp/nonebot_plugin_bilichat-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-2.5.0.tar", last modified: Fri Jun  9 16:36:34 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-2.6.0.tar", last modified: Fri Jun 16 16:28:16 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-2.5.0.tar` & `nonebot_plugin_bilichat-2.6.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    34523 2023-06-09 16:36:23.265984 nonebot_plugin_bilichat-2.5.0/LICENSE
--rw-r--r--   0        0        0    12555 2023-06-09 16:36:23.265984 nonebot_plugin_bilichat-2.5.0/README.md
--rw-r--r--   0        0        0     9322 2023-06-09 16:36:23.273984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4914 2023-06-09 16:36:23.273984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-06-09 16:36:23.273984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      871 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     6463 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0    11820 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3812 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      555 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0      387 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/model/content.py
--rw-r--r--   0        0        0      503 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0    27359 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/model/newbing.py
--rw-r--r--   0        0        0      323 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-06-09 16:36:23.277984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-06-09 16:36:23.281984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1363 2023-06-09 16:36:23.281984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     5904 2023-06-09 16:36:23.281984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4916 2023-06-09 16:36:23.281984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2363 2023-06-09 16:36:23.281984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-06-09 16:36:23.281984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1780 2023-06-09 16:36:23.281984 nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1499 2023-06-09 16:36:34.534059 nonebot_plugin_bilichat-2.5.0/pyproject.toml
--rw-r--r--   0        0        0    13996 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-16 16:28:08.131567 nonebot_plugin_bilichat-2.6.0/LICENSE
+-rw-r--r--   0        0        0    12661 2023-06-16 16:28:08.131567 nonebot_plugin_bilichat-2.6.0/README.md
+-rw-r--r--   0        0        0     9278 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4914 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      871 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6463 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0    11820 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3812 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      555 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-06-16 16:28:08.139567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0      503 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0    27359 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/model/newbing.py
+-rw-r--r--   0        0        0      323 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1363 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     6899 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4916 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2363 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1780 2023-06-16 16:28:08.143567 nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1499 2023-06-16 16:28:16.331509 nonebot_plugin_bilichat-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0    14102 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-2.6.0/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-2.5.0/LICENSE` & `nonebot_plugin_bilichat-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.5.0/README.md` & `nonebot_plugin_bilichat-2.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -197,15 +197,15 @@
 注:
 
 1. openai 与 newbing 目前均需求科学上网才能使用，国内服务器请务必填写 `bilichat_openai_proxy` 或全局透明代理
 2. 如果同时填写了 `bilichat_openai_token` 和 `bilichat_newbing_cookie`，则会使用 `newbing` 进行总结, 并在 `newbing` 总结失败时使用 `openai` 进行总结
 3. `newbing` 和 `openai` 均有缓存机制，同一视频在**获取到正常的总结内容后**不会重复发送请求，如需刷新请求内容可以 [添加参数](#参数表) 或手动删除对应视频的缓存文件或整个缓存文件夹
 4. 经测试，目前 `newbing` 至少能总结 12000 字符以上的文本，推测 token 上限应为 `gpt-4-32k-0314` 的 `32200` token，但过长的内容易造成输出内容包含额外内容或总结失败，因此也建议设置一个合理的 token 上限 ~~（反正不要钱，要啥自行车）~~
 5. 由于 `newbing` 限制较大，也不如 `openai` 听话，且需要联网查询资料，因此使用体验并不如 chatgpt ~~（反正不要钱，要啥自行车）~~
-6. newbing cookie 文件获取方式参考[这里](https://github.com/acheong08/EdgeGPT#getting-authentication-required)和[这里](https://github.com/Harry-Jing/nonebot-plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)。目前 newbing 已正式公布且无需登录也可使用，填写 `bilichat_newbing_cookie=no_login` 即可无 cookie 使用
+6. newbing cookie 文件获取方式参考[这里](https://github.com/acheong08/EdgeGPT#getting-authentication-required)和[这里](https://github.com/Harry-Jing/nonebot-plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)。~~目前 newbing 已正式公布且无需登录也可使用，填写 `bilichat_newbing_cookie=no_login` 即可无 cookie 使用。~~ 目前无 cookie 使用**失败概率极高**，请谨慎考虑是否采用无 cookie 的方式。
 
 ## 🎉 使用
 
 直接发送视频(专栏)链接即可
 
 ### 参数表
```

#### html2text {}

```diff
@@ -97,19 +97,20 @@
 tokenï¼ä½è¿é¿çåå®¹æé æè¾åºåå®¹åå«é¢å¤åå®¹ææ»ç»å¤±è´¥ï¼å æ­¤ä¹å»ºè®®è®¾ç½®ä¸ä¸ªåçç
 token ä¸é ~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ 5. ç±äº `newbing`
 éå¶è¾å¤§ï¼ä¹ä¸å¦ `openai`
 å¬è¯ï¼ä¸éè¦èç½æ¥è¯¢èµæï¼å æ­¤ä½¿ç¨ä½éªå¹¶ä¸å¦ chatgpt
 ~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ 6. newbing cookie
 æä»¶è·åæ¹å¼åè[è¿é](https://github.com/acheong08/EdgeGPT#getting-
 authentication-required)å[è¿é](https://github.com/Harry-Jing/nonebot-
-plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)ãç®å newbing
+plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)ã~~ç®å newbing
 å·²æ­£å¼å¬å¸ä¸æ éç»å½ä¹å¯ä½¿ç¨ï¼å¡«å
-`bilichat_newbing_cookie=no_login` å³å¯æ  cookie ä½¿ç¨ ## ð ä½¿ç¨
-ç´æ¥åéè§é¢(ä¸æ )é¾æ¥å³å¯ ### åæ°è¡¨
-å¨åéè§é¢æ¶ï¼å¯ä»¥é¢å¤æ·»å ä»¥ä¸ç±»ä¼¼ shell
+`bilichat_newbing_cookie=no_login` å³å¯æ  cookie ä½¿ç¨ã~~ ç®åæ 
+cookie ä½¿ç¨**å¤±è´¥æ¦çæé«**ï¼è¯·è°¨æèèæ¯å¦éç¨æ  cookie
+çæ¹å¼ã ## ð ä½¿ç¨ ç´æ¥åéè§é¢(ä¸æ )é¾æ¥å³å¯ ###
+åæ°è¡¨ å¨åéè§é¢æ¶ï¼å¯ä»¥é¢å¤æ·»å ä»¥ä¸ç±»ä¼¼ shell
 æä»¤çåæ°ï¼è¿èå¯¹è§£ææµç¨è¿è¡è°æ´ãä¾å¦ ```shell
 BV12v4y1E7NT --refresh BV12v4y1E7NT -r # å¯ä»¥ä½¿ç¨ç®å BV12v4y1E7NT -r --
 no-cache # å¯ä»¥å¤ä¸ªåæ°æ··ç¨ -r BV12v4y1E7NT -n #
 è½ç¶ä¸å»ºè®®ï¼ä½ç¡®å®å¯ä»¥æåæ°æ¾åé¢ ``` | æä»¤ | ç®å |
 è¯´æ | |:-----:|:----:|:----:| | --no-cache | -n | æ¬æ¬¡æ»ç»ç¦ç¨ç¼å­
 (ä¸ä¼å½±åå·²å­å¨çç¼å­æä»¶) | | --refresh | -r |
 å·æ°æ­¤è§é¢çè¯äºåæ»ç»ç¼å­(ä¼è¦çå·²å­å¨çç¼å­æä»¶) |
```

### Comparing `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,14 @@
 
 async def _permission_check(bot: BOT, event: MESSAGE_EVENT, state: T_State):
     # 检查权限
     # check if self msg
     if str(event.get_user_id()) == str(bot.self_id):
         if plugin_config.bilichat_only_self:
             state["_uid_"] = event.get_session_id()
-            print("_permission_check true")
             return True
         elif not plugin_config.bilichat_enable_self:
             return False
     elif plugin_config.bilichat_only_self:
         return False
     # private msg use user id
     if isinstance(event, (V11_PME, V12_PME, Mirai_PME)):
```

### Comparing `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/store.py` & `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/model/newbing.py` & `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/model/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,53 @@
+import asyncio
+import concurrent.futures
 import json
 import random
 import re
 from collections import OrderedDict
 from pathlib import Path
 from typing import List, Literal
 
 from EdgeGPT import Chatbot, ConversationStyle
 from nonebot.log import logger
 
 from ..config import plugin_config
 from ..lib.store import BING_APOLOGY
 from ..model.cache import Cache
-from ..model.exception import (
-    AbortError,
-    BingChatResponseException,
-)
+from ..model.exception import AbortError, BingChatResponseException
 from ..model.newbing import BingChatResponse
 from ..optional import capture_exception  # type: ignore
 from .text_to_image import rich_text2image
 
 cookies = (
     {}
     if plugin_config.bilichat_newbing_cookie == "no_login"
     else json.loads(Path(plugin_config.bilichat_newbing_cookie).read_text("utf-8"))  # type: ignore
 )
-logger.info("Try init bing chatbot")
-init = False
-for count in range(5):
-    try:
-        bot = Chatbot(cookies=cookies, proxy=plugin_config.bilichat_openai_proxy)  # type: ignore
-        logger.success("Bing chatbot init success")
-        init = True
-        break
-    except Exception as e:
-        logger.error(f"Bing chatbot init failed, retrying {count+1}/5: {e}")
 
-if not init:
+bot = None
+
+
+def init_chatbot(total_count: int = 5):
+    global bot
+    for count in range(total_count):
+        try:
+            bot = Chatbot(cookies=cookies, proxy=plugin_config.bilichat_openai_proxy)  # type: ignore
+            logger.success("Bing chatbot init success")
+            return
+        except Exception as e:
+            logger.error(f"Bing chatbot init failed, retrying {count+1}/5: {e}")
     raise RuntimeError("Bing chatbot init failed")
 
 
+logger.info("Try init bing chatbot")
+init_chatbot()
+assert bot, "Bing chatbot init failed"
+
+
 def get_small_size_transcripts(title: str, text_data: List[str], type_: Literal["视频字幕", "专栏文章"] = "视频字幕"):
     prompt = (
         f"使用以下Markdown模板为我总结{type_}数据，除非{type_[2:]}中的内容无意义，或者内容较少无法总结，或者未提供{type_[2:]}数据，或者无有效内容，你就不使用模板回复，只回复“无意义”："
         + "## 概述\
         {内容，尽可能精简总结内容不要太详细}\
         ## 要点\
         - {使用不重复并合适的emoji，仅限一个，禁止重复} {内容不换行大于15字，可多项，条数与有效内容数量呈正比}\
@@ -72,28 +77,47 @@
         logger.info(f"Newbing summary: \n{bing_summary}")
         return bing_summary
     else:
         logger.debug(f"Newbing output is meaningless: \n{ai_summary}")
         return ""
 
 
-async def newbing_req(prompt: str):
+async def newbing_req(prompt: str, _is_retry: bool = False):
     logger.debug(f"prompt have {len(prompt)} chars")
-    raw = await bot.ask(
-        prompt=prompt,
-        conversation_style=ConversationStyle.creative,
-        wss_link="wss://sydney.bing.com/sydney/ChatHub",
-    )
-    await bot.reset()
-    res = BingChatResponse(raw=raw)
-    return (
-        newbing_summary_preprocess(res.content_answer)
-        if plugin_config.bilichat_newbing_preprocess
-        else res.content_answer
-    )
+    try:
+        if not isinstance(bot, Chatbot):
+            raise TypeError
+        raw = await bot.ask(
+            prompt=prompt,
+            conversation_style=ConversationStyle.creative,
+            wss_link="wss://sydney.bing.com/sydney/ChatHub",
+        )
+        await bot.reset()
+        res = BingChatResponse(raw=raw)
+        return (
+            newbing_summary_preprocess(res.content_answer)
+            if plugin_config.bilichat_newbing_preprocess
+            else res.content_answer
+        )
+    except BingChatResponseException as e:
+        raise e
+    except Exception as e:
+        if _is_retry:
+            raise e
+        # 如果没有重试，则刷新 bot 后重试
+        logger.warning(f"newbing summary failed (Retrying): {e}")
+        try:
+            logger.info("Try init bing chatbot")
+            loop = asyncio.get_running_loop()
+            executor = concurrent.futures.ThreadPoolExecutor()
+            await loop.run_in_executor(executor, init_chatbot)
+            assert bot, "Bing chatbot init failed"
+        except Exception:
+            return "newbing chatbot 失效，请检查 cookie 文件是否过期"
+        return await newbing_req(prompt, _is_retry=True)
 
 
 async def newbing_summarization(cache: Cache, cid: str = "0"):
     meaning = False
     try:
         if not cache.episodes[cid].newbing:
             if cache.id[:2].lower() in ["bv", "av"]:
```

### Comparing `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.5.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-2.6.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-2.5.0/pyproject.toml` & `nonebot_plugin_bilichat-2.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "2.5.0"
+version = "2.6.0"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.4",
```

### Comparing `nonebot_plugin_bilichat-2.5.0/PKG-INFO` & `nonebot_plugin_bilichat-2.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 2.5.0
+Version: 2.6.0
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
@@ -233,15 +233,15 @@
 注:
 
 1. openai 与 newbing 目前均需求科学上网才能使用，国内服务器请务必填写 `bilichat_openai_proxy` 或全局透明代理
 2. 如果同时填写了 `bilichat_openai_token` 和 `bilichat_newbing_cookie`，则会使用 `newbing` 进行总结, 并在 `newbing` 总结失败时使用 `openai` 进行总结
 3. `newbing` 和 `openai` 均有缓存机制，同一视频在**获取到正常的总结内容后**不会重复发送请求，如需刷新请求内容可以 [添加参数](#参数表) 或手动删除对应视频的缓存文件或整个缓存文件夹
 4. 经测试，目前 `newbing` 至少能总结 12000 字符以上的文本，推测 token 上限应为 `gpt-4-32k-0314` 的 `32200` token，但过长的内容易造成输出内容包含额外内容或总结失败，因此也建议设置一个合理的 token 上限 ~~（反正不要钱，要啥自行车）~~
 5. 由于 `newbing` 限制较大，也不如 `openai` 听话，且需要联网查询资料，因此使用体验并不如 chatgpt ~~（反正不要钱，要啥自行车）~~
-6. newbing cookie 文件获取方式参考[这里](https://github.com/acheong08/EdgeGPT#getting-authentication-required)和[这里](https://github.com/Harry-Jing/nonebot-plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)。目前 newbing 已正式公布且无需登录也可使用，填写 `bilichat_newbing_cookie=no_login` 即可无 cookie 使用
+6. newbing cookie 文件获取方式参考[这里](https://github.com/acheong08/EdgeGPT#getting-authentication-required)和[这里](https://github.com/Harry-Jing/nonebot-plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)。~~目前 newbing 已正式公布且无需登录也可使用，填写 `bilichat_newbing_cookie=no_login` 即可无 cookie 使用。~~ 目前无 cookie 使用**失败概率极高**，请谨慎考虑是否采用无 cookie 的方式。
 
 ## 🎉 使用
 
 直接发送视频(专栏)链接即可
 
 ### 参数表
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.5.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 2.6.0 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-Dist: nonebot-plugin-
 segbuilder>=0.2.0 Requires-Dist: nonebot2>=2.0.0 Requires-Dist: nonebot-plugin-
@@ -118,19 +118,20 @@
 tokenï¼ä½è¿é¿çåå®¹æé æè¾åºåå®¹åå«é¢å¤åå®¹ææ»ç»å¤±è´¥ï¼å æ­¤ä¹å»ºè®®è®¾ç½®ä¸ä¸ªåçç
 token ä¸é ~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ 5. ç±äº `newbing`
 éå¶è¾å¤§ï¼ä¹ä¸å¦ `openai`
 å¬è¯ï¼ä¸éè¦èç½æ¥è¯¢èµæï¼å æ­¤ä½¿ç¨ä½éªå¹¶ä¸å¦ chatgpt
 ~~ï¼åæ­£ä¸è¦é±ï¼è¦å¥èªè¡è½¦ï¼~~ 6. newbing cookie
 æä»¶è·åæ¹å¼åè[è¿é](https://github.com/acheong08/EdgeGPT#getting-
 authentication-required)å[è¿é](https://github.com/Harry-Jing/nonebot-
-plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)ãç®å newbing
+plugin-bing-chat#%EF%B8%8F-%E9%85%8D%E7%BD%AE)ã~~ç®å newbing
 å·²æ­£å¼å¬å¸ä¸æ éç»å½ä¹å¯ä½¿ç¨ï¼å¡«å
-`bilichat_newbing_cookie=no_login` å³å¯æ  cookie ä½¿ç¨ ## ð ä½¿ç¨
-ç´æ¥åéè§é¢(ä¸æ )é¾æ¥å³å¯ ### åæ°è¡¨
-å¨åéè§é¢æ¶ï¼å¯ä»¥é¢å¤æ·»å ä»¥ä¸ç±»ä¼¼ shell
+`bilichat_newbing_cookie=no_login` å³å¯æ  cookie ä½¿ç¨ã~~ ç®åæ 
+cookie ä½¿ç¨**å¤±è´¥æ¦çæé«**ï¼è¯·è°¨æèèæ¯å¦éç¨æ  cookie
+çæ¹å¼ã ## ð ä½¿ç¨ ç´æ¥åéè§é¢(ä¸æ )é¾æ¥å³å¯ ###
+åæ°è¡¨ å¨åéè§é¢æ¶ï¼å¯ä»¥é¢å¤æ·»å ä»¥ä¸ç±»ä¼¼ shell
 æä»¤çåæ°ï¼è¿èå¯¹è§£ææµç¨è¿è¡è°æ´ãä¾å¦ ```shell
 BV12v4y1E7NT --refresh BV12v4y1E7NT -r # å¯ä»¥ä½¿ç¨ç®å BV12v4y1E7NT -r --
 no-cache # å¯ä»¥å¤ä¸ªåæ°æ··ç¨ -r BV12v4y1E7NT -n #
 è½ç¶ä¸å»ºè®®ï¼ä½ç¡®å®å¯ä»¥æåæ°æ¾åé¢ ``` | æä»¤ | ç®å |
 è¯´æ | |:-----:|:----:|:----:| | --no-cache | -n | æ¬æ¬¡æ»ç»ç¦ç¨ç¼å­
 (ä¸ä¼å½±åå·²å­å¨çç¼å­æä»¶) | | --refresh | -r |
 å·æ°æ­¤è§é¢çè¯äºåæ»ç»ç¼å­(ä¼è¦çå·²å­å¨çç¼å­æä»¶) |
```

