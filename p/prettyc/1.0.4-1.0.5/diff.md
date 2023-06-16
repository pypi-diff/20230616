# Comparing `tmp/prettyc-1.0.4.tar.gz` & `tmp/prettyc-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettyc-1.0.4.tar", last modified: Wed Jun  7 19:11:59 2023, max compression
+gzip compressed data, was "prettyc-1.0.5.tar", last modified: Fri Jun 16 19:39:20 2023, max compression
```

## Comparing `prettyc-1.0.4.tar` & `prettyc-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-07 19:11:59.360051 prettyc-1.0.4/
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     1502 2023-06-07 13:06:43.000000 prettyc-1.0.4/LICENSE
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     1732 2023-06-07 19:11:59.360051 prettyc-1.0.4/PKG-INFO
--rw-rw-r--   0 vahid     (1000) vahid     (1000)      797 2023-06-07 14:02:40.000000 prettyc-1.0.4/README.md
-drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-07 19:11:59.360051 prettyc-1.0.4/prettyc.egg-info/
--rw-rw-r--   0 vahid     (1000) vahid     (1000)     1732 2023-06-07 19:11:59.000000 prettyc-1.0.4/prettyc.egg-info/PKG-INFO
--rw-rw-r--   0 vahid     (1000) vahid     (1000)      195 2023-06-07 19:11:59.000000 prettyc-1.0.4/prettyc.egg-info/SOURCES.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)        1 2023-06-07 19:11:59.000000 prettyc-1.0.4/prettyc.egg-info/dependency_links.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)       42 2023-06-07 19:11:59.000000 prettyc-1.0.4/prettyc.egg-info/entry_points.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)        8 2023-06-07 19:11:59.000000 prettyc-1.0.4/prettyc.egg-info/top_level.txt
--rw-rw-r--   0 vahid     (1000) vahid     (1000)   259324 2023-06-07 19:11:19.000000 prettyc-1.0.4/prettyc.py
--rw-rw-r--   0 vahid     (1000) vahid     (1000)       38 2023-06-07 19:11:59.360051 prettyc-1.0.4/setup.cfg
--rwxrwxr-x   0 vahid     (1000) vahid     (1000)     1470 2023-06-07 13:01:31.000000 prettyc-1.0.4/setup.py
+drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-16 19:39:20.145261 prettyc-1.0.5/
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)     1502 2023-06-07 13:06:43.000000 prettyc-1.0.5/LICENSE
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)     1732 2023-06-16 19:39:20.145261 prettyc-1.0.5/PKG-INFO
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)      797 2023-06-07 14:02:40.000000 prettyc-1.0.5/README.md
+drwxrwxr-x   0 vahid     (1000) vahid     (1000)        0 2023-06-16 19:39:20.145261 prettyc-1.0.5/prettyc.egg-info/
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)     1732 2023-06-16 19:39:20.000000 prettyc-1.0.5/prettyc.egg-info/PKG-INFO
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)      195 2023-06-16 19:39:20.000000 prettyc-1.0.5/prettyc.egg-info/SOURCES.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)        1 2023-06-16 19:39:20.000000 prettyc-1.0.5/prettyc.egg-info/dependency_links.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)       42 2023-06-16 19:39:20.000000 prettyc-1.0.5/prettyc.egg-info/entry_points.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)        8 2023-06-16 19:39:20.000000 prettyc-1.0.5/prettyc.egg-info/top_level.txt
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)   257930 2023-06-16 19:38:04.000000 prettyc-1.0.5/prettyc.py
+-rw-rw-r--   0 vahid     (1000) vahid     (1000)       38 2023-06-16 19:39:20.145261 prettyc-1.0.5/setup.cfg
+-rwxrwxr-x   0 vahid     (1000) vahid     (1000)     1470 2023-06-07 13:01:31.000000 prettyc-1.0.5/setup.py
```

### Comparing `prettyc-1.0.4/LICENSE` & `prettyc-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prettyc-1.0.4/PKG-INFO` & `prettyc-1.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettyc
-Version: 1.0.4
+Version: 1.0.5
 Summary: Fork of Google's cpplint, modified to work only with C.
 Home-page: http://github.com/pylover/prettyc
 Author: Vahid Mardani
 Author-email: vahid.mardani@gmail.com
 License: BSD-3-Clause
 Keywords: lint,python,c
 Platform: UNKNOWN
```

### Comparing `prettyc-1.0.4/README.md` & `prettyc-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `prettyc-1.0.4/prettyc.egg-info/PKG-INFO` & `prettyc-1.0.5/prettyc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettyc
-Version: 1.0.4
+Version: 1.0.5
 Summary: Fork of Google's cpplint, modified to work only with C.
 Home-page: http://github.com/pylover/prettyc
 Author: Vahid Mardani
 Author-email: vahid.mardani@gmail.com
 License: BSD-3-Clause
 Keywords: lint,python,c
 Platform: UNKNOWN
```

### Comparing `prettyc-1.0.4/prettyc.py` & `prettyc-1.0.5/prettyc.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 import sysconfig
 import unicodedata
 import xml.etree.ElementTree
 
 # if empty, use defaults
 _valid_extensions = set([])
 
-__version__ = '1.0.4'
+__version__ = '1.0.5'
 __verbose__ = False
 
 try:
   #  -- pylint: disable=used-before-assignment
   xrange          # Python 2
 except NameError:
   #  -- pylint: disable=redefined-builtin
@@ -380,19 +380,14 @@
 
 # The default state of the category filter. This is overridden by the --filter=
 # flag. By default all errors are on, so only add here categories that should be
 # off by default (i.e., categories that must be enabled by the --filter= flags).
 # All entries here should start with a '-' or '+', as in the --filter= flag.
 _DEFAULT_FILTERS = ['-build/include_alpha']
 
-# The default list of categories suppressed for C (not C++) files.
-_DEFAULT_C_SUPPRESSED_CATEGORIES = [
-    'readability/casting',
-    ]
-
 # The default list of categories suppressed for Linux Kernel files.
 _DEFAULT_KERNEL_SUPPRESSED_CATEGORIES = [
     'whitespace/tab',
     ]
 
 # We used to check for high-bit characters, but after much discussion we
 # decided those were OK, as long as they were in UTF-8 and didn't represent
@@ -841,18 +836,14 @@
 _BLOCK_ASM = 3    # The whole block is an inline assembly block
 
 # Match start of assembly blocks
 _MATCH_ASM = re.compile(r'^\s*(?:asm|_asm|__asm|__asm__)'
                         r'(?:\s+(volatile|__volatile__))?'
                         r'\s*[{(]')
 
-# Match strings that indicate we're working on a C (not C++) file.
-_SEARCH_C_FILE = re.compile(r'\b(?:LINT_C_FILE|'
-                            r'vim?:\s*.*(\s*|:)filetype=c(\s*|:|$))')
-
 # Match string that indicates we're working on a Linux Kernel file.
 _SEARCH_KERNEL_FILE = re.compile(r'\b(?:LINT_KERNEL_FILE)')
 
 # Commands for sed to fix the problem
 _SED_FIXUPS = {
   'Remove spaces around =': r's/ = /=/',
   'Remove spaces around !=': r's/ != /!=/',
@@ -1020,17 +1011,14 @@
   Parses any lint directives in the file that have global effect.
 
   Args:
     lines: An array of strings, each representing a line of the file, with the
            last element being empty if the file is terminated with a newline.
   """
   for line in lines:
-    if _SEARCH_C_FILE.search(line):
-      for category in _DEFAULT_C_SUPPRESSED_CATEGORIES:
-        _global_error_suppressions[category] = True
     if _SEARCH_KERNEL_FILE.search(line):
       for category in _DEFAULT_KERNEL_SUPPRESSED_CATEGORIES:
         _global_error_suppressions[category] = True
 
 
 def ResetNolintSuppressions():
   """Resets the set of NOLINT suppressions to empty."""
@@ -5672,32 +5660,14 @@
     matched_new_or_template = match.group(1)
 
     # Avoid arrays by looking for brackets that come after the closing
     # parenthesis.
     if Match(r'\([^()]+\)\s*\[', match.group(3)):
       return
 
-    # Other things to ignore:
-    # - Function pointers
-    # - Casts to pointer types
-    # - Placement new
-    # - Alias declarations
-    matched_funcptr = match.group(3)
-    if (matched_new_or_template is None and
-        not (matched_funcptr and
-             (Match(r'\((?:[^() ]+::\s*\*\s*)?[^() ]+\)\s*\(',
-                    matched_funcptr) or
-              matched_funcptr.startswith('(*)'))) and
-        not Match(r'\s*using\s+\S+\s*=\s*' + matched_type, line) and
-        not Search(r'new\(\S+\)\s*' + matched_type, line)):
-      error(filename, linenum, 'readability/casting', 4,
-            'Using deprecated casting style.  '
-            'Use static_cast<%s>(...) instead' %
-            matched_type)
-
   if not expecting_function:
     CheckCStyleCast(filename, clean_lines, linenum, 'static_cast',
                     r'\((int|float|double|bool|char|u?int(16|32|64)|size_t)\)', error)
 
   # This doesn't catch all cases. Consider (const char * const)"hello".
   #
   # (char *) "foo" should always be a const_cast (reinterpret_cast won't
@@ -5795,19 +5765,14 @@
   # A single unnamed argument for a function tends to look like old style cast.
   # If we see those, don't issue warnings for deprecated casts.
   remainder = line[match.end(0):]
   if Match(r'^\s*(?:;|const\b|throw\b|final\b|override\b|[=>{),]|->)',
            remainder):
     return False
 
-  # At this point, all that should be left is actual casts.
-  error(filename, linenum, 'readability/casting', 4,
-        'Using C-style cast.  Use %s<%s>(...) instead' %
-        (cast_type, match.group(1)))
-
   return True
 
 
 def ExpectingFunctionArgs(clean_lines, linenum):
   """Checks whether where function type arguments are expected.
 
   Args:
```

### Comparing `prettyc-1.0.4/setup.py` & `prettyc-1.0.5/setup.py`

 * *Files identical despite different names*

