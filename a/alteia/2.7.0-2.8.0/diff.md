# Comparing `tmp/alteia-2.7.0.tar.gz` & `tmp/alteia-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alteia-2.7.0.tar", max compression
+gzip compressed data, was "alteia-2.8.0.tar", max compression
```

## Comparing `alteia-2.7.0.tar` & `alteia-2.8.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0     1084 2023-03-14 09:06:19.364378 alteia-2.7.0/LICENSE
--rw-r--r--   0        0        0     1426 2023-03-14 09:06:19.364378 alteia-2.7.0/README.md
--rw-r--r--   0        0        0      257 2023-03-14 09:06:19.364378 alteia-2.7.0/alteia/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/analytics/__init__.py
--rw-r--r--   0        0        0    26328 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/analytics/analyticsimpl.py
--rwxr-xr-x   0        0        0    16721 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/analytics/configurationsimpl.py
--rw-r--r--   0        0        0     7927 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/analytics/productsimpl.py
--rw-r--r--   0        0        0        0 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/annotations/__init__.py
--rw-r--r--   0        0        0    30043 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/annotations/annotationsimpl.py
--rw-r--r--   0        0        0        0 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/auth/__init__.py
--rw-r--r--   0        0        0     4227 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/auth/companiesimpl.py
--rw-r--r--   0        0        0     4316 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/auth/oauthclientsimpl.py
--rw-r--r--   0        0        0     5681 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/auth/sharetokensimpl.py
--rw-r--r--   0        0        0     3619 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/auth/usersimpl.py
--rw-r--r--   0        0        0        0 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/comments/__init__.py
--rw-r--r--   0        0        0     7097 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/comments/commentsimpl.py
--rw-r--r--   0        0        0        0 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/credentials/__init__.py
--rw-r--r--   0        0        0     5944 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/credentials/credentialsimpl.py
--rw-r--r--   0        0        0        0 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/datacapture/__init__.py
--rw-r--r--   0        0        0     4263 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/datacapture/carriersimpl.py
--rw-r--r--   0        0        0     5288 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/datacapture/carriersmodelsimpl.py
--rw-r--r--   0        0        0    11560 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/datacapture/collectiontasksimpl.py
--rw-r--r--   0        0        0     1445 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/datacapture/pilotsimpl.py
--rw-r--r--   0        0        0     4924 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/datacapture/teamsimpl.py
--rw-r--r--   0        0        0       94 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/datamngt/__init__.py
--rw-r--r--   0        0        0    49466 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/datamngt/datasetsimpl.py
--rw-r--r--   0        0        0        0 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/datastream/__init__.py
--rw-r--r--   0        0        0     3757 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/datastream/datastreamassetmonitoredimpl.py
--rw-r--r--   0        0        0     3705 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/datastream/datastreamsfilesimpl.py
--rw-r--r--   0        0        0     6023 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/datastream/datastreamsimpl.py
--rw-r--r--   0        0        0     8913 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/datastreamtemplate/datastreamtemplateimpl.py
--rw-r--r--   0        0        0        0 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/featuresservice/__init__.py
--rw-r--r--   0        0        0     6443 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/featuresservice/collectionsimpl.py
--rw-r--r--   0        0        0    12604 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/featuresservice/featuresimpl.py
--rw-r--r--   0        0        0        0 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/projectmngt/__init__.py
--rw-r--r--   0        0        0    14906 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/projectmngt/flightsimpl.py
--rw-r--r--   0        0        0    20382 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/projectmngt/missionsimpl.py
--rw-r--r--   0        0        0    18356 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/projectmngt/projectsimpl.py
--rw-r--r--   0        0        0        0 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/tags/__init__.py
--rw-r--r--   0        0        0     5779 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/client/tags/tagsimpl.py
--rw-r--r--   0        0        0     6637 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/apis/provider.py
--rw-r--r--   0        0        0        0 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/__init__.py
--rw-r--r--   0        0        0     3023 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/config.py
--rw-r--r--   0        0        0        0 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/connection/__init__.py
--rw-r--r--   0        0        0     2853 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/connection/abstract_connection.py
--rw-r--r--   0        0        0     4115 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/connection/async_connection.py
--rw-r--r--   0        0        0     6049 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/connection/connection.py
--rw-r--r--   0        0        0     1441 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/connection/credentials.py
--rw-r--r--   0        0        0     3202 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/connection/token.py
--rw-r--r--   0        0        0     1407 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/errors.py
--rw-r--r--   0        0        0        0 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/resources/analytics/__init__.py
--rw-r--r--   0        0        0      364 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/resources/analytics/products.py
--rw-r--r--   0        0        0     1734 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/resources/comments.py
--rw-r--r--   0        0        0        0 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/resources/datamngt/__init__.py
--rw-r--r--   0        0        0    11346 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/resources/datamngt/upload.py
--rw-r--r--   0        0        0        0 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/resources/projectmngt/__init__.py
--rw-r--r--   0        0        0      636 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/resources/projectmngt/flights.py
--rw-r--r--   0        0        0      914 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/resources/projectmngt/missions.py
--rw-r--r--   0        0        0     1105 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/resources/projectmngt/projects.py
--rw-r--r--   0        0        0     1514 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/resources/resource.py
--rw-r--r--   0        0        0     1842 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/resources/tags.py
--rw-r--r--   0        0        0     5819 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/resources/utils.py
--rw-r--r--   0        0        0        0 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/utils/__init__.py
--rw-r--r--   0        0        0     1232 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/utils/filehelper.py
--rw-r--r--   0        0        0     1200 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/utils/geo_utils.py
--rw-r--r--   0        0        0     3178 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/utils/requests.py
--rw-r--r--   0        0        0     1769 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/utils/srs.py
--rw-r--r--   0        0        0      344 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/utils/typing.py
--rw-r--r--   0        0        0     6114 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/utils/utils.py
--rw-r--r--   0        0        0      696 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/utils/versions.py
--rw-r--r--   0        0        0        0 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/utils/vertcrs/__init__.py
--rw-r--r--   0        0        0      119 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/utils/vertcrs/arbitrary.wkt
--rw-r--r--   0        0        0      130 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/utils/vertcrs/arbitrary_feet.wkt
--rw-r--r--   0        0        0      149 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/utils/vertcrs/arbitrary_feet_us.wkt
--rw-r--r--   0        0        0      211 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/utils/vertcrs/egm2008.wkt
--rw-r--r--   0        0        0      213 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/utils/vertcrs/egm2008_feet.wkt
--rw-r--r--   0        0        0      232 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/utils/vertcrs/egm2008_feet_us.wkt
--rw-r--r--   0        0        0      207 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/utils/vertcrs/egm96.wkt
--rw-r--r--   0        0        0      209 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/utils/vertcrs/egm96_feet.wkt
--rw-r--r--   0        0        0      228 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/utils/vertcrs/egm96_feet_us.wkt
--rw-r--r--   0        0        0      140 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/utils/vertcrs/wgs84.wkt
--rw-r--r--   0        0        0      136 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/utils/vertcrs/wgs84_feet.wkt
--rw-r--r--   0        0        0      155 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/utils/vertcrs/wgs84_feet_us.wkt
--rw-r--r--   0        0        0     1614 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/core/utils/warnings.py
--rw-r--r--   0        0        0        0 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/py.typed
--rw-r--r--   0        0        0    11832 2023-03-14 09:06:19.368378 alteia-2.7.0/alteia/sdk.py
--rw-r--r--   0        0        0     2808 2023-03-14 09:06:19.372378 alteia-2.7.0/pyproject.toml
--rw-r--r--   0        0        0     3355 2023-03-14 09:06:20.500504 alteia-2.7.0/setup.py
--rw-r--r--   0        0        0     3115 2023-03-14 09:06:20.500845 alteia-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-08 14:47:27.453100 alteia-2.8.0/LICENSE
+-rw-r--r--   0        0        0     1426 2023-06-08 14:47:27.453100 alteia-2.8.0/README.md
+-rw-r--r--   0        0        0      257 2023-06-08 14:47:27.453100 alteia-2.8.0/alteia/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:47:27.569102 alteia-2.8.0/alteia/apis/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:47:27.569102 alteia-2.8.0/alteia/apis/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:47:27.569102 alteia-2.8.0/alteia/apis/client/analytics/__init__.py
+-rw-r--r--   0        0        0    26328 2023-06-08 14:47:27.453100 alteia-2.8.0/alteia/apis/client/analytics/analyticsimpl.py
+-rwxr-xr-x   0        0        0    16721 2023-06-08 14:47:27.453100 alteia-2.8.0/alteia/apis/client/analytics/configurationsimpl.py
+-rw-r--r--   0        0        0     7927 2023-06-08 14:47:27.453100 alteia-2.8.0/alteia/apis/client/analytics/productsimpl.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:47:27.569102 alteia-2.8.0/alteia/apis/client/annotations/__init__.py
+-rw-r--r--   0        0        0    30043 2023-06-08 14:47:27.453100 alteia-2.8.0/alteia/apis/client/annotations/annotationsimpl.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:47:27.569102 alteia-2.8.0/alteia/apis/client/auth/__init__.py
+-rw-r--r--   0        0        0     4227 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/apis/client/auth/companiesimpl.py
+-rw-r--r--   0        0        0     4316 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/apis/client/auth/oauthclientsimpl.py
+-rw-r--r--   0        0        0     5681 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/apis/client/auth/sharetokensimpl.py
+-rw-r--r--   0        0        0     3619 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/apis/client/auth/usersimpl.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:47:27.569102 alteia-2.8.0/alteia/apis/client/comments/__init__.py
+-rw-r--r--   0        0        0     7097 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/apis/client/comments/commentsimpl.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:47:27.569102 alteia-2.8.0/alteia/apis/client/credentials/__init__.py
+-rw-r--r--   0        0        0     7071 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/apis/client/credentials/credentialsimpl.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:47:27.569102 alteia-2.8.0/alteia/apis/client/datacapture/__init__.py
+-rw-r--r--   0        0        0     4263 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/apis/client/datacapture/carriersimpl.py
+-rw-r--r--   0        0        0     5288 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/apis/client/datacapture/carriersmodelsimpl.py
+-rw-r--r--   0        0        0    11560 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/apis/client/datacapture/collectiontasksimpl.py
+-rw-r--r--   0        0        0     1445 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/apis/client/datacapture/pilotsimpl.py
+-rw-r--r--   0        0        0     4924 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/apis/client/datacapture/teamsimpl.py
+-rw-r--r--   0        0        0       94 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/apis/client/datamngt/__init__.py
+-rw-r--r--   0        0        0    49466 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/apis/client/datamngt/datasetsimpl.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:47:27.569102 alteia-2.8.0/alteia/apis/client/datastream/__init__.py
+-rw-r--r--   0        0        0     3757 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/apis/client/datastream/datastreamassetmonitoredimpl.py
+-rw-r--r--   0        0        0     3705 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/apis/client/datastream/datastreamsfilesimpl.py
+-rw-r--r--   0        0        0     6023 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/apis/client/datastream/datastreamsimpl.py
+-rw-r--r--   0        0        0     8351 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/apis/client/datastreamtemplate/datastreamtemplateimpl.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:47:27.569102 alteia-2.8.0/alteia/apis/client/featuresservice/__init__.py
+-rw-r--r--   0        0        0     6443 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/apis/client/featuresservice/collectionsimpl.py
+-rw-r--r--   0        0        0    12604 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/apis/client/featuresservice/featuresimpl.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:47:27.569102 alteia-2.8.0/alteia/apis/client/projectmngt/__init__.py
+-rw-r--r--   0        0        0    14906 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/apis/client/projectmngt/flightsimpl.py
+-rw-r--r--   0        0        0    20382 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/apis/client/projectmngt/missionsimpl.py
+-rw-r--r--   0        0        0    18356 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/apis/client/projectmngt/projectsimpl.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:47:27.569102 alteia-2.8.0/alteia/apis/client/tags/__init__.py
+-rw-r--r--   0        0        0     5779 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/apis/client/tags/tagsimpl.py
+-rw-r--r--   0        0        0     6637 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/apis/provider.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:47:27.573102 alteia-2.8.0/alteia/core/__init__.py
+-rw-r--r--   0        0        0     3023 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/core/config.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:47:27.573102 alteia-2.8.0/alteia/core/connection/__init__.py
+-rw-r--r--   0        0        0     2853 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/core/connection/abstract_connection.py
+-rw-r--r--   0        0        0     4115 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/core/connection/async_connection.py
+-rw-r--r--   0        0        0     6077 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/core/connection/connection.py
+-rw-r--r--   0        0        0     1441 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/core/connection/credentials.py
+-rw-r--r--   0        0        0     3202 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/core/connection/token.py
+-rw-r--r--   0        0        0     1527 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/core/errors.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:47:27.573102 alteia-2.8.0/alteia/core/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:47:27.573102 alteia-2.8.0/alteia/core/resources/analytics/__init__.py
+-rw-r--r--   0        0        0      364 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/core/resources/analytics/products.py
+-rw-r--r--   0        0        0     1734 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/core/resources/comments.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:47:27.573102 alteia-2.8.0/alteia/core/resources/datamngt/__init__.py
+-rw-r--r--   0        0        0    11346 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/core/resources/datamngt/upload.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:47:27.573102 alteia-2.8.0/alteia/core/resources/projectmngt/__init__.py
+-rw-r--r--   0        0        0      636 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/core/resources/projectmngt/flights.py
+-rw-r--r--   0        0        0      914 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/core/resources/projectmngt/missions.py
+-rw-r--r--   0        0        0     1105 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/core/resources/projectmngt/projects.py
+-rw-r--r--   0        0        0     1514 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/core/resources/resource.py
+-rw-r--r--   0        0        0     1842 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/core/resources/tags.py
+-rw-r--r--   0        0        0     5819 2023-06-08 14:47:27.457100 alteia-2.8.0/alteia/core/resources/utils.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:47:27.573102 alteia-2.8.0/alteia/core/utils/__init__.py
+-rw-r--r--   0        0        0     1232 2023-06-08 14:47:27.461100 alteia-2.8.0/alteia/core/utils/filehelper.py
+-rw-r--r--   0        0        0     1200 2023-06-08 14:47:27.461100 alteia-2.8.0/alteia/core/utils/geo_utils.py
+-rw-r--r--   0        0        0     3178 2023-06-08 14:47:27.461100 alteia-2.8.0/alteia/core/utils/requests.py
+-rw-r--r--   0        0        0     1769 2023-06-08 14:47:27.461100 alteia-2.8.0/alteia/core/utils/srs.py
+-rw-r--r--   0        0        0      344 2023-06-08 14:47:27.461100 alteia-2.8.0/alteia/core/utils/typing.py
+-rw-r--r--   0        0        0     6114 2023-06-08 14:47:27.461100 alteia-2.8.0/alteia/core/utils/utils.py
+-rw-r--r--   0        0        0      696 2023-06-08 14:47:27.461100 alteia-2.8.0/alteia/core/utils/versions.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:47:27.573102 alteia-2.8.0/alteia/core/utils/vertcrs/__init__.py
+-rw-r--r--   0        0        0      119 2023-06-08 14:47:27.461100 alteia-2.8.0/alteia/core/utils/vertcrs/arbitrary.wkt
+-rw-r--r--   0        0        0      130 2023-06-08 14:47:27.461100 alteia-2.8.0/alteia/core/utils/vertcrs/arbitrary_feet.wkt
+-rw-r--r--   0        0        0      149 2023-06-08 14:47:27.461100 alteia-2.8.0/alteia/core/utils/vertcrs/arbitrary_feet_us.wkt
+-rw-r--r--   0        0        0      211 2023-06-08 14:47:27.461100 alteia-2.8.0/alteia/core/utils/vertcrs/egm2008.wkt
+-rw-r--r--   0        0        0      213 2023-06-08 14:47:27.461100 alteia-2.8.0/alteia/core/utils/vertcrs/egm2008_feet.wkt
+-rw-r--r--   0        0        0      232 2023-06-08 14:47:27.461100 alteia-2.8.0/alteia/core/utils/vertcrs/egm2008_feet_us.wkt
+-rw-r--r--   0        0        0      207 2023-06-08 14:47:27.461100 alteia-2.8.0/alteia/core/utils/vertcrs/egm96.wkt
+-rw-r--r--   0        0        0      209 2023-06-08 14:47:27.461100 alteia-2.8.0/alteia/core/utils/vertcrs/egm96_feet.wkt
+-rw-r--r--   0        0        0      228 2023-06-08 14:47:27.461100 alteia-2.8.0/alteia/core/utils/vertcrs/egm96_feet_us.wkt
+-rw-r--r--   0        0        0      140 2023-06-08 14:47:27.461100 alteia-2.8.0/alteia/core/utils/vertcrs/wgs84.wkt
+-rw-r--r--   0        0        0      136 2023-06-08 14:47:27.461100 alteia-2.8.0/alteia/core/utils/vertcrs/wgs84_feet.wkt
+-rw-r--r--   0        0        0      155 2023-06-08 14:47:27.461100 alteia-2.8.0/alteia/core/utils/vertcrs/wgs84_feet_us.wkt
+-rw-r--r--   0        0        0     1614 2023-06-08 14:47:27.461100 alteia-2.8.0/alteia/core/utils/warnings.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:47:27.573102 alteia-2.8.0/alteia/py.typed
+-rw-r--r--   0        0        0    11832 2023-06-08 14:47:27.461100 alteia-2.8.0/alteia/sdk.py
+-rw-r--r--   0        0        0     2808 2023-06-08 14:47:27.461100 alteia-2.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3355 2023-06-08 14:47:28.514963 alteia-2.8.0/setup.py
+-rw-r--r--   0        0        0     3115 2023-06-08 14:47:28.515293 alteia-2.8.0/PKG-INFO
```

### Comparing `alteia-2.7.0/LICENSE` & `alteia-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/README.md` & `alteia-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/apis/client/analytics/analyticsimpl.py` & `alteia-2.8.0/alteia/apis/client/analytics/analyticsimpl.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 """
 
 import warnings
 from collections import defaultdict
 from typing import (Any, DefaultDict, Dict, Generator, List, Optional, Union,
                     cast)
 
-from alteia.core.utils.warnings import deprecated, warn_for_deprecation
 from semantic_version import NpmSpec, Version
 
 from alteia.apis.provider import AnalyticsServiceAPI
 from alteia.core.errors import ParameterError
 from alteia.core.resources.resource import Resource, ResourcesWithTotal
 from alteia.core.resources.utils import search_generator
 from alteia.core.utils.typing import ResourceId
 from alteia.core.utils.versions import select_version
+from alteia.core.utils.warnings import deprecated, warn_for_deprecation
 
 
 class AnalyticsImpl:
     def __init__(self, analytics_service_api: AnalyticsServiceAPI, **kwargs):
         self._provider = analytics_service_api
 
     @deprecated(target='3.0.0')
```

### Comparing `alteia-2.7.0/alteia/apis/client/analytics/configurationsimpl.py` & `alteia-2.8.0/alteia/apis/client/analytics/configurationsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/apis/client/analytics/productsimpl.py` & `alteia-2.8.0/alteia/apis/client/analytics/productsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/apis/client/annotations/annotationsimpl.py` & `alteia-2.8.0/alteia/apis/client/annotations/annotationsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/apis/client/auth/companiesimpl.py` & `alteia-2.8.0/alteia/apis/client/auth/companiesimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/apis/client/auth/oauthclientsimpl.py` & `alteia-2.8.0/alteia/apis/client/auth/oauthclientsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/apis/client/auth/sharetokensimpl.py` & `alteia-2.8.0/alteia/apis/client/auth/sharetokensimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/apis/client/auth/usersimpl.py` & `alteia-2.8.0/alteia/apis/client/auth/usersimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/apis/client/comments/commentsimpl.py` & `alteia-2.8.0/alteia/apis/client/comments/commentsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/apis/client/credentials/credentialsimpl.py` & `alteia-2.8.0/alteia/apis/client/credentials/credentialsimpl.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """
     Credential implementation
 """
 
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List, Optional, Union
 
 from alteia.apis.provider import CredentialsServiceAPI
 from alteia.core.errors import ParameterError
 from alteia.core.resources.resource import ResourcesWithTotal
 from alteia.core.utils.typing import Resource, ResourceId
 
 DOCKER = 'docker'
 OBJECT_STORAGE = 'object-storage'
 
+OBJECT_STORAGE_TYPES = ("s3", "azure-blob")
+DOCKER_TYPES = ("aws", "docker")
+
 
 class CredentialsImpl:
     def __init__(self,
                  credentials_service_api: CredentialsServiceAPI,
                  **kwargs):
         self._provider = credentials_service_api
 
@@ -80,68 +83,89 @@
 
         if return_total:
             total = search_desc.get('total')
             return ResourcesWithTotal(total=total, results=results)
 
         return results
 
-    def create(self, *, name: str, credentials_type: str = DOCKER, credentials: Dict[str, str],
+    def create(self, *, name: str, credentials: Dict[str, str], credentials_type: Optional[str] = None,
                **kwargs) -> Resource:
         """Create a credential entry.
 
         Args:
             name: Credential name (must be unique).
 
-            credentials_type : Credentials type (docker or object-storage), default: docker
+            credentials_type : Credentials type (docker or object-storage)
 
             credentials: Credential dict.
 
             **kwargs: Optional keyword arguments. Those arguments are
                 passed as is to the API provider.
 
         Returns:
             The created credential description.
 
         Examples:
             >>> sdk.credentials.create(name="My Docker registry",
+            ...     credentials_type="docker"
             ...     credentials={
             ...         "type": "docker",
             ...         "login": "my_login",
             ...         "password": "my_password",
             ...         "registry": "mydockerregistry.com"
             ...     }
             ... )
             Resource(_id='5e5155ae8dcb064fcbf4ae35')
 
-            >>> sdk.credentials.create(name="My Docker registry",
+            >>> sdk.credentials.create(name="My aws registry",
+            ...     credentials_type="docker"
             ...     credentials={
             ...         "type": "aws",
             ...         "aws_access_key_id": "key_id",
             ...         "aws_secret_access_key": "password_test",
             ...         "aws_region": "us-east-1",
-            ...         "registry": "XXX..dkr.ecr.us-east-1.amazonaws.com"
+            ...         "registry": "XXX.dkr.ecr.us-east-1.amazonaws.com"
             ...     }
             ... )
             Resource(_id='5e6155ae8dcb064fcbf4ae35')
 
             >>> sdk.credentials.create(name="My bucket S3",
+            ...     credentials_type="object-storage"
             ...     credentials={
             ...         "type": "s3",
             ...         "aws_access_key_id": "key_id",
             ...         "aws_secret_access_key": "password_test",
             ...         "aws_region": "us-east-1",
-            ...         "registry": "XXX..s3.us-east-1.amazonaws.com/key"
+            ...         "bucket": "XXX.s3.us-east-1.amazonaws.com/key"
+            ...     }
+            ... )
+            Resource(_id='5e6155ae8dcb064fcbf4ae35')
+
+            >>> sdk.credentials.create(name="My azure blob",
+            ...     credentials_type="object-storage"
+            ...     credentials={
+            ...         "type": "azure-blob",
+            ...         "azure_client_id": "key_id",
+            ...         "azure_tenant_id": "password_test",
+            ...         "azure_client_secret": "us-east-1",
+            ...         "account_url": "https://mystorage.blob.core.windows.net"
             ...     }
             ... )
             Resource(_id='5e6155ae8dcb064fcbf4ae35')
 
         """
         data = kwargs
-
-        if credentials_type not in [DOCKER, OBJECT_STORAGE]:
+        if not credentials_type:
+            if credentials["type"] in DOCKER_TYPES:
+                credentials_type = DOCKER
+            elif credentials["type"] in OBJECT_STORAGE_TYPES:
+                credentials_type = OBJECT_STORAGE
+            else:
+                raise ParameterError(f'Impossible to retrieve credentials type from {credentials["type"]}')
+        elif credentials_type not in (DOCKER, OBJECT_STORAGE):
             raise ParameterError('Type of credentials is wrong')
 
         data.update({
             'name': name,
             'type': credentials_type,
             'credentials': credentials
         })
```

### Comparing `alteia-2.7.0/alteia/apis/client/datacapture/carriersimpl.py` & `alteia-2.8.0/alteia/apis/client/datacapture/carriersimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/apis/client/datacapture/carriersmodelsimpl.py` & `alteia-2.8.0/alteia/apis/client/datacapture/carriersmodelsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/apis/client/datacapture/collectiontasksimpl.py` & `alteia-2.8.0/alteia/apis/client/datacapture/collectiontasksimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/apis/client/datacapture/pilotsimpl.py` & `alteia-2.8.0/alteia/apis/client/datacapture/pilotsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/apis/client/datacapture/teamsimpl.py` & `alteia-2.8.0/alteia/apis/client/datacapture/teamsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/apis/client/datamngt/datasetsimpl.py` & `alteia-2.8.0/alteia/apis/client/datamngt/datasetsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/apis/client/datastream/datastreamassetmonitoredimpl.py` & `alteia-2.8.0/alteia/apis/client/datastream/datastreamassetmonitoredimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/apis/client/datastream/datastreamsfilesimpl.py` & `alteia-2.8.0/alteia/apis/client/datastream/datastreamsfilesimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/apis/client/datastream/datastreamsimpl.py` & `alteia-2.8.0/alteia/apis/client/datastream/datastreamsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/apis/client/datastreamtemplate/datastreamtemplateimpl.py` & `alteia-2.8.0/alteia/apis/client/datastreamtemplate/datastreamtemplateimpl.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 
     def create(
         self,
         *,
         name: str,
         source: Dict,
         import_dataset: Dict,
-        contextualisation: Dict,
-        transform: Dict,
         **kwargs
     ) -> Resource:
         """Create a datastream template.
 
         Args:
             name: Datastream template name.
 
@@ -34,26 +32,14 @@
                     category to set on the dataset.
 
                 horizontal_srs_wkt: Optional geographic coordinate system
                     for horizontal coordinattes in WKT format.
 
                 ingestion: ingestion parameters
 
-            contextualisation: contextualisation parameters.
-
-                assets_schema_repository: name of assets schema repository
-
-                geographic_buffer: buffer enlarging the search box
-
-                assets_schema: name of asset schema
-
-                assets_schema_property_name: name of assets schema property
-
-            transform: information for the analytic process.
-
             **kwargs: Optional keyword arguments. Those arguments are
                 passed as is to the API provider.
 
         Returns:
             The created datastream template description.
 
         Examples:
@@ -108,24 +94,21 @@
             ...     "company": "XXX"
             ...     "description": "My datastream description",
             ... )
             Resource(_id='5e5155ae8dcb064fcbf4ae35')
 
         """
         data: Dict = kwargs
+        template = {
+            "name": name,
+            "source": source,
+            "import": import_dataset,
+        }
 
-        data.update(
-            {
-                "name": name,
-                "source": source,
-                "import": import_dataset,
-                "contextualisation": contextualisation,
-                "transform": transform,
-            }
-        )
+        data.update(template)
 
         desc = self._provider.post(path="create-datastream-template", data=data)
 
         return Resource(**desc)
 
     def delete(self, template: ResourceId) -> None:
         """Delete a datastream template entry.
```

### Comparing `alteia-2.7.0/alteia/apis/client/featuresservice/collectionsimpl.py` & `alteia-2.8.0/alteia/apis/client/featuresservice/collectionsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/apis/client/featuresservice/featuresimpl.py` & `alteia-2.8.0/alteia/apis/client/featuresservice/featuresimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/apis/client/projectmngt/flightsimpl.py` & `alteia-2.8.0/alteia/apis/client/projectmngt/flightsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/apis/client/projectmngt/missionsimpl.py` & `alteia-2.8.0/alteia/apis/client/projectmngt/missionsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/apis/client/projectmngt/projectsimpl.py` & `alteia-2.8.0/alteia/apis/client/projectmngt/projectsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/apis/client/tags/tagsimpl.py` & `alteia-2.8.0/alteia/apis/client/tags/tagsimpl.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/apis/provider.py` & `alteia-2.8.0/alteia/apis/provider.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/core/config.py` & `alteia-2.8.0/alteia/core/config.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/core/connection/abstract_connection.py` & `alteia-2.8.0/alteia/core/connection/abstract_connection.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/core/connection/async_connection.py` & `alteia-2.8.0/alteia/core/connection/async_connection.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/core/connection/connection.py` & `alteia-2.8.0/alteia/core/connection/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,10 +152,10 @@
                 self._renew_token()
                 self._add_authorization_maybe(params['headers'], params['url'])
 
                 LOGGER.debug('Retrying to request using the new token..')
                 response = self._http.request(**params)
 
         if response.status not in range(200, 300):
-            raise ResponseError(f'{response.status}: {response.data[:256]}')
+            raise ResponseError(msg=f'{response.status}: {response.data[:256]}', status=response.status)
 
         return response
```

### Comparing `alteia-2.7.0/alteia/core/connection/credentials.py` & `alteia-2.8.0/alteia/core/connection/credentials.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/core/connection/token.py` & `alteia-2.8.0/alteia/core/connection/token.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/core/errors.py` & `alteia-2.8.0/alteia/core/errors.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,14 +9,15 @@
            'DownloadError', 'BoundingBoxError', 'ParameterError', 'SearchError')
 
 
 class _Error(Exception):
     """Base class for all package exceptions.
 
     """
+
     def __init__(self, msg=''):
         super().__init__(msg)
 
 
 class ConfigError(_Error):
     pass
 
@@ -45,15 +46,17 @@
 
 
 class QueryError(_Error):
     pass
 
 
 class ResponseError(_Error):
-    pass
+    def __init__(self, msg, status: int = 0):
+        super(ResponseError, self).__init__(msg=msg)
+        self.status = status
 
 
 class MissingCredentialsError(_Error):
     pass
 
 
 class TokenRenewalError(_Error):
```

### Comparing `alteia-2.7.0/alteia/core/resources/comments.py` & `alteia-2.8.0/alteia/core/resources/comments.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/core/resources/datamngt/upload.py` & `alteia-2.8.0/alteia/core/resources/datamngt/upload.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/core/resources/projectmngt/flights.py` & `alteia-2.8.0/alteia/core/resources/projectmngt/flights.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/core/resources/projectmngt/missions.py` & `alteia-2.8.0/alteia/core/resources/projectmngt/missions.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/core/resources/projectmngt/projects.py` & `alteia-2.8.0/alteia/core/resources/projectmngt/projects.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/core/resources/resource.py` & `alteia-2.8.0/alteia/core/resources/resource.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/core/resources/tags.py` & `alteia-2.8.0/alteia/core/resources/tags.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/core/resources/utils.py` & `alteia-2.8.0/alteia/core/resources/utils.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/core/utils/filehelper.py` & `alteia-2.8.0/alteia/core/utils/filehelper.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/core/utils/geo_utils.py` & `alteia-2.8.0/alteia/core/utils/geo_utils.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/core/utils/requests.py` & `alteia-2.8.0/alteia/core/utils/requests.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/core/utils/srs.py` & `alteia-2.8.0/alteia/core/utils/srs.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/core/utils/utils.py` & `alteia-2.8.0/alteia/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/core/utils/versions.py` & `alteia-2.8.0/alteia/core/utils/versions.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/core/utils/warnings.py` & `alteia-2.8.0/alteia/core/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/alteia/sdk.py` & `alteia-2.8.0/alteia/sdk.py`

 * *Files identical despite different names*

### Comparing `alteia-2.7.0/pyproject.toml` & `alteia-2.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alteia"
-version = "2.7.0"  # must match the version in alteia/__init__.py
+version = "2.8.0"  # must match the version in alteia/__init__.py
 description = "High-level Python interface to Alteia API"
 authors = ["Alteia Backend team <backend-team@alteia.com>"]
 repository = "https://github.com/alteia-ai/alteia-python-sdk"
 documentation = "https://alteia.readthedocs.io/en/latest/index.html"
 license = "MIT"
 readme = "README.md"
 keywords = ["sdk",
@@ -34,15 +34,15 @@
 recommonmark = {version = "^0.7.1", optional = true, python = ">=3.8"}
 semantic-version = "^2.8.5"
 importlib-resources = {version = ">=1.4", python = "<3.7"}
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 flake8 = "^3.7.9"
-pylint = "^2.4.4"
+pylint = "2.12.0"
 pre-commit = "^2.6.0"
 urllib3-mock = "^0.3.3"
 mypy = "^0.910"
 types-setuptools = "^57.4.0"
 
 [tool.poetry.extras]
 documentation = [
```

### Comparing `alteia-2.7.0/setup.py` & `alteia-2.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
  'documentation:python_version >= "3.8"': ['sphinx>=4.1.2,<5.0.0',
                                            'sphinx_autodoc_typehints>=1.12.0,<2.0.0',
                                            'sphinx-autobuild>=2021.3.14,<2022.0.0',
                                            'recommonmark>=0.7.1,<0.8.0']}
 
 setup_kwargs = {
     'name': 'alteia',
-    'version': '2.7.0',
+    'version': '2.8.0',
     'description': 'High-level Python interface to Alteia API',
     'long_description': '<p align="center">\n<img src="https://raw.githubusercontent.com/alteia-ai/alteia-python-sdk/master/docs/images/SDK_Python.png" alt="logo" style="max-width:100%;">\n\n<p align="center">\n<a href="https://pypi.org/project/alteia/" rel="nofollow"><img src="https://img.shields.io/pypi/v/alteia.svg" alt="pypi version" style="max-width:100%;"></a>\n<a href="https://pypi.org/project/alteia/" rel="nofollow"><img src="https://img.shields.io/pypi/pyversions/alteia.svg" alt="compatible python versions" style="max-width:100%;"></a>\n</p>\n\n> This SDK offers a high-level Python interface to [Alteia APIs](https://www.alteia.com).\n\n## Installation\n\n```bash\npip install alteia\n```\n\n**requires Python >= 3.6.1, pip >= 20.3*\n\n## Basic usage\n\n```python\nimport alteia\n\nsdk = alteia.SDK(user="YOUR_EMAIL_ADDRESS", password="YOUR_ALTEIA_PASSWORD")\n\nprojects = sdk.projects.search()\n\nfor project in projects:\n    print(project.name)\n\n# My awesome project\n```\n\n<p>&nbsp;</p>\n\n## 📕 Documentation\n\n- [Reference documentation](https://alteia.readthedocs.io/en/latest/index.html)\n- [Jupyter notebook tutorials](https://github.com/alteia-ai/tutorials)\n\n## Contributing\n\nPackage installation:\n\n```bash\npoetry install\n```\n\n(Optional) To install pre-commit hooks (and detect problems before the pipelines):\n\n```bash\npip install pre-commit\npre-commit install\npre-commit run --all-files\npre-commit autoupdate  # Optional, to update pre-commit versions\n```\n',
     'author': 'Alteia Backend team',
     'author_email': 'backend-team@alteia.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/alteia-ai/alteia-python-sdk',
```

#### html2text {}

```diff
@@ -11,15 +11,15 @@
 'alteia.core.utils', 'alteia.core.utils.vertcrs'] package_data = \ {'': ['*']}
 install_requires = \ ['appdirs>=1.4.3,<2.0.0', 'pathvalidate>=2.3.0,<3.0.0',
 'semantic-version>=2.8.5,<3.0.0', 'urllib3>=1.26,<2.0'] extras_require = \ {':
 python_version < "3.7"': ['importlib-resources>=1.4'], 'documentation:
 python_version >= "3.8"': ['sphinx>=4.1.2,<5.0.0',
 'sphinx_autodoc_typehints>=1.12.0,<2.0.0', 'sphinx-
 autobuild>=2021.3.14,<2022.0.0', 'recommonmark>=0.7.1,<0.8.0']} setup_kwargs =
-{ 'name': 'alteia', 'version': '2.7.0', 'description': 'High-level Python
+{ 'name': 'alteia', 'version': '2.8.0', 'description': 'High-level Python
 interface to Alteia API', 'long_description': '
                                  \n[logo]\n\n
                \n[pypi_version]\n[compatible_python_versions]\n
 \n\n> This SDK offers a high-level Python interface to [Alteia APIs](https://
 www.alteia.com).\n\n## Installation\n\n```bash\npip install
 alteia\n```\n\n**requires Python >= 3.6.1, pip >= 20.3*\n\n## Basic
 usage\n\n```python\nimport alteia\n\nsdk = alteia.SDK
```

### Comparing `alteia-2.7.0/PKG-INFO` & `alteia-2.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alteia
-Version: 2.7.0
+Version: 2.8.0
 Summary: High-level Python interface to Alteia API
 Home-page: https://github.com/alteia-ai/alteia-python-sdk
 License: MIT
 Keywords: sdk,alteia
 Author: Alteia Backend team
 Author-email: backend-team@alteia.com
 Requires-Python: >=3.6.1,<4.0.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alteia Version: 2.7.0 Summary: High-level Python
+Metadata-Version: 2.1 Name: alteia Version: 2.8.0 Summary: High-level Python
 interface to Alteia API Home-page: https://github.com/alteia-ai/alteia-python-
 sdk License: MIT Keywords: sdk,alteia Author: Alteia Backend team Author-email:
 backend-team@alteia.com Requires-Python: >=3.6.1,<4.0.0 Classifier: Development
 Status :: 5 - Production/Stable Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
```

