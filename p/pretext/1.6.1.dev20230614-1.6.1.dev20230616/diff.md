# Comparing `tmp/pretext-1.6.1.dev20230614.tar.gz` & `tmp/pretext-1.6.1.dev20230616.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretext-1.6.1.dev20230614.tar", max compression
+gzip compressed data, was "pretext-1.6.1.dev20230616.tar", max compression
```

## Comparing `pretext-1.6.1.dev20230614.tar` & `pretext-1.6.1.dev20230616.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    35148 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/LICENSE
--rw-r--r--   0        0        0     9757 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/README.md
--rw-r--r--   0        0        0     1901 2023-06-14 06:19:41.464059 pretext-1.6.1.dev20230614/pretext/__init__.py
--rw-r--r--   0        0        0       61 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/pretext/__main__.py
--rw-r--r--   0        0        0     8170 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/pretext/build.py
--rw-r--r--   0        0        0    25351 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/pretext/cli.py
--rw-r--r--   0        0        0     5694 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/pretext/codechat.py
--rw-r--r--   0        0        0     5692 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/pretext/config/xml_overlay.py
--rw-r--r--   0        0        0      350 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/pretext/core/__init__.py
--rw-r--r--   0        0        0   172432 2023-06-14 06:19:46.556099 pretext-1.6.1.dev20230614/pretext/core/pretext.py
--rw-r--r--   0        0        0     1465 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/pretext/core/resources.py
--rw-r--r--   0        0        0  1035294 2023-06-14 06:19:46.552099 pretext-1.6.1.dev20230614/pretext/core/resources.zip
--rw-r--r--   0        0        0    15723 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/pretext/generate.py
--rw-r--r--   0        0        0    27475 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/pretext/project.py
--rw-r--r--   0        0        0      516 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/pretext/templates/__init__.py
--rw-r--r--   0        0        0     1676 2023-06-14 06:19:46.624100 pretext-1.6.1.dev20230614/pretext/templates/resources/.gitignore
--rw-r--r--   0        0        0        0 2023-06-14 06:19:46.624100 pretext-1.6.1.dev20230614/pretext/templates/resources/__init__.py
--rw-r--r--   0        0        0   160064 2023-06-14 06:19:46.600100 pretext-1.6.1.dev20230614/pretext/templates/resources/article.zip
--rw-r--r--   0        0        0     7570 2023-06-14 06:19:46.604100 pretext-1.6.1.dev20230614/pretext/templates/resources/book.zip
--rw-r--r--   0        0        0   173263 2023-06-14 06:19:46.616100 pretext-1.6.1.dev20230614/pretext/templates/resources/demo.zip
--rw-r--r--   0        0        0     2059 2023-06-14 06:19:46.624100 pretext-1.6.1.dev20230614/pretext/templates/resources/devcontainer.json
--rw-r--r--   0        0        0     4611 2023-06-14 06:19:46.620100 pretext-1.6.1.dev20230614/pretext/templates/resources/hello.zip
--rw-r--r--   0        0        0     1710 2023-06-14 06:19:46.624100 pretext-1.6.1.dev20230614/pretext/templates/resources/project.ptx
--rw-r--r--   0        0        0      242 2023-06-14 06:19:46.624100 pretext-1.6.1.dev20230614/pretext/templates/resources/publication.ptx
--rw-r--r--   0        0        0     8346 2023-06-14 06:19:46.624100 pretext-1.6.1.dev20230614/pretext/templates/resources/slideshow.zip
--rw-r--r--   0        0        0    18416 2023-06-14 06:19:06.307832 pretext-1.6.1.dev20230614/pretext/utils.py
--rw-r--r--   0        0        0     1143 2023-06-14 06:19:41.464059 pretext-1.6.1.dev20230614/pyproject.toml
--rw-r--r--   0        0        0    10854 1970-01-01 00:00:00.000000 pretext-1.6.1.dev20230614/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-06-16 06:18:27.362869 pretext-1.6.1.dev20230616/LICENSE
+-rw-r--r--   0        0        0     9757 2023-06-16 06:18:27.362869 pretext-1.6.1.dev20230616/README.md
+-rw-r--r--   0        0        0     1901 2023-06-16 06:18:58.155167 pretext-1.6.1.dev20230616/pretext/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-16 06:18:27.362869 pretext-1.6.1.dev20230616/pretext/__main__.py
+-rw-r--r--   0        0        0     8170 2023-06-16 06:18:27.362869 pretext-1.6.1.dev20230616/pretext/build.py
+-rw-r--r--   0        0        0    25351 2023-06-16 06:18:27.362869 pretext-1.6.1.dev20230616/pretext/cli.py
+-rw-r--r--   0        0        0     5694 2023-06-16 06:18:27.362869 pretext-1.6.1.dev20230616/pretext/codechat.py
+-rw-r--r--   0        0        0     5692 2023-06-16 06:18:27.362869 pretext-1.6.1.dev20230616/pretext/config/xml_overlay.py
+-rw-r--r--   0        0        0      350 2023-06-16 06:18:27.362869 pretext-1.6.1.dev20230616/pretext/core/__init__.py
+-rw-r--r--   0        0        0   172432 2023-06-16 06:19:03.235211 pretext-1.6.1.dev20230616/pretext/core/pretext.py
+-rw-r--r--   0        0        0     1465 2023-06-16 06:18:27.362869 pretext-1.6.1.dev20230616/pretext/core/resources.py
+-rw-r--r--   0        0        0  1035425 2023-06-16 06:19:03.235211 pretext-1.6.1.dev20230616/pretext/core/resources.zip
+-rw-r--r--   0        0        0    15723 2023-06-16 06:18:27.362869 pretext-1.6.1.dev20230616/pretext/generate.py
+-rw-r--r--   0        0        0    27475 2023-06-16 06:18:27.362869 pretext-1.6.1.dev20230616/pretext/project.py
+-rw-r--r--   0        0        0      516 2023-06-16 06:18:27.362869 pretext-1.6.1.dev20230616/pretext/templates/__init__.py
+-rw-r--r--   0        0        0     1676 2023-06-16 06:19:03.307211 pretext-1.6.1.dev20230616/pretext/templates/resources/.gitignore
+-rw-r--r--   0        0        0        0 2023-06-16 06:19:03.307211 pretext-1.6.1.dev20230616/pretext/templates/resources/__init__.py
+-rw-r--r--   0        0        0   160064 2023-06-16 06:19:03.303212 pretext-1.6.1.dev20230616/pretext/templates/resources/article.zip
+-rw-r--r--   0        0        0     7570 2023-06-16 06:19:03.275211 pretext-1.6.1.dev20230616/pretext/templates/resources/book.zip
+-rw-r--r--   0        0        0   173263 2023-06-16 06:19:03.291211 pretext-1.6.1.dev20230616/pretext/templates/resources/demo.zip
+-rw-r--r--   0        0        0     2059 2023-06-16 06:19:03.307211 pretext-1.6.1.dev20230616/pretext/templates/resources/devcontainer.json
+-rw-r--r--   0        0        0     4611 2023-06-16 06:19:03.275211 pretext-1.6.1.dev20230616/pretext/templates/resources/hello.zip
+-rw-r--r--   0        0        0     1710 2023-06-16 06:19:03.307211 pretext-1.6.1.dev20230616/pretext/templates/resources/project.ptx
+-rw-r--r--   0        0        0      242 2023-06-16 06:19:03.307211 pretext-1.6.1.dev20230616/pretext/templates/resources/publication.ptx
+-rw-r--r--   0        0        0     8346 2023-06-16 06:19:03.303212 pretext-1.6.1.dev20230616/pretext/templates/resources/slideshow.zip
+-rw-r--r--   0        0        0    18416 2023-06-16 06:18:27.362869 pretext-1.6.1.dev20230616/pretext/utils.py
+-rw-r--r--   0        0        0     1143 2023-06-16 06:18:58.155167 pretext-1.6.1.dev20230616/pyproject.toml
+-rw-r--r--   0        0        0    10854 1970-01-01 00:00:00.000000 pretext-1.6.1.dev20230616/PKG-INFO
```

### Comparing `pretext-1.6.1.dev20230614/LICENSE` & `pretext-1.6.1.dev20230616/LICENSE`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230614/README.md` & `pretext-1.6.1.dev20230616/README.md`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230614/pretext/__init__.py` & `pretext-1.6.1.dev20230616/pretext/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from pathlib import Path
 from single_version import get_version
 
 VERSION = get_version("pretext", Path(__file__).parent.parent)
 
-CORE_COMMIT = 'dff67ac239d84354138b15cf6a729200f606ea94'
+CORE_COMMIT = 'ff0bbb5094413ea2c332328c2359226629b9e7c5'
 
 # List of templates, build formats, and assets that are supported by the CLI.
 NEW_TEMPLATES = ["book", "article", "demo", "hello", "slideshow"]
 BUILD_FORMATS = [
     "html",
     "pdf",
     "latex",
```

### Comparing `pretext-1.6.1.dev20230614/pretext/build.py` & `pretext-1.6.1.dev20230616/pretext/build.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230614/pretext/cli.py` & `pretext-1.6.1.dev20230616/pretext/cli.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230614/pretext/codechat.py` & `pretext-1.6.1.dev20230616/pretext/codechat.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230614/pretext/config/xml_overlay.py` & `pretext-1.6.1.dev20230616/pretext/config/xml_overlay.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230614/pretext/core/pretext.py` & `pretext-1.6.1.dev20230616/pretext/core/pretext.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230614/pretext/core/resources.py` & `pretext-1.6.1.dev20230616/pretext/core/resources.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230614/pretext/core/resources.zip` & `pretext-1.6.1.dev20230616/pretext/core/resources.zip`

 * *Files 12% similar despite different names*

#### zipinfo {}

```diff
@@ -1,143 +1,143 @@
-Zip file size: 1035294 bytes, number of entries: 141
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 css/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 pretext/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 schema/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 script/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 xsl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 xsl/latex/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 xsl/localizations/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 xsl/support/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 xsl/utilities/
--rw-r--r--  2.0 unx   231248 b- defN 23-Jun-14 06:19 xsl/publisher-variables.xsl
--rw-r--r--  2.0 unx   611581 b- defN 23-Jun-14 06:19 xsl/pretext-html.xsl
--rw-r--r--  2.0 unx     6066 b- defN 23-Jun-14 06:19 xsl/pretext-json-manifest.xsl
--rw-r--r--  2.0 unx     4571 b- defN 23-Jun-14 06:19 xsl/pretext-litprog.xsl
--rw-r--r--  2.0 unx     2725 b- defN 23-Jun-14 06:19 xsl/extract-asymptote.xsl
--rw-r--r--  2.0 unx   139486 b- defN 23-Jun-14 06:19 xsl/extract-pg.xsl
--rw-r--r--  2.0 unx     9787 b- defN 23-Jun-14 06:19 xsl/entities.ent
--rw-r--r--  2.0 unx    13186 b- defN 23-Jun-14 06:19 xsl/pretext-solution-manual-latex.xsl
--rw-r--r--  2.0 unx     6281 b- defN 23-Jun-14 06:19 xsl/pretext-numbers.xsl
--rw-r--r--  2.0 unx     2597 b- defN 23-Jun-14 06:19 xsl/extract-trace.xsl
--rw-r--r--  2.0 unx     8535 b- defN 23-Jun-14 06:19 xsl/pretext-view-source.xsl
--rw-r--r--  2.0 unx    10708 b- defN 23-Jun-14 06:19 xsl/pretext-units.xsl
--rw-r--r--  2.0 unx     3239 b- defN 23-Jun-14 06:19 xsl/extract-interactive.xsl
--rw-r--r--  2.0 unx    40230 b- defN 23-Jun-14 06:19 xsl/pretext-jupyter.xsl
--rw-r--r--  2.0 unx   112450 b- defN 23-Jun-14 06:19 xsl/pretext-assembly.xsl
--rw-r--r--  2.0 unx    43020 b- defN 23-Jun-14 06:19 xsl/pretext-text-utilities.xsl
--rw-r--r--  2.0 unx    39918 b- defN 23-Jun-14 06:19 xsl/pretext-runestone-static.xsl
--rw-r--r--  2.0 unx    13037 b- defN 23-Jun-14 06:19 xsl/pretext-text.xsl
--rw-r--r--  2.0 unx    89128 b- defN 23-Jun-14 06:19 xsl/pretext-braille-preprint.xsl
--rw-r--r--  2.0 unx     2846 b- defN 23-Jun-14 06:19 xsl/extract-datafile.xsl
--rw-r--r--  2.0 unx     2601 b- defN 23-Jun-14 06:19 xsl/pretext-merge.xsl
--rw-r--r--  2.0 unx    17293 b- defN 23-Jun-14 06:19 xsl/pretext-ww-problem-sets.xsl
--rw-r--r--  2.0 unx   546938 b- defN 23-Jun-14 06:19 xsl/pretext-common.xsl
--rw-r--r--  2.0 unx    21086 b- defN 23-Jun-14 06:19 xsl/pretext-smc.xsl
--rw-r--r--  2.0 unx     8125 b- defN 23-Jun-14 06:19 xsl/extract-sageplot.xsl
--rw-r--r--  2.0 unx     8130 b- defN 23-Jun-14 06:19 xsl/extract-identity.xsl
--rw-r--r--  2.0 unx    41730 b- defN 23-Jun-14 06:19 xsl/pretext-beamer.xsl
--rw-r--r--  2.0 unx   109017 b- defN 23-Jun-14 06:19 xsl/pretext-runestone.xsl
--rw-r--r--  2.0 unx     3560 b- defN 23-Jun-14 06:19 xsl/pretext-basic-html.xsl
--rw-r--r--  2.0 unx     2709 b- defN 23-Jun-14 06:19 xsl/extract-qrcode.xsl
--rw-r--r--  2.0 unx     2248 b- defN 23-Jun-14 06:19 xsl/extract-mom.xsl
--rw-r--r--  2.0 unx     2740 b- defN 23-Jun-14 06:19 xsl/extract-youtube.xsl
--rw-r--r--  2.0 unx     1768 b- defN 23-Jun-14 06:19 xsl/README.md
--rw-r--r--  2.0 unx    67275 b- defN 23-Jun-14 06:19 xsl/pretext-epub.xsl
--rw-r--r--  2.0 unx    11766 b- defN 23-Jun-14 06:19 xsl/pretext-sage-doctest.xsl
--rw-r--r--  2.0 unx    22121 b- defN 23-Jun-14 06:19 xsl/pretext-revealjs.xsl
--rw-r--r--  2.0 unx    12084 b- defN 23-Jun-14 06:19 xsl/xml-to-json.xsl
--rw-r--r--  2.0 unx   544229 b- defN 23-Jun-14 06:19 xsl/pretext-latex.xsl
--rw-r--r--  2.0 unx    19072 b- defN 23-Jun-14 06:19 xsl/extract-latex-image.xsl
--rw-r--r--  2.0 unx      513 b- defN 23-Jun-14 06:19 xsl/utilities/deprecate-autoname.sed
--rw-r--r--  2.0 unx      787 b- defN 23-Jun-14 06:19 xsl/utilities/deprecate-index.sed
--rw-r--r--  2.0 unx    30257 b- defN 23-Jun-14 06:19 xsl/utilities/fix-deprecations.xsl
--rw-r--r--  2.0 unx     4299 b- defN 23-Jun-14 06:19 xsl/utilities/author-report.xsl
--rw-r--r--  2.0 unx     4926 b- defN 23-Jun-14 06:19 xsl/utilities/pretext-enhanced-source.xsl
--rw-r--r--  2.0 unx     1810 b- defN 23-Jun-14 06:19 xsl/utilities/README.md
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 xsl/support/play-button/
--rw-r--r--  2.0 unx    10306 b- defN 23-Jun-14 06:19 xsl/support/extract-math.xsl
--rw-r--r--  2.0 unx     5241 b- defN 23-Jun-14 06:19 xsl/support/pretext-pg-macros.xsl
--rw-r--r--  2.0 unx      486 b- defN 23-Jun-14 06:19 xsl/support/runestone-services.xml
--rw-r--r--  2.0 unx     5065 b- defN 23-Jun-14 06:19 xsl/support/extract-latex-image-labels.xsl
--rw-r--r--  2.0 unx     5879 b- defN 23-Jun-14 06:19 xsl/support/package-math.xsl
--rw-r--r--  2.0 unx      504 b- defN 23-Jun-14 06:19 xsl/support/README.md
--rw-r--r--  2.0 unx     5800 b- defN 23-Jun-14 06:19 xsl/support/tactile-svg.xsl
--rw-r--r--  2.0 unx      722 b- defN 23-Jun-14 06:19 xsl/support/play-button/play-button.svg
--rw-r--r--  2.0 unx     2657 b- defN 23-Jun-14 06:19 xsl/support/play-button/README.md
--rw-r--r--  2.0 unx     6621 b- defN 23-Jun-14 06:19 xsl/support/play-button/play-button.png
--rw-r--r--  2.0 unx    16236 b- defN 23-Jun-14 06:19 xsl/localizations/ca-ES.xml
--rw-r--r--  2.0 unx    16821 b- defN 23-Jun-14 06:19 xsl/localizations/af-ZA.xml
--rw-r--r--  2.0 unx    16518 b- defN 23-Jun-14 06:19 xsl/localizations/es-ES.xml
--rw-r--r--  2.0 unx    17215 b- defN 23-Jun-14 06:19 xsl/localizations/de-DE.xml
--rw-r--r--  2.0 unx    15566 b- defN 23-Jun-14 06:19 xsl/localizations/cs-CZ.xml
--rw-r--r--  2.0 unx    19169 b- defN 23-Jun-14 06:19 xsl/localizations/nl-NL.xml
--rw-r--r--  2.0 unx    19049 b- defN 23-Jun-14 06:19 xsl/localizations/en-US.xml
--rw-r--r--  2.0 unx    15938 b- defN 23-Jun-14 06:19 xsl/localizations/it-IT.xml
--rw-r--r--  2.0 unx    17285 b- defN 23-Jun-14 06:19 xsl/localizations/fi-FI.xml
--rw-r--r--  2.0 unx    16296 b- defN 23-Jun-14 06:19 xsl/localizations/pt-BR.xml
--rw-r--r--  2.0 unx    16333 b- defN 23-Jun-14 06:19 xsl/localizations/fr-FR.xml
--rw-r--r--  2.0 unx    17065 b- defN 23-Jun-14 06:19 xsl/localizations/pt-PT.xml
--rw-r--r--  2.0 unx    16069 b- defN 23-Jun-14 06:19 xsl/localizations/hu-HU.xml
--rw-r--r--  2.0 unx    16484 b- defN 23-Jun-14 06:19 xsl/localizations/fr-CA.xml
--rw-r--r--  2.0 unx    17040 b- defN 23-Jun-14 06:19 xsl/localizations/bg-BG.xml
--rw-r--r--  2.0 unx     2227 b- defN 23-Jun-14 06:19 xsl/localizations/localizations.xml
--rw-r--r--  2.0 unx     4708 b- defN 23-Jun-14 06:19 xsl/localizations/README.md
--rw-r--r--  2.0 unx    14482 b- defN 23-Jun-14 06:19 xsl/latex/pretext-latex-chaos.xsl
--rw-r--r--  2.0 unx     2261 b- defN 23-Jun-14 06:19 xsl/latex/pretext-latex-AIM.xsl
--rw-r--r--  2.0 unx     7526 b- defN 23-Jun-14 06:19 xsl/latex/pretext-latex-CLP.xsl
--rw-r--r--  2.0 unx     3024 b- defN 23-Jun-14 06:19 xsl/latex/pretext-latex-dyslexic-font.xsl
--rw-r--r--  2.0 unx     5135 b- defN 23-Jun-14 06:19 xsl/latex/pretext-latex-guide.xsl
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-14 06:19 css/colors_orange_navy.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-14 06:19 css/colors_green_blue.css
--rw-r--r--  2.0 unx     2441 b- defN 23-Jun-14 06:19 css/kindle.css
--rw-r--r--  2.0 unx     4021 b- defN 23-Jun-14 06:19 css/update_css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-14 06:19 css/colors_ruby_turquoise.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-14 06:19 css/colors_ruby_amethyst.css
--rw-r--r--  2.0 unx     2608 b- defN 23-Jun-14 06:19 css/colors_default.css
--rw-r--r--  2.0 unx     1338 b- defN 23-Jun-14 06:19 css/colors_red_blue.css
--rw-r--r--  2.0 unx      691 b- defN 23-Jun-14 06:19 css/colors_pastel_blue_orange.css
--rw-r--r--  2.0 unx     3473 b- defN 23-Jun-14 06:19 css/style_soundwriting.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jun-14 06:19 css/colors_darkmartiansands.css
--rw-r--r--  2.0 unx     2438 b- defN 23-Jun-14 06:19 css/colors_blue_grey.css
--rw-r--r--  2.0 unx     4308 b- defN 23-Jun-14 06:19 css/colors_blue_green.css
--rw-r--r--  2.0 unx   146685 b- defN 23-Jun-14 06:19 css/mathbook-content.css
--rw-r--r--  2.0 unx     1276 b- defN 23-Jun-14 06:19 css/colors_maroon_grey.css
--rw-r--r--  2.0 unx    22438 b- defN 23-Jun-14 06:19 css/pretext.css
--rw-r--r--  2.0 unx     1280 b- defN 23-Jun-14 06:19 css/colors_brown_gold.css
--rw-r--r--  2.0 unx     1362 b- defN 23-Jun-14 06:19 css/epub.css
--rw-r--r--  2.0 unx    63664 b- defN 23-Jun-14 06:19 css/mathbook-add-on.css
--rw-r--r--  2.0 unx    14069 b- defN 23-Jun-14 06:19 css/setcolors.css
--rw-r--r--  2.0 unx    71198 b- defN 23-Jun-14 06:19 css/pretext_add_on.css
--rw-r--r--  2.0 unx   435680 b- defN 23-Jun-14 06:19 css/mathbook-3.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-14 06:19 css/colors_green_plum.css
--rw-r--r--  2.0 unx    12567 b- defN 23-Jun-14 06:19 css/style_oscarlevin.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-14 06:19 css/colors_blue_red.css
--rw-r--r--  2.0 unx     2446 b- defN 23-Jun-14 06:19 css/colors_martiansands.css
--rw-r--r--  2.0 unx     1865 b- defN 23-Jun-14 06:19 css/README.md
--rw-r--r--  2.0 unx     7761 b- defN 23-Jun-14 06:19 css/style_default.css
--rw-r--r--  2.0 unx     2397 b- defN 23-Jun-14 06:19 css/colors_ruby_emerald.css
--rw-r--r--  2.0 unx    35449 b- defN 23-Jun-14 06:19 pretext/braille_format.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-14 06:19 pretext/__init__.py
--rw-r--r--  2.0 unx     2566 b- defN 23-Jun-14 06:19 pretext/pretext.cfg
--rw-r--r--  2.0 unx    30908 b- defN 23-Jun-14 06:19 pretext/pretext
--rw-r--r--  2.0 unx     1955 b- defN 23-Jun-14 06:19 pretext/module-test.py
--rw-r--r--  2.0 unx   172432 b- defN 23-Jun-14 06:19 pretext/pretext.py
--rw-r--r--  2.0 unx     1367 b- defN 23-Jun-14 06:19 pretext/README.md
--rw-r--r--  2.0 unx      326 b- defN 23-Jun-14 06:19 schema/xml.xsd
--rw-r--r--  2.0 unx    18421 b- defN 23-Jun-14 06:19 schema/pretext-schematron.xsl
--rw-r--r--  2.0 unx    17587 b- defN 23-Jun-14 06:19 schema/pretext-dev.rnc
--rw-r--r--  2.0 unx   134043 b- defN 23-Jun-14 06:19 schema/pretext.xml
--rw-r--r--  2.0 unx    58086 b- defN 23-Jun-14 06:19 schema/pretext.rnc
--rw-r--r--  2.0 unx   101829 b- defN 23-Jun-14 06:19 schema/pretext.rng
--rw-r--r--  2.0 unx    34210 b- defN 23-Jun-14 06:19 schema/pretext-dev.rng
--rw-r--r--  2.0 unx     3135 b- defN 23-Jun-14 06:19 schema/build.sh
--rw-r--r--  2.0 unx   125135 b- defN 23-Jun-14 06:19 schema/pretext.xsd
--rw-r--r--  2.0 unx     1180 b- defN 23-Jun-14 06:19 schema/README.md
--rw-r--r--  2.0 unx    25870 b- defN 23-Jun-14 06:19 schema/pretext-validation-plus.xsl
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 script/mjsre/
--rw-r--r--  2.0 unx     2666 b- defN 23-Jun-14 06:19 script/mbx
--rw-r--r--  2.0 unx      258 b- defN 23-Jun-14 06:19 script/README.md
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-14 06:19 script/mjsre/update-sre
--rw-r--r--  2.0 unx      116 b- defN 23-Jun-14 06:19 script/mjsre/package.json
--rw-r--r--  2.0 unx      481 b- defN 23-Jun-14 06:19 script/mjsre/README.md
--rw-r--r--  2.0 unx     9251 b- defN 23-Jun-14 06:19 script/mjsre/mj-sre-page.js
-141 files, 4813648 bytes uncompressed, 1017852 bytes compressed:  78.9%
+Zip file size: 1035425 bytes, number of entries: 141
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:19 css/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:19 pretext/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:19 schema/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:19 script/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:19 xsl/
+-rw-r--r--  2.0 unx     2608 b- defN 23-Jun-16 06:19 css/colors_default.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-16 06:19 css/colors_green_plum.css
+-rw-r--r--  2.0 unx    14069 b- defN 23-Jun-16 06:19 css/setcolors.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-16 06:19 css/colors_ruby_emerald.css
+-rw-r--r--  2.0 unx   435680 b- defN 23-Jun-16 06:19 css/mathbook-3.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-16 06:19 css/colors_blue_red.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-16 06:19 css/colors_orange_navy.css
+-rw-r--r--  2.0 unx    63664 b- defN 23-Jun-16 06:19 css/mathbook-add-on.css
+-rw-r--r--  2.0 unx     1362 b- defN 23-Jun-16 06:19 css/epub.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-16 06:19 css/colors_green_blue.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-16 06:19 css/colors_ruby_turquoise.css
+-rw-r--r--  2.0 unx     1865 b- defN 23-Jun-16 06:19 css/README.md
+-rw-r--r--  2.0 unx     1338 b- defN 23-Jun-16 06:19 css/colors_red_blue.css
+-rw-r--r--  2.0 unx    12567 b- defN 23-Jun-16 06:19 css/style_oscarlevin.css
+-rw-r--r--  2.0 unx     1276 b- defN 23-Jun-16 06:19 css/colors_maroon_grey.css
+-rw-r--r--  2.0 unx      691 b- defN 23-Jun-16 06:19 css/colors_pastel_blue_orange.css
+-rw-r--r--  2.0 unx     1280 b- defN 23-Jun-16 06:19 css/colors_brown_gold.css
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-16 06:19 css/colors_ruby_amethyst.css
+-rw-r--r--  2.0 unx    71198 b- defN 23-Jun-16 06:19 css/pretext_add_on.css
+-rw-r--r--  2.0 unx     4021 b- defN 23-Jun-16 06:19 css/update_css
+-rw-r--r--  2.0 unx     2438 b- defN 23-Jun-16 06:19 css/colors_blue_grey.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jun-16 06:19 css/colors_darkmartiansands.css
+-rw-r--r--  2.0 unx     7761 b- defN 23-Jun-16 06:19 css/style_default.css
+-rw-r--r--  2.0 unx   146685 b- defN 23-Jun-16 06:19 css/mathbook-content.css
+-rw-r--r--  2.0 unx     2441 b- defN 23-Jun-16 06:19 css/kindle.css
+-rw-r--r--  2.0 unx     3473 b- defN 23-Jun-16 06:19 css/style_soundwriting.css
+-rw-r--r--  2.0 unx    22438 b- defN 23-Jun-16 06:19 css/pretext.css
+-rw-r--r--  2.0 unx     4308 b- defN 23-Jun-16 06:19 css/colors_blue_green.css
+-rw-r--r--  2.0 unx     2446 b- defN 23-Jun-16 06:19 css/colors_martiansands.css
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:19 xsl/latex/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:19 xsl/localizations/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:19 xsl/support/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:19 xsl/utilities/
+-rw-r--r--  2.0 unx     2248 b- defN 23-Jun-16 06:19 xsl/extract-mom.xsl
+-rw-r--r--  2.0 unx   109017 b- defN 23-Jun-16 06:19 xsl/pretext-runestone.xsl
+-rw-r--r--  2.0 unx     8535 b- defN 23-Jun-16 06:19 xsl/pretext-view-source.xsl
+-rw-r--r--  2.0 unx     6066 b- defN 23-Jun-16 06:19 xsl/pretext-json-manifest.xsl
+-rw-r--r--  2.0 unx   112450 b- defN 23-Jun-16 06:19 xsl/pretext-assembly.xsl
+-rw-r--r--  2.0 unx    41730 b- defN 23-Jun-16 06:19 xsl/pretext-beamer.xsl
+-rw-r--r--  2.0 unx    40230 b- defN 23-Jun-16 06:19 xsl/pretext-jupyter.xsl
+-rw-r--r--  2.0 unx   231248 b- defN 23-Jun-16 06:19 xsl/publisher-variables.xsl
+-rw-r--r--  2.0 unx   612399 b- defN 23-Jun-16 06:19 xsl/pretext-html.xsl
+-rw-r--r--  2.0 unx     8130 b- defN 23-Jun-16 06:19 xsl/extract-identity.xsl
+-rw-r--r--  2.0 unx    43020 b- defN 23-Jun-16 06:19 xsl/pretext-text-utilities.xsl
+-rw-r--r--  2.0 unx    67275 b- defN 23-Jun-16 06:19 xsl/pretext-epub.xsl
+-rw-r--r--  2.0 unx    21086 b- defN 23-Jun-16 06:19 xsl/pretext-smc.xsl
+-rw-r--r--  2.0 unx    13037 b- defN 23-Jun-16 06:19 xsl/pretext-text.xsl
+-rw-r--r--  2.0 unx     1768 b- defN 23-Jun-16 06:19 xsl/README.md
+-rw-r--r--  2.0 unx    12084 b- defN 23-Jun-16 06:19 xsl/xml-to-json.xsl
+-rw-r--r--  2.0 unx    17293 b- defN 23-Jun-16 06:19 xsl/pretext-ww-problem-sets.xsl
+-rw-r--r--  2.0 unx   139486 b- defN 23-Jun-16 06:19 xsl/extract-pg.xsl
+-rw-r--r--  2.0 unx     2709 b- defN 23-Jun-16 06:19 xsl/extract-qrcode.xsl
+-rw-r--r--  2.0 unx    13186 b- defN 23-Jun-16 06:19 xsl/pretext-solution-manual-latex.xsl
+-rw-r--r--  2.0 unx     6281 b- defN 23-Jun-16 06:19 xsl/pretext-numbers.xsl
+-rw-r--r--  2.0 unx     8125 b- defN 23-Jun-16 06:19 xsl/extract-sageplot.xsl
+-rw-r--r--  2.0 unx     2740 b- defN 23-Jun-16 06:19 xsl/extract-youtube.xsl
+-rw-r--r--  2.0 unx     4571 b- defN 23-Jun-16 06:19 xsl/pretext-litprog.xsl
+-rw-r--r--  2.0 unx     3560 b- defN 23-Jun-16 06:19 xsl/pretext-basic-html.xsl
+-rw-r--r--  2.0 unx    11766 b- defN 23-Jun-16 06:19 xsl/pretext-sage-doctest.xsl
+-rw-r--r--  2.0 unx    19072 b- defN 23-Jun-16 06:19 xsl/extract-latex-image.xsl
+-rw-r--r--  2.0 unx     9787 b- defN 23-Jun-16 06:19 xsl/entities.ent
+-rw-r--r--  2.0 unx   544229 b- defN 23-Jun-16 06:19 xsl/pretext-latex.xsl
+-rw-r--r--  2.0 unx    39918 b- defN 23-Jun-16 06:19 xsl/pretext-runestone-static.xsl
+-rw-r--r--  2.0 unx     3239 b- defN 23-Jun-16 06:19 xsl/extract-interactive.xsl
+-rw-r--r--  2.0 unx    89128 b- defN 23-Jun-16 06:19 xsl/pretext-braille-preprint.xsl
+-rw-r--r--  2.0 unx     2597 b- defN 23-Jun-16 06:19 xsl/extract-trace.xsl
+-rw-r--r--  2.0 unx     2601 b- defN 23-Jun-16 06:19 xsl/pretext-merge.xsl
+-rw-r--r--  2.0 unx    22121 b- defN 23-Jun-16 06:19 xsl/pretext-revealjs.xsl
+-rw-r--r--  2.0 unx   546938 b- defN 23-Jun-16 06:19 xsl/pretext-common.xsl
+-rw-r--r--  2.0 unx     2725 b- defN 23-Jun-16 06:19 xsl/extract-asymptote.xsl
+-rw-r--r--  2.0 unx    10708 b- defN 23-Jun-16 06:19 xsl/pretext-units.xsl
+-rw-r--r--  2.0 unx     2846 b- defN 23-Jun-16 06:19 xsl/extract-datafile.xsl
+-rw-r--r--  2.0 unx     4926 b- defN 23-Jun-16 06:19 xsl/utilities/pretext-enhanced-source.xsl
+-rw-r--r--  2.0 unx     4299 b- defN 23-Jun-16 06:19 xsl/utilities/author-report.xsl
+-rw-r--r--  2.0 unx    30257 b- defN 23-Jun-16 06:19 xsl/utilities/fix-deprecations.xsl
+-rw-r--r--  2.0 unx      513 b- defN 23-Jun-16 06:19 xsl/utilities/deprecate-autoname.sed
+-rw-r--r--  2.0 unx     1810 b- defN 23-Jun-16 06:19 xsl/utilities/README.md
+-rw-r--r--  2.0 unx      787 b- defN 23-Jun-16 06:19 xsl/utilities/deprecate-index.sed
+-rw-r--r--  2.0 unx     7526 b- defN 23-Jun-16 06:19 xsl/latex/pretext-latex-CLP.xsl
+-rw-r--r--  2.0 unx     2261 b- defN 23-Jun-16 06:19 xsl/latex/pretext-latex-AIM.xsl
+-rw-r--r--  2.0 unx    14482 b- defN 23-Jun-16 06:19 xsl/latex/pretext-latex-chaos.xsl
+-rw-r--r--  2.0 unx     3024 b- defN 23-Jun-16 06:19 xsl/latex/pretext-latex-dyslexic-font.xsl
+-rw-r--r--  2.0 unx     5135 b- defN 23-Jun-16 06:19 xsl/latex/pretext-latex-guide.xsl
+-rw-r--r--  2.0 unx    17065 b- defN 23-Jun-16 06:19 xsl/localizations/pt-PT.xml
+-rw-r--r--  2.0 unx    15566 b- defN 23-Jun-16 06:19 xsl/localizations/cs-CZ.xml
+-rw-r--r--  2.0 unx    16069 b- defN 23-Jun-16 06:19 xsl/localizations/hu-HU.xml
+-rw-r--r--  2.0 unx    16518 b- defN 23-Jun-16 06:19 xsl/localizations/es-ES.xml
+-rw-r--r--  2.0 unx    15938 b- defN 23-Jun-16 06:19 xsl/localizations/it-IT.xml
+-rw-r--r--  2.0 unx    16333 b- defN 23-Jun-16 06:19 xsl/localizations/fr-FR.xml
+-rw-r--r--  2.0 unx     4708 b- defN 23-Jun-16 06:19 xsl/localizations/README.md
+-rw-r--r--  2.0 unx    16296 b- defN 23-Jun-16 06:19 xsl/localizations/pt-BR.xml
+-rw-r--r--  2.0 unx    16821 b- defN 23-Jun-16 06:19 xsl/localizations/af-ZA.xml
+-rw-r--r--  2.0 unx     2227 b- defN 23-Jun-16 06:19 xsl/localizations/localizations.xml
+-rw-r--r--  2.0 unx    19169 b- defN 23-Jun-16 06:19 xsl/localizations/nl-NL.xml
+-rw-r--r--  2.0 unx    16236 b- defN 23-Jun-16 06:19 xsl/localizations/ca-ES.xml
+-rw-r--r--  2.0 unx    17215 b- defN 23-Jun-16 06:19 xsl/localizations/de-DE.xml
+-rw-r--r--  2.0 unx    17040 b- defN 23-Jun-16 06:19 xsl/localizations/bg-BG.xml
+-rw-r--r--  2.0 unx    16484 b- defN 23-Jun-16 06:19 xsl/localizations/fr-CA.xml
+-rw-r--r--  2.0 unx    17285 b- defN 23-Jun-16 06:19 xsl/localizations/fi-FI.xml
+-rw-r--r--  2.0 unx    19049 b- defN 23-Jun-16 06:19 xsl/localizations/en-US.xml
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:19 xsl/support/play-button/
+-rw-r--r--  2.0 unx     5241 b- defN 23-Jun-16 06:19 xsl/support/pretext-pg-macros.xsl
+-rw-r--r--  2.0 unx     5879 b- defN 23-Jun-16 06:19 xsl/support/package-math.xsl
+-rw-r--r--  2.0 unx      504 b- defN 23-Jun-16 06:19 xsl/support/README.md
+-rw-r--r--  2.0 unx     5065 b- defN 23-Jun-16 06:19 xsl/support/extract-latex-image-labels.xsl
+-rw-r--r--  2.0 unx     5800 b- defN 23-Jun-16 06:19 xsl/support/tactile-svg.xsl
+-rw-r--r--  2.0 unx    10306 b- defN 23-Jun-16 06:19 xsl/support/extract-math.xsl
+-rw-r--r--  2.0 unx      486 b- defN 23-Jun-16 06:19 xsl/support/runestone-services.xml
+-rw-r--r--  2.0 unx     2657 b- defN 23-Jun-16 06:19 xsl/support/play-button/README.md
+-rw-r--r--  2.0 unx     6621 b- defN 23-Jun-16 06:19 xsl/support/play-button/play-button.png
+-rw-r--r--  2.0 unx      722 b- defN 23-Jun-16 06:19 xsl/support/play-button/play-button.svg
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-16 06:19 pretext/__init__.py
+-rw-r--r--  2.0 unx     1955 b- defN 23-Jun-16 06:19 pretext/module-test.py
+-rw-r--r--  2.0 unx     2566 b- defN 23-Jun-16 06:19 pretext/pretext.cfg
+-rw-r--r--  2.0 unx     1367 b- defN 23-Jun-16 06:19 pretext/README.md
+-rw-r--r--  2.0 unx    30908 b- defN 23-Jun-16 06:19 pretext/pretext
+-rw-r--r--  2.0 unx   172432 b- defN 23-Jun-16 06:19 pretext/pretext.py
+-rw-r--r--  2.0 unx    35449 b- defN 23-Jun-16 06:19 pretext/braille_format.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:19 script/mjsre/
+-rw-r--r--  2.0 unx      258 b- defN 23-Jun-16 06:19 script/README.md
+-rw-r--r--  2.0 unx     2666 b- defN 23-Jun-16 06:19 script/mbx
+-rw-r--r--  2.0 unx      481 b- defN 23-Jun-16 06:19 script/mjsre/README.md
+-rw-r--r--  2.0 unx     9251 b- defN 23-Jun-16 06:19 script/mjsre/mj-sre-page.js
+-rw-r--r--  2.0 unx      116 b- defN 23-Jun-16 06:19 script/mjsre/package.json
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-16 06:19 script/mjsre/update-sre
+-rw-r--r--  2.0 unx   125135 b- defN 23-Jun-16 06:19 schema/pretext.xsd
+-rw-r--r--  2.0 unx   101829 b- defN 23-Jun-16 06:19 schema/pretext.rng
+-rw-r--r--  2.0 unx   134043 b- defN 23-Jun-16 06:19 schema/pretext.xml
+-rw-r--r--  2.0 unx    18421 b- defN 23-Jun-16 06:19 schema/pretext-schematron.xsl
+-rw-r--r--  2.0 unx    58086 b- defN 23-Jun-16 06:19 schema/pretext.rnc
+-rw-r--r--  2.0 unx     1180 b- defN 23-Jun-16 06:19 schema/README.md
+-rw-r--r--  2.0 unx    17587 b- defN 23-Jun-16 06:19 schema/pretext-dev.rnc
+-rw-r--r--  2.0 unx      326 b- defN 23-Jun-16 06:19 schema/xml.xsd
+-rw-r--r--  2.0 unx     3135 b- defN 23-Jun-16 06:19 schema/build.sh
+-rw-r--r--  2.0 unx    25870 b- defN 23-Jun-16 06:19 schema/pretext-validation-plus.xsl
+-rw-r--r--  2.0 unx    34210 b- defN 23-Jun-16 06:19 schema/pretext-dev.rng
+141 files, 4814466 bytes uncompressed, 1017983 bytes compressed:  78.9%
```

#### zipnote {}

```diff
@@ -9,416 +9,416 @@
 
 Filename: script/
 Comment: 
 
 Filename: xsl/
 Comment: 
 
-Filename: xsl/latex/
-Comment: 
-
-Filename: xsl/localizations/
+Filename: css/colors_default.css
 Comment: 
 
-Filename: xsl/support/
+Filename: css/colors_green_plum.css
 Comment: 
 
-Filename: xsl/utilities/
+Filename: css/setcolors.css
 Comment: 
 
-Filename: xsl/publisher-variables.xsl
+Filename: css/colors_ruby_emerald.css
 Comment: 
 
-Filename: xsl/pretext-html.xsl
+Filename: css/mathbook-3.css
 Comment: 
 
-Filename: xsl/pretext-json-manifest.xsl
+Filename: css/colors_blue_red.css
 Comment: 
 
-Filename: xsl/pretext-litprog.xsl
+Filename: css/colors_orange_navy.css
 Comment: 
 
-Filename: xsl/extract-asymptote.xsl
+Filename: css/mathbook-add-on.css
 Comment: 
 
-Filename: xsl/extract-pg.xsl
+Filename: css/epub.css
 Comment: 
 
-Filename: xsl/entities.ent
+Filename: css/colors_green_blue.css
 Comment: 
 
-Filename: xsl/pretext-solution-manual-latex.xsl
+Filename: css/colors_ruby_turquoise.css
 Comment: 
 
-Filename: xsl/pretext-numbers.xsl
+Filename: css/README.md
 Comment: 
 
-Filename: xsl/extract-trace.xsl
+Filename: css/colors_red_blue.css
 Comment: 
 
-Filename: xsl/pretext-view-source.xsl
+Filename: css/style_oscarlevin.css
 Comment: 
 
-Filename: xsl/pretext-units.xsl
+Filename: css/colors_maroon_grey.css
 Comment: 
 
-Filename: xsl/extract-interactive.xsl
+Filename: css/colors_pastel_blue_orange.css
 Comment: 
 
-Filename: xsl/pretext-jupyter.xsl
+Filename: css/colors_brown_gold.css
 Comment: 
 
-Filename: xsl/pretext-assembly.xsl
+Filename: css/colors_ruby_amethyst.css
 Comment: 
 
-Filename: xsl/pretext-text-utilities.xsl
+Filename: css/pretext_add_on.css
 Comment: 
 
-Filename: xsl/pretext-runestone-static.xsl
+Filename: css/update_css
 Comment: 
 
-Filename: xsl/pretext-text.xsl
+Filename: css/colors_blue_grey.css
 Comment: 
 
-Filename: xsl/pretext-braille-preprint.xsl
+Filename: css/colors_darkmartiansands.css
 Comment: 
 
-Filename: xsl/extract-datafile.xsl
+Filename: css/style_default.css
 Comment: 
 
-Filename: xsl/pretext-merge.xsl
+Filename: css/mathbook-content.css
 Comment: 
 
-Filename: xsl/pretext-ww-problem-sets.xsl
+Filename: css/kindle.css
 Comment: 
 
-Filename: xsl/pretext-common.xsl
+Filename: css/style_soundwriting.css
 Comment: 
 
-Filename: xsl/pretext-smc.xsl
+Filename: css/pretext.css
 Comment: 
 
-Filename: xsl/extract-sageplot.xsl
+Filename: css/colors_blue_green.css
 Comment: 
 
-Filename: xsl/extract-identity.xsl
+Filename: css/colors_martiansands.css
 Comment: 
 
-Filename: xsl/pretext-beamer.xsl
+Filename: xsl/latex/
 Comment: 
 
-Filename: xsl/pretext-runestone.xsl
+Filename: xsl/localizations/
 Comment: 
 
-Filename: xsl/pretext-basic-html.xsl
+Filename: xsl/support/
 Comment: 
 
-Filename: xsl/extract-qrcode.xsl
+Filename: xsl/utilities/
 Comment: 
 
 Filename: xsl/extract-mom.xsl
 Comment: 
 
-Filename: xsl/extract-youtube.xsl
+Filename: xsl/pretext-runestone.xsl
 Comment: 
 
-Filename: xsl/README.md
+Filename: xsl/pretext-view-source.xsl
 Comment: 
 
-Filename: xsl/pretext-epub.xsl
+Filename: xsl/pretext-json-manifest.xsl
 Comment: 
 
-Filename: xsl/pretext-sage-doctest.xsl
+Filename: xsl/pretext-assembly.xsl
 Comment: 
 
-Filename: xsl/pretext-revealjs.xsl
+Filename: xsl/pretext-beamer.xsl
 Comment: 
 
-Filename: xsl/xml-to-json.xsl
+Filename: xsl/pretext-jupyter.xsl
 Comment: 
 
-Filename: xsl/pretext-latex.xsl
+Filename: xsl/publisher-variables.xsl
 Comment: 
 
-Filename: xsl/extract-latex-image.xsl
+Filename: xsl/pretext-html.xsl
 Comment: 
 
-Filename: xsl/utilities/deprecate-autoname.sed
+Filename: xsl/extract-identity.xsl
 Comment: 
 
-Filename: xsl/utilities/deprecate-index.sed
+Filename: xsl/pretext-text-utilities.xsl
 Comment: 
 
-Filename: xsl/utilities/fix-deprecations.xsl
+Filename: xsl/pretext-epub.xsl
 Comment: 
 
-Filename: xsl/utilities/author-report.xsl
+Filename: xsl/pretext-smc.xsl
 Comment: 
 
-Filename: xsl/utilities/pretext-enhanced-source.xsl
+Filename: xsl/pretext-text.xsl
 Comment: 
 
-Filename: xsl/utilities/README.md
+Filename: xsl/README.md
 Comment: 
 
-Filename: xsl/support/play-button/
+Filename: xsl/xml-to-json.xsl
 Comment: 
 
-Filename: xsl/support/extract-math.xsl
+Filename: xsl/pretext-ww-problem-sets.xsl
 Comment: 
 
-Filename: xsl/support/pretext-pg-macros.xsl
+Filename: xsl/extract-pg.xsl
 Comment: 
 
-Filename: xsl/support/runestone-services.xml
+Filename: xsl/extract-qrcode.xsl
 Comment: 
 
-Filename: xsl/support/extract-latex-image-labels.xsl
+Filename: xsl/pretext-solution-manual-latex.xsl
 Comment: 
 
-Filename: xsl/support/package-math.xsl
+Filename: xsl/pretext-numbers.xsl
 Comment: 
 
-Filename: xsl/support/README.md
+Filename: xsl/extract-sageplot.xsl
 Comment: 
 
-Filename: xsl/support/tactile-svg.xsl
+Filename: xsl/extract-youtube.xsl
 Comment: 
 
-Filename: xsl/support/play-button/play-button.svg
+Filename: xsl/pretext-litprog.xsl
 Comment: 
 
-Filename: xsl/support/play-button/README.md
+Filename: xsl/pretext-basic-html.xsl
 Comment: 
 
-Filename: xsl/support/play-button/play-button.png
+Filename: xsl/pretext-sage-doctest.xsl
 Comment: 
 
-Filename: xsl/localizations/ca-ES.xml
+Filename: xsl/extract-latex-image.xsl
 Comment: 
 
-Filename: xsl/localizations/af-ZA.xml
+Filename: xsl/entities.ent
 Comment: 
 
-Filename: xsl/localizations/es-ES.xml
+Filename: xsl/pretext-latex.xsl
 Comment: 
 
-Filename: xsl/localizations/de-DE.xml
+Filename: xsl/pretext-runestone-static.xsl
 Comment: 
 
-Filename: xsl/localizations/cs-CZ.xml
+Filename: xsl/extract-interactive.xsl
 Comment: 
 
-Filename: xsl/localizations/nl-NL.xml
+Filename: xsl/pretext-braille-preprint.xsl
 Comment: 
 
-Filename: xsl/localizations/en-US.xml
+Filename: xsl/extract-trace.xsl
 Comment: 
 
-Filename: xsl/localizations/it-IT.xml
+Filename: xsl/pretext-merge.xsl
 Comment: 
 
-Filename: xsl/localizations/fi-FI.xml
+Filename: xsl/pretext-revealjs.xsl
 Comment: 
 
-Filename: xsl/localizations/pt-BR.xml
+Filename: xsl/pretext-common.xsl
 Comment: 
 
-Filename: xsl/localizations/fr-FR.xml
+Filename: xsl/extract-asymptote.xsl
 Comment: 
 
-Filename: xsl/localizations/pt-PT.xml
+Filename: xsl/pretext-units.xsl
 Comment: 
 
-Filename: xsl/localizations/hu-HU.xml
+Filename: xsl/extract-datafile.xsl
 Comment: 
 
-Filename: xsl/localizations/fr-CA.xml
+Filename: xsl/utilities/pretext-enhanced-source.xsl
 Comment: 
 
-Filename: xsl/localizations/bg-BG.xml
+Filename: xsl/utilities/author-report.xsl
 Comment: 
 
-Filename: xsl/localizations/localizations.xml
+Filename: xsl/utilities/fix-deprecations.xsl
 Comment: 
 
-Filename: xsl/localizations/README.md
+Filename: xsl/utilities/deprecate-autoname.sed
 Comment: 
 
-Filename: xsl/latex/pretext-latex-chaos.xsl
+Filename: xsl/utilities/README.md
 Comment: 
 
-Filename: xsl/latex/pretext-latex-AIM.xsl
+Filename: xsl/utilities/deprecate-index.sed
 Comment: 
 
 Filename: xsl/latex/pretext-latex-CLP.xsl
 Comment: 
 
-Filename: xsl/latex/pretext-latex-dyslexic-font.xsl
+Filename: xsl/latex/pretext-latex-AIM.xsl
 Comment: 
 
-Filename: xsl/latex/pretext-latex-guide.xsl
+Filename: xsl/latex/pretext-latex-chaos.xsl
 Comment: 
 
-Filename: css/colors_orange_navy.css
+Filename: xsl/latex/pretext-latex-dyslexic-font.xsl
 Comment: 
 
-Filename: css/colors_green_blue.css
+Filename: xsl/latex/pretext-latex-guide.xsl
 Comment: 
 
-Filename: css/kindle.css
+Filename: xsl/localizations/pt-PT.xml
 Comment: 
 
-Filename: css/update_css
+Filename: xsl/localizations/cs-CZ.xml
 Comment: 
 
-Filename: css/colors_ruby_turquoise.css
+Filename: xsl/localizations/hu-HU.xml
 Comment: 
 
-Filename: css/colors_ruby_amethyst.css
+Filename: xsl/localizations/es-ES.xml
 Comment: 
 
-Filename: css/colors_default.css
+Filename: xsl/localizations/it-IT.xml
 Comment: 
 
-Filename: css/colors_red_blue.css
+Filename: xsl/localizations/fr-FR.xml
 Comment: 
 
-Filename: css/colors_pastel_blue_orange.css
+Filename: xsl/localizations/README.md
 Comment: 
 
-Filename: css/style_soundwriting.css
+Filename: xsl/localizations/pt-BR.xml
 Comment: 
 
-Filename: css/colors_darkmartiansands.css
+Filename: xsl/localizations/af-ZA.xml
 Comment: 
 
-Filename: css/colors_blue_grey.css
+Filename: xsl/localizations/localizations.xml
 Comment: 
 
-Filename: css/colors_blue_green.css
+Filename: xsl/localizations/nl-NL.xml
 Comment: 
 
-Filename: css/mathbook-content.css
+Filename: xsl/localizations/ca-ES.xml
 Comment: 
 
-Filename: css/colors_maroon_grey.css
+Filename: xsl/localizations/de-DE.xml
 Comment: 
 
-Filename: css/pretext.css
+Filename: xsl/localizations/bg-BG.xml
 Comment: 
 
-Filename: css/colors_brown_gold.css
+Filename: xsl/localizations/fr-CA.xml
 Comment: 
 
-Filename: css/epub.css
+Filename: xsl/localizations/fi-FI.xml
 Comment: 
 
-Filename: css/mathbook-add-on.css
+Filename: xsl/localizations/en-US.xml
 Comment: 
 
-Filename: css/setcolors.css
+Filename: xsl/support/play-button/
 Comment: 
 
-Filename: css/pretext_add_on.css
+Filename: xsl/support/pretext-pg-macros.xsl
 Comment: 
 
-Filename: css/mathbook-3.css
+Filename: xsl/support/package-math.xsl
 Comment: 
 
-Filename: css/colors_green_plum.css
+Filename: xsl/support/README.md
 Comment: 
 
-Filename: css/style_oscarlevin.css
+Filename: xsl/support/extract-latex-image-labels.xsl
 Comment: 
 
-Filename: css/colors_blue_red.css
+Filename: xsl/support/tactile-svg.xsl
 Comment: 
 
-Filename: css/colors_martiansands.css
+Filename: xsl/support/extract-math.xsl
 Comment: 
 
-Filename: css/README.md
+Filename: xsl/support/runestone-services.xml
 Comment: 
 
-Filename: css/style_default.css
+Filename: xsl/support/play-button/README.md
 Comment: 
 
-Filename: css/colors_ruby_emerald.css
+Filename: xsl/support/play-button/play-button.png
 Comment: 
 
-Filename: pretext/braille_format.py
+Filename: xsl/support/play-button/play-button.svg
 Comment: 
 
 Filename: pretext/__init__.py
 Comment: 
 
+Filename: pretext/module-test.py
+Comment: 
+
 Filename: pretext/pretext.cfg
 Comment: 
 
-Filename: pretext/pretext
+Filename: pretext/README.md
 Comment: 
 
-Filename: pretext/module-test.py
+Filename: pretext/pretext
 Comment: 
 
 Filename: pretext/pretext.py
 Comment: 
 
-Filename: pretext/README.md
+Filename: pretext/braille_format.py
 Comment: 
 
-Filename: schema/xml.xsd
+Filename: script/mjsre/
 Comment: 
 
-Filename: schema/pretext-schematron.xsl
+Filename: script/README.md
 Comment: 
 
-Filename: schema/pretext-dev.rnc
+Filename: script/mbx
 Comment: 
 
-Filename: schema/pretext.xml
+Filename: script/mjsre/README.md
 Comment: 
 
-Filename: schema/pretext.rnc
+Filename: script/mjsre/mj-sre-page.js
 Comment: 
 
-Filename: schema/pretext.rng
+Filename: script/mjsre/package.json
 Comment: 
 
-Filename: schema/pretext-dev.rng
+Filename: script/mjsre/update-sre
 Comment: 
 
-Filename: schema/build.sh
+Filename: schema/pretext.xsd
 Comment: 
 
-Filename: schema/pretext.xsd
+Filename: schema/pretext.rng
 Comment: 
 
-Filename: schema/README.md
+Filename: schema/pretext.xml
 Comment: 
 
-Filename: schema/pretext-validation-plus.xsl
+Filename: schema/pretext-schematron.xsl
 Comment: 
 
-Filename: script/mjsre/
+Filename: schema/pretext.rnc
 Comment: 
 
-Filename: script/mbx
+Filename: schema/README.md
 Comment: 
 
-Filename: script/README.md
+Filename: schema/pretext-dev.rnc
 Comment: 
 
-Filename: script/mjsre/update-sre
+Filename: schema/xml.xsd
 Comment: 
 
-Filename: script/mjsre/package.json
+Filename: schema/build.sh
 Comment: 
 
-Filename: script/mjsre/README.md
+Filename: schema/pretext-validation-plus.xsl
 Comment: 
 
-Filename: script/mjsre/mj-sre-page.js
+Filename: schema/pretext-dev.rng
 Comment: 
 
 Zip file comment:
```

#### xsl/pretext-html.xsl

##### xsl/pretext-html.xsl

```diff
@@ -2038,16 +2038,16 @@
         <xsl:when test="$knowl-type = 'hidden'">
           <xsl:apply-templates select="." mode="hidden-knowl-filename"/>
         </xsl:when>
       </xsl:choose>
     </xsl:variable>
     <!-- write file infrastructure first -->
     <exsl:document href="{$knowl-file}" method="html" indent="yes" encoding="UTF-8" doctype-system="about:legacy-compat">
-      <html lang="{$document-language}">
-        <!-- dir="rtl" here -->
+      <html>
+        <xsl:call-template name="language-attributes"/>
         <!-- header since separate file -->
         <xsl:text/>
         <xsl:call-template name="converter-blurb-html-no-date"/>
         <head>
           <!-- dissuade indexing duplicated content -->
           <meta name="robots" content="noindex, nofollow"/>
           <!-- we need Sage cell configuration functions     -->
@@ -6544,16 +6544,16 @@
   <xsl:template match="*" mode="standalone-page">
     <xsl:param name="content" select="''"/>
     <xsl:variable name="filename">
       <xsl:apply-templates select="." mode="standalone-filename"/>
     </xsl:variable>
     <exsl:document href="{$filename}" method="html" indent="yes" encoding="UTF-8" doctype-system="about:legacy-compat">
       <xsl:call-template name="converter-blurb-html-no-date"/>
-      <html lang="{$document-language}">
-        <!-- dir="rtl" here -->
+      <html>
+        <xsl:call-template name="language-attributes"/>
         <!-- Open Graph Protocol only in "meta" elements, within "head" -->
         <head xmlns:og="http://ogp.me/ns#" xmlns:book="https://ogp.me/ns/book#">
           <title>
             <!-- Leading with initials is useful for small tabs -->
             <xsl:if test="$docinfo/initialism">
               <xsl:apply-templates select="$docinfo/initialism"/>
               <xsl:text/>
@@ -9202,15 +9202,16 @@
   <!--   Author-libraries after slate exist     -->
   <xsl:template match="interactive[@platform]" mode="create-iframe-page">
     <xsl:variable name="if-filename">
       <xsl:apply-templates select="." mode="iframe-filename"/>
     </xsl:variable>
     <exsl:document href="{$if-filename}" method="html" indent="yes" encoding="UTF-8" doctype-system="about:legacy-compat">
       <xsl:call-template name="converter-blurb-html-no-date"/>
-      <html lang="{$document-language}">
+      <html>
+        <xsl:call-template name="language-attributes"/>
         <head>
           <!-- configure MathJax by default for @platform variants -->
           <xsl:call-template name="mathjax"/>
           <!-- need CSS for sidebyside         -->
           <!-- perhaps this can be specialized -->
           <xsl:call-template name="css"/>
           <!-- maybe icons in captions? -->
@@ -10007,16 +10008,16 @@
       </xsl:variable>
       <exsl:document href="{$the-source-filename}" method="xml" omit-xml-declaration="no" indent="yes" encoding="UTF-8">
         <xsl:copy-of select="."/>
       </exsl:document>
     </xsl:if>
     <exsl:document href="{$the-filename}" method="html" indent="yes" encoding="UTF-8" doctype-system="about:legacy-compat">
       <xsl:call-template name="converter-blurb-html-no-date"/>
-      <html lang="{$document-language}">
-        <!-- dir="rtl" here -->
+      <html>
+        <xsl:call-template name="language-attributes"/>
         <!-- Open Graph Protocol only in "meta" elements, within "head" -->
         <head xmlns:og="http://ogp.me/ns#" xmlns:book="https://ogp.me/ns/book#">
           <title>
             <!-- Leading with initials is useful for small tabs -->
             <xsl:if test="$docinfo/initialism">
               <xsl:apply-templates select="$docinfo/initialism"/>
               <xsl:text/>
@@ -10169,16 +10170,16 @@
     <xsl:variable name="filename">
       <!-- do not use "containing-filename" may be different -->
       <xsl:apply-templates select="." mode="visible-id"/>
       <text>.html</text>
     </xsl:variable>
     <exsl:document href="{$filename}" method="html" indent="yes" encoding="UTF-8" doctype-system="about:legacy-compat">
       <xsl:call-template name="converter-blurb-html-no-date"/>
-      <html lang="{$document-language}">
-        <!-- dir="rtl" here -->
+      <html>
+        <xsl:call-template name="language-attributes"/>
         <!-- Open Graph Protocol only in "meta" elements, within "head" -->
         <head xmlns:og="http://ogp.me/ns#" xmlns:book="https://ogp.me/ns/book#">
           <meta name="Keywords" content="Authored in PreTeXt"/>
           <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
           <!-- canonical link for better SEO -->
           <xsl:call-template name="canonical-link">
             <xsl:with-param name="filename" select="$filename"/>
@@ -12215,14 +12216,35 @@
   <!-- HTML page/file.  Not present in *every* page implemented -->
   <!-- in this file, such as knowls.                            -->
   <xsl:template name="extra-js-footer">
     <xsl:if test="not($html.js.extra = '')">
       <script src="{$html.js.extra}"/>
     </xsl:if>
   </xsl:template>
+  <!-- ################## -->
+  <!-- Language Direction -->
+  <!-- ################## -->
+  <!-- Note: perhaps this should begin in a localization file, -->
+  <!-- and come through as a key; but perhaps this template    -->
+  <!-- can stay as is.                                         -->
+  <xsl:template name="language-attributes">
+    <xsl:attribute name="lang">
+      <xsl:value-of select="$document-language"/>
+    </xsl:attribute>
+    <xsl:attribute name="dir">
+      <xsl:choose>
+        <xsl:when test="$document-language = 'ku-CKB'">
+          <xsl:text>rtl</xsl:text>
+        </xsl:when>
+        <xsl:otherwise>
+          <xsl:text>ltr</xsl:text>
+        </xsl:otherwise>
+      </xsl:choose>
+    </xsl:attribute>
+  </xsl:template>
   <!-- ############## -->
   <!-- LaTeX Preamble -->
   <!-- ############## -->
   <!-- First a variable to massage the author-supplied -->
   <!-- package list to the form MathJax expects        -->
   <xsl:variable name="latex-packages-mathjax">
     <xsl:value-of select="str:replace($latex-packages, '\usepackage{', '\require{')"/>
```

### Comparing `pretext-1.6.1.dev20230614/pretext/generate.py` & `pretext-1.6.1.dev20230616/pretext/generate.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230614/pretext/project.py` & `pretext-1.6.1.dev20230616/pretext/project.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230614/pretext/templates/__init__.py` & `pretext-1.6.1.dev20230616/pretext/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230614/pretext/templates/resources/.gitignore` & `pretext-1.6.1.dev20230616/pretext/templates/resources/.gitignore`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230614/pretext/templates/resources/article.zip` & `pretext-1.6.1.dev20230616/pretext/templates/resources/article.zip`

 * *Files 4% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,16 @@
 Zip file size: 160064 bytes, number of entries: 14
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-14 06:19 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-14 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-14 06:19 project.ptx
--rw-r--r--  2.0 unx       86 b- defN 23-Jun-14 06:19 README.md
--rw-r--r--  2.0 unx   154806 b- defN 23-Jun-14 06:19 assets/frog.jpg
--rw-r--r--  2.0 unx      242 b- defN 23-Jun-14 06:19 publication/publication.ptx
--rw-r--r--  2.0 unx      430 b- defN 23-Jun-14 06:19 source/main.ptx
--rw-r--r--  2.0 unx      449 b- defN 23-Jun-14 06:19 source/section-1.ptx
--rw-r--r--  2.0 unx      982 b- defN 23-Jun-14 06:19 source/section-2.ptx
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-14 06:19 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:19 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:18 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:18 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-16 06:19 .gitignore
+-rw-r--r--  2.0 unx       86 b- defN 23-Jun-16 06:18 README.md
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-16 06:19 codechat_config.yaml
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-16 06:19 project.ptx
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jun-16 06:18 assets/frog.jpg
+-rw-r--r--  2.0 unx      449 b- defN 23-Jun-16 06:18 source/section-1.ptx
+-rw-r--r--  2.0 unx      430 b- defN 23-Jun-16 06:18 source/main.ptx
+-rw-r--r--  2.0 unx      982 b- defN 23-Jun-16 06:18 source/section-2.ptx
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-16 06:19 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      242 b- defN 23-Jun-16 06:18 publication/publication.ptx
 14 files, 164708 bytes uncompressed, 158542 bytes compressed:  3.7%
```

#### zipnote {}

```diff
@@ -9,35 +9,35 @@
 
 Filename: source/
 Comment: 
 
 Filename: .gitignore
 Comment: 
 
-Filename: codechat_config.yaml
+Filename: README.md
 Comment: 
 
-Filename: project.ptx
+Filename: codechat_config.yaml
 Comment: 
 
-Filename: README.md
+Filename: project.ptx
 Comment: 
 
 Filename: assets/frog.jpg
 Comment: 
 
-Filename: publication/publication.ptx
+Filename: source/section-1.ptx
 Comment: 
 
 Filename: source/main.ptx
 Comment: 
 
-Filename: source/section-1.ptx
-Comment: 
-
 Filename: source/section-2.ptx
 Comment: 
 
 Filename: .devcontainer/devcontainer.json
 Comment: 
 
+Filename: publication/publication.ptx
+Comment: 
+
 Zip file comment:
```

### Comparing `pretext-1.6.1.dev20230614/pretext/templates/resources/book.zip` & `pretext-1.6.1.dev20230616/pretext/templates/resources/book.zip`

 * *Files 8% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 7570 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-14 06:19 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-14 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-14 06:19 project.ptx
--rw-r--r--  2.0 unx       82 b- defN 23-Jun-14 06:19 README.md
--rw-r--r--  2.0 unx     6114 b- defN 23-Jun-14 06:19 publication/publication.ptx
--rw-r--r--  2.0 unx     1767 b- defN 23-Jun-14 06:19 source/main.ptx
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-14 06:19 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:19 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:18 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-16 06:19 .gitignore
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-16 06:18 README.md
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-16 06:19 codechat_config.yaml
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-16 06:19 project.ptx
+-rw-r--r--  2.0 unx     1767 b- defN 23-Jun-16 06:18 source/main.ptx
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-16 06:19 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx     6114 b- defN 23-Jun-16 06:18 publication/publication.ptx
 10 files, 15676 bytes uncompressed, 6476 bytes compressed:  58.7%
```

#### zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: source/
 Comment: 
 
 Filename: .gitignore
 Comment: 
 
-Filename: codechat_config.yaml
-Comment: 
-
-Filename: project.ptx
+Filename: README.md
 Comment: 
 
-Filename: README.md
+Filename: codechat_config.yaml
 Comment: 
 
-Filename: publication/publication.ptx
+Filename: project.ptx
 Comment: 
 
 Filename: source/main.ptx
 Comment: 
 
 Filename: .devcontainer/devcontainer.json
 Comment: 
 
+Filename: publication/publication.ptx
+Comment: 
+
 Zip file comment:
```

### Comparing `pretext-1.6.1.dev20230614/pretext/templates/resources/demo.zip` & `pretext-1.6.1.dev20230616/pretext/templates/resources/demo.zip`

 * *Files 6% similar despite different names*

#### zipinfo {}

```diff
@@ -1,36 +1,36 @@
 Zip file size: 173263 bytes, number of entries: 34
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 assets/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-14 06:19 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-14 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx     1710 b- defN 23-Jun-14 06:19 project.ptx
--rw-r--r--  2.0 unx       82 b- defN 23-Jun-14 06:19 README.md
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 assets/jsxgraph/
--rw-r--r--  2.0 unx   154806 b- defN 23-Jun-14 06:19 assets/frog.jpg
--rw-r--r--  2.0 unx     1737 b- defN 23-Jun-14 06:19 assets/jsxgraph/infinity.js
--rw-r--r--  2.0 unx     6092 b- defN 23-Jun-14 06:19 publication/publication.ptx
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 source/images/
--rw-r--r--  2.0 unx      867 b- defN 23-Jun-14 06:19 source/sec-features.ptx
--rw-r--r--  2.0 unx      411 b- defN 23-Jun-14 06:19 source/fig-sage3d.ptx
--rw-r--r--  2.0 unx     2080 b- defN 23-Jun-14 06:19 source/frontmatter.ptx
--rw-r--r--  2.0 unx     1515 b- defN 23-Jun-14 06:19 source/ex-first.ptx
--rw-r--r--  2.0 unx     1115 b- defN 23-Jun-14 06:19 source/ch-first with spaces.ptx
--rw-r--r--  2.0 unx     2517 b- defN 23-Jun-14 06:19 source/main.ptx
--rw-r--r--  2.0 unx     3036 b- defN 23-Jun-14 06:19 source/ch-generate.ptx
--rw-r--r--  2.0 unx      885 b- defN 23-Jun-14 06:19 source/backmatter.ptx
--rw-r--r--  2.0 unx      375 b- defN 23-Jun-14 06:19 source/fig-sage2d.ptx
--rw-r--r--  2.0 unx     1697 b- defN 23-Jun-14 06:19 source/sec-first-examples.ptx
--rw-r--r--  2.0 unx      847 b- defN 23-Jun-14 06:19 source/sec-first-intro.ptx
--rw-r--r--  2.0 unx      339 b- defN 23-Jun-14 06:19 source/ch-features.ptx
--rw-r--r--  2.0 unx      335 b- defN 23-Jun-14 06:19 source/fig-asymptote.ptx
--rw-r--r--  2.0 unx      381 b- defN 23-Jun-14 06:19 source/fig-tikz.ptx
--rw-r--r--  2.0 unx      230 b- defN 23-Jun-14 06:19 source/ch-empty.ptx
--rw-r--r--  2.0 unx     1616 b- defN 23-Jun-14 06:19 source/docinfo.ptx
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-14 06:19 source/images/sageplot2d.sage
--rw-r--r--  2.0 unx      357 b- defN 23-Jun-14 06:19 source/images/tikz.tex
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-14 06:19 source/images/sageplot3d.sage
--rw-r--r--  2.0 unx      835 b- defN 23-Jun-14 06:19 source/images/cflag.asy
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-14 06:19 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:19 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:18 assets/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:18 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-16 06:19 .gitignore
+-rw-r--r--  2.0 unx       82 b- defN 23-Jun-16 06:18 README.md
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-16 06:19 codechat_config.yaml
+-rw-r--r--  2.0 unx     1710 b- defN 23-Jun-16 06:19 project.ptx
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:18 assets/jsxgraph/
+-rw-r--r--  2.0 unx   154806 b- defN 23-Jun-16 06:18 assets/frog.jpg
+-rw-r--r--  2.0 unx     1737 b- defN 23-Jun-16 06:18 assets/jsxgraph/infinity.js
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:18 source/images/
+-rw-r--r--  2.0 unx      375 b- defN 23-Jun-16 06:18 source/fig-sage2d.ptx
+-rw-r--r--  2.0 unx      411 b- defN 23-Jun-16 06:18 source/fig-sage3d.ptx
+-rw-r--r--  2.0 unx     1697 b- defN 23-Jun-16 06:18 source/sec-first-examples.ptx
+-rw-r--r--  2.0 unx      230 b- defN 23-Jun-16 06:18 source/ch-empty.ptx
+-rw-r--r--  2.0 unx     2517 b- defN 23-Jun-16 06:18 source/main.ptx
+-rw-r--r--  2.0 unx     1515 b- defN 23-Jun-16 06:18 source/ex-first.ptx
+-rw-r--r--  2.0 unx      847 b- defN 23-Jun-16 06:18 source/sec-first-intro.ptx
+-rw-r--r--  2.0 unx     1616 b- defN 23-Jun-16 06:18 source/docinfo.ptx
+-rw-r--r--  2.0 unx      339 b- defN 23-Jun-16 06:18 source/ch-features.ptx
+-rw-r--r--  2.0 unx      335 b- defN 23-Jun-16 06:18 source/fig-asymptote.ptx
+-rw-r--r--  2.0 unx     3036 b- defN 23-Jun-16 06:18 source/ch-generate.ptx
+-rw-r--r--  2.0 unx      867 b- defN 23-Jun-16 06:18 source/sec-features.ptx
+-rw-r--r--  2.0 unx      381 b- defN 23-Jun-16 06:18 source/fig-tikz.ptx
+-rw-r--r--  2.0 unx      885 b- defN 23-Jun-16 06:18 source/backmatter.ptx
+-rw-r--r--  2.0 unx     2080 b- defN 23-Jun-16 06:18 source/frontmatter.ptx
+-rw-r--r--  2.0 unx     1115 b- defN 23-Jun-16 06:18 source/ch-first with spaces.ptx
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-16 06:18 source/images/sageplot3d.sage
+-rw-r--r--  2.0 unx      835 b- defN 23-Jun-16 06:18 source/images/cflag.asy
+-rw-r--r--  2.0 unx      357 b- defN 23-Jun-16 06:18 source/images/tikz.tex
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-16 06:18 source/images/sageplot2d.sage
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-16 06:19 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx     6092 b- defN 23-Jun-16 06:18 publication/publication.ptx
 34 files, 189971 bytes uncompressed, 169307 bytes compressed:  10.9%
```

#### zipnote {}

```diff
@@ -9,95 +9,95 @@
 
 Filename: source/
 Comment: 
 
 Filename: .gitignore
 Comment: 
 
-Filename: codechat_config.yaml
+Filename: README.md
 Comment: 
 
-Filename: project.ptx
+Filename: codechat_config.yaml
 Comment: 
 
-Filename: README.md
+Filename: project.ptx
 Comment: 
 
 Filename: assets/jsxgraph/
 Comment: 
 
 Filename: assets/frog.jpg
 Comment: 
 
 Filename: assets/jsxgraph/infinity.js
 Comment: 
 
-Filename: publication/publication.ptx
-Comment: 
-
 Filename: source/images/
 Comment: 
 
-Filename: source/sec-features.ptx
+Filename: source/fig-sage2d.ptx
 Comment: 
 
 Filename: source/fig-sage3d.ptx
 Comment: 
 
-Filename: source/frontmatter.ptx
-Comment: 
-
-Filename: source/ex-first.ptx
+Filename: source/sec-first-examples.ptx
 Comment: 
 
-Filename: source/ch-first with spaces.ptx
+Filename: source/ch-empty.ptx
 Comment: 
 
 Filename: source/main.ptx
 Comment: 
 
-Filename: source/ch-generate.ptx
+Filename: source/ex-first.ptx
 Comment: 
 
-Filename: source/backmatter.ptx
+Filename: source/sec-first-intro.ptx
 Comment: 
 
-Filename: source/fig-sage2d.ptx
+Filename: source/docinfo.ptx
 Comment: 
 
-Filename: source/sec-first-examples.ptx
+Filename: source/ch-features.ptx
 Comment: 
 
-Filename: source/sec-first-intro.ptx
+Filename: source/fig-asymptote.ptx
 Comment: 
 
-Filename: source/ch-features.ptx
+Filename: source/ch-generate.ptx
 Comment: 
 
-Filename: source/fig-asymptote.ptx
+Filename: source/sec-features.ptx
 Comment: 
 
 Filename: source/fig-tikz.ptx
 Comment: 
 
-Filename: source/ch-empty.ptx
-Comment: 
-
-Filename: source/docinfo.ptx
+Filename: source/backmatter.ptx
 Comment: 
 
-Filename: source/images/sageplot2d.sage
+Filename: source/frontmatter.ptx
 Comment: 
 
-Filename: source/images/tikz.tex
+Filename: source/ch-first with spaces.ptx
 Comment: 
 
 Filename: source/images/sageplot3d.sage
 Comment: 
 
 Filename: source/images/cflag.asy
 Comment: 
 
+Filename: source/images/tikz.tex
+Comment: 
+
+Filename: source/images/sageplot2d.sage
+Comment: 
+
 Filename: .devcontainer/devcontainer.json
 Comment: 
 
+Filename: publication/publication.ptx
+Comment: 
+
 Zip file comment:
```

### Comparing `pretext-1.6.1.dev20230614/pretext/templates/resources/devcontainer.json` & `pretext-1.6.1.dev20230616/pretext/templates/resources/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230614/pretext/templates/resources/hello.zip` & `pretext-1.6.1.dev20230616/pretext/templates/resources/hello.zip`

 * *Files 9% similar despite different names*

#### zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 4611 bytes, number of entries: 10
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 source/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-14 06:19 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-14 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx     1217 b- defN 23-Jun-14 06:19 project.ptx
--rw-r--r--  2.0 unx       69 b- defN 23-Jun-14 06:19 README.md
--rw-r--r--  2.0 unx      242 b- defN 23-Jun-14 06:19 publication/publication.ptx
--rw-r--r--  2.0 unx      156 b- defN 23-Jun-14 06:19 source/main.ptx
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-14 06:19 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:19 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:18 source/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-16 06:19 .gitignore
+-rw-r--r--  2.0 unx       69 b- defN 23-Jun-16 06:18 README.md
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-16 06:19 codechat_config.yaml
+-rw-r--r--  2.0 unx     1217 b- defN 23-Jun-16 06:18 project.ptx
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-16 06:18 source/main.ptx
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-16 06:19 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx      242 b- defN 23-Jun-16 06:18 publication/publication.ptx
 10 files, 7687 bytes uncompressed, 3517 bytes compressed:  54.2%
```

#### zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: source/
 Comment: 
 
 Filename: .gitignore
 Comment: 
 
-Filename: codechat_config.yaml
-Comment: 
-
-Filename: project.ptx
+Filename: README.md
 Comment: 
 
-Filename: README.md
+Filename: codechat_config.yaml
 Comment: 
 
-Filename: publication/publication.ptx
+Filename: project.ptx
 Comment: 
 
 Filename: source/main.ptx
 Comment: 
 
 Filename: .devcontainer/devcontainer.json
 Comment: 
 
+Filename: publication/publication.ptx
+Comment: 
+
 Zip file comment:
```

### Comparing `pretext-1.6.1.dev20230614/pretext/templates/resources/project.ptx` & `pretext-1.6.1.dev20230616/pretext/templates/resources/project.ptx`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230614/pretext/templates/resources/slideshow.zip` & `pretext-1.6.1.dev20230616/pretext/templates/resources/slideshow.zip`

 * *Files 11% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 8346 bytes, number of entries: 11
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 .devcontainer/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 publication/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 source/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-14 06:19 xsl/
--rw-r--r--  2.0 unx     1676 b- defN 23-Jun-14 06:19 .gitignore
--rw-r--r--  2.0 unx     2268 b- defN 23-Jun-14 06:19 codechat_config.yaml
--rw-r--r--  2.0 unx      784 b- defN 23-Jun-14 06:19 project.ptx
--rw-r--r--  2.0 unx      190 b- defN 23-Jun-14 06:19 xsl/slides.xsl
--rw-r--r--  2.0 unx     2097 b- defN 23-Jun-14 06:19 publication/publication.ptx
--rw-r--r--  2.0 unx    11200 b- defN 23-Jun-14 06:19 source/main.ptx
--rw-r--r--  2.0 unx     2059 b- defN 23-Jun-14 06:19 .devcontainer/devcontainer.json
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:19 .devcontainer/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:18 publication/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:18 source/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-16 06:18 xsl/
+-rw-r--r--  2.0 unx     1676 b- defN 23-Jun-16 06:19 .gitignore
+-rw-r--r--  2.0 unx     2268 b- defN 23-Jun-16 06:19 codechat_config.yaml
+-rw-r--r--  2.0 unx      784 b- defN 23-Jun-16 06:18 project.ptx
+-rw-r--r--  2.0 unx    11200 b- defN 23-Jun-16 06:18 source/main.ptx
+-rw-r--r--  2.0 unx      190 b- defN 23-Jun-16 06:18 xsl/slides.xsl
+-rw-r--r--  2.0 unx     2059 b- defN 23-Jun-16 06:19 .devcontainer/devcontainer.json
+-rw-r--r--  2.0 unx     2097 b- defN 23-Jun-16 06:18 publication/publication.ptx
 11 files, 20274 bytes uncompressed, 7158 bytes compressed:  64.7%
```

#### zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: codechat_config.yaml
 Comment: 
 
 Filename: project.ptx
 Comment: 
 
-Filename: xsl/slides.xsl
+Filename: source/main.ptx
 Comment: 
 
-Filename: publication/publication.ptx
+Filename: xsl/slides.xsl
 Comment: 
 
-Filename: source/main.ptx
+Filename: .devcontainer/devcontainer.json
 Comment: 
 
-Filename: .devcontainer/devcontainer.json
+Filename: publication/publication.ptx
 Comment: 
 
 Zip file comment:
```

### Comparing `pretext-1.6.1.dev20230614/pretext/utils.py` & `pretext-1.6.1.dev20230616/pretext/utils.py`

 * *Files identical despite different names*

### Comparing `pretext-1.6.1.dev20230614/pyproject.toml` & `pretext-1.6.1.dev20230616/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pretext"
-version = "1.6.1.dev20230614"
+version = "1.6.1.dev20230616"
 description = "A package to author, build, and deploy PreTeXt projects."
 readme = "README.md"
 homepage = "https://pretextbook.org"
 repository = "https://github.com/PreTeXtBook/pretext-cli"
 authors = ["Oscar Levin <oscar.levin@unco.edu>", "Steven Clontz <steven.clontz@gmail.com>",]
 license = "GPL-3.0-or-later"
 include = [
```

### Comparing `pretext-1.6.1.dev20230614/PKG-INFO` & `pretext-1.6.1.dev20230616/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretext
-Version: 1.6.1.dev20230614
+Version: 1.6.1.dev20230616
 Summary: A package to author, build, and deploy PreTeXt projects.
 Home-page: https://pretextbook.org
 License: GPL-3.0-or-later
 Author: Oscar Levin
 Author-email: oscar.levin@unco.edu
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

