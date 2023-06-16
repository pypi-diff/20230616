# Comparing `tmp/wom_py-0.4.1.tar.gz` & `tmp/wom_py-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wom_py-0.4.1.tar", max compression
+gzip compressed data, was "wom_py-0.4.2.tar", max compression
```

## Comparing `wom_py-0.4.1.tar` & `wom_py-0.4.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1074 2023-05-23 00:08:59.093807 wom_py-0.4.1/LICENSE
--rw-r--r--   0        0        0     2712 2023-05-23 00:08:59.093807 wom_py-0.4.1/README.md
--rw-r--r--   0        0        0     2138 2023-05-23 00:08:59.093807 wom_py-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     4385 2023-05-23 00:08:59.173811 wom_py-0.4.1/wom/__init__.py
--rw-r--r--   0        0        0     1324 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/__main__.py
--rw-r--r--   0        0        0     1808 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/_cli.py
--rw-r--r--   0        0        0     8648 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/client.py
--rw-r--r--   0        0        0     1447 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/constants.py
--rw-r--r--   0        0        0     7010 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/enums.py
--rw-r--r--   0        0        0     1729 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/errors.py
--rw-r--r--   0        0        0     3228 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/__init__.py
--rw-r--r--   0        0        0     1557 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/base.py
--rw-r--r--   0        0        0     1673 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/competitions/__init__.py
--rw-r--r--   0        0        0     1591 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/competitions/enums.py
--rw-r--r--   0        0        0     7413 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/competitions/models.py
--rw-r--r--   0        0        0     1289 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/deltas/__init__.py
--rw-r--r--   0        0        0     1824 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/deltas/models.py
--rw-r--r--   0        0        0     1716 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/groups/__init__.py
--rw-r--r--   0        0        0     7780 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/groups/enums.py
--rw-r--r--   0        0        0     9275 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/groups/models.py
--rw-r--r--   0        0        0     1738 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/http.py
--rw-r--r--   0        0        0     1471 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/names/__init__.py
--rw-r--r--   0        0        0     1793 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/names/enums.py
--rw-r--r--   0        0        0     5138 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/names/models.py
--rw-r--r--   0        0        0     1754 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/players/__init__.py
--rw-r--r--   0        0        0     5664 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/players/enums.py
--rw-r--r--   0        0        0    11907 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/players/models.py
--rw-r--r--   0        0        0     1300 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/records/__init__.py
--rw-r--r--   0        0        0     2217 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/models/records/models.py
--rw-r--r--   0        0        0        0 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/py.typed
--rw-r--r--   0        0        0     5561 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/result.py
--rw-r--r--   0        0        0     6505 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/routes.py
--rw-r--r--   0        0        0    34477 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/serializer.py
--rw-r--r--   0        0        0     1709 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/services/__init__.py
--rw-r--r--   0        0        0     2050 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/services/base.py
--rw-r--r--   0        0        0    21170 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/services/competitions.py
--rw-r--r--   0        0        0     3528 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/services/deltas.py
--rw-r--r--   0        0        0     3688 2023-05-23 00:08:59.097808 wom_py-0.4.1/wom/services/efficiency.py
--rw-r--r--   0        0        0    24099 2023-05-23 00:08:59.101808 wom_py-0.4.1/wom/services/groups.py
--rw-r--r--   0        0        0     5772 2023-05-23 00:08:59.101808 wom_py-0.4.1/wom/services/http.py
--rw-r--r--   0        0        0     4031 2023-05-23 00:08:59.101808 wom_py-0.4.1/wom/services/names.py
--rw-r--r--   0        0        0    18088 2023-05-23 00:08:59.101808 wom_py-0.4.1/wom/services/players.py
--rw-r--r--   0        0        0     3506 2023-05-23 00:08:59.101808 wom_py-0.4.1/wom/services/records.py
--rw-r--r--   0        0        0     3828 1970-01-01 00:00:00.000000 wom_py-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-16 02:46:15.366136 wom_py-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2712 2023-06-16 02:46:15.366136 wom_py-0.4.2/README.md
+-rw-r--r--   0        0        0     2157 2023-06-16 02:46:15.370136 wom_py-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     4385 2023-06-16 02:46:15.450135 wom_py-0.4.2/wom/__init__.py
+-rw-r--r--   0        0        0     1324 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/__main__.py
+-rw-r--r--   0        0        0     1808 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/_cli.py
+-rw-r--r--   0        0        0     8648 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/client.py
+-rw-r--r--   0        0        0     1447 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/constants.py
+-rw-r--r--   0        0        0     7388 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/enums.py
+-rw-r--r--   0        0        0     1729 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/errors.py
+-rw-r--r--   0        0        0     3228 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/__init__.py
+-rw-r--r--   0        0        0     1557 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/base.py
+-rw-r--r--   0        0        0     1673 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/competitions/__init__.py
+-rw-r--r--   0        0        0     1591 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/competitions/enums.py
+-rw-r--r--   0        0        0     7413 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/competitions/models.py
+-rw-r--r--   0        0        0     1289 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/deltas/__init__.py
+-rw-r--r--   0        0        0     1824 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/deltas/models.py
+-rw-r--r--   0        0        0     1716 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/groups/__init__.py
+-rw-r--r--   0        0        0     7780 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/groups/enums.py
+-rw-r--r--   0        0        0     9275 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/groups/models.py
+-rw-r--r--   0        0        0     1738 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/http.py
+-rw-r--r--   0        0        0     1471 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/names/__init__.py
+-rw-r--r--   0        0        0     1793 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/names/enums.py
+-rw-r--r--   0        0        0     4894 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/names/models.py
+-rw-r--r--   0        0        0     1754 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/players/__init__.py
+-rw-r--r--   0        0        0     5686 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/players/enums.py
+-rw-r--r--   0        0        0    11907 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/players/models.py
+-rw-r--r--   0        0        0     1300 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/records/__init__.py
+-rw-r--r--   0        0        0     2217 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/models/records/models.py
+-rw-r--r--   0        0        0        0 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/py.typed
+-rw-r--r--   0        0        0     5561 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/result.py
+-rw-r--r--   0        0        0     6505 2023-06-16 02:46:15.370136 wom_py-0.4.2/wom/routes.py
+-rw-r--r--   0        0        0    34477 2023-06-16 02:46:15.374136 wom_py-0.4.2/wom/serializer.py
+-rw-r--r--   0        0        0     1709 2023-06-16 02:46:15.374136 wom_py-0.4.2/wom/services/__init__.py
+-rw-r--r--   0        0        0     2050 2023-06-16 02:46:15.374136 wom_py-0.4.2/wom/services/base.py
+-rw-r--r--   0        0        0    21170 2023-06-16 02:46:15.374136 wom_py-0.4.2/wom/services/competitions.py
+-rw-r--r--   0        0        0     3528 2023-06-16 02:46:15.374136 wom_py-0.4.2/wom/services/deltas.py
+-rw-r--r--   0        0        0     3688 2023-06-16 02:46:15.374136 wom_py-0.4.2/wom/services/efficiency.py
+-rw-r--r--   0        0        0    24099 2023-06-16 02:46:15.374136 wom_py-0.4.2/wom/services/groups.py
+-rw-r--r--   0        0        0     5772 2023-06-16 02:46:15.374136 wom_py-0.4.2/wom/services/http.py
+-rw-r--r--   0        0        0     4031 2023-06-16 02:46:15.374136 wom_py-0.4.2/wom/services/names.py
+-rw-r--r--   0        0        0    18088 2023-06-16 02:46:15.374136 wom_py-0.4.2/wom/services/players.py
+-rw-r--r--   0        0        0     3506 2023-06-16 02:46:15.374136 wom_py-0.4.2/wom/services/records.py
+-rw-r--r--   0        0        0     3828 1970-01-01 00:00:00.000000 wom_py-0.4.2/PKG-INFO
```

### Comparing `wom_py-0.4.1/LICENSE` & `wom_py-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/README.md` & `wom_py-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/pyproject.toml` & `wom_py-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wom.py"
-version = "0.4.1"
+version = "0.4.2"
 description = "An asynchronous wrapper for the Wise Old Man API."
 authors = ["Jonxslays"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Jonxslays/wom.py"
 repository = "https://github.com/Jonxslays/wom.py"
 documentation = "https://jonxslays.github.io/wom.py"
@@ -36,20 +36,21 @@
 aiohttp = ">3.8.1"
 attrs = ">=22"
 
 [tool.poetry.group.dev.dependencies]
 black = "==23.1.0"
 coverage = "==7.1.0"
 flake8 = { version = "==6.0.0", python = ">=3.8.1" }
+griffe = ">=0.28.2"
 isort = "==5.12.0"
 len8 = { version = "==0.7.3.post0", python = "<3.12" }
 mike = "==1.1.2"
-mkdocs-include-markdown-plugin = { version = "==4.0.3", python = "<3.12" }
-mkdocs-material = "==9.0.13"
-mkdocstrings =  { version = "==0.20.0", extras = ["python"] }
+mkdocs-include-markdown-plugin = { version = "==4.0.4", python = "<3.12" }
+mkdocs-material = "==9.1.14"
+mkdocstrings = { version = "==0.21.2", extras = ["python"] }
 mypy = "==1.0.0"
 nox = "==2022.11.21"
 pyright = "==1.1.295"
 pytest = "==7.2.1"
 pytest-asyncio = "==0.20.3"
 pytest-testdox = "==3.0.1"
 types-toml = "==0.10.8.3"
```

### Comparing `wom_py-0.4.1/wom/__init__.py` & `wom_py-0.4.2/wom/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,23 +28,23 @@
 """
 
 from __future__ import annotations
 
 from typing import Final
 
 __packagename__: Final[str] = "wom.py"
-__version__: Final[str] = "0.4.1"
+__version__: Final[str] = "0.4.2"
 __author__: Final[str] = "Jonxslays"
 __copyright__: Final[str] = "2023-present Jonxslays"
 __description__: Final[str] = "An asynchronous wrapper for the Wise Old Man API."
 __url__: Final[str] = "https://github.com/Jonxslays/wom.py"
 __docs__: Final[str] = "https://jonxslays.github.io/wom.py"
 __repository__: Final[str] = __url__
 __license__: Final[str] = "MIT"
-__git_sha__: Final[str] = "[c7d71ca]"
+__git_sha__: Final[str] = "[ea0f52d]"
 
 from . import client
 from . import constants
 from . import enums
 from . import errors
 from . import models
 from . import result
```

### Comparing `wom_py-0.4.1/wom/__main__.py` & `wom_py-0.4.2/wom/__main__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/_cli.py` & `wom_py-0.4.2/wom/_cli.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/client.py` & `wom_py-0.4.2/wom/client.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/constants.py` & `wom_py-0.4.2/wom/constants.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/enums.py` & `wom_py-0.4.2/wom/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,21 @@
 
         Args:
             value: The value to generate from.
 
         Returns:
             The generated enum.
         """
-        return cls(value)
+        try:
+            return cls(value)
+        except ValueError as e:
+            raise ValueError(
+                f"{e} variant. Please report this issue on github at "
+                "https://github.com/Jonxslays/wom.py/issues/new"
+            ) from None
 
     @classmethod
     def from_str_maybe(cls: t.Type[T], value: str) -> t.Optional[T]:
         """Attempt to generate this enum from the given value.
 
         Args:
             value: The value to generate from.
@@ -83,30 +89,33 @@
         [`Bosses`][wom.Bosses], [`ComputedMetrics`][wom.ComputedMetrics],
         or [`Skills`][wom.Skills].
     """
 
     @classmethod
     def from_str(cls: t.Type[T], value: str) -> T:
         if cls is not Metric:
-            return cls(value)
+            return super().from_str(value)
 
         children = {Skills, Activities, Bosses, ComputedMetrics}
 
         for child in children:
             try:
                 return child(value)  # type: ignore
             except ValueError:
                 continue
 
-        raise RuntimeError(f"No {cls} variant for {value!r}.")
+        raise ValueError(
+            f"{value!r} is not a valid {cls.__name__} variant. "
+            "Please report this issue on github at https://github.com/Jonxslays/wom.py/issues/new"
+        )
 
     @classmethod
     def from_str_maybe(cls: t.Type[T], value: str) -> t.Optional[T]:
         if cls is not Metric:
-            return super(Metric, cls).from_str_maybe(value)  # pyright: ignore
+            return super().from_str_maybe(value)  # pyright: ignore
 
         children = {Skills, Activities, Bosses, ComputedMetrics}
 
         for child in children:
             try:
                 return child(value)  # type: ignore
             except ValueError:
```

### Comparing `wom_py-0.4.1/wom/errors.py` & `wom_py-0.4.2/wom/errors.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/models/__init__.py` & `wom_py-0.4.2/wom/models/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/models/base.py` & `wom_py-0.4.2/wom/models/base.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/models/competitions/__init__.py` & `wom_py-0.4.2/wom/models/competitions/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/models/competitions/enums.py` & `wom_py-0.4.2/wom/models/competitions/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/models/competitions/models.py` & `wom_py-0.4.2/wom/models/competitions/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/models/deltas/__init__.py` & `wom_py-0.4.2/wom/models/deltas/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/models/deltas/models.py` & `wom_py-0.4.2/wom/models/deltas/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/models/groups/__init__.py` & `wom_py-0.4.2/wom/models/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/models/groups/enums.py` & `wom_py-0.4.2/wom/models/groups/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/models/groups/models.py` & `wom_py-0.4.2/wom/models/groups/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/models/http.py` & `wom_py-0.4.2/wom/models/http.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/models/names/__init__.py` & `wom_py-0.4.2/wom/models/names/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/models/names/enums.py` & `wom_py-0.4.2/wom/models/names/enums.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/models/names/models.py` & `wom_py-0.4.2/wom/models/names/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         NameChangeReviewReason.NewNameNotFound,
         NameChangeReviewReason.NegativeGains,
     ]
     """The reason this name change was denied."""
 
     negative_gains: t.Optional[t.Dict[enums.Metric, int]]
     """The negative gains that were observed, if there were any. Only populated
-    when the reason is [`NegativeGains`][wom.NameChangeReviewReason].
+    when the reason is `NegativeGains`.
     """
 
 
 @attrs.define(init=False)
 class SkippedNameChangeReviewContext(NameChangeReviewContext):  # type: ignore[override]
     """The review context for a name change that was skipped."""
 
@@ -87,41 +87,40 @@
         NameChangeReviewReason.ExcessiveGains,
         NameChangeReviewReason.TotalLevelTooLow,
     ]
     """The reason this name change was denied."""
 
     max_hours_diff: t.Optional[int]
     """The max number of hours in the transition period. Only populated when
-    reason is [`TransitionTooLong`][wom.NameChangeReviewReason].
+    reason is `TransitionTooLong`.
     """
 
     hours_diff: t.Optional[int]
     """The actual number of hours in the transition period. Only populated when
-    reason is [`TransitionTooLong`][wom.NameChangeReviewReason] or
-    [`ExcessiveGains`][wom.NameChangeReviewReason].
+    reason is `TransitionTooLong` or `ExcessiveGains`.
     """
 
     ehp_diff: t.Optional[int]
     """The number difference between the old and new names ehp. Only populated
-    when the reason is [`ExcessiveGains`][wom.NameChangeReviewReason].
+    when the reason is `ExcessiveGains`.
     """
 
     ehb_diff: t.Optional[int]
     """The number difference between the old and new names ehb. Only populated
-    when the reason is [`ExcessiveGains`][wom.NameChangeReviewReason].
+    when the reason is `ExcessiveGains`.
     """
 
     min_total_level: t.Optional[int]
     """The minimum total level allowed for this name change. Only populated
-    when the reason is [`TotalLevelTooLow`][wom.NameChangeReviewReason].
+    when the reason is `TotalLevelTooLow`.
     """
 
     total_level: t.Optional[int]
     """The number difference between the old and new names ehb. Only populated
-    when the reason is [`TotalLevelTooLow`][wom.NameChangeReviewReason].
+    when the reason is `TotalLevelTooLow`.
     """
 
 
 @attrs.define(init=False)
 class NameChange(BaseModel):
     """Represents a player name change."""
```

### Comparing `wom_py-0.4.1/wom/models/players/__init__.py` & `wom_py-0.4.2/wom/models/players/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/models/players/enums.py` & `wom_py-0.4.2/wom/models/players/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 class PlayerStatus(BaseEnum):
     """Status for the players account."""
 
     Active = "active"
     Unranked = "unranked"
     Flagged = "flagged"
     Archived = "archived"
+    Banned = "banned"
 
 
 class AchievementMeasure(BaseEnum):
     """Measures used to categorize achievements."""
 
     Levels = "levels"
     Experience = "experience"
```

### Comparing `wom_py-0.4.1/wom/models/players/models.py` & `wom_py-0.4.2/wom/models/players/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/models/records/__init__.py` & `wom_py-0.4.2/wom/models/records/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/models/records/models.py` & `wom_py-0.4.2/wom/models/records/models.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/result.py` & `wom_py-0.4.2/wom/result.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/routes.py` & `wom_py-0.4.2/wom/routes.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/serializer.py` & `wom_py-0.4.2/wom/serializer.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/services/__init__.py` & `wom_py-0.4.2/wom/services/__init__.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/services/base.py` & `wom_py-0.4.2/wom/services/base.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/services/competitions.py` & `wom_py-0.4.2/wom/services/competitions.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/services/deltas.py` & `wom_py-0.4.2/wom/services/deltas.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/services/efficiency.py` & `wom_py-0.4.2/wom/services/efficiency.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/services/groups.py` & `wom_py-0.4.2/wom/services/groups.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/services/http.py` & `wom_py-0.4.2/wom/services/http.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/services/names.py` & `wom_py-0.4.2/wom/services/names.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/services/players.py` & `wom_py-0.4.2/wom/services/players.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/wom/services/records.py` & `wom_py-0.4.2/wom/services/records.py`

 * *Files identical despite different names*

### Comparing `wom_py-0.4.1/PKG-INFO` & `wom_py-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wom-py
-Version: 0.4.1
+Version: 0.4.2
 Summary: An asynchronous wrapper for the Wise Old Man API.
 Home-page: https://github.com/Jonxslays/wom.py
 License: MIT
 Author: Jonxslays
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wom-py Version: 0.4.1 Summary: An asynchronous
+Metadata-Version: 2.1 Name: wom-py Version: 0.4.2 Summary: An asynchronous
 wrapper for the Wise Old Man API. Home-page: https://github.com/Jonxslays/
 wom.py License: MIT Author: Jonxslays Requires-Python: >=3.8 Classifier:
 Development Status :: 4 - Beta Classifier: Framework :: AsyncIO Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

