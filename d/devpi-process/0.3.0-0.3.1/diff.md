# Comparing `tmp/devpi_process-0.3.0.tar.gz` & `tmp/devpi_process-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devpi_process-0.3.0.tar", last modified: Sat Dec  3 22:52:15 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `devpi_process-0.3.0.tar` & `devpi_process-0.3.1.tar`

### file list

```diff
@@ -1,38 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 22:52:15.693089 devpi_process-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 22:52:15.689089 devpi_process-0.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2022-12-03 22:52:08.000000 devpi_process-0.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 22:52:15.689089 devpi_process-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2022-12-03 22:52:08.000000 devpi_process-0.3.0/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2022-12-03 22:52:08.000000 devpi_process-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-03 22:52:08.000000 devpi_process-0.3.0/.markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2022-12-03 22:52:08.000000 devpi_process-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      245 2022-12-03 22:52:08.000000 devpi_process-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2022-12-03 22:52:08.000000 devpi_process-0.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2022-12-03 22:52:08.000000 devpi_process-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2022-12-03 22:52:15.693089 devpi_process-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2022-12-03 22:52:08.000000 devpi_process-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2022-12-03 22:52:08.000000 devpi_process-0.3.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      644 2022-12-03 22:52:08.000000 devpi_process-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2022-12-03 22:52:15.693089 devpi_process-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-03 22:52:08.000000 devpi_process-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 22:52:15.689089 devpi_process-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 22:52:15.693089 devpi_process-0.3.0/src/devpi_process/
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2022-12-03 22:52:08.000000 devpi_process-0.3.0/src/devpi_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-03 22:52:08.000000 devpi_process-0.3.0/src/devpi_process/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       51 2022-12-03 22:52:15.000000 devpi_process-0.3.0/src/devpi_process/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 22:52:15.693089 devpi_process-0.3.0/src/devpi_process.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2022-12-03 22:52:15.000000 devpi_process-0.3.0/src/devpi_process.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2022-12-03 22:52:15.000000 devpi_process-0.3.0/src/devpi_process.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-03 22:52:15.000000 devpi_process-0.3.0/src/devpi_process.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-03 22:52:15.000000 devpi_process-0.3.0/src/devpi_process.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2022-12-03 22:52:15.000000 devpi_process-0.3.0/src/devpi_process.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-03 22:52:15.000000 devpi_process-0.3.0/src/devpi_process.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 22:52:15.693089 devpi_process-0.3.0/src/pytest_devpi/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-03 22:52:08.000000 devpi_process-0.3.0/src/pytest_devpi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 22:52:15.693089 devpi_process-0.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-03 22:52:15.693089 devpi_process-0.3.0/tests/demo_pkg_inline/
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2022-12-03 22:52:08.000000 devpi_process-0.3.0/tests/demo_pkg_inline/build.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-03 22:52:08.000000 devpi_process-0.3.0/tests/demo_pkg_inline/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2022-12-03 22:52:08.000000 devpi_process-0.3.0/tests/test_devpi_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2022-12-03 22:52:08.000000 devpi_process-0.3.0/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-03 22:52:08.000000 devpi_process-0.3.0/whitelist.txt
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 devpi_process-0.3.1/.markdownlint.yaml
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 devpi_process-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 devpi_process-0.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 devpi_process-0.3.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 devpi_process-0.3.1/tox.ini
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 devpi_process-0.3.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 devpi_process-0.3.1/.github/workflows/check.yml
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 devpi_process-0.3.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     7264 2020-02-02 00:00:00.000000 devpi_process-0.3.1/src/devpi_process/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 devpi_process-0.3.1/src/devpi_process/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 devpi_process-0.3.1/src/devpi_process/py.typed
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 devpi_process-0.3.1/tests/test_devpi_process.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 devpi_process-0.3.1/tests/demo_pkg_inline/build.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 devpi_process-0.3.1/tests/demo_pkg_inline/pyproject.toml
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 devpi_process-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 devpi_process-0.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 devpi_process-0.3.1/README.md
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 devpi_process-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 devpi_process-0.3.1/PKG-INFO
```

### Comparing `devpi_process-0.3.0/.github/workflows/check.yml` & `devpi_process-0.3.1/.github/workflows/check.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 name: check
 on:
   push:
+    tags-ignore: ["**"]
   pull_request:
   schedule:
     - cron: "0 8 * * *"
 
 concurrency:
   group: check-${{ github.ref }}
   cancel-in-progress: true
@@ -15,20 +16,19 @@
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         py:
           - "3.11"
           - "3.10"
-          - "pypy-3.7-v7.3.7" # ahead to start it earlier because takes longer
           - "3.9"
           - "3.8"
           - "3.7"
         os:
-          - ubuntu-22.04
+          - ubuntu-latest
           - windows-2022
           - macos-12
 
     steps:
       - name: Setup python for tox
         uses: actions/setup-python@v4
         with:
@@ -61,15 +61,15 @@
   check:
     name: tox env ${{ matrix.tox_env }} - ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os:
-          - ubuntu-22.04
+          - ubuntu-latest
           - windows-2022
         tox_env:
           - dev
           - type
           - readme
         exclude:
           - { os: windows-2022, tox_env: readme }
@@ -83,30 +83,7 @@
           python-version: "3.11"
       - name: Install tox
         run: python -m pip install tox
       - name: Setup test suite
         run: tox -vv --notest -e ${{ matrix.tox_env }}
       - name: Run test suite
         run: tox --skip-pkg-install -e ${{ matrix.tox_env }}
-
-  publish:
-    if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
-    needs: [check, test]
-    runs-on: ubuntu-latest
-    steps:
-      - name: Setup python to build package
-        uses: actions/setup-python@v4
-        with:
-          python-version: "3.11"
-      - name: Install build
-        run: python -m pip install build
-      - uses: actions/checkout@v3
-        with:
-          fetch-depth: 0
-      - name: Build sdist and wheel
-        run: python -m build -s -w . -o dist
-      - name: Publish to PyPi
-        uses: pypa/gh-action-pypi-publish@v1.5.2
-        with:
-          skip_existing: true
-          user: __token__
-          password: ${{ secrets.pypi_password }}
```

### Comparing `devpi_process-0.3.0/CODE_OF_CONDUCT.md` & `devpi_process-0.3.1/CODE_OF_CONDUCT.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,17 @@
 project or its community. Examples of representing a project or community include using an official project e-mail
 address, posting via an official social media account, or acting as an appointed representative at an online or offline
 event. Representation of a project may be further defined and clarified by project maintainers.
 
 ## Enforcement
 
 Instances of abusive, harassing, or otherwise unacceptable behavior may be reported by contacting the project team at
-tox-dev@python.org. The project team will review and investigate all complaints, and will respond in a way that it deems
-appropriate to the circumstances. The project team is obligated to maintain confidentiality with regard to the reporter
-of an incident. Further details of specific enforcement policies may be posted separately.
+`tox-dev@python.org`. The project team will review and investigate all complaints, and will respond in a way that it
+deems appropriate to the circumstances. The project team is obligated to maintain confidentiality with regard to the
+reporter of an incident. Further details of specific enforcement policies may be posted separately.
 
 Project maintainers who do not follow or enforce the Code of Conduct in good faith may face temporary or permanent
 repercussions as determined by other members of the project's leadership.
 
 ## Attribution
 
 This Code of Conduct is adapted from the [Contributor Covenant][homepage], version 1.4, available at
```

### Comparing `devpi_process-0.3.0/LICENSE.txt` & `devpi_process-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `devpi_process-0.3.0/PKG-INFO` & `devpi_process-0.3.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: devpi_process
-Version: 0.3.0
-Summary: devpi process provides a programmatic API to create and use a devpi server process
-Home-page: https://github.com/tox-dev/devpi-process
-Maintainer: Bernat Gabor
-Maintainer-email: gaborjbernat@gmail.com
-License: MIT
-Project-URL: Source, https://github.com/tox-dev/devpi-process
-Project-URL: Tracker, https://github.com/tox-dev/devpi-process
-Keywords: devpi,programmatic
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE.txt
-
 # devpi-process
 
 [![PyPI](https://img.shields.io/pypi/v/devpi-process?style=flat-square)](https://pypi.org/project/devpi-process)
 [![PyPI - Implementation](https://img.shields.io/pypi/implementation/devpi-process?style=flat-square)](https://pypi.org/project/devpi-process)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/devpi-process?style=flat-square)](https://pypi.org/project/devpi-process)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/devpi-process?style=flat-square)](https://pypistats.org/packages/devpi-process)
 [![PyPI - License](https://img.shields.io/pypi/l/devpi-process?style=flat-square)](https://opensource.org/licenses/MIT)
```

### Comparing `devpi_process-0.3.0/src/devpi_process/__init__.py` & `devpi_process-0.3.1/src/devpi_process/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,98 @@
+"""Devpi PyPI to test with."""
 from __future__ import annotations
 
 import random
 import socket
 import string
 import sys
 import sysconfig
 from contextlib import closing
 from pathlib import Path
 from subprocess import PIPE, Popen, run
 from threading import Thread
-from types import TracebackType
-from typing import IO, Iterator, Sequence, cast
+from typing import IO, TYPE_CHECKING, Iterator, Sequence, cast
 
-from .version import __version__
+from ._version import __version__
+
+if TYPE_CHECKING:
+    from types import TracebackType
 
 
 def _check_call(cmd: list[str]) -> None:
-    run(cmd, check=True, stdout=PIPE, stderr=PIPE)
+    run(cmd, check=True, capture_output=True)  # noqa: S603
 
 
 class Index:
+    """Index."""
+
     def __init__(self, base_url: str, name: str, user: str, client_cmd_base: list[str]) -> None:
+        """
+        Create index.
+
+        :param base_url: base url
+        :param name: name for the index server
+        :param user: the username to use
+        :param client_cmd_base:
+        """
         self._client_cmd_base = client_cmd_base
         self._server_url = base_url
         self.name = name
         self.user = user
 
     @property
     def url(self) -> str:
+        """:return: the URL to the index server"""
         return f"{self._server_url}/{self.name}/+simple/"
 
     def use(self) -> None:
-        _check_call(self._client_cmd_base + ["use", f"{self.user}/{self.name}"])
+        """Use this index server."""
+        _check_call([*self._client_cmd_base, "use", f"{self.user}/{self.name}"])
 
     def upload(self, *files: Path) -> None:
+        """
+        Upload packages to the index.
+
+        :param files: the files to upload
+        """
         cmd = self._client_cmd_base + ["upload", "--index", self.name] + [str(i) for i in files]
         _check_call(cmd)
 
     def __repr__(self) -> str:
+        """:return: repr of the index"""
         return f"{self.__class__.__name__}(url={self.url})"
 
 
 class IndexServer:
-    def __init__(self, path: Path, with_root_pypi: bool = False, start_args: Sequence[str] | None = None) -> None:
+    """A PyPI index server locally."""
+
+    def __init__(
+        self,
+        path: Path,
+        with_root_pypi: bool = False,  # noqa: FBT001, FBT002
+        start_args: Sequence[str] | None = None,
+    ) -> None:
+        """
+        Create the local index server.
+
+        :param path: the path where to host files
+        :param with_root_pypi: access to upstream PyPI
+        :param start_args: additional arguments to start the server
+        """
         self.path = path
         self._with_root_pypi = with_root_pypi
         self._start_args: Sequence[str] = [] if start_args is None else start_args
 
         self.host, self.port = "localhost", _find_free_port()
-        self._passwd = "".join(random.choices(string.ascii_letters, k=8))
+        self._passwd = "".join(random.choices(string.ascii_letters, k=8))  # noqa: S311
 
         scripts_dir = sysconfig.get_path("scripts")
         if scripts_dir is None:
-            raise RuntimeError("could not get scripts folder of host interpreter")  # pragma: no cover
+            msg = "could not get scripts folder of host interpreter"  # pragma: no cover
+            raise RuntimeError(msg)  # pragma: no cover
 
         def _exe(name: str) -> str:
             return str(Path(scripts_dir) / f"{name}{'.exe' if sys.platform == 'win32' else ''}")
 
         self._init: str = _exe("devpi-init")
         self._server: str = _exe("devpi-server")
         self._client: str = _exe("devpi")
@@ -66,17 +102,19 @@
         self._indexes: dict[str, Index] = {}
         self._process: Popen[str] | None = None
         self._has_use = False
         self._stdout_drain: Thread | None = None
 
     @property
     def user(self) -> str:
+        """:return: username of the index server"""
         return "root"
 
     def __enter__(self) -> IndexServer:
+        """:return: start the index server"""
         self._create_and_start_server()
         self._setup_client()
         return self
 
     def _create_and_start_server(self) -> None:
         self._server_dir.mkdir(exist_ok=True)
         server_at = str(self._server_dir)
@@ -85,15 +123,15 @@
         cmd.extend(("--role", "standalone", "--root-passwd", self._passwd))
         if self._with_root_pypi is False:
             cmd.append("--no-root-pypi")
         _check_call(cmd)
         # 2. start the server
         cmd = [self._server, "--serverdir", server_at, "--port", str(self.port)]
         cmd.extend(self._start_args)
-        self._process = Popen(cmd, stdout=PIPE, universal_newlines=True)
+        self._process = Popen(cmd, stdout=PIPE, universal_newlines=True)  # noqa: S603
         stdout = self._drain_stdout()
         for line in stdout:  # pragma: no branch # will always loop at least once
             if "serving at url" in line:
 
                 def _keep_draining() -> None:
                     for _ in stdout:
                         pass
@@ -104,50 +142,67 @@
                 break
 
     def _drain_stdout(self) -> Iterator[str]:
         process = cast("Popen[str]", self._process)
         stdout = cast(IO[str], process.stdout)
         while True:
             if process.poll() is not None:  # pragma: no cover
-                print(f"devpi server with pid {process.pid} at {self._server_dir} died")
+                print(f"devpi server with pid {process.pid} at {self._server_dir} died")  # noqa: T201
                 break
             yield stdout.readline()
 
     def _setup_client(self) -> None:
-        """create a user on the server and authenticate it"""
+        """Create a user on the server and authenticate it."""
         self._client_dir.mkdir(exist_ok=True)
         base = ["--clientdir", str(self._client_dir)]
-        _check_call([self._client, "use"] + base + [self.url])
-        _check_call([self._client, "login"] + base + [self.user, "--password", self._passwd])
+        _check_call([self._client, "use", *base, self.url])
+        _check_call([self._client, "login", *base, self.user, "--password", self._passwd])
 
     def create_index(self, name: str, *args: str) -> Index:
+        """
+        Create an index on the server.
+
+        :param name: with name
+        :param args: additional arguments
+        :return: the created index
+        """
         if name in self._indexes:  # pragma: no cover
-            raise ValueError(f"index {name} already exists")
+            msg = f"index {name} already exists"
+            raise ValueError(msg)
         base = [self._client, "--clientdir", str(self._client_dir)]
-        _check_call(base + ["index", "-c", name, *args])
+        _check_call([*base, "index", "-c", name, *args])
         index = Index(f"{self.url}/{self.user}", name, self.user, base)
         self._indexes[name] = index
         return index
 
     def __exit__(
         self,
-        exc_type: type[BaseException] | None,  # noqa: U100
-        exc_val: BaseException | None,  # noqa: U100
-        exc_tb: TracebackType | None,  # noqa: U100
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
     ) -> None:
+        """
+        Stop the index server.
+
+        :param exc_type:
+        :param exc_val:
+        :param exc_tb:
+        """
         if self._process is not None:  # pragma: no cover # defend against devpi startup fail
             self._process.terminate()
         if self._stdout_drain is not None and self._stdout_drain.is_alive():  # pragma: no cover # devpi startup fail
             self._stdout_drain.join()
 
     @property
     def url(self) -> str:
+        """:return: url to the index server"""
         return f"http://{self.host}:{self.port}"
 
     def __repr__(self) -> str:
+        """:return: repr of the index server"""
         return f"{self.__class__.__name__}(url={self.url}, indexes={list(self._indexes)})"
 
 
 def _find_free_port() -> int:
     with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as socket_handler:
         socket_handler.bind(("", 0))
         return cast(int, socket_handler.getsockname()[1])
```

### Comparing `devpi_process-0.3.0/tests/demo_pkg_inline/build.py` & `devpi_process-0.3.1/tests/demo_pkg_inline/build.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
-import os
 import sys
 import tarfile
 from io import BytesIO
+from pathlib import Path
 from textwrap import dedent
 from zipfile import ZipFile
 
 name = "demo_pkg_inline"
 pkg_name = name.replace("_", "-")
 
 version = "1.0.0"
@@ -27,71 +27,75 @@
         Author: UNKNOWN
         Author-email: UNKNOWN
         License: UNKNOWN
         Platform: UNKNOWN
 
         UNKNOWN
        """.format(
-        pkg_name, version
+        pkg_name,
+        version,
     ),
     wheel: """
         Wheel-Version: 1.0
         Generator: {}-{}
         Root-Is-Purelib: true
         Tag: py{}-none-any
        """.format(
-        name, version, sys.version_info[0]
+        name,
+        version,
+        sys.version_info[0],
     ),
     f"{dist_info}/top_level.txt": name,
     record: """
         {0}/__init__.py,,
         {1}/METADATA,,
         {1}/WHEEL,,
         {1}/top_level.txt,,
         {1}/RECORD,,
        """.format(
-        name, dist_info
+        name,
+        dist_info,
     ),
 }
 
 
 def build_wheel(
     wheel_directory: str,
-    metadata_directory: str | None = None,  # noqa: U100
-    config_settings: None = None,  # noqa: U100
+    metadata_directory: str | None = None,  # noqa: ARG001
+    config_settings: None = None,  # noqa: ARG001
 ) -> str:
     base_name = f"{name}-{version}-py{sys.version_info[0]}-none-any.whl"
-    path = os.path.join(wheel_directory, base_name)
-    with ZipFile(path, "w") as zip_file_handler:
+    path = Path(wheel_directory) / base_name
+    with ZipFile(str(path), "w") as zip_file_handler:
         for arc_name, data in content.items():  # pragma: no branch
             zip_file_handler.writestr(arc_name, dedent(data).strip())
     return base_name
 
 
 def get_requires_for_build_wheel(
-    config_settings: None = None,  # noqa: U100
+    config_settings: None = None,  # noqa: ARG001
 ) -> list[str]:
     return []  # pragma: no cover # only executed in non-host pythons
 
 
 def build_sdist(
     sdist_directory: str,
-    config_settings: None = None,  # noqa: U100
+    config_settings: None = None,  # noqa: ARG001
 ) -> str:
     result = f"{name}-{version}.tar.gz"
-    with tarfile.open(os.path.join(sdist_directory, result), "w:gz") as tar:
-        root = os.path.dirname(os.path.abspath(__file__))
-        tar.add(os.path.join(root, "build.py"), "build.py")
-        tar.add(os.path.join(root, "pyproject.toml"), "pyproject.toml")
+    with tarfile.open(str(Path(sdist_directory) / result), "w:gz") as tar:
+        root = Path(__file__).parent
+        tar.add(str(root / "build.py"), "build.py")
+        tar.add(str(root / "pyproject.toml"), "pyproject.toml")
 
         pkg_info = dedent(content[metadata]).strip().encode("utf-8")
         info = tarfile.TarInfo("PKG-INFO")
         info.size = len(pkg_info)
         tar.addfile(info, BytesIO(pkg_info))
 
     return result
 
 
 def get_requires_for_build_sdist(
-    config_settings: None = None,  # noqa: U100
+    config_settings: None = None,  # noqa: ARG001
 ) -> list[str]:
     return []  # pragma: no cover # only executed in non-host pythons
```

### Comparing `devpi_process-0.3.0/tests/test_devpi_process.py` & `devpi_process-0.3.1/tests/test_devpi_process.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
 from importlib.util import module_from_spec, spec_from_file_location
 from pathlib import Path
+from typing import TYPE_CHECKING
 
 import pytest
-from _pytest.tmpdir import TempPathFactory
 from httpx import get
 
 from devpi_process import IndexServer
 
+if TYPE_CHECKING:
+    from _pytest.tmpdir import TempPathFactory
+
 
 def test_version() -> None:
     import devpi_process
 
     assert devpi_process.__version__ is not None
 
 
@@ -62,9 +65,9 @@
     with IndexServer(tmp_path, with_root_pypi=True) as server:
         state = get(server.url).json()["result"]["root"]
         assert state["indexes"].keys() == {"pypi"}
 
 
 def test_create_server_start_args(tmp_path: Path) -> None:
     with IndexServer(tmp_path, start_args=["--offline-mode"]) as server:
-        assert server._process is not None
-        assert server._process.args[-1] == "--offline-mode"  # type: ignore
+        assert server._process is not None  # noqa: SLF001
+        assert server._process.args[-1] == "--offline-mode"  # type: ignore[index] # noqa: SLF001
```

### Comparing `devpi_process-0.3.0/tox.ini` & `devpi_process-0.3.1/tox.ini`

 * *Files 21% similar despite different names*

```diff
@@ -1,79 +1,72 @@
 [tox]
-envlist =
+requires =
+    tox>=4.2
+env_list =
     fix
+    py311
     py310
     py39
     py38
     py37
     type
     readme
-isolated_build = true
 skip_missing_interpreters = true
-minversion = 3.14
 
 [testenv]
 description = run the unit tests with pytest under {basepython}
-setenv =
-    COVERAGE_FILE = {toxworkdir}/.coverage.{envname}
-    COVERAGE_PROCESS_START = {toxinidir}/setup.cfg
-    _COVERAGE_SRC = {envsitepackagesdir}/sphinx_argparse_cli
+package = wheel
+wheel_build_env = .pkg
 extras =
     test
+set_env =
+    COVERAGE_FILE = {toxworkdir}/.coverage.{envname}
+    COVERAGE_PROCESS_START = {toxinidir}/pyproject.toml
+    _COVERAGE_SRC = {envsitepackagesdir}/devpi_process
 commands =
     pytest {tty:--color=yes} {posargs: \
       --junitxml {toxworkdir}{/}junit.{envname}.xml --cov {envsitepackagesdir}{/}devpi_process \
       --cov {toxinidir}{/}tests --cov-fail-under=100 \
-      --cov-config=setup.cfg --no-cov-on-fail --cov-report term-missing:skip-covered --cov-context=test \
+      --cov-config=pyproject.toml --no-cov-on-fail --cov-report term-missing:skip-covered --cov-context=test \
       --cov-report html:{envtmpdir}{/}htmlcov --cov-report xml:{toxworkdir}{/}coverage.{envname}.xml \
       tests}
-package = wheel
-wheel_build_env = .pkg
 
 [testenv:fix]
 description = run static analysis and style check using flake8
-passenv =
-    HOMEPATH
-    PROGRAMDATA
 skip_install = true
 deps =
-    pre-commit>=2.20
+    pre-commit>=3.2.2
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
-    mypy==0.991
+    mypy==1.3
+set_env =
+    {tty:MYPY_FORCE_COLOR = 1}
 commands =
-    mypy --strict --python-version 3.10 src
-    mypy --strict --python-version 3.10 tests
+    mypy src
+    mypy tests
 
 [testenv:readme]
 description = check that the long description is valid
 skip_install = true
 deps =
-    build[virtualenv]>=0.9
+    build[virtualenv]>=0.10
     twine>=4.0.2
 commands =
     python -m build --sdist --wheel -o {envtmpdir} .
     twine check {envtmpdir}/*
 
 [testenv:dev]
 description = generate a DEV environment
-usedevelop = true
+package = editable
 extras =
     docs
     test
 commands =
     python -m pip list --format=columns
     python -c 'import sys; print(sys.executable)'
-
-[testenv:py311]
-setenv =
-    {[testenv]setenv}
-    AIOHTTP_NO_EXTENSIONS = 1
-
-[pytest]
-junit_family = xunit2
```

