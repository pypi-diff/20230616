# Comparing `tmp/tldr_man-1.1.1.tar.gz` & `tmp/tldr_man-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tldr_man-1.1.1.tar", max compression
+gzip compressed data, was "tldr_man-1.2.0.tar", max compression
```

## Comparing `tldr_man-1.1.1.tar` & `tldr_man-1.2.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0    11357 2022-07-17 04:30:22.662713 tldr_man-1.1.1/LICENSE
--rw-r--r--   0        0        0     3417 2022-07-29 21:47:31.099058 tldr_man-1.1.1/README.md
--rwxr-xr-x   0        0        0      952 2022-07-29 02:18:33.311697 tldr_man-1.1.1/generate_completions.sh
--rw-r--r--   0        0        0     1549 2023-03-21 00:58:33.517016 tldr_man-1.1.1/pyproject.toml
--rw-r--r--   0        0        0       28 2022-07-29 03:20:39.631247 tldr_man-1.1.1/src/tldr_man/__init__.py
--rw-r--r--   0        0        0       37 2022-07-29 03:10:10.456815 tldr_man-1.1.1/src/tldr_man/__main__.py
--rw-r--r--   0        0        0     2503 2023-03-10 03:58:37.773707 tldr_man-1.1.1/src/tldr_man/languages.py
--rwxr-xr-x   0        0        0     6877 2023-03-14 00:15:45.094169 tldr_man-1.1.1/src/tldr_man/main.py
--rw-r--r--   0        0        0    10579 2023-03-21 00:57:37.014396 tldr_man-1.1.1/src/tldr_man/pages.py
--rw-r--r--   0        0        0     1332 2023-03-10 03:58:37.775022 tldr_man-1.1.1/src/tldr_man/util.py
--rw-r--r--   0        0        0     5013 1970-01-01 00:00:00.000000 tldr_man-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-07-17 04:30:22.662713 tldr_man-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3448 2023-06-16 06:22:32.619707 tldr_man-1.2.0/README.md
+-rwxr-xr-x   0        0        0      953 2023-06-16 07:23:05.228692 tldr_man-1.2.0/generate_completions.sh
+-rw-r--r--   0        0        0     1502 2023-06-16 07:25:33.049272 tldr_man-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       28 2022-07-29 03:20:39.631247 tldr_man-1.2.0/src/tldr_man/__init__.py
+-rw-r--r--   0        0        0       37 2022-07-29 03:10:10.456815 tldr_man-1.2.0/src/tldr_man/__main__.py
+-rw-r--r--   0        0        0     3347 2023-06-16 00:38:00.476437 tldr_man-1.2.0/src/tldr_man/languages.py
+-rwxr-xr-x   0        0        0     5931 2023-06-16 06:19:30.171795 tldr_man-1.2.0/src/tldr_man/main.py
+-rw-r--r--   0        0        0    11806 2023-06-16 07:24:14.611691 tldr_man-1.2.0/src/tldr_man/pages.py
+-rw-r--r--   0        0        0     1614 2023-06-16 00:35:28.327932 tldr_man-1.2.0/src/tldr_man/platforms.py
+-rw-r--r--   0        0        0     1812 2023-06-16 04:54:01.856938 tldr_man-1.2.0/src/tldr_man/shell_completion.py
+-rw-r--r--   0        0        0     1359 2023-06-16 04:55:12.255927 tldr_man-1.2.0/src/tldr_man/util.py
+-rw-r--r--   0        0        0     5045 1970-01-01 00:00:00.000000 tldr_man-1.2.0/PKG-INFO
```

### Comparing `tldr_man-1.1.1/LICENSE` & `tldr_man-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tldr_man-1.1.1/README.md` & `tldr_man-1.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 <div>
-    <h1 align="center">tldr-man-client</h1>
+    <h1 align="center">tldr-man</h1>
     <h5 align="center">A tldr-pages client that works just like <code>man</code></h5>
 </div>
 
-`tldr-man-client` is a command-line client for [tldr-pages][tldr-pages],
+`tldr-man` is a command-line client for [tldr-pages][tldr-pages],
 a collection of community-maintained help pages for command-line tools.
 It differs from other clients because it displays its pages as `man` pages.
 
 This client is also able to integrate with the `man` command to fall back to displaying a tldr-page for a command when
 no manpage exists.
 
 Features:
 - Fully abides by the [tldr-pages client specification][client-spec].
 - Supports all page languages, not just English pages.
 - Displays tldr-pages in the same style as manpages.
 - Integrates with `man` to provide a fallback for missing manpages.
 - Supports rendering markdown formatted tldr-pages with `--render`.
 - Local cache abides by the [XDG base directory specification][xdg].
+- Supports shell completion for `bash`, `zsh`, and `fish` shells.
 - And much more!
 
 
 ## Installation
 
 ### With Homebrew
 
-Install `tldr-man-client` with [Homebrew](https://brew.sh):
+Install `tldr-man` with [Homebrew](https://brew.sh):
 
 ```shell
 brew install superatomic/tap/tldr-man
 ```
 
 ### With Pip
 
-Install `tldr-man-client` with pip (version 3.10+):
+Install `tldr-man` with pip (version 3.10+):
 
 ```shell
 pip install tldr-man
 ```
 
-`tldr-man-client` additionally depends on [`pandoc`](https://pandoc.org/installing.html) being installed.
+`tldr-man` additionally depends on [`pandoc`](https://pandoc.org/installing.html) being installed.
 
 After installation, you can view a tldr-page with the `tldr` command.
 
 
 ## Usage
 
 **Display a tldr-page for a command:**
```

### Comparing `tldr_man-1.1.1/generate_completions.sh` & `tldr_man-1.2.0/generate_completions.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env bash
 
-# Copyright 2022 Ethan Kinnear
+# Copyright 2023 Olivia Kinnear
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `tldr_man-1.1.1/pyproject.toml` & `tldr_man-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "tldr-man"
-version = "1.1.1"
+version = "1.2.0"
 description = "Command-line TLDR client that displays tldr-pages as manpages"
 license = 'Apache-2.0'
 readme = "README.md"
-authors = ["Ethan Kinnear <contact@superatomic.dev>"]
+authors = ["Olivia Kinnear <contact@superatomic.dev>"]
 homepage = 'https://tldr-man.superatomic.dev/'
 repository = 'https://github.com/superatomic/tldr-man-client'
 documentation = 'https://github.com/superatomic/tldr-man-client#readme'
 keywords = ['tldr', 'tldr-pages', 'man', 'manpage', 'tldr-client']
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
@@ -33,17 +33,14 @@
 [tool.poetry.dependencies]
 python = "^3.10.4"
 click = "^8.1.3"
 click-help-colors = "^0.9.1"
 xdg = "^5.1.1"
 requests = "^2.28.1"
 
-[tool.poetry.dev-dependencies]
-pytest = "^5.2"
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 tldr = "tldr_man:cli"
 tldr-man = "tldr_man:cli"
```

### Comparing `tldr_man-1.1.1/src/tldr_man/languages.py` & `tldr_man-1.2.0/src/tldr_man/languages.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,52 @@
-# Copyright 2022 Ethan Kinnear
+# Copyright 2023 Olivia Kinnear
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Handle tldr-page languages."""
+"""Handle languages for the client."""
 
 from os import getenv
 from collections.abc import Iterator
 
-from tldr_man.pages import TLDR_CACHE_HOME
+from click import Context
+
+from tldr_man.pages import TLDR_CACHE_HOME, language_directory_to_code
+from tldr_man.util import exit_with
 
 
 def all_languages() -> Iterator[str]:
+    """Returns an iterator of all languages directory names."""
+    return map(get_language_directory, all_language_codes())
+
+
+def all_language_codes() -> Iterator[str]:
+    """Returns an iterator of all language codes, based on all language directories."""
     return (
-        get_language_directory(pages_dir.name.removeprefix('pages').lstrip('.') or 'en')
+        language_directory_to_code(pages_dir)
         for pages_dir in TLDR_CACHE_HOME.iterdir()
         if pages_dir.is_dir()
     )
 
 
-def get_languages() -> Iterator[str]:
+def get_environment_languages() -> Iterator[str]:
     """
-    Returns a list of the user's preferred languages, inferred by the environment variables LANG and LANGUAGE.
+    Returns an iterator of the user's preferred languages,
+    inferred from the environment variables `LANG`, `LANGUAGE`, and `TLDR_LANGUAGE`.
 
-    See https://github.com/tldr-pages/tldr/blob/main/CLIENT-SPECIFICATION.md#language for details.
+    See https://github.com/tldr-pages/tldr/blob/main/CLIENT-SPECIFICATION.md#language for more details.
     """
 
     languages: list[str] = []
 
     env_lang = getenv('LANG')
     env_language = getenv('LANGUAGE')
     env_tldr_language = getenv('TLDR_LANGUAGE')
@@ -52,20 +62,20 @@
 
     languages.append('en')
 
     # Remove country code from the language codes
     return map(get_language_directory, languages)
 
 
-def _language_code_as_parts(language_code: str) -> (str, str):
+def _language_code_as_parts(language_code: str) -> tuple[str, str]:
     """Removes country codes from language codes and preforms data normalization."""
-    code = language_code.split('.')[0].split('_', 1)
+    language, is_region, region = language_code.split('.')[0].partition('_')
 
-    language = code[0].strip().lower()
-    region = code[1].strip().upper() if len(code) >= 2 else language.upper()
+    language = language.strip().lower()
+    region = region.strip().upper() if is_region else language.upper()
 
     return language, region
 
 
 def get_language_directory(language_code: str) -> str:
     """Get the name of the directory for a language code."""
     language, region = _language_code_as_parts(language_code)
@@ -73,7 +83,20 @@
         return 'pages'
     else:
         full_locale = f'pages.{language}_{region}'
         if (TLDR_CACHE_HOME / full_locale).is_dir():
             return full_locale
         else:
             return f'pages.{language}'
+
+
+def get_locales(ctx: Context) -> list[str]:
+    """Return an ordered list of the languages that the user specifies."""
+    language = ctx.params.get('language')
+    if language is not None:
+        page_locale = get_language_directory(language)
+        if page_locale not in all_languages():
+            exit_with(f"Unrecognized locale: {language}")
+        else:
+            return [page_locale]
+    else:
+        return list(get_environment_languages())
```

### Comparing `tldr_man-1.1.1/src/tldr_man/main.py` & `tldr_man-1.2.0/src/tldr_man/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,61 @@
 #!/usr/bin/env python3
 
-# Copyright 2022 Ethan Kinnear
+# Copyright 2023 Olivia Kinnear
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-tldr-man-client: Command-line TLDR client that displays tldr-pages as manpages.
+tldr-man: Command-line TLDR client that displays tldr-pages as manpages.
 
 Depends on pandoc (and man!). Install `pandoc` from https://pandoc.org/installing.html.
 
 Run `tldr --help` for more information,
 or visit the project repository at https://github.com/superatomic/tldr-man-client.
 """
 
-from importlib import metadata
-__version__ = metadata.version('tldr-man')
-__author__ = "Ethan Kinnear <contact@superatomic.dev>"
+__author__ = "Olivia Kinnear <contact@superatomic.dev>"
 
-import sys
 from pathlib import Path
 from contextlib import suppress
 from os import remove
 from functools import wraps
-from typing import Optional
 
 import click
+from click import Context, command, argument, option, version_option, help_option, pass_context
 from click_help_colors import HelpColorsCommand
 
-from tldr_man import languages, pages
-from tldr_man.util import unique, mkstemp_path, exit_with
+from tldr_man import pages
+from tldr_man.shell_completion import page_shell_complete, language_shell_complete
+from tldr_man.languages import get_locales
+from tldr_man.platforms import get_page_sections, TLDR_PLATFORMS
+from tldr_man.util import unique, mkstemp_path
 
 
-TLDR_COMMAND_NAME = 'tldr'
-
-TLDR_PLATFORMS = 'android linux macos osx sunos windows'.split()
-
-
-def click_standalone_subcommand(func):
+def standalone_subcommand(func):
     """Function decorator to reduce boilerplate code at the start and end of all subcommand callback functions."""
     @wraps(func)
-    def wrapper(ctx, param, value):
+    def wrapper(ctx: Context, _param, value):
         if not value or ctx.resilient_parsing:
             return
 
         exited_with_error = False
         # noinspection PyBroadException
         try:
-            func(ctx, param, value)
+            return func(ctx, value) if value is not True else func(ctx)
         except Exception:
             from traceback import format_exc
             from sys import stderr
 
             print(format_exc(), file=stderr)
             exited_with_error = True  # Don't call the `ctx.exit()` in the `finally` block
             ctx.exit(1)
@@ -70,152 +65,112 @@
             ctx.exit(err.code)
         finally:
             if not exited_with_error:
                 ctx.exit()
 
     return wrapper
 
+def require_tldr_cache(func):
+    """
+    Function decorator to mark that a subcommand requires the tldr-page cache to exist.
+    Additionally, maps `ctx` into the valid locales and platforms.
+
+    func(locales, platforms, ...) --> func(ctx, ...)
+    """
+    @wraps(func)
+    def wrapper(ctx: Context, *args, **kwargs):
+        pages.verify_tldr_cache_exists()
+
+        locales: list[str] = get_locales(ctx)
+        page_sections: list[str] = get_page_sections(ctx)
+
+        return func(locales, page_sections, *args, **kwargs)
+
+    return wrapper
 
-@click_standalone_subcommand
-def subcommand_update(_ctx, _param, _value):
+
+@standalone_subcommand
+def subcommand_update(_ctx):
     pages.update_cache()
 
 
-@click_standalone_subcommand
-def subcommand_render(_ctx, _param, value: Path):
+@standalone_subcommand
+def subcommand_render(_ctx, value: Path):
     page_to_render = value.read_text()
     rendered_page = pages.render_manpage(page_to_render)
 
     try:
         path = mkstemp_path('tldr-man', text=True)
         path.write_text(rendered_page)
         pages.display_page(path)
     finally:
         with suppress(NameError, FileNotFoundError):
             # noinspection PyUnboundLocalVariable
             remove(path)
 
 
-@click_standalone_subcommand
-def subcommand_list(ctx, _param, _value):
-    pages.verify_tldr_cache_exists()
-
-    locales = get_locales(ctx)
-    page_sections = get_page_sections(ctx)
-
+@standalone_subcommand
+@require_tldr_cache
+def subcommand_list(locales, page_sections):
     print('\n'.join(unique(
         page.stem
         for section in pages.get_dir_search_order(locales, page_sections)
         for page in section.iterdir()
         if page.is_file()
     )))
 
 
-@click_standalone_subcommand
-def subcommand_manpath(ctx, _param, _value):
-    pages.verify_tldr_cache_exists()
-
-    locales = get_locales(ctx)
-    page_sections = get_page_sections(ctx)
-
-    print(':'.join(unique(str(x.parent) for x in pages.get_dir_search_order(locales, page_sections))))
-
-
-@click_standalone_subcommand
-def subcommand_version(_ctx, _param, _value):
-    print(TLDR_COMMAND_NAME, __version__)
-
-
-@click.command(cls=HelpColorsCommand, help_headers_color='yellow', help_options_color='green')
-@click.argument('page', nargs=-1, required=True)
-@click.option('-p', '--platform',
-              type=click.Choice(TLDR_PLATFORMS),
-              is_eager=True,
-              help='Override the preferred platform')
-@click.option('-L', '--language',
-              is_eager=True,
-              help='Specify a preferred language')
-@click.option('-u', '--update',
-              callback=subcommand_update, expose_value=False,
-              is_flag=True,
-              is_eager=True,
-              help='Update the tldr-pages cache')
-@click.option('-r', '--render',
-              callback=subcommand_render, expose_value=False,
-              type=click.Path(exists=True, dir_okay=False, path_type=Path), nargs=1,
-              is_eager=True,
-              help='Render a page locally')
-@click.option('-l', '--list',
-              callback=subcommand_list, expose_value=False,
-              is_flag=True,
-              help='List all the pages for the current platform')
-@click.option('--manpath',
-              callback=subcommand_manpath, expose_value=False,
-              is_flag=True,
-              help='Print the paths to the tldr manpages')
-@click.option('-v', '-V', '--version',
-              callback=subcommand_version, expose_value=False,
-              is_flag=True,
-              is_eager=True,
-              help='Display the version of the client')
-@click.help_option('-h', '--help')
-@click.pass_context
-def cli(ctx, page: list[str], **_):
+@standalone_subcommand
+@require_tldr_cache
+def subcommand_manpath(locales, page_sections):
+    print(':'.join(unique(str(man_dir.parent) for man_dir in pages.get_dir_search_order(locales, page_sections))))
+
+
+@command(cls=HelpColorsCommand, help_headers_color='yellow', help_options_color='green', no_args_is_help=True)
+@argument('page', nargs=-1, required=True, shell_complete=page_shell_complete)
+@option('-p', '--platform',
+        metavar='PLATFORM',
+        type=click.Choice(TLDR_PLATFORMS),
+        is_eager=True,
+        help='Override the preferred platform')
+@option('-L', '--language',
+        metavar='LANGUAGE',
+        is_eager=True,
+        shell_complete=language_shell_complete,
+        help='Specify a preferred language')
+@option('-u', '--update',
+        callback=subcommand_update, expose_value=False,
+        is_flag=True,
+        is_eager=True,
+        help='Update the tldr-pages cache')
+@option('-r', '--render',
+        callback=subcommand_render, expose_value=False,
+        type=click.Path(exists=True, dir_okay=False, path_type=Path), nargs=1,
+        is_eager=True,
+        help='Render a page locally')
+@option('-l', '--list',
+        callback=subcommand_list, expose_value=False,
+        is_flag=True,
+        help='List all the pages for the current platform')
+@option('-M', '--manpath',
+        callback=subcommand_manpath, expose_value=False,
+        is_flag=True,
+        help='Print the paths to the tldr manpages')
+@version_option(None, '-v', '-V', '--version',
+                message="%(prog)s %(version)s",
+                help='Display the version and exit')
+@help_option('-h', '--help',
+             help='Show this message and exit')
+@pass_context
+@require_tldr_cache
+def cli(locales, page_sections, page: list[str], **_):
     """TLDR client that displays tldr-pages as manpages"""
-
-    pages.verify_tldr_cache_exists()
-
-    locales = get_locales(ctx)
-    page_sections = get_page_sections(ctx)
-
     page_name = '-'.join(page).strip().lower()
 
-    page = pages.find_page(page_name, locales, page_sections)
-
-    if page is not None:
-        pages.display_page(page)
-
+    page_path = pages.find_page(page_name, locales, page_sections)
 
-def get_locales(ctx) -> list[str]:
-    language = ctx.params.get('language')
-    if language is not None:
-        page_locale = languages.get_language_directory(language)
-        if page_locale not in languages.all_languages():
-            exit_with(f"Unrecognized locale: {language}")
-        else:
-            return [page_locale]
-    else:
-        return list(languages.get_languages())
-
-
-def get_page_sections(ctx) -> list[str]:
-    page_sections = ['common']
-
-    current_platform = get_current_platform()
-    custom_platform = ctx.params.get('platform')
-
-    if current_platform:
-        page_sections.insert(0, current_platform)
-
-    if custom_platform:
-        page_sections.insert(0, custom_platform.replace('macos', 'osx'))
-
-    return page_sections
-
-
-def get_current_platform() -> Optional[str]:
-    """Get the correct tldr platform directory name from `sys.platform`."""
-    match sys.platform:
-        case 'darwin':
-            return 'osx'
-        case 'linux':
-            return 'linux'
-        case 'win32' | 'cygwin' | 'msys':
-            return 'windows'
-        case 'sunos5':
-            return 'sunos'
-        case _:
-            return None
+    if page_path is not None:
+        pages.display_page(page_path)
 
 
 if __name__ == '__main__':
     cli()
```

### Comparing `tldr_man-1.1.1/src/tldr_man/pages.py` & `tldr_man-1.2.0/src/tldr_man/pages.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Ethan Kinnear
+# Copyright 2023 Olivia Kinnear
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -22,15 +22,15 @@
 from os import remove, makedirs
 from shutil import rmtree, move
 from subprocess import run, PIPE, DEVNULL
 from typing import Optional
 from collections.abc import Iterable
 
 import requests
-from click import secho, progressbar, style
+from click import secho, progressbar, style, echo
 from xdg import XDG_CACHE_HOME
 
 from tldr_man.util import mkstemp_path, mkdtemp_path, eprint, exit_with
 
 TLDR_CACHE_DIR_NAME = 'tldr-man'
 
 TLDR_ZIP_ARCHIVE_URL = "https://tldr.sh/assets/tldr.zip"
@@ -105,14 +105,16 @@
     """Updates the tldr-pages manpage cache."""
 
     if not pandoc_exists():
         exit_with(PANDOC_MISSING_MESSAGE, exitcode=127)
 
     secho('Updating tldr-pages cache...', fg='cyan')
 
+    created, updated, unchanged = 0, 0, 0
+
     try:
         # Create a temporary file for the tldr-pages zip archive to generate manpages from.
         tldr_zip_archive = mkstemp_path('tldr.zip')
         download_tldr_zip_archive(tldr_zip_archive)
 
         # Create the cache directory that will be copied to `~/.cache/tldr-man`.
         tldr_temp_dir = mkdtemp_path('tldr-man')
@@ -125,28 +127,34 @@
             raise
 
         # Iterate through each language and section in the zip file.
         for language_dir in tldr_zip_path.iterdir():
             if not language_dir.is_dir():
                 continue
             for sections_dir in language_dir.iterdir():
-
                 # Get the full path to the directory where all manpages for this language and section will be extracted.
                 res_dir = tldr_temp_dir / language_dir.name / sections_dir.name / ('man' + TLDR_MANPAGE_SECTION)
                 res_dir.mkdir(parents=True, exist_ok=True)  # Create the directories if they don't exist.
 
+                # Get the directory where the old versions of the manpages are located,
+                # to compare it with the new versions that are generated:
+                original_dir = (
+                    TLDR_CACHE_HOME / language_dir.name / sections_dir.name / ('man' + TLDR_MANPAGE_SECTION)
+                    if TLDR_CACHE_HOME.exists() else None
+                )
+
                 # Create the label for the progress bars that are shown.
-                progressbar_label = (style(f'{language_dir.name:11s}', fg='blue')
+                progressbar_label = (style(f"{language_directory_to_code(language_dir):5s}", fg='blue')
                                      + ' / '
                                      + style(f'{sections_dir.name:7s}', fg='blue'))
 
                 # `render_manpage()` takes a significant amount of time to run.
                 # Due to the number of pages that need to be rendered,
                 # this function is invoked simultaneously using threads.
-                def to_manpage(tldr_page: zipfile.Path) -> (str, str):
+                def to_manpage(tldr_page: zipfile.Path) -> tuple[str, str]:
                     """Convert a tldr-page into a manpage"""
                     rendered_manpage = render_manpage(tldr_page.read_text())
                     manpage_filename = tldr_page.name.removesuffix('.md') + '.' + TLDR_MANPAGE_SECTION
                     # Return the filename to save the manpage to along with the rendered manpage itself.
                     return manpage_filename, rendered_manpage
 
                 # Get a list of all tldr-pages in the current language and section.
@@ -161,43 +169,55 @@
                         # As each manpage finishes rendering, save their contents to the destination file.
                         # Note: This operation must be done here and not within a thread! `Path.write_text` and
                         #       `shutil.rmtree` (called as part of cleanup) are not thread-safe if they happen at the
                         #       same time. (This would occur during a keyboard interrupt)
                         for filename, manpage in fut:
                             res_file = res_dir / filename
                             res_file.write_text(manpage)
+
+                            # Log whether the file was created, updated, or unchanged:
+                            if original_dir is None or not (original_file := original_dir / filename).exists():
+                                created += 1
+                            elif original_file.read_text() != manpage:
+                                updated += 1
+                            else:
+                                unchanged += 1
                     except:
-                        # If an exceptiom occurs, such as a KeyboardInterrupt or an actual Exception,
+                        # If an exception occurs, such as a KeyboardInterrupt or an actual Exception,
                         # shutdown the pool *without* waiting for any remaining futures to finish. This will prevent the
                         # program from having a significant delay when it exits prematurely.
                         # This is not a `finally` clause because the normal `pool.shutdown` behavior implemented by
                         # `Executor.__exit__` is correct when no error occurs.
                         pool.shutdown(wait=False, cancel_futures=True)
                         raise
 
         # Now that the updated cache has been generated, remove the old cache, make sure the parent directory exists,
         # and move the new cache into the correct directory from the temporary directory.
 
         with suppress(FileNotFoundError):
             rmtree(TLDR_CACHE_HOME)
 
         makedirs(TLDR_CACHE_HOME.parent, exist_ok=True)
-
         move(tldr_temp_dir, TLDR_CACHE_HOME)
+
     finally:
         # Clean up any temporary files that aren't gone.
-
         with suppress(NameError, FileNotFoundError):
             # noinspection PyUnboundLocalVariable
             remove(tldr_zip_archive)
         with suppress(NameError, FileNotFoundError):
             # noinspection PyUnboundLocalVariable
             rmtree(tldr_temp_dir)
 
-    secho('Done!', fg='green', bold=True)
+    # Display the details for the cache update:
+    echo(', '.join([
+        style(f'{created} Added', fg='green', bold=True),
+        style(f'{updated} Updated', fg='blue', bold=True),
+        style(f'{unchanged} Unchanged', bold=True),
+    ]))
 
 
 def render_manpage(tldr_page: str) -> str:
     """
     Render a manpage from a markdown formatted tldr-page.
 
     Exits with an error message if `pandoc` is not installed.
@@ -272,7 +292,11 @@
 
 def get_dir_search_order(locales: Iterable[str], page_sections: Iterable[str]) -> Iterable[Path]:
     return (
         TLDR_CACHE_HOME / locale / section / ('man' + TLDR_MANPAGE_SECTION)
         for locale in locales
         for section in page_sections
     )
+
+
+def language_directory_to_code(language_dir: Path):
+    return language_dir.name.removeprefix('pages').lstrip('.') or 'en'
```

### Comparing `tldr_man-1.1.1/src/tldr_man/util.py` & `tldr_man-1.2.0/src/tldr_man/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Ethan Kinnear
+# Copyright 2023 Olivia Kinnear
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 # http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,20 +14,20 @@
 
 """Various utility functions."""
 
 from sys import exit
 from pathlib import Path
 from tempfile import mkstemp, mkdtemp
 from typing import TypeVar, NoReturn
-from collections.abc import Iterable, Iterator
+from collections.abc import Iterable, Iterator, Hashable
 
 from click import secho
 
 
-T = TypeVar('T')
+T = TypeVar('T', bound=Hashable)
 
 def unique(items: Iterable[T]) -> Iterator[T]:
     seen = set()
     for item in items:
         if item not in seen:
             seen.add(item)
             yield item
```

### Comparing `tldr_man-1.1.1/PKG-INFO` & `tldr_man-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: tldr-man
-Version: 1.1.1
+Version: 1.2.0
 Summary: Command-line TLDR client that displays tldr-pages as manpages
 Home-page: https://tldr-man.superatomic.dev/
 License: Apache-2.0
 Keywords: tldr,tldr-pages,man,manpage,tldr-client
-Author: Ethan Kinnear
+Author: Olivia Kinnear
 Author-email: contact@superatomic.dev
 Requires-Python: >=3.10.4,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
@@ -31,54 +31,55 @@
 Project-URL: Bug Tracker, https://github.com/superatomic/tldr-man-client/issues
 Project-URL: Documentation, https://github.com/superatomic/tldr-man-client#readme
 Project-URL: Repository, https://github.com/superatomic/tldr-man-client
 Project-URL: Say Thanks!, https://saythanks.io/to/superatomic
 Description-Content-Type: text/markdown
 
 <div>
-    <h1 align="center">tldr-man-client</h1>
+    <h1 align="center">tldr-man</h1>
     <h5 align="center">A tldr-pages client that works just like <code>man</code></h5>
 </div>
 
-`tldr-man-client` is a command-line client for [tldr-pages][tldr-pages],
+`tldr-man` is a command-line client for [tldr-pages][tldr-pages],
 a collection of community-maintained help pages for command-line tools.
 It differs from other clients because it displays its pages as `man` pages.
 
 This client is also able to integrate with the `man` command to fall back to displaying a tldr-page for a command when
 no manpage exists.
 
 Features:
 - Fully abides by the [tldr-pages client specification][client-spec].
 - Supports all page languages, not just English pages.
 - Displays tldr-pages in the same style as manpages.
 - Integrates with `man` to provide a fallback for missing manpages.
 - Supports rendering markdown formatted tldr-pages with `--render`.
 - Local cache abides by the [XDG base directory specification][xdg].
+- Supports shell completion for `bash`, `zsh`, and `fish` shells.
 - And much more!
 
 
 ## Installation
 
 ### With Homebrew
 
-Install `tldr-man-client` with [Homebrew](https://brew.sh):
+Install `tldr-man` with [Homebrew](https://brew.sh):
 
 ```shell
 brew install superatomic/tap/tldr-man
 ```
 
 ### With Pip
 
-Install `tldr-man-client` with pip (version 3.10+):
+Install `tldr-man` with pip (version 3.10+):
 
 ```shell
 pip install tldr-man
 ```
 
-`tldr-man-client` additionally depends on [`pandoc`](https://pandoc.org/installing.html) being installed.
+`tldr-man` additionally depends on [`pandoc`](https://pandoc.org/installing.html) being installed.
 
 After installation, you can view a tldr-page with the `tldr` command.
 
 
 ## Usage
 
 **Display a tldr-page for a command:**
```

