# Comparing `tmp/pdm-bump-0.7.0a1.tar.gz` & `tmp/pdm_bump-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-bump-0.7.0a1.tar", last modified: Mon Apr 10 20:10:45 2023, max compression
+gzip compressed data, was "pdm_bump-0.7.1.tar", last modified: Fri Jun 16 19:21:29 2023, max compression
```

## Comparing `pdm-bump-0.7.0a1.tar` & `pdm_bump-0.7.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1092 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/LICENSE
--rw-r--r--   0        0        0     2397 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/README.md
--rw-r--r--   0        0        0     3890 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/pyproject.toml
--rw-r--r--   0        0        0      770 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/__init__.py
--rw-r--r--   0        0        0      541 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/actions/__init__.py
--rw-r--r--   0        0        0     5964 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/actions/base.py
--rw-r--r--   0        0        0     1784 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/actions/explicit.py
--rw-r--r--   0        0        0     9068 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/actions/increment.py
--rw-r--r--   0        0        0     8128 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/actions/preview.py
--rw-r--r--   0        0        0     1193 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/actions/vcs.py
--rw-r--r--   0        0        0      864 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/cli.py
--rw-r--r--   0        0        0      251 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/core/__init__.py
--rw-r--r--   0        0        0     7530 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/core/config.py
--rw-r--r--   0        0        0     5755 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/core/logging.py
--rw-r--r--   0        0        0     6908 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/core/version.py
--rw-r--r--   0        0        0     4999 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/dynamic.py
--rw-r--r--   0        0        0     5347 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/plugin.py
--rw-r--r--   0        0        0        0 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/py.typed
--rw-r--r--   0        0        0     2032 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/source.py
--rw-r--r--   0        0        0      699 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/vcs/__init__.py
--rw-r--r--   0        0        0     7057 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/vcs/core.py
--rw-r--r--   0        0        0      948 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/vcs/git.py
--rw-r--r--   0        0        0     6826 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/vcs/gitcli.py
--rw-r--r--   0        0        0     3997 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/vcs/mixins.py
--rw-r--r--   0        0        0    28261 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/tests/action_test.py
--rw-r--r--   0        0        0     4317 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/tests/plugin_test.py
--rw-r--r--   0        0        0    27307 2023-04-10 20:10:12.668938 pdm-bump-0.7.0a1/tests/version_test.py
--rw-r--r--   0        0        0     2733 1970-01-01 00:00:00.000000 pdm-bump-0.7.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-06-16 19:20:42.381374 pdm_bump-0.7.1/LICENSE
+-rw-r--r--   0        0        0     2397 2023-06-16 19:20:42.381374 pdm_bump-0.7.1/README.md
+-rw-r--r--   0        0        0     6003 2023-06-16 19:21:29.162035 pdm_bump-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      869 2023-06-16 19:20:42.381374 pdm_bump-0.7.1/src/pdm_bump/__init__.py
+-rw-r--r--   0        0        0      542 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/actions/__init__.py
+-rw-r--r--   0        0        0     8508 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/actions/base.py
+-rw-r--r--   0        0        0     1954 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/actions/explicit.py
+-rw-r--r--   0        0        0     9966 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/actions/increment.py
+-rw-r--r--   0        0        0     8897 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/actions/preview.py
+-rw-r--r--   0        0        0     1558 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/actions/vcs.py
+-rw-r--r--   0        0        0     1378 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/cli.py
+-rw-r--r--   0        0        0      259 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/core/__init__.py
+-rw-r--r--   0        0        0     9465 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/core/config.py
+-rw-r--r--   0        0        0     2293 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/core/loader.py
+-rw-r--r--   0        0        0     7404 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/core/logging.py
+-rw-r--r--   0        0        0     7593 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/core/version.py
+-rw-r--r--   0        0        0     6592 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/dynamic.py
+-rw-r--r--   0        0        0     6668 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/plugin.py
+-rw-r--r--   0        0        0        0 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/py.typed
+-rw-r--r--   0        0        0     2402 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/source.py
+-rw-r--r--   0        0        0      792 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/vcs/__init__.py
+-rw-r--r--   0        0        0     9907 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/vcs/core.py
+-rw-r--r--   0        0        0     1103 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/vcs/git.py
+-rw-r--r--   0        0        0     7356 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/vcs/gitcli.py
+-rw-r--r--   0        0        0     4906 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/src/pdm_bump/vcs/mixins.py
+-rw-r--r--   0        0        0    25464 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/tests/action_test.py
+-rw-r--r--   0        0        0     3743 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/tests/plugin_test.py
+-rw-r--r--   0        0        0    24207 2023-06-16 19:20:42.385375 pdm_bump-0.7.1/tests/version_test.py
+-rw-r--r--   0        0        0     3062 1970-01-01 00:00:00.000000 pdm_bump-0.7.1/PKG-INFO
```

### Comparing `pdm-bump-0.7.0a1/LICENSE` & `pdm_bump-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-bump-0.7.0a1/README.md` & `pdm_bump-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pdm-bump-0.7.0a1/src/pdm_bump/actions/explicit.py` & `pdm_bump-0.7.1/src/pdm_bump/actions/explicit.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,27 +5,31 @@
 #
 # This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
+""""""
+
 
 from argparse import ArgumentParser
 from traceback import format_exc as get_traceback
 from typing import final
 
 from ..core.logging import logger
 from ..core.version import Version
 from .base import VersionModifier, VersionPersister, action
 
 
 @final
 @action
 class SetExplicitVersionModifier(VersionModifier):
+    """"""
+
     name: str = "to"
     description: str = "Sets a new version explicitly from CLI"
 
     def __init__(
         self,
         version: Version,
         persister: VersionPersister,
@@ -34,25 +38,37 @@
     ) -> None:
         super().__init__(version, persister, **kwargs)
         if len(new_version) != 1:
             raise ValueError("Only one value is supported")
         self.__new_version: str = new_version[0]
 
     def create_new_version(self) -> Version:
+        """"""
         try:
             new_version: Version = Version.from_string(self.__new_version)
             return new_version
         except ValueError as exc:
             err: str = f"'{self.__new_version}' is not a valid value."
             logger.exception(err, exc_info=True)
             logger.debug("Exception occurred: %s", get_traceback())
             raise ValueError(err) from exc
 
     @classmethod
     def _update_command(cls, sub_parser: ArgumentParser) -> None:
+        """
+
+        Parameters
+        ----------
+        sub_parser: ArgumentParser :
+
+
+        Returns
+        -------
+
+        """
         sub_parser.add_argument(
             "new_version",
             action="store",
             nargs=1,
             type=str,
             default=None,
             help="The next version to set.",
```

### Comparing `pdm-bump-0.7.0a1/src/pdm_bump/actions/increment.py` & `pdm_bump-0.7.1/src/pdm_bump/actions/increment.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 #
 # This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
+""""""
+
 
 import sys
 from abc import abstractmethod
 from argparse import ArgumentParser
 from dataclasses import asdict as dataclass_to_dict
 from typing import Any, Final, final
 
@@ -27,47 +29,75 @@
     from typing_extensions import TypeAlias
 
 
 _formatter = Pep440VersionFormatter()
 
 
 class _NonFinalPartsRemovingVersionModifier(VersionModifier):
+    """"""
+
     def __init__(
         self,
         version: Version,
         persister: VersionPersister,
         remove_parts: bool = True,
         **kwargs,
     ) -> None:
         super().__init__(version, persister, **kwargs)
         self.__remove_parts = remove_parts
 
     @property
     def remove_non_final_parts(self) -> bool:
+        """"""
         return self.__remove_parts
 
     @abstractmethod
     def create_new_version(self) -> Version:
+        """"""
         raise NotImplementedError()
 
     @staticmethod
     def _create_new_constructional_args(
         release: tuple[NonNegativeInteger, ...], epoch: NonNegativeInteger = 0
     ) -> dict[str, Any]:
+        """
+
+        Parameters
+        ----------
+        release: tuple[NonNegativeInteger, ...] :
+
+        epoch: NonNegativeInteger :
+             (Default value = 0)
+
+        Returns
+        -------
+
+        """
         return {
             "epoch": epoch,
             "release_tuple": release,
             "preview": None,
             "post": None,
             "dev": None,
             "local": None,
         }
 
     @classmethod
     def _update_command(cls, sub_parser: ArgumentParser) -> None:
+        """
+
+        Parameters
+        ----------
+        sub_parser: ArgumentParser :
+
+
+        Returns
+        -------
+
+        """
         sub_parser.add_argument(
             "--no-remove",
             action="store_false",
             dest="remove_parts",
             help="When incrementing major, minor, micro or epoch, "
             + "do not remove all pre-release parts.",
         )
@@ -75,21 +105,25 @@
         VersionModifier._update_command(sub_parser)
 
 
 _NFPR: TypeAlias = _NonFinalPartsRemovingVersionModifier
 
 
 class _ReleaseVersionModifier(_NonFinalPartsRemovingVersionModifier):
+    """"""
+
     @property
     @abstractmethod
     def release_part(self) -> NonNegativeInteger:
+        """"""
         raise NotImplementedError()
 
     @traced_function
     def create_new_version(self) -> Version:
+        """"""
         construction_args: dict[str, Any] = dataclass_to_dict(
             self.current_version
         )
 
         next_release: tuple[
             NonNegativeInteger, ...
         ] = self._update_release_version_part(self.release_part)
@@ -107,14 +141,25 @@
         self._report_new_version(next_version)
 
         return next_version
 
     def _update_release_version_part(
         self, part_id: NonNegativeInteger
     ) -> tuple[NonNegativeInteger, ...]:
+        """
+
+        Parameters
+        ----------
+        part_id: NonNegativeInteger :
+
+
+        Returns
+        -------
+
+        """
         release_part: list[NonNegativeInteger] = list(
             self.current_version.release
         )
 
         for i in range(len(release_part)):  # pylint: disable=C0200
             logger.debug("Checking if version part at %d must be modified", i)
             if i == part_id:
@@ -126,24 +171,27 @@
 
         return tuple(release_part)
 
 
 @final
 @action
 class FinalizingVersionModifier(_NonFinalPartsRemovingVersionModifier):
+    """"""
+
     name: str = "no-pre-release"
     description: str = "Remove all pre-release parts from the version"
 
     def __init__(
         self, version: Version, persister: VersionPersister, **kwargs
     ) -> None:
-        super().__init__(version, persister, True, **kwargs)
+        super().__init__(version, persister, **kwargs)
 
     @traced_function
     def create_new_version(self) -> Version:
+        """"""
         constructional_args: dict[
             str,
             Any
             # Using type alias due to line length enforced by black
         ] = _NFPR._create_new_constructional_args(  # noqa: E501 pylint: disable=W0212
             self.current_version.release, self.current_version.epoch
         )
@@ -153,54 +201,65 @@
 
         return next_version
 
 
 @final
 @action
 class MajorIncrementingVersionModifier(_ReleaseVersionModifier):
+    """"""
+
     name: str = "major"
     description: str = "Increment the major part of the version"
 
     __MAJOR_PART: Final[NonNegativeInteger] = 0
 
     @property
     def release_part(self) -> NonNegativeInteger:
+        """"""
         return self.__MAJOR_PART
 
 
 @final
 @action
 class MinorIncrementingVersionModifier(_ReleaseVersionModifier):
+    """"""
+
     name: str = "minor"
     description: str = "Increment the minor part of the version"
 
     __MINOR_PART: Final[NonNegativeInteger] = 1
 
     @property
     def release_part(self) -> NonNegativeInteger:
+        """"""
         return self.__MINOR_PART
 
 
 @final
 @action
 class MicroIncrementingVersionModifier(_ReleaseVersionModifier):
+    """"""
+
     name: str = "micro"
     description: str = "Increment the micro (or patch) part of the version"
     aliases: tuple[str] = ("patch",)
 
     __MICRO_PART: Final[NonNegativeInteger] = 2
 
     @property
     def release_part(self) -> int:
+        """"""
         return self.__MICRO_PART
 
 
 @final
 @action
 class EpochIncrementingVersionModifier(_NonFinalPartsRemovingVersionModifier):
+    """"""
+
     name: str = "epoch"
     description: str = "Increment the epoch of the version"
 
     def __init__(
         self,
         version: Version,
         persister: VersionPersister,
@@ -208,14 +267,15 @@
         reset_version: bool = True,
     ):
         super().__init__(version, persister, remove_parts)
         self.__reset_version = reset_version
 
     @traced_function
     def create_new_version(self) -> Version:
+        """"""
         constructional_args: dict[str, Any] = dataclass_to_dict(
             self.current_version
         )
 
         if self.__reset_version or self.remove_non_final_parts:
             constructional_args = dataclass_to_dict(Version.default())
             if not self.__reset_version:
@@ -229,33 +289,47 @@
 
         next_version: Version = Version(**constructional_args)
         self._report_new_version(next_version)
         return next_version
 
     @classmethod
     def _update_command(cls, sub_parser: ArgumentParser) -> None:
+        """
+
+        Parameters
+        ----------
+        sub_parser: ArgumentParser :
+
+
+        Returns
+        -------
+
+        """
         sub_parser.add_argument(
             "--reset",
             action="store_true",
             dest="reset_version",
             help="Reset version to 1.0.0 on epoch increment",
         )
 
         # Justification: Call protected method of parent class
         _NFPR._update_command(sub_parser)  # pylint: disable=W0212
 
 
 @final
 @action
 class DevelopmentVersionIncrementingVersionModifier(VersionModifier):
+    """"""
+
     name: str = "dev"
     description: str = "Increment the local development part"
 
     @traced_function
     def create_new_version(self) -> Version:
+        """"""
         dev_version: NonNegativeInteger = 1
         if self.current_version.dev is not None:
             _, dev_version = self.current_version.dev
             logger.debug("Incrementing development version part by one")
             dev_version = dev_version + 1
 
         constructional_args: dict[str, Any] = dataclass_to_dict(
@@ -268,19 +342,22 @@
 
         return next_version
 
 
 @final
 @action
 class PostVersionIncrementingVersionModifier(VersionModifier):
+    """"""
+
     name: str = "post"
     description: str = "Increment the post version part"
 
     @traced_function
     def create_new_version(self) -> Version:
+        """"""
         post_version: NonNegativeInteger = 1
         if self.current_version.post is not None:
             _, post_version = self.current_version.post
             logger.debug("Incrementing post version part by one")
             post_version = post_version + 1
 
         constructional_args: dict[str, Any] = dataclass_to_dict(
```

### Comparing `pdm-bump-0.7.0a1/src/pdm_bump/actions/preview.py` & `pdm_bump-0.7.1/src/pdm_bump/actions/preview.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,63 +5,95 @@
 #
 # This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
+""""""
+
 
 from abc import abstractmethod
 from argparse import ArgumentParser
 from typing import Literal, cast, final
 
 from ..core.logging import logger, traced_function
 from ..core.version import NonNegativeInteger, Pep440VersionFormatter, Version
 from .base import VersionModifier, VersionPersister, action
 
 _formatter = Pep440VersionFormatter()
 
 
 class PreviewMismatchError(Exception):
-    pass
+    """"""
+
+    # Justification: Zen of Python: Explicit is better than implicit
+    pass  # pylint: disable=W0107
 
 
 # Justification fulfills a protocol
 class _DummyPersister:  # pylint: disable=R0903
+    """"""
+
     def save_version(self, version: Version) -> None:
+        """
+
+        Parameters
+        ----------
+        version: Version :
+
+
+        Returns
+        -------
+
+        """
         # This must not be implemented as it is only a dummy.
-        pass
+        raise NotImplementedError()
 
 
 class _PreReleaseIncrementingVersionModified(VersionModifier):
+    """"""
+
     def __init__(
         self,
         version: Version,
         persister: VersionPersister,
         increment_micro: bool = True,
         **kwargs,
     ) -> None:
         super().__init__(version, persister, **kwargs)
         self.__increment_micro = increment_micro
 
     @classmethod
     def _update_command(cls, sub_parser: ArgumentParser) -> None:
+        """
+
+        Parameters
+        ----------
+        sub_parser: ArgumentParser :
+
+
+        Returns
+        -------
+
+        """
         sub_parser.add_argument(
             "--micro",
             action="store_true",
             dest="increment_micro",
             help="When setting pre-release, specifies "
             + "whether micro version shall "
             + "be incremented as well",
         )
 
         VersionModifier._update_command(sub_parser)
 
     @traced_function
     def create_new_version(self) -> Version:
+        """"""
         letter: Literal["a", "b", "c", "alpha", "beta", "rc"]
         name: str
         letter, name = self.pre_release_part
         pre: tuple[
             Literal["a", "b", "c", "alpha", "beta", "rc"], NonNegativeInteger
         ] = (letter, 1)
 
@@ -107,21 +139,24 @@
         return result
 
     @property
     @abstractmethod
     def pre_release_part(
         self,
     ) -> tuple[Literal["a", "b", "c", "alpha", "beta", "rc"], str]:
+        """"""
         raise NotImplementedError()
 
     @abstractmethod
     def _is_valid_preview_version(self) -> bool:
+        """"""
         raise NotImplementedError()
 
     def _get_next_release(self) -> tuple[NonNegativeInteger, ...]:
+        """"""
         micro = self.current_version.micro
         if self.__increment_micro and self.current_version.preview is None:
             micro = micro + 1
 
         ret: list[NonNegativeInteger] = []
         for val in self.current_version.release:
             ret.append(val)
@@ -133,14 +168,16 @@
 
         return tuple(ret)
 
 
 @final
 @action
 class PreReleaseIncrementingVersionModifier(VersionModifier):
+    """"""
+
     name: str = "pre-release"
     description: str = (
         "Increment a pre-release part (alpha, beta, release-candidate)"
     )
 
     def __init__(
         self,
@@ -172,18 +209,30 @@
         else:
             raise ValueError(
                 f"{pre_release_part} is not a valid pre-release part"
             )
 
     @traced_function
     def create_new_version(self) -> Version:
+        """"""
         return self.__sub_modifier.create_new_version()
 
     @classmethod
     def _update_command(cls, sub_parser: ArgumentParser) -> None:
+        """
+
+        Parameters
+        ----------
+        sub_parser: ArgumentParser :
+
+
+        Returns
+        -------
+
+        """
         valid_values = []
         valid_values.append(AlphaIncrementingVersionModifier.name)
         valid_values.append(BetaIncrementingVersionModifier.name)
         valid_values.append(ReleaseCandidateIncrementingVersionModifier.name)
         valid_values.extend(
             ReleaseCandidateIncrementingVersionModifier.aliases
         )
@@ -206,57 +255,69 @@
         # Justification: Class is a mixin
         # pylint: disable=W0212
         _PreReleaseIncrementingVersionModified._update_command(sub_parser)
 
 
 @final
 class AlphaIncrementingVersionModifier(_PreReleaseIncrementingVersionModified):
+    """"""
+
     name: str = "alpha"
     description: str = "Increment the alpha pre-release version part"
 
     @property
     def pre_release_part(
         self,
     ) -> tuple[Literal["a", "b", "c", "alpha", "beta", "rc"], str]:
+        """"""
         return ("a", "alpha")
 
     def _is_valid_preview_version(self) -> bool:
+        """"""
         return self.current_version.is_alpha
 
 
 @final
 class BetaIncrementingVersionModifier(_PreReleaseIncrementingVersionModified):
+    """"""
+
     name: str = "beta"
     description: str = "Increment the beta pre-release version part"
 
     @property
     def pre_release_part(
         self,
     ) -> tuple[Literal["a", "b", "c", "alpha", "beta", "rc"], str]:
+        """"""
         return ("b", "alpha or beta")
 
     def _is_valid_preview_version(self) -> bool:
+        """"""
         return self.current_version.is_alpha or self.current_version.is_beta
 
 
 @final
 class ReleaseCandidateIncrementingVersionModifier(
     _PreReleaseIncrementingVersionModified
 ):
+    """"""
+
     name: str = "rc"
     description: str = (
         "Increment the release-candidate pre-release version part"
     )
     aliases: tuple[str] = ("c",)
 
     @property
     def pre_release_part(
         self,
     ) -> tuple[Literal["a", "b", "c", "alpha", "beta", "rc"], str]:
+        """"""
         return ("rc", "pre-release")
 
     def _is_valid_preview_version(self) -> bool:
+        """"""
         return (
             self.current_version.is_alpha
             or self.current_version.is_beta
             or self.current_version.is_release_candidate
         )
```

### Comparing `pdm-bump-0.7.0a1/src/pdm_bump/actions/vcs.py` & `pdm_bump-0.7.1/src/pdm_bump/actions/vcs.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,36 +5,58 @@
 #
 # This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
+""""""
+
 
 from typing import final
 
 from ..core.logging import logger
 from ..core.version import Pep440VersionFormatter, Version
 from ..vcs import VcsProvider, VcsProviderAggregator
 from .base import VersionConsumer, action
 
 
 @final
 @action
 class CreateTagFromVersion(VersionConsumer, VcsProviderAggregator):
+    """"""
+
     name: str = "tag"
     description: str = "Create a VCS revision tag from the current version"
 
     def __init__(
         self, version: Version, vcs_provider: VcsProvider, **kwargs
     ) -> None:
         VersionConsumer.__init__(self, version, **kwargs)
         VcsProviderAggregator.__init__(self, vcs_provider, **kwargs)
 
     def run(self, dry_run: bool = False) -> None:
+        """
+
+        Parameters
+        ----------
+        dry_run: bool :
+             (Default value = False)
+
+        Returns
+        -------
+
+        """
         if not dry_run:
             self.vcs_provider.create_tag_from_version(self.current_version)
         else:
             logger.info(
                 "Would create tag v%s",
                 Pep440VersionFormatter().format(self.current_version),
             )
+
+    @classmethod
+    def get_allowed_arguments(cls) -> set[str]:
+        """"""
+        return set(["vcs_provider"]).union(
+            VersionConsumer.get_allowed_arguments()
+        )
```

### Comparing `pdm-bump-0.7.0a1/src/pdm_bump/core/config.py` & `pdm_bump-0.7.1/src/pdm_bump/core/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 #
 # This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
+""""""
+
+
 import sys
 from collections.abc import Iterable
 from enum import Enum, IntEnum, auto
 from functools import cached_property
 from io import BytesIO
 from pathlib import Path
 from typing import Any, Final, Optional, Protocol, cast
@@ -36,32 +39,53 @@
     from tomli import load as load_toml  # type: ignore
 
 
 _ConfigMapping: TypeAlias = dict[str, Any]
 
 
 class _StringEnum(str, Enum):
-    pass
+    """"""
+
+    # Justification: Zen of python: Explicit is better than implicit
+    pass  # pylint: disable=W0107
 
 
 # Justification: Minimal protocol
 class ConfigHolder(Protocol):  # pylint: disable=R0903
+    """"""
+
     root: Path
     PYPROJECT_FILENAME: str
 
     @property
     def config(self) -> _ConfigMapping:
+        """"""
         # Method empty: Only a protocol stub
-        pass
+        raise NotImplementedError()
 
 
 @traced_function
 def _get_config_value(
     config: _ConfigMapping, *keys: str, default_value: Optional[Any] = None
 ) -> Optional[Any]:
+    """
+
+    Parameters
+    ----------
+    config: _ConfigMapping :
+
+    *keys: str :
+
+    default_value: Optional[Any] :
+         (Default value = None)
+
+    Returns
+    -------
+
+    """
     front: str
 
     key: str = ".".join(keys)
     logger.debug("Searching for '%s' in configuration", key)
     logger.debug("Configuration is set to: \n%s", config)
 
     while len(keys) > 1:
@@ -79,14 +103,29 @@
     result = default_value if front not in config.keys() else config[front]
     logger.debug("Found value at '%s' is: %s", key, result)
     return result
 
 
 @traced_function
 def _set_config_value(config: _ConfigMapping, value: Any, *keys: str) -> None:
+    """
+
+    Parameters
+    ----------
+    config: _ConfigMapping :
+
+    value: Any :
+
+    *keys: str :
+
+
+    Returns
+    -------
+
+    """
     front: str
 
     key: str = ".".join(keys)
     logger.debug("Setting '%s' to '%s'", key, value)
 
     while len(keys) > 1:
         front = keys[0]
@@ -99,127 +138,242 @@
         keys = tuple(keys[1:])
 
     front = keys[0]
     config[front] = value
 
 
 class ConfigSections(_StringEnum):
+    """"""
+
     PDM_BUMP: Final[str] = "pdm_bump"
     PDM_BUMP_VCS: Final[str] = "vcs"
 
 
 class ConfigKeys(_StringEnum):
+    """"""
+
     VERSION: Final[str] = "version"
     VERSION_SOURCE: Final[str] = "source"
     VERSION_SOURCE_FILE_PATH: Final[str] = "path"
     BUILD_BACKEND: Final[str] = "build-backend"
     VCS_PROVIDER: Final[str] = "provider"
     PROJECT_METADATA: Final[str] = "project"
 
 
 class ConfigValues(_StringEnum):
+    """"""
+
     VERSION_SOURCE_FILE: Final[str] = "file"
-    BUILD_BACKEND_PDM_PEP517_API: Final[str] = "pdm.pep517.api"
+    VERSION_SOURCE_SCM: Final[str] = "scm"
+    DEPREACTED_BUILD_BACKEND_PDM_PEP517_API: Final[str] = "pdm.pep517.api"
+    BUILD_BACKEND_PDM_BACKEND: Final[str] = "pdm.backend"
 
 
 # Justification: Currently no more meta data to check
 class ProjectMetaData:  # pylint: disable=R0903
+    """"""
+
     def __init__(self, meta_data: StandardMetadata) -> None:
         self.__meta_data = meta_data
 
     @property
     def is_dynamic_version(self) -> bool:
+        """"""
         return ConfigKeys.VERSION in self.__meta_data.dynamic
 
 
 class _ConfigSection(IntEnum):
+    """"""
+
     ROOT = auto()
     METADATA = auto()
     PLUGIN_CONFIG = auto()
     BUILD_SYSTEM = auto()
     TOOL_CONFIG = auto()
 
 
 class Config:
+    """"""
+
     def __init__(self, project: ConfigHolder) -> None:
         self.__project: ConfigHolder = project
 
     @cached_property
     @traced_function
     def pyproject_file(self) -> Path:
+        """"""
         return self.__project.root / self.__project.PYPROJECT_FILENAME
 
     @property
     @traced_function
     def meta_data(self) -> ProjectMetaData:
+        """"""
         data: _ConfigMapping = self._get_pyproject_config(_ConfigSection.ROOT)
         meta: StandardMetadata = StandardMetadata.from_pyproject(data)
         return ProjectMetaData(meta)
 
     @traced_function
-    def get_pyproject_metadata(self, *keys: str) -> Optional[Any]:
+    def get_pyproject_metadata(self, *keys: tuple[str, ...]) -> Optional[Any]:
+        """
+
+        Parameters
+        ----------
+        *keys: tuple[str, ...] :
+
+
+        Returns
+        -------
+
+        """
         config: _ConfigMapping = self._get_pyproject_config(
             _ConfigSection.METADATA
         )
         return _get_config_value(config, *keys)
 
     @traced_function
-    def get_pyproject_build_system(self, *keys: str) -> Optional[Any]:
+    def get_pyproject_build_system(
+        self, *keys: tuple[str, ...]
+    ) -> Optional[Any]:
+        """
+
+        Parameters
+        ----------
+        *keys: tuple[str, ...] :
+
+
+        Returns
+        -------
+
+        """
         config: _ConfigMapping = self._get_pyproject_config(
             _ConfigSection.BUILD_SYSTEM
         )
         return _get_config_value(config, *keys)
 
     @traced_function
-    def get_pyproject_tool_config(self, *keys: str) -> Optional[Any]:
+    def get_pyproject_tool_config(
+        self, *keys: tuple[str, ...]
+    ) -> Optional[Any]:
+        """
+
+        Parameters
+        ----------
+        *keys: tuple[str, ...] :
+
+
+        Returns
+        -------
+
+        """
         config: _ConfigMapping = self._get_pyproject_config(
             _ConfigSection.TOOL_CONFIG
         )
         return _get_config_value(config, *keys)
 
     @traced_function
-    def get_config_value(self, *keys: str) -> Optional[Any]:
+    def get_config_value(self, *keys: tuple[str, ...]) -> Optional[Any]:
+        """
+
+        Parameters
+        ----------
+        *keys: tuple[str, ...] :
+
+
+        Returns
+        -------
+
+        """
         config: dict[str, Any] = self.__project.config
         return _get_config_value(config, *keys)
 
     @traced_function
-    def get_config_or_pyproject_value(self, *keys: str) -> Optional[Any]:
+    def get_config_or_pyproject_value(
+        self, *keys: tuple[str, ...]
+    ) -> Optional[Any]:
+        """
+
+        Parameters
+        ----------
+        *keys: tuple[str, ...] :
+
+
+        Returns
+        -------
+
+        """
         config1: _ConfigMapping = self.__project.config
         config2: _ConfigMapping = self._get_pyproject_config(
             _ConfigSection.PLUGIN_CONFIG
         )
 
         return _get_config_value(config1, *keys) or _get_config_value(
             config2, *keys
         )
 
     @traced_function
-    def set_pyproject_metadata(self, value: Any, *keys: str) -> None:
+    def set_pyproject_metadata(
+        self, value: Any, *keys: tuple[str, ...]
+    ) -> None:
+        """
+
+        Parameters
+        ----------
+        value: Any :
+
+        *keys: tuple[str, ...] :
+
+
+        Returns
+        -------
+
+        """
         config: _ConfigMapping = self._get_pyproject_config(
             _ConfigSection.ROOT
         )
         new_config: _ConfigMapping = _get_config_value(
             config, ConfigKeys.PROJECT_METADATA, default_value={}
         )
         _set_config_value(new_config, value, *keys)
         self._write_config(config)
 
     def _write_config(self, config: _ConfigMapping) -> None:
+        """
+
+        Parameters
+        ----------
+        config: _ConfigMapping :
+
+
+        Returns
+        -------
+
+        """
         with BytesIO() as buffer:
             dump_toml(config, buffer)
 
             with open(self.pyproject_file, "wb+") as file_ptr:
                 file_ptr.write(buffer.getvalue())
                 logger.info(
                     "Successfully saved configuration to %s",
                     self.pyproject_file,
                 )
 
     @traced_function
     def _get_pyproject_config(self, section: _ConfigSection) -> _ConfigMapping:
+        """
+
+        Parameters
+        ----------
+        section: _ConfigSection :
+
+
+        Returns
+        -------
+
+        """
         project_data: _ConfigMapping = self._read_config()
         section_key: Iterable[str] = ()
         if section in (
             _ConfigSection.TOOL_CONFIG,
             _ConfigSection.PLUGIN_CONFIG,
         ):
             section_key = ["tool", "pdm"]
@@ -235,10 +389,11 @@
 
         data = _get_config_value(project_data, *section_key, default_value={})
 
         return cast(_ConfigMapping, data)
 
     @traced_function
     def _read_config(self) -> dict[str, Any]:
+        """"""
         project_file = self.pyproject_file
         with open(project_file, "rb") as file_pointer:
             return load_toml(file_pointer)
```

### Comparing `pdm-bump-0.7.0a1/src/pdm_bump/core/version.py` & `pdm_bump-0.7.1/src/pdm_bump/core/version.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 #
 # This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
+""""""
+
 
 # Implementation of the PEP 440 version.
 from dataclasses import dataclass, field
 from functools import total_ordering
 from typing import Annotated, Any, Final, Literal, Optional, cast, final
 
 from annotated_types import Ge
@@ -20,26 +22,31 @@
 from packaging.version import Version as BaseVersion
 
 from .logging import traced_function
 
 
 @final
 class VersionParserError(ValueError):
-    pass
+    """"""
+
+    # Justification: Zen of python: Explicit is better than implicit
+    pass  # pylint: disable=W0107
 
 
 NonNegative = Ge(0)
 
 NonNegativeInteger = Annotated[int, NonNegative]
 
 
 @final
 @dataclass(eq=False, order=False, frozen=True)
 @total_ordering
 class Version:
+    """"""
+
     epoch: NonNegativeInteger = field(
         default=0, repr=True, hash=True, compare=True
     )
     release_tuple: tuple[NonNegativeInteger, ...] = field(default=(1, 0, 0))
     preview: Optional[
         tuple[
             Literal["a", "b", "c", "alpha", "beta", "rc"], NonNegativeInteger
@@ -60,62 +67,73 @@
             if self.preview[0] not in ["a", "b", "c", "alpha", "beta", "rc"]:
                 raise ValueError(
                     f"Invalid pre-release identifier {self.preview[0]}"
                 )
 
     @property
     def major(self) -> NonNegativeInteger:
+        """"""
         return self.release_tuple[0] if len(self.release_tuple) >= 1 else 0
 
     @property
     def minor(self) -> NonNegativeInteger:
+        """"""
         return self.release_tuple[1] if len(self.release_tuple) >= 2 else 0
 
     @property
     def micro(self) -> NonNegativeInteger:
+        """"""
         return self.release_tuple[2] if len(self.release_tuple) >= 3 else 0
 
     @property
     def release(
         self,
     ) -> tuple[NonNegativeInteger, NonNegativeInteger, NonNegativeInteger]:
+        """"""
         return (
             self.major,
             self.minor,
             self.micro,
         )
 
     @property
     def is_pre_release(self) -> bool:
+        """"""
         return self.preview is not None or self.is_development_version
 
     @property
     def is_development_version(self) -> bool:
+        """"""
         return self.dev is not None
 
     @property
     def is_post_release(self) -> bool:
+        """"""
         return self.post is not None
 
     @property
     def is_local_version(self) -> bool:
+        """"""
         return self.local is not None
 
     @property
     def is_alpha(self) -> bool:
+        """"""
         alpha_part: Final[tuple[str, ...]] = ("a", "alpha")
         return self.preview is not None and self.__compare_preview(alpha_part)
 
     @property
     def is_beta(self) -> bool:
+        """"""
         beta_part: Final[tuple[str, ...]] = ("b", "beta")
         return self.preview is not None and self.__compare_preview(beta_part)
 
     @property
     def is_release_candidate(self) -> bool:
+        """"""
         rc_part: Final[tuple[str, ...]] = ("c", "rc")
         return self.preview is not None and self.__compare_preview(rc_part)
 
     def __compare_preview(self, valid_parts: tuple[str, ...]) -> bool:
         if self.preview is not None:
             pre: tuple[str, int] = cast(tuple[str, int], self.preview)
             return pre[0] in valid_parts
@@ -157,18 +175,30 @@
         return my_data < other_data
 
     def __str__(self) -> str:
         return Pep440VersionFormatter().format(self)
 
     @staticmethod
     def default() -> "Version":
+        """"""
         return Version(0, (1,), None, None, None, None)
 
     @staticmethod
     def from_string(version: str) -> "Version":
+        """
+
+        Parameters
+        ----------
+        version: str :
+
+
+        Returns
+        -------
+
+        """
         try:
             _version: BaseVersion = BaseVersion(version)
 
             return Version(
                 _version.epoch,
                 _version.release,
                 cast(
@@ -186,26 +216,50 @@
         except InvalidVersion as error:
             raise VersionParserError(
                 f"{version} is not a valid version according to PEP 440."
             ) from error
 
     @staticmethod
     def can_parse_to_version(version: str) -> bool:
+        """
+
+        Parameters
+        ----------
+        version: str :
+
+
+        Returns
+        -------
+
+        """
         try:
             _ = Version.from_string(version)
             return True
         except VersionParserError:
             return False
 
 
 @final
 # Justification: Only method to provide
 class Pep440VersionFormatter:  # pylint: disable=R0903
+    """"""
+
     @traced_function
     def format(self, version: Version) -> str:
+        """
+
+        Parameters
+        ----------
+        version: Version :
+
+
+        Returns
+        -------
+
+        """
         parts: list[str] = []
 
         if version.epoch > 0:
             parts.append(f"{version.epoch}!")
 
         parts.append(".".join(str(part) for part in version.release))
```

### Comparing `pdm-bump-0.7.0a1/src/pdm_bump/dynamic.py` & `pdm_bump-0.7.1/src/pdm_bump/dynamic.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,59 +5,79 @@
 #
 # This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
+""""""
+
+
 from functools import cached_property
 from pathlib import Path
 from re import M as MultilinePattern  # noqa: N811
 from re import Match, Pattern
 from re import compile as compile_re
 from typing import Final, Optional, cast
 
 from .core.config import Config, ConfigKeys, ConfigValues
+from .core.logging import logger
 from .core.version import Pep440VersionFormatter, Version
 
 DEFAULT_REGEX: Final[Pattern[str]] = compile_re(
     r"^__version__\s*=\s*[\"'](?P<version>.+?)[\"']\s*(?:#.*)?$",
     MultilinePattern,
 )
 
 
 class DynamicVersionConfig:
+    """"""
+
     __file: Path
     __pattern: Pattern[str]
     __file_encoding: str
 
     def __init__(
         self, file_path: Path, pattern: Pattern[str], encoding: str = "utf-8"
     ) -> None:
         self.__file = file_path
         self.__pattern = pattern
         self.__file_encoding = encoding
 
     @property
     def file(self) -> Path:
+        """"""
         return self.__file
 
     @property
     def pattern(self) -> Pattern[str]:
+        """"""
         return self.__pattern
 
     @cached_property
     def dynamic_version(self) -> Optional[str]:
+        """"""
         with self.__file.open("r", encoding=self.__file_encoding) as file_ptr:
             match = self.__pattern.search(file_ptr.read())
         if match is not None:
             return match.group(ConfigKeys.VERSION)
         return None
 
     def replace_dynamic_version(self, new_version: str) -> None:
+        """
+
+        Parameters
+        ----------
+        new_version: str :
+
+
+        Returns
+        -------
+
+        """
         with self.__file.open("r", encoding=self.__file_encoding) as file_ptr:
             version_file = file_ptr.read()
             match = self.__pattern.search(version_file)
             if match is None:
                 raise ValueError("Failed to fetch version")
             match = cast(Match[str], match)
             version_start, version_end = match.span(ConfigKeys.VERSION)
@@ -69,41 +89,86 @@
         with self.__file.open("w", encoding=self.__file_encoding) as file_ptr:
             file_ptr.write(new_version_file)
 
     @staticmethod
     def find_dynamic_config(
         root_path: Path, project_config: Config
     ) -> Optional["DynamicVersionConfig"]:
+        """
+
+        Parameters
+        ----------
+        root_path: Path :
+
+        project_config: Config :
+
+
+        Returns
+        -------
+
+        """
         if (
             project_config.get_pyproject_build_system(ConfigKeys.BUILD_BACKEND)
-            == ConfigValues.BUILD_BACKEND_PDM_PEP517_API
+            == ConfigValues.DEPREACTED_BUILD_BACKEND_PDM_PEP517_API
             and project_config.get_pyproject_tool_config(
                 ConfigKeys.VERSION, ConfigKeys.VERSION_SOURCE
             )
             == ConfigValues.VERSION_SOURCE_FILE
         ):
+            logger.warning(
+                "Build backend pdm-pep517 is deprecated. Consider upgrading."
+            )
             file_path = project_config.get_pyproject_tool_config(
                 ConfigKeys.VERSION, ConfigKeys.VERSION_SOURCE_FILE_PATH
             )
             return DynamicVersionConfig(
                 file_path=root_path / file_path,
                 pattern=DEFAULT_REGEX,
             )
+        if (
+            project_config.get_pyproject_metadata(ConfigKeys.BUILD_BACKEND)
+            == ConfigValues.BUILD_BACKEND_PDM_BACKEND
+        ):
+            if (
+                project_config.get_pyproject_tool_config(
+                    ConfigKeys.VERSION, ConfigKeys.VERSION_SOURCE
+                )
+                == ConfigValues.VERSION_SOURCE_SCM
+            ):
+                logger.error(
+                    "PDM bump cannot be used if version is fetched from scm"
+                )
+            if (
+                project_config.get_pyproject_tool_config(
+                    ConfigKeys.VERSION, ConfigKeys.VERSION_SOURCE
+                )
+                == ConfigValues.VERSION_SOURCE_FILE
+            ):
+                file_path = project_config.get_pyproject_tool_config(
+                    ConfigKeys.VERSION, ConfigKeys.VERSION_SOURCE_FILE_PATH
+                )
+                return DynamicVersionConfig(
+                    file_path=root_path / file_path,
+                    pattern=DEFAULT_REGEX,
+                )
         return None
 
 
 # Justification: Implementation of minimal protocol
 class DynamicVersionSource:  # pylint: disable=R0903
+    """"""
+
     def __init__(self, project_root: Path, config: Config) -> None:
         self.__project_root = project_root
         self.__config = config
         self.__current_version: Optional[Version] = None
 
     @property
     def is_enabled(self) -> bool:
+        """"""
         return self.__config.meta_data.is_dynamic_version
 
     def __get_current_version(self) -> Version:
         if self.__current_version is not None:
             return cast(Version, self.__current_version)
 
         dynamic: DynamicVersionConfig = self.__get_dynamic_version()
```

### Comparing `pdm-bump-0.7.0a1/src/pdm_bump/plugin.py` & `pdm_bump-0.7.1/src/pdm_bump/plugin.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,27 +5,31 @@
 #
 # This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
+""""""
+
+
 from argparse import ArgumentParser, Namespace
 from pathlib import Path
 from traceback import format_exc as get_traceback
 from typing import Final, Optional, Protocol, cast, final
 
 # MyPy does not recognize this during pull requests
 from pdm.cli.commands.base import BaseCommand  # type: ignore
 from pdm.termui import UI  # type: ignore
 
 from .actions import actions
 from .core.config import Config, ConfigHolder, ConfigKeys, ConfigSections
 from .core.logging import (
     logger,
+    setup_logger,
     traced_function,
     update_logger_from_project_ui,
 )
 from .core.version import Pep440VersionFormatter, Version
 from .dynamic import DynamicVersionSource
 from .source import StaticPep621VersionSource
 from .vcs import (
@@ -34,32 +38,50 @@
     VcsProviderRegistry,
     vcs_providers,
 )
 
 
 # Justification: Protocol for interoperability
 class _CoreLike(Protocol):  # pylint: disable=R0903
+    """"""
+
     ui: UI
 
 
 class _ProjectLike(ConfigHolder, Protocol):
+    """"""
+
     root: Path
     core: _CoreLike
     PYPROJECT_FILENAME: str
 
     def write_pyproject(self, show_message: bool) -> None:
+        """
+
+        Parameters
+        ----------
+        show_message: bool :
+
+
+        Returns
+        -------
+
+        """
         # Method empty: Only a protocol stub
-        pass
+        raise NotImplementedError()
 
 
 # Justification: Minimal protocol. Maybe false positive,
 # since 2 public methods available
 class _VersionSource(Protocol):  # pylint: disable=R0903
+    """"""
+
     @property
     def is_enabled(self) -> bool:
+        """"""
         raise NotImplementedError()
 
     def __get_current_version(self) -> Version:
         raise NotImplementedError()
 
     def __set_current_version(self, version: Version) -> None:
         raise NotImplementedError()
@@ -67,41 +89,83 @@
     current_version: property = property(
         __get_current_version, __set_current_version
     )
 
 
 @final
 class BumpCommand(BaseCommand):
+    """"""
+
     name: Final[str] = "bump"
     description: str = "Bumps the version to a next version following PEP440."
 
-    def __init__(self, parser) -> None:
-        super().__init__(parser)
+    def __init__(self) -> None:
+        super().__init__()
         self.__backend: Optional[_VersionSource] = None
 
     @traced_function
     def add_arguments(self, parser: ArgumentParser) -> None:
+        """
+
+        Parameters
+        ----------
+        parser: ArgumentParser :
+
+
+        Returns
+        -------
+
+        """
         actions.update_parser(parser)
 
     @traced_function
     def save_version(self, version: Version) -> None:
+        """
+
+        Parameters
+        ----------
+        version: Version :
+
+
+        Returns
+        -------
+
+        """
         if self.__backend is None:
             msg = ". ".join(
                 (
                     "No source for a version could be determined.",
                     "Saving version failed.",
                 )
             )
             logger.error(msg)
             return
 
         self.__backend.current_version = version
 
     @traced_function
     def handle(self, project: _ProjectLike, options: Namespace) -> None:
+        """
+
+        Parameters
+        ----------
+        project: _ProjectLike :
+
+        options: Namespace :
+
+
+        Returns
+        -------
+
+        """
+        # This will not handling tracing or related parts
+        # Should be evaluated at start-up time
+        if hasattr(options, "verbose"):
+            setup_logger(options.verbose)
+
         config: Config = Config(project)
         update_logger_from_project_ui(project.core.ui)
 
         selected_backend: Optional[_VersionSource] = self._select_backend(
             project, config
         )
 
@@ -113,23 +177,37 @@
             return
 
         backend: _VersionSource = cast(_VersionSource, selected_backend)
         vcs_provider: VcsProvider = self._get_vcs_provider(project)
 
         try:
             actions.execute(
-                options, backend.current_version, self, vcs_provider
+                options,
+                version=backend.current_version,
+                persister=self,
+                vcs_provider=vcs_provider,
             )
         except ValueError as exc:
             logger.exception("Failed to execute action", exc_info=True)
             logger.debug("Exception occurred: %s", get_traceback())
             raise SystemExit(1) from exc
 
     @traced_function
     def _get_vcs_provider(self, project: _ProjectLike) -> VcsProvider:
+        """
+
+        Parameters
+        ----------
+        project: _ProjectLike :
+
+
+        Returns
+        -------
+
+        """
         config: Config = Config(project)
         value = config.get_config_or_pyproject_value(
             ConfigSections.PDM_BUMP,
             ConfigSections.PDM_BUMP_VCS,
             ConfigKeys.VCS_PROVIDER,
         )
 
@@ -148,14 +226,27 @@
 
         return DefaultVcsProvider(project.root)
 
     @traced_function
     def _select_backend(
         self, project: _ProjectLike, config: Config
     ) -> Optional[_VersionSource]:
+        """
+
+        Parameters
+        ----------
+        project: _ProjectLike :
+
+        config: Config :
+
+
+        Returns
+        -------
+
+        """
         static_backend: _VersionSource = StaticPep621VersionSource(
             project, config
         )
         dynamic_backend: _VersionSource = DynamicVersionSource(
             project.root, config
         )
 
@@ -165,9 +256,20 @@
                 selected_backend = backend
                 break
 
         return selected_backend
 
     @traced_function
     def _version_to_string(self, version: Version) -> str:
+        """
+
+        Parameters
+        ----------
+        version: Version :
+
+
+        Returns
+        -------
+
+        """
         result: str = Pep440VersionFormatter().format(version)
         return result
```

### Comparing `pdm-bump-0.7.0a1/src/pdm_bump/vcs/git.py` & `pdm_bump-0.7.1/src/pdm_bump/vcs/git.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,30 +5,47 @@
 #
 # This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
+""""""
+
+
 from abc import abstractmethod
 from collections.abc import Iterator
 from pathlib import Path
 
 from .core import VcsFileSystemIdentifier, VcsProvider, VcsProviderFactory
 
 
 class GitCommonVcsProviderFactory(VcsProviderFactory):
+    """"""
+
     __git_dir_provider = VcsFileSystemIdentifier(
         file_name=None, dir_name=".git"
     )
     __git_wt_file_provider = VcsFileSystemIdentifier(
         file_name=".git", dir_name=None
     )
 
     @abstractmethod
     def _create_provider(self, path: Path) -> VcsProvider:
+        """
+
+        Parameters
+        ----------
+        path: Path :
+
+
+        Returns
+        -------
+
+        """
         raise NotImplementedError()
 
     @property
     def vcs_fs_root(self) -> Iterator[VcsFileSystemIdentifier]:
+        """"""
         yield self.__git_dir_provider
         yield self.__git_wt_file_provider
```

### Comparing `pdm-bump-0.7.0a1/src/pdm_bump/vcs/gitcli.py` & `pdm_bump-0.7.1/src/pdm_bump/vcs/gitcli.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,54 +5,62 @@
 #
 # This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
+""""""
+
+
 from functools import cached_property
 from pathlib import Path
 from subprocess import CalledProcessError
 from typing import Optional, cast
 
 from ..core.logging import logger
 from ..core.version import Version
 from .core import VcsProvider, VcsProviderError, vcs_provider
 from .git import GitCommonVcsProviderFactory
 from .mixins import CliRunnerMixin
 
 
 class GitCliVcsProvider(VcsProvider, CliRunnerMixin):
+    """"""
+
     __GIT_EXECUTABLE_NAME = "git"
 
     @cached_property
     def git_executable_path(self) -> Path:
+        """"""
         logger.debug("Searching for %s executable", self.__GIT_EXECUTABLE_NAME)
         git_executable_path: Optional[Path] = self._which(
             self.__GIT_EXECUTABLE_NAME
         )
         if git_executable_path is None:
             raise FileNotFoundError(
                 f"No executable '{self.__GIT_EXECUTABLE_NAME}' found in PATH"
             )
         return cast(Path, git_executable_path)
 
     @property
     def is_available(self) -> bool:
+        """"""
         logger.debug("Checking, if we're working on a git repository")
         exit_code, _out, _err = self.run(
             self.git_executable_path,
             ("rev-parse", "--root-dir"),
             raise_on_exit=False,
             cwd=self.current_path,
         )
         return 0 == exit_code
 
     @property
     def is_clean(self) -> bool:
+        """"""
         try:
             logger.debug("Checking, if there are any changes")
             _ex, out, _err = self.run(
                 self.git_executable_path,
                 ("status", "--porcelain"),
                 cwd=self.current_path,
                 raise_on_exit=True,
@@ -73,14 +81,27 @@
         except CalledProcessError as cpe:
             raise VcsProviderError(
                 f"Failed to check if {self.current_path} is a clean "
                 f"git repository. Reason: {cpe.stderr}"
             ) from cpe
 
     def check_in_items(self, message: str, *files: tuple[Path, ...]) -> None:
+        """
+
+        Parameters
+        ----------
+        message: str :
+
+        *files: tuple[Path, ...] :
+
+
+        Returns
+        -------
+
+        """
         try:
             args: list[str] = ["add", "--update"]
             args.extend(str(f) for f in files)
             logger.debug(
                 "Checking in the following files: \n%s",
                 ", ".join([str(f) for f in files]),
             )
@@ -101,14 +122,25 @@
             f_args = ",".join([str(f) for f in files])
             raise VcsProviderError(
                 f"Failed to check in items in {self.current_path} "
                 f"using {f_args}. Reason: {cpe.stderr}"
             ) from cpe
 
     def create_tag_from_string(self, version_formatted: str) -> None:
+        """
+
+        Parameters
+        ----------
+        version_formatted: str :
+
+
+        Returns
+        -------
+
+        """
         try:
             logger.info(
                 "Creating tag '%s' on current commit.", version_formatted
             )
             _ = self.run(
                 self.git_executable_path,
                 ("tag", version_formatted),
@@ -118,14 +150,15 @@
         except CalledProcessError as cpe:
             raise VcsProviderError(
                 f"Failed to create tag {version_formatted} "
                 f"in {self.current_path}. Reason: {cpe.stderr}"
             ) from cpe
 
     def get_most_recent_tag(self) -> Optional[Version]:
+        """"""
         try:
             logger.debug("Checking for most recent tag.")
             _, output, _ = self.run(
                 self.git_executable_path,
                 ("describe", "--tags", "--abbrev=0"),
                 raise_on_exit=True,
                 cwd=self.current_path,
@@ -139,14 +172,15 @@
             logger.debug("Could not find a tagged version.")
             return None
 
         logger.debug("Found version '%s'", output)
         return Version.from_string(output)
 
     def get_number_of_changes_since_last_release(self) -> int:
+        """"""
         try:
             logger.debug("Searching last tag ...")
             _, output, _ = self.run(
                 self.git_executable_path,
                 ("describe", "--tags"),
                 raise_on_exit=False,
                 cwd=self.current_path,
@@ -166,14 +200,15 @@
         except CalledProcessError as cpe:
             raise VcsProviderError(
                 f"Failed to receive number of commits since last tag."
                 f" Reason: {cpe.stderr}"
             ) from cpe
 
     def get_changes_not_checked_in(self) -> int:
+        """"""
         try:
             logger.debug("Searching for changes")
             _, output, _ = self.run(
                 self.git_executable_path,
                 ("status", "--porcelain"),
                 raise_on_exit=True,
                 cwd=self.current_path,
@@ -188,9 +223,22 @@
                 f"Failed to receive number of changes that are not committed."
                 f" Reason: {cpe.stderr}"
             ) from cpe
 
 
 @vcs_provider("git-cli")
 class GitCliVcsProviderFactory(GitCommonVcsProviderFactory):
+    """"""
+
     def _create_provider(self, path: Path) -> VcsProvider:
+        """
+
+        Parameters
+        ----------
+        path: Path :
+
+
+        Returns
+        -------
+
+        """
         return GitCliVcsProvider(path)
```

### Comparing `pdm-bump-0.7.0a1/tests/action_test.py` & `pdm_bump-0.7.1/tests/action_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,709 +6,700 @@
 # This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
 
-import unittest
 from typing import Callable
 
 from pdm_bump.actions import (
-    PreviewMismatchError,
     VersionModifier,
+)
+from pdm_bump.actions.increment import (
     MajorIncrementingVersionModifier,
     MinorIncrementingVersionModifier,
     MicroIncrementingVersionModifier,
-    AlphaIncrementingVersionModifier,
-    BetaIncrementingVersionModifier,
-    ReleaseCandidateIncrementingVersionModifier,
     FinalizingVersionModifier,
     EpochIncrementingVersionModifier,
     DevelopmentVersionIncrementingVersionModifier,
     PostVersionIncrementingVersionModifier,
 )
+from pdm_bump.actions.preview import (
+    PreviewMismatchError,
+    AlphaIncrementingVersionModifier,
+    BetaIncrementingVersionModifier,
+    ReleaseCandidateIncrementingVersionModifier,
+)
+
 from pdm_bump.core.version import Version
 
+import pytest
+
+parametrize = pytest.mark.parametrize
+assert_raises = pytest.raises
+
 
 class _UnitTestPersister:
     def save_version(self, version: Version) -> None:
         # Just for testing
         pass
 
 _unit_test_persister = _UnitTestPersister()
 
+_CREATE_NEXT_VERSION_PARAMS: list[
+    tuple[str, str, str, Callable[[Version], Version]]
+] = [
+    (
+        "Increment major parts with removing pre-parts and no pre-parts",
+        "1.0.0",
+        "2.0.0",
+        lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment major parts with removing pre-parts and alpha pre-parts",
+        "1.0.0a1",
+        "2.0.0",
+        lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment major parts with removing pre-parts and beta pre-parts",
+        "1.0.0b1",
+        "2.0.0",
+        lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment major parts with removing pre-parts and rc pre-parts",
+        "1.0.0rc1",
+        "2.0.0",
+        lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment major parts with removing pre-parts and dev parts",
+        "1.0.0dev1",
+        "2.0.0",
+        lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment major parts with removing pre-parts and post parts",
+        "1.0.0post1",
+        "2.0.0",
+        lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment major parts with removing pre-parts and local parts",
+        "1.0.0+local",
+        "2.0.0",
+        lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment major parts without removing pre-parts and no pre-parts",
+        "1.0.0",
+        "2.0.0",
+        lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment major parts without removing pre-parts and alpha pre-parts",
+        "1.0.0a1",
+        "2.0.0a1",
+        lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment major parts without removing pre-parts and beta pre-parts",
+        "1.0.0b1",
+        "2.0.0b1",
+        lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment major parts without removing pre-parts and rc pre-parts",
+        "1.0.0rc1",
+        "2.0.0rc1",
+        lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment major parts without removing pre-parts and dev parts",
+        "1.0.0dev1",
+        "2.0.0dev1",
+        lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment major parts without removing pre-parts and post parts",
+        "1.0.0post1",
+        "2.0.0post1",
+        lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment major parts without removing pre-parts and local parts",
+        "1.0.0+local",
+        "2.0.0+local",
+        lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment minor parts with removing pre-parts and no pre-parts",
+        "1.0.0",
+        "1.1.0",
+        lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment minor parts with removing pre-parts and alpha pre-parts",
+        "1.0.0a1",
+        "1.1.0",
+        lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment minor parts with removing pre-parts and beta pre-parts",
+        "1.0.0b1",
+        "1.1.0",
+        lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment minor parts with removing pre-parts and rc pre-parts",
+        "1.0.0rc1",
+        "1.1.0",
+        lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment minor parts with removing pre-parts and dev parts",
+        "1.0.0dev1",
+        "1.1.0",
+        lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment minor parts with removing pre-parts and post parts",
+        "1.0.0post1",
+        "1.1.0",
+        lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment minor parts with removing pre-parts and local parts",
+        "1.0.0+local",
+        "1.1.0",
+        lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment minor parts without removing pre-parts and no pre-parts",
+        "1.0.0",
+        "1.1.0",
+        lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment minor parts without removing pre-parts and alpha pre-parts",
+        "1.0.0a1",
+        "1.1.0a1",
+        lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment minor parts without removing pre-parts and beta pre-parts",
+        "1.0.0b1",
+        "1.1.0b1",
+        lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment minor parts without removing pre-parts and rc pre-parts",
+        "1.0.0rc1",
+        "1.1.0rc1",
+        lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment minor parts without removing pre-parts and dev parts",
+        "1.0.0dev1",
+        "1.1.0dev1",
+        lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment minor parts without removing pre-parts and post parts",
+        "1.0.0post1",
+        "1.1.0post1",
+        lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment minor parts without removing pre-parts and local parts",
+        "1.0.0+local",
+        "1.1.0+local",
+        lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment micro parts with removing pre-parts and no pre-parts",
+        "1.0.0",
+        "1.0.1",
+        lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment micro parts with removing pre-parts and alpha pre-parts",
+        "1.0.0a1",
+        "1.0.1",
+        lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment micro parts with removing pre-parts and beta pre-parts",
+        "1.0.0b1",
+        "1.0.1",
+        lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment micro parts with removing pre-parts and rc pre-parts",
+        "1.0.0rc1",
+        "1.0.1",
+        lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment micro parts with removing pre-parts and dev parts",
+        "1.0.0dev1",
+        "1.0.1",
+        lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment micro parts with removing pre-parts and post parts",
+        "1.0.0post1",
+        "1.0.1",
+        lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment micro parts with removing pre-parts and local parts",
+        "1.0.0+local",
+        "1.0.1",
+        lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment micro parts without removing pre-parts and no pre-parts",
+        "1.0.0",
+        "1.0.1",
+        lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment micro parts without removing pre-parts and alpha pre-parts",
+        "1.0.0a1",
+        "1.0.1a1",
+        lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment micro parts without removing pre-parts and beta pre-parts",
+        "1.0.0b1",
+        "1.0.1b1",
+        lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment micro parts without removing pre-parts and rc pre-parts",
+        "1.0.0rc1",
+        "1.0.1rc1",
+        lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment micro parts without removing pre-parts and dev parts",
+        "1.0.0dev1",
+        "1.0.1dev1",
+        lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment micro parts without removing pre-parts and post parts",
+        "1.0.0post1",
+        "1.0.1post1",
+        lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment micro parts without removing pre-parts and local parts",
+        "1.0.0+local",
+        "1.0.1+local",
+        lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment alpha parts without incrementing micro and providing no pre-release part",
+        "1.0.0",
+        "1.0.0a1",
+        lambda v: AlphaIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment alpha parts without incrementing micro and providing a pre-release part",
+        "1.0.0a1",
+        "1.0.0a2",
+        lambda v: AlphaIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment alpha parts with incrementing micro and providing no pre-release part",
+        "1.0.0",
+        "1.0.1a1",
+        lambda v: AlphaIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment alpha parts with incrementing micro and providing a pre-release part",
+        "1.0.0a1",
+        "1.0.0a2",
+        lambda v: AlphaIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment beta parts without incrementing micro and providing no pre-release part",
+        "1.0.0",
+        "1.0.0b1",
+        lambda v: BetaIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment beta parts without incrementing micro and providing a pre-release part",
+        "1.0.0b1",
+        "1.0.0b2",
+        lambda v: BetaIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment beta parts without incrementing micro and providing a pre-release part",
+        "1.0.0a2",
+        "1.0.0b1",
+        lambda v: BetaIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment beta parts with incrementing micro and providing no pre-release part",
+        "1.0.0",
+        "1.0.1b1",
+        lambda v: BetaIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment beta parts with incrementing micro and providing a pre-release part",
+        "1.0.0b1",
+        "1.0.0b2",
+        lambda v: BetaIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment beta parts with incrementing micro and providing no pre-release part",
+        "1.0.0a2",
+        "1.0.0b1",
+        lambda v: BetaIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment rc parts without incrementing micro and providing no pre-release part",
+        "1.0.0",
+        "1.0.0rc1",
+        lambda v: ReleaseCandidateIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment rc parts without incrementing micro and providing a pre-release part",
+        "1.0.0rc1",
+        "1.0.0rc2",
+        lambda v: ReleaseCandidateIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment rc parts without incrementing micro and providing no pre-release part",
+        "1.0.0a2",
+        "1.0.0rc1",
+        lambda v: ReleaseCandidateIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment rc parts without incrementing micro and providing no pre-release part",
+        "1.0.0b2",
+        "1.0.0rc1",
+        lambda v: ReleaseCandidateIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment rc parts with incrementing micro and providing no pre-release part",
+        "1.0.0",
+        "1.0.1rc1",
+        lambda v: ReleaseCandidateIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment rc parts with incrementing micro and providing a pre-release part",
+        "1.0.0rc1",
+        "1.0.0rc2",
+        lambda v: ReleaseCandidateIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment rc parts with incrementing micro and providing no pre-release part",
+        "1.0.0a2",
+        "1.0.0rc1",
+        lambda v: ReleaseCandidateIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment rc parts with incrementing micro and providing a pre-release part",
+        "1.0.0b2",
+        "1.0.0rc1",
+        lambda v: ReleaseCandidateIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3",
+        "1!1.2.3",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, False),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3a4",
+        "1!1.2.3a4",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, False),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3b4",
+        "1!1.2.3b4",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, False),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3rc4",
+        "1!1.2.3rc4",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, False),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3dev5",
+        "1!1.2.3dev5",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, False),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3post6",
+        "1!1.2.3post6",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, False),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3+local7",
+        "1!1.2.3+local7",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, False),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3b4post3dev6+local7",
+        "1!1.2.3b4post3dev6+local7",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, False),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3",
+        "1!1.2.3",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, False),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3a4",
+        "1!1.2.3",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, False),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3b4",
+        "1!1.2.3",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, False),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3rc4",
+        "1!1.2.3",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, False),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3dev5",
+        "1!1.2.3",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, False),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3post6",
+        "1!1.2.3",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, False),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3+local7",
+        "1!1.2.3",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, False),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3b4post3dev6+local7",
+        "1!1.2.3",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, False),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3",
+        "1!1.0.0",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, True),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3a4",
+        "1!1.0.0",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, True),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3b4",
+        "1!1.0.0",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, True),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3rc4",
+        "1!1.0.0",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, True),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3dev5",
+        "1!1.0.0",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, True),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3post6",
+        "1!1.0.0",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, True),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3+local7",
+        "1!1.0.0",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, True),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3b4post3dev6+local7",
+        "1!1.0.0",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, True),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3",
+        "1!1.0.0",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, True),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3a4",
+        "1!1.0.0",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, True),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3b4",
+        "1!1.0.0",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, True),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3rc4",
+        "1!1.0.0",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, True),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3dev5",
+        "1!1.0.0",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, True),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3post6",
+        "1!1.0.0",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, True),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3+local7",
+        "1!1.0.0",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, True),
+    ),
+    (
+        "Increment epoch without an epoch and without resetting version or removing any version part",
+        "1.2.3b4post3dev6+local7",
+        "1!1.0.0",
+        lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, True),
+    ),
+    (
+        "Remove non-final parts",
+        "1.2.3",
+        "1.2.3",
+        lambda v: FinalizingVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Remove non-final parts",
+        "1.2.3a1",
+        "1.2.3",
+        lambda v: FinalizingVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Remove non-final parts",
+        "1.2.3b2",
+        "1.2.3",
+        lambda v: FinalizingVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Remove non-final parts",
+        "1.2.3rc3",
+        "1.2.3",
+        lambda v: FinalizingVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Remove non-final parts",
+        "1.2.3-dev1",
+        "1.2.3",
+        lambda v: FinalizingVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Remove non-final parts",
+        "1.2.3-post4",
+        "1.2.3",
+        lambda v: FinalizingVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Remove non-final parts",
+        "1.2.3+local8",
+        "1.2.3",
+        lambda v: FinalizingVersionModifier(v, _unit_test_persister),
+    ),
+    (
+        "Remove non-final parts",
+        "1.2.3-b4-post6-dev8+local9",
+        "1.2.3",
+        lambda v: FinalizingVersionModifier(v, _unit_test_persister),
+    ),
+]  # TODO Test Dev and Post Incrementing modifier
+_CREATE_NEXT_VERSION_ERROR_PARAMS: list[
+    tuple[str, str, Callable[[Version], VersionModifier]]
+] = [
+    (
+        "Increment alpha version if beta is present",
+        "1.2.3b1",
+        lambda v: AlphaIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment alpha version if beta is present",
+        "1.2.3b1",
+        lambda v: AlphaIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment alpha version if rc is present",
+        "1.2.3rc1",
+        lambda v: AlphaIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment alpha version if rc is present",
+        "1.2.3rc1",
+        lambda v: AlphaIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+    (
+        "Increment beta version if rc is present",
+        "1.2.3rc1",
+        lambda v: BetaIncrementingVersionModifier(v, _unit_test_persister, False),
+    ),
+    (
+        "Increment beta version if rc is present",
+        "1.2.3rc1",
+        lambda v: BetaIncrementingVersionModifier(v, _unit_test_persister, True),
+    ),
+]
+
+@parametrize(",".join(["message", "current_version_str", "expected_version_str", "factory"]), _CREATE_NEXT_VERSION_PARAMS)
+def test_create_next_version_success(message, current_version_str, expected_version_str, factory) -> None:
+    current: Version = Version.from_string(current_version_str)
+    expected: Version = Version.from_string(expected_version_str)
+
+    command: VersionModifier = factory(current)
+
+    modified: Version = command.create_new_version()
+    assert modified == expected
+
+@parametrize(",".join(["message", "current_version_str", "factory"]), _CREATE_NEXT_VERSION_ERROR_PARAMS)
+def test_create_next_version_fail(message, current_version_str, factory) -> None:
+    current: Version = Version.from_string(current_version_str)
+
+    command: VersionModifier = factory(current)
 
-class ActionTest(unittest.TestCase):
-    CREATE_NEXT_VERSION_PARAMS: list[
-        tuple[str, str, str, Callable[[Version], Version]]
-    ] = [
-        (
-            "Increment major parts with removing pre-parts and no pre-parts",
-            "1.0.0",
-            "2.0.0",
-            lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment major parts with removing pre-parts and alpha pre-parts",
-            "1.0.0a1",
-            "2.0.0",
-            lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment major parts with removing pre-parts and beta pre-parts",
-            "1.0.0b1",
-            "2.0.0",
-            lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment major parts with removing pre-parts and rc pre-parts",
-            "1.0.0rc1",
-            "2.0.0",
-            lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment major parts with removing pre-parts and dev parts",
-            "1.0.0dev1",
-            "2.0.0",
-            lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment major parts with removing pre-parts and post parts",
-            "1.0.0post1",
-            "2.0.0",
-            lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment major parts with removing pre-parts and local parts",
-            "1.0.0+local",
-            "2.0.0",
-            lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment major parts without removing pre-parts and no pre-parts",
-            "1.0.0",
-            "2.0.0",
-            lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment major parts without removing pre-parts and alpha pre-parts",
-            "1.0.0a1",
-            "2.0.0a1",
-            lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment major parts without removing pre-parts and beta pre-parts",
-            "1.0.0b1",
-            "2.0.0b1",
-            lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment major parts without removing pre-parts and rc pre-parts",
-            "1.0.0rc1",
-            "2.0.0rc1",
-            lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment major parts without removing pre-parts and dev parts",
-            "1.0.0dev1",
-            "2.0.0dev1",
-            lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment major parts without removing pre-parts and post parts",
-            "1.0.0post1",
-            "2.0.0post1",
-            lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment major parts without removing pre-parts and local parts",
-            "1.0.0+local",
-            "2.0.0+local",
-            lambda v: MajorIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment minor parts with removing pre-parts and no pre-parts",
-            "1.0.0",
-            "1.1.0",
-            lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment minor parts with removing pre-parts and alpha pre-parts",
-            "1.0.0a1",
-            "1.1.0",
-            lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment minor parts with removing pre-parts and beta pre-parts",
-            "1.0.0b1",
-            "1.1.0",
-            lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment minor parts with removing pre-parts and rc pre-parts",
-            "1.0.0rc1",
-            "1.1.0",
-            lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment minor parts with removing pre-parts and dev parts",
-            "1.0.0dev1",
-            "1.1.0",
-            lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment minor parts with removing pre-parts and post parts",
-            "1.0.0post1",
-            "1.1.0",
-            lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment minor parts with removing pre-parts and local parts",
-            "1.0.0+local",
-            "1.1.0",
-            lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment minor parts without removing pre-parts and no pre-parts",
-            "1.0.0",
-            "1.1.0",
-            lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment minor parts without removing pre-parts and alpha pre-parts",
-            "1.0.0a1",
-            "1.1.0a1",
-            lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment minor parts without removing pre-parts and beta pre-parts",
-            "1.0.0b1",
-            "1.1.0b1",
-            lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment minor parts without removing pre-parts and rc pre-parts",
-            "1.0.0rc1",
-            "1.1.0rc1",
-            lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment minor parts without removing pre-parts and dev parts",
-            "1.0.0dev1",
-            "1.1.0dev1",
-            lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment minor parts without removing pre-parts and post parts",
-            "1.0.0post1",
-            "1.1.0post1",
-            lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment minor parts without removing pre-parts and local parts",
-            "1.0.0+local",
-            "1.1.0+local",
-            lambda v: MinorIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment micro parts with removing pre-parts and no pre-parts",
-            "1.0.0",
-            "1.0.1",
-            lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment micro parts with removing pre-parts and alpha pre-parts",
-            "1.0.0a1",
-            "1.0.1",
-            lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment micro parts with removing pre-parts and beta pre-parts",
-            "1.0.0b1",
-            "1.0.1",
-            lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment micro parts with removing pre-parts and rc pre-parts",
-            "1.0.0rc1",
-            "1.0.1",
-            lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment micro parts with removing pre-parts and dev parts",
-            "1.0.0dev1",
-            "1.0.1",
-            lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment micro parts with removing pre-parts and post parts",
-            "1.0.0post1",
-            "1.0.1",
-            lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment micro parts with removing pre-parts and local parts",
-            "1.0.0+local",
-            "1.0.1",
-            lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment micro parts without removing pre-parts and no pre-parts",
-            "1.0.0",
-            "1.0.1",
-            lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment micro parts without removing pre-parts and alpha pre-parts",
-            "1.0.0a1",
-            "1.0.1a1",
-            lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment micro parts without removing pre-parts and beta pre-parts",
-            "1.0.0b1",
-            "1.0.1b1",
-            lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment micro parts without removing pre-parts and rc pre-parts",
-            "1.0.0rc1",
-            "1.0.1rc1",
-            lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment micro parts without removing pre-parts and dev parts",
-            "1.0.0dev1",
-            "1.0.1dev1",
-            lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment micro parts without removing pre-parts and post parts",
-            "1.0.0post1",
-            "1.0.1post1",
-            lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment micro parts without removing pre-parts and local parts",
-            "1.0.0+local",
-            "1.0.1+local",
-            lambda v: MicroIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment alpha parts without incrementing micro and providing no pre-release part",
-            "1.0.0",
-            "1.0.0a1",
-            lambda v: AlphaIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment alpha parts without incrementing micro and providing a pre-release part",
-            "1.0.0a1",
-            "1.0.0a2",
-            lambda v: AlphaIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment alpha parts with incrementing micro and providing no pre-release part",
-            "1.0.0",
-            "1.0.1a1",
-            lambda v: AlphaIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment alpha parts with incrementing micro and providing a pre-release part",
-            "1.0.0a1",
-            "1.0.0a2",
-            lambda v: AlphaIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment beta parts without incrementing micro and providing no pre-release part",
-            "1.0.0",
-            "1.0.0b1",
-            lambda v: BetaIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment beta parts without incrementing micro and providing a pre-release part",
-            "1.0.0b1",
-            "1.0.0b2",
-            lambda v: BetaIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment beta parts without incrementing micro and providing a pre-release part",
-            "1.0.0a2",
-            "1.0.0b1",
-            lambda v: BetaIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment beta parts with incrementing micro and providing no pre-release part",
-            "1.0.0",
-            "1.0.1b1",
-            lambda v: BetaIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment beta parts with incrementing micro and providing a pre-release part",
-            "1.0.0b1",
-            "1.0.0b2",
-            lambda v: BetaIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment beta parts with incrementing micro and providing no pre-release part",
-            "1.0.0a2",
-            "1.0.0b1",
-            lambda v: BetaIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment rc parts without incrementing micro and providing no pre-release part",
-            "1.0.0",
-            "1.0.0rc1",
-            lambda v: ReleaseCandidateIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment rc parts without incrementing micro and providing a pre-release part",
-            "1.0.0rc1",
-            "1.0.0rc2",
-            lambda v: ReleaseCandidateIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment rc parts without incrementing micro and providing no pre-release part",
-            "1.0.0a2",
-            "1.0.0rc1",
-            lambda v: ReleaseCandidateIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment rc parts without incrementing micro and providing no pre-release part",
-            "1.0.0b2",
-            "1.0.0rc1",
-            lambda v: ReleaseCandidateIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment rc parts with incrementing micro and providing no pre-release part",
-            "1.0.0",
-            "1.0.1rc1",
-            lambda v: ReleaseCandidateIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment rc parts with incrementing micro and providing a pre-release part",
-            "1.0.0rc1",
-            "1.0.0rc2",
-            lambda v: ReleaseCandidateIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment rc parts with incrementing micro and providing no pre-release part",
-            "1.0.0a2",
-            "1.0.0rc1",
-            lambda v: ReleaseCandidateIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment rc parts with incrementing micro and providing a pre-release part",
-            "1.0.0b2",
-            "1.0.0rc1",
-            lambda v: ReleaseCandidateIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3",
-            "1!1.2.3",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, False),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3a4",
-            "1!1.2.3a4",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, False),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3b4",
-            "1!1.2.3b4",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, False),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3rc4",
-            "1!1.2.3rc4",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, False),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3dev5",
-            "1!1.2.3dev5",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, False),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3post6",
-            "1!1.2.3post6",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, False),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3+local7",
-            "1!1.2.3+local7",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, False),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3b4post3dev6+local7",
-            "1!1.2.3b4post3dev6+local7",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, False),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3",
-            "1!1.2.3",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, False),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3a4",
-            "1!1.2.3",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, False),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3b4",
-            "1!1.2.3",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, False),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3rc4",
-            "1!1.2.3",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, False),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3dev5",
-            "1!1.2.3",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, False),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3post6",
-            "1!1.2.3",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, False),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3+local7",
-            "1!1.2.3",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, False),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3b4post3dev6+local7",
-            "1!1.2.3",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, False),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3",
-            "1!1.0.0",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, True),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3a4",
-            "1!1.0.0",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, True),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3b4",
-            "1!1.0.0",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, True),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3rc4",
-            "1!1.0.0",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, True),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3dev5",
-            "1!1.0.0",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, True),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3post6",
-            "1!1.0.0",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, True),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3+local7",
-            "1!1.0.0",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, True),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3b4post3dev6+local7",
-            "1!1.0.0",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, False, True),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3",
-            "1!1.0.0",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, True),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3a4",
-            "1!1.0.0",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, True),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3b4",
-            "1!1.0.0",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, True),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3rc4",
-            "1!1.0.0",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, True),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3dev5",
-            "1!1.0.0",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, True),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3post6",
-            "1!1.0.0",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, True),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3+local7",
-            "1!1.0.0",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, True),
-        ),
-        (
-            "Increment epoch without an epoch and without resetting version or removing any version part",
-            "1.2.3b4post3dev6+local7",
-            "1!1.0.0",
-            lambda v: EpochIncrementingVersionModifier(v, _unit_test_persister, True, True),
-        ),
-        (
-            "Remove non-final parts",
-            "1.2.3",
-            "1.2.3",
-            lambda v: FinalizingVersionModifier(v, _unit_test_persister),
-        ),
-        (
-            "Remove non-final parts",
-            "1.2.3a1",
-            "1.2.3",
-            lambda v: FinalizingVersionModifier(v, _unit_test_persister),
-        ),
-        (
-            "Remove non-final parts",
-            "1.2.3b2",
-            "1.2.3",
-            lambda v: FinalizingVersionModifier(v, _unit_test_persister),
-        ),
-        (
-            "Remove non-final parts",
-            "1.2.3rc3",
-            "1.2.3",
-            lambda v: FinalizingVersionModifier(v, _unit_test_persister),
-        ),
-        (
-            "Remove non-final parts",
-            "1.2.3-dev1",
-            "1.2.3",
-            lambda v: FinalizingVersionModifier(v, _unit_test_persister),
-        ),
-        (
-            "Remove non-final parts",
-            "1.2.3-post4",
-            "1.2.3",
-            lambda v: FinalizingVersionModifier(v, _unit_test_persister),
-        ),
-        (
-            "Remove non-final parts",
-            "1.2.3+local8",
-            "1.2.3",
-            lambda v: FinalizingVersionModifier(v, _unit_test_persister),
-        ),
-        (
-            "Remove non-final parts",
-            "1.2.3-b4-post6-dev8+local9",
-            "1.2.3",
-            lambda v: FinalizingVersionModifier(v, _unit_test_persister),
-        ),
-    ]  # TODO Test Dev and Post Incrementing modifier
-    CREATE_NEXT_VERSION_ERROR_PARAMS: list[
-        tuple[str, str, Callable[[Version], VersionModifier]]
-    ] = [
-        (
-            "Increment alpha version if beta is present",
-            "1.2.3b1",
-            lambda v: AlphaIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment alpha version if beta is present",
-            "1.2.3b1",
-            lambda v: AlphaIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment alpha version if rc is present",
-            "1.2.3rc1",
-            lambda v: AlphaIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment alpha version if rc is present",
-            "1.2.3rc1",
-            lambda v: AlphaIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-        (
-            "Increment beta version if rc is present",
-            "1.2.3rc1",
-            lambda v: BetaIncrementingVersionModifier(v, _unit_test_persister, False),
-        ),
-        (
-            "Increment beta version if rc is present",
-            "1.2.3rc1",
-            lambda v: BetaIncrementingVersionModifier(v, _unit_test_persister, True),
-        ),
-    ]
-
-    def test_create_next_version_success(self) -> None:
-        for (
-            message,
-            current_version_str,
-            expected_version_str,
-            factory,
-        ) in self.CREATE_NEXT_VERSION_PARAMS:
-            with self.subTest(
-                message,
-                current=current_version_str,
-                expected=expected_version_str,
-            ):
-                current: Version = Version.from_string(current_version_str)
-                expected: Version = Version.from_string(expected_version_str)
-
-                command: VersionModifier = factory(current)
-
-                modified: Version = command.create_new_version()
-                self.assertEqual(modified, expected)
-
-    def test_create_next_version_fail(self) -> None:
-        for (
-            message,
-            current_version_str,
-            factory,
-        ) in self.CREATE_NEXT_VERSION_ERROR_PARAMS:
-            with self.subTest(message, current=current_version_str):
-                current: Version = Version.from_string(current_version_str)
-
-                command: VersionModifier = factory(current)
-
-                self.assertRaises(
-                    PreviewMismatchError, command.create_new_version
-                )
+    with assert_raises(PreviewMismatchError):
+        _ = command.create_new_version()
```

### Comparing `pdm-bump-0.7.0a1/tests/plugin_test.py` & `pdm_bump-0.7.1/tests/plugin_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,25 +6,30 @@
 # This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
 
-from unittest import TestCase
-from typing import Optional
+from typing import Optional, Generator
 from collections.abc import Iterable
 from argparse import ArgumentParser, Namespace, ArgumentError
 
 from pdm.project.config import ConfigItem
 from pdm.cli.commands.base import BaseCommand
 
 from pdm_bump.cli import main
 from pdm_bump.plugin import BumpCommand
 
+import pytest
+
+parametrize = pytest.mark.parametrize
+assert_raises = pytest.raises
+fixture = pytest.fixture
+
 
 _registered_configurations: dict[str, ConfigItem] = {}
 
 
 class _CoreStub:
     registered_command: Optional[type[BaseCommand]] = None
     registered_name: Optional[str] = None
@@ -35,99 +40,84 @@
         self.registered_command = command
         self.registered_name = name
 
     @staticmethod
     def add_config(name: str, config_item: ConfigItem) -> None:
         _registered_configurations[str] = config_item
 
+@fixture
+def registrations() -> Generator:
+    yield
+    _registered_configurations.clear()
+
+def test_registration_command_type(registrations) -> None:
+    core: _CoreStub = _CoreStub()
+    main(core)
+    assert core.registered_command == BumpCommand, "The command is registered correctly"
+
+def test_registration_command_name(registrations) -> None:
+    core: _CoreStub = _CoreStub()
+    main(core)
+    assert core.registered_name is None, "No name has been supplied"
+
+def test_registered_config_items(registrations) -> None:
+    core: _CoreStub = _CoreStub()
+    main(core)
+    assert len(_registered_configurations) == 0, "No config item has been registered"
+
+
+SUB_TEST_PARAMS_WHAT_SUCCESS: Iterable[tuple[str, str]] = [
+    ("major", "major"),
+    ("minor", "minor"),
+    ("micro", "micro"),
+    ("patch", "patch"),
+    ("pre-release", "pre-release"),
+    ("no-pre-release", "no-pre-release"),
+    ("post", "post"),
+    ("dev", "dev"),
+]
+SUB_TEST_PARAMS_PRE_SUCCESS: Iterable[tuple[str, str]] = [
+    ("alpha", "alpha"),
+    ("beta", "beta"),
+    ("c", "c"),
+    ("rc", "rc"),
+]
+SUB_TEST_PARAMS_FAIL: Iterable[tuple[str, list[str]]] = [
+    ("major", ["maj"]),
+    ("minor", ["min"]),
+    ("micro", ["mic"]),
+    ("patch", ["pa"]),
+    ("pre-release", ["pre"]),
+    ("no-pre-release", ["no-pre"]),
+    ("alpha", ["pre-release", "--pre", "a"]),
+    ("beta", ["pre-release", "--pre", "b"]),
+    ("c", ["pre-release", "--pre", "release"]),
+    ("rc", ["pre-release", "--pre", "release-candidate"]),
+]
+
+@parametrize(",".join(["msg", "what_success"]), SUB_TEST_PARAMS_WHAT_SUCCESS)
+def test_parser_setup_what_success(msg, what_success) -> None:
+    parser: ArgumentParser = ArgumentParser()
+    _ = BumpCommand.init_parser(parser)
+
+    options: Namespace = parser.parse_args([what_success])
+
+    assert options.selected_command == what_success, "The first item is only matched"
+
+@parametrize(",".join(["msg", "pre_success"]), SUB_TEST_PARAMS_PRE_SUCCESS)
+def test_parser_setup_pre_success(msg, pre_success) -> None:
+    parser: ArgumentParser = ArgumentParser()
+    _ = BumpCommand.init_parser(parser)
+
+    options: Namespace = parser.parse_args(
+        ["pre-release", "--pre", pre_success]
+    )
+
+    assert options.pre_release_part == pre_success, "The second item is only matched"
+
+@parametrize(",".join(["msg", "options"]), SUB_TEST_PARAMS_FAIL)
+def test_parser_setup_fail(msg, options) -> None:
+    parser: ArgumentParser = ArgumentParser(exit_on_error=False)
+    _ = BumpCommand.init_parser(parser)
 
-class CliRegistrationTest(TestCase):
-    def tearDown(self) -> None:
-        _registered_configurations.clear()
-
-    def test_registration_command_type(self) -> None:
-        core: _CoreStub = _CoreStub()
-        main(core)
-        self.assertEqual(
-            core.registered_command,
-            BumpCommand,
-            "The command is registered correctly",
-        )
-
-    def test_registration_command_name(self) -> None:
-        core: _CoreStub = _CoreStub()
-        main(core)
-        self.assertIsNone(core.registered_name, "No name has been supplied")
-
-    def test_registered_config_items(self) -> None:
-        core: _CoreStub = _CoreStub()
-        main(core)
-        self.assertTrue(
-            len(_registered_configurations) == 0,
-            "No config item has been registered",
-        )
-
-
-class BumpVersionCommandParserTests(TestCase):
-    SUB_TEST_PARAMS_WHAT_SUCCESS: Iterable[tuple[str, str]] = [
-        ("major", "major"),
-        ("minor", "minor"),
-        ("micro", "micro"),
-        ("patch", "patch"),
-        ("pre-release", "pre-release"),
-        ("no-pre-release", "no-pre-release"),
-        ("post", "post"),
-        ("dev", "dev"),
-    ]
-    SUB_TEST_PARAMS_PRE_SUCCESS: Iterable[tuple[str, str]] = [
-        ("alpha", "alpha"),
-        ("beta", "beta"),
-        ("c", "c"),
-        ("rc", "rc"),
-    ]
-    SUB_TEST_PARAMS_FAIL: Iterable[tuple[str, list[str]]] = [
-        ("major", ["maj"]),
-        ("minor", ["min"]),
-        ("micro", ["mic"]),
-        ("patch", ["pa"]),
-        ("pre-release", ["pre"]),
-        ("no-pre-release", ["no-pre"]),
-        ("alpha", ["pre-release", "--pre", "a"]),
-        ("beta", ["pre-release", "--pre", "b"]),
-        ("c", ["pre-release", "--pre", "release"]),
-        ("rc", ["pre-release", "--pre", "release-candidate"]),
-    ]
-
-    def test_parser_setup_what_success(self) -> None:
-        parser: ArgumentParser = ArgumentParser()
-        _ = BumpCommand(parser)
-
-        for msg, what_success in self.SUB_TEST_PARAMS_WHAT_SUCCESS:
-            with self.subTest(msg, what=what_success):
-                options: Namespace = parser.parse_args([what_success])
-                self.assertEqual(
-                    options.selected_command,
-                    what_success,
-                    "The first item is only matched",
-                )
-
-    def test_parser_setup_pre_success(self) -> None:
-        parser: ArgumentParser = ArgumentParser()
-        _ = BumpCommand(parser)
-
-        for msg, pre_success in self.SUB_TEST_PARAMS_PRE_SUCCESS:
-            with self.subTest(msg, pre=pre_success):
-                options: Namespace = parser.parse_args(
-                    ["pre-release", "--pre", pre_success]
-                )
-                self.assertEqual(
-                    options.pre_release_part, pre_success, "The second item is only matched"
-                )
-
-    def test_parser_setup_fail(self) -> None:
-        parser: ArgumentParser = ArgumentParser(exit_on_error=False)
-        _ = BumpCommand(parser)
-
-        for msg, options in self.SUB_TEST_PARAMS_FAIL:
-            with self.subTest(msg, options=options):
-                call = lambda options=options: parser.parse_args(options)
-                self.assertRaises(ArgumentError, call)
+    with assert_raises(ArgumentError):
+        parser.parse_args(options)
```

### Comparing `pdm-bump-0.7.0a1/tests/version_test.py` & `pdm_bump-0.7.1/tests/version_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,703 +6,694 @@
 # This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
 
-import unittest
-
 from typing import Final, final
 
 from pdm_bump.core.version import (
     Version,
     VersionParserError,
     Pep440VersionFormatter,
     BaseVersion,
 )
 
+import pytest
 
-@final
-class ParseVersionTest(unittest.TestCase):
-    SUB_TESTS_VERSION_FROM_STR_RLS: Final[
-        list[tuple[str, str, tuple[int, int, int]]]
-    ] = [
-        ("Regular default version", "1.0.0", (1, 0, 0)),
-        ("Regular default version no micro", "1.0", (1, 0, 0)),
-        ("Regular default version no minor and no micro", "1", (1, 0, 0)),
-        ("Pre-fixed default version", "v1.0.0", (1, 0, 0)),
-        ("Pre-fixed default version no micro", "v1.0", (1, 0, 0)),
-        ("Pre-fixed default version no minor and no micro", "v1", (1, 0, 0)),
-        ("Regular non-final version", "0.1.0", (0, 1, 0)),
-        ("Regular non-final version no micro", "0.1.0", (0, 1, 0)),
-        ("Pre-fixed non-final version", "v0.1.0", (0, 1, 0)),
-        ("Pre-fixed non-final version no micro", "v0.1", (0, 1, 0)),
-        ("Regular version", "6.2.13", (6, 2, 13)),
-        ("Regular version no micro", "6.2", (6, 2, 0)),
-        ("Regular version no minor and no micro", "6", (6, 0, 0)),
-        ("Pre-fixed version", "v6.2.13", (6, 2, 13)),
-        ("Pre-fixed version no micro", "v6.2", (6, 2, 0)),
-        ("Pre-fixed version no minor and no micro", "v6", (6, 0, 0)),
-        ("Regular double-digit version", "19.22.83", (19, 22, 83)),
-        ("Regular double-digit version no micro", "19.22", (19, 22, 0)),
-        (
-            "Regular double-digit version no minor and no micro",
-            "19",
-            (19, 0, 0),
-        ),
-        ("Pre-fixed double-digit version", "v19.22.83", (19, 22, 83)),
-        ("Pre-fixed double-digit version no micro", "v19.22", (19, 22, 0)),
-        (
-            "Pre-fixed double-digit version no minor and no micro",
-            "v19",
-            (19, 0, 0),
-        ),
-    ]
-    SUB_TESTS_VERSION_FROM_STR_EPOCH: Final[list[tuple[str, str, int]]] = [
-        ("No epoch set", "1.0.0", 0),
-        ("Epoch is one", "1!1.0.0", 1),
-        ("Epoch is double-digit", "17!1.0.0", 17),
-    ]
-    SUB_TESTS_VERSION_FROM_STR_PRE: Final[
-        list[tuple[str, str, tuple[str, int]]]
-    ] = [
-        ("None: Alpha short single digit no prefix", "0.1.0a1", ("a", 1)),
-        ("None: Alpha long single digit no prefix", "0.1.0alpha1", ("a", 1)),
-        ("None: Alpha short single digit prefix", "v0.1.0a1", ("a", 1)),
-        ("None: Alpha long single digit prefix", "v0.1.0alpha1", ("a", 1)),
-        ("None: Alpha short double digit no prefix", "0.1.0a23", ("a", 23)),
-        ("None: Alpha long double digit no prefix", "0.1.0alpha23", ("a", 23)),
-        ("None: Alpha short double digit prefix", "v0.1.0a23", ("a", 23)),
-        ("None: Alpha long double digit prefix", "v0.1.0alpha23", ("a", 23)),
-        ("None: Beta short single digit no prefix", "0.1.0b1", ("b", 1)),
-        ("None: Beta long single digit no prefix", "0.1.0beta1", ("b", 1)),
-        ("None: Beta short single digit prefix", "v0.1.0b1", ("b", 1)),
-        ("None: Beta long single digit prefix", "v0.1.0beta1", ("b", 1)),
-        ("None: Beta short double digit no prefix", "0.1.0b42", ("b", 42)),
-        ("None: Beta long double digit no prefix", "0.1.0beta42", ("b", 42)),
-        ("None: Beta short double digit prefix", "v0.1.0b42", ("b", 42)),
-        ("None: Beta long double digit prefix", "v0.1.0beta42", ("b", 42)),
-        (
-            "None: Release-candidate short single digit no prefix",
-            "0.1.0rc1",
-            ("rc", 1),
-        ),
-        (
-            "None: Release-candidate long single digit no prefix",
-            "0.1.0rc1",
-            ("rc", 1),
-        ),
-        (
-            "None: Release-candidate short single digit prefix",
-            "v0.1.0c1",
-            ("rc", 1),
-        ),
-        (
-            "None: Release-candidate long single digit prefix",
-            "v0.1.0rc1",
-            ("rc", 1),
-        ),
-        (
-            "None: Release-candidate short double digit no prefix",
-            "0.1.0rc99",
-            ("rc", 99),
-        ),
-        (
-            "None: Release-candidate long double digit no prefix",
-            "0.1.0rc99",
-            ("rc", 99),
-        ),
-        (
-            "None: Release-candidate short double digit prefix",
-            "v0.1.0c99",
-            ("rc", 99),
-        ),
-        (
-            "None: Release-candidate long double digit prefix",
-            "v0.1.0rc99",
-            ("rc", 99),
-        ),
-        ("Dot: Alpha short single digit no prefix", "0.1.0.a1", ("a", 1)),
-        ("Dot: Alpha long single digit no prefix", "0.1.0.alpha1", ("a", 1)),
-        ("Dot: Alpha short single digit prefix", "v0.1.0.a1", ("a", 1)),
-        ("Dot: Alpha long single digit prefix", "v0.1.0.alpha1", ("a", 1)),
-        ("Dot: Alpha short double digit no prefix", "0.1.0.a23", ("a", 23)),
-        ("Dot: Alpha long double digit no prefix", "0.1.0.alpha23", ("a", 23)),
-        ("Dot: Alpha short double digit prefix", "v0.1.0.a23", ("a", 23)),
-        ("Dot: Alpha long double digit prefix", "v0.1.0.alpha23", ("a", 23)),
-        ("Dot: Beta short single digit no prefix", "0.1.0.b1", ("b", 1)),
-        ("Dot: Beta long single digit no prefix", "0.1.0.beta1", ("b", 1)),
-        ("Dot: Beta short single digit prefix", "v0.1.0.b1", ("b", 1)),
-        ("Dot: Beta long single digit prefix", "v0.1.0.beta1", ("b", 1)),
-        ("Dot: Beta short double digit no prefix", "0.1.0.b42", ("b", 42)),
-        ("Dot: Beta long double digit no prefix", "0.1.0.beta42", ("b", 42)),
-        ("Dot: Beta short double digit prefix", "v0.1.0.b42", ("b", 42)),
-        ("Dot: Beta long double digit prefix", "v0.1.0.beta42", ("b", 42)),
-        (
-            "Dot: Release-candidate short single digit no prefix",
-            "0.1.0.rc1",
-            ("rc", 1),
-        ),
-        (
-            "Dot: Release-candidate long single digit no prefix",
-            "0.1.0.rc1",
-            ("rc", 1),
-        ),
-        (
-            "Dot: Release-candidate short single digit prefix",
-            "v0.1.0.c1",
-            ("rc", 1),
-        ),
-        (
-            "Dot: Release-candidate long single digit prefix",
-            "v0.1.0.rc1",
-            ("rc", 1),
-        ),
-        (
-            "Dot: Release-candidate short double digit no prefix",
-            "0.1.0.rc99",
-            ("rc", 99),
-        ),
-        (
-            "Dot: Release-candidate long double digit no prefix",
-            "0.1.0.rc99",
-            ("rc", 99),
-        ),
-        (
-            "Dot: Release-candidate short double digit prefix",
-            "v0.1.0.c99",
-            ("rc", 99),
-        ),
-        (
-            "Dot: Release-candidate long double digit prefix",
-            "v0.1.0.rc99",
-            ("rc", 99),
-        ),
-        ("Hyphen: Alpha short single digit no prefix", "0.1.0-a1", ("a", 1)),
-        (
-            "Hyphen: Alpha long single digit no prefix",
-            "0.1.0-alpha1",
-            ("a", 1),
-        ),
-        ("Hyphen: Alpha short single digit prefix", "v0.1.0-a1", ("a", 1)),
-        ("Hyphen: Alpha long single digit prefix", "v0.1.0-alpha1", ("a", 1)),
-        ("Hyphen: Alpha short double digit no prefix", "0.1.0-a23", ("a", 23)),
-        (
-            "Hyphen: Alpha long double digit no prefix",
-            "0.1.0-alpha23",
-            ("a", 23),
-        ),
-        ("Hyphen: Alpha short double digit prefix", "v0.1.0-a23", ("a", 23)),
-        (
-            "Hyphen: Alpha long double digit prefix",
-            "v0.1.0-alpha23",
-            ("a", 23),
-        ),
-        ("Hyphen: Beta short single digit no prefix", "0.1.0-b1", ("b", 1)),
-        ("Hyphen: Beta long single digit no prefix", "0.1.0-beta1", ("b", 1)),
-        ("Hyphen: Beta short single digit prefix", "v0.1.0-b1", ("b", 1)),
-        ("Hyphen: Beta long single digit prefix", "v0.1.0-beta1", ("b", 1)),
-        ("Hyphen: Beta short double digit no prefix", "0.1.0-b42", ("b", 42)),
-        (
-            "Hyphen: Beta long double digit no prefix",
-            "0.1.0-beta42",
-            ("b", 42),
-        ),
-        ("Hyphen: Beta short double digit prefix", "v0.1.0-b42", ("b", 42)),
-        ("Hyphen: Beta long double digit prefix", "v0.1.0-beta42", ("b", 42)),
-        (
-            "Hyphen: Release-candidate short single digit no prefix",
-            "0.1.0-rc1",
-            ("rc", 1),
-        ),
-        (
-            "Hyphen: Release-candidate long single digit no prefix",
-            "0.1.0-rc1",
-            ("rc", 1),
-        ),
-        (
-            "Hyphen: Release-candidate short single digit prefix",
-            "v0.1.0-c1",
-            ("rc", 1),
-        ),
-        (
-            "Hyphen: Release-candidate long single digit prefix",
-            "v0.1.0-rc1",
-            ("rc", 1),
-        ),
-        (
-            "Hyphen: Release-candidate short double digit no prefix",
-            "0.1.0-rc99",
-            ("rc", 99),
-        ),
-        (
-            "Hyphen: Release-candidate long double digit no prefix",
-            "0.1.0-rc99",
-            ("rc", 99),
-        ),
-        (
-            "Hyphen: Release-candidate short double digit prefix",
-            "v0.1.0-c99",
-            ("rc", 99),
-        ),
-        (
-            "Hyphen: Release-candidate long double digit prefix",
-            "v0.1.0-rc99",
-            ("rc", 99),
-        ),
-        (
-            "Underscore: Alpha short single digit no prefix",
-            "0.1.0_a1",
-            ("a", 1),
-        ),
-        (
-            "Underscore: Alpha long single digit no prefix",
-            "0.1.0_alpha1",
-            ("a", 1),
-        ),
-        ("Underscore: Alpha short single digit prefix", "v0.1.0_a1", ("a", 1)),
-        (
-            "Underscore: Alpha long single digit prefix",
-            "v0.1.0_alpha1",
-            ("a", 1),
-        ),
-        (
-            "Underscore: Alpha short double digit no prefix",
-            "0.1.0_a23",
-            ("a", 23),
-        ),
-        (
-            "Underscore: Alpha long double digit no prefix",
-            "0.1.0_alpha23",
-            ("a", 23),
-        ),
-        (
-            "Underscore: Alpha short double digit prefix",
-            "v0.1.0_a23",
-            ("a", 23),
-        ),
-        (
-            "Underscore: Alpha long double digit prefix",
-            "v0.1.0_alpha23",
-            ("a", 23),
-        ),
-        (
-            "Underscore: Beta short single digit no prefix",
-            "0.1.0_b1",
-            ("b", 1),
-        ),
-        (
-            "Underscore: Beta long single digit no prefix",
-            "0.1.0_beta1",
-            ("b", 1),
-        ),
-        ("Underscore: Beta short single digit prefix", "v0.1.0_b1", ("b", 1)),
-        (
-            "Underscore: Beta long single digit prefix",
-            "v0.1.0_beta1",
-            ("b", 1),
-        ),
-        (
-            "Underscore: Beta short double digit no prefix",
-            "0.1.0_b42",
-            ("b", 42),
-        ),
-        (
-            "Underscore: Beta long double digit no prefix",
-            "0.1.0_beta42",
-            ("b", 42),
-        ),
-        (
-            "Underscore: Beta short double digit prefix",
-            "v0.1.0_b42",
-            ("b", 42),
-        ),
-        (
-            "Underscore: Beta long double digit prefix",
-            "v0.1.0_beta42",
-            ("b", 42),
-        ),
-        (
-            "Underscore: Release-candidate short single digit no prefix",
-            "0.1.0_rc1",
-            ("rc", 1),
-        ),
-        (
-            "Underscore: Release-candidate long single digit no prefix",
-            "0.1.0_rc1",
-            ("rc", 1),
-        ),
-        (
-            "Underscore: Release-candidate short single digit prefix",
-            "v0.1.0_c1",
-            ("rc", 1),
-        ),
-        (
-            "Underscore: Release-candidate long single digit prefix",
-            "v0.1.0_rc1",
-            ("rc", 1),
-        ),
-        (
-            "Underscore: Release-candidate short double digit no prefix",
-            "0.1.0_rc99",
-            ("rc", 99),
-        ),
-        (
-            "Underscore: Release-candidate long double digit no prefix",
-            "0.1.0_rc99",
-            ("rc", 99),
-        ),
-        (
-            "Underscore: Release-candidate short double digit prefix",
-            "v0.1.0_c99",
-            ("rc", 99),
-        ),
-        (
-            "Underscore: Release-candidate long double digit prefix",
-            "v0.1.0_rc99",
-            ("rc", 99),
-        ),
-    ]
-    SUB_TESTS_VERSION_FROM_STR_DEV: Final[
-        list[tuple[str, str, tuple[str, int]]]
-    ] = [
-        ("Regular version zero digit none", "0.0.1dev0", ("dev", 0)),
-        ("Regular version zero digit dot", "0.0.1.dev0", ("dev", 0)),
-        ("Regular version zero digit hyphen", "0.0.1-dev0", ("dev", 0)),
-        ("Regular version zero digit underscore", "0.0.1_dev0", ("dev", 0)),
-        ("Regular version no digit none", "0.0.1dev", ("dev", 0)),
-        ("Regular version no digit dot", "0.0.1.dev", ("dev", 0)),
-        ("Regular version no digit hyphen", "0.0.1-dev", ("dev", 0)),
-        ("Regular version no digit underscore", "0.0.1_dev", ("dev", 0)),
-        ("Regular version single digit none", "0.0.1dev1", ("dev", 1)),
-        ("Regular version single digit dot", "0.0.1.dev1", ("dev", 1)),
-        ("Regular version single digit hyphen", "0.0.1-dev1", ("dev", 1)),
-        ("Regular version single digit underscore", "0.0.1_dev1", ("dev", 1)),
-        ("Regular version double digit none", "0.0.1dev57", ("dev", 57)),
-        ("Regular version double digit dot", "0.0.1.dev57", ("dev", 57)),
-        ("Regular version double digit hyphen", "0.0.1-dev57", ("dev", 57)),
-        (
-            "Regular version double digit underscore",
-            "0.0.1_dev57",
-            ("dev", 57),
-        ),
-        ("Pre-fixed version single digit none", "v0.0.1dev1", ("dev", 1)),
-        ("Pre-fixed version single digit dot", "v0.0.1.dev1", ("dev", 1)),
-        ("Pre-fixed version single digit hyphen", "v0.0.1-dev1", ("dev", 1)),
-        (
-            "Pre-fixed version single digit underscore",
-            "v0.0.1_dev1",
-            ("dev", 1),
-        ),
-        ("Pre-fixed version double digit none", "v0.0.1dev57", ("dev", 57)),
-        ("Pre-fixed version double digit dot", "v0.0.1.dev57", ("dev", 57)),
-        ("Pre-fixed version double digit hyphen", "v0.0.1-dev57", ("dev", 57)),
-        (
-            "Pre-fixed version double digit underscore",
-            "v0.0.1_dev57",
-            ("dev", 57),
-        ),
-    ]
-    SUB_TESTS_VERSION_FROM_STR_POST: Final[
-        list[tuple[str, str, tuple[str, int]]]
-    ] = [
-        ("Regular version zero digit none", "2.0.0post0", ("post", 0)),
-        ("Regular version zero digit dot", "2.0.0.post0", ("post", 0)),
-        ("Regular version zero digit hyphen", "2.0.0-post0", ("post", 0)),
-        ("Regular version zero digit underscore", "2.0.0_post0", ("post", 0)),
-        ("Regular version no digit none", "2.0.0post", ("post", 0)),
-        ("Regular version no digit dot", "2.0.0.post", ("post", 0)),
-        ("Regular version no digit hyphen", "2.0.0-post", ("post", 0)),
-        ("Regular version no digit underscore", "2.0.0_post", ("post", 0)),
-        ("Regular version single digit none", "2.0.0post7", ("post", 7)),
-        ("Regular version single digit dot", "2.0.0.post7", ("post", 7)),
-        ("Regular version single digit hyphen", "2.0.0-post7", ("post", 7)),
-        (
-            "Regular version single digit underscore",
-            "2.0.0_post7",
-            ("post", 7),
-        ),
-        ("Regular version double digit none", "2.0.0post63", ("post", 63)),
-        ("Regular version double digit dot", "2.0.0.post63", ("post", 63)),
-        ("Regular version double digit hyphen", "2.0.0-post63", ("post", 63)),
-        (
-            "Regular version double digit underscore",
-            "2.0.0_post63",
-            ("post", 63),
-        ),
-        ("Regular version single digit special form", "2.0.0-3", ("post", 3)),
-        (
-            "Regular version double digit special form",
-            "2.0.0-78",
-            ("post", 78),
-        ),
-        ("Pre-fixed version zero digit none", "v2.0.0post0", ("post", 0)),
-        ("Pre-fixed version zero digit dot", "v2.0.0.post0", ("post", 0)),
-        ("Pre-fixed version zero digit hyphen", "v2.0.0-post0", ("post", 0)),
-        (
-            "Pre-fixed version zero digit underscore",
-            "v2.0.0_post0",
-            ("post", 0),
-        ),
-        ("Pre-fixed version no digit none", "v2.0.0post", ("post", 0)),
-        ("Pre-fixed version no digit dot", "v2.0.0.post", ("post", 0)),
-        ("Pre-fixed version no digit hyphen", "v2.0.0-post", ("post", 0)),
-        ("Pre-fixed version no digit underscore", "v2.0.0_post", ("post", 0)),
-        ("Pre-fixed version single digit none", "v2.0.0post7", ("post", 7)),
-        ("Pre-fixed version single digit dot", "v2.0.0.post7", ("post", 7)),
-        ("Pre-fixed version single digit hyphen", "v2.0.0-post7", ("post", 7)),
-        (
-            "Pre-fixed version single digit underscore",
-            "v2.0.0_post7",
-            ("post", 7),
-        ),
-        ("Pre-fixed version double digit none", "v2.0.0post63", ("post", 63)),
-        ("Pre-fixed version double digit dot", "v2.0.0.post63", ("post", 63)),
-        (
-            "Pre-fixed version double digit hyphen",
-            "v2.0.0-post63",
-            ("post", 63),
-        ),
-        (
-            "Pre-fixed version double digit underscore",
-            "v2.0.0_post63",
-            ("post", 63),
-        ),
-        (
-            "Pre-fixed version single digit special form",
-            "v2.0.0-3",
-            ("post", 3),
-        ),
-        (
-            "Pre-fixed version double digit special form",
-            "v2.0.0-78",
-            ("post", 78),
-        ),
-    ]  # TODO: rev/r
-    SUB_TESTS_VERSION_FROM_STR_LOCAL: Final[list[tuple[str, str, str]]] = [
-        ("Regular version single digit plus", "3.1.4+2", "2"),
-        ("Regular version double digit plus", "3.1.4+12", "12"),
-        ("Regular version alpha-numeric plus", "3.1.4+af2b", "af2b"),
-        (
-            "Regular version hyphen plus",
-            "3.1.4+just-my-2-cents",
-            "just.my.2.cents",
-        ),
-        (
-            "Regular version hyphen underscore plus",
-            "3.1.4+just_my-2_cents",
-            "just.my.2.cents",
-        ),
-        ("Pre-fixed version single digit plus", "v3.1.4+2", "2"),
-        ("Pre-fixed version double digit plus", "v3.1.4+12", "12"),
-        ("Pre-fixed version alpha-numeric plus", "v3.1.4+af2b", "af2b"),
-        (
-            "Pre-fixed version hyphen plus",
-            "v3.1.4+just-my-2-cents",
-            "just.my.2.cents",
-        ),
-        (
-            "Pre-fixed version hyphen underscore plus",
-            "v3.1.4+just_my-2_cents",
-            "just.my.2.cents",
-        ),
-    ]
-    SUB_TESTS_VERSION_PARSE_SUCCESS: Final[list[tuple[str, str]]] = [
-        ("Regular version", "1.2.3"),
-        ("Prefixed version", "v1.2.3"),
-        ("Prefixed version with alpha", "v1.2.3a4"),
-        ("Prefixed version with beta", "v1.2.3b4"),
-        ("Prefixed version with rc", "v1.2.3rc4"),
-        ("Prefixed version with rc as post", "v1.2.3a4post5"),
-        ("Prefixed version with rc as post alternative", "v1.2.3a4-5"),
-        ("Prefixed version with rc as post and dev", "v1.2.3a4-post5.dev17"),
-        (
-            "Prefixed version with rc as post and dev and local",
-            "v1.2.3a4-post5.dev17+erg.13",
-        ),
-    ]
-    SUB_TESTS_VERSION_PARSE_FAIL: Final[list[tuple[str, str]]] = [
-        ("Wrong prefix", "a0.1.0+2"),
-        ("Negative epoch", "-2!v0.1.0+2"),
-        ("Alpha epoch", "f!v0.1.0+2"),
-        ("Wrong separators", "0-1-0"),
-        ("Wrong alpha", "0.1.0alp1"),
-        ("Wrong beta", "0.1.0bet2"),
-        ("Wrong release candidate", "0.1.0relca3"),
-        ("Negative major", "-1.0.0"),
-        ("Negative minor", "1.-2.0"),
-        ("Negative micro", "1.2.-3"),
-    ]
-
-    def test_default_version_is_one(self) -> None:
-        v1: Version = Version.default()
-        v2: Version = Version.from_string("1")
-        self.assertEqual(v1, v2)
-
-    def test_create_version_from_str_epoch_part(self) -> None:
-        for message, version, epoch in self.SUB_TESTS_VERSION_FROM_STR_EPOCH:
-            with self.subTest(message, version=version):
-                v: Version = Version.from_string(version)
-                self.assertEqual(v.epoch, epoch)
-
-    def test_create_version_from_str_rls_part(self) -> None:
-        for message, version, release in self.SUB_TESTS_VERSION_FROM_STR_RLS:
-            with self.subTest(message, version=version):
-                v: Version = Version.from_string(version)
-                self.assertEqual(v.release, release)
-
-    def test_create_version_from_str_preview_part(self) -> None:
-        for message, version, preview in self.SUB_TESTS_VERSION_FROM_STR_PRE:
-            with self.subTest(message, version=version):
-                v: Version = Version.from_string(version)
-                self.assertEqual(v.preview, preview)
-
-    def test_create_version_from_str_dev_part(self) -> None:
-        for message, version, dev in self.SUB_TESTS_VERSION_FROM_STR_DEV:
-            with self.subTest(message, version=version):
-                v: Version = Version.from_string(version)
-                self.assertEqual(v.dev, dev)
-
-    def test_create_version_from_str_post_part(self) -> None:
-        for message, version, post in self.SUB_TESTS_VERSION_FROM_STR_POST:
-            with self.subTest(message, version=version):
-                v: Version = Version.from_string(version)
-                self.assertEqual(v.post, post)
-
-    def test_create_version_from_str_local_part(self) -> None:
-        for message, version, local in self.SUB_TESTS_VERSION_FROM_STR_LOCAL:
-            with self.subTest(message, version=version):
-                v: Version = Version.from_string(version)
-                self.assertEqual(v.local, local)
-
-    def test_create_version_from_str_can_parse_success(self) -> None:
-        for message, version in self.SUB_TESTS_VERSION_PARSE_SUCCESS:
-            with self.subTest(message, version=version):
-                result: bool = Version.can_parse_to_version(version)
-                self.assertTrue(result)
-
-    def test_create_version_from_str_can_parse_fail(self) -> None:
-        for message, version in self.SUB_TESTS_VERSION_PARSE_FAIL:
-            with self.subTest(message, version=version):
-                result: bool = Version.can_parse_to_version(version)
-                self.assertFalse(result)
-
-    def test_create_version_from_str_parse_raises(self) -> None:
-        for message, version in self.SUB_TESTS_VERSION_PARSE_FAIL:
-            with self.subTest(message, version=version):
-                parse = lambda version=version: Version.from_string(version)
-                self.assertRaises(VersionParserError, parse)
+parameterize = pytest.mark.parametrize
+assert_raises = pytest.raises
 
 
-@final
-class CreateVersionTest(unittest.TestCase):
-    pass  # TODO implement
+_SUB_TESTS_VERSION_FROM_STR_RLS: Final[
+    list[tuple[str, str, tuple[int, int, int]]]
+] = [
+    ("Regular default version", "1.0.0", (1, 0, 0)),
+    ("Regular default version no micro", "1.0", (1, 0, 0)),
+    ("Regular default version no minor and no micro", "1", (1, 0, 0)),
+    ("Pre-fixed default version", "v1.0.0", (1, 0, 0)),
+    ("Pre-fixed default version no micro", "v1.0", (1, 0, 0)),
+    ("Pre-fixed default version no minor and no micro", "v1", (1, 0, 0)),
+    ("Regular non-final version", "0.1.0", (0, 1, 0)),
+    ("Regular non-final version no micro", "0.1.0", (0, 1, 0)),
+    ("Pre-fixed non-final version", "v0.1.0", (0, 1, 0)),
+    ("Pre-fixed non-final version no micro", "v0.1", (0, 1, 0)),
+    ("Regular version", "6.2.13", (6, 2, 13)),
+    ("Regular version no micro", "6.2", (6, 2, 0)),
+    ("Regular version no minor and no micro", "6", (6, 0, 0)),
+    ("Pre-fixed version", "v6.2.13", (6, 2, 13)),
+    ("Pre-fixed version no micro", "v6.2", (6, 2, 0)),
+    ("Pre-fixed version no minor and no micro", "v6", (6, 0, 0)),
+    ("Regular double-digit version", "19.22.83", (19, 22, 83)),
+    ("Regular double-digit version no micro", "19.22", (19, 22, 0)),
+    (
+        "Regular double-digit version no minor and no micro",
+        "19",
+        (19, 0, 0),
+    ),
+    ("Pre-fixed double-digit version", "v19.22.83", (19, 22, 83)),
+    ("Pre-fixed double-digit version no micro", "v19.22", (19, 22, 0)),
+    (
+        "Pre-fixed double-digit version no minor and no micro",
+        "v19",
+        (19, 0, 0),
+    ),
+]
+_SUB_TESTS_VERSION_FROM_STR_EPOCH: Final[list[tuple[str, str, int]]] = [
+    ("No epoch set", "1.0.0", 0),
+    ("Epoch is one", "1!1.0.0", 1),
+    ("Epoch is double-digit", "17!1.0.0", 17),
+]
+_SUB_TESTS_VERSION_FROM_STR_PRE: Final[
+    list[tuple[str, str, tuple[str, int]]]
+] = [
+    ("None: Alpha short single digit no prefix", "0.1.0a1", ("a", 1)),
+    ("None: Alpha long single digit no prefix", "0.1.0alpha1", ("a", 1)),
+    ("None: Alpha short single digit prefix", "v0.1.0a1", ("a", 1)),
+    ("None: Alpha long single digit prefix", "v0.1.0alpha1", ("a", 1)),
+    ("None: Alpha short double digit no prefix", "0.1.0a23", ("a", 23)),
+    ("None: Alpha long double digit no prefix", "0.1.0alpha23", ("a", 23)),
+    ("None: Alpha short double digit prefix", "v0.1.0a23", ("a", 23)),
+    ("None: Alpha long double digit prefix", "v0.1.0alpha23", ("a", 23)),
+    ("None: Beta short single digit no prefix", "0.1.0b1", ("b", 1)),
+    ("None: Beta long single digit no prefix", "0.1.0beta1", ("b", 1)),
+    ("None: Beta short single digit prefix", "v0.1.0b1", ("b", 1)),
+    ("None: Beta long single digit prefix", "v0.1.0beta1", ("b", 1)),
+    ("None: Beta short double digit no prefix", "0.1.0b42", ("b", 42)),
+    ("None: Beta long double digit no prefix", "0.1.0beta42", ("b", 42)),
+    ("None: Beta short double digit prefix", "v0.1.0b42", ("b", 42)),
+    ("None: Beta long double digit prefix", "v0.1.0beta42", ("b", 42)),
+    (
+        "None: Release-candidate short single digit no prefix",
+        "0.1.0rc1",
+        ("rc", 1),
+    ),
+    (
+        "None: Release-candidate long single digit no prefix",
+        "0.1.0rc1",
+        ("rc", 1),
+    ),
+    (
+        "None: Release-candidate short single digit prefix",
+        "v0.1.0c1",
+        ("rc", 1),
+    ),
+    (
+        "None: Release-candidate long single digit prefix",
+        "v0.1.0rc1",
+        ("rc", 1),
+    ),
+    (
+        "None: Release-candidate short double digit no prefix",
+        "0.1.0rc99",
+        ("rc", 99),
+    ),
+    (
+        "None: Release-candidate long double digit no prefix",
+        "0.1.0rc99",
+        ("rc", 99),
+    ),
+    (
+        "None: Release-candidate short double digit prefix",
+        "v0.1.0c99",
+        ("rc", 99),
+    ),
+    (
+        "None: Release-candidate long double digit prefix",
+        "v0.1.0rc99",
+        ("rc", 99),
+    ),
+    ("Dot: Alpha short single digit no prefix", "0.1.0.a1", ("a", 1)),
+    ("Dot: Alpha long single digit no prefix", "0.1.0.alpha1", ("a", 1)),
+    ("Dot: Alpha short single digit prefix", "v0.1.0.a1", ("a", 1)),
+    ("Dot: Alpha long single digit prefix", "v0.1.0.alpha1", ("a", 1)),
+    ("Dot: Alpha short double digit no prefix", "0.1.0.a23", ("a", 23)),
+    ("Dot: Alpha long double digit no prefix", "0.1.0.alpha23", ("a", 23)),
+    ("Dot: Alpha short double digit prefix", "v0.1.0.a23", ("a", 23)),
+    ("Dot: Alpha long double digit prefix", "v0.1.0.alpha23", ("a", 23)),
+    ("Dot: Beta short single digit no prefix", "0.1.0.b1", ("b", 1)),
+    ("Dot: Beta long single digit no prefix", "0.1.0.beta1", ("b", 1)),
+    ("Dot: Beta short single digit prefix", "v0.1.0.b1", ("b", 1)),
+    ("Dot: Beta long single digit prefix", "v0.1.0.beta1", ("b", 1)),
+    ("Dot: Beta short double digit no prefix", "0.1.0.b42", ("b", 42)),
+    ("Dot: Beta long double digit no prefix", "0.1.0.beta42", ("b", 42)),
+    ("Dot: Beta short double digit prefix", "v0.1.0.b42", ("b", 42)),
+    ("Dot: Beta long double digit prefix", "v0.1.0.beta42", ("b", 42)),
+    (
+        "Dot: Release-candidate short single digit no prefix",
+        "0.1.0.rc1",
+        ("rc", 1),
+    ),
+    (
+        "Dot: Release-candidate long single digit no prefix",
+        "0.1.0.rc1",
+        ("rc", 1),
+    ),
+    (
+        "Dot: Release-candidate short single digit prefix",
+        "v0.1.0.c1",
+        ("rc", 1),
+    ),
+    (
+        "Dot: Release-candidate long single digit prefix",
+        "v0.1.0.rc1",
+        ("rc", 1),
+    ),
+    (
+        "Dot: Release-candidate short double digit no prefix",
+        "0.1.0.rc99",
+        ("rc", 99),
+    ),
+    (
+        "Dot: Release-candidate long double digit no prefix",
+        "0.1.0.rc99",
+        ("rc", 99),
+    ),
+    (
+        "Dot: Release-candidate short double digit prefix",
+        "v0.1.0.c99",
+        ("rc", 99),
+    ),
+    (
+        "Dot: Release-candidate long double digit prefix",
+        "v0.1.0.rc99",
+        ("rc", 99),
+    ),
+    ("Hyphen: Alpha short single digit no prefix", "0.1.0-a1", ("a", 1)),
+    (
+        "Hyphen: Alpha long single digit no prefix",
+        "0.1.0-alpha1",
+        ("a", 1),
+    ),
+    ("Hyphen: Alpha short single digit prefix", "v0.1.0-a1", ("a", 1)),
+    ("Hyphen: Alpha long single digit prefix", "v0.1.0-alpha1", ("a", 1)),
+    ("Hyphen: Alpha short double digit no prefix", "0.1.0-a23", ("a", 23)),
+    (
+        "Hyphen: Alpha long double digit no prefix",
+        "0.1.0-alpha23",
+        ("a", 23),
+    ),
+    ("Hyphen: Alpha short double digit prefix", "v0.1.0-a23", ("a", 23)),
+    (
+        "Hyphen: Alpha long double digit prefix",
+        "v0.1.0-alpha23",
+        ("a", 23),
+    ),
+    ("Hyphen: Beta short single digit no prefix", "0.1.0-b1", ("b", 1)),
+    ("Hyphen: Beta long single digit no prefix", "0.1.0-beta1", ("b", 1)),
+    ("Hyphen: Beta short single digit prefix", "v0.1.0-b1", ("b", 1)),
+    ("Hyphen: Beta long single digit prefix", "v0.1.0-beta1", ("b", 1)),
+    ("Hyphen: Beta short double digit no prefix", "0.1.0-b42", ("b", 42)),
+    (
+        "Hyphen: Beta long double digit no prefix",
+        "0.1.0-beta42",
+        ("b", 42),
+    ),
+    ("Hyphen: Beta short double digit prefix", "v0.1.0-b42", ("b", 42)),
+    ("Hyphen: Beta long double digit prefix", "v0.1.0-beta42", ("b", 42)),
+    (
+        "Hyphen: Release-candidate short single digit no prefix",
+        "0.1.0-rc1",
+        ("rc", 1),
+    ),
+    (
+        "Hyphen: Release-candidate long single digit no prefix",
+        "0.1.0-rc1",
+        ("rc", 1),
+    ),
+    (
+        "Hyphen: Release-candidate short single digit prefix",
+        "v0.1.0-c1",
+        ("rc", 1),
+    ),
+    (
+        "Hyphen: Release-candidate long single digit prefix",
+        "v0.1.0-rc1",
+        ("rc", 1),
+    ),
+    (
+        "Hyphen: Release-candidate short double digit no prefix",
+        "0.1.0-rc99",
+        ("rc", 99),
+    ),
+    (
+        "Hyphen: Release-candidate long double digit no prefix",
+        "0.1.0-rc99",
+        ("rc", 99),
+    ),
+    (
+        "Hyphen: Release-candidate short double digit prefix",
+        "v0.1.0-c99",
+        ("rc", 99),
+    ),
+    (
+        "Hyphen: Release-candidate long double digit prefix",
+        "v0.1.0-rc99",
+        ("rc", 99),
+    ),
+    (
+        "Underscore: Alpha short single digit no prefix",
+        "0.1.0_a1",
+        ("a", 1),
+    ),
+    (
+        "Underscore: Alpha long single digit no prefix",
+        "0.1.0_alpha1",
+        ("a", 1),
+    ),
+    ("Underscore: Alpha short single digit prefix", "v0.1.0_a1", ("a", 1)),
+    (
+        "Underscore: Alpha long single digit prefix",
+        "v0.1.0_alpha1",
+        ("a", 1),
+    ),
+    (
+        "Underscore: Alpha short double digit no prefix",
+        "0.1.0_a23",
+        ("a", 23),
+    ),
+    (
+        "Underscore: Alpha long double digit no prefix",
+        "0.1.0_alpha23",
+        ("a", 23),
+    ),
+    (
+        "Underscore: Alpha short double digit prefix",
+        "v0.1.0_a23",
+        ("a", 23),
+    ),
+    (
+        "Underscore: Alpha long double digit prefix",
+        "v0.1.0_alpha23",
+        ("a", 23),
+    ),
+    (
+        "Underscore: Beta short single digit no prefix",
+        "0.1.0_b1",
+        ("b", 1),
+    ),
+    (
+        "Underscore: Beta long single digit no prefix",
+        "0.1.0_beta1",
+        ("b", 1),
+    ),
+    ("Underscore: Beta short single digit prefix", "v0.1.0_b1", ("b", 1)),
+    (
+        "Underscore: Beta long single digit prefix",
+        "v0.1.0_beta1",
+        ("b", 1),
+    ),
+    (
+        "Underscore: Beta short double digit no prefix",
+        "0.1.0_b42",
+        ("b", 42),
+    ),
+    (
+        "Underscore: Beta long double digit no prefix",
+        "0.1.0_beta42",
+        ("b", 42),
+    ),
+    (
+        "Underscore: Beta short double digit prefix",
+        "v0.1.0_b42",
+        ("b", 42),
+    ),
+    (
+        "Underscore: Beta long double digit prefix",
+        "v0.1.0_beta42",
+        ("b", 42),
+    ),
+    (
+        "Underscore: Release-candidate short single digit no prefix",
+        "0.1.0_rc1",
+        ("rc", 1),
+    ),
+    (
+        "Underscore: Release-candidate long single digit no prefix",
+        "0.1.0_rc1",
+        ("rc", 1),
+    ),
+    (
+        "Underscore: Release-candidate short single digit prefix",
+        "v0.1.0_c1",
+        ("rc", 1),
+    ),
+    (
+        "Underscore: Release-candidate long single digit prefix",
+        "v0.1.0_rc1",
+        ("rc", 1),
+    ),
+    (
+        "Underscore: Release-candidate short double digit no prefix",
+        "0.1.0_rc99",
+        ("rc", 99),
+    ),
+    (
+        "Underscore: Release-candidate long double digit no prefix",
+        "0.1.0_rc99",
+        ("rc", 99),
+    ),
+    (
+        "Underscore: Release-candidate short double digit prefix",
+        "v0.1.0_c99",
+        ("rc", 99),
+    ),
+    (
+        "Underscore: Release-candidate long double digit prefix",
+        "v0.1.0_rc99",
+        ("rc", 99),
+    ),
+]
+_SUB_TESTS_VERSION_FROM_STR_DEV: Final[
+    list[tuple[str, str, tuple[str, int]]]
+] = [
+    ("Regular version zero digit none", "0.0.1dev0", ("dev", 0)),
+    ("Regular version zero digit dot", "0.0.1.dev0", ("dev", 0)),
+    ("Regular version zero digit hyphen", "0.0.1-dev0", ("dev", 0)),
+    ("Regular version zero digit underscore", "0.0.1_dev0", ("dev", 0)),
+    ("Regular version no digit none", "0.0.1dev", ("dev", 0)),
+    ("Regular version no digit dot", "0.0.1.dev", ("dev", 0)),
+    ("Regular version no digit hyphen", "0.0.1-dev", ("dev", 0)),
+    ("Regular version no digit underscore", "0.0.1_dev", ("dev", 0)),
+    ("Regular version single digit none", "0.0.1dev1", ("dev", 1)),
+    ("Regular version single digit dot", "0.0.1.dev1", ("dev", 1)),
+    ("Regular version single digit hyphen", "0.0.1-dev1", ("dev", 1)),
+    ("Regular version single digit underscore", "0.0.1_dev1", ("dev", 1)),
+    ("Regular version double digit none", "0.0.1dev57", ("dev", 57)),
+    ("Regular version double digit dot", "0.0.1.dev57", ("dev", 57)),
+    ("Regular version double digit hyphen", "0.0.1-dev57", ("dev", 57)),
+    (
+        "Regular version double digit underscore",
+        "0.0.1_dev57",
+        ("dev", 57),
+    ),
+    ("Pre-fixed version single digit none", "v0.0.1dev1", ("dev", 1)),
+    ("Pre-fixed version single digit dot", "v0.0.1.dev1", ("dev", 1)),
+    ("Pre-fixed version single digit hyphen", "v0.0.1-dev1", ("dev", 1)),
+    (
+        "Pre-fixed version single digit underscore",
+        "v0.0.1_dev1",
+        ("dev", 1),
+    ),
+    ("Pre-fixed version double digit none", "v0.0.1dev57", ("dev", 57)),
+    ("Pre-fixed version double digit dot", "v0.0.1.dev57", ("dev", 57)),
+    ("Pre-fixed version double digit hyphen", "v0.0.1-dev57", ("dev", 57)),
+    (
+        "Pre-fixed version double digit underscore",
+        "v0.0.1_dev57",
+        ("dev", 57),
+    ),
+]
+_SUB_TESTS_VERSION_FROM_STR_POST: Final[
+    list[tuple[str, str, tuple[str, int]]]
+] = [
+    ("Regular version zero digit none", "2.0.0post0", ("post", 0)),
+    ("Regular version zero digit dot", "2.0.0.post0", ("post", 0)),
+    ("Regular version zero digit hyphen", "2.0.0-post0", ("post", 0)),
+    ("Regular version zero digit underscore", "2.0.0_post0", ("post", 0)),
+    ("Regular version no digit none", "2.0.0post", ("post", 0)),
+    ("Regular version no digit dot", "2.0.0.post", ("post", 0)),
+    ("Regular version no digit hyphen", "2.0.0-post", ("post", 0)),
+    ("Regular version no digit underscore", "2.0.0_post", ("post", 0)),
+    ("Regular version single digit none", "2.0.0post7", ("post", 7)),
+    ("Regular version single digit dot", "2.0.0.post7", ("post", 7)),
+    ("Regular version single digit hyphen", "2.0.0-post7", ("post", 7)),
+    (
+        "Regular version single digit underscore",
+        "2.0.0_post7",
+        ("post", 7),
+    ),
+    ("Regular version double digit none", "2.0.0post63", ("post", 63)),
+    ("Regular version double digit dot", "2.0.0.post63", ("post", 63)),
+    ("Regular version double digit hyphen", "2.0.0-post63", ("post", 63)),
+    (
+        "Regular version double digit underscore",
+        "2.0.0_post63",
+        ("post", 63),
+    ),
+    ("Regular version single digit special form", "2.0.0-3", ("post", 3)),
+    (
+        "Regular version double digit special form",
+        "2.0.0-78",
+        ("post", 78),
+    ),
+    ("Pre-fixed version zero digit none", "v2.0.0post0", ("post", 0)),
+    ("Pre-fixed version zero digit dot", "v2.0.0.post0", ("post", 0)),
+    ("Pre-fixed version zero digit hyphen", "v2.0.0-post0", ("post", 0)),
+    (
+        "Pre-fixed version zero digit underscore",
+        "v2.0.0_post0",
+        ("post", 0),
+    ),
+    ("Pre-fixed version no digit none", "v2.0.0post", ("post", 0)),
+    ("Pre-fixed version no digit dot", "v2.0.0.post", ("post", 0)),
+    ("Pre-fixed version no digit hyphen", "v2.0.0-post", ("post", 0)),
+    ("Pre-fixed version no digit underscore", "v2.0.0_post", ("post", 0)),
+    ("Pre-fixed version single digit none", "v2.0.0post7", ("post", 7)),
+    ("Pre-fixed version single digit dot", "v2.0.0.post7", ("post", 7)),
+    ("Pre-fixed version single digit hyphen", "v2.0.0-post7", ("post", 7)),
+    (
+        "Pre-fixed version single digit underscore",
+        "v2.0.0_post7",
+        ("post", 7),
+    ),
+    ("Pre-fixed version double digit none", "v2.0.0post63", ("post", 63)),
+    ("Pre-fixed version double digit dot", "v2.0.0.post63", ("post", 63)),
+    (
+        "Pre-fixed version double digit hyphen",
+        "v2.0.0-post63",
+        ("post", 63),
+    ),
+    (
+        "Pre-fixed version double digit underscore",
+        "v2.0.0_post63",
+        ("post", 63),
+    ),
+    (
+        "Pre-fixed version single digit special form",
+        "v2.0.0-3",
+        ("post", 3),
+    ),
+    (
+        "Pre-fixed version double digit special form",
+        "v2.0.0-78",
+        ("post", 78),
+    ),
+]  # TODO: rev/r
+_SUB_TESTS_VERSION_FROM_STR_LOCAL: Final[list[tuple[str, str, str]]] = [
+    ("Regular version single digit plus", "3.1.4+2", "2"),
+    ("Regular version double digit plus", "3.1.4+12", "12"),
+    ("Regular version alpha-numeric plus", "3.1.4+af2b", "af2b"),
+    (
+        "Regular version hyphen plus",
+        "3.1.4+just-my-2-cents",
+        "just.my.2.cents",
+    ),
+    (
+        "Regular version hyphen underscore plus",
+        "3.1.4+just_my-2_cents",
+        "just.my.2.cents",
+    ),
+    ("Pre-fixed version single digit plus", "v3.1.4+2", "2"),
+    ("Pre-fixed version double digit plus", "v3.1.4+12", "12"),
+    ("Pre-fixed version alpha-numeric plus", "v3.1.4+af2b", "af2b"),
+    (
+        "Pre-fixed version hyphen plus",
+        "v3.1.4+just-my-2-cents",
+        "just.my.2.cents",
+    ),
+    (
+        "Pre-fixed version hyphen underscore plus",
+        "v3.1.4+just_my-2_cents",
+        "just.my.2.cents",
+    ),
+]
+_SUB_TESTS_VERSION_PARSE_SUCCESS: Final[list[tuple[str, str]]] = [
+    ("Regular version", "1.2.3"),
+    ("Prefixed version", "v1.2.3"),
+    ("Prefixed version with alpha", "v1.2.3a4"),
+    ("Prefixed version with beta", "v1.2.3b4"),
+    ("Prefixed version with rc", "v1.2.3rc4"),
+    ("Prefixed version with rc as post", "v1.2.3a4post5"),
+    ("Prefixed version with rc as post alternative", "v1.2.3a4-5"),
+    ("Prefixed version with rc as post and dev", "v1.2.3a4-post5.dev17"),
+    (
+        "Prefixed version with rc as post and dev and local",
+        "v1.2.3a4-post5.dev17+erg.13",
+    ),
+]
+_SUB_TESTS_VERSION_PARSE_FAIL: Final[list[tuple[str, str]]] = [
+    ("Wrong prefix", "a0.1.0+2"),
+    ("Negative epoch", "-2!v0.1.0+2"),
+    ("Alpha epoch", "f!v0.1.0+2"),
+    ("Wrong separators", "0-1-0"),
+    ("Wrong alpha", "0.1.0alp1"),
+    ("Wrong beta", "0.1.0bet2"),
+    ("Wrong release candidate", "0.1.0relca3"),
+    ("Negative major", "-1.0.0"),
+    ("Negative minor", "1.-2.0"),
+    ("Negative micro", "1.2.-3"),
+]
+
+def test_default_version_is_one() -> None:
+    v1: Version = Version.default()
+    v2: Version = Version.from_string("1")
+    assert v1 == v2, "Versions match"
+
+@parameterize(",".join(["message", "version", "epoch"]), _SUB_TESTS_VERSION_FROM_STR_EPOCH)
+def test_create_version_from_str_epoch_part(message, version, epoch) -> None:
+    v: Version = Version.from_string(version)
+    assert v.epoch == epoch
+
+@parameterize(",".join(["message", "version", "release"]), _SUB_TESTS_VERSION_FROM_STR_RLS)
+def test_create_version_from_str_rls_part(message, version, release) -> None:
+    v: Version = Version.from_string(version)
+    assert v.release == release
+
+@parameterize(",".join(["message", "version", "preview"]), _SUB_TESTS_VERSION_FROM_STR_PRE)
+def test_create_version_from_str_preview_part(message, version, preview) -> None:
+    v: Version = Version.from_string(version)
+    assert v.preview == preview
+
+@parameterize(",".join(["message", "version", "dev"]), _SUB_TESTS_VERSION_FROM_STR_DEV)
+def test_create_version_from_str_dev_part(message, version, dev) -> None:
+    v: Version = Version.from_string(version)
+    assert v.dev == dev
+
+@parameterize(",".join(["message", "version", "post"]), _SUB_TESTS_VERSION_FROM_STR_POST)
+def test_create_version_from_str_post_part(message, version, post) -> None:
+    v: Version = Version.from_string(version)
+    assert v.post == post
+
+@parameterize(",".join(["message", "version", "local"]), _SUB_TESTS_VERSION_FROM_STR_LOCAL)
+def test_create_version_from_str_local_part(message, version, local) -> None:
+    v: Version = Version.from_string(version)
+    assert v.local == local
+
+@parameterize(",".join(["message", "version"]), _SUB_TESTS_VERSION_PARSE_SUCCESS)
+def test_create_version_from_str_can_parse_success(message, version) -> None:
+    result: bool = Version.can_parse_to_version(version)
+    assert result is True
+
+@parameterize(",".join(["message", "version"]), _SUB_TESTS_VERSION_PARSE_FAIL)
+def test_create_version_from_str_can_parse_fail(message, version) -> None:
+    result: bool = Version.can_parse_to_version(version)
+    assert result is False
+
+@parameterize(",".join(["message", "version"]), _SUB_TESTS_VERSION_PARSE_FAIL)
+def test_create_version_from_str_parse_raises(message, version) -> None:
+    with assert_raises(VersionParserError):
+        Version.from_string(version)
+
+def test_version_major() -> None:
+    v = Version(release_tuple=(1, 2, 3))
+    assert v.major == 1
+
+def test_version_minor() -> None:
+    v = Version(release_tuple=(1, 2, 3))
+    assert v.minor == 2
+
+def test_version_micro() -> None:
+    v = Version(release_tuple=(1, 2, 3))
+    assert v.micro == 3
+
+def test_version_major_unset() -> None:
+    v = Version(release_tuple=tuple())
+    assert v.major == 0
+
+def test_version_minor_unset() -> None:
+    v = Version(release_tuple=(1,))
+    assert v.minor == 0
+
+def test_version_micro_unset() -> None:
+    v = Version(release_tuple=(1, 2))
+    assert v.micro == 0
+
+def test_version_is_no_pre_release() -> None:
+    v = Version(release_tuple=(1, 2, 3))
+    _assure_pre_matches(v, False, False, False, False, False)
+    assert (v.is_post_release or v.is_local_version) is False
+
+def test_version_is_alpha_true() -> None:
+    v = _create_version(as_alpha=True)
+    _assure_pre_matches(v, True, False, False, True, False)
+    assert (v.is_post_release or v.is_local_version) is False
+
+def test_version_is_beta_true() -> None:
+    v = _create_version(as_beta=True)
+    _assure_pre_matches(v, False, True, False, True, False)
+    assert (v.is_post_release or v.is_local_version) is False
+
+def test_version_is_rc_true() -> None:
+    v = _create_version(as_rc=True)
+    _assure_pre_matches(v, False, False, True, True, False)
+    assert (v.is_post_release or v.is_local_version) is False
+
+def test_version_is_dev_true() -> None:
+    v = _create_version(as_dev=True)
+    _assure_pre_matches(v, False, False, False, True, True)
+    assert (v.is_post_release or v.is_local_version) is False
+
+def test_version_is_post_true() -> None:
+    v = _create_version(as_post=True)
+    _assure_pre_matches(v, False, False, False, False, False)
+    assert v.is_post_release is True
+    assert (v.is_post_release and v.is_local_version) is False
+
+def test_version_is_local_true() -> None:
+    v = _create_version(as_local=True)
+    _assure_pre_matches(v, False, False, False, False, False)
+    assert v.is_local_version is True
+    assert (v.is_post_release and v.is_local_version) is False
+
+def _create_version(
+    *,
+    as_alpha: bool = False,
+    as_beta: bool = False,
+    as_rc: bool = False,
+    as_dev: bool = False,
+    as_post: bool = False,
+    as_local: bool = False,
+) -> Version:
+    epoch = 1
+    release = (2, 3, 4)
+    dev = None if not as_dev else ("dev", 5)
+    post = None if not as_post else ("post", 6)
+    local = None if not as_local else "as.local7"
+
+    items = int(as_alpha) + int(as_beta) + int(as_rc)
+    if items > 1:
+        raise ValueError("Only one pre-release identifier can be set")
+    pre = None
+    if as_alpha:
+        pre = ("a", 8)
+    elif as_beta:
+        pre = ("b", 9)
+    elif as_rc:
+        pre = ("rc", 10)
+
+    return Version(epoch, release, pre, post, dev, local)
+
+def _assure_pre_matches(
+    version: Version, is_alpha, is_beta, is_rc, is_pre, is_dev
+) -> None:
+    assert version.is_alpha == is_alpha, "Alpha part matches"
+    assert version.is_beta == is_beta, "Beta part matches"
+    assert version.is_release_candidate == is_rc, "RC part matches"
+    assert version.is_pre_release == is_pre, "pre-release matches"
+    assert version.is_development_version == is_dev, "Development matches"
+
+
+import unittest
 
 
 @final
-class VersionPropertiesTest(unittest.TestCase):
-    def test_version_major(self) -> None:
-        v = Version(release_tuple=(1, 2, 3))
-        self.assertEqual(v.major, 1)
-
-    def test_version_minor(self) -> None:
-        v = Version(release_tuple=(1, 2, 3))
-        self.assertEqual(v.minor, 2)
-
-    def test_version_micro(self) -> None:
-        v = Version(release_tuple=(1, 2, 3))
-        self.assertEqual(v.micro, 3)
-
-    def test_version_major_unset(self) -> None:
-        v = Version(release_tuple=tuple())
-        self.assertEqual(v.major, 0)
-
-    def test_version_minor_unset(self) -> None:
-        v = Version(release_tuple=(1,))
-        self.assertEqual(v.minor, 0)
-
-    def test_version_micro_unset(self) -> None:
-        v = Version(release_tuple=(1, 2))
-        self.assertEqual(v.micro, 0)
-
-    def test_version_is_no_pre_release(self) -> None:
-        v = Version(release_tuple=(1, 2, 3))
-        self._assure_pre_matches(v, False, False, False, False, False)
-        self.assertFalse(v.is_post_release or v.is_local_version)
-
-    def test_version_is_alpha_true(self) -> None:
-        v = self._create_version(as_alpha=True)
-        self._assure_pre_matches(v, True, False, False, True, False)
-        self.assertFalse(v.is_post_release or v.is_local_version)
-
-    def test_version_is_beta_true(self) -> None:
-        v = self._create_version(as_beta=True)
-        self._assure_pre_matches(v, False, True, False, True, False)
-        self.assertFalse(v.is_post_release or v.is_local_version)
-
-    def test_version_is_rc_true(self) -> None:
-        v = self._create_version(as_rc=True)
-        self._assure_pre_matches(v, False, False, True, True, False)
-        self.assertFalse(v.is_post_release or v.is_local_version)
-
-    def test_version_is_dev_true(self) -> None:
-        v = self._create_version(as_dev=True)
-        self._assure_pre_matches(v, False, False, False, True, True)
-        self.assertFalse(v.is_post_release or v.is_local_version)
-
-    def test_version_is_post_true(self) -> None:
-        v = self._create_version(as_post=True)
-        self._assure_pre_matches(v, False, False, False, False, False)
-        self.assertTrue(v.is_post_release)
-        self.assertFalse(v.is_post_release and v.is_local_version)
-
-    def test_version_is_local_true(self) -> None:
-        v = self._create_version(as_local=True)
-        self._assure_pre_matches(v, False, False, False, False, False)
-        self.assertTrue(v.is_local_version)
-        self.assertFalse(v.is_post_release and v.is_local_version)
-
-    def _create_version(
-        self,
-        *,
-        as_alpha: bool = False,
-        as_beta: bool = False,
-        as_rc: bool = False,
-        as_dev: bool = False,
-        as_post: bool = False,
-        as_local: bool = False,
-    ) -> Version:
-        epoch = 1
-        release = (2, 3, 4)
-        dev = None if not as_dev else ("dev", 5)
-        post = None if not as_post else ("post", 6)
-        local = None if not as_local else "as.local7"
-
-        items = int(as_alpha) + int(as_beta) + int(as_rc)
-        if items > 1:
-            raise ValueError("Only one pre-release identifier can be set")
-        pre = None
-        if as_alpha:
-            pre = ("a", 8)
-        elif as_beta:
-            pre = ("b", 9)
-        elif as_rc:
-            pre = ("rc", 10)
-
-        return Version(epoch, release, pre, post, dev, local)
-
-    def _assure_pre_matches(
-        self, version: Version, is_alpha, is_beta, is_rc, is_pre, is_dev
-    ) -> None:
-        self.assertEqual(version.is_alpha, is_alpha)
-        self.assertEqual(version.is_beta, is_beta)
-        self.assertEqual(version.is_release_candidate, is_rc)
-        self.assertEqual(version.is_pre_release, is_pre)
-        self.assertEqual(version.is_development_version, is_dev)
+class CreateVersionTest(unittest.TestCase):
+    pass  # TODO implement
 
 
 @final
 class VersionOrderingTest(unittest.TestCase):
     pass  # TODO implement
```

### Comparing `pdm-bump-0.7.0a1/PKG-INFO` & `pdm_bump-0.7.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 Metadata-Version: 2.1
 Name: pdm-bump
-Version: 0.7.0a1
+Version: 0.7.1
 Summary: A plugin for PDM providing the ability to modify the version according to PEP440
+Home-page: https://github.com/carstencodes/pdm-bump
+Author-Email: Carsten Igel <cig@bite-that-bit.de>
 License: MIT
-Author-email: Carsten Igel <cig@bite-that-bit.de>
+Project-URL: Homepage, https://github.com/carstencodes/pdm-bump
 Requires-Python: >=3.9
-Project-URL: homepage, https://github.com/carstencodes/pdm-bump
+Requires-Dist: pdm>=2.00
+Requires-Dist: annotated-types>=0.2.0
+Requires-Dist: typing-extensions>=4; python_version <= "3.9"
+Requires-Dist: tomlkit>=0.11.6
+Requires-Dist: tomli>=2.0.1; python_version <= "3.10"
+Requires-Dist: pyproject-metadata>=0.6.1
+Requires-Dist: tomli-w>=1.0.0
 Description-Content-Type: text/markdown
 
 # pdm-bump
 
 ![PyPI](https://img.shields.io/pypi/v/pdm-bump?logo=python&logoColor=%23cccccc)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 
@@ -68,8 +76,7 @@
 1. Tests: To run the tests for your current checks, run `pdm run pytest`.
 2. tox: If you are using `pyenv` you can use `pdm run tox` to run the tests for all supported Python versions.
 3. Code Style: You can use `pdm check-style` to check code format.
 4. Format: You can use `pdm format` to format your code.
 5. Commit messages: You can run `pdm check-commits` to run `gitlint` on your commit messages.
 
 Before opening a Pull Request make sure that the quality gates are passed.
-
```

