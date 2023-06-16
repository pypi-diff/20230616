# Comparing `tmp/piccolo_theme-0.8.1.tar.gz` & `tmp/piccolo_theme-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piccolo_theme-0.8.1.tar", last modified: Tue Apr  5 19:58:36 2022, max compression
+gzip compressed data, was "piccolo_theme-0.9.0.tar", last modified: Thu Apr 14 19:50:45 2022, max compression
```

## Comparing `piccolo_theme-0.8.1.tar` & `piccolo_theme-0.9.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 19:58:36.886796 piccolo_theme-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-04-05 19:58:27.000000 piccolo_theme-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-05 19:58:27.000000 piccolo_theme-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2688 2022-04-05 19:58:36.886796 piccolo_theme-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1906 2022-04-05 19:58:27.000000 piccolo_theme-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 19:58:36.882796 piccolo_theme-0.8.1/piccolo_theme/
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-04-05 19:58:27.000000 piccolo_theme-0.8.1/piccolo_theme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 19:58:36.882796 piccolo_theme-0.8.1/piccolo_theme/components/
--rw-r--r--   0 runner    (1001) docker     (121)     9501 2022-04-05 19:58:27.000000 piccolo_theme-0.8.1/piccolo_theme/components/dark_mode_toggle.html
--rw-r--r--   0 runner    (1001) docker     (121)     4048 2022-04-05 19:58:27.000000 piccolo_theme-0.8.1/piccolo_theme/components/notification_banner.html
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-04-05 19:58:27.000000 piccolo_theme-0.8.1/piccolo_theme/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (121)     3068 2022-04-05 19:58:27.000000 piccolo_theme-0.8.1/piccolo_theme/layout.html
--rw-r--r--   0 runner    (1001) docker     (121)     3003 2022-04-05 19:58:27.000000 piccolo_theme-0.8.1/piccolo_theme/snippets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 19:58:36.882796 piccolo_theme-0.8.1/piccolo_theme/static/
--rw-r--r--   0 runner    (1001) docker     (121)    27385 2022-04-05 19:58:27.000000 piccolo_theme-0.8.1/piccolo_theme/static/basic_mod.css
--rw-r--r--   0 runner    (1001) docker     (121)     4940 2022-04-05 19:58:27.000000 piccolo_theme-0.8.1/piccolo_theme/static/basic_mod.css.map
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 19:58:36.882796 piccolo_theme-0.8.1/piccolo_theme/static/js/
--rw-r--r--   0 runner    (1001) docker     (121)    16901 2022-04-05 19:58:27.000000 piccolo_theme-0.8.1/piccolo_theme/static/js/petite-vue.js
--rw-r--r--   0 runner    (1001) docker     (121)     3442 2022-04-05 19:58:27.000000 piccolo_theme-0.8.1/piccolo_theme/static/js/theme.js
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-04-05 19:58:27.000000 piccolo_theme-0.8.1/piccolo_theme/theme.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 19:58:36.882796 piccolo_theme-0.8.1/piccolo_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2688 2022-04-05 19:58:36.000000 piccolo_theme-0.8.1/piccolo_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-04-05 19:58:36.000000 piccolo_theme-0.8.1/piccolo_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-05 19:58:36.000000 piccolo_theme-0.8.1/piccolo_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-04-05 19:58:36.000000 piccolo_theme-0.8.1/piccolo_theme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-04-05 19:58:36.000000 piccolo_theme-0.8.1/piccolo_theme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-04-05 19:58:27.000000 piccolo_theme-0.8.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-05 19:58:36.882796 piccolo_theme-0.8.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-05 19:58:27.000000 piccolo_theme-0.8.1/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-05 19:58:36.886796 piccolo_theme-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1763 2022-04-05 19:58:27.000000 piccolo_theme-0.8.1/setup.py
+drwxr-xr-x   0 dantownsend   (501) staff       (20)        0 2022-04-14 19:50:45.656458 piccolo_theme-0.9.0/
+-rw-r--r--   0 dantownsend   (501) staff       (20)     1072 2022-02-17 20:18:35.000000 piccolo_theme-0.9.0/LICENSE
+-rw-r--r--   0 dantownsend   (501) staff       (20)       38 2022-02-21 20:29:58.000000 piccolo_theme-0.9.0/MANIFEST.in
+-rw-r--r--   0 dantownsend   (501) staff       (20)     2688 2022-04-14 19:50:45.655811 piccolo_theme-0.9.0/PKG-INFO
+-rw-r--r--   0 dantownsend   (501) staff       (20)     1906 2022-04-05 09:43:49.000000 piccolo_theme-0.9.0/README.md
+drwxr-xr-x   0 dantownsend   (501) staff       (20)        0 2022-04-14 19:50:45.646044 piccolo_theme-0.9.0/piccolo_theme/
+-rw-r--r--   0 dantownsend   (501) staff       (20)      335 2022-04-14 19:38:19.000000 piccolo_theme-0.9.0/piccolo_theme/__init__.py
+drwxr-xr-x   0 dantownsend   (501) staff       (20)        0 2022-04-14 19:50:45.650049 piccolo_theme-0.9.0/piccolo_theme/components/
+-rw-r--r--   0 dantownsend   (501) staff       (20)     9501 2022-03-22 21:01:33.000000 piccolo_theme-0.9.0/piccolo_theme/components/dark_mode_toggle.html
+-rw-r--r--   0 dantownsend   (501) staff       (20)     4048 2022-03-23 15:23:38.000000 piccolo_theme-0.9.0/piccolo_theme/components/notification_banner.html
+-rw-r--r--   0 dantownsend   (501) staff       (20)      147 2022-02-15 19:58:19.000000 piccolo_theme-0.9.0/piccolo_theme/globaltoc.html
+-rw-r--r--   0 dantownsend   (501) staff       (20)     3068 2022-04-05 19:52:15.000000 piccolo_theme-0.9.0/piccolo_theme/layout.html
+-rw-r--r--   0 dantownsend   (501) staff       (20)     3003 2022-03-17 10:41:42.000000 piccolo_theme-0.9.0/piccolo_theme/snippets.py
+drwxr-xr-x   0 dantownsend   (501) staff       (20)        0 2022-04-14 19:50:45.652568 piccolo_theme-0.9.0/piccolo_theme/static/
+-rw-r--r--   0 dantownsend   (501) staff       (20)    27436 2022-04-14 19:36:57.000000 piccolo_theme-0.9.0/piccolo_theme/static/basic_mod.css
+-rw-r--r--   0 dantownsend   (501) staff       (20)     4918 2022-04-14 19:36:57.000000 piccolo_theme-0.9.0/piccolo_theme/static/basic_mod.css.map
+drwxr-xr-x   0 dantownsend   (501) staff       (20)        0 2022-04-14 19:50:45.654597 piccolo_theme-0.9.0/piccolo_theme/static/js/
+-rw-r--r--   0 dantownsend   (501) staff       (20)    16901 2022-02-26 16:00:59.000000 piccolo_theme-0.9.0/piccolo_theme/static/js/petite-vue.js
+-rw-r--r--   0 dantownsend   (501) staff       (20)     3476 2022-04-14 19:36:57.000000 piccolo_theme-0.9.0/piccolo_theme/static/js/theme.js
+-rw-r--r--   0 dantownsend   (501) staff       (20)      243 2022-03-23 09:17:17.000000 piccolo_theme-0.9.0/piccolo_theme/theme.conf
+drwxr-xr-x   0 dantownsend   (501) staff       (20)        0 2022-04-14 19:50:45.648615 piccolo_theme-0.9.0/piccolo_theme.egg-info/
+-rw-r--r--   0 dantownsend   (501) staff       (20)     2688 2022-04-14 19:50:45.000000 piccolo_theme-0.9.0/piccolo_theme.egg-info/PKG-INFO
+-rw-r--r--   0 dantownsend   (501) staff       (20)      645 2022-04-14 19:50:45.000000 piccolo_theme-0.9.0/piccolo_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 dantownsend   (501) staff       (20)        1 2022-04-14 19:50:45.000000 piccolo_theme-0.9.0/piccolo_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 dantownsend   (501) staff       (20)       52 2022-04-14 19:50:45.000000 piccolo_theme-0.9.0/piccolo_theme.egg-info/entry_points.txt
+-rw-r--r--   0 dantownsend   (501) staff       (20)       14 2022-04-14 19:50:45.000000 piccolo_theme-0.9.0/piccolo_theme.egg-info/top_level.txt
+-rw-r--r--   0 dantownsend   (501) staff       (20)      104 2022-02-08 13:41:27.000000 piccolo_theme-0.9.0/pyproject.toml
+drwxr-xr-x   0 dantownsend   (501) staff       (20)        0 2022-04-14 19:50:45.655265 piccolo_theme-0.9.0/requirements/
+-rw-r--r--   0 dantownsend   (501) staff       (20)        0 2022-02-17 12:04:27.000000 piccolo_theme-0.9.0/requirements/requirements.txt
+-rw-r--r--   0 dantownsend   (501) staff       (20)       38 2022-04-14 19:50:45.656674 piccolo_theme-0.9.0/setup.cfg
+-rw-r--r--   0 dantownsend   (501) staff       (20)     1763 2022-03-07 12:29:20.000000 piccolo_theme-0.9.0/setup.py
```

### Comparing `piccolo_theme-0.8.1/LICENSE` & `piccolo_theme-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `piccolo_theme-0.8.1/PKG-INFO` & `piccolo_theme-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piccolo_theme
-Version: 0.8.1
+Version: 0.9.0
 Summary: A modern Sphinx theme.
 Home-page: https://github.com/piccolo-orm/piccolo_theme
 Author: Daniel Townsend
 Author-email: dan@dantownsend.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `piccolo_theme-0.8.1/README.md` & `piccolo_theme-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `piccolo_theme-0.8.1/piccolo_theme/components/dark_mode_toggle.html` & `piccolo_theme-0.9.0/piccolo_theme/components/dark_mode_toggle.html`

 * *Files identical despite different names*

### Comparing `piccolo_theme-0.8.1/piccolo_theme/components/notification_banner.html` & `piccolo_theme-0.9.0/piccolo_theme/components/notification_banner.html`

 * *Files identical despite different names*

### Comparing `piccolo_theme-0.8.1/piccolo_theme/layout.html` & `piccolo_theme-0.9.0/piccolo_theme/layout.html`

 * *Files identical despite different names*

### Comparing `piccolo_theme-0.8.1/piccolo_theme/snippets.py` & `piccolo_theme-0.9.0/piccolo_theme/snippets.py`

 * *Files identical despite different names*

### Comparing `piccolo_theme-0.8.1/piccolo_theme/static/basic_mod.css` & `piccolo_theme-0.9.0/piccolo_theme/static/basic_mod.css`

 * *Files 1% similar despite different names*

```diff
@@ -428,45 +428,39 @@
 }
 div.document dl.py span.sig-return span.sig-return-typehint pre {
   color: var(--fontColor);
 }
 div.document dl.py em.sig-param > span:first-child {
   font-weight: bold;
 }
-div.document dl:not(.cpp) dt.cpp.sig em {
-  color: var(--fontColor);
-}
-div.document dl:not(.cpp) dt.cpp.sig span.descname {
-  color: var(--fontColor);
-}
-div.document dl.cpp {
+div.document dl.cpp, div.document dl.c {
   margin-bottom: 1rem;
 }
-div.document dl.cpp dt.sig {
+div.document dl.cpp dt.sig, div.document dl.c dt.sig {
   background-color: var(--codeBackgroundColor);
   color: var(--fontColor);
   box-sizing: border-box;
   font-family: "Roboto Mono", monospace, Monaco, Consolas, Andale Mono;
   font-size: 0.9rem;
   padding: 1rem;
   border-left: 5px solid rgba(0, 0, 0, 0.1);
   border-radius: 0.2rem;
   line-height: 1.4;
 }
-div.document dl.cpp span.sig-name {
+div.document dl.cpp span.sig-name, div.document dl.c span.sig-name {
   color: var(--codeBlue);
   font-weight: bold;
 }
-div.document dl.cpp span.sig-indent {
+div.document dl.cpp span.sig-indent, div.document dl.c span.sig-indent {
   margin-left: 2rem;
 }
-div.document dl.cpp span.target + span {
+div.document dl.cpp span.target + span, div.document dl.c span.target + span {
   color: var(--codeGreen);
 }
-div.document dl.cpp span.sig-param > span:first-child {
+div.document dl.cpp span.sig-param > span:first-child, div.document dl.c span.sig-param > span:first-child {
   font-weight: bold;
 }
 div.document div.admonition {
   box-shadow: 0px 0px 0px 1px var(--dividerColor);
   border-radius: 0.2rem;
   margin: 1rem 0;
   overflow: hidden;
```

### Comparing `piccolo_theme-0.8.1/piccolo_theme/static/basic_mod.css.map` & `piccolo_theme-0.9.0/piccolo_theme/static/basic_mod.css.map`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'mappings'": "'AAEQ;AAUR;AACA;AAEA;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAEA;EACE;EACA;EACA;EACA;;AAGF;EACE;EACA;EACA;EACA;;AAGF;EAEE;EACA;EACA;EACA;EACA;EACA;EACA;;;AAIJ;EACE;EACA;EACA;;;AAGF;EACE;;;AAGF;EACE;;;AAGF;EACE;;;AAGF;EACE;EACA;;;AAGF;AAEA;EACE;EAEA;;;AAGF;AAAA;EAEE;EACA;EACA;;;AAGF;EACE;EACA;;;AAGF;AACA;AAGE;EACE;;AAGF;EACE;EACA;;AAEA;EACE;EACA;EACA;EACA;EACA,eA9GS;;AAiHX;EACE;EACA;EACA;EACA;;AAEA;EACE;;AAIJ;EACE;EACA;EACA;EACA;EACA;;;AAKN;EACE;EACA;EACA;EACA; […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "basic_mod.css",
-    "mappings": "AAEQ;AAUR;AACA;AAEA;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAEA;EACE;EACA;EACA;EACA;;AAGF;EACE;EACA;EACA;EACA;;AAGF;EAEE;EACA;EACA;EACA;EACA;EACA;EACA;;;AAIJ;EACE;EACA;EACA;;;AAGF;EACE;;;AAGF;EACE;;;AAGF;EACE;;;AAGF;EACE;EACA;;;AAGF;AAEA;EACE;EAEA;;;AAGF;AAAA;EAEE;EACA;EACA;;;AAGF;EACE;EACA;;;AAGF;AACA;AAGE;EACE;;AAGF;EACE;EACA;;AAEA;EACE;EACA;EACA;EACA;EACA,eA9GS;;AAiHX;EACE;EACA;EACA;EACA;;AAEA;EACE;;AAIJ;EACE;EACA;EACA;EACA;EACA;;;AAKN;EACE;EACA;EACA;EACA;EACA;EACA;;AAEA;EACE;EACA;EACA;EACA;EACA;EACA;EACA;;AAEA;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAEA;EACE;;AAIJ;EACE;EACA;EACA;EACA;EACA;EACA;;AAEA;EACE;EACA;;AAMN;EACE;EACA;EACA;EACA;EACA;EACA;;AAEA;EACE;EACA;EACA;EACA;EACA;;AAEA;EACE;;AAKJ;EACE;EACA;EACA;EACA;EACA;;AAEA;EACE,OAvNa;EAwNb;;AAKJ;EACE;EACA;EACA;;AAEA;EACE;EACA;EACA;;AAKJ;EACE;;AAEA;EAHF;IAII;;;AAGF;EACE;;AAEA;EACE;EACA;;AAOJ;EADF;IAEI;;;AAGF;EACE;EACA;EACA;;AAGE;EACE;EACA;EACA;EACA;;AAEA;EACE;;;AASd;AACA;AAEA;EACE;EACA;EACA;EACA,aAxRa;EAyRb,cAzRa;EA0Rb;AAOA;AAqDA;;AA1DA;EARF;IASI;IACA;;;AAgBF;AAAA;EAEE;;AAGA;AAAA;EACE;;AAOJ;AAAA;EAEE;;AAIF;AAAA;EAEE;;AAIF;AAAA;EAEE;;AAGF;AAAA;EAEE;;AAGF;AAAA;EAEE;;AAKF;EACE;;AAGF;EACE;EACA;EACA,eAlWW;EAmWX,aArWO;EAsWP;;AAGF;EACE,WAvWW;EAwWX;EACA;EACA;EACA;;AAGF;EACE;EACA;EACA;EACA,eAnXW;EAoXX;EAIA;;AAEA;EACE,aA7XK;;AAkYT;EACE;;AAGF;EACE;EACA;EACA;EACA;;AAGF;AAAA;AAAA;AAAA;AAAA;AAAA;AAAA;AAAA;EAQE;;AAGF;EACE;;AAGF;EACE;;AAGF;EACE;;AAOA;AAAA;AAAA;AAAA;EACE;;AAIJ;AAAA;EAEE;EACA;;AAQA;EACE;;AAIJ;EACE;;AAGF;EACE;;AAGF;EACE;EACA;EACA;EACA;;AAGF;EACE;;AACA;EACE;EACA;EACA;;AAEA;EACE;;AAEF;EACE;;AAQN;EACE;EACA;;AAGF;EACE;;AAEA;EACE;;AAGF;EACE;EACA;;AAEA;EACE;EACA;;AAQJ;EACE;;AAIJ;EACE;;AAEA;EACE;EACA;EACA;EACA,aArgBK;EAsgBL;EACA;EACA;EACA,eAvgBS;;AA2gBX;EACE;EACA;;AAIF;EACE;EACA;;AAIF;EACE;;AAGF;EACE;;AAEA;EACE;;AAKF;EACE;;AAEA;EACE;;AAMN;EACE;;AAQF;EACE;;AAEF;EACE;;AAIJ;EACE;;AAEA;EACE;EACA;EACA;EACA,aAxkBK;EAykBL;EACA;EACA;EACA,eA1kBS;EA2kBT;;AAIF;EACE;EACA;;AAIF;EACE;;AAIF;EACE;;AAIF;EACE;;AAMJ;EACE;EACA,eAxmBW;EAymBX;EACA;;AAEA;EACE;EACA;EACA;EACA;;AAGF;EACE;EACA;;AAGF;EACE;;AAGF;EACE;EACA;;AAGF;EAIE;;AAEA;EACE,OAJM;;AAQV;EAEE;;AAEA;EACE,OAJM;;AAQV;EAGE;;AAEA;EACE,OAJM;;AAQV;EAIE;;AAEA;EACE,OAJM;;;AAUd;AACA;AAwCA;EACE;EACA;EACA;EACA;EACA;EACA;EACA,OAztBa;EA0tBb;EACA;;AAEA;EAXF;IAYI;;;AAGF;EACE;EACA;;AAtDF;EACE;EACA;;AAEA;EACE;EACA;;AAEA;EACE;EACA;EACA;EACA;EACA;;AAEA;EACE;;AAGF;EACE;;AAKN;EACE;;AAMJ;EACE;;;AA4BJ;AACA;AAiBA;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAEA;EACE;;AAxBF;EACE;EACA;;AAEA;EACE;EACA;EACA;;;AAuBN;EACE;EACA;EACA;EACA;EACA;EACA,OAnxBa;EAoxBb;EACA;EACA;EACA;EACA;;AAzCA;EACE;EACA;;AAEA;EACE;EACA;EACA;;AAzEJ;EACE;EACA;;AAEA;EACE;EACA;;AAEA;EACE;EACA;EACA;EACA;EACA;;AAEA;EACE;;AAGF;EACE;;AAKN;EACE;;AAMJ;EACE;;AAmFF;EApBF;IAqBI;;;;AAIJ;AACA;AAEA;EACE;EACA;EACA;EACA;EACA;EACA;;;AAGF;EACE;EACA;EACA;EACA;;;AAGF;AACA;AAEA;EACE,aA7zBa;EA8zBb,cA9zBa;;AAg0Bb;EAJF;IAKI;IACA;;;AAGF;EACE,WAx0BW;EAy0BX;EACA;EACA;EACA;;AAEA;EACE;EACA;EACA;;AAEA;EACE;;AAEA;EACE;;AAGF;EACE;EACA;;AAKF;EACE;;AAEA;EACE;;AAMJ;EACE;;AAEA;EACE;;;AAQZ;AACA;AAOE;AAAA;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EAEA;EACA;AAoCE;AAGA;AAIA;AAGA;AAIA;AAIA;AAGA;AAIA;AAIA;AAIA;AAGA;AAGA;AAGA;AAIA;AAGA;AAGA;AAIA;AAGA;AAIA;AAGA;AAIA;AAIA;AAIA;AAGA;AAIA;AAGA;AAGA;AAGA;AAGA;AAGA;AAIA;AAGA;AAGA;AAIA;AAIA;AAGA;AAGA;AAIA;AAIA;AAGA;AAIA;AAGA;AAGA;AAGA;AAGA;AAGA;AAGA;AAGA;AAGA;AAGA;AAGA;AAIA;AAGA;AAIA;AAGA;AAIA;AAGA;AAGA;AAGA;AAGA;AAGA;AAGA;AAGA;AAGA;AAGA;AAGA;AAGA;;AA9PF;AAAA;EACE;;AAGF;AAAA;EACE;EACA;EACA;EACA;;AAEF;AAAA;EACE;EACA;EACA;EACA;;AAEF;AAAA;EACE;EACA;EACA;EACA;;AAEF;AAAA;EACE;EACA;EACA;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE",
+    "mappings": "AAEQ;AAUR;AACA;AAEA;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAEA;EACE;EACA;EACA;EACA;;AAGF;EACE;EACA;EACA;EACA;;AAGF;EAEE;EACA;EACA;EACA;EACA;EACA;EACA;;;AAIJ;EACE;EACA;EACA;;;AAGF;EACE;;;AAGF;EACE;;;AAGF;EACE;;;AAGF;EACE;EACA;;;AAGF;AAEA;EACE;EAEA;;;AAGF;AAAA;EAEE;EACA;EACA;;;AAGF;EACE;EACA;;;AAGF;AACA;AAGE;EACE;;AAGF;EACE;EACA;;AAEA;EACE;EACA;EACA;EACA;EACA,eA9GS;;AAiHX;EACE;EACA;EACA;EACA;;AAEA;EACE;;AAIJ;EACE;EACA;EACA;EACA;EACA;;;AAKN;EACE;EACA;EACA;EACA;EACA;EACA;;AAEA;EACE;EACA;EACA;EACA;EACA;EACA;EACA;;AAEA;EACE;EACA;EACA;EACA;EACA;EACA;EACA;EACA;EACA;;AAEA;EACE;;AAIJ;EACE;EACA;EACA;EACA;EACA;EACA;;AAEA;EACE;EACA;;AAMN;EACE;EACA;EACA;EACA;EACA;EACA;;AAEA;EACE;EACA;EACA;EACA;EACA;;AAEA;EACE;;AAKJ;EACE;EACA;EACA;EACA;EACA;;AAEA;EACE,OAvNa;EAwNb;;AAKJ;EACE;EACA;EACA;;AAEA;EACE;EACA;EACA;;AAKJ;EACE;;AAEA;EAHF;IAII;;;AAGF;EACE;;AAEA;EACE;EACA;;AAOJ;EADF;IAEI;;;AAGF;EACE;EACA;EACA;;AAGE;EACE;EACA;EACA;EACA;;AAEA;EACE;;;AASd;AACA;AAEA;EACE;EACA;EACA;EACA,aAxRa;EAyRb,cAzRa;EA0Rb;AAOA;AAqDA;;AA1DA;EARF;IASI;IACA;;;AAgBF;AAAA;EAEE;;AAGA;AAAA;EACE;;AAOJ;AAAA;EAEE;;AAIF;AAAA;EAEE;;AAIF;AAAA;EAEE;;AAGF;AAAA;EAEE;;AAGF;AAAA;EAEE;;AAKF;EACE;;AAGF;EACE;EACA;E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;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;EACA;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE;;AAEF;AAAA;EACE",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "../../src/sass/basic_mod.scss"
     ],
     "version": 3
 }
```

### Comparing `piccolo_theme-0.8.1/piccolo_theme/static/js/petite-vue.js` & `piccolo_theme-0.9.0/piccolo_theme/static/js/petite-vue.js`

 * *Files identical despite different names*

### Comparing `piccolo_theme-0.8.1/piccolo_theme/static/js/theme.js` & `piccolo_theme-0.9.0/piccolo_theme/static/js/theme.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -15,21 +15,21 @@
     Array(...lastParamElements).forEach((element) => {
         let brElement = document.createElement('br')
         element.after(brElement)
     })
 }
 
 function setupAutodocCpp() {
-    const highlightableElements = document.querySelectorAll(".cpp dt.sig-object")
+    const highlightableElements = document.querySelectorAll(".c dt.sig-object, .cpp dt.sig-object")
 
     Array(...highlightableElements).forEach((element) => {
         element.classList.add("highlight");
     })
 
-    const documentables = document.querySelectorAll("dt.sig-object.cpp");
+    const documentables = document.querySelectorAll("dt.sig-object.c,dt.sig-object.cpp");
 
     Array(...documentables).forEach((element) => {
         element.classList.add("highlight");
 
         var parens = element.querySelectorAll(".sig-paren");
         var commas = Array(...element.childNodes).filter(e => e.textContent == ", ")
```

### Comparing `piccolo_theme-0.8.1/piccolo_theme.egg-info/PKG-INFO` & `piccolo_theme-0.9.0/piccolo_theme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piccolo-theme
-Version: 0.8.1
+Version: 0.9.0
 Summary: A modern Sphinx theme.
 Home-page: https://github.com/piccolo-orm/piccolo_theme
 Author: Daniel Townsend
 Author-email: dan@dantownsend.co.uk
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `piccolo_theme-0.8.1/piccolo_theme.egg-info/SOURCES.txt` & `piccolo_theme-0.9.0/piccolo_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piccolo_theme-0.8.1/setup.py` & `piccolo_theme-0.9.0/setup.py`

 * *Files identical despite different names*

