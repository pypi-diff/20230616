# Comparing `tmp/nonebot_plugin_pixivbot-2.0.0.tar.gz` & `tmp/nonebot_plugin_pixivbot-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pixivbot-2.0.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_pixivbot-2.0.0a1.tar", max compression
```

## Comparing `nonebot_plugin_pixivbot-2.0.0.tar` & `nonebot_plugin_pixivbot-2.0.0a1.tar`

### file list

```diff
@@ -1,131 +1,131 @@
--rw-r--r--   0        0        0     1064 2023-06-16 15:41:46.675872 nonebot_plugin_pixivbot-2.0.0/LICENSE
--rw-r--r--   0        0        0    16194 2023-06-16 15:41:46.675872 nonebot_plugin_pixivbot-2.0.0/README.md
--rw-r--r--   0        0        0     1135 2023-06-16 15:41:46.675872 nonebot_plugin_pixivbot-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      881 2023-06-16 15:41:46.675872 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/__init__.py
--rw-r--r--   0        0        0     7164 2023-06-16 15:41:46.675872 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/config.py
--rw-r--r--   0        0        0     4262 2023-06-16 15:41:46.675872 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/context.py
--rw-r--r--   0        0        0        0 2023-06-16 15:41:46.675872 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/__init__.py
--rw-r--r--   0        0        0       54 2023-06-16 15:41:46.675872 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/errors.py
--rw-r--r--   0        0        0      891 2023-06-16 15:41:46.675872 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/interval_task_repo.py
--rw-r--r--   0        0        0     2468 2023-06-16 15:41:46.675872 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/local_tag.py
--rw-r--r--   0        0        0      835 2023-06-16 15:41:46.675872 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/nb_session.py
--rw-r--r--   0        0        0     2449 2023-06-16 15:41:46.675872 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_binding.py
--rw-r--r--   0        0        0      253 2023-06-16 15:41:46.675872 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/__init__.py
--rw-r--r--   0        0        0     1482 2023-06-16 15:41:46.675872 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/base.py
--rw-r--r--   0        0        0     1774 2023-06-16 15:41:46.675872 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/compressor.py
--rw-r--r--   0        0        0      336 2023-06-16 15:41:46.675872 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/enums.py
--rw-r--r--   0        0        0      319 2023-06-16 15:41:46.675872 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/errors.py
--rw-r--r--   0        0        0      997 2023-06-16 15:41:46.675872 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/lazy_illust.py
--rw-r--r--   0        0        0      513 2023-06-16 15:41:46.675872 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/__init__.py
--rw-r--r--   0        0        0     2745 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/base.py
--rw-r--r--   0        0        0     3308 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/dummy.py
--rw-r--r--   0        0        0    32537 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql.py
--rw-r--r--   0        0        0     3360 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql_models.py
--rw-r--r--   0        0        0     9764 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator.py
--rw-r--r--   0        0        0    21709 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator_repo.py
--rw-r--r--   0        0        0      319 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/models.py
--rw-r--r--   0        0        0    18411 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/remote_repo.py
--rw-r--r--   0        0        0        0 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/source/__init__.py
--rw-r--r--   0        0        0     1769 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/source/lifecycle_mixin.py
--rw-r--r--   0        0        0     3128 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/source/migration_manager.py
--rw-r--r--   0        0        0     5263 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/source/sql/__init__.py
--rw-r--r--   0        0        0      259 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/source/sql/meta_info.py
--rw-r--r--   0        0        0      507 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/source/sql/migration/__init__.py
--rw-r--r--   0        0        0     3753 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v1_to_v2.py
--rw-r--r--   0        0        0     1736 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v2_to_v3.py
--rw-r--r--   0        0        0      315 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v3_to_v4.py
--rw-r--r--   0        0        0     8376 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v4_to_v5.py
--rw-r--r--   0        0        0     5615 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/subscription.py
--rw-r--r--   0        0        0        0 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/utils/__init__.py
--rw-r--r--   0        0        0      157 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/utils/shortuuid.py
--rw-r--r--   0        0        0      792 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/utils/sql/__init__.py
--rw-r--r--   0        0        0      733 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/utils/sql/utc_datetime.py
--rw-r--r--   0        0        0      703 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/utils/sql.pyi
--rw-r--r--   0        0        0     6319 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/watch_task.py
--rw-r--r--   0        0        0      835 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/enums.py
--rw-r--r--   0        0        0       97 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/global_context.py
--rw-r--r--   0        0        0       88 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/__init__.py
--rw-r--r--   0        0        0     9127 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/base.py
--rw-r--r--   0        0        0      300 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/command/__init__.py
--rw-r--r--   0        0        0     2249 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/command/bind.py
--rw-r--r--   0        0        0     4968 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/command/command.py
--rw-r--r--   0        0        0      471 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/command/help.py
--rw-r--r--   0        0        0      726 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/command/invalidate_cache.py
--rw-r--r--   0        0        0     5244 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/command/schedule.py
--rw-r--r--   0        0        0     5668 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/command/watch.py
--rw-r--r--   0        0        0      620 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/common/__init__.py
--rw-r--r--   0        0        0      668 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/common/base.py
--rw-r--r--   0        0        0     1513 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/common/illust.py
--rw-r--r--   0        0        0     1329 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/common/more.py
--rw-r--r--   0        0        0     2491 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/common/random_bookmark.py
--rw-r--r--   0        0        0     1741 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/common/random_illust.py
--rw-r--r--   0        0        0     1527 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/common/random_recommended_illust.py
--rw-r--r--   0        0        0     1941 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/common/random_related_illust.py
--rw-r--r--   0        0        0     2093 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/common/random_user_illust.py
--rw-r--r--   0        0        0     4069 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/common/ranking.py
--rw-r--r--   0        0        0        0 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/interceptor/__init__.py
--rw-r--r--   0        0        0      478 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/interceptor/base.py
--rw-r--r--   0        0        0     1924 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/interceptor/combined_interceptor.py
--rw-r--r--   0        0        0     1532 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/interceptor/default_error_interceptor.py
--rw-r--r--   0        0        0     1179 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/interceptor/loading_prompt_interceptor.py
--rw-r--r--   0        0        0     1799 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/interceptor/permission_interceptor.py
--rw-r--r--   0        0        0      521 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/interceptor/record_req_interceptor.py
--rw-r--r--   0        0        0      857 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/interceptor/retry_interceptor.py
--rw-r--r--   0        0        0     1613 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/interceptor/service_interceptor.py
--rw-r--r--   0        0        0      588 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/interceptor/timeout_interceptor.py
--rw-r--r--   0        0        0      151 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/pkg_context.py
--rw-r--r--   0        0        0     2538 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/recorder.py
--rw-r--r--   0        0        0      320 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/schedule/__init__.py
--rw-r--r--   0        0        0      340 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/schedule/base.py
--rw-r--r--   0        0        0      448 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/schedule/random_bookmark.py
--rw-r--r--   0        0        0      440 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/schedule/random_illust.py
--rw-r--r--   0        0        0      485 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/schedule/random_recommended_illust.py
--rw-r--r--   0        0        0      457 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/schedule/random_user_illust.py
--rw-r--r--   0        0        0      419 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/schedule/ranking.py
--rw-r--r--   0        0        0       45 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/sniffer/__init__.py
--rw-r--r--   0        0        0     1019 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/sniffer/illust_link.py
--rw-r--r--   0        0        0     1251 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/sniffer/poke.py
--rw-r--r--   0        0        0     1177 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/utils.py
--rw-r--r--   0        0        0      110 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/watch/__init__.py
--rw-r--r--   0        0        0      845 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/watch/base.py
--rw-r--r--   0        0        0     2305 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/watch/following_illusts.py
--rw-r--r--   0        0        0     1716 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/watch/user_illusts.py
--rw-r--r--   0        0        0      384 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/model/__init__.py
--rw-r--r--   0        0        0     1787 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/model/illust.py
--rw-r--r--   0        0        0      150 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/model/interval_task.py
--rw-r--r--   0        0        0      153 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/model/message/__init__.py
--rw-r--r--   0        0        0     2439 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/model/message/illust_message.py
--rw-r--r--   0        0        0     2312 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/model/message/illust_messages.py
--rw-r--r--   0        0        0      122 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/model/pixiv_binding.py
--rw-r--r--   0        0        0     2071 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/model/subscription.py
--rw-r--r--   0        0        0      189 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/model/tag.py
--rw-r--r--   0        0        0      121 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/model/user.py
--rw-r--r--   0        0        0      229 2023-06-16 15:41:46.679873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/model/user_preview.py
--rw-r--r--   0        0        0      895 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/model/watch_task.py
--rw-r--r--   0        0        0      201 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/platform/__init__.py
--rw-r--r--   0        0        0      514 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/platform/available/__init__.py
--rw-r--r--   0        0        0     4242 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/platform/available/kaiheila.py
--rw-r--r--   0        0        0      805 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/platform/available/onebot_v11.py
--rw-r--r--   0        0        0      845 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/platform/func_manager.py
--rw-r--r--   0        0        0     1644 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/plugin_service.py
--rw-r--r--   0        0        0       47 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/service/__init__.py
--rw-r--r--   0        0        0     4372 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/service/interval_task_worker.py
--rw-r--r--   0        0        0      819 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/service/pixiv_account_binder.py
--rw-r--r--   0        0        0     5889 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/service/pixiv_service.py
--rw-r--r--   0        0        0     4497 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/service/postman.py
--rw-r--r--   0        0        0     2158 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/service/roulette.py
--rw-r--r--   0        0        0     7240 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/service/scheduler.py
--rw-r--r--   0        0        0     3089 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/service/watchman.py
--rw-r--r--   0        0        0      771 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/usage.py
--rw-r--r--   0        0        0        0 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/utils/__init__.py
--rw-r--r--   0        0        0      217 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/utils/algorithm.py
--rw-r--r--   0        0        0      252 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/utils/coros.py
--rw-r--r--   0        0        0     1109 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/utils/decode_integer.py
--rw-r--r--   0        0        0      492 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/utils/errors.py
--rw-r--r--   0        0        0     3501 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/utils/expires_lru_dict.py
--rw-r--r--   0        0        0       93 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/utils/format.py
--rw-r--r--   0        0        0      483 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/utils/lazy_delegation.py
--rw-r--r--   0        0        0     4038 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/utils/lifecycler.py
--rw-r--r--   0        0        0      312 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/utils/nonebot.py
--rw-r--r--   0        0        0     8450 2023-06-16 15:41:46.683873 nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/utils/shared_agen.py
--rw-r--r--   0        0        0    17511 1970-01-01 00:00:00.000000 nonebot_plugin_pixivbot-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-02-13 05:42:01.812872 nonebot_plugin_pixivbot-2.0.0a1/LICENSE
+-rw-r--r--   0        0        0     1179 2023-06-15 02:11:03.871897 nonebot_plugin_pixivbot-2.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0    17595 2023-04-27 10:16:31.843054 nonebot_plugin_pixivbot-2.0.0a1/README.md
+-rw-r--r--   0        0        0      915 2023-06-15 01:44:24.090734 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/__init__.py
+-rw-r--r--   0        0        0     7217 2023-06-15 01:44:24.091241 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/config.py
+-rw-r--r--   0        0        0     4411 2023-04-27 10:16:31.872054 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/context.py
+-rw-r--r--   0        0        0        0 2023-06-15 01:44:24.091241 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/__init__.py
+-rw-r--r--   0        0        0       56 2023-02-13 05:42:01.817000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/errors.py
+-rw-r--r--   0        0        0      924 2023-06-15 01:44:24.092249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/interval_task_repo.py
+-rw-r--r--   0        0        0     2541 2023-06-15 01:44:24.092249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/local_tag.py
+-rw-r--r--   0        0        0      858 2023-06-15 01:44:24.092249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/nb_session.py
+-rw-r--r--   0        0        0     2513 2023-06-15 01:44:24.093248 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_binding.py
+-rw-r--r--   0        0        0      262 2023-02-13 05:42:01.821000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/__init__.py
+-rw-r--r--   0        0        0     1524 2023-02-13 05:42:01.822000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/base.py
+-rw-r--r--   0        0        0     1829 2023-04-26 10:41:42.739000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/compressor.py
+-rw-r--r--   0        0        0      355 2023-02-13 05:42:01.822000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/enums.py
+-rw-r--r--   0        0        0      334 2023-02-13 05:42:01.823000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/errors.py
+-rw-r--r--   0        0        0     1036 2023-02-13 05:42:01.823000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/lazy_illust.py
+-rw-r--r--   0        0        0      532 2023-06-15 01:44:24.093248 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/__init__.py
+-rw-r--r--   0        0        0     2823 2023-03-15 03:26:56.195000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/base.py
+-rw-r--r--   0        0        0     3419 2023-04-26 10:41:42.740000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/dummy.py
+-rw-r--r--   0        0        0    33227 2023-06-15 01:44:24.094251 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql.py
+-rw-r--r--   0        0        0     3460 2023-06-15 01:44:24.094251 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql_models.py
+-rw-r--r--   0        0        0     9990 2023-04-26 10:41:42.822000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator.py
+-rw-r--r--   0        0        0    22139 2023-04-26 10:41:42.822000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator_repo.py
+-rw-r--r--   0        0        0      332 2023-04-26 10:41:42.823000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/models.py
+-rw-r--r--   0        0        0    18821 2023-04-27 13:33:43.566000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/remote_repo.py
+-rw-r--r--   0        0        0        0 2023-06-15 01:44:24.095249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/__init__.py
+-rw-r--r--   0        0        0     1815 2023-06-15 01:44:24.095249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/lifecycle_mixin.py
+-rw-r--r--   0        0        0     3211 2023-02-13 05:42:01.830000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/migration_manager.py
+-rw-r--r--   0        0        0     5411 2023-06-15 01:44:24.096249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/sql/__init__.py
+-rw-r--r--   0        0        0      270 2023-06-15 01:44:24.096249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/sql/meta_info.py
+-rw-r--r--   0        0        0      523 2023-06-15 01:44:24.097249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/sql/migration/__init__.py
+-rw-r--r--   0        0        0     3824 2023-02-13 05:42:01.838000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v1_to_v2.py
+-rw-r--r--   0        0        0     1783 2023-06-15 01:44:24.097249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v2_to_v3.py
+-rw-r--r--   0        0        0      327 2023-06-15 01:44:24.098250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v3_to_v4.py
+-rw-r--r--   0        0        0     8662 2023-06-15 01:44:24.098250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v4_to_v5.py
+-rw-r--r--   0        0        0     5554 2023-06-15 01:44:24.099249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/subscription.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.842000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/utils/__init__.py
+-rw-r--r--   0        0        0      164 2023-02-13 05:42:01.842000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/utils/shortuuid.py
+-rw-r--r--   0        0        0      814 2023-02-13 05:42:01.843000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/utils/sql/__init__.py
+-rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/utils/sql/utc_datetime.py
+-rw-r--r--   0        0        0      720 2023-02-13 05:42:01.842000 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/utils/sql.pyi
+-rw-r--r--   0        0        0     6474 2023-06-15 01:44:24.099249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/watch_task.py
+-rw-r--r--   0        0        0      870 2023-06-15 01:44:24.100250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/enums.py
+-rw-r--r--   0        0        0      102 2023-02-14 03:27:31.463009 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/global_context.py
+-rw-r--r--   0        0        0       92 2023-02-13 05:42:01.847870 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/__init__.py
+-rw-r--r--   0        0        0     9360 2023-06-15 01:44:24.100250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/base.py
+-rw-r--r--   0        0        0      308 2023-02-13 05:42:01.847870 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/command/__init__.py
+-rw-r--r--   0        0        0     2318 2023-06-15 01:44:24.101249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/command/bind.py
+-rw-r--r--   0        0        0     2500 2023-06-15 01:44:24.101249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/command/command.py
+-rw-r--r--   0        0        0      369 2023-06-15 01:44:24.102249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/command/help.py
+-rw-r--r--   0        0        0      696 2023-06-15 01:44:24.102249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/command/invalidate_cache.py
+-rw-r--r--   0        0        0     4064 2023-06-15 01:44:24.103249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/command/schedule.py
+-rw-r--r--   0        0        0     1342 2023-06-15 01:44:24.103249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/command/subcommand.py
+-rw-r--r--   0        0        0     5664 2023-06-15 01:44:24.104250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/command/watch.py
+-rw-r--r--   0        0        0      633 2023-02-13 05:42:01.851870 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/__init__.py
+-rw-r--r--   0        0        0      688 2023-03-29 02:34:22.117934 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/base.py
+-rw-r--r--   0        0        0     1560 2023-06-15 01:44:24.104250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/illust.py
+-rw-r--r--   0        0        0     1369 2023-06-15 01:44:24.105250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/more.py
+-rw-r--r--   0        0        0     2558 2023-06-15 01:44:24.105250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/random_bookmark.py
+-rw-r--r--   0        0        0     1790 2023-06-15 01:44:24.106249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/random_illust.py
+-rw-r--r--   0        0        0     1566 2023-06-15 01:44:24.106249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/random_recommended_illust.py
+-rw-r--r--   0        0        0     1992 2023-06-15 01:44:24.107248 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/random_related_illust.py
+-rw-r--r--   0        0        0     2148 2023-06-15 01:44:24.107248 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/random_user_illust.py
+-rw-r--r--   0        0        0     4180 2023-06-15 01:44:24.108251 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/ranking.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.857869 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/__init__.py
+-rw-r--r--   0        0        0      494 2023-06-15 01:44:24.108251 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/base.py
+-rw-r--r--   0        0        0     1982 2023-06-15 01:44:24.109250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/combined_interceptor.py
+-rw-r--r--   0        0        0     1571 2023-06-15 01:44:24.109250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/default_error_interceptor.py
+-rw-r--r--   0        0        0     1218 2023-06-15 01:44:24.110248 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/loading_prompt_interceptor.py
+-rw-r--r--   0        0        0     1855 2023-06-15 01:44:24.110248 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/permission_interceptor.py
+-rw-r--r--   0        0        0      538 2023-06-15 01:44:24.111251 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/record_req_interceptor.py
+-rw-r--r--   0        0        0      887 2023-06-15 01:44:24.111251 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/retry_interceptor.py
+-rw-r--r--   0        0        0     1654 2023-06-15 01:44:24.112250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/service_interceptor.py
+-rw-r--r--   0        0        0      609 2023-06-15 01:44:24.112250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/timeout_interceptor.py
+-rw-r--r--   0        0        0      157 2023-06-15 01:44:24.113251 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/pkg_context.py
+-rw-r--r--   0        0        0     2620 2023-06-15 01:44:24.113251 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/recorder.py
+-rw-r--r--   0        0        0      325 2023-02-14 11:56:02.041347 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/schedule/__init__.py
+-rw-r--r--   0        0        0      349 2023-04-26 11:20:41.850065 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/schedule/base.py
+-rw-r--r--   0        0        0      461 2023-03-29 02:34:22.131121 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/schedule/random_bookmark.py
+-rw-r--r--   0        0        0      453 2023-03-29 02:34:22.131121 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/schedule/random_illust.py
+-rw-r--r--   0        0        0      498 2023-03-29 02:34:22.132122 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/schedule/random_recommended_illust.py
+-rw-r--r--   0        0        0      470 2023-03-29 02:34:22.132122 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/schedule/random_user_illust.py
+-rw-r--r--   0        0        0      432 2023-03-29 02:34:22.133120 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/schedule/ranking.py
+-rw-r--r--   0        0        0       27 2023-02-13 05:42:01.862870 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/sniffer/__init__.py
+-rw-r--r--   0        0        0     1051 2023-06-15 01:44:24.114250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/sniffer/illust_link.py
+-rw-r--r--   0        0        0     1219 2023-06-15 01:44:24.114250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/utils.py
+-rw-r--r--   0        0        0      112 2023-02-14 12:15:47.490983 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/watch/__init__.py
+-rw-r--r--   0        0        0      865 2023-04-26 11:20:41.827066 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/watch/base.py
+-rw-r--r--   0        0        0     2363 2023-06-15 01:44:24.115250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/watch/following_illusts.py
+-rw-r--r--   0        0        0     1759 2023-06-15 01:44:24.116249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/watch/user_illusts.py
+-rw-r--r--   0        0        0      394 2023-06-15 01:44:24.116249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/__init__.py
+-rw-r--r--   0        0        0     1858 2023-04-27 09:18:54.765186 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/illust.py
+-rw-r--r--   0        0        0      157 2023-06-15 01:44:24.117251 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/interval_task.py
+-rw-r--r--   0        0        0      157 2023-02-13 05:42:01.867870 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/message/__init__.py
+-rw-r--r--   0        0        0     2512 2023-06-15 01:44:24.117251 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/message/illust_message.py
+-rw-r--r--   0        0        0     2379 2023-06-15 01:44:24.118248 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/message/illust_messages.py
+-rw-r--r--   0        0        0      129 2023-06-15 01:44:24.118248 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/pixiv_binding.py
+-rw-r--r--   0        0        0     1376 2023-06-15 01:44:24.118248 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/subscription.py
+-rw-r--r--   0        0        0      203 2023-02-13 05:42:01.870869 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/tag.py
+-rw-r--r--   0        0        0      131 2023-02-13 05:42:01.870869 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/user.py
+-rw-r--r--   0        0        0      242 2023-02-13 05:42:01.871622 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/user_preview.py
+-rw-r--r--   0        0        0      930 2023-06-15 01:44:24.119250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/watch_task.py
+-rw-r--r--   0        0        0      208 2023-06-15 01:44:24.119250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/platform/__init__.py
+-rw-r--r--   0        0        0      531 2023-06-15 01:44:24.120252 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/platform/available/__init__.py
+-rw-r--r--   0        0        0     4368 2023-06-15 01:44:24.120252 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/platform/available/kaiheila.py
+-rw-r--r--   0        0        0      826 2023-06-15 01:44:24.121250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/platform/available/onebot_v11.py
+-rw-r--r--   0        0        0      878 2023-06-15 01:44:24.121250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/platform/func_manager.py
+-rw-r--r--   0        0        0     1680 2023-06-14 12:11:02.914517 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/plugin_service.py
+-rw-r--r--   0        0        0       49 2023-02-13 05:42:01.874870 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/__init__.py
+-rw-r--r--   0        0        0     4494 2023-06-15 01:44:24.122249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/interval_task_worker.py
+-rw-r--r--   0        0        0      844 2023-06-15 01:44:24.122249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/pixiv_account_binder.py
+-rw-r--r--   0        0        0     6023 2023-04-26 10:41:42.751891 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/pixiv_service.py
+-rw-r--r--   0        0        0     4506 2023-06-15 02:08:21.682591 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/postman.py
+-rw-r--r--   0        0        0     2244 2023-02-13 05:42:01.877869 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/roulette.py
+-rw-r--r--   0        0        0     5082 2023-06-15 01:44:24.123250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/scheduler.py
+-rw-r--r--   0        0        0     3170 2023-06-15 01:44:24.124250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/watchman.py
+-rw-r--r--   0        0        0      790 2023-06-15 01:44:24.124250 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/usage.py
+-rw-r--r--   0        0        0        0 2023-02-13 05:42:01.878870 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/__init__.py
+-rw-r--r--   0        0        0      230 2023-03-29 02:34:22.138709 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/algorithm.py
+-rw-r--r--   0        0        0      265 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/coros.py
+-rw-r--r--   0        0        0     1148 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/decode_integer.py
+-rw-r--r--   0        0        0      515 2023-02-13 05:42:01.879870 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/errors.py
+-rw-r--r--   0        0        0     3604 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/expires_lru_dict.py
+-rw-r--r--   0        0        0       95 2023-04-26 10:41:42.825893 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/format.py
+-rw-r--r--   0        0        0      494 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/lazy_delegation.py
+-rw-r--r--   0        0        0     4188 2023-02-13 05:42:01.880869 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/lifecycler.py
+-rw-r--r--   0        0        0      324 2023-06-15 01:44:24.125249 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/nonebot.py
+-rw-r--r--   0        0        0     8653 2023-04-27 14:59:21.481094 nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/shared_agen.py
+-rw-r--r--   0        0        0    18550 1970-01-01 00:00:00.000000 nonebot_plugin_pixivbot-2.0.0a1/PKG-INFO
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/README.md` & `nonebot_plugin_pixivbot-2.0.0a1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: nonebot-plugin-pixivbot
+Version: 2.0.0a1
+Summary: Nonebot Plugin PixivBot
+Home-page: https://github.com/ssttkkl/nonebot-plugin-pixivbot
+License: MIT
+Author: ssttkkl
+Author-email: huang.wen.long@hotmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Pillow (>=9.2.0,<10.0.0)
+Requires-Dist: PixivPy-Async (>=1.2.14,<2.0.0)
+Requires-Dist: aiohttp-socks (>=0.8.0,<0.9.0)
+Requires-Dist: asyncache (>=0.3.1,<0.4.0)
+Requires-Dist: cachetools (>=5.2.0,<6.0.0)
+Requires-Dist: frozendict (>=2.3.4,<3.0.0)
+Requires-Dist: lazy (>=1.4,<2.0)
+Requires-Dist: nonebot-plugin-access-control (>=0.5.5)
+Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.7,<0.3.0)
+Requires-Dist: nonebot-plugin-session (>=0.0.4)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
+Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
+Requires-Dist: numpy (>=1.23.1,<2.0.0)
+Requires-Dist: shortuuid (>=1.0.9,<2.0.0)
+Requires-Dist: tzlocal (>=5.0.1,<6.0.0)
+Project-URL: Repository, https://github.com/ssttkkl/nonebot-plugin-pixivbot
+Description-Content-Type: text/markdown
+
 <!-- markdownlint-disable MD033 MD036 MD041 -->
 
 <p align="center">
   <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
 </p>
 
 <div align="center">
@@ -21,14 +53,20 @@
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-pixivbot.svg" alt="pypi">
   </a>
   <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
 </p>
 
 NoneBot插件，支持发送随机Pixiv插画、画师更新推送、定时订阅推送……
 
+适配协议：
+
+- [Onebot V11](https://onebot.adapters.nonebot.dev/)
+- [KOOK / 开黑啦](https://github.com/Tian-que/nonebot-adapter-kaiheila)
+- [Telegram](https://github.com/nonebot/adapter-telegram)
+
 ## 触发语句
 
 ### 普通语句
 
 所有数字参数均支持中文数字和罗马数字。
 
 - **看看<类型>榜<范围>**：查看pixiv榜单（<类型>可省略，<范围>应为a-b或a）
@@ -47,37 +85,39 @@
 - **还要**：重复上一次请求
 - **不够色**：获取上一张插画的相关插画
 
 ### 命令语句
 
 - **/pixivbot schedule \<type\> \<schedule\> [..args]**：为本群（本用户）订阅类型为<type>的定时推送功能，时间满足<schedule>时进行推送
     - \<type\>：可选值有ranking, random_bookmark, random_recommended_illust, random_illust, random_user_illust
-    - \<schedule\>：格式为HH:mm（每日固定时间点推送）或HH:mm*x（间隔时间推送），或者使用cron表达式
+    - \<schedule\>：有三种格式，*00:30\*x*为每隔30分钟进行一次推送，*12:00*为每天12:00进行一次推送，*00:10+00:30\*x*为从今天00:
+      10开始每隔30分钟进行一次推送（开始时间若是一个过去的时间点，则从下一个开始推送的时间点进行推送）
     - [..args]：
-        - \<type\>为ranking时，接受mode、range
-            - 示例：/pixivbot schedle ranking 12:00 --mode day --range 1-10
-        - \<type\>为random_bookmark时，接受user
+        - \<type\>为ranking时，接受\<mode\> \<range\>
+            - 示例：/pixivbot schedle ranking 12:00 day 1-10
+        - \<type\>为random_bookmark时，接受\<pixiv_user_id\>（可空）
             - 示例：/pixivbot schedle random_bookmark 01:00*x
-            - 示例：/pixivbot schedle random_bookmark 01:00*x --user 114514
-        - \<type\>为random_illust时，接受word（必需）
-            - 示例：/pixivbot schedle random_illust "0 */2 * * * *" --word ロリ
-            - 示例：/pixivbot schedle random_illust "0 */2 * * * *" --word "Hatsune Miku"
-        - \<type\>为random_user_illust时，接受user（必需）
-            - 示例：/pixivbot schedle random_user_illust 01:00*x --user 森倉円
+            - 示例：/pixivbot schedle random_bookmark 01:00*x 114514
+        - \<type\>为random_illust时，接受\<word\>，若需要输入空格请用反斜杠`\ `
+            - 示例：/pixivbot schedle random_illust 01:00*x
+            - 示例：/pixivbot schedle random_illust 01:00*x ロリ
+            - 示例：/pixivbot schedle random_illust 01:00*x Hatsune\ Miku
+        - \<type\>为random_user_illust时，接受\<user\>
+            - 示例：/pixivbot schedle random_user_illust 01:00*x 森倉円
         - \<type\>为random_recommend_illust时，不接受参数
 - **/pixivbot schedule**：查看本群（本用户）的所有定时推送订阅
 - **/pixivbot unschedule \<id\>**：取消本群（本用户）的指定的定时推送订阅
 - **/pixivbot watch \<type\> [..args]**：为本群（本用户）订阅类型为<type>的更新推送功能
     - \<type\>：可选值有user_illusts, following_illusts
     - [..args]：
-        - \<type\>为user_illusts时，接受user（必需）
-            - 示例：/pixivbot watch user_illusts --user 森倉円
-        - \<type\>为following_illusts时，接受user
+        - \<type\>为user_illusts时，接受\<user\>
+            - 示例：/pixivbot watch user_illusts 森倉円
+        - \<type\>为following_illusts时，接受\<pixiv_user_id\>（可空）
             - 示例：/pixivbot watch following_illusts
-            - 示例：/pixivbot watch following_illusts --user 114514
+            - 示例：/pixivbot watch following_illusts 114514
 - **/pixivbot watch**：查看本群（本用户）的所有更新推送订阅
 - **/pixivbot watch fetch \<id\>**：【调试用命令】立刻手动触发一次指定的更新推送订阅
 - **/pixivbot unwatch \<id\> [..args]**：取消本群（本用户）的指定的更新推送订阅
 - **/pixivbot bind \<pixiv_user_id\>**：绑定Pixiv账号（用于随机书签功能）
 - **/pixivbot unbind**：解绑Pixiv账号
 - **/pixivbot invalidate_cache**：清除缓存（只有超级用户能够发送此命令）
 - **/pixivbot**、**/pixivbot help**：查看帮助
@@ -106,14 +146,23 @@
 
 若需要使用PostgreSQL，请设置配置项：
 
 - pixiv_sql_conn_url=`postgresql+asyncpg://<用户名>:<密码>@<主机>:<端口>/<数据库名>`
 
 并且安装`nonebot-plugin-pixivbot[postgresql]`
 
+### MongoDB
+
+若需要使用MongoDB，请设置配置项：
+
+- pixiv_mongo_conn_url=`mongodb://<用户名>:<密码>@<主机>:<端口>/<用户所属的数据库>`
+- pixiv_mongo_database_name=`连接的MongoDB数据库`
+
+并且安装`nonebot-plugin-pixivbot[mongo]`
+
 ## 权限控制
 
 插件接入了[nonebot-plugin-access-control](https://github.com/ssttkkl/nonebot-plugin-access-control)实现细粒度的权限控制：
 
 ```
 nonebot_plugin_pixivbot
 ├── common
@@ -196,15 +245,18 @@
 
 除最小配置出现的配置项以外都是可选项，给出的是默认值，建议只将自己需要的项加入.env.prod文件
 
 完整配置：
 
 ```
 # 数据库配置
+pixiv_data_source=  # 使用的数据库类型，可选值：sql，mongo。若未设置，则根据是否设置了pixiv_mongo_conn_url自动判断。
 pixiv_sql_conn_url=sqlite+aiosqlite:///pixiv_bot.db  # SQL连接URL，仅支持SQLite与PostgreSQL（通过SQLAlchemy进行连接，必须使用异步的DBAPI）
+pixiv_mongo_conn_url=  # MongoDB连接URL，格式：mongodb://<用户名>:<密码>@<主机>:<端口>/<数据库>。
+pixiv_mongo_database_name=  # 连接的MongoDB数据库
 pixiv_use_local_cache=True  # 是否启用本地缓存
 
 # 连接配置
 pixiv_refresh_token=  # 前面获取的REFRESH_TOKEN
 pixiv_proxy=  # 代理URL，推荐使用socks5代理
 pixiv_query_timeout=60  # 查询超时（单位：秒）
 pixiv_loading_prompt_delayed_time=5  # 加载提示消息的延迟时间（“努力加载中”的消息会在请求发出多少秒后发出）（单位：秒）
@@ -245,16 +297,16 @@
 pixiv_user_bookmarks_cache_expires_in=86400
 pixiv_user_bookmarks_cache_delete_in=2592000
 pixiv_related_illusts_cache_expires_in=86400
 pixiv_other_cache_expires_in=21600
 
 # QQ平台（主要是gocq）配置
 pixiv_poke_action=random_recommended_illust  # 响应戳一戳动作，可选值：ranking, random_recommended_illust, random_bookmark, 什么都不填即忽略戳一戳动作
-pixiv_send_illust_with_link=False  # 发图时是否带上链接（容易被tx盯上）
-pixiv_send_forward_message=auto  # 发图时是否使用转发消息的形式，可选值：always(永远使用), auto(仅在多张图片时使用), never(永远不使用)
+pixiv_onebot_with_link=False  # 发图时是否带上链接（容易被tx盯上）
+pixiv_onebot_send_forward_message=auto  # 发图时是否使用转发消息的形式，可选值：always(永远使用), auto(仅在多张图片时使用), never(永远不使用)
 
 # 功能配置
 pixiv_more_enabled=True  # 启用重复上一次请求（还要）功能
 pixiv_query_expires_in=600  # 上一次请求的过期时间（单位：秒）
 
 pixiv_illust_query_enabled=True  # 启用插画查询（看看图）功能
 
@@ -338,7 +390,8 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 ```
+
```

#### html2text {}

```diff
@@ -1,12 +1,32 @@
+Metadata-Version: 2.1 Name: nonebot-plugin-pixivbot Version: 2.0.0a1 Summary:
+Nonebot Plugin PixivBot Home-page: https://github.com/ssttkkl/nonebot-plugin-
+pixivbot License: MIT Author: ssttkkl Author-email: huang.wen.long@hotmail.com
+Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: Pillow
+(>=9.2.0,<10.0.0) Requires-Dist: PixivPy-Async (>=1.2.14,<2.0.0) Requires-Dist:
+aiohttp-socks (>=0.8.0,<0.9.0) Requires-Dist: asyncache (>=0.3.1,<0.4.0)
+Requires-Dist: cachetools (>=5.2.0,<6.0.0) Requires-Dist: frozendict
+(>=2.3.4,<3.0.0) Requires-Dist: lazy (>=1.4,<2.0) Requires-Dist: nonebot-
+plugin-access-control (>=0.5.5) Requires-Dist: nonebot-plugin-send-anything-
+anywhere (>=0.2.7,<0.3.0) Requires-Dist: nonebot-plugin-session (>=0.0.4)
+Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Requires-Dist:
+nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist: numpy
+(>=1.23.1,<2.0.0) Requires-Dist: shortuuid (>=1.0.9,<2.0.0) Requires-Dist:
+tzlocal (>=5.0.1,<6.0.0) Project-URL: Repository, https://github.com/ssttkkl/
+nonebot-plugin-pixivbot Description-Content-Type: text/markdown
                                    [nonebot]
                nonebot_plugin_pixivbot ===== _â¨ PixivBot â¨_
                            [license] [pypi] [python]
 NoneBotæä»¶ï¼æ¯æåééæºPixivæç»ãç»å¸æ´æ°æ¨éãå®æ¶è®¢éæ¨éâ¦â¦
-## è§¦åè¯­å¥ ### æ®éè¯­å¥
+ééåè®®ï¼ - [Onebot V11](https://onebot.adapters.nonebot.dev/) - [KOOK /
+å¼é»å¦](https://github.com/Tian-que/nonebot-adapter-kaiheila) - [Telegram]
+(https://github.com/nonebot/adapter-telegram) ## è§¦åè¯­å¥ ### æ®éè¯­å¥
 æææ°å­åæ°åæ¯æä¸­ææ°å­åç½é©¬æ°å­ã -
 **çç<ç±»å>æ¦<èå´>**ï¼æ¥çpixivæ¦åï¼<ç±»å>å¯çç¥ï¼<èå´>åºä¸ºa-
 bæaï¼ - ç¤ºä¾ï¼ççæ¦ãççæ¥æ¦ãççæ¦1-5ãççææ¦ä¸ -
 **æ¥<æ°é>å¼ å¾**ï¼ä»æ¨èæç»éæºæ½éä¸å¼ æç»ï¼<æ°é>å¯çç¥ï¼ä¸åï¼
 - ç¤ºä¾ï¼æ¥å¼ å¾ãæ¥äºå¼ å¾ -
 **æ¥<æ°é>å¼ <å³é®å­>å¾**ï¼æç´¢å³é®å­ï¼ä»æç´¢ç»æéæºæ½éä¸å¼ æç»
 - ç¤ºä¾ï¼æ¥å¼ åé³ãã¯å¾ãæ¥äºå¼ åé³ãã¯å¾ -
@@ -22,39 +42,44 @@
 pixivbot schedule \
 > \
 >
 [..args]**ï¼ä¸ºæ¬ç¾¤ï¼æ¬ç¨æ·ï¼è®¢éç±»åä¸ºçå®æ¶æ¨éåè½ï¼æ¶é´æ»¡è¶³æ¶è¿è¡æ¨é
 - \
 >ï¼å¯éå¼æranking, random_bookmark, random_recommended_illust,
 random_illust, random_user_illust - \
->ï¼æ ¼å¼ä¸ºHH:mmï¼æ¯æ¥åºå®æ¶é´ç¹æ¨éï¼æHH:
-mm*xï¼é´éæ¶é´æ¨éï¼ï¼æèä½¿ç¨cronè¡¨è¾¾å¼ - [..args]ï¼ - \
->ä¸ºrankingæ¶ï¼æ¥åmodeãrange - ç¤ºä¾ï¼/pixivbot schedle ranking 12:00
---mode day --range 1-10 - \
->ä¸ºrandom_bookmarkæ¶ï¼æ¥åuser - ç¤ºä¾ï¼/pixivbot schedle
-random_bookmark 01:00*x - ç¤ºä¾ï¼/pixivbot schedle random_bookmark 01:00*x --
-user 114514 - \
->ä¸ºrandom_illustæ¶ï¼æ¥åwordï¼å¿éï¼ - ç¤ºä¾ï¼/pixivbot schedle
-random_illust "0 */2 * * * *" --word ã­ãª - ç¤ºä¾ï¼/pixivbot schedle
-random_illust "0 */2 * * * *" --word "Hatsune Miku" - \
->ä¸ºrandom_user_illustæ¶ï¼æ¥åuserï¼å¿éï¼ - ç¤ºä¾ï¼/pixivbot schedle
-random_user_illust 01:00*x --user æ£®åå - \
+>ï¼æä¸ç§æ ¼å¼ï¼*00:30\*x*ä¸ºæ¯é30åéè¿è¡ä¸æ¬¡æ¨éï¼*12:
+00*ä¸ºæ¯å¤©12:00è¿è¡ä¸æ¬¡æ¨éï¼*00:10+00:30\*x*ä¸ºä»ä»å¤©00:
+10å¼å§æ¯é30åéè¿è¡ä¸æ¬¡æ¨éï¼å¼å§æ¶é´è¥æ¯ä¸ä¸ªè¿å»çæ¶é´ç¹ï¼åä»ä¸ä¸ä¸ªå¼å§æ¨éçæ¶é´ç¹è¿è¡æ¨éï¼
+- [..args]ï¼ - \
+>ä¸ºrankingæ¶ï¼æ¥å\
+> \
+> - ç¤ºä¾ï¼/pixivbot schedle ranking 12:00 day 1-10 - \
+>ä¸ºrandom_bookmarkæ¶ï¼æ¥å\
+>ï¼å¯ç©ºï¼ - ç¤ºä¾ï¼/pixivbot schedle random_bookmark 01:00*x - ç¤ºä¾ï¼/
+pixivbot schedle random_bookmark 01:00*x 114514 - \
+>ä¸ºrandom_illustæ¶ï¼æ¥å\
+>ï¼è¥éè¦è¾å¥ç©ºæ ¼è¯·ç¨åææ `\ ` - ç¤ºä¾ï¼/pixivbot schedle
+random_illust 01:00*x - ç¤ºä¾ï¼/pixivbot schedle random_illust 01:00*x ã­ãª
+- ç¤ºä¾ï¼/pixivbot schedle random_illust 01:00*x Hatsune\ Miku - \
+>ä¸ºrandom_user_illustæ¶ï¼æ¥å\
+> - ç¤ºä¾ï¼/pixivbot schedle random_user_illust 01:00*x æ£®åå - \
 >ä¸ºrandom_recommend_illustæ¶ï¼ä¸æ¥ååæ° - **/pixivbot
 schedule**ï¼æ¥çæ¬ç¾¤ï¼æ¬ç¨æ·ï¼çææå®æ¶æ¨éè®¢é - **/
 pixivbot unschedule \
 >**ï¼åæ¶æ¬ç¾¤ï¼æ¬ç¨æ·ï¼çæå®çå®æ¶æ¨éè®¢é - **/pixivbot
 watch \
 > [..args]**ï¼ä¸ºæ¬ç¾¤ï¼æ¬ç¨æ·ï¼è®¢éç±»åä¸ºçæ´æ°æ¨éåè½ - \
 >ï¼å¯éå¼æuser_illusts, following_illusts - [..args]ï¼ - \
->ä¸ºuser_illustsæ¶ï¼æ¥åuserï¼å¿éï¼ - ç¤ºä¾ï¼/pixivbot watch
-user_illusts --user æ£®åå - \
->ä¸ºfollowing_illustsæ¶ï¼æ¥åuser - ç¤ºä¾ï¼/pixivbot watch
-following_illusts - ç¤ºä¾ï¼/pixivbot watch following_illusts --user 114514 -
-**/pixivbot watch**ï¼æ¥çæ¬ç¾¤ï¼æ¬ç¨æ·ï¼çæææ´æ°æ¨éè®¢é -
-**/pixivbot watch fetch \
+>ä¸ºuser_illustsæ¶ï¼æ¥å\
+> - ç¤ºä¾ï¼/pixivbot watch user_illusts æ£®åå - \
+>ä¸ºfollowing_illustsæ¶ï¼æ¥å\
+>ï¼å¯ç©ºï¼ - ç¤ºä¾ï¼/pixivbot watch following_illusts - ç¤ºä¾ï¼/pixivbot
+watch following_illusts 114514 - **/pixivbot
+watch**ï¼æ¥çæ¬ç¾¤ï¼æ¬ç¨æ·ï¼çæææ´æ°æ¨éè®¢é - **/pixivbot
+watch fetch \
 >**ï¼ãè°è¯ç¨å½ä»¤ãç«å»æå¨è§¦åä¸æ¬¡æå®çæ´æ°æ¨éè®¢é
 - **/pixivbot unwatch \
 > [..args]**ï¼åæ¶æ¬ç¾¤ï¼æ¬ç¨æ·ï¼çæå®çæ´æ°æ¨éè®¢é - **/
 pixivbot bind \
 >**ï¼ç»å®Pixivè´¦å·ï¼ç¨äºéæºä¹¦ç­¾åè½ï¼ - **/pixivbot
 unbind**ï¼è§£ç»Pixivè´¦å· - **/pixivbot
 invalidate_cache**ï¼æ¸é¤ç¼å­ï¼åªæè¶çº§ç¨æ·è½å¤åéæ­¤å½ä»¤ï¼
@@ -71,29 +96,34 @@
 éç½®å¤é¨æ°æ®åºï¼å¯éï¼
 PixivBotéè¦ä½¿ç¨æ°æ®åºå­æ¾è®¢éä»¥åç¼å­ï¼é»è®¤ä½¿ç¨SQLiteã
 ### SQLite
 è¥éè¦èªå®ä¹SQLiteæ°æ®åºæä»¶è·¯å¾ï¼è¯·è®¾ç½®éç½®é¡¹ï¼ -
 pixiv_sql_conn_url=`sqlite+aiosqlite:///<æ°æ®åºæä»¶è·¯å¾>` ### PostgreSQL
 è¥éè¦ä½¿ç¨PostgreSQLï¼è¯·è®¾ç½®éç½®é¡¹ï¼ -
 pixiv_sql_conn_url=`postgresql+asyncpg://<ç¨æ·å>:<å¯ç >@<ä¸»æº>:
-<ç«¯å£>/<æ°æ®åºå>` å¹¶ä¸å®è£`nonebot-plugin-pixivbot[postgresql]` ##
-æéæ§å¶ æä»¶æ¥å¥äº[nonebot-plugin-access-control](https://github.com/
-ssttkkl/nonebot-plugin-access-control)å®ç°ç»ç²åº¦çæéæ§å¶ï¼ ```
-nonebot_plugin_pixivbot âââ common â âââ illust ï¼ççå¾ï¼
-â âââ ranking ï¼ççæ¦ï¼ â âââ more ï¼è¿è¦ï¼ â
-âââ random_bookmark ï¼æ¥å¼ ç§å®¶è½¦ï¼ â âââ random_illust
-ï¼æ¥å¼ xxå¾ï¼ â âââ random_recommended_illust ï¼æ¥å¼ å¾ï¼ â
-âââ random_related_illust ï¼ä¸å¤è²ï¼ â âââ
-random_user_illust ï¼æ¥å¼ xxèå¸çå¾ï¼ âââ illust_link
-ï¼Pç«é¾æ¥åæ¢ï¼ âââ schedule â âââ receive
-ï¼æ¥æ¶å®æ¶æ¨éï¼ â âââ manage ï¼ç®¡çå®æ¶æ¨éï¼
-âââ watch â âââ receive ï¼æ¥æ¶æ´æ°æ¨éï¼ â âââ
-manage ï¼ç®¡çå®æ¶æ¨éï¼ âââ invalidate_cache ï¼æ¸é¤ç¼å­ï¼
-âââ bind ï¼ç»å®Pç«è´¦å·ï¼ âââ help ï¼å¸®å©ææ¬ï¼
-âââ r18 ï¼æ¾ç¤ºR-18åå®¹ï¼ âââ g ï¼æ¾ç¤ºR-18Gåå®¹ï¼ ```
+<ç«¯å£>/<æ°æ®åºå>` å¹¶ä¸å®è£`nonebot-plugin-pixivbot[postgresql]` ###
+MongoDB è¥éè¦ä½¿ç¨MongoDBï¼è¯·è®¾ç½®éç½®é¡¹ï¼ -
+pixiv_mongo_conn_url=`mongodb://<ç¨æ·å>:<å¯ç >@<ä¸»æº>:<ç«¯å£>/
+<ç¨æ·æå±çæ°æ®åº>` -
+pixiv_mongo_database_name=`è¿æ¥çMongoDBæ°æ®åº` å¹¶ä¸å®è£`nonebot-
+plugin-pixivbot[mongo]` ## æéæ§å¶ æä»¶æ¥å¥äº[nonebot-plugin-access-
+control](https://github.com/ssttkkl/nonebot-plugin-access-
+control)å®ç°ç»ç²åº¦çæéæ§å¶ï¼ ``` nonebot_plugin_pixivbot âââ
+common â âââ illust ï¼ççå¾ï¼ â âââ ranking
+ï¼ççæ¦ï¼ â âââ more ï¼è¿è¦ï¼ â âââ random_bookmark
+ï¼æ¥å¼ ç§å®¶è½¦ï¼ â âââ random_illust ï¼æ¥å¼ xxå¾ï¼ â
+âââ random_recommended_illust ï¼æ¥å¼ å¾ï¼ â âââ
+random_related_illust ï¼ä¸å¤è²ï¼ â âââ random_user_illust
+ï¼æ¥å¼ xxèå¸çå¾ï¼ âââ illust_link ï¼Pç«é¾æ¥åæ¢ï¼
+âââ schedule â âââ receive ï¼æ¥æ¶å®æ¶æ¨éï¼ â âââ
+manage ï¼ç®¡çå®æ¶æ¨éï¼ âââ watch â âââ receive
+ï¼æ¥æ¶æ´æ°æ¨éï¼ â âââ manage ï¼ç®¡çå®æ¶æ¨éï¼
+âââ invalidate_cache ï¼æ¸é¤ç¼å­ï¼ âââ bind
+ï¼ç»å®Pç«è´¦å·ï¼ âââ help ï¼å¸®å©ææ¬ï¼ âââ r18
+ï¼æ¾ç¤ºR-18åå®¹ï¼ âââ g ï¼æ¾ç¤ºR-18Gåå®¹ï¼ ```
 è­¬å¦ï¼è¶çº§ç¨æ·å¯ä»¥éè¿åé`/ac permission deny --srv
 nonebot_plugin_pixivbot.r18 --sbj all`å¨å±æ¦æªR-18ã
 åè­¬å¦ï¼è¶çº§ç¨æ·å¯ä»¥éè¿åå«åéä»¥ä¸æä»¤ï¼ä½¿å¾åªæè¶çº§ç¨æ·ãQQç§èä¸QQç¾¤èçç¾¤ç®¡çè½å¤è°ç¨`/
 pixivbot schedule`ä¸`/pixivbot unschedule`å½ä»¤ã ``` /ac permission deny --
 srv nonebot_plugin_pixivbot.schedule.manage --sbj all /ac permission allow --
 srv nonebot_plugin_pixivbot.schedule.manage --sbj qq:private /ac permission
 allow --srv nonebot_plugin_pixivbot.schedule.manage --sbj qq:group_admin /ac
@@ -118,20 +148,23 @@
 ### åé¨éè¯¯ï¼
 sqlalchemy.exc.OperationalError'>(sqlite3.OperationalError) near "ON": syntax
 error å¤åæ¯SQLiteçæ¬è¿ä½ï¼ä¸æ¯æON
 CONFLICTå­å¥ï¼å¦ææ¯Linuxç³»ç»è¯·æ´æ°å®è£çSQLiteçæ¬ ##
 éç½®é¡¹ä¸è§ æå°éç½®ï¼ ``` pixiv_refresh_token= #
 åé¢è·åçREFRESH_TOKEN ```
 é¤æå°éç½®åºç°çéç½®é¡¹ä»¥å¤é½æ¯å¯éé¡¹ï¼ç»åºçæ¯é»è®¤å¼ï¼å»ºè®®åªå°èªå·±éè¦çé¡¹å å¥.env.prodæä»¶
-å®æ´éç½®ï¼ ``` # æ°æ®åºéç½® pixiv_sql_conn_url=sqlite+aiosqlite:///
-pixiv_bot.db #
+å®æ´éç½®ï¼ ``` # æ°æ®åºéç½® pixiv_data_source= #
+ä½¿ç¨çæ°æ®åºç±»åï¼å¯éå¼ï¼sqlï¼mongoãè¥æªè®¾ç½®ï¼åæ ¹æ®æ¯å¦è®¾ç½®äºpixiv_mongo_conn_urlèªå¨å¤æ­ã
+pixiv_sql_conn_url=sqlite+aiosqlite:///pixiv_bot.db #
 SQLè¿æ¥URLï¼ä»æ¯æSQLiteä¸PostgreSQLï¼éè¿SQLAlchemyè¿è¡è¿æ¥ï¼å¿é¡»ä½¿ç¨å¼æ­¥çDBAPIï¼
-pixiv_use_local_cache=True # æ¯å¦å¯ç¨æ¬å°ç¼å­ # è¿æ¥éç½®
-pixiv_refresh_token= # åé¢è·åçREFRESH_TOKEN pixiv_proxy= #
-ä»£çURLï¼æ¨èä½¿ç¨socks5ä»£ç pixiv_query_timeout=60 #
+pixiv_mongo_conn_url= # MongoDBè¿æ¥URLï¼æ ¼å¼ï¼mongodb://<ç¨æ·å>:
+<å¯ç >@<ä¸»æº>:<ç«¯å£>/<æ°æ®åº>ã pixiv_mongo_database_name= #
+è¿æ¥çMongoDBæ°æ®åº pixiv_use_local_cache=True # æ¯å¦å¯ç¨æ¬å°ç¼å­
+# è¿æ¥éç½® pixiv_refresh_token= # åé¢è·åçREFRESH_TOKEN pixiv_proxy=
+# ä»£çURLï¼æ¨èä½¿ç¨socks5ä»£ç pixiv_query_timeout=60 #
 æ¥è¯¢è¶æ¶ï¼åä½ï¼ç§ï¼ pixiv_loading_prompt_delayed_time=5 #
 å è½½æç¤ºæ¶æ¯çå»¶è¿æ¶é´ï¼âåªåå è½½ä¸­âçæ¶æ¯ä¼å¨è¯·æ±ååºå¤å°ç§åååºï¼ï¼åä½ï¼ç§ï¼
 pixiv_simultaneous_query=8 # åPixivæ¥è¯¢çå¹¶åæ°
 pixiv_download_custom_domain= # ä½¿ç¨ååä»£çä¸è½½æç»çåå #
 æ¥è¯¢è®¾ç½® pixiv_query_to_me_only=False # åªååºå³äºBotçæ¥è¯¢
 pixiv_command_to_me_only=False # åªååºå³äºBotçå½ä»¤
 pixiv_max_item_per_query=10 # æ¯ä¸ªæ¥è¯¢æå¤è¯·æ±çæç»æ°é
@@ -159,17 +192,17 @@
 pixiv_user_illusts_cache_delete_in=2592000
 pixiv_user_bookmarks_cache_expires_in=86400
 pixiv_user_bookmarks_cache_delete_in=2592000
 pixiv_related_illusts_cache_expires_in=86400 pixiv_other_cache_expires_in=21600
 # QQå¹³å°ï¼ä¸»è¦æ¯gocqï¼éç½® pixiv_poke_action=random_recommended_illust
 # ååºæ³ä¸æ³å¨ä½ï¼å¯éå¼ï¼ranking, random_recommended_illust,
 random_bookmark, ä»ä¹é½ä¸å¡«å³å¿½ç¥æ³ä¸æ³å¨ä½
-pixiv_send_illust_with_link=False #
+pixiv_onebot_with_link=False #
 åå¾æ¶æ¯å¦å¸¦ä¸é¾æ¥ï¼å®¹æè¢«txç¯ä¸ï¼
-pixiv_send_forward_message=auto #
+pixiv_onebot_send_forward_message=auto #
 åå¾æ¶æ¯å¦ä½¿ç¨è½¬åæ¶æ¯çå½¢å¼ï¼å¯éå¼ï¼always(æ°¸è¿ä½¿ç¨),
 auto(ä»å¨å¤å¼ å¾çæ¶ä½¿ç¨), never(æ°¸è¿ä¸ä½¿ç¨) # åè½éç½®
 pixiv_more_enabled=True # å¯ç¨éå¤ä¸ä¸æ¬¡è¯·æ±ï¼è¿è¦ï¼åè½
 pixiv_query_expires_in=600 # ä¸ä¸æ¬¡è¯·æ±çè¿ææ¶é´ï¼åä½ï¼ç§ï¼
 pixiv_illust_query_enabled=True # å¯ç¨æç»æ¥è¯¢ï¼ççå¾ï¼åè½
 pixiv_ranking_query_enabled=True # å¯ç¨æ¦åæ¥è¯¢ï¼ççæ¦ï¼åè½
 pixiv_ranking_default_mode=day # é»è®¤æ¥è¯¢çæ¦åï¼å¯éå¼ï¼day, week,
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/__init__.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/__init__.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-"""
-nonebot-plugin-pixivbot
-
-@Author         : ssttkkl
-@License        : MIT
-@GitHub         : https://github.com/ssttkkl/nonebot-plugin-pixivbot
-"""
-from nonebot.plugin import PluginMetadata
-
-from .config import Config
-from .usage import usage
-
-__plugin_meta__ = PluginMetadata(
-    name='PixivBot',
-    description='发送随机Pixiv插画、画师更新推送、定时订阅推送……',
-    usage=usage,
-    type="application",
-    homepage="https://github.com/ssttkkl/nonebot-plugin-pixivbot",
-    config=Config,
-)
-
-# =========== require dependency ============
-from nonebot import require
-
-require("nonebot_plugin_apscheduler")
-require("nonebot_plugin_access_control")
-require("nonebot_plugin_session")
-require("nonebot_plugin_saa")
-
-# =========== register handler & service ============
-from . import service
-from . import handler
-
-__all__ = ("context", "__plugin_meta__")
+"""
+nonebot-plugin-pixivbot
+
+@Author         : ssttkkl
+@License        : MIT
+@GitHub         : https://github.com/ssttkkl/nonebot-plugin-pixivbot
+"""
+from nonebot.plugin import PluginMetadata
+
+from .config import Config
+from .usage import usage
+
+__plugin_meta__ = PluginMetadata(
+    name='PixivBot',
+    description='发送随机Pixiv插画、画师更新推送、定时订阅推送……',
+    usage=usage,
+    type="application",
+    homepage="https://github.com/ssttkkl/nonebot-plugin-pixivbot",
+    config=Config,
+)
+
+# =========== require dependency ============
+from nonebot import require
+
+require("nonebot_plugin_apscheduler")
+require("nonebot_plugin_access_control")
+require("nonebot_plugin_session")
+require("nonebot_plugin_saa")
+
+# =========== register handler & service ============
+from . import service
+from . import handler
+
+__all__ = ("context", "__plugin_meta__")
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/config.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,190 +1,187 @@
-from pathlib import Path
-from typing import Optional, List, Literal
-from urllib.parse import urlparse
-
-from nonebot import get_driver, logger, require
-from pydantic import BaseSettings, validator, root_validator
-from pydantic.fields import ModelField
-
-require("nonebot_plugin_localstore")
-
-import nonebot_plugin_localstore as store
-
-from .enums import *
-from .global_context import context
-
-
-def _get_default_sql_conn_url():
-    # 旧版本的sqlite数据库在working directory
-    data_file = Path("pixiv_bot.db")
-    if not data_file.exists():
-        data_file = store.get_data_file("nonebot_plugin_pixivbot", "pixiv_bot.db")
-
-    return "sqlite+aiosqlite:///" + str(data_file)
-
-
-@context.register_singleton(**get_driver().config.dict())
-class Config(BaseSettings):
-    @root_validator(pre=True, allow_reuse=True)
-    def deprecated_access_control_config(cls, values):
-        for name in {"blacklist", "pixiv_query_cooldown", "pixiv_no_query_cooldown_users"}:
-            if name in values:
-                logger.warning(f"config \"{name}\" is deprecated, use nonebot-plugin-access-control instead "
-                               "(MORE INFO: https://github.com/ssttkkl/nonebot-plugin-pixivbot#%E6%9D%83%E9%99%90%E6%8E%A7%E5%88%B6)")
-        return values
-
-    @root_validator(pre=True, allow_reuse=True)
-    def deprecated_mongodb_config(cls, values):
-        if values.get("pixiv_data_source", "sql") == "mongo" or "pixiv_mongo_conn_url" in values:
-            logger.warning("mongo support was removed, use sql instead")
-        return values
-
-    pixiv_refresh_token: str
-
-    pixiv_sql_conn_url: str
-    pixiv_sql_dialect: str
-    pixiv_use_local_cache: bool = True
-
-    @root_validator(pre=True, allow_reuse=True)
-    def default_sql_conn_url(cls, values):
-        if "pixiv_sql_conn_url" not in values:
-            values["pixiv_sql_conn_url"] = _get_default_sql_conn_url()
-        return values
-
-    @root_validator(pre=True, allow_reuse=True)
-    def detect_sql_dialect(cls, values):
-        values["pixiv_mongo_conn_url"] = ""
-        values["pixiv_mongo_database_name"] = ""
-
-        url = urlparse(values["pixiv_sql_conn_url"])
-        if '+' in url.scheme:
-            pixiv_sql_dialect = url.scheme.split('+')[0]
-        else:
-            pixiv_sql_dialect = url.scheme
-        values["pixiv_sql_dialect"] = pixiv_sql_dialect
-
-        return values
-
-    pixiv_proxy: Optional[str]
-    pixiv_query_timeout: float = 60.0
-    pixiv_loading_prompt_delayed_time: float = 5.0
-    pixiv_simultaneous_query: int = 8
-
-    pixiv_download_cache_expires_in = 3600 * 24 * 7
-    pixiv_illust_detail_cache_expires_in = 3600 * 24 * 7
-    pixiv_user_detail_cache_expires_in = 3600 * 24 * 7
-    pixiv_illust_ranking_cache_expires_in = 3600 * 6
-    pixiv_search_illust_cache_expires_in = 3600 * 24
-    pixiv_search_illust_cache_delete_in = 3600 * 24 * 30
-    pixiv_search_user_cache_expires_in = 3600 * 24
-    pixiv_search_user_cache_delete_in = 3600 * 24 * 30
-    pixiv_user_illusts_cache_expires_in = 3600 * 24
-    pixiv_user_illusts_cache_delete_in = 3600 * 24 * 30
-    pixiv_user_bookmarks_cache_expires_in = 3600 * 24
-    pixiv_user_bookmarks_cache_delete_in = 3600 * 24 * 30
-    pixiv_related_illusts_cache_expires_in = 3600 * 24
-    pixiv_other_cache_expires_in = 3600 * 6
-
-    pixiv_block_tags: List[str] = []
-    pixiv_block_action: BlockAction = BlockAction.no_image
-
-    pixiv_exclude_ai_illusts: bool = False
-
-    pixiv_download_custom_domain: Optional[str]
-
-    pixiv_compression_enabled: bool = False
-    pixiv_compression_max_size: Optional[int]
-    pixiv_compression_quantity: Optional[float]
-
-    # 不加allow_reuse跑pytest会报错
-    @validator('pixiv_compression_max_size', 'pixiv_compression_quantity', allow_reuse=True)
-    def compression_validator(cls, v, values, field: ModelField):
-        if values['pixiv_compression_enabled'] and v is None:
-            raise ValueError(
-                f'pixiv_compression_enabled is True but {field.name} got None.')
-        return v
-
-    pixiv_query_to_me_only = False
-    pixiv_command_to_me_only = False
-
-    pixiv_poke_action: Literal[
-        "", "ranking", "random_recommended_illust", "random_bookmark"] = "random_recommended_illust"
-
-    pixiv_send_illust_link: bool = False
-    pixiv_send_forward_message: Literal['always', 'auto', 'never'] = 'auto'
-
-    pixiv_max_item_per_query = 10
-
-    pixiv_tag_translation_enabled = True
-
-    pixiv_more_enabled = True
-    pixiv_query_expires_in = 10 * 60
-
-    pixiv_illust_query_enabled = True
-    pixiv_illust_sniffer_enabled = True
-
-    pixiv_ranking_query_enabled = True
-    pixiv_ranking_default_mode: RankingMode = RankingMode.day
-    pixiv_ranking_default_range = [1, 3]
-    pixiv_ranking_fetch_item = 150
-    pixiv_ranking_max_item_per_query = 10
-
-    @validator('pixiv_ranking_default_range', allow_reuse=True)
-    def ranking_default_range_validator(cls, v, field: ModelField):
-        if len(v) < 2 or v[0] > v[1]:
-            raise ValueError(f'illegal {field.name} value: {v}')
-        return v
-
-    pixiv_random_illust_query_enabled = True
-    pixiv_random_illust_method = RandomIllustMethod.bookmark_proportion
-    pixiv_random_illust_min_bookmark = 0
-    pixiv_random_illust_min_view = 0
-    pixiv_random_illust_max_page = 20
-    pixiv_random_illust_max_item = 500
-
-    pixiv_random_recommended_illust_query_enabled = True
-    pixiv_random_recommended_illust_method = RandomIllustMethod.uniform
-    pixiv_random_recommended_illust_min_bookmark = 0
-    pixiv_random_recommended_illust_min_view = 0
-    pixiv_random_recommended_illust_max_page = 40
-    pixiv_random_recommended_illust_max_item = 1000
-
-    pixiv_random_related_illust_query_enabled = True
-    pixiv_random_related_illust_method = RandomIllustMethod.bookmark_proportion
-    pixiv_random_related_illust_min_bookmark = 0
-    pixiv_random_related_illust_min_view = 0
-    pixiv_random_related_illust_max_page = 4
-    pixiv_random_related_illust_max_item = 100
-
-    pixiv_random_user_illust_query_enabled = True
-    pixiv_random_user_illust_method = RandomIllustMethod.timedelta_proportion
-    pixiv_random_user_illust_min_bookmark = 0
-    pixiv_random_user_illust_min_view = 0
-    pixiv_random_user_illust_max_page = 2 ** 31
-    pixiv_random_user_illust_max_item = 2 ** 31
-
-    pixiv_random_bookmark_query_enabled = True
-    pixiv_random_bookmark_user_id: Optional[int] = None
-    pixiv_random_bookmark_method = RandomIllustMethod.uniform
-    pixiv_random_bookmark_min_bookmark = 0
-    pixiv_random_bookmark_min_view = 0
-    pixiv_random_bookmark_max_page = 2 ** 31
-    pixiv_random_bookmark_max_item = 2 ** 31
-
-    pixiv_random_following_illust_query_enabled = True
-    pixiv_random_following_illust_method = RandomIllustMethod.timedelta_proportion
-    pixiv_random_following_illust_min_bookmark = 0
-    pixiv_random_following_illust_min_view = 0
-    pixiv_random_following_illust_max_page = 2 ** 31
-    pixiv_random_following_illust_max_item = 2 ** 31
-
-    pixiv_watch_interval = 600
-
-    access_control_reply_on_permission_denied: Optional[str]
-    access_control_reply_on_rate_limited: Optional[str]
-
-    class Config:
-        extra = "ignore"
-
-
-__all__ = ("Config",)
+from pathlib import Path
+from typing import Optional, List, Literal
+from urllib.parse import urlparse
+
+from nonebot import get_driver, logger, require
+from pydantic import BaseSettings, validator, root_validator
+from pydantic.fields import ModelField
+
+require("nonebot_plugin_localstore")
+
+import nonebot_plugin_localstore as store
+
+from .enums import *
+from .global_context import context
+
+
+def _get_default_sql_conn_url():
+    # 旧版本的sqlite数据库在working directory
+    data_file = Path("pixiv_bot.db")
+    if not data_file.exists():
+        data_file = store.get_data_file("nonebot_plugin_pixivbot", "pixiv_bot.db")
+
+    return "sqlite+aiosqlite:///" + str(data_file)
+
+
+@context.register_singleton(**get_driver().config.dict())
+class Config(BaseSettings):
+    @root_validator(pre=True, allow_reuse=True)
+    def deprecated_access_control_config(cls, values):
+        for name in {"blacklist", "pixiv_query_cooldown", "pixiv_no_query_cooldown_users"}:
+            if name in values:
+                logger.warning(f"config \"{name}\" is deprecated, use nonebot-plugin-access-control instead "
+                               "(MORE INFO: https://github.com/ssttkkl/nonebot-plugin-pixivbot#%E6%9D%83%E9%99%90%E6%8E%A7%E5%88%B6)")
+        return values
+
+    @root_validator(pre=True, allow_reuse=True)
+    def deprecated_mongodb_config(cls, values):
+        if values.get("pixiv_data_source", "sql") == "mongo" or "pixiv_mongo_conn_url" in values:
+            logger.warning("mongo support was removed, use sql instead")
+        return values
+
+    pixiv_refresh_token: str
+
+    pixiv_sql_conn_url: str
+    pixiv_sql_dialect: str
+    pixiv_use_local_cache: bool = True
+
+    @root_validator(pre=True, allow_reuse=True)
+    def default_sql_conn_url(cls, values):
+        if "pixiv_sql_conn_url" not in values:
+            values["pixiv_sql_conn_url"] = _get_default_sql_conn_url()
+        return values
+
+    @root_validator(pre=True, allow_reuse=True)
+    def detect_sql_dialect(cls, values):
+        values["pixiv_mongo_conn_url"] = ""
+        values["pixiv_mongo_database_name"] = ""
+
+        url = urlparse(values["pixiv_sql_conn_url"])
+        if '+' in url.scheme:
+            pixiv_sql_dialect = url.scheme.split('+')[0]
+        else:
+            pixiv_sql_dialect = url.scheme
+        values["pixiv_sql_dialect"] = pixiv_sql_dialect
+
+        return values
+
+    pixiv_proxy: Optional[str]
+    pixiv_query_timeout: float = 60.0
+    pixiv_loading_prompt_delayed_time: float = 5.0
+    pixiv_simultaneous_query: int = 8
+
+    pixiv_download_cache_expires_in = 3600 * 24 * 7
+    pixiv_illust_detail_cache_expires_in = 3600 * 24 * 7
+    pixiv_user_detail_cache_expires_in = 3600 * 24 * 7
+    pixiv_illust_ranking_cache_expires_in = 3600 * 6
+    pixiv_search_illust_cache_expires_in = 3600 * 24
+    pixiv_search_illust_cache_delete_in = 3600 * 24 * 30
+    pixiv_search_user_cache_expires_in = 3600 * 24
+    pixiv_search_user_cache_delete_in = 3600 * 24 * 30
+    pixiv_user_illusts_cache_expires_in = 3600 * 24
+    pixiv_user_illusts_cache_delete_in = 3600 * 24 * 30
+    pixiv_user_bookmarks_cache_expires_in = 3600 * 24
+    pixiv_user_bookmarks_cache_delete_in = 3600 * 24 * 30
+    pixiv_related_illusts_cache_expires_in = 3600 * 24
+    pixiv_other_cache_expires_in = 3600 * 6
+
+    pixiv_block_tags: List[str] = []
+    pixiv_block_action: BlockAction = BlockAction.no_image
+
+    pixiv_exclude_ai_illusts: bool = False
+
+    pixiv_download_custom_domain: Optional[str]
+
+    pixiv_compression_enabled: bool = False
+    pixiv_compression_max_size: Optional[int]
+    pixiv_compression_quantity: Optional[float]
+
+    # 不加allow_reuse跑pytest会报错
+    @validator('pixiv_compression_max_size', 'pixiv_compression_quantity', allow_reuse=True)
+    def compression_validator(cls, v, values, field: ModelField):
+        if values['pixiv_compression_enabled'] and v is None:
+            raise ValueError(
+                f'pixiv_compression_enabled is True but {field.name} got None.')
+        return v
+
+    pixiv_query_to_me_only = False
+    pixiv_command_to_me_only = False
+
+    pixiv_send_illust_link: bool = False
+    pixiv_send_forward_message: Literal['always', 'auto', 'never'] = 'auto'
+
+    pixiv_max_item_per_query = 10
+
+    pixiv_tag_translation_enabled = True
+
+    pixiv_more_enabled = True
+    pixiv_query_expires_in = 10 * 60
+
+    pixiv_illust_query_enabled = True
+    pixiv_illust_sniffer_enabled = True
+
+    pixiv_ranking_query_enabled = True
+    pixiv_ranking_default_mode: RankingMode = RankingMode.day
+    pixiv_ranking_default_range = [1, 3]
+    pixiv_ranking_fetch_item = 150
+    pixiv_ranking_max_item_per_query = 10
+
+    @validator('pixiv_ranking_default_range', allow_reuse=True)
+    def ranking_default_range_validator(cls, v, field: ModelField):
+        if len(v) < 2 or v[0] > v[1]:
+            raise ValueError(f'illegal {field.name} value: {v}')
+        return v
+
+    pixiv_random_illust_query_enabled = True
+    pixiv_random_illust_method = RandomIllustMethod.bookmark_proportion
+    pixiv_random_illust_min_bookmark = 0
+    pixiv_random_illust_min_view = 0
+    pixiv_random_illust_max_page = 20
+    pixiv_random_illust_max_item = 500
+
+    pixiv_random_recommended_illust_query_enabled = True
+    pixiv_random_recommended_illust_method = RandomIllustMethod.uniform
+    pixiv_random_recommended_illust_min_bookmark = 0
+    pixiv_random_recommended_illust_min_view = 0
+    pixiv_random_recommended_illust_max_page = 40
+    pixiv_random_recommended_illust_max_item = 1000
+
+    pixiv_random_related_illust_query_enabled = True
+    pixiv_random_related_illust_method = RandomIllustMethod.bookmark_proportion
+    pixiv_random_related_illust_min_bookmark = 0
+    pixiv_random_related_illust_min_view = 0
+    pixiv_random_related_illust_max_page = 4
+    pixiv_random_related_illust_max_item = 100
+
+    pixiv_random_user_illust_query_enabled = True
+    pixiv_random_user_illust_method = RandomIllustMethod.timedelta_proportion
+    pixiv_random_user_illust_min_bookmark = 0
+    pixiv_random_user_illust_min_view = 0
+    pixiv_random_user_illust_max_page = 2 ** 31
+    pixiv_random_user_illust_max_item = 2 ** 31
+
+    pixiv_random_bookmark_query_enabled = True
+    pixiv_random_bookmark_user_id: Optional[int] = None
+    pixiv_random_bookmark_method = RandomIllustMethod.uniform
+    pixiv_random_bookmark_min_bookmark = 0
+    pixiv_random_bookmark_min_view = 0
+    pixiv_random_bookmark_max_page = 2 ** 31
+    pixiv_random_bookmark_max_item = 2 ** 31
+
+    pixiv_random_following_illust_query_enabled = True
+    pixiv_random_following_illust_method = RandomIllustMethod.timedelta_proportion
+    pixiv_random_following_illust_min_bookmark = 0
+    pixiv_random_following_illust_min_view = 0
+    pixiv_random_following_illust_max_page = 2 ** 31
+    pixiv_random_following_illust_max_item = 2 ** 31
+
+    pixiv_watch_interval = 600
+
+    access_control_reply_on_permission_denied: Optional[str]
+    access_control_reply_on_rate_limited: Optional[str]
+
+    class Config:
+        extra = "ignore"
+
+
+__all__ = ("Config",)
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/context.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/context.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,149 +1,149 @@
-from abc import ABC, abstractmethod
-from typing import TypeVar, Type, Callable, Union, Generic, Dict
-
-from nonebot.log import logger
-
-T = TypeVar("T")
-T2 = TypeVar("T2")
-
-
-class Provider(ABC, Generic[T]):
-    @abstractmethod
-    def provide(self) -> T:
-        raise NotImplementedError()
-
-
-class InstanceProvider(Provider[T], Generic[T]):
-    def __init__(self, instance: T):
-        self._instance = instance
-
-    def provide(self) -> T:
-        return self._instance
-
-
-class DynamicProvider(Provider[T], Generic[T]):
-    def __init__(self, func: Callable[[], T], use_cache: bool = True):
-        self._func = func
-        self._use_cache = use_cache
-
-        self._cache = None
-        self._cached = False
-
-    def provide(self) -> T:
-        if not self._use_cache:
-            return self._func()
-
-        if not self._cached:
-            self._cache = self._func()  # just let it throw
-            self._cached = True
-        return self._cache
-
-
-class Context:
-    def __init__(self, parent: "Context" = None):
-        self._parent = parent
-        self._container: Dict[T, Provider[T]] = {}
-
-    @property
-    def parent(self) -> "Context":
-        return self._parent
-
-    @property
-    def root(self) -> "Context":
-        if self._parent is None:
-            return self
-        else:
-            return self._parent.root
-
-    def register(self, key: Type[T], bean: Union[T, Provider[T]]):
-        """
-        register a bean
-        """
-        if not isinstance(bean, Provider):
-            bean = InstanceProvider(bean)
-
-        self._container[key] = bean
-        logger.trace(f"registered bean {key}, provider type: {type(bean)}")
-
-    def register_lazy(self, key: Type[T], bean_initializer: Callable[[], T]):
-        """
-        register a bean lazily
-        """
-        self._container[key] = DynamicProvider(bean_initializer)
-        logger.trace(f"lazily registered bean {key}")
-
-    def register_singleton(self, *args, **kwargs) -> Callable[[Type[T]], Type[T]]:
-        """
-        decorator for a class to register a bean lazily
-        """
-
-        def decorator(cls: Type[T]) -> Type[T]:
-            self.register_lazy(cls, lambda: cls(*args, **kwargs))
-            return cls
-
-        return decorator
-
-    def register_eager_singleton(self, *args, **kwargs) -> Callable[[Type[T]], Type[T]]:
-        """
-        decorator for a class to register a bean lazily
-        """
-
-        def decorator(cls: Type[T]) -> Type[T]:
-            bean = cls(*args, **kwargs)
-            self.register(cls, bean)
-            return cls
-
-        return decorator
-
-    def unregister(self, key: Type[T]) -> bool:
-        """
-        unregister the bean of key
-        """
-        if key in self._container:
-            del self._container[key]
-            return True
-        return False
-
-    def bind(self, key: Type[T], src_key: Type[T2]):
-        """
-        bind key (usually the implementation class) to src_key (usually the base class)
-        """
-        self._container[key] = DynamicProvider(lambda: self._find_provider(src_key).provide(), use_cache=False)
-        logger.trace(f"bind bean {key} to {src_key}")
-
-    def bind_singleton_to(self, key: Type[T], *args, **kwargs) -> Callable[[Type[T2]], Type[T2]]:
-        """
-        decorator for a class (usually the implementation class) to bind to another class (usually the base class)
-        """
-
-        def decorator(cls: Type[T2]) -> Type[T2]:
-            self.register_singleton(*args, **kwargs)(cls)
-            self.bind(key, cls)
-            return cls
-
-        return decorator
-
-    def require(self, key: Type[T]) -> T:
-        return self._find_provider(key).provide()
-
-    def _find_provider(self, key: Type[T]) -> Provider[T]:
-        if key in self._container:
-            return self._container[key]
-        elif self._parent is not None:
-            return self._parent._find_provider(key)
-        else:
-            raise KeyError(key)
-
-    def __getitem__(self, key: Type[T]):
-        return self.require(key)
-
-    def __contains__(self, key: Type[T]) -> bool:
-        if key in self._container:
-            return True
-        elif self._parent is not None:
-            return self._parent.__contains__(key)
-        else:
-            return False
-
-
-__all__ = ("Context",)
+from abc import ABC, abstractmethod
+from typing import TypeVar, Type, Callable, Union, Generic, Dict
+
+from nonebot.log import logger
+
+T = TypeVar("T")
+T2 = TypeVar("T2")
+
+
+class Provider(ABC, Generic[T]):
+    @abstractmethod
+    def provide(self) -> T:
+        raise NotImplementedError()
+
+
+class InstanceProvider(Provider[T], Generic[T]):
+    def __init__(self, instance: T):
+        self._instance = instance
+
+    def provide(self) -> T:
+        return self._instance
+
+
+class DynamicProvider(Provider[T], Generic[T]):
+    def __init__(self, func: Callable[[], T], use_cache: bool = True):
+        self._func = func
+        self._use_cache = use_cache
+
+        self._cache = None
+        self._cached = False
+
+    def provide(self) -> T:
+        if not self._use_cache:
+            return self._func()
+
+        if not self._cached:
+            self._cache = self._func()  # just let it throw
+            self._cached = True
+        return self._cache
+
+
+class Context:
+    def __init__(self, parent: "Context" = None):
+        self._parent = parent
+        self._container: Dict[T, Provider[T]] = {}
+
+    @property
+    def parent(self) -> "Context":
+        return self._parent
+
+    @property
+    def root(self) -> "Context":
+        if self._parent is None:
+            return self
+        else:
+            return self._parent.root
+
+    def register(self, key: Type[T], bean: Union[T, Provider[T]]):
+        """
+        register a bean
+        """
+        if not isinstance(bean, Provider):
+            bean = InstanceProvider(bean)
+
+        self._container[key] = bean
+        logger.trace(f"registered bean {key}, provider type: {type(bean)}")
+
+    def register_lazy(self, key: Type[T], bean_initializer: Callable[[], T]):
+        """
+        register a bean lazily
+        """
+        self._container[key] = DynamicProvider(bean_initializer)
+        logger.trace(f"lazily registered bean {key}")
+
+    def register_singleton(self, *args, **kwargs) -> Callable[[Type[T]], Type[T]]:
+        """
+        decorator for a class to register a bean lazily
+        """
+
+        def decorator(cls: Type[T]) -> Type[T]:
+            self.register_lazy(cls, lambda: cls(*args, **kwargs))
+            return cls
+
+        return decorator
+
+    def register_eager_singleton(self, *args, **kwargs) -> Callable[[Type[T]], Type[T]]:
+        """
+        decorator for a class to register a bean lazily
+        """
+
+        def decorator(cls: Type[T]) -> Type[T]:
+            bean = cls(*args, **kwargs)
+            self.register(cls, bean)
+            return cls
+
+        return decorator
+
+    def unregister(self, key: Type[T]) -> bool:
+        """
+        unregister the bean of key
+        """
+        if key in self._container:
+            del self._container[key]
+            return True
+        return False
+
+    def bind(self, key: Type[T], src_key: Type[T2]):
+        """
+        bind key (usually the implementation class) to src_key (usually the base class)
+        """
+        self._container[key] = DynamicProvider(lambda: self._find_provider(src_key).provide(), use_cache=False)
+        logger.trace(f"bind bean {key} to {src_key}")
+
+    def bind_singleton_to(self, key: Type[T], *args, **kwargs) -> Callable[[Type[T2]], Type[T2]]:
+        """
+        decorator for a class (usually the implementation class) to bind to another class (usually the base class)
+        """
+
+        def decorator(cls: Type[T2]) -> Type[T2]:
+            self.register_singleton(*args, **kwargs)(cls)
+            self.bind(key, cls)
+            return cls
+
+        return decorator
+
+    def require(self, key: Type[T]) -> T:
+        return self._find_provider(key).provide()
+
+    def _find_provider(self, key: Type[T]) -> Provider[T]:
+        if key in self._container:
+            return self._container[key]
+        elif self._parent is not None:
+            return self._parent._find_provider(key)
+        else:
+            raise KeyError(key)
+
+    def __getitem__(self, key: Type[T]):
+        return self.require(key)
+
+    def __contains__(self, key: Type[T]) -> bool:
+        if key in self._container:
+            return True
+        elif self._parent is not None:
+            return self._parent.__contains__(key)
+        else:
+            return False
+
+
+__all__ = ("Context",)
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/nb_session.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/nb_session.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Optional
-
-from nonebot_plugin_datastore.db import get_engine
-from nonebot_plugin_session import Session
-from nonebot_plugin_session.model import get_or_add_session_model, SessionModel
-from sqlalchemy.ext.asyncio import AsyncSession
-
-from ..global_context import context
-
-
-@context.register_singleton()
-class NbSessionRepo:
-    async def get_id(self, session: Session) -> int:
-        async with AsyncSession(get_engine()) as db_sess:
-            model = await get_or_add_session_model(session, db_sess)
-            return model.id
-
-    async def get_session(self, session_id: int) -> Optional[Session]:
-        async with AsyncSession(get_engine()) as db_sess:
-            model = await db_sess.get(SessionModel, session_id)
-            if model is None:
-                return None
-            return model.session
+from typing import Optional
+
+from nonebot_plugin_datastore.db import get_engine
+from nonebot_plugin_session import Session
+from nonebot_plugin_session.model import get_or_add_session_model, SessionModel
+from sqlalchemy.ext.asyncio import AsyncSession
+
+from ..global_context import context
+
+
+@context.register_singleton()
+class NbSessionRepo:
+    async def get_id(self, session: Session) -> int:
+        async with AsyncSession(get_engine()) as db_sess:
+            model = await get_or_add_session_model(session, db_sess)
+            return model.id
+
+    async def get_session(self, session_id: int) -> Optional[Session]:
+        async with AsyncSession(get_engine()) as db_sess:
+            model = await db_sess.get(SessionModel, session_id)
+            if model is None:
+                return None
+            return model.session
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_binding.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_binding.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-from typing import Optional
-
-from sqlalchemy import select, delete
-from sqlalchemy.orm import Mapped, mapped_column
-
-from .source.sql import DataSource
-from .utils.sql import insert
-from ..global_context import context
-from ..model import PixivBinding
-
-
-@DataSource.registry.mapped
-class PixivBindingOrm:
-    __tablename__ = "pixiv_binding"
-
-    platform: Mapped[str] = mapped_column(primary_key=True)
-    user_id: Mapped[str] = mapped_column(primary_key=True)
-    pixiv_user_id: Mapped[int]
-
-
-data_source = context.require(DataSource)
-
-
-@context.register_singleton()
-class PixivBindingRepo:
-
-    async def get(self, platform: str, user_id: str) -> Optional[PixivBinding]:
-        async with data_source.start_session() as session:
-            stmt = (select(PixivBindingOrm)
-                    .where(PixivBindingOrm.platform == platform,
-                           PixivBindingOrm.user_id == user_id)
-                    .limit(1))
-            result = (await session.execute(stmt)).scalar_one_or_none()
-            if result is not None:
-                return PixivBinding(platform=result.platform,
-                                    user_id=result.user_id,
-                                    pixiv_user_id=result.pixiv_user_id)
-            else:
-                return None
-
-    async def update(self, binding: PixivBinding):
-        async with data_source.start_session() as session:
-            stmt = (insert(PixivBindingOrm)
-                    .values(platform=binding.platform,
-                            user_id=binding.user_id,
-                            pixiv_user_id=binding.pixiv_user_id)
-                    .on_conflict_do_update(index_elements=[PixivBindingOrm.platform, PixivBindingOrm.user_id],
-                                           set_={
-                                               PixivBindingOrm.pixiv_user_id: binding.pixiv_user_id
-                                           }))
-            await session.execute(stmt)
-            await session.commit()
-
-    async def remove(self, platform: str, user_id: str) -> bool:
-        async with data_source.start_session() as session:
-            stmt = (delete(PixivBindingOrm)
-                    .where(PixivBindingOrm.platform == platform,
-                           PixivBindingOrm.user_id == user_id))
-            result = await session.execute(stmt)
-            await session.commit()
-            return result.rowcount == 1
-
-
-__all__ = ("PixivBindingRepo",)
+from typing import Optional
+
+from sqlalchemy import select, delete
+from sqlalchemy.orm import Mapped, mapped_column
+
+from .source.sql import DataSource
+from .utils.sql import insert
+from ..global_context import context
+from ..model import PixivBinding
+
+
+@DataSource.registry.mapped
+class PixivBindingOrm:
+    __tablename__ = "pixiv_binding"
+
+    platform: Mapped[str] = mapped_column(primary_key=True)
+    user_id: Mapped[str] = mapped_column(primary_key=True)
+    pixiv_user_id: Mapped[int]
+
+
+data_source = context.require(DataSource)
+
+
+@context.register_singleton()
+class PixivBindingRepo:
+
+    async def get(self, platform: str, user_id: str) -> Optional[PixivBinding]:
+        async with data_source.start_session() as session:
+            stmt = (select(PixivBindingOrm)
+                    .where(PixivBindingOrm.platform == platform,
+                           PixivBindingOrm.user_id == user_id)
+                    .limit(1))
+            result = (await session.execute(stmt)).scalar_one_or_none()
+            if result is not None:
+                return PixivBinding(platform=result.platform,
+                                    user_id=result.user_id,
+                                    pixiv_user_id=result.pixiv_user_id)
+            else:
+                return None
+
+    async def update(self, binding: PixivBinding):
+        async with data_source.start_session() as session:
+            stmt = (insert(PixivBindingOrm)
+                    .values(platform=binding.platform,
+                            user_id=binding.user_id,
+                            pixiv_user_id=binding.pixiv_user_id)
+                    .on_conflict_do_update(index_elements=[PixivBindingOrm.platform, PixivBindingOrm.user_id],
+                                           set_={
+                                               PixivBindingOrm.pixiv_user_id: binding.pixiv_user_id
+                                           }))
+            await session.execute(stmt)
+            await session.commit()
+
+    async def remove(self, platform: str, user_id: str) -> bool:
+        async with data_source.start_session() as session:
+            stmt = (delete(PixivBindingOrm)
+                    .where(PixivBindingOrm.platform == platform,
+                           PixivBindingOrm.user_id == user_id))
+            result = await session.execute(stmt)
+            await session.commit()
+            return result.rowcount == 1
+
+
+__all__ = ("PixivBindingRepo",)
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/base.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/base.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from typing import Union, AsyncGenerator, Protocol
-
-from nonebot_plugin_pixivbot.enums import RankingMode
-from nonebot_plugin_pixivbot.model import Illust, User
-from .lazy_illust import LazyIllust
-from .models import PixivRepoMetadata
-
-
-class PixivRepo(Protocol):
-    def illust_detail(self, illust_id: int) -> AsyncGenerator[Union[Illust, PixivRepoMetadata], None]:
-        ...
-
-    def user_detail(self, user_id: int) -> AsyncGenerator[Union[User, PixivRepoMetadata], None]:
-        ...
-
-    def search_illust(self, word: str) -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        ...
-
-    def search_user(self, word: str) -> AsyncGenerator[Union[User, PixivRepoMetadata], None]:
-        ...
-
-    def user_illusts(self, user_id: int) -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        ...
-
-    def user_bookmarks(self, user_id: int = 0) -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        ...
-
-    def recommended_illusts(self) -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        ...
-
-    def related_illusts(self, illust_id: int) -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        ...
-
-    def illust_ranking(self, mode: Union[str, RankingMode]) \
-            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        ...
-
-    def image(self, illust: Illust, page: int = 0) -> AsyncGenerator[Union[bytes, PixivRepoMetadata], None]:
-        ...
-
-
-__all__ = ("PixivRepo",)
+from typing import Union, AsyncGenerator, Protocol
+
+from nonebot_plugin_pixivbot.enums import RankingMode
+from nonebot_plugin_pixivbot.model import Illust, User
+from .lazy_illust import LazyIllust
+from .models import PixivRepoMetadata
+
+
+class PixivRepo(Protocol):
+    def illust_detail(self, illust_id: int) -> AsyncGenerator[Union[Illust, PixivRepoMetadata], None]:
+        ...
+
+    def user_detail(self, user_id: int) -> AsyncGenerator[Union[User, PixivRepoMetadata], None]:
+        ...
+
+    def search_illust(self, word: str) -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
+        ...
+
+    def search_user(self, word: str) -> AsyncGenerator[Union[User, PixivRepoMetadata], None]:
+        ...
+
+    def user_illusts(self, user_id: int) -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
+        ...
+
+    def user_bookmarks(self, user_id: int = 0) -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
+        ...
+
+    def recommended_illusts(self) -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
+        ...
+
+    def related_illusts(self, illust_id: int) -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
+        ...
+
+    def illust_ranking(self, mode: Union[str, RankingMode]) \
+            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
+        ...
+
+    def image(self, illust: Illust, page: int = 0) -> AsyncGenerator[Union[bytes, PixivRepoMetadata], None]:
+        ...
+
+
+__all__ = ("PixivRepo",)
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/compressor.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/compressor.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-import asyncio
-import functools
-import multiprocessing
-from concurrent.futures.thread import ThreadPoolExecutor
-from io import BytesIO
-
-from PIL import Image, ImageFile
-
-from nonebot_plugin_pixivbot.config import Config
-from nonebot_plugin_pixivbot.global_context import context
-
-conf = context.require(Config)
-
-
-@context.register_singleton()
-class Compressor:
-
-    def __init__(self) -> None:
-        self.enabled = conf.pixiv_compression_enabled
-        self.max_size = conf.pixiv_compression_max_size
-        self.quantity = conf.pixiv_compression_quantity
-
-        if self.enabled:
-            cpu_count = multiprocessing.cpu_count()
-            self._executor = ThreadPoolExecutor(cpu_count, "compressor")
-            # logger.info(f"A ThreadPool with {cpu_count} worker(s) was created for compression")
-
-    async def compress(self, content: bytes) -> bytes:
-        if self.enabled:
-            loop = asyncio.get_running_loop()
-            task = loop.run_in_executor(
-                self._executor, functools.partial(self._compress, content))
-            return await task
-        else:
-            return content
-
-    def _compress(self, content: bytes) -> bytes:
-        p = ImageFile.Parser()
-        p.feed(content)
-        img = p.close()
-
-        w, h = img.size
-        if w > self.max_size or h > self.max_size:
-            ratio = min(self.max_size / w,
-                        self.max_size / h)
-            img_cp = img.resize(
-                (int(ratio * w), int(ratio * h)), Image.ANTIALIAS)
-        else:
-            img_cp = img.copy()
-        img_cp = img_cp.convert("RGB")
-
-        with BytesIO() as bio:
-            img_cp.save(bio, format="JPEG", optimize=True,
-                        quantity=self.quantity)
-            return bio.getvalue()
+import asyncio
+import functools
+import multiprocessing
+from concurrent.futures.thread import ThreadPoolExecutor
+from io import BytesIO
+
+from PIL import Image, ImageFile
+
+from nonebot_plugin_pixivbot.config import Config
+from nonebot_plugin_pixivbot.global_context import context
+
+conf = context.require(Config)
+
+
+@context.register_singleton()
+class Compressor:
+
+    def __init__(self) -> None:
+        self.enabled = conf.pixiv_compression_enabled
+        self.max_size = conf.pixiv_compression_max_size
+        self.quantity = conf.pixiv_compression_quantity
+
+        if self.enabled:
+            cpu_count = multiprocessing.cpu_count()
+            self._executor = ThreadPoolExecutor(cpu_count, "compressor")
+            # logger.info(f"A ThreadPool with {cpu_count} worker(s) was created for compression")
+
+    async def compress(self, content: bytes) -> bytes:
+        if self.enabled:
+            loop = asyncio.get_running_loop()
+            task = loop.run_in_executor(
+                self._executor, functools.partial(self._compress, content))
+            return await task
+        else:
+            return content
+
+    def _compress(self, content: bytes) -> bytes:
+        p = ImageFile.Parser()
+        p.feed(content)
+        img = p.close()
+
+        w, h = img.size
+        if w > self.max_size or h > self.max_size:
+            ratio = min(self.max_size / w,
+                        self.max_size / h)
+            img_cp = img.resize(
+                (int(ratio * w), int(ratio * h)), Image.ANTIALIAS)
+        else:
+            img_cp = img.copy()
+        img_cp = img_cp.convert("RGB")
+
+        with BytesIO() as bio:
+            img_cp.save(bio, format="JPEG", optimize=True,
+                        quantity=self.quantity)
+            return bio.getvalue()
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/__init__.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/__init__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from nonebot import logger
-
-from .base import LocalPixivRepo
-from ....config import Config
-from ....global_context import context
-
-conf = context.require(Config)
-if not conf.pixiv_use_local_cache:
-    from .dummy import DummyPixivRepo
-
-    context.bind(LocalPixivRepo, DummyPixivRepo)
-    logger.info("local cache: disabled")
-else:
-    from .sql import SqlPixivRepo
-
-    context.bind(LocalPixivRepo, SqlPixivRepo)
-    logger.info(f"local cache: enabled ({conf.pixiv_sql_dialect})")
-
-__all__ = ("LocalPixivRepo",)
+from nonebot import logger
+
+from .base import LocalPixivRepo
+from ....config import Config
+from ....global_context import context
+
+conf = context.require(Config)
+if not conf.pixiv_use_local_cache:
+    from .dummy import DummyPixivRepo
+
+    context.bind(LocalPixivRepo, DummyPixivRepo)
+    logger.info("local cache: disabled")
+else:
+    from .sql import SqlPixivRepo
+
+    context.bind(LocalPixivRepo, SqlPixivRepo)
+    logger.info(f"local cache: enabled ({conf.pixiv_sql_dialect})")
+
+__all__ = ("LocalPixivRepo",)
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/base.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/base.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-from typing import List, Union
-
-from nonebot_plugin_pixivbot.enums import RankingMode
-from nonebot_plugin_pixivbot.model import Illust, User
-from ..base import PixivRepo
-from ..lazy_illust import LazyIllust
-from ..models import PixivRepoMetadata
-
-
-class LocalPixivRepo(PixivRepo):
-    async def update_illust_detail(self, illust: Illust, metadata: PixivRepoMetadata):
-        ...
-
-    async def update_user_detail(self, user: User, metadata: PixivRepoMetadata):
-        ...
-
-    async def invalidate_search_illust(self, word: str):
-        ...
-
-    async def append_search_illust(self, word: str,
-                                   content: List[Union[Illust, LazyIllust]],
-                                   metadata: PixivRepoMetadata) -> bool:
-        ...
-
-    async def invalidate_search_user(self, word: str):
-        ...
-
-    async def append_search_user(self, word: str, content: List[User],
-                                 metadata: PixivRepoMetadata) -> bool:
-        ...
-
-    async def invalidate_user_illusts(self, user_id: int):
-        ...
-
-    async def append_user_illusts(self, user_id: int,
-                                  content: List[Union[Illust, LazyIllust]],
-                                  metadata: PixivRepoMetadata,
-                                  append_at_begin: bool = False) -> bool:
-        ...
-
-    async def invalidate_user_bookmarks(self, user_id: int):
-        ...
-
-    async def append_user_bookmarks(self, user_id: int,
-                                    content: List[Union[Illust, LazyIllust]],
-                                    metadata: PixivRepoMetadata,
-                                    append_at_begin: bool = False) -> bool:
-        ...
-
-    async def invalidate_recommended_illusts(self):
-        ...
-
-    async def append_recommended_illusts(self, content: List[Union[Illust, LazyIllust]],
-                                         metadata: PixivRepoMetadata) -> bool:
-        ...
-
-    async def invalidate_related_illusts(self, illust_id: int):
-        ...
-
-    async def append_related_illusts(self, illust_id: int,
-                                     content: List[Union[Illust, LazyIllust]],
-                                     metadata: PixivRepoMetadata) -> bool:
-        ...
-
-    async def invalidate_illust_ranking(self, mode: RankingMode):
-        ...
-
-    async def append_illust_ranking(self, mode: RankingMode,
-                                    content: List[Union[Illust, LazyIllust]],
-                                    metadata: PixivRepoMetadata) -> bool:
-        ...
-
-    async def update_image(self, illust_id: int, page: int, content: bytes,
-                           metadata: PixivRepoMetadata):
-        ...
-
-    async def invalidate_all(self):
-        ...
+from typing import List, Union
+
+from nonebot_plugin_pixivbot.enums import RankingMode
+from nonebot_plugin_pixivbot.model import Illust, User
+from ..base import PixivRepo
+from ..lazy_illust import LazyIllust
+from ..models import PixivRepoMetadata
+
+
+class LocalPixivRepo(PixivRepo):
+    async def update_illust_detail(self, illust: Illust, metadata: PixivRepoMetadata):
+        ...
+
+    async def update_user_detail(self, user: User, metadata: PixivRepoMetadata):
+        ...
+
+    async def invalidate_search_illust(self, word: str):
+        ...
+
+    async def append_search_illust(self, word: str,
+                                   content: List[Union[Illust, LazyIllust]],
+                                   metadata: PixivRepoMetadata) -> bool:
+        ...
+
+    async def invalidate_search_user(self, word: str):
+        ...
+
+    async def append_search_user(self, word: str, content: List[User],
+                                 metadata: PixivRepoMetadata) -> bool:
+        ...
+
+    async def invalidate_user_illusts(self, user_id: int):
+        ...
+
+    async def append_user_illusts(self, user_id: int,
+                                  content: List[Union[Illust, LazyIllust]],
+                                  metadata: PixivRepoMetadata,
+                                  append_at_begin: bool = False) -> bool:
+        ...
+
+    async def invalidate_user_bookmarks(self, user_id: int):
+        ...
+
+    async def append_user_bookmarks(self, user_id: int,
+                                    content: List[Union[Illust, LazyIllust]],
+                                    metadata: PixivRepoMetadata,
+                                    append_at_begin: bool = False) -> bool:
+        ...
+
+    async def invalidate_recommended_illusts(self):
+        ...
+
+    async def append_recommended_illusts(self, content: List[Union[Illust, LazyIllust]],
+                                         metadata: PixivRepoMetadata) -> bool:
+        ...
+
+    async def invalidate_related_illusts(self, illust_id: int):
+        ...
+
+    async def append_related_illusts(self, illust_id: int,
+                                     content: List[Union[Illust, LazyIllust]],
+                                     metadata: PixivRepoMetadata) -> bool:
+        ...
+
+    async def invalidate_illust_ranking(self, mode: RankingMode):
+        ...
+
+    async def append_illust_ranking(self, mode: RankingMode,
+                                    content: List[Union[Illust, LazyIllust]],
+                                    metadata: PixivRepoMetadata) -> bool:
+        ...
+
+    async def update_image(self, illust_id: int, page: int, content: bytes,
+                           metadata: PixivRepoMetadata):
+        ...
+
+    async def invalidate_all(self):
+        ...
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/dummy.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/dummy.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-from nonebot_plugin_pixivbot.data.pixiv_repo.errors import NoSuchItemError
-from nonebot_plugin_pixivbot.data.pixiv_repo.local_repo import LocalPixivRepo
-
-from nonebot_plugin_pixivbot.global_context import context
-
-
-@context.register_singleton()
-class DummyPixivRepo(LocalPixivRepo):
-    # ================ illust_detail ================
-    async def illust_detail(self, *args, **kwargs):
-        raise NoSuchItemError()
-        yield None
-
-    async def update_illust_detail(self, *args, **kwargs):
-        pass
-
-    # ================ user_detail ================
-    async def user_detail(self, *args, **kwargs):
-        raise NoSuchItemError()
-        yield None
-
-    async def update_user_detail(self, *args, **kwargs):
-        pass
-
-    # ================ search_illust ================
-    async def search_illust(self, *args, **kwargs):
-        raise NoSuchItemError()
-        yield None
-
-    async def invalidate_search_illust(self, *args, **kwargs):
-        pass
-
-    async def append_search_illust(self, *args, **kwargs) -> bool:
-        return False
-
-    # ================ search_user ================
-    async def search_user(self, *args, **kwargs):
-        raise NoSuchItemError()
-        yield None
-
-    async def invalidate_search_user(self, *args, **kwargs):
-        pass
-
-    async def append_search_user(self, *args, **kwargs) -> bool:
-        return False
-
-    # ================ user_illusts ================
-    async def user_illusts(self, *args, **kwargs):
-        raise NoSuchItemError()
-        yield None
-
-    async def invalidate_user_illusts(self, *args, **kwargs):
-        pass
-
-    async def append_user_illusts(self, *args, **kwargs) -> bool:
-        return False
-
-    # ================ user_bookmarks ================
-    async def user_bookmarks(self, *args, **kwargs):
-        raise NoSuchItemError()
-        yield None
-
-    async def invalidate_user_bookmarks(self, *args, **kwargs):
-        pass
-
-    async def append_user_bookmarks(self, *args, **kwargs) -> bool:
-        return False
-
-    # ================ recommended_illusts ================
-    async def recommended_illusts(self, *args, **kwargs):
-        raise NoSuchItemError()
-        yield None
-
-    async def invalidate_recommended_illusts(self, *args, **kwargs):
-        pass
-
-    async def append_recommended_illusts(self, *args, **kwargs) -> bool:
-        return False
-
-    # ================ related_illusts ================
-    async def related_illusts(self, *args, **kwargs):
-        raise NoSuchItemError()
-        yield None
-
-    async def invalidate_related_illusts(self, *args, **kwargs):
-        pass
-
-    async def append_related_illusts(self, *args, **kwargs) -> bool:
-        return False
-
-    # ================ illust_ranking ================
-    async def illust_ranking(self, *args, **kwargs):
-        raise NoSuchItemError()
-        yield None
-
-    async def invalidate_illust_ranking(self, *args, **kwargs):
-        pass
-
-    async def append_illust_ranking(self, *args, **kwargs) -> bool:
-        return False
-
-    # ================ image ================
-    async def image(self, *args, **kwargs):
-        raise NoSuchItemError()
-        yield None
-
-    async def update_image(self, *args, **kwargs):
-        pass
-
-    async def invalidate_all(self, *args, **kwargs):
-        pass
+from nonebot_plugin_pixivbot.data.pixiv_repo.errors import NoSuchItemError
+from nonebot_plugin_pixivbot.data.pixiv_repo.local_repo import LocalPixivRepo
+
+from nonebot_plugin_pixivbot.global_context import context
+
+
+@context.register_singleton()
+class DummyPixivRepo(LocalPixivRepo):
+    # ================ illust_detail ================
+    async def illust_detail(self, *args, **kwargs):
+        raise NoSuchItemError()
+        yield None
+
+    async def update_illust_detail(self, *args, **kwargs):
+        pass
+
+    # ================ user_detail ================
+    async def user_detail(self, *args, **kwargs):
+        raise NoSuchItemError()
+        yield None
+
+    async def update_user_detail(self, *args, **kwargs):
+        pass
+
+    # ================ search_illust ================
+    async def search_illust(self, *args, **kwargs):
+        raise NoSuchItemError()
+        yield None
+
+    async def invalidate_search_illust(self, *args, **kwargs):
+        pass
+
+    async def append_search_illust(self, *args, **kwargs) -> bool:
+        return False
+
+    # ================ search_user ================
+    async def search_user(self, *args, **kwargs):
+        raise NoSuchItemError()
+        yield None
+
+    async def invalidate_search_user(self, *args, **kwargs):
+        pass
+
+    async def append_search_user(self, *args, **kwargs) -> bool:
+        return False
+
+    # ================ user_illusts ================
+    async def user_illusts(self, *args, **kwargs):
+        raise NoSuchItemError()
+        yield None
+
+    async def invalidate_user_illusts(self, *args, **kwargs):
+        pass
+
+    async def append_user_illusts(self, *args, **kwargs) -> bool:
+        return False
+
+    # ================ user_bookmarks ================
+    async def user_bookmarks(self, *args, **kwargs):
+        raise NoSuchItemError()
+        yield None
+
+    async def invalidate_user_bookmarks(self, *args, **kwargs):
+        pass
+
+    async def append_user_bookmarks(self, *args, **kwargs) -> bool:
+        return False
+
+    # ================ recommended_illusts ================
+    async def recommended_illusts(self, *args, **kwargs):
+        raise NoSuchItemError()
+        yield None
+
+    async def invalidate_recommended_illusts(self, *args, **kwargs):
+        pass
+
+    async def append_recommended_illusts(self, *args, **kwargs) -> bool:
+        return False
+
+    # ================ related_illusts ================
+    async def related_illusts(self, *args, **kwargs):
+        raise NoSuchItemError()
+        yield None
+
+    async def invalidate_related_illusts(self, *args, **kwargs):
+        pass
+
+    async def append_related_illusts(self, *args, **kwargs) -> bool:
+        return False
+
+    # ================ illust_ranking ================
+    async def illust_ranking(self, *args, **kwargs):
+        raise NoSuchItemError()
+        yield None
+
+    async def invalidate_illust_ranking(self, *args, **kwargs):
+        pass
+
+    async def append_illust_ranking(self, *args, **kwargs) -> bool:
+        return False
+
+    # ================ image ================
+    async def image(self, *args, **kwargs):
+        raise NoSuchItemError()
+        yield None
+
+    async def update_image(self, *args, **kwargs):
+        pass
+
+    async def invalidate_all(self, *args, **kwargs):
+        pass
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,690 +1,690 @@
-from datetime import datetime, timezone, timedelta
-from functools import partial
-from typing import AsyncGenerator, Union, Optional, List
-
-from apscheduler.triggers.interval import IntervalTrigger
-from nonebot import logger
-from nonebot_plugin_apscheduler import scheduler as apscheduler
-from sqlalchemy import select, delete, func, text
-from sqlalchemy.ext.asyncio import AsyncSession
-
-from .base import LocalPixivRepo
-from .sql_models import IllustDetailCache, UserDetailCache, DownloadCache, IllustSetCache, IllustSetCacheIllust, \
-    UserSetCache, UserSetCacheUser
-from ..errors import CacheExpiredError, NoSuchItemError
-from ..lazy_illust import LazyIllust
-from ..models import PixivRepoMetadata
-from ...local_tag import LocalTagRepo
-from ...source.sql import DataSource
-from ...utils.sql import insert
-from ....config import Config
-from ....enums import RankingMode
-from ....global_context import context
-from ....model import Illust, User
-from ....utils.lifecycler import on_startup
-
-
-def _handle_expires_in(metadata: PixivRepoMetadata, expires_in: int):
-    if datetime.now(timezone.utc) - metadata.update_time >= timedelta(seconds=expires_in):
-        raise CacheExpiredError(metadata)
-
-
-def _extract_metadata(cache, is_set_cache):
-    update_time = cache.update_time.replace(tzinfo=timezone.utc)
-
-    if is_set_cache:
-        metadata = PixivRepoMetadata(update_time=update_time, pages=cache.pages, next_qs=cache.next_qs)
-    else:
-        metadata = PixivRepoMetadata(update_time=update_time)
-    return metadata
-
-
-conf = context.require(Config)
-data_source = context.require(DataSource)
-local_tags = context.require(LocalTagRepo)
-
-
-@context.register_singleton()
-class SqlPixivRepo(LocalPixivRepo):
-
-    def __init__(self):
-        on_startup(replay=True)(
-            partial(
-                apscheduler.add_job,
-                self.clean_expired,
-                id='pixivbot_sql_pixiv_repo_clean_expired',
-                trigger=IntervalTrigger(hours=2),
-                max_instances=1
-            )
-        )
-
-    async def _get_illusts(self, session: AsyncSession,
-                           cache_type: str,
-                           key: dict,
-                           expired_in: int,
-                           offset: int = 0, ):
-        stmt = (select(IllustSetCache)
-                .where(IllustSetCache.cache_type == cache_type,
-                       IllustSetCache.key == key))
-        cache: Optional[IllustSetCache] = (await session.execute(stmt)).scalar_one_or_none()
-        if cache is None:
-            raise NoSuchItemError()
-
-        metadata = _extract_metadata(cache, True)
-        _handle_expires_in(metadata, expired_in)
-
-        yield metadata.copy(update={"pages": 0})
-
-        stmt = (select(IllustSetCacheIllust, IllustDetailCache)
-                .where(IllustSetCacheIllust.cache_id == cache.id)
-                .outerjoin(IllustDetailCache, IllustSetCacheIllust.illust_id == IllustDetailCache.illust_id)
-                .order_by(IllustSetCacheIllust.rank, IllustDetailCache.update_time.desc())
-                .offset(offset))
-
-        total = 0
-        broken = 0
-
-        try:
-            async for cache_illust, illust in await session.stream(stmt):
-                cache_illust: IllustSetCacheIllust
-                illust: Optional[IllustDetailCache]
-
-                total += 1
-
-                if illust is not None:
-                    yield LazyIllust(illust.illust_id, Illust(**illust.illust))
-                else:
-                    yield LazyIllust(cache_illust.illust_id)
-                    broken += 1
-        finally:
-            logger.debug(f"[local] got {total} illusts, illust_detail of {broken} are missed")
-
-        yield metadata
-
-    async def _invalidate_illusts(self, session: AsyncSession,
-                                  cache_type: str,
-                                  key: dict):
-        if conf.pixiv_sql_dialect == 'sqlite':
-            await session.execute(text("PRAGMA foreign_keys = ON;"))
-
-        stmt = (delete(IllustSetCache)
-                .where(IllustSetCache.cache_type == cache_type,
-                       IllustSetCache.key == key))
-        await session.execute(stmt)
-        await session.commit()
-
-    async def _append_and_check_illusts(self, session: AsyncSession,
-                                        cache_type: str,
-                                        key: dict,
-                                        content: List[Union[Illust, LazyIllust]],
-                                        metadata: PixivRepoMetadata,
-                                        append_at_begin: bool = False):
-        async with session.begin_nested() as tx1:
-            async with session.begin_nested() as tx2:
-                stmt = (select(IllustSetCache)
-                        .where(IllustSetCache.cache_type == cache_type,
-                               IllustSetCache.key == key)
-                        .limit(1))
-                cache = (await session.execute(stmt)).scalar_one_or_none()
-                if cache is None:
-                    cache = IllustSetCache(cache_type=cache_type, key=key)
-                    session.add(cache)
-
-                cache.update_time = metadata.update_time
-                cache.next_qs = metadata.next_qs
-                cache.pages = metadata.pages
-
-                # commit to get cache id
-                await tx2.commit()
-
-            row_count = 0
-            if append_at_begin:
-                stmt = select(
-                    func.min(IllustSetCacheIllust.rank)
-                ).select_from(IllustSetCacheIllust).where(
-                    IllustSetCacheIllust.cache_id == cache.id
-                )
-
-                rnk = (await session.execute(stmt)).scalar_one_or_none()
-                if rnk is None:
-                    rnk = 0
-
-                for x in reversed(content):
-                    stmt = insert(IllustSetCacheIllust).values(
-                        cache_id=cache.id, illust_id=x.id, rank=rnk - 1
-                    ).on_conflict_do_nothing(index_elements=[
-                        IllustSetCacheIllust.cache_id, IllustSetCacheIllust.illust_id
-                    ])
-                    result = await session.execute(stmt)
-                    row_count += result.rowcount
-                    rnk -= result.rowcount
-            else:
-                stmt = select(
-                    func.max(IllustSetCacheIllust.rank)
-                ).select_from(IllustSetCacheIllust).where(
-                    IllustSetCacheIllust.cache_id == cache.id
-                )
-
-                rnk = (await session.execute(stmt)).scalar_one_or_none()
-                if rnk is None:
-                    rnk = 0
-
-                for x in content:
-                    stmt = insert(IllustSetCacheIllust).values(
-                        cache_id=cache.id, illust_id=x.id, rank=rnk + 1
-                    ).on_conflict_do_nothing(index_elements=[
-                        IllustSetCacheIllust.cache_id, IllustSetCacheIllust.illust_id
-                    ])
-                    result = await session.execute(stmt)
-                    row_count += result.rowcount
-                    rnk += result.rowcount
-
-            cache.size += row_count
-
-            await tx1.commit()
-
-        # insert illust detail
-        for x in content:
-            if isinstance(x, LazyIllust):
-                if not x.loaded:
-                    continue
-                x = x.content
-
-            stmt = insert(IllustDetailCache).values(
-                illust_id=x.id, illust=x.dict(), update_time=metadata.update_time
-            )
-            stmt = stmt.on_conflict_do_update(
-                index_elements=[IllustDetailCache.illust_id],
-                set_={
-                    IllustDetailCache.illust: stmt.excluded.illust,
-                    IllustDetailCache.update_time: stmt.excluded.update_time
-                }
-            )
-            await session.execute(stmt)
-
-        await session.commit()
-
-        # insert local tags
-        li = []
-        for x in content:
-            if isinstance(x, LazyIllust):
-                if not x.loaded:
-                    continue
-                x = x.content
-            li.append(x)
-        await local_tags.update_from_illusts(li)
-
-        return row_count != len(content)
-
-    async def _get_users(self, session: AsyncSession,
-                         cache_type: str,
-                         key: dict,
-                         expired_in: int,
-                         offset: int = 0):
-        stmt = (select(UserSetCache)
-                .where(UserSetCache.cache_type == cache_type,
-                       UserSetCache.key == key))
-        cache = (await session.execute(stmt)).scalar_one_or_none()
-        if cache is None:
-            raise NoSuchItemError()
-
-        metadata = _extract_metadata(cache, True)
-        _handle_expires_in(metadata, expired_in)
-
-        yield metadata.copy(update={"pages": 0})
-
-        stmt = (select(UserSetCacheUser, UserDetailCache)
-                .where(UserSetCacheUser.cache_id == cache.id)
-                .outerjoin(UserDetailCache, UserSetCacheUser.user_id == UserDetailCache.user_id)
-                .offset(offset))
-
-        total = 0
-        try:
-            async for cache_user, user in await session.stream(stmt):
-                if user is not None:
-                    yield User(**user.user)
-                else:
-                    yield User(id=cache_user.user_id, name="", account="")
-                total += 1
-        finally:
-            logger.debug(f"[local] got {total} users")
-
-        yield metadata
-
-    async def _invalidate_users(self, session: AsyncSession,
-                                cache_type: str,
-                                key: dict):
-        if conf.pixiv_sql_dialect == 'sqlite':
-            await session.execute(text("PRAGMA foreign_keys = ON;"))
-
-        stmt = (delete(UserSetCache)
-                .where(UserSetCache.cache_type == cache_type,
-                       UserSetCache.key == key))
-        await session.execute(stmt)
-        await session.commit()
-
-    async def _append_and_check_users(self, session: AsyncSession,
-                                      cache_type: str,
-                                      key: dict,
-                                      content: List[User],
-                                      metadata: PixivRepoMetadata):
-
-        async with session.begin_nested() as tx1:
-            async with session.begin_nested() as tx2:
-                stmt = (select(UserSetCache)
-                        .where(UserSetCache.cache_type == cache_type,
-                               UserSetCache.key == key)
-                        .limit(1))
-                cache = (await session.execute(stmt)).scalar_one_or_none()
-                if cache is None:
-                    cache = UserSetCache(cache_type=cache_type, key=key)
-                    session.add(cache)
-
-                cache.update_time = metadata.update_time
-                cache.next_qs = metadata.next_qs
-                cache.pages = metadata.pages
-
-                # commit to get cache id
-                await tx2.commit()
-
-            row_count = 0
-            for x in content:
-                stmt = insert(UserSetCacheUser).values(
-                    cache_id=cache.id, user_id=x.id
-                ).on_conflict_do_nothing(index_elements=[
-                    UserSetCacheUser.cache_id, UserSetCacheUser.user_id
-                ])
-                row_count += (await session.execute(stmt)).rowcount
-
-            await tx1.commit()
-
-        # insert user detail
-        for x in content:
-            stmt = insert(UserDetailCache).values(
-                user_id=x.id, user=x.dict(), update_time=metadata.update_time
-            )
-            stmt = stmt.on_conflict_do_update(
-                index_elements=[UserDetailCache.user_id],
-                set_={
-                    UserDetailCache.user: stmt.excluded.user,
-                    UserDetailCache.update_time: stmt.excluded.update_time
-                }
-            )
-            await session.execute(stmt)
-            await session.commit()
-
-        return row_count != len(content)
-
-    # ================ illust_detail ================
-    async def illust_detail(self, illust_id: int) \
-            -> AsyncGenerator[Union[Illust, PixivRepoMetadata], None]:
-        logger.debug(f"[local] illust_detail {illust_id}")
-
-        async with data_source.start_session() as session:
-            stmt = select(IllustDetailCache).where(IllustDetailCache.illust_id == illust_id).limit(1)
-            cache = (await session.execute(stmt)).scalar_one_or_none()
-
-            if cache is not None:
-                metadata = _extract_metadata(cache, False)
-                _handle_expires_in(metadata, conf.pixiv_illust_detail_cache_expires_in)
-
-                yield metadata
-                yield Illust(**cache.illust)
-            else:
-                raise NoSuchItemError()
-
-    async def update_illust_detail(self, illust: Illust, metadata: PixivRepoMetadata):
-        logger.debug(f"[local] update illust_detail {illust.id} {metadata}")
-
-        async with data_source.start_session() as session:
-            stmt = (insert(IllustDetailCache)
-                    .values(illust_id=illust.id, illust=illust.dict(), update_time=metadata.update_time))
-            stmt = stmt.on_conflict_do_update(index_elements=[IllustDetailCache.illust_id],
-                                              set_={
-                                                  IllustDetailCache.illust: stmt.excluded.illust,
-                                                  IllustDetailCache.update_time: stmt.excluded.update_time
-                                              })
-
-            await session.execute(stmt)
-            await session.commit()
-
-            if conf.pixiv_tag_translation_enabled:
-                await local_tags.update_from_illusts([illust])
-
-    # ================ user_detail ================
-    async def user_detail(self, user_id: int) \
-            -> AsyncGenerator[Union[User, PixivRepoMetadata], None]:
-        logger.debug(f"[local] user_detail {user_id}")
-
-        async with data_source.start_session() as session:
-            stmt = select(UserDetailCache).where(UserDetailCache.user_id == user_id).limit(1)
-            cache = (await session.execute(stmt)).scalar_one_or_none()
-
-            if cache is not None:
-                metadata = _extract_metadata(cache, False)
-                _handle_expires_in(metadata, conf.pixiv_user_detail_cache_expires_in)
-
-                yield metadata
-                yield User(**cache.user)
-            else:
-                raise NoSuchItemError()
-
-    async def update_user_detail(self, user: User, metadata: PixivRepoMetadata):
-        logger.debug(f"[local] update user_detail {user.id} {metadata}")
-
-        async with data_source.start_session() as session:
-            stmt = (insert(UserDetailCache)
-                    .values(user_id=user.id, user=user.dict(), update_time=metadata.update_time))
-            stmt = stmt.on_conflict_do_update(index_elements=[UserDetailCache.user_id],
-                                              set_={
-                                                  UserDetailCache.user: stmt.excluded.user,
-                                                  UserDetailCache.update_time: stmt.excluded.update_time
-                                              })
-
-            await session.execute(stmt)
-            await session.commit()
-
-    # ================ image ================
-    async def image(self, illust: Illust, page: int = 0) -> AsyncGenerator[Union[bytes, PixivRepoMetadata], None]:
-        logger.debug(f"[local] image {illust.id}")
-
-        async with data_source.start_session() as session:
-            stmt = select(DownloadCache).where(DownloadCache.illust_id == illust.id,
-                                               DownloadCache.page == page).limit(1)
-            cache = (await session.execute(stmt)).scalar_one_or_none()
-
-            if cache is not None:
-                metadata = _extract_metadata(cache, False)
-                _handle_expires_in(metadata, conf.pixiv_download_cache_expires_in)
-
-                yield metadata
-                yield cache.content
-            else:
-                raise NoSuchItemError()
-
-    async def update_image(self, illust_id: int, page: int,
-                           content: bytes, metadata: PixivRepoMetadata):
-        logger.debug(f"[local] update image {illust_id} {metadata}")
-
-        async with data_source.start_session() as session:
-            stmt = (insert(DownloadCache)
-                    .values(illust_id=illust_id, page=page, content=content, update_time=metadata.update_time))
-            stmt = stmt.on_conflict_do_update(index_elements=[DownloadCache.illust_id, DownloadCache.page],
-                                              set_={
-                                                  DownloadCache.content: stmt.excluded.content,
-                                                  DownloadCache.update_time: stmt.excluded.update_time
-                                              })
-
-            await session.execute(stmt)
-            await session.commit()
-
-    # ================ illust_ranking ================
-    async def illust_ranking(self, mode: Union[str, RankingMode], *, offset: int = 0) \
-            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        if isinstance(mode, str):
-            mode = RankingMode[mode]
-
-        logger.debug(f"[local] illust_ranking {mode}")
-
-        async with data_source.start_session() as session:
-            async for x in self._get_illusts(session, "illust_ranking", {"mode": mode},
-                                             expired_in=conf.pixiv_illust_ranking_cache_expires_in, offset=offset):
-                yield x
-
-    async def invalidate_illust_ranking(self, mode: RankingMode):
-        logger.debug(f"[local] invalidate illust_ranking")
-        async with data_source.start_session() as session:
-            await self._invalidate_illusts(session, "illust_ranking", {"mode": mode})
-
-    async def append_illust_ranking(self, mode: RankingMode, content: List[Union[Illust, LazyIllust]],
-                                    metadata: PixivRepoMetadata) -> bool:
-        logger.debug(f"[local] append illust_ranking {mode} "
-                     f"({len(content)} items) "
-                     f"{metadata}")
-        async with data_source.start_session() as session:
-            return await self._append_and_check_illusts(session, "illust_ranking", {"mode": mode},
-                                                        content=content, metadata=metadata)
-
-    # ================ search_illust ================
-    async def search_illust(self, word: str, *, offset: int = 0) \
-            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        logger.debug(f"[local] search_illust {word}")
-        async with data_source.start_session() as session:
-            async for x in self._get_illusts(session, "search_illust", {"word": word},
-                                             expired_in=conf.pixiv_search_illust_cache_expires_in, offset=offset):
-                yield x
-
-    async def invalidate_search_illust(self, word: str):
-        logger.debug(f"[local] invalidate search_illust {word}")
-        async with data_source.start_session() as session:
-            await self._invalidate_illusts(session, "search_illust", {"word": word})
-
-    async def append_search_illust(self, word: str, content: List[Union[Illust, LazyIllust]],
-                                   metadata: PixivRepoMetadata) -> bool:
-        # 返回值表示content中是否有已经存在于集合的文档，下同
-        logger.debug(f"[local] append search_illust {word} "
-                     f"({len(content)} items) "
-                     f"{metadata}")
-        async with data_source.start_session() as session:
-            return await self._append_and_check_illusts(session, "search_illust", {"word": word},
-                                                        content=content, metadata=metadata)
-
-    # ================ user_illusts ================
-    async def user_illusts(self, user_id: int, *, offset: int = 0) \
-            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        logger.debug(f"[local] user_illusts {user_id}")
-        async with data_source.start_session() as session:
-            async for x in self._get_illusts(session, "user_illusts", {"user_id": user_id},
-                                             expired_in=conf.pixiv_user_illusts_cache_expires_in, offset=offset):
-                yield x
-
-    async def invalidate_user_illusts(self, user_id: int):
-        logger.debug(f"[local] invalidate user_illusts {user_id}")
-        async with data_source.start_session() as session:
-            await self._invalidate_illusts(session, "user_illusts", {"user_id": user_id})
-
-    async def append_user_illusts(self, user_id: int,
-                                  content: List[Union[Illust, LazyIllust]],
-                                  metadata: PixivRepoMetadata,
-                                  append_at_begin: bool = False) -> bool:
-        logger.debug(f"[local] append user_illusts {user_id} "
-                     f"{'at begin ' if append_at_begin else ''}"
-                     f"({len(content)} items) "
-                     f"{metadata}")
-        async with data_source.start_session() as session:
-            return await self._append_and_check_illusts(session, "user_illusts", {"user_id": user_id},
-                                                        content=content, metadata=metadata,
-                                                        append_at_begin=append_at_begin)
-
-    # ================ user_bookmarks ================
-    async def user_bookmarks(self, user_id: int = 0, *, offset: int = 0) \
-            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        logger.debug(f"[local] user_bookmarks {user_id}")
-        async with data_source.start_session() as session:
-            async for x in self._get_illusts(session, "user_bookmarks", {"user_id": user_id},
-                                             expired_in=conf.pixiv_user_bookmarks_cache_expires_in, offset=offset):
-                yield x
-
-    async def invalidate_user_bookmarks(self, user_id: int):
-        logger.debug(f"[local] invalidate user_bookmarks {user_id}")
-        async with data_source.start_session() as session:
-            await self._invalidate_illusts(session, "user_bookmarks", {"user_id": user_id})
-
-    async def append_user_bookmarks(self, user_id: int,
-                                    content: List[Union[Illust, LazyIllust]],
-                                    metadata: PixivRepoMetadata,
-                                    append_at_begin: bool = False) -> bool:
-        logger.debug(f"[local] append user_bookmarks {user_id} "
-                     f"{'at begin ' if append_at_begin else ''} "
-                     f"({len(content)} items) "
-                     f"{metadata}")
-        async with data_source.start_session() as session:
-            return await self._append_and_check_illusts(session, "user_bookmarks", {"user_id": user_id},
-                                                        content=content, metadata=metadata,
-                                                        append_at_begin=append_at_begin)
-
-    # ================ recommended_illusts ================
-    async def recommended_illusts(self, *, offset: int = 0) \
-            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        logger.debug(f"[local] recommended_illusts")
-        async with data_source.start_session() as session:
-            async for x in self._get_illusts(session, "other", {"type": "recommended_illusts"},
-                                             expired_in=conf.pixiv_other_cache_expires_in, offset=offset):
-                yield x
-
-    async def invalidate_recommended_illusts(self):
-        logger.debug(f"[local] invalidate recommended_illusts")
-        async with data_source.start_session() as session:
-            await self._invalidate_illusts(session, "other", {"type": "recommended_illusts"})
-
-    async def append_recommended_illusts(self, content: List[Union[Illust, LazyIllust]],
-                                         metadata: PixivRepoMetadata) -> bool:
-        logger.debug(f"[local] append recommended_illusts "
-                     f"({len(content)} items) "
-                     f"{metadata}")
-        async with data_source.start_session() as session:
-            return await self._append_and_check_illusts(session, "other", {"type": "recommended_illusts"},
-                                                        content=content, metadata=metadata)
-
-    # ================ related_illusts ================
-    async def related_illusts(self, illust_id: int, *, offset: int = 0) \
-            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        logger.debug(f"[local] related_illusts {illust_id}")
-        async with data_source.start_session() as session:
-            async for x in self._get_illusts(session, "related_illusts", {"original_illust_id": illust_id},
-                                             expired_in=conf.pixiv_related_illusts_cache_expires_in,
-                                             offset=offset):
-                yield x
-
-    async def invalidate_related_illusts(self, illust_id: int):
-        logger.debug(f"[local] invalidate related_illusts")
-        async with data_source.start_session() as session:
-            await self._invalidate_illusts(session, "related_illusts", {"original_illust_id": illust_id})
-
-    async def append_related_illusts(self, illust_id: int, content: List[Union[Illust, LazyIllust]],
-                                     metadata: PixivRepoMetadata) -> bool:
-        logger.debug(f"[local] append related_illusts {illust_id} "
-                     f"({len(content)} items) "
-                     f"{metadata}")
-        async with data_source.start_session() as session:
-            return await self._append_and_check_illusts(session, "related_illusts", {"original_illust_id": illust_id},
-                                                        content=content, metadata=metadata)
-
-    # ================ search_user ================
-    async def search_user(self, word: str, *, offset: int = 0) \
-            -> AsyncGenerator[Union[User, PixivRepoMetadata], None]:
-        logger.debug(f"[local] search_user {word}")
-        async with data_source.start_session() as session:
-            async for x in self._get_users(session, "search_user", {"word": word},
-                                           expired_in=conf.pixiv_search_user_cache_expires_in, offset=offset):
-                yield x
-
-    async def invalidate_search_user(self, word: str):
-        logger.debug(f"[local] invalidate search_user {word}")
-        async with data_source.start_session() as session:
-            await self._invalidate_users(session, "search_user", {"word": word})
-
-    async def append_search_user(self, word: str, content: List[User],
-                                 metadata: PixivRepoMetadata) -> bool:
-        logger.debug(f"[local] append search_user {word} "
-                     f"({len(content)} items) "
-                     f"{metadata}")
-        async with data_source.start_session() as session:
-            return await self._append_and_check_users(session, "search_user", {"word": word},
-                                                      content=content, metadata=metadata)
-
-    async def invalidate_all(self):
-        logger.debug(f"[local] invalidate_all")
-
-        async with data_source.start_session() as session:
-            if conf.pixiv_sql_dialect == 'sqlite':
-                await session.execute(text("PRAGMA foreign_keys = ON;"))
-
-            result = await session.execute(delete(IllustSetCache))
-            logger.success(f"[local] deleted {result.rowcount} illust_set cache")
-            result = await session.execute(delete(UserSetCache))
-            logger.success(f"[local] deleted {result.rowcount} user_set cache")
-            result = await session.execute(delete(IllustDetailCache))
-            logger.success(f"[local] deleted {result.rowcount} illust_detail cache")
-            result = await session.execute(delete(UserDetailCache))
-            logger.success(f"[local] deleted {result.rowcount} user_detail cache")
-            result = await session.execute(delete(DownloadCache))
-            logger.success(f"[local] deleted {result.rowcount} download cache")
-            await session.commit()
-
-    async def clean_expired(self):
-        logger.debug(f"[local] clean_expired")
-
-        async with data_source.start_session() as session:
-            if conf.pixiv_sql_dialect == 'sqlite':
-                await session.execute(text("PRAGMA foreign_keys = ON;"))
-
-            now = datetime.utcnow()
-            stmt = delete(IllustDetailCache).where(
-                IllustDetailCache.update_time <= now - timedelta(seconds=conf.pixiv_illust_detail_cache_expires_in)
-            )
-            result = await session.execute(stmt)
-            logger.success(f"[local] deleted {result.rowcount} illust_detail cache")
-
-            stmt = delete(UserDetailCache).where(
-                UserDetailCache.update_time <= now - timedelta(seconds=conf.pixiv_user_detail_cache_expires_in)
-            )
-            result = await session.execute(stmt)
-            logger.success(f"[local] deleted {result.rowcount} user_detail cache")
-
-            stmt = delete(DownloadCache).where(
-                DownloadCache.update_time <= now - timedelta(seconds=conf.pixiv_download_cache_expires_in)
-            )
-            result = await session.execute(stmt)
-            logger.success(f"[local] deleted {result.rowcount} download cache")
-
-            stmt = delete(IllustSetCache).where(
-                IllustSetCache.cache_type == 'illust_ranking',
-                IllustSetCache.update_time <= now - timedelta(seconds=conf.pixiv_illust_ranking_cache_expires_in)
-            )
-            result = await session.execute(stmt)
-            logger.success(f"[local] deleted {result.rowcount} illust_ranking cache")
-
-            stmt = delete(IllustSetCache).where(
-                IllustSetCache.cache_type == 'search_illust',
-                IllustSetCache.update_time <= now - timedelta(seconds=conf.pixiv_search_illust_cache_delete_in)
-            )
-            result = await session.execute(stmt)
-            logger.success(f"[local] deleted {result.rowcount} search_illust cache")
-
-            stmt = delete(UserSetCache).where(
-                UserSetCache.cache_type == 'search_user',
-                UserSetCache.update_time <= now - timedelta(seconds=conf.pixiv_search_user_cache_delete_in)
-            )
-            result = await session.execute(stmt)
-            logger.success(f"[local] deleted {result.rowcount} search_user cache")
-
-            stmt = delete(IllustSetCache).where(
-                IllustSetCache.cache_type == 'user_illusts',
-                IllustSetCache.update_time <= now - timedelta(seconds=conf.pixiv_user_illusts_cache_delete_in)
-            )
-            result = await session.execute(stmt)
-            logger.success(f"[local] deleted {result.rowcount} user_illusts cache")
-
-            stmt = delete(IllustSetCache).where(
-                IllustSetCache.cache_type == 'user_bookmarks',
-                IllustSetCache.update_time <= now - timedelta(seconds=conf.pixiv_user_bookmarks_cache_delete_in)
-            )
-            result = await session.execute(stmt)
-            logger.success(f"[local] deleted {result.rowcount} user_bookmarks cache")
-
-            stmt = delete(IllustSetCache).where(
-                IllustSetCache.cache_type == 'related_illusts',
-                IllustSetCache.update_time <= now - timedelta(seconds=conf.pixiv_related_illusts_cache_expires_in)
-            )
-            result = await session.execute(stmt)
-            logger.success(f"[local] deleted {result.rowcount} related_illusts cache")
-
-            stmt = delete(IllustSetCache).where(
-                IllustSetCache.cache_type == 'other',
-                IllustSetCache.update_time <= now - timedelta(seconds=conf.pixiv_other_cache_expires_in)
-            )
-            result = await session.execute(stmt)
-            logger.success(f"[local] deleted {result.rowcount} other cache")
-
-            await session.commit()
+from datetime import datetime, timezone, timedelta
+from functools import partial
+from typing import AsyncGenerator, Union, Optional, List
+
+from apscheduler.triggers.interval import IntervalTrigger
+from nonebot import logger
+from nonebot_plugin_apscheduler import scheduler as apscheduler
+from sqlalchemy import select, delete, func, text
+from sqlalchemy.ext.asyncio import AsyncSession
+
+from .base import LocalPixivRepo
+from .sql_models import IllustDetailCache, UserDetailCache, DownloadCache, IllustSetCache, IllustSetCacheIllust, \
+    UserSetCache, UserSetCacheUser
+from ..errors import CacheExpiredError, NoSuchItemError
+from ..lazy_illust import LazyIllust
+from ..models import PixivRepoMetadata
+from ...local_tag import LocalTagRepo
+from ...source.sql import DataSource
+from ...utils.sql import insert
+from ....config import Config
+from ....enums import RankingMode
+from ....global_context import context
+from ....model import Illust, User
+from ....utils.lifecycler import on_startup
+
+
+def _handle_expires_in(metadata: PixivRepoMetadata, expires_in: int):
+    if datetime.now(timezone.utc) - metadata.update_time >= timedelta(seconds=expires_in):
+        raise CacheExpiredError(metadata)
+
+
+def _extract_metadata(cache, is_set_cache):
+    update_time = cache.update_time.replace(tzinfo=timezone.utc)
+
+    if is_set_cache:
+        metadata = PixivRepoMetadata(update_time=update_time, pages=cache.pages, next_qs=cache.next_qs)
+    else:
+        metadata = PixivRepoMetadata(update_time=update_time)
+    return metadata
+
+
+conf = context.require(Config)
+data_source = context.require(DataSource)
+local_tags = context.require(LocalTagRepo)
+
+
+@context.register_singleton()
+class SqlPixivRepo(LocalPixivRepo):
+
+    def __init__(self):
+        on_startup(replay=True)(
+            partial(
+                apscheduler.add_job,
+                self.clean_expired,
+                id='pixivbot_sql_pixiv_repo_clean_expired',
+                trigger=IntervalTrigger(hours=2),
+                max_instances=1
+            )
+        )
+
+    async def _get_illusts(self, session: AsyncSession,
+                           cache_type: str,
+                           key: dict,
+                           expired_in: int,
+                           offset: int = 0, ):
+        stmt = (select(IllustSetCache)
+                .where(IllustSetCache.cache_type == cache_type,
+                       IllustSetCache.key == key))
+        cache: Optional[IllustSetCache] = (await session.execute(stmt)).scalar_one_or_none()
+        if cache is None:
+            raise NoSuchItemError()
+
+        metadata = _extract_metadata(cache, True)
+        _handle_expires_in(metadata, expired_in)
+
+        yield metadata.copy(update={"pages": 0})
+
+        stmt = (select(IllustSetCacheIllust, IllustDetailCache)
+                .where(IllustSetCacheIllust.cache_id == cache.id)
+                .outerjoin(IllustDetailCache, IllustSetCacheIllust.illust_id == IllustDetailCache.illust_id)
+                .order_by(IllustSetCacheIllust.rank, IllustDetailCache.update_time.desc())
+                .offset(offset))
+
+        total = 0
+        broken = 0
+
+        try:
+            async for cache_illust, illust in await session.stream(stmt):
+                cache_illust: IllustSetCacheIllust
+                illust: Optional[IllustDetailCache]
+
+                total += 1
+
+                if illust is not None:
+                    yield LazyIllust(illust.illust_id, Illust(**illust.illust))
+                else:
+                    yield LazyIllust(cache_illust.illust_id)
+                    broken += 1
+        finally:
+            logger.debug(f"[local] got {total} illusts, illust_detail of {broken} are missed")
+
+        yield metadata
+
+    async def _invalidate_illusts(self, session: AsyncSession,
+                                  cache_type: str,
+                                  key: dict):
+        if conf.pixiv_sql_dialect == 'sqlite':
+            await session.execute(text("PRAGMA foreign_keys = ON;"))
+
+        stmt = (delete(IllustSetCache)
+                .where(IllustSetCache.cache_type == cache_type,
+                       IllustSetCache.key == key))
+        await session.execute(stmt)
+        await session.commit()
+
+    async def _append_and_check_illusts(self, session: AsyncSession,
+                                        cache_type: str,
+                                        key: dict,
+                                        content: List[Union[Illust, LazyIllust]],
+                                        metadata: PixivRepoMetadata,
+                                        append_at_begin: bool = False):
+        async with session.begin_nested() as tx1:
+            async with session.begin_nested() as tx2:
+                stmt = (select(IllustSetCache)
+                        .where(IllustSetCache.cache_type == cache_type,
+                               IllustSetCache.key == key)
+                        .limit(1))
+                cache = (await session.execute(stmt)).scalar_one_or_none()
+                if cache is None:
+                    cache = IllustSetCache(cache_type=cache_type, key=key)
+                    session.add(cache)
+
+                cache.update_time = metadata.update_time
+                cache.next_qs = metadata.next_qs
+                cache.pages = metadata.pages
+
+                # commit to get cache id
+                await tx2.commit()
+
+            row_count = 0
+            if append_at_begin:
+                stmt = select(
+                    func.min(IllustSetCacheIllust.rank)
+                ).select_from(IllustSetCacheIllust).where(
+                    IllustSetCacheIllust.cache_id == cache.id
+                )
+
+                rnk = (await session.execute(stmt)).scalar_one_or_none()
+                if rnk is None:
+                    rnk = 0
+
+                for x in reversed(content):
+                    stmt = insert(IllustSetCacheIllust).values(
+                        cache_id=cache.id, illust_id=x.id, rank=rnk - 1
+                    ).on_conflict_do_nothing(index_elements=[
+                        IllustSetCacheIllust.cache_id, IllustSetCacheIllust.illust_id
+                    ])
+                    result = await session.execute(stmt)
+                    row_count += result.rowcount
+                    rnk -= result.rowcount
+            else:
+                stmt = select(
+                    func.max(IllustSetCacheIllust.rank)
+                ).select_from(IllustSetCacheIllust).where(
+                    IllustSetCacheIllust.cache_id == cache.id
+                )
+
+                rnk = (await session.execute(stmt)).scalar_one_or_none()
+                if rnk is None:
+                    rnk = 0
+
+                for x in content:
+                    stmt = insert(IllustSetCacheIllust).values(
+                        cache_id=cache.id, illust_id=x.id, rank=rnk + 1
+                    ).on_conflict_do_nothing(index_elements=[
+                        IllustSetCacheIllust.cache_id, IllustSetCacheIllust.illust_id
+                    ])
+                    result = await session.execute(stmt)
+                    row_count += result.rowcount
+                    rnk += result.rowcount
+
+            cache.size += row_count
+
+            await tx1.commit()
+
+        # insert illust detail
+        for x in content:
+            if isinstance(x, LazyIllust):
+                if not x.loaded:
+                    continue
+                x = x.content
+
+            stmt = insert(IllustDetailCache).values(
+                illust_id=x.id, illust=x.dict(), update_time=metadata.update_time
+            )
+            stmt = stmt.on_conflict_do_update(
+                index_elements=[IllustDetailCache.illust_id],
+                set_={
+                    IllustDetailCache.illust: stmt.excluded.illust,
+                    IllustDetailCache.update_time: stmt.excluded.update_time
+                }
+            )
+            await session.execute(stmt)
+
+        await session.commit()
+
+        # insert local tags
+        li = []
+        for x in content:
+            if isinstance(x, LazyIllust):
+                if not x.loaded:
+                    continue
+                x = x.content
+            li.append(x)
+        await local_tags.update_from_illusts(li)
+
+        return row_count != len(content)
+
+    async def _get_users(self, session: AsyncSession,
+                         cache_type: str,
+                         key: dict,
+                         expired_in: int,
+                         offset: int = 0):
+        stmt = (select(UserSetCache)
+                .where(UserSetCache.cache_type == cache_type,
+                       UserSetCache.key == key))
+        cache = (await session.execute(stmt)).scalar_one_or_none()
+        if cache is None:
+            raise NoSuchItemError()
+
+        metadata = _extract_metadata(cache, True)
+        _handle_expires_in(metadata, expired_in)
+
+        yield metadata.copy(update={"pages": 0})
+
+        stmt = (select(UserSetCacheUser, UserDetailCache)
+                .where(UserSetCacheUser.cache_id == cache.id)
+                .outerjoin(UserDetailCache, UserSetCacheUser.user_id == UserDetailCache.user_id)
+                .offset(offset))
+
+        total = 0
+        try:
+            async for cache_user, user in await session.stream(stmt):
+                if user is not None:
+                    yield User(**user.user)
+                else:
+                    yield User(id=cache_user.user_id, name="", account="")
+                total += 1
+        finally:
+            logger.debug(f"[local] got {total} users")
+
+        yield metadata
+
+    async def _invalidate_users(self, session: AsyncSession,
+                                cache_type: str,
+                                key: dict):
+        if conf.pixiv_sql_dialect == 'sqlite':
+            await session.execute(text("PRAGMA foreign_keys = ON;"))
+
+        stmt = (delete(UserSetCache)
+                .where(UserSetCache.cache_type == cache_type,
+                       UserSetCache.key == key))
+        await session.execute(stmt)
+        await session.commit()
+
+    async def _append_and_check_users(self, session: AsyncSession,
+                                      cache_type: str,
+                                      key: dict,
+                                      content: List[User],
+                                      metadata: PixivRepoMetadata):
+
+        async with session.begin_nested() as tx1:
+            async with session.begin_nested() as tx2:
+                stmt = (select(UserSetCache)
+                        .where(UserSetCache.cache_type == cache_type,
+                               UserSetCache.key == key)
+                        .limit(1))
+                cache = (await session.execute(stmt)).scalar_one_or_none()
+                if cache is None:
+                    cache = UserSetCache(cache_type=cache_type, key=key)
+                    session.add(cache)
+
+                cache.update_time = metadata.update_time
+                cache.next_qs = metadata.next_qs
+                cache.pages = metadata.pages
+
+                # commit to get cache id
+                await tx2.commit()
+
+            row_count = 0
+            for x in content:
+                stmt = insert(UserSetCacheUser).values(
+                    cache_id=cache.id, user_id=x.id
+                ).on_conflict_do_nothing(index_elements=[
+                    UserSetCacheUser.cache_id, UserSetCacheUser.user_id
+                ])
+                row_count += (await session.execute(stmt)).rowcount
+
+            await tx1.commit()
+
+        # insert user detail
+        for x in content:
+            stmt = insert(UserDetailCache).values(
+                user_id=x.id, user=x.dict(), update_time=metadata.update_time
+            )
+            stmt = stmt.on_conflict_do_update(
+                index_elements=[UserDetailCache.user_id],
+                set_={
+                    UserDetailCache.user: stmt.excluded.user,
+                    UserDetailCache.update_time: stmt.excluded.update_time
+                }
+            )
+            await session.execute(stmt)
+            await session.commit()
+
+        return row_count != len(content)
+
+    # ================ illust_detail ================
+    async def illust_detail(self, illust_id: int) \
+            -> AsyncGenerator[Union[Illust, PixivRepoMetadata], None]:
+        logger.debug(f"[local] illust_detail {illust_id}")
+
+        async with data_source.start_session() as session:
+            stmt = select(IllustDetailCache).where(IllustDetailCache.illust_id == illust_id).limit(1)
+            cache = (await session.execute(stmt)).scalar_one_or_none()
+
+            if cache is not None:
+                metadata = _extract_metadata(cache, False)
+                _handle_expires_in(metadata, conf.pixiv_illust_detail_cache_expires_in)
+
+                yield metadata
+                yield Illust(**cache.illust)
+            else:
+                raise NoSuchItemError()
+
+    async def update_illust_detail(self, illust: Illust, metadata: PixivRepoMetadata):
+        logger.debug(f"[local] update illust_detail {illust.id} {metadata}")
+
+        async with data_source.start_session() as session:
+            stmt = (insert(IllustDetailCache)
+                    .values(illust_id=illust.id, illust=illust.dict(), update_time=metadata.update_time))
+            stmt = stmt.on_conflict_do_update(index_elements=[IllustDetailCache.illust_id],
+                                              set_={
+                                                  IllustDetailCache.illust: stmt.excluded.illust,
+                                                  IllustDetailCache.update_time: stmt.excluded.update_time
+                                              })
+
+            await session.execute(stmt)
+            await session.commit()
+
+            if conf.pixiv_tag_translation_enabled:
+                await local_tags.update_from_illusts([illust])
+
+    # ================ user_detail ================
+    async def user_detail(self, user_id: int) \
+            -> AsyncGenerator[Union[User, PixivRepoMetadata], None]:
+        logger.debug(f"[local] user_detail {user_id}")
+
+        async with data_source.start_session() as session:
+            stmt = select(UserDetailCache).where(UserDetailCache.user_id == user_id).limit(1)
+            cache = (await session.execute(stmt)).scalar_one_or_none()
+
+            if cache is not None:
+                metadata = _extract_metadata(cache, False)
+                _handle_expires_in(metadata, conf.pixiv_user_detail_cache_expires_in)
+
+                yield metadata
+                yield User(**cache.user)
+            else:
+                raise NoSuchItemError()
+
+    async def update_user_detail(self, user: User, metadata: PixivRepoMetadata):
+        logger.debug(f"[local] update user_detail {user.id} {metadata}")
+
+        async with data_source.start_session() as session:
+            stmt = (insert(UserDetailCache)
+                    .values(user_id=user.id, user=user.dict(), update_time=metadata.update_time))
+            stmt = stmt.on_conflict_do_update(index_elements=[UserDetailCache.user_id],
+                                              set_={
+                                                  UserDetailCache.user: stmt.excluded.user,
+                                                  UserDetailCache.update_time: stmt.excluded.update_time
+                                              })
+
+            await session.execute(stmt)
+            await session.commit()
+
+    # ================ image ================
+    async def image(self, illust: Illust, page: int = 0) -> AsyncGenerator[Union[bytes, PixivRepoMetadata], None]:
+        logger.debug(f"[local] image {illust.id}")
+
+        async with data_source.start_session() as session:
+            stmt = select(DownloadCache).where(DownloadCache.illust_id == illust.id,
+                                               DownloadCache.page == page).limit(1)
+            cache = (await session.execute(stmt)).scalar_one_or_none()
+
+            if cache is not None:
+                metadata = _extract_metadata(cache, False)
+                _handle_expires_in(metadata, conf.pixiv_download_cache_expires_in)
+
+                yield metadata
+                yield cache.content
+            else:
+                raise NoSuchItemError()
+
+    async def update_image(self, illust_id: int, page: int,
+                           content: bytes, metadata: PixivRepoMetadata):
+        logger.debug(f"[local] update image {illust_id} {metadata}")
+
+        async with data_source.start_session() as session:
+            stmt = (insert(DownloadCache)
+                    .values(illust_id=illust_id, page=page, content=content, update_time=metadata.update_time))
+            stmt = stmt.on_conflict_do_update(index_elements=[DownloadCache.illust_id, DownloadCache.page],
+                                              set_={
+                                                  DownloadCache.content: stmt.excluded.content,
+                                                  DownloadCache.update_time: stmt.excluded.update_time
+                                              })
+
+            await session.execute(stmt)
+            await session.commit()
+
+    # ================ illust_ranking ================
+    async def illust_ranking(self, mode: Union[str, RankingMode], *, offset: int = 0) \
+            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
+        if isinstance(mode, str):
+            mode = RankingMode[mode]
+
+        logger.debug(f"[local] illust_ranking {mode}")
+
+        async with data_source.start_session() as session:
+            async for x in self._get_illusts(session, "illust_ranking", {"mode": mode},
+                                             expired_in=conf.pixiv_illust_ranking_cache_expires_in, offset=offset):
+                yield x
+
+    async def invalidate_illust_ranking(self, mode: RankingMode):
+        logger.debug(f"[local] invalidate illust_ranking")
+        async with data_source.start_session() as session:
+            await self._invalidate_illusts(session, "illust_ranking", {"mode": mode})
+
+    async def append_illust_ranking(self, mode: RankingMode, content: List[Union[Illust, LazyIllust]],
+                                    metadata: PixivRepoMetadata) -> bool:
+        logger.debug(f"[local] append illust_ranking {mode} "
+                     f"({len(content)} items) "
+                     f"{metadata}")
+        async with data_source.start_session() as session:
+            return await self._append_and_check_illusts(session, "illust_ranking", {"mode": mode},
+                                                        content=content, metadata=metadata)
+
+    # ================ search_illust ================
+    async def search_illust(self, word: str, *, offset: int = 0) \
+            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
+        logger.debug(f"[local] search_illust {word}")
+        async with data_source.start_session() as session:
+            async for x in self._get_illusts(session, "search_illust", {"word": word},
+                                             expired_in=conf.pixiv_search_illust_cache_expires_in, offset=offset):
+                yield x
+
+    async def invalidate_search_illust(self, word: str):
+        logger.debug(f"[local] invalidate search_illust {word}")
+        async with data_source.start_session() as session:
+            await self._invalidate_illusts(session, "search_illust", {"word": word})
+
+    async def append_search_illust(self, word: str, content: List[Union[Illust, LazyIllust]],
+                                   metadata: PixivRepoMetadata) -> bool:
+        # 返回值表示content中是否有已经存在于集合的文档，下同
+        logger.debug(f"[local] append search_illust {word} "
+                     f"({len(content)} items) "
+                     f"{metadata}")
+        async with data_source.start_session() as session:
+            return await self._append_and_check_illusts(session, "search_illust", {"word": word},
+                                                        content=content, metadata=metadata)
+
+    # ================ user_illusts ================
+    async def user_illusts(self, user_id: int, *, offset: int = 0) \
+            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
+        logger.debug(f"[local] user_illusts {user_id}")
+        async with data_source.start_session() as session:
+            async for x in self._get_illusts(session, "user_illusts", {"user_id": user_id},
+                                             expired_in=conf.pixiv_user_illusts_cache_expires_in, offset=offset):
+                yield x
+
+    async def invalidate_user_illusts(self, user_id: int):
+        logger.debug(f"[local] invalidate user_illusts {user_id}")
+        async with data_source.start_session() as session:
+            await self._invalidate_illusts(session, "user_illusts", {"user_id": user_id})
+
+    async def append_user_illusts(self, user_id: int,
+                                  content: List[Union[Illust, LazyIllust]],
+                                  metadata: PixivRepoMetadata,
+                                  append_at_begin: bool = False) -> bool:
+        logger.debug(f"[local] append user_illusts {user_id} "
+                     f"{'at begin ' if append_at_begin else ''}"
+                     f"({len(content)} items) "
+                     f"{metadata}")
+        async with data_source.start_session() as session:
+            return await self._append_and_check_illusts(session, "user_illusts", {"user_id": user_id},
+                                                        content=content, metadata=metadata,
+                                                        append_at_begin=append_at_begin)
+
+    # ================ user_bookmarks ================
+    async def user_bookmarks(self, user_id: int = 0, *, offset: int = 0) \
+            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
+        logger.debug(f"[local] user_bookmarks {user_id}")
+        async with data_source.start_session() as session:
+            async for x in self._get_illusts(session, "user_bookmarks", {"user_id": user_id},
+                                             expired_in=conf.pixiv_user_bookmarks_cache_expires_in, offset=offset):
+                yield x
+
+    async def invalidate_user_bookmarks(self, user_id: int):
+        logger.debug(f"[local] invalidate user_bookmarks {user_id}")
+        async with data_source.start_session() as session:
+            await self._invalidate_illusts(session, "user_bookmarks", {"user_id": user_id})
+
+    async def append_user_bookmarks(self, user_id: int,
+                                    content: List[Union[Illust, LazyIllust]],
+                                    metadata: PixivRepoMetadata,
+                                    append_at_begin: bool = False) -> bool:
+        logger.debug(f"[local] append user_bookmarks {user_id} "
+                     f"{'at begin ' if append_at_begin else ''} "
+                     f"({len(content)} items) "
+                     f"{metadata}")
+        async with data_source.start_session() as session:
+            return await self._append_and_check_illusts(session, "user_bookmarks", {"user_id": user_id},
+                                                        content=content, metadata=metadata,
+                                                        append_at_begin=append_at_begin)
+
+    # ================ recommended_illusts ================
+    async def recommended_illusts(self, *, offset: int = 0) \
+            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
+        logger.debug(f"[local] recommended_illusts")
+        async with data_source.start_session() as session:
+            async for x in self._get_illusts(session, "other", {"type": "recommended_illusts"},
+                                             expired_in=conf.pixiv_other_cache_expires_in, offset=offset):
+                yield x
+
+    async def invalidate_recommended_illusts(self):
+        logger.debug(f"[local] invalidate recommended_illusts")
+        async with data_source.start_session() as session:
+            await self._invalidate_illusts(session, "other", {"type": "recommended_illusts"})
+
+    async def append_recommended_illusts(self, content: List[Union[Illust, LazyIllust]],
+                                         metadata: PixivRepoMetadata) -> bool:
+        logger.debug(f"[local] append recommended_illusts "
+                     f"({len(content)} items) "
+                     f"{metadata}")
+        async with data_source.start_session() as session:
+            return await self._append_and_check_illusts(session, "other", {"type": "recommended_illusts"},
+                                                        content=content, metadata=metadata)
+
+    # ================ related_illusts ================
+    async def related_illusts(self, illust_id: int, *, offset: int = 0) \
+            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
+        logger.debug(f"[local] related_illusts {illust_id}")
+        async with data_source.start_session() as session:
+            async for x in self._get_illusts(session, "related_illusts", {"original_illust_id": illust_id},
+                                             expired_in=conf.pixiv_related_illusts_cache_expires_in,
+                                             offset=offset):
+                yield x
+
+    async def invalidate_related_illusts(self, illust_id: int):
+        logger.debug(f"[local] invalidate related_illusts")
+        async with data_source.start_session() as session:
+            await self._invalidate_illusts(session, "related_illusts", {"original_illust_id": illust_id})
+
+    async def append_related_illusts(self, illust_id: int, content: List[Union[Illust, LazyIllust]],
+                                     metadata: PixivRepoMetadata) -> bool:
+        logger.debug(f"[local] append related_illusts {illust_id} "
+                     f"({len(content)} items) "
+                     f"{metadata}")
+        async with data_source.start_session() as session:
+            return await self._append_and_check_illusts(session, "related_illusts", {"original_illust_id": illust_id},
+                                                        content=content, metadata=metadata)
+
+    # ================ search_user ================
+    async def search_user(self, word: str, *, offset: int = 0) \
+            -> AsyncGenerator[Union[User, PixivRepoMetadata], None]:
+        logger.debug(f"[local] search_user {word}")
+        async with data_source.start_session() as session:
+            async for x in self._get_users(session, "search_user", {"word": word},
+                                           expired_in=conf.pixiv_search_user_cache_expires_in, offset=offset):
+                yield x
+
+    async def invalidate_search_user(self, word: str):
+        logger.debug(f"[local] invalidate search_user {word}")
+        async with data_source.start_session() as session:
+            await self._invalidate_users(session, "search_user", {"word": word})
+
+    async def append_search_user(self, word: str, content: List[User],
+                                 metadata: PixivRepoMetadata) -> bool:
+        logger.debug(f"[local] append search_user {word} "
+                     f"({len(content)} items) "
+                     f"{metadata}")
+        async with data_source.start_session() as session:
+            return await self._append_and_check_users(session, "search_user", {"word": word},
+                                                      content=content, metadata=metadata)
+
+    async def invalidate_all(self):
+        logger.debug(f"[local] invalidate_all")
+
+        async with data_source.start_session() as session:
+            if conf.pixiv_sql_dialect == 'sqlite':
+                await session.execute(text("PRAGMA foreign_keys = ON;"))
+
+            result = await session.execute(delete(IllustSetCache))
+            logger.success(f"[local] deleted {result.rowcount} illust_set cache")
+            result = await session.execute(delete(UserSetCache))
+            logger.success(f"[local] deleted {result.rowcount} user_set cache")
+            result = await session.execute(delete(IllustDetailCache))
+            logger.success(f"[local] deleted {result.rowcount} illust_detail cache")
+            result = await session.execute(delete(UserDetailCache))
+            logger.success(f"[local] deleted {result.rowcount} user_detail cache")
+            result = await session.execute(delete(DownloadCache))
+            logger.success(f"[local] deleted {result.rowcount} download cache")
+            await session.commit()
+
+    async def clean_expired(self):
+        logger.debug(f"[local] clean_expired")
+
+        async with data_source.start_session() as session:
+            if conf.pixiv_sql_dialect == 'sqlite':
+                await session.execute(text("PRAGMA foreign_keys = ON;"))
+
+            now = datetime.utcnow()
+            stmt = delete(IllustDetailCache).where(
+                IllustDetailCache.update_time <= now - timedelta(seconds=conf.pixiv_illust_detail_cache_expires_in)
+            )
+            result = await session.execute(stmt)
+            logger.success(f"[local] deleted {result.rowcount} illust_detail cache")
+
+            stmt = delete(UserDetailCache).where(
+                UserDetailCache.update_time <= now - timedelta(seconds=conf.pixiv_user_detail_cache_expires_in)
+            )
+            result = await session.execute(stmt)
+            logger.success(f"[local] deleted {result.rowcount} user_detail cache")
+
+            stmt = delete(DownloadCache).where(
+                DownloadCache.update_time <= now - timedelta(seconds=conf.pixiv_download_cache_expires_in)
+            )
+            result = await session.execute(stmt)
+            logger.success(f"[local] deleted {result.rowcount} download cache")
+
+            stmt = delete(IllustSetCache).where(
+                IllustSetCache.cache_type == 'illust_ranking',
+                IllustSetCache.update_time <= now - timedelta(seconds=conf.pixiv_illust_ranking_cache_expires_in)
+            )
+            result = await session.execute(stmt)
+            logger.success(f"[local] deleted {result.rowcount} illust_ranking cache")
+
+            stmt = delete(IllustSetCache).where(
+                IllustSetCache.cache_type == 'search_illust',
+                IllustSetCache.update_time <= now - timedelta(seconds=conf.pixiv_search_illust_cache_delete_in)
+            )
+            result = await session.execute(stmt)
+            logger.success(f"[local] deleted {result.rowcount} search_illust cache")
+
+            stmt = delete(UserSetCache).where(
+                UserSetCache.cache_type == 'search_user',
+                UserSetCache.update_time <= now - timedelta(seconds=conf.pixiv_search_user_cache_delete_in)
+            )
+            result = await session.execute(stmt)
+            logger.success(f"[local] deleted {result.rowcount} search_user cache")
+
+            stmt = delete(IllustSetCache).where(
+                IllustSetCache.cache_type == 'user_illusts',
+                IllustSetCache.update_time <= now - timedelta(seconds=conf.pixiv_user_illusts_cache_delete_in)
+            )
+            result = await session.execute(stmt)
+            logger.success(f"[local] deleted {result.rowcount} user_illusts cache")
+
+            stmt = delete(IllustSetCache).where(
+                IllustSetCache.cache_type == 'user_bookmarks',
+                IllustSetCache.update_time <= now - timedelta(seconds=conf.pixiv_user_bookmarks_cache_delete_in)
+            )
+            result = await session.execute(stmt)
+            logger.success(f"[local] deleted {result.rowcount} user_bookmarks cache")
+
+            stmt = delete(IllustSetCache).where(
+                IllustSetCache.cache_type == 'related_illusts',
+                IllustSetCache.update_time <= now - timedelta(seconds=conf.pixiv_related_illusts_cache_expires_in)
+            )
+            result = await session.execute(stmt)
+            logger.success(f"[local] deleted {result.rowcount} related_illusts cache")
+
+            stmt = delete(IllustSetCache).where(
+                IllustSetCache.cache_type == 'other',
+                IllustSetCache.update_time <= now - timedelta(seconds=conf.pixiv_other_cache_expires_in)
+            )
+            result = await session.execute(stmt)
+            logger.success(f"[local] deleted {result.rowcount} other cache")
+
+            await session.commit()
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql_models.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/local_repo/sql_models.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-from datetime import datetime
-from typing import Optional, List
-
-from sqlalchemy import ForeignKey, UniqueConstraint
-from sqlalchemy.orm import mapped_column, relationship, Mapped
-
-from ...source.sql import DataSource
-from ...utils.sql import BLOB, JSON, UTCDateTime
-
-
-@DataSource.registry.mapped
-class DownloadCache:
-    __tablename__ = "download_cache"
-
-    illust_id: Mapped[int] = mapped_column(primary_key=True)
-    page: Mapped[int] = mapped_column(primary_key=True, default=0)
-    content: Mapped[bytes] = mapped_column(BLOB)
-
-    update_time: Mapped[datetime] = mapped_column(UTCDateTime, index=True)
-
-
-@DataSource.registry.mapped
-class IllustDetailCache:
-    __tablename__ = "illust_detail_cache"
-
-    illust_id: Mapped[int] = mapped_column(primary_key=True)
-    illust: Mapped[dict] = mapped_column(JSON)
-
-    update_time: Mapped[datetime] = mapped_column(UTCDateTime, index=True)
-
-
-@DataSource.registry.mapped
-class UserDetailCache:
-    __tablename__ = "user_detail_cache"
-
-    user_id: Mapped[int] = mapped_column(primary_key=True)
-    user: Mapped[dict] = mapped_column(JSON)
-
-    update_time: Mapped[datetime] = mapped_column(UTCDateTime, index=True)
-
-
-@DataSource.registry.mapped
-class IllustSetCache:
-    __tablename__ = "illust_set_cache"
-
-    id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
-    cache_type: Mapped[str]
-    key: Mapped[dict] = mapped_column(JSON)
-
-    update_time: Mapped[datetime] = mapped_column(UTCDateTime, index=True)
-    pages: Mapped[Optional[int]]
-    next_qs: Mapped[Optional[dict]] = mapped_column(JSON)
-
-    illust_id: Mapped[List["IllustSetCacheIllust"]] = relationship(foreign_keys="IllustSetCacheIllust.cache_id",
-                                                                   cascade="save-update, delete",
-                                                                   passive_deletes=True)
-
-    size: Mapped[int] = mapped_column(default=0)
-
-    __table_args__ = (
-        UniqueConstraint('cache_type', 'key'),
-    )
-
-
-@DataSource.registry.mapped
-class IllustSetCacheIllust:
-    __tablename__ = "illust_set_cache_illust"
-
-    cache_id: Mapped[int] = mapped_column(ForeignKey("illust_set_cache.id", ondelete="cascade"), primary_key=True)
-    illust_id: Mapped[int] = mapped_column(primary_key=True)
-    rank: Mapped[int] = mapped_column(default=0)
-
-
-@DataSource.registry.mapped
-class UserSetCache:
-    __tablename__ = "user_set_cache"
-
-    id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
-    cache_type: Mapped[str]
-    key: Mapped[dict] = mapped_column(JSON)
-
-    update_time: Mapped[datetime] = mapped_column(UTCDateTime, index=True)
-    pages: Mapped[Optional[int]]
-    next_qs: Mapped[Optional[dict]] = mapped_column(JSON)
-
-    illust_id: Mapped[List["UserSetCacheUser"]] = relationship(foreign_keys="UserSetCacheUser.cache_id",
-                                                               cascade="save-update, delete",
-                                                               passive_deletes=True)
-
-    __table_args__ = (
-        UniqueConstraint('cache_type', 'key'),
-    )
-
-
-@DataSource.registry.mapped
-class UserSetCacheUser:
-    __tablename__ = "user_set_cache_user"
-
-    cache_id: Mapped[int] = mapped_column(ForeignKey("user_set_cache.id", ondelete="cascade"), primary_key=True)
-    user_id: Mapped[int] = mapped_column(primary_key=True)
+from datetime import datetime
+from typing import Optional, List
+
+from sqlalchemy import ForeignKey, UniqueConstraint
+from sqlalchemy.orm import mapped_column, relationship, Mapped
+
+from ...source.sql import DataSource
+from ...utils.sql import BLOB, JSON, UTCDateTime
+
+
+@DataSource.registry.mapped
+class DownloadCache:
+    __tablename__ = "download_cache"
+
+    illust_id: Mapped[int] = mapped_column(primary_key=True)
+    page: Mapped[int] = mapped_column(primary_key=True, default=0)
+    content: Mapped[bytes] = mapped_column(BLOB)
+
+    update_time: Mapped[datetime] = mapped_column(UTCDateTime, index=True)
+
+
+@DataSource.registry.mapped
+class IllustDetailCache:
+    __tablename__ = "illust_detail_cache"
+
+    illust_id: Mapped[int] = mapped_column(primary_key=True)
+    illust: Mapped[dict] = mapped_column(JSON)
+
+    update_time: Mapped[datetime] = mapped_column(UTCDateTime, index=True)
+
+
+@DataSource.registry.mapped
+class UserDetailCache:
+    __tablename__ = "user_detail_cache"
+
+    user_id: Mapped[int] = mapped_column(primary_key=True)
+    user: Mapped[dict] = mapped_column(JSON)
+
+    update_time: Mapped[datetime] = mapped_column(UTCDateTime, index=True)
+
+
+@DataSource.registry.mapped
+class IllustSetCache:
+    __tablename__ = "illust_set_cache"
+
+    id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
+    cache_type: Mapped[str]
+    key: Mapped[dict] = mapped_column(JSON)
+
+    update_time: Mapped[datetime] = mapped_column(UTCDateTime, index=True)
+    pages: Mapped[Optional[int]]
+    next_qs: Mapped[Optional[dict]] = mapped_column(JSON)
+
+    illust_id: Mapped[List["IllustSetCacheIllust"]] = relationship(foreign_keys="IllustSetCacheIllust.cache_id",
+                                                                   cascade="save-update, delete",
+                                                                   passive_deletes=True)
+
+    size: Mapped[int] = mapped_column(default=0)
+
+    __table_args__ = (
+        UniqueConstraint('cache_type', 'key'),
+    )
+
+
+@DataSource.registry.mapped
+class IllustSetCacheIllust:
+    __tablename__ = "illust_set_cache_illust"
+
+    cache_id: Mapped[int] = mapped_column(ForeignKey("illust_set_cache.id", ondelete="cascade"), primary_key=True)
+    illust_id: Mapped[int] = mapped_column(primary_key=True)
+    rank: Mapped[int] = mapped_column(default=0)
+
+
+@DataSource.registry.mapped
+class UserSetCache:
+    __tablename__ = "user_set_cache"
+
+    id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
+    cache_type: Mapped[str]
+    key: Mapped[dict] = mapped_column(JSON)
+
+    update_time: Mapped[datetime] = mapped_column(UTCDateTime, index=True)
+    pages: Mapped[Optional[int]]
+    next_qs: Mapped[Optional[dict]] = mapped_column(JSON)
+
+    illust_id: Mapped[List["UserSetCacheUser"]] = relationship(foreign_keys="UserSetCacheUser.cache_id",
+                                                               cascade="save-update, delete",
+                                                               passive_deletes=True)
+
+    __table_args__ = (
+        UniqueConstraint('cache_type', 'key'),
+    )
+
+
+@DataSource.registry.mapped
+class UserSetCacheUser:
+    __tablename__ = "user_set_cache_user"
+
+    cache_id: Mapped[int] = mapped_column(ForeignKey("user_set_cache.id", ondelete="cascade"), primary_key=True)
+    user_id: Mapped[int] = mapped_column(primary_key=True)
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,226 +1,226 @@
-from datetime import datetime, timezone
-from typing import List, AsyncGenerator, TypeVar, Union, Callable, Awaitable, Optional, Any, Mapping, Protocol, Generic
-
-from nonebot import logger
-
-from .errors import NoSuchItemError, CacheExpiredError
-from .models import PixivRepoMetadata
-from ...utils.format import format_kwargs
-
-T = TypeVar("T")
-
-T_KWARGS = Mapping[str, Any]
-
-
-class Mediator(Protocol[T]):
-    def mediate(self, query_kwargs: T_KWARGS, **kwargs) -> AsyncGenerator[Union[T, PixivRepoMetadata], None]:
-        ...
-
-
-class SingleMediator(Mediator, Generic[T]):
-    def __init__(self, tag: str,
-                 cache_factory: Callable[[T_KWARGS], AsyncGenerator[Union[T, PixivRepoMetadata], None]],
-                 remote_factory: Callable[[T_KWARGS], AsyncGenerator[Union[T, PixivRepoMetadata], None]],
-                 cache_updater: Callable[[T_KWARGS, T, Optional[PixivRepoMetadata]], Awaitable[Any]]):
-        self.tag = tag
-        self.cache_factory = cache_factory
-        self.remote_factory = remote_factory
-        self.cache_updater = cache_updater
-
-    async def mediate(self, query_kwargs: T_KWARGS,
-                      *, force_expiration: bool = False) -> AsyncGenerator[Union[T, PixivRepoMetadata], None]:
-        try:
-            if force_expiration:
-                raise NoSuchItemError()
-            async for x in self.cache_factory(query_kwargs):
-                yield x
-            logger.info(f"[{self.tag}] cache loaded  ({format_kwargs(**query_kwargs)})")
-        except (NoSuchItemError, CacheExpiredError):
-            logger.info(f"[{self.tag}] no cache or cache expired  ({format_kwargs(**query_kwargs)})")
-
-            content = None
-            metadata = None
-
-            async for x in self.remote_factory(query_kwargs):
-                if isinstance(x, PixivRepoMetadata):
-                    metadata = x
-                else:
-                    content = x
-
-            if metadata:
-                # 先update再yield，受到SharedAsyncGeneratorManager的影响finally内的语句无法按时执行
-                await self.cache_updater(query_kwargs, content, metadata)
-                logger.info(f"[{self.tag}] cache updated  ({format_kwargs(**query_kwargs)})")
-
-                yield metadata
-                yield content
-
-            else:
-                raise RuntimeError("no metadata")
-
-
-class ManyMediator(Mediator, Generic[T]):
-    def __init__(self, tag: str,
-                 cache_factory: Callable[[T_KWARGS], AsyncGenerator[Union[T, PixivRepoMetadata], None]],
-                 remote_factory: Callable[[T_KWARGS], AsyncGenerator[Union[T, PixivRepoMetadata], None]],
-                 cache_invalidator: Callable[[T_KWARGS], Awaitable[Any]],
-                 cache_appender: Callable[[T_KWARGS, List[T], Optional[PixivRepoMetadata]], Awaitable[Any]]):
-        self.tag = tag
-        self.cache_factory = cache_factory
-        self.remote_factory = remote_factory
-        self.cache_invalidator = cache_invalidator
-        self.cache_appender = cache_appender
-
-    async def _load_many_from_local_and_remote_and_append(self, query_kwargs: T_KWARGS,
-                                                          max_item: int,
-                                                          max_page: int):
-        loaded_items = 0
-        loaded_pages = 0
-
-        # first load from cache
-        metadata = None
-        async for x in self.cache_factory(query_kwargs):
-            if isinstance(x, PixivRepoMetadata):
-                metadata = x
-                loaded_pages = metadata.pages
-            else:
-                loaded_items += 1
-
-            yield x
-
-            # check whether we approach limit
-            if loaded_items >= max_item or loaded_pages >= max_page:
-                break
-
-        logger.info(f"[{self.tag}] cache loaded  ({format_kwargs(**query_kwargs)})")
-
-        if loaded_items >= max_item or loaded_pages >= max_page:
-            return
-
-        # then check metadata["next_qs"] and load from remote
-        if metadata and metadata.next_qs:
-            async for x in self._load_many_from_remote_and_append(metadata.next_qs,
-                                                                  max_item - loaded_items, max_page - loaded_pages,
-                                                                  loaded_pages):
-                yield x
-
-    async def _load_many_from_remote_and_append(self, query_kwargs: T_KWARGS,
-                                                max_item: int,
-                                                max_page: int,
-                                                metadata_page_offset: int = 0):
-        loaded_items = 0
-        loaded_pages = 0
-
-        buffer = []
-
-        async for item in self.remote_factory(query_kwargs):
-            if isinstance(item, PixivRepoMetadata):
-                item.pages += metadata_page_offset
-                loaded_pages = item.pages
-
-                if len(buffer) > 0:
-                    await self.cache_appender(query_kwargs, buffer, item)
-                    logger.info(f"[{self.tag}] cache appended  ({format_kwargs(**query_kwargs)})")
-
-                    for x in buffer:
-                        yield x
-
-                    buffer.clear()
-
-                    # check whether we approach limit
-                    if loaded_items >= max_item or loaded_pages >= max_page:
-                        return
-
-                yield item
-            else:
-                loaded_items += 1
-                buffer.append(item)
-
-    async def mediate(self, query_kwargs: T_KWARGS,
-                      *, force_expiration: bool = False,
-                      max_item: int = 2 ** 31,
-                      max_page: int = 2 ** 31, ) -> AsyncGenerator[Union[T, PixivRepoMetadata], None]:
-        try:
-            if force_expiration:
-                raise NoSuchItemError()
-
-            async for x in self._load_many_from_local_and_remote_and_append(query_kwargs, max_item, max_page):
-                yield x
-        except NoSuchItemError:
-            logger.info(f"[{self.tag}] no cache  ({format_kwargs(**query_kwargs)})")
-            async for x in self._load_many_from_remote_and_append(query_kwargs, max_item, max_page):
-                yield x
-        except CacheExpiredError:
-            logger.info(f"[{self.tag}] cache expired  ({format_kwargs(**query_kwargs)})")
-            await self.cache_invalidator(query_kwargs)
-            logger.info(f"[{self.tag}] cache invalidated  ({format_kwargs(**query_kwargs)})")
-            async for x in self._load_many_from_remote_and_append(query_kwargs, max_item, max_page):
-                yield x
-
-
-class AppendMediator(ManyMediator):
-    def __init__(self, tag: str,
-                 cache_factory: Callable[[T_KWARGS], AsyncGenerator[Union[T, PixivRepoMetadata], None]],
-                 remote_factory: Callable[[T_KWARGS], AsyncGenerator[Union[T, PixivRepoMetadata], None]],
-                 cache_invalidator: Callable[[T_KWARGS], Awaitable[Any]],
-                 cache_appender: Callable[[T_KWARGS, List[T], Optional[PixivRepoMetadata]], Awaitable[Any]],
-                 front_cache_appender: Callable[[T_KWARGS, List[T], Optional[PixivRepoMetadata]], Awaitable[bool]]):
-        super().__init__(tag, cache_factory, remote_factory, cache_invalidator, cache_appender)
-        self.front_cache_appender = front_cache_appender
-
-    async def mediate(self, query_kwargs: Mapping[str, Any],
-                      *, force_expiration: bool = False,
-                      max_item: int = 2 ** 31,
-                      max_page: int = 2 ** 31) -> AsyncGenerator[Union[T, PixivRepoMetadata], None]:
-        try:
-            if force_expiration:
-                metadata = None
-                async for x in self.cache_factory(query_kwargs):
-                    if isinstance(x, PixivRepoMetadata):
-                        metadata = x
-                        break
-
-                if not metadata:
-                    raise NoSuchItemError()
-                else:
-                    raise CacheExpiredError(metadata)
-
-            async for x in self._load_many_from_local_and_remote_and_append(query_kwargs, max_item, max_page):
-                yield x
-        except NoSuchItemError:
-            logger.info(f"[{self.tag}] no cache  ({format_kwargs(**query_kwargs)})")
-            async for x in self._load_many_from_remote_and_append(query_kwargs, max_item, max_page):
-                yield x
-        except CacheExpiredError as e:
-            logger.info(f"[{self.tag}] cache expired  ({format_kwargs(**query_kwargs)})")
-            loaded_items = 0
-            loaded_pages = 0
-
-            # peek new bookmarks from remote
-            # then append them to local cache until we found some items already exist
-            buffer = []
-            metadata = e.metadata
-
-            async for x in self.remote_factory(query_kwargs):
-                if isinstance(x, PixivRepoMetadata):
-                    loaded_pages = x.pages
-                    # we don't use this metadata
-
-                    if len(buffer) > 0:
-                        metadata.update_time = datetime.now(timezone.utc)
-                        if await self.front_cache_appender(query_kwargs, buffer, metadata):
-                            break
-                        buffer = []
-
-                        # check whether we approach limit
-                        if loaded_items >= max_item or loaded_pages >= max_page:
-                            return
-                else:
-                    loaded_items += 1
-                    buffer.append(x)
-
-            async for x in self._load_many_from_local_and_remote_and_append(query_kwargs, max_item, max_page):
-                yield x
-
-
-__all__ = ("SingleMediator", "ManyMediator", "AppendMediator")
+from datetime import datetime, timezone
+from typing import List, AsyncGenerator, TypeVar, Union, Callable, Awaitable, Optional, Any, Mapping, Protocol, Generic
+
+from nonebot import logger
+
+from .errors import NoSuchItemError, CacheExpiredError
+from .models import PixivRepoMetadata
+from ...utils.format import format_kwargs
+
+T = TypeVar("T")
+
+T_KWARGS = Mapping[str, Any]
+
+
+class Mediator(Protocol[T]):
+    def mediate(self, query_kwargs: T_KWARGS, **kwargs) -> AsyncGenerator[Union[T, PixivRepoMetadata], None]:
+        ...
+
+
+class SingleMediator(Mediator, Generic[T]):
+    def __init__(self, tag: str,
+                 cache_factory: Callable[[T_KWARGS], AsyncGenerator[Union[T, PixivRepoMetadata], None]],
+                 remote_factory: Callable[[T_KWARGS], AsyncGenerator[Union[T, PixivRepoMetadata], None]],
+                 cache_updater: Callable[[T_KWARGS, T, Optional[PixivRepoMetadata]], Awaitable[Any]]):
+        self.tag = tag
+        self.cache_factory = cache_factory
+        self.remote_factory = remote_factory
+        self.cache_updater = cache_updater
+
+    async def mediate(self, query_kwargs: T_KWARGS,
+                      *, force_expiration: bool = False) -> AsyncGenerator[Union[T, PixivRepoMetadata], None]:
+        try:
+            if force_expiration:
+                raise NoSuchItemError()
+            async for x in self.cache_factory(query_kwargs):
+                yield x
+            logger.info(f"[{self.tag}] cache loaded  ({format_kwargs(**query_kwargs)})")
+        except (NoSuchItemError, CacheExpiredError):
+            logger.info(f"[{self.tag}] no cache or cache expired  ({format_kwargs(**query_kwargs)})")
+
+            content = None
+            metadata = None
+
+            async for x in self.remote_factory(query_kwargs):
+                if isinstance(x, PixivRepoMetadata):
+                    metadata = x
+                else:
+                    content = x
+
+            if metadata:
+                # 先update再yield，受到SharedAsyncGeneratorManager的影响finally内的语句无法按时执行
+                await self.cache_updater(query_kwargs, content, metadata)
+                logger.info(f"[{self.tag}] cache updated  ({format_kwargs(**query_kwargs)})")
+
+                yield metadata
+                yield content
+
+            else:
+                raise RuntimeError("no metadata")
+
+
+class ManyMediator(Mediator, Generic[T]):
+    def __init__(self, tag: str,
+                 cache_factory: Callable[[T_KWARGS], AsyncGenerator[Union[T, PixivRepoMetadata], None]],
+                 remote_factory: Callable[[T_KWARGS], AsyncGenerator[Union[T, PixivRepoMetadata], None]],
+                 cache_invalidator: Callable[[T_KWARGS], Awaitable[Any]],
+                 cache_appender: Callable[[T_KWARGS, List[T], Optional[PixivRepoMetadata]], Awaitable[Any]]):
+        self.tag = tag
+        self.cache_factory = cache_factory
+        self.remote_factory = remote_factory
+        self.cache_invalidator = cache_invalidator
+        self.cache_appender = cache_appender
+
+    async def _load_many_from_local_and_remote_and_append(self, query_kwargs: T_KWARGS,
+                                                          max_item: int,
+                                                          max_page: int):
+        loaded_items = 0
+        loaded_pages = 0
+
+        # first load from cache
+        metadata = None
+        async for x in self.cache_factory(query_kwargs):
+            if isinstance(x, PixivRepoMetadata):
+                metadata = x
+                loaded_pages = metadata.pages
+            else:
+                loaded_items += 1
+
+            yield x
+
+            # check whether we approach limit
+            if loaded_items >= max_item or loaded_pages >= max_page:
+                break
+
+        logger.info(f"[{self.tag}] cache loaded  ({format_kwargs(**query_kwargs)})")
+
+        if loaded_items >= max_item or loaded_pages >= max_page:
+            return
+
+        # then check metadata["next_qs"] and load from remote
+        if metadata and metadata.next_qs:
+            async for x in self._load_many_from_remote_and_append(metadata.next_qs,
+                                                                  max_item - loaded_items, max_page - loaded_pages,
+                                                                  loaded_pages):
+                yield x
+
+    async def _load_many_from_remote_and_append(self, query_kwargs: T_KWARGS,
+                                                max_item: int,
+                                                max_page: int,
+                                                metadata_page_offset: int = 0):
+        loaded_items = 0
+        loaded_pages = 0
+
+        buffer = []
+
+        async for item in self.remote_factory(query_kwargs):
+            if isinstance(item, PixivRepoMetadata):
+                item.pages += metadata_page_offset
+                loaded_pages = item.pages
+
+                if len(buffer) > 0:
+                    await self.cache_appender(query_kwargs, buffer, item)
+                    logger.info(f"[{self.tag}] cache appended  ({format_kwargs(**query_kwargs)})")
+
+                    for x in buffer:
+                        yield x
+
+                    buffer.clear()
+
+                    # check whether we approach limit
+                    if loaded_items >= max_item or loaded_pages >= max_page:
+                        return
+
+                yield item
+            else:
+                loaded_items += 1
+                buffer.append(item)
+
+    async def mediate(self, query_kwargs: T_KWARGS,
+                      *, force_expiration: bool = False,
+                      max_item: int = 2 ** 31,
+                      max_page: int = 2 ** 31, ) -> AsyncGenerator[Union[T, PixivRepoMetadata], None]:
+        try:
+            if force_expiration:
+                raise NoSuchItemError()
+
+            async for x in self._load_many_from_local_and_remote_and_append(query_kwargs, max_item, max_page):
+                yield x
+        except NoSuchItemError:
+            logger.info(f"[{self.tag}] no cache  ({format_kwargs(**query_kwargs)})")
+            async for x in self._load_many_from_remote_and_append(query_kwargs, max_item, max_page):
+                yield x
+        except CacheExpiredError:
+            logger.info(f"[{self.tag}] cache expired  ({format_kwargs(**query_kwargs)})")
+            await self.cache_invalidator(query_kwargs)
+            logger.info(f"[{self.tag}] cache invalidated  ({format_kwargs(**query_kwargs)})")
+            async for x in self._load_many_from_remote_and_append(query_kwargs, max_item, max_page):
+                yield x
+
+
+class AppendMediator(ManyMediator):
+    def __init__(self, tag: str,
+                 cache_factory: Callable[[T_KWARGS], AsyncGenerator[Union[T, PixivRepoMetadata], None]],
+                 remote_factory: Callable[[T_KWARGS], AsyncGenerator[Union[T, PixivRepoMetadata], None]],
+                 cache_invalidator: Callable[[T_KWARGS], Awaitable[Any]],
+                 cache_appender: Callable[[T_KWARGS, List[T], Optional[PixivRepoMetadata]], Awaitable[Any]],
+                 front_cache_appender: Callable[[T_KWARGS, List[T], Optional[PixivRepoMetadata]], Awaitable[bool]]):
+        super().__init__(tag, cache_factory, remote_factory, cache_invalidator, cache_appender)
+        self.front_cache_appender = front_cache_appender
+
+    async def mediate(self, query_kwargs: Mapping[str, Any],
+                      *, force_expiration: bool = False,
+                      max_item: int = 2 ** 31,
+                      max_page: int = 2 ** 31) -> AsyncGenerator[Union[T, PixivRepoMetadata], None]:
+        try:
+            if force_expiration:
+                metadata = None
+                async for x in self.cache_factory(query_kwargs):
+                    if isinstance(x, PixivRepoMetadata):
+                        metadata = x
+                        break
+
+                if not metadata:
+                    raise NoSuchItemError()
+                else:
+                    raise CacheExpiredError(metadata)
+
+            async for x in self._load_many_from_local_and_remote_and_append(query_kwargs, max_item, max_page):
+                yield x
+        except NoSuchItemError:
+            logger.info(f"[{self.tag}] no cache  ({format_kwargs(**query_kwargs)})")
+            async for x in self._load_many_from_remote_and_append(query_kwargs, max_item, max_page):
+                yield x
+        except CacheExpiredError as e:
+            logger.info(f"[{self.tag}] cache expired  ({format_kwargs(**query_kwargs)})")
+            loaded_items = 0
+            loaded_pages = 0
+
+            # peek new bookmarks from remote
+            # then append them to local cache until we found some items already exist
+            buffer = []
+            metadata = e.metadata
+
+            async for x in self.remote_factory(query_kwargs):
+                if isinstance(x, PixivRepoMetadata):
+                    loaded_pages = x.pages
+                    # we don't use this metadata
+
+                    if len(buffer) > 0:
+                        metadata.update_time = datetime.now(timezone.utc)
+                        if await self.front_cache_appender(query_kwargs, buffer, metadata):
+                            break
+                        buffer = []
+
+                        # check whether we approach limit
+                        if loaded_items >= max_item or loaded_pages >= max_page:
+                            return
+                else:
+                    loaded_items += 1
+                    buffer.append(x)
+
+            async for x in self._load_many_from_local_and_remote_and_append(query_kwargs, max_item, max_page):
+                yield x
+
+
+__all__ = ("SingleMediator", "ManyMediator", "AppendMediator")
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator_repo.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/mediator_repo.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,430 +1,430 @@
-from datetime import datetime, timedelta
-from typing import Any, AsyncGenerator, Union
-
-from frozendict import frozendict
-from nonebot import logger
-from pydantic import BaseModel
-
-from nonebot_plugin_pixivbot.config import Config
-from nonebot_plugin_pixivbot.enums import RankingMode
-from nonebot_plugin_pixivbot.global_context import context
-from nonebot_plugin_pixivbot.model import Illust, User, UserPreview
-from nonebot_plugin_pixivbot.utils.shared_agen import SharedAsyncGeneratorManager
-from .base import PixivRepo
-from .enums import PixivResType, CacheStrategy
-from .lazy_illust import LazyIllust
-from .local_repo import LocalPixivRepo
-from .mediator import SingleMediator, AppendMediator, ManyMediator
-from .models import PixivRepoMetadata
-from .remote_repo import RemotePixivRepo
-from ...utils.format import format_kwargs
-
-conf = context.require(Config)
-local = context.require(LocalPixivRepo)
-remote = context.require(RemotePixivRepo)
-
-
-class SharedAgenIdentifier(BaseModel):
-    type: PixivResType
-    kwargs: frozendict[str, Any]
-
-    def __init__(self, type: PixivResType, **kwargs):
-        super().__init__(type=type, kwargs=frozendict(kwargs))
-
-    def __str__(self):
-        return f"({self.type.name} {format_kwargs(**self.kwargs)})"
-
-    class Config:
-        frozen = True
-
-
-class PixivSharedAsyncGeneratorManager(SharedAsyncGeneratorManager[SharedAgenIdentifier, Any]):
-    log_tag = "pixiv_shared_agen"
-
-    mediators = {
-        "illust_detail": SingleMediator(
-            "illust_detail",
-            cache_factory=lambda kwargs: local.illust_detail(kwargs["illust_id"]),
-            remote_factory=lambda kwargs: remote.illust_detail(**kwargs),
-            cache_updater=lambda kwargs, data, meta: local.update_illust_detail(data, meta)
-        ),
-        "user_detail": SingleMediator(
-            "user_detail",
-            cache_factory=lambda kwargs: local.user_detail(kwargs["user_id"]),
-            remote_factory=lambda kwargs: remote.user_detail(**kwargs),
-            cache_updater=lambda kwargs, data, meta: local.update_user_detail(data, meta)
-        ),
-        "search_illust": AppendMediator(
-            "search_illust",
-            cache_factory=lambda kwargs: local.search_illust(kwargs["word"]),
-            remote_factory=lambda kwargs: remote.search_illust(**kwargs),
-            cache_invalidator=lambda kwargs: local.invalidate_search_illust(kwargs["word"]),
-            cache_appender=lambda kwargs, data, meta: local.append_search_illust(kwargs["word"], data, meta),
-            front_cache_appender=lambda kwargs, data, meta: local.append_search_illust(kwargs["word"], data, meta),
-        ),
-        "search_user": AppendMediator(
-            "search_user",
-            cache_factory=lambda kwargs: local.search_user(kwargs["word"]),
-            remote_factory=lambda kwargs: remote.search_user(**kwargs),
-            cache_invalidator=lambda kwargs: local.invalidate_search_user(kwargs["word"]),
-            cache_appender=lambda kwargs, data, meta: local.append_search_user(kwargs["word"], data, meta),
-            front_cache_appender=lambda kwargs, data, meta: local.append_search_user(kwargs["word"], data, meta),
-        ),
-        "user_illusts": AppendMediator(
-            "user_illusts",
-            cache_factory=lambda kwargs: local.user_illusts(kwargs["user_id"]),
-            remote_factory=lambda kwargs: remote.user_illusts(**kwargs),
-            cache_invalidator=lambda kwargs: local.invalidate_user_illusts(kwargs["user_id"]),
-            cache_appender=lambda kwargs, data, meta: local.append_user_illusts(kwargs["user_id"], data, meta),
-            front_cache_appender=lambda kwargs, data, meta: local.append_user_illusts(kwargs["user_id"], data, meta,
-                                                                                      append_at_begin=True),
-        ),
-        "user_bookmarks": AppendMediator(
-            "user_bookmarks",
-            cache_factory=lambda kwargs: local.user_bookmarks(kwargs["user_id"]),
-            remote_factory=lambda kwargs: remote.user_bookmarks(**kwargs),
-            cache_invalidator=lambda kwargs: local.invalidate_user_bookmarks(kwargs["user_id"]),
-            cache_appender=lambda kwargs, data, meta: local.append_user_bookmarks(kwargs["user_id"], data, meta),
-            front_cache_appender=lambda kwargs, data, meta: local.append_user_bookmarks(kwargs["user_id"], data, meta,
-                                                                                        append_at_begin=True),
-        ),
-        "recommended_illusts": ManyMediator(
-            "recommended_illusts",
-            cache_factory=lambda kwargs: local.recommended_illusts(),
-            remote_factory=lambda kwargs: remote.recommended_illusts(**kwargs),
-            cache_invalidator=lambda kwargs: local.invalidate_recommended_illusts(),
-            cache_appender=lambda kwargs, data, meta: local.append_recommended_illusts(data, meta),
-        ),
-        "related_illusts": ManyMediator(
-            "related_illusts",
-            cache_factory=lambda kwargs: local.related_illusts(kwargs["illust_id"]),
-            remote_factory=lambda kwargs: remote.related_illusts(**kwargs),
-            cache_invalidator=lambda kwargs: local.invalidate_related_illusts(kwargs["illust_id"]),
-            cache_appender=lambda kwargs, data, meta: local.append_related_illusts(kwargs["illust_id"], data, meta),
-        ),
-        "illust_ranking": ManyMediator(
-            "illust_ranking",
-            cache_factory=lambda kwargs: local.illust_ranking(kwargs["mode"]),
-            remote_factory=lambda kwargs: remote.illust_ranking(**kwargs),
-            cache_invalidator=lambda kwargs: local.invalidate_illust_ranking(kwargs["mode"]),
-            cache_appender=lambda kwargs, data, meta: local.append_illust_ranking(kwargs["mode"], data, meta),
-        ),
-        "image": SingleMediator(
-            "image",
-            cache_factory=lambda kwargs: local.image(kwargs["illust"], kwargs["page"]),
-            remote_factory=lambda kwargs: remote.image(**kwargs),
-            cache_updater=lambda kwargs, data, meta: local.update_image(kwargs["illust"].id, kwargs["page"], data, meta)
-        ),
-    }
-
-    def illust_detail_factory(self, illust_id: int,
-                              cache_strategy: CacheStrategy) -> AsyncGenerator[Illust, None]:
-        return self.mediators["illust_detail"].mediate(
-            {"illust_id": illust_id},
-            force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
-        )
-
-    def user_detail_factory(self, user_id: int,
-                            cache_strategy: CacheStrategy) -> AsyncGenerator[User, None]:
-        return self.mediators["user_detail"].mediate(
-            query_kwargs={"user_id": user_id},
-            force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
-        )
-
-    def search_illust_factory(self, word: str,
-                              cache_strategy: CacheStrategy) -> AsyncGenerator[LazyIllust, None]:
-        return self.mediators["search_illust"].mediate(
-            query_kwargs={"word": word},
-            max_item=conf.pixiv_random_illust_max_item,
-            max_page=conf.pixiv_random_illust_max_page,
-            force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
-        )
-
-    def search_user_factory(self, word: str,
-                            cache_strategy: CacheStrategy) -> AsyncGenerator[User, None]:
-        return self.mediators["search_user"].mediate(
-            query_kwargs={"word": word},
-            max_page=1,
-            force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
-        )
-
-    def user_illusts_factory(self, user_id: int,
-                             cache_strategy: CacheStrategy) -> AsyncGenerator[LazyIllust, None]:
-        return self.mediators["user_illusts"].mediate(
-            query_kwargs={"user_id": user_id},
-            max_item=conf.pixiv_random_user_illust_max_item,
-            max_page=conf.pixiv_random_user_illust_max_page,
-            force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
-        )
-
-    def user_bookmarks_factory(self, user_id: int,
-                               cache_strategy: CacheStrategy) -> AsyncGenerator[LazyIllust, None]:
-        return self.mediators["user_bookmarks"].mediate(
-            query_kwargs={"user_id": user_id},
-            max_item=conf.pixiv_random_bookmark_max_item,
-            max_page=conf.pixiv_random_bookmark_max_page,
-            force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
-        )
-
-    def recommended_illusts_factory(self, cache_strategy: CacheStrategy) -> AsyncGenerator[LazyIllust, None]:
-        return self.mediators["recommended_illusts"].mediate(
-            query_kwargs={},
-            max_item=conf.pixiv_random_recommended_illust_max_item,
-            max_page=conf.pixiv_random_recommended_illust_max_page,
-            force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
-        )
-
-    def related_illusts_factory(self, illust_id: int,
-                                cache_strategy: CacheStrategy) -> AsyncGenerator[LazyIllust, None]:
-        return self.mediators["related_illusts"].mediate(
-            query_kwargs={"illust_id": illust_id},
-            max_item=conf.pixiv_random_related_illust_max_item,
-            max_page=conf.pixiv_random_related_illust_max_page,
-            force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
-        )
-
-    def illust_ranking_factory(self, mode: RankingMode,
-                               cache_strategy: CacheStrategy) -> AsyncGenerator[LazyIllust, None]:
-        return self.mediators["illust_ranking"].mediate(
-            query_kwargs={"mode": mode},
-            max_item=conf.pixiv_ranking_fetch_item,
-            force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
-        )
-
-    def image_factory(self, illust_id: int, illust: Illust, page: int,
-                      cache_strategy: CacheStrategy) -> AsyncGenerator[bytes, None]:
-        return self.mediators["image"].mediate(
-            query_kwargs={"illust": illust, "page": page},
-            force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
-        )
-
-    factories = {
-        PixivResType.ILLUST_DETAIL: illust_detail_factory,
-        PixivResType.USER_DETAIL: user_detail_factory,
-        PixivResType.SEARCH_ILLUST: search_illust_factory,
-        PixivResType.SEARCH_USER: search_user_factory,
-        PixivResType.USER_ILLUSTS: user_illusts_factory,
-        PixivResType.USER_BOOKMARKS: user_bookmarks_factory,
-        PixivResType.RECOMMENDED_ILLUSTS: recommended_illusts_factory,
-        PixivResType.RELATED_ILLUSTS: related_illusts_factory,
-        PixivResType.ILLUST_RANKING: illust_ranking_factory,
-        PixivResType.IMAGE: image_factory,
-    }
-
-    def agen(self, identifier: SharedAgenIdentifier,
-             cache_strategy: CacheStrategy, **kwargs) -> AsyncGenerator[Any, None]:
-        if identifier.type in self.factories:
-            merged_kwargs = identifier.kwargs | kwargs
-            # noinspection PyTypeChecker
-            return self.factories[identifier.type](self, cache_strategy=cache_strategy, **merged_kwargs)
-        else:
-            raise ValueError("invalid identifier: " + str(identifier))
-
-    expires_in = {
-        PixivResType.ILLUST_DETAIL: timedelta(seconds=context.require(Config).pixiv_illust_detail_cache_expires_in),
-        PixivResType.USER_DETAIL: timedelta(seconds=context.require(Config).pixiv_user_detail_cache_expires_in),
-        PixivResType.SEARCH_ILLUST: timedelta(seconds=context.require(Config).pixiv_search_illust_cache_expires_in),
-        PixivResType.SEARCH_USER: timedelta(seconds=context.require(Config).pixiv_search_user_cache_expires_in),
-        PixivResType.USER_ILLUSTS: timedelta(seconds=context.require(Config).pixiv_user_illusts_cache_expires_in),
-        PixivResType.USER_BOOKMARKS: timedelta(seconds=context.require(Config).pixiv_user_bookmarks_cache_expires_in),
-        PixivResType.RECOMMENDED_ILLUSTS: timedelta(seconds=context.require(Config).pixiv_other_cache_expires_in),
-        PixivResType.RELATED_ILLUSTS: timedelta(seconds=context.require(Config).pixiv_related_illusts_cache_expires_in),
-        PixivResType.ILLUST_RANKING: timedelta(seconds=context.require(Config).pixiv_illust_ranking_cache_expires_in),
-        PixivResType.IMAGE: timedelta(seconds=context.require(Config).pixiv_download_cache_expires_in),
-    }
-
-    def calc_expires_time(self, identifier: SharedAgenIdentifier, update_time: datetime) -> datetime:
-        if identifier.type in self.factories:
-            return update_time + self.expires_in[identifier.type]
-        else:
-            raise ValueError("invalid identifier: " + str(identifier))
-
-    async def on_agen_next(self, identifier: SharedAgenIdentifier, item: Any):
-        await super().on_agen_next(identifier, item)
-        if isinstance(item, PixivRepoMetadata) and not self.get_expires_time(identifier):
-            expires_time = self.calc_expires_time(identifier, item.update_time)
-            await self.set_expires_time(identifier, expires_time.timestamp())
-
-
-@context.root.register_singleton()
-class MediatorPixivRepo(PixivRepo):
-    def __init__(self):
-        self.shared_agen_mgr = PixivSharedAsyncGeneratorManager()
-
-    async def invalidate_cache(self):
-        await self.shared_agen_mgr.invalidate_all()
-        await local.invalidate_all()
-
-    async def illust_detail(self, illust_id: int,
-                            cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[Illust, None]:
-        logger.debug(f"[mediator] illust_detail {illust_id} "
-                     f"cache_strategy={cache_strategy.name}")
-        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.ILLUST_DETAIL, illust_id=illust_id),
-                                            cache_strategy) as gen:
-            data = None
-            async for x in gen:
-                if not isinstance(x, PixivRepoMetadata):
-                    data = x
-
-        # 保证shared_agen能正常结束
-        if data is not None:
-            yield data
-
-    async def user_detail(self, user_id: int,
-                          cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[User, None]:
-        logger.debug(f"[mediator] user_detail {user_id} "
-                     f"cache_strategy={cache_strategy.name}")
-        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.USER_DETAIL, user_id=user_id),
-                                            cache_strategy) as gen:
-            data = None
-            async for x in gen:
-                if not isinstance(x, PixivRepoMetadata):
-                    data = x
-
-        # 保证shared_agen能正常结束
-        if data is not None:
-            yield data
-
-    async def search_illust(self, word: str,
-                            cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[LazyIllust, None]:
-        logger.debug(f"[mediator] search_illust {word} "
-                     f"cache_strategy={cache_strategy.name}")
-        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.SEARCH_ILLUST, word=word),
-                                            cache_strategy) as gen:
-            async for x in gen:
-                if not isinstance(x, PixivRepoMetadata):
-                    yield x
-
-    async def search_user(self, word: str,
-                          cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[User, None]:
-        logger.debug(f"[mediator] search_user {word} "
-                     f"cache_strategy={cache_strategy.name}")
-        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.SEARCH_USER, word=word),
-                                            cache_strategy) as gen:
-            async for x in gen:
-                if not isinstance(x, PixivRepoMetadata):
-                    yield x
-
-    async def user_bookmarks(self, user_id: int = 0,
-                             cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[LazyIllust, None]:
-        logger.debug(f"[mediator] user_bookmarks {user_id} "
-                     f"cache_strategy={cache_strategy.name}")
-        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.USER_BOOKMARKS, user_id=user_id),
-                                            cache_strategy) as gen:
-            async for x in gen:
-                if not isinstance(x, PixivRepoMetadata):
-                    yield x
-
-    async def user_illusts(self, user_id: int = 0,
-                           cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[LazyIllust, None]:
-        logger.debug(f"[mediator] user_illusts {user_id} "
-                     f"cache_strategy={cache_strategy.name}")
-        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.USER_ILLUSTS, user_id=user_id),
-                                            cache_strategy) as gen:
-            async for x in gen:
-                if not isinstance(x, PixivRepoMetadata):
-                    yield x
-
-    async def _contact_user_illusts_with_preview(self, user_preview: UserPreview,
-                                                 cache_strategy: CacheStrategy = CacheStrategy.NORMAL) \
-            -> AsyncGenerator[LazyIllust, None]:
-        for illust in user_preview.illusts:
-            yield LazyIllust(illust.id, illust)
-
-        ids = {x.id for x in user_preview.illusts}
-
-        if len(user_preview.illusts) >= 3:
-            gen = self.user_illusts(user_preview.user.id, cache_strategy)
-
-            async for x in gen:
-                if x.id not in ids:
-                    yield x
-
-    async def user_following_illusts(self, user_id: int,
-                                     cache_strategy: CacheStrategy = CacheStrategy.NORMAL) \
-            -> AsyncGenerator[LazyIllust, None]:
-        logger.debug(f"[mediator] user_following_illusts {user_id} "
-                     f"cache_strategy={cache_strategy.name}")
-
-        n = 0
-        gen = []
-        peeked = []
-
-        async for user_preview in remote.user_following_with_preview(user_id):
-            if not isinstance(user_preview, PixivRepoMetadata):
-                n += 1
-                gen.append(self._contact_user_illusts_with_preview(user_preview, cache_strategy))
-                peeked.append(None)
-
-        try:
-            while True:
-                select = -1
-                for i in range(n):
-                    try:
-                        if not peeked[i]:
-                            peeked[i] = await gen[i].__anext__()
-
-                        if select == -1 or peeked[i].create_date > peeked[select].create_date:
-                            select = i
-                    except StopAsyncIteration:
-                        pass
-
-                if select == -1:
-                    break
-
-                yield peeked[select]
-                peeked[select] = None
-        except GeneratorExit:
-            for gen in gen:
-                await gen.aclose()
-
-    async def recommended_illusts(self, cache_strategy: CacheStrategy = CacheStrategy.NORMAL) \
-            -> AsyncGenerator[LazyIllust, None]:
-        logger.debug(f"[mediator] recommended_illusts "
-                     f"cache_strategy={cache_strategy.name}")
-        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.RECOMMENDED_ILLUSTS),
-                                            cache_strategy) as gen:
-            async for x in gen:
-                if not isinstance(x, PixivRepoMetadata):
-                    yield x
-
-    async def related_illusts(self, illust_id: int,
-                              cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[LazyIllust, None]:
-        logger.debug(f"[mediator] related_illusts {illust_id} "
-                     f"cache_strategy={cache_strategy.name}")
-        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.RELATED_ILLUSTS, illust_id=illust_id),
-                                            cache_strategy) as gen:
-            async for x in gen:
-                if not isinstance(x, PixivRepoMetadata):
-                    yield x
-
-    async def illust_ranking(self, mode: Union[str, RankingMode],
-                             cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[LazyIllust, None]:
-        if isinstance(mode, str):
-            mode = RankingMode[mode]
-
-        logger.debug(f"[mediator] illust_ranking {mode} "
-                     f"cache_strategy={cache_strategy.name}")
-        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.ILLUST_RANKING, mode=mode),
-                                            cache_strategy) as gen:
-            async for x in gen:
-                if not isinstance(x, PixivRepoMetadata):
-                    yield x
-
-    async def image(self, illust: Illust, page: int = 0,
-                    cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[bytes, None]:
-        logger.debug(f"[mediator] image {illust.id}[{page}] "
-                     f"cache_strategy={cache_strategy.name}")
-        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.IMAGE, illust_id=illust.id, page=page),
-                                            cache_strategy, illust=illust) as gen:
-            data = None
-            async for x in gen:
-                if not isinstance(x, PixivRepoMetadata):
-                    data = x
-
-        # 保证shared_agen能正常退出
-        if data is not None:
-            yield data
-
-
-__all__ = ('MediatorPixivRepo',)
+from datetime import datetime, timedelta
+from typing import Any, AsyncGenerator, Union
+
+from frozendict import frozendict
+from nonebot import logger
+from pydantic import BaseModel
+
+from nonebot_plugin_pixivbot.config import Config
+from nonebot_plugin_pixivbot.enums import RankingMode
+from nonebot_plugin_pixivbot.global_context import context
+from nonebot_plugin_pixivbot.model import Illust, User, UserPreview
+from nonebot_plugin_pixivbot.utils.shared_agen import SharedAsyncGeneratorManager
+from .base import PixivRepo
+from .enums import PixivResType, CacheStrategy
+from .lazy_illust import LazyIllust
+from .local_repo import LocalPixivRepo
+from .mediator import SingleMediator, AppendMediator, ManyMediator
+from .models import PixivRepoMetadata
+from .remote_repo import RemotePixivRepo
+from ...utils.format import format_kwargs
+
+conf = context.require(Config)
+local = context.require(LocalPixivRepo)
+remote = context.require(RemotePixivRepo)
+
+
+class SharedAgenIdentifier(BaseModel):
+    type: PixivResType
+    kwargs: frozendict[str, Any]
+
+    def __init__(self, type: PixivResType, **kwargs):
+        super().__init__(type=type, kwargs=frozendict(kwargs))
+
+    def __str__(self):
+        return f"({self.type.name} {format_kwargs(**self.kwargs)})"
+
+    class Config:
+        frozen = True
+
+
+class PixivSharedAsyncGeneratorManager(SharedAsyncGeneratorManager[SharedAgenIdentifier, Any]):
+    log_tag = "pixiv_shared_agen"
+
+    mediators = {
+        "illust_detail": SingleMediator(
+            "illust_detail",
+            cache_factory=lambda kwargs: local.illust_detail(kwargs["illust_id"]),
+            remote_factory=lambda kwargs: remote.illust_detail(**kwargs),
+            cache_updater=lambda kwargs, data, meta: local.update_illust_detail(data, meta)
+        ),
+        "user_detail": SingleMediator(
+            "user_detail",
+            cache_factory=lambda kwargs: local.user_detail(kwargs["user_id"]),
+            remote_factory=lambda kwargs: remote.user_detail(**kwargs),
+            cache_updater=lambda kwargs, data, meta: local.update_user_detail(data, meta)
+        ),
+        "search_illust": AppendMediator(
+            "search_illust",
+            cache_factory=lambda kwargs: local.search_illust(kwargs["word"]),
+            remote_factory=lambda kwargs: remote.search_illust(**kwargs),
+            cache_invalidator=lambda kwargs: local.invalidate_search_illust(kwargs["word"]),
+            cache_appender=lambda kwargs, data, meta: local.append_search_illust(kwargs["word"], data, meta),
+            front_cache_appender=lambda kwargs, data, meta: local.append_search_illust(kwargs["word"], data, meta),
+        ),
+        "search_user": AppendMediator(
+            "search_user",
+            cache_factory=lambda kwargs: local.search_user(kwargs["word"]),
+            remote_factory=lambda kwargs: remote.search_user(**kwargs),
+            cache_invalidator=lambda kwargs: local.invalidate_search_user(kwargs["word"]),
+            cache_appender=lambda kwargs, data, meta: local.append_search_user(kwargs["word"], data, meta),
+            front_cache_appender=lambda kwargs, data, meta: local.append_search_user(kwargs["word"], data, meta),
+        ),
+        "user_illusts": AppendMediator(
+            "user_illusts",
+            cache_factory=lambda kwargs: local.user_illusts(kwargs["user_id"]),
+            remote_factory=lambda kwargs: remote.user_illusts(**kwargs),
+            cache_invalidator=lambda kwargs: local.invalidate_user_illusts(kwargs["user_id"]),
+            cache_appender=lambda kwargs, data, meta: local.append_user_illusts(kwargs["user_id"], data, meta),
+            front_cache_appender=lambda kwargs, data, meta: local.append_user_illusts(kwargs["user_id"], data, meta,
+                                                                                      append_at_begin=True),
+        ),
+        "user_bookmarks": AppendMediator(
+            "user_bookmarks",
+            cache_factory=lambda kwargs: local.user_bookmarks(kwargs["user_id"]),
+            remote_factory=lambda kwargs: remote.user_bookmarks(**kwargs),
+            cache_invalidator=lambda kwargs: local.invalidate_user_bookmarks(kwargs["user_id"]),
+            cache_appender=lambda kwargs, data, meta: local.append_user_bookmarks(kwargs["user_id"], data, meta),
+            front_cache_appender=lambda kwargs, data, meta: local.append_user_bookmarks(kwargs["user_id"], data, meta,
+                                                                                        append_at_begin=True),
+        ),
+        "recommended_illusts": ManyMediator(
+            "recommended_illusts",
+            cache_factory=lambda kwargs: local.recommended_illusts(),
+            remote_factory=lambda kwargs: remote.recommended_illusts(**kwargs),
+            cache_invalidator=lambda kwargs: local.invalidate_recommended_illusts(),
+            cache_appender=lambda kwargs, data, meta: local.append_recommended_illusts(data, meta),
+        ),
+        "related_illusts": ManyMediator(
+            "related_illusts",
+            cache_factory=lambda kwargs: local.related_illusts(kwargs["illust_id"]),
+            remote_factory=lambda kwargs: remote.related_illusts(**kwargs),
+            cache_invalidator=lambda kwargs: local.invalidate_related_illusts(kwargs["illust_id"]),
+            cache_appender=lambda kwargs, data, meta: local.append_related_illusts(kwargs["illust_id"], data, meta),
+        ),
+        "illust_ranking": ManyMediator(
+            "illust_ranking",
+            cache_factory=lambda kwargs: local.illust_ranking(kwargs["mode"]),
+            remote_factory=lambda kwargs: remote.illust_ranking(**kwargs),
+            cache_invalidator=lambda kwargs: local.invalidate_illust_ranking(kwargs["mode"]),
+            cache_appender=lambda kwargs, data, meta: local.append_illust_ranking(kwargs["mode"], data, meta),
+        ),
+        "image": SingleMediator(
+            "image",
+            cache_factory=lambda kwargs: local.image(kwargs["illust"], kwargs["page"]),
+            remote_factory=lambda kwargs: remote.image(**kwargs),
+            cache_updater=lambda kwargs, data, meta: local.update_image(kwargs["illust"].id, kwargs["page"], data, meta)
+        ),
+    }
+
+    def illust_detail_factory(self, illust_id: int,
+                              cache_strategy: CacheStrategy) -> AsyncGenerator[Illust, None]:
+        return self.mediators["illust_detail"].mediate(
+            {"illust_id": illust_id},
+            force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
+        )
+
+    def user_detail_factory(self, user_id: int,
+                            cache_strategy: CacheStrategy) -> AsyncGenerator[User, None]:
+        return self.mediators["user_detail"].mediate(
+            query_kwargs={"user_id": user_id},
+            force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
+        )
+
+    def search_illust_factory(self, word: str,
+                              cache_strategy: CacheStrategy) -> AsyncGenerator[LazyIllust, None]:
+        return self.mediators["search_illust"].mediate(
+            query_kwargs={"word": word},
+            max_item=conf.pixiv_random_illust_max_item,
+            max_page=conf.pixiv_random_illust_max_page,
+            force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
+        )
+
+    def search_user_factory(self, word: str,
+                            cache_strategy: CacheStrategy) -> AsyncGenerator[User, None]:
+        return self.mediators["search_user"].mediate(
+            query_kwargs={"word": word},
+            max_page=1,
+            force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
+        )
+
+    def user_illusts_factory(self, user_id: int,
+                             cache_strategy: CacheStrategy) -> AsyncGenerator[LazyIllust, None]:
+        return self.mediators["user_illusts"].mediate(
+            query_kwargs={"user_id": user_id},
+            max_item=conf.pixiv_random_user_illust_max_item,
+            max_page=conf.pixiv_random_user_illust_max_page,
+            force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
+        )
+
+    def user_bookmarks_factory(self, user_id: int,
+                               cache_strategy: CacheStrategy) -> AsyncGenerator[LazyIllust, None]:
+        return self.mediators["user_bookmarks"].mediate(
+            query_kwargs={"user_id": user_id},
+            max_item=conf.pixiv_random_bookmark_max_item,
+            max_page=conf.pixiv_random_bookmark_max_page,
+            force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
+        )
+
+    def recommended_illusts_factory(self, cache_strategy: CacheStrategy) -> AsyncGenerator[LazyIllust, None]:
+        return self.mediators["recommended_illusts"].mediate(
+            query_kwargs={},
+            max_item=conf.pixiv_random_recommended_illust_max_item,
+            max_page=conf.pixiv_random_recommended_illust_max_page,
+            force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
+        )
+
+    def related_illusts_factory(self, illust_id: int,
+                                cache_strategy: CacheStrategy) -> AsyncGenerator[LazyIllust, None]:
+        return self.mediators["related_illusts"].mediate(
+            query_kwargs={"illust_id": illust_id},
+            max_item=conf.pixiv_random_related_illust_max_item,
+            max_page=conf.pixiv_random_related_illust_max_page,
+            force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
+        )
+
+    def illust_ranking_factory(self, mode: RankingMode,
+                               cache_strategy: CacheStrategy) -> AsyncGenerator[LazyIllust, None]:
+        return self.mediators["illust_ranking"].mediate(
+            query_kwargs={"mode": mode},
+            max_item=conf.pixiv_ranking_fetch_item,
+            force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
+        )
+
+    def image_factory(self, illust_id: int, illust: Illust, page: int,
+                      cache_strategy: CacheStrategy) -> AsyncGenerator[bytes, None]:
+        return self.mediators["image"].mediate(
+            query_kwargs={"illust": illust, "page": page},
+            force_expiration=cache_strategy == CacheStrategy.FORCE_EXPIRATION,
+        )
+
+    factories = {
+        PixivResType.ILLUST_DETAIL: illust_detail_factory,
+        PixivResType.USER_DETAIL: user_detail_factory,
+        PixivResType.SEARCH_ILLUST: search_illust_factory,
+        PixivResType.SEARCH_USER: search_user_factory,
+        PixivResType.USER_ILLUSTS: user_illusts_factory,
+        PixivResType.USER_BOOKMARKS: user_bookmarks_factory,
+        PixivResType.RECOMMENDED_ILLUSTS: recommended_illusts_factory,
+        PixivResType.RELATED_ILLUSTS: related_illusts_factory,
+        PixivResType.ILLUST_RANKING: illust_ranking_factory,
+        PixivResType.IMAGE: image_factory,
+    }
+
+    def agen(self, identifier: SharedAgenIdentifier,
+             cache_strategy: CacheStrategy, **kwargs) -> AsyncGenerator[Any, None]:
+        if identifier.type in self.factories:
+            merged_kwargs = identifier.kwargs | kwargs
+            # noinspection PyTypeChecker
+            return self.factories[identifier.type](self, cache_strategy=cache_strategy, **merged_kwargs)
+        else:
+            raise ValueError("invalid identifier: " + str(identifier))
+
+    expires_in = {
+        PixivResType.ILLUST_DETAIL: timedelta(seconds=context.require(Config).pixiv_illust_detail_cache_expires_in),
+        PixivResType.USER_DETAIL: timedelta(seconds=context.require(Config).pixiv_user_detail_cache_expires_in),
+        PixivResType.SEARCH_ILLUST: timedelta(seconds=context.require(Config).pixiv_search_illust_cache_expires_in),
+        PixivResType.SEARCH_USER: timedelta(seconds=context.require(Config).pixiv_search_user_cache_expires_in),
+        PixivResType.USER_ILLUSTS: timedelta(seconds=context.require(Config).pixiv_user_illusts_cache_expires_in),
+        PixivResType.USER_BOOKMARKS: timedelta(seconds=context.require(Config).pixiv_user_bookmarks_cache_expires_in),
+        PixivResType.RECOMMENDED_ILLUSTS: timedelta(seconds=context.require(Config).pixiv_other_cache_expires_in),
+        PixivResType.RELATED_ILLUSTS: timedelta(seconds=context.require(Config).pixiv_related_illusts_cache_expires_in),
+        PixivResType.ILLUST_RANKING: timedelta(seconds=context.require(Config).pixiv_illust_ranking_cache_expires_in),
+        PixivResType.IMAGE: timedelta(seconds=context.require(Config).pixiv_download_cache_expires_in),
+    }
+
+    def calc_expires_time(self, identifier: SharedAgenIdentifier, update_time: datetime) -> datetime:
+        if identifier.type in self.factories:
+            return update_time + self.expires_in[identifier.type]
+        else:
+            raise ValueError("invalid identifier: " + str(identifier))
+
+    async def on_agen_next(self, identifier: SharedAgenIdentifier, item: Any):
+        await super().on_agen_next(identifier, item)
+        if isinstance(item, PixivRepoMetadata) and not self.get_expires_time(identifier):
+            expires_time = self.calc_expires_time(identifier, item.update_time)
+            await self.set_expires_time(identifier, expires_time.timestamp())
+
+
+@context.root.register_singleton()
+class MediatorPixivRepo(PixivRepo):
+    def __init__(self):
+        self.shared_agen_mgr = PixivSharedAsyncGeneratorManager()
+
+    async def invalidate_cache(self):
+        await self.shared_agen_mgr.invalidate_all()
+        await local.invalidate_all()
+
+    async def illust_detail(self, illust_id: int,
+                            cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[Illust, None]:
+        logger.debug(f"[mediator] illust_detail {illust_id} "
+                     f"cache_strategy={cache_strategy.name}")
+        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.ILLUST_DETAIL, illust_id=illust_id),
+                                            cache_strategy) as gen:
+            data = None
+            async for x in gen:
+                if not isinstance(x, PixivRepoMetadata):
+                    data = x
+
+        # 保证shared_agen能正常结束
+        if data is not None:
+            yield data
+
+    async def user_detail(self, user_id: int,
+                          cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[User, None]:
+        logger.debug(f"[mediator] user_detail {user_id} "
+                     f"cache_strategy={cache_strategy.name}")
+        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.USER_DETAIL, user_id=user_id),
+                                            cache_strategy) as gen:
+            data = None
+            async for x in gen:
+                if not isinstance(x, PixivRepoMetadata):
+                    data = x
+
+        # 保证shared_agen能正常结束
+        if data is not None:
+            yield data
+
+    async def search_illust(self, word: str,
+                            cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[LazyIllust, None]:
+        logger.debug(f"[mediator] search_illust {word} "
+                     f"cache_strategy={cache_strategy.name}")
+        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.SEARCH_ILLUST, word=word),
+                                            cache_strategy) as gen:
+            async for x in gen:
+                if not isinstance(x, PixivRepoMetadata):
+                    yield x
+
+    async def search_user(self, word: str,
+                          cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[User, None]:
+        logger.debug(f"[mediator] search_user {word} "
+                     f"cache_strategy={cache_strategy.name}")
+        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.SEARCH_USER, word=word),
+                                            cache_strategy) as gen:
+            async for x in gen:
+                if not isinstance(x, PixivRepoMetadata):
+                    yield x
+
+    async def user_bookmarks(self, user_id: int = 0,
+                             cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[LazyIllust, None]:
+        logger.debug(f"[mediator] user_bookmarks {user_id} "
+                     f"cache_strategy={cache_strategy.name}")
+        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.USER_BOOKMARKS, user_id=user_id),
+                                            cache_strategy) as gen:
+            async for x in gen:
+                if not isinstance(x, PixivRepoMetadata):
+                    yield x
+
+    async def user_illusts(self, user_id: int = 0,
+                           cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[LazyIllust, None]:
+        logger.debug(f"[mediator] user_illusts {user_id} "
+                     f"cache_strategy={cache_strategy.name}")
+        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.USER_ILLUSTS, user_id=user_id),
+                                            cache_strategy) as gen:
+            async for x in gen:
+                if not isinstance(x, PixivRepoMetadata):
+                    yield x
+
+    async def _contact_user_illusts_with_preview(self, user_preview: UserPreview,
+                                                 cache_strategy: CacheStrategy = CacheStrategy.NORMAL) \
+            -> AsyncGenerator[LazyIllust, None]:
+        for illust in user_preview.illusts:
+            yield LazyIllust(illust.id, illust)
+
+        ids = {x.id for x in user_preview.illusts}
+
+        if len(user_preview.illusts) >= 3:
+            gen = self.user_illusts(user_preview.user.id, cache_strategy)
+
+            async for x in gen:
+                if x.id not in ids:
+                    yield x
+
+    async def user_following_illusts(self, user_id: int,
+                                     cache_strategy: CacheStrategy = CacheStrategy.NORMAL) \
+            -> AsyncGenerator[LazyIllust, None]:
+        logger.debug(f"[mediator] user_following_illusts {user_id} "
+                     f"cache_strategy={cache_strategy.name}")
+
+        n = 0
+        gen = []
+        peeked = []
+
+        async for user_preview in remote.user_following_with_preview(user_id):
+            if not isinstance(user_preview, PixivRepoMetadata):
+                n += 1
+                gen.append(self._contact_user_illusts_with_preview(user_preview, cache_strategy))
+                peeked.append(None)
+
+        try:
+            while True:
+                select = -1
+                for i in range(n):
+                    try:
+                        if not peeked[i]:
+                            peeked[i] = await gen[i].__anext__()
+
+                        if select == -1 or peeked[i].create_date > peeked[select].create_date:
+                            select = i
+                    except StopAsyncIteration:
+                        pass
+
+                if select == -1:
+                    break
+
+                yield peeked[select]
+                peeked[select] = None
+        except GeneratorExit:
+            for gen in gen:
+                await gen.aclose()
+
+    async def recommended_illusts(self, cache_strategy: CacheStrategy = CacheStrategy.NORMAL) \
+            -> AsyncGenerator[LazyIllust, None]:
+        logger.debug(f"[mediator] recommended_illusts "
+                     f"cache_strategy={cache_strategy.name}")
+        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.RECOMMENDED_ILLUSTS),
+                                            cache_strategy) as gen:
+            async for x in gen:
+                if not isinstance(x, PixivRepoMetadata):
+                    yield x
+
+    async def related_illusts(self, illust_id: int,
+                              cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[LazyIllust, None]:
+        logger.debug(f"[mediator] related_illusts {illust_id} "
+                     f"cache_strategy={cache_strategy.name}")
+        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.RELATED_ILLUSTS, illust_id=illust_id),
+                                            cache_strategy) as gen:
+            async for x in gen:
+                if not isinstance(x, PixivRepoMetadata):
+                    yield x
+
+    async def illust_ranking(self, mode: Union[str, RankingMode],
+                             cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[LazyIllust, None]:
+        if isinstance(mode, str):
+            mode = RankingMode[mode]
+
+        logger.debug(f"[mediator] illust_ranking {mode} "
+                     f"cache_strategy={cache_strategy.name}")
+        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.ILLUST_RANKING, mode=mode),
+                                            cache_strategy) as gen:
+            async for x in gen:
+                if not isinstance(x, PixivRepoMetadata):
+                    yield x
+
+    async def image(self, illust: Illust, page: int = 0,
+                    cache_strategy: CacheStrategy = CacheStrategy.NORMAL) -> AsyncGenerator[bytes, None]:
+        logger.debug(f"[mediator] image {illust.id}[{page}] "
+                     f"cache_strategy={cache_strategy.name}")
+        async with self.shared_agen_mgr.get(SharedAgenIdentifier(PixivResType.IMAGE, illust_id=illust.id, page=page),
+                                            cache_strategy, illust=illust) as gen:
+            data = None
+            async for x in gen:
+                if not isinstance(x, PixivRepoMetadata):
+                    data = x
+
+        # 保证shared_agen能正常退出
+        if data is not None:
+            yield data
+
+
+__all__ = ('MediatorPixivRepo',)
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/pixiv_repo/remote_repo.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/pixiv_repo/remote_repo.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,410 +1,410 @@
-from asyncio import sleep, create_task, CancelledError, Semaphore, Task
-from contextlib import asynccontextmanager
-from datetime import datetime, timedelta
-from io import BytesIO
-from typing import TypeVar, Optional, Awaitable, List, Callable, Tuple, AsyncGenerator, Union
-
-from cachetools.func import rr_cache
-from nonebot import logger
-from pixivpy_async import *
-from pixivpy_async.error import TokenError
-
-from nonebot_plugin_pixivbot.config import Config
-from nonebot_plugin_pixivbot.enums import RankingMode
-from nonebot_plugin_pixivbot.global_context import context
-from nonebot_plugin_pixivbot.model import Illust, User, UserPreview
-from nonebot_plugin_pixivbot.utils.errors import QueryError, RateLimitError
-from nonebot_plugin_pixivbot.utils.lifecycler import on_startup, on_shutdown
-from .base import PixivRepo
-from .compressor import Compressor
-from .lazy_illust import LazyIllust
-from .models import PixivRepoMetadata
-
-_conf = context.require(Config)
-_compressor = context.require(Compressor)
-
-T = TypeVar("T")
-
-
-@context.register_eager_singleton()
-class RemotePixivRepo(PixivRepo):
-
-    # noinspection PyTypeChecker
-    def __init__(self):
-        self._sema: Semaphore = None
-        self._pclient: PixivClient = None
-        self._papi: AppPixivAPI = None
-        self._refresh_daemon: Task = None
-
-        self._got_rate_limit: Optional[datetime] = None
-
-        self.user_id = 0
-
-        on_startup(replay=True)(self.start)
-        on_shutdown()(self.shutdown)
-
-    async def _refresh(self):
-        # Latest app version can be found using GET /old/application-info/android
-        USER_AGENT = "PixivAndroidApp/5.0.234 (Android 11; Pixel 5)"
-        # REDIRECT_URI = "https://app-api.pixiv.net/web/v1/users/auth/pixiv/callback"
-        # LOGIN_URL = "https://app-api.pixiv.net/web/v1/login"
-        AUTH_TOKEN_URL = "https://oauth.secure.pixiv.net/auth/token"
-        CLIENT_ID = "MOBrBDS8blbauoSck0ZfDbtuzpyT"
-        CLIENT_SECRET = "lsACyCD94FhDUtGTXi3QzcFE2uU1hqtDaKeqrdwj"
-
-        refresh_token = _conf.pixiv_refresh_token
-
-        data = {
-            "client_id": CLIENT_ID,
-            "client_secret": CLIENT_SECRET,
-            "grant_type": "refresh_token",
-            "include_policy": "true",
-            "refresh_token": refresh_token,
-        }
-        result = await self._papi.requests_(method="POST", url=AUTH_TOKEN_URL, data=data,
-                                            headers={"User-Agent": USER_AGENT},
-                                            auth=False)
-        if result.has_error:
-            raise TokenError(None, result)
-        else:
-            self._papi.set_auth(result.access_token, result.refresh_token)
-            self.user_id = result["user"]["id"]
-
-            logger.success(
-                f"refresh access token successfully. new token expires in {result.expires_in} seconds.")
-            logger.debug(f"access_token: {result.access_token}")
-            logger.debug(f"refresh_token: {result.refresh_token}")
-
-            # maybe the refresh token will be changed (even thought i haven't seen it yet)
-            if result.refresh_token != refresh_token:
-                refresh_token = result.refresh_token
-                logger.warning(
-                    f"refresh token has been changed: {result.refresh_token}")
-
-            return result
-
-    async def _refresh_daemon_worker(self):
-        while True:
-            try:
-                result = await self._refresh()
-                await sleep(result.expires_in * 0.8)
-            except CancelledError as e:
-                raise e
-            except Exception as e:
-                logger.opt(exception=e).error("failed to refresh access token, will retry after 60s.")
-                await sleep(60)
-
-    def start(self):
-        self._pclient = PixivClient(proxy=_conf.pixiv_proxy, timeout=_conf.pixiv_query_timeout)
-        self._papi = AppPixivAPI(client=self._pclient.start())
-        self._papi.set_additional_headers({'Accept-Language': 'zh-CN'})
-        self._refresh_daemon = create_task(self._refresh_daemon_worker())
-        self._sema = Semaphore(_conf.pixiv_simultaneous_query)
-
-    async def shutdown(self):
-        await self._pclient.close()
-        self._refresh_daemon.cancel()
-
-    def _check_error_in_raw_result(self, raw_result: dict):
-        if "error" in raw_result:
-            message = raw_result["error"]["user_message"] \
-                      or raw_result["error"]["message"] \
-                      or raw_result["error"]["reason"]
-            if message == "Rate Limit":
-                # 处理RateLimit
-                self._got_rate_limit = datetime.utcnow()
-                raise RateLimitError()
-            else:
-                raise QueryError(message)
-
-    @asynccontextmanager
-    async def _query(self):
-        # RateLimit期间不进行查询
-        if self._got_rate_limit is not None:
-            now = datetime.utcnow()
-            if now - self._got_rate_limit >= timedelta(minutes=2):
-                self._got_rate_limit = None
-            else:
-                raise RateLimitError()
-
-        async with self._sema:
-            yield
-
-    async def _load_raw_page(self, papi_search_func: Callable[..., Awaitable[dict]],
-                             **kwargs):
-        async with self._query():
-            raw_result = await papi_search_func(**kwargs)
-            self._check_error_in_raw_result(raw_result)
-            return raw_result
-
-    @staticmethod
-    @rr_cache()  # 因为size足够就不会发生替换，所以缓存用random replacement算法最快
-    def _make_illust_filter(min_view: int = 2 ** 31 - 1, min_bookmark: int = 2 ** 31 - 1):
-        def illust_filter(illust: Illust) -> bool:
-            # 标签过滤
-            for tag in _conf.pixiv_block_tags:
-                if illust.has_tag(tag):
-                    return False
-            # 书签下限过滤
-            if illust.total_bookmarks < min_bookmark:
-                return False
-            # 浏览量下限过滤
-            if illust.total_view < min_view:
-                return False
-            # AI过滤
-            if _conf.pixiv_exclude_ai_illusts and illust.illust_ai_type != 0:
-                return False
-            return True
-
-        return illust_filter
-
-    async def _load_page(self, papi_search_func: Callable[..., Awaitable[dict]],
-                         element_list_name: str,
-                         *, mapper: Optional[Callable[[dict], T]] = None,
-                         filter_item: Optional[Callable[[T], bool]] = None,
-                         **kwargs) -> Tuple[List[T], PixivRepoMetadata]:
-        """
-        加载一页
-        :param papi_search_func: PixivPy-Async的加载方法
-        :param element_list_name: 返回JSON中元素所在列表名
-        :param mapper: 将元素从JSON格式映射为特定格式
-        :param filter_item: 过滤不符合条件的元素（先映射再过滤）
-        :param kwargs: 传给papi_search_func的参数
-        :return: 加载结果
-        """
-        raw_result = await self._load_raw_page(papi_search_func, **kwargs)
-
-        pending = []
-        for x in raw_result[element_list_name]:
-            if mapper is not None:
-                x = mapper(x)
-
-            if not filter_item or filter_item(x):
-                pending.append(x)
-
-        metadata = PixivRepoMetadata(next_qs=AppPixivAPI.parse_qs(next_url=raw_result["next_url"]))
-
-        return pending, metadata
-
-    async def _load_many_pages(self, papi_search_func: Callable[..., Awaitable[dict]],
-                               element_list_name: str,
-                               *, mapper: Optional[Callable[[dict], T]] = None,
-                               filter_item: Optional[Callable[[T], bool]] = None,
-                               **kwargs) -> AsyncGenerator[Tuple[List[T], PixivRepoMetadata], None]:
-        """
-        一次加载多页
-        :param papi_search_func: PixivPy-Async的加载方法
-        :param element_list_name: 返回JSON中元素所在列表名
-        :param mapper: 将元素从JSON格式映射为特定格式
-        :param filter_item: 过滤不符合条件的元素（先映射再过滤）
-        :param kwargs: 传给papi_search_func的参数
-        :return: 加载结果
-        """
-        loaded_items = 0
-        loaded_pages = 0
-        next_qs = kwargs
-
-        while True:
-            logger.debug(f"[remote] loading page {loaded_pages}")
-            page, metadata = await self._load_page(papi_search_func, element_list_name, mapper=mapper,
-                                                   filter_item=filter_item, **next_qs)
-
-            loaded_pages = loaded_pages + 1
-            loaded_items += len(page)
-
-            metadata.pages = loaded_pages
-            yield page, metadata
-
-            next_qs = metadata.next_qs
-            if next_qs:
-                if 'viewed' in next_qs:
-                    # 由于pixivpy-async的illust_recommended的bug，需要删掉这个参数
-                    del next_qs['viewed']
-            else:
-                break
-
-    async def _get_illusts(self, papi_search_func: Callable[[], Awaitable[dict]],
-                           *, min_bookmark: int = 0,
-                           min_view: int = 0,
-                           **kwargs) \
-            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        """
-        加载插画
-        :param papi_search_func: PixivPy-Async的加载方法
-        :param min_bookmark: 书签数下限
-        :param min_view: 阅读数下限
-        :param kwargs: 传给papi_search_func的参数
-        :return:
-        """
-        total = 0
-        broken = 0
-
-        try:
-            yield PixivRepoMetadata(pages=0, next_qs=kwargs)
-            async for page, metadata in self._load_many_pages(papi_search_func, "illusts",
-                                                              mapper=lambda x: Illust.parse_obj(x),
-                                                              filter_item=self._make_illust_filter(min_view,
-                                                                                                   min_bookmark),
-                                                              **kwargs):
-                for item in page:
-                    total += 1
-                    if "limit_unknown_360.png" in item.image_urls.large:
-                        broken += 1
-                        yield LazyIllust(item.id)
-                    else:
-                        yield LazyIllust(item.id, item)
-                yield metadata
-        finally:
-            logger.debug(f"[remote] got {total} illusts, illust_detail of {broken} are missed")
-
-    async def _get_user_previews(self, papi_search_func: Callable[[], Awaitable[dict]], **kwargs) \
-            -> AsyncGenerator[Union[PixivRepoMetadata, UserPreview], None]:
-        yield PixivRepoMetadata(pages=0, next_qs=kwargs)
-        async for page, metadata in self._load_many_pages(papi_search_func, "user_previews",
-                                                          mapper=lambda x: UserPreview.parse_obj(x), **kwargs):
-            for item in page:
-                item: UserPreview
-                item.illusts = list(filter(self._make_illust_filter(), item.illusts))
-                yield item
-            yield metadata
-
-    async def _get_users(self, papi_search_func: Callable[[], Awaitable[dict]], **kwargs) \
-            -> AsyncGenerator[Union[PixivRepoMetadata, User], None]:
-        yield PixivRepoMetadata(pages=0, next_qs=kwargs)
-        async for page, metadata in self._load_many_pages(papi_search_func, "user_previews",
-                                                          mapper=lambda x: User.parse_obj(x["user"]), **kwargs):
-            for item in page:
-                yield item
-            yield metadata
-
-    async def _raw_illust_detail(self, illust_id: int, **kwargs) -> dict:
-        async with self._query():
-            raw_result = await self._papi.illust_detail(illust_id, **kwargs)
-            self._check_error_in_raw_result(raw_result)
-            return raw_result
-
-    async def illust_detail(self, illust_id: int, **kwargs) -> AsyncGenerator[Illust, None]:
-        logger.debug(f"[remote] illust_detail {illust_id}")
-        raw_result = await self._raw_illust_detail(illust_id, **kwargs)
-        yield PixivRepoMetadata()
-        yield Illust.parse_obj(raw_result["illust"])
-
-    async def _raw_user_detail(self, user_id: int, **kwargs) -> dict:
-        async with self._query():
-            raw_result = await self._papi.user_detail(user_id, **kwargs)
-            self._check_error_in_raw_result(raw_result)
-            return raw_result
-
-    async def user_detail(self, user_id: int, **kwargs) -> AsyncGenerator[User, None]:
-        logger.debug(f"[remote] user_detail {user_id}")
-        raw_result = await self._raw_user_detail(user_id, **kwargs)
-        yield PixivRepoMetadata()
-        yield User.parse_obj(raw_result["user"])
-
-    def search_illust(self, word: str, **kwargs) \
-            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        logger.debug(f"[remote] search_illust {word}")
-        return self._get_illusts(self._papi.search_illust,
-                                 min_bookmark=_conf.pixiv_random_illust_min_bookmark,
-                                 min_view=_conf.pixiv_random_illust_min_view,
-                                 word=word, **kwargs)
-
-    def search_user(self, word: str, **kwargs) \
-            -> AsyncGenerator[Union[User, PixivRepoMetadata], None]:
-        logger.debug(f"[remote] search_user {word}")
-        return self._get_users(self._papi.search_user,
-                               word=word, **kwargs)
-
-    def search_user_with_preview(self, word: str, **kwargs) \
-            -> AsyncGenerator[Union[UserPreview, PixivRepoMetadata], None]:
-        logger.debug(f"[remote] search_user {word}")
-        return self._get_user_previews(self._papi.search_user,
-                                       word=word, **kwargs)
-
-    def user_following(self, user_id: int, **kwargs) \
-            -> AsyncGenerator[Union[User, PixivRepoMetadata], None]:
-        logger.debug(f"[remote] following_users {user_id}")
-        return self._get_users(self._papi.user_following,
-                               user_id=user_id, **kwargs)
-
-    def user_following_with_preview(self, user_id: int, **kwargs) \
-            -> AsyncGenerator[Union[UserPreview, PixivRepoMetadata], None]:
-        logger.debug(f"[remote] following_users {user_id}")
-        return self._get_user_previews(self._papi.user_following,
-                                       user_id=user_id, **kwargs)
-
-    def user_illusts(self, user_id: int, **kwargs) \
-            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        logger.debug(f"[remote] user_illusts {user_id}")
-        return self._get_illusts(self._papi.user_illusts,
-                                 min_bookmark=_conf.pixiv_random_user_illust_min_bookmark,
-                                 min_view=_conf.pixiv_random_user_illust_min_view,
-                                 user_id=user_id, **kwargs)
-
-    def user_bookmarks(self, user_id: int = 0, **kwargs) \
-            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        if user_id == 0:
-            user_id = self.user_id
-
-        logger.debug(f"[remote] user_bookmarks {user_id}")
-        return self._get_illusts(self._papi.user_bookmarks_illust,
-                                 min_bookmark=_conf.pixiv_random_bookmark_min_bookmark,
-                                 min_view=_conf.pixiv_random_bookmark_min_view,
-                                 user_id=user_id, **kwargs)
-
-    # def following_illusts(self, **kwargs) \
-    #         -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-    #     logger.debug(f"[remote] following_illusts")
-    #     return self._get_illusts(self._papi.illust_follow,
-    #                              min_bookmark=_conf.pixiv_random_following_illust_min_bookmark,
-    #                              min_view=_conf.pixiv_random_following_illust_min_view,
-    #                              **kwargs)
-
-    def recommended_illusts(self, **kwargs) \
-            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        logger.debug(f"[remote] recommended_illusts")
-        return self._get_illusts(self._papi.illust_recommended,
-                                 min_bookmark=_conf.pixiv_random_recommended_illust_min_bookmark,
-                                 min_view=_conf.pixiv_random_recommended_illust_min_view,
-                                 **kwargs)
-
-    def related_illusts(self, illust_id: int, **kwargs) \
-            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        logger.debug(f"[remote] related_illusts {illust_id}")
-        return self._get_illusts(self._papi.illust_related,
-                                 min_bookmark=_conf.pixiv_random_related_illust_min_bookmark,
-                                 min_view=_conf.pixiv_random_related_illust_min_view,
-                                 illust_id=illust_id, **kwargs)
-
-    def illust_ranking(self, mode: Union[str, RankingMode], **kwargs) \
-            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
-        if isinstance(mode, str):
-            mode = RankingMode[mode]
-
-        logger.debug(f"[remote] illust_ranking {mode}")
-        return self._get_illusts(self._papi.illust_ranking,
-                                 mode=mode.name, **kwargs)
-
-    async def _raw_image(self, illust: Illust, page: int, **kwargs) -> bytes:
-        custom_domain = _conf.pixiv_download_custom_domain
-
-        url = illust.page_image_url(page)
-        if custom_domain is not None:
-            url = url.replace("i.pximg.net", custom_domain)
-
-        async with self._query():
-            with BytesIO() as bio:
-                await self._papi.download(url, fname=bio, **kwargs)
-                content = bio.getvalue()
-                return content
-
-    async def image(self, illust: Illust, page: int = 0, **kwargs) \
-            -> AsyncGenerator[Union[bytes, PixivRepoMetadata], None]:
-        logger.debug(f"[remote] image {illust.id}")
-        content = await self._raw_image(illust, page, **kwargs)
-        content = await _compressor.compress(content)
-        yield PixivRepoMetadata()
-        yield content
-
-
-__all__ = ("RemotePixivRepo",)
+from asyncio import sleep, create_task, CancelledError, Semaphore, Task
+from contextlib import asynccontextmanager
+from datetime import datetime, timedelta
+from io import BytesIO
+from typing import TypeVar, Optional, Awaitable, List, Callable, Tuple, AsyncGenerator, Union
+
+from cachetools.func import rr_cache
+from nonebot import logger
+from pixivpy_async import *
+from pixivpy_async.error import TokenError
+
+from nonebot_plugin_pixivbot.config import Config
+from nonebot_plugin_pixivbot.enums import RankingMode
+from nonebot_plugin_pixivbot.global_context import context
+from nonebot_plugin_pixivbot.model import Illust, User, UserPreview
+from nonebot_plugin_pixivbot.utils.errors import QueryError, RateLimitError
+from nonebot_plugin_pixivbot.utils.lifecycler import on_startup, on_shutdown
+from .base import PixivRepo
+from .compressor import Compressor
+from .lazy_illust import LazyIllust
+from .models import PixivRepoMetadata
+
+_conf = context.require(Config)
+_compressor = context.require(Compressor)
+
+T = TypeVar("T")
+
+
+@context.register_eager_singleton()
+class RemotePixivRepo(PixivRepo):
+
+    # noinspection PyTypeChecker
+    def __init__(self):
+        self._sema: Semaphore = None
+        self._pclient: PixivClient = None
+        self._papi: AppPixivAPI = None
+        self._refresh_daemon: Task = None
+
+        self._got_rate_limit: Optional[datetime] = None
+
+        self.user_id = 0
+
+        on_startup(replay=True)(self.start)
+        on_shutdown()(self.shutdown)
+
+    async def _refresh(self):
+        # Latest app version can be found using GET /old/application-info/android
+        USER_AGENT = "PixivAndroidApp/5.0.234 (Android 11; Pixel 5)"
+        # REDIRECT_URI = "https://app-api.pixiv.net/web/v1/users/auth/pixiv/callback"
+        # LOGIN_URL = "https://app-api.pixiv.net/web/v1/login"
+        AUTH_TOKEN_URL = "https://oauth.secure.pixiv.net/auth/token"
+        CLIENT_ID = "MOBrBDS8blbauoSck0ZfDbtuzpyT"
+        CLIENT_SECRET = "lsACyCD94FhDUtGTXi3QzcFE2uU1hqtDaKeqrdwj"
+
+        refresh_token = _conf.pixiv_refresh_token
+
+        data = {
+            "client_id": CLIENT_ID,
+            "client_secret": CLIENT_SECRET,
+            "grant_type": "refresh_token",
+            "include_policy": "true",
+            "refresh_token": refresh_token,
+        }
+        result = await self._papi.requests_(method="POST", url=AUTH_TOKEN_URL, data=data,
+                                            headers={"User-Agent": USER_AGENT},
+                                            auth=False)
+        if result.has_error:
+            raise TokenError(None, result)
+        else:
+            self._papi.set_auth(result.access_token, result.refresh_token)
+            self.user_id = result["user"]["id"]
+
+            logger.success(
+                f"refresh access token successfully. new token expires in {result.expires_in} seconds.")
+            logger.debug(f"access_token: {result.access_token}")
+            logger.debug(f"refresh_token: {result.refresh_token}")
+
+            # maybe the refresh token will be changed (even thought i haven't seen it yet)
+            if result.refresh_token != refresh_token:
+                refresh_token = result.refresh_token
+                logger.warning(
+                    f"refresh token has been changed: {result.refresh_token}")
+
+            return result
+
+    async def _refresh_daemon_worker(self):
+        while True:
+            try:
+                result = await self._refresh()
+                await sleep(result.expires_in * 0.8)
+            except CancelledError as e:
+                raise e
+            except Exception as e:
+                logger.opt(exception=e).error("failed to refresh access token, will retry after 60s.")
+                await sleep(60)
+
+    def start(self):
+        self._pclient = PixivClient(proxy=_conf.pixiv_proxy, timeout=_conf.pixiv_query_timeout)
+        self._papi = AppPixivAPI(client=self._pclient.start())
+        self._papi.set_additional_headers({'Accept-Language': 'zh-CN'})
+        self._refresh_daemon = create_task(self._refresh_daemon_worker())
+        self._sema = Semaphore(_conf.pixiv_simultaneous_query)
+
+    async def shutdown(self):
+        await self._pclient.close()
+        self._refresh_daemon.cancel()
+
+    def _check_error_in_raw_result(self, raw_result: dict):
+        if "error" in raw_result:
+            message = raw_result["error"]["user_message"] \
+                      or raw_result["error"]["message"] \
+                      or raw_result["error"]["reason"]
+            if message == "Rate Limit":
+                # 处理RateLimit
+                self._got_rate_limit = datetime.utcnow()
+                raise RateLimitError()
+            else:
+                raise QueryError(message)
+
+    @asynccontextmanager
+    async def _query(self):
+        # RateLimit期间不进行查询
+        if self._got_rate_limit is not None:
+            now = datetime.utcnow()
+            if now - self._got_rate_limit >= timedelta(minutes=2):
+                self._got_rate_limit = None
+            else:
+                raise RateLimitError()
+
+        async with self._sema:
+            yield
+
+    async def _load_raw_page(self, papi_search_func: Callable[..., Awaitable[dict]],
+                             **kwargs):
+        async with self._query():
+            raw_result = await papi_search_func(**kwargs)
+            self._check_error_in_raw_result(raw_result)
+            return raw_result
+
+    @staticmethod
+    @rr_cache()  # 因为size足够就不会发生替换，所以缓存用random replacement算法最快
+    def _make_illust_filter(min_view: int = 2 ** 31 - 1, min_bookmark: int = 2 ** 31 - 1):
+        def illust_filter(illust: Illust) -> bool:
+            # 标签过滤
+            for tag in _conf.pixiv_block_tags:
+                if illust.has_tag(tag):
+                    return False
+            # 书签下限过滤
+            if illust.total_bookmarks < min_bookmark:
+                return False
+            # 浏览量下限过滤
+            if illust.total_view < min_view:
+                return False
+            # AI过滤
+            if _conf.pixiv_exclude_ai_illusts and illust.illust_ai_type != 0:
+                return False
+            return True
+
+        return illust_filter
+
+    async def _load_page(self, papi_search_func: Callable[..., Awaitable[dict]],
+                         element_list_name: str,
+                         *, mapper: Optional[Callable[[dict], T]] = None,
+                         filter_item: Optional[Callable[[T], bool]] = None,
+                         **kwargs) -> Tuple[List[T], PixivRepoMetadata]:
+        """
+        加载一页
+        :param papi_search_func: PixivPy-Async的加载方法
+        :param element_list_name: 返回JSON中元素所在列表名
+        :param mapper: 将元素从JSON格式映射为特定格式
+        :param filter_item: 过滤不符合条件的元素（先映射再过滤）
+        :param kwargs: 传给papi_search_func的参数
+        :return: 加载结果
+        """
+        raw_result = await self._load_raw_page(papi_search_func, **kwargs)
+
+        pending = []
+        for x in raw_result[element_list_name]:
+            if mapper is not None:
+                x = mapper(x)
+
+            if not filter_item or filter_item(x):
+                pending.append(x)
+
+        metadata = PixivRepoMetadata(next_qs=AppPixivAPI.parse_qs(next_url=raw_result["next_url"]))
+
+        return pending, metadata
+
+    async def _load_many_pages(self, papi_search_func: Callable[..., Awaitable[dict]],
+                               element_list_name: str,
+                               *, mapper: Optional[Callable[[dict], T]] = None,
+                               filter_item: Optional[Callable[[T], bool]] = None,
+                               **kwargs) -> AsyncGenerator[Tuple[List[T], PixivRepoMetadata], None]:
+        """
+        一次加载多页
+        :param papi_search_func: PixivPy-Async的加载方法
+        :param element_list_name: 返回JSON中元素所在列表名
+        :param mapper: 将元素从JSON格式映射为特定格式
+        :param filter_item: 过滤不符合条件的元素（先映射再过滤）
+        :param kwargs: 传给papi_search_func的参数
+        :return: 加载结果
+        """
+        loaded_items = 0
+        loaded_pages = 0
+        next_qs = kwargs
+
+        while True:
+            logger.debug(f"[remote] loading page {loaded_pages}")
+            page, metadata = await self._load_page(papi_search_func, element_list_name, mapper=mapper,
+                                                   filter_item=filter_item, **next_qs)
+
+            loaded_pages = loaded_pages + 1
+            loaded_items += len(page)
+
+            metadata.pages = loaded_pages
+            yield page, metadata
+
+            next_qs = metadata.next_qs
+            if next_qs:
+                if 'viewed' in next_qs:
+                    # 由于pixivpy-async的illust_recommended的bug，需要删掉这个参数
+                    del next_qs['viewed']
+            else:
+                break
+
+    async def _get_illusts(self, papi_search_func: Callable[[], Awaitable[dict]],
+                           *, min_bookmark: int = 0,
+                           min_view: int = 0,
+                           **kwargs) \
+            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
+        """
+        加载插画
+        :param papi_search_func: PixivPy-Async的加载方法
+        :param min_bookmark: 书签数下限
+        :param min_view: 阅读数下限
+        :param kwargs: 传给papi_search_func的参数
+        :return:
+        """
+        total = 0
+        broken = 0
+
+        try:
+            yield PixivRepoMetadata(pages=0, next_qs=kwargs)
+            async for page, metadata in self._load_many_pages(papi_search_func, "illusts",
+                                                              mapper=lambda x: Illust.parse_obj(x),
+                                                              filter_item=self._make_illust_filter(min_view,
+                                                                                                   min_bookmark),
+                                                              **kwargs):
+                for item in page:
+                    total += 1
+                    if "limit_unknown_360.png" in item.image_urls.large:
+                        broken += 1
+                        yield LazyIllust(item.id)
+                    else:
+                        yield LazyIllust(item.id, item)
+                yield metadata
+        finally:
+            logger.debug(f"[remote] got {total} illusts, illust_detail of {broken} are missed")
+
+    async def _get_user_previews(self, papi_search_func: Callable[[], Awaitable[dict]], **kwargs) \
+            -> AsyncGenerator[Union[PixivRepoMetadata, UserPreview], None]:
+        yield PixivRepoMetadata(pages=0, next_qs=kwargs)
+        async for page, metadata in self._load_many_pages(papi_search_func, "user_previews",
+                                                          mapper=lambda x: UserPreview.parse_obj(x), **kwargs):
+            for item in page:
+                item: UserPreview
+                item.illusts = list(filter(self._make_illust_filter(), item.illusts))
+                yield item
+            yield metadata
+
+    async def _get_users(self, papi_search_func: Callable[[], Awaitable[dict]], **kwargs) \
+            -> AsyncGenerator[Union[PixivRepoMetadata, User], None]:
+        yield PixivRepoMetadata(pages=0, next_qs=kwargs)
+        async for page, metadata in self._load_many_pages(papi_search_func, "user_previews",
+                                                          mapper=lambda x: User.parse_obj(x["user"]), **kwargs):
+            for item in page:
+                yield item
+            yield metadata
+
+    async def _raw_illust_detail(self, illust_id: int, **kwargs) -> dict:
+        async with self._query():
+            raw_result = await self._papi.illust_detail(illust_id, **kwargs)
+            self._check_error_in_raw_result(raw_result)
+            return raw_result
+
+    async def illust_detail(self, illust_id: int, **kwargs) -> AsyncGenerator[Illust, None]:
+        logger.debug(f"[remote] illust_detail {illust_id}")
+        raw_result = await self._raw_illust_detail(illust_id, **kwargs)
+        yield PixivRepoMetadata()
+        yield Illust.parse_obj(raw_result["illust"])
+
+    async def _raw_user_detail(self, user_id: int, **kwargs) -> dict:
+        async with self._query():
+            raw_result = await self._papi.user_detail(user_id, **kwargs)
+            self._check_error_in_raw_result(raw_result)
+            return raw_result
+
+    async def user_detail(self, user_id: int, **kwargs) -> AsyncGenerator[User, None]:
+        logger.debug(f"[remote] user_detail {user_id}")
+        raw_result = await self._raw_user_detail(user_id, **kwargs)
+        yield PixivRepoMetadata()
+        yield User.parse_obj(raw_result["user"])
+
+    def search_illust(self, word: str, **kwargs) \
+            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
+        logger.debug(f"[remote] search_illust {word}")
+        return self._get_illusts(self._papi.search_illust,
+                                 min_bookmark=_conf.pixiv_random_illust_min_bookmark,
+                                 min_view=_conf.pixiv_random_illust_min_view,
+                                 word=word, **kwargs)
+
+    def search_user(self, word: str, **kwargs) \
+            -> AsyncGenerator[Union[User, PixivRepoMetadata], None]:
+        logger.debug(f"[remote] search_user {word}")
+        return self._get_users(self._papi.search_user,
+                               word=word, **kwargs)
+
+    def search_user_with_preview(self, word: str, **kwargs) \
+            -> AsyncGenerator[Union[UserPreview, PixivRepoMetadata], None]:
+        logger.debug(f"[remote] search_user {word}")
+        return self._get_user_previews(self._papi.search_user,
+                                       word=word, **kwargs)
+
+    def user_following(self, user_id: int, **kwargs) \
+            -> AsyncGenerator[Union[User, PixivRepoMetadata], None]:
+        logger.debug(f"[remote] following_users {user_id}")
+        return self._get_users(self._papi.user_following,
+                               user_id=user_id, **kwargs)
+
+    def user_following_with_preview(self, user_id: int, **kwargs) \
+            -> AsyncGenerator[Union[UserPreview, PixivRepoMetadata], None]:
+        logger.debug(f"[remote] following_users {user_id}")
+        return self._get_user_previews(self._papi.user_following,
+                                       user_id=user_id, **kwargs)
+
+    def user_illusts(self, user_id: int, **kwargs) \
+            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
+        logger.debug(f"[remote] user_illusts {user_id}")
+        return self._get_illusts(self._papi.user_illusts,
+                                 min_bookmark=_conf.pixiv_random_user_illust_min_bookmark,
+                                 min_view=_conf.pixiv_random_user_illust_min_view,
+                                 user_id=user_id, **kwargs)
+
+    def user_bookmarks(self, user_id: int = 0, **kwargs) \
+            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
+        if user_id == 0:
+            user_id = self.user_id
+
+        logger.debug(f"[remote] user_bookmarks {user_id}")
+        return self._get_illusts(self._papi.user_bookmarks_illust,
+                                 min_bookmark=_conf.pixiv_random_bookmark_min_bookmark,
+                                 min_view=_conf.pixiv_random_bookmark_min_view,
+                                 user_id=user_id, **kwargs)
+
+    # def following_illusts(self, **kwargs) \
+    #         -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
+    #     logger.debug(f"[remote] following_illusts")
+    #     return self._get_illusts(self._papi.illust_follow,
+    #                              min_bookmark=_conf.pixiv_random_following_illust_min_bookmark,
+    #                              min_view=_conf.pixiv_random_following_illust_min_view,
+    #                              **kwargs)
+
+    def recommended_illusts(self, **kwargs) \
+            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
+        logger.debug(f"[remote] recommended_illusts")
+        return self._get_illusts(self._papi.illust_recommended,
+                                 min_bookmark=_conf.pixiv_random_recommended_illust_min_bookmark,
+                                 min_view=_conf.pixiv_random_recommended_illust_min_view,
+                                 **kwargs)
+
+    def related_illusts(self, illust_id: int, **kwargs) \
+            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
+        logger.debug(f"[remote] related_illusts {illust_id}")
+        return self._get_illusts(self._papi.illust_related,
+                                 min_bookmark=_conf.pixiv_random_related_illust_min_bookmark,
+                                 min_view=_conf.pixiv_random_related_illust_min_view,
+                                 illust_id=illust_id, **kwargs)
+
+    def illust_ranking(self, mode: Union[str, RankingMode], **kwargs) \
+            -> AsyncGenerator[Union[LazyIllust, PixivRepoMetadata], None]:
+        if isinstance(mode, str):
+            mode = RankingMode[mode]
+
+        logger.debug(f"[remote] illust_ranking {mode}")
+        return self._get_illusts(self._papi.illust_ranking,
+                                 mode=mode.name, **kwargs)
+
+    async def _raw_image(self, illust: Illust, page: int, **kwargs) -> bytes:
+        custom_domain = _conf.pixiv_download_custom_domain
+
+        url = illust.page_image_url(page)
+        if custom_domain is not None:
+            url = url.replace("i.pximg.net", custom_domain)
+
+        async with self._query():
+            with BytesIO() as bio:
+                await self._papi.download(url, fname=bio, **kwargs)
+                content = bio.getvalue()
+                return content
+
+    async def image(self, illust: Illust, page: int = 0, **kwargs) \
+            -> AsyncGenerator[Union[bytes, PixivRepoMetadata], None]:
+        logger.debug(f"[remote] image {illust.id}")
+        content = await self._raw_image(illust, page, **kwargs)
+        content = await _compressor.compress(content)
+        yield PixivRepoMetadata()
+        yield content
+
+
+__all__ = ("RemotePixivRepo",)
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/source/lifecycle_mixin.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/lifecycle_mixin.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-import asyncio
-from inspect import isawaitable
-from typing import Callable, Union, Awaitable
-
-from nonebot import logger
-
-
-class DataSourceLifecycle:
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._on_initializing_callbacks = []
-        self._on_initialized_callbacks = []
-        self._on_closing_callbacks = []
-        self._on_closed_callbacks = []
-
-    def on_initializing(self, func: Callable[[], Union[None, Awaitable[None]]]):
-        self._on_initializing_callbacks.append(func)
-
-    def on_initialized(self, func: Callable[[], Union[None, Awaitable[None]]]):
-        self._on_initialized_callbacks.append(func)
-
-    def on_closing(self, func: Callable[[], Union[None, Awaitable[None]]]):
-        self._on_closing_callbacks.append(func)
-
-    def on_closed(self, func: Callable[[], Union[None, Awaitable[None]]]):
-        self._on_closed_callbacks.append(func)
-
-    async def _fire_initializing(self):
-        logger.trace("[data source] Firing initializing event")
-        fut = filter(isawaitable, (x() for x in self._on_initializing_callbacks))
-        await asyncio.gather(*fut)
-
-    async def _fire_initialized(self):
-        logger.trace("[data source] Firing initialized event")
-        fut = filter(isawaitable, (x() for x in self._on_initialized_callbacks))
-        await asyncio.gather(*fut)
-
-    async def _fire_closing(self):
-        logger.trace("[data source] Firing closing event")
-        fut = filter(isawaitable, (x() for x in self._on_closing_callbacks))
-        await asyncio.gather(*fut)
-
-    async def _fire_closed(self):
-        logger.trace("[data source] Firing closed event")
-        fut = filter(isawaitable, (x() for x in self._on_closed_callbacks))
-        await asyncio.gather(*fut)
+import asyncio
+from inspect import isawaitable
+from typing import Callable, Union, Awaitable
+
+from nonebot import logger
+
+
+class DataSourceLifecycle:
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._on_initializing_callbacks = []
+        self._on_initialized_callbacks = []
+        self._on_closing_callbacks = []
+        self._on_closed_callbacks = []
+
+    def on_initializing(self, func: Callable[[], Union[None, Awaitable[None]]]):
+        self._on_initializing_callbacks.append(func)
+
+    def on_initialized(self, func: Callable[[], Union[None, Awaitable[None]]]):
+        self._on_initialized_callbacks.append(func)
+
+    def on_closing(self, func: Callable[[], Union[None, Awaitable[None]]]):
+        self._on_closing_callbacks.append(func)
+
+    def on_closed(self, func: Callable[[], Union[None, Awaitable[None]]]):
+        self._on_closed_callbacks.append(func)
+
+    async def _fire_initializing(self):
+        logger.trace("[data source] Firing initializing event")
+        fut = filter(isawaitable, (x() for x in self._on_initializing_callbacks))
+        await asyncio.gather(*fut)
+
+    async def _fire_initialized(self):
+        logger.trace("[data source] Firing initialized event")
+        fut = filter(isawaitable, (x() for x in self._on_initialized_callbacks))
+        await asyncio.gather(*fut)
+
+    async def _fire_closing(self):
+        logger.trace("[data source] Firing closing event")
+        fut = filter(isawaitable, (x() for x in self._on_closing_callbacks))
+        await asyncio.gather(*fut)
+
+    async def _fire_closed(self):
+        logger.trace("[data source] Firing closed event")
+        fut = filter(isawaitable, (x() for x in self._on_closed_callbacks))
+        await asyncio.gather(*fut)
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/source/sql/__init__.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/sql/__init__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,148 +1,148 @@
-import json
-from contextlib import asynccontextmanager
-from datetime import datetime, date
-from typing import AsyncContextManager
-
-from nonebot import get_driver, logger
-from sqlalchemy import select, inspect
-from sqlalchemy.ext.asyncio import create_async_engine, AsyncSession, AsyncEngine, AsyncConnection
-from sqlalchemy.orm import registry, sessionmaker
-from sqlalchemy.pool import StaticPool
-
-from ..lifecycle_mixin import DataSourceLifecycle
-from ...errors import DataSourceNotReadyError
-from ....config import Config
-from ....global_context import context
-from ....utils.lifecycler import on_startup, on_shutdown
-
-conf = context.require(Config)
-
-
-def default_dumps(obj):
-    if isinstance(obj, (datetime, date)):
-        return obj.isoformat()
-
-    return None
-
-
-def json_serializer(obj):
-    return json.dumps(obj, default=default_dumps)
-
-
-@context.register_eager_singleton()
-class DataSource(DataSourceLifecycle):
-    app_db_version = 5
-    registry = registry()
-
-    def __init__(self):
-        super().__init__()
-
-        self._engine = None
-        self._sessionmaker = None
-
-        on_startup(replay=True)(self.initialize)
-        on_shutdown()(self.close)
-
-    async def _raw_get_db_version(self, conn: AsyncConnection) -> int:
-        async with AsyncSession(conn, expire_on_commit=False) as session:
-            from .meta_info import MetaInfo
-
-            # 判断是否初次建库
-            blank_database = not await conn.run_sync(lambda conn: inspect(conn).has_table("subscription"))
-            if blank_database:
-                result = MetaInfo(key="db_version", value=str(self.app_db_version))
-                session.add(result)
-                await session.commit()
-                v = self.app_db_version
-            else:
-                stmt = select(MetaInfo).where(MetaInfo.key == "db_version")
-                result = (await session.execute(stmt)).scalar_one_or_none()
-                if result is None:
-                    result = MetaInfo(key="db_version", value="1")
-                    session.add(result)
-                    await session.commit()
-
-                v = int(result.value)
-        return v
-
-    async def _raw_set_db_version(self, db_version: int, conn: AsyncConnection):
-        from .meta_info import MetaInfo
-        async with AsyncSession(conn, expire_on_commit=False) as session:
-            stmt = select(MetaInfo).where(MetaInfo.key == "db_version")
-            result = (await session.execute(stmt)).scalar_one_or_none()
-            if result is None:
-                result = MetaInfo(key="db_version", value="1")
-                session.add(result)
-
-            result.value = str(db_version)
-            await session.commit()
-
-    async def initialize(self):
-        await self._fire_initializing()
-
-        driver = get_driver()
-
-        params = {
-            # 仅当TRACE模式时回显sql语句
-            'echo': driver.config.log_level == 'TRACE',
-            'future': True,
-            'json_serializer': json_serializer
-        }
-
-        if conf.detect_sql_dialect == 'sqlite':
-            # 使用 SQLite 数据库时，如果在写入时遇到 (sqlite3.OperationalError) database is locked 错误。
-            # 可尝试将 poolclass 设置为 StaticPool，保持有且仅有一个连接。
-            # 不过这样设置之后，在程序运行期间，你的数据库文件都将被占用。
-            params['poolclass'] = StaticPool
-
-        logger.info("[data source] sql conn url: " + conf.pixiv_sql_conn_url)
-        self._engine = create_async_engine(conf.pixiv_sql_conn_url, **params)
-
-        async with self._engine.begin() as conn:
-            from .migration import SqlMigrationManager
-            from .meta_info import MetaInfo
-
-            await conn.run_sync(lambda conn: MetaInfo.__table__.create(conn, checkfirst=True))
-
-            # migrate
-            mig_mgr = SqlMigrationManager(lambda prev, cur: self._raw_set_db_version(cur, conn))
-            db_version = await self._raw_get_db_version(conn)
-            await mig_mgr.perform_migration(conn, db_version, self.app_db_version)
-
-            await conn.run_sync(lambda conn: self.registry.metadata.create_all(conn))
-
-            await conn.commit()
-
-        # expire_on_commit=False will prevent attributes from being expired
-        # after commit.
-        self._sessionmaker = sessionmaker(self._engine, expire_on_commit=False, class_=AsyncSession)
-
-        logger.success(f"[data source] SqlDataSource Initialized (dialect: {conf.pixiv_sql_dialect})")
-        await self._fire_initialized()
-
-    async def close(self):
-        await self._fire_closing()
-
-        await self._engine.dispose()
-
-        self._engine = None
-        self._sessionmaker = None
-
-        logger.success("[data source] SqlDataSource Disposed.")
-        await self._fire_closed()
-
-    @asynccontextmanager
-    async def start_session(self) -> AsyncContextManager[AsyncSession]:
-        if self._engine is None:
-            raise DataSourceNotReadyError()
-        async with self._sessionmaker() as session:
-            yield session
-
-    @property
-    def engine(self) -> AsyncEngine:
-        if self._engine is None:
-            raise DataSourceNotReadyError()
-        return self._engine
-
-
-__all__ = ("DataSource",)
+import json
+from contextlib import asynccontextmanager
+from datetime import datetime, date
+from typing import AsyncContextManager
+
+from nonebot import get_driver, logger
+from sqlalchemy import select, inspect
+from sqlalchemy.ext.asyncio import create_async_engine, AsyncSession, AsyncEngine, AsyncConnection
+from sqlalchemy.orm import registry, sessionmaker
+from sqlalchemy.pool import StaticPool
+
+from ..lifecycle_mixin import DataSourceLifecycle
+from ...errors import DataSourceNotReadyError
+from ....config import Config
+from ....global_context import context
+from ....utils.lifecycler import on_startup, on_shutdown
+
+conf = context.require(Config)
+
+
+def default_dumps(obj):
+    if isinstance(obj, (datetime, date)):
+        return obj.isoformat()
+
+    return None
+
+
+def json_serializer(obj):
+    return json.dumps(obj, default=default_dumps)
+
+
+@context.register_eager_singleton()
+class DataSource(DataSourceLifecycle):
+    app_db_version = 5
+    registry = registry()
+
+    def __init__(self):
+        super().__init__()
+
+        self._engine = None
+        self._sessionmaker = None
+
+        on_startup(replay=True)(self.initialize)
+        on_shutdown()(self.close)
+
+    async def _raw_get_db_version(self, conn: AsyncConnection) -> int:
+        async with AsyncSession(conn, expire_on_commit=False) as session:
+            from .meta_info import MetaInfo
+
+            # 判断是否初次建库
+            blank_database = not await conn.run_sync(lambda conn: inspect(conn).has_table("subscription"))
+            if blank_database:
+                result = MetaInfo(key="db_version", value=str(self.app_db_version))
+                session.add(result)
+                await session.commit()
+                v = self.app_db_version
+            else:
+                stmt = select(MetaInfo).where(MetaInfo.key == "db_version")
+                result = (await session.execute(stmt)).scalar_one_or_none()
+                if result is None:
+                    result = MetaInfo(key="db_version", value="1")
+                    session.add(result)
+                    await session.commit()
+
+                v = int(result.value)
+        return v
+
+    async def _raw_set_db_version(self, db_version: int, conn: AsyncConnection):
+        from .meta_info import MetaInfo
+        async with AsyncSession(conn, expire_on_commit=False) as session:
+            stmt = select(MetaInfo).where(MetaInfo.key == "db_version")
+            result = (await session.execute(stmt)).scalar_one_or_none()
+            if result is None:
+                result = MetaInfo(key="db_version", value="1")
+                session.add(result)
+
+            result.value = str(db_version)
+            await session.commit()
+
+    async def initialize(self):
+        await self._fire_initializing()
+
+        driver = get_driver()
+
+        params = {
+            # 仅当TRACE模式时回显sql语句
+            'echo': driver.config.log_level == 'TRACE',
+            'future': True,
+            'json_serializer': json_serializer
+        }
+
+        if conf.detect_sql_dialect == 'sqlite':
+            # 使用 SQLite 数据库时，如果在写入时遇到 (sqlite3.OperationalError) database is locked 错误。
+            # 可尝试将 poolclass 设置为 StaticPool，保持有且仅有一个连接。
+            # 不过这样设置之后，在程序运行期间，你的数据库文件都将被占用。
+            params['poolclass'] = StaticPool
+
+        logger.info("[data source] sql conn url: " + conf.pixiv_sql_conn_url)
+        self._engine = create_async_engine(conf.pixiv_sql_conn_url, **params)
+
+        async with self._engine.begin() as conn:
+            from .migration import SqlMigrationManager
+            from .meta_info import MetaInfo
+
+            await conn.run_sync(lambda conn: MetaInfo.__table__.create(conn, checkfirst=True))
+
+            # migrate
+            mig_mgr = SqlMigrationManager(lambda prev, cur: self._raw_set_db_version(cur, conn))
+            db_version = await self._raw_get_db_version(conn)
+            await mig_mgr.perform_migration(conn, db_version, self.app_db_version)
+
+            await conn.run_sync(lambda conn: self.registry.metadata.create_all(conn))
+
+            await conn.commit()
+
+        # expire_on_commit=False will prevent attributes from being expired
+        # after commit.
+        self._sessionmaker = sessionmaker(self._engine, expire_on_commit=False, class_=AsyncSession)
+
+        logger.success(f"[data source] SqlDataSource Initialized (dialect: {conf.pixiv_sql_dialect})")
+        await self._fire_initialized()
+
+    async def close(self):
+        await self._fire_closing()
+
+        await self._engine.dispose()
+
+        self._engine = None
+        self._sessionmaker = None
+
+        logger.success("[data source] SqlDataSource Disposed.")
+        await self._fire_closed()
+
+    @asynccontextmanager
+    async def start_session(self) -> AsyncContextManager[AsyncSession]:
+        if self._engine is None:
+            raise DataSourceNotReadyError()
+        async with self._sessionmaker() as session:
+            yield session
+
+    @property
+    def engine(self) -> AsyncEngine:
+        if self._engine is None:
+            raise DataSourceNotReadyError()
+        return self._engine
+
+
+__all__ = ("DataSource",)
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v2_to_v3.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v2_to_v3.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from typing import Callable, Awaitable
-
-from nonebot import Bot
-from sqlalchemy import text
-from sqlalchemy.ext.asyncio import AsyncConnection
-
-from ...migration_manager import DeferrableMigration
-from ...sql import DataSource
-from .....global_context import context
-from .....utils.lifecycler import on_bot_connect
-from .....utils.nonebot import get_adapter_name
-
-
-class SqlV2ToV3(DeferrableMigration):
-    from_db_version = 2
-    to_db_version = 3
-    safe = True
-
-    async def migrate(self, conn: AsyncConnection, on_migrated: Callable[[], Awaitable[None]]):
-        data_source = context.require(DataSource)
-
-        @on_bot_connect(replay=True, first=True)
-        async def _(bot: Bot):
-            async with AsyncConnection(data_source.engine) as conn:
-                adapter = get_adapter_name(bot)
-                await conn.execute(
-                    text(f"update watch_task set bot=bot || '\:{bot.self_id}' where bot = '{adapter}'; ")
-                )
-                await conn.execute(
-                    text(f"update subscription set bot=bot || '\:{bot.self_id}' where bot = '{adapter}'; ")
-                )
-                await conn.commit()
-
-        @data_source.on_closing
-        async def _():
-            async with AsyncConnection(data_source.engine) as conn:
-                stmt = text("select count(*) from subscription where bot not like '%:%'")
-                cnt = (await conn.execute(stmt)).scalar()
-                if cnt != 0:
-                    return
-
-                stmt = text("select count(*) from watch_task where bot not like '%:%'")
-                cnt = (await conn.execute(stmt)).scalar()
-                if cnt != 0:
-                    return
-
-                await on_migrated()
+from typing import Callable, Awaitable
+
+from nonebot import Bot
+from sqlalchemy import text
+from sqlalchemy.ext.asyncio import AsyncConnection
+
+from ...migration_manager import DeferrableMigration
+from ...sql import DataSource
+from .....global_context import context
+from .....utils.lifecycler import on_bot_connect
+from .....utils.nonebot import get_adapter_name
+
+
+class SqlV2ToV3(DeferrableMigration):
+    from_db_version = 2
+    to_db_version = 3
+    safe = True
+
+    async def migrate(self, conn: AsyncConnection, on_migrated: Callable[[], Awaitable[None]]):
+        data_source = context.require(DataSource)
+
+        @on_bot_connect(replay=True, first=True)
+        async def _(bot: Bot):
+            async with AsyncConnection(data_source.engine) as conn:
+                adapter = get_adapter_name(bot)
+                await conn.execute(
+                    text(f"update watch_task set bot=bot || '\:{bot.self_id}' where bot = '{adapter}'; ")
+                )
+                await conn.execute(
+                    text(f"update subscription set bot=bot || '\:{bot.self_id}' where bot = '{adapter}'; ")
+                )
+                await conn.commit()
+
+        @data_source.on_closing
+        async def _():
+            async with AsyncConnection(data_source.engine) as conn:
+                stmt = text("select count(*) from subscription where bot not like '%:%'")
+                cnt = (await conn.execute(stmt)).scalar()
+                if cnt != 0:
+                    return
+
+                stmt = text("select count(*) from watch_task where bot not like '%:%'")
+                cnt = (await conn.execute(stmt)).scalar()
+                if cnt != 0:
+                    return
+
+                await on_migrated()
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v4_to_v5.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/source/sql/migration/sql_v4_to_v5.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,201 +1,204 @@
-import json
-from typing import Union
-
-from nonebot_plugin_datastore.db import get_engine
-from nonebot_plugin_session import Session, SessionLevel
-from nonebot_plugin_session.model import get_or_add_session_model
-from sqlalchemy import text
-from sqlalchemy.ext.asyncio import AsyncConnection, AsyncSession
-
-from nonebot_plugin_pixivbot import Config
-from nonebot_plugin_pixivbot.global_context import context
-from ...migration_manager import Migration
-
-
-def convert_session(bot: str, subscriber: Union[str, bytes, dict]) -> Session:
-    bot_adapter, bot_id = bot.split(":")
-
-    if not isinstance(subscriber, dict):
-        subscriber = json.loads(subscriber)
-
-    if bot_adapter == "onebot":
-        bot_type = "OneBot V11"
-        platform = "qq"
-        if subscriber["group_id"] is None:
-            level = SessionLevel.LEVEL1
-        else:
-            level = SessionLevel.LEVEL2
-    elif bot_adapter == "kaiheila":
-        bot_type = "Kaiheila"
-        platform = "kaiheila"
-        if subscriber["group_id"] is None:
-            level = SessionLevel.LEVEL1
-        else:
-            level = SessionLevel.LEVEL3
-    elif bot_adapter == "telegram":
-        bot_type = "Telegram"
-        platform = "telegram"
-        if subscriber["group_id"] is None:
-            level = SessionLevel.LEVEL1
-        else:
-            level = SessionLevel.LEVEL3
-    else:
-        raise RuntimeError("Unknown adapter: " + bot_adapter)
-
-    session = Session(bot_id=bot_id, bot_type=bot_type, platform=platform, level=level,
-                      id1=subscriber["user_id"] or "0",
-                      id2=subscriber["group_id"])
-    return session
-
-
-def convert_kwargs(kwargs):
-    if not isinstance(kwargs, dict):
-        kwargs = json.loads(kwargs)
-    else:
-        kwargs = {**kwargs}
-
-    if "sender_user_id" in kwargs:
-        kwargs["sender_user_id"] = str(kwargs["sender_user_id"])
-    return kwargs
-
-
-conf = context.require(Config)
-
-
-class SqlV4ToV5(Migration):
-    from_db_version = 4
-    to_db_version = 5
-
-    async def migrate(self, conn: AsyncConnection):
-        # pixiv binding
-        await conn.execute(text("alter table pixiv_binding rename to pixiv_binding_old;"))
-        await conn.execute(text("""
-            create table pixiv_binding
-            (
-                platform      VARCHAR not null,
-                user_id       VARCHAR not null,
-                pixiv_user_id INTEGER not null,
-                primary key (platform, user_id)
-            );
-        """))
-        await conn.execute(text("update pixiv_binding_old set adapter='qq' where adapter = 'onebot';"))
-        await conn.execute(text("insert into pixiv_binding (platform, user_id, pixiv_user_id)"
-                                "select adapter, user_id, pixiv_user_id from pixiv_binding_old;"))
-        await conn.execute(text("drop table pixiv_binding_old;"))
-
-        # subscription
-        await conn.execute(text("alter table subscription rename to subscription_old;"))
-        if conf.pixiv_sql_dialect == 'postgresql':
-            await conn.execute(text("""
-                create table subscription
-                (
-                    id         INTEGER     not null
-                        primary key default nextval('subscription_id_seq'::regclass),
-                    code       VARCHAR     not null,
-                    session_id INTEGER     not null,
-                    bot_id     VARCHAR     not null,
-                    type       VARCHAR(25) not null,
-                    kwargs     JSON        not null,
-                    schedule   JSON        not null,
-                    tz         VARCHAR     not null,
-                    unique (bot_id, session_id, code)
-                );
-            """))
-            await conn.execute(text("alter sequence subscription_id_seq owned by subscription.id;"))
-        else:
-            await conn.execute(text("""
-                create table subscription
-                (
-                    id         INTEGER     not null
-                        primary key autoincrement,
-                    code       VARCHAR     not null,
-                    session_id INTEGER     not null,
-                    bot_id     VARCHAR     not null,
-                    type       VARCHAR(25) not null,
-                    kwargs     JSON        not null,
-                    schedule   JSON        not null,
-                    tz         VARCHAR     not null,
-                    unique (bot_id, session_id, code)
-                );
-            """))
-
-        async with AsyncSession(get_engine()) as db_sess:
-            result = await conn.execute(
-                text("select id, subscriber, code, type, kwargs, bot, schedule, tz from subscription_old;"))
-
-            for id, subscriber, code, type, kwargs, bot, schedule, tz in result.fetchall():
-                session = convert_session(bot, subscriber)
-                session_id = (await get_or_add_session_model(session, db_sess)).id
-
-                kwargs = convert_kwargs(kwargs)
-                if not isinstance(kwargs, str):
-                    kwargs = json.dumps(kwargs)
-
-                await conn.execute(
-                    text("insert into subscription(id, session_id, code, type, kwargs, bot_id, schedule, tz) "
-                         "values (:id, :session_id, :code, :type, :kwargs, :bot_id, :schedule, :tz);"),
-                    dict(id=id, session_id=session_id, code=code, type=type, kwargs=kwargs, bot_id=session.bot_id,
-                         schedule=schedule, tz=tz)
-                )
-
-        await conn.execute(text("drop table subscription_old;"))
-
-        # watch_task
-        await conn.execute(text("alter table watch_task rename to watch_task_old;"))
-        if conf.pixiv_sql_dialect == 'postgresql':
-            await conn.execute(text("""
-                CREATE TABLE watch_task (
-                    id         INTEGER     not null
-                        primary key default nextval('watch_task_id_seq'::regclass),
-                    session_id INTEGER     not null,
-                    code       VARCHAR     not null,
-                    "type" watchtype NOT NULL,
-                    kwargs jsonb NOT NULL,
-                    bot_id     VARCHAR     not null,
-                    "checkpoint" timestamp NOT NULL,
-                    unique (bot_id, session_id, code),
-                    unique (bot_id, session_id, type, kwargs)
-                );
-            """))
-            await conn.execute(text("alter sequence watch_task_id_seq owned by watch_task.id;"))
-        else:
-            await conn.execute(text("""
-                create table watch_task
-                (
-                    id         INTEGER     not null
-                        primary key autoincrement,
-                    session_id INTEGER     not null,
-                    code       VARCHAR     not null,
-                    type       VARCHAR(17) not null,
-                    kwargs     JSON        not null,
-                    bot_id     VARCHAR     not null,
-                    checkpoint DATETIME    not null,
-                    unique (bot_id, session_id, code),
-                    unique (bot_id, session_id, type, kwargs)
-                );
-            """))
-
-        async with AsyncSession(get_engine()) as db_sess:
-            result = await conn.execute(
-                text("select id, subscriber, code, type, kwargs, bot, checkpoint from watch_task_old;"))
-
-            for id, subscriber, code, type, kwargs, bot, checkpoint in result.fetchall():
-                session = convert_session(bot, subscriber)
-                session_id = (await get_or_add_session_model(session, db_sess)).id
-
-                kwargs = convert_kwargs(kwargs)
-
-                if not isinstance(kwargs, str):
-                    kwargs = json.dumps(kwargs)
-
-                if not isinstance(schedule, str):
-                    schedule = json.dumps(schedule)
-
-                await conn.execute(
-                    text("insert into watch_task(id, session_id, code, type, kwargs, bot_id, checkpoint) "
-                         "values (:id, :session_id, :code, :type, :kwargs, :bot_id, :checkpoint);"),
-                    dict(id=id, session_id=session_id, code=code, type=type, kwargs=kwargs, bot_id=session.bot_id,
-                         checkpoint=checkpoint)
-                )
-
-        await conn.execute(text("drop table watch_task_old;"))
+import json
+from typing import Union
+
+from nonebot_plugin_datastore.db import get_engine
+from nonebot_plugin_session import Session, SessionLevel
+from nonebot_plugin_session.model import get_or_add_session_model
+from sqlalchemy import text
+from sqlalchemy.ext.asyncio import AsyncConnection, AsyncSession
+
+from nonebot_plugin_pixivbot import Config
+from nonebot_plugin_pixivbot.global_context import context
+from ...migration_manager import Migration
+
+
+def convert_session(bot: str, subscriber: Union[str, bytes, dict]) -> Session:
+    bot_adapter, bot_id = bot.split(":")
+
+    if not isinstance(subscriber, dict):
+        subscriber = json.loads(subscriber)
+
+    if bot_adapter == "onebot":
+        bot_type = "OneBot V11"
+        platform = "qq"
+        if subscriber["group_id"] is None:
+            level = SessionLevel.LEVEL1
+        else:
+            level = SessionLevel.LEVEL2
+    elif bot_adapter == "kaiheila":
+        bot_type = "Kaiheila"
+        platform = "kaiheila"
+        if subscriber["group_id"] is None:
+            level = SessionLevel.LEVEL1
+        else:
+            level = SessionLevel.LEVEL3
+    elif bot_adapter == "telegram":
+        bot_type = "Telegram"
+        platform = "telegram"
+        if subscriber["group_id"] is None:
+            level = SessionLevel.LEVEL1
+        else:
+            level = SessionLevel.LEVEL3
+    else:
+        raise RuntimeError("Unknown adapter: " + bot_adapter)
+
+    session = Session(bot_id=bot_id, bot_type=bot_type, platform=platform, level=level, id1=subscriber["user_id"] or "0",
+                      id2=subscriber["group_id"])
+    return session
+
+
+def convert_kwargs(kwargs):
+    if not isinstance(kwargs, dict):
+        kwargs = json.loads(kwargs)
+    else:
+        kwargs = {**kwargs}
+
+    if "sender_user_id" in kwargs:
+        kwargs["sender_user_id"] = str(kwargs["sender_user_id"])
+    return kwargs
+
+
+conf = context.require(Config)
+
+
+class SqlV4ToV5(Migration):
+    from_db_version = 4
+    to_db_version = 5
+
+    async def migrate(self, conn: AsyncConnection):
+        # pixiv binding
+        await conn.execute(text("alter table pixiv_binding rename to pixiv_binding_old;"))
+        await conn.execute(text("""
+            create table pixiv_binding
+            (
+                platform      VARCHAR not null,
+                user_id       VARCHAR not null,
+                pixiv_user_id INTEGER not null,
+                primary key (platform, user_id)
+            );
+        """))
+        await conn.execute(text("update pixiv_binding_old set adapter='qq' where adapter = 'onebot';"))
+        await conn.execute(text("insert into pixiv_binding (platform, user_id, pixiv_user_id)"
+                                "select adapter, user_id, pixiv_user_id from pixiv_binding_old;"))
+        await conn.execute(text("drop table pixiv_binding_old;"))
+
+        # subscription
+        await conn.execute(text("alter table subscription rename to subscription_old;"))
+        if conf.pixiv_sql_dialect == 'postgresql':
+            await conn.execute(text("""
+                create table subscription
+                (
+                    id         INTEGER     not null
+                        primary key default nextval('subscription_id_seq'::regclass),
+                    code       VARCHAR     not null,
+                    session_id INTEGER     not null,
+                    bot_id     VARCHAR     not null,
+                    type       VARCHAR(25) not null,
+                    kwargs     JSON        not null,
+                    schedule   JSON        not null,
+                    tz         VARCHAR     not null,
+                    unique (bot_id, session_id, code)
+                );
+            """))
+            await conn.execute(text("alter sequence subscription_id_seq owned by subscription.id;"))
+        else:
+            await conn.execute(text("""
+                create table subscription
+                (
+                    id         INTEGER     not null
+                        primary key autoincrement,
+                    code       VARCHAR     not null,
+                    session_id INTEGER     not null,
+                    bot_id     VARCHAR     not null,
+                    type       VARCHAR(25) not null,
+                    kwargs     JSON        not null,
+                    schedule   JSON        not null,
+                    tz         VARCHAR     not null,
+                    unique (bot_id, session_id, code)
+                );
+            """))
+
+        async with AsyncSession(get_engine()) as db_sess:
+            result = await conn.execute(
+                text("select id, subscriber, code, type, kwargs, bot, schedule, tz from subscription_old;"))
+
+            for id, subscriber, code, type, kwargs, bot, schedule, tz in result.fetchall():
+                session = convert_session(bot, subscriber)
+                session_id = (await get_or_add_session_model(session, db_sess)).id
+
+                kwargs = convert_kwargs(kwargs)
+
+                if not isinstance(kwargs, str):
+                    kwargs = json.dumps(kwargs)
+
+                if not isinstance(schedule, str):
+                    schedule = json.dumps(schedule)
+
+                await conn.execute(
+                    text("insert into subscription(id, session_id, code, type, kwargs, bot_id, schedule, tz) "
+                         "values (:id, :session_id, :code, :type, :kwargs, :bot_id, :schedule, :tz);"),
+                    dict(id=id, session_id=session_id, code=code, type=type, kwargs=kwargs, bot_id=session.bot_id,
+                         schedule=schedule, tz=tz)
+                )
+
+        await conn.execute(text("drop table subscription_old;"))
+
+        # watch_task
+        await conn.execute(text("alter table watch_task rename to watch_task_old;"))
+        if conf.pixiv_sql_dialect == 'postgresql':
+            await conn.execute(text("""
+                CREATE TABLE watch_task (
+                    id         INTEGER     not null
+                        primary key default nextval('watch_task_id_seq'::regclass),
+                    session_id INTEGER     not null,
+                    code       VARCHAR     not null,
+                    "type" watchtype NOT NULL,
+                    kwargs jsonb NOT NULL,
+                    bot_id     VARCHAR     not null,
+                    "checkpoint" timestamp NOT NULL,
+                    unique (bot_id, session_id, code),
+                    unique (bot_id, session_id, type, kwargs)
+                );
+            """))
+            await conn.execute(text("alter sequence watch_task_id_seq owned by watch_task.id;"))
+        else:
+            await conn.execute(text("""
+                create table watch_task
+                (
+                    id         INTEGER     not null
+                        primary key autoincrement,
+                    session_id INTEGER     not null,
+                    code       VARCHAR     not null,
+                    type       VARCHAR(17) not null,
+                    kwargs     JSON        not null,
+                    bot_id     VARCHAR     not null,
+                    checkpoint DATETIME    not null,
+                    unique (bot_id, session_id, code),
+                    unique (bot_id, session_id, type, kwargs)
+                );
+            """))
+
+        async with AsyncSession(get_engine()) as db_sess:
+            result = await conn.execute(
+                text("select id, subscriber, code, type, kwargs, bot, checkpoint from watch_task_old;"))
+
+            for id, subscriber, code, type, kwargs, bot, checkpoint in result.fetchall():
+                session = convert_session(bot, subscriber)
+                session_id = (await get_or_add_session_model(session, db_sess)).id
+
+                kwargs = convert_kwargs(kwargs)
+
+                if not isinstance(kwargs, str):
+                    kwargs = json.dumps(kwargs)
+
+                if not isinstance(schedule, str):
+                    schedule = json.dumps(schedule)
+
+                await conn.execute(
+                    text("insert into watch_task(id, session_id, code, type, kwargs, bot_id, checkpoint) "
+                         "values (:id, :session_id, :code, :type, :kwargs, :bot_id, :checkpoint);"),
+                    dict(id=id, session_id=session_id, code=code, type=type, kwargs=kwargs, bot_id=session.bot_id,
+                         checkpoint=checkpoint)
+                )
+
+        await conn.execute(text("drop table watch_task_old;"))
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/subscription.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/subscription.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,145 +1,140 @@
-from typing import Optional, AsyncIterable, Collection
-
-import tzlocal
-from nonebot_plugin_session import Session
-from sqlalchemy import select, UniqueConstraint
-from sqlalchemy.orm import mapped_column, Mapped
-
-from .interval_task_repo import IntervalTaskRepo, process_subscriber
-from .nb_session import NbSessionRepo
-from .source.sql import DataSource
-from .utils.shortuuid import gen_code
-from .utils.sql import insert, JSON
-from ..global_context import context
-from ..model import Subscription, ScheduleType
-from ..model.subscription import IntervalSchedule, CronSchedule
-
-
-@DataSource.registry.mapped
-class SubscriptionOrm:
-    __tablename__ = "subscription"
-
-    id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
-    session_id: Mapped[int]
-    code: Mapped[str]
-    type: Mapped[ScheduleType]
-    kwargs: Mapped[dict] = mapped_column(JSON, default=dict)
-    bot_id: Mapped[str]
-    schedule: Mapped[list] = mapped_column(JSON)
-    tz: Mapped[str] = mapped_column(default=tzlocal.get_localzone_name)
-
-    __table_args__ = (
-        UniqueConstraint("bot_id", "session_id", "code"),
-    )
-
-
-data_source = context.require(DataSource)
-nb_session_repo = context.require(NbSessionRepo)
-
-
-async def _to_model(item: SubscriptionOrm) -> Subscription:
-    subscriber = await nb_session_repo.get_session(item.session_id)
-    if len(item.schedule) == 4:
-        schedule = IntervalSchedule(*item.schedule)
-    else:
-        schedule = CronSchedule(*item.schedule)
-    return Subscription(subscriber=subscriber,
-                        code=item.code,
-                        type=item.type,
-                        kwargs=item.kwargs,
-                        schedule=schedule,
-                        tz=item.tz)
-
-
-@context.register_singleton()
-class SubscriptionRepo(IntervalTaskRepo[Subscription]):
-    async def get_by_session(self, session: Session) -> AsyncIterable[Subscription]:
-        session = process_subscriber(session)
-        session_id = await nb_session_repo.get_id(session)
-        async with data_source.start_session() as db_sess:
-            stmt = (
-                select(SubscriptionOrm)
-                .where(SubscriptionOrm.session_id == session_id)
-            )
-            async for x in await db_sess.stream_scalars(stmt):
-                yield await _to_model(x)
-
-    async def get_by_bot(self, bot_id: str) -> AsyncIterable[Subscription]:
-        async with data_source.start_session() as db_sess:
-            stmt = (
-                select(SubscriptionOrm)
-                .where(SubscriptionOrm.bot_id == bot_id)
-            )
-            async for x in await db_sess.stream_scalars(stmt):
-                yield await _to_model(x)
-
-    async def get_by_code(self, session: Session,
-                          code: str) -> Optional[Subscription]:
-        session = process_subscriber(session)
-        session_id = await nb_session_repo.get_id(session)
-        async with data_source.start_session() as db_sess:
-            stmt = (
-                select(SubscriptionOrm)
-                .where(SubscriptionOrm.bot_id == session.bot_id,
-                       SubscriptionOrm.session_id == session_id,
-                       SubscriptionOrm.code == code)
-            )
-            x = (await db_sess.execute(stmt)).scalar_one_or_none()
-            if x is not None:
-                return await _to_model(x)
-            else:
-                return None
-
-    async def insert(self, item: Subscription) -> bool:
-        item.code = gen_code()
-        item.subscriber = process_subscriber(item.subscriber)
-        session_id = await nb_session_repo.get_id(item.subscriber)
-
-        async with data_source.start_session() as db_sess:
-            stmt = (insert(SubscriptionOrm)
-                    .values(session_id=session_id,
-                            code=item.code,
-                            type=item.type,
-                            kwargs=item.kwargs,
-                            bot_id=item.subscriber.bot_id,
-                            schedule=item.schedule,
-                            tz=item.tz))
-            await db_sess.execute(stmt)
-            await db_sess.commit()
-        return True
-
-    async def delete_one(self, session: Session, code: str) -> Optional[Subscription]:
-        session = process_subscriber(session)
-        session_id = await nb_session_repo.get_id(session)
-        async with data_source.start_session() as db_sess:
-            stmt = (select(SubscriptionOrm)
-                    .where(SubscriptionOrm.bot_id == session.bot_id,
-                           SubscriptionOrm.session_id == session_id,
-                           SubscriptionOrm.code == code)
-                    .limit(1))
-            sub = (await db_sess.execute(stmt)).scalar_one_or_none()
-
-            if sub is None:
-                return sub
-
-            await db_sess.delete(sub)
-            await db_sess.commit()
-            return await _to_model(sub)
-
-    async def delete_many_by_session(self, session: Session) -> Collection[Subscription]:
-        session = process_subscriber(session)
-        session_id = await nb_session_repo.get_id(session)
-        async with data_source.start_session() as db_sess:
-            stmt = (select(SubscriptionOrm)
-                    .where(SubscriptionOrm.bot_id == session.bot_id,
-                           SubscriptionOrm.session_id == session_id))
-            subs = (await db_sess.execute(stmt)).scalars().all()
-
-            for t in subs:
-                await db_sess.delete(t)
-
-            await db_sess.commit()
-            return [await _to_model(x) for x in subs]
-
-
-__all__ = ("SubscriptionRepo",)
+from typing import Optional, AsyncIterable, Collection
+
+import tzlocal
+from nonebot_plugin_session import Session
+from sqlalchemy import select, UniqueConstraint
+from sqlalchemy.orm import mapped_column, Mapped
+
+from .interval_task_repo import IntervalTaskRepo, process_subscriber
+from .nb_session import NbSessionRepo
+from .source.sql import DataSource
+from .utils.shortuuid import gen_code
+from .utils.sql import insert, JSON
+from ..global_context import context
+from ..model import Subscription, ScheduleType
+
+
+@DataSource.registry.mapped
+class SubscriptionOrm:
+    __tablename__ = "subscription"
+
+    id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
+    session_id: Mapped[int]
+    code: Mapped[str]
+    type: Mapped[ScheduleType]
+    kwargs: Mapped[dict] = mapped_column(JSON, default=dict)
+    bot_id: Mapped[str]
+    schedule: Mapped[dict] = mapped_column(JSON)
+    tz: Mapped[str] = mapped_column(default=tzlocal.get_localzone_name)
+
+    __table_args__ = (
+        UniqueConstraint("bot_id", "session_id", "code"),
+    )
+
+
+data_source = context.require(DataSource)
+nb_session_repo = context.require(NbSessionRepo)
+
+
+async def _to_model(item: SubscriptionOrm) -> Subscription:
+    subscriber = await nb_session_repo.get_session(item.session_id)
+    return Subscription(subscriber=subscriber,
+                        code=item.code,
+                        type=item.type,
+                        kwargs=item.kwargs,
+                        schedule=item.schedule,
+                        tz=item.tz)
+
+
+@context.register_singleton()
+class SubscriptionRepo(IntervalTaskRepo[Subscription]):
+    async def get_by_session(self, session: Session) -> AsyncIterable[Subscription]:
+        session = process_subscriber(session)
+        session_id = await nb_session_repo.get_id(session)
+        async with data_source.start_session() as db_sess:
+            stmt = (
+                select(SubscriptionOrm)
+                .where(SubscriptionOrm.session_id == session_id)
+            )
+            async for x in await db_sess.stream_scalars(stmt):
+                yield await _to_model(x)
+
+    async def get_by_bot(self, bot_id: str) -> AsyncIterable[Subscription]:
+        async with data_source.start_session() as db_sess:
+            stmt = (
+                select(SubscriptionOrm)
+                .where(SubscriptionOrm.bot_id == bot_id)
+            )
+            async for x in await db_sess.stream_scalars(stmt):
+                yield await _to_model(x)
+
+    async def get_by_code(self, session: Session,
+                          code: str) -> Optional[Subscription]:
+        session = process_subscriber(session)
+        session_id = await nb_session_repo.get_id(session)
+        async with data_source.start_session() as db_sess:
+            stmt = (
+                select(SubscriptionOrm)
+                .where(SubscriptionOrm.bot_id == session.bot_id,
+                       SubscriptionOrm.session_id == session_id,
+                       SubscriptionOrm.code == code)
+            )
+            x = (await db_sess.execute(stmt)).scalar_one_or_none()
+            if x is not None:
+                return await _to_model(x)
+            else:
+                return None
+
+    async def insert(self, item: Subscription) -> bool:
+        item.code = gen_code()
+        item.subscriber = process_subscriber(item.subscriber)
+        session_id = await nb_session_repo.get_id(item.subscriber)
+
+        async with data_source.start_session() as db_sess:
+            stmt = (insert(SubscriptionOrm)
+                    .values(session_id=session_id,
+                            code=item.code,
+                            type=item.type,
+                            kwargs=item.kwargs,
+                            bot_id=item.subscriber.bot_id,
+                            schedule=item.schedule,
+                            tz=item.tz))
+            await db_sess.execute(stmt)
+            await db_sess.commit()
+        return True
+
+    async def delete_one(self, session: Session, code: str) -> Optional[Subscription]:
+        session = process_subscriber(session)
+        session_id = await nb_session_repo.get_id(session)
+        async with data_source.start_session() as db_sess:
+            stmt = (select(SubscriptionOrm)
+                    .where(SubscriptionOrm.bot_id == session.bot_id,
+                           SubscriptionOrm.session_id == session_id,
+                           SubscriptionOrm.code == code)
+                    .limit(1))
+            sub = (await db_sess.execute(stmt)).scalar_one_or_none()
+
+            if sub is None:
+                return sub
+
+            await db_sess.delete(sub)
+            await db_sess.commit()
+            return await _to_model(sub)
+
+    async def delete_many_by_session(self, session: Session) -> Collection[Subscription]:
+        session = process_subscriber(session)
+        session_id = await nb_session_repo.get_id(session)
+        async with data_source.start_session() as db_sess:
+            stmt = (select(SubscriptionOrm)
+                    .where(SubscriptionOrm.bot_id == session.bot_id,
+                           SubscriptionOrm.session_id == session_id))
+            subs = (await db_sess.execute(stmt)).scalars().all()
+
+            for t in subs:
+                await db_sess.delete(t)
+
+            await db_sess.commit()
+            return [await _to_model(x) for x in subs]
+
+
+__all__ = ("SubscriptionRepo",)
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/utils/sql/__init__.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/utils/sql/__init__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from nonebot_plugin_pixivbot.config import Config
-from nonebot_plugin_pixivbot.global_context import context
-
-dialect = context.require(Config).pixiv_sql_dialect
-if dialect == 'sqlite':
-    from sqlalchemy.dialects.sqlite import insert as _insert
-    from sqlalchemy.dialects.sqlite import JSON as _JSON
-    from sqlalchemy.dialects.sqlite import BLOB as _BLOB
-elif dialect == 'postgresql':
-    from sqlalchemy.dialects.postgresql import insert as _insert
-    from sqlalchemy.dialects.postgresql import JSONB as _JSON
-    from sqlalchemy.dialects.postgresql import BYTEA as _BLOB
-else:
-    raise RuntimeError(f"不支持使用此SQL数据库：{dialect}")
-
-insert = _insert
-JSON = _JSON
-BLOB = _BLOB
-
-from .utc_datetime import UTCDateTime
-
-__all__ = ("insert", "JSON", "BLOB", "UTCDateTime")
+from nonebot_plugin_pixivbot.config import Config
+from nonebot_plugin_pixivbot.global_context import context
+
+dialect = context.require(Config).pixiv_sql_dialect
+if dialect == 'sqlite':
+    from sqlalchemy.dialects.sqlite import insert as _insert
+    from sqlalchemy.dialects.sqlite import JSON as _JSON
+    from sqlalchemy.dialects.sqlite import BLOB as _BLOB
+elif dialect == 'postgresql':
+    from sqlalchemy.dialects.postgresql import insert as _insert
+    from sqlalchemy.dialects.postgresql import JSONB as _JSON
+    from sqlalchemy.dialects.postgresql import BYTEA as _BLOB
+else:
+    raise RuntimeError(f"不支持使用此SQL数据库：{dialect}")
+
+insert = _insert
+JSON = _JSON
+BLOB = _BLOB
+
+from .utc_datetime import UTCDateTime
+
+__all__ = ("insert", "JSON", "BLOB", "UTCDateTime")
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/utils/sql.pyi` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/utils/sql.pyi`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Union
-
-from sqlalchemy import BLOB as StandardBLOB
-from sqlalchemy import DateTime as StandardDateTime
-from sqlalchemy import JSON as StandardJSON
-from sqlalchemy.dialects.mysql import Insert as MysqlInsert
-from sqlalchemy.dialects.postgresql import BYTEA as PostgresqlBYTEA
-from sqlalchemy.dialects.postgresql import Insert as PostgresqlInsert
-from sqlalchemy.dialects.sqlite import Insert as SqliteInsert
-from sqlalchemy.sql import Insert as StandardInsert
-
-insert = Union[StandardInsert, PostgresqlInsert, SqliteInsert, MysqlInsert]
-JSON = StandardJSON
-BLOB = Union[StandardBLOB, PostgresqlBYTEA]
-UTCDateTime = StandardDateTime
-
-__all__ = ("insert", "JSON", "BLOB", "UTCDateTime")
+from typing import Union
+
+from sqlalchemy import BLOB as StandardBLOB
+from sqlalchemy import DateTime as StandardDateTime
+from sqlalchemy import JSON as StandardJSON
+from sqlalchemy.dialects.mysql import Insert as MysqlInsert
+from sqlalchemy.dialects.postgresql import BYTEA as PostgresqlBYTEA
+from sqlalchemy.dialects.postgresql import Insert as PostgresqlInsert
+from sqlalchemy.dialects.sqlite import Insert as SqliteInsert
+from sqlalchemy.sql import Insert as StandardInsert
+
+insert = Union[StandardInsert, PostgresqlInsert, SqliteInsert, MysqlInsert]
+JSON = StandardJSON
+BLOB = Union[StandardBLOB, PostgresqlBYTEA]
+UTCDateTime = StandardDateTime
+
+__all__ = ("insert", "JSON", "BLOB", "UTCDateTime")
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/data/watch_task.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/data/watch_task.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,155 +1,155 @@
-from datetime import datetime
-from typing import Optional, AsyncIterable, Collection
-
-from nonebot_plugin_session import Session
-from pytz import utc
-from sqlalchemy import select, UniqueConstraint, update
-from sqlalchemy.orm import mapped_column, Mapped
-
-from .interval_task_repo import IntervalTaskRepo, process_subscriber
-from .nb_session import NbSessionRepo
-from .source.sql import DataSource
-from .utils.shortuuid import gen_code
-from .utils.sql import insert, JSON, UTCDateTime
-from ..global_context import context
-from ..model import WatchType, WatchTask
-
-
-@DataSource.registry.mapped
-class WatchTaskOrm:
-    __tablename__ = "watch_task"
-
-    id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
-    session_id: Mapped[int]
-    code: Mapped[str]
-    type: Mapped[WatchType]
-    kwargs: Mapped[dict] = mapped_column(JSON, default=dict)
-    bot_id: Mapped[str]
-    checkpoint: Mapped[datetime] = mapped_column(UTCDateTime)
-
-    __table_args__ = (
-        UniqueConstraint("bot_id", "session_id", "code"),
-        UniqueConstraint("bot_id", "session_id", "type", "kwargs"),
-    )
-
-
-data_source = context.require(DataSource)
-nb_session_repo = context.require(NbSessionRepo)
-
-
-async def _to_model(item: WatchTaskOrm) -> WatchTask:
-    subscriber = await nb_session_repo.get_session(item.session_id)
-    return WatchTask(subscriber=subscriber,
-                     code=item.code,
-                     type=item.type,
-                     kwargs=item.kwargs,
-                     checkpoint=item.checkpoint)
-
-
-@context.register_singleton()
-class WatchTaskRepo(IntervalTaskRepo[WatchTask]):
-    async def get_by_session(self, session: Session) -> AsyncIterable[WatchTask]:
-        session = process_subscriber(session)
-        session_id = await nb_session_repo.get_id(session)
-        async with data_source.start_session() as db_sess:
-            stmt = (
-                select(WatchTaskOrm)
-                .where(WatchTaskOrm.bot_id == session.bot_id,
-                       WatchTaskOrm.session_id == session_id)
-            )
-            async for x in await db_sess.stream_scalars(stmt):
-                x.checkpoint = x.checkpoint.replace(tzinfo=utc)
-                yield await _to_model(x)
-
-    async def get_by_bot(self, bot_id: str) -> AsyncIterable[WatchTask]:
-        async with data_source.start_session() as db_sess:
-            stmt = (
-                select(WatchTaskOrm)
-                .where(WatchTaskOrm.bot_id == bot_id)
-            )
-            async for x in await db_sess.stream_scalars(stmt):
-                x.checkpoint = x.checkpoint.replace(tzinfo=utc)
-                yield await _to_model(x)
-
-    async def get_by_code(self, session: Session,
-                          code: str) -> Optional[WatchTask]:
-        session = process_subscriber(session)
-        session_id = await nb_session_repo.get_id(session)
-        async with data_source.start_session() as db_sess:
-            stmt = (select(WatchTaskOrm)
-                    .where(WatchTaskOrm.bot_id == session.bot_id,
-                           WatchTaskOrm.session_id == session_id,
-                           WatchTaskOrm.code == code))
-            result = (await db_sess.execute(stmt)).scalar_one_or_none()
-            result.checkpoint = result.checkpoint.replace(tzinfo=utc)
-            return await _to_model(result)
-
-    async def insert(self, item: WatchTask) -> bool:
-        item.code = gen_code()
-        item.subscriber = process_subscriber(item.subscriber)
-        session_id = await nb_session_repo.get_id(item.subscriber)
-
-        async with data_source.start_session() as db_session:
-            stmt = (insert(WatchTaskOrm)
-                    .values(session_id=session_id,
-                            code=item.code,
-                            type=item.type,
-                            kwargs=item.kwargs,
-                            bot_id=item.subscriber.bot_id,
-                            checkpoint=item.checkpoint))
-            stmt = stmt.on_conflict_do_nothing()
-            result = await db_session.execute(stmt)
-            await db_session.commit()
-
-            return result.rowcount == 1
-
-    async def update(self, item: WatchTask) -> bool:
-        item.subscriber = process_subscriber(item.subscriber)
-        session_id = await nb_session_repo.get_id(item.subscriber)
-        async with data_source.start_session() as db_session:
-            stmt = (update(WatchTaskOrm)
-                    .values(type=item.type,
-                            kwargs=item.kwargs,
-                            bot_id=item.subscriber.bot_id,
-                            checkpoint=item.checkpoint)
-                    .where(WatchTaskOrm.session_id == session_id,
-                           WatchTaskOrm.code == item.code))
-            result = await db_session.execute(stmt)
-            await db_session.commit()
-            return result.rowcount == 1
-
-    async def delete_one(self, session: Session, code: str) -> Optional[WatchTask]:
-        session = process_subscriber(session)
-        session_id = await nb_session_repo.get_id(session)
-        async with data_source.start_session() as db_sess:
-            stmt = (select(WatchTaskOrm)
-                    .where(WatchTaskOrm.bot_id == session.bot_id,
-                           WatchTaskOrm.session_id == session_id,
-                           WatchTaskOrm.code == code)
-                    .limit(1))
-            task = (await db_sess.execute(stmt)).scalar_one_or_none()
-
-            if task is None:
-                return task
-
-            await db_sess.delete(task)
-            await db_sess.commit()
-            return await _to_model(task)
-
-    async def delete_many_by_session(self, session: Session) -> Collection[WatchTask]:
-        session = process_subscriber(session)
-        session_id = await nb_session_repo.get_id(session)
-        async with data_source.start_session() as db_sess:
-            stmt = (select(WatchTaskOrm)
-                    .where(WatchTaskOrm.bot_id == session.bot_id,
-                           WatchTaskOrm.session_id == session_id))
-            tasks = (await db_sess.execute(stmt)).scalars().all()
-
-            for t in tasks:
-                await db_sess.delete(t)
-
-            await db_sess.commit()
-            return [await _to_model(x) for x in tasks]
-
-
-__all__ = ("WatchTaskRepo",)
+from datetime import datetime
+from typing import Optional, AsyncIterable, Collection
+
+from nonebot_plugin_session import Session
+from pytz import utc
+from sqlalchemy import select, UniqueConstraint, update
+from sqlalchemy.orm import mapped_column, Mapped
+
+from .interval_task_repo import IntervalTaskRepo, process_subscriber
+from .nb_session import NbSessionRepo
+from .source.sql import DataSource
+from .utils.shortuuid import gen_code
+from .utils.sql import insert, JSON, UTCDateTime
+from ..global_context import context
+from ..model import WatchType, WatchTask
+
+
+@DataSource.registry.mapped
+class WatchTaskOrm:
+    __tablename__ = "watch_task"
+
+    id: Mapped[int] = mapped_column(primary_key=True, autoincrement=True)
+    session_id: Mapped[int]
+    code: Mapped[str]
+    type: Mapped[WatchType]
+    kwargs: Mapped[dict] = mapped_column(JSON, default=dict)
+    bot_id: Mapped[str]
+    checkpoint: Mapped[datetime] = mapped_column(UTCDateTime)
+
+    __table_args__ = (
+        UniqueConstraint("bot_id", "session_id", "code"),
+        UniqueConstraint("bot_id", "session_id", "type", "kwargs"),
+    )
+
+
+data_source = context.require(DataSource)
+nb_session_repo = context.require(NbSessionRepo)
+
+
+async def _to_model(item: WatchTaskOrm) -> WatchTask:
+    subscriber = await nb_session_repo.get_session(item.session_id)
+    return WatchTask(subscriber=subscriber,
+                     code=item.code,
+                     type=item.type,
+                     kwargs=item.kwargs,
+                     checkpoint=item.checkpoint)
+
+
+@context.register_singleton()
+class WatchTaskRepo(IntervalTaskRepo[WatchTask]):
+    async def get_by_session(self, session: Session) -> AsyncIterable[WatchTask]:
+        session = process_subscriber(session)
+        session_id = await nb_session_repo.get_id(session)
+        async with data_source.start_session() as db_sess:
+            stmt = (
+                select(WatchTaskOrm)
+                .where(WatchTaskOrm.bot_id == session.bot_id,
+                       WatchTaskOrm.session_id == session_id)
+            )
+            async for x in await db_sess.stream_scalars(stmt):
+                x.checkpoint = x.checkpoint.replace(tzinfo=utc)
+                yield await _to_model(x)
+
+    async def get_by_bot(self, bot_id: str) -> AsyncIterable[WatchTask]:
+        async with data_source.start_session() as db_sess:
+            stmt = (
+                select(WatchTaskOrm)
+                .where(WatchTaskOrm.bot_id == bot_id)
+            )
+            async for x in await db_sess.stream_scalars(stmt):
+                x.checkpoint = x.checkpoint.replace(tzinfo=utc)
+                yield await _to_model(x)
+
+    async def get_by_code(self, session: Session,
+                          code: str) -> Optional[WatchTask]:
+        session = process_subscriber(session)
+        session_id = await nb_session_repo.get_id(session)
+        async with data_source.start_session() as db_sess:
+            stmt = (select(WatchTaskOrm)
+                    .where(WatchTaskOrm.bot_id == session.bot_id,
+                           WatchTaskOrm.session_id == session_id,
+                           WatchTaskOrm.code == code))
+            result = (await db_sess.execute(stmt)).scalar_one_or_none()
+            result.checkpoint = result.checkpoint.replace(tzinfo=utc)
+            return await _to_model(result)
+
+    async def insert(self, item: WatchTask) -> bool:
+        item.code = gen_code()
+        item.subscriber = process_subscriber(item.subscriber)
+        session_id = await nb_session_repo.get_id(item.subscriber)
+
+        async with data_source.start_session() as db_session:
+            stmt = (insert(WatchTaskOrm)
+                    .values(session_id=session_id,
+                            code=item.code,
+                            type=item.type,
+                            kwargs=item.kwargs,
+                            bot_id=item.subscriber.bot_id,
+                            checkpoint=item.checkpoint))
+            stmt = stmt.on_conflict_do_nothing()
+            result = await db_session.execute(stmt)
+            await db_session.commit()
+
+            return result.rowcount == 1
+
+    async def update(self, item: WatchTask) -> bool:
+        item.subscriber = process_subscriber(item.subscriber)
+        session_id = await nb_session_repo.get_id(item.subscriber)
+        async with data_source.start_session() as db_session:
+            stmt = (update(WatchTaskOrm)
+                    .values(type=item.type,
+                            kwargs=item.kwargs,
+                            bot_id=item.subscriber.bot_id,
+                            checkpoint=item.checkpoint)
+                    .where(WatchTaskOrm.session_id == session_id,
+                           WatchTaskOrm.code == item.code))
+            result = await db_session.execute(stmt)
+            await db_session.commit()
+            return result.rowcount == 1
+
+    async def delete_one(self, session: Session, code: str) -> Optional[WatchTask]:
+        session = process_subscriber(session)
+        session_id = await nb_session_repo.get_id(session)
+        async with data_source.start_session() as db_sess:
+            stmt = (select(WatchTaskOrm)
+                    .where(WatchTaskOrm.bot_id == session.bot_id,
+                           WatchTaskOrm.session_id == session_id,
+                           WatchTaskOrm.code == code)
+                    .limit(1))
+            task = (await db_sess.execute(stmt)).scalar_one_or_none()
+
+            if task is None:
+                return task
+
+            await db_sess.delete(task)
+            await db_sess.commit()
+            return await _to_model(task)
+
+    async def delete_many_by_session(self, session: Session) -> Collection[WatchTask]:
+        session = process_subscriber(session)
+        session_id = await nb_session_repo.get_id(session)
+        async with data_source.start_session() as db_sess:
+            stmt = (select(WatchTaskOrm)
+                    .where(WatchTaskOrm.bot_id == session.bot_id,
+                           WatchTaskOrm.session_id == session_id))
+            tasks = (await db_sess.execute(stmt)).scalars().all()
+
+            for t in tasks:
+                await db_sess.delete(t)
+
+            await db_sess.commit()
+            return [await _to_model(x) for x in tasks]
+
+
+__all__ = ("WatchTaskRepo",)
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/enums.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/enums.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from enum import Enum
-
-__all__ = ("BlockAction", "DownloadQuantity", "RandomIllustMethod", "RankingMode",)
-
-
-class BlockAction(str, Enum):
-    no_image = 'no_image'
-    completely_block = 'completely_block'
-    no_reply = 'no_reply'
-
-
-class DownloadQuantity(str, Enum):
-    original = 'original'
-    square_medium = 'square_medium'
-    medium = 'medium'
-    large = 'large'
-
-
-class RandomIllustMethod(str, Enum):
-    uniform = 'uniform'
-    bookmark_proportion = 'bookmark_proportion'
-    view_proportion = 'view_proportion'
-    timedelta_proportion = 'timedelta_proportion'
-
-
-class RankingMode(str, Enum):
-    day = 'day'
-    week = 'week'
-    month = 'month'
-    day_male = 'day_male'
-    day_female = 'day_female'
-    week_original = 'week_original'
-    week_rookie = 'week_rookie'
-    day_manga = 'day_manga'
-    day_ai = 'day_ai'
+from enum import Enum
+
+__all__ = ("BlockAction", "DownloadQuantity", "RandomIllustMethod", "RankingMode",)
+
+
+class BlockAction(str, Enum):
+    no_image = 'no_image'
+    completely_block = 'completely_block'
+    no_reply = 'no_reply'
+
+
+class DownloadQuantity(str, Enum):
+    original = 'original'
+    square_medium = 'square_medium'
+    medium = 'medium'
+    large = 'large'
+
+
+class RandomIllustMethod(str, Enum):
+    uniform = 'uniform'
+    bookmark_proportion = 'bookmark_proportion'
+    view_proportion = 'view_proportion'
+    timedelta_proportion = 'timedelta_proportion'
+
+
+class RankingMode(str, Enum):
+    day = 'day'
+    week = 'week'
+    month = 'month'
+    day_male = 'day_male'
+    day_female = 'day_female'
+    week_original = 'week_original'
+    week_rookie = 'week_rookie'
+    day_manga = 'day_manga'
+    day_ai = 'day_ai'
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/base.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/base.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,233 +1,233 @@
-from abc import ABC, abstractmethod, ABCMeta
-from asyncio import Event
-from typing import Sequence, Optional
-from typing import Type
-
-from nonebot import logger
-from nonebot_plugin_access_control.subject.extractor import extract_subjects_from_session
-from nonebot_plugin_session import Session
-
-from .interceptor.base import Interceptor, DummyInterceptor
-from .interceptor.combined_interceptor import CombinedInterceptor
-from .interceptor.default_error_interceptor import DefaultErrorInterceptor
-from .interceptor.service_interceptor import ServiceInterceptor
-from .pkg_context import context
-from ..config import Config
-from ..model import Illust
-from ..model.message import IllustMessagesModel
-from ..plugin_service import r18_service, r18g_service
-from ..service.postman import Postman
-from ..utils.algorithm import as_unique
-
-conf = context.require(Config)
-
-
-def _log_interceptors(cls: Type["Handler"]):
-    if isinstance(cls.interceptor, CombinedInterceptor):
-        logger.trace(
-            f"{cls.__name__}: apply interceptors [{', '.join(map(lambda x: type(x).__name__, cls.interceptor.flat()))}]")
-    else:
-        logger.trace(f"{cls.__name__}: apply interceptors [{type(cls.interceptor).__name__}]")
-
-
-class HandlerMeta(ABCMeta):
-    interceptor: Interceptor
-
-    def __new__(mcs, name, bases, namespace, **kwargs):
-        interceptors = []
-
-        if not kwargs.get("overwrite_interceptors", False):
-            for base_cls in bases:
-                if isinstance(base_cls, HandlerMeta):
-                    if isinstance(base_cls.interceptor, CombinedInterceptor):
-                        interceptors.extend(base_cls.interceptor.flat())
-                    elif isinstance(base_cls.interceptor, DummyInterceptor):
-                        pass
-                    else:
-                        interceptors.append(base_cls.interceptor)
-
-        if "interceptors" in kwargs:
-            interceptors.extend(kwargs["interceptors"])
-            del kwargs["interceptors"]
-
-        if "service" in kwargs:
-            service = kwargs["service"]
-            del kwargs["service"]
-
-            if "service_interceptor_kwargs" in kwargs:
-                service_interceptor_kwargs = kwargs["service_interceptor_kwargs"]
-                del kwargs["service_interceptor_kwargs"]
-            else:
-                service_interceptor_kwargs = {}
-
-            interceptors.insert(0, ServiceInterceptor(service, **service_interceptor_kwargs))
-
-        interceptors = as_unique(interceptors)
-
-        cls = super().__new__(mcs, name, bases, namespace, **kwargs)
-
-        if len(interceptors) == 0:
-            cls.interceptor = DummyInterceptor()
-        elif len(interceptors) == 1:
-            cls.interceptor = interceptors[0]
-        else:
-            cls.interceptor = CombinedInterceptor.from_iterable(interceptors)
-
-        _log_interceptors(cls)
-
-        return cls
-
-
-class Handler(ABC, metaclass=HandlerMeta):
-    interceptor: Interceptor
-
-    def __init__(self, session: Session, event: Optional[Event] = None,
-                 *, silently: bool = False,
-                 disable_interceptors: bool = False):
-        self.session = session
-        self.event = event
-        self.silently = silently
-        self.disable_interceptors = disable_interceptors
-
-    @classmethod
-    @abstractmethod
-    def type(cls) -> str:
-        raise NotImplementedError()
-
-    @classmethod
-    def enabled(cls) -> bool:
-        return True
-
-    async def parse_args(self, args: Sequence[str]) -> dict:
-        """
-        将位置参数转化为命名参数
-        :param args: 位置参数sequence
-        :return: 命名参数dict
-        """
-        return {}
-
-    async def handle(self, *args, **kwargs):
-        if not self.disable_interceptors:
-            await self.interceptor.intercept(self, self._parse_args_and_actual_handle, *args, **kwargs)
-        else:
-            await self._parse_args_and_actual_handle(*args, **kwargs)
-
-    async def handle_with_parsed_args(self, **kwargs):
-        if not self.disable_interceptors:
-            await self.interceptor.intercept(self, self.actual_handle, **kwargs)
-        else:
-            await self.actual_handle(**kwargs)
-
-    async def _parse_args_and_actual_handle(self, *args, **kwargs):
-        parsed_kwargs = await self.parse_args(args)
-        kwargs = {**kwargs, **parsed_kwargs}
-        await self.actual_handle(**kwargs)
-
-    @abstractmethod
-    async def actual_handle(self, **kwargs):
-        """
-        处理指令
-        :param kwargs: 参数dict
-        """
-        raise NotImplementedError()
-
-    @classmethod
-    def add_interceptor_before(cls, interceptor: Interceptor, before: Interceptor):
-        """
-        添加一个拦截器到指定拦截器之前
-
-        :param interceptor:
-        :param before: 指定添加到哪个拦截器之前
-        """
-        if isinstance(cls.interceptor, CombinedInterceptor):
-            itcps = list(cls.interceptor.flat())
-            for i, itcp in enumerate(itcps):
-                if itcp is before:
-                    cls.interceptor = CombinedInterceptor.from_iterable([
-                        *itcps[:i], interceptor, *itcps[i:]
-                    ])
-                    break
-            else:
-                raise ValueError("the interceptor specified by \'before\' argument was not found")
-        elif cls.interceptor is before:
-            cls.interceptor = CombinedInterceptor(interceptor, cls.interceptor)
-        else:
-            raise ValueError("the interceptor specified by \'before\' argument was not found")
-
-        _log_interceptors(cls)
-
-    @classmethod
-    def add_interceptor_after(cls, interceptor: Interceptor, after: Interceptor):
-        """
-        添加一个拦截器到指定拦截器之后
-
-        :param interceptor:
-        :param after: 指定添加到哪个拦截器之后
-        """
-        if isinstance(cls.interceptor, CombinedInterceptor):
-            itcps = list(cls.interceptor.flat())
-            for i, itcp in enumerate(itcps):
-                if itcp is after:
-                    cls.interceptor = CombinedInterceptor.from_iterable([
-                        *itcps[:i + 1], interceptor, *itcps[i + 1:]
-                    ])
-                    break
-            else:
-                raise ValueError("the interceptor specified by \'after\' argument was not found")
-        elif cls.interceptor is after:
-            cls.interceptor = CombinedInterceptor(cls.interceptor, interceptor)
-        else:
-            raise ValueError("the interceptor specified by \'after\' argument was not found")
-
-        _log_interceptors(cls)
-
-    @classmethod
-    def add_interceptor(cls, interceptor: Interceptor, front: bool = False):
-        """
-        添加一个拦截器
-
-        :param interceptor:
-        :param front: 添加到最前
-        """
-        if front:
-            cls.interceptor = CombinedInterceptor(interceptor, cls.interceptor)
-        else:
-            cls.interceptor = CombinedInterceptor(cls.interceptor, interceptor)
-        _log_interceptors(cls)
-
-    async def is_r18_allowed(self) -> bool:
-        return await r18_service.check_by_subject(*extract_subjects_from_session(self.session),
-                                                  acquire_rate_limit_token=False)
-
-    async def is_r18g_allowed(self) -> bool:
-        return await r18g_service.check_by_subject(*extract_subjects_from_session(self.session),
-                                                   acquire_rate_limit_token=False)
-
-    async def post_plain_text(self, message: str):
-        await context.require(Postman).post_plain_text(message, self.session, self.event)
-
-    async def post_illust(self, illust: Illust, *,
-                          header: Optional[str] = None,
-                          number: Optional[int] = None):
-        model = await IllustMessagesModel.from_illust(illust, header=header, number=number,
-                                                      max_page=conf.pixiv_max_item_per_query,
-                                                      block_r18=(not await self.is_r18_allowed()),
-                                                      block_r18g=(not await self.is_r18g_allowed()))
-        if model:
-            await context.require(Postman).post_illusts(model, self.session, self.event)
-
-    async def post_illusts(self, illusts: Sequence[Illust], *,
-                           header: Optional[str] = None,
-                           number: Optional[int] = None):
-        if len(illusts) == 1:
-            await self.post_illust(illusts[0], header=header, number=number)
-        else:
-            model = await IllustMessagesModel.from_illusts(illusts, header=header, number=number,
-                                                           block_r18=(not await self.is_r18_allowed()),
-                                                           block_r18g=(not await self.is_r18g_allowed()))
-            if model:
-                await context.require(Postman).post_illusts(model, self.session, self.event)
-
-
-class EntryHandler(Handler, ABC, interceptors=[context.require(DefaultErrorInterceptor)]):
-    pass
+from abc import ABC, abstractmethod, ABCMeta
+from asyncio import Event
+from typing import Sequence, Optional
+from typing import Type
+
+from nonebot import logger
+from nonebot_plugin_access_control.subject.extractor import extract_subjects_from_session
+from nonebot_plugin_session import Session
+
+from .interceptor.base import Interceptor, DummyInterceptor
+from .interceptor.combined_interceptor import CombinedInterceptor
+from .interceptor.default_error_interceptor import DefaultErrorInterceptor
+from .interceptor.service_interceptor import ServiceInterceptor
+from .pkg_context import context
+from ..config import Config
+from ..model import Illust
+from ..model.message import IllustMessagesModel
+from ..plugin_service import r18_service, r18g_service
+from ..service.postman import Postman
+from ..utils.algorithm import as_unique
+
+conf = context.require(Config)
+
+
+def _log_interceptors(cls: Type["Handler"]):
+    if isinstance(cls.interceptor, CombinedInterceptor):
+        logger.trace(
+            f"{cls.__name__}: apply interceptors [{', '.join(map(lambda x: type(x).__name__, cls.interceptor.flat()))}]")
+    else:
+        logger.trace(f"{cls.__name__}: apply interceptors [{type(cls.interceptor).__name__}]")
+
+
+class HandlerMeta(ABCMeta):
+    interceptor: Interceptor
+
+    def __new__(mcs, name, bases, namespace, **kwargs):
+        interceptors = []
+
+        if not kwargs.get("overwrite_interceptors", False):
+            for base_cls in bases:
+                if isinstance(base_cls, HandlerMeta):
+                    if isinstance(base_cls.interceptor, CombinedInterceptor):
+                        interceptors.extend(base_cls.interceptor.flat())
+                    elif isinstance(base_cls.interceptor, DummyInterceptor):
+                        pass
+                    else:
+                        interceptors.append(base_cls.interceptor)
+
+        if "interceptors" in kwargs:
+            interceptors.extend(kwargs["interceptors"])
+            del kwargs["interceptors"]
+
+        if "service" in kwargs:
+            service = kwargs["service"]
+            del kwargs["service"]
+
+            if "service_interceptor_kwargs" in kwargs:
+                service_interceptor_kwargs = kwargs["service_interceptor_kwargs"]
+                del kwargs["service_interceptor_kwargs"]
+            else:
+                service_interceptor_kwargs = {}
+
+            interceptors.insert(0, ServiceInterceptor(service, **service_interceptor_kwargs))
+
+        interceptors = as_unique(interceptors)
+
+        cls = super().__new__(mcs, name, bases, namespace, **kwargs)
+
+        if len(interceptors) == 0:
+            cls.interceptor = DummyInterceptor()
+        elif len(interceptors) == 1:
+            cls.interceptor = interceptors[0]
+        else:
+            cls.interceptor = CombinedInterceptor.from_iterable(interceptors)
+
+        _log_interceptors(cls)
+
+        return cls
+
+
+class Handler(ABC, metaclass=HandlerMeta):
+    interceptor: Interceptor
+
+    def __init__(self, session: Session, event: Optional[Event] = None,
+                 *, silently: bool = False,
+                 disable_interceptors: bool = False):
+        self.session = session
+        self.event = event
+        self.silently = silently
+        self.disable_interceptors = disable_interceptors
+
+    @classmethod
+    @abstractmethod
+    def type(cls) -> str:
+        raise NotImplementedError()
+
+    @classmethod
+    def enabled(cls) -> bool:
+        return True
+
+    async def parse_args(self, args: Sequence[str]) -> dict:
+        """
+        将位置参数转化为命名参数
+        :param args: 位置参数sequence
+        :return: 命名参数dict
+        """
+        return {}
+
+    async def handle(self, *args, **kwargs):
+        if not self.disable_interceptors:
+            await self.interceptor.intercept(self, self._parse_args_and_actual_handle, *args, **kwargs)
+        else:
+            await self._parse_args_and_actual_handle(*args, **kwargs)
+
+    async def handle_with_parsed_args(self, **kwargs):
+        if not self.disable_interceptors:
+            await self.interceptor.intercept(self, self.actual_handle, **kwargs)
+        else:
+            await self.actual_handle(**kwargs)
+
+    async def _parse_args_and_actual_handle(self, *args, **kwargs):
+        parsed_kwargs = await self.parse_args(args)
+        kwargs = {**kwargs, **parsed_kwargs}
+        await self.actual_handle(**kwargs)
+
+    @abstractmethod
+    async def actual_handle(self, **kwargs):
+        """
+        处理指令
+        :param kwargs: 参数dict
+        """
+        raise NotImplementedError()
+
+    @classmethod
+    def add_interceptor_before(cls, interceptor: Interceptor, before: Interceptor):
+        """
+        添加一个拦截器到指定拦截器之前
+
+        :param interceptor:
+        :param before: 指定添加到哪个拦截器之前
+        """
+        if isinstance(cls.interceptor, CombinedInterceptor):
+            itcps = list(cls.interceptor.flat())
+            for i, itcp in enumerate(itcps):
+                if itcp is before:
+                    cls.interceptor = CombinedInterceptor.from_iterable([
+                        *itcps[:i], interceptor, *itcps[i:]
+                    ])
+                    break
+            else:
+                raise ValueError("the interceptor specified by \'before\' argument was not found")
+        elif cls.interceptor is before:
+            cls.interceptor = CombinedInterceptor(interceptor, cls.interceptor)
+        else:
+            raise ValueError("the interceptor specified by \'before\' argument was not found")
+
+        _log_interceptors(cls)
+
+    @classmethod
+    def add_interceptor_after(cls, interceptor: Interceptor, after: Interceptor):
+        """
+        添加一个拦截器到指定拦截器之后
+
+        :param interceptor:
+        :param after: 指定添加到哪个拦截器之后
+        """
+        if isinstance(cls.interceptor, CombinedInterceptor):
+            itcps = list(cls.interceptor.flat())
+            for i, itcp in enumerate(itcps):
+                if itcp is after:
+                    cls.interceptor = CombinedInterceptor.from_iterable([
+                        *itcps[:i + 1], interceptor, *itcps[i + 1:]
+                    ])
+                    break
+            else:
+                raise ValueError("the interceptor specified by \'after\' argument was not found")
+        elif cls.interceptor is after:
+            cls.interceptor = CombinedInterceptor(cls.interceptor, interceptor)
+        else:
+            raise ValueError("the interceptor specified by \'after\' argument was not found")
+
+        _log_interceptors(cls)
+
+    @classmethod
+    def add_interceptor(cls, interceptor: Interceptor, front: bool = False):
+        """
+        添加一个拦截器
+
+        :param interceptor:
+        :param front: 添加到最前
+        """
+        if front:
+            cls.interceptor = CombinedInterceptor(interceptor, cls.interceptor)
+        else:
+            cls.interceptor = CombinedInterceptor(cls.interceptor, interceptor)
+        _log_interceptors(cls)
+
+    async def is_r18_allowed(self) -> bool:
+        return await r18_service.check_by_subject(*extract_subjects_from_session(self.session),
+                                                  acquire_rate_limit_token=False)
+
+    async def is_r18g_allowed(self) -> bool:
+        return await r18g_service.check_by_subject(*extract_subjects_from_session(self.session),
+                                                   acquire_rate_limit_token=False)
+
+    async def post_plain_text(self, message: str):
+        await context.require(Postman).post_plain_text(message, self.session, self.event)
+
+    async def post_illust(self, illust: Illust, *,
+                          header: Optional[str] = None,
+                          number: Optional[int] = None):
+        model = await IllustMessagesModel.from_illust(illust, header=header, number=number,
+                                                      max_page=conf.pixiv_max_item_per_query,
+                                                      block_r18=(not await self.is_r18_allowed()),
+                                                      block_r18g=(not await self.is_r18g_allowed()))
+        if model:
+            await context.require(Postman).post_illusts(model, self.session, self.event)
+
+    async def post_illusts(self, illusts: Sequence[Illust], *,
+                           header: Optional[str] = None,
+                           number: Optional[int] = None):
+        if len(illusts) == 1:
+            await self.post_illust(illusts[0], header=header, number=number)
+        else:
+            model = await IllustMessagesModel.from_illusts(illusts, header=header, number=number,
+                                                           block_r18=(not await self.is_r18_allowed()),
+                                                           block_r18g=(not await self.is_r18g_allowed()))
+            if model:
+                await context.require(Postman).post_illusts(model, self.session, self.event)
+
+
+class EntryHandler(Handler, ABC, interceptors=[context.require(DefaultErrorInterceptor)]):
+    pass
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/common/__init__.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/__init__.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from .illust import IllustHandler
-from .more import MoreHandler
-from .random_bookmark import RandomBookmarkHandler
-from .random_illust import RandomIllustHandler
-from .random_recommended_illust import RandomRecommendedIllustHandler
-from .random_related_illust import RandomRelatedIllustHandler
-from .random_user_illust import RandomUserIllustHandler
-from .ranking import RankingHandler
-
-__all__ = ("RandomBookmarkHandler", "RandomRecommendedIllustHandler",
-           "RankingHandler", "RandomIllustHandler",
-           "RandomUserIllustHandler", "IllustHandler",
-           "MoreHandler", "RandomRelatedIllustHandler")
+from .illust import IllustHandler
+from .more import MoreHandler
+from .random_bookmark import RandomBookmarkHandler
+from .random_illust import RandomIllustHandler
+from .random_recommended_illust import RandomRecommendedIllustHandler
+from .random_related_illust import RandomRelatedIllustHandler
+from .random_user_illust import RandomUserIllustHandler
+from .ranking import RankingHandler
+
+__all__ = ("RandomBookmarkHandler", "RandomRecommendedIllustHandler",
+           "RankingHandler", "RandomIllustHandler",
+           "RandomUserIllustHandler", "IllustHandler",
+           "MoreHandler", "RandomRelatedIllustHandler")
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/common/base.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/base.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from abc import ABC
-
-from ..base import EntryHandler
-from ..interceptor.loading_prompt_interceptor import LoadingPromptInterceptor
-from ..interceptor.record_req_interceptor import RecordReqInterceptor
-from ..interceptor.retry_interceptor import RetryInterceptor
-from ..interceptor.timeout_interceptor import TimeoutInterceptor
-from ..pkg_context import context
-
-
-class CommonHandler(EntryHandler, ABC, interceptors=[
-    context.require(TimeoutInterceptor),
-    context.require(LoadingPromptInterceptor),
-    context.require(RetryInterceptor)
-]):
-    pass
-
-
-class RecordCommonHandler(CommonHandler, ABC, interceptors=[context.require(RecordReqInterceptor)]):
-    pass
+from abc import ABC
+
+from ..base import EntryHandler
+from ..interceptor.loading_prompt_interceptor import LoadingPromptInterceptor
+from ..interceptor.record_req_interceptor import RecordReqInterceptor
+from ..interceptor.retry_interceptor import RetryInterceptor
+from ..interceptor.timeout_interceptor import TimeoutInterceptor
+from ..pkg_context import context
+
+
+class CommonHandler(EntryHandler, ABC, interceptors=[
+    context.require(TimeoutInterceptor),
+    context.require(LoadingPromptInterceptor),
+    context.require(RetryInterceptor)
+]):
+    pass
+
+
+class RecordCommonHandler(CommonHandler, ABC, interceptors=[context.require(RecordReqInterceptor)]):
+    pass
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/common/illust.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/illust.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from typing import Sequence
-
-from nonebot import on_regex
-from nonebot.internal.adapter import Event
-from nonebot.internal.params import Depends
-from nonebot.params import RegexGroup
-from nonebot_plugin_session import extract_session
-
-from .base import CommonHandler
-from ..pkg_context import context
-from ..utils import get_common_query_rule
-from ...config import Config
-from ...plugin_service import illust_service
-from ...service.pixiv_service import PixivService
-from ...utils.errors import BadRequestError
-
-conf = context.require(Config)
-service = context.require(PixivService)
-
-
-class IllustHandler(CommonHandler, service=illust_service):
-    @classmethod
-    def type(cls) -> str:
-        return "illust"
-
-    @classmethod
-    def enabled(cls) -> bool:
-        return conf.pixiv_illust_query_enabled
-
-    async def parse_args(self, args: Sequence[str]) -> dict:
-        try:
-            return {"illust_id": int(args[0])}
-        except ValueError:
-            raise BadRequestError(f"{args[0]}不是合法的插画ID")
-
-    # noinspection PyMethodOverriding
-    async def actual_handle(self, illust_id: int):
-        illust = await service.illust_detail(illust_id)
-        await self.post_illust(illust)
-
-
-@on_regex(r"^看看图\s*([1-9][0-9]*)$", rule=get_common_query_rule(), priority=5).handle()
-async def _(event: Event,
-            session=Depends(extract_session),
-            matched_groups=RegexGroup()):
-    illust_id = matched_groups[0]
-    await IllustHandler(session, event).handle(illust_id)
+from typing import Sequence
+
+from nonebot import on_regex
+from nonebot.internal.adapter import Event
+from nonebot.internal.params import Depends
+from nonebot.params import RegexGroup
+from nonebot_plugin_session import extract_session
+
+from .base import CommonHandler
+from ..pkg_context import context
+from ..utils import get_common_query_rule
+from ...config import Config
+from ...plugin_service import illust_service
+from ...service.pixiv_service import PixivService
+from ...utils.errors import BadRequestError
+
+conf = context.require(Config)
+service = context.require(PixivService)
+
+
+class IllustHandler(CommonHandler, service=illust_service):
+    @classmethod
+    def type(cls) -> str:
+        return "illust"
+
+    @classmethod
+    def enabled(cls) -> bool:
+        return conf.pixiv_illust_query_enabled
+
+    async def parse_args(self, args: Sequence[str]) -> dict:
+        try:
+            return {"illust_id": int(args[0])}
+        except ValueError:
+            raise BadRequestError(f"{args[0]}不是合法的插画ID")
+
+    # noinspection PyMethodOverriding
+    async def actual_handle(self, illust_id: int):
+        illust = await service.illust_detail(illust_id)
+        await self.post_illust(illust)
+
+
+@on_regex(r"^看看图\s*([1-9][0-9]*)$", rule=get_common_query_rule(), priority=5).handle()
+async def _(event: Event,
+            session=Depends(extract_session),
+            matched_groups=RegexGroup()):
+    illust_id = matched_groups[0]
+    await IllustHandler(session, event).handle(illust_id)
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/common/more.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/random_illust.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,49 @@
-from nonebot import on_regex
-from nonebot.internal.adapter import Event
-from nonebot.internal.params import Depends
-from nonebot_plugin_session import extract_session
-
-from .base import CommonHandler
-from ..pkg_context import context
-from ..recorder import Recorder
-from ..utils import get_common_query_rule, ArgCount
-from ...config import Config
-from ...plugin_service import more_service
-from ...utils.errors import BadRequestError
-
-recorder = context.require(Recorder)
-conf = context.require(Config)
-
-
-class MoreHandler(CommonHandler, service=more_service):
-    @classmethod
-    def type(cls) -> str:
-        return "more"
-
-    @classmethod
-    def enabled(cls) -> bool:
-        return conf.pixiv_more_enabled
-
-    async def actual_handle(self, count: int = 1):
-        req = recorder.get_req(self.session)
-        if not req:
-            raise BadRequestError("你还没有发送过请求")
-
-        handler = req.handler_type(self.session, silently=self.silently, disable_interceptors=True)
-        await handler.handle(*req.args, **{**req.kwargs, "count": count})
-
-
-@on_regex("^还要((.*)张)?$", rule=get_common_query_rule(), priority=1, block=True).handle()
-async def _(event: Event,
-            session=Depends(extract_session),
-            count=ArgCount(1)):
-    await MoreHandler(session, event).handle(count=count)
+from typing import Sequence
+
+from nonebot import on_regex
+from nonebot.internal.adapter import Event
+from nonebot.internal.params import Depends
+from nonebot.params import RegexGroup
+from nonebot_plugin_session import extract_session
+
+from .base import RecordCommonHandler
+from ..pkg_context import context
+from ..utils import get_common_query_rule, ArgCount
+from ...config import Config
+from ...plugin_service import random_illust_service
+from ...service.pixiv_service import PixivService
+
+conf = context.require(Config)
+service = context.require(PixivService)
+
+
+class RandomIllustHandler(RecordCommonHandler, service=random_illust_service):
+    @classmethod
+    def type(cls) -> str:
+        return "random_illust"
+
+    @classmethod
+    def enabled(cls) -> bool:
+        return conf.pixiv_random_illust_query_enabled
+
+    async def parse_args(self, args: Sequence[str]) -> dict:
+        return {"word": args[0]}
+
+    # noinspection PyMethodOverriding
+    async def actual_handle(self, *, word: str,
+                            count: int = 1):
+        illusts = await service.random_illust(word, count=count,
+                                              exclude_r18=(not await self.is_r18_allowed()),
+                                              exclude_r18g=(not await self.is_r18g_allowed()))
+
+        await self.post_illusts(illusts,
+                                header=f"这是您点的{word}图")
+
+
+@on_regex("^来(.*)?张(.+)图$", rule=get_common_query_rule(), priority=5).handle()
+async def _(event: Event,
+            matched_groups=RegexGroup(),
+            session=Depends(extract_session),
+            count=ArgCount()):
+    word = matched_groups[1]
+    await RandomIllustHandler(session, event).handle(word, count=count)
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/common/random_bookmark.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/random_bookmark.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-from typing import Sequence
-
-from nonebot import on_regex
-from nonebot.internal.adapter import Event
-from nonebot.internal.params import Depends
-from nonebot_plugin_session import extract_session
-
-from .base import RecordCommonHandler
-from ..pkg_context import context
-from ..utils import get_common_query_rule, ArgCount
-from ...config import Config
-from ...plugin_service import random_bookmark_service
-from ...service.pixiv_account_binder import PixivAccountBinder
-from ...service.pixiv_service import PixivService
-from ...utils.errors import BadRequestError
-
-conf = context.require(Config)
-binder = context.require(PixivAccountBinder)
-service = context.require(PixivService)
-
-
-class RandomBookmarkHandler(RecordCommonHandler, service=random_bookmark_service):
-    @classmethod
-    def type(cls) -> str:
-        return "random_bookmark"
-
-    @classmethod
-    def enabled(cls) -> bool:
-        return conf.pixiv_random_bookmark_query_enabled
-
-    async def parse_args(self, args: Sequence[str]) -> dict:
-        pixiv_user_id = 0
-
-        if len(args) > 0:
-            try:
-                pixiv_user_id = int(args[0])
-            except ValueError:
-                raise BadRequestError(f"{args[0]}不是合法的ID")
-
-        return {"pixiv_user_id": pixiv_user_id, "sender_user_id": self.session.id1}
-
-    # noinspection PyMethodOverriding
-    async def actual_handle(self, *, pixiv_user_id: int = 0,
-                            sender_user_id: int = 0,
-                            count: int = 1):
-        if not pixiv_user_id and sender_user_id:
-            pixiv_user_id = await binder.get_binding(self.session.platform, sender_user_id)
-
-        if not pixiv_user_id:
-            pixiv_user_id = conf.pixiv_random_bookmark_user_id
-
-        if not pixiv_user_id:
-            raise BadRequestError("无效的Pixiv账号，或未绑定Pixiv账号")
-
-        illusts = await service.random_bookmark(pixiv_user_id, count=count,
-                                                exclude_r18=(not await self.is_r18_allowed()),
-                                                exclude_r18g=(not await self.is_r18g_allowed()))
-
-        await self.post_illusts(illusts,
-                                header="这是您点的私家车")
-
-
-@on_regex("^来(.*)?张私家车$", rule=get_common_query_rule(), priority=5).handle()
-async def _(event: Event,
-            session=Depends(extract_session),
-            count=ArgCount()):
-    await RandomBookmarkHandler(session, event).handle(count=count)
+from typing import Sequence
+
+from nonebot import on_regex
+from nonebot.internal.adapter import Event
+from nonebot.internal.params import Depends
+from nonebot_plugin_session import extract_session
+
+from .base import RecordCommonHandler
+from ..pkg_context import context
+from ..utils import get_common_query_rule, ArgCount
+from ...config import Config
+from ...plugin_service import random_bookmark_service
+from ...service.pixiv_account_binder import PixivAccountBinder
+from ...service.pixiv_service import PixivService
+from ...utils.errors import BadRequestError
+
+conf = context.require(Config)
+binder = context.require(PixivAccountBinder)
+service = context.require(PixivService)
+
+
+class RandomBookmarkHandler(RecordCommonHandler, service=random_bookmark_service):
+    @classmethod
+    def type(cls) -> str:
+        return "random_bookmark"
+
+    @classmethod
+    def enabled(cls) -> bool:
+        return conf.pixiv_random_bookmark_query_enabled
+
+    async def parse_args(self, args: Sequence[str]) -> dict:
+        pixiv_user_id = 0
+
+        if len(args) > 0:
+            try:
+                pixiv_user_id = int(args[0])
+            except ValueError:
+                raise BadRequestError(f"{args[0]}不是合法的ID")
+
+        return {"pixiv_user_id": pixiv_user_id, "sender_user_id": self.session.id1}
+
+    # noinspection PyMethodOverriding
+    async def actual_handle(self, *, pixiv_user_id: int = 0,
+                            sender_user_id: int = 0,
+                            count: int = 1):
+        if not pixiv_user_id and sender_user_id:
+            pixiv_user_id = await binder.get_binding(self.session.platform, sender_user_id)
+
+        if not pixiv_user_id:
+            pixiv_user_id = conf.pixiv_random_bookmark_user_id
+
+        if not pixiv_user_id:
+            raise BadRequestError("无效的Pixiv账号，或未绑定Pixiv账号")
+
+        illusts = await service.random_bookmark(pixiv_user_id, count=count,
+                                                exclude_r18=(not await self.is_r18_allowed()),
+                                                exclude_r18g=(not await self.is_r18g_allowed()))
+
+        await self.post_illusts(illusts,
+                                header="这是您点的私家车")
+
+
+@on_regex("^来(.*)?张私家车$", rule=get_common_query_rule(), priority=5).handle()
+async def _(event: Event,
+            session=Depends(extract_session),
+            count=ArgCount()):
+    await RandomBookmarkHandler(session, event).handle(count=count)
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/common/random_illust.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/random_related_illust.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,51 @@
-from typing import Sequence
-
-from nonebot import on_regex
-from nonebot.internal.adapter import Event
-from nonebot.internal.params import Depends
-from nonebot.params import RegexGroup
-from nonebot_plugin_session import extract_session
-
-from .base import RecordCommonHandler
-from ..pkg_context import context
-from ..utils import get_common_query_rule, ArgCount
-from ...config import Config
-from ...plugin_service import random_illust_service
-from ...service.pixiv_service import PixivService
-
-conf = context.require(Config)
-service = context.require(PixivService)
-
-
-class RandomIllustHandler(RecordCommonHandler, service=random_illust_service):
-    @classmethod
-    def type(cls) -> str:
-        return "random_illust"
-
-    @classmethod
-    def enabled(cls) -> bool:
-        return conf.pixiv_random_illust_query_enabled
-
-    async def parse_args(self, args: Sequence[str]) -> dict:
-        return {"word": args[0]}
-
-    # noinspection PyMethodOverriding
-    async def actual_handle(self, *, word: str,
-                            count: int = 1):
-        illusts = await service.random_illust(word, count=count,
-                                              exclude_r18=(not await self.is_r18_allowed()),
-                                              exclude_r18g=(not await self.is_r18g_allowed()))
-
-        await self.post_illusts(illusts,
-                                header=f"这是您点的{word}图")
-
-
-@on_regex("^来(.*)?张(.+)图$", rule=get_common_query_rule(), priority=5).handle()
-async def _(event: Event,
-            matched_groups=RegexGroup(),
-            session=Depends(extract_session),
-            count=ArgCount()):
-    word = matched_groups[1]
-    await RandomIllustHandler(session, event).handle(word, count=count)
+from typing import Sequence
+
+from nonebot import on_regex
+from nonebot.internal.adapter import Event
+from nonebot.internal.params import Depends
+from nonebot_plugin_session import extract_session
+
+from .base import RecordCommonHandler
+from ..pkg_context import context
+from ..recorder import Recorder
+from ..utils import get_common_query_rule
+from ...config import Config
+from ...plugin_service import random_related_illust_service
+from ...service.pixiv_service import PixivService
+from ...utils.errors import BadRequestError
+
+conf = context.require(Config)
+service = context.require(PixivService)
+recorder = context.require(Recorder)
+
+
+class RandomRelatedIllustHandler(RecordCommonHandler, service=random_related_illust_service):
+    @classmethod
+    def type(cls) -> str:
+        return "random_related_illust"
+
+    @classmethod
+    def enabled(cls) -> bool:
+        return conf.pixiv_random_related_illust_query_enabled
+
+    async def parse_args(self, args: Sequence[str]) -> dict:
+        illust_id = recorder.get_resp(self.session)
+        if not illust_id:
+            raise BadRequestError("你还没有发送过请求")
+        return {"illust_id": illust_id}
+
+    # noinspection PyMethodOverriding
+    async def actual_handle(self, *, illust_id: int,
+                            count: int = 1):
+        illusts = await service.random_related_illust(illust_id, count=count,
+                                                      exclude_r18=(not await self.is_r18_allowed()),
+                                                      exclude_r18g=(not await self.is_r18g_allowed()))
+
+        await self.post_illusts(illusts,
+                                header=f"这是您点的[{illust_id}]的相关图片")
+
+
+@on_regex("^不够色$", rule=get_common_query_rule(), priority=1, block=True).handle()
+async def _(event: Event,
+            session=Depends(extract_session)):
+    await RandomRelatedIllustHandler(session, event).handle()
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/common/random_recommended_illust.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/random_recommended_illust.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from nonebot import on_regex
-from nonebot.internal.adapter import Event
-from nonebot.internal.params import Depends
-from nonebot_plugin_session import extract_session
-
-from .base import RecordCommonHandler
-from ..pkg_context import context
-from ..utils import get_common_query_rule, ArgCount
-from ...config import Config
-from ...plugin_service import random_recommended_illust_service
-from ...service.pixiv_service import PixivService
-
-conf = context.require(Config)
-service = context.require(PixivService)
-
-
-class RandomRecommendedIllustHandler(RecordCommonHandler, service=random_recommended_illust_service):
-    @classmethod
-    def type(cls) -> str:
-        return "random_recommended_illust"
-
-    @classmethod
-    def enabled(cls) -> bool:
-        return conf.pixiv_random_recommended_illust_query_enabled
-
-    async def actual_handle(self, *, count: int = 1):
-        illusts = await service.random_recommended_illust(count=count,
-                                                          exclude_r18=(not await self.is_r18_allowed()),
-                                                          exclude_r18g=(not await self.is_r18g_allowed()))
-
-        await self.post_illusts(illusts,
-                                header="这是您点的图")
-
-
-@on_regex("^来(.*)?张图$", rule=get_common_query_rule(), priority=3, block=True).handle()
-async def _(event: Event,
-            session=Depends(extract_session),
-            count=ArgCount()):
-    await RandomRecommendedIllustHandler(session, event).handle(count=count)
+from nonebot import on_regex
+from nonebot.internal.adapter import Event
+from nonebot.internal.params import Depends
+from nonebot_plugin_session import extract_session
+
+from .base import RecordCommonHandler
+from ..pkg_context import context
+from ..utils import get_common_query_rule, ArgCount
+from ...config import Config
+from ...plugin_service import random_recommended_illust_service
+from ...service.pixiv_service import PixivService
+
+conf = context.require(Config)
+service = context.require(PixivService)
+
+
+class RandomRecommendedIllustHandler(RecordCommonHandler, service=random_recommended_illust_service):
+    @classmethod
+    def type(cls) -> str:
+        return "random_recommended_illust"
+
+    @classmethod
+    def enabled(cls) -> bool:
+        return conf.pixiv_random_recommended_illust_query_enabled
+
+    async def actual_handle(self, *, count: int = 1):
+        illusts = await service.random_recommended_illust(count=count,
+                                                          exclude_r18=(not await self.is_r18_allowed()),
+                                                          exclude_r18g=(not await self.is_r18g_allowed()))
+
+        await self.post_illusts(illusts,
+                                header="这是您点的图")
+
+
+@on_regex("^来(.*)?张图$", rule=get_common_query_rule(), priority=3, block=True).handle()
+async def _(event: Event,
+            session=Depends(extract_session),
+            count=ArgCount()):
+    await RandomRecommendedIllustHandler(session, event).handle(count=count)
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/common/random_user_illust.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/random_user_illust.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-from typing import Sequence
-from typing import Union
-
-from nonebot import on_regex
-from nonebot.internal.adapter import Event
-from nonebot.internal.params import Depends
-from nonebot.params import RegexGroup
-from nonebot_plugin_session import extract_session
-
-from nonebot_plugin_pixivbot.plugin_service import random_user_illust_service
-from .base import RecordCommonHandler
-from ..pkg_context import context
-from ..utils import get_common_query_rule, ArgCount
-from ...config import Config
-from ...service.pixiv_service import PixivService
-
-conf = context.require(Config)
-service = context.require(PixivService)
-
-
-class RandomUserIllustHandler(RecordCommonHandler, service=random_user_illust_service):
-    @classmethod
-    def type(cls) -> str:
-        return "random_user_illust"
-
-    @classmethod
-    def enabled(cls) -> bool:
-        return conf.pixiv_random_user_illust_query_enabled
-
-    async def parse_args(self, args: Sequence[str]) -> dict:
-        try:
-            user_id = int(args[0])
-            return {"user": user_id}
-        except ValueError:
-            user = await service.get_user(args[0])
-            return {"user": user.id}
-
-    # noinspection PyMethodOverriding
-    async def actual_handle(self, *, user: Union[str, int],
-                            count: int = 1):
-        userinfo, illusts = await service.random_user_illust(user, count=count,
-                                                             exclude_r18=(not await self.is_r18_allowed()),
-                                                             exclude_r18g=(not await self.is_r18g_allowed()))
-
-        await self.post_illusts(illusts,
-                                header=f"这是您点的{userinfo.name}({userinfo.id})老师的图")
-
-
-@on_regex("^来(.*)?张(.+)老师的图$", rule=get_common_query_rule(), priority=4, block=True).handle()
-async def _(event: Event,
-            matched_groups=RegexGroup(),
-            session=Depends(extract_session),
-            count=ArgCount()):
-    user = matched_groups[1]
-    await RandomUserIllustHandler(session, event).handle(user, count=count)
+from typing import Sequence
+from typing import Union
+
+from nonebot import on_regex
+from nonebot.internal.adapter import Event
+from nonebot.internal.params import Depends
+from nonebot.params import RegexGroup
+from nonebot_plugin_session import extract_session
+
+from nonebot_plugin_pixivbot.plugin_service import random_user_illust_service
+from .base import RecordCommonHandler
+from ..pkg_context import context
+from ..utils import get_common_query_rule, ArgCount
+from ...config import Config
+from ...service.pixiv_service import PixivService
+
+conf = context.require(Config)
+service = context.require(PixivService)
+
+
+class RandomUserIllustHandler(RecordCommonHandler, service=random_user_illust_service):
+    @classmethod
+    def type(cls) -> str:
+        return "random_user_illust"
+
+    @classmethod
+    def enabled(cls) -> bool:
+        return conf.pixiv_random_user_illust_query_enabled
+
+    async def parse_args(self, args: Sequence[str]) -> dict:
+        try:
+            user_id = int(args[0])
+            return {"user": user_id}
+        except ValueError:
+            user = await service.get_user(args[0])
+            return {"user": user.id}
+
+    # noinspection PyMethodOverriding
+    async def actual_handle(self, *, user: Union[str, int],
+                            count: int = 1):
+        userinfo, illusts = await service.random_user_illust(user, count=count,
+                                                             exclude_r18=(not await self.is_r18_allowed()),
+                                                             exclude_r18g=(not await self.is_r18g_allowed()))
+
+        await self.post_illusts(illusts,
+                                header=f"这是您点的{userinfo.name}({userinfo.id})老师的图")
+
+
+@on_regex("^来(.*)?张(.+)老师的图$", rule=get_common_query_rule(), priority=4, block=True).handle()
+async def _(event: Event,
+            matched_groups=RegexGroup(),
+            session=Depends(extract_session),
+            count=ArgCount()):
+    user = matched_groups[1]
+    await RandomUserIllustHandler(session, event).handle(user, count=count)
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/common/ranking.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/common/ranking.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-from typing import Sequence
-from typing import Tuple
-from typing import Union
-
-from nonebot import on_regex
-from nonebot.internal.adapter import Event
-from nonebot.internal.params import Depends
-from nonebot.params import RegexGroup
-from nonebot_plugin_session import extract_session
-
-from .base import CommonHandler
-from ..pkg_context import context
-from ..utils import get_common_query_rule
-from ...config import Config
-from ...enums import RankingMode
-from ...plugin_service import ranking_service
-from ...service.pixiv_service import PixivService
-from ...utils.decode_integer import decode_integer
-from ...utils.errors import BadRequestError
-
-conf = context.require(Config)
-service = context.require(PixivService)
-
-
-class RankingHandler(CommonHandler, service=ranking_service):
-    @classmethod
-    def type(cls) -> str:
-        return "ranking"
-
-    mode_mapping = {RankingMode.day: "日", RankingMode.week: "周", RankingMode.month: "月",
-                    RankingMode.day_male: "男性", RankingMode.day_female: "女性", RankingMode.week_original: "原创",
-                    RankingMode.week_rookie: "新人", RankingMode.day_manga: "漫画", RankingMode.day_ai: 'ai'}
-
-    mode_rev_mapping = {}
-    for mode, text in mode_mapping.items():
-        mode_rev_mapping[text] = mode
-
-    @classmethod
-    def enabled(cls) -> bool:
-        return conf.pixiv_ranking_query_enabled
-
-    def validate_range(self, range: Tuple[int, int] = None):
-        if range:
-            start, end = range
-            if end - start + 1 > conf.pixiv_ranking_max_item_per_query:
-                raise BadRequestError(
-                    f"仅支持一次查询{conf.pixiv_ranking_max_item_per_query}张以下插画")
-            elif start > end:
-                raise BadRequestError("范围不合法")
-            elif end > conf.pixiv_ranking_fetch_item:
-                raise BadRequestError(
-                    f'仅支持查询{conf.pixiv_ranking_fetch_item}名以内的插画')
-
-    async def parse_args(self, args: Sequence[str]) -> dict:
-        mode = args[0].lower() if len(args) > 0 else None
-        range = args[1] if len(args) > 1 else None
-
-        if not mode:  # 判断是不是空字符串
-            mode = None
-        elif mode in self.mode_rev_mapping:
-            mode = self.mode_rev_mapping[mode]
-        elif isinstance(mode, str):
-            try:
-                mode = RankingMode[mode]
-            except:
-                raise BadRequestError(f"{mode}不是合法的榜单类型")
-
-        if not range:
-            range = None
-        else:
-            try:
-                if "-" in range:
-                    start, end = range.split("-")
-                    range = int(start), int(end)
-                else:
-                    range = decode_integer(range)
-                    range = range, range
-            except ValueError:
-                raise BadRequestError(f"{range}不是合法的范围")
-
-        return {"mode": mode, "range": range}
-
-    async def actual_handle(self, *, mode: Union[RankingMode, None] = None,
-                            range: Union[Tuple[int, int], int, None] = None):
-        if mode is None:
-            mode = conf.pixiv_ranking_default_mode
-
-        if range is None:
-            range = conf.pixiv_ranking_default_range
-
-        if isinstance(range, int):
-            range = range, range
-
-        self.validate_range(range)
-        illusts = await service.illust_ranking(mode, range)
-        await self.post_illusts(illusts,
-                                header=f"这是您点的{self.mode_mapping[mode]}榜",
-                                number=range[0])
-
-
-@on_regex(r"^看看(.*)?榜\s*(.*)?$", rule=get_common_query_rule(), priority=4, block=True).handle()
-async def on_match(event: Event,
-                   matched_groups=RegexGroup(),
-                   session=Depends(extract_session)):
-    if matched_groups:
-        mode = matched_groups[0]
-        num = matched_groups[1]
-    else:
-        mode = None
-        num = None
-    await RankingHandler(session, event).handle(mode, num)
+from typing import Sequence
+from typing import Tuple
+from typing import Union
+
+from nonebot import on_regex
+from nonebot.internal.adapter import Event
+from nonebot.internal.params import Depends
+from nonebot.params import RegexGroup
+from nonebot_plugin_session import extract_session
+
+from .base import CommonHandler
+from ..pkg_context import context
+from ..utils import get_common_query_rule
+from ...config import Config
+from ...enums import RankingMode
+from ...plugin_service import ranking_service
+from ...service.pixiv_service import PixivService
+from ...utils.decode_integer import decode_integer
+from ...utils.errors import BadRequestError
+
+conf = context.require(Config)
+service = context.require(PixivService)
+
+
+class RankingHandler(CommonHandler, service=ranking_service):
+    @classmethod
+    def type(cls) -> str:
+        return "ranking"
+
+    mode_mapping = {RankingMode.day: "日", RankingMode.week: "周", RankingMode.month: "月",
+                    RankingMode.day_male: "男性", RankingMode.day_female: "女性", RankingMode.week_original: "原创",
+                    RankingMode.week_rookie: "新人", RankingMode.day_manga: "漫画", RankingMode.day_ai: 'ai'}
+
+    mode_rev_mapping = {}
+    for mode, text in mode_mapping.items():
+        mode_rev_mapping[text] = mode
+
+    @classmethod
+    def enabled(cls) -> bool:
+        return conf.pixiv_ranking_query_enabled
+
+    def validate_range(self, range: Tuple[int, int] = None):
+        if range:
+            start, end = range
+            if end - start + 1 > conf.pixiv_ranking_max_item_per_query:
+                raise BadRequestError(
+                    f"仅支持一次查询{conf.pixiv_ranking_max_item_per_query}张以下插画")
+            elif start > end:
+                raise BadRequestError("范围不合法")
+            elif end > conf.pixiv_ranking_fetch_item:
+                raise BadRequestError(
+                    f'仅支持查询{conf.pixiv_ranking_fetch_item}名以内的插画')
+
+    async def parse_args(self, args: Sequence[str]) -> dict:
+        mode = args[0].lower() if len(args) > 0 else None
+        range = args[1] if len(args) > 1 else None
+
+        if not mode:  # 判断是不是空字符串
+            mode = None
+        elif mode in self.mode_rev_mapping:
+            mode = self.mode_rev_mapping[mode]
+        elif isinstance(mode, str):
+            try:
+                mode = RankingMode[mode]
+            except:
+                raise BadRequestError(f"{mode}不是合法的榜单类型")
+
+        if not range:
+            range = None
+        else:
+            try:
+                if "-" in range:
+                    start, end = range.split("-")
+                    range = int(start), int(end)
+                else:
+                    range = decode_integer(range)
+                    range = range, range
+            except ValueError:
+                raise BadRequestError(f"{range}不是合法的范围")
+
+        return {"mode": mode, "range": range}
+
+    async def actual_handle(self, *, mode: Union[RankingMode, None] = None,
+                            range: Union[Tuple[int, int], int, None] = None):
+        if mode is None:
+            mode = conf.pixiv_ranking_default_mode
+
+        if range is None:
+            range = conf.pixiv_ranking_default_range
+
+        if isinstance(range, int):
+            range = range, range
+
+        self.validate_range(range)
+        illusts = await service.illust_ranking(mode, range)
+        await self.post_illusts(illusts,
+                                header=f"这是您点的{self.mode_mapping[mode]}榜",
+                                number=range[0])
+
+
+@on_regex(r"^看看(.*)?榜\s*(.*)?$", rule=get_common_query_rule(), priority=4, block=True).handle()
+async def on_match(event: Event,
+                   matched_groups=RegexGroup(),
+                   session=Depends(extract_session)):
+    if matched_groups:
+        mode = matched_groups[0]
+        num = matched_groups[1]
+    else:
+        mode = None
+        num = None
+    await RankingHandler(session, event).handle(mode, num)
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/interceptor/loading_prompt_interceptor.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/loading_prompt_interceptor.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from asyncio import create_task, sleep, shield, Task, CancelledError
-from typing import Callable, Optional, TYPE_CHECKING
-
-from nonebot import logger
-
-from .base import Interceptor
-from ..pkg_context import context
-from ...config import Config
-
-if TYPE_CHECKING:
-    from ..base import Handler
-
-conf = context.require(Config)
-
-
-@context.register_singleton()
-class LoadingPromptInterceptor(Interceptor):
-
-    async def send_delayed_loading_prompt(self, handler: "Handler"):
-        try:
-            await sleep(conf.pixiv_loading_prompt_delayed_time)
-
-            logger.debug(f"send delayed loading")
-            await shield(handler.post_plain_text("努力加载中"))
-        except CancelledError as e:
-            raise e
-        except BaseException as e:
-            logger.exception(e)
-
-    async def intercept(self, handler: "Handler", wrapped_func: Callable, *args, **kwargs):
-        task: Optional[Task] = None
-        if not handler.silently:
-            task = create_task(self.send_delayed_loading_prompt(handler))
-
-        try:
-            await wrapped_func(*args, **kwargs)
-        finally:
-            if task and not task.done():
-                task.cancel()
+from asyncio import create_task, sleep, shield, Task, CancelledError
+from typing import Callable, Optional, TYPE_CHECKING
+
+from nonebot import logger
+
+from .base import Interceptor
+from ..pkg_context import context
+from ...config import Config
+
+if TYPE_CHECKING:
+    from ..base import Handler
+
+conf = context.require(Config)
+
+
+@context.register_singleton()
+class LoadingPromptInterceptor(Interceptor):
+
+    async def send_delayed_loading_prompt(self, handler: "Handler"):
+        try:
+            await sleep(conf.pixiv_loading_prompt_delayed_time)
+
+            logger.debug(f"send delayed loading")
+            await shield(handler.post_plain_text("努力加载中"))
+        except CancelledError as e:
+            raise e
+        except BaseException as e:
+            logger.exception(e)
+
+    async def intercept(self, handler: "Handler", wrapped_func: Callable, *args, **kwargs):
+        task: Optional[Task] = None
+        if not handler.silently:
+            task = create_task(self.send_delayed_loading_prompt(handler))
+
+        try:
+            await wrapped_func(*args, **kwargs)
+        finally:
+            if task and not task.done():
+                task.cancel()
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/interceptor/permission_interceptor.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/permission_interceptor.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-from abc import ABC, abstractmethod
-from typing import Callable, Optional, TYPE_CHECKING
-
-from nonebot import logger
-from nonebot_plugin_access_control.subject import extract_subjects_from_session
-
-from .base import Interceptor
-from ..pkg_context import context
-
-if TYPE_CHECKING:
-    from ..base import Handler
-
-
-class PermissionInterceptor(Interceptor, ABC):
-    @abstractmethod
-    async def has_permission(self, handler: "Handler") -> bool:
-        raise NotImplementedError()
-
-    async def get_permission_denied_msg(self, handler: "Handler") -> Optional[str]:
-        return None
-
-    async def intercept(self, handler: "Handler", wrapped_func: Callable, *args, **kwargs):
-        p = await self.has_permission(handler)
-
-        if p:
-            await wrapped_func(*args, **kwargs)
-        else:
-            logger.debug(f"permission denied")
-            if not handler.silently:
-                msg = await self.get_permission_denied_msg(handler)
-                if msg:
-                    await handler.post_plain_text(msg)
-
-
-class AnyPermissionInterceptor(PermissionInterceptor):
-    def __init__(self, *interceptors: PermissionInterceptor):
-        super().__init__()
-        self.interceptors = list(interceptors)
-
-    def append(self, interceptor: PermissionInterceptor):
-        self.interceptors.append(interceptor)
-
-    async def has_permission(self, handler: "Handler") -> bool:
-        for inter in self.interceptors:
-            p = await inter.has_permission(handler)
-            if p:
-                return True
-
-        return False
-
-
-@context.register_singleton()
-class SuperuserInterceptor(PermissionInterceptor):
-    async def has_permission(self, handler: "Handler") -> bool:
-        sbj = extract_subjects_from_session(handler.session)
-        return "superuser" in sbj
+from abc import ABC, abstractmethod
+from typing import Callable, Optional, TYPE_CHECKING
+
+from nonebot import logger
+from nonebot_plugin_access_control.subject import extract_subjects_from_session
+
+from .base import Interceptor
+from ..pkg_context import context
+
+if TYPE_CHECKING:
+    from ..base import Handler
+
+
+class PermissionInterceptor(Interceptor, ABC):
+    @abstractmethod
+    async def has_permission(self, handler: "Handler") -> bool:
+        raise NotImplementedError()
+
+    async def get_permission_denied_msg(self, handler: "Handler") -> Optional[str]:
+        return None
+
+    async def intercept(self, handler: "Handler", wrapped_func: Callable, *args, **kwargs):
+        p = await self.has_permission(handler)
+
+        if p:
+            await wrapped_func(*args, **kwargs)
+        else:
+            logger.debug(f"permission denied")
+            if not handler.silently:
+                msg = await self.get_permission_denied_msg(handler)
+                if msg:
+                    await handler.post_plain_text(msg)
+
+
+class AnyPermissionInterceptor(PermissionInterceptor):
+    def __init__(self, *interceptors: PermissionInterceptor):
+        super().__init__()
+        self.interceptors = list(interceptors)
+
+    def append(self, interceptor: PermissionInterceptor):
+        self.interceptors.append(interceptor)
+
+    async def has_permission(self, handler: "Handler") -> bool:
+        for inter in self.interceptors:
+            p = await inter.has_permission(handler)
+            if p:
+                return True
+
+        return False
+
+
+@context.register_singleton()
+class SuperuserInterceptor(PermissionInterceptor):
+    async def has_permission(self, handler: "Handler") -> bool:
+        sbj = extract_subjects_from_session(handler.session)
+        return "superuser" in sbj
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/interceptor/record_req_interceptor.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/record_req_interceptor.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Callable, TYPE_CHECKING
-
-from .base import Interceptor
-from ..pkg_context import context
-from ..recorder import Recorder, Req
-
-if TYPE_CHECKING:
-    from ..base import Handler
-
-recorder = context.require(Recorder)
-
-
-@context.register_singleton()
-class RecordReqInterceptor(Interceptor):
-    async def intercept(self, handler: "Handler", wrapped_func: Callable, *args, **kwargs):
-        await wrapped_func(*args, **kwargs)
-        recorder.record_req(Req(type(handler), args, kwargs), handler.session)
+from typing import Callable, TYPE_CHECKING
+
+from .base import Interceptor
+from ..pkg_context import context
+from ..recorder import Recorder, Req
+
+if TYPE_CHECKING:
+    from ..base import Handler
+
+recorder = context.require(Recorder)
+
+
+@context.register_singleton()
+class RecordReqInterceptor(Interceptor):
+    async def intercept(self, handler: "Handler", wrapped_func: Callable, *args, **kwargs):
+        await wrapped_func(*args, **kwargs)
+        recorder.record_req(Req(type(handler), args, kwargs), handler.session)
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/interceptor/retry_interceptor.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/interceptor/retry_interceptor.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-import asyncio
-from typing import Callable, TYPE_CHECKING
-
-from aiohttp import ServerConnectionError
-from nonebot import logger
-
-from .base import Interceptor
-from ...global_context import context
-
-if TYPE_CHECKING:
-    from ..base import Handler
-
-exception = (asyncio.TimeoutError, ServerConnectionError, ConnectionError)
-
-
-@context.register_singleton()
-class RetryInterceptor(Interceptor):
-    async def intercept(self, handler: "Handler", wrapped_func: Callable, *args, **kwargs):
-        err = None
-
-        for i in range(10):
-            try:
-                return await wrapped_func(*args, **kwargs)
-            except exception as e:
-                logger.opt(exception=e).error(f"Network error occurred while handling, retrying... {i + 1}/10")
-                err = e
-            except Exception as e:
-                raise e
-
-        raise err
+import asyncio
+from typing import Callable, TYPE_CHECKING
+
+from aiohttp import ServerConnectionError
+from nonebot import logger
+
+from .base import Interceptor
+from ...global_context import context
+
+if TYPE_CHECKING:
+    from ..base import Handler
+
+exception = (asyncio.TimeoutError, ServerConnectionError, ConnectionError)
+
+
+@context.register_singleton()
+class RetryInterceptor(Interceptor):
+    async def intercept(self, handler: "Handler", wrapped_func: Callable, *args, **kwargs):
+        err = None
+
+        for i in range(10):
+            try:
+                return await wrapped_func(*args, **kwargs)
+            except exception as e:
+                logger.opt(exception=e).error(f"Network error occurred while handling, retrying... {i + 1}/10")
+                err = e
+            except Exception as e:
+                raise e
+
+        raise err
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/utils.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/utils.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from nonebot.internal.params import Depends
-from nonebot.params import RegexGroup
-from nonebot.rule import to_me
-
-from nonebot_plugin_pixivbot.config import Config
-from nonebot_plugin_pixivbot.global_context import context
-from nonebot_plugin_pixivbot.utils.decode_integer import decode_integer
-from nonebot_plugin_pixivbot.utils.errors import BadRequestError
-
-
-def ArgCount(pos: int = 0):
-    def dep(matched_groups=RegexGroup()):
-        count = 1
-        if matched_groups:
-            raw_count = matched_groups[pos]
-            if raw_count:
-                try:
-                    count = decode_integer(raw_count)
-                except ValueError:
-                    raise BadRequestError(f"{raw_count}不是合法的数字")
-        return count
-
-    return Depends(dep)
-
-
-def get_common_query_rule():
-    if context.require(Config).pixiv_query_to_me_only:
-        rule = to_me()
-    else:
-        rule = None
-    return rule
-
-
-def get_command_rule():
-    if context.require(Config).pixiv_command_to_me_only:
-        rule = to_me()
-    else:
-        rule = None
-    return rule
-
-
-__all__ = ("get_count", "get_common_query_rule", "get_command_rule", "get_post_dest")
+from nonebot.internal.params import Depends
+from nonebot.params import RegexGroup
+from nonebot.rule import to_me
+
+from nonebot_plugin_pixivbot.config import Config
+from nonebot_plugin_pixivbot.global_context import context
+from nonebot_plugin_pixivbot.utils.decode_integer import decode_integer
+from nonebot_plugin_pixivbot.utils.errors import BadRequestError
+
+
+def ArgCount(pos: int = 0):
+    def dep(matched_groups=RegexGroup()):
+        count = 1
+        if matched_groups:
+            raw_count = matched_groups[pos]
+            if raw_count:
+                try:
+                    count = decode_integer(raw_count)
+                except ValueError:
+                    raise BadRequestError(f"{raw_count}不是合法的数字")
+        return count
+
+    return Depends(dep)
+
+
+def get_common_query_rule():
+    if context.require(Config).pixiv_query_to_me_only:
+        rule = to_me()
+    else:
+        rule = None
+    return rule
+
+
+def get_command_rule():
+    if context.require(Config).pixiv_command_to_me_only:
+        rule = to_me()
+    else:
+        rule = None
+    return rule
+
+
+__all__ = ("get_count", "get_common_query_rule", "get_command_rule", "get_post_dest")
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/watch/base.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/watch/base.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from abc import ABC
-
-from nonebot_plugin_pixivbot.service.pixiv_service import PixivService
-from ..base import EntryHandler
-from ..interceptor.retry_interceptor import RetryInterceptor
-from ..interceptor.timeout_interceptor import TimeoutInterceptor
-from ..pkg_context import context
-from ...plugin_service import receive_watch_service
-
-service = context.require(PixivService)
-
-
-class WatchTaskHandler(EntryHandler, ABC, service=receive_watch_service,
-                       service_interceptor_kwargs={"acquire_rate_limit_token": False},
-                       interceptors=[
-                           context.require(TimeoutInterceptor),
-                           context.require(RetryInterceptor)
-                       ]):
-    async def parse_args(self, args):
-        raise RuntimeError("Please call handle_with_parsed_args() instead! ")
+from abc import ABC
+
+from nonebot_plugin_pixivbot.service.pixiv_service import PixivService
+from ..base import EntryHandler
+from ..interceptor.retry_interceptor import RetryInterceptor
+from ..interceptor.timeout_interceptor import TimeoutInterceptor
+from ..pkg_context import context
+from ...plugin_service import receive_watch_service
+
+service = context.require(PixivService)
+
+
+class WatchTaskHandler(EntryHandler, ABC, service=receive_watch_service,
+                       service_interceptor_kwargs={"acquire_rate_limit_token": False},
+                       interceptors=[
+                           context.require(TimeoutInterceptor),
+                           context.require(RetryInterceptor)
+                       ]):
+    async def parse_args(self, args):
+        raise RuntimeError("Please call handle_with_parsed_args() instead! ")
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/watch/following_illusts.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/watch/following_illusts.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-import time
-
-from nonebot import logger
-
-from .base import WatchTaskHandler
-from ..pkg_context import context
-from ...config import Config
-from ...data.pixiv_repo import PixivRepo
-from ...data.pixiv_repo.enums import CacheStrategy
-from ...model import WatchTask, Illust
-from ...service.pixiv_account_binder import PixivAccountBinder
-from ...utils.shared_agen import SharedAsyncGeneratorManager
-
-conf = context.require(Config)
-binder = context.require(PixivAccountBinder)
-pixiv = context.require(PixivRepo)
-
-
-# 因为要强制从远端获取，所以用这个shared_agen_mgr来缓存
-class WatchFollowingIllustsSharedAsyncGeneratorManager(SharedAsyncGeneratorManager[int, Illust]):
-    log_tag = "watch_following_illusts_shared_agen"
-
-    async def agen(self, identifier: int, cache_strategy: CacheStrategy, **kwargs):
-        await self.set_expires_time(identifier, time.time() + 30)  # 30s过期，保证每分钟的所有task都能共享
-        async for x in pixiv.user_following_illusts(user_id=identifier,
-                                                    cache_strategy=CacheStrategy.FORCE_EXPIRATION):
-            yield await x.get()
-
-
-shared_agen_mgr = WatchFollowingIllustsSharedAsyncGeneratorManager()
-
-
-class WatchFollowingIllustsHandler(WatchTaskHandler):
-    @classmethod
-    def type(cls) -> str:
-        return "watch_user_illusts"
-
-    # noinspection PyMethodOverriding
-    async def actual_handle(self, *, task: WatchTask):
-        pixiv_user_id = task.kwargs.get("pixiv_user_id", 0)
-        sender_user_id = task.kwargs.get("sender_user_id", 0)
-
-        if not pixiv_user_id and sender_user_id:
-            pixiv_user_id = await binder.get_binding(task.subscriber.platform, sender_user_id)
-
-        if not pixiv_user_id:
-            pixiv_user_id = conf.pixiv_random_bookmark_user_id
-
-        if not pixiv_user_id:
-            logger.warning(f"[watchman] no binding found for {task.subscriber.id1}")
-            return
-
-        async with shared_agen_mgr.get(pixiv_user_id) as illusts:
-            async for illust in illusts:
-                if illust.create_date <= task.checkpoint:
-                    break
-                logger.info(f"[watchman] send illust {illust.id} to {task.subscriber}")
-                await self.post_illust(illust, header="您关注的画师更新了")
+import time
+
+from nonebot import logger
+
+from .base import WatchTaskHandler
+from ..pkg_context import context
+from ...config import Config
+from ...data.pixiv_repo import PixivRepo
+from ...data.pixiv_repo.enums import CacheStrategy
+from ...model import WatchTask, Illust
+from ...service.pixiv_account_binder import PixivAccountBinder
+from ...utils.shared_agen import SharedAsyncGeneratorManager
+
+conf = context.require(Config)
+binder = context.require(PixivAccountBinder)
+pixiv = context.require(PixivRepo)
+
+
+# 因为要强制从远端获取，所以用这个shared_agen_mgr来缓存
+class WatchFollowingIllustsSharedAsyncGeneratorManager(SharedAsyncGeneratorManager[int, Illust]):
+    log_tag = "watch_following_illusts_shared_agen"
+
+    async def agen(self, identifier: int, cache_strategy: CacheStrategy, **kwargs):
+        await self.set_expires_time(identifier, time.time() + 30)  # 30s过期，保证每分钟的所有task都能共享
+        async for x in pixiv.user_following_illusts(user_id=identifier,
+                                                    cache_strategy=CacheStrategy.FORCE_EXPIRATION):
+            yield await x.get()
+
+
+shared_agen_mgr = WatchFollowingIllustsSharedAsyncGeneratorManager()
+
+
+class WatchFollowingIllustsHandler(WatchTaskHandler):
+    @classmethod
+    def type(cls) -> str:
+        return "watch_user_illusts"
+
+    # noinspection PyMethodOverriding
+    async def actual_handle(self, *, task: WatchTask):
+        pixiv_user_id = task.kwargs.get("pixiv_user_id", 0)
+        sender_user_id = task.kwargs.get("sender_user_id", 0)
+
+        if not pixiv_user_id and sender_user_id:
+            pixiv_user_id = await binder.get_binding(task.subscriber.platform, sender_user_id)
+
+        if not pixiv_user_id:
+            pixiv_user_id = conf.pixiv_random_bookmark_user_id
+
+        if not pixiv_user_id:
+            logger.warning(f"[watchman] no binding found for {task.subscriber.id1}")
+            return
+
+        async with shared_agen_mgr.get(pixiv_user_id) as illusts:
+            async for illust in illusts:
+                if illust.create_date <= task.checkpoint:
+                    break
+                logger.info(f"[watchman] send illust {illust.id} to {task.subscriber}")
+                await self.post_illust(illust, header="您关注的画师更新了")
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/handler/watch/user_illusts.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/handler/watch/user_illusts.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-import time
-
-from nonebot import logger
-
-from .base import WatchTaskHandler
-from ..pkg_context import context
-from ...data.pixiv_repo import PixivRepo
-from ...data.pixiv_repo.enums import CacheStrategy
-from ...data.pixiv_repo.remote_repo import RemotePixivRepo
-from ...model import WatchTask, Illust
-from ...utils.shared_agen import SharedAsyncGeneratorManager
-
-pixiv = context.require(PixivRepo)
-remote_pixiv = context.require(RemotePixivRepo)
-
-
-# 因为要强制从远端获取，所以用这个shared_agen_mgr来缓存
-class WatchUserIllustsSharedAsyncGeneratorManager(SharedAsyncGeneratorManager[int, Illust]):
-    log_tag = "watch_user_illusts_shared_agen"
-
-    async def agen(self, identifier: int, cache_strategy: CacheStrategy, **kwargs):
-        await self.set_expires_time(identifier, time.time() + 30)  # 30s过期，保证每分钟的所有task都能共享
-        async for x in pixiv.user_illusts(user_id=identifier,
-                                          cache_strategy=CacheStrategy.FORCE_EXPIRATION):
-            yield await x.get()
-
-
-shared_agen_mgr = WatchUserIllustsSharedAsyncGeneratorManager()
-
-
-class WatchUserIllustsHandler(WatchTaskHandler):
-    @classmethod
-    def type(cls) -> str:
-        return "watch_user_illusts"
-
-    # noinspection PyMethodOverriding
-    async def actual_handle(self, *, task: WatchTask):
-        async with shared_agen_mgr.get(task.kwargs["user_id"]) as illusts:
-            async for illust in illusts:
-                if illust.create_date <= task.checkpoint:
-                    break
-                logger.info(f"[watchman] send illust {illust.id} to {task.subscriber}")
-                await self.post_illust(illust, header="您订阅的画师更新了")
+import time
+
+from nonebot import logger
+
+from .base import WatchTaskHandler
+from ..pkg_context import context
+from ...data.pixiv_repo import PixivRepo
+from ...data.pixiv_repo.enums import CacheStrategy
+from ...data.pixiv_repo.remote_repo import RemotePixivRepo
+from ...model import WatchTask, Illust
+from ...utils.shared_agen import SharedAsyncGeneratorManager
+
+pixiv = context.require(PixivRepo)
+remote_pixiv = context.require(RemotePixivRepo)
+
+
+# 因为要强制从远端获取，所以用这个shared_agen_mgr来缓存
+class WatchUserIllustsSharedAsyncGeneratorManager(SharedAsyncGeneratorManager[int, Illust]):
+    log_tag = "watch_user_illusts_shared_agen"
+
+    async def agen(self, identifier: int, cache_strategy: CacheStrategy, **kwargs):
+        await self.set_expires_time(identifier, time.time() + 30)  # 30s过期，保证每分钟的所有task都能共享
+        async for x in pixiv.user_illusts(user_id=identifier,
+                                          cache_strategy=CacheStrategy.FORCE_EXPIRATION):
+            yield await x.get()
+
+
+shared_agen_mgr = WatchUserIllustsSharedAsyncGeneratorManager()
+
+
+class WatchUserIllustsHandler(WatchTaskHandler):
+    @classmethod
+    def type(cls) -> str:
+        return "watch_user_illusts"
+
+    # noinspection PyMethodOverriding
+    async def actual_handle(self, *, task: WatchTask):
+        async with shared_agen_mgr.get(task.kwargs["user_id"]) as illusts:
+            async for illust in illusts:
+                if illust.create_date <= task.checkpoint:
+                    break
+                logger.info(f"[watchman] send illust {illust.id} to {task.subscriber}")
+                await self.post_illust(illust, header="您订阅的画师更新了")
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/model/message/illust_message.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/model/message/illust_message.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-from io import BytesIO
-from typing import Optional
-
-from pydantic import BaseModel
-from tzlocal import get_localzone
-
-from .. import Illust
-from ...config import Config
-from ...data.pixiv_repo import PixivRepo
-from ...enums import BlockAction
-from ...global_context import context
-
-conf = context.require(Config)
-
-
-async def download_image(illust: Illust, page: int):
-    with BytesIO() as bio:
-        repo = context.require(PixivRepo)
-        async for x in repo.image(illust, page):
-            bio.write(x)
-            break
-        return bio.getvalue()
-
-
-class IllustMessageModel(BaseModel):
-    id: int
-    title: str = ""
-    author: str = ""
-    create_time: str = ""
-    link: str = ""
-    image: bytes = bytes(0)
-
-    header: Optional[str]
-    number: Optional[int]
-
-    page: int
-    total: int
-
-    block_action: Optional[BlockAction] = None
-    block_message: str = ""
-
-    @staticmethod
-    async def from_illust(illust: Illust, *,
-                          header: Optional[str] = None,
-                          number: Optional[int] = None,
-                          page: int = 0,
-                          block_r18: bool = False,
-                          block_r18g: bool = False) -> Optional["IllustMessageModel"]:
-        model = IllustMessageModel(id=illust.id, header=header, number=number, page=page, total=illust.page_count)
-
-        block_tags = [*conf.pixiv_block_tags]
-        if block_r18:
-            block_tags.append("R-18")
-        if block_r18g:
-            block_tags.append("R-18G")
-
-        if illust.has_tags(block_tags):
-            model.block_action = conf.pixiv_block_action
-            if conf.pixiv_block_action == BlockAction.no_image:
-                model.block_message = "该画像因含有不可描述的tag而被自主规制"
-            elif conf.pixiv_block_action == BlockAction.completely_block:
-                model.block_message = "该画像因含有不可描述的tag而被自主规制"
-                return model
-            elif conf.pixiv_block_action == BlockAction.no_reply:
-                return None
-        else:
-            model.image = await download_image(illust, page)
-        model.title = illust.title
-        model.author = f"{illust.user.name} ({illust.user.id})"
-        model.create_time = illust.create_date.astimezone(get_localzone()).strftime('%Y-%m-%d %H:%M:%S')
-        model.link = f"https://www.pixiv.net/artworks/{illust.id}"
-
-        return model
+from io import BytesIO
+from typing import Optional
+
+from pydantic import BaseModel
+from tzlocal import get_localzone
+
+from .. import Illust
+from ...config import Config
+from ...data.pixiv_repo import PixivRepo
+from ...enums import BlockAction
+from ...global_context import context
+
+conf = context.require(Config)
+
+
+async def download_image(illust: Illust, page: int):
+    with BytesIO() as bio:
+        repo = context.require(PixivRepo)
+        async for x in repo.image(illust, page):
+            bio.write(x)
+            break
+        return bio.getvalue()
+
+
+class IllustMessageModel(BaseModel):
+    id: int
+    title: str = ""
+    author: str = ""
+    create_time: str = ""
+    link: str = ""
+    image: bytes = bytes(0)
+
+    header: Optional[str]
+    number: Optional[int]
+
+    page: int
+    total: int
+
+    block_action: Optional[BlockAction] = None
+    block_message: str = ""
+
+    @staticmethod
+    async def from_illust(illust: Illust, *,
+                          header: Optional[str] = None,
+                          number: Optional[int] = None,
+                          page: int = 0,
+                          block_r18: bool = False,
+                          block_r18g: bool = False) -> Optional["IllustMessageModel"]:
+        model = IllustMessageModel(id=illust.id, header=header, number=number, page=page, total=illust.page_count)
+
+        block_tags = [*conf.pixiv_block_tags]
+        if block_r18:
+            block_tags.append("R-18")
+        if block_r18g:
+            block_tags.append("R-18G")
+
+        if illust.has_tags(block_tags):
+            model.block_action = conf.pixiv_block_action
+            if conf.pixiv_block_action == BlockAction.no_image:
+                model.block_message = "该画像因含有不可描述的tag而被自主规制"
+            elif conf.pixiv_block_action == BlockAction.completely_block:
+                model.block_message = "该画像因含有不可描述的tag而被自主规制"
+                return model
+            elif conf.pixiv_block_action == BlockAction.no_reply:
+                return None
+        else:
+            model.image = await download_image(illust, page)
+        model.title = illust.title
+        model.author = f"{illust.user.name} ({illust.user.id})"
+        model.create_time = illust.create_date.astimezone(get_localzone()).strftime('%Y-%m-%d %H:%M:%S')
+        model.link = f"https://www.pixiv.net/artworks/{illust.id}"
+
+        return model
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/platform/available/__init__.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/platform/available/__init__.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from ..func_manager import FuncManagerFactory
-
-
-def register(factory: FuncManagerFactory):
-    try:
-        from nonebot.adapters.onebot.v11 import Adapter
-        from .onebot_v11 import available
-        factory.register(Adapter.get_name(), "available", available)
-    except ImportError:
-        pass
-
-    try:
-        from nonebot.adapters.kaiheila import Adapter
-        from .kaiheila import available
-        factory.register(Adapter.get_name(), "available", available)
-    except ImportError:
-        pass
+from ..func_manager import FuncManagerFactory
+
+
+def register(factory: FuncManagerFactory):
+    try:
+        from nonebot.adapters.onebot.v11 import Adapter
+        from .onebot_v11 import available
+        factory.register(Adapter.get_name(), "available", available)
+    except ImportError:
+        pass
+
+    try:
+        from nonebot.adapters.kaiheila import Adapter
+        from .kaiheila import available
+        factory.register(Adapter.get_name(), "available", available)
+    except ImportError:
+        pass
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/platform/available/onebot_v11.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/platform/available/onebot_v11.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from nonebot import get_bot
-from nonebot.adapters.onebot.v11 import Bot
-from nonebot.exception import ActionFailed
-from nonebot_plugin_session import Session
-
-
-async def available(session: Session) -> bool:
-    bot: Bot = get_bot(session.bot_id)
-    try:
-        if session.id2 is not None:
-            group_info = await bot.get_group_info(group_id=int(session.id2))
-            # 如果机器人尚未加入群, group_create_time, group_level, max_member_count 和 member_count 将会为0
-            return group_info["member_count"] != 0
-        else:
-            friend_list = await bot.get_friend_list()
-            for friend in friend_list:
-                if friend["user_id"] == session.id1:
-                    return True
-            return False
-    except ActionFailed:
-        return False
+from nonebot import get_bot
+from nonebot.adapters.onebot.v11 import Bot
+from nonebot.exception import ActionFailed
+from nonebot_plugin_session import Session
+
+
+async def available(session: Session) -> bool:
+    bot: Bot = get_bot(session.bot_id)
+    try:
+        if session.id2 is not None:
+            group_info = await bot.get_group_info(group_id=int(session.id2))
+            # 如果机器人尚未加入群, group_create_time, group_level, max_member_count 和 member_count 将会为0
+            return group_info["member_count"] != 0
+        else:
+            friend_list = await bot.get_friend_list()
+            for friend in friend_list:
+                if friend["user_id"] == session.id1:
+                    return True
+            return False
+    except ActionFailed:
+        return False
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/plugin_service.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/plugin_service.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from nonebot import require
-
-require("nonebot_plugin_access_control")
-
-from nonebot_plugin_access_control.service import create_plugin_service
-
-plugin_service = create_plugin_service("nonebot_plugin_pixivbot")
-
-common_service = plugin_service.create_subservice("common")
-illust_service = common_service.create_subservice("illust")
-ranking_service = common_service.create_subservice("ranking")
-more_service = common_service.create_subservice("more")
-random_bookmark_service = common_service.create_subservice("random_bookmark")
-random_illust_service = common_service.create_subservice("random_illust")
-random_recommended_illust_service = common_service.create_subservice("random_recommended_illust")
-random_related_illust_service = common_service.create_subservice("random_related_illust")
-random_user_illust_service = common_service.create_subservice("random_user_illust")
-
-illust_link_service = plugin_service.create_subservice("illust_link")
-
-schedule_service = plugin_service.create_subservice("schedule")
-receive_schedule_service = schedule_service.create_subservice("receive")
-manage_schedule_service = schedule_service.create_subservice("manage")
-
-watch_service = plugin_service.create_subservice("watch")
-receive_watch_service = watch_service.create_subservice("receive")
-manage_watch_service = watch_service.create_subservice("manage")
-
-invalidate_cache_service = plugin_service.create_subservice("invalidate_cache")
-
-bind_service = plugin_service.create_subservice("bind")
-
-help_service = plugin_service.create_subservice("help")
-
-r18_service = plugin_service.create_subservice("r18")
-r18g_service = r18_service.create_subservice("g")
+from nonebot import require
+
+require("nonebot_plugin_access_control")
+
+from nonebot_plugin_access_control.service import create_plugin_service
+
+plugin_service = create_plugin_service("nonebot_plugin_pixivbot")
+
+common_service = plugin_service.create_subservice("common")
+illust_service = common_service.create_subservice("illust")
+ranking_service = common_service.create_subservice("ranking")
+more_service = common_service.create_subservice("more")
+random_bookmark_service = common_service.create_subservice("random_bookmark")
+random_illust_service = common_service.create_subservice("random_illust")
+random_recommended_illust_service = common_service.create_subservice("random_recommended_illust")
+random_related_illust_service = common_service.create_subservice("random_related_illust")
+random_user_illust_service = common_service.create_subservice("random_user_illust")
+
+illust_link_service = plugin_service.create_subservice("illust_link")
+
+schedule_service = plugin_service.create_subservice("schedule")
+receive_schedule_service = schedule_service.create_subservice("receive")
+manage_schedule_service = schedule_service.create_subservice("manage")
+
+watch_service = plugin_service.create_subservice("watch")
+receive_watch_service = watch_service.create_subservice("receive")
+manage_watch_service = watch_service.create_subservice("manage")
+
+invalidate_cache_service = plugin_service.create_subservice("invalidate_cache")
+
+bind_service = plugin_service.create_subservice("bind")
+
+help_service = plugin_service.create_subservice("help")
+
+r18_service = plugin_service.create_subservice("r18")
+r18g_service = r18_service.create_subservice("g")
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/service/interval_task_worker.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/interval_task_worker.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-from abc import ABC, abstractmethod
-from typing import Generic, TypeVar, AsyncIterable
-
-from apscheduler.triggers.base import BaseTrigger
-from nonebot import logger, Bot
-from nonebot.exception import ActionFailed
-from nonebot_plugin_apscheduler import scheduler as apscheduler
-from nonebot_plugin_session import Session, SessionIdType
-
-from ..data.interval_task_repo import IntervalTaskRepo
-from ..model.interval_task import IntervalTask
-from ..platform import platform_func
-from ..platform.func_manager import UnsupportedBotError
-from ..utils.lifecycler import on_bot_connect, on_bot_disconnect
-
-T = TypeVar("T", bound=IntervalTask)
-
-
-class IntervalTaskWorker(ABC, Generic[T]):
-    tag: str = ""
-
-    @property
-    @abstractmethod
-    def repo(self) -> IntervalTaskRepo[T]:
-        raise NotImplementedError()
-
-    def __init__(self):
-        @on_bot_connect(replay=True)
-        async def _(bot: Bot):
-            async for task in self.repo.get_by_bot(bot.self_id):
-                try:
-                    self._add_job(task)
-                except Exception as e:
-                    logger.opt(exception=e).error(f"[{self.tag}] error occurred when adding job for task \"{task}\"")
-
-        @on_bot_disconnect()
-        async def _(bot: Bot):
-            async for task in self.repo.get_by_bot(bot.self_id):
-                try:
-                    self._remove_job(task)
-                except Exception as e:
-                    logger.opt(exception=e).error(f"[{self.tag}] error occurred when removing job for task \"{task}\"")
-
-    @classmethod
-    def _make_job_id(cls, item: T):
-        return f'{cls.tag} {item.subscriber.get_id(SessionIdType.GROUP)} {item.code}'
-
-    @abstractmethod
-    async def _handle_trigger(self, item: T):
-        ...
-
-    async def _on_trigger(self, item: T):
-        logger.info(f"[{self.tag}] triggered \"{item}\"")
-
-        try:
-            await self._handle_trigger(item)
-        except ActionFailed as e:
-            logger.opt(exception=e).error(f"[{self.tag}] action failed when handling task \"{item.code}\"")
-
-            try:
-                available = await platform_func(item.subscriber.bot_type).available(item.subscriber)
-            except UnsupportedBotError:
-                available = True
-
-            if not available:
-                logger.info(f"[{self.tag}] {item.subscriber} is no longer available, removing all his tasks...")
-                await self.remove_all_by_subscriber(item.subscriber)
-
-    @abstractmethod
-    def _make_job_trigger(self, item: T) -> BaseTrigger:
-        ...
-
-    def _add_job(self, item: T):
-        job_id = self._make_job_id(item)
-        job_exists = apscheduler.get_job(job_id) is not None
-
-        if not job_exists:
-            trigger = self._make_job_trigger(item)
-
-            apscheduler.add_job(self._on_trigger, id=job_id, trigger=trigger,
-                                args=[item])
-            logger.success(f"[{self.tag}] added job \"{job_id}\"")
-        else:
-            logger.debug(f"[{self.tag}] job \"{job_id}\" already exists")
-
-    def _remove_job(self, item: T):
-        job_id = self._make_job_id(item)
-        apscheduler.remove_job(job_id)
-        logger.success(f"[{self.tag}] removed job \"{item}\"")
-
-    async def _check_by_subject(self, item: T) -> bool:
-        ...
-
-    async def _build_task(self, *args, **kwargs) -> T:
-        ...
-
-    async def add_task(self, *args, **kwargs) -> bool:
-        item = await self._build_task(*args, **kwargs)
-        ok = await self.repo.insert(item)
-        if ok:
-            logger.success(f"[{self.tag}] inserted task \"{item}\"")
-            self._add_job(item)
-        return ok
-
-    async def remove_task(self, session: Session, code: str) -> bool:
-        item = await self.repo.delete_one(session, code)
-        if item:
-            logger.success(f"[{self.tag}] removed task \"{item}\"")
-            self._remove_job(item)
-            return True
-        else:
-            return False
-
-    async def remove_all_by_subscriber(self, session: Session):
-        old = await self.repo.delete_many_by_session(session)
-        for item in old:
-            logger.success(f"[{self.tag}] removed task \"{item}\"")
-            self._remove_job(item)
-
-    async def get_by_subscriber(self, session: Session) -> AsyncIterable[T]:
-        async for x in self.repo.get_by_session(session):
-            yield x
+from abc import ABC, abstractmethod
+from typing import Generic, TypeVar, AsyncIterable
+
+from apscheduler.triggers.base import BaseTrigger
+from nonebot import logger, Bot
+from nonebot.exception import ActionFailed
+from nonebot_plugin_apscheduler import scheduler as apscheduler
+from nonebot_plugin_session import Session, SessionIdType
+
+from ..data.interval_task_repo import IntervalTaskRepo
+from ..model.interval_task import IntervalTask
+from ..platform import platform_func
+from ..platform.func_manager import UnsupportedBotError
+from ..utils.lifecycler import on_bot_connect, on_bot_disconnect
+
+T = TypeVar("T", bound=IntervalTask)
+
+
+class IntervalTaskWorker(ABC, Generic[T]):
+    tag: str = ""
+
+    @property
+    @abstractmethod
+    def repo(self) -> IntervalTaskRepo[T]:
+        raise NotImplementedError()
+
+    def __init__(self):
+        @on_bot_connect(replay=True)
+        async def _(bot: Bot):
+            async for task in self.repo.get_by_bot(bot.self_id):
+                try:
+                    self._add_job(task)
+                except Exception as e:
+                    logger.opt(exception=e).error(f"[{self.tag}] error occurred when adding job for task \"{task}\"")
+
+        @on_bot_disconnect()
+        async def _(bot: Bot):
+            async for task in self.repo.get_by_bot(bot.self_id):
+                try:
+                    self._remove_job(task)
+                except Exception as e:
+                    logger.opt(exception=e).error(f"[{self.tag}] error occurred when removing job for task \"{task}\"")
+
+    @classmethod
+    def _make_job_id(cls, item: T):
+        return f'{cls.tag} {item.subscriber.get_id(SessionIdType.GROUP)} {item.code}'
+
+    @abstractmethod
+    async def _handle_trigger(self, item: T):
+        ...
+
+    async def _on_trigger(self, item: T):
+        logger.info(f"[{self.tag}] triggered \"{item}\"")
+
+        try:
+            await self._handle_trigger(item)
+        except ActionFailed as e:
+            logger.opt(exception=e).error(f"[{self.tag}] action failed when handling task \"{item.code}\"")
+
+            try:
+                available = await platform_func(item.subscriber.bot_type).available(item.subscriber)
+            except UnsupportedBotError:
+                available = True
+
+            if not available:
+                logger.info(f"[{self.tag}] {item.subscriber} is no longer available, removing all his tasks...")
+                await self.remove_all_by_subscriber(item.subscriber)
+
+    @abstractmethod
+    def _make_job_trigger(self, item: T) -> BaseTrigger:
+        ...
+
+    def _add_job(self, item: T):
+        job_id = self._make_job_id(item)
+        job_exists = apscheduler.get_job(job_id) is not None
+
+        if not job_exists:
+            trigger = self._make_job_trigger(item)
+
+            apscheduler.add_job(self._on_trigger, id=job_id, trigger=trigger,
+                                args=[item])
+            logger.success(f"[{self.tag}] added job \"{job_id}\"")
+        else:
+            logger.debug(f"[{self.tag}] job \"{job_id}\" already exists")
+
+    def _remove_job(self, item: T):
+        job_id = self._make_job_id(item)
+        apscheduler.remove_job(job_id)
+        logger.success(f"[{self.tag}] removed job \"{item}\"")
+
+    async def _check_by_subject(self, item: T) -> bool:
+        ...
+
+    async def _build_task(self, *args, **kwargs) -> T:
+        ...
+
+    async def add_task(self, *args, **kwargs) -> bool:
+        item = await self._build_task(*args, **kwargs)
+        ok = await self.repo.insert(item)
+        if ok:
+            logger.success(f"[{self.tag}] inserted task \"{item}\"")
+            self._add_job(item)
+        return ok
+
+    async def remove_task(self, session: Session, code: str) -> bool:
+        item = await self.repo.delete_one(session, code)
+        if item:
+            logger.success(f"[{self.tag}] removed task \"{item}\"")
+            self._remove_job(item)
+            return True
+        else:
+            return False
+
+    async def remove_all_by_subscriber(self, session: Session):
+        old = await self.repo.delete_many_by_session(session)
+        for item in old:
+            logger.success(f"[{self.tag}] removed task \"{item}\"")
+            self._remove_job(item)
+
+    async def get_by_subscriber(self, session: Session) -> AsyncIterable[T]:
+        async for x in self.repo.get_by_session(session):
+            yield x
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/service/pixiv_service.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/pixiv_service.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,134 +1,134 @@
-from typing import List, Union, Tuple, Iterable, Sequence
-
-from nonebot import logger
-
-from nonebot_plugin_pixivbot.config import Config
-from nonebot_plugin_pixivbot.data.local_tag import LocalTagRepo
-from nonebot_plugin_pixivbot.data.pixiv_repo import LazyIllust, PixivRepo
-from nonebot_plugin_pixivbot.enums import RandomIllustMethod, RankingMode
-from nonebot_plugin_pixivbot.global_context import context
-from nonebot_plugin_pixivbot.model import Illust, User
-from nonebot_plugin_pixivbot.service.roulette import roulette
-from nonebot_plugin_pixivbot.utils.errors import BadRequestError, QueryError
-
-conf = context.require(Config)
-repo = context.require(PixivRepo)
-local_tags = context.require(LocalTagRepo)
-
-
-@context.register_singleton()
-class PixivService:
-
-    @staticmethod
-    def _handle_r18(illusts: Iterable[LazyIllust],
-                    exclude_r18: bool = False,
-                    exclude_r18g: bool = False) -> Iterable[LazyIllust]:
-        if not exclude_r18 and not exclude_r18g:
-            return illusts
-        else:
-            def _():
-                for x in illusts:
-                    if not x.loaded:
-                        continue
-                    if x.content.has_tag("R-18") and exclude_r18:
-                        continue
-                    if x.content.has_tag("R-18G") and exclude_r18g:
-                        continue
-                    yield x
-
-            return _()
-
-    async def _choice_and_load(self, illusts: Sequence[LazyIllust], random_method: RandomIllustMethod, count: int) \
-            -> List[Illust]:
-        if count <= 0:
-            raise BadRequestError("不合法的请求数量")
-        if count > conf.pixiv_max_item_per_query:
-            raise BadRequestError("数量超过单次请求上限")
-        if count > len(illusts):
-            raise QueryError("别看了，没有的。")
-
-        winners = roulette(illusts, random_method, count)
-        logger.info(f"[pixiv_service] choice {[x.id for x in winners]}")
-        return [await x.get() for x in winners]
-
-    async def illust_ranking(self, mode: RankingMode, range: Tuple[int, int]) -> List[Illust]:
-        # range 下标从1开始 闭区间
-        i = 1
-        li = []
-        async for x in repo.illust_ranking(mode):
-            if i > range[1]:
-                break
-            elif i >= range[0]:
-                li.append(await x.get())
-            i += 1
-        return li
-
-    async def illust_detail(self, illust: int) -> Illust:
-        async for x in repo.illust_detail(illust):
-            return x
-
-    async def random_illust(self, word: str,
-                            *, count: int = 1,
-                            exclude_r18: bool = False,
-                            exclude_r18g: bool = False) -> List[Illust]:
-        if conf.pixiv_tag_translation_enabled:
-            # 只有原word不是标签时获取翻译（例子：唐可可）
-            tag = await local_tags.find_by_name(word)
-            if not tag:
-                tag = await local_tags.find_by_translated_name(word)
-                if tag:
-                    logger.info(f"[pixiv_service] found translation {word} -> {tag.name}")
-                    word = tag.name
-
-        illusts = [x async for x in repo.search_illust(word)]
-        illusts = self._handle_r18(illusts, exclude_r18, exclude_r18g)
-        return await self._choice_and_load(list(illusts), conf.pixiv_random_illust_method, count)
-
-    async def get_user(self, user: Union[str, int]) -> User:
-        if isinstance(user, str):
-            async for x in repo.search_user(user):
-                logger.info(f"[pixiv_service] select user {x.name}({x.id})")
-                return x
-            raise QueryError("未找到用户")
-        else:
-            async for x in repo.user_detail(user):
-                return x
-
-    async def random_user_illust(self, user: Union[str, int],
-                                 *, count: int = 1,
-                                 exclude_r18: bool = False,
-                                 exclude_r18g: bool = False) -> Tuple[User, List[Illust]]:
-        user = await self.get_user(user)
-
-        illusts = [x async for x in repo.user_illusts(user.id)]
-        illusts = self._handle_r18(illusts, exclude_r18, exclude_r18g)
-        illust = await self._choice_and_load(list(illusts), conf.pixiv_random_user_illust_method, count)
-        return user, illust
-
-    async def random_recommended_illust(self, *, count: int = 1,
-                                        exclude_r18: bool = False,
-                                        exclude_r18g: bool = False) -> List[Illust]:
-        illusts = [x async for x in repo.recommended_illusts()]
-        return await self._choice_and_load(illusts, conf.pixiv_random_recommended_illust_method, count)
-
-    async def random_bookmark(self, pixiv_user_id: int = 0,
-                              *, count: int = 1,
-                              exclude_r18: bool = False,
-                              exclude_r18g: bool = False) -> List[Illust]:
-        illusts = [x async for x in repo.user_bookmarks(pixiv_user_id)]
-        illusts = self._handle_r18(illusts, exclude_r18, exclude_r18g)
-        return await self._choice_and_load(list(illusts), conf.pixiv_random_bookmark_method, count)
-
-    async def random_related_illust(self, illust_id: int,
-                                    *, count: int = 1,
-                                    exclude_r18: bool = False,
-                                    exclude_r18g: bool = False) -> List[Illust]:
-        if illust_id == 0:
-            raise BadRequestError("你还没有发送过请求")
-
-        illusts = [x async for x in repo.related_illusts(illust_id)]
-        illusts = self._handle_r18(illusts, exclude_r18, exclude_r18g)
-        return await self._choice_and_load(list(illusts), conf.pixiv_random_related_illust_method, count)
-
-
-__all__ = ("PixivService",)
+from typing import List, Union, Tuple, Iterable, Sequence
+
+from nonebot import logger
+
+from nonebot_plugin_pixivbot.config import Config
+from nonebot_plugin_pixivbot.data.local_tag import LocalTagRepo
+from nonebot_plugin_pixivbot.data.pixiv_repo import LazyIllust, PixivRepo
+from nonebot_plugin_pixivbot.enums import RandomIllustMethod, RankingMode
+from nonebot_plugin_pixivbot.global_context import context
+from nonebot_plugin_pixivbot.model import Illust, User
+from nonebot_plugin_pixivbot.service.roulette import roulette
+from nonebot_plugin_pixivbot.utils.errors import BadRequestError, QueryError
+
+conf = context.require(Config)
+repo = context.require(PixivRepo)
+local_tags = context.require(LocalTagRepo)
+
+
+@context.register_singleton()
+class PixivService:
+
+    @staticmethod
+    def _handle_r18(illusts: Iterable[LazyIllust],
+                    exclude_r18: bool = False,
+                    exclude_r18g: bool = False) -> Iterable[LazyIllust]:
+        if not exclude_r18 and not exclude_r18g:
+            return illusts
+        else:
+            def _():
+                for x in illusts:
+                    if not x.loaded:
+                        continue
+                    if x.content.has_tag("R-18") and exclude_r18:
+                        continue
+                    if x.content.has_tag("R-18G") and exclude_r18g:
+                        continue
+                    yield x
+
+            return _()
+
+    async def _choice_and_load(self, illusts: Sequence[LazyIllust], random_method: RandomIllustMethod, count: int) \
+            -> List[Illust]:
+        if count <= 0:
+            raise BadRequestError("不合法的请求数量")
+        if count > conf.pixiv_max_item_per_query:
+            raise BadRequestError("数量超过单次请求上限")
+        if count > len(illusts):
+            raise QueryError("别看了，没有的。")
+
+        winners = roulette(illusts, random_method, count)
+        logger.info(f"[pixiv_service] choice {[x.id for x in winners]}")
+        return [await x.get() for x in winners]
+
+    async def illust_ranking(self, mode: RankingMode, range: Tuple[int, int]) -> List[Illust]:
+        # range 下标从1开始 闭区间
+        i = 1
+        li = []
+        async for x in repo.illust_ranking(mode):
+            if i > range[1]:
+                break
+            elif i >= range[0]:
+                li.append(await x.get())
+            i += 1
+        return li
+
+    async def illust_detail(self, illust: int) -> Illust:
+        async for x in repo.illust_detail(illust):
+            return x
+
+    async def random_illust(self, word: str,
+                            *, count: int = 1,
+                            exclude_r18: bool = False,
+                            exclude_r18g: bool = False) -> List[Illust]:
+        if conf.pixiv_tag_translation_enabled:
+            # 只有原word不是标签时获取翻译（例子：唐可可）
+            tag = await local_tags.find_by_name(word)
+            if not tag:
+                tag = await local_tags.find_by_translated_name(word)
+                if tag:
+                    logger.info(f"[pixiv_service] found translation {word} -> {tag.name}")
+                    word = tag.name
+
+        illusts = [x async for x in repo.search_illust(word)]
+        illusts = self._handle_r18(illusts, exclude_r18, exclude_r18g)
+        return await self._choice_and_load(list(illusts), conf.pixiv_random_illust_method, count)
+
+    async def get_user(self, user: Union[str, int]) -> User:
+        if isinstance(user, str):
+            async for x in repo.search_user(user):
+                logger.info(f"[pixiv_service] select user {x.name}({x.id})")
+                return x
+            raise QueryError("未找到用户")
+        else:
+            async for x in repo.user_detail(user):
+                return x
+
+    async def random_user_illust(self, user: Union[str, int],
+                                 *, count: int = 1,
+                                 exclude_r18: bool = False,
+                                 exclude_r18g: bool = False) -> Tuple[User, List[Illust]]:
+        user = await self.get_user(user)
+
+        illusts = [x async for x in repo.user_illusts(user.id)]
+        illusts = self._handle_r18(illusts, exclude_r18, exclude_r18g)
+        illust = await self._choice_and_load(list(illusts), conf.pixiv_random_user_illust_method, count)
+        return user, illust
+
+    async def random_recommended_illust(self, *, count: int = 1,
+                                        exclude_r18: bool = False,
+                                        exclude_r18g: bool = False) -> List[Illust]:
+        illusts = [x async for x in repo.recommended_illusts()]
+        return await self._choice_and_load(illusts, conf.pixiv_random_recommended_illust_method, count)
+
+    async def random_bookmark(self, pixiv_user_id: int = 0,
+                              *, count: int = 1,
+                              exclude_r18: bool = False,
+                              exclude_r18g: bool = False) -> List[Illust]:
+        illusts = [x async for x in repo.user_bookmarks(pixiv_user_id)]
+        illusts = self._handle_r18(illusts, exclude_r18, exclude_r18g)
+        return await self._choice_and_load(list(illusts), conf.pixiv_random_bookmark_method, count)
+
+    async def random_related_illust(self, illust_id: int,
+                                    *, count: int = 1,
+                                    exclude_r18: bool = False,
+                                    exclude_r18g: bool = False) -> List[Illust]:
+        if illust_id == 0:
+            raise BadRequestError("你还没有发送过请求")
+
+        illusts = [x async for x in repo.related_illusts(illust_id)]
+        illusts = self._handle_r18(illusts, exclude_r18, exclude_r18g)
+        return await self._choice_and_load(list(illusts), conf.pixiv_random_related_illust_method, count)
+
+
+__all__ = ("PixivService",)
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/service/roulette.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/roulette.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-from time import time
-from typing import Sequence
-
-import numpy as np
-
-from nonebot_plugin_pixivbot.data.pixiv_repo import LazyIllust
-from nonebot_plugin_pixivbot.enums import RandomIllustMethod
-
-
-def uniform(illusts: Sequence[LazyIllust]) -> np.ndarray:
-    # 概率相等
-    n = len(illusts)
-    return np.ones(n) / n
-
-
-def bookmark_proportion(illusts: Sequence[LazyIllust]) -> np.ndarray:
-    # 概率正比于书签数
-    n = len(illusts)
-    p = np.zeros(n)
-
-    for i, x in enumerate(illusts):
-        if x.loaded:
-            p[i] = x.content.total_bookmarks + 10  # 加10平滑
-        else:
-            p[i] = 10
-
-    p = np.array(p)
-    return p / np.sum(p)
-
-
-def view_proportion(illusts: Sequence[LazyIllust]) -> np.ndarray:
-    # 概率正比于查看人数
-    n = len(illusts)
-    p = np.zeros(n)
-
-    for i, x in enumerate(illusts):
-        if x.loaded:
-            p[i] = x.content.total_view + 10  # 加10平滑
-        else:
-            p[i] = 10
-
-    p = np.array(p)
-    return p / np.sum(p)
-
-
-def timedelta_proportion(illusts: Sequence[LazyIllust]) -> np.ndarray:
-    # 概率正比于 exp(归一化后的画像发布时间差)
-    n = len(illusts)
-    p = np.zeros(n)
-
-    now = time()
-    min_p = 0
-    for i, x in enumerate(illusts):
-        if x.loaded:
-            p[i] = x.create_date.timestamp() - now
-            if p[i] < min_p:
-                min_p = p[i]
-        else:
-            p[i] = float("-inf")
-
-    if min_p == 0:
-        return uniform(illusts)
-    else:
-        p = p / -min_p  # 归一化
-        p = np.exp(p)
-        return p / np.sum(p)
-
-
-p_gen = {
-    RandomIllustMethod.uniform: uniform,
-    RandomIllustMethod.bookmark_proportion: bookmark_proportion,
-    RandomIllustMethod.view_proportion: view_proportion,
-    RandomIllustMethod.timedelta_proportion: timedelta_proportion,
-}
-
-
-def roulette(illusts: Sequence[LazyIllust], random_method: RandomIllustMethod, k: int) -> Sequence[LazyIllust]:
-    n = len(illusts)
-    p = p_gen[random_method](illusts)
-
-    if n <= k:
-        return illusts
-
-    rng = np.random.default_rng()
-    winners = rng.choice(n, k, False, p)
-    return [illusts[c] for c in winners]
+from time import time
+from typing import Sequence
+
+import numpy as np
+
+from nonebot_plugin_pixivbot.data.pixiv_repo import LazyIllust
+from nonebot_plugin_pixivbot.enums import RandomIllustMethod
+
+
+def uniform(illusts: Sequence[LazyIllust]) -> np.ndarray:
+    # 概率相等
+    n = len(illusts)
+    return np.ones(n) / n
+
+
+def bookmark_proportion(illusts: Sequence[LazyIllust]) -> np.ndarray:
+    # 概率正比于书签数
+    n = len(illusts)
+    p = np.zeros(n)
+
+    for i, x in enumerate(illusts):
+        if x.loaded:
+            p[i] = x.content.total_bookmarks + 10  # 加10平滑
+        else:
+            p[i] = 10
+
+    p = np.array(p)
+    return p / np.sum(p)
+
+
+def view_proportion(illusts: Sequence[LazyIllust]) -> np.ndarray:
+    # 概率正比于查看人数
+    n = len(illusts)
+    p = np.zeros(n)
+
+    for i, x in enumerate(illusts):
+        if x.loaded:
+            p[i] = x.content.total_view + 10  # 加10平滑
+        else:
+            p[i] = 10
+
+    p = np.array(p)
+    return p / np.sum(p)
+
+
+def timedelta_proportion(illusts: Sequence[LazyIllust]) -> np.ndarray:
+    # 概率正比于 exp(归一化后的画像发布时间差)
+    n = len(illusts)
+    p = np.zeros(n)
+
+    now = time()
+    min_p = 0
+    for i, x in enumerate(illusts):
+        if x.loaded:
+            p[i] = x.create_date.timestamp() - now
+            if p[i] < min_p:
+                min_p = p[i]
+        else:
+            p[i] = float("-inf")
+
+    if min_p == 0:
+        return uniform(illusts)
+    else:
+        p = p / -min_p  # 归一化
+        p = np.exp(p)
+        return p / np.sum(p)
+
+
+p_gen = {
+    RandomIllustMethod.uniform: uniform,
+    RandomIllustMethod.bookmark_proportion: bookmark_proportion,
+    RandomIllustMethod.view_proportion: view_proportion,
+    RandomIllustMethod.timedelta_proportion: timedelta_proportion,
+}
+
+
+def roulette(illusts: Sequence[LazyIllust], random_method: RandomIllustMethod, k: int) -> Sequence[LazyIllust]:
+    n = len(illusts)
+    p = p_gen[random_method](illusts)
+
+    if n <= k:
+        return illusts
+
+    rng = np.random.default_rng()
+    winners = rng.choice(n, k, False, p)
+    return [illusts[c] for c in winners]
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/service/watchman.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/service/watchman.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-from datetime import datetime, timedelta, timezone
-from typing import Dict, Any, overload, Type, TYPE_CHECKING
-
-from apscheduler.triggers.interval import IntervalTrigger
-from nonebot_plugin_session import Session
-
-from .interval_task_worker import IntervalTaskWorker
-from ..config import Config
-from ..data.watch_task import WatchTaskRepo
-from ..global_context import context
-from ..model import WatchTask, WatchType
-
-if TYPE_CHECKING:
-    from ..handler.base import Handler
-
-conf = context.require(Config)
-
-
-@context.root.register_eager_singleton()
-class Watchman(IntervalTaskWorker[WatchTask]):
-    tag = "watchman"
-
-    _trigger_hasher_mapper = {
-        WatchType.user_illusts: lambda item: item.kwargs["user_id"],
-        WatchType.following_illusts: lambda item: hash(item.subscriber.id1),
-    }
-
-    @property
-    def repo(self) -> WatchTaskRepo:
-        return context.require(WatchTaskRepo)
-
-    @classmethod
-    def _get_handler_type(cls, type: WatchType) -> Type["Handler"]:
-        from ..handler.watch import WatchUserIllustsHandler, WatchFollowingIllustsHandler
-
-        if type == WatchType.user_illusts:
-            return WatchUserIllustsHandler
-        elif type == WatchType.following_illusts:
-            return WatchFollowingIllustsHandler
-
-    async def _handle_trigger(self, item: WatchTask, manually: bool = False):
-        try:
-            handler_type = self._get_handler_type(item.type)
-            handler = handler_type(item.subscriber, silently=not manually, disable_interceptors=manually)
-            await handler.handle_with_parsed_args(task=item)
-        finally:
-            # 保存checkpoint，避免一次异常后下一次重复推送
-            # 但是会存在丢失推送的问题
-            item.checkpoint = datetime.now(timezone.utc)
-            await self.repo.update(item)
-
-    def _make_job_trigger(self, item: WatchTask) -> IntervalTrigger:
-        hasher = self._trigger_hasher_mapper[item.type]
-        hash_sec = hasher(item) % conf.pixiv_watch_interval
-        yesterday = datetime.now(timezone.utc).replace(
-            hour=0, minute=0, second=0, microsecond=0
-        ) + timedelta(days=-1) + timedelta(seconds=hash_sec)
-        trigger = IntervalTrigger(seconds=conf.pixiv_watch_interval, start_date=yesterday)
-        return trigger
-
-    async def _build_task(self, type_: WatchType,
-                          kwargs: Dict[str, Any],
-                          session: Session) -> WatchTask:
-        return WatchTask(type=type_, kwargs=kwargs,
-                         subscriber=session)
-
-    @overload
-    async def add_task(self, type_: WatchType,
-                       kwargs: Dict[str, Any],
-                       session: Session) -> bool:
-        ...
-
-    async def add_task(self, *args, **kwargs) -> bool:
-        return await super().add_task(*args, **kwargs)
-
-    async def fetch(self, code: str, session: Session) -> bool:
-        task = await self.repo.get_by_code(session, code)
-        if task is not None:
-            await self._handle_trigger(task, manually=True)
-            return True
-        return False
+from datetime import datetime, timedelta, timezone
+from typing import Dict, Any, overload, Type, TYPE_CHECKING
+
+from apscheduler.triggers.interval import IntervalTrigger
+from nonebot_plugin_session import Session
+
+from .interval_task_worker import IntervalTaskWorker
+from ..config import Config
+from ..data.watch_task import WatchTaskRepo
+from ..global_context import context
+from ..model import WatchTask, WatchType
+
+if TYPE_CHECKING:
+    from ..handler.base import Handler
+
+conf = context.require(Config)
+
+
+@context.root.register_eager_singleton()
+class Watchman(IntervalTaskWorker[WatchTask]):
+    tag = "watchman"
+
+    _trigger_hasher_mapper = {
+        WatchType.user_illusts: lambda item: item.kwargs["user_id"],
+        WatchType.following_illusts: lambda item: hash(item.subscriber.id1),
+    }
+
+    @property
+    def repo(self) -> WatchTaskRepo:
+        return context.require(WatchTaskRepo)
+
+    @classmethod
+    def _get_handler_type(cls, type: WatchType) -> Type["Handler"]:
+        from ..handler.watch import WatchUserIllustsHandler, WatchFollowingIllustsHandler
+
+        if type == WatchType.user_illusts:
+            return WatchUserIllustsHandler
+        elif type == WatchType.following_illusts:
+            return WatchFollowingIllustsHandler
+
+    async def _handle_trigger(self, item: WatchTask, manually: bool = False):
+        try:
+            handler_type = self._get_handler_type(item.type)
+            handler = handler_type(item.subscriber, silently=not manually, disable_interceptors=manually)
+            await handler.handle_with_parsed_args(task=item)
+        finally:
+            # 保存checkpoint，避免一次异常后下一次重复推送
+            # 但是会存在丢失推送的问题
+            item.checkpoint = datetime.now(timezone.utc)
+            await self.repo.update(item)
+
+    def _make_job_trigger(self, item: WatchTask) -> IntervalTrigger:
+        hasher = self._trigger_hasher_mapper[item.type]
+        hash_sec = hasher(item) % conf.pixiv_watch_interval
+        yesterday = datetime.now(timezone.utc).replace(
+            hour=0, minute=0, second=0, microsecond=0
+        ) + timedelta(days=-1) + timedelta(seconds=hash_sec)
+        trigger = IntervalTrigger(seconds=conf.pixiv_watch_interval, start_date=yesterday)
+        return trigger
+
+    async def _build_task(self, type_: WatchType,
+                          kwargs: Dict[str, Any],
+                          session: Session) -> WatchTask:
+        return WatchTask(type=type_, kwargs=kwargs,
+                         subscriber=session)
+
+    @overload
+    async def add_task(self, type_: WatchType,
+                       kwargs: Dict[str, Any],
+                       session: Session) -> bool:
+        ...
+
+    async def add_task(self, *args, **kwargs) -> bool:
+        return await super().add_task(*args, **kwargs)
+
+    async def fetch(self, code: str, session: Session) -> bool:
+        task = await self.repo.get_by_code(session, code)
+        if task is not None:
+            await self._handle_trigger(task, manually=True)
+            return True
+        return False
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/utils/decode_integer.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/decode_integer.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-__numerals = {'零': 0, '一': 1, '二': 2, '两': 2, '三': 3, '四': 4, '五': 5, '六': 6, '七': 7, '八': 8, '九': 9, '十': 10,
-              '百': 100, '千': 1000, '万': 10000, '亿': 100000000}
-
-
-def decode_chinese_integer(text: str) -> int:
-    """
-    将中文整数转换为int
-    :param text: 中文整数
-    :return: 对应int
-    """
-    ans = 0
-    radix = 1
-    for i in reversed(range(len(text))):
-        if text[i] not in __numerals:
-            raise ValueError()
-        digit = __numerals[text[i]]
-        if digit >= 10:
-            if digit > radix:  # 成为新的基数
-                radix = digit
-                if i == 0:  # 若给定字符串省略了最前面的“一”，如十三、十五……
-                    ans = ans + radix
-            else:
-                radix = radix * digit
-        else:
-            ans = ans + radix * digit
-
-    return ans
-
-
-def decode_integer(text: str) -> int:
-    try:
-        return int(text)
-    except ValueError:
-        pass
-
-    return decode_chinese_integer(text)
-
-
-__all__ = ("decode_integer", "decode_chinese_integer")
+__numerals = {'零': 0, '一': 1, '二': 2, '两': 2, '三': 3, '四': 4, '五': 5, '六': 6, '七': 7, '八': 8, '九': 9, '十': 10,
+              '百': 100, '千': 1000, '万': 10000, '亿': 100000000}
+
+
+def decode_chinese_integer(text: str) -> int:
+    """
+    将中文整数转换为int
+    :param text: 中文整数
+    :return: 对应int
+    """
+    ans = 0
+    radix = 1
+    for i in reversed(range(len(text))):
+        if text[i] not in __numerals:
+            raise ValueError()
+        digit = __numerals[text[i]]
+        if digit >= 10:
+            if digit > radix:  # 成为新的基数
+                radix = digit
+                if i == 0:  # 若给定字符串省略了最前面的“一”，如十三、十五……
+                    ans = ans + radix
+            else:
+                radix = radix * digit
+        else:
+            ans = ans + radix * digit
+
+    return ans
+
+
+def decode_integer(text: str) -> int:
+    try:
+        return int(text)
+    except ValueError:
+        pass
+
+    return decode_chinese_integer(text)
+
+
+__all__ = ("decode_integer", "decode_chinese_integer")
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/utils/expires_lru_dict.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/expires_lru_dict.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,103 +1,103 @@
-from collections import OrderedDict
-from dataclasses import dataclass
-from datetime import datetime, timezone
-from functools import total_ordering
-from heapq import heappop, heapify, heappush
-from typing import TypeVar, Generic, List, Optional, Callable, Union, Awaitable, AsyncIterator
-
-from nonebot_plugin_pixivbot.utils.coros import as_async
-
-_KT = TypeVar("_KT")
-_VT = TypeVar("_VT")
-
-
-@dataclass(frozen=True)
-@total_ordering
-class ExpiresNode(Generic[_KT, _VT]):
-    key: _KT
-    value: _VT
-    expires_time: datetime
-
-    def __le__(self, other: "ExpiresNode"):
-        return self.expires_time < other.expires_time
-
-
-class AsyncExpiresLruDict(Generic[_KT, _VT]):
-    def __init__(self, maxsize: int,
-                 on_cleanup: Optional[Callable[[_KT, _VT], Union[None, Awaitable[None]]]] = None):
-        self.maxsize = maxsize
-        self.on_cleanup = as_async(on_cleanup)
-
-        self._data = OrderedDict[_KT, ExpiresNode[_KT, _VT]]()
-        self._expires_heap: List[ExpiresNode[_KT, _VT]] = []
-
-    async def _collate(self, ensure_size_for_put: bool):
-        now = datetime.now(timezone.utc)
-        while len(self._expires_heap) > 0 and self._expires_heap[0].expires_time <= now:
-            node = self._expires_heap[0]
-            if self._data.get(node.key, None) is node:
-                del self._data[node.key]
-                self.on_cleanup and await self.on_cleanup(node.key, node.value)
-
-            heappop(self._expires_heap)
-
-        if ensure_size_for_put and len(self._data) == self.maxsize:
-            key, node = self._data.popitem(last=False)
-            self.on_cleanup and await self.on_cleanup(key, node.value)
-            # we will not remove items from expires_heap
-            # until its size reach the threshold (checked on add)
-
-    def _collate_expires_heap(self):
-        threshold = 2 * self.maxsize - 1
-
-        if len(self._expires_heap) > threshold:
-            # rebuild _expires_heap
-            self._expires_heap = []
-            for node in self._data.values():
-                self._expires_heap.append(node)
-            heapify(self._expires_heap)
-
-    async def add(self, key: _KT, value: _VT, expires_time: datetime):
-        await self._collate(True)
-
-        if self._data.__contains__(key):
-            raise KeyError(key)
-
-        node = ExpiresNode(key, value, expires_time)
-        self._data.__setitem__(key, node)
-        heappush(self._expires_heap, node)
-
-        self._collate_expires_heap()
-
-    async def set(self, key: _KT, value: _VT) -> None:
-        await self._collate(False)
-        if key not in self._data:
-            raise KeyError(key)
-
-        node = self._data.__getitem__(key)
-        self._data[key] = ExpiresNode(key, value, node.expires_time)
-
-    async def pop(self, key: _KT) -> _VT:
-        await self._collate(False)
-
-        # we will not remove items from expires_heap
-        # until its size reach the threshold (checked on add)
-        return self._data.pop(key)
-
-    async def get(self, key: _KT) -> _VT:
-        await self._collate(False)
-        node = self._data.get(key, None)
-        return node.value if node else None
-
-    async def len(self) -> int:
-        await self._collate(False)
-        return self._data.__len__()
-
-    async def iter(self) -> AsyncIterator[_KT]:
-        await self._collate(False)
-        for k in self._data.__iter__():
-            yield k
-
-    async def contains(self, key: _KT) -> bool:
-        await self._collate(False)
-        return self._data.__contains__(key)
+from collections import OrderedDict
+from dataclasses import dataclass
+from datetime import datetime, timezone
+from functools import total_ordering
+from heapq import heappop, heapify, heappush
+from typing import TypeVar, Generic, List, Optional, Callable, Union, Awaitable, AsyncIterator
+
+from nonebot_plugin_pixivbot.utils.coros import as_async
+
+_KT = TypeVar("_KT")
+_VT = TypeVar("_VT")
+
+
+@dataclass(frozen=True)
+@total_ordering
+class ExpiresNode(Generic[_KT, _VT]):
+    key: _KT
+    value: _VT
+    expires_time: datetime
+
+    def __le__(self, other: "ExpiresNode"):
+        return self.expires_time < other.expires_time
+
+
+class AsyncExpiresLruDict(Generic[_KT, _VT]):
+    def __init__(self, maxsize: int,
+                 on_cleanup: Optional[Callable[[_KT, _VT], Union[None, Awaitable[None]]]] = None):
+        self.maxsize = maxsize
+        self.on_cleanup = as_async(on_cleanup)
+
+        self._data = OrderedDict[_KT, ExpiresNode[_KT, _VT]]()
+        self._expires_heap: List[ExpiresNode[_KT, _VT]] = []
+
+    async def _collate(self, ensure_size_for_put: bool):
+        now = datetime.now(timezone.utc)
+        while len(self._expires_heap) > 0 and self._expires_heap[0].expires_time <= now:
+            node = self._expires_heap[0]
+            if self._data.get(node.key, None) is node:
+                del self._data[node.key]
+                self.on_cleanup and await self.on_cleanup(node.key, node.value)
+
+            heappop(self._expires_heap)
+
+        if ensure_size_for_put and len(self._data) == self.maxsize:
+            key, node = self._data.popitem(last=False)
+            self.on_cleanup and await self.on_cleanup(key, node.value)
+            # we will not remove items from expires_heap
+            # until its size reach the threshold (checked on add)
+
+    def _collate_expires_heap(self):
+        threshold = 2 * self.maxsize - 1
+
+        if len(self._expires_heap) > threshold:
+            # rebuild _expires_heap
+            self._expires_heap = []
+            for node in self._data.values():
+                self._expires_heap.append(node)
+            heapify(self._expires_heap)
+
+    async def add(self, key: _KT, value: _VT, expires_time: datetime):
+        await self._collate(True)
+
+        if self._data.__contains__(key):
+            raise KeyError(key)
+
+        node = ExpiresNode(key, value, expires_time)
+        self._data.__setitem__(key, node)
+        heappush(self._expires_heap, node)
+
+        self._collate_expires_heap()
+
+    async def set(self, key: _KT, value: _VT) -> None:
+        await self._collate(False)
+        if key not in self._data:
+            raise KeyError(key)
+
+        node = self._data.__getitem__(key)
+        self._data[key] = ExpiresNode(key, value, node.expires_time)
+
+    async def pop(self, key: _KT) -> _VT:
+        await self._collate(False)
+
+        # we will not remove items from expires_heap
+        # until its size reach the threshold (checked on add)
+        return self._data.pop(key)
+
+    async def get(self, key: _KT) -> _VT:
+        await self._collate(False)
+        node = self._data.get(key, None)
+        return node.value if node else None
+
+    async def len(self) -> int:
+        await self._collate(False)
+        return self._data.__len__()
+
+    async def iter(self) -> AsyncIterator[_KT]:
+        await self._collate(False)
+        for k in self._data.__iter__():
+            yield k
+
+    async def contains(self, key: _KT) -> bool:
+        await self._collate(False)
+        return self._data.__contains__(key)
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/src/nonebot_plugin_pixivbot/utils/shared_agen.py` & `nonebot_plugin_pixivbot-2.0.0a1/src/nonebot_plugin_pixivbot/utils/shared_agen.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,203 +1,203 @@
-import time
-from abc import ABC, abstractmethod
-from asyncio import Lock
-from contextlib import AbstractAsyncContextManager, asynccontextmanager
-from types import TracebackType
-from typing import Any, Generic, TypeVar, AsyncGenerator, List, Type, Optional, AsyncContextManager
-
-from cachetools import TLRUCache
-from nonebot import logger
-
-from nonebot_plugin_pixivbot.data.pixiv_repo.enums import CacheStrategy
-
-T_ID = TypeVar("T_ID")
-T_ITEM = TypeVar("T_ITEM")
-
-
-class SharedAsyncGeneratorManager(ABC, Generic[T_ID, T_ITEM]):
-    log_tag = "shared_agen"
-
-    class _AgenHolder(AbstractAsyncContextManager):
-        def __init__(self, origin: AsyncGenerator[T_ITEM, None],
-                     identifier: T_ID,
-                     manager: "SharedAsyncGeneratorManager"):
-            super().__init__()
-            self._origin = origin
-            self._stopped = False  # whether origin has raised a StopIteration
-            self._got_items = []  # items got from origin, used to replay
-            self._got = 0  # count of items got from origin
-            self._mutex = Lock()  # to solve race
-            self._consumers = 0  # count of consumer
-
-            self._identifier = identifier
-            self._manager = manager
-
-        @property
-        def consumers(self) -> int:
-            return self._consumers
-
-        async def _generator(self) -> AsyncGenerator[T_ITEM, None]:
-            cur = 0
-            while True:
-                if cur < self._got:
-                    yield self._got_items[cur]
-                    cur += 1
-                else:
-                    if self._stopped:
-                        break
-
-                    async with self._mutex:
-                        if self._stopped:
-                            break
-
-                        if cur == self._got:
-                            try:
-                                new_data = await self._origin.__anext__()
-                            except StopAsyncIteration:
-                                self._stopped = True
-                                await self._manager.on_agen_stop(self._identifier, self._got_items)
-                                break
-                            except Exception as e:
-                                await self._manager.on_agen_error(self._identifier, e)
-                                raise e
-
-                            await self._manager.on_agen_next(self._identifier, new_data)
-
-                            self._got_items.append(new_data)
-                            self._got += 1
-
-                        yield self._got_items[cur]
-                        cur += 1
-
-        async def __aenter__(self) -> AsyncGenerator[T_ITEM, None]:
-            self._consumers += 1
-            await self._manager._on_consumers_changed(self._identifier, self, self._consumers)
-            return self._generator()
-
-        async def __aexit__(self, exc_type: Optional[Type[BaseException]],
-                            exc_value: Optional[BaseException],
-                            traceback: Optional[TracebackType]) -> None:
-            self._consumers -= 1
-            await self._manager._on_consumers_changed(self._identifier, self, self._consumers)
-
-        async def aclose(self):
-            return await self._origin.aclose()
-
-    def __init__(self):
-        self._running_holders = dict[T_ID, self._AgenHolder]()
-        self._expires_time = dict[T_ID, float]()
-
-        self._stopped_holders = TLRUCache[T_ID, self._AgenHolder](maxsize=2048,
-                                                                  ttu=lambda k, v, now: self._expires_time[k],
-                                                                  timer=time.time)
-
-    @abstractmethod
-    def agen(self, identifier: T_ID,
-             cache_strategy: CacheStrategy,
-             **kwargs) -> AsyncGenerator[T_ITEM, None]:
-        raise NotImplementedError()
-
-    async def on_agen_next(self, identifier: T_ID, item: T_ITEM):
-        pass
-
-    async def on_agen_stop(self, identifier: T_ID, items: List[T_ITEM]):
-        # 如果用户手动调用invalidate，该holder已不存在于self._running_holders中
-        # 自然也不需要缓存到self._stopped_holders中
-        if identifier in self._running_holders:
-            holder = self._running_holders.pop(identifier)
-            if identifier in self._expires_time:
-                self._stopped_holders[identifier] = holder
-                logger.debug(f"[{self.log_tag}] {identifier} was stopped and cached")
-            else:
-                logger.debug(f"[{self.log_tag}] {identifier} was stopped but not cached")
-
-    async def on_agen_error(self, identifier: T_ID, e: Exception):
-        await self.invalidate(identifier)
-
-    async def _on_consumers_changed(self, identifier: T_ID,
-                                    holder: _AgenHolder,
-                                    consumers: int):
-        if identifier in self._running_holders and consumers == 0:
-            del self._running_holders[identifier]
-
-            if identifier in self._expires_time:
-                del self._expires_time[identifier]
-
-            await holder.aclose()
-            logger.debug(f"[{self.log_tag}] {identifier} cannot be reused "
-                         "(the origin agen hasn't stopped when all consumers exited)")
-
-    async def invalidate(self, identifier: T_ID):
-        if identifier in self._stopped_holders:
-            logger.debug(f"[{self.log_tag}] {identifier} was invalidated from cached state")
-            del self._stopped_holders[identifier]
-        elif identifier in self._running_holders:
-            logger.debug(f"[{self.log_tag}] {identifier} was invalidated from running state")
-            holder = self._running_holders.pop(identifier)
-            await holder.aclose()
-
-            if identifier in self._expires_time:
-                del self._expires_time[identifier]
-        else:
-            logger.debug(f"[{self.log_tag}] {identifier} was not found")
-            return
-
-    async def invalidate_all(self):
-        keys = {*self._stopped_holders.keys(), *self._running_holders.keys()}
-        for k in keys:
-            await self.invalidate(k)
-
-    def get_expires_time(self, identifier: T_ID) -> Optional[float]:
-        if identifier in self._stopped_holders:
-            t = self._stopped_holders.__getitem(identifier).expires
-            return t
-        elif identifier in self._running_holders:
-            t = self._expires_time.get(identifier, None)
-            return t
-        else:
-            return None
-
-    async def set_expires_time(self, identifier: T_ID, expires_time: float):
-        now = time.time()
-        if expires_time <= now:
-            await self.invalidate(identifier)
-            logger.debug(f"[{self.log_tag}] {identifier} was expired "
-                         "(due to a past expires time was set)")
-            return
-
-        if identifier in self._stopped_holders:
-            holder = self._stopped_holders.pop(identifier)
-
-            if expires_time > now:
-                self._expires_time[identifier] = expires_time
-                self._stopped_holders[identifier] = holder
-                del self._expires_time[identifier]
-
-                logger.debug(f"[{self.log_tag}] {identifier} will expires at {expires_time}")
-        elif identifier in self._running_holders:
-            self._expires_time[identifier] = expires_time
-            logger.debug(f"[{self.log_tag}] {identifier} will expire at {expires_time}")
-        else:
-            logger.warning(f"[{self.log_tag}] {identifier} was not found")
-
-    @asynccontextmanager
-    async def get(self, identifier: Any,
-                  cache_strategy: CacheStrategy = CacheStrategy.NORMAL,
-                  **kwargs) -> AsyncContextManager[AsyncGenerator[T_ITEM, None]]:
-        if cache_strategy == CacheStrategy.FORCE_EXPIRATION:
-            await self.invalidate(identifier)
-
-        holder = self._stopped_holders.get(identifier, None)
-        if holder is None:
-            holder = self._running_holders.get(identifier, None)
-            if holder is None:
-                origin = self.agen(identifier, cache_strategy, **kwargs)
-                holder = self._AgenHolder(origin, identifier, self)
-                logger.debug(f"[{self.log_tag}] {identifier} was created")
-                self._running_holders[identifier] = holder
-
-        async with holder as x:
-            yield x
-
-
-__all__ = ("SharedAsyncGeneratorManager",)
+import time
+from abc import ABC, abstractmethod
+from asyncio import Lock
+from contextlib import AbstractAsyncContextManager, asynccontextmanager
+from types import TracebackType
+from typing import Any, Generic, TypeVar, AsyncGenerator, List, Type, Optional, AsyncContextManager
+
+from cachetools import TLRUCache
+from nonebot import logger
+
+from nonebot_plugin_pixivbot.data.pixiv_repo.enums import CacheStrategy
+
+T_ID = TypeVar("T_ID")
+T_ITEM = TypeVar("T_ITEM")
+
+
+class SharedAsyncGeneratorManager(ABC, Generic[T_ID, T_ITEM]):
+    log_tag = "shared_agen"
+
+    class _AgenHolder(AbstractAsyncContextManager):
+        def __init__(self, origin: AsyncGenerator[T_ITEM, None],
+                     identifier: T_ID,
+                     manager: "SharedAsyncGeneratorManager"):
+            super().__init__()
+            self._origin = origin
+            self._stopped = False  # whether origin has raised a StopIteration
+            self._got_items = []  # items got from origin, used to replay
+            self._got = 0  # count of items got from origin
+            self._mutex = Lock()  # to solve race
+            self._consumers = 0  # count of consumer
+
+            self._identifier = identifier
+            self._manager = manager
+
+        @property
+        def consumers(self) -> int:
+            return self._consumers
+
+        async def _generator(self) -> AsyncGenerator[T_ITEM, None]:
+            cur = 0
+            while True:
+                if cur < self._got:
+                    yield self._got_items[cur]
+                    cur += 1
+                else:
+                    if self._stopped:
+                        break
+
+                    async with self._mutex:
+                        if self._stopped:
+                            break
+
+                        if cur == self._got:
+                            try:
+                                new_data = await self._origin.__anext__()
+                            except StopAsyncIteration:
+                                self._stopped = True
+                                await self._manager.on_agen_stop(self._identifier, self._got_items)
+                                break
+                            except Exception as e:
+                                await self._manager.on_agen_error(self._identifier, e)
+                                raise e
+
+                            await self._manager.on_agen_next(self._identifier, new_data)
+
+                            self._got_items.append(new_data)
+                            self._got += 1
+
+                        yield self._got_items[cur]
+                        cur += 1
+
+        async def __aenter__(self) -> AsyncGenerator[T_ITEM, None]:
+            self._consumers += 1
+            await self._manager._on_consumers_changed(self._identifier, self, self._consumers)
+            return self._generator()
+
+        async def __aexit__(self, exc_type: Optional[Type[BaseException]],
+                            exc_value: Optional[BaseException],
+                            traceback: Optional[TracebackType]) -> None:
+            self._consumers -= 1
+            await self._manager._on_consumers_changed(self._identifier, self, self._consumers)
+
+        async def aclose(self):
+            return await self._origin.aclose()
+
+    def __init__(self):
+        self._running_holders = dict[T_ID, self._AgenHolder]()
+        self._expires_time = dict[T_ID, float]()
+
+        self._stopped_holders = TLRUCache[T_ID, self._AgenHolder](maxsize=2048,
+                                                                  ttu=lambda k, v, now: self._expires_time[k],
+                                                                  timer=time.time)
+
+    @abstractmethod
+    def agen(self, identifier: T_ID,
+             cache_strategy: CacheStrategy,
+             **kwargs) -> AsyncGenerator[T_ITEM, None]:
+        raise NotImplementedError()
+
+    async def on_agen_next(self, identifier: T_ID, item: T_ITEM):
+        pass
+
+    async def on_agen_stop(self, identifier: T_ID, items: List[T_ITEM]):
+        # 如果用户手动调用invalidate，该holder已不存在于self._running_holders中
+        # 自然也不需要缓存到self._stopped_holders中
+        if identifier in self._running_holders:
+            holder = self._running_holders.pop(identifier)
+            if identifier in self._expires_time:
+                self._stopped_holders[identifier] = holder
+                logger.debug(f"[{self.log_tag}] {identifier} was stopped and cached")
+            else:
+                logger.debug(f"[{self.log_tag}] {identifier} was stopped but not cached")
+
+    async def on_agen_error(self, identifier: T_ID, e: Exception):
+        await self.invalidate(identifier)
+
+    async def _on_consumers_changed(self, identifier: T_ID,
+                                    holder: _AgenHolder,
+                                    consumers: int):
+        if identifier in self._running_holders and consumers == 0:
+            del self._running_holders[identifier]
+
+            if identifier in self._expires_time:
+                del self._expires_time[identifier]
+
+            await holder.aclose()
+            logger.debug(f"[{self.log_tag}] {identifier} cannot be reused "
+                         "(the origin agen hasn't stopped when all consumers exited)")
+
+    async def invalidate(self, identifier: T_ID):
+        if identifier in self._stopped_holders:
+            logger.debug(f"[{self.log_tag}] {identifier} was invalidated from cached state")
+            del self._stopped_holders[identifier]
+        elif identifier in self._running_holders:
+            logger.debug(f"[{self.log_tag}] {identifier} was invalidated from running state")
+            holder = self._running_holders.pop(identifier)
+            await holder.aclose()
+
+            if identifier in self._expires_time:
+                del self._expires_time[identifier]
+        else:
+            logger.debug(f"[{self.log_tag}] {identifier} was not found")
+            return
+
+    async def invalidate_all(self):
+        keys = {*self._stopped_holders.keys(), *self._running_holders.keys()}
+        for k in keys:
+            await self.invalidate(k)
+
+    def get_expires_time(self, identifier: T_ID) -> Optional[float]:
+        if identifier in self._stopped_holders:
+            t = self._stopped_holders.__getitem(identifier).expires
+            return t
+        elif identifier in self._running_holders:
+            t = self._expires_time.get(identifier, None)
+            return t
+        else:
+            return None
+
+    async def set_expires_time(self, identifier: T_ID, expires_time: float):
+        now = time.time()
+        if expires_time <= now:
+            await self.invalidate(identifier)
+            logger.debug(f"[{self.log_tag}] {identifier} was expired "
+                         "(due to a past expires time was set)")
+            return
+
+        if identifier in self._stopped_holders:
+            holder = self._stopped_holders.pop(identifier)
+
+            if expires_time > now:
+                self._expires_time[identifier] = expires_time
+                self._stopped_holders[identifier] = holder
+                del self._expires_time[identifier]
+
+                logger.debug(f"[{self.log_tag}] {identifier} will expires at {expires_time}")
+        elif identifier in self._running_holders:
+            self._expires_time[identifier] = expires_time
+            logger.debug(f"[{self.log_tag}] {identifier} will expire at {expires_time}")
+        else:
+            logger.warning(f"[{self.log_tag}] {identifier} was not found")
+
+    @asynccontextmanager
+    async def get(self, identifier: Any,
+                  cache_strategy: CacheStrategy = CacheStrategy.NORMAL,
+                  **kwargs) -> AsyncContextManager[AsyncGenerator[T_ITEM, None]]:
+        if cache_strategy == CacheStrategy.FORCE_EXPIRATION:
+            await self.invalidate(identifier)
+
+        holder = self._stopped_holders.get(identifier, None)
+        if holder is None:
+            holder = self._running_holders.get(identifier, None)
+            if holder is None:
+                origin = self.agen(identifier, cache_strategy, **kwargs)
+                holder = self._AgenHolder(origin, identifier, self)
+                logger.debug(f"[{self.log_tag}] {identifier} was created")
+                self._running_holders[identifier] = holder
+
+        async with holder as x:
+            yield x
+
+
+__all__ = ("SharedAsyncGeneratorManager",)
```

### Comparing `nonebot_plugin_pixivbot-2.0.0/PKG-INFO` & `nonebot_plugin_pixivbot-2.0.0a1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,377 +1,364 @@
-Metadata-Version: 2.1
-Name: nonebot-plugin-pixivbot
-Version: 2.0.0
-Summary: Nonebot Plugin PixivBot
-Home-page: https://github.com/ssttkkl/nonebot-plugin-pixivbot
-License: MIT
-Author: ssttkkl
-Author-email: huang.wen.long@hotmail.com
-Requires-Python: >=3.9,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Pillow (>=9.2.0,<10.0.0)
-Requires-Dist: PixivPy-Async (>=1.2.14,<2.0.0)
-Requires-Dist: aiohttp-socks (>=0.8.0,<0.9.0)
-Requires-Dist: asyncache (>=0.3.1,<0.4.0)
-Requires-Dist: cachetools (>=5.2.0,<6.0.0)
-Requires-Dist: frozendict (>=2.3.4,<3.0.0)
-Requires-Dist: lazy (>=1.4,<2.0)
-Requires-Dist: nonebot-plugin-access-control (>=0.5.5)
-Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.7,<0.3.0)
-Requires-Dist: nonebot-plugin-session (>=0.0.4)
-Requires-Dist: nonebot2 (>=2.0.0,<3.0.0)
-Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
-Requires-Dist: numpy (>=1.23.1,<2.0.0)
-Requires-Dist: shortuuid (>=1.0.9,<2.0.0)
-Requires-Dist: tzlocal (>=5.0.1,<6.0.0)
-Project-URL: Repository, https://github.com/ssttkkl/nonebot-plugin-pixivbot
-Description-Content-Type: text/markdown
-
-<!-- markdownlint-disable MD033 MD036 MD041 -->
-
-<p align="center">
-  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
-</p>
-
-<div align="center">
-
-nonebot_plugin_pixivbot
-=====
-
-_✨ PixivBot ✨_
-
-</div>
-
-<p align="center">
-  <a href="https://raw.githubusercontent.com/ssttkkl/nonebot-plugin-pixivbot/master/LICENSE">
-    <img src="https://img.shields.io/github/license/ssttkkl/nonebot-plugin-pixivbot.svg" alt="license">
-  </a>
-  <a href="https://pypi.python.org/pypi/nonebot-plugin-pixivbot">
-    <img src="https://img.shields.io/pypi/v/nonebot-plugin-pixivbot.svg" alt="pypi">
-  </a>
-  <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
-</p>
-
-NoneBot插件，支持发送随机Pixiv插画、画师更新推送、定时订阅推送……
-
-## 触发语句
-
-### 普通语句
-
-所有数字参数均支持中文数字和罗马数字。
-
-- **看看<类型>榜<范围>**：查看pixiv榜单（<类型>可省略，<范围>应为a-b或a）
-    - 示例：看看榜、看看日榜、看看榜1-5、看看月榜一
-- **来<数量>张图**：从推荐插画随机抽选一张插画（<数量>可省略，下同）
-    - 示例：来张图、来五张图
-- **来<数量>张<关键字>图**：搜索关键字，从搜索结果随机抽选一张插画
-    - 示例：来张初音ミク图、来五张初音ミク图
-    - 注：默认开启关键字翻译功能。Bot会在平时的数据爬取时记录各个Tag的中文翻译。在搜索时，若关键字的日文翻译存在，则使用日文翻译代替关键字进行搜索。
-- **来<数量>张<用户>老师的图**：搜索用户，从插画列表中随机抽选一张插画
-    - 示例：来张Rella老师的图、来五张Rella老师的图
-- **看看图<插画ID>**：查看ID对应的插画
-    - 示例：看看图114514
-- **来<数量>张私家车**：从书签中随机抽选一张插画（发送者需绑定Pixiv账号，或者在配置中指定默认Pixiv账号）
-    - 示例：来张私家车、来五张私家车
-- **还要**：重复上一次请求
-- **不够色**：获取上一张插画的相关插画
-
-### 命令语句
-
-- **/pixivbot schedule \<type\> \<schedule\> [..args]**：为本群（本用户）订阅类型为<type>的定时推送功能，时间满足<schedule>时进行推送
-    - \<type\>：可选值有ranking, random_bookmark, random_recommended_illust, random_illust, random_user_illust
-    - \<schedule\>：格式为HH:mm（每日固定时间点推送）或HH:mm*x（间隔时间推送），或者使用cron表达式
-    - [..args]：
-        - \<type\>为ranking时，接受mode、range
-            - 示例：/pixivbot schedle ranking 12:00 --mode day --range 1-10
-        - \<type\>为random_bookmark时，接受user
-            - 示例：/pixivbot schedle random_bookmark 01:00*x
-            - 示例：/pixivbot schedle random_bookmark 01:00*x --user 114514
-        - \<type\>为random_illust时，接受word（必需）
-            - 示例：/pixivbot schedle random_illust "0 */2 * * * *" --word ロリ
-            - 示例：/pixivbot schedle random_illust "0 */2 * * * *" --word "Hatsune Miku"
-        - \<type\>为random_user_illust时，接受user（必需）
-            - 示例：/pixivbot schedle random_user_illust 01:00*x --user 森倉円
-        - \<type\>为random_recommend_illust时，不接受参数
-- **/pixivbot schedule**：查看本群（本用户）的所有定时推送订阅
-- **/pixivbot unschedule \<id\>**：取消本群（本用户）的指定的定时推送订阅
-- **/pixivbot watch \<type\> [..args]**：为本群（本用户）订阅类型为<type>的更新推送功能
-    - \<type\>：可选值有user_illusts, following_illusts
-    - [..args]：
-        - \<type\>为user_illusts时，接受user（必需）
-            - 示例：/pixivbot watch user_illusts --user 森倉円
-        - \<type\>为following_illusts时，接受user
-            - 示例：/pixivbot watch following_illusts
-            - 示例：/pixivbot watch following_illusts --user 114514
-- **/pixivbot watch**：查看本群（本用户）的所有更新推送订阅
-- **/pixivbot watch fetch \<id\>**：【调试用命令】立刻手动触发一次指定的更新推送订阅
-- **/pixivbot unwatch \<id\> [..args]**：取消本群（本用户）的指定的更新推送订阅
-- **/pixivbot bind \<pixiv_user_id\>**：绑定Pixiv账号（用于随机书签功能）
-- **/pixivbot unbind**：解绑Pixiv账号
-- **/pixivbot invalidate_cache**：清除缓存（只有超级用户能够发送此命令）
-- **/pixivbot**、**/pixivbot help**：查看帮助
-
-## 环境配置
-
-事前准备：登录pixiv账号并获取refresh_token。（参考：[@ZipFile Pixiv OAuth Flow](https://gist.github.com/ZipFile/c9ebedb224406f4f11845ab700124362)
-、[eggplants/get-pixivpy-token](https://github.com/eggplants/get-pixivpy-token)）
-
-1. 参考[安装 | NoneBot](https://v2.nonebot.dev/docs/start/installation)安装NoneBot；
-2. 参考[创建项目 | NoneBot](https://v2.nonebot.dev/docs/tutorial/create-project)创建一个NoneBot实例；
-3. 使用`nb plugin install nonebot-plugin-pixivbot`安装插件；
-5. 在.env.prod中修改配置（参考下方）；
-
-## 配置外部数据库（可选）
-
-PixivBot需要使用数据库存放订阅以及缓存，默认使用SQLite。
-
-### SQLite
-
-若需要自定义SQLite数据库文件路径，请设置配置项：
-
-- pixiv_sql_conn_url=`sqlite+aiosqlite:///<数据库文件路径>`
-
-### PostgreSQL
-
-若需要使用PostgreSQL，请设置配置项：
-
-- pixiv_sql_conn_url=`postgresql+asyncpg://<用户名>:<密码>@<主机>:<端口>/<数据库名>`
-
-并且安装`nonebot-plugin-pixivbot[postgresql]`
-
-## 权限控制
-
-插件接入了[nonebot-plugin-access-control](https://github.com/ssttkkl/nonebot-plugin-access-control)实现细粒度的权限控制：
-
-```
-nonebot_plugin_pixivbot
-├── common
-│   ├── illust  （看看图）
-│   ├── ranking  （看看榜）
-│   ├── more  （还要）
-│   ├── random_bookmark  （来张私家车）
-│   ├── random_illust  （来张xx图）
-│   ├── random_recommended_illust  （来张图）
-│   ├── random_related_illust  （不够色）
-│   └── random_user_illust  （来张xx老师的图）
-├── illust_link  （P站链接嗅探）
-├── schedule
-│   ├── receive  （接收定时推送）
-│   └── manage  （管理定时推送）
-├── watch
-│   ├── receive  （接收更新推送）
-│   └── manage  （管理定时推送）
-├── invalidate_cache  （清除缓存）
-├── bind  （绑定P站账号）
-├── help  （帮助文本）
-└── r18  （显示R-18内容）
-    └── g  （显示R-18G内容）
-```
-
-譬如，超级用户可以通过发送`/ac permission deny --srv nonebot_plugin_pixivbot.r18 --sbj all`全局拦截R-18。
-
-又譬如，超级用户可以通过分别发送以下指令，使得只有超级用户、QQ私聊与QQ群聊的群管理能够调用`/pixivbot schedule`与`/pixivbot unschedule`命令。
-
-```
-/ac permission deny --srv nonebot_plugin_pixivbot.schedule.manage --sbj all
-/ac permission allow --srv nonebot_plugin_pixivbot.schedule.manage --sbj qq:private
-/ac permission allow --srv nonebot_plugin_pixivbot.schedule.manage --sbj qq:group_admin
-/ac permission allow --srv nonebot_plugin_pixivbot.schedule.manage --sbj superuser
-```
-
-具体可以参考[nonebot-plugin-access-control](https://github.com/ssttkkl/nonebot-plugin-access-control)的文档进行权限控制。
-
-## 常见问题
-
-**遇到问题时请先尝试执行`pip install nonebot-plugin-pixivbot -U`更新到最新版本**。
-
-Issue请尽可能带上详细的日志、配置文件与环境信息。功能请求请移步Discussion。
-
-### 内部错误：<class 'pixivpy_async.error.NoTokenError'>No access_token Found!
-
-没登录成功，多半是网络问题。在国内请配置代理。
-
-如果登录成功的话会在bot初始化后有这几句：
-
-```
-03-13 11:19:36 [SUCCESS] nonebot_plugin_pixivbot | refresh access token successfully. new token expires in 3600 seconds.
-03-13 11:19:36 [DEBUG] nonebot_plugin_pixivbot | access_token: ***************
-03-13 11:19:36 [DEBUG] nonebot_plugin_pixivbot | refresh_token: *****************
-```
-
-### 如何配置代理
-
-将`pixiv_proxy`配置项设为代理服务器地址（支持http、socks5协议）
-
-```
-pixiv_proxy=socks5://127.0.0.1:7890
-```
-
-### 发送合并转发消息惨遭风控
-
-将`pixiv_onebot_send_forward_message`配置项设为`never`可禁用合并转发
-
-### 内部错误：<class 'sqlalchemy.exc.OperationalError'>(sqlite3.OperationalError) near "ON": syntax error
-
-多半是SQLite版本过低，不支持ON CONFLICT子句，如果是Linux系统请更新安装的SQLite版本
-
-## 配置项一览
-
-最小配置：
-
-```
-pixiv_refresh_token=  # 前面获取的REFRESH_TOKEN
-```
-
-除最小配置出现的配置项以外都是可选项，给出的是默认值，建议只将自己需要的项加入.env.prod文件
-
-完整配置：
-
-```
-# 数据库配置
-pixiv_sql_conn_url=sqlite+aiosqlite:///pixiv_bot.db  # SQL连接URL，仅支持SQLite与PostgreSQL（通过SQLAlchemy进行连接，必须使用异步的DBAPI）
-pixiv_use_local_cache=True  # 是否启用本地缓存
-
-# 连接配置
-pixiv_refresh_token=  # 前面获取的REFRESH_TOKEN
-pixiv_proxy=  # 代理URL，推荐使用socks5代理
-pixiv_query_timeout=60  # 查询超时（单位：秒）
-pixiv_loading_prompt_delayed_time=5  # 加载提示消息的延迟时间（“努力加载中”的消息会在请求发出多少秒后发出）（单位：秒）
-pixiv_simultaneous_query=8  # 向Pixiv查询的并发数
-pixiv_download_custom_domain=  # 使用反向代理下载插画的域名
-
-# 查询设置
-pixiv_query_to_me_only=False  # 只响应关于Bot的查询
-pixiv_command_to_me_only=False  # 只响应关于Bot的命令
-
-pixiv_max_item_per_query=10  # 每个查询最多请求的插画数量
-
-pixiv_tag_translation_enabled=True  # 启用搜索关键字翻译功能（平时搜索时记录标签翻译，在查询时判断是否存在对应中日翻译）
-
-pixiv_block_tags=[]  # 当插画含有指定tag时会被阻拦
-pixiv_block_action=no_image  # 阻拦时的动作，可选值：no_image(不显示插画，回复插画信息), completely_block(只回复过滤提示), no_reply(无回复)
-
-pixiv_exclude_ai_illusts=False  # 是否过滤AI绘图作品
-
-pixiv_watch_interval=600  # 更新推送的查询间隔（单位：秒）
-
-# 插画压缩
-pixiv_compression_enabled=False  # 启用插画压缩
-pixiv_compression_max_size=  # 插画压缩最大尺寸
-pixiv_compression_quantity=  # 插画压缩品质（0到100）
-
-# 缓存过期时间/删除时间（单位：秒）
-pixiv_download_cache_expires_in=604800  # 默认值：7天
-pixiv_illust_detail_cache_expires_in=604800
-pixiv_user_detail_cache_expires_in=604800
-pixiv_illust_ranking_cache_expires_in=21600  # 默认值：6小时
-pixiv_search_illust_cache_expires_in=86400  # 默认值：1天
-pixiv_search_illust_cache_delete_in=2592000  # 默认值：30天
-pixiv_search_user_cache_expires_in=86400
-pixiv_search_user_cache_delete_in=2592000
-pixiv_user_illusts_cache_expires_in=86400
-pixiv_user_illusts_cache_delete_in=2592000
-pixiv_user_bookmarks_cache_expires_in=86400
-pixiv_user_bookmarks_cache_delete_in=2592000
-pixiv_related_illusts_cache_expires_in=86400
-pixiv_other_cache_expires_in=21600
-
-# QQ平台（主要是gocq）配置
-pixiv_poke_action=random_recommended_illust  # 响应戳一戳动作，可选值：ranking, random_recommended_illust, random_bookmark, 什么都不填即忽略戳一戳动作
-pixiv_send_illust_with_link=False  # 发图时是否带上链接（容易被tx盯上）
-pixiv_send_forward_message=auto  # 发图时是否使用转发消息的形式，可选值：always(永远使用), auto(仅在多张图片时使用), never(永远不使用)
-
-# 功能配置
-pixiv_more_enabled=True  # 启用重复上一次请求（还要）功能
-pixiv_query_expires_in=600  # 上一次请求的过期时间（单位：秒）
-
-pixiv_illust_query_enabled=True  # 启用插画查询（看看图）功能
-
-pixiv_ranking_query_enabled=True  # 启用榜单查询（看看榜）功能
-pixiv_ranking_default_mode=day  # 默认查询的榜单，可选值：day, week, month, day_male, day_female, week_original, week_rookie, day_manga
-pixiv_ranking_default_range=[1, 3]  # 默认查询的榜单范围
-pixiv_ranking_fetch_item=150  # 每次从服务器获取的榜单项数（查询的榜单范围必须在这个数目内）
-pixiv_ranking_max_item_per_query=5  # 每次榜单查询最多能查询多少项
-
-pixiv_random_illust_query_enabled=True  # 启用关键字插画随机抽选（来张xx图）功能
-pixiv_random_illust_method=bookmark_proportion  # 随机抽选方法，下同，可选值：bookmark_proportion(概率与书签数成正比), view_proportion(概率与阅读量成正比), timedelta_proportion(概率与投稿时间和现在的时间差成正比), uniform(相等概率)
-pixiv_random_illust_min_bookmark=0  # 过滤掉书签数小于该值的插画，下同
-pixiv_random_illust_min_view=0  # 过滤掉阅读量小于该值的插画，下同
-pixiv_random_illust_max_page=20  # 每次从服务器获取的查询结果页数，下同
-pixiv_random_illust_max_item=500  # 每次从服务器获取的查询结果项数，下同
-
-pixiv_random_recommended_illust_query_enabled=True  # 启用推荐插画随机抽选（来张图）功能
-pixiv_random_recommended_illust_method=uniform
-pixiv_random_recommended_illust_min_bookmark=0
-pixiv_random_recommended_illust_min_view=0
-pixiv_random_recommended_illust_max_page=40
-pixiv_random_recommended_illust_max_item=1000
-
-pixiv_random_related_illust_query_enabled=True  # 启用关联插画随机抽选（不够色）功能
-pixiv_random_related_illust_method=bookmark_proportion
-pixiv_random_related_illust_min_bookmark=0
-pixiv_random_related_illust_min_view=0
-pixiv_random_related_illust_max_page=4
-pixiv_random_related_illust_max_item=100
-
-pixiv_random_user_illust_query_enabled=True  # 启用用户插画随机抽选（来张xx老师的图）功能
-pixiv_random_user_illust_method=timedelta_proportion
-pixiv_random_user_illust_min_bookmark=0
-pixiv_random_user_illust_min_view=0
-pixiv_random_user_illust_max_page=2147483647
-pixiv_random_user_illust_max_item=2147483647
-
-pixiv_random_bookmark_query_enabled=True  # 启用用户书签随机抽选（来张私家车）功能
-pixiv_random_bookmark_user_id=0  # 当QQ用户未绑定Pixiv账号时，从该Pixiv账号的书签内抽选
-pixiv_random_bookmark_method=uniform
-pixiv_random_bookmark_min_bookmark=0
-pixiv_random_bookmark_min_view=0
-pixiv_random_bookmark_max_page=2147483647
-pixiv_random_bookmark_max_item=2147483647
-
-```
-
-## Special Thanks
-
-- [Mikubill/pixivpy-async](https://github.com/Mikubill/pixivpy-async)
-
-- [nonebot/nonebot2](https://github.com/nonebot/nonebot2)
-
-## 在线乞讨
-
-<details><summary>点击请我打两把maimai</summary>
-
-![](https://github.com/ssttkkl/ssttkkl/blob/main/afdian-ssttkkl.jfif)
-
-</details>
-
-## LICENSE
-
-```
-MIT License
-
-Copyright (c) 2021 ssttkkl
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
-```
-
+<!-- markdownlint-disable MD033 MD036 MD041 -->
+
+<p align="center">
+  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
+</p>
+
+<div align="center">
+
+nonebot_plugin_pixivbot
+=====
+
+_✨ PixivBot ✨_
+
+</div>
+
+<p align="center">
+  <a href="https://raw.githubusercontent.com/ssttkkl/nonebot-plugin-pixivbot/master/LICENSE">
+    <img src="https://img.shields.io/github/license/ssttkkl/nonebot-plugin-pixivbot.svg" alt="license">
+  </a>
+  <a href="https://pypi.python.org/pypi/nonebot-plugin-pixivbot">
+    <img src="https://img.shields.io/pypi/v/nonebot-plugin-pixivbot.svg" alt="pypi">
+  </a>
+  <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
+</p>
+
+NoneBot插件，支持发送随机Pixiv插画、画师更新推送、定时订阅推送……
+
+适配协议：
+
+- [Onebot V11](https://onebot.adapters.nonebot.dev/)
+- [KOOK / 开黑啦](https://github.com/Tian-que/nonebot-adapter-kaiheila)
+- [Telegram](https://github.com/nonebot/adapter-telegram)
+
+## 触发语句
+
+### 普通语句
+
+所有数字参数均支持中文数字和罗马数字。
+
+- **看看<类型>榜<范围>**：查看pixiv榜单（<类型>可省略，<范围>应为a-b或a）
+    - 示例：看看榜、看看日榜、看看榜1-5、看看月榜一
+- **来<数量>张图**：从推荐插画随机抽选一张插画（<数量>可省略，下同）
+    - 示例：来张图、来五张图
+- **来<数量>张<关键字>图**：搜索关键字，从搜索结果随机抽选一张插画
+    - 示例：来张初音ミク图、来五张初音ミク图
+    - 注：默认开启关键字翻译功能。Bot会在平时的数据爬取时记录各个Tag的中文翻译。在搜索时，若关键字的日文翻译存在，则使用日文翻译代替关键字进行搜索。
+- **来<数量>张<用户>老师的图**：搜索用户，从插画列表中随机抽选一张插画
+    - 示例：来张Rella老师的图、来五张Rella老师的图
+- **看看图<插画ID>**：查看ID对应的插画
+    - 示例：看看图114514
+- **来<数量>张私家车**：从书签中随机抽选一张插画（发送者需绑定Pixiv账号，或者在配置中指定默认Pixiv账号）
+    - 示例：来张私家车、来五张私家车
+- **还要**：重复上一次请求
+- **不够色**：获取上一张插画的相关插画
+
+### 命令语句
+
+- **/pixivbot schedule \<type\> \<schedule\> [..args]**：为本群（本用户）订阅类型为<type>的定时推送功能，时间满足<schedule>时进行推送
+    - \<type\>：可选值有ranking, random_bookmark, random_recommended_illust, random_illust, random_user_illust
+    - \<schedule\>：有三种格式，*00:30\*x*为每隔30分钟进行一次推送，*12:00*为每天12:00进行一次推送，*00:10+00:30\*x*为从今天00:
+      10开始每隔30分钟进行一次推送（开始时间若是一个过去的时间点，则从下一个开始推送的时间点进行推送）
+    - [..args]：
+        - \<type\>为ranking时，接受\<mode\> \<range\>
+            - 示例：/pixivbot schedle ranking 12:00 day 1-10
+        - \<type\>为random_bookmark时，接受\<pixiv_user_id\>（可空）
+            - 示例：/pixivbot schedle random_bookmark 01:00*x
+            - 示例：/pixivbot schedle random_bookmark 01:00*x 114514
+        - \<type\>为random_illust时，接受\<word\>，若需要输入空格请用反斜杠`\ `
+            - 示例：/pixivbot schedle random_illust 01:00*x
+            - 示例：/pixivbot schedle random_illust 01:00*x ロリ
+            - 示例：/pixivbot schedle random_illust 01:00*x Hatsune\ Miku
+        - \<type\>为random_user_illust时，接受\<user\>
+            - 示例：/pixivbot schedle random_user_illust 01:00*x 森倉円
+        - \<type\>为random_recommend_illust时，不接受参数
+- **/pixivbot schedule**：查看本群（本用户）的所有定时推送订阅
+- **/pixivbot unschedule \<id\>**：取消本群（本用户）的指定的定时推送订阅
+- **/pixivbot watch \<type\> [..args]**：为本群（本用户）订阅类型为<type>的更新推送功能
+    - \<type\>：可选值有user_illusts, following_illusts
+    - [..args]：
+        - \<type\>为user_illusts时，接受\<user\>
+            - 示例：/pixivbot watch user_illusts 森倉円
+        - \<type\>为following_illusts时，接受\<pixiv_user_id\>（可空）
+            - 示例：/pixivbot watch following_illusts
+            - 示例：/pixivbot watch following_illusts 114514
+- **/pixivbot watch**：查看本群（本用户）的所有更新推送订阅
+- **/pixivbot watch fetch \<id\>**：【调试用命令】立刻手动触发一次指定的更新推送订阅
+- **/pixivbot unwatch \<id\> [..args]**：取消本群（本用户）的指定的更新推送订阅
+- **/pixivbot bind \<pixiv_user_id\>**：绑定Pixiv账号（用于随机书签功能）
+- **/pixivbot unbind**：解绑Pixiv账号
+- **/pixivbot invalidate_cache**：清除缓存（只有超级用户能够发送此命令）
+- **/pixivbot**、**/pixivbot help**：查看帮助
+
+## 环境配置
+
+事前准备：登录pixiv账号并获取refresh_token。（参考：[@ZipFile Pixiv OAuth Flow](https://gist.github.com/ZipFile/c9ebedb224406f4f11845ab700124362)
+、[eggplants/get-pixivpy-token](https://github.com/eggplants/get-pixivpy-token)）
+
+1. 参考[安装 | NoneBot](https://v2.nonebot.dev/docs/start/installation)安装NoneBot；
+2. 参考[创建项目 | NoneBot](https://v2.nonebot.dev/docs/tutorial/create-project)创建一个NoneBot实例；
+3. 使用`nb plugin install nonebot-plugin-pixivbot`安装插件；
+5. 在.env.prod中修改配置（参考下方）；
+
+## 配置外部数据库（可选）
+
+PixivBot需要使用数据库存放订阅以及缓存，默认使用SQLite。
+
+### SQLite
+
+若需要自定义SQLite数据库文件路径，请设置配置项：
+
+- pixiv_sql_conn_url=`sqlite+aiosqlite:///<数据库文件路径>`
+
+### PostgreSQL
+
+若需要使用PostgreSQL，请设置配置项：
+
+- pixiv_sql_conn_url=`postgresql+asyncpg://<用户名>:<密码>@<主机>:<端口>/<数据库名>`
+
+并且安装`nonebot-plugin-pixivbot[postgresql]`
+
+### MongoDB
+
+若需要使用MongoDB，请设置配置项：
+
+- pixiv_mongo_conn_url=`mongodb://<用户名>:<密码>@<主机>:<端口>/<用户所属的数据库>`
+- pixiv_mongo_database_name=`连接的MongoDB数据库`
+
+并且安装`nonebot-plugin-pixivbot[mongo]`
+
+## 权限控制
+
+插件接入了[nonebot-plugin-access-control](https://github.com/ssttkkl/nonebot-plugin-access-control)实现细粒度的权限控制：
+
+```
+nonebot_plugin_pixivbot
+├── common
+│   ├── illust  （看看图）
+│   ├── ranking  （看看榜）
+│   ├── more  （还要）
+│   ├── random_bookmark  （来张私家车）
+│   ├── random_illust  （来张xx图）
+│   ├── random_recommended_illust  （来张图）
+│   ├── random_related_illust  （不够色）
+│   └── random_user_illust  （来张xx老师的图）
+├── illust_link  （P站链接嗅探）
+├── schedule
+│   ├── receive  （接收定时推送）
+│   └── manage  （管理定时推送）
+├── watch
+│   ├── receive  （接收更新推送）
+│   └── manage  （管理定时推送）
+├── invalidate_cache  （清除缓存）
+├── bind  （绑定P站账号）
+├── help  （帮助文本）
+└── r18  （显示R-18内容）
+    └── g  （显示R-18G内容）
+```
+
+譬如，超级用户可以通过发送`/ac permission deny --srv nonebot_plugin_pixivbot.r18 --sbj all`全局拦截R-18。
+
+又譬如，超级用户可以通过分别发送以下指令，使得只有超级用户、QQ私聊与QQ群聊的群管理能够调用`/pixivbot schedule`与`/pixivbot unschedule`命令。
+
+```
+/ac permission deny --srv nonebot_plugin_pixivbot.schedule.manage --sbj all
+/ac permission allow --srv nonebot_plugin_pixivbot.schedule.manage --sbj qq:private
+/ac permission allow --srv nonebot_plugin_pixivbot.schedule.manage --sbj qq:group_admin
+/ac permission allow --srv nonebot_plugin_pixivbot.schedule.manage --sbj superuser
+```
+
+具体可以参考[nonebot-plugin-access-control](https://github.com/ssttkkl/nonebot-plugin-access-control)的文档进行权限控制。
+
+## 常见问题
+
+**遇到问题时请先尝试执行`pip install nonebot-plugin-pixivbot -U`更新到最新版本**。
+
+Issue请尽可能带上详细的日志、配置文件与环境信息。功能请求请移步Discussion。
+
+### 内部错误：<class 'pixivpy_async.error.NoTokenError'>No access_token Found!
+
+没登录成功，多半是网络问题。在国内请配置代理。
+
+如果登录成功的话会在bot初始化后有这几句：
+
+```
+03-13 11:19:36 [SUCCESS] nonebot_plugin_pixivbot | refresh access token successfully. new token expires in 3600 seconds.
+03-13 11:19:36 [DEBUG] nonebot_plugin_pixivbot | access_token: ***************
+03-13 11:19:36 [DEBUG] nonebot_plugin_pixivbot | refresh_token: *****************
+```
+
+### 如何配置代理
+
+将`pixiv_proxy`配置项设为代理服务器地址（支持http、socks5协议）
+
+```
+pixiv_proxy=socks5://127.0.0.1:7890
+```
+
+### 发送合并转发消息惨遭风控
+
+将`pixiv_onebot_send_forward_message`配置项设为`never`可禁用合并转发
+
+### 内部错误：<class 'sqlalchemy.exc.OperationalError'>(sqlite3.OperationalError) near "ON": syntax error
+
+多半是SQLite版本过低，不支持ON CONFLICT子句，如果是Linux系统请更新安装的SQLite版本
+
+## 配置项一览
+
+最小配置：
+
+```
+pixiv_refresh_token=  # 前面获取的REFRESH_TOKEN
+```
+
+除最小配置出现的配置项以外都是可选项，给出的是默认值，建议只将自己需要的项加入.env.prod文件
+
+完整配置：
+
+```
+# 数据库配置
+pixiv_data_source=  # 使用的数据库类型，可选值：sql，mongo。若未设置，则根据是否设置了pixiv_mongo_conn_url自动判断。
+pixiv_sql_conn_url=sqlite+aiosqlite:///pixiv_bot.db  # SQL连接URL，仅支持SQLite与PostgreSQL（通过SQLAlchemy进行连接，必须使用异步的DBAPI）
+pixiv_mongo_conn_url=  # MongoDB连接URL，格式：mongodb://<用户名>:<密码>@<主机>:<端口>/<数据库>。
+pixiv_mongo_database_name=  # 连接的MongoDB数据库
+pixiv_use_local_cache=True  # 是否启用本地缓存
+
+# 连接配置
+pixiv_refresh_token=  # 前面获取的REFRESH_TOKEN
+pixiv_proxy=  # 代理URL，推荐使用socks5代理
+pixiv_query_timeout=60  # 查询超时（单位：秒）
+pixiv_loading_prompt_delayed_time=5  # 加载提示消息的延迟时间（“努力加载中”的消息会在请求发出多少秒后发出）（单位：秒）
+pixiv_simultaneous_query=8  # 向Pixiv查询的并发数
+pixiv_download_custom_domain=  # 使用反向代理下载插画的域名
+
+# 查询设置
+pixiv_query_to_me_only=False  # 只响应关于Bot的查询
+pixiv_command_to_me_only=False  # 只响应关于Bot的命令
+
+pixiv_max_item_per_query=10  # 每个查询最多请求的插画数量
+
+pixiv_tag_translation_enabled=True  # 启用搜索关键字翻译功能（平时搜索时记录标签翻译，在查询时判断是否存在对应中日翻译）
+
+pixiv_block_tags=[]  # 当插画含有指定tag时会被阻拦
+pixiv_block_action=no_image  # 阻拦时的动作，可选值：no_image(不显示插画，回复插画信息), completely_block(只回复过滤提示), no_reply(无回复)
+
+pixiv_exclude_ai_illusts=False  # 是否过滤AI绘图作品
+
+pixiv_watch_interval=600  # 更新推送的查询间隔（单位：秒）
+
+# 插画压缩
+pixiv_compression_enabled=False  # 启用插画压缩
+pixiv_compression_max_size=  # 插画压缩最大尺寸
+pixiv_compression_quantity=  # 插画压缩品质（0到100）
+
+# 缓存过期时间/删除时间（单位：秒）
+pixiv_download_cache_expires_in=604800  # 默认值：7天
+pixiv_illust_detail_cache_expires_in=604800
+pixiv_user_detail_cache_expires_in=604800
+pixiv_illust_ranking_cache_expires_in=21600  # 默认值：6小时
+pixiv_search_illust_cache_expires_in=86400  # 默认值：1天
+pixiv_search_illust_cache_delete_in=2592000  # 默认值：30天
+pixiv_search_user_cache_expires_in=86400
+pixiv_search_user_cache_delete_in=2592000
+pixiv_user_illusts_cache_expires_in=86400
+pixiv_user_illusts_cache_delete_in=2592000
+pixiv_user_bookmarks_cache_expires_in=86400
+pixiv_user_bookmarks_cache_delete_in=2592000
+pixiv_related_illusts_cache_expires_in=86400
+pixiv_other_cache_expires_in=21600
+
+# QQ平台（主要是gocq）配置
+pixiv_poke_action=random_recommended_illust  # 响应戳一戳动作，可选值：ranking, random_recommended_illust, random_bookmark, 什么都不填即忽略戳一戳动作
+pixiv_onebot_with_link=False  # 发图时是否带上链接（容易被tx盯上）
+pixiv_onebot_send_forward_message=auto  # 发图时是否使用转发消息的形式，可选值：always(永远使用), auto(仅在多张图片时使用), never(永远不使用)
+
+# 功能配置
+pixiv_more_enabled=True  # 启用重复上一次请求（还要）功能
+pixiv_query_expires_in=600  # 上一次请求的过期时间（单位：秒）
+
+pixiv_illust_query_enabled=True  # 启用插画查询（看看图）功能
+
+pixiv_ranking_query_enabled=True  # 启用榜单查询（看看榜）功能
+pixiv_ranking_default_mode=day  # 默认查询的榜单，可选值：day, week, month, day_male, day_female, week_original, week_rookie, day_manga
+pixiv_ranking_default_range=[1, 3]  # 默认查询的榜单范围
+pixiv_ranking_fetch_item=150  # 每次从服务器获取的榜单项数（查询的榜单范围必须在这个数目内）
+pixiv_ranking_max_item_per_query=5  # 每次榜单查询最多能查询多少项
+
+pixiv_random_illust_query_enabled=True  # 启用关键字插画随机抽选（来张xx图）功能
+pixiv_random_illust_method=bookmark_proportion  # 随机抽选方法，下同，可选值：bookmark_proportion(概率与书签数成正比), view_proportion(概率与阅读量成正比), timedelta_proportion(概率与投稿时间和现在的时间差成正比), uniform(相等概率)
+pixiv_random_illust_min_bookmark=0  # 过滤掉书签数小于该值的插画，下同
+pixiv_random_illust_min_view=0  # 过滤掉阅读量小于该值的插画，下同
+pixiv_random_illust_max_page=20  # 每次从服务器获取的查询结果页数，下同
+pixiv_random_illust_max_item=500  # 每次从服务器获取的查询结果项数，下同
+
+pixiv_random_recommended_illust_query_enabled=True  # 启用推荐插画随机抽选（来张图）功能
+pixiv_random_recommended_illust_method=uniform
+pixiv_random_recommended_illust_min_bookmark=0
+pixiv_random_recommended_illust_min_view=0
+pixiv_random_recommended_illust_max_page=40
+pixiv_random_recommended_illust_max_item=1000
+
+pixiv_random_related_illust_query_enabled=True  # 启用关联插画随机抽选（不够色）功能
+pixiv_random_related_illust_method=bookmark_proportion
+pixiv_random_related_illust_min_bookmark=0
+pixiv_random_related_illust_min_view=0
+pixiv_random_related_illust_max_page=4
+pixiv_random_related_illust_max_item=100
+
+pixiv_random_user_illust_query_enabled=True  # 启用用户插画随机抽选（来张xx老师的图）功能
+pixiv_random_user_illust_method=timedelta_proportion
+pixiv_random_user_illust_min_bookmark=0
+pixiv_random_user_illust_min_view=0
+pixiv_random_user_illust_max_page=2147483647
+pixiv_random_user_illust_max_item=2147483647
+
+pixiv_random_bookmark_query_enabled=True  # 启用用户书签随机抽选（来张私家车）功能
+pixiv_random_bookmark_user_id=0  # 当QQ用户未绑定Pixiv账号时，从该Pixiv账号的书签内抽选
+pixiv_random_bookmark_method=uniform
+pixiv_random_bookmark_min_bookmark=0
+pixiv_random_bookmark_min_view=0
+pixiv_random_bookmark_max_page=2147483647
+pixiv_random_bookmark_max_item=2147483647
+
+```
+
+## Special Thanks
+
+- [Mikubill/pixivpy-async](https://github.com/Mikubill/pixivpy-async)
+
+- [nonebot/nonebot2](https://github.com/nonebot/nonebot2)
+
+## 在线乞讨
+
+<details><summary>点击请我打两把maimai</summary>
+
+![](https://github.com/ssttkkl/ssttkkl/blob/main/afdian-ssttkkl.jfif)
+
+</details>
+
+## LICENSE
+
+```
+MIT License
+
+Copyright (c) 2021 ssttkkl
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+```
```

#### html2text {}

```diff
@@ -1,30 +1,14 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-pixivbot Version: 2.0.0 Summary:
-Nonebot Plugin PixivBot Home-page: https://github.com/ssttkkl/nonebot-plugin-
-pixivbot License: MIT Author: ssttkkl Author-email: huang.wen.long@hotmail.com
-Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: Pillow
-(>=9.2.0,<10.0.0) Requires-Dist: PixivPy-Async (>=1.2.14,<2.0.0) Requires-Dist:
-aiohttp-socks (>=0.8.0,<0.9.0) Requires-Dist: asyncache (>=0.3.1,<0.4.0)
-Requires-Dist: cachetools (>=5.2.0,<6.0.0) Requires-Dist: frozendict
-(>=2.3.4,<3.0.0) Requires-Dist: lazy (>=1.4,<2.0) Requires-Dist: nonebot-
-plugin-access-control (>=0.5.5) Requires-Dist: nonebot-plugin-send-anything-
-anywhere (>=0.2.7,<0.3.0) Requires-Dist: nonebot-plugin-session (>=0.0.4)
-Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Requires-Dist:
-nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist: numpy
-(>=1.23.1,<2.0.0) Requires-Dist: shortuuid (>=1.0.9,<2.0.0) Requires-Dist:
-tzlocal (>=5.0.1,<6.0.0) Project-URL: Repository, https://github.com/ssttkkl/
-nonebot-plugin-pixivbot Description-Content-Type: text/markdown
                                    [nonebot]
                nonebot_plugin_pixivbot ===== _â¨ PixivBot â¨_
                            [license] [pypi] [python]
 NoneBotæä»¶ï¼æ¯æåééæºPixivæç»ãç»å¸æ´æ°æ¨éãå®æ¶è®¢éæ¨éâ¦â¦
-## è§¦åè¯­å¥ ### æ®éè¯­å¥
+ééåè®®ï¼ - [Onebot V11](https://onebot.adapters.nonebot.dev/) - [KOOK /
+å¼é»å¦](https://github.com/Tian-que/nonebot-adapter-kaiheila) - [Telegram]
+(https://github.com/nonebot/adapter-telegram) ## è§¦åè¯­å¥ ### æ®éè¯­å¥
 æææ°å­åæ°åæ¯æä¸­ææ°å­åç½é©¬æ°å­ã -
 **çç<ç±»å>æ¦<èå´>**ï¼æ¥çpixivæ¦åï¼<ç±»å>å¯çç¥ï¼<èå´>åºä¸ºa-
 bæaï¼ - ç¤ºä¾ï¼ççæ¦ãççæ¥æ¦ãççæ¦1-5ãççææ¦ä¸ -
 **æ¥<æ°é>å¼ å¾**ï¼ä»æ¨èæç»éæºæ½éä¸å¼ æç»ï¼<æ°é>å¯çç¥ï¼ä¸åï¼
 - ç¤ºä¾ï¼æ¥å¼ å¾ãæ¥äºå¼ å¾ -
 **æ¥<æ°é>å¼ <å³é®å­>å¾**ï¼æç´¢å³é®å­ï¼ä»æç´¢ç»æéæºæ½éä¸å¼ æç»
 - ç¤ºä¾ï¼æ¥å¼ åé³ãã¯å¾ãæ¥äºå¼ åé³ãã¯å¾ -
@@ -40,39 +24,44 @@
 pixivbot schedule \
 > \
 >
 [..args]**ï¼ä¸ºæ¬ç¾¤ï¼æ¬ç¨æ·ï¼è®¢éç±»åä¸ºçå®æ¶æ¨éåè½ï¼æ¶é´æ»¡è¶³æ¶è¿è¡æ¨é
 - \
 >ï¼å¯éå¼æranking, random_bookmark, random_recommended_illust,
 random_illust, random_user_illust - \
->ï¼æ ¼å¼ä¸ºHH:mmï¼æ¯æ¥åºå®æ¶é´ç¹æ¨éï¼æHH:
-mm*xï¼é´éæ¶é´æ¨éï¼ï¼æèä½¿ç¨cronè¡¨è¾¾å¼ - [..args]ï¼ - \
->ä¸ºrankingæ¶ï¼æ¥åmodeãrange - ç¤ºä¾ï¼/pixivbot schedle ranking 12:00
---mode day --range 1-10 - \
->ä¸ºrandom_bookmarkæ¶ï¼æ¥åuser - ç¤ºä¾ï¼/pixivbot schedle
-random_bookmark 01:00*x - ç¤ºä¾ï¼/pixivbot schedle random_bookmark 01:00*x --
-user 114514 - \
->ä¸ºrandom_illustæ¶ï¼æ¥åwordï¼å¿éï¼ - ç¤ºä¾ï¼/pixivbot schedle
-random_illust "0 */2 * * * *" --word ã­ãª - ç¤ºä¾ï¼/pixivbot schedle
-random_illust "0 */2 * * * *" --word "Hatsune Miku" - \
->ä¸ºrandom_user_illustæ¶ï¼æ¥åuserï¼å¿éï¼ - ç¤ºä¾ï¼/pixivbot schedle
-random_user_illust 01:00*x --user æ£®åå - \
+>ï¼æä¸ç§æ ¼å¼ï¼*00:30\*x*ä¸ºæ¯é30åéè¿è¡ä¸æ¬¡æ¨éï¼*12:
+00*ä¸ºæ¯å¤©12:00è¿è¡ä¸æ¬¡æ¨éï¼*00:10+00:30\*x*ä¸ºä»ä»å¤©00:
+10å¼å§æ¯é30åéè¿è¡ä¸æ¬¡æ¨éï¼å¼å§æ¶é´è¥æ¯ä¸ä¸ªè¿å»çæ¶é´ç¹ï¼åä»ä¸ä¸ä¸ªå¼å§æ¨éçæ¶é´ç¹è¿è¡æ¨éï¼
+- [..args]ï¼ - \
+>ä¸ºrankingæ¶ï¼æ¥å\
+> \
+> - ç¤ºä¾ï¼/pixivbot schedle ranking 12:00 day 1-10 - \
+>ä¸ºrandom_bookmarkæ¶ï¼æ¥å\
+>ï¼å¯ç©ºï¼ - ç¤ºä¾ï¼/pixivbot schedle random_bookmark 01:00*x - ç¤ºä¾ï¼/
+pixivbot schedle random_bookmark 01:00*x 114514 - \
+>ä¸ºrandom_illustæ¶ï¼æ¥å\
+>ï¼è¥éè¦è¾å¥ç©ºæ ¼è¯·ç¨åææ `\ ` - ç¤ºä¾ï¼/pixivbot schedle
+random_illust 01:00*x - ç¤ºä¾ï¼/pixivbot schedle random_illust 01:00*x ã­ãª
+- ç¤ºä¾ï¼/pixivbot schedle random_illust 01:00*x Hatsune\ Miku - \
+>ä¸ºrandom_user_illustæ¶ï¼æ¥å\
+> - ç¤ºä¾ï¼/pixivbot schedle random_user_illust 01:00*x æ£®åå - \
 >ä¸ºrandom_recommend_illustæ¶ï¼ä¸æ¥ååæ° - **/pixivbot
 schedule**ï¼æ¥çæ¬ç¾¤ï¼æ¬ç¨æ·ï¼çææå®æ¶æ¨éè®¢é - **/
 pixivbot unschedule \
 >**ï¼åæ¶æ¬ç¾¤ï¼æ¬ç¨æ·ï¼çæå®çå®æ¶æ¨éè®¢é - **/pixivbot
 watch \
 > [..args]**ï¼ä¸ºæ¬ç¾¤ï¼æ¬ç¨æ·ï¼è®¢éç±»åä¸ºçæ´æ°æ¨éåè½ - \
 >ï¼å¯éå¼æuser_illusts, following_illusts - [..args]ï¼ - \
->ä¸ºuser_illustsæ¶ï¼æ¥åuserï¼å¿éï¼ - ç¤ºä¾ï¼/pixivbot watch
-user_illusts --user æ£®åå - \
->ä¸ºfollowing_illustsæ¶ï¼æ¥åuser - ç¤ºä¾ï¼/pixivbot watch
-following_illusts - ç¤ºä¾ï¼/pixivbot watch following_illusts --user 114514 -
-**/pixivbot watch**ï¼æ¥çæ¬ç¾¤ï¼æ¬ç¨æ·ï¼çæææ´æ°æ¨éè®¢é -
-**/pixivbot watch fetch \
+>ä¸ºuser_illustsæ¶ï¼æ¥å\
+> - ç¤ºä¾ï¼/pixivbot watch user_illusts æ£®åå - \
+>ä¸ºfollowing_illustsæ¶ï¼æ¥å\
+>ï¼å¯ç©ºï¼ - ç¤ºä¾ï¼/pixivbot watch following_illusts - ç¤ºä¾ï¼/pixivbot
+watch following_illusts 114514 - **/pixivbot
+watch**ï¼æ¥çæ¬ç¾¤ï¼æ¬ç¨æ·ï¼çæææ´æ°æ¨éè®¢é - **/pixivbot
+watch fetch \
 >**ï¼ãè°è¯ç¨å½ä»¤ãç«å»æå¨è§¦åä¸æ¬¡æå®çæ´æ°æ¨éè®¢é
 - **/pixivbot unwatch \
 > [..args]**ï¼åæ¶æ¬ç¾¤ï¼æ¬ç¨æ·ï¼çæå®çæ´æ°æ¨éè®¢é - **/
 pixivbot bind \
 >**ï¼ç»å®Pixivè´¦å·ï¼ç¨äºéæºä¹¦ç­¾åè½ï¼ - **/pixivbot
 unbind**ï¼è§£ç»Pixivè´¦å· - **/pixivbot
 invalidate_cache**ï¼æ¸é¤ç¼å­ï¼åªæè¶çº§ç¨æ·è½å¤åéæ­¤å½ä»¤ï¼
@@ -89,29 +78,34 @@
 éç½®å¤é¨æ°æ®åºï¼å¯éï¼
 PixivBotéè¦ä½¿ç¨æ°æ®åºå­æ¾è®¢éä»¥åç¼å­ï¼é»è®¤ä½¿ç¨SQLiteã
 ### SQLite
 è¥éè¦èªå®ä¹SQLiteæ°æ®åºæä»¶è·¯å¾ï¼è¯·è®¾ç½®éç½®é¡¹ï¼ -
 pixiv_sql_conn_url=`sqlite+aiosqlite:///<æ°æ®åºæä»¶è·¯å¾>` ### PostgreSQL
 è¥éè¦ä½¿ç¨PostgreSQLï¼è¯·è®¾ç½®éç½®é¡¹ï¼ -
 pixiv_sql_conn_url=`postgresql+asyncpg://<ç¨æ·å>:<å¯ç >@<ä¸»æº>:
-<ç«¯å£>/<æ°æ®åºå>` å¹¶ä¸å®è£`nonebot-plugin-pixivbot[postgresql]` ##
-æéæ§å¶ æä»¶æ¥å¥äº[nonebot-plugin-access-control](https://github.com/
-ssttkkl/nonebot-plugin-access-control)å®ç°ç»ç²åº¦çæéæ§å¶ï¼ ```
-nonebot_plugin_pixivbot âââ common â âââ illust ï¼ççå¾ï¼
-â âââ ranking ï¼ççæ¦ï¼ â âââ more ï¼è¿è¦ï¼ â
-âââ random_bookmark ï¼æ¥å¼ ç§å®¶è½¦ï¼ â âââ random_illust
-ï¼æ¥å¼ xxå¾ï¼ â âââ random_recommended_illust ï¼æ¥å¼ å¾ï¼ â
-âââ random_related_illust ï¼ä¸å¤è²ï¼ â âââ
-random_user_illust ï¼æ¥å¼ xxèå¸çå¾ï¼ âââ illust_link
-ï¼Pç«é¾æ¥åæ¢ï¼ âââ schedule â âââ receive
-ï¼æ¥æ¶å®æ¶æ¨éï¼ â âââ manage ï¼ç®¡çå®æ¶æ¨éï¼
-âââ watch â âââ receive ï¼æ¥æ¶æ´æ°æ¨éï¼ â âââ
-manage ï¼ç®¡çå®æ¶æ¨éï¼ âââ invalidate_cache ï¼æ¸é¤ç¼å­ï¼
-âââ bind ï¼ç»å®Pç«è´¦å·ï¼ âââ help ï¼å¸®å©ææ¬ï¼
-âââ r18 ï¼æ¾ç¤ºR-18åå®¹ï¼ âââ g ï¼æ¾ç¤ºR-18Gåå®¹ï¼ ```
+<ç«¯å£>/<æ°æ®åºå>` å¹¶ä¸å®è£`nonebot-plugin-pixivbot[postgresql]` ###
+MongoDB è¥éè¦ä½¿ç¨MongoDBï¼è¯·è®¾ç½®éç½®é¡¹ï¼ -
+pixiv_mongo_conn_url=`mongodb://<ç¨æ·å>:<å¯ç >@<ä¸»æº>:<ç«¯å£>/
+<ç¨æ·æå±çæ°æ®åº>` -
+pixiv_mongo_database_name=`è¿æ¥çMongoDBæ°æ®åº` å¹¶ä¸å®è£`nonebot-
+plugin-pixivbot[mongo]` ## æéæ§å¶ æä»¶æ¥å¥äº[nonebot-plugin-access-
+control](https://github.com/ssttkkl/nonebot-plugin-access-
+control)å®ç°ç»ç²åº¦çæéæ§å¶ï¼ ``` nonebot_plugin_pixivbot âââ
+common â âââ illust ï¼ççå¾ï¼ â âââ ranking
+ï¼ççæ¦ï¼ â âââ more ï¼è¿è¦ï¼ â âââ random_bookmark
+ï¼æ¥å¼ ç§å®¶è½¦ï¼ â âââ random_illust ï¼æ¥å¼ xxå¾ï¼ â
+âââ random_recommended_illust ï¼æ¥å¼ å¾ï¼ â âââ
+random_related_illust ï¼ä¸å¤è²ï¼ â âââ random_user_illust
+ï¼æ¥å¼ xxèå¸çå¾ï¼ âââ illust_link ï¼Pç«é¾æ¥åæ¢ï¼
+âââ schedule â âââ receive ï¼æ¥æ¶å®æ¶æ¨éï¼ â âââ
+manage ï¼ç®¡çå®æ¶æ¨éï¼ âââ watch â âââ receive
+ï¼æ¥æ¶æ´æ°æ¨éï¼ â âââ manage ï¼ç®¡çå®æ¶æ¨éï¼
+âââ invalidate_cache ï¼æ¸é¤ç¼å­ï¼ âââ bind
+ï¼ç»å®Pç«è´¦å·ï¼ âââ help ï¼å¸®å©ææ¬ï¼ âââ r18
+ï¼æ¾ç¤ºR-18åå®¹ï¼ âââ g ï¼æ¾ç¤ºR-18Gåå®¹ï¼ ```
 è­¬å¦ï¼è¶çº§ç¨æ·å¯ä»¥éè¿åé`/ac permission deny --srv
 nonebot_plugin_pixivbot.r18 --sbj all`å¨å±æ¦æªR-18ã
 åè­¬å¦ï¼è¶çº§ç¨æ·å¯ä»¥éè¿åå«åéä»¥ä¸æä»¤ï¼ä½¿å¾åªæè¶çº§ç¨æ·ãQQç§èä¸QQç¾¤èçç¾¤ç®¡çè½å¤è°ç¨`/
 pixivbot schedule`ä¸`/pixivbot unschedule`å½ä»¤ã ``` /ac permission deny --
 srv nonebot_plugin_pixivbot.schedule.manage --sbj all /ac permission allow --
 srv nonebot_plugin_pixivbot.schedule.manage --sbj qq:private /ac permission
 allow --srv nonebot_plugin_pixivbot.schedule.manage --sbj qq:group_admin /ac
@@ -136,20 +130,23 @@
 ### åé¨éè¯¯ï¼
 sqlalchemy.exc.OperationalError'>(sqlite3.OperationalError) near "ON": syntax
 error å¤åæ¯SQLiteçæ¬è¿ä½ï¼ä¸æ¯æON
 CONFLICTå­å¥ï¼å¦ææ¯Linuxç³»ç»è¯·æ´æ°å®è£çSQLiteçæ¬ ##
 éç½®é¡¹ä¸è§ æå°éç½®ï¼ ``` pixiv_refresh_token= #
 åé¢è·åçREFRESH_TOKEN ```
 é¤æå°éç½®åºç°çéç½®é¡¹ä»¥å¤é½æ¯å¯éé¡¹ï¼ç»åºçæ¯é»è®¤å¼ï¼å»ºè®®åªå°èªå·±éè¦çé¡¹å å¥.env.prodæä»¶
-å®æ´éç½®ï¼ ``` # æ°æ®åºéç½® pixiv_sql_conn_url=sqlite+aiosqlite:///
-pixiv_bot.db #
+å®æ´éç½®ï¼ ``` # æ°æ®åºéç½® pixiv_data_source= #
+ä½¿ç¨çæ°æ®åºç±»åï¼å¯éå¼ï¼sqlï¼mongoãè¥æªè®¾ç½®ï¼åæ ¹æ®æ¯å¦è®¾ç½®äºpixiv_mongo_conn_urlèªå¨å¤æ­ã
+pixiv_sql_conn_url=sqlite+aiosqlite:///pixiv_bot.db #
 SQLè¿æ¥URLï¼ä»æ¯æSQLiteä¸PostgreSQLï¼éè¿SQLAlchemyè¿è¡è¿æ¥ï¼å¿é¡»ä½¿ç¨å¼æ­¥çDBAPIï¼
-pixiv_use_local_cache=True # æ¯å¦å¯ç¨æ¬å°ç¼å­ # è¿æ¥éç½®
-pixiv_refresh_token= # åé¢è·åçREFRESH_TOKEN pixiv_proxy= #
-ä»£çURLï¼æ¨èä½¿ç¨socks5ä»£ç pixiv_query_timeout=60 #
+pixiv_mongo_conn_url= # MongoDBè¿æ¥URLï¼æ ¼å¼ï¼mongodb://<ç¨æ·å>:
+<å¯ç >@<ä¸»æº>:<ç«¯å£>/<æ°æ®åº>ã pixiv_mongo_database_name= #
+è¿æ¥çMongoDBæ°æ®åº pixiv_use_local_cache=True # æ¯å¦å¯ç¨æ¬å°ç¼å­
+# è¿æ¥éç½® pixiv_refresh_token= # åé¢è·åçREFRESH_TOKEN pixiv_proxy=
+# ä»£çURLï¼æ¨èä½¿ç¨socks5ä»£ç pixiv_query_timeout=60 #
 æ¥è¯¢è¶æ¶ï¼åä½ï¼ç§ï¼ pixiv_loading_prompt_delayed_time=5 #
 å è½½æç¤ºæ¶æ¯çå»¶è¿æ¶é´ï¼âåªåå è½½ä¸­âçæ¶æ¯ä¼å¨è¯·æ±ååºå¤å°ç§åååºï¼ï¼åä½ï¼ç§ï¼
 pixiv_simultaneous_query=8 # åPixivæ¥è¯¢çå¹¶åæ°
 pixiv_download_custom_domain= # ä½¿ç¨ååä»£çä¸è½½æç»çåå #
 æ¥è¯¢è®¾ç½® pixiv_query_to_me_only=False # åªååºå³äºBotçæ¥è¯¢
 pixiv_command_to_me_only=False # åªååºå³äºBotçå½ä»¤
 pixiv_max_item_per_query=10 # æ¯ä¸ªæ¥è¯¢æå¤è¯·æ±çæç»æ°é
@@ -177,17 +174,17 @@
 pixiv_user_illusts_cache_delete_in=2592000
 pixiv_user_bookmarks_cache_expires_in=86400
 pixiv_user_bookmarks_cache_delete_in=2592000
 pixiv_related_illusts_cache_expires_in=86400 pixiv_other_cache_expires_in=21600
 # QQå¹³å°ï¼ä¸»è¦æ¯gocqï¼éç½® pixiv_poke_action=random_recommended_illust
 # ååºæ³ä¸æ³å¨ä½ï¼å¯éå¼ï¼ranking, random_recommended_illust,
 random_bookmark, ä»ä¹é½ä¸å¡«å³å¿½ç¥æ³ä¸æ³å¨ä½
-pixiv_send_illust_with_link=False #
+pixiv_onebot_with_link=False #
 åå¾æ¶æ¯å¦å¸¦ä¸é¾æ¥ï¼å®¹æè¢«txç¯ä¸ï¼
-pixiv_send_forward_message=auto #
+pixiv_onebot_send_forward_message=auto #
 åå¾æ¶æ¯å¦ä½¿ç¨è½¬åæ¶æ¯çå½¢å¼ï¼å¯éå¼ï¼always(æ°¸è¿ä½¿ç¨),
 auto(ä»å¨å¤å¼ å¾çæ¶ä½¿ç¨), never(æ°¸è¿ä¸ä½¿ç¨) # åè½éç½®
 pixiv_more_enabled=True # å¯ç¨éå¤ä¸ä¸æ¬¡è¯·æ±ï¼è¿è¦ï¼åè½
 pixiv_query_expires_in=600 # ä¸ä¸æ¬¡è¯·æ±çè¿ææ¶é´ï¼åä½ï¼ç§ï¼
 pixiv_illust_query_enabled=True # å¯ç¨æç»æ¥è¯¢ï¼ççå¾ï¼åè½
 pixiv_ranking_query_enabled=True # å¯ç¨æ¦åæ¥è¯¢ï¼ççæ¦ï¼åè½
 pixiv_ranking_default_mode=day # é»è®¤æ¥è¯¢çæ¦åï¼å¯éå¼ï¼day, week,
```

