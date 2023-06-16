# Comparing `tmp/testflows.asserts-6.5.221019.1152644.tar.gz` & `tmp/testflows.asserts-6.5.230616.1120952.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.asserts-6.5.221019.1152644.tar", last modified: Wed Oct 19 15:26:44 2022, max compression
+gzip compressed data, was "testflows.asserts-6.5.230616.1120952.tar", last modified: Fri Jun 16 12:09:53 2023, max compression
```

## Comparing `testflows.asserts-6.5.221019.1152644.tar` & `testflows.asserts-6.5.230616.1120952.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-10-19 15:26:44.775065 testflows.asserts-6.5.221019.1152644/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2020-09-12 20:31:35.000000 testflows.asserts-6.5.221019.1152644/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       16 2020-09-12 20:31:35.000000 testflows.asserts-6.5.221019.1152644/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     9612 2022-10-19 15:26:44.774065 testflows.asserts-6.5.221019.1152644/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     6972 2020-09-12 20:31:35.000000 testflows.asserts-6.5.221019.1152644/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2022-10-19 15:26:44.775065 testflows.asserts-6.5.221019.1152644/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1597 2022-10-19 15:26:44.000000 testflows.asserts-6.5.221019.1152644/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-10-19 15:26:44.770065 testflows.asserts-6.5.221019.1152644/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-10-19 15:26:44.774065 testflows.asserts-6.5.221019.1152644/testflows/asserts/
--rw-rw-r--   0 user      (1000) user      (1000)     1470 2022-10-19 15:26:44.000000 testflows.asserts-6.5.221019.1152644/testflows/asserts/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    25290 2022-10-19 15:25:58.000000 testflows.asserts-6.5.221019.1152644/testflows/asserts/asserts.py
--rw-rw-r--   0 user      (1000) user      (1000)     5766 2022-10-19 15:25:58.000000 testflows.asserts-6.5.221019.1152644/testflows/asserts/helpers.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-10-19 15:26:44.774065 testflows.asserts-6.5.221019.1152644/testflows.asserts.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     9612 2022-10-19 15:26:44.000000 testflows.asserts-6.5.221019.1152644/testflows.asserts.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      371 2022-10-19 15:26:44.000000 testflows.asserts-6.5.221019.1152644/testflows.asserts.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2022-10-19 15:26:44.000000 testflows.asserts-6.5.221019.1152644/testflows.asserts.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2020-09-16 17:03:09.000000 testflows.asserts-6.5.221019.1152644/testflows.asserts.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       27 2022-10-19 15:26:44.000000 testflows.asserts-6.5.221019.1152644/testflows.asserts.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2022-10-19 15:26:44.000000 testflows.asserts-6.5.221019.1152644/testflows.asserts.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-16 12:09:53.191473 testflows.asserts-6.5.230616.1120952/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-03-13 19:56:48.000000 testflows.asserts-6.5.230616.1120952/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       16 2023-03-13 19:56:48.000000 testflows.asserts-6.5.230616.1120952/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     7427 2023-06-16 12:09:53.191473 testflows.asserts-6.5.230616.1120952/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     6852 2023-03-13 19:57:54.000000 testflows.asserts-6.5.230616.1120952/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-16 12:09:53.191473 testflows.asserts-6.5.230616.1120952/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1597 2023-06-16 12:09:52.000000 testflows.asserts-6.5.230616.1120952/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-16 12:09:53.187473 testflows.asserts-6.5.230616.1120952/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-16 12:09:53.191473 testflows.asserts-6.5.230616.1120952/testflows/asserts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1470 2023-06-16 12:09:52.000000 testflows.asserts-6.5.230616.1120952/testflows/asserts/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    25290 2023-03-13 19:56:48.000000 testflows.asserts-6.5.230616.1120952/testflows/asserts/asserts.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6161 2023-06-15 01:11:04.000000 testflows.asserts-6.5.230616.1120952/testflows/asserts/helpers.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-16 12:09:53.191473 testflows.asserts-6.5.230616.1120952/testflows.asserts.egg-info/
+-rwxrwxr-x   0 user      (1000) user      (1000)     7427 2023-06-16 12:09:53.000000 testflows.asserts-6.5.230616.1120952/testflows.asserts.egg-info/PKG-INFO
+-rwxrwxr-x   0 user      (1000) user      (1000)      386 2023-06-16 12:09:53.000000 testflows.asserts-6.5.230616.1120952/testflows.asserts.egg-info/SOURCES.txt
+-rwxrwxr-x   0 user      (1000) user      (1000)        1 2023-06-16 12:09:53.000000 testflows.asserts-6.5.230616.1120952/testflows.asserts.egg-info/dependency_links.txt
+-rwxrwxr-x   0 user      (1000) user      (1000)        1 2022-12-23 06:55:07.000000 testflows.asserts-6.5.230616.1120952/testflows.asserts.egg-info/not-zip-safe
+-rwxrwxr-x   0 user      (1000) user      (1000)       27 2023-06-16 12:09:53.000000 testflows.asserts-6.5.230616.1120952/testflows.asserts.egg-info/requires.txt
+-rwxrwxr-x   0 user      (1000) user      (1000)       10 2023-06-16 12:09:53.000000 testflows.asserts-6.5.230616.1120952/testflows.asserts.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-16 12:09:53.191473 testflows.asserts-6.5.230616.1120952/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)    28026 2023-03-13 19:56:48.000000 testflows.asserts-6.5.230616.1120952/tests/tests.py
```

### Comparing `testflows.asserts-6.5.221019.1152644/LICENSE` & `testflows.asserts-6.5.230616.1120952/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.asserts-6.5.221019.1152644/PKG-INFO` & `testflows.asserts-6.5.230616.1120952/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,274 +1,271 @@
 Metadata-Version: 2.1
 Name: testflows.asserts
-Version: 6.5.221019.1152644
+Version: 6.5.230616.1120952
 Summary: TestFlows - Asserts Assertion Library
 Home-page: https://github.com/testflows/testflows-asserts
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
-Description: `TestFlows.com Open-Source Software Testing Framework`_ Asserts
-        =================================================================
-        
-        .. image:: https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/testbug-laptop-testflows.png
-           :width: 100%
-           :alt: test bug
-           :align: center
-        
-        **The asserts module is still work in progress and is currently under development.
-        Please use it only for reference.**
-        
-        No magic, intuitive assertion library with descriptive error messages.
-        Works with Python's `assert statement`_ and is inspired by pytest_
-        support for assertions and `grappa-py/grappa`_ descriptive error messages.
-        
-        Currently supports only Python 3.6 or above.
-        
-        Why
-        ***
-        
-        * No special assertion methods.
-          Uses the default `assert statement`_.
-        * No magic.
-          Assertion statements are not modified and the default AssertionError_
-          class is not overridden.
-        * High performance.
-          No extra code is executed if the assertion does not fail unless the assertion has side effects.
-        * No external dependencies.
-        * Simple and clean API.
-        * Compatible with most Python test frameworks.
-        
-        Usage
-        *****
-        
-        Use **error** for a single assert statement
-        
-        .. code-block:: python
-        
-            from testflows.asserts import error
-        
-            assert 1 == 1, error()
-        
-        or use **errors** context manager to wrap multiple assert statements
-        
-        .. code-block:: python
-        
-            from testflows.asserts import errors
-        
-            with errors():
-                assert 1 == 1
-                assert 2 == 2
-        
-        and if you don't want to abort when an assertion fails and would like to
-        keep going then the **errors** context manager supports soft assertions through it's
-        **error** method.
-        
-        .. code-block:: python
-        
-            from testflows.asserts import errors
-        
-            with errors() as soft:
-                with soft.error():
-                    assert 1 == 2
-                assert 2 == 2
-        
-        When an assertion fails a descriptive error message is produced.
-        For example
-        
-            .. code-block:: python
-        
-               from testflows.asserts import error
-        
-               assert 1 == 2, error()
-        
-        produces the following output
-        
-            .. code-block:: bash
-        
-                AssertionError: Oops! Assertion failed
-        
-                The following assertion was not satisfied
-                  assert 1 == 2, error()
-        
-                Assertion values
-                  assert 1 == 2, error()
-                           ^ is = False
-                  assert 1 == 2, error()
-                  ^ is False
-        
-                Where
-                  File 't.py', line 3 in '<module>'
-        
-                0|
-                1|  from testflows.asserts import error
-                2|
-                3|> assert 1 == 2, error()
-        
-        How
-        ***
-        
-        The **asserts** module works similarly to the old implementation of
-        pytest_ assertions. If the assertion fails, the `assert statement`_ is reinterpreted
-        to produce a detailed error message.
-        
-          Therefore, if the assertion statement has a side effect it might not
-          work as expected when an assertion fails.
-        
-        In the pytest_ framework, this problem_ is solved
-        by rewriting the original assertion.
-        The **asserts** module solves this problem_ by explicitly using **values** context manager
-        to store the values of the expression that has a side effect.
-        
-        Installation
-        ************
-        
-        .. code-block:: bash
-        
-            $ ./build; ./install
-        
-        
-        where
-        
-        .. code-block:: bash
-        
-            $ ./build
-        
-        creates a pip installable package in *./dist*, for example
-        
-        .. code-block:: bash
-        
-            $ ls dist/
-            testflows.asserts-4.1.190811.155018.tar.gz
-        
-        and
-        
-        .. code-block:: bash
-        
-            $ ./install
-        
-        uses *sudo pip install* command to perform the system-wide installation.
-        
-        Assertions with side-effects
-        ****************************
-        
-        If assertion has side effects then **values** context manager can be used to
-        address this problem_.
-        
-        The example below demonstrates the problem_.
-        
-        .. code-block:: python
-        
-            from testflows.asserts import error
-        
-            buf = [1]
-            assert buf.append(2) and buf, error()
-        
-        
-        In the code above, the assertion fails and the **buf** list is modified twice. Once
-        when the assertion fails and once when the assertion is reinterpreted when
-        **error()** method is evaluated.
-        
-        The error message that is produced shows the problem_
-        
-        .. code-block:: bash
-        
-            The following assertion was not satisfied
-              assert buf.append(2) and buf, error()
-        
-            Assertion values
-              assert buf.append(2) and buf, error()
-                     ^ is [1, 2, 2]
-              assert buf.append(2) and buf, error()
-                     ^ is = <built-in method append of list object at 0x7f13d1c41248>
-              assert buf.append(2) and buf, error()
-                     ^ is = None
-              assert buf.append(2) and buf, error()
-                                       ^ is [1, 2, 2]
-              assert buf.append(2) and buf, error()
-                                   ^ is = None
-              assert buf.append(2) and buf, error()
-              ^ is False
-        
-            Where
-              File 't.py', line 4 in '<module>'
-        
-            1|  from testflows.asserts import error
-            2|
-            3|  buf = [1]
-            4|> assert buf.append(2) and buf, error()
-        
-        specifically, the lines below show that value of **buf** is [1,2,2] instead
-        of the desired value of [1,2]
-        
-        .. code-block:: bash
-        
-            Assertion values
-              assert buf.append(2) and buf, error()
-                     ^ is [1, 2, 2]
-        
-        In order to work around this problem_, **values** context manager can be used
-        as follows
-        
-        .. code-block:: python
-        
-            from testflows.asserts import values, error
-        
-            buf = [1]
-            with values() as that:
-                assert that(buf.append(2)) and buf, error()
-        
-        
-        
-        and it will produce the error message
-        
-        .. code-block:: bash
-        
-            The following assertion was not satisfied
-              assert that(buf.append(2)) and buf, error()
-        
-            Assertion values
-              assert that(buf.append(2)) and buf, error()
-                     ^ is = None
-              assert that(buf.append(2)) and buf, error()
-                                             ^ is [1, 2]
-              assert that(buf.append(2)) and buf, error()
-                                         ^ is = None
-              assert that(buf.append(2)) and buf, error()
-              ^ is False
-        
-            Where
-              File 't.py', line 5 in '<module>'
-        
-            1|  from testflows.asserts import values, error
-            2|
-            3|  buf = [1]
-            4|  with values() as that:
-            5|>     assert that(buf.append(2)) and buf, error()
-        
-        the lines below show that the **buf** list has the expected value of [1,2]
-        
-        .. code-block:: bash
-        
-              assert that(buf.append(2)) and buf, error()
-                                             ^ is [1, 2]
-        
-        this is because the expression passed to **that** is not reinterpreted and only the
-        result of the expression is stored and used during the generation of the error message.
-        
-          The explicit use of **values** context manager provides a simple solution without
-          any need to rewrite the original assertion statement.
-        
-        .. _problem: http://pybites.blogspot.com/2011/07/behind-scenes-of-pytests-new-assertion.html
-        .. _AssertionError: https://docs.python.org/3/library/exceptions.html#AssertionError
-        .. _`assert statement`: https://docs.python.org/3/reference/simple_stmts.html#assert
-        .. _`grappa-py/grappa`: https://github.com/grappa-py/grappa
-        .. _pytest: https://docs.pytest.org/en/latest/assert.html
-        .. _`TestFlows.com Open-Source Software Testing Framework`: https://testflows.com
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
+License-File: LICENSE
+
+`TestFlows.com Open-Source Software Testing Framework`_ Asserts
+=================================================================
+
+.. image:: https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/testbug-laptop-testflows.png
+   :width: 100%
+   :alt: test bug
+   :align: center
+
+No magic, intuitive assertion library with descriptive error messages.
+Works with Python's `assert statement`_ and is inspired by pytest_
+support for assertions and `grappa-py/grappa`_ descriptive error messages.
+
+Currently supports only Python 3.6 or above.
+
+Why
+***
+
+* No special assertion methods.
+  Uses the default `assert statement`_.
+* No magic.
+  Assertion statements are not modified and the default AssertionError_
+  class is not overridden.
+* High performance.
+  No extra code is executed if the assertion does not fail unless the assertion has side effects.
+* No external dependencies.
+* Simple and clean API.
+* Compatible with most Python test frameworks.
+
+Usage
+*****
+
+Use **error** for a single assert statement
+
+.. code-block:: python
+
+    from testflows.asserts import error
+
+    assert 1 == 1, error()
+
+or use **errors** context manager to wrap multiple assert statements
+
+.. code-block:: python
+
+    from testflows.asserts import errors
+
+    with errors():
+        assert 1 == 1
+        assert 2 == 2
+
+and if you don't want to abort when an assertion fails and would like to
+keep going then the **errors** context manager supports soft assertions through it's
+**error** method.
+
+.. code-block:: python
+
+    from testflows.asserts import errors
+
+    with errors() as soft:
+        with soft.error():
+            assert 1 == 2
+        assert 2 == 2
+
+When an assertion fails a descriptive error message is produced.
+For example
+
+    .. code-block:: python
+
+       from testflows.asserts import error
+
+       assert 1 == 2, error()
+
+produces the following output
+
+    .. code-block:: bash
+
+        AssertionError: Oops! Assertion failed
+
+        The following assertion was not satisfied
+          assert 1 == 2, error()
+
+        Assertion values
+          assert 1 == 2, error()
+                   ^ is = False
+          assert 1 == 2, error()
+          ^ is False
+
+        Where
+          File 't.py', line 3 in '<module>'
+
+        0|
+        1|  from testflows.asserts import error
+        2|
+        3|> assert 1 == 2, error()
+
+How
+***
+
+The **asserts** module works similarly to the old implementation of
+pytest_ assertions. If the assertion fails, the `assert statement`_ is reinterpreted
+to produce a detailed error message.
+
+  Therefore, if the assertion statement has a side effect it might not
+  work as expected when an assertion fails.
+
+In the pytest_ framework, this problem_ is solved
+by rewriting the original assertion.
+The **asserts** module solves this problem_ by explicitly using **values** context manager
+to store the values of the expression that has a side effect.
+
+Installation
+************
+
+.. code-block:: bash
+
+    $ ./build; ./install
+
+
+where
+
+.. code-block:: bash
+
+    $ ./build
+
+creates a pip installable package in *./dist*, for example
+
+.. code-block:: bash
+
+    $ ls dist/
+    testflows.asserts-4.1.190811.155018.tar.gz
+
+and
+
+.. code-block:: bash
+
+    $ ./install
+
+uses *sudo pip install* command to perform the system-wide installation.
+
+Assertions with side-effects
+****************************
+
+If assertion has side effects then **values** context manager can be used to
+address this problem_.
+
+The example below demonstrates the problem_.
+
+.. code-block:: python
+
+    from testflows.asserts import error
+
+    buf = [1]
+    assert buf.append(2) and buf, error()
+
+
+In the code above, the assertion fails and the **buf** list is modified twice. Once
+when the assertion fails and once when the assertion is reinterpreted when
+**error()** method is evaluated.
+
+The error message that is produced shows the problem_
+
+.. code-block:: bash
+
+    The following assertion was not satisfied
+      assert buf.append(2) and buf, error()
+
+    Assertion values
+      assert buf.append(2) and buf, error()
+             ^ is [1, 2, 2]
+      assert buf.append(2) and buf, error()
+             ^ is = <built-in method append of list object at 0x7f13d1c41248>
+      assert buf.append(2) and buf, error()
+             ^ is = None
+      assert buf.append(2) and buf, error()
+                               ^ is [1, 2, 2]
+      assert buf.append(2) and buf, error()
+                           ^ is = None
+      assert buf.append(2) and buf, error()
+      ^ is False
+
+    Where
+      File 't.py', line 4 in '<module>'
+
+    1|  from testflows.asserts import error
+    2|
+    3|  buf = [1]
+    4|> assert buf.append(2) and buf, error()
+
+specifically, the lines below show that value of **buf** is [1,2,2] instead
+of the desired value of [1,2]
+
+.. code-block:: bash
+
+    Assertion values
+      assert buf.append(2) and buf, error()
+             ^ is [1, 2, 2]
+
+In order to work around this problem_, **values** context manager can be used
+as follows
+
+.. code-block:: python
+
+    from testflows.asserts import values, error
+
+    buf = [1]
+    with values() as that:
+        assert that(buf.append(2)) and buf, error()
+
+
+
+and it will produce the error message
+
+.. code-block:: bash
+
+    The following assertion was not satisfied
+      assert that(buf.append(2)) and buf, error()
+
+    Assertion values
+      assert that(buf.append(2)) and buf, error()
+             ^ is = None
+      assert that(buf.append(2)) and buf, error()
+                                     ^ is [1, 2]
+      assert that(buf.append(2)) and buf, error()
+                                 ^ is = None
+      assert that(buf.append(2)) and buf, error()
+      ^ is False
+
+    Where
+      File 't.py', line 5 in '<module>'
+
+    1|  from testflows.asserts import values, error
+    2|
+    3|  buf = [1]
+    4|  with values() as that:
+    5|>     assert that(buf.append(2)) and buf, error()
+
+the lines below show that the **buf** list has the expected value of [1,2]
+
+.. code-block:: bash
+
+      assert that(buf.append(2)) and buf, error()
+                                     ^ is [1, 2]
+
+this is because the expression passed to **that** is not reinterpreted and only the
+result of the expression is stored and used during the generation of the error message.
+
+  The explicit use of **values** context manager provides a simple solution without
+  any need to rewrite the original assertion statement.
+
+.. _problem: http://pybites.blogspot.com/2011/07/behind-scenes-of-pytests-new-assertion.html
+.. _AssertionError: https://docs.python.org/3/library/exceptions.html#AssertionError
+.. _`assert statement`: https://docs.python.org/3/reference/simple_stmts.html#assert
+.. _`grappa-py/grappa`: https://github.com/grappa-py/grappa
+.. _pytest: https://docs.pytest.org/en/latest/assert.html
+.. _`TestFlows.com Open-Source Software Testing Framework`: https://testflows.com
```

### Comparing `testflows.asserts-6.5.221019.1152644/README.rst` & `testflows.asserts-6.5.230616.1120952/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 =================================================================
 
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/testbug-laptop-testflows.png
    :width: 100%
    :alt: test bug
    :align: center
 
-**The asserts module is still work in progress and is currently under development.
-Please use it only for reference.**
-
 No magic, intuitive assertion library with descriptive error messages.
 Works with Python's `assert statement`_ and is inspired by pytest_
 support for assertions and `grappa-py/grappa`_ descriptive error messages.
 
 Currently supports only Python 3.6 or above.
 
 Why
```

### Comparing `testflows.asserts-6.5.221019.1152644/setup.py` & `testflows.asserts-6.5.230616.1120952/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from setuptools import setup
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 setup(
     name="testflows.asserts",
-    version="6.5.221019.1152644",
+    version="6.5.230616.1120952",
     description="TestFlows - Asserts Assertion Library",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/testflows-asserts",
     classifiers=[
```

### Comparing `testflows.asserts-6.5.221019.1152644/testflows/asserts/__init__.py` & `testflows.asserts-6.5.230616.1120952/testflows/asserts/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "6.5.221019.1152644"
+__version__ = "6.5.230616.1120952"
 __license__ = f"""
 Copyright 2019 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.asserts-6.5.221019.1152644/testflows/asserts/asserts.py` & `testflows.asserts-6.5.230616.1120952/testflows/asserts/asserts.py`

 * *Files identical despite different names*

### Comparing `testflows.asserts-6.5.221019.1152644/testflows/asserts/helpers.py` & `testflows.asserts-6.5.230616.1120952/testflows/asserts/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -75,47 +75,51 @@
                     frame_info=self.frame_info,
                     nodes=[],
                 )
             )
         return True
 
 
-def snapshot(value, id=None, output=None, path=None, name="snapshot", encoder=repr):
+def snapshot(value, id=None, output=None, path=None, name="snapshot", encoder=repr, comment=None):
     """Compare value representation to a stored snapshot.
     If snapshot does not exist, assertion passes else
     representation of the value is compared to the stored snapshot.
 
     Snapshot files have format:
 
         <test file name>[.<id>].snapshot
 
     :param value: value to be used for snapshot
     :param id: unique id of the snapshot file, default: `None`
     :param output: function to output the representation of the value
     :param path: custom snapshot path, default: `./snapshots`
     :param name: name of the snapshot value inside the snapshots file, default: `snapshot`
     :param encoder: custom snapshot encoder, default: `repr`
+    :param comment: optional comment to be added at the end of the snapshot value
     """
     name = varname(name) if name != "snapshot" else name
 
     class SnapshotError(object):
-        def __init__(self, filename, name, snapshot_value, actual_value, diff=None):
+        def __init__(self, filename, name, snapshot_value, actual_value, comment=None, diff=None):
             self.snapshot_value = snapshot_value
             self.actual_value = actual_value
             self.diff = diff
             self.filename = str(filename)
             self.name = str(name)
+            self.comment = str(comment) if comment is not None else None
 
         def __bool__(self):
             return False
 
         def __repr__(self):
             r = "SnapshotError("
             r += "\nfilename=" + self.filename
             r += "\nname=" + self.name
+            if comment is not None:
+                r += "\ncomment=" + self.comment
             r += '\nsnapshot_value="""\n'
             r += textwrap.indent(self.snapshot_value, " " * 4)
             r += '""",\nactual_value="""\n'
             r += textwrap.indent(self.actual_value, " " * 4)
             r += '""",\ndiff="""\n'
             r += textwrap.indent(
                 "\n".join(
@@ -161,16 +165,20 @@
 
     if os.path.exists(filename):
         module_name = f"snapshot_{hashlib.sha1(os.path.abspath(filename).encode('utf-8')).hexdigest()}"
         snapshot_module = SourceFileLoader(module_name, filename).load_module()
         if hasattr(snapshot_module, name):
             snapshot_value = getattr(snapshot_module, name)
             if not (snapshot_value == repr_value):
-                return SnapshotError(filename, name, snapshot_value, repr_value)
+                return SnapshotError(filename, name, snapshot_value, repr_value, comment)
             return True
 
     # no snapshot, so just store the representation
     with open(filename, "a") as fd:
         repr_value = repr_value.replace('"""', '""" + \'"""\' + r"""')
-        fd.write(f'''{name} = r"""{repr_value}"""\n\n''')
+        if comment is not None:
+            comment = f" # {comment}"
+        else:
+            comment = ""
+        fd.write(f'''{name} = r"""{repr_value}"""{comment}\n\n''')
 
     return True
```

### Comparing `testflows.asserts-6.5.221019.1152644/testflows.asserts.egg-info/PKG-INFO` & `testflows.asserts-6.5.230616.1120952/testflows.asserts.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,274 +1,271 @@
 Metadata-Version: 2.1
 Name: testflows.asserts
-Version: 6.5.221019.1152644
+Version: 6.5.230616.1120952
 Summary: TestFlows - Asserts Assertion Library
 Home-page: https://github.com/testflows/testflows-asserts
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
-Description: `TestFlows.com Open-Source Software Testing Framework`_ Asserts
-        =================================================================
-        
-        .. image:: https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/testbug-laptop-testflows.png
-           :width: 100%
-           :alt: test bug
-           :align: center
-        
-        **The asserts module is still work in progress and is currently under development.
-        Please use it only for reference.**
-        
-        No magic, intuitive assertion library with descriptive error messages.
-        Works with Python's `assert statement`_ and is inspired by pytest_
-        support for assertions and `grappa-py/grappa`_ descriptive error messages.
-        
-        Currently supports only Python 3.6 or above.
-        
-        Why
-        ***
-        
-        * No special assertion methods.
-          Uses the default `assert statement`_.
-        * No magic.
-          Assertion statements are not modified and the default AssertionError_
-          class is not overridden.
-        * High performance.
-          No extra code is executed if the assertion does not fail unless the assertion has side effects.
-        * No external dependencies.
-        * Simple and clean API.
-        * Compatible with most Python test frameworks.
-        
-        Usage
-        *****
-        
-        Use **error** for a single assert statement
-        
-        .. code-block:: python
-        
-            from testflows.asserts import error
-        
-            assert 1 == 1, error()
-        
-        or use **errors** context manager to wrap multiple assert statements
-        
-        .. code-block:: python
-        
-            from testflows.asserts import errors
-        
-            with errors():
-                assert 1 == 1
-                assert 2 == 2
-        
-        and if you don't want to abort when an assertion fails and would like to
-        keep going then the **errors** context manager supports soft assertions through it's
-        **error** method.
-        
-        .. code-block:: python
-        
-            from testflows.asserts import errors
-        
-            with errors() as soft:
-                with soft.error():
-                    assert 1 == 2
-                assert 2 == 2
-        
-        When an assertion fails a descriptive error message is produced.
-        For example
-        
-            .. code-block:: python
-        
-               from testflows.asserts import error
-        
-               assert 1 == 2, error()
-        
-        produces the following output
-        
-            .. code-block:: bash
-        
-                AssertionError: Oops! Assertion failed
-        
-                The following assertion was not satisfied
-                  assert 1 == 2, error()
-        
-                Assertion values
-                  assert 1 == 2, error()
-                           ^ is = False
-                  assert 1 == 2, error()
-                  ^ is False
-        
-                Where
-                  File 't.py', line 3 in '<module>'
-        
-                0|
-                1|  from testflows.asserts import error
-                2|
-                3|> assert 1 == 2, error()
-        
-        How
-        ***
-        
-        The **asserts** module works similarly to the old implementation of
-        pytest_ assertions. If the assertion fails, the `assert statement`_ is reinterpreted
-        to produce a detailed error message.
-        
-          Therefore, if the assertion statement has a side effect it might not
-          work as expected when an assertion fails.
-        
-        In the pytest_ framework, this problem_ is solved
-        by rewriting the original assertion.
-        The **asserts** module solves this problem_ by explicitly using **values** context manager
-        to store the values of the expression that has a side effect.
-        
-        Installation
-        ************
-        
-        .. code-block:: bash
-        
-            $ ./build; ./install
-        
-        
-        where
-        
-        .. code-block:: bash
-        
-            $ ./build
-        
-        creates a pip installable package in *./dist*, for example
-        
-        .. code-block:: bash
-        
-            $ ls dist/
-            testflows.asserts-4.1.190811.155018.tar.gz
-        
-        and
-        
-        .. code-block:: bash
-        
-            $ ./install
-        
-        uses *sudo pip install* command to perform the system-wide installation.
-        
-        Assertions with side-effects
-        ****************************
-        
-        If assertion has side effects then **values** context manager can be used to
-        address this problem_.
-        
-        The example below demonstrates the problem_.
-        
-        .. code-block:: python
-        
-            from testflows.asserts import error
-        
-            buf = [1]
-            assert buf.append(2) and buf, error()
-        
-        
-        In the code above, the assertion fails and the **buf** list is modified twice. Once
-        when the assertion fails and once when the assertion is reinterpreted when
-        **error()** method is evaluated.
-        
-        The error message that is produced shows the problem_
-        
-        .. code-block:: bash
-        
-            The following assertion was not satisfied
-              assert buf.append(2) and buf, error()
-        
-            Assertion values
-              assert buf.append(2) and buf, error()
-                     ^ is [1, 2, 2]
-              assert buf.append(2) and buf, error()
-                     ^ is = <built-in method append of list object at 0x7f13d1c41248>
-              assert buf.append(2) and buf, error()
-                     ^ is = None
-              assert buf.append(2) and buf, error()
-                                       ^ is [1, 2, 2]
-              assert buf.append(2) and buf, error()
-                                   ^ is = None
-              assert buf.append(2) and buf, error()
-              ^ is False
-        
-            Where
-              File 't.py', line 4 in '<module>'
-        
-            1|  from testflows.asserts import error
-            2|
-            3|  buf = [1]
-            4|> assert buf.append(2) and buf, error()
-        
-        specifically, the lines below show that value of **buf** is [1,2,2] instead
-        of the desired value of [1,2]
-        
-        .. code-block:: bash
-        
-            Assertion values
-              assert buf.append(2) and buf, error()
-                     ^ is [1, 2, 2]
-        
-        In order to work around this problem_, **values** context manager can be used
-        as follows
-        
-        .. code-block:: python
-        
-            from testflows.asserts import values, error
-        
-            buf = [1]
-            with values() as that:
-                assert that(buf.append(2)) and buf, error()
-        
-        
-        
-        and it will produce the error message
-        
-        .. code-block:: bash
-        
-            The following assertion was not satisfied
-              assert that(buf.append(2)) and buf, error()
-        
-            Assertion values
-              assert that(buf.append(2)) and buf, error()
-                     ^ is = None
-              assert that(buf.append(2)) and buf, error()
-                                             ^ is [1, 2]
-              assert that(buf.append(2)) and buf, error()
-                                         ^ is = None
-              assert that(buf.append(2)) and buf, error()
-              ^ is False
-        
-            Where
-              File 't.py', line 5 in '<module>'
-        
-            1|  from testflows.asserts import values, error
-            2|
-            3|  buf = [1]
-            4|  with values() as that:
-            5|>     assert that(buf.append(2)) and buf, error()
-        
-        the lines below show that the **buf** list has the expected value of [1,2]
-        
-        .. code-block:: bash
-        
-              assert that(buf.append(2)) and buf, error()
-                                             ^ is [1, 2]
-        
-        this is because the expression passed to **that** is not reinterpreted and only the
-        result of the expression is stored and used during the generation of the error message.
-        
-          The explicit use of **values** context manager provides a simple solution without
-          any need to rewrite the original assertion statement.
-        
-        .. _problem: http://pybites.blogspot.com/2011/07/behind-scenes-of-pytests-new-assertion.html
-        .. _AssertionError: https://docs.python.org/3/library/exceptions.html#AssertionError
-        .. _`assert statement`: https://docs.python.org/3/reference/simple_stmts.html#assert
-        .. _`grappa-py/grappa`: https://github.com/grappa-py/grappa
-        .. _pytest: https://docs.pytest.org/en/latest/assert.html
-        .. _`TestFlows.com Open-Source Software Testing Framework`: https://testflows.com
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
+License-File: LICENSE
+
+`TestFlows.com Open-Source Software Testing Framework`_ Asserts
+=================================================================
+
+.. image:: https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/testbug-laptop-testflows.png
+   :width: 100%
+   :alt: test bug
+   :align: center
+
+No magic, intuitive assertion library with descriptive error messages.
+Works with Python's `assert statement`_ and is inspired by pytest_
+support for assertions and `grappa-py/grappa`_ descriptive error messages.
+
+Currently supports only Python 3.6 or above.
+
+Why
+***
+
+* No special assertion methods.
+  Uses the default `assert statement`_.
+* No magic.
+  Assertion statements are not modified and the default AssertionError_
+  class is not overridden.
+* High performance.
+  No extra code is executed if the assertion does not fail unless the assertion has side effects.
+* No external dependencies.
+* Simple and clean API.
+* Compatible with most Python test frameworks.
+
+Usage
+*****
+
+Use **error** for a single assert statement
+
+.. code-block:: python
+
+    from testflows.asserts import error
+
+    assert 1 == 1, error()
+
+or use **errors** context manager to wrap multiple assert statements
+
+.. code-block:: python
+
+    from testflows.asserts import errors
+
+    with errors():
+        assert 1 == 1
+        assert 2 == 2
+
+and if you don't want to abort when an assertion fails and would like to
+keep going then the **errors** context manager supports soft assertions through it's
+**error** method.
+
+.. code-block:: python
+
+    from testflows.asserts import errors
+
+    with errors() as soft:
+        with soft.error():
+            assert 1 == 2
+        assert 2 == 2
+
+When an assertion fails a descriptive error message is produced.
+For example
+
+    .. code-block:: python
+
+       from testflows.asserts import error
+
+       assert 1 == 2, error()
+
+produces the following output
+
+    .. code-block:: bash
+
+        AssertionError: Oops! Assertion failed
+
+        The following assertion was not satisfied
+          assert 1 == 2, error()
+
+        Assertion values
+          assert 1 == 2, error()
+                   ^ is = False
+          assert 1 == 2, error()
+          ^ is False
+
+        Where
+          File 't.py', line 3 in '<module>'
+
+        0|
+        1|  from testflows.asserts import error
+        2|
+        3|> assert 1 == 2, error()
+
+How
+***
+
+The **asserts** module works similarly to the old implementation of
+pytest_ assertions. If the assertion fails, the `assert statement`_ is reinterpreted
+to produce a detailed error message.
+
+  Therefore, if the assertion statement has a side effect it might not
+  work as expected when an assertion fails.
+
+In the pytest_ framework, this problem_ is solved
+by rewriting the original assertion.
+The **asserts** module solves this problem_ by explicitly using **values** context manager
+to store the values of the expression that has a side effect.
+
+Installation
+************
+
+.. code-block:: bash
+
+    $ ./build; ./install
+
+
+where
+
+.. code-block:: bash
+
+    $ ./build
+
+creates a pip installable package in *./dist*, for example
+
+.. code-block:: bash
+
+    $ ls dist/
+    testflows.asserts-4.1.190811.155018.tar.gz
+
+and
+
+.. code-block:: bash
+
+    $ ./install
+
+uses *sudo pip install* command to perform the system-wide installation.
+
+Assertions with side-effects
+****************************
+
+If assertion has side effects then **values** context manager can be used to
+address this problem_.
+
+The example below demonstrates the problem_.
+
+.. code-block:: python
+
+    from testflows.asserts import error
+
+    buf = [1]
+    assert buf.append(2) and buf, error()
+
+
+In the code above, the assertion fails and the **buf** list is modified twice. Once
+when the assertion fails and once when the assertion is reinterpreted when
+**error()** method is evaluated.
+
+The error message that is produced shows the problem_
+
+.. code-block:: bash
+
+    The following assertion was not satisfied
+      assert buf.append(2) and buf, error()
+
+    Assertion values
+      assert buf.append(2) and buf, error()
+             ^ is [1, 2, 2]
+      assert buf.append(2) and buf, error()
+             ^ is = <built-in method append of list object at 0x7f13d1c41248>
+      assert buf.append(2) and buf, error()
+             ^ is = None
+      assert buf.append(2) and buf, error()
+                               ^ is [1, 2, 2]
+      assert buf.append(2) and buf, error()
+                           ^ is = None
+      assert buf.append(2) and buf, error()
+      ^ is False
+
+    Where
+      File 't.py', line 4 in '<module>'
+
+    1|  from testflows.asserts import error
+    2|
+    3|  buf = [1]
+    4|> assert buf.append(2) and buf, error()
+
+specifically, the lines below show that value of **buf** is [1,2,2] instead
+of the desired value of [1,2]
+
+.. code-block:: bash
+
+    Assertion values
+      assert buf.append(2) and buf, error()
+             ^ is [1, 2, 2]
+
+In order to work around this problem_, **values** context manager can be used
+as follows
+
+.. code-block:: python
+
+    from testflows.asserts import values, error
+
+    buf = [1]
+    with values() as that:
+        assert that(buf.append(2)) and buf, error()
+
+
+
+and it will produce the error message
+
+.. code-block:: bash
+
+    The following assertion was not satisfied
+      assert that(buf.append(2)) and buf, error()
+
+    Assertion values
+      assert that(buf.append(2)) and buf, error()
+             ^ is = None
+      assert that(buf.append(2)) and buf, error()
+                                     ^ is [1, 2]
+      assert that(buf.append(2)) and buf, error()
+                                 ^ is = None
+      assert that(buf.append(2)) and buf, error()
+      ^ is False
+
+    Where
+      File 't.py', line 5 in '<module>'
+
+    1|  from testflows.asserts import values, error
+    2|
+    3|  buf = [1]
+    4|  with values() as that:
+    5|>     assert that(buf.append(2)) and buf, error()
+
+the lines below show that the **buf** list has the expected value of [1,2]
+
+.. code-block:: bash
+
+      assert that(buf.append(2)) and buf, error()
+                                     ^ is [1, 2]
+
+this is because the expression passed to **that** is not reinterpreted and only the
+result of the expression is stored and used during the generation of the error message.
+
+  The explicit use of **values** context manager provides a simple solution without
+  any need to rewrite the original assertion statement.
+
+.. _problem: http://pybites.blogspot.com/2011/07/behind-scenes-of-pytests-new-assertion.html
+.. _AssertionError: https://docs.python.org/3/library/exceptions.html#AssertionError
+.. _`assert statement`: https://docs.python.org/3/reference/simple_stmts.html#assert
+.. _`grappa-py/grappa`: https://github.com/grappa-py/grappa
+.. _pytest: https://docs.pytest.org/en/latest/assert.html
+.. _`TestFlows.com Open-Source Software Testing Framework`: https://testflows.com
```

