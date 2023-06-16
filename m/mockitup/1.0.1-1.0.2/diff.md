# Comparing `tmp/mockitup-1.0.1.tar.gz` & `tmp/mockitup-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mockitup-1.0.1.tar", last modified: Thu Jan 12 14:44:04 2023, max compression
+gzip compressed data, was "mockitup-1.0.2.tar", last modified: Fri Jun 16 05:37:10 2023, max compression
```

## Comparing `mockitup-1.0.1.tar` & `mockitup-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:44:04.141222 mockitup-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-12 14:43:44.000000 mockitup-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-01-12 14:44:04.141222 mockitup-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-01-12 14:43:44.000000 mockitup-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-01-12 14:43:44.000000 mockitup-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 14:44:04.141222 mockitup-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:44:04.141222 mockitup-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:44:04.141222 mockitup-1.0.1/src/mockitup/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-01-12 14:43:44.000000 mockitup-1.0.1/src/mockitup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-01-12 14:43:44.000000 mockitup-1.0.1/src/mockitup/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-01-12 14:43:44.000000 mockitup-1.0.1/src/mockitup/arguments_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-01-12 14:43:44.000000 mockitup-1.0.1/src/mockitup/composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-01-12 14:43:44.000000 mockitup-1.0.1/src/mockitup/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 14:44:04.141222 mockitup-1.0.1/src/mockitup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-01-12 14:44:04.000000 mockitup-1.0.1/src/mockitup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-01-12 14:44:04.000000 mockitup-1.0.1/src/mockitup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 14:44:04.000000 mockitup-1.0.1/src/mockitup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-12 14:44:04.000000 mockitup-1.0.1/src/mockitup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-12 14:44:04.000000 mockitup-1.0.1/src/mockitup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:37:10.242501 mockitup-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-16 05:36:53.000000 mockitup-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-06-16 05:37:10.242501 mockitup-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-06-16 05:36:53.000000 mockitup-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-16 05:36:53.000000 mockitup-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 05:37:10.242501 mockitup-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:37:10.242501 mockitup-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:37:10.242501 mockitup-1.0.2/src/mockitup/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-16 05:36:53.000000 mockitup-1.0.2/src/mockitup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-16 05:36:53.000000 mockitup-1.0.2/src/mockitup/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-16 05:36:53.000000 mockitup-1.0.2/src/mockitup/arguments_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-06-16 05:36:53.000000 mockitup-1.0.2/src/mockitup/composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-16 05:36:53.000000 mockitup-1.0.2/src/mockitup/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:37:10.242501 mockitup-1.0.2/src/mockitup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-06-16 05:37:10.000000 mockitup-1.0.2/src/mockitup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-16 05:37:10.000000 mockitup-1.0.2/src/mockitup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 05:37:10.000000 mockitup-1.0.2/src/mockitup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-16 05:37:10.000000 mockitup-1.0.2/src/mockitup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 05:37:10.000000 mockitup-1.0.2/src/mockitup.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 05:37:10.242501 mockitup-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-16 05:36:53.000000 mockitup-1.0.2/tests/test_async_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-16 05:36:53.000000 mockitup-1.0.2/tests/test_composer.py
```

### Comparing `mockitup-1.0.1/LICENSE` & `mockitup-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mockitup-1.0.1/PKG-INFO` & `mockitup-1.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mockitup
-Version: 1.0.1
+Version: 1.0.2
 Summary: A `unittest.mock` wrapper for easier mocking
 Author-email: Shacham Ginat <shacham6@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Shacham Ginat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -58,15 +58,15 @@
 
 # And now to use the mock
 assert mock.add_five(4) == 9  # SUCCESS
 assert mock.add_five(5) == 10 # SUCCESS
 assert mock.add_five(3) == 8  # FAILED. WE DIDN'T ALLOW THAT TO HAPPEN.
 ```
 
-The library has two main concepts that it uses to configure the mock objects: `allowances`, and `expectations`. 
+The library has two main concepts that it uses to configure the mock objects: `allowances`, and `expectations`.
 
 ### Allowances
 
 ***Allowances*** let us give the mock _permission_ to be invoked in a certain way, without **requiring** it actually being invoked.
 
 ``` python
 from unittest.mock import Mock
@@ -169,15 +169,15 @@
 ```
 
 ## Extra features
 
 `mockitup` contains more features that allow you to test your code more
 efficiently.
 
-Click the following heading for details.
+Click the following headings for details:
 
 <details>
 <summary>Call raises an exception</summary>
 
 In order to make a method raise an exception when called with some input, simply use the `.raises` directive:
 
 ``` python
@@ -278,7 +278,58 @@
 assert mock.pop_number() == 3
 assert mock.pop_number() == 3
 assert mock.pop_number() == 3
 assert mock.pop_number() == 3
 ```
 
 </details>
+
+<details>
+<summary>Wildcard matching</summary>
+
+Up until now, all of the examples presented so far included a strict parametrization of each `expect`ation and `allow`ence.
+But, in some cases, a softer, more dynamic approach is prefered. Luckily, `mockitup` has you covered, in *plenty* of ways:
+
+1. Use `ANY_ARG` when you know that there's an argument, but don't care about it's value:
+    ``` python
+    from unittest.mock import MagicMock
+    from mockitup import ANY_ARG, allow
+
+    mock = MagicMock()
+    allow(mock).call(ANY_ARG, 2).returns(3)
+
+    assert mock.call(1, 2) == 3
+    mock.call(2, 2) == 3
+    ```
+
+2. Use `ANY_ARGS` when you don't care about **any** of the arguments provided to the mock:
+    ``` python
+    from unittest.mock import MagicMock
+    from mockitup import ANY_ARGS, allow
+
+    mock = MagicMock()
+    allow(mock).call(ANY_ARGS).returns(1)
+
+    assert mock.call(1) == 1
+    assert mock.call("lol", 123) == 1
+    assert mock.call([1, 0.1], False, "You get the point") == 1
+
+
+3. Use `PyHamcrest` matchers in order to define expected constraints over the arguments, without defining concrete values:
+
+    ``` python
+    from unittest.mock import Mock
+    from mockitup import allow
+    from hamcrest import any_of
+
+    picky_eater = Mock()
+
+    allow(picky_eater).eat(any_of("pizza", "hamburger")).returns("yum")
+    allow(picky_eater).eat(ANY_ARGS).raises(ValueError())
+
+    assert picky_eater.eat("pizza") == "yum"
+    assert picky_eater.eat("hamburger") == "yum"
+
+    picky_eater.eat("vegetables")  # Will raise a value error.
+    ```
+
+</details>
```

### Comparing `mockitup-1.0.1/README.md` & `mockitup-1.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 # And now to use the mock
 assert mock.add_five(4) == 9  # SUCCESS
 assert mock.add_five(5) == 10 # SUCCESS
 assert mock.add_five(3) == 8  # FAILED. WE DIDN'T ALLOW THAT TO HAPPEN.
 ```
 
-The library has two main concepts that it uses to configure the mock objects: `allowances`, and `expectations`. 
+The library has two main concepts that it uses to configure the mock objects: `allowances`, and `expectations`.
 
 ### Allowances
 
 ***Allowances*** let us give the mock _permission_ to be invoked in a certain way, without **requiring** it actually being invoked.
 
 ``` python
 from unittest.mock import Mock
@@ -138,15 +138,15 @@
 ```
 
 ## Extra features
 
 `mockitup` contains more features that allow you to test your code more
 efficiently.
 
-Click the following heading for details.
+Click the following headings for details:
 
 <details>
 <summary>Call raises an exception</summary>
 
 In order to make a method raise an exception when called with some input, simply use the `.raises` directive:
 
 ``` python
@@ -247,7 +247,58 @@
 assert mock.pop_number() == 3
 assert mock.pop_number() == 3
 assert mock.pop_number() == 3
 assert mock.pop_number() == 3
 ```
 
 </details>
+
+<details>
+<summary>Wildcard matching</summary>
+
+Up until now, all of the examples presented so far included a strict parametrization of each `expect`ation and `allow`ence.
+But, in some cases, a softer, more dynamic approach is prefered. Luckily, `mockitup` has you covered, in *plenty* of ways:
+
+1. Use `ANY_ARG` when you know that there's an argument, but don't care about it's value:
+    ``` python
+    from unittest.mock import MagicMock
+    from mockitup import ANY_ARG, allow
+
+    mock = MagicMock()
+    allow(mock).call(ANY_ARG, 2).returns(3)
+
+    assert mock.call(1, 2) == 3
+    mock.call(2, 2) == 3
+    ```
+
+2. Use `ANY_ARGS` when you don't care about **any** of the arguments provided to the mock:
+    ``` python
+    from unittest.mock import MagicMock
+    from mockitup import ANY_ARGS, allow
+
+    mock = MagicMock()
+    allow(mock).call(ANY_ARGS).returns(1)
+
+    assert mock.call(1) == 1
+    assert mock.call("lol", 123) == 1
+    assert mock.call([1, 0.1], False, "You get the point") == 1
+
+
+3. Use `PyHamcrest` matchers in order to define expected constraints over the arguments, without defining concrete values:
+
+    ``` python
+    from unittest.mock import Mock
+    from mockitup import allow
+    from hamcrest import any_of
+
+    picky_eater = Mock()
+
+    allow(picky_eater).eat(any_of("pizza", "hamburger")).returns("yum")
+    allow(picky_eater).eat(ANY_ARGS).raises(ValueError())
+
+    assert picky_eater.eat("pizza") == "yum"
+    assert picky_eater.eat("hamburger") == "yum"
+
+    picky_eater.eat("vegetables")  # Will raise a value error.
+    ```
+
+</details>
```

### Comparing `mockitup-1.0.1/pyproject.toml` & `mockitup-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 dependencies = [
     "PyHamcrest>=2.0.2",
     "typing-extensions>=3.10.0",
     "PyHamcrest>=2.0.2",
     "typing-extensions>=3.10.0",
 ]
 name = "mockitup"
-version = "1.0.1"
+version = "1.0.2"
 description = "A `unittest.mock` wrapper for easier mocking"
 
 license = { file = "LICENSE" }
 readme = "README.md"
 
 [tool.pdm]
 [tool.pdm.dev-dependencies]
```

### Comparing `mockitup-1.0.1/src/mockitup/actions.py` & `mockitup-1.0.2/src/mockitup/actions.py`

 * *Files identical despite different names*

### Comparing `mockitup-1.0.1/src/mockitup/arguments_matcher.py` & `mockitup-1.0.2/src/mockitup/arguments_matcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,20 +16,21 @@
 
     def _matches(self, args: Tuple[Any], kwargs: Mapping[str, Any]) -> Tuple[bool, str]:
         registered_len = len(self.args) + len(self.kwargs)
         provided_len = len(args) + len(kwargs)
         if registered_len == provided_len == 0:
             return True, "Arguments matched"
 
-        if registered_len != provided_len:
-            return False, "Length of provided positional arguments isn't the same as the registered"
-
+        # Lengths don't have to match in case of `ANY_ARGS` wildcard.
         if self.args[0] is ANY_ARGS:
             return True, "Matched wildcard `ANY_ARGS`"
 
+        if registered_len != provided_len:
+            return False, "Length of provided positional arguments isn't the same as the registered"
+
         for index, (registered, provided) in enumerate(zip(self.args, args)):
             matched = self.__match_values(registered, provided)
             if not matched:
                 return False, (f"Positional arguments at index {index} didn't match "
                                f"(registered: `{registered}`, provided: `{provided}`)")
 
         # Should have same keys
```

### Comparing `mockitup-1.0.1/src/mockitup/composer.py` & `mockitup-1.0.2/src/mockitup/composer.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,9 +219,18 @@
             return action_result.provide_result()
         raise UnregisteredCall(results)
 
 
 class UnregisteredCall(Exception):
 
     def __init__(self, failed_matches: List[ArgumentsMatchResult]):
-        Exception.__init__(self, "Failed all arguments matching, can't finish call")
+        Exception.__init__(self, _assemble_unregistered_call_message(failed_matches))
         self.failed_matches = failed_matches
+
+
+def _assemble_unregistered_call_message(failed_matches: List[ArgumentsMatchResult]) -> str:
+    lines = [
+        "Failed all arguments matching, can't finish call:",
+    ]
+    for failed_match in failed_matches:
+        lines.append(f" - {failed_match.explanation}")
+    return "\n".join(lines)
```

### Comparing `mockitup-1.0.1/src/mockitup/proxies.py` & `mockitup-1.0.2/src/mockitup/proxies.py`

 * *Files identical despite different names*

### Comparing `mockitup-1.0.1/src/mockitup.egg-info/PKG-INFO` & `mockitup-1.0.2/src/mockitup.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mockitup
-Version: 1.0.1
+Version: 1.0.2
 Summary: A `unittest.mock` wrapper for easier mocking
 Author-email: Shacham Ginat <shacham6@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Shacham Ginat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -58,15 +58,15 @@
 
 # And now to use the mock
 assert mock.add_five(4) == 9  # SUCCESS
 assert mock.add_five(5) == 10 # SUCCESS
 assert mock.add_five(3) == 8  # FAILED. WE DIDN'T ALLOW THAT TO HAPPEN.
 ```
 
-The library has two main concepts that it uses to configure the mock objects: `allowances`, and `expectations`. 
+The library has two main concepts that it uses to configure the mock objects: `allowances`, and `expectations`.
 
 ### Allowances
 
 ***Allowances*** let us give the mock _permission_ to be invoked in a certain way, without **requiring** it actually being invoked.
 
 ``` python
 from unittest.mock import Mock
@@ -169,15 +169,15 @@
 ```
 
 ## Extra features
 
 `mockitup` contains more features that allow you to test your code more
 efficiently.
 
-Click the following heading for details.
+Click the following headings for details:
 
 <details>
 <summary>Call raises an exception</summary>
 
 In order to make a method raise an exception when called with some input, simply use the `.raises` directive:
 
 ``` python
@@ -278,7 +278,58 @@
 assert mock.pop_number() == 3
 assert mock.pop_number() == 3
 assert mock.pop_number() == 3
 assert mock.pop_number() == 3
 ```
 
 </details>
+
+<details>
+<summary>Wildcard matching</summary>
+
+Up until now, all of the examples presented so far included a strict parametrization of each `expect`ation and `allow`ence.
+But, in some cases, a softer, more dynamic approach is prefered. Luckily, `mockitup` has you covered, in *plenty* of ways:
+
+1. Use `ANY_ARG` when you know that there's an argument, but don't care about it's value:
+    ``` python
+    from unittest.mock import MagicMock
+    from mockitup import ANY_ARG, allow
+
+    mock = MagicMock()
+    allow(mock).call(ANY_ARG, 2).returns(3)
+
+    assert mock.call(1, 2) == 3
+    mock.call(2, 2) == 3
+    ```
+
+2. Use `ANY_ARGS` when you don't care about **any** of the arguments provided to the mock:
+    ``` python
+    from unittest.mock import MagicMock
+    from mockitup import ANY_ARGS, allow
+
+    mock = MagicMock()
+    allow(mock).call(ANY_ARGS).returns(1)
+
+    assert mock.call(1) == 1
+    assert mock.call("lol", 123) == 1
+    assert mock.call([1, 0.1], False, "You get the point") == 1
+
+
+3. Use `PyHamcrest` matchers in order to define expected constraints over the arguments, without defining concrete values:
+
+    ``` python
+    from unittest.mock import Mock
+    from mockitup import allow
+    from hamcrest import any_of
+
+    picky_eater = Mock()
+
+    allow(picky_eater).eat(any_of("pizza", "hamburger")).returns("yum")
+    allow(picky_eater).eat(ANY_ARGS).raises(ValueError())
+
+    assert picky_eater.eat("pizza") == "yum"
+    assert picky_eater.eat("hamburger") == "yum"
+
+    picky_eater.eat("vegetables")  # Will raise a value error.
+    ```
+
+</details>
```

