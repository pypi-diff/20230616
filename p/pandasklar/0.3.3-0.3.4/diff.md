# Comparing `tmp/pandasklar-0.3.3.tar.gz` & `tmp/pandasklar-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasklar-0.3.3.tar", last modified: Wed Jun 14 04:42:13 2023, max compression
+gzip compressed data, was "pandasklar-0.3.4.tar", last modified: Fri Jun 16 08:34:52 2023, max compression
```

## Comparing `pandasklar-0.3.3.tar` & `pandasklar-0.3.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-14 04:42:13.710746 pandasklar-0.3.3/
--rw-r--r--   0 me        (1000) me        (1000)     1063 2022-09-06 17:06:11.000000 pandasklar-0.3.3/LICENSE
--rw-rw-r--   0 me        (1000) me        (1000)     9805 2023-06-14 04:42:13.710746 pandasklar-0.3.3/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)     9297 2023-06-14 04:41:46.000000 pandasklar-0.3.3/README.md
--rw-r--r--   0 me        (1000) me        (1000)     1301 2023-06-14 04:41:35.000000 pandasklar-0.3.3/pyproject.toml
--rw-rw-r--   0 me        (1000) me        (1000)       38 2023-06-14 04:42:13.710746 pandasklar-0.3.3/setup.cfg
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-14 04:42:13.706746 pandasklar-0.3.3/src/
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-14 04:42:13.710746 pandasklar-0.3.3/src/pandasklar/
--rw-r--r--   0 me        (1000) me        (1000)      537 2023-02-13 16:45:54.000000 pandasklar-0.3.3/src/pandasklar/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)      214 2023-02-14 22:57:35.000000 pandasklar-0.3.3/src/pandasklar/__main__.py
--rw-r--r--   0 me        (1000) me        (1000)    19899 2023-05-12 20:23:55.000000 pandasklar-0.3.3/src/pandasklar/aggregate.py
--rw-r--r--   0 me        (1000) me        (1000)    27540 2023-04-11 17:22:24.000000 pandasklar-0.3.3/src/pandasklar/analyse.py
--rw-r--r--   0 me        (1000) me        (1000)    10330 2023-02-12 20:17:03.000000 pandasklar-0.3.3/src/pandasklar/compare.py
--rw-r--r--   0 me        (1000) me        (1000)     1092 2023-02-19 10:51:49.000000 pandasklar-0.3.3/src/pandasklar/config.py
--rw-r--r--   0 me        (1000) me        (1000)    26803 2023-02-20 15:41:11.000000 pandasklar-0.3.3/src/pandasklar/content.py
--rw-r--r--   0 me        (1000) me        (1000)     8710 2023-03-11 11:39:52.000000 pandasklar-0.3.3/src/pandasklar/develop.py
--rw-r--r--   0 me        (1000) me        (1000)    32239 2023-03-16 08:54:51.000000 pandasklar-0.3.3/src/pandasklar/pandas.py
--rw-r--r--   0 me        (1000) me        (1000)     2613 2023-02-13 21:21:37.000000 pandasklar-0.3.3/src/pandasklar/plot.py
--rw-r--r--   0 me        (1000) me        (1000)     4827 2023-02-08 06:49:03.000000 pandasklar-0.3.3/src/pandasklar/rank.py
--rw-r--r--   0 me        (1000) me        (1000)     8464 2023-02-12 21:40:20.000000 pandasklar-0.3.3/src/pandasklar/scale.py
--rw-r--r--   0 me        (1000) me        (1000)     8975 2023-04-10 20:10:39.000000 pandasklar-0.3.3/src/pandasklar/string.py
--rw-r--r--   0 me        (1000) me        (1000)     8810 2022-11-12 13:55:33.000000 pandasklar-0.3.3/src/pandasklar/subsets.py
--rw-r--r--   0 me        (1000) me        (1000)     5665 2023-06-09 20:00:34.000000 pandasklar-0.3.3/src/pandasklar/type_info.py
--rw-r--r--   0 me        (1000) me        (1000)     5467 2022-11-09 07:00:35.000000 pandasklar-0.3.3/src/pandasklar/values_info.py
-drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-14 04:42:13.710746 pandasklar-0.3.3/src/pandasklar.egg-info/
--rw-r--r--   0 me        (1000) me        (1000)     9805 2023-06-14 04:42:13.000000 pandasklar-0.3.3/src/pandasklar.egg-info/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)      677 2023-06-14 04:42:13.000000 pandasklar-0.3.3/src/pandasklar.egg-info/SOURCES.txt
--rw-r--r--   0 me        (1000) me        (1000)        1 2023-06-14 04:42:13.000000 pandasklar-0.3.3/src/pandasklar.egg-info/dependency_links.txt
--rw-r--r--   0 me        (1000) me        (1000)       56 2023-06-14 04:42:13.000000 pandasklar-0.3.3/src/pandasklar.egg-info/entry_points.txt
--rw-r--r--   0 me        (1000) me        (1000)       47 2023-06-14 04:42:13.000000 pandasklar-0.3.3/src/pandasklar.egg-info/requires.txt
--rw-r--r--   0 me        (1000) me        (1000)       11 2023-06-14 04:42:13.000000 pandasklar-0.3.3/src/pandasklar.egg-info/top_level.txt
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-16 08:34:52.223574 pandasklar-0.3.4/
+-rw-r--r--   0 me        (1000) me        (1000)     1063 2022-09-06 17:06:11.000000 pandasklar-0.3.4/LICENSE
+-rw-rw-r--   0 me        (1000) me        (1000)     9805 2023-06-16 08:34:52.223574 pandasklar-0.3.4/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)     9297 2023-06-16 08:34:16.000000 pandasklar-0.3.4/README.md
+-rw-r--r--   0 me        (1000) me        (1000)     1301 2023-06-16 08:34:00.000000 pandasklar-0.3.4/pyproject.toml
+-rw-rw-r--   0 me        (1000) me        (1000)       38 2023-06-16 08:34:52.223574 pandasklar-0.3.4/setup.cfg
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-16 08:34:52.215574 pandasklar-0.3.4/src/
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-16 08:34:52.223574 pandasklar-0.3.4/src/pandasklar/
+-rw-r--r--   0 me        (1000) me        (1000)      537 2023-02-13 16:45:54.000000 pandasklar-0.3.4/src/pandasklar/__init__.py
+-rw-r--r--   0 me        (1000) me        (1000)      214 2023-02-14 22:57:35.000000 pandasklar-0.3.4/src/pandasklar/__main__.py
+-rw-r--r--   0 me        (1000) me        (1000)    19899 2023-05-12 20:23:55.000000 pandasklar-0.3.4/src/pandasklar/aggregate.py
+-rw-r--r--   0 me        (1000) me        (1000)    27921 2023-06-16 07:57:01.000000 pandasklar-0.3.4/src/pandasklar/analyse.py
+-rw-r--r--   0 me        (1000) me        (1000)    10330 2023-02-12 20:17:03.000000 pandasklar-0.3.4/src/pandasklar/compare.py
+-rw-r--r--   0 me        (1000) me        (1000)     1092 2023-02-19 10:51:49.000000 pandasklar-0.3.4/src/pandasklar/config.py
+-rw-r--r--   0 me        (1000) me        (1000)    27326 2023-06-16 08:25:57.000000 pandasklar-0.3.4/src/pandasklar/content.py
+-rw-r--r--   0 me        (1000) me        (1000)     8710 2023-03-11 11:39:52.000000 pandasklar-0.3.4/src/pandasklar/develop.py
+-rw-r--r--   0 me        (1000) me        (1000)    32239 2023-03-16 08:54:51.000000 pandasklar-0.3.4/src/pandasklar/pandas.py
+-rw-r--r--   0 me        (1000) me        (1000)     2613 2023-02-13 21:21:37.000000 pandasklar-0.3.4/src/pandasklar/plot.py
+-rw-r--r--   0 me        (1000) me        (1000)     4827 2023-02-08 06:49:03.000000 pandasklar-0.3.4/src/pandasklar/rank.py
+-rw-r--r--   0 me        (1000) me        (1000)     8464 2023-02-12 21:40:20.000000 pandasklar-0.3.4/src/pandasklar/scale.py
+-rw-r--r--   0 me        (1000) me        (1000)     8975 2023-04-10 20:10:39.000000 pandasklar-0.3.4/src/pandasklar/string.py
+-rw-r--r--   0 me        (1000) me        (1000)     8810 2022-11-12 13:55:33.000000 pandasklar-0.3.4/src/pandasklar/subsets.py
+-rw-r--r--   0 me        (1000) me        (1000)     5665 2023-06-09 20:00:34.000000 pandasklar-0.3.4/src/pandasklar/type_info.py
+-rw-r--r--   0 me        (1000) me        (1000)     5467 2022-11-09 07:00:35.000000 pandasklar-0.3.4/src/pandasklar/values_info.py
+drwxrwxr-x   0 me        (1000) me        (1000)        0 2023-06-16 08:34:52.223574 pandasklar-0.3.4/src/pandasklar.egg-info/
+-rw-r--r--   0 me        (1000) me        (1000)     9805 2023-06-16 08:34:52.000000 pandasklar-0.3.4/src/pandasklar.egg-info/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)      677 2023-06-16 08:34:52.000000 pandasklar-0.3.4/src/pandasklar.egg-info/SOURCES.txt
+-rw-r--r--   0 me        (1000) me        (1000)        1 2023-06-16 08:34:52.000000 pandasklar-0.3.4/src/pandasklar.egg-info/dependency_links.txt
+-rw-r--r--   0 me        (1000) me        (1000)       56 2023-06-16 08:34:52.000000 pandasklar-0.3.4/src/pandasklar.egg-info/entry_points.txt
+-rw-r--r--   0 me        (1000) me        (1000)       47 2023-06-16 08:34:52.000000 pandasklar-0.3.4/src/pandasklar.egg-info/requires.txt
+-rw-r--r--   0 me        (1000) me        (1000)       11 2023-06-16 08:34:52.000000 pandasklar-0.3.4/src/pandasklar.egg-info/top_level.txt
```

### Comparing `pandasklar-0.3.3/LICENSE` & `pandasklar-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.3/PKG-INFO` & `pandasklar-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasklar
-Version: 0.3.3
+Version: 0.3.4
 Summary: Toolbox / Ecosystem for data science. Easier handling of pandas, especially when thinking in SQL.
 Author-email: djekra <hopsalla@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/djekra/pandasklar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pandasklar-0.3.3/README.md` & `pandasklar-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.3/pyproject.toml` & `pandasklar-0.3.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pyproject.toml
 
 
 [project]
 name            = "pandasklar"
-version         = "0.3.3"    
+version         = "0.3.4"    
 
 requires-python = ">=3.8"
 dependencies    = ['pandas','numpy','perlin_noise','termcolor','bpyth','blab',]
 
 authors        = [{ name = "djekra", email = "hopsalla@gmail.com" }]
 description     = "Toolbox / Ecosystem for data science. Easier handling of pandas, especially when thinking in SQL."
 readme          = "README.md"
```

### Comparing `pandasklar-0.3.3/src/pandasklar/__init__.py` & `pandasklar-0.3.4/src/pandasklar/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.3/src/pandasklar/aggregate.py` & `pandasklar-0.3.4/src/pandasklar/aggregate.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.3/src/pandasklar/analyse.py` & `pandasklar-0.3.4/src/pandasklar/analyse.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,29 +112,42 @@
 
 
 # Alle class_info einer Series oder eines Index   
 def analyse_datatype(data):
     """ 
     Returns a dict with info about the datatypes of a Series or Index and it's content
     """
+
+
+    def is_datetime_series(series):
+        try:
+            pd.to_datetime(series)
+            return pd.api.types.is_datetime64_any_dtype(series)
+        except ValueError:
+            return False
+
     
+    if isinstance(data, pd.DataFrame): 
+        return dataframe( analyse_datatypes(data) ) 
+        
     # Aufruf mit Index
     if isinstance(data, pd.Index): 
         series = data.to_series()
         series.name = '__index__'
         return analyse_datatype(series)    
 
     info = type_info(data)
     result = {
         'col_name': data.name,
         'datatype_instance': info.name_instance,  
         'datatype': info.name,        
         'datatype_short': info.name_short,        
         'is_numeric': is_numeric_dtype(data),                
         'is_string': is_string_dtype(data),  
+        'is_datetime': pd.api.types.is_datetime64_any_dtype(data),         
         'is_hashable': info.is_hashable,
         'nan_allowed': info.nan_allowed,   
         'mem_usage': mem_usage(data),        
     }
         
     return result
```

### Comparing `pandasklar-0.3.3/src/pandasklar/compare.py` & `pandasklar-0.3.4/src/pandasklar/compare.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.3/src/pandasklar/config.py` & `pandasklar-0.3.4/src/pandasklar/config.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.3/src/pandasklar/content.py` & `pandasklar-0.3.4/src/pandasklar/content.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 #################################################################################
 
 
 def random_series(size, typ, **kwargs):
     ''' 
     Returns a series of random data. 
     * size
-    * typ: 'int', 'float', 'string', 'name', 'choice', 'list', 'mix',
+    * typ: 'int', 'float', 'string', 'name', 'choice', 'list', 'time', mix',
            'ascending', 'descending', 'perlin' or 'errorprone'. Or the first letter of this.
            'name' generates random first names, 'list' generates lists of random first names.
            'mix' generates mixed datatypes. 
            'ascending', 'descending' and 'perlin' generates ordered random sequences.
            'errorprone' generates sequences of NaNs, 0, 1 with similar index. Useful for testing. 
 
     The other arguments are passed to the appropriate functions for the type of random data.
@@ -157,15 +157,16 @@
     
     There are extra parameters for some types of random data:
     - int:    min, max: closed interval, min and max are both possible values in the generated data
     - float:  decimals: how many decimal places
     - string: len_min, len_max: controls the length of the generated character sequence
               mix: Explicit specification of the available character set. Overwrites p_dup. 
                    Example: mix='ABCabc'
-    - list:   len_min, len_max: controls the length of the generated lists.                   
+    - list:   len_min, len_max: controls the length of the generated lists. 
+    - time:   min, max
     - choice: choice: List or Series of elements to choose
     - perlin: freq: List of up to frequencies, see random_perlin for more details
               op: 'add' or 'mult', how the frequencies are linked together
               sc: scaling, default is 'max_abs', this scales -1..1, see function scale
     
     Examples:    
     =========
@@ -186,15 +187,17 @@
     elif typ in ['string','str','s']: 
         myfunc = random_series_string 
     elif typ in ['name','n']: 
         myfunc = random_series_name  
     elif typ in ['choice','c']: 
         myfunc = random_series_choice  
     elif typ in ['list','l']: 
-        myfunc = random_series_list     
+        myfunc = random_series_list  
+    elif typ in ['time','t','datetime']: 
+        myfunc = random_series_datetime         
     elif typ in ['mix','m']: 
         myfunc = random_series_mix     
     elif typ in ['errorprone','e']: 
         myfunc = random_series_errorprone        
     
     p_dup = kwargs.get('p_dup',0)
     p_nan = kwargs.get('p_nan',0)    
@@ -380,14 +383,24 @@
 
 
 
 
 # ==================================================================================================
 # Interne Funktionen für zufällige Testdaten
 # ==================================================================================================
+
+
+def random_series_datetime( size, min='1900-01-01', max='2023-12-31', name='rnd_time', index=None, p_nan=0, p_dup=0):
+    '''
+    Returns a series of random datetime between min and max. 
+    '''
+    random_dates = pd.to_datetime(np.random.randint(pd.Timestamp(min).value, pd.Timestamp(max).value, size), unit='ns')
+    result = pd.Series(random_dates)  
+    result = result.rename(name)  
+    return result
     
 
 def random_series_int( size, min=0, max=1000, name='rnd_int', index=None, p_nan=0, p_dup=0):
     '''
     Returns a series of random integers between min and max. min and max are both possible.
     '''
     result = pd.Series(np.random.randint(min, max+1, size))
@@ -532,18 +545,18 @@
     anz = int(size / 5) + 1
     
     b = random_series( anz, 'int',    min=-66666, max=66666,          )    
     c = random_series( anz, 'float',  decimals=4,                     )
     d = random_series( anz, 'string', len_min=2, len_max=20,          )
     e = random_series( anz, 'name',                                   )
     f = random_series( anz, 'choice', choice=['Bremen','Bremerhaven'] )
-    g = random_series( anz, 'list',                                   )    
+    g = random_series( anz, 'list',                                   )  
+    h = random_series( anz, 'time',                                   )      
       
-    #result = b.append(c).append(d).append(e).append(f).append(g)
-    result = pd.concat( [b, c, d, e, f, g] )
+    result = pd.concat( [b, c, d, e, f, g, h] )
     result = result.sample(frac=1).reset_index(drop=True).head(size)
     result = result.rename(name)    
     result.iloc[0] = {0}
     
     return result
```

### Comparing `pandasklar-0.3.3/src/pandasklar/develop.py` & `pandasklar-0.3.4/src/pandasklar/develop.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.3/src/pandasklar/pandas.py` & `pandasklar-0.3.4/src/pandasklar/pandas.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.3/src/pandasklar/plot.py` & `pandasklar-0.3.4/src/pandasklar/plot.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.3/src/pandasklar/rank.py` & `pandasklar-0.3.4/src/pandasklar/rank.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.3/src/pandasklar/scale.py` & `pandasklar-0.3.4/src/pandasklar/scale.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.3/src/pandasklar/string.py` & `pandasklar-0.3.4/src/pandasklar/string.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.3/src/pandasklar/subsets.py` & `pandasklar-0.3.4/src/pandasklar/subsets.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.3/src/pandasklar/type_info.py` & `pandasklar-0.3.4/src/pandasklar/type_info.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.3/src/pandasklar/values_info.py` & `pandasklar-0.3.4/src/pandasklar/values_info.py`

 * *Files identical despite different names*

### Comparing `pandasklar-0.3.3/src/pandasklar.egg-info/PKG-INFO` & `pandasklar-0.3.4/src/pandasklar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasklar
-Version: 0.3.3
+Version: 0.3.4
 Summary: Toolbox / Ecosystem for data science. Easier handling of pandas, especially when thinking in SQL.
 Author-email: djekra <hopsalla@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/djekra/pandasklar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pandasklar-0.3.3/src/pandasklar.egg-info/SOURCES.txt` & `pandasklar-0.3.4/src/pandasklar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

