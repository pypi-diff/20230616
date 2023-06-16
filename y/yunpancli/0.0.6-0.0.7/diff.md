# Comparing `tmp/yunpancli-0.0.6.tar.gz` & `tmp/yunpancli-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yunpancli-0.0.6.tar", last modified: Thu May 25 06:27:07 2023, max compression
+gzip compressed data, was "yunpancli-0.0.7.tar", last modified: Fri Jun 16 09:03:50 2023, max compression
```

## Comparing `yunpancli-0.0.6.tar` & `yunpancli-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-25 06:27:07.081769 yunpancli-0.0.6/
--rw-r--r--   0 mac        (501) staff       (20)     1063 2023-05-02 10:51:07.000000 yunpancli-0.0.6/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)      436 2023-05-25 06:27:07.081874 yunpancli-0.0.6/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-05-03 08:16:36.000000 yunpancli-0.0.6/README.md
--rw-r--r--   0 mac        (501) staff       (20)      125 2023-05-25 06:27:07.082216 yunpancli-0.0.6/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      689 2023-05-25 06:26:26.000000 yunpancli-0.0.6/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-25 06:27:07.080568 yunpancli-0.0.6/yunpancli/
--rw-r--r--   0 mac        (501) staff       (20)       39 2023-05-03 08:15:03.000000 yunpancli-0.0.6/yunpancli/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     8499 2023-05-03 10:18:36.000000 yunpancli-0.0.6/yunpancli/baidu_pan_sdk.py
--rw-r--r--   0 mac        (501) staff       (20)     7146 2023-05-25 03:04:58.000000 yunpancli-0.0.6/yunpancli/base.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-25 06:27:07.081623 yunpancli-0.0.6/yunpancli.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      436 2023-05-25 06:27:07.000000 yunpancli-0.0.6/yunpancli.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      303 2023-05-25 06:27:07.000000 yunpancli-0.0.6/yunpancli.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-25 06:27:07.000000 yunpancli-0.0.6/yunpancli.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       42 2023-05-25 06:27:07.000000 yunpancli-0.0.6/yunpancli.egg-info/entry_points.txt
--rw-r--r--   0 mac        (501) staff       (20)       14 2023-05-25 06:27:07.000000 yunpancli-0.0.6/yunpancli.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       10 2023-05-25 06:27:07.000000 yunpancli-0.0.6/yunpancli.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-16 09:03:50.428973 yunpancli-0.0.7/
+-rw-r--r--   0 mac        (501) staff       (20)     1063 2023-05-02 10:51:07.000000 yunpancli-0.0.7/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)      436 2023-06-16 09:03:50.429151 yunpancli-0.0.7/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-05-03 08:16:36.000000 yunpancli-0.0.7/README.md
+-rw-r--r--   0 mac        (501) staff       (20)      138 2023-06-16 09:03:50.429528 yunpancli-0.0.7/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      689 2023-06-16 07:46:08.000000 yunpancli-0.0.7/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-16 09:03:50.427461 yunpancli-0.0.7/yunpancli/
+-rw-r--r--   0 mac        (501) staff       (20)       39 2023-05-03 08:15:03.000000 yunpancli-0.0.7/yunpancli/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     9592 2023-06-16 09:01:50.000000 yunpancli-0.0.7/yunpancli/baidu_pan_sdk.py
+-rw-r--r--   0 mac        (501) staff       (20)     7241 2023-05-26 02:59:50.000000 yunpancli-0.0.7/yunpancli/base.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-06-16 09:03:50.428704 yunpancli-0.0.7/yunpancli.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      436 2023-06-16 09:03:50.000000 yunpancli-0.0.7/yunpancli.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      303 2023-06-16 09:03:50.000000 yunpancli-0.0.7/yunpancli.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-06-16 09:03:50.000000 yunpancli-0.0.7/yunpancli.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       42 2023-06-16 09:03:50.000000 yunpancli-0.0.7/yunpancli.egg-info/entry_points.txt
+-rw-r--r--   0 mac        (501) staff       (20)       26 2023-06-16 09:03:50.000000 yunpancli-0.0.7/yunpancli.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       10 2023-06-16 09:03:50.000000 yunpancli-0.0.7/yunpancli.egg-info/top_level.txt
```

### Comparing `yunpancli-0.0.6/LICENSE` & `yunpancli-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `yunpancli-0.0.6/setup.py` & `yunpancli-0.0.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yunpancli",
     entry_points={"console_scripts": ["pancli=yunpancli:main"]},
-    version="0.0.6",
+    version="0.0.7",
     author="Tang Yubin",
     author_email="tang-yu-bin@qq.com",
     description="cloud storage CLI (Command Line Interface)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/aierwiki/yunpancli",
     packages=setuptools.find_packages(),
```

### Comparing `yunpancli-0.0.6/yunpancli/baidu_pan_sdk.py` & `yunpancli-0.0.7/yunpancli/baidu_pan_sdk.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import requests
 import json
 import os
+import math
 import hashlib
 from urllib.parse import urlencode
+from rich.progress import track
 from loguru import logger
 logger.remove(0)
 
 
 class BaiduPanSDK:
     # access_token获取地址
     ACCESS_TOKEN_API = 'https://openapi.baidu.com/oauth/2.0/token'
@@ -56,65 +58,87 @@
             'uploadid': uploadid,
             'block_list': block_list
         }
         response = requests.post(api, data=data)
 
     # 分片上传
     def upload(self, remote_path, uploadid, partseq, file_path, access_token):
-        data = {}
-        files = [
-            ('file', open(file_path, 'rb'))
-        ]
-        params = {
-            'method': 'upload',
-            'access_token': access_token,
-            'path': remote_path,
-            'type': 'tmpfile',
-            'uploadid': uploadid,
-            'partseq': partseq
-        }
-        api = BaiduPanSDK.UPLOAD_API + urlencode(params)
-        res = requests.post(api, data=data, files=files)
         
-    def precreate(self, local_file_path, remote_file_path, access_token):
-        size = os.path.getsize(local_file_path)  
+        with open(file_path, "rb") as f:
+            size = os.path.getsize(file_path)
+            buffer_size = 4 * 1024 * 1024
+            buffer_cnt = math.ceil(size / buffer_size)
+            for seq in track(range(buffer_cnt), description="上传中..."):
+                buffer = f.read(buffer_size)
+                if not buffer:
+                    break
+                files = [
+                    ('file', buffer)
+                ]
+                params = {
+                    'method': 'upload',
+                    'access_token': access_token,
+                    'path': remote_path,
+                    'type': 'tmpfile',
+                    'uploadid': uploadid,
+                    'partseq': seq
+                }
+                api = BaiduPanSDK.UPLOAD_API + urlencode(params)
+                res = requests.post(api, files=files)
+                if res.status_code != 200:
+                    print(BaiduPanSDK.ERROR_INFO.get(res['errno'], '未知错误'))
+                    return False
+        
+        return True
+        
+    def precreate(self, local_file_path, remote_file_path, access_token):  
         block_list = []
         with open(local_file_path, 'rb') as f:
-            data = f.read()
-            file_md5 = hashlib.md5(data).hexdigest()
-            block_list.append(file_md5)
-            f.close()
+            size = os.path.getsize(local_file_path)
+            buffer_size = 4 * 1024 * 1024
+            buffer_cnt = math.ceil(size / buffer_size)
+            for seq in track(range(buffer_cnt), description="文件读取中..."):
+                buffer = f.read(buffer_size)
+                if not buffer:
+                    break
+                buffer_md5 = hashlib.md5(buffer).hexdigest()
+                block_list.append(buffer_md5)   
         block_list = json.dumps(block_list)
         params = {
             'method': 'precreate',
             'access_token': access_token,
         }
         data = {
             'path': remote_file_path,
             'size': size,
             'isdir': 0,
             'autoinit': 1,
             'block_list': block_list
         }
         api = BaiduPanSDK.PRECREATE_API + urlencode(params)
         res = requests.post(api, data=data)
+        if res.status_code != 200:
+            print(BaiduPanSDK.ERROR_INFO.get(res['errno'], '未知错误'))
+            return None, None, None
         json_resp = json.loads(res.content)
-        if "path" in json_resp:
-            return json_resp['uploadid'], size, block_list
-        else:
-            return '', size, block_list
+        return json_resp['uploadid'], size, block_list
         
     def upload_file(self, local_file_path, remote_file_path, access_token):
         logger.debug(f"upload {local_file_path} to {remote_file_path}")
         # 1. 预上传
         uploadid, size, block_list = self.precreate(local_file_path, remote_file_path, access_token)
+        if uploadid is None:
+            return False
         # 2. 分片上传（文件切片这里没有做，超级会员单文件最大20G）
-        self.upload(remote_file_path, uploadid, 0, local_file_path, access_token)
+        ret = self.upload(remote_file_path, uploadid, 0, local_file_path, access_token)
+        if not ret:
+            return False
         # 3. 创建文件
         self.create(remote_file_path, size, uploadid, block_list, access_token)
+        return True
     
     def get_file_list(self, dir, access_token):
         params = {
             'method': 'list',
             'access_token': access_token,
             'dir': dir,
             'showempty': 1
@@ -182,15 +206,15 @@
         if res['errno'] != 0:
             print(BaiduPanSDK.ERROR_INFO.get(res['errno'], '未知错误'))
             return False
         result_list = res['list']
         dlink_list = [result['dlink'] for result in result_list]
         dlink = dlink_list[0]
         download_url = dlink + f'&access_token={access_token}'
-        cmd = f"wget --header='User-Agent: pan.baidu.com' -q '{download_url}' -O {os.path.join(dest, filename)}"
+        cmd = f"wget --header='User-Agent: pan.baidu.com' '{download_url}' -O {os.path.join(dest, filename)}"
         logger.debug(f"cmd = {cmd}")
         print(f"download {filename} complete !")
         os.system(cmd)
         
     
     def download(self, pan_path, dest, access_token):
         logger.debug(f"download {pan_path} to {dest}")
```

### Comparing `yunpancli-0.0.6/yunpancli/base.py` & `yunpancli-0.0.7/yunpancli/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
             if key not in account_info:
                 logger.debug(f"{key} not in account_info")
                 return False
         self.account_info = account_info
         return True
 
     def handle_config(self):
+        print("配置参数获取请参考文档：https://pan.baidu.com/union/doc/ol0rsap9s")
         app_key = input("请输入AppKey:")
         secret_key = input("请输入SecretKey:")
         url = f"https://openapi.baidu.com/oauth/2.0/authorize?response_type=code&client_id={app_key}&redirect_uri=oob&scope=basic,netdisk&force_login=1"
         print(f"请点击下面的链接，打开页面获取授权码：{url}")
         auth_code = input("请输入授权码:")
         refresh_token, access_token = self.sdk.get_access_token(auth_code, app_key, secret_key)
         account_info = {
```

