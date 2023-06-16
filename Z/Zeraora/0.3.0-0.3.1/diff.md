# Comparing `tmp/Zeraora-0.3.0.tar.gz` & `tmp/Zeraora-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Zeraora-0.3.0.tar", last modified: Fri Jun  9 03:01:13 2023, max compression
+gzip compressed data, was "dist/Zeraora-0.3.1.tar", last modified: Fri Jun 16 07:31:18 2023, max compression
```

## Comparing `Zeraora-0.3.0.tar` & `Zeraora-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:01:13.000000 Zeraora-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-09 03:01:13.000000 Zeraora-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-09 03:00:58.000000 Zeraora-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:01:13.000000 Zeraora-0.3.0/Zeraora.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-09 03:01:13.000000 Zeraora-0.3.0/Zeraora.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-09 03:01:13.000000 Zeraora-0.3.0/Zeraora.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 03:01:13.000000 Zeraora-0.3.0/Zeraora.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 03:01:13.000000 Zeraora-0.3.0/Zeraora.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 03:01:13.000000 Zeraora-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-09 03:00:58.000000 Zeraora-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:01:13.000000 Zeraora-0.3.0/zeraora/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-09 03:00:58.000000 Zeraora-0.3.0/zeraora/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:01:13.000000 Zeraora-0.3.0/zeraora/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-09 03:00:58.000000 Zeraora-0.3.0/zeraora/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-09 03:00:58.000000 Zeraora-0.3.0/zeraora/constants/charsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-09 03:00:58.000000 Zeraora-0.3.0/zeraora/constants/division.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-06-09 03:00:58.000000 Zeraora-0.3.0/zeraora/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:01:13.000000 Zeraora-0.3.0/zeraora/dj/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-09 03:00:58.000000 Zeraora-0.3.0/zeraora/dj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-09 03:00:58.000000 Zeraora-0.3.0/zeraora/dj/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 03:01:13.000000 Zeraora-0.3.0/zeraora/drf/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-09 03:00:58.000000 Zeraora-0.3.0/zeraora/drf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-06-09 03:00:58.000000 Zeraora-0.3.0/zeraora/drf/viewsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-06-09 03:00:58.000000 Zeraora-0.3.0/zeraora/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    12256 2023-06-09 03:00:58.000000 Zeraora-0.3.0/zeraora/typeclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12159 2023-06-09 03:00:58.000000 Zeraora-0.3.0/zeraora/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:31:18.000000 Zeraora-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-16 07:31:18.000000 Zeraora-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-16 07:31:02.000000 Zeraora-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:31:18.000000 Zeraora-0.3.1/Zeraora.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-06-16 07:31:17.000000 Zeraora-0.3.1/Zeraora.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-16 07:31:18.000000 Zeraora-0.3.1/Zeraora.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:31:17.000000 Zeraora-0.3.1/Zeraora.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 07:31:17.000000 Zeraora-0.3.1/Zeraora.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 07:31:18.000000 Zeraora-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-06-16 07:31:03.000000 Zeraora-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:31:18.000000 Zeraora-0.3.1/zeraora/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-16 07:31:03.000000 Zeraora-0.3.1/zeraora/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:31:18.000000 Zeraora-0.3.1/zeraora/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-16 07:31:03.000000 Zeraora-0.3.1/zeraora/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-16 07:31:03.000000 Zeraora-0.3.1/zeraora/constants/charsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-16 07:31:03.000000 Zeraora-0.3.1/zeraora/constants/chores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-06-16 07:31:03.000000 Zeraora-0.3.1/zeraora/constants/division.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10784 2023-06-16 07:31:03.000000 Zeraora-0.3.1/zeraora/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:31:18.000000 Zeraora-0.3.1/zeraora/dj/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-16 07:31:03.000000 Zeraora-0.3.1/zeraora/dj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-06-16 07:31:03.000000 Zeraora-0.3.1/zeraora/dj/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:31:18.000000 Zeraora-0.3.1/zeraora/drf/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-16 07:31:03.000000 Zeraora-0.3.1/zeraora/drf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-16 07:31:03.000000 Zeraora-0.3.1/zeraora/drf/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-16 07:31:03.000000 Zeraora-0.3.1/zeraora/drf/viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-06-16 07:31:03.000000 Zeraora-0.3.1/zeraora/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-16 07:31:03.000000 Zeraora-0.3.1/zeraora/gvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-16 07:31:03.000000 Zeraora-0.3.1/zeraora/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13293 2023-06-16 07:31:03.000000 Zeraora-0.3.1/zeraora/typeclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16832 2023-06-16 07:31:03.000000 Zeraora-0.3.1/zeraora/utils.py
```

### Comparing `Zeraora-0.3.0/README.md` & `Zeraora-0.3.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 <h1 align="center" style="padding-top: 32px">Zeraora</h1>
 
 <div align="center">
-    <a href="https://docs.python.org/zh-cn/3/whatsnew/index.html"><img src="https://img.shields.io/pypi/pyversions/zeraora?label=Python&logo=python&logoColor=yellow"></a>
-    <a href="https://en.wikipedia.org/wiki/MIT_License"><img src="https://img.shields.io/badge/License-MIT-purple.svg"></a>
-    <a href="https://pypi.org/project/Zeraora/"><img src="https://img.shields.io/pypi/v/zeraora?color=darkgreen&label=PyPI"></a>
-    <a href=""><img src="https://img.shields.io/conda/v/conda-forge/zeraora"></a>
+    <a href="https://docs.python.org/zh-cn/3/whatsnew/index.html"><img src="https://img.shields.io/pypi/pyversions/zeraora?logo=python&logoColor=yellow"></a>
+    <a href="https://en.wikipedia.org/wiki/MIT_License"><img src="https://img.shields.io/pypi/l/Zeraora?color=purple"></a>
+    <a href="https://pypi.org/project/Zeraora/"><img src="https://img.shields.io/pypi/v/zeraora?color=darkgreen"></a>
+    <a href=""><img src="https://img.shields.io/pypi/dm/zeraora?color=C72777"></a>
+    <a href=""><img src="https://img.shields.io/pypi/status/Zeraora"></a>
+    <!--a href=""><img src="https://img.shields.io/conda/v/conda-forge/zeraora"></a-->
 </div>
 <div align="center">
-    <i>长期维护的个人开源工具库</i>
+    <i>实际应用积累的长期维护的实用开源工具库</i>
     <br>
-    <i>An utility Python package supports for my personal and company projects</i>
+    <i>A utility Python package for our personal and corporate projects, with long time support</i>
 </div>
 
+
 ## 特性
 
 - 支持with、注解和实例化三种方式调用的计时器 `BearTimer` ；
 - 生成通用representation方便调试时查看对象内部信息的 `ReprMixin` ；
 - 将字典的任意层级递归转化为对象，以便支持点分法访问数据的 `OnionObject` ；
-- 受 Django 的 `Choices` 启发的、可为枚举添加任意属性的 `Items` ；
+- 受 Django 的 `Choices` 和 Java 原生枚举语法启发的、可为枚举添加任意属性的 `Items` ；
 - 用以简化 `.as_view()` 传参的 `EasyViewSetMixin` ；
 - 仿照 `DestroyModelMixin` 实现的 `SoftDeleteModelMixin` ；
-- 安全转换快捷函数 `safecast()` 和链式调用安全转换的 `SafeCast` ；
+- 自动为Django模型生成下划线小写（即蛇形）数据表名的 `SnakeModel` ；
+- 包含34个省级行政区名称、区划代码、字母码、大区、简称、缩写的枚举 `Province` ；
 - 不强制依赖任何非[标准库](https://docs.python.org/zh-cn/3/library/index.html)；
 - 更多……
 
 ## 安装
 
 使用 pip 直接安装：
 
@@ -46,18 +50,25 @@
 
 ## 文档
 
 见[全局符号索引](./docs/README.md)。
 
 ## 版本
 
-|      | 状态[^1] | 支持时间 | 依赖              | 备注                                       |
-| ---- | -------- | -------- | ----------------- | ------------------------------------------ |
-| v0.3 | 🆕feature | 长期     | Python 3.7 或更新 | 趋于稳定，但改了包结构，不向下兼容。       |
-| v0.2 | ✅bugfix  | 长期     | Python 3.7 或更新 | 探索包结构，完善核心特性，补充非核心特性。 |
-| v0.1 | ❌EOL     | 不再支持 | Python 3.7 或更新 | 试验自动部署，只有核心特性。               |
+|       | 状态[^1] | 维护时间 | 依赖[^2]          | 备注                                                         |
+| ----- | -------- | -------- | ----------------- | ------------------------------------------------------------ |
+| 0.3.x | 🆕feature | 长期     | Python 3.7 或更新 | **分支**：main<br/>趋于稳定，但改了包结构，没办法向下兼容。  |
+| 0.2.x | ✅bugfix  | 长期     | Python 3.7 或更新 | **分支**：0.2.x<br/>探索包结构，完善核心特性，补充非核心特性。 |
+| 0.1.x | ❌EOL     | 不再维护 | Python 3.7 或更新 | **分支**：release/*<br/>试验自动部署，只有核心特性。         |
+
+[^1]: 概念参见[Python版本状态](https://devguide.python.org/versions/#status-key)。
+[^2]: 仅在最低依赖版本中进行(过)单元测试。
+
+## 分支
+
+主分支将从名为 `master` 的分支切换为 `main` 并且于2023年6月12日删除前者（自动同步不好做所以躺平了），原因是 `main` 听起来确实比前者要舒服一点点，若要深究的话参见[这里](https://stackoverflow.com/a/65021103)。两条分支是完全一致的，换句话说，后续的更新**就是**在 `master` 基础上进行的。
 
-[^1]: 概念参见[Python版本状态](https://devguide.python.org/versions/#status-key)，目前只借用了以上三种。
+## 帮助
 
-## 计划
+这个包偏向于抽象及封装一些实际在用的实用功能，目前整体趋于稳定，如需部署生产环境，请优先考虑 0.3.x 或后续更新的版本。
 
-- [ ] 打包到conda（未来，未来。）
+欢迎通过 Issue 或 Pull Request 来提出功能创意、命名建议，亦或反馈问题、修复漏洞、编写测试等等等等；如有需要，可以进入QQ群 699090940 获取帮助。
```

#### html2text {}

```diff
@@ -1,34 +1,47 @@
                              ****** Zeraora ******
-                   [https://img.shields.io/pypi/pyversions/
-  zeraora?label=Python&logo=python&logoColor=yellow] [https://img.shields.io/
-         badge/License-MIT-purple.svg] [https://img.shields.io/pypi/v/
-  zeraora?color=darkgreen&label=PyPI] [https://img.shields.io/conda/v/conda-
-                                forge/zeraora]
-                     é¿æç»´æ¤çä¸ªäººå¼æºå·¥å·åº
-    An utility Python package supports for my personal and company projects
+[https://img.shields.io/pypi/pyversions/zeraora?logo=python&logoColor=yellow]
+ [https://img.shields.io/pypi/l/Zeraora?color=purple] [https://img.shields.io/
+       pypi/v/zeraora?color=darkgreen] [https://img.shields.io/pypi/dm/
+      zeraora?color=C72777] [https://img.shields.io/pypi/status/Zeraora]
+          å®éåºç¨ç§¯ç´¯çé¿æç»´æ¤çå®ç¨å¼æºå·¥å·åº
+  A utility Python package for our personal and corporate projects, with long
+                                 time support
 ## ç¹æ§ - æ¯æwithãæ³¨è§£åå®ä¾åä¸ç§æ¹å¼è°ç¨çè®¡æ¶å¨
 `BearTimer` ï¼ -
 çæéç¨representationæ¹ä¾¿è°è¯æ¶æ¥çå¯¹è±¡åé¨ä¿¡æ¯ç
 `ReprMixin` ï¼ -
 å°å­å¸çä»»æå±çº§éå½è½¬åä¸ºå¯¹è±¡ï¼ä»¥ä¾¿æ¯æç¹åæ³è®¿é®æ°æ®ç
-`OnionObject` ï¼ - å Django ç `Choices`
-å¯åçãå¯ä¸ºæä¸¾æ·»å ä»»æå±æ§ç `Items` ï¼ - ç¨ä»¥ç®å
-`.as_view()` ä¼ åç `EasyViewSetMixin` ï¼ - ä»¿ç§ `DestroyModelMixin`
-å®ç°ç `SoftDeleteModelMixin` ï¼ - å®å¨è½¬æ¢å¿«æ·å½æ° `safecast()`
-åé¾å¼è°ç¨å®å¨è½¬æ¢ç `SafeCast` ï¼ - ä¸å¼ºå¶ä¾èµä»»ä½é
-[æ ååº](https://docs.python.org/zh-cn/3/library/index.html)ï¼ -
-æ´å¤â¦â¦ ## å®è£ ä½¿ç¨ pip ç´æ¥å®è£ï¼ ```shell pip install zeraora
-``` ä¸´æ¶éè¿æ¬å°ä»£çä½¿ç¨ pip å®è£ï¼ ```shell pip install zeraora -
--proxy=127.0.0.1:6666 ``` ä½¿ç¨ pip æ¶ä¸´æ¶æå®å®è£æºæ¥å®è£ï¼
-```shell pip install zeraora -i http://pypi.mirrors.ustc.edu.cn/simple/ ``` ##
-ææ¡£ è§[å¨å±ç¬¦å·ç´¢å¼](./docs/README.md)ã ## çæ¬ | | ç¶æ[^1] |
-æ¯ææ¶é´ | ä¾èµ | å¤æ³¨ | | ---- | -------- | -------- | ---------------
--- | ------------------------------------------ | | v0.3 | ðfeature | é¿æ
-| Python 3.7 ææ´æ° | è¶äºç¨³å®ï¼ä½æ¹äºåç»æï¼ä¸åä¸å¼å®¹ã
-| | v0.2 | âbugfix | é¿æ | Python 3.7 ææ´æ° |
-æ¢ç´¢åç»æï¼å®åæ ¸å¿ç¹æ§ï¼è¡¥åéæ ¸å¿ç¹æ§ã | | v0.1 |
-âEOL | ä¸åæ¯æ | Python 3.7 ææ´æ° |
+`OnionObject` ï¼ - å Django ç `Choices` å Java
+åçæä¸¾è¯­æ³å¯åçãå¯ä¸ºæä¸¾æ·»å ä»»æå±æ§ç `Items` ï¼ -
+ç¨ä»¥ç®å `.as_view()` ä¼ åç `EasyViewSetMixin` ï¼ - ä»¿ç§
+`DestroyModelMixin` å®ç°ç `SoftDeleteModelMixin` ï¼ -
+èªå¨ä¸ºDjangoæ¨¡åçæä¸åçº¿å°åï¼å³èå½¢ï¼æ°æ®è¡¨åç
+`SnakeModel` ï¼ -
+åå«34ä¸ªççº§è¡æ¿åºåç§°ãåºåä»£ç ãå­æ¯ç ãå¤§åºãç®ç§°ãç¼©åçæä¸¾
+`Province` ï¼ - ä¸å¼ºå¶ä¾èµä»»ä½é[æ ååº](https://docs.python.org/
+zh-cn/3/library/index.html)ï¼ - æ´å¤â¦â¦ ## å®è£ ä½¿ç¨ pip
+ç´æ¥å®è£ï¼ ```shell pip install zeraora ``` ä¸´æ¶éè¿æ¬å°ä»£çä½¿ç¨
+pip å®è£ï¼ ```shell pip install zeraora --proxy=127.0.0.1:6666 ``` ä½¿ç¨
+pip æ¶ä¸´æ¶æå®å®è£æºæ¥å®è£ï¼ ```shell pip install zeraora -i http:/
+/pypi.mirrors.ustc.edu.cn/simple/ ``` ## ææ¡£ è§[å¨å±ç¬¦å·ç´¢å¼](./docs/
+README.md)ã ## çæ¬ | | ç¶æ[^1] | ç»´æ¤æ¶é´ | ä¾èµ[^2] | å¤æ³¨ | |
+----- | -------- | -------- | ----------------- | -----------------------------
+------------------------------- | | 0.3.x | ðfeature | é¿æ | Python 3.7
+ææ´æ° | **åæ¯**ï¼main
+è¶äºç¨³å®ï¼ä½æ¹äºåç»æï¼æ²¡åæ³åä¸å¼å®¹ã | | 0.2.x |
+âbugfix | é¿æ | Python 3.7 ææ´æ° | **åæ¯**ï¼0.2.x
+æ¢ç´¢åç»æï¼å®åæ ¸å¿ç¹æ§ï¼è¡¥åéæ ¸å¿ç¹æ§ã | | 0.1.x |
+âEOL | ä¸åç»´æ¤ | Python 3.7 ææ´æ° | **åæ¯**ï¼release/*
 è¯éªèªå¨é¨ç½²ï¼åªææ ¸å¿ç¹æ§ã | [^1]: æ¦å¿µåè§
-[Pythonçæ¬ç¶æ](https://devguide.python.org/versions/#status-
-key)ï¼ç®ååªåç¨äºä»¥ä¸ä¸ç§ã ## è®¡å - [ ]
-æåå°condaï¼æªæ¥ï¼æªæ¥ãï¼
+[Pythonçæ¬ç¶æ](https://devguide.python.org/versions/#status-key)ã [^2]:
+ä»å¨æä½ä¾èµçæ¬ä¸­è¿è¡(è¿)ååæµè¯ã ## åæ¯
+ä¸»åæ¯å°ä»åä¸º `master` çåæ¯åæ¢ä¸º `main`
+å¹¶ä¸äº2023å¹´6æ12æ¥å é¤åèï¼èªå¨åæ­¥ä¸å¥½åæä»¥èººå¹³äºï¼ï¼åå æ¯
+`main` å¬èµ·æ¥ç¡®å®æ¯åèè¦èæä¸ç¹ç¹ï¼è¥è¦æ·±ç©¶çè¯åè§
+[è¿é](https://stackoverflow.com/a/
+65021103)ãä¸¤æ¡åæ¯æ¯å®å¨ä¸è´çï¼æ¢å¥è¯è¯´ï¼åç»­çæ´æ°**å°±æ¯**å¨
+`master` åºç¡ä¸è¿è¡çã ## å¸®å©
+è¿ä¸ªåååäºæ½è±¡åå°è£ä¸äºå®éå¨ç¨çå®ç¨åè½ï¼ç®åæ´ä½è¶äºç¨³å®ï¼å¦éé¨ç½²çäº§ç¯å¢ï¼è¯·ä¼åèè
+0.3.x æåç»­æ´æ°ççæ¬ã æ¬¢è¿éè¿ Issue æ Pull Request
+æ¥æåºåè½åæãå½åå»ºè®®ï¼äº¦æåé¦é®é¢ãä¿®å¤æ¼æ´ãç¼åæµè¯ç­ç­ç­ç­ï¼å¦æéè¦ï¼å¯ä»¥è¿å¥QQç¾¤
+699090940 è·åå¸®å©ã
```

### Comparing `Zeraora-0.3.0/setup.py` & `Zeraora-0.3.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 setup(
     name='Zeraora',
     version=version,
     url='https://github.com/aixcyi/zeraora',
     license='MIT',
     author='aixcyi',
     author_email='75880483+aixcyi@users.noreply.github.com',
-    description="一个长期维护的个人开源工具库。"
-                "A utility Python package supports for my personal and company projects.",
+    description="实际应用积累的长期维护的实用开源工具库。"
+                "A utility Python package for our personal and corporate projects, with long time support.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
@@ -41,9 +41,9 @@
         "Typing :: Typed",
     ],
     project_urls={
         "Source": "https://github.com/aixcyi/zeraora",
         "Tracker": "https://github.com/aixcyi/zeraora/issues",
     },
     python_requires='>=3.7',
-    packages=find_packages(where=".", exclude=['test*']),
+    packages=find_packages(where=".", exclude=['test*', 'dataset']),
 )
```

### Comparing `Zeraora-0.3.0/zeraora/constants/charsets.py` & `Zeraora-0.3.1/zeraora/constants/charsets.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.0/zeraora/converters.py` & `Zeraora-0.3.1/zeraora/converters.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 用于将一种值转换为另一种值的转换器。
 """
 
 __all__ = [
     'delta2hms', 'delta2ms', 'delta2s',
+    'wdate', 'get_week_range', 'get_week_side',
+    'get_week_in_year',
     'represent', 'datasize', 'dsz', 'true',
     'SafeCaster', 'safecast', 'safecasts',
     'remove_exponent',
 ]
 
 import re
 from datetime import timedelta, datetime, date
@@ -60,14 +62,99 @@
 
     :param delta: 时间增量。
     :return: 一个小数。
     """
     return delta.seconds + delta.microseconds / 1000000
 
 
+# 仿构造器命名
+def wdate(year: int, week_in_year: int, day_in_week: int, sunday_first=False) -> date:
+    """
+    将某一年的某一周的星期几转换为一个具体的日期。
+
+    :param year: 具体年份。比如 2012、2023 等。
+    :param week_in_year: 一年中的第几周。从 0 开始。
+    :param day_in_week: 星期几。0 表示周日、1 表示周一，以此类推。
+    :param sunday_first: 是否以周日为一周的开始。
+    :return: 一个日期。
+    """
+    day = f'{year:04d}-{week_in_year:02d}-{day_in_week:1d}'
+    fmt = '%Y-%U-%w' if sunday_first else '%Y-%W-%w'
+    return datetime.strptime(day, fmt).date()
+
+
+def get_week_range(year: int,
+                   week_in_year: int,
+                   month: int = UNSET,
+                   sunday_first=False) -> Tuple[date, ...]:
+    """
+    计算一年中某一周对应的所有日期。
+
+    :param year: 具体年份。比如 2012、2023 等。
+    :param week_in_year: 一年中的第几周。从 0 开始。
+    :param month: 具体月份。若指定了这个参数，则只计算这个月的那一部分日期。
+    :param sunday_first: 是否以周日为一周的开始。
+    :return: 若指定了不恰当的月份，有可能返回空列表。
+    :raise ValueError: year 年的 week_in_year 周不在当年的 month 月里。
+    """
+    fmt = '%Y-%U-%w' if sunday_first else '%Y-%W-%w'
+    start = f'{year:04d}-{week_in_year:02d}-{0 if sunday_first else 1}'
+    start = datetime.strptime(start, fmt).date()
+    days = tuple(start + timedelta(days=i) for i in range(7))
+    days = days if month is UNSET else tuple(day for day in days if day.month == month)
+    if not days:
+        raise ValueError(
+            f'{year} 年的 {week_in_year} 周不在当年的 {month} 月里。'
+        )
+    return days
+
+
+def get_week_side(year: int,
+                  week_in_year: int,
+                  month: int = UNSET,
+                  sunday_first=False) -> Tuple[date, date]:
+    """
+    计算一年中某一周对应的第一天和最后一天。
+
+    :param year: 具体年份。比如 2012、2023 等。
+    :param week_in_year: 一年中的第几周。从 0 开始。
+    :param month: 具体月份。若指定了这个参数，则只计算这个月的那一部分日期。
+    :param sunday_first: 是否以周日为一周的开始。
+    :return: 两个日期，表示（这个月的）这一周的第一天和最后一天。
+    :raise ValueError: year 年的 week_in_year 周不在当年的 month 月里。
+    """
+    days = get_week_range(year, week_in_year, month, sunday_first)
+    return days[0], days[-1]
+
+
+def get_week_in_year(*args, sunday_first=False) -> int:
+    """
+    计算一个具体日期自一年开始的周序号。
+
+    如果 ``sunday_first=False`` ，那么一年中第一个星期一之前的日子都算作第 0 周。
+    如果 ``sunday_first=True`` ，那么一年中第一个星期日之前的日子都算作第 0 周。
+
+    - ``get_week_in_year(date)`` ，提供一个日期。
+    - ``get_week_in_year(datetime)`` ，提供一个时刻。
+    - ``get_week_in_year(int, int, int)`` ，分别提供年月日。
+
+    :param args: 参数。
+    :param sunday_first: 是否以周日作为一周的开始。
+    :return: 一个从 0 开始递增的整数。
+    """
+    if len(args) == 1 and isinstance(args[0], date):
+        day = args[0]
+    elif len(args) >= 3 and all(isinstance(a, int) for a in args):
+        day = date(*args[:3])
+    else:
+        raise ValueError
+    week = day.strftime('%U') if sunday_first else day.strftime('%W')
+    return int(week)
+
+
 def represent(value: Any) -> str:
     """
     将任意值转换为一个易于阅读的字符串。
 
     也是 ReprMixin 的默认格式化函数。
 
     默认使用 repr() 函数进行转换。如果自定义的类需要实现被此函数转换，请重写 .__repr__() 方法。
@@ -107,17 +194,15 @@
     - 1 MB == 1000 KB
     - 1 MiB == 1024 KiB
 
     :param literal: 一个整数后缀数据大小的单位。
     :return:
     """
     if not isinstance(literal, str):
-        raise TypeError(
-            '不支持解析一个非字符串类型的值。'  # pragma: no cover
-        )
+        raise TypeError('不支持解析一个非字符串类型的值。')
 
     pattern = re.compile(r'^([0-9]+)\s*([KMGTPEZY]?)(i?[Bb])$')
     result = re.fullmatch(pattern, literal)
 
     if result is None:
         return 0
 
@@ -135,15 +220,15 @@
 def true(value) -> bool:
     """
     将HTTP请求中 query 部分的参数值转换为 Python 的逻辑值。
 
     :param value: query 中的参数值。
     :return: True 或 False。
     """
-    return value in ('true', 'True', 'TRUE', 1, True)
+    return value in ('true', 'True', 'TRUE', 1, True, '1')
 
 
 def safecast(mapper: Callable, raw, *errs: Throwable, default=None) -> Any:
     """
     转换一个值，转换失败时返回default，确保不会发生指定异常。
 
     默认捕获以下异常，可以通过errs参数追加更多异常：
@@ -160,31 +245,31 @@
     exceptions = tuple(
         exc for exc in errs
         if exc.__class__ is type
         and issubclass(exc, BaseException)
         or isinstance(exc, BaseException)
     )
     if not callable(mapper):
-        return default  # pragma: no cover
+        return default
     try:
         return mapper(raw)
     except (TypeError, ValueError, KeyboardInterrupt) + exceptions:
         return default
 
 
 class SafeCaster:
+    _exceptions = ()
 
     def __init__(self, raw: Any = UNSET):
         """
         创建一个安全转换器，用于转换某个值而不发生特定异常。若不提供初值，则第一个转换器也必须允许无参调用。
         """
         self._value = raw
         self._default = None
         self._converters = tuple()
-        self._exceptions = tuple()
 
     def __call__(self, raw: Any = UNSET) -> 'SafeCaster':
         self._value = raw
         return self
 
     def catch(self, *exceptions: Throwable) -> 'SafeCaster':
         """
@@ -208,24 +293,29 @@
         )
         return self
 
     def get(self, default=None) -> Any:
         """
         执行转换并返回转换结果。若触发置入的异常或没有置入转换器则返回默认值；若触发未被置入的异常将原样抛出。
         """
-        if len(self._converters) <= 0:
-            return default
+        result = self.__invoke(default)
+        self.__init__()
+        return result
 
+    def __invoke(self, default) -> Any:
         if self._value is UNSET:
             result = self._converters[0]()
             converters = self._converters[1:]
         else:
             result = self._value
             converters = self._converters
 
+        if len(self._converters) <= 0:
+            return default
+
         try:
             for converter in converters:
                 result = converter(result) if callable(converter) else result
             return result
         except self._exceptions:
             return default
```

### Comparing `Zeraora-0.3.0/zeraora/drf/viewsets.py` & `Zeraora-0.3.1/zeraora/drf/viewsets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 """
 对 Django REST Framework 视图集（viewset）的增强。
 """
+
+__all__ = [
+    'EasyViewSetMixin',
+    'SoftDeleteModelMixin',
+]
+
 from typing import Any, Dict
 
 try:
     from django.utils.decorators import classonlymethod
     from rest_framework import status
     from rest_framework.response import Response
     from rest_framework.viewsets import ViewSetMixin
-except ImportError:
-    print('需要安装Django以及DRF框架：pip install django djangorestframework')
-    raise
+except ImportError as e:
+    raise ImportError('需要安装Django以及DRF框架：\npip install django djangorestframework') from e
 
 
 class EasyViewSetMixin(ViewSetMixin):
     """
     提供了两个方法来简化 ``.as_view()`` 的传参。
 
     适用于：
```

### Comparing `Zeraora-0.3.0/zeraora/generators.py` & `Zeraora-0.3.1/zeraora/generators.py`

 * *Files identical despite different names*

### Comparing `Zeraora-0.3.0/zeraora/typeclasses.py` & `Zeraora-0.3.1/zeraora/typeclasses.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         :param depth: 递归转化的层数。负数表示无限递归转化，正数表示递归层数，0无意义。
         :return: OnionObject 的对象。
         :raise TypeError: 属性名称必须是字符串。
         """
         if dictionary is None:
             dictionary = {}
         if not isinstance(dictionary, dict):
-            raise TypeError  # pragma: no cover
+            raise TypeError
         if depth == 0:
             return dictionary
         dictionary.update(kvs)
 
         self = object.__new__(cls)
         self.__depth = depth
         self.__ior__(dictionary)
@@ -157,15 +157,15 @@
                 if be else
                 int.from_bytes(x, 'little', signed=negative)
             )
 
         elif isinstance(x, (tuple, list)):
             if min(x) < 0:
                 raise ValueError('x 只能包含非负整数。')
-            radix = max(x)
+            radix = max(x) + 1
             if not radix <= n:
                 raise ValueError(
                     f'x 的进位制最低是 {radix}，高于给定的 {n} 。'
                 )
             pairs = zip(x, reversed(range(len(x))))
             self = tuple.__new__(cls, x[::-1] if be else x)
             self._radix = n
@@ -214,17 +214,29 @@
             )
         pks = classdict['__properties__']
         if not isinstance(pks, (tuple, list)):
             raise TypeError(
                 f'{classname}.__properties__ 只允许是一个 tuple 或 list 。'
             )
         if not all(isinstance(pk, str) and not pk.startswith('_') for pk in pks):
-            raise TypeError(
+            raise ValueError(
                 f'{classname}.__properties__ 的值必须是字符串且不以下划线 “_” 开头。'
             )
+        for pk in pks:
+            # https://docs.python.org/zh-cn/3/library/enum.html#supported-sunder-names
+            if pk in ('name', 'value'):
+                raise KeyError(
+                    f'不能也不必在 {classname}.__properties__ 中定义 name 和 value，'
+                    f'它们是原生枚举就已经支持的。'
+                )
+            if pk in ('generate_next_value',):
+                raise KeyError(
+                    f'不能在 {classname}.__properties__ 中定义 {pk}，'
+                    f'因为它会被转化成 _{pk}_ ，而这属于保留名称。'
+                )
         pks = tuple(f'_{pk}_' for pk in pks)
         qty = len(pks) + 1  # 等号右侧所有元素的总数
 
         # 获取属性值（pvs）和枚举值（value）
         pvs_list = []
         for key in classdict._member_names:
             value = classdict[key]
@@ -246,61 +258,72 @@
         if not isinstance(member, enum.Enum):
             # Allow non-enums to match against member values.
             return any(x.value == member for x in cls)
         return super().__contains__(member)
 
     def __getattr__(cls, name):
         if not isinstance(name, str):
-            raise TypeError
+            raise TypeError  # pragma: no cover
         if name[:-1] in cls.__properties__ and name.endswith('s'):
             return [getattr(member, name[:-1]) for member in cls]
         if name[:-2] in cls.__properties__ and name.endswith('es'):
             return [getattr(member, name[:-2]) for member in cls]
         return object.__getattribute__(cls, name)
 
     # 对 __empty__ 属性的支持是为了与 Django 的 Choices 相兼容，可参见：
     # https://docs.djangoproject.com/zh-hans/4.2/ref/models/fields/#enumeration-types
 
     @property
     def names(cls) -> t.List[str]:
+        """
+        所有枚举成员的名称（定义枚举成员时的全大写变量名）。
+        """
         empty = ["__empty__"] if hasattr(cls, "__empty__") else []
         return empty + [member.name for member in cls]
 
     @property
     def values(cls) -> list:
+        """
+        所有枚举成员的值（定义枚举成员时等号右边元组的第一个值）。
+        """
         empty = [None] if hasattr(cls, "__empty__") else []
         return empty + [member.value for member in cls]
 
     @property
     def items(cls) -> t.Dict[str, t.Any]:
+        """
+        所有枚举成员的名称和值。
+        """
         its = {"__empty__": None} if hasattr(cls, "__empty__") else {}
-        its.update({member.name: member.value for member in cls})
+        its.update((member.name, member.value) for member in cls)
         return its
 
     @property
-    def choices(cls) -> t.List[t.Tuple[t.Union[str, None], t.Any]]:
+    def choices(cls) -> t.List[t.Union[t.Tuple[str, t.Any], t.Tuple[None, t.Any]]]:
+        """
+        所有枚举成员的值，和所有枚举成员的属性中的标签（label）。
+        """
         if 'label' not in cls.__properties__:
             raise AttributeError(
                 '使用 .choices 属性前必须在 __properties__ 中'
                 '添加一个名为 "label" 的属性，且必须保证枚举值中有相应的属性值。'
             )
         empty = [(None, cls.__empty__)] if hasattr(cls, "__empty__") else []
         return empty + [(member.value, member.label) for member in cls]
 
-    def value_of(cls, value: str) -> enum.Enum:
+    def asdict(cls) -> t.Dict[enum.Enum, t.Any]:
         """
-        将一个枚举值转换为一个枚举。
-
-        :raise ValueError: 在枚举类中没有找到相应的枚举.
+        返回枚举成员与枚举值之间的映射。
         """
-        if value not in cls._value2member_map_:
-            raise ValueError(
-                f'{cls.__name__} 不存在值为 {value!s} 的枚举。'
-            )
-        return cls._value2member_map_[value]
+        return {member: member.value for member in cls}
+
+    def value_of(cls, value: str) -> enum.Enum:
+        raise NotImplementedError(
+            f'该方法是多余的，请使用 {cls.__name__}(value) 代替。'
+        )  # pragma: no cover
 
 
 class Items(enum.Enum, metaclass=ItemsMeta):
     """
     用于创建带有任意属性的枚举。
 
     >>> from enum import Enum
```

### Comparing `Zeraora-0.3.0/zeraora/utils.py` & `Zeraora-0.3.1/zeraora/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,30 @@
 """
 偏工具属性的类与函数。
 """
+
+__all__ = [
+    'bear_config', 'BearTimer', 'ReprMixin', 'start', 'deprecate',
+    'load_ads4', 'warn_empty_ads',
+]
+
+import json
 import logging
 import sys
-from datetime import datetime
+import warnings
+from decimal import Decimal
 from functools import wraps
-from typing import Tuple, Optional
-
-from .converters import delta2s, represent
+from itertools import groupby
+from pathlib import Path
+from time import time_ns
+from typing import Tuple, NoReturn, Union
+
+from . import gvs
+from .converters import represent
+from .structures import DivisionCode
 
 logger_bear = logging.getLogger('zeraora.bear')
 
 bear_config = {
     'version': 1,
     'formatters': {
         'bear': {
@@ -42,17 +55,50 @@
         },
     },
 }
 
 
 class BearTimer(object):
 
-    def __init__(self, label: str = None, printable=True):
+    def __init__(self, label: str = None, *_, **__):
         """
-        熊牌计时器。对代码运行进行计时，并打印时间和提示。
+        熊牌计时器。对代码运行进行计时，并向名为 "zeraora.bear" 的Logger发送DEBUG等级的日志。
+
+        ----
+
+        使用前，需要先启用日志输出：
+
+        >>> import logging.config
+        >>> from zeraora.utils import BearTimer, bear_config
+        >>>
+        >>> logging.config.dictConfig(bear_config)
+        >>> bear = BearTimer()
+
+        对于使用 Django 的项目可以改为在 settings.py 中进行如下设置：
+
+        >>> LOGGING = {
+        >>>     'version': 1,
+        >>>     'formatters': {...},
+        >>>     'filters': {...},
+        >>>     'handlers': {
+        >>>         'Console': {
+        >>>             'level': 'DEBUG',
+        >>>             'class': 'logging.StreamHandler',
+        >>>         },
+        >>>         # ...
+        >>>     },
+        >>>     'loggers': {
+        >>>         'zeraora.bear': {
+        >>>             'level': 'DEBUG',
+        >>>             'handlers': ['Console'],
+        >>>         },
+        >>>     },
+        >>> }
+
+        ----
 
         最简单是使用 ``with`` 语句包裹需要计时的部分：
 
         >>> with BearTimer() as bear:
         >>>     # 业务逻辑
         >>>     pass
 
@@ -83,30 +129,20 @@
         此外还可以实例化一个对象。每个对象都是独立的计时器，互不影响。
 
         >>> bear = BearTimer()
         >>> bear.start()
         >>> # 业务逻辑
         >>> bear.stop()
 
-        若需要将计时消息输出到日志而非标准输出时，如果没有使用框架，可以通过以下方法启用日志记录：
-
-        >>> import logging.config
-        >>> from zeraora.utils import BearTimer, bear_config
-        >>>
-        >>> logging.config.dictConfig(bear_config)
-        >>> bear = BearTimer(printable=False)
-
         :param label: 计时器的标题，用以标明输出信息归属于哪个计时器。默认从打印消息时的上下文中获取。
-        :param printable: 若为True，消息会打印到系统标准输出；
-                          若为False，则向名为 "zeraora.bear" 的Logger发送DEBUG等级的日志。
         """
-        self._start = None  # 计时开始时间
-        self._point = None  # 中途标记时间（用于计算距离上次标记过去了多久）
-        self._print = printable
-        self._label = sys._getframe().f_back.f_code.co_name if not label and hasattr(sys, '_getframe') else str(label)
+        context = sys._getframe().f_back.f_code.co_name
+        self._start: int = 0  # 计时开始时间
+        self._point: int = 0  # 中途标记时间（用于计算距离上次标记过去了多久）
+        self._label = context if not label and hasattr(sys, '_getframe') else str(label)
 
     def __call__(self, func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             self._label = func.__name__
             self.start()
             returns = func(*args, **kwargs)
@@ -118,69 +154,66 @@
     def __enter__(self):
         self.start()
         return self
 
     def __exit__(self, exc_type, exc_val, traceback):
         self.stop()
 
-    def _record(self, msg: str = '') -> datetime:
+    def _record(self, msg: str = '') -> int:
         """
         打印一行消息，标明此刻的时间、经历的时长、距上次打印的时长、计时器标题，以及附加的消息。
 
         :param msg: 要附加的消息。默认为空文本。
-        :return: 此时的时刻。
+        :return: 自纪元以来的当前时间（以纳秒为单位）。
         """
-        now = datetime.now()
-        total = delta2s(now - self._start) if self._start else 0
-        delta = delta2s(now - self._point) if self._point else 0
-        if self._print:
-            print(f'[{now:%H:%M:%S.%f}] [{self._label}] [{total:.6f} +{delta:.6f}]: {msg}')
-        else:
-            logger_bear.debug(f'[{self._label}] [{total:.6f} +{delta:.6f}]: {msg}')
+        now = time_ns()
+        total = Decimal((now - self._start) if self._start else 0) / 1000000000
+        delta = Decimal((now - self._point) if self._point else 0) / 1000000000
+        logger_bear.debug(f'[{self._label}] [{total:.9f} +{delta:.9f}]: {msg}')
         self._point = now
         return now
 
     def start(self, msg='Starting...'):
         """
         开始计时。
 
         如果计时尚未结束，会重新开始计时，中途记录的标记也会被清除。
 
         :param msg: 要附加的消息。
         :return: 计时器对象自身。
         """
-        self._point = None
-        self._start = datetime.now()
+        self._point = 0
+        self._start = time_ns()
         self._record(msg)
         return self
 
-    def step(self, msg='') -> Tuple[Optional[datetime], datetime]:
+    def step(self, msg='') -> Tuple[int, int]:
         """
         中途标记。
 
         用此方法可以计算出距离上一次标记/开始计时过去了多久。
 
         如果计时器尚未开始计时，那么过去的时间始终是 0 秒。
 
         :param msg: 要附加的消息。
-        :return: 二元元组。包含上一次标记/开始计时的时刻，和此时的时刻。
+        :return: 二元元组。包含上一次标记/开始计时的时刻，和此时的时刻。时刻是自纪元以来的当前时间（以纳秒为单位）。
         """
         prev = self._point
         curr = self._record(msg)
         return prev, curr
 
-    def stop(self, msg='Stopped.') -> datetime:
+    def stop(self, msg='Stopped.') -> int:
         """
         结束计时。
 
         :param msg: 要附加的消息。
-        :return: 此时的时刻。
+        :return: 返回自纪元以来的当前时间（以纳秒为单位）。
         """
         curr = self._record(msg)
-        self._start = None
+        self._start = 0
         return curr
 
 
 class ReprMixin(object):
     """
     重写 ``self.__repr__()`` 来生成特定格式的representation。
 
@@ -347,7 +380,113 @@
             pk = self.id
         else:
             return ''
         return pk if isinstance(pk, str) else represent(pk)
 
     def _obtain_kls(self) -> str:
         return self.__class__.__name__
+
+
+def start(*version, note: str = None):
+    """
+    检查 Python 版本是否高于或等于指定值，
+    如果低于指定的版本就会抛出 RuntimeError。
+
+    若提供了 ``note`` 参数，则会在末尾输出。
+    """
+
+    def decorator(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            if sys.version_info < version:
+                v = '.'.join(map(str, version))
+                raise RuntimeError(
+                    # 英文在前保证控制台出现乱码时不会掩盖该错误信息
+                    f'Require Python version {v} or above to run. '
+                    f'Python运行版本需要在 {v} 或以上。'
+                    + ('' if note is None else note)
+                )
+            return func(*args, **kwargs)
+
+        return wrapper
+
+    return decorator
+
+
+def deprecate(*since,
+              ref=sys.version_info,
+              reason: str = 'This function is deprecated since %(since)s .',
+              suggestion: str = 'This function will be deprecate at %(since)s .',
+              migration: str = None,
+              ):
+    """
+    为一个函数作废弃标记。
+
+    :param since: 自哪个版本开始废弃。
+    :param ref: 参照版本。用于确定状态是准备废弃还是已经废弃。
+    :param reason: 已废弃的原因。（废弃后的提示）
+    :param suggestion: 准备废弃时提供的建议。（废弃前的提示）
+    :param migration: 假设废弃之后应该采取的迁移措施或用法变更说明。
+    """
+
+    def decorator(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            tips = (suggestion if ref < since else reason) % dict(since='.'.join(map(str, since)))
+            tips += ('\n' + migration) if migration else ''
+            if ref < since:
+                warnings.warn(tips, category=PendingDeprecationWarning, stacklevel=2)
+            else:
+                warnings.warn(tips, category=DeprecationWarning, stacklevel=2)
+            return func(*args, **kwargs)
+
+        return wrapper
+
+    return decorator
+
+
+def warn_empty_ads():
+    """
+    在未载入行政区划映射表时发出警告。（您不应该使用此方法，它只在包内使用）
+    """
+    if not gvs.ad_map or not gvs.ad_tree:
+        warnings.warn('未载入行政区划映射表，该方法可能会失效或返回非期望值。', category=UserWarning)
+
+
+def load_ads4(fp: Union[str, Path], encoding='UTF-8', **kwargs) -> NoReturn:
+    """
+    读取并过滤前四级行政区划，然后赋值给全局变量 ``zeraora.gvs.ad_map`` 和 ``zeraora.gvs.ad_tree`` 。
+
+    测试数据可以在 `GitHub <https://github.com/aixcyi/zeraora/tree/main/dataset>`_
+    或 `码云 <https://github.com/aixcyi/zeraora/tree/main/dataset>`_ 中找到。
+
+    ----
+
+    警告：这会耗费一定的时间并且占用一些内存，同时造成线程阻塞，请在合适的时候再执行调用。
+
+    :param fp: 数据文件地址。
+    :param encoding: 文件编码。
+    :param kwargs: 其它提供给 ``open()`` 的参数。
+    :return: 无
+    """
+    with open(fp, 'r', encoding=encoding, **kwargs) as f:
+        data = json.load(f)
+    if not isinstance(data, dict):
+        raise ValueError('提供的数据不是一对一映射。')  # pragma: no cover
+
+    steam = data.items()
+    steam = ((c, n) for c, n in steam if isinstance(c, str) and isinstance(n, str))
+    steam = ((DivisionCode.fromcode(c), n) for c, n in steam)
+    steam = ((c, n) for c, n in steam if c.village == '000')  # 只要前四个级别
+    steam = ((c, n) for c, n in steam if (c.county != '00' and c.township == '000') or c.county == '00')
+
+    gvs.ad_map = dict(steam)
+    gvs.ad_tree = fork(gvs.ad_map, depth=0, floor=4)
+
+
+def fork(__steam, depth: int, floor: int):
+    if depth >= floor:
+        return next(__steam)[-1]
+    return {
+        k: fork(v, depth + 1, floor)
+        for k, v in groupby(__steam, lambda item: item[depth])
+    }
```

