# Comparing `tmp/auto-screener-0.1.1.tar.gz` & `tmp/auto-screener-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-screener-0.1.1.tar", last modified: Thu Jun 15 21:24:22 2023, max compression
+gzip compressed data, was "auto-screener-0.1.2.tar", last modified: Fri Jun 16 12:15:57 2023, max compression
```

## Comparing `auto-screener-0.1.1.tar` & `auto-screener-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 21:24:22.309890 auto-screener-0.1.1/
--rw-rw-rw-   0        0        0       98 2023-06-15 21:24:22.000000 auto-screener-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2066 2023-06-15 21:24:22.308889 auto-screener-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1255 2023-04-21 09:27:54.000000 auto-screener-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 21:24:22.303930 auto-screener-0.1.1/auto_screener/
--rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 auto-screener-0.1.1/auto_screener/base.py
--rw-rw-rw-   0        0        0    17233 2023-06-15 21:24:06.000000 auto-screener-0.1.1/auto_screener/collect.py
--rw-rw-rw-   0        0        0    12082 2023-06-13 07:30:11.000000 auto-screener-0.1.1/auto_screener/dataset.py
--rw-rw-rw-   0        0        0      753 2023-06-06 19:23:53.000000 auto-screener-0.1.1/auto_screener/document.py
--rw-rw-rw-   0        0        0      194 2023-06-07 17:03:17.000000 auto-screener-0.1.1/auto_screener/exchanges.py
--rw-rw-rw-   0        0        0    25427 2023-06-15 15:04:45.000000 auto-screener-0.1.1/auto_screener/feed.py
--rw-rw-rw-   0        0        0      180 2023-04-21 16:51:56.000000 auto-screener-0.1.1/auto_screener/hints.py
--rw-rw-rw-   0        0        0     2665 2023-04-21 16:51:36.000000 auto-screener-0.1.1/auto_screener/interval.py
--rw-rw-rw-   0        0        0    26142 2023-06-15 15:32:24.000000 auto-screener-0.1.1/auto_screener/screener.py
--rw-rw-rw-   0        0        0    24728 2023-06-13 13:49:29.000000 auto-screener-0.1.1/auto_screener/screening.py
--rw-rw-rw-   0        0        0    10070 2023-06-15 16:44:13.000000 auto-screener-0.1.1/auto_screener/symbols.py
-drwxrwxrwx   0        0        0        0 2023-06-15 21:24:22.307881 auto-screener-0.1.1/auto_screener.egg-info/
--rw-rw-rw-   0        0        0     2066 2023-06-15 21:24:22.000000 auto-screener-0.1.1/auto_screener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2023-06-15 21:24:22.000000 auto-screener-0.1.1/auto_screener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 21:24:22.000000 auto-screener-0.1.1/auto_screener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-15 21:24:22.000000 auto-screener-0.1.1/auto_screener.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-15 21:24:22.000000 auto-screener-0.1.1/auto_screener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 auto-screener-0.1.1/build.py
--rw-rw-rw-   0        0        0      645 2023-06-15 21:24:22.000000 auto-screener-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       59 2023-05-24 20:12:53.000000 auto-screener-0.1.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       50 2023-05-24 19:47:16.000000 auto-screener-0.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 21:24:22.309890 auto-screener-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1564 2023-06-15 21:24:18.000000 auto-screener-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 12:15:57.382559 auto-screener-0.1.2/
+-rw-rw-rw-   0        0        0       98 2023-06-16 12:15:57.000000 auto-screener-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2066 2023-06-16 12:15:57.382559 auto-screener-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1255 2023-04-21 09:27:54.000000 auto-screener-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 12:15:57.377535 auto-screener-0.1.2/auto_screener/
+-rw-rw-rw-   0        0        0     6694 2023-03-18 20:51:39.000000 auto-screener-0.1.2/auto_screener/base.py
+-rw-rw-rw-   0        0        0    17233 2023-06-15 21:24:06.000000 auto-screener-0.1.2/auto_screener/collect.py
+-rw-rw-rw-   0        0        0    12082 2023-06-13 07:30:11.000000 auto-screener-0.1.2/auto_screener/dataset.py
+-rw-rw-rw-   0        0        0      753 2023-06-06 19:23:53.000000 auto-screener-0.1.2/auto_screener/document.py
+-rw-rw-rw-   0        0        0      194 2023-06-07 17:03:17.000000 auto-screener-0.1.2/auto_screener/exchanges.py
+-rw-rw-rw-   0        0        0    26687 2023-06-16 12:15:07.000000 auto-screener-0.1.2/auto_screener/feed.py
+-rw-rw-rw-   0        0        0      180 2023-04-21 16:51:56.000000 auto-screener-0.1.2/auto_screener/hints.py
+-rw-rw-rw-   0        0        0     2665 2023-04-21 16:51:36.000000 auto-screener-0.1.2/auto_screener/interval.py
+-rw-rw-rw-   0        0        0    26820 2023-06-16 12:11:56.000000 auto-screener-0.1.2/auto_screener/screener.py
+-rw-rw-rw-   0        0        0    24728 2023-06-13 13:49:29.000000 auto-screener-0.1.2/auto_screener/screening.py
+-rw-rw-rw-   0        0        0    10070 2023-06-15 16:44:13.000000 auto-screener-0.1.2/auto_screener/symbols.py
+drwxrwxrwx   0        0        0        0 2023-06-16 12:15:57.381559 auto-screener-0.1.2/auto_screener.egg-info/
+-rw-rw-rw-   0        0        0     2066 2023-06-16 12:15:57.000000 auto-screener-0.1.2/auto_screener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-06-16 12:15:57.000000 auto-screener-0.1.2/auto_screener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 12:15:57.000000 auto-screener-0.1.2/auto_screener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-16 12:15:57.000000 auto-screener-0.1.2/auto_screener.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-16 12:15:57.000000 auto-screener-0.1.2/auto_screener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 auto-screener-0.1.2/build.py
+-rw-rw-rw-   0        0        0      645 2023-06-16 12:15:57.000000 auto-screener-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       59 2023-05-24 20:12:53.000000 auto-screener-0.1.2/requirements-dev.txt
+-rw-rw-rw-   0        0        0       50 2023-05-24 19:47:16.000000 auto-screener-0.1.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 12:15:57.382559 auto-screener-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1564 2023-06-16 12:15:48.000000 auto-screener-0.1.2/setup.py
```

### Comparing `auto-screener-0.1.1/PKG-INFO` & `auto-screener-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-screener
-Version: 0.1.1
+Version: 0.1.2
 Summary: A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `auto-screener-0.1.1/README.md` & `auto-screener-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `auto-screener-0.1.1/auto_screener/base.py` & `auto-screener-0.1.2/auto_screener/base.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.1.1/auto_screener/collect.py` & `auto-screener-0.1.2/auto_screener/collect.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.1.1/auto_screener/dataset.py` & `auto-screener-0.1.2/auto_screener/dataset.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.1.1/auto_screener/document.py` & `auto-screener-0.1.2/auto_screener/document.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.1.1/auto_screener/feed.py` & `auto-screener-0.1.2/auto_screener/feed.py`

 * *Files 5% similar despite different names*

```diff
@@ -426,42 +426,55 @@
     __slots__ = (
         "handler", "recorder", "updating",
         "update_process", "loop", "limited",
         "feeds_parameters", "screening_parameters"
     )
 
     DELAY = 10
+    AMOUNT = 5
+
+    REFRESH = dt.timedelta(minutes=5)
 
     def __init__(
             self,
             location: Optional[str] = None,
             cancel: Optional[Union[Number, dt.timedelta]] = None,
             delay: Optional[Union[Number, dt.timedelta]] = None,
+            refresh: Optional[Union[Number, dt.timedelta, bool]] = None,
             limited: Optional[bool] = None,
             handler: Optional[FeedHandler] = None,
+            amount: Optional[int] = None,
             recorder: Optional[MarketRecorder] = None
     ) -> None:
         """
         Creates the class attributes.
 
         :param location: The saving location for the data.
         :param delay: The delay for the process.
         :param cancel: The cancel time for the loops.
         :param limited: The value to limit the screeners to active only.
+        :param refresh: The refresh time for rerunning.
         :param handler: The handler object for the market data.
+        :param amount: The maximum amount of symbols for each feed.
         :param recorder: The recorder object for recording the data.
         """
 
         super().__init__(
             location=location, cancel=cancel, delay=delay
         )
 
+        if refresh is True:
+            refresh = self.REFRESH
+        # end if
+
         self.handler = handler or MarketHandler()
         self.recorder = recorder or MarketRecorder()
         self.limited = limited or False
+        self.amount = amount or self.AMOUNT
+        self.refresh = refresh
 
         self.screeners: List[BaseScreener] = self.create_screeners()
 
         self.updating = False
 
         self.update_process: Optional[threading.Thread] = None
         self.loop: Optional[asyncio.AbstractEventLoop] = None
@@ -526,39 +539,41 @@
     # end create_screeners
 
     def add_feeds(
             self,
             data: Dict[str, Iterable[str]],
             fixed: Optional[bool] = True,
             separator: Optional[str] = Separator.value,
+            amount: Optional[int] = None,
             parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
     ) -> None:
         """
         Adds the tickers to the handler for each exchange.
 
         :param data: The data of the exchanges and tickers to add.
         :param parameters: The parameters for the exchanges.
         :param fixed: The value for fixed parameters to all exchanges.
+        :param amount: The maximum amount of symbols for each feed.
         :param separator: The separator of the assets.
         """
 
         self.feeds_parameters = dict(
             data=data, fixed=fixed, separator=separator, parameters=parameters
         )
 
         feed_params = self.recorder.parameters()
         feed_params.update(parameters or {})
 
         add_feeds(
             self.handler, data=data, fixed=fixed, separator=separator,
-            parameters=feed_params
+            parameters=feed_params, amount=amount or self.amount
         )
     # end add_feeds
 
-    def refresh(self) -> None:
+    def refresh_feeds(self) -> None:
         """Refreshes the feed objects."""
 
         if self.feeds_parameters is None:
             warnings.warn(
                 "Cannot refresh feeds as there was "
                 "no feeds initialization to repeat."
             )
@@ -580,15 +595,15 @@
                 "no initial process to repeat."
             )
 
             return
         # end if
 
         self.terminate()
-        self.refresh()
+        self.refresh_feeds()
         self.run(**self.screening_parameters)
     # end rerun
 
     def data(self, exchange: str, symbol: str) -> pd.DataFrame:
         """
         Returns the market data of the symbol from the exchange.
 
@@ -641,17 +656,33 @@
     # end saving_loop
 
     def update_loop(self) -> None:
         """Updates the state of the screeners."""
 
         self.updating = True
 
+        refresh = self.refresh
+
+        if isinstance(refresh, dt.timedelta):
+            refresh = refresh.total_seconds()
+        # end if
+
+        start = time.time()
+
         while self.updating:
             if self.running:
                 self.update()
+
+                current = time.time()
+
+                if refresh and ((current - start) >= refresh):
+                    self.rerun()
+
+                    start = current
+                # end if
             # end if
 
             time.sleep(self.delay)
         # end while
     # end update_loop
 
     def save(self) -> None:
@@ -825,43 +856,47 @@
         data: Dict[str, Iterable[str]],
         location: Optional[str] = None,
         cancel: Optional[Union[Number, dt.timedelta]] = None,
         delay: Optional[Union[Number, dt.timedelta]] = None,
         limited: Optional[bool] = None,
         handler: Optional[FeedHandler] = None,
         market: Optional[Market] = None,
+        amount: Optional[int] = None,
+        refresh: Optional[Union[Number, dt.timedelta, bool]] = None,
         recorder: Optional[MarketRecorder] = None,
         fixed: Optional[bool] = True,
         separator: Optional[str] = Separator.value,
         parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
 ) -> MarketScreener:
     """
     Creates the market screener object for the data.
 
     :param data: The market data.
     :param handler: The handler object for the market data.
     :param limited: The value to limit the screeners to active only.
     :param parameters: The parameters for the exchanges.
     :param market: The object to fill with the crypto feed record.
     :param fixed: The value for fixed parameters to all exchanges.
+    :param refresh: The refresh time for rerunning.
+    :param amount: The maximum amount of symbols for each feed.
     :param separator: The separator of the assets.
     :param recorder: The recorder object for recording the data.
     :param location: The saving location for the data.
     :param delay: The delay for the process.
     :param cancel: The cancel time for the loops.
 
     :return: The market screener object.
     """
 
     screener = MarketScreener(
         recorder=recorder or MarketRecorder(
             market=market or create_market(data=data)
         ),
-        handler=handler, location=location,
-        cancel=cancel, delay=delay, limited=limited
+        handler=handler, location=location, amount=amount,
+        cancel=cancel, delay=delay, limited=limited, refresh=refresh
     )
 
     screener.add_feeds(
         data=screener.recorder.structure(), fixed=fixed,
         separator=separator, parameters=parameters
     )
```

### Comparing `auto-screener-0.1.1/auto_screener/interval.py` & `auto-screener-0.1.2/auto_screener/interval.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.1.1/auto_screener/screener.py` & `auto-screener-0.1.2/auto_screener/screener.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
     "DataCollector",
     "collect_screeners",
     "wait_for_dynamic_update",
     "wait_for_dynamic_initialization",
     "BaseMultiScreener",
     "live_screeners",
     "create_market_dataframe",
-    "structure_screeners"
+    "structure_screeners",
+    "find_screeners"
 ]
 
 class WaitingState(BaseModel):
     """A class to represent the waiting state of screener objects."""
 
     modifiers = Modifiers(excluded=["create_screeners"])
 
@@ -916,8 +917,30 @@
             structure.
             setdefault(screener.exchange, {}).
             setdefault(screener.symbol, [])
         ).append(screener)
     # end for
 
     return structure
-# end structure_screeners
+# end structure_screeners
+
+def find_screeners(
+        screeners: Iterable[BaseScreener], exchange: str, symbol: str
+) -> List[BaseScreener]:
+    """
+    Finds all the screeners with the matching exchange and symbol name.
+
+    :param screeners: The screeners to process.
+    :param exchange: The exchange name for the symbol.
+    :param symbol: The pair symbol to search its screeners.
+
+    :return: The matching screeners.
+    """
+
+    return [
+        screener for screener in screeners
+        if (
+            (screener.symbol.lower() == symbol.lower()) and
+            (exchange.lower() == screener.exchange.lower())
+        )
+    ]
+# end find_screeners
```

### Comparing `auto-screener-0.1.1/auto_screener/screening.py` & `auto-screener-0.1.2/auto_screener/screening.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.1.1/auto_screener/symbols.py` & `auto-screener-0.1.2/auto_screener/symbols.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.1.1/auto_screener.egg-info/PKG-INFO` & `auto-screener-0.1.2/auto_screener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-screener
-Version: 0.1.1
+Version: 0.1.2
 Summary: A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `auto-screener-0.1.1/auto_screener.egg-info/SOURCES.txt` & `auto-screener-0.1.2/auto_screener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-screener-0.1.1/build.py` & `auto-screener-0.1.2/build.py`

 * *Files identical despite different names*

### Comparing `auto-screener-0.1.1/pyproject.toml` & `auto-screener-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'auto-screener'
-version = '0.1.1'
+version = '0.1.2'
 description = 'A software for automatically screening crypto exchanges for crypto pairs trading prices and rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `auto-screener-0.1.1/setup.py` & `auto-screener-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='auto-screener',
-        version='0.1.1',
+        version='0.1.2',
         description=(
             "A software for automatically screening "
             "crypto exchanges for crypto pairs "
             "trading prices and rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

