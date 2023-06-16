# Comparing `tmp/exergenics-etl-1.2.0.tar.gz` & `tmp/exergenics-etl-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exergenics-etl-1.2.0.tar", last modified: Thu Jun  8 00:19:55 2023, max compression
+gzip compressed data, was "exergenics-etl-1.3.0.tar", last modified: Fri Jun 16 05:32:10 2023, max compression
```

## Comparing `exergenics-etl-1.2.0.tar` & `exergenics-etl-1.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:19:55.380217 exergenics-etl-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-08 00:19:52.000000 exergenics-etl-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-08 00:19:55.380217 exergenics-etl-1.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:19:55.376217 exergenics-etl-1.2.0/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:19:55.376217 exergenics-etl-1.2.0/app/exergenics_etl/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-08 00:19:52.000000 exergenics-etl-1.2.0/app/exergenics_etl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:19:55.380217 exergenics-etl-1.2.0/app/exergenics_etl/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 00:19:52.000000 exergenics-etl-1.2.0/app/exergenics_etl/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52545 2023-06-08 00:19:52.000000 exergenics-etl-1.2.0/app/exergenics_etl/src/exergenics_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-08 00:19:52.000000 exergenics-etl-1.2.0/app/exergenics_etl/src/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:19:55.380217 exergenics-etl-1.2.0/app/exergenics_etl/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 00:19:52.000000 exergenics-etl-1.2.0/app/exergenics_etl/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-08 00:19:52.000000 exergenics-etl-1.2.0/app/exergenics_etl/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    34705 2023-06-08 00:19:52.000000 exergenics-etl-1.2.0/app/exergenics_etl/test/test_exergenics_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-08 00:19:52.000000 exergenics-etl-1.2.0/app/exergenics_etl/test/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:19:55.376217 exergenics-etl-1.2.0/app/exergenics_etl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-08 00:19:55.000000 exergenics-etl-1.2.0/app/exergenics_etl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-08 00:19:55.000000 exergenics-etl-1.2.0/app/exergenics_etl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 00:19:55.000000 exergenics-etl-1.2.0/app/exergenics_etl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-08 00:19:55.000000 exergenics-etl-1.2.0/app/exergenics_etl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 00:19:55.000000 exergenics-etl-1.2.0/app/exergenics_etl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 00:19:55.380217 exergenics-etl-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-08 00:19:54.000000 exergenics-etl-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:32:10.229068 exergenics-etl-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-16 05:32:07.000000 exergenics-etl-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-16 05:32:10.229068 exergenics-etl-1.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:32:10.229068 exergenics-etl-1.3.0/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:32:10.229068 exergenics-etl-1.3.0/app/exergenics_etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-16 05:32:07.000000 exergenics-etl-1.3.0/app/exergenics_etl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:32:10.229068 exergenics-etl-1.3.0/app/exergenics_etl/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 05:32:07.000000 exergenics-etl-1.3.0/app/exergenics_etl/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53219 2023-06-16 05:32:07.000000 exergenics-etl-1.3.0/app/exergenics_etl/src/exergenics_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-16 05:32:07.000000 exergenics-etl-1.3.0/app/exergenics_etl/src/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:32:10.229068 exergenics-etl-1.3.0/app/exergenics_etl/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 05:32:07.000000 exergenics-etl-1.3.0/app/exergenics_etl/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-16 05:32:07.000000 exergenics-etl-1.3.0/app/exergenics_etl/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35383 2023-06-16 05:32:07.000000 exergenics-etl-1.3.0/app/exergenics_etl/test/test_exergenics_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-16 05:32:07.000000 exergenics-etl-1.3.0/app/exergenics_etl/test/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:32:10.229068 exergenics-etl-1.3.0/app/exergenics_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-16 05:32:10.000000 exergenics-etl-1.3.0/app/exergenics_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-16 05:32:10.000000 exergenics-etl-1.3.0/app/exergenics_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 05:32:10.000000 exergenics-etl-1.3.0/app/exergenics_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-16 05:32:10.000000 exergenics-etl-1.3.0/app/exergenics_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-16 05:32:10.000000 exergenics-etl-1.3.0/app/exergenics_etl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 05:32:10.229068 exergenics-etl-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-16 05:32:09.000000 exergenics-etl-1.3.0/setup.py
```

### Comparing `exergenics-etl-1.2.0/LICENSE` & `exergenics-etl-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.2.0/app/exergenics_etl/__init__.py` & `exergenics-etl-1.3.0/app/exergenics_etl/__init__.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.2.0/app/exergenics_etl/src/exergenics_etl.py` & `exergenics-etl-1.3.0/app/exergenics_etl/src/exergenics_etl.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,17 @@
 logger = Logger(loggerName='Exergenics-ETL',
                 component='python_package', subComponent='exergenics_etl')
 
 
 class EtlError(Exception):
     """Exception raised for errors in ETL function."""
 
-    def __init__(self, message=""):
+    def __init__(self, message="", *args):
         self.message = message
-        super().__init__(self.message)
+        super().__init__(self.message, *args)
 
 
 def hello(name: str) -> None:
     """Says hello to someone.
 
     Args:
         name (str): The name of the person to greet.
@@ -570,54 +570,64 @@
     def _check_for_wide_format(self, df: pd.DataFrame) -> bool:
         """Method check whether input dataframe is in a wide format.
 
         Args:
             df (pd.DataFrame): Pandas DataFrame to apply format checking on. 
 
         Raises:
-            EtlError: If the input dataframe is in a long format.
+            EtlError: If the input dataframe is in a long format. 
+            The exception is raised with three arguments: the error message, 
+            the names and the values column IDs of the long dataframe.
 
         Returns:
             bool: True if input is in a wide format.
         """
 
         # If there are only 3 columns in this data file
         if df.shape[1] == N_COLUMN_LONG_DATA:
 
             # Check if the 2nd or 3rd column is a variable name column
 
+            # Check the 2nd column
+            namesColumnId = 1  # The column ID of the names column (0-based indexing)
+            valuesColumnId = 2  # The column ID of the values column (0-based indexing)
+
             # If none of the values in the 2nd column can be converted to float
-            secondColumnName = df.columns[1]
+            secondColumnName = df.columns[namesColumnId]
             secondColumn = df[secondColumnName]
             if not any(secondColumn.apply(convertable_to_float)):
 
                 # If the average length of the strings in the 2nd column is longer than 10
                 if secondColumn.apply(lambda x: len(x)).mean() > LENGTH_THRESHOLD:
                     
                     # Raise error when a long format dataset is detected
                     errorMessage = 'This data file looks like in a long format. ' \
                         + f'The 2nd column (\"{secondColumnName}\") is likely a variable name column. ' \
                         + 'However, we currently only accept datasets in a wide format.'
                     logger.error(errorMessage)
-                    raise EtlError(errorMessage)
-            
+                    raise EtlError(errorMessage, namesColumnId, valuesColumnId)
+                
+            # Check the 3rd column
+            namesColumnId = 2  # The column ID of the names column (0-based indexing)
+            valuesColumnId = 1  # The column ID of the values column (0-based indexing)
+
             # If none of the values in the 3rd column can be converted to float
-            thirdColumnName = df.columns[2]
+            thirdColumnName = df.columns[namesColumnId]
             thirdColumn = df[thirdColumnName]
             if not any(thirdColumn.apply(convertable_to_float)):
 
                 # If the average length of the strings in the 3rd column is longer than 10
                 if thirdColumn.apply(lambda x: len(x)).mean() > LENGTH_THRESHOLD:
 
                     # Raise error when a long format dataset is detected
                     errorMessage = 'This data file looks like in a long format. ' \
                         + f'The 3rd column (\"{thirdColumnName}\") is likely a variable name column. ' \
                         + 'However, we currently only accept datasets in a wide format.'
                     logger.error(errorMessage)
-                    raise EtlError(errorMessage)
+                    raise EtlError(errorMessage, namesColumnId, valuesColumnId)
 
         return True
 
     def check_input_dataframe(self, df: pd.DataFrame) -> bool:
         """Validate the format of a dataframe read from a data file.
 
         Args:
```

### Comparing `exergenics-etl-1.2.0/app/exergenics_etl/src/logger.py` & `exergenics-etl-1.3.0/app/exergenics_etl/src/logger.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.2.0/app/exergenics_etl/test/conftest.py` & `exergenics-etl-1.3.0/app/exergenics_etl/test/conftest.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.2.0/app/exergenics_etl/test/test_exergenics_etl.py` & `exergenics-etl-1.3.0/app/exergenics_etl/test/test_exergenics_etl.py`

 * *Files 5% similar despite different names*

```diff
@@ -246,24 +246,34 @@
     @pytest.fixture(scope='class')
     def my_wide_format_dataframe(self):
         filePath = 'app/exergenics_etl/test/testData/wideData.csv'
         df = pd.read_csv(filePath)
         return df
 
     @pytest.fixture(scope='class')
-    def my_long_format_dataframe1(self):
+    def my_check_for_wide_format_test_case_long1(self):
+        """Second test case for the _check_for_wide_format method where the 
+        input is a long dataframe, and the names column is in the 2rd 
+        column."""
         filePath = 'app/exergenics_etl/test/testData/longData_nameColumnIn2ndColumn.csv'
         df = pd.read_csv(filePath)
-        return df
+        namesColumnId = 1
+        valuesColumnId = 2
+        return df, namesColumnId, valuesColumnId
     
     @pytest.fixture(scope='class')
-    def my_long_format_dataframe2(self):
+    def my_check_for_wide_format_test_case_long2(self):
+        """Second test case for the _check_for_wide_format method where the 
+        input is a long dataframe, and the names column is in the 3rd 
+        column."""
         filePath = 'app/exergenics_etl/test/testData/longData_nameColumnIn3rdColumn.csv'
         df = pd.read_csv(filePath)
-        return df
+        namesColumnId = 2
+        valuesColumnId = 1
+        return df, namesColumnId, valuesColumnId
 
     @pytest.fixture(scope='class')
     def my_valid_timestamp_headers(self):
         return ['datetime', 'timestamp', 'event', 'timepretty', 'ts']
 
     @pytest.fixture(scope='class')
     def my_generic_column_headers(self):
@@ -277,21 +287,24 @@
         return inputValidation
 
     def test_check_for_wide_format(self, my_inputValidation_object, my_wide_format_dataframe):
         """Check for wide format when a wide format dataframe is passed."""
         assert my_inputValidation_object._check_for_wide_format(
             my_wide_format_dataframe)
 
-    @pytest.mark.parametrize("my_long_format_dataframe", ['my_long_format_dataframe1', 'my_long_format_dataframe2'])
-    def test_check_for_wide_format_on_long_dataframe(self, my_inputValidation_object, my_long_format_dataframe, request):
+    @pytest.mark.parametrize("my_test_case", ['my_check_for_wide_format_test_case_long1', 'my_check_for_wide_format_test_case_long2'])
+    def test_check_for_wide_format_on_long_dataframe(self, my_inputValidation_object, my_test_case, request):
         """Check for wide format when a long format dataframe is passed."""
-        my_long_format_dataframe = request.getfixturevalue(my_long_format_dataframe)
-        with pytest.raises(EtlError):
+        myLongDf, expectedNamesColumnId, expectedValuesColumnId = request.getfixturevalue(my_test_case)
+        with pytest.raises(EtlError) as errInfo:
             my_inputValidation_object._check_for_wide_format(
-                my_long_format_dataframe)
+                myLongDf)
+
+        assert errInfo.value.args[1] == expectedNamesColumnId
+        assert errInfo.value.args[2] == expectedValuesColumnId
 
     def test_check_for_generic_header1(self, my_inputValidation_object):
         myDfSameName = pd.read_csv(
             'app/exergenics_etl/test/testData/dfSameName.csv', parse_dates=['timepretty'])
         myDfNew = pd.read_csv(
             'app/exergenics_etl/test/testData/dfNew.csv', parse_dates=['timepretty'])
         myPointName = 'Ch1-kwr'
```

### Comparing `exergenics-etl-1.2.0/app/exergenics_etl.egg-info/SOURCES.txt` & `exergenics-etl-1.3.0/app/exergenics_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.2.0/setup.py` & `exergenics-etl-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 # with open("app/Readme.md", "r") as f:
 #     long_description = f.read()
 
 setup(
     name="exergenics-etl",
-    version="v1.2.0",
+    version="v1.3.0",
     description="Exergenics shared Data ETL functions",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description="### Exergenics ETL Pytho package",
     long_description_content_type="text/markdown",
     url="",
     author="Nobel Wong",
```

