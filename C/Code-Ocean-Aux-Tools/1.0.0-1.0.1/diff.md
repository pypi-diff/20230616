# Comparing `tmp/code_ocean_aux_tools-1.0.0.tar.gz` & `tmp/code_ocean_aux_tools-1.0.1.tar.gz`

## Comparing `code_ocean_aux_tools-1.0.0.tar` & `code_ocean_aux_tools-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,59 @@
--rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/setup.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/src/__init__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/src/co_tools/__init__.py
--rwxr-xr-x   0        0        0     2014 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/src/co_tools/co_fasta.py
--rwxr-xr-x   0        0        0     7434 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/src/co_tools/co_fastq.py
--rwxr-xr-x   0        0        0     4334 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/src/co_tools/co_utils.py
--rwxr-xr-x   0        0        0      190 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/src/co_tools/get_cpu_count.py
--rwxr-xr-x   0        0        0      716 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/src/co_tools/get_dir_contents.py
--rwxr-xr-x   0        0        0      693 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/src/co_tools/get_fasta_file.py
--rwxr-xr-x   0        0        0      515 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/src/co_tools/get_fastq_pair.py
--rwxr-xr-x   0        0        0      573 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/src/co_tools/get_fwd_fastqs.py
--rwxr-xr-x   0        0        0      503 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/src/co_tools/get_groups.py
--rwxr-xr-x   0        0        0     3821 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/src/co_tools/get_logger.py
--rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/src/co_tools/get_pipeline_confirm.py
--rwxr-xr-x   0        0        0      534 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/src/co_tools/get_read_direction.py
--rwxr-xr-x   0        0        0      641 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/src/co_tools/get_read_pattern.py
--rwxr-xr-x   0        0        0      609 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/src/co_tools/get_read_prefix.py
--rwxr-xr-x   0        0        0      633 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/src/co_tools/get_rev_file.py
--rwxr-xr-x   0        0        0      556 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/src/co_tools/set_log_msg.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/tests/__init__.py
--rwxr-xr-x   0        0        0      200 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/tests/conftest.py
--rwxr-xr-x   0        0        0      649 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/tests/test_get_cpu_count.py
--rwxr-xr-x   0        0        0      664 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/tests/test_get_dir_contents.py
--rwxr-xr-x   0        0        0     1781 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/tests/test_get_fasta_file.py
--rwxr-xr-x   0        0        0      502 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/tests/test_get_fwd_fastqs.py
--rwxr-xr-x   0        0        0      478 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/tests/test_get_groups.py
--rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/tests/test_get_pipeline_confirm.py
--rwxr-xr-x   0        0        0     1533 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/tests/test_get_read_direction.py
--rwxr-xr-x   0        0        0     3356 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/tests/test_get_read_pattern.py
--rwxr-xr-x   0        0        0     1330 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/tests/test_get_read_prefix.py
--rwxr-xr-x   0        0        0     2175 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/tests/test_get_rev_file.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/tests/fixtures/__init__.py
--rwxr-xr-x   0        0        0      857 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/tests/fixtures/dirs_of_files.py
--rwxr-xr-x   0        0        0      320 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/tests/fixtures/fastq_file.py
--rwxr-xr-x   0        0        0      659 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/tests/fixtures/sample_sheets.py
--rwxr-xr-x   0        0        0       77 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/.gitignore
--rwxr-xr-x   0        0        0     1067 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/LICENSE
--rwxr-xr-x   0        0        0     3653 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/README.md
--rwxr-xr-x   0        0        0     1387 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0       38 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/setup.py
+-rwxr-xr-x   0        0        0      143 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/index.html
+-rwxr-xr-x   0        0        0   145343 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/search.js
+-rwxr-xr-x   0        0        0    35405 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools.html
+-rwxr-xr-x   0        0        0    64876 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/co_fasta.html
+-rwxr-xr-x   0        0        0   137471 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/co_fastq.html
+-rwxr-xr-x   0        0        0    95633 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/co_utils.html
+-rwxr-xr-x   0        0        0    38262 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_cpu_count.html
+-rwxr-xr-x   0        0        0    46146 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_dir_contents.html
+-rwxr-xr-x   0        0        0    45020 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_fasta_file.html
+-rwxr-xr-x   0        0        0    43404 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_fastq_pair.html
+-rwxr-xr-x   0        0        0    44350 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_fwd_fastqs.html
+-rwxr-xr-x   0        0        0    43368 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_groups.html
+-rwxr-xr-x   0        0        0    77308 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_logger.html
+-rwxr-xr-x   0        0        0    38284 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_pipeline_confirm.html
+-rwxr-xr-x   0        0        0    43353 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_read_direction.html
+-rwxr-xr-x   0        0        0    45190 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_read_pattern.html
+-rwxr-xr-x   0        0        0    45128 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_read_prefix.html
+-rwxr-xr-x   0        0        0    45408 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/get_rev_file.html
+-rwxr-xr-x   0        0        0    43629 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/docs/src/co_tools/set_log_msg.html
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/__init__.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/__init__.py
+-rwxr-xr-x   0        0        0     2014 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/co_fasta.py
+-rwxr-xr-x   0        0        0     7434 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/co_fastq.py
+-rwxr-xr-x   0        0        0     4334 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/co_utils.py
+-rwxr-xr-x   0        0        0      190 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/get_cpu_count.py
+-rwxr-xr-x   0        0        0      716 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/get_dir_contents.py
+-rwxr-xr-x   0        0        0      693 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/get_fasta_file.py
+-rwxr-xr-x   0        0        0      515 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/get_fastq_pair.py
+-rwxr-xr-x   0        0        0      573 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/get_fwd_fastqs.py
+-rwxr-xr-x   0        0        0      503 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/get_groups.py
+-rwxr-xr-x   0        0        0     3821 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/get_logger.py
+-rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/get_pipeline_confirm.py
+-rwxr-xr-x   0        0        0      534 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/get_read_direction.py
+-rwxr-xr-x   0        0        0      641 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/get_read_pattern.py
+-rwxr-xr-x   0        0        0      609 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/get_read_prefix.py
+-rwxr-xr-x   0        0        0      633 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/get_rev_file.py
+-rwxr-xr-x   0        0        0      556 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/src/co_tools/set_log_msg.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/__init__.py
+-rwxr-xr-x   0        0        0      200 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/conftest.py
+-rwxr-xr-x   0        0        0      649 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/test_get_cpu_count.py
+-rwxr-xr-x   0        0        0      664 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/test_get_dir_contents.py
+-rwxr-xr-x   0        0        0     1781 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/test_get_fasta_file.py
+-rwxr-xr-x   0        0        0      502 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/test_get_fwd_fastqs.py
+-rwxr-xr-x   0        0        0      478 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/test_get_groups.py
+-rwxr-xr-x   0        0        0      286 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/test_get_pipeline_confirm.py
+-rwxr-xr-x   0        0        0     1533 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/test_get_read_direction.py
+-rwxr-xr-x   0        0        0     3356 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/test_get_read_pattern.py
+-rwxr-xr-x   0        0        0     1330 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/test_get_read_prefix.py
+-rwxr-xr-x   0        0        0     2175 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/test_get_rev_file.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/fixtures/__init__.py
+-rwxr-xr-x   0        0        0      857 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/fixtures/dirs_of_files.py
+-rwxr-xr-x   0        0        0      320 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/fixtures/fastq_file.py
+-rwxr-xr-x   0        0        0      659 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/tests/fixtures/sample_sheets.py
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/.gitignore
+-rwxr-xr-x   0        0        0     1067 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/LICENSE
+-rwxr-xr-x   0        0        0     3985 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/README.md
+-rwxr-xr-x   0        0        0     1388 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 code_ocean_aux_tools-1.0.1/PKG-INFO
```

### Comparing `code_ocean_aux_tools-1.0.0/src/co_tools/co_fasta.py` & `code_ocean_aux_tools-1.0.1/src/co_tools/co_fasta.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.0/src/co_tools/co_fastq.py` & `code_ocean_aux_tools-1.0.1/src/co_tools/co_fastq.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.0/src/co_tools/co_utils.py` & `code_ocean_aux_tools-1.0.1/src/co_tools/co_utils.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.0/src/co_tools/get_dir_contents.py` & `code_ocean_aux_tools-1.0.1/src/co_tools/get_dir_contents.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.0/src/co_tools/get_fasta_file.py` & `code_ocean_aux_tools-1.0.1/src/co_tools/get_fasta_file.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.0/src/co_tools/get_fastq_pair.py` & `code_ocean_aux_tools-1.0.1/src/co_tools/get_fastq_pair.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.0/src/co_tools/get_fwd_fastqs.py` & `code_ocean_aux_tools-1.0.1/src/co_tools/get_fwd_fastqs.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.0/src/co_tools/get_logger.py` & `code_ocean_aux_tools-1.0.1/src/co_tools/get_logger.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.0/src/co_tools/get_read_direction.py` & `code_ocean_aux_tools-1.0.1/src/co_tools/get_read_direction.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.0/src/co_tools/get_read_pattern.py` & `code_ocean_aux_tools-1.0.1/src/co_tools/get_read_pattern.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.0/src/co_tools/get_read_prefix.py` & `code_ocean_aux_tools-1.0.1/src/co_tools/get_read_prefix.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.0/src/co_tools/get_rev_file.py` & `code_ocean_aux_tools-1.0.1/src/co_tools/get_rev_file.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.0/src/co_tools/set_log_msg.py` & `code_ocean_aux_tools-1.0.1/src/co_tools/set_log_msg.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.0/tests/test_get_cpu_count.py` & `code_ocean_aux_tools-1.0.1/tests/test_get_cpu_count.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.0/tests/test_get_dir_contents.py` & `code_ocean_aux_tools-1.0.1/tests/test_get_dir_contents.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.0/tests/test_get_fasta_file.py` & `code_ocean_aux_tools-1.0.1/tests/test_get_fasta_file.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.0/tests/test_get_read_direction.py` & `code_ocean_aux_tools-1.0.1/tests/test_get_read_direction.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.0/tests/test_get_read_pattern.py` & `code_ocean_aux_tools-1.0.1/tests/test_get_read_pattern.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.0/tests/test_get_read_prefix.py` & `code_ocean_aux_tools-1.0.1/tests/test_get_read_prefix.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.0/tests/test_get_rev_file.py` & `code_ocean_aux_tools-1.0.1/tests/test_get_rev_file.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.0/tests/fixtures/dirs_of_files.py` & `code_ocean_aux_tools-1.0.1/tests/fixtures/dirs_of_files.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.0/tests/fixtures/sample_sheets.py` & `code_ocean_aux_tools-1.0.1/tests/fixtures/sample_sheets.py`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.0/LICENSE` & `code_ocean_aux_tools-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `code_ocean_aux_tools-1.0.0/README.md` & `code_ocean_aux_tools-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 ---
 
 ### Installing *Code Ocean* Aux Tools in your capsule
 
 Add one line of code to your postintall script. At a later time this will be a package you can add to pip in the environment UI.
 
-`pip install -i https://test.pypi.org/simple/ Code-Ocean-Aux-Tools`
+`pip install Code-Ocean-Aux-Tools`
 
 ---
 ### List of  Available Commands
 
 The following commands will work at the terminal or in a bash script
 
     - get_cpu_count
@@ -70,15 +70,15 @@
     - get_read_direction()
     - get_read_pattern()
     - get_prefix()
     - get_rev_file()
 
 ---
 
-### Logging
+## Logging
 
 There is a pre-configured logger that will work seamlessly in bash and/or python and output to the same log file. The format for each log entry is:
 
 `[{Date} {Time} - {log name} - {filename}:{lineno} - {Log Level}] {log message}`
 
 The available [log levels](https://docs.python.org/3/howto/logging.html) are `debug`, `info`, `warning`, `error`, and `critical`
 
@@ -97,17 +97,27 @@
 
 To use the logger in a bash script, just use the `set_log_msg` command. It takes 1 required argument and an additional optional argument.
 
 The required argument is the log message and the optional argument is for the desired log level.
 
 e.g. `set_log_msg "logging is fun" "INFO"`
 
-### Setting the log level for LOGGER
+---
+## Configuring the LOGGER
+
+
+### Activating the LOGGER 
+
+The Code Ocean LOGGER is turned off by default. To turn it on, create an environment variable called `CO_LOG` and assign a value of `true`.
+
+eg. `export CO_LOG=true`
+
+### Assigning the log level
 
-Create an environment variable called `CO_LOG_LEVEL` and assign it one of the 5 available log levels. The default value is `WARNING`. Ideally you will assign the value to `CO_LOG_LEVEL` in your runscript just before the entry script is executed.
+Create an environment variable called `CO_LOG_LEVEL` and assign it one of the 5 available log levels. The default value is `WARNING`. One method can be to assign the value to `CO_LOG_LEVEL` in your runscript just before the entry script is executed.
 
 e.g.
 ```
 export CO_LOG_LEVEL="INFO"
 python -u main.py "$@"
 ```
 or
@@ -116,9 +126,9 @@
 export CO_LOG_LEVEL="INFO"
 bash main.sh "$@"
 ```
 
 
 ---
 
-[Code Ocean](https://codeocean.com/) is a cloud-based computational platform that aims to make it easy for researchers to share, discover, and run code. Visit our [Open Science Library](https://codeocean.com/explore) for free code and to demo our free product. Contact our [sales](https://codeocean.com/contact-us/sales/) for a demo of our [enterprise VPC product](https://codeocean.com/product/).<br /><br />
+[Code Ocean](https://codeocean.com/) is a cloud-based dry lab for scientific computing with a focus on guaranteeing reproducibility, collaboration and organizing scientific projects. Code Ocean automates best practices allowing users of the platform to focus on science yet follow best practices. Visit our [Open Science Library](https://codeocean.com/explore) for free code and to demo our free product. Contact our [sales](https://codeocean.com/contact-us/sales/) for a demo of our [enterprise VPC product](https://codeocean.com/product/).<br /><br />
 [![Code Ocean Logo](https://github.com/codeocean/branding/raw/main/logo/CO_logo_68x36.png)](https://www.codeocean.com)
```

### Comparing `code_ocean_aux_tools-1.0.0/pyproject.toml` & `code_ocean_aux_tools-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/co_tools"]
 
 [project]
 name = "Code_Ocean_Aux_Tools"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Frank Zappulla", email="frank@codeocean.com" },
 ]
 maintainers = [
     { name="Frank Zappulla", email="frank@codeocean.com" }
 ]
-description = "A suite of convenience tools for working with sequencing files and Code Ocean capsules"
+description = "A suite of convenience tools for working with sequencing files and Code Ocean capsules."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `code_ocean_aux_tools-1.0.0/PKG-INFO` & `code_ocean_aux_tools-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Code_Ocean_Aux_Tools
-Version: 1.0.0
-Summary: A suite of convenience tools for working with sequencing files and Code Ocean capsules
+Version: 1.0.1
+Summary: A suite of convenience tools for working with sequencing files and Code Ocean capsules.
 Project-URL: Homepage, https://github.com/codeocean/co_aux_tools
 Project-URL: Bug Tracker, https://github.com/codeocean/co_aux_tools/issues
 Author-email: Frank Zappulla <frank@codeocean.com>
 Maintainer-email: Frank Zappulla <frank@codeocean.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,15 +36,15 @@
 
 ---
 
 ### Installing *Code Ocean* Aux Tools in your capsule
 
 Add one line of code to your postintall script. At a later time this will be a package you can add to pip in the environment UI.
 
-`pip install -i https://test.pypi.org/simple/ Code-Ocean-Aux-Tools`
+`pip install Code-Ocean-Aux-Tools`
 
 ---
 ### List of  Available Commands
 
 The following commands will work at the terminal or in a bash script
 
     - get_cpu_count
@@ -85,15 +85,15 @@
     - get_read_direction()
     - get_read_pattern()
     - get_prefix()
     - get_rev_file()
 
 ---
 
-### Logging
+## Logging
 
 There is a pre-configured logger that will work seamlessly in bash and/or python and output to the same log file. The format for each log entry is:
 
 `[{Date} {Time} - {log name} - {filename}:{lineno} - {Log Level}] {log message}`
 
 The available [log levels](https://docs.python.org/3/howto/logging.html) are `debug`, `info`, `warning`, `error`, and `critical`
 
@@ -112,17 +112,27 @@
 
 To use the logger in a bash script, just use the `set_log_msg` command. It takes 1 required argument and an additional optional argument.
 
 The required argument is the log message and the optional argument is for the desired log level.
 
 e.g. `set_log_msg "logging is fun" "INFO"`
 
-### Setting the log level for LOGGER
+---
+## Configuring the LOGGER
+
+
+### Activating the LOGGER 
+
+The Code Ocean LOGGER is turned off by default. To turn it on, create an environment variable called `CO_LOG` and assign a value of `true`.
+
+eg. `export CO_LOG=true`
+
+### Assigning the log level
 
-Create an environment variable called `CO_LOG_LEVEL` and assign it one of the 5 available log levels. The default value is `WARNING`. Ideally you will assign the value to `CO_LOG_LEVEL` in your runscript just before the entry script is executed.
+Create an environment variable called `CO_LOG_LEVEL` and assign it one of the 5 available log levels. The default value is `WARNING`. One method can be to assign the value to `CO_LOG_LEVEL` in your runscript just before the entry script is executed.
 
 e.g.
 ```
 export CO_LOG_LEVEL="INFO"
 python -u main.py "$@"
 ```
 or
@@ -131,9 +141,9 @@
 export CO_LOG_LEVEL="INFO"
 bash main.sh "$@"
 ```
 
 
 ---
 
-[Code Ocean](https://codeocean.com/) is a cloud-based computational platform that aims to make it easy for researchers to share, discover, and run code. Visit our [Open Science Library](https://codeocean.com/explore) for free code and to demo our free product. Contact our [sales](https://codeocean.com/contact-us/sales/) for a demo of our [enterprise VPC product](https://codeocean.com/product/).<br /><br />
+[Code Ocean](https://codeocean.com/) is a cloud-based dry lab for scientific computing with a focus on guaranteeing reproducibility, collaboration and organizing scientific projects. Code Ocean automates best practices allowing users of the platform to focus on science yet follow best practices. Visit our [Open Science Library](https://codeocean.com/explore) for free code and to demo our free product. Contact our [sales](https://codeocean.com/contact-us/sales/) for a demo of our [enterprise VPC product](https://codeocean.com/product/).<br /><br />
 [![Code Ocean Logo](https://github.com/codeocean/branding/raw/main/logo/CO_logo_68x36.png)](https://www.codeocean.com)
```

