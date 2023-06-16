# Comparing `tmp/rouver-2.6.1.tar.gz` & `tmp/rouver-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rouver-2.6.1.tar", max compression
+gzip compressed data, was "rouver-2.6.2.tar", max compression
```

## Comparing `rouver-2.6.1.tar` & `rouver-2.6.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1083 2019-04-08 18:12:19.695481 rouver-2.6.1/LICENSE
--rw-r--r--   0        0        0     2575 2019-11-05 14:50:38.760380 rouver-2.6.1/README.md
--rw-r--r--   0        0        0     1245 2023-03-15 12:51:42.502985 rouver-2.6.1/pyproject.toml
--rw-r--r--   0        0        0       61 2021-04-08 13:08:50.841638 rouver-2.6.1/rouver/__init__.py
--rw-r--r--   0        0        0    14780 2021-04-08 13:11:03.767927 rouver-2.6.1/rouver/args.py
--rw-r--r--   0        0        0      666 2019-04-08 18:12:19.695481 rouver-2.6.1/rouver/exceptions.py
--rw-r--r--   0        0        0     5989 2023-01-18 15:58:36.236448 rouver-2.6.1/rouver/handler.py
--rw-r--r--   0        0        0     2508 2019-12-13 13:44:09.153088 rouver-2.6.1/rouver/html.py
--rw-r--r--   0        0        0        0 2019-04-08 18:12:19.695481 rouver-2.6.1/rouver/py.typed
--rw-r--r--   0        0        0     5944 2021-04-08 13:14:02.919414 rouver-2.6.1/rouver/response.py
--rw-r--r--   0        0        0    14229 2023-03-15 12:47:26.347317 rouver-2.6.1/rouver/router.py
--rw-r--r--   0        0        0      123 2019-04-08 18:12:19.695481 rouver-2.6.1/rouver/status.py
--rw-r--r--   0        0        0    20201 2023-03-15 12:13:42.717304 rouver-2.6.1/rouver/test.py
--rw-r--r--   0        0        0      900 2022-05-25 13:35:06.266733 rouver-2.6.1/rouver/types.py
--rw-r--r--   0        0        0      599 2022-08-26 14:32:42.352766 rouver-2.6.1/rouver/util.py
--rw-r--r--   0        0        0        0 2019-04-08 18:12:19.695481 rouver-2.6.1/rouver_test/__init__.py
--rw-r--r--   0        0        0    18462 2021-04-08 13:19:48.050997 rouver-2.6.1/rouver_test/args.py
--rw-r--r--   0        0        0      456 2019-12-13 13:44:09.153088 rouver-2.6.1/rouver_test/exceptions.py
--rw-r--r--   0        0        0     6955 2023-01-18 15:57:30.703255 rouver-2.6.1/rouver_test/handler.py
--rw-r--r--   0        0        0     4989 2019-12-13 13:44:09.153088 rouver-2.6.1/rouver_test/html.py
--rw-r--r--   0        0        0    16693 2022-01-31 12:47:31.971807 rouver-2.6.1/rouver_test/response.py
--rw-r--r--   0        0        0    27781 2023-03-15 12:43:51.996698 rouver-2.6.1/rouver_test/router.py
--rw-r--r--   0        0        0      306 2019-12-13 13:44:09.153088 rouver-2.6.1/rouver_test/status.py
--rw-r--r--   0        0        0    36059 2023-03-15 12:13:47.965455 rouver-2.6.1/rouver_test/test.py
--rw-r--r--   0        0        0     2844 2023-02-01 10:15:22.893154 rouver-2.6.1/rouver_test/testutil.py
--rw-r--r--   0        0        0     1836 2020-03-12 14:50:04.877825 rouver-2.6.1/rouver_test/util.py
--rw-r--r--   0        0        0     3380 1970-01-01 00:00:00.000000 rouver-2.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2019-04-08 18:12:19.695481 rouver-2.6.2/LICENSE
+-rw-r--r--   0        0        0     2575 2019-11-05 14:50:38.760380 rouver-2.6.2/README.md
+-rw-r--r--   0        0        0     1442 2023-06-16 10:45:54.406183 rouver-2.6.2/pyproject.toml
+-rw-r--r--   0        0        0       61 2021-04-08 13:08:50.841638 rouver-2.6.2/rouver/__init__.py
+-rw-r--r--   0        0        0    14780 2023-04-27 14:05:55.648409 rouver-2.6.2/rouver/args.py
+-rw-r--r--   0        0        0      666 2019-04-08 18:12:19.695481 rouver-2.6.2/rouver/exceptions.py
+-rw-r--r--   0        0        0     5989 2023-01-18 15:58:36.236448 rouver-2.6.2/rouver/handler.py
+-rw-r--r--   0        0        0     2508 2019-12-13 13:44:09.153088 rouver-2.6.2/rouver/html.py
+-rw-r--r--   0        0        0        0 2019-04-08 18:12:19.695481 rouver-2.6.2/rouver/py.typed
+-rw-r--r--   0        0        0     5944 2021-04-08 13:14:02.919414 rouver-2.6.2/rouver/response.py
+-rw-r--r--   0        0        0    14229 2023-03-15 12:47:26.347317 rouver-2.6.2/rouver/router.py
+-rw-r--r--   0        0        0      123 2019-04-08 18:12:19.695481 rouver-2.6.2/rouver/status.py
+-rw-r--r--   0        0        0    20195 2023-06-16 10:25:59.018156 rouver-2.6.2/rouver/test.py
+-rw-r--r--   0        0        0      900 2022-05-25 13:35:06.266733 rouver-2.6.2/rouver/types.py
+-rw-r--r--   0        0        0     1491 2023-06-16 10:22:47.631525 rouver-2.6.2/rouver/util.py
+-rw-r--r--   0        0        0        0 2019-04-08 18:12:19.695481 rouver-2.6.2/rouver_test/__init__.py
+-rw-r--r--   0        0        0    18572 2023-06-16 10:01:17.548263 rouver-2.6.2/rouver_test/args.py
+-rw-r--r--   0        0        0      456 2019-12-13 13:44:09.153088 rouver-2.6.2/rouver_test/exceptions.py
+-rw-r--r--   0        0        0     6955 2023-01-18 15:57:30.703255 rouver-2.6.2/rouver_test/handler.py
+-rw-r--r--   0        0        0     4989 2019-12-13 13:44:09.153088 rouver-2.6.2/rouver_test/html.py
+-rw-r--r--   0        0        0    16693 2022-01-31 12:47:31.971807 rouver-2.6.2/rouver_test/response.py
+-rw-r--r--   0        0        0    27781 2023-03-15 12:43:51.996698 rouver-2.6.2/rouver_test/router.py
+-rw-r--r--   0        0        0      306 2019-12-13 13:44:09.153088 rouver-2.6.2/rouver_test/status.py
+-rw-r--r--   0        0        0    36048 2023-06-16 10:29:20.104700 rouver-2.6.2/rouver_test/test.py
+-rw-r--r--   0        0        0     2844 2023-02-01 10:15:22.893154 rouver-2.6.2/rouver_test/testutil.py
+-rw-r--r--   0        0        0     2070 2023-06-16 10:23:24.120827 rouver-2.6.2/rouver_test/util.py
+-rw-r--r--   0        0        0     3581 1970-01-01 00:00:00.000000 rouver-2.6.2/PKG-INFO
```

### Comparing `rouver-2.6.1/LICENSE` & `rouver-2.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rouver-2.6.1/README.md` & `rouver-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `rouver-2.6.1/pyproject.toml` & `rouver-2.6.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 [tool.poetry]
 name = "rouver"
-version = "2.6.1"
+version = "2.6.2"
 description = "A microframework"
 readme = "README.md"
 authors = ["Sebastian Rittau <srittau@rittau.biz>"]
 license = "MIT"
 homepage = "https://github.com/srittau/rouver"
 repository = "https://github.com/srittau/rouver"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Topic :: Internet :: WWW/HTTP :: WSGI",
 ]
 packages = [{ include = "rouver" }, { include = "rouver_test" }]
 include = ["*/py.typed"]
 
+[tool.poetry.urls]
+"GitHub" = "https://github.com/srittau/rouver"
+"Bug Tracker" = "https://github.com/srittau/rouver/issues"
+"Changes" = "https://github.com/srittau/rouver/blob/main/CHANGELOG.md"
+
 [tool.poetry.dependencies]
 python = "^3.9"
 dectest = "^1.0.0"
 werkzeug = "^2.0"
 typing-extensions = "^4.1.1"
 
 [tool.poetry.dev-dependencies]
 asserts = ">=0.10.0,<0.13"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 isort = "^5.11.4"
-mypy = "~1.1.1"
+mypy = "~1.3.0"
 pytest = ">=6.2.5, <8"
 
 [tool.black]
 line-length = 79
 target-version = ["py39"]
 
 [tool.isort]
```

### Comparing `rouver-2.6.1/rouver/args.py` & `rouver-2.6.2/rouver/args.py`

 * *Files identical despite different names*

### Comparing `rouver-2.6.1/rouver/exceptions.py` & `rouver-2.6.2/rouver/exceptions.py`

 * *Files identical despite different names*

### Comparing `rouver-2.6.1/rouver/handler.py` & `rouver-2.6.2/rouver/handler.py`

 * *Files identical despite different names*

### Comparing `rouver-2.6.1/rouver/html.py` & `rouver-2.6.2/rouver/html.py`

 * *Files identical despite different names*

### Comparing `rouver-2.6.1/rouver/response.py` & `rouver-2.6.2/rouver/response.py`

 * *Files identical despite different names*

### Comparing `rouver-2.6.1/rouver/router.py` & `rouver-2.6.2/rouver/router.py`

 * *Files identical despite different names*

### Comparing `rouver-2.6.1/rouver/test.py` & `rouver-2.6.2/rouver/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from dectest import TestCase, before
 from werkzeug.http import parse_options_header
 
 from rouver.args import Multiplicity
 from rouver.router import Router
 from rouver.types import Header, WSGIApplication, WSGIEnvironment
+from rouver.util import rfc5987_encode
 
 _STATUS_RE = re.compile(r"^(\d\d\d) [ -~]+$")
 
 
 class TestRequest:
     def __init__(self, method: str, path: str) -> None:
         self.method = method.upper()
@@ -201,17 +202,15 @@
         for name, content, content_type, filename in self._file_arguments:
             body += b"--" + boundary.encode("ascii") + b"\r\n"
             body += (
                 b'Content-Disposition: form-data; name="'
                 + quote_plus(name).encode("ascii")
             ) + b'"; '
             if filename:
-                body += b"filename*=UTF-8''" + quote_plus(filename).encode(
-                    "ascii"
-                )
+                body += rfc5987_encode("filename", filename).encode("ascii")
             else:
                 body += b'filename=""'
             body += b"\r\n"
             body += b"Content-Type: " + content_type.encode("ascii") + b"\r\n"
             body += (
                 b"Content-Length: "
                 + str(len(content)).encode("ascii")
```

### Comparing `rouver-2.6.1/rouver/types.py` & `rouver-2.6.2/rouver/types.py`

 * *Files identical despite different names*

### Comparing `rouver-2.6.1/rouver_test/args.py` & `rouver-2.6.2/rouver_test/args.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,24 +13,25 @@
     fail,
 )
 from dectest import TestCase, before, test
 from werkzeug.exceptions import BadRequest
 
 from rouver.args import ArgumentParser, Multiplicity, parse_args
 from rouver.exceptions import ArgumentsError
+from rouver.util import rfc5987_encode
 from rouver_test.testutil import default_environment
 
 MULTIPART_PART_TMPL = """--1234567890
 Content-Disposition: form-data; name="{name}"
 
 {value}
 """
 
 MULTIPART_FILE_BODY_TMPL = """--1234567890
-Content-Disposition: form-data; name="{name}"; filename={filename}
+Content-Disposition: form-data; name="{name}"; {filename_param}
 Content-Type: {type}
 
 {content}
 --1234567890--
 """
 
 
@@ -74,17 +75,18 @@
         self.env["CONTENT_LENGTH"] = str(len(body))
         self.env["wsgi.input"] = BytesIO(body)
 
     def setup_multipart_file_request(
         self, name: str, filename: str, file_content: str, content_type: str
     ) -> None:
         self.env["CONTENT_TYPE"] = "multipart/form-data; boundary=1234567890"
+        filename_param = rfc5987_encode("filename", filename)
         body = MULTIPART_FILE_BODY_TMPL.format(
             name=name,
-            filename=filename,
+            filename_param=filename_param,
             content=file_content,
             type=content_type,
         ).encode("utf-8")
         self.env["CONTENT_LENGTH"] = str(len(body))
         self.env["wsgi.input"] = BytesIO(body)
 
     @test
```

### Comparing `rouver-2.6.1/rouver_test/handler.py` & `rouver-2.6.2/rouver_test/handler.py`

 * *Files identical despite different names*

### Comparing `rouver-2.6.1/rouver_test/html.py` & `rouver-2.6.2/rouver_test/html.py`

 * *Files identical despite different names*

### Comparing `rouver-2.6.1/rouver_test/response.py` & `rouver-2.6.2/rouver_test/response.py`

 * *Files identical despite different names*

### Comparing `rouver-2.6.1/rouver_test/router.py` & `rouver-2.6.2/rouver_test/router.py`

 * *Files identical despite different names*

### Comparing `rouver-2.6.1/rouver_test/test.py` & `rouver-2.6.2/rouver_test/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,21 +252,21 @@
         request = create_request("PUT", "/foo")
         request.add_argument('f"öo', "bär")
         request.add_file_argument(
             'f"öle', b"", "text/plain", filename="ä\"'bc"
         )
         environ = request.to_environment()
         assert "QUERY_STRING" not in environ
-        content_type, boundary = environ["CONTENT_TYPE"].split(";")
+        content_type, _ = environ["CONTENT_TYPE"].split(";")
         assert content_type == "multipart/form-data"
         _, args, files = parse_form_data(environ)
         assert len(args) == 1
-        assert "bär" == args["f%22%C3%B6o"]
+        assert "bär" == args['f"%C3%B6o']
         assert len(files) == 1
-        file = files["f%22%C3%B6le"]
+        file = files['f"%C3%B6le']
         assert file.mimetype == "text/plain"
         assert file.filename == "ä\"'bc"
         assert file.stream.read() == b""
 
     def test_clear_arguments(self) -> None:
         request = create_request("GET", "/foo")
         request.add_argument("foo", "bar")
```

### Comparing `rouver-2.6.1/rouver_test/testutil.py` & `rouver-2.6.2/rouver_test/testutil.py`

 * *Files identical despite different names*

### Comparing `rouver-2.6.1/rouver_test/util.py` & `rouver-2.6.2/rouver_test/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,65 @@
-from asserts import assert_equal
-from dectest import TestCase, test
+import pytest
 from werkzeug import Request
 
-from rouver.util import absolute_url
+from rouver.util import absolute_url, rfc5987_encode
 
 
-class AbsoluteURLTest(TestCase):
+class TestAbsoluteURL:
     @staticmethod
     def _create_request(*, path_info: str = "/path") -> Request:
         return Request(
             {
                 "wsgi.url_scheme": "https",
                 "SERVER_NAME": "example.com",
                 "SERVER_PORT": "443",
                 "SCRIPT_NAME": "/base/",
                 "PATH_INFO": path_info,
             }
         )
 
-    @test
-    def path_is_not_ascii(self) -> None:
+    def test_path_is_not_ascii(self) -> None:
         request = self._create_request()
-        url = absolute_url(request, "/~föo")
-        assert_equal("https://example.com/~f%C3%B6o", url)
+        assert (
+            absolute_url(request, "/~föo") == "https://example.com/~f%C3%B6o"
+        )
 
-    @test
-    def path_is_absolute(self) -> None:
+    def test_path_is_absolute(self) -> None:
         request = self._create_request()
-        url = absolute_url(request, "https://example.org/foo")
-        assert_equal("https://example.org/foo", url)
+        assert (
+            absolute_url(request, "https://example.org/foo")
+            == "https://example.org/foo"
+        )
 
-    @test
-    def path_is_root_relative(self) -> None:
+    def test_path_is_root_relative(self) -> None:
         request = self._create_request()
-        url = absolute_url(request, "/foo")
-        assert_equal("https://example.com/foo", url)
+        assert absolute_url(request, "/foo") == "https://example.com/foo"
 
-    @test
-    def path_is_relative__base_with_slash(self) -> None:
+    def test_path_is_relative__base_with_slash(self) -> None:
         request = self._create_request(path_info="/path/")
-        url = absolute_url(request, "foo")
-        assert_equal("https://example.com/base/path/foo", url)
+        assert (
+            absolute_url(request, "foo") == "https://example.com/base/path/foo"
+        )
 
-    @test
-    def path_is_relative__base_without_slash(self) -> None:
+    def test_path_is_relative__base_without_slash(self) -> None:
         request = self._create_request(path_info="/path")
-        url = absolute_url(request, "foo")
-        assert_equal("https://example.com/base/foo", url)
+        assert absolute_url(request, "foo") == "https://example.com/base/foo"
 
-    @test
-    def do_not_encode_special_characters(self) -> None:
+    def test_do_not_encode_special_characters(self) -> None:
         request = self._create_request()
-        url = absolute_url(request, "/foo?bar=baz&abc=%6A;+,@:$")
-        assert_equal("https://example.com/foo?bar=baz&abc=%6A;+,@:$", url)
+        assert (
+            absolute_url(request, "/foo?bar=baz&abc=%6A;+,@:$")
+            == "https://example.com/foo?bar=baz&abc=%6A;+,@:$"
+        )
+
+
+@pytest.mark.parametrize(
+    "string, encoded",
+    [
+        ("", "key="),
+        ("foo", "key=foo"),
+        ("foo bar\tbaz", 'key="foo bar\\\tbaz"'),
+        ("föo bar", "key*=UTF-8''f%C3%B6o%20bar"),
+    ],
+)
+def test_rfc5987_encode(string: str, encoded: str) -> None:
+    assert encoded == rfc5987_encode("key", string)
```

### Comparing `rouver-2.6.1/PKG-INFO` & `rouver-2.6.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rouver
-Version: 2.6.1
+Version: 2.6.2
 Summary: A microframework
 Home-page: https://github.com/srittau/rouver
 License: MIT
 Author: Sebastian Rittau
 Author-email: srittau@rittau.biz
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Requires-Dist: dectest (>=1.0.0,<2.0.0)
 Requires-Dist: typing-extensions (>=4.1.1,<5.0.0)
 Requires-Dist: werkzeug (>=2.0,<3.0)
+Project-URL: Bug Tracker, https://github.com/srittau/rouver/issues
+Project-URL: Changes, https://github.com/srittau/rouver/blob/main/CHANGELOG.md
+Project-URL: GitHub, https://github.com/srittau/rouver
 Project-URL: Repository, https://github.com/srittau/rouver
 Description-Content-Type: text/markdown
 
 # Rouver
 
 A microframework for Python 3, based on werkzeug.
```

