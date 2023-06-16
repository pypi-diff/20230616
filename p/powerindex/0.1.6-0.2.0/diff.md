# Comparing `tmp/powerindex-0.1.6.tar.gz` & `tmp/powerindex-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerindex-0.1.6.tar", last modified: Sun Jul 25 20:00:34 2021, max compression
+gzip compressed data, was "powerindex-0.2.0.tar", last modified: Fri Jun 16 15:28:18 2023, max compression
```

## Comparing `powerindex-0.1.6.tar` & `powerindex-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2021-07-25 20:00:34.000000 powerindex-0.1.6/
--rw-r--r--   0 jovyan    (1000) users      (100)      922 2021-07-25 20:00:34.000000 powerindex-0.1.6/PKG-INFO
--rw-rw-rw-   0 jovyan    (1000) users      (100)     5464 2021-07-25 20:00:18.000000 powerindex-0.1.6/README.md
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2021-07-25 20:00:34.000000 powerindex-0.1.6/powerindex/
--rw-rw-rw-   0 jovyan    (1000) users      (100)       36 2021-07-25 20:00:18.000000 powerindex-0.1.6/powerindex/__init__.py
--rw-rw-rw-   0 jovyan    (1000) users      (100)    12803 2021-07-25 20:00:18.000000 powerindex-0.1.6/powerindex/powerindex.py
--rw-rw-rw-   0 jovyan    (1000) users      (100)     2926 2021-07-25 20:00:18.000000 powerindex-0.1.6/powerindex/testpowerindex.py
-drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2021-07-25 20:00:34.000000 powerindex-0.1.6/powerindex.egg-info/
--rw-r--r--   0 jovyan    (1000) users      (100)      922 2021-07-25 20:00:34.000000 powerindex-0.1.6/powerindex.egg-info/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)      231 2021-07-25 20:00:34.000000 powerindex-0.1.6/powerindex.egg-info/SOURCES.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2021-07-25 20:00:34.000000 powerindex-0.1.6/powerindex.egg-info/dependency_links.txt
--rw-r--r--   0 jovyan    (1000) users      (100)       11 2021-07-25 20:00:34.000000 powerindex-0.1.6/powerindex.egg-info/top_level.txt
--rw-r--r--   0 jovyan    (1000) users      (100)       38 2021-07-25 20:00:34.000000 powerindex-0.1.6/setup.cfg
--rw-rw-rw-   0 jovyan    (1000) users      (100)     1221 2021-07-25 20:00:18.000000 powerindex-0.1.6/setup.py
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-16 15:28:18.833151 powerindex-0.2.0/
+-rw-r--r--   0 jovyan    (1000) users      (100)      922 2023-06-16 15:28:18.833151 powerindex-0.2.0/PKG-INFO
+-rw-rw-rw-   0 jovyan    (1000) users      (100)     5974 2023-06-16 15:28:07.000000 powerindex-0.2.0/README.md
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-16 15:28:18.832236 powerindex-0.2.0/powerindex/
+-rw-rw-rw-   0 jovyan    (1000) users      (100)       36 2023-06-16 15:28:07.000000 powerindex-0.2.0/powerindex/__init__.py
+-rw-rw-rw-   0 jovyan    (1000) users      (100)    14099 2023-06-16 15:28:07.000000 powerindex-0.2.0/powerindex/powerindex.py
+-rw-rw-rw-   0 jovyan    (1000) users      (100)     2926 2023-06-16 15:28:07.000000 powerindex-0.2.0/powerindex/testpowerindex.py
+drwxr-xr-x   0 jovyan    (1000) users      (100)        0 2023-06-16 15:28:18.833151 powerindex-0.2.0/powerindex.egg-info/
+-rw-r--r--   0 jovyan    (1000) users      (100)      922 2023-06-16 15:28:18.000000 powerindex-0.2.0/powerindex.egg-info/PKG-INFO
+-rw-r--r--   0 jovyan    (1000) users      (100)      283 2023-06-16 15:28:18.000000 powerindex-0.2.0/powerindex.egg-info/SOURCES.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)        1 2023-06-16 15:28:18.000000 powerindex-0.2.0/powerindex.egg-info/dependency_links.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)       51 2023-06-16 15:28:18.000000 powerindex-0.2.0/powerindex.egg-info/entry_points.txt
+-rw-r--r--   0 jovyan    (1000) users      (100)       11 2023-06-16 15:28:18.000000 powerindex-0.2.0/powerindex.egg-info/top_level.txt
+-rw-rw-rw-   0 jovyan    (1000) users      (100)      369 2023-06-16 15:28:07.000000 powerindex-0.2.0/pyproject.toml
+-rw-r--r--   0 jovyan    (1000) users      (100)       38 2023-06-16 15:28:18.833151 powerindex-0.2.0/setup.cfg
+-rw-rw-rw-   0 jovyan    (1000) users      (100)     1335 2023-06-16 15:28:07.000000 powerindex-0.2.0/setup.py
```

### Comparing `powerindex-0.1.6/PKG-INFO` & `powerindex-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 1.1
 Name: powerindex
-Version: 0.1.6
+Version: 0.2.0
 Summary: python library to calculate power indices in weighted voting games
-Home-page: http://github.com/maxlit/powerindex
+Home-page: http://gitlab.com/maxlit/powerindex
 Author: Maxim Litvak
 Author-email: maxim@litvak.eu
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: power index,voting,Banzhaf,Shapley,Shubik,weighted voting game,game theory,political science
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `powerindex-0.1.6/README.md` & `powerindex-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,120 +3,158 @@
 [![Build Status](https://travis-ci.org/maxlit/powerindex.svg?branch=master)](https://travis-ci.org/maxlit/powerindex)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/maxlit/powerindex/master?filepath=README.ipynb)
 
 A python library to compute power indices
 
 __Installation__: pip install powerindex
 
+## TL;DR
+
+Calculation of power indices. Example of CLI ("px" alias) run ([EEC](https://en.wikipedia.org/wiki/European_Economic_Community) in 1957 ):
+
+![png](cli.png)
+
 ## What is all about
 
-The aim of the package is to compute different power indices of the so-called weighted voting systems (games). This package was employed to perform calculations at [powdist.com](powdist.com)
+The aim of the package is to compute different power indices of the so-called weighted voting systems (games).
 
 Players have weights and can form coalitions. A coalition that achieves the required threshold wins.
 
 To start with a simple example, consider a system with two parties __A__ and  **B** having 51 and 49 seats respectively with a simple majority rule (i.e. the threshold is 51 seats). How much power do they have? It may appear that according to the number of the seats they have 51% and 49% respectively.
 
 However, party **A** can impose any decision without cooperating with party __B__.
 
 It leads to a conclusion that any reasonable rule would assign to party **A** 100% of the power (since it wins without cooperation) and to the party __B__ 0% of the power and not 51% to 49%.
 
 The most popular approaches to measure power are [Banzhaf](http://en.wikipedia.org/wiki/Banzhaf_power_index) and [Shapley-Shubik](http://en.wikipedia.org/wiki/Shapley–Shubik_power_index) power indices.
 
 ## How to use it
 
-If you work with docker, launch the jupyter notebook from the command line as follows
+It can be run either as a command line (px) or in python interpreter.
+CLI run:
 
 ```bash
-docker pull axlit/powerindex
-docker run -p 8888:8888 axlit/powerindex
+px -i b -q 4 -w 3 2 1 
 ```
 
-copy the link from the command line and then navigate to /powerindex/README.ipynb notebook in the browser.
+Flags:
+**-i** (index) is either 'b' for Banzhaf, or 'ss' for Shapley-Shubik.
+**-q** (quota) number of votes for a coalition to win.
+**-w** (weights) weights of players.
+
+There's a jupyter notebook /powerindex/README.ipynb that shows some python examples.
+
+A trivial example from the introduction:
 
-Let's implement an example from the introduction:
+```bash
+#bash
+px -i b -q 51 -w 51 49
+px -i ss -q 51 -w 51 49 
+```
 
 ```python
-%matplotlib inline
+#python
+#%matplotlib inline
 import powerindex as px
 game=px.Game(quota=51,weights=[51,49])
 ```
 
-Now calculate Banzhaf and Shapley-Shubik power indices:
-
+Calculation of Banzhaf and Shapley-Shubik power indices:
 
 ```python
+#python
 game.calc_banzhaf()
 print(game.banzhaf)
 ```
 
     [1.0, 0.0]
 
 
-
 ```python
+#python
 game.calc_shapley_shubik()
 print(game.shapley_shubik)
 ```
 
     [1.0, 0.0]
 
 
 Function calc() computes all available indices.
 
 Thus, in this simple example both indices give 100% to 0% distribution.
 
 Now let's changes the seats distribution to the parity and see what happens:
 
+```bash
+#bash
+px -i b -q 51 -w 50 50
+px -i ss -q 51 -w 50 50 
+```
 
 ```python
+#python
 game=px.Game(51,weights=[50,50])
 game.calc()
 
 print(game.banzhaf)
 print(game.shapley_shubik)
 ```
 
     [0.5, 0.5]
     [0.5, 0.5]
 
+As the result, the distribution of power is also at parity.
 
-As the result, the power distribution is also at parity.
-
-Now, consider a non-trivial, but still simple examples from [Wikipedia](https://en.wikipedia.org/wiki/Banzhaf_power_index#Simple_voting_game):
+Now, consider a non-trivial, but still a simple examples from [Wikipedia](https://en.wikipedia.org/wiki/Banzhaf_power_index#Simple_voting_game):
 
+```bash
+#bash
+px -i b -q 6 -w 4 3 2 1 
+```
 
 ```python
+#python
 game=px.Game(6,[4, 3, 2, 1])
 game.calc_banzhaf()
 print(game.banzhaf)
 ```
 
     [0.4166666666666667, 0.25, 0.25, 0.08333333333333333]
 
 
 Interpretation is simple. A committee where 4 parties hold 40%, 30%, 20% and 10% of seats with required qualified majority of 60%, have 41.7%, 25%, 25%, 8.3% of power respectively.
 
 In this example, having 2 or 3 seats leads to the same level of power.
 
 Another example:
 
+```bash
+#bash
+px -i b -q 6 -w 3 2 1 1 
+```
 
 ```python
+#python
 game=px.Game(6,[3, 2, 1, 1])
 game.calc_banzhaf()
 print(game.banzhaf)
 ```
 
     [0.375, 0.375, 0.125, 0.125]
 
 
 Notice that in the previous two examples Banzhaf and Shapley-Shubik indices coincides. It doesn't hold in general even in the games of 3 voters:
 
+```bash
+#bash
+px -i ss -q 6 -w 3 2 1 1 
+```
 
 ```python
+#python
 game=px.Game(4,[3, 2, 1])
 game.calc() # again it calculates all available indices
 print("Banzhaf index:")
 print(game.banzhaf)
 print("Shapley-Shubik index:")
 print(game.shapley_shubik)
 ```
@@ -129,29 +167,30 @@
 
 ## Plot results
 
 There's a possibility to plot the power distribution as a pie chart:
 
 
 ```python
+#python
 game=px.Game(4,[3, 2, 1])
 game.calc()
 game.pie_chart()
 ```
 
-
 ![png](output_14_0.png)
 
 
 As you can see on the plot, the parties have numbers. In order, to put their names on the chart you need to work with Party class. 
 
 Let's take Europen Economic Community (EEC) in the years 1958-1972, its members were Germany (4 votes), France (4 votes), Italy (4 votes), Belgium (2 votes), Netherlands (2 votes) and Luxembourg (1 vote) with qualified majority of 12 votes:
 
 
 ```python
+#python
 countries={"Germany":4,"France":4,"Italy":4,"Belgium":2,"Netherlands":2,"Luxembourg":1}
 parties=[px.Party(countries[country],country) for country in countries]
 game=px.Game(12,parties=parties)
 game.calc()
 game.pie_chart()
 ```
```

### Comparing `powerindex-0.1.6/powerindex/powerindex.py` & `powerindex-0.2.0/powerindex/powerindex.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import math
 import itertools as it
+import argparse
+import sys
 
 class Party:
     def __init__(self,weight,name):
         self.weight=weight
         self.name=name
     def __eq__(self,other):
         if self.name==other.name:
@@ -44,22 +46,23 @@
         return "The game consists of %s parties, the threshold is %s"%(len(self.parties),self.quota)
 
     """
         This function launches calculation of all implemented indeces
     """
     def calc(self):
         # find if there's a party with seats greater or equal to quota
-        ge_quota=map(lambda x: 1 if x>=self.quota else 0,self.weights)
-        num_ge_quota=sum(ge_quota)
-        if num_ge_quota==0: # if not calculate according to algos
+        ge_quota = list(map(lambda x: 1 if x >= self.quota else 0, self.weights))
+        num_ge_quota = sum(ge_quota)
+        if num_ge_quota == 0: # if not calculate according to algos
             self.calc_banzhaf()
             self.calc_shapley_shubik()
         else: # if yes manually assign all power to the party (parties)
-            self.banzhaf=map(lambda x: x/float(num_ge_quota),ge_quota)
-            self.shapley_shubik=map(lambda x: x/float(num_ge_quota),ge_quota)
+            self.banzhaf = list(map(lambda x: x / float(num_ge_quota), ge_quota))
+            self.shapley_shubik = list(map(lambda x: x / float(num_ge_quota), ge_quota))
+
 
     """
         Computes Banzhaf power index using generating function approach.
     """
     def calc_banzhaf(self):
         coeffs=self._coeffs_of_general_GF("Banzhaf")
         pows=[sum(self._coeffs_of_player_GF(coeffs,weight,"Banzhaf")[(self.quota-weight):self.quota]) for weight in self.weights]
@@ -306,7 +309,40 @@
         f.write(output)
         f.close()
 
     def hist():
         # to do
         n, bins, patches = plt.hist(x, num_bins, normed=1, facecolor='green', alpha=0.5)
         print("not implemented yet")
+
+
+def calculate_power_index(weights, quota, index_type):
+    # Your power index calculation logic goes here
+    game=Game(quota, weights)
+    if index_type=="ss":
+        game.calc_shapley_shubik()
+        return game.shapley_shubik
+    elif index_type=="b":
+        game.calc_banzhaf()
+        return game.banzhaf
+    else:
+        raise ValueError("Unknown power index type: %s, only 'ss' (Shapley-Shubik) and 'b' (Banzhaf) are accepted" % index_type)
+
+def main():
+    parser = argparse.ArgumentParser(prog='px', description='Calculate power index')
+    parser.add_argument('-i', '--index', metavar='INDEX', choices=['ss', 'b'], required=True, help='Power index type')
+    parser.add_argument('-q', '--quota', metavar='QUOTA', type=int, required=True, help='Quota value')
+    parser.add_argument('-w', '--weights', metavar='WEIGHT', type=int, nargs='+', required=True, help='Weights')
+
+    args = parser.parse_args()
+    index_type = args.index
+    quota = args.quota
+    weights = list(args.weights)  # Convert to a Python list
+
+    power_index = calculate_power_index(weights, quota, index_type)
+    print(power_index)
+    sys.stdout.flush()
+    # Print or use the power index as needed
+
+if __name__ == '__main__':
+    main()
+
```

### Comparing `powerindex-0.1.6/powerindex/testpowerindex.py` & `powerindex-0.2.0/powerindex/testpowerindex.py`

 * *Files identical despite different names*

### Comparing `powerindex-0.1.6/powerindex.egg-info/PKG-INFO` & `powerindex-0.2.0/powerindex.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 1.1
 Name: powerindex
-Version: 0.1.6
+Version: 0.2.0
 Summary: python library to calculate power indices in weighted voting games
-Home-page: http://github.com/maxlit/powerindex
+Home-page: http://gitlab.com/maxlit/powerindex
 Author: Maxim Litvak
 Author-email: maxim@litvak.eu
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: power index,voting,Banzhaf,Shapley,Shubik,weighted voting game,game theory,political science
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `powerindex-0.1.6/setup.py` & `powerindex-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 setup(name='powerindex',
     version=os.environ['CI_COMMIT_TAG'],
     description='python library to calculate power indices in weighted voting games',
     author='Maxim Litvak',
     author_email='maxim@litvak.eu',
-    url='http://github.com/maxlit/powerindex',
+    url='http://gitlab.com/maxlit/powerindex',
     test_suite='test',
     packages=['powerindex'],
     keywords=['power index','voting','Banzhaf','Shapley','Shubik', 'weighted voting game','game theory', 'political science'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Environment :: Console',
         'Intended Audience :: Developers',
@@ -25,9 +25,14 @@
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: POSIX',
         'Programming Language :: Python',
         'Topic :: Education',
         'Topic :: Sociology'
         ],
+    entry_points={
+        'console_scripts': [
+            'px = powerindex.powerindex:main'
+        ]
+        }
                                          )
```

