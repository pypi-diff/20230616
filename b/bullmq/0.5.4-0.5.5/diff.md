# Comparing `tmp/bullmq-0.5.4.tar.gz` & `tmp/bullmq-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-0.5.4.tar", last modified: Wed Jun 14 14:01:52 2023, max compression
+gzip compressed data, was "bullmq-0.5.5.tar", last modified: Fri Jun 16 16:50:45 2023, max compression
```

## Comparing `bullmq-0.5.4.tar` & `bullmq-0.5.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:52.110907 bullmq-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-14 14:01:52.110907 bullmq-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-14 14:00:25.000000 bullmq-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:52.102907 bullmq-0.5.4/bullmq/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-14 14:01:50.000000 bullmq-0.5.4/bullmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/backoffs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:52.106907 bullmq-0.5.4/bullmq/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/addJob-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/changeDelay-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/changePriority-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/drain-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/getState-7.lua
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/getStateV2-7.lua
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/moveJobFromActiveToWait-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/moveStalledJobsToWait-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/moveToActive-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/moveToDelayed-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/moveToFinished-12.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/moveToWaitingChildren-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/pause-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/promote-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/reprocessJob-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/retryJob-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/retryJobs-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/saveStacktrace-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/updateData-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-14 14:01:13.000000 bullmq-0.5.4/bullmq/commands/updateProgress-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/redis_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    16635 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:52.110907 bullmq-0.5.4/bullmq/types/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/types/backoff_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/types/job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/types/keep_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/types/queue_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/types/retry_job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/types/worker_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-06-14 14:00:25.000000 bullmq-0.5.4/bullmq/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 14:01:52.102907 bullmq-0.5.4/bullmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-14 14:01:52.000000 bullmq-0.5.4/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-14 14:01:52.000000 bullmq-0.5.4/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 14:01:52.000000 bullmq-0.5.4/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-14 14:01:52.000000 bullmq-0.5.4/bullmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 14:01:52.000000 bullmq-0.5.4/bullmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-14 14:01:52.110907 bullmq-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-14 14:00:25.000000 bullmq-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:50:45.505620 bullmq-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-16 16:50:45.505620 bullmq-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-16 16:48:49.000000 bullmq-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:50:45.497620 bullmq-0.5.5/bullmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-16 16:50:43.000000 bullmq-0.5.5/bullmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/backoffs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:50:45.505620 bullmq-0.5.5/bullmq/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/addJob-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/changeDelay-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/changePriority-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/cleanJobsInSet-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/drain-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/extendLock-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/getCounts-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/getRanges-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/getState-7.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/getStateV2-7.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/isFinished-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/isJobInList-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/moveJobFromActiveToWait-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/moveStalledJobsToWait-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/moveToActive-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/moveToDelayed-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    21811 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/moveToFinished-12.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/moveToWaitingChildren-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/obliterate-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/pause-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/promote-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/releaseLock-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/removeJob-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/removeRepeatable-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/reprocessJob-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/retryJob-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/retryJobs-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/saveStacktrace-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/updateData-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-16 16:50:14.000000 bullmq-0.5.5/bullmq/commands/updateProgress-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/redis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16635 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:50:45.505620 bullmq-0.5.5/bullmq/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/types/backoff_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/types/job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/types/keep_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/types/queue_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/types/retry_job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/types/worker_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-06-16 16:48:49.000000 bullmq-0.5.5/bullmq/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:50:45.497620 bullmq-0.5.5/bullmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-16 16:50:45.000000 bullmq-0.5.5/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-16 16:50:45.000000 bullmq-0.5.5/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:50:45.000000 bullmq-0.5.5/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-16 16:50:45.000000 bullmq-0.5.5/bullmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 16:50:45.000000 bullmq-0.5.5/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-16 16:50:45.509620 bullmq-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-16 16:48:49.000000 bullmq-0.5.5/setup.py
```

### Comparing `bullmq-0.5.4/PKG-INFO` & `bullmq-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 0.5.4
+Version: 0.5.5
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-0.5.4/README.md` & `bullmq-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/backoffs.py` & `bullmq-0.5.5/bullmq/backoffs.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/commands/addJob-8.lua` & `bullmq-0.5.5/bullmq/commands/addJob-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/commands/changeDelay-3.lua` & `bullmq-0.5.5/bullmq/commands/changeDelay-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/commands/changePriority-4.lua` & `bullmq-0.5.5/bullmq/commands/changePriority-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/commands/cleanJobsInSet-2.lua` & `bullmq-0.5.5/bullmq/commands/cleanJobsInSet-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/commands/drain-4.lua` & `bullmq-0.5.5/bullmq/commands/drain-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/commands/getCounts-1.lua` & `bullmq-0.5.5/bullmq/commands/getCounts-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/commands/getRanges-1.lua` & `bullmq-0.5.5/bullmq/commands/getRanges-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/commands/getState-7.lua` & `bullmq-0.5.5/bullmq/commands/getState-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/commands/getStateV2-7.lua` & `bullmq-0.5.5/bullmq/commands/getStateV2-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/commands/isFinished-3.lua` & `bullmq-0.5.5/bullmq/commands/isFinished-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/commands/moveJobFromActiveToWait-9.lua` & `bullmq-0.5.5/bullmq/commands/moveJobFromActiveToWait-9.lua`

 * *Files 9% similar despite different names*

```diff
@@ -13,21 +13,22 @@
     ARGV[1] job id
     ARGV[2] lock token
     ARGV[3] job id key
 ]]
 local rcall = redis.call
 -- Includes
 --[[
-  Function to add job considering priority.
+  Function to add push back job considering priority in front of same prioritized jobs.
 ]]
-local function addJobWithPriority(priorityKey, priority, targetKey, jobId)
+local function pushBackJobWithPriority(priorityKey, priority, targetKey, jobId)
   rcall("ZADD", priorityKey, priority, jobId)
-  local count = rcall("ZCOUNT", priorityKey, 0, priority)
+  local count = rcall("ZCOUNT", priorityKey, 0, priority-1)
   local len = rcall("LLEN", targetKey)
-  local id = rcall("LINDEX", targetKey, len - (count - 1))
+  local id = rcall("LINDEX", targetKey, len - count)
+  rcall("ZADD", priorityKey, priority, jobId)
   if id then
     rcall("LINSERT", targetKey, "BEFORE", id, jobId)
   else
     rcall("RPUSH", targetKey, jobId)
   end
 end
 --[[
@@ -49,15 +50,15 @@
 if lockToken == token and pttl > 0 then
   local removed = rcall("LREM", KEYS[1], 1, jobId)
   if (removed > 0) then
     local target = getTargetQueueList(KEYS[6], KEYS[2], KEYS[5])
     rcall("SREM", KEYS[3], jobId)
     local priority = tonumber(rcall("HGET", ARGV[3], "priority")) or 0
     if priority > 0 then
-      addJobWithPriority(KEYS[8], priority, target, jobId)
+      pushBackJobWithPriority(KEYS[8], priority, target, jobId)
     else
       rcall("RPUSH", target, jobId)
     end
     rcall("DEL", lockKey)
     -- Emit waiting event
     rcall("XADD", KEYS[9], "*", "event", "waiting", "jobId", jobId)
   end
```

### Comparing `bullmq-0.5.4/bullmq/commands/moveStalledJobsToWait-8.lua` & `bullmq-0.5.5/bullmq/commands/moveStalledJobsToWait-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/commands/moveToActive-9.lua` & `bullmq-0.5.5/bullmq/commands/moveToActive-9.lua`

 * *Files 8% similar despite different names*

```diff
@@ -39,41 +39,62 @@
     -- Rate limiting
     keys[6] rate limiter key
     keys[7] delayed key
     opts - token - lock token
     opts - lockDuration
     opts - limiter
 ]]
+-- Includes
+--[[
+  Function to add push back job considering priority in front of same prioritized jobs.
+]]
+local function pushBackJobWithPriority(priorityKey, priority, targetKey, jobId)
+  rcall("ZADD", priorityKey, priority, jobId)
+  local count = rcall("ZCOUNT", priorityKey, 0, priority-1)
+  local len = rcall("LLEN", targetKey)
+  local id = rcall("LINDEX", targetKey, len - count)
+  rcall("ZADD", priorityKey, priority, jobId)
+  if id then
+    rcall("LINSERT", targetKey, "BEFORE", id, jobId)
+  else
+    rcall("RPUSH", targetKey, jobId)
+  end
+end
 local function moveJobFromWaitToActive(keys, keyPrefix, targetKey, jobId, processedOn,
     maxJobs, expireTime, opts)
+  rcall("ZREM", keys[3], jobId) -- remove from priority
+  local jobKey = keyPrefix .. jobId
   -- Check if we need to perform rate limiting.
   if maxJobs then
     local rateLimiterKey = keys[6];
-    local jobCounter = tonumber(rcall("INCR", rateLimiterKey))
-    if jobCounter == 1 then
-      local limiterDuration = opts['limiter'] and opts['limiter']['duration']
-      local integerDuration = math.floor(math.abs(limiterDuration))
-      rcall("PEXPIRE", rateLimiterKey, integerDuration)
-    end
     -- check if we passed rate limit, we need to remove the job and return expireTime
     if expireTime > 0 then
       -- remove from active queue and add back to the wait list
       rcall("LREM", keys[2], 1, jobId)
-      rcall("RPUSH", targetKey, jobId)
+      local priority = tonumber(rcall("HGET", jobKey, "priority")) or 0
+      if priority > 0 then
+        pushBackJobWithPriority(keys[3], priority, targetKey, jobId)
+      else
+        rcall("RPUSH", targetKey, jobId)
+      end
       -- Return when we can process more jobs
       return {0, 0, expireTime, 0}
     end
+    local jobCounter = tonumber(rcall("INCR", rateLimiterKey))
+    if jobCounter == 1 then
+      local limiterDuration = opts['limiter'] and opts['limiter']['duration']
+      local integerDuration = math.floor(math.abs(limiterDuration))
+      rcall("PEXPIRE", rateLimiterKey, integerDuration)
+    end
   end
-  local jobKey = keyPrefix .. jobId
   local lockKey = jobKey .. ':lock'
   -- get a lock
   if opts['token'] ~= "0" then
     rcall("SET", lockKey, opts['token'], "PX", opts['lockDuration'])
   end
-  rcall("ZREM", keys[3], jobId) -- remove from priority
   rcall("XADD", keys[4], "*", "event", "active", "jobId", jobId, "prev", "waiting")
   rcall("HSET", jobKey, "processedOn", processedOn)
   rcall("HINCRBY", jobKey, "attemptsMade", 1)
   return {rcall("HGETALL", jobKey), jobId, 0, 0} -- get job data
 end
 --[[
   Function to return the next delayed job timestamp.
```

### Comparing `bullmq-0.5.4/bullmq/commands/moveToDelayed-8.lua` & `bullmq-0.5.5/bullmq/commands/moveToDelayed-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/commands/moveToFinished-12.lua` & `bullmq-0.5.5/bullmq/commands/moveToFinished-12.lua`

 * *Files 5% similar despite different names*

```diff
@@ -123,41 +123,62 @@
     -- Rate limiting
     keys[6] rate limiter key
     keys[7] delayed key
     opts - token - lock token
     opts - lockDuration
     opts - limiter
 ]]
+-- Includes
+--[[
+  Function to add push back job considering priority in front of same prioritized jobs.
+]]
+local function pushBackJobWithPriority(priorityKey, priority, targetKey, jobId)
+  rcall("ZADD", priorityKey, priority, jobId)
+  local count = rcall("ZCOUNT", priorityKey, 0, priority-1)
+  local len = rcall("LLEN", targetKey)
+  local id = rcall("LINDEX", targetKey, len - count)
+  rcall("ZADD", priorityKey, priority, jobId)
+  if id then
+    rcall("LINSERT", targetKey, "BEFORE", id, jobId)
+  else
+    rcall("RPUSH", targetKey, jobId)
+  end
+end
 local function moveJobFromWaitToActive(keys, keyPrefix, targetKey, jobId, processedOn,
     maxJobs, expireTime, opts)
+  rcall("ZREM", keys[3], jobId) -- remove from priority
+  local jobKey = keyPrefix .. jobId
   -- Check if we need to perform rate limiting.
   if maxJobs then
     local rateLimiterKey = keys[6];
-    local jobCounter = tonumber(rcall("INCR", rateLimiterKey))
-    if jobCounter == 1 then
-      local limiterDuration = opts['limiter'] and opts['limiter']['duration']
-      local integerDuration = math.floor(math.abs(limiterDuration))
-      rcall("PEXPIRE", rateLimiterKey, integerDuration)
-    end
     -- check if we passed rate limit, we need to remove the job and return expireTime
     if expireTime > 0 then
       -- remove from active queue and add back to the wait list
       rcall("LREM", keys[2], 1, jobId)
-      rcall("RPUSH", targetKey, jobId)
+      local priority = tonumber(rcall("HGET", jobKey, "priority")) or 0
+      if priority > 0 then
+        pushBackJobWithPriority(keys[3], priority, targetKey, jobId)
+      else
+        rcall("RPUSH", targetKey, jobId)
+      end
       -- Return when we can process more jobs
       return {0, 0, expireTime, 0}
     end
+    local jobCounter = tonumber(rcall("INCR", rateLimiterKey))
+    if jobCounter == 1 then
+      local limiterDuration = opts['limiter'] and opts['limiter']['duration']
+      local integerDuration = math.floor(math.abs(limiterDuration))
+      rcall("PEXPIRE", rateLimiterKey, integerDuration)
+    end
   end
-  local jobKey = keyPrefix .. jobId
   local lockKey = jobKey .. ':lock'
   -- get a lock
   if opts['token'] ~= "0" then
     rcall("SET", lockKey, opts['token'], "PX", opts['lockDuration'])
   end
-  rcall("ZREM", keys[3], jobId) -- remove from priority
   rcall("XADD", keys[4], "*", "event", "active", "jobId", jobId, "prev", "waiting")
   rcall("HSET", jobKey, "processedOn", processedOn)
   rcall("HINCRBY", jobKey, "attemptsMade", 1)
   return {rcall("HGETALL", jobKey), jobId, 0, 0} -- get job data
 end
 --[[
   Function to recursively move from waitingChildren to failed.
```

### Comparing `bullmq-0.5.4/bullmq/commands/moveToWaitingChildren-4.lua` & `bullmq-0.5.5/bullmq/commands/moveToWaitingChildren-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/commands/obliterate-2.lua` & `bullmq-0.5.5/bullmq/commands/obliterate-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/commands/promote-6.lua` & `bullmq-0.5.5/bullmq/commands/promote-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/commands/removeJob-1.lua` & `bullmq-0.5.5/bullmq/commands/removeJob-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/commands/removeRepeatable-2.lua` & `bullmq-0.5.5/bullmq/commands/removeRepeatable-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/commands/reprocessJob-6.lua` & `bullmq-0.5.5/bullmq/commands/reprocessJob-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/commands/retryJob-8.lua` & `bullmq-0.5.5/bullmq/commands/retryJob-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/commands/retryJobs-6.lua` & `bullmq-0.5.5/bullmq/commands/retryJobs-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/event_emitter.py` & `bullmq-0.5.5/bullmq/event_emitter.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/job.py` & `bullmq-0.5.5/bullmq/job.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/queue.py` & `bullmq-0.5.5/bullmq/queue.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/redis_connection.py` & `bullmq-0.5.5/bullmq/redis_connection.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/scripts.py` & `bullmq-0.5.5/bullmq/scripts.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/timer.py` & `bullmq-0.5.5/bullmq/timer.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/types/job_options.py` & `bullmq-0.5.5/bullmq/types/job_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/types/worker_options.py` & `bullmq-0.5.5/bullmq/types/worker_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq/worker.py` & `bullmq-0.5.5/bullmq/worker.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/bullmq.egg-info/PKG-INFO` & `bullmq-0.5.5/bullmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 0.5.4
+Version: 0.5.5
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-0.5.4/bullmq.egg-info/SOURCES.txt` & `bullmq-0.5.5/bullmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.4/setup.py` & `bullmq-0.5.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     install_requires=[
         'redis',
         'msgpack',
         'semver',
     ],
     extras_require={
         "dev": [
-            "pre-commit==3.3.2",
+            "pre-commit==3.3.3",
             "python-semantic-release==7.34.3",
         ]
     },
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
```

