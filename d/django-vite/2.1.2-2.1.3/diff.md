# Comparing `tmp/django-vite-2.1.2.tar.gz` & `tmp/django-vite-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-vite-2.1.2.tar", last modified: Fri Jun  2 14:26:26 2023, max compression
+gzip compressed data, was "django-vite-2.1.3.tar", last modified: Fri Jun 16 07:11:23 2023, max compression
```

## Comparing `django-vite-2.1.2.tar` & `django-vite-2.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:26:26.349416 django-vite-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-02 14:26:15.000000 django-vite-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-02 14:26:15.000000 django-vite-2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-06-02 14:26:26.349416 django-vite-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-06-02 14:26:15.000000 django-vite-2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:26:26.349416 django-vite-2.1.2/django_vite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:26:15.000000 django-vite-2.1.2/django_vite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-02 14:26:15.000000 django-vite-2.1.2/django_vite/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:26:26.349416 django-vite-2.1.2/django_vite/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:26:15.000000 django-vite-2.1.2/django_vite/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17967 2023-06-02 14:26:15.000000 django-vite-2.1.2/django_vite/templatetags/django_vite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:26:26.349416 django-vite-2.1.2/django_vite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-06-02 14:26:26.000000 django-vite-2.1.2/django_vite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-02 14:26:26.000000 django-vite-2.1.2/django_vite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:26:26.000000 django-vite-2.1.2/django_vite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-02 14:26:26.000000 django-vite-2.1.2/django_vite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-02 14:26:26.000000 django-vite-2.1.2/django_vite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-02 14:26:15.000000 django-vite-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 14:26:26.349416 django-vite-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-02 14:26:15.000000 django-vite-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:11:23.513719 django-vite-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-16 07:11:12.000000 django-vite-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-16 07:11:12.000000 django-vite-2.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-06-16 07:11:23.513719 django-vite-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-06-16 07:11:12.000000 django-vite-2.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:11:23.513719 django-vite-2.1.3/django_vite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:11:12.000000 django-vite-2.1.3/django_vite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-16 07:11:12.000000 django-vite-2.1.3/django_vite/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:11:23.513719 django-vite-2.1.3/django_vite/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 07:11:12.000000 django-vite-2.1.3/django_vite/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22775 2023-06-16 07:11:12.000000 django-vite-2.1.3/django_vite/templatetags/django_vite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 07:11:23.513719 django-vite-2.1.3/django_vite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-06-16 07:11:23.000000 django-vite-2.1.3/django_vite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-16 07:11:23.000000 django-vite-2.1.3/django_vite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 07:11:23.000000 django-vite-2.1.3/django_vite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-16 07:11:23.000000 django-vite-2.1.3/django_vite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 07:11:23.000000 django-vite-2.1.3/django_vite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-16 07:11:12.000000 django-vite-2.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 07:11:23.513719 django-vite-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-06-16 07:11:12.000000 django-vite-2.1.3/setup.py
```

### Comparing `django-vite-2.1.2/LICENSE` & `django-vite-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-vite-2.1.2/PKG-INFO` & `django-vite-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vite
-Version: 2.1.2
+Version: 2.1.3
 Summary: Integration of ViteJS in a Django project.
 Home-page: https://github.com/MrBin99/django-vite
 Author: MrBin99
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires: Django (>=1.11)
 Description-Content-Type: text/markdown
```

### Comparing `django-vite-2.1.2/README.md` & `django-vite-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `django-vite-2.1.2/django_vite/apps.py` & `django-vite-2.1.3/django_vite/apps.py`

 * *Files identical despite different names*

### Comparing `django-vite-2.1.2/django_vite/templatetags/django_vite.py` & `django-vite-2.1.3/django_vite/templatetags/django_vite.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from pathlib import Path
-from typing import Dict, List
+from typing import Dict, List, Callable
 from urllib.parse import urljoin
 
 from django import template
 from django.apps import apps
 from django.conf import settings
 from django.utils.safestring import mark_safe
 
@@ -89,17 +89,18 @@
 
     def generate_vite_asset(
         self,
         path: str,
         **kwargs: Dict[str, str],
     ) -> str:
         """
-        Generates a <script> tag for this JS/TS asset and a <link> tag for
-        all of its CSS dependencies by reading the manifest
-        file (for production only).
+        Generates a <script> tag for this JS/TS asset, a <link> tag for
+        all of its CSS dependencies, and a <link modulepreload>
+        for the js dependencies, as listed in the manifest file
+        (for production only).
         In development Vite loads all by itself.
 
         Arguments:
             path {str} -- Path to a Vite JS/TS asset to include.
 
         Returns:
             str -- All tags to import this file in your HTML page.
@@ -130,31 +131,145 @@
             )
 
         tags = []
         manifest_entry = self._manifest[path]
         scripts_attrs = {"type": "module", "crossorigin": "", **kwargs}
 
         # Add dependent CSS
-        tags.extend(self._generate_css_files_of_asset(path, []))
+        tags.extend(self._load_css_files_of_asset(path, []))
 
         # Add the script by itself
         tags.append(
             DjangoViteAssetLoader._generate_script_tag(
                 DjangoViteAssetLoader._generate_production_server_url(
                     manifest_entry["file"]
                 ),
                 attrs=scripts_attrs,
             )
         )
 
+        # Preload imports
+        preload_attrs = {
+            "type": "text/javascript",
+            "crossorigin": "anonymous",
+            "rel": "modulepreload",
+            "as": "script",
+        }
+
+        for dep in manifest_entry.get("imports", []):
+            dep_manifest_entry = self._manifest[dep]
+            dep_file = dep_manifest_entry["file"]
+            url = DjangoViteAssetLoader._generate_production_server_url(
+                dep_file
+            )
+            tags.append(
+                DjangoViteAssetLoader._generate_preload_tag(
+                    url,
+                    attrs=preload_attrs,
+                )
+            )
+
         return "\n".join(tags)
 
-    def _generate_css_files_of_asset(
+    def preload_vite_asset(
+        self,
+        path: str,
+    ) -> str:
+        """
+        Generates a <link modulepreload> tag for this JS/TS asset, a
+        <link preload> tag for all of its CSS dependencies,
+        and a <link modulepreload> for the js dependencies.
+        In development this template tag renders nothing,
+        since files aren't compiled yet"
+
+        Arguments:
+            path {str} -- Path to a Vite JS/TS asset to preload.
+
+        Returns:
+            str -- All tags to preload this file in your HTML page.
+
+        Raises:
+            RuntimeError: If cannot find the file path in the
+                manifest.
+
+        Returns:
+            str -- all <link> tags to preload
+                this asset.
+        """
+        if DJANGO_VITE_DEV_MODE:
+            return ""
+
+        if not self._manifest or path not in self._manifest:
+            raise RuntimeError(
+                f"Cannot find {path} in Vite manifest "
+                f"at {DJANGO_VITE_MANIFEST_PATH}"
+            )
+
+        tags = []
+        manifest_entry = self._manifest[path]
+
+        # Add the script by itself
+        script_attrs = {
+            "type": "text/javascript",
+            "crossorigin": "anonymous",
+            "rel": "modulepreload",
+            "as": "script",
+        }
+
+        manifest_file = manifest_entry["file"]
+        url = DjangoViteAssetLoader._generate_production_server_url(
+            manifest_file
+        )
+        tags.append(
+            DjangoViteAssetLoader._generate_preload_tag(
+                url,
+                attrs=script_attrs,
+            )
+        )
+
+        # Add dependent CSS
+        tags.extend(self._preload_css_files_of_asset(path, []))
+
+        # Preload imports
+        for dep in manifest_entry.get("imports", []):
+            dep_manifest_entry = self._manifest[dep]
+            dep_file = dep_manifest_entry["file"]
+            url = DjangoViteAssetLoader._generate_production_server_url(
+                dep_file
+            )
+            tags.append(
+                DjangoViteAssetLoader._generate_preload_tag(
+                    url,
+                    attrs=script_attrs,
+                )
+            )
+
+        return "\n".join(tags)
+
+    def _preload_css_files_of_asset(
         self, path: str, already_processed: List[str]
     ) -> List[str]:
+        return self._generate_css_files_of_asset(
+            path,
+            already_processed,
+            DjangoViteAssetLoader._generate_stylesheet_preload_tag,
+        )
+
+    def _load_css_files_of_asset(
+        self, path: str, already_processed: List[str]
+    ) -> List[str]:
+        return self._generate_css_files_of_asset(
+            path,
+            already_processed,
+            DjangoViteAssetLoader._generate_stylesheet_tag,
+        )
+
+    def _generate_css_files_of_asset(
+        self, path: str, already_processed: List[str], tag_generator: Callable
+    ) -> List[str]:
         """
         Generates all CSS tags for dependencies of an asset.
 
         Arguments:
             path {str} -- Path to an asset in the 'manifest.json'.
             already_processed {list} -- List of already processed CSS file.
 
@@ -165,29 +280,27 @@
         tags = []
         manifest_entry = self._manifest[path]
 
         if "imports" in manifest_entry:
             for import_path in manifest_entry["imports"]:
                 tags.extend(
                     self._generate_css_files_of_asset(
-                        import_path, already_processed
+                        import_path, already_processed, tag_generator
                     )
                 )
 
         if "css" in manifest_entry:
             for css_path in manifest_entry["css"]:
                 if css_path not in already_processed:
                     url = (
                         DjangoViteAssetLoader._generate_production_server_url(
                             css_path
                         )
                     )
-                    tags.append(
-                        DjangoViteAssetLoader._generate_stylesheet_tag(url)
-                    )
+                    tags.append(tag_generator(url))
 
                 already_processed.append(css_path)
 
         return tags
 
     def generate_vite_asset_url(self, path: str) -> str:
         """
@@ -388,26 +501,48 @@
         )
 
         return f'<script {attrs_str} src="{src}"></script>'
 
     @staticmethod
     def _generate_stylesheet_tag(href: str) -> str:
         """
-        Generates and HTML <link> stylesheet tag for CSS.
+        Generates an HTML <link> stylesheet tag for CSS.
 
         Arguments:
             href {str} -- CSS file URL.
 
         Returns:
             str -- CSS link tag.
         """
 
         return f'<link rel="stylesheet" href="{href}" />'
 
     @staticmethod
+    def _generate_stylesheet_preload_tag(href: str) -> str:
+        """
+        Generates an HTML <link> preload tag for CSS.
+
+        Arguments:
+            href {str} -- CSS file URL.
+
+        Returns:
+            str -- CSS link tag.
+        """
+
+        return f'<link rel="preload" href="{href}" as="style" />'
+
+    @staticmethod
+    def _generate_preload_tag(href: str, attrs: Dict[str, str]) -> str:
+        attrs_str = " ".join(
+            [f'{key}="{value}"' for key, value in attrs.items()]
+        )
+
+        return f'<link href="{href}" {attrs_str} />'
+
+    @staticmethod
     def _generate_vite_server_url(path: str) -> str:
         """
         Generates an URL to and asset served by the Vite development server.
 
         Keyword Arguments:
             path {str} -- Path to the asset.
 
@@ -452,18 +587,19 @@
         Keyword Arguments:
             path {str} -- Path to the asset.
 
         Returns:
             str -- Full URL to the asset.
         """
 
-        prefix = DJANGO_VITE_STATIC_URL_PREFIX
-        if not DJANGO_VITE_STATIC_URL_PREFIX.endswith("/"):
-            prefix += "/"
-        production_server_url = urljoin(prefix, path)
+        production_server_url = path
+        if prefix := DJANGO_VITE_STATIC_URL_PREFIX:
+            if not DJANGO_VITE_STATIC_URL_PREFIX.endswith("/"):
+                prefix += "/"
+            production_server_url = urljoin(prefix, path)
 
         if apps.is_installed("django.contrib.staticfiles"):
             from django.contrib.staticfiles.storage import staticfiles_storage
 
             return staticfiles_storage.url(production_server_url)
 
         return production_server_url
@@ -491,17 +627,17 @@
 @register.simple_tag
 @mark_safe
 def vite_asset(
     path: str,
     **kwargs: Dict[str, str],
 ) -> str:
     """
-    Generates a <script> tag for this JS/TS asset and a <link> tag for
-    all of its CSS dependencies by reading the manifest
-    file (for production only).
+    Generates a <script> tag for this JS/TS asset, a <link> tag for
+    all of its CSS dependencies, and a <link rel="modulepreload">
+    for all js dependencies, as listed in the manifest file
     In development Vite loads all by itself.
 
     Arguments:
         path {str} -- Path to a Vite JS/TS asset to include.
 
     Returns:
         str -- All tags to import this file in your HTML page.
@@ -521,14 +657,42 @@
 
     assert path is not None
 
     return DjangoViteAssetLoader.instance().generate_vite_asset(path, **kwargs)
 
 
 @register.simple_tag
+@mark_safe
+def vite_preload_asset(
+    path: str,
+) -> str:
+    """
+    Generates preloadmodule tag for this JS/TS asset and preloads
+    all of its CSS and JS dependencies by reading the manifest
+    file (for production only).
+    In development does nothing.
+
+    Arguments:
+        path {str} -- Path to a Vite JS/TS asset to include.
+
+    Returns:
+        str -- All tags to import this file in your HTML page.
+
+    Raises:
+        RuntimeError: If cannot find the file path in the
+            manifest (only in production).
+
+    """
+
+    assert path is not None
+
+    return DjangoViteAssetLoader.instance().preload_vite_asset(path)
+
+
+@register.simple_tag
 def vite_asset_url(path: str) -> str:
     """
     Generates only the URL of an asset managed by ViteJS.
     Warning, this function does not generate URLs for dependant assets.
 
     Arguments:
         path {str} -- Path to a Vite asset.
```

### Comparing `django-vite-2.1.2/django_vite.egg-info/PKG-INFO` & `django-vite-2.1.3/django_vite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vite
-Version: 2.1.2
+Version: 2.1.3
 Summary: Integration of ViteJS in a Django project.
 Home-page: https://github.com/MrBin99/django-vite
 Author: MrBin99
 License: Apache License, Version 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires: Django (>=1.11)
 Description-Content-Type: text/markdown
```

### Comparing `django-vite-2.1.2/setup.py` & `django-vite-2.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     README = f.read()
 
 
 setup(
     name="django-vite",
-    version="2.1.2",
+    version="2.1.3",
     description="Integration of ViteJS in a Django project.",
     long_description=README,
     long_description_content_type="text/markdown",
     author="MrBin99",
     url="https://github.com/MrBin99/django-vite",
     license="Apache License, Version 2.0",
     include_package_data=True,
```

