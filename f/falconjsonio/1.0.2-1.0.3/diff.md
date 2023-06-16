# Comparing `tmp/falconjsonio-1.0.2.tar.gz` & `tmp/falconjsonio-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/falconjsonio-1.0.2.tar", last modified: Tue Jun  6 11:15:12 2017, max compression
+gzip compressed data, was "falconjsonio-1.0.3.tar", last modified: Fri Jun 16 00:45:01 2023, max compression
```

## Comparing `falconjsonio-1.0.2.tar` & `falconjsonio-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2017-06-06 11:15:12.000000 falconjsonio-1.0.2/
--rw-rw-r--   0 gary      (1000) gary      (1000)       79 2017-06-06 11:15:12.000000 falconjsonio-1.0.2/setup.cfg
--rw-rw-r--   0 gary      (1000) gary      (1000)       36 2016-05-12 10:20:14.000000 falconjsonio-1.0.2/requirements.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)     5745 2017-06-06 11:15:12.000000 falconjsonio-1.0.2/PKG-INFO
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2017-06-06 11:15:12.000000 falconjsonio-1.0.2/falconjsonio/
--rw-rw-r--   0 gary      (1000) gary      (1000)    17932 2017-06-06 11:10:51.000000 falconjsonio-1.0.2/falconjsonio/test.py
--rw-rw-r--   0 gary      (1000) gary      (1000)        0 2015-12-31 05:42:47.000000 falconjsonio-1.0.2/falconjsonio/__init__.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     2022 2017-06-06 11:10:51.000000 falconjsonio-1.0.2/falconjsonio/schema.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     4232 2017-06-06 11:10:51.000000 falconjsonio-1.0.2/falconjsonio/middleware.py
-drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2017-06-06 11:15:12.000000 falconjsonio-1.0.2/falconjsonio.egg-info/
--rw-rw-r--   0 gary      (1000) gary      (1000)     5745 2017-06-06 11:15:12.000000 falconjsonio-1.0.2/falconjsonio.egg-info/PKG-INFO
--rw-rw-r--   0 gary      (1000) gary      (1000)       32 2017-06-06 11:15:12.000000 falconjsonio-1.0.2/falconjsonio.egg-info/requires.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)        1 2015-12-31 05:44:07.000000 falconjsonio-1.0.2/falconjsonio.egg-info/not-zip-safe
--rw-rw-r--   0 gary      (1000) gary      (1000)      379 2017-06-06 11:15:12.000000 falconjsonio-1.0.2/falconjsonio.egg-info/SOURCES.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)       13 2017-06-06 11:15:12.000000 falconjsonio-1.0.2/falconjsonio.egg-info/top_level.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)        1 2017-06-06 11:15:12.000000 falconjsonio-1.0.2/falconjsonio.egg-info/dependency_links.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)     1205 2017-06-06 11:11:16.000000 falconjsonio-1.0.2/setup.py
--rw-rw-r--   0 gary      (1000) gary      (1000)     3567 2016-02-14 08:19:32.000000 falconjsonio-1.0.2/README.md
--rw-rw-r--   0 gary      (1000) gary      (1000)     1055 2015-12-31 05:42:47.000000 falconjsonio-1.0.2/LICENSE.txt
--rw-rw-r--   0 gary      (1000) gary      (1000)       63 2015-12-31 05:42:47.000000 falconjsonio-1.0.2/MANIFEST.in
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-06-16 00:45:01.601414 falconjsonio-1.0.3/
+-rw-rw-r--   0 gary      (1000) gary      (1000)     1055 2023-06-15 06:38:02.000000 falconjsonio-1.0.3/LICENSE.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)       63 2023-06-15 06:38:02.000000 falconjsonio-1.0.3/MANIFEST.in
+-rw-rw-r--   0 gary      (1000) gary      (1000)     5685 2023-06-16 00:45:01.601414 falconjsonio-1.0.3/PKG-INFO
+-rw-rw-r--   0 gary      (1000) gary      (1000)     3567 2023-06-15 06:38:02.000000 falconjsonio-1.0.3/README.md
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-06-16 00:45:01.597414 falconjsonio-1.0.3/falconjsonio/
+-rw-rw-r--   0 gary      (1000) gary      (1000)        0 2023-06-15 06:38:02.000000 falconjsonio-1.0.3/falconjsonio/__init__.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     4232 2023-06-15 06:38:02.000000 falconjsonio-1.0.3/falconjsonio/middleware.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)     2022 2023-06-15 06:38:02.000000 falconjsonio-1.0.3/falconjsonio/schema.py
+-rw-rw-r--   0 gary      (1000) gary      (1000)    17932 2023-06-15 06:38:02.000000 falconjsonio-1.0.3/falconjsonio/test.py
+drwxrwxr-x   0 gary      (1000) gary      (1000)        0 2023-06-16 00:45:01.601414 falconjsonio-1.0.3/falconjsonio.egg-info/
+-rw-rw-r--   0 gary      (1000) gary      (1000)     5685 2023-06-16 00:45:01.000000 falconjsonio-1.0.3/falconjsonio.egg-info/PKG-INFO
+-rw-rw-r--   0 gary      (1000) gary      (1000)      379 2023-06-16 00:45:01.000000 falconjsonio-1.0.3/falconjsonio.egg-info/SOURCES.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)        1 2023-06-16 00:45:01.000000 falconjsonio-1.0.3/falconjsonio.egg-info/dependency_links.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)        1 2023-06-16 00:37:21.000000 falconjsonio-1.0.3/falconjsonio.egg-info/not-zip-safe
+-rw-rw-r--   0 gary      (1000) gary      (1000)       40 2023-06-16 00:45:01.000000 falconjsonio-1.0.3/falconjsonio.egg-info/requires.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)       13 2023-06-16 00:45:01.000000 falconjsonio-1.0.3/falconjsonio.egg-info/top_level.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)        2 2023-06-15 06:46:18.000000 falconjsonio-1.0.3/requirements.txt
+-rw-rw-r--   0 gary      (1000) gary      (1000)       79 2023-06-16 00:45:01.601414 falconjsonio-1.0.3/setup.cfg
+-rw-rw-r--   0 gary      (1000) gary      (1000)     1125 2023-06-15 06:53:09.000000 falconjsonio-1.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `falconjsonio-1.0.2/PKG-INFO` & `falconjsonio-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: falconjsonio
-Version: 1.0.2
+Version: 1.0.3
 Summary: JSON-Schema input and output for Falcon
 Home-page: https://bitbucket.org/garymonson/falcon-json-io
 Author: Gary Monson
 Author-email: gary.monson@gmail.com
 License: MIT
 Description: Falcon JSON IO
         ==============
@@ -25,127 +25,127 @@
         request matches your specification. Otherwise, an error is returned to
         the caller.
         
         Define your response body schema, and your response is validated before
         returning to the sender. A response that does not match the
         specification will return a 500 error instead.
         
-        Retrieve your request JSON using req.context['doc'].
+        Retrieve your request JSON using req.context[‘doc’].
         
-        Set your JSON response in req.context['result'].
+        Set your JSON response in req.context[‘result’].
         
         Using the middleware
         --------------------
         
         Enabled the middleware:
         
         ::
         
-            app = falcon.API(
-                middleware=[
-                    falconjsonio.middleware.RequireJSON(),
-                    falconjsonio.middleware.JSONTranslator(),
-                ],
-            )
+           app = falcon.API(
+               middleware=[
+                   falconjsonio.middleware.RequireJSON(),
+                   falconjsonio.middleware.JSONTranslator(),
+               ],
+           )
         
         Define your requirements:
         
         ::
         
-            from falconjsonio.schema import request_schema, response_schema
+           from falconjsonio.schema import request_schema, response_schema
         
-            people_post_request_schema = {
-                'type':       'object',
-                'properties': {
-                    'title':  {'type': 'string'},
-                    'name':   {'type': 'string'},
-                    'dob':    {'type': 'date-time'},
-                    'email':  {'type': 'email'},
-                },
-                'required': ['name', 'dob'],
-            }
-            people_post_response_schema = {
-                'oneOf': [
-                    {
-                        'type':       'object',
-                        'properties': {
-                            'href': {'type': uri'},
-                        },
-                        'required': ['uri'],
-                    },
-                    {
-                        'type':       'object',
-                        'properties': {
-                            'error': {'type': 'string'},
-                        },
-                        'required': ['error'],
-                    },
-                ],
-            }
-        
-            # ...
-        
-            class People(object):
-                @response_schema(people_get_response_schema)
-                def on_get(self, req, resp):
-                    # Put your JSON response here:
-                    req.context['result'] = {'some': 'json'}
-        
-                @request_schema(people_post_request_schema)
-                @response_schema(people_post_response_schema)
-                def on_post(self, req, resp):
-                    # JSON request supplied here:
-                    form = req.context['doc']
-                    # Put your JSON response here:
-                    req.context['result'] = {'some': 'json'}
+           people_post_request_schema = {
+               'type':       'object',
+               'properties': {
+                   'title':  {'type': 'string'},
+                   'name':   {'type': 'string'},
+                   'dob':    {'type': 'date-time'},
+                   'email':  {'type': 'email'},
+               },
+               'required': ['name', 'dob'],
+           }
+           people_post_response_schema = {
+               'oneOf': [
+                   {
+                       'type':       'object',
+                       'properties': {
+                           'href': {'type': uri'},
+                       },
+                       'required': ['uri'],
+                   },
+                   {
+                       'type':       'object',
+                       'properties': {
+                           'error': {'type': 'string'},
+                       },
+                       'required': ['error'],
+                   },
+               ],
+           }
+        
+           # ...
+        
+           class People(object):
+               @response_schema(people_get_response_schema)
+               def on_get(self, req, resp):
+                   # Put your JSON response here:
+                   req.context['result'] = {'some': 'json'}
+        
+               @request_schema(people_post_request_schema)
+               @response_schema(people_post_response_schema)
+               def on_post(self, req, resp):
+                   # JSON request supplied here:
+                   form = req.context['doc']
+                   # Put your JSON response here:
+                   req.context['result'] = {'some': 'json'}
         
         Hook the endpoint in, of course:
         
         ::
         
-            app.add_route('/people', People())
+           app.add_route('/people', People())
         
         If your methods are inherited from a parent class, you can apply the
         decorator to the resource class instead, and pass the method name to the
         decorator:
         
         ::
         
-            class People(object):
-                def on_get(self, req, resp):
-                    # Put your JSON response here:
-                    req.context['result'] = {'some': 'json'}
-        
-                def on_post(self, req, resp):
-                    # JSON request supplied here:
-                    form = req.context['doc']
-                    # Put your JSON response here:
-                    req.context['result'] = {'some': 'json'}
-        
-            @response_schema(schema=people_get_response_schema, method_name='on_get')
-            @request_schema(schema=people_post_request_schema, method_name='on_post')
-            @response_schema(schema=people_post_response_schema, method_name='on_post')
-            class ChildPeople(People):
-                pass
+           class People(object):
+               def on_get(self, req, resp):
+                   # Put your JSON response here:
+                   req.context['result'] = {'some': 'json'}
+        
+               def on_post(self, req, resp):
+                   # JSON request supplied here:
+                   form = req.context['doc']
+                   # Put your JSON response here:
+                   req.context['result'] = {'some': 'json'}
+        
+           @response_schema(schema=people_get_response_schema, method_name='on_get')
+           @request_schema(schema=people_post_request_schema, method_name='on_post')
+           @response_schema(schema=people_post_response_schema, method_name='on_post')
+           class ChildPeople(People):
+               pass
         
         This is especially useful when you have a parent class with all the
         smarts, and your child classes merely declare a few settings for the
         parent class (e.g.
         `falcon-autocrud <https://pypi.python.org/pypi/falcon-autocrud>`__)
         
         Quick start for contributing
         ----------------------------
         
         ::
         
-            virtualenv -p `which python3` virtualenv
-            source virtualenv/bin/activate
-            pip install -r requirements.txt
-            pip install -r dev_requirements.txt
-            nosetests
+           virtualenv -p `which python3` virtualenv
+           source virtualenv/bin/activate
+           pip install -r requirements.txt
+           pip install -r dev_requirements.txt
+           nosetests
         
         .. |Codeship Status for garymonson/falcon-json-io| image:: https://codeship.com/projects/c370db70-b520-0133-3191-1af10c27659b/status?branch=master
            :target: https://codeship.com/projects/134051
         
 Keywords: json schema falcon
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `falconjsonio-1.0.2/falconjsonio/test.py` & `falconjsonio-1.0.3/falconjsonio/test.py`

 * *Files identical despite different names*

### Comparing `falconjsonio-1.0.2/falconjsonio/schema.py` & `falconjsonio-1.0.3/falconjsonio/schema.py`

 * *Files identical despite different names*

### Comparing `falconjsonio-1.0.2/falconjsonio/middleware.py` & `falconjsonio-1.0.3/falconjsonio/middleware.py`

 * *Files identical despite different names*

### Comparing `falconjsonio-1.0.2/falconjsonio.egg-info/PKG-INFO` & `falconjsonio-1.0.3/falconjsonio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: falconjsonio
-Version: 1.0.2
+Version: 1.0.3
 Summary: JSON-Schema input and output for Falcon
 Home-page: https://bitbucket.org/garymonson/falcon-json-io
 Author: Gary Monson
 Author-email: gary.monson@gmail.com
 License: MIT
 Description: Falcon JSON IO
         ==============
@@ -25,127 +25,127 @@
         request matches your specification. Otherwise, an error is returned to
         the caller.
         
         Define your response body schema, and your response is validated before
         returning to the sender. A response that does not match the
         specification will return a 500 error instead.
         
-        Retrieve your request JSON using req.context['doc'].
+        Retrieve your request JSON using req.context[‘doc’].
         
-        Set your JSON response in req.context['result'].
+        Set your JSON response in req.context[‘result’].
         
         Using the middleware
         --------------------
         
         Enabled the middleware:
         
         ::
         
-            app = falcon.API(
-                middleware=[
-                    falconjsonio.middleware.RequireJSON(),
-                    falconjsonio.middleware.JSONTranslator(),
-                ],
-            )
+           app = falcon.API(
+               middleware=[
+                   falconjsonio.middleware.RequireJSON(),
+                   falconjsonio.middleware.JSONTranslator(),
+               ],
+           )
         
         Define your requirements:
         
         ::
         
-            from falconjsonio.schema import request_schema, response_schema
+           from falconjsonio.schema import request_schema, response_schema
         
-            people_post_request_schema = {
-                'type':       'object',
-                'properties': {
-                    'title':  {'type': 'string'},
-                    'name':   {'type': 'string'},
-                    'dob':    {'type': 'date-time'},
-                    'email':  {'type': 'email'},
-                },
-                'required': ['name', 'dob'],
-            }
-            people_post_response_schema = {
-                'oneOf': [
-                    {
-                        'type':       'object',
-                        'properties': {
-                            'href': {'type': uri'},
-                        },
-                        'required': ['uri'],
-                    },
-                    {
-                        'type':       'object',
-                        'properties': {
-                            'error': {'type': 'string'},
-                        },
-                        'required': ['error'],
-                    },
-                ],
-            }
-        
-            # ...
-        
-            class People(object):
-                @response_schema(people_get_response_schema)
-                def on_get(self, req, resp):
-                    # Put your JSON response here:
-                    req.context['result'] = {'some': 'json'}
-        
-                @request_schema(people_post_request_schema)
-                @response_schema(people_post_response_schema)
-                def on_post(self, req, resp):
-                    # JSON request supplied here:
-                    form = req.context['doc']
-                    # Put your JSON response here:
-                    req.context['result'] = {'some': 'json'}
+           people_post_request_schema = {
+               'type':       'object',
+               'properties': {
+                   'title':  {'type': 'string'},
+                   'name':   {'type': 'string'},
+                   'dob':    {'type': 'date-time'},
+                   'email':  {'type': 'email'},
+               },
+               'required': ['name', 'dob'],
+           }
+           people_post_response_schema = {
+               'oneOf': [
+                   {
+                       'type':       'object',
+                       'properties': {
+                           'href': {'type': uri'},
+                       },
+                       'required': ['uri'],
+                   },
+                   {
+                       'type':       'object',
+                       'properties': {
+                           'error': {'type': 'string'},
+                       },
+                       'required': ['error'],
+                   },
+               ],
+           }
+        
+           # ...
+        
+           class People(object):
+               @response_schema(people_get_response_schema)
+               def on_get(self, req, resp):
+                   # Put your JSON response here:
+                   req.context['result'] = {'some': 'json'}
+        
+               @request_schema(people_post_request_schema)
+               @response_schema(people_post_response_schema)
+               def on_post(self, req, resp):
+                   # JSON request supplied here:
+                   form = req.context['doc']
+                   # Put your JSON response here:
+                   req.context['result'] = {'some': 'json'}
         
         Hook the endpoint in, of course:
         
         ::
         
-            app.add_route('/people', People())
+           app.add_route('/people', People())
         
         If your methods are inherited from a parent class, you can apply the
         decorator to the resource class instead, and pass the method name to the
         decorator:
         
         ::
         
-            class People(object):
-                def on_get(self, req, resp):
-                    # Put your JSON response here:
-                    req.context['result'] = {'some': 'json'}
-        
-                def on_post(self, req, resp):
-                    # JSON request supplied here:
-                    form = req.context['doc']
-                    # Put your JSON response here:
-                    req.context['result'] = {'some': 'json'}
-        
-            @response_schema(schema=people_get_response_schema, method_name='on_get')
-            @request_schema(schema=people_post_request_schema, method_name='on_post')
-            @response_schema(schema=people_post_response_schema, method_name='on_post')
-            class ChildPeople(People):
-                pass
+           class People(object):
+               def on_get(self, req, resp):
+                   # Put your JSON response here:
+                   req.context['result'] = {'some': 'json'}
+        
+               def on_post(self, req, resp):
+                   # JSON request supplied here:
+                   form = req.context['doc']
+                   # Put your JSON response here:
+                   req.context['result'] = {'some': 'json'}
+        
+           @response_schema(schema=people_get_response_schema, method_name='on_get')
+           @request_schema(schema=people_post_request_schema, method_name='on_post')
+           @response_schema(schema=people_post_response_schema, method_name='on_post')
+           class ChildPeople(People):
+               pass
         
         This is especially useful when you have a parent class with all the
         smarts, and your child classes merely declare a few settings for the
         parent class (e.g.
         `falcon-autocrud <https://pypi.python.org/pypi/falcon-autocrud>`__)
         
         Quick start for contributing
         ----------------------------
         
         ::
         
-            virtualenv -p `which python3` virtualenv
-            source virtualenv/bin/activate
-            pip install -r requirements.txt
-            pip install -r dev_requirements.txt
-            nosetests
+           virtualenv -p `which python3` virtualenv
+           source virtualenv/bin/activate
+           pip install -r requirements.txt
+           pip install -r dev_requirements.txt
+           nosetests
         
         .. |Codeship Status for garymonson/falcon-json-io| image:: https://codeship.com/projects/c370db70-b520-0133-3191-1af10c27659b/status?branch=master
            :target: https://codeship.com/projects/134051
         
 Keywords: json schema falcon
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `falconjsonio-1.0.2/README.md` & `falconjsonio-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `falconjsonio-1.0.2/LICENSE.txt` & `falconjsonio-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

