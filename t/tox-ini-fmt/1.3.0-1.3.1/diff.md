# Comparing `tmp/tox_ini_fmt-1.3.0.tar.gz` & `tmp/tox_ini_fmt-1.3.1.tar.gz`

## Comparing `tox_ini_fmt-1.3.0.tar` & `tox_ini_fmt-1.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/tox.ini
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/src/tox_ini_fmt/__init__.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/src/tox_ini_fmt/__main__.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/src/tox_ini_fmt/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/src/tox_ini_fmt/py.typed
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/src/tox_ini_fmt/version.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/src/tox_ini_fmt/formatter/__init__.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/src/tox_ini_fmt/formatter/requires.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/src/tox_ini_fmt/formatter/section_order.py
--rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/src/tox_ini_fmt/formatter/test_env.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/src/tox_ini_fmt/formatter/tox_section.py
--rw-r--r--   0        0        0     5775 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/src/tox_ini_fmt/formatter/util.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/tests/conftest.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/tests/test_cli.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/tests/test_main.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/tests/test_tox_ini_fmt.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/tests/test_upgrade.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/tests/formatter/test_line_endings.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/tests/formatter/test_requires.py
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/tests/formatter/test_section_order.py
--rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/tests/formatter/test_test_env.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/tests/formatter/test_tox_section.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/.gitignore
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/LICENSE.txt
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/README.md
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     5371 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/tox.ini
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/src/tox_ini_fmt/__init__.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/src/tox_ini_fmt/__main__.py
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/src/tox_ini_fmt/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/src/tox_ini_fmt/py.typed
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/src/tox_ini_fmt/version.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/src/tox_ini_fmt/formatter/__init__.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/src/tox_ini_fmt/formatter/requires.py
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/src/tox_ini_fmt/formatter/section_order.py
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/src/tox_ini_fmt/formatter/test_env.py
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/src/tox_ini_fmt/formatter/tox_section.py
+-rw-r--r--   0        0        0     6850 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/src/tox_ini_fmt/formatter/util.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/tests/test_cli.py
+-rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/tests/test_main.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/tests/test_tox_ini_fmt.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/tests/test_upgrade.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/tests/formatter/test_line_endings.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/tests/formatter/test_requires.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/tests/formatter/test_section_order.py
+-rw-r--r--   0        0        0     5174 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/tests/formatter/test_test_env.py
+-rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/tests/formatter/test_tox_section.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/README.md
+-rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 tox_ini_fmt-1.3.1/PKG-INFO
```

### Comparing `tox_ini_fmt-1.3.0/tox.ini` & `tox_ini_fmt-1.3.1/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [tox]
 requires =
     tox>=4.2
 env_list =
     fix
+    py312
     py311
     py310
     py39
     py38
     py37
     type
     readme
@@ -16,40 +17,40 @@
 description = run the unit tests with pytest under {base_python}
 package = wheel
 wheel_build_env = .pkg
 extras =
     test
 set_env =
     COVERAGE_FILE = {work_dir}/.coverage.{env_name}
-    COVERAGE_PROCESS_START = {tox_root}/setup.cfg
+    COVERAGE_PROCESS_START = {tox_root}/pyproject.toml
     _COVERAGE_SRC = {env_site_packages_dir}/sphinx_argparse_cli
 commands =
     pytest {tty:--color=yes} {posargs: \
       --junitxml {work_dir}{/}junit.{env_name}.xml --cov {env_site_packages_dir}{/}tox_ini_fmt \
       --cov {tox_root}{/}tests --cov-fail-under=100 \
-      --cov-config=setup.cfg --no-cov-on-fail --cov-report term-missing:skip-covered --cov-context=test \
+      --cov-config=pyproject.toml --no-cov-on-fail --cov-report term-missing:skip-covered --cov-context=test \
       --cov-report html:{env_tmp_dir}{/}htmlcov --cov-report xml:{work_dir}{/}coverage.{env_name}.xml \
       tests}
 
 [testenv:fix]
 description = run static analysis and style check using flake8
 package = skip
 deps =
-    pre-commit>=3.2.1
+    pre-commit>=3.3.3
 pass_env =
     HOMEPATH
     PROGRAMDATA
 commands =
     pre-commit run --all-files --show-diff-on-failure
     python -c 'print("hint: run {envdir}/bin/pre-commit install to add checks as pre-commit hook")'
 
 [testenv:type]
 description = run type check on code base
 deps =
-    mypy==1.1.1
+    mypy==1.3
 set_env =
     {tty:MYPY_FORCE_COLOR = 1}
 commands =
     mypy src
     mypy tests
 
 [testenv:readme]
```

### Comparing `tox_ini_fmt-1.3.0/src/tox_ini_fmt/__main__.py` & `tox_ini_fmt-1.3.1/src/tox_ini_fmt/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Main entry point."""
 from __future__ import annotations
 
 import difflib
 import sys
 from pathlib import Path
 from typing import Iterable, Sequence
 
@@ -10,36 +11,47 @@
 
 GREEN = "\u001b[32m"
 RED = "\u001b[31m"
 RESET = "\u001b[0m"
 
 
 def color_diff(diff: Iterable[str]) -> Iterable[str]:
+    """
+    Display diff in colored mode.
+
+    :param diff: the diff lines
+    """
     for line in diff:
         if line.startswith("+"):
             yield GREEN + line + RESET
         elif line.startswith("-"):
             yield RED + line + RESET
         else:
             yield line
 
 
 def run(args: Sequence[str] | None = None) -> int:
+    """
+    Run the formatter.
+
+    :param args: CLI arguments
+    :return: exit code
+    """
     opts = cli_args(sys.argv[1:] if args is None else args)
     changed = False
     for tox_ini in opts.tox_ini:
         with tox_ini.open("rt") as file:
             before = file.read()
             original_newlines = file.newlines
         if isinstance(original_newlines, tuple):
             original_newlines = original_newlines[0]
         formatted = format_tox_ini(before, opts)
         changed |= before != formatted
         if opts.stdout:  # stdout just prints new format to stdout
-            print(formatted, end="")
+            print(formatted, end="")  # noqa: T201
         else:
             if before != formatted:
                 with tox_ini.open("wt", newline=original_newlines) as file:
                     file.write(formatted)
             try:
                 name = str(tox_ini.relative_to(Path.cwd()))
             except ValueError:
@@ -47,16 +59,16 @@
             diff = (
                 difflib.unified_diff(before.splitlines(), formatted.splitlines(), fromfile=name, tofile=name)
                 if changed
                 else []
             )
             if diff:
                 diff_text = "\n".join(color_diff(diff))
-                print(diff_text)  # print diff on change
+                print(diff_text)  # print diff on change  # noqa: T201
             else:
-                print(f"no change for {name}")
+                print(f"no change for {name}")  # noqa: T201
     # exit with non success on change
     return 1 if changed else 0
 
 
 if __name__ == "__main__":
-    sys.exit(run())
+    raise SystemExit(run())
```

### Comparing `tox_ini_fmt-1.3.0/src/tox_ini_fmt/cli.py` & `tox_ini_fmt-1.3.1/src/tox_ini_fmt/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,50 @@
+"""CLI argument parsing."""
 from __future__ import annotations
 
 import os
 from argparse import Action, ArgumentParser, ArgumentTypeError, Namespace
 from pathlib import Path
 from typing import Any, Sequence
 
 
 class ToxIniFmtNamespace(Namespace):
-    """Options for tox-ini-fmt tool"""
+    """Options for tox-ini-fmt tool."""
 
     tox_ini: list[Path]
     stdout: bool
     pin_toxenvs: list[str]
 
 
 def tox_ini_path_creator(argument: str) -> Path:
-    """Validate that tox.ini can be formatted.
+    """
+    Validate that tox.ini can be formatted.
 
     :param argument: the string argument passed in
     :return: the tox.ini path
     """
     path = Path(argument).absolute()
     if not path.exists():
-        raise ArgumentTypeError("path does not exists")
+        msg = "path does not exists"
+        raise ArgumentTypeError(msg)
     if not path.is_file():
-        raise ArgumentTypeError("path is not a file")
+        msg = "path is not a file"
+        raise ArgumentTypeError(msg)
     if not os.access(path, os.R_OK):
-        raise ArgumentTypeError("cannot read path")  # pragma: no cover
+        msg = "cannot read path"
+        raise ArgumentTypeError(msg)  # pragma: no cover
     if not os.access(path, os.W_OK):
-        raise ArgumentTypeError("cannot write path")  # pragma: no cover
+        msg = "cannot write path"
+        raise ArgumentTypeError(msg)  # pragma: no cover
     return path
 
 
 def cli_args(args: Sequence[str]) -> ToxIniFmtNamespace:
-    """Load the tools options.
+    """
+    Load the tools options.
 
     :param args: CLI arguments
     :return: the parsed options
     """
     parser = ArgumentParser()
     parser.add_argument(
         "-s",
@@ -45,18 +52,18 @@
         action="store_true",
         help="print the formatted text to the stdout (instead of update in-place)",
     )
 
     class CommaSeparatedStr(Action):
         def __call__(
             self,
-            parser: ArgumentParser,  # noqa: U100
+            parser: ArgumentParser,  # noqa: ARG002
             namespace: Namespace,
             values: str | Sequence[Any] | None,
-            option_string: str | None = None,  # noqa: U100
+            option_string: str | None = None,  # noqa: ARG002
         ) -> None:
             if isinstance(values, str):  # pragma: no cover
                 setattr(namespace, self.dest, [i.strip() for i in values.split(",")])
 
     parser.add_argument(
         "-p",
         dest="pin_toxenvs",
```

### Comparing `tox_ini_fmt-1.3.0/src/tox_ini_fmt/formatter/__init__.py` & `tox_ini_fmt-1.3.1/src/tox_ini_fmt/formatter/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Logic related to formatting the file."""
 from __future__ import annotations
 
 from configparser import ConfigParser
 from io import StringIO
 from pathlib import Path
 
 from tox_ini_fmt.cli import ToxIniFmtNamespace
@@ -10,21 +11,25 @@
 from .test_env import format_test_env
 from .tox_section import format_tox_section
 
 INDENTATION = "    "
 
 
 def format_tox_ini(tox_ini: str | Path, opts: ToxIniFmtNamespace | None = None) -> str:
+    """
+    Format a tox ini file.
+
+    :param tox_ini:
+    :param opts:
+    :return:
+    """
     if opts is None:
         opts = ToxIniFmtNamespace(pin_toxenvs=[])
     parser = ConfigParser(interpolation=None)
-    if isinstance(tox_ini, Path):
-        text = tox_ini.read_text()
-    else:
-        text = tox_ini
+    text = tox_ini.read_text() if isinstance(tox_ini, Path) else tox_ini
     parser.read_string(text)
 
     format_tox_section(parser, opts.pin_toxenvs)
     for section_name in parser.sections():
         if section_name == "testenv" or section_name.startswith("testenv:"):
             format_test_env(parser, section_name)
     order_sections(parser, opts.pin_toxenvs)
```

### Comparing `tox_ini_fmt-1.3.0/src/tox_ini_fmt/formatter/requires.py` & `tox_ini_fmt-1.3.1/src/tox_ini_fmt/formatter/requires.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Normalize requires values."""
 from __future__ import annotations
 
 from packaging.requirements import InvalidRequirement, Requirement
 
 
 def normalize_req(req: str) -> str:
     try:
@@ -10,27 +11,32 @@
         return req
 
     for spec in parsed.specifier:
         if spec.operator in (">=", "=="):
             version = spec.version
             while version.endswith(".0"):
                 version = version[:-2]
-                spec._spec = (spec._spec[0], version)
+                spec._spec = (spec._spec[0], version)  # noqa: SLF001
     return str(parsed)
 
 
 def _req_name(req: str) -> str:
     try:
         return Requirement(req).name
     except InvalidRequirement:
         return req
 
 
 def requires(raws: list[str]) -> list[str]:
+    """
+    Normalize a list of requires.
+
+    :param raws: the raw values
+    :return: the formatted values
+    """
     values = (normalize_req(req) for req in raws if req)
-    normalized = sorted(values, key=lambda req: (";" in req, _req_name(req), req))
-    return normalized
+    return sorted(values, key=lambda req: (";" in req, _req_name(req), req))
 
 
 __all__ = [
     "requires",
 ]
```

### Comparing `tox_ini_fmt-1.3.0/src/tox_ini_fmt/formatter/section_order.py` & `tox_ini_fmt-1.3.1/src/tox_ini_fmt/formatter/section_order.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,72 @@
+"""Order configuration sections."""
 from __future__ import annotations
 
 import itertools
-from configparser import ConfigParser
+from typing import TYPE_CHECKING
 
 from .util import order_env_list
 
+if TYPE_CHECKING:
+    from configparser import ConfigParser
+
 
 def order_sections(parser: ConfigParser, pin_toxenvs: list[str]) -> None:
     """
-    Start with tox, then testenv. The testenv elements follow the order within envlist. Then all other testenv elements,
-    and end it with any other sections present in the file (e.g. pytest/mypy configuration).
+    Order sections.
+
+    :param parser: the INI parsers
+    :param pin_toxenvs: envs to pin
     """
+    # Start with tox, then testenv. The testenv elements follow the order within envlist. Then all other testenv
+    # elements and end it with any other sections present in the file (e.g. pytest/mypy configuration).
     order = ["tox", "testenv"]
     order.extend(f"testenv:{env}" for env in load_and_order_env_list(parser, pin_toxenvs))
     order.extend(s for s in parser.sections() if s not in order and s.startswith("testenv:"))
     order.extend(s for s in parser.sections() if s not in order and not s.startswith("testenv:"))
     sections: dict[str, dict[str, str]] = {}
     for section in order:
         if parser.has_section(section):
             sections[section] = dict(parser[section])
             parser.pop(section)
     for k, v in sections.items():
         parser[k] = v
 
 
 def load_and_order_env_list(parser: ConfigParser, pin_toxenvs: list[str]) -> list[str]:
+    """
+    Load and order tox env list.
+
+    :param parser: the INI parser
+    :param pin_toxenvs: envs to pint at the top
+    :return: the expanded and ordered list.
+    """
     result: list[str] = next(
         (explode_env_list(parser["tox"][i]) for i in ("envlist", "env_list") if i in parser["tox"]),
         [],
     )
     missing = [e for e in pin_toxenvs if e not in result]
     if missing:
-        raise RuntimeError(f"missing tox environment(s) to pin {', '.join(missing)}")
+        msg = f"missing tox environment(s) to pin {', '.join(missing)}"
+        raise RuntimeError(msg)
     order_env_list(result, pin_toxenvs)
     return result
 
 
 def explode_env_list(env_list: str) -> list[str]:
+    """
+    Explode a tox env list.
+
+    :param env_list: the raw value
+    :return: exploded representation
+    """
     result: list[str] = []
-    for entry in env_list.split("\n"):
-        entry = entry.strip()
+    for raw_entry in env_list.split("\n"):
+        entry = raw_entry.strip()
         if entry:
             parts = []
             for part in entry.split("-"):
-                if part[0] == "{" and part[-1] == "}":
-                    sub_part = part[1:-1]
-                else:
-                    sub_part = part
+                sub_part = part[1:-1] if part[0] == "{" and part[-1] == "}" else part
                 sub_parts = [i.strip() for i in sub_part.split(",")]
                 parts.append(sub_parts)
             result.extend("-".join(i).strip("-") for i in itertools.product(*parts))
     return result
```

### Comparing `tox_ini_fmt-1.3.0/src/tox_ini_fmt/formatter/test_env.py` & `tox_ini_fmt-1.3.1/src/tox_ini_fmt/formatter/test_env.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,26 @@
+"""Formatting the test environment sections."""
 from __future__ import annotations
 
-from configparser import ConfigParser
 from functools import partial
-from typing import Callable, Mapping
+from typing import TYPE_CHECKING, Callable, Mapping
 
 from .util import collect_multi_line, fix_and_reorder, fmt_list, to_boolean, to_list_of_env_values, to_py_dependencies
 
+if TYPE_CHECKING:
+    from configparser import ConfigParser
+
 
 def format_test_env(parser: ConfigParser, name: str) -> None:
+    """
+    Format a tox test environment.
+
+    :param parser: the INI parser
+    :param name:  name of the test env
+    """
     tox_section_cfg: Mapping[str, Callable[[str], str]] = {
         "runner": str,
         "description": str,
         "base_python": str,
         "system_site_packages": to_boolean,
         "always_copy": to_boolean,
         "download": to_boolean,
@@ -62,43 +71,62 @@
     if to_boolean(use_develop) == "true":
         parser[name]["package"] = "editable"
 
     fix_and_reorder(parser, name, tox_section_cfg, upgrade)
 
 
 def to_ordered_list(value: str) -> str:
-    """Must be a line separated list - fix comma separated format"""
+    """Must be a line separated list - fix comma separated format."""
     extras, substitute = collect_multi_line(value)
     return fmt_list(extras, substitute)
 
 
 def to_pass_env(value: str) -> str:
+    """
+    Format the pass env sections.
+
+    :param value:
+    :return:
+    """
     pass_env, substitute = collect_multi_line(value)
     return fmt_list(sorted(pass_env), substitute)
 
 
 def to_set_env(value: str) -> str:
+    """
+    Format the set env.
+
+    :param value:
+    :return:
+    """
     raw_set_env, substitute = collect_multi_line(value, line_split=None)
     set_env: list[str] = []
     for env in raw_set_env:
         at = env.find("=")
         if at == -1:
-            raise RuntimeError(f"invalid line {env} in setenv")
+            msg = f"invalid line {env} in setenv"
+            raise RuntimeError(msg)
         set_env.append(f"{env[:at].strip()} = {env[at+1:].strip()}")
     return fmt_list(sorted(set_env), substitute)
 
 
 _CMD_SEP = "\\"
 
 
 def to_commands(value: str) -> str:
+    """
+    Format the tox commands.
+
+    :param value: the raw value
+    :return: the formatted value
+    """
     result: list[str] = []
     ends_with_sep = False
-    for val in value.splitlines():
-        val = val.strip()
+    for raw_val in value.splitlines():
+        val = raw_val.strip()
         cur_ends_with_sep = val.endswith(_CMD_SEP)
         if cur_ends_with_sep:
             val = val[:-1].strip()
         if val and val != _CMD_SEP:
             ending = f" {_CMD_SEP}" if cur_ends_with_sep else ""
             prepend = "  " if ends_with_sep else ""
             result.append(f"{prepend}{val}{ending}")
```

### Comparing `tox_ini_fmt-1.3.0/src/tox_ini_fmt/formatter/tox_section.py` & `tox_ini_fmt-1.3.1/src/tox_ini_fmt/formatter/tox_section.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,30 @@
+"""Formatting the core tox section."""
 from __future__ import annotations
 
-from configparser import ConfigParser, SectionProxy
 from functools import partial
-from typing import Callable, Mapping
+from typing import TYPE_CHECKING, Callable, Mapping
 
 from packaging.requirements import Requirement
 from packaging.version import Version
 
 from .requires import requires
 from .util import collect_multi_line, fix_and_reorder, to_boolean, to_list_of_env_values, to_py_dependencies
 
+if TYPE_CHECKING:
+    from configparser import ConfigParser, SectionProxy
+
 
 def format_tox_section(parser: ConfigParser, pin_toxenvs: list[str]) -> None:
+    """
+    Format the core tox section.
+
+    :param parser: the INI parser
+    :param pin_toxenvs: environments to pin at start
+    """
     if not parser.has_section("tox"):
         parser.add_section("tox")
     tox = parser["tox"]
     _handle_min_version(tox)
     tox.pop("isolated_build", None)
 
     tox_section_cfg: Mapping[str, Callable[[str], str]] = {
@@ -39,15 +48,15 @@
         "ignore_basepython_conflict": "ignore_base_python_conflict",
     }
     fix_and_reorder(parser, "tox", tox_section_cfg, upgrade)
 
 
 def _handle_min_version(tox: SectionProxy) -> None:
     min_version = next((tox.pop(i) for i in ("minversion", "min_version") if i in tox), None)
-    if min_version is None or int(min_version.split(".")[0]) < 4:
+    if min_version is None or int(min_version.split(".")[0]) < 4:  # noqa: PLR2004
         min_version = "4.2"
     tox_requires = [
         Requirement(i)
         for i in collect_multi_line(
             tox.get("requires", ""),
             line_split=None,
             normalize=lambda groups: {k: requires(v) for k, v in groups.items()},
```

### Comparing `tox_ini_fmt-1.3.0/src/tox_ini_fmt/formatter/util.py` & `tox_ini_fmt-1.3.1/src/tox_ini_fmt/formatter/util.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,60 @@
+"""Utility methods."""
 from __future__ import annotations
 
 import itertools
 import re
 from collections import defaultdict
-from configparser import ConfigParser
 from functools import partial
-from typing import Callable, Mapping
+from typing import TYPE_CHECKING, Callable, Mapping
 
 from .requires import requires
 
+if TYPE_CHECKING:
+    from configparser import ConfigParser
+
 
 def to_boolean(payload: str) -> str:
+    """
+    Convert value to boolean.
+
+    :param payload: the raw value
+    :return: converted value
+    """
     return "true" if payload.lower() == "true" else "false"
 
 
 def fix_and_reorder(
     parser: ConfigParser,
     name: str,
     fix_cfg: Mapping[str, Callable[[str], str]],
     upgrade: dict[str, str],
 ) -> None:
+    """
+    Fix and reorder values.
+
+    :param parser: the INI parser
+    :param name:  name
+    :param fix_cfg: values to fix
+    :param upgrade: values to upgrade
+    """
     section = parser[name]
     # upgrade
     for key, to in upgrade.items():
         if key in section:
             if to in section:
-                raise RuntimeError(f"upgrade alias {to} also present for {key}")
+                msg = f"upgrade alias {to} also present for {key}"
+                raise RuntimeError(msg)
             section[to] = section.pop(key)
     # normalize
     for key, fix in fix_cfg.items():
         if key in section:
             section[key] = fix(section[key])
     # reorder keys within section
-    new_section = {k: section.pop(k) for k in fix_cfg.keys() if k in section}
+    new_section = {k: section.pop(k) for k in fix_cfg if k in section}
     new_section.update(sorted(section.items()))  # sort any remaining keys
     parser[name] = new_section
 
 
 RE_ITEM_REF = re.compile(
     r"""
         (?<!\\)[{]
@@ -46,30 +64,41 @@
         [}]
         """,
     re.VERBOSE,
 )
 
 
 def is_substitute(value: str) -> bool:
+    """
+    Check if has substitute value.
+
+    :param value: the raw value
+    """
     match = RE_ITEM_REF.match(value)
     if match:
         sub_key = match.group("substitution_value")
         return sub_key.startswith("[") and "]" in sub_key
     return False
 
 
 _MATCHER = re.compile(r"^([a-zA-Z]*)(\d*)$")
 
 
 def to_list_of_env_values(pin_toxenvs: list[str], payload: str) -> str:
     """
-    Example:
+    Expand list of tox envs.
+
+    :param pin_toxenvs: envs to pin at top.
+    :param payload: the tox envs list
+    :return: the expanded tox env list
 
+    Example:
+    -------
     envlist = py39,py38
-    envlist = {py37,py36}-django{20,21},{py37,py36}-mango{20,21},py38
+    envlist = {py37,py36}-django{20,21},{py37,py36}-mango{20,21},py38.
     """
     within_braces, values = False, []
     cur_str, brace_str = "", ""
     for char in payload:
         if char == "{":
             within_braces = True
         elif char == "}":
@@ -90,21 +119,20 @@
                 continue
         if within_braces:
             brace_str += char
         else:
             cur_str += char
     # avoid adding an empty value, caused e.g. by a trailing comma
     last_entry = cur_str.strip()
-    if last_entry != "":
+    if last_entry:
         values.append(last_entry)
     # start with higher python version
     order_env_list(values, pin_toxenvs)
     # use newline instead of comma as separator, indent values one per newline (no value on key-row)
-    result = "\n{}".format("\n".join(f"{v}" for v in values))
-    return result
+    return "\n{}".format("\n".join(f"{v}" for v in values))
 
 
 def _get_py_version(pin_toxenvs: list[str], env_list: str) -> tuple[int, int]:
     for element in env_list.split("-"):
         if element in pin_toxenvs:
             return len(element) - pin_toxenvs.index(element), 0
         match = _MATCHER.match(element)
@@ -118,57 +146,84 @@
             else:
                 main = -2
             return main, int(version) if version else 0
     return -3, 0
 
 
 def order_env_list(values: list[str], pin_toxenvs: list[str]) -> None:
+    """
+    Order environment list.
+
+    :param values: list of environments
+    :param pin_toxenvs: values to pin at top
+    """
     values.sort(key=partial(_get_py_version, pin_toxenvs), reverse=True)
 
 
 CONDITIONAL_MARKER = re.compile(r"(?P<envs>[a-zA-Z0-9, ]+):(?P<value>.*)")
 
 
 def collect_multi_line(
     value: str,
     line_split: str | None = r",| |\t",
     normalize: Callable[[dict[str, list[str]]], dict[str, list[str]]] | None = None,
     sort_key: Callable[[str], str] | None = None,
 ) -> tuple[list[str], list[str]]:
+    """
+    Collect multiline values.
+
+    :param value:
+    :param line_split:
+    :param normalize:
+    :param sort_key:
+    :return:
+    """
     groups: defaultdict[str, list[str]] = defaultdict(list)
     substitute: list[str] = []
     for line in value.strip().splitlines():
         match = CONDITIONAL_MARKER.match(line)
         if match:
             elements = match.groupdict()
             normalized_key = ", ".join(sorted(i.strip() for i in elements["envs"].split(",")))
             groups[normalized_key].append(elements["value"].strip())
         else:
             for part in re.split(line_split, line.strip()) if line_split else [line.strip()]:
                 if part:  # remove empty lines
                     if is_substitute(part):
                         substitute.append(part)
-                    else:
-                        if part not in groups[""]:  # remove duplicates
-                            groups[""].append(part)
+                    elif part not in groups[""]:  # remove duplicates
+                        groups[""].append(part)
     normalized_group = normalize(groups) if normalize else groups
     result = list(
         itertools.chain.from_iterable(
-            (f"{k}: {d}" if k != "" else d for d in sorted(v, key=sort_key))
+            (f"{k}: {d}" if k else d for d in sorted(v, key=sort_key))
             for k, v in sorted(normalized_group.items(), key=lambda i: (len(i[0].split(", ")), i[0]))
         ),
     )
     return result, substitute
 
 
 def to_py_dependencies(value: str) -> str:
+    """
+    Format to list Python dependencies.
+
+    :param value: the raw value
+    :return: the formatted value
+    """
     raw_deps, substitute = collect_multi_line(
         value,
         line_split=None,
         normalize=lambda groups: {k: requires(v) for k, v in groups.items()},
-        sort_key=lambda _: "",  # noqa: U101 # we already sorted as we wanted in normalize, keep it as is
+        sort_key=lambda _: "",  # we already sorted as we wanted in normalize, keep it as is
     )
     return fmt_list(raw_deps, substitute)
 
 
 def fmt_list(values: list[str], substitute: list[str]) -> str:
-    return "\n".join([""] + sorted(substitute) + values)
+    """
+    Format a list of values.
+
+    :param values: the raw values
+    :param substitute: substitution
+    :return: formatted list
+    """
+    return "\n".join(["", *sorted(substitute), *values])
```

### Comparing `tox_ini_fmt-1.3.0/tests/test_cli.py` & `tox_ini_fmt-1.3.1/tests/test_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from __future__ import annotations
 
 import sys
-from pathlib import Path
 from stat import S_IREAD, S_IWRITE
+from typing import TYPE_CHECKING
 
 import pytest
 
 from tox_ini_fmt.cli import cli_args
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
 def test_cli_tox_ini_ok(tmp_path: Path) -> None:
     path = tmp_path / "tox.ini"
     path.write_text("")
     result = cli_args([str(path)])
     assert result.tox_ini[0] == path
```

### Comparing `tox_ini_fmt-1.3.0/tests/test_main.py` & `tox_ini_fmt-1.3.1/tests/test_main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from __future__ import annotations
 
 import difflib
-from pathlib import Path
+from typing import TYPE_CHECKING
 
 import pytest
 
 import tox_ini_fmt.__main__
 from tox_ini_fmt.__main__ import GREEN, RED, RESET, color_diff, run
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
 def test_color_diff() -> None:
     # Arrange
     before = """
     abc
     def
     ghi
@@ -78,15 +81,15 @@
             "[tox]\nrequires =\n    tox>=4.2\n\n[testenv]\ncommands =\n    pytest --log-format='%(asctime)s'\n",
             "[tox]\nrequires =\n    tox>=4.2\n\n[testenv]\ncommands =\n    pytest --log-format='%(asctime)s'\n",
             "no change for {0}\n",
             id="no-change-testenv",
         ),
     ],
 )
-def test_main(
+def test_main(  # noqa: PLR0913
     tmp_path: Path,
     capsys: pytest.CaptureFixture[str],
     in_place: bool,
     cwd: bool,
     start: str,
     outcome: str,
     output: str,
```

### Comparing `tox_ini_fmt-1.3.0/tests/formatter/test_line_endings.py` & `tox_ini_fmt-1.3.1/tests/formatter/test_line_endings.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from __future__ import annotations
 
 import os
-from pathlib import Path
+from typing import TYPE_CHECKING
 
 import pytest
 
 from tox_ini_fmt.__main__ import run
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
 def test_platform_default(tox_ini: Path) -> None:
     """If the ini file has no newlines, the platform default may be inserted."""
 
     tox_ini.write_bytes(b"[tox]")
     run([str(tox_ini)])
     assert tox_ini.read_bytes() == f"[tox]{os.linesep}requires ={os.linesep}    tox>=4.2{os.linesep}".encode()
```

### Comparing `tox_ini_fmt-1.3.0/tests/formatter/test_requires.py` & `tox_ini_fmt-1.3.1/tests/formatter/test_requires.py`

 * *Files identical despite different names*

### Comparing `tox_ini_fmt-1.3.0/tests/formatter/test_section_order.py` & `tox_ini_fmt-1.3.1/tests/formatter/test_section_order.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
-from pathlib import Path
 from textwrap import dedent
+from typing import TYPE_CHECKING
 
 import pytest
 
 from tox_ini_fmt.cli import ToxIniFmtNamespace
 from tox_ini_fmt.formatter import format_tox_ini
 from tox_ini_fmt.formatter.section_order import explode_env_list
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
 @pytest.mark.parametrize(
     ("argument", "output"),
     [
         ("{py38,py37}-{,magic}\npy39-ok\npy37", ["py38", "py38-magic", "py37", "py37-magic", "py39-ok", "py37"]),
         ("py38\npy37", ["py38", "py37"]),
         ("py37\npy38", ["py37", "py38"]),
```

### Comparing `tox_ini_fmt-1.3.0/tests/formatter/test_test_env.py` & `tox_ini_fmt-1.3.1/tests/formatter/test_test_env.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
-from pathlib import Path
 from textwrap import dedent
+from typing import TYPE_CHECKING
 
 import pytest
 
 from tox_ini_fmt.formatter import format_tox_ini
 from tox_ini_fmt.formatter.test_env import to_ordered_list
 from tox_ini_fmt.formatter.util import to_py_dependencies
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
 def test_no_tox_section(tox_ini: Path) -> None:
     tox_ini.write_text("")
     assert format_tox_ini(tox_ini) == "[tox]\nrequires =\n    tox>=4.2\n"
 
 
 def test_format_test_env(tox_ini: Path) -> None:
@@ -127,15 +130,22 @@
             "B",
             "C",
             "\n    {[testenv:x]X}\n    {[testenv]extras}\n    B\n    C",
             id="extras",
         ),
     ],
 )
-def test_format_test_env_ref(tox_ini: Path, key: str, before: str, pre: str, post: str, expected: str) -> None:
+def test_format_test_env_ref(  # noqa: PLR0913
+    tox_ini: Path,
+    key: str,
+    before: str,
+    pre: str,
+    post: str,
+    expected: str,
+) -> None:
     text = (
         f"[testenv]\n{key}={before}\n[testenv:py]"
         f"\n{key}=\n {pre}\n {{[testenv:x]X}}\n {{[testenv]{key}}}\n {post}\n"
     )
     tox_ini.write_text(text)
     outcome = format_tox_ini(tox_ini)
     expected = f"[tox]\nrequires =\n    tox>=4.2\n\n[testenv]\n{key} ={before}\n\n[testenv:py]\n{key} ={expected}\n"
```

### Comparing `tox_ini_fmt-1.3.0/tests/formatter/test_tox_section.py` & `tox_ini_fmt-1.3.1/tests/formatter/test_tox_section.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from __future__ import annotations
 
-from pathlib import Path
 from textwrap import dedent
+from typing import TYPE_CHECKING
 
 import pytest
 
 from tox_ini_fmt.formatter import format_tox_ini
 from tox_ini_fmt.formatter.util import order_env_list
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 
 def test_no_tox_section(tox_ini: Path) -> None:
     tox_ini.write_text("")
     assert format_tox_ini(tox_ini) == "[tox]\nrequires =\n    tox>=4.2\n"
 
 
 def test_format_env_list_simple(tox_ini: Path) -> None:
@@ -113,15 +116,15 @@
 
 
 def test_format_tox_ini_handles_trailing_comma(tox_ini: Path) -> None:
     """tox.ini gets formatted without adding additional whitespace
 
     This was previously caused by a trailing comma in the `env_list`.
     """
-    tox_ini.write_text("[tox]\nenv_list=\n    py38,\n    pkg,\n" "[testenv:pkg]\na=b\n")
+    tox_ini.write_text("[tox]\nenv_list=\n    py38,\n    pkg,\n[testenv:pkg]\na=b\n")
     result = format_tox_ini(tox_ini)
     assert result == "[tox]\nrequires =\n    tox>=4.2\nenv_list =\n    py38\n    pkg\n\n[testenv:pkg]\na = b\n"
 
 
 def test_min_version_less_requires(tox_ini: Path) -> None:
     text = """
     [tox]
```

### Comparing `tox_ini_fmt-1.3.0/LICENSE.txt` & `tox_ini_fmt-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tox_ini_fmt-1.3.0/README.md` & `tox_ini_fmt-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tox_ini_fmt-1.3.0/pyproject.toml` & `tox_ini_fmt-1.3.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = [
   "hatch-vcs>=0.3",
-  "hatchling>=1.13",
+  "hatchling>=1.17.1",
 ]
 
 [project]
 name = "tox-ini-fmt"
 description = "tox is a generic virtualenv management and test command line tool"
 readme.content-type = "text/markdown"
 readme.file = "README.md"
@@ -25,35 +25,35 @@
   "Development Status :: 5 - Production/Stable",
   "Framework :: tox",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: POSIX",
-  "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries",
   "Topic :: Software Development :: Testing",
   "Topic :: Utilities",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
-  "packaging>=23",
+  "packaging>=23.1",
 ]
 optional-dependencies.test = [
   "covdefaults>=2.3",
-  "pytest>=7.2.2",
-  "pytest-cov>=4",
+  "pytest>=7.3.2",
+  "pytest-cov>=4.1",
 ]
 urls.Documentation = "https://tox.wiki"
 urls.Homepage = "https://github.com/tox-dev/tox-ini-fmt/blob/main/README.md#tox-ini-fmt"
 urls."Release Notes" = "https://github.com/tox-dev/tox-ini-fmt/blob/main/CHANGELOG.md"
 urls.Source = "https://github.com/tox-dev/tox-ini-fmt"
 urls.Tracker = "https://github.com/tox-dev/tox-ini-fmt/issues"
 scripts.tox-ini-fmt = "tox_ini_fmt.__main__:run"
@@ -63,26 +63,35 @@
 build.hooks.vcs.version-file = "src/tox_ini_fmt/version.py"
 build.targets.sdist.include = ["/src", "/tests", "/tox.ini"]
 version.source = "vcs"
 
 [tool.black]
 line-length = 120
 
-[tool.isort]
-known_first_party = ["tox", "tests"]
-profile = "black"
-line_length = 120
-add_imports = ["from __future__ import annotations"]
-
-[tool.flake8]
-max-complexity = 22
-max-line-length = 120
-unused-arguments-ignore-abstract-functions = true
-noqa-require-code = true
-dictionaries = ["en_US", "python", "technical", "django"]
+[tool.ruff]
+select = ["ALL"]
+line-length = 120
+target-version = "py37"
+isort = {known-first-party = ["tox_ini_fmt"], required-imports = ["from __future__ import annotations"]}
+ignore = [
+  "ANN101",  # no typoe annotation for self
+  "ANN401",  # allow Any as type annotation
+  "D203",  # `one-blank-line-before-class` (D203) and `no-blank-line-before-class` (D211) are incompatible
+  "D212",  # `multi-line-summary-first-line` (D212) and `multi-line-summary-second-line` (D213) are incompatible
+  "S104",  # Possible binding to all interface
+]
+[tool.ruff.per-file-ignores]
+"tests/**/*.py" = [
+  "S101",  # asserts allowed in tests...
+  "FBT",  # don"t care about booleans as positional arguments in tests
+  "INP001", # no implicit namespace
+  "D",  # don"t care about documentation in tests
+  "S603",  # `subprocess` call: check for execution of untrusted input
+  "PLR2004",  # Magic value used in comparison, consider replacing with a constant variable
+]
 
 [tool.coverage]
 html.show_contexts = true
 html.skip_covered = false
 paths.source = [
   "src",
   ".tox*/*/lib/python*/site-packages",
```

### Comparing `tox_ini_fmt-1.3.0/PKG-INFO` & `tox_ini_fmt-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox-ini-fmt
-Version: 1.3.0
+Version: 1.3.1
 Summary: tox is a generic virtualenv management and test command line tool
 Project-URL: Documentation, https://tox.wiki
 Project-URL: Homepage, https://github.com/tox-dev/tox-ini-fmt/blob/main/README.md#tox-ini-fmt
 Project-URL: Release Notes, https://github.com/tox-dev/tox-ini-fmt/blob/main/CHANGELOG.md
 Project-URL: Source, https://github.com/tox-dev/tox-ini-fmt
 Project-URL: Tracker, https://github.com/tox-dev/tox-ini-fmt/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>
@@ -14,30 +14,30 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: tox
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
-Requires-Dist: packaging>=23
+Requires-Dist: packaging>=23.1
 Provides-Extra: test
 Requires-Dist: covdefaults>=2.3; extra == 'test'
-Requires-Dist: pytest-cov>=4; extra == 'test'
-Requires-Dist: pytest>=7.2.2; extra == 'test'
+Requires-Dist: pytest-cov>=4.1; extra == 'test'
+Requires-Dist: pytest>=7.3.2; extra == 'test'
 Description-Content-Type: text/markdown
 
 # tox-ini-fmt
 
 [![PyPI](https://img.shields.io/pypi/v/tox-ini-fmt?style=flat-square)](https://pypi.org/project/tox-ini-fmt)
 [![PyPI - Implementation](https://img.shields.io/pypi/implementation/tox-ini-fmt?style=flat-square)](https://pypi.org/project/tox-ini-fmt)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tox-ini-fmt?style=flat-square)](https://pypi.org/project/tox-ini-fmt)
```

