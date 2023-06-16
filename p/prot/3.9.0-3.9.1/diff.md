# Comparing `tmp/prot-3.9.0.tar.gz` & `tmp/prot-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prot-3.9.0.tar", last modified: Fri Jun 16 11:49:10 2023, max compression
+gzip compressed data, was "prot-3.9.1.tar", last modified: Fri Jun 16 14:28:29 2023, max compression
```

## Comparing `prot-3.9.0.tar` & `prot-3.9.1.tar`

### file list

```diff
@@ -1,213 +1,213 @@
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.644819 prot-3.9.0/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1069 2023-06-15 09:23:01.000000 prot-3.9.0/LICENSE
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2341 2023-06-16 11:49:10.644819 prot-3.9.0/PKG-INFO
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1444 2023-06-15 09:23:01.000000 prot-3.9.0/README.md
--rw-r--r--   0 u0_a269  (10269) u0_a269  (10269)       57 2023-06-15 09:29:23.000000 prot-3.9.0/pyproject.toml
--rw-------   0 u0_a269  (10269) u0_a269  (10269)       38 2023-06-16 11:49:10.644819 prot-3.9.0/setup.cfg
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1429 2023-06-15 09:23:01.000000 prot-3.9.0/setup.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.580819 prot-3.9.0/src/
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.584819 prot-3.9.0/src/prot/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    48198 2023-06-16 11:24:28.000000 prot-3.9.0/src/prot/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     4568 2023-06-16 11:24:23.000000 prot-3.9.0/src/prot/__main__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)       22 2023-06-16 11:48:00.000000 prot-3.9.0/src/prot/__version__.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.584819 prot-3.9.0/src/prot/bs/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      177 2023-06-16 11:24:23.000000 prot-3.9.0/src/prot/bs/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     5599 2023-06-16 11:24:23.000000 prot-3.9.0/src/prot/bs/bs.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2190 2023-06-16 11:24:23.000000 prot-3.9.0/src/prot/bs/bsMap.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      914 2023-06-16 11:24:23.000000 prot-3.9.0/src/prot/bs/bsPro.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1300 2023-06-16 11:24:23.000000 prot-3.9.0/src/prot/bs/bsSpaz.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    16217 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/code.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.588819 prot-3.9.0/src/prot/color/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      239 2023-06-16 11:24:46.000000 prot-3.9.0/src/prot/color/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2299 2023-06-16 11:24:46.000000 prot-3.9.0/src/prot/color/ansi.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    10558 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/color/ansitowin32.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1916 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/color/initialise.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     5480 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/color/win32.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     6464 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/color/winterm.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.588819 prot-3.9.0/src/prot/pip/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    12222 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/pip/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2354 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/pip/__main__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      797 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/pip/extra.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)       18 2023-06-16 11:46:04.000000 prot-3.9.0/src/prot/pip/packagesList.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.588819 prot-3.9.0/src/prot/progress/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     4882 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/progress/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2789 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/progress/bar.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1372 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/progress/counter.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1380 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/progress/spinner.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.596819 prot-3.9.0/src/prot/prompt/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      872 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/__init__.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.596819 prot-3.9.0/src/prot/prompt/application/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      519 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/application/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    44227 2023-06-16 11:24:49.000000 prot-3.9.0/src/prot/prompt/application/application.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     5050 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/prompt/application/current.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1349 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/application/dummy.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3699 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/application/run_in_terminal.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     5918 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/prompt/auto_suggest.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    70320 2023-06-16 11:24:51.000000 prot-3.9.0/src/prot/prompt/buffer.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3766 2023-06-16 11:24:48.000000 prot-3.9.0/src/prot/prompt/cache.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.596819 prot-3.9.0/src/prot/prompt/clipboard/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      403 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/clipboard/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2488 2023-06-16 11:24:47.000000 prot-3.9.0/src/prot/prompt/clipboard/base.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1076 2023-06-16 11:24:48.000000 prot-3.9.0/src/prot/prompt/clipboard/in_memory.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1147 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/clipboard/pyperclip.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.600819 prot-3.9.0/src/prot/prompt/completion/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      810 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/completion/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    11486 2023-06-16 11:24:48.000000 prot-3.9.0/src/prot/prompt/completion/base.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3831 2023-06-16 11:24:48.000000 prot-3.9.0/src/prot/prompt/completion/filesystem.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     6940 2023-06-16 11:24:48.000000 prot-3.9.0/src/prot/prompt/completion/fuzzy_completer.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3884 2023-06-16 11:24:48.000000 prot-3.9.0/src/prot/prompt/completion/nested.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2931 2023-06-16 11:24:48.000000 prot-3.9.0/src/prot/prompt/completion/word_completer.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.600819 prot-3.9.0/src/prot/prompt/contrib/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/contrib/__init__.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.600819 prot-3.9.0/src/prot/prompt/contrib/completers/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)       36 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/contrib/completers/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2012 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/contrib/completers/system.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.604819 prot-3.9.0/src/prot/prompt/contrib/regular_languages/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3220 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/contrib/regular_languages/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    21888 2023-06-16 11:24:49.000000 prot-3.9.0/src/prot/prompt/contrib/regular_languages/compiler.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3238 2023-06-16 11:24:48.000000 prot-3.9.0/src/prot/prompt/contrib/regular_languages/completion.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3385 2023-06-16 11:24:48.000000 prot-3.9.0/src/prot/prompt/contrib/regular_languages/lexer.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     7825 2023-06-16 11:24:49.000000 prot-3.9.0/src/prot/prompt/contrib/regular_languages/regex_parser.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2034 2023-06-16 11:24:48.000000 prot-3.9.0/src/prot/prompt/contrib/regular_languages/validation.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.604819 prot-3.9.0/src/prot/prompt/contrib/ssh/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      138 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/contrib/ssh/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     4365 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/contrib/ssh/server.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.604819 prot-3.9.0/src/prot/prompt/contrib/telnet/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)       68 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/contrib/telnet/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      130 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/contrib/telnet/log.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     4965 2023-06-16 11:24:49.000000 prot-3.9.0/src/prot/prompt/contrib/telnet/protocol.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     9512 2023-06-16 11:24:49.000000 prot-3.9.0/src/prot/prompt/contrib/telnet/server.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      187 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/data_structures.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    40559 2023-06-16 11:24:51.000000 prot-3.9.0/src/prot/prompt/document.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      322 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/enums.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.608819 prot-3.9.0/src/prot/prompt/eventloop/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      636 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/eventloop/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     4125 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/eventloop/async_context_manager.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1711 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/eventloop/async_generator.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1117 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/eventloop/dummy_contextvars.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     5514 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/eventloop/inputhook.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3251 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/eventloop/utils.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2008 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/eventloop/win32.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.608819 prot-3.9.0/src/prot/prompt/filters/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1028 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/filters/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     9261 2023-06-16 11:24:50.000000 prot-3.9.0/src/prot/prompt/filters/app.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     5733 2023-06-16 11:24:49.000000 prot-3.9.0/src/prot/prompt/filters/base.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1830 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/filters/cli.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      848 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/filters/utils.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.612819 prot-3.9.0/src/prot/prompt/formatted_text/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1378 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/formatted_text/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     8089 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/formatted_text/ansi.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     4885 2023-06-16 11:24:50.000000 prot-3.9.0/src/prot/prompt/formatted_text/base.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     4324 2023-06-16 11:24:50.000000 prot-3.9.0/src/prot/prompt/formatted_text/html.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      756 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/formatted_text/pygments.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2747 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/formatted_text/utils.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     7129 2023-06-16 11:24:50.000000 prot-3.9.0/src/prot/prompt/history.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.616819 prot-3.9.0/src/prot/prompt/input/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      209 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/input/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    13116 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/input/ansi_escape_sequences.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3269 2023-06-16 11:24:50.000000 prot-3.9.0/src/prot/prompt/input/base.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1522 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/input/defaults.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1831 2023-06-16 11:24:50.000000 prot-3.9.0/src/prot/prompt/input/posix_pipe.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3897 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/input/posix_utils.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2538 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/input/typeahead.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    10129 2023-06-16 11:24:50.000000 prot-3.9.0/src/prot/prompt/input/vt100.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     8400 2023-06-16 11:24:50.000000 prot-3.9.0/src/prot/prompt/input/vt100_parser.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    22280 2023-06-16 11:24:51.000000 prot-3.9.0/src/prot/prompt/input/win32.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     4101 2023-06-16 11:24:50.000000 prot-3.9.0/src/prot/prompt/input/win32_pipe.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.620819 prot-3.9.0/src/prot/prompt/key_binding/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      335 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/key_binding/__init__.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.624819 prot-3.9.0/src/prot/prompt/key_binding/bindings/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1736 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/auto_suggest.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     7103 2023-06-16 11:24:51.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/basic.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     6965 2023-06-16 11:24:51.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/completion.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      744 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/cpr.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    19603 2023-06-16 11:24:52.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/emacs.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      468 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/focus.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     4946 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/mouse.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    18366 2023-06-16 11:24:52.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/named_commands.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1316 2023-06-16 11:24:51.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/open_in_editor.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2349 2023-06-16 11:24:51.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/page_navigation.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     5573 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/scroll.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2583 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/search.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    75190 2023-06-16 11:24:56.000000 prot-3.9.0/src/prot/prompt/key_binding/bindings/vi.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1917 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/key_binding/defaults.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    32798 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/key_binding/digraphs.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      889 2023-06-16 11:24:51.000000 prot-3.9.0/src/prot/prompt/key_binding/emacs_state.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    19387 2023-06-16 11:24:52.000000 prot-3.9.0/src/prot/prompt/key_binding/key_bindings.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    17624 2023-06-16 11:24:53.000000 prot-3.9.0/src/prot/prompt/key_binding/key_processor.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3312 2023-06-16 11:24:52.000000 prot-3.9.0/src/prot/prompt/key_binding/vi_state.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     4885 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/keys.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.628819 prot-3.9.0/src/prot/prompt/layout/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3462 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/layout/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    97453 2023-06-16 11:24:57.000000 prot-3.9.0/src/prot/prompt/layout/containers.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    34933 2023-06-16 11:24:54.000000 prot-3.9.0/src/prot/prompt/layout/controls.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     6937 2023-06-16 11:24:53.000000 prot-3.9.0/src/prot/prompt/layout/dimension.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1001 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/layout/dummy.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    14081 2023-06-16 11:24:53.000000 prot-3.9.0/src/prot/prompt/layout/layout.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    10366 2023-06-16 11:24:53.000000 prot-3.9.0/src/prot/prompt/layout/margins.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    25351 2023-06-16 11:24:54.000000 prot-3.9.0/src/prot/prompt/layout/menus.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1043 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/layout/mouse_handlers.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    34123 2023-06-16 11:24:55.000000 prot-3.9.0/src/prot/prompt/layout/processors.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     9744 2023-06-16 11:24:54.000000 prot-3.9.0/src/prot/prompt/layout/screen.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2259 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/layout/utils.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.632819 prot-3.9.0/src/prot/prompt/lexers/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      372 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/lexers/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2320 2023-06-16 11:24:54.000000 prot-3.9.0/src/prot/prompt/lexers/base.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    11933 2023-06-16 11:24:55.000000 prot-3.9.0/src/prot/prompt/lexers/pygments.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      116 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/log.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1339 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/mouse_events.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.632819 prot-3.9.0/src/prot/prompt/output/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      244 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/output/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     6268 2023-06-16 11:24:54.000000 prot-3.9.0/src/prot/prompt/output/base.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2199 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/output/color_depth.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1487 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/output/conemu.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1886 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/output/defaults.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    21307 2023-06-16 11:24:56.000000 prot-3.9.0/src/prot/prompt/output/vt100.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    21122 2023-06-16 11:24:56.000000 prot-3.9.0/src/prot/prompt/output/win32.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2794 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/output/windows10.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     5154 2023-06-16 11:24:55.000000 prot-3.9.0/src/prot/prompt/patch_stdout.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    25802 2023-06-16 11:24:56.000000 prot-3.9.0/src/prot/prompt/renderer.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     6996 2023-06-16 11:24:56.000000 prot-3.9.0/src/prot/prompt/search.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1288 2023-06-16 11:24:56.000000 prot-3.9.0/src/prot/prompt/selection.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.636819 prot-3.9.0/src/prot/prompt/shortcuts/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      844 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/shortcuts/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     8758 2023-06-16 11:24:57.000000 prot-3.9.0/src/prot/prompt/shortcuts/dialogs.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.636819 prot-3.9.0/src/prot/prompt/shortcuts/progress_bar/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      458 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/shortcuts/progress_bar/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    14068 2023-06-16 11:24:57.000000 prot-3.9.0/src/prot/prompt/shortcuts/progress_bar/base.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    11758 2023-06-16 11:24:57.000000 prot-3.9.0/src/prot/prompt/shortcuts/progress_bar/formatters.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    57259 2023-06-16 11:24:59.000000 prot-3.9.0/src/prot/prompt/shortcuts/prompt.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     5707 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/shortcuts/utils.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.640819 prot-3.9.0/src/prot/prompt/styles/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1603 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/styles/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     5062 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/styles/base.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     8409 2023-06-16 11:24:57.000000 prot-3.9.0/src/prot/prompt/styles/defaults.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     4355 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/styles/named_colors.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1952 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/styles/pygments.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    13019 2023-06-16 11:24:58.000000 prot-3.9.0/src/prot/prompt/styles/style.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    12433 2023-06-16 11:24:58.000000 prot-3.9.0/src/prot/prompt/styles/style_transformation.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)       85 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/token.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     8107 2023-06-16 11:24:57.000000 prot-3.9.0/src/prot/prompt/utils.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     5836 2023-06-16 11:24:57.000000 prot-3.9.0/src/prot/prompt/validation.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.640819 prot-3.9.0/src/prot/prompt/widgets/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     1181 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/widgets/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    28425 2023-06-16 11:24:59.000000 prot-3.9.0/src/prot/prompt/widgets/base.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3348 2023-06-16 11:24:58.000000 prot-3.9.0/src/prot/prompt/widgets/dialogs.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    12722 2023-06-16 11:24:58.000000 prot-3.9.0/src/prot/prompt/widgets/menus.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    12179 2023-06-16 11:24:58.000000 prot-3.9.0/src/prot/prompt/widgets/toolbars.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     4138 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/prompt/win32_types.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.640819 prot-3.9.0/src/prot/wcwidth/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)      150 2023-06-16 11:24:58.000000 prot-3.9.0/src/prot/wcwidth/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    10556 2023-06-16 11:24:58.000000 prot-3.9.0/src/prot/wcwidth/table_wide.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)    31378 2023-06-16 11:24:59.000000 prot-3.9.0/src/prot/wcwidth/table_zero.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.644819 prot-3.9.0/src/prot/wcwidth/tests/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)       42 2023-06-15 09:23:01.000000 prot-3.9.0/src/prot/wcwidth/tests/__init__.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     3941 2023-06-16 11:24:58.000000 prot-3.9.0/src/prot/wcwidth/tests/test_core.py
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     7908 2023-06-16 11:24:58.000000 prot-3.9.0/src/prot/wcwidth/wcwidth.py
-drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 11:49:10.584819 prot-3.9.0/src/prot.egg-info/
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     2341 2023-06-16 11:49:10.000000 prot-3.9.0/src/prot.egg-info/PKG-INFO
--rw-------   0 u0_a269  (10269) u0_a269  (10269)     6360 2023-06-16 11:49:10.000000 prot-3.9.0/src/prot.egg-info/SOURCES.txt
--rw-------   0 u0_a269  (10269) u0_a269  (10269)        1 2023-06-16 11:49:10.000000 prot-3.9.0/src/prot.egg-info/dependency_links.txt
--rw-------   0 u0_a269  (10269) u0_a269  (10269)       59 2023-06-16 11:49:10.000000 prot-3.9.0/src/prot.egg-info/entry_points.txt
--rw-------   0 u0_a269  (10269) u0_a269  (10269)        5 2023-06-16 11:49:10.000000 prot-3.9.0/src/prot.egg-info/top_level.txt
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.388023 prot-3.9.1/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1069 2023-06-15 09:23:01.000000 prot-3.9.1/LICENSE
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2341 2023-06-16 14:28:29.388023 prot-3.9.1/PKG-INFO
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1444 2023-06-15 09:23:01.000000 prot-3.9.1/README.md
+-rw-r--r--   0 u0_a269  (10269) u0_a269  (10269)       57 2023-06-15 09:29:23.000000 prot-3.9.1/pyproject.toml
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)       38 2023-06-16 14:28:29.388023 prot-3.9.1/setup.cfg
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1429 2023-06-15 09:23:01.000000 prot-3.9.1/setup.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.348023 prot-3.9.1/src/
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.356023 prot-3.9.1/src/prot/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    48198 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     4570 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/__main__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)       22 2023-06-16 14:27:37.000000 prot-3.9.1/src/prot/__version__.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.356023 prot-3.9.1/src/prot/bs/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      137 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/bs/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     5598 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/bs/bs.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2190 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/bs/bsMap.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      913 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/bs/bsPro.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1300 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/bs/bsSpaz.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    16236 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/code.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.356023 prot-3.9.1/src/prot/color/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      239 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/color/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2299 2023-06-16 11:24:46.000000 prot-3.9.1/src/prot/color/ansi.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    10557 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/color/ansitowin32.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1915 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/color/initialise.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     5480 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/color/win32.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     6464 2023-06-16 11:24:47.000000 prot-3.9.1/src/prot/color/winterm.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.360023 prot-3.9.1/src/prot/pip/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    12223 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/pip/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2355 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/pip/__main__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      797 2023-06-16 11:24:47.000000 prot-3.9.1/src/prot/pip/extra.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)       18 2023-06-16 11:46:04.000000 prot-3.9.1/src/prot/pip/packagesList.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.360023 prot-3.9.1/src/prot/progress/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     4883 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/progress/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2789 2023-06-16 11:24:47.000000 prot-3.9.1/src/prot/progress/bar.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1373 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/progress/counter.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1381 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/progress/spinner.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.364023 prot-3.9.1/src/prot/prompt/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      872 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/__init__.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.364023 prot-3.9.1/src/prot/prompt/application/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      518 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/application/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    44504 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/application/application.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     5061 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/application/current.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1349 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/application/dummy.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3699 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/application/run_in_terminal.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     5918 2023-06-16 11:24:47.000000 prot-3.9.1/src/prot/prompt/auto_suggest.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    70295 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/buffer.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3788 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/cache.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.364023 prot-3.9.1/src/prot/prompt/clipboard/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      403 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/clipboard/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2488 2023-06-16 11:24:47.000000 prot-3.9.1/src/prot/prompt/clipboard/base.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1076 2023-06-16 11:24:48.000000 prot-3.9.1/src/prot/prompt/clipboard/in_memory.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1148 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/clipboard/pyperclip.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.364023 prot-3.9.1/src/prot/prompt/completion/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      813 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/completion/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    11486 2023-06-16 11:24:48.000000 prot-3.9.1/src/prot/prompt/completion/base.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3831 2023-06-16 11:24:48.000000 prot-3.9.1/src/prot/prompt/completion/filesystem.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     6962 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/completion/fuzzy_completer.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3884 2023-06-16 11:24:48.000000 prot-3.9.1/src/prot/prompt/completion/nested.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2931 2023-06-16 11:24:48.000000 prot-3.9.1/src/prot/prompt/completion/word_completer.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.364023 prot-3.9.1/src/prot/prompt/contrib/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/contrib/__init__.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.368023 prot-3.9.1/src/prot/prompt/contrib/completers/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)       36 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/contrib/completers/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2061 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/contrib/completers/system.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.368023 prot-3.9.1/src/prot/prompt/contrib/regular_languages/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3220 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/contrib/regular_languages/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    21876 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/contrib/regular_languages/compiler.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3238 2023-06-16 11:24:48.000000 prot-3.9.1/src/prot/prompt/contrib/regular_languages/completion.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3385 2023-06-16 11:24:48.000000 prot-3.9.1/src/prot/prompt/contrib/regular_languages/lexer.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     7825 2023-06-16 11:24:49.000000 prot-3.9.1/src/prot/prompt/contrib/regular_languages/regex_parser.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2034 2023-06-16 11:24:48.000000 prot-3.9.1/src/prot/prompt/contrib/regular_languages/validation.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.368023 prot-3.9.1/src/prot/prompt/contrib/ssh/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      138 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/contrib/ssh/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     4365 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/contrib/ssh/server.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.368023 prot-3.9.1/src/prot/prompt/contrib/telnet/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)       68 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/contrib/telnet/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      130 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/contrib/telnet/log.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     4965 2023-06-16 11:24:49.000000 prot-3.9.1/src/prot/prompt/contrib/telnet/protocol.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     9510 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/contrib/telnet/server.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      187 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/data_structures.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    40581 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/document.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      322 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/enums.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.368023 prot-3.9.1/src/prot/prompt/eventloop/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      670 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/eventloop/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     4126 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/eventloop/async_context_manager.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1711 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/eventloop/async_generator.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1117 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/eventloop/dummy_contextvars.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     5514 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/eventloop/inputhook.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3251 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/eventloop/utils.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2008 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/eventloop/win32.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.372023 prot-3.9.1/src/prot/prompt/filters/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1028 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/filters/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     9261 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/filters/app.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     5733 2023-06-16 11:24:49.000000 prot-3.9.1/src/prot/prompt/filters/base.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1830 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/filters/cli.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      848 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/filters/utils.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.372023 prot-3.9.1/src/prot/prompt/formatted_text/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1386 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/formatted_text/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     8089 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/formatted_text/ansi.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     4907 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/formatted_text/base.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     4324 2023-06-16 11:24:50.000000 prot-3.9.1/src/prot/prompt/formatted_text/html.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      756 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/formatted_text/pygments.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2747 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/formatted_text/utils.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     7129 2023-06-16 11:24:50.000000 prot-3.9.1/src/prot/prompt/history.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.372023 prot-3.9.1/src/prot/prompt/input/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      209 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/input/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    13116 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/input/ansi_escape_sequences.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3269 2023-06-16 11:24:50.000000 prot-3.9.1/src/prot/prompt/input/base.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1522 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/input/defaults.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1831 2023-06-16 11:24:50.000000 prot-3.9.1/src/prot/prompt/input/posix_pipe.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3897 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/input/posix_utils.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2538 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/input/typeahead.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    10106 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/input/vt100.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     8400 2023-06-16 11:24:50.000000 prot-3.9.1/src/prot/prompt/input/vt100_parser.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    22331 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/input/win32.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     4101 2023-06-16 11:24:50.000000 prot-3.9.1/src/prot/prompt/input/win32_pipe.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.376023 prot-3.9.1/src/prot/prompt/key_binding/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      339 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/key_binding/__init__.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.376023 prot-3.9.1/src/prot/prompt/key_binding/bindings/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1736 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/auto_suggest.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     7109 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/basic.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     6986 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/completion.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      744 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/cpr.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    19692 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/emacs.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      468 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/focus.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     4946 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/mouse.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    18366 2023-06-16 11:24:52.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/named_commands.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1316 2023-06-16 11:24:51.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/open_in_editor.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2437 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/page_navigation.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     5573 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/scroll.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2583 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/search.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    75426 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/key_binding/bindings/vi.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2034 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/key_binding/defaults.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    32798 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/key_binding/digraphs.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      889 2023-06-16 11:24:51.000000 prot-3.9.1/src/prot/prompt/key_binding/emacs_state.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    19364 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/key_binding/key_bindings.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    17624 2023-06-16 11:24:53.000000 prot-3.9.1/src/prot/prompt/key_binding/key_processor.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3312 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/key_binding/vi_state.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     4885 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/keys.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.380023 prot-3.9.1/src/prot/prompt/layout/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3503 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/layout/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    97509 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/layout/containers.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    35014 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/layout/controls.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     6937 2023-06-16 11:24:53.000000 prot-3.9.1/src/prot/prompt/layout/dimension.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1001 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/layout/dummy.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    14083 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/layout/layout.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    10431 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/layout/margins.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    25363 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/layout/menus.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1043 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/layout/mouse_handlers.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    34212 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/layout/processors.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     9766 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/layout/screen.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2259 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/layout/utils.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.380023 prot-3.9.1/src/prot/prompt/lexers/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      372 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/lexers/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2320 2023-06-16 11:24:54.000000 prot-3.9.1/src/prot/prompt/lexers/base.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    11918 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/lexers/pygments.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      116 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/log.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1339 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/mouse_events.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.384023 prot-3.9.1/src/prot/prompt/output/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      244 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/output/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     6268 2023-06-16 11:24:54.000000 prot-3.9.1/src/prot/prompt/output/base.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2199 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/output/color_depth.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1487 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/output/conemu.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1902 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/output/defaults.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    21280 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/output/vt100.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    21158 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/output/win32.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2794 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/output/windows10.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     5154 2023-06-16 11:24:55.000000 prot-3.9.1/src/prot/prompt/patch_stdout.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    25837 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/renderer.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     6996 2023-06-16 11:24:56.000000 prot-3.9.1/src/prot/prompt/search.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1288 2023-06-16 11:24:56.000000 prot-3.9.1/src/prot/prompt/selection.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.384023 prot-3.9.1/src/prot/prompt/shortcuts/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      877 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/shortcuts/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     8808 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/shortcuts/dialogs.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.384023 prot-3.9.1/src/prot/prompt/shortcuts/progress_bar/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      461 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/shortcuts/progress_bar/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    14072 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/shortcuts/progress_bar/base.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    11779 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/shortcuts/progress_bar/formatters.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    58073 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/shortcuts/prompt.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     5770 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/shortcuts/utils.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.384023 prot-3.9.1/src/prot/prompt/styles/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1844 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/styles/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     5062 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/styles/base.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     8409 2023-06-16 11:24:57.000000 prot-3.9.1/src/prot/prompt/styles/defaults.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     4355 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/styles/named_colors.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1952 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/styles/pygments.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    13015 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/styles/style.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    12433 2023-06-16 11:24:58.000000 prot-3.9.1/src/prot/prompt/styles/style_transformation.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)       85 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/token.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     8084 2023-06-16 14:15:03.000000 prot-3.9.1/src/prot/prompt/utils.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     5836 2023-06-16 11:24:57.000000 prot-3.9.1/src/prot/prompt/validation.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.388023 prot-3.9.1/src/prot/prompt/widgets/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     1164 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/widgets/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    28649 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/widgets/base.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3372 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/widgets/dialogs.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    12824 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/widgets/menus.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    12441 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/prompt/widgets/toolbars.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     4138 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/prompt/win32_types.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.388023 prot-3.9.1/src/prot/wcwidth/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)      150 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/wcwidth/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    10556 2023-06-16 11:24:58.000000 prot-3.9.1/src/prot/wcwidth/table_wide.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)    31378 2023-06-16 11:24:59.000000 prot-3.9.1/src/prot/wcwidth/table_zero.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.388023 prot-3.9.1/src/prot/wcwidth/tests/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)       42 2023-06-15 09:23:01.000000 prot-3.9.1/src/prot/wcwidth/tests/__init__.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     3941 2023-06-16 11:24:58.000000 prot-3.9.1/src/prot/wcwidth/tests/test_core.py
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     7908 2023-06-16 14:15:04.000000 prot-3.9.1/src/prot/wcwidth/wcwidth.py
+drwx------   0 u0_a269  (10269) u0_a269  (10269)        0 2023-06-16 14:28:29.356023 prot-3.9.1/src/prot.egg-info/
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     2341 2023-06-16 14:28:29.000000 prot-3.9.1/src/prot.egg-info/PKG-INFO
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)     6360 2023-06-16 14:28:29.000000 prot-3.9.1/src/prot.egg-info/SOURCES.txt
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)        1 2023-06-16 14:28:29.000000 prot-3.9.1/src/prot.egg-info/dependency_links.txt
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)       59 2023-06-16 14:28:29.000000 prot-3.9.1/src/prot.egg-info/entry_points.txt
+-rw-------   0 u0_a269  (10269) u0_a269  (10269)        5 2023-06-16 14:28:29.000000 prot-3.9.1/src/prot.egg-info/top_level.txt
```

### Comparing `prot-3.9.0/LICENSE` & `prot-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/PKG-INFO` & `prot-3.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prot
-Version: 3.9.0
+Version: 3.9.1
 Summary: A Simple Tool That Contains Advance Functions.
 Home-page: https://github.com/SAPTeamDEV/prot
 Author: Alireza Poodineh
 Author-email: itsaeliux@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prot-3.9.0/README.md` & `prot-3.9.1/README.md`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/setup.py` & `prot-3.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/__init__.py` & `prot-3.9.1/src/prot/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import sys as _sys
-import os as _os
+import builtins as _builtins
 import hashlib as _hashlib
+import os as _os
+import py_compile as _py_compile
 import random as _random
+import runpy as _r
+import socket as _socket
+import sys as _sys
 import threading as _threading
-import builtins as _builtins
-import py_compile as _py_compile
 import time as _time
-import socket as _socket
 from time import sleep as _sleep
-import runpy as _r
 
 try:
     from docutils.core import publish_file as _pf
 except:
     _pf = None
 try:
     from . import color as _c
```

### Comparing `prot-3.9.0/src/prot/__main__.py` & `prot-3.9.1/src/prot/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import sys
+
+import prot
+
 from . import *
 from . import __version__ as version
-import prot
-import sys
 
 exit = False
 if "light" in status:
     printErr("command line interface not available in light version")
     exit = True
 
 if __name__ == "__main__" and not exit:
```

### Comparing `prot-3.9.0/src/prot/bs/bs.py` & `prot-3.9.1/src/prot/bs/bs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from . import *
-
-import os
 import hashlib
+import os
 import shutil
-
 from base64 import b64encode
 from functools import partial
 
+from . import *
+
 treeCache = {}
 
 
 def getModel(file):
     return file + ".bob"
```

### Comparing `prot-3.9.0/src/prot/bs/bsMap.py` & `prot-3.9.1/src/prot/bs/bsMap.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from . import *
-
 import builtins as _builtins
 
+from . import *
+
 maps = {}
 depends = []
 
 
 class Map(object):
     name = "Map"
```

### Comparing `prot-3.9.0/src/prot/bs/bsPro.py` & `prot-3.9.1/src/prot/bs/bsPro.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from . import *
-
 import json
-
 from base64 import b64encode
 
+from . import *
+
 
 def bpp2cbpp(source):
     with open(source) as file:
         codesList = [row for row in file]
     codedStr = None
     stdStr = ""
     for c in codesList:
```

### Comparing `prot-3.9.0/src/prot/bs/bsSpaz.py` & `prot-3.9.1/src/prot/bs/bsSpaz.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from . import *
-
 import os
 import shutil
 
+from . import *
+
 appearances = {}
 
 
 class Appearance(Database):
     def __init__(self, name):
         Database.__init__(self)
         if not name in appearances:
```

### Comparing `prot-3.9.0/src/prot/code.py` & `prot-3.9.1/src/prot/code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
-from . import printMsg, printErr, printWarn, Database, list2str
-import random, base64 as __cmethst__, os, sys
+import base64 as __cmethst__
+import os
+import random
+import sys
+
+from . import Database, list2str, printErr, printMsg, printWarn
 
 __spec__.data = Database()
 __spec__.data.codeType = [
     {
         "codes": [
             "D=u*JdO7&//+g7fsH33Xk*M*$7*u_.",
             "=ev1=5u?$?-W5gf0n%w#5_7$%h__kq",
```

### Comparing `prot-3.9.0/src/prot/color/ansi.py` & `prot-3.9.1/src/prot/color/ansi.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/color/ansitowin32.py` & `prot-3.9.1/src/prot/color/ansitowin32.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # Copyright Jonathan Hartley 2013. BSD 3-Clause license, see LICENSE file.
+import os
 import re
 import sys
-import os
-
-from .ansi import AnsiFore, AnsiBack, AnsiStyle, Style
-from .winterm import WinTerm, WinColor, WinStyle
-from .win32 import windll, winapi_test
 
+from .ansi import AnsiBack, AnsiFore, AnsiStyle, Style
+from .win32 import winapi_test, windll
+from .winterm import WinColor, WinStyle, WinTerm
 
 winterm = None
 if windll is not None:
     winterm = WinTerm()
 
 
 class StreamWrapper(object):
```

### Comparing `prot-3.9.0/src/prot/color/initialise.py` & `prot-3.9.1/src/prot/color/initialise.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright Jonathan Hartley 2013. BSD 3-Clause license, see LICENSE file.
 import atexit
 import contextlib
 import sys
 
 from .ansitowin32 import AnsiToWin32
 
-
 orig_stdout = None
 orig_stderr = None
 
 wrapped_stdout = None
 wrapped_stderr = None
 
 atexit_done = False
```

### Comparing `prot-3.9.0/src/prot/color/win32.py` & `prot-3.9.1/src/prot/color/win32.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     windll = LibraryLoader(ctypes.WinDLL)
     from ctypes import wintypes
 except (AttributeError, ImportError):
     windll = None
     SetConsoleTextAttribute = lambda *_: None
     winapi_test = lambda *_: None
 else:
-    from ctypes import byref, Structure, c_char, POINTER
+    from ctypes import POINTER, Structure, byref, c_char
 
     COORD = wintypes._COORD
 
     class CONSOLE_SCREEN_BUFFER_INFO(Structure):
         """struct in wincon.h."""
 
         _fields_ = [
```

### Comparing `prot-3.9.0/src/prot/color/winterm.py` & `prot-3.9.1/src/prot/color/winterm.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/pip/__init__.py` & `prot-3.9.1/src/prot/pip/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 try:
     from .packagesList import packagesList as _p
 except:
     _p = []
 import os
 import runpy as _r
+
 from .. import *
 
 try:
     import xmlrpc.client as xmlrpclib
 except:
     xmlrpclib = None
```

### Comparing `prot-3.9.0/src/prot/pip/__main__.py` & `prot-3.9.1/src/prot/pip/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import sys
-from . import *
+
 from .. import *
+from . import *
 
 exit = False
 if "light" in status:
     printErr("command line interface not available in light version")
     exit = True
 
 if __name__ == "__main__" and not exit:
```

### Comparing `prot-3.9.0/src/prot/pip/extra.py` & `prot-3.9.1/src/prot/pip/extra.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/progress/__init__.py` & `prot-3.9.1/src/prot/progress/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,20 +10,21 @@
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 from __future__ import division, print_function
 
-from .. import printMsg
 from collections import deque
 from datetime import timedelta
 from math import ceil
 from sys import stderr, stdout
 
+from .. import printMsg
+
 try:
     from time import monotonic
 except ImportError:
     from time import time as monotonic
 
 
 __version__ = "1.5"
```

### Comparing `prot-3.9.0/src/prot/progress/bar.py` & `prot-3.9.1/src/prot/progress/bar.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/progress/counter.py` & `prot-3.9.1/src/prot/progress/counter.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 from __future__ import unicode_literals
+
 from . import Infinite, Progress
 
 
 class Counter(Infinite):
     def update(self):
         self.write(str(self.index))
```

### Comparing `prot-3.9.0/src/prot/progress/spinner.py` & `prot-3.9.1/src/prot/progress/spinner.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 from __future__ import unicode_literals
+
 from . import Infinite
 
 
 class Spinner(Infinite):
     phases = ("-", "\\", "|", "/")
     hide_cursor = True
```

### Comparing `prot-3.9.0/src/prot/prompt/__init__.py` & `prot-3.9.1/src/prot/prompt/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/application/__init__.py` & `prot-3.9.1/src/prot/prompt/application/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 from .application import Application
-from .current import (
-    create_app_session,
-    get_app,
-    get_app_or_none,
-    get_app_session,
-    set_app,
-)
+from .current import (create_app_session, get_app, get_app_or_none,
+                      get_app_session, set_app)
 from .dummy import DummyApplication
 from .run_in_terminal import in_terminal, run_in_terminal
 
 __all__ = [
     # Application.
     "Application",
     # Current.
```

### Comparing `prot-3.9.0/src/prot/prompt/application/application.py` & `prot-3.9.1/src/prot/prompt/application/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,93 +1,58 @@
 import asyncio
 import os
 import re
 import signal
 import sys
 import time
-from prot import printMsg
-from asyncio import (
-    AbstractEventLoop,
-    CancelledError,
-    Future,
-    Task,
-    ensure_future,
-    get_event_loop,
-    new_event_loop,
-    set_event_loop,
-    sleep,
-)
+from asyncio import (AbstractEventLoop, CancelledError, Future, Task,
+                     ensure_future, get_event_loop, new_event_loop,
+                     set_event_loop, sleep)
 from subprocess import Popen
 from traceback import format_tb
-from typing import (
-    Any,
-    Awaitable,
-    Callable,
-    Dict,
-    FrozenSet,
-    Generic,
-    Hashable,
-    Iterable,
-    List,
-    Optional,
-    Tuple,
-    Type,
-    TypeVar,
-    Union,
-    cast,
-    overload,
-)
+from typing import (Any, Awaitable, Callable, Dict, FrozenSet, Generic,
+                    Hashable, Iterable, List, Optional, Tuple, Type, TypeVar,
+                    Union, cast, overload)
 
+from prot import printMsg
 from prot.prompt.buffer import Buffer
 from prot.prompt.cache import SimpleCache
 from prot.prompt.clipboard import Clipboard, InMemoryClipboard
 from prot.prompt.enums import EditingMode
-from prot.prompt.eventloop import (
-    get_traceback_from_context,
-    run_in_executor_with_context,
-)
+from prot.prompt.eventloop import (get_traceback_from_context,
+                                   run_in_executor_with_context)
 from prot.prompt.eventloop.utils import call_soon_threadsafe
 from prot.prompt.filters import Condition, Filter, FilterOrBool, to_filter
 from prot.prompt.formatted_text import AnyFormattedText
 from prot.prompt.input.base import Input
 from prot.prompt.input.typeahead import get_typeahead, store_typeahead
-from prot.prompt.key_binding.bindings.page_navigation import (
-    load_page_navigation_bindings,
-)
+from prot.prompt.key_binding.bindings.page_navigation import \
+    load_page_navigation_bindings
 from prot.prompt.key_binding.defaults import load_key_bindings
 from prot.prompt.key_binding.emacs_state import EmacsState
-from prot.prompt.key_binding.key_bindings import (
-    Binding,
-    ConditionalKeyBindings,
-    GlobalOnlyKeyBindings,
-    KeyBindings,
-    KeyBindingsBase,
-    KeysTuple,
-    merge_key_bindings,
-)
+from prot.prompt.key_binding.key_bindings import (Binding,
+                                                  ConditionalKeyBindings,
+                                                  GlobalOnlyKeyBindings,
+                                                  KeyBindings, KeyBindingsBase,
+                                                  KeysTuple,
+                                                  merge_key_bindings)
 from prot.prompt.key_binding.key_processor import KeyPressEvent, KeyProcessor
 from prot.prompt.key_binding.vi_state import ViState
 from prot.prompt.keys import Keys
 from prot.prompt.layout.containers import Container, Window
 from prot.prompt.layout.controls import BufferControl, UIControl
 from prot.prompt.layout.dummy import create_dummy_layout
 from prot.prompt.layout.layout import Layout, walk
 from prot.prompt.output import ColorDepth, Output
 from prot.prompt.renderer import Renderer, print_formatted_text
 from prot.prompt.search import SearchState
-from prot.prompt.styles import (
-    BaseStyle,
-    DummyStyle,
-    DummyStyleTransformation,
-    DynamicStyle,
-    StyleTransformation,
-    default_pygments_style,
-    default_ui_style,
-    merge_styles,
-)
+from prot.prompt.styles import (BaseStyle, DummyStyle,
+                                DummyStyleTransformation, DynamicStyle,
+                                StyleTransformation, default_pygments_style,
+                                default_ui_style, merge_styles)
 from prot.prompt.utils import Event, in_main_thread
 
 from .current import get_app_session, set_app
 from .run_in_terminal import in_terminal, run_in_terminal
 
 try:
     import contextvars
```

### Comparing `prot-3.9.0/src/prot/prompt/application/current.py` & `prot-3.9.1/src/prot/prompt/application/current.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import sys
 from contextlib import contextmanager
 from typing import TYPE_CHECKING, Any, Generator, Optional
 
 try:
     from contextvars import ContextVar
 except ImportError:
-    from prot.prompt.eventloop.dummy_contextvars import ContextVar  # type: ignore
+    from prot.prompt.eventloop.dummy_contextvars import \
+        ContextVar  # type: ignore
 
 if TYPE_CHECKING:
-    from .application import Application
     from prot.prompt.input.defaults import Input
     from prot.prompt.output.defaults import Output
 
+    from .application import Application
+
 __all__ = [
     "get_app_session",
     "get_app",
     "get_app_or_none",
     "set_app",
     "create_app_session",
 ]
```

### Comparing `prot-3.9.0/src/prot/prompt/application/dummy.py` & `prot-3.9.1/src/prot/prompt/application/dummy.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/application/run_in_terminal.py` & `prot-3.9.1/src/prot/prompt/application/run_in_terminal.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/auto_suggest.py` & `prot-3.9.1/src/prot/prompt/auto_suggest.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/buffer.py` & `prot-3.9.1/src/prot/prompt/buffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,40 +7,24 @@
 import re
 import shlex
 import shutil
 import subprocess
 import tempfile
 from enum import Enum
 from functools import wraps
-from typing import (
-    Any,
-    Awaitable,
-    Callable,
-    Iterable,
-    List,
-    Optional,
-    Set,
-    Tuple,
-    TypeVar,
-    Union,
-    cast,
-)
+from typing import (Any, Awaitable, Callable, Iterable, List, Optional, Set,
+                    Tuple, TypeVar, Union, cast)
 
 from .application.current import get_app
 from .application.run_in_terminal import run_in_terminal
 from .auto_suggest import AutoSuggest, Suggestion
 from .cache import FastDictCache
 from .clipboard import ClipboardData
-from .completion import (
-    CompleteEvent,
-    Completer,
-    Completion,
-    DummyCompleter,
-    get_common_complete_suffix,
-)
+from .completion import (CompleteEvent, Completer, Completion, DummyCompleter,
+                         get_common_complete_suffix)
 from .document import Document
 from .filters import FilterOrBool, to_filter
 from .history import History, InMemoryHistory
 from .search import SearchDirection, SearchState
 from .selection import PasteMode, SelectionState, SelectionType
 from .utils import Event, to_str
 from .validation import ValidationError, Validator
```

### Comparing `prot-3.9.0/src/prot/prompt/cache.py` & `prot-3.9.1/src/prot/prompt/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from collections import deque
 from functools import wraps
-from typing import Any, Callable, Deque, Dict, Generic, Hashable, Tuple, TypeVar, cast
+from typing import (Any, Callable, Deque, Dict, Generic, Hashable, Tuple,
+                    TypeVar, cast)
 
 __all__ = [
     "SimpleCache",
     "FastDictCache",
     "memoized",
 ]
```

### Comparing `prot-3.9.0/src/prot/prompt/clipboard/base.py` & `prot-3.9.1/src/prot/prompt/clipboard/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/clipboard/in_memory.py` & `prot-3.9.1/src/prot/prompt/clipboard/in_memory.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/clipboard/pyperclip.py` & `prot-3.9.1/src/prot/prompt/clipboard/pyperclip.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Optional
 
 import pyperclip
+
 from prot.prompt.selection import SelectionType
 
 from .base import Clipboard, ClipboardData
 
 __all__ = [
     "PyperclipClipboard",
 ]
```

### Comparing `prot-3.9.0/src/prot/prompt/completion/__init__.py` & `prot-3.9.1/src/prot/prompt/completion/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,10 @@
-from .base import (
-    CompleteEvent,
-    Completer,
-    Completion,
-    DummyCompleter,
-    DynamicCompleter,
-    ThreadedCompleter,
-    get_common_complete_suffix,
-    merge_completers,
-)
+from .base import (CompleteEvent, Completer, Completion, DummyCompleter,
+                   DynamicCompleter, ThreadedCompleter,
+                   get_common_complete_suffix, merge_completers)
 from .filesystem import ExecutableCompleter, PathCompleter
 from .fuzzy_completer import FuzzyCompleter, FuzzyWordCompleter
 from .nested import NestedCompleter
 from .word_completer import WordCompleter
 
 __all__ = [
     # Base.
```

### Comparing `prot-3.9.0/src/prot/prompt/completion/base.py` & `prot-3.9.1/src/prot/prompt/completion/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/completion/filesystem.py` & `prot-3.9.1/src/prot/prompt/completion/filesystem.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/completion/fuzzy_completer.py` & `prot-3.9.1/src/prot/prompt/completion/fuzzy_completer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
-from typing import Callable, Dict, Iterable, List, NamedTuple, Optional, Tuple, Union
+from typing import (Callable, Dict, Iterable, List, NamedTuple, Optional,
+                    Tuple, Union)
 
 from prot.prompt.document import Document
 from prot.prompt.filters import FilterOrBool, to_filter
 from prot.prompt.formatted_text import AnyFormattedText, StyleAndTextTuples
 
 from .base import CompleteEvent, Completer, Completion
 from .word_completer import WordCompleter
```

### Comparing `prot-3.9.0/src/prot/prompt/completion/nested.py` & `prot-3.9.1/src/prot/prompt/completion/nested.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/completion/word_completer.py` & `prot-3.9.1/src/prot/prompt/completion/word_completer.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/contrib/completers/system.py` & `prot-3.9.1/src/prot/prompt/contrib/completers/system.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from prot.prompt.completion.filesystem import ExecutableCompleter, PathCompleter
+from prot.prompt.completion.filesystem import (ExecutableCompleter,
+                                               PathCompleter)
 from prot.prompt.contrib.regular_languages.compiler import compile
 from prot.prompt.contrib.regular_languages.completion import GrammarCompleter
 
 __all__ = [
     "SystemCompleter",
 ]
```

### Comparing `prot-3.9.0/src/prot/prompt/contrib/regular_languages/__init__.py` & `prot-3.9.1/src/prot/prompt/contrib/regular_languages/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/contrib/regular_languages/compiler.py` & `prot-3.9.1/src/prot/prompt/contrib/regular_languages/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,25 +39,16 @@
 
 """
 import re
 from typing import Callable, Dict, Iterable, Iterator, List
 from typing import Match as RegexMatch
 from typing import Optional, Pattern, Tuple, cast
 
-from .regex_parser import (
-    AnyNode,
-    Lookahead,
-    Node,
-    NodeSequence,
-    Regex,
-    Repeat,
-    Variable,
-    parse_regex,
-    tokenize_regex,
-)
+from .regex_parser import (AnyNode, Lookahead, Node, NodeSequence, Regex,
+                           Repeat, Variable, parse_regex, tokenize_regex)
 
 __all__ = [
     "compile",
 ]
 
 
 # Name of the named group in the regex, matching trailing input.
```

### Comparing `prot-3.9.0/src/prot/prompt/contrib/regular_languages/completion.py` & `prot-3.9.1/src/prot/prompt/contrib/regular_languages/completion.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/contrib/regular_languages/lexer.py` & `prot-3.9.1/src/prot/prompt/contrib/regular_languages/lexer.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/contrib/regular_languages/regex_parser.py` & `prot-3.9.1/src/prot/prompt/contrib/regular_languages/regex_parser.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/contrib/regular_languages/validation.py` & `prot-3.9.1/src/prot/prompt/contrib/regular_languages/validation.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/contrib/ssh/server.py` & `prot-3.9.1/src/prot/prompt/contrib/ssh/server.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/contrib/telnet/protocol.py` & `prot-3.9.1/src/prot/prompt/contrib/telnet/protocol.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/contrib/telnet/server.py` & `prot-3.9.1/src/prot/prompt/contrib/telnet/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,30 @@
 """
 Telnet server.
 """
 import asyncio
 import contextvars  # Requires Python3.7!
 import socket
-from prot import printMsg
 from asyncio import get_event_loop
-from typing import Awaitable, Callable, List, Optional, Set, TextIO, Tuple, cast
+from typing import (Awaitable, Callable, List, Optional, Set, TextIO, Tuple,
+                    cast)
 
+from prot import printMsg
 from prot.prompt.application.current import create_app_session, get_app
 from prot.prompt.application.run_in_terminal import run_in_terminal
 from prot.prompt.data_structures import Size
 from prot.prompt.formatted_text import AnyFormattedText, to_formatted_text
 from prot.prompt.input.posix_pipe import PosixPipeInput
 from prot.prompt.output.vt100 import Vt100_Output
 from prot.prompt.renderer import print_formatted_text as print_formatted_text
 from prot.prompt.styles import BaseStyle, DummyStyle
 
 from .log import logger
-from .protocol import (
-    DO,
-    ECHO,
-    IAC,
-    LINEMODE,
-    MODE,
-    NAWS,
-    SB,
-    SE,
-    SUPPRESS_GO_AHEAD,
-    WILL,
-    TelnetProtocolParser,
-)
+from .protocol import (DO, ECHO, IAC, LINEMODE, MODE, NAWS, SB, SE,
+                       SUPPRESS_GO_AHEAD, WILL, TelnetProtocolParser)
 
 __all__ = [
     "TelnetServer",
 ]
 
 
 def int2byte(number: int) -> bytes:
```

### Comparing `prot-3.9.0/src/prot/prompt/document.py` & `prot-3.9.1/src/prot/prompt/document.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 The `Document` that implements all the text operations/querying.
 """
 import bisect
 import re
 import string
 import weakref
-from typing import Callable, Dict, Iterable, List, Optional, Pattern, Tuple, cast
+from typing import (Callable, Dict, Iterable, List, Optional, Pattern, Tuple,
+                    cast)
 
 from .clipboard import ClipboardData
 from .filters import vi_mode
 from .selection import PasteMode, SelectionState, SelectionType
 
 __all__ = [
     "Document",
```

### Comparing `prot-3.9.0/src/prot/prompt/eventloop/__init__.py` & `prot-3.9.1/src/prot/prompt/eventloop/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 from .async_generator import generator_to_async_generator
-from .inputhook import (
-    InputHookContext,
-    InputHookSelector,
-    new_eventloop_with_inputhook,
-    set_eventloop_with_inputhook,
-)
-from .utils import (
-    call_soon_threadsafe,
-    get_traceback_from_context,
-    run_in_executor_with_context,
-)
+from .inputhook import (InputHookContext, InputHookSelector,
+                        new_eventloop_with_inputhook,
+                        set_eventloop_with_inputhook)
+from .utils import (call_soon_threadsafe, get_traceback_from_context,
+                    run_in_executor_with_context)
 
 __all__ = [
     # Async generator
     "generator_to_async_generator",
     # Utils.
     "run_in_executor_with_context",
     "call_soon_threadsafe",
```

### Comparing `prot-3.9.0/src/prot/prompt/eventloop/async_context_manager.py` & `prot-3.9.1/src/prot/prompt/eventloop/async_context_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 @asynccontextmanager code, copied from Python 3.7's contextlib.
 For usage in Python 3.6.
 """
-import _collections_abc
 import abc
 from functools import wraps
 
+import _collections_abc
+
 __all__ = ["asynccontextmanager"]
 
 
 class AbstractAsyncContextManager(abc.ABC):
 
     """An abstract base class for asynchronous context managers."""
```

### Comparing `prot-3.9.0/src/prot/prompt/eventloop/async_generator.py` & `prot-3.9.1/src/prot/prompt/eventloop/async_generator.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/eventloop/dummy_contextvars.py` & `prot-3.9.1/src/prot/prompt/eventloop/dummy_contextvars.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/eventloop/inputhook.py` & `prot-3.9.1/src/prot/prompt/eventloop/inputhook.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/eventloop/utils.py` & `prot-3.9.1/src/prot/prompt/eventloop/utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/eventloop/win32.py` & `prot-3.9.1/src/prot/prompt/eventloop/win32.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/filters/__init__.py` & `prot-3.9.1/src/prot/prompt/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/filters/app.py` & `prot-3.9.1/src/prot/prompt/filters/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,17 +48,17 @@
 
 @memoized()
 def has_focus(value: "FocusableElement") -> Condition:
     """
     Enable when this buffer has the focus.
     """
     from prot.prompt.buffer import Buffer
-    from prot.prompt.layout.controls import UIControl
-    from prot.prompt.layout.containers import to_container, Window, Container
     from prot.prompt.layout import walk
+    from prot.prompt.layout.containers import Container, Window, to_container
+    from prot.prompt.layout.controls import UIControl
 
     if isinstance(value, str):
 
         def test() -> bool:
             return get_app().current_buffer.name == value
 
     elif isinstance(value, Buffer):
```

### Comparing `prot-3.9.0/src/prot/prompt/filters/base.py` & `prot-3.9.1/src/prot/prompt/filters/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/filters/cli.py` & `prot-3.9.1/src/prot/prompt/filters/cli.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/filters/utils.py` & `prot-3.9.1/src/prot/prompt/filters/utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/formatted_text/__init__.py` & `prot-3.9.1/src/prot/prompt/formatted_text/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,31 +7,21 @@
 
 In any case, there is an input that can either be just plain text (a string),
 an :class:`.HTML` object, an :class:`.ANSI` object or a sequence of
 `(style_string, text)` tuples. The :func:`.to_formatted_text` conversion
 function takes any of these and turns all of them into such a tuple sequence.
 """
 from .ansi import ANSI
-from .base import (
-    AnyFormattedText,
-    FormattedText,
-    StyleAndTextTuples,
-    Template,
-    is_formatted_text,
-    merge_formatted_text,
-    to_formatted_text,
-)
+from .base import (AnyFormattedText, FormattedText, StyleAndTextTuples,
+                   Template, is_formatted_text, merge_formatted_text,
+                   to_formatted_text)
 from .html import HTML
 from .pygments import PygmentsTokens
-from .utils import (
-    fragment_list_len,
-    fragment_list_to_text,
-    fragment_list_width,
-    split_lines,
-)
+from .utils import (fragment_list_len, fragment_list_to_text,
+                    fragment_list_width, split_lines)
 
 __all__ = [
     # Base.
     "AnyFormattedText",
     "to_formatted_text",
     "is_formatted_text",
     "Template",
```

### Comparing `prot-3.9.0/src/prot/prompt/formatted_text/ansi.py` & `prot-3.9.1/src/prot/prompt/formatted_text/ansi.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/formatted_text/base.py` & `prot-3.9.1/src/prot/prompt/formatted_text/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import TYPE_CHECKING, Any, Callable, Iterable, List, Tuple, Union, cast
+from typing import (TYPE_CHECKING, Any, Callable, Iterable, List, Tuple, Union,
+                    cast)
 
 from prot.prompt.mouse_events import MouseEvent
 
 if TYPE_CHECKING:
     from typing_extensions import Protocol
 
 __all__ = [
```

### Comparing `prot-3.9.0/src/prot/prompt/formatted_text/html.py` & `prot-3.9.1/src/prot/prompt/formatted_text/html.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/formatted_text/pygments.py` & `prot-3.9.1/src/prot/prompt/formatted_text/pygments.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/formatted_text/utils.py` & `prot-3.9.1/src/prot/prompt/formatted_text/utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/history.py` & `prot-3.9.1/src/prot/prompt/history.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/input/ansi_escape_sequences.py` & `prot-3.9.1/src/prot/prompt/input/ansi_escape_sequences.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/input/base.py` & `prot-3.9.1/src/prot/prompt/input/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/input/defaults.py` & `prot-3.9.1/src/prot/prompt/input/defaults.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/input/posix_pipe.py` & `prot-3.9.1/src/prot/prompt/input/posix_pipe.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/input/posix_utils.py` & `prot-3.9.1/src/prot/prompt/input/posix_utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/input/typeahead.py` & `prot-3.9.1/src/prot/prompt/input/typeahead.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/input/vt100.py` & `prot-3.9.1/src/prot/prompt/input/vt100.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 import contextlib
 import io
 import os
 import sys
 import termios
 import tty
 from asyncio import AbstractEventLoop, get_event_loop
-from typing import (
-    Callable,
-    ContextManager,
-    Dict,
-    Generator,
-    List,
-    Optional,
-    Set,
-    TextIO,
-    Tuple,
-    Union,
-)
+from typing import (Callable, ContextManager, Dict, Generator, List, Optional,
+                    Set, TextIO, Tuple, Union)
 
 from prot.prompt.utils import is_dumb_terminal
 
 from ..key_binding import KeyPress
 from .base import Input
 from .posix_utils import PosixStdinReader
 from .vt100_parser import Vt100Parser
```

### Comparing `prot-3.9.0/src/prot/prompt/input/vt100_parser.py` & `prot-3.9.1/src/prot/prompt/input/vt100_parser.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/input/win32.py` & `prot-3.9.1/src/prot/prompt/input/win32.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,21 +9,17 @@
 from typing import Callable, ContextManager, Dict, Iterable, Optional, TextIO
 
 from prot.prompt.eventloop import run_in_executor_with_context
 from prot.prompt.eventloop.win32 import create_win32_event, wait_for_handles
 from prot.prompt.key_binding.key_processor import KeyPress
 from prot.prompt.keys import Keys
 from prot.prompt.mouse_events import MouseEventType
-from prot.prompt.win32_types import (
-    INPUT_RECORD,
-    KEY_EVENT_RECORD,
-    MOUSE_EVENT_RECORD,
-    STD_INPUT_HANDLE,
-    EventTypes,
-)
+from prot.prompt.win32_types import (INPUT_RECORD, KEY_EVENT_RECORD,
+                                     MOUSE_EVENT_RECORD, STD_INPUT_HANDLE,
+                                     EventTypes)
 
 from .ansi_escape_sequences import REVERSE_ANSI_SEQUENCES
 from .base import Input
 
 __all__ = [
     "Win32Input",
     "ConsoleInputReader",
```

### Comparing `prot-3.9.0/src/prot/prompt/input/win32_pipe.py` & `prot-3.9.1/src/prot/prompt/input/win32_pipe.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/key_binding/bindings/auto_suggest.py` & `prot-3.9.1/src/prot/prompt/key_binding/bindings/auto_suggest.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/key_binding/bindings/basic.py` & `prot-3.9.1/src/prot/prompt/key_binding/bindings/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 # pylint: disable=function-redefined
 from prot.prompt.application.current import get_app
-from prot.prompt.filters import (
-    Condition,
-    emacs_insert_mode,
-    has_selection,
-    in_paste_mode,
-    is_multiline,
-    vi_insert_mode,
-)
+from prot.prompt.filters import (Condition, emacs_insert_mode, has_selection,
+                                 in_paste_mode, is_multiline, vi_insert_mode)
 from prot.prompt.key_binding.key_processor import KeyPress, KeyPressEvent
 from prot.prompt.keys import Keys
 
 from ..key_bindings import KeyBindings
 from .named_commands import get_by_name
 
 __all__ = [
```

### Comparing `prot-3.9.0/src/prot/prompt/key_binding/bindings/completion.py` & `prot-3.9.1/src/prot/prompt/key_binding/bindings/completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,16 @@
 Key binding handlers for displaying completions.
 """
 import asyncio
 import math
 from typing import TYPE_CHECKING, List
 
 from prot.prompt.application.run_in_terminal import in_terminal
-from prot.prompt.completion import (
-    CompleteEvent,
-    Completion,
-    get_common_complete_suffix,
-)
+from prot.prompt.completion import (CompleteEvent, Completion,
+                                    get_common_complete_suffix)
 from prot.prompt.formatted_text import StyleAndTextTuples
 from prot.prompt.key_binding.key_bindings import KeyBindings
 from prot.prompt.key_binding.key_processor import KeyPressEvent
 from prot.prompt.keys import Keys
 from prot.prompt.utils import get_cwidth
 
 if TYPE_CHECKING:
@@ -83,16 +80,16 @@
     app: "Application", completions: List[Completion]
 ) -> "asyncio.Task[None]":
     """
     Display the list of completions in columns above the prompt.
     This will ask for a confirmation if there are too many completions to fit
     on a single page and provide a paginator to walk through them.
     """
-    from prot.prompt.shortcuts.prompt import create_confirm_session
     from prot.prompt.formatted_text import to_formatted_text
+    from prot.prompt.shortcuts.prompt import create_confirm_session
 
     # Get terminal dimensions.
     term_size = app.output.get_size()
     term_width = term_size.columns
     term_height = term_size.rows
 
     # Calculate amount of required columns/rows for displaying the
```

### Comparing `prot-3.9.0/src/prot/prompt/key_binding/bindings/cpr.py` & `prot-3.9.1/src/prot/prompt/key_binding/bindings/cpr.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/key_binding/bindings/emacs.py` & `prot-3.9.1/src/prot/prompt/key_binding/bindings/emacs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,18 @@
 # pylint: disable=function-redefined
 from typing import Dict, Union
 
 from prot.prompt.application.current import get_app
 from prot.prompt.buffer import Buffer, SelectionType, indent, unindent
 from prot.prompt.completion import CompleteEvent
-from prot.prompt.filters import (
-    Condition,
-    emacs_insert_mode,
-    emacs_mode,
-    has_arg,
-    has_selection,
-    in_paste_mode,
-    is_multiline,
-    is_read_only,
-    shift_selection_mode,
-    vi_search_direction_reversed,
-)
+from prot.prompt.filters import (Condition, emacs_insert_mode, emacs_mode,
+                                 has_arg, has_selection, in_paste_mode,
+                                 is_multiline, is_read_only,
+                                 shift_selection_mode,
+                                 vi_search_direction_reversed)
 from prot.prompt.key_binding.key_bindings import Binding
 from prot.prompt.key_binding.key_processor import KeyPressEvent
 from prot.prompt.keys import Keys
 
 from ..key_bindings import ConditionalKeyBindings, KeyBindings, KeyBindingsBase
 from .named_commands import get_by_name
```

### Comparing `prot-3.9.0/src/prot/prompt/key_binding/bindings/mouse.py` & `prot-3.9.1/src/prot/prompt/key_binding/bindings/mouse.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/key_binding/bindings/named_commands.py` & `prot-3.9.1/src/prot/prompt/key_binding/bindings/named_commands.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/key_binding/bindings/open_in_editor.py` & `prot-3.9.1/src/prot/prompt/key_binding/bindings/open_in_editor.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/key_binding/bindings/page_navigation.py` & `prot-3.9.1/src/prot/prompt/key_binding/bindings/page_navigation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,19 @@
 """
 Key bindings for extra page navigation: bindings for up/down scrolling through
 long pages, like in Emacs or Vi.
 """
 from prot.prompt.filters import buffer_has_focus, emacs_mode, vi_mode
-from prot.prompt.key_binding.key_bindings import (
-    ConditionalKeyBindings,
-    KeyBindings,
-    KeyBindingsBase,
-    merge_key_bindings,
-)
+from prot.prompt.key_binding.key_bindings import (ConditionalKeyBindings,
+                                                  KeyBindings, KeyBindingsBase,
+                                                  merge_key_bindings)
 
-from .scroll import (
-    scroll_backward,
-    scroll_forward,
-    scroll_half_page_down,
-    scroll_half_page_up,
-    scroll_one_line_down,
-    scroll_one_line_up,
-    scroll_page_down,
-    scroll_page_up,
-)
+from .scroll import (scroll_backward, scroll_forward, scroll_half_page_down,
+                     scroll_half_page_up, scroll_one_line_down,
+                     scroll_one_line_up, scroll_page_down, scroll_page_up)
 
 __all__ = [
     "load_page_navigation_bindings",
     "load_emacs_page_navigation_bindings",
     "load_vi_page_navigation_bindings",
 ]
```

### Comparing `prot-3.9.0/src/prot/prompt/key_binding/bindings/scroll.py` & `prot-3.9.1/src/prot/prompt/key_binding/bindings/scroll.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/key_binding/bindings/search.py` & `prot-3.9.1/src/prot/prompt/key_binding/bindings/search.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/key_binding/bindings/vi.py` & `prot-3.9.1/src/prot/prompt/key_binding/bindings/vi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,29 @@
 # pylint: disable=function-redefined
 import codecs
 import string
 from enum import Enum
 from itertools import accumulate
-from typing import Callable, Iterable, List, Optional, Tuple, TypeVar, Union, cast
+from typing import (Callable, Iterable, List, Optional, Tuple, TypeVar, Union,
+                    cast)
 
 from prot.prompt.application.current import get_app
 from prot.prompt.buffer import Buffer, indent, reshape_text, unindent
 from prot.prompt.clipboard import ClipboardData
 from prot.prompt.document import Document
-from prot.prompt.filters import (
-    Always,
-    Condition,
-    Filter,
-    has_arg,
-    is_read_only,
-    is_searching,
-)
-from prot.prompt.filters.app import (
-    in_paste_mode,
-    is_multiline,
-    vi_digraph_mode,
-    vi_insert_mode,
-    vi_insert_multiple_mode,
-    vi_mode,
-    vi_navigation_mode,
-    vi_recording_macro,
-    vi_replace_mode,
-    vi_search_direction_reversed,
-    vi_selection_mode,
-    vi_waiting_for_text_object_mode,
-)
+from prot.prompt.filters import (Always, Condition, Filter, has_arg,
+                                 is_read_only, is_searching)
+from prot.prompt.filters.app import (in_paste_mode, is_multiline,
+                                     vi_digraph_mode, vi_insert_mode,
+                                     vi_insert_multiple_mode, vi_mode,
+                                     vi_navigation_mode, vi_recording_macro,
+                                     vi_replace_mode,
+                                     vi_search_direction_reversed,
+                                     vi_selection_mode,
+                                     vi_waiting_for_text_object_mode)
 from prot.prompt.input.vt100_parser import Vt100Parser
 from prot.prompt.key_binding.digraphs import DIGRAPHS
 from prot.prompt.key_binding.key_processor import KeyPress, KeyPressEvent
 from prot.prompt.key_binding.vi_state import CharacterFind, InputMode
 from prot.prompt.keys import Keys
 from prot.prompt.search import SearchDirection
 from prot.prompt.selection import PasteMode, SelectionState, SelectionType
```

### Comparing `prot-3.9.0/src/prot/prompt/key_binding/defaults.py` & `prot-3.9.1/src/prot/prompt/key_binding/defaults.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,28 +4,22 @@
     key_bindings = load_key_bindings()
     app = Application(key_bindings=key_bindings)
 """
 from prot.prompt.filters import buffer_has_focus
 from prot.prompt.key_binding.bindings.basic import load_basic_bindings
 from prot.prompt.key_binding.bindings.cpr import load_cpr_bindings
 from prot.prompt.key_binding.bindings.emacs import (
-    load_emacs_bindings,
-    load_emacs_search_bindings,
-    load_emacs_shift_selection_bindings,
-)
+    load_emacs_bindings, load_emacs_search_bindings,
+    load_emacs_shift_selection_bindings)
 from prot.prompt.key_binding.bindings.mouse import load_mouse_bindings
-from prot.prompt.key_binding.bindings.vi import (
-    load_vi_bindings,
-    load_vi_search_bindings,
-)
-from prot.prompt.key_binding.key_bindings import (
-    ConditionalKeyBindings,
-    KeyBindingsBase,
-    merge_key_bindings,
-)
+from prot.prompt.key_binding.bindings.vi import (load_vi_bindings,
+                                                 load_vi_search_bindings)
+from prot.prompt.key_binding.key_bindings import (ConditionalKeyBindings,
+                                                  KeyBindingsBase,
+                                                  merge_key_bindings)
 
 __all__ = [
     "load_key_bindings",
 ]
 
 
 def load_key_bindings() -> KeyBindingsBase:
```

### Comparing `prot-3.9.0/src/prot/prompt/key_binding/digraphs.py` & `prot-3.9.1/src/prot/prompt/key_binding/digraphs.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/key_binding/emacs_state.py` & `prot-3.9.1/src/prot/prompt/key_binding/emacs_state.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/key_binding/key_bindings.py` & `prot-3.9.1/src/prot/prompt/key_binding/key_bindings.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,26 +31,16 @@
     def my_key_binding(event):
         ...
 
     # Later, add it to the key bindings.
     kb.add(Keys.A, my_key_binding)
 """
 from abc import ABCMeta, abstractmethod, abstractproperty
-from typing import (
-    TYPE_CHECKING,
-    Callable,
-    Hashable,
-    List,
-    Optional,
-    Sequence,
-    Tuple,
-    TypeVar,
-    Union,
-    cast,
-)
+from typing import (TYPE_CHECKING, Callable, Hashable, List, Optional,
+                    Sequence, Tuple, TypeVar, Union, cast)
 
 from prot.prompt.cache import SimpleCache
 from prot.prompt.filters import FilterOrBool, Never, to_filter
 from prot.prompt.keys import KEY_ALIASES, Keys
 
 # Avoid circular imports.
 if TYPE_CHECKING:
```

### Comparing `prot-3.9.0/src/prot/prompt/key_binding/key_processor.py` & `prot-3.9.1/src/prot/prompt/key_binding/key_processor.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/key_binding/vi_state.py` & `prot-3.9.1/src/prot/prompt/key_binding/vi_state.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
 from typing import TYPE_CHECKING, Callable, Dict, Optional
 
 from prot.prompt.clipboard import ClipboardData
 
 if TYPE_CHECKING:
-    from .key_processor import KeyPressEvent
     from .bindings.vi import TextObject
+    from .key_processor import KeyPressEvent
 
 __all__ = [
     "InputMode",
     "CharacterFind",
     "ViState",
 ]
```

### Comparing `prot-3.9.0/src/prot/prompt/keys.py` & `prot-3.9.1/src/prot/prompt/keys.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/layout/__init__.py` & `prot-3.9.1/src/prot/prompt/layout/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,58 +40,27 @@
 - ValidationToolbar (Shows validation errors of the current buffer.)
 
 And one prepared menu:
 
 - CompletionsMenu
 
 """
-from .containers import (
-    ColorColumn,
-    ConditionalContainer,
-    Container,
-    DynamicContainer,
-    Float,
-    FloatContainer,
-    HorizontalAlign,
-    HSplit,
-    ScrollOffsets,
-    VerticalAlign,
-    VSplit,
-    Window,
-    WindowAlign,
-    WindowRenderInfo,
-    is_container,
-    to_container,
-    to_window,
-)
-from .controls import (
-    BufferControl,
-    DummyControl,
-    FormattedTextControl,
-    SearchBufferControl,
-    UIContent,
-    UIControl,
-)
-from .dimension import (
-    AnyDimension,
-    D,
-    Dimension,
-    is_dimension,
-    max_layout_dimensions,
-    sum_layout_dimensions,
-    to_dimension,
-)
+from .containers import (ColorColumn, ConditionalContainer, Container,
+                         DynamicContainer, Float, FloatContainer,
+                         HorizontalAlign, HSplit, ScrollOffsets, VerticalAlign,
+                         VSplit, Window, WindowAlign, WindowRenderInfo,
+                         is_container, to_container, to_window)
+from .controls import (BufferControl, DummyControl, FormattedTextControl,
+                       SearchBufferControl, UIContent, UIControl)
+from .dimension import (AnyDimension, D, Dimension, is_dimension,
+                        max_layout_dimensions, sum_layout_dimensions,
+                        to_dimension)
 from .layout import InvalidLayoutError, Layout, walk
-from .margins import (
-    ConditionalMargin,
-    Margin,
-    NumberedMargin,
-    PromptMargin,
-    ScrollbarMargin,
-)
+from .margins import (ConditionalMargin, Margin, NumberedMargin, PromptMargin,
+                      ScrollbarMargin)
 from .menus import CompletionsMenu, MultiColumnCompletionsMenu
 
 __all__ = [
     # Layout.
     "Layout",
     "InvalidLayoutError",
     "walk",
```

### Comparing `prot-3.9.0/src/prot/prompt/layout/containers.py` & `prot-3.9.1/src/prot/prompt/layout/containers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,62 +1,34 @@
 """
 Container for the layout.
 (Containers can contain other containers or user interface controls.)
 """
 from abc import ABCMeta, abstractmethod
 from enum import Enum
 from functools import partial
-from typing import (
-    TYPE_CHECKING,
-    Callable,
-    Dict,
-    List,
-    Optional,
-    Sequence,
-    Tuple,
-    Union,
-    cast,
-)
+from typing import (TYPE_CHECKING, Callable, Dict, List, Optional, Sequence,
+                    Tuple, Union, cast)
 
 from prot.prompt.application.current import get_app
 from prot.prompt.cache import SimpleCache
 from prot.prompt.data_structures import Point
-from prot.prompt.filters import (
-    FilterOrBool,
-    emacs_insert_mode,
-    to_filter,
-    vi_insert_mode,
-)
-from prot.prompt.formatted_text import (
-    AnyFormattedText,
-    StyleAndTextTuples,
-    to_formatted_text,
-)
-from prot.prompt.formatted_text.utils import (
-    fragment_list_to_text,
-    fragment_list_width,
-)
+from prot.prompt.filters import (FilterOrBool, emacs_insert_mode, to_filter,
+                                 vi_insert_mode)
+from prot.prompt.formatted_text import (AnyFormattedText, StyleAndTextTuples,
+                                        to_formatted_text)
+from prot.prompt.formatted_text.utils import (fragment_list_to_text,
+                                              fragment_list_width)
 from prot.prompt.key_binding import KeyBindingsBase
 from prot.prompt.mouse_events import MouseEvent, MouseEventType
 from prot.prompt.utils import get_cwidth, take_using_weights, to_int, to_str
 
-from .controls import (
-    DummyControl,
-    FormattedTextControl,
-    GetLinePrefixCallable,
-    UIContent,
-    UIControl,
-)
-from .dimension import (
-    AnyDimension,
-    Dimension,
-    max_layout_dimensions,
-    sum_layout_dimensions,
-    to_dimension,
-)
+from .controls import (DummyControl, FormattedTextControl,
+                       GetLinePrefixCallable, UIContent, UIControl)
+from .dimension import (AnyDimension, Dimension, max_layout_dimensions,
+                        sum_layout_dimensions, to_dimension)
 from .margins import Margin
 from .mouse_handlers import MouseHandlers
 from .screen import _CHAR_CACHE, Screen, WritePosition
 from .utils import explode_text_fragments
 
 if TYPE_CHECKING:
     from typing_extensions import Protocol
```

### Comparing `prot-3.9.0/src/prot/prompt/layout/controls.py` & `prot-3.9.1/src/prot/prompt/layout/controls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,55 +1,35 @@
 """
 User interface Controls for the layout.
 """
 import time
 from abc import ABCMeta, abstractmethod
-from typing import (
-    TYPE_CHECKING,
-    Callable,
-    Dict,
-    Hashable,
-    Iterable,
-    List,
-    NamedTuple,
-    Optional,
-    Union,
-)
+from typing import (TYPE_CHECKING, Callable, Dict, Hashable, Iterable, List,
+                    NamedTuple, Optional, Union)
 
 from prot.prompt.application.current import get_app
 from prot.prompt.buffer import Buffer
 from prot.prompt.cache import SimpleCache
 from prot.prompt.data_structures import Point
 from prot.prompt.document import Document
 from prot.prompt.filters import FilterOrBool, to_filter
-from prot.prompt.formatted_text import (
-    AnyFormattedText,
-    StyleAndTextTuples,
-    to_formatted_text,
-)
-from prot.prompt.formatted_text.utils import (
-    fragment_list_to_text,
-    fragment_list_width,
-    split_lines,
-)
+from prot.prompt.formatted_text import (AnyFormattedText, StyleAndTextTuples,
+                                        to_formatted_text)
+from prot.prompt.formatted_text.utils import (fragment_list_to_text,
+                                              fragment_list_width, split_lines)
 from prot.prompt.lexers import Lexer, SimpleLexer
 from prot.prompt.mouse_events import MouseEvent, MouseEventType
 from prot.prompt.search import SearchState
 from prot.prompt.selection import SelectionType
 from prot.prompt.utils import get_cwidth
 
-from .processors import (
-    DisplayMultipleCursors,
-    HighlightIncrementalSearchProcessor,
-    HighlightSearchProcessor,
-    HighlightSelectionProcessor,
-    Processor,
-    TransformationInput,
-    merge_processors,
-)
+from .processors import (DisplayMultipleCursors,
+                         HighlightIncrementalSearchProcessor,
+                         HighlightSearchProcessor, HighlightSelectionProcessor,
+                         Processor, TransformationInput, merge_processors)
 
 if TYPE_CHECKING:
     from prot.prompt.key_binding.key_bindings import KeyBindingsBase
     from prot.prompt.utils import Event
 
     # The only two return values for a mouse hander are `None` and
     # `NotImplemented`. For the type checker it's best to annotate this as
```

### Comparing `prot-3.9.0/src/prot/prompt/layout/dimension.py` & `prot-3.9.1/src/prot/prompt/layout/dimension.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/layout/dummy.py` & `prot-3.9.1/src/prot/prompt/layout/dummy.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/layout/layout.py` & `prot-3.9.1/src/prot/prompt/layout/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 """
 Wrapper for the layout.
 """
 from typing import Dict, Generator, Iterable, List, Optional, Union
 
 from prot.prompt.buffer import Buffer
 
-from .containers import (
-    AnyContainer,
-    ConditionalContainer,
-    Container,
-    Window,
-    to_container,
-)
+from .containers import (AnyContainer, ConditionalContainer, Container, Window,
+                         to_container)
 from .controls import BufferControl, SearchBufferControl, UIControl
 
 __all__ = [
     "Layout",
     "InvalidLayoutError",
     "walk",
 ]
```

### Comparing `prot-3.9.0/src/prot/prompt/layout/margins.py` & `prot-3.9.1/src/prot/prompt/layout/margins.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """
 Margin implementations for a :class:`~prompt_toolkit.layout.containers.Window`.
 """
 from abc import ABCMeta, abstractmethod
 from typing import TYPE_CHECKING, Callable, Optional
 
 from prot.prompt.filters import FilterOrBool, to_filter
-from prot.prompt.formatted_text import (
-    StyleAndTextTuples,
-    fragment_list_to_text,
-    to_formatted_text,
-)
+from prot.prompt.formatted_text import (StyleAndTextTuples,
+                                        fragment_list_to_text,
+                                        to_formatted_text)
 from prot.prompt.utils import get_cwidth
 
 from .controls import UIContent
 
 if TYPE_CHECKING:
     from .containers import WindowRenderInfo
```

### Comparing `prot-3.9.0/src/prot/prompt/layout/menus.py` & `prot-3.9.1/src/prot/prompt/layout/menus.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,20 @@
 import math
 from itertools import zip_longest
-from typing import (
-    TYPE_CHECKING,
-    Callable,
-    Dict,
-    Iterable,
-    List,
-    Optional,
-    Tuple,
-    TypeVar,
-    Union,
-    cast,
-)
+from typing import (TYPE_CHECKING, Callable, Dict, Iterable, List, Optional,
+                    Tuple, TypeVar, Union, cast)
 
 from prot.prompt.application.current import get_app
 from prot.prompt.buffer import CompletionState
 from prot.prompt.completion import Completion
 from prot.prompt.data_structures import Point
-from prot.prompt.filters import (
-    Condition,
-    FilterOrBool,
-    has_completions,
-    is_done,
-    to_filter,
-)
-from prot.prompt.formatted_text import (
-    StyleAndTextTuples,
-    fragment_list_width,
-    to_formatted_text,
-)
+from prot.prompt.filters import (Condition, FilterOrBool, has_completions,
+                                 is_done, to_filter)
+from prot.prompt.formatted_text import (StyleAndTextTuples,
+                                        fragment_list_width, to_formatted_text)
 from prot.prompt.key_binding.key_processor import KeyPressEvent
 from prot.prompt.layout.utils import explode_text_fragments
 from prot.prompt.mouse_events import MouseEvent, MouseEventType
 from prot.prompt.utils import get_cwidth
 
 from .containers import ConditionalContainer, HSplit, ScrollOffsets, Window
 from .controls import GetLinePrefixCallable, UIContent, UIControl
```

### Comparing `prot-3.9.0/src/prot/prompt/layout/mouse_handlers.py` & `prot-3.9.1/src/prot/prompt/layout/mouse_handlers.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/layout/processors.py` & `prot-3.9.1/src/prot/prompt/layout/processors.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,36 +3,26 @@
 from a buffer before the BufferControl will render it to the screen.
 
 They can insert fragments before or after, or highlight fragments by replacing the
 fragment types.
 """
 import re
 from abc import ABCMeta, abstractmethod
-from typing import (
-    TYPE_CHECKING,
-    Callable,
-    Hashable,
-    List,
-    Optional,
-    Tuple,
-    Type,
-    Union,
-    cast,
-)
+from typing import (TYPE_CHECKING, Callable, Hashable, List, Optional, Tuple,
+                    Type, Union, cast)
 
 from prot.prompt.application.current import get_app
 from prot.prompt.cache import SimpleCache
 from prot.prompt.document import Document
-from prot.prompt.filters import FilterOrBool, to_filter, vi_insert_multiple_mode
-from prot.prompt.formatted_text import (
-    AnyFormattedText,
-    StyleAndTextTuples,
-    to_formatted_text,
-)
-from prot.prompt.formatted_text.utils import fragment_list_len, fragment_list_to_text
+from prot.prompt.filters import (FilterOrBool, to_filter,
+                                 vi_insert_multiple_mode)
+from prot.prompt.formatted_text import (AnyFormattedText, StyleAndTextTuples,
+                                        to_formatted_text)
+from prot.prompt.formatted_text.utils import (fragment_list_len,
+                                              fragment_list_to_text)
 from prot.prompt.search import SearchDirection
 from prot.prompt.utils import to_int, to_str
 
 from .utils import explode_text_fragments
 
 if TYPE_CHECKING:
     from .controls import BufferControl, UIContent
```

### Comparing `prot-3.9.0/src/prot/prompt/layout/screen.py` & `prot-3.9.1/src/prot/prompt/layout/screen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import defaultdict
-from typing import TYPE_CHECKING, Callable, DefaultDict, Dict, List, Optional, Tuple
+from typing import (TYPE_CHECKING, Callable, DefaultDict, Dict, List, Optional,
+                    Tuple)
 
 from prot.prompt.cache import FastDictCache
 from prot.prompt.data_structures import Point
 from prot.prompt.utils import get_cwidth
 
 if TYPE_CHECKING:
     from .containers import Window
```

### Comparing `prot-3.9.0/src/prot/prompt/layout/utils.py` & `prot-3.9.1/src/prot/prompt/layout/utils.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/lexers/base.py` & `prot-3.9.1/src/prot/prompt/lexers/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/lexers/pygments.py` & `prot-3.9.1/src/prot/prompt/lexers/pygments.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,24 +2,16 @@
 Adaptor classes for using Pygments lexers within prompt_toolkit.
 
 This includes syntax synchronization code, so that we don't have to start
 lexing at the beginning of a document, when displaying a very large text.
 """
 import re
 from abc import ABCMeta, abstractmethod
-from typing import (
-    TYPE_CHECKING,
-    Callable,
-    Dict,
-    Generator,
-    Iterable,
-    Optional,
-    Tuple,
-    Type,
-)
+from typing import (TYPE_CHECKING, Callable, Dict, Generator, Iterable,
+                    Optional, Tuple, Type)
 
 from prot.prompt.document import Document
 from prot.prompt.filters import FilterOrBool, to_filter
 from prot.prompt.formatted_text.base import StyleAndTextTuples
 from prot.prompt.formatted_text.utils import split_lines
 from prot.prompt.styles.pygments import pygments_token_to_classname
 
@@ -206,16 +198,16 @@
     def from_filename(
         cls, filename: str, sync_from_start: FilterOrBool = True
     ) -> "Lexer":
         """
         Create a `Lexer` from a filename.
         """
         # Inline imports: the Pygments dependency is optional!
-        from pygments.util import ClassNotFound
         from pygments.lexers import get_lexer_for_filename
+        from pygments.util import ClassNotFound
 
         try:
             pygments_lexer = get_lexer_for_filename(filename)
         except ClassNotFound:
             return SimpleLexer()
         else:
             return cls(pygments_lexer.__class__, sync_from_start=sync_from_start)
```

### Comparing `prot-3.9.0/src/prot/prompt/mouse_events.py` & `prot-3.9.1/src/prot/prompt/mouse_events.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/output/base.py` & `prot-3.9.1/src/prot/prompt/output/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/output/color_depth.py` & `prot-3.9.1/src/prot/prompt/output/color_depth.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/output/conemu.py` & `prot-3.9.1/src/prot/prompt/output/conemu.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/output/defaults.py` & `prot-3.9.1/src/prot/prompt/output/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import sys
 from typing import Optional, TextIO, cast
 
 from prot.prompt.patch_stdout import StdoutProxy
-from prot.prompt.utils import (
-    get_term_environment_variable,
-    is_conemu_ansi,
-    is_windows,
-)
+from prot.prompt.utils import (get_term_environment_variable, is_conemu_ansi,
+                               is_windows)
 
 from .base import Output
 
 __all__ = [
     "create_output",
 ]
 
@@ -44,15 +41,15 @@
     # the real stdout.
     while isinstance(stdout, StdoutProxy):
         stdout = stdout.original_stdout
 
     if is_windows():
         from .conemu import ConEmuOutput
         from .win32 import Win32Output
-        from .windows10 import is_win_vt100_enabled, Windows10_Output
+        from .windows10 import Windows10_Output, is_win_vt100_enabled
 
         if is_win_vt100_enabled():
             return cast(Output, Windows10_Output(stdout))
         if is_conemu_ansi():
             return cast(Output, ConEmuOutput(stdout))
         else:
             return Win32Output(stdout)
```

### Comparing `prot-3.9.0/src/prot/prompt/output/vt100.py` & `prot-3.9.1/src/prot/prompt/output/vt100.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,27 +5,16 @@
 (We don't rely on Pygments anymore, because many things are very custom, and
 everything has been highly optimized.)
 http://pygments.org/
 """
 import array
 import errno
 import sys
-from typing import (
-    IO,
-    Callable,
-    Dict,
-    Hashable,
-    Iterable,
-    List,
-    Optional,
-    Sequence,
-    Set,
-    TextIO,
-    Tuple,
-)
+from typing import (IO, Callable, Dict, Hashable, Iterable, List, Optional,
+                    Sequence, Set, TextIO, Tuple)
 
 from prot.prompt.data_structures import Size
 from prot.prompt.output import Output
 from prot.prompt.styles import ANSI_COLOR_NAMES, Attrs
 
 from .color_depth import ColorDepth
```

### Comparing `prot-3.9.0/src/prot/prompt/output/win32.py` & `prot-3.9.1/src/prot/prompt/output/win32.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,20 @@
 import os
-from ctypes import (
-    ArgumentError,
-    byref,
-    c_char,
-    c_long,
-    c_uint,
-    c_ulong,
-    pointer,
-    windll,
-)
+from ctypes import (ArgumentError, byref, c_char, c_long, c_uint, c_ulong,
+                    pointer, windll)
 from ctypes.wintypes import DWORD, HANDLE
 from typing import Dict, List, TextIO, Tuple
 
 from prot.prompt.data_structures import Size
 from prot.prompt.renderer import Output
 from prot.prompt.styles import ANSI_COLOR_NAMES, Attrs
 from prot.prompt.utils import get_cwidth
-from prot.prompt.win32_types import (
-    CONSOLE_SCREEN_BUFFER_INFO,
-    COORD,
-    SMALL_RECT,
-    STD_INPUT_HANDLE,
-    STD_OUTPUT_HANDLE,
-)
+from prot.prompt.win32_types import (CONSOLE_SCREEN_BUFFER_INFO, COORD,
+                                     SMALL_RECT, STD_INPUT_HANDLE,
+                                     STD_OUTPUT_HANDLE)
 
 from .color_depth import ColorDepth
 
 __all__ = [
     "Win32Output",
 ]
```

### Comparing `prot-3.9.0/src/prot/prompt/output/windows10.py` & `prot-3.9.1/src/prot/prompt/output/windows10.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/patch_stdout.py` & `prot-3.9.1/src/prot/prompt/patch_stdout.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/renderer.py` & `prot-3.9.1/src/prot/prompt/renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """
 Renders the command line on the console.
 (Redraws parts of the input line that were changed.)
 """
 from asyncio import FIRST_COMPLETED, Future, sleep, wait
 from collections import deque
 from enum import Enum
-from typing import TYPE_CHECKING, Any, Callable, Deque, Dict, Hashable, Optional, Tuple
+from typing import (TYPE_CHECKING, Any, Callable, Deque, Dict, Hashable,
+                    Optional, Tuple)
 
 from prot.prompt.application.current import get_app
 from prot.prompt.data_structures import Point, Size
 from prot.prompt.filters import FilterOrBool, to_filter
 from prot.prompt.formatted_text import AnyFormattedText, to_formatted_text
 from prot.prompt.input.base import Input
 from prot.prompt.layout.mouse_handlers import MouseHandlers
 from prot.prompt.layout.screen import Char, Screen, WritePosition
 from prot.prompt.output import ColorDepth, Output
-from prot.prompt.styles import (
-    Attrs,
-    BaseStyle,
-    DummyStyleTransformation,
-    StyleTransformation,
-)
+from prot.prompt.styles import (Attrs, BaseStyle, DummyStyleTransformation,
+                                StyleTransformation)
 from prot.prompt.utils import is_windows
 
 if TYPE_CHECKING:
     from prot.prompt.application import Application
     from prot.prompt.layout.layout import Layout
```

### Comparing `prot-3.9.0/src/prot/prompt/search.py` & `prot-3.9.1/src/prot/prompt/search.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/selection.py` & `prot-3.9.1/src/prot/prompt/selection.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/shortcuts/__init__.py` & `prot-3.9.1/src/prot/prompt/shortcuts/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,15 @@
-from .dialogs import (
-    button_dialog,
-    checkboxlist_dialog,
-    input_dialog,
-    message_dialog,
-    progress_dialog,
-    radiolist_dialog,
-    yes_no_dialog,
-)
+from .dialogs import (button_dialog, checkboxlist_dialog, input_dialog,
+                      message_dialog, progress_dialog, radiolist_dialog,
+                      yes_no_dialog)
 from .progress_bar import ProgressBar
-from .prompt import (
-    CompleteStyle,
-    PromptSession,
-    confirm,
-    create_confirm_session,
-    prompt,
-)
-from .utils import clear, clear_title, print_container, print_formatted_text, set_title
+from .prompt import (CompleteStyle, PromptSession, confirm,
+                     create_confirm_session, prompt)
+from .utils import (clear, clear_title, print_container, print_formatted_text,
+                    set_title)
 
 __all__ = [
     # Dialogs.
     "input_dialog",
     "message_dialog",
     "progress_dialog",
     "checkboxlist_dialog",
```

### Comparing `prot-3.9.0/src/prot/prompt/shortcuts/dialogs.py` & `prot-3.9.1/src/prot/prompt/shortcuts/dialogs.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,29 +7,22 @@
 from prot.prompt.buffer import Buffer
 from prot.prompt.completion import Completer
 from prot.prompt.eventloop import run_in_executor_with_context
 from prot.prompt.filters import FilterOrBool
 from prot.prompt.formatted_text import AnyFormattedText
 from prot.prompt.key_binding.bindings.focus import focus_next, focus_previous
 from prot.prompt.key_binding.defaults import load_key_bindings
-from prot.prompt.key_binding.key_bindings import KeyBindings, merge_key_bindings
+from prot.prompt.key_binding.key_bindings import (KeyBindings,
+                                                  merge_key_bindings)
 from prot.prompt.layout import Layout
 from prot.prompt.layout.containers import AnyContainer, HSplit
 from prot.prompt.layout.dimension import Dimension as D
 from prot.prompt.styles import BaseStyle
-from prot.prompt.widgets import (
-    Box,
-    Button,
-    CheckboxList,
-    Dialog,
-    Label,
-    ProgressBar,
-    RadioList,
-    TextArea,
-)
+from prot.prompt.widgets import (Box, Button, CheckboxList, Dialog, Label,
+                                 ProgressBar, RadioList, TextArea)
 
 __all__ = [
     "yes_no_dialog",
     "button_dialog",
     "input_dialog",
     "message_dialog",
     "radiolist_dialog",
```

### Comparing `prot-3.9.0/src/prot/prompt/shortcuts/progress_bar/base.py` & `prot-3.9.1/src/prot/prompt/shortcuts/progress_bar/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,61 +9,42 @@
 """
 import datetime
 import functools
 import os
 import signal
 import threading
 import traceback
-from prot import printMsg
 from asyncio import get_event_loop, new_event_loop, set_event_loop
-from typing import (
-    Generic,
-    Iterable,
-    List,
-    Optional,
-    Sequence,
-    Sized,
-    TextIO,
-    TypeVar,
-    cast,
-)
+from typing import (Generic, Iterable, List, Optional, Sequence, Sized, TextIO,
+                    TypeVar, cast)
 
+from prot import printMsg
 from prot.prompt.application import Application
 from prot.prompt.application.current import get_app_session
 from prot.prompt.filters import Condition, is_done, renderer_height_is_known
-from prot.prompt.formatted_text import (
-    AnyFormattedText,
-    StyleAndTextTuples,
-    to_formatted_text,
-)
+from prot.prompt.formatted_text import (AnyFormattedText, StyleAndTextTuples,
+                                        to_formatted_text)
 from prot.prompt.input import Input
 from prot.prompt.key_binding import KeyBindings
 from prot.prompt.key_binding.key_processor import KeyPressEvent
-from prot.prompt.layout import (
-    ConditionalContainer,
-    FormattedTextControl,
-    HSplit,
-    Layout,
-    VSplit,
-    Window,
-)
+from prot.prompt.layout import (ConditionalContainer, FormattedTextControl,
+                                HSplit, Layout, VSplit, Window)
 from prot.prompt.layout.controls import UIContent, UIControl
 from prot.prompt.layout.dimension import AnyDimension, D
 from prot.prompt.output import ColorDepth, Output
 from prot.prompt.styles import BaseStyle
 from prot.prompt.utils import in_main_thread
 
 from .formatters import Formatter, create_default_formatters
 
 try:
     import contextvars
 except ImportError:
-    from prot.prompt.eventloop import (  # type: ignore
-        dummy_contextvars as contextvars,
-    )
+    from prot.prompt.eventloop import \
+        dummy_contextvars as contextvars  # type: ignore
 
 
 __all__ = ["ProgressBar"]
 
 E = KeyPressEvent
```

### Comparing `prot-3.9.0/src/prot/prompt/shortcuts/progress_bar/formatters.py` & `prot-3.9.1/src/prot/prompt/shortcuts/progress_bar/formatters.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,16 @@
 Each progress bar consists of a list of these formatters.
 """
 import datetime
 import time
 from abc import ABCMeta, abstractmethod
 from typing import TYPE_CHECKING, List, Tuple
 
-from prot.prompt.formatted_text import (
-    HTML,
-    AnyFormattedText,
-    StyleAndTextTuples,
-    to_formatted_text,
-)
+from prot.prompt.formatted_text import (HTML, AnyFormattedText,
+                                        StyleAndTextTuples, to_formatted_text)
 from prot.prompt.formatted_text.utils import fragment_list_width
 from prot.prompt.layout.dimension import AnyDimension, D
 from prot.prompt.layout.utils import explode_text_fragments
 from prot.prompt.utils import get_cwidth
 
 if TYPE_CHECKING:
     from .base import ProgressBar, ProgressBarCounter
```

### Comparing `prot-3.9.0/src/prot/prompt/shortcuts/prompt.py` & `prot-3.9.1/src/prot/prompt/shortcuts/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,115 +23,78 @@
         # Using a 'session'.
         s = PromptSession()
         result = s.prompt('Say something: ')
 """
 from asyncio import get_event_loop
 from enum import Enum
 from functools import partial
-from typing import (
-    TYPE_CHECKING,
-    Callable,
-    Generic,
-    List,
-    Optional,
-    Tuple,
-    TypeVar,
-    Union,
-    cast,
-)
+from typing import (TYPE_CHECKING, Callable, Generic, List, Optional, Tuple,
+                    TypeVar, Union, cast)
 
 from prot.prompt.application import Application
 from prot.prompt.application.current import get_app
 from prot.prompt.auto_suggest import AutoSuggest, DynamicAutoSuggest
 from prot.prompt.buffer import Buffer
-from prot.prompt.clipboard import Clipboard, DynamicClipboard, InMemoryClipboard
-from prot.prompt.completion import Completer, DynamicCompleter, ThreadedCompleter
+from prot.prompt.clipboard import (Clipboard, DynamicClipboard,
+                                   InMemoryClipboard)
+from prot.prompt.completion import (Completer, DynamicCompleter,
+                                    ThreadedCompleter)
 from prot.prompt.document import Document
 from prot.prompt.enums import DEFAULT_BUFFER, SEARCH_BUFFER, EditingMode
-from prot.prompt.filters import (
-    Condition,
-    FilterOrBool,
-    has_arg,
-    has_focus,
-    is_done,
-    is_true,
-    renderer_height_is_known,
-    to_filter,
-)
-from prot.prompt.formatted_text import (
-    AnyFormattedText,
-    StyleAndTextTuples,
-    fragment_list_to_text,
-    merge_formatted_text,
-    to_formatted_text,
-)
+from prot.prompt.filters import (Condition, FilterOrBool, has_arg, has_focus,
+                                 is_done, is_true, renderer_height_is_known,
+                                 to_filter)
+from prot.prompt.formatted_text import (AnyFormattedText, StyleAndTextTuples,
+                                        fragment_list_to_text,
+                                        merge_formatted_text,
+                                        to_formatted_text)
 from prot.prompt.history import History, InMemoryHistory
 from prot.prompt.input.base import Input
-from prot.prompt.key_binding.bindings.auto_suggest import load_auto_suggest_bindings
-from prot.prompt.key_binding.bindings.completion import (
-    display_completions_like_readline,
-)
-from prot.prompt.key_binding.bindings.open_in_editor import (
-    load_open_in_editor_bindings,
-)
-from prot.prompt.key_binding.key_bindings import (
-    ConditionalKeyBindings,
-    DynamicKeyBindings,
-    KeyBindings,
-    KeyBindingsBase,
-    merge_key_bindings,
-)
+from prot.prompt.key_binding.bindings.auto_suggest import \
+    load_auto_suggest_bindings
+from prot.prompt.key_binding.bindings.completion import \
+    display_completions_like_readline
+from prot.prompt.key_binding.bindings.open_in_editor import \
+    load_open_in_editor_bindings
+from prot.prompt.key_binding.key_bindings import (ConditionalKeyBindings,
+                                                  DynamicKeyBindings,
+                                                  KeyBindings, KeyBindingsBase,
+                                                  merge_key_bindings)
 from prot.prompt.key_binding.key_processor import KeyPressEvent
 from prot.prompt.keys import Keys
 from prot.prompt.layout import Float, FloatContainer, HSplit, Window
 from prot.prompt.layout.containers import ConditionalContainer, WindowAlign
-from prot.prompt.layout.controls import (
-    BufferControl,
-    FormattedTextControl,
-    SearchBufferControl,
-)
+from prot.prompt.layout.controls import (BufferControl, FormattedTextControl,
+                                         SearchBufferControl)
 from prot.prompt.layout.dimension import Dimension
 from prot.prompt.layout.layout import Layout
-from prot.prompt.layout.menus import CompletionsMenu, MultiColumnCompletionsMenu
-from prot.prompt.layout.processors import (
-    AppendAutoSuggestion,
-    ConditionalProcessor,
-    DisplayMultipleCursors,
-    DynamicProcessor,
-    HighlightIncrementalSearchProcessor,
-    HighlightSelectionProcessor,
-    PasswordProcessor,
-    Processor,
-    ReverseSearchProcessor,
-    merge_processors,
-)
+from prot.prompt.layout.menus import (CompletionsMenu,
+                                      MultiColumnCompletionsMenu)
+from prot.prompt.layout.processors import (AppendAutoSuggestion,
+                                           ConditionalProcessor,
+                                           DisplayMultipleCursors,
+                                           DynamicProcessor,
+                                           HighlightIncrementalSearchProcessor,
+                                           HighlightSelectionProcessor,
+                                           PasswordProcessor, Processor,
+                                           ReverseSearchProcessor,
+                                           merge_processors)
 from prot.prompt.layout.utils import explode_text_fragments
 from prot.prompt.lexers import DynamicLexer, Lexer
 from prot.prompt.output import ColorDepth, DummyOutput, Output
-from prot.prompt.styles import (
-    BaseStyle,
-    ConditionalStyleTransformation,
-    DynamicStyle,
-    DynamicStyleTransformation,
-    StyleTransformation,
-    SwapLightAndDarkStyleTransformation,
-    merge_style_transformations,
-)
-from prot.prompt.utils import (
-    get_cwidth,
-    is_dumb_terminal,
-    suspend_to_background_supported,
-    to_str,
-)
+from prot.prompt.styles import (BaseStyle, ConditionalStyleTransformation,
+                                DynamicStyle, DynamicStyleTransformation,
+                                StyleTransformation,
+                                SwapLightAndDarkStyleTransformation,
+                                merge_style_transformations)
+from prot.prompt.utils import (get_cwidth, is_dumb_terminal,
+                               suspend_to_background_supported, to_str)
 from prot.prompt.validation import DynamicValidator, Validator
-from prot.prompt.widgets.toolbars import (
-    SearchToolbar,
-    SystemToolbar,
-    ValidationToolbar,
-)
+from prot.prompt.widgets.toolbars import (SearchToolbar, SystemToolbar,
+                                          ValidationToolbar)
 
 if TYPE_CHECKING:
     from prot.prompt.formatted_text.base import MagicFormattedText
 
 __all__ = [
     "PromptSession",
     "prompt",
```

### Comparing `prot-3.9.0/src/prot/prompt/shortcuts/utils.py` & `prot-3.9.1/src/prot/prompt/shortcuts/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 from asyncio import get_event_loop
 from typing import TYPE_CHECKING, Any, Optional, TextIO
 
 from prot.prompt.application import Application
 from prot.prompt.application.current import get_app_session
-from prot.prompt.formatted_text import (
-    FormattedText,
-    StyleAndTextTuples,
-    to_formatted_text,
-)
+from prot.prompt.formatted_text import (FormattedText, StyleAndTextTuples,
+                                        to_formatted_text)
 from prot.prompt.input import DummyInput
 from prot.prompt.layout import Layout
 from prot.prompt.output import ColorDepth, Output
 from prot.prompt.output.defaults import create_output
-from prot.prompt.renderer import (
-    print_formatted_text as renderer_print_formatted_text,
-)
-from prot.prompt.styles import (
-    BaseStyle,
-    StyleTransformation,
-    default_pygments_style,
-    default_ui_style,
-    merge_styles,
-)
+from prot.prompt.renderer import \
+    print_formatted_text as renderer_print_formatted_text
+from prot.prompt.styles import (BaseStyle, StyleTransformation,
+                                default_pygments_style, default_ui_style,
+                                merge_styles)
 
 if TYPE_CHECKING:
     from prot.prompt.layout.containers import Container
 
 __all__ = [
     "print_formatted_text",
     "print_container",
```

### Comparing `prot-3.9.0/src/prot/prompt/styles/__init__.py` & `prot-3.9.1/src/prot/prompt/styles/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,26 @@
 """
 Styling for prompt_toolkit applications.
 """
-from .base import (
-    ANSI_COLOR_NAMES,
-    DEFAULT_ATTRS,
-    Attrs,
-    BaseStyle,
-    DummyStyle,
-    DynamicStyle,
-)
+from .base import (ANSI_COLOR_NAMES, DEFAULT_ATTRS, Attrs, BaseStyle,
+                   DummyStyle, DynamicStyle)
 from .defaults import default_pygments_style, default_ui_style
 from .named_colors import NAMED_COLORS
-from .pygments import (
-    pygments_token_to_classname,
-    style_from_pygments_cls,
-    style_from_pygments_dict,
-)
+from .pygments import (pygments_token_to_classname, style_from_pygments_cls,
+                       style_from_pygments_dict)
 from .style import Priority, Style, merge_styles, parse_color
-from .style_transformation import (
-    AdjustBrightnessStyleTransformation,
-    ConditionalStyleTransformation,
-    DummyStyleTransformation,
-    DynamicStyleTransformation,
-    ReverseStyleTransformation,
-    SetDefaultColorStyleTransformation,
-    StyleTransformation,
-    SwapLightAndDarkStyleTransformation,
-    merge_style_transformations,
-)
+from .style_transformation import (AdjustBrightnessStyleTransformation,
+                                   ConditionalStyleTransformation,
+                                   DummyStyleTransformation,
+                                   DynamicStyleTransformation,
+                                   ReverseStyleTransformation,
+                                   SetDefaultColorStyleTransformation,
+                                   StyleTransformation,
+                                   SwapLightAndDarkStyleTransformation,
+                                   merge_style_transformations)
 
 __all__ = [
     # Base.
     "Attrs",
     "DEFAULT_ATTRS",
     "ANSI_COLOR_NAMES",
     "BaseStyle",
```

### Comparing `prot-3.9.0/src/prot/prompt/styles/base.py` & `prot-3.9.1/src/prot/prompt/styles/base.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/styles/defaults.py` & `prot-3.9.1/src/prot/prompt/styles/defaults.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/styles/named_colors.py` & `prot-3.9.1/src/prot/prompt/styles/named_colors.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/styles/pygments.py` & `prot-3.9.1/src/prot/prompt/styles/pygments.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     style = style_from_pygments_cls(pygments_style_cls=TangoStyle)
 """
 from typing import TYPE_CHECKING, Dict, Type
 
 from .style import Style
 
 if TYPE_CHECKING:
-    from pygments.token import Token
     from pygments.style import Style as PygmentsStyle
+    from pygments.token import Token
 
 
 __all__ = [
     "style_from_pygments_cls",
     "style_from_pygments_dict",
     "pygments_token_to_classname",
 ]
```

### Comparing `prot-3.9.0/src/prot/prompt/styles/style.py` & `prot-3.9.1/src/prot/prompt/styles/style.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,16 @@
 import re
 import sys
 from enum import Enum
 from typing import Dict, Hashable, List, Set, Tuple, TypeVar
 
 from prot.prompt.cache import SimpleCache
 
-from .base import (
-    ANSI_COLOR_NAMES,
-    ANSI_COLOR_NAMES_ALIASES,
-    DEFAULT_ATTRS,
-    Attrs,
-    BaseStyle,
-)
+from .base import (ANSI_COLOR_NAMES, ANSI_COLOR_NAMES_ALIASES, DEFAULT_ATTRS,
+                   Attrs, BaseStyle)
 from .named_colors import NAMED_COLORS
 
 __all__ = [
     "Style",
     "parse_color",
     "Priority",
     "merge_styles",
```

### Comparing `prot-3.9.0/src/prot/prompt/styles/style_transformation.py` & `prot-3.9.1/src/prot/prompt/styles/style_transformation.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/utils.py` & `prot-3.9.1/src/prot/prompt/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,14 @@
 import os
 import signal
 import sys
 import threading
 from collections import deque
-from typing import (
-    Callable,
-    ContextManager,
-    Deque,
-    Dict,
-    Generator,
-    Generic,
-    List,
-    Optional,
-    TypeVar,
-    Union,
-)
+from typing import (Callable, ContextManager, Deque, Dict, Generator, Generic,
+                    List, Optional, TypeVar, Union)
 
 from prot.wcwidth import wcwidth
 
 __all__ = [
     "Event",
     "DummyContext",
     "get_cwidth",
```

### Comparing `prot-3.9.0/src/prot/prompt/validation.py` & `prot-3.9.1/src/prot/prompt/validation.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/prompt/widgets/__init__.py` & `prot-3.9.1/src/prot/prompt/widgets/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,38 +2,21 @@
 Collection of reusable components for building full screen applications.
 These are higher level abstractions on top of the `prompt_toolkit.layout`
 module.
 
 Most of these widgets implement the ``__pt_container__`` method, which makes it
 possible to embed these in the layout like any other container.
 """
-from .base import (
-    Box,
-    Button,
-    Checkbox,
-    CheckboxList,
-    Frame,
-    HorizontalLine,
-    Label,
-    ProgressBar,
-    RadioList,
-    Shadow,
-    TextArea,
-    VerticalLine,
-)
+from .base import (Box, Button, Checkbox, CheckboxList, Frame, HorizontalLine,
+                   Label, ProgressBar, RadioList, Shadow, TextArea,
+                   VerticalLine)
 from .dialogs import Dialog
 from .menus import MenuContainer, MenuItem
-from .toolbars import (
-    ArgToolbar,
-    CompletionsToolbar,
-    FormattedTextToolbar,
-    SearchToolbar,
-    SystemToolbar,
-    ValidationToolbar,
-)
+from .toolbars import (ArgToolbar, CompletionsToolbar, FormattedTextToolbar,
+                       SearchToolbar, SystemToolbar, ValidationToolbar)
 
 __all__ = [
     # Base.
     "TextArea",
     "Label",
     "Button",
     "Frame",
```

### Comparing `prot-3.9.0/src/prot/prompt/widgets/base.py` & `prot-3.9.1/src/prot/prompt/widgets/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,68 +9,44 @@
 
     At this point, the API for these widgets is considered unstable, and can
     potentially change between minor releases (we try not too, but no
     guarantees are made yet). The public API in
     `prompt_toolkit.shortcuts.dialogs` on the other hand is considered stable.
 """
 from functools import partial
-from typing import Callable, Generic, List, Optional, Sequence, Tuple, TypeVar, Union
+from typing import (Callable, Generic, List, Optional, Sequence, Tuple,
+                    TypeVar, Union)
 
 from prot.prompt.application.current import get_app
 from prot.prompt.auto_suggest import AutoSuggest, DynamicAutoSuggest
 from prot.prompt.buffer import Buffer, BufferAcceptHandler
 from prot.prompt.completion import Completer, DynamicCompleter
 from prot.prompt.document import Document
-from prot.prompt.filters import (
-    Condition,
-    FilterOrBool,
-    has_focus,
-    is_done,
-    is_true,
-    to_filter,
-)
-from prot.prompt.formatted_text import (
-    AnyFormattedText,
-    StyleAndTextTuples,
-    Template,
-    to_formatted_text,
-)
+from prot.prompt.filters import (Condition, FilterOrBool, has_focus, is_done,
+                                 is_true, to_filter)
+from prot.prompt.formatted_text import (AnyFormattedText, StyleAndTextTuples,
+                                        Template, to_formatted_text)
 from prot.prompt.formatted_text.utils import fragment_list_to_text
 from prot.prompt.history import History
 from prot.prompt.key_binding.key_bindings import KeyBindings
 from prot.prompt.key_binding.key_processor import KeyPressEvent
 from prot.prompt.keys import Keys
-from prot.prompt.layout.containers import (
-    AnyContainer,
-    ConditionalContainer,
-    Container,
-    DynamicContainer,
-    Float,
-    FloatContainer,
-    HSplit,
-    VSplit,
-    Window,
-    WindowAlign,
-)
-from prot.prompt.layout.controls import (
-    BufferControl,
-    FormattedTextControl,
-    GetLinePrefixCallable,
-)
+from prot.prompt.layout.containers import (AnyContainer, ConditionalContainer,
+                                           Container, DynamicContainer, Float,
+                                           FloatContainer, HSplit, VSplit,
+                                           Window, WindowAlign)
+from prot.prompt.layout.controls import (BufferControl, FormattedTextControl,
+                                         GetLinePrefixCallable)
 from prot.prompt.layout.dimension import AnyDimension
 from prot.prompt.layout.dimension import Dimension as D
 from prot.prompt.layout.dimension import to_dimension
 from prot.prompt.layout.margins import NumberedMargin, ScrollbarMargin
-from prot.prompt.layout.processors import (
-    AppendAutoSuggestion,
-    BeforeInput,
-    ConditionalProcessor,
-    PasswordProcessor,
-    Processor,
-)
+from prot.prompt.layout.processors import (AppendAutoSuggestion, BeforeInput,
+                                           ConditionalProcessor,
+                                           PasswordProcessor, Processor)
 from prot.prompt.lexers import DynamicLexer, Lexer
 from prot.prompt.mouse_events import MouseEvent, MouseEventType
 from prot.prompt.utils import get_cwidth
 
 from .toolbars import SearchToolbar
 
 __all__ = [
```

### Comparing `prot-3.9.0/src/prot/prompt/widgets/dialogs.py` & `prot-3.9.1/src/prot/prompt/widgets/dialogs.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,16 @@
 """
 from typing import Optional, Sequence, Union
 
 from prot.prompt.filters import has_completions, has_focus
 from prot.prompt.formatted_text import AnyFormattedText
 from prot.prompt.key_binding.bindings.focus import focus_next, focus_previous
 from prot.prompt.key_binding.key_bindings import KeyBindings
-from prot.prompt.layout.containers import (
-    AnyContainer,
-    DynamicContainer,
-    HSplit,
-    VSplit,
-)
+from prot.prompt.layout.containers import (AnyContainer, DynamicContainer,
+                                           HSplit, VSplit)
 from prot.prompt.layout.dimension import AnyDimension
 from prot.prompt.layout.dimension import Dimension as D
 
 from .base import Box, Button, Frame, Shadow
 
 __all__ = [
     "Dialog",
```

### Comparing `prot-3.9.0/src/prot/prompt/widgets/menus.py` & `prot-3.9.1/src/prot/prompt/widgets/menus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 from typing import Callable, Iterable, List, Optional, Sequence, Union
 
 from prot.prompt.application.current import get_app
 from prot.prompt.filters import Condition
-from prot.prompt.formatted_text.base import OneStyleAndTextTuple, StyleAndTextTuples
+from prot.prompt.formatted_text.base import (OneStyleAndTextTuple,
+                                             StyleAndTextTuples)
 from prot.prompt.key_binding.key_bindings import KeyBindings, KeyBindingsBase
 from prot.prompt.key_binding.key_processor import KeyPressEvent
 from prot.prompt.keys import Keys
-from prot.prompt.layout.containers import (
-    AnyContainer,
-    ConditionalContainer,
-    Container,
-    Float,
-    FloatContainer,
-    HSplit,
-    Window,
-)
+from prot.prompt.layout.containers import (AnyContainer, ConditionalContainer,
+                                           Container, Float, FloatContainer,
+                                           HSplit, Window)
 from prot.prompt.layout.controls import FormattedTextControl
 from prot.prompt.mouse_events import MouseEvent, MouseEventType
 from prot.prompt.utils import get_cwidth
 from prot.prompt.widgets import Shadow
 
 from .base import Border
```

### Comparing `prot-3.9.0/src/prot/prompt/widgets/toolbars.py` & `prot-3.9.1/src/prot/prompt/widgets/toolbars.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,29 @@
 from typing import Optional
 
 from prot.prompt.application.current import get_app
 from prot.prompt.buffer import Buffer
 from prot.prompt.enums import SYSTEM_BUFFER
-from prot.prompt.filters import (
-    Condition,
-    FilterOrBool,
-    emacs_mode,
-    has_arg,
-    has_completions,
-    has_focus,
-    has_validation_error,
-    to_filter,
-    vi_mode,
-    vi_navigation_mode,
-)
-from prot.prompt.formatted_text import (
-    AnyFormattedText,
-    StyleAndTextTuples,
-    fragment_list_len,
-    to_formatted_text,
-)
-from prot.prompt.key_binding.key_bindings import (
-    ConditionalKeyBindings,
-    KeyBindings,
-    KeyBindingsBase,
-    merge_key_bindings,
-)
+from prot.prompt.filters import (Condition, FilterOrBool, emacs_mode, has_arg,
+                                 has_completions, has_focus,
+                                 has_validation_error, to_filter, vi_mode,
+                                 vi_navigation_mode)
+from prot.prompt.formatted_text import (AnyFormattedText, StyleAndTextTuples,
+                                        fragment_list_len, to_formatted_text)
+from prot.prompt.key_binding.key_bindings import (ConditionalKeyBindings,
+                                                  KeyBindings, KeyBindingsBase,
+                                                  merge_key_bindings)
 from prot.prompt.key_binding.key_processor import KeyPressEvent
 from prot.prompt.key_binding.vi_state import InputMode
 from prot.prompt.keys import Keys
-from prot.prompt.layout.containers import ConditionalContainer, Container, Window
-from prot.prompt.layout.controls import (
-    BufferControl,
-    FormattedTextControl,
-    SearchBufferControl,
-    UIContent,
-    UIControl,
-)
+from prot.prompt.layout.containers import (ConditionalContainer, Container,
+                                           Window)
+from prot.prompt.layout.controls import (BufferControl, FormattedTextControl,
+                                         SearchBufferControl, UIContent,
+                                         UIControl)
 from prot.prompt.layout.dimension import Dimension
 from prot.prompt.layout.processors import BeforeInput
 from prot.prompt.lexers import SimpleLexer
 from prot.prompt.search import SearchDirection
 
 __all__ = [
     "ArgToolbar",
```

### Comparing `prot-3.9.0/src/prot/prompt/win32_types.py` & `prot-3.9.1/src/prot/prompt/win32_types.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/wcwidth/table_wide.py` & `prot-3.9.1/src/prot/wcwidth/table_wide.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/wcwidth/table_zero.py` & `prot-3.9.1/src/prot/wcwidth/table_zero.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/wcwidth/tests/test_core.py` & `prot-3.9.1/src/prot/wcwidth/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `prot-3.9.0/src/prot/wcwidth/wcwidth.py` & `prot-3.9.1/src/prot/wcwidth/wcwidth.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -66,18 +66,18 @@
 for any purpose and without fee is hereby granted. The author
 disclaims all warranties with regard to this software.
 
 Latest version: http://www.cl.cam.ac.uk/~mgk25/ucs/wcwidth.c
 """
 
 from __future__ import division
+
 from .table_wide import WIDE_EASTASIAN
 from .table_zero import ZERO_WIDTH
 
-
 # NOTE: created by hand, there isn't anything identifiable other than
 # general Cf category code to identify these, and some characters in Cf
 # category code are of non-zero width.
 # Also includes some Cc, Mn, Zl, and Zp characters
 ZERO_WIDTH_CF = set(
     [
         0,  # Null (Cc)
```

### Comparing `prot-3.9.0/src/prot.egg-info/PKG-INFO` & `prot-3.9.1/src/prot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prot
-Version: 3.9.0
+Version: 3.9.1
 Summary: A Simple Tool That Contains Advance Functions.
 Home-page: https://github.com/SAPTeamDEV/prot
 Author: Alireza Poodineh
 Author-email: itsaeliux@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prot-3.9.0/src/prot.egg-info/SOURCES.txt` & `prot-3.9.1/src/prot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

