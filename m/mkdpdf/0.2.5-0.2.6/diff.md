# Comparing `tmp/mkdpdf-0.2.5.tar.gz` & `tmp/mkdpdf-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdpdf-0.2.5.tar", last modified: Thu Jun 15 00:30:33 2023, max compression
+gzip compressed data, was "mkdpdf-0.2.6.tar", last modified: Thu Jun 15 22:11:11 2023, max compression
```

## Comparing `mkdpdf-0.2.5.tar` & `mkdpdf-0.2.6.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.477287 mkdpdf-0.2.5/
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      303 2023-06-15 00:30:33.476287 mkdpdf-0.2.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.468288 mkdpdf-0.2.5/mkdpdf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      671 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.470287 mkdpdf-0.2.5/mkdpdf/document/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/document/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12516 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/document/document.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.464288 mkdpdf-0.2.5/mkdpdf/document/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.464288 mkdpdf-0.2.5/mkdpdf/document/templates/pdf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.471288 mkdpdf-0.2.5/mkdpdf/document/templates/pdf/style/
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/document/templates/pdf/style/document.css
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/document/templates/pdf/style/footer.css
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/document/templates/pdf/style/header.css
--rw-rw-rw-   0 root         (0) root         (0)     6683 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/document/templates/pdf/style/mermaid.css
--rw-rw-rw-   0 root         (0) root         (0)     2193 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/document/templates/pdf/style/pdf.css
--rw-rw-rw-   0 root         (0) root         (0)     3199 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/document/templates/pdf/style/reset.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.471288 mkdpdf-0.2.5/mkdpdf/documentation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/documentation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8053 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/documentation/documentation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.465288 mkdpdf-0.2.5/mkdpdf/documentation/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.472288 mkdpdf-0.2.5/mkdpdf/documentation/templates/md/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.472288 mkdpdf-0.2.5/mkdpdf/documentation/templates/md/class/
--rw-rw-rw-   0 root         (0) root         (0)      564 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/documentation/templates/md/class/header.md
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/documentation/templates/md/class/main.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.472288 mkdpdf-0.2.5/mkdpdf/documentation/templates/md/functions/
--rw-rw-rw-   0 root         (0) root         (0)      517 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/documentation/templates/md/functions/header.md
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/documentation/templates/md/functions/main.md
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/documentation/templates/md/header.md
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/documentation/templates/md/main.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.465288 mkdpdf-0.2.5/mkdpdf/documentation/templates/pdf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.473287 mkdpdf-0.2.5/mkdpdf/documentation/templates/pdf/style/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/documentation/templates/pdf/style/document.css
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/documentation/templates/pdf/style/footer.css
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/documentation/templates/pdf/style/header.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.473287 mkdpdf-0.2.5/mkdpdf/md/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/md/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1298 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/md/md.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.474287 mkdpdf-0.2.5/mkdpdf/pdf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/pdf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5935 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/pdf/pdf.py
--rw-rw-rw-   0 root         (0) root         (0)     3234 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/pdf/publisher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.474287 mkdpdf-0.2.5/mkdpdf/report/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/report/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/report/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.466287 mkdpdf-0.2.5/mkdpdf/report/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.475287 mkdpdf-0.2.5/mkdpdf/report/templates/md/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/report/templates/md/footer.md
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/report/templates/md/header.md
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/report/templates/md/main.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.476287 mkdpdf-0.2.5/mkdpdf/report/templates/pdf/
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/report/templates/pdf/footer.html
--rw-rw-rw-   0 root         (0) root         (0)      809 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/report/templates/pdf/header.html
--rw-rw-rw-   0 root         (0) root         (0)     1338 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/report/templates/pdf/main.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.476287 mkdpdf-0.2.5/mkdpdf/report/templates/pdf/style/
--rw-rw-rw-   0 root         (0) root         (0)      358 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/report/templates/pdf/style/document.css
--rw-rw-rw-   0 root         (0) root         (0)      755 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/report/templates/pdf/style/footer.css
--rw-rw-rw-   0 root         (0) root         (0)     1518 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/report/templates/pdf/style/header.css
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/report/templates/pdf/style/pdf.css
--rw-rw-rw-   0 root         (0) root         (0)     1027 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/mkdpdf/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 00:30:33.469287 mkdpdf-0.2.5/mkdpdf.egg-info/
--rw-r--r--   0 root         (0) root         (0)      303 2023-06-15 00:30:33.000000 mkdpdf-0.2.5/mkdpdf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1737 2023-06-15 00:30:33.000000 mkdpdf-0.2.5/mkdpdf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 00:30:33.000000 mkdpdf-0.2.5/mkdpdf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-06-15 00:30:33.000000 mkdpdf-0.2.5/mkdpdf.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-15 00:30:33.000000 mkdpdf-0.2.5/mkdpdf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-15 00:30:33.000000 mkdpdf-0.2.5/mkdpdf.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       28 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 00:30:33.477287 mkdpdf-0.2.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      976 2023-06-15 00:30:25.000000 mkdpdf-0.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:11:11.438648 mkdpdf-0.2.6/
+-rw-rw-rw-   0 root         (0) root         (0)      147 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      303 2023-06-15 22:11:11.437648 mkdpdf-0.2.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:11:11.431648 mkdpdf-0.2.6/mkdpdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      671 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:11:11.432648 mkdpdf-0.2.6/mkdpdf/document/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/document/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12516 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/document/document.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:11:11.428648 mkdpdf-0.2.6/mkdpdf/document/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:11:11.428648 mkdpdf-0.2.6/mkdpdf/document/templates/pdf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:11:11.433648 mkdpdf-0.2.6/mkdpdf/document/templates/pdf/style/
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/document/templates/pdf/style/document.css
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/document/templates/pdf/style/footer.css
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/document/templates/pdf/style/header.css
+-rw-rw-rw-   0 root         (0) root         (0)     6683 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/document/templates/pdf/style/mermaid.css
+-rw-rw-rw-   0 root         (0) root         (0)     2193 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/document/templates/pdf/style/pdf.css
+-rw-rw-rw-   0 root         (0) root         (0)     3199 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/document/templates/pdf/style/reset.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:11:11.433648 mkdpdf-0.2.6/mkdpdf/documentation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/documentation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8053 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/documentation/documentation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:11:11.428648 mkdpdf-0.2.6/mkdpdf/documentation/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:11:11.434648 mkdpdf-0.2.6/mkdpdf/documentation/templates/md/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:11:11.434648 mkdpdf-0.2.6/mkdpdf/documentation/templates/md/class/
+-rw-rw-rw-   0 root         (0) root         (0)      564 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/documentation/templates/md/class/header.md
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/documentation/templates/md/class/main.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:11:11.434648 mkdpdf-0.2.6/mkdpdf/documentation/templates/md/functions/
+-rw-rw-rw-   0 root         (0) root         (0)      517 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/documentation/templates/md/functions/header.md
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/documentation/templates/md/functions/main.md
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/documentation/templates/md/header.md
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/documentation/templates/md/main.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:11:11.429648 mkdpdf-0.2.6/mkdpdf/documentation/templates/pdf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:11:11.435648 mkdpdf-0.2.6/mkdpdf/documentation/templates/pdf/style/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/documentation/templates/pdf/style/document.css
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/documentation/templates/pdf/style/footer.css
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/documentation/templates/pdf/style/header.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:11:11.435648 mkdpdf-0.2.6/mkdpdf/md/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/md/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1298 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/md/md.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:11:11.435648 mkdpdf-0.2.6/mkdpdf/pdf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/pdf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5935 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/pdf/pdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3234 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/pdf/publisher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:11:11.436648 mkdpdf-0.2.6/mkdpdf/report/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/report/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2025 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/report/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:11:11.429648 mkdpdf-0.2.6/mkdpdf/report/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:11:11.436648 mkdpdf-0.2.6/mkdpdf/report/templates/md/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/report/templates/md/footer.md
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/report/templates/md/header.md
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/report/templates/md/main.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:11:11.437648 mkdpdf-0.2.6/mkdpdf/report/templates/pdf/
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/report/templates/pdf/footer.html
+-rw-rw-rw-   0 root         (0) root         (0)      809 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/report/templates/pdf/header.html
+-rw-rw-rw-   0 root         (0) root         (0)     1338 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/report/templates/pdf/main.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:11:11.437648 mkdpdf-0.2.6/mkdpdf/report/templates/pdf/style/
+-rw-rw-rw-   0 root         (0) root         (0)      358 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/report/templates/pdf/style/document.css
+-rw-rw-rw-   0 root         (0) root         (0)      755 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/report/templates/pdf/style/footer.css
+-rw-rw-rw-   0 root         (0) root         (0)     1518 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/report/templates/pdf/style/header.css
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/report/templates/pdf/style/pdf.css
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/mkdpdf/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 22:11:11.432648 mkdpdf-0.2.6/mkdpdf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      303 2023-06-15 22:11:11.000000 mkdpdf-0.2.6/mkdpdf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1737 2023-06-15 22:11:11.000000 mkdpdf-0.2.6/mkdpdf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 22:11:11.000000 mkdpdf-0.2.6/mkdpdf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-06-15 22:11:11.000000 mkdpdf-0.2.6/mkdpdf.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-15 22:11:11.000000 mkdpdf-0.2.6/mkdpdf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-15 22:11:11.000000 mkdpdf-0.2.6/mkdpdf.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       28 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 22:11:11.438648 mkdpdf-0.2.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      976 2023-06-15 22:11:04.000000 mkdpdf-0.2.6/setup.py
```

### Comparing `mkdpdf-0.2.5/mkdpdf/configuration.py` & `mkdpdf-0.2.6/mkdpdf/configuration.py`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.5/mkdpdf/document/document.py` & `mkdpdf-0.2.6/mkdpdf/document/document.py`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.5/mkdpdf/document/templates/pdf/style/mermaid.css` & `mkdpdf-0.2.6/mkdpdf/document/templates/pdf/style/mermaid.css`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.5/mkdpdf/document/templates/pdf/style/pdf.css` & `mkdpdf-0.2.6/mkdpdf/document/templates/pdf/style/pdf.css`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.5/mkdpdf/document/templates/pdf/style/reset.css` & `mkdpdf-0.2.6/mkdpdf/document/templates/pdf/style/reset.css`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.5/mkdpdf/documentation/documentation.py` & `mkdpdf-0.2.6/mkdpdf/documentation/documentation.py`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.5/mkdpdf/documentation/templates/md/class/header.md` & `mkdpdf-0.2.6/mkdpdf/documentation/templates/md/class/header.md`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.5/mkdpdf/documentation/templates/md/functions/header.md` & `mkdpdf-0.2.6/mkdpdf/documentation/templates/md/functions/header.md`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.5/mkdpdf/md/md.py` & `mkdpdf-0.2.6/mkdpdf/md/md.py`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.5/mkdpdf/pdf/pdf.py` & `mkdpdf-0.2.6/mkdpdf/pdf/pdf.py`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.5/mkdpdf/pdf/publisher.py` & `mkdpdf-0.2.6/mkdpdf/pdf/publisher.py`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.5/mkdpdf/report/templates/pdf/header.html` & `mkdpdf-0.2.6/mkdpdf/report/templates/pdf/header.html`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.5/mkdpdf/report/templates/pdf/main.html` & `mkdpdf-0.2.6/mkdpdf/report/templates/pdf/main.html`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.5/mkdpdf/report/templates/pdf/style/footer.css` & `mkdpdf-0.2.6/mkdpdf/report/templates/pdf/style/footer.css`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.5/mkdpdf/report/templates/pdf/style/header.css` & `mkdpdf-0.2.6/mkdpdf/report/templates/pdf/style/header.css`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.5/mkdpdf/utilities.py` & `mkdpdf-0.2.6/mkdpdf/utilities.py`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.5/mkdpdf.egg-info/SOURCES.txt` & `mkdpdf-0.2.6/mkdpdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdpdf-0.2.5/setup.py` & `mkdpdf-0.2.6/setup.py`

 * *Files identical despite different names*

