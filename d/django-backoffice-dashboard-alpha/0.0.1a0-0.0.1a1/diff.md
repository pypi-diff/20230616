# Comparing `tmp/django-backoffice-dashboard-alpha-0.0.1a0.tar.gz` & `tmp/django-backoffice-dashboard-alpha-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-backoffice-dashboard-alpha-0.0.1a0.tar", last modified: Thu Jun 15 08:19:48 2023, max compression
+gzip compressed data, was "django-backoffice-dashboard-alpha-0.0.1a1.tar", last modified: Fri Jun 16 08:10:01 2023, max compression
```

## Comparing `django-backoffice-dashboard-alpha-0.0.1a0.tar` & `django-backoffice-dashboard-alpha-0.0.1a1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-06-15 08:19:48.851953 django-backoffice-dashboard-alpha-0.0.1a0/
--rw-r--r--   0 irfanpule   (501) staff       (20)     1059 2023-06-15 07:58:56.000000 django-backoffice-dashboard-alpha-0.0.1a0/LICENSE
--rw-r--r--   0 irfanpule   (501) staff       (20)      158 2023-06-15 07:58:56.000000 django-backoffice-dashboard-alpha-0.0.1a0/MANIFEST.in
--rw-r--r--   0 irfanpule   (501) staff       (20)     3661 2023-06-15 08:19:48.851837 django-backoffice-dashboard-alpha-0.0.1a0/PKG-INFO
--rw-r--r--   0 irfanpule   (501) staff       (20)     2386 2023-06-15 08:15:39.000000 django-backoffice-dashboard-alpha-0.0.1a0/README.md
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-06-15 08:19:48.849220 django-backoffice-dashboard-alpha-0.0.1a0/django_backoffice_dashboard_alpha.egg-info/
--rw-r--r--   0 irfanpule   (501) staff       (20)     3661 2023-06-15 08:19:48.000000 django-backoffice-dashboard-alpha-0.0.1a0/django_backoffice_dashboard_alpha.egg-info/PKG-INFO
--rw-r--r--   0 irfanpule   (501) staff       (20)      667 2023-06-15 08:19:48.000000 django-backoffice-dashboard-alpha-0.0.1a0/django_backoffice_dashboard_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 irfanpule   (501) staff       (20)        1 2023-06-15 08:19:48.000000 django-backoffice-dashboard-alpha-0.0.1a0/django_backoffice_dashboard_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 irfanpule   (501) staff       (20)        1 2023-06-15 08:19:48.000000 django-backoffice-dashboard-alpha-0.0.1a0/django_backoffice_dashboard_alpha.egg-info/not-zip-safe
--rw-r--r--   0 irfanpule   (501) staff       (20)       17 2023-06-15 08:19:48.000000 django-backoffice-dashboard-alpha-0.0.1a0/django_backoffice_dashboard_alpha.egg-info/requires.txt
--rw-r--r--   0 irfanpule   (501) staff       (20)       37 2023-06-15 08:19:48.000000 django-backoffice-dashboard-alpha-0.0.1a0/django_backoffice_dashboard_alpha.egg-info/top_level.txt
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-06-15 08:19:48.851520 django-backoffice-dashboard-alpha-0.0.1a0/djbackoffice/
--rw-r--r--   0 irfanpule   (501) staff       (20)      402 2023-06-15 08:19:20.000000 django-backoffice-dashboard-alpha-0.0.1a0/djbackoffice/__init__.py
--rw-r--r--   0 irfanpule   (501) staff       (20)      237 2023-06-15 07:58:56.000000 django-backoffice-dashboard-alpha-0.0.1a0/djbackoffice/apps.py
--rw-r--r--   0 irfanpule   (501) staff       (20)     8795 2023-06-15 07:58:56.000000 django-backoffice-dashboard-alpha-0.0.1a0/djbackoffice/core.py
--rw-r--r--   0 irfanpule   (501) staff       (20)      611 2023-06-15 07:58:56.000000 django-backoffice-dashboard-alpha-0.0.1a0/djbackoffice/decorators.py
-drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-06-15 08:19:48.851666 django-backoffice-dashboard-alpha-0.0.1a0/djbackoffice/migrations/
--rw-r--r--   0 irfanpule   (501) staff       (20)        0 2023-06-15 07:58:56.000000 django-backoffice-dashboard-alpha-0.0.1a0/djbackoffice/migrations/__init__.py
--rw-r--r--   0 irfanpule   (501) staff       (20)     4771 2023-06-15 07:58:56.000000 django-backoffice-dashboard-alpha-0.0.1a0/djbackoffice/mixin.py
--rw-r--r--   0 irfanpule   (501) staff       (20)      737 2023-06-15 07:58:56.000000 django-backoffice-dashboard-alpha-0.0.1a0/djbackoffice/models.py
--rw-r--r--   0 irfanpule   (501) staff       (20)      270 2023-06-15 07:58:56.000000 django-backoffice-dashboard-alpha-0.0.1a0/djbackoffice/settings.py
--rw-r--r--   0 irfanpule   (501) staff       (20)      230 2023-06-15 07:58:56.000000 django-backoffice-dashboard-alpha-0.0.1a0/djbackoffice/tables.py
--rw-r--r--   0 irfanpule   (501) staff       (20)       60 2023-06-15 07:58:56.000000 django-backoffice-dashboard-alpha-0.0.1a0/djbackoffice/tests.py
--rw-r--r--   0 irfanpule   (501) staff       (20)     1713 2023-06-15 07:58:56.000000 django-backoffice-dashboard-alpha-0.0.1a0/djbackoffice/utils.py
--rw-r--r--   0 irfanpule   (501) staff       (20)     4168 2023-06-15 07:58:56.000000 django-backoffice-dashboard-alpha-0.0.1a0/djbackoffice/views.py
--rw-r--r--   0 irfanpule   (501) staff       (20)       38 2023-06-15 08:19:48.851992 django-backoffice-dashboard-alpha-0.0.1a0/setup.cfg
--rw-r--r--   0 irfanpule   (501) staff       (20)     3329 2023-06-15 08:14:07.000000 django-backoffice-dashboard-alpha-0.0.1a0/setup.py
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-06-16 08:10:01.282813 django-backoffice-dashboard-alpha-0.0.1a1/
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1059 2023-06-15 07:58:56.000000 django-backoffice-dashboard-alpha-0.0.1a1/LICENSE
+-rw-r--r--   0 irfanpule   (501) staff       (20)      158 2023-06-15 07:58:56.000000 django-backoffice-dashboard-alpha-0.0.1a1/MANIFEST.in
+-rw-r--r--   0 irfanpule   (501) staff       (20)     3800 2023-06-16 08:10:01.282649 django-backoffice-dashboard-alpha-0.0.1a1/PKG-INFO
+-rw-r--r--   0 irfanpule   (501) staff       (20)     2525 2023-06-16 04:20:44.000000 django-backoffice-dashboard-alpha-0.0.1a1/README.md
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-06-16 08:10:01.277090 django-backoffice-dashboard-alpha-0.0.1a1/django_backoffice_dashboard_alpha.egg-info/
+-rw-r--r--   0 irfanpule   (501) staff       (20)     3800 2023-06-16 08:10:01.000000 django-backoffice-dashboard-alpha-0.0.1a1/django_backoffice_dashboard_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 irfanpule   (501) staff       (20)      667 2023-06-16 08:10:01.000000 django-backoffice-dashboard-alpha-0.0.1a1/django_backoffice_dashboard_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 irfanpule   (501) staff       (20)        1 2023-06-16 08:10:01.000000 django-backoffice-dashboard-alpha-0.0.1a1/django_backoffice_dashboard_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 irfanpule   (501) staff       (20)        1 2023-06-15 08:19:48.000000 django-backoffice-dashboard-alpha-0.0.1a1/django_backoffice_dashboard_alpha.egg-info/not-zip-safe
+-rw-r--r--   0 irfanpule   (501) staff       (20)       17 2023-06-16 08:10:01.000000 django-backoffice-dashboard-alpha-0.0.1a1/django_backoffice_dashboard_alpha.egg-info/requires.txt
+-rw-r--r--   0 irfanpule   (501) staff       (20)       37 2023-06-16 08:10:01.000000 django-backoffice-dashboard-alpha-0.0.1a1/django_backoffice_dashboard_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-06-16 08:10:01.282163 django-backoffice-dashboard-alpha-0.0.1a1/djbackoffice/
+-rw-r--r--   0 irfanpule   (501) staff       (20)      355 2023-06-16 08:09:49.000000 django-backoffice-dashboard-alpha-0.0.1a1/djbackoffice/__init__.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      237 2023-06-15 07:58:56.000000 django-backoffice-dashboard-alpha-0.0.1a1/djbackoffice/apps.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)     8795 2023-06-15 07:58:56.000000 django-backoffice-dashboard-alpha-0.0.1a1/djbackoffice/core.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      611 2023-06-15 07:58:56.000000 django-backoffice-dashboard-alpha-0.0.1a1/djbackoffice/decorators.py
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-06-16 08:10:01.282400 django-backoffice-dashboard-alpha-0.0.1a1/djbackoffice/migrations/
+-rw-r--r--   0 irfanpule   (501) staff       (20)        0 2023-06-15 07:58:56.000000 django-backoffice-dashboard-alpha-0.0.1a1/djbackoffice/migrations/__init__.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)     4771 2023-06-15 07:58:56.000000 django-backoffice-dashboard-alpha-0.0.1a1/djbackoffice/mixin.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      737 2023-06-15 07:58:56.000000 django-backoffice-dashboard-alpha-0.0.1a1/djbackoffice/models.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      270 2023-06-15 07:58:56.000000 django-backoffice-dashboard-alpha-0.0.1a1/djbackoffice/settings.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      274 2023-06-16 08:01:53.000000 django-backoffice-dashboard-alpha-0.0.1a1/djbackoffice/tables.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)       60 2023-06-15 07:58:56.000000 django-backoffice-dashboard-alpha-0.0.1a1/djbackoffice/tests.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1713 2023-06-15 07:58:56.000000 django-backoffice-dashboard-alpha-0.0.1a1/djbackoffice/utils.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)     4168 2023-06-16 08:00:16.000000 django-backoffice-dashboard-alpha-0.0.1a1/djbackoffice/views.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)       38 2023-06-16 08:10:01.282858 django-backoffice-dashboard-alpha-0.0.1a1/setup.cfg
+-rw-r--r--   0 irfanpule   (501) staff       (20)     3137 2023-06-16 03:19:20.000000 django-backoffice-dashboard-alpha-0.0.1a1/setup.py
```

### Comparing `django-backoffice-dashboard-alpha-0.0.1a0/LICENSE` & `django-backoffice-dashboard-alpha-0.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-backoffice-dashboard-alpha-0.0.1a0/PKG-INFO` & `django-backoffice-dashboard-alpha-0.0.1a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-backoffice-dashboard-alpha
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: A simple Django app to build backoffice dashboard
 Home-page: https://github.com/irfanpule/django-backoffice-dashboard
 Author: irfanpule
 Author-email: irfan.pule2@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -33,30 +33,33 @@
 # Django Backoffice Dashboard
 
 Django Backoffice is an application Django to easier create backoffice dashboard integrated for your project.
 ![img](https://github.com/irfanpule/django-backoffice-dashboard/raw/main/docs/screnshots/ss1.png?raw=true)
  
 ## Installation
 - Install django-backoffice using:
-    ```
+    ```bash
     pip install django-backoffice-dashboard-alpha
     ```
 
 - Add `djbackoffice` to your `INSTALLED_APPS` setting like this
-    ```
+    ```python
     INSTALLED_APPS = [
-        ...
+        # ... other apps
+  
         'djbackoffice',
+        'sweetify',  # djbackoffice need it
+        'django_tables2' # djbackoffice need it
     ]
     ```
 - Run `python manage.py collectstatic` to collect file static djbackoffice into project.
 - Include url `djbackoffice` in your root url
-    ```
+    ```python
     from djbackoffice.core import backoffice
-    ....
+    # .... other import
 
     urlpatterns = [
         path('admin/', admin.site.urls),
         .....
         path('backoffice/', backoffice.urls),
     ]
     ```
```

### Comparing `django-backoffice-dashboard-alpha-0.0.1a0/README.md` & `django-backoffice-dashboard-alpha-0.0.1a1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 # Django Backoffice Dashboard
 
 Django Backoffice is an application Django to easier create backoffice dashboard integrated for your project.
 ![img](https://github.com/irfanpule/django-backoffice-dashboard/raw/main/docs/screnshots/ss1.png?raw=true)
  
 ## Installation
 - Install django-backoffice using:
-    ```
+    ```bash
     pip install django-backoffice-dashboard-alpha
     ```
 
 - Add `djbackoffice` to your `INSTALLED_APPS` setting like this
-    ```
+    ```python
     INSTALLED_APPS = [
-        ...
+        # ... other apps
+  
         'djbackoffice',
+        'sweetify',  # djbackoffice need it
+        'django_tables2' # djbackoffice need it
     ]
     ```
 - Run `python manage.py collectstatic` to collect file static djbackoffice into project.
 - Include url `djbackoffice` in your root url
-    ```
+    ```python
     from djbackoffice.core import backoffice
-    ....
+    # .... other import
 
     urlpatterns = [
         path('admin/', admin.site.urls),
         .....
         path('backoffice/', backoffice.urls),
     ]
     ```
```

### Comparing `django-backoffice-dashboard-alpha-0.0.1a0/django_backoffice_dashboard_alpha.egg-info/PKG-INFO` & `django-backoffice-dashboard-alpha-0.0.1a1/django_backoffice_dashboard_alpha.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-backoffice-dashboard-alpha
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: A simple Django app to build backoffice dashboard
 Home-page: https://github.com/irfanpule/django-backoffice-dashboard
 Author: irfanpule
 Author-email: irfan.pule2@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -33,30 +33,33 @@
 # Django Backoffice Dashboard
 
 Django Backoffice is an application Django to easier create backoffice dashboard integrated for your project.
 ![img](https://github.com/irfanpule/django-backoffice-dashboard/raw/main/docs/screnshots/ss1.png?raw=true)
  
 ## Installation
 - Install django-backoffice using:
-    ```
+    ```bash
     pip install django-backoffice-dashboard-alpha
     ```
 
 - Add `djbackoffice` to your `INSTALLED_APPS` setting like this
-    ```
+    ```python
     INSTALLED_APPS = [
-        ...
+        # ... other apps
+  
         'djbackoffice',
+        'sweetify',  # djbackoffice need it
+        'django_tables2' # djbackoffice need it
     ]
     ```
 - Run `python manage.py collectstatic` to collect file static djbackoffice into project.
 - Include url `djbackoffice` in your root url
-    ```
+    ```python
     from djbackoffice.core import backoffice
-    ....
+    # .... other import
 
     urlpatterns = [
         path('admin/', admin.site.urls),
         .....
         path('backoffice/', backoffice.urls),
     ]
     ```
```

### Comparing `django-backoffice-dashboard-alpha-0.0.1a0/django_backoffice_dashboard_alpha.egg-info/SOURCES.txt` & `django-backoffice-dashboard-alpha-0.0.1a1/django_backoffice_dashboard_alpha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-backoffice-dashboard-alpha-0.0.1a0/djbackoffice/core.py` & `django-backoffice-dashboard-alpha-0.0.1a1/djbackoffice/core.py`

 * *Files identical despite different names*

### Comparing `django-backoffice-dashboard-alpha-0.0.1a0/djbackoffice/decorators.py` & `django-backoffice-dashboard-alpha-0.0.1a1/djbackoffice/decorators.py`

 * *Files identical despite different names*

### Comparing `django-backoffice-dashboard-alpha-0.0.1a0/djbackoffice/mixin.py` & `django-backoffice-dashboard-alpha-0.0.1a1/djbackoffice/mixin.py`

 * *Files identical despite different names*

### Comparing `django-backoffice-dashboard-alpha-0.0.1a0/djbackoffice/models.py` & `django-backoffice-dashboard-alpha-0.0.1a1/djbackoffice/models.py`

 * *Files identical despite different names*

### Comparing `django-backoffice-dashboard-alpha-0.0.1a0/djbackoffice/utils.py` & `django-backoffice-dashboard-alpha-0.0.1a1/djbackoffice/utils.py`

 * *Files identical despite different names*

### Comparing `django-backoffice-dashboard-alpha-0.0.1a0/djbackoffice/views.py` & `django-backoffice-dashboard-alpha-0.0.1a1/djbackoffice/views.py`

 * *Files identical despite different names*

### Comparing `django-backoffice-dashboard-alpha-0.0.1a0/setup.py` & `django-backoffice-dashboard-alpha-0.0.1a1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,20 +14,16 @@
     """
     Return package version as listed in `__version__` in `init.py`.
     """
     init_py = open(os.path.join(package, '__init__.py')).read()
     return re.search("__version__ = ['\"]([^'\"]+)['\"]", init_py).group(1)
 
 
-def get_name(package):
-    """
-    Return package version as listed in `__name__` in `init.py`.
-    """
-    init_py = open(os.path.join(package, '__init__.py')).read()
-    return re.search("__name__ = ['\"]([^'\"]+)['\"]", init_py).group(1)
+def get_name():
+    return 'django-backoffice-dashboard-alpha'
 
 
 def get_packages(package):
     return [
         dirpath
         for dirpath, dirnames, filenames in os.walk(package)
         if os.path.exists(os.path.join(dirpath, "__init__.py"))
@@ -62,15 +58,15 @@
 if sys.argv[-1] == 'build_pre_publish':
     build_package()
     print("The version now: ", version)
     sys.exit()
 
 
 setup(
-    name=get_name('djbackoffice'),
+    name=get_name(),
     version=version,
     url='https://github.com/irfanpule/django-backoffice-dashboard',
     license='MIT License',
     description='A simple Django app to build backoffice dashboard',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     author='irfanpule',
```

