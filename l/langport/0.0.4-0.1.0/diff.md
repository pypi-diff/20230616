# Comparing `tmp/langport-0.0.4.tar.gz` & `tmp/langport-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langport-0.0.4.tar", last modified: Fri May 26 08:53:01 2023, max compression
+gzip compressed data, was "langport-0.1.0.tar", last modified: Fri Jun 16 07:21:30 2023, max compression
```

## Comparing `langport-0.0.4.tar` & `langport-0.1.0.tar`

### file list

```diff
@@ -1,119 +1,138 @@
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:53:01.909212 langport-0.0.4/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1068 2023-05-10 14:48:47.000000 langport-0.0.4/LICENSE
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3825 2023-05-26 08:53:01.909212 langport-0.0.4/PKG-INFO
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3370 2023-05-26 08:52:20.000000 langport-0.0.4/README.md
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:53:01.901212 langport-0.0.4/langport/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:31:47.000000 langport-0.0.4/langport/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      626 2023-05-24 15:12:40.000000 langport-0.0.4/langport/constants.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:53:01.901212 langport-0.0.4/langport/core/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 16:59:08.000000 langport-0.0.4/langport/core/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2540 2023-05-23 04:14:03.000000 langport-0.0.4/langport/core/base_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    13055 2023-05-25 14:06:55.000000 langport-0.0.4/langport/core/cluster_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6852 2023-05-25 13:35:01.000000 langport-0.0.4/langport/core/cluster_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      364 2023-05-23 04:14:03.000000 langport-0.0.4/langport/core/dispatch.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:53:01.901212 langport-0.0.4/langport/data/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:56:40.000000 langport-0.0.4/langport/data/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:53:01.901212 langport-0.0.4/langport/data/conversation/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5684 2023-05-26 06:52:11.000000 langport-0.0.4/langport/data/conversation/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1115 2023-05-24 09:57:36.000000 langport-0.0.4/langport/data/conversation/conversation_settings.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:53:01.901212 langport-0.0.4/langport/data/conversation/settings/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-24 09:29:33.000000 langport-0.0.4/langport/data/conversation/settings/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-05-24 13:17:01.000000 langport-0.0.4/langport/data/conversation/settings/baize.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      194 2023-05-24 09:59:51.000000 langport-0.0.4/langport/data/conversation/settings/bard.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      264 2023-05-24 10:00:06.000000 langport-0.0.4/langport/data/conversation/settings/billa.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      288 2023-05-26 06:54:17.000000 langport-0.0.4/langport/data/conversation/settings/chatgpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-05-24 10:01:03.000000 langport-0.0.4/langport/data/conversation/settings/claude.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-05-24 10:01:14.000000 langport-0.0.4/langport/data/conversation/settings/dolly.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      244 2023-05-24 10:01:23.000000 langport-0.0.4/langport/data/conversation/settings/h2ogpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      273 2023-05-24 10:01:33.000000 langport-0.0.4/langport/data/conversation/settings/koala.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      310 2023-05-24 10:01:44.000000 langport-0.0.4/langport/data/conversation/settings/oasst_pythia.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      265 2023-05-24 10:01:57.000000 langport-0.0.4/langport/data/conversation/settings/one_shot.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      267 2023-05-24 10:02:05.000000 langport-0.0.4/langport/data/conversation/settings/openbuddy.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      259 2023-05-24 10:02:15.000000 langport-0.0.4/langport/data/conversation/settings/phoenix.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      272 2023-05-24 10:02:22.000000 langport-0.0.4/langport/data/conversation/settings/redpajama.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-05-24 10:02:29.000000 langport-0.0.4/langport/data/conversation/settings/rwkv.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      328 2023-05-24 10:02:37.000000 langport-0.0.4/langport/data/conversation/settings/stablelm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      282 2023-05-24 10:02:45.000000 langport-0.0.4/langport/data/conversation/settings/vicuna.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      268 2023-05-24 10:02:53.000000 langport-0.0.4/langport/data/conversation/settings/zero_shot.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:53:01.905212 langport-0.0.4/langport/model/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 15:10:39.000000 langport-0.0.4/langport/model/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:53:01.905212 langport-0.0.4/langport/model/adapters/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:31:13.000000 langport-0.0.4/langport/model/adapters/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1383 2023-05-24 10:05:59.000000 langport-0.0.4/langport/model/adapters/baize.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      815 2023-05-24 10:10:17.000000 langport-0.0.4/langport/model/adapters/bard.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      701 2023-05-24 13:06:10.000000 langport-0.0.4/langport/model/adapters/billa.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      598 2023-05-24 13:06:30.000000 langport-0.0.4/langport/model/adapters/chatglm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      793 2023-05-26 07:07:02.000000 langport-0.0.4/langport/model/adapters/chatgpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      749 2023-05-24 13:08:03.000000 langport-0.0.4/langport/model/adapters/claude.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1257 2023-05-24 13:08:43.000000 langport-0.0.4/langport/model/adapters/dolly_v2.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      660 2023-05-24 13:09:13.000000 langport-0.0.4/langport/model/adapters/koala.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1151 2023-05-24 13:09:46.000000 langport-0.0.4/langport/model/adapters/oasst_pythia.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2043 2023-05-24 13:10:32.000000 langport-0.0.4/langport/model/adapters/openbuddy.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1251 2023-05-24 13:11:20.000000 langport-0.0.4/langport/model/adapters/phoenix.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1015 2023-05-24 13:11:57.000000 langport-0.0.4/langport/model/adapters/rwkv.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1555 2023-05-24 13:12:30.000000 langport-0.0.4/langport/model/adapters/stable_lm.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      610 2023-05-24 09:29:33.000000 langport-0.0.4/langport/model/adapters/t5.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2060 2023-05-24 13:13:27.000000 langport-0.0.4/langport/model/adapters/vicuna.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7171 2023-05-23 04:14:03.000000 langport-0.0.4/langport/model/compression.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:53:01.905212 langport-0.0.4/langport/model/executor/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-23 04:14:03.000000 langport-0.0.4/langport/model/executor/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1739 2023-05-26 07:23:50.000000 langport-0.0.4/langport/model/executor/base.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:53:01.905212 langport-0.0.4/langport/model/executor/embedding/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      984 2023-05-23 04:14:03.000000 langport-0.0.4/langport/model/executor/embedding/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5205 2023-05-26 06:41:44.000000 langport-0.0.4/langport/model/executor/embedding/huggingface.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:53:01.905212 langport-0.0.4/langport/model/executor/generation/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      887 2023-05-23 04:14:03.000000 langport-0.0.4/langport/model/executor/generation/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4505 2023-05-26 07:24:56.000000 langport-0.0.4/langport/model/executor/generation/chatgpt.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    12841 2023-05-26 06:41:59.000000 langport-0.0.4/langport/model/executor/generation/huggingface.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3957 2023-05-26 07:26:41.000000 langport-0.0.4/langport/model/executor/huggingface_utils.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3387 2023-05-25 10:30:42.000000 langport-0.0.4/langport/model/model_adapter.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1164 2023-05-25 13:11:00.000000 langport-0.0.4/langport/model/model_args.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:53:01.905212 langport-0.0.4/langport/model/models/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:40:16.000000 langport-0.0.4/langport/model/models/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      996 2023-05-11 08:40:28.000000 langport-0.0.4/langport/model/models/rwkv_model.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4163 2023-05-23 04:14:03.000000 langport-0.0.4/langport/model/monkey_patch_non_inplace.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:53:01.905212 langport-0.0.4/langport/protocol/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:14.000000 langport-0.0.4/langport/protocol/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        8 2023-05-11 09:58:58.000000 langport-0.0.4/langport/protocol/fauxpilot_api_protocol.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4477 2023-05-14 15:31:14.000000 langport-0.0.4/langport/protocol/openai_api_protocol.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2726 2023-05-26 07:00:41.000000 langport-0.0.4/langport/protocol/worker_protocol.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:53:01.905212 langport-0.0.4/langport/routers/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:44:40.000000 langport-0.0.4/langport/routers/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:53:01.905212 langport-0.0.4/langport/routers/gateway/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:44:59.000000 langport-0.0.4/langport/routers/gateway/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:53:01.905212 langport-0.0.4/langport/routers/server/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:44:59.000000 langport-0.0.4/langport/routers/server/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2106 2023-05-23 08:00:25.000000 langport-0.0.4/langport/routers/server/core_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      544 2023-05-23 04:14:03.000000 langport-0.0.4/langport/routers/server/embedding_node.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3486 2023-05-23 04:14:03.000000 langport-0.0.4/langport/routers/server/generation_node.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:53:01.905212 langport-0.0.4/langport/service/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:01.000000 langport-0.0.4/langport/service/__init__.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:53:01.905212 langport-0.0.4/langport/service/gateway/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-23 04:14:03.000000 langport-0.0.4/langport/service/gateway/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5201 2023-05-23 04:14:03.000000 langport-0.0.4/langport/service/gateway/fauxpilot_api.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    25418 2023-05-26 07:15:03.000000 langport-0.0.4/langport/service/gateway/openai_api.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:53:01.905212 langport-0.0.4/langport/service/server/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-23 04:14:03.000000 langport-0.0.4/langport/service/server/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2382 2023-05-26 08:45:55.000000 langport-0.0.4/langport/service/server/chatgpt_generation_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1210 2023-05-26 08:46:05.000000 langport-0.0.4/langport/service/server/dummy_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2721 2023-05-26 08:45:35.000000 langport-0.0.4/langport/service/server/embedding_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2756 2023-05-26 08:45:42.000000 langport-0.0.4/langport/service/server/generation_worker.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:53:01.909212 langport-0.0.4/langport/utils/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7172 2023-05-14 15:31:14.000000 langport-0.0.4/langport/utils/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      508 2023-05-23 04:14:03.000000 langport-0.0.4/langport/utils/cache_state.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2568 2023-05-23 04:14:03.000000 langport-0.0.4/langport/utils/evaluation.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      552 2023-05-23 04:14:03.000000 langport-0.0.4/langport/utils/http_pool.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2207 2023-05-23 04:14:03.000000 langport-0.0.4/langport/utils/interval_timer.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       26 2023-05-26 08:51:08.000000 langport-0.0.4/langport/version.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:53:01.909212 langport-0.0.4/langport/workers/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-23 04:14:03.000000 langport-0.0.4/langport/workers/__init__.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3167 2023-05-23 10:24:47.000000 langport-0.0.4/langport/workers/embedding_worker.py
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3835 2023-05-25 13:37:50.000000 langport-0.0.4/langport/workers/generation_worker.py
-drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:53:01.901212 langport-0.0.4/langport.egg-info/
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3825 2023-05-26 08:53:01.000000 langport-0.0.4/langport.egg-info/PKG-INFO
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3481 2023-05-26 08:53:01.000000 langport-0.0.4/langport.egg-info/SOURCES.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        1 2023-05-26 08:53:01.000000 langport-0.0.4/langport.egg-info/dependency_links.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      215 2023-05-26 08:53:01.000000 langport-0.0.4/langport.egg-info/requires.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       14 2023-05-26 08:53:01.000000 langport-0.0.4/langport.egg-info/top_level.txt
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1057 2023-05-26 08:51:12.000000 langport-0.0.4/pyproject.toml
--rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       38 2023-05-26 08:53:01.909212 langport-0.0.4/setup.cfg
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.127148 langport-0.1.0/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1068 2023-05-10 14:48:47.000000 langport-0.1.0/LICENSE
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5396 2023-06-16 07:21:30.127148 langport-0.1.0/PKG-INFO
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4916 2023-06-16 07:20:16.000000 langport-0.1.0/README.md
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.115149 langport-0.1.0/langport/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-26 08:31:47.000000 langport-0.1.0/langport/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      588 2023-06-12 17:00:54.000000 langport-0.1.0/langport/constants.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.115149 langport-0.1.0/langport/core/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 16:59:08.000000 langport-0.1.0/langport/core/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2195 2023-06-16 07:20:16.000000 langport-0.1.0/langport/core/base_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    12807 2023-06-16 07:20:16.000000 langport-0.1.0/langport/core/cluster_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6252 2023-06-16 07:20:16.000000 langport-0.1.0/langport/core/cluster_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      364 2023-06-12 17:00:54.000000 langport-0.1.0/langport/core/dispatch.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.115149 langport-0.1.0/langport/data/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:56:40.000000 langport-0.1.0/langport/data/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.115149 langport-0.1.0/langport/data/conversation/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5684 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1115 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/conversation_settings.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.119149 langport-0.1.0/langport/data/conversation/settings/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/baize.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      194 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/bard.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      264 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/billa.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      288 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/chatgpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/claude.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      293 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/dolly.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      315 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/falcon.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      244 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/h2ogpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      273 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/koala.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      271 2023-06-16 07:20:16.000000 langport-0.1.0/langport/data/conversation/settings/llama_cpp.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      320 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/mpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      310 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/oasst_pythia.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      265 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/one_shot.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      267 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/openbuddy.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      259 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/phoenix.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      272 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/redpajama.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      266 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/rwkv.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      328 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/stablelm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      282 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/vicuna.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      268 2023-06-12 17:00:54.000000 langport-0.1.0/langport/data/conversation/settings/zero_shot.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.119149 langport-0.1.0/langport/model/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 15:10:39.000000 langport-0.1.0/langport/model/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.123149 langport-0.1.0/langport/model/adapters/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:31:13.000000 langport-0.1.0/langport/model/adapters/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1383 2023-06-12 17:00:54.000000 langport-0.1.0/langport/model/adapters/baize.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      705 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/bard.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      701 2023-06-12 17:00:54.000000 langport-0.1.0/langport/model/adapters/billa.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      280 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/chatglm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/chatgpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      639 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/claude.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      442 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/codegen.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      841 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/dolly_v2.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      683 2023-06-12 17:00:54.000000 langport-0.1.0/langport/model/adapters/falcon.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      660 2023-06-12 17:00:54.000000 langport-0.1.0/langport/model/adapters/koala.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1377 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/llama_cpp.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      806 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/oasst_pythia.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1577 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/openbuddy.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      906 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/phoenix.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      694 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/rwkv.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1210 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/stable_lm.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      303 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/starcoder.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      291 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/t5.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      215 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/text2vec.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1664 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/adapters/vicuna.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7171 2023-06-12 17:00:54.000000 langport-0.1.0/langport/model/compression.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.123149 langport-0.1.0/langport/model/executor/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.1.0/langport/model/executor/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1739 2023-06-12 17:00:54.000000 langport-0.1.0/langport/model/executor/base.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.123149 langport-0.1.0/langport/model/executor/embedding/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      984 2023-06-12 17:00:54.000000 langport-0.1.0/langport/model/executor/embedding/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5816 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/executor/embedding/huggingface.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.123149 langport-0.1.0/langport/model/executor/generation/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3482 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/executor/generation/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4505 2023-06-12 17:00:54.000000 langport-0.1.0/langport/model/executor/generation/chatgpt.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    15561 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/executor/generation/huggingface.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4463 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/executor/generation/llamacpp.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7037 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/executor/huggingface.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      909 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/executor/llamacpp.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3070 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/model_adapter.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1272 2023-06-16 07:20:16.000000 langport-0.1.0/langport/model/model_args.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.123149 langport-0.1.0/langport/model/models/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-11 08:40:16.000000 langport-0.1.0/langport/model/models/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      996 2023-05-11 08:40:28.000000 langport-0.1.0/langport/model/models/rwkv_model.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4163 2023-06-12 17:00:54.000000 langport-0.1.0/langport/model/monkey_patch_non_inplace.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.123149 langport-0.1.0/langport/protocol/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:14.000000 langport-0.1.0/langport/protocol/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    10174 2023-06-12 17:00:54.000000 langport-0.1.0/langport/protocol/huggingface_api_protocol.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4477 2023-05-14 15:31:14.000000 langport-0.1.0/langport/protocol/openai_api_protocol.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3283 2023-06-12 17:00:54.000000 langport-0.1.0/langport/protocol/tabby_api_protocol.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2726 2023-06-12 17:00:54.000000 langport-0.1.0/langport/protocol/worker_protocol.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.123149 langport-0.1.0/langport/routers/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.1.0/langport/routers/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.123149 langport-0.1.0/langport/routers/gateway/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.1.0/langport/routers/gateway/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     6901 2023-06-16 07:20:16.000000 langport-0.1.0/langport/routers/gateway/common.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)    16376 2023-06-12 17:00:54.000000 langport-0.1.0/langport/routers/gateway/openai_compatible.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.123149 langport-0.1.0/langport/routers/server/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.1.0/langport/routers/server/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1781 2023-06-16 07:20:16.000000 langport-0.1.0/langport/routers/server/core_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      544 2023-06-12 17:00:54.000000 langport-0.1.0/langport/routers/server/embedding_node.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3486 2023-06-12 17:00:54.000000 langport-0.1.0/langport/routers/server/generation_node.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.123149 langport-0.1.0/langport/service/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-05-10 14:53:01.000000 langport-0.1.0/langport/service/__init__.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.127148 langport-0.1.0/langport/service/gateway/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.1.0/langport/service/gateway/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      955 2023-06-16 07:20:16.000000 langport-0.1.0/langport/service/gateway/cluster_monitor.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1510 2023-06-16 07:20:16.000000 langport-0.1.0/langport/service/gateway/cluster_monitor_app.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3842 2023-06-16 07:20:16.000000 langport-0.1.0/langport/service/gateway/fauxpilot_api.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2499 2023-06-16 07:20:16.000000 langport-0.1.0/langport/service/gateway/graphite_feeder.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5693 2023-06-16 07:20:16.000000 langport-0.1.0/langport/service/gateway/huggingface_api.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5714 2023-06-16 07:20:16.000000 langport-0.1.0/langport/service/gateway/openai_api.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5664 2023-06-16 07:20:16.000000 langport-0.1.0/langport/service/gateway/tabby_api.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.127148 langport-0.1.0/langport/service/server/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.1.0/langport/service/server/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2187 2023-06-16 07:20:16.000000 langport-0.1.0/langport/service/server/chatgpt_generation_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1107 2023-06-16 07:20:16.000000 langport-0.1.0/langport/service/server/dummy_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2693 2023-06-16 07:20:16.000000 langport-0.1.0/langport/service/server/embedding_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2610 2023-06-16 07:20:16.000000 langport-0.1.0/langport/service/server/generation_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2830 2023-06-16 07:20:16.000000 langport-0.1.0/langport/service/server/ggml_generation_worker.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.127148 langport-0.1.0/langport/utils/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     7261 2023-06-16 07:20:16.000000 langport-0.1.0/langport/utils/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      508 2023-06-12 17:00:54.000000 langport-0.1.0/langport/utils/cache_state.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2568 2023-06-12 17:00:54.000000 langport-0.1.0/langport/utils/evaluation.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      641 2023-06-16 07:20:16.000000 langport-0.1.0/langport/utils/http_pool.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     2332 2023-06-16 07:20:16.000000 langport-0.1.0/langport/utils/interval_timer.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       27 2023-06-16 07:20:16.000000 langport-0.1.0/langport/version.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.127148 langport-0.1.0/langport/workers/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        0 2023-06-12 17:00:54.000000 langport-0.1.0/langport/workers/__init__.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3068 2023-06-16 07:20:16.000000 langport-0.1.0/langport/workers/embedding_worker.py
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     3176 2023-06-16 07:20:16.000000 langport-0.1.0/langport/workers/generation_worker.py
+drwxrwxr-x   0 wangjun   (1001) wangjun   (1001)        0 2023-06-16 07:21:30.115149 langport-0.1.0/langport.egg-info/
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     5396 2023-06-16 07:21:30.000000 langport-0.1.0/langport.egg-info/PKG-INFO
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     4266 2023-06-16 07:21:30.000000 langport-0.1.0/langport.egg-info/SOURCES.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)        1 2023-06-16 07:21:30.000000 langport-0.1.0/langport.egg-info/dependency_links.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)      244 2023-06-16 07:21:30.000000 langport-0.1.0/langport.egg-info/requires.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       14 2023-06-16 07:21:30.000000 langport-0.1.0/langport.egg-info/top_level.txt
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)     1089 2023-06-16 07:21:09.000000 langport-0.1.0/pyproject.toml
+-rw-rw-r--   0 wangjun   (1001) wangjun   (1001)       38 2023-06-16 07:21:30.127148 langport-0.1.0/setup.cfg
```

### Comparing `langport-0.0.4/LICENSE` & `langport-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `langport-0.0.4/PKG-INFO` & `langport-0.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,240 +1,308 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6c61 6e67  : 2.1.Name: lang
-00000020: 706f 7274 0a56 6572 7369 6f6e 3a20 302e  port.Version: 0.
-00000030: 302e 340a 5375 6d6d 6172 793a 2041 206c  0.4.Summary: A l
-00000040: 6172 6765 206c 616e 6775 6167 6520 6d6f  arge language mo
-00000050: 6465 6c20 7365 7276 696e 6720 706c 6174  del serving plat
-00000060: 666f 726d 2e0a 5072 6f6a 6563 742d 5552  form..Project-UR
-00000070: 4c3a 2048 6f6d 6570 6167 652c 2068 7474  L: Homepage, htt
-00000080: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000090: 7674 7562 6572 2d70 6c61 6e2f 6c61 6e67  vtuber-plan/lang
-000000a0: 706f 7274 0a50 726f 6a65 6374 2d55 524c  port.Project-URL
-000000b0: 3a20 4275 6720 5472 6163 6b65 722c 2068  : Bug Tracker, h
-000000c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000000d0: 6d2f 7674 7562 6572 2d70 6c61 6e2f 6c61  m/vtuber-plan/la
-000000e0: 6e67 706f 7274 2f69 7373 7565 730a 436c  ngport/issues.Cl
-000000f0: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
-00000100: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000110: 3a20 5079 7468 6f6e 203a 3a20 330a 436c  : Python :: 3.Cl
-00000120: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
-00000130: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-00000140: 6420 3a3a 2041 7061 6368 6520 536f 6674  d :: Apache Soft
-00000150: 7761 7265 204c 6963 656e 7365 0a52 6571  ware License.Req
-00000160: 7569 7265 732d 5079 7468 6f6e 3a20 3e3d  uires-Python: >=
-00000170: 332e 380a 4465 7363 7269 7074 696f 6e2d  3.8.Description-
-00000180: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
-00000190: 7874 2f6d 6172 6b64 6f77 6e0a 5072 6f76  xt/markdown.Prov
-000001a0: 6964 6573 2d45 7874 7261 3a20 6465 760a  ides-Extra: dev.
-000001b0: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
-000001c0: 4345 4e53 450a 0a23 206c 616e 6770 6f72  CENSE..# langpor
-000001d0: 740a 4c61 6e67 506f 7274 2069 7320 6120  t.LangPort is a 
-000001e0: 6f70 656e 2d73 6f75 7263 6520 6c61 7267  open-source larg
-000001f0: 6520 6c61 6e67 7561 6765 206d 6f64 656c  e language model
-00000200: 2073 6572 7669 6e67 2070 6c61 7466 6f72   serving platfor
-00000210: 6d2e 0a4f 7572 2067 6f61 6c20 6973 2074  m..Our goal is t
-00000220: 6f20 6275 696c 6420 6120 7375 7065 7220  o build a super 
-00000230: 6661 7374 204c 4c4d 2069 6e66 6572 656e  fast LLM inferen
-00000240: 6365 2073 6572 7669 6365 2e0a 0a54 6869  ce service...Thi
-00000250: 7320 7072 6f6a 6563 7420 6973 2069 6e73  s project is ins
-00000260: 7069 7265 6420 6279 205b 6c6d 7379 732f  pired by [lmsys/
-00000270: 6661 7374 6368 6174 5d28 6874 7470 733a  fastchat](https:
-00000280: 2f2f 6769 7468 7562 2e63 6f6d 2f6c 6d2d  //github.com/lm-
-00000290: 7379 732f 4661 7374 4368 6174 292c 2077  sys/FastChat), w
-000002a0: 6520 686f 7065 2074 6861 7420 7468 6520  e hope that the 
-000002b0: 7365 7276 696e 6720 706c 6174 666f 726d  serving platform
-000002c0: 2069 7320 6c69 6768 7477 6569 6768 7420   is lightweight 
-000002d0: 616e 6420 6661 7374 2c20 6275 7420 6661  and fast, but fa
-000002e0: 7374 6368 6174 2069 6e63 6c75 6465 7320  stchat includes 
-000002f0: 6f74 6865 7220 6665 6174 7572 6573 2073  other features s
-00000300: 7563 6820 6173 2074 7261 696e 696e 6720  uch as training 
-00000310: 616e 6420 6576 616c 7561 7469 6f6e 206d  and evaluation m
-00000320: 616b 6520 6974 2063 6f6d 706c 6963 6174  ake it complicat
-00000330: 6564 2e0a 0a54 6865 2063 6f72 6520 6665  ed...The core fe
-00000340: 6174 7572 6573 2069 6e63 6c75 6465 3a0a  atures include:.
-00000350: 2d20 4120 6469 7374 7269 6275 7465 6420  - A distributed 
-00000360: 7365 7276 696e 6720 7379 7374 656d 2066  serving system f
-00000370: 6f72 2073 7461 7465 2d6f 662d 7468 652d  or state-of-the-
-00000380: 6172 7420 6d6f 6465 6c73 2e0a 2d20 5374  art models..- St
-00000390: 7265 616d 696e 6720 4150 4920 696e 7465  reaming API inte
-000003a0: 7266 6163 6520 7375 7070 6f72 742e 0a2d  rface support..-
-000003b0: 2042 6174 6368 2069 6e66 6572 656e 6365   Batch inference
-000003c0: 2066 6f72 2068 6967 6865 7220 7468 726f   for higher thro
-000003d0: 7567 6870 7574 2e0a 2d20 4f70 656e 4149  ughput..- OpenAI
-000003e0: 2d43 6f6d 7061 7469 626c 6520 5245 5354  -Compatible REST
-000003f0: 6675 6c20 4150 4973 2e0a 2d20 4661 7578  ful APIs..- Faux
-00000400: 5069 6c6f 742d 436f 6d70 6174 6962 6c65  Pilot-Compatible
-00000410: 2052 4553 5466 756c 2041 5049 732e 0a0a   RESTful APIs...
-00000420: 2323 2042 656e 6368 6d61 726b 0a57 6520  ## Benchmark.We 
-00000430: 7573 6520 7369 6e67 6c65 2052 5458 3330  use single RTX30
-00000440: 3930 2074 6f20 7275 6e20 6120 6669 6e65  90 to run a fine
-00000450: 7475 6e65 6420 3742 204c 4c61 4d41 206d  tuned 7B LLaMA m
-00000460: 6f64 656c 2028 4f70 656e 4275 6464 7920  odel (OpenBuddy 
-00000470: 5630 2e39 2920 696e 2074 6865 2062 6631  V0.9) in the bf1
-00000480: 3620 7365 7474 696e 672e 2057 6520 6372  6 setting. We cr
-00000490: 6561 7465 2033 3220 7468 7265 6164 7320  eate 32 threads 
-000004a0: 746f 2073 7562 6d69 7420 6368 6174 2074  to submit chat t
-000004b0: 6173 6b73 2074 6f20 7468 6520 7365 7276  asks to the serv
-000004c0: 6572 2c20 616e 6420 7468 6520 666f 6c6c  er, and the foll
-000004d0: 6f77 696e 6720 6669 6775 7265 2073 686f  owing figure sho
-000004e0: 7773 2074 6865 2051 7565 7269 6573 2050  ws the Queries P
-000004f0: 6572 2053 6563 6f6e 6420 2851 5053 2920  er Second (QPS) 
-00000500: 616e 6420 546f 6b65 6e73 2050 6572 2053  and Tokens Per S
-00000510: 6563 6f6e 6420 2854 5053 2920 6f66 2046  econd (TPS) of F
-00000520: 6173 7443 6861 7420 616e 6420 4c61 6e67  astChat and Lang
-00000530: 506f 7274 2077 6974 6820 6469 6666 6572  Port with differ
-00000540: 656e 7420 6d61 7820 6d6f 6465 6c20 636f  ent max model co
-00000550: 6e63 7572 7265 6e63 7920 7365 7474 696e  ncurrency settin
-00000560: 6773 2e0a 0a21 5b62 656e 6368 6d61 726b  gs...![benchmark
-00000570: 5f63 6861 745d 2864 6f63 732f 6265 6e63  _chat](docs/benc
-00000580: 686d 6172 6b5f 6368 6174 2e6a 7067 290a  hmark_chat.jpg).
-00000590: 0a0a 2323 204e 6577 730a 2d20 5b32 3032  ..## News.- [202
-000005a0: 332f 3035 2f31 305d 204c 616e 6770 6f72  3/05/10] Langpor
-000005b0: 7420 7072 6f6a 6563 7420 7374 6172 7465  t project starte
-000005c0: 642e 0a2d 205b 3230 3233 2f30 352f 3134  d..- [2023/05/14
-000005d0: 5d20 4261 7463 6820 696e 6665 7265 6e63  ] Batch inferenc
-000005e0: 6520 7375 7070 6f72 7465 642e 0a2d 205b  e supported..- [
-000005f0: 3230 3233 2f30 352f 3232 5d20 4e65 7720  2023/05/22] New 
-00000600: 6469 7374 7269 6275 7465 6420 6172 6368  distributed arch
-00000610: 6974 6563 7475 7265 2e0a 2d20 5b32 3032  itecture..- [202
-00000620: 332f 3035 2f32 335d 2041 6464 2063 6861  3/05/23] Add cha
-00000630: 7420 7468 726f 7567 6870 7574 2074 6573  t throughput tes
-00000640: 7420 7363 7269 7074 2e0a 0a0a 2323 2049  t script....## I
-00000650: 6e73 7461 6c6c 0a0a 2323 2320 4d65 7468  nstall..### Meth
-00000660: 6f64 2031 3a20 5769 7468 2070 6970 0a0a  od 1: With pip..
-00000670: 6060 6062 6173 680a 7069 7033 2069 6e73  ```bash.pip3 ins
-00000680: 7461 6c6c 2067 6974 2b68 7474 7073 3a2f  tall git+https:/
-00000690: 2f67 6974 6875 622e 636f 6d2f 7674 7562  /github.com/vtub
-000006a0: 6572 2d70 6c61 6e2f 6c61 6e67 706f 7274  er-plan/langport
-000006b0: 2e67 6974 200a 6060 600a 0a23 2323 204d  .git .```..### M
-000006c0: 6574 686f 6420 323a 2046 726f 6d20 736f  ethod 2: From so
-000006d0: 7572 6365 0a0a 312e 2043 6c6f 6e65 2074  urce..1. Clone t
-000006e0: 6869 7320 7265 706f 7369 746f 7279 0a60  his repository.`
-000006f0: 6060 6261 7368 0a67 6974 2063 6c6f 6e65  ``bash.git clone
-00000700: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000710: 636f 6d2f 7674 7562 6572 2d70 6c61 6e2f  com/vtuber-plan/
-00000720: 6c61 6e67 706f 7274 2e67 6974 0a63 6420  langport.git.cd 
-00000730: 6c61 6e67 706f 7274 0a60 6060 0a0a 322e  langport.```..2.
-00000740: 2049 6e73 7461 6c6c 2074 6865 2050 6163   Install the Pac
-00000750: 6b61 6765 0a60 6060 6261 7368 0a70 6970  kage.```bash.pip
-00000760: 2069 6e73 7461 6c6c 202d 2d75 7067 7261   install --upgra
-00000770: 6465 2070 6970 0a70 6970 2069 6e73 7461  de pip.pip insta
-00000780: 6c6c 202d 6520 2e0a 6060 600a 0a23 2320  ll -e ..```..## 
-00000790: 5374 6172 7420 7468 6520 7365 7276 6572  Start the server
-000007a0: 0a0a 4974 2069 7320 7369 6d70 6c65 2074  ..It is simple t
-000007b0: 6f20 7374 6172 7420 6120 7369 6e67 6c65  o start a single
-000007c0: 206e 6f64 6520 6368 6174 2041 5049 2073   node chat API s
-000007d0: 6572 7669 6365 3a0a 6060 6020 6261 7368  ervice:.``` bash
-000007e0: 0a70 7974 686f 6e20 2d6d 206c 616e 6770  .python -m langp
-000007f0: 6f72 742e 7365 7276 6963 652e 7365 7276  ort.service.serv
-00000800: 6572 2e67 656e 6572 6174 696f 6e5f 776f  er.generation_wo
-00000810: 726b 6572 202d 2d70 6f72 7420 3231 3030  rker --port 2100
-00000820: 3120 2d2d 6d6f 6465 6c2d 7061 7468 203c  1 --model-path <
-00000830: 796f 7572 206d 6f64 656c 2070 6174 683e  your model path>
-00000840: 0a70 7974 686f 6e20 2d6d 206c 616e 6770  .python -m langp
-00000850: 6f72 742e 7365 7276 6963 652e 6761 7465  ort.service.gate
-00000860: 7761 792e 6f70 656e 6169 5f61 7069 0a60  way.openai_api.`
-00000870: 6060 0a0a 4966 2079 6f75 206e 6565 6420  ``..If you need 
-00000880: 7468 6520 656d 6265 6464 696e 6773 2041  the embeddings A
-00000890: 5049 206f 7220 6f74 6865 7220 6665 6174  PI or other feat
-000008a0: 7572 6573 2c20 796f 7520 6361 6e20 6465  ures, you can de
-000008b0: 706c 6f79 2061 2064 6973 7472 6962 7574  ploy a distribut
-000008c0: 6564 2069 6e66 6572 656e 6365 2063 6c75  ed inference clu
-000008d0: 7374 6572 3a0a 6060 6020 6261 7368 0a70  ster:.``` bash.p
-000008e0: 7974 686f 6e20 2d6d 206c 616e 6770 6f72  ython -m langpor
-000008f0: 742e 7365 7276 6963 652e 7365 7276 6572  t.service.server
-00000900: 2e64 756d 6d79 5f77 6f72 6b65 7220 2d2d  .dummy_worker --
-00000910: 706f 7274 2032 3130 3031 0a70 7974 686f  port 21001.pytho
-00000920: 6e20 2d6d 206c 616e 6770 6f72 742e 7365  n -m langport.se
-00000930: 7276 6963 652e 7365 7276 6572 2e67 656e  rvice.server.gen
-00000940: 6572 6174 696f 6e5f 776f 726b 6572 202d  eration_worker -
-00000950: 2d6d 6f64 656c 2d70 6174 6820 3c79 6f75  -model-path <you
-00000960: 7220 6d6f 6465 6c20 7061 7468 3e20 2d2d  r model path> --
-00000970: 6e65 6967 6862 6f72 7320 6874 7470 3a2f  neighbors http:/
-00000980: 2f6c 6f63 616c 686f 7374 3a32 3130 3031  /localhost:21001
-00000990: 0a70 7974 686f 6e20 2d6d 206c 616e 6770  .python -m langp
-000009a0: 6f72 742e 7365 7276 6963 652e 7365 7276  ort.service.serv
-000009b0: 6572 2e65 6d62 6564 6469 6e67 5f77 6f72  er.embedding_wor
-000009c0: 6b65 7220 2d2d 6d6f 6465 6c2d 7061 7468  ker --model-path
-000009d0: 203c 796f 7572 206d 6f64 656c 2070 6174   <your model pat
-000009e0: 683e 202d 2d6e 6569 6768 626f 7273 2068  h> --neighbors h
-000009f0: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
-00000a00: 3231 3030 310a 7079 7468 6f6e 202d 6d20  21001.python -m 
-00000a10: 6c61 6e67 706f 7274 2e73 6572 7669 6365  langport.service
-00000a20: 2e67 6174 6577 6179 2e6f 7065 6e61 695f  .gateway.openai_
-00000a30: 6170 6920 2d2d 636f 6e74 726f 6c6c 6572  api --controller
-00000a40: 2d61 6464 7265 7373 2068 7474 703a 2f2f  -address http://
-00000a50: 6c6f 6361 6c68 6f73 743a 3231 3030 310a  localhost:21001.
-00000a60: 6060 600a 0a49 6e20 7072 6163 7469 6365  ```..In practice
-00000a70: 2c20 7468 6520 6761 7465 7761 7920 6361  , the gateway ca
-00000a80: 6e20 636f 6e6e 6563 7420 746f 2061 6e79  n connect to any
-00000a90: 206e 6f64 6520 746f 2064 6973 7472 6962   node to distrib
-00000aa0: 7574 6520 696e 6665 7265 6e63 6520 7461  ute inference ta
-00000ab0: 736b 733a 0a0a 6060 6020 6261 7368 0a70  sks:..``` bash.p
-00000ac0: 7974 686f 6e20 2d6d 206c 616e 6770 6f72  ython -m langpor
-00000ad0: 742e 7365 7276 6963 652e 7365 7276 6572  t.service.server
-00000ae0: 2e64 756d 6d79 5f77 6f72 6b65 7220 2d2d  .dummy_worker --
-00000af0: 706f 7274 2032 3130 3031 0a70 7974 686f  port 21001.pytho
-00000b00: 6e20 2d6d 206c 616e 6770 6f72 742e 7365  n -m langport.se
-00000b10: 7276 6963 652e 7365 7276 6572 2e67 656e  rvice.server.gen
-00000b20: 6572 6174 696f 6e5f 776f 726b 6572 202d  eration_worker -
-00000b30: 2d70 6f72 7420 3231 3030 3220 2d2d 6d6f  -port 21002 --mo
-00000b40: 6465 6c2d 7061 7468 203c 796f 7572 206d  del-path <your m
-00000b50: 6f64 656c 2070 6174 683e 202d 2d6e 6569  odel path> --nei
-00000b60: 6768 626f 7273 2068 7474 703a 2f2f 6c6f  ghbors http://lo
-00000b70: 6361 6c68 6f73 743a 3231 3030 310a 7079  calhost:21001.py
-00000b80: 7468 6f6e 202d 6d20 6c61 6e67 706f 7274  thon -m langport
-00000b90: 2e73 6572 7669 6365 2e73 6572 7665 722e  .service.server.
-00000ba0: 6765 6e65 7261 7469 6f6e 5f77 6f72 6b65  generation_worke
-00000bb0: 7220 2d2d 706f 7274 2032 3130 3033 202d  r --port 21003 -
-00000bc0: 2d6d 6f64 656c 2d70 6174 6820 3c79 6f75  -model-path <you
-00000bd0: 7220 6d6f 6465 6c20 7061 7468 3e20 2d2d  r model path> --
-00000be0: 6e65 6967 6862 6f72 7320 6874 7470 3a2f  neighbors http:/
-00000bf0: 2f6c 6f63 616c 686f 7374 3a32 3130 3031  /localhost:21001
-00000c00: 2068 7474 703a 2f2f 6c6f 6361 6c68 6f73   http://localhos
-00000c10: 743a 3231 3030 320a 7079 7468 6f6e 202d  t:21002.python -
-00000c20: 6d20 6c61 6e67 706f 7274 2e73 6572 7669  m langport.servi
-00000c30: 6365 2e73 6572 7665 722e 6765 6e65 7261  ce.server.genera
-00000c40: 7469 6f6e 5f77 6f72 6b65 7220 2d2d 706f  tion_worker --po
-00000c50: 7274 2032 3130 3034 202d 2d6d 6f64 656c  rt 21004 --model
-00000c60: 2d70 6174 6820 3c79 6f75 7220 6d6f 6465  -path <your mode
-00000c70: 6c20 7061 7468 3e20 2d2d 6e65 6967 6862  l path> --neighb
-00000c80: 6f72 7320 6874 7470 3a2f 2f6c 6f63 616c  ors http://local
-00000c90: 686f 7374 3a32 3130 3031 2068 7474 703a  host:21001 http:
-00000ca0: 2f2f 6c6f 6361 6c68 6f73 743a 3231 3030  //localhost:2100
-00000cb0: 330a 7079 7468 6f6e 202d 6d20 6c61 6e67  3.python -m lang
-00000cc0: 706f 7274 2e73 6572 7669 6365 2e73 6572  port.service.ser
-00000cd0: 7665 722e 6765 6e65 7261 7469 6f6e 5f77  ver.generation_w
-00000ce0: 6f72 6b65 7220 2d2d 706f 7274 2032 3130  orker --port 210
-00000cf0: 3035 202d 2d6d 6f64 656c 2d70 6174 6820  05 --model-path 
-00000d00: 3c79 6f75 7220 6d6f 6465 6c20 7061 7468  <your model path
-00000d10: 3e20 2d2d 6e65 6967 6862 6f72 7320 6874  > --neighbors ht
-00000d20: 7470 3a2f 2f6c 6f63 616c 686f 7374 3a32  tp://localhost:2
-00000d30: 3130 3031 2068 7474 703a 2f2f 6c6f 6361  1001 http://loca
-00000d40: 6c68 6f73 743a 3231 3030 340a 7079 7468  lhost:21004.pyth
-00000d50: 6f6e 202d 6d20 6c61 6e67 706f 7274 2e73  on -m langport.s
-00000d60: 6572 7669 6365 2e67 6174 6577 6179 2e6f  ervice.gateway.o
-00000d70: 7065 6e61 695f 6170 6920 2d2d 636f 6e74  penai_api --cont
-00000d80: 726f 6c6c 6572 2d61 6464 7265 7373 2068  roller-address h
-00000d90: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
-00000da0: 3231 3030 3320 2320 3231 3030 3320 6973  21003 # 21003 is
-00000db0: 204f 4b21 0a70 7974 686f 6e20 2d6d 206c   OK!.python -m l
-00000dc0: 616e 6770 6f72 742e 7365 7276 6963 652e  angport.service.
-00000dd0: 6761 7465 7761 792e 6f70 656e 6169 5f61  gateway.openai_a
-00000de0: 7069 202d 2d63 6f6e 7472 6f6c 6c65 722d  pi --controller-
-00000df0: 6164 6472 6573 7320 6874 7470 3a2f 2f6c  address http://l
-00000e00: 6f63 616c 686f 7374 3a32 3130 3032 2023  ocalhost:21002 #
-00000e10: 2041 6e79 2077 6f72 6b65 7220 6973 2061   Any worker is a
-00000e20: 6c73 6f20 4f4b 210a 6060 600a 0a23 2320  lso OK!.```..## 
-00000e30: 4c69 6365 6e73 650a 0a6c 616e 6770 6f72  License..langpor
-00000e40: 7420 6973 2072 656c 6561 7365 6420 756e  t is released un
-00000e50: 6465 7220 7468 6520 4170 6163 6865 2053  der the Apache S
-00000e60: 6f66 7477 6172 6520 4c69 6365 6e73 652e  oftware License.
-00000e70: 0a0a 0a23 2320 5365 6520 616c 736f 0a0a  ...## See also..
-00000e80: 2d20 5b6c 616e 6770 6f72 742d 646f 6373  - [langport-docs
-00000e90: 5d28 6874 7470 733a 2f2f 6c61 6e67 706f  ](https://langpo
-00000ea0: 7274 2e72 6561 6474 6865 646f 6373 2e69  rt.readthedocs.i
-00000eb0: 6f2f 290a 2d20 5b6c 616e 6770 6f72 742d  o/).- [langport-
-00000ec0: 736f 7572 6365 5d28 6874 7470 733a 2f2f  source](https://
-00000ed0: 6769 7468 7562 2e63 6f6d 2f76 7475 6265  github.com/vtube
-00000ee0: 722d 706c 616e 2f6c 616e 6770 6f72 7429  r-plan/langport)
-00000ef0: 0a                                       .
+00000000: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00000010: 6572 223e 0a0a 2320 4c61 6e67 506f 7274  er">..# LangPort
+00000020: 0a0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
+00000030: 3a2f 2f67 6974 6875 622e 636f 6d2f 7674  ://github.com/vt
+00000040: 7562 6572 2d70 6c61 6e2f 6c61 6e67 706f  uber-plan/langpo
+00000050: 7274 223e 0a20 203c 696d 6720 616c 743d  rt">.  <img alt=
+00000060: 2247 6974 4875 6220 5265 706f 2073 7461  "GitHub Repo sta
+00000070: 7273 2220 7372 633d 2268 7474 7073 3a2f  rs" src="https:/
+00000080: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000090: 6769 7468 7562 2f73 7461 7273 2f76 7475  github/stars/vtu
+000000a0: 6265 722d 706c 616e 2f6c 616e 6770 6f72  ber-plan/langpor
+000000b0: 743f 7374 796c 653d 736f 6369 616c 223e  t?style=social">
+000000c0: 0a3c 2f61 3e0a 3c61 2068 7265 663d 2268  .</a>.<a href="h
+000000d0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000000e0: 6d2f 7674 7562 6572 2d70 6c61 6e2f 6c61  m/vtuber-plan/la
+000000f0: 6e67 706f 7274 2f62 6c6f 622f 6d61 696e  ngport/blob/main
+00000100: 2f4c 4943 454e 5345 223e 0a20 203c 696d  /LICENSE">.  <im
+00000110: 6720 616c 743d 224c 6963 656e 7365 2220  g alt="License" 
+00000120: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00000130: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+00000140: 7562 2f6c 6963 656e 7365 2f76 7475 6265  ub/license/vtube
+00000150: 722d 706c 616e 2f6c 616e 6770 6f72 7422  r-plan/langport"
+00000160: 3e0a 3c2f 613e 0a0a 215b 6172 6368 6974  >.</a>..![archit
+00000170: 6563 7475 7265 5d28 6173 7365 7473 2f61  ecture](assets/a
+00000180: 7263 6869 7465 6374 7572 652e 6a70 6729  rchitecture.jpg)
+00000190: 0a0a 3c2f 6469 763e 0a0a 4c61 6e67 506f  ..</div>..LangPo
+000001a0: 7274 2069 7320 6120 6f70 656e 2d73 6f75  rt is a open-sou
+000001b0: 7263 6520 6c61 7267 6520 6c61 6e67 7561  rce large langua
+000001c0: 6765 206d 6f64 656c 2073 6572 7669 6e67  ge model serving
+000001d0: 2070 6c61 7466 6f72 6d2e 0a4f 7572 2067   platform..Our g
+000001e0: 6f61 6c20 6973 2074 6f20 6275 696c 6420  oal is to build 
+000001f0: 6120 7375 7065 7220 6661 7374 204c 4c4d  a super fast LLM
+00000200: 2069 6e66 6572 656e 6365 2073 6572 7669   inference servi
+00000210: 6365 2e0a 0a54 6869 7320 7072 6f6a 6563  ce...This projec
+00000220: 7420 6973 2069 6e73 7069 7265 6420 6279  t is inspired by
+00000230: 205b 6c6d 7379 732f 6661 7374 6368 6174   [lmsys/fastchat
+00000240: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000250: 2e63 6f6d 2f6c 6d2d 7379 732f 4661 7374  .com/lm-sys/Fast
+00000260: 4368 6174 292c 2077 6520 686f 7065 2074  Chat), we hope t
+00000270: 6861 7420 7468 6520 7365 7276 696e 6720  hat the serving 
+00000280: 706c 6174 666f 726d 2069 7320 6c69 6768  platform is ligh
+00000290: 7477 6569 6768 7420 616e 6420 6661 7374  tweight and fast
+000002a0: 2c20 6275 7420 6661 7374 6368 6174 2069  , but fastchat i
+000002b0: 6e63 6c75 6465 7320 6f74 6865 7220 6665  ncludes other fe
+000002c0: 6174 7572 6573 2073 7563 6820 6173 2074  atures such as t
+000002d0: 7261 696e 696e 6720 616e 6420 6576 616c  raining and eval
+000002e0: 7561 7469 6f6e 206d 616b 6520 6974 2063  uation make it c
+000002f0: 6f6d 706c 6963 6174 6564 2e0a 0a54 6865  omplicated...The
+00000300: 2063 6f72 6520 6665 6174 7572 6573 2069   core features i
+00000310: 6e63 6c75 6465 3a0a 2d20 4120 6469 7374  nclude:.- A dist
+00000320: 7269 6275 7465 6420 7365 7276 696e 6720  ributed serving 
+00000330: 7379 7374 656d 2066 6f72 2073 7461 7465  system for state
+00000340: 2d6f 662d 7468 652d 6172 7420 6d6f 6465  -of-the-art mode
+00000350: 6c73 2e0a 2d20 5374 7265 616d 696e 6720  ls..- Streaming 
+00000360: 6765 6e65 7261 7469 6f6e 2073 7570 706f  generation suppo
+00000370: 7274 2077 6974 6820 7661 7269 6f75 7320  rt with various 
+00000380: 6465 636f 6469 6e67 2073 7472 6174 6567  decoding strateg
+00000390: 6965 732e 0a2d 2042 6174 6368 2069 6e66  ies..- Batch inf
+000003a0: 6572 656e 6365 2066 6f72 2068 6967 6865  erence for highe
+000003b0: 7220 7468 726f 7567 6870 7574 2e0a 2d20  r throughput..- 
+000003c0: 5375 7070 6f72 7420 666f 7220 656e 636f  Support for enco
+000003d0: 6465 722d 6f6e 6c79 2c20 6465 636f 6465  der-only, decode
+000003e0: 722d 6f6e 6c79 2061 6e64 2065 6e63 6f64  r-only and encod
+000003f0: 6572 2d64 6563 6f64 6572 206d 6f64 656c  er-decoder model
+00000400: 732e 0a2d 204f 7065 6e41 492d 636f 6d70  s..- OpenAI-comp
+00000410: 6174 6962 6c65 2052 4553 5466 756c 2041  atible RESTful A
+00000420: 5049 732e 0a2d 2046 6175 7850 696c 6f74  PIs..- FauxPilot
+00000430: 2d63 6f6d 7061 7469 626c 6520 5245 5354  -compatible REST
+00000440: 6675 6c20 4150 4973 2e0a 2d20 4875 6767  ful APIs..- Hugg
+00000450: 696e 6746 6163 652d 636f 6d70 6174 6962  ingFace-compatib
+00000460: 6c65 2052 4553 5466 756c 2041 5049 732e  le RESTful APIs.
+00000470: 0a2d 2054 6162 6279 2d63 6f6d 7061 7469  .- Tabby-compati
+00000480: 626c 6520 5245 5354 6675 6c20 4150 4973  ble RESTful APIs
+00000490: 2e0a 0a23 2320 4265 6e63 686d 6172 6b0a  ...## Benchmark.
+000004a0: 5765 2075 7365 2073 696e 676c 6520 5254  We use single RT
+000004b0: 5833 3039 3020 746f 2072 756e 2061 2066  X3090 to run a f
+000004c0: 696e 6574 756e 6564 2037 4220 4c4c 614d  inetuned 7B LLaM
+000004d0: 4120 6d6f 6465 6c20 284f 7065 6e42 7564  A model (OpenBud
+000004e0: 6479 2056 302e 3929 2075 6e64 6572 2074  dy V0.9) under t
+000004f0: 6865 2062 6631 3620 7365 7474 696e 672e  he bf16 setting.
+00000500: 0a57 6520 6372 6561 7465 2033 3220 7468  .We create 32 th
+00000510: 7265 6164 7320 746f 2073 7562 6d69 7420  reads to submit 
+00000520: 6368 6174 2074 6173 6b73 2074 6f20 7468  chat tasks to th
+00000530: 6520 7365 7276 6572 2c20 616e 6420 7468  e server, and th
+00000540: 6520 666f 6c6c 6f77 696e 6720 6669 6775  e following figu
+00000550: 7265 2073 686f 7773 2074 6865 2051 7565  re shows the Que
+00000560: 7269 6573 2050 6572 2053 6563 6f6e 6420  ries Per Second 
+00000570: 2851 5053 2920 616e 6420 546f 6b65 6e73  (QPS) and Tokens
+00000580: 2050 6572 2053 6563 6f6e 6420 2854 5053   Per Second (TPS
+00000590: 2920 6f66 2046 6173 7443 6861 7420 616e  ) of FastChat an
+000005a0: 6420 4c61 6e67 506f 7274 2077 6974 6820  d LangPort with 
+000005b0: 6469 6666 6572 656e 7420 6d61 7820 6d6f  different max mo
+000005c0: 6465 6c20 636f 6e63 7572 7265 6e63 7920  del concurrency 
+000005d0: 7365 7474 696e 6773 2e0a 0a21 5b62 656e  settings...![ben
+000005e0: 6368 6d61 726b 5f63 6861 745d 2861 7373  chmark_chat](ass
+000005f0: 6574 732f 6265 6e63 686d 6172 6b5f 6368  ets/benchmark_ch
+00000600: 6174 2e6a 7067 290a 0a0a 2323 204e 6577  at.jpg)...## New
+00000610: 730a 2d20 5b32 3032 332f 3036 2f30 395d  s.- [2023/06/09]
+00000620: 2041 6464 204c 4c61 6d61 2e63 7070 2077   Add LLama.cpp w
+00000630: 6f72 6b65 7220 7375 7070 6f72 742e 0a2d  orker support..-
+00000640: 205b 3230 3233 2f30 362f 3031 5d20 4164   [2023/06/01] Ad
+00000650: 6420 4875 6767 696e 6746 6163 6520 4265  d HuggingFace Be
+00000660: 7274 2065 6d62 6564 6469 6e67 2077 6f72  rt embedding wor
+00000670: 6b65 7220 7375 7070 6f72 742e 0a2d 205b  ker support..- [
+00000680: 3230 3233 2f30 362f 3031 5d20 4164 6420  2023/06/01] Add 
+00000690: 4875 6767 696e 6746 6163 6520 7465 7874  HuggingFace text
+000006a0: 2067 656e 6572 6174 696f 6e20 4150 4920   generation API 
+000006b0: 7375 7070 6f72 742e 0a2d 205b 3230 3233  support..- [2023
+000006c0: 2f30 362f 3031 5d20 4164 6420 7461 6262  /06/01] Add tabb
+000006d0: 7920 4150 4920 7375 7070 6f72 742e 0a2d  y API support..-
+000006e0: 205b 3230 3233 2f30 352f 3233 5d20 4164   [2023/05/23] Ad
+000006f0: 6420 6368 6174 2074 6872 6f75 6768 7075  d chat throughpu
+00000700: 7420 7465 7374 2073 6372 6970 742e 0a2d  t test script..-
+00000710: 205b 3230 3233 2f30 352f 3232 5d20 4e65   [2023/05/22] Ne
+00000720: 7720 6469 7374 7269 6275 7465 6420 6172  w distributed ar
+00000730: 6368 6974 6563 7475 7265 2e0a 2d20 5b32  chitecture..- [2
+00000740: 3032 332f 3035 2f31 345d 2042 6174 6368  023/05/14] Batch
+00000750: 2069 6e66 6572 656e 6365 2073 7570 706f   inference suppo
+00000760: 7274 6564 2e0a 2d20 5b32 3032 332f 3035  rted..- [2023/05
+00000770: 2f31 305d 204c 616e 6770 6f72 7420 7072  /10] Langport pr
+00000780: 6f6a 6563 7420 7374 6172 7465 642e 0a0a  oject started...
+00000790: 0a23 2320 496e 7374 616c 6c0a 0a23 2323  .## Install..###
+000007a0: 204d 6574 686f 6420 313a 2057 6974 6820   Method 1: With 
+000007b0: 7069 700a 0a60 6060 6261 7368 0a70 6970  pip..```bash.pip
+000007c0: 3320 696e 7374 616c 6c20 6c61 6e67 706f  3 install langpo
+000007d0: 7274 0a60 6060 0a0a 6f72 3a0a 0a60 6060  rt.```..or:..```
+000007e0: 6261 7368 0a70 6970 3320 696e 7374 616c  bash.pip3 instal
+000007f0: 6c20 6769 742b 6874 7470 733a 2f2f 6769  l git+https://gi
+00000800: 7468 7562 2e63 6f6d 2f76 7475 6265 722d  thub.com/vtuber-
+00000810: 706c 616e 2f6c 616e 6770 6f72 742e 6769  plan/langport.gi
+00000820: 7420 0a60 6060 0a0a 4966 2079 6f75 206e  t .```..If you n
+00000830: 6565 6420 6c6c 616d 6163 7070 2067 656e  eed llamacpp gen
+00000840: 6572 6174 696f 6e20 776f 726b 6572 2c20  eration worker, 
+00000850: 7573 6520 7468 6973 2063 6f6d 6d61 6e64  use this command
+00000860: 3a0a 6060 6062 6173 680a 7069 7033 2069  :.```bash.pip3 i
+00000870: 6e73 7461 6c6c 206c 616e 6770 6f72 745b  nstall langport[
+00000880: 6c6c 616d 6163 7070 5d0a 6060 600a 0a23  llamacpp].```..#
+00000890: 2323 204d 6574 686f 6420 323a 2046 726f  ## Method 2: Fro
+000008a0: 6d20 736f 7572 6365 0a0a 312e 2043 6c6f  m source..1. Clo
+000008b0: 6e65 2074 6869 7320 7265 706f 7369 746f  ne this reposito
+000008c0: 7279 0a60 6060 6261 7368 0a67 6974 2063  ry.```bash.git c
+000008d0: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
+000008e0: 6875 622e 636f 6d2f 7674 7562 6572 2d70  hub.com/vtuber-p
+000008f0: 6c61 6e2f 6c61 6e67 706f 7274 2e67 6974  lan/langport.git
+00000900: 0a63 6420 6c61 6e67 706f 7274 0a60 6060  .cd langport.```
+00000910: 0a0a 322e 2049 6e73 7461 6c6c 2074 6865  ..2. Install the
+00000920: 2050 6163 6b61 6765 0a60 6060 6261 7368   Package.```bash
+00000930: 0a70 6970 2069 6e73 7461 6c6c 202d 2d75  .pip install --u
+00000940: 7067 7261 6465 2070 6970 0a70 6970 2069  pgrade pip.pip i
+00000950: 6e73 7461 6c6c 202d 6520 2e0a 6060 600a  nstall -e ..```.
+00000960: 0a23 2320 5374 6172 7420 7468 6520 7365  .## Start the se
+00000970: 7276 6572 0a0a 4974 2069 7320 7369 6d70  rver..It is simp
+00000980: 6c65 2074 6f20 7374 6172 7420 6120 7369  le to start a si
+00000990: 6e67 6c65 206e 6f64 6520 6368 6174 2041  ngle node chat A
+000009a0: 5049 2073 6572 7669 6365 3a0a 6060 6020  PI service:.``` 
+000009b0: 6261 7368 0a70 7974 686f 6e20 2d6d 206c  bash.python -m l
+000009c0: 616e 6770 6f72 742e 7365 7276 6963 652e  angport.service.
+000009d0: 7365 7276 6572 2e67 656e 6572 6174 696f  server.generatio
+000009e0: 6e5f 776f 726b 6572 202d 2d70 6f72 7420  n_worker --port 
+000009f0: 3231 3030 3120 2d2d 6d6f 6465 6c2d 7061  21001 --model-pa
+00000a00: 7468 203c 796f 7572 206d 6f64 656c 2070  th <your model p
+00000a10: 6174 683e 0a70 7974 686f 6e20 2d6d 206c  ath>.python -m l
+00000a20: 616e 6770 6f72 742e 7365 7276 6963 652e  angport.service.
+00000a30: 6761 7465 7761 792e 6f70 656e 6169 5f61  gateway.openai_a
+00000a40: 7069 0a60 6060 0a0a 4966 2079 6f75 206e  pi.```..If you n
+00000a50: 6565 6420 7468 6520 656d 6265 6464 696e  eed the embeddin
+00000a60: 6773 2041 5049 206f 7220 6f74 6865 7220  gs API or other 
+00000a70: 6665 6174 7572 6573 2c20 796f 7520 6361  features, you ca
+00000a80: 6e20 6465 706c 6f79 2061 2064 6973 7472  n deploy a distr
+00000a90: 6962 7574 6564 2069 6e66 6572 656e 6365  ibuted inference
+00000aa0: 2063 6c75 7374 6572 3a0a 6060 6020 6261   cluster:.``` ba
+00000ab0: 7368 0a70 7974 686f 6e20 2d6d 206c 616e  sh.python -m lan
+00000ac0: 6770 6f72 742e 7365 7276 6963 652e 7365  gport.service.se
+00000ad0: 7276 6572 2e64 756d 6d79 5f77 6f72 6b65  rver.dummy_worke
+00000ae0: 7220 2d2d 706f 7274 2032 3130 3031 0a70  r --port 21001.p
+00000af0: 7974 686f 6e20 2d6d 206c 616e 6770 6f72  ython -m langpor
+00000b00: 742e 7365 7276 6963 652e 7365 7276 6572  t.service.server
+00000b10: 2e67 656e 6572 6174 696f 6e5f 776f 726b  .generation_work
+00000b20: 6572 202d 2d6d 6f64 656c 2d70 6174 6820  er --model-path 
+00000b30: 3c79 6f75 7220 6d6f 6465 6c20 7061 7468  <your model path
+00000b40: 3e20 2d2d 6e65 6967 6862 6f72 7320 6874  > --neighbors ht
+00000b50: 7470 3a2f 2f6c 6f63 616c 686f 7374 3a32  tp://localhost:2
+00000b60: 3130 3031 0a70 7974 686f 6e20 2d6d 206c  1001.python -m l
+00000b70: 616e 6770 6f72 742e 7365 7276 6963 652e  angport.service.
+00000b80: 7365 7276 6572 2e65 6d62 6564 6469 6e67  server.embedding
+00000b90: 5f77 6f72 6b65 7220 2d2d 6d6f 6465 6c2d  _worker --model-
+00000ba0: 7061 7468 203c 796f 7572 206d 6f64 656c  path <your model
+00000bb0: 2070 6174 683e 202d 2d6e 6569 6768 626f   path> --neighbo
+00000bc0: 7273 2068 7474 703a 2f2f 6c6f 6361 6c68  rs http://localh
+00000bd0: 6f73 743a 3231 3030 310a 7079 7468 6f6e  ost:21001.python
+00000be0: 202d 6d20 6c61 6e67 706f 7274 2e73 6572   -m langport.ser
+00000bf0: 7669 6365 2e67 6174 6577 6179 2e6f 7065  vice.gateway.ope
+00000c00: 6e61 695f 6170 6920 2d2d 636f 6e74 726f  nai_api --contro
+00000c10: 6c6c 6572 2d61 6464 7265 7373 2068 7474  ller-address htt
+00000c20: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3231  p://localhost:21
+00000c30: 3030 310a 6060 600a 0a49 6e20 7072 6163  001.```..In prac
+00000c40: 7469 6365 2c20 7468 6520 6761 7465 7761  tice, the gatewa
+00000c50: 7920 6361 6e20 636f 6e6e 6563 7420 746f  y can connect to
+00000c60: 2061 6e79 206e 6f64 6520 746f 2064 6973   any node to dis
+00000c70: 7472 6962 7574 6520 696e 6665 7265 6e63  tribute inferenc
+00000c80: 6520 7461 736b 733a 0a0a 6060 6020 6261  e tasks:..``` ba
+00000c90: 7368 0a70 7974 686f 6e20 2d6d 206c 616e  sh.python -m lan
+00000ca0: 6770 6f72 742e 7365 7276 6963 652e 7365  gport.service.se
+00000cb0: 7276 6572 2e64 756d 6d79 5f77 6f72 6b65  rver.dummy_worke
+00000cc0: 7220 2d2d 706f 7274 2032 3130 3031 0a70  r --port 21001.p
+00000cd0: 7974 686f 6e20 2d6d 206c 616e 6770 6f72  ython -m langpor
+00000ce0: 742e 7365 7276 6963 652e 7365 7276 6572  t.service.server
+00000cf0: 2e67 656e 6572 6174 696f 6e5f 776f 726b  .generation_work
+00000d00: 6572 202d 2d70 6f72 7420 3231 3030 3220  er --port 21002 
+00000d10: 2d2d 6d6f 6465 6c2d 7061 7468 203c 796f  --model-path <yo
+00000d20: 7572 206d 6f64 656c 2070 6174 683e 202d  ur model path> -
+00000d30: 2d6e 6569 6768 626f 7273 2068 7474 703a  -neighbors http:
+00000d40: 2f2f 6c6f 6361 6c68 6f73 743a 3231 3030  //localhost:2100
+00000d50: 310a 7079 7468 6f6e 202d 6d20 6c61 6e67  1.python -m lang
+00000d60: 706f 7274 2e73 6572 7669 6365 2e73 6572  port.service.ser
+00000d70: 7665 722e 6765 6e65 7261 7469 6f6e 5f77  ver.generation_w
+00000d80: 6f72 6b65 7220 2d2d 706f 7274 2032 3130  orker --port 210
+00000d90: 3033 202d 2d6d 6f64 656c 2d70 6174 6820  03 --model-path 
+00000da0: 3c79 6f75 7220 6d6f 6465 6c20 7061 7468  <your model path
+00000db0: 3e20 2d2d 6e65 6967 6862 6f72 7320 6874  > --neighbors ht
+00000dc0: 7470 3a2f 2f6c 6f63 616c 686f 7374 3a32  tp://localhost:2
+00000dd0: 3130 3031 2068 7474 703a 2f2f 6c6f 6361  1001 http://loca
+00000de0: 6c68 6f73 743a 3231 3030 320a 7079 7468  lhost:21002.pyth
+00000df0: 6f6e 202d 6d20 6c61 6e67 706f 7274 2e73  on -m langport.s
+00000e00: 6572 7669 6365 2e73 6572 7665 722e 6765  ervice.server.ge
+00000e10: 6e65 7261 7469 6f6e 5f77 6f72 6b65 7220  neration_worker 
+00000e20: 2d2d 706f 7274 2032 3130 3034 202d 2d6d  --port 21004 --m
+00000e30: 6f64 656c 2d70 6174 6820 3c79 6f75 7220  odel-path <your 
+00000e40: 6d6f 6465 6c20 7061 7468 3e20 2d2d 6e65  model path> --ne
+00000e50: 6967 6862 6f72 7320 6874 7470 3a2f 2f6c  ighbors http://l
+00000e60: 6f63 616c 686f 7374 3a32 3130 3031 2068  ocalhost:21001 h
+00000e70: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
+00000e80: 3231 3030 330a 7079 7468 6f6e 202d 6d20  21003.python -m 
+00000e90: 6c61 6e67 706f 7274 2e73 6572 7669 6365  langport.service
+00000ea0: 2e73 6572 7665 722e 6765 6e65 7261 7469  .server.generati
+00000eb0: 6f6e 5f77 6f72 6b65 7220 2d2d 706f 7274  on_worker --port
+00000ec0: 2032 3130 3035 202d 2d6d 6f64 656c 2d70   21005 --model-p
+00000ed0: 6174 6820 3c79 6f75 7220 6d6f 6465 6c20  ath <your model 
+00000ee0: 7061 7468 3e20 2d2d 6e65 6967 6862 6f72  path> --neighbor
+00000ef0: 7320 6874 7470 3a2f 2f6c 6f63 616c 686f  s http://localho
+00000f00: 7374 3a32 3130 3031 2068 7474 703a 2f2f  st:21001 http://
+00000f10: 6c6f 6361 6c68 6f73 743a 3231 3030 340a  localhost:21004.
+00000f20: 7079 7468 6f6e 202d 6d20 6c61 6e67 706f  python -m langpo
+00000f30: 7274 2e73 6572 7669 6365 2e67 6174 6577  rt.service.gatew
+00000f40: 6179 2e6f 7065 6e61 695f 6170 6920 2d2d  ay.openai_api --
+00000f50: 636f 6e74 726f 6c6c 6572 2d61 6464 7265  controller-addre
+00000f60: 7373 2068 7474 703a 2f2f 6c6f 6361 6c68  ss http://localh
+00000f70: 6f73 743a 3231 3030 3320 2320 3231 3030  ost:21003 # 2100
+00000f80: 3320 6973 204f 4b21 0a70 7974 686f 6e20  3 is OK!.python 
+00000f90: 2d6d 206c 616e 6770 6f72 742e 7365 7276  -m langport.serv
+00000fa0: 6963 652e 6761 7465 7761 792e 6f70 656e  ice.gateway.open
+00000fb0: 6169 5f61 7069 202d 2d63 6f6e 7472 6f6c  ai_api --control
+00000fc0: 6c65 722d 6164 6472 6573 7320 6874 7470  ler-address http
+00000fd0: 3a2f 2f6c 6f63 616c 686f 7374 3a32 3130  ://localhost:210
+00000fe0: 3032 2023 2041 6e79 2077 6f72 6b65 7220  02 # Any worker 
+00000ff0: 6973 2061 6c73 6f20 4f4b 210a 6060 600a  is also OK!.```.
+00001000: 0a52 756e 2074 6578 7420 6765 6e65 7261  .Run text genera
+00001010: 7469 6f6e 2077 6974 6820 6d75 6c74 6920  tion with multi 
+00001020: 4750 5573 3a0a 0a60 6060 2062 6173 680a  GPUs:..``` bash.
+00001030: 7079 7468 6f6e 202d 6d20 6c61 6e67 706f  python -m langpo
+00001040: 7274 2e73 6572 7669 6365 2e73 6572 7665  rt.service.serve
+00001050: 722e 6765 6e65 7261 7469 6f6e 5f77 6f72  r.generation_wor
+00001060: 6b65 7220 2d2d 706f 7274 2032 3130 3031  ker --port 21001
+00001070: 202d 2d6d 6f64 656c 2d70 6174 6820 3c79   --model-path <y
+00001080: 6f75 7220 6d6f 6465 6c20 7061 7468 3e20  our model path> 
+00001090: 2d2d 6770 7573 2030 2c31 202d 2d6e 756d  --gpus 0,1 --num
+000010a0: 2d67 7075 7320 320a 7079 7468 6f6e 202d  -gpus 2.python -
+000010b0: 6d20 6c61 6e67 706f 7274 2e73 6572 7669  m langport.servi
+000010c0: 6365 2e67 6174 6577 6179 2e6f 7065 6e61  ce.gateway.opena
+000010d0: 695f 6170 690a 6060 600a 0a52 756e 2074  i_api.```..Run t
+000010e0: 6578 7420 6765 6e65 7261 7469 6f6e 2077  ext generation w
+000010f0: 6974 6820 4c4c 616d 612e 6370 7020 776f  ith LLama.cpp wo
+00001100: 726b 6572 3a0a 0a60 6060 6261 7368 0a70  rker:..```bash.p
+00001110: 7974 686f 6e20 2d6d 206c 616e 6770 6f72  ython -m langpor
+00001120: 742e 7365 7276 6963 652e 7365 7276 6572  t.service.server
+00001130: 2e67 656e 6572 6174 696f 6e5f 776f 726b  .generation_work
+00001140: 6572 202d 2d70 6f72 7420 3231 3030 3120  er --port 21001 
+00001150: 2d2d 6d6f 6465 6c2d 7061 7468 203c 796f  --model-path <yo
+00001160: 7572 206d 6f64 656c 2070 6174 683e 202d  ur model path> -
+00001170: 2d6e 2d67 7075 2d6c 6179 6572 7320 3c6e  -n-gpu-layers <n
+00001180: 756d 206c 6179 6572 2074 6f20 6770 7520  um layer to gpu 
+00001190: 2872 6573 697a 6520 7468 6973 2066 6f72  (resize this for
+000011a0: 2079 6f75 7220 5652 414d 293e 0a60 6060   your VRAM)>.```
+000011b0: 0a0a 2323 204c 6963 656e 7365 0a0a 6c61  ..## License..la
+000011c0: 6e67 706f 7274 2069 7320 7265 6c65 6173  ngport is releas
+000011d0: 6564 2075 6e64 6572 2074 6865 2041 7061  ed under the Apa
+000011e0: 6368 6520 536f 6674 7761 7265 204c 6963  che Software Lic
+000011f0: 656e 7365 2e0a 0a0a 2323 2053 6565 2061  ense....## See a
+00001200: 6c73 6f0a 0a2d 205b 6c61 6e67 706f 7274  lso..- [langport
+00001210: 2d64 6f63 735d 2868 7474 7073 3a2f 2f67  -docs](https://g
+00001220: 6974 6875 622e 636f 6d2f 7674 7562 6572  ithub.com/vtuber
+00001230: 2d70 6c61 6e2f 6c61 6e67 706f 7274 2f74  -plan/langport/t
+00001240: 7265 652f 6d61 696e 2f64 6f63 7329 0a2d  ree/main/docs).-
+00001250: 205b 6c61 6e67 706f 7274 2d73 6f75 7263   [langport-sourc
+00001260: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+00001270: 622e 636f 6d2f 7674 7562 6572 2d70 6c61  b.com/vtuber-pla
+00001280: 6e2f 6c61 6e67 706f 7274 290a 0a0a 2323  n/langport)...##
+00001290: 2053 7461 7220 4869 7374 6f72 790a 0a5b   Star History..[
+000012a0: 215b 5374 6172 2048 6973 746f 7279 2043  ![Star History C
+000012b0: 6861 7274 5d28 6874 7470 733a 2f2f 6170  hart](https://ap
+000012c0: 692e 7374 6172 2d68 6973 746f 7279 2e63  i.star-history.c
+000012d0: 6f6d 2f73 7667 3f72 6570 6f73 3d76 7475  om/svg?repos=vtu
+000012e0: 6265 722d 706c 616e 2f6c 616e 6770 6f72  ber-plan/langpor
+000012f0: 7426 7479 7065 3d44 6174 6529 5d28 6874  t&type=Date)](ht
+00001300: 7470 733a 2f2f 7374 6172 2d68 6973 746f  tps://star-histo
+00001310: 7279 2e63 6f6d 2f23 7674 7562 6572 2d70  ry.com/#vtuber-p
+00001320: 6c61 6e2f 6c61 6e67 706f 7274 2644 6174  lan/langport&Dat
+00001330: 6529 0a0a                                e)..
```

### Comparing `langport-0.0.4/langport/constants.py` & `langport-0.1.0/langport/constants.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from enum import IntEnum
 
 
 HEART_BEAT_EXPIRATION = 90
-CONTROLLER_STATUS_FRESH_INTERVAL = 30
 WORKER_HEART_BEAT_INTERVAL = 30
 EMBEDDING_INFERENCE_INTERVAL = 0.1
 GENERATION_INFERENCE_INTERVAL = 0.3
 WORKER_API_TIMEOUT = 20
 
 LOGDIR = "./logs"
```

### Comparing `langport-0.0.4/langport/core/base_node.py` & `langport-0.1.0/langport/core/base_node.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,11 @@
-import argparse
-import asyncio
-from collections import defaultdict
-import dataclasses
 import inspect
 import logging
-import json
-import os
-import time
-from typing import Any, Callable, Dict, Iterable, List, Mapping, Optional, Union
-import threading
-import queue
-import uuid
 
-import requests
-from tenacity import retry, stop_after_attempt
-
-from langport.constants import (
-    WORKER_API_TIMEOUT,
-    WORKER_HEART_BEAT_INTERVAL,
-    ErrorCode,
-)
+from typing import Any, Callable, Dict, Iterable, Mapping, Optional
 from langport.utils.interval_timer import IntervalTimer
 
 
 class BaseNode(object):
     def __init__(
         self,
         node_addr: str,
```

### Comparing `langport-0.0.4/langport/core/cluster_node.py` & `langport-0.1.0/langport/core/cluster_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,15 @@
-import argparse
 import asyncio
 from collections import defaultdict
-import dataclasses
-from functools import partial
 import logging
 import json
-import os
 import time
-from typing import Any, Callable, Dict, Iterable, List, Mapping, Optional, Tuple, Union
-import threading
-import queue
-import uuid
+from typing import Any, Dict, List
 
 import httpx
-import requests
-from tenacity import retry, stop_after_attempt
 from langport.core.base_node import BaseNode
 
 from langport.protocol.worker_protocol import (
     GetNodeStateRequest,
     GetNodeStateResponse,
     NodeInfo,
     NodeInfoRequest,
@@ -37,15 +28,14 @@
     HEART_BEAT_EXPIRATION,
     WORKER_API_TIMEOUT,
     WORKER_HEART_BEAT_INTERVAL,
     ErrorCode,
 )
 from langport.utils.cache_state import CacheState
 from langport.utils.http_pool import AsyncHttpPool
-from langport.utils.interval_timer import IntervalTimer
 from cachetools import LRUCache, TTLCache
 from asyncache import cached
 
 class ClusterNode(BaseNode):
     def __init__(
         self,
         node_addr: str,
@@ -203,15 +193,14 @@
     async def remove_self_node_broadcast(self):
         await self.remove_node_broadcast(self.node_id)
 
     async def send_heartbeat(self, node_addr: str):
         data = HeartbeatPing(
             node_id=self.node_id,
         )
-
         response = await self.client.post(
             node_addr + "/heartbeat",
             headers=self.headers,
             json=data.dict(),
             timeout=WORKER_API_TIMEOUT,
         )
         ret = HeartbeatPong.parse_obj(response.json())
@@ -289,15 +278,17 @@
         node_info = self.neighborhoods[node_id]
         response = await self.request_node_state(node_info.node_addr, name)
         value = json.loads(response.state_value)
         ttl = response.state_ttl
         if value is not None:
             # print(f"refresh state {name}, node id {node_id}, value {value}")
             self.remote_states[node_id][name] = CacheState(value, ttl)
-        return self.remote_states[node_id][name].get()
+            return self.remote_states[node_id][name].get()
+        else:
+            return None
     
     async def get_node_state(self, node_id: str, name: str) -> Any:
         if node_id == self.node_id:
             return await self._get_node_state_local(node_id, name)
         else:
             state_lock = asyncio.Lock()
             async with state_lock:
```

### Comparing `langport-0.0.4/langport/core/cluster_worker.py` & `langport-0.1.0/langport/core/cluster_worker.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,31 @@
-import argparse
 import asyncio
 from collections import defaultdict
-import dataclasses
-from functools import partial
 import logging
 import json
-import os
 import re
-import time
-from typing import Any, Callable, Dict, Iterable, List, Mapping, Optional, Union
-import threading
-import queue
-import uuid
-
+from typing import Dict, List, Optional
 
-import httpx
-import numpy as np
-import requests
-from tenacity import retry, stop_after_attempt
-from langport.core.base_node import BaseNode
+import queue
 from langport.core.cluster_node import ClusterNode
 
 from langport.protocol.worker_protocol import (
     BaseWorkerResult,
     BaseWorkerTask,
-    NodeInfo,
-    NodeInfoRequest,
-    NodeInfoResponse,
-    NodeListRequest,
-    NodeListResponse,
-    RegisterNodeRequest,
-    RegisterNodeResponse,
-    RemoveNodeRequest,
-    RemoveNodeResponse,
-    HeartbeatPing,
-    HeartbeatPong,
     WorkerAddressRequest,
     WorkerAddressResponse,
 )
 
 from langport.constants import (
     HEART_BEAT_EXPIRATION,
     WORKER_API_TIMEOUT,
     WORKER_HEART_BEAT_INTERVAL,
     ErrorCode,
 )
 from langport.utils.evaluation import safe_eval
-from langport.utils.interval_timer import IntervalTimer
 
 class ClusterWorker(ClusterNode):
     def __init__(
         self,
         node_addr: str,
         node_id: str,
         init_neighborhoods_addr: List[str],
@@ -105,28 +80,28 @@
             self.model_semaphore is None
             or self.model_semaphore._value is None
             or self.model_semaphore._waiters is None
         ):
             return 0
         else:
             return (
-                self.limit_model_concurrency
-                - self.model_semaphore._value
+                self.task_queue.qsize()
                 + len(self.model_semaphore._waiters)
             )
 
     async def add_task(self, task: BaseWorkerTask):
         self.task_queue.put(task, block=True, timeout=WORKER_API_TIMEOUT)
         self.output_queue[task.task_id] = queue.Queue()
         await self.set_queue_state()
 
     async def fetch_task_result(self, task_id: str):
         result_queue = self.output_queue[task_id]
         retry_counter = 0
         while True:
+            await self.set_queue_state()
             try:
                 event = result_queue.get(block=False, timeout=None)
             except queue.Empty:
                 await asyncio.sleep(0.01)
                 retry_counter += 1
                 # If client disconnected, stop to wait queue.
                 if retry_counter > 2000:
```

### Comparing `langport-0.0.4/langport/data/conversation/__init__.py` & `langport-0.1.0/langport/data/conversation/__init__.py`

 * *Files identical despite different names*

### Comparing `langport-0.0.4/langport/data/conversation/conversation_settings.py` & `langport-0.1.0/langport/data/conversation/conversation_settings.py`

 * *Files identical despite different names*

### Comparing `langport-0.0.4/langport/model/adapters/baize.py` & `langport-0.1.0/langport/model/adapters/baize.py`

 * *Files identical despite different names*

### Comparing `langport-0.0.4/langport/model/adapters/bard.py` & `langport-0.1.0/langport/model/adapters/claude.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,19 @@
-from typing import List, Optional
-import warnings
-from functools import cache
-
 from langport.data.conversation import ConversationHistory, SeparatorStyle
 from langport.data.conversation.conversation_settings import get_conv_settings
 from langport.model.model_adapter import BaseAdapter
 
-class BardAdapter(BaseAdapter):
-    """The model adapter for Bard."""
 
-    def match(self, model_path: str):
-        return model_path == "bard"
+class ClaudeAdapter(BaseAdapter):
+    """The model adapter for Claude."""
 
-    def load_model(self, model_path: str, from_pretrained_kwargs: dict):
-        raise NotImplementedError()
+    def match(self, model_path: str):
+        return model_path == "claude-v1"
 
     def get_default_conv_template(self, model_path: str) -> ConversationHistory:
-        settings = get_conv_settings("bard")
+        settings = get_conv_settings("claude")
         return ConversationHistory(
             system="",
             messages=(),
             offset=0,
             settings=settings,
-        )
+        )
```

### Comparing `langport-0.0.4/langport/model/adapters/billa.py` & `langport-0.1.0/langport/model/adapters/billa.py`

 * *Files identical despite different names*

### Comparing `langport-0.0.4/langport/model/adapters/chatgpt.py` & `langport-0.1.0/langport/model/adapters/falcon.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,19 @@
-from langport.data.conversation import ConversationHistory
+from langport.data.conversation import ConversationHistory, SeparatorStyle
 from langport.data.conversation.conversation_settings import get_conv_settings
 from langport.model.model_adapter import BaseAdapter
 
 
-class ChatGPTAdapter(BaseAdapter):
-    """The model adapter for ChatGPT."""
+class FalconAdapter(BaseAdapter):
+    """The model adapter for falcon"""
 
     def match(self, model_path: str):
-        return model_path == "gpt-3.5-turbo" or model_path == "gpt-4"
-
-    def load_model(self, model_path: str, from_pretrained_kwargs: dict):
-        raise NotImplementedError()
+        return "falcon" in model_path
 
     def get_default_conv_template(self, model_path: str) -> ConversationHistory:
-        settings = get_conv_settings("chatgpt")
+        settings = get_conv_settings("falcon")
         return ConversationHistory(
-            system="You are a helpful assistant.",
+            system="The conversation between human and AI assistant.",
             messages=[],
             offset=0,
             settings=settings,
         )
```

### Comparing `langport-0.0.4/langport/model/adapters/claude.py` & `langport-0.1.0/langport/model/adapters/oasst_pythia.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+from transformers import (
+    AutoModelForCausalLM,
+    AutoTokenizer,
+)
+
 from langport.data.conversation import ConversationHistory, SeparatorStyle
 from langport.data.conversation.conversation_settings import get_conv_settings
 from langport.model.model_adapter import BaseAdapter
 
-
-class ClaudeAdapter(BaseAdapter):
-    """The model adapter for Claude."""
+class OasstPythiaAdapter(BaseAdapter):
+    """The model adapter for OpenAssistant/oasst-sft-1-pythia-12b"""
 
     def match(self, model_path: str):
-        return model_path == "claude-v1"
-
-    def load_model(self, model_path: str, from_pretrained_kwargs: dict):
-        raise NotImplementedError()
-
+        return "oasst" in model_path and "pythia" in model_path
+    
     def get_default_conv_template(self, model_path: str) -> ConversationHistory:
-        settings = get_conv_settings("claude")
+        settings = get_conv_settings("oasst_pythia")
         return ConversationHistory(
-            system="",
+            system="BEGINNING OF CONVERSATION:",
             messages=(),
             offset=0,
             settings=settings,
         )
```

### Comparing `langport-0.0.4/langport/model/adapters/koala.py` & `langport-0.1.0/langport/model/adapters/koala.py`

 * *Files identical despite different names*

### Comparing `langport-0.0.4/langport/model/adapters/oasst_pythia.py` & `langport-0.1.0/langport/model/adapters/phoenix.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,30 +3,21 @@
     AutoTokenizer,
 )
 
 from langport.data.conversation import ConversationHistory, SeparatorStyle
 from langport.data.conversation.conversation_settings import get_conv_settings
 from langport.model.model_adapter import BaseAdapter
 
-class OasstPythiaAdapter(BaseAdapter):
-    """The model adapter for OpenAssistant/oasst-sft-1-pythia-12b"""
+class PhoenixAdapter(BaseAdapter):
+    """The model adapter for FreedomIntelligence/phoenix-inst-chat-7b"""
 
     def match(self, model_path: str):
-        return "oasst" in model_path and "pythia" in model_path
+        return "phoenix" in model_path
 
-    def load_model(self, model_path: str, from_pretrained_kwargs: dict):
-        tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=True)
-        model = AutoModelForCausalLM.from_pretrained(
-            model_path,
-            low_cpu_mem_usage=True,
-            **from_pretrained_kwargs,
-        )
-        return model, tokenizer
-    
     def get_default_conv_template(self, model_path: str) -> ConversationHistory:
-        settings = get_conv_settings("oasst_pythia")
+        settings = get_conv_settings("phoenix")
         return ConversationHistory(
-            system="BEGINNING OF CONVERSATION:",
+            system="A chat between a curious human and an artificial intelligence assistant. The assistant gives helpful, detailed, and polite answers to the human's questions.\n\n",
             messages=(),
             offset=0,
             settings=settings,
         )
```

### Comparing `langport-0.0.4/langport/model/adapters/openbuddy.py` & `langport-0.1.0/langport/model/adapters/openbuddy.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,21 @@
-import warnings
-
-import torch
-from transformers import (
-    LlamaTokenizer,
-    LlamaForCausalLM,
-)
-
-from langport.data.conversation import ConversationHistory, SeparatorStyle
+import os
+from langport.data.conversation import ConversationHistory
 from langport.data.conversation.conversation_settings import get_conv_settings
 from langport.model.model_adapter import BaseAdapter
 
 class OpenBuddyAdapter(BaseAdapter):
-    """The model adapter for OpenBuddy/openbuddy-7b-v1.1-bf16-enc"""
+    """The model adapter for OpenBuddy"""
 
     def match(self, model_path: str):
-        return "openbuddy" in model_path
-
-    def load_model(self, model_path: str, from_pretrained_kwargs: dict):
-        if "-bf16" in model_path:
-            from_pretrained_kwargs["torch_dtype"] = torch.bfloat16
-            warnings.warn(
-                "## This is a bf16(bfloat16) variant of OpenBuddy. Please make sure your GPU supports bf16."
-            )
-        model = LlamaForCausalLM.from_pretrained(
-            model_path, low_cpu_mem_usage=True, **from_pretrained_kwargs
-        )
-        tokenizer = LlamaTokenizer.from_pretrained(model_path)
-        return model, tokenizer
+        if model_path.endswith('/'):
+            model_path = model_path[:-1]
+        dir_name = os.path.basename(model_path)
+        parent_name = os.path.dirname(model_path)
+        return dir_name.startswith('openbuddy') or parent_name.startswith('openbuddy')
 
     def get_default_conv_template(self, model_path: str) -> ConversationHistory:
         settings = get_conv_settings("openbuddy")
         return ConversationHistory(
             system="""Consider a conversation between User (a human) and Assistant (named Buddy).
 Buddy is an INTP-T, a friendly, intelligent and multilingual AI assistant, by OpenBuddy team. GitHub: https://github.com/OpenBuddy/OpenBuddy
 Buddy cannot access the Internet.
@@ -38,11 +23,11 @@
 Buddy can generate poems, stories, code, essays, songs, parodies, and more.
 Buddy possesses vast knowledge about the world, history, and culture.
 Buddy's responses are always safe, creative, high-quality, human-like, and interesting.
 Buddy strictly refuses to discuss political, NSFW, or other unsafe topics.
 
 User: Hi.
 Assistant: Hi, I'm Buddy, your AI assistant. How can I help you today?""",
-            messages=(),
+            messages=[],
             offset=0,
             settings=settings,
         )
```

### Comparing `langport-0.0.4/langport/model/adapters/phoenix.py` & `langport-0.1.0/langport/model/adapters/rwkv.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 from transformers import (
-    AutoModelForCausalLM,
     AutoTokenizer,
 )
 
 from langport.data.conversation import ConversationHistory, SeparatorStyle
 from langport.data.conversation.conversation_settings import get_conv_settings
 from langport.model.model_adapter import BaseAdapter
 
-class PhoenixAdapter(BaseAdapter):
-    """The model adapter for FreedomIntelligence/phoenix-inst-chat-7b"""
 
-    def match(self, model_path: str):
-        return "phoenix" in model_path
+class RwkvAdapter(BaseAdapter):
+    """The model adapter for BlinkDL/RWKV-4-Raven"""
 
-    def load_model(self, model_path: str, from_pretrained_kwargs: dict):
-        tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=True)
-        model = AutoModelForCausalLM.from_pretrained(
-            model_path,
-            low_cpu_mem_usage=True,
-            **from_pretrained_kwargs,
-        )
-        return model, tokenizer
+    def match(self, model_path: str):
+        return "RWKV-4" in model_path
 
     def get_default_conv_template(self, model_path: str) -> ConversationHistory:
-        settings = get_conv_settings("phoenix")
+        settings = get_conv_settings("rwkv")
         return ConversationHistory(
-            system="A chat between a curious human and an artificial intelligence assistant. The assistant gives helpful, detailed, and polite answers to the human's questions.\n\n",
+            system="",
             messages=(),
             offset=0,
             settings=settings,
         )
```

### Comparing `langport-0.0.4/langport/model/adapters/vicuna.py` & `langport-0.1.0/langport/model/adapters/vicuna.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,24 +12,14 @@
 
 class VicunaAdapter(BaseAdapter):
     "Model adapater for vicuna-v1.1"
 
     def match(self, model_path: str):
         return "vicuna" in model_path
 
-    def load_model(self, model_path: str, from_pretrained_kwargs: dict):
-        tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=False)
-        model = AutoModelForCausalLM.from_pretrained(
-            model_path,
-            low_cpu_mem_usage=True,
-            **from_pretrained_kwargs,
-        )
-        self.raise_warning_for_old_weights(model)
-        return model, tokenizer
-
     def get_default_conv_template(self, model_path: str) -> ConversationHistory:
         settings = get_conv_settings("vicuna_v1.1")
         return ConversationHistory(
             system="A chat between a curious user and an artificial intelligence assistant. "
             "The assistant gives helpful, detailed, and polite answers to the user's questions.",
             messages=(),
             offset=0,
```

### Comparing `langport-0.0.4/langport/model/compression.py` & `langport-0.1.0/langport/model/compression.py`

 * *Files identical despite different names*

### Comparing `langport-0.0.4/langport/model/executor/base.py` & `langport-0.1.0/langport/model/executor/base.py`

 * *Files identical despite different names*

### Comparing `langport-0.0.4/langport/model/executor/embedding/__init__.py` & `langport-0.1.0/langport/model/executor/embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `langport-0.0.4/langport/model/executor/embedding/huggingface.py` & `langport-0.1.0/langport/model/executor/embedding/huggingface.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,43 @@
-
-
-
-
 import traceback
 from typing import List, Optional
 
 import torch
-from langport.model.executor.base import LocalModelExecutor
-from langport.model.executor.embedding import EmbeddingExecutor
-from langport.model.executor.huggingface_utils import load_model
+from langport.model.executor.huggingface import HuggingfaceExecutor
 from langport.protocol.worker_protocol import BaseWorkerResult, EmbeddingWorkerResult, UsageInfo
 from langport.workers.embedding_worker import EmbeddingModelWorker
 
 
-class HuggingfaceEmbeddingExecutor(LocalModelExecutor):
+class HuggingfaceEmbeddingExecutor(HuggingfaceExecutor):
     def __init__(
         self,
         model_name: str,
         model_path: str,
         device: str,
         num_gpus: int,
         max_gpu_memory: Optional[str],
         load_8bit: bool,
         cpu_offloading: bool,
         deepspeed: bool = False,
+        trust_remote_code: bool = False,
     ) -> None:
         super(HuggingfaceEmbeddingExecutor, self).__init__(
             model_name=model_name,
             model_path=model_path,
             device=device,
             num_gpus=num_gpus,
             max_gpu_memory=max_gpu_memory,
             load_8bit=load_8bit,
             cpu_offloading=cpu_offloading
         )
         self.adapter = None
         self.model = None
         self.tokenizer = None
-        self.adapter, self.model, self.tokenizer = load_model(
-            model_path, device, num_gpus, max_gpu_memory, load_8bit, cpu_offloading, deepspeed
+        self.adapter, self.model, self.tokenizer = self.load_model(
+            model_path, device, num_gpus, max_gpu_memory, load_8bit, cpu_offloading, deepspeed, trust_remote_code
         )
 
         if hasattr(self.model.config, "max_sequence_length"):
             self._context_len = self.model.config.max_sequence_length
         elif hasattr(self.model.config, "max_position_embeddings"):
             self._context_len = self.model.config.max_position_embeddings
         else:
@@ -52,14 +47,21 @@
     def context_length(self) -> int:
         return self._context_len
 
     def tokenize(self, text: str) -> List[int]:
         input_ids = self.tokenizer(text).input_ids
         return input_ids
     
+    # Mean Pooling - Take attention mask into account for correct averaging
+    def _mean_pooling(self, model_output, attention_mask):
+        token_embeddings = model_output[0]  # First element of model_output contains all token embeddings
+        input_mask_expanded = attention_mask.unsqueeze(-1).expand(token_embeddings.size()).float()
+        return torch.sum(token_embeddings * input_mask_expanded, 1) / torch.clamp(input_mask_expanded.sum(1), min=1e-9)
+    
+    @torch.inference_mode()
     def inference(self, worker: "EmbeddingModelWorker"):
         if not worker.online:
             return
         tasks = worker.fetch_tasks()
         batch_size = len(tasks)
         if batch_size == 0:
             return
@@ -72,33 +74,36 @@
 
             # ValueError: Asking to pad but the tokenizer does not have a padding token.
             # Please select a token to use as `pad_token` `(tokenizer.pad_token = tokenizer.eos_token e.g.)`
             # or add a new pad token via `tokenizer.add_special_tokens({'pad_token': '[PAD]'})`.
             if tokenizer._pad_token is None:
                 tokenizer.pad_token = tokenizer.eos_token
 
-            encoded_prompts = tokenizer(prompts, return_tensors="pt", padding="longest")
-            input_ids = encoded_prompts.input_ids.to(self.device)
+            encoded_prompts = tokenizer(prompts, return_tensors="pt", padding="longest").to(self.device)
+            input_ids = encoded_prompts.input_ids
             if model.config.is_encoder_decoder:
                 decoder_input_ids = torch.full(
                     (batch_size, 1),
                     model.generation_config.decoder_start_token_id,
                     dtype=torch.long,
                     device=self.device,
                 )
                 model_output = model(input_ids, decoder_input_ids=decoder_input_ids, output_hidden_states=True)
                 data = model_output.decoder_hidden_states[-1]
-            else:
+            elif model.config.is_decoder:
                 model_output = model(input_ids, output_hidden_states=True)
                 is_chatglm = "chatglm" in str(type(model)).lower()
                 if is_chatglm:
                     data = model_output.hidden_states[-1].transpose(0, 1)
                 else:
                     data = model_output.hidden_states[-1]
-            embeddings = torch.mean(data, dim=1)
+            else:
+                data = model(**encoded_prompts)
+            # embeddings = torch.mean(data, dim=1)
+            embeddings = self._mean_pooling(data, encoded_prompts['attention_mask'])
             for i in range(batch_size):
                 token_num = len(tokenizer(prompts[i]).input_ids)
                 worker.push_task_result(
                     tasks[i].task_id,
                     EmbeddingWorkerResult(
                         task_id=tasks[i].task_id,
                         type="data",
```

### Comparing `langport-0.0.4/langport/model/executor/generation/chatgpt.py` & `langport-0.1.0/langport/model/executor/generation/chatgpt.py`

 * *Files identical despite different names*

### Comparing `langport-0.0.4/langport/model/model_adapter.py` & `langport-0.1.0/langport/model/model_adapter.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,36 +4,24 @@
 import pkgutil
 import sys
 import os
 from typing import List
 import warnings
 from functools import cache
 
-from transformers import (
-    AutoModelForCausalLM,
-    AutoTokenizer,
-)
-
 from langport.data.conversation import ConversationHistory, SeparatorStyle
 from langport.data.conversation.conversation_settings import get_conv_settings
 
 
 class BaseAdapter:
     """The base and the default model adapter."""
 
-    def match(self, model_path: str):
+    def match(self, model_path: str) -> bool:
         return True
 
-    def load_model(self, model_path: str, from_pretrained_kwargs: dict):
-        tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=False)
-        model = AutoModelForCausalLM.from_pretrained(
-            model_path, low_cpu_mem_usage=True, **from_pretrained_kwargs
-        )
-        return model, tokenizer
-
     def get_default_conv_template(self, model_path: str) -> ConversationHistory:
         settings = get_conv_settings("zero_shot")
         return ConversationHistory(
             system="A chat between a curious human and an artificial intelligence assistant. "
             "The assistant gives helpful, detailed, and polite answers to the human's questions.",
             messages=[],
             offset=2,
@@ -51,14 +39,15 @@
 
 
 @cache
 def get_model_adapter(model_path: str) -> BaseAdapter:
     """Get a model adapter for a model_path."""
     for adapter in model_adapters:
         if adapter.match(model_path):
+            print(f"Using model adapter {adapter.__class__.__name__}")
             return adapter
     raise ValueError(f"No valid model adapter for {model_path}")
 
 
 def raise_warning_for_incompatible_cpu_offloading_configuration(
     device: str, load_8bit: bool, cpu_offloading: bool
 ):
```

### Comparing `langport-0.0.4/langport/model/model_args.py` & `langport-0.1.0/langport/model/model_args.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,8 +31,11 @@
     parser.add_argument(
         "--cpu-offloading",
         action="store_true",
         help="Only when using 8-bit quantization: Offload excess weights to the CPU that don't fit on the GPU",
     )
     parser.add_argument(
         "--deepspeed", action="store_true", help="Use deepspeed"
+    )
+    parser.add_argument(
+        "--trust-remote-code", action="store_true", help="Trust remote code"
     )
```

### Comparing `langport-0.0.4/langport/model/models/rwkv_model.py` & `langport-0.1.0/langport/model/models/rwkv_model.py`

 * *Files identical despite different names*

### Comparing `langport-0.0.4/langport/model/monkey_patch_non_inplace.py` & `langport-0.1.0/langport/model/monkey_patch_non_inplace.py`

 * *Files identical despite different names*

### Comparing `langport-0.0.4/langport/protocol/openai_api_protocol.py` & `langport-0.1.0/langport/protocol/openai_api_protocol.py`

 * *Files identical despite different names*

### Comparing `langport-0.0.4/langport/protocol/worker_protocol.py` & `langport-0.1.0/langport/protocol/worker_protocol.py`

 * *Files identical despite different names*

### Comparing `langport-0.0.4/langport/routers/server/core_node.py` & `langport-0.1.0/langport/routers/server/core_node.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,12 @@
-import argparse
-import asyncio
-import os
-import random
-import time
-from typing import List, Union
-import threading
-import uuid
-
-from fastapi import FastAPI, Request, BackgroundTasks
-from fastapi.responses import StreamingResponse, JSONResponse
-
-import uvicorn
-from langport.model.model_args import add_model_args
-from langport.protocol.worker_protocol import EmbeddingsTask, GetNodeStateRequest, HeartbeatPing, NodeInfoRequest, NodeListRequest, RegisterNodeRequest, RemoveNodeRequest, WorkerAddressRequest
-from langport.utils import build_logger
+from fastapi import FastAPI, BackgroundTasks
+from langport.protocol.worker_protocol import GetNodeStateRequest, HeartbeatPing, NodeInfoRequest, NodeListRequest, RegisterNodeRequest, RemoveNodeRequest, WorkerAddressRequest
 
 app = FastAPI()
 
-
 def create_background_tasks(worker):
     background_tasks = BackgroundTasks()
     background_tasks.add_task(lambda: worker.release_model_semaphore())
     return background_tasks
 
 @app.on_event("startup")
 async def startup_event():
```

### Comparing `langport-0.0.4/langport/routers/server/embedding_node.py` & `langport-0.1.0/langport/routers/server/embedding_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.0.4/langport/routers/server/generation_node.py` & `langport-0.1.0/langport/routers/server/generation_node.py`

 * *Files identical despite different names*

### Comparing `langport-0.0.4/langport/service/server/chatgpt_generation_worker.py` & `langport-0.1.0/langport/service/server/chatgpt_generation_worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,15 @@
 import argparse
-import asyncio
 import os
 import random
-import time
-from typing import List, Union
-import threading
+import uvicorn
 import uuid
 
-from fastapi import FastAPI, Request, BackgroundTasks
-from fastapi.responses import StreamingResponse, JSONResponse
-
 from langport.workers.generation_worker import GenerationModelWorker
-
-import uvicorn
-
 from langport.utils import build_logger
-
 from langport.routers.server.generation_node import app
 
 
 # We suggest that concurrency == batch * thread (thread == 4)
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--host", type=str, default="localhost")
```

### Comparing `langport-0.0.4/langport/service/server/dummy_worker.py` & `langport-0.1.0/langport/service/server/dummy_worker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,15 @@
 import argparse
-import asyncio
-from typing import List, Union
 import uuid
-
-from fastapi import FastAPI, Request
-from fastapi.responses import StreamingResponse
-import numpy as np
-import requests
 import uvicorn
 
-from langport.core.cluster_node import ClusterNode
 from langport.core.cluster_worker import ClusterWorker
 from langport.utils import build_logger
-
 from langport.routers.server.core_node import app
+from langport.utils.cache_state import CacheState
 
 logger = build_logger("langport.service.dummy_worker", "dummy_worker.log")
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--host", type=str, default="localhost")
     parser.add_argument("--port", type=int, default=21001)
@@ -32,8 +24,9 @@
         node_id=node_id,
         init_neighborhoods_addr=args.neighbors,
         limit_model_concurrency=32,
         max_batch=1,
         stream_interval=2,
         logger=logger,
     )
+    app.node.states["model_name"] = CacheState("dummy_node", 360)
     uvicorn.run(app, host=args.host, port=args.port, log_level="info")
```

### Comparing `langport-0.0.4/langport/service/server/embedding_worker.py` & `langport-0.1.0/langport/service/server/embedding_worker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 import argparse
-import asyncio
 import os
 import random
-import time
-from typing import List, Union
-import threading
 import uuid
-from langport.model.executor.embedding.huggingface import HuggingfaceEmbeddingExecutor
+import uvicorn
 
 from langport.workers.embedding_worker import EmbeddingModelWorker
-
-import uvicorn
+from langport.model.executor.embedding.huggingface import HuggingfaceEmbeddingExecutor
 from langport.model.model_args import add_model_args
 from langport.utils import build_logger
-
 from langport.routers.server.embedding_node import app
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--host", type=str, default="localhost")
     parser.add_argument("--port", type=int, default=None)
     parser.add_argument("--worker-address", type=str, default=None)
@@ -61,14 +55,15 @@
         model_path=args.model_path,
         device=args.device,
         num_gpus=args.num_gpus,
         max_gpu_memory=args.max_gpu_memory,
         load_8bit=args.load_8bit,
         cpu_offloading=args.cpu_offloading,
         deepspeed=args.deepspeed,
+        trust_remote_code=args.trust_remote_code
     )
 
     app.node = EmbeddingModelWorker(
         node_addr=args.worker_address,
         node_id=node_id,
         init_neighborhoods_addr=args.neighbors,
         executor=executor,
```

### Comparing `langport-0.0.4/langport/service/server/generation_worker.py` & `langport-0.1.0/langport/service/server/generation_worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 import argparse
-import asyncio
 import os
 import random
-import time
-from typing import List, Union
-import threading
 import uuid
-
-from fastapi import FastAPI, Request, BackgroundTasks
-from fastapi.responses import StreamingResponse, JSONResponse
-
-from langport.workers.generation_worker import GenerationModelWorker
-
 import uvicorn
 
+from langport.workers.generation_worker import GenerationModelWorker
 from langport.model.model_args import add_model_args
 from langport.utils import build_logger
-
 from langport.routers.server.generation_node import app
 
 
 # We suggest that concurrency == batch * thread (thread == 4)
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--host", type=str, default="localhost")
@@ -61,14 +51,15 @@
         model_path=args.model_path,
         device=args.device,
         num_gpus=args.num_gpus,
         max_gpu_memory=args.max_gpu_memory,
         load_8bit=args.load_8bit,
         cpu_offloading=args.cpu_offloading,
         deepspeed=args.deepspeed,
+        trust_remote_code=args.trust_remote_code
     )
 
     app.node = GenerationModelWorker(
         node_addr=args.worker_address,
         node_id=node_id,
         init_neighborhoods_addr=args.neighbors,
         executor=executor,
```

### Comparing `langport-0.0.4/langport/utils/__init__.py` & `langport-0.1.0/langport/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,15 +85,19 @@
     def __init__(self, logger, log_level=logging.INFO):
         self.terminal = sys.stdout
         self.logger = logger
         self.log_level = log_level
         self.linebuf = ""
 
     def __getattr__(self, attr):
-        return getattr(self.terminal, attr)
+        try:
+            attr_value = getattr(self.terminal, attr)
+        except:
+            return None
+        return attr_value
 
     def write(self, buf):
         temp_linebuf = self.linebuf + buf
         self.linebuf = ""
         for line in temp_linebuf.splitlines(True):
             # From the io.TextIOWrapper docs:
             #   On output, if newline is None, any '\n' characters written
```

### Comparing `langport-0.0.4/langport/utils/evaluation.py` & `langport-0.1.0/langport/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `langport-0.0.4/langport/utils/interval_timer.py` & `langport-0.1.0/langport/utils/interval_timer.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,33 +38,35 @@
 
     def function_wrapper(
         self,
         args: Optional[Iterable[Any]] = None,
         kwargs: Optional[Mapping[str, Any]] = None,
     ):
         try:
-            loop = asyncio.new_event_loop()
             if inspect.iscoroutinefunction(self.fn):
+                loop = asyncio.new_event_loop()
+                asyncio.set_event_loop(loop)
                 loop.run_until_complete(self.fn(*args, **kwargs))
+                loop.close()
             else:
                 self.fn(*args, **kwargs)
         except:
             traceback.print_exc()
 
     def run(self):
         while True:
             if self.is_activated:
                 start_time = time.time()
                 if start_time - self.last_time > self.interval:
                     self._executor.submit(self.function_wrapper, self.args, self.kwargs)
-                    finish_time = time.time()
-                    self.last_time = finish_time
-                    if finish_time - start_time > self.interval:
-                        print(
-                            f"Overloaded!! Last timer using {finish_time - start_time}s."
-                        )
-                    else:
-                        time.sleep(0.01)
+                    self.last_time = time.time()
+                    # Never run this code, because finish_time - start_time = 0.
+                    # if finish_time - start_time > self.interval:
+                    #     print(
+                    #         f"Overloaded!! Last timer using {finish_time - start_time}s."
+                    #     )
+                    # else:
+                        # time.sleep(0.01)
                 else:
                     time.sleep(0.01)
             else:
                 break
```

### Comparing `langport-0.0.4/langport/workers/embedding_worker.py` & `langport-0.1.0/langport/workers/embedding_worker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-import argparse
-import asyncio
-import dataclasses
-import logging
-import json
-import os
-import time
 from typing import List, Optional, Union
 import threading
 import uuid
 
 from fastapi import FastAPI, Request, BackgroundTasks
 from fastapi.responses import StreamingResponse, JSONResponse
 import requests
```

### Comparing `langport-0.0.4/langport/workers/generation_worker.py` & `langport-0.1.0/langport/workers/generation_worker.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,20 @@
-import argparse
-import asyncio
-import dataclasses
-import logging
 import json
-import os
-import time
-from typing import Iterable, List, Optional, Union
-import threading
-import uuid
-import traceback
-
-from fastapi import FastAPI, Request, BackgroundTasks
-from fastapi.responses import StreamingResponse, JSONResponse
-import requests
-from tenacity import retry, stop_after_attempt
+from typing import List
+
 from langport.core.cluster_worker import ClusterWorker
-from langport.model.executor.base import BaseModelExecutor
 from langport.model.executor.generation import GenerationExecutor
 
 from langport.protocol.worker_protocol import (
     BaseWorkerResult,
     GenerationTask,
     GenerationWorkerResult,
     UsageInfo,
 )
 
-import torch
-
-from transformers import PreTrainedModel, PreTrainedTokenizerBase
-from transformers.generation.logits_process import (
-    LogitsProcessor,
-    LogitsProcessorList,
-    TemperatureLogitsWarper,
-    RepetitionPenaltyLogitsProcessor,
-    TopPLogitsWarper,
-    TopKLogitsWarper,
-)
 from langport.constants import (
     GENERATION_INFERENCE_INTERVAL,
     WORKER_API_TIMEOUT,
     WORKER_HEART_BEAT_INTERVAL,
     ErrorCode,
 )
 from langport.utils import server_error_msg, pretty_print_semaphore
@@ -88,15 +63,15 @@
 
 
     async def generation_stream(self, task: GenerationTask):
         prompt_tokens = len(self.executor.tokenize(task.prompt))
         max_tokens = task.max_tokens
         context_length = self.executor.context_length
 
-        if prompt_tokens + max_tokens > context_length:
+        if context_length is not None and prompt_tokens + max_tokens > context_length:
             yield BaseWorkerResult(task_id=task.task_id,
                                    type="error",
                                    message=f"This model's maximum context length is {context_length} tokens. "
                                     f"However, you requested {max_tokens + prompt_tokens} tokens "
                                     f"({prompt_tokens} in the messages, "
                                     f"{max_tokens} in the completion). "
                                     f"Please reduce the length of the messages or completion.",
```

### Comparing `langport-0.0.4/langport.egg-info/PKG-INFO` & `langport-0.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6c61 6e67  : 2.1.Name: lang
 00000020: 706f 7274 0a56 6572 7369 6f6e 3a20 302e  port.Version: 0.
-00000030: 302e 340a 5375 6d6d 6172 793a 2041 206c  0.4.Summary: A l
+00000030: 312e 300a 5375 6d6d 6172 793a 2041 206c  1.0.Summary: A l
 00000040: 6172 6765 206c 616e 6775 6167 6520 6d6f  arge language mo
 00000050: 6465 6c20 7365 7276 696e 6720 706c 6174  del serving plat
 00000060: 666f 726d 2e0a 5072 6f6a 6563 742d 5552  form..Project-UR
 00000070: 4c3a 2048 6f6d 6570 6167 652c 2068 7474  L: Homepage, htt
 00000080: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
 00000090: 7674 7562 6572 2d70 6c61 6e2f 6c61 6e67  vtuber-plan/lang
 000000a0: 706f 7274 0a50 726f 6a65 6374 2d55 524c  port.Project-URL
@@ -21,220 +21,318 @@
 00000140: 6420 3a3a 2041 7061 6368 6520 536f 6674  d :: Apache Soft
 00000150: 7761 7265 204c 6963 656e 7365 0a52 6571  ware License.Req
 00000160: 7569 7265 732d 5079 7468 6f6e 3a20 3e3d  uires-Python: >=
 00000170: 332e 380a 4465 7363 7269 7074 696f 6e2d  3.8.Description-
 00000180: 436f 6e74 656e 742d 5479 7065 3a20 7465  Content-Type: te
 00000190: 7874 2f6d 6172 6b64 6f77 6e0a 5072 6f76  xt/markdown.Prov
 000001a0: 6964 6573 2d45 7874 7261 3a20 6465 760a  ides-Extra: dev.
-000001b0: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
-000001c0: 4345 4e53 450a 0a23 206c 616e 6770 6f72  CENSE..# langpor
-000001d0: 740a 4c61 6e67 506f 7274 2069 7320 6120  t.LangPort is a 
-000001e0: 6f70 656e 2d73 6f75 7263 6520 6c61 7267  open-source larg
-000001f0: 6520 6c61 6e67 7561 6765 206d 6f64 656c  e language model
-00000200: 2073 6572 7669 6e67 2070 6c61 7466 6f72   serving platfor
-00000210: 6d2e 0a4f 7572 2067 6f61 6c20 6973 2074  m..Our goal is t
-00000220: 6f20 6275 696c 6420 6120 7375 7065 7220  o build a super 
-00000230: 6661 7374 204c 4c4d 2069 6e66 6572 656e  fast LLM inferen
-00000240: 6365 2073 6572 7669 6365 2e0a 0a54 6869  ce service...Thi
-00000250: 7320 7072 6f6a 6563 7420 6973 2069 6e73  s project is ins
-00000260: 7069 7265 6420 6279 205b 6c6d 7379 732f  pired by [lmsys/
-00000270: 6661 7374 6368 6174 5d28 6874 7470 733a  fastchat](https:
-00000280: 2f2f 6769 7468 7562 2e63 6f6d 2f6c 6d2d  //github.com/lm-
-00000290: 7379 732f 4661 7374 4368 6174 292c 2077  sys/FastChat), w
-000002a0: 6520 686f 7065 2074 6861 7420 7468 6520  e hope that the 
-000002b0: 7365 7276 696e 6720 706c 6174 666f 726d  serving platform
-000002c0: 2069 7320 6c69 6768 7477 6569 6768 7420   is lightweight 
-000002d0: 616e 6420 6661 7374 2c20 6275 7420 6661  and fast, but fa
-000002e0: 7374 6368 6174 2069 6e63 6c75 6465 7320  stchat includes 
-000002f0: 6f74 6865 7220 6665 6174 7572 6573 2073  other features s
-00000300: 7563 6820 6173 2074 7261 696e 696e 6720  uch as training 
-00000310: 616e 6420 6576 616c 7561 7469 6f6e 206d  and evaluation m
-00000320: 616b 6520 6974 2063 6f6d 706c 6963 6174  ake it complicat
-00000330: 6564 2e0a 0a54 6865 2063 6f72 6520 6665  ed...The core fe
-00000340: 6174 7572 6573 2069 6e63 6c75 6465 3a0a  atures include:.
-00000350: 2d20 4120 6469 7374 7269 6275 7465 6420  - A distributed 
-00000360: 7365 7276 696e 6720 7379 7374 656d 2066  serving system f
-00000370: 6f72 2073 7461 7465 2d6f 662d 7468 652d  or state-of-the-
-00000380: 6172 7420 6d6f 6465 6c73 2e0a 2d20 5374  art models..- St
-00000390: 7265 616d 696e 6720 4150 4920 696e 7465  reaming API inte
-000003a0: 7266 6163 6520 7375 7070 6f72 742e 0a2d  rface support..-
-000003b0: 2042 6174 6368 2069 6e66 6572 656e 6365   Batch inference
-000003c0: 2066 6f72 2068 6967 6865 7220 7468 726f   for higher thro
-000003d0: 7567 6870 7574 2e0a 2d20 4f70 656e 4149  ughput..- OpenAI
-000003e0: 2d43 6f6d 7061 7469 626c 6520 5245 5354  -Compatible REST
-000003f0: 6675 6c20 4150 4973 2e0a 2d20 4661 7578  ful APIs..- Faux
-00000400: 5069 6c6f 742d 436f 6d70 6174 6962 6c65  Pilot-Compatible
-00000410: 2052 4553 5466 756c 2041 5049 732e 0a0a   RESTful APIs...
-00000420: 2323 2042 656e 6368 6d61 726b 0a57 6520  ## Benchmark.We 
-00000430: 7573 6520 7369 6e67 6c65 2052 5458 3330  use single RTX30
-00000440: 3930 2074 6f20 7275 6e20 6120 6669 6e65  90 to run a fine
-00000450: 7475 6e65 6420 3742 204c 4c61 4d41 206d  tuned 7B LLaMA m
-00000460: 6f64 656c 2028 4f70 656e 4275 6464 7920  odel (OpenBuddy 
-00000470: 5630 2e39 2920 696e 2074 6865 2062 6631  V0.9) in the bf1
-00000480: 3620 7365 7474 696e 672e 2057 6520 6372  6 setting. We cr
-00000490: 6561 7465 2033 3220 7468 7265 6164 7320  eate 32 threads 
-000004a0: 746f 2073 7562 6d69 7420 6368 6174 2074  to submit chat t
-000004b0: 6173 6b73 2074 6f20 7468 6520 7365 7276  asks to the serv
-000004c0: 6572 2c20 616e 6420 7468 6520 666f 6c6c  er, and the foll
-000004d0: 6f77 696e 6720 6669 6775 7265 2073 686f  owing figure sho
-000004e0: 7773 2074 6865 2051 7565 7269 6573 2050  ws the Queries P
-000004f0: 6572 2053 6563 6f6e 6420 2851 5053 2920  er Second (QPS) 
-00000500: 616e 6420 546f 6b65 6e73 2050 6572 2053  and Tokens Per S
-00000510: 6563 6f6e 6420 2854 5053 2920 6f66 2046  econd (TPS) of F
-00000520: 6173 7443 6861 7420 616e 6420 4c61 6e67  astChat and Lang
-00000530: 506f 7274 2077 6974 6820 6469 6666 6572  Port with differ
-00000540: 656e 7420 6d61 7820 6d6f 6465 6c20 636f  ent max model co
-00000550: 6e63 7572 7265 6e63 7920 7365 7474 696e  ncurrency settin
-00000560: 6773 2e0a 0a21 5b62 656e 6368 6d61 726b  gs...![benchmark
-00000570: 5f63 6861 745d 2864 6f63 732f 6265 6e63  _chat](docs/benc
-00000580: 686d 6172 6b5f 6368 6174 2e6a 7067 290a  hmark_chat.jpg).
-00000590: 0a0a 2323 204e 6577 730a 2d20 5b32 3032  ..## News.- [202
-000005a0: 332f 3035 2f31 305d 204c 616e 6770 6f72  3/05/10] Langpor
-000005b0: 7420 7072 6f6a 6563 7420 7374 6172 7465  t project starte
-000005c0: 642e 0a2d 205b 3230 3233 2f30 352f 3134  d..- [2023/05/14
-000005d0: 5d20 4261 7463 6820 696e 6665 7265 6e63  ] Batch inferenc
-000005e0: 6520 7375 7070 6f72 7465 642e 0a2d 205b  e supported..- [
-000005f0: 3230 3233 2f30 352f 3232 5d20 4e65 7720  2023/05/22] New 
-00000600: 6469 7374 7269 6275 7465 6420 6172 6368  distributed arch
-00000610: 6974 6563 7475 7265 2e0a 2d20 5b32 3032  itecture..- [202
-00000620: 332f 3035 2f32 335d 2041 6464 2063 6861  3/05/23] Add cha
-00000630: 7420 7468 726f 7567 6870 7574 2074 6573  t throughput tes
-00000640: 7420 7363 7269 7074 2e0a 0a0a 2323 2049  t script....## I
-00000650: 6e73 7461 6c6c 0a0a 2323 2320 4d65 7468  nstall..### Meth
-00000660: 6f64 2031 3a20 5769 7468 2070 6970 0a0a  od 1: With pip..
-00000670: 6060 6062 6173 680a 7069 7033 2069 6e73  ```bash.pip3 ins
-00000680: 7461 6c6c 2067 6974 2b68 7474 7073 3a2f  tall git+https:/
-00000690: 2f67 6974 6875 622e 636f 6d2f 7674 7562  /github.com/vtub
-000006a0: 6572 2d70 6c61 6e2f 6c61 6e67 706f 7274  er-plan/langport
-000006b0: 2e67 6974 200a 6060 600a 0a23 2323 204d  .git .```..### M
-000006c0: 6574 686f 6420 323a 2046 726f 6d20 736f  ethod 2: From so
-000006d0: 7572 6365 0a0a 312e 2043 6c6f 6e65 2074  urce..1. Clone t
-000006e0: 6869 7320 7265 706f 7369 746f 7279 0a60  his repository.`
-000006f0: 6060 6261 7368 0a67 6974 2063 6c6f 6e65  ``bash.git clone
-00000700: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000710: 636f 6d2f 7674 7562 6572 2d70 6c61 6e2f  com/vtuber-plan/
-00000720: 6c61 6e67 706f 7274 2e67 6974 0a63 6420  langport.git.cd 
-00000730: 6c61 6e67 706f 7274 0a60 6060 0a0a 322e  langport.```..2.
-00000740: 2049 6e73 7461 6c6c 2074 6865 2050 6163   Install the Pac
-00000750: 6b61 6765 0a60 6060 6261 7368 0a70 6970  kage.```bash.pip
-00000760: 2069 6e73 7461 6c6c 202d 2d75 7067 7261   install --upgra
-00000770: 6465 2070 6970 0a70 6970 2069 6e73 7461  de pip.pip insta
-00000780: 6c6c 202d 6520 2e0a 6060 600a 0a23 2320  ll -e ..```..## 
-00000790: 5374 6172 7420 7468 6520 7365 7276 6572  Start the server
-000007a0: 0a0a 4974 2069 7320 7369 6d70 6c65 2074  ..It is simple t
-000007b0: 6f20 7374 6172 7420 6120 7369 6e67 6c65  o start a single
-000007c0: 206e 6f64 6520 6368 6174 2041 5049 2073   node chat API s
-000007d0: 6572 7669 6365 3a0a 6060 6020 6261 7368  ervice:.``` bash
-000007e0: 0a70 7974 686f 6e20 2d6d 206c 616e 6770  .python -m langp
-000007f0: 6f72 742e 7365 7276 6963 652e 7365 7276  ort.service.serv
-00000800: 6572 2e67 656e 6572 6174 696f 6e5f 776f  er.generation_wo
-00000810: 726b 6572 202d 2d70 6f72 7420 3231 3030  rker --port 2100
-00000820: 3120 2d2d 6d6f 6465 6c2d 7061 7468 203c  1 --model-path <
-00000830: 796f 7572 206d 6f64 656c 2070 6174 683e  your model path>
-00000840: 0a70 7974 686f 6e20 2d6d 206c 616e 6770  .python -m langp
-00000850: 6f72 742e 7365 7276 6963 652e 6761 7465  ort.service.gate
-00000860: 7761 792e 6f70 656e 6169 5f61 7069 0a60  way.openai_api.`
-00000870: 6060 0a0a 4966 2079 6f75 206e 6565 6420  ``..If you need 
-00000880: 7468 6520 656d 6265 6464 696e 6773 2041  the embeddings A
-00000890: 5049 206f 7220 6f74 6865 7220 6665 6174  PI or other feat
-000008a0: 7572 6573 2c20 796f 7520 6361 6e20 6465  ures, you can de
-000008b0: 706c 6f79 2061 2064 6973 7472 6962 7574  ploy a distribut
-000008c0: 6564 2069 6e66 6572 656e 6365 2063 6c75  ed inference clu
-000008d0: 7374 6572 3a0a 6060 6020 6261 7368 0a70  ster:.``` bash.p
-000008e0: 7974 686f 6e20 2d6d 206c 616e 6770 6f72  ython -m langpor
-000008f0: 742e 7365 7276 6963 652e 7365 7276 6572  t.service.server
-00000900: 2e64 756d 6d79 5f77 6f72 6b65 7220 2d2d  .dummy_worker --
-00000910: 706f 7274 2032 3130 3031 0a70 7974 686f  port 21001.pytho
-00000920: 6e20 2d6d 206c 616e 6770 6f72 742e 7365  n -m langport.se
-00000930: 7276 6963 652e 7365 7276 6572 2e67 656e  rvice.server.gen
-00000940: 6572 6174 696f 6e5f 776f 726b 6572 202d  eration_worker -
-00000950: 2d6d 6f64 656c 2d70 6174 6820 3c79 6f75  -model-path <you
-00000960: 7220 6d6f 6465 6c20 7061 7468 3e20 2d2d  r model path> --
-00000970: 6e65 6967 6862 6f72 7320 6874 7470 3a2f  neighbors http:/
-00000980: 2f6c 6f63 616c 686f 7374 3a32 3130 3031  /localhost:21001
-00000990: 0a70 7974 686f 6e20 2d6d 206c 616e 6770  .python -m langp
-000009a0: 6f72 742e 7365 7276 6963 652e 7365 7276  ort.service.serv
-000009b0: 6572 2e65 6d62 6564 6469 6e67 5f77 6f72  er.embedding_wor
-000009c0: 6b65 7220 2d2d 6d6f 6465 6c2d 7061 7468  ker --model-path
-000009d0: 203c 796f 7572 206d 6f64 656c 2070 6174   <your model pat
-000009e0: 683e 202d 2d6e 6569 6768 626f 7273 2068  h> --neighbors h
-000009f0: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
-00000a00: 3231 3030 310a 7079 7468 6f6e 202d 6d20  21001.python -m 
-00000a10: 6c61 6e67 706f 7274 2e73 6572 7669 6365  langport.service
-00000a20: 2e67 6174 6577 6179 2e6f 7065 6e61 695f  .gateway.openai_
-00000a30: 6170 6920 2d2d 636f 6e74 726f 6c6c 6572  api --controller
-00000a40: 2d61 6464 7265 7373 2068 7474 703a 2f2f  -address http://
-00000a50: 6c6f 6361 6c68 6f73 743a 3231 3030 310a  localhost:21001.
-00000a60: 6060 600a 0a49 6e20 7072 6163 7469 6365  ```..In practice
-00000a70: 2c20 7468 6520 6761 7465 7761 7920 6361  , the gateway ca
-00000a80: 6e20 636f 6e6e 6563 7420 746f 2061 6e79  n connect to any
-00000a90: 206e 6f64 6520 746f 2064 6973 7472 6962   node to distrib
-00000aa0: 7574 6520 696e 6665 7265 6e63 6520 7461  ute inference ta
-00000ab0: 736b 733a 0a0a 6060 6020 6261 7368 0a70  sks:..``` bash.p
-00000ac0: 7974 686f 6e20 2d6d 206c 616e 6770 6f72  ython -m langpor
-00000ad0: 742e 7365 7276 6963 652e 7365 7276 6572  t.service.server
-00000ae0: 2e64 756d 6d79 5f77 6f72 6b65 7220 2d2d  .dummy_worker --
-00000af0: 706f 7274 2032 3130 3031 0a70 7974 686f  port 21001.pytho
-00000b00: 6e20 2d6d 206c 616e 6770 6f72 742e 7365  n -m langport.se
-00000b10: 7276 6963 652e 7365 7276 6572 2e67 656e  rvice.server.gen
-00000b20: 6572 6174 696f 6e5f 776f 726b 6572 202d  eration_worker -
-00000b30: 2d70 6f72 7420 3231 3030 3220 2d2d 6d6f  -port 21002 --mo
-00000b40: 6465 6c2d 7061 7468 203c 796f 7572 206d  del-path <your m
-00000b50: 6f64 656c 2070 6174 683e 202d 2d6e 6569  odel path> --nei
-00000b60: 6768 626f 7273 2068 7474 703a 2f2f 6c6f  ghbors http://lo
-00000b70: 6361 6c68 6f73 743a 3231 3030 310a 7079  calhost:21001.py
-00000b80: 7468 6f6e 202d 6d20 6c61 6e67 706f 7274  thon -m langport
-00000b90: 2e73 6572 7669 6365 2e73 6572 7665 722e  .service.server.
-00000ba0: 6765 6e65 7261 7469 6f6e 5f77 6f72 6b65  generation_worke
-00000bb0: 7220 2d2d 706f 7274 2032 3130 3033 202d  r --port 21003 -
-00000bc0: 2d6d 6f64 656c 2d70 6174 6820 3c79 6f75  -model-path <you
-00000bd0: 7220 6d6f 6465 6c20 7061 7468 3e20 2d2d  r model path> --
-00000be0: 6e65 6967 6862 6f72 7320 6874 7470 3a2f  neighbors http:/
-00000bf0: 2f6c 6f63 616c 686f 7374 3a32 3130 3031  /localhost:21001
-00000c00: 2068 7474 703a 2f2f 6c6f 6361 6c68 6f73   http://localhos
-00000c10: 743a 3231 3030 320a 7079 7468 6f6e 202d  t:21002.python -
-00000c20: 6d20 6c61 6e67 706f 7274 2e73 6572 7669  m langport.servi
-00000c30: 6365 2e73 6572 7665 722e 6765 6e65 7261  ce.server.genera
-00000c40: 7469 6f6e 5f77 6f72 6b65 7220 2d2d 706f  tion_worker --po
-00000c50: 7274 2032 3130 3034 202d 2d6d 6f64 656c  rt 21004 --model
-00000c60: 2d70 6174 6820 3c79 6f75 7220 6d6f 6465  -path <your mode
-00000c70: 6c20 7061 7468 3e20 2d2d 6e65 6967 6862  l path> --neighb
-00000c80: 6f72 7320 6874 7470 3a2f 2f6c 6f63 616c  ors http://local
-00000c90: 686f 7374 3a32 3130 3031 2068 7474 703a  host:21001 http:
-00000ca0: 2f2f 6c6f 6361 6c68 6f73 743a 3231 3030  //localhost:2100
-00000cb0: 330a 7079 7468 6f6e 202d 6d20 6c61 6e67  3.python -m lang
-00000cc0: 706f 7274 2e73 6572 7669 6365 2e73 6572  port.service.ser
-00000cd0: 7665 722e 6765 6e65 7261 7469 6f6e 5f77  ver.generation_w
-00000ce0: 6f72 6b65 7220 2d2d 706f 7274 2032 3130  orker --port 210
-00000cf0: 3035 202d 2d6d 6f64 656c 2d70 6174 6820  05 --model-path 
-00000d00: 3c79 6f75 7220 6d6f 6465 6c20 7061 7468  <your model path
-00000d10: 3e20 2d2d 6e65 6967 6862 6f72 7320 6874  > --neighbors ht
-00000d20: 7470 3a2f 2f6c 6f63 616c 686f 7374 3a32  tp://localhost:2
-00000d30: 3130 3031 2068 7474 703a 2f2f 6c6f 6361  1001 http://loca
-00000d40: 6c68 6f73 743a 3231 3030 340a 7079 7468  lhost:21004.pyth
-00000d50: 6f6e 202d 6d20 6c61 6e67 706f 7274 2e73  on -m langport.s
-00000d60: 6572 7669 6365 2e67 6174 6577 6179 2e6f  ervice.gateway.o
-00000d70: 7065 6e61 695f 6170 6920 2d2d 636f 6e74  penai_api --cont
-00000d80: 726f 6c6c 6572 2d61 6464 7265 7373 2068  roller-address h
-00000d90: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
-00000da0: 3231 3030 3320 2320 3231 3030 3320 6973  21003 # 21003 is
-00000db0: 204f 4b21 0a70 7974 686f 6e20 2d6d 206c   OK!.python -m l
-00000dc0: 616e 6770 6f72 742e 7365 7276 6963 652e  angport.service.
-00000dd0: 6761 7465 7761 792e 6f70 656e 6169 5f61  gateway.openai_a
-00000de0: 7069 202d 2d63 6f6e 7472 6f6c 6c65 722d  pi --controller-
-00000df0: 6164 6472 6573 7320 6874 7470 3a2f 2f6c  address http://l
-00000e00: 6f63 616c 686f 7374 3a32 3130 3032 2023  ocalhost:21002 #
-00000e10: 2041 6e79 2077 6f72 6b65 7220 6973 2061   Any worker is a
-00000e20: 6c73 6f20 4f4b 210a 6060 600a 0a23 2320  lso OK!.```..## 
-00000e30: 4c69 6365 6e73 650a 0a6c 616e 6770 6f72  License..langpor
-00000e40: 7420 6973 2072 656c 6561 7365 6420 756e  t is released un
-00000e50: 6465 7220 7468 6520 4170 6163 6865 2053  der the Apache S
-00000e60: 6f66 7477 6172 6520 4c69 6365 6e73 652e  oftware License.
-00000e70: 0a0a 0a23 2320 5365 6520 616c 736f 0a0a  ...## See also..
-00000e80: 2d20 5b6c 616e 6770 6f72 742d 646f 6373  - [langport-docs
-00000e90: 5d28 6874 7470 733a 2f2f 6c61 6e67 706f  ](https://langpo
-00000ea0: 7274 2e72 6561 6474 6865 646f 6373 2e69  rt.readthedocs.i
-00000eb0: 6f2f 290a 2d20 5b6c 616e 6770 6f72 742d  o/).- [langport-
-00000ec0: 736f 7572 6365 5d28 6874 7470 733a 2f2f  source](https://
-00000ed0: 6769 7468 7562 2e63 6f6d 2f76 7475 6265  github.com/vtube
-00000ee0: 722d 706c 616e 2f6c 616e 6770 6f72 7429  r-plan/langport)
-00000ef0: 0a                                       .
+000001b0: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
+000001c0: 6c6c 616d 6163 7070 0a4c 6963 656e 7365  llamacpp.License
+000001d0: 2d46 696c 653a 204c 4943 454e 5345 0a0a  -File: LICENSE..
+000001e0: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+000001f0: 6572 223e 0a0a 2320 4c61 6e67 506f 7274  er">..# LangPort
+00000200: 0a0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
+00000210: 3a2f 2f67 6974 6875 622e 636f 6d2f 7674  ://github.com/vt
+00000220: 7562 6572 2d70 6c61 6e2f 6c61 6e67 706f  uber-plan/langpo
+00000230: 7274 223e 0a20 203c 696d 6720 616c 743d  rt">.  <img alt=
+00000240: 2247 6974 4875 6220 5265 706f 2073 7461  "GitHub Repo sta
+00000250: 7273 2220 7372 633d 2268 7474 7073 3a2f  rs" src="https:/
+00000260: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000270: 6769 7468 7562 2f73 7461 7273 2f76 7475  github/stars/vtu
+00000280: 6265 722d 706c 616e 2f6c 616e 6770 6f72  ber-plan/langpor
+00000290: 743f 7374 796c 653d 736f 6369 616c 223e  t?style=social">
+000002a0: 0a3c 2f61 3e0a 3c61 2068 7265 663d 2268  .</a>.<a href="h
+000002b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000002c0: 6d2f 7674 7562 6572 2d70 6c61 6e2f 6c61  m/vtuber-plan/la
+000002d0: 6e67 706f 7274 2f62 6c6f 622f 6d61 696e  ngport/blob/main
+000002e0: 2f4c 4943 454e 5345 223e 0a20 203c 696d  /LICENSE">.  <im
+000002f0: 6720 616c 743d 224c 6963 656e 7365 2220  g alt="License" 
+00000300: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00000310: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+00000320: 7562 2f6c 6963 656e 7365 2f76 7475 6265  ub/license/vtube
+00000330: 722d 706c 616e 2f6c 616e 6770 6f72 7422  r-plan/langport"
+00000340: 3e0a 3c2f 613e 0a0a 215b 6172 6368 6974  >.</a>..![archit
+00000350: 6563 7475 7265 5d28 6173 7365 7473 2f61  ecture](assets/a
+00000360: 7263 6869 7465 6374 7572 652e 6a70 6729  rchitecture.jpg)
+00000370: 0a0a 3c2f 6469 763e 0a0a 4c61 6e67 506f  ..</div>..LangPo
+00000380: 7274 2069 7320 6120 6f70 656e 2d73 6f75  rt is a open-sou
+00000390: 7263 6520 6c61 7267 6520 6c61 6e67 7561  rce large langua
+000003a0: 6765 206d 6f64 656c 2073 6572 7669 6e67  ge model serving
+000003b0: 2070 6c61 7466 6f72 6d2e 0a4f 7572 2067   platform..Our g
+000003c0: 6f61 6c20 6973 2074 6f20 6275 696c 6420  oal is to build 
+000003d0: 6120 7375 7065 7220 6661 7374 204c 4c4d  a super fast LLM
+000003e0: 2069 6e66 6572 656e 6365 2073 6572 7669   inference servi
+000003f0: 6365 2e0a 0a54 6869 7320 7072 6f6a 6563  ce...This projec
+00000400: 7420 6973 2069 6e73 7069 7265 6420 6279  t is inspired by
+00000410: 205b 6c6d 7379 732f 6661 7374 6368 6174   [lmsys/fastchat
+00000420: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000430: 2e63 6f6d 2f6c 6d2d 7379 732f 4661 7374  .com/lm-sys/Fast
+00000440: 4368 6174 292c 2077 6520 686f 7065 2074  Chat), we hope t
+00000450: 6861 7420 7468 6520 7365 7276 696e 6720  hat the serving 
+00000460: 706c 6174 666f 726d 2069 7320 6c69 6768  platform is ligh
+00000470: 7477 6569 6768 7420 616e 6420 6661 7374  tweight and fast
+00000480: 2c20 6275 7420 6661 7374 6368 6174 2069  , but fastchat i
+00000490: 6e63 6c75 6465 7320 6f74 6865 7220 6665  ncludes other fe
+000004a0: 6174 7572 6573 2073 7563 6820 6173 2074  atures such as t
+000004b0: 7261 696e 696e 6720 616e 6420 6576 616c  raining and eval
+000004c0: 7561 7469 6f6e 206d 616b 6520 6974 2063  uation make it c
+000004d0: 6f6d 706c 6963 6174 6564 2e0a 0a54 6865  omplicated...The
+000004e0: 2063 6f72 6520 6665 6174 7572 6573 2069   core features i
+000004f0: 6e63 6c75 6465 3a0a 2d20 4120 6469 7374  nclude:.- A dist
+00000500: 7269 6275 7465 6420 7365 7276 696e 6720  ributed serving 
+00000510: 7379 7374 656d 2066 6f72 2073 7461 7465  system for state
+00000520: 2d6f 662d 7468 652d 6172 7420 6d6f 6465  -of-the-art mode
+00000530: 6c73 2e0a 2d20 5374 7265 616d 696e 6720  ls..- Streaming 
+00000540: 6765 6e65 7261 7469 6f6e 2073 7570 706f  generation suppo
+00000550: 7274 2077 6974 6820 7661 7269 6f75 7320  rt with various 
+00000560: 6465 636f 6469 6e67 2073 7472 6174 6567  decoding strateg
+00000570: 6965 732e 0a2d 2042 6174 6368 2069 6e66  ies..- Batch inf
+00000580: 6572 656e 6365 2066 6f72 2068 6967 6865  erence for highe
+00000590: 7220 7468 726f 7567 6870 7574 2e0a 2d20  r throughput..- 
+000005a0: 5375 7070 6f72 7420 666f 7220 656e 636f  Support for enco
+000005b0: 6465 722d 6f6e 6c79 2c20 6465 636f 6465  der-only, decode
+000005c0: 722d 6f6e 6c79 2061 6e64 2065 6e63 6f64  r-only and encod
+000005d0: 6572 2d64 6563 6f64 6572 206d 6f64 656c  er-decoder model
+000005e0: 732e 0a2d 204f 7065 6e41 492d 636f 6d70  s..- OpenAI-comp
+000005f0: 6174 6962 6c65 2052 4553 5466 756c 2041  atible RESTful A
+00000600: 5049 732e 0a2d 2046 6175 7850 696c 6f74  PIs..- FauxPilot
+00000610: 2d63 6f6d 7061 7469 626c 6520 5245 5354  -compatible REST
+00000620: 6675 6c20 4150 4973 2e0a 2d20 4875 6767  ful APIs..- Hugg
+00000630: 696e 6746 6163 652d 636f 6d70 6174 6962  ingFace-compatib
+00000640: 6c65 2052 4553 5466 756c 2041 5049 732e  le RESTful APIs.
+00000650: 0a2d 2054 6162 6279 2d63 6f6d 7061 7469  .- Tabby-compati
+00000660: 626c 6520 5245 5354 6675 6c20 4150 4973  ble RESTful APIs
+00000670: 2e0a 0a23 2320 4265 6e63 686d 6172 6b0a  ...## Benchmark.
+00000680: 5765 2075 7365 2073 696e 676c 6520 5254  We use single RT
+00000690: 5833 3039 3020 746f 2072 756e 2061 2066  X3090 to run a f
+000006a0: 696e 6574 756e 6564 2037 4220 4c4c 614d  inetuned 7B LLaM
+000006b0: 4120 6d6f 6465 6c20 284f 7065 6e42 7564  A model (OpenBud
+000006c0: 6479 2056 302e 3929 2075 6e64 6572 2074  dy V0.9) under t
+000006d0: 6865 2062 6631 3620 7365 7474 696e 672e  he bf16 setting.
+000006e0: 0a57 6520 6372 6561 7465 2033 3220 7468  .We create 32 th
+000006f0: 7265 6164 7320 746f 2073 7562 6d69 7420  reads to submit 
+00000700: 6368 6174 2074 6173 6b73 2074 6f20 7468  chat tasks to th
+00000710: 6520 7365 7276 6572 2c20 616e 6420 7468  e server, and th
+00000720: 6520 666f 6c6c 6f77 696e 6720 6669 6775  e following figu
+00000730: 7265 2073 686f 7773 2074 6865 2051 7565  re shows the Que
+00000740: 7269 6573 2050 6572 2053 6563 6f6e 6420  ries Per Second 
+00000750: 2851 5053 2920 616e 6420 546f 6b65 6e73  (QPS) and Tokens
+00000760: 2050 6572 2053 6563 6f6e 6420 2854 5053   Per Second (TPS
+00000770: 2920 6f66 2046 6173 7443 6861 7420 616e  ) of FastChat an
+00000780: 6420 4c61 6e67 506f 7274 2077 6974 6820  d LangPort with 
+00000790: 6469 6666 6572 656e 7420 6d61 7820 6d6f  different max mo
+000007a0: 6465 6c20 636f 6e63 7572 7265 6e63 7920  del concurrency 
+000007b0: 7365 7474 696e 6773 2e0a 0a21 5b62 656e  settings...![ben
+000007c0: 6368 6d61 726b 5f63 6861 745d 2861 7373  chmark_chat](ass
+000007d0: 6574 732f 6265 6e63 686d 6172 6b5f 6368  ets/benchmark_ch
+000007e0: 6174 2e6a 7067 290a 0a0a 2323 204e 6577  at.jpg)...## New
+000007f0: 730a 2d20 5b32 3032 332f 3036 2f30 395d  s.- [2023/06/09]
+00000800: 2041 6464 204c 4c61 6d61 2e63 7070 2077   Add LLama.cpp w
+00000810: 6f72 6b65 7220 7375 7070 6f72 742e 0a2d  orker support..-
+00000820: 205b 3230 3233 2f30 362f 3031 5d20 4164   [2023/06/01] Ad
+00000830: 6420 4875 6767 696e 6746 6163 6520 4265  d HuggingFace Be
+00000840: 7274 2065 6d62 6564 6469 6e67 2077 6f72  rt embedding wor
+00000850: 6b65 7220 7375 7070 6f72 742e 0a2d 205b  ker support..- [
+00000860: 3230 3233 2f30 362f 3031 5d20 4164 6420  2023/06/01] Add 
+00000870: 4875 6767 696e 6746 6163 6520 7465 7874  HuggingFace text
+00000880: 2067 656e 6572 6174 696f 6e20 4150 4920   generation API 
+00000890: 7375 7070 6f72 742e 0a2d 205b 3230 3233  support..- [2023
+000008a0: 2f30 362f 3031 5d20 4164 6420 7461 6262  /06/01] Add tabb
+000008b0: 7920 4150 4920 7375 7070 6f72 742e 0a2d  y API support..-
+000008c0: 205b 3230 3233 2f30 352f 3233 5d20 4164   [2023/05/23] Ad
+000008d0: 6420 6368 6174 2074 6872 6f75 6768 7075  d chat throughpu
+000008e0: 7420 7465 7374 2073 6372 6970 742e 0a2d  t test script..-
+000008f0: 205b 3230 3233 2f30 352f 3232 5d20 4e65   [2023/05/22] Ne
+00000900: 7720 6469 7374 7269 6275 7465 6420 6172  w distributed ar
+00000910: 6368 6974 6563 7475 7265 2e0a 2d20 5b32  chitecture..- [2
+00000920: 3032 332f 3035 2f31 345d 2042 6174 6368  023/05/14] Batch
+00000930: 2069 6e66 6572 656e 6365 2073 7570 706f   inference suppo
+00000940: 7274 6564 2e0a 2d20 5b32 3032 332f 3035  rted..- [2023/05
+00000950: 2f31 305d 204c 616e 6770 6f72 7420 7072  /10] Langport pr
+00000960: 6f6a 6563 7420 7374 6172 7465 642e 0a0a  oject started...
+00000970: 0a23 2320 496e 7374 616c 6c0a 0a23 2323  .## Install..###
+00000980: 204d 6574 686f 6420 313a 2057 6974 6820   Method 1: With 
+00000990: 7069 700a 0a60 6060 6261 7368 0a70 6970  pip..```bash.pip
+000009a0: 3320 696e 7374 616c 6c20 6c61 6e67 706f  3 install langpo
+000009b0: 7274 0a60 6060 0a0a 6f72 3a0a 0a60 6060  rt.```..or:..```
+000009c0: 6261 7368 0a70 6970 3320 696e 7374 616c  bash.pip3 instal
+000009d0: 6c20 6769 742b 6874 7470 733a 2f2f 6769  l git+https://gi
+000009e0: 7468 7562 2e63 6f6d 2f76 7475 6265 722d  thub.com/vtuber-
+000009f0: 706c 616e 2f6c 616e 6770 6f72 742e 6769  plan/langport.gi
+00000a00: 7420 0a60 6060 0a0a 4966 2079 6f75 206e  t .```..If you n
+00000a10: 6565 6420 6c6c 616d 6163 7070 2067 656e  eed llamacpp gen
+00000a20: 6572 6174 696f 6e20 776f 726b 6572 2c20  eration worker, 
+00000a30: 7573 6520 7468 6973 2063 6f6d 6d61 6e64  use this command
+00000a40: 3a0a 6060 6062 6173 680a 7069 7033 2069  :.```bash.pip3 i
+00000a50: 6e73 7461 6c6c 206c 616e 6770 6f72 745b  nstall langport[
+00000a60: 6c6c 616d 6163 7070 5d0a 6060 600a 0a23  llamacpp].```..#
+00000a70: 2323 204d 6574 686f 6420 323a 2046 726f  ## Method 2: Fro
+00000a80: 6d20 736f 7572 6365 0a0a 312e 2043 6c6f  m source..1. Clo
+00000a90: 6e65 2074 6869 7320 7265 706f 7369 746f  ne this reposito
+00000aa0: 7279 0a60 6060 6261 7368 0a67 6974 2063  ry.```bash.git c
+00000ab0: 6c6f 6e65 2068 7474 7073 3a2f 2f67 6974  lone https://git
+00000ac0: 6875 622e 636f 6d2f 7674 7562 6572 2d70  hub.com/vtuber-p
+00000ad0: 6c61 6e2f 6c61 6e67 706f 7274 2e67 6974  lan/langport.git
+00000ae0: 0a63 6420 6c61 6e67 706f 7274 0a60 6060  .cd langport.```
+00000af0: 0a0a 322e 2049 6e73 7461 6c6c 2074 6865  ..2. Install the
+00000b00: 2050 6163 6b61 6765 0a60 6060 6261 7368   Package.```bash
+00000b10: 0a70 6970 2069 6e73 7461 6c6c 202d 2d75  .pip install --u
+00000b20: 7067 7261 6465 2070 6970 0a70 6970 2069  pgrade pip.pip i
+00000b30: 6e73 7461 6c6c 202d 6520 2e0a 6060 600a  nstall -e ..```.
+00000b40: 0a23 2320 5374 6172 7420 7468 6520 7365  .## Start the se
+00000b50: 7276 6572 0a0a 4974 2069 7320 7369 6d70  rver..It is simp
+00000b60: 6c65 2074 6f20 7374 6172 7420 6120 7369  le to start a si
+00000b70: 6e67 6c65 206e 6f64 6520 6368 6174 2041  ngle node chat A
+00000b80: 5049 2073 6572 7669 6365 3a0a 6060 6020  PI service:.``` 
+00000b90: 6261 7368 0a70 7974 686f 6e20 2d6d 206c  bash.python -m l
+00000ba0: 616e 6770 6f72 742e 7365 7276 6963 652e  angport.service.
+00000bb0: 7365 7276 6572 2e67 656e 6572 6174 696f  server.generatio
+00000bc0: 6e5f 776f 726b 6572 202d 2d70 6f72 7420  n_worker --port 
+00000bd0: 3231 3030 3120 2d2d 6d6f 6465 6c2d 7061  21001 --model-pa
+00000be0: 7468 203c 796f 7572 206d 6f64 656c 2070  th <your model p
+00000bf0: 6174 683e 0a70 7974 686f 6e20 2d6d 206c  ath>.python -m l
+00000c00: 616e 6770 6f72 742e 7365 7276 6963 652e  angport.service.
+00000c10: 6761 7465 7761 792e 6f70 656e 6169 5f61  gateway.openai_a
+00000c20: 7069 0a60 6060 0a0a 4966 2079 6f75 206e  pi.```..If you n
+00000c30: 6565 6420 7468 6520 656d 6265 6464 696e  eed the embeddin
+00000c40: 6773 2041 5049 206f 7220 6f74 6865 7220  gs API or other 
+00000c50: 6665 6174 7572 6573 2c20 796f 7520 6361  features, you ca
+00000c60: 6e20 6465 706c 6f79 2061 2064 6973 7472  n deploy a distr
+00000c70: 6962 7574 6564 2069 6e66 6572 656e 6365  ibuted inference
+00000c80: 2063 6c75 7374 6572 3a0a 6060 6020 6261   cluster:.``` ba
+00000c90: 7368 0a70 7974 686f 6e20 2d6d 206c 616e  sh.python -m lan
+00000ca0: 6770 6f72 742e 7365 7276 6963 652e 7365  gport.service.se
+00000cb0: 7276 6572 2e64 756d 6d79 5f77 6f72 6b65  rver.dummy_worke
+00000cc0: 7220 2d2d 706f 7274 2032 3130 3031 0a70  r --port 21001.p
+00000cd0: 7974 686f 6e20 2d6d 206c 616e 6770 6f72  ython -m langpor
+00000ce0: 742e 7365 7276 6963 652e 7365 7276 6572  t.service.server
+00000cf0: 2e67 656e 6572 6174 696f 6e5f 776f 726b  .generation_work
+00000d00: 6572 202d 2d6d 6f64 656c 2d70 6174 6820  er --model-path 
+00000d10: 3c79 6f75 7220 6d6f 6465 6c20 7061 7468  <your model path
+00000d20: 3e20 2d2d 6e65 6967 6862 6f72 7320 6874  > --neighbors ht
+00000d30: 7470 3a2f 2f6c 6f63 616c 686f 7374 3a32  tp://localhost:2
+00000d40: 3130 3031 0a70 7974 686f 6e20 2d6d 206c  1001.python -m l
+00000d50: 616e 6770 6f72 742e 7365 7276 6963 652e  angport.service.
+00000d60: 7365 7276 6572 2e65 6d62 6564 6469 6e67  server.embedding
+00000d70: 5f77 6f72 6b65 7220 2d2d 6d6f 6465 6c2d  _worker --model-
+00000d80: 7061 7468 203c 796f 7572 206d 6f64 656c  path <your model
+00000d90: 2070 6174 683e 202d 2d6e 6569 6768 626f   path> --neighbo
+00000da0: 7273 2068 7474 703a 2f2f 6c6f 6361 6c68  rs http://localh
+00000db0: 6f73 743a 3231 3030 310a 7079 7468 6f6e  ost:21001.python
+00000dc0: 202d 6d20 6c61 6e67 706f 7274 2e73 6572   -m langport.ser
+00000dd0: 7669 6365 2e67 6174 6577 6179 2e6f 7065  vice.gateway.ope
+00000de0: 6e61 695f 6170 6920 2d2d 636f 6e74 726f  nai_api --contro
+00000df0: 6c6c 6572 2d61 6464 7265 7373 2068 7474  ller-address htt
+00000e00: 703a 2f2f 6c6f 6361 6c68 6f73 743a 3231  p://localhost:21
+00000e10: 3030 310a 6060 600a 0a49 6e20 7072 6163  001.```..In prac
+00000e20: 7469 6365 2c20 7468 6520 6761 7465 7761  tice, the gatewa
+00000e30: 7920 6361 6e20 636f 6e6e 6563 7420 746f  y can connect to
+00000e40: 2061 6e79 206e 6f64 6520 746f 2064 6973   any node to dis
+00000e50: 7472 6962 7574 6520 696e 6665 7265 6e63  tribute inferenc
+00000e60: 6520 7461 736b 733a 0a0a 6060 6020 6261  e tasks:..``` ba
+00000e70: 7368 0a70 7974 686f 6e20 2d6d 206c 616e  sh.python -m lan
+00000e80: 6770 6f72 742e 7365 7276 6963 652e 7365  gport.service.se
+00000e90: 7276 6572 2e64 756d 6d79 5f77 6f72 6b65  rver.dummy_worke
+00000ea0: 7220 2d2d 706f 7274 2032 3130 3031 0a70  r --port 21001.p
+00000eb0: 7974 686f 6e20 2d6d 206c 616e 6770 6f72  ython -m langpor
+00000ec0: 742e 7365 7276 6963 652e 7365 7276 6572  t.service.server
+00000ed0: 2e67 656e 6572 6174 696f 6e5f 776f 726b  .generation_work
+00000ee0: 6572 202d 2d70 6f72 7420 3231 3030 3220  er --port 21002 
+00000ef0: 2d2d 6d6f 6465 6c2d 7061 7468 203c 796f  --model-path <yo
+00000f00: 7572 206d 6f64 656c 2070 6174 683e 202d  ur model path> -
+00000f10: 2d6e 6569 6768 626f 7273 2068 7474 703a  -neighbors http:
+00000f20: 2f2f 6c6f 6361 6c68 6f73 743a 3231 3030  //localhost:2100
+00000f30: 310a 7079 7468 6f6e 202d 6d20 6c61 6e67  1.python -m lang
+00000f40: 706f 7274 2e73 6572 7669 6365 2e73 6572  port.service.ser
+00000f50: 7665 722e 6765 6e65 7261 7469 6f6e 5f77  ver.generation_w
+00000f60: 6f72 6b65 7220 2d2d 706f 7274 2032 3130  orker --port 210
+00000f70: 3033 202d 2d6d 6f64 656c 2d70 6174 6820  03 --model-path 
+00000f80: 3c79 6f75 7220 6d6f 6465 6c20 7061 7468  <your model path
+00000f90: 3e20 2d2d 6e65 6967 6862 6f72 7320 6874  > --neighbors ht
+00000fa0: 7470 3a2f 2f6c 6f63 616c 686f 7374 3a32  tp://localhost:2
+00000fb0: 3130 3031 2068 7474 703a 2f2f 6c6f 6361  1001 http://loca
+00000fc0: 6c68 6f73 743a 3231 3030 320a 7079 7468  lhost:21002.pyth
+00000fd0: 6f6e 202d 6d20 6c61 6e67 706f 7274 2e73  on -m langport.s
+00000fe0: 6572 7669 6365 2e73 6572 7665 722e 6765  ervice.server.ge
+00000ff0: 6e65 7261 7469 6f6e 5f77 6f72 6b65 7220  neration_worker 
+00001000: 2d2d 706f 7274 2032 3130 3034 202d 2d6d  --port 21004 --m
+00001010: 6f64 656c 2d70 6174 6820 3c79 6f75 7220  odel-path <your 
+00001020: 6d6f 6465 6c20 7061 7468 3e20 2d2d 6e65  model path> --ne
+00001030: 6967 6862 6f72 7320 6874 7470 3a2f 2f6c  ighbors http://l
+00001040: 6f63 616c 686f 7374 3a32 3130 3031 2068  ocalhost:21001 h
+00001050: 7474 703a 2f2f 6c6f 6361 6c68 6f73 743a  ttp://localhost:
+00001060: 3231 3030 330a 7079 7468 6f6e 202d 6d20  21003.python -m 
+00001070: 6c61 6e67 706f 7274 2e73 6572 7669 6365  langport.service
+00001080: 2e73 6572 7665 722e 6765 6e65 7261 7469  .server.generati
+00001090: 6f6e 5f77 6f72 6b65 7220 2d2d 706f 7274  on_worker --port
+000010a0: 2032 3130 3035 202d 2d6d 6f64 656c 2d70   21005 --model-p
+000010b0: 6174 6820 3c79 6f75 7220 6d6f 6465 6c20  ath <your model 
+000010c0: 7061 7468 3e20 2d2d 6e65 6967 6862 6f72  path> --neighbor
+000010d0: 7320 6874 7470 3a2f 2f6c 6f63 616c 686f  s http://localho
+000010e0: 7374 3a32 3130 3031 2068 7474 703a 2f2f  st:21001 http://
+000010f0: 6c6f 6361 6c68 6f73 743a 3231 3030 340a  localhost:21004.
+00001100: 7079 7468 6f6e 202d 6d20 6c61 6e67 706f  python -m langpo
+00001110: 7274 2e73 6572 7669 6365 2e67 6174 6577  rt.service.gatew
+00001120: 6179 2e6f 7065 6e61 695f 6170 6920 2d2d  ay.openai_api --
+00001130: 636f 6e74 726f 6c6c 6572 2d61 6464 7265  controller-addre
+00001140: 7373 2068 7474 703a 2f2f 6c6f 6361 6c68  ss http://localh
+00001150: 6f73 743a 3231 3030 3320 2320 3231 3030  ost:21003 # 2100
+00001160: 3320 6973 204f 4b21 0a70 7974 686f 6e20  3 is OK!.python 
+00001170: 2d6d 206c 616e 6770 6f72 742e 7365 7276  -m langport.serv
+00001180: 6963 652e 6761 7465 7761 792e 6f70 656e  ice.gateway.open
+00001190: 6169 5f61 7069 202d 2d63 6f6e 7472 6f6c  ai_api --control
+000011a0: 6c65 722d 6164 6472 6573 7320 6874 7470  ler-address http
+000011b0: 3a2f 2f6c 6f63 616c 686f 7374 3a32 3130  ://localhost:210
+000011c0: 3032 2023 2041 6e79 2077 6f72 6b65 7220  02 # Any worker 
+000011d0: 6973 2061 6c73 6f20 4f4b 210a 6060 600a  is also OK!.```.
+000011e0: 0a52 756e 2074 6578 7420 6765 6e65 7261  .Run text genera
+000011f0: 7469 6f6e 2077 6974 6820 6d75 6c74 6920  tion with multi 
+00001200: 4750 5573 3a0a 0a60 6060 2062 6173 680a  GPUs:..``` bash.
+00001210: 7079 7468 6f6e 202d 6d20 6c61 6e67 706f  python -m langpo
+00001220: 7274 2e73 6572 7669 6365 2e73 6572 7665  rt.service.serve
+00001230: 722e 6765 6e65 7261 7469 6f6e 5f77 6f72  r.generation_wor
+00001240: 6b65 7220 2d2d 706f 7274 2032 3130 3031  ker --port 21001
+00001250: 202d 2d6d 6f64 656c 2d70 6174 6820 3c79   --model-path <y
+00001260: 6f75 7220 6d6f 6465 6c20 7061 7468 3e20  our model path> 
+00001270: 2d2d 6770 7573 2030 2c31 202d 2d6e 756d  --gpus 0,1 --num
+00001280: 2d67 7075 7320 320a 7079 7468 6f6e 202d  -gpus 2.python -
+00001290: 6d20 6c61 6e67 706f 7274 2e73 6572 7669  m langport.servi
+000012a0: 6365 2e67 6174 6577 6179 2e6f 7065 6e61  ce.gateway.opena
+000012b0: 695f 6170 690a 6060 600a 0a52 756e 2074  i_api.```..Run t
+000012c0: 6578 7420 6765 6e65 7261 7469 6f6e 2077  ext generation w
+000012d0: 6974 6820 4c4c 616d 612e 6370 7020 776f  ith LLama.cpp wo
+000012e0: 726b 6572 3a0a 0a60 6060 6261 7368 0a70  rker:..```bash.p
+000012f0: 7974 686f 6e20 2d6d 206c 616e 6770 6f72  ython -m langpor
+00001300: 742e 7365 7276 6963 652e 7365 7276 6572  t.service.server
+00001310: 2e67 656e 6572 6174 696f 6e5f 776f 726b  .generation_work
+00001320: 6572 202d 2d70 6f72 7420 3231 3030 3120  er --port 21001 
+00001330: 2d2d 6d6f 6465 6c2d 7061 7468 203c 796f  --model-path <yo
+00001340: 7572 206d 6f64 656c 2070 6174 683e 202d  ur model path> -
+00001350: 2d6e 2d67 7075 2d6c 6179 6572 7320 3c6e  -n-gpu-layers <n
+00001360: 756d 206c 6179 6572 2074 6f20 6770 7520  um layer to gpu 
+00001370: 2872 6573 697a 6520 7468 6973 2066 6f72  (resize this for
+00001380: 2079 6f75 7220 5652 414d 293e 0a60 6060   your VRAM)>.```
+00001390: 0a0a 2323 204c 6963 656e 7365 0a0a 6c61  ..## License..la
+000013a0: 6e67 706f 7274 2069 7320 7265 6c65 6173  ngport is releas
+000013b0: 6564 2075 6e64 6572 2074 6865 2041 7061  ed under the Apa
+000013c0: 6368 6520 536f 6674 7761 7265 204c 6963  che Software Lic
+000013d0: 656e 7365 2e0a 0a0a 2323 2053 6565 2061  ense....## See a
+000013e0: 6c73 6f0a 0a2d 205b 6c61 6e67 706f 7274  lso..- [langport
+000013f0: 2d64 6f63 735d 2868 7474 7073 3a2f 2f67  -docs](https://g
+00001400: 6974 6875 622e 636f 6d2f 7674 7562 6572  ithub.com/vtuber
+00001410: 2d70 6c61 6e2f 6c61 6e67 706f 7274 2f74  -plan/langport/t
+00001420: 7265 652f 6d61 696e 2f64 6f63 7329 0a2d  ree/main/docs).-
+00001430: 205b 6c61 6e67 706f 7274 2d73 6f75 7263   [langport-sourc
+00001440: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+00001450: 622e 636f 6d2f 7674 7562 6572 2d70 6c61  b.com/vtuber-pla
+00001460: 6e2f 6c61 6e67 706f 7274 290a 0a0a 2323  n/langport)...##
+00001470: 2053 7461 7220 4869 7374 6f72 790a 0a5b   Star History..[
+00001480: 215b 5374 6172 2048 6973 746f 7279 2043  ![Star History C
+00001490: 6861 7274 5d28 6874 7470 733a 2f2f 6170  hart](https://ap
+000014a0: 692e 7374 6172 2d68 6973 746f 7279 2e63  i.star-history.c
+000014b0: 6f6d 2f73 7667 3f72 6570 6f73 3d76 7475  om/svg?repos=vtu
+000014c0: 6265 722d 706c 616e 2f6c 616e 6770 6f72  ber-plan/langpor
+000014d0: 7426 7479 7065 3d44 6174 6529 5d28 6874  t&type=Date)](ht
+000014e0: 7470 733a 2f2f 7374 6172 2d68 6973 746f  tps://star-histo
+000014f0: 7279 2e63 6f6d 2f23 7674 7562 6572 2d70  ry.com/#vtuber-p
+00001500: 6c61 6e2f 6c61 6e67 706f 7274 2644 6174  lan/langport&Dat
+00001510: 6529 0a0a                                e)..
```

### Comparing `langport-0.0.4/langport.egg-info/SOURCES.txt` & `langport-0.1.0/langport.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -20,16 +20,19 @@
 langport/data/conversation/settings/__init__.py
 langport/data/conversation/settings/baize.py
 langport/data/conversation/settings/bard.py
 langport/data/conversation/settings/billa.py
 langport/data/conversation/settings/chatgpt.py
 langport/data/conversation/settings/claude.py
 langport/data/conversation/settings/dolly.py
+langport/data/conversation/settings/falcon.py
 langport/data/conversation/settings/h2ogpt.py
 langport/data/conversation/settings/koala.py
+langport/data/conversation/settings/llama_cpp.py
+langport/data/conversation/settings/mpt.py
 langport/data/conversation/settings/oasst_pythia.py
 langport/data/conversation/settings/one_shot.py
 langport/data/conversation/settings/openbuddy.py
 langport/data/conversation/settings/phoenix.py
 langport/data/conversation/settings/redpajama.py
 langport/data/conversation/settings/rwkv.py
 langport/data/conversation/settings/stablelm.py
@@ -43,52 +46,68 @@
 langport/model/adapters/__init__.py
 langport/model/adapters/baize.py
 langport/model/adapters/bard.py
 langport/model/adapters/billa.py
 langport/model/adapters/chatglm.py
 langport/model/adapters/chatgpt.py
 langport/model/adapters/claude.py
+langport/model/adapters/codegen.py
 langport/model/adapters/dolly_v2.py
+langport/model/adapters/falcon.py
 langport/model/adapters/koala.py
+langport/model/adapters/llama_cpp.py
 langport/model/adapters/oasst_pythia.py
 langport/model/adapters/openbuddy.py
 langport/model/adapters/phoenix.py
 langport/model/adapters/rwkv.py
 langport/model/adapters/stable_lm.py
+langport/model/adapters/starcoder.py
 langport/model/adapters/t5.py
+langport/model/adapters/text2vec.py
 langport/model/adapters/vicuna.py
 langport/model/executor/__init__.py
 langport/model/executor/base.py
-langport/model/executor/huggingface_utils.py
+langport/model/executor/huggingface.py
+langport/model/executor/llamacpp.py
 langport/model/executor/embedding/__init__.py
 langport/model/executor/embedding/huggingface.py
 langport/model/executor/generation/__init__.py
 langport/model/executor/generation/chatgpt.py
 langport/model/executor/generation/huggingface.py
+langport/model/executor/generation/llamacpp.py
 langport/model/models/__init__.py
 langport/model/models/rwkv_model.py
 langport/protocol/__init__.py
-langport/protocol/fauxpilot_api_protocol.py
+langport/protocol/huggingface_api_protocol.py
 langport/protocol/openai_api_protocol.py
+langport/protocol/tabby_api_protocol.py
 langport/protocol/worker_protocol.py
 langport/routers/__init__.py
 langport/routers/gateway/__init__.py
+langport/routers/gateway/common.py
+langport/routers/gateway/openai_compatible.py
 langport/routers/server/__init__.py
 langport/routers/server/core_node.py
 langport/routers/server/embedding_node.py
 langport/routers/server/generation_node.py
 langport/service/__init__.py
 langport/service/gateway/__init__.py
+langport/service/gateway/cluster_monitor.py
+langport/service/gateway/cluster_monitor_app.py
 langport/service/gateway/fauxpilot_api.py
+langport/service/gateway/graphite_feeder.py
+langport/service/gateway/huggingface_api.py
 langport/service/gateway/openai_api.py
+langport/service/gateway/tabby_api.py
 langport/service/server/__init__.py
 langport/service/server/chatgpt_generation_worker.py
 langport/service/server/dummy_worker.py
 langport/service/server/embedding_worker.py
 langport/service/server/generation_worker.py
+langport/service/server/ggml_generation_worker.py
 langport/utils/__init__.py
 langport/utils/cache_state.py
 langport/utils/evaluation.py
 langport/utils/http_pool.py
 langport/utils/interval_timer.py
 langport/workers/__init__.py
 langport/workers/embedding_worker.py
```

### Comparing `langport-0.0.4/pyproject.toml` & `langport-0.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "langport"
-version = "0.0.4"
+version = "0.1.0"
 description = "A large language model serving platform."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
@@ -17,14 +17,15 @@
     "rich>=10.0.0", "sentencepiece",
     "shortuuid", "shortuuid", "tokenizers>=0.12.1", "torch",
     "transformers>=4.28.0,<4.29.0", "uvicorn", "wandb", "tenacity>=8.2.2",
 ]
 
 [project.optional-dependencies]
 dev = ["black==23.3.0", "pylint==2.8.2"]
+llamacpp = ["llama-cpp-python"]
 
 [project.urls]
 "Homepage" = "https://github.com/vtuber-plan/langport"
 "Bug Tracker" = "https://github.com/vtuber-plan/langport/issues"
 
 [tool.setuptools.packages.find]
 exclude = ["assets*", "benchmark*", "docs", "dist*", "playground*", "scripts*", "tests*"]
```

