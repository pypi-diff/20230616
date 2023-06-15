# Comparing `tmp/dagger_io-0.6.1.tar.gz` & `tmp/dagger_io-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagger_io-0.6.1.tar", max compression
+gzip compressed data, was "dagger_io-0.6.2.tar", max compression
```

## Comparing `dagger_io-0.6.1.tar` & `dagger_io-0.6.2.tar`

### file list

```diff
@@ -1,33 +1,32 @@
--rw-r--r--   0        0        0    10758 2023-06-02 13:32:48.480901 dagger_io-0.6.1/LICENSE
--rw-r--r--   0        0        0     4727 2023-06-02 13:32:48.480901 dagger_io-0.6.1/README.md
--rw-r--r--   0        0        0     6403 2023-06-02 13:33:57.833945 dagger_io-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      360 2023-06-02 13:32:48.480901 dagger_io-0.6.1/src/dagger/__init__.py
--rw-r--r--   0        0        0       71 2023-06-02 13:32:48.480901 dagger_io-0.6.1/src/dagger/__main__.py
--rw-r--r--   0        0        0       69 2023-06-02 13:32:48.480901 dagger_io-0.6.1/src/dagger/api/.gitattributes
--rw-r--r--   0        0        0        0 2023-06-02 13:32:48.480901 dagger_io-0.6.1/src/dagger/api/__init__.py
--rw-r--r--   0        0        0    11873 2023-06-02 13:32:48.480901 dagger_io-0.6.1/src/dagger/api/base.py
--rw-r--r--   0        0        0    90131 2023-06-02 13:32:48.480901 dagger_io-0.6.1/src/dagger/api/gen.py
--rw-r--r--   0        0        0    89730 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/api/gen_sync.py
--rw-r--r--   0        0        0     1683 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/cli.py
--rw-r--r--   0        0        0    20500 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/codegen.py
--rw-r--r--   0        0        0     1302 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/config.py
--rw-r--r--   0        0        0     1884 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/connection.py
--rw-r--r--   0        0        0      964 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/context.py
--rw-r--r--   0        0        0       37 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/engine/.gitattributes
--rw-r--r--   0        0        0       35 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/engine/__init__.py
--rw-r--r--   0        0        0       64 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/engine/_version.py
--rw-r--r--   0        0        0     4202 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/engine/cli.py
--rw-r--r--   0        0        0     2068 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/engine/conn.py
--rw-r--r--   0        0        0     8163 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/engine/download.py
--rw-r--r--   0        0        0     4262 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/exceptions.py
--rw-r--r--   0        0        0      677 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/log.py
--rw-r--r--   0        0        0        0 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/py.typed
--rw-r--r--   0        0        0     2320 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/server/__init__.py
--rw-r--r--   0        0        0       78 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/server/__main__.py
--rw-r--r--   0        0        0      911 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/server/cli.py
--rw-r--r--   0        0        0      865 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/server/converter.py
--rw-r--r--   0        0        0     3892 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/session.py
--rw-r--r--   0        0        0        0 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/transport/__init__.py
--rw-r--r--   0        0        0     5820 2023-06-02 13:32:48.484901 dagger_io-0.6.1/src/dagger/transport/httpx.py
--rw-r--r--   0        0        0     5951 1970-01-01 00:00:00.000000 dagger_io-0.6.1/setup.py
--rw-r--r--   0        0        0     6524 1970-01-01 00:00:00.000000 dagger_io-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    10758 2023-06-15 23:19:36.174779 dagger_io-0.6.2/LICENSE
+-rw-r--r--   0        0        0     4762 2023-06-15 23:19:36.174779 dagger_io-0.6.2/README.md
+-rw-r--r--   0        0        0     6531 2023-06-15 23:20:36.607025 dagger_io-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      360 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/__init__.py
+-rw-r--r--   0        0        0       71 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/__main__.py
+-rw-r--r--   0        0        0       69 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/api/.gitattributes
+-rw-r--r--   0        0        0        0 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/api/__init__.py
+-rw-r--r--   0        0        0    11873 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/api/base.py
+-rw-r--r--   0        0        0    91550 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/api/gen.py
+-rw-r--r--   0        0        0    91142 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/api/gen_sync.py
+-rw-r--r--   0        0        0     1683 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/cli.py
+-rw-r--r--   0        0        0    20466 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/codegen.py
+-rw-r--r--   0        0        0     1302 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/config.py
+-rw-r--r--   0        0        0     1924 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/connection.py
+-rw-r--r--   0        0        0      964 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/context.py
+-rw-r--r--   0        0        0       37 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/engine/.gitattributes
+-rw-r--r--   0        0        0       35 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/engine/__init__.py
+-rw-r--r--   0        0        0       64 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/engine/_version.py
+-rw-r--r--   0        0        0     4201 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/engine/cli.py
+-rw-r--r--   0        0        0     2066 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/engine/conn.py
+-rw-r--r--   0        0        0     8162 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/engine/download.py
+-rw-r--r--   0        0        0     4262 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/exceptions.py
+-rw-r--r--   0        0        0      677 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/log.py
+-rw-r--r--   0        0        0        0 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/py.typed
+-rw-r--r--   0        0        0     2319 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/server/__init__.py
+-rw-r--r--   0        0        0       78 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/server/__main__.py
+-rw-r--r--   0        0        0      911 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/server/cli.py
+-rw-r--r--   0        0        0      865 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/server/converter.py
+-rw-r--r--   0        0        0     3890 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/session.py
+-rw-r--r--   0        0        0        0 2023-06-15 23:19:36.174779 dagger_io-0.6.2/src/dagger/transport/__init__.py
+-rw-r--r--   0        0        0     5811 2023-06-15 23:19:36.178779 dagger_io-0.6.2/src/dagger/transport/httpx.py
+-rw-r--r--   0        0        0     6409 1970-01-01 00:00:00.000000 dagger_io-0.6.2/PKG-INFO
```

### Comparing `dagger_io-0.6.1/LICENSE` & `dagger_io-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.1/README.md` & `dagger_io-0.6.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Dagger Python SDK
 
-[![PyPI Version](https://img.shields.io/pypi/v/dagger-io)](https://pypi.org/project/dagger-io/) 
+[![PyPI Version](https://img.shields.io/pypi/v/dagger-io)](https://pypi.org/project/dagger-io/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/dagger-io.svg)](https://anaconda.org/conda-forge/dagger-io)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/dagger-io.svg)](https://pypi.org/project/dagger-io/)
 [![License](https://img.shields.io/pypi/l/dagger-io.svg)](https://pypi.python.org/pypi/dagger-io)
 [![Code style](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
 
 A client package for running [Dagger](https://dagger.io/) pipelines.
@@ -108,19 +108,19 @@
 ```
 
 The following commands are available:
 - `poe test`: Run tests.
 - `poe fmt`: Re-format code following common styling conventions.
 - `poe lint`: Check for linting violations.
 - `poe generate`: Regenerate API client after changes to the codegen.
-- `poe docs`: Build reference docs locally.
+- `poe docs`: Build reference docs locally (needs `poetry install --with docs`).
 
 ### Engine changes
 
-Testing and regenerating the client may fail if there’s changes in the engine code that haven’t been released yet. 
+Testing and regenerating the client may fail if there’s changes in the engine code that haven’t been released yet.
 
 The simplest way to run those commands locally with the most updated engine version is to build it using [Dagger’s CI pipelines](https://github.com/dagger/dagger/blob/main/internal/mage/sdk/python.go) :
 
 ```shell
 ../../hack/make sdk:python:test
 ../../hack/make sdk:python:generate
 ```
```

### Comparing `dagger_io-0.6.1/pyproject.toml` & `dagger_io-0.6.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dagger-io"
-version = "0.6.1"
+version = "0.6.2"
 description = "A client package for running Dagger pipelines in Python."
 license = "Apache-2.0"
 authors = ["Dagger <hello@dagger.io>"]
 readme = "README.md"
 homepage = "https://dagger.io"
 documentation = "https://docs.dagger.io/sdk/python"
 repository = "https://github.com/dagger/dagger/tree/main/sdk/python"
@@ -19,15 +19,15 @@
     "Framework :: Pytest",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: Apache Software License",
-    # FIXME: just waiting on windows tests for this
+    # TODO: just waiting on windows tests for this
     # "Operating System :: OS Independent",
     "Typing :: Typed",
 ]
 packages = [
     { include = "dagger", from = "src" },
 ]
 
@@ -39,15 +39,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 anyio = ">=3.6.2"
 attrs = ">=22.1.0"
 cattrs = ">=22.2.0"
 graphql-core = ">=3.2.3"
-# FIXME: replace next two lines with the following when gql version 3.5.0 is released
+# TODO: replace next two lines with the following when gql version 3.5.0 is released
 # gql = {version = ">=3.5.0", extras = ["httpx"]}
 gql = ">=3.4.0"
 httpx = ">=0.23.1"
 beartype = ">=0.11.0"
 platformdirs = ">=2.6.2"
 typing_extensions = ">=4.4.0"
 rich = ">=12.6.0"
@@ -68,70 +68,85 @@
 black = ">=22.3.0"
 mypy = ">=0.942"
 ruff = ">=0.0.218"
 
 [tool.poetry.group.dev.dependencies]
 poethepoet = ">=0.16.4"
 
+[tool.poetry.group.docs]
+optional = true
+
 [tool.poetry.group.docs.dependencies]
 sphinx = ">=5.3.0"
 sphinx-rtd-theme = "^1.1.1"
 
 [tool.poe.env]
 GEN_PATH = "./src/dagger/api"
 
 [tool.poe.env.DOCS_SNIPPETS]
-default = "../../docs/current/sdk/python/snippets"
+default = "../../docs/current"
 
 [tool.poe.tasks]
 test = "pytest"
 unittest = "pytest -m 'not slow'"
 typing = "mypy src/dagger tests"
 
 [tool.poe.tasks.docs]
 cmd = "sphinx-build -v . _build"
 cwd = "docs"
 
 [tool.poe.tasks.lint]
 sequence = [
-    "ruff ${target}",
-    "black --check ${target}",
+    "ruff check ${target}",
+    "black --preview --check ${target}",
 ]
 default_item_type = "cmd"
 
 [[tool.poe.tasks.lint.args]]
 name = "target"
 positional = true
 multiple = true
 default = "."
 
 [tool.poe.tasks.lint-docs]
 ref = "lint ${DOCS_SNIPPETS}"
 
 [tool.poe.tasks.lint-all]
-ref = "lint . ${DOCS_SNIPPETS}"
+sequence = [
+    "lint",
+    "lint-docs",
+]
 
 [tool.poe.tasks.fmt]
 sequence = [
     "ruff --fix-only -e ${target}",
-    "black ${target}",
+    "black --preview ${target}",
 ]
 default_item_type = "cmd"
 
 [[tool.poe.tasks.fmt.args]]
 name = "target"
 positional = true
 multiple = true
-default = ". ${DOCS_SNIPPETS}"
+default = "."
+
+[tool.poe.tasks.fmt-docs]
+ref = "fmt ${DOCS_SNIPPETS}"
+
+[tool.poe.tasks.fmt-all]
+sequence = [
+    "fmt",
+    "fmt-docs",
+]
 
 [tool.poe.tasks.generate]
 sequence = [
     "python -m dagger generate --output ${GEN_PATH}/gen.py",
     "python -m dagger generate --output ${GEN_PATH}/gen_sync.py --sync",
-    "black ${GEN_PATH}/gen*.py",
+    "black --preview ${GEN_PATH}/gen*.py",
 ]
 default_item_type = "cmd"
 
 [tool.pytest.ini_options]
 testpaths = ["tests/"]
 addopts = [
     "--import-mode=importlib",
@@ -168,15 +183,15 @@
     # Type inferrance is ok in a lot of places.
     "ANN",
     # This rule doesn't know to ignore a subclass override
     # so we get false positives for unused arguments.
     "ARG002",
     # Black can handle trailing commas automatically.
     "COM812",
-    # FIXME: prefix everything internal with an underscore and document
+    # TODO: prefix everything internal with an underscore and document
     # what's left (public).
     "D1",
     # Imperative mood only makes sense in functions, not classes.
     "D401",
     # Not using timezones in this project.
     "DTZ",
     # Allow logging with default %. You need custom setup to use `extra`.
@@ -186,14 +201,18 @@
     # Unnecessary variable assignment before `return` statement
     # doesn't seem to work as expected.
     "RET504",
     # We don't use asserts as runtime validation guarantees.
     "S101",
     # Don't guard types. Don't want to stringize them.
     "TCH",
+    # Don't require author and link in TODO comments.
+    "TD002",
+    "TD003",
+    "FIX002",
     # Pandas
     "PD",
 ]
 unfixable = [
     # Don't remove `print` statements, just warn.
     "T201",
 ]
@@ -201,16 +220,14 @@
 [tool.ruff.isort]
 known-first-party = ["dagger"]
 
 [tool.ruff.flake8-bugbear]
 extend-immutable-calls = ["typer.Option"]
 
 [tool.ruff.per-file-ignores]
-# Docs and examples can have `print` statements.
-"../../docs/current/sdk/python/*.py" = ["T201"]
 "./examples/*" = ["T201"]
 "./src/dagger/api/gen*.py" = [
     # Not much control over field names and docs coming from the API.
     # Note: We could detect built-in shadowing like the reserved
     # keywords but these built-ins aren't being used in the generated
     # code so no need to bother.
     "A",
@@ -232,12 +249,11 @@
     "PLR2004",
     # Allow more than one statement in pytest.raises.
     "PT012",
 ]
 # Allow some patterns to redefine imports in __init__.
 "__init__.py" = ["F401", "F403", "PLC0414"]
 # Typer uses boolean parameters for the CLI. Let it.
-"./src/dagger/cli.py" = ["FBT"]
-"./src/dagger/server/cli.py" = ["FBT"]
+"./src/**/cli.py" = ["FBT"]
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
```

### Comparing `dagger_io-0.6.1/src/dagger/api/base.py` & `dagger_io-0.6.2/src/dagger/api/base.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.1/src/dagger/api/gen.py` & `dagger_io-0.6.2/src/dagger/api/gen.py`

 * *Files 0% similar despite different names*

```diff
@@ -442,14 +442,17 @@
         _ctx = self._select("export", _args)
         return await _ctx.execute(bool)
 
     @typecheck
     def exposed_ports(self) -> "Port":
         """Retrieves the list of exposed ports.
 
+        This includes ports already exposed by the image, even if not
+        explicitly added with dagger.
+
         Currently experimental; set _EXPERIMENTAL_DAGGER_SERVICES_DNS=0 to
         disable.
         """
         _args: list[Arg] = []
         _ctx = self._select("exposedPorts", _args)
         return Port(_ctx)
 
@@ -2003,21 +2006,29 @@
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("contents", _args)
         return await _ctx.execute(str)
 
     @typecheck
-    async def export(self, path: str) -> bool:
+    async def export(
+        self,
+        path: str,
+        allow_parent_dir_path: Optional[bool] = None,
+    ) -> bool:
         """Writes the file to a file path on the host.
 
         Parameters
         ----------
         path:
             Location of the written directory (e.g., "output.txt").
+        allow_parent_dir_path:
+            If allowParentDirPath is true, the path argument can be a
+            directory path, in which case
+            the file will be created in that directory.
 
         Returns
         -------
         bool
             The `Boolean` scalar type represents `true` or `false`.
 
         Raises
@@ -2025,14 +2036,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args = [
             Arg("path", path),
+            Arg("allowParentDirPath", allow_parent_dir_path, None),
         ]
         _ctx = self._select("export", _args)
         return await _ctx.execute(bool)
 
     @typecheck
     async def id(self) -> FileID:
         """Retrieves the content-addressed identifier of the file.
@@ -2062,15 +2074,18 @@
         """Retrieves a secret referencing the contents of this file.
 
         .. deprecated::
             insecure, leaves secret in cache. Superseded by
             :py:meth:`set_secret`
         """
         warnings.warn(
-            'Method "secret" is deprecated: insecure, leaves secret in cache. Superseded by "set_secret"',
+            (
+                'Method "secret" is deprecated: insecure, leaves secret in cache.'
+                ' Superseded by "set_secret"'
+            ),
             DeprecationWarning,
             stacklevel=4,
         )
         _args: list[Arg] = []
         _ctx = self._select("secret", _args)
         return Secret(_ctx)
 
@@ -2291,14 +2306,29 @@
         _args = [
             Arg("name", name),
         ]
         _ctx = self._select("envVariable", _args)
         return HostVariable(_ctx)
 
     @typecheck
+    def file(self, path: str) -> File:
+        """Accesses a file on the host.
+
+        Parameters
+        ----------
+        path:
+            Location of the file to retrieve (e.g., "README.md").
+        """
+        _args = [
+            Arg("path", path),
+        ]
+        _ctx = self._select("file", _args)
+        return File(_ctx)
+
+    @typecheck
     def unix_socket(self, path: str) -> "Socket":
         """Accesses a Unix socket on the host.
 
         Parameters
         ----------
         path:
             Location of the Unix socket (e.g., "/var/run/docker.sock").
@@ -2326,15 +2356,18 @@
             Exclude artifacts that match the given pattern (e.g.,
             ["node_modules/", ".git*"]).
         include:
             Include only artifacts that match the given pattern (e.g.,
             ["app/", "package.*"]).
         """
         warnings.warn(
-            'Method "workdir" is deprecated: Use "directory" with path set to \'.\' instead.',
+            (
+                'Method "workdir" is deprecated: Use "directory" with path set to \'.\''
+                " instead."
+            ),
             DeprecationWarning,
             stacklevel=4,
         )
         _args = [
             Arg("exclude", exclude, None),
             Arg("include", include, None),
         ]
@@ -2508,38 +2541,36 @@
     def commands(self) -> "ProjectCommand":
         """Commands provided by this project"""
         _args: list[Arg] = []
         _ctx = self._select("commands", _args)
         return ProjectCommand(_ctx)
 
     @typecheck
-    async def id(self) -> str:
+    async def id(self) -> ProjectID:
         """A unique identifier for this project.
 
         Note
         ----
         This is lazyly evaluated, no operation is actually run.
 
         Returns
         -------
-        str
-            The `String` scalar type represents textual data, represented as
-            UTF-8 character sequences. The String type is most often used by
-            GraphQL to represent free-form human-readable text.
+        ProjectID
+            A unique project identifier.
 
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
-        return await _ctx.execute(str)
+        return await _ctx.execute(ProjectID)
 
     @typecheck
     def load(
         self,
         source: Directory,
         config_path: str,
     ) -> "Project":
@@ -2603,38 +2634,36 @@
     def flags(self) -> "ProjectCommandFlag":
         """Flags accepted by this command."""
         _args: list[Arg] = []
         _ctx = self._select("flags", _args)
         return ProjectCommandFlag(_ctx)
 
     @typecheck
-    async def id(self) -> str:
+    async def id(self) -> ProjectCommandID:
         """A unique identifier for this command.
 
         Note
         ----
         This is lazyly evaluated, no operation is actually run.
 
         Returns
         -------
-        str
-            The `String` scalar type represents textual data, represented as
-            UTF-8 character sequences. The String type is most often used by
-            GraphQL to represent free-form human-readable text.
+        ProjectCommandID
+            A unique project command identifier.
 
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
-        return await _ctx.execute(str)
+        return await _ctx.execute(ProjectCommandID)
 
     @typecheck
     async def name(self) -> str:
         """The name of the command.
 
         Returns
         -------
@@ -2651,14 +2680,36 @@
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
         return await _ctx.execute(str)
 
     @typecheck
+    async def result_type(self) -> Optional[str]:
+        """The name of the type returned by this command.
+
+        Returns
+        -------
+        Optional[str]
+            The `String` scalar type represents textual data, represented as
+            UTF-8 character sequences. The String type is most often used by
+            GraphQL to represent free-form human-readable text.
+
+        Raises
+        ------
+        ExecuteTimeoutError
+            If the time to execute the query exceeds the configured timeout.
+        QueryError
+            If the API returns an error.
+        """
+        _args: list[Arg] = []
+        _ctx = self._select("resultType", _args)
+        return await _ctx.execute(Optional[str])
+
+    @typecheck
     def subcommands(self) -> "ProjectCommand":
         """Subcommands, if any, that this command provides."""
         _args: list[Arg] = []
         _ctx = self._select("subcommands", _args)
         return ProjectCommand(_ctx)
 
 
@@ -2901,14 +2952,15 @@
         _ctx = self._select("secret", _args)
         return Secret(_ctx)
 
     @typecheck
     def set_secret(self, name: str, plaintext: str) -> "Secret":
         """Sets a secret given a user defined name to its plaintext and returns
         the secret.
+        The plaintext value is limited to a size of 128000 bytes.
 
         Parameters
         ----------
         name:
             The user defined name for this secret
         plaintext:
             The plaintext of the secret
```

### Comparing `dagger_io-0.6.1/src/dagger/api/gen_sync.py` & `dagger_io-0.6.2/src/dagger/api/gen_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -442,14 +442,17 @@
         _ctx = self._select("export", _args)
         return _ctx.execute_sync(bool)
 
     @typecheck
     def exposed_ports(self) -> "Port":
         """Retrieves the list of exposed ports.
 
+        This includes ports already exposed by the image, even if not
+        explicitly added with dagger.
+
         Currently experimental; set _EXPERIMENTAL_DAGGER_SERVICES_DNS=0 to
         disable.
         """
         _args: list[Arg] = []
         _ctx = self._select("exposedPorts", _args)
         return Port(_ctx)
 
@@ -2000,21 +2003,29 @@
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("contents", _args)
         return _ctx.execute_sync(str)
 
     @typecheck
-    def export(self, path: str) -> bool:
+    def export(
+        self,
+        path: str,
+        allow_parent_dir_path: Optional[bool] = None,
+    ) -> bool:
         """Writes the file to a file path on the host.
 
         Parameters
         ----------
         path:
             Location of the written directory (e.g., "output.txt").
+        allow_parent_dir_path:
+            If allowParentDirPath is true, the path argument can be a
+            directory path, in which case
+            the file will be created in that directory.
 
         Returns
         -------
         bool
             The `Boolean` scalar type represents `true` or `false`.
 
         Raises
@@ -2022,14 +2033,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args = [
             Arg("path", path),
+            Arg("allowParentDirPath", allow_parent_dir_path, None),
         ]
         _ctx = self._select("export", _args)
         return _ctx.execute_sync(bool)
 
     @typecheck
     def id(self) -> FileID:
         """Retrieves the content-addressed identifier of the file.
@@ -2059,15 +2071,18 @@
         """Retrieves a secret referencing the contents of this file.
 
         .. deprecated::
             insecure, leaves secret in cache. Superseded by
             :py:meth:`set_secret`
         """
         warnings.warn(
-            'Method "secret" is deprecated: insecure, leaves secret in cache. Superseded by "set_secret"',
+            (
+                'Method "secret" is deprecated: insecure, leaves secret in cache.'
+                ' Superseded by "set_secret"'
+            ),
             DeprecationWarning,
             stacklevel=4,
         )
         _args: list[Arg] = []
         _ctx = self._select("secret", _args)
         return Secret(_ctx)
 
@@ -2288,14 +2303,29 @@
         _args = [
             Arg("name", name),
         ]
         _ctx = self._select("envVariable", _args)
         return HostVariable(_ctx)
 
     @typecheck
+    def file(self, path: str) -> File:
+        """Accesses a file on the host.
+
+        Parameters
+        ----------
+        path:
+            Location of the file to retrieve (e.g., "README.md").
+        """
+        _args = [
+            Arg("path", path),
+        ]
+        _ctx = self._select("file", _args)
+        return File(_ctx)
+
+    @typecheck
     def unix_socket(self, path: str) -> "Socket":
         """Accesses a Unix socket on the host.
 
         Parameters
         ----------
         path:
             Location of the Unix socket (e.g., "/var/run/docker.sock").
@@ -2323,15 +2353,18 @@
             Exclude artifacts that match the given pattern (e.g.,
             ["node_modules/", ".git*"]).
         include:
             Include only artifacts that match the given pattern (e.g.,
             ["app/", "package.*"]).
         """
         warnings.warn(
-            'Method "workdir" is deprecated: Use "directory" with path set to \'.\' instead.',
+            (
+                'Method "workdir" is deprecated: Use "directory" with path set to \'.\''
+                " instead."
+            ),
             DeprecationWarning,
             stacklevel=4,
         )
         _args = [
             Arg("exclude", exclude, None),
             Arg("include", include, None),
         ]
@@ -2505,38 +2538,36 @@
     def commands(self) -> "ProjectCommand":
         """Commands provided by this project"""
         _args: list[Arg] = []
         _ctx = self._select("commands", _args)
         return ProjectCommand(_ctx)
 
     @typecheck
-    def id(self) -> str:
+    def id(self) -> ProjectID:
         """A unique identifier for this project.
 
         Note
         ----
         This is lazyly evaluated, no operation is actually run.
 
         Returns
         -------
-        str
-            The `String` scalar type represents textual data, represented as
-            UTF-8 character sequences. The String type is most often used by
-            GraphQL to represent free-form human-readable text.
+        ProjectID
+            A unique project identifier.
 
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
-        return _ctx.execute_sync(str)
+        return _ctx.execute_sync(ProjectID)
 
     @typecheck
     def load(
         self,
         source: Directory,
         config_path: str,
     ) -> "Project":
@@ -2600,38 +2631,36 @@
     def flags(self) -> "ProjectCommandFlag":
         """Flags accepted by this command."""
         _args: list[Arg] = []
         _ctx = self._select("flags", _args)
         return ProjectCommandFlag(_ctx)
 
     @typecheck
-    def id(self) -> str:
+    def id(self) -> ProjectCommandID:
         """A unique identifier for this command.
 
         Note
         ----
         This is lazyly evaluated, no operation is actually run.
 
         Returns
         -------
-        str
-            The `String` scalar type represents textual data, represented as
-            UTF-8 character sequences. The String type is most often used by
-            GraphQL to represent free-form human-readable text.
+        ProjectCommandID
+            A unique project command identifier.
 
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
-        return _ctx.execute_sync(str)
+        return _ctx.execute_sync(ProjectCommandID)
 
     @typecheck
     def name(self) -> str:
         """The name of the command.
 
         Returns
         -------
@@ -2648,14 +2677,36 @@
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
         return _ctx.execute_sync(str)
 
     @typecheck
+    def result_type(self) -> Optional[str]:
+        """The name of the type returned by this command.
+
+        Returns
+        -------
+        Optional[str]
+            The `String` scalar type represents textual data, represented as
+            UTF-8 character sequences. The String type is most often used by
+            GraphQL to represent free-form human-readable text.
+
+        Raises
+        ------
+        ExecuteTimeoutError
+            If the time to execute the query exceeds the configured timeout.
+        QueryError
+            If the API returns an error.
+        """
+        _args: list[Arg] = []
+        _ctx = self._select("resultType", _args)
+        return _ctx.execute_sync(Optional[str])
+
+    @typecheck
     def subcommands(self) -> "ProjectCommand":
         """Subcommands, if any, that this command provides."""
         _args: list[Arg] = []
         _ctx = self._select("subcommands", _args)
         return ProjectCommand(_ctx)
 
 
@@ -2898,14 +2949,15 @@
         _ctx = self._select("secret", _args)
         return Secret(_ctx)
 
     @typecheck
     def set_secret(self, name: str, plaintext: str) -> "Secret":
         """Sets a secret given a user defined name to its plaintext and returns
         the secret.
+        The plaintext value is limited to a size of 128000 bytes.
 
         Parameters
         ----------
         name:
             The user defined name for this secret
         plaintext:
             The plaintext of the secret
```

### Comparing `dagger_io-0.6.1/src/dagger/cli.py` & `dagger_io-0.6.2/src/dagger/cli.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.1/src/dagger/codegen.py` & `dagger_io-0.6.2/src/dagger/codegen.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     id_map: IDMap = attrs.Factory(dict)
     """Map to convert ids (custom scalars) to corresponding types."""
 
     remaining: set[str] = attrs.Factory(set)
     """Remaining type names that haven't been defined yet."""
 
 
-# FIXME: break into class
+# TODO: break into class
 @joiner
 def generate(  # noqa: C901
     schema: GraphQLSchema,
     sync: bool = False,  # noqa: FBT001, FBT002
 ) -> Iterator[str]:
     """Code generation main function."""
     yield textwrap.dedent(
@@ -195,15 +195,15 @@
 
     yield ""
     yield "__all__ = ["
     yield from (indent(f'"{name}",') for name in defined)
     yield "]"
 
 
-# FIXME: these typeguards should be contributed upstream
+# TODO: these typeguards should be contributed upstream
 #        https://github.com/graphql-python/graphql-core/issues/183
 
 
 def is_required_type(t: GraphQLType) -> TypeGuard[GraphQLNonNull]:
     return isinstance(t, GraphQLNonNull)
 
 
@@ -271,15 +271,15 @@
     # only wrap optional and list when ready
     if is_output_leaf_type(t):
         return format_input_type(t, {})
 
     # when building the query return shouldn't be None
     # even if optional to not break the chain while
     # we're only building the query
-    # FIXME: detect this when returning the scalar
+    # TODO: detect this when returning the scalar
     #        since it affects the result
     if is_wrapping_type(t):
         return format_output_type(t.of_type)
 
     return Scalars.from_type(t) if is_scalar_type(t) else t.name
 
 
@@ -397,15 +397,15 @@
         self.description = field.description
 
         self.is_leaf = is_output_leaf_type(field.type)
         self.is_custom_scalar = is_custom_scalar_type(field.type)
         self.type = format_output_type(field.type).replace("Query", "Client")
         self.convert_id = False
 
-        # FIXME: We don't have a simple way to convert any ID to its
+        # TODO: We don't have a simple way to convert any ID to its
         # corresponding object (in codegen) so for now just return the
         # current instance. Currently, `sync` is the only field where
         # the error is what we care about but more could be added later.
         # To avoid wasting a result, we return the ID which is a leaf value
         # and triggers execution, but then convert to object in the SDK to
         # allow continued chaining. For this, we're assuming the returned
         # ID represents the exact same object but if that changes, we'll
@@ -455,23 +455,21 @@
         if docstring := self.func_doc():
             yield doc(docstring)
 
         if deprecated := self.deprecated():
             msg = f'Method "{self.name}" is deprecated: {deprecated}'.replace(
                 '"', '\\"'
             )
-            yield textwrap.dedent(
-                f"""\
+            yield textwrap.dedent(f"""\
                 warnings.warn(
                     "{msg}",
                     DeprecationWarning,
                     stacklevel=4,
                 )\
-                """
-            )
+                """)
 
         if not self.args:
             yield "_args: list[Arg] = []"
         else:
             yield "_args = ["
             yield from (indent(arg.as_arg()) for arg in self.args)
             yield "]"
```

### Comparing `dagger_io-0.6.1/src/dagger/config.py` & `dagger_io-0.6.2/src/dagger/config.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.1/src/dagger/connection.py` & `dagger_io-0.6.2/src/dagger/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,17 +44,19 @@
         async with self.get_stack() as stack:
             conn = await stack.enter_async_context(Engine(self.cfg))
             session = await stack.enter_async_context(Session(conn, self.cfg))
         return Client.from_session(session)
 
     def __enter__(self) -> SyncClient:
         warnings.warn(
-            "The synchronous API is deprecated and will be removed in a future"
-            " release. See https://github.com/dagger/dagger/issues/5192"
-            " for more information.",
+            (
+                "The synchronous API is deprecated and will be removed in a future"
+                " release. See https://github.com/dagger/dagger/issues/5192"
+                " for more information."
+            ),
             DeprecationWarning,
             stacklevel=2,
         )
         with self.get_sync_stack() as stack:
             conn = stack.enter_context(Engine(self.cfg))
             session = stack.enter_context(Session(conn, self.cfg))
         return SyncClient.from_session(session)
```

### Comparing `dagger_io-0.6.1/src/dagger/context.py` & `dagger_io-0.6.2/src/dagger/context.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.1/src/dagger/engine/cli.py` & `dagger_io-0.6.2/src/dagger/engine/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             else:
                 return proc
 
         msg = "CLI busy"
         raise SessionError(msg)
 
     def _get_conn(self, proc: subprocess.Popen) -> ConnectParams:
-        # FIXME: implement engine session timeout (self.cfg.engine_timeout?)
+        # TODO: implement engine session timeout (self.cfg.engine_timeout?)
         conn = proc.stdout.readline()
 
         # Check if subprocess exited with an error
         if ret := proc.poll():
             out = conn + proc.stdout.read()
             err = proc.stderr.read() if proc.stderr and proc.stderr.readable() else None
```

### Comparing `dagger_io-0.6.1/src/dagger/engine/conn.py` & `dagger_io-0.6.2/src/dagger/engine/conn.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     def __enter__(self) -> ConnectParams:
         self.is_async = False
         return self.start()
 
     async def __aenter__(self) -> ConnectParams:
         self.is_async = True
-        # FIXME: Create proper async provisioning later.
+        # TODO: Create proper async provisioning later.
         # This is just to support sync faster.
         return await anyio.to_thread.run_sync(self.start)
 
     async def __aexit__(self, *exc_details) -> None:
-        # FIXME: Create proper async provisioning later.
+        # TODO: Create proper async provisioning later.
         # This is just to support sync faster.
         await anyio.to_thread.run_sync(self.__exit__, *exc_details)
```

### Comparing `dagger_io-0.6.1/src/dagger/engine/download.py` & `dagger_io-0.6.2/src/dagger/engine/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,15 @@
                     break
             else:
                 msg = "There is no item named 'dagger' in the archive"
                 raise DownloadError(msg)
 
     @contextlib.contextmanager
     def _extract_from_zip(self, reader: StreamReader) -> Iterator[IO[bytes]]:
-        # FIXME: extract from stream instead of loading archive into memory
+        # TODO: extract from stream instead of loading archive into memory
         with zipfile.ZipFile(reader.getbuffer()) as zar:
             try:
                 with zar.open("dagger.exe") as file:
                     yield file
             except KeyError as e:
                 msg = "There is no item named 'dagger.exe' in the archive"
                 raise DownloadError(msg) from e
```

### Comparing `dagger_io-0.6.1/src/dagger/exceptions.py` & `dagger_io-0.6.2/src/dagger/exceptions.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.1/src/dagger/log.py` & `dagger_io-0.6.2/src/dagger/log.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.1/src/dagger/server/__init__.py` & `dagger_io-0.6.2/src/dagger/server/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     def _read_inputs(self) -> Inputs:
         return self.converter.loads(inputs_path.read_text(), Inputs)
 
     async def _call_resolver(self, inputs: Inputs):
         type_name, field_name = inputs.resolver.split(".", 2)
         field = self.schema.get_field_for_type(field_name, type_name)
         if field is None:
-            # FIXME: use proper error class
+            # TODO: use proper error class
             msg = f"Can't find field `{field_name}` for type `{type_name}`"
             raise RuntimeError(msg)
         resolver: Callable = self.schema.schema_converter.from_resolver(field)
         origin = cast(Callable, field.origin)
         parent = origin(**inputs.parent) if inputs.parent else origin()
         return await await_maybe(resolver(parent, info=None, **inputs.args))
```

### Comparing `dagger_io-0.6.1/src/dagger/server/cli.py` & `dagger_io-0.6.2/src/dagger/server/cli.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.1/src/dagger/server/converter.py` & `dagger_io-0.6.2/src/dagger/server/converter.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.6.1/src/dagger/session.py` & `dagger_io-0.6.2/src/dagger/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,26 +65,26 @@
         )
 
     async def __aenter__(self) -> AsyncClientSession:
         transport = self.make_transport()
         client = self.make_graphql_client(transport)
 
         async with self.get_stack() as stack:
-            # FIXME: handle cancellation, retries and timeout (self.cfg.timeout)
+            # TODO: handle cancellation, retries and timeout (self.cfg.timeout)
             with self._handle_connection():
                 session = await stack.enter_async_context(client)
 
         return session
 
     def __enter__(self) -> SyncClientSession:
         transport = self.make_sync_transport()
         client = self.make_graphql_client(transport)
 
         with self.get_sync_stack() as stack, self._handle_connection():
-            # FIXME: handle cancellation, retries and timeout (self.cfg.timeout)
+            # TODO: handle cancellation, retries and timeout (self.cfg.timeout)
             session = stack.enter_context(client)
 
         return session
 
     @contextlib.contextmanager
     def _handle_connection(self):
         # Reduces duplication when handling errors, between sync and async.
```

### Comparing `dagger_io-0.6.1/src/dagger/transport/httpx.py` & `dagger_io-0.6.2/src/dagger/transport/httpx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # flake8: noqa
 """
 GraphQL client transport using HTTPX.
 
-FIXME: remove this file when gql releases a version with httpx support.
+TODO: remove this file when gql releases a version with httpx support.
     It was added in https://github.com/graphql-python/gql/pull/370
 """
 import io
 import json
 import logging
 from typing import Any, AsyncGenerator, Callable, Dict, Optional, Tuple, Type, Union
 
@@ -99,15 +99,15 @@
         try:
             # Raise a HTTPError if response status is 400 or higher
             response.raise_for_status()
         except httpx.HTTPStatusError as e:
             raise TransportServerError(str(e), e.response.status_code) from e
 
         raise TransportProtocolError(
-            f"Server did not return a GraphQL result: " f"{reason}: " f"{response.text}"
+            f"Server did not return a GraphQL result: {reason}: {response.text}"
         )
 
 
 class HTTPXTransport(Transport, _HTTPXTransport):
     client: Optional[httpx.Client] = None
 
     def connect(self):
```

### Comparing `dagger_io-0.6.1/setup.py` & `dagger_io-0.6.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,182 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dagger-io
+Version: 0.6.2
+Summary: A client package for running Dagger pipelines in Python.
+Home-page: https://dagger.io
+License: Apache-2.0
+Author: Dagger
+Author-email: hello@dagger.io
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Framework :: AnyIO
+Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Typing :: Typed
+Provides-Extra: server
+Requires-Dist: anyio (>=3.6.2)
+Requires-Dist: attrs (>=22.1.0)
+Requires-Dist: beartype (>=0.11.0)
+Requires-Dist: cattrs (>=22.2.0)
+Requires-Dist: gql (>=3.4.0)
+Requires-Dist: graphql-core (>=3.2.3)
+Requires-Dist: httpx (>=0.23.1)
+Requires-Dist: platformdirs (>=2.6.2)
+Requires-Dist: rich (>=12.6.0)
+Requires-Dist: strawberry-graphql (>=0.133.5) ; extra == "server"
+Requires-Dist: typer[all] (>=0.6.1)
+Requires-Dist: typing_extensions (>=4.4.0)
+Project-URL: Community, https://discord.gg/ufnyBtc8uY
+Project-URL: Documentation, https://docs.dagger.io/sdk/python
+Project-URL: Repository, https://github.com/dagger/dagger/tree/main/sdk/python
+Project-URL: Release Notes, https://github.com/dagger/dagger/releases?q=tag%3Asdk%2Fpython%2Fv0
+Project-URL: Tracker, https://github.com/dagger/dagger/issues
+Project-URL: Twitter, https://twitter.com/dagger_io
+Description-Content-Type: text/markdown
+
+# Dagger Python SDK
+
+[![PyPI Version](https://img.shields.io/pypi/v/dagger-io)](https://pypi.org/project/dagger-io/)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/dagger-io.svg)](https://anaconda.org/conda-forge/dagger-io)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/dagger-io.svg)](https://pypi.org/project/dagger-io/)
+[![License](https://img.shields.io/pypi/l/dagger-io.svg)](https://pypi.python.org/pypi/dagger-io)
+[![Code style](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
+
+A client package for running [Dagger](https://dagger.io/) pipelines.
+
+## What is the Dagger Python SDK?
+
+The Dagger Python SDK contains everything you need to develop CI/CD pipelines in Python, and run them on any OCI-compatible container runtime.
+
+## Requirements
+
+- Python 3.10 or later
+- [Docker](https://docs.docker.com/engine/install/), or another OCI-compatible container runtime
+
+A compatible version of the  [Dagger CLI](https://docs.dagger.io/cli) is automatically downloaded and run by the SDK for you, although it’s possible to manage it manually.
+
+## Installation
+
+From [PyPI](https://pypi.org/project/dagger-io/), using `pip`:
+
+```shell
+pip install dagger-io
+```
+
+You can also install via [Conda](https://anaconda.org/conda-forge/dagger-io), from the [conda-forge](https://conda-forge.org/docs/user/introduction.html#how-can-i-install-packages-from-conda-forge) channel:
+
+```shell
+conda install dagger-io
+```
+
+## Example
+
+Create a `main.py` file:
+
+```python
+import sys
+
+import anyio
+import dagger
+
+
+async def main(args: list[str]):
+    async with dagger.Connection() as client:
+        # build container with cowsay entrypoint
+        ctr = (
+            client.container()
+            .from_("python:alpine")
+            .with_exec(["pip", "install", "cowsay"])
+            .with_entrypoint(["cowsay"])
+        )
+
+        # run cowsay with requested message
+        result = await ctr.with_exec(args).stdout()
+
+    print(result)
+
+
+anyio.run(main, sys.argv[1:])
+```
+
+Run with:
+
+```console
+$ python main.py "Simple is better than complex"
+  _____________________________
+| Simple is better than complex |
+  =============================
+                             \
+                              \
+                                ^__^
+                                (oo)\_______
+                                (__)\       )\/\
+                                    ||----w |
+                                    ||     ||
+```
+
+> **Note**
+> It may take a while for it to finish, especially on first run with cold cache.
+
+If you need to debug, you can stream the logs from the engine with the `log_output`  config:
+
+```python
+config = dagger.Config(log_output=sys.stderr)
+async with dagger.Connection(config) as client:
+    ...
+```
+
+## Learn more
+
+- [Documentation](https://docs.dagger.io/sdk/python)
+- [API Reference](https://dagger-io.readthedocs.org)
+- [Source code](https://github.com/dagger/dagger/tree/main/sdk/python)
+
+## Development
+
+This library is maintained with [Poetry](https://python-poetry.org/docs/).
+
+If you already have a [Python 3.10 or later](https://docs.python.org/3/using/index.html) interpreter in your `$PATH`, you can let [Poetry manage](https://python-poetry.org/docs/basic-usage/#using-your-virtual-environment) the [virtual environment](https://packaging.python.org/en/latest/tutorials/installing-packages/#creating-virtual-environments) automatically. Otherwise you need to activate it first, before installing dependencies:
+
+```shell
+poetry install
+```
+
+The following commands are available:
+- `poe test`: Run tests.
+- `poe fmt`: Re-format code following common styling conventions.
+- `poe lint`: Check for linting violations.
+- `poe generate`: Regenerate API client after changes to the codegen.
+- `poe docs`: Build reference docs locally (needs `poetry install --with docs`).
+
+### Engine changes
+
+Testing and regenerating the client may fail if there’s changes in the engine code that haven’t been released yet.
+
+The simplest way to run those commands locally with the most updated engine version is to build it using [Dagger’s CI pipelines](https://github.com/dagger/dagger/blob/main/internal/mage/sdk/python.go) :
+
+```shell
+../../hack/make sdk:python:test
+../../hack/make sdk:python:generate
+```
+
+You can also build the CLI and use it directly within the Python SDK:
+
+```shell
+../../hack/dev poe test
+```
+
+Or build it separately and tell the SDK to use it directly (or any other CLI binary):
+
+```shell
+../../hack/make
+_EXPERIMENTAL_DAGGER_CLI_BIN=../../bin/dagger poe test
+```
 
-package_dir = \
-{'': 'src'}
 
-packages = \
-['dagger', 'dagger.api', 'dagger.engine', 'dagger.server', 'dagger.transport']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['anyio>=3.6.2',
- 'attrs>=22.1.0',
- 'beartype>=0.11.0',
- 'cattrs>=22.2.0',
- 'gql>=3.4.0',
- 'graphql-core>=3.2.3',
- 'httpx>=0.23.1',
- 'platformdirs>=2.6.2',
- 'rich>=12.6.0',
- 'typer[all]>=0.6.1',
- 'typing_extensions>=4.4.0']
-
-extras_require = \
-{'server': ['strawberry-graphql>=0.133.5']}
-
-setup_kwargs = {
-    'name': 'dagger-io',
-    'version': '0.6.1',
-    'description': 'A client package for running Dagger pipelines in Python.',
-    'long_description': '# Dagger Python SDK\n\n[![PyPI Version](https://img.shields.io/pypi/v/dagger-io)](https://pypi.org/project/dagger-io/) \n[![Conda Version](https://img.shields.io/conda/vn/conda-forge/dagger-io.svg)](https://anaconda.org/conda-forge/dagger-io)\n[![Supported Python Versions](https://img.shields.io/pypi/pyversions/dagger-io.svg)](https://pypi.org/project/dagger-io/)\n[![License](https://img.shields.io/pypi/l/dagger-io.svg)](https://pypi.python.org/pypi/dagger-io)\n[![Code style](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)\n\nA client package for running [Dagger](https://dagger.io/) pipelines.\n\n## What is the Dagger Python SDK?\n\nThe Dagger Python SDK contains everything you need to develop CI/CD pipelines in Python, and run them on any OCI-compatible container runtime.\n\n## Requirements\n\n- Python 3.10 or later\n- [Docker](https://docs.docker.com/engine/install/), or another OCI-compatible container runtime\n\nA compatible version of the  [Dagger CLI](https://docs.dagger.io/cli) is automatically downloaded and run by the SDK for you, although it’s possible to manage it manually.\n\n## Installation\n\nFrom [PyPI](https://pypi.org/project/dagger-io/), using `pip`:\n\n```shell\npip install dagger-io\n```\n\nYou can also install via [Conda](https://anaconda.org/conda-forge/dagger-io), from the [conda-forge](https://conda-forge.org/docs/user/introduction.html#how-can-i-install-packages-from-conda-forge) channel:\n\n```shell\nconda install dagger-io\n```\n\n## Example\n\nCreate a `main.py` file:\n\n```python\nimport sys\n\nimport anyio\nimport dagger\n\n\nasync def main(args: list[str]):\n    async with dagger.Connection() as client:\n        # build container with cowsay entrypoint\n        ctr = (\n            client.container()\n            .from_("python:alpine")\n            .with_exec(["pip", "install", "cowsay"])\n            .with_entrypoint(["cowsay"])\n        )\n\n        # run cowsay with requested message\n        result = await ctr.with_exec(args).stdout()\n\n    print(result)\n\n\nanyio.run(main, sys.argv[1:])\n```\n\nRun with:\n\n```console\n$ python main.py "Simple is better than complex"\n  _____________________________\n| Simple is better than complex |\n  =============================\n                             \\\n                              \\\n                                ^__^\n                                (oo)\\_______\n                                (__)\\       )\\/\\\n                                    ||----w |\n                                    ||     ||\n```\n\n> **Note**\n> It may take a while for it to finish, especially on first run with cold cache.\n\nIf you need to debug, you can stream the logs from the engine with the `log_output`  config:\n\n```python\nconfig = dagger.Config(log_output=sys.stderr)\nasync with dagger.Connection(config) as client:\n    ...\n```\n\n## Learn more\n\n- [Documentation](https://docs.dagger.io/sdk/python)\n- [API Reference](https://dagger-io.readthedocs.org)\n- [Source code](https://github.com/dagger/dagger/tree/main/sdk/python)\n\n## Development\n\nThis library is maintained with [Poetry](https://python-poetry.org/docs/).\n\nIf you already have a [Python 3.10 or later](https://docs.python.org/3/using/index.html) interpreter in your `$PATH`, you can let [Poetry manage](https://python-poetry.org/docs/basic-usage/#using-your-virtual-environment) the [virtual environment](https://packaging.python.org/en/latest/tutorials/installing-packages/#creating-virtual-environments) automatically. Otherwise you need to activate it first, before installing dependencies:\n\n```shell\npoetry install\n```\n\nThe following commands are available:\n- `poe test`: Run tests.\n- `poe fmt`: Re-format code following common styling conventions.\n- `poe lint`: Check for linting violations.\n- `poe generate`: Regenerate API client after changes to the codegen.\n- `poe docs`: Build reference docs locally.\n\n### Engine changes\n\nTesting and regenerating the client may fail if there’s changes in the engine code that haven’t been released yet. \n\nThe simplest way to run those commands locally with the most updated engine version is to build it using [Dagger’s CI pipelines](https://github.com/dagger/dagger/blob/main/internal/mage/sdk/python.go) :\n\n```shell\n../../hack/make sdk:python:test\n../../hack/make sdk:python:generate\n```\n\nYou can also build the CLI and use it directly within the Python SDK:\n\n```shell\n../../hack/dev poe test\n```\n\nOr build it separately and tell the SDK to use it directly (or any other CLI binary):\n\n```shell\n../../hack/make\n_EXPERIMENTAL_DAGGER_CLI_BIN=../../bin/dagger poe test\n```\n\n',
-    'author': 'Dagger',
-    'author_email': 'hello@dagger.io',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://dagger.io',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

