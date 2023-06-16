# Comparing `tmp/craft-cli-1.2.0.tar.gz` & `tmp/craft-cli-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft-cli-1.2.0.tar", last modified: Mon Aug  8 12:30:29 2022, max compression
+gzip compressed data, was "craft-cli-2.0.0.tar", last modified: Fri Jun 16 18:37:43 2023, max compression
```

## Comparing `craft-cli-1.2.0.tar` & `craft-cli-2.0.0.tar`

### file list

```diff
@@ -1,24 +1,89 @@
-drwxrwxr-x   0 facundo   (1000) facundo   (1000)        0 2022-08-08 12:30:29.452455 craft-cli-1.2.0/
--rw-rw-r--   0 facundo   (1000) facundo   (1000)     7652 2021-11-10 16:17:03.000000 craft-cli-1.2.0/LICENSE
--rw-rw-r--   0 facundo   (1000) facundo   (1000)       34 2022-01-25 18:16:20.000000 craft-cli-1.2.0/MANIFEST.in
--rw-rw-r--   0 facundo   (1000) facundo   (1000)     2952 2022-08-08 12:30:29.456455 craft-cli-1.2.0/PKG-INFO
--rw-rw-r--   0 facundo   (1000) facundo   (1000)     1266 2022-02-25 14:58:57.000000 craft-cli-1.2.0/README.md
-drwxrwxr-x   0 facundo   (1000) facundo   (1000)        0 2022-08-08 12:30:29.452455 craft-cli-1.2.0/craft_cli/
--rw-rw-r--   0 facundo   (1000) facundo   (1000)     1420 2022-08-08 12:30:23.000000 craft-cli-1.2.0/craft_cli/__init__.py
--rw-rw-r--   0 facundo   (1000) facundo   (1000)    18761 2022-08-04 15:13:36.000000 craft-cli-1.2.0/craft_cli/dispatcher.py
--rw-rw-r--   0 facundo   (1000) facundo   (1000)     3076 2022-06-20 17:38:33.000000 craft-cli-1.2.0/craft_cli/errors.py
--rw-rw-r--   0 facundo   (1000) facundo   (1000)    14578 2022-08-05 17:26:33.000000 craft-cli-1.2.0/craft_cli/helptexts.py
--rw-rw-r--   0 facundo   (1000) facundo   (1000)    37992 2022-08-08 12:01:33.000000 craft-cli-1.2.0/craft_cli/messages.py
--rw-rw-r--   0 facundo   (1000) facundo   (1000)        0 2021-11-30 11:27:27.000000 craft-cli-1.2.0/craft_cli/py.typed
--rw-rw-r--   0 facundo   (1000) facundo   (1000)     8090 2022-06-28 19:36:35.000000 craft-cli-1.2.0/craft_cli/pytest_plugin.py
-drwxrwxr-x   0 facundo   (1000) facundo   (1000)        0 2022-08-08 12:30:29.452455 craft-cli-1.2.0/craft_cli.egg-info/
--rw-rw-r--   0 facundo   (1000) facundo   (1000)     2952 2022-08-08 12:30:29.000000 craft-cli-1.2.0/craft_cli.egg-info/PKG-INFO
--rw-rw-r--   0 facundo   (1000) facundo   (1000)      452 2022-08-08 12:30:29.000000 craft-cli-1.2.0/craft_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 facundo   (1000) facundo   (1000)        1 2022-08-08 12:30:29.000000 craft-cli-1.2.0/craft_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 facundo   (1000) facundo   (1000)       46 2022-08-08 12:30:29.000000 craft-cli-1.2.0/craft_cli.egg-info/entry_points.txt
--rw-rw-r--   0 facundo   (1000) facundo   (1000)        1 2022-04-22 14:43:03.000000 craft-cli-1.2.0/craft_cli.egg-info/not-zip-safe
--rw-rw-r--   0 facundo   (1000) facundo   (1000)      620 2022-08-08 12:30:29.000000 craft-cli-1.2.0/craft_cli.egg-info/requires.txt
--rw-rw-r--   0 facundo   (1000) facundo   (1000)       10 2022-08-08 12:30:29.000000 craft-cli-1.2.0/craft_cli.egg-info/top_level.txt
--rw-rw-r--   0 facundo   (1000) facundo   (1000)      194 2021-11-10 16:17:03.000000 craft-cli-1.2.0/pyproject.toml
--rw-rw-r--   0 facundo   (1000) facundo   (1000)     2329 2022-08-08 12:30:29.456455 craft-cli-1.2.0/setup.cfg
--rw-rw-r--   0 facundo   (1000) facundo   (1000)      804 2021-11-10 16:17:03.000000 craft-cli-1.2.0/setup.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.479392 craft-cli-2.0.0/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      193 2022-08-15 14:30:03.000000 craft-cli-2.0.0/.bumpversion.cfg
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      723 2023-06-15 14:02:00.000000 craft-cli-2.0.0/.editorconfig
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.471392 craft-cli-2.0.0/.github/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      172 2023-06-15 14:02:00.000000 craft-cli-2.0.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      506 2023-06-15 14:02:00.000000 craft-cli-2.0.0/.github/release-drafter.yml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3504 2023-06-15 14:02:00.000000 craft-cli-2.0.0/.github/renovate.json5
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.475392 craft-cli-2.0.0/.github/workflows/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      179 2023-06-15 14:02:00.000000 craft-cli-2.0.0/.github/workflows/cla-check.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      822 2023-06-15 14:02:00.000000 craft-cli-2.0.0/.github/workflows/docs.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      347 2023-06-15 14:02:00.000000 craft-cli-2.0.0/.github/workflows/release-drafter.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2441 2023-06-15 22:43:44.000000 craft-cli-2.0.0/.github/workflows/tests.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1949 2023-06-15 14:02:00.000000 craft-cli-2.0.0/.gitignore
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      921 2023-06-15 14:02:00.000000 craft-cli-2.0.0/.pre-commit-config.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    17440 2023-06-15 14:02:00.000000 craft-cli-2.0.0/.pylintrc
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      485 2023-06-15 14:02:00.000000 craft-cli-2.0.0/.readthedocs.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      188 2023-06-15 14:02:00.000000 craft-cli-2.0.0/.yamllint.yaml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3819 2023-06-16 18:31:51.000000 craft-cli-2.0.0/HACKING.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2362 2022-08-15 14:30:03.000000 craft-cli-2.0.0/HOWTO_RELEASE.md
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     7652 2023-06-15 13:31:45.000000 craft-cli-2.0.0/LICENSE
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       34 2022-08-15 14:30:03.000000 craft-cli-2.0.0/MANIFEST.in
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    10877 2023-06-16 18:37:43.479392 craft-cli-2.0.0/PKG-INFO
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      755 2023-06-16 18:31:51.000000 craft-cli-2.0.0/README.rst
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.475392 craft-cli-2.0.0/craft_cli/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1661 2023-06-15 14:02:00.000000 craft-cli-2.0.0/craft_cli/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      160 2023-06-16 18:37:43.000000 craft-cli-2.0.0/craft_cli/_version.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    18909 2023-06-15 18:06:58.000000 craft-cli-2.0.0/craft_cli/dispatcher.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3076 2023-06-07 17:48:53.000000 craft-cli-2.0.0/craft_cli/errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    14578 2023-06-07 18:36:51.000000 craft-cli-2.0.0/craft_cli/helptexts.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    26272 2023-06-15 17:13:52.000000 craft-cli-2.0.0/craft_cli/messages.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    14777 2023-06-15 14:02:00.000000 craft-cli-2.0.0/craft_cli/printer.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2022-08-15 14:30:03.000000 craft-cli-2.0.0/craft_cli/py.typed
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     8155 2023-06-15 17:18:02.000000 craft-cli-2.0.0/craft_cli/pytest_plugin.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.475392 craft-cli-2.0.0/craft_cli.egg-info/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    10877 2023-06-16 18:37:43.000000 craft-cli-2.0.0/craft_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1693 2023-06-16 18:37:43.000000 craft-cli-2.0.0/craft_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        1 2023-06-16 18:37:43.000000 craft-cli-2.0.0/craft_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       45 2023-06-16 18:37:43.000000 craft-cli-2.0.0/craft_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      554 2023-06-16 18:37:43.000000 craft-cli-2.0.0/craft_cli.egg-info/requires.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       19 2023-06-16 18:37:43.000000 craft-cli-2.0.0/craft_cli.egg-info/top_level.txt
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.475392 craft-cli-2.0.0/docs/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       42 2022-08-15 14:30:03.000000 craft-cli-2.0.0/docs/.gitignore
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.475392 craft-cli-2.0.0/docs/_static/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2022-08-15 14:30:03.000000 craft-cli-2.0.0/docs/_static/.gitempty
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.475392 craft-cli-2.0.0/docs/_static/css/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      481 2023-06-15 14:02:00.000000 craft-cli-2.0.0/docs/_static/css/custom.css
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2668 2023-06-15 14:02:00.000000 craft-cli-2.0.0/docs/conf.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    16076 2023-06-15 14:02:00.000000 craft-cli-2.0.0/docs/explanations.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     8484 2023-06-15 14:02:00.000000 craft-cli-2.0.0/docs/howtos.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      771 2023-06-15 14:02:00.000000 craft-cli-2.0.0/docs/index.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       90 2023-06-15 14:02:00.000000 craft-cli-2.0.0/docs/reference.rst
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     6550 2023-06-15 14:02:00.000000 craft-cli-2.0.0/docs/tutorials.rst
+-rwxrwxr-x   0 tiago     (1000) tiago     (1000)    14270 2023-06-15 14:01:56.000000 craft-cli-2.0.0/examples.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     8687 2023-06-16 18:31:51.000000 craft-cli-2.0.0/pyproject.toml
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       38 2023-06-16 18:37:43.479392 craft-cli-2.0.0/setup.cfg
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.475392 craft-cli-2.0.0/tests/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2022-08-15 14:30:03.000000 craft-cli-2.0.0/tests/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2813 2023-06-15 17:20:37.000000 craft-cli-2.0.0/tests/conftest.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1285 2022-08-15 14:30:03.000000 craft-cli-2.0.0/tests/factory.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.475392 craft-cli-2.0.0/tests/integration/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2022-08-15 14:30:03.000000 craft-cli-2.0.0/tests/integration/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       33 2022-08-15 14:30:03.000000 craft-cli-2.0.0/tests/integration/test_stub.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2022-08-15 14:30:03.000000 craft-cli-2.0.0/tests/py.typed
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     7507 2023-06-07 17:48:53.000000 craft-cli-2.0.0/tests/test_pytest_plugin.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.479392 craft-cli-2.0.0/tests/unit/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        0 2022-08-15 14:30:03.000000 craft-cli-2.0.0/tests/unit/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    23381 2023-06-15 14:01:56.000000 craft-cli-2.0.0/tests/unit/test_dispatcher.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     2046 2023-06-07 17:48:53.000000 craft-cli-2.0.0/tests/unit/test_errors.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    44447 2023-06-07 17:48:53.000000 craft-cli-2.0.0/tests/unit/test_help.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    37699 2023-06-15 17:13:52.000000 craft-cli-2.0.0/tests/unit/test_messages_emitter.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    14173 2023-06-07 17:48:53.000000 craft-cli-2.0.0/tests/unit/test_messages_helpers.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    45581 2023-06-15 17:13:52.000000 craft-cli-2.0.0/tests/unit/test_messages_integration.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    10797 2023-06-15 17:13:52.000000 craft-cli-2.0.0/tests/unit/test_messages_stream_cm.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    39741 2023-06-14 18:56:33.000000 craft-cli-2.0.0/tests/unit/test_printer.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     5350 2023-06-15 22:43:44.000000 craft-cli-2.0.0/tox.ini
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.471392 craft-cli-2.0.0/venv/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2023-06-16 18:37:43.479392 craft-cli-2.0.0/venv/bin/
+-rwxrwxr-x   0 tiago     (1000) tiago     (1000)      631 2023-06-14 15:13:41.000000 craft-cli-2.0.0/venv/bin/rst2html.py
+-rwxrwxr-x   0 tiago     (1000) tiago     (1000)      751 2023-06-14 15:13:41.000000 craft-cli-2.0.0/venv/bin/rst2html4.py
+-rwxrwxr-x   0 tiago     (1000) tiago     (1000)     1119 2023-06-14 15:13:41.000000 craft-cli-2.0.0/venv/bin/rst2html5.py
+-rwxrwxr-x   0 tiago     (1000) tiago     (1000)      828 2023-06-14 15:13:41.000000 craft-cli-2.0.0/venv/bin/rst2latex.py
+-rwxrwxr-x   0 tiago     (1000) tiago     (1000)      636 2023-06-14 15:13:41.000000 craft-cli-2.0.0/venv/bin/rst2man.py
+-rwxrwxr-x   0 tiago     (1000) tiago     (1000)      801 2023-06-14 15:13:41.000000 craft-cli-2.0.0/venv/bin/rst2odt.py
+-rwxrwxr-x   0 tiago     (1000) tiago     (1000)     1763 2023-06-14 15:13:41.000000 craft-cli-2.0.0/venv/bin/rst2odt_prepstyles.py
+-rwxrwxr-x   0 tiago     (1000) tiago     (1000)      638 2023-06-14 15:13:41.000000 craft-cli-2.0.0/venv/bin/rst2pseudoxml.py
+-rwxrwxr-x   0 tiago     (1000) tiago     (1000)      674 2023-06-14 15:13:41.000000 craft-cli-2.0.0/venv/bin/rst2s5.py
+-rwxrwxr-x   0 tiago     (1000) tiago     (1000)      908 2023-06-14 15:13:41.000000 craft-cli-2.0.0/venv/bin/rst2xetex.py
+-rwxrwxr-x   0 tiago     (1000) tiago     (1000)      639 2023-06-14 15:13:41.000000 craft-cli-2.0.0/venv/bin/rst2xml.py
+-rwxrwxr-x   0 tiago     (1000) tiago     (1000)      707 2023-06-14 15:13:41.000000 craft-cli-2.0.0/venv/bin/rstpep2html.py
```

### Comparing `craft-cli-1.2.0/LICENSE` & `craft-cli-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `craft-cli-1.2.0/craft_cli/__init__.py` & `craft-cli-2.0.0/craft_cli/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,24 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 """Interact with Canonical services such as Charmhub and the Snap Store."""
 
-__version__ = "1.2.0"
+try:
+    from ._version import __version__
+except ImportError:  # pragma: no cover
+    from importlib.metadata import version, PackageNotFoundError
+
+    try:
+        __version__ = version("craft-cli")
+    except PackageNotFoundError:
+        __version__ = "dev"
+
 
 # names included here only to be exposed as external API; the particular order of imports
 # is to break cyclic dependencies
 from .messages import EmitterMode, emit  # noqa: F401 ; isort:skip
 from .dispatcher import BaseCommand, CommandGroup, Dispatcher, GlobalArgument  # noqa: F401
 from .errors import ArgumentParsingError, CraftError, ProvideHelpException  # noqa: F401
 from .helptexts import HIDDEN  # noqa: F401
```

### Comparing `craft-cli-1.2.0/craft_cli/dispatcher.py` & `craft-cli-2.0.0/craft_cli/dispatcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,43 +13,55 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 """Argument processing and command dispatching functionality."""
 
 import argparse
 import difflib
-from collections import namedtuple
-from typing import Any, Dict, List, Optional, Tuple, Type
+from typing import Any, Dict, List, Literal, NamedTuple, Optional, Tuple, Type
 
 from craft_cli import EmitterMode, emit
 from craft_cli.errors import ArgumentParsingError, ProvideHelpException
 from craft_cli.helptexts import HelpBuilder, OutputFormat
 
-CommandGroup = namedtuple("CommandGroup", "name commands")
-"""Definition of a command group.
 
-A list of these is what is passed to the ``Dispatcher`` to run commands as part
-of the application.
+class CommandGroup(NamedTuple):
+    """Definition of a command group.
+
+    A list of these is what is passed to the ``Dispatcher`` to run commands as part
+    of the application.
+
+    :param name: identifier of the command group (to be used in help texts).
+    :param commands: a list of the commands in this group.
+    """
+
+    name: str
+    commands: List[Type["BaseCommand"]]
+
+
+class GlobalArgument(NamedTuple):
+    """Definition of a global argument to be handled by the Dispatcher.
+
+    :param name: identifier of the argument (the reference in the dictionary returned
+        by ``Dispatcher.pre_parse_args`` method)
+    :param type: the argument type: ``flag`` for arguments that are set to ``True`` if
+        specified (``False`` by default), or ``option`` if a value is needed after it.
+    :param short_option: the short form of the argument (a dash with a letter, e.g. ``-s``); it can
+        be None if the option does not have a short form.
+    :param long_option: the long form of the argument (two dashes and a name, e.g. ``--secure``).
+    :param help_message: the one-line text that describes the argument, for building the help texts.
+    """
+
+    name: str
+    type: Literal["flag", "option"]
+    short_option: Optional[str]
+    long_option: str
+    help_message: str
+
 
-:param name: identifier of the command group (to be used in help texts).
-:param commands: a list of the commands in this group.
-"""
-
-GlobalArgument = namedtuple("GlobalArgument", "name type short_option long_option help_message")
-"""Definition of a global argument to be handled by the Dispatcher.
-
-:param name: identifier of the argument (the reference in the dictionary returned
-    by ``Dispatcher.pre_parse_args`` method)
-:param type: the argument type: ``flag`` for arguments that are set to ``True`` if
-    specified (``False`` by default), or ``option`` if a value is needed after it.
-:param short_option: the short form of the argument (a dash with a letter, e.g. ``-s``); it can
-    be None if the option does not have a short form.
-:param long_option: the long form of the argument (two dashes and a name, e.g. ``--secure``).
-:param help_message: the one-line text that describes the argument, for building the help texts.
-"""
 _DEFAULT_GLOBAL_ARGS = [
     GlobalArgument(
         "help",
         "flag",
         "-h",
         "--help",
         "Show this help message and exit",
@@ -100,27 +112,27 @@
     It also must/can override some methods for the proper command behaviour (see each
     method's docstring).
 
     The subclass must be declared in the corresponding section of command groups indicated
     to the Dispatcher.
     """
 
+    name: str
+    help_msg: str
+    overview: str
     common = False
     hidden = False
-    name: Optional[str] = None
-    help_msg: Optional[str] = None
-    overview: Optional[str] = None
 
     def __init__(self, config: Optional[Dict[str, Any]]):
         self.config = config
 
         # validate attributes
         mandatory = ("name", "help_msg", "overview")
         for attr_name in mandatory:
-            if getattr(self, attr_name) is None:
+            if getattr(self, attr_name, None) is None:
                 raise ValueError(f"Bad command configuration: missing value in '{attr_name}'.")
         if self.common and self.hidden:
             raise ValueError("Common commands can not be hidden.")
 
     def fill_parser(self, parser: "_CustomArgumentParser") -> None:
         """Specify command's specific parameters.
 
@@ -238,15 +250,15 @@
             help_text = self._help_builder.get_detailed_help(options)
         else:
             help_text = self._help_builder.get_full_help(options)
         return help_text
 
     def _build_usage_exc(self, text):
         """Build an ArgumentParsingError exception with the usage message from the given text."""
-        raise ArgumentParsingError(self._help_builder.get_usage_message(text))
+        return ArgumentParsingError(self._help_builder.get_usage_message(text))
 
     def _get_requested_help(
         self, parameters
     ):  # pylint: disable=too-many-locals disable=too-many-branches
         """Produce the requested help depending on the rest of the command line params."""
         if len(parameters) == 0:
             # provide a general text when help was requested without parameters
@@ -330,15 +342,17 @@
             else:
                 *previous, last = similar
                 similar_text = ", ".join(repr(x) for x in previous) + f" or {last!r}"
             extra_similar = f", maybe you meant {similar_text}"
         msg = f"no such command {missing_command!r}{extra_similar}"
         return self._help_builder.get_usage_message(msg)
 
-    def _parse_options(self, defined_arguments, sysargs):  # pylint: disable=too-many-branches
+    def _parse_options(
+        self, defined_arguments: List[GlobalArgument], sysargs: List[str]
+    ):  # pylint: disable=too-many-branches
         """Parse arguments."""
         # get all arguments (default to what's specified) and those per options, to filter sysargs
         global_args: Dict[str, Any] = {}
         arg_per_option = {}
         options_with_equal = []
         for arg in defined_arguments:
             if arg.short_option is not None:
```

### Comparing `craft-cli-1.2.0/craft_cli/errors.py` & `craft-cli-2.0.0/craft_cli/errors.py`

 * *Files identical despite different names*

### Comparing `craft-cli-1.2.0/craft_cli/helptexts.py` & `craft-cli-2.0.0/craft_cli/helptexts.py`

 * *Files identical despite different names*

### Comparing `craft-cli-1.2.0/craft_cli/messages.py` & `craft-cli-2.0.0/craft_cli/messages.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-#
-# Copyright 2021-2022 Canonical Ltd.
+# Copyright 2021-2023 Canonical Ltd.
 #
 # This program is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License version 3 as published by the Free Software Foundation.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -19,91 +18,51 @@
 __all__ = [
     "EmitterMode",
     "TESTMODE",
     "emit",
 ]
 
 import enum
-import itertools
 import logging
-import math
 import os
 import pathlib
-import queue
 import select
-import shutil
 import sys
 import threading
-import time
 import traceback
 from contextlib import contextmanager
-from dataclasses import dataclass, field
 from datetime import datetime
-from functools import lru_cache
-from typing import Literal, Optional, TextIO, Union
+from typing import Any, Callable, cast, Dict, Literal, Optional, TextIO, TypeVar, Union
 
 import platformdirs
 
 try:
     import win32pipe  # type: ignore
 
     _WINDOWS_MODE = True
 except ImportError:
     _WINDOWS_MODE = False
 
 from craft_cli import errors
-
-
-@lru_cache
-def _stream_is_terminal(stream: Union[TextIO, None]) -> bool:
-    is_a_terminal = getattr(stream, "isatty", lambda: False)()
-    return is_a_terminal and _get_terminal_width() > 0
-
-
-@dataclass
-class _MessageInfo:  # pylint: disable=too-many-instance-attributes
-    """Comprehensive information for a message that may go to screen and log."""
-
-    stream: Union[TextIO, None]
-    text: str
-    ephemeral: bool = False
-    bar_progress: Union[int, float, None] = None
-    bar_total: Union[int, float, None] = None
-    use_timestamp: bool = False
-    end_line: bool = False
-    created_at: datetime = field(default_factory=datetime.now)
-
+from craft_cli.printer import Printer
 
 # the different modes the Emitter can be set
 EmitterMode = enum.Enum("EmitterMode", "QUIET BRIEF VERBOSE DEBUG TRACE")
 
 # the limit to how many log files to have
 _MAX_LOG_FILES = 5
 
-# the char used to draw the progress bar ('FULL BLOCK')
-_PROGRESS_BAR_SYMBOL = "█"
-
-# seconds before putting the spinner to work
-_SPINNER_THRESHOLD = 2
-
-# seconds between each spinner char
-_SPINNER_DELAY = 0.1
-
 # the size of bytes chunk that the pipe reader will read at once
 _PIPE_READER_CHUNK_SIZE = 4096
 
-# set to true when running *application* tests so some behaviours change
+# set to true when running *application* tests so some behaviours change (see
+# craft_cli/pytest_plugin.py )
 TESTMODE = False
 
 
-def _get_terminal_width() -> int:
-    """Return the number of columns of the terminal."""
-    return shutil.get_terminal_size().columns
-
-
 def _get_log_filepath(appname: str) -> pathlib.Path:
     """Provide a unique filepath for logging.
 
     The app name is used for both the directory where the logs are located and each log name.
 
     Rules:
     - use an platformdirs provided directory
@@ -138,322 +97,20 @@
     """Get the traceback lines (if any) from an exception."""
     tback_lines = traceback.format_exception(type(exc), exc, exc.__traceback__)
     for tback_line in tback_lines:
         for real_line in tback_line.rstrip().split("\n"):
             yield real_line
 
 
-class _Spinner(threading.Thread):
-    """A supervisor thread that will repeat long-standing messages with a spinner besides it.
-
-    This will be a long-lived single thread that will supervise each message received
-    through the `supervise` method, and when it stays too long, the printer's `spin`
-    will be called with that message and a text to "draw" a spinner, including the elapsed
-    time.
-
-    The timing related part of the code uses two constants: _SPINNER_THRESHOLD is how
-    many seconds before activating the spinner for the message, and _SPINNER_DELAY is
-    the time between `spin` calls.
-
-    When a new message arrives (or None, to indicate that there is nothing to supervise) and
-    the previous message was "being spinned", a last `spin` call will be done to clean
-    the spinner.
-    """
-
-    def __init__(self, printer: "_Printer"):
-        super().__init__()
-        # special flag used to stop the spinner thread
-        self.stop_flag = object()
-
-        # daemon mode, so if the app crashes this thread does not holds everything
-        self.daemon = True
-
-        # communication from the printer
-        self.queue: queue.Queue = queue.Queue()
-
-        # hold the printer, to make it spin
-        self.printer = printer
-
-        # a lock to wait the spinner to stop spinning
-        self.lock = threading.Lock()
-
-    def run(self) -> None:
-        prv_msg = None
-        t_init = time.time()
-        while prv_msg is not self.stop_flag:
-            try:
-                new_msg = self.queue.get(timeout=_SPINNER_THRESHOLD)
-            except queue.Empty:
-                # waited too much, start to show a spinner (if have a previous message) until
-                # we have further info
-                if prv_msg is None or prv_msg.end_line:
-                    continue
-                spinchars = itertools.cycle("-\\|/")
-                with self.lock:
-                    while True:
-                        t_delta = time.time() - t_init
-                        spintext = f" {next(spinchars)} ({t_delta:.1f}s)"
-                        self.printer.spin(prv_msg, spintext)
-                        try:
-                            new_msg = self.queue.get(timeout=_SPINNER_DELAY)
-                        except queue.Empty:
-                            # still nothing! keep going
-                            continue
-                        # got a new message: clean the spinner and exit from the spinning state
-                        self.printer.spin(prv_msg, " ")
-                        break
-
-            prv_msg = new_msg
-            t_init = time.time()
-
-    def supervise(self, message: Optional[_MessageInfo]) -> None:
-        """Supervise a message to spin it if it remains too long."""
-        self.queue.put(message)
-        # (maybe) wait for the spinner to exit spinning state (which does some cleaning)
-        self.lock.acquire()  # pylint: disable=consider-using-with
-        self.lock.release()
-
-    def stop(self) -> None:
-        """Stop self."""
-        self.queue.put(self.stop_flag)
-        self.join()
-
-
-class _Printer:
-    """Handle writing the different messages to the different outputs (out, err and log).
-
-    If TESTMODE is True, this class changes its behaviour: the spinner is never started,
-    so there is no thread polluting messages when running tests if they take too long to run.
-    """
-
-    def __init__(self, log_filepath: pathlib.Path) -> None:
-        self.stopped = False
-
-        # holder of the previous message
-        self.prv_msg: Optional[_MessageInfo] = None
-
-        # open the log file (will be closed explicitly later)
-        self.log = open(log_filepath, "at", encoding="utf8")  # pylint: disable=consider-using-with
-
-        # keep account of output streams with unfinished lines
-        self.unfinished_stream: Optional[TextIO] = None
-
-        # run the spinner supervisor
-        self.spinner = _Spinner(self)
-        if not TESTMODE:
-            self.spinner.start()
-
-    def _write_line_terminal(self, message: _MessageInfo, *, spintext: str = "") -> None:
-        """Write a simple line message to the screen."""
-        # prepare the text with (maybe) the timestamp
-        if message.use_timestamp:
-            timestamp_str = message.created_at.isoformat(sep=" ", timespec="milliseconds")
-            text = timestamp_str + " " + message.text
-        else:
-            text = message.text
-
-        if spintext:
-            # forced to overwrite the previous message to present the spinner
-            maybe_cr = "\r"
-        elif self.prv_msg is None or self.prv_msg.end_line:
-            # first message, or previous message completed the line: start clean
-            maybe_cr = ""
-        elif self.prv_msg.ephemeral:
-            # the last one was ephemeral, overwrite it
-            maybe_cr = "\r"
-        else:
-            # complete the previous line, leaving that message ok
-            maybe_cr = ""
-            print(flush=True, file=self.prv_msg.stream)
-
-        # fill with spaces until the very end, on one hand to clear a possible previous message,
-        # but also to always have the cursor at the very end
-        width = _get_terminal_width()
-        usable = width - len(spintext) - 1  # the 1 is the cursor itself
-        if len(text) > usable:
-            if message.ephemeral:
-                text = text[: usable - 1] + "…"
-            elif spintext:
-                # we need to rewrite the message with the spintext, use only the last line for
-                # multiline messages, and ensure (again) that the last real line fits
-                remaining_for_last_line = len(text) % width
-                text = text[-remaining_for_last_line:]
-                if len(text) > usable:
-                    text = text[: usable - 1] + "…"
-        cleaner = " " * (usable - len(text) % width)
-
-        line = maybe_cr + text + spintext + cleaner
-        print(line, end="", flush=True, file=message.stream)
-        if message.end_line:
-            # finish the just shown line, as we need a clean terminal for some external thing
-            print(flush=True, file=message.stream)
-            self.unfinished_stream = None
-        else:
-            self.unfinished_stream = message.stream
-
-    def _write_line_captured(self, message: _MessageInfo) -> None:
-        """Write a simple line message to a captured output."""
-        # prepare the text with (maybe) the timestamp
-        if message.use_timestamp:
-            timestamp_str = message.created_at.isoformat(sep=" ", timespec="milliseconds")
-            text = timestamp_str + " " + message.text
-        else:
-            text = message.text
-
-        print(text, file=message.stream)
-
-    def _write_bar_terminal(self, message: _MessageInfo) -> None:
-        """Write a progress bar to the screen."""
-        # prepare the text with (maybe) the timestamp
-        if message.use_timestamp:
-            timestamp_str = message.created_at.isoformat(sep=" ", timespec="milliseconds")
-            text = timestamp_str + " " + message.text
-        else:
-            text = message.text
-
-        if self.prv_msg is None or self.prv_msg.end_line:
-            # first message, or previous message completed the line: start clean
-            maybe_cr = ""
-        elif self.prv_msg.ephemeral:
-            # the last one was ephemeral, overwrite it
-            maybe_cr = "\r"
-        else:
-            # complete the previous line, leaving that message ok
-            maybe_cr = ""
-            print(flush=True, file=self.prv_msg.stream)
-
-        numerical_progress = f"{message.bar_progress}/{message.bar_total}"
-        bar_percentage = min(message.bar_progress / message.bar_total, 1)  # type: ignore
-
-        # terminal size minus the text and numerical progress, and 5 (the cursor at the end,
-        # two spaces before and after the bar, and two surrounding brackets)
-        terminal_width = _get_terminal_width()
-        bar_width = terminal_width - len(text) - len(numerical_progress) - 5
-
-        # only show the bar with progress if there is enough space, otherwise just the
-        # message (truncated, if needed)
-        if bar_width > 0:
-            completed_width = math.floor(bar_width * min(bar_percentage, 100))
-            completed_bar = _PROGRESS_BAR_SYMBOL * completed_width
-            empty_bar = " " * (bar_width - completed_width)
-            line = f"{maybe_cr}{text} [{completed_bar}{empty_bar}] {numerical_progress}"
-        else:
-            text = text[: terminal_width - 1]  # space for cursor
-            line = f"{maybe_cr}{text}"
-
-        print(line, end="", flush=True, file=message.stream)
-        self.unfinished_stream = message.stream
-
-    def _write_bar_captured(self, message: _MessageInfo) -> None:
-        """Do not write any progress bar to the captured output."""
-
-    def _show(self, msg: _MessageInfo) -> None:
-        """Show the composed message."""
-        # show the message in one way or the other only if there is a stream
-        if msg.stream is None:
-            return
-
-        # the writing functions depend on the final output: if the stream is captured or it's
-        # a real terminal
-        if _stream_is_terminal(msg.stream):
-            write_line = self._write_line_terminal
-            write_bar = self._write_bar_terminal
-        else:
-            write_line = self._write_line_captured  # type: ignore
-            write_bar = self._write_bar_captured
-
-        if msg.bar_progress is None:
-            # regular message, send it to the spinner and write it
-            self.spinner.supervise(msg)
-            write_line(msg)
-        else:
-            # progress bar, send None to the spinner (as it's not a "spinnable" message)
-            # and write it
-            self.spinner.supervise(None)
-            write_bar(msg)
-        self.prv_msg = msg
-
-    def _log(self, message: _MessageInfo) -> None:
-        """Write the line message to the log file."""
-        # prepare the text with (maybe) the timestamp
-        timestamp_str = message.created_at.isoformat(sep=" ", timespec="milliseconds")
-        self.log.write(f"{timestamp_str} {message.text}\n")
-
-    def spin(self, message: _MessageInfo, spintext: str) -> None:
-        """Write a line message including a spin text, only to a terminal."""
-        if _stream_is_terminal(message.stream):
-            self._write_line_terminal(message, spintext=spintext)
-
-    def show(
-        self,
-        stream: Optional[TextIO],
-        text: str,
-        *,
-        ephemeral: bool = False,
-        use_timestamp: bool = False,
-        end_line: bool = False,
-        avoid_logging: bool = False,
-    ) -> None:
-        """Show a text to the given stream if not stopped."""
-        if self.stopped:
-            return
-
-        msg = _MessageInfo(
-            stream=stream,
-            text=text.rstrip(),
-            ephemeral=ephemeral,
-            use_timestamp=use_timestamp,
-            end_line=end_line,
-        )
-        self._show(msg)
-        if not avoid_logging:
-            self._log(msg)
-
-    def progress_bar(
-        self,
-        stream: Optional[TextIO],
-        text: str,
-        *,
-        progress: Union[int, float],
-        total: Union[int, float],
-        use_timestamp: bool,
-    ) -> None:
-        """Show a progress bar to the given stream."""
-        msg = _MessageInfo(
-            stream=stream,
-            text=text.rstrip(),
-            bar_progress=progress,
-            bar_total=total,
-            ephemeral=True,  # so it gets eventually overwritten by other message
-            use_timestamp=use_timestamp,
-        )
-        self._show(msg)
-
-    def stop(self) -> None:
-        """Stop the printing infrastructure.
-
-        In detail:
-        - stop the spinner
-        - add a new line to the screen (if needed)
-        - close the log file
-        """
-        if not TESTMODE:
-            self.spinner.stop()
-        if self.unfinished_stream is not None:
-            print(flush=True, file=self.unfinished_stream)
-        self.log.close()
-        self.stopped = True
-
-
 class _Progresser:  # pylint: disable=too-many-instance-attributes
     """A context manager to follow progress on any specific action."""
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
-        printer: _Printer,
+        printer: Printer,
         total: Union[int, float],
         text: str,
         stream: Optional[TextIO],
         delta: bool,
         use_timestamp: bool,
         ephemeral_context: bool,
     ):
@@ -511,26 +168,29 @@
     - windows: read in a blocking way, so the `stop` method will write a byte to unblock it
         after setting the stop flag (this extra byte is handled by the reading code)
     """
 
     # byte used to unblock the reading (under Windows)
     UNBLOCK_BYTE = b"\x00"
 
-    def __init__(self, printer: _Printer, stream: Optional[TextIO], use_timestamp: bool):
+    def __init__(self, printer: Printer, stream: Optional[TextIO], printer_flags: Dict[str, bool]):
         super().__init__()
-        self.use_timestamp = use_timestamp
+        self.printer_flags = printer_flags
 
         # prepare the pipe pair: the one to read (used in the thread core loop) and the
         # one which is to be written externally (and also used internally under windows
         # to unblock the reading); also note that the pipe pair themselves depend
         # on the platform
         if _WINDOWS_MODE:
             # parameters: default security, default buffer size, binary mode
             binary_mode = os.O_BINARY  # pylint: disable=no-member  # (it does exist in Windows!)
-            self.read_pipe, self.write_pipe = win32pipe.FdCreatePipe(None, 0, binary_mode)
+            # ignoring the type of the first parameter below, as documentation allows to use None
+            # to make it use a NULL security descriptor:
+            #     https://www.markjour.com/docs/pywin32-docs/PySECURITY_ATTRIBUTES.html
+            self.read_pipe, self.write_pipe = win32pipe.FdCreatePipe(None, 0, binary_mode)  # type: ignore
         else:
             self.read_pipe, self.write_pipe = os.pipe()
 
         # special flag used to stop the pipe reader thread
         self.stop_flag = False
 
         # where to collect the content that is being read but yet not written (waiting for
@@ -557,16 +217,19 @@
             # get the useful line and update pointer for next cycle (plus one, to
             # skip the new line itself)
             useful_line = data[pointer:newline_position]
             pointer = newline_position + 1
 
             # write the useful line to intended outputs
             unicode_line = useful_line.decode("utf8")
+            # replace tabs with a set number of spaces so that the printer
+            # can correctly count the characters.
+            unicode_line = unicode_line.replace("\t", "  ")
             text = f":: {unicode_line}"
-            self.printer.show(self.stream, text, end_line=True, use_timestamp=self.use_timestamp)
+            self.printer.show(self.stream, text, **self.printer_flags)
 
     def _run_posix(self) -> None:
         """Run the thread, handling pipes in the POSIX way."""
         poller = select.poll()
         poller.register(self.read_pipe, select.POLLIN)
         while True:
             rlist = poller.poll(0.1)
@@ -590,15 +253,14 @@
                 data = data[:-1]
                 if data:
                     self._write(data)
                 break
 
             if data:
                 self._write(data)
-            time.sleep(0.1)
 
     def run(self) -> None:
         """Run the thread."""
         if _WINDOWS_MODE:
             self._run_windows()
         else:
             self._run_posix()
@@ -618,37 +280,50 @@
         os.close(self.read_pipe)
         os.close(self.write_pipe)
 
 
 class _StreamContextManager:
     """A context manager that provides a pipe for subprocess to write its output."""
 
-    def __init__(
-        self, printer: _Printer, text: str, stream: Optional[TextIO], use_timestamp: bool
+    def __init__(  # pylint: disable=too-many-arguments
+        self,
+        printer: Printer,
+        text: str,
+        stream: Optional[TextIO],
+        use_timestamp: bool,
+        ephemeral_mode: bool,
     ):
+        # prepare the printer flags for the initial message and everything produced
+        # by the pipe reader
+        printer_flags = {
+            "use_timestamp": use_timestamp,
+            "ephemeral": ephemeral_mode,
+            "end_line": not ephemeral_mode,
+        }
+
         # show the intended text (explicitly asking for a complete line) before passing the
         # output command to the pip-reading thread
-        printer.show(stream, text, end_line=True, use_timestamp=use_timestamp)
+        printer.show(stream, text, **printer_flags)
 
         # enable the thread to read and show what comes through the provided pipe
-        self.pipe_reader = _PipeReaderThread(printer, stream, use_timestamp)
+        self.pipe_reader = _PipeReaderThread(printer, stream, printer_flags)
 
     def __enter__(self):
         self.pipe_reader.start()
         return self.pipe_reader.write_pipe
 
     def __exit__(self, *exc_info):
         self.pipe_reader.stop()
         return False  # do not consume any exception
 
 
 class _Handler(logging.Handler):
     """A logging handler that emits messages through the core Printer."""
 
-    def __init__(self, printer: _Printer):
+    def __init__(self, printer: Printer):
         super().__init__()
         self.printer = printer
 
         # level is 0 so we get EVERYTHING (as we need to send it all to the log file), and
         # will decide on "emit" if also goes to screen using the custom mode
         self.level = 0
         self.mode = EmitterMode.QUIET
@@ -672,33 +347,38 @@
             # in trace, everything
             stream = sys.stderr
 
         use_timestamp = self.mode in (EmitterMode.DEBUG, EmitterMode.TRACE)
         self.printer.show(stream, record.getMessage(), use_timestamp=use_timestamp)
 
 
-def _active_guard(ignore_when_stopped=False):
+FuncT = TypeVar("FuncT", bound=Callable[..., Any])
+
+
+def _active_guard(ignore_when_stopped: bool = False) -> Callable[..., Any]:
     """Decorate Emitter methods to be called when active.
 
     It will check that the emitter is initiated and that is not stopped (except when
     ignore_when_stopped=True, in that case the call will be ignored, to support
     double-ending).
     """
 
-    def decorator(wrapped_func):
-        def func(self, *args, **kwargs):  # pylint: disable=inconsistent-return-statements
+    def decorator(wrapped_func: FuncT) -> FuncT:
+        def func(  # pylint: disable=inconsistent-return-statements
+            self, *args: Any, **kwargs: Any
+        ) -> Any:
             if not self._initiated:  # pylint: disable=protected-access
                 raise RuntimeError("Emitter needs to be initiated first")
             if self._stopped:  # pylint: disable=protected-access
                 if ignore_when_stopped:
                     return
                 raise RuntimeError("Emitter is stopped already")
             return wrapped_func(self, *args, **kwargs)
 
-        return func
+        return cast(FuncT, func)
 
     return decorator
 
 
 class Emitter:
     """Main interface to all the messages emitting functionality.
 
@@ -747,15 +427,15 @@
                 raise RuntimeError("Double Emitter init detected!")
 
         self._greeting = greeting
 
         # create a log file, bootstrap the printer, and before anything else send the greeting
         # to the file
         self._log_filepath = _get_log_filepath(appname) if log_filepath is None else log_filepath
-        self._printer = _Printer(self._log_filepath)
+        self._printer = Printer(self._log_filepath)
         self._printer.show(None, greeting)
 
         # hook into the logging system
         logger = logging.getLogger()
         self._log_handler = _Handler(self._printer)
         logger.addHandler(self._log_handler)
 
@@ -835,15 +515,15 @@
         A way to expose system-generated information, about the general process or
         particular information, which in general would be too overwhelming for
         debugging purposes but sometimes needed for particular analysis.
 
         It only produces information to the screen and into the logs if in TRACE mode.
         """
         # as we're not even logging anything if not in TRACE mode, instead of calling the
-        # _Printer with no stream and the 'avoid_logging' flag (which would be more consistent
+        # Printer with no stream and the 'avoid_logging' flag (which would be more consistent
         # with the rest of the Emitter methods, in this case we just avoid moving any
         # machinery as much as possible, because potentially there will be huge number
         # of trace calls.
         if self._mode == EmitterMode.TRACE:
             self._printer.show(sys.stderr, text, use_timestamp=True)  # type: ignore
 
     def _get_progress_params(self, permanent: bool):
@@ -897,25 +577,41 @@
         """
         stream, use_timestamp, ephemeral = self._get_progress_params(permanent=False)
         return _Progresser(self._printer, total, text, stream, delta, use_timestamp, ephemeral)  # type: ignore
 
     @_active_guard()
     def open_stream(self, text: str):
         """Open a stream context manager to get messages from subprocesses."""
-        if self._mode in (EmitterMode.QUIET, EmitterMode.BRIEF):
-            # don't show third party streams if quiet or normal
+        if self._mode == EmitterMode.QUIET:
+            # no third party stream
             stream = None
+            ephemeral = True
+            use_timestamp = False
+        elif self._mode == EmitterMode.BRIEF:
+            stream = sys.stderr
+            ephemeral = True
             use_timestamp = False
         elif self._mode == EmitterMode.VERBOSE:
+            # third party stream to stderr
             stream = sys.stderr
+            ephemeral = False
             use_timestamp = False
         else:
+            # third party stream to stderr with timestamp
             stream = sys.stderr
+            ephemeral = False
             use_timestamp = True
-        return _StreamContextManager(self._printer, text, stream=stream, use_timestamp=use_timestamp)  # type: ignore
+        manager = _StreamContextManager(
+            self._printer,  # type: ignore
+            text,
+            stream=stream,
+            use_timestamp=use_timestamp,
+            ephemeral_mode=ephemeral,
+        )
+        return manager
 
     @_active_guard()
     @contextmanager
     def pause(self):
         """Context manager that pauses and resumes the control of the terminal.
 
         Note that no messages will be collected while paused, not even for logging.
@@ -923,15 +619,15 @@
         self.debug("Emitter: Pausing control of the terminal")
         self._printer.stop()  # type: ignore
         self._stopped = True
         try:
             yield
         finally:
             self._stopped = False
-            self._printer = _Printer(self._log_filepath)  # type: ignore
+            self._printer = self._log_handler.printer = Printer(self._log_filepath)  # type: ignore
             self.debug("Emitter: Resuming control of the terminal")
 
     def _stop(self) -> None:
         """Do all the stopping."""
         self._printer.stop()  # type: ignore
         self._stopped = True
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `craft-cli-1.2.0/craft_cli/pytest_plugin.py` & `craft-cli-2.0.0/craft_cli/pytest_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Canonical Ltd.
+# Copyright 2022-2023 Canonical Ltd.
 #
 # This program is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License version 3 as published by the Free Software Foundation.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -20,15 +20,15 @@
 import pathlib
 import re
 import tempfile
 from unittest.mock import call
 
 import pytest
 
-from craft_cli import messages
+from craft_cli import messages, printer
 
 
 @pytest.fixture(autouse=True)
 def init_emitter(monkeypatch):
     """Ensure ``emit`` is always clean, and initiated (in test mode).
 
     Note that the ``init`` is done in the current instance that all modules already
@@ -41,14 +41,15 @@
     # effect we would be polluting that temporary directory (potentially messing with
     # tests, that may need that empty), so we use another one
     temp_fd, temp_logfile = tempfile.mkstemp(prefix="emitter-logs")
     os.close(temp_fd)
     temp_logfile = pathlib.Path(temp_logfile)
 
     monkeypatch.setattr(messages, "TESTMODE", True)
+    monkeypatch.setattr(printer, "TESTMODE", True)
     messages.emit.init(
         messages.EmitterMode.QUIET, "test-emitter", "Hello world", log_filepath=temp_logfile
     )
     yield
     # end machinery (just in case it was not ended before; note it's ok to "double end")
     messages.emit.ended_ok()
     temp_logfile.unlink()
```

