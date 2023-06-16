# Comparing `tmp/rug-0.8.tar.gz` & `tmp/rug-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rug-0.8.tar", max compression
+gzip compressed data, was "rug-0.8.1.tar", max compression
```

## Comparing `rug-0.8.tar` & `rug-0.8.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      775 2022-12-23 18:16:50.519949 rug-0.8/README.md
--rw-r--r--   0        0        0      851 2023-05-05 07:11:21.747804 rug-0.8/pyproject.toml
--rw-r--r--   0        0        0      288 2022-12-15 16:02:47.957044 rug-0.8/rug/__init__.py
--rw-r--r--   0        0        0     4266 2022-10-10 19:45:59.707606 rug-0.8/rug/alphaquery.py
--rw-r--r--   0        0        0     2688 2022-08-11 07:37:52.820634 rug-0.8/rug/barchart.py
--rw-r--r--   0        0        0     4641 2022-12-15 16:08:39.724843 rug-0.8/rug/base.py
--rw-r--r--   0        0        0     4150 2022-12-23 18:09:17.774153 rug-0.8/rug/etfdb.py
--rw-r--r--   0        0        0      683 2022-07-27 20:03:36.438856 rug-0.8/rug/exceptions.py
--rw-r--r--   0        0        0     3002 2023-04-05 05:45:36.800863 rug-0.8/rug/finviz.py
--rw-r--r--   0        0        0     1253 2022-12-12 10:12:35.894849 rug-0.8/rug/stockanalysis.py
--rw-r--r--   0        0        0     1947 2022-08-11 08:42:20.047418 rug-0.8/rug/stocktwits.py
--rw-r--r--   0        0        0     6910 2023-05-05 06:58:34.815386 rug-0.8/rug/tipranks.py
--rw-r--r--   0        0        0     4022 2022-08-11 08:43:03.063984 rug-0.8/rug/yahoo.py
--rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 rug-0.8/PKG-INFO
+-rw-r--r--   0        0        0      762 2023-06-16 06:42:16.417052 rug-0.8.1/README.md
+-rw-r--r--   0        0        0      853 2023-06-16 06:43:21.893792 rug-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      288 2022-12-15 16:02:47.957044 rug-0.8.1/rug/__init__.py
+-rw-r--r--   0        0        0     4266 2022-10-10 19:45:59.707606 rug-0.8.1/rug/alphaquery.py
+-rw-r--r--   0        0        0     2688 2022-08-11 07:37:52.820634 rug-0.8.1/rug/barchart.py
+-rw-r--r--   0        0        0     4997 2023-06-16 06:35:11.344249 rug-0.8.1/rug/base.py
+-rw-r--r--   0        0        0     4150 2022-12-23 18:09:17.774153 rug-0.8.1/rug/etfdb.py
+-rw-r--r--   0        0        0      683 2022-07-27 20:03:36.438856 rug-0.8.1/rug/exceptions.py
+-rw-r--r--   0        0        0     3038 2023-06-16 06:33:17.358960 rug-0.8.1/rug/finviz.py
+-rw-r--r--   0        0        0     1253 2022-12-12 10:12:35.894849 rug-0.8.1/rug/stockanalysis.py
+-rw-r--r--   0        0        0     1947 2022-08-11 08:42:20.047418 rug-0.8.1/rug/stocktwits.py
+-rw-r--r--   0        0        0     6910 2023-05-05 06:58:34.815386 rug-0.8.1/rug/tipranks.py
+-rw-r--r--   0        0        0     4021 2023-06-16 06:39:28.231152 rug-0.8.1/rug/yahoo.py
+-rw-r--r--   0        0        0     1764 1970-01-01 00:00:00.000000 rug-0.8.1/PKG-INFO
```

### Comparing `rug-0.8/README.md` & `rug-0.8.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -13,11 +13,8 @@
 Universal library for fetching Stock and ETF data from the internet - mostly unofficial
 APIs - no limits, more free data.
 
 (for Cryptocurrency alternative see [karpet](https://github.com/im-n1/karpet))
 
 * [PyPI](https://pypi.org/project/rug/)
 * [documentation](https://rug.readthedocs.io/en/latest/) ![Documentation Status](https://readthedocs.org/projects/rug/badge/?version=latest)
-
-## Changelog
-
-[changelog](./CHANGELOG.md)
+* [changelog](./CHANGELOG.md)
```

### Comparing `rug-0.8/pyproject.toml` & `rug-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rug"
-version = "0.8"
+version = "0.8.1"
 description = "Library for fetching various stock data from the internet (official and unofficial APIs)."
 authors = ["Pavel Hrdina"]
 classifiers = [
     "Programming Language :: Python :: 3.6",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
     "Intended Audience :: Developers",
```

### Comparing `rug-0.8/rug/alphaquery.py` & `rug-0.8.1/rug/alphaquery.py`

 * *Files identical despite different names*

### Comparing `rug-0.8/rug/barchart.py` & `rug-0.8.1/rug/barchart.py`

 * *Files identical despite different names*

### Comparing `rug-0.8/rug/base.py` & `rug-0.8.1/rug/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 import httpx
 
 from .exceptions import HttpException
 
 
 class BaseAPI:
-
     timeout = 10
     user_agent = (
         "Mozilla/5.0 (X11; Linux x86_64; rv:103.0) Gecko/20100101 Firefox/103.0"
     )
 
     def __init__(self, symbol=None):
         """
@@ -40,17 +39,15 @@
             ) from exc
 
         response.raise_for_status()
 
         return response
 
     async def _aget(self, *args):
-
         async with httpx.AsyncClient() as client:
-
             try:
                 response = await client.get(*args, timeout=self.timeout)
             except Exception as exc:
                 raise HttpException(
                     f"Couldn't perform GET request with args {args}"
                 ) from exc
 
@@ -62,27 +59,25 @@
 class Data(dict):
     """
     Dict substitution which recursivelly handles
     non-existing keys.
     """
 
     def __getitem__(self, key):
-
         try:
             data = super().__getitem__(key)
 
             # If the data is dict we need to wrap it with
             # this class so it will carry this logic.
             if type(data) == dict:
                 return self.__class__(data)
 
             # Data is not a dict so we return what we found.
             return data
         except:
-
             # In case of non existing key we return empty self
             # which makes sure another direct key demand will
             # copy this logic.
             return self.__class__()
 
 
 class HtmlTableParser(HTMLParser):
@@ -101,15 +96,14 @@
         """
 
         self.data = []
         self.columns = columns
         super().__init__(*args, **kwargs)
 
     def handle_data(self, data):
-
         if data := data.strip():
             self.data.append(self.parse_data(data))
 
     def parse_data(self, data):
         """
         Parses out all data from the given table and
         casts them into ``datetime.date`` or ``float``.
@@ -165,14 +159,26 @@
             data[1:],
             key=lambda row: row[0],
         )
         sorted_data.insert(0, data[0])
 
         return sorted_data
 
+    @staticmethod
+    def fix_empty_cells(html):
+        """
+        Fixes impty <td> cells and will them with "--"
+        which later gets recognized as 0.0 float.
+
+        :param str html: HTML table to be fixed.
+        :return: Fixed HTML.
+        :rtype: str
+        """
+        return re.sub(r"<td([^>]*)><\/td>", "<td$1>--</td>", html, flags=re.DOTALL)
+
 
 def strip_html_tags(text):
     """
     Removes HTML tags from the given string.
 
     :param str text: The string we want remove tags from.
     """
```

### Comparing `rug-0.8/rug/etfdb.py` & `rug-0.8.1/rug/etfdb.py`

 * *Files identical despite different names*

### Comparing `rug-0.8/rug/exceptions.py` & `rug-0.8.1/rug/exceptions.py`

 * *Files identical despite different names*

### Comparing `rug-0.8/rug/finviz.py` & `rug-0.8.1/rug/finviz.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,24 +32,25 @@
                 f"https://finviz.com/quote.ashx?t={self.symbol.upper()}&ty=c&ta=1&p=d",
                 headers={"User-Agent": self.user_agent},
             )
         except Exception as e:
             raise SymbolNotFound from e
 
         finds = re.findall(
-            r"<td[^>]*fullview-ratings-inner[^>]*>(<table[^>]*>(?:.+?)<\/table>)",
+            r"<table[^>]*fullview-ratings-outer[^>]*>(.+?)</table>",
             html.text,
             re.DOTALL,
         )
         rows = []
 
-        for find in finds:
+        if finds:
+            html = HtmlTableParser.fix_empty_cells(finds[0])
             parser = HtmlTableParser(columns=5)
-            parser.feed(find)
-            rows.extend(parser.get_data())
+            parser.feed(html)
+            rows = parser.get_data()[1:]
 
         return rows
 
     def get_insider_trading(self):
         """
         Fetches insiders transactions (if available) as a
         list with following fields:
```

### Comparing `rug-0.8/rug/stockanalysis.py` & `rug-0.8.1/rug/stockanalysis.py`

 * *Files identical despite different names*

### Comparing `rug-0.8/rug/stocktwits.py` & `rug-0.8.1/rug/stocktwits.py`

 * *Files identical despite different names*

### Comparing `rug-0.8/rug/tipranks.py` & `rug-0.8.1/rug/tipranks.py`

 * *Files identical despite different names*

### Comparing `rug-0.8/rug/yahoo.py` & `rug-0.8.1/rug/yahoo.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
             }
 
         :return: Current/Pre/Post market numbers (all are floats).
         :rtype: dict
         """
 
         def parse_state(state):
-
             # No state at all.
             if not state:
                 return None
 
             state = state.lower()
 
             if state.startswith("pre"):
```

### Comparing `rug-0.8/PKG-INFO` & `rug-0.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rug
-Version: 0.8
+Version: 0.8.1
 Summary: Library for fetching various stock data from the internet (official and unofficial APIs).
 Home-page: https://github.com/im-n1/rug
 License: MIT
 Author: Pavel Hrdina
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -37,12 +37,9 @@
 Universal library for fetching Stock and ETF data from the internet - mostly unofficial
 APIs - no limits, more free data.
 
 (for Cryptocurrency alternative see [karpet](https://github.com/im-n1/karpet))
 
 * [PyPI](https://pypi.org/project/rug/)
 * [documentation](https://rug.readthedocs.io/en/latest/) ![Documentation Status](https://readthedocs.org/projects/rug/badge/?version=latest)
-
-## Changelog
-
-[changelog](./CHANGELOG.md)
+* [changelog](./CHANGELOG.md)
```

