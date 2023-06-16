# Comparing `tmp/validador_colab-0.0.1.tar.gz` & `tmp/validador_colab-0.0.2.tar.gz`

## Comparing `validador_colab-0.0.1.tar` & `validador_colab-0.0.2.tar`

### file list

```diff
@@ -1,57 +1,37 @@
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 validador_colab-0.0.1/main.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 validador_colab-0.0.1/requirements.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/core/__init__.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/core/entities/__init__.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/core/entities/colab_counter.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/core/entities/natural_one.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/core/entities/sakura.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/core/entities/smarket_counter.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/core/entities/validation_detail.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/core/errors/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/core/errors/divergent_data.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/core/errors/no_data_found.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/core/repositories/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/core/repositories/colab_counters.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/core/repositories/smarket_analytics.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/core/usecases/__init__.py
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/core/usecases/colab_service.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/core/usecases/smarket_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/infra/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/infra/configs/__init__.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/infra/configs/configs.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/infra/database/__init__.py
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/infra/database/postgres.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/infra/database/postgres_controle.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/infra/repositories/__init__.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/infra/repositories/colab_counters_repository.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/infra/repositories/smarket_analytics_repository.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/infra/routes/__init__.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/infra/routes/daily_conf.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/infra/utils/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/loop/__init__.py
--rw-r--r--   0        0        0    13853 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/loop/first_block.py
--rw-r--r--   0        0        0    19747 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/loop/temp_data/colab_data_NaturalOne_2023-06-01_2023-06-11.pkl
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/loop/temp_data/colab_data_NaturalOne_2023-06-05_2023-06-05.pkl
--rw-r--r--   0        0        0    74659 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/loop/temp_data/colab_data_Sakura_2023-03-01_2023-03-31.pkl
--rw-r--r--   0        0        0    74329 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/loop/temp_data/colab_data_Sakura_2023-04-01_2023-04-30.pkl
--rw-r--r--   0        0        0    37738 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/loop/temp_data/colab_data_Sakura_2023-05-01_2023-05-15.pkl
--rw-r--r--   0        0        0    76973 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/loop/temp_data/colab_data_Sakura_2023-05-01_2023-05-31.pkl
--rw-r--r--   0        0        0    41709 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/loop/temp_data/colab_data_Sakura_2023-05-15_2023-05-31.pkl
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/loop/temp_data/colab_data_Sakura_2023-06-01_2023-06-01.pkl
--rw-r--r--   0        0        0     7840 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/loop/temp_data/colab_data_Sakura_2023-06-01_2023-06-03.pkl
--rw-r--r--   0        0        0    61588 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/loop/temp_data/smarket_data_NaturalOne_2023-06-01_2023-06-11.pkl
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/loop/temp_data/smarket_data_NaturalOne_2023-06-05_2023-06-05.pkl
--rw-r--r--   0        0        0   178573 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/loop/temp_data/smarket_data_Sakura_2023-03-01_2023-03-31.pkl
--rw-r--r--   0        0        0   153985 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/loop/temp_data/smarket_data_Sakura_2023-04-01_2023-04-30.pkl
--rw-r--r--   0        0        0    80293 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/loop/temp_data/smarket_data_Sakura_2023-05-01_2023-05-15.pkl
--rw-r--r--   0        0        0   164284 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/loop/temp_data/smarket_data_Sakura_2023-05-01_2023-05-31.pkl
--rw-r--r--   0        0        0    89565 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/loop/temp_data/smarket_data_Sakura_2023-05-15_2023-05-31.pkl
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/loop/temp_data/smarket_data_Sakura_2023-06-01_2023-06-01.pkl
--rw-r--r--   0        0        0    11672 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/loop/temp_data/smarket_data_Sakura_2023-06-01_2023-06-03.pkl
--rw-r--r--   0        0        0    57900 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/loop/temp_data/smarket_data_Sakura_2023-06-01_2023-06-11.pkl
--rw-r--r--   0        0        0     6279 2020-02-02 00:00:00.000000 validador_colab-0.0.1/validador_colab/loop/temp_data/smarket_data_Sakura_2023-06-08_2023-06-08.pkl
--rw-r--r--   0        0        0     5517 2020-02-02 00:00:00.000000 validador_colab-0.0.1/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-0.0.1/README.md
--rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 validador_colab-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 validador_colab-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 validador_colab-0.0.2/main.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 validador_colab-0.0.2/requirements.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/core/__init__.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/core/entities/__init__.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/core/entities/colab_counter.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/core/entities/natural_one.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/core/entities/sakura.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/core/entities/smarket_counter.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/core/entities/validation_detail.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/core/errors/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/core/errors/divergent_data.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/core/errors/no_data_found.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/core/repositories/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/core/repositories/colab_counters.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/core/repositories/smarket_analytics.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/core/usecases/__init__.py
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/core/usecases/colab_service.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/core/usecases/smarket_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/infra/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/infra/configs/__init__.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/infra/configs/configs.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/infra/database/__init__.py
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/infra/database/postgres.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/infra/database/postgres_controle.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/infra/repositories/__init__.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/infra/repositories/colab_counters_repository.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/infra/repositories/smarket_analytics_repository.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/infra/routes/__init__.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/infra/routes/daily_conf.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/infra/utils/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/loop/__init__.py
+-rw-r--r--   0        0        0    13853 2020-02-02 00:00:00.000000 validador_colab-0.0.2/validador_colab/loop/first_block.py
+-rw-r--r--   0        0        0     5538 2020-02-02 00:00:00.000000 validador_colab-0.0.2/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 validador_colab-0.0.2/README.md
+-rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 validador_colab-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 validador_colab-0.0.2/PKG-INFO
```

### Comparing `validador_colab-0.0.1/main.py` & `validador_colab-0.0.2/main.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.1/requirements.txt` & `validador_colab-0.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.1/validador_colab/core/entities/natural_one.py` & `validador_colab-0.0.2/validador_colab/core/entities/natural_one.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.1/validador_colab/core/entities/sakura.py` & `validador_colab-0.0.2/validador_colab/core/entities/sakura.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.1/validador_colab/core/usecases/colab_service.py` & `validador_colab-0.0.2/validador_colab/core/usecases/colab_service.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.1/validador_colab/core/usecases/smarket_service.py` & `validador_colab-0.0.2/validador_colab/core/usecases/smarket_service.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.1/validador_colab/infra/configs/configs.py` & `validador_colab-0.0.2/validador_colab/infra/configs/configs.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.1/validador_colab/infra/database/postgres.py` & `validador_colab-0.0.2/validador_colab/infra/database/postgres.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.1/validador_colab/infra/database/postgres_controle.py` & `validador_colab-0.0.2/validador_colab/infra/database/postgres_controle.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.1/validador_colab/infra/repositories/colab_counters_repository.py` & `validador_colab-0.0.2/validador_colab/infra/repositories/colab_counters_repository.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.1/validador_colab/infra/repositories/smarket_analytics_repository.py` & `validador_colab-0.0.2/validador_colab/infra/repositories/smarket_analytics_repository.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.1/validador_colab/infra/routes/daily_conf.py` & `validador_colab-0.0.2/validador_colab/infra/routes/daily_conf.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.1/validador_colab/loop/first_block.py` & `validador_colab-0.0.2/validador_colab/loop/first_block.py`

 * *Files identical despite different names*

### Comparing `validador_colab-0.0.1/.gitignore` & `validador_colab-0.0.2/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -269,8 +269,14 @@
 [Ll]ib
 [Ll]ib64
 [Ll]ocal
 [Ss]cripts
 pyvenv.cfg
 pip-selfcheck.json
 
+/venv
+
+/dist
+
+*.pkl
+
 # End of https://www.toptal.com/developers/gitignore/api/pycharm+all,python,venv
```

### Comparing `validador_colab-0.0.1/pyproject.toml` & `validador_colab-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "validador-colab"
 description = 'Validador colab é uma ferramenta para validar os dados diarios incrementáis nas tabelas de fato do colab e no Analytics'
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
-version = "0.0.1"
+version = "0.0.2"
 keywords = []
 authors = [
   { name = "Davi Amaral de Araujo", email = "davi@smarketsolutions.com.br" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
```

### Comparing `validador_colab-0.0.1/PKG-INFO` & `validador_colab-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: validador-colab
-Version: 0.0.1
+Version: 0.0.2
 Summary: Validador colab é uma ferramenta para validar os dados diarios incrementáis nas tabelas de fato do colab e no Analytics
 Project-URL: Documentation, https://github.com/unknown/validador-colab#readme
 Project-URL: Issues, https://github.com/unknown/validador-colab/issues
 Project-URL: Source, https://github.com/unknown/validador-colab
 Author-email: Davi Amaral de Araujo <davi@smarketsolutions.com.br>
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
```

