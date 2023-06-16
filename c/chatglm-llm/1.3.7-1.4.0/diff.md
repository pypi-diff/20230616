# Comparing `tmp/chatglm-llm-1.3.7.tar.gz` & `tmp/chatglm-llm-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatglm-llm-1.3.7.tar", last modified: Thu Jun 15 08:48:43 2023, max compression
+gzip compressed data, was "chatglm-llm-1.4.0.tar", last modified: Fri Jun 16 02:42:45 2023, max compression
```

## Comparing `chatglm-llm-1.3.7.tar` & `chatglm-llm-1.4.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-15 08:48:43.362502 chatglm-llm-1.3.7/
--rw-r--r--   0 mroy       (501) staff       (20)       36 2023-05-10 01:48:15.000000 chatglm-llm-1.3.7/MANIFEST.in
--rw-r--r--   0 mroy       (501) staff       (20)      212 2023-06-15 08:48:43.362354 chatglm-llm-1.3.7/PKG-INFO
--rw-r--r--   0 mroy       (501) staff       (20)     1887 2023-05-04 01:08:28.000000 chatglm-llm-1.3.7/README.md
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-15 08:48:43.360073 chatglm-llm-1.3.7/chatglm_llm.egg-info/
--rw-r--r--   0 mroy       (501) staff       (20)      212 2023-06-15 08:48:43.000000 chatglm-llm-1.3.7/chatglm_llm.egg-info/PKG-INFO
--rw-r--r--   0 mroy       (501) staff       (20)      480 2023-06-15 08:48:43.000000 chatglm-llm-1.3.7/chatglm_llm.egg-info/SOURCES.txt
--rw-r--r--   0 mroy       (501) staff       (20)        1 2023-06-15 08:48:43.000000 chatglm-llm-1.3.7/chatglm_llm.egg-info/dependency_links.txt
--rw-r--r--   0 mroy       (501) staff       (20)       53 2023-06-15 08:48:43.000000 chatglm-llm-1.3.7/chatglm_llm.egg-info/entry_points.txt
--rw-r--r--   0 mroy       (501) staff       (20)        1 2023-05-04 01:12:10.000000 chatglm-llm-1.3.7/chatglm_llm.egg-info/not-zip-safe
--rw-r--r--   0 mroy       (501) staff       (20)      240 2023-06-15 08:48:43.000000 chatglm-llm-1.3.7/chatglm_llm.egg-info/requires.txt
--rw-r--r--   0 mroy       (501) staff       (20)       12 2023-06-15 08:48:43.000000 chatglm-llm-1.3.7/chatglm_llm.egg-info/top_level.txt
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-15 08:48:43.361312 chatglm-llm-1.3.7/chatglm_src/
--rw-r--r--   0 mroy       (501) staff       (20)      690 2023-05-30 04:21:32.000000 chatglm-llm-1.3.7/chatglm_src/__init__.py
--rw-r--r--   0 mroy       (501) staff       (20)     4201 2023-05-13 02:36:58.000000 chatglm-llm-1.3.7/chatglm_src/callbacks.py
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-15 08:48:43.361765 chatglm-llm-1.3.7/chatglm_src/chains/
--rw-r--r--   0 mroy       (501) staff       (20)       69 2023-05-10 01:48:15.000000 chatglm-llm-1.3.7/chatglm_src/chains/__init__.py
--rw-r--r--   0 mroy       (501) staff       (20)     4402 2023-05-11 09:17:21.000000 chatglm-llm-1.3.7/chatglm_src/chains/local_qa.py
--rw-r--r--   0 mroy       (501) staff       (20)      537 2023-05-30 04:20:56.000000 chatglm-llm-1.3.7/chatglm_src/cmd.py
--rw-r--r--   0 mroy       (501) staff       (20)     3052 2023-06-15 08:48:00.000000 chatglm-llm-1.3.7/chatglm_src/embeding.py
--rw-r--r--   0 mroy       (501) staff       (20)    36155 2023-06-01 08:59:10.000000 chatglm-llm-1.3.7/chatglm_src/llm.py
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-15 08:48:43.362148 chatglm-llm-1.3.7/chatglm_src/loader/
--rw-r--r--   0 mroy       (501) staff       (20)     1403 2023-05-11 01:28:05.000000 chatglm-llm-1.3.7/chatglm_src/loader/__init__.py
--rw-r--r--   0 mroy       (501) staff       (20)       38 2023-06-15 08:48:43.362553 chatglm-llm-1.3.7/setup.cfg
--rw-r--r--   0 mroy       (501) staff       (20)     1026 2023-06-15 08:48:34.000000 chatglm-llm-1.3.7/setup.py
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-16 02:42:45.831946 chatglm-llm-1.4.0/
+-rw-r--r--   0 mroy       (501) staff       (20)       36 2023-05-10 01:48:15.000000 chatglm-llm-1.4.0/MANIFEST.in
+-rw-r--r--   0 mroy       (501) staff       (20)      212 2023-06-16 02:42:45.831833 chatglm-llm-1.4.0/PKG-INFO
+-rw-r--r--   0 mroy       (501) staff       (20)     1887 2023-05-04 01:08:28.000000 chatglm-llm-1.4.0/README.md
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-16 02:42:45.830272 chatglm-llm-1.4.0/chatglm_llm.egg-info/
+-rw-r--r--   0 mroy       (501) staff       (20)      212 2023-06-16 02:42:45.000000 chatglm-llm-1.4.0/chatglm_llm.egg-info/PKG-INFO
+-rw-r--r--   0 mroy       (501) staff       (20)      511 2023-06-16 02:42:45.000000 chatglm-llm-1.4.0/chatglm_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 mroy       (501) staff       (20)        1 2023-06-16 02:42:45.000000 chatglm-llm-1.4.0/chatglm_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 mroy       (501) staff       (20)       53 2023-06-16 02:42:45.000000 chatglm-llm-1.4.0/chatglm_llm.egg-info/entry_points.txt
+-rw-r--r--   0 mroy       (501) staff       (20)        1 2023-05-04 01:12:10.000000 chatglm-llm-1.4.0/chatglm_llm.egg-info/not-zip-safe
+-rw-r--r--   0 mroy       (501) staff       (20)      266 2023-06-16 02:42:45.000000 chatglm-llm-1.4.0/chatglm_llm.egg-info/requires.txt
+-rw-r--r--   0 mroy       (501) staff       (20)       12 2023-06-16 02:42:45.000000 chatglm-llm-1.4.0/chatglm_llm.egg-info/top_level.txt
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-16 02:42:45.831275 chatglm-llm-1.4.0/chatglm_src/
+-rw-r--r--   0 mroy       (501) staff       (20)      755 2023-06-16 02:41:40.000000 chatglm-llm-1.4.0/chatglm_src/__init__.py
+-rw-r--r--   0 mroy       (501) staff       (20)     4201 2023-05-13 02:36:58.000000 chatglm-llm-1.4.0/chatglm_src/callbacks.py
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-16 02:42:45.831564 chatglm-llm-1.4.0/chatglm_src/chains/
+-rw-r--r--   0 mroy       (501) staff       (20)       69 2023-05-10 01:48:15.000000 chatglm-llm-1.4.0/chatglm_src/chains/__init__.py
+-rw-r--r--   0 mroy       (501) staff       (20)     4402 2023-05-11 09:17:21.000000 chatglm-llm-1.4.0/chatglm_src/chains/local_qa.py
+-rw-r--r--   0 mroy       (501) staff       (20)     2608 2023-06-16 00:55:31.000000 chatglm-llm-1.4.0/chatglm_src/cluster_and_smi.py
+-rw-r--r--   0 mroy       (501) staff       (20)      537 2023-05-30 04:20:56.000000 chatglm-llm-1.4.0/chatglm_src/cmd.py
+-rw-r--r--   0 mroy       (501) staff       (20)     3052 2023-06-15 08:48:00.000000 chatglm-llm-1.4.0/chatglm_src/embeding.py
+-rw-r--r--   0 mroy       (501) staff       (20)    37638 2023-06-16 02:31:49.000000 chatglm-llm-1.4.0/chatglm_src/llm.py
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-16 02:42:45.831668 chatglm-llm-1.4.0/chatglm_src/loader/
+-rw-r--r--   0 mroy       (501) staff       (20)     1403 2023-05-11 01:28:05.000000 chatglm-llm-1.4.0/chatglm_src/loader/__init__.py
+-rw-r--r--   0 mroy       (501) staff       (20)       38 2023-06-16 02:42:45.831987 chatglm-llm-1.4.0/setup.cfg
+-rw-r--r--   0 mroy       (501) staff       (20)     1078 2023-06-16 02:42:24.000000 chatglm-llm-1.4.0/setup.py
```

### Comparing `chatglm-llm-1.3.7/README.md` & `chatglm-llm-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.3.7/chatglm_src/__init__.py` & `chatglm-llm-1.4.0/chatglm_src/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import pathlib
 from .llm import ChatGLMLLM,Vicuna13B
 from .chains import KnowdageQA
-from .embeding import ChatGLMEmbeding
+from .embeding import ChatGLMEmbeding as Embeddings
+from .cluster_and_smi import papers as QueryTexts
+
 
 # _EMBEDDING_PATH = pathlib.Path.home() / ".cache" / "chatglm-embedding"
 
 # if not _EMBEDDING_PATH.exists():
 #     print("------ start founding embedding  ------:", _EMBEDDING_PATH)
 #     import os
 #     # unzip emb.zip to _EMBEDDING_PATH
```

### Comparing `chatglm-llm-1.3.7/chatglm_src/callbacks.py` & `chatglm-llm-1.4.0/chatglm_src/callbacks.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.3.7/chatglm_src/chains/local_qa.py` & `chatglm-llm-1.4.0/chatglm_src/chains/local_qa.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.3.7/chatglm_src/cmd.py` & `chatglm-llm-1.4.0/chatglm_src/cmd.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.3.7/chatglm_src/embeding.py` & `chatglm-llm-1.4.0/chatglm_src/embeding.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.3.7/chatglm_src/llm.py` & `chatglm-llm-1.4.0/chatglm_src/llm.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from websocket import create_connection
 import websockets
 from websockets.server import serve
 from langchain.embeddings import HuggingFaceEmbeddings
 import gptcache
 from gptcache.processor.pre import get_prompt
 from gptcache.manager.factory import get_data_manager
-
+from .cluster_and_smi import cluster, similarity
 try:
     from langchain.cache import GPTCache
 except:
     pass
 
 
 try:
@@ -50,14 +50,19 @@
     
     langchain.llm_cache = GPTCache(init_gptcache_map)
     print(colored("init gptcache", "green"))
 except Exception as e:
     print("use remote ignore this / load transformers failed, please install transformers and accelerate first and torch.")
 from .callbacks import AsyncWebsocketHandler, AsyncWebSocksetCallbackManager
 
+TEXT_EMB_PATH = pathlib.Path("~").expanduser() / ".cache"/"torch"/"sentence_transformers"/"GanymedeNil_text2vec-large-chinese"
+if TEXT_EMB_PATH.exists():
+    TEXT_EMB_PATH = str(TEXT_EMB_PATH)
+else:
+    TEXT_EMB_PATH = "GanymedeNil/text2vec-large-chinese"
 
 def is_async_method(method):
     return inspect.iscoroutinefunction(method)
 ## LLM for chatglm
 # only load from local's path
 # default path is in ~/.cache/chatglm, if not exists, will download from huggingface'url :https://huggingface.co/THUDM/chatglm-6b
 # 
@@ -725,15 +730,19 @@
     
     async def reply(self, data):
         await self.websocket.send(str(len(data)))
         for i in range(0,len(data), 1024*1024*2):
             await self.websocket.send(data[i:i+1024*1024*2])
         await self.websocket.send("[STOP]")
     
-    async def __call__(self, prompt=None,model=None,temperature=None, embed_documents=None,embed_query=None,history=None):
+    async def __call__(self, 
+                       prompt=None,model=None,temperature=None,
+                       embed_documents=None,embed_query=None,
+                       method=None, eps=None, min_samples=None,n_clusters=None,
+                       history=None):
         try:
             # assert prompt is not None 
             if prompt is not None:
                 assert isinstance(prompt, str)
                 assert model is not None
                 if model == "chatglm":
                     llm = self.llm
@@ -748,28 +757,47 @@
                         current_completion = response
                         data = { "new":delta,"response": response, "history": history,"query": prompt}
                         await self.websocket.send(json.dumps(data))
                     data = { "new":delta,"response": response, "history": history,"query": prompt, "stop":True}
                 elif model == "vicuna-13b":
                     
                     data = await self.llm._ncall(self.websocket, prompt, history,temperature=temperature)
-                    
+                
                 else:
                     data = { "new":"X","response": "Not Support Model !:"+model, "history": history,"query": prompt, "stop":True}
                 await self.websocket.send(json.dumps(data))
             elif embed_query is not None:
                 res = self.embeding.embed_query(embed_query)
                 data = { "embed":res} 
                 data = json.dumps(data, cls=NumpyEncoder)
                 await self.reply(data)
-            elif embed_documents is not None:
+            elif embed_documents is not None and method is None:
                 res = self.embeding.embed_documents(embed_documents)
                 data = { "embed":res}
                 data = json.dumps(data, cls=NumpyEncoder)
                 await self.reply(data)
+            elif method is not None and embed_documents is not None:
+                res = self.embeding.embed_documents(embed_documents)
+
+                if method in ['kmeans', 'dbscan']:
+                    labels = cluster(res, eps=eps, min_samples=min_samples, method=method, n_clusters=n_clusters)
+                    data = {}
+                    for ix, document in enumerate(embed_documents):
+                        l = labels[ix]
+                        if l != -1: # remove noise
+                            continue
+                        data[l] = data.get(l, []) + [document]
+                    data = json.dumps(data, cls=NumpyEncoder)
+                    await self.reply(data)
+                elif method in ["euclidean","cosine"]:
+                    data = {"similarity":similarity(res, method=method)}
+                    data = json.dumps(data, cls=NumpyEncoder)
+                    await self.reply(data)
+                else:
+                    await self.reply({"msg":"not support method:"+method})
         finally:
             auto_gc()
 
 
 
 class AsyncServer:
     __users = {}
@@ -884,15 +912,16 @@
 
     @classmethod
     def start(cls,port=15000, model_path=None, name="chatglm"):
         cpu = False
         if not torch.cuda.is_available():
             cpu = True
         print(colored(f"[cpu:{cpu} ]","green"),":",f"listen:0.0.0.0:{port}")
-        cls.embeding = HuggingFaceEmbeddings(model_name="GanymedeNil/text2vec-large-chinese")
+        
+        cls.embeding = HuggingFaceEmbeddings(model_name=TEXT_EMB_PATH)
         print(colored(f"[embedding: use cpu{cpu} ]","green"),":",f"GanymedeNil/text2vec-large-chinese")
         if name == "chatglm":
             cls.llm = ChatGLMLLM.load(model_path=model_path, cpu=cpu, streaming=True)
             print(colored(f"[ starting chatglm]","green"),":",f"listen:0.0.0.0:{port}")
         elif name == "vicuna-13b":
             cls.llm = Vicuna13B.load(model_path=model_path, cpu=cpu, streaming=True)
             print(colored(f"[ starting vicuna-13b]","green"),":",f"listen:0.0.0.0:{port}")
```

### Comparing `chatglm-llm-1.3.7/chatglm_src/loader/__init__.py` & `chatglm-llm-1.4.0/chatglm_src/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.3.7/setup.py` & `chatglm-llm-1.4.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 
 setup(name='chatglm-llm',
-    version='1.3.7',
+    version='1.4.0',
     description='chatglm llm',
     url='https://github.com/xxx',
     author='auth',
     author_email='xxx@gmail.com',
     license='MIT',
     include_package_data=True,
     zip_safe=False,
@@ -18,25 +18,27 @@
             'tensorboard',
             "protobuf",
             "fschat==0.2.2",
             "cpm_kernels",
             "mdtex2html",
             "sentencepiece",
             "accelerate",
+            "scikit-learn",
             'torch',    
             'transformers',
         ],
     },
     install_requires=[
         'requests',
         'termcolor',
         'tqdm',
         'gptcache',
         'numpy',
         'pypdf',
+        "scikit-learn",
         'langchain',
         'websockets',
         'websocket-client',
         'unstructured',
         'aiowebsocket',
         ],
     entry_points={
```

