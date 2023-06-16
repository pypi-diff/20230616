# Comparing `tmp/pyrealb-2.3.5.tar.gz` & `tmp/pyrealb-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrealb-2.3.5.tar", last modified: Sat May 27 19:28:10 2023, max compression
+gzip compressed data, was "pyrealb-2.3.6.tar", last modified: Fri Jun 16 20:41:07 2023, max compression
```

## Comparing `pyrealb-2.3.5.tar` & `pyrealb-2.3.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-27 19:28:10.932472 pyrealb-2.3.5/
--rw-r--r--   0 lapalme    (503) staff       (20)    35129 2021-12-01 22:24:50.000000 pyrealb-2.3.5/LICENSE
--rw-r--r--   0 lapalme    (503) staff       (20)       23 2022-01-27 01:45:34.000000 pyrealb-2.3.5/MANIFEST.in
--rw-r--r--   0 lapalme    (503) staff       (20)     7577 2023-05-27 19:28:10.932522 pyrealb-2.3.5/PKG-INFO
--rw-r--r--   0 lapalme    (503) staff       (20)     7080 2023-05-27 19:23:04.000000 pyrealb-2.3.5/README.md
--rw-r--r--   0 lapalme    (503) staff       (20)      104 2021-12-13 01:31:17.000000 pyrealb-2.3.5/pyproject.toml
--rw-r--r--   0 lapalme    (503) staff       (20)      649 2023-05-27 19:28:10.932745 pyrealb-2.3.5/setup.cfg
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-27 19:28:10.923357 pyrealb-2.3.5/src/
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-27 19:28:10.925145 pyrealb-2.3.5/src/pyrealb/
--rw-r--r--   0 lapalme    (503) staff       (20)    44540 2023-05-24 14:55:41.000000 pyrealb-2.3.5/src/pyrealb/Constituent.py
--rw-r--r--   0 lapalme    (503) staff       (20)    40808 2023-05-24 14:36:19.000000 pyrealb-2.3.5/src/pyrealb/Dependent.py
--rw-r--r--   0 lapalme    (503) staff       (20)     3050 2023-05-24 14:52:06.000000 pyrealb-2.3.5/src/pyrealb/Lexicon.py
--rw-r--r--   0 lapalme    (503) staff       (20)     7609 2023-05-25 19:51:40.000000 pyrealb-2.3.5/src/pyrealb/Number.py
--rw-r--r--   0 lapalme    (503) staff       (20)    57924 2023-05-24 14:43:55.000000 pyrealb-2.3.5/src/pyrealb/Phrase.py
--rw-r--r--   0 lapalme    (503) staff       (20)    37885 2023-05-26 01:43:01.000000 pyrealb-2.3.5/src/pyrealb/Terminal.py
--rw-r--r--   0 lapalme    (503) staff       (20)    14266 2023-03-27 13:03:50.000000 pyrealb-2.3.5/src/pyrealb/Warning.py
--rw-r--r--   0 lapalme    (503) staff       (20)      857 2023-05-24 14:58:21.000000 pyrealb-2.3.5/src/pyrealb/__init__.py
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-27 19:28:10.927754 pyrealb-2.3.5/src/pyrealb/data/
--rw-r--r--   0 lapalme    (503) staff       (20)  1324969 2023-05-25 18:45:57.000000 pyrealb-2.3.5/src/pyrealb/data/lexicon-en.json
--rw-r--r--   0 lapalme    (503) staff       (20)  2479817 2023-05-25 18:45:57.000000 pyrealb-2.3.5/src/pyrealb/data/lexicon-fr.json
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-27 19:28:10.931892 pyrealb-2.3.5/src/pyrealb/data/pyrealb.egg-info/
--rw-r--r--   0 lapalme    (503) staff       (20)     4155 2022-01-26 22:41:53.000000 pyrealb-2.3.5/src/pyrealb/data/pyrealb.egg-info/PKG-INFO
--rw-r--r--   0 lapalme    (503) staff       (20)        0 2022-01-26 22:41:53.000000 pyrealb-2.3.5/src/pyrealb/data/pyrealb.egg-info/SOURCES.txt
--rw-r--r--   0 lapalme    (503) staff       (20)        1 2022-01-26 22:41:53.000000 pyrealb-2.3.5/src/pyrealb/data/pyrealb.egg-info/dependency_links.txt
--rw-r--r--   0 lapalme    (503) staff       (20)        8 2022-01-26 22:41:53.000000 pyrealb-2.3.5/src/pyrealb/data/pyrealb.egg-info/top_level.txt
--rw-r--r--   0 lapalme    (503) staff       (20)    85976 2023-05-24 15:04:29.000000 pyrealb-2.3.5/src/pyrealb/data/rules-en.json
--rw-r--r--   0 lapalme    (503) staff       (20)   173554 2022-06-14 19:51:41.000000 pyrealb-2.3.5/src/pyrealb/data/rules-fr.json
--rw-r--r--   0 lapalme    (503) staff       (20)     2953 2023-05-27 19:23:04.000000 pyrealb-2.3.5/src/pyrealb/utils.py
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-27 19:28:10.925628 pyrealb-2.3.5/src/pyrealb.egg-info/
--rw-r--r--   0 lapalme    (503) staff       (20)     7577 2023-05-27 19:28:10.000000 pyrealb-2.3.5/src/pyrealb.egg-info/PKG-INFO
--rw-r--r--   0 lapalme    (503) staff       (20)      756 2023-05-27 19:28:10.000000 pyrealb-2.3.5/src/pyrealb.egg-info/SOURCES.txt
--rw-r--r--   0 lapalme    (503) staff       (20)        1 2023-05-27 19:28:10.000000 pyrealb-2.3.5/src/pyrealb.egg-info/dependency_links.txt
--rw-r--r--   0 lapalme    (503) staff       (20)        8 2023-05-27 19:28:10.000000 pyrealb-2.3.5/src/pyrealb.egg-info/top_level.txt
-drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-05-27 19:28:10.932363 pyrealb-2.3.5/tests/
--rw-r--r--   0 lapalme    (503) staff       (20)     1879 2023-03-04 13:28:19.000000 pyrealb-2.3.5/tests/test.py
--rw-r--r--   0 lapalme    (503) staff       (20)     2870 2023-02-24 19:49:08.000000 pyrealb-2.3.5/tests/testAll.py
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-06-16 20:41:07.372591 pyrealb-2.3.6/
+-rw-r--r--   0 lapalme    (503) staff       (20)    35129 2021-12-01 22:24:50.000000 pyrealb-2.3.6/LICENSE
+-rw-r--r--   0 lapalme    (503) staff       (20)       23 2022-01-27 01:45:34.000000 pyrealb-2.3.6/MANIFEST.in
+-rw-r--r--   0 lapalme    (503) staff       (20)     7578 2023-06-16 20:41:07.372663 pyrealb-2.3.6/PKG-INFO
+-rw-r--r--   0 lapalme    (503) staff       (20)     7081 2023-06-16 20:39:39.000000 pyrealb-2.3.6/README.md
+-rw-r--r--   0 lapalme    (503) staff       (20)      104 2021-12-13 01:31:17.000000 pyrealb-2.3.6/pyproject.toml
+-rw-r--r--   0 lapalme    (503) staff       (20)      649 2023-06-16 20:41:07.372888 pyrealb-2.3.6/setup.cfg
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-06-16 20:41:07.361863 pyrealb-2.3.6/src/
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-06-16 20:41:07.365967 pyrealb-2.3.6/src/pyrealb/
+-rw-r--r--   0 lapalme    (503) staff       (20)    44540 2023-05-24 14:55:41.000000 pyrealb-2.3.6/src/pyrealb/Constituent.py
+-rw-r--r--   0 lapalme    (503) staff       (20)    41365 2023-06-16 20:26:39.000000 pyrealb-2.3.6/src/pyrealb/Dependent.py
+-rw-r--r--   0 lapalme    (503) staff       (20)     3050 2023-05-24 14:52:06.000000 pyrealb-2.3.6/src/pyrealb/Lexicon.py
+-rw-r--r--   0 lapalme    (503) staff       (20)     7609 2023-05-25 19:51:40.000000 pyrealb-2.3.6/src/pyrealb/Number.py
+-rw-r--r--   0 lapalme    (503) staff       (20)    58433 2023-06-16 20:18:10.000000 pyrealb-2.3.6/src/pyrealb/Phrase.py
+-rw-r--r--   0 lapalme    (503) staff       (20)    37991 2023-06-16 20:21:55.000000 pyrealb-2.3.6/src/pyrealb/Terminal.py
+-rw-r--r--   0 lapalme    (503) staff       (20)    14266 2023-03-27 13:03:50.000000 pyrealb-2.3.6/src/pyrealb/Warning.py
+-rw-r--r--   0 lapalme    (503) staff       (20)      857 2023-05-24 14:58:21.000000 pyrealb-2.3.6/src/pyrealb/__init__.py
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-06-16 20:41:07.368821 pyrealb-2.3.6/src/pyrealb/data/
+-rw-r--r--   0 lapalme    (503) staff       (20)  1324966 2023-06-02 03:26:46.000000 pyrealb-2.3.6/src/pyrealb/data/lexicon-en.json
+-rw-r--r--   0 lapalme    (503) staff       (20)  2479817 2023-05-25 18:45:57.000000 pyrealb-2.3.6/src/pyrealb/data/lexicon-fr.json
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-06-16 20:41:07.372068 pyrealb-2.3.6/src/pyrealb/data/pyrealb.egg-info/
+-rw-r--r--   0 lapalme    (503) staff       (20)     4155 2022-01-26 22:41:53.000000 pyrealb-2.3.6/src/pyrealb/data/pyrealb.egg-info/PKG-INFO
+-rw-r--r--   0 lapalme    (503) staff       (20)        0 2022-01-26 22:41:53.000000 pyrealb-2.3.6/src/pyrealb/data/pyrealb.egg-info/SOURCES.txt
+-rw-r--r--   0 lapalme    (503) staff       (20)        1 2022-01-26 22:41:53.000000 pyrealb-2.3.6/src/pyrealb/data/pyrealb.egg-info/dependency_links.txt
+-rw-r--r--   0 lapalme    (503) staff       (20)        8 2022-01-26 22:41:53.000000 pyrealb-2.3.6/src/pyrealb/data/pyrealb.egg-info/top_level.txt
+-rw-r--r--   0 lapalme    (503) staff       (20)    85976 2023-05-24 15:04:29.000000 pyrealb-2.3.6/src/pyrealb/data/rules-en.json
+-rw-r--r--   0 lapalme    (503) staff       (20)   173554 2022-06-14 19:51:41.000000 pyrealb-2.3.6/src/pyrealb/data/rules-fr.json
+-rw-r--r--   0 lapalme    (503) staff       (20)     2953 2023-06-16 20:39:56.000000 pyrealb-2.3.6/src/pyrealb/utils.py
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-06-16 20:41:07.366482 pyrealb-2.3.6/src/pyrealb.egg-info/
+-rw-r--r--   0 lapalme    (503) staff       (20)     7578 2023-06-16 20:41:07.000000 pyrealb-2.3.6/src/pyrealb.egg-info/PKG-INFO
+-rw-r--r--   0 lapalme    (503) staff       (20)      756 2023-06-16 20:41:07.000000 pyrealb-2.3.6/src/pyrealb.egg-info/SOURCES.txt
+-rw-r--r--   0 lapalme    (503) staff       (20)        1 2023-06-16 20:41:07.000000 pyrealb-2.3.6/src/pyrealb.egg-info/dependency_links.txt
+-rw-r--r--   0 lapalme    (503) staff       (20)        8 2023-06-16 20:41:07.000000 pyrealb-2.3.6/src/pyrealb.egg-info/top_level.txt
+drwxr-xr-x   0 lapalme    (503) staff       (20)        0 2023-06-16 20:41:07.372467 pyrealb-2.3.6/tests/
+-rw-r--r--   0 lapalme    (503) staff       (20)     1879 2023-03-04 13:28:19.000000 pyrealb-2.3.6/tests/test.py
+-rw-r--r--   0 lapalme    (503) staff       (20)     2870 2023-02-24 19:49:08.000000 pyrealb-2.3.6/tests/testAll.py
```

### Comparing `pyrealb-2.3.5/LICENSE` & `pyrealb-2.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.5/PKG-INFO` & `pyrealb-2.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyrealb
-Version: 2.3.5
+Version: 2.3.6
 Summary: A French-English text realizer
 Home-page: https://github.com/lapalme/pyrealb
 Author: Guy Lapalme
 Author-email: lapalme@iro.umontreal.ca
 Project-URL: Bug Tracker, https://github.com/lapalme/pyrealb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # *pyRealB* - A Python Bilingual Text Realizer
 
-*Version 2.3.5 - May 2023*
+*Version 2.3.6 - June 2023*
 
 *pyRealB* is a Python adaptation of the JavaScript [**jsRealB**](http://rali.iro.umontreal.ca/jsRealB) 
 text realizer with the same constituent and dependency syntax notation. 
 It facilitates its integration within Python applications by simply adding
 
 	from pyrealb import *
```

### Comparing `pyrealb-2.3.5/README.md` & `pyrealb-2.3.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # *pyRealB* - A Python Bilingual Text Realizer
 
-*Version 2.3.5 - May 2023*
+*Version 2.3.6 - June 2023*
 
 *pyRealB* is a Python adaptation of the JavaScript [**jsRealB**](http://rali.iro.umontreal.ca/jsRealB) 
 text realizer with the same constituent and dependency syntax notation. 
 It facilitates its integration within Python applications by simply adding
 
 	from pyrealb import *
```

### Comparing `pyrealb-2.3.5/setup.cfg` & `pyrealb-2.3.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyrealb
-version = 2.3.5
+version = 2.3.6
 author = Guy Lapalme
 author_email = lapalme@iro.umontreal.ca
 description = A French-English text realizer
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/lapalme/pyrealb
 project_urls =
```

### Comparing `pyrealb-2.3.5/src/pyrealb/Constituent.py` & `pyrealb-2.3.6/src/pyrealb/Constituent.py`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.5/src/pyrealb/Dependent.py` & `pyrealb-2.3.6/src/pyrealb/Dependent.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,14 +165,21 @@
                     if iRel>=0:
                         rel = dep.dependents[iRel].constType
                         if rel=="subj": # verb agrees with this subject
                             depTerm.peng=self.peng
                         elif self.isFr(): # rel is comp or mod
                             # in French past participle can agree with a cod appearing before... keep that info in case
                             depTerm.cod=headTerm
+                            # HACK: check for a "temps composé" formed by "avoir" followed by a past participle
+                            if depTerm.lemma == "avoir":
+                                iVerb = dep.findIndex(lambda depI:depI.isA("comp") and
+                                                      depI.terminal.isA("V") and
+                                                      depI.terminal.getProp("t") == "pp")
+                                if iVerb >= 0:
+                                    dep.dependents[iVerb].terminal.cod = headTerm
                     # check for past participle in French that should agree with the head
                     if self.isFr() and depTerm.getProp("t")=="pp":
                         depTerm.peng=self.peng
                 elif depTerm.isA("Pro") and depTerm.lemma in ["qui","que","who","that"]:
                     # a relative linked to depTerm in which the new peng should be propagated
                     if hasattr(self,"peng"):
                         depTerm.peng=self.peng
```

### Comparing `pyrealb-2.3.5/src/pyrealb/Lexicon.py` & `pyrealb-2.3.6/src/pyrealb/Lexicon.py`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.5/src/pyrealb/Number.py` & `pyrealb-2.3.6/src/pyrealb/Number.py`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.5/src/pyrealb/Phrase.py` & `pyrealb-2.3.6/src/pyrealb/Phrase.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,14 +207,21 @@
                     if v is not None:
                         if pro.lemma in ["qui", "who", "which", "that"]:  # agrees with self NP
                             v.peng = self.peng
                             self.linkAttributes(v,self.getFromPath([["VP"],["CP"]]),self)
                         elif self.isFr() and pro.lemma == "que":
                             # in French past participle can agree with a cod appearing before... keep that info just in case
                             v.cod = self
+                            # HACK: check for a "temps composé" formed by "avoir" followed by a past participle
+                            if v.lemma == "avoir":
+                                idx = v.parentConst.getIndex("V")
+                                if len(v.parentConst.elements)>idx+1:
+                                    next=v.parentConst.elements[idx+1]
+                                    if next.isA("V") and next.getProp("t") == "pp":
+                                        next.cod=self
         elif self.isA("VP"):
             headIndex = self.getHeadIndex("VP")  # head is the first internal V
             self.peng = self.elements[headIndex].peng
             self.taux = self.elements[headIndex].taux
         elif self.isOneOf(["AdvP", "PP", "AP"]):
             headIndex = self.getHeadIndex(self.constType)
             if hasattr(self.elements[headIndex], "peng"):
```

### Comparing `pyrealb-2.3.5/src/pyrealb/Terminal.py` & `pyrealb-2.3.6/src/pyrealb/Terminal.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         if isinstance(lemma, str):
             lemma=lemma.replace("œ","oe").replace("æ","ae")
         self.lemma=lemma
         if not hasattr(self, "peng"):self.initProps()
         if terminalType=="DT":
             if lemma is None or lemma=="":
                 self.date=datetime.datetime.today()
+                self.lemma=str(self.date)
             else:
                 if isinstance(lemma,str):
                     self.date=self.parseDateString(lemma)
                 elif isinstance(lemma,datetime.datetime):
                     self.date=lemma
                 else:
                     self.warn("bad parameter","str,datetime.datetime",type(lemma).__name__)
@@ -478,17 +479,18 @@
                     return res
                 elif t in ["b","pr","pp"]:
                     self.realization=self.stem+conjugation[t]
                     res=[self]
                     if t!="pp" and self.isReflexive() and self.parentConst is None:
                         self.insertReal(res, Pro("moi","fr").c("refl").pe(pe).n(n).g(g), 0)
                     if t=="pp" and self.realization!="été": # HACK: frequent case of être that does not change
-                        g=self.getProp("g")
+                        x = self.cod if hasattr(self,"cod") else self
+                        g=x.getProp("g")
                         if g=="x" or g=="n":g="m"   # neutre peut arriver si le sujet est en anglais
-                        n=self.getProp("n")
+                        n=x.getProp("n")
                         if n=="x":n="s"
                         if (g+n)=="mp" and self.realization.endswith("s"):
                             pass    # pas d'ajout de s au masculin pluriel si la réalisation termine en s
                         else:
                             if (g+n)!="ms" and self.realization.endswith("û"): #changer "dû" en "du" sauf pour masc sing
                                 self.realization = self.realization[:-1]+"u"+{"ms":"","mp":"s","fs":"e","fp":"es"}[g+n]
                             else:
```

### Comparing `pyrealb-2.3.5/src/pyrealb/Warning.py` & `pyrealb-2.3.6/src/pyrealb/Warning.py`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.5/src/pyrealb/__init__.py` & `pyrealb-2.3.6/src/pyrealb/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.5/src/pyrealb/data/lexicon-en.json` & `pyrealb-2.3.6/src/pyrealb/data/lexicon-en.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999953954735663%*

 * *Differences: {"'bias'": "{'V': {'tab': 'v1'}}",*

 * * "'grave'": "{'V': {'tab': 'v3'}}",*

 * * "'smell'": "{'V': {'tab': 'v97'}}",*

 * * "'spell'": "{'V': {'tab': 'v97'}}"}*

```diff
@@ -18922,15 +18922,15 @@
         }
     },
     "bias": {
         "N": {
             "tab": "n2"
         },
         "V": {
-            "tab": "v56"
+            "tab": "v1"
         },
         "basic": true
     },
     "bib": {
         "N": {
             "tab": "n1"
         },
@@ -73547,15 +73547,15 @@
         "A": {
             "tab": "a2"
         },
         "N": {
             "tab": "n1"
         },
         "V": {
-            "tab": "v170"
+            "tab": "v3"
         },
         "basic": true
     },
     "grave-clothes": {
         "N": {
             "tab": "n6"
         }
@@ -154951,15 +154951,15 @@
         }
     },
     "smell": {
         "N": {
             "tab": "n1"
         },
         "V": {
-            "tab": "v99"
+            "tab": "v97"
         },
         "basic": true
     },
     "smelling-bottle": {
         "N": {
             "tab": "n1"
         }
@@ -158191,15 +158191,15 @@
         }
     },
     "spell": {
         "N": {
             "tab": "n1"
         },
         "V": {
-            "tab": "v98"
+            "tab": "v97"
         },
         "basic": true
     },
     "spellbinder": {
         "N": {
             "tab": "n1"
         }
```

### Comparing `pyrealb-2.3.5/src/pyrealb/data/lexicon-fr.json` & `pyrealb-2.3.6/src/pyrealb/data/lexicon-fr.json`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.5/src/pyrealb/data/pyrealb.egg-info/PKG-INFO` & `pyrealb-2.3.6/src/pyrealb/data/pyrealb.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.5/src/pyrealb/data/rules-en.json` & `pyrealb-2.3.6/src/pyrealb/data/rules-en.json`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.5/src/pyrealb/data/rules-fr.json` & `pyrealb-2.3.6/src/pyrealb/data/rules-fr.json`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.5/src/pyrealb/utils.py` & `pyrealb-2.3.6/src/pyrealb/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,9 +71,9 @@
 
 # useful variables for using expressions written originally for the javascript version
 false = False
 true = True
 null = None
 
 # version and date informations
-pyrealb_version = "2.3.5"
+pyrealb_version = "2.3.6"
 pyrealb_datecreated = datetime.datetime.today()
```

### Comparing `pyrealb-2.3.5/src/pyrealb.egg-info/PKG-INFO` & `pyrealb-2.3.6/src/pyrealb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyrealb
-Version: 2.3.5
+Version: 2.3.6
 Summary: A French-English text realizer
 Home-page: https://github.com/lapalme/pyrealb
 Author: Guy Lapalme
 Author-email: lapalme@iro.umontreal.ca
 Project-URL: Bug Tracker, https://github.com/lapalme/pyrealb/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # *pyRealB* - A Python Bilingual Text Realizer
 
-*Version 2.3.5 - May 2023*
+*Version 2.3.6 - June 2023*
 
 *pyRealB* is a Python adaptation of the JavaScript [**jsRealB**](http://rali.iro.umontreal.ca/jsRealB) 
 text realizer with the same constituent and dependency syntax notation. 
 It facilitates its integration within Python applications by simply adding
 
 	from pyrealb import *
```

### Comparing `pyrealb-2.3.5/src/pyrealb.egg-info/SOURCES.txt` & `pyrealb-2.3.6/src/pyrealb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.5/tests/test.py` & `pyrealb-2.3.6/tests/test.py`

 * *Files identical despite different names*

### Comparing `pyrealb-2.3.5/tests/testAll.py` & `pyrealb-2.3.6/tests/testAll.py`

 * *Files identical despite different names*

