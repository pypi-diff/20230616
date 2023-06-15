# Comparing `tmp/memento-scorecard-0.2.7.tar.gz` & `tmp/memento-scorecard-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memento-scorecard-0.2.7.tar", last modified: Wed Jun  7 21:40:12 2023, max compression
+gzip compressed data, was "memento-scorecard-0.7.2.tar", last modified: Thu Jun 15 23:20:18 2023, max compression
```

## Comparing `memento-scorecard-0.2.7.tar` & `memento-scorecard-0.7.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 21:40:12.456616 memento-scorecard-0.2.7/
--rw-rw-rw-   0        0        0    11558 2023-06-07 21:33:58.000000 memento-scorecard-0.2.7/LICENSE
--rw-rw-rw-   0        0        0     1157 2023-06-07 21:40:12.454006 memento-scorecard-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0       46 2023-06-07 21:33:58.000000 memento-scorecard-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 21:40:12.443029 memento-scorecard-0.2.7/memento/
--rw-rw-rw-   0        0        0     1144 2023-06-07 21:37:46.000000 memento-scorecard-0.2.7/memento/__init__.py
--rw-rw-rw-   0        0        0    20799 2023-06-07 14:51:04.000000 memento-scorecard-0.2.7/memento/bojack.py
--rw-rw-rw-   0        0        0     7612 2023-06-07 14:48:04.000000 memento-scorecard-0.2.7/memento/diane.py
--rw-rw-rw-   0        0        0    15680 2023-06-07 14:48:05.000000 memento-scorecard-0.2.7/memento/mr_peanutbutter.py
--rw-rw-rw-   0        0        0    23651 2023-06-07 14:48:05.000000 memento-scorecard-0.2.7/memento/princess_carolyn.py
--rw-rw-rw-   0        0        0     3241 2023-06-07 14:48:03.000000 memento-scorecard-0.2.7/memento/todd.py
-drwxrwxrwx   0        0        0        0 2023-06-07 21:40:12.452047 memento-scorecard-0.2.7/memento_scorecard.egg-info/
--rw-rw-rw-   0        0        0     1157 2023-06-07 21:40:12.000000 memento-scorecard-0.2.7/memento_scorecard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-06-07 21:40:12.000000 memento-scorecard-0.2.7/memento_scorecard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 21:40:12.000000 memento-scorecard-0.2.7/memento_scorecard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-07 21:40:12.000000 memento-scorecard-0.2.7/memento_scorecard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 21:40:12.456616 memento-scorecard-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1433 2023-06-07 21:36:49.000000 memento-scorecard-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-15 23:20:18.909085 memento-scorecard-0.7.2/
+-rw-rw-rw-   0        0        0    11558 2023-06-07 21:33:58.000000 memento-scorecard-0.7.2/LICENSE
+-rw-rw-rw-   0        0        0     1157 2023-06-15 23:20:18.906576 memento-scorecard-0.7.2/PKG-INFO
+-rw-rw-rw-   0        0        0       46 2023-06-07 21:33:58.000000 memento-scorecard-0.7.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-15 23:20:18.887353 memento-scorecard-0.7.2/memento/
+-rw-rw-rw-   0        0        0     1384 2023-06-15 23:20:12.000000 memento-scorecard-0.7.2/memento/__init__.py
+-rw-rw-rw-   0        0        0    28736 2023-06-15 23:13:37.000000 memento-scorecard-0.7.2/memento/bojack.py
+-rw-rw-rw-   0        0        0     7582 2023-06-15 23:06:58.000000 memento-scorecard-0.7.2/memento/diane.py
+-rw-rw-rw-   0        0        0    20641 2023-06-15 23:07:02.000000 memento-scorecard-0.7.2/memento/mr_peanutbutter.py
+-rw-rw-rw-   0        0        0    23946 2023-06-15 23:07:00.000000 memento-scorecard-0.7.2/memento/princess_carolyn.py
+-rw-rw-rw-   0        0        0     3243 2023-06-15 23:06:56.000000 memento-scorecard-0.7.2/memento/todd.py
+drwxrwxrwx   0        0        0        0 2023-06-15 23:20:18.902112 memento-scorecard-0.7.2/memento_scorecard.egg-info/
+-rw-rw-rw-   0        0        0     1157 2023-06-15 23:20:18.000000 memento-scorecard-0.7.2/memento_scorecard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-06-15 23:20:18.000000 memento-scorecard-0.7.2/memento_scorecard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-15 23:20:18.000000 memento-scorecard-0.7.2/memento_scorecard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-15 23:20:18.000000 memento-scorecard-0.7.2/memento_scorecard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-15 23:20:18.909592 memento-scorecard-0.7.2/setup.cfg
+-rw-rw-rw-   0        0        0     1433 2023-06-07 21:36:49.000000 memento-scorecard-0.7.2/setup.py
```

### Comparing `memento-scorecard-0.2.7/LICENSE` & `memento-scorecard-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `memento-scorecard-0.2.7/PKG-INFO` & `memento-scorecard-0.7.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memento-scorecard
-Version: 0.2.7
+Version: 0.7.2
 Summary: Scorecard development with Python
 Home-page: https://github.com/Guilliu/Memento
 Author: Guillermo Lizcano Villafáñez
 Author-email: guille.lv.97@gmail.com
 License: Apache License 2.0
 Keywords: python,scoring,rating,logistic,regression,scorecard,woe,credit-risk,autogrouping
 Platform: UNKNOWN
```

### Comparing `memento-scorecard-0.2.7/memento/__init__.py` & `memento-scorecard-0.7.2/memento/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from memento.todd import (string_categories1, string_categories2, string_to_num,
 breakpoints_to_str, breakpoints_to_num, remapeo_missing, data_convert, adapt_data)
 from memento.diane import (compute_group_names, compute_table, transform_to_woes,
 calib_score, compute_scorecard, transform_to_points, apply_scorecard, compute_metrics)
 from memento.princess_carolyn import (compute_final_breakpoints,
 compute_info, features_selection, display_table_ng, reagrupa_var)
-from memento.mr_peanutbutter import pretty_scorecard, parceling, cell_style, proc_freq
+from memento.mr_peanutbutter import (pretty_scorecard, parceling, cell_style,
+predict_pyspark, metrics_pyspark, compute_pyspark_ks, save_model,
+save_light_model, load_model, genera_punt_par, proc_freq)
 from memento.bojack import scorecard, autogrouping
 
-__version__ = '0.2.7'
+__version__ = '0.7.2'
 
 __all__ = (
     string_categories1, string_categories2, string_to_num,
     breakpoints_to_str, breakpoints_to_num, remapeo_missing, data_convert, adapt_data,
     compute_group_names, compute_table, transform_to_woes,
     calib_score, compute_scorecard, transform_to_points, apply_scorecard, compute_metrics,
     compute_final_breakpoints,
     compute_info, features_selection, display_table_ng, reagrupa_var,
-    pretty_scorecard, parceling, cell_style, proc_freq,
+    pretty_scorecard, parceling, cell_style,
+    predict_pyspark, metrics_pyspark, compute_pyspark_ks, save_model,
+    save_light_model, load_model, genera_punt_par, proc_freq,
     scorecard, autogrouping
 )
```

### Comparing `memento-scorecard-0.2.7/memento/bojack.py` & `memento-scorecard-0.7.2/memento/bojack.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         flag_train_test=[],
 
         autogrp_all=False,
         autogrp_max_groups=5,
         autogrp_min_pct=0.05,
         autogrp_dict_max_groups={},
         autogrp_dict_min_pct={},
+        autogrp_dict_manual_types={},
 
         features=[],
         excluded_vars=[],
         included_vars=[],
 
         iv_threshold=0.015,
         selection_show = 'gini',
@@ -40,32 +41,34 @@
         selection_metric='pvalue',
         selection_threshold=0.01,
         selection_max_iters=14,
         selection_stop_ks_gini=True,
         selection_check_overfitting=True,
         
         user_breakpoints={},
+        logistic_method = 'newton',
 
         id_columns=[],
         save_tables='features',
         save_autogroupings='features'
-
+        
     ):
 
         self.test_seed = test_seed
         self.test_size = test_size
         self.stratify = stratify
         self.stratify_var = stratify_var
         self.flag_train_test = flag_train_test
         
         self.autogrp_all = autogrp_all
         self.autogrp_max_groups = autogrp_max_groups
         self.autogrp_min_pct = autogrp_min_pct
         self.autogrp_dict_max_groups = autogrp_dict_max_groups
         self.autogrp_dict_min_pct = autogrp_dict_min_pct
+        self.autogrp_dict_manual_types = autogrp_dict_manual_types
         
         self.features = features
         self.excluded_vars = excluded_vars
         self.included_vars = included_vars
         
         self.iv_threshold = iv_threshold
         self.selection_show = selection_show
@@ -73,19 +76,20 @@
         self.selection_metric = selection_metric
         self.selection_threshold = selection_threshold
         self.selection_max_iters = selection_max_iters
         self.selection_stop_ks_gini = selection_stop_ks_gini
         self.selection_check_overfitting = selection_check_overfitting
 
         self.user_breakpoints = user_breakpoints
-
+        self.logistic_method = logistic_method
+        
         self.id_columns = id_columns
         self.save_tables = save_tables
         self.save_autogroupings = save_autogroupings
-
+        
 
     def fit(self, X, y):
 
         ### INICIO PARTICIONADO
 
         if self.flag_train_test != []:
 
@@ -150,68 +154,65 @@
         if self.autogrp_all: variables = X.columns
         else: 
             if self.features != []: variables = self.features
             else: variables = list(set(list(X.columns)) - set(self.excluded_vars))
 
         autogroupings = {}
         variables_no_agrupadas_error = []
-        variables_no_agrupadas_raras = []
 
         for variable in variables:
 
             try:
                 
                 if variable in self.autogrp_dict_max_groups:
                     max_groups = self.autogrp_dict_max_groups[variable]
                 else: max_groups = self.autogrp_max_groups
 
                 if variable in self.autogrp_dict_min_pct:
                     min_pct = self.autogrp_dict_min_pct[variable]
                 else: min_pct = self.autogrp_min_pct
 
+                if variable in self.autogrp_dict_manual_types: 
+                    manual_type = self.autogrp_dict_manual_types[variable]
+                else: manual_type = ''
+
                 x = X_train[variable].values
-                frenken = autogrouping(max_groups=max_groups, min_pct=min_pct).fit(x, y_train)
+                frenken = autogrouping(max_groups=max_groups, 
+                min_pct=min_pct, manual_type=manual_type).fit(x, y_train)
 
-                if len(frenken.breakpoints_num) == 0: variables_no_agrupadas_raras.append(variable)
+                if len(frenken.breakpoints_num) == 0: variables_no_agrupadas_error.append(variable)
                 else: autogroupings[variable] = frenken
- 
+                
             except:
                 variables_no_agrupadas_error.append(variable)
 
         print('Autogrouping terminado. Máximo número de buckets = {}. Mínimo porcentaje '
         'por bucket = {}'.format(self.autogrp_max_groups, self.autogrp_min_pct))
         print('-' * N)
 
-        if len(variables_no_agrupadas_raras) > 0:
-            print('Variables no agrupadas por algún motivo extraño: {}'\
-            .format(variables_no_agrupadas_raras))
-            print('-' * N)
-
         if len(variables_no_agrupadas_error) > 0:
             print('Variables no agrupadas por algún error, seguramente por excesiva '
             'concentración en algún valor (> 95%) : {}'.format(variables_no_agrupadas_error))
             print('-' * N)
-
-        self.variables_no_agrupadas_raras = variables_no_agrupadas_raras
+            
         self.variables_no_agrupadas_error = variables_no_agrupadas_error
 
         tabla_ivs, contador = pd.DataFrame(columns=['variable', 'iv']), 0
         for variable in autogroupings:
             tabla_ivs.loc[contador] = variable, autogroupings[variable].iv
             contador += 1
         tabla_ivs = tabla_ivs.sort_values('iv', ascending=False).reset_index(drop=True)
 
         self.tabla_ivs = tabla_ivs
-
+        
         variables_filtro_iv = tabla_ivs[tabla_ivs['iv'] >= self.iv_threshold]['variable']
         
         if self.features != []: variables_def = self.features
         else:
-            variables_def = list(set(variables_filtro_iv) - 
-            set(variables_no_agrupadas_raras) - set(variables_no_agrupadas_error))
+            variables_def = list(set(variables_filtro_iv) - set(variables_no_agrupadas_error))
 
         self.final_breakpoints = compute_final_breakpoints(
         variables_def, autogroupings, self.user_breakpoints)
         info = compute_info(X_train, variables_def, self.final_breakpoints)
 
         df_train = adapt_data(X_train, y_train, variables_def, self.final_breakpoints)
         df_test = adapt_data(X_test, y_test, variables_def, self.final_breakpoints)
@@ -220,21 +221,23 @@
 
         features = features_selection(
         df_train, self.features, variables_def, info, 'target_4815162342',
         method=self.selection_method, metric=self.selection_metric,
         threshold=self.selection_threshold, stop_ks_gini=self.selection_stop_ks_gini,
         max_iters=self.selection_max_iters, included_vars=self.included_vars,
         muestra_test=df_test, show=self.selection_show, 
-        check_overfitting=self.selection_check_overfitting)
+        check_overfitting=self.selection_check_overfitting,
+        logistic_method=self.logistic_method)
 
         df_train = df_train[features + ['target_4815162342']]
         df_test = df_test[features + ['target_4815162342']]
 
         scorecard, features_length, pvalues, coefs = compute_scorecard(
-        df_train, features, info, pvalues=True, ret_coefs=True)
+        df_train, features, info, pvalues=True, 
+        ret_coefs=True, logistic_method=self.logistic_method)
 
         df_train_final = apply_scorecard(df_train, scorecard, info, 'target_4815162342')
         ks_train, gini_train = compute_metrics(df_train_final, 'target_4815162342', ['gini', 'ks'])
 
         print('El modelo tiene un {:.2f}% de KS y un {:.2f}% de Gini en '
         'la muestra de entrenamiento'.format(round(ks_train*100, 2), round(gini_train*100, 2)))
         print('-' * N)
@@ -266,20 +269,21 @@
 
         for objeto in autogroupings: del autogroupings[objeto].x_final
 
         if self.save_autogroupings == 'all': 
             self.autogroupings = autogroupings
         elif self.save_autogroupings == 'features':
             self.autogroupings = dict((k, autogroupings[k]) for k in features if k in autogroupings)
-
-        # self.pyspark_formula = compute_pyspark_formula(self)
+            
+        try: self.create_pyspark_formula()
+        except: self.pypsark_formula = ['Por algún motivo no se ha podido calcular la fórmula SQL']
 
         return self
-        
 
+        
     def create_excel(self, ruta, color='blue'):
         
         import openpyxl
         from openpyxl.utils.dataframe import dataframe_to_rows
         from openpyxl.styles import PatternFill
         
         scorecard = self.scorecard.copy()
@@ -381,15 +385,176 @@
                     for cell in row:
                         cell.fill = PatternFill(fill_type='solid', fgColor=color)
             contador = new_contador
             moneda += 1
             
         wb.save(ruta)
 
+    
+    def create_pyspark_formula(self):
+    
+        import copy
+
+        pyspark_formula = []
+
+        for i in self.features:
+
+            aux = 'CASE '
+            points = list(self.scorecard[self.scorecard['Variable'] == i]['Aligned score'])
+            groups = copy.deepcopy(list(self.scorecard[self.scorecard['Variable'] == i]['Group']))
+            
+            for j in range(len(groups)):
+
+                if self.autogroupings[i].dtype not in ('object', 'bool'):
+                    if 'Missing' in groups[j]:
+                        aux += 'WHEN (isnan({}) OR ({} IS NULL)) THEN {} '.format(i, i, points[j])
+                    if 'inf)' not in groups[j] and groups[j] != 'Missing':
+                        lim = groups[j].split(', ')[1][:-1]
+                        aux += 'WHEN {} < {} THEN {} '.format(i, lim, points[j])
+                    if 'inf)' in groups[j]:
+                        lim = groups[j].split(', ')[0][1:]
+                        aux += 'WHEN {} >= {} THEN {} '.format(i, lim, points[j])
+
+                else:
+                    if 'Missing' in groups[j]:
+                        todos = [aaa for bbb in groups for aaa in bbb] # CAMBIAR
+                        if True in todos or False in todos: # CAMBIAR
+                            aux += 'WHEN {} IS NULL THEN {} '.format(i, points[j]) # CAMBIAR
+                        else: # CAMBIAR
+                            aux += 'WHEN (isnan({}) OR ({} IS NULL)) THEN {} '\
+                            .format(i, i, points[j]) # CAMBIAR
+                    try: groups[j].remove('Missing')
+                    except: pass
+                    if groups[j] != []: 
+                        aux += 'WHEN {} IN {} THEN {} '.format(i, groups[j], points[j])
+
+            aux += 'ELSE {} END'.format(min(points))
+            aux = aux.replace('[', '(').replace(']', ')')
+
+            pyspark_formula.append(aux)
+        
+        self.pyspark_formula = pyspark_formula
 
+        
+    def create_pmml(self, nombre_archivo, 
+    nombre_modelo='mew', score_name='scorecardpoints', reasons_code=True):
+
+        import copy
+
+        texto = '<PMML xmlns="http://www.dmg.org/PMML-4_4" version="4.4">\n'
+        texto += '<DataDictionary>\n'
+
+        for feature in self.features:
+            objeto = self.autogroupings[feature]
+            if 'int' in str(objeto.dtype): 
+                tipo1 = 'integer'
+                tipo2 = 'continuous'
+            elif 'float' in str(objeto.dtype): 
+                tipo1 = 'double'
+                tipo2 = 'continuous'
+            elif 'object' in str(objeto.dtype): 
+                tipo1 = 'string'
+                tipo2 = 'categorical'
+            elif 'bool' in str(objeto.dtype): 
+                tipo1 = 'boolean'
+                tipo2 = 'categorical'
+            else: 
+                raise Exception('WTF, qué tipo de datos tiene {}: '\
+                .format(feature), str(objeto.dtype))
+            texto += '<DataField name="{}" dataType="{}" optype="{}"/>\n'\
+            .format(feature, tipo1, tipo2)
+        
+        min_score = min(self.scorecard['Aligned score'])
+        texto += '<DataField name="{}" dataType="integer" \
+        optype="continuous"/>\n'.format(score_name)
+        texto += '</DataDictionary>\n'
+        if reasons_code:
+            texto += '<Scorecard modelName="{}" functionName="regression" initialScore="0" \
+            useReasonCodes="true" reasonCodeAlgorithm="pointsAbove" \
+            baselineScore="{}">\n'.format(nombre_modelo, min_score)
+        else:
+            texto += '<Scorecard modelName="{}" functionName="regression" \
+            initialScore="0" useReasonCodes="false">\n'.format(nombre_modelo, min_score)
+        texto += '<MiningSchema>\n'
+
+        for feature in self.features:
+            texto += '<MiningField name="{}" usageType="active" \
+            invalidValueTreatment="asMissing"/>\n'.format(feature)
+
+        texto += '<MiningField name="{}" usageType="predicted"/>\n'.format(score_name)
+        texto += '</MiningSchema>\n'
+        if reasons_code:
+            texto += '<Output>\n'
+            contador = 1
+            for i in self.features:
+                texto += '<OutputField name="reasoncode_{}" rank="{}" feature="reasonCode"\
+                dataType="string" optype="categorical"/>\n'.format(contador, contador)
+                contador += 1
+            texto += '</Output>\n'     
+        texto += '<Characteristics>\n'
+        contador = 1
+        for i in self.features:
+            
+            contador += 1
+            aux = '<Characteristic name="{}">\n'.format(i)
+            points = list(self.scorecard[self.scorecard['Variable'] == i]['Aligned score'])
+            groups = copy.deepcopy(list(self.scorecard[self.scorecard['Variable'] == i]['Group']))
+            
+            for j in range(len(points)):
+                
+                if reasons_code: 
+                    aux += '<Attribute partialScore="{}" \
+                    reasonCode="{}_{}">\n'.format(points[j], i, j+1)
+                else: aux += '<Attribute partialScore="{}">\n'.format(points[j])
+                
+                if self.autogroupings[i].dtype not in ('object', 'bool'):
+  
+                    if 'Missing' in groups[j]:
+                        if len(groups[j]) > 7: aux += '<CompoundPredicate booleanOperator="or">\n'
+                        aux += '<SimplePredicate field="{}" operator="isMissing"/>\n'.format(i)
+                    if 'inf)' not in groups[j] and groups[j] != 'Missing':
+                        lim = groups[j].split(', ')[1][:-1]
+                        aux += '<SimplePredicate field="{}" operator="lessThan" \
+                        value="{}"/>\n'.format(i, lim)
+                    if 'inf)' in groups[j]:
+                        lim = groups[j].split(', ')[0][1:]
+                        aux += '<SimplePredicate field="{}" operator="greaterOrEqual" \
+                        value="{}"/>\n'.format(i, lim)
+                    if 'Missing' in groups[j] and len(groups[j]) > 7:
+                        aux += '</CompoundPredicate>\n'
+        
+                else:
+                
+                    if len(groups[j]) > 1:
+                        aux += '<CompoundPredicate booleanOperator="or">\n'
+                    for k in groups[j]:
+                        if k != 'Missing':
+                            aux += '<SimplePredicate field="{}" operator="equal" \
+                            value="{}"/>\n'.format(i, k)
+                        else:
+                            aux += '<SimplePredicate field="{}" operator="isMissing"/>\n'.format(i)
+                    if len(groups[j]) > 1:
+                        aux += '</CompoundPredicate>\n'
+            
+                aux += '</Attribute>\n'
+            if reasons_code: 
+                aux += '<Attribute partialScore="{}" \
+                reasonCode="{}_{}">\n'.format(min(points), i, 404)
+            else: aux += '<Attribute partialScore="{}">\n'.format(min(points))
+            aux += '<True/>\n'
+            aux += '</Attribute>\n'
+            aux += '</Characteristic>\n'
+            texto += aux
+        texto += '</Characteristics>\n'
+        texto += '</Scorecard>\n'
+        texto += '</PMML>'
+        
+        with open('{}'.format(nombre_archivo), 'w') as f: f.write(texto)
+    
+        
     def predict(self, data, target_name='', keep_columns=[], binary_treshold=0.0):
                    
         if target_name != '': X1 = data[keep_columns + self.features + [target_name]].copy()
         else: X1 = data[keep_columns + self.features].copy()
 
         X1_v2, info = X1.copy(), {}
         for feature in self.features:
@@ -405,15 +570,16 @@
 
             else:
                 X1_v2[feature] = remapeo_missing(data_convert(
                 X1[feature].values, string_categories2(bp))[3], bp)
                 info[feature]['breakpoints_num'] = breakpoints_to_num(bp['bp'])
                 info[feature]['group_names'] = compute_group_names(
                 X1[feature].values.dtype, bp['bp'], bp['mg'])
-
+                
+        X1_v2 = X1_v2.reset_index(drop=True)
         X2 = apply_scorecard(X1_v2, self.scorecard, info, 
         target_name=target_name, binary_treshold=binary_treshold)
 
         venga = 0
         for i in X2.columns:
             if 'scr_' in i:
                 break
@@ -423,23 +589,25 @@
 
         return X1
         
 
 class autogrouping:
 
 
-    def __init__(self, max_groups=5, min_pct=0.05):
+    def __init__(self, max_groups=5, min_pct=0.05, manual_type=''):
 
         self.max_groups = max_groups
         self.min_pct = min_pct
+        self.manual_type = manual_type
 
 
     def fit(self, x, y):
-
-        dtype = x.dtype
+        
+        if self.manual_type != '': dtype = self.manual_type
+        else: dtype = x.dtype
 
         if dtype not in ('O', 'bool'): categories = {}
 
         else:
 
             categories = string_categories1(x, y)
```

### Comparing `memento-scorecard-0.2.7/memento/diane.py` & `memento-scorecard-0.7.2/memento/diane.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,16 +84,14 @@
         table.loc['Totals'] = ['', total_e, 1, total_g, total_b, total_b_rate, '', total_iv]
 
     return table, total_iv
 
 
 def transform_to_woes(x, y, breakpoints_num):
 
-    ''' Transforma a woes los valores de una columna numérica dado sus breakpoints. '''
-
     x_groups = np.digitize(x, breakpoints_num)
 
     ngroups = len(breakpoints_num) + 1
     g = np.empty(ngroups).astype(np.int64)
     b = np.empty(ngroups).astype(np.int64)
 
     for i in range(ngroups):
@@ -125,15 +123,15 @@
 
     new_points = -(points + intercept / n) * factor + offset / n
 
     return new_points
 
 
 def compute_scorecard(data, features, info, target_name='target_4815162342',
-pvalues=False, ret_coefs=False, redondeo=True):
+pvalues=False, ret_coefs=False, redondeo=True, logistic_method='newton'):
 
     X = data.drop(target_name, axis=1).copy()
     y = data[target_name].values
 
     Xwoes = pd.DataFrame()
     scorecard, features_length = pd.DataFrame(), np.array([], 'int64')
 
@@ -146,15 +144,15 @@
         table = compute_table(x, y, breakpoints_num, group_names, False)[0]
         table.insert(0, 'Variable', feature)
         scorecard = pd.concat([scorecard, table])
         features_length = np.append(features_length, len(table))
 
         Xwoes[feature] = transform_to_woes(x, y, breakpoints_num)
 
-    log_reg = sm.Logit(y, sm.add_constant(Xwoes.values)).fit(method='lbfgs')
+    log_reg = sm.Logit(y, sm.add_constant(Xwoes.values)).fit(method=logistic_method, disp=0)
     coefs, intercept = np.array([log_reg.params[1:]]), np.array([log_reg.params[0]])
 
     scorecard['Raw score'] = scorecard['WoE'] * np.repeat(coefs.ravel(), features_length)
     scorecard['Aligned score'] = calib_score(scorecard['Raw score'], len(features), intercept)
     if redondeo: scorecard['Aligned score'] = scorecard['Aligned score'].round().astype('int')
     scorecard = scorecard.reset_index(drop=True)
 
@@ -165,67 +163,68 @@
 
 
 def transform_to_points(x, breakpoints_num, mapeo_points):
 
     return pd.Series([mapeo_points[i] for i in np.digitize(x, breakpoints_num)])
 
 
-def apply_scorecard(data, scorecard, info, target_name='', binary_treshold=0.0):
+def apply_scorecard(data, scorecard, info, target_name='',
+binary_treshold=0.0, score_name='scorecardpoints'):
 
     features = list(scorecard['Variable'].unique())
     if target_name != '': columnas = features + [target_name]
     else: columnas = features
                  
     data_final = data[columnas].copy()
     data_final = data.copy()
-    data_final['scorecardpoints'] = 0
+    data_final[score_name] = 0
 
     for feature in features:
 
         x = data_final[feature]
         breakpoints_num = info[feature]['breakpoints_num']
 
         mapeo_points = scorecard[scorecard['Variable'] == feature]\
         .reset_index(drop=True)['Aligned score'].to_dict()
 
         data_final['scr_{}'.format(feature)] = \
         transform_to_points(x, breakpoints_num, mapeo_points)
-        data_final['scorecardpoints'] += data_final['scr_{}'.format(feature)]
+        data_final[score_name] += data_final['scr_{}'.format(feature)]
     
     columnas = list(data_final.columns)
-    columnas.remove('scorecardpoints')
-    data_final = data_final[columnas + ['scorecardpoints']]
+    columnas.remove(score_name)
+    data_final = data_final[columnas + [score_name]]
 
     if binary_treshold != 0.0:
-        data_final['prediction'] = np.where(data_final.scorecardpoints >= binary_treshold, 0, 1)
+        data_final['prediction'] = np.where(data_final[score_name] >= binary_treshold, 0, 1)
 
     return data_final
 
-def compute_metrics(data, target_name, metrics, print_log=False):
+def compute_metrics(data, target_name, metrics, print_log=False, score_name='scorecardpoints'):
 
     if metrics not in (['ks'], ['gini'], ['ks', 'gini'], ['gini', 'ks']):
-        raise ValueError("Wrong value for 'metrics'. The values "
-        "allowed are: ['ks'], ['gini'], ['ks', 'gini'], ['gini', 'ks']")
+        raise ValueError("Valor erroneo para 'metrics'. Los valores "
+        "váidos son: ['ks'], ['gini'], ['ks', 'gini'], ['gini', 'ks']")
 
     if 'ks' in metrics:
-        g = data.loc[data[target_name] == 0, 'scorecardpoints']
-        b = data.loc[data[target_name] == 1, 'scorecardpoints']
+        g = data.loc[data[target_name] == 0, score_name]
+        b = data.loc[data[target_name] == 1, score_name]
         ks = ks_2samp(g, b)[0]
 
     if 'gini' in metrics:
-        gini = abs(2*(1 - roc_auc_score(data[target_name], data['scorecardpoints'])) - 1)
+        gini = abs(2*(1 - roc_auc_score(data[target_name], data[score_name])) - 1)
 
     if metrics == ['ks']:
         if print_log:
-            print('The model has a {:.2f}% of KS in this sample'.format(round(ks*100, 2)))
+            print('El modelo tiene un {:.2f}% de KS en esta muestra'.format(round(ks*100, 2)))
         return ks
 
     if metrics == ['gini']:
         if print_log:
-            print('The model has a {:.2f}% of Gini in this sample'.format(round(gini*100, 2), ))
+            print('El modelo tiene un {:.2f}% de Gini en esta muestra'.format(round(gini*100, 2), ))
         return gini
 
     if metrics in (['ks', 'gini'], ['gini', 'ks']):
         if print_log:
             print('El  modelo tiene un {:.2f}% de KS y un {:.2f}% de Gini '
             'en esta muestra'.format(round(ks*100, 2), round(gini*100, 2)))
         return ks, gini
```

### Comparing `memento-scorecard-0.2.7/memento/mr_peanutbutter.py` & `memento-scorecard-0.7.2/memento/mr_peanutbutter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import numpy as np, pandas as pd
 
 ####################################################################################################
 
 
 def pretty_scorecard(modelo, color1='blue', color2='#FFFFFF'):
     
-    from IPython.display import display
-
     if color1 == 'green': color1 = '#CCFFCC'
     if color1 == 'light_blue': color1 = '#CCFFFF'
     if color1 == 'blue': color1 = '#CCECFF'
     if color1 == 'pink': color1 = '#FFCCFF'
     if color1 == 'red': color1 = '#FFCCCC'
     if color1 == 'yellow': color1 = '#FFFFCC'
     if color1 == 'purple': color1 = '#CCCCFE'
@@ -100,14 +98,154 @@
     vertical=ver_alignment, wrap_text=wrap_text)
     cell.border = Border(left=Side(border_style=left_border, color=left_border_color),
     right=Side(border_style=right_border, color=right_border_color),
     top=Side(border_style=top_border, color=top_border_color),
     bottom=Side(border_style=bottom_border, color=bottom_border_color))
 
 
+def predict_pyspark(data, features, pyspark_formula,
+target_name='', keep_columns=[], binary_treshold=0.0, score_name='scorecardpoints'):
+            
+    import pyspark.sql.functions as sf
+    from pyspark.sql.types import IntegerType
+    
+    if target_name != '': X1 = data.select(keep_columns + features + [target_name])
+    else: X1 = data.select(keep_columns + features)
+            
+    X1 = X1.withColumn(score_name, sf.lit(0).cast(IntegerType()))
+
+    for i in range(len(pyspark_formula)):
+        X1 = X1.withColumn('scr_{}'.format(features[i]), 
+        sf.expr(pyspark_formula[i])).withColumn(score_name,
+        sf.col(score_name) + sf.col('scr_{}'.format(features[i])))
+
+    if binary_treshold != 0.0:
+        X1 = X1.withColumn('prediction',
+        sf.when(sf.col(score_name) >= binary_treshold, 0).otherwise(1))
+
+    columnas = list(X1.columns).copy()
+    columnas.remove(score_name)
+    if binary_treshold != 0.0: columnas.remove('prediction')
+    columnas += [score_name]
+    if binary_treshold != 0.0: columnas += ['prediction']
+    X1 = X1.select(columnas)
+
+    return X1
+
+
+def metrics_pyspark(data, target_name, metrics, print_log=False, score_name='scorecardpoints'):
+    
+    import pyspark.sql.functions as sf
+    from pyspark.sql.types import DoubleType
+    from pyspark.ml.evaluation import BinaryClassificationEvaluator
+
+    if metrics not in (['ks'], ['gini'], ['ks', 'gini'], ['gini', 'ks']):
+        raise ValueError("Valor erroneo para 'metrics'. Los valores "
+        "váidos son: ['ks'], ['gini'], ['ks', 'gini'], ['gini', 'ks']")
+
+    if 'ks' in metrics:
+        ks = compute_pyspark_ks(data.withColumn(score_name,
+        sf.col(score_name).cast(DoubleType())), target_name, score_name)
+
+    if 'gini' in metrics:
+        evaluator = BinaryClassificationEvaluator(rawPredictionCol=score_name,
+        labelCol=target_name, metricName='areaUnderROC')
+        auroc = evaluator.evaluate(data.withColumn(
+        score_name, sf.col(score_name).cast(DoubleType())))
+        gini = 1 - 2 * auroc
+
+    if metrics == ['ks']:
+        if print_log:
+            print('El modelo tiene un {:.2f}% de KS en esta muestra'.format(round(ks*100, 2)))
+        return ks
+
+    if metrics == ['gini']:
+        if print_log:
+            print('El modelo tiene un {:.2f}% de Gini en esta muestra'.format(round(gini*100, 2), ))
+        return gini
+
+    if metrics in (['ks', 'gini'], ['gini', 'ks']):
+        if print_log:
+            print('El  modelo tiene un {:.2f}% de KS y un {:.2f}% de Gini '
+            'en esta muestra'.format(round(ks*100, 2), round(gini*100, 2)))
+        return ks, gini
+    
+    
+def compute_pyspark_ks(df, target, score):
+    
+    import pyspark.sql.functions as sf
+    from pyspark.ml.feature import Bucketizer
+    
+    df = df.withColumn(score, sf.round(sf.col(score), 3))
+    minimo = df.agg({score: 'min'}).collect()[0][0]
+    maximo = df.agg({score: 'max'}).collect()[0][0]
+    bins = np.arange(minimo, maximo + 0.001, np.round((maximo - minimo) / 1000, 3))
+    bins[0] = -float('inf')
+    bins[len(bins) -1 ] = float('inf')
+
+    bucketizer = Bucketizer(splits=list(bins), inputCol=score, outputCol='buckets')
+    bucketed = bucketizer.setHandleInvalid('keep').transform(df)
+    pre_pivot = bucketed.groupby('buckets', target).count().toPandas()
+    pivot_table = pre_pivot.pivot_table(values='count', columns=target, index='buckets').fillna(0)
+    pivot_table['pct_ceros'] = pivot_table.iloc[:, 0] / np.sum(pivot_table.iloc[:, 0].values)
+    pivot_table['pct_unos'] = pivot_table.iloc[:, 1] / np.sum(pivot_table.iloc[:, 1].values)
+    pivot_table['pct_ceros_cum'] = pivot_table['pct_ceros'].cumsum()
+    pivot_table['pct_unos_cum'] = pivot_table['pct_unos'].cumsum()
+    pivot_table['KS'] = (pivot_table['pct_ceros_cum'] - pivot_table['pct_unos_cum']).abs()
+    KS = pivot_table['KS'].max()
+
+    return KS
+    
+
+def save_model(modelo, name):
+
+    import _pickle
+
+    pickle_file = open(name, 'wb')
+    _pickle.dump(modelo, pickle_file)
+    pickle_file.close()
+    
+    
+def save_light_model(modelo, name):
+
+    import _pickle
+
+    light_model = {
+        'features': modelo.features,
+        'pyspark_formula': modelo.pyspark_formula,
+        }
+
+    pickle_file = open(name, 'wb')
+    _pickle.dump(light_model, pickle_file)
+    pickle_file.close()
+    
+    
+def load_model(name):
+
+    import _pickle
+
+    pickle_file = open(name, 'rb')
+    obj = _pickle.load(pickle_file)
+    pickle_file.close()
+    
+    return obj
+
+
+def genera_punt_par(df, features):
+    
+    import pyspark.sql.functions as sf
+    
+    for feature in features:
+        condition = 'sf'
+        for rc in [i for i in dfOut.columns if 'reasoncode_' in i]:
+            condition += ".when(sf.col('{}').contains('{}'), sf.col('{}'))".format(rc, feature, rc)
+        df = df.withColumn('grp_{}'.format(feature), eval(condition))
+    
+    return df
+
 
 def proc_freq(data, row, col='', weight='', decimals=None, cumulative=False,
 sort_col='', sort_dir='', option='', values=[], output=None):
 
     '''
     Generates the frequency table of a variable in a DataFrame. If two variables are passed,
     inside the 'row' and 'col' parameters, then it computes their crosstab.
```

### Comparing `memento-scorecard-0.2.7/memento/princess_carolyn.py` & `memento-scorecard-0.7.2/memento/princess_carolyn.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,16 @@
                 X[variable].values.dtype, bp['bp'], bp['mg'])
                 
     return info
 
 
 def features_selection(data, features, var_list, info, target_name='target_4815162342',
 method='stepwise', metric='pvalue', threshold=0.01, stop_ks_gini=True, 
-max_iters=14, included_vars=[], muestra_test=None, show='gini', check_overfitting=True):
+max_iters=14, included_vars=[], muestra_test=None, show='gini',
+check_overfitting=True, logistic_method='newton'):
     
     # if log_file: file_prints = open('log_modelo.txt', 'a')
     # else: file_prints = None
 
     if features != []: included_vars, max_iters = features, 0
 
     if method not in ('forward', 'stepwise'):
@@ -66,15 +67,15 @@
     if check_overfitting:
         
         posible_sobreajuste = []
         for var in var_list:
             
             try:
                 scorecard, features_length = compute_scorecard(
-                data, [var], info, target_name=target_name)
+                data, [var], info, target_name=target_name, logistic_method=logistic_method)
                 data_final = apply_scorecard(data, scorecard, info, target_name)
                 gini_train = compute_metrics(data_final, target_name, ['gini'])
                 if not isinstance(muestra_test, type(None)):
                     test_final = apply_scorecard(muestra_test, scorecard, info, target_name)
                     gini_test = compute_metrics(test_final, target_name, ['gini'])
                 if gini_test + 0.25 < gini_train:
                     posible_sobreajuste.append(var)
@@ -96,15 +97,15 @@
 
             new_var = included_vars.pop(0)
             features.append(new_var)
 
             if metric == 'pvalue':
 
                 scorecard, features_length, pvalues = compute_scorecard(
-                data, features, info, target_name=target_name, pvalues=True)
+                data, features, info, target_name=target_name, pvalues=True, logistic_method=logistic_method)
                 train_final = apply_scorecard(data, scorecard, info, target_name)
                 ks_train, gini_train = compute_metrics(train_final, target_name, ['ks', 'gini'])
                 if not isinstance(muestra_test, type(None)):
                     test_final = apply_scorecard(muestra_test, scorecard, info, target_name)
                     ks_test, gini_test = compute_metrics(test_final, target_name, ['ks', 'gini'])
                 
                 if pvalues[-1] < 1e-100: pvalorcito = 0
@@ -141,15 +142,15 @@
                         '| KS test = {:.2f}% | Gini train = {:.2f}% | Gini test '
                         '= {:.2f}% ---> Feature selected: {}'.format(str(i+1).zfill(2), pvalorcito,
                          ks_train*100, ks_test*100, gini_train*100, gini_test*100, new_var)) 
 
             else:
 
                 scorecard, features_length = compute_scorecard(
-                data, features, info, target_name=target_name)
+                data, features, info, target_name=target_name, logistic_method=logistic_method)
                 train_final = apply_scorecard(data, scorecard, info, target_name)
                 ks_train, gini_train = compute_metrics(train_final, target_name, ['ks', 'gini'])
                 if not isinstance(muestra_test, type(None)):
                     test_final = apply_scorecard(muestra_test, scorecard, info, target_name)
                     ks_test, gini_test = compute_metrics(test_final, target_name, ['ks', 'gini'])
 
                 if isinstance(muestra_test, type(None)):
@@ -195,27 +196,27 @@
                 
                 for var in var_list:
 
                     if var not in features:
 
                         features.append(var)
                         scorecard, features_length = compute_scorecard(
-                        data, features, info, target_name=target_name)
+                        data, features, info, target_name=target_name, logistic_method=logistic_method)
                         data_final = apply_scorecard(data, scorecard, info, target_name)
                         metrica = compute_metrics(data_final, target_name, [metric])
                         aux.loc[contador] = [var, metrica]
                         features.pop()
                         contador += 1
 
                 aux = aux.sort_values('metric', ascending=False)
                 new_var = aux.iloc[0]['var']
                 features.append(new_var)
 
                 scorecard, features_length = compute_scorecard(
-                data, features, info, target_name=target_name)
+                data, features, info, target_name=target_name, logistic_method=logistic_method)
                 train_final = apply_scorecard(data, scorecard, info, target_name)
                 ks_train, gini_train = compute_metrics(train_final, target_name, ['ks', 'gini'])
                 
                 if metric == 'ks':
                     if ks_train <= old_ks+0.0020:
                         print('-' * N)
                         print('En el siguiente paso el KS no sube '
@@ -280,15 +281,15 @@
                 
                 for var in var_list:
 
                     if var not in features:
 
                         features.append(var)
                         scorecard, features_length, pvalues = compute_scorecard(
-                        data, features, info, target_name=target_name, pvalues=True)
+                        data, features, info, target_name=target_name, pvalues=True, logistic_method=logistic_method)
                         pvalue = pvalues[-1]
                         if pvalue == 0:
                             gini_auxiliar = compute_metrics(apply_scorecard(
                             data, scorecard, info, target_name), target_name, ['gini'])
                         else: gini_auxiliar = 0
                         aux.loc[contador] = [var, pvalue, gini_auxiliar]
                         features.pop()
@@ -303,15 +304,15 @@
                     ' < {}, detenemos el proceso'.format(threshold))
                     break
 
                 new_var = aux.iloc[0]['var']
                 features.append(new_var)
 
                 scorecard, features_length, pvalues = compute_scorecard(
-                data, features, info, target_name=target_name, pvalues=True)
+                data, features, info, target_name=target_name, pvalues=True, logistic_method=logistic_method)
                 new_pvalue = pvalues[-1]
                 train_final = apply_scorecard(data, scorecard, info, target_name)
                 ks_train, gini_train = compute_metrics(train_final, target_name, ['ks', 'gini'])
                 
                 if stop_ks_gini:
                     if ks_train <= old_ks+0.002 and gini_train <= old_gini+0.003:
                         print('-' * N)
@@ -368,15 +369,15 @@
                 for v in dict_pvalues:
                     if dict_pvalues[v] >= threshold:
                         to_delete[v] = dict_pvalues[v]
                 if to_delete != {}:
                     for v in to_delete:
                         features.remove(v)
                         scorecard, features_length = compute_scorecard(
-                        data, features, info, target_name=target_name)
+                        data, features, info, target_name=target_name, logistic_method=logistic_method)
                         train_final = apply_scorecard(data, scorecard, info, target_name)
                         ks_train, gini_train = compute_metrics(
                         train_final, target_name, ['ks', 'gini'])
                         old_ks, old_gini = ks_train, gini_train
                         if not isinstance(muestra_test, type(None)):
                             test_final = apply_scorecard(
                             muestra_test, scorecard, info, target_name)
@@ -418,15 +419,15 @@
                                     'deleted : {}'.format(str(i+1).zfill(2), dict_pvalues[v],
                                     ks_train*100, ks_test*100, gini_train*100, gini_test*100, v))
 
     print('-' * N)
     print('Selección terminada: {}'.format(features))
     print('-' * N)
 
-    return features
+    return features    
 
 
 def display_table_ng(modelo_newgroups, candidate_var, objeto, bp):
 
     if not isinstance(bp, dict):
         vector = data_convert(
         modelo_newgroups.X_train[candidate_var].values, string_categories2(bp))[3]
```

### Comparing `memento-scorecard-0.2.7/memento/todd.py` & `memento-scorecard-0.7.2/memento/todd.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,26 +76,27 @@
             raise ValueError('En una variable de tipo texto o booleana '
             'es necesario especificar el diccionario de categorias')
         if pd.Series(x).isna().sum() > 0:
             x = pd.Series(x).replace(np.nan, 'Missing').values
         x_initial = x
         x = string_to_num(x, categories)
         x_converted = x
+
     else:
         x_initial = x
         x_converted = x
 
     if x.dtype not in ('O', 'bool') and np.isnan(x).sum() > 0:
         x_final = np.nan_to_num(x, nan=-12345678)
+
     else: x_final = x_converted
 
     return x_original, x_initial, x_converted, x_final
 
 
-
 def adapt_data(X, y, variables, breakpoints, target_name='target_4815162342'):
     
     df = pd.DataFrame()
     for variable in variables:
         
             bp = breakpoints[variable]
```

### Comparing `memento-scorecard-0.2.7/memento_scorecard.egg-info/PKG-INFO` & `memento-scorecard-0.7.2/memento_scorecard.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memento-scorecard
-Version: 0.2.7
+Version: 0.7.2
 Summary: Scorecard development with Python
 Home-page: https://github.com/Guilliu/Memento
 Author: Guillermo Lizcano Villafáñez
 Author-email: guille.lv.97@gmail.com
 License: Apache License 2.0
 Keywords: python,scoring,rating,logistic,regression,scorecard,woe,credit-risk,autogrouping
 Platform: UNKNOWN
```

### Comparing `memento-scorecard-0.2.7/setup.py` & `memento-scorecard-0.7.2/setup.py`

 * *Files identical despite different names*

