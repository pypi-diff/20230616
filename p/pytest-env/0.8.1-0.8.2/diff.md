# Comparing `tmp/pytest_env-0.8.1.tar.gz` & `tmp/pytest_env-0.8.2.tar.gz`

## Comparing `pytest_env-0.8.1.tar` & `pytest_env-0.8.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 pytest_env-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 pytest_env-0.8.1/tox.ini
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pytest_env-0.8.1/whitelist.txt
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 pytest_env-0.8.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pytest_env-0.8.1/.github/dependabot.yml
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 pytest_env-0.8.1/.github/workflows/check.yml
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pytest_env-0.8.1/src/pytest_env/__init__.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 pytest_env-0.8.1/src/pytest_env/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_env-0.8.1/src/pytest_env/py.typed
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pytest_env-0.8.1/src/pytest_env/version.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pytest_env-0.8.1/tests/conftest.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 pytest_env-0.8.1/tests/template.py
--rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 pytest_env-0.8.1/tests/test_env.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pytest_env-0.8.1/tests/test_version.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pytest_env-0.8.1/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pytest_env-0.8.1/LICENSE
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 pytest_env-0.8.1/README.md
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 pytest_env-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 pytest_env-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 pytest_env-0.8.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 pytest_env-0.8.2/tox.ini
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 pytest_env-0.8.2/.github/CODEOWNERS
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pytest_env-0.8.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pytest_env-0.8.2/.github/SECURITY.md
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 pytest_env-0.8.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 pytest_env-0.8.2/.github/workflows/check.yml
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 pytest_env-0.8.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pytest_env-0.8.2/src/pytest_env/__init__.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 pytest_env-0.8.2/src/pytest_env/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_env-0.8.2/src/pytest_env/py.typed
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pytest_env-0.8.2/src/pytest_env/version.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 pytest_env-0.8.2/tests/conftest.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 pytest_env-0.8.2/tests/template.py
+-rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 pytest_env-0.8.2/tests/test_env.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pytest_env-0.8.2/tests/test_version.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 pytest_env-0.8.2/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pytest_env-0.8.2/LICENSE
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 pytest_env-0.8.2/README.md
+-rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 pytest_env-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 pytest_env-0.8.2/PKG-INFO
```

### Comparing `pytest_env-0.8.1/.pre-commit-config.yaml` & `pytest_env-0.8.2/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,34 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
-      - id: check-ast
-      - id: check-builtin-literals
-      - id: check-docstring-first
-      - id: check-merge-conflict
-      - id: check-yaml
-      - id: check-toml
-      - id: debug-statements
       - id: end-of-file-fixer
       - id: trailing-whitespace
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v3.0.0
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: "v0.0.272"
     hooks:
-      - id: pyupgrade
-        args: [ "--py37-plus" ]
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
-    hooks:
-      - id: isort
+      - id: ruff
+        args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/psf/black
-    rev: 22.10.0
+    rev: 23.3.0
     hooks:
       - id: black
-        args: [ --safe ]
-  - repo: https://github.com/asottile/blacken-docs
-    rev: v1.12.1
-    hooks:
-      - id: blacken-docs
-        additional_dependencies: [ black==22.10 ]
-  - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.9.0
-    hooks:
-      - id: rst-backticks
   - repo: https://github.com/tox-dev/tox-ini-fmt
-    rev: "0.5.2"
+    rev: "1.3.0"
     hooks:
       - id: tox-ini-fmt
-        args: [ "-p", "fix" ]
-  - repo: https://github.com/PyCQA/flake8
-    rev: 5.0.4
-    hooks:
-      - id: flake8
-        additional_dependencies:
-        - flake8-bugbear==22.9.23
-        - flake8-comprehensions==3.10
-        - flake8-pytest-style==1.6
-        - flake8-spellcheck==0.28
-        - flake8-unused-arguments==0.0.12
-        - flake8-noqa==1.2.9
-        - pep8-naming==0.13.2
+        args: ["-p", "fix"]
+  - repo: https://github.com/tox-dev/pyproject-fmt
+    rev: "0.11.2"
+    hooks:
+      - id: pyproject-fmt
+        additional_dependencies: ["tox>=4.6"]
+  - repo: https://github.com/pre-commit/mirrors-prettier
+    rev: "v3.0.0-alpha.9-for-vscode"
+    hooks:
+      - id: prettier
+        args: ["--print-width=120", "--prose-wrap=always"]
+  - repo: meta
+    hooks:
+      - id: check-hooks-apply
+      - id: check-useless-excludes
```

### Comparing `pytest_env-0.8.1/tox.ini` & `pytest_env-0.8.2/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -1,73 +1,74 @@
 [tox]
-envlist =
+requires =
+    tox>=4.2
+env_list =
     fix
+    py312
     py311
     py310
     py39
     py38
     py37
     type
     readme
-isolated_build = true
 skip_missing_interpreters = true
-minversion = 3.21
 
 [testenv]
 description = run the tests with pytest
-setenv =
-    COVERAGE_FILE = {env:COVERAGE_FILE:{toxworkdir}{/}.coverage.{envname}}
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
-    HOMEPATH
-    PROGRAMDATA
 skip_install = true
 deps =
-    pre-commit>=2.20
+    pre-commit>=3.2.
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
-    mypy==0.982
+    mypy==1.3
+set_env =
+    {tty:MYPY_FORCE_COLOR = 1}
 commands =
     mypy --strict src
     mypy --strict tests
 
 [testenv:readme]
 description = check that the long description is valid
 skip_install = true
 deps =
-    build[virtualenv]>=0.8
-    twine>=4.0.1
-changedir = {toxinidir}
+    build[virtualenv]>=0.10
+    twine>=4.0.2
+change_dir = {toxinidir}
 commands =
     python -m build -o {envtmpdir} .
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
 
 [flake8]
```

### Comparing `pytest_env-0.8.1/.github/workflows/check.yml` & `pytest_env-0.8.2/.github/workflows/check.yml`

 * *Files 10% similar despite different names*

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
@@ -13,27 +14,28 @@
   test:
     name: test ${{ matrix.py }} - ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         py:
-          - "3.11.0-rc.2"
+          - "3.12.0-beta.2"
+          - "3.11"
           - "3.10"
           - "3.9"
           - "3.8"
           - "3.7"
         os:
-          - ubuntu-22.04
+          - ubuntu-latest
 
     steps:
       - name: Setup python for tox
         uses: actions/setup-python@v4
         with:
-          python-version: "3.10"
+          python-version: "3.11"
       - name: Install tox
         run: python -m pip install tox
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
       - name: Setup python for test ${{ matrix.py }}
         uses: actions/setup-python@v4
@@ -57,49 +59,26 @@
   check:
     name: ${{ matrix.tox_env }} - ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os:
-          - ubuntu-22.04
+          - ubuntu-latest
         tox_env:
           - dev
           - type
           - readme
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
-      - name: Setup Python "3.10"
+      - name: Setup Python "3.11"
         uses: actions/setup-python@v4
         with:
-          python-version: "3.10"
+          python-version: "3.11"
       - name: Install tox
         run: python -m pip install tox
       - name: Setup test suite
         run: tox -vv --notest -e ${{ matrix.tox_env }}
       - name: Run test suite
         run: tox --skip-pkg-install -e ${{ matrix.tox_env }}
-
-  publish:
-    if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
-    needs: [ test, check ]
-    runs-on: ubuntu-latest
-    steps:
-      - name: Setup python to build package
-        uses: actions/setup-python@v4
-        with:
-          python-version: "3.10"
-      - name: Install build
-        run: python -m pip install build
-      - uses: actions/checkout@v3
-        with:
-          fetch-depth: 0
-      - name: Build sdist and wheel
-        run: python -m build -s -w . -o dist
-      - name: Publish to PyPi
-        uses: pypa/gh-action-pypi-publish@v1.5.1
-        with:
-          skip_existing: true
-          user: __token__
-          password: ${{ secrets.pypi_password }}
```

### Comparing `pytest_env-0.8.1/src/pytest_env/plugin.py` & `pytest_env-0.8.2/src/pytest_env/plugin.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 
 def pytest_addoption(parser: pytest.Parser) -> None:
     """Add section to configuration files."""
     help_msg = "a line separated list of environment variables of the form (FLAG:)NAME=VALUE"
     parser.addini("env", type="linelist", help=help_msg, default=[])
 
 
-@pytest.hookimpl(tryfirst=True)  # type: ignore # untyped decorator
+@pytest.hookimpl(tryfirst=True)  # type: ignore[misc]
 def pytest_load_initial_conftests(
-    args: list[str], early_config: pytest.Config, parser: pytest.Parser  # noqa: U100
+    args: list[str],  # noqa: ARG001
+    early_config: pytest.Config,
+    parser: pytest.Parser,  # noqa: ARG001
 ) -> None:
     """Load environment variables from configuration files."""
     for line in early_config.getini("env"):
-
         # INI lines e.g. D:R:NAME=VAL has two flags (R and D), NAME key, and VAL value
         parts = line.partition("=")
         ini_key_parts = parts[0].split(":")
         flags = {k.strip().upper() for k in ini_key_parts[:-1]}
         # R: is a way to designate whether to use raw value -> perform no transformation of the value
         transform = "R" not in flags
         # D: is a way to mark the value to be set only if it does not exist yet
```

### Comparing `pytest_env-0.8.1/tests/test_env.py` & `pytest_env-0.8.2/tests/test_env.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,18 +89,23 @@
             "",
             {"MAGIC": "zero"},
             id="empty ini works",
         ),
     ],
 )
 def test_env(
-    testdir: pytest.Testdir, env: dict[str, str], ini: str, expected_env: dict[str, str], request: pytest.FixtureRequest
+    testdir: pytest.Testdir,
+    env: dict[str, str],
+    ini: str,
+    expected_env: dict[str, str],
+    request: pytest.FixtureRequest,
 ) -> None:
+    tmp_dir = Path(str(testdir.tmpdir))
     test_name = re.sub(r"\W|^(?=\d)", "_", request.node.callspec.id).lower()
-    Path(str(testdir.tmpdir / f"test_{test_name}.py")).symlink_to(Path(__file__).parent / "template.py")
-    (testdir.tmpdir / "pytest.ini").write_text(ini, encoding="utf-8")
+    Path(str(tmp_dir / f"test_{test_name}.py")).symlink_to(Path(__file__).parent / "template.py")
+    (tmp_dir / "pytest.ini").write_text(ini, encoding="utf-8")
 
     # monkeypatch persists env variables across parametrized tests, therefore using mock.patch.dict
     with mock.patch.dict(os.environ, {**env, "_TEST_ENV": repr(expected_env)}, clear=True):
         result = testdir.runpytest()
 
     result.assert_outcomes(passed=1)
```

### Comparing `pytest_env-0.8.1/LICENSE` & `pytest_env-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_env-0.8.1/README.md` & `pytest_env-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pytest_env-0.8.1/PKG-INFO` & `pytest_env-0.8.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-env
-Version: 0.8.1
+Version: 0.8.2
 Summary: py.test plugin that allows you to add environment variables.
 Project-URL: Homepage, https://github.com/pytest-dev/pytest-env
 Project-URL: Source, https://github.com/pytest-dev/pytest-env
 Project-URL: Tracker, https://github.com/pytest-dev/pytest-env/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>
 License: MIT License
         
@@ -30,22 +30,27 @@
 License-File: LICENSE
 Keywords: env,pytest
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
-Requires-Dist: pytest>=7.1.3
+Requires-Dist: pytest>=7.3.1
 Provides-Extra: test
-Requires-Dist: coverage>=6.5; extra == 'test'
+Requires-Dist: coverage>=7.2.7; extra == 'test'
 Requires-Dist: pytest-mock>=3.10; extra == 'test'
 Description-Content-Type: text/markdown
 
 # pytest-env
 
 [![PyPI](https://img.shields.io/pypi/v/pytest-env?style=flat-square)](https://pypi.org/project/pytest-env/)
 [![Supported Python
```

