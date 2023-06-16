# Comparing `tmp/pycoparsec-0.0.1.tar.gz` & `tmp/pycoparsec-0.0.2.tar.gz`

## Comparing `pycoparsec-0.0.1.tar` & `pycoparsec-0.0.2.tar`

### file list

```diff
@@ -1,69 +1,66 @@
--rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/.pyproject.toml.~undo-tree~
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/Makefile
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/conf.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/make.bat
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/modules.rst
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/pycoparsec.rst
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/.buildinfo
--rw-r--r--   0        0        0     5788 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/genindex.html
--rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/index.html
--rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/modules.html
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/objects.inv
--rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/py-modindex.html
--rw-r--r--   0        0        0    17184 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/pycoparsec.html
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/search.html
--rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/searchindex.js
--rw-r--r--   0        0        0    79334 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/.doctrees/environment.pickle
--rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/.doctrees/index.doctree
--rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/.doctrees/modules.doctree
--rw-r--r--   0        0        0    36742 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/.doctrees/pycoparsec.doctree
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/_modules/index.html
--rw-r--r--   0        0        0    19926 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/_modules/pycoparsec/parser.html
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/_sources/index.rst.txt
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/_sources/modules.rst.txt
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/_sources/pycoparsec.rst.txt
--rw-r--r--   0        0        0    11230 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/_static/alabaster.css
--rw-r--r--   0        0        0    14813 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/_static/basic.css
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/_static/custom.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/_static/doctools.js
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/_static/file.png
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/_static/plus.png
--rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/_static/pygments.css
--rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/_static/sphinx_highlight.js
--rw-r--r--   0        0        0    17499 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/doctrees/environment.pickle
--rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/doctrees/index.doctree
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/html/.buildinfo
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/html/genindex.html
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/html/index.html
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/html/objects.inv
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/html/search.html
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/html/searchindex.js
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0        0        0    11230 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/html/_static/alabaster.css
--rw-r--r--   0        0        0    14813 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/html/_static/basic.css
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/html/_static/custom.css
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/html/_static/doctools.js
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/html/_static/file.png
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/html/_static/language_data.js
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/html/_static/minus.png
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/html/_static/plus.png
--rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/html/_static/pygments.css
--rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/html/_static/searchtools.js
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/src/pycoparsec/.__about__.py.~undo-tree~
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/src/pycoparsec/.__init__.py.~undo-tree~
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/src/pycoparsec/__about__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/src/pycoparsec/__init__.py
--rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/src/pycoparsec/parser.py
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/tests/.__init__.py.~undo-tree~
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     7440 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/README.md
--rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5286 2020-02-02 00:00:00.000000 pycoparsec-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/Makefile
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/conf.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/make.bat
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/modules.rst
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/pycoparsec.rst
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/.buildinfo
+-rw-r--r--   0        0        0     5788 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/genindex.html
+-rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/index.html
+-rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/modules.html
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/objects.inv
+-rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/py-modindex.html
+-rw-r--r--   0        0        0    17184 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/pycoparsec.html
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/search.html
+-rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/searchindex.js
+-rw-r--r--   0        0        0    79334 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/.doctrees/environment.pickle
+-rw-r--r--   0        0        0     4973 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/.doctrees/index.doctree
+-rw-r--r--   0        0        0     2700 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/.doctrees/modules.doctree
+-rw-r--r--   0        0        0    36742 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/.doctrees/pycoparsec.doctree
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/_modules/index.html
+-rw-r--r--   0        0        0    19926 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/_modules/pycoparsec/parser.html
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/_sources/index.rst.txt
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/_sources/modules.rst.txt
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/_sources/pycoparsec.rst.txt
+-rw-r--r--   0        0        0    11230 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/_static/alabaster.css
+-rw-r--r--   0        0        0    14813 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/_static/basic.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/_static/doctools.js
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/_static/file.png
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/_static/plus.png
+-rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0    17499 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0        0        0     4953 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/doctrees/index.doctree
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/html/.buildinfo
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/html/genindex.html
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/html/index.html
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/html/objects.inv
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/html/search.html
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/html/searchindex.js
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0        0        0    11230 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0        0        0    14813 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/html/_static/basic.css
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/html/_static/custom.css
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/html/_static/doctools.js
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/html/_static/file.png
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/html/_static/language_data.js
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/html/_static/minus.png
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/html/_static/plus.png
+-rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/html/_static/pygments.css
+-rw-r--r--   0        0        0    18215 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/src/pycoparsec/__about__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/src/pycoparsec/__init__.py
+-rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/src/pycoparsec/parser.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/.gitignore
+-rw-r--r--   0        0        0     7440 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/README.md
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5372 2020-02-02 00:00:00.000000 pycoparsec-0.0.2/PKG-INFO
```

### Comparing `pycoparsec-0.0.1/docs/Makefile` & `pycoparsec-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/conf.py` & `pycoparsec-0.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/make.bat` & `pycoparsec-0.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/genindex.html` & `pycoparsec-0.0.2/docs/_build/genindex.html`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/index.html` & `pycoparsec-0.0.2/docs/_build/index.html`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/modules.html` & `pycoparsec-0.0.2/docs/_build/modules.html`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/py-modindex.html` & `pycoparsec-0.0.2/docs/_build/py-modindex.html`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/pycoparsec.html` & `pycoparsec-0.0.2/docs/_build/pycoparsec.html`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/search.html` & `pycoparsec-0.0.2/docs/_build/search.html`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/searchindex.js` & `pycoparsec-0.0.2/docs/_build/searchindex.js`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/.doctrees/environment.pickle` & `pycoparsec-0.0.2/docs/_build/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/.doctrees/index.doctree` & `pycoparsec-0.0.2/docs/_build/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/.doctrees/modules.doctree` & `pycoparsec-0.0.2/docs/_build/.doctrees/modules.doctree`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/.doctrees/pycoparsec.doctree` & `pycoparsec-0.0.2/docs/_build/.doctrees/pycoparsec.doctree`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/_modules/index.html` & `pycoparsec-0.0.2/docs/_build/_modules/index.html`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/_modules/pycoparsec/parser.html` & `pycoparsec-0.0.2/docs/_build/_modules/pycoparsec/parser.html`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/_static/alabaster.css` & `pycoparsec-0.0.2/docs/_build/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/_static/basic.css` & `pycoparsec-0.0.2/docs/_build/_static/basic.css`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/_static/doctools.js` & `pycoparsec-0.0.2/docs/_build/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/_static/language_data.js` & `pycoparsec-0.0.2/docs/_build/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/_static/pygments.css` & `pycoparsec-0.0.2/docs/_build/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/_static/searchtools.js` & `pycoparsec-0.0.2/docs/_build/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/_static/sphinx_highlight.js` & `pycoparsec-0.0.2/docs/_build/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/doctrees/environment.pickle` & `pycoparsec-0.0.2/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/doctrees/index.doctree` & `pycoparsec-0.0.2/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/html/genindex.html` & `pycoparsec-0.0.2/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/html/index.html` & `pycoparsec-0.0.2/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/html/search.html` & `pycoparsec-0.0.2/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/html/searchindex.js` & `pycoparsec-0.0.2/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/html/_static/alabaster.css` & `pycoparsec-0.0.2/docs/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/html/_static/basic.css` & `pycoparsec-0.0.2/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/html/_static/doctools.js` & `pycoparsec-0.0.2/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/html/_static/language_data.js` & `pycoparsec-0.0.2/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/html/_static/pygments.css` & `pycoparsec-0.0.2/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/html/_static/searchtools.js` & `pycoparsec-0.0.2/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/docs/_build/html/_static/sphinx_highlight.js` & `pycoparsec-0.0.2/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/src/pycoparsec/parser.py` & `pycoparsec-0.0.2/src/pycoparsec/parser.py`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/LICENSE.txt` & `pycoparsec-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/README.md` & `pycoparsec-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pycoparsec-0.0.1/pyproject.toml` & `pycoparsec-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pycoparsec"
 dynamic = ["version"]
-description = ''
+description = 'A proof-of-concept parser combinator library employing stack frame closures.'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "LGPL-3.0-or-later"
 keywords = []
 authors = [
   { name = "DataKinds", email = "tslimkemann42@gmail.com" },
 ]
```

### Comparing `pycoparsec-0.0.1/PKG-INFO` & `pycoparsec-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: pycoparsec
-Version: 0.0.1
+Version: 0.0.2
+Summary: A proof-of-concept parser combinator library employing stack frame closures.
 Project-URL: Documentation, https://github.com/DataKinds/pycoparsec#readme
 Project-URL: Issues, https://github.com/DataKinds/pycoparsec/issues
 Project-URL: Source, https://github.com/DataKinds/pycoparsec
 Author-email: DataKinds <tslimkemann42@gmail.com>
 License-Expression: LGPL-3.0-or-later
 License-File: LICENSE.txt
 Classifier: Development Status :: 2 - Pre-Alpha
```

