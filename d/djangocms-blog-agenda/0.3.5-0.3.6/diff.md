# Comparing `tmp/djangocms-blog-agenda-0.3.5.tar.gz` & `tmp/djangocms-blog-agenda-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-blog-agenda-0.3.5.tar", last modified: Thu May 25 14:33:25 2023, max compression
+gzip compressed data, was "djangocms-blog-agenda-0.3.6.tar", last modified: Fri Jun 16 10:02:09 2023, max compression
```

## Comparing `djangocms-blog-agenda-0.3.5.tar` & `djangocms-blog-agenda-0.3.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 kapt       (501)       20        0 2023-05-25 14:33:25.068078 djangocms-blog-agenda-0.3.5/
--rw-r--r--   0 kapt       (501)       20       45 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.5/AUTHORS.md
--rw-r--r--   0 kapt       (501)       20     1318 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.5/CONTRIBUTING.md
--rw-r--r--   0 kapt       (501)       20    35149 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.5/LICENSE
--rw-r--r--   0 kapt       (501)       20      159 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.5/MANIFEST.in
--rw-r--r--   0 kapt       (501)       20     3435 2023-05-25 14:33:25.068078 djangocms-blog-agenda-0.3.5/PKG-INFO
--rw-r--r--   0 kapt       (501)       20     2682 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.5/README.md
-drwxr-xr-x   0 kapt       (501)       20        0 2023-05-25 14:33:25.063078 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/
--rw-r--r--   0 kapt       (501)       20        0 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/__init__.py
--rw-r--r--   0 kapt       (501)       20     4389 2023-05-25 06:47:09.000000 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/admin.py
--rw-r--r--   0 kapt       (501)       20     1746 2023-03-31 09:10:44.000000 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/apps.py
--rw-r--r--   0 kapt       (501)       20     2364 2023-05-25 14:32:42.000000 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/cms_plugins.py
-drwxr-xr-x   0 kapt       (501)       20        0 2023-05-25 14:33:25.058078 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/locale/
-drwxr-xr-x   0 kapt       (501)       20        0 2023-05-25 14:33:25.058078 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/locale/fr/
-drwxr-xr-x   0 kapt       (501)       20        0 2023-05-25 14:33:25.066078 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/locale/fr/LC_MESSAGES/
--rw-r--r--   0 kapt       (501)       20     1899 2023-05-25 14:31:59.000000 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 kapt       (501)       20     3995 2023-05-25 14:31:46.000000 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 kapt       (501)       20        0 2023-05-25 14:33:25.067078 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/migrations/
--rw-r--r--   0 kapt       (501)       20     1076 2023-03-30 10:38:48.000000 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/migrations/0001_initial.py
--rw-r--r--   0 kapt       (501)       20     1139 2023-03-30 14:50:16.000000 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py
--rw-r--r--   0 kapt       (501)       20        0 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/migrations/__init__.py
--rw-r--r--   0 kapt       (501)       20      765 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/misc.py
--rw-r--r--   0 kapt       (501)       20     1004 2023-05-25 14:32:42.000000 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/models.py
--rw-r--r--   0 kapt       (501)       20      672 2023-04-17 13:58:19.000000 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/patched_urls.py
-drwxr-xr-x   0 kapt       (501)       20        0 2023-05-25 14:33:25.058078 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/templates/
-drwxr-xr-x   0 kapt       (501)       20        0 2023-05-25 14:33:25.068078 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/templates/djangocms_blog_agenda/
--rw-r--r--   0 kapt       (501)       20     1341 2023-03-30 10:37:22.000000 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html
--rw-r--r--   0 kapt       (501)       20     1742 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html
--rw-r--r--   0 kapt       (501)       20     1361 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html
--rw-r--r--   0 kapt       (501)       20     1889 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html
--rw-r--r--   0 kapt       (501)       20     1285 2023-04-17 16:22:43.000000 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/views.py
-drwxr-xr-x   0 kapt       (501)       20        0 2023-05-25 14:33:25.065078 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda.egg-info/
--rw-r--r--   0 kapt       (501)       20     3435 2023-05-25 14:33:25.000000 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda.egg-info/PKG-INFO
--rw-r--r--   0 kapt       (501)       20     1102 2023-05-25 14:33:25.000000 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda.egg-info/SOURCES.txt
--rw-r--r--   0 kapt       (501)       20        1 2023-05-25 14:33:25.000000 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda.egg-info/dependency_links.txt
--rw-r--r--   0 kapt       (501)       20       15 2023-05-25 14:33:25.000000 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda.egg-info/requires.txt
--rw-r--r--   0 kapt       (501)       20       22 2023-05-25 14:33:25.000000 djangocms-blog-agenda-0.3.5/djangocms_blog_agenda.egg-info/top_level.txt
--rw-r--r--   0 kapt       (501)       20      786 2023-05-25 14:33:25.068078 djangocms-blog-agenda-0.3.5/setup.cfg
--rw-r--r--   0 kapt       (501)       20       53 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.5/setup.py
+drwxr-xr-x   0 kapt       (501)       20        0 2023-06-16 10:02:09.407899 djangocms-blog-agenda-0.3.6/
+-rw-r--r--   0 kapt       (501)       20       45 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.6/AUTHORS.md
+-rw-r--r--   0 kapt       (501)       20     1318 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.6/CONTRIBUTING.md
+-rw-r--r--   0 kapt       (501)       20    35149 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.6/LICENSE
+-rw-r--r--   0 kapt       (501)       20      159 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.6/MANIFEST.in
+-rw-r--r--   0 kapt       (501)       20     3435 2023-06-16 10:02:09.407899 djangocms-blog-agenda-0.3.6/PKG-INFO
+-rw-r--r--   0 kapt       (501)       20     2682 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.6/README.md
+drwxr-xr-x   0 kapt       (501)       20        0 2023-06-16 10:02:09.377899 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/
+-rw-r--r--   0 kapt       (501)       20        0 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/__init__.py
+-rw-r--r--   0 kapt       (501)       20     4389 2023-05-25 06:47:09.000000 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/admin.py
+-rw-r--r--   0 kapt       (501)       20     1746 2023-03-31 09:10:44.000000 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/apps.py
+-rw-r--r--   0 kapt       (501)       20     2364 2023-05-25 14:32:42.000000 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/cms_plugins.py
+drwxr-xr-x   0 kapt       (501)       20        0 2023-06-16 10:02:09.345899 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/locale/
+drwxr-xr-x   0 kapt       (501)       20        0 2023-06-16 10:02:09.346899 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/locale/fr/
+drwxr-xr-x   0 kapt       (501)       20        0 2023-06-16 10:02:09.396899 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 kapt       (501)       20     1899 2023-05-25 14:31:59.000000 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 kapt       (501)       20     3995 2023-05-25 14:31:46.000000 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 kapt       (501)       20        0 2023-06-16 10:02:09.400899 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/migrations/
+-rw-r--r--   0 kapt       (501)       20     1076 2023-03-30 10:38:48.000000 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/migrations/0001_initial.py
+-rw-r--r--   0 kapt       (501)       20     1139 2023-03-30 14:50:16.000000 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py
+-rw-r--r--   0 kapt       (501)       20        0 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/migrations/__init__.py
+-rw-r--r--   0 kapt       (501)       20      765 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/misc.py
+-rw-r--r--   0 kapt       (501)       20     1004 2023-05-25 14:32:42.000000 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/models.py
+-rw-r--r--   0 kapt       (501)       20      960 2023-06-16 10:00:24.000000 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/patched_urls.py
+drwxr-xr-x   0 kapt       (501)       20        0 2023-06-16 10:02:09.346899 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/templates/
+drwxr-xr-x   0 kapt       (501)       20        0 2023-06-16 10:02:09.406899 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/
+-rw-r--r--   0 kapt       (501)       20     1341 2023-03-30 10:37:22.000000 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html
+-rw-r--r--   0 kapt       (501)       20     1742 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html
+-rw-r--r--   0 kapt       (501)       20     1361 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html
+-rw-r--r--   0 kapt       (501)       20     1889 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html
+-rw-r--r--   0 kapt       (501)       20     1577 2023-06-16 10:00:24.000000 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/views.py
+drwxr-xr-x   0 kapt       (501)       20        0 2023-06-16 10:02:09.390899 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda.egg-info/
+-rw-r--r--   0 kapt       (501)       20     3435 2023-06-16 10:02:09.000000 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda.egg-info/PKG-INFO
+-rw-r--r--   0 kapt       (501)       20     1102 2023-06-16 10:02:09.000000 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda.egg-info/SOURCES.txt
+-rw-r--r--   0 kapt       (501)       20        1 2023-06-16 10:02:09.000000 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda.egg-info/dependency_links.txt
+-rw-r--r--   0 kapt       (501)       20       15 2023-06-16 10:02:09.000000 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda.egg-info/requires.txt
+-rw-r--r--   0 kapt       (501)       20       22 2023-06-16 10:02:09.000000 djangocms-blog-agenda-0.3.6/djangocms_blog_agenda.egg-info/top_level.txt
+-rw-r--r--   0 kapt       (501)       20      786 2023-06-16 10:02:09.408899 djangocms-blog-agenda-0.3.6/setup.cfg
+-rw-r--r--   0 kapt       (501)       20       53 2023-03-30 09:34:19.000000 djangocms-blog-agenda-0.3.6/setup.py
```

### Comparing `djangocms-blog-agenda-0.3.5/CONTRIBUTING.md` & `djangocms-blog-agenda-0.3.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.5/LICENSE` & `djangocms-blog-agenda-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.5/PKG-INFO` & `djangocms-blog-agenda-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-blog-agenda
-Version: 0.3.5
+Version: 0.3.6
 Summary: Create an agenda on top of djangocms-blog!
 Home-page: https://gitlab.com/kapt/open-source/djangocms-blog-agenda
 Author: Corentin Bettiol
 Author-email: dev@kapt.mobi
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django CMS
```

### Comparing `djangocms-blog-agenda-0.3.5/README.md` & `djangocms-blog-agenda-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/admin.py` & `djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/admin.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/apps.py` & `djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/apps.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/cms_plugins.py` & `djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.mo` & `djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.po` & `djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/migrations/0001_initial.py` & `djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py` & `djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/migrations/0002_auto_20230330_1359.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/misc.py` & `djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/misc.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/models.py` & `djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/patched_urls.py` & `djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/patched_urls.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 from django.urls import path
 from django.utils.translation import pgettext_lazy
 from djangocms_blog.urls import urlpatterns as original_patterns
 
-from .views import AgendaAndPostListView, AgendaPreviousEventsListView
+from .views import (
+    AgendaAndPostListView,
+    AgendaCategoryEntriesView,
+    AgendaPreviousEventsListView,
+    AgendaTaggedListView,
+)
 
 
 # Here are the patched urls that still includes the original urlpattern of djangocms_blog.
 # But it also adds an AgendaAndPostListView (that replace the original PostListView).
 
 urlpatterns = [
     path(
         pgettext_lazy("agenda_view_url", "archives/"),
         AgendaPreviousEventsListView.as_view(),
         name="agenda-previous-events",
     ),
     path("", AgendaAndPostListView.as_view(), name="agenda-coming-soon"),
+    path(
+        "category/<str:category>/",
+        AgendaCategoryEntriesView.as_view(),
+        name="agenda-posts-category",
+    ),
+    path("tag/<slug:tag>/", AgendaTaggedListView.as_view(), name="posts-tagged"),
     *original_patterns,
 ]
```

### Comparing `djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html` & `djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/blog_meta.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html` & `djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_detail.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html` & `djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_item.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.5/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html` & `djangocms-blog-agenda-0.3.6/djangocms_blog_agenda/templates/djangocms_blog_agenda/post_list.html`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.5/djangocms_blog_agenda.egg-info/PKG-INFO` & `djangocms-blog-agenda-0.3.6/djangocms_blog_agenda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-blog-agenda
-Version: 0.3.5
+Version: 0.3.6
 Summary: Create an agenda on top of djangocms-blog!
 Home-page: https://gitlab.com/kapt/open-source/djangocms-blog-agenda
 Author: Corentin Bettiol
 Author-email: dev@kapt.mobi
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django CMS
```

### Comparing `djangocms-blog-agenda-0.3.5/djangocms_blog_agenda.egg-info/SOURCES.txt` & `djangocms-blog-agenda-0.3.6/djangocms_blog_agenda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangocms-blog-agenda-0.3.5/setup.cfg` & `djangocms-blog-agenda-0.3.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = djangocms-blog-agenda
-version = 0.3.5
+version = 0.3.6
 description = Create an agenda on top of djangocms-blog!
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/kapt/open-source/djangocms-blog-agenda
 author = Corentin Bettiol
 author_email = dev@kapt.mobi
 classifiers =
```

