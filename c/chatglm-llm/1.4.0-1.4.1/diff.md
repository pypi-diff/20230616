# Comparing `tmp/chatglm-llm-1.4.0.tar.gz` & `tmp/chatglm-llm-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatglm-llm-1.4.0.tar", last modified: Fri Jun 16 02:42:45 2023, max compression
+gzip compressed data, was "chatglm-llm-1.4.1.tar", last modified: Fri Jun 16 08:15:31 2023, max compression
```

## Comparing `chatglm-llm-1.4.0.tar` & `chatglm-llm-1.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-16 02:42:45.831946 chatglm-llm-1.4.0/
--rw-r--r--   0 mroy       (501) staff       (20)       36 2023-05-10 01:48:15.000000 chatglm-llm-1.4.0/MANIFEST.in
--rw-r--r--   0 mroy       (501) staff       (20)      212 2023-06-16 02:42:45.831833 chatglm-llm-1.4.0/PKG-INFO
--rw-r--r--   0 mroy       (501) staff       (20)     1887 2023-05-04 01:08:28.000000 chatglm-llm-1.4.0/README.md
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-16 02:42:45.830272 chatglm-llm-1.4.0/chatglm_llm.egg-info/
--rw-r--r--   0 mroy       (501) staff       (20)      212 2023-06-16 02:42:45.000000 chatglm-llm-1.4.0/chatglm_llm.egg-info/PKG-INFO
--rw-r--r--   0 mroy       (501) staff       (20)      511 2023-06-16 02:42:45.000000 chatglm-llm-1.4.0/chatglm_llm.egg-info/SOURCES.txt
--rw-r--r--   0 mroy       (501) staff       (20)        1 2023-06-16 02:42:45.000000 chatglm-llm-1.4.0/chatglm_llm.egg-info/dependency_links.txt
--rw-r--r--   0 mroy       (501) staff       (20)       53 2023-06-16 02:42:45.000000 chatglm-llm-1.4.0/chatglm_llm.egg-info/entry_points.txt
--rw-r--r--   0 mroy       (501) staff       (20)        1 2023-05-04 01:12:10.000000 chatglm-llm-1.4.0/chatglm_llm.egg-info/not-zip-safe
--rw-r--r--   0 mroy       (501) staff       (20)      266 2023-06-16 02:42:45.000000 chatglm-llm-1.4.0/chatglm_llm.egg-info/requires.txt
--rw-r--r--   0 mroy       (501) staff       (20)       12 2023-06-16 02:42:45.000000 chatglm-llm-1.4.0/chatglm_llm.egg-info/top_level.txt
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-16 02:42:45.831275 chatglm-llm-1.4.0/chatglm_src/
--rw-r--r--   0 mroy       (501) staff       (20)      755 2023-06-16 02:41:40.000000 chatglm-llm-1.4.0/chatglm_src/__init__.py
--rw-r--r--   0 mroy       (501) staff       (20)     4201 2023-05-13 02:36:58.000000 chatglm-llm-1.4.0/chatglm_src/callbacks.py
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-16 02:42:45.831564 chatglm-llm-1.4.0/chatglm_src/chains/
--rw-r--r--   0 mroy       (501) staff       (20)       69 2023-05-10 01:48:15.000000 chatglm-llm-1.4.0/chatglm_src/chains/__init__.py
--rw-r--r--   0 mroy       (501) staff       (20)     4402 2023-05-11 09:17:21.000000 chatglm-llm-1.4.0/chatglm_src/chains/local_qa.py
--rw-r--r--   0 mroy       (501) staff       (20)     2608 2023-06-16 00:55:31.000000 chatglm-llm-1.4.0/chatglm_src/cluster_and_smi.py
--rw-r--r--   0 mroy       (501) staff       (20)      537 2023-05-30 04:20:56.000000 chatglm-llm-1.4.0/chatglm_src/cmd.py
--rw-r--r--   0 mroy       (501) staff       (20)     3052 2023-06-15 08:48:00.000000 chatglm-llm-1.4.0/chatglm_src/embeding.py
--rw-r--r--   0 mroy       (501) staff       (20)    37638 2023-06-16 02:31:49.000000 chatglm-llm-1.4.0/chatglm_src/llm.py
-drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-16 02:42:45.831668 chatglm-llm-1.4.0/chatglm_src/loader/
--rw-r--r--   0 mroy       (501) staff       (20)     1403 2023-05-11 01:28:05.000000 chatglm-llm-1.4.0/chatglm_src/loader/__init__.py
--rw-r--r--   0 mroy       (501) staff       (20)       38 2023-06-16 02:42:45.831987 chatglm-llm-1.4.0/setup.cfg
--rw-r--r--   0 mroy       (501) staff       (20)     1078 2023-06-16 02:42:24.000000 chatglm-llm-1.4.0/setup.py
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-16 08:15:31.134631 chatglm-llm-1.4.1/
+-rw-r--r--   0 mroy       (501) staff       (20)       36 2023-05-10 01:48:15.000000 chatglm-llm-1.4.1/MANIFEST.in
+-rw-r--r--   0 mroy       (501) staff       (20)      212 2023-06-16 08:15:31.134503 chatglm-llm-1.4.1/PKG-INFO
+-rw-r--r--   0 mroy       (501) staff       (20)     1887 2023-05-04 01:08:28.000000 chatglm-llm-1.4.1/README.md
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-16 08:15:31.133267 chatglm-llm-1.4.1/chatglm_llm.egg-info/
+-rw-r--r--   0 mroy       (501) staff       (20)      212 2023-06-16 08:15:30.000000 chatglm-llm-1.4.1/chatglm_llm.egg-info/PKG-INFO
+-rw-r--r--   0 mroy       (501) staff       (20)      511 2023-06-16 08:15:31.000000 chatglm-llm-1.4.1/chatglm_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 mroy       (501) staff       (20)        1 2023-06-16 08:15:30.000000 chatglm-llm-1.4.1/chatglm_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 mroy       (501) staff       (20)       53 2023-06-16 08:15:30.000000 chatglm-llm-1.4.1/chatglm_llm.egg-info/entry_points.txt
+-rw-r--r--   0 mroy       (501) staff       (20)        1 2023-05-04 01:12:10.000000 chatglm-llm-1.4.1/chatglm_llm.egg-info/not-zip-safe
+-rw-r--r--   0 mroy       (501) staff       (20)      266 2023-06-16 08:15:31.000000 chatglm-llm-1.4.1/chatglm_llm.egg-info/requires.txt
+-rw-r--r--   0 mroy       (501) staff       (20)       12 2023-06-16 08:15:31.000000 chatglm-llm-1.4.1/chatglm_llm.egg-info/top_level.txt
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-16 08:15:31.133895 chatglm-llm-1.4.1/chatglm_src/
+-rw-r--r--   0 mroy       (501) staff       (20)      755 2023-06-16 02:41:40.000000 chatglm-llm-1.4.1/chatglm_src/__init__.py
+-rw-r--r--   0 mroy       (501) staff       (20)     4201 2023-05-13 02:36:58.000000 chatglm-llm-1.4.1/chatglm_src/callbacks.py
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-16 08:15:31.134178 chatglm-llm-1.4.1/chatglm_src/chains/
+-rw-r--r--   0 mroy       (501) staff       (20)       69 2023-05-10 01:48:15.000000 chatglm-llm-1.4.1/chatglm_src/chains/__init__.py
+-rw-r--r--   0 mroy       (501) staff       (20)     4402 2023-05-11 09:17:21.000000 chatglm-llm-1.4.1/chatglm_src/chains/local_qa.py
+-rw-r--r--   0 mroy       (501) staff       (20)     2777 2023-06-16 06:08:22.000000 chatglm-llm-1.4.1/chatglm_src/cluster_and_smi.py
+-rw-r--r--   0 mroy       (501) staff       (20)      537 2023-05-30 04:20:56.000000 chatglm-llm-1.4.1/chatglm_src/cmd.py
+-rw-r--r--   0 mroy       (501) staff       (20)     3052 2023-06-15 08:48:00.000000 chatglm-llm-1.4.1/chatglm_src/embeding.py
+-rw-r--r--   0 mroy       (501) staff       (20)    38577 2023-06-16 07:01:29.000000 chatglm-llm-1.4.1/chatglm_src/llm.py
+drwxr-xr-x   0 mroy       (501) staff       (20)        0 2023-06-16 08:15:31.134293 chatglm-llm-1.4.1/chatglm_src/loader/
+-rw-r--r--   0 mroy       (501) staff       (20)     1403 2023-05-11 01:28:05.000000 chatglm-llm-1.4.1/chatglm_src/loader/__init__.py
+-rw-r--r--   0 mroy       (501) staff       (20)       38 2023-06-16 08:15:31.134679 chatglm-llm-1.4.1/setup.cfg
+-rw-r--r--   0 mroy       (501) staff       (20)     1078 2023-06-16 08:15:26.000000 chatglm-llm-1.4.1/setup.py
```

### Comparing `chatglm-llm-1.4.0/README.md` & `chatglm-llm-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.0/chatglm_src/__init__.py` & `chatglm-llm-1.4.1/chatglm_src/__init__.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.0/chatglm_src/callbacks.py` & `chatglm-llm-1.4.1/chatglm_src/callbacks.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.0/chatglm_src/chains/local_qa.py` & `chatglm-llm-1.4.1/chatglm_src/chains/local_qa.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.0/chatglm_src/cluster_and_smi.py` & `chatglm-llm-1.4.1/chatglm_src/cluster_and_smi.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,36 +8,38 @@
 import json
 from termcolor import colored
 import tqdm
 
 TODAY = datetime.datetime.now()
 PASSWORD = "ADSFADSGADSHDAFHDSG@#%!@#T%DSAGADSHDFAGSY@#%@!#^%@#$Y^#$TYDGVDFSGDS!@$!@$" + f"{TODAY.year}-{TODAY.month}"
 
-def cluster(data, n_clusters=2,eps=0.3,min_samples=3, method='kmeans'):
+def cluster(data, n_clusters=2,eps=0.5,min_samples=3, method='kmeans'):
     
     if method == 'kmeans':
-        kmeans = KMeans(n_clusters=n_clusters, random_state=0).fit(data)
+        kmeans = KMeans(n_clusters=n_clusters, random_state=0, n_init='auto').fit(data)
         return kmeans.labels_
     elif method == 'dbscan':
-        db = DBSCAN(eps=eps, min_samples=min_samples).fit(data)
+        db = DBSCAN(metric='euclidean',eps=eps, min_samples=min_samples).fit(data)
         return db.labels_
+    elif method == 'cosine':
+        sim_vec = cosine_similarity(data).tolist()
     else:
         raise ValueError('method must be kmeans or dbscan')
 
 
 def similarity(data, method='cosine'):
     if method == 'cosine':
         return cosine_similarity(data).tolist()
     elif method == 'euclidean':
         return euclidean_distances(data).tolist()
     else:
         raise ValueError('method must be cosine or euclidean')
 
 
-def papers(remote_host,texts, method="dbscan", eps=0.3, min_samples=3, n_clusters=2):
+def papers(remote_host,texts, method="dbscan", eps=0.3, min_samples=3, n_clusters=2,filter_noise=None):
     """
     @method : str, default='dbscan' , can used 'kmeans' or 'dbscan' or 'cosine' or 'euclidean'
         @eps : float, default=0.3, used in dbscan
         @min_samples : int, default=3, used in dbscan
         @n_clusters : int, default=2, used in kmeans
     
     """
@@ -50,14 +52,15 @@
         print(colored("[info]:","yellow") ,res)
         raise Exception("password error")
     
     data = json.dumps({
         "embed_documents":texts,
         "method":method,
         "n_clusters":n_clusters,
+        "filter_noise":filter_noise,
         "eps":eps,
         "min_samples":min_samples
 
     })
     msg = send_and_recv(data, ws)
     return msg
```

### Comparing `chatglm-llm-1.4.0/chatglm_src/cmd.py` & `chatglm-llm-1.4.1/chatglm_src/cmd.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.0/chatglm_src/embeding.py` & `chatglm-llm-1.4.1/chatglm_src/embeding.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.0/chatglm_src/llm.py` & `chatglm-llm-1.4.1/chatglm_src/llm.py`

 * *Files 3% similar despite different names*

```diff
@@ -734,14 +734,15 @@
             await self.websocket.send(data[i:i+1024*1024*2])
         await self.websocket.send("[STOP]")
     
     async def __call__(self, 
                        prompt=None,model=None,temperature=None,
                        embed_documents=None,embed_query=None,
                        method=None, eps=None, min_samples=None,n_clusters=None,
+                       filter_noise=None,
                        history=None):
         try:
             # assert prompt is not None 
             if prompt is not None:
                 assert isinstance(prompt, str)
                 assert model is not None
                 if model == "chatglm":
@@ -768,36 +769,50 @@
             elif embed_query is not None:
                 res = self.embeding.embed_query(embed_query)
                 data = { "embed":res} 
                 data = json.dumps(data, cls=NumpyEncoder)
                 await self.reply(data)
             elif embed_documents is not None and method is None:
                 res = self.embeding.embed_documents(embed_documents)
+                if filter_noise is not None:
+                    # filter noise value in vec, for example: 
+                    # vec exists 512 dim, but most of them are a small value, we can filter them
+                    w = np.array(res)
+                    w[np.abs(w) < filter_noise] = 0
+                    res = w.tolist()
                 data = { "embed":res}
                 data = json.dumps(data, cls=NumpyEncoder)
                 await self.reply(data)
             elif method is not None and embed_documents is not None:
                 res = self.embeding.embed_documents(embed_documents)
+                if filter_noise is not None:
+                    # filter noise value in vec, for example: 
+                    # vec exists 512 dim, but most of them are a small value, we can filter them
+                    w = np.array(res)
+                    w[np.abs(w) < filter_noise] = 0
+                    res = w.tolist()
 
                 if method in ['kmeans', 'dbscan']:
+                    print(colored("[method]","green"),":",method, colored("[eps]","green"),":",eps, colored("[min_samples]","green"),":",min_samples, colored("[n_clusters]","green"),":",n_clusters)
                     labels = cluster(res, eps=eps, min_samples=min_samples, method=method, n_clusters=n_clusters)
                     data = {}
                     for ix, document in enumerate(embed_documents):
                         l = labels[ix]
-                        if l != -1: # remove noise
+                        if l < 0: # remove noise
                             continue
+                        
                         data[l] = data.get(l, []) + [document]
                     data = json.dumps(data, cls=NumpyEncoder)
                     await self.reply(data)
                 elif method in ["euclidean","cosine"]:
                     data = {"similarity":similarity(res, method=method)}
                     data = json.dumps(data, cls=NumpyEncoder)
                     await self.reply(data)
                 else:
-                    await self.reply({"msg":"not support method:"+method})
+                    await self.reply(json.dumps({"msg":"not support method:"+method}))
         finally:
             auto_gc()
 
 
 
 class AsyncServer:
     __users = {}
```

### Comparing `chatglm-llm-1.4.0/chatglm_src/loader/__init__.py` & `chatglm-llm-1.4.1/chatglm_src/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `chatglm-llm-1.4.0/setup.py` & `chatglm-llm-1.4.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 
 setup(name='chatglm-llm',
-    version='1.4.0',
+    version='1.4.1',
     description='chatglm llm',
     url='https://github.com/xxx',
     author='auth',
     author_email='xxx@gmail.com',
     license='MIT',
     include_package_data=True,
     zip_safe=False,
```

