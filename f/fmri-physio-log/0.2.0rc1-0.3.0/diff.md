# Comparing `tmp/fmri-physio-log-0.2.0rc1.tar.gz` & `tmp/fmri_physio_log-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmri-physio-log-0.2.0rc1.tar", max compression
+gzip compressed data, was "fmri_physio_log-0.3.0.tar", max compression
```

## Comparing `fmri-physio-log-0.2.0rc1.tar` & `fmri_physio_log-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1068 2022-03-07 16:52:02.827558 fmri-physio-log-0.2.0rc1/LICENSE
--rw-r--r--   0        0        0     1896 2022-03-07 16:52:02.827558 fmri-physio-log-0.2.0rc1/README.md
--rw-r--r--   0        0        0      978 2022-03-07 16:52:02.827558 fmri-physio-log-0.2.0rc1/pyproject.toml
--rw-r--r--   0        0        0     7467 2022-03-07 16:52:02.831558 fmri-physio-log-0.2.0rc1/src/fmri_physio_log.py
--rw-r--r--   0        0        0     2633 2022-03-07 16:52:16.436064 fmri-physio-log-0.2.0rc1/setup.py
--rw-r--r--   0        0        0     2878 2022-03-07 16:52:16.436355 fmri-physio-log-0.2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-16 04:18:07.106927 fmri_physio_log-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4988 2023-06-16 04:18:07.106927 fmri_physio_log-0.3.0/README.md
+-rw-r--r--   0        0        0      973 2023-06-16 04:18:07.106927 fmri_physio_log-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8739 2023-06-16 04:18:07.114927 fmri_physio_log-0.3.0/src/fmri_physio_log.py
+-rw-r--r--   0        0        0     5914 1970-01-01 00:00:00.000000 fmri_physio_log-0.3.0/PKG-INFO
```

### Comparing `fmri-physio-log-0.2.0rc1/LICENSE` & `fmri_physio_log-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fmri-physio-log-0.2.0rc1/pyproject.toml` & `fmri_physio_log-0.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "fmri-physio-log"
-version = "0.2.0rc1"
-description = "Load fMRI PMU files into python"
+version = "0.3.0"
+description = "Parse Siemens PMU files"
 authors = [
     "Andrew Ross <andrew.ross.mail@gmail.com>"
 ]
 license = "MIT"
 
 readme = "README.md"
 
@@ -19,23 +19,22 @@
     "Programming Language :: Python :: 3.0",
     "Topic :: Scientific/Engineering :: Medical Science Apps.",
     "License :: OSI Approved :: MIT License",
     "Development Status :: 4 - Beta",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
 pyparsing = "^3.0.7"
 
-[tool.poetry.dev-dependencies]
-black = "^22.1.0"
-flake8 = "^4.0.1"
-pylint = "^2.12.2"
-reorder-python-imports = "^2.7.1"
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+flake8 = "^6.0.0"
+pylint = "^2.17.4"
+reorder-python-imports = "^3.9.0"
 bump2version = "^1.0.1"
-pre-commit = "^2.17.0"
-pytest = "^7.0.1"
-
+pre-commit = "^3.3.3"
+pytest = "^7.3.2"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `fmri-physio-log-0.2.0rc1/src/fmri_physio_log.py` & `fmri_physio_log-0.3.0/src/fmri_physio_log.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from pyparsing import OneOrMore
 from pyparsing import ParseResults
 from pyparsing import printables
 from pyparsing import Suppress
 from pyparsing import Word
 
 
-__version__ = "0.2.0rc1"
+__version__ = "0.3.0"
 
 
 class PhysioLog:
     def __init__(self, content: str):
         self.content = content
         self._grammar = create_grammar()
 
@@ -32,14 +32,15 @@
         self.info: list[str]
         self.ts: list[int]
 
         self.ecg: MeasurementSummary
         self.puls: MeasurementSummary
         self.resp: MeasurementSummary
         self.ext: MeasurementSummary
+        self.ext2: MeasurementSummary | None = None
 
         self.nr: NrSummary
 
         self.mdh: LogTime
         self.mpcu: LogTime
 
         # this method sets all of the above values
@@ -119,18 +120,54 @@
 
         # set the log time attributes
         for attr, values in _logs.items():
             setattr(self, attr.lower(), LogTime(*values))
 
 
 def create_grammar():
+    """Creates the pyparsing grammar used parse pmu files.
+
+    Roughly speaking, this is the PMU grammar that this function creates:
+
+    <content> ::= <body> <footer>
+
+    <body> ::= <params> <data>
+    <params> ::= <detailed_params> | <simple_params>
+    <simple_params> ::= INT INT INT INT
+    <detailed_params> ::= INT INT INT INT [INT] <info>
+    <info> ::= 5002 PRINTABLE 6002
+    <data> ::= (<info> | 5000 | INT)+
+
+    <footer> ::= 5003 <footer_line> [<footer_line>]+ 6003
+    <footer_line> ::= <rate_line> | <stat_line> | <nr_line> | <log_line>
+    <rate_line> ::= <modality> <rate>
+    <rate> ::= <rate_prefix> INT INT
+    <rate_prefix> ::= 'Freq Per:'
+    <stat_line> ::= <modality> <stat>
+    <stat> ::= <stat_prefix> INT INT INT INT
+    <stat_prefix> ::= 'Min Max Avg StdDiff:'
+    <nr_line> ::= <nr_prefix> INT INT INT INT
+    <nr_prefix> ::= 'NrTrig NrMP NrArr AcqWin:'
+    <log_line> ::= <log_prefix> INT
+    <log_prefix> ::= 'LogStartMDHTime:'
+                   | 'LogStopMDHTime:'
+                   | 'LogStartMPCUTime:'
+                   | 'LogStopMPCUTime:'
+    <modality> ::= 'ECG' | 'PULS' | 'RESP' | 'EXT' | 'EXT2'
+    """
     _int = Word(nums)
 
     # footer
-    modality = Literal("ECG") | Literal("PULS") | Literal("RESP") | Literal("EXT")
+    modality = (
+        Literal("ECG")
+        | Literal("PULS")
+        | Literal("RESP")
+        | Literal("EXT2")
+        | Literal("EXT")
+    )
     log_type = Literal("MDH") | Literal("MPCU")
     log_event = Literal("Start") | Literal("Stop")
     rate = (
         Suppress("Freq") + Suppress("Per") + Suppress(":") + _int("freq") + _int("per")
     )
     stat = (
         Suppress("Min")
@@ -212,15 +249,16 @@
             isinstance(o, self.__class__)
             and self.start == o.start
             and self.stop == o.stop
         )
 
     @staticmethod
     def logptime(timestamp: int) -> datetime.time:
-        """Converts an integer denoting milliseconds past midnight to a datetime.time object.
+        """Converts an integer denoting milliseconds past midnight to a
+        datetime.time object.
 
         Args:
             timestamp (int): The integer to convert.
 
         Returns:
             datetime.time: The time object.
```

