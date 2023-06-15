# Comparing `tmp/backrefs-5.4.tar.gz` & `tmp/backrefs-5.5.tar.gz`

## Comparing `backrefs-5.4.tar` & `backrefs-5.5.tar`

### file list

```diff
@@ -1,70 +1,72 @@
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 backrefs-5.4/.coveragerc
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 backrefs-5.4/.pyspelling.yml
--rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 backrefs-5.4/mkdocs.yml
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 backrefs-5.4/tox.ini
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 backrefs-5.4/backrefs/__init__.py
--rw-r--r--   0        0        0     6842 2020-02-02 00:00:00.000000 backrefs-5.4/backrefs/__meta__.py
--rw-r--r--   0        0        0    52082 2020-02-02 00:00:00.000000 backrefs-5.4/backrefs/_bre_parse.py
--rw-r--r--   0        0        0    47189 2020-02-02 00:00:00.000000 backrefs-5.4/backrefs/_bregex_parse.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 backrefs-5.4/backrefs/_bregex_typing.py
--rw-r--r--   0        0        0    20079 2020-02-02 00:00:00.000000 backrefs-5.4/backrefs/bre.py
--rw-r--r--   0        0        0    21235 2020-02-02 00:00:00.000000 backrefs-5.4/backrefs/bregex.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 backrefs-5.4/backrefs/py.typed
--rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 backrefs-5.4/backrefs/util.py
--rw-r--r--   0        0        0    21040 2020-02-02 00:00:00.000000 backrefs-5.4/backrefs/uniprops/__init__.py
--rwxr-xr-x   0        0        0     1169 2020-02-02 00:00:00.000000 backrefs-5.4/docs/src/markdown/index.md
--rw-r--r--   0        0        0    20021 2020-02-02 00:00:00.000000 backrefs-5.4/docs/src/markdown/refs.md
--rwxr-xr-x   0        0        0    10241 2020-02-02 00:00:00.000000 backrefs-5.4/docs/src/markdown/usage.md
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 backrefs-5.4/docs/src/markdown/.snippets/links.md
--rw-r--r--   0        0        0    11662 2020-02-02 00:00:00.000000 backrefs-5.4/docs/src/markdown/about/changelog.md
--rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 backrefs-5.4/docs/src/markdown/about/contributing.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 backrefs-5.4/docs/src/markdown/about/license.md
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 backrefs-5.4/docs/theme/announce.html
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 backrefs-5.4/requirements/docs.txt
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 backrefs-5.4/requirements/extras.txt
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 backrefs-5.4/requirements/flake8.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 backrefs-5.4/requirements/project.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 backrefs-5.4/requirements/test.txt
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 backrefs-5.4/tests/__init__.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_age.py
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_bidiclass.py
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_bidipairedbrackettype.py
--rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_binary.py
--rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_block.py
--rw-r--r--   0        0        0    89070 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_bre.py
--rw-r--r--   0        0        0    78502 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_bregex.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_canonicalcombiningclass.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_decompositiontype.py
--rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_eastasianwidth.py
--rw-r--r--   0        0        0     5865 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_generalcategory.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_graphemeclusterbreak.py
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_hangulsyllabletype.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_indicpositionalcategory.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_indicsylabiccategory.py
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_joininggroup.py
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_joiningtype.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_linebreak.py
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_numerictype.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_numericvalue.py
--rw-r--r--   0        0        0    11215 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_quickcheck.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_script.py
--rw-r--r--   0        0        0     4409 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_scriptextensions.py
--rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_sentencebreak.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_uniprops.py
--rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_versions.py
--rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_verticalorientation.py
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 backrefs-5.4/tests/test_wordbreak.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 backrefs-5.4/tools/__init__.py
--rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 backrefs-5.4/tools/unidatadownload.py
--rw-r--r--   0        0        0    46083 2020-02-02 00:00:00.000000 backrefs-5.4/tools/unipropgen.py
--rw-r--r--   0        0        0  1025065 2020-02-02 00:00:00.000000 backrefs-5.4/tools/unicodedata/11.0.0.zip
--rw-r--r--   0        0        0  1041557 2020-02-02 00:00:00.000000 backrefs-5.4/tools/unicodedata/12.1.0.zip
--rw-r--r--   0        0        0  1086547 2020-02-02 00:00:00.000000 backrefs-5.4/tools/unicodedata/13.0.0.zip
--rw-r--r--   0        0        0  1115995 2020-02-02 00:00:00.000000 backrefs-5.4/tools/unicodedata/14.0.0.zip
--rw-r--r--   0        0        0     8944 2020-02-02 00:00:00.000000 backrefs-5.4/tools/unicodedata/LICENSE
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 backrefs-5.4/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 backrefs-5.4/LICENSE.md
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 backrefs-5.4/README.md
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 backrefs-5.4/hatch_build.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 backrefs-5.4/pyproject.toml
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 backrefs-5.4/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 backrefs-5.5/.coveragerc
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 backrefs-5.5/.pyspelling.yml
+-rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 backrefs-5.5/mkdocs.yml
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 backrefs-5.5/tox.ini
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 backrefs-5.5/backrefs/__init__.py
+-rw-r--r--   0        0        0     6842 2020-02-02 00:00:00.000000 backrefs-5.5/backrefs/__meta__.py
+-rw-r--r--   0        0        0    52712 2020-02-02 00:00:00.000000 backrefs-5.5/backrefs/_bre_parse.py
+-rw-r--r--   0        0        0    46543 2020-02-02 00:00:00.000000 backrefs-5.5/backrefs/_bregex_parse.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 backrefs-5.5/backrefs/_bregex_typing.py
+-rw-r--r--   0        0        0    19923 2020-02-02 00:00:00.000000 backrefs-5.5/backrefs/bre.py
+-rw-r--r--   0        0        0    21051 2020-02-02 00:00:00.000000 backrefs-5.5/backrefs/bregex.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 backrefs-5.5/backrefs/py.typed
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 backrefs-5.5/backrefs/util.py
+-rw-r--r--   0        0        0    21009 2020-02-02 00:00:00.000000 backrefs-5.5/backrefs/uniprops/__init__.py
+-rwxr-xr-x   0        0        0     1173 2020-02-02 00:00:00.000000 backrefs-5.5/docs/src/markdown/index.md
+-rw-r--r--   0        0        0    20335 2020-02-02 00:00:00.000000 backrefs-5.5/docs/src/markdown/refs.md
+-rwxr-xr-x   0        0        0    10252 2020-02-02 00:00:00.000000 backrefs-5.5/docs/src/markdown/usage.md
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 backrefs-5.5/docs/src/markdown/.snippets/links.md
+-rw-r--r--   0        0        0    12146 2020-02-02 00:00:00.000000 backrefs-5.5/docs/src/markdown/about/changelog.md
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 backrefs-5.5/docs/src/markdown/about/contributing.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 backrefs-5.5/docs/src/markdown/about/license.md
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 backrefs-5.5/docs/src/markdown/about/security.md
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 backrefs-5.5/docs/theme/announce.html
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 backrefs-5.5/requirements/docs.txt
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 backrefs-5.5/requirements/extras.txt
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 backrefs-5.5/requirements/flake8.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 backrefs-5.5/requirements/project.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 backrefs-5.5/requirements/test.txt
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 backrefs-5.5/tests/__init__.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_age.py
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_bidiclass.py
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_bidipairedbrackettype.py
+-rw-r--r--   0        0        0     5524 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_binary.py
+-rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_block.py
+-rw-r--r--   0        0        0    89827 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_bre.py
+-rw-r--r--   0        0        0    78561 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_bregex.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_canonicalcombiningclass.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_decompositiontype.py
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_eastasianwidth.py
+-rw-r--r--   0        0        0     5865 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_generalcategory.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_graphemeclusterbreak.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_hangulsyllabletype.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_indicpositionalcategory.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_indicsylabiccategory.py
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_joininggroup.py
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_joiningtype.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_linebreak.py
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_numerictype.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_numericvalue.py
+-rw-r--r--   0        0        0    11215 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_quickcheck.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_script.py
+-rw-r--r--   0        0        0     4409 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_scriptextensions.py
+-rw-r--r--   0        0        0     2846 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_sentencebreak.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_uniprops.py
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_versions.py
+-rw-r--r--   0        0        0     2984 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_verticalorientation.py
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 backrefs-5.5/tests/test_wordbreak.py
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 backrefs-5.5/tools/__init__.py
+-rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 backrefs-5.5/tools/unidatadownload.py
+-rw-r--r--   0        0        0    46083 2020-02-02 00:00:00.000000 backrefs-5.5/tools/unipropgen.py
+-rw-r--r--   0        0        0  1025065 2020-02-02 00:00:00.000000 backrefs-5.5/tools/unicodedata/11.0.0.zip
+-rw-r--r--   0        0        0  1041557 2020-02-02 00:00:00.000000 backrefs-5.5/tools/unicodedata/12.1.0.zip
+-rw-r--r--   0        0        0  1086547 2020-02-02 00:00:00.000000 backrefs-5.5/tools/unicodedata/13.0.0.zip
+-rw-r--r--   0        0        0  1115995 2020-02-02 00:00:00.000000 backrefs-5.5/tools/unicodedata/14.0.0.zip
+-rw-r--r--   0        0        0  1129421 2020-02-02 00:00:00.000000 backrefs-5.5/tools/unicodedata/15.0.0.zip
+-rw-r--r--   0        0        0     8944 2020-02-02 00:00:00.000000 backrefs-5.5/tools/unicodedata/LICENSE
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 backrefs-5.5/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 backrefs-5.5/LICENSE.md
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 backrefs-5.5/README.md
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 backrefs-5.5/hatch_build.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 backrefs-5.5/pyproject.toml
+-rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 backrefs-5.5/PKG-INFO
```

### Comparing `backrefs-5.4/.pyspelling.yml` & `backrefs-5.5/.pyspelling.yml`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/mkdocs.yml` & `backrefs-5.5/mkdocs.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 site_name: Backrefs Documentation
 site_url: https://facelessuser.github.io/backrefs
 repo_url: https://github.com/facelessuser/backrefs
 edit_uri: tree/master/docs/src/markdown
 site_description: A library to add additional back references to regular expressions.
 copyright: |
-  Copyright &copy; 2015 - 2022 <a href="https://github.com/facelessuser"  target="_blank" rel="noopener">Isaac Muse</a>
+  Copyright &copy; 2015 - 2023 <a href="https://github.com/facelessuser"  target="_blank" rel="noopener">Isaac Muse</a>
 
 docs_dir: docs/src/markdown
 theme:
   name: material
   custom_dir: docs/theme
   icon:
     logo: material/book-open-page-variant
@@ -16,40 +16,46 @@
     primary: deep purple
     accent: deep purple
   font:
     text: Roboto
     code: Roboto Mono
   features:
     - navigation.tabs
-    - navigation.sections
     - navigation.top
     - navigation.instant
+    - navigation.sections
+    - navigation.indexes
+    - toc.follow
+    - content.code.copy
+    - navigation.footer
+    - search.share
+    - search.highlight
+    - search.suggest
   pymdownx:
     sponsor: "https://github.com/sponsors/facelessuser"
 
 nav:
   - Getting Started:
     - Installation: index.md
     - Usage: usage.md
     - Supported References: refs.md
   - About:
     - Contributing &amp; Support: about/contributing.md
+    - Security Vulnerabilities: about/security.md
     - Changelog: about/changelog.md
     - License: about/license.md
 
 markdown_extensions:
   - markdown.extensions.toc:
       slugify: !!python/object/apply:pymdownx.slugs.slugify {kwds: {case: lower}}
       permalink: ""
-  - markdown.extensions.admonition:
   - markdown.extensions.smarty:
       smart_quotes: false
   - pymdownx.betterem:
   - markdown.extensions.attr_list:
-  - markdown.extensions.def_list:
   - markdown.extensions.tables:
   - markdown.extensions.abbr:
   - markdown.extensions.md_in_html:
   - pymdownx.superfences:
   - pymdownx.highlight:
       extend_pygments_lang:
         - name: php-inline
@@ -81,22 +87,41 @@
   - pymdownx.progressbar:
   - pymdownx.mark:
   - pymdownx.striphtml:
   - pymdownx.snippets:
       base_path:
       - docs/src/markdown/.snippets
       - LICENSE.md
+      - SECURITY.md
       auto_append:
       - links.md
   - pymdownx.keys:
       separator: "\uff0b"
-  - pymdownx.details:
-  - pymdownx.tabbed:
-      alternate_style: true
   - pymdownx.saneheaders:
+  - pymdownx.blocks.admonition:
+      types:
+      - new
+      - settings
+      - note
+      - abstract
+      - info
+      - tip
+      - success
+      - question
+      - warning
+      - failure
+      - danger
+      - bug
+      - example
+      - quote
+  - pymdownx.blocks.details:
+  - pymdownx.blocks.html:
+  - pymdownx.blocks.definition:
+  - pymdownx.blocks.tab:
+      alternate_style: True
 
 extra:
   social:
     - icon: fontawesome/brands/github
       link: https://github.com/facelessuser
     - icon: fontawesome/brands/discord
       link: https://discord.gg/TWs8Tgr
```

#### html2text {}

```diff
@@ -1,33 +1,39 @@
 site_name: Backrefs Documentation site_url: https://facelessuser.github.io/
 backrefs repo_url: https://github.com/facelessuser/backrefs edit_uri: tree/
 master/docs/src/markdown site_description: A library to add additional back
-references to regular expressions. copyright: | Copyright © 2015 - 2022 Isaac
+references to regular expressions. copyright: | Copyright © 2015 - 2023 Isaac
 Muse docs_dir: docs/src/markdown theme: name: material custom_dir: docs/theme
 icon: logo: material/book-open-page-variant palette: primary: deep purple
 accent: deep purple font: text: Roboto code: Roboto Mono features: -
-navigation.tabs - navigation.sections - navigation.top - navigation.instant
-pymdownx: sponsor: "https://github.com/sponsors/facelessuser" nav: - Getting
-Started: - Installation: index.md - Usage: usage.md - Supported References:
-refs.md - About: - Contributing & Support: about/contributing.md - Changelog:
-about/changelog.md - License: about/license.md markdown_extensions: -
-markdown.extensions.toc: slugify: !!python/object/apply:pymdownx.slugs.slugify
-{kwds: {case: lower}} permalink: "" - markdown.extensions.admonition: -
+navigation.tabs - navigation.top - navigation.instant - navigation.sections -
+navigation.indexes - toc.follow - content.code.copy - navigation.footer -
+search.share - search.highlight - search.suggest pymdownx: sponsor: "https://
+github.com/sponsors/facelessuser" nav: - Getting Started: - Installation:
+index.md - Usage: usage.md - Supported References: refs.md - About: -
+Contributing & Support: about/contributing.md - Security Vulnerabilities:
+about/security.md - Changelog: about/changelog.md - License: about/license.md
+markdown_extensions: - markdown.extensions.toc: slugify: !!python/object/apply:
+pymdownx.slugs.slugify {kwds: {case: lower}} permalink: "" -
 markdown.extensions.smarty: smart_quotes: false - pymdownx.betterem: -
-markdown.extensions.attr_list: - markdown.extensions.def_list: -
-markdown.extensions.tables: - markdown.extensions.abbr: -
-markdown.extensions.md_in_html: - pymdownx.superfences: - pymdownx.highlight:
-extend_pygments_lang: - name: php-inline lang: php options: startinline: true -
-name: pycon3 lang: pycon options: python3: true - pymdownx.inlinehilite: -
-pymdownx.magiclink: repo_url_shortener: true repo_url_shorthand: true
-social_url_shorthand: true user: facelessuser repo: backrefs - pymdownx.tilde:
-- pymdownx.caret: - pymdownx.smartsymbols: - pymdownx.emoji: emoji_index:
-!!python/name:materialx.emoji.twemoji emoji_generator: !!python/name:
-materialx.emoji.to_svg - pymdownx.escapeall: hardbreak: True nbsp: True -
-pymdownx.tasklist: custom_checkbox: true - pymdownx.progressbar: -
-pymdownx.mark: - pymdownx.striphtml: - pymdownx.snippets: base_path: - docs/
-src/markdown/.snippets - LICENSE.md auto_append: - links.md - pymdownx.keys:
-separator: "\uff0b" - pymdownx.details: - pymdownx.tabbed: alternate_style:
-true - pymdownx.saneheaders: extra: social: - icon: fontawesome/brands/github
-link: https://github.com/facelessuser - icon: fontawesome/brands/discord link:
-https://discord.gg/TWs8Tgr plugins: - search - git-revision-date-localized -
-minify: minify_html: true - mkdocs_pymdownx_material_extras
+markdown.extensions.attr_list: - markdown.extensions.tables: -
+markdown.extensions.abbr: - markdown.extensions.md_in_html: -
+pymdownx.superfences: - pymdownx.highlight: extend_pygments_lang: - name: php-
+inline lang: php options: startinline: true - name: pycon3 lang: pycon options:
+python3: true - pymdownx.inlinehilite: - pymdownx.magiclink:
+repo_url_shortener: true repo_url_shorthand: true social_url_shorthand: true
+user: facelessuser repo: backrefs - pymdownx.tilde: - pymdownx.caret: -
+pymdownx.smartsymbols: - pymdownx.emoji: emoji_index: !!python/name:
+materialx.emoji.twemoji emoji_generator: !!python/name:materialx.emoji.to_svg -
+pymdownx.escapeall: hardbreak: True nbsp: True - pymdownx.tasklist:
+custom_checkbox: true - pymdownx.progressbar: - pymdownx.mark: -
+pymdownx.striphtml: - pymdownx.snippets: base_path: - docs/src/
+markdown/.snippets - LICENSE.md - SECURITY.md auto_append: - links.md -
+pymdownx.keys: separator: "\uff0b" - pymdownx.saneheaders: -
+pymdownx.blocks.admonition: types: - new - settings - note - abstract - info -
+tip - success - question - warning - failure - danger - bug - example - quote -
+pymdownx.blocks.details: - pymdownx.blocks.html: - pymdownx.blocks.definition:
+- pymdownx.blocks.tab: alternate_style: True extra: social: - icon:
+fontawesome/brands/github link: https://github.com/facelessuser - icon:
+fontawesome/brands/discord link: https://discord.gg/TWs8Tgr plugins: - search -
+git-revision-date-localized - minify: minify_html: true -
+mkdocs_pymdownx_material_extras
```

### Comparing `backrefs-5.4/backrefs/__meta__.py` & `backrefs-5.5/backrefs/__meta__.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,9 +189,9 @@
 
     # Handle post
     post = int(m.group('post')) if m.group('post') else 0
 
     return Version(major, minor, micro, release, pre, post, dev)
 
 
-__version_info__ = Version(5, 4, 0, "final")
+__version_info__ = Version(5, 5, 0, "final")
 __version__ = __version_info__._get_canonical()
```

### Comparing `backrefs-5.4/backrefs/_bre_parse.py` & `backrefs-5.5/backrefs/_bre_parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from __future__ import annotations
 import re as _re
 import sys
 import copyreg as _copyreg
 from . import util as _util
 import unicodedata as _unicodedata
 from . import uniprops as _uniprops
-from typing import Generic, AnyStr, Optional, Match, Any, Pattern
+from typing import Generic, AnyStr, Match, Any, Pattern, cast
 
 if sys.version_info >= (3, 11):
     import re._parser as _parser  # type: ignore[import]
 else:
     import sre_parse as _parser
 
 __all__ = ("ReplaceTemplate",)
@@ -73,26 +73,26 @@
     """Search Template."""
 
     _new_refs = ("c", "C", "e", "E", "h", "l", "L", "m", "M", "N", "p", "P", "Q", "R", "X")
     _re_escape = r"\x1b"
     _re_start_wb = r"\b(?=\w)"
     _re_end_wb = r"\b(?<=\w)"
     _line_break = r'(?:\r\n|(?!\r\n)[\n\v\f\r\x85\u2028\u2029])'
-    _bytes_line_break = r'(?:\r\n|(?!\r\n)[\n\v\f\r\x85])'
+    _bytes_line_break = r'(?>\r\n|[\n\v\f\r\x85])' if _util.PY311 else r'(?:\r\n|(?!\r\n)[\n\v\f\r\x85])'
     _grapheme_cluster = r'(?:{}{}*(?!{}))'
 
     verbose: bool
     unicode: bool
     global_flag_swap: dict[str, bool]
     temp_global_flag_swap: dict[str, bool]
     ascii: bool  # noqa: A003
     is_bytes: bool
     search: AnyStr
 
-    def __init__(self, search: AnyStr, re_verbose: bool = False, re_unicode: Optional[bool] = None) -> None:
+    def __init__(self, search: AnyStr, re_verbose: bool = False, re_unicode: bool | None = None) -> None:
         """Initialize."""
 
         if isinstance(search, bytes):
             self.is_bytes = True
         else:
             self.is_bytes = False
 
@@ -284,16 +284,18 @@
         elif not in_group and t == "R":
             current.append(self._re_line_break)
         elif not in_group and t == "X":
             no_mark = self.unicode_props("^m", None, in_group=False)[0]
             mark = self.unicode_props("m", None, in_group=False)[0]
             current.extend(self._grapheme_cluster.format(no_mark, mark, mark))
         elif t == "e":
+            _util.warn_deprecated(R"The \e reference has been deprecated, please use \x1b instead")
             current.append(self._re_escape)
         elif t == "h":
+            _util.warn_deprecated(R"The \h reference has been deprecated, please use \p{Horiz_Space} instead")
             current.extend(self.unicode_props('blank', None, in_group=in_group))
             if in_group:
                 self.found_property = True
         elif t == 'p':
             prop = self.get_unicode_property(i)
             current.extend(self.unicode_props(prop[0], prop[1], in_group=in_group))
             if in_group:
@@ -308,15 +310,15 @@
             current.extend(self.unicode_name(text, in_group))
             if in_group:
                 self.found_named_unicode = True
         else:
             current.extend(["\\", t])
         return current
 
-    def get_comments(self, i: _util.StringIter) -> Optional[str]:
+    def get_comments(self, i: _util.StringIter) -> str | None:
         """Get comments."""
 
         index = i.index
         value = ['(']
         escaped = False
         try:
             c = next(i)
@@ -339,15 +341,15 @@
                 c = next(i)
             value.append(c)
         except StopIteration:
             raise SyntaxError("Unmatched '(' at {}!".format(index - 1))
 
         return ''.join(value)
 
-    def get_flags(self, i: _util.StringIter, scoped: bool = False) -> Optional[str]:
+    def get_flags(self, i: _util.StringIter, scoped: bool = False) -> str | None:
         """Get flags."""
 
         index = i.index
         value = ['(']
         toggle = False
         end = ':' if scoped else ')'
         try:
@@ -460,15 +462,15 @@
                 elif t == "[" and not found:
                     found = True
                     first = pos
                     current.append(t)
                 elif t == "[":
                     index = i.index
                     try:
-                        prop = self.get_unicode_property(i, True)  # type: Optional[tuple[str, str]]
+                        prop = self.get_unicode_property(i, True)  # type: tuple[str, str] | None
                     except Exception:
                         prop = None
                         i.rewind(i.index - index)
                     if prop is not None:
                         value = self.unicode_props(prop[0], prop[1], in_group=True)
                         if current[-1] == '-':
                             current[-1] = _re.escape('-')
@@ -542,15 +544,15 @@
             else:
                 return ['']
         return ['\\{:03o}'.format(value) if value <= 0xFF else chr(value)]
 
     def unicode_props(
         self,
         props: str,
-        prop_value: Optional[str],
+        prop_value: str | None,
         in_group: bool = False,
         negate: bool = False
     ) -> list[str]:
         """
         Insert Unicode properties.
 
         Unicode properties are very forgiving.
@@ -655,20 +657,20 @@
         """Initialize."""
 
         self.pattern = pattern  # type: Pattern[AnyStr]
         self._original = template  # type: AnyStr
         self._template = template  # type: AnyStr
         self.use_format = use_format
         self.end_found = False
-        self.group_slots = []  # type: list[tuple[int, tuple[Optional[int], Optional[int], Any]]]
+        self.group_slots = []  # type: list[tuple[int, tuple[int | None, int | None, Any]]]
         self.literal_slots = []  # type: list[str]
         self.result = []  # type: list[str]
         self.span_stack = []  # type: list[int]
         self.single_stack = []  # type: list[int]
-        self.literals = []  # type: list[Optional[AnyStr]]
+        self.literals = []  # type: list[AnyStr | None]
         self.groups = []  # type: list[tuple[int, int]]
         self.slot = 0
         self.manual = False
         self.auto = False
         self.auto_index = 0
         self.is_bytes = isinstance(self._original, bytes)
 
@@ -760,15 +762,15 @@
                     if c not in _FMT_CONV_TYPE:
                         raise SyntaxError("Invalid conversion type at {}!".format(i.index - 1))
                     value.append((_util.FMT_CONV, c))
                     c = self.format_next(i)
 
                 # Format spec
                 if c == ':':
-                    fill = None  # type: Optional[str]
+                    fill = None  # type: str | None
                     width = []
                     align = None
                     convert = None
                     c = self.format_next(i)
 
                     if c in ('<', '>', '^'):
                         # Get fill and alignment
@@ -850,15 +852,15 @@
             t = self.format_next(i)
             if t == '}':
                 self.get_single_stack()
                 self.result.append(t)
             else:
                 raise SyntaxError("Unmatched '}}' at {}!".format(i.index - 2))
 
-    def get_octal(self, c: str, i: _util.StringIter) -> Optional[str]:
+    def get_octal(self, c: str, i: _util.StringIter) -> str | None:
         """Get octal."""
 
         index = i.index
         value = []
         zero_count = 0
         try:
             if c == '0':
@@ -1052,15 +1054,15 @@
             else:
                 raise SyntaxError("Invalid group character at {}!".format(i.index - 1))
         except StopIteration:
             raise SyntaxError("Unmatched '<' at {}!".format(index))
 
         return ''.join(value)
 
-    def get_group(self, t: str, i: _util.StringIter) -> Optional[str]:
+    def get_group(self, t: str, i: _util.StringIter) -> str | None:
         """Get group number."""
 
         value = []
         try:
             if t in _DIGIT and t != '0':
                 value.append(t)
                 t = next(i)
@@ -1184,15 +1186,27 @@
         """Parse template."""
 
         if isinstance(self._original, bytes):
             self._template = self._parse_template(self._original.decode('latin-1')).encode('latin-1')
         else:
             self._template = self._parse_template(self._original)
 
-        self.groups, self.literals = _parser.parse_template(self._template, self.pattern)
+        if _util.PY312:
+            count = 0
+            for part in _parser.parse_template(self._template, self.pattern):
+                if isinstance(part, int):
+                    self.groups.append((count, part))
+                    self.literals.append(None)
+                elif part:
+                    self.literals.append(cast(AnyStr, part))
+                else:
+                    continue
+                count += 1
+        else:
+            self.groups, self.literals = _parser.parse_template(self._template, self.pattern)
 
     def span_case(self, i: _util.StringIter, case: int) -> None:
         """Uppercase or lowercase the next range of characters until end marker is found."""
 
         # A new \L, \C or \E should pop the last in the stack.
         if self.span_stack:
             self.span_stack.pop()
@@ -1258,15 +1272,15 @@
             elif self.single_stack:
                 this_case = self.get_single_stack()
                 if this_case is not None:
                     self.result.append(self.convert_case(t, this_case))
         except StopIteration:
             pass
 
-    def get_single_stack(self) -> Optional[int]:
+    def get_single_stack(self) -> int | None:
         """Get the correct single stack item to use."""
 
         single = None
         while self.single_stack:
             single = self.single_stack.pop()
         return single
 
@@ -1292,15 +1306,15 @@
             raise ValueError("Cannot switch to manual format during auto format!")
 
         self.handle_group(field, tuple(text), True)
 
     def handle_group(
         self,
         text: str,
-        capture: Optional[tuple[tuple[int, Any], ...]] = None,
+        capture: tuple[tuple[int, Any], ...] | None = None,
         is_format: bool = False
     ) -> None:
         """Handle groups."""
 
         if len(self.result) > 1:
             self.literal_slots.append("".join(self.result))
             if is_format:
@@ -1352,26 +1366,26 @@
 
 class ReplaceTemplate(_util.Immutable, Generic[AnyStr]):
     """Replacement template expander."""
 
     __slots__ = ("groups", "group_slots", "literals", "pattern_hash", "use_format", "_hash", "_bytes")
 
     groups: tuple[tuple[int, int], ...]
-    group_slots: tuple[tuple[int, tuple[Optional[int], Optional[int], Any]], ...]
-    literals: tuple[Optional[AnyStr], ...]
+    group_slots: tuple[tuple[int, tuple[int | None, int | None, Any]], ...]
+    literals: tuple[AnyStr | None, ...]
     pattern_hash: int
     use_format: bool
     _hash: int
     _bytes: bool
 
     def __init__(
         self,
         groups: tuple[tuple[int, int], ...],
-        group_slots: tuple[tuple[int, tuple[Optional[int], Optional[int], Any]], ...],
-        literals: tuple[Optional[AnyStr], ...],
+        group_slots: tuple[tuple[int, tuple[int | None, int | None, Any]], ...],
+        literals: tuple[AnyStr | None, ...],
         pattern_hash: int,
         use_format: bool,
         is_bytes: bool
     ) -> None:
         """Initialize."""
 
         super().__init__(
@@ -1386,15 +1400,15 @@
                     type(self),
                     groups, group_slots, literals,
                     pattern_hash, use_format, is_bytes
                 )
             )
         )
 
-    def __call__(self, m: Optional[Match[AnyStr]]) -> AnyStr:
+    def __call__(self, m: Match[AnyStr] | None) -> AnyStr:
         """Call."""
 
         return self.expand(m)
 
     def __hash__(self) -> int:
         """Hash."""
 
@@ -1441,25 +1455,25 @@
         g_index = 0
         for group in self.groups:
             if group[0] == index:
                 g_index = group[1]
                 break
         return g_index
 
-    def _get_group_attributes(self, index: int) -> tuple[Optional[int], Optional[int], Any]:
+    def _get_group_attributes(self, index: int) -> tuple[int | None, int | None, Any]:
         """Find and return the appropriate group case."""
 
-        g_case = (None, None, -1)  # type: tuple[Optional[int], Optional[int], Any]
+        g_case = (None, None, -1)  # type: tuple[int | None, int | None, Any]
         for group in self.group_slots:
             if group[0] == index:
                 g_case = group[1]
                 break
         return g_case
 
-    def expand(self, m: Optional[Match[AnyStr]]) -> AnyStr:
+    def expand(self, m: Match[AnyStr] | None) -> AnyStr:
         """Using the template, expand the string."""
 
         if m is None:
             raise ValueError("Match is None!")
 
         sep = m.string[:0]
         if not isinstance(sep, bytes if self._bytes else str):
```

### Comparing `backrefs-5.4/backrefs/_bregex_parse.py` & `backrefs-5.5/backrefs/_bregex_parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 from __future__ import annotations
 import unicodedata as _unicodedata
 import copyreg as _copyreg
 from . import util as _util
 import regex as _regex  # type: ignore[import]
 from regex.regex import _compile_replacement_helper  # type: ignore[import]
-from typing import Generic, AnyStr, Optional, Any, cast
+from typing import Generic, AnyStr, Any, cast
 from ._bregex_typing import Pattern, Match
 
 _ASCII_LETTERS = frozenset(
     (
         'a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm',
         'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z',
         'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M',
@@ -188,20 +188,21 @@
         """Handle references."""
 
         current = []
 
         if not in_group and t == "R":
             current.append(self._re_line_break)
         elif t == 'e':
+            _util.warn_deprecated(R"The \e reference has been deprecated, please use \x1b instead")
             current.extend(self._re_escape)
         else:
             current.extend(["\\", t])
         return current
 
-    def get_posix(self, i: _util.StringIter) -> Optional[str]:
+    def get_posix(self, i: _util.StringIter) -> str | None:
         """Get POSIX."""
 
         index = i.index
         value = ['[']
         try:
             c = next(i)
             if c != ':':
@@ -224,15 +225,15 @@
                     raise ValueError('Unmatched ]')
                 value.append(c)
         except Exception:
             i.rewind(i.index - index)
             value = []
         return ''.join(value) if value else None
 
-    def get_comments(self, i: _util.StringIter) -> Optional[str]:
+    def get_comments(self, i: _util.StringIter) -> str | None:
         """Get comments."""
 
         index = i.index
         value = ['(']
         escaped = False
         try:
             c = next(i)
@@ -255,15 +256,15 @@
                 c = next(i)
             value.append(c)
         except StopIteration:
             raise SyntaxError("Unmatched '(' at {}!".format(index - 1))
 
         return ''.join(value) if value else None
 
-    def get_flags(self, i: _util.StringIter, version0: bool, scoped: bool = False) -> Optional[str]:
+    def get_flags(self, i: _util.StringIter, version0: bool, scoped: bool = False) -> str | None:
         """Get flags."""
 
         index = i.index
         value = ['(']
         version = False
         toggle = False
         end = ':' if scoped else ')'
@@ -495,20 +496,20 @@
         """Initialize."""
 
         self.pattern = pattern  # type: Pattern[AnyStr]
         self._original = template  # type: AnyStr
         self._template = template  # type: AnyStr
         self.use_format = use_format
         self.end_found = False
-        self.group_slots = []  # type: list[tuple[int, tuple[Optional[int], Optional[int], Any]]]
+        self.group_slots = []  # type: list[tuple[int, tuple[int | None, int | None, Any]]]
         self.literal_slots = []  # type: list[str]
         self.result = []  # type: list[str]
         self.span_stack = []  # type: list[int]
         self.single_stack = []  # type: list[int]
-        self.literals = []  # type: list[Optional[AnyStr]]
+        self.literals = []  # type: list[AnyStr | None]
         self.groups = []  # type: list[tuple[int, int]]
         self.slot = 0
         self.manual = False
         self.auto = False
         self.auto_index = 0
         self.is_bytes = isinstance(self._original, bytes)
 
@@ -600,15 +601,15 @@
                     if c not in _FMT_CONV_TYPE:
                         raise SyntaxError("Invalid conversion type at {}!".format(i.index - 1))
                     value.append((_util.FMT_CONV, c))
                     c = self.format_next(i)
 
                 # Format spec
                 if c == ':':
-                    fill = None  # type: Optional[str]
+                    fill = None  # type: str | None
                     width = []
                     align = None
                     convert = None
                     c = self.format_next(i)
 
                     if c in ('<', '>', '^'):
                         # Get fill and alignment
@@ -690,15 +691,15 @@
             t = self.format_next(i)
             if t == '}':
                 self.get_single_stack()
                 self.result.append(t)
             else:
                 raise SyntaxError("Unmatched '}}' at {}!".format(i.index - 2))
 
-    def get_octal(self, c: str, i: _util.StringIter) -> Optional[str]:
+    def get_octal(self, c: str, i: _util.StringIter) -> str | None:
         """Get octal."""
 
         index = i.index
         value = []
         zero_count = 0
         try:
             if c == '0':
@@ -892,15 +893,15 @@
             else:
                 raise SyntaxError("Invalid group character at {}!".format(i.index - 1))
         except StopIteration:
             raise SyntaxError("Unmatched '<' at {}!".format(index))
 
         return ''.join(value)
 
-    def get_group(self, t: str, i: _util.StringIter) -> Optional[str]:
+    def get_group(self, t: str, i: _util.StringIter) -> str | None:
         """Get group number."""
 
         value = []
         try:
             if t in _DIGIT and t != '0':
                 value.append(t)
                 t = next(i)
@@ -983,41 +984,14 @@
         else:
             value = '\\' + t
             self.get_single_stack()
             if self.span_stack:
                 value = self.convert_case(value, self.span_stack[-1])
             self.result.append(value)
 
-    def regex_parse_template(
-        self,
-        template: AnyStr,
-        pattern: Pattern[AnyStr]
-    ) -> tuple[list[tuple[int, int]], list[Optional[AnyStr]]]:
-        """
-        Parse template for the regex module.
-
-        Do NOT edit the literal list returned by
-        _compile_replacement_helper as you will edit
-        the original cached value.  Copy the values
-        instead.
-        """
-
-        groups = []  # type: list[tuple[int, int]]
-        literals = []  # type: list[Optional[AnyStr]]
-        replacements = _compile_replacement_helper(pattern, template)  # type: list[int | AnyStr]
-        count = 0
-        for part in replacements:
-            if isinstance(part, int):
-                literals.append(None)
-                groups.append((count, part))
-            else:
-                literals.append(part)
-            count += 1
-        return groups, literals
-
     def _parse_template(self, template: str) -> str:
         """Parse template."""
 
         self.result = [""]
 
         i = _util.StringIter(template)
 
@@ -1051,15 +1025,22 @@
         """Parse template."""
 
         if isinstance(self._original, bytes):
             self._template = self._parse_template(self._original.decode('latin-1')).encode('latin-1')
         else:
             self._template = self._parse_template(self._original)
 
-        self.groups, self.literals = self.regex_parse_template(self._template, self.pattern)
+        count = 0
+        for part in _compile_replacement_helper(self.pattern, self._template):
+            if isinstance(part, int):
+                self.literals.append(None)
+                self.groups.append((count, part))
+            else:
+                self.literals.append(cast(AnyStr, part))
+            count += 1
 
     def span_case(self, i: _util.StringIter, case: int) -> None:
         """Uppercase or lowercase the next range of characters until end marker is found."""
 
         # A new \L, \C or \E should pop the last in the stack.
         if self.span_stack:
             self.span_stack.pop()
@@ -1125,15 +1106,15 @@
             else:
                 this_case = self.get_single_stack()
                 if this_case is not None:
                     self.result.append(self.convert_case(t, this_case))
         except StopIteration:
             pass
 
-    def get_single_stack(self) -> Optional[int]:
+    def get_single_stack(self) -> int | None:
         """Get the correct single stack item to use."""
 
         single = None
         while self.single_stack:
             single = self.single_stack.pop()
         return single
 
@@ -1159,15 +1140,15 @@
             raise ValueError("Cannot switch to manual format during auto format!")
 
         self.handle_group(field, tuple(text), True)
 
     def handle_group(
         self,
         text: str,
-        capture: Optional[tuple[tuple[int, Any], ...]] = None,
+        capture: tuple[tuple[int, Any], ...] | None = None,
         is_format: bool = False
     ) -> None:
         """Handle groups."""
 
         if len(self.result) > 1:
             self.literal_slots.append("".join(self.result))
             if is_format:
@@ -1219,26 +1200,26 @@
 
 class ReplaceTemplate(_util.Immutable, Generic[AnyStr]):
     """Replacement template expander."""
 
     __slots__ = ("groups", "group_slots", "literals", "pattern_hash", "use_format", "_hash", "_bytes")
 
     groups: tuple[tuple[int, int], ...]
-    group_slots: tuple[tuple[int, tuple[Optional[int], Optional[int], Any]], ...]
-    literals: tuple[Optional[AnyStr], ...]
+    group_slots: tuple[tuple[int, tuple[int | None, int | None, Any]], ...]
+    literals: tuple[AnyStr | None, ...]
     pattern_hash: int
     use_format: bool
     _hash: int
     _bytes: bool
 
     def __init__(
         self,
         groups: tuple[tuple[int, int], ...],
-        group_slots: tuple[tuple[int, tuple[Optional[int], Optional[int], Any]], ...],
-        literals: tuple[Optional[AnyStr], ...],
+        group_slots: tuple[tuple[int, tuple[int | None, int | None, Any]], ...],
+        literals: tuple[AnyStr | None, ...],
         pattern_hash: int,
         use_format: bool,
         is_bytes: bool
     ) -> None:
         """Initialize."""
 
         super().__init__(
@@ -1253,15 +1234,15 @@
                     type(self),
                     groups, group_slots, literals,
                     pattern_hash, use_format, is_bytes
                 )
             )
         )
 
-    def __call__(self, m: Optional[Match[AnyStr]]) -> AnyStr:
+    def __call__(self, m: Match[AnyStr] | None) -> AnyStr:
         """Call."""
 
         return self.expand(m)
 
     def __hash__(self) -> int:
         """Hash."""
 
@@ -1308,44 +1289,44 @@
         g_index = 0
         for group in self.groups:
             if group[0] == index:
                 g_index = group[1]
                 break
         return g_index
 
-    def _get_group_attributes(self, index: int) -> tuple[Optional[int], Optional[int], Any]:
+    def _get_group_attributes(self, index: int) -> tuple[int | None, int | None, Any]:
         """Find and return the appropriate group case."""
 
-        g_case = (None, None, -1)  # type: tuple[Optional[int], Optional[int], Any]
+        g_case = (None, None, -1)  # type: tuple[int | None, int | None, Any]
         for group in self.group_slots:
             if group[0] == index:
                 g_case = group[1]
                 break
         return g_case
 
-    def expand(self, m: Optional[Match[AnyStr]]) -> AnyStr:
+    def expand(self, m: Match[AnyStr] | None) -> AnyStr:
         """Using the template, expand the string."""
 
         if m is None:
             raise ValueError("Match is None!")
 
         sep = m.re.pattern[:0]  # type: AnyStr
         if isinstance(sep, bytes) != self._bytes:
             raise TypeError('Match string type does not match expander string type!')
         text = []
         # Expand string
         for index in range(0, len(self.literals)):
-            l = self.literals[index]  # type: Optional[AnyStr]
+            l = self.literals[index]  # type: AnyStr | None
             if l is None:
                 g_index = self._get_group_index(index)
                 span_case, single_case, capture = self._get_group_attributes(index)
                 if not self.use_format:
                     # Non format replace
                     try:
-                        l = cast(Optional[AnyStr], m.group(g_index))
+                        l = cast('AnyStr | None', m.group(g_index))
                         if l is None:
                             l = sep
                     except IndexError:  # pragma: no cover
                         raise IndexError("'{}' is out of range!".format(g_index))
                 else:
                     # String format replace
                     try:
```

### Comparing `backrefs-5.4/backrefs/bre.py` & `backrefs-5.5/backrefs/bre.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,32 +12,30 @@
  - `\l` and `\L...\E`                                            - Lowercase char or chars (replace)
  - `[:ascii:]`                                                   - Posix style classes (search)
  - `[:^ascii:]`                                                  - Inverse Posix style classes (search)
  - `\pL`, `\p{Lu}`, \p{Letter}, `\p{gc=Uppercase_Letter}`        - Unicode properties (search Unicode)
  - `\PL`, `\P{Lu}`, `\p{^Lu}`                                    - Inverse Unicode properties (search Unicode)
  - `\N{Black Club Suit}`                                         - Unicode character by name (search & replace)
  - `\u0000` and `\U00000000`                                     - Unicode characters (replace)
- - `\e`                                                          - Escape character (search)
  - `\m`                                                          - Starting word boundary (search)
  - `\M`                                                          - Ending word boundary (search)
  - `\R`                                                          - Generic line breaks (search)
- - `\h`                                                          - Horizontal whitespace (search)
  - `\X`                                                          - Simplified grapheme clusters (search)
 
 Licensed under MIT
 Copyright (c) 2011 - 2020 Isaac Muse <isaacmuse@gmail.com>
 """
 from __future__ import annotations
 import re as _re
 import copyreg as _copyreg
 from functools import lru_cache as _lru_cache
 from . import util as _util
 from . import _bre_parse
 from ._bre_parse import ReplaceTemplate
-from typing import AnyStr, Pattern, Match, Callable, Any, Optional, Generic, Mapping, Iterator, cast
+from typing import AnyStr, Pattern, Match, Callable, Any, Generic, Mapping, Iterator, cast
 
 __all__ = (
     "expand", "expandf", "search", "match", "fullmatch", "split", "findall", "finditer", "sub", "subf",
     "subn", "subfn", "purge", "escape", "fullmatch", "DEBUG", "I", "IGNORECASE", "L", "LOCALE", "M", "MULTILINE",
     "S", "DOTALL", "U", "UNICODE", "X", "VERBOSE", "compile", "compile_search", "compile_replace", "Bre",
     "ReplaceTemplate", "A", "ASCII"
 )
@@ -114,15 +112,15 @@
 def _is_replace(obj: Any) -> bool:
     """Check if object is a replace object."""
 
     return isinstance(obj, ReplaceTemplate)
 
 
 def _apply_replace_backrefs(
-    m: Optional[Match[AnyStr]],
+    m: Match[AnyStr] | None,
     repl: ReplaceTemplate[AnyStr] | AnyStr,
     flags: int = 0
 ) -> AnyStr:
     """Expand with either the `ReplaceTemplate` or compile on the fly, or return None."""
 
     if m is None:
         raise ValueError("Match is None!")
@@ -213,18 +211,18 @@
     @property
     def groupindex(self) -> Mapping[str, int]:
         """Return group index."""
 
         return self._pattern.groupindex
 
     @property
-    def groups(self) -> tuple[Optional[AnyStr], ...]:
+    def groups(self) -> tuple[AnyStr | None, ...]:
         """Return groups."""
 
-        return cast('tuple[Optional[AnyStr], ...]', self._pattern.groups)
+        return cast('tuple[AnyStr | None, ...]', self._pattern.groups)
 
     @property
     def scanner(self) -> Any:
         """Return scanner."""
 
         return self._pattern.scanner  # type: ignore[attr-defined]
 
@@ -287,35 +285,35 @@
         return compile_replace(self._pattern, repl, flags)
 
     def search(
         self,
         string: AnyStr,
         *args: Any,
         **kwargs: Any
-    ) -> Optional[Match[AnyStr]]:
+    ) -> Match[AnyStr] | None:
         """Apply `search`."""
 
         return self._pattern.search(string, *args, **kwargs)
 
     def match(
         self,
         string: AnyStr,
         *args: Any,
         **kwargs: Any
-    ) -> Optional[Match[AnyStr]]:
+    ) -> Match[AnyStr] | None:
         """Apply `match`."""
 
         return self._pattern.match(string, *args, **kwargs)
 
     def fullmatch(
         self,
         string: AnyStr,
         *args: Any,
         **kwargs: Any
-    ) -> Optional[Match[AnyStr]]:
+    ) -> Match[AnyStr] | None:
         """Apply `fullmatch`."""
 
         return self._pattern.fullmatch(string, *args, **kwargs)
 
     def split(
         self,
         string: AnyStr,
@@ -390,15 +388,15 @@
 
         return self._pattern.subn(self._auto_compile(repl, True), string, *args, **kwargs)
 
 
 def compile(  # noqa A001
     pattern: AnyStr | Pattern[AnyStr] | Bre[AnyStr],
     flags: int = 0,
-    auto_compile: Optional[bool] = None
+    auto_compile: bool | None = None
 ) -> 'Bre[AnyStr]':
     """Compile both the search or search and replace into one object."""
 
     if isinstance(pattern, Bre):
         if auto_compile is not None:
             raise ValueError("Cannot compile Bre with a different auto_compile!")
         elif flags != 0:
@@ -449,185 +447,212 @@
 def purge() -> None:
     """Purge caches."""
 
     _purge_cache()
     _re.purge()
 
 
-def expand(m: Optional[Match[AnyStr]], repl: ReplaceTemplate[AnyStr] | AnyStr) -> AnyStr:
+def expand(m: Match[AnyStr] | None, repl: ReplaceTemplate[AnyStr] | AnyStr) -> AnyStr:
     """Expand the string using the replace pattern or function."""
 
     _assert_expandable(repl)
     return _apply_replace_backrefs(m, repl)
 
 
-def expandf(m: Optional[Match[AnyStr]], repl: ReplaceTemplate[AnyStr] | AnyStr) -> AnyStr:
+def expandf(m: Match[AnyStr] | None, repl: ReplaceTemplate[AnyStr] | AnyStr) -> AnyStr:
     """Expand the string using the format replace pattern or function."""
 
     _assert_expandable(repl, True)
     return _apply_replace_backrefs(m, repl, flags=FORMAT)
 
 
 def search(
     pattern: AnyStr | Pattern[AnyStr] | Bre[AnyStr],
     string: AnyStr,
+    flags: int | _re.RegexFlag = 0,
     *args: Any,
     **kwargs: Any
-) -> Optional[Match[AnyStr]]:
+) -> Match[AnyStr] | None:
     """Apply `search` after applying backrefs."""
 
-    flags = args[2] if len(args) > 2 else kwargs.get('flags', 0)
-    return _re.search(_apply_search_backrefs(pattern, flags), string, *args, **kwargs)
+    return _re.search(_apply_search_backrefs(pattern, flags), string, flags, *args, **kwargs)
 
 
 def match(
     pattern: AnyStr | Pattern[AnyStr] | Bre[AnyStr],
     string: AnyStr,
+    flags: int | _re.RegexFlag = 0,
     *args: Any,
     **kwargs: Any
-) -> Optional[Match[AnyStr]]:
+) -> Match[AnyStr] | None:
     """Apply `match` after applying backrefs."""
 
-    flags = args[2] if len(args) > 2 else kwargs.get('flags', 0)
-    return _re.match(_apply_search_backrefs(pattern, flags), string, *args, **kwargs)
+    return _re.match(_apply_search_backrefs(pattern, flags), string, flags, *args, **kwargs)
 
 
 def fullmatch(
     pattern: AnyStr | Pattern[AnyStr] | Bre[AnyStr],
     string: AnyStr,
+    flags: int | _re.RegexFlag = 0,
     *args: Any,
     **kwargs: Any
-) -> Optional[Match[AnyStr]]:
+) -> Match[AnyStr] | None:
     """Apply `fullmatch` after applying backrefs."""
 
-    flags = args[2] if len(args) > 2 else kwargs.get('flags', 0)
-    return _re.fullmatch(_apply_search_backrefs(pattern, flags), string, *args, **kwargs)
+    return _re.fullmatch(_apply_search_backrefs(pattern, flags), string, flags, *args, **kwargs)
 
 
 def split(
     pattern: AnyStr | Pattern[AnyStr] | Bre[AnyStr],
     string: AnyStr,
+    maxsplit: int = 0,
+    flags: int | _re.RegexFlag = 0,
     *args: Any,
     **kwargs: Any
 ) -> list[AnyStr]:
     """Apply `split` after applying backrefs."""
 
-    flags = args[3] if len(args) > 3 else kwargs.get('flags', 0)
-    return _re.split(_apply_search_backrefs(pattern, flags), string, *args, **kwargs)
+    return _re.split(_apply_search_backrefs(pattern, flags), string, maxsplit, flags, *args, **kwargs)
 
 
 def findall(
     pattern: AnyStr | Pattern[AnyStr] | Bre[AnyStr],
     string: AnyStr,
+    flags: int | _re.RegexFlag = 0,
     *args: Any,
     **kwargs: Any
 ) -> list[AnyStr] | list[tuple[AnyStr, ...]]:
     """Apply `findall` after applying backrefs."""
 
-    flags = args[2] if len(args) > 2 else kwargs.get('flags', 0)
-    return _re.findall(_apply_search_backrefs(pattern, flags), string, *args, **kwargs)
+    return _re.findall(_apply_search_backrefs(pattern, flags), string, flags, *args, **kwargs)
 
 
 def finditer(
     pattern: AnyStr | Pattern[AnyStr] | Bre[AnyStr],
     string: AnyStr,
+    flags: int | _re.RegexFlag = 0,
     *args: Any,
     **kwargs: Any
 ) -> Iterator[Match[AnyStr]]:
     """Apply `finditer` after applying backrefs."""
 
-    flags = args[2] if len(args) > 2 else kwargs.get('flags', 0)
-    return _re.finditer(_apply_search_backrefs(pattern, flags), string, *args, **kwargs)
+    return _re.finditer(_apply_search_backrefs(pattern, flags), string, flags, *args, **kwargs)
 
 
 def sub(
     pattern: AnyStr | Pattern[AnyStr] | Bre[AnyStr],
     repl: AnyStr | Callable[..., AnyStr],
     string: AnyStr,
+    count: int = 0,
+    flags: int | _re.RegexFlag = 0,
     *args: Any,
     **kwargs: Any
 ) -> AnyStr:
     """Apply `sub` after applying backrefs."""
 
-    flags = args[4] if len(args) > 4 else kwargs.get('flags', 0)
     is_replace = _is_replace(repl)
     is_string = isinstance(repl, (str, bytes))
     if is_replace and cast(ReplaceTemplate[AnyStr], repl).use_format:
         raise ValueError("Compiled replace cannot be a format object!")
 
     pattern = compile_search(pattern, flags)
     return _re.sub(
-        pattern, (compile_replace(pattern, repl) if is_replace or is_string else repl), string, *args, **kwargs
+        pattern,
+        (compile_replace(pattern, repl) if is_replace or is_string else repl),
+        string,
+        count,
+        0,
+        *args,
+        **kwargs
     )
 
 
 def subf(
     pattern: AnyStr | Pattern[AnyStr] | Bre[AnyStr],
     repl: AnyStr | Callable[..., AnyStr],
     string: AnyStr,
+    count: int = 0,
+    flags: int | _re.RegexFlag = 0,
     *args: Any,
     **kwargs: Any
 ) -> AnyStr:
     """Apply `sub` with format style replace."""
 
-    flags = args[4] if len(args) > 4 else kwargs.get('flags', 0)
     is_replace = _is_replace(repl)
     is_string = isinstance(repl, (str, bytes))
     if is_replace and not cast(ReplaceTemplate[AnyStr], repl).use_format:
         raise ValueError("Compiled replace is not a format object!")
 
     pattern = compile_search(pattern, flags)
     rflags = FORMAT if is_string else 0
     return _re.sub(
-        pattern, (compile_replace(pattern, repl, flags=rflags) if is_replace or is_string else repl), string,
-        *args, **kwargs
+        pattern,
+        (compile_replace(pattern, repl, flags=rflags) if is_replace or is_string else repl),
+        string,
+        count,
+        0,
+        *args,
+        **kwargs
     )
 
 
 def subn(
     pattern: AnyStr | Pattern[AnyStr] | Bre[AnyStr],
     repl: AnyStr | Callable[..., AnyStr],
     string: AnyStr,
+    count: int = 0,
+    flags: int | _re.RegexFlag = 0,
     *args: Any,
     **kwargs: Any
 ) -> tuple[AnyStr, int]:
     """Apply `subn` with format style replace."""
 
-    flags = args[4] if len(args) > 4 else kwargs.get('flags', 0)
     is_replace = _is_replace(repl)
     is_string = isinstance(repl, (str, bytes))
     if is_replace and cast(ReplaceTemplate[AnyStr], repl).use_format:
         raise ValueError("Compiled replace cannot be a format object!")
 
     pattern = compile_search(pattern, flags)
     return _re.subn(
-        pattern, (compile_replace(pattern, repl) if is_replace or is_string else repl), string, *args, **kwargs
+        pattern,
+        (compile_replace(pattern, repl) if is_replace or is_string else repl),
+        string,
+        count,
+        0,
+        *args,
+        **kwargs
     )
 
 
 def subfn(
     pattern: AnyStr | Pattern[AnyStr] | Bre[AnyStr],
     repl: AnyStr | Callable[..., AnyStr],
     string: AnyStr,
+    count: int = 0,
+    flags: int | _re.RegexFlag = 0,
     *args: Any,
     **kwargs: Any
 ) -> tuple[AnyStr, int]:
     """Apply `subn` after applying backrefs."""
 
-    flags = args[4] if len(args) > 4 else kwargs.get('flags', 0)
     is_replace = _is_replace(repl)
     is_string = isinstance(repl, (str, bytes))
     if is_replace and not cast(ReplaceTemplate[AnyStr], repl).use_format:
         raise ValueError("Compiled replace is not a format object!")
 
     pattern = compile_search(pattern, flags)
     rflags = FORMAT if is_string else 0
     return _re.subn(
-        pattern, (compile_replace(pattern, repl, flags=rflags) if is_replace or is_string else repl), string,
-        *args, **kwargs
+        pattern,
+        (compile_replace(pattern, repl, flags=rflags) if is_replace or is_string else repl),
+        string,
+        count,
+        0,
+        *args,
+        **kwargs
     )
 
 
 def _pickle(p):  # type: ignore[no-untyped-def]
     return Bre, (p._pattern, p.auto_compile)
```

### Comparing `backrefs-5.4/backrefs/bregex.py` & `backrefs-5.5/backrefs/bregex.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,27 +5,26 @@
 
  - `\Q` and `\Q...\E`                                           - Escape/quote chars (search)
  - `\c` and `\C...\E`                                           - Uppercase char or chars (replace)
  - `\l` and `\L...\E`                                           - Lowercase char or chars (replace)
  - `\N{Black Club Suit}`                                        - Unicode character by name (replace)
  - `\u0000` and `\U00000000`                                    - Unicode characters (replace)
  - `\R`                                                         - Generic line breaks (search)
- - `\e`                                                         - Escape character (search)
 
 Licensed under MIT
 Copyright (c) 2015 - 2020 Isaac Muse <isaacmuse@gmail.com>
 """
 from __future__ import annotations
 import regex as _regex  # type: ignore[import]
 import copyreg as _copyreg
 from functools import lru_cache as _lru_cache
 from . import util as _util
 from . import _bregex_parse
 from ._bregex_parse import ReplaceTemplate
-from typing import AnyStr, Callable, Any, Optional, Generic, Mapping, Iterator, cast
+from typing import AnyStr, Callable, Any, Generic, Mapping, Iterator, cast
 from ._bregex_typing import Pattern, Match
 
 __all__ = (
     "expand", "expandf", "match", "fullmatch", "search", "sub", "subf", "subn", "subfn", "split", "splititer",
     "findall", "finditer", "purge", "escape", "D", "DEBUG", "A", "ASCII", "B", "BESTMATCH",
     "E", "ENHANCEMATCH", "F", "FULLCASE", "I", "IGNORECASE", "L", "LOCALE", "M", "MULTILINE", "R", "REVERSE",
     "S", "DOTALL", "U", "UNICODE", "X", "VERBOSE", "V0", "VERSION0", "V1", "VERSION1", "W", "WORD",
@@ -127,15 +126,15 @@
 def _is_replace(obj: Any) -> bool:
     """Check if object is a replace object."""
 
     return isinstance(obj, ReplaceTemplate)
 
 
 def _apply_replace_backrefs(
-    m: Optional[Match[AnyStr]],
+    m: Match[AnyStr] | None,
     repl: ReplaceTemplate[AnyStr] | AnyStr,
     flags: int = 0
 ) -> AnyStr:
     """Expand with either the `ReplaceTemplate` or compile on the fly, or return None."""
 
     if m is None:
         raise ValueError("Match is None!")
@@ -227,18 +226,18 @@
     @property
     def groupindex(self) -> Mapping[str, int]:
         """Return group index."""
 
         return cast(Mapping[str, int], self._pattern.groupindex)
 
     @property
-    def groups(self) -> tuple[Optional[AnyStr], ...]:
+    def groups(self) -> tuple[AnyStr | None, ...]:
         """Return groups."""
 
-        return cast('tuple[Optional[AnyStr], ...]', self._pattern.groups)
+        return cast('tuple[AnyStr | None, ...]', self._pattern.groups)
 
     @property
     def scanner(self) -> Any:
         """Return scanner."""
 
         return self._pattern.scanner
 
@@ -307,38 +306,38 @@
         return cast('Mapping[str, set[str | bytes]]', self._pattern.named_lists)
 
     def search(
         self,
         string: AnyStr,
         *args: Any,
         **kwargs: Any
-    ) -> Optional[Match[AnyStr]]:
+    ) -> Match[AnyStr] | None:
         """Apply `search`."""
 
         return self._pattern.search(string, *args, **kwargs)
 
     def match(
         self,
         string: AnyStr,
         *args: Any,
         **kwargs: Any
-    ) -> Optional[Match[AnyStr]]:
+    ) -> Match[AnyStr] | None:
         """Apply `match`."""
 
-        return cast(Optional[Match[AnyStr]], self._pattern.match(string, *args, **kwargs))
+        return cast('Match[AnyStr] | None', self._pattern.match(string, *args, **kwargs))
 
     def fullmatch(
         self,
         string: AnyStr,
         *args: Any,
         **kwargs: Any
-    ) -> Optional[Match[AnyStr]]:
+    ) -> Match[AnyStr] | None:
         """Apply `fullmatch`."""
 
-        return cast(Optional[Match[AnyStr]], self._pattern.fullmatch(string, *args, **kwargs))
+        return cast('Match[AnyStr] | None', self._pattern.fullmatch(string, *args, **kwargs))
 
     def split(
         self,
         string: AnyStr,
         *args: Any,
         **kwargs: Any
     ) -> list[AnyStr]:
@@ -420,15 +419,15 @@
 
         return cast('tuple[AnyStr, int]', self._pattern.subfn(self._auto_compile(repl, True), string, *args, **kwargs))
 
 
 def compile(  # noqa A001
     pattern: AnyStr | Pattern[AnyStr] | Bregex[AnyStr],
     flags: int = 0,
-    auto_compile: Optional[bool] = None,
+    auto_compile: bool | None = None,
     **kwargs: Any
 ) -> 'Bregex[AnyStr]':
     """Compile both the search or search and replace into one object."""
 
     if isinstance(pattern, Bregex):
         if auto_compile is not None:
             raise ValueError("Cannot compile Bregex with a different auto_compile!")
@@ -481,102 +480,107 @@
 def purge() -> None:
     """Purge caches."""
 
     _purge_cache()
     _regex.purge()
 
 
-def expand(m: Optional[Match[AnyStr]], repl: ReplaceTemplate[AnyStr] | AnyStr) -> AnyStr:
+def expand(m: Match[AnyStr] | None, repl: ReplaceTemplate[AnyStr] | AnyStr) -> AnyStr:
     """Expand the string using the replace pattern or function."""
 
     _assert_expandable(repl)
     return _apply_replace_backrefs(m, repl)
 
 
-def expandf(m: Optional[Match[AnyStr]], repl: ReplaceTemplate[AnyStr] | AnyStr) -> AnyStr:
+def expandf(m: Match[AnyStr] | None, repl: ReplaceTemplate[AnyStr] | AnyStr) -> AnyStr:
     """Expand the string using the format replace pattern or function."""
 
     _assert_expandable(repl, True)
     return _apply_replace_backrefs(m, repl, flags=FORMAT)
 
 
 def match(
     pattern: AnyStr | Pattern[AnyStr] | Bregex[AnyStr],
     string: AnyStr,
+    flags: int = 0,
     *args: Any,
     **kwargs: Any
-) -> Optional[Match[AnyStr]]:
+) -> Match[AnyStr] | None:
     """Wrapper for `match`."""
 
-    flags = args[2] if len(args) > 2 else kwargs.get('flags', 0)
     return cast(
-        Optional[Match[AnyStr]],
-        _regex.match(_apply_search_backrefs(pattern, flags), string, *args, **kwargs)
+        'Match[AnyStr] | None',
+        _regex.match(_apply_search_backrefs(pattern, flags), string, flags, *args, **kwargs)
     )
 
 
 def fullmatch(
     pattern: AnyStr | Pattern[AnyStr] | Bregex[AnyStr],
     string: AnyStr,
+    flags: int = 0,
     *args: Any,
     **kwargs: Any
-) -> Optional[Match[AnyStr]]:
+) -> Match[AnyStr] | None:
     """Wrapper for `fullmatch`."""
 
-    flags = args[2] if len(args) > 2 else kwargs.get('flags', 0)
     return cast(
-        Optional[Match[AnyStr]],
-        _regex.fullmatch(_apply_search_backrefs(pattern, flags), string, *args, **kwargs)
+        'Match[AnyStr] | None',
+        _regex.fullmatch(_apply_search_backrefs(pattern, flags), string, flags, *args, **kwargs)
     )
 
 
 def search(
     pattern: AnyStr | Pattern[AnyStr] | Bregex[AnyStr],
     string: AnyStr,
+    flags: int = 0,
     *args: Any,
     **kwargs: Any
-) -> Optional[Match[AnyStr]]:
+) -> Match[AnyStr] | None:
     """Wrapper for `search`."""
 
-    flags = args[2] if len(args) > 2 else kwargs.get('flags', 0)
     return cast(
-        Optional[Match[AnyStr]],
-        _regex.search(_apply_search_backrefs(pattern, flags), string, *args, **kwargs)
+        'Match[AnyStr] | None',
+        _regex.search(_apply_search_backrefs(pattern, flags), string, flags, *args, **kwargs)
     )
 
 
 def sub(
     pattern: AnyStr | Pattern[AnyStr] | Bregex[AnyStr],
     repl: AnyStr | Callable[..., AnyStr],
     string: AnyStr,
+    count: int = 0,
+    flags: int = 0,
     *args: Any,
     **kwargs: Any
 ) -> AnyStr:
     """Wrapper for `sub`."""
 
-    flags = args[4] if len(args) > 4 else kwargs.get('flags', 0)
     is_replace = _is_replace(repl)
     is_string = isinstance(repl, (str, bytes))
     if is_replace and cast(ReplaceTemplate[AnyStr], repl).use_format:
         raise ValueError("Compiled replace cannot be a format object!")
 
     pattern = compile_search(pattern, flags)
     return cast(
         AnyStr,
         _regex.sub(
             pattern, (compile_replace(pattern, repl) if is_replace or is_string else repl), string,
+            count,
+            0,
             *args, **kwargs
         )
     )
 
 
 def subf(
     pattern: AnyStr | Pattern[AnyStr] | Bregex[AnyStr],
     repl: AnyStr | Callable[..., AnyStr],
     string: AnyStr,
+    count: int = 0,
+    flags: int = 0,
     *args: Any,
     **kwargs: Any
 ) -> AnyStr:
     """Wrapper for `subf`."""
 
     flags = args[4] if len(args) > 4 else kwargs.get('flags', 0)
     is_replace = _is_replace(repl)
@@ -586,124 +590,135 @@
 
     pattern = compile_search(pattern, flags)
     rflags = FORMAT if is_string else 0
     return cast(
         AnyStr,
         _regex.sub(
             pattern, (compile_replace(pattern, repl, flags=rflags) if is_replace or is_string else repl), string,
+            count,
+            0,
             *args, **kwargs
         )
     )
 
 
 def subn(
     pattern: AnyStr | Pattern[AnyStr] | Bregex[AnyStr],
     repl: AnyStr | Callable[..., AnyStr],
     string: AnyStr,
+    count: int = 0,
+    flags: int = 0,
     *args: Any,
     **kwargs: Any
 ) -> tuple[AnyStr, int]:
     """Wrapper for `subn`."""
 
-    flags = args[4] if len(args) > 4 else kwargs.get('flags', 0)
     is_replace = _is_replace(repl)
     is_string = isinstance(repl, (str, bytes))
     if is_replace and cast(ReplaceTemplate[AnyStr], repl).use_format:
         raise ValueError("Compiled replace cannot be a format object!")
 
     pattern = compile_search(pattern, flags)
     return cast(
         'tuple[AnyStr, int]',
         _regex.subn(
             pattern, (compile_replace(pattern, repl) if is_replace or is_string else repl), string,
+            count,
+            0,
             *args, **kwargs
         )
     )
 
 
 def subfn(
     pattern: AnyStr | Pattern[AnyStr] | Bregex[AnyStr],
     repl: AnyStr | Callable[..., AnyStr],
     string: AnyStr,
+    count: int = 0,
+    flags: int = 0,
     *args: Any,
     **kwargs: Any
 ) -> tuple[AnyStr, int]:
     """Wrapper for `subfn`."""
 
-    flags = args[4] if len(args) > 4 else kwargs.get('flags', 0)
     is_replace = _is_replace(repl)
     is_string = isinstance(repl, (str, bytes))
     if is_replace and not cast(ReplaceTemplate[AnyStr], repl).use_format:
         raise ValueError("Compiled replace is not a format object!")
 
     pattern = compile_search(pattern, flags)
     rflags = FORMAT if is_string else 0
     return cast(
         'tuple[AnyStr, int]',
         _regex.subn(
             pattern, (compile_replace(pattern, repl, flags=rflags) if is_replace or is_string else repl), string,
+            count,
+            0,
             *args, **kwargs
         )
     )
 
 
 def split(
     pattern: AnyStr | Pattern[AnyStr] | Bregex[AnyStr],
     string: AnyStr,
+    maxsplit: int = 0,
+    flags: int = 0,
     *args: Any,
     **kwargs: Any
 ) -> list[AnyStr]:
     """Wrapper for `split`."""
 
     flags = args[3] if len(args) > 3 else kwargs.get('flags', 0)
     return cast(
         'list[AnyStr]',
-        _regex.split(_apply_search_backrefs(pattern, flags), string, *args, **kwargs)
+        _regex.split(_apply_search_backrefs(pattern, flags), string, maxsplit, flags, *args, **kwargs)
     )
 
 
 def splititer(
     pattern: AnyStr | Pattern[AnyStr] | Bregex[AnyStr],
     string: AnyStr,
+    maxsplit: int = 0,
+    flags: int = 0,
     *args: Any,
     **kwargs: Any
 ) -> Iterator[AnyStr]:
     """Wrapper for `splititer`."""
 
-    flags = args[3] if len(args) > 3 else kwargs.get('flags', 0)
     return cast(
         Iterator[AnyStr],
-        _regex.splititer(_apply_search_backrefs(pattern, flags), string, *args, **kwargs)
+        _regex.splititer(_apply_search_backrefs(pattern, flags), string, maxsplit, flags, *args, **kwargs)
     )
 
 
 def findall(
     pattern: AnyStr | Pattern[AnyStr] | Bregex[AnyStr],
     string: AnyStr,
+    flags: int = 0,
     *args: Any,
     **kwargs: Any
 ) -> list[AnyStr] | list[tuple[AnyStr, ...]]:
     """Wrapper for `findall`."""
 
-    flags = args[2] if len(args) > 2 else kwargs.get('flags', 0)
     return cast(
         'list[AnyStr] | list[tuple[AnyStr, ...]]',
-        _regex.findall(_apply_search_backrefs(pattern, flags), string, *args, **kwargs)
+        _regex.findall(_apply_search_backrefs(pattern, flags), string, flags, *args, **kwargs)
     )
 
 
 def finditer(
     pattern: AnyStr | Pattern[AnyStr] | Bregex[AnyStr],
     string: AnyStr,
+    flags: int = 0,
     *args: Any,
     **kwargs: Any
 ) -> Iterator[Match[AnyStr]]:
     """Wrapper for `finditer`."""
 
-    flags = args[2] if len(args) > 2 else kwargs.get('flags', 0)
     return cast(
         Iterator[Match[AnyStr]],
         _regex.finditer(_apply_search_backrefs(pattern, flags), string, *args, **kwargs)
     )
 
 
 def _pickle(p):  # type: ignore[no-untyped-def]
```

### Comparing `backrefs-5.4/backrefs/util.py` & `backrefs-5.5/backrefs/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 """
 from __future__ import annotations
 import warnings
 import sys
 from typing import Any, Callable, AnyStr
 
 PY311 = (3, 11) <= sys.version_info
+PY312 = (3, 12) <= sys.version_info
 
 FMT_FIELD = 0
 FMT_INDEX = 1
 FMT_ATTR = 2
 FMT_CONV = 3
 FMT_SPEC = 4
```

### Comparing `backrefs-5.4/backrefs/uniprops/__init__.py` & `backrefs-5.5/backrefs/uniprops/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Unicode Properties."""
 from __future__ import annotations
 from . import unidata
-from typing import Optional
 
 UNICODE_RANGE = '\u0000-\U0010ffff'
 ASCII_RANGE = '\x00-\xff'
 
 MODE_NORMAL = 0
 MODE_ASCII = 1
 MODE_UNICODE = 2
@@ -473,15 +472,15 @@
 
 def _is_binary(name: str) -> bool:
     """Check if name is an enum (not a binary) property."""
 
     return name in unidata.unicode_binary or name in unidata.unicode_alias['binary']
 
 
-def get_unicode_property(prop: str, value: Optional[str] = None, mode: int = MODE_UNICODE) -> str:
+def get_unicode_property(prop: str, value: str | None = None, mode: int = MODE_UNICODE) -> str:
     """Retrieve the Unicode category from the table."""
 
     if value is not None:
 
         negate = prop.startswith('^')
 
         # Normalize binary true/false input so we can handle it properly
```

### Comparing `backrefs-5.4/docs/src/markdown/index.md` & `backrefs-5.5/docs/src/markdown/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,33 +9,33 @@
 
 Backrefs comes in two flavors: `bre` (a Re wrapper) and `bregex` (a Regex wrapper).
 
 ## Installation
 
 There are a couple of recommended ways to install Backrefs.
 
-1. Install with pip:
+1.  Install with pip:
 
     ```console
     $ pip install backrefs
     ```
 
-2. Install with optional requirement `regex`:
+2.  Install with optional requirement `regex`:
 
     ```console
     $ pip install backrefs[extras]
     ```
 
-2. Install locally from source via:
+2.  Install locally from source via:
 
     ```console
     $ python setup.py build
     $ python setup.py install
     ```
 
-3. If developing Backrefs, you can install via:
+3.  If developing Backrefs, you can install via:
 
     ```console
     $ pip install --editable .
     ```
 
     This method will allow you to instantly see your changes without reinstalling which is great for developing.
```

### Comparing `backrefs-5.4/docs/src/markdown/refs.md` & `backrefs-5.5/docs/src/markdown/refs.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,81 +4,95 @@
 
 Re and Regex out of the box have very different feature sets. Backrefs tailors the supported features for each regular
 expression engine. For instance, Regex already supports Unicode properties, so Backrefs does not attempt to provide such
 support.
 
 ### Re
 
-!!! info "LOCALE and Character Properties"
-    Backrefs does not consider `LOCALE` when inserting POSIX or Unicode properties. When forced int ASCII mode, either
-    by  the `ASCII` (or `LOCALE`) flag or when operating on a byte string, Unicode properties are restricted to the
-    ASCII range.
+/// info | LOCALE and Character Properties
+Backrefs does not consider `LOCALE` when inserting POSIX or Unicode properties. When forced int ASCII mode, either
+by  the `ASCII` (or `LOCALE`) flag or when operating on a byte string, Unicode properties are restricted to the
+ASCII range.
+///
 
 Back\ References      | Description
 --------------------- |------------
-`\e`                  | Escape character `\x1b`.
+`\e`                  | **Deprecated: Use `\x1b` instead.** Escape character `\x1b`.
 `\Q...\E`             | Quotes (escapes) text for regular expression.  `\E` signifies the end of the quoting. Affects any and all characters no matter where in the regular expression pattern it is placed.
 `\p{UnicodeProperty}` | Unicode property character class. Can be used in character classes `[]`. See [Unicode Properties](#unicode-properties) for more info.
 `\pX`                 | Unicode property character class where `X` is the uppercase letter that represents the General Category property.  For instance, `\pL` would be equivalent to `\p{L}` or `\p{Letter}`.
 `\P{UnicodeProperty}` | Inverse Unicode property character class. Can be used in character classes `[]`. See [Unicode Properties](#unicode-properties) for more info.
 `\PX`                 | Inverse Unicode property character class where `X` is the uppercase letter that represents the General Category property. For instance, `\PL` would be equivalent to `\P{L}` or `\P{Letter}`.
 `[[:alnum:]]`         | Though not really a back reference, support for POSIX style character classes is available. See [POSIX Style Properties](#posix-style-properties) for more info.
 `\N{UnicodeName}`     | Named characters are are normally ignored in Re, but Backrefs adds support for them.
 `\m`                  | Start word boundary. Translates to `\b(?=\w)`.
 `\M`                  | End word boundary. Translates to `\b(?<=\w)`.
-`\h`                  | Horizontal whitespace. Equivalent to using `[[:blank:]]` or `[\t\p{Zs}]`.
+`\h`                  | **Deprecated: Use `\p{Horiz_Space}` instead.** Horizontal whitespace. Equivalent to using `[[:blank:]]` or `[\t\p{Zs}]`.
 `\R`                  | Generic line breaks. This will use the pattern `(?:\r\n|(?!\r\n)[\n\v\f\r\x85\u2028\u2029])` which is roughly equivalent the to atomic group form that other engines use: `(?>\r\n|[\n\v\f\r\x85\u2028\u2029])`. When applied to byte strings, the pattern `(?:\r\n|(?!\r\n)[\n\v\f\r\x85])` will be used.
 `\X`                  | Grapheme clusters. This will use the pattern `(?:\PM\pM*(?!\pM))` which is roughly equivalent to the atomic group form that other engines have used in the past:  `(?>\PM\pM*)`. This does not implement [full, proper grapheme clusters][grapheme-boundaries] like the 3rd party Regex module does as this would require changes to the Re core engine.
 
+/// warning | Deprecated 6.0
+`\e` and `\h` have both been deprecated in 6.0. Please migrate to using `\x1b` and `\p{Horiz_Space}` in their places
+respectively.
+///
+
 ### Regex
 
-!!! note
-    Regex already natively supports `\p{...}`, `\P{...}`, `\pX`, `\PX`, `\N{...}`, `\X`, `\h`, `\m`, and `\M` so
-    Backrefs does not attempt to add this to search patterns.
+/// note
+Regex already natively supports `\p{...}`, `\P{...}`, `\pX`, `\PX`, `\N{...}`, `\X`, `\h`, `\m`, and `\M` so
+Backrefs does not attempt to add this to search patterns.
+///
 
 Back\ References | Description
 ---------------- | -----------
-`\e`             | Escape character `\x1b`.
+`\e`             | **Deprecated: Use `\x1b` instead.** Escape character `\x1b`.
 `\Q...\E`        | Quotes (escapes) text for regular expression.  `\E` signifies the end of the quoting. Affects any and all characters no matter where in the regular expression pattern it is placed.
 `\R`             | Generic line breaks. When searching a Unicode string, this will use the pattern `(?>\r\n|[\n\v\f\r\x85\u2028\u2029])`, and when applied to byte strings, the pattern `(?>\r\n|[\n\v\f\r\x85])` will be used.
 
+/// warning | Deprecated 6.0
+`\e` has been deprecated in 6.0. Please migrate to using `\x1b` in its place.
+///
+
 ## Replace Back References
 
 The replace back references below apply to both Re **and** Regex and are essentially non-specific to the regular
 expression engine being used.  Casing is applied to both the literal text and the replacement groups within the replace
 template.  In most cases you'd only need to wrap the groups, but it may be useful to apply casing to the literal
 portions if you are dynamically assembling replacement patterns.
 
-!!! info "LOCALE and Casing"
-    `LOCALE` is not considered when applying character casing. Unicode casing is applied in Unicode strings and ASCII
-    casing is applied to byte strings.
+/// info | LOCALE and Casing
+`LOCALE` is not considered when applying character casing. Unicode casing is applied in Unicode strings and ASCII
+casing is applied to byte strings.
+///
 
 Back\ References     | Description
 ---------------------|-------------
 `\c`                 | Uppercase the next character.
 `\l`                 | Lowercase the next character.
 `\C...\E`            | Apply uppercase to all characters until either the end of the string, the end marker `\E` is found, or another `\C` or `\L` is encountered.
 `\L...\E`            | Apply lowercase to all characters until either the end of the string, the end marker `\E` is found, or another `\L` or `\C` is encountered.
 `\U`                 | Wide Unicode character `\U00000057`. Re doesn't translate this notation in raw strings (`#!py3 r"..."`), and Regex doesn't in format templates in raw strings (`#!py3 r"{} {}"`).  This adds support for them.
 `\u`                 | Narrow Unicode character `\u0057`. Re doesn't translate this notation in raw strings (`#!py3 r"..."`), and Regex doesn't in format templates in raw strings (`#!py3 r"{} {}"`).  This adds support for them.
 `\x`                 | Byte character `\x57`. Re doesn't translate this notation in raw strings (`#!py3 r"..."`), and Regex doesn't in format templates in raw strings (`#!py3 r"{} {}"`).  This adds support for them.
 `\N{UnicodeName}`    | Named characters are are normally ignored in Re, but Backrefs adds support for them.
 
-!!! tip "Tip"
-    Complex configurations of casing should work fine.
+/// tip
+Complex configurations of casing should work fine.
 
-    - `\L\cTEST\E` --> `Test`
-    - `\c\LTEST\E` --> `test`
-    - `\L\cTEST \cTEST\E` --> `Test Test`
+-   `\L\cTEST\E` --> `Test`
+-   `\c\LTEST\E` --> `test`
+-   `\L\cTEST \cTEST\E` --> `Test Test`
+///
 
 ## Unicode Properties
 
-!!! new "New in 5.0"
-    5.0 brings significant improvements and bug fixes to Unicode property handling. Properties are sensitive to the
-    `ASCII` flag along with more extensive testing and bug fixes.
+/// new | New in 5.0
+5.0 brings significant improvements and bug fixes to Unicode property handling. Properties are sensitive to the
+`ASCII` flag along with more extensive testing and bug fixes.
+///
 
 A number of various Unicode properties are supported in Backrefs, but only for Re as Regex already has its own
 implementation of Unicode properties. Some properties may not be available on certain Python versions due to the
 included Unicode build.
 
 It is important to note that Backrefs handles Unicode properties by transforming them to character classes with all the
 associated characters: `\p{Cs}` --> `[\ud800\udb7f-\udb80\udbff-\udc00\udfff]`.  Because of this, Backrefs can create
@@ -116,22 +130,24 @@
 `Numeric_Value`                             | `nv`
 `Script`                                    | `sc`
 `Script_Extensions`                         | `scx`
 `Sentence_Break`                            | `sb`
 `Vertical_Orientation`\ (Python\ 3.7+)      | `vt`
 `Word_Break`                                | `wb`
 
-!!! note
-    The Binary property is not actually a property, but more a type of Unicode property.  The available binary
-    properties may differ from Unicode version to Unicode version.
-
-!!! new "New 4.4.0"
-    Python 3.9 now uses Unicode 13, and with that comes various new binary properties: `emoji`, `emojicomponent`,
-    `emojimodifier`, `emojimodifierbase`, and `emojipresentation`. Associated aliases are also included: `ecomp`,
-    `emod`, `ebase`, and `epres`.
+/// note
+The Binary property is not actually a property, but more a type of Unicode property.  The available binary
+properties may differ from Unicode version to Unicode version.
+///
+
+/// new | New 4.4.0
+Python 3.9 now uses Unicode 13, and with that comes various new binary properties: `emoji`, `emojicomponent`,
+`emojimodifier`, `emojimodifierbase`, and `emojipresentation`. Associated aliases are also included: `ecomp`,
+`emod`, `ebase`, and `epres`.
+///
 
 Exhaustive documentation on all these properties and their values is not currently provided. In general, we'll cover the
 syntax rules, and [special short name handling](#property-short-names) to those rules for specific properties.
 Though we will outline all the values for General Category, we will not outline all of the valid values for the other
 properties. You can look at [Perl's Unicode property documentation][perl-uniprops] to get an idea of what values are
 appropriate for a given property, but keep in mind, syntax may vary from Perl's syntax.
 
@@ -156,47 +172,49 @@
 `\p{UPPERCASELETTER}`, `\p{upper case letter}`.
 
 There are a number of binary properties. In general, binary properties are specified by stating the binary property and
 a boolean value. True values can be `Yes`, `Y`, `True`, or `T`. False values can be `No`, `N`, `False`, or `F`. For
 example, to specify characters that are "alphabetic", we can use `\p{Alphabetic: Y}`. To specify characters that are
 **not** "alphabetic": `\p{Alphabetic: N}`.
 
-!!! new "New 5.4 Custom Binary properties"
-    In 5.4, the new custom binary properties `Vert_space` and `Horiz_Space` were added.
+/// new | New 5.4 Custom Binary properties
+In 5.4, the new custom binary properties `Vert_space` and `Horiz_Space` were added.
+///
 
 ### Property Short Names
 
 General Category, Script Extensions, Blocks, and Binary all can be specified in a short form using just their name or
 alias: `\p{value}`, but they will be evaluated in the following order to resolve name conflicts as some the same value
 that is used in Script may be used in Blocks etc.
 
-1. General Category
-2. Script Extensions
-4. Binary
-3. Blocks
+1.  General Category
+2.  Script Extensions
+4.  Binary
+3.  Blocks
 
 Script Extensions and Binary properties can also be defined in the format `IsValue`.  For instance, if we wanted to
 match characters in the `Latin` script, we could use the syntax `\p{IsLatin}`, which would be the same as `\p{Latin}` or
 `\p{scx: Latin}`.  For Binary properties, `\p{IsAlphabetic}` is the same as `\p{Alphabetic: Y}` or `\p{Alphabetic}`.
 
 Block properties have a similar short form as Script and Binary properties.  For Blocks you can use `InValue` to specify
 a block. If we wanted to match characters in the `Basic_Latin` block, we could use the syntax `\p{InBasic_Latin}`. This
 would be the same as `\p{Block: Basic_Latin}` or `\p{Basic_Latin}`.
 
-!!! warn "Short Name Conflicts"
-    When it comes to short names, each new Unicode version, there is a risk that new properties could cause conflicts
-    with existing names and/or aliases. Currently, most of the conflicts involve the Block properties. To reduce
-    friction, they are evaluated last.
-
-    Generally, it is discouraged to use short names for Block properties. But the option is still supported, but Block 
-    properties will be evaluated last. There are currently no known conflicts with `In*` properties, but in future
-    Unicode versions there could.
-
-    As for short names for scripts, Binary, or General Categories, there is always the possibility that these could
-    break in the future as well. Generally, more explicit is better and probably safer.
+/// warn | Short Name Conflicts
+When it comes to short names, each new Unicode version, there is a risk that new properties could cause conflicts
+with existing names and/or aliases. Currently, most of the conflicts involve the Block properties. To reduce
+friction, they are evaluated last.
+
+Generally, it is discouraged to use short names for Block properties. But the option is still supported, but Block 
+properties will be evaluated last. There are currently no known conflicts with `In*` properties, but in future
+Unicode versions there could.
+
+As for short names for scripts, Binary, or General Categories, there is always the possibility that these could
+break in the future as well. Generally, more explicit is better and probably safer.
+///
 
 Lastly, you can specify general category properties in the form `\pX` where `X` is the single letter terse property
 form. In this form, you can only use the single character values. So you could specify `Letter`, whose terse form is `L`
 with `\pL`, but cannot specify `Cased_Letter` which has a terse form of `Lc`.
 
 See the table below to see all the Unicode General Category values and their terse forms.
 
@@ -239,28 +257,29 @@
  `Separator`                       | `Z`
  `Space_Separator`                 | `Zs`
  `Line_Separator`                  | `Zl`
  `Paragraph_Separator`             | `Z`
 
 ### POSIX Style Properties
 
-!!! new "New in 5.0"
-    5.0 brings significant improvements and bug fixes to Unicode property handling. Properties are sensitive to the
-    `ASCII` flag along with more extensive testing and bug fixes. Additionally, POSIX style properties are now just
-    an extension of normal Unicode properties. All the POSIX names are available and now conform to
-    the [Unicode specification for POSIX compatibility](https://unicode.org/reports/tr18/#Compatibility_Properties).
-    Read on to learn more.
+/// new | New in 5.0
+5.0 brings significant improvements and bug fixes to Unicode property handling. Properties are sensitive to the
+`ASCII` flag along with more extensive testing and bug fixes. Additionally, POSIX style properties are now just
+an extension of normal Unicode properties. All the POSIX names are available and now conform to
+the [Unicode specification for POSIX compatibility](https://unicode.org/reports/tr18/#Compatibility_Properties).
+Read on to learn more.
+///
 
 Backrefs allows for POSIX style properties in the form `[:name:]`. These properties can only be used inside character
 classes and are another form for expressing Unicode properties. Any Unicode property that can be expressed via the
 `\p{name}` form can also be expressed in the `[:name:]` form. To illustrate, the following are all the same:
 
-- `[[:upper:]]` == `[\p{upper}]`
-- `[[:^upper:]]` == `[\p{^upper}]`
-- `[[:alpha=yes:]]` == `[\p{alpha=yes}]`
+-   `[[:upper:]]` == `[\p{upper}]`
+-   `[[:^upper:]]` == `[\p{^upper}]`
+-   `[[:alpha=yes:]]` == `[\p{alpha=yes}]`
 
 A number of POSIX property names are available via compatibility properties as outlined in the
 [Unicode specification for POSIX compatibility](https://unicode.org/reports/tr18/#Compatibility_Properties). These
 properties will operate in the Unicode range and the ASCII range depending on the regular expression mode. These
 patterns, like all Unicode properties, are sensitive to the `ASCII` flag (or `LOCALE` which will treat them as `ASCII`).
 
 It is important to note that whether used in the form `[[:name:]]` or `\p{name}`, each POSIX name is available both with
@@ -286,17 +305,18 @@
 `punct`    | `PosixPunct`  | ``[!\"\#$%&'()*+,\-./:;&lt;=&gt;?@\[\\\]^_`{}~]`` | `[[[:graph:][:blank:]]--[[:cntrl:]]]`
 `space`    | `Space`       | `[ \t\r\n\v\f]`                                   | `[\p{Whitespace}]`
 `upper`    | `Upper`       | `[A-Z]`                                           | `[\p{Uppercase}]`
 `xdigit`   | `PosixXDigit` | `[A-Fa-f0-9]`                                     | `[A-Fa-f0-9]`
 
 ### Compatibility Properties
 
-!!! new "New in 5.0"
-    While many of the properties were available before 5.0, `word` is newly available. And all the properties now
-    conform to the [Unicode specification for POSIX compatibility](https://unicode.org/reports/tr18/#Compatibility_Properties).
+/// new | New in 5.0
+While many of the properties were available before 5.0, `word` is newly available. And all the properties now
+conform to the [Unicode specification for POSIX compatibility](https://unicode.org/reports/tr18/#Compatibility_Properties).
+///
 
 [Unicode specification for POSIX compatibility][unicode-posix] defines a number of properties, many of which double as
 [Posix properties](#posix-style-properties). These properties can be accessed via `\p{name}` or `[[:name:]]`.
 
 In the table below, patterns with `--` mean `[[in this] -- [but not this]]`.
 
 \\p\{Posix}   | Unicode
```

### Comparing `backrefs-5.4/docs/src/markdown/usage.md` & `backrefs-5.5/docs/src/markdown/usage.md`

 * *Files 2% similar despite different names*

```diff
@@ -128,30 +128,30 @@
 ```
 
 ### Enhancements
 
 Backrefs' implementation is a little different than Regex's default implementation. Below we cover what is different and
 why.
 
-1. Regex's original implementation is very much like it's non-format style replacement accept for two differences: you
-  can access individual captures and you cannot use Python string back references such as specifying Unicode via
-  `\u<code>`, etc. In Backrefs, we've enhanced the syntax -- for both Re and Regex -- to allow back references to work
-  along side brace replacements. This means you can use string back references and and built-in Backrefs features like
-  `\C...\E` or `\L...\E`.
+1.  Regex's original implementation is very much like it's non-format style replacement accept for two differences: you
+    can access individual captures and you cannot use Python string back references such as specifying Unicode via
+    `\u<code>`, etc. In Backrefs, we've enhanced the syntax -- for both Re and Regex -- to allow back references to work
+    along side brace replacements. This means you can use string back references and and built-in Backrefs features like
+    `\C...\E` or `\L...\E`.
 
     ```pycon3
     >>> bre.subf(r"(\w+) (\w+)", r"{0} => \C{2} {1}\E", "foo bar")
     'foo bar => BAR FOO'
     >>> bregex.subf(r"(\w+) (\w+)", r"{0} => \C{2} {1}\E", "foo bar")
     'foo bar => BAR FOO'
     ```
 
-2. The second enhancement that Backrefs adds is the ability to use format string alignment features. In the following
-  example, we center the replacement and pad it out to 8 characters using `|` for the padding. We also use casing
-  references (`\C...\E`) to capitalize the replacement group.
+2.  The second enhancement that Backrefs adds is the ability to use format string alignment features. In the following
+    example, we center the replacement and pad it out to 8 characters using `|` for the padding. We also use casing
+    references (`\C...\E`) to capitalize the replacement group.
 
     ```pycon3
     >>> bregex.subf(r'(test)', r'\C{0:|^8}\E', 'test')
     '||TEST||'
     ```
 
     Backrefs implements a subset of the [Format Specification Mini-Language][format-spec] (`format_spec`) that allows
@@ -173,28 +173,29 @@
     format_spec ::=  [[fill]align][0][width][type]
     fill        ::=  <any character>
     align       ::=  "<" | ">" | "^"
     width       ::=  integer
     type        ::=  "s"
     ```
 
-3. Lastly, our implementation of the [Format Specification Mini-Language][format-spec] (`format_spec`) allows format
-  strings to work for byte strings as well as Unicode strings. This is something that Regex does not allow without
-  Backrefs.
+3.  Lastly, our implementation of the [Format Specification Mini-Language][format-spec] (`format_spec`) allows format
+    strings to work for byte strings as well as Unicode strings. This is something that Regex does not allow without
+    Backrefs.
 
     ```pycon3
     >>> bre.subf(br'(test)', br'\C{0:|^8}\E', b'test')
     b'||TEST||'
     ```
 
-    !!! note "Conversion Syntax and Bytes"
-        In almost all instances, using conversion types (`{!s}`, etc.) won't make sense in a regular expression replace
-        as the objects will already be strings in the needed format, but if you were to use a conversion using byte
-        strings, when converting from `bytes` to `str`, ASCII will be the assumed encoding, and the object or Unicode
-        string would be encoded using the `backslashreplace` option as well.
+    /// note | Conversion Syntax and Bytes
+    In almost all instances, using conversion types (`{!s}`, etc.) won't make sense in a regular expression replace
+    as the objects will already be strings in the needed format, but if you were to use a conversion using byte
+    strings, when converting from `bytes` to `str`, ASCII will be the assumed encoding, and the object or Unicode
+    string would be encoded using the `backslashreplace` option as well.
+    ///
 
 ## Advanced Usage
 
 As noted, Backrefs wraps the regular expression object on compile with its own object. This is so it can provide
 the replace features seamlessly without the user having to do anything extra. But if you only wanted the search
 features, the `compile_search` method can be used to compile the pattern and directly return the regular expression
 object with no wrapper:
```

### Comparing `backrefs-5.4/docs/src/markdown/.snippets/links.md` & `backrefs-5.5/docs/src/markdown/.snippets/links.md`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/docs/src/markdown/about/changelog.md` & `backrefs-5.5/docs/src/markdown/about/changelog.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,257 +1,265 @@
 # Changelog
 
+## 5.5
+
+-   **NEW**: `\e` and `\h` have both been deprecated in 6.0. Please migrate to using `\x1b` and `\p{Horiz_Space}` in
+    their respective place.
+-   **FIX**: Fix flag issue with `sub` functions.
+
 ## 5.4
 
-- **NEW**: Officially support Python 3.11.
-- **NEW**: Add to Bre compatible custom Unicode properties `\p{Vert_Space}` and `\p{Horiz_Space}` that match Regex's new
-  custom properties. This helps to expose vertical space shorthand that was not previously present.
+-   **NEW**: Officially support Python 3.11.
+-   **NEW**: Add to Bre compatible custom Unicode properties `\p{Vert_Space}` and `\p{Horiz_Space}` that match Regex's
+    new custom properties. This helps to expose vertical space shorthand that was not previously present.
 
 ## 5.3
 
-- **NEW**: Drop Python 3.6 support.
-- **NEW**: Update build backend to use Hatch.
+-   **NEW**: Drop Python 3.6 support.
+-   **NEW**: Update build backend to use Hatch.
 
 ## 5.2
 
-- **NEW**: Add type annotations.
-- **FIX**: Re format replacement captures behave more like Regex in that you can technically index into the captures of
-  a given group in Re, but in Re there is only ever one or zero captures. Documentation was never really explicit on
-  what one should expect if indexing a group in Re occurred. The documentation seemed to vaguely insinuate that it would
-  behave like a Regex capture list, just with one or zero values in the list. In reality, the value was a simple string
-  or `None`. This caused a bug in some cases where you'd have `None` inserted for a group if a group was optional, but
-  referenced in the replacement template. Now the implementation matches the description in the documentation with the
-  documentation now being more explicit about behavior.
-- **FIX**: Match Re and Regex handling when doing a non-format replacement that references a group that is present in
-  the search pattern but has no actual captures. Such a case should not fail, but simply return an empty string for the
-  group.
-- **FIX**: Format replacements that that have groups with no captures will yield an empty string as the only capture as
-  long as the user does not try to index into any captures as there are no actual captures. This behavior was a bug in
-  Regex that we duplicated and should now be fixed in the latest Regex (mrabarnett/mrab-regex#439) as well as in
-  Backrefs.
+-   **NEW**: Add type annotations.
+-   **FIX**: Re format replacement captures behave more like Regex in that you can technically index into the captures
+    of a given group in Re, but in Re there is only ever one or zero captures. Documentation was never really explicit
+    on what one should expect if indexing a group in Re occurred. The documentation seemed to vaguely insinuate that it
+    would behave like a Regex capture list, just with one or zero values in the list. In reality, the value was a simple
+    string or `None`. This caused a bug in some cases where you'd have `None` inserted for a group if a group was
+    optional, but referenced in the replacement template. Now the implementation matches the description in the
+    documentation with the documentation now being more explicit about behavior.
+-   **FIX**: Match Re and Regex handling when doing a non-format replacement that references a group that is present in
+    the search pattern but has no actual captures. Such a case should not fail, but simply return an empty string for
+    the group.
+-   **FIX**: Format replacements that that have groups with no captures will yield an empty string as the only capture
+    as long as the user does not try to index into any captures as there are no actual captures. This behavior was a bug
+    in Regex that we duplicated and should now be fixed in the latest Regex (mrabarnett/mrab-regex#439) as well as in
+    Backrefs.
 
 ## 5.1
 
-- **NEW**: Add support for Python 3.10.
+-   **NEW**: Add support for Python 3.10.
 
 ## 5.0.1
 
-- **FIX**: Fix wheel names.
+-   **FIX**: Fix wheel names.
 
 ## 5.0
 
-- **NEW**: Significant improvements to Unicode handling. A lot of testing was implemented to catch existing bugs and to
-  improve result.
-- **NEW**: POSIX style properties now handle all existing Unicode properties.
-- **NEW**: POSIX properties now follow the [Unicode specification for POSIX compatibility][unicode-posix].
-  Read the [documentation](../refs.md#posix-style-properties) to learn more.
-- **NEW**: Unicode properties are now sensitive to the `ASCII` flag and will properly restrict the range of properties
-  to the ASCII range even in Unicode strings.
-- **NEW**: Removed the old deprecated search references: `\l`, `\L`, `\c`, and `\C`. These are available in various
-  other forms: `[[:lower:]]`, `\p{lower}`, etc.
-- **NEW**: To reduce conflicts of naming, Binary properties are evaluated before Block properties when using short
-  names. Block has conflicts with some other properties of various types, using short names for blocks is discouraged.
-- **FIX**: Numerous fixes to existing Unicode properties: missing values, incorrect values, etc.
+-   **NEW**: Significant improvements to Unicode handling. A lot of testing was implemented to catch existing bugs and
+    to improve result.
+-   **NEW**: POSIX style properties now handle all existing Unicode properties.
+-   **NEW**: POSIX properties now follow the [Unicode specification for POSIX compatibility][unicode-posix].
+    Read the [documentation](../refs.md#posix-style-properties) to learn more.
+-   **NEW**: Unicode properties are now sensitive to the `ASCII` flag and will properly restrict the range of properties
+    to the ASCII range even in Unicode strings.
+-   **NEW**: Removed the old deprecated search references: `\l`, `\L`, `\c`, and `\C`. These are available in various
+    other forms: `[[:lower:]]`, `\p{lower}`, etc.
+-   **NEW**: To reduce conflicts of naming, Binary properties are evaluated before Block properties when using short
+    names. Block has conflicts with some other properties of various types, using short names for blocks is discouraged.
+-   **FIX**: Numerous fixes to existing Unicode properties: missing values, incorrect values, etc.
 
 ## 4.6
 
 - **NEW**: Provide wheels for all officially supported versions of Python.
 
 ## 4.5
 
-- **NEW**: Added new back reference `\h` to Re. To get similar functionality with Regex, users must update to the latest
-  Regex release.
+-   **NEW**: Added new back reference `\h` to Re. To get similar functionality with Regex, users must update to the
+    latest Regex release.
 
 ## 4.4
 
-- **NEW**: Added the following binary properties for Unicode 13.0 support (Python 3.9): `emoji`, `emojicomponent`,
-  `emojimodifier`, `emojimodifierbase`, and `emojipresentation`. Associated aliases are also included: `ecomp`, `emod`,
-  `ebase`, and `epres`.
+-   **NEW**: Added the following binary properties for Unicode 13.0 support (Python 3.9): `emoji`, `emojicomponent`,
+    `emojimodifier`, `emojimodifierbase`, and `emojipresentation`. Associated aliases are also included: `ecomp`,
+    `emod`, `ebase`, and `epres`.
 
 ## 4.3
 
-- **NEW**: Install Regex library along Backrefs via `pip install backrefs[extras]`.
-- **NEW**: Remove `version` and `__version__` and remove associated deprecation code.
+-   **NEW**: Install Regex library along Backrefs via `pip install backrefs[extras]`.
+-   **NEW**: Remove `version` and `__version__` and remove associated deprecation code.
 
 ## 4.2.1
 
-- **FIX**: Fix Python 3.8 installation issue due to Unicode bundle having an incorrect encoding in some files.
+-   **FIX**: Fix Python 3.8 installation issue due to Unicode bundle having an incorrect encoding in some files.
 
 ## 4.2
 
-- **NEW**: Deprecate the **search** references `\l`, `\L`, `\c`, and `\C`. The POSIX alternatives (which these were
-  shortcuts for) should be used instead: `[[:lower:]]`, `[[:^lower:]]`, `[:upper:]]`, and `[[:^upper:]]` respectively.
-- **NEW**: Formally drop support for Python 3.4.
+-   **NEW**: Deprecate the **search** references `\l`, `\L`, `\c`, and `\C`. The POSIX alternatives (which these were
+    shortcuts for) should be used instead: `[[:lower:]]`, `[[:^lower:]]`, `[:upper:]]`, and `[[:^upper:]]` respectively.
+-   **NEW**: Formally drop support for Python 3.4.
 
 ## 4.1.1
 
-- **FIX**: Later pre-release versions of Python 3.8 will support Unicode 12.1.0.
+-   **FIX**: Later pre-release versions of Python 3.8 will support Unicode 12.1.0.
 
 ## 4.1
 
-- **NEW**: Add official support for Python 3.8.
-- **NEW**: Vendor the `Pep562` library instead of requiring as a dependency.
-- **NEW**: Input parameters accept `*args` and `**kwargs` instead of specify every parameter in order to allow Backrefs
-to work even when the Re or Regex API changes. Change was made to support new Regex `timeout` parameter.
+-   **NEW**: Add official support for Python 3.8.
+-   **NEW**: Vendor the `Pep562` library instead of requiring as a dependency.
+-   **NEW**: Input parameters accept `*args` and `**kwargs` instead of specify every parameter in order to allow
+    Backrefs to work even when the Re or Regex API changes. Change was made to support new Regex `timeout` parameter.
 
 ## 4.0.2
 
-- **FIX**: Fix compatibility issues with latest Regex versions.
+-   **FIX**: Fix compatibility issues with latest Regex versions.
 
 ## 4.0.1
 
-- **FIX**: Ensure that when generating the Unicode property tables, that the property files are read in with `UTF-8`
-  encoding.
+-   **FIX**: Ensure that when generating the Unicode property tables, that the property files are read in with `UTF-8`
+    encoding.
 
 ## 4.0
 
-- **NEW**: Drop support for new features in Python 2. Python 2 support is limited to the 3.X.X series and will only
-  receive bug fixes up to 2020. All new features moving forward will be on the 4.X.X series and will be for Python 3+
-  only.
+-   **NEW**: Drop support for new features in Python 2. Python 2 support is limited to the 3.X.X series and will only
+    receive bug fixes up to 2020. All new features moving forward will be on the 4.X.X series and will be for Python 3+
+    only.
 
 ## 3.6
 
-- **NEW**: Make version available via the new, and more standard, `__version__` attribute and add the `__version_info__`
-  attribute as well. Deprecate the old `version` and `version_info` attribute for future removal.
+-   **NEW**: Make version available via the new, and more standard, `__version__` attribute and add the
+    `__version_info__` attribute as well. Deprecate the old `version` and `version_info` attribute for future removal.
 
 ## 3.5.2
 
-- **FIX**: Include zip for Unicode 11 (Python 3.7) to make installation more reliable.
+-   **FIX**: Include zip for Unicode 11 (Python 3.7) to make installation more reliable.
 
 ## 3.5.1
 
-- **FIX**: POSIX character classes should not be part of a range.
-- **FIX**: Replace string casing logic properly follows other implementations like Boost etc. `\L`, `\C`, and `\E`
-  should all terminate `\L`, and `\C`. `\l` and `\c` will be ignored if followed by `\C` or `\L`.
+-   **FIX**: POSIX character classes should not be part of a range.
+-   **FIX**: Replace string casing logic properly follows other implementations like Boost etc. `\L`, `\C`, and `\E`
+    should all terminate `\L`, and `\C`. `\l` and `\c` will be ignored if followed by `\C` or `\L`.
 
 ## 3.5
 
-- **NEW**: Use a more advanced format string implementation that implements all string features, included those found in
-  `format_spec`.
-- **FIX**: Relax validation so not to exclude valid named Unicode values.
-- **FIX**: Caching issues where byte string patterns were confused with Unicode patterns.
-- **FIX**: More protection against using conflicting string type combinations with search and replace.
+-   **NEW**: Use a more advanced format string implementation that implements all string features, included those found
+    in `format_spec`.
+-   **FIX**: Relax validation so not to exclude valid named Unicode values.
+-   **FIX**: Caching issues where byte string patterns were confused with Unicode patterns.
+-   **FIX**: More protection against using conflicting string type combinations with search and replace.
 
 ## 3.4
 
-- **NEW**: Add support for generic line breaks (`\R`) to Re.
-- **NEW**: Add support for an overly simplified form of grapheme clusters (`\X`) to Re. Roughly equivalent to
-  `(?>\PM\pM*)`.
-- **NEW**: Add support for `Vertical_Orientation` property for Unicode 10.0.0 on Python 3.7.
+-   **NEW**: Add support for generic line breaks (`\R`) to Re.
+-   **NEW**: Add support for an overly simplified form of grapheme clusters (`\X`) to Re. Roughly equivalent to
+    `(?>\PM\pM*)`.
+-   **NEW**: Add support for `Vertical_Orientation` property for Unicode 10.0.0 on Python 3.7.
 
 ## 3.3
 
-- **NEW**: Add support for `Indic_Positional_Category`\\`Indic_Matra_Category` and `Indic_Syllabic_Category` properties.
+-   **NEW**: Add support for `Indic_Positional_Category`\\`Indic_Matra_Category` and `Indic_Syllabic_Category`
+    properties.
 
 ## 3.2.1
 
-- **FIX**: `Bidi_Paired_Bracket_type` property's `None` value should be equivalent to all characters that are not `open`
-  or `close` characters.
+-   **FIX**: `Bidi_Paired_Bracket_type` property's `None` value should be equivalent to all characters that are not
+    `open` or `close` characters.
 
 ## 3.2
 
-- **NEW**: Add support for `Script_Extensions` Unicode properties (Python 3 only as Python 2, Unicode 5.2.0 does not
-  define these). Can be accessed via `\p{scripts_extensions: kana}` or `\p{scx: kana}`.
-- **NEW**: When defining scripts with just their name `\p{Kana}`, use `Script_Extensions` instead of `Scripts`. To get
-  `Scripts` results, you must specify `\p{scripts: kana}` or `\p{sc: scripts}`.
-- **NEW**: Add `Bidi_Paired_Bracket_Type` Unicode property (Python 3.4+ only).
-- **NEW**: Add support for `IsBinary` for binary properties: `\p{IsAlphabetic}` == `\p{Alphabetic: Y}`.
-- **FIX**: Tweaks/improvements to string iteration.
+-   **NEW**: Add support for `Script_Extensions` Unicode properties (Python 3 only as Python 2, Unicode 5.2.0 does not
+    define these). Can be accessed via `\p{scripts_extensions: kana}` or `\p{scx: kana}`.
+-   **NEW**: When defining scripts with just their name `\p{Kana}`, use `Script_Extensions` instead of `Scripts`. To get
+    `Scripts` results, you must specify `\p{scripts: kana}` or `\p{sc: scripts}`.
+-   **NEW**: Add `Bidi_Paired_Bracket_Type` Unicode property (Python 3.4+ only).
+-   **NEW**: Add support for `IsBinary` for binary properties: `\p{IsAlphabetic}` == `\p{Alphabetic: Y}`.
+-   **FIX**: Tweaks/improvements to string iteration.
 
 ## 3.1.2
 
-- **FIX**: Properly escape any problematic characters in Unicode tables.
+-   **FIX**: Properly escape any problematic characters in Unicode tables.
 
 ## 3.1.1
 
-- **FIX**: `bregex.compile` now supports additional keyword arguments for named lists like `bregex.compile_search` does.
+-   **FIX**: `bregex.compile` now supports additional keyword arguments for named lists like `bregex.compile_search`
+    does.
 
 ## 3.1
 
-- **NEW**: Start and end word boundary back references are now specified with `\m` and `\M` like Regex does.  `\<` and
-  `\>` have been removed from Regex.
-- **FIX**: Escaped `\<` and `\>` are no longer processed as Re is known to escape these in versions less than Python
-  3.7.
+-   **NEW**: Start and end word boundary back references are now specified with `\m` and `\M` like Regex does.  `\<` and
+    `\>` have been removed from Regex.
+-   **FIX**: Escaped `\<` and `\>` are no longer processed as Re is known to escape these in versions less than Python
+    3.7.
 
 ## 3.0.5
 
-- **FIX**: Process non raw string equivalent escaped Unicode on Python 2.7.
-- **FIX**: Compiled objects should return the pattern string, not the pattern object via the property `pattern`.
+-   **FIX**: Process non raw string equivalent escaped Unicode on Python 2.7.
+-   **FIX**: Compiled objects should return the pattern string, not the pattern object via the property `pattern`.
 
 ## 3.0.4
 
-- **FIX**: Formally enable Python 3.7 support.
-- **FIX**: Tweak to Unicode wide character handling.
+-   **FIX**: Formally enable Python 3.7 support.
+-   **FIX**: Tweak to Unicode wide character handling.
 
 ## 3.0.3
 
-- **FIX**: Compiled search and replace objects should be hashable.
-- **FIX**: Handle cases where a new compiled pattern object is passed back through compile functions.
+-   **FIX**: Compiled search and replace objects should be hashable.
+-   **FIX**: Handle cases where a new compiled pattern object is passed back through compile functions.
 
 ## 3.0.2
 
-- **FIX**: Bregex purge was calling Re's purge instead of Regex's purge.
+-   **FIX**: Bregex purge was calling Re's purge instead of Regex's purge.
 
 ## 3.0.1
 
-- **FIX**: Do not accidentally `\.` as a group in replace strings (don't use `isdigit` string method).
-- **FIX**: Group names can start with `_` in replace strings.
-- **FIX**: Do not rely on Re for parsing string.
-- **FIX**: Match behavior in `\g<group>` parsing better.
-- **FIX**: Raise some exceptions in a few places we weren't.
+-   **FIX**: Do not accidentally `\.` as a group in replace strings (don't use `isdigit` string method).
+-   **FIX**: Group names can start with `_` in replace strings.
+-   **FIX**: Do not rely on Re for parsing string.
+-   **FIX**: Match behavior in `\g<group>` parsing better.
+-   **FIX**: Raise some exceptions in a few places we weren't.
 
 ## 3.0
 
-- **NEW**: Added new `compile` function that returns a pattern object that feels like Re's and Regex's pattern object.
-- **NEW**: Add some caching of search and replace patterns.
-- **NEW**: Completely refactored algorithm for search and replace pattern augmentation.
-- **NEW**: Add support for `\e` for escape character `\x1b` in both Re and Regex.
-- **NEW**: Add support for `\R` for generic newlines in the Regex module (Regex only).
-- **NEW**: Support Unicode property form `\pP` and `\PP`.
-- **NEW**: Add support for properly handling per group, scoped verbose flags in the preprocess step (Regex).
-- **NEW**: Handle `(?#comments)` properly in the preprocess step.
-- **NEW**: Add support for `\N` in byte strings (characters out of range won't be included).
-- **NEW**: Add support for `\p` and `\P` in byte strings (characters out of range won't be included).
-- **NEW**: Add support for `\<` and `\>` word boundary escapes.
-- **FIX**: Missing block properties on narrow systems when the property starts beyond the narrow limit.
-- **FIX**: Fix issue where an invalid general category could sometimes pass and return no characters.
-- **FIX**: Fix `\Q...\E` behavior so it is applied first as a separate step. No longer avoids `\Q...\E` in things like
-  character groups or comments.
-- **FIX**: Flag related parsing issues in Regex and Re Python 3.6+.
+-   **NEW**: Added new `compile` function that returns a pattern object that feels like Re's and Regex's pattern object.
+-   **NEW**: Add some caching of search and replace patterns.
+-   **NEW**: Completely refactored algorithm for search and replace pattern augmentation.
+-   **NEW**: Add support for `\e` for escape character `\x1b` in both Re and Regex.
+-   **NEW**: Add support for `\R` for generic newlines in the Regex module (Regex only).
+-   **NEW**: Support Unicode property form `\pP` and `\PP`.
+-   **NEW**: Add support for properly handling per group, scoped verbose flags in the preprocess step (Regex).
+-   **NEW**: Handle `(?#comments)` properly in the preprocess step.
+-   **NEW**: Add support for `\N` in byte strings (characters out of range won't be included).
+-   **NEW**: Add support for `\p` and `\P` in byte strings (characters out of range won't be included).
+-   **NEW**: Add support for `\<` and `\>` word boundary escapes.
+-   **FIX**: Missing block properties on narrow systems when the property starts beyond the narrow limit.
+-   **FIX**: Fix issue where an invalid general category could sometimes pass and return no characters.
+-   **FIX**: Fix `\Q...\E` behavior so it is applied first as a separate step. No longer avoids `\Q...\E` in things like
+    character groups or comments.
+-   **FIX**: Flag related parsing issues in Regex and Re Python 3.6+.
 
 ## 2.2
 
-- **NEW**: Proper support for `\N{Unicode Name}`.
-- **FIX**: Incomplete escapes will not be passed through, but will instead throw an error. For instance `\p` should only
-  be passed through if it is complete `\p{category}`.  Python 3.7 will error on this if we pass it through, and Python
-  3.6 will generate warnings.  We should just consistently fail on it for all Python versions.
+-   **NEW**: Proper support for `\N{Unicode Name}`.
+-   **FIX**: Incomplete escapes will not be passed through, but will instead throw an error. For instance `\p` should
+    only be passed through if it is complete `\p{category}`.  Python 3.7 will error on this if we pass it through, and
+    Python 3.6 will generate warnings.  We should just consistently fail on it for all Python versions.
 
 ## 2.1
 
-- **NEW**: Handle Unicode and byte notation in Re replace templates.
-- **NEW**: Rework algorithm to handle replace casing back references in Python 3.7 development builds in preparation for
-  Python 3.7 release.
-- **NEW**: Add support for case back references when using the Regex module's `subf` and `subfn`.
-- **NEW**: Add new convenience method `expandf` to Regex that can take a format string and apply format style replaces.
-- **NEW**: Add `FORMAT` flag to `compile_replace` to apply format style replaces when applicable.
-- **NEW**: Add the same support that Regex has in relation to format style replacements to Re.
-- **NEW**: Compiled replacements are now immutable.
-- **NEW**: Various logic checking proper types and values.
-- **FIX**: Fix octal/group logic in Regex and Re.
-- **FIX**: Fix issue dealing with trailing backslashes in replace templates.
+-   **NEW**: Handle Unicode and byte notation in Re replace templates.
+-   **NEW**: Rework algorithm to handle replace casing back references in Python 3.7 development builds in preparation
+    for Python 3.7 release.
+-   **NEW**: Add support for case back references when using the Regex module's `subf` and `subfn`.
+-   **NEW**: Add new convenience method `expandf` to Regex that can take a format string and apply format style replaces.
+-   **NEW**: Add `FORMAT` flag to `compile_replace` to apply format style replaces when applicable.
+-   **NEW**: Add the same support that Regex has in relation to format style replacements to Re.
+-   **NEW**: Compiled replacements are now immutable.
+-   **NEW**: Various logic checking proper types and values.
+-   **FIX**: Fix octal/group logic in Regex and Re.
+-   **FIX**: Fix issue dealing with trailing backslashes in replace templates.
 
 ## 2.0
 
-- **NEW**: First attempt at bringing Python 3.7 support, fixing back reference logic, and adding new back reference.
-  Released and then removed due to very poor behavior.
+-   **NEW**: First attempt at bringing Python 3.7 support, fixing back reference logic, and adding new back reference.
+    Released and then removed due to very poor behavior.
 
 ## 1.0.2
 
-- **FIX**: Issues related to downloading Unicode data and Unicode table generation. Include Unicode data in release.
+-   **FIX**: Issues related to downloading Unicode data and Unicode table generation. Include Unicode data in release.
 
 ## 1.0.1
 
-- **FIX**: Fixes for Python 3.6.
+-   **FIX**: Fixes for Python 3.6.
 
 ## 1.0
 
-- **NEW**: Initial release.
+-   **NEW**: Initial release.
```

### Comparing `backrefs-5.4/docs/src/markdown/about/contributing.md` & `backrefs-5.5/docs/src/markdown/about/contributing.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 # Contributing &amp; Support
 
 ## Overview
 
 Contribution from the community is encouraged and can be done in a variety of ways:
 
-- Bug reports.
-- Reviewing code.
-- Code patches via pull requests.
-- Documentation improvements via pull requests.
-- Become a sponsor.
+-   Bug reports.
+-   Reviewing code.
+-   Code patches via pull requests.
+-   Documentation improvements via pull requests.
+-   Become a sponsor.
 
 ## Become a Sponsor :octicons-heart-fill-16:{: .heart-throb}
 
 Open source projects take time and money. Help support the project by becoming a sponsor. You can add your support at
 any tier you feel comfortable with. No amount is too little. We also accept one time contributions via PayPal.
 
 [:octicons-mark-github-16: GitHub Sponsors](https://github.com/sponsors/facelessuser){: .md-button .md-button--primary }
 [:fontawesome-brands-paypal: PayPal](https://www.paypal.me/facelessuser){ .md-button}
 
 ## Bug Reports
 
-1. Please **read the documentation** and **search the issue tracker** to try to find the answer to your question
-  **before** posting an issue.
+1.  Please **read the documentation** and **search the issue tracker** to try to find the answer to your question
+    **before** posting an issue.
 
-2. When creating an issue on the repository, please provide as much info as possible:
+2.  When creating an issue on the repository, please provide as much info as possible:
 
-    - Version being used.
-    - Operating system.
-    - Errors in console.
-    - Detailed description of the problem.
-    - Examples for reproducing the error.  You can post pictures, but if specific text or code is required to reproduce
-      the issue, please provide the text in a plain text format for easy copy/paste.
+    -   Version being used.
+    -   Operating system.
+    -   Errors in console.
+    -   Detailed description of the problem.
+    -   Examples for reproducing the error.  You can post pictures, but if specific text or code is required to
+        reproduce the issue, please provide the text in a plain text format for easy copy/paste.
 
     The more info provided the greater the chance someone will take the time to answer, implement, or fix the issue.
 
-3. Be prepared to answer questions and provide additional information if required.  Issues in which the creator refuses
-  to respond to follow up questions will be marked as stale and closed.
+3.  Be prepared to answer questions and provide additional information if required.  Issues in which the creator refuses
+    to respond to follow up questions will be marked as stale and closed.
 
 ## Reviewing Code
 
 Take part in reviewing pull requests and/or reviewing direct commits.  Make suggestions to improve the code and discuss
 solutions to overcome weakness in the algorithm.
 
 ## Pull Requests
@@ -52,21 +52,21 @@
 pull requesting.  If it is not possible to run these tests locally, they will be run when the pull request is made, but
 it is strongly suggested that requesters make an effort to verify before requesting to allow for a quick, smooth merge.
 
 Feel free to use a virtual environment if you are concerned about installing any of the Python packages.
 
 ### Running Validation Tests
 
-1. Make sure that [Tox][tox] is installed:
+1.  Make sure that [Tox][tox] is installed:
 
     ```
     pip install tox
     ```
 
-2. Run Tox:
+2.  Run Tox:
 
     ```
     tox
     ```
 
     Tox should install necessary dependencies and run the tests.
```

### Comparing `backrefs-5.4/docs/theme/announce.html` & `backrefs-5.5/docs/theme/announce.html`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_age.py` & `backrefs-5.5/tests/test_age.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_bidiclass.py` & `backrefs-5.5/tests/test_bidiclass.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_bidipairedbrackettype.py` & `backrefs-5.5/tests/test_bidipairedbrackettype.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_binary.py` & `backrefs-5.5/tests/test_binary.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_block.py` & `backrefs-5.5/tests/test_block.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_bre.py` & `backrefs-5.5/tests/test_bre.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,17 +65,17 @@
         self.assertTrue(bre.match(r'[\p{digit}-Z]', '5') is not None)
 
         self.assertTrue(bre.match(r'[0-\p{upper}]', '-') is not None)
         self.assertTrue(bre.match(r'[0-\p{upper}]', '0') is not None)
         self.assertTrue(bre.match(r'[0-\p{upper}]', 'A') is not None)
         self.assertTrue(bre.match(r'[0-\p{upper}]', 'D') is not None)
 
-        self.assertTrue(bre.match(r'[\h-Z]', 'Z') is not None)
-        self.assertTrue(bre.match(r'[\h-Z]', '\x20') is not None)
-        self.assertTrue(bre.match(r'[\h-Z]', '-') is not None)
+        self.assertTrue(bre.match(r'[\p{HorizSpace}-Z]', 'Z') is not None)
+        self.assertTrue(bre.match(r'[\p{HorizSpace}-Z]', '\x20') is not None)
+        self.assertTrue(bre.match(r'[\p{HorizSpace}-Z]', '-') is not None)
 
     def test_non_raw_string_unicode(self):
         """Test non raw string Unicode notation."""
 
         self.assertTrue(bre.compile('\\u0070\\U00000070').match('pp') is not None)
         self.assertTrue(bre.compile('\\Q\\u0070\\U00000070\\E').match('\\u0070\\U00000070') is not None)
 
@@ -134,17 +134,20 @@
         """Test inverse POSIX property."""
 
         self.assertTrue(bre.compile(r'[[:^xdigit:]]').match('i') is not None)
 
     def test_posix_property_bad_syntax(self):
         """Test that we ignore an incomplete POSIX syntax."""
 
-        self.assertTrue(bre.compile(r'[[:a]]').match('a]') is not None)
-        self.assertTrue(bre.compile(r'[[:a]').match('a') is not None)
-        self.assertTrue(bre.compile(r'[[:graph:a]').match('a') is not None)
+        with pytest.warns(FutureWarning):
+            self.assertTrue(bre.compile(r'[[:a]]').match('a]') is not None)
+        with pytest.warns(FutureWarning):
+            self.assertTrue(bre.compile(r'[[:a]').match('a') is not None)
+        with pytest.warns(FutureWarning):
+            self.assertTrue(bre.compile(r'[[:graph:a]').match('a') is not None)
 
     def test_unicode_property_failures(self):
         """Test Unicode property."""
 
         with pytest.raises(SyntaxError):
             bre.compile(r'\p')
 
@@ -234,31 +237,31 @@
         self.assertTrue(pattern.match('ÀÀAÀÀÀ') is None)
         self.assertTrue(pattern.match('ÀÀÀAÀÀ') is None)
 
     def test_comments_with_scoped_verbose(self):
         """Test scoped verbose with comments (Python 3.6+)."""
 
         pattern = bre.compile_search(
-            r'''(?u)Test # \e(?#\e)(?x:
-            Test #\e(?#\e)
-            (Test # \e
-            )Test #\e
-            )Test # \e'''
+            r'''(?u)Test # \R(?#\R)(?x:
+            Test #\R(?#\R)
+            (Test # \R
+            )Test #\R
+            )Test # \R'''
         )
 
         self.assertEqual(
             pattern.pattern,
-            r'''(?u)Test # \x1b(?#\e)(?x:
-            Test #\\e(?#\\e)
-            (Test # \\e
-            )Test #\\e
-            )Test # \x1b'''
+            r'''(?u)Test # (?:\r\n|(?!\r\n)[\n\v\f\r\x85\u2028\u2029])(?#\R)(?x:
+            Test #\\R(?#\\R)
+            (Test # \\R
+            )Test #\\R
+            )Test # (?:\r\n|(?!\r\n)[\n\v\f\r\x85\u2028\u2029])'''
         )
 
-        self.assertTrue(pattern.match('Test # \x1bTestTestTestTest # \x1b') is not None)
+        self.assertTrue(pattern.match('Test # \nTestTestTestTest # \r\n') is not None)
 
     def test_byte_string_named_chars(self):
         """Test byte string named char."""
 
         pattern = bre.compile_search(br'\N{Latin small letter a}')
         self.assertEqual(
             pattern.pattern,
@@ -293,17 +296,18 @@
             b'[\x00-\xff]'
         )
         self.assertTrue(pattern.match(b'a') is not None)
 
     def test_escape_char(self):
         """Test escape char."""
 
-        pattern = bre.compile_search(
-            r'test\etest[\e]{2}'
-        )
+        with pytest.warns(DeprecationWarning):
+            pattern = bre.compile_search(
+                r'test\etest[\e]{2}'
+            )
 
         self.assertEqual(
             pattern.pattern,
             r'test\x1btest[\x1b]{2}'
         )
 
         self.assertTrue(pattern.match('test\x1btest\x1b\x1b') is not None)
@@ -350,15 +354,16 @@
 
         pattern = bre.compile_search(r'(?x)test # \l \p{numbers}', re.UNICODE)
         self.assertEqual(pattern.pattern, r'(?x)test # \\l \\p{numbers}', re.UNICODE)
 
     def test_char_group_nested_opening(self):
         """Test char group with nested opening [."""
 
-        pattern = bre.compile_search(r'test [[] \N{black club suit}', re.UNICODE)
+        with pytest.warns(FutureWarning):
+            pattern = bre.compile_search(r'test [[] \N{black club suit}', re.UNICODE)
         self.assertEqual(pattern.pattern, 'test [[] \u2663', re.UNICODE)
 
     def test_inline_comments(self):
         """Test that we properly find inline comments and avoid them."""
         pattern = bre.compile_search(r'test(?#\l\p{^IsLatin})', re.UNICODE)
         m = pattern.match('test')
         self.assertEqual(pattern.pattern, r'test(?#\l\p{^IsLatin})')
@@ -1055,42 +1060,46 @@
 
         with pytest.raises(_constants.error):
             bre.sub(r"[\R]", 'l', 'Rine\r\nRine\nRine\r')
 
     def test_horizontal_ws(self):
         """Test horizontal whitespace."""
 
-        self.assertEqual(
-            bre.sub(r'\h*', '', '    \t\ttest    \t'),
-            'test'
-        )
+        with pytest.warns(DeprecationWarning):
+            self.assertEqual(
+                bre.sub(r'\h*', '', '    \t\ttest    \t'),
+                'test'
+            )
 
     def test_horizontal_ws_in_group(self):
         """Test horizontal whitespace."""
 
-        self.assertEqual(
-            bre.sub(r'[\ht]*', '', '    \t\ttest    \t'),
-            'es'
-        )
+        with pytest.warns(DeprecationWarning):
+            self.assertEqual(
+                bre.sub(r'[\ht]*', '', '    \t\ttest    \t'),
+                'es'
+            )
 
     def test_horizontal_ws_in_inverse_group(self):
         """Test horizontal whitespace."""
 
-        self.assertEqual(
-            bre.sub(r'[^\ht]*', '', '    \t\ttest    \t'),
-            '    \t\ttt    \t'
-        )
+        with pytest.warns(DeprecationWarning):
+            self.assertEqual(
+                bre.sub(r'[^\ht]*', '', '    \t\ttest    \t'),
+                '    \t\ttt    \t'
+            )
 
     def test_horizontal_ws_bytes(self):
         """Test horizontal whitespace as byte string."""
 
-        self.assertEqual(
-            bre.sub(br'\h*', b'', b'    \t\ttest    \t'),
-            b'test'
-        )
+        with pytest.warns(DeprecationWarning):
+            self.assertEqual(
+                bre.sub(br'\h*', b'', b'    \t\ttest    \t'),
+                b'test'
+            )
 
     def test_grapheme_cluster(self):
         """Test simple grapheme cluster."""
 
         self.assertEqual(
             bre.compile(r'\X').pattern,
             bre.compile(r'(?:\PM\pM*(?!\pM))').pattern
@@ -2289,21 +2298,24 @@
         m = bre.match(r'This is a test for m[[:lower:t:]]+!', "This is a test for match!")
         self.assertTrue(m is not None)
 
     def test_incomplete_posix_value(self):
         """Test incomplete POSIX value."""
 
         with pytest.raises(re.error):
-            bre.match(r'This is a test for m[[:lower=t', "This is a test for m[[:lower=t")
+            with pytest.warns(FutureWarning):
+                bre.match(r'This is a test for m[[:lower=t', "This is a test for m[[:lower=t")
 
         with pytest.raises(re.error):
-            bre.match(r'This is a test for m[[:lower=t:', "This is a test for m[[:lower=t:")
+            with pytest.warns(FutureWarning):
+                bre.match(r'This is a test for m[[:lower=t:', "This is a test for m[[:lower=t:")
 
         with pytest.raises(re.error):
-            bre.match(r'This is a test for m[[:lower=t: ', "This is a test for m[[:lower=t: ")
+            with pytest.warns(FutureWarning):
+                bre.match(r'This is a test for m[[:lower=t: ', "This is a test for m[[:lower=t: ")
 
     def test_fullmatch(self):
         """Test that `fullmatch` works."""
 
         m = bre.fullmatch(r'This is a test for match!', "This is a test for match!")
         self.assertTrue(m is not None)
```

### Comparing `backrefs-5.4/tests/test_bregex.py` & `backrefs-5.5/tests/test_bregex.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,17 +143,18 @@
 
         with pytest.raises(_bregex_parse.LoopException):
             bregex.compile_search(r'(?V1)(?V0)')
 
     def test_escape_char(self):
         """Test escape char."""
 
-        pattern = bregex.compile_search(
-            r'test\etest[\e]{2}'
-        )
+        with pytest.warns(DeprecationWarning):
+            pattern = bregex.compile_search(
+                r'test\etest[\e]{2}'
+            )
 
         self.assertEqual(
             pattern.pattern,
             r'test\x1btest[\x1b]{2}'
         )
 
         self.assertTrue(pattern.match('test\x1btest\x1b\x1b') is not None)
```

### Comparing `backrefs-5.4/tests/test_canonicalcombiningclass.py` & `backrefs-5.5/tests/test_canonicalcombiningclass.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_decompositiontype.py` & `backrefs-5.5/tests/test_decompositiontype.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_eastasianwidth.py` & `backrefs-5.5/tests/test_eastasianwidth.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_generalcategory.py` & `backrefs-5.5/tests/test_generalcategory.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_graphemeclusterbreak.py` & `backrefs-5.5/tests/test_graphemeclusterbreak.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_hangulsyllabletype.py` & `backrefs-5.5/tests/test_hangulsyllabletype.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_indicpositionalcategory.py` & `backrefs-5.5/tests/test_indicpositionalcategory.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_indicsylabiccategory.py` & `backrefs-5.5/tests/test_indicsylabiccategory.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_joininggroup.py` & `backrefs-5.5/tests/test_joininggroup.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_joiningtype.py` & `backrefs-5.5/tests/test_joiningtype.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_linebreak.py` & `backrefs-5.5/tests/test_linebreak.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_numerictype.py` & `backrefs-5.5/tests/test_numerictype.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_numericvalue.py` & `backrefs-5.5/tests/test_numericvalue.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_quickcheck.py` & `backrefs-5.5/tests/test_quickcheck.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_script.py` & `backrefs-5.5/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_scriptextensions.py` & `backrefs-5.5/tests/test_scriptextensions.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_sentencebreak.py` & `backrefs-5.5/tests/test_sentencebreak.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_uniprops.py` & `backrefs-5.5/tests/test_uniprops.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_versions.py` & `backrefs-5.5/tests/test_versions.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_verticalorientation.py` & `backrefs-5.5/tests/test_verticalorientation.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tests/test_wordbreak.py` & `backrefs-5.5/tests/test_wordbreak.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tools/unidatadownload.py` & `backrefs-5.5/tools/unidatadownload.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tools/unipropgen.py` & `backrefs-5.5/tools/unipropgen.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tools/unicodedata/11.0.0.zip` & `backrefs-5.5/tools/unicodedata/11.0.0.zip`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tools/unicodedata/12.1.0.zip` & `backrefs-5.5/tools/unicodedata/12.1.0.zip`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tools/unicodedata/13.0.0.zip` & `backrefs-5.5/tools/unicodedata/13.0.0.zip`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tools/unicodedata/14.0.0.zip` & `backrefs-5.5/tools/unicodedata/14.0.0.zip`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/tools/unicodedata/LICENSE` & `backrefs-5.5/tools/unicodedata/LICENSE`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/.gitignore` & `backrefs-5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/LICENSE.md` & `backrefs-5.5/LICENSE.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2015 - 2022 Isaac Muse
+Copyright (c) 2015 - 2023 Isaac Muse
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `backrefs-5.4/hatch_build.py` & `backrefs-5.5/hatch_build.py`

 * *Files identical despite different names*

### Comparing `backrefs-5.4/pyproject.toml` & `backrefs-5.5/pyproject.toml`

 * *Files identical despite different names*

