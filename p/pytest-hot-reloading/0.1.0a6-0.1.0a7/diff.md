# Comparing `tmp/pytest_hot_reloading-0.1.0a6.tar.gz` & `tmp/pytest_hot_reloading-0.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_hot_reloading-0.1.0a6.tar", max compression
+gzip compressed data, was "pytest_hot_reloading-0.1.0a7.tar", max compression
```

## Comparing `pytest_hot_reloading-0.1.0a6.tar` & `pytest_hot_reloading-0.1.0a7.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1072 2023-06-15 23:41:37.815060 pytest_hot_reloading-0.1.0a6/LICENSE
--rw-r--r--   0        0        0     3975 2023-06-15 23:41:37.815060 pytest_hot_reloading-0.1.0a6/README.md
--rw-r--r--   0        0        0     1037 2023-06-15 23:41:37.815060 pytest_hot_reloading-0.1.0a6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-15 23:41:37.815060 pytest_hot_reloading-0.1.0a6/pytest_hot_reloading/__init__.py
--rw-r--r--   0        0        0     2049 2023-06-15 23:41:37.815060 pytest_hot_reloading-0.1.0a6/pytest_hot_reloading/client.py
--rw-r--r--   0        0        0    10046 2023-06-15 23:41:37.815060 pytest_hot_reloading-0.1.0a6/pytest_hot_reloading/daemon.py
--rw-r--r--   0        0        0     9072 2023-06-15 23:41:37.815060 pytest_hot_reloading-0.1.0a6/pytest_hot_reloading/plugin.py
--rw-r--r--   0        0        0     2305 2023-06-15 23:41:37.815060 pytest_hot_reloading-0.1.0a6/pytest_hot_reloading/workarounds.py
--rw-r--r--   0        0        0     4473 1970-01-01 00:00:00.000000 pytest_hot_reloading-0.1.0a6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-16 20:01:51.315319 pytest_hot_reloading-0.1.0a7/LICENSE
+-rw-r--r--   0        0        0     4916 2023-06-16 20:01:51.315319 pytest_hot_reloading-0.1.0a7/README.md
+-rw-r--r--   0        0        0     1037 2023-06-16 20:01:51.331320 pytest_hot_reloading-0.1.0a7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-16 20:01:51.331320 pytest_hot_reloading-0.1.0a7/pytest_hot_reloading/__init__.py
+-rw-r--r--   0        0        0     2435 2023-06-16 20:01:51.331320 pytest_hot_reloading-0.1.0a7/pytest_hot_reloading/client.py
+-rw-r--r--   0        0        0    10617 2023-06-16 20:01:51.331320 pytest_hot_reloading-0.1.0a7/pytest_hot_reloading/daemon.py
+-rw-r--r--   0        0        0     9551 2023-06-16 20:01:51.331320 pytest_hot_reloading-0.1.0a7/pytest_hot_reloading/plugin.py
+-rw-r--r--   0        0        0        1 2023-06-16 20:01:51.331320 pytest_hot_reloading-0.1.0a7/pytest_hot_reloading/py.typed
+-rw-r--r--   0        0        0     2305 2023-06-16 20:01:51.331320 pytest_hot_reloading-0.1.0a7/pytest_hot_reloading/workarounds.py
+-rw-r--r--   0        0        0     5414 1970-01-01 00:00:00.000000 pytest_hot_reloading-0.1.0a7/PKG-INFO
```

### Comparing `pytest_hot_reloading-0.1.0a6/LICENSE` & `pytest_hot_reloading-0.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_hot_reloading-0.1.0a6/README.md` & `pytest_hot_reloading-0.1.0a7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 # A PyTest Hot Reloading Plugin
 A hot reloading pytest daemon, implemented as a plugin.
 
 This uses the [jurigged](https://github.com/breuleux/jurigged) library to watch files.
 
 If it takes less than 5 seconds to do all of the imports
-necessary to run a unit test, then you probably don't need this.
+necessary to run a unit test, then you probably don't need this. If you use Django,
+you'll probably love this.
+
+The minimum Python version is 3.10
+
+## Demo
+
+### With hot reloading
+![Hot reloading demo](docs/hot-reloading-demo.gif)
+
+### Without hot reloading
+![Not hot reloading demo](docs/not-hot-reloading-demo.gif)
 
 ## Installation
 Do not install in production code. This is exclusively for the developer environment.
 
 pip: Add `pytest-hot-reloading` to your `dev-requirements.txt` file and `pip install -r dev-requirements.txt`
+
 poetry: `poetry add --group=dev pytest-hot-reloading`
 
+
 ## Usage
 Add the plugin to the pytest arguments. Example using pyproject.toml:
 ```toml
 [tool.pytest.ini_options]
 addopts = "-p pytest_hot_reloading.plugin"
 ```
 
@@ -53,14 +66,34 @@
 The only reason you would need to limit the watched files is because the jurigged library
 opens every file it watches, so it can exhaust the open file limit if you have a lot of files.
 
 If the daemon is already running and you run pytest with `--daemon`, then the old one will be stopped
 and a new one will be started. Note that `pytest --daemon` is NOT how you run tests. It is only used to start
 the daemon.
 
+The daemon can be stopped with `pytest --stop-daemon`. This can be used if it gets into a bad state.
+
+## Arguments and Env Variables
+- `PYTEST_DAEMON_PORT`
+    - The port the daemon listens on.
+    - Default: `4852`.
+    - Command line: `--daemon-port`
+- `PYTEST_DAEMON_PYTEST_NAME`
+    - The name of the pytest executable.
+    - Default: `pytest`.
+    - Command line: `--pytest-name`
+- `PYTEST_DAEMON_WATCH_GLOBS`
+    - The colon separated globs to watch.
+    - Default: `./**/*.py`.
+    - Command line: `--daemon-watch-globs`
+- `PYTEST_DAEMON_IGNORE_WATCH_GLOBS`
+    - The colon separated globs to ignore.
+    - Default: `./.venv/*`.
+    - Command line: `--daemon-ignore-watch-globs`
+
 ## Workarounds
 Libraries that use mutated globals may need a workaround to work with this plugin. The preferred
 route is to have the library update its code to not mutate globals in a test environment, or to
 restore them after a test suite has ran. In some cases, that isn't possible, usually because
 the person with the problem doesn't own the library and can't wait around for a fix.
 
 To register a workaround, create a function that is decorated by the
```

### Comparing `pytest_hot_reloading-0.1.0a6/pyproject.toml` & `pytest_hot_reloading-0.1.0a7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 line-length = 120
 
 [tool.black]
 line-length = 98
 
 [tool.poetry]
 name = "pytest-hot-reloading"
-version = "0.1.0-alpha.6"
+version = "0.1.0-alpha.7"
 description = ""
 authors = ["James Hutchison <jamesghutchison@proton.me>"]
 readme = "README.md"
 packages = [{ include = "pytest_hot_reloading" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -19,15 +19,15 @@
 types-cachetools = "^5.3.0.5"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.2.0"
 ruff = "^0.0.261"
 black = "^23.3.0"
 pytest = "^7.2.2"
-megamock = "^0.1.0b3"
+megamock = "^0.1.0b6"
 pytest-django = "^4.5.2"
 django = "^4.2.2"
 psycopg2-binary = "^2.9.6"
 pytest-env = "^0.8.1"
 pytest-xdist = "^3.3.1"
 
 [build-system]
```

### Comparing `pytest_hot_reloading-0.1.0a6/pytest_hot_reloading/client.py` & `pytest_hot_reloading-0.1.0a7/pytest_hot_reloading/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,32 +15,50 @@
         self, daemon_host: str = "localhost", daemon_port: int = 4852, pytest_name: str = "pytest"
     ) -> None:
         self._socket = None
         self._daemon_host = daemon_host
         self._daemon_port = daemon_port
         self._pytest_name = pytest_name
 
+    def _get_server(self) -> xmlrpc.client.ServerProxy:
+        server_url = f"http://{self._daemon_host}:{self._daemon_port}"
+        server = xmlrpc.client.ServerProxy(server_url)
+
+        return server
+
     def run(self, args: list[str]) -> int:
         self._start_daemon_if_needed()
 
-        server_url = f"http://{self._daemon_host}:{self._daemon_port}"
-        server = xmlrpc.client.ServerProxy(server_url)
+        server = self._get_server()
 
         start = time.time()
         result: dict = cast(dict, server.run_pytest(args))
         print(f"Daemon took {(time.time() - start):.3f} seconds to reply")
 
         stdout = result["stdout"].data.decode("utf-8")
         stderr = result["stderr"].data.decode("utf-8")
 
         print(stdout, file=sys.stdout)
         print(stderr, file=sys.stderr)
 
         return result["status_code"]
 
+    def stop(self) -> None:
+        """
+        Stop the daemon
+        """
+        server = self._get_server()
+
+        try:
+            server.stop()
+        except OSError:
+            print("Daemon is not running")
+        else:
+            print("Daemon stopped")
+
     def abort(self) -> None:
         # Close the socket
         if self._socket:
             self._socket.close()
 
     def _start_daemon_if_needed(self) -> None:
         # check if the daemon is running on the expected host and port
```

### Comparing `pytest_hot_reloading-0.1.0a6/pytest_hot_reloading/daemon.py` & `pytest_hot_reloading-0.1.0a7/pytest_hot_reloading/daemon.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import copy
 import os
 import re
 import socket
 import subprocess
 import sys
+import tempfile
 import time
+from pathlib import Path
+from threading import Thread
 from typing import Counter, Generator
 from xmlrpc.server import SimpleXMLRPCServer
 
 import pytest
 from cachetools import TTLCache
 
 from pytest_hot_reloading.workarounds import (
@@ -17,18 +20,19 @@
 )
 
 
 class PytestDaemon:
     def __init__(self, daemon_host: str = "localhost", daemon_port: int = 4852) -> None:
         self._daemon_host = daemon_host
         self._daemon_port = daemon_port
+        self._server: SimpleXMLRPCServer | None = None
 
     @property
-    def pid_file(self) -> str:
-        return f".pytest_hot_reloading_{self._daemon_port}.pid"
+    def pid_file(self) -> Path:
+        return Path(tempfile.gettempdir()) / f".pytest_hot_reloading_{self._daemon_port}.pid"
 
     @staticmethod
     def start(
         host: str,
         port: int,
         pytest_name: str = "pytest",
         watch_globs: str | None = None,
@@ -53,14 +57,22 @@
                 env=os.environ,
                 cwd=os.getcwd(),
             )
         else:
             raise NotImplementedError("Only localhost is supported for now")
         PytestDaemon.wait_to_be_ready(host, port)
 
+    def stop(self) -> dict:
+        if self._server:
+            t = Thread(target=self._server.shutdown, daemon=True)
+            t.start()
+            self._delete_pid_file()
+
+        return {"shutdown": "ok"}
+
     @staticmethod
     def wait_to_be_ready(host: str = "localhost", port: int = 4852) -> None:
         # poll the connection to the daemon using sockets
         # and return when it is ready
         for _ in range(100):
             try:
                 sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
@@ -82,21 +94,27 @@
                 time.sleep(2)
                 server = SimpleXMLRPCServer((self._daemon_host, self._daemon_port))
 
         self._write_pid_file()
 
         # register the 'run_pytest' function
         server.register_function(self.run_pytest, "run_pytest")  # type: ignore
+        server.register_function(self.stop, "stop")
 
+        self._server = server
         server.serve_forever()
 
     def _write_pid_file(self) -> None:
         with open(self.pid_file, "w") as f:
             f.write(str(os.getpid()))
 
+    def _delete_pid_file(self) -> None:
+        if os.path.exists(self.pid_file):
+            os.unlink(self.pid_file)
+
     def _kill_existing_daemon(self) -> None:
         try:
             with open(self.pid_file, "r") as f:
                 pid = int(f.read())
             os.kill(pid, 9)
         except FileNotFoundError:
             raise Exception(f"Port {self._daemon_port} is already in use")
```

### Comparing `pytest_hot_reloading-0.1.0a6/pytest_hot_reloading/plugin.py` & `pytest_hot_reloading-0.1.0a7/pytest_hot_reloading/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,46 +21,52 @@
 
 def pytest_addoption(parser) -> None:
     group = parser.getgroup("daemon")
     group.addoption(
         "--daemon",
         action="store_true",
         default=False,
-        help="Start the daemon",
+        help="Start the daemon. If it is already running, the old instance will stop.",
     )
     group.addoption(
         "--daemon-port",
         action="store",
-        default=4852,
+        default=int(os.getenv("PYTEST_DAEMON_PORT", "4852")),
         help="The port to use for the daemon. You generally shouldn't need to set this.",
     )
     group.addoption(
         "--pytest-name",
         action="store",
-        default="pytest",
+        default=os.getenv("PYTEST_DAEMON_PYTEST_NAME", "pytest"),
         help="The name of the pytest executable or module",
     )
     group.addoption(
         "--daemon-timeout",
         action="store",
-        default=(5 * 60),
-        help="The timeout in seconds to wait on a test suite to finish",
+        default=os.getenv("PYTEST_DAEMON_TIMEOUT", (5 * 60)),
+        help="The timeout in seconds to wait on a test suite to finish. This is not yet implemented.",
     )
     group.addoption(
         "--daemon-watch-globs",
         action="store",
-        default="./*.py",
+        default=os.getenv("PYTEST_DAEMON_WATCH_GLOBS", "./*.py"),
         help="The globs to watch for changes. This is a colon separated list of globs.",
     )
     group.addoption(
         "--daemon-ignore-watch-globs",
         action="store",
-        default="./.venv/*",
+        default=os.getenv("PYTEST_DAEMON_IGNORE_WATCH_GLOBS", "./.venv/*"),
         help="The globs to ignore for changes. This is a colon separated list of globs.",
     )
+    group.addoption(
+        "--stop-daemon",
+        action="store_true",
+        default=False,
+        help="Stop the daemon",
+    )
 
 
 # list of pytest hooks
 # https://docs.pytest.org/en/stable/reference.html#_pytest.hookspec.pytest_addhooks
 
 
 def pytest_cmdline_main(config: Config) -> Optional[int]:
@@ -168,18 +174,23 @@
         setup_jurigged(config)
 
         from pytest_hot_reloading.daemon import PytestDaemon
 
         daemon = PytestDaemon(daemon_port=daemon_port)
 
         daemon.run_forever()
-        raise Exception("Daemon should never exit")
+        sys.exit(0)
     else:
         pytest_name = config.option.pytest_name
         client = PytestClient(daemon_port=daemon_port, pytest_name=pytest_name)
+
+        if config.option.stop_daemon:
+            client.stop()
+            return 0
+
         # find the index of the first value that is not None
         for idx, val in enumerate(
             [
                 x.endswith(pytest_name) or x.endswith(f"{pytest_name}/__main__.py")
                 for x in sys.argv
             ]
         ):
```

### Comparing `pytest_hot_reloading-0.1.0a6/pytest_hot_reloading/workarounds.py` & `pytest_hot_reloading-0.1.0a7/pytest_hot_reloading/workarounds.py`

 * *Files identical despite different names*

### Comparing `pytest_hot_reloading-0.1.0a6/PKG-INFO` & `pytest_hot_reloading-0.1.0a7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-hot-reloading
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: 
 Author: James Hutchison
 Author-email: jamesghutchison@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -15,22 +15,35 @@
 
 # A PyTest Hot Reloading Plugin
 A hot reloading pytest daemon, implemented as a plugin.
 
 This uses the [jurigged](https://github.com/breuleux/jurigged) library to watch files.
 
 If it takes less than 5 seconds to do all of the imports
-necessary to run a unit test, then you probably don't need this.
+necessary to run a unit test, then you probably don't need this. If you use Django,
+you'll probably love this.
+
+The minimum Python version is 3.10
+
+## Demo
+
+### With hot reloading
+![Hot reloading demo](docs/hot-reloading-demo.gif)
+
+### Without hot reloading
+![Not hot reloading demo](docs/not-hot-reloading-demo.gif)
 
 ## Installation
 Do not install in production code. This is exclusively for the developer environment.
 
 pip: Add `pytest-hot-reloading` to your `dev-requirements.txt` file and `pip install -r dev-requirements.txt`
+
 poetry: `poetry add --group=dev pytest-hot-reloading`
 
+
 ## Usage
 Add the plugin to the pytest arguments. Example using pyproject.toml:
 ```toml
 [tool.pytest.ini_options]
 addopts = "-p pytest_hot_reloading.plugin"
 ```
 
@@ -68,14 +81,34 @@
 The only reason you would need to limit the watched files is because the jurigged library
 opens every file it watches, so it can exhaust the open file limit if you have a lot of files.
 
 If the daemon is already running and you run pytest with `--daemon`, then the old one will be stopped
 and a new one will be started. Note that `pytest --daemon` is NOT how you run tests. It is only used to start
 the daemon.
 
+The daemon can be stopped with `pytest --stop-daemon`. This can be used if it gets into a bad state.
+
+## Arguments and Env Variables
+- `PYTEST_DAEMON_PORT`
+    - The port the daemon listens on.
+    - Default: `4852`.
+    - Command line: `--daemon-port`
+- `PYTEST_DAEMON_PYTEST_NAME`
+    - The name of the pytest executable.
+    - Default: `pytest`.
+    - Command line: `--pytest-name`
+- `PYTEST_DAEMON_WATCH_GLOBS`
+    - The colon separated globs to watch.
+    - Default: `./**/*.py`.
+    - Command line: `--daemon-watch-globs`
+- `PYTEST_DAEMON_IGNORE_WATCH_GLOBS`
+    - The colon separated globs to ignore.
+    - Default: `./.venv/*`.
+    - Command line: `--daemon-ignore-watch-globs`
+
 ## Workarounds
 Libraries that use mutated globals may need a workaround to work with this plugin. The preferred
 route is to have the library update its code to not mutate globals in a test environment, or to
 restore them after a test suite has ran. In some cases, that isn't possible, usually because
 the person with the problem doesn't own the library and can't wait around for a fix.
 
 To register a workaround, create a function that is decorated by the
```

