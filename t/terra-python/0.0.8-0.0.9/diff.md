# Comparing `tmp/terra-python-0.0.8.tar.gz` & `tmp/terra-python-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terra-python-0.0.8.tar", last modified: Fri Mar 24 00:31:31 2023, max compression
+gzip compressed data, was "terra-python-0.0.9.tar", last modified: Mon May 22 16:00:44 2023, max compression
```

## Comparing `terra-python-0.0.8.tar` & `terra-python-0.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 00:31:31.862718 terra-python-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-24 00:31:21.000000 terra-python-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-24 00:31:21.000000 terra-python-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-03-24 00:31:31.862718 terra-python-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-03-24 00:31:21.000000 terra-python-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-24 00:31:21.000000 terra-python-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-24 00:31:21.000000 terra-python-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-24 00:31:31.866718 terra-python-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-03-24 00:31:21.000000 terra-python-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 00:31:31.858718 terra-python-0.0.8/terra/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-03-24 00:31:21.000000 terra-python-0.0.8/terra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 00:31:31.858718 terra-python-0.0.8/terra/api/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-24 00:31:21.000000 terra-python-0.0.8/terra/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-03-24 00:31:21.000000 terra-python-0.0.8/terra/api/api_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)    20429 2023-03-24 00:31:21.000000 terra-python-0.0.8/terra/base_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-03-24 00:31:21.000000 terra-python-0.0.8/terra/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-03-24 00:31:21.000000 terra-python-0.0.8/terra/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 00:31:31.862718 terra-python-0.0.8/terra/models/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-03-24 00:31:21.000000 terra-python-0.0.8/terra/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-03-24 00:31:21.000000 terra-python-0.0.8/terra/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-03-24 00:31:21.000000 terra-python-0.0.8/terra/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 00:31:31.862718 terra-python-0.0.8/terra/models/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-03-24 00:31:21.000000 terra-python-0.0.8/terra/models/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-03-24 00:31:21.000000 terra-python-0.0.8/terra/models/v2/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-03-24 00:31:21.000000 terra-python-0.0.8/terra/models/v2/activity_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-03-24 00:31:21.000000 terra-python-0.0.8/terra/models/v2/athlete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-03-24 00:31:21.000000 terra-python-0.0.8/terra/models/v2/body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-03-24 00:31:21.000000 terra-python-0.0.8/terra/models/v2/daily.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-03-24 00:31:21.000000 terra-python-0.0.8/terra/models/v2/menstruation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-03-24 00:31:21.000000 terra-python-0.0.8/terra/models/v2/nutrition.py
--rw-r--r--   0 runner    (1001) docker     (123)    13372 2023-03-24 00:31:21.000000 terra-python-0.0.8/terra/models/v2/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-03-24 00:31:21.000000 terra-python-0.0.8/terra/models/v2/sleep.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 00:31:21.000000 terra-python-0.0.8/terra/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-03-24 00:31:21.000000 terra-python-0.0.8/terra/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 00:31:31.862718 terra-python-0.0.8/terra_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-03-24 00:31:31.000000 terra-python-0.0.8/terra_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-24 00:31:31.000000 terra-python-0.0.8/terra_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 00:31:31.000000 terra-python-0.0.8/terra_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 00:31:31.000000 terra-python-0.0.8/terra_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-24 00:31:31.000000 terra-python-0.0.8/terra_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-24 00:31:31.000000 terra-python-0.0.8/terra_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:00:44.853447 terra-python-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 16:00:36.000000 terra-python-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-22 16:00:36.000000 terra-python-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-22 16:00:44.853447 terra-python-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-22 16:00:36.000000 terra-python-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 16:00:36.000000 terra-python-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-22 16:00:36.000000 terra-python-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 16:00:44.857447 terra-python-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-22 16:00:36.000000 terra-python-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:00:44.849447 terra-python-0.0.9/terra/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-22 16:00:36.000000 terra-python-0.0.9/terra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:00:44.849447 terra-python-0.0.9/terra/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-22 16:00:36.000000 terra-python-0.0.9/terra/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-05-22 16:00:36.000000 terra-python-0.0.9/terra/api/api_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21545 2023-05-22 16:00:36.000000 terra-python-0.0.9/terra/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-22 16:00:36.000000 terra-python-0.0.9/terra/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-22 16:00:36.000000 terra-python-0.0.9/terra/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:00:44.849447 terra-python-0.0.9/terra/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-22 16:00:36.000000 terra-python-0.0.9/terra/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-05-22 16:00:36.000000 terra-python-0.0.9/terra/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-05-22 16:00:36.000000 terra-python-0.0.9/terra/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:00:44.853447 terra-python-0.0.9/terra/models/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-22 16:00:36.000000 terra-python-0.0.9/terra/models/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13079 2023-05-22 16:00:36.000000 terra-python-0.0.9/terra/models/v2/activity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-22 16:00:36.000000 terra-python-0.0.9/terra/models/v2/activity_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-22 16:00:36.000000 terra-python-0.0.9/terra/models/v2/athlete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-05-22 16:00:36.000000 terra-python-0.0.9/terra/models/v2/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-05-22 16:00:36.000000 terra-python-0.0.9/terra/models/v2/daily.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-22 16:00:36.000000 terra-python-0.0.9/terra/models/v2/menstruation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-05-22 16:00:36.000000 terra-python-0.0.9/terra/models/v2/nutrition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13372 2023-05-22 16:00:36.000000 terra-python-0.0.9/terra/models/v2/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-05-22 16:00:36.000000 terra-python-0.0.9/terra/models/v2/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:00:36.000000 terra-python-0.0.9/terra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-22 16:00:36.000000 terra-python-0.0.9/terra/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:00:44.853447 terra-python-0.0.9/terra_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-22 16:00:44.000000 terra-python-0.0.9/terra_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-22 16:00:44.000000 terra-python-0.0.9/terra_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:00:44.000000 terra-python-0.0.9/terra_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:00:44.000000 terra-python-0.0.9/terra_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 16:00:44.000000 terra-python-0.0.9/terra_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-22 16:00:44.000000 terra-python-0.0.9/terra_python.egg-info/top_level.txt
```

### Comparing `terra-python-0.0.8/LICENSE` & `terra-python-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `terra-python-0.0.8/PKG-INFO` & `terra-python-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terra-python
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python wrapper for the Terra API
 Home-page: https://github.com/tryterra/terra-client-python
 Author: Terra Enabling Developers
 Author-email: dev@tryterra.co
 License: APACHE-2.0-ONLY
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `terra-python-0.0.8/README.md` & `terra-python-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `terra-python-0.0.8/setup.py` & `terra-python-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `terra-python-0.0.8/terra/__init__.py` & `terra-python-0.0.9/terra/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 from terra import constants
 from terra import exceptions
 from terra import models
 from terra import utils
 from terra.base_client import *
 from terra.exceptions import *
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
```

### Comparing `terra-python-0.0.8/terra/api/__init__.py` & `terra-python-0.0.9/terra/api/__init__.py`

 * *Files identical despite different names*

### Comparing `terra-python-0.0.8/terra/api/api_responses.py` & `terra-python-0.0.9/terra/api/api_responses.py`

 * *Files identical despite different names*

### Comparing `terra-python-0.0.8/terra/base_client.py` & `terra-python-0.0.9/terra/base_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -102,122 +102,134 @@
 
     def get_activity_for_user(
         self,
         user: user_.User,
         start_date: datetime.datetime,
         end_date: typing.Optional[datetime.datetime] = None,
         to_webhook: bool = True,
+        with_samples: bool = True,
     ) -> api_responses.TerraApiResponse:
         """
         Retrieves workouts/activity data for a given User object. By default, data will be asynchronously sent to registered
         webhook URL.
 
         Args:
             user (:obj:`models.user.User`): User for whom to fetch data
             start_date (:obj:`datetime.datetime`): Datetime object for which to fetch data
             end_date:obj (:`datetime.datetime`): Optional end_date for which to fetch data - if not set, will
                 default to start_date + 24h according to current API specifications
             to_webhook (:obj:`bool`): Whether to send data to registered webhook URL or return as a response body
+            with_samples (:obj:`bool`): Whether to respond with samples (e.g heartrate samples) included or not
 
         Returns:
             :obj:`models.api_responses.TerraApiResponse`: API response object containing DataReturned parsed
                 response object if no error has occured
 
         """
         return user.get_activity(
             start_date=start_date,
             end_date=end_date if end_date is not None else None,
             to_webhook=to_webhook,
+            with_samples=with_samples,
         )
 
     def get_body_for_user(
         self,
         user: user_.User,
         start_date: datetime.datetime,
         end_date: typing.Optional[datetime.datetime] = None,
         to_webhook: bool = True,
+        with_samples: bool = True,
     ) -> api_responses.TerraApiResponse:
         """
         Retrieves body metrics data for a given User object. By default, data will be asynchronously sent to registered
         webhook URL.
 
         Args:
             user (:obj:`models.user.User`): User for whom to fetch data
             start_date (:obj:`datetime.datetime`): Datetime object for which to fetch data
             end_date:obj (:`datetime.datetime`): Optional end_date for which to fetch data - if not set, will
                 default to start_date + 24h according to current API specifications
             to_webhook (:obj:`bool`): Whether to send data to registered webhook URL or return as a response body
+            with_samples (:obj:`bool`): Whether to respond with samples (e.g heartrate samples) included or not
 
         Returns:
             :obj:`models.api_responses.TerraApiResponse`: API response object containing DataReturned parsed
                 response object if no error has occured
 
         """
         return user.get_body(
             start_date=start_date,
             end_date=end_date if end_date is not None else None,
             to_webhook=to_webhook,
+            with_samples=with_samples,
         )
 
     def get_daily_for_user(
         self,
         user: user_.User,
         start_date: datetime.datetime,
         end_date: typing.Optional[datetime.datetime] = None,
         to_webhook: bool = True,
+        with_samples: bool = True,
     ) -> api_responses.TerraApiResponse:
         """
         Retrieves daily summary data for a given User object. By default, data will be asynchronously sent to registered
         webhook URL.
 
         Args:
             user (:obj:`models.user.User`): User for whom to fetch data
             start_date (:obj:`datetime.datetime`): Datetime object for which to fetch data
             end_date:obj (:`datetime.datetime`): Optional end_date for which to fetch data - if not set, will
                 default to start_date + 24h according to current API specifications
             to_webhook (:obj:`bool`): Whether to send data to registered webhook URL or return as a response body
+            with_samples (:obj:`bool`): Whether to respond with samples (e.g heartrate samples) included or not
 
         Returns:
             :obj:`models.api_responses.TerraApiResponse`: API response object containing DataReturned parsed
                 response object if no error has occured
 
         """
         return user.get_daily(
             start_date=start_date,
             end_date=end_date if end_date is not None else None,
             to_webhook=to_webhook,
+            with_samples=with_samples,
         )
 
     def get_sleep_for_user(
         self,
         user: user_.User,
         start_date: datetime.datetime,
         end_date: typing.Optional[datetime.datetime] = None,
         to_webhook: bool = True,
+        with_samples: bool = True,
     ) -> api_responses.TerraApiResponse:
         """
         Retrieves sleep data for a given User object. By default, data will be asynchronously sent to registered
         webhook URL.
 
         Args:
             user (:obj:`models.user.User`): User for whom to fetch data
             start_date (:obj:`datetime.datetime`): Datetime object for which to fetch data
             end_date:obj (:`datetime.datetime`): Optional end_date for which to fetch data - if not set, will
                 default to start_date + 24h according to current API specifications
             to_webhook (:obj:`bool`): Whether to send data to registered webhook URL or return as a response body
+            with_samples (:obj:`bool`): Whether to respond with samples (e.g heartrate samples) included or not
 
         Returns:
             :obj:`models.api_responses.TerraApiResponse`: API response object containing DataReturned parsed
                 response object if no error has occured
 
         """
         return user.get_sleep(
             start_date=start_date,
             end_date=end_date if end_date is not None else None,
             to_webhook=to_webhook,
+            with_samples=with_samples,
         )
 
     def get_athlete_for_user(
         self,
         user: user_.User,
         to_webhook: bool = True,
     ) -> api_responses.TerraApiResponse:
@@ -238,66 +250,72 @@
 
     def get_menstruation_for_user(
         self,
         user: user_.User,
         start_date: datetime.datetime,
         end_date: typing.Optional[datetime.datetime] = None,
         to_webhook: bool = True,
+        with_samples: bool = True,
     ) -> api_responses.TerraApiResponse:
         """
         Retrieves daily summary data for a given User object. By default, data will be asynchronously sent to registered
         webhook URL.
 
         Args:
             user (:obj:`models.user.User`): User for whom to fetch data
             start_date (:obj:`datetime.datetime`): Datetime object for which to fetch data
             end_date:obj (:`datetime.datetime`): Optional end_date for which to fetch data - if not set,
                 will default to start_date + 24h according to current API specifications
             to_webhook (:obj:`bool`): Whether to send data to registered webhook URL or return as a response body
+            with_samples (:obj:`bool`): Whether to respond with samples (e.g heartrate samples) included or not
 
         Returns:
             :obj:`models.api_responses.TerraApiResponse`: API response object containing DataReturned parsed
                 response object if no error has occured
 
         """
 
         return user.get_menstruation(
             start_date=start_date,
             end_date=end_date if end_date is not None else None,
             to_webhook=to_webhook,
+            with_samples=with_samples,
         )
 
     def get_nutrition_for_user(
         self,
         user: user_.User,
         start_date: datetime.datetime,
         end_date: typing.Optional[datetime.datetime] = None,
         to_webhook: bool = True,
+        with_samples: bool = True,
     ) -> api_responses.TerraApiResponse:
         """
         Retrieves daily summary data for a given User object. By default, data will be asynchronously sent to registered
         webhook URL.
 
         Args:
             user (:obj:`models.user.User`): User for whom to fetch data
             start_date (:obj:`datetime.datetime`): Datetime object for which to fetch data
             end_date:obj (:`datetime.datetime`): Optional end_date for which to fetch data - if not set, will
                 default to start_date + 24h according to current API specifications
             to_webhook (:obj:`bool`): Whether to send data to registered webhook URL or return as a response body
+            with_samples (:obj:`bool`): Whether to respond with samples (e.g heartrate samples) included or not
 
         Returns:
             :obj:`models.api_responses.TerraApiResponse`: API response object containing DataReturned parsed
                 response object if no error has occured
 
         """
 
         return user.get_nutrition(
             start_date=start_date,
             end_date=end_date if end_date is not None else None,
             to_webhook=to_webhook,
+            with_samples=with_samples,
         )
 
     def generate_widget_session(
         self,
         providers: typing.List[str],
         auth_success_redirect_url: typing.Optional[str] = None,
         auth_failure_redirect_url: typing.Optional[str] = None,
```

### Comparing `terra-python-0.0.8/terra/constants.py` & `terra-python-0.0.9/terra/constants.py`

 * *Files identical despite different names*

### Comparing `terra-python-0.0.8/terra/exceptions.py` & `terra-python-0.0.9/terra/exceptions.py`

 * *Files identical despite different names*

### Comparing `terra-python-0.0.8/terra/models/__init__.py` & `terra-python-0.0.9/terra/models/__init__.py`

 * *Files identical despite different names*

### Comparing `terra-python-0.0.8/terra/models/base_model.py` & `terra-python-0.0.9/terra/models/base_model.py`

 * *Files identical despite different names*

### Comparing `terra-python-0.0.8/terra/models/user.py` & `terra-python-0.0.9/terra/models/user.py`

 * *Files 9% similar despite different names*

```diff
@@ -81,24 +81,26 @@
             raise exceptions.NoClientAvailable
 
     def get_activity(
         self,
         start_date: datetime.datetime,
         end_date: t.Optional[datetime.datetime] = None,
         to_webhook: bool = True,
+        with_samples: bool = True,
     ) -> api_responses.TerraApiResponse:
         """
         Retrieves workouts/activity data for a given User object. By default, data will be asynchronously sent to registered
         webhook URL.
 
         Args:
 
             start_date (:obj:`datetime.datetime`): Datetime object for which to fetch data
             end_date:obj (:`datetime.datetime`): Optional end_date for which to fetch data - if not set, will default to start_date + 24h according to current API specifications
             to_webhook (:obj:`bool`): Whether to send data to registered webhook URL or return as a response body
+            with_samples (:obj:`bool`): Whether to respond with samples (e.g heartrate samples) included or not
 
         Returns:
             :obj:`models.api_responses.TerraApiResponse`: API response object containing DataReturned parsed response object if no error has occured
 
         """
 
         if self._client is None:
@@ -106,30 +108,33 @@
 
         return self._client._get_arbitrary_data(
             dtype="activity",
             user=self,
             start_date=int(start_date.timestamp()),
             end_date=int(end_date.timestamp()) if end_date is not None else None,
             to_webhook=to_webhook,
+            with_samples=with_samples,
         )
 
     def get_body(
         self,
         start_date: datetime.datetime,
         end_date: t.Optional[datetime.datetime] = None,
         to_webhook: bool = True,
+        with_samples: bool = True,
     ) -> api_responses.TerraApiResponse:
         """
         Retrieves body metrics data for a given User object. By default, data will be asynchronously sent to registered
         webhook URL.
 
         Args:
             start_date (:obj:`datetime.datetime`): Datetime object for which to fetch data
             end_date:obj (:`datetime.datetime`): Optional end_date for which to fetch data - if not set, will default to start_date + 24h according to current API specifications
             to_webhook (:obj:`bool`): Whether to send data to registered webhook URL or return as a response body
+            with_samples (:obj:`bool`): Whether to respond with samples (e.g heartrate samples) included or not
 
         Returns:
             :obj:`models.api_responses.TerraApiResponse`: API response object containing DataReturned parsed response object if no error has occured
 
         """
 
         if self._client is None:
@@ -137,105 +142,115 @@
 
         return self._client._get_arbitrary_data(
             dtype="body",
             user=self,
             start_date=int(start_date.timestamp()),
             end_date=int(end_date.timestamp()) if end_date is not None else None,
             to_webhook=to_webhook,
+            with_samples=with_samples,
         )
 
     def get_nutrition(
         self,
         start_date: datetime.datetime,
         end_date: t.Optional[datetime.datetime] = None,
         to_webhook: bool = True,
+        with_samples: bool = True,
     ) -> api_responses.TerraApiResponse:
         """
         Retrieves nutrition data for a given User object. By default, data will be asynchronously sent to registered
         webhook URL.
 
         Args:
             start_date (:obj:`datetime.datetime`): Datetime object for which to fetch data
             end_date:obj (:`datetime.datetime`): Optional end_date for which to fetch data - if not set, will default to start_date + 24h according to current API specifications
             to_webhook (:obj:`bool`): Whether to send data to registered webhook URL or return as a response body
+            with_samples (:obj:`bool`): Whether to respond with samples (e.g heartrate samples) included or not
 
         Returns:
             :obj:`models.api_responses.TerraApiResponse`: API response object containing DataReturned parsed response object if no error has occured
 
         """
         if self._client is None:
             raise exceptions.NoClientAvailable
 
         return self._client._get_arbitrary_data(
             dtype="nutrition",
             user=self,
             start_date=int(start_date.timestamp()),
             end_date=int(end_date.timestamp()) if end_date is not None else None,
             to_webhook=to_webhook,
+            with_samples=with_samples,
         )
 
     def get_daily(
         self,
         start_date: datetime.datetime,
         end_date: t.Optional[datetime.datetime] = None,
         to_webhook: bool = True,
+        with_samples: bool = True,
     ) -> api_responses.TerraApiResponse:
         """
         Retrieves daily summary data for a given User object. By default, data will be asynchronously sent to registered
         webhook URL.
 
         Args:
             start_date (:obj:`datetime.datetime`): Datetime object for which to fetch data
             end_date:obj (:`datetime.datetime`): Optional end_date for which to fetch data - if not set, will default to start_date + 24h according to current API specifications
             to_webhook (:obj:`bool`): Whether to send data to registered webhook URL or return as a response body
+            with_samples (:obj:`bool`): Whether to respond with samples (e.g heartrate samples) included or not
 
         Returns:
             :obj:`models.api_responses.TerraApiResponse`: API response object containing DataReturned parsed response object if no error has occured
 
         """
         if self._client is None:
             raise exceptions.NoClientAvailable
 
         return self._client._get_arbitrary_data(
             dtype="daily",
             user=self,
             start_date=int(start_date.timestamp()),
             end_date=int(end_date.timestamp()) if end_date is not None else None,
             to_webhook=to_webhook,
+            with_samples=with_samples,
         )
 
     def get_sleep(
         self,
         start_date: datetime.datetime,
         end_date: t.Optional[datetime.datetime] = None,
         to_webhook: bool = True,
+        with_samples: bool = True,
     ) -> api_responses.TerraApiResponse:
         """
         Retrieves sleep data for a given User object. By default, data will be asynchronously sent to registered
         webhook URL.
 
         Args:
 
             start_date (:obj:`datetime.datetime`): Datetime object for which to fetch data
             end_date:obj (:`datetime.datetime`): Optional end_date for which to fetch data - if not set, will default to start_date + 24h according to current API specifications
             to_webhook (:obj:`bool`): Whether to send data to registered webhook URL or return as a response body
+            with_samples (:obj:`bool`): Whether to respond with samples (e.g heartrate samples) included or not
 
         Returns:
             :obj:`models.api_responses.TerraApiResponse`: API response object containing DataReturned parsed response object if no error has occured
 
         """
         if self._client is None:
             raise exceptions.NoClientAvailable
 
         return self._client._get_arbitrary_data(
             dtype="sleep",
             user=self,
             start_date=int(start_date.timestamp()),
             end_date=int(end_date.timestamp()) if end_date is not None else None,
             to_webhook=to_webhook,
+            with_samples=with_samples,
         )
 
     def get_athlete(
         self,
         to_webhook: bool = True,
     ) -> api_responses.TerraApiResponse:
         """
@@ -254,31 +269,34 @@
         return self._client._get_arbitrary_data(dtype="athlete", user=self, to_webhook=to_webhook)
 
     def get_menstruation(
         self,
         start_date: datetime.datetime,
         end_date: t.Optional[datetime.datetime] = None,
         to_webhook: bool = True,
+        with_samples: bool = True,
     ) -> api_responses.TerraApiResponse:
         """
         Retrieves daily summary data for a given User object. By default, data will be asynchronously sent to registered
         webhook URL.
 
         Args:
             start_date (:obj:`datetime.datetime`): Datetime object for which to fetch data
             end_date:obj (:`datetime.datetime`): Optional end_date for which to fetch data - if not set, will default to start_date + 24h according to current API specifications
             to_webhook (:obj:`bool`): Whether to send data to registered webhook URL or return as a response body
+            with_samples (:obj:`bool`): Whether to respond with samples (e.g heartrate samples) included or not
 
         Returns:
             :obj:`models.api_responses.TerraApiResponse`: API response object containing DataReturned parsed response object if no error has occured
 
         """
         if self._client is None:
             raise exceptions.NoClientAvailable
 
         return self._client._get_arbitrary_data(
             dtype="menstruation",
             user=self,
             start_date=int(start_date.timestamp()),
             end_date=int(end_date.timestamp()) if end_date is not None else None,
             to_webhook=to_webhook,
+            with_samples=with_samples,
         )
```

### Comparing `terra-python-0.0.8/terra/models/v2/__init__.py` & `terra-python-0.0.9/terra/models/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `terra-python-0.0.8/terra/models/v2/activity.py` & `terra-python-0.0.9/terra/models/v2/activity.py`

 * *Files identical despite different names*

### Comparing `terra-python-0.0.8/terra/models/v2/activity_sample.py` & `terra-python-0.0.9/terra/models/v2/activity_sample.py`

 * *Files identical despite different names*

### Comparing `terra-python-0.0.8/terra/models/v2/athlete.py` & `terra-python-0.0.9/terra/models/v2/athlete.py`

 * *Files identical despite different names*

### Comparing `terra-python-0.0.8/terra/models/v2/body.py` & `terra-python-0.0.9/terra/models/v2/body.py`

 * *Files identical despite different names*

### Comparing `terra-python-0.0.8/terra/models/v2/daily.py` & `terra-python-0.0.9/terra/models/v2/daily.py`

 * *Files identical despite different names*

### Comparing `terra-python-0.0.8/terra/models/v2/menstruation.py` & `terra-python-0.0.9/terra/models/v2/menstruation.py`

 * *Files identical despite different names*

### Comparing `terra-python-0.0.8/terra/models/v2/nutrition.py` & `terra-python-0.0.9/terra/models/v2/nutrition.py`

 * *Files identical despite different names*

### Comparing `terra-python-0.0.8/terra/models/v2/samples.py` & `terra-python-0.0.9/terra/models/v2/samples.py`

 * *Files identical despite different names*

### Comparing `terra-python-0.0.8/terra/models/v2/sleep.py` & `terra-python-0.0.9/terra/models/v2/sleep.py`

 * *Files identical despite different names*

### Comparing `terra-python-0.0.8/terra/utils.py` & `terra-python-0.0.9/terra/utils.py`

 * *Files identical despite different names*

### Comparing `terra-python-0.0.8/terra_python.egg-info/PKG-INFO` & `terra-python-0.0.9/terra_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terra-python
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python wrapper for the Terra API
 Home-page: https://github.com/tryterra/terra-client-python
 Author: Terra Enabling Developers
 Author-email: dev@tryterra.co
 License: APACHE-2.0-ONLY
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `terra-python-0.0.8/terra_python.egg-info/SOURCES.txt` & `terra-python-0.0.9/terra_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

