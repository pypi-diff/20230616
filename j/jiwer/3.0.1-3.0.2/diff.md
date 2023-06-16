# Comparing `tmp/jiwer-3.0.1.tar.gz` & `tmp/jiwer-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiwer-3.0.1.tar", max compression
+gzip compressed data, was "jiwer-3.0.2.tar", max compression
```

## Comparing `jiwer-3.0.1.tar` & `jiwer-3.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11339 2023-03-28 18:38:57.974167 jiwer-3.0.1/LICENSE
--rw-r--r--   0        0        0     1729 2023-03-28 18:38:57.974167 jiwer-3.0.1/README.md
--rw-r--r--   0        0        0      145 2023-03-28 18:38:57.978167 jiwer-3.0.1/jiwer/__init__.py
--rw-r--r--   0        0        0     5733 2023-03-28 18:38:57.978167 jiwer-3.0.1/jiwer/alignment.py
--rw-r--r--   0        0        0     3731 2023-03-28 18:38:57.978167 jiwer-3.0.1/jiwer/cli.py
--rw-r--r--   0        0        0    15308 2023-03-28 18:38:57.978167 jiwer-3.0.1/jiwer/measures.py
--rw-r--r--   0        0        0    13422 2023-03-28 18:38:57.978167 jiwer-3.0.1/jiwer/process.py
--rw-r--r--   0        0        0     3670 2023-03-28 18:38:57.978167 jiwer-3.0.1/jiwer/transformations.py
--rw-r--r--   0        0        0    17834 2023-03-28 18:38:57.978167 jiwer-3.0.1/jiwer/transforms.py
--rw-r--r--   0        0        0      651 2023-03-28 18:38:57.978167 jiwer-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     2555 1970-01-01 00:00:00.000000 jiwer-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-06-16 15:40:45.227239 jiwer-3.0.2/LICENSE
+-rw-r--r--   0        0        0     1729 2023-06-16 15:40:45.227239 jiwer-3.0.2/README.md
+-rw-r--r--   0        0        0      145 2023-06-16 15:40:45.227239 jiwer-3.0.2/jiwer/__init__.py
+-rw-r--r--   0        0        0     5971 2023-06-16 15:40:45.227239 jiwer-3.0.2/jiwer/alignment.py
+-rw-r--r--   0        0        0     3731 2023-06-16 15:40:45.227239 jiwer-3.0.2/jiwer/cli.py
+-rw-r--r--   0        0        0    15308 2023-06-16 15:40:45.227239 jiwer-3.0.2/jiwer/measures.py
+-rw-r--r--   0        0        0    13422 2023-06-16 15:40:45.231239 jiwer-3.0.2/jiwer/process.py
+-rw-r--r--   0        0        0     3670 2023-06-16 15:40:45.231239 jiwer-3.0.2/jiwer/transformations.py
+-rw-r--r--   0        0        0    17834 2023-06-16 15:40:45.231239 jiwer-3.0.2/jiwer/transforms.py
+-rw-r--r--   0        0        0      651 2023-06-16 15:40:45.231239 jiwer-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2555 1970-01-01 00:00:00.000000 jiwer-3.0.2/PKG-INFO
```

### Comparing `jiwer-3.0.1/LICENSE` & `jiwer-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jiwer-3.0.1/README.md` & `jiwer-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `jiwer-3.0.1/jiwer/alignment.py` & `jiwer-3.0.2/jiwer/alignment.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,27 +26,30 @@
 
 from jiwer.process import CharacterOutput, WordOutput, AlignmentChunk
 
 __all__ = ["visualize_alignment"]
 
 
 def visualize_alignment(
-    output: Union[WordOutput, CharacterOutput], show_measures: bool = True
+    output: Union[WordOutput, CharacterOutput],
+    show_measures: bool = True,
+    skip_correct: bool = True,
 ) -> str:
     """
     Visualize the output of [jiwer.process_words][process.process_words] and
     [jiwer.process_characters][process.process_characters]. The visualization
     shows the alignment between each processed reference and hypothesis pair.
     If `show_measures=True`, the output string will also contain all measures in the
     output.
 
     Args:
         output: The processed output of reference and hypothesis pair(s).
         show_measures: If enabled, the visualization will include measures like the WER
                        or CER
+        skip_correct: If enabled, the visualization will exclude correct reference and hypothesis pairs
 
     Returns:
         (str): The visualization as a string
 
     Example:
         This code snippet
         ```python
@@ -97,14 +100,17 @@
     references = output.references
     hypothesis = output.hypotheses
     alignment = output.alignments
     is_cer = isinstance(output, CharacterOutput)
 
     final_str = ""
     for idx, (gt, hp, chunks) in enumerate(zip(references, hypothesis, alignment)):
+        if skip_correct and len(chunks) == 1 and chunks[0].type == "equal":
+            continue
+
         final_str += f"sentence {idx+1}\n"
         final_str += _construct_comparison_string(
             gt, hp, chunks, include_space_seperator=not is_cer
         )
         final_str += "\n"
 
     if show_measures:
```

### Comparing `jiwer-3.0.1/jiwer/cli.py` & `jiwer-3.0.2/jiwer/cli.py`

 * *Files identical despite different names*

### Comparing `jiwer-3.0.1/jiwer/measures.py` & `jiwer-3.0.2/jiwer/measures.py`

 * *Files identical despite different names*

### Comparing `jiwer-3.0.1/jiwer/process.py` & `jiwer-3.0.2/jiwer/process.py`

 * *Files identical despite different names*

### Comparing `jiwer-3.0.1/jiwer/transformations.py` & `jiwer-3.0.2/jiwer/transformations.py`

 * *Files identical despite different names*

### Comparing `jiwer-3.0.1/jiwer/transforms.py` & `jiwer-3.0.2/jiwer/transforms.py`

 * *Files identical despite different names*

### Comparing `jiwer-3.0.1/pyproject.toml` & `jiwer-3.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jiwer"
-version = "3.0.1"
+version = "3.0.2"
 description = "Evaluate your speech-to-text system with similarity measures such as word error rate (WER)"
 authors = ["Nik Vaessen <nikvaes@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/jitsi/jiwer"
 include = ["LICENCE"]
```

### Comparing `jiwer-3.0.1/PKG-INFO` & `jiwer-3.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiwer
-Version: 3.0.1
+Version: 3.0.2
 Summary: Evaluate your speech-to-text system with similarity measures such as word error rate (WER)
 Home-page: https://github.com/jitsi/jiwer
 License: Apache-2.0
 Author: Nik Vaessen
 Author-email: nikvaes@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

