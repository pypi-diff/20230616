# Comparing `tmp/fastsession-0.1.2.tar.gz` & `tmp/fastsession-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastsession-0.1.2.tar", last modified: Mon May 22 02:50:06 2023, max compression
+gzip compressed data, was "fastsession-0.2.0.tar", last modified: Fri Jun 16 02:51:02 2023, max compression
```

## Comparing `fastsession-0.1.2.tar` & `fastsession-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 02:50:06.779543 fastsession-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-05-22 02:50:06.684017 fastsession-0.1.2/FastSession.egg-info/
--rw-rw-rw-   0        0        0     3272 2023-05-22 02:50:06.000000 fastsession-0.1.2/FastSession.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      626 2023-05-22 02:50:06.000000 fastsession-0.1.2/FastSession.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 02:50:06.000000 fastsession-0.1.2/FastSession.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-05-22 02:50:06.000000 fastsession-0.1.2/FastSession.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-22 02:50:06.000000 fastsession-0.1.2/FastSession.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11556 2023-05-05 05:02:46.000000 fastsession-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     3272 2023-05-22 02:50:06.775546 fastsession-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2557 2023-05-15 07:54:01.000000 fastsession-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 02:50:06.733013 fastsession-0.1.2/fastsession/
--rw-rw-rw-   0        0        0      165 2023-05-15 04:03:26.000000 fastsession-0.1.2/fastsession/__init__.py
--rw-rw-rw-   0        0        0    10213 2023-05-15 07:50:50.000000 fastsession-0.1.2/fastsession/fast_session_middleware.py
--rw-rw-rw-   0        0        0     3703 2023-05-15 07:22:02.000000 fastsession-0.1.2/fastsession/memory_store.py
--rw-rw-rw-   0        0        0     3020 2023-05-15 03:33:44.000000 fastsession-0.1.2/fastsession/timed_signature_serializer.py
--rw-rw-rw-   0        0        0       42 2023-05-22 02:50:06.780546 fastsession-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-05-22 02:43:40.000000 fastsession-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 02:50:06.772542 fastsession-0.1.2/tests/
--rw-rw-rw-   0        0        0        0 2023-05-14 08:02:49.000000 fastsession-0.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0     8754 2023-05-15 07:00:42.000000 fastsession-0.1.2/tests/test_session_middleware.py
--rw-rw-rw-   0        0        0      636 2023-05-15 01:16:58.000000 fastsession-0.1.2/tests/test_store_memory.py
--rw-rw-rw-   0        0        0     1740 2023-05-15 07:44:41.000000 fastsession-0.1.2/tests/test_timed_signature_serializer.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:51:02.876707 fastsession-0.2.0/
+drwxrwxrwx   0        0        0        0 2023-06-16 02:51:02.853258 fastsession-0.2.0/FastSession.egg-info/
+-rw-rw-rw-   0        0        0     3439 2023-06-16 02:51:02.000000 fastsession-0.2.0/FastSession.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      626 2023-06-16 02:51:02.000000 fastsession-0.2.0/FastSession.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 02:51:02.000000 fastsession-0.2.0/FastSession.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-16 02:51:02.000000 fastsession-0.2.0/FastSession.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-16 02:51:02.000000 fastsession-0.2.0/FastSession.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11556 2023-05-05 05:02:46.000000 fastsession-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3439 2023-06-16 02:51:02.875488 fastsession-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2722 2023-06-16 02:47:25.000000 fastsession-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 02:51:02.869258 fastsession-0.2.0/fastsession/
+-rw-rw-rw-   0        0        0      165 2023-05-15 04:03:26.000000 fastsession-0.2.0/fastsession/__init__.py
+-rw-rw-rw-   0        0        0    14070 2023-06-16 02:44:52.000000 fastsession-0.2.0/fastsession/fast_session_middleware.py
+-rw-rw-rw-   0        0        0     3703 2023-05-15 07:22:02.000000 fastsession-0.2.0/fastsession/memory_store.py
+-rw-rw-rw-   0        0        0     3020 2023-05-15 03:33:44.000000 fastsession-0.2.0/fastsession/timed_signature_serializer.py
+-rw-rw-rw-   0        0        0       42 2023-06-16 02:51:02.876707 fastsession-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      951 2023-06-16 02:43:42.000000 fastsession-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 02:51:02.875488 fastsession-0.2.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-14 08:02:49.000000 fastsession-0.2.0/tests/__init__.py
+-rw-rw-rw-   0        0        0    11390 2023-06-16 02:28:12.000000 fastsession-0.2.0/tests/test_session_middleware.py
+-rw-rw-rw-   0        0        0      636 2023-05-15 01:16:58.000000 fastsession-0.2.0/tests/test_store_memory.py
+-rw-rw-rw-   0        0        0     1740 2023-05-15 07:44:41.000000 fastsession-0.2.0/tests/test_timed_signature_serializer.py
```

### Comparing `fastsession-0.1.2/FastSession.egg-info/PKG-INFO` & `fastsession-0.2.0/FastSession.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastsession
-Version: 0.1.2
+Version: 0.2.0
 Summary: A session middleware for Starlette and FastAPI
 Home-page: https://github.com/riversun/FastSession
 Author: Tom Misawa
 Author-email: riversun.org@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,14 +13,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FastSession
 
+[English](https://github.com/riversun/FastSession/blob/main/README.md) | [&#26085;&#26412;&#35486;](https://github.com/riversun/FastSession/blob/main/README_ja.md)
+
 FastSession is a session management library for FastAPI. 
 
 It provides a middleware, `FastSessionMiddleware`, 
 that helps you manage user sessions effectively in your FastAPI applications.
 
 ## Features
```

### Comparing `fastsession-0.1.2/FastSession.egg-info/SOURCES.txt` & `fastsession-0.2.0/FastSession.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastsession-0.1.2/LICENSE` & `fastsession-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastsession-0.1.2/PKG-INFO` & `fastsession-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastsession
-Version: 0.1.2
+Version: 0.2.0
 Summary: A session middleware for Starlette and FastAPI
 Home-page: https://github.com/riversun/FastSession
 Author: Tom Misawa
 Author-email: riversun.org@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,14 +13,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # FastSession
 
+[English](https://github.com/riversun/FastSession/blob/main/README.md) | [&#26085;&#26412;&#35486;](https://github.com/riversun/FastSession/blob/main/README_ja.md)
+
 FastSession is a session management library for FastAPI. 
 
 It provides a middleware, `FastSessionMiddleware`, 
 that helps you manage user sessions effectively in your FastAPI applications.
 
 ## Features
```

### Comparing `fastsession-0.1.2/README.md` & `fastsession-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # FastSession
 
+[English](https://github.com/riversun/FastSession/blob/main/README.md) | [&#26085;&#26412;&#35486;](https://github.com/riversun/FastSession/blob/main/README_ja.md)
+
 FastSession is a session management library for FastAPI. 
 
 It provides a middleware, `FastSessionMiddleware`, 
 that helps you manage user sessions effectively in your FastAPI applications.
 
 ## Features
```

### Comparing `fastsession-0.1.2/fastsession/fast_session_middleware.py` & `fastsession-0.2.0/fastsession/fast_session_middleware.py`

 * *Files 22% similar despite different names*

```diff
@@ -28,189 +28,251 @@
         self.session_save()
         pass
 
 
 class FastSessionMiddleware(BaseHTTPMiddleware):
     """
     A FastAPI middleware for managing user sessions.
-    FastAPIのユーザーセッションを管理するためのミドルウェア。
     """
 
+    # FastAPIのユーザーセッションを管理するためのミドルウェア。
+
     def __init__(self, app,
                  secret_key,  # クッキー署名用のキー
-                 store=MemoryStore,  # セッション保存用ストア
+                 store=MemoryStore(),  # セッション保存用ストア
                  http_only=True,  # True: CookieがJavaScriptなどのクライアントサイドのスクリプトからアクセス不可となる
                  secure=True,  # True: Https が必要
                  max_age=0,  # 0を指定すると、ブラウザを起動しているときのみ有効。0より大きな値を指定するとブラウザを閉じても有効時間内はセッションが継続される
                  session_cookie="sid",  # セッションクッキーの名前
                  session_object="session",  # request.state以下にぶるさげるSessionオブジェクトの属性名
+                 skip_session_header=None,
                  logger=None):
-        """
-        Initialize FastSessionMiddleware.
-        FastSessionMiddlewareを初期化する。
-        """
+
         super().__init__(app)
 
+        self.skip_session_header = skip_session_header  # like [{"header_name":"X-FastSession-Skip", "header_value":"skip"}]
         self.http_only = http_only
         self.max_age = max_age
         self.secure = secure
         self.secret_key = secret_key
         self.session_cookie_name = session_cookie
         self.session_store = store
         self.serializer = TimedSignatureSerializer(self.secret_key, expired_in=self.max_age)
         self.session_object = session_object
         self.logger = logger
 
-    def logi(self, message: str):
-        if self.logger is not None:
-            self.logger.info(message)
+        if self.logger is None:
+            class ConsoleLogger:
+                def info(self, str):
+                    #print(f"[INFO ]{str}")
+                    pass
+
+                def debug(self, str):
+                    #print(f"[DEBUG]{str}")
+                    pass
+
+            self.logger = ConsoleLogger()
+
+        self.logger.debug(f"xxxxx")
+        self.logger.debug(
+            f"FastSession initialized http_only:{http_only} secure:{secure} session_key:'{session_object}' session_cookie_name:{session_cookie} store:{store}")
 
     def create_session_cookie(self, session_id):
         """
         Create and sign a session cookie.
-        セッションキーを署名してクッキーに保存。
         """
+
+        # セッションID に署名してクッキーオブジェクトに保存する
+
+        # たとえば、セッションクッキーの名前が "session" とするとき、
+        # 　{"session":セッションID} な　「セッションID入り辞書オブジェクト」 を作り、
+        # その　セッションID入り辞書オブジェクトに対して署名を行う
         session_id_dict_obj = {self.session_cookie_name: session_id}
+
+        # 「セッションID入り辞書オブジェクト」 に署名をしたものは「署名済セッションID文字列」と呼ぶこととする。
+        # 辞書オブジェクトがシリアライズされてるので「署名済セッションID入り辞書オブジェクト」ではなく「署名済セッションID文字列」とする。
         signed_session_id = self.serializer.encode(session_id_dict_obj)  # ser.dumps({'session_id': session_id})
 
         cookie = SimpleCookie()
+
+        # クッキーオブジェクトにキーを "session" として、今署名済の　「署名済セッションID文字列」　を格納する
         cookie[self.session_cookie_name] = signed_session_id
 
+        self.logger.debug(f"[session_id:'{session_id}'] Creating new Cookie object... cookie[{self.session_cookie_name}]")
+
         if self.http_only:
+            self.logger.debug(f"[session_id:'{session_id}'] cookie[{self.session_cookie_name}]['httponly'] enabled")
+
             cookie[self.session_cookie_name]["httponly"] = True  # Set the HTTP-only flag. HTTP-onlyフラグを設定
 
         if self.secure:
+            self.logger.debug(f"[session_id:'{session_id}'] cookie[{self.session_cookie_name}]['secure'] enabled")
             cookie[self.session_cookie_name]["secure"] = True  # Set the Secure flag. Secure フラグを設定
 
         if self.max_age > 0:
+            self.logger.debug(f"[session_id:'{session_id}'] cookie[{self.session_cookie_name}]['maxage']={self.max_age} enabled")
             cookie[self.session_cookie_name][
-                "max-age"] = self.max_age  # Set the Max-Age attribute. Max-Age 属性を設定（この例では1時間）
+                "max-age"] = self.max_age  # Max-Age 属性を設定（この例では1時間）
             # cookie[self.session_cookie_name]["max-age"] = 60 * 60 * 24 * 365 * 100  # 100 years for example
 
         return cookie
 
+    def should_skip_session_management_by_checking_header(self, request: Request) -> bool:
+        """
+        リクエストヘッダーをチェックしてセッション処理をスキップするか否かを返す
+        :param request:
+        :return:
+        """
+        skip_header = self.skip_session_header
+
+        if skip_header is None:
+            self.logger.debug(f"Don't use skip_header")
+            return False
+
+        if isinstance(skip_header, dict):  # 辞書の場合はリストに変換
+            skip_header = [skip_header]
+
+        header_names = []
+
+        for header in skip_header:
+            header_name = header.get('header_name')
+            header_value = header.get('header_value')
+            header_names.append(header_name)
+
+            self.logger.debug(f"Use skip_header option. skip_header:'{header_name}':'{header_value}'")
+
+            # request.headers は Headers オブジェクトで、ヘッダー名は大文字、小文字どちらで指定してもよい(RFC上はヘッダーは大文字、小文字を区別しない)
+            request_header_value = request.headers.get(header_name)
+            self.logger.debug(f"Use skip_header option. Checking request header: '{header_name}':'{request_header_value}'")
+
+            # header_valueが"*"の場合、header_nameが存在するか確認
+            # またはrequest_header_valueがheader_valueと一致する場合
+            if (header_value == "*" and request_header_value is not None) or request_header_value == header_value:
+                self.logger.debug(f"Use skip_header option. skip_header matched!")
+                return True
+
+        self.logger.debug(f"Use skip_header option. skip_headers:{header_names} not matched in request headers.")
+        return False
+
     async def dispatch(self, request: Request, call_next: RequestResponseEndpoint) -> Response:
         """
         Dispatch the request, handling session management.
-        リクエストをディスパッチし、セッション管理を行う。
         """
 
-        # Get session key from cookies. クッキーからセッションキーを取得
+        # スキップすべきかどうか判定
+        if self.should_skip_session_management_by_checking_header(request):
+            # ある特定のヘッダと値のペアが含まれていたら、スキップする
+            self.logger.debug(f"Skip session management.")
+            response = await call_next(request)
+            return response
+
+        # リクエストをディスパッチし、セッション管理を行う。
+        # クライアントからのリクエストに含まれるクッキーから
+        # 「署名済セッションID文字列」を取得する
         signed_session_id = request.cookies.get(self.session_cookie_name)
 
         cookie = None
+
         if signed_session_id is None:
-            # No session cookie, completely new access.
-            # => Generate a new session.
             # セッションクッキーが無い完全新規アクセス
             # => セッションの新規生成
-            self.logi(f"Completely new access with no session cookies")
+            self.logger.info(f"Completely new access with no session cookies")
+
+            # セッションID に署名してクッキーオブジェクトに保存する。
+            # また request.state 以下にセッションマネージャをぶるさげてセッションの入出力ができるようにする
             cookie = await self.create_new_session_id_and_store(request, cause="new")
 
         else:
-            # Access with session cookie. セッションクッキーがある状態でアクセス
+            # セッションクッキーがある状態でアクセス
+
+            # 「署名済セッションID文字列」をデコードして「セッションID入り辞書オブジェクト」を得る
             decoded_dict, err = self.serializer.decode(signed_session_id)
 
             if decoded_dict is not None:
-                #
-                # Cookie signature verification succeeded.
-                # クッキー署名検証に成功
+
+                # - クッキー署名検証に成功したとき
+                self.logger.debug(f"Cookie signature validation success")
+                # 「セッションID入り辞書オブジェクト」から セッションID を取得する
                 session_id = decoded_dict.get(self.session_cookie_name)
                 session_store = self.session_store.get_store(session_id)
 
                 if session_store is None:
-                    # The session cookie is correct and the session ID decoded from it is also normal.
-                    # However, the session store linked to the session ID could not be properly retrieved.
-                    # This happens when the server is restarted and the in-memory store is lost,
-                    # but the session cookie remains in the user's browser.
-                    # => Regenerate the session ID and the store.
-
                     # 正しい署名のクッキーがあり、そこからデコードしたセッションIDも正常
                     # だがセッションIDにひもづいたセッションストアが正しく取得できなかった
                     # こうなる原因はサーバーを再起動しオンメモリのストアが消えたがユーザーの
                     # ブラウザにセッションクッキーが残っている場合
                     # => セッションIDを再生成し、ストアを再生成する
 
-                    self.logi(f"Session cookies available. No store.")
+                    self.logger.info(f"[session_id:'{session_id}'] Session cookie available. But no store for this sessionId found. Maybe store had cleaned.")
                     cookie = await self.create_new_session_id_and_store(request, cause="valid_cookie_but_no_store")
-                    # request.state.session["__cause__"] =
+
                 else:
-                    # The session cookie is correct, the session ID decoded from it is also normal,
-                    # and the session store linked to the session ID was properly retrieved.
 
                     # 正しい署名のクッキーがあり、そこからデコードしたセッションIDも正常
                     # かつセッションIDにひもづいたセッションストアが正しく取得できた
-                    self.logi(f"Session cookies,Store available.")
+                    self.logger.info(f"[session_id:'{session_id}'] Session cookie and Store is available! set session_mgr to reqeust.state.{self.session_object}")
 
                     setattr(request.state,
                             self.session_object,
                             FastSession(
                                 store=session_store,
                                 session_id=session_id,
                                 session_save=lambda: self.session_store.save_store(session_id))
                             )
 
-                    # request.state.session_save = lambda: self.session_store.save_store(session_id)
                     session_store["__cause__"] = "success"
 
             else:
-                # Cookie signature verification failed.
-                # Signature verification of the session id failed due to some reason.
-                # Reason 1: Tampering with the session id.
-                # Reason 2: Expired.
-                # => Delete the storage for the old session ID.
-                # => Generate a new session.
-
                 # クッキーの署名検証に失敗
                 # 理由１　セッションidの改ざん
                 # 理由２　有効期限切れ
                 # => 旧セッションID用のストレージを削除する
                 # => 新たにセッションを生成
-                self.logi(f"Session cookies available. Verification failed! err:{err}")
+                self.logger.info(f"Session cookies available but verification failed! err:{err}")
 
                 if err == "SignatureExpired":
-                    # In case the session has expired.
-                    # セッションの有効期限が
-                    # Expired. セッションの有効期限が切れていた場合
+                    # セッションの有効期限が切れていた場合
                     pass
 
                 cookie = await self.create_new_session_id_and_store(request, cause=f"renew after {err}")
 
         response = await call_next(request)
 
-        # From here, processing for the response side.
         # ここから response 側の処理
         if cookie is not None:
-            # If there is a cookie to be set.
-            # => Set a cookie that encodes the session_id.
-
-            # セットすべきクッキーがある場合
+            # - セットすべきクッキーがあるとき
             # => session_id をエンコードしたクッキーをセットする
+
             cookie_val = cookie.output(header="").strip()
-            response.headers["Set-Cookie"] = cookie_val
+            self.logger.info(f"Set response header 'Set-Cookie' to signed cookie value")
+            response.headers["Set-Cookie"] = cookie_val  # レスポンスヘッダにセッションID署名済データが入ったクッキーをセットし、クライアント側に反映する
 
         return response
 
     async def create_new_session_id_and_store(self, request, cause=None):
         """
         Create a new session ID and its corresponding store.
-        新しいセッションIDとそのストアを生成する。
         """
+
+        # セッションID に署名してクッキーオブジェクトに保存する。また request.state 以下にセッションマネージャをぶるさげてセッションの入出力ができるようにする
         session_id = str(uuid.uuid4())
+
         session_store = self.session_store.create_store(session_id)
+        self.logger.debug(f"[session_id:'{session_id}'(NEW)] New session_id and store for session_id created.")
 
         if cause is not None:
             session_store["__cause__"] = cause  # セッションが新規生成された理由を格納
 
+
         fast_session_obj = FastSession(
             store=session_store,
             session_id=session_id,
             session_save=lambda: self.session_store.save_store(session_id)
         )
-
+        self.logger.info(f"[session_id:'{session_id}'(NEW)] Set session_mgr to request.state.{self.session_object} ")
         # request.state に self.session_object に指定された属性名で FastSessionオブジェクトをぶらさげる
         setattr(request.state,
                 self.session_object,
                 fast_session_obj)
 
         self.session_store.gc()  # たまったストアのクリーンアップをトライする
```

### Comparing `fastsession-0.1.2/fastsession/memory_store.py` & `fastsession-0.2.0/fastsession/memory_store.py`

 * *Files identical despite different names*

### Comparing `fastsession-0.1.2/fastsession/timed_signature_serializer.py` & `fastsession-0.2.0/fastsession/timed_signature_serializer.py`

 * *Files identical despite different names*

### Comparing `fastsession-0.1.2/setup.py` & `fastsession-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fastsession",
-    version="0.1.2",
+    version="0.2.0",
     author="Tom Misawa",
     author_email="riversun.org@gmail.com",
     description="A session middleware for Starlette and FastAPI",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/riversun/FastSession",
     packages=find_packages(exclude=["tests.*", "tests", "examples.*", "examples"]),
-    tests_require=["pytest", "httpx"],
+    tests_require=["pytest", "pytest-asyncio", "httpx"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

### Comparing `fastsession-0.1.2/tests/test_session_middleware.py` & `fastsession-0.2.0/tests/test_session_middleware.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,17 @@
+import pytest
+from unittest.mock import Mock
+
 from starlette.testclient import TestClient
 from starlette.applications import Starlette
 from starlette.responses import PlainTextResponse
 from starlette.routing import Route
 from fastsession.fast_session_middleware import FastSessionMiddleware, MemoryStore
+from starlette.requests import Request
+from starlette.responses import Response
 
 
 def test_create_session_id_and_store():
     """
     Test session ID creation and store operation.
 
     テストセッションIDの作成とストア操作
@@ -86,14 +91,15 @@
     response = client.get("/")
     assert response.status_code == 200
     assert "Counter: 3" in response.text
 
 
 import time
 
+
 def test_session_cookie_expiry():
     """
     Test that the session cookie expires after the max_age limit (1 second in this case).
 
     セッションクッキーがmax_age（この場合は1秒）の制限後に期限切れになることをテストします。
     """
 
@@ -194,15 +200,15 @@
         return PlainTextResponse(f"Counter: {session['test_counter']}")
 
     # アプリケーションの作成とミドルウェアの追加
     app = Starlette()
     app.add_route("/", test_route)
 
     is_cookie_secure = False  # テスト用途なので False にする
-    is_http_only=True #  HttpOnly を付与する
+    is_http_only = True  # HttpOnly を付与する
     app.add_middleware(FastSessionMiddleware,
                        secret_key='test-secret',
                        store=MemoryStore(),  # Use the same memory store
                        http_only=is_http_only,
                        max_age=3600,
                        secure=is_cookie_secure,
                        session_cookie="sid"
@@ -250,7 +256,68 @@
 
     # テストクライアントの作成
     client = TestClient(app)
 
     # First request
     response = client.get("/")
     assert 'HttpOnly' not in response.headers['Set-Cookie']
+
+@pytest.mark.asyncio
+async def test_dispatch_should_skip_session_management_with_skip_header():
+    app = Mock(return_value=Response("OK"))  # モックのASGIアプリケーションを作成します
+    middleware = FastSessionMiddleware(
+        app=app,
+        secret_key="test",
+        skip_session_header={"header_name": "X-FastSession-Skip", "header_value": "skip"}
+    )
+
+    # Starlette の Request オブジェクトを(UTなどの目的で)自前で生成するときは、
+    # (1) ヘッダーを　小文字にした、タプルで指定する
+    # (2) バイト文字列（b""） で指定する
+    headers = [(b"x-fastsession-skip", b"skip")]
+    request = Request(scope={"type": "http", "headers": headers}, receive=None)
+
+    # headers = [(b"X-FastSession-Skip", b"skip")]
+    # request = Request(scope={"type": "http", "headers": headers}, receive=None)
+
+    class MockResponse:
+        def __init__(self):
+            self.headers = {}
+
+    emulated_response=MockResponse()
+
+    async def call_next(request):
+        return emulated_response
+
+    response = await middleware.dispatch(request,call_next)
+    print(f"res:{response}")
+    assert not hasattr(request.state, 'session')  # request.stateにsession属性が存在しないことを確認します
+
+
+@pytest.mark.asyncio
+async def test_dispatch_should_not_skip_session_management_without_skip_heade1r():
+    # スキップヘッダが存在しないとき、appが直接呼び出されないことを確認します
+    app = Mock(return_value=Response("OK"))  # モックのASGIアプリケーションを作成します
+    middleware = FastSessionMiddleware(
+        app=app,
+        secret_key="test",
+        skip_session_header={"header_name": "X-FastSession-Skip", "header_value": "skip"}
+    )
+
+    headers = [(b"ignore", b"ignore")]
+    request = Request(scope={"type": "http", "headers": headers}, receive=None)
+
+    # headers = [(b"X-FastSession-Skip", b"skip")]
+    # request = Request(scope={"type": "http", "headers": headers}, receive=None)
+
+    class MockResponse:
+        def __init__(self):
+            self.headers = {}
+
+    emulated_response = MockResponse()
+
+    async def call_next(request):
+        return emulated_response
+
+    response = await middleware.dispatch(request, call_next)
+    print(f"res:{response}")
+    assert hasattr(request.state, 'session')  # request.stateにsession属性が存在することを確認します
```

### Comparing `fastsession-0.1.2/tests/test_store_memory.py` & `fastsession-0.2.0/tests/test_store_memory.py`

 * *Files identical despite different names*

### Comparing `fastsession-0.1.2/tests/test_timed_signature_serializer.py` & `fastsession-0.2.0/tests/test_timed_signature_serializer.py`

 * *Files identical despite different names*

