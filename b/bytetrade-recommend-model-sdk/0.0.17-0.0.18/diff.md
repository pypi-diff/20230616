# Comparing `tmp/bytetrade-recommend-model-sdk-0.0.17.tar.gz` & `tmp/bytetrade-recommend-model-sdk-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.17.tar", last modified: Tue May 30 08:54:47 2023, max compression
+gzip compressed data, was "bytetrade-recommend-model-sdk-0.0.18.tar", last modified: Fri Jun 16 07:59:02 2023, max compression
```

## Comparing `bytetrade-recommend-model-sdk-0.0.17.tar` & `bytetrade-recommend-model-sdk-0.0.18.tar`

### file list

```diff
@@ -1,35 +1,54 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 08:54:47.771402 bytetrade-recommend-model-sdk-0.0.17/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-05-30 08:54:47.767402 bytetrade-recommend-model-sdk-0.0.17/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 08:54:47.767402 bytetrade-recommend-model-sdk-0.0.17/bytetrade_recommend_model_sdk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-05-30 08:54:47.000000 bytetrade-recommend-model-sdk-0.0.17/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1032 2023-05-30 08:54:47.000000 bytetrade-recommend-model-sdk-0.0.17/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-30 08:54:47.000000 bytetrade-recommend-model-sdk-0.0.17/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2023-05-30 08:54:47.000000 bytetrade-recommend-model-sdk-0.0.17/bytetrade_recommend_model_sdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-05-30 08:54:47.000000 bytetrade-recommend-model-sdk-0.0.17/bytetrade_recommend_model_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 08:54:47.767402 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 08:54:47.767402 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/embeddings/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/embeddings/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      495 2023-05-30 08:37:42.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/embeddings/bert_embedding.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/embeddings/embedding_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5430 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/embeddings/word2vec_embedding.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 08:54:47.767402 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/proto_class/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/proto_class/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2661 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/proto_class/embedding_pb2.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 08:54:47.767402 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/rank/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/rank/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/rank/faiss_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9322 2023-05-29 08:12:34.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/rank/rank_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/rank/time_weight_decay_tool.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 08:54:47.767402 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/resources/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1800 2023-05-30 08:47:17.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/resources/model_management.json
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-30 08:54:47.767402 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/tools/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/tools/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3456 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/tools/aws_s3_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3652 2023-05-25 22:22:09.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/tools/common_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27487 2023-05-30 08:43:31.000000 bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/tools/model_tool.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-30 08:54:47.771402 bytetrade-recommend-model-sdk-0.0.17/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      978 2023-05-30 08:52:43.000000 bytetrade-recommend-model-sdk-0.0.17/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 07:59:02.219612 bytetrade-recommend-model-sdk-0.0.18/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.18/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-06-16 07:59:02.219612 bytetrade-recommend-model-sdk-0.0.18/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.18/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 07:59:02.215612 bytetrade-recommend-model-sdk-0.0.18/bytetrade_recommend_model_sdk.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-06-16 07:59:02.000000 bytetrade-recommend-model-sdk-0.0.18/bytetrade_recommend_model_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1808 2023-06-16 07:59:02.000000 bytetrade-recommend-model-sdk-0.0.18/bytetrade_recommend_model_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-16 07:59:02.000000 bytetrade-recommend-model-sdk-0.0.18/bytetrade_recommend_model_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       63 2023-06-16 07:59:02.000000 bytetrade-recommend-model-sdk-0.0.18/bytetrade_recommend_model_sdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       20 2023-06-16 07:59:02.000000 bytetrade-recommend-model-sdk-0.0.18/bytetrade_recommend_model_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 07:59:02.215612 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 07:59:02.215612 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/embeddings/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/embeddings/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      495 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/embeddings/bert_embedding.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      872 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/embeddings/embedding_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5430 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/embeddings/word2vec_embedding.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 07:59:02.215612 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/mind_sdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-02 06:43:29.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/mind_sdk/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 07:59:02.215612 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/mind_sdk/config/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 22:12:28.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/mind_sdk/config/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      675 2023-06-16 07:42:45.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/mind_sdk/config/content_similar_config.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      141 2023-06-10 21:00:03.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/mind_sdk/config/mind_base_config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 07:59:02.219612 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/mind_sdk/dataset/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 21:32:28.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/mind_sdk/dataset/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1529 2023-06-10 21:40:00.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/mind_sdk/dataset/mind_behaviours_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2180 2023-06-12 05:18:24.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/mind_sdk/dataset/mind_news_dataset.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2873 2023-06-09 01:37:52.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/mind_sdk/dataset/mind_user_dataset.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 07:59:02.219612 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/mind_sdk/eval/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 22:36:32.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/mind_sdk/eval/__init_.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1113 2023-06-07 22:40:09.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/mind_sdk/eval/eval_operation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11614 2023-06-13 09:09:31.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/mind_sdk/eval/mind_eval_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-06-07 07:14:04.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/mind_sdk/experiment_enum.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 07:59:02.219612 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/mind_sdk/model/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-07 22:01:07.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/mind_sdk/model/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9414 2023-06-16 07:32:06.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/mind_sdk/model/content_similar_model.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 07:59:02.219612 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/proto_class/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/proto_class/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2661 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/proto_class/embedding_pb2.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 07:59:02.219612 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/recommend/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/recommend/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3354 2023-06-16 05:57:06.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/recommend/recommend_common_util.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1774 2023-06-16 07:52:03.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/recommend/recommend_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2150 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/recommend/time_weight_decay_tool.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 07:59:02.219612 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/resources/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1835 2023-06-16 07:54:02.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/resources/model_management.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 07:59:02.219612 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/tools/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/tools/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5147 2023-06-06 23:52:17.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/tools/aws_s3_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10416 2023-06-12 05:13:22.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/tools/common_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    27487 2023-05-31 06:38:05.000000 bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/tools/model_tool.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-16 07:59:02.219612 bytetrade-recommend-model-sdk-0.0.18/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      978 2023-06-16 07:58:36.000000 bytetrade-recommend-model-sdk-0.0.18/setup.py
```

### Comparing `bytetrade-recommend-model-sdk-0.0.17/README.md` & `bytetrade-recommend-model-sdk-0.0.18/README.md`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/embeddings/embedding_tool.py` & `bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/embeddings/embedding_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/embeddings/word2vec_embedding.py` & `bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/embeddings/word2vec_embedding.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/proto_class/embedding_pb2.py` & `bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/proto_class/embedding_pb2.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/rank/time_weight_decay_tool.py` & `bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/recommend/time_weight_decay_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/resources/model_management.json` & `bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/resources/model_management.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9754464285714286%*

 * *Differences: {"'bert'": "{'v1': {'embedding_dim': 768}}",*

 * * "'word2vec_google'": "{'v1': {'active': False}, 'v2': {'active': False}}"}*

```diff
@@ -1,22 +1,23 @@
 {
     "bert": {
         "v1": {
             "active": true,
+            "embedding_dim": 768,
             "model_related_files": [],
             "model_related_files_public": {},
             "model_related_files_suffix": {},
             "mongodb_embedding_field": "bert_v1",
             "pg_embedding_mark_field": "bert_v1",
             "s3_bucket": "gpu-model-data"
         }
     },
     "word2vec_google": {
         "v1": {
-            "active": true,
+            "active": false,
             "model_related_files": [
                 "GoogleNews-vectors-negative300.bin",
                 "tfidf.model",
                 "dictionary"
             ],
             "model_related_files_public": {
                 "GoogleNews-vectors-negative300.bin": true,
@@ -29,15 +30,15 @@
                 "tfidf.model": "gz"
             },
             "mongodb_embedding_field": "word2vec_google_v1",
             "pg_embedding_mark_field": "word2vec_google_embedding",
             "s3_bucket": "gpu-model-data"
         },
         "v2": {
-            "active": true,
+            "active": false,
             "model_related_files": [
                 "GoogleNews-vectors-negative300.bin",
                 "tfidf.model",
                 "dictionary"
             ],
             "model_related_files_public": {
                 "GoogleNews-vectors-negative300.bin": true,
```

### Comparing `bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/tools/aws_s3_tool.py` & `bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/tools/aws_s3_tool.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import boto3
+import json
 import sys 
 
 from recommend_model_sdk.tools.common_tool import CommonTool
 
 class AWSS3Tool:
     def __init__(self) -> None:
         self.__client = boto3.client('s3')
@@ -84,17 +85,55 @@
             
         else:
             current_byte = response["Body"].read()
             result["success"] = True
             result["response"] = response
             result["bytes"] = current_byte
         return result
-            
-            
-            
-        
-
-    
+              
     def get_object_header(self,s3_bucket, s3_object_key):
         meta_data = self.__client.head_object(Bucket=s3_bucket, Key=s3_object_key)
         return meta_data
-    
+    
+    def get_object_dict(self,bucket_name,key):
+        if isinstance(bucket_name,str) is False:
+            raise ValueError("bucket name is not str")
+        if isinstance(key,str) is False:
+            raise ValueError("key is not str")
+        response = self.__client.get_object(
+            Bucket=bucket_name,
+            Key=key,
+        )
+        result=dict()
+        if ("ResponseMetadata" not in response or 
+            "HTTPStatusCode" not in response["ResponseMetadata"] or
+            response["ResponseMetadata"]["HTTPStatusCode"] != 200):
+            self.__logger.error(f"get bucket {bucket_name} key {key} fail, response {response}")
+            result["success"] = False
+            result["response"] = response
+            
+        else:
+            current_byte = response["Body"].read()
+            result["success"] = True
+            result["response"] = response
+            result["dict"] = json.loads(current_byte)
+        return result
+
+
+    def put_oject_dict(self,bucket_name,key,meta_data_dict,data_dict):
+        if isinstance(bucket_name,str) is False:
+            raise ValueError("bucket name is not str")
+        if isinstance(key,str) is False:
+            raise ValueError("key is not str")
+        if isinstance(meta_data_dict,dict) is False:
+            raise ValueError("meta_data_dict is not dict")
+        if isinstance(data_dict,dict) is False:
+            raise ValueError("data_dict is not dict")
+        
+        response = self.__client.put_object(
+            Body=json.dumps(data_dict).encode("utf-8"),
+            Bucket=bucket_name,
+            Key=key,
+            # ContentType=content_type,
+            Metadata=meta_data_dict
+        )
+        return response
```

### Comparing `bytetrade-recommend-model-sdk-0.0.17/recommend_model_sdk/tools/model_tool.py` & `bytetrade-recommend-model-sdk-0.0.18/recommend_model_sdk/tools/model_tool.py`

 * *Files identical despite different names*

### Comparing `bytetrade-recommend-model-sdk-0.0.17/setup.py` & `bytetrade-recommend-model-sdk-0.0.18/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 sys.path.append(os.path.dirname(__file__) + "/recommend-model")
 
 
 
 
 setup(
     name="bytetrade-recommend-model-sdk",
-    version="0.0.17",
+    version="0.0.18",
     # packages=find_packages(exclude="unit_test"),
     install_requires=[
         "pandas==2.0.0",
         "gensim==4.3.1",
         "protobuf==4.21.8",
         "nltk==3.8.1",
         "boto3"
```

