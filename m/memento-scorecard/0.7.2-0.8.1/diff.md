# Comparing `tmp/memento-scorecard-0.7.2.tar.gz` & `tmp/memento-scorecard-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memento-scorecard-0.7.2.tar", last modified: Thu Jun 15 23:20:18 2023, max compression
+gzip compressed data, was "memento-scorecard-0.8.1.tar", last modified: Thu Jun 15 23:29:01 2023, max compression
```

## Comparing `memento-scorecard-0.7.2.tar` & `memento-scorecard-0.8.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 23:20:18.909085 memento-scorecard-0.7.2/
--rw-rw-rw-   0        0        0    11558 2023-06-07 21:33:58.000000 memento-scorecard-0.7.2/LICENSE
--rw-rw-rw-   0        0        0     1157 2023-06-15 23:20:18.906576 memento-scorecard-0.7.2/PKG-INFO
--rw-rw-rw-   0        0        0       46 2023-06-07 21:33:58.000000 memento-scorecard-0.7.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-15 23:20:18.887353 memento-scorecard-0.7.2/memento/
--rw-rw-rw-   0        0        0     1384 2023-06-15 23:20:12.000000 memento-scorecard-0.7.2/memento/__init__.py
--rw-rw-rw-   0        0        0    28736 2023-06-15 23:13:37.000000 memento-scorecard-0.7.2/memento/bojack.py
--rw-rw-rw-   0        0        0     7582 2023-06-15 23:06:58.000000 memento-scorecard-0.7.2/memento/diane.py
--rw-rw-rw-   0        0        0    20641 2023-06-15 23:07:02.000000 memento-scorecard-0.7.2/memento/mr_peanutbutter.py
--rw-rw-rw-   0        0        0    23946 2023-06-15 23:07:00.000000 memento-scorecard-0.7.2/memento/princess_carolyn.py
--rw-rw-rw-   0        0        0     3243 2023-06-15 23:06:56.000000 memento-scorecard-0.7.2/memento/todd.py
-drwxrwxrwx   0        0        0        0 2023-06-15 23:20:18.902112 memento-scorecard-0.7.2/memento_scorecard.egg-info/
--rw-rw-rw-   0        0        0     1157 2023-06-15 23:20:18.000000 memento-scorecard-0.7.2/memento_scorecard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-06-15 23:20:18.000000 memento-scorecard-0.7.2/memento_scorecard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 23:20:18.000000 memento-scorecard-0.7.2/memento_scorecard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-15 23:20:18.000000 memento-scorecard-0.7.2/memento_scorecard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 23:20:18.909592 memento-scorecard-0.7.2/setup.cfg
--rw-rw-rw-   0        0        0     1433 2023-06-07 21:36:49.000000 memento-scorecard-0.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 23:29:01.108561 memento-scorecard-0.8.1/
+-rw-rw-rw-   0        0        0    11558 2023-06-07 21:33:58.000000 memento-scorecard-0.8.1/LICENSE
+-rw-rw-rw-   0        0        0     1157 2023-06-15 23:29:01.106567 memento-scorecard-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0       46 2023-06-07 21:33:58.000000 memento-scorecard-0.8.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 23:29:01.088184 memento-scorecard-0.8.1/memento/
+-rw-rw-rw-   0        0        0     1384 2023-06-15 23:28:46.000000 memento-scorecard-0.8.1/memento/__init__.py
+-rw-rw-rw-   0        0        0    28777 2023-06-15 23:28:28.000000 memento-scorecard-0.8.1/memento/bojack.py
+-rw-rw-rw-   0        0        0     7582 2023-06-15 23:06:58.000000 memento-scorecard-0.8.1/memento/diane.py
+-rw-rw-rw-   0        0        0    20641 2023-06-15 23:07:02.000000 memento-scorecard-0.8.1/memento/mr_peanutbutter.py
+-rw-rw-rw-   0        0        0    23946 2023-06-15 23:07:00.000000 memento-scorecard-0.8.1/memento/princess_carolyn.py
+-rw-rw-rw-   0        0        0     3243 2023-06-15 23:06:56.000000 memento-scorecard-0.8.1/memento/todd.py
+drwxrwxrwx   0        0        0        0 2023-06-15 23:29:01.102284 memento-scorecard-0.8.1/memento_scorecard.egg-info/
+-rw-rw-rw-   0        0        0     1157 2023-06-15 23:29:00.000000 memento-scorecard-0.8.1/memento_scorecard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-06-15 23:29:00.000000 memento-scorecard-0.8.1/memento_scorecard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 23:29:00.000000 memento-scorecard-0.8.1/memento_scorecard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-15 23:29:00.000000 memento-scorecard-0.8.1/memento_scorecard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 23:29:01.109858 memento-scorecard-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     1433 2023-06-07 21:36:49.000000 memento-scorecard-0.8.1/setup.py
```

### Comparing `memento-scorecard-0.7.2/LICENSE` & `memento-scorecard-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `memento-scorecard-0.7.2/PKG-INFO` & `memento-scorecard-0.8.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memento-scorecard
-Version: 0.7.2
+Version: 0.8.1
 Summary: Scorecard development with Python
 Home-page: https://github.com/Guilliu/Memento
 Author: Guillermo Lizcano Villafáñez
 Author-email: guille.lv.97@gmail.com
 License: Apache License 2.0
 Keywords: python,scoring,rating,logistic,regression,scorecard,woe,credit-risk,autogrouping
 Platform: UNKNOWN
```

### Comparing `memento-scorecard-0.7.2/memento/__init__.py` & `memento-scorecard-0.8.1/memento/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from memento.princess_carolyn import (compute_final_breakpoints,
 compute_info, features_selection, display_table_ng, reagrupa_var)
 from memento.mr_peanutbutter import (pretty_scorecard, parceling, cell_style,
 predict_pyspark, metrics_pyspark, compute_pyspark_ks, save_model,
 save_light_model, load_model, genera_punt_par, proc_freq)
 from memento.bojack import scorecard, autogrouping
 
-__version__ = '0.7.2'
+__version__ = '0.8.1'
 
 __all__ = (
     string_categories1, string_categories2, string_to_num,
     breakpoints_to_str, breakpoints_to_num, remapeo_missing, data_convert, adapt_data,
     compute_group_names, compute_table, transform_to_woes,
     calib_score, compute_scorecard, transform_to_points, apply_scorecard, compute_metrics,
     compute_final_breakpoints,
```

### Comparing `memento-scorecard-0.7.2/memento/bojack.py` & `memento-scorecard-0.8.1/memento/bojack.py`

 * *Files 1% similar despite different names*

```diff
@@ -460,38 +460,38 @@
             else: 
                 raise Exception('WTF, qué tipo de datos tiene {}: '\
                 .format(feature), str(objeto.dtype))
             texto += '<DataField name="{}" dataType="{}" optype="{}"/>\n'\
             .format(feature, tipo1, tipo2)
         
         min_score = min(self.scorecard['Aligned score'])
-        texto += '<DataField name="{}" dataType="integer" \
-        optype="continuous"/>\n'.format(score_name)
+        texto += '<DataField name="{}" dataType="integer" ' +\
+        'optype="continuous"/>\n'.format(score_name)
         texto += '</DataDictionary>\n'
         if reasons_code:
-            texto += '<Scorecard modelName="{}" functionName="regression" initialScore="0" \
-            useReasonCodes="true" reasonCodeAlgorithm="pointsAbove" \
-            baselineScore="{}">\n'.format(nombre_modelo, min_score)
+            texto += '<Scorecard modelName="{}" functionName="regression" initialScore="0" ' +\
+            'useReasonCodes="true" reasonCodeAlgorithm="pointsAbove" ' +\
+            'baselineScore="{}">\n'.format(nombre_modelo, min_score)
         else:
-            texto += '<Scorecard modelName="{}" functionName="regression" \
-            initialScore="0" useReasonCodes="false">\n'.format(nombre_modelo, min_score)
+            texto += '<Scorecard modelName="{}" functionName="regression" ' +\
+            'initialScore="0" useReasonCodes="false">\n'.format(nombre_modelo, min_score)
         texto += '<MiningSchema>\n'
 
         for feature in self.features:
-            texto += '<MiningField name="{}" usageType="active" \
-            invalidValueTreatment="asMissing"/>\n'.format(feature)
+            texto += '<MiningField name="{}" usageType="active" ' +\
+            'invalidValueTreatment="asMissing"/>\n'.format(feature)
 
         texto += '<MiningField name="{}" usageType="predicted"/>\n'.format(score_name)
         texto += '</MiningSchema>\n'
         if reasons_code:
             texto += '<Output>\n'
             contador = 1
             for i in self.features:
-                texto += '<OutputField name="reasoncode_{}" rank="{}" feature="reasonCode"\
-                dataType="string" optype="categorical"/>\n'.format(contador, contador)
+                texto += '<OutputField name="reasoncode_{}" rank="{}" feature="reasonCode" ' +\
+                'dataType="string" optype="categorical"/>\n'.format(contador, contador)
                 contador += 1
             texto += '</Output>\n'     
         texto += '<Characteristics>\n'
         contador = 1
         for i in self.features:
             
             contador += 1
@@ -509,40 +509,40 @@
                 if self.autogroupings[i].dtype not in ('object', 'bool'):
   
                     if 'Missing' in groups[j]:
                         if len(groups[j]) > 7: aux += '<CompoundPredicate booleanOperator="or">\n'
                         aux += '<SimplePredicate field="{}" operator="isMissing"/>\n'.format(i)
                     if 'inf)' not in groups[j] and groups[j] != 'Missing':
                         lim = groups[j].split(', ')[1][:-1]
-                        aux += '<SimplePredicate field="{}" operator="lessThan" \
-                        value="{}"/>\n'.format(i, lim)
+                        aux += '<SimplePredicate field="{}" operator="lessThan" ' +\
+                        'value="{}"/>\n'.format(i, lim)
                     if 'inf)' in groups[j]:
                         lim = groups[j].split(', ')[0][1:]
-                        aux += '<SimplePredicate field="{}" operator="greaterOrEqual" \
-                        value="{}"/>\n'.format(i, lim)
+                        aux += '<SimplePredicate field="{}" operator="greaterOrEqual" ' +\
+                        'value="{}"/>\n'.format(i, lim)
                     if 'Missing' in groups[j] and len(groups[j]) > 7:
                         aux += '</CompoundPredicate>\n'
         
                 else:
                 
                     if len(groups[j]) > 1:
                         aux += '<CompoundPredicate booleanOperator="or">\n'
                     for k in groups[j]:
                         if k != 'Missing':
-                            aux += '<SimplePredicate field="{}" operator="equal" \
-                            value="{}"/>\n'.format(i, k)
+                            aux += '<SimplePredicate field="{}" operator="equal" ' +\
+                            'value="{}"/>\n'.format(i, k)
                         else:
                             aux += '<SimplePredicate field="{}" operator="isMissing"/>\n'.format(i)
                     if len(groups[j]) > 1:
                         aux += '</CompoundPredicate>\n'
             
                 aux += '</Attribute>\n'
             if reasons_code: 
-                aux += '<Attribute partialScore="{}" \
-                reasonCode="{}_{}">\n'.format(min(points), i, 404)
+                aux += '<Attribute partialScore="{}" ' +\
+                'reasonCode="{}_{}">\n'.format(min(points), i, 404)
             else: aux += '<Attribute partialScore="{}">\n'.format(min(points))
             aux += '<True/>\n'
             aux += '</Attribute>\n'
             aux += '</Characteristic>\n'
             texto += aux
         texto += '</Characteristics>\n'
         texto += '</Scorecard>\n'
```

### Comparing `memento-scorecard-0.7.2/memento/diane.py` & `memento-scorecard-0.8.1/memento/diane.py`

 * *Files identical despite different names*

### Comparing `memento-scorecard-0.7.2/memento/mr_peanutbutter.py` & `memento-scorecard-0.8.1/memento/mr_peanutbutter.py`

 * *Files identical despite different names*

### Comparing `memento-scorecard-0.7.2/memento/princess_carolyn.py` & `memento-scorecard-0.8.1/memento/princess_carolyn.py`

 * *Files identical despite different names*

### Comparing `memento-scorecard-0.7.2/memento/todd.py` & `memento-scorecard-0.8.1/memento/todd.py`

 * *Files identical despite different names*

### Comparing `memento-scorecard-0.7.2/memento_scorecard.egg-info/PKG-INFO` & `memento-scorecard-0.8.1/memento_scorecard.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memento-scorecard
-Version: 0.7.2
+Version: 0.8.1
 Summary: Scorecard development with Python
 Home-page: https://github.com/Guilliu/Memento
 Author: Guillermo Lizcano Villafáñez
 Author-email: guille.lv.97@gmail.com
 License: Apache License 2.0
 Keywords: python,scoring,rating,logistic,regression,scorecard,woe,credit-risk,autogrouping
 Platform: UNKNOWN
```

### Comparing `memento-scorecard-0.7.2/setup.py` & `memento-scorecard-0.8.1/setup.py`

 * *Files identical despite different names*

