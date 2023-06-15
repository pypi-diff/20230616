# Comparing `tmp/memento-scorecard-0.8.1.tar.gz` & `tmp/memento-scorecard-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memento-scorecard-0.8.1.tar", last modified: Thu Jun 15 23:29:01 2023, max compression
+gzip compressed data, was "memento-scorecard-1.2.7.tar", last modified: Thu Jun 15 23:33:07 2023, max compression
```

## Comparing `memento-scorecard-0.8.1.tar` & `memento-scorecard-1.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 23:29:01.108561 memento-scorecard-0.8.1/
--rw-rw-rw-   0        0        0    11558 2023-06-07 21:33:58.000000 memento-scorecard-0.8.1/LICENSE
--rw-rw-rw-   0        0        0     1157 2023-06-15 23:29:01.106567 memento-scorecard-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0       46 2023-06-07 21:33:58.000000 memento-scorecard-0.8.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 23:29:01.088184 memento-scorecard-0.8.1/memento/
--rw-rw-rw-   0        0        0     1384 2023-06-15 23:28:46.000000 memento-scorecard-0.8.1/memento/__init__.py
--rw-rw-rw-   0        0        0    28777 2023-06-15 23:28:28.000000 memento-scorecard-0.8.1/memento/bojack.py
--rw-rw-rw-   0        0        0     7582 2023-06-15 23:06:58.000000 memento-scorecard-0.8.1/memento/diane.py
--rw-rw-rw-   0        0        0    20641 2023-06-15 23:07:02.000000 memento-scorecard-0.8.1/memento/mr_peanutbutter.py
--rw-rw-rw-   0        0        0    23946 2023-06-15 23:07:00.000000 memento-scorecard-0.8.1/memento/princess_carolyn.py
--rw-rw-rw-   0        0        0     3243 2023-06-15 23:06:56.000000 memento-scorecard-0.8.1/memento/todd.py
-drwxrwxrwx   0        0        0        0 2023-06-15 23:29:01.102284 memento-scorecard-0.8.1/memento_scorecard.egg-info/
--rw-rw-rw-   0        0        0     1157 2023-06-15 23:29:00.000000 memento-scorecard-0.8.1/memento_scorecard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-06-15 23:29:00.000000 memento-scorecard-0.8.1/memento_scorecard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 23:29:00.000000 memento-scorecard-0.8.1/memento_scorecard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-15 23:29:00.000000 memento-scorecard-0.8.1/memento_scorecard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 23:29:01.109858 memento-scorecard-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0     1433 2023-06-07 21:36:49.000000 memento-scorecard-0.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 23:33:07.924055 memento-scorecard-1.2.7/
+-rw-rw-rw-   0        0        0    11558 2023-06-07 21:33:58.000000 memento-scorecard-1.2.7/LICENSE
+-rw-rw-rw-   0        0        0     1157 2023-06-15 23:33:07.921803 memento-scorecard-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0       46 2023-06-07 21:33:58.000000 memento-scorecard-1.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 23:33:07.905454 memento-scorecard-1.2.7/memento/
+-rw-rw-rw-   0        0        0     1384 2023-06-15 23:32:58.000000 memento-scorecard-1.2.7/memento/__init__.py
+-rw-rw-rw-   0        0        0    28781 2023-06-15 23:32:29.000000 memento-scorecard-1.2.7/memento/bojack.py
+-rw-rw-rw-   0        0        0     7582 2023-06-15 23:06:58.000000 memento-scorecard-1.2.7/memento/diane.py
+-rw-rw-rw-   0        0        0    20641 2023-06-15 23:07:02.000000 memento-scorecard-1.2.7/memento/mr_peanutbutter.py
+-rw-rw-rw-   0        0        0    23946 2023-06-15 23:07:00.000000 memento-scorecard-1.2.7/memento/princess_carolyn.py
+-rw-rw-rw-   0        0        0     3243 2023-06-15 23:06:56.000000 memento-scorecard-1.2.7/memento/todd.py
+drwxrwxrwx   0        0        0        0 2023-06-15 23:33:07.917820 memento-scorecard-1.2.7/memento_scorecard.egg-info/
+-rw-rw-rw-   0        0        0     1157 2023-06-15 23:33:07.000000 memento-scorecard-1.2.7/memento_scorecard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-06-15 23:33:07.000000 memento-scorecard-1.2.7/memento_scorecard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 23:33:07.000000 memento-scorecard-1.2.7/memento_scorecard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-15 23:33:07.000000 memento-scorecard-1.2.7/memento_scorecard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 23:33:07.924055 memento-scorecard-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1433 2023-06-07 21:36:49.000000 memento-scorecard-1.2.7/setup.py
```

### Comparing `memento-scorecard-0.8.1/LICENSE` & `memento-scorecard-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `memento-scorecard-0.8.1/PKG-INFO` & `memento-scorecard-1.2.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memento-scorecard
-Version: 0.8.1
+Version: 1.2.7
 Summary: Scorecard development with Python
 Home-page: https://github.com/Guilliu/Memento
 Author: Guillermo Lizcano Villafáñez
 Author-email: guille.lv.97@gmail.com
 License: Apache License 2.0
 Keywords: python,scoring,rating,logistic,regression,scorecard,woe,credit-risk,autogrouping
 Platform: UNKNOWN
```

### Comparing `memento-scorecard-0.8.1/memento/__init__.py` & `memento-scorecard-1.2.7/memento/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from memento.princess_carolyn import (compute_final_breakpoints,
 compute_info, features_selection, display_table_ng, reagrupa_var)
 from memento.mr_peanutbutter import (pretty_scorecard, parceling, cell_style,
 predict_pyspark, metrics_pyspark, compute_pyspark_ks, save_model,
 save_light_model, load_model, genera_punt_par, proc_freq)
 from memento.bojack import scorecard, autogrouping
 
-__version__ = '0.8.1'
+__version__ = '1.2.7'
 
 __all__ = (
     string_categories1, string_categories2, string_to_num,
     breakpoints_to_str, breakpoints_to_num, remapeo_missing, data_convert, adapt_data,
     compute_group_names, compute_table, transform_to_woes,
     calib_score, compute_scorecard, transform_to_points, apply_scorecard, compute_metrics,
     compute_final_breakpoints,
```

### Comparing `memento-scorecard-0.8.1/memento/bojack.py` & `memento-scorecard-1.2.7/memento/bojack.py`

 * *Files 0% similar despite different names*

```diff
@@ -498,16 +498,16 @@
             aux = '<Characteristic name="{}">\n'.format(i)
             points = list(self.scorecard[self.scorecard['Variable'] == i]['Aligned score'])
             groups = copy.deepcopy(list(self.scorecard[self.scorecard['Variable'] == i]['Group']))
             
             for j in range(len(points)):
                 
                 if reasons_code: 
-                    aux += '<Attribute partialScore="{}" \
-                    reasonCode="{}_{}">\n'.format(points[j], i, j+1)
+                    aux += '<Attribute partialScore="{}" ' +\
+                    'reasonCode="{}_{}">\n'.format(points[j], i, j+1)
                 else: aux += '<Attribute partialScore="{}">\n'.format(points[j])
                 
                 if self.autogroupings[i].dtype not in ('object', 'bool'):
   
                     if 'Missing' in groups[j]:
                         if len(groups[j]) > 7: aux += '<CompoundPredicate booleanOperator="or">\n'
                         aux += '<SimplePredicate field="{}" operator="isMissing"/>\n'.format(i)
```

### Comparing `memento-scorecard-0.8.1/memento/diane.py` & `memento-scorecard-1.2.7/memento/diane.py`

 * *Files identical despite different names*

### Comparing `memento-scorecard-0.8.1/memento/mr_peanutbutter.py` & `memento-scorecard-1.2.7/memento/mr_peanutbutter.py`

 * *Files identical despite different names*

### Comparing `memento-scorecard-0.8.1/memento/princess_carolyn.py` & `memento-scorecard-1.2.7/memento/princess_carolyn.py`

 * *Files identical despite different names*

### Comparing `memento-scorecard-0.8.1/memento/todd.py` & `memento-scorecard-1.2.7/memento/todd.py`

 * *Files identical despite different names*

### Comparing `memento-scorecard-0.8.1/memento_scorecard.egg-info/PKG-INFO` & `memento-scorecard-1.2.7/memento_scorecard.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memento-scorecard
-Version: 0.8.1
+Version: 1.2.7
 Summary: Scorecard development with Python
 Home-page: https://github.com/Guilliu/Memento
 Author: Guillermo Lizcano Villafáñez
 Author-email: guille.lv.97@gmail.com
 License: Apache License 2.0
 Keywords: python,scoring,rating,logistic,regression,scorecard,woe,credit-risk,autogrouping
 Platform: UNKNOWN
```

### Comparing `memento-scorecard-0.8.1/setup.py` & `memento-scorecard-1.2.7/setup.py`

 * *Files identical despite different names*

