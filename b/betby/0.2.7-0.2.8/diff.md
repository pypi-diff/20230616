# Comparing `tmp/betby-0.2.7.tar.gz` & `tmp/betby-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betby-0.2.7.tar", last modified: Thu Jun 15 12:34:50 2023, max compression
+gzip compressed data, was "betby-0.2.8.tar", last modified: Fri Jun 16 10:51:48 2023, max compression
```

## Comparing `betby-0.2.7.tar` & `betby-0.2.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 12:34:50.013244 betby-0.2.7/
--rw-rw-rw-   0        0        0      539 2023-06-15 12:34:50.012243 betby-0.2.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-15 12:34:49.989243 betby-0.2.7/betby/
--rw-rw-rw-   0        0        0       21 2023-05-09 23:44:47.000000 betby-0.2.7/betby/__init__.py
--rw-rw-rw-   0        0        0     8736 2023-06-15 11:56:52.000000 betby-0.2.7/betby/markets.py
-drwxrwxrwx   0        0        0        0 2023-06-15 12:34:50.008243 betby-0.2.7/betby.egg-info/
--rw-rw-rw-   0        0        0      539 2023-06-15 12:34:47.000000 betby-0.2.7/betby.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      159 2023-06-15 12:34:49.000000 betby-0.2.7/betby.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 12:34:47.000000 betby-0.2.7/betby.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-15 12:34:47.000000 betby-0.2.7/betby.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 12:34:50.014243 betby-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      637 2023-06-15 12:00:01.000000 betby-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 10:51:48.623677 betby-0.2.8/
+-rw-rw-rw-   0        0        0      539 2023-06-16 10:51:48.622677 betby-0.2.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-16 10:51:48.600678 betby-0.2.8/betby/
+-rw-rw-rw-   0        0        0       21 2023-05-09 23:44:47.000000 betby-0.2.8/betby/__init__.py
+-rw-rw-rw-   0        0        0     9722 2023-06-16 10:49:52.000000 betby-0.2.8/betby/markets.py
+drwxrwxrwx   0        0        0        0 2023-06-16 10:51:48.618678 betby-0.2.8/betby.egg-info/
+-rw-rw-rw-   0        0        0      539 2023-06-16 10:51:45.000000 betby-0.2.8/betby.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      159 2023-06-16 10:51:47.000000 betby-0.2.8/betby.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 10:51:45.000000 betby-0.2.8/betby.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-16 10:51:45.000000 betby-0.2.8/betby.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 10:51:48.623677 betby-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      637 2023-06-16 10:50:19.000000 betby-0.2.8/setup.py
```

### Comparing `betby-0.2.7/PKG-INFO` & `betby-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betby
-Version: 0.2.7
+Version: 0.2.8
 Summary: Betby libraries
 Author: Ayrat Badrutdinov
 Author-email: a.badrutdinov@betby.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betby-0.2.7/betby/markets.py` & `betby-0.2.8/betby/markets.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import numpy as np
 from math import exp, factorial
+import markets
+from markets.specifiers import format_specifiers
 
 
 class Get_markets:
     def __init__(self, avg_1, avg_2, score_1=0, score_2=0, time=0,
                  time_full=93, time_block=90, matrix=None, poisson=False,
                  result=None):
         self.avg_1 = avg_1
@@ -88,111 +90,140 @@
         for i in range(self.poisson or self.poi_1):
             for j in range(self.poisson or self.poi_1):
                 if j - i < -0.5 + self.score_1 - self.score_2:
                     prob_1 += self.matrix[i, j]
                 if j - i > 0.5 + self.score_1 - self.score_2:
                     prob_2 += self.matrix[i, j]
         hand_key = format_specifiers(markets.THREE_WAY_WINNER, {})
-        hand_dict = {
-            markets.THREE_WAY_WINNER_HOME: self.get_outcome(
-                self.margin(1 / prob_1, mar, max_odds), 0),
-            markets.THREE_WAY_WINNER_DRAW: self.get_outcome(
-                self.margin(1 / (1 - prob_1 - prob_2), mar, max_odds), 0),
-            markets.THREE_WAY_WINNER_AWAY: self.get_outcome(
-                self.margin(1 / prob_2, mar, max_odds), 0)
-        }
-        if not self.betstop and prob_1 <= 1 - min_prob and prob_1 >= \
-                min_prob and prob_2 <= 1 - min_prob and prob_2 >= min_prob \
-                and 1 - prob_1 - prob_2 <= 1 - min_prob and 1 - prob_1 - \
-                prob_2 >= min_prob:
+        hand_dict = {}
+
+        if prob_1 != 0 and prob_2 != 0 and 1 - prob_1 - prob_2 != 0:
+            hand_dict = {
+                markets.THREE_WAY_WINNER_HOME: self.get_outcome(
+                    self.margin(1 / prob_1, mar, max_odds), 0),
+                markets.THREE_WAY_WINNER_DRAW: self.get_outcome(
+                    self.margin(1 / (1 - prob_1 - prob_2), mar, max_odds), 0),
+                markets.THREE_WAY_WINNER_AWAY: self.get_outcome(
+                    self.margin(1 / prob_2, mar, max_odds), 0)
+            }
+
+        if (
+            not self.betstop
+            and prob_1 <= 1 - min_prob
+            and prob_1 >= min_prob
+            and prob_2 <= 1 - min_prob
+            and prob_2 >= min_prob
+            and 1 - prob_1 - prob_2 <= 1 - min_prob
+            and 1 - prob_1 - prob_2 >= min_prob
+            and hand_dict
+        ):
             if markets.THREE_WAY_WINNER not in self.result:
                 self.result[markets.THREE_WAY_WINNER] = {}
             self.result[markets.THREE_WAY_WINNER].update({hand_key: hand_dict})
 
     def total(self, mar=0.05, min_prob=0.2, max_odds=25):
         prob = 0
         for val in range(2 * self.poisson or 2 * self.poi_1):
             for i in range(self.poisson or self.poi_1):
                 for j in range(self.poisson or self.poi_1):
                     if i + j < val + 0.5:
                         prob += self.matrix[i, j]
-            total_key = format_specifiers(markets.TOTAL,
-                    {'total': str(val + 0.5 + self.score_1 + self.score_2)})
-            total_dict = {
-                markets.TOTAL_OVER: self.get_outcome(self.margin(
-                    1 / (1 - prob), mar, max_odds), 0),
-                markets.TOTAL_UNDER: self.get_outcome(self.margin(
-                    1 / prob, mar, max_odds), 0)
-            }
-            if not self.betstop and prob <= 1 - min_prob and prob >= min_prob:
+            total_key = format_specifiers(markets.TOTAL, {
+                'total': str(val + 0.5 + self.score_1 + self.score_2)})
+            total_dict = {}
+
+            if prob != 0 and 1 - prob != 0:  # Добавленная проверка
+                total_dict = {
+                    markets.TOTAL_OVER: self.get_outcome(
+                        self.margin(1 / (1 - prob), mar, max_odds), 0),
+                    markets.TOTAL_UNDER: self.get_outcome(
+                        self.margin(1 / prob, mar, max_odds), 0)
+                }
+
+            if not self.betstop and prob <= 1 - min_prob and prob >= \
+                    min_prob and total_dict:
                 if markets.TOTAL not in self.result:
                     self.result[markets.TOTAL] = {}
                 self.result[markets.TOTAL].update({total_key: total_dict})
             prob = 0
 
     def handicap(self, mar=0.05, min_prob=0.2, max_odds=25):
         prob = 0
-        for val in range(1 - (
-                self.poisson or self.poi_1), (
-                    self.poisson or self.poi_1) - 1):
+        for val in range(1 - (self.poisson or self.poi_1),
+                         (self.poisson or self.poi_1) - 1):
             for i in range(self.poisson or self.poi_1):
                 for j in range(self.poisson or self.poi_1):
                     if j - i > val + 0.5:
                         prob += self.matrix[i, j]
                         # print(val + 0.5, i, j, prob)
-            hand_key = format_specifiers(markets.HANDICAP,
-                    {'hcp': str(val + 0.5 - self.score_1 + self.score_2)})
-            hand_dict = {
-                markets.HANDICAP_HOME: self.get_outcome(
-                    self.margin(1 / (1 - prob), mar, max_odds), 0),
-                markets.HANDICAP_AWAY: self.get_outcome(
-                    self.margin(1 / prob, mar, max_odds), 0)
-            }
-            if not self.betstop and prob <= 1 - min_prob and prob >= min_prob:
+            hand_key = format_specifiers(markets.HANDICAP, {
+                'hcp': str(val + 0.5 - self.score_1 + self.score_2)})
+            hand_dict = {}
+
+            if prob != 0 and 1 - prob != 0:  # Добавленная проверка
+                hand_dict = {
+                    markets.HANDICAP_HOME: self.get_outcome(
+                        self.margin(1 / (1 - prob), mar, max_odds), 0),
+                    markets.HANDICAP_AWAY: self.get_outcome(
+                        self.margin(1 / prob, mar, max_odds), 0)
+                }
+
+            if not self.betstop and prob <= 1 - min_prob and prob >= \
+                    min_prob and hand_dict:
                 if markets.HANDICAP not in self.result:
                     self.result[markets.HANDICAP] = {}
                 self.result[markets.HANDICAP].update({hand_key: hand_dict})
             prob = 0
 
     def home_total(self, mar=0.05, min_prob=0.2, max_odds=25):
         prob = 0
         for val in range(self.poisson or self.poi_1):
             for i in range(self.poisson or self.poi_1):
                 for j in range(self.poisson or self.poi_1):
                     if i < val + 0.5:
                         prob += self.matrix[i, j]
-            home_total_key = format_specifiers(markets.HOME_TOTAL,
-                        {'total': str(val + 0.5 + self.score_1)})
-            home_total_dict = {
-                markets.HOME_TOTAL_OVER: self.get_outcome(self.margin(
-                    1 / (1 - prob), mar, max_odds), 0),
-                markets.HOME_TOTAL_UNDER: self.get_outcome(self.margin(
-                    1 / prob, mar, max_odds), 0)
-            }
-            if not self.betstop and prob <= 1 - min_prob and prob >= min_prob:
+            home_total_key = format_specifiers(markets.HOME_TOTAL, {
+                'total': str(val + 0.5 + self.score_1)})
+            home_total_dict = {}
+
+            if prob != 0 and 1 - prob != 0:  # Добавленная проверка
+                home_total_dict = {
+                    markets.HOME_TOTAL_OVER: self.get_outcome(
+                        self.margin(1 / (1 - prob), mar, max_odds), 0),
+                    markets.HOME_TOTAL_UNDER: self.get_outcome(
+                        self.margin(1 / prob, mar, max_odds), 0)
+                }
+
+            if not self.betstop and prob <= 1 - min_prob and prob >= \
+                    min_prob and home_total_dict:
                 if markets.HOME_TOTAL not in self.result:
                     self.result[markets.HOME_TOTAL] = {}
                 self.result[markets.HOME_TOTAL].update(
                     {home_total_key: home_total_dict})
             prob = 0
 
     def away_total(self, mar=0.05, min_prob=0.2, max_odds=25):
         prob = 0
         for val in range(self.poisson or self.poi_1):
             for i in range(self.poisson or self.poi_1):
                 for j in range(self.poisson or self.poi_1):
                     if j < val + 0.5:
                         prob += self.matrix[i, j]
-            away_total_key = format_specifiers(markets.AWAY_TOTAL,
-                        {'total': str(val + 0.5 + self.score_2)})
-            away_total_dict = {
-                markets.AWAY_TOTAL_OVER: self.get_outcome(self.margin(
-                    1 / (1 - prob), mar, max_odds), 0),
-                markets.AWAY_TOTAL_UNDER: self.get_outcome(self.margin(
-                    1 / prob, mar, max_odds), 0)
-            }
-            if not self.betstop and prob <= 1 - min_prob and prob >= min_prob:
+            away_total_key = format_specifiers(markets.AWAY_TOTAL, {
+                'total': str(val + 0.5 + self.score_2)})
+            away_total_dict = {}
+
+            if prob != 0 and 1 - prob != 0:  # Добавленная проверка
+                away_total_dict = {
+                    markets.AWAY_TOTAL_OVER: self.get_outcome(
+                        self.margin(1 / (1 - prob), mar, max_odds), 0),
+                    markets.AWAY_TOTAL_UNDER: self.get_outcome(
+                        self.margin(1 / prob, mar, max_odds), 0)
+                }
+
+            if not self.betstop and prob <= 1 - min_prob and prob >= \
+                    min_prob and away_total_dict:
                 if markets.AWAY_TOTAL not in self.result:
                     self.result[markets.AWAY_TOTAL] = {}
                 self.result[markets.AWAY_TOTAL].update(
                     {away_total_key: away_total_dict})
             prob = 0
```

### Comparing `betby-0.2.7/betby.egg-info/PKG-INFO` & `betby-0.2.8/betby.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betby
-Version: 0.2.7
+Version: 0.2.8
 Summary: Betby libraries
 Author: Ayrat Badrutdinov
 Author-email: a.badrutdinov@betby.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `betby-0.2.7/setup.py` & `betby-0.2.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="betby",
-    version="0.2.7",
+    version="0.2.8",
     author="Ayrat Badrutdinov",
     author_email="a.badrutdinov@betby.com",
     description="Betby libraries",
     packages=["betby"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

