# Comparing `tmp/FicusFramework-3.1.0.tar.gz` & `tmp/FicusFramework-3.1.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/FicusFramework-3.1.0.tar", last modified: Tue Apr 18 02:40:39 2023, max compression
+gzip compressed data, was "dist/FicusFramework-3.1.0.post2.tar", last modified: Fri Jun 16 10:22:58 2023, max compression
```

## Comparing `FicusFramework-3.1.0.tar` & `FicusFramework-3.1.0.post2.tar`

### file list

```diff
@@ -1,293 +1,293 @@
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/
--rw-r--r--   0 sun        (501) wheel        (0)     2936 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/PKG-INFO
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/test/
--rw-r--r--   0 sun        (501) wheel        (0)     1535 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/test/test_factDatasourceChangeListener.py
--rw-r--r--   0 sun        (501) wheel        (0)     2748 2019-11-22 03:45:56.000000 FicusFramework-3.1.0/test/test_abstractSimpleScripCrawlTestSuite.py
--rw-r--r--   0 sun        (501) wheel        (0)      984 2019-08-02 08:53:21.000000 FicusFramework-3.1.0/test/test_utils.py
--rw-r--r--   0 sun        (501) wheel        (0)     1701 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/test/test_customerDaoContextHolder.py
--rw-r--r--   0 sun        (501) wheel        (0)     1765 2020-03-23 08:49:50.000000 FicusFramework-3.1.0/test/test_cryptography.py
--rw-r--r--   0 sun        (501) wheel        (0)     1192 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/test/test_distributedFactDatasourceProxy.py
--rw-r--r--   0 sun        (501) wheel        (0)     3242 2022-10-13 03:25:59.000000 FicusFramework-3.1.0/test/test_abstractBatchCETestSuite.py
--rw-r--r--   0 sun        (501) wheel        (0)     1302 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/test/test_factDatasourceService.py
--rw-r--r--   0 sun        (501) wheel        (0)     3280 2022-10-13 03:25:59.000000 FicusFramework-3.1.0/test/test_abstractSimpleScriptCETestSuite.py
--rw-r--r--   0 sun        (501) wheel        (0)     2742 2019-11-22 03:45:56.000000 FicusFramework-3.1.0/test/test_abstractSimpleCrawlTestSuite.py
--rw-r--r--   0 sun        (501) wheel        (0)     2926 2019-11-22 03:45:56.000000 FicusFramework-3.1.0/test/test_abstractBatchCrawlTestSuite.py
--rw-r--r--   0 sun        (501) wheel        (0)     1263 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/setup.py
--rw-r--r--   0 sun        (501) wheel        (0)      100 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/setup.cfg
--rw-r--r--   0 sun        (501) wheel        (0)     2346 2018-06-15 02:07:44.000000 FicusFramework-3.1.0/README.rst
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/init/
--rw-r--r--   0 sun        (501) wheel        (0)        0 2020-10-27 11:51:51.000000 FicusFramework-3.1.0/src/init/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)     5199 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/init/app.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/schedule/
--rw-r--r--   0 sun        (501) wheel        (0)     3436 2020-12-11 02:26:37.000000 FicusFramework-3.1.0/src/schedule/TaskThreadHolder.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/schedule/test/
--rw-r--r--   0 sun        (501) wheel        (0)       88 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/schedule/test/__init__.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/schedule/test/suite/
--rw-r--r--   0 sun        (501) wheel        (0)    14543 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/schedule/test/suite/crawl.py
--rw-r--r--   0 sun        (501) wheel        (0)     6427 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/schedule/test/suite/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)    10984 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/schedule/test/suite/ce.py
--rw-r--r--   0 sun        (501) wheel        (0)       28 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/schedule/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)    16977 2021-07-22 02:54:07.000000 FicusFramework-3.1.0/src/schedule/TaskThread.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/schedule/utils/
--rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/schedule/utils/__init__.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/schedule/utils/log/
--rw-r--r--   0 sun        (501) wheel        (0)     4438 2020-08-18 09:18:52.000000 FicusFramework-3.1.0/src/schedule/utils/log/TaskLogFileAppender.py
--rw-r--r--   0 sun        (501) wheel        (0)     2428 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/schedule/utils/log/TaskLogCleanScheduler.py
--rw-r--r--   0 sun        (501) wheel        (0)     2284 2019-11-22 03:45:56.000000 FicusFramework-3.1.0/src/schedule/utils/log/TaskLogger.py
--rw-r--r--   0 sun        (501) wheel        (0)     2981 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/schedule/utils/log/FrameworkHandlerLogger.py
--rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/schedule/utils/log/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)     4190 2021-05-08 09:50:08.000000 FicusFramework-3.1.0/src/schedule/TriggerActor.py
--rw-r--r--   0 sun        (501) wheel        (0)      484 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/schedule/ShardContext.py
--rw-r--r--   0 sun        (501) wheel        (0)      245 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/schedule/TaskHandlerContext.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/cloudcelery/
--rw-r--r--   0 sun        (501) wheel        (0)     4930 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/cloudcelery/CeleryOnRequest.py
--rw-r--r--   0 sun        (501) wheel        (0)     4780 2023-01-06 10:44:05.000000 FicusFramework-3.1.0/src/cloudcelery/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)     1096 2021-07-22 02:42:02.000000 FicusFramework-3.1.0/src/cloudcelery/celery_config.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/config/
--rw-r--r--   0 sun        (501) wheel        (0)    10997 2021-07-16 06:13:02.000000 FicusFramework-3.1.0/src/config/BootstrapPropertyLoader.py
--rw-r--r--   0 sun        (501) wheel        (0)     4953 2023-03-16 07:22:14.000000 FicusFramework-3.1.0/src/config/annotation.py
--rw-r--r--   0 sun        (501) wheel        (0)     2302 2021-07-16 06:12:10.000000 FicusFramework-3.1.0/src/config/__init__.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/discovery/
--rw-r--r--   0 sun        (501) wheel        (0)    14413 2021-07-07 07:23:16.000000 FicusFramework-3.1.0/src/discovery/__init__.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/
--rw-r--r--   0 sun        (501) wheel        (0)    33598 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/factdatasource/FactDatasourceProxyService.py
--rw-r--r--   0 sun        (501) wheel        (0)    12673 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/factdatasource/FactDatasourceContextHolder.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/transformer/
--rw-r--r--   0 sun        (501) wheel        (0)      718 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/transformer/ChineseToNumberTransformer.py
--rw-r--r--   0 sun        (501) wheel        (0)     2338 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/transformer/TransformerContext.py
--rw-r--r--   0 sun        (501) wheel        (0)      762 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/transformer/ITransformer.py
--rw-r--r--   0 sun        (501) wheel        (0)      579 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/transformer/CompleteGB32100Transformer.py
--rw-r--r--   0 sun        (501) wheel        (0)        0 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/transformer/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)     1001 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/transformer/FixItemTransformer.py
--rw-r--r--   0 sun        (501) wheel        (0)      991 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/transformer/ParseDateTimeTransformer.py
--rw-r--r--   0 sun        (501) wheel        (0)     3749 2021-03-25 11:30:40.000000 FicusFramework-3.1.0/src/factdatasource/transformer/DefaultValueTransformer.py
--rw-r--r--   0 sun        (501) wheel        (0)      881 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/transformer/CompleteStringTransformer.py
--rw-r--r--   0 sun        (501) wheel        (0)      900 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/transformer/NumberToChineseTransformer.py
--rw-r--r--   0 sun        (501) wheel        (0)    34157 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/factdatasource/FactDatasourceProxyServiceV2.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/dao/
--rw-r--r--   0 sun        (501) wheel        (0)     2095 2022-11-15 06:30:54.000000 FicusFramework-3.1.0/src/factdatasource/dao/MultipleDatasourceHolder.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/dao/redis/
--rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/redis/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)      643 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/redis/RedisDatasourceDao.py
--rw-r--r--   0 sun        (501) wheel        (0)     7237 2021-12-10 03:38:55.000000 FicusFramework-3.1.0/src/factdatasource/dao/redis/MultipleRedisDatasource.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/dao/graph/
--rw-r--r--   0 sun        (501) wheel        (0)     8390 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/graph/GraphDatasourceDao.py
--rw-r--r--   0 sun        (501) wheel        (0)     1093 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/graph/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/__init__.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/dao/amqp/
--rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/amqp/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)     5310 2021-12-10 03:28:59.000000 FicusFramework-3.1.0/src/factdatasource/dao/amqp/MultipleAmqpDatasource.py
--rw-r--r--   0 sun        (501) wheel        (0)     1778 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/amqp/AmqpDatasourceDao.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/dao/jdbc/
--rw-r--r--   0 sun        (501) wheel        (0)     3174 2020-09-28 06:27:10.000000 FicusFramework-3.1.0/src/factdatasource/dao/jdbc/JdbcDatasourceDao.py
--rw-r--r--   0 sun        (501) wheel        (0)    12694 2021-12-10 03:36:30.000000 FicusFramework-3.1.0/src/factdatasource/dao/jdbc/MultipleJdbcDatasource.py
--rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/jdbc/__init__.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/dao/kafka/
--rw-r--r--   0 sun        (501) wheel        (0)     5501 2020-09-28 07:42:31.000000 FicusFramework-3.1.0/src/factdatasource/dao/kafka/MultipleKafkaDatasource.py
--rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/kafka/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)      926 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/kafka/KafkaDatasourceDao.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/dao/stomp/
--rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/stomp/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)     5132 2020-09-28 07:42:31.000000 FicusFramework-3.1.0/src/factdatasource/dao/stomp/MultipleStompDatasource.py
--rw-r--r--   0 sun        (501) wheel        (0)     1035 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/stomp/StompDatasourceDao.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/dao/tablestore/
--rw-r--r--   0 sun        (501) wheel        (0)       88 2022-11-15 06:30:54.000000 FicusFramework-3.1.0/src/factdatasource/dao/tablestore/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)     5137 2022-11-15 06:30:54.000000 FicusFramework-3.1.0/src/factdatasource/dao/tablestore/MultipleTableStoreDatasource.py
--rw-r--r--   0 sun        (501) wheel        (0)      564 2022-11-15 06:30:54.000000 FicusFramework-3.1.0/src/factdatasource/dao/tablestore/TableStoreDatasourceDao.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/dao/mongo/
--rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/mongo/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)     3567 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/mongo/MongoDatasourceDao.py
--rw-r--r--   0 sun        (501) wheel        (0)     5894 2021-12-10 03:37:48.000000 FicusFramework-3.1.0/src/factdatasource/dao/mongo/MultipleMongoDatasource.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/dao/es/
--rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/es/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)     3287 2020-06-17 11:00:50.000000 FicusFramework-3.1.0/src/factdatasource/dao/es/EsDatasourceDao.py
--rw-r--r--   0 sun        (501) wheel        (0)     4484 2020-09-28 07:42:31.000000 FicusFramework-3.1.0/src/factdatasource/dao/es/MultipleEsDatasource.py
--rw-r--r--   0 sun        (501) wheel        (0)     4600 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/dao/FactDatasource.py
--rw-r--r--   0 sun        (501) wheel        (0)     1603 2020-09-28 07:42:31.000000 FicusFramework-3.1.0/src/factdatasource/__init__.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/message/
--rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/message/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)    10913 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/factdatasource/message/FactDatasourceMessageHanlder.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/file/
--rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/file/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)     3186 2020-03-23 08:49:50.000000 FicusFramework-3.1.0/src/factdatasource/persistence/file/FileFactDatasourceContext.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/redis/
--rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/redis/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)    12650 2020-12-09 07:31:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/redis/RedisFactDatasourceContext.py
--rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/__init__.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/amqp/
--rw-r--r--   0 sun        (501) wheel        (0)     5276 2020-12-09 07:28:30.000000 FicusFramework-3.1.0/src/factdatasource/persistence/amqp/AmqpFactDatasourceContext.py
--rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/amqp/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)    12086 2020-12-09 07:23:42.000000 FicusFramework-3.1.0/src/factdatasource/persistence/AbstractFactDatasourceContext.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/algorithm/
--rw-r--r--   0 sun        (501) wheel        (0)        0 2020-07-27 11:07:37.000000 FicusFramework-3.1.0/src/factdatasource/persistence/algorithm/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)     8030 2020-07-27 11:07:37.000000 FicusFramework-3.1.0/src/factdatasource/persistence/algorithm/AlgorithmFactDatasourceContext.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/
--rw-r--r--   0 sun        (501) wheel        (0)      534 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)    15075 2020-12-09 07:29:32.000000 FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/JdbcFactDatasourceContext.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/
--rw-r--r--   0 sun        (501) wheel        (0)      740 2021-02-03 08:54:08.000000 FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/VernoxntsJdbcFactDatasourceContext.py
--rw-r--r--   0 sun        (501) wheel        (0)     3436 2020-12-09 07:30:40.000000 FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/PostgresqlJdbcFactDatasourceContext.py
--rw-r--r--   0 sun        (501) wheel        (0)     3703 2020-12-09 07:30:49.000000 FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/SqlserverJdbcFactDatasourceContext.py
--rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)      532 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/Db2JdbcFactDatasourceContext.py
--rw-r--r--   0 sun        (501) wheel        (0)     3801 2020-12-09 07:30:13.000000 FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/OracleJdbcFactDatasourceContext.py
--rw-r--r--   0 sun        (501) wheel        (0)      283 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/VernoxJdbcFactDatasourceContext.py
--rw-r--r--   0 sun        (501) wheel        (0)     3291 2020-12-09 07:29:54.000000 FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/MysqlJdbcFactDatasourceContext.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/kafka/
--rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/kafka/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)     5513 2021-01-27 02:59:31.000000 FicusFramework-3.1.0/src/factdatasource/persistence/kafka/KafkaFactDatasourceContext.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/stomp/
--rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/stomp/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)     5325 2020-12-09 07:31:55.000000 FicusFramework-3.1.0/src/factdatasource/persistence/stomp/StompFactDatasourceContext.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/tablestore/
--rw-r--r--   0 sun        (501) wheel        (0)       88 2022-11-15 06:30:54.000000 FicusFramework-3.1.0/src/factdatasource/persistence/tablestore/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)    29851 2022-11-15 06:30:54.000000 FicusFramework-3.1.0/src/factdatasource/persistence/tablestore/TableStoreDatasourceContext.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/mongo/
--rw-r--r--   0 sun        (501) wheel        (0)    13093 2021-05-18 02:18:14.000000 FicusFramework-3.1.0/src/factdatasource/persistence/mongo/MongoFactDatasourceContext.py
--rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/mongo/__init__.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/sobeyhive/
--rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/sobeyhive/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)    15917 2020-12-09 07:31:49.000000 FicusFramework-3.1.0/src/factdatasource/persistence/sobeyhive/SobeyHiveFactDatasourceContext.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/es/
--rw-r--r--   0 sun        (501) wheel        (0)    14150 2020-12-09 07:29:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/es/EsFactDatasourceContext.py
--rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/es/__init__.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/custom/
--rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/custom/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)     2913 2020-03-23 08:49:50.000000 FicusFramework-3.1.0/src/factdatasource/persistence/custom/CustomFactDatasourceContext.py
--rw-r--r--   0 sun        (501) wheel        (0)     6093 2020-03-23 08:49:50.000000 FicusFramework-3.1.0/src/factdatasource/persistence/SqlableDeleteCondition.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/factdatasource/persistence/graphdb/
--rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/persistence/graphdb/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)    11260 2020-12-09 07:29:19.000000 FicusFramework-3.1.0/src/factdatasource/persistence/graphdb/GraphdbFactDatasourceContext.py
--rw-r--r--   0 sun        (501) wheel        (0)     4175 2020-03-23 08:49:50.000000 FicusFramework-3.1.0/src/factdatasource/FactDatasourceContext.py
--rw-r--r--   0 sun        (501) wheel        (0)      609 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/factdatasource/execptions.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/libs/
--rw-r--r--   0 sun        (501) wheel        (0)     1008 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/libs/HeaderHolder.py
--rw-r--r--   0 sun        (501) wheel        (0)       89 2023-04-14 11:35:27.000000 FicusFramework-3.1.0/src/libs/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)     6659 2021-02-03 08:54:08.000000 FicusFramework-3.1.0/src/libs/utils.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/py_eureka_client/
--rw-r--r--   0 sun        (501) wheel        (0)     3118 2020-06-15 12:21:33.000000 FicusFramework-3.1.0/src/py_eureka_client/__urlopen_proxy__.py
--rw-r--r--   0 sun        (501) wheel        (0)     4398 2020-06-15 12:21:33.000000 FicusFramework-3.1.0/src/py_eureka_client/http_client.py
--rw-r--r--   0 sun        (501) wheel        (0)       25 2020-06-15 12:21:33.000000 FicusFramework-3.1.0/src/py_eureka_client/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)    52699 2021-07-07 06:44:45.000000 FicusFramework-3.1.0/src/py_eureka_client/eureka_client.py
--rw-r--r--   0 sun        (501) wheel        (0)      951 2020-06-15 12:21:33.000000 FicusFramework-3.1.0/src/py_eureka_client/__logger__.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/registry/
--rw-r--r--   0 sun        (501) wheel        (0)    12773 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/registry/LoadOnRegistryLoader.py
--rw-r--r--   0 sun        (501) wheel        (0)     7749 2020-09-28 06:27:10.000000 FicusFramework-3.1.0/src/registry/LoadOnAlgorithmLoader.py
--rw-r--r--   0 sun        (501) wheel        (0)     2681 2020-07-20 06:12:53.000000 FicusFramework-3.1.0/src/registry/__init__.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/api/
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/api/handler/
--rw-r--r--   0 sun        (501) wheel        (0)      114 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/api/handler/IKillable.py
--rw-r--r--   0 sun        (501) wheel        (0)     6935 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/handler/ICacheAbleHandler.py
--rw-r--r--   0 sun        (501) wheel        (0)      160 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/api/handler/IHandler.py
--rw-r--r--   0 sun        (501) wheel        (0)      530 2019-12-13 09:21:10.000000 FicusFramework-3.1.0/src/api/handler/IProgressAble.py
--rw-r--r--   0 sun        (501) wheel        (0)       77 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/api/handler/__init__.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/api/handler/message/
--rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/handler/message/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)     1075 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/api/handler/message/IMessageHandler.py
--rw-r--r--   0 sun        (501) wheel        (0)     1039 2021-05-28 02:02:59.000000 FicusFramework-3.1.0/src/api/handler/ITaskHandler.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/api/handler/script/
--rw-r--r--   0 sun        (501) wheel        (0)      134 2019-12-13 09:21:10.000000 FicusFramework-3.1.0/src/api/handler/script/ScriptHandlerHolder.py
--rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/handler/script/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)     3686 2023-03-16 07:29:04.000000 FicusFramework-3.1.0/src/api/handler/script/ScriptPythonFactory.py
--rw-r--r--   0 sun        (501) wheel        (0)     1759 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/handler/script/ICacheAbleScript.py
--rw-r--r--   0 sun        (501) wheel        (0)    11195 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/handler/script/ScriptPythonTaskHandler.py
--rw-r--r--   0 sun        (501) wheel        (0)      301 2019-12-13 09:21:10.000000 FicusFramework-3.1.0/src/api/handler/script/IProgressAbleScript.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/api/handler/crawl/
--rw-r--r--   0 sun        (501) wheel        (0)      638 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/handler/crawl/ISampleScriptCrawl.py
--rw-r--r--   0 sun        (501) wheel        (0)     6190 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/handler/crawl/AbstractBatchCrawl.py
--rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/handler/crawl/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)     5522 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/handler/crawl/AbstractSimpleCrawl.py
--rw-r--r--   0 sun        (501) wheel        (0)      937 2021-05-28 02:29:13.000000 FicusFramework-3.1.0/src/api/handler/crawl/ISimpleScriptCrawl.py
--rw-r--r--   0 sun        (501) wheel        (0)      428 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/handler/ILogAbleHandler.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/api/handler/outputer/
--rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/handler/outputer/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)      923 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/handler/outputer/ISimpleOutputer.py
--rw-r--r--   0 sun        (501) wheel        (0)     3929 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/handler/outputer/IBatchOutputer.py
--rw-r--r--   0 sun        (501) wheel        (0)     5490 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/handler/outputer/IBaseOutputer.py
--rw-r--r--   0 sun        (501) wheel        (0)      199 2021-05-28 02:09:19.000000 FicusFramework-3.1.0/src/api/handler/IRevoke.py
--rw-r--r--   0 sun        (501) wheel        (0)     1203 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/handler/ICacheAble.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/api/handler/ce/
--rw-r--r--   0 sun        (501) wheel        (0)     7827 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/handler/ce/IMessageCE.py
--rw-r--r--   0 sun        (501) wheel        (0)    13379 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/handler/ce/AbstractAsyncServiceBatchCE.py
--rw-r--r--   0 sun        (501) wheel        (0)     6467 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/handler/ce/AbstractBatchCE.py
--rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/handler/ce/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)      765 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/handler/ce/ISampleScriptCE.py
--rw-r--r--   0 sun        (501) wheel        (0)     1094 2021-05-28 02:28:47.000000 FicusFramework-3.1.0/src/api/handler/ce/ISimpleScriptCE.py
--rw-r--r--   0 sun        (501) wheel        (0)     5919 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/handler/ce/AbstractMessageCE.py
--rw-r--r--   0 sun        (501) wheel        (0)      421 2020-07-06 10:53:29.000000 FicusFramework-3.1.0/src/api/handler/IAsyncAble.py
--rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/__init__.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/api/annotation/
--rw-r--r--   0 sun        (501) wheel        (0)      396 2020-03-23 08:49:50.000000 FicusFramework-3.1.0/src/api/annotation/annotation.py
--rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/annotation/__init__.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/api/model/
--rw-r--r--   0 sun        (501) wheel        (0)     2026 2019-12-13 09:21:10.000000 FicusFramework-3.1.0/src/api/model/OutputWrapper.py
--rw-r--r--   0 sun        (501) wheel        (0)     1123 2020-07-06 10:53:29.000000 FicusFramework-3.1.0/src/api/model/AsyncServiceRequest.py
--rw-r--r--   0 sun        (501) wheel        (0)     3853 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/model/AlgorithmFdInputWrapper.py
--rw-r--r--   0 sun        (501) wheel        (0)     1182 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/model/GraphNode.py
--rw-r--r--   0 sun        (501) wheel        (0)     1128 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/model/ReadWriteLock.py
--rw-r--r--   0 sun        (501) wheel        (0)     2088 2021-01-27 02:59:31.000000 FicusFramework-3.1.0/src/api/model/MetaModel.py
--rw-r--r--   0 sun        (501) wheel        (0)      679 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/model/ResultVO.py
--rw-r--r--   0 sun        (501) wheel        (0)     1777 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/model/GraphRelation.py
--rw-r--r--   0 sun        (501) wheel        (0)      640 2020-07-06 10:53:29.000000 FicusFramework-3.1.0/src/api/model/AsyncServiceResponse.py
--rw-r--r--   0 sun        (501) wheel        (0)     1791 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/model/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)     3225 2019-12-13 09:21:10.000000 FicusFramework-3.1.0/src/api/model/BatchOutputPipe.py
--rw-r--r--   0 sun        (501) wheel        (0)     1879 2021-03-25 11:31:25.000000 FicusFramework-3.1.0/src/api/model/Page.py
--rw-r--r--   0 sun        (501) wheel        (0)      375 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/model/FactDatasourceQueryParameter.py
--rw-r--r--   0 sun        (501) wheel        (0)     1857 2021-03-25 10:50:10.000000 FicusFramework-3.1.0/src/api/model/MetaModelField.py
--rw-r--r--   0 sun        (501) wheel        (0)     2046 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/api/model/MetaModelTransform.py
--rw-r--r--   0 sun        (501) wheel        (0)      952 2020-03-23 08:49:50.000000 FicusFramework-3.1.0/src/api/model/Condition.py
--rw-r--r--   0 sun        (501) wheel        (0)      855 2020-07-27 11:07:37.000000 FicusFramework-3.1.0/src/api/model/AlgoOutWrapper.py
--rw-r--r--   0 sun        (501) wheel        (0)     1572 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/model/FdInputPipe.py
--rw-r--r--   0 sun        (501) wheel        (0)     6733 2019-02-27 06:21:54.000000 FicusFramework-3.1.0/src/api/model/OtherTargetOutputPipe.py
--rw-r--r--   0 sun        (501) wheel        (0)     4423 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/api/model/FdInputWrapper.py
--rw-r--r--   0 sun        (501) wheel        (0)     5501 2022-11-15 06:30:54.000000 FicusFramework-3.1.0/src/api/model/FactDatasource.py
--rw-r--r--   0 sun        (501) wheel        (0)      245 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/api/exceptions.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/rule_engine/
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/rule_engine/operation/
--rw-r--r--   0 sun        (501) wheel        (0)     4529 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/rule_engine/operation/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)    13749 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/rule_engine/RuleEngineInitialize.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/rule_engine/core/
--rw-r--r--   0 sun        (501) wheel        (0)     3330 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/rule_engine/core/SimpleValueProvider.py
--rw-r--r--   0 sun        (501) wheel        (0)     1201 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/rule_engine/core/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)     3576 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/rule_engine/core/SimpleRuleGroupSession.py
--rw-r--r--   0 sun        (501) wheel        (0)     2784 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/rule_engine/core/DefaultAgenda.py
--rw-r--r--   0 sun        (501) wheel        (0)     3489 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/rule_engine/core/PattenMatcher.py
--rw-r--r--   0 sun        (501) wheel        (0)     2061 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/rule_engine/RuleEngine.py
--rw-r--r--   0 sun        (501) wheel        (0)    11736 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/rule_engine/__init__.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/rule_engine/action/
--rw-r--r--   0 sun        (501) wheel        (0)     1347 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/rule_engine/action/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)     1678 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/rule_engine/RuleEngineCustomScriptFactory.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/service/
--rw-r--r--   0 sun        (501) wheel        (0)     1809 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/service/FactDatasourceService.py
--rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0/src/service/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)     2256 2020-04-29 11:49:46.000000 FicusFramework-3.1.0/src/service/TaskQueueService.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/FicusFramework.egg-info/
--rw-r--r--   0 sun        (501) wheel        (0)     2936 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/FicusFramework.egg-info/PKG-INFO
--rw-r--r--   0 sun        (501) wheel        (0)        1 2019-02-27 06:22:29.000000 FicusFramework-3.1.0/src/FicusFramework.egg-info/not-zip-safe
--rw-r--r--   0 sun        (501) wheel        (0)     9687 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/FicusFramework.egg-info/SOURCES.txt
--rw-r--r--   0 sun        (501) wheel        (0)      247 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/FicusFramework.egg-info/requires.txt
--rw-r--r--   0 sun        (501) wheel        (0)      127 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/FicusFramework.egg-info/top_level.txt
--rw-r--r--   0 sun        (501) wheel        (0)        1 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/FicusFramework.egg-info/dependency_links.txt
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/client/
--rw-r--r--   0 sun        (501) wheel        (0)     3234 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/client/ComputeExecutionClient.py
--rw-r--r--   0 sun        (501) wheel        (0)     1035 2020-09-28 07:42:31.000000 FicusFramework-3.1.0/src/client/FactDatasourceManageClient.py
--rw-r--r--   0 sun        (501) wheel        (0)     6946 2021-08-13 06:23:01.000000 FicusFramework-3.1.0/src/client/ScheduleJobTaskLogClient.py
--rw-r--r--   0 sun        (501) wheel        (0)     1173 2020-04-29 13:07:29.000000 FicusFramework-3.1.0/src/client/ScheduleCloudClient.py
--rw-r--r--   0 sun        (501) wheel        (0)     2158 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/client/HandlerLogClient.py
--rw-r--r--   0 sun        (501) wheel        (0)     1791 2021-06-04 07:35:30.000000 FicusFramework-3.1.0/src/client/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)     8802 2019-04-15 11:08:40.000000 FicusFramework-3.1.0/src/client/JobScheduleClient.py
--rw-r--r--   0 sun        (501) wheel        (0)     4296 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/client/DataCrawlClient.py
--rw-r--r--   0 sun        (501) wheel        (0)     3996 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/client/ClientAuth.py
--rw-r--r--   0 sun        (501) wheel        (0)     3815 2020-07-24 11:47:04.000000 FicusFramework-3.1.0/src/client/DataAlgorithmClient.py
--rw-r--r--   0 sun        (501) wheel        (0)     2850 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/client/AuthClient.py
--rw-r--r--   0 sun        (501) wheel        (0)     2254 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/client/FactDatasourceClient.py
--rw-r--r--   0 sun        (501) wheel        (0)     3905 2019-04-15 11:08:07.000000 FicusFramework-3.1.0/src/client/ScheduleCacheClient.py
-drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-04-18 02:40:39.000000 FicusFramework-3.1.0/src/remote/
--rw-r--r--   0 sun        (501) wheel        (0)     1453 2020-03-23 08:49:50.000000 FicusFramework-3.1.0/src/remote/TriggerRemoteActor.py
--rw-r--r--   0 sun        (501) wheel        (0)      591 2020-06-15 12:21:33.000000 FicusFramework-3.1.0/src/remote/__init__.py
--rw-r--r--   0 sun        (501) wheel        (0)      795 2020-03-24 09:55:45.000000 FicusFramework-3.1.0/src/remote/PrometheusMetricsRemoteService.py
--rw-r--r--   0 sun        (501) wheel        (0)      375 2023-04-18 02:39:13.000000 FicusFramework-3.1.0/src/remote/ActuatorRemote.py
--rw-r--r--   0 sun        (501) wheel        (0)      914 2019-06-25 08:47:51.000000 FicusFramework-3.1.0/src/remote/LogReadRemoteService.py
--rw-r--r--   0 sun        (501) wheel        (0)     7060 2020-12-11 02:26:37.000000 FicusFramework-3.1.0/src/remote/AsyncResponseRestService.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/
+-rw-r--r--   0 sun        (501) wheel        (0)     2978 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/PKG-INFO
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/test/
+-rw-r--r--   0 sun        (501) wheel        (0)     1535 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/test/test_factDatasourceChangeListener.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2748 2019-11-22 03:45:56.000000 FicusFramework-3.1.0.post2/test/test_abstractSimpleScripCrawlTestSuite.py
+-rw-r--r--   0 sun        (501) wheel        (0)      984 2023-04-24 03:54:23.000000 FicusFramework-3.1.0.post2/test/test_utils.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1701 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/test/test_customerDaoContextHolder.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1765 2020-03-23 08:49:50.000000 FicusFramework-3.1.0.post2/test/test_cryptography.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1192 2023-04-24 03:54:17.000000 FicusFramework-3.1.0.post2/test/test_distributedFactDatasourceProxy.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3242 2022-10-13 03:25:59.000000 FicusFramework-3.1.0.post2/test/test_abstractBatchCETestSuite.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1302 2023-04-24 03:54:17.000000 FicusFramework-3.1.0.post2/test/test_factDatasourceService.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3280 2022-10-13 03:25:59.000000 FicusFramework-3.1.0.post2/test/test_abstractSimpleScriptCETestSuite.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2742 2019-11-22 03:45:56.000000 FicusFramework-3.1.0.post2/test/test_abstractSimpleCrawlTestSuite.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2926 2019-11-22 03:45:56.000000 FicusFramework-3.1.0.post2/test/test_abstractBatchCrawlTestSuite.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1305 2023-06-16 10:22:56.000000 FicusFramework-3.1.0.post2/setup.py
+-rw-r--r--   0 sun        (501) wheel        (0)      100 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/setup.cfg
+-rw-r--r--   0 sun        (501) wheel        (0)     2346 2018-06-15 02:07:44.000000 FicusFramework-3.1.0.post2/README.rst
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/init/
+-rw-r--r--   0 sun        (501) wheel        (0)        0 2020-10-27 11:51:51.000000 FicusFramework-3.1.0.post2/src/init/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     5199 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/init/app.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/schedule/
+-rw-r--r--   0 sun        (501) wheel        (0)     3436 2020-12-11 02:26:37.000000 FicusFramework-3.1.0.post2/src/schedule/TaskThreadHolder.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/schedule/test/
+-rw-r--r--   0 sun        (501) wheel        (0)       88 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/schedule/test/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/schedule/test/suite/
+-rw-r--r--   0 sun        (501) wheel        (0)    14543 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/schedule/test/suite/crawl.py
+-rw-r--r--   0 sun        (501) wheel        (0)     6427 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/schedule/test/suite/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)    10984 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/schedule/test/suite/ce.py
+-rw-r--r--   0 sun        (501) wheel        (0)       28 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/schedule/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)    16977 2021-07-22 02:54:07.000000 FicusFramework-3.1.0.post2/src/schedule/TaskThread.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/schedule/utils/
+-rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/schedule/utils/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/schedule/utils/log/
+-rw-r--r--   0 sun        (501) wheel        (0)     4438 2020-08-18 09:18:52.000000 FicusFramework-3.1.0.post2/src/schedule/utils/log/TaskLogFileAppender.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2428 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/schedule/utils/log/TaskLogCleanScheduler.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2284 2019-11-22 03:45:56.000000 FicusFramework-3.1.0.post2/src/schedule/utils/log/TaskLogger.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2981 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/schedule/utils/log/FrameworkHandlerLogger.py
+-rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/schedule/utils/log/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     4190 2021-05-08 09:50:08.000000 FicusFramework-3.1.0.post2/src/schedule/TriggerActor.py
+-rw-r--r--   0 sun        (501) wheel        (0)      484 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/schedule/ShardContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)      245 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/schedule/TaskHandlerContext.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/cloudcelery/
+-rw-r--r--   0 sun        (501) wheel        (0)     4930 2023-05-22 07:56:37.000000 FicusFramework-3.1.0.post2/src/cloudcelery/CeleryOnRequest.py
+-rw-r--r--   0 sun        (501) wheel        (0)     4780 2023-05-26 08:36:10.000000 FicusFramework-3.1.0.post2/src/cloudcelery/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1096 2021-07-22 02:42:02.000000 FicusFramework-3.1.0.post2/src/cloudcelery/celery_config.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/config/
+-rw-r--r--   0 sun        (501) wheel        (0)    10997 2021-07-16 06:13:02.000000 FicusFramework-3.1.0.post2/src/config/BootstrapPropertyLoader.py
+-rw-r--r--   0 sun        (501) wheel        (0)     4953 2023-03-16 07:22:14.000000 FicusFramework-3.1.0.post2/src/config/annotation.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2302 2021-07-16 06:12:10.000000 FicusFramework-3.1.0.post2/src/config/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/discovery/
+-rw-r--r--   0 sun        (501) wheel        (0)    14413 2021-07-07 07:23:16.000000 FicusFramework-3.1.0.post2/src/discovery/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/
+-rw-r--r--   0 sun        (501) wheel        (0)    33598 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/factdatasource/FactDatasourceProxyService.py
+-rw-r--r--   0 sun        (501) wheel        (0)    12673 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/factdatasource/FactDatasourceContextHolder.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/transformer/
+-rw-r--r--   0 sun        (501) wheel        (0)      718 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/transformer/ChineseToNumberTransformer.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2338 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/transformer/TransformerContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)      762 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/transformer/ITransformer.py
+-rw-r--r--   0 sun        (501) wheel        (0)      579 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/transformer/CompleteGB32100Transformer.py
+-rw-r--r--   0 sun        (501) wheel        (0)        0 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/transformer/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1001 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/transformer/FixItemTransformer.py
+-rw-r--r--   0 sun        (501) wheel        (0)      991 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/transformer/ParseDateTimeTransformer.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3749 2021-03-25 11:30:40.000000 FicusFramework-3.1.0.post2/src/factdatasource/transformer/DefaultValueTransformer.py
+-rw-r--r--   0 sun        (501) wheel        (0)      881 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/transformer/CompleteStringTransformer.py
+-rw-r--r--   0 sun        (501) wheel        (0)      900 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/transformer/NumberToChineseTransformer.py
+-rw-r--r--   0 sun        (501) wheel        (0)    34157 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/factdatasource/FactDatasourceProxyServiceV2.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/
+-rw-r--r--   0 sun        (501) wheel        (0)     2095 2022-11-15 06:30:54.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/MultipleDatasourceHolder.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/redis/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/redis/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)      643 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/redis/RedisDatasourceDao.py
+-rw-r--r--   0 sun        (501) wheel        (0)     7237 2021-12-10 03:38:55.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/redis/MultipleRedisDatasource.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/graph/
+-rw-r--r--   0 sun        (501) wheel        (0)     8390 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/graph/GraphDatasourceDao.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1093 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/graph/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/amqp/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/amqp/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     5310 2021-12-10 03:28:59.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/amqp/MultipleAmqpDatasource.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1778 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/amqp/AmqpDatasourceDao.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/jdbc/
+-rw-r--r--   0 sun        (501) wheel        (0)     3174 2020-09-28 06:27:10.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/jdbc/JdbcDatasourceDao.py
+-rw-r--r--   0 sun        (501) wheel        (0)    12694 2021-12-10 03:36:30.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/jdbc/MultipleJdbcDatasource.py
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/jdbc/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/kafka/
+-rw-r--r--   0 sun        (501) wheel        (0)     5501 2020-09-28 07:42:31.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/kafka/MultipleKafkaDatasource.py
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/kafka/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)      926 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/kafka/KafkaDatasourceDao.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/stomp/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/stomp/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     5132 2020-09-28 07:42:31.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/stomp/MultipleStompDatasource.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1035 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/stomp/StompDatasourceDao.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/tablestore/
+-rw-r--r--   0 sun        (501) wheel        (0)       88 2022-11-15 06:30:54.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/tablestore/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     5137 2022-11-15 06:30:54.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/tablestore/MultipleTableStoreDatasource.py
+-rw-r--r--   0 sun        (501) wheel        (0)      564 2022-11-15 06:30:54.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/tablestore/TableStoreDatasourceDao.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/mongo/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/mongo/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3567 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/mongo/MongoDatasourceDao.py
+-rw-r--r--   0 sun        (501) wheel        (0)     5894 2021-12-10 03:37:48.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/mongo/MultipleMongoDatasource.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/es/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/es/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3287 2020-06-17 11:00:50.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/es/EsDatasourceDao.py
+-rw-r--r--   0 sun        (501) wheel        (0)     4484 2020-09-28 07:42:31.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/es/MultipleEsDatasource.py
+-rw-r--r--   0 sun        (501) wheel        (0)     4600 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/dao/FactDatasource.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1603 2020-09-28 07:42:31.000000 FicusFramework-3.1.0.post2/src/factdatasource/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/message/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/message/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)    10913 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/factdatasource/message/FactDatasourceMessageHanlder.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/file/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/file/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3186 2020-03-23 08:49:50.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/file/FileFactDatasourceContext.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/redis/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/redis/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)    12650 2020-12-09 07:31:39.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/redis/RedisFactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/amqp/
+-rw-r--r--   0 sun        (501) wheel        (0)     5276 2020-12-09 07:28:30.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/amqp/AmqpFactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/amqp/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)    12086 2020-12-09 07:23:42.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/AbstractFactDatasourceContext.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/algorithm/
+-rw-r--r--   0 sun        (501) wheel        (0)        0 2020-07-27 11:07:37.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/algorithm/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     8030 2020-07-27 11:07:37.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/algorithm/AlgorithmFactDatasourceContext.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/jdbc/
+-rw-r--r--   0 sun        (501) wheel        (0)      534 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/jdbc/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)    15075 2020-12-09 07:29:32.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/jdbc/JdbcFactDatasourceContext.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/jdbc/dialect/
+-rw-r--r--   0 sun        (501) wheel        (0)      740 2021-02-03 08:54:08.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/jdbc/dialect/VernoxntsJdbcFactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3436 2020-12-09 07:30:40.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/jdbc/dialect/PostgresqlJdbcFactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3703 2020-12-09 07:30:49.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/jdbc/dialect/SqlserverJdbcFactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/jdbc/dialect/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)      532 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/jdbc/dialect/Db2JdbcFactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3801 2020-12-09 07:30:13.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/jdbc/dialect/OracleJdbcFactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)      283 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/jdbc/dialect/VernoxJdbcFactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3291 2020-12-09 07:29:54.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/jdbc/dialect/MysqlJdbcFactDatasourceContext.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/kafka/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/kafka/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     5513 2021-01-27 02:59:31.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/kafka/KafkaFactDatasourceContext.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/stomp/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/stomp/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     5325 2020-12-09 07:31:55.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/stomp/StompFactDatasourceContext.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/tablestore/
+-rw-r--r--   0 sun        (501) wheel        (0)       88 2022-11-15 06:30:54.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/tablestore/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)    29851 2022-11-15 06:30:54.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/tablestore/TableStoreDatasourceContext.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/mongo/
+-rw-r--r--   0 sun        (501) wheel        (0)    13093 2021-05-18 02:18:14.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/mongo/MongoFactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/mongo/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/sobeyhive/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/sobeyhive/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)    15917 2020-12-09 07:31:49.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/sobeyhive/SobeyHiveFactDatasourceContext.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/es/
+-rw-r--r--   0 sun        (501) wheel        (0)    14150 2020-12-09 07:29:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/es/EsFactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/es/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/custom/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/custom/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2913 2020-03-23 08:49:50.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/custom/CustomFactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)     6093 2020-03-23 08:49:50.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/SqlableDeleteCondition.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/graphdb/
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/graphdb/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)    11260 2020-12-09 07:29:19.000000 FicusFramework-3.1.0.post2/src/factdatasource/persistence/graphdb/GraphdbFactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)     4175 2020-03-23 08:49:50.000000 FicusFramework-3.1.0.post2/src/factdatasource/FactDatasourceContext.py
+-rw-r--r--   0 sun        (501) wheel        (0)      609 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/factdatasource/execptions.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/libs/
+-rw-r--r--   0 sun        (501) wheel        (0)     1008 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/libs/HeaderHolder.py
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2023-04-14 11:35:27.000000 FicusFramework-3.1.0.post2/src/libs/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     6659 2021-02-03 08:54:08.000000 FicusFramework-3.1.0.post2/src/libs/utils.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/py_eureka_client/
+-rw-r--r--   0 sun        (501) wheel        (0)     3118 2020-06-15 12:21:33.000000 FicusFramework-3.1.0.post2/src/py_eureka_client/__urlopen_proxy__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     4398 2020-06-15 12:21:33.000000 FicusFramework-3.1.0.post2/src/py_eureka_client/http_client.py
+-rw-r--r--   0 sun        (501) wheel        (0)       25 2020-06-15 12:21:33.000000 FicusFramework-3.1.0.post2/src/py_eureka_client/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)    52699 2021-07-07 06:44:45.000000 FicusFramework-3.1.0.post2/src/py_eureka_client/eureka_client.py
+-rw-r--r--   0 sun        (501) wheel        (0)      951 2020-06-15 12:21:33.000000 FicusFramework-3.1.0.post2/src/py_eureka_client/__logger__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/registry/
+-rw-r--r--   0 sun        (501) wheel        (0)    12757 2023-06-16 10:18:53.000000 FicusFramework-3.1.0.post2/src/registry/LoadOnRegistryLoader.py
+-rw-r--r--   0 sun        (501) wheel        (0)     7749 2020-09-28 06:27:10.000000 FicusFramework-3.1.0.post2/src/registry/LoadOnAlgorithmLoader.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2681 2020-07-20 06:12:53.000000 FicusFramework-3.1.0.post2/src/registry/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/api/
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/api/handler/
+-rw-r--r--   0 sun        (501) wheel        (0)      114 2019-04-15 11:08:07.000000 FicusFramework-3.1.0.post2/src/api/handler/IKillable.py
+-rw-r--r--   0 sun        (501) wheel        (0)     6935 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/api/handler/ICacheAbleHandler.py
+-rw-r--r--   0 sun        (501) wheel        (0)      160 2019-04-15 11:08:07.000000 FicusFramework-3.1.0.post2/src/api/handler/IHandler.py
+-rw-r--r--   0 sun        (501) wheel        (0)      530 2019-12-13 09:21:10.000000 FicusFramework-3.1.0.post2/src/api/handler/IProgressAble.py
+-rw-r--r--   0 sun        (501) wheel        (0)       77 2019-04-15 11:08:07.000000 FicusFramework-3.1.0.post2/src/api/handler/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/api/handler/message/
+-rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/api/handler/message/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1075 2019-04-15 11:08:07.000000 FicusFramework-3.1.0.post2/src/api/handler/message/IMessageHandler.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1039 2021-05-28 02:02:59.000000 FicusFramework-3.1.0.post2/src/api/handler/ITaskHandler.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/api/handler/script/
+-rw-r--r--   0 sun        (501) wheel        (0)      134 2019-12-13 09:21:10.000000 FicusFramework-3.1.0.post2/src/api/handler/script/ScriptHandlerHolder.py
+-rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/api/handler/script/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3686 2023-03-16 07:29:04.000000 FicusFramework-3.1.0.post2/src/api/handler/script/ScriptPythonFactory.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1759 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/api/handler/script/ICacheAbleScript.py
+-rw-r--r--   0 sun        (501) wheel        (0)    11195 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/api/handler/script/ScriptPythonTaskHandler.py
+-rw-r--r--   0 sun        (501) wheel        (0)      301 2019-12-13 09:21:10.000000 FicusFramework-3.1.0.post2/src/api/handler/script/IProgressAbleScript.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/api/handler/crawl/
+-rw-r--r--   0 sun        (501) wheel        (0)      638 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/api/handler/crawl/ISampleScriptCrawl.py
+-rw-r--r--   0 sun        (501) wheel        (0)     6190 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/api/handler/crawl/AbstractBatchCrawl.py
+-rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/api/handler/crawl/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     5522 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/api/handler/crawl/AbstractSimpleCrawl.py
+-rw-r--r--   0 sun        (501) wheel        (0)      937 2021-05-28 02:29:13.000000 FicusFramework-3.1.0.post2/src/api/handler/crawl/ISimpleScriptCrawl.py
+-rw-r--r--   0 sun        (501) wheel        (0)      428 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/api/handler/ILogAbleHandler.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/api/handler/outputer/
+-rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/api/handler/outputer/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)      923 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/api/handler/outputer/ISimpleOutputer.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3929 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/api/handler/outputer/IBatchOutputer.py
+-rw-r--r--   0 sun        (501) wheel        (0)     5490 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/api/handler/outputer/IBaseOutputer.py
+-rw-r--r--   0 sun        (501) wheel        (0)      199 2021-05-28 02:09:19.000000 FicusFramework-3.1.0.post2/src/api/handler/IRevoke.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1203 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/api/handler/ICacheAble.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/api/handler/ce/
+-rw-r--r--   0 sun        (501) wheel        (0)     7827 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/api/handler/ce/IMessageCE.py
+-rw-r--r--   0 sun        (501) wheel        (0)    13379 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/api/handler/ce/AbstractAsyncServiceBatchCE.py
+-rw-r--r--   0 sun        (501) wheel        (0)     6467 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/api/handler/ce/AbstractBatchCE.py
+-rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/api/handler/ce/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)      765 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/api/handler/ce/ISampleScriptCE.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1094 2021-05-28 02:28:47.000000 FicusFramework-3.1.0.post2/src/api/handler/ce/ISimpleScriptCE.py
+-rw-r--r--   0 sun        (501) wheel        (0)     5919 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/api/handler/ce/AbstractMessageCE.py
+-rw-r--r--   0 sun        (501) wheel        (0)      421 2020-07-06 10:53:29.000000 FicusFramework-3.1.0.post2/src/api/handler/IAsyncAble.py
+-rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/api/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/api/annotation/
+-rw-r--r--   0 sun        (501) wheel        (0)      396 2020-03-23 08:49:50.000000 FicusFramework-3.1.0.post2/src/api/annotation/annotation.py
+-rw-r--r--   0 sun        (501) wheel        (0)        0 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/api/annotation/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/api/model/
+-rw-r--r--   0 sun        (501) wheel        (0)     2026 2019-12-13 09:21:10.000000 FicusFramework-3.1.0.post2/src/api/model/OutputWrapper.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1123 2020-07-06 10:53:29.000000 FicusFramework-3.1.0.post2/src/api/model/AsyncServiceRequest.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3853 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/api/model/AlgorithmFdInputWrapper.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1182 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/api/model/GraphNode.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1128 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/api/model/ReadWriteLock.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2088 2021-01-27 02:59:31.000000 FicusFramework-3.1.0.post2/src/api/model/MetaModel.py
+-rw-r--r--   0 sun        (501) wheel        (0)      679 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/api/model/ResultVO.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1777 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/api/model/GraphRelation.py
+-rw-r--r--   0 sun        (501) wheel        (0)      640 2020-07-06 10:53:29.000000 FicusFramework-3.1.0.post2/src/api/model/AsyncServiceResponse.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1791 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/api/model/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3225 2019-12-13 09:21:10.000000 FicusFramework-3.1.0.post2/src/api/model/BatchOutputPipe.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1879 2021-03-25 11:31:25.000000 FicusFramework-3.1.0.post2/src/api/model/Page.py
+-rw-r--r--   0 sun        (501) wheel        (0)      375 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/api/model/FactDatasourceQueryParameter.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1857 2021-03-25 10:50:10.000000 FicusFramework-3.1.0.post2/src/api/model/MetaModelField.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2046 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/api/model/MetaModelTransform.py
+-rw-r--r--   0 sun        (501) wheel        (0)      952 2020-03-23 08:49:50.000000 FicusFramework-3.1.0.post2/src/api/model/Condition.py
+-rw-r--r--   0 sun        (501) wheel        (0)      855 2020-07-27 11:07:37.000000 FicusFramework-3.1.0.post2/src/api/model/AlgoOutWrapper.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1572 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/api/model/FdInputPipe.py
+-rw-r--r--   0 sun        (501) wheel        (0)     6733 2019-02-27 06:21:54.000000 FicusFramework-3.1.0.post2/src/api/model/OtherTargetOutputPipe.py
+-rw-r--r--   0 sun        (501) wheel        (0)     4423 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/api/model/FdInputWrapper.py
+-rw-r--r--   0 sun        (501) wheel        (0)     5501 2022-11-15 06:30:54.000000 FicusFramework-3.1.0.post2/src/api/model/FactDatasource.py
+-rw-r--r--   0 sun        (501) wheel        (0)      245 2019-04-15 11:08:07.000000 FicusFramework-3.1.0.post2/src/api/exceptions.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/rule_engine/
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/rule_engine/operation/
+-rw-r--r--   0 sun        (501) wheel        (0)     4529 2019-04-15 11:08:07.000000 FicusFramework-3.1.0.post2/src/rule_engine/operation/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)    13749 2019-04-15 11:08:07.000000 FicusFramework-3.1.0.post2/src/rule_engine/RuleEngineInitialize.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/rule_engine/core/
+-rw-r--r--   0 sun        (501) wheel        (0)     3330 2019-04-15 11:08:07.000000 FicusFramework-3.1.0.post2/src/rule_engine/core/SimpleValueProvider.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1201 2019-04-15 11:08:07.000000 FicusFramework-3.1.0.post2/src/rule_engine/core/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3576 2019-04-15 11:08:07.000000 FicusFramework-3.1.0.post2/src/rule_engine/core/SimpleRuleGroupSession.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2784 2019-04-15 11:08:07.000000 FicusFramework-3.1.0.post2/src/rule_engine/core/DefaultAgenda.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3489 2019-04-15 11:08:07.000000 FicusFramework-3.1.0.post2/src/rule_engine/core/PattenMatcher.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2061 2019-04-15 11:08:07.000000 FicusFramework-3.1.0.post2/src/rule_engine/RuleEngine.py
+-rw-r--r--   0 sun        (501) wheel        (0)    11736 2019-04-15 11:08:07.000000 FicusFramework-3.1.0.post2/src/rule_engine/__init__.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/rule_engine/action/
+-rw-r--r--   0 sun        (501) wheel        (0)     1347 2019-04-15 11:08:07.000000 FicusFramework-3.1.0.post2/src/rule_engine/action/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1678 2019-04-15 11:08:07.000000 FicusFramework-3.1.0.post2/src/rule_engine/RuleEngineCustomScriptFactory.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/service/
+-rw-r--r--   0 sun        (501) wheel        (0)     1809 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/service/FactDatasourceService.py
+-rw-r--r--   0 sun        (501) wheel        (0)       89 2019-05-13 10:28:04.000000 FicusFramework-3.1.0.post2/src/service/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2256 2020-04-29 11:49:46.000000 FicusFramework-3.1.0.post2/src/service/TaskQueueService.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/FicusFramework.egg-info/
+-rw-r--r--   0 sun        (501) wheel        (0)     2978 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/FicusFramework.egg-info/PKG-INFO
+-rw-r--r--   0 sun        (501) wheel        (0)        1 2019-02-27 06:22:29.000000 FicusFramework-3.1.0.post2/src/FicusFramework.egg-info/not-zip-safe
+-rw-r--r--   0 sun        (501) wheel        (0)     9687 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/FicusFramework.egg-info/SOURCES.txt
+-rw-r--r--   0 sun        (501) wheel        (0)      247 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/FicusFramework.egg-info/requires.txt
+-rw-r--r--   0 sun        (501) wheel        (0)      127 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/FicusFramework.egg-info/top_level.txt
+-rw-r--r--   0 sun        (501) wheel        (0)        1 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/FicusFramework.egg-info/dependency_links.txt
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/client/
+-rw-r--r--   0 sun        (501) wheel        (0)     3234 2019-04-15 11:08:07.000000 FicusFramework-3.1.0.post2/src/client/ComputeExecutionClient.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1035 2020-09-28 07:42:31.000000 FicusFramework-3.1.0.post2/src/client/FactDatasourceManageClient.py
+-rw-r--r--   0 sun        (501) wheel        (0)     6946 2021-08-13 06:23:01.000000 FicusFramework-3.1.0.post2/src/client/ScheduleJobTaskLogClient.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1173 2020-04-29 13:07:29.000000 FicusFramework-3.1.0.post2/src/client/ScheduleCloudClient.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2158 2019-04-15 11:08:07.000000 FicusFramework-3.1.0.post2/src/client/HandlerLogClient.py
+-rw-r--r--   0 sun        (501) wheel        (0)     1791 2021-06-04 07:35:30.000000 FicusFramework-3.1.0.post2/src/client/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)     8802 2019-04-15 11:08:40.000000 FicusFramework-3.1.0.post2/src/client/JobScheduleClient.py
+-rw-r--r--   0 sun        (501) wheel        (0)     4296 2019-04-15 11:08:07.000000 FicusFramework-3.1.0.post2/src/client/DataCrawlClient.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3996 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/client/ClientAuth.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3815 2020-07-24 11:47:04.000000 FicusFramework-3.1.0.post2/src/client/DataAlgorithmClient.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2850 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/client/AuthClient.py
+-rw-r--r--   0 sun        (501) wheel        (0)     2254 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/client/FactDatasourceClient.py
+-rw-r--r--   0 sun        (501) wheel        (0)     3905 2019-04-15 11:08:07.000000 FicusFramework-3.1.0.post2/src/client/ScheduleCacheClient.py
+drwxr-xr-x   0 sun        (501) wheel        (0)        0 2023-06-16 10:22:58.000000 FicusFramework-3.1.0.post2/src/remote/
+-rw-r--r--   0 sun        (501) wheel        (0)     1453 2020-03-23 08:49:50.000000 FicusFramework-3.1.0.post2/src/remote/TriggerRemoteActor.py
+-rw-r--r--   0 sun        (501) wheel        (0)      591 2020-06-15 12:21:33.000000 FicusFramework-3.1.0.post2/src/remote/__init__.py
+-rw-r--r--   0 sun        (501) wheel        (0)      795 2020-03-24 09:55:45.000000 FicusFramework-3.1.0.post2/src/remote/PrometheusMetricsRemoteService.py
+-rw-r--r--   0 sun        (501) wheel        (0)      375 2023-04-24 03:54:16.000000 FicusFramework-3.1.0.post2/src/remote/ActuatorRemote.py
+-rw-r--r--   0 sun        (501) wheel        (0)      914 2019-06-25 08:47:51.000000 FicusFramework-3.1.0.post2/src/remote/LogReadRemoteService.py
+-rw-r--r--   0 sun        (501) wheel        (0)     7060 2020-12-11 02:26:37.000000 FicusFramework-3.1.0.post2/src/remote/AsyncResponseRestService.py
```

### Comparing `FicusFramework-3.1.0/PKG-INFO` & `FicusFramework-3.1.0.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 1.1
 Name: FicusFramework
-Version: 3.1.0
-Summary: A framework for Ficus by Python3.
+Version: 3.1.0.post2
+Summary: A framework for Ficus by Python3. Require Sobey-Ficus:3.0.2304181043+
 Home-page: https://git.sobey.com/SobeyHive/FicusFramework4Py
 Author: sunxiang0918
 Author-email: sunxiang0918@gmail.com
 License: MIT
 Description: \u0023\u0020\u0046\u0069\u0063\u0075\u0073\u0020\u0050\u0079\u0074\u0068\u006f\u006e\u0020\u5f00\u53d1\u5957\u4ef6\u000d\u000a\u000d\u000a\u000d\u000a\u0023\u0023\u0020\u5f00\u53d1\u6b65\u9aa4\u000d\u000a\u000d\u000a\u0031\u002e\u0020\u5fc5\u987b\u8981\u6709\u4e00\u4e2a\u0060\u0061\u0070\u0070\u002e\u0070\u0079\u0060\u6587\u4ef6\u002c\u7528\u4e8e\u53d1\u5e03\u0060\u0066\u006c\u0061\u0073\u006b\u0060\u7684\u0072\u0065\u0073\u0074\u0066\u0075\u006c\u0020\u0041\u0070\u0069\u000d\u000a\u0032\u002e\u0020\u5728\u0060\u0061\u0070\u0070\u002e\u0070\u0079\u0060\u4e2d\u6267\u884c\u0060\u0061\u0070\u0070\u0020\u003d\u0020\u0046\u006c\u0061\u0073\u006b\u0028\u005f\u005f\u006e\u0061\u006d\u0065\u005f\u005f\u0029\u0060\u7528\u4e8e\u542f\u52a8\u0046\u006c\u0061\u0073\u006b\u670d\u52a1\u000d\u000a\u0033\u002e\u0020\u4f7f\u7528\u0060\u0066\u0072\u006f\u006d\u0020\u0072\u0065\u006d\u006f\u0074\u0065\u0020\u0069\u006d\u0070\u006f\u0072\u0074\u0020\u002a\u0060\u0020\u5bfc\u5165\u0072\u0065\u0073\u0074\u7684\u0060\u0065\u006e\u0064\u0070\u006f\u0069\u006e\u0074\u0060\u000d\u000a\u0034\u002e\u0020\u5728\u9879\u76ee\u4e2d\u521b\u5efa\u4e00\u4e2a\u0060\u0045\u0075\u0072\u0065\u006b\u0061\u0043\u006c\u0069\u0065\u006e\u0074\u0060\u002c\u5e76\u6307\u5b9a\u670d\u52a1\u7684\u540d\u79f0\u548c\u0065\u0075\u0072\u0065\u006b\u0061\u7684\u5730\u5740\u000d\u000a\u0035\u002e\u0020\u8c03\u7528\u0060\u0045\u0075\u0072\u0065\u006b\u0061\u0043\u006c\u0069\u0065\u006e\u0074\u0060\u7684\u65b9\u6cd5\u0060\u0072\u0065\u0067\u0069\u0073\u0074\u0065\u0072\u0028\u0026\u0071\u0075\u006f\u0074\u003b\u0055\u0050\u0026\u0071\u0075\u006f\u0074\u003b\u0029\u0060\u4ee5\u53ca\u0060\u0073\u0074\u0061\u0072\u0074\u005f\u0068\u0065\u0061\u0072\u0074\u0062\u0065\u0061\u0074\u0060\u5411\u0065\u0075\u0072\u0065\u006b\u0061\u6ce8\u518c\u53ca\u5fc3\u8df3\u000d\u000a\u000d\u000a\u000d\u000a\u0023\u0023\u0020\u6ce8\u610f\u4e8b\u9879\u000d\u000a\u000d\u000a\u0031\u002e\u0020\u0041\u0070\u0069\u4e2d\u6240\u6709\u7684\u0056\u004f\u5bf9\u8c61\u0020\u90fd\u662f\u7528\u4e86\u0020\u005b\u0060\u006d\u0075\u006e\u0063\u0068\u0060\u005d\u0028\u0068\u0074\u0074\u0070\u0073\u003a\u002f\u002f\u0067\u0069\u0074\u0068\u0075\u0062\u002e\u0063\u006f\u006d\u002f\u0049\u006e\u0066\u0069\u006e\u0069\u0064\u0061\u0074\u002f\u006d\u0075\u006e\u0063\u0068\u0029\u0020\u505a\u4ea4\u4e92\u002e
 Keywords: ficus framework python
 Platform: UNKNOWN
```

### Comparing `FicusFramework-3.1.0/test/test_factDatasourceChangeListener.py` & `FicusFramework-3.1.0.post2/test/test_factDatasourceChangeListener.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/test/test_abstractSimpleScripCrawlTestSuite.py` & `FicusFramework-3.1.0.post2/test/test_abstractSimpleScripCrawlTestSuite.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/test/test_utils.py` & `FicusFramework-3.1.0.post2/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/test/test_customerDaoContextHolder.py` & `FicusFramework-3.1.0.post2/test/test_customerDaoContextHolder.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/test/test_cryptography.py` & `FicusFramework-3.1.0.post2/test/test_cryptography.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/test/test_distributedFactDatasourceProxy.py` & `FicusFramework-3.1.0.post2/test/test_distributedFactDatasourceProxy.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/test/test_abstractBatchCETestSuite.py` & `FicusFramework-3.1.0.post2/test/test_abstractBatchCETestSuite.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/test/test_factDatasourceService.py` & `FicusFramework-3.1.0.post2/test/test_factDatasourceService.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/test/test_abstractSimpleScriptCETestSuite.py` & `FicusFramework-3.1.0.post2/test/test_abstractSimpleScriptCETestSuite.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/test/test_abstractSimpleCrawlTestSuite.py` & `FicusFramework-3.1.0.post2/test/test_abstractSimpleCrawlTestSuite.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/test/test_abstractBatchCrawlTestSuite.py` & `FicusFramework-3.1.0.post2/test/test_abstractBatchCrawlTestSuite.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/setup.py` & `FicusFramework-3.1.0.post2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name="FicusFramework",
-    version="3.1.0",
+    version="3.1.0.post2",
 
     packages=find_packages('src'),
     package_dir={'': 'src'},
     test_suite="test",
 
     install_requires=["flask>=1.1.2", "flask-cors>=3.0.8", "requests>=2.23.0", "apscheduler>=3.6.3", "jsonpath-rw>=1.4.0",
                       "munch>=2.5.0", "PyYaml>=5.3.1", "readerwriterlock>=1.0.7", "confluent-kafka>=1.3.0",
                       "sqlalchemy>=1.3.3", "mysqlclient","pymongo","gevent","Celery==4.4.7","redis>=3.5.3","python-consul2"],
 
     author='sunxiang0918',
     author_email="sunxiang0918@gmail.com",
-    description="A framework for Ficus by Python3.",
+    description="A framework for Ficus by Python3. Require Sobey-Ficus:3.0.2304181043+",
     long_description=read("README.rst"),
     license="MIT",
     keywords="ficus framework python",
     url="https://git.sobey.com/SobeyHive/FicusFramework4Py",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
```

### Comparing `FicusFramework-3.1.0/README.rst` & `FicusFramework-3.1.0.post2/README.rst`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/init/app.py` & `FicusFramework-3.1.0.post2/src/init/app.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/schedule/TaskThreadHolder.py` & `FicusFramework-3.1.0.post2/src/schedule/TaskThreadHolder.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/schedule/test/suite/crawl.py` & `FicusFramework-3.1.0.post2/src/schedule/test/suite/crawl.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/schedule/test/suite/__init__.py` & `FicusFramework-3.1.0.post2/src/schedule/test/suite/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/schedule/test/suite/ce.py` & `FicusFramework-3.1.0.post2/src/schedule/test/suite/ce.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/schedule/TaskThread.py` & `FicusFramework-3.1.0.post2/src/schedule/TaskThread.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/schedule/utils/log/TaskLogFileAppender.py` & `FicusFramework-3.1.0.post2/src/schedule/utils/log/TaskLogFileAppender.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/schedule/utils/log/TaskLogCleanScheduler.py` & `FicusFramework-3.1.0.post2/src/schedule/utils/log/TaskLogCleanScheduler.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/schedule/utils/log/TaskLogger.py` & `FicusFramework-3.1.0.post2/src/schedule/utils/log/TaskLogger.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/schedule/utils/log/FrameworkHandlerLogger.py` & `FicusFramework-3.1.0.post2/src/schedule/utils/log/FrameworkHandlerLogger.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/schedule/TriggerActor.py` & `FicusFramework-3.1.0.post2/src/schedule/TriggerActor.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/cloudcelery/CeleryOnRequest.py` & `FicusFramework-3.1.0.post2/src/cloudcelery/CeleryOnRequest.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/cloudcelery/__init__.py` & `FicusFramework-3.1.0.post2/src/cloudcelery/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/cloudcelery/celery_config.py` & `FicusFramework-3.1.0.post2/src/cloudcelery/celery_config.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/config/BootstrapPropertyLoader.py` & `FicusFramework-3.1.0.post2/src/config/BootstrapPropertyLoader.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/config/annotation.py` & `FicusFramework-3.1.0.post2/src/config/annotation.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/config/__init__.py` & `FicusFramework-3.1.0.post2/src/config/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/discovery/__init__.py` & `FicusFramework-3.1.0.post2/src/discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/FactDatasourceProxyService.py` & `FicusFramework-3.1.0.post2/src/factdatasource/FactDatasourceProxyService.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/FactDatasourceContextHolder.py` & `FicusFramework-3.1.0.post2/src/factdatasource/FactDatasourceContextHolder.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/transformer/ChineseToNumberTransformer.py` & `FicusFramework-3.1.0.post2/src/factdatasource/transformer/ChineseToNumberTransformer.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/transformer/TransformerContext.py` & `FicusFramework-3.1.0.post2/src/factdatasource/transformer/TransformerContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/transformer/ITransformer.py` & `FicusFramework-3.1.0.post2/src/factdatasource/transformer/ITransformer.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/transformer/CompleteGB32100Transformer.py` & `FicusFramework-3.1.0.post2/src/factdatasource/transformer/CompleteGB32100Transformer.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/transformer/FixItemTransformer.py` & `FicusFramework-3.1.0.post2/src/factdatasource/transformer/FixItemTransformer.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/transformer/ParseDateTimeTransformer.py` & `FicusFramework-3.1.0.post2/src/factdatasource/transformer/ParseDateTimeTransformer.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/transformer/DefaultValueTransformer.py` & `FicusFramework-3.1.0.post2/src/factdatasource/transformer/DefaultValueTransformer.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/transformer/CompleteStringTransformer.py` & `FicusFramework-3.1.0.post2/src/factdatasource/transformer/CompleteStringTransformer.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/transformer/NumberToChineseTransformer.py` & `FicusFramework-3.1.0.post2/src/factdatasource/transformer/NumberToChineseTransformer.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/FactDatasourceProxyServiceV2.py` & `FicusFramework-3.1.0.post2/src/factdatasource/FactDatasourceProxyServiceV2.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/dao/MultipleDatasourceHolder.py` & `FicusFramework-3.1.0.post2/src/factdatasource/dao/MultipleDatasourceHolder.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/dao/redis/RedisDatasourceDao.py` & `FicusFramework-3.1.0.post2/src/factdatasource/dao/redis/RedisDatasourceDao.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/dao/redis/MultipleRedisDatasource.py` & `FicusFramework-3.1.0.post2/src/factdatasource/dao/redis/MultipleRedisDatasource.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/dao/graph/GraphDatasourceDao.py` & `FicusFramework-3.1.0.post2/src/factdatasource/dao/graph/GraphDatasourceDao.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/dao/graph/__init__.py` & `FicusFramework-3.1.0.post2/src/factdatasource/dao/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/dao/amqp/MultipleAmqpDatasource.py` & `FicusFramework-3.1.0.post2/src/factdatasource/dao/amqp/MultipleAmqpDatasource.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/dao/amqp/AmqpDatasourceDao.py` & `FicusFramework-3.1.0.post2/src/factdatasource/dao/amqp/AmqpDatasourceDao.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/dao/jdbc/JdbcDatasourceDao.py` & `FicusFramework-3.1.0.post2/src/factdatasource/dao/jdbc/JdbcDatasourceDao.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/dao/jdbc/MultipleJdbcDatasource.py` & `FicusFramework-3.1.0.post2/src/factdatasource/dao/jdbc/MultipleJdbcDatasource.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/dao/kafka/MultipleKafkaDatasource.py` & `FicusFramework-3.1.0.post2/src/factdatasource/dao/kafka/MultipleKafkaDatasource.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/dao/kafka/KafkaDatasourceDao.py` & `FicusFramework-3.1.0.post2/src/factdatasource/dao/kafka/KafkaDatasourceDao.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/dao/stomp/MultipleStompDatasource.py` & `FicusFramework-3.1.0.post2/src/factdatasource/dao/stomp/MultipleStompDatasource.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/dao/stomp/StompDatasourceDao.py` & `FicusFramework-3.1.0.post2/src/factdatasource/dao/stomp/StompDatasourceDao.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/dao/tablestore/MultipleTableStoreDatasource.py` & `FicusFramework-3.1.0.post2/src/factdatasource/dao/tablestore/MultipleTableStoreDatasource.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/dao/tablestore/TableStoreDatasourceDao.py` & `FicusFramework-3.1.0.post2/src/factdatasource/dao/tablestore/TableStoreDatasourceDao.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/dao/mongo/MongoDatasourceDao.py` & `FicusFramework-3.1.0.post2/src/factdatasource/dao/mongo/MongoDatasourceDao.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/dao/mongo/MultipleMongoDatasource.py` & `FicusFramework-3.1.0.post2/src/factdatasource/dao/mongo/MultipleMongoDatasource.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/dao/es/EsDatasourceDao.py` & `FicusFramework-3.1.0.post2/src/factdatasource/dao/es/EsDatasourceDao.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/dao/es/MultipleEsDatasource.py` & `FicusFramework-3.1.0.post2/src/factdatasource/dao/es/MultipleEsDatasource.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/dao/FactDatasource.py` & `FicusFramework-3.1.0.post2/src/factdatasource/dao/FactDatasource.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/__init__.py` & `FicusFramework-3.1.0.post2/src/factdatasource/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/message/FactDatasourceMessageHanlder.py` & `FicusFramework-3.1.0.post2/src/factdatasource/message/FactDatasourceMessageHanlder.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/persistence/file/FileFactDatasourceContext.py` & `FicusFramework-3.1.0.post2/src/factdatasource/persistence/file/FileFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/persistence/redis/RedisFactDatasourceContext.py` & `FicusFramework-3.1.0.post2/src/factdatasource/persistence/redis/RedisFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/persistence/amqp/AmqpFactDatasourceContext.py` & `FicusFramework-3.1.0.post2/src/factdatasource/persistence/amqp/AmqpFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/persistence/AbstractFactDatasourceContext.py` & `FicusFramework-3.1.0.post2/src/factdatasource/persistence/AbstractFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/persistence/algorithm/AlgorithmFactDatasourceContext.py` & `FicusFramework-3.1.0.post2/src/factdatasource/persistence/algorithm/AlgorithmFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/__init__.py` & `FicusFramework-3.1.0.post2/src/factdatasource/persistence/jdbc/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/JdbcFactDatasourceContext.py` & `FicusFramework-3.1.0.post2/src/factdatasource/persistence/jdbc/JdbcFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/VernoxntsJdbcFactDatasourceContext.py` & `FicusFramework-3.1.0.post2/src/factdatasource/persistence/jdbc/dialect/VernoxntsJdbcFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/PostgresqlJdbcFactDatasourceContext.py` & `FicusFramework-3.1.0.post2/src/factdatasource/persistence/jdbc/dialect/PostgresqlJdbcFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/SqlserverJdbcFactDatasourceContext.py` & `FicusFramework-3.1.0.post2/src/factdatasource/persistence/jdbc/dialect/SqlserverJdbcFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/Db2JdbcFactDatasourceContext.py` & `FicusFramework-3.1.0.post2/src/factdatasource/persistence/jdbc/dialect/Db2JdbcFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/OracleJdbcFactDatasourceContext.py` & `FicusFramework-3.1.0.post2/src/factdatasource/persistence/jdbc/dialect/OracleJdbcFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/persistence/jdbc/dialect/MysqlJdbcFactDatasourceContext.py` & `FicusFramework-3.1.0.post2/src/factdatasource/persistence/jdbc/dialect/MysqlJdbcFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/persistence/kafka/KafkaFactDatasourceContext.py` & `FicusFramework-3.1.0.post2/src/factdatasource/persistence/kafka/KafkaFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/persistence/stomp/StompFactDatasourceContext.py` & `FicusFramework-3.1.0.post2/src/factdatasource/persistence/stomp/StompFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/persistence/tablestore/TableStoreDatasourceContext.py` & `FicusFramework-3.1.0.post2/src/factdatasource/persistence/tablestore/TableStoreDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/persistence/mongo/MongoFactDatasourceContext.py` & `FicusFramework-3.1.0.post2/src/factdatasource/persistence/mongo/MongoFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/persistence/sobeyhive/SobeyHiveFactDatasourceContext.py` & `FicusFramework-3.1.0.post2/src/factdatasource/persistence/sobeyhive/SobeyHiveFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/persistence/es/EsFactDatasourceContext.py` & `FicusFramework-3.1.0.post2/src/factdatasource/persistence/es/EsFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/persistence/custom/CustomFactDatasourceContext.py` & `FicusFramework-3.1.0.post2/src/factdatasource/persistence/custom/CustomFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/persistence/SqlableDeleteCondition.py` & `FicusFramework-3.1.0.post2/src/factdatasource/persistence/SqlableDeleteCondition.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/persistence/graphdb/GraphdbFactDatasourceContext.py` & `FicusFramework-3.1.0.post2/src/factdatasource/persistence/graphdb/GraphdbFactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/FactDatasourceContext.py` & `FicusFramework-3.1.0.post2/src/factdatasource/FactDatasourceContext.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/factdatasource/execptions.py` & `FicusFramework-3.1.0.post2/src/factdatasource/execptions.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/libs/HeaderHolder.py` & `FicusFramework-3.1.0.post2/src/libs/HeaderHolder.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/libs/utils.py` & `FicusFramework-3.1.0.post2/src/libs/utils.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/py_eureka_client/__urlopen_proxy__.py` & `FicusFramework-3.1.0.post2/src/py_eureka_client/__urlopen_proxy__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/py_eureka_client/http_client.py` & `FicusFramework-3.1.0.post2/src/py_eureka_client/http_client.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/py_eureka_client/eureka_client.py` & `FicusFramework-3.1.0.post2/src/py_eureka_client/eureka_client.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/py_eureka_client/__logger__.py` & `FicusFramework-3.1.0.post2/src/py_eureka_client/__logger__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/registry/LoadOnRegistryLoader.py` & `FicusFramework-3.1.0.post2/src/registry/LoadOnRegistryLoader.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,25 +57,25 @@
                 computeexecution["execution"]["limits"] = -1
             if "params" not in computeexecution["execution"] or computeexecution["execution"]["params"] is None:
                 computeexecution["execution"]["params"] = {}
             if "retryTimes" not in computeexecution["execution"] or computeexecution["execution"]["retryTimes"] is None:
                 computeexecution["execution"]["retryTimes"] = 0
 
         if "managed" not in computeexecution or computeexecution["managed"] is None:
-            computeexecution["managed"] = {"type": "STANDBY", "serviceName": "STANDBY", "routing": "RANDOM"}
+            computeexecution["managed"] = {"type": "STANDBY", "serviceName": "STANDBY", "routing": None}
         else:
             if "type" not in computeexecution["managed"] or computeexecution["managed"]["type"] is None or \
                     computeexecution["managed"]["type"] == "":
                 computeexecution["managed"]["type"] = "STANDBY"
             if "serviceName" not in computeexecution["managed"] or computeexecution["managed"]["serviceName"] is None or \
                     computeexecution["managed"]["serviceName"] == "":
                 computeexecution["managed"]["serviceName"] = "STANDBY"
             if "routing" not in computeexecution["managed"] or computeexecution["managed"]["routing"] is None or \
                     computeexecution["managed"]["routing"] == "":
-                computeexecution["managed"]["routing"] = "RANDOM"
+                computeexecution["managed"]["routing"] = None
 
         if "outputs" not in computeexecution or computeexecution["outputs"] is None:
             computeexecution["outputs"] = []
         # endregion
 
         index = index + 1
 
@@ -167,22 +167,22 @@
             if "retryTimes" not in crawl["execution"] or crawl["execution"][
                 "retryTimes"] is None:
                 crawl["execution"]["retryTimes"] = 0
             if "params" not in crawl["execution"]:
                 crawl["execution"]["params"] = {}
 
         if "managed" not in crawl:
-            crawl["managed"] = {"type": "STANDBY", "serviceName": "STANDBY", "routing": "RANDOM"}
+            crawl["managed"] = {"type": "STANDBY", "serviceName": "STANDBY", "routing": None}
         else:
             if "type" not in crawl["managed"]:
                 crawl["managed"]["type"] = "STANDBY"
             if "serviceName" not in crawl["managed"]:
                 crawl["managed"]["serviceName"] = "STANDBY"
             if "routing" not in crawl["managed"]:
-                crawl["managed"]["routing"] = "RANDOM"
+                crawl["managed"]["routing"] = None
 
         if "outputs" not in crawl:
             crawl["outputs"] = []
         # endregion
 
         index = index + 1
```

### Comparing `FicusFramework-3.1.0/src/registry/LoadOnAlgorithmLoader.py` & `FicusFramework-3.1.0.post2/src/registry/LoadOnAlgorithmLoader.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/registry/__init__.py` & `FicusFramework-3.1.0.post2/src/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/handler/ICacheAbleHandler.py` & `FicusFramework-3.1.0.post2/src/api/handler/ICacheAbleHandler.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/handler/IProgressAble.py` & `FicusFramework-3.1.0.post2/src/api/handler/IProgressAble.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/handler/message/IMessageHandler.py` & `FicusFramework-3.1.0.post2/src/api/handler/message/IMessageHandler.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/handler/ITaskHandler.py` & `FicusFramework-3.1.0.post2/src/api/handler/ITaskHandler.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/handler/script/ScriptPythonFactory.py` & `FicusFramework-3.1.0.post2/src/api/handler/script/ScriptPythonFactory.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/handler/script/ICacheAbleScript.py` & `FicusFramework-3.1.0.post2/src/api/handler/script/ICacheAbleScript.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/handler/script/ScriptPythonTaskHandler.py` & `FicusFramework-3.1.0.post2/src/api/handler/script/ScriptPythonTaskHandler.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/handler/crawl/ISampleScriptCrawl.py` & `FicusFramework-3.1.0.post2/src/api/handler/crawl/ISampleScriptCrawl.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/handler/crawl/AbstractBatchCrawl.py` & `FicusFramework-3.1.0.post2/src/api/handler/crawl/AbstractBatchCrawl.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/handler/crawl/AbstractSimpleCrawl.py` & `FicusFramework-3.1.0.post2/src/api/handler/crawl/AbstractSimpleCrawl.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/handler/crawl/ISimpleScriptCrawl.py` & `FicusFramework-3.1.0.post2/src/api/handler/crawl/ISimpleScriptCrawl.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/handler/outputer/ISimpleOutputer.py` & `FicusFramework-3.1.0.post2/src/api/handler/outputer/ISimpleOutputer.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/handler/outputer/IBatchOutputer.py` & `FicusFramework-3.1.0.post2/src/api/handler/outputer/IBatchOutputer.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/handler/outputer/IBaseOutputer.py` & `FicusFramework-3.1.0.post2/src/api/handler/outputer/IBaseOutputer.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/handler/ICacheAble.py` & `FicusFramework-3.1.0.post2/src/api/handler/ICacheAble.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/handler/ce/IMessageCE.py` & `FicusFramework-3.1.0.post2/src/api/handler/ce/IMessageCE.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/handler/ce/AbstractAsyncServiceBatchCE.py` & `FicusFramework-3.1.0.post2/src/api/handler/ce/AbstractAsyncServiceBatchCE.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/handler/ce/AbstractBatchCE.py` & `FicusFramework-3.1.0.post2/src/api/handler/ce/AbstractBatchCE.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/handler/ce/ISampleScriptCE.py` & `FicusFramework-3.1.0.post2/src/api/handler/ce/ISampleScriptCE.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/handler/ce/ISimpleScriptCE.py` & `FicusFramework-3.1.0.post2/src/api/handler/ce/ISimpleScriptCE.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/handler/ce/AbstractMessageCE.py` & `FicusFramework-3.1.0.post2/src/api/handler/ce/AbstractMessageCE.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/model/OutputWrapper.py` & `FicusFramework-3.1.0.post2/src/api/model/OutputWrapper.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/model/AsyncServiceRequest.py` & `FicusFramework-3.1.0.post2/src/api/model/AsyncServiceRequest.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/model/AlgorithmFdInputWrapper.py` & `FicusFramework-3.1.0.post2/src/api/model/AlgorithmFdInputWrapper.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/model/GraphNode.py` & `FicusFramework-3.1.0.post2/src/api/model/GraphNode.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/model/ReadWriteLock.py` & `FicusFramework-3.1.0.post2/src/api/model/ReadWriteLock.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/model/MetaModel.py` & `FicusFramework-3.1.0.post2/src/api/model/MetaModel.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/model/ResultVO.py` & `FicusFramework-3.1.0.post2/src/api/model/ResultVO.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/model/GraphRelation.py` & `FicusFramework-3.1.0.post2/src/api/model/GraphRelation.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/model/AsyncServiceResponse.py` & `FicusFramework-3.1.0.post2/src/api/model/AsyncServiceResponse.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/model/__init__.py` & `FicusFramework-3.1.0.post2/src/api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/model/BatchOutputPipe.py` & `FicusFramework-3.1.0.post2/src/api/model/BatchOutputPipe.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/model/Page.py` & `FicusFramework-3.1.0.post2/src/api/model/Page.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/model/MetaModelField.py` & `FicusFramework-3.1.0.post2/src/api/model/MetaModelField.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/model/MetaModelTransform.py` & `FicusFramework-3.1.0.post2/src/api/model/MetaModelTransform.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/model/Condition.py` & `FicusFramework-3.1.0.post2/src/api/model/Condition.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/model/AlgoOutWrapper.py` & `FicusFramework-3.1.0.post2/src/api/model/AlgoOutWrapper.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/model/FdInputPipe.py` & `FicusFramework-3.1.0.post2/src/api/model/FdInputPipe.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/model/OtherTargetOutputPipe.py` & `FicusFramework-3.1.0.post2/src/api/model/OtherTargetOutputPipe.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/model/FdInputWrapper.py` & `FicusFramework-3.1.0.post2/src/api/model/FdInputWrapper.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/api/model/FactDatasource.py` & `FicusFramework-3.1.0.post2/src/api/model/FactDatasource.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/rule_engine/operation/__init__.py` & `FicusFramework-3.1.0.post2/src/rule_engine/operation/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/rule_engine/RuleEngineInitialize.py` & `FicusFramework-3.1.0.post2/src/rule_engine/RuleEngineInitialize.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/rule_engine/core/SimpleValueProvider.py` & `FicusFramework-3.1.0.post2/src/rule_engine/core/SimpleValueProvider.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/rule_engine/core/__init__.py` & `FicusFramework-3.1.0.post2/src/rule_engine/core/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/rule_engine/core/SimpleRuleGroupSession.py` & `FicusFramework-3.1.0.post2/src/rule_engine/core/SimpleRuleGroupSession.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/rule_engine/core/DefaultAgenda.py` & `FicusFramework-3.1.0.post2/src/rule_engine/core/DefaultAgenda.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/rule_engine/core/PattenMatcher.py` & `FicusFramework-3.1.0.post2/src/rule_engine/core/PattenMatcher.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/rule_engine/RuleEngine.py` & `FicusFramework-3.1.0.post2/src/rule_engine/RuleEngine.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/rule_engine/__init__.py` & `FicusFramework-3.1.0.post2/src/rule_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/rule_engine/action/__init__.py` & `FicusFramework-3.1.0.post2/src/rule_engine/action/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/rule_engine/RuleEngineCustomScriptFactory.py` & `FicusFramework-3.1.0.post2/src/rule_engine/RuleEngineCustomScriptFactory.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/service/FactDatasourceService.py` & `FicusFramework-3.1.0.post2/src/service/FactDatasourceService.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/service/TaskQueueService.py` & `FicusFramework-3.1.0.post2/src/service/TaskQueueService.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/FicusFramework.egg-info/PKG-INFO` & `FicusFramework-3.1.0.post2/src/FicusFramework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 1.1
 Name: FicusFramework
-Version: 3.1.0
-Summary: A framework for Ficus by Python3.
+Version: 3.1.0.post2
+Summary: A framework for Ficus by Python3. Require Sobey-Ficus:3.0.2304181043+
 Home-page: https://git.sobey.com/SobeyHive/FicusFramework4Py
 Author: sunxiang0918
 Author-email: sunxiang0918@gmail.com
 License: MIT
 Description: \u0023\u0020\u0046\u0069\u0063\u0075\u0073\u0020\u0050\u0079\u0074\u0068\u006f\u006e\u0020\u5f00\u53d1\u5957\u4ef6\u000d\u000a\u000d\u000a\u000d\u000a\u0023\u0023\u0020\u5f00\u53d1\u6b65\u9aa4\u000d\u000a\u000d\u000a\u0031\u002e\u0020\u5fc5\u987b\u8981\u6709\u4e00\u4e2a\u0060\u0061\u0070\u0070\u002e\u0070\u0079\u0060\u6587\u4ef6\u002c\u7528\u4e8e\u53d1\u5e03\u0060\u0066\u006c\u0061\u0073\u006b\u0060\u7684\u0072\u0065\u0073\u0074\u0066\u0075\u006c\u0020\u0041\u0070\u0069\u000d\u000a\u0032\u002e\u0020\u5728\u0060\u0061\u0070\u0070\u002e\u0070\u0079\u0060\u4e2d\u6267\u884c\u0060\u0061\u0070\u0070\u0020\u003d\u0020\u0046\u006c\u0061\u0073\u006b\u0028\u005f\u005f\u006e\u0061\u006d\u0065\u005f\u005f\u0029\u0060\u7528\u4e8e\u542f\u52a8\u0046\u006c\u0061\u0073\u006b\u670d\u52a1\u000d\u000a\u0033\u002e\u0020\u4f7f\u7528\u0060\u0066\u0072\u006f\u006d\u0020\u0072\u0065\u006d\u006f\u0074\u0065\u0020\u0069\u006d\u0070\u006f\u0072\u0074\u0020\u002a\u0060\u0020\u5bfc\u5165\u0072\u0065\u0073\u0074\u7684\u0060\u0065\u006e\u0064\u0070\u006f\u0069\u006e\u0074\u0060\u000d\u000a\u0034\u002e\u0020\u5728\u9879\u76ee\u4e2d\u521b\u5efa\u4e00\u4e2a\u0060\u0045\u0075\u0072\u0065\u006b\u0061\u0043\u006c\u0069\u0065\u006e\u0074\u0060\u002c\u5e76\u6307\u5b9a\u670d\u52a1\u7684\u540d\u79f0\u548c\u0065\u0075\u0072\u0065\u006b\u0061\u7684\u5730\u5740\u000d\u000a\u0035\u002e\u0020\u8c03\u7528\u0060\u0045\u0075\u0072\u0065\u006b\u0061\u0043\u006c\u0069\u0065\u006e\u0074\u0060\u7684\u65b9\u6cd5\u0060\u0072\u0065\u0067\u0069\u0073\u0074\u0065\u0072\u0028\u0026\u0071\u0075\u006f\u0074\u003b\u0055\u0050\u0026\u0071\u0075\u006f\u0074\u003b\u0029\u0060\u4ee5\u53ca\u0060\u0073\u0074\u0061\u0072\u0074\u005f\u0068\u0065\u0061\u0072\u0074\u0062\u0065\u0061\u0074\u0060\u5411\u0065\u0075\u0072\u0065\u006b\u0061\u6ce8\u518c\u53ca\u5fc3\u8df3\u000d\u000a\u000d\u000a\u000d\u000a\u0023\u0023\u0020\u6ce8\u610f\u4e8b\u9879\u000d\u000a\u000d\u000a\u0031\u002e\u0020\u0041\u0070\u0069\u4e2d\u6240\u6709\u7684\u0056\u004f\u5bf9\u8c61\u0020\u90fd\u662f\u7528\u4e86\u0020\u005b\u0060\u006d\u0075\u006e\u0063\u0068\u0060\u005d\u0028\u0068\u0074\u0074\u0070\u0073\u003a\u002f\u002f\u0067\u0069\u0074\u0068\u0075\u0062\u002e\u0063\u006f\u006d\u002f\u0049\u006e\u0066\u0069\u006e\u0069\u0064\u0061\u0074\u002f\u006d\u0075\u006e\u0063\u0068\u0029\u0020\u505a\u4ea4\u4e92\u002e
 Keywords: ficus framework python
 Platform: UNKNOWN
```

### Comparing `FicusFramework-3.1.0/src/FicusFramework.egg-info/SOURCES.txt` & `FicusFramework-3.1.0.post2/src/FicusFramework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/client/ComputeExecutionClient.py` & `FicusFramework-3.1.0.post2/src/client/ComputeExecutionClient.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/client/FactDatasourceManageClient.py` & `FicusFramework-3.1.0.post2/src/client/FactDatasourceManageClient.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/client/ScheduleJobTaskLogClient.py` & `FicusFramework-3.1.0.post2/src/client/ScheduleJobTaskLogClient.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/client/ScheduleCloudClient.py` & `FicusFramework-3.1.0.post2/src/client/ScheduleCloudClient.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/client/HandlerLogClient.py` & `FicusFramework-3.1.0.post2/src/client/HandlerLogClient.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/client/__init__.py` & `FicusFramework-3.1.0.post2/src/client/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/client/JobScheduleClient.py` & `FicusFramework-3.1.0.post2/src/client/JobScheduleClient.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/client/DataCrawlClient.py` & `FicusFramework-3.1.0.post2/src/client/DataCrawlClient.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/client/ClientAuth.py` & `FicusFramework-3.1.0.post2/src/client/ClientAuth.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/client/DataAlgorithmClient.py` & `FicusFramework-3.1.0.post2/src/client/DataAlgorithmClient.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/client/AuthClient.py` & `FicusFramework-3.1.0.post2/src/client/AuthClient.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/client/FactDatasourceClient.py` & `FicusFramework-3.1.0.post2/src/client/FactDatasourceClient.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/client/ScheduleCacheClient.py` & `FicusFramework-3.1.0.post2/src/client/ScheduleCacheClient.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/remote/TriggerRemoteActor.py` & `FicusFramework-3.1.0.post2/src/remote/TriggerRemoteActor.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/remote/__init__.py` & `FicusFramework-3.1.0.post2/src/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/remote/PrometheusMetricsRemoteService.py` & `FicusFramework-3.1.0.post2/src/remote/PrometheusMetricsRemoteService.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/remote/LogReadRemoteService.py` & `FicusFramework-3.1.0.post2/src/remote/LogReadRemoteService.py`

 * *Files identical despite different names*

### Comparing `FicusFramework-3.1.0/src/remote/AsyncResponseRestService.py` & `FicusFramework-3.1.0.post2/src/remote/AsyncResponseRestService.py`

 * *Files identical despite different names*

