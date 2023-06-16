# Comparing `tmp/click_extra-4.3.0.tar.gz` & `tmp/click_extra-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click_extra-4.3.0.tar", max compression
+gzip compressed data, was "click_extra-4.4.0.tar", max compression
```

## Comparing `click_extra-4.3.0.tar` & `click_extra-4.4.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     6143 2023-06-02 16:27:11.922412 click_extra-4.3.0/click_extra/__init__.py
--rw-r--r--   0        0        0    27870 2023-06-02 16:27:11.922412 click_extra-4.3.0/click_extra/colorize.py
--rw-r--r--   0        0        0    14959 2023-06-02 16:27:11.922412 click_extra-4.3.0/click_extra/commands.py
--rw-r--r--   0        0        0    15734 2023-06-02 16:27:11.922412 click_extra-4.3.0/click_extra/config.py
--rw-r--r--   0        0        0     3996 2023-06-02 16:27:11.922412 click_extra-4.3.0/click_extra/decorators.py
--rw-r--r--   0        0        0     6402 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/docs_update.py
--rw-r--r--   0        0        0    11542 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/logging.py
--rw-r--r--   0        0        0    22569 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/parameters.py
--rw-r--r--   0        0        0    14061 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/platforms.py
--rw-r--r--   0        0        0        0 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/py.typed
--rw-r--r--   0        0        0     7671 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/pygments.py
--rw-r--r--   0        0        0     6113 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/sphinx.py
--rw-r--r--   0        0        0     5718 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tabulate.py
--rw-r--r--   0        0        0     2534 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/telemetry.py
--rw-r--r--   0        0        0    23502 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/testing.py
--rw-r--r--   0        0        0      770 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/__init__.py
--rw-r--r--   0        0        0    11926 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/conftest.py
--rw-r--r--   0        0        0    17800 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/test_colorize.py
--rw-r--r--   0        0        0    12945 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/test_commands.py
--rw-r--r--   0        0        0    16166 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/test_config.py
--rw-r--r--   0        0        0     7238 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/test_logging.py
--rw-r--r--   0        0        0    14323 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/test_parameters.py
--rw-r--r--   0        0        0     9733 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/test_platforms.py
--rw-r--r--   0        0        0     8377 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/test_pygments.py
--rw-r--r--   0        0        0    14284 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/test_tabulate.py
--rw-r--r--   0        0        0     3153 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/test_telemetry.py
--rw-r--r--   0        0        0     8215 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/test_testing.py
--rw-r--r--   0        0        0     3530 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/test_timer.py
--rw-r--r--   0        0        0     4585 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/tests/test_version.py
--rw-r--r--   0        0        0     2385 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/timer.py
--rw-r--r--   0        0        0     7098 2023-06-02 16:27:11.926412 click_extra-4.3.0/click_extra/version.py
--rw-r--r--   0        0        0     6948 2023-06-02 16:27:11.934412 click_extra-4.3.0/pyproject.toml
--rw-r--r--   0        0        0     6640 2023-06-02 16:27:11.934412 click_extra-4.3.0/readme.md
--rw-r--r--   0        0        0     9684 1970-01-01 00:00:00.000000 click_extra-4.3.0/PKG-INFO
+-rw-r--r--   0        0        0     5977 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/__init__.py
+-rw-r--r--   0        0        0    27916 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/colorize.py
+-rw-r--r--   0        0        0    15032 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/commands.py
+-rw-r--r--   0        0        0    15847 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/config.py
+-rw-r--r--   0        0        0     4014 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/decorators.py
+-rw-r--r--   0        0        0     6262 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/docs_update.py
+-rw-r--r--   0        0        0    11581 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/logging.py
+-rw-r--r--   0        0        0    23480 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/parameters.py
+-rw-r--r--   0        0        0    17118 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/platforms.py
+-rw-r--r--   0        0        0        0 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/py.typed
+-rw-r--r--   0        0        0     7685 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/pygments.py
+-rw-r--r--   0        0        0     4969 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/sphinx.py
+-rw-r--r--   0        0        0     5733 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/tabulate.py
+-rw-r--r--   0        0        0     2542 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/telemetry.py
+-rw-r--r--   0        0        0    23592 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/testing.py
+-rw-r--r--   0        0        0      770 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/tests/__init__.py
+-rw-r--r--   0        0        0    11217 2023-06-16 05:42:43.350333 click_extra-4.4.0/click_extra/tests/conftest.py
+-rw-r--r--   0        0        0    17920 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/tests/test_colorize.py
+-rw-r--r--   0        0        0    12975 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/tests/test_commands.py
+-rw-r--r--   0        0        0    16381 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/tests/test_config.py
+-rw-r--r--   0        0        0     7290 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/tests/test_logging.py
+-rw-r--r--   0        0        0    14348 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/tests/test_parameters.py
+-rw-r--r--   0        0        0    10873 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/tests/test_platforms.py
+-rw-r--r--   0        0        0     8406 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/tests/test_pygments.py
+-rw-r--r--   0        0        0    14343 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/tests/test_tabulate.py
+-rw-r--r--   0        0        0     3165 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/tests/test_telemetry.py
+-rw-r--r--   0        0        0     8259 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/tests/test_testing.py
+-rw-r--r--   0        0        0     3551 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/tests/test_timer.py
+-rw-r--r--   0        0        0     4615 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/tests/test_version.py
+-rw-r--r--   0        0        0     2398 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/timer.py
+-rw-r--r--   0        0        0     7165 2023-06-16 05:42:43.354333 click_extra-4.4.0/click_extra/version.py
+-rw-r--r--   0        0        0     7439 2023-06-16 05:42:43.358332 click_extra-4.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6631 2023-06-16 05:42:43.358332 click_extra-4.4.0/readme.md
+-rw-r--r--   0        0        0     9675 1970-01-01 00:00:00.000000 click_extra-4.4.0/PKG-INFO
```

### Comparing `click_extra-4.3.0/click_extra/__init__.py` & `click_extra-4.4.0/click_extra/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 """Expose package-wide elements."""
 
 import sys
 
-__version__ = "4.3.0"
+__version__ = "4.4.0"
 """Examples of valid version strings according :pep:`440#version-scheme`:
 
 .. code-block:: python
 
     __version__ = "1.2.3.dev1"  # Development release 1
     __version__ = "1.2.3a1"  # Alpha Release 1
     __version__ = "1.2.3b1"  # Beta Release 1
@@ -49,60 +49,60 @@
 
 
 # Import all click's module-level content to allow for drop-in replacement.
 # XXX Star import is really badly supported by mypy for now and leads to lots of
 # "Module 'XXX' has no attribute 'YYY'". See: https://github.com/python/mypy/issues/4930
 # Overrides click helpers with cloup's.
 from click import *  # noqa: E402, F403
-from click.core import ParameterSource  # noqa: E402, F401
+from click.core import ParameterSource  # noqa: E402
 from cloup import *  # type: ignore[no-redef] # noqa: E402, F403
 
-from .colorize import (  # noqa: I001, E402, F401
+from .colorize import (  # noqa: E402
     ColorOption,
     HelpExtraFormatter,
     HelpExtraTheme,
     HelpOption,
 )
-from .commands import (  # noqa: I001, E402, F401
+from .commands import (  # noqa: E402
     ExtraCommand,
     ExtraContext,
     ExtraGroup,
 )
-from .config import ConfigOption  # noqa: I001, E402, F401
-from .decorators import (  # type: ignore[no-redef] # noqa: I001, E402, F401
+from .config import ConfigOption  # noqa: E402
+from .decorators import (  # type: ignore[no-redef] # noqa: E402
     color_option,
-    command,  # noqa: E402
+    command,
     config_option,
     extra_command,
     extra_group,
-    group,  # noqa: E402
+    group,
     help_option,
     show_params_option,
     table_format_option,
     telemetry_option,
     timer_option,
     verbosity_option,
     version_option,
 )
-from .logging import (  # noqa: I001, E402, F401
+from .logging import (  # noqa: E402
     ExtraLogFormatter,
     ExtraLogHandler,
     VerbosityOption,
     extra_basic_config,
 )
-from .parameters import (  # noqa: I001, E402, F401
+from .parameters import (  # noqa: E402
     ExtraOption,
     ParamStructure,
     ShowParamsOption,
 )
-from .tabulate import TableFormatOption  # noqa: I001, E402, F401
-from .telemetry import TelemetryOption  # noqa: I001, E402, F401
-from .testing import ExtraCliRunner  # noqa: I001, E402, F401
-from .timer import TimerOption  # noqa: I001, E402, F401
-from .version import VersionOption  # noqa: I001, E402, F401
+from .tabulate import TableFormatOption  # noqa: E402
+from .telemetry import TelemetryOption  # noqa: E402
+from .testing import ExtraCliRunner  # noqa: E402
+from .timer import TimerOption  # noqa: E402
+from .version import VersionOption  # noqa: E402
 
 __all__ = [  # noqa: F405
     "Abort",
     "Argument",
     "argument",
     "BadArgumentUsage",
     "BadOptionUsage",
```

### Comparing `click_extra-4.3.0/click_extra/colorize.py` & `click_extra-4.4.0/click_extra/colorize.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from __future__ import annotations
 
 import os
 import re
 from configparser import RawConfigParser
 from gettext import gettext as _
 from operator import getitem
-from typing import NamedTuple, Optional, Sequence, cast
+from typing import NamedTuple, Sequence, cast
 
 import click
 import regex as re3
 from boltons.strutils import complement_int_list, int_ranges_from_int_list
 from cloup._util import identity
 from cloup.styling import Color, IStyle
 from cloup.typing import MISSING, Possibly
@@ -61,15 +61,15 @@
     command_help: IStyle = identity
     heading: IStyle = identity
     constraint: IStyle = identity
     section_help: IStyle = identity
     col1: IStyle = identity
     col2: IStyle = identity
     alias: IStyle = identity
-    alias_secondary: Optional[IStyle] = None
+    alias_secondary: IStyle | None = None
     epilog: IStyle = identity
     """Set of properties inherited from ``cloup.HelpTheme``.
 
     See: https://cloup.readthedocs.io/en/stable/autoapi/cloup/index.html#cloup.HelpTheme.invoked_command
     """
 
     critical: IStyle = identity
@@ -110,15 +110,15 @@
         command_help: IStyle | None = None,
         heading: IStyle | None = None,
         constraint: IStyle | None = None,
         section_help: IStyle | None = None,
         col1: IStyle | None = None,
         col2: IStyle | None = None,
         alias: IStyle | None = None,
-        alias_secondary: Possibly[Optional[IStyle]] = MISSING,
+        alias_secondary: Possibly[IStyle | None] = MISSING,
         epilog: IStyle | None = None,
         ### Log levels.
         critical: IStyle | None = None,
         error: IStyle | None = None,
         warning: IStyle | None = None,
         info: IStyle | None = None,
         debug: IStyle | None = None,
@@ -257,15 +257,16 @@
                 # Presence of the variable in the environment without a value encodes
                 # for an activation, hence the default to True.
                 var_value = os.environ.get(var, "true")
                 # `os.environ` is a dict whose all values are strings. Here we normalize
                 # these string into booleans. If we can't, we fallback to True, in the
                 # same spirit as above.
                 var_boolean = RawConfigParser.BOOLEAN_STATES.get(
-                    var_value.lower(), True
+                    var_value.lower(),
+                    True,
                 )
                 colorize_from_env.add(default ^ (not var_boolean))
 
         # Re-interpret the provided value against the recognized environment variables.
         if colorize_from_env:
             # The environment can only override the provided value if it comes from
             # the default value or the config file.
@@ -333,15 +334,15 @@
         self,
         param_decls: Sequence[str] | None = None,
         is_flag=True,
         expose_value=False,
         is_eager=True,
         help=_("Show this message and exit."),
         **kwargs,
-    ):
+    ) -> None:
         if not param_decls:
             param_decls = ("--help", "-h")
 
         kwargs.setdefault("callback", self.print_help)
 
         super().__init__(
             param_decls=param_decls,
@@ -480,15 +481,15 @@
     - https://github.com/janluke/cloup/issues/97
     - https://github.com/click-contrib/click-help-colors/issues/17
     - https://github.com/janluke/cloup/issues/95
     """
 
     theme: HelpExtraTheme
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         """Forces theme to our default.
 
         Also transform Cloup's standard ``HelpTheme`` to our own ``HelpExtraTheme``.
         """
         theme = kwargs.get("theme", default_theme)
         if not isinstance(theme, HelpExtraTheme):
             theme = default_theme.with_(**theme._asdict())
@@ -580,18 +581,19 @@
                     txt += self.colorize_group(group_string, group_id)
             else:
                 # No named group matching this string. Leave it as-is.
                 txt += group_string
 
         # Double-check we processed all named groups.
         if len(named_matches) != 0:
-            raise ValueError(
+            msg = (
                 "The matching result contains named groups that were not processed. "
                 "There is an edge-case in the design of regular expressions."
             )
+            raise ValueError(msg)
 
         return txt
 
     def highlight_extra_keywords(self, help_text):
         """Highlight extra keywords in help screens based on the theme.
 
         It is based on regular expressions. While this is not a bullet-proof method, it
@@ -746,15 +748,15 @@
             for match in re3.finditer(part, string, flags=flags, overlapped=True)
         }
 
     # Reduce ranges, compute complement ranges, transform them to list of integers.
     ranges = ",".join(ranges)
     highlight_ranges = int_ranges_from_int_list(ranges)
     untouched_ranges = int_ranges_from_int_list(
-        complement_int_list(ranges, range_end=len(string))
+        complement_int_list(ranges, range_end=len(string)),
     )
 
     # Apply style to range of characters flagged as matching.
     styled_str = ""
     for i, j in sorted(highlight_ranges + untouched_ranges):
         segment = getitem(string, slice(i, j + 1))
         if (i, j) in highlight_ranges:
```

### Comparing `click_extra-4.3.0/click_extra/commands.py` & `click_extra-4.4.0/click_extra/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 counterparts, but are pre-configured with good and common defaults. You can still
 leverage the mixins in here to build up your own custom variants.
 """
 
 from __future__ import annotations
 
 import logging
-from typing import Any, Dict
+from typing import Any
 
 import click
 import cloup
 
 from . import Command, Group
 from .colorize import ColorOption, ExtraHelpColorsMixin, HelpOption
 from .config import ConfigOption
@@ -41,15 +41,16 @@
 )
 from .timer import TimerOption
 from .version import VersionOption
 
 
 class ExtraContext(cloup.Context):
     """Like ``cloup._context.Context``, but with the ability to populate the context's
-    ``meta`` property at instanciation."""
+    ``meta`` property at instanciation.
+    """
 
     _extra_meta: dict[str, Any] = {}
 
     def __init__(self, *args, meta: dict[str, Any] = {}, **kwargs) -> None:
         """Like parent's context but with an extra ``meta`` keyword-argument."""
         self._extra_meta = meta
         super().__init__(*args, **kwargs)
@@ -118,15 +119,15 @@
     def __init__(
         self,
         *args,
         version: str | None = None,
         extra_option_at_end: bool = True,
         populate_auto_envvars: bool = True,
         **kwargs: Any,
-    ):
+    ) -> None:
         """List of extra parameters:
 
         :param version: allows a version string to be set directly on the command. Will
             be passed to the first instance of ``VersionOption`` parameter attached to
             the command.
         :param extra_option_at_end: `reorders all parameters attached to the command
             <https://kdeldycke.github.io/click-extra/commands.html#option-order>`_, by
@@ -216,15 +217,15 @@
             )
         """
         super().__init__(*args, **kwargs)
 
         # List of additional global settings for options.
         extra_option_settings = ["show_choices", "show_envvar"]
 
-        default_ctx_settings: Dict[str, Any] = {
+        default_ctx_settings: dict[str, Any] = {
             # Click settings:
             # "default_map": {"verbosity": "DEBUG"},
             "help_option_names": ("--help", "-h"),
             "show_default": True,
             # Cloup settings:
             "align_option_groups": False,
             "show_constraints": True,
@@ -248,15 +249,15 @@
                     # These attributes are specific to options.
                     if isinstance(param, click.Option):
                         param.show_envvar = default_ctx_settings[setting]
 
         # Remove Click Extra-specific settings, before passing it to Cloup and Click.
         for setting in extra_option_settings:
             del default_ctx_settings[setting]
-        self.context_settings: Dict[str, Any] = default_ctx_settings
+        self.context_settings: dict[str, Any] = default_ctx_settings
 
         if populate_auto_envvars:
             for param in self.params:
                 param.envvar = all_envvars(param, self.context_settings)
 
         if version:
             version_param = search_params(self.params, VersionOption)
@@ -315,26 +316,30 @@
         """
         logger = logging.getLogger("click_extra")
         if logger.getEffectiveLevel() == logging.DEBUG:
             # Look for our custom version parameter.
             version_param = search_params(ctx.command.params, VersionOption)
             if version_param:
                 version_message = version_param.callback(
-                    ctx, version_param, True, capture_output=True
+                    ctx,
+                    version_param,
+                    True,
+                    capture_output=True,
                 )
                 for line in version_message.splitlines():
                     # TODO: pretty print JSON output (easier to read in bug reports)?
                     logger.debug(line)
 
         return super().invoke(ctx)
 
 
 class ExtraGroup(ExtraCommand, Group):
     """Same as ``cloup.group``, but with sane defaults and extra help screen
-    colorization."""
+    colorization.
+    """
 
     # XXX This simple override might be enough to replace the command() override below,
     # but there is a bug in click that prevents this from working:
     #   https://github.com/pallets/click/issues/2416
     #   https://github.com/pallets/click/pull/2417
     #
     # command_class = ExtraCommand
```

### Comparing `click_extra-4.3.0/click_extra/config.py` & `click_extra-4.4.0/click_extra/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,25 +89,25 @@
     def __init__(
         self,
         param_decls: Sequence[str] | None = None,
         metavar="CONFIG_PATH",
         type=STRING,
         help=_(
             "Location of the configuration file. Supports glob pattern of local "
-            "path and remote URL."
+            "path and remote URL.",
         ),
         is_eager=True,
         expose_value=False,
         formats=tuple(Formats),
         roaming=True,
         force_posix=False,
-        exclude_params=None,
+        excluded_params=None,
         strict=False,
         **kwargs,
-    ):
+    ) -> None:
         """Takes as input a glob pattern or an URL.
 
         Glob patterns must follow the syntax of `wcmatch.glob
         <https://facelessuser.github.io/wcmatch/glob/#syntax>`_.
 
         - ``is_eager`` is active by default so the config option's ``callback``
           gets the opportunity to set the ``default_map`` values before the
@@ -116,17 +116,17 @@
         - ``formats`` is the ordered list of formats that the configuration
           file will be tried to be read with. Can be a single one.
 
         - ``roaming`` and ``force_posix`` are `fed to click.get_app_dir()
           <https://click.palletsprojects.com/en/8.1.x/api/#click.get_app_dir>`_
           to setup the default configuration folder.
 
-        - ``exclude_params`` is a list of options to ignore by the
+        - ``excluded_params`` is a list of options to ignore by the
           configuration parser. Defaults to
-          ``ParamStructure.DEFAULT_EXCLUDE_PARAMS``.
+          ``ParamStructure.DEFAULT_EXCLUDED_PARAMS``.
 
         - ``strict``
             - If ``True``, raise an error if the configuration file contain
               unrecognized content.
             - If ``False``, silently ignore unsupported configuration option.
         """
         if not param_decls:
@@ -138,16 +138,16 @@
         self.formats = formats
 
         # Setup the configuration default folder.
         self.roaming = roaming
         self.force_posix = force_posix
         kwargs.setdefault("default", self.default_pattern)
 
-        if exclude_params is not None:
-            self.exclude_params = exclude_params
+        if excluded_params is not None:
+            self.excluded_params = excluded_params
 
         self.strict = strict
 
         kwargs.setdefault("callback", self.load_conf)
 
         super().__init__(
             param_decls=param_decls,
@@ -175,15 +175,15 @@
         - an expanded ``*.{ext1,ext2,...}`` pattern if multiple formats are set
         """
         ctx = get_current_context()
         cli_name = ctx.find_root().info_name
         if not cli_name:
             raise ValueError
         app_dir = Path(
-            get_app_dir(cli_name, roaming=self.roaming, force_posix=self.force_posix)
+            get_app_dir(cli_name, roaming=self.roaming, force_posix=self.force_posix),
         ).resolve()
         # Build the extension matching pattern.
         extensions = flatten(f.value for f in self.formats)
         if len(extensions) == 1:
             ext_pattern = extensions[0]
         else:
             # Use brace notation for multiple extension matching.
@@ -299,15 +299,17 @@
 
         conf = {}
         for section_id in ini_config.sections():
             # Extract all options of the section.
             sub_conf = {}
             for option_id in ini_config.options(section_id):
                 target_type = self.get_tree_value(
-                    self.params_types, section_id, option_id
+                    self.params_types,
+                    section_id,
+                    option_id,
                 )
 
                 if target_type in (None, str):
                     value = ini_config.get(section_id, option_id)
 
                 elif target_type == int:
                     value = ini_config.getint(section_id, option_id)
@@ -320,18 +322,19 @@
 
                 # Types not natively supported by INI format are loaded as
                 # JSON-serialized strings.
                 elif target_type in (list, tuple, set, frozenset, dict):
                     value = json.loads(ini_config.get(section_id, option_id))
 
                 else:
-                    raise ValueError(
+                    msg = (
                         f"Conversion of {target_type} type for "
                         f"[{section_id}]:{option_id} INI config option."
                     )
+                    raise ValueError(msg)
 
                 sub_conf[option_id] = value
 
             # Place collected options at the right level of the dict tree.
             merge(conf, self.init_tree_dict(*section_id.split(self.SEP), leaf=sub_conf))
 
         return conf
@@ -344,16 +347,17 @@
         for k, v in b.items():
             if isinstance(v, dict) and isinstance(a.get(k), dict):
                 a[k] = self.recursive_update(a[k], v)
             # Ignore elements unregistered in the template structure.
             elif k in a:
                 a[k] = b[k]
             elif self.strict:
+                msg = f"Parameter {k!r} is not allowed in configuration file."
                 raise ValueError(
-                    f"Parameter {k!r} is not allowed in configuration file."
+                    msg,
                 )
         return a
 
     def merge_conf(self, user_conf):
         """Try-out configuration formats againts file's content and returns a ``dict``.
 
         The returned ``dict`` will only contain options and parameters defined on the
@@ -422,12 +426,12 @@
 
         else:
             conf = self.merge_conf(user_conf)
             logger.debug(f"Loaded configuration: {conf}")
 
             # Merge config to the default_map.
             if ctx.default_map is None:
-                ctx.default_map = dict()
+                ctx.default_map = {}
             ctx.default_map.update(conf.get(ctx.find_root().command.name, {}))
             logger.debug(f"New defaults: {ctx.default_map}")
 
-        return path_pattern
+        return path_pattern
```

### Comparing `click_extra-4.3.0/click_extra/decorators.py` & `click_extra-4.4.0/click_extra/decorators.py`

 * *Files 9% similar despite different names*

```diff
@@ -82,18 +82,22 @@
 
 # Redefine cloup decorators to allow them to be used with or without parenthesis.
 command = decorator_factory(dec=cloup.command)
 group = decorator_factory(dec=cloup.group)
 
 # Extra command and group decorators with default options.
 extra_command = decorator_factory(
-    dec=cloup.command, cls=ExtraCommand, params=default_extra_params
+    dec=cloup.command,
+    cls=ExtraCommand,
+    params=default_extra_params,
 )
 extra_group = decorator_factory(
-    dec=cloup.group, cls=ExtraGroup, params=default_extra_params
+    dec=cloup.group,
+    cls=ExtraGroup,
+    params=default_extra_params,
 )
 
 
 # Option decorators.
 color_option = decorator_factory(dec=cloup.option, cls=ColorOption)
 config_option = decorator_factory(dec=cloup.option, cls=ConfigOption)
 help_option = decorator_factory(dec=cloup.option, cls=HelpOption)
```

### Comparing `click_extra-4.3.0/click_extra/docs_update.py` & `click_extra-4.4.0/click_extra/docs_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,38 +36,33 @@
 
 from .platforms import ALL_GROUPS, EXTRA_GROUPS, NON_OVERLAPPING_GROUPS, Group
 from .pygments import lexer_map
 from .tabulate import tabulate
 
 
 def replace_content(
-    filepath: Path, start_tag: str, end_tag: str, new_content: str
+    filepath: Path,
+    start_tag: str,
+    end_tag: str,
+    new_content: str,
 ) -> None:
     """Replace in the provided file the content surrounded by the provided tags."""
     filepath = filepath.resolve()
     assert filepath.exists(), f"File {filepath} does not exist."
     assert filepath.is_file(), f"File {filepath} is not a file."
 
     orig_content = filepath.read_text()
 
     # Extract pre- and post-content surrounding the tags.
     pre_content, table_start = orig_content.split(start_tag, 1)
     _, post_content = table_start.split(end_tag, 1)
 
     # Reconstruct the content with our updated table.
     filepath.write_text(
-        "".join(
-            (
-                pre_content,
-                start_tag,
-                new_content,
-                end_tag,
-                post_content,
-            )
-        )
+        f"{pre_content}{start_tag}{new_content}{end_tag}{post_content}",
     )
 
 
 def generate_lexer_table() -> str:
     """Generate a Markdown table mapping original Pygments' lexers to their new ANSI
     variants implemented by Click Extra."""
     table = []
@@ -77,15 +72,15 @@
     ):
         table.append(
             [
                 f"[`{orig_lexer.__qualname__}`](https://pygments.org/docs/lexers/#"
                 f"{orig_lexer.__module__}.{orig_lexer.__qualname__})",
                 f"{', '.join(f'`{a}`' for a in sorted(orig_lexer.aliases))}",
                 f"{', '.join(f'`{a}`' for a in sorted(ansi_lexer.aliases))}",
-            ]
+            ],
         )
     output = tabulate.tabulate(
         table,
         headers=[
             "Original Lexer",
             "Original IDs",
             "ANSI variants",
@@ -94,15 +89,17 @@
         colalign=["left", "left", "left"],
         disable_numparse=True,
     )
     return output
 
 
 def generate_platforms_graph(
-    graph_id: str, description: str, groups: frozenset[Group]
+    graph_id: str,
+    description: str,
+    groups: frozenset[Group],
 ) -> str:
     """Generates an `Euler diagram <https://xkcd.com/2721/>`_ of platform and their
     grouping.
 
     Euler diagrams are
     `not supported by mermaid yet <https://github.com/mermaid-js/mermaid/issues/2583>`_
     so we fallback on a flowchart without arrows.
@@ -115,36 +112,34 @@
     # Create one subgraph per group.
     for group in sorted(groups, key=lambda g: g.id):
         nodes = set()
         for platform in group:
             # Make the node ID unique for overlapping groups.
             nodes.add(
                 f"{group.id}_{platform.id}"
-                f"(<code>{platform.id}</code><br/><em>{html.escape(platform.name)}</em>)"
+                f"(<code>{platform.id}</code><br/><em>{html.escape(platform.name)}</em>)",
             )
         subgraphs.add(
-            (
-                f"subgraph <code>click_extra.platforms.{group.id.upper()}</code>"
-                "<br/>"
-                f"<em>{group.name}</em>"
-                "\n" + indent("\n".join(sorted(nodes)), INDENT) + "\nend"
-            )
+            f"subgraph <code>click_extra.platforms.{group.id.upper()}</code>"
+            "<br/>"
+            f"<em>{group.name}</em>"
+            "\n" + indent("\n".join(sorted(nodes)), INDENT) + "\nend",
         )
 
     # Wrap the Mermaid code into a MyST block.
     return "\n".join(
         (
             # Use attributes blocks extension to add a title.
             ('{caption="' f"`click_extra.platforms.{graph_id}` - {description}" '"}'),
             "```mermaid",
             ":zoom:",
             "flowchart",
             indent("\n".join(sorted(subgraphs)), INDENT),
             "```",
-        )
+        ),
     )
 
 
 def update_docs() -> None:
     """Update documentation with dynamic content."""
     project_root = Path(__file__).parent.parent
```

### Comparing `click_extra-4.3.0/click_extra/logging.py` & `click_extra-4.4.0/click_extra/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,32 +15,34 @@
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 """Logging utilities."""
 
 from __future__ import annotations
 
 import logging
 import sys
-from collections.abc import Generator, Iterable, Sequence
 from gettext import gettext as _
 from logging import (
     WARNING,
     Formatter,
     Handler,
     Logger,
     LogRecord,
     _levelToName,
 )
-from typing import Literal, TypeVar
+from typing import TYPE_CHECKING, Literal, TypeVar
 
 import click
 
 from . import Choice
 from .colorize import default_theme
 from .parameters import ExtraOption
 
+if TYPE_CHECKING:
+    from collections.abc import Generator, Iterable, Sequence
+
 _original_get_logger = logging.getLogger
 
 
 def _patched_get_logger(name: str | None = None) -> Logger:
     """Patch ``logging.getLogger`` to return the right root logger object.
 
     .. warning::
@@ -238,15 +240,15 @@
         .. danger::
             Resseting loggers is extremely important for unittests. Because they're
             global, loggers have tendency to leak and pollute their state between
             multiple test calls.
         """
         for logger in list(self.all_loggers)[::-1]:
             logging.getLogger("click_extra").debug(
-                f"Reset {logger} to {DEFAULT_LEVEL_NAME}."
+                f"Reset {logger} to {DEFAULT_LEVEL_NAME}.",
             )
             logger.setLevel(DEFAULT_LEVEL)
 
     def set_levels(self, ctx, param, value):
         """Set level of all loggers configured on the option.
 
         Also prints the chosen value as a debug message via the internal
```

### Comparing `click_extra-4.3.0/click_extra/parameters.py` & `click_extra-4.4.0/click_extra/parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import inspect
 import logging
 import re
 from collections.abc import MutableMapping
 from functools import cached_property, reduce
 from gettext import gettext as _
 from operator import getitem, methodcaller
-from typing import Any, Dict, Iterable, Sequence
+from typing import Any, Iterable, Sequence
 
 import click
 from boltons.iterutils import unique
 from mergedeep import merge
 from tabulate import tabulate
 
 from . import (
@@ -51,15 +51,16 @@
     Tuple,
     echo,
     get_current_context,
 )
 
 
 def auto_envvar(
-    param: click.Parameter, ctx: click.Context | Dict[str, Any]
+    param: click.Parameter,
+    ctx: click.Context | dict[str, Any],
 ) -> str | None:
     """Compute the auto-generated environment variable of an option or argument.
 
     Returns the auto envvar as it is exacly computed within Click's internals, i.e.
     ``click.core.Parameter.resolve_envvar_value()`` and
     ``click.core.Option.resolve_envvar_value()``.
     """
@@ -75,30 +76,28 @@
         return None
 
     # Mimicks Click's internals.
     return f"{prefix}_{param.name.upper()}"
 
 
 def extend_envvars(
-    envvars_1: str | Sequence[str] | None, envvars_2: str | Sequence[str] | None
+    envvars_1: str | Sequence[str] | None,
+    envvars_2: str | Sequence[str] | None,
 ) -> tuple[str, ...]:
     """Utility to build environment variables value to be fed to options.
 
     Variable names are deduplicated while preserving their initial order.
 
     Returns a tuple of environment variable strings. The result is ready to be used as
     the ``envvar`` parameter for options or arguments.
     """
     # Make the fist argument into a list of string.
     envvars = []
     if envvars_1:
-        if isinstance(envvars_1, str):
-            envvars = [envvars_1]
-        else:
-            envvars = list(envvars_1)
+        envvars = [envvars_1] if isinstance(envvars_1, str) else list(envvars_1)
 
     # Merge the second argument into the list.
     if envvars_2:
         if isinstance(envvars_2, str):
             envvars.append(envvars_2)
         else:
             envvars.extend(envvars_2)
@@ -109,30 +108,32 @@
 
 def normalize_envvar(envvar: str) -> str:
     """Utility to normalize an environment variable name.
 
     The normalization process separates all contiguous alphanumeric string segments,
     eliminate empty strings, join them with an underscore and uppercase the result.
     """
-    return "_".join((p for p in re.split(r"[^a-zA-Z0-9]+", envvar) if p)).upper()
+    return "_".join(p for p in re.split(r"[^a-zA-Z0-9]+", envvar) if p).upper()
 
 
 def all_envvars(
-    param: click.Parameter, ctx: click.Context | Dict[str, Any], normalize: bool = False
+    param: click.Parameter,
+    ctx: click.Context | dict[str, Any],
+    normalize: bool = False,
 ) -> tuple[str, ...]:
     """Returns the deduplicated, ordered list of environment variables for an option or
     argument, including the auto-generated one.
 
     The auto-generated environment variable is added at the end of the list, so that
     user-defined envvars takes precedence. This respects the current implementation
     of ``click.core.Option.resolve_envvar_value()``.
 
     If ``normalize`` is `True`, the returned value is normalized. By default it is
-    `False` to perfectly reproduce the
-    `current behavior of Click, which is subject to discussions <https://github.com/pallets/click/issues/2483>`_.
+    `False` to perfectly reproduce the `current behavior of Click, which is subject to
+    discussions <https://github.com/pallets/click/issues/2483>`_.
     """
     auto_envvar_id = auto_envvar(param, ctx)
     envvars = extend_envvars(param.envvar, auto_envvar_id)
 
     if normalize:
         envvars = tuple(normalize_envvar(var) for var in envvars)
 
@@ -152,18 +153,19 @@
         provided ``klass`` is found.
     """
     param_list = [p for p in params if isinstance(p, klass)]
     if not param_list:
         return None
     if unique:
         if len(param_list) != 1:
-            raise RuntimeError(
-                f"More than one {klass.__name__} parameters found "
-                f"on command: {param_list}"
+            msg = (
+                f"More than one {klass.__name__} parameters found on command: "
+                f"{param_list}"
             )
+            raise RuntimeError(msg)
         return param_list.pop()
     return param_list
 
 
 class ExtraOption(Option):
     """All new options implemented by ``click-extra`` inherits this class.
 
@@ -235,15 +237,15 @@
                 default_string = ", ".join(str(d) for d in default_value)
             elif inspect.isfunction(default_value):
                 default_string = _("(dynamic)")
             elif option.is_bool_flag and option.secondary_opts:
                 # For boolean flags that have distinct True/False opts,
                 # use the opt without prefix instead of the value.
                 default_string = click.parser.split_opt(
-                    (option.opts if option.default else option.secondary_opts)[0]
+                    (option.opts if option.default else option.secondary_opts)[0],
                 )[1]
             elif (
                 option.is_bool_flag and not option.secondary_opts and not default_value
             ):
                 default_string = ""
             else:
                 default_string = str(default_value)
@@ -257,21 +259,26 @@
 class ParamStructure:
     """Utilities to introspect CLI options and commands structure.
 
     Structures are represented by a tree-like ``dict``.
 
     Access to a node is available using a serialized path string composed of the keys to
     descend to that node, separated by a dot ``.``.
+
+    .. todo::
+        Evaluates the possibility of replacing all key-based access to the tree-like
+        structure by a `Box <https://github.com/cdgriffith/Box>`_ object, as it
+        provides lots of utilities to merge its content.
     """
 
     SEP: str = "."
     """Use a dot ``.`` as a separator between levels of the tree-like parameter
     structure."""
 
-    DEFAULT_EXCLUDE_PARAMS: Iterable[str] = (
+    DEFAULT_EXCLUDED_PARAMS: Iterable[str] = (
         "config",
         "help",
         "show_params",
         "version",
     )
     """List of root parameters to exclude from configuration by default:
 
@@ -279,28 +286,35 @@
       configuration file.
     - ``--help``, as it makes no sense to have the configurable file always
       forces a CLI to show the help and exit.
     - ``--show-params`` flag, which is like ``--help`` and stops the CLI execution.
     - ``--version``, which is not a configurable option *per-se*.
     """
 
-    def __init__(self, *args, exclude_params: Iterable[str] | None = None, **kwargs):
-        """Force the blocklist with paramerers provided by the user.
+    def __init__(
+        self,
+        *args,
+        excluded_params: Iterable[str] | None = None,
+        **kwargs,
+    ) -> None:
+        """Allow a list of paramerers to be blocked from the parameter structure.
 
-        Else, let the cached ``self.exclude_params`` property compute it.
+        If ``excluded_params`` is not provided, let the dynamic and cached
+        ``self.excluded_params`` property to compute the default value on first use.
         """
-        if exclude_params is not None:
-            self.exclude_params = exclude_params
+        if excluded_params is not None:
+            self.excluded_params = excluded_params
 
         super().__init__(*args, **kwargs)
 
     @staticmethod
     def init_tree_dict(*path: str, leaf: Any = None):
         """Utility method to recursively create a nested dict structure whose keys are
-        provided by ``path`` list and at the end is populated by a copy of ``leaf``."""
+        provided by ``path`` list and at the end is populated by a copy of ``leaf``.
+        """
 
         def dive(levels):
             if levels:
                 return {levels[0]: dive(levels[1:])}
             return leaf
 
         return dive(path)
@@ -310,37 +324,39 @@
         """Get in the ``tree_dict`` the value located at the ``path``."""
         try:
             return reduce(getitem, path, tree_dict)
         except KeyError:
             return None
 
     def _flatten_tree_dict_gen(self, tree_dict, parent_key):
-        """
-        `Source of this snippet
+        """`Source of this snippet
         <https://www.freecodecamp.org/news/how-to-flatten-a-dictionary-in-python-in-4-different-ways/>`_.
         """
         for k, v in tree_dict.items():
             new_key = f"{parent_key}{self.SEP}{k}" if parent_key else k
             if isinstance(v, MutableMapping):
                 yield from self.flatten_tree_dict(v, new_key).items()
             else:
                 yield new_key, v
 
     def flatten_tree_dict(
-        self, tree_dict: MutableMapping, parent_key: str | None = None
+        self,
+        tree_dict: MutableMapping,
+        parent_key: str | None = None,
     ):
         """Recursively traverse the tree-like ``dict`` and produce a flat ``dict`` whose
-        keys are path and values are the leaf's content."""
+        keys are path and values are the leaf's content.
+        """
         return dict(self._flatten_tree_dict_gen(tree_dict, parent_key))
 
     def walk_params(self):
         """Generates an unfiltered list of all CLI parameters.
 
-        Everything is included, from top-level to subcommands, from options to
-        arguments.
+        Everything is included, from top-level groups to subcommands, and from options
+        to arguments.
 
         Returns a 2-elements tuple:
             - the first being a tuple of keys leading to the parameter
             - the second being the parameter object itself
         """
         ctx = get_current_context()
         cli = ctx.find_root().command
@@ -354,91 +370,100 @@
             top_level_params.add(p.name)
             yield (cli.name, p.name), p
 
         # Subcommand-specific options.
         if hasattr(cli, "commands"):
             for cmd_id, cmd in cli.commands.items():
                 if cmd_id in top_level_params:
-                    raise ValueError(
+                    msg = (
                         f"{cli.name}{self.SEP}{cmd_id} subcommand conflicts with "
                         f"{top_level_params} top-level parameters"
                     )
+                    raise ValueError(msg)
 
                 for p in cmd.params:
                     yield (cli.name, cmd_id, p.name), p
 
+    TYPE_MAP = {
+        # Instances of click.types.ParamType.
+        STRING: str,
+        INT: int,
+        FLOAT: float,
+        BOOL: bool,
+        UUID: str,
+        UNPROCESSED: str,
+        # Subclasses of click.types.ParamType.
+        File: str,
+        click.Path: str,
+        Choice: str,
+        IntRange: int,
+        FloatRange: float,
+        DateTime: str,
+        Tuple: list,
+    }
+    """Mapping of Click types to their Python equivalent.
+
+    Keys can be a mix of instances or subclasses of ``click.types.ParamType``. Values
+    are expected to be simple Python types.
+
+    This mapping can be seen as a reverse of the ``click.types.convert_type()`` method.
+    """
+
     def get_param_type(self, param):
         """Get the Python type of a Click parameter.
 
         See the list of
         `custom types provided by Click <https://click.palletsprojects.com/en/8.1.x/api/?highlight=intrange#types>`_.
         """
         if param.multiple or param.nargs != 1:
             return list
 
-        if hasattr(param, "is_bool_flag") and getattr(param, "is_bool_flag"):
+        if hasattr(param, "is_bool_flag") and param.is_bool_flag:
             return bool
 
-        direct_map = {
-            STRING: str,
-            INT: int,
-            FLOAT: float,
-            BOOL: bool,
-            UUID: str,
-            UNPROCESSED: str,
-        }
-
-        for click_type, py_type in direct_map.items():
+        for click_type, py_type in self.TYPE_MAP.items():
             if param.type == click_type:
                 return py_type
-
-        instance_map = {
-            File: str,
-            click.Path: str,
-            Choice: str,
-            IntRange: int,
-            FloatRange: float,
-            DateTime: str,
-            Tuple: list,
-        }
-
-        for click_type, py_type in instance_map.items():
-            if isinstance(param.type, click_type):
+            if inspect.isclass(click_type) and isinstance(param.type, click_type):
                 return py_type
 
-        raise ValueError(
-            f"Can't guess the appropriate Python type of {param!r} parameter."
-        )
+        msg = f"Can't guess the appropriate Python type of {param!r} parameter."
+        raise ValueError(msg)
 
     @cached_property
-    def exclude_params(self) -> Iterable[str]:
+    def excluded_params(self) -> Iterable[str]:
         """List of parameter IDs to exclude from the parameter structure.
 
         Elements of this list are expected to be the fully-qualified ID of the
         parameter, i.e. the dot-separated ID that is prefixed by the CLI name.
 
-        It's been made into a property to allow for a last-minute call to the current
-        context to fetch the CLI name.
+        .. caution::
+            It is only called once to produce the list of default parameters to
+            exclude, if the user did not provided its own list to the constructor.
+
+            It was not implemented in the constructor but made as a property, to allow
+            for a just-in-time call to the current context. Without this trick we could
+            not have fetched the CLI name.
         """
         ctx = get_current_context()
         cli = ctx.find_root().command
-        return [f"{cli.name}{self.SEP}{p}" for p in self.DEFAULT_EXCLUDE_PARAMS]
+        return [f"{cli.name}{self.SEP}{p}" for p in self.DEFAULT_EXCLUDED_PARAMS]
 
     def build_param_trees(self) -> None:
         """Build all parameters tree structure in one go and cache them.
 
-        This removes parameters whose fully-qualified IDs are in the ``exclude_params``
+        This removes parameters whose fully-qualified IDs are in the ``excluded_params``
         blocklist.
         """
         template: dict[str, Any] = {}
         types: dict[str, Any] = {}
         objects: dict[str, Any] = {}
 
         for keys, param in self.walk_params():
-            if self.SEP.join(keys) in self.exclude_params:
+            if self.SEP.join(keys) in self.excluded_params:
                 continue
             merge(template, self.init_tree_dict(*keys))
             merge(types, self.init_tree_dict(*keys, leaf=self.get_param_type(param)))
             merge(objects, self.init_tree_dict(*keys, leaf=param))
 
         self.params_template = template
         self.params_types = types
@@ -500,25 +525,25 @@
     def __init__(
         self,
         param_decls: Sequence[str] | None = None,
         is_flag=True,
         expose_value=False,
         is_eager=True,
         help=_(
-            "Show all CLI parameters, their provenance, defaults and value, then exit."
+            "Show all CLI parameters, their provenance, defaults and value, then exit.",
         ),
         **kwargs,
     ) -> None:
         if not param_decls:
             param_decls = ("--show-params",)
 
         kwargs.setdefault("callback", self.print_params)
 
-        # Deactivate blocking of any parameter.
-        self.exclude_params = ()
+        self.excluded_params = ()
+        """Deactivates the blocking of any parameter."""
 
         super().__init__(
             param_decls=param_decls,
             is_flag=is_flag,
             expose_value=expose_value,
             is_eager=is_eager,
             help=help,
@@ -565,15 +590,15 @@
 
             get_param_value = methodcaller("consume_value", ctx, opts)
 
         else:
             logger.debug(f"click_extra.raw_args not in {ctx.meta}")
             logger.warning(
                 f"Cannot extract parameters values: "
-                f"{ctx.command} does not inherits from ExtraCommand."
+                f"{ctx.command} does not inherits from ExtraCommand.",
             )
 
             def vanilla_getter(param):
                 param_value = None
                 source = ctx.get_parameter_source(param.name)
                 return param_value, source
 
@@ -592,18 +617,15 @@
             param_value, source = get_param_value(param)
             param_class = self.get_tree_value(self.params_objects, *tree_keys).__class__
             param_spec = param.get_help_record(ctx)[0]
 
             # Check if the parameter is allowed in the configuration file.
             allowed_in_conf = None
             if config_option:
-                if path in config_option.exclude_params:
-                    allowed_in_conf = KO
-                else:
-                    allowed_in_conf = OK
+                allowed_in_conf = KO if path in config_option.excluded_params else OK
 
             line = (
                 default_theme.invoked_command(path),
                 f"{param_class.__module__}.{param_class.__qualname__}",
                 param_spec,
                 param_type.__name__,
                 allowed_in_conf,
@@ -632,8 +654,8 @@
             disable_numparse=True,
         )
         echo(output, color=ctx.color)
 
         # Do not just ctx.exit() as it will prevent callbacks defined on options
         # to be called.
         ctx.close()
-        ctx.exit()
+        ctx.exit()
```

### Comparing `click_extra-4.3.0/click_extra/platforms.py` & `click_extra-4.4.0/click_extra/platforms.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 """
 
 from __future__ import annotations
 
 import platform
 import sys
 from dataclasses import dataclass, field
+from itertools import combinations
 from typing import Iterable
 
 from . import cache
 
 """ Below is the collection of heuristics used to identify each platform.
 
 All these heuristics can be hard-cached as the underlying system is not suppose to
@@ -231,27 +232,31 @@
 
     icon: str | None = field(repr=False, default=None)
     """Optional icon of the group."""
 
     def __post_init__(self):
         """Keep the platforms sorted by IDs."""
         object.__setattr__(
-            self, "platforms", tuple(sorted(self.platforms, key=lambda p: p.id))
+            self,
+            "platforms",
+            tuple(sorted(self.platforms, key=lambda p: p.id)),
         )
         object.__setattr__(
-            self, "platform_ids", frozenset({p.id for p in self.platforms})
+            self,
+            "platform_ids",
+            frozenset({p.id for p in self.platforms}),
         )
         # Double-check there is no duplicate platforms.
         assert len(self.platforms) == len(self.platform_ids)
 
     def __iter__(self):
         """Iterate over the platforms of the group."""
         yield from self.platforms
 
-    def __len__(self):
+    def __len__(self) -> int:
         """Return the number of platforms in the group."""
         return len(self.platforms)
 
     @staticmethod
     def _extract_platform_ids(other: Group | Iterable[Platform]) -> frozenset[str]:
         """Extract the platform IDs from ``other``."""
         if isinstance(other, Group):
@@ -275,15 +280,15 @@
 
     def issuperset(self, other: Group | Iterable[Platform]) -> bool:
         return self.platform_ids.issuperset(self._extract_platform_ids(other))
 
 
 ALL_PLATFORMS: Group = Group(
     "all_platforms",
-    "All platforms",
+    "Any platforms",
     (
         AIX,
         CYGWIN,
         FREEBSD,
         HURD,
         LINUX,
         MACOS,
@@ -295,38 +300,38 @@
         WSL1,
         WSL2,
     ),
 )
 """All recognized platforms."""
 
 
-ALL_WINDOWS = Group("all_windows", "All Windows", (WINDOWS,))
+ALL_WINDOWS = Group("all_windows", "Any Windows", (WINDOWS,))
 """All Windows operating systems."""
 
 
 UNIX = Group(
     "unix",
-    "All Unix",
+    "Any Unix",
     tuple(p for p in ALL_PLATFORMS.platforms if p not in ALL_WINDOWS),
 )
 """All Unix-like operating systems and compatibility layers."""
 
 
 UNIX_WITHOUT_MACOS = Group(
     "unix_without_macos",
-    "All Unix without macOS",
+    "Any Unix but macOS",
     tuple(p for p in UNIX if p is not MACOS),
 )
 """All Unix platforms, without macOS.
 
 This is useful to avoid macOS-specific workarounds on Unix platforms.
 """
 
 
-BSD = Group("bsd", "All BSD", (FREEBSD, MACOS, NETBSD, OPENBSD, SUNOS))
+BSD = Group("bsd", "Any BSD", (FREEBSD, MACOS, NETBSD, OPENBSD, SUNOS))
 """All BSD platforms.
 
 .. note::
     Are considered of this family (`according Wikipedia
     <https://en.wikipedia.org/wiki/Template:Unix>`_):
 
     - `386BSD` (`FreeBSD`, `NetBSD`, `OpenBSD`, `DragonFly BSD`)
@@ -335,48 +340,48 @@
     - `SunOS`
     - `Ultrix`
 """
 
 
 BSD_WITHOUT_MACOS = Group(
     "bsd_without_macos",
-    "All BSD without macOS",
+    "Any BSD but macOS",
     tuple(p for p in BSD if p is not MACOS),
 )
 """All BSD platforms, without macOS.
 
 This is useful to avoid macOS-specific workarounds on BSD platforms.
 """
 
 
-ALL_LINUX = Group("all_linux", "All Linux", (LINUX,))
+ALL_LINUX = Group("all_linux", "Any Linux", (LINUX,))
 """All Unix platforms based on a Linux kernel.
 
 .. note::
     Are considered of this family (`according Wikipedia
     <https://en.wikipedia.org/wiki/Template:Unix>`_):
 
     - `Android`
     - `ChromeOS`
     - any other distribution
 """
 
 
-LINUX_LAYERS = Group("linux_layers", "All Linux compatibility layers", (WSL1, WSL2))
+LINUX_LAYERS = Group("linux_layers", "Any Linux compatibility layers", (WSL1, WSL2))
 """Interfaces that allows Linux binaries to run on a different host system.
 
 .. note::
     Are considered of this family (`according Wikipedia
     <https://en.wikipedia.org/wiki/Template:Unix>`_):
 
     - `Windows Subsystem for Linux`
 """
 
 
-SYSTEM_V = Group("system_v", "All Unix derived from AT&T System Five", (AIX, SOLARIS))
+SYSTEM_V = Group("system_v", "Any Unix derived from AT&T System Five", (AIX, SOLARIS))
 """All Unix platforms derived from AT&T System Five.
 
 .. note::
     Are considered of this family (`according Wikipedia
     <https://en.wikipedia.org/wiki/Template:Unix>`_):
 
     - `A/UX`
@@ -389,15 +394,15 @@
     - `Illumos`
     - `Tru64`
     - `UNIX`
     - `UnixWare`
 """
 
 
-UNIX_LAYERS = Group("unix_layers", "All Unix compatibility layers", (CYGWIN,))
+UNIX_LAYERS = Group("unix_layers", "Any Unix compatibility layers", (CYGWIN,))
 """Interfaces that allows Unix binaries to run on a different host system.
 
 .. note::
     Are considered of this family (`according Wikipedia
     <https://en.wikipedia.org/wiki/Template:Unix>`_):
 
     - `Cygwin`
@@ -415,15 +420,15 @@
     - `UserLAnd Technologies`
     - `Windows Services for UNIX`
 """
 
 
 OTHER_UNIX = Group(
     "other_unix",
-    "All other Unix",
+    "Any other Unix",
     tuple(
         p
         for p in UNIX
         if p
         not in (
             BSD.platforms
             + ALL_LINUX.platforms
@@ -459,38 +464,109 @@
         ALL_WINDOWS,
         BSD,
         ALL_LINUX,
         LINUX_LAYERS,
         SYSTEM_V,
         UNIX_LAYERS,
         OTHER_UNIX,
-    )
+    ),
 )
 """Non-overlapping groups."""
 
 
 EXTRA_GROUPS: frozenset[Group] = frozenset(
     (
         ALL_PLATFORMS,
         UNIX,
         UNIX_WITHOUT_MACOS,
         BSD_WITHOUT_MACOS,
-    )
+    ),
 )
 """Overlapping groups, defined for convenience."""
 
 
 ALL_GROUPS: frozenset[Group] = frozenset(NON_OVERLAPPING_GROUPS | EXTRA_GROUPS)
 """All groups."""
 
 
 ALL_OS_LABELS: frozenset[str] = frozenset(p.name for p in ALL_PLATFORMS.platforms)
 """Sets of all recognized labels."""
 
 
+def reduce(items: Iterable[Group | Platform]) -> set[Group | Platform]:
+    """Reduce a collection of ``Group`` and ``Platform`` to a minimal set.
+
+    Returns a deduplicated set of ``Group`` and ``Platform`` that covers the same exact
+    platforms as the original input, but group as much platforms as possible, to reduce
+    the number of items.
+
+    .. hint::
+        Maybe this could be solved with some `Euler diagram
+        <https://en.wikipedia.org/wiki/Euler_diagram>`_ algorithms, like those
+        implemented in `eule <https://github.com/trouchet/eule>`_.
+    """
+    # Collect all platforms.
+    platforms: set[Platform] = set()
+    for item in items:
+        if isinstance(item, Group):
+            platforms.update(item.platforms)
+        else:
+            platforms.add(item)
+
+    # List any group matching the platforms.
+    valid_groups: set[Group] = set()
+    for group in ALL_GROUPS:
+        if group.issubset(platforms):
+            valid_groups.add(group)
+
+    # Test all combination of groups to find the smallest set of groups + platforms.
+    min_items: int = 0
+    results: list[set[Group | Platform]] = []
+    # Serialize group sets for deterministic lookups. Sort them by platform count.
+    groups = tuple(sorted(valid_groups, key=len, reverse=True))
+    for subset_size in range(1, len(groups) + 1):
+        # If we already have a solution that involves less items than the current
+        # subset of groups we're going to evaluates, there is no point in continuing.
+        if min_items and subset_size > min_items:
+            break
+
+        for group_subset in combinations(groups, subset_size):
+            # If any group overlaps another, there is no point in exploring this subset.
+            if not all(g[0].isdisjoint(g[1]) for g in combinations(group_subset, 2)):
+                continue
+
+            # Remove all platforms covered by the groups.
+            ungrouped_platforms = platforms.copy()
+            for group in group_subset:
+                ungrouped_platforms.difference_update(group.platforms)
+
+            # Merge the groups and the remaining platforms.
+            reduction = ungrouped_platforms.union(group_subset)
+            reduction_size = len(reduction)
+
+            # Reset the results if we have a new solution that is better than the
+            # previous ones.
+            if not results or reduction_size < min_items:
+                results = [reduction]
+                min_items = reduction_size
+            # If the solution is as good as the previous one, add it to the results.
+            elif reduction_size == min_items:
+                results.append(reduction)
+
+    if len(results) > 1:
+        msg = f"Multiple solutions found: {results}"
+        raise RuntimeError(msg)
+
+    # If no reduceted solution was found, return the original platforms.
+    if not results:
+        return platforms  # type: ignore[return-value]
+
+    return results.pop()
+
+
 @cache
 def os_label(os_id: str) -> str | None:
     """Return platform label for user-friendly output."""
     for p in ALL_PLATFORMS.platforms:
         if p.id == os_id:
             return p.name
     return None
@@ -501,21 +577,23 @@
     """Return the current platform."""
     matching = []
     for p in ALL_PLATFORMS.platforms:
         if p.current:
             matching.append(p)
 
     if len(matching) > 1:
-        raise RuntimeError(f"Multiple platforms match current OS: {matching}")
+        msg = f"Multiple platforms match current OS: {matching}"
+        raise RuntimeError(msg)
 
     if not matching:
-        raise SystemError(
+        msg = (
             f"Unrecognized {sys.platform} / "
             f"{platform.platform(aliased=True, terse=True)} platform."
         )
+        raise SystemError(msg)
 
     assert len(matching) == 1
     return matching.pop()
 
 
 CURRENT_OS_ID: str = current_os().id
 CURRENT_OS_LABEL: str = current_os().name
```

### Comparing `click_extra-4.3.0/click_extra/pygments.py` & `click_extra-4.4.0/click_extra/pygments.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,29 +49,30 @@
 We defaults to ``Generic.Output`` tokens, as this is the token type used by all REPL-
 like and terminal lexers.
 """
 
 
 class AnsiFilter(Filter):
     """Custom filter transforming a particular kind of token (``Generic.Output`` by
-    defaults) into ANSI tokens."""
+    defaults) into ANSI tokens.
+    """
 
     def __init__(self, **options) -> None:
         """Initialize a ``AnsiColorLexer`` and configure the ``token_type`` to be
         colorized.
 
         .. todo::
 
             Allow multiple ``token_type`` to be configured for colorization (if
             traditions are changed on Pygments' side).
         """
         super().__init__(**options)
         self.ansi_lexer = AnsiColorLexer()
         self.token_type = string_to_tokentype(
-            options.get("token_type", DEFAULT_TOKEN_TYPE)
+            options.get("token_type", DEFAULT_TOKEN_TYPE),
         )
 
     def filter(self, lexer, stream):
         """Transform each token of ``token_type`` type into a stream of ANSI tokens."""
         for ttype, value in stream:
             if ttype == self.token_type:
                 # TODO: Should we re-wrap the resulting list of token into their
@@ -167,15 +168,15 @@
     `Adds support for ANSI 256 colors
     <https://github.com/chriskuehl/pygments-ansi-color#optional-enable-256-color-support>`_.
     """
 
     name = "ANSI HTML"
     aliases = ["ansi-html"]
 
-    def __init__(self, **kwargs):
+    def __init__(self, **kwargs) -> None:
         """Intercept the ``style`` argument to augment it with ANSI colors support.
 
         Creates a new style instance that inherits from the one provided by the user,
         but updates its ``styles`` attribute to add ANSI colors support from
         ``pygments_ansi_color``.
         """
         # XXX Same default style as in Pygments' HtmlFormatter, which is... `default`:
```

### Comparing `click_extra-4.3.0/click_extra/sphinx.py` & `click_extra-4.4.0/click_extra/sphinx.py`

 * *Files 16% similar despite different names*

```diff
@@ -53,49 +53,20 @@
     Fix the need to have both ``.. click:example::`` and ``.. click:run::`` directives
     in the same ``{eval-rst}`` block in MyST. This is required to have both directives
     shares states and context.
 """
 
 from __future__ import annotations
 
-from unittest.mock import patch
-
-import click
 from docutils.statemachine import ViewList
 from sphinx.highlighting import PygmentsBridge
 
 from .pygments import AnsiHtmlFormatter
 from .tests.conftest import ExtraCliRunner
 
-click_compat_hack = patch.object(
-    click._compat, "text_type", create=True, return_value=str
-)
-"""Workaround for ``pallets-sphinx-themes``'s outdated reference to old ``click``'s
-Python 2 compatibility hack.
-
-Emulates:
-    .. code-block:: python
-
-        import click._compat
-
-        click._compat.text_type = str
-
-.. hint::
-    A fix has been proposed upstream at
-    `pallets-sphinx-themes#69 <https://github.com/pallets/pallets-sphinx-themes/pull/69>`_
-    and is waiting for a merge.
-
-.. seealso::
-    - `similar hack in click 8.x's docs/conf.py
-      <https://github.com/pallets/click/commit/00883dd3d0a29f68f375cab5e21cef0669941aba#diff-85933aa74a2d66c3e4dcdf7a9ad8397f5a7971080d34ef1108296a7c6b69e7e3>`_
-
-    - `incriminating import in pallets_sphinx_themes
-      <https://github.com/pallets/pallets-sphinx-themes/blob/7b69241/src/pallets_sphinx_themes/themes/click/domain.py#L9>`_
-"""
-
 
 class PatchedViewList(ViewList):
     """Force the rendering of ANSI shell session.
 
     Replaces the ``.. sourcecode:: shell-session`` code block produced by
     ``.. click:run::`` directive with an ANSI Shell Session:
     ``.. code-block:: ansi-shell-session``.
@@ -126,36 +97,32 @@
 
     .. danger::
         This function activates lots of monkey-patches:
 
         - ``sphinx.highlighting.PygmentsBridge`` is updated to set its default HTML
           formatter to an ANSI capable one for the whole Sphinx app.
 
-        - ``click_compat_hack`` to `bypass old Python 2.x in pallets-sphinx-themes
-          <#click_extra.sphinx.click_compat_hack>`.
-
         - ``pallets_sphinx_themes.themes.click.domain.ViewList`` is
           `patched to force an ANSI lexer on the rST code block
           <#click_extra.sphinx.PatchedViewList>`_.
 
         - ``pallets_sphinx_themes.themes.click.domain.ExampleRunner`` is replaced with
           ``click_extra.testing.ExtraCliRunner`` to have full control of
           contextual color settings by the way of the ``color`` parameter. It also
           produce unfiltered ANSI codes so that the other ``PatchedViewList``
           monkey-patch can do its job and render colors in the HTML output.
     """
     # Set Sphinx's default HTML formatter to an ANSI capable one.
     PygmentsBridge.html_formatter = AnsiHtmlFormatter
 
-    with click_compat_hack:
-        from pallets_sphinx_themes.themes.click import domain
+    from pallets_sphinx_themes.themes.click import domain
 
-        domain.ViewList = PatchedViewList
+    domain.ViewList = PatchedViewList
 
-        # Brutal, but effective.
-        # Alternative patching methods: https://stackoverflow.com/a/38928265
-        domain.ExampleRunner.__bases__ = (ExtraCliRunner,)
-        # Force color rendering in ``invoke`` calls.
-        domain.ExampleRunner.force_color = True
+    # Brutal, but effective.
+    # Alternative patching methods: https://stackoverflow.com/a/38928265
+    domain.ExampleRunner.__bases__ = (ExtraCliRunner,)
+    # Force color rendering in ``invoke`` calls.
+    domain.ExampleRunner.force_color = True
 
-        # Register directives to Sphinx.
-        domain.setup(app)
+    # Register directives to Sphinx.
+    domain.setup(app)
```

### Comparing `click_extra-4.3.0/click_extra/tabulate.py` & `click_extra-4.4.0/click_extra/tabulate.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             linebetweenrows=None,
             linebelow=None,
             headerrow=DataRow("| ", " | ", " |"),
             datarow=DataRow("| ", " | ", " |"),
             padding=0,
             with_header_hide=["lineabove"],
         ),
-    }
+    },
 )
 """Tweak table separators to match MyST and GFM syntax.
 
 I.e. add a space between the column separator and the dashes filling a cell:
 
 ``|---|---|---|`` → ``| --- | --- | --- |``
 
@@ -62,15 +62,15 @@
 
 output_formats: list[str] = sorted(
     # Formats from tabulate.
     list(tabulate._table_formats)  # type: ignore[attr-defined]
     # Formats inherited from previous legacy cli-helpers dependency.
     + ["csv", "vertical"]
     # Formats derived from CSV dialects.
-    + [f"csv-{d}" for d in csv.list_dialects()]
+    + [f"csv-{d}" for d in csv.list_dialects()],
 )
 """All output formats supported by click-extra."""
 
 
 def get_csv_dialect(format_id: str) -> str | None:
     """Extract, validate and normalize CSV dialect ID from format."""
     assert format_id.startswith("csv")
@@ -118,15 +118,16 @@
     }
     defaults.update(kwargs)
     echo(tabulate.tabulate(tabular_data, headers, **defaults))
 
 
 class TableFormatOption(ExtraOption):
     """A pre-configured option that is adding a ``-t``/``--table-format`` flag to select
-    the rendering style of a table."""
+    the rendering style of a table.
+    """
 
     def init_formatter(self, ctx, param, value):
         """Save table format ID in the context, and attach ``print_table()`` method to
         it.
 
         ``print_table(tabular_data, headers)`` is a ready-to-use method that takes a
         2-dimentional ``tabular_data`` iterable of iterables and a list of headers.
@@ -146,15 +147,15 @@
         self,
         param_decls: Sequence[str] | None = None,
         type=Choice(output_formats, case_sensitive=False),
         default="rounded_outline",
         expose_value=False,
         help=_("Rendering style of tables."),
         **kwargs,
-    ):
+    ) -> None:
         if not param_decls:
             param_decls = ("-t", "--table-format")
 
         kwargs.setdefault("callback", self.init_formatter)
 
         super().__init__(
             param_decls=param_decls,
```

### Comparing `click_extra-4.3.0/click_extra/telemetry.py` & `click_extra-4.4.0/click_extra/telemetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         param_decls: Sequence[str] | None = None,
         default=False,
         expose_value=False,
         envvar=None,
         show_envvar=True,
         help=_("Collect telemetry and usage data."),
         **kwargs,
-    ):
+    ) -> None:
         if not param_decls:
             param_decls = ("--telemetry/--no-telemetry",)
 
         envvar = extend_envvars(["DO_NOT_TRACK"], envvar)
 
         kwargs.setdefault("callback", self.save_telemetry)
```

### Comparing `click_extra-4.3.0/click_extra/testing.py` & `click_extra-4.4.0/click_extra/testing.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,28 +24,26 @@
 import shlex
 import subprocess
 import sys
 from contextlib import nullcontext
 from functools import partial
 from pathlib import Path
 from textwrap import indent
-from types import TracebackType
 from typing import (
     IO,
+    TYPE_CHECKING,
     Any,
     BinaryIO,
     ContextManager,
     Iterable,
     Iterator,
     Literal,
     Mapping,
     Optional,
     Sequence,
-    Tuple,
-    Type,
     Union,
     cast,
 )
 from unittest.mock import patch
 
 import click
 import click.testing
@@ -53,14 +51,17 @@
 from boltons.strutils import strip_ansi
 from boltons.tbutils import ExceptionInfo
 from click import formatting, termui, utils
 
 from . import Color, Style
 from .colorize import default_theme
 
+if TYPE_CHECKING:
+    from types import TracebackType
+
 PROMPT = "► "
 INDENT = " " * len(PROMPT)
 """Constants for rendering of CLI execution."""
 
 
 EnvVars = Mapping[str, Optional[str]]
 """Type for ``dict``-like environment variables."""
@@ -87,26 +88,26 @@
 
 
 def format_cli_prompt(cmd_args: Iterable[str], extra_env: EnvVars | None = None) -> str:
     """Simulate the console prompt used to invoke the CLI."""
     extra_env_string = ""
     if extra_env:
         extra_env_string = default_theme.envvar(
-            "".join(f"{k}={v} " for k, v in extra_env.items())
+            "".join(f"{k}={v} " for k, v in extra_env.items()),
         )
 
     cmd_str = default_theme.invoked_command(" ".join(cmd_args))
 
     return f"{PROMPT}{extra_env_string}{cmd_str}"
 
 
 def print_cli_run(
     args: Iterable[str],
     result: click.testing.Result | subprocess.CompletedProcess,
-    env: EnvVars | None = None
+    env: EnvVars | None = None,
 ) -> None:
     """Prints the full simulation of CLI execution, including output.
 
     Mostly used to print debug traces to user or in test results.
     """
     prompt = format_cli_prompt(args, env)
     stdout = ""
@@ -123,17 +124,14 @@
             output = result.output
 
     elif isinstance(result, subprocess.CompletedProcess):
         stdout = result.stdout
         stderr = result.stderr
         exit_code = result.returncode
 
-    else:
-        raise TypeError(f"Unknown result type: {type(result)}")
-
     # Render the execution trace.
     print()
     print(prompt)
     if output:
         print(f"{PROMPT}{Style(fg=Color.blue)('<output>')} stream:")
         print(indent(output, INDENT))
     if stdout:
@@ -170,15 +168,15 @@
         env_copy.update(extend)
     return env_copy
 
 
 def run_cmd(
     *args: str,
     extra_env: EnvVars | None = None,
-    print_output: bool = True
+    print_output: bool = True,
 ) -> tuple[int, str, str]:
     """Run a system command, print output and return results."""
     result = subprocess.run(
         args,
         capture_output=True,
         encoding="utf-8",
         env=cast("subprocess._ENV", env_copy(extra_env)),
@@ -255,26 +253,25 @@
         <https://github.com/pallets/click/pull/2523>`_ but has not been merged yet.
     """
 
     stderr_bytes: bytes
     """Makes ``stderr_bytes`` mandatory."""
 
     def __init__(
-            self,
-            runner: click.testing.CliRunner,
-            stdout_bytes: bytes,
-            stderr_bytes: bytes,
-            output_bytes: bytes,
-            return_value: Any,
-            exit_code: int,
-            exception: Optional[BaseException],
-            exc_info: Optional[
-                Tuple[Type[BaseException], BaseException, TracebackType]
-            ] = None,
-    ):
+        self,
+        runner: click.testing.CliRunner,
+        stdout_bytes: bytes,
+        stderr_bytes: bytes,
+        output_bytes: bytes,
+        return_value: Any,
+        exit_code: int,
+        exception: BaseException | None,
+        exc_info: tuple[type[BaseException], BaseException, TracebackType]
+        | None = None,
+    ) -> None:
         """Same as original but adds ``output_bytes`` parameter.
 
         Also makes ``stderr_bytes`` mandatory.
         """
         self.output_bytes = output_bytes
         super().__init__(
             runner=runner,
@@ -292,27 +289,29 @@
 
         .. caution::
             Contrary to original ``click.testing.Result.output``, it is not a proxy for
             ``self.stdout``. It now possess its own stream to mix ``<stdout>`` and
             ``<stderr>`` depending on the ``mix_stderr`` value.
         """
         return self.output_bytes.decode(self.runner.charset, "replace").replace(
-            "\r\n", "\n"
+            "\r\n",
+            "\n",
         )
 
     @property
     def stderr(self) -> str:
         """The standard error as unicode string.
 
         .. caution::
             Contrary to original ``click.testing.Result.stderr``, it no longer raise an
             exception, and always returns the ``<stderr>`` string.
         """
         return self.stderr_bytes.decode(self.runner.charset, "replace").replace(
-            "\r\n", "\n"
+            "\r\n",
+            "\n",
         )
 
 
 class ExtraCliRunner(click.testing.CliRunner):
     """Augment ``click.testing.CliRunner`` with extra features and bug fixes."""
 
     force_color: bool = False
@@ -324,30 +323,33 @@
         was the only way we found, as to patch some code we had to operate at the class
         level.
     """
 
     @contextlib.contextmanager
     def isolation(  # type: ignore[override]
         self,
-        input: Optional[Union[str, bytes, IO[Any]]] = None,
-        env: Optional[Mapping[str, Optional[str]]] = None,
+        input: str | bytes | IO[Any] | None = None,
+        env: Mapping[str, str | None] | None = None,
         color: bool = False,
-    ) -> Iterator[Tuple[io.BytesIO, io.BytesIO, io.BytesIO]]:
+    ) -> Iterator[tuple[io.BytesIO, io.BytesIO, io.BytesIO]]:
         """Copy of ``click.testing.CliRunner.isolation()`` with extra features.
 
         - An additional output stream is returned, which is a mix of ``<stdout>`` and
           ``<stderr>`` streams if ``mix_stderr=True``.
 
         - Always returns the ``<stderr>`` stream.
 
         .. caution::
             This is a hard-copy of the modified ``isolation()`` method `from click#2523
             PR
             <https://github.com/pallets/click/pull/2523/files#diff-b07fd6fad9f9ea8be5cbcbeaf34c956703b929b2de95c56229e77c328a7c6010>`_
             which has not been merged upstream yet.
+
+        .. todo::
+            Reduce the code duplication here by using clever monkeypatching?
         """
         bytes_input = click.testing.make_input_stream(input, self.charset)
         echo_input = None
 
         old_stdin = sys.stdin
         old_stdout = sys.stdout
         old_stderr = sys.stderr
@@ -356,48 +358,55 @@
 
         env = self.make_env(env)
 
         stream_mixer = StreamMixer(mix_stderr=self.mix_stderr)
 
         if self.echo_stdin:
             bytes_input = echo_input = cast(
-                BinaryIO, click.testing.EchoingStdin(bytes_input, stream_mixer.stdout)
+                BinaryIO,
+                click.testing.EchoingStdin(bytes_input, stream_mixer.stdout),
             )
 
         sys.stdin = text_input = click.testing._NamedTextIOWrapper(
-            bytes_input, encoding=self.charset, name="<stdin>", mode="r"
+            bytes_input,
+            encoding=self.charset,
+            name="<stdin>",
+            mode="r",
         )
 
         if self.echo_stdin:
             # Force unbuffered reads, otherwise TextIOWrapper reads a
             # large chunk which is echoed early.
             text_input._CHUNK_SIZE = 1  # type: ignore
 
         sys.stdout = click.testing._NamedTextIOWrapper(
-            stream_mixer.stdout, encoding=self.charset, name="<stdout>", mode="w"
+            stream_mixer.stdout,
+            encoding=self.charset,
+            name="<stdout>",
+            mode="w",
         )
 
         sys.stderr = click.testing._NamedTextIOWrapper(
             stream_mixer.stderr,
             encoding=self.charset,
             name="<stderr>",
             mode="w",
             errors="backslashreplace",
         )
 
         @click.testing._pause_echo(echo_input)  # type: ignore[arg-type]
-        def visible_input(prompt: Optional[str] = None) -> str:
+        def visible_input(prompt: str | None = None) -> str:
             sys.stdout.write(prompt or "")
             val = text_input.readline().rstrip("\r\n")
             sys.stdout.write(f"{val}\n")
             sys.stdout.flush()
             return val
 
         @click.testing._pause_echo(echo_input)  # type: ignore[arg-type]
-        def hidden_input(prompt: Optional[str] = None) -> str:
+        def hidden_input(prompt: str | None = None) -> str:
             sys.stdout.write(f"{prompt or ''}\n")
             sys.stdout.flush()
             return text_input.readline().rstrip("\r\n")
 
         @click.testing._pause_echo(echo_input)  # type: ignore[arg-type]
         def _getchar(echo: bool) -> str:
             char = sys.stdin.read(1)
@@ -407,15 +416,16 @@
 
             sys.stdout.flush()
             return char
 
         default_color = color
 
         def should_strip_ansi(
-            stream: Optional[IO[Any]] = None, color: Optional[bool] = None
+            stream: IO[Any] | None = None,
+            color: bool | None = None,
         ) -> bool:
             if color is None:
                 return not default_color
             return not color
 
         old_visible_prompt_func = termui.visible_prompt_func
         old_hidden_prompt_func = termui.hidden_prompt_func
@@ -427,60 +437,61 @@
         utils.should_strip_ansi = should_strip_ansi
 
         old_env = {}
         try:
             for key, value in env.items():
                 old_env[key] = os.environ.get(key)
                 if value is None:
-                    try:
+                    with contextlib.suppress(Exception):
                         del os.environ[key]
-                    except Exception:
-                        pass
+
                 else:
                     os.environ[key] = value
             yield (stream_mixer.stdout, stream_mixer.stderr, stream_mixer.output)
         finally:
             for key, value in old_env.items():
                 if value is None:
-                    try:
+                    with contextlib.suppress(Exception):
                         del os.environ[key]
-                    except Exception:
-                        pass
+
                 else:
                     os.environ[key] = value
             sys.stdout = old_stdout
             sys.stderr = old_stderr
             sys.stdin = old_stdin
             termui.visible_prompt_func = old_visible_prompt_func
             termui.hidden_prompt_func = old_hidden_prompt_func
             termui._getchar = old__getchar_func
             utils.should_strip_ansi = old_should_strip_ansi
             formatting.FORCED_WIDTH = old_forced_width
 
     def invoke2(
         self,
         cli: click.core.BaseCommand,
-        args: Optional[Union[str, Sequence[str]]] = None,
-        input: Optional[Union[str, bytes, IO[Any]]] = None,
-        env: Optional[Mapping[str, Optional[str]]] = None,
+        args: str | Sequence[str] | None = None,
+        input: str | bytes | IO[Any] | None = None,
+        env: Mapping[str, str | None] | None = None,
         catch_exceptions: bool = True,
         color: bool = False,
         **extra: Any,
     ) -> ExtraResult:
         """Copy of ``click.testing.CliRunner.invoke()`` with extra ``<output>`` stream.
 
         .. caution::
             This is a hard-copy of the modified ``invoke()`` method `from click#2523 PR
             <https://github.com/pallets/click/pull/2523/files#diff-b07fd6fad9f9ea8be5cbcbeaf34c956703b929b2de95c56229e77c328a7c6010>`_
             which has not been merged upstream yet.
+
+        .. todo::
+            Reduce the code duplication here by using clever monkeypatching?
         """
         exc_info = None
         with self.isolation(input=input, env=env, color=color) as outstreams:
             return_value = None
-            exception: Optional[BaseException] = None
+            exception: BaseException | None = None
             exit_code = 0
 
             if isinstance(args, str):
                 args = shlex.split(args)
 
             try:
                 prog_name = extra.pop("prog_name")
@@ -525,15 +536,14 @@
             output_bytes=output,
             return_value=return_value,
             exit_code=exit_code,
             exception=exception,
             exc_info=exc_info,  # type: ignore
         )
 
-
     def invoke(  # type: ignore[override]
         self,
         cli: click.core.BaseCommand,
         *args: Arg | NestedArgs,
         input: str | bytes | IO | None = None,
         env: EnvVars | None = None,
         catch_exceptions: bool = True,
@@ -621,37 +631,39 @@
         if colliding_params:
             # Transfer colliding parameters from ``extra`` to ``extra_bypass``.
             extra_bypass = {pid: extra.pop(pid) for pid in colliding_params}
             # Monkeypatch the original command's ``main()`` call to pass extra
             # parameter for ``Context`` initialization. Because we cannot simply add
             # colliding parameter IDs to ``**extra``.
             extra_params_bypass = patch.object(
-                cli, "main", partial(cli.main, **extra_bypass)
+                cli,
+                "main",
+                partial(cli.main, **extra_bypass),
             )
 
         with extra_params_bypass:
             result = self.invoke2(
-                    cli=cli,
-                    args=clean_args,
-                    input=input,
-                    env=env,
-                    catch_exceptions=catch_exceptions,
-                    color=isolation_color,
-                    **extra,
-                )
+                cli=cli,
+                args=clean_args,
+                input=input,
+                env=env,
+                catch_exceptions=catch_exceptions,
+                color=isolation_color,
+                **extra,
+            )
 
         # ``color`` has been explicitly set to ``False``, so strip all ANSI codes.
         if color is False:
             result.stdout_bytes = strip_ansi(result.stdout_bytes)
             result.stderr_bytes = strip_ansi(result.stderr_bytes)
             result.output_bytes = strip_ansi(result.output_bytes)
 
         print_cli_run(
-            [self.get_default_prog_name(cli)] + list(clean_args),
+            [self.get_default_prog_name(cli), *clean_args],
             result,
             env=env,
         )
 
         if result.exception:
             print(ExceptionInfo.from_exc_info(*result.exc_info).get_formatted())
 
-        return result
+        return result
```

### Comparing `click_extra-4.3.0/click_extra/tests/__init__.py` & `click_extra-4.4.0/click_extra/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.3.0/click_extra/tests/conftest.py` & `click_extra-4.4.0/click_extra/tests/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,54 +13,25 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 """Fixtures, configuration and helpers for tests."""
 
 from __future__ import annotations
 
-import os
-from configparser import RawConfigParser  # noqa: E402
 from pathlib import Path
 from textwrap import dedent
 
 import click
 import click.testing
 import cloup
 import pytest
 
-from ..decorators import command, extra_command, extra_group, group
-from ..platforms import is_linux, is_macos, is_windows
-from ..testing import ExtraCliRunner
-
-DESTRUCTIVE_MODE = RawConfigParser.BOOLEAN_STATES[
-    str(os.environ.get("DESTRUCTIVE_TESTS", False)).lower()
-]
-"""Pre-computed boolean flag indicating if destructive mode is activated by the presence
-of a ``DESTRUCTIVE_TESTS`` environment variable set to ``True``."""
-
-
-destructive = pytest.mark.skipif(DESTRUCTIVE_MODE, reason="destructive test")
-"""Pytest mark to skip a test unless destructive mode is allowed.
-
-.. todo:
-
-    Test destructive test assessment.
-"""
-
-
-non_destructive = pytest.mark.skipif(
-    not DESTRUCTIVE_MODE, reason="non-destructive test"
-)
-"""Pytest mark to skip a test unless destructive mode is allowed.
-
-.. todo:
-
-    Test destructive test assessment.
-"""
-
+from click_extra.decorators import command, extra_command, extra_group, group
+from click_extra.platforms import is_linux, is_macos, is_windows
+from click_extra.testing import ExtraCliRunner
 
 skip_linux = pytest.mark.skipif(is_linux(), reason="Skip Linux")
 """Pytest mark to skip a test if run on a Linux system."""
 
 skip_macos = pytest.mark.skipif(is_macos(), reason="Skip macOS")
 """Pytest mark to skip a test if run on a macOS system."""
 
@@ -83,23 +54,23 @@
 
 See:
 - https://github.com/pallets/click/issues/2111
 - https://github.com/pallets/click/issues/2110
 """
 
 
-@pytest.fixture
+@pytest.fixture()
 def extra_runner():
     """Runner fixture for ``click.testing.ExtraCliRunner``."""
     runner = ExtraCliRunner()
     with runner.isolated_filesystem():
         yield runner
 
 
-@pytest.fixture
+@pytest.fixture()
 def invoke(extra_runner):
     """Invoke fixture shorthand for ``click.testing.ExtraCliRunner.invoke``."""
     return extra_runner.invoke
 
 
 # XXX Support for decorator without parenthesis in Cloup has been reported upstream:
 # https://github.com/janluke/cloup/issues/127
@@ -121,31 +92,31 @@
 
     if no_commands is False:
         if not no_click:
             params.extend(
                 [
                     (click.command, {"click", "command"}, "click.command", ()),
                     (click.command(), {"click", "command"}, "click.command()", ()),
-                ]
+                ],
             )
 
         if not no_cloup:
             params.extend(
                 [
                     (cloup.command, {"cloup", "command"}, "cloup.command", skip_naked),
                     (cloup.command(), {"cloup", "command"}, "cloup.command()", ()),
-                ]
+                ],
             )
 
         if not no_redefined:
             params.extend(
                 [
                     (command, {"redefined", "command"}, "click_extra.command", ()),
                     (command(), {"redefined", "command"}, "click_extra.command()", ()),
-                ]
+                ],
             )
 
         if not no_extra:
             params.extend(
                 [
                     (
                         extra_command,
@@ -155,40 +126,40 @@
                     ),
                     (
                         extra_command(),
                         {"extra", "command"},
                         "click_extra.extra_command()",
                         (),
                     ),
-                ]
+                ],
             )
 
     if not no_groups:
         if not no_click:
             params.extend(
                 [
                     (click.group, {"click", "group"}, "click.group", ()),
                     (click.group(), {"click", "group"}, "click.group()", ()),
-                ]
+                ],
             )
 
         if not no_cloup:
             params.extend(
                 [
                     (cloup.group, {"cloup", "group"}, "cloup.group", skip_naked),
                     (cloup.group(), {"cloup", "group"}, "cloup.group()", ()),
-                ]
+                ],
             )
 
         if not no_redefined:
             params.extend(
                 [
                     (group, {"redefined", "group"}, "click_extra.group", ()),
                     (group(), {"redefined", "group"}, "click_extra.group()", ()),
-                ]
+                ],
             )
 
         if not no_extra:
             params.extend(
                 [
                     (
                         extra_group,
@@ -198,28 +169,28 @@
                     ),
                     (
                         extra_group(),
                         {"extra", "group"},
                         "click_extra.extra_group()",
                         (),
                     ),
-                ]
+                ],
             )
 
     decorator_params = []
     for deco, deco_type, label, marks in params:
         args = [deco]
         if with_types:
             args.append(deco_type)
         decorator_params.append(pytest.param(*args, id=label, marks=marks))
 
     return tuple(decorator_params)
 
 
-@pytest.fixture
+@pytest.fixture()
 def create_config(tmp_path):
     """A generic fixture to produce a temporary configuration file."""
 
     def _create_config(filename, content):
         """Create a fake configuration file."""
         assert isinstance(content, str)
```

### Comparing `click_extra-4.3.0/click_extra/tests/test_colorize.py` & `click_extra-4.4.0/click_extra/tests/test_colorize.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,30 +22,40 @@
 
 import click
 import cloup
 import pytest
 from boltons.strutils import strip_ansi
 from pytest_cases import parametrize
 
-from .. import HelpTheme, Style, argument, echo, option, option_group, secho, style
-from ..colorize import (
+from click_extra import (
+    HelpTheme,
+    Style,
+    argument,
+    echo,
+    option,
+    option_group,
+    secho,
+    style,
+)
+from click_extra.colorize import (
     HelpExtraFormatter,
     HelpExtraTheme,
     default_theme,
     highlight,
 )
-from ..decorators import (
+from click_extra.decorators import (
     color_option,
     command,
     extra_command,
     extra_group,
     help_option,
     verbosity_option,
 )
-from ..logging import LOG_LEVELS
+from click_extra.logging import LOG_LEVELS
+
 from .conftest import (
     command_decorators,
     default_debug_colored_log_end,
     default_debug_colored_log_start,
     default_debug_uncolored_log_end,
     default_debug_uncolored_log_start,
     default_options_colored_help,
@@ -78,15 +88,15 @@
     formatter = HelpExtraFormatter()
     formatter.write(
         """
         -e, --apt [apm|apt|apt-mint|brew]
                         Exclude a package manager.
                         Repeat to exclude multiple
                         managers.
-        """
+        """,
     )
 
     formatter.choices = {"apm", "apt", "apt-mint", "brew"}
 
     output = formatter.getvalue()
     assert default_theme.choice("apm") in output
     assert default_theme.choice("apt") in output
@@ -156,15 +166,15 @@
     def command4():
         echo("Run click-extra command #4...")
 
     color_cli1.section("Subcommand group 1", command1, command2)
     color_cli1.section("Extra commands", command3, command4)
 
     help_screen = (
-        r"\x1b\[94m\x1b\[1m\x1b\[4mUsage: \x1b\[0m\x1b\[97mcolor-cli1\x1b\[0m "
+        r"\x1b\[94m\x1b\[1m\x1b\[4mUsage:\x1b\[0m \x1b\[97mcolor-cli1\x1b\[0m "
         r"\x1b\[36m\x1b\[2m\[OPTIONS\]\x1b\[0m"
         r" \x1b\[36m\x1b\[2mCOMMAND \[ARGS\]...\x1b\[0m\n\n"
         r"\x1b\[94m\x1b\[1m\x1b\[4mGroup 1:\x1b\[0m\n"
         r"  \x1b\[36m-a\x1b\[0m, \x1b\[36m--o1\x1b\[0m \x1b\[36m\x1b\[2mTEXT\x1b\[0m\n"
         r"  \x1b\[36m-b\x1b\[0m, \x1b\[36m--o2\x1b\[0m \x1b\[36m\x1b\[2mTEXT\x1b\[0m\n"
         r"\n"
         r"\x1b\[94m\x1b\[1m\x1b\[4mGroup 2:\x1b\[0m\n"
@@ -205,15 +215,15 @@
     assert not result.stderr
 
     # CLI main group is invoked before sub-command.
     result = invoke(color_cli1, "command1", "--help", color=True)
     assert result.exit_code == 0
     assert result.stdout == (
         "It works!\n"
-        "\x1b[94m\x1b[1m\x1b[4mUsage: \x1b[0m\x1b[97mcolor-cli1 command1\x1b[0m"
+        "\x1b[94m\x1b[1m\x1b[4mUsage:\x1b[0m \x1b[97mcolor-cli1 command1\x1b[0m"
         " \x1b[36m\x1b[2m[OPTIONS]\x1b[0m [\x1b[36mMY_ARG\x1b[0m]...\n"
         "\n"
         "  CLI description with extra MY_VAR reference.\n"
         "\n"
         "\x1b[94m\x1b[1m\x1b[4mPositional arguments:\x1b[0m\n"
         "  [\x1b[36mMY_ARG\x1b[0m]...  Argument supports help.\n"
         "\n"
@@ -222,15 +232,15 @@
     )
     assert not result.stderr
 
     # Standalone call to command: CLI main group is skipped.
     result = invoke(command1, "--help", color=True)
     assert result.exit_code == 0
     assert result.stdout == (
-        "\x1b[94m\x1b[1m\x1b[4mUsage: \x1b[0m\x1b[97mcommand1\x1b[0m"
+        "\x1b[94m\x1b[1m\x1b[4mUsage:\x1b[0m \x1b[97mcommand1\x1b[0m"
         " \x1b[36m\x1b[2m[OPTIONS]\x1b[0m [\x1b[36mMY_ARG\x1b[0m]...\n"
         "\n"
         "  CLI description with extra MY_VAR reference.\n"
         "\n"
         "\x1b[94m\x1b[1m\x1b[4mPositional arguments:\x1b[0m\n"
         "  [\x1b[36mMY_ARG\x1b[0m]...  Argument supports help.\n"
         "\n"
@@ -246,23 +256,23 @@
         assert result.stdout == dedent(
             f"""\
             It works!
             Usage: color-cli1 {cmd_id} [OPTIONS]
 
             Options:
               -h, --help  Show this message and exit.
-            """
+            """,
         )
         assert not result.stderr
 
 
 @skip_windows_colors
 @parametrize("option_decorator", (color_option, color_option()))
 @pytest.mark.parametrize(
-    "param, expecting_colors",
+    ("param", "expecting_colors"),
     (
         ("--color", True),
         ("--no-color", False),
         ("--ansi", True),
         ("--no-ansi", False),
         (None, True),
     ),
@@ -320,15 +330,15 @@
             ),
             result.stderr,
         )
 
 
 @skip_windows_colors
 @pytest.mark.parametrize(
-    "env, env_expect_colors",
+    ("env", "env_expect_colors"),
     (
         ({"COLOR": "True"}, True),
         ({"COLOR": "true"}, True),
         ({"COLOR": "1"}, True),
         ({"COLOR": ""}, True),
         ({"COLOR": "False"}, False),
         ({"COLOR": "false"}, False),
@@ -340,25 +350,29 @@
         ({"NO_COLOR": "False"}, True),
         ({"NO_COLOR": "false"}, True),
         ({"NO_COLOR": "0"}, True),
         (None, True),
     ),
 )
 @pytest.mark.parametrize(
-    "param, param_expect_colors",
+    ("param", "param_expect_colors"),
     (
         ("--color", True),
         ("--no-color", False),
         ("--ansi", True),
         ("--no-ansi", False),
         (None, True),
     ),
 )
 def test_no_color_env_convention(
-    invoke, env, env_expect_colors, param, param_expect_colors
+    invoke,
+    env,
+    env_expect_colors,
+    param,
+    param_expect_colors,
 ):
     @click.command
     @color_option
     def color_cli7():
         echo(Style(fg="yellow")("It works!"))
 
     result = invoke(color_cli7, param, color=True, env=env)
@@ -377,15 +391,15 @@
 
 
 # TODO: test with  configuration file
 
 
 @skip_windows_colors
 @pytest.mark.parametrize(
-    "param, expecting_colors",
+    ("param", "expecting_colors"),
     (
         ("--color", True),
         ("--no-color", False),
         ("--ansi", True),
         ("--no-ansi", False),
         (None, True),
     ),
@@ -438,15 +452,15 @@
                 rf"{default_debug_uncolored_log_end}"
             ),
             result.stderr,
         )
 
 
 @pytest.mark.parametrize(
-    "substrings, expected, ignore_case",
+    ("substrings", "expected", "ignore_case"),
     (
         # Function input types.
         (["hey"], "Hey-xx-xxx-heY-xXxXxxxxx-\x1b[32mhey\x1b[0m", False),
         (("hey",), "Hey-xx-xxx-heY-xXxXxxxxx-\x1b[32mhey\x1b[0m", False),
         ({"hey"}, "Hey-xx-xxx-heY-xXxXxxxxx-\x1b[32mhey\x1b[0m", False),
         (
             "hey",
@@ -524,18 +538,18 @@
     if "group" in cmd_type:
         assert result.stdout == dedent(
             """\
             Usage: standalone-help [OPTIONS] COMMAND [ARGS]...
 
             Options:
               -h, --help  Show this message and exit.
-            """
+            """,
         )
     else:
         assert result.stdout == dedent(
             """\
             Usage: standalone-help [OPTIONS]
 
             Options:
               -h, --help  Show this message and exit.
-            """
+            """,
         )
```

### Comparing `click_extra-4.3.0/click_extra/tests/test_commands.py` & `click_extra-4.4.0/click_extra/tests/test_commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,17 @@
 from textwrap import dedent
 
 import click
 import cloup
 import pytest
 from pytest_cases import fixture
 
-from .. import echo, option, option_group
-from ..decorators import extra_command, extra_group
+from click_extra import echo, option, option_group
+from click_extra.decorators import extra_command, extra_group
+
 from .conftest import (
     default_debug_uncolored_log_end,
     default_debug_uncolored_log_start,
     default_options_colored_help,
     default_options_uncolored_help,
     skip_windows_colors,
 )
@@ -176,16 +177,16 @@
 
 
 @pytest.mark.parametrize(
     "params",
     ("--version", "blah", ("--verbosity", "DEBUG"), ("--config", "random.toml")),
 )
 def test_help_eagerness(invoke, all_command_cli, params):
-    """
-    See: https://click.palletsprojects.com/en/8.0.x/advanced/#callback-evaluation-order
+    """See: https://click.palletsprojects.com/en/8.0.x/advanced/#callback-evaluation-
+    order.
     """
     result = invoke(all_command_cli, "--help", params)
     assert result.exit_code == 0
     assert re.fullmatch(help_screen, result.stdout)
     assert "It works!" not in result.stdout
     assert not result.stderr
 
@@ -196,16 +197,16 @@
 def test_subcommand_help(invoke, all_command_cli, cmd_id, param):
     result = invoke(all_command_cli, f"{cmd_id}-subcommand", param)
     assert result.exit_code == 0
     assert not result.stderr
 
     colored_help_header = (
         r"It works!\n"
-        r"\x1b\[94m\x1b\[1m\x1b\[4mUsage: "
-        rf"\x1b\[0m\x1b\[97mcommand-cli1 {cmd_id}-subcommand\x1b\[0m"
+        r"\x1b\[94m\x1b\[1m\x1b\[4mUsage:\x1b\[0m "
+        rf"\x1b\[97mcommand-cli1 {cmd_id}-subcommand\x1b\[0m"
         r" \x1b\[36m\x1b\[2m\[OPTIONS\]\x1b\[0m\n"
         r"\n"
         r"\x1b\[94m\x1b\[1m\x1b\[4mOptions:\x1b\[0m\n"
     )
 
     # Extra sucommands are colored and include all extra options.
     if cmd_id == "click-extra":
@@ -231,27 +232,27 @@
         assert result.stdout == dedent(
             f"""\
             It works!
             Usage: command-cli1 {cmd_id}-subcommand [OPTIONS]
 
             Options:
               -h, --help  Show this message and exit.
-            """
+            """,
         )
 
 
 @pytest.mark.parametrize("cmd_id", ("default", "click-extra", "cloup", "click"))
 def test_subcommand_execution(invoke, all_command_cli, cmd_id):
     result = invoke(all_command_cli, f"{cmd_id}-subcommand", color=False)
     assert result.exit_code == 0
     assert result.stdout == dedent(
         f"""\
         It works!
         Run {cmd_id} subcommand...
-        """
+        """,
     )
     assert not result.stderr
 
 
 def test_integrated_version_value(invoke, all_command_cli):
     result = invoke(all_command_cli, "--version", color=False)
     assert result.exit_code == 0
@@ -290,15 +291,15 @@
 
         Options:
           --help  Show this message and exit.
 
         Commands:
           bar  Bar subcommand.
           foo
-        """
+        """,
     )
     assert not result.stderr
 
     result = invoke(cli, "foo", "--help", color=False)
     assert result.exit_code == 0
     assert re.fullmatch(
         (
@@ -367,15 +368,15 @@
         result.stdout,
     )
     assert "It works!" not in result.stdout
     assert not result.stderr
 
 
 @pytest.mark.parametrize(
-    "cmd_decorator, ctx_settings, expected_help",
+    ("cmd_decorator", "ctx_settings", "expected_help"),
     (
         # Click does not show all envvar in the help screen by default, unless
         # specifficaly set on an option.
         (
             click.command,
             {},
             "  --flag1\n  --flag2  [env var: custom2]\n  --flag3\n",
```

### Comparing `click_extra-4.3.0/click_extra/tests/test_config.py` & `click_extra-4.4.0/click_extra/tests/test_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from pathlib import Path
 
 import click
 import pytest
 from boltons.pathutils import shrinkuser
 from pytest_cases import fixture, parametrize
 
-from .. import (
+from click_extra import (
     BOOL,
     FLOAT,
     INT,
     STRING,
     UNPROCESSED,
     UUID,
     Choice,
@@ -38,18 +38,19 @@
     IntRange,
     Tuple,
     argument,
     echo,
     get_app_dir,
     option,
 )
-from ..colorize import escape_for_help_sceen
-from ..config import ConfigOption
-from ..decorators import config_option, extra_group
-from ..parameters import search_params
+from click_extra.colorize import escape_for_help_sceen
+from click_extra.config import ConfigOption
+from click_extra.decorators import config_option, extra_group
+from click_extra.parameters import search_params
+
 from .conftest import (
     default_debug_uncolored_log_end,
     default_debug_uncolored_log_start,
 )
 
 DUMMY_TOML_FILE = """
     # Comment
@@ -224,15 +225,19 @@
     assert result.exit_code == 0
     assert not result.stderr
     assert result.stdout == "dummy_flag = False\nmy_list = ()\nint_parameter = 10\n"
 
 
 def test_unset_conf_debug_message(invoke, simple_config_cli):
     result = invoke(
-        simple_config_cli, "--verbosity", "DEBUG", "default-command", color=False
+        simple_config_cli,
+        "--verbosity",
+        "DEBUG",
+        "default-command",
+        color=False,
     )
     assert result.exit_code == 0
     assert result.stdout == "dummy_flag = False\nmy_list = ()\nint_parameter = 10\n"
     assert re.fullmatch(
         default_debug_uncolored_log_start + default_debug_uncolored_log_end,
         result.stderr,
     )
@@ -241,39 +246,47 @@
 def test_conf_default_path(invoke, simple_config_cli):
     result = invoke(simple_config_cli, "--help", color=False)
     assert result.exit_code == 0
     assert not result.stderr
 
     # OS-specific path.
     default_path = shrinkuser(
-        Path(get_app_dir("config-cli1")) / "*.{toml,yaml,yml,json,ini,xml}"
+        Path(get_app_dir("config-cli1")) / "*.{toml,yaml,yml,json,ini,xml}",
     )
 
     # Make path string compatible with regexp.
     assert re.search(
         rf"\[default:\s+{escape_for_help_sceen(str(default_path))}\]",
         result.stdout,
     )
 
 
 def test_conf_not_exist(invoke, simple_config_cli):
     conf_path = Path("dummy.toml")
     result = invoke(
-        simple_config_cli, "--config", str(conf_path), "default-command", color=False
+        simple_config_cli,
+        "--config",
+        str(conf_path),
+        "default-command",
+        color=False,
     )
     assert result.exit_code == 2
     assert not result.stdout
     assert f"Load configuration matching {conf_path}\n" in result.stderr
     assert "critical: No configuration file found.\n" in result.stderr
 
 
 def test_conf_not_file(invoke, simple_config_cli):
     conf_path = Path().parent
     result = invoke(
-        simple_config_cli, "--config", str(conf_path), "default-command", color=False
+        simple_config_cli,
+        "--config",
+        str(conf_path),
+        "default-command",
+        color=False,
     )
     assert result.exit_code == 2
     assert not result.stdout
 
     assert f"Load configuration matching {conf_path}\n" in result.stderr
     assert "critical: No configuration file found.\n" in result.stderr
 
@@ -373,15 +386,15 @@
             "count_param": None,
             "float_range_param": None,
             "datetime_param": None,
             "tuple1": None,
             "list1": None,
             "file_arg1": None,
             "file_arg2": None,
-        }
+        },
     }
     assert cli_config_option.params_types == {
         "config-cli2": {
             "flag1": bool,
             "flag2": bool,
             "str_param1": str,
             "str_param2": str,
@@ -400,15 +413,15 @@
             "count_param": int,
             "float_range_param": float,
             "datetime_param": str,
             "tuple1": list,
             "list1": list,
             "file_arg1": str,
             "file_arg2": list,
-        }
+        },
     }
 
 
 def test_strict_conf(invoke, create_config):
     """Same test as the one shown in the readme, but in strict validation mode."""
 
     @click.group
@@ -450,15 +463,20 @@
     assert result.exit_code == 1
     assert f"Load configuration matching {conf_path}\n" in result.stderr
     assert not result.stdout
 
 
 @all_config_formats
 def test_conf_file_overrides_defaults(
-    invoke, simple_config_cli, create_config, httpserver, conf_name, conf_content
+    invoke,
+    simple_config_cli,
+    create_config,
+    httpserver,
+    conf_name,
+    conf_content,
 ):
     # Create a local file and remote config.
     conf_filepath = create_config(conf_name, conf_content)
     httpserver.expect_request(f"/{conf_name}").respond_with_data(conf_content)
     conf_url = httpserver.url_for(f"/{conf_name}")
 
     for conf_path, is_url in (conf_filepath, False), (conf_url, True):
@@ -489,15 +507,20 @@
             rf"{default_debug_uncolored_log_end}"
         )
         assert re.fullmatch(debug_log, result.stderr)
 
 
 @all_config_formats
 def test_auto_env_var_conf(
-    invoke, simple_config_cli, create_config, httpserver, conf_name, conf_content
+    invoke,
+    simple_config_cli,
+    create_config,
+    httpserver,
+    conf_name,
+    conf_content,
 ):
     # Create a local config.
     conf_filepath = create_config(conf_name, conf_content)
 
     # Create a remote config.
     httpserver.expect_request(f"/{conf_name}").respond_with_data(conf_content)
     conf_url = httpserver.url_for(f"/{conf_name}")
@@ -519,15 +542,20 @@
             f"Load configuration matching {conf_path.resolve()}\n"
             "debug: Verbosity set to DEBUG.\n"
         )
 
 
 @all_config_formats
 def test_conf_file_overrided_by_cli_param(
-    invoke, simple_config_cli, create_config, httpserver, conf_name, conf_content
+    invoke,
+    simple_config_cli,
+    create_config,
+    httpserver,
+    conf_name,
+    conf_content,
 ):
     # Create a local file and remote config.
     conf_filepath = create_config(conf_name, conf_content)
     httpserver.expect_request(f"/{conf_name}").respond_with_data(conf_content)
     conf_url = httpserver.url_for(f"/{conf_name}")
 
     for conf_path in conf_filepath, conf_url:
```

### Comparing `click_extra-4.3.0/click_extra/tests/test_logging.py` & `click_extra-4.4.0/click_extra/tests/test_logging.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,17 +20,18 @@
 import random
 import re
 
 import click
 import pytest
 from pytest_cases import parametrize
 
-from .. import echo
-from ..decorators import extra_command, verbosity_option
-from ..logging import DEFAULT_LEVEL, LOG_LEVELS
+from click_extra import echo
+from click_extra.decorators import extra_command, verbosity_option
+from click_extra.logging import DEFAULT_LEVEL, LOG_LEVELS
+
 from .conftest import (
     command_decorators,
     default_debug_colored_log_end,
     default_debug_colored_log_start,
     default_debug_uncolored_log_end,
     skip_windows_colors,
 )
@@ -49,15 +50,18 @@
 
     # Check root logger's level.
     assert logging.root.getEffectiveLevel() == logging.WARNING
     assert logging._levelToName[logging.root.level] == "WARNING"
     assert logging.root.level == DEFAULT_LEVEL
 
 
-@pytest.mark.parametrize("cmd_decorator, cmd_type", command_decorators(with_types=True))
+@pytest.mark.parametrize(
+    ("cmd_decorator", "cmd_type"),
+    command_decorators(with_types=True),
+)
 def test_unrecognized_verbosity(invoke, cmd_decorator, cmd_type):
     @cmd_decorator
     @verbosity_option
     def logging_cli1():
         echo("It works!")
 
     result = invoke(logging_cli1, "--verbosity", "random")
@@ -85,24 +89,24 @@
 @parametrize("option_decorator", (verbosity_option, verbosity_option()))
 @pytest.mark.parametrize("level", LOG_LEVELS.keys())
 def test_default_root_logger(invoke, cmd_decorator, option_decorator, level):
     """Checks:
     - the default logger is ``<root>``
     - the default logger message format
     - level names are colored
-    - log level is propagated to all other loggers
+    - log level is propagated to all other loggers.
     """
 
     @cmd_decorator
     @option_decorator
     def logging_cli2():
         echo("It works!")
 
         random_logger = logging.getLogger(
-            f"random_logger_{random.randrange(10000, 99999)}"
+            f"random_logger_{random.randrange(10000, 99999)}",
         )
         random_logger.debug("my random message.")
 
         logging.debug("my debug message.")
         logging.info("my info message.")
         logging.warning("my warning message.")
         logging.error("my error message.")
@@ -149,15 +153,16 @@
             result.stderr,
         )
     else:
         assert not result.stderr
 
 
 @pytest.mark.parametrize(
-    "logger_param", (logging.getLogger("awesome_app"), "awesome_app")
+    "logger_param",
+    (logging.getLogger("awesome_app"), "awesome_app"),
 )
 @pytest.mark.parametrize("params", (("--verbosity", "DEBUG"), None))
 def test_custom_logger_param(invoke, logger_param, params):
     """Passing a logger instance or name to the ``default_logger`` parameter works."""
 
     @click.command
     @verbosity_option(default_logger=logger_param)
```

### Comparing `click_extra-4.3.0/click_extra/tests/test_parameters.py` & `click_extra-4.4.0/click_extra/tests/test_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,29 +21,24 @@
 from textwrap import dedent
 
 import click
 import pytest
 from pytest_cases import parametrize
 from tabulate import tabulate
 
-from .. import (
-    command,
-    echo,
-    get_app_dir,
-    option,
-    pass_context,
-)
-from ..decorators import extra_command, extra_group, show_params_option
-from ..parameters import ShowParamsOption, extend_envvars, normalize_envvar
-from ..platforms import is_windows
+from click_extra import command, echo, get_app_dir, option, pass_context
+from click_extra.decorators import extra_command, extra_group, show_params_option
+from click_extra.parameters import ShowParamsOption, extend_envvars, normalize_envvar
+from click_extra.platforms import is_windows
+
 from .conftest import command_decorators
 
 
 @pytest.mark.parametrize(
-    "envvars_1, envvars_2, result",
+    ("envvars_1", "envvars_2", "result"),
     (
         ("MY_VAR", "MY_VAR", ("MY_VAR",)),
         (None, "MY_VAR", ("MY_VAR",)),
         ("MY_VAR", None, ("MY_VAR",)),
         (["MY_VAR"], "MY_VAR", ("MY_VAR",)),
         (["MY_VAR"], None, ("MY_VAR",)),
         ("MY_VAR", ["MY_VAR"], ("MY_VAR",)),
@@ -57,27 +52,27 @@
     ),
 )
 def test_extend_envvars(envvars_1, envvars_2, result):
     assert extend_envvars(envvars_1, envvars_2) == result
 
 
 @pytest.mark.parametrize(
-    "env_name, normalized_env",
+    ("env_name", "normalized_env"),
     (
         ("show-params-cli_VERSION", "SHOW_PARAMS_CLI_VERSION"),
         ("show---params-cli___VERSION", "SHOW_PARAMS_CLI_VERSION"),
         ("__show-__params-_-_-", "SHOW_PARAMS"),
     ),
 )
 def test_normalize_envvar(env_name, normalized_env):
     assert normalize_envvar(env_name) == normalized_env
 
 
 @pytest.mark.parametrize(
-    "cmd_decorator, option_help",
+    ("cmd_decorator", "option_help"),
     (
         # Click does not show the auto-generated envvar in the help screen.
         (click.command, "  --flag / --no-flag  [env var: custom]\n"),
         # Click Extra always adds the auto-generated envvar to the help screen
         # (and show the defaults).
         (
             extra_command,
@@ -195,15 +190,15 @@
                     envvar = {envvar_name: envar_value}
                     params.append(
                         pytest.param(
                             cmd_decorator,
                             envvar,
                             expected_flag,
                             id=f"{decorator_name}|{case_name}={envvar}|expected_flag={expected_flag}",
-                        )
+                        ),
                     )
 
     return params
 
 
 @parametrize("cmd_decorator, envvars, expected_flag", envvars_test_cases())
 def test_auto_envvar_parsing(invoke, cmd_decorator, envvars, expected_flag):
@@ -217,15 +212,15 @@
     @option("--flag/--no-flag", envvar=["Magic", "sUper"])
     def my_cli(flag):
         echo(f"Flag value: {flag}")
 
     registered_envvars = ["Magic", "sUper"]
     # @extra_command forces registration of auto-generated envvar.
     if cmd_decorator == extra_command:
-        registered_envvars = tuple(registered_envvars + ["yo_FLAG"])
+        registered_envvars = (*registered_envvars, "yo_FLAG")
     assert my_cli.params[0].envvar == registered_envvars
 
     result = invoke(my_cli, env=envvars)
     assert result.exit_code == 0
     assert not result.stderr
     assert result.stdout == f"Flag value: {expected_flag}\n"
 
@@ -256,15 +251,15 @@
         """\
         -- Group output --
         dummy_flag is True
         Raw parameters: ['--dummy-flag', 'subcommand', '--int-param', '33']
         -- Subcommand output --
         int_parameter is 33
         Raw parameters: ['--int-param', '33']
-        """
+        """,
     )
 
 
 @parametrize(
     "cmd_decorator",
     # Skip click extra's commands, as show_params option is already part of the default.
     command_decorators(no_groups=True, no_extra=True),
@@ -299,15 +294,15 @@
         tablefmt="rounded_outline",
         disable_numparse=True,
     )
     assert result.stdout == f"{output}\n"
 
     assert result.stderr.endswith(
         "warning: Cannot extract parameters values: "
-        "<Command show-params> does not inherits from ExtraCommand.\n"
+        "<Command show-params> does not inherits from ExtraCommand.\n",
     )
 
 
 def test_integrated_show_params_option(invoke, create_config):
     @extra_command
     @option("--int-param1", type=int, default=10)
     @option("--int-param2", type=int, default=555)
```

### Comparing `click_extra-4.3.0/click_extra/tests/test_platforms.py` & `click_extra-4.4.0/click_extra/tests/test_platforms.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,36 +15,48 @@
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 
 from __future__ import annotations
 
 import functools
 from itertools import combinations
 
-from .. import platforms as platforms_module
-from ..platforms import (
+import pytest
+
+from click_extra import platforms as platforms_module
+from click_extra.platforms import (
+    AIX,
     ALL_GROUPS,
     ALL_LINUX,
     ALL_OS_LABELS,
     ALL_PLATFORMS,
     ALL_WINDOWS,
     BSD,
     BSD_WITHOUT_MACOS,
     CURRENT_OS_ID,
     CURRENT_OS_LABEL,
+    CYGWIN,
     EXTRA_GROUPS,
+    FREEBSD,
+    HURD,
     LINUX,
     LINUX_LAYERS,
     MACOS,
+    NETBSD,
     NON_OVERLAPPING_GROUPS,
+    OPENBSD,
     OTHER_UNIX,
+    SOLARIS,
+    SUNOS,
     SYSTEM_V,
     UNIX,
     UNIX_LAYERS,
     UNIX_WITHOUT_MACOS,
     WINDOWS,
+    WSL1,
+    WSL2,
     Group,
     current_os,
     is_aix,
     is_cygwin,
     is_freebsd,
     is_hurd,
     is_linux,
@@ -53,61 +65,63 @@
     is_openbsd,
     is_solaris,
     is_sunos,
     is_windows,
     is_wsl1,
     is_wsl2,
     os_label,
+    reduce,
 )
+
 from .conftest import (
     skip_linux,
     skip_macos,
     skip_windows,
     unless_linux,
     unless_macos,
     unless_windows,
 )
 
 
 def test_mutual_exclusion():
     """Only directly tests OSes on which the test suite is running via GitHub
     actions."""
     if is_linux():
-        assert CURRENT_OS_ID == LINUX.id
-        assert CURRENT_OS_LABEL == os_label(LINUX.id)
+        assert LINUX.id == CURRENT_OS_ID
+        assert os_label(LINUX.id) == CURRENT_OS_LABEL
         assert not is_aix()
         assert not is_cygwin()
         assert not is_freebsd()
         assert not is_hurd()
         assert not is_macos()
         assert not is_netbsd()
         assert not is_openbsd()
         assert not is_solaris()
         assert not is_sunos()
         assert not is_windows()
         assert not is_wsl1()
         assert not is_wsl2()
     if is_macos():
-        assert CURRENT_OS_ID == MACOS.id
-        assert CURRENT_OS_LABEL == os_label(MACOS.id)
+        assert MACOS.id == CURRENT_OS_ID
+        assert os_label(MACOS.id) == CURRENT_OS_LABEL
         assert not is_aix()
         assert not is_cygwin()
         assert not is_freebsd()
         assert not is_hurd()
         assert not is_linux()
         assert not is_netbsd()
         assert not is_openbsd()
         assert not is_solaris()
         assert not is_sunos()
         assert not is_windows()
         assert not is_wsl1()
         assert not is_wsl2()
     if is_windows():
-        assert CURRENT_OS_ID == WINDOWS.id
-        assert CURRENT_OS_LABEL == os_label(WINDOWS.id)
+        assert WINDOWS.id == CURRENT_OS_ID
+        assert os_label(WINDOWS.id) == CURRENT_OS_LABEL
         assert not is_aix()
         assert not is_cygwin()
         assert not is_freebsd()
         assert not is_hurd()
         assert not is_linux()
         assert not is_macos()
         assert not is_netbsd()
@@ -181,22 +195,22 @@
             # Each group is both a subset and a superset of itself.
             assert group.issubset(group)
             assert group.issuperset(group)
             assert group.issubset(group.platforms)
             assert group.issuperset(group.platforms)
 
             # Test against empty iterables.
-            assert group.issuperset(tuple())
-            assert group.issuperset(list())
-            assert group.issuperset(dict())
+            assert group.issuperset(())
+            assert group.issuperset([])
+            assert group.issuperset({})
             assert group.issuperset(set())
             assert group.issuperset(frozenset())
-            assert not group.issubset(tuple())
-            assert not group.issubset(list())
-            assert not group.issubset(dict())
+            assert not group.issubset(())
+            assert not group.issubset([])
+            assert not group.issubset({})
             assert not group.issubset(set())
             assert not group.issubset(frozenset())
 
             for platform in group.platforms:
                 assert platform in group
                 assert platform in ALL_PLATFORMS
                 assert platform.id in group.platform_ids
@@ -264,14 +278,55 @@
         for group in NON_OVERLAPPING_GROUPS:
             if not extra_group.isdisjoint(group):
                 overlap = True
                 break
         assert overlap is True
 
 
+@pytest.mark.parametrize(
+    ("items", "expected"),
+    [
+        ([], set()),
+        ((), set()),
+        (set(), set()),
+        ([AIX], {AIX}),
+        ([AIX, AIX], {AIX}),
+        ([UNIX], {UNIX}),
+        ([UNIX, UNIX], {UNIX}),
+        ([UNIX, AIX], {UNIX}),
+        ([WINDOWS], {ALL_WINDOWS}),
+        ([ALL_PLATFORMS, WINDOWS], {ALL_PLATFORMS}),
+        ([UNIX, WINDOWS], {ALL_PLATFORMS}),
+        ([UNIX, ALL_WINDOWS], {ALL_PLATFORMS}),
+        ([BSD_WITHOUT_MACOS, UNIX], {UNIX}),
+        ([BSD_WITHOUT_MACOS, MACOS], {BSD}),
+        (
+            [
+                AIX,
+                CYGWIN,
+                FREEBSD,
+                HURD,
+                LINUX,
+                MACOS,
+                NETBSD,
+                OPENBSD,
+                SOLARIS,
+                SUNOS,
+                WINDOWS,
+                WSL1,
+                WSL2,
+            ],
+            {ALL_PLATFORMS},
+        ),
+    ],
+)
+def test_reduction(items, expected):
+    assert reduce(items) == expected
+
+
 def test_current_os_func():
     # Function.
     current_platform = current_os()
     assert current_platform in ALL_PLATFORMS.platforms
     # Constants.
     assert current_platform.id == CURRENT_OS_ID
     assert current_platform.name == CURRENT_OS_LABEL
```

### Comparing `click_extra-4.3.0/click_extra/tests/test_pygments.py` & `click_extra-4.4.0/click_extra/tests/test_pygments.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 from pygments.filter import Filter
 from pygments.filters import get_filter_by_name
 from pygments.formatter import Formatter
 from pygments.formatters import get_formatter_by_name
 from pygments.lexer import Lexer
 from pygments.lexers import find_lexer_class_by_name, get_lexer_by_name
 
-from .. import pygments as extra_pygments
-from ..pygments import DEFAULT_TOKEN_TYPE, collect_session_lexers
+from click_extra import pygments as extra_pygments
+from click_extra.pygments import DEFAULT_TOKEN_TYPE, collect_session_lexers
 
 PROJECT_ROOT = Path(__file__).parent.parent.parent
 
 
 def is_relative_to(path: Path, *other: Path) -> bool:
     """Return `True` if the path is relative to another path or `False`.
 
@@ -143,25 +143,27 @@
     # We cannot test for strict equality yet, as some ANSI-ready lexers do not
     # have any test artifacts producing ``Generic.Output`` tokens.
     assert lexer_classes.issubset(collect_session_lexers())
 
 
 def collect_classes(klass, prefix="Ansi"):
     """Returns all classes defined in ``click_extra.pygments`` that are a
-    subclass of ``klass``, and whose name starts with the provided ``prefix``."""
+    subclass of ``klass``, and whose name starts with the provided ``prefix``.
+    """
     klasses = {}
     for name, var in extra_pygments.__dict__.items():
         if issubclass(var, klass) and name.startswith(prefix):
             klasses[name] = var
     return klasses
 
 
 def get_pyproject_section(*section_path: str) -> dict[str, str]:
     """Descends into the TOML tree of ``pyproject.toml`` to reach the value specified by
-    ``section_path``."""
+    ``section_path``.
+    """
     toml_path = PROJECT_ROOT.joinpath("pyproject.toml").resolve()
     section: dict = tomllib.loads(toml_path.read_text(encoding="utf-8"))
     for section_id in section_path:
         section = section[section_id]
     return section
```

### Comparing `click_extra-4.3.0/click_extra/tests/test_tabulate.py` & `click_extra-4.4.0/click_extra/tests/test_tabulate.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,22 +17,26 @@
 from __future__ import annotations
 
 import pytest
 import tabulate
 from pytest_cases import fixture, parametrize
 
 # We use vanilla click primitives here to demonstrate the full-compatibility.
-from .. import echo, pass_context
-from ..decorators import table_format_option
-from ..platforms import is_windows
-from ..tabulate import output_formats
+from click_extra import echo, pass_context
+from click_extra.decorators import table_format_option
+from click_extra.platforms import is_windows
+from click_extra.tabulate import output_formats
+
 from .conftest import command_decorators
 
 
-@pytest.mark.parametrize("cmd_decorator, cmd_type", command_decorators(with_types=True))
+@pytest.mark.parametrize(
+    ("cmd_decorator", "cmd_type"),
+    command_decorators(with_types=True),
+)
 def test_unrecognized_format(invoke, cmd_decorator, cmd_type):
     @cmd_decorator
     @table_format_option
     def tabulate_cli1():
         echo("It works!")
 
     result = invoke(tabulate_cli1, "--table-format", "random")
@@ -525,15 +529,15 @@
         headers = ("day", "temperature")
         ctx.print_table(data, headers)
 
     return tabulate_cli2
 
 
 @pytest.mark.parametrize(
-    "format_name, expected",
+    ("format_name", "expected"),
     (pytest.param(k, v, id=k) for k, v in expected_renderings.items()),
 )
 def test_all_table_rendering(invoke, table_cli, format_name, expected):
     result = invoke(table_cli, "--table-format", format_name)
     assert result.exit_code == 0
     if not is_windows():
         expected = expected.replace("\r\n", "\n")
```

### Comparing `click_extra-4.3.0/click_extra/tests/test_telemetry.py` & `click_extra-4.4.0/click_extra/tests/test_telemetry.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 
 from __future__ import annotations
 
 from textwrap import dedent
 
 from pytest_cases import parametrize
 
-from .. import command, echo, pass_context, telemetry_option
+from click_extra import command, echo, pass_context, telemetry_option
+
 from .conftest import command_decorators
 
 
 @parametrize("cmd_decorator", command_decorators(no_groups=True, no_extra=True))
 @parametrize("option_decorator", (telemetry_option, telemetry_option()))
 def test_standalone_telemetry_option(invoke, cmd_decorator, option_decorator):
     @cmd_decorator
@@ -42,15 +43,15 @@
         """\
         Usage: standalone-telemetry [OPTIONS]
 
         Options:
           --telemetry / --no-telemetry  Collect telemetry and usage data.  [env var:
                                         DO_NOT_TRACK]
           --help                        Show this message and exit.
-        """
+        """,
     )
 
     result = invoke(standalone_telemetry, "--telemetry")
     assert result.exit_code == 0
     assert not result.stderr
     assert result.stdout == "It works!\nTelemetry value: True\n"
 
@@ -76,14 +77,14 @@
         """\
         Usage: standalone-telemetry [OPTIONS]
 
         Options:
           --telemetry / --no-telemetry  Collect telemetry and usage data.  [env var:
                                         DO_NOT_TRACK; default: no-telemetry]
           --help                        Show this message and exit.
-        """
+        """,
     )
 
     result = invoke(standalone_telemetry, env={"DO_NOT_TRACK": "1"})
     assert result.exit_code == 0
     assert not result.stderr
     assert result.stdout == "It works!\nTelemetry value: True\n"
```

### Comparing `click_extra-4.3.0/click_extra/tests/test_testing.py` & `click_extra-4.4.0/click_extra/tests/test_testing.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 import os
 from pathlib import Path
 
 import click
 import pytest
 from pytest_cases import fixture, parametrize
 
-from .. import Style, command, echo, pass_context, secho, style
-from ..platforms import is_windows
-from ..testing import ExtraCliRunner, env_copy
+from click_extra import Style, command, echo, pass_context, secho, style
+from click_extra.platforms import is_windows
+from click_extra.testing import ExtraCliRunner, env_copy
+
 from .conftest import command_decorators, skip_windows_colors
 
 
 def test_real_fs():
     """Check a simple test is not caught into the CLI runner fixture which is
     encapsulating all filesystem access into temporary directory structure."""
     assert str(Path(__file__)).startswith(str(Path.cwd()))
@@ -53,15 +54,14 @@
     extended_env = env_copy({env_var: "yo"})
     assert env_var in extended_env
     assert extended_env[env_var] == "yo"
     assert env_var not in os.environ
 
 
 def test_runner_output():
-
     @command
     def cli_output():
         echo("1 - stdout")
         echo("2 - stderr", err=True)
         echo("3 - stdout")
         echo("4 - stderr", err=True)
 
@@ -78,15 +78,14 @@
     assert result_mix.output == "1 - stdout\n2 - stderr\n3 - stdout\n4 - stderr\n"
     assert result_mix.stdout == "1 - stdout\n3 - stdout\n"
     assert result_mix.stderr == "2 - stderr\n4 - stderr\n"
 
 
 @pytest.mark.parametrize("mix_stderr", (True, False))
 def test_runner_empty_stderr(mix_stderr):
-
     @command
     def cli_empty_stderr():
         echo("stdout")
 
     runner = ExtraCliRunner(mix_stderr=mix_stderr)
     result = runner.invoke(cli_empty_stderr)
 
@@ -123,15 +122,16 @@
     @cmd_decorator
     @pass_context
     def run_cli2(ctx):
         """https://github.com/pallets/click/issues/2111."""
         echo(Style(fg="green")("echo()"))
         echo(Style(fg="green")("echo(color=None)"), color=None)
         echo(
-            Style(fg="red")("echo(color=True) bypass invoke.color = False"), color=True
+            Style(fg="red")("echo(color=True) bypass invoke.color = False"),
+            color=True,
         )
         echo(Style(fg="green")("echo(color=False)"), color=False)
 
         secho("secho()", fg="green")
         secho("secho(color=None)", fg="green", color=None)
         secho("secho(color=True) bypass invoke.color = False", fg="red", color=True)
         secho("secho(color=False)", fg="green", color=False)
@@ -153,15 +153,15 @@
         "\x1b[32mecho(color=None)\x1b[0m\n"
         "\x1b[31mecho(color=True) bypass invoke.color = False\x1b[0m\n"
         "echo(color=False)\n"
         "\x1b[32msecho()\x1b[0m\n"
         "\x1b[32msecho(color=None)\x1b[0m\n"
         "\x1b[31msecho(color=True) bypass invoke.color = False\x1b[0m\n"
         "secho(color=False)\n"
-        "\x1b[34mprint() bypass Click.\x1b[0m\n"
+        "\x1b[34mprint() bypass Click.\x1b[0m\n",
     )
     assert result.stderr == "\x1b[33mwarning\x1b[0m: Is the logger colored?\n"
 
 
 def check_default_uncolored_rendering(result):
     assert result.exit_code == 0
     assert result.stdout.startswith(
@@ -169,15 +169,15 @@
         "echo(color=None)\n"
         "\x1b[31mecho(color=True) bypass invoke.color = False\x1b[0m\n"
         "echo(color=False)\n"
         "secho()\n"
         "secho(color=None)\n"
         "\x1b[31msecho(color=True) bypass invoke.color = False\x1b[0m\n"
         "secho(color=False)\n"
-        "\x1b[34mprint() bypass Click.\x1b[0m\n"
+        "\x1b[34mprint() bypass Click.\x1b[0m\n",
     )
     assert result.stderr == "warning: Is the logger colored?\n"
 
 
 def check_forced_uncolored_rendering(result):
     assert result.exit_code == 0
     assert result.stdout.startswith(
@@ -185,63 +185,62 @@
         "echo(color=None)\n"
         "echo(color=True) bypass invoke.color = False\n"
         "echo(color=False)\n"
         "secho()\n"
         "secho(color=None)\n"
         "secho(color=True) bypass invoke.color = False\n"
         "secho(color=False)\n"
-        "print() bypass Click.\n"
+        "print() bypass Click.\n",
     )
     assert result.stderr == "warning: Is the logger colored?\n"
 
 
 @skip_windows_colors
 def test_invoke_optional_color(invoke):
     result = invoke(run_cli1, color=None)
     check_default_uncolored_rendering(result)
     assert result.stdout.endswith(
-        "Context.color = None\nclick.utils.should_strip_ansi = True\n"
+        "Context.color = None\nclick.utils.should_strip_ansi = True\n",
     )
 
 
 @skip_windows_colors
 def test_invoke_default_color(invoke):
     result = invoke(run_cli1)
     check_default_uncolored_rendering(result)
     assert result.stdout.endswith(
-        "Context.color = None\nclick.utils.should_strip_ansi = True\n"
+        "Context.color = None\nclick.utils.should_strip_ansi = True\n",
     )
 
 
 @skip_windows_colors
 def test_invoke_forced_color_stripping(invoke):
     result = invoke(run_cli1, color=False)
     check_forced_uncolored_rendering(result)
     assert result.stdout.endswith(
-        "Context.color = None\nclick.utils.should_strip_ansi = True\n"
+        "Context.color = None\nclick.utils.should_strip_ansi = True\n",
     )
 
 
 @skip_windows_colors
 def test_invoke_color_keep(invoke):
     """On Windows Click ends up deciding it is not running in an interactive terminal
     and forces the stripping of all colors."""
     result = invoke(run_cli1, color=True)
     if is_windows():
         check_default_uncolored_rendering(result)
     else:
         check_default_colored_rendering(result)
     assert result.stdout.endswith(
-        "Context.color = None\nclick.utils.should_strip_ansi = False\n"
+        "Context.color = None\nclick.utils.should_strip_ansi = False\n",
     )
 
 
 @skip_windows_colors
 def test_invoke_color_forced(invoke):
-    """Test colors are preserved while invoking, and forced to be rendered
-    on Windows.
-    """
+    """Test colors are preserved while invoking, and forced to be rendered on
+    Windows."""
     result = invoke(run_cli1, color="forced")
     check_default_colored_rendering(result)
     assert result.stdout.endswith(
-        "Context.color = True\nclick.utils.should_strip_ansi = False\n"
+        "Context.color = True\nclick.utils.should_strip_ansi = False\n",
     )
```

### Comparing `click_extra-4.3.0/click_extra/tests/test_timer.py` & `click_extra-4.4.0/click_extra/tests/test_timer.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,16 +20,17 @@
 
 import re
 from textwrap import dedent
 from time import sleep
 
 from pytest_cases import parametrize
 
-from .. import echo
-from ..decorators import extra_group, timer_option
+from click_extra import echo
+from click_extra.decorators import extra_group, timer_option
+
 from .conftest import (
     command_decorators,
 )
 
 
 @extra_group
 def integrated_timer():
@@ -94,15 +95,15 @@
     assert result.stdout == dedent(
         """\
         Usage: standalone-timer [OPTIONS]
 
         Options:
           --time / --no-time  Measure and print elapsed execution time.
           --help              Show this message and exit.
-        """
+        """,
     )
 
     result = invoke(standalone_timer, "--time")
     assert result.exit_code == 0
     assert not result.stderr
     assert re.fullmatch(
         r"It works!\nExecution time: [0-9.]+ seconds.\n",
```

### Comparing `click_extra-4.3.0/click_extra/tests/test_version.py` & `click_extra-4.4.0/click_extra/tests/test_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 
 import re
 
 import click
 import pytest
 from pytest_cases import parametrize
 
-from .. import Style, echo
-from ..decorators import color_option, extra_group, version_option
+from click_extra import Style, echo
+from click_extra.decorators import color_option, extra_group, version_option
+
 from .conftest import command_decorators, skip_windows_colors
 
 
 @skip_windows_colors
 @parametrize("cmd_decorator", command_decorators())
 @parametrize("option_decorator", (version_option, version_option()))
 def test_standalone_version_option(invoke, cmd_decorator, option_decorator):
@@ -63,15 +64,16 @@
     )
     assert re.fullmatch(regex_stdout, result.stdout)
 
     assert not result.stderr
 
 
 @pytest.mark.xfail(
-    strict=False, reason="version_option always displays click-extra version. See #176."
+    strict=False,
+    reason="version_option always displays click-extra version. See #176.",
 )
 @skip_windows_colors
 @parametrize("cmd_decorator", command_decorators(no_groups=True))
 def test_standalone_version_option_without_env_info(invoke, cmd_decorator):
     @cmd_decorator
     @version_option(version="1.2.3.4", print_env_info=False)
     def color_cli3():
@@ -84,15 +86,16 @@
         result.stdout == "\x1b[97mcolor-cli3\x1b[0m, version \x1b[32m1.2.3.4\x1b[0m\n"
     )
     assert not result.stderr
 
 
 @skip_windows_colors
 @pytest.mark.parametrize(
-    "params", (None, "--help", "blah", ("--config", "random.toml"))
+    "params",
+    (None, "--help", "blah", ("--config", "random.toml")),
 )
 def test_integrated_version_option_precedence(invoke, params):
     @extra_group(version="1.2.3.4")
     def color_cli4():
         echo("It works!")
 
     result = invoke(color_cli4, "--version", params, color=True)
```

### Comparing `click_extra-4.3.0/click_extra/timer.py` & `click_extra-4.4.0/click_extra/timer.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 
 from . import echo
 from .parameters import ExtraOption
 
 
 class TimerOption(ExtraOption):
     """A pre-configured option that is adding a ``--time``/``--no-time`` flag to print
-    elapsed time at the end of CLI execution."""
+    elapsed time at the end of CLI execution.
+    """
 
     def print_timer(self):
         """Compute and print elapsed execution time."""
         echo(f"Execution time: {perf_counter() - self.start_time:0.3f} seconds.")
 
     def register_timer_on_close(self, ctx, param, value):
         """Callback setting up all timer's machinery.
@@ -52,15 +53,15 @@
     def __init__(
         self,
         param_decls: Sequence[str] | None = None,
         default=False,
         expose_value=False,
         help=_("Measure and print elapsed execution time."),
         **kwargs,
-    ):
+    ) -> None:
         if not param_decls:
             param_decls = ("--time/--no-time",)
 
         kwargs.setdefault("callback", self.register_timer_on_close)
 
         super().__init__(
             param_decls=param_decls,
```

### Comparing `click_extra-4.3.0/click_extra/version.py` & `click_extra-4.4.0/click_extra/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 
 class VersionOption(ExtraOption):
     """Prints the colored version of the CLI.
 
     .. warning::
         This is a `copy of the standard @click.version_option() decorator
-        <https://github.com/pallets/click/blob/dc918b48fb9006be683a684b42cc7496ad649b83/src/click/decorators.py#L399-L466>`_.
+        <https://github.com/pallets/click/blob/dc918b4/src/click/decorators.py#L399-L466>`_.
 
         It has been made into a class here, to allow its use with the declarative
         ``params=`` argument. Which `fixes Click #2324 issue
         <https://github.com/pallets/click/issues/2324>`_.
     """
 
     version: str | None = None
@@ -86,24 +86,26 @@
         if self.prog_name is None:
             self.prog_name = ctx.find_root().info_name
 
         if self.version is None and self.package_name is not None:
             try:
                 self.version = metadata.version(self.package_name)
             except metadata.PackageNotFoundError:
-                raise RuntimeError(
-                    f"{self.package_name!r} is not installed. Try passing"
-                    " 'package_name' instead."
-                ) from None
+                msg = (
+                    f"{self.package_name!r} is not installed. Try passing "
+                    "'package_name' instead."
+                )
+                raise RuntimeError(msg) from None
 
         if self.version is None:
-            raise RuntimeError(
-                f"Could not determine the version for "
-                f"{self.package_name!r} automatically."
+            msg = (
+                f"Could not determine the version for {self.package_name!r} "
+                "automatically."
             )
+            raise RuntimeError(msg)
 
         output = self.message % {
             "prog": self.prog_name,
             "package": self.package_name,
             "version": self.version,
         }
 
@@ -112,14 +114,15 @@
 
         echo(output, color=ctx.color)
 
         # Do not just ctx.exit() as it will prevent callbacks defined on options
         # to be called.
         ctx.close()
         ctx.exit()
+        return None  # type: ignore[unreachable]
 
     def __init__(
         self,
         param_decls: Sequence[str] | None = None,
         version: str | None = None,
         package_name: str | None = None,
         prog_name: str | None = None,
```

### Comparing `click_extra-4.3.0/pyproject.toml` & `click_extra-4.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 # Docs: https://python-poetry.org/docs/pyproject/
 name = "click-extra"
-version = "4.3.0"
+version = "4.4.0"
 description = "🌈 Extra colorization and configuration loading for Click."
 license = 'GPL-2.0-or-later'
 authors = ["Kevin Deldycke <kevin@deldycke.com>"]
 readme = "readme.md"
 homepage = 'https://github.com/kdeldycke/click-extra'
 repository = 'https://github.com/kdeldycke/click-extra'
 documentation = 'https://kdeldycke.github.io/click-extra'
@@ -70,20 +70,20 @@
 python = "^3.8"
 # XXX boltons.ecoutils 23.0.0 breaks PDB interactive sessions in pytest.
 # Investigation of the root cause is being discussed upstream at:
 # https://github.com/mahmoud/boltons/issues/334
 boltons = "^23.0.0"
 # Click 8.1 is the first version to support ``params=`` in ``@command``.
 click = "^8.1"
-# Cloup 2.1.0 introduced colorization of subcommand aliases.
-cloup = "^2.1.0"
+# Cloup 2.1.1 fix heading colorization.
+cloup = "^2.1.1"
 commentjson = "^0.9.0"
 mergedeep = "^1.3.4"
-# Pallets-Sphinx-Themes 2.1.0 is the first version rendering ``.. sourcecode:: shell-session`` code-blocks.
-Pallets-Sphinx-Themes = "^2.1.0"
+# Pallets-Sphinx-Themes 2.1.1 is the first version removing old and conflicting Python 2 code.
+Pallets-Sphinx-Themes = "^2.1.1"
 # Pygments 2.14.0 is the first version with ``lexers.algebra.GAPConsoleLexer`` that is referenced in our code.
 pygments = "^2.14"
 # pygments-ansi-color 0.3.0 is the first version to set the default theme of ANSI colors.
 pygments-ansi-color = "^0.3.0"
 pyyaml = "^6.0.0"
 # regex is required for case-insensitive matches in Unicode.
 # v2023.3.22 is the first to drop Python 3.7.
@@ -95,19 +95,18 @@
 # tabulate 0.9 is the first to add `*grid` and `*outline` formats.
 tabulate = { extras = ["widechars"], version = "^0.9" }
 tomli = { version = "^2.0.1", python = "< 3.11" }
 wcmatch = "^8.4.1"
 xmltodict = "^0.13.0"
 
 [tool.poetry.group.dev.dependencies]
-bump2version = "^1.0.1"
 coverage = { extras = ["toml"], version = "^7.2.3" }
 furo = "^2023.05.20"
 mypy = "^1.2.0"
-myst-parser = "^1.0.0"
+myst-parser = ">=1,<3"
 pytest = "^7.3.1"
 # More pytest plugins at: https://docs.pytest.org/en/latest/reference/plugin_list.html
 pytest-cases = "^3.6.14"
 pytest-cov = "^4.0.0"
 pytest-httpserver = "^1.0.6"
 pytest-randomly = "^3.12.0"
 sphinx-autodoc-typehints = "^1.23.0"
@@ -179,10 +178,32 @@
 
 # https://coverage.readthedocs.io/en/latest/config.html
 [tool.coverage.run]
 branch = true
 [tool.coverage.report]
 precision = 2
 
+[tool.bumpversion]
+current_version = "4.4.0"
+allow_dirty = true
+
+[[tool.bumpversion.files]]
+filename = "./click_extra/__init__.py"
+
+[[tool.bumpversion.files]]
+filename = "./pyproject.toml"
+search = 'version = "{current_version}"'
+replace = 'version = "{new_version}"'
+
+[[tool.bumpversion.files]]
+filename = "./changelog.md"
+search = "{{gh}}`{current_version} (unreleased)"
+replace = "{{gh}}`{new_version} (unreleased)"
+
+[[tool.bumpversion.files]]
+filename = "./citation.cff"
+search = "version: {current_version}"
+replace = "version: {new_version}"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `click_extra-4.3.0/readme.md` & `click_extra-4.4.0/readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,34 +5,34 @@
 </p>
 
 [![Last release](https://img.shields.io/pypi/v/click-extra.svg)](https://pypi.python.org/pypi/click-extra)
 [![Python versions](https://img.shields.io/pypi/pyversions/click-extra.svg)](https://pypi.python.org/pypi/click-extra)
 [![Unittests status](https://github.com/kdeldycke/click-extra/actions/workflows/tests.yaml/badge.svg?branch=main)](https://github.com/kdeldycke/click-extra/actions/workflows/tests.yaml?query=branch%3Amain)
 [![Documentation status](https://github.com/kdeldycke/click-extra/actions/workflows/docs.yaml/badge.svg?branch=main)](https://github.com/kdeldycke/click-extra/actions/workflows/docs.yaml?query=branch%3Amain)
 [![Coverage status](https://codecov.io/gh/kdeldycke/click-extra/branch/main/graph/badge.svg)](https://app.codecov.io/gh/kdeldycke/click-extra)
-[![DOI](https://zenodo.org/badge/418402236.svg)](https://zenodo.org/badge/latestdoi/418402236)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7116050.svg)](https://doi.org/10.5281/zenodo.7116050)
 
 ## What is Click Extra?
 
 A ready-to-use wrapper for [Click](https://click.palletsprojects.com), the Python CLI framework.
 
 It is a drop-in replacement with good defaults that saves lots of boilerplate code and frustration.
 It also comes with
 [workarounds and patches](https://kdeldycke.github.io/click-extra/issues.html) that have not
 reached upstream yet (or are unlikely to).
 
 ## Example
 
 It transforms this vanilla `click` CLI:
 
-![click CLI help screen](https://github.com/kdeldycke/click-extra/raw/main/docs/assets/click-help-screen.png)
+![click CLI help screen](https://raw.githubusercontent.com/kdeldycke/click-extra/main/docs/assets/click-help-screen.png)
 
 Into this:
 
-![click-extra CLI help screen](https://github.com/kdeldycke/click-extra/raw/main/docs/assets/click-extra-screen.png)
+![click-extra CLI help screen](https://raw.githubusercontent.com/kdeldycke/click-extra/main/docs/assets/click-extra-screen.png)
 
 To undestrand how we ended up with the result above, [go read the tutorial](https://kdeldycke.github.io/click-extra/tutorial.html).
 
 ## Features
 
 - [Configuration file](https://kdeldycke.github.io/click-extra/config.html) loader for:
   - `TOML`
@@ -61,15 +61,14 @@
 - [Colored `--verbosity` option and logs](https://kdeldycke.github.io/click-extra/logging.html)
 - `--time`/`--no-time` flag to measure duration of command execution
 - Global `show_choices` to activate selection of choices on user input prompts
 - [Platform recognition](https://kdeldycke.github.io/click-extra/platforms.html) utilities (macOS, Linux, Windows, UNIX, \*BSD, …)
 - New conditional markers for `pytest`:
   - `@skip_linux`, `@skip_macos` and `@skip_windows`
   - `@unless_linux`, `@unless_macos` and `@unless_windows`
-  - `@destructive` and `@non_destructive`
 - [`.. click:example::` and `.. click:run::` Sphinx directives](https://kdeldycke.github.io/click-extra/sphinx.html) to document CLI source code and their execution
 - [Inline testing of CLI examples](https://kdeldycke.github.io/click-extra/sphinx.html#inline-tests) in documentation
 - [ANSI-capable Pygments lexers](https://kdeldycke.github.io/click-extra/pygments.html#lexers) for shell session and console output
 - [Fixes 40+ bugs](https://kdeldycke.github.io/click-extra/issues.html) from other Click-related projects
 - Rely on [Cloup](https://github.com/janluke/cloup) to add:
   - option groups
   - constraints
```

#### html2text {}

```diff
@@ -5,24 +5,25 @@
 [Unittests status](https://github.com/kdeldycke/click-extra/actions/workflows/
 tests.yaml/badge.svg?branch=main)](https://github.com/kdeldycke/click-extra/
 actions/workflows/tests.yaml?query=branch%3Amain) [![Documentation status]
 (https://github.com/kdeldycke/click-extra/actions/workflows/docs.yaml/
 badge.svg?branch=main)](https://github.com/kdeldycke/click-extra/actions/
 workflows/docs.yaml?query=branch%3Amain) [![Coverage status](https://
 codecov.io/gh/kdeldycke/click-extra/branch/main/graph/badge.svg)](https://
-app.codecov.io/gh/kdeldycke/click-extra) [![DOI](https://zenodo.org/badge/
-418402236.svg)](https://zenodo.org/badge/latestdoi/418402236) ## What is Click
-Extra? A ready-to-use wrapper for [Click](https://click.palletsprojects.com),
-the Python CLI framework. It is a drop-in replacement with good defaults that
-saves lots of boilerplate code and frustration. It also comes with [workarounds
-and patches](https://kdeldycke.github.io/click-extra/issues.html) that have not
-reached upstream yet (or are unlikely to). ## Example It transforms this
-vanilla `click` CLI: ![click CLI help screen](https://github.com/kdeldycke/
-click-extra/raw/main/docs/assets/click-help-screen.png) Into this: ![click-
-extra CLI help screen](https://github.com/kdeldycke/click-extra/raw/main/docs/
+app.codecov.io/gh/kdeldycke/click-extra) [![DOI](https://zenodo.org/badge/DOI/
+10.5281/zenodo.7116050.svg)](https://doi.org/10.5281/zenodo.7116050) ## What is
+Click Extra? A ready-to-use wrapper for [Click](https://
+click.palletsprojects.com), the Python CLI framework. It is a drop-in
+replacement with good defaults that saves lots of boilerplate code and
+frustration. It also comes with [workarounds and patches](https://
+kdeldycke.github.io/click-extra/issues.html) that have not reached upstream yet
+(or are unlikely to). ## Example It transforms this vanilla `click` CLI: !
+[click CLI help screen](https://raw.githubusercontent.com/kdeldycke/click-
+extra/main/docs/assets/click-help-screen.png) Into this: ![click-extra CLI help
+screen](https://raw.githubusercontent.com/kdeldycke/click-extra/main/docs/
 assets/click-extra-screen.png) To undestrand how we ended up with the result
 above, [go read the tutorial](https://kdeldycke.github.io/click-extra/
 tutorial.html). ## Features - [Configuration file](https://kdeldycke.github.io/
 click-extra/config.html) loader for: - `TOML` - `YAML` - `JSON`, with inline
 and block comments (Python-style `#` and Javascript-style `//`) - `INI`, with
 extended interpolation, multi-level sections and non-native types (`list`,
 `set`, â¦) - `XML` - Automatic inference of the configuration file structure
@@ -51,36 +52,35 @@
 [`consoledonottrack.com`](https://consoledonottrack.com) - Colored `--version`
 option - [Colored `--verbosity` option and logs](https://kdeldycke.github.io/
 click-extra/logging.html) - `--time`/`--no-time` flag to measure duration of
 command execution - Global `show_choices` to activate selection of choices on
 user input prompts - [Platform recognition](https://kdeldycke.github.io/click-
 extra/platforms.html) utilities (macOS, Linux, Windows, UNIX, \*BSD, â¦) - New
 conditional markers for `pytest`: - `@skip_linux`, `@skip_macos` and
-`@skip_windows` - `@unless_linux`, `@unless_macos` and `@unless_windows` -
-`@destructive` and `@non_destructive` - [`.. click:example::` and `.. click:
-run::` Sphinx directives](https://kdeldycke.github.io/click-extra/sphinx.html)
-to document CLI source code and their execution - [Inline testing of CLI
-examples](https://kdeldycke.github.io/click-extra/sphinx.html#inline-tests) in
-documentation - [ANSI-capable Pygments lexers](https://kdeldycke.github.io/
-click-extra/pygments.html#lexers) for shell session and console output - [Fixes
-40+ bugs](https://kdeldycke.github.io/click-extra/issues.html) from other
-Click-related projects - Rely on [Cloup](https://github.com/janluke/cloup) to
-add: - option groups - constraints - subcommands sections - aliases - command
-suggestion (`Did you mean ?`) ## Used in Check these projects to get real-life
-examples of `click-extra` usage: - ![GitHub stars](https://img.shields.io/
-github/stars/kdeldycke/meta-package-manager?label=%E2%AD%90&style=flat-square)
-[Meta Package Manager](https://github.com/kdeldycke/meta-package-
-manager#readme) \- A unifying CLI for multiple package managers. - ![GitHub
-stars](https://img.shields.io/github/stars/kdeldycke/mail-
-deduplicate?label=%E2%AD%90&style=flat-square) [Mail Deduplicate](https://
-github.com/kdeldycke/mail-deduplicate#readme) - A CLI to deduplicate similar
-emails. - ![GitHub stars](https://img.shields.io/github/stars/Sprocket-
-Security/fireproxng?label=%E2%AD%90&style=flat-square) [fireproxng](https://
-github.com/Sprocket-Security/fireproxng#readme) - A rewrite of the fireprox
-tool. - ![GitHub stars](https://img.shields.io/github/stars/hugolundin/
-badger?label=%E2%AD%90&style=flat-square) [badger-proxy](https://github.com/
-hugolundin/badger#readme) - An mDNS-based reverse proxy for naming services on
-a local network. Feel free to send a PR to add your project in this list if you
-are relying on Click Extra in any way. ## Development [Development guidelines]
-(https://kdeldycke.github.io/meta-package-manager/development.html) are the
-same as [parent project `mpm`](https://github.com/kdeldycke/meta-package-
-manager), from which `click-extra` originated.
+`@skip_windows` - `@unless_linux`, `@unless_macos` and `@unless_windows` - [`..
+click:example::` and `.. click:run::` Sphinx directives](https://
+kdeldycke.github.io/click-extra/sphinx.html) to document CLI source code and
+their execution - [Inline testing of CLI examples](https://kdeldycke.github.io/
+click-extra/sphinx.html#inline-tests) in documentation - [ANSI-capable Pygments
+lexers](https://kdeldycke.github.io/click-extra/pygments.html#lexers) for shell
+session and console output - [Fixes 40+ bugs](https://kdeldycke.github.io/
+click-extra/issues.html) from other Click-related projects - Rely on [Cloup]
+(https://github.com/janluke/cloup) to add: - option groups - constraints -
+subcommands sections - aliases - command suggestion (`Did you mean ?`) ## Used
+in Check these projects to get real-life examples of `click-extra` usage: - !
+[GitHub stars](https://img.shields.io/github/stars/kdeldycke/meta-package-
+manager?label=%E2%AD%90&style=flat-square) [Meta Package Manager](https://
+github.com/kdeldycke/meta-package-manager#readme) \- A unifying CLI for
+multiple package managers. - ![GitHub stars](https://img.shields.io/github/
+stars/kdeldycke/mail-deduplicate?label=%E2%AD%90&style=flat-square) [Mail
+Deduplicate](https://github.com/kdeldycke/mail-deduplicate#readme) - A CLI to
+deduplicate similar emails. - ![GitHub stars](https://img.shields.io/github/
+stars/Sprocket-Security/fireproxng?label=%E2%AD%90&style=flat-square)
+[fireproxng](https://github.com/Sprocket-Security/fireproxng#readme) - A
+rewrite of the fireprox tool. - ![GitHub stars](https://img.shields.io/github/
+stars/hugolundin/badger?label=%E2%AD%90&style=flat-square) [badger-proxy]
+(https://github.com/hugolundin/badger#readme) - An mDNS-based reverse proxy for
+naming services on a local network. Feel free to send a PR to add your project
+in this list if you are relying on Click Extra in any way. ## Development
+[Development guidelines](https://kdeldycke.github.io/meta-package-manager/
+development.html) are the same as [parent project `mpm`](https://github.com/
+kdeldycke/meta-package-manager), from which `click-extra` originated.
```

### Comparing `click_extra-4.3.0/PKG-INFO` & `click_extra-4.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click-extra
-Version: 4.3.0
+Version: 4.4.0
 Summary: 🌈 Extra colorization and configuration loading for Click.
 Home-page: https://github.com/kdeldycke/click-extra
 License: GPL-2.0-or-later
 Keywords: ansi-colors,cli,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-tabulate,sphinx,terminal,toml,xml,yaml
 Author: Kevin Deldycke
 Author-email: kevin@deldycke.com
 Requires-Python: >=3.8,<4.0
@@ -35,18 +35,18 @@
 Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: Topic :: Text Processing :: Markup :: reStructuredText
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Dist: Pallets-Sphinx-Themes (>=2.1.0,<3.0.0)
+Requires-Dist: Pallets-Sphinx-Themes (>=2.1.1,<3.0.0)
 Requires-Dist: boltons (>=23.0.0,<24.0.0)
 Requires-Dist: click (>=8.1,<9.0)
-Requires-Dist: cloup (>=2.1.0,<3.0.0)
+Requires-Dist: cloup (>=2.1.1,<3.0.0)
 Requires-Dist: commentjson (>=0.9.0,<0.10.0)
 Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
 Requires-Dist: pygments (>=2.14,<3.0)
 Requires-Dist: pygments-ansi-color (>=0.3.0,<0.4.0)
 Requires-Dist: pyyaml (>=6.0.0,<7.0.0)
 Requires-Dist: regex (>=2023.3.22,<2024.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
@@ -69,34 +69,34 @@
 </p>
 
 [![Last release](https://img.shields.io/pypi/v/click-extra.svg)](https://pypi.python.org/pypi/click-extra)
 [![Python versions](https://img.shields.io/pypi/pyversions/click-extra.svg)](https://pypi.python.org/pypi/click-extra)
 [![Unittests status](https://github.com/kdeldycke/click-extra/actions/workflows/tests.yaml/badge.svg?branch=main)](https://github.com/kdeldycke/click-extra/actions/workflows/tests.yaml?query=branch%3Amain)
 [![Documentation status](https://github.com/kdeldycke/click-extra/actions/workflows/docs.yaml/badge.svg?branch=main)](https://github.com/kdeldycke/click-extra/actions/workflows/docs.yaml?query=branch%3Amain)
 [![Coverage status](https://codecov.io/gh/kdeldycke/click-extra/branch/main/graph/badge.svg)](https://app.codecov.io/gh/kdeldycke/click-extra)
-[![DOI](https://zenodo.org/badge/418402236.svg)](https://zenodo.org/badge/latestdoi/418402236)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7116050.svg)](https://doi.org/10.5281/zenodo.7116050)
 
 ## What is Click Extra?
 
 A ready-to-use wrapper for [Click](https://click.palletsprojects.com), the Python CLI framework.
 
 It is a drop-in replacement with good defaults that saves lots of boilerplate code and frustration.
 It also comes with
 [workarounds and patches](https://kdeldycke.github.io/click-extra/issues.html) that have not
 reached upstream yet (or are unlikely to).
 
 ## Example
 
 It transforms this vanilla `click` CLI:
 
-![click CLI help screen](https://github.com/kdeldycke/click-extra/raw/main/docs/assets/click-help-screen.png)
+![click CLI help screen](https://raw.githubusercontent.com/kdeldycke/click-extra/main/docs/assets/click-help-screen.png)
 
 Into this:
 
-![click-extra CLI help screen](https://github.com/kdeldycke/click-extra/raw/main/docs/assets/click-extra-screen.png)
+![click-extra CLI help screen](https://raw.githubusercontent.com/kdeldycke/click-extra/main/docs/assets/click-extra-screen.png)
 
 To undestrand how we ended up with the result above, [go read the tutorial](https://kdeldycke.github.io/click-extra/tutorial.html).
 
 ## Features
 
 - [Configuration file](https://kdeldycke.github.io/click-extra/config.html) loader for:
   - `TOML`
@@ -125,15 +125,14 @@
 - [Colored `--verbosity` option and logs](https://kdeldycke.github.io/click-extra/logging.html)
 - `--time`/`--no-time` flag to measure duration of command execution
 - Global `show_choices` to activate selection of choices on user input prompts
 - [Platform recognition](https://kdeldycke.github.io/click-extra/platforms.html) utilities (macOS, Linux, Windows, UNIX, \*BSD, …)
 - New conditional markers for `pytest`:
   - `@skip_linux`, `@skip_macos` and `@skip_windows`
   - `@unless_linux`, `@unless_macos` and `@unless_windows`
-  - `@destructive` and `@non_destructive`
 - [`.. click:example::` and `.. click:run::` Sphinx directives](https://kdeldycke.github.io/click-extra/sphinx.html) to document CLI source code and their execution
 - [Inline testing of CLI examples](https://kdeldycke.github.io/click-extra/sphinx.html#inline-tests) in documentation
 - [ANSI-capable Pygments lexers](https://kdeldycke.github.io/click-extra/pygments.html#lexers) for shell session and console output
 - [Fixes 40+ bugs](https://kdeldycke.github.io/click-extra/issues.html) from other Click-related projects
 - Rely on [Cloup](https://github.com/janluke/cloup) to add:
   - option groups
   - constraints
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: click-extra Version: 4.3.0 Summary: ð Extra
+Metadata-Version: 2.1 Name: click-extra Version: 4.4.0 Summary: ð Extra
 colorization and configuration loading for Click. Home-page: https://
 github.com/kdeldycke/click-extra License: GPL-2.0-or-later Keywords: ansi-
 colors,cli,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-
 tabulate,sphinx,terminal,toml,xml,yaml Author: Kevin Deldycke Author-email:
 kevin@deldycke.com Requires-Python: >=3.8,<4.0 Classifier: Development Status
 :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Environment :: Plugins Classifier: Framework :: Pytest Classifier: Framework ::
@@ -20,16 +20,16 @@
 Software Development :: User Interfaces Classifier: Topic :: System :: Logging
 Classifier: Topic :: System :: Shells Classifier: Topic :: Terminals
 Classifier: Topic :: Text Processing :: Filters Classifier: Topic :: Text
 Processing :: Markup :: HTML Classifier: Topic :: Text Processing :: Markup ::
 Markdown Classifier: Topic :: Text Processing :: Markup :: XML Classifier:
 Topic :: Text Processing :: Markup :: reStructuredText Classifier: Topic ::
 Utilities Classifier: Typing :: Typed Requires-Dist: Pallets-Sphinx-Themes
-(>=2.1.0,<3.0.0) Requires-Dist: boltons (>=23.0.0,<24.0.0) Requires-Dist: click
-(>=8.1,<9.0) Requires-Dist: cloup (>=2.1.0,<3.0.0) Requires-Dist: commentjson
+(>=2.1.1,<3.0.0) Requires-Dist: boltons (>=23.0.0,<24.0.0) Requires-Dist: click
+(>=8.1,<9.0) Requires-Dist: cloup (>=2.1.1,<3.0.0) Requires-Dist: commentjson
 (>=0.9.0,<0.10.0) Requires-Dist: mergedeep (>=1.3.4,<2.0.0) Requires-Dist:
 pygments (>=2.14,<3.0) Requires-Dist: pygments-ansi-color (>=0.3.0,<0.4.0)
 Requires-Dist: pyyaml (>=6.0.0,<7.0.0) Requires-Dist: regex
 (>=2023.3.22,<2024.0.0) Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-
 Dist: sphinx (>=6,<7) Requires-Dist: tabulate[widechars] (>=0.9,<0.10)
 Requires-Dist: tomli (>=2.0.1,<3.0.0) ; python_version < "3.11" Requires-Dist:
 wcmatch (>=8.4.1,<9.0.0) Requires-Dist: xmltodict (>=0.13.0,<0.14.0) Project-
@@ -45,24 +45,25 @@
 [Unittests status](https://github.com/kdeldycke/click-extra/actions/workflows/
 tests.yaml/badge.svg?branch=main)](https://github.com/kdeldycke/click-extra/
 actions/workflows/tests.yaml?query=branch%3Amain) [![Documentation status]
 (https://github.com/kdeldycke/click-extra/actions/workflows/docs.yaml/
 badge.svg?branch=main)](https://github.com/kdeldycke/click-extra/actions/
 workflows/docs.yaml?query=branch%3Amain) [![Coverage status](https://
 codecov.io/gh/kdeldycke/click-extra/branch/main/graph/badge.svg)](https://
-app.codecov.io/gh/kdeldycke/click-extra) [![DOI](https://zenodo.org/badge/
-418402236.svg)](https://zenodo.org/badge/latestdoi/418402236) ## What is Click
-Extra? A ready-to-use wrapper for [Click](https://click.palletsprojects.com),
-the Python CLI framework. It is a drop-in replacement with good defaults that
-saves lots of boilerplate code and frustration. It also comes with [workarounds
-and patches](https://kdeldycke.github.io/click-extra/issues.html) that have not
-reached upstream yet (or are unlikely to). ## Example It transforms this
-vanilla `click` CLI: ![click CLI help screen](https://github.com/kdeldycke/
-click-extra/raw/main/docs/assets/click-help-screen.png) Into this: ![click-
-extra CLI help screen](https://github.com/kdeldycke/click-extra/raw/main/docs/
+app.codecov.io/gh/kdeldycke/click-extra) [![DOI](https://zenodo.org/badge/DOI/
+10.5281/zenodo.7116050.svg)](https://doi.org/10.5281/zenodo.7116050) ## What is
+Click Extra? A ready-to-use wrapper for [Click](https://
+click.palletsprojects.com), the Python CLI framework. It is a drop-in
+replacement with good defaults that saves lots of boilerplate code and
+frustration. It also comes with [workarounds and patches](https://
+kdeldycke.github.io/click-extra/issues.html) that have not reached upstream yet
+(or are unlikely to). ## Example It transforms this vanilla `click` CLI: !
+[click CLI help screen](https://raw.githubusercontent.com/kdeldycke/click-
+extra/main/docs/assets/click-help-screen.png) Into this: ![click-extra CLI help
+screen](https://raw.githubusercontent.com/kdeldycke/click-extra/main/docs/
 assets/click-extra-screen.png) To undestrand how we ended up with the result
 above, [go read the tutorial](https://kdeldycke.github.io/click-extra/
 tutorial.html). ## Features - [Configuration file](https://kdeldycke.github.io/
 click-extra/config.html) loader for: - `TOML` - `YAML` - `JSON`, with inline
 and block comments (Python-style `#` and Javascript-style `//`) - `INI`, with
 extended interpolation, multi-level sections and non-native types (`list`,
 `set`, â¦) - `XML` - Automatic inference of the configuration file structure
@@ -91,36 +92,35 @@
 [`consoledonottrack.com`](https://consoledonottrack.com) - Colored `--version`
 option - [Colored `--verbosity` option and logs](https://kdeldycke.github.io/
 click-extra/logging.html) - `--time`/`--no-time` flag to measure duration of
 command execution - Global `show_choices` to activate selection of choices on
 user input prompts - [Platform recognition](https://kdeldycke.github.io/click-
 extra/platforms.html) utilities (macOS, Linux, Windows, UNIX, \*BSD, â¦) - New
 conditional markers for `pytest`: - `@skip_linux`, `@skip_macos` and
-`@skip_windows` - `@unless_linux`, `@unless_macos` and `@unless_windows` -
-`@destructive` and `@non_destructive` - [`.. click:example::` and `.. click:
-run::` Sphinx directives](https://kdeldycke.github.io/click-extra/sphinx.html)
-to document CLI source code and their execution - [Inline testing of CLI
-examples](https://kdeldycke.github.io/click-extra/sphinx.html#inline-tests) in
-documentation - [ANSI-capable Pygments lexers](https://kdeldycke.github.io/
-click-extra/pygments.html#lexers) for shell session and console output - [Fixes
-40+ bugs](https://kdeldycke.github.io/click-extra/issues.html) from other
-Click-related projects - Rely on [Cloup](https://github.com/janluke/cloup) to
-add: - option groups - constraints - subcommands sections - aliases - command
-suggestion (`Did you mean ?`) ## Used in Check these projects to get real-life
-examples of `click-extra` usage: - ![GitHub stars](https://img.shields.io/
-github/stars/kdeldycke/meta-package-manager?label=%E2%AD%90&style=flat-square)
-[Meta Package Manager](https://github.com/kdeldycke/meta-package-
-manager#readme) \- A unifying CLI for multiple package managers. - ![GitHub
-stars](https://img.shields.io/github/stars/kdeldycke/mail-
-deduplicate?label=%E2%AD%90&style=flat-square) [Mail Deduplicate](https://
-github.com/kdeldycke/mail-deduplicate#readme) - A CLI to deduplicate similar
-emails. - ![GitHub stars](https://img.shields.io/github/stars/Sprocket-
-Security/fireproxng?label=%E2%AD%90&style=flat-square) [fireproxng](https://
-github.com/Sprocket-Security/fireproxng#readme) - A rewrite of the fireprox
-tool. - ![GitHub stars](https://img.shields.io/github/stars/hugolundin/
-badger?label=%E2%AD%90&style=flat-square) [badger-proxy](https://github.com/
-hugolundin/badger#readme) - An mDNS-based reverse proxy for naming services on
-a local network. Feel free to send a PR to add your project in this list if you
-are relying on Click Extra in any way. ## Development [Development guidelines]
-(https://kdeldycke.github.io/meta-package-manager/development.html) are the
-same as [parent project `mpm`](https://github.com/kdeldycke/meta-package-
-manager), from which `click-extra` originated.
+`@skip_windows` - `@unless_linux`, `@unless_macos` and `@unless_windows` - [`..
+click:example::` and `.. click:run::` Sphinx directives](https://
+kdeldycke.github.io/click-extra/sphinx.html) to document CLI source code and
+their execution - [Inline testing of CLI examples](https://kdeldycke.github.io/
+click-extra/sphinx.html#inline-tests) in documentation - [ANSI-capable Pygments
+lexers](https://kdeldycke.github.io/click-extra/pygments.html#lexers) for shell
+session and console output - [Fixes 40+ bugs](https://kdeldycke.github.io/
+click-extra/issues.html) from other Click-related projects - Rely on [Cloup]
+(https://github.com/janluke/cloup) to add: - option groups - constraints -
+subcommands sections - aliases - command suggestion (`Did you mean ?`) ## Used
+in Check these projects to get real-life examples of `click-extra` usage: - !
+[GitHub stars](https://img.shields.io/github/stars/kdeldycke/meta-package-
+manager?label=%E2%AD%90&style=flat-square) [Meta Package Manager](https://
+github.com/kdeldycke/meta-package-manager#readme) \- A unifying CLI for
+multiple package managers. - ![GitHub stars](https://img.shields.io/github/
+stars/kdeldycke/mail-deduplicate?label=%E2%AD%90&style=flat-square) [Mail
+Deduplicate](https://github.com/kdeldycke/mail-deduplicate#readme) - A CLI to
+deduplicate similar emails. - ![GitHub stars](https://img.shields.io/github/
+stars/Sprocket-Security/fireproxng?label=%E2%AD%90&style=flat-square)
+[fireproxng](https://github.com/Sprocket-Security/fireproxng#readme) - A
+rewrite of the fireprox tool. - ![GitHub stars](https://img.shields.io/github/
+stars/hugolundin/badger?label=%E2%AD%90&style=flat-square) [badger-proxy]
+(https://github.com/hugolundin/badger#readme) - An mDNS-based reverse proxy for
+naming services on a local network. Feel free to send a PR to add your project
+in this list if you are relying on Click Extra in any way. ## Development
+[Development guidelines](https://kdeldycke.github.io/meta-package-manager/
+development.html) are the same as [parent project `mpm`](https://github.com/
+kdeldycke/meta-package-manager), from which `click-extra` originated.
```

