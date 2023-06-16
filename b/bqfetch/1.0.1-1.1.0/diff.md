# Comparing `tmp/bqfetch-1.0.1.tar.gz` & `tmp/bqfetch-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bqfetch-1.0.1.tar", last modified: Wed Aug 18 14:16:15 2021, max compression
+gzip compressed data, was "bqfetch-1.1.0.tar", last modified: Fri Jun 16 12:50:21 2023, max compression
```

## Comparing `bqfetch-1.0.1.tar` & `bqfetch-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tristanbilot   (501) staff       (20)        0 2021-08-18 14:16:15.953325 bqfetch-1.0.1/
--rw-r--r--   0 tristanbilot   (501) staff       (20)     1070 2021-08-17 09:52:05.000000 bqfetch-1.0.1/LICENSE
--rw-r--r--   0 tristanbilot   (501) staff       (20)     7238 2021-08-18 14:16:15.953503 bqfetch-1.0.1/PKG-INFO
--rw-r--r--   0 tristanbilot   (501) staff       (20)     6732 2021-08-18 14:02:28.000000 bqfetch-1.0.1/README.md
-drwxr-xr-x   0 tristanbilot   (501) staff       (20)        0 2021-08-18 14:16:15.951490 bqfetch-1.0.1/bqfetch/
--rw-r--r--   0 tristanbilot   (501) staff       (20)        0 2021-07-28 14:44:26.000000 bqfetch-1.0.1/bqfetch/__init__.py
--rw-r--r--   0 tristanbilot   (501) staff       (20)    19612 2021-08-18 13:10:28.000000 bqfetch-1.0.1/bqfetch/bqfetch.py
--rw-r--r--   0 tristanbilot   (501) staff       (20)     2589 2021-08-17 15:46:28.000000 bqfetch-1.0.1/bqfetch/utils.py
-drwxr-xr-x   0 tristanbilot   (501) staff       (20)        0 2021-08-18 14:16:15.953068 bqfetch-1.0.1/bqfetch.egg-info/
--rw-r--r--   0 tristanbilot   (501) staff       (20)     7238 2021-08-18 14:16:15.000000 bqfetch-1.0.1/bqfetch.egg-info/PKG-INFO
--rw-r--r--   0 tristanbilot   (501) staff       (20)      222 2021-08-18 14:16:15.000000 bqfetch-1.0.1/bqfetch.egg-info/SOURCES.txt
--rw-r--r--   0 tristanbilot   (501) staff       (20)        1 2021-08-18 14:16:15.000000 bqfetch-1.0.1/bqfetch.egg-info/dependency_links.txt
--rw-r--r--   0 tristanbilot   (501) staff       (20)        8 2021-08-18 14:16:15.000000 bqfetch-1.0.1/bqfetch.egg-info/top_level.txt
--rw-r--r--   0 tristanbilot   (501) staff       (20)      287 2021-08-18 13:31:18.000000 bqfetch-1.0.1/pyproject.toml
--rw-r--r--   0 tristanbilot   (501) staff       (20)      558 2021-08-18 14:16:15.954191 bqfetch-1.0.1/setup.cfg
+drwxr-xr-x   0 tb         (501) staff       (20)        0 2023-06-16 12:50:21.078643 bqfetch-1.1.0/
+-rw-r--r--   0 tb         (501) staff       (20)     1070 2023-06-16 12:37:19.000000 bqfetch-1.1.0/LICENSE
+-rw-r--r--   0 tb         (501) staff       (20)     6812 2023-06-16 12:50:21.078716 bqfetch-1.1.0/PKG-INFO
+-rw-r--r--   0 tb         (501) staff       (20)     6343 2023-06-16 12:37:19.000000 bqfetch-1.1.0/README.md
+drwxr-xr-x   0 tb         (501) staff       (20)        0 2023-06-16 12:50:21.077955 bqfetch-1.1.0/bqfetch/
+-rw-r--r--   0 tb         (501) staff       (20)      273 2023-06-16 12:37:19.000000 bqfetch-1.1.0/bqfetch/__init__.py
+-rw-r--r--   0 tb         (501) staff       (20)    19744 2023-06-16 12:37:19.000000 bqfetch-1.1.0/bqfetch/bqfetch.py
+-rw-r--r--   0 tb         (501) staff       (20)     2589 2023-06-16 12:37:19.000000 bqfetch-1.1.0/bqfetch/utils.py
+drwxr-xr-x   0 tb         (501) staff       (20)        0 2023-06-16 12:50:21.078545 bqfetch-1.1.0/bqfetch.egg-info/
+-rw-r--r--   0 tb         (501) staff       (20)     6812 2023-06-16 12:50:21.000000 bqfetch-1.1.0/bqfetch.egg-info/PKG-INFO
+-rw-r--r--   0 tb         (501) staff       (20)      222 2023-06-16 12:50:21.000000 bqfetch-1.1.0/bqfetch.egg-info/SOURCES.txt
+-rw-r--r--   0 tb         (501) staff       (20)        1 2023-06-16 12:50:21.000000 bqfetch-1.1.0/bqfetch.egg-info/dependency_links.txt
+-rw-r--r--   0 tb         (501) staff       (20)        8 2023-06-16 12:50:21.000000 bqfetch-1.1.0/bqfetch.egg-info/top_level.txt
+-rw-rw-r--   0 tb         (501) staff       (20)      287 2023-06-16 12:49:21.000000 bqfetch-1.1.0/pyproject.toml
+-rw-rw-r--   0 tb         (501) staff       (20)      558 2023-06-16 12:50:21.079040 bqfetch-1.1.0/setup.cfg
```

### Comparing `bqfetch-1.0.1/LICENSE` & `bqfetch-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bqfetch-1.0.1/PKG-INFO` & `bqfetch-1.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: bqfetch
-Version: 1.0.1
+Version: 1.1.0
 Summary: A tool to fetch tables from BigQuery as pandas DataFrames, fast.
 Home-page: https://github.com/TristanBilot/bqfetch
 Author: Tristan Bilot
 Author-email: bilot.tristan@hotmail.fr
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -22,15 +20,15 @@
   <a href=""><img src="https://img.shields.io/github/release-date/tristanbilot/bqfetch" alt="Release date"></a>
   <br>
   <a href=""><img src="https://img.shields.io/badge/Python-%3E%3D3.6-blue" alt="Python version"></a>
   <a href=""><img src="https://img.shields.io/github/license/tristanbilot/bqfetch" alt="Python version"></a>
 </p>
 
 # <p align="center">bqfetch<p>
-**A lightweight tool to fetch tables from BigQuery as pandas DataFrames very fast using BigQuery Storage API combined with multiprocessing.**
+**A lightweight tool to fetch tables from BigQuery as pandas DataFrames very fast using BigQuery Storage API combined with multiprocessing. This module also aims to fetch large tables that cannot fit into memory, by chunking the table in a smart and scalable way.**
 
 
 ## Installation
 ```
 pip install bqfetch
 pip install -r requirements.txt
 ```
@@ -53,64 +51,64 @@
 |  id |   Name  | Age |
 |:---:|:-------:|:---:|
 | 187 | Bartolomé |  30 |
 | 188 | Tristan |  22 |
 | ... |   ...   | ... |
 
 ```python
->>> table = BigQueryTable("my_project", "dataset1", "users_table")
+>>> table = BigQueryTable("PROJECT", "DATASET", "TABLE")
 >>> fetcher = BigQueryFetcher('/path/to/service_account.json', table)
->>> nb_chunks = 10
->>> chunks = fetcher.chunks('id', nb_chunks)
+>>> chunks = fetcher.chunks('id', by_chunk_size_in_GB=5)
 
 >>> for chunk in chunks:
         df = fetcher.fetch(chunk, nb_cores=-1, parallel_backend='billiard')
         # ...
 ```
   
 * First, we have to create a `BigQueryTable` object which contains the path to the BigQuery table stored in GCP.
 * A fetcher is created, given in parameter the absolute path to the service_account.json file, the file is mandatory in order to do operations in GCP.
-* Define the number of chunks to divide the table. Ex: if `nb_chunks` is set to 10, then the whole values in the index column will be fetched and divised in 10. However, setting `nb_chunks` to 10 does not mean that the table will necessarly be divided equally in 10 parts because some values in the index column can appear more than other and vice versa, causing that a value containing multiple row will be considered the same as a value containing only one row in the table.
-* Chunk the whole table, given the `column` name and the chunk size. In this case, choosing the **id** column is perfect because this each value of this column appears the same number of times: 1 time.
+* Chunks the whole table, given the `column` name and the chunk size. In this case, choosing the **id** column is perfect because this each value of this column appears the same number of times: 1 time. Concerning the chunks size, if by_chunk_size_in_GB=5, each chunk that will be fetched on the machine will be of size 5GB. Thus it has to fit into memory. You need to save 1/3 more memory because the size of a DataFrame object is larger than the raw fetched data.
 * For each chunk, fetch it.
     * `nb_cores`=-1 will use the number of cores available on the machine.
     * `parallel_backend`='billiard' | 'joblib' | 'multiprocessing' specify the backend framework to use.
 
-## Chunk size approximation function
-In some cases, choosing the good `chunk_size` can be difficult, so a function is available to approximate the perfect size to chunk the table. However, this function will throw if there is too much variance between the number of values in the index column (if more than 25% of the values appear more or less than 25% of the mean of the appearance of all the values in the column).
+## Fetch by number of chunks
+It is also possible to use `by_nb_chunks` instead of `by_chunk_size_in_GB`. It will divided the table in N, so you cannot control more flexibly the size of each chunk.
   
 ```python
->>> table = BigQueryTable("my_project", "dataset1", "users_table")
+>>> table = BigQueryTable("PROJECT", "DATASET", "TABLE")
 >>> fetcher = BigQueryFetcher('/path/to/service_account.json', table)
->>> perfect_nb_chunks = fetcher.get_chunk_size_approximation('id')
->>> chunks = fetcher.chunks('id', perfect_nb_chunks)
+>>> chunks = fetcher.chunks('id', by_nb_chunks=10)
+
+>>> for chunk in chunks:
+        df = fetcher.fetch(chunk, nb_cores=-1, parallel_backend='billiard')
+        # ...
 ```
 
 ## Verbose mode
 
 ```python
->>> perfect_nb_chunks = fetcher.get_chunk_size_approximation('barcode', verbose=True)
+>>> chunks = fetcher.chunks(column='id', by_nb_chunks=1, verbose=True)
 # Available memory on device:  7.04GB
 # Size of table:               2.19GB
 # Prefered size of chunk:      3GB
 # Size per chunk:              3GB
-# Chunk size approximation:    1
-
->>> chunks = fetcher.chunks(column='id', chunk_size=perfect_nb_chunks, verbose=True)
+# Nb chunks:                   1
+  
 # Nb values in "id":           96
-# Chunk size:                  1GB
+# Chunk size:                  3GB
 # Nb chunks:                   1
   
 >>> for chunk in chunks:
 >>>        df = fetcher.fetch(chunk=chunk, nb_cores=1, parallel_backend='joblib', verbose=True)
 # Use multiprocessing :        False
 # Nb cores:                    1
 # Parallel backend:            joblib
 
-# Time to fetch:               102.21s
+# Time to fetch:               43.21s
 # Nb lines in dataframe:       3375875
 # Size of dataframe:           2.83GB
 ```
   
 ## Warning
 We recommend to use this tool only in the case where the table to fetch contains a column that can be easily chunked (divided in small parts). Thus the perfect column to achieve this is a column containing distinct values or values that appear ~ the same number of time. **If some values appear thousands of times and some only fews, then the chunking will not be reliable** because we need to make the assumption that each chunk will be approximatively the same size in order to estimate the needed memory necessary to fetch in an optimize way the table.
   
@@ -143,9 +141,7 @@
 ## Contribution
 bqfetch is open to new contributors, especially for bug fixing or implementation of new features. Do not hesitate to open an issue/pull request :)
   
 ## License
   <a href="https://opensource.org/licenses/MIT">MIT</a>
   
   Copyright (c) 2021-present, Tristan Bilot
-
-
```

#### html2text {}

```diff
@@ -1,71 +1,65 @@
-Metadata-Version: 2.1 Name: bqfetch Version: 1.0.1 Summary: A tool to fetch
+Metadata-Version: 2.1 Name: bqfetch Version: 1.1.0 Summary: A tool to fetch
 tables from BigQuery as pandas DataFrames, fast. Home-page: https://github.com/
 TristanBilot/bqfetch Author: Tristan Bilot Author-email:
-bilot.tristan@hotmail.fr License: UNKNOWN Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE
+bilot.tristan@hotmail.fr Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
+markdown License-File: LICENSE
     [https://raw.githubusercontent.com/TristanBilot/bqfetch/master/.github/
                                    logo.svg]
                    [Last commit] [Languages] [Release date]
                        [Python version] [Python version]
 #
                                     bqfetch
 **A lightweight tool to fetch tables from BigQuery as pandas DataFrames very
-fast using BigQuery Storage API combined with multiprocessing.** ##
-Installation ``` pip install bqfetch pip install -r requirements.txt ``` ##
-Algorithm * Fetch all distinct values from the given index `column`. * Divide
-these indices in `chunks` based on the available memory and the number of cores
-on the machine. * `If multiprocessing`: * Each chunk will be divided in
-multiple sub-chunks based on the parameter `nb_cores` and the available memory.
-* For each sub-chunk, create a temporary table containing all the matching rows
-in the whole table. * Fetch these temporary tables using BigQuery Storage as
-dataframes. * Merge the dataframes. * Delete temporary tables. * `If
-!multiprocessing`: * Same process with only one temporary table and no parallel
-processes created. ## Use case ### Fetching a huge table of users using
-multiple cores | id | Name | Age | |:---:|:-------:|:---:| | 187 | BartolomÃ© |
-30 | | 188 | Tristan | 22 | | ... | ... | ... | ```python >>> table =
-BigQueryTable("my_project", "dataset1", "users_table") >>> fetcher =
-BigQueryFetcher('/path/to/service_account.json', table) >>> nb_chunks = 10 >>>
-chunks = fetcher.chunks('id', nb_chunks) >>> for chunk in chunks: df =
-fetcher.fetch(chunk, nb_cores=-1, parallel_backend='billiard') # ... ``` *
+fast using BigQuery Storage API combined with multiprocessing. This module also
+aims to fetch large tables that cannot fit into memory, by chunking the table
+in a smart and scalable way.** ## Installation ``` pip install bqfetch pip
+install -r requirements.txt ``` ## Algorithm * Fetch all distinct values from
+the given index `column`. * Divide these indices in `chunks` based on the
+available memory and the number of cores on the machine. * `If
+multiprocessing`: * Each chunk will be divided in multiple sub-chunks based on
+the parameter `nb_cores` and the available memory. * For each sub-chunk, create
+a temporary table containing all the matching rows in the whole table. * Fetch
+these temporary tables using BigQuery Storage as dataframes. * Merge the
+dataframes. * Delete temporary tables. * `If !multiprocessing`: * Same process
+with only one temporary table and no parallel processes created. ## Use case
+### Fetching a huge table of users using multiple cores | id | Name | Age | |:-
+--:|:-------:|:---:| | 187 | BartolomÃ© | 30 | | 188 | Tristan | 22 | | ... |
+... | ... | ```python >>> table = BigQueryTable("PROJECT", "DATASET", "TABLE")
+>>> fetcher = BigQueryFetcher('/path/to/service_account.json', table) >>>
+chunks = fetcher.chunks('id', by_chunk_size_in_GB=5) >>> for chunk in chunks:
+df = fetcher.fetch(chunk, nb_cores=-1, parallel_backend='billiard') # ... ``` *
 First, we have to create a `BigQueryTable` object which contains the path to
 the BigQuery table stored in GCP. * A fetcher is created, given in parameter
 the absolute path to the service_account.json file, the file is mandatory in
-order to do operations in GCP. * Define the number of chunks to divide the
-table. Ex: if `nb_chunks` is set to 10, then the whole values in the index
-column will be fetched and divised in 10. However, setting `nb_chunks` to 10
-does not mean that the table will necessarly be divided equally in 10 parts
-because some values in the index column can appear more than other and vice
-versa, causing that a value containing multiple row will be considered the same
-as a value containing only one row in the table. * Chunk the whole table, given
-the `column` name and the chunk size. In this case, choosing the **id** column
-is perfect because this each value of this column appears the same number of
-times: 1 time. * For each chunk, fetch it. * `nb_cores`=-1 will use the number
-of cores available on the machine. * `parallel_backend`='billiard' | 'joblib' |
-'multiprocessing' specify the backend framework to use. ## Chunk size
-approximation function In some cases, choosing the good `chunk_size` can be
-difficult, so a function is available to approximate the perfect size to chunk
-the table. However, this function will throw if there is too much variance
-between the number of values in the index column (if more than 25% of the
-values appear more or less than 25% of the mean of the appearance of all the
-values in the column). ```python >>> table = BigQueryTable("my_project",
-"dataset1", "users_table") >>> fetcher = BigQueryFetcher('/path/to/
-service_account.json', table) >>> perfect_nb_chunks =
-fetcher.get_chunk_size_approximation('id') >>> chunks = fetcher.chunks('id',
-perfect_nb_chunks) ``` ## Verbose mode ```python >>> perfect_nb_chunks =
-fetcher.get_chunk_size_approximation('barcode', verbose=True) # Available
-memory on device: 7.04GB # Size of table: 2.19GB # Prefered size of chunk: 3GB
-# Size per chunk: 3GB # Chunk size approximation: 1 >>> chunks = fetcher.chunks
-(column='id', chunk_size=perfect_nb_chunks, verbose=True) # Nb values in "id":
-96 # Chunk size: 1GB # Nb chunks: 1 >>> for chunk in chunks: >>> df =
+order to do operations in GCP. * Chunks the whole table, given the `column`
+name and the chunk size. In this case, choosing the **id** column is perfect
+because this each value of this column appears the same number of times: 1
+time. Concerning the chunks size, if by_chunk_size_in_GB=5, each chunk that
+will be fetched on the machine will be of size 5GB. Thus it has to fit into
+memory. You need to save 1/3 more memory because the size of a DataFrame object
+is larger than the raw fetched data. * For each chunk, fetch it. * `nb_cores`=-
+1 will use the number of cores available on the machine. *
+`parallel_backend`='billiard' | 'joblib' | 'multiprocessing' specify the
+backend framework to use. ## Fetch by number of chunks It is also possible to
+use `by_nb_chunks` instead of `by_chunk_size_in_GB`. It will divided the table
+in N, so you cannot control more flexibly the size of each chunk. ```python >>>
+table = BigQueryTable("PROJECT", "DATASET", "TABLE") >>> fetcher =
+BigQueryFetcher('/path/to/service_account.json', table) >>> chunks =
+fetcher.chunks('id', by_nb_chunks=10) >>> for chunk in chunks: df =
+fetcher.fetch(chunk, nb_cores=-1, parallel_backend='billiard') # ... ``` ##
+Verbose mode ```python >>> chunks = fetcher.chunks(column='id', by_nb_chunks=1,
+verbose=True) # Available memory on device: 7.04GB # Size of table: 2.19GB #
+Prefered size of chunk: 3GB # Size per chunk: 3GB # Nb chunks: 1 # Nb values in
+"id": 96 # Chunk size: 3GB # Nb chunks: 1 >>> for chunk in chunks: >>> df =
 fetcher.fetch(chunk=chunk, nb_cores=1, parallel_backend='joblib', verbose=True)
 # Use multiprocessing : False # Nb cores: 1 # Parallel backend: joblib # Time
-to fetch: 102.21s # Nb lines in dataframe: 3375875 # Size of dataframe: 2.83GB
+to fetch: 43.21s # Nb lines in dataframe: 3375875 # Size of dataframe: 2.83GB
 ``` ## Warning We recommend to use this tool only in the case where the table
 to fetch contains a column that can be easily chunked (divided in small parts).
 Thus the perfect column to achieve this is a column containing distinct values
 or values that appear ~ the same number of time. **If some values appear
 thousands of times and some only fews, then the chunking will not be reliable**
 because we need to make the assumption that each chunk will be approximatively
 the same size in order to estimate the needed memory necessary to fetch in an
```

### Comparing `bqfetch-1.0.1/README.md` & `bqfetch-1.1.0/bqfetch.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,34 @@
+Metadata-Version: 2.1
+Name: bqfetch
+Version: 1.1.0
+Summary: A tool to fetch tables from BigQuery as pandas DataFrames, fast.
+Home-page: https://github.com/TristanBilot/bqfetch
+Author: Tristan Bilot
+Author-email: bilot.tristan@hotmail.fr
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center"><img width="15%" src="https://raw.githubusercontent.com/TristanBilot/bqfetch/master/.github/logo.svg"/></p>
 
 <p align="center">
   <a href=""><img src="https://img.shields.io/github/last-commit/tristanbilot/bqfetch" alt="Last commit"></a>
   <a href="https://img.shields.io/github/languages/count/tristanbilot/bqfetch"><img src="https://img.shields.io/github/languages/count/tristanbilot/bqfetch" alt="Languages"></a>
   <a href=""><img src="https://img.shields.io/github/release-date/tristanbilot/bqfetch" alt="Release date"></a>
   <br>
   <a href=""><img src="https://img.shields.io/badge/Python-%3E%3D3.6-blue" alt="Python version"></a>
   <a href=""><img src="https://img.shields.io/github/license/tristanbilot/bqfetch" alt="Python version"></a>
 </p>
 
 # <p align="center">bqfetch<p>
-**A lightweight tool to fetch tables from BigQuery as pandas DataFrames very fast using BigQuery Storage API combined with multiprocessing.**
+**A lightweight tool to fetch tables from BigQuery as pandas DataFrames very fast using BigQuery Storage API combined with multiprocessing. This module also aims to fetch large tables that cannot fit into memory, by chunking the table in a smart and scalable way.**
 
 
 ## Installation
 ```
 pip install bqfetch
 pip install -r requirements.txt
 ```
@@ -37,64 +51,64 @@
 |  id |   Name  | Age |
 |:---:|:-------:|:---:|
 | 187 | Bartolomé |  30 |
 | 188 | Tristan |  22 |
 | ... |   ...   | ... |
 
 ```python
->>> table = BigQueryTable("my_project", "dataset1", "users_table")
+>>> table = BigQueryTable("PROJECT", "DATASET", "TABLE")
 >>> fetcher = BigQueryFetcher('/path/to/service_account.json', table)
->>> nb_chunks = 10
->>> chunks = fetcher.chunks('id', nb_chunks)
+>>> chunks = fetcher.chunks('id', by_chunk_size_in_GB=5)
 
 >>> for chunk in chunks:
         df = fetcher.fetch(chunk, nb_cores=-1, parallel_backend='billiard')
         # ...
 ```
   
 * First, we have to create a `BigQueryTable` object which contains the path to the BigQuery table stored in GCP.
 * A fetcher is created, given in parameter the absolute path to the service_account.json file, the file is mandatory in order to do operations in GCP.
-* Define the number of chunks to divide the table. Ex: if `nb_chunks` is set to 10, then the whole values in the index column will be fetched and divised in 10. However, setting `nb_chunks` to 10 does not mean that the table will necessarly be divided equally in 10 parts because some values in the index column can appear more than other and vice versa, causing that a value containing multiple row will be considered the same as a value containing only one row in the table.
-* Chunk the whole table, given the `column` name and the chunk size. In this case, choosing the **id** column is perfect because this each value of this column appears the same number of times: 1 time.
+* Chunks the whole table, given the `column` name and the chunk size. In this case, choosing the **id** column is perfect because this each value of this column appears the same number of times: 1 time. Concerning the chunks size, if by_chunk_size_in_GB=5, each chunk that will be fetched on the machine will be of size 5GB. Thus it has to fit into memory. You need to save 1/3 more memory because the size of a DataFrame object is larger than the raw fetched data.
 * For each chunk, fetch it.
     * `nb_cores`=-1 will use the number of cores available on the machine.
     * `parallel_backend`='billiard' | 'joblib' | 'multiprocessing' specify the backend framework to use.
 
-## Chunk size approximation function
-In some cases, choosing the good `chunk_size` can be difficult, so a function is available to approximate the perfect size to chunk the table. However, this function will throw if there is too much variance between the number of values in the index column (if more than 25% of the values appear more or less than 25% of the mean of the appearance of all the values in the column).
+## Fetch by number of chunks
+It is also possible to use `by_nb_chunks` instead of `by_chunk_size_in_GB`. It will divided the table in N, so you cannot control more flexibly the size of each chunk.
   
 ```python
->>> table = BigQueryTable("my_project", "dataset1", "users_table")
+>>> table = BigQueryTable("PROJECT", "DATASET", "TABLE")
 >>> fetcher = BigQueryFetcher('/path/to/service_account.json', table)
->>> perfect_nb_chunks = fetcher.get_chunk_size_approximation('id')
->>> chunks = fetcher.chunks('id', perfect_nb_chunks)
+>>> chunks = fetcher.chunks('id', by_nb_chunks=10)
+
+>>> for chunk in chunks:
+        df = fetcher.fetch(chunk, nb_cores=-1, parallel_backend='billiard')
+        # ...
 ```
 
 ## Verbose mode
 
 ```python
->>> perfect_nb_chunks = fetcher.get_chunk_size_approximation('barcode', verbose=True)
+>>> chunks = fetcher.chunks(column='id', by_nb_chunks=1, verbose=True)
 # Available memory on device:  7.04GB
 # Size of table:               2.19GB
 # Prefered size of chunk:      3GB
 # Size per chunk:              3GB
-# Chunk size approximation:    1
-
->>> chunks = fetcher.chunks(column='id', chunk_size=perfect_nb_chunks, verbose=True)
+# Nb chunks:                   1
+  
 # Nb values in "id":           96
-# Chunk size:                  1GB
+# Chunk size:                  3GB
 # Nb chunks:                   1
   
 >>> for chunk in chunks:
 >>>        df = fetcher.fetch(chunk=chunk, nb_cores=1, parallel_backend='joblib', verbose=True)
 # Use multiprocessing :        False
 # Nb cores:                    1
 # Parallel backend:            joblib
 
-# Time to fetch:               102.21s
+# Time to fetch:               43.21s
 # Nb lines in dataframe:       3375875
 # Size of dataframe:           2.83GB
 ```
   
 ## Warning
 We recommend to use this tool only in the case where the table to fetch contains a column that can be easily chunked (divided in small parts). Thus the perfect column to achieve this is a column containing distinct values or values that appear ~ the same number of time. **If some values appear thousands of times and some only fews, then the chunking will not be reliable** because we need to make the assumption that each chunk will be approximatively the same size in order to estimate the needed memory necessary to fetch in an optimize way the table.
```

#### html2text {}

```diff
@@ -1,64 +1,65 @@
+Metadata-Version: 2.1 Name: bqfetch Version: 1.1.0 Summary: A tool to fetch
+tables from BigQuery as pandas DataFrames, fast. Home-page: https://github.com/
+TristanBilot/bqfetch Author: Tristan Bilot Author-email:
+bilot.tristan@hotmail.fr Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
+markdown License-File: LICENSE
     [https://raw.githubusercontent.com/TristanBilot/bqfetch/master/.github/
                                    logo.svg]
                    [Last commit] [Languages] [Release date]
                        [Python version] [Python version]
 #
                                     bqfetch
 **A lightweight tool to fetch tables from BigQuery as pandas DataFrames very
-fast using BigQuery Storage API combined with multiprocessing.** ##
-Installation ``` pip install bqfetch pip install -r requirements.txt ``` ##
-Algorithm * Fetch all distinct values from the given index `column`. * Divide
-these indices in `chunks` based on the available memory and the number of cores
-on the machine. * `If multiprocessing`: * Each chunk will be divided in
-multiple sub-chunks based on the parameter `nb_cores` and the available memory.
-* For each sub-chunk, create a temporary table containing all the matching rows
-in the whole table. * Fetch these temporary tables using BigQuery Storage as
-dataframes. * Merge the dataframes. * Delete temporary tables. * `If
-!multiprocessing`: * Same process with only one temporary table and no parallel
-processes created. ## Use case ### Fetching a huge table of users using
-multiple cores | id | Name | Age | |:---:|:-------:|:---:| | 187 | BartolomÃ© |
-30 | | 188 | Tristan | 22 | | ... | ... | ... | ```python >>> table =
-BigQueryTable("my_project", "dataset1", "users_table") >>> fetcher =
-BigQueryFetcher('/path/to/service_account.json', table) >>> nb_chunks = 10 >>>
-chunks = fetcher.chunks('id', nb_chunks) >>> for chunk in chunks: df =
-fetcher.fetch(chunk, nb_cores=-1, parallel_backend='billiard') # ... ``` *
+fast using BigQuery Storage API combined with multiprocessing. This module also
+aims to fetch large tables that cannot fit into memory, by chunking the table
+in a smart and scalable way.** ## Installation ``` pip install bqfetch pip
+install -r requirements.txt ``` ## Algorithm * Fetch all distinct values from
+the given index `column`. * Divide these indices in `chunks` based on the
+available memory and the number of cores on the machine. * `If
+multiprocessing`: * Each chunk will be divided in multiple sub-chunks based on
+the parameter `nb_cores` and the available memory. * For each sub-chunk, create
+a temporary table containing all the matching rows in the whole table. * Fetch
+these temporary tables using BigQuery Storage as dataframes. * Merge the
+dataframes. * Delete temporary tables. * `If !multiprocessing`: * Same process
+with only one temporary table and no parallel processes created. ## Use case
+### Fetching a huge table of users using multiple cores | id | Name | Age | |:-
+--:|:-------:|:---:| | 187 | BartolomÃ© | 30 | | 188 | Tristan | 22 | | ... |
+... | ... | ```python >>> table = BigQueryTable("PROJECT", "DATASET", "TABLE")
+>>> fetcher = BigQueryFetcher('/path/to/service_account.json', table) >>>
+chunks = fetcher.chunks('id', by_chunk_size_in_GB=5) >>> for chunk in chunks:
+df = fetcher.fetch(chunk, nb_cores=-1, parallel_backend='billiard') # ... ``` *
 First, we have to create a `BigQueryTable` object which contains the path to
 the BigQuery table stored in GCP. * A fetcher is created, given in parameter
 the absolute path to the service_account.json file, the file is mandatory in
-order to do operations in GCP. * Define the number of chunks to divide the
-table. Ex: if `nb_chunks` is set to 10, then the whole values in the index
-column will be fetched and divised in 10. However, setting `nb_chunks` to 10
-does not mean that the table will necessarly be divided equally in 10 parts
-because some values in the index column can appear more than other and vice
-versa, causing that a value containing multiple row will be considered the same
-as a value containing only one row in the table. * Chunk the whole table, given
-the `column` name and the chunk size. In this case, choosing the **id** column
-is perfect because this each value of this column appears the same number of
-times: 1 time. * For each chunk, fetch it. * `nb_cores`=-1 will use the number
-of cores available on the machine. * `parallel_backend`='billiard' | 'joblib' |
-'multiprocessing' specify the backend framework to use. ## Chunk size
-approximation function In some cases, choosing the good `chunk_size` can be
-difficult, so a function is available to approximate the perfect size to chunk
-the table. However, this function will throw if there is too much variance
-between the number of values in the index column (if more than 25% of the
-values appear more or less than 25% of the mean of the appearance of all the
-values in the column). ```python >>> table = BigQueryTable("my_project",
-"dataset1", "users_table") >>> fetcher = BigQueryFetcher('/path/to/
-service_account.json', table) >>> perfect_nb_chunks =
-fetcher.get_chunk_size_approximation('id') >>> chunks = fetcher.chunks('id',
-perfect_nb_chunks) ``` ## Verbose mode ```python >>> perfect_nb_chunks =
-fetcher.get_chunk_size_approximation('barcode', verbose=True) # Available
-memory on device: 7.04GB # Size of table: 2.19GB # Prefered size of chunk: 3GB
-# Size per chunk: 3GB # Chunk size approximation: 1 >>> chunks = fetcher.chunks
-(column='id', chunk_size=perfect_nb_chunks, verbose=True) # Nb values in "id":
-96 # Chunk size: 1GB # Nb chunks: 1 >>> for chunk in chunks: >>> df =
+order to do operations in GCP. * Chunks the whole table, given the `column`
+name and the chunk size. In this case, choosing the **id** column is perfect
+because this each value of this column appears the same number of times: 1
+time. Concerning the chunks size, if by_chunk_size_in_GB=5, each chunk that
+will be fetched on the machine will be of size 5GB. Thus it has to fit into
+memory. You need to save 1/3 more memory because the size of a DataFrame object
+is larger than the raw fetched data. * For each chunk, fetch it. * `nb_cores`=-
+1 will use the number of cores available on the machine. *
+`parallel_backend`='billiard' | 'joblib' | 'multiprocessing' specify the
+backend framework to use. ## Fetch by number of chunks It is also possible to
+use `by_nb_chunks` instead of `by_chunk_size_in_GB`. It will divided the table
+in N, so you cannot control more flexibly the size of each chunk. ```python >>>
+table = BigQueryTable("PROJECT", "DATASET", "TABLE") >>> fetcher =
+BigQueryFetcher('/path/to/service_account.json', table) >>> chunks =
+fetcher.chunks('id', by_nb_chunks=10) >>> for chunk in chunks: df =
+fetcher.fetch(chunk, nb_cores=-1, parallel_backend='billiard') # ... ``` ##
+Verbose mode ```python >>> chunks = fetcher.chunks(column='id', by_nb_chunks=1,
+verbose=True) # Available memory on device: 7.04GB # Size of table: 2.19GB #
+Prefered size of chunk: 3GB # Size per chunk: 3GB # Nb chunks: 1 # Nb values in
+"id": 96 # Chunk size: 3GB # Nb chunks: 1 >>> for chunk in chunks: >>> df =
 fetcher.fetch(chunk=chunk, nb_cores=1, parallel_backend='joblib', verbose=True)
 # Use multiprocessing : False # Nb cores: 1 # Parallel backend: joblib # Time
-to fetch: 102.21s # Nb lines in dataframe: 3375875 # Size of dataframe: 2.83GB
+to fetch: 43.21s # Nb lines in dataframe: 3375875 # Size of dataframe: 2.83GB
 ``` ## Warning We recommend to use this tool only in the case where the table
 to fetch contains a column that can be easily chunked (divided in small parts).
 Thus the perfect column to achieve this is a column containing distinct values
 or values that appear ~ the same number of time. **If some values appear
 thousands of times and some only fews, then the chunking will not be reliable**
 because we need to make the assumption that each chunk will be approximatively
 the same size in order to estimate the needed memory necessary to fetch in an
```

### Comparing `bqfetch-1.0.1/bqfetch/bqfetch.py` & `bqfetch-1.1.0/bqfetch/bqfetch.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,30 +57,33 @@
     ----------
     service_account_path: str
         The path and file name of credentials file bq_service_account.json.
         The path should be absolute.
     '''
     def __init__(
         self,
-        service_account_path: str,
+        service_account_path: str=None,
         creds_scope: str=None,
     ) -> None:
         if isinstance(service_account_path, str):
             creds_scope = creds_scope if creds_scope is not None \
                 else CREDS_SCOPES
             credentials = service_account.Credentials.from_service_account_file(
                 service_account_path, scopes=creds_scope
             )
+            bq_client = bigquery.Client(
+                credentials=credentials,
+                project=credentials.project_id
+            )
+        elif service_account_path is None:
+            bq_client = bigquery.Client()
         else:
-            raise ValueError('`service_account_path` should be of type str or Credentials')
+            raise ValueError('`service_account_path` should be of type str or None')
 
-        bq_client = bigquery.Client(
-            credentials=credentials,
-            project=credentials.project_id
-        )
+        
         self._client = bq_client
 
     def run(
         self,
         request: str
     ) -> bigquery.table.RowIterator:
         """
@@ -185,16 +188,14 @@
         '''
         Delete the temporary table used to chunk the table.
         '''
         var = table.variables
         table = f'{var["PROJECT_ID"]}.{var["DATASET"]}.{partitioned_table_name}'
         self.delete_table(table)
 
-class InvalidChunkRangeException(Exception):
-    pass
 
 class BigQueryFetcher:
     '''
     An object used to fetch BigQuery tables easily and progressively
     in order to handle huge tables that does not fit into memory.
     The fetcher divides the table in chunks of size `chunk_size_in_GB`
     based on the `column` parameter. Then each chunk is fetched 
@@ -211,16 +212,16 @@
     >>> chunks = fetcher.chunks('user_id', 50000)
     >>> for chunk in chunks:
             df = fetcher.fetch(chunk, nb_cores=-1)
             # compute df...
     '''
     def __init__(
         self, 
-        service_account_filename: str,
         bq_table: BigQueryTable,
+        service_account_filename: str=None,
         existing_client: BigQueryClient=None,
         creds_scope: str=None,
     ):
         self._client = existing_client if existing_client is not None \
             else BigQueryClient(service_account_filename, creds_scope=creds_scope)
         self._bq_table = bq_table
         self._service_account_filename = service_account_filename
@@ -410,16 +411,16 @@
         mean = sum(nb_occurences) / len(nb_occurences)
         coeff = 0.25
         nb_dispersed_values = sum(not (mean * (1 - coeff) < count < mean * (1 + coeff)) \
             for count in nb_occurences)
         dispersion_quotient = nb_dispersed_values / len(nb_occurences)
 
         if dispersion_quotient > coeff:
-            raise InvalidChunkRangeException(f'''Difference of range between elements of column {column} \
-                is too high: more than {coeff * 100}% of elements are too far from the mean.''')
+            print(f'''Warning: Difference of range between elements of column {column} \
+                is too high: {(dispersion_quotient * 100):.2f}%, more than {coeff * 100}% of elements are too far from the mean.''')
 
         available_memory_in_GB = (psutil.virtual_memory()[1] - nb_GB_to_save) / 1024**3
         if chunk_size_in_GB >= available_memory_in_GB:
             print(f'WARNING: you are using a chunk size bigger than the available memory ({ft(chunk_size_in_GB)}>{ft(available_memory_in_GB)})')
         nb_chunks, size_of_table_in_GB = self._nb_chunks_approximation_formula(nb_cores, chunk_size_in_GB, \
             available_memory_in_GB)
         size_per_chunk_in_GB = math.ceil(size_of_table_in_GB / nb_chunks)
@@ -466,16 +467,16 @@
     Function should be global, not inside a class.
     '''
     from google.cloud.bigquery_storage import BigQueryReadClient, ReadSession, DataFormat
 
     service_account_filename, creds_scopes, partitioned_table_name, bq_table, column, chunk = pickled_parameters
 
     credentials = service_account.Credentials.from_service_account_file(
-        service_account_filename, scopes=creds_scopes
-    )
+        service_account_filename, scopes=creds_scopes) \
+            if service_account_filename != None else None
     var = bq_table.variables
     bqstorageclient = BigQueryReadClient(credentials=credentials)
     stringify_table = f"projects/{var['PROJECT_ID']}/datasets/{var['DATASET']}/tables/{partitioned_table_name}"
     parent = "projects/{}".format(var['PROJECT_ID'])
 
     requested_session = None
     if chunk is not None:
```

### Comparing `bqfetch-1.0.1/bqfetch/utils.py` & `bqfetch-1.1.0/bqfetch/utils.py`

 * *Files identical despite different names*

### Comparing `bqfetch-1.0.1/bqfetch.egg-info/PKG-INFO` & `bqfetch-1.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,20 @@
-Metadata-Version: 2.1
-Name: bqfetch
-Version: 1.0.1
-Summary: A tool to fetch tables from BigQuery as pandas DataFrames, fast.
-Home-page: https://github.com/TristanBilot/bqfetch
-Author: Tristan Bilot
-Author-email: bilot.tristan@hotmail.fr
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center"><img width="15%" src="https://raw.githubusercontent.com/TristanBilot/bqfetch/master/.github/logo.svg"/></p>
 
 <p align="center">
   <a href=""><img src="https://img.shields.io/github/last-commit/tristanbilot/bqfetch" alt="Last commit"></a>
   <a href="https://img.shields.io/github/languages/count/tristanbilot/bqfetch"><img src="https://img.shields.io/github/languages/count/tristanbilot/bqfetch" alt="Languages"></a>
   <a href=""><img src="https://img.shields.io/github/release-date/tristanbilot/bqfetch" alt="Release date"></a>
   <br>
   <a href=""><img src="https://img.shields.io/badge/Python-%3E%3D3.6-blue" alt="Python version"></a>
   <a href=""><img src="https://img.shields.io/github/license/tristanbilot/bqfetch" alt="Python version"></a>
 </p>
 
 # <p align="center">bqfetch<p>
-**A lightweight tool to fetch tables from BigQuery as pandas DataFrames very fast using BigQuery Storage API combined with multiprocessing.**
+**A lightweight tool to fetch tables from BigQuery as pandas DataFrames very fast using BigQuery Storage API combined with multiprocessing. This module also aims to fetch large tables that cannot fit into memory, by chunking the table in a smart and scalable way.**
 
 
 ## Installation
 ```
 pip install bqfetch
 pip install -r requirements.txt
 ```
@@ -53,64 +37,64 @@
 |  id |   Name  | Age |
 |:---:|:-------:|:---:|
 | 187 | Bartolomé |  30 |
 | 188 | Tristan |  22 |
 | ... |   ...   | ... |
 
 ```python
->>> table = BigQueryTable("my_project", "dataset1", "users_table")
+>>> table = BigQueryTable("PROJECT", "DATASET", "TABLE")
 >>> fetcher = BigQueryFetcher('/path/to/service_account.json', table)
->>> nb_chunks = 10
->>> chunks = fetcher.chunks('id', nb_chunks)
+>>> chunks = fetcher.chunks('id', by_chunk_size_in_GB=5)
 
 >>> for chunk in chunks:
         df = fetcher.fetch(chunk, nb_cores=-1, parallel_backend='billiard')
         # ...
 ```
   
 * First, we have to create a `BigQueryTable` object which contains the path to the BigQuery table stored in GCP.
 * A fetcher is created, given in parameter the absolute path to the service_account.json file, the file is mandatory in order to do operations in GCP.
-* Define the number of chunks to divide the table. Ex: if `nb_chunks` is set to 10, then the whole values in the index column will be fetched and divised in 10. However, setting `nb_chunks` to 10 does not mean that the table will necessarly be divided equally in 10 parts because some values in the index column can appear more than other and vice versa, causing that a value containing multiple row will be considered the same as a value containing only one row in the table.
-* Chunk the whole table, given the `column` name and the chunk size. In this case, choosing the **id** column is perfect because this each value of this column appears the same number of times: 1 time.
+* Chunks the whole table, given the `column` name and the chunk size. In this case, choosing the **id** column is perfect because this each value of this column appears the same number of times: 1 time. Concerning the chunks size, if by_chunk_size_in_GB=5, each chunk that will be fetched on the machine will be of size 5GB. Thus it has to fit into memory. You need to save 1/3 more memory because the size of a DataFrame object is larger than the raw fetched data.
 * For each chunk, fetch it.
     * `nb_cores`=-1 will use the number of cores available on the machine.
     * `parallel_backend`='billiard' | 'joblib' | 'multiprocessing' specify the backend framework to use.
 
-## Chunk size approximation function
-In some cases, choosing the good `chunk_size` can be difficult, so a function is available to approximate the perfect size to chunk the table. However, this function will throw if there is too much variance between the number of values in the index column (if more than 25% of the values appear more or less than 25% of the mean of the appearance of all the values in the column).
+## Fetch by number of chunks
+It is also possible to use `by_nb_chunks` instead of `by_chunk_size_in_GB`. It will divided the table in N, so you cannot control more flexibly the size of each chunk.
   
 ```python
->>> table = BigQueryTable("my_project", "dataset1", "users_table")
+>>> table = BigQueryTable("PROJECT", "DATASET", "TABLE")
 >>> fetcher = BigQueryFetcher('/path/to/service_account.json', table)
->>> perfect_nb_chunks = fetcher.get_chunk_size_approximation('id')
->>> chunks = fetcher.chunks('id', perfect_nb_chunks)
+>>> chunks = fetcher.chunks('id', by_nb_chunks=10)
+
+>>> for chunk in chunks:
+        df = fetcher.fetch(chunk, nb_cores=-1, parallel_backend='billiard')
+        # ...
 ```
 
 ## Verbose mode
 
 ```python
->>> perfect_nb_chunks = fetcher.get_chunk_size_approximation('barcode', verbose=True)
+>>> chunks = fetcher.chunks(column='id', by_nb_chunks=1, verbose=True)
 # Available memory on device:  7.04GB
 # Size of table:               2.19GB
 # Prefered size of chunk:      3GB
 # Size per chunk:              3GB
-# Chunk size approximation:    1
-
->>> chunks = fetcher.chunks(column='id', chunk_size=perfect_nb_chunks, verbose=True)
+# Nb chunks:                   1
+  
 # Nb values in "id":           96
-# Chunk size:                  1GB
+# Chunk size:                  3GB
 # Nb chunks:                   1
   
 >>> for chunk in chunks:
 >>>        df = fetcher.fetch(chunk=chunk, nb_cores=1, parallel_backend='joblib', verbose=True)
 # Use multiprocessing :        False
 # Nb cores:                    1
 # Parallel backend:            joblib
 
-# Time to fetch:               102.21s
+# Time to fetch:               43.21s
 # Nb lines in dataframe:       3375875
 # Size of dataframe:           2.83GB
 ```
   
 ## Warning
 We recommend to use this tool only in the case where the table to fetch contains a column that can be easily chunked (divided in small parts). Thus the perfect column to achieve this is a column containing distinct values or values that appear ~ the same number of time. **If some values appear thousands of times and some only fews, then the chunking will not be reliable** because we need to make the assumption that each chunk will be approximatively the same size in order to estimate the needed memory necessary to fetch in an optimize way the table.
   
@@ -143,9 +127,7 @@
 ## Contribution
 bqfetch is open to new contributors, especially for bug fixing or implementation of new features. Do not hesitate to open an issue/pull request :)
   
 ## License
   <a href="https://opensource.org/licenses/MIT">MIT</a>
   
   Copyright (c) 2021-present, Tristan Bilot
-
-
```

#### html2text {}

```diff
@@ -1,71 +1,58 @@
-Metadata-Version: 2.1 Name: bqfetch Version: 1.0.1 Summary: A tool to fetch
-tables from BigQuery as pandas DataFrames, fast. Home-page: https://github.com/
-TristanBilot/bqfetch Author: Tristan Bilot Author-email:
-bilot.tristan@hotmail.fr License: UNKNOWN Platform: UNKNOWN Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
-Description-Content-Type: text/markdown License-File: LICENSE
     [https://raw.githubusercontent.com/TristanBilot/bqfetch/master/.github/
                                    logo.svg]
                    [Last commit] [Languages] [Release date]
                        [Python version] [Python version]
 #
                                     bqfetch
 **A lightweight tool to fetch tables from BigQuery as pandas DataFrames very
-fast using BigQuery Storage API combined with multiprocessing.** ##
-Installation ``` pip install bqfetch pip install -r requirements.txt ``` ##
-Algorithm * Fetch all distinct values from the given index `column`. * Divide
-these indices in `chunks` based on the available memory and the number of cores
-on the machine. * `If multiprocessing`: * Each chunk will be divided in
-multiple sub-chunks based on the parameter `nb_cores` and the available memory.
-* For each sub-chunk, create a temporary table containing all the matching rows
-in the whole table. * Fetch these temporary tables using BigQuery Storage as
-dataframes. * Merge the dataframes. * Delete temporary tables. * `If
-!multiprocessing`: * Same process with only one temporary table and no parallel
-processes created. ## Use case ### Fetching a huge table of users using
-multiple cores | id | Name | Age | |:---:|:-------:|:---:| | 187 | BartolomÃ© |
-30 | | 188 | Tristan | 22 | | ... | ... | ... | ```python >>> table =
-BigQueryTable("my_project", "dataset1", "users_table") >>> fetcher =
-BigQueryFetcher('/path/to/service_account.json', table) >>> nb_chunks = 10 >>>
-chunks = fetcher.chunks('id', nb_chunks) >>> for chunk in chunks: df =
-fetcher.fetch(chunk, nb_cores=-1, parallel_backend='billiard') # ... ``` *
+fast using BigQuery Storage API combined with multiprocessing. This module also
+aims to fetch large tables that cannot fit into memory, by chunking the table
+in a smart and scalable way.** ## Installation ``` pip install bqfetch pip
+install -r requirements.txt ``` ## Algorithm * Fetch all distinct values from
+the given index `column`. * Divide these indices in `chunks` based on the
+available memory and the number of cores on the machine. * `If
+multiprocessing`: * Each chunk will be divided in multiple sub-chunks based on
+the parameter `nb_cores` and the available memory. * For each sub-chunk, create
+a temporary table containing all the matching rows in the whole table. * Fetch
+these temporary tables using BigQuery Storage as dataframes. * Merge the
+dataframes. * Delete temporary tables. * `If !multiprocessing`: * Same process
+with only one temporary table and no parallel processes created. ## Use case
+### Fetching a huge table of users using multiple cores | id | Name | Age | |:-
+--:|:-------:|:---:| | 187 | BartolomÃ© | 30 | | 188 | Tristan | 22 | | ... |
+... | ... | ```python >>> table = BigQueryTable("PROJECT", "DATASET", "TABLE")
+>>> fetcher = BigQueryFetcher('/path/to/service_account.json', table) >>>
+chunks = fetcher.chunks('id', by_chunk_size_in_GB=5) >>> for chunk in chunks:
+df = fetcher.fetch(chunk, nb_cores=-1, parallel_backend='billiard') # ... ``` *
 First, we have to create a `BigQueryTable` object which contains the path to
 the BigQuery table stored in GCP. * A fetcher is created, given in parameter
 the absolute path to the service_account.json file, the file is mandatory in
-order to do operations in GCP. * Define the number of chunks to divide the
-table. Ex: if `nb_chunks` is set to 10, then the whole values in the index
-column will be fetched and divised in 10. However, setting `nb_chunks` to 10
-does not mean that the table will necessarly be divided equally in 10 parts
-because some values in the index column can appear more than other and vice
-versa, causing that a value containing multiple row will be considered the same
-as a value containing only one row in the table. * Chunk the whole table, given
-the `column` name and the chunk size. In this case, choosing the **id** column
-is perfect because this each value of this column appears the same number of
-times: 1 time. * For each chunk, fetch it. * `nb_cores`=-1 will use the number
-of cores available on the machine. * `parallel_backend`='billiard' | 'joblib' |
-'multiprocessing' specify the backend framework to use. ## Chunk size
-approximation function In some cases, choosing the good `chunk_size` can be
-difficult, so a function is available to approximate the perfect size to chunk
-the table. However, this function will throw if there is too much variance
-between the number of values in the index column (if more than 25% of the
-values appear more or less than 25% of the mean of the appearance of all the
-values in the column). ```python >>> table = BigQueryTable("my_project",
-"dataset1", "users_table") >>> fetcher = BigQueryFetcher('/path/to/
-service_account.json', table) >>> perfect_nb_chunks =
-fetcher.get_chunk_size_approximation('id') >>> chunks = fetcher.chunks('id',
-perfect_nb_chunks) ``` ## Verbose mode ```python >>> perfect_nb_chunks =
-fetcher.get_chunk_size_approximation('barcode', verbose=True) # Available
-memory on device: 7.04GB # Size of table: 2.19GB # Prefered size of chunk: 3GB
-# Size per chunk: 3GB # Chunk size approximation: 1 >>> chunks = fetcher.chunks
-(column='id', chunk_size=perfect_nb_chunks, verbose=True) # Nb values in "id":
-96 # Chunk size: 1GB # Nb chunks: 1 >>> for chunk in chunks: >>> df =
+order to do operations in GCP. * Chunks the whole table, given the `column`
+name and the chunk size. In this case, choosing the **id** column is perfect
+because this each value of this column appears the same number of times: 1
+time. Concerning the chunks size, if by_chunk_size_in_GB=5, each chunk that
+will be fetched on the machine will be of size 5GB. Thus it has to fit into
+memory. You need to save 1/3 more memory because the size of a DataFrame object
+is larger than the raw fetched data. * For each chunk, fetch it. * `nb_cores`=-
+1 will use the number of cores available on the machine. *
+`parallel_backend`='billiard' | 'joblib' | 'multiprocessing' specify the
+backend framework to use. ## Fetch by number of chunks It is also possible to
+use `by_nb_chunks` instead of `by_chunk_size_in_GB`. It will divided the table
+in N, so you cannot control more flexibly the size of each chunk. ```python >>>
+table = BigQueryTable("PROJECT", "DATASET", "TABLE") >>> fetcher =
+BigQueryFetcher('/path/to/service_account.json', table) >>> chunks =
+fetcher.chunks('id', by_nb_chunks=10) >>> for chunk in chunks: df =
+fetcher.fetch(chunk, nb_cores=-1, parallel_backend='billiard') # ... ``` ##
+Verbose mode ```python >>> chunks = fetcher.chunks(column='id', by_nb_chunks=1,
+verbose=True) # Available memory on device: 7.04GB # Size of table: 2.19GB #
+Prefered size of chunk: 3GB # Size per chunk: 3GB # Nb chunks: 1 # Nb values in
+"id": 96 # Chunk size: 3GB # Nb chunks: 1 >>> for chunk in chunks: >>> df =
 fetcher.fetch(chunk=chunk, nb_cores=1, parallel_backend='joblib', verbose=True)
 # Use multiprocessing : False # Nb cores: 1 # Parallel backend: joblib # Time
-to fetch: 102.21s # Nb lines in dataframe: 3375875 # Size of dataframe: 2.83GB
+to fetch: 43.21s # Nb lines in dataframe: 3375875 # Size of dataframe: 2.83GB
 ``` ## Warning We recommend to use this tool only in the case where the table
 to fetch contains a column that can be easily chunked (divided in small parts).
 Thus the perfect column to achieve this is a column containing distinct values
 or values that appear ~ the same number of time. **If some values appear
 thousands of times and some only fews, then the chunking will not be reliable**
 because we need to make the assumption that each chunk will be approximatively
 the same size in order to estimate the needed memory necessary to fetch in an
```

### Comparing `bqfetch-1.0.1/setup.cfg` & `bqfetch-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bqfetch
-version = 1.0.1
+version = 1.1.0
 author = Tristan Bilot
 author_email = bilot.tristan@hotmail.fr
 description = A tool to fetch tables from BigQuery as pandas DataFrames, fast.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/TristanBilot/bqfetch
 classifiers =
```

