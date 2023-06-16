# Comparing `tmp/pytest_print-0.3.1.tar.gz` & `tmp/pytest_print-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_print-0.3.1.tar", last modified: Tue Dec 28 23:46:06 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pytest_print-0.3.1.tar` & `pytest_print-0.3.2.tar`

### file list

```diff
@@ -1,34 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:46:06.103513 pytest_print-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:46:06.099513 pytest_print-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:46:06.099513 pytest_print-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     3257 2021-12-28 23:45:59.000000 pytest_print-0.3.1/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (121)      115 2021-12-28 23:45:59.000000 pytest_print-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1623 2021-12-28 23:45:59.000000 pytest_print-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3196 2021-12-28 23:45:59.000000 pytest_print-0.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     3252 2021-12-28 23:45:59.000000 pytest_print-0.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2021-12-28 23:45:59.000000 pytest_print-0.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4007 2021-12-28 23:46:06.103513 pytest_print-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2578 2021-12-28 23:45:59.000000 pytest_print-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      387 2021-12-28 23:45:59.000000 pytest_print-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      117 2021-12-28 23:45:59.000000 pytest_print-0.3.1/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2729 2021-12-28 23:46:06.103513 pytest_print-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-28 23:45:59.000000 pytest_print-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:46:06.099513 pytest_print-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:46:06.099513 pytest_print-0.3.1/src/pytest_print/
--rw-r--r--   0 runner    (1001) docker     (121)     2420 2021-12-28 23:45:59.000000 pytest_print-0.3.1/src/pytest_print/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-28 23:45:59.000000 pytest_print-0.3.1/src/pytest_print/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)       51 2021-12-28 23:46:06.000000 pytest_print-0.3.1/src/pytest_print/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:46:06.103513 pytest_print-0.3.1/src/pytest_print.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4007 2021-12-28 23:46:06.000000 pytest_print-0.3.1/src/pytest_print.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      603 2021-12-28 23:46:06.000000 pytest_print-0.3.1/src/pytest_print.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-28 23:46:06.000000 pytest_print-0.3.1/src/pytest_print.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2021-12-28 23:46:06.000000 pytest_print-0.3.1/src/pytest_print.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-12-28 23:46:06.000000 pytest_print-0.3.1/src/pytest_print.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-12-28 23:46:06.000000 pytest_print-0.3.1/src/pytest_print.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-28 23:46:05.000000 pytest_print-0.3.1/src/pytest_print.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-28 23:46:06.103513 pytest_print-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2021-12-28 23:45:59.000000 pytest_print-0.3.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      948 2021-12-28 23:45:59.000000 pytest_print-0.3.1/tests/example.py
--rw-r--r--   0 runner    (1001) docker     (121)     3058 2021-12-28 23:45:59.000000 pytest_print-0.3.1/tests/test_print.py
--rw-r--r--   0 runner    (1001) docker     (121)     1576 2021-12-28 23:45:59.000000 pytest_print-0.3.1/tox.ini
--rw-r--r--   0 runner    (1001) docker     (121)      161 2021-12-28 23:45:59.000000 pytest_print-0.3.1/whitelist.txt
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 pytest_print-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 pytest_print-0.3.2/CHANGELOG.md
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 pytest_print-0.3.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 pytest_print-0.3.2/tox.ini
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pytest_print-0.3.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 pytest_print-0.3.2/.github/workflows/check.yml
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 pytest_print-0.3.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 pytest_print-0.3.2/src/pytest_print/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pytest_print-0.3.2/src/pytest_print/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_print-0.3.2/src/pytest_print/py.typed
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pytest_print-0.3.2/tests/conftest.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 pytest_print-0.3.2/tests/example.py
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 pytest_print-0.3.2/tests/test_print.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pytest_print-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 pytest_print-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 pytest_print-0.3.2/README.md
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 pytest_print-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5255 2020-02-02 00:00:00.000000 pytest_print-0.3.2/PKG-INFO
```

### Comparing `pytest_print-0.3.1/CHANGELOG.md` & `pytest_print-0.3.2/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,28 @@
 
 ## [0.3.0](https://github.com/pytest-dev/pytest-print/tree/0.3.0) (2021-06-17)
 
 [Full Changelog](https://github.com/pytest-dev/pytest-print/compare/0.2.1...0.3.0)
 
 **Merged pull requests:**
 
-- Drop python 2 support [\#17](https://github.com/pytest-dev/pytest-print/pull/17) ([gaborbernat](https://github.com/gaborbernat))
-- \[pre-commit.ci\] pre-commit autoupdate [\#14](https://github.com/pytest-dev/pytest-print/pull/14) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
-- \[pre-commit.ci\] pre-commit autoupdate [\#13](https://github.com/pytest-dev/pytest-print/pull/13) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
-- \[pre-commit.ci\] pre-commit autoupdate [\#12](https://github.com/pytest-dev/pytest-print/pull/12) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
-- \[pre-commit.ci\] pre-commit autoupdate [\#11](https://github.com/pytest-dev/pytest-print/pull/11) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
-- \[pre-commit.ci\] pre-commit autoupdate [\#10](https://github.com/pytest-dev/pytest-print/pull/10) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
-- \[pre-commit.ci\] pre-commit autoupdate [\#9](https://github.com/pytest-dev/pytest-print/pull/9) ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
+- Drop python 2 support [\#17](https://github.com/pytest-dev/pytest-print/pull/17)
+  ([gaborbernat](https://github.com/gaborbernat))
+- \[pre-commit.ci\] pre-commit autoupdate [\#14](https://github.com/pytest-dev/pytest-print/pull/14)
+  ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
+- \[pre-commit.ci\] pre-commit autoupdate [\#13](https://github.com/pytest-dev/pytest-print/pull/13)
+  ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
+- \[pre-commit.ci\] pre-commit autoupdate [\#12](https://github.com/pytest-dev/pytest-print/pull/12)
+  ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
+- \[pre-commit.ci\] pre-commit autoupdate [\#11](https://github.com/pytest-dev/pytest-print/pull/11)
+  ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
+- \[pre-commit.ci\] pre-commit autoupdate [\#10](https://github.com/pytest-dev/pytest-print/pull/10)
+  ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
+- \[pre-commit.ci\] pre-commit autoupdate [\#9](https://github.com/pytest-dev/pytest-print/pull/9)
+  ([pre-commit-ci[bot]](https://github.com/apps/pre-commit-ci))
 
 ## [0.2.1](https://github.com/pytest-dev/pytest-print/tree/0.2.1) (2020-10-23)
 
 [Full Changelog](https://github.com/pytest-dev/pytest-print/compare/0.2.0...0.2.1)
 
 **Closed issues:**
 
@@ -28,36 +35,38 @@
 
 ## [0.1.3](https://github.com/pytest-dev/pytest-print/tree/0.1.3) (2019-09-03)
 
 [Full Changelog](https://github.com/pytest-dev/pytest-print/compare/0.1.2...0.1.3)
 
 **Implemented enhancements:**
 
-- allow force on, document flags [\#3](https://github.com/pytest-dev/pytest-print/pull/3) ([gaborbernat](https://github.com/gaborbernat))
+- allow force on, document flags [\#3](https://github.com/pytest-dev/pytest-print/pull/3)
+  ([gaborbernat](https://github.com/gaborbernat))
 
 **Merged pull requests:**
 
-- Remove PyPy special cases [\#4](https://github.com/pytest-dev/pytest-print/pull/4) ([vtbassmatt](https://github.com/vtbassmatt))
+- Remove PyPy special cases [\#4](https://github.com/pytest-dev/pytest-print/pull/4)
+  ([vtbassmatt](https://github.com/vtbassmatt))
 
 ## [0.1.2](https://github.com/pytest-dev/pytest-print/tree/0.1.2) (2018-11-29)
 
 [Full Changelog](https://github.com/pytest-dev/pytest-print/compare/0.1.1...0.1.2)
 
 ## [0.1.1](https://github.com/pytest-dev/pytest-print/tree/0.1.1) (2018-11-15)
 
 [Full Changelog](https://github.com/pytest-dev/pytest-print/compare/0.1.0...0.1.1)
 
 **Closed issues:**
 
-- How to use “pytest\_print” [\#1](https://github.com/pytest-dev/pytest-print/issues/1)
+- How to use “pytest_print” [\#1](https://github.com/pytest-dev/pytest-print/issues/1)
 
 **Merged pull requests:**
 
-- Update setup.py [\#2](https://github.com/pytest-dev/pytest-print/pull/2) ([shashanksingh28](https://github.com/shashanksingh28))
+- Update setup.py [\#2](https://github.com/pytest-dev/pytest-print/pull/2)
+  ([shashanksingh28](https://github.com/shashanksingh28))
 
 ## [0.1.0](https://github.com/pytest-dev/pytest-print/tree/0.1.0) (2018-04-14)
 
 [Full Changelog](https://github.com/pytest-dev/pytest-print/compare/727896d18cab117ad84010086cbc4c9a16d9e8f7...0.1.0)
 
-
-
-\* *This Changelog was automatically generated by [github_changelog_generator](https://github.com/github-changelog-generator/github-changelog-generator)*
+\* _This Changelog was automatically generated by
+[github_changelog_generator](https://github.com/github-changelog-generator/github-changelog-generator)_
```

### Comparing `pytest_print-0.3.1/CODE_OF_CONDUCT.md` & `pytest_print-0.3.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pytest_print-0.3.1/LICENSE.txt` & `pytest_print-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_print-0.3.1/PKG-INFO` & `pytest_print-0.3.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,57 @@
 Metadata-Version: 2.1
-Name: pytest_print
-Version: 0.3.1
+Name: pytest-print
+Version: 0.3.2
 Summary: pytest-print adds the printer fixture you can use to print messages to the user (directly to the pytest runner, not stdout)
-Home-page: https://github.com/pytest-dev/pytest-print#pytest-print
-Maintainer: Bernat Gabor
-Maintainer-email: gaborjbernat@gmail.com
-License: MIT
+Project-URL: Homepage, https://github.com/pytest-dev/pytest-print
 Project-URL: Source, https://github.com/pytest-dev/pytest-print
 Project-URL: Tracker, https://github.com/pytest-dev/pytest-print/issues
-Keywords: pytest,print,debug
-Platform: any
+Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>
+License: 
+        Permission is hereby granted, free of charge, to any person obtaining a
+        copy of this software and associated documentation files (the
+        "Software"), to deal in the Software without restriction, including
+        without limitation the rights to use, copy, modify, merge, publish,
+        distribute, sublicense, and/or sell copies of the Software, and to
+        permit persons to whom the Software is furnished to do so, subject to
+        the following conditions:
+        
+        The above copyright notice and this permission notice shall be included
+        in all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
+        OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+        MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+        IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+        CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
+        TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
+        SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+License-File: LICENSE
+Keywords: env,pytest
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Plugins
-Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: Utilities
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Requires-Dist: pytest>=7.3.2
 Provides-Extra: test
-License-File: LICENSE.txt
+Requires-Dist: covdefaults>=2.3; extra == 'test'
+Requires-Dist: coverage>=7.2.7; extra == 'test'
+Requires-Dist: pytest-mock>=3.11.1; extra == 'test'
+Description-Content-Type: text/markdown
 
 # pytest-print
 
 [![PyPI](https://img.shields.io/pypi/v/pytest-print?style=flat-square)](https://pypi.org/project/pytest-print)
 [![PyPI - Implementation](https://img.shields.io/pypi/implementation/pytest-print?style=flat-square)](https://pypi.org/project/pytest-print)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytest-print?style=flat-square)](https://pypi.org/project/pytest-print)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pytest-print?style=flat-square)](https://pypistats.org/packages/pytest-print)
@@ -61,15 +78,15 @@
 - `--print-relative-time` will print the relative time since the start of the test (display how long it takes to reach
   prints)
 
 ## use cases
 
 ### sub-step reporting
 
-For tests that are long running this can provide a feedback ot the end-user that what is just happening in the
+For tests that are long running this can provide a feedback to the end-user that what is just happening in the
 background.
 
 ```python
 def test_server_parallel_requests(printer, tmpdir):
     printer("create virtual environment into {}".format(tmpdir))
     create_virtual_environment(tmpdir)
 
@@ -90,9 +107,7 @@
     create virtual environment
     start server from virtual env
     do the parallel request test
 PASSED                                                                   [100%]
 
 =========================== 1 passed in 0.02 seconds ===========================
 ```
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytest_print-0.3.1/README.md` & `pytest_print-0.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 - `--print-relative-time` will print the relative time since the start of the test (display how long it takes to reach
   prints)
 
 ## use cases
 
 ### sub-step reporting
 
-For tests that are long running this can provide a feedback ot the end-user that what is just happening in the
+For tests that are long running this can provide a feedback to the end-user that what is just happening in the
 background.
 
 ```python
 def test_server_parallel_requests(printer, tmpdir):
     printer("create virtual environment into {}".format(tmpdir))
     create_virtual_environment(tmpdir)
```

### Comparing `pytest_print-0.3.1/src/pytest_print/__init__.py` & `pytest_print-0.3.2/src/pytest_print/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,21 @@
-from datetime import datetime
-from typing import Callable, Optional
+"""Pytest print functionality."""
+from __future__ import annotations
+
+from timeit import default_timer
+from typing import TYPE_CHECKING, Callable
 
 import pytest
-from _pytest.config.argparsing import Parser
-from _pytest.fixtures import SubRequest
-from _pytest.terminal import TerminalReporter
 
-from .version import __version__
+from ._version import __version__
+
+if TYPE_CHECKING:
+    from _pytest.config.argparsing import Parser
+    from _pytest.fixtures import SubRequest
+    from _pytest.terminal import TerminalReporter
 
 
 def pytest_addoption(parser: Parser) -> None:
     group = parser.getgroup("general")
     group.addoption(
         "--print-relative-time",
         action="store_true",
@@ -25,15 +30,15 @@
         default=False,
         help="By default the plugins if verbosity is greater than zero (-v flag), this forces on",
     )
 
 
 @pytest.fixture(name="printer")
 def printer(request: SubRequest) -> Callable[[str], None]:
-    """pytest plugin to print test progress steps in verbose mode"""
+    """Pytest plugin to print test progress steps in verbose mode."""
     return create_printer(request)
 
 
 @pytest.fixture(scope="session", name="printer_session")
 def printer_session(request: SubRequest) -> Callable[[str], None]:
     return create_printer(request)
 
@@ -44,29 +49,29 @@
         if terminal_reporter is not None:  # pragma: no branch
             state = State(request.config.getoption("pytest_print_relative_time"), terminal_reporter)
             return state.printer
 
     return no_op
 
 
-def no_op(msg: str) -> None:  # noqa: U100
-    """Do nothing"""
+def no_op(msg: str) -> None:  # noqa: ARG001
+    """Do nothing."""
 
 
 class State:
-    def __init__(self, print_relative: bool, reporter: TerminalReporter) -> None:
+    def __init__(self, print_relative: bool, reporter: TerminalReporter) -> None:  # noqa: FBT001
         self._reporter = reporter
-        self._start = datetime.now() if print_relative else None
+        self._start = default_timer() if print_relative else None
         self._print_relative = print_relative
 
     @property
-    def elapsed(self) -> Optional[float]:
+    def elapsed(self) -> float | None:
         if self._start is None:
             return None  # pragma: no cover
-        return (datetime.now() - self._start).total_seconds()
+        return default_timer() - self._start
 
     def printer(self, msg: str) -> None:
         msg = "\t{}{}".format(f"{self.elapsed}\t" if self._print_relative else "", msg)
         self._reporter.write_line(msg)
 
     __slots__ = ("_start", "_print_relative", "_reporter")
```

### Comparing `pytest_print-0.3.1/tests/example.py` & `pytest_print-0.3.2/tests/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from time import sleep
 from typing import Callable, Iterator
 
 import pytest
 
 
 def create_virtual_environment() -> None:
```

### Comparing `pytest_print-0.3.1/tests/test_print.py` & `pytest_print-0.3.2/tests/test_print.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,42 @@
+from __future__ import annotations
+
 from pathlib import Path
 from shutil import copy2
+from typing import TYPE_CHECKING
 
 import pytest
-from _pytest.monkeypatch import MonkeyPatch
-from _pytest.pytester import Testdir
+
+if TYPE_CHECKING:
+    from _pytest.monkeypatch import MonkeyPatch
 
 _EXAMPLE = Path(__file__).parent / "example.py"
 
 
 def test_version() -> None:
     import pytest_print
 
     assert pytest_print.__version__ is not None
 
 
 @pytest.fixture()
-def example(testdir: Testdir) -> Testdir:
-    dest = Path(str(testdir.tmpdir / "test_example.py"))
-    # dest.symlink_to(_EXAMPLE)  # for local debugging use this
+def example(testdir: pytest.Testdir) -> pytest.Testdir:
+    dest = Path(str(testdir.tmpdir)) / "test_example.py"
     copy2(str(_EXAMPLE), str(dest))
     return testdir
 
 
-def test_progress_no_v(example: Testdir) -> None:
+def test_progress_no_v(example: pytest.Testdir) -> None:
     result = example.runpytest()
     result.assert_outcomes(passed=2)
     assert "	start server from virtual env" not in result.outlines
     assert "global peace" not in result.outlines
 
 
-def test_progress_v_no_relative(example: Testdir, monkeypatch: MonkeyPatch) -> None:
+def test_progress_v_no_relative(example: pytest.Testdir, monkeypatch: MonkeyPatch) -> None:
     monkeypatch.setattr("_pytest._io.terminalwriter.get_terminal_width", lambda: 80)
     monkeypatch.setenv("COLUMNS", str(80))
     result_verbose = example.runpytest("-v", "--print")
     result_verbose.assert_outcomes(passed=2)
 
     report_lines = [
         "test_example.py::test_global_peace ",
@@ -50,17 +53,21 @@
         "\tteardown global peace",
     ]
     from_index = result_verbose.outlines.index(report_lines[0])
     found = result_verbose.outlines[from_index : from_index + len(report_lines)]
     assert found == report_lines
 
 
-def test_progress_v_relative(example: Testdir) -> None:
+def test_progress_v_relative(example: pytest.Testdir) -> None:
     result_verbose_relative = example.runpytest(
-        "--print", "-v", "--print-relative-time", "-k", "test_server_parallel_requests"
+        "--print",
+        "-v",
+        "--print-relative-time",
+        "-k",
+        "test_server_parallel_requests",
     )
     out = "\n".join(result_verbose_relative.outlines)
     result_verbose_relative.assert_outcomes(passed=1)
 
     assert "example.py::test_server_parallel_requests " in out, out
     output = (i.split("\t") for i in result_verbose_relative.outlines if i.startswith("\t"))
     found = [(float(relative), msg) for _, relative, msg in output]
@@ -75,12 +82,12 @@
     session = [m for _, m in sorted(i for i in found if "peace" in i[1])]
     assert session == [
         "attempt global peace",
         "teardown global peace",
     ], session
 
 
-def test_progress_no_v_but_with_print_request(example: Testdir) -> None:
+def test_progress_no_v_but_with_print_request(example: pytest.Testdir) -> None:
     result = example.runpytest("--print")
     result.assert_outcomes(passed=2)
     assert "	start server from virtual env" in result.outlines
     assert "	attempt global peace" in result.outlines
```

### Comparing `pytest_print-0.3.1/tox.ini` & `pytest_print-0.3.2/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,72 @@
 [tox]
-envlist =
+requires =
+    tox>=4.2
+env_list =
     fix
+    py312
+    py311
     py310
     py39
     py38
     py37
-    py36
-    pypy3
     type
     readme
-isolated_build = true
 skip_missing_interpreters = true
-minversion = 3.21
 
 [testenv]
 description = run the tests with pytest
-passenv =
-    SSL_CERT_FILE
-setenv =
-    COVERAGE_FILE = {env:COVERAGE_FILE:{toxworkdir}{/}.coverage.{envname}}
-    _COVERAGE_SRC = {envsitepackagesdir}{/}pytest_print
-    _COVERAGE_TEST = {toxinidir}{/}tests
+package = wheel
+wheel_build_env = .pkg
 extras =
     test
+set_env =
+    COVERAGE_FILE = {env:COVERAGE_FILE:{toxworkdir}{/}.coverage.{envname}}
 commands =
     coverage erase
     coverage run -m pytest {tty:--color=yes} \
       --junitxml {toxworkdir}{/}junit.{envname}.xml \
       {posargs:tests}
     coverage combine
     coverage report
     coverage html -d {envtmpdir}{/}htmlcov
-package = wheel
-wheel_build_env = .pkg
 
 [testenv:fix]
 description = run static analysis and style check using flake8
-passenv =
-    {[testenv]passenv}
-    HOMEPATH
-    PROGRAMDATA
 skip_install = true
 deps =
-    pre-commit>=2
+    pre-commit>=3.3.3
+pass_env =
+    HOMEPATH
+    PROGRAMDATA
 commands =
     pre-commit run --all-files --show-diff-on-failure
 
 [testenv:type]
 description = run type check on code base
-setenv =
-    {tty:MYPY_FORCE_COLOR = 1}
 deps =
-    mypy==0.930
+    mypy==1.3
+set_env =
+    {tty:MYPY_FORCE_COLOR = 1}
 commands =
-    mypy src/pytest_print
-    mypy tests
+    mypy --strict src
+    mypy --strict tests
 
 [testenv:readme]
 description = check that the long description is valid
 skip_install = true
 deps =
-    build
-    twine>=3.4
-changedir = {toxinidir}
+    build[virtualenv]>=0.10
+    twine>=4.0.2
+change_dir = {toxinidir}
 commands =
-    python -m build -s -w . -o {envtmpdir}
+    python -m build -o {envtmpdir} .
     twine check {envtmpdir}/*
 
 [testenv:dev]
 description = generate a DEV environment
-usedevelop = true
+package = editable
 extras =
     test
 commands =
     python -m pip list --format=columns
     python -c 'import sys; print(sys.executable)'
```

