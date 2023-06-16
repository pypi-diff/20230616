# Comparing `tmp/bump_deps_index-1.4.2.tar.gz` & `tmp/bump_deps_index-1.4.3.tar.gz`

## Comparing `bump_deps_index-1.4.2.tar` & `bump_deps_index-1.4.3.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/.readthedocs.yml
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/tox.ini
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/whitelist.txt
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/.github/CODEOWNERS
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/.github/dependabot.yml
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/.github/workflows/check.yml
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/.github/workflows/release.yml
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/docs/changelog.rst
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/docs/cli.rst
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/docs/conf.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/docs/index.rst
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/docs/py_api.rst
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/src/bump_deps_index/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/src/bump_deps_index/__main__.py
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/src/bump_deps_index/_cli.py
--rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/src/bump_deps_index/_run.py
--rw-r--r--   0        0        0     4487 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/src/bump_deps_index/_spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/src/bump_deps_index/py.typed
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/src/bump_deps_index/version.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/tests/test_cli.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/tests/test_main.py
--rw-r--r--   0        0        0     8684 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/tests/test_run.py
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/tests/test_spec.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/tests/test_version.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/LICENSE
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/README.md
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     3808 2020-02-02 00:00:00.000000 bump_deps_index-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/.readthedocs.yml
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/tox.ini
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/.github/CODEOWNERS
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/.github/dependabot.yml
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/.github/workflows/check.yml
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/docs/changelog.rst
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/docs/cli.rst
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/docs/conf.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/docs/index.rst
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/docs/py_api.rst
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/src/bump_deps_index/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/src/bump_deps_index/__main__.py
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/src/bump_deps_index/_cli.py
+-rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/src/bump_deps_index/_run.py
+-rw-r--r--   0        0        0     4619 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/src/bump_deps_index/_spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/src/bump_deps_index/py.typed
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/src/bump_deps_index/version.py
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/tests/test_cli.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/tests/test_main.py
+-rw-r--r--   0        0        0     8711 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/tests/test_run.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/tests/test_spec.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/tests/test_version.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/LICENSE
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/README.md
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 bump_deps_index-1.4.3/PKG-INFO
```

### Comparing `bump_deps_index-1.4.2/tox.ini` & `bump_deps_index-1.4.3/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
       --cov-report html:{envtmpdir}{/}htmlcov --cov-report xml:{toxworkdir}{/}coverage.{envname}.xml \
       tests}
 
 [testenv:fix]
 description = run static analysis and style check using flake8
 skip_install = true
 deps =
-    pre-commit>=3.3.1
+    pre-commit>=3.3.3
 pass_env =
     HOMEPATH
     PROGRAMDATA
 commands =
     pre-commit run --all-files --show-diff-on-failure
 
 [testenv:docs]
@@ -44,16 +44,16 @@
     python -c 'import glob; import subprocess; subprocess.call(["proselint"] + glob.glob("docs/*.rst"))'
     sphinx-build -d "{envtmpdir}/doctree" docs "{toxworkdir}/docs_out" --color -b html {posargs}
     python -c 'import pathlib; print("documentation available under \{0\}".format((pathlib.Path(r"{toxworkdir}") / "docs_out" / "index.html").as_uri()))'
 
 [testenv:type]
 description = run type check on code base
 deps =
-    mypy==1.2
-    types-PyYaml>=6.0.12.9
+    mypy==1.3
+    types-PyYaml>=6.0.12.10
 set_env =
     {tty:MYPY_FORCE_COLOR = 1}
 commands =
     mypy --strict src
     mypy --strict tests
 
 [testenv:readme]
```

### Comparing `bump_deps_index-1.4.2/.github/workflows/check.yml` & `bump_deps_index-1.4.3/.github/workflows/check.yml`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,19 @@
   test:
     name: test ${{ matrix.py }} - ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         py:
-          - "3.12.0-alpha.7"
+          - "3.12.0-beta.2"
           - "3.11"
           - "3.10"
         os:
-          - ubuntu-22.04
+          - ubuntu-latest
 
     steps:
       - name: Setup python for tox
         uses: actions/setup-python@v4
         with:
           python-version: "3.11"
       - name: Install tox
@@ -56,15 +56,15 @@
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
           - docs
           - readme
     steps:
       - uses: actions/checkout@v3
```

### Comparing `bump_deps_index-1.4.2/.github/workflows/release.yml` & `bump_deps_index-1.4.3/.github/workflows/release.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 name: Release to PyPI
 on:
   push:
     tags: ["*"]
 
 jobs:
   release:
-    runs-on: ubuntu-22.04
+    runs-on: ubuntu-latest
     environment:
       name: release
       url: https://pypi.org/p/bump-deps-index
     permissions:
       id-token: write
     steps:
       - name: Setup python to build package
```

### Comparing `bump_deps_index-1.4.2/docs/changelog.rst` & `bump_deps_index-1.4.3/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.2/docs/conf.py` & `bump_deps_index-1.4.3/docs/conf.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,32 @@
+"""Documentation generation configuration."""  # noqa: INP001
 from __future__ import annotations
 
-from datetime import datetime
+from datetime import datetime, timezone
 
 import bump_deps_index
 from bump_deps_index import __version__
 
 project = name = "bumps-deps-index"
-copyright = f"2022-{datetime.today().year}"
+now = datetime.now(tz=timezone.utc)
+copyright = f"2022-{now.year}"  # noqa: A001
 version, release = __version__, __version__.split("+")[0]
 
 extensions = [
     "sphinx.ext.autosectionlabel",
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.inheritance_diagram",
     "sphinx_argparse_cli",
 ]
 
 master_doc, source_suffix = "index", ".rst"
 
 html_theme = "furo"
-html_title, html_last_updated_fmt = "Bump PyPI deps from index", datetime.now().isoformat()
+html_title, html_last_updated_fmt = "Bump PyPI deps from index", now.isoformat()
 pygments_style, pygments_dark_style = "sphinx", "monokai"
 
 autoclass_content, autodoc_typehints, autodoc_typehints_format = "both", "description", "short"
 inheritance_alias, inheritance_graph_attrs = {}, {"rankdir": "TB"}
 autodoc_default_options = {"members": True, "member-order": "bysource", "undoc-members": True, "show-inheritance": True}
 
 intersphinx_mapping = {"python": ("https://docs.python.org/3.10", None)}
```

### Comparing `bump_deps_index-1.4.2/src/bump_deps_index/_cli.py` & `bump_deps_index-1.4.3/src/bump_deps_index/_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 import os
 from argparse import ArgumentParser, Namespace, RawDescriptionHelpFormatter
-from collections.abc import Sequence
 from pathlib import Path
-from typing import Literal
+from typing import TYPE_CHECKING, Literal
 
 from bump_deps_index.version import version
 
+if TYPE_CHECKING:
+    from collections.abc import Sequence
+
 
 class Options(Namespace):
     """Run options."""
 
     index_url: str
     """The PyPI Index URL to query for Python versions."""
     npm_registry: str
```

### Comparing `bump_deps_index-1.4.2/src/bump_deps_index/_run.py` & `bump_deps_index-1.4.3/src/bump_deps_index/_run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from __future__ import annotations
 
 import sys
-from collections.abc import Callable, Iterable, Iterator, Mapping, Sequence
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from configparser import RawConfigParser
-from pathlib import Path
-from typing import cast
+from typing import TYPE_CHECKING, cast
 
-from yaml import Loader
-from yaml import load as load_yaml
+from yaml import safe_load as load_yaml
 
-from ._cli import Options
 from ._spec import PkgType
 from ._spec import update as update_spec
 
+if TYPE_CHECKING:
+    from collections.abc import Callable, Iterable, Iterator, Mapping, Sequence
+    from pathlib import Path
+
+    from ._cli import Options
+
 if sys.version_info >= (3, 11):  # pragma: no cover (py311+)
     from tomllib import load as load_toml
 else:  # pragma: no cover (py311+)
     from tomli import load as load_toml
 
 
 def run(opt: Options) -> None:
@@ -37,15 +39,16 @@
             ".pre-commit-config.yaml": load_from_pre_commit,
             "tox.ini": load_from_tox_ini,
             "setup.cfg": load_from_setup_cfg,
         }
         for filename in opt.filenames:
             is_req_txt = filename.suffix == ".txt"
             if filename.name not in mapping and not is_req_txt:
-                raise NotImplementedError(f"we do not support {filename}")
+                msg = f"we do not support {filename}"  # pragma: no cover
+                raise NotImplementedError(msg)  # pragma: no cover
             loader = mapping.get(filename.name, load_from_requirements_txt)
             pre_release = {"yes": True, "no": False, "file-default": None}[opt.pre_release]
             specs = {(i.strip(), t, p): None for i, t, p in loader(filename, pre_release) if i.strip()}
             changes = calculate_update(opt.index_url, opt.npm_registry, list(specs))
             update_file(filename, changes)
 
 
@@ -61,15 +64,17 @@
     yield from _generate(cfg.get("project", {}).get("dependencies", []), pkg_type=PkgType.PYTHON)
     pre = False if pre_release is None else pre_release
     for entries in cfg.get("project", {}).get("optional-dependencies", {}).values():
         yield from _generate(entries, pkg_type=PkgType.PYTHON, pre_release=pre)
 
 
 def _generate(
-    generator: Iterable[str], pkg_type: PkgType, pre_release: bool = False
+    generator: Iterable[str],
+    pkg_type: PkgType,
+    pre_release: bool = False,  # noqa: FBT001, FBT002
 ) -> Iterator[tuple[str, PkgType, bool]]:
     for value in generator:
         yield value, pkg_type, pre_release
 
 
 def load_from_tox_ini(filename: Path, pre_release: bool | None) -> Iterator[tuple[str, PkgType, bool]]:
     cfg = NoTransformConfigParser()
@@ -79,15 +84,15 @@
         if section.startswith("testenv"):
             values = cast(list[str], cfg[section].get("deps", "").split("\n"))
             yield from _generate(values, pkg_type=PkgType.PYTHON, pre_release=pre)
 
 
 def load_from_pre_commit(filename: Path, pre_release: bool | None) -> Iterator[tuple[str, PkgType, bool]]:
     with filename.open("rt") as file_handler:
-        cfg = load_yaml(file_handler, Loader)
+        cfg = load_yaml(file_handler)
     pre = True if pre_release is None else pre_release
     for repo in cfg.get("repos", []) if isinstance(cfg, dict) else []:
         for hook in repo["hooks"]:
             for pkg in hook.get("additional_dependencies", []):
                 yield pkg, PkgType.JS if "@" in pkg else PkgType.PYTHON, pre
 
 
@@ -100,44 +105,46 @@
     if cfg.has_section("options.extras_require"):
         for group in cfg["options.extras_require"].values():
             yield from _generate(group.split("\n"), pkg_type=PkgType.PYTHON, pre_release=pre)
 
 
 class NoTransformConfigParser(RawConfigParser):
     def optionxform(self, s: str) -> str:
-        """disable default lower-casing"""
+        """Disable default lower-casing."""
         return s
 
 
 def update_file(filename: Path, changes: Mapping[str, str]) -> None:
     text = filename.read_text()
     for src, dst in changes.items():
         text = text.replace(src, dst)
     filename.write_text(text)
 
 
 def calculate_update(
-    index_url: str, npm_registry: str, specs: Sequence[tuple[str, PkgType, bool]]
+    index_url: str,
+    npm_registry: str,
+    specs: Sequence[tuple[str, PkgType, bool]],
 ) -> Mapping[str, str]:
     changes: dict[str, str] = {}
     if specs:
         with ThreadPoolExecutor(max_workers=min(len(specs), 10)) as executor:
             # Start the load operations and mark each future with its URL
             future_to_url = {
                 executor.submit(update_spec, index_url, npm_registry, pkg, pkg_type, pre_release): pkg
                 for pkg, pkg_type, pre_release in specs
             }
             for future in as_completed(future_to_url):
                 spec = future_to_url[future]
                 try:
                     res = future.result()
-                except Exception as exc:
-                    print(f"failed {spec} with {exc!r}", file=sys.stderr)
+                except Exception as exc:  # noqa: BLE001
+                    print(f"failed {spec} with {exc!r}", file=sys.stderr)  # noqa: T201
                 else:
                     changes[spec] = res
-                    print(f"{spec}{f' -> {res}' if res != spec else ''}")
+                    print(f"{spec}{f' -> {res}' if res != spec else ''}")  # noqa: T201
     return changes
 
 
 __all__ = [
     "run",
 ]
```

### Comparing `bump_deps_index-1.4.2/src/bump_deps_index/_spec.py` & `bump_deps_index-1.4.3/src/bump_deps_index/_spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,71 +13,71 @@
 
 
 class PkgType(Enum):
     PYTHON = auto()
     JS = auto()
 
 
-def update(index_url: str, npm_registry: str, spec: str, pkg_type: PkgType, pre_release: bool) -> str:
+def update(index_url: str, npm_registry: str, spec: str, pkg_type: PkgType, pre_release: bool) -> str:  # noqa: FBT001
     if pkg_type is PkgType.PYTHON:
         with _py_lock:
             print_index("Python", index_url)
         return update_python(index_url, spec, pre_release)
-    else:
-        with _js_lock:
-            print_index("JavaScript", npm_registry)
-        return update_js(npm_registry, spec, pre_release)
+    with _js_lock:
+        print_index("JavaScript", npm_registry)
+    return update_js(npm_registry, spec, pre_release)
 
 
 _py_lock, _js_lock = Lock(), Lock()
 
 
 @cache
 def print_index(of_type: str, registry: str) -> None:
-    print(f"Using {of_type} index: {registry}")
+    print(f"Using {of_type} index: {registry}")  # noqa: T201
 
 
-def update_js(npm_registry: str, spec: str, pre_release: bool) -> str:
+def update_js(npm_registry: str, spec: str, pre_release: bool) -> str:  # noqa: FBT001
     ver_at = spec.rfind("@")
     package = spec[: len(spec) if ver_at == -1 else ver_at]
     version = get_js_pkgs(npm_registry, package, pre_release)[0]
     ver = str(version)
     while ver.endswith(".0"):
         ver = ver[:-2]
     return f"{package}@{ver}"
 
 
-def get_js_pkgs(npm_registry: str, package: str, pre_release: bool) -> list[str]:
-    with urlopen(f"{npm_registry}/{package}") as handler:
+def get_js_pkgs(npm_registry: str, package: str, pre_release: bool) -> list[str]:  # noqa: FBT001
+    with urlopen(f"{npm_registry}/{package}") as handler:  # noqa: S310
         text = handler.read().decode("utf-8")
     info = json.loads(text)
     return sorted(
         (
             v[1]
-            for v in ((Version(i), i) for i in info["versions"].keys())
+            for v in ((Version(i), i) for i in info["versions"])
             if (True if pre_release else not v[0].is_prerelease)
         ),
         reverse=True,
     )
 
 
-def update_python(index_url: str, spec: str, pre_release: bool) -> str:
+def update_python(index_url: str, spec: str, pre_release: bool) -> str:  # noqa: FBT001
     req = Requirement(spec)
     eq = any(s for s in req.specifier if s.operator == "==")
     for version in get_pkgs(index_url, req.name, pre_release):
         if eq or all(s.contains(str(version)) for s in req.specifier):
             break
     else:
         return spec
     ver = str(version)
     ver = ver.split("+")[0]  # strip build numbers
     while ver.endswith(".0"):
         ver = ver[:-2]
     c_ver = next(
-        (s.version for s in req.specifier if (s.operator == ">=" and not eq) or (eq and s.operator == "==")), None
+        (s.version for s in req.specifier if (s.operator == ">=" and not eq) or (eq and s.operator == "==")),
+        None,
     )
     if c_ver is None:
         new_ver = req.name
         if req.extras:
             new_ver = f"{new_ver}[{', '.join(req.extras)}]"
         new_ver = f"{new_ver}{',' if req.specifier else ''}>={ver}"
         if req.marker:
@@ -95,34 +95,35 @@
         self._at_tag: deque[str] = deque()
         self._files: list[str] = []
 
     @property
     def files(self) -> frozenset[str]:
         return frozenset(self._files)
 
-    def handle_starttag(self, tag: str, attrs: list[tuple[str, str | None]]) -> None:  # noqa: U100
+    def handle_starttag(self, tag: str, attrs: list[tuple[str, str | None]]) -> None:  # noqa: ARG002
         self._at_tag.append(tag)
 
     def handle_endtag(self, tag: str) -> None:
         if self._at_tag and self._at_tag[-1] == tag:  # pragma: no branch
             self._at_tag.pop()
 
     def handle_data(self, data: str) -> None:
         if self._at_tag and self._at_tag[-1] == "a" and data.strip():
             self._files.append(data.strip())
 
 
-def get_pkgs(index_url: str, package: str, pre_release: bool) -> list[Version]:
-    with urlopen(f"{index_url}/{package}") as handler:
+def get_pkgs(index_url: str, package: str, pre_release: bool) -> list[Version]:  # noqa: FBT001
+    with urlopen(f"{index_url}/{package}") as handler:  # noqa: S310
         text = handler.read().decode("utf-8")
 
     versions: set[Version] = set()
     parser = IndexParser()
     parser.feed(text)
-    for file in parser.files:
+    for raw_file in parser.files:
+        file = raw_file
         if file.endswith(".tar.bz2"):
             file = file[:-8]
         if file.endswith(".tar.gz"):
             file = file[:-7]
         if file.endswith(".whl"):
             file = file[:-4]
         if file.endswith(".zip"):
```

### Comparing `bump_deps_index-1.4.2/tests/test_cli.py` & `bump_deps_index-1.4.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.2/tests/test_main.py` & `bump_deps_index-1.4.3/tests/test_main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from __future__ import annotations
 
 import sys
 from pathlib import Path
 from subprocess import check_call
-
-import pytest
-from pytest_mock import MockerFixture
+from typing import TYPE_CHECKING
 
 from bump_deps_index import Options, main
 
+if TYPE_CHECKING:
+    import pytest
+    from pytest_mock import MockerFixture
+
 
 def test_main(capfd: pytest.CaptureFixture[str]) -> None:
     check_call([sys.executable, "-m", "bump_deps_index", "-h"])
     out, err = capfd.readouterr()
     assert out
     assert not err
```

### Comparing `bump_deps_index-1.4.2/tests/test_run.py` & `bump_deps_index-1.4.3/tests/test_run.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 from __future__ import annotations
 
-from pathlib import Path
 from textwrap import dedent
-
-import pytest
-from pytest_mock import MockerFixture
+from typing import TYPE_CHECKING
 
 from bump_deps_index import Options, run
 from bump_deps_index._spec import PkgType
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
+    import pytest
+    from pytest_mock import MockerFixture
+
 
 def test_run_args(capsys: pytest.CaptureFixture[str], mocker: MockerFixture) -> None:
     mapping = {"A": "A>=1", "B": "B"}
     update_spec = mocker.patch(
-        "bump_deps_index._run.update_spec", side_effect=lambda _, __, spec, ___, ____: mapping[spec]  # noqa: U101
+        "bump_deps_index._run.update_spec",
+        side_effect=lambda _, __, spec, ___, ____: mapping[spec],
     )
 
     run(
         Options(
             index_url="https://pypi.org/simple",
             npm_registry="N",
             pkgs=[" A ", "B", "C"],
             filenames=None,
             pre_release=False,
-        )
+        ),
     )
 
     out, err = capsys.readouterr()
     assert err == "failed C with KeyError('C')\n"
     assert set(out.splitlines()) == {"A -> A>=1", "B"}
 
     found = set()
@@ -40,15 +44,16 @@
         assert not called.kwargs
     assert found == {("C", PkgType.PYTHON), ("B", PkgType.PYTHON), ("A", PkgType.PYTHON)}
 
 
 def test_run_pyproject_toml(capsys: pytest.CaptureFixture[str], mocker: MockerFixture, tmp_path: Path) -> None:
     mapping = {"A": "A>=1", "B==2": "B==1", "C": "C>=1"}
     mocker.patch(
-        "bump_deps_index._run.update_spec", side_effect=lambda _, __, spec, ___, ____: mapping[spec]  # noqa: U101
+        "bump_deps_index._run.update_spec",
+        side_effect=lambda _, __, spec, ___, ____: mapping[spec],
     )
     dest = tmp_path / "pyproject.toml"
     toml = """
     [build-system]
     requires = ["A"]
     [project]
     dependencies = [ "B==2"]
@@ -77,21 +82,22 @@
     dest = tmp_path / "tox.ini"
     dest.write_text("")
     run(Options(index_url="https://pypi.org/simple", npm_registry="", pkgs=[], filenames=[dest], pre_release="no"))
 
     out, err = capsys.readouterr()
     assert not err
     assert not set(out.splitlines())
-    assert dest.read_text() == ""
+    assert not dest.read_text()
 
 
 def test_run_tox_ini(capsys: pytest.CaptureFixture[str], mocker: MockerFixture, tmp_path: Path) -> None:
     mapping = {"A": "A>=1", "B==2": "B==1"}
     mocker.patch(
-        "bump_deps_index._run.update_spec", side_effect=lambda _, __, spec, ___, ____: mapping[spec]  # noqa: U101
+        "bump_deps_index._run.update_spec",
+        side_effect=lambda _, __, spec, ___, ____: mapping[spec],
     )
     dest = tmp_path / "tox.ini"
     tox_ini = """
     [testenv]
     deps =
         A
     [testenv:ok]
@@ -124,21 +130,22 @@
     dest = tmp_path / "tox.ini"
     dest.write_text("")
     run(Options(index_url="https://pypi.org/simple", npm_registry="", pkgs=[], filenames=[dest], pre_release="no"))
 
     out, err = capsys.readouterr()
     assert not err
     assert not set(out.splitlines())
-    assert dest.read_text() == ""
+    assert not dest.read_text()
 
 
 def test_run_setup_cfg(capsys: pytest.CaptureFixture[str], mocker: MockerFixture, tmp_path: Path) -> None:
     mapping = {"A": "A>=1", "B": "B==1", "C": "C>=3"}
     mocker.patch(
-        "bump_deps_index._run.update_spec", side_effect=lambda _, __, spec, ___, ____: mapping[spec]  # noqa: U101
+        "bump_deps_index._run.update_spec",
+        side_effect=lambda _, __, spec, ___, ____: mapping[spec],
     )
     dest = tmp_path / "setup.cfg"
     setup_cfg = """
     [options]
     install_requires =
         A
     [options.extras_require]
@@ -171,25 +178,26 @@
     dest = tmp_path / "setup.cfg"
     dest.write_text("")
     run(Options(index_url="https://pypi.org/simple", npm_registry="", pkgs=[], filenames=[dest], pre_release="no"))
 
     out, err = capsys.readouterr()
     assert not err
     assert not set(out.splitlines())
-    assert dest.read_text() == ""
+    assert not dest.read_text()
 
 
 def test_run_pre_commit(capsys: pytest.CaptureFixture[str], mocker: MockerFixture, tmp_path: Path) -> None:
     mapping = {
         "flake8-bugbear==22.7.1": "flake8-bugbear==22.7.2",
         "black==22.6.0": "black==22.6",
         "prettier@2.7.0": "prettier@2.8",
     }
     mocker.patch(
-        "bump_deps_index._run.update_spec", side_effect=lambda _, __, spec, ___, ____: mapping[spec]  # noqa: U101
+        "bump_deps_index._run.update_spec",
+        side_effect=lambda _, __, spec, ___, ____: mapping[spec],
     )
     dest = tmp_path / ".pre-commit-config.yaml"
     setup_cfg = """
     repos:
       - repo: https://github.com/asottile/blacken-docs
         hooks:
           - id: blacken-docs
@@ -234,30 +242,31 @@
     dest = tmp_path / ".pre-commit-config.yaml"
     dest.write_text("")
     run(Options(index_url="https://pypi.org/simple", npm_registry="", pkgs=[], filenames=[dest], pre_release="no"))
 
     out, err = capsys.readouterr()
     assert not err
     assert not set(out.splitlines())
-    assert dest.read_text() == ""
+    assert not dest.read_text()
 
 
 def test_run_args_empty(capsys: pytest.CaptureFixture[str], mocker: MockerFixture) -> None:
     mocker.patch("bump_deps_index._run.update_spec", side_effect=ValueError)
     run(Options(index_url="https://pypi.org/simple", pkgs=[], filenames=[], pre_release="no"))
 
     out, err = capsys.readouterr()
     assert not err
     assert not out
 
 
 def test_run_requirements_txt(capsys: pytest.CaptureFixture[str], mocker: MockerFixture, tmp_path: Path) -> None:
     mapping = {"A": "A>=1", "B==1": "B==2"}
     mocker.patch(
-        "bump_deps_index._run.update_spec", side_effect=lambda _, __, spec, ___, ____: mapping[spec]  # noqa: U101
+        "bump_deps_index._run.update_spec",
+        side_effect=lambda _, __, spec, ___, ____: mapping[spec],
     )
     dest = tmp_path / "requirements.txt"
     req_txt = """
     A
     B==1
     """
     dest.write_text(dedent(req_txt).lstrip())
```

### Comparing `bump_deps_index-1.4.2/tests/test_spec.py` & `bump_deps_index-1.4.3/tests/test_spec.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from __future__ import annotations
 
-from collections.abc import Iterator
 from contextlib import contextmanager
 from io import BytesIO
+from typing import TYPE_CHECKING
 
 import pytest
 from packaging.version import Version
-from pytest_mock import MockerFixture
 
 from bump_deps_index._spec import PkgType, get_js_pkgs, get_pkgs, update
 
+if TYPE_CHECKING:
+    from collections.abc import Iterator
+
+    from pytest_mock import MockerFixture
+
 
 def test_get_pkgs(mocker: MockerFixture, capsys: pytest.CaptureFixture[str]) -> None:
     @contextmanager
     def _read_url(url: str) -> Iterator[BytesIO]:
         assert url == "I/A-B"
         yield BytesIO(raw_html.encode("utf-8"))
 
@@ -78,16 +82,21 @@
             "A>=1.1",
             id="ignore-build-marker",
         ),
         pytest.param("A@1", PkgType.JS, False, [Version("2.0")], "A@2", id="js-ver"),
         pytest.param("A", PkgType.JS, False, [Version("2.0")], "A@2", id="js-bare"),
     ],
 )
-def test_update(
-    mocker: MockerFixture, spec: str, pkg_type: PkgType, pre_release: bool, versions: list[Version], result: str
+def test_update(  # noqa: PLR0913
+    mocker: MockerFixture,
+    spec: str,
+    pkg_type: PkgType,
+    pre_release: bool,
+    versions: list[Version],
+    result: str,
 ) -> None:
     if pkg_type is PkgType.PYTHON:
         mocker.patch("bump_deps_index._spec.get_pkgs", return_value=versions)
     else:
         mocker.patch("bump_deps_index._spec.get_js_pkgs", return_value=versions)
     res = update("I", "N", spec, pkg_type, pre_release)
     assert res == result
```

### Comparing `bump_deps_index-1.4.2/LICENSE` & `bump_deps_index-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.2/README.md` & `bump_deps_index-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `bump_deps_index-1.4.2/pyproject.toml` & `bump_deps_index-1.4.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = [
   "hatch-vcs>=0.3",
-  "hatchling>=1.14.1",
+  "hatchling>=1.18",
 ]
 
 [project]
 name = "bump-deps-index"
 description = "Bump your dependencies to latest available from index."
 readme = "README.md"
 keywords = [
@@ -38,24 +38,24 @@
 ]
 dependencies = [
   "packaging>=23.1",
   "pyyaml>=6",
   'tomli>=2.0.1; python_version < "3.11"',
 ]
 optional-dependencies.docs = [
-  "furo>=2023.3.27",
+  "furo>=2023.5.20",
   "proselint>=0.13",
-  "sphinx>=6.2.1",
+  "sphinx>=7.0.1",
   "sphinx-argparse-cli>=1.11",
 ]
 optional-dependencies.test = [
   "covdefaults>=2.3",
-  "pytest>=7.3.1",
-  "pytest-cov>=4",
-  "pytest-mock>=3.10",
+  "pytest>=7.3.2",
+  "pytest-cov>=4.1",
+  "pytest-mock>=3.11",
 ]
 urls.Documentation = "https://bump-deps-index.readthedocs.io"
 urls.Homepage = "https://github.com/gaborbernat/bump-deps-index"
 urls.Source = "https://github.com/gaborbernat/bump-deps-index"
 urls.Tracker = "https://github.com/gaborbernat/bump-deps-index/issues"
 [project.entry-points.console_scripts]
 bump-deps-index = "bump_deps_index.__main__:main"
@@ -63,26 +63,35 @@
 [tool.hatch]
 build.hooks.vcs.version-file = "src/bump_deps_index/version.py"
 version.source = "vcs"
 
 [tool.black]
 line-length = 120
 
-[tool.isort]
-profile = "black"
-known_first_party = ["bumps_deps_index"]
-
-[tool.flake8]
-max-complexity = 22
-max-line-length = 120
-noqa-require-code = true
-ignore =  [
-  "E203", # whitespace before ':'
+[tool.ruff]
+select = ["ALL"]
+line-length = 120
+target-version = "py310"
+isort = {known-first-party = ["bump_deps_index"], required-imports = ["from __future__ import annotations"]}
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
 ]
-dictionaries = ["en_US", "python", "technical", "django"]
 
 [tool.coverage]
 run.dynamic_context = "test_function"
 run.plugins = ["covdefaults"]
 run.parallel = true
 report.fail_under = 100
 html.show_contexts = true
```

### Comparing `bump_deps_index-1.4.2/PKG-INFO` & `bump_deps_index-1.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bump-deps-index
-Version: 1.4.2
+Version: 1.4.3
 Summary: Bump your dependencies to latest available from index.
 Project-URL: Documentation, https://bump-deps-index.readthedocs.io
 Project-URL: Homepage, https://github.com/gaborbernat/bump-deps-index
 Project-URL: Source, https://github.com/gaborbernat/bump-deps-index
 Project-URL: Tracker, https://github.com/gaborbernat/bump-deps-index/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>
 License: MIT License
@@ -42,23 +42,23 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Requires-Dist: packaging>=23.1
 Requires-Dist: pyyaml>=6
 Requires-Dist: tomli>=2.0.1; python_version < '3.11'
 Provides-Extra: docs
-Requires-Dist: furo>=2023.3.27; extra == 'docs'
+Requires-Dist: furo>=2023.5.20; extra == 'docs'
 Requires-Dist: proselint>=0.13; extra == 'docs'
 Requires-Dist: sphinx-argparse-cli>=1.11; extra == 'docs'
-Requires-Dist: sphinx>=6.2.1; extra == 'docs'
+Requires-Dist: sphinx>=7.0.1; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: covdefaults>=2.3; extra == 'test'
-Requires-Dist: pytest-cov>=4; extra == 'test'
-Requires-Dist: pytest-mock>=3.10; extra == 'test'
-Requires-Dist: pytest>=7.3.1; extra == 'test'
+Requires-Dist: pytest-cov>=4.1; extra == 'test'
+Requires-Dist: pytest-mock>=3.11; extra == 'test'
+Requires-Dist: pytest>=7.3.2; extra == 'test'
 Description-Content-Type: text/markdown
 
 # bump-deps-index
 
 [![PyPI](https://img.shields.io/pypi/v/bump-deps-index?style=flat-square)](https://pypi.org/project/bump-deps-index/)
 [![Supported Python
 versions](https://img.shields.io/pypi/pyversions/bump-deps-index.svg)](https://pypi.org/project/bump-deps-index/)
```

