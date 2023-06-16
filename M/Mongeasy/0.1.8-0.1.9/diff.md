# Comparing `tmp/Mongeasy-0.1.8.tar.gz` & `tmp/Mongeasy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mongeasy-0.1.8.tar", last modified: Fri Apr 21 10:45:23 2023, max compression
+gzip compressed data, was "Mongeasy-0.1.9.tar", last modified: Fri Jun 16 12:08:47 2023, max compression
```

## Comparing `Mongeasy-0.1.8.tar` & `Mongeasy-0.1.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 10:45:23.638808 Mongeasy-0.1.8/
--rw-rw-rw-   0        0        0     1096 2023-04-17 10:50:01.000000 Mongeasy-0.1.8/LICENSE
-drwxrwxrwx   0        0        0        0 2023-04-21 10:45:23.621786 Mongeasy-0.1.8/Mongeasy.egg-info/
--rw-rw-rw-   0        0        0    10874 2023-04-21 10:45:23.000000 Mongeasy-0.1.8/Mongeasy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      599 2023-04-21 10:45:23.000000 Mongeasy-0.1.8/Mongeasy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 10:45:23.000000 Mongeasy-0.1.8/Mongeasy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-21 10:45:23.000000 Mongeasy-0.1.8/Mongeasy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-04-21 10:45:23.000000 Mongeasy-0.1.8/Mongeasy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-21 10:45:23.000000 Mongeasy-0.1.8/Mongeasy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10874 2023-04-21 10:45:23.638808 Mongeasy-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    10042 2023-04-21 10:40:28.000000 Mongeasy-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 10:45:23.633302 Mongeasy-0.1.8/mongeasy/
--rw-rw-rw-   0        0        0     2164 2023-04-21 10:45:10.000000 Mongeasy-0.1.8/mongeasy/__init__.py
--rw-rw-rw-   0        0        0     2775 2023-03-03 13:34:30.000000 Mongeasy-0.1.8/mongeasy/base_dict.py
--rw-rw-rw-   0        0        0     2420 2023-04-21 10:30:51.000000 Mongeasy-0.1.8/mongeasy/connection.py
--rw-rw-rw-   0        0        0     2535 2023-04-21 08:00:17.000000 Mongeasy-0.1.8/mongeasy/core.py
--rw-rw-rw-   0        0        0    12866 2023-04-20 14:08:47.000000 Mongeasy-0.1.8/mongeasy/document.py
--rw-rw-rw-   0        0        0     2657 2023-04-20 11:53:13.000000 Mongeasy-0.1.8/mongeasy/dynamics.py
-drwxrwxrwx   0        0        0        0 2023-04-21 10:45:23.633302 Mongeasy-0.1.8/mongeasy/examples/
--rw-rw-rw-   0        0        0        0 2023-04-20 11:53:13.000000 Mongeasy-0.1.8/mongeasy/examples/__init__.py
--rw-rw-rw-   0        0        0     1851 2023-04-20 11:53:13.000000 Mongeasy-0.1.8/mongeasy/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-21 10:45:23.634303 Mongeasy-0.1.8/mongeasy/extensions/
--rw-rw-rw-   0        0        0        0 2023-04-20 11:53:13.000000 Mongeasy-0.1.8/mongeasy/extensions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 10:45:23.635302 Mongeasy-0.1.8/mongeasy/plugins/
--rw-rw-rw-   0        0        0        0 2023-04-20 11:53:13.000000 Mongeasy-0.1.8/mongeasy/plugins/__init__.py
--rw-rw-rw-   0        0        0     4963 2023-04-20 11:49:23.000000 Mongeasy-0.1.8/mongeasy/resultlist.py
-drwxrwxrwx   0        0        0        0 2023-04-21 10:45:23.636302 Mongeasy-0.1.8/mongeasy/utils/
--rw-rw-rw-   0        0        0        0 2023-04-20 11:53:13.000000 Mongeasy-0.1.8/mongeasy/utils/__init__.py
--rw-rw-rw-   0        0        0     1803 2023-04-20 11:53:13.000000 Mongeasy-0.1.8/mongeasy/utils/utils.py
--rw-rw-rw-   0        0        0       91 2023-04-17 11:07:53.000000 Mongeasy-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0     1057 2023-04-21 10:45:23.640814 Mongeasy-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1106 2023-04-21 10:44:51.000000 Mongeasy-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 10:45:23.638303 Mongeasy-0.1.8/tests/
--rw-rw-rw-   0        0        0       39 2023-04-17 07:50:37.000000 Mongeasy-0.1.8/tests/__init__.py
--rw-rw-rw-   0        0        0    10126 2023-04-20 11:53:13.000000 Mongeasy-0.1.8/tests/test_mongeasy.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-16 12:08:47.744907 Mongeasy-0.1.9/
+-rw-r--r--   0 javv       (501) staff       (20)     1074 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/LICENSE
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-16 12:08:47.718171 Mongeasy-0.1.9/Mongeasy.egg-info/
+-rw-r--r--   0 javv       (501) staff       (20)    11039 2023-06-16 12:08:47.000000 Mongeasy-0.1.9/Mongeasy.egg-info/PKG-INFO
+-rw-r--r--   0 javv       (501) staff       (20)      599 2023-06-16 12:08:47.000000 Mongeasy-0.1.9/Mongeasy.egg-info/SOURCES.txt
+-rw-r--r--   0 javv       (501) staff       (20)        1 2023-06-16 12:08:47.000000 Mongeasy-0.1.9/Mongeasy.egg-info/dependency_links.txt
+-rw-r--r--   0 javv       (501) staff       (20)       47 2023-06-16 12:08:47.000000 Mongeasy-0.1.9/Mongeasy.egg-info/entry_points.txt
+-rw-r--r--   0 javv       (501) staff       (20)       15 2023-06-16 12:08:47.000000 Mongeasy-0.1.9/Mongeasy.egg-info/requires.txt
+-rw-r--r--   0 javv       (501) staff       (20)       15 2023-06-16 12:08:47.000000 Mongeasy-0.1.9/Mongeasy.egg-info/top_level.txt
+-rw-r--r--   0 javv       (501) staff       (20)    11039 2023-06-16 12:08:47.745078 Mongeasy-0.1.9/PKG-INFO
+-rw-r--r--   0 javv       (501) staff       (20)    10228 2023-06-16 12:03:09.000000 Mongeasy-0.1.9/README.md
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-16 12:08:47.726863 Mongeasy-0.1.9/mongeasy/
+-rw-r--r--   0 javv       (501) staff       (20)     2235 2023-06-03 05:07:09.000000 Mongeasy-0.1.9/mongeasy/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)     2692 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/mongeasy/base_dict.py
+-rw-r--r--   0 javv       (501) staff       (20)     2809 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/mongeasy/connection.py
+-rw-r--r--   0 javv       (501) staff       (20)     4690 2023-06-16 10:02:45.000000 Mongeasy-0.1.9/mongeasy/core.py
+-rw-r--r--   0 javv       (501) staff       (20)    12539 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/mongeasy/document.py
+-rw-r--r--   0 javv       (501) staff       (20)     2601 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/mongeasy/dynamics.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-16 12:08:47.730061 Mongeasy-0.1.9/mongeasy/examples/
+-rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/mongeasy/examples/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)     1792 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/mongeasy/exceptions.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-16 12:08:47.731047 Mongeasy-0.1.9/mongeasy/extensions/
+-rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/mongeasy/extensions/__init__.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-16 12:08:47.732038 Mongeasy-0.1.9/mongeasy/plugins/
+-rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/mongeasy/plugins/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)     4842 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/mongeasy/resultlist.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-16 12:08:47.735211 Mongeasy-0.1.9/mongeasy/utils/
+-rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/mongeasy/utils/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)     1755 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/mongeasy/utils/utils.py
+-rw-r--r--   0 javv       (501) staff       (20)       89 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/pyproject.toml
+-rw-r--r--   0 javv       (501) staff       (20)     1013 2023-06-16 12:08:47.746351 Mongeasy-0.1.9/setup.cfg
+-rw-r--r--   0 javv       (501) staff       (20)     1072 2023-06-16 12:04:34.000000 Mongeasy-0.1.9/setup.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-16 12:08:47.741997 Mongeasy-0.1.9/tests/
+-rw-r--r--   0 javv       (501) staff       (20)       38 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/tests/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)    13041 2023-06-16 10:09:31.000000 Mongeasy-0.1.9/tests/test_mongeasy.py
```

### Comparing `Mongeasy-0.1.8/LICENSE` & `Mongeasy-0.1.9/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-MIT License
-
-Copyright (c) 2023, Joakim Wassberg
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
+MIT License
+
+Copyright (c) 2023, Joakim Wassberg
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
```

### Comparing `Mongeasy-0.1.8/Mongeasy.egg-info/PKG-INFO` & `Mongeasy-0.1.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,341 +1,335 @@
-Metadata-Version: 2.1
-Name: Mongeasy
-Version: 0.1.8
-Summary: Easy to use wrapper around pymongo for easy access to MongoDB.
-Home-page: https://github.com/artheadsweden/mongeasy
-Author: Joakim Wassberg
-Author-email: joakim.wassberg@arthead.se
-License: MIT
-Project-URL: Bug Tracker, https://github.com/artheadsweden/mongeasy/issues
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Database
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Mongeasy
-
-Mongeasy is a easy to use library to be used for simple access to a MongoDB database, without any need for schemas or validation. Just store the data as it is used in your application.
-
-### Installation
-Mongoeasy is available on PyPI and can be installed using pip:
-
-```bash
-pip install mongeasy
-```
-
-### Documentation
-The documentation can be found at [https://mongeasy.readthedocs.io](https://mongeasy.readthedocs.io)
-
-### What's new in version 0.1.7?
-* Documents now support raw queries using the `raw_query` method. This method will return a pymongo cursor object that can be used to iterate over the documents in the collection.
-* Documents now support raw aggregation using the `raw_aggregate` method. This method will return a pymongo cursor object that can be used to iterate over the documents in the collection.
-* Extended the Query class to support more operators
-
-### Connection
-Connection to the database is handled automtically for you if you have the conenction information in a configfile or set as environment variables.
-
-#### Connection using configfile
-Create a file called `mongeasy_config.yml` and place it in your project root folder.
-
-The contents of the file should be:
-
-```bash
-db_config:
-  uri: mongodb://localhost:27017
-  database: mydatabase
-```
-
-#### Connection using environment variables
-You can, as an alternative method, define your connection information using environment variables. Just set these two:
-
-```bash
-MONGOEASY_CONNECTION_STRING=mongodb://localhost:27017/
-MONGOEASY_DATABASE_NAME=mydatabase
-```
-
-### Create a document class
-To use Mongeasy you will create a document class that can be used with the collection of choice. To do this you will use the `create_document_class` factory function like this:
-
-```python
-from mongeasy import create_document_class
-
-
-User = create_document_class('User', 'users')
-
-```
-
-The first argument is the name the class will get and the second argument is the name of the collection to use. If the collection does not exist it will be created when you use the class to store documents.
-
-You will not need to assign the returned value to a class variable as in the example above, as the generated class is injected into the current namespace:
-
-```python
-from mongeasy import create_document_class
-
-
-create_document_class('User', 'users')
-
-# The class User exist from this point in the code
-
-```
-
-### Create a store a document
-You can create a documnet by using the generated class. You can either use keyword arguments or pass a dict.
-
-```python
-from mongeasy import create_document_class
-
-
-User = create_document_class('User', 'users')
-
-# Create a document using keyword arguments
-user1 = User(name='Alice', age=25)
-user1.save()
-
-# Create a document using a dict
-user2 = User({'name': 'Bob', 'age': 30})
-user2.save()
-
-```
-
-### Find documents
-You can find documents using the `find` method on the generated class. This method will return a list of documents.
-
-```python
-from mongeasy import create_document_class
-
-
-User = create_document_class('User', 'users')
-
-# Find all documents
-users = User.all()
-
-# Find all documents with age 25
-users = User.find({'age': 25})
-
-```
-#### Find one document
-You can find one document using the `find` method on the generated class.
-
-Find will return a ResultList object that can be used to get the first, or last, document in the list. If no document is found None is returned.
-
-```python
-from mongeasy import create_document_class
-
-
-User = create_document_class('User', 'users')
-
-# Find one document with age 25
-user = User.find({'age': 25}).first()
-
-if user is None:
-    print('No user found')
-
-```
-
-### Update a document
-You can update a document just by changing the attributes and then calling the `save` method.
-
-```python
-from mongeasy import create_document_class
-
-
-User = create_document_class('User', 'users')
-
-# Find one document with age 25
-user = User.find({'age': 25}).first()
-
-if user is None:
-    print('No user found')
-else:
-    # Update the age of the user
-    user.age = 26
-    user.save()
-```
-
-### Delete a document
-You can delete a document by calling the `delete` method on the document.
-
-```python
-from mongeasy import create_document_class
-
-
-User = create_document_class('User', 'users')
-
-# Find one document with age 25
-user = User.find({'age': 25}).first()
-
-if user is None:
-    print('No user found')
-else:
-    # Delete the user
-    user.delete()
-```
-
-You can also delete all documents in a collection by calling the `delete` method on the generated class.
-
-```python
-from mongeasy import create_document_class
-
-
-User = create_document_class('User', 'users')
-
-
-# Delete using a filter
-User.delete({'age': 25})
-
-# Delete all documents in the collection
-User.delete()
-```
-
-### Indexes
-You can create indexes on the collection by using the `create_index` method on the generated class.
-
-```python
-from mongeasy import create_document_class
-
-
-User = create_document_class('User', 'users')
-
-# Create a unique index on the name field
-User.create_index('name', unique=True)
-```
-
-### Other uses
-When you create the document class you have an option to pass additional bases classes. You can use this feature to add functionality to the generated class.
-
-This can also be useful if you want to use Mongeasy with for example flask-login.
-
-```python
-from flask import Flask
-from flask_login import UserMixin, LoginManager
-from mongeasy import create_document_class
-from bson import ObjectId
-
-login_manager = LoginManager()
-# Create User class with mongeasy and UserMixin from flask_login as a base class
-User = create_document_class('User', 'users', base_classes=(UserMixin,))
-def get_id(self):
-    return str(self._id)
-# Add get_id method to User class
-User.get_id = get_id
-
-
-def create_app():
-    app = Flask(__name__)
-   # Define the user loader function for Flask-Login
-    @login_manager.user_loader
-    def load_user(user_id):
-        # Load the user object from the database using the user_id
-        user_id = ObjectId(user_id)
-        user = User.find(_id=user_id).first()
-        return user
-
-    return app
-
-```
-### Query objects
-To simplify queries to the database you can use the mongeasy query object. You construct it and make your query using normal python syntax.
-
-Instead of using a mongodb query like this
-```python
-query = {'$or': [{'$or': [{'name': {'$eq': 'John'}}, {'age': {'$lt': 40}}]}, {'$and': [{'name': {'$eq': 'Jane'}}, {'age': {'$gt': 20}}]}]}
-```
-
-you can accomplish the same thing by using the Query object
-
-```python
-from mongeasy.core import Query
-
-
-query = Query('(name == "John" or age < 40) or (name == "Jane" and age > 20)')
-```
-
-The query can then be used in your queries like this:
-
-```python
-from mongeasy import create_document_class
-from mongeasy.core import Query
-
-
-User = create_document_class('User', 'users')
-query = Query('(name == "John" or age < 40) or (name == "Jane" and age > 20)')
-result = User.find(query)
-```
-
-Supported operators are:
-* ==
-* !=
-* <
-* >
-* <=
-* >=
-* and
-* or
-* not
-* in
-* not in
-
-### ResultList
-All queries that can return more than one document will return a `ResultList` object. This object can be used to get the first or last document in the list, or None if no document is found.
-
-
-```python
-from mongeasy import create_document_class
-
-
-User = create_document_class('User', 'users')
-
-# Find one document with age 25
-user = User.find({'age': 25}).first()
-
-if user is None:
-    print('No user found')
-```
-
-There are also other methods on the `ResultList` object that can be used. These are:
-
-* `first` - Get the first document in the list or None if no document is found
-* `last` - Get the last document in the list or None if no document is found
-* `first_or_none` - Get the first document in the list or None if no document is found, same as first
-* `last_or_none` - Get the last document in the list or None if no document is found, same as last
-* `map` - Apply a given function to each element in the list and return a new ResultList containing the results
-* `filter` - Filter the list using a given function and return a new ResultList containing the results
-* `reduce` - Apply a given function to each element in the list and return a single value
-* `group_by` - Group the list by a given key and return a dict with the results grouped by the key
-* `random` - Get a random document from the list or None if no document is found
-
-### Planned features
-* Enable lazy-loading of query results and support for query chaining
-* Implement a schema plugin system to allow for validation and type checking of documents
-* Add support for transactions using resource management
-* Implement logging and profiling to aid with debugging and performance tuning
-* Enable asynchronous I/O support for improved scalability
-* Implement caching with customizable caching strategies
-* Add support for background tasks using a task queue
-* Implement a paginator utility to allow for pagination of query results
-* Support for MongoDB Atlas search
-* Data migration and seeding utilities
-* Real-time sync feature for monitoring and syncing with another database
-* Automatic data splitting for large documents approaching the 16 MB limit
-* Support for SQL-style auto-increment fields
-* Middleware support for request/response processing
-* Integration with machine learning libraries for data analysis and prediction
-* Built-in analytics to provide insights into database usage and performance
-* Visualization tools to aid with data exploration and presentation
-
-
-### Contributing
-Contributions are welcome. Please create a pull request with your changes.
-
-### Issues
-If you find any issues please create an issue on the github page.
-
-### License
-This project is licensed under the MIT License - see the LICENSE file for details
+# Mongeasy
+
+Mongeasy is a easy to use library to be used for simple access to a MongoDB database, without any need for schemas or validation. Just store the data as it is used in your application.
+
+### Installation
+Mongoeasy is available on PyPI and can be installed using pip:
+
+```bash
+pip install mongeasy
+```
+
+### Documentation
+The documentation can be found at [https://mongeasy.readthedocs.io](https://mongeasy.readthedocs.io)
+
+### What's new in version 0.1.9?
+* Improvement and bugfixes for Query
+
+### Connection
+Connection to the database is handled automtically for you if you have the conenction information in a configfile or set as environment variables.
+
+#### Connection using configfile
+Create a file called `mongeasy_config.yml` and place it in your project root folder.
+
+The contents of the file should be:
+
+```bash
+db_config:
+  uri: mongodb://localhost:27017
+  database: mydatabase
+```
+
+#### Connection using environment variables
+You can, as an alternative method, define your connection information using environment variables. Just set these two:
+
+```bash
+MONGOEASY_CONNECTION_STRING=mongodb://localhost:27017/
+MONGOEASY_DATABASE_NAME=mydatabase
+```
+
+### Create a document class
+To use Mongeasy you will create a document class that can be used with the collection of choice. To do this you will use the `create_document_class` factory function like this:
+
+```python
+from mongeasy import create_document_class
+
+
+User = create_document_class('User', 'users')
+
+```
+
+The first argument is the name the class will get and the second argument is the name of the collection to use. If the collection does not exist it will be created when you use the class to store documents.
+
+You will not need to assign the returned value to a class variable as in the example above, as the generated class is injected into the current namespace:
+
+```python
+from mongeasy import create_document_class
+
+
+create_document_class('User', 'users')
+
+# The class User exist from this point in the code
+
+```
+
+### Create a store a document
+You can create a documnet by using the generated class. You can either use keyword arguments or pass a dict.
+
+```python
+from mongeasy import create_document_class
+
+
+User = create_document_class('User', 'users')
+
+# Create a document using keyword arguments
+user1 = User(name='Alice', age=25)
+user1.save()
+
+# Create a document using a dict
+user2 = User({'name': 'Bob', 'age': 30})
+user2.save()
+
+```
+
+### Find documents
+You can find documents using the `find` method on the generated class. This method will return a list of documents.
+
+```python
+from mongeasy import create_document_class
+
+
+User = create_document_class('User', 'users')
+
+# Find all documents
+users = User.all()
+
+# Find all documents with age 25
+users = User.find({'age': 25})
+
+```
+#### Find one document
+You can find one document using the `find` method on the generated class.
+
+Find will return a ResultList object that can be used to get the first, or last, document in the list. If no document is found None is returned.
+
+```python
+from mongeasy import create_document_class
+
+
+User = create_document_class('User', 'users')
+
+# Find one document with age 25
+user = User.find({'age': 25}).first()
+
+if user is None:
+    print('No user found')
+
+```
+
+### Update a document
+You can update a document just by changing the attributes and then calling the `save` method.
+
+```python
+from mongeasy import create_document_class
+
+
+User = create_document_class('User', 'users')
+
+# Find one document with age 25
+user = User.find({'age': 25}).first()
+
+if user is None:
+    print('No user found')
+else:
+    # Update the age of the user
+    user.age = 26
+    user.save()
+```
+
+### Delete a document
+You can delete a document by calling the `delete` method on the document.
+
+```python
+from mongeasy import create_document_class
+
+
+User = create_document_class('User', 'users')
+
+# Find one document with age 25
+user = User.find({'age': 25}).first()
+
+if user is None:
+    print('No user found')
+else:
+    # Delete the user
+    user.delete()
+```
+
+You can also delete all documents in a collection by calling the `delete` method on the generated class.
+
+```python
+from mongeasy import create_document_class
+
+
+User = create_document_class('User', 'users')
+
+
+# Delete using a filter
+User.delete({'age': 25})
+
+# Delete all documents in the collection
+User.delete()
+```
+
+### Indexes
+You can create indexes on the collection by using the `create_index` method on the generated class.
+
+```python
+from mongeasy import create_document_class
+
+
+User = create_document_class('User', 'users')
+
+# Create a unique index on the name field
+User.create_index('name', unique=True)
+```
+
+### Other uses
+When you create the document class you have an option to pass additional bases classes. You can use this feature to add functionality to the generated class.
+
+This can also be useful if you want to use Mongeasy with for example flask-login.
+
+```python
+from flask import Flask
+from flask_login import UserMixin, LoginManager
+from mongeasy import create_document_class
+from bson import ObjectId
+
+login_manager = LoginManager()
+# Create User class with mongeasy and UserMixin from flask_login as a base class
+User = create_document_class('User', 'users', base_classes=(UserMixin,))
+def get_id(self):
+    return str(self._id)
+# Add get_id method to User class
+User.get_id = get_id
+
+
+def create_app():
+    app = Flask(__name__)
+   # Define the user loader function for Flask-Login
+    @login_manager.user_loader
+    def load_user(user_id):
+        # Load the user object from the database using the user_id
+        user_id = ObjectId(user_id)
+        user = User.find(_id=user_id).first()
+        return user
+
+    return app
+
+```
+### Query objects
+Mongeasy simplifies the process of creating complex database queries by using the Query object. This object allows you to use Python-like syntax for creating your queries, making it easier and more intuitive than using traditional MongoDB queries.
+
+For instance, consider the following MongoDB query:
+
+```python
+query = {'$or': [{'$or': [{'name': {'$eq': 'John'}}, {'age': {'$lt': 40}}]}, {'$and': [{'name': {'$eq': 'Jane'}}, {'age': {'$gt': 20}}]}]}
+```
+
+You can achieve the same result using the Query object:
+
+```python
+from mongeasy.core import Query
+
+query = Query('(name == "John" or age < 40) or (name == "Jane" and age > 20)')
+```
+
+This query can then be used in your database queries like this:
+
+```python
+from mongeasy import create_document_class
+from mongeasy.core import Query
+
+User = create_document_class('User', 'users')
+query = Query('(name == "John" or age < 40) or (name == "Jane" and age > 20)')
+result = User.find(query)
+```
+
+Mongeasy supports the following operators in the Query object:
+
+* `==`: equality
+* `!=`: inequality
+* `<`: less than
+* `>`: greater than
+* `<=`: less than or equal to
+* `>=`: greater than or equal to
+* `and`: logical AND
+* `or`: logical OR
+* `not`: logical NOT
+* `in`: check if a value is in a list
+* `not in`: check if a value is not in a list
+
+You can also access subdocuments or nested fields in your documents using the dot notation:
+
+```python
+query = Query('age > 25 and friends.age == 32')
+```
+
+In case of invalid queries, an error will be raised with detailed information about the problem:
+
+```python
+try:
+    query = Query("age <> 25")  # Invalid operator
+except ValueError as e:
+    print(e)
+```
+
+This approach makes it easier to write, read, and manage your database queries in Python, providing a more user-friendly interface for MongoDB.
+
+### ResultList
+All queries that can return more than one document will return a `ResultList` object. This object can be used to get the first or last document in the list, or None if no document is found.
+
+
+```python
+from mongeasy import create_document_class
+
+
+User = create_document_class('User', 'users')
+
+# Find one document with age 25
+user = User.find({'age': 25}).first()
+
+if user is None:
+    print('No user found')
+```
+
+There are also other methods on the `ResultList` object that can be used. These are:
+
+* `first` - Get the first document in the list or None if no document is found
+* `last` - Get the last document in the list or None if no document is found
+* `first_or_none` - Get the first document in the list or None if no document is found, same as first
+* `last_or_none` - Get the last document in the list or None if no document is found, same as last
+* `map` - Apply a given function to each element in the list and return a new ResultList containing the results
+* `filter` - Filter the list using a given function and return a new ResultList containing the results
+* `reduce` - Apply a given function to each element in the list and return a single value
+* `group_by` - Group the list by a given key and return a dict with the results grouped by the key
+* `random` - Get a random document from the list or None if no document is found
+
+### Planned features
+* Enable lazy-loading of query results and support for query chaining
+* Implement a schema plugin system to allow for validation and type checking of documents
+* Add support for transactions using resource management
+* Implement logging and profiling to aid with debugging and performance tuning
+* Enable asynchronous I/O support for improved scalability
+* Implement caching with customizable caching strategies
+* Add support for background tasks using a task queue
+* Implement a paginator utility to allow for pagination of query results
+* Support for MongoDB Atlas search
+* Data migration and seeding utilities
+* Real-time sync feature for monitoring and syncing with another database
+* Automatic data splitting for large documents approaching the 16 MB limit
+* Support for SQL-style auto-increment fields
+* Middleware support for request/response processing
+* Integration with machine learning libraries for data analysis and prediction
+* Built-in analytics to provide insights into database usage and performance
+* Visualization tools to aid with data exploration and presentation
+
+
+### Contributing
+Contributions are welcome. Please create a pull request with your changes.
+
+### Issues
+If you find any issues please create an issue on the github page.
+
+### License
+This project is licensed under the MIT License - see the LICENSE file for details
```

### Comparing `Mongeasy-0.1.8/Mongeasy.egg-info/SOURCES.txt` & `Mongeasy-0.1.9/Mongeasy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.8/PKG-INFO` & `Mongeasy-0.1.9/Mongeasy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,341 +1,356 @@
-Metadata-Version: 2.1
-Name: Mongeasy
-Version: 0.1.8
-Summary: Easy to use wrapper around pymongo for easy access to MongoDB.
-Home-page: https://github.com/artheadsweden/mongeasy
-Author: Joakim Wassberg
-Author-email: joakim.wassberg@arthead.se
-License: MIT
-Project-URL: Bug Tracker, https://github.com/artheadsweden/mongeasy/issues
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Database
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Mongeasy
-
-Mongeasy is a easy to use library to be used for simple access to a MongoDB database, without any need for schemas or validation. Just store the data as it is used in your application.
-
-### Installation
-Mongoeasy is available on PyPI and can be installed using pip:
-
-```bash
-pip install mongeasy
-```
-
-### Documentation
-The documentation can be found at [https://mongeasy.readthedocs.io](https://mongeasy.readthedocs.io)
-
-### What's new in version 0.1.7?
-* Documents now support raw queries using the `raw_query` method. This method will return a pymongo cursor object that can be used to iterate over the documents in the collection.
-* Documents now support raw aggregation using the `raw_aggregate` method. This method will return a pymongo cursor object that can be used to iterate over the documents in the collection.
-* Extended the Query class to support more operators
-
-### Connection
-Connection to the database is handled automtically for you if you have the conenction information in a configfile or set as environment variables.
-
-#### Connection using configfile
-Create a file called `mongeasy_config.yml` and place it in your project root folder.
-
-The contents of the file should be:
-
-```bash
-db_config:
-  uri: mongodb://localhost:27017
-  database: mydatabase
-```
-
-#### Connection using environment variables
-You can, as an alternative method, define your connection information using environment variables. Just set these two:
-
-```bash
-MONGOEASY_CONNECTION_STRING=mongodb://localhost:27017/
-MONGOEASY_DATABASE_NAME=mydatabase
-```
-
-### Create a document class
-To use Mongeasy you will create a document class that can be used with the collection of choice. To do this you will use the `create_document_class` factory function like this:
-
-```python
-from mongeasy import create_document_class
-
-
-User = create_document_class('User', 'users')
-
-```
-
-The first argument is the name the class will get and the second argument is the name of the collection to use. If the collection does not exist it will be created when you use the class to store documents.
-
-You will not need to assign the returned value to a class variable as in the example above, as the generated class is injected into the current namespace:
-
-```python
-from mongeasy import create_document_class
-
-
-create_document_class('User', 'users')
-
-# The class User exist from this point in the code
-
-```
-
-### Create a store a document
-You can create a documnet by using the generated class. You can either use keyword arguments or pass a dict.
-
-```python
-from mongeasy import create_document_class
-
-
-User = create_document_class('User', 'users')
-
-# Create a document using keyword arguments
-user1 = User(name='Alice', age=25)
-user1.save()
-
-# Create a document using a dict
-user2 = User({'name': 'Bob', 'age': 30})
-user2.save()
-
-```
-
-### Find documents
-You can find documents using the `find` method on the generated class. This method will return a list of documents.
-
-```python
-from mongeasy import create_document_class
-
-
-User = create_document_class('User', 'users')
-
-# Find all documents
-users = User.all()
-
-# Find all documents with age 25
-users = User.find({'age': 25})
-
-```
-#### Find one document
-You can find one document using the `find` method on the generated class.
-
-Find will return a ResultList object that can be used to get the first, or last, document in the list. If no document is found None is returned.
-
-```python
-from mongeasy import create_document_class
-
-
-User = create_document_class('User', 'users')
-
-# Find one document with age 25
-user = User.find({'age': 25}).first()
-
-if user is None:
-    print('No user found')
-
-```
-
-### Update a document
-You can update a document just by changing the attributes and then calling the `save` method.
-
-```python
-from mongeasy import create_document_class
-
-
-User = create_document_class('User', 'users')
-
-# Find one document with age 25
-user = User.find({'age': 25}).first()
-
-if user is None:
-    print('No user found')
-else:
-    # Update the age of the user
-    user.age = 26
-    user.save()
-```
-
-### Delete a document
-You can delete a document by calling the `delete` method on the document.
-
-```python
-from mongeasy import create_document_class
-
-
-User = create_document_class('User', 'users')
-
-# Find one document with age 25
-user = User.find({'age': 25}).first()
-
-if user is None:
-    print('No user found')
-else:
-    # Delete the user
-    user.delete()
-```
-
-You can also delete all documents in a collection by calling the `delete` method on the generated class.
-
-```python
-from mongeasy import create_document_class
-
-
-User = create_document_class('User', 'users')
-
-
-# Delete using a filter
-User.delete({'age': 25})
-
-# Delete all documents in the collection
-User.delete()
-```
-
-### Indexes
-You can create indexes on the collection by using the `create_index` method on the generated class.
-
-```python
-from mongeasy import create_document_class
-
-
-User = create_document_class('User', 'users')
-
-# Create a unique index on the name field
-User.create_index('name', unique=True)
-```
-
-### Other uses
-When you create the document class you have an option to pass additional bases classes. You can use this feature to add functionality to the generated class.
-
-This can also be useful if you want to use Mongeasy with for example flask-login.
-
-```python
-from flask import Flask
-from flask_login import UserMixin, LoginManager
-from mongeasy import create_document_class
-from bson import ObjectId
-
-login_manager = LoginManager()
-# Create User class with mongeasy and UserMixin from flask_login as a base class
-User = create_document_class('User', 'users', base_classes=(UserMixin,))
-def get_id(self):
-    return str(self._id)
-# Add get_id method to User class
-User.get_id = get_id
-
-
-def create_app():
-    app = Flask(__name__)
-   # Define the user loader function for Flask-Login
-    @login_manager.user_loader
-    def load_user(user_id):
-        # Load the user object from the database using the user_id
-        user_id = ObjectId(user_id)
-        user = User.find(_id=user_id).first()
-        return user
-
-    return app
-
-```
-### Query objects
-To simplify queries to the database you can use the mongeasy query object. You construct it and make your query using normal python syntax.
-
-Instead of using a mongodb query like this
-```python
-query = {'$or': [{'$or': [{'name': {'$eq': 'John'}}, {'age': {'$lt': 40}}]}, {'$and': [{'name': {'$eq': 'Jane'}}, {'age': {'$gt': 20}}]}]}
-```
-
-you can accomplish the same thing by using the Query object
-
-```python
-from mongeasy.core import Query
-
-
-query = Query('(name == "John" or age < 40) or (name == "Jane" and age > 20)')
-```
-
-The query can then be used in your queries like this:
-
-```python
-from mongeasy import create_document_class
-from mongeasy.core import Query
-
-
-User = create_document_class('User', 'users')
-query = Query('(name == "John" or age < 40) or (name == "Jane" and age > 20)')
-result = User.find(query)
-```
-
-Supported operators are:
-* ==
-* !=
-* <
-* >
-* <=
-* >=
-* and
-* or
-* not
-* in
-* not in
-
-### ResultList
-All queries that can return more than one document will return a `ResultList` object. This object can be used to get the first or last document in the list, or None if no document is found.
-
-
-```python
-from mongeasy import create_document_class
-
-
-User = create_document_class('User', 'users')
-
-# Find one document with age 25
-user = User.find({'age': 25}).first()
-
-if user is None:
-    print('No user found')
-```
-
-There are also other methods on the `ResultList` object that can be used. These are:
-
-* `first` - Get the first document in the list or None if no document is found
-* `last` - Get the last document in the list or None if no document is found
-* `first_or_none` - Get the first document in the list or None if no document is found, same as first
-* `last_or_none` - Get the last document in the list or None if no document is found, same as last
-* `map` - Apply a given function to each element in the list and return a new ResultList containing the results
-* `filter` - Filter the list using a given function and return a new ResultList containing the results
-* `reduce` - Apply a given function to each element in the list and return a single value
-* `group_by` - Group the list by a given key and return a dict with the results grouped by the key
-* `random` - Get a random document from the list or None if no document is found
-
-### Planned features
-* Enable lazy-loading of query results and support for query chaining
-* Implement a schema plugin system to allow for validation and type checking of documents
-* Add support for transactions using resource management
-* Implement logging and profiling to aid with debugging and performance tuning
-* Enable asynchronous I/O support for improved scalability
-* Implement caching with customizable caching strategies
-* Add support for background tasks using a task queue
-* Implement a paginator utility to allow for pagination of query results
-* Support for MongoDB Atlas search
-* Data migration and seeding utilities
-* Real-time sync feature for monitoring and syncing with another database
-* Automatic data splitting for large documents approaching the 16 MB limit
-* Support for SQL-style auto-increment fields
-* Middleware support for request/response processing
-* Integration with machine learning libraries for data analysis and prediction
-* Built-in analytics to provide insights into database usage and performance
-* Visualization tools to aid with data exploration and presentation
-
-
-### Contributing
-Contributions are welcome. Please create a pull request with your changes.
-
-### Issues
-If you find any issues please create an issue on the github page.
-
-### License
-This project is licensed under the MIT License - see the LICENSE file for details
+Metadata-Version: 2.1
+Name: Mongeasy
+Version: 0.1.9
+Summary: Easy to use wrapper around pymongo for easy access to MongoDB.
+Home-page: https://github.com/artheadsweden/mongeasy
+Author: Joakim Wassberg
+Author-email: joakim.wassberg@arthead.se
+License: MIT
+Project-URL: Bug Tracker, https://github.com/artheadsweden/mongeasy/issues
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Database
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Mongeasy
+
+Mongeasy is a easy to use library to be used for simple access to a MongoDB database, without any need for schemas or validation. Just store the data as it is used in your application.
+
+### Installation
+Mongoeasy is available on PyPI and can be installed using pip:
+
+```bash
+pip install mongeasy
+```
+
+### Documentation
+The documentation can be found at [https://mongeasy.readthedocs.io](https://mongeasy.readthedocs.io)
+
+### What's new in version 0.1.9?
+* Improvement and bugfixes for Query
+
+### Connection
+Connection to the database is handled automtically for you if you have the conenction information in a configfile or set as environment variables.
+
+#### Connection using configfile
+Create a file called `mongeasy_config.yml` and place it in your project root folder.
+
+The contents of the file should be:
+
+```bash
+db_config:
+  uri: mongodb://localhost:27017
+  database: mydatabase
+```
+
+#### Connection using environment variables
+You can, as an alternative method, define your connection information using environment variables. Just set these two:
+
+```bash
+MONGOEASY_CONNECTION_STRING=mongodb://localhost:27017/
+MONGOEASY_DATABASE_NAME=mydatabase
+```
+
+### Create a document class
+To use Mongeasy you will create a document class that can be used with the collection of choice. To do this you will use the `create_document_class` factory function like this:
+
+```python
+from mongeasy import create_document_class
+
+
+User = create_document_class('User', 'users')
+
+```
+
+The first argument is the name the class will get and the second argument is the name of the collection to use. If the collection does not exist it will be created when you use the class to store documents.
+
+You will not need to assign the returned value to a class variable as in the example above, as the generated class is injected into the current namespace:
+
+```python
+from mongeasy import create_document_class
+
+
+create_document_class('User', 'users')
+
+# The class User exist from this point in the code
+
+```
+
+### Create a store a document
+You can create a documnet by using the generated class. You can either use keyword arguments or pass a dict.
+
+```python
+from mongeasy import create_document_class
+
+
+User = create_document_class('User', 'users')
+
+# Create a document using keyword arguments
+user1 = User(name='Alice', age=25)
+user1.save()
+
+# Create a document using a dict
+user2 = User({'name': 'Bob', 'age': 30})
+user2.save()
+
+```
+
+### Find documents
+You can find documents using the `find` method on the generated class. This method will return a list of documents.
+
+```python
+from mongeasy import create_document_class
+
+
+User = create_document_class('User', 'users')
+
+# Find all documents
+users = User.all()
+
+# Find all documents with age 25
+users = User.find({'age': 25})
+
+```
+#### Find one document
+You can find one document using the `find` method on the generated class.
+
+Find will return a ResultList object that can be used to get the first, or last, document in the list. If no document is found None is returned.
+
+```python
+from mongeasy import create_document_class
+
+
+User = create_document_class('User', 'users')
+
+# Find one document with age 25
+user = User.find({'age': 25}).first()
+
+if user is None:
+    print('No user found')
+
+```
+
+### Update a document
+You can update a document just by changing the attributes and then calling the `save` method.
+
+```python
+from mongeasy import create_document_class
+
+
+User = create_document_class('User', 'users')
+
+# Find one document with age 25
+user = User.find({'age': 25}).first()
+
+if user is None:
+    print('No user found')
+else:
+    # Update the age of the user
+    user.age = 26
+    user.save()
+```
+
+### Delete a document
+You can delete a document by calling the `delete` method on the document.
+
+```python
+from mongeasy import create_document_class
+
+
+User = create_document_class('User', 'users')
+
+# Find one document with age 25
+user = User.find({'age': 25}).first()
+
+if user is None:
+    print('No user found')
+else:
+    # Delete the user
+    user.delete()
+```
+
+You can also delete all documents in a collection by calling the `delete` method on the generated class.
+
+```python
+from mongeasy import create_document_class
+
+
+User = create_document_class('User', 'users')
+
+
+# Delete using a filter
+User.delete({'age': 25})
+
+# Delete all documents in the collection
+User.delete()
+```
+
+### Indexes
+You can create indexes on the collection by using the `create_index` method on the generated class.
+
+```python
+from mongeasy import create_document_class
+
+
+User = create_document_class('User', 'users')
+
+# Create a unique index on the name field
+User.create_index('name', unique=True)
+```
+
+### Other uses
+When you create the document class you have an option to pass additional bases classes. You can use this feature to add functionality to the generated class.
+
+This can also be useful if you want to use Mongeasy with for example flask-login.
+
+```python
+from flask import Flask
+from flask_login import UserMixin, LoginManager
+from mongeasy import create_document_class
+from bson import ObjectId
+
+login_manager = LoginManager()
+# Create User class with mongeasy and UserMixin from flask_login as a base class
+User = create_document_class('User', 'users', base_classes=(UserMixin,))
+def get_id(self):
+    return str(self._id)
+# Add get_id method to User class
+User.get_id = get_id
+
+
+def create_app():
+    app = Flask(__name__)
+   # Define the user loader function for Flask-Login
+    @login_manager.user_loader
+    def load_user(user_id):
+        # Load the user object from the database using the user_id
+        user_id = ObjectId(user_id)
+        user = User.find(_id=user_id).first()
+        return user
+
+    return app
+
+```
+### Query objects
+Mongeasy simplifies the process of creating complex database queries by using the Query object. This object allows you to use Python-like syntax for creating your queries, making it easier and more intuitive than using traditional MongoDB queries.
+
+For instance, consider the following MongoDB query:
+
+```python
+query = {'$or': [{'$or': [{'name': {'$eq': 'John'}}, {'age': {'$lt': 40}}]}, {'$and': [{'name': {'$eq': 'Jane'}}, {'age': {'$gt': 20}}]}]}
+```
+
+You can achieve the same result using the Query object:
+
+```python
+from mongeasy.core import Query
+
+query = Query('(name == "John" or age < 40) or (name == "Jane" and age > 20)')
+```
+
+This query can then be used in your database queries like this:
+
+```python
+from mongeasy import create_document_class
+from mongeasy.core import Query
+
+User = create_document_class('User', 'users')
+query = Query('(name == "John" or age < 40) or (name == "Jane" and age > 20)')
+result = User.find(query)
+```
+
+Mongeasy supports the following operators in the Query object:
+
+* `==`: equality
+* `!=`: inequality
+* `<`: less than
+* `>`: greater than
+* `<=`: less than or equal to
+* `>=`: greater than or equal to
+* `and`: logical AND
+* `or`: logical OR
+* `not`: logical NOT
+* `in`: check if a value is in a list
+* `not in`: check if a value is not in a list
+
+You can also access subdocuments or nested fields in your documents using the dot notation:
+
+```python
+query = Query('age > 25 and friends.age == 32')
+```
+
+In case of invalid queries, an error will be raised with detailed information about the problem:
+
+```python
+try:
+    query = Query("age <> 25")  # Invalid operator
+except ValueError as e:
+    print(e)
+```
+
+This approach makes it easier to write, read, and manage your database queries in Python, providing a more user-friendly interface for MongoDB.
+
+### ResultList
+All queries that can return more than one document will return a `ResultList` object. This object can be used to get the first or last document in the list, or None if no document is found.
+
+
+```python
+from mongeasy import create_document_class
+
+
+User = create_document_class('User', 'users')
+
+# Find one document with age 25
+user = User.find({'age': 25}).first()
+
+if user is None:
+    print('No user found')
+```
+
+There are also other methods on the `ResultList` object that can be used. These are:
+
+* `first` - Get the first document in the list or None if no document is found
+* `last` - Get the last document in the list or None if no document is found
+* `first_or_none` - Get the first document in the list or None if no document is found, same as first
+* `last_or_none` - Get the last document in the list or None if no document is found, same as last
+* `map` - Apply a given function to each element in the list and return a new ResultList containing the results
+* `filter` - Filter the list using a given function and return a new ResultList containing the results
+* `reduce` - Apply a given function to each element in the list and return a single value
+* `group_by` - Group the list by a given key and return a dict with the results grouped by the key
+* `random` - Get a random document from the list or None if no document is found
+
+### Planned features
+* Enable lazy-loading of query results and support for query chaining
+* Implement a schema plugin system to allow for validation and type checking of documents
+* Add support for transactions using resource management
+* Implement logging and profiling to aid with debugging and performance tuning
+* Enable asynchronous I/O support for improved scalability
+* Implement caching with customizable caching strategies
+* Add support for background tasks using a task queue
+* Implement a paginator utility to allow for pagination of query results
+* Support for MongoDB Atlas search
+* Data migration and seeding utilities
+* Real-time sync feature for monitoring and syncing with another database
+* Automatic data splitting for large documents approaching the 16 MB limit
+* Support for SQL-style auto-increment fields
+* Middleware support for request/response processing
+* Integration with machine learning libraries for data analysis and prediction
+* Built-in analytics to provide insights into database usage and performance
+* Visualization tools to aid with data exploration and presentation
+
+
+### Contributing
+Contributions are welcome. Please create a pull request with your changes.
+
+### Issues
+If you find any issues please create an issue on the github page.
+
+### License
+This project is licensed under the MIT License - see the LICENSE file for details
```

### Comparing `Mongeasy-0.1.8/mongeasy/__init__.py` & `Mongeasy-0.1.9/mongeasy/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,71 @@
-"""Top-level package for Mongeasy."""
-
-__author__ = """Joakim Wassberg"""
-__email__ = 'joakim.wassberg@arthead.se'
-__version__ = '0.1.8'
-
-from mongeasy.connection import MongeasyConnection
-from mongeasy.exceptions import MongeasyDBConnectionError
-from mongeasy.dynamics import create_document_class
-
-connection = MongeasyConnection()
-
-# connection = None
-
-
-# def get_connection():
-#     return connection
-
-
-# def connect(connection_str: str=None, db_name: str=None):
-#     global connection
-#     if connection is not None:
-#         return connection
-
-#     try:
-#         # Try connecting using connect function
-#         if connection_str and db_name:
-#             connection = pymongo.MongoClient(connection_str)[db_name]
-#             return connection
-#     except Exception as e:
-#         print(e)
-    
-#     connect_from_env()
-#     connect_from_config()
-
-#     if connection is None:
-#         raise MongEasyDBConnectionError("Failed to connect to database using environment variables or config file.")
-
-#     return connection
-
-# def connect_from_env():
-#     global connection
-#     try:
-#         # Try connecting using environment variables
-#         connection_string = os.environ.get('MONGOEASY_CONNECTION_STRING')
-#         database_name = os.environ.get('MONGOEASY_DATABASE_NAME')
-#         if connection_string and database_name:
-#             connection = pymongo.MongoClient(connection_string)[database_name]
-#     except Exception as e:
-#         print(e)
-
-# def connect_from_config():
-#     global connection
-#     try:
-#         # Try connecting using config file
-#         config = configparser.ConfigParser()
-#         config.read('mongeasy.conf')
-#         if 'mongoeasy' in config:
-#             section = config['mongoeasy']
-#             connection_string = section.get('connection_string')
-#             database_name = section.get('database_name')
-#             if connection_string and database_name:
-#                 connection = pymongo.MongoClient(connection_string)[database_name]
-#     except Exception as e:
-#         print(e)
-        
-        
+"""Top-level package for Mongeasy."""
+
+__author__ = """Joakim Wassberg"""
+__email__ = 'joakim.wassberg@arthead.se'
+__version__ = '0.1.8'
+
+from mongeasy.connection import MongeasyConnection
+from mongeasy.exceptions import MongeasyDBConnectionError
+from mongeasy.dynamics import create_document_class
+from mongeasy.core import Query
+
+connection = MongeasyConnection()
+
+def connect(connection_str: str=None, db_name: str=None):
+    connection.connect(connection_str, db_name)
+# connection = None
+
+
+# def get_connection():
+#     return connection
+
+
+# def connect(connection_str: str=None, db_name: str=None):
+#     global connection
+#     if connection is not None:
+#         return connection
+
+#     try:
+#         # Try connecting using connect function
+#         if connection_str and db_name:
+#             connection = pymongo.MongoClient(connection_str)[db_name]
+#             return connection
+#     except Exception as e:
+#         print(e)
+    
+#     connect_from_env()
+#     connect_from_config()
+
+#     if connection is None:
+#         raise MongEasyDBConnectionError("Failed to connect to database using environment variables or config file.")
+
+#     return connection
+
+# def connect_from_env():
+#     global connection
+#     try:
+#         # Try connecting using environment variables
+#         connection_string = os.environ.get('MONGOEASY_CONNECTION_STRING')
+#         database_name = os.environ.get('MONGOEASY_DATABASE_NAME')
+#         if connection_string and database_name:
+#             connection = pymongo.MongoClient(connection_string)[database_name]
+#     except Exception as e:
+#         print(e)
+
+# def connect_from_config():
+#     global connection
+#     try:
+#         # Try connecting using config file
+#         config = configparser.ConfigParser()
+#         config.read('mongeasy.conf')
+#         if 'mongoeasy' in config:
+#             section = config['mongoeasy']
+#             connection_string = section.get('connection_string')
+#             database_name = section.get('database_name')
+#             if connection_string and database_name:
+#                 connection = pymongo.MongoClient(connection_string)[database_name]
+#     except Exception as e:
+#         print(e)
+        
+        
 # connect()
```

### Comparing `Mongeasy-0.1.8/mongeasy/connection.py` & `Mongeasy-0.1.9/mongeasy/connection.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,70 @@
-import yaml
-import os
-import pymongo
-from mongeasy.exceptions import MongeasyDBConnectionError
-
-class MongeasyConnection:
-    def __init__(self, uri=None, database=None, connection_options=None):
-        self.uri = uri
-        self.database = database
-        self.connection_options = {} if connection_options is None else connection_options
-        self.connection_options.setdefault('maxPoolSize', 100)
-        self.connection_options.setdefault('retryWrites', True)
-        self.connection_options.setdefault('retryReads', True)
-        self.check_env()
-        self.check_conf_file()
-
-        if self.uri is None:
-            raise ValueError("No connection string provided.")
-        if self.database is None:
-            raise ValueError("No database name provided.")
-        
-        try:
-            self.client = pymongo.MongoClient(self.uri, **self.connection_options)
-            self.db = self.client[self.database]
-        except (pymongo.errors.ConnectionFailure,
-                pymongo.errors.ServerSelectionTimeoutError,
-                pymongo.errors.ConfigurationError,
-                pymongo.errors.InvalidURI) as e:
-            raise MongeasyDBConnectionError(f'Failed to connect to database: {e}')
-        
-        
-    def check_env(self):
-        if self.uri is None:
-            self.uri = os.environ.get('MONGOEASY_CONNECTION_STRING')
-        if self.database is None:
-            self.database = os.environ.get('MONGOEASY_DATABASE_NAME')
-        if self.connection_options is None:
-            self.connection_options = os.environ.get('MONGOEASY_CONNECTION_OPTIONS')
-
-    def check_conf_file(self):
-        config_path = os.path.join(os.getcwd(), 'mongeasy_config.yml')
-
-        # Check if the configuration file exists
-        if os.path.exists(config_path):
-            # Read the configuration from the file
-            with open(config_path, 'r') as f:
-                config = yaml.safe_load(f)
-                db_config = config.get('db_config', {})
-
-            if self.uri is None:
-                self.uri = db_config.get('uri', None)
-            if self.database is None:
-                self.database = db_config.get('database', None)
-            if self.connection_options is None:
-                self.connection_options = db_config.get('connection_options', None)
-
-    def disconnect(self):
-        self.client.close()
+import yaml
+import os
+import pymongo
+from mongeasy.exceptions import MongeasyDBConnectionError
+
+class MongeasyConnection:
+    def __init__(self, uri=None, database=None, connection_options=None):
+        self.uri = uri
+        self.database = database
+        self.connection_options = {} if connection_options is None else connection_options
+        self.connection_options.setdefault('maxPoolSize', 100)
+        self.connection_options.setdefault('retryWrites', True)
+        self.connection_options.setdefault('retryReads', True)
+        self.check_env()
+        self.check_conf_file()
+
+        if self.uri is None:
+            raise ValueError("No connection string provided.")
+        if self.database is None:
+            raise ValueError("No database name provided.")
+        
+        try:
+            self.client = pymongo.MongoClient(self.uri, **self.connection_options)
+            self.db = self.client[self.database]
+        except (pymongo.errors.ConnectionFailure,
+                pymongo.errors.ServerSelectionTimeoutError,
+                pymongo.errors.ConfigurationError,
+                pymongo.errors.InvalidURI) as e:
+            raise MongeasyDBConnectionError(f'Failed to connect to database: {e}')
+        
+        
+    def check_env(self):
+        if self.uri is None:
+            self.uri = os.environ.get('MONGOEASY_CONNECTION_STRING')
+        if self.database is None:
+            self.database = os.environ.get('MONGOEASY_DATABASE_NAME')
+        if self.connection_options is None:
+            self.connection_options = os.environ.get('MONGOEASY_CONNECTION_OPTIONS')
+
+    def check_conf_file(self):
+        config_path = os.path.join(os.getcwd(), 'mongeasy_config.yml')
+
+        # Check if the configuration file exists
+        if os.path.exists(config_path):
+            # Read the configuration from the file
+            with open(config_path, 'r') as f:
+                config = yaml.safe_load(f)
+                db_config = config.get('db_config', {})
+
+            if self.uri is None:
+                self.uri = db_config.get('uri', None)
+            if self.database is None:
+                self.database = db_config.get('database', None)
+            if self.connection_options is None:
+                self.connection_options = db_config.get('connection_options', None)
+
+    def connect(self, uri=None, database=None, connection_options=None):
+        if uri is not None:
+            self.uri = uri
+        if database is not None:
+            self.database = database
+        if connection_options is not None:
+            self.connection_options = connection_options
+
+        self.client = pymongo.MongoClient(self.uri, **self.connection_options)
+        self.db = self.client[self.database]
+        return self.db
+
+    def disconnect(self):
+        self.client.close()
```

### Comparing `Mongeasy-0.1.8/mongeasy/dynamics.py` & `Mongeasy-0.1.9/mongeasy/dynamics.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-"""
-This module contains the dynamic class generation of document classes.
-
-MIT License
-
-Copyright (c) 2023 Joakim Wassberg
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation 
-files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, 
-copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom 
-the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE 
-WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, 
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-"""
-import inspect
-from typing import Union
-from .utils.utils import pascal_to_snake
-from .document import Document
-from .exceptions import MongeasyValidationException, MongeasyFieldError
-
-
-def create_document_class(class_name: str, collection_name: str = None, base_classes: tuple = ()):
-    """
-    Dynamically create a document class and register it in the calling module's namespace.
-    Args:
-        class_name (str): Name of the class to create.
-        collection_name (str, optional): Name of the collection. Defaults to None. 
-            If None, the collection name will be the snake_case version of the class name with an 's' appended.
-        base_classes (tuple, optional): Optional base classes to be added to the document class. Defaults to ().
-
-    Returns:
-        _type_: The newly created document class.
-    """
-    # Get the calling module
-    frame = inspect.currentframe().f_back
-    calling_module = inspect.getmodule(frame)
-
-    # Dynamically generate the document class
-    from . import connection
-    if collection_name is None:
-        collection_name = pascal_to_snake(class_name) + 's'
-    
-    # Create the collection object
-    collection = connection.db[collection_name]
-    
-    doc_class = type(class_name, base_classes + (Document, ), {'collection':collection})
-
-    # Register the document class in the calling module's namespace
-    setattr(calling_module, class_name, doc_class)
-    
-    return doc_class
+"""
+This module contains the dynamic class generation of document classes.
+
+MIT License
+
+Copyright (c) 2023 Joakim Wassberg
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation 
+files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, 
+copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom 
+the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE 
+WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, 
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+"""
+import inspect
+from typing import Union
+from .utils.utils import pascal_to_snake
+from .document import Document
+from .exceptions import MongeasyValidationException, MongeasyFieldError
+
+
+def create_document_class(class_name: str, collection_name: str = None, base_classes: tuple = ()):
+    """
+    Dynamically create a document class and register it in the calling module's namespace.
+    Args:
+        class_name (str): Name of the class to create.
+        collection_name (str, optional): Name of the collection. Defaults to None. 
+            If None, the collection name will be the snake_case version of the class name with an 's' appended.
+        base_classes (tuple, optional): Optional base classes to be added to the document class. Defaults to ().
+
+    Returns:
+        _type_: The newly created document class.
+    """
+    # Get the calling module
+    frame = inspect.currentframe().f_back
+    calling_module = inspect.getmodule(frame)
+
+    # Dynamically generate the document class
+    from . import connection
+    if collection_name is None:
+        collection_name = pascal_to_snake(class_name) + 's'
+    
+    # Create the collection object
+    collection = connection.db[collection_name]
+    
+    doc_class = type(class_name, base_classes + (Document, ), {'collection':collection})
+
+    # Register the document class in the calling module's namespace
+    setattr(calling_module, class_name, doc_class)
+    
+    return doc_class
```

### Comparing `Mongeasy-0.1.8/mongeasy/resultlist.py` & `Mongeasy-0.1.9/mongeasy/resultlist.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-"""
-This module contains the ResultList class that adds extra features to lists.
-
-MIT License
-
-Copyright (c) 2023 Joakim Wassberg
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation 
-files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, 
-copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom 
-the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE 
-WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, 
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-"""
-import functools
-import random
-
-
-class ResultList(list):
-    """
-    Extends the list class with methods to retrieve the first or last value,
-    or None if the list is empty, and additional methods for filtering,
-    mapping, reducing, sorting, grouping, and selecting a random element.
-    This class is used as a return value for returned documents
-    """
-
-    def first_or_none(self):
-        """
-        Return the first value or None if list is empty
-        :return: First list element or None
-        """
-        return self[0] if len(self) > 0 else None
-    
-    def first(self):
-        """
-        Return the first value or None if list is empty
-        Synonym for first_or_none
-        :return: First list element or None
-        """
-        return self.first_or_none()
-
-    def last_or_none(self):
-        """
-       Return the last value or None if list is empty
-       :return: Last list element or None
-       """
-        return self[-1] if len(self) > 0 else None
-
-    def last(self):
-        """
-        Return the last value or None if list is empty
-        Synonym for last_or_none
-        :return: Last list element or None
-        """
-        return self.last_or_none()
-    
-    
-    def filter(self, predicate):
-        """
-        Return a new ResultList containing only elements that match a given predicate function
-        :param predicate: A function that takes an element and returns a boolean value
-        :return: A new ResultList containing only matching elements
-        """
-        return ResultList(filter(predicate, self))
-
-    def map(self, mapper):
-        """
-        Apply a given function to each element in the list and return a new ResultList containing the results
-        :param mapper: A function that takes an element and returns a new value
-        :return: A new ResultList containing the results of applying the mapper function to each element
-        """
-        return ResultList(map(mapper, self))
-
-    def reduce(self, reducer, initial=None):
-        """
-        Reduce the list to a single value using a given reducer function
-        :param reducer: A function that takes two elements and returns a single value
-        :param initial: An optional initial value to start the reduction
-        :return: The final reduced value
-        """
-        if initial is not None:
-            return functools.reduce(reducer, self, initial)
-        else:
-            return functools.reduce(reducer, self)
-
-    def sort(self, key=None, reverse=False):
-        """
-        Sort the list in place using a given sorting function
-        :param key: A function that takes an element and returns a value to sort by
-        :param reverse: A boolean indicating whether to sort in descending order (default is ascending)
-        :return: None
-        """
-        super().sort(key=key, reverse=reverse)
-
-    def group_by(self, keyfunc):
-        """
-        Group the elements in the list by a given key function and return a dictionary where the keys are the group keys
-        and the values are lists of elements in that group.
-        :param keyfunc: A function that takes an element and returns a key to group by
-        :return: A dictionary of group keys and lists of elements in each group
-        """
-        groups = {}
-        for elem in self:
-            key = keyfunc(elem)
-            if key in groups:
-                groups[key].append(elem)
-            else:
-                groups[key] = [elem]
-        return groups
-
-    def random(self):
-        """
-        Return a random element from the list
-        :return: A random element from the list
-        """
-        return None if len(self) < 1 else random.choice(self)
+"""
+This module contains the ResultList class that adds extra features to lists.
+
+MIT License
+
+Copyright (c) 2023 Joakim Wassberg
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation 
+files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, 
+copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom 
+the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE 
+WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, 
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+"""
+import functools
+import random
+
+
+class ResultList(list):
+    """
+    Extends the list class with methods to retrieve the first or last value,
+    or None if the list is empty, and additional methods for filtering,
+    mapping, reducing, sorting, grouping, and selecting a random element.
+    This class is used as a return value for returned documents
+    """
+
+    def first_or_none(self):
+        """
+        Return the first value or None if list is empty
+        :return: First list element or None
+        """
+        return self[0] if len(self) > 0 else None
+    
+    def first(self):
+        """
+        Return the first value or None if list is empty
+        Synonym for first_or_none
+        :return: First list element or None
+        """
+        return self.first_or_none()
+
+    def last_or_none(self):
+        """
+       Return the last value or None if list is empty
+       :return: Last list element or None
+       """
+        return self[-1] if len(self) > 0 else None
+
+    def last(self):
+        """
+        Return the last value or None if list is empty
+        Synonym for last_or_none
+        :return: Last list element or None
+        """
+        return self.last_or_none()
+    
+    
+    def filter(self, predicate):
+        """
+        Return a new ResultList containing only elements that match a given predicate function
+        :param predicate: A function that takes an element and returns a boolean value
+        :return: A new ResultList containing only matching elements
+        """
+        return ResultList(filter(predicate, self))
+
+    def map(self, mapper):
+        """
+        Apply a given function to each element in the list and return a new ResultList containing the results
+        :param mapper: A function that takes an element and returns a new value
+        :return: A new ResultList containing the results of applying the mapper function to each element
+        """
+        return ResultList(map(mapper, self))
+
+    def reduce(self, reducer, initial=None):
+        """
+        Reduce the list to a single value using a given reducer function
+        :param reducer: A function that takes two elements and returns a single value
+        :param initial: An optional initial value to start the reduction
+        :return: The final reduced value
+        """
+        if initial is not None:
+            return functools.reduce(reducer, self, initial)
+        else:
+            return functools.reduce(reducer, self)
+
+    def sort(self, key=None, reverse=False):
+        """
+        Sort the list in place using a given sorting function
+        :param key: A function that takes an element and returns a value to sort by
+        :param reverse: A boolean indicating whether to sort in descending order (default is ascending)
+        :return: None
+        """
+        super().sort(key=key, reverse=reverse)
+
+    def group_by(self, keyfunc):
+        """
+        Group the elements in the list by a given key function and return a dictionary where the keys are the group keys
+        and the values are lists of elements in that group.
+        :param keyfunc: A function that takes an element and returns a key to group by
+        :return: A dictionary of group keys and lists of elements in each group
+        """
+        groups = {}
+        for elem in self:
+            key = keyfunc(elem)
+            if key in groups:
+                groups[key].append(elem)
+            else:
+                groups[key] = [elem]
+        return groups
+
+    def random(self):
+        """
+        Return a random element from the list
+        :return: A random element from the list
+        """
+        return None if len(self) < 1 else random.choice(self)
```

### Comparing `Mongeasy-0.1.8/mongeasy/utils/utils.py` & `Mongeasy-0.1.9/mongeasy/utils/utils.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-"""
-This module contains misc util functions.
-
-MIT License
-
-Copyright (c) 2023 Joakim Wassberg
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation 
-files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, 
-copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom 
-the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE 
-WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, 
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-"""
-
-def snake_to_pascal(s: str):
-    """
-    Convert a snake_case string to PascalCase.
-
-    Example:
-    snake_to_pascal('my_snake_string') -> 'MySnakeString'
-    """
-    words = s.split('_')
-    return ''.join(w.capitalize() for w in words)
-
-
-def pascal_to_snake(s: str):
-    """
-    Convert a PascalCase string to snake_case.
-
-    Example:
-    pascal_to_snake('MyPascalString') -> 'my_pascal_string'
-    """
-    result = ''
-    for i, c in enumerate(s):
-        if i == 0:
-            result += c.lower()
-        elif c.isupper():
-            result += '_' + c.lower()
-        else:
-            result += c
-    return result
-
+"""
+This module contains misc util functions.
+
+MIT License
+
+Copyright (c) 2023 Joakim Wassberg
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation 
+files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, 
+copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom 
+the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE 
+WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR 
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, 
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+"""
+
+def snake_to_pascal(s: str):
+    """
+    Convert a snake_case string to PascalCase.
+
+    Example:
+    snake_to_pascal('my_snake_string') -> 'MySnakeString'
+    """
+    words = s.split('_')
+    return ''.join(w.capitalize() for w in words)
+
+
+def pascal_to_snake(s: str):
+    """
+    Convert a PascalCase string to snake_case.
+
+    Example:
+    pascal_to_snake('MyPascalString') -> 'my_pascal_string'
+    """
+    result = ''
+    for i, c in enumerate(s):
+        if i == 0:
+            result += c.lower()
+        elif c.isupper():
+            result += '_' + c.lower()
+        else:
+            result += c
+    return result
+
```

### Comparing `Mongeasy-0.1.8/setup.cfg` & `Mongeasy-0.1.9/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,64 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 206d 6f6e 6765 6173 790d 0a76 6572   = mongeasy..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e38 0d0a 6175  sion = 0.1.8..au
-00000030: 7468 6f72 203d 204a 6f61 6b69 6d20 5761  thor = Joakim Wa
-00000040: 7373 6265 7267 0d0a 6175 7468 6f72 5f65  ssberg..author_e
-00000050: 6d61 696c 203d 206a 6f61 6b69 6d2e 7761  mail = joakim.wa
-00000060: 7373 6265 7267 4061 7274 6865 6164 2e73  ssberg@arthead.s
-00000070: 650d 0a64 6573 6372 6970 7469 6f6e 203d  e..description =
-00000080: 2045 6173 7920 746f 2075 7365 2077 7261   Easy to use wra
-00000090: 7070 6572 2061 726f 756e 6420 7079 6d6f  pper around pymo
-000000a0: 6e67 6f20 666f 7220 6561 7379 2061 6363  ngo for easy acc
-000000b0: 6573 7320 746f 204d 6f6e 676f 4442 2e0d  ess to MongoDB..
-000000c0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
-000000d0: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
-000000e0: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
-000000f0: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
-00000100: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
-00000110: 776e 0d0a 7572 6c20 3d20 6874 7470 733a  wn..url = https:
-00000120: 2f2f 6769 7468 7562 2e63 6f6d 2f61 7274  //github.com/art
-00000130: 6865 6164 7377 6564 656e 2f6d 6f6e 6765  headsweden/monge
-00000140: 6173 790d 0a70 726f 6a65 6374 5f75 726c  asy..project_url
-00000150: 7320 3d20 0d0a 0942 7567 2054 7261 636b  s = ...Bug Track
-00000160: 6572 203d 2068 7474 7073 3a2f 2f67 6974  er = https://git
-00000170: 6875 622e 636f 6d2f 6172 7468 6561 6473  hub.com/artheads
-00000180: 7765 6465 6e2f 6d6f 6e67 6561 7379 2f69  weden/mongeasy/i
-00000190: 7373 7565 730d 0a63 6c61 7373 6966 6965  ssues..classifie
-000001a0: 7273 203d 200d 0a09 4465 7665 6c6f 706d  rs = ...Developm
-000001b0: 656e 7420 5374 6174 7573 203a 3a20 3420  ent Status :: 4 
-000001c0: 2d20 4265 7461 0d0a 094c 6963 656e 7365  - Beta...License
-000001d0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-000001e0: 203a 3a20 4d49 5420 4c69 6365 6e73 650d   :: MIT License.
-000001f0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000200: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000210: 203a 3a20 330d 0a09 5072 6f67 7261 6d6d   :: 3...Programm
-00000220: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000230: 5079 7468 6f6e 203a 3a20 332e 380d 0a09  Python :: 3.8...
-00000240: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000250: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000260: 3a20 332e 390d 0a09 5072 6f67 7261 6d6d  : 3.9...Programm
-00000270: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000280: 5079 7468 6f6e 203a 3a20 332e 3130 0d0a  Python :: 3.10..
-00000290: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-000002a0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000002b0: 3a3a 2033 2e31 310d 0a0d 0a5b 6f70 7469  :: 3.11....[opti
-000002c0: 6f6e 735d 0d0a 7061 636b 6167 6573 203d  ons]..packages =
-000002d0: 2066 696e 643a 0d0a 696e 7374 616c 6c5f   find:..install_
-000002e0: 7265 7175 6972 6573 203d 200d 0a09 7079  requires = ...py
-000002f0: 6d6f 6e67 6f3e 3d34 2e33 2e33 0d0a 0d0a  mongo>=4.3.3....
-00000300: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-00000310: 732e 6669 6e64 5d0d 0a65 7863 6c75 6465  s.find]..exclude
-00000320: 203d 200d 0a09 7465 7374 732a 0d0a 0d0a   = ...tests*....
-00000330: 5b6f 7074 696f 6e73 2e65 6e74 7279 5f70  [options.entry_p
-00000340: 6f69 6e74 735d 0d0a 636f 6e73 6f6c 655f  oints]..console_
-00000350: 7363 7269 7074 7320 3d20 0d0a 096d 6f6e  scripts = ...mon
-00000360: 6765 6173 7920 3d20 6d6f 6e67 6561 7379  geasy = mongeasy
-00000370: 2e63 6c69 3a6d 6169 6e0d 0a0d 0a5b 666c  .cli:main....[fl
-00000380: 616b 6538 5d0d 0a6d 6178 2d6c 696e 652d  ake8]..max-line-
-00000390: 6c65 6e67 7468 203d 2031 3230 0d0a 6578  length = 120..ex
-000003a0: 636c 7564 6520 3d20 2e67 6974 2c5f 5f70  clude = .git,__p
-000003b0: 7963 6163 6865 5f5f 2c2e 7665 6e76 2c2e  ycache__,.venv,.
-000003c0: 6567 6773 2c2a 2e65 6767 2d69 6e66 6f0d  eggs,*.egg-info.
-000003d0: 0a0d 0a5b 746f 6f6c 3a70 7974 6573 745d  ...[tool:pytest]
-000003e0: 0d0a 7465 7374 7061 7468 7320 3d20 7465  ..testpaths = te
-000003f0: 7374 730d 0a0d 0a5b 6567 675f 696e 666f  sts....[egg_info
-00000400: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-00000410: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-00000420: 0a                                       .
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 6d6f 6e67 6561 7379 0a76 6572 7369  = mongeasy.versi
+00000020: 6f6e 203d 2030 2e31 2e39 0a61 7574 686f  on = 0.1.9.autho
+00000030: 7220 3d20 4a6f 616b 696d 2057 6173 7362  r = Joakim Wassb
+00000040: 6572 670a 6175 7468 6f72 5f65 6d61 696c  erg.author_email
+00000050: 203d 206a 6f61 6b69 6d2e 7761 7373 6265   = joakim.wassbe
+00000060: 7267 4061 7274 6865 6164 2e73 650a 6465  rg@arthead.se.de
+00000070: 7363 7269 7074 696f 6e20 3d20 4561 7379  scription = Easy
+00000080: 2074 6f20 7573 6520 7772 6170 7065 7220   to use wrapper 
+00000090: 6172 6f75 6e64 2070 796d 6f6e 676f 2066  around pymongo f
+000000a0: 6f72 2065 6173 7920 6163 6365 7373 2074  or easy access t
+000000b0: 6f20 4d6f 6e67 6f44 422e 0a6c 6f6e 675f  o MongoDB..long_
+000000c0: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
+000000d0: 6c65 3a20 5245 4144 4d45 2e6d 640a 6c6f  le: README.md.lo
+000000e0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
+000000f0: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
+00000100: 7874 2f6d 6172 6b64 6f77 6e0a 7572 6c20  xt/markdown.url 
+00000110: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+00000120: 2e63 6f6d 2f61 7274 6865 6164 7377 6564  .com/artheadswed
+00000130: 656e 2f6d 6f6e 6765 6173 790a 7072 6f6a  en/mongeasy.proj
+00000140: 6563 745f 7572 6c73 203d 200a 0942 7567  ect_urls = ..Bug
+00000150: 2054 7261 636b 6572 203d 2068 7474 7073   Tracker = https
+00000160: 3a2f 2f67 6974 6875 622e 636f 6d2f 6172  ://github.com/ar
+00000170: 7468 6561 6473 7765 6465 6e2f 6d6f 6e67  theadsweden/mong
+00000180: 6561 7379 2f69 7373 7565 730a 636c 6173  easy/issues.clas
+00000190: 7369 6669 6572 7320 3d20 0a09 4465 7665  sifiers = ..Deve
+000001a0: 6c6f 706d 656e 7420 5374 6174 7573 203a  lopment Status :
+000001b0: 3a20 3420 2d20 4265 7461 0a09 4c69 6365  : 4 - Beta..Lice
+000001c0: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+000001d0: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
+000001e0: 7365 0a09 5072 6f67 7261 6d6d 696e 6720  se..Programming 
+000001f0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000200: 6f6e 203a 3a20 330a 0950 726f 6772 616d  on :: 3..Program
+00000210: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000220: 2050 7974 686f 6e20 3a3a 2033 2e38 0a09   Python :: 3.8..
+00000230: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000240: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000250: 3a20 332e 390a 0950 726f 6772 616d 6d69  : 3.9..Programmi
+00000260: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000270: 7974 686f 6e20 3a3a 2033 2e31 300a 0950  ython :: 3.10..P
+00000280: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000290: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000002a0: 2033 2e31 310a 0a5b 6f70 7469 6f6e 735d   3.11..[options]
+000002b0: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
+000002c0: 3a0a 696e 7374 616c 6c5f 7265 7175 6972  :.install_requir
+000002d0: 6573 203d 200a 0970 796d 6f6e 676f 3e3d  es = ..pymongo>=
+000002e0: 342e 332e 330a 0a5b 6f70 7469 6f6e 732e  4.3.3..[options.
+000002f0: 7061 636b 6167 6573 2e66 696e 645d 0a65  packages.find].e
+00000300: 7863 6c75 6465 203d 200a 0974 6573 7473  xclude = ..tests
+00000310: 2a0a 0a5b 6f70 7469 6f6e 732e 656e 7472  *..[options.entr
+00000320: 795f 706f 696e 7473 5d0a 636f 6e73 6f6c  y_points].consol
+00000330: 655f 7363 7269 7074 7320 3d20 0a09 6d6f  e_scripts = ..mo
+00000340: 6e67 6561 7379 203d 206d 6f6e 6765 6173  ngeasy = mongeas
+00000350: 792e 636c 693a 6d61 696e 0a0a 5b66 6c61  y.cli:main..[fla
+00000360: 6b65 385d 0a6d 6178 2d6c 696e 652d 6c65  ke8].max-line-le
+00000370: 6e67 7468 203d 2031 3230 0a65 7863 6c75  ngth = 120.exclu
+00000380: 6465 203d 202e 6769 742c 5f5f 7079 6361  de = .git,__pyca
+00000390: 6368 655f 5f2c 2e76 656e 762c 2e65 6767  che__,.venv,.egg
+000003a0: 732c 2a2e 6567 672d 696e 666f 0a0a 5b74  s,*.egg-info..[t
+000003b0: 6f6f 6c3a 7079 7465 7374 5d0a 7465 7374  ool:pytest].test
+000003c0: 7061 7468 7320 3d20 7465 7374 730a 0a5b  paths = tests..[
+000003d0: 6567 675f 696e 666f 5d0a 7461 675f 6275  egg_info].tag_bu
+000003e0: 696c 6420 3d20 0a74 6167 5f64 6174 6520  ild = .tag_date 
+000003f0: 3d20 300a 0a                             = 0..
```

### Comparing `Mongeasy-0.1.8/setup.py` & `Mongeasy-0.1.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-#!/usr/bin/env python
-
-from setuptools import setup, find_packages
-
-with open("README.md", encoding="utf8") as f:
-    readme = f.read()
-
-with open("LICENSE", encoding="utf8") as f:
-    license = f.read()
-
-setup(
-    name="Mongeasy",
-    version="0.1.8",
-    author="Joakim Wassberg",
-    author_email="joakim.wassberg@arthead.se",
-    description="Easy to use wrapper around pymongo for easy access to MongoDB.",
-    long_description=readme,
-    long_description_content_type="text/markdown",
-    url="https://github.com/artheadsweden/mongeasy",
-    license="MIT",
-    classifiers=[
-        "Development Status :: 4 - Beta",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Topic :: Database",
-    ],
-    packages=find_packages(),
-    install_requires=["pymongo>=4.3.3"],
-)
+#!/usr/bin/env python
+
+from setuptools import setup, find_packages
+
+with open("README.md", encoding="utf8") as f:
+    readme = f.read()
+
+with open("LICENSE", encoding="utf8") as f:
+    license = f.read()
+
+setup(
+    name="Mongeasy",
+    version="0.1.9",
+    author="Joakim Wassberg",
+    author_email="joakim.wassberg@arthead.se",
+    description="Easy to use wrapper around pymongo for easy access to MongoDB.",
+    long_description=readme,
+    long_description_content_type="text/markdown",
+    url="https://github.com/artheadsweden/mongeasy",
+    license="MIT",
+    classifiers=[
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Topic :: Database",
+    ],
+    packages=find_packages(),
+    install_requires=["pymongo>=4.3.3"],
+)
```

