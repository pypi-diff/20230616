# Comparing `tmp/pytest_hot_reloading-0.1.0a5.tar.gz` & `tmp/pytest_hot_reloading-0.1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_hot_reloading-0.1.0a5.tar", max compression
+gzip compressed data, was "pytest_hot_reloading-0.1.0a6.tar", max compression
```

## Comparing `pytest_hot_reloading-0.1.0a5.tar` & `pytest_hot_reloading-0.1.0a6.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1072 2023-05-18 23:38:57.592078 pytest_hot_reloading-0.1.0a5/LICENSE
--rw-r--r--   0        0        0     2442 2023-05-18 23:38:57.592078 pytest_hot_reloading-0.1.0a5/README.md
--rw-r--r--   0        0        0      676 2023-05-18 23:38:57.592078 pytest_hot_reloading-0.1.0a5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-18 23:38:57.592078 pytest_hot_reloading-0.1.0a5/pytest_hot_reloading/__init__.py
--rw-r--r--   0        0        0     1969 2023-05-18 23:38:57.592078 pytest_hot_reloading-0.1.0a5/pytest_hot_reloading/client.py
--rw-r--r--   0        0        0     9556 2023-05-18 23:38:57.592078 pytest_hot_reloading-0.1.0a5/pytest_hot_reloading/daemon.py
--rw-r--r--   0        0        0     8221 2023-05-18 23:38:57.592078 pytest_hot_reloading-0.1.0a5/pytest_hot_reloading/plugin.py
--rw-r--r--   0        0        0     2887 1970-01-01 00:00:00.000000 pytest_hot_reloading-0.1.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-15 23:41:37.815060 pytest_hot_reloading-0.1.0a6/LICENSE
+-rw-r--r--   0        0        0     3975 2023-06-15 23:41:37.815060 pytest_hot_reloading-0.1.0a6/README.md
+-rw-r--r--   0        0        0     1037 2023-06-15 23:41:37.815060 pytest_hot_reloading-0.1.0a6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-15 23:41:37.815060 pytest_hot_reloading-0.1.0a6/pytest_hot_reloading/__init__.py
+-rw-r--r--   0        0        0     2049 2023-06-15 23:41:37.815060 pytest_hot_reloading-0.1.0a6/pytest_hot_reloading/client.py
+-rw-r--r--   0        0        0    10046 2023-06-15 23:41:37.815060 pytest_hot_reloading-0.1.0a6/pytest_hot_reloading/daemon.py
+-rw-r--r--   0        0        0     9072 2023-06-15 23:41:37.815060 pytest_hot_reloading-0.1.0a6/pytest_hot_reloading/plugin.py
+-rw-r--r--   0        0        0     2305 2023-06-15 23:41:37.815060 pytest_hot_reloading-0.1.0a6/pytest_hot_reloading/workarounds.py
+-rw-r--r--   0        0        0     4473 1970-01-01 00:00:00.000000 pytest_hot_reloading-0.1.0a6/PKG-INFO
```

### Comparing `pytest_hot_reloading-0.1.0a5/LICENSE` & `pytest_hot_reloading-0.1.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_hot_reloading-0.1.0a5/pytest_hot_reloading/client.py` & `pytest_hot_reloading-0.1.0a6/pytest_hot_reloading/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import socket
 import sys
 import time
 import xmlrpc.client
+from typing import cast
 
 
 class PytestClient:
     _socket: socket.socket | None
     _daemon_host: str
     _daemon_port: int
     _pytest_name: str
@@ -14,30 +15,32 @@
         self, daemon_host: str = "localhost", daemon_port: int = 4852, pytest_name: str = "pytest"
     ) -> None:
         self._socket = None
         self._daemon_host = daemon_host
         self._daemon_port = daemon_port
         self._pytest_name = pytest_name
 
-    def run(self, args: list[str]) -> str:
+    def run(self, args: list[str]) -> int:
         self._start_daemon_if_needed()
 
         server_url = f"http://{self._daemon_host}:{self._daemon_port}"
         server = xmlrpc.client.ServerProxy(server_url)
 
         start = time.time()
-        result = server.run_pytest(args)
+        result: dict = cast(dict, server.run_pytest(args))
         print(f"Daemon took {(time.time() - start):.3f} seconds to reply")
 
         stdout = result["stdout"].data.decode("utf-8")
         stderr = result["stderr"].data.decode("utf-8")
 
         print(stdout, file=sys.stdout)
         print(stderr, file=sys.stderr)
 
+        return result["status_code"]
+
     def abort(self) -> None:
         # Close the socket
         if self._socket:
             self._socket.close()
 
     def _start_daemon_if_needed(self) -> None:
         # check if the daemon is running on the expected host and port
```

### Comparing `pytest_hot_reloading-0.1.0a5/pytest_hot_reloading/daemon.py` & `pytest_hot_reloading-0.1.0a6/pytest_hot_reloading/daemon.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import copy
 import os
 import re
 import socket
 import subprocess
 import sys
 import time
-from typing import Counter
+from typing import Counter, Generator
 from xmlrpc.server import SimpleXMLRPCServer
 
 import pytest
 from cachetools import TTLCache
 
+from pytest_hot_reloading.workarounds import (
+    run_workarounds_post,
+    run_workarounds_pre,
+)
+
 
 class PytestDaemon:
     def __init__(self, daemon_host: str = "localhost", daemon_port: int = 4852) -> None:
         self._daemon_host = daemon_host
         self._daemon_port = daemon_port
 
     @property
@@ -76,15 +81,15 @@
                 self._kill_existing_daemon()
                 time.sleep(2)
                 server = SimpleXMLRPCServer((self._daemon_host, self._daemon_port))
 
         self._write_pid_file()
 
         # register the 'run_pytest' function
-        server.register_function(self.run_pytest, "run_pytest")
+        server.register_function(self.run_pytest, "run_pytest")  # type: ignore
 
         server.serve_forever()
 
     def _write_pid_file(self) -> None:
         with open(self.pid_file, "w") as f:
             f.write(str(os.getpid()))
 
@@ -96,15 +101,15 @@
         except FileNotFoundError:
             raise Exception(f"Port {self._daemon_port} is already in use")
 
     def run_pytest(self, args: list[str]) -> dict:
         # run pytest using command line args
         # run the pytest main logic
 
-        self._workaround_library_issues(args)
+        in_progress_workarounds = self._workaround_library_issues_pre()
 
         import pytest_hot_reloading.plugin as plugin
 
         # indicate to the plugin to NOT run custom pytest collect logic
         plugin.i_am_server = True
 
         # capture stdout and stderr
@@ -125,16 +130,18 @@
 
         # monkeypatch in the main that does test collection caching
         orig_main = _pytest.main._main
         _pytest.main._main = _pytest_main
 
         try:
             # args must omit the calling program
-            pytest.main(["--color=yes"] + args)
+            status_code = pytest.main(["--color=yes"] + args)
         finally:
+            self._workaround_library_issues_post(in_progress_workarounds)
+
             # restore originals
             _pytest.main._main = orig_main
 
             sys.stdout = stdout_bak
             sys.stderr = stderr_bak
 
             stdout.seek(0)
@@ -143,28 +150,31 @@
             stderr_str = stderr.read()
 
             print(stdout_str, file=sys.stdout)
             print(stderr_str, file=sys.stderr)
         return {
             "stdout": self._remove_ansi_escape(stdout_str).encode("utf-8"),
             "stderr": self._remove_ansi_escape(stderr_str).encode("utf-8"),
+            "status_code": int(status_code),
         }
 
     def _remove_ansi_escape(self, s: str) -> str:
         return re.sub(r"\x1b(\[.*?[@-~]|\].*?(\x07|\x1b\\))", "", s, flags=re.MULTILINE)
 
-    def _workaround_library_issues(self, args: list[str]) -> None:
-        # load modules that workaround library issues, as needed
-        pass
+    def _workaround_library_issues_pre(self) -> list[Generator]:
+        return run_workarounds_pre()
+
+    def _workaround_library_issues_post(self, in_progress_workarounds: list[Generator]) -> None:
+        run_workarounds_post(in_progress_workarounds)
 
 
-session_item_cache = TTLCache(16, 500)
+session_item_cache: TTLCache[tuple, tuple] = TTLCache(16, 500)
 # hack: keeping a session cache since pytest has session references
 #       littered everywhere on objects
-prior_sessions = set()
+prior_sessions: set[pytest.Session] = set()
 
 
 def _manage_prior_session_garbage(session: pytest.Session) -> None:
     """
     Pytest creates a bunch of objects and nodes and assigns the session
     to them. This creates a lot of dangling references to sessions that
     can come up later due to reuse. To work around this, all prior
@@ -205,24 +215,24 @@
     """
     A monkey patched version of _pytest._main that caches test collection
     """
     _manage_prior_session_garbage(session)
 
     import _pytest.capture
 
-    _pytest.capture.CaptureManager.stop_global_capturing = lambda self: None
+    _pytest.capture.CaptureManager.stop_global_capturing = lambda self: None  # type: ignore
     start_global_capturing = _pytest.capture.CaptureManager.start_global_capturing
     resume_global_capture = _pytest.capture.CaptureManager.resume_global_capture
 
     def start_global_capture_if_needed(self: _pytest.capture.CaptureManager):
         if self._global_capturing is None:
             start_global_capturing(self)
         return resume_global_capture(self)
 
-    _pytest.capture.CaptureManager.resume_global_capture = start_global_capture_if_needed
+    _pytest.capture.CaptureManager.resume_global_capture = start_global_capture_if_needed  # type: ignore
 
     def best_effort_copy(item, depth_remaining=2):
         """
         Copy test items. The items have references to modules and
         other things that cannot be deep copied.
         """
         if depth_remaining <= 0:
@@ -253,15 +263,15 @@
         start = time.time()
         config.hook.pytest_collection(session=session)
         print(f"Pytest Daemon: Collection took {(time.time() - start):0.3f} seconds")
         session_item_cache[session_key] = tuple(best_effort_copy(x) for x in session.items)
     else:
         print("Pytest Daemon: Using cached collection")
         # Assign the prior test items (tests to run) and config to the current session
-        session.items = items
+        session.items = items  # type: ignore
         session.config = config
         for i in items:
             # Items have references to the config and the session
             i.config = config
             i.session = session
             if i._request:
                 i._request._pyfuncitem = i
```

### Comparing `pytest_hot_reloading-0.1.0a5/pytest_hot_reloading/plugin.py` & `pytest_hot_reloading-0.1.0a6/pytest_hot_reloading/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 Pytest Hot Reloading plugin
 """
 from __future__ import annotations
 
 import os
 import sys
-from typing import TYPE_CHECKING, Callable
+from pathlib import Path
+from typing import TYPE_CHECKING, Callable, Optional
 
 from pytest_hot_reloading.client import PytestClient
 
 # this is modified by the daemon so that the pytest_collection hooks does not run
 i_am_server = False
 
-seen_paths = set()
+seen_paths: set[Path] = set()
 
 if TYPE_CHECKING:
     from pytest import Config, Item, Session
 
 
 def pytest_addoption(parser) -> None:
     group = parser.getgroup("daemon")
@@ -58,49 +59,51 @@
     )
 
 
 # list of pytest hooks
 # https://docs.pytest.org/en/stable/reference.html#_pytest.hookspec.pytest_addhooks
 
 
-def pytest_cmdline_main(config: Config) -> None:
+def pytest_cmdline_main(config: Config) -> Optional[int]:
     """
     This hook is called by pytest and is one of the first hooks.
     """
     # early escapes
     if config.option.collectonly:
-        return
+        return None
     if i_am_server:
-        return
-    _plugin_logic(config)
+        return None
+    status_code = _plugin_logic(config)
     # dont do any more work. Don't let pytest continue
-    return 0  # status code 0
+    return status_code  # status code 0
 
 
 def monkey_patch_jurigged_function_definition():
-    import jurigged.codetools as jurigged_codetools
+    import jurigged.codetools as jurigged_codetools  # type: ignore
+    import jurigged.utils as jurigged_utils  # type: ignore
 
     OrigFunctionDefinition = jurigged_codetools.FunctionDefinition
 
     import ast
 
     class NewFunctionDefinition(OrigFunctionDefinition):
         def reevaluate(self, new_node, glb):
             new_node = self.apply_assertion_rewrite(new_node, glb)
-            return super().reevaluate(new_node, glb)
+            obj = super().reevaluate(new_node, glb)
+            return obj
 
         def apply_assertion_rewrite(self, ast_func, glb):
             from _pytest.assertion.rewrite import AssertionRewriter
 
-            nodes: list[ast.AST] = [ast_func]
+            nodes: list[ast.AST] = [ast_func]  # type: ignore
             while nodes:
                 node = nodes.pop()
                 for name, field in ast.iter_fields(node):
                     if isinstance(field, list):
-                        new: list[ast.AST] = []
+                        new: list[ast.AST] = []  # type: ignore
                         for i, child in enumerate(field):
                             if isinstance(child, ast.Assert):
                                 # Transform assert.
                                 new.extend(
                                     AssertionRewriter(glb["__file__"], None, None).visit(child)
                                 )
                             else:
@@ -113,14 +116,24 @@
                         # Don't recurse into expressions as they can't contain
                         # asserts.
                         and not isinstance(field, ast.expr)
                     ):
                         nodes.append(field)
             return ast_func
 
+        def stash(self, lineno=1, col_offset=0):
+            if not isinstance(self.parent, OrigFunctionDefinition):
+                co = self.get_object()
+                if co and (delta := lineno - co.co_firstlineno):
+                    delta -= 1  # fix off-by-one
+                    if delta > 0:
+                        self.recode(jurigged_utils.shift_lineno(co, delta), use_cache=False)
+
+            return super(OrigFunctionDefinition, self).stash(lineno, col_offset)
+
     # monkey patch in new definition
     jurigged_codetools.FunctionDefinition = NewFunctionDefinition
 
 
 def setup_jurigged(config: Config):
     def _jurigged_logger(x: str) -> None:
         """
@@ -129,20 +142,22 @@
         By default this creates duplicated output.
 
         Pass in a no-op logger to prevent this.
         """
 
     import jurigged
 
+    monkey_patch_jurigged_function_definition()
+
     pattern = _get_pattern_filters(config)
     # TODO: intelligently use poll versus watchman (https://github.com/JamesHutchison/pytest-hot-reloading/issues/16)
     jurigged.watch(pattern=pattern, logger=_jurigged_logger, poll=True)
 
 
-def _plugin_logic(config: Config) -> None:
+def _plugin_logic(config: Config) -> int:
     """
     The core plugin logic. This is where it splits based on whether we are the server or client.
 
     In either case, the pytest logic will not continue after this.
     """
     # if daemon is passed, then we are the daemon / server
     # if daemon is not passed, then we are the client
@@ -153,14 +168,15 @@
         setup_jurigged(config)
 
         from pytest_hot_reloading.daemon import PytestDaemon
 
         daemon = PytestDaemon(daemon_port=daemon_port)
 
         daemon.run_forever()
+        raise Exception("Daemon should never exit")
     else:
         pytest_name = config.option.pytest_name
         client = PytestClient(daemon_port=daemon_port, pytest_name=pytest_name)
         # find the index of the first value that is not None
         for idx, val in enumerate(
             [
                 x.endswith(pytest_name) or x.endswith(f"{pytest_name}/__main__.py")
@@ -172,15 +188,16 @@
                 break
         else:
             print(sys.argv)
             raise Exception(
                 "Could not find pytest name in args. "
                 "Check the configured name versus the actual name."
             )
-        client.run(sys.argv[pytest_name_index + 1 :])
+        status_code = client.run(sys.argv[pytest_name_index + 1 :])
+        return status_code
 
 
 def _get_pattern_filters(config: Config) -> str | Callable[[str], bool]:
     """
     Jurigged takes in a pattern argument. The argument is either a glob string
     or a function that returns True if the path passed into it should be watched.
 
@@ -214,18 +231,18 @@
         ignore_globs = config.option.daemon_ignore_watch_globs.split(":")
         ignore_regex_matches = [
             re.compile(fnmatch.translate(normalize(glob))).match for glob in ignore_globs
         ]
     else:
         ignore_regex_matches = []
 
-    def matcher(filename) -> bool:
+    def matcher(filename: str) -> bool:
         if filename in seen_paths:
             return False
-        seen_paths.add(filename)
+        seen_paths.add(Path(filename))
         if any(regex_match(filename) for regex_match in regex_matches):
             if not any(
                 ignore_regex_match(filename) for ignore_regex_match in ignore_regex_matches
             ):
                 return True
         return False
```

