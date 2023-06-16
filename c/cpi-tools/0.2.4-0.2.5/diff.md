# Comparing `tmp/cpi_tools-0.2.4.tar.gz` & `tmp/cpi_tools-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/nikitamarini/Desktop/CPI/cpi_tools/dist/.tmp-piqjlkg3/cpi_tools-0.2.4.tar", last modified: Fri Jun  9 13:34:33 2023, max compression
+gzip compressed data, was "cpi_tools-0.2.5.tar", last modified: Fri Jun 16 14:42:22 2023, max compression
```

## Comparing `cpi_tools-0.2.4.tar` & `cpi_tools-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 nikitamarini   (501) staff       (20)        0 2023-06-09 13:34:33.297533 cpi_tools-0.2.4/
--rw-r--r--   0 nikitamarini   (501) staff       (20)     1074 2023-06-09 10:53:47.000000 cpi_tools-0.2.4/LICENSE
--rw-r--r--   0 nikitamarini   (501) staff       (20)        0 2023-06-09 10:53:47.000000 cpi_tools-0.2.4/MANIFEST.in
--rw-r--r--   0 nikitamarini   (501) staff       (20)      911 2023-06-09 13:34:33.297597 cpi_tools-0.2.4/PKG-INFO
--rw-r--r--   0 nikitamarini   (501) staff       (20)      442 2023-06-09 10:53:47.000000 cpi_tools-0.2.4/README.md
-drwxr-xr-x   0 nikitamarini   (501) staff       (20)        0 2023-06-09 13:34:33.296774 cpi_tools-0.2.4/cpi_tools/
--rw-r--r--   0 nikitamarini   (501) staff       (20)        0 2023-06-09 10:53:47.000000 cpi_tools-0.2.4/cpi_tools/__init__.py
--rw-r--r--   0 nikitamarini   (501) staff       (20)     2375 2023-06-09 10:53:47.000000 cpi_tools-0.2.4/cpi_tools/aws_tools.py
--rw-r--r--   0 nikitamarini   (501) staff       (20)     4535 2023-06-09 10:53:47.000000 cpi_tools-0.2.4/cpi_tools/cpi_validation.py
--rw-r--r--   0 nikitamarini   (501) staff       (20)     7278 2023-06-09 13:33:43.000000 cpi_tools-0.2.4/cpi_tools/fuzzy_matching_cpi.py
--rw-r--r--   0 nikitamarini   (501) staff       (20)    14573 2023-06-09 10:53:47.000000 cpi_tools-0.2.4/cpi_tools/tracking_processing_tools.py
-drwxr-xr-x   0 nikitamarini   (501) staff       (20)        0 2023-06-09 13:34:33.297419 cpi_tools-0.2.4/cpi_tools.egg-info/
--rw-r--r--   0 nikitamarini   (501) staff       (20)      911 2023-06-09 13:34:33.000000 cpi_tools-0.2.4/cpi_tools.egg-info/PKG-INFO
--rw-r--r--   0 nikitamarini   (501) staff       (20)      330 2023-06-09 13:34:33.000000 cpi_tools-0.2.4/cpi_tools.egg-info/SOURCES.txt
--rw-r--r--   0 nikitamarini   (501) staff       (20)        1 2023-06-09 13:34:33.000000 cpi_tools-0.2.4/cpi_tools.egg-info/dependency_links.txt
--rw-r--r--   0 nikitamarini   (501) staff       (20)       10 2023-06-09 13:34:33.000000 cpi_tools-0.2.4/cpi_tools.egg-info/top_level.txt
--rw-r--r--   0 nikitamarini   (501) staff       (20)      103 2023-06-09 10:53:47.000000 cpi_tools-0.2.4/pyproject.toml
--rw-r--r--   0 nikitamarini   (501) staff       (20)      558 2023-06-09 13:34:33.297921 cpi_tools-0.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 14:42:22.610111 cpi_tools-0.2.5/
+-rw-rw-rw-   0        0        0     1094 2023-06-12 14:53:43.000000 cpi_tools-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-06-12 14:53:43.000000 cpi_tools-0.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      956 2023-06-16 14:42:22.610111 cpi_tools-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      473 2023-06-12 14:53:43.000000 cpi_tools-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 14:42:22.608431 cpi_tools-0.2.5/cpi_tools/
+-rw-rw-rw-   0        0        0        0 2023-06-12 14:53:43.000000 cpi_tools-0.2.5/cpi_tools/__init__.py
+-rw-rw-rw-   0        0        0     2436 2023-06-12 14:53:43.000000 cpi_tools-0.2.5/cpi_tools/aws_tools.py
+-rw-rw-rw-   0        0        0     4633 2023-06-12 14:53:43.000000 cpi_tools-0.2.5/cpi_tools/cpi_validation.py
+-rw-rw-rw-   0        0        0     7497 2023-06-12 14:53:43.000000 cpi_tools-0.2.5/cpi_tools/fuzzy_matching_cpi.py
+-rw-rw-rw-   0        0        0    14916 2023-06-16 14:33:00.000000 cpi_tools-0.2.5/cpi_tools/tracking_processing_tools.py
+drwxrwxrwx   0        0        0        0 2023-06-16 14:42:22.610111 cpi_tools-0.2.5/cpi_tools.egg-info/
+-rw-rw-rw-   0        0        0      956 2023-06-16 14:42:22.000000 cpi_tools-0.2.5/cpi_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-06-16 14:42:22.000000 cpi_tools-0.2.5/cpi_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 14:42:22.000000 cpi_tools-0.2.5/cpi_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-16 14:42:22.000000 cpi_tools-0.2.5/cpi_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-06-12 14:53:43.000000 cpi_tools-0.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0      581 2023-06-16 14:42:22.610111 cpi_tools-0.2.5/setup.cfg
```

### Comparing `cpi_tools-0.2.4/PKG-INFO` & `cpi_tools-0.2.5/cpi_tools.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-Metadata-Version: 2.1
-Name: cpi_tools
-Version: 0.2.4
-Summary: Repository of functions used across CPI
-Home-page: https://github.com/climatepolicydata/cpi_tools
-Author: Jake Connolly, Nikita Marini
-Author-email: datascience@cpiglobal.org
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# CPI Data Tools
-
-A repository of commonly used tools across CPI
-
-## Instructions
-
-1. Install:
-
-```
-pip install cpi_tools
-```
-
-AWS Tools
-
-```python
-from cpi_tools import aws_tools
-
-#S3 Bucket
-bucket = 'YOUR_BUCKET'
-#Path within S3
-path = 'PATH_IN_BUCKET'
-#S3 File name 
-file_name = 'FILE_NAME'
-
-#Read file from S3
-df = aws_tools.read_from_s3(bucket, path, file_name)
-
-#Write file to S3
-aws_tools.write_to_s3(df, bucket, path, file_name)
-```
-
+Metadata-Version: 2.1
+Name: cpi-tools
+Version: 0.2.5
+Summary: Repository of functions used across CPI
+Home-page: https://github.com/climatepolicydata/cpi_tools
+Author: Jake Connolly, Nikita Marini
+Author-email: datascience@cpiglobal.org
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# CPI Data Tools
+
+A repository of commonly used tools across CPI
+
+## Instructions
+
+1. Install:
+
+```
+pip install cpi_tools
+```
+
+AWS Tools
+
+```python
+from cpi_tools import aws_tools
+
+#S3 Bucket
+bucket = 'YOUR_BUCKET'
+#Path within S3
+path = 'PATH_IN_BUCKET'
+#S3 File name 
+file_name = 'FILE_NAME'
+
+#Read file from S3
+df = aws_tools.read_from_s3(bucket, path, file_name)
+
+#Write file to S3
+aws_tools.write_to_s3(df, bucket, path, file_name)
+```
+
```

### Comparing `cpi_tools-0.2.4/cpi_tools/aws_tools.py` & `cpi_tools-0.2.5/cpi_tools/aws_tools.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-import pandas as pd
-import boto3
-import s3fs
-from io import StringIO
-
-from dotenv import load_dotenv, find_dotenv
-
-def read_from_s3(s3_bucket: str, s3_file_path:str, file_name: str, file_type = 'csv', sheet_name=None, skip_rows=0) -> pd.DataFrame:
-    """
-    This function reads data from an S3 bucket and returns it as a pandas DataFrame.
-
-    Inputs:
-
-    s3_bucket (str): The name of the S3 bucket where the file is located.
-    s3_file_path (str): The file path within the S3 bucket.
-    file_name (str): The name of the file to be read.
-    file_type (str, optional): The file type of the file to be read. Defaults to 'csv'.
-    sheet_name (str, optional): The sheet name to be read from the excel file. Only used if file_type is 'xlsx'.
-    skip_rows (int, optional): The number of rows to skip when reading the file. Defaults to 0.
-    Returns:
-
-    df (pd.DataFrame): The data read from the file.
-    """
-
-    if load_dotenv(find_dotenv()):
-
-        if file_type == 'csv':
-            df = pd.read_csv(f's3://{s3_bucket}/{s3_file_path}/{file_name}.csv',skiprows=skip_rows, encoding='utf-8')
-
-        elif file_type == 'xlsx':
-            if sheet_name:
-                df = pd.read_excel(f's3://{s3_bucket}/{s3_file_path}/{file_name}.xlsx', sheet_name=sheet_name, skiprows=skip_rows)
-            else:
-                df = pd.read_excel(f's3://{s3_bucket}/{s3_file_path}/{file_name}.xlsx', skiprows=skip_rows)
-    else:
-        print('No AWS account variables found. Please add account variables to the .env file in your local directory')
-
-    return df
-
-
-def write_to_s3(df: pd.DataFrame, s3_bucket: str, s3_file_path:str, file_name: str):
-
-    '''
-    This function takes a processed reference dataframe and the filename for it to be saved as within S3 
-    and uploads the dataframe as a CSV
-
-    Inputs:
-
-    df (pd.DataFrame): The dataframe to be written to s3
-    s3_bucket (str): The name of the S3 bucket where the file will ve saved.
-    s3_file_path (str): The file path within the S3 bucket.
-    file_name (str): The name of the file to be saved.
-
-    Returns:
-    None
-    '''
-    
-    #Filepath to processed cpi reference folder
-    csv_buffer = StringIO()
-    df.to_csv(csv_buffer, index=False, encoding="utf-8")
-    s3_resource = boto3.resource('s3')
+import pandas as pd
+import boto3
+import s3fs
+from io import StringIO
+
+from dotenv import load_dotenv, find_dotenv
+
+def read_from_s3(s3_bucket: str, s3_file_path:str, file_name: str, file_type = 'csv', sheet_name=None, skip_rows=0) -> pd.DataFrame:
+    """
+    This function reads data from an S3 bucket and returns it as a pandas DataFrame.
+
+    Inputs:
+
+    s3_bucket (str): The name of the S3 bucket where the file is located.
+    s3_file_path (str): The file path within the S3 bucket.
+    file_name (str): The name of the file to be read.
+    file_type (str, optional): The file type of the file to be read. Defaults to 'csv'.
+    sheet_name (str, optional): The sheet name to be read from the excel file. Only used if file_type is 'xlsx'.
+    skip_rows (int, optional): The number of rows to skip when reading the file. Defaults to 0.
+    Returns:
+
+    df (pd.DataFrame): The data read from the file.
+    """
+
+    if load_dotenv(find_dotenv()):
+
+        if file_type == 'csv':
+            df = pd.read_csv(f's3://{s3_bucket}/{s3_file_path}/{file_name}.csv',skiprows=skip_rows, encoding='utf-8')
+
+        elif file_type == 'xlsx':
+            if sheet_name:
+                df = pd.read_excel(f's3://{s3_bucket}/{s3_file_path}/{file_name}.xlsx', sheet_name=sheet_name, skiprows=skip_rows)
+            else:
+                df = pd.read_excel(f's3://{s3_bucket}/{s3_file_path}/{file_name}.xlsx', skiprows=skip_rows)
+    else:
+        print('No AWS account variables found. Please add account variables to the .env file in your local directory')
+
+    return df
+
+
+def write_to_s3(df: pd.DataFrame, s3_bucket: str, s3_file_path:str, file_name: str):
+
+    '''
+    This function takes a processed reference dataframe and the filename for it to be saved as within S3 
+    and uploads the dataframe as a CSV
+
+    Inputs:
+
+    df (pd.DataFrame): The dataframe to be written to s3
+    s3_bucket (str): The name of the S3 bucket where the file will ve saved.
+    s3_file_path (str): The file path within the S3 bucket.
+    file_name (str): The name of the file to be saved.
+
+    Returns:
+    None
+    '''
+    
+    #Filepath to processed cpi reference folder
+    csv_buffer = StringIO()
+    df.to_csv(csv_buffer, index=False, encoding="utf-8")
+    s3_resource = boto3.resource('s3')
     s3_resource.Object(s3_bucket, f'{s3_file_path}/{file_name}.csv').put(Body=csv_buffer.getvalue())
```

### Comparing `cpi_tools-0.2.4/cpi_tools/cpi_validation.py` & `cpi_tools-0.2.5/cpi_tools/cpi_validation.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-import pandas as pd
-import pandera as pa
-from cpi_tools import aws_tools
-import boto3
-import s3fs
-
-def get_valid_ref_values(ref_file, ref_column) -> list[str]:
-    """ Retrieve valid GLCF column values from ref table"""
-    ref_bucket = 'cpi-reference-data'
-    ref_file_path = 'cpi/processed'
-    ref_table = aws_tools.read_from_s3(ref_bucket, ref_file_path, ref_file)
-    return list(ref_table[ref_column].unique())
-
-
-def validate_glcf_data(df: pd.DataFrame, min_date: int = 2019, max_date:int = 2020) -> None:
-
-    '''
-    Input:
-
-    df: pandas DataFrame containing GLCF data to be validated
-    min_date (optional): integer representing the minimum year for valid data (default value is 2019)
-    max_date (optional): integer representing the maximum year for valid data (default value is 2020)
-
-    Returns: None
-
-    This function validates a pandas DataFrame containing GLCF data, ensuring that it conforms to a specified schema. 
-    The schema includes checks for valid values in various columns, such as sector, sub_sector, country, region, and institution type. 
-    The function uses the validate method from the pandas_schema library to validate the DataFrame against the schema, 
-    and raises an exception if the validation fails. If the validation is successful, the function prints a message 
-    indicating that the DataFrame is GLCF compatible.
-        
-    '''
-
-    # Get or define valid column values
-    valid_sector_values = get_valid_ref_values('ref_project_type', 'sector')
-    valid_sub_sector_values = get_valid_ref_values('ref_project_type', 'sub_sector')
-    valid_solution_values = get_valid_ref_values('ref_project_type', 'solution')
-    valid_country_values = get_valid_ref_values('ref_geog_list_cpi', 'country_cpi')
-    valid_region_values = get_valid_ref_values('ref_geog_list_cpi', 'region_cpi')
-    
-    valid_institution_type_layer2_values =  ["Bilateral DFI", "Commercial FI", 'Corporation', 'Export Credit Agency (ECA)',
-                            'Funds','Government', 'Household/Individual', 'Institutional Investors', 
-                            'Multilateral Climate Funds','Multilateral DFI','National DFI', 'Public Fund',
-                            'SOE', 'State-owned FI', 'Unknown']
-    
-    valid_institution_type_layer1_values = ['Public', 'Private']
-
-    valid_domestic_international_values = ['Domestic', 'International']
-
-    valid_use_values = ['Mitigation', 'Adaptation', 'Multiple Objectives']
-
-
-    # Define GLCF Schema
-    schema = pa.DataFrameSchema({
-        "id_glcf": pa.Column(str),
-        "data_source_id": pa.Column(str, required=False),
-        "data_source": pa.Column(str),
-        "year": pa.Column(int, checks=pa.Check.in_range(min_date, max_date)),
-        "project_name": pa.Column(str),
-        "project_description": pa.Column(str, nullable=True),
-        "country_origin_cpi": pa.Column(str, pa.Check.isin(valid_country_values)),
-        "region_origin_cpi": pa.Column(str, pa.Check.isin(valid_region_values)),
-        "oecd_origin_cpi": pa.Column(str),
-        "country_destination_cpi": pa.Column(str, pa.Check.isin(valid_country_values)),
-        "region_destination_cpi": pa.Column(str, pa.Check.isin(valid_region_values)),
-        "oecd_destination_cpi": pa.Column(str),
-        "institution_cpi": pa.Column(str),
-        "institution_type_layer1": pa.Column(str, pa.Check.isin(valid_institution_type_layer1_values)),
-        "institution_type_layer2": pa.Column(str, pa.Check.isin(valid_institution_type_layer2_values)),
-        "recipient_type_layer1": pa.Column(str),
-        "domestic_international": pa.Column(str, pa.Check.isin(valid_domestic_international_values)),
-        "value_USDm": pa.Column(float, pa.Check.ge(0)), #Greater than or equal to 0
-        "instrument_cpi": pa.Column(str),
-        "sector_original": pa.Column(str),
-        "sector_key_cpi": pa.Column(str),
-        "sector_cpi": pa.Column(str, checks=pa.Check.isin(valid_sector_values)),
-        "sub_sector_cpi": pa.Column(str, pa.Check.isin(valid_sub_sector_values)),
-        "solution_cpi": pa.Column(str, pa.Check.isin(valid_solution_values)),
-        "use_cpi": pa.Column(str, pa.Check.isin(valid_use_values)),
-        "gender_cpi": pa.Column(str),
-        "exclude_include": pa.Column(str)
-    })
-
-    # Attempt Validation
-    try:
-        schema.validate(df, lazy=True)
-        print('Dataframe GLCF Compatible')
-    except pa.errors.SchemaErrors as e:
-        #Display Errors upon validation failure
-        display(e.failure_cases)
-
-
-
-    
-    
-    
-    
-    
+import pandas as pd
+import pandera as pa
+from cpi_tools import aws_tools
+import boto3
+import s3fs
+
+def get_valid_ref_values(ref_file, ref_column) -> list[str]:
+    """ Retrieve valid GLCF column values from ref table"""
+    ref_bucket = 'cpi-reference-data'
+    ref_file_path = 'cpi/processed'
+    ref_table = aws_tools.read_from_s3(ref_bucket, ref_file_path, ref_file)
+    return list(ref_table[ref_column].unique())
+
+
+def validate_glcf_data(df: pd.DataFrame, min_date: int = 2019, max_date:int = 2020) -> None:
+
+    '''
+    Input:
+
+    df: pandas DataFrame containing GLCF data to be validated
+    min_date (optional): integer representing the minimum year for valid data (default value is 2019)
+    max_date (optional): integer representing the maximum year for valid data (default value is 2020)
+
+    Returns: None
+
+    This function validates a pandas DataFrame containing GLCF data, ensuring that it conforms to a specified schema. 
+    The schema includes checks for valid values in various columns, such as sector, sub_sector, country, region, and institution type. 
+    The function uses the validate method from the pandas_schema library to validate the DataFrame against the schema, 
+    and raises an exception if the validation fails. If the validation is successful, the function prints a message 
+    indicating that the DataFrame is GLCF compatible.
+        
+    '''
+
+    # Get or define valid column values
+    valid_sector_values = get_valid_ref_values('ref_project_type', 'sector')
+    valid_sub_sector_values = get_valid_ref_values('ref_project_type', 'sub_sector')
+    valid_solution_values = get_valid_ref_values('ref_project_type', 'solution')
+    valid_country_values = get_valid_ref_values('ref_geog_list_cpi', 'country_cpi')
+    valid_region_values = get_valid_ref_values('ref_geog_list_cpi', 'region_cpi')
+    
+    valid_institution_type_layer2_values =  ["Bilateral DFI", "Commercial FI", 'Corporation', 'Export Credit Agency (ECA)',
+                            'Funds','Government', 'Household/Individual', 'Institutional Investors', 
+                            'Multilateral Climate Funds','Multilateral DFI','National DFI', 'Public Fund',
+                            'SOE', 'State-owned FI', 'Unknown']
+    
+    valid_institution_type_layer1_values = ['Public', 'Private']
+
+    valid_domestic_international_values = ['Domestic', 'International']
+
+    valid_use_values = ['Mitigation', 'Adaptation', 'Multiple Objectives']
+
+
+    # Define GLCF Schema
+    schema = pa.DataFrameSchema({
+        "id_glcf": pa.Column(str),
+        "data_source_id": pa.Column(str, required=False),
+        "data_source": pa.Column(str),
+        "year": pa.Column(int, checks=pa.Check.in_range(min_date, max_date)),
+        "project_name": pa.Column(str),
+        "project_description": pa.Column(str, nullable=True),
+        "country_origin_cpi": pa.Column(str, pa.Check.isin(valid_country_values)),
+        "region_origin_cpi": pa.Column(str, pa.Check.isin(valid_region_values)),
+        "oecd_origin_cpi": pa.Column(str),
+        "country_destination_cpi": pa.Column(str, pa.Check.isin(valid_country_values)),
+        "region_destination_cpi": pa.Column(str, pa.Check.isin(valid_region_values)),
+        "oecd_destination_cpi": pa.Column(str),
+        "institution_cpi": pa.Column(str),
+        "institution_type_layer1": pa.Column(str, pa.Check.isin(valid_institution_type_layer1_values)),
+        "institution_type_layer2": pa.Column(str, pa.Check.isin(valid_institution_type_layer2_values)),
+        "recipient_type_layer1": pa.Column(str),
+        "domestic_international": pa.Column(str, pa.Check.isin(valid_domestic_international_values)),
+        "value_USDm": pa.Column(float, pa.Check.ge(0)), #Greater than or equal to 0
+        "instrument_cpi": pa.Column(str),
+        "sector_original": pa.Column(str),
+        "sector_key_cpi": pa.Column(str),
+        "sector_cpi": pa.Column(str, checks=pa.Check.isin(valid_sector_values)),
+        "sub_sector_cpi": pa.Column(str, pa.Check.isin(valid_sub_sector_values)),
+        "solution_cpi": pa.Column(str, pa.Check.isin(valid_solution_values)),
+        "use_cpi": pa.Column(str, pa.Check.isin(valid_use_values)),
+        "gender_cpi": pa.Column(str),
+        "exclude_include": pa.Column(str)
+    })
+
+    # Attempt Validation
+    try:
+        schema.validate(df, lazy=True)
+        print('Dataframe GLCF Compatible')
+    except pa.errors.SchemaErrors as e:
+        #Display Errors upon validation failure
+        display(e.failure_cases)
+
+
+
+    
+    
+    
+    
+
```

### Comparing `cpi_tools-0.2.4/cpi_tools/fuzzy_matching_cpi.py` & `cpi_tools-0.2.5/cpi_tools/fuzzy_matching_cpi.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,219 +1,219 @@
-# Import packages
-from io import StringIO
-import pandas as pd
-import numpy as np
-import string
-from unidecode import unidecode
-import warnings
-import time
-import s3fs
-import boto3
-import jaro  # pip install jaro-winkler
-
-# ------------------------------------
-# -- Define cleaning function
-# ------------------------------------
-
-
-def clean_entity_name(original_entity: str, remove_stop_words: bool = True):
-
-    clean_entity_name = str(original_entity)
-    clean_entity_name = clean_entity_name.lower()
-    clean_entity_name = clean_entity_name.split(" (")[0]
-    translator = str.maketrans("", "", string.punctuation)
-    clean_entity_name = clean_entity_name.translate(translator)
-    clean_entity_name = unidecode(clean_entity_name)
-
-    if remove_stop_words == True:
-        # Remove stop words
-        stop_words = [
-            "limited",
-            "ltd",
-            "ag",
-            "eg",
-            "spa",
-            "the",
-            "sa",
-            "ab",
-            "llc",
-            "llp",
-            "plc",
-            "inc",
-            "ltd",
-            "aktiengesellschaft",
-            "nv",
-            "a/s",
-            "oc",
-        ]
-        clean_entity_name = " ".join(
-            word for word in clean_entity_name.split() if word.lower() not in stop_words
-        )
-
-    return clean_entity_name
-
-
-# ------------------------------------
-# -- Define threshold function
-# ------------------------------------
-
-
-def dynamic_threshold(matching_scores: list, lower_threshold: float) -> float:
-
-    # Sort the pairs based on the scores in descending order
-    sorted_scores = sorted(matching_scores, reverse=True)
-    # Remove scores below the lower threshold set in the main function
-    sorted_scores = [x for x in sorted_scores if x >= lower_threshold]
-    # Compute the ratio between any two consecutive pairs of scores
-    score_ratios = [
-        sorted_scores[i] / sorted_scores[i + 1] for i in range(len(sorted_scores) - 1)
-    ]
-
-    return sorted_scores[(score_ratios.index(max(score_ratios)))]
-
-
-# ------------------------------------
-# -- Define manual input of
-# -- threshold function
-# ------------------------------------
-
-
-def threshold_check(
-    matched_scores: list, matched_entities: list, current_threshold: float
-) -> float:
-
-    # Zip the two lists together
-    combined_list = list(zip(matched_scores, matched_entities))
-    # Sort the pairs based on the scores in descending order
-    sorted_pairs = sorted(combined_list, reverse=True)
-    # Separate the sorted pairs back into two lists
-    sorted_scores, sorted_matches = zip(*sorted_pairs)
-
-    # Keep only those entities above the threshold
-    new_threshold = current_threshold
-    while new_threshold != "":
-        new_threshold = float(new_threshold)
-        scores_to_keep = [x for x in sorted_scores if x >= new_threshold]
-        matches_to_keep = sorted_matches[: len(scores_to_keep) + 1]
-        first_three_discared_matches = sorted_matches[
-            len(scores_to_keep) + 1 : len(scores_to_keep) + 4
-        ]
-        # matched_entities = [entity for entity, score in zip(matched_entities, matched_scores) if score > fixed_value]
-        new_threshold = input(
-            f"With a threshold of {calculated_threshold}, \
-			the last three retained matches are {matches_to_keep[-3:]}, \
-			while the first three discared ones are {first_three_discared_matches}. \
-			Please input the new desired threshold (leave blank if current one is acceptable)"
-        )
-
-    return new_threshold
-
-
-# ------------------------------------
-# -- Define fuzzy matching function
-# ------------------------------------
-
-
-def run_fuzzy_match(
-    entity_to_match: str,
-    search_list: list,
-    clean_names: bool = True,
-    multiple_matches: bool = False,
-    set_threshold_dynamically: bool = False,
-    lower_threshold: float = 0.8,
-) -> list:
-
-    if clean_names == True:  # perform round of cleaning of names
-        entity_to_match_clean = clean_entity_name(entity_to_match)
-        search_list_clean = [clean_entity_name(x) for x in search_list]
-    else:
-        entity_to_match_clean = entity_to_match
-        search_list_clean = search_list
-
-    # Initialize empty lists
-    matched_entities = []
-    matched_scores = []
-
-    # Compute a Jaro-Winkler score for each combination of entities
-    for i, s in enumerate(search_list_clean):
-        score = jaro.jaro_winkler_metric(entity_to_match_clean, s)
-        matched_entities.append(search_list[i])
-        matched_scores.append(score)
-
-    # Extract matches of interest on the basis of the various parameters
-    if multiple_matches == False:
-        # Retain highest score only
-        max_score = max(matched_scores)
-        if max_score >= lower_threshold:
-            matched_entities = matched_entities[
-                matched_scores.index(max(matched_scores))
-            ]
-            matched_scores = max_score
-        else:
-            matched_scores = []
-            matched_entities = []
-
-    elif (multiple_matches == True) & (set_threshold_dynamically == False):
-        matched_entities = [
-            entity
-            for entity, score in zip(matched_entities, matched_scores)
-            if score >= lower_threshold
-        ]
-        matched_scores = [x for x in matched_scores if x >= lower_threshold]
-
-    elif (multiple_matches == True) & (set_threshold_dynamically == True):
-        # Calculate the dynamic threshold
-        calculated_threshold = float(dynamic_threshold(matched_scores, lower_threshold))
-        # Zip the two lists together
-        combined_list = list(zip(matched_scores, matched_entities))
-        # Sort the pairs based on the scores in descending order
-        sorted_pairs = sorted(combined_list, reverse=True)
-        # Separate the sorted pairs back into two lists
-        sorted_scores, sorted_matches = zip(*sorted_pairs)
-        # Retain all scores above or equal to the calculated threshold
-        matched_scores = [x for x in sorted_scores if x >= calculated_threshold]
-        matched_entities = sorted_matches[: len(matched_scores)]
-
-    return matched_scores, matched_entities
-
-
-# ------------------------------------
-# -- Define master function
-# ------------------------------------
-
-
-def fuzzy_match_cpi(
-    dataframe_to_match: pd.DataFrame,
-    entity_column: str,
-    search_list: list,
-    clean_names: bool = True,
-    multiple_matches: bool = False,
-    set_threshold_dynamically: bool = False,
-    lower_threshold: float = 0.8,
-) -> pd.DataFrame:
-
-    # Apply function
-    results = dataframe_to_match[entity_column].apply(
-        run_fuzzy_match,
-        args=(
-            search_list,
-            clean_names,
-            multiple_matches,
-            set_threshold_dynamically,
-            lower_threshold,
-        ),
-    )
-
-    # Create two new columns to store the results
-    dataframe_to_match["Matched score"] = results.apply(lambda x: x[0])
-    dataframe_to_match["Matched entity"] = results.apply(lambda x: x[1])
-
-    return dataframe_to_match
-
-
-# Test
-# importpath = '/Users/nikitamarini/Desktop/CPI'
-# df = pd.read_csv(f'{importpath}/gfanz_entities.csv')
-# search_list_test = ['Ageas', 'ABN AMRO', 'Intesa San Paolo']
-
-# df = run_fuzzy_match(df, 'Entity', search_list_test)
-# print(df[df['Matched entity'].apply(len) > 0])
+# Import packages
+from io import StringIO
+import pandas as pd
+import numpy as np
+import string
+from unidecode import unidecode
+import warnings
+import time
+import s3fs
+import boto3
+import jaro  # pip install jaro-winkler
+
+# ------------------------------------
+# -- Define cleaning function
+# ------------------------------------
+
+
+def clean_entity_name(original_entity: str, remove_stop_words: bool = True):
+
+    clean_entity_name = str(original_entity)
+    clean_entity_name = clean_entity_name.lower()
+    clean_entity_name = clean_entity_name.split(" (")[0]
+    translator = str.maketrans("", "", string.punctuation)
+    clean_entity_name = clean_entity_name.translate(translator)
+    clean_entity_name = unidecode(clean_entity_name)
+
+    if remove_stop_words == True:
+        # Remove stop words
+        stop_words = [
+            "limited",
+            "ltd",
+            "ag",
+            "eg",
+            "spa",
+            "the",
+            "sa",
+            "ab",
+            "llc",
+            "llp",
+            "plc",
+            "inc",
+            "ltd",
+            "aktiengesellschaft",
+            "nv",
+            "a/s",
+            "oc",
+        ]
+        clean_entity_name = " ".join(
+            word for word in clean_entity_name.split() if word.lower() not in stop_words
+        )
+
+    return clean_entity_name
+
+
+# ------------------------------------
+# -- Define threshold function
+# ------------------------------------
+
+
+def dynamic_threshold(matching_scores: list, lower_threshold: float) -> float:
+
+    # Sort the pairs based on the scores in descending order
+    sorted_scores = sorted(matching_scores, reverse=True)
+    # Remove scores below the lower threshold set in the main function
+    sorted_scores = [x for x in sorted_scores if x >= lower_threshold]
+    # Compute the ratio between any two consecutive pairs of scores
+    score_ratios = [
+        sorted_scores[i] / sorted_scores[i + 1] for i in range(len(sorted_scores) - 1)
+    ]
+
+    return sorted_scores[(score_ratios.index(max(score_ratios)))]
+
+
+# ------------------------------------
+# -- Define manual input of
+# -- threshold function
+# ------------------------------------
+
+
+def threshold_check(
+    matched_scores: list, matched_entities: list, current_threshold: float
+) -> float:
+
+    # Zip the two lists together
+    combined_list = list(zip(matched_scores, matched_entities))
+    # Sort the pairs based on the scores in descending order
+    sorted_pairs = sorted(combined_list, reverse=True)
+    # Separate the sorted pairs back into two lists
+    sorted_scores, sorted_matches = zip(*sorted_pairs)
+
+    # Keep only those entities above the threshold
+    new_threshold = current_threshold
+    while new_threshold != "":
+        new_threshold = float(new_threshold)
+        scores_to_keep = [x for x in sorted_scores if x >= new_threshold]
+        matches_to_keep = sorted_matches[: len(scores_to_keep) + 1]
+        first_three_discared_matches = sorted_matches[
+            len(scores_to_keep) + 1 : len(scores_to_keep) + 4
+        ]
+        # matched_entities = [entity for entity, score in zip(matched_entities, matched_scores) if score > fixed_value]
+        new_threshold = input(
+            f"With a threshold of {calculated_threshold}, \
+			the last three retained matches are {matches_to_keep[-3:]}, \
+			while the first three discared ones are {first_three_discared_matches}. \
+			Please input the new desired threshold (leave blank if current one is acceptable)"
+        )
+
+    return new_threshold
+
+
+# ------------------------------------
+# -- Define fuzzy matching function
+# ------------------------------------
+
+
+def run_fuzzy_match(
+    entity_to_match: str,
+    search_list: list,
+    clean_names: bool = True,
+    multiple_matches: bool = False,
+    set_threshold_dynamically: bool = False,
+    lower_threshold: float = 0.8,
+) -> list:
+
+    if clean_names == True:  # perform round of cleaning of names
+        entity_to_match_clean = clean_entity_name(entity_to_match)
+        search_list_clean = [clean_entity_name(x) for x in search_list]
+    else:
+        entity_to_match_clean = entity_to_match
+        search_list_clean = search_list
+
+    # Initialize empty lists
+    matched_entities = []
+    matched_scores = []
+
+    # Compute a Jaro-Winkler score for each combination of entities
+    for i, s in enumerate(search_list_clean):
+        score = jaro.jaro_winkler_metric(entity_to_match_clean, s)
+        matched_entities.append(search_list[i])
+        matched_scores.append(score)
+
+    # Extract matches of interest on the basis of the various parameters
+    if multiple_matches == False:
+        # Retain highest score only
+        max_score = max(matched_scores)
+        if max_score >= lower_threshold:
+            matched_entities = matched_entities[
+                matched_scores.index(max(matched_scores))
+            ]
+            matched_scores = max_score
+        else:
+            matched_scores = []
+            matched_entities = []
+
+    elif (multiple_matches == True) & (set_threshold_dynamically == False):
+        matched_entities = [
+            entity
+            for entity, score in zip(matched_entities, matched_scores)
+            if score >= lower_threshold
+        ]
+        matched_scores = [x for x in matched_scores if x >= lower_threshold]
+
+    elif (multiple_matches == True) & (set_threshold_dynamically == True):
+        # Calculate the dynamic threshold
+        calculated_threshold = float(dynamic_threshold(matched_scores, lower_threshold))
+        # Zip the two lists together
+        combined_list = list(zip(matched_scores, matched_entities))
+        # Sort the pairs based on the scores in descending order
+        sorted_pairs = sorted(combined_list, reverse=True)
+        # Separate the sorted pairs back into two lists
+        sorted_scores, sorted_matches = zip(*sorted_pairs)
+        # Retain all scores above or equal to the calculated threshold
+        matched_scores = [x for x in sorted_scores if x >= calculated_threshold]
+        matched_entities = sorted_matches[: len(matched_scores)]
+
+    return matched_scores, matched_entities
+
+
+# ------------------------------------
+# -- Define master function
+# ------------------------------------
+
+
+def fuzzy_match_cpi(
+    dataframe_to_match: pd.DataFrame,
+    entity_column: str,
+    search_list: list,
+    clean_names: bool = True,
+    multiple_matches: bool = False,
+    set_threshold_dynamically: bool = False,
+    lower_threshold: float = 0.8,
+) -> pd.DataFrame:
+
+    # Apply function
+    results = dataframe_to_match[entity_column].apply(
+        run_fuzzy_match,
+        args=(
+            search_list,
+            clean_names,
+            multiple_matches,
+            set_threshold_dynamically,
+            lower_threshold,
+        ),
+    )
+
+    # Create two new columns to store the results
+    dataframe_to_match["Matched score"] = results.apply(lambda x: x[0])
+    dataframe_to_match["Matched entity"] = results.apply(lambda x: x[1])
+
+    return dataframe_to_match
+
+
+# Test
+# importpath = '/Users/nikitamarini/Desktop/CPI'
+# df = pd.read_csv(f'{importpath}/gfanz_entities.csv')
+# search_list_test = ['Ageas', 'ABN AMRO', 'Intesa San Paolo']
+
+# df = run_fuzzy_match(df, 'Entity', search_list_test)
+# print(df[df['Matched entity'].apply(len) > 0])
```

### Comparing `cpi_tools-0.2.4/cpi_tools/tracking_processing_tools.py` & `cpi_tools-0.2.5/cpi_tools/tracking_processing_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,14 +253,17 @@
                            'ref_ownership')
 
     process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='sector'),
                            'ref_sector', 'SQL Field Name')
 
     process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='soe'),
                            'ref_soe', 'SQL Field Name')
+    
+    process_reference_data(pd.read_excel(f's3://{S3_REFERENCE_BUCKET}/{s3_file_path}/{file_name}', sheet_name='data_source'),
+                           'ref_data_source')
 
     return None
 
 
 def update_ref_tables():
     """
     This function updates reference tables by reading a master reference table from Dropbox,
@@ -346,12 +349,15 @@
     ref_sector = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_sector.csv', encoding='utf-8')
     
     # Instrument table
     ref_instr = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_instr.csv', encoding='utf-8')
     
     # Recipient table
     ref_recipient = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_recipient.csv', encoding='utf-8')
+    
+    # Data source
+    ref_data_source = pd.read_csv(f's3://{S3_REFERENCE_BUCKET}/{cpi_reference_folder}/ref_data_source.csv', encoding='utf-8')
 
     # Return all the DataFrames as a tuple
     return ref_geog_list_all, ref_coeff, ref_fx, ref_gender, ref_geog_list_all, ref_geog_list_cpi, ref_institution_list_all, \
-    ref_institution_list_cpi, ref_ownership, ref_project_type, ref_sector, ref_instr, ref_recipient
+    ref_institution_list_cpi, ref_ownership, ref_project_type, ref_sector, ref_instr, ref_recipient, ref_data_source
```

