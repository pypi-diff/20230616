# Comparing `tmp/dpytest-0.6.6.tar.gz` & `tmp/dpytest-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpytest-0.6.6.tar", last modified: Thu May 11 08:49:49 2023, max compression
+gzip compressed data, was "dpytest-0.6.7.tar", last modified: Fri Jun 16 12:31:44 2023, max compression
```

## Comparing `dpytest-0.6.6.tar` & `dpytest-0.6.7.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 08:49:49.272755 dpytest-0.6.6/
--rw-rw-rw-   0        0        0     1969 2023-05-11 08:45:53.000000 dpytest-0.6.6/HISTORY.md
--rw-rw-rw-   0        0        0     1102 2023-05-05 10:24:22.000000 dpytest-0.6.6/LICENSE
--rw-rw-rw-   0        0        0      228 2023-05-05 10:24:22.000000 dpytest-0.6.6/MANIFEST.in
--rw-rw-rw-   0        0        0     5443 2023-05-11 08:49:49.276753 dpytest-0.6.6/PKG-INFO
--rw-rw-rw-   0        0        0     1142 2023-05-05 10:24:22.000000 dpytest-0.6.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 08:49:48.334757 dpytest-0.6.6/discord/
-drwxrwxrwx   0        0        0        0 2023-05-11 08:49:48.337762 dpytest-0.6.6/discord/ext/
-drwxrwxrwx   0        0        0        0 2023-05-11 08:49:48.494756 dpytest-0.6.6/discord/ext/test/
--rw-rw-rw-   0        0        0      586 2023-05-11 08:46:22.000000 dpytest-0.6.6/discord/ext/test/__init__.py
--rw-rw-rw-   0        0        0      541 2023-05-05 10:24:22.000000 dpytest-0.6.6/discord/ext/test/_types.py
--rw-rw-rw-   0        0        0    41717 2023-05-11 08:44:19.000000 dpytest-0.6.6/discord/ext/test/backend.py
--rw-rw-rw-   0        0        0     1992 2023-05-05 10:24:22.000000 dpytest-0.6.6/discord/ext/test/callbacks.py
--rw-rw-rw-   0        0        0    20502 2023-05-11 08:44:19.000000 dpytest-0.6.6/discord/ext/test/factories.py
--rw-rw-rw-   0        0        0    14745 2023-05-11 08:44:19.000000 dpytest-0.6.6/discord/ext/test/runner.py
--rw-rw-rw-   0        0        0     3873 2023-05-05 10:24:22.000000 dpytest-0.6.6/discord/ext/test/state.py
--rw-rw-rw-   0        0        0     1870 2023-05-05 11:49:16.000000 dpytest-0.6.6/discord/ext/test/utils.py
--rw-rw-rw-   0        0        0    10242 2023-05-05 10:24:22.000000 dpytest-0.6.6/discord/ext/test/verify.py
--rw-rw-rw-   0        0        0     1355 2023-05-05 10:24:22.000000 dpytest-0.6.6/discord/ext/test/voice.py
--rw-rw-rw-   0        0        0     1605 2023-05-05 10:24:22.000000 dpytest-0.6.6/discord/ext/test/websocket.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:49:48.524752 dpytest-0.6.6/docs/
--rw-rw-rw-   0        0        0     2957 2023-05-11 08:46:22.000000 dpytest-0.6.6/docs/conf.py
--rw-rw-rw-   0        0        0      796 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/index.rst
-drwxrwxrwx   0        0        0        0 2023-05-11 08:49:48.796753 dpytest-0.6.6/docs/modules/
--rw-rw-rw-   0        0        0       64 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/modules/backend.rst
--rw-rw-rw-   0        0        0       70 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/modules/callbacks.rst
--rw-rw-rw-   0        0        0       70 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/modules/factories.rst
--rw-rw-rw-   0        0        0      171 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/modules/index.rst
--rw-rw-rw-   0        0        0       61 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/modules/runner.rst
--rw-rw-rw-   0        0        0       58 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/modules/state.rst
--rw-rw-rw-   0        0        0       58 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/modules/utils.rst
--rw-rw-rw-   0        0        0       61 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/modules/verify.rst
--rw-rw-rw-   0        0        0       70 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/modules/websocket.rst
-drwxrwxrwx   0        0        0        0 2023-05-11 08:49:48.955751 dpytest-0.6.6/docs/tutorials/
--rw-rw-rw-   0        0        0     1707 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/tutorials/getting_started.rst
--rw-rw-rw-   0        0        0      310 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/tutorials/index.rst
--rw-rw-rw-   0        0        0     5008 2023-05-05 10:24:22.000000 dpytest-0.6.6/docs/tutorials/using_pytest.rst
-drwxrwxrwx   0        0        0        0 2023-05-11 08:49:49.055757 dpytest-0.6.6/dpytest.egg-info/
--rw-rw-rw-   0        0        0     5443 2023-05-11 08:49:48.000000 dpytest-0.6.6/dpytest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1493 2023-05-11 08:49:48.000000 dpytest-0.6.6/dpytest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 08:49:48.000000 dpytest-0.6.6/dpytest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      111 2023-05-11 08:49:48.000000 dpytest-0.6.6/dpytest.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-11 08:49:48.000000 dpytest-0.6.6/dpytest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1534 2023-05-05 10:24:22.000000 dpytest-0.6.6/pyproject.toml
--rw-rw-rw-   0        0        0      514 2023-05-11 08:49:49.293752 dpytest-0.6.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-11 08:49:49.242753 dpytest-0.6.6/tests/
--rw-rw-rw-   0        0        0        0 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/__init__.py
--rw-rw-rw-   0        0        0     1377 2023-05-05 12:04:47.000000 dpytest-0.6.6/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:49:49.259750 dpytest-0.6.6/tests/data/
--rw-rw-rw-   0        0        0     3561 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/data/loremimpsum.txt
--rw-rw-rw-   0        0        0    48027 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/data/unit-tests.jpg
-drwxrwxrwx   0        0        0        0 2023-05-11 08:49:49.262751 dpytest-0.6.6/tests/internal/
--rw-rw-rw-   0        0        0        0 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/internal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 08:49:49.269753 dpytest-0.6.6/tests/internal/cogs/
--rw-rw-rw-   0        0        0        0 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/internal/cogs/__init__.py
--rw-rw-rw-   0        0        0      330 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/internal/cogs/echo.py
--rw-rw-rw-   0        0        0      352 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/internal/cogs/greeting.py
--rw-rw-rw-   0        0        0      809 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_activity.py
--rw-rw-rw-   0        0        0      948 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_create_channel.py
--rw-rw-rw-   0        0        0      508 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_dmchannel.py
--rw-rw-rw-   0        0        0      552 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_edit.py
--rw-rw-rw-   0        0        0      442 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_fetch_message.py
--rw-rw-rw-   0        0        0     1800 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_get.py
--rw-rw-rw-   0        0        0      783 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_member.py
--rw-rw-rw-   0        0        0     1386 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_mentions.py
--rw-rw-rw-   0        0        0     1192 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_message.py
--rw-rw-rw-   0        0        0     2333 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_permissions.py
--rw-rw-rw-   0        0        0     1789 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_reactions.py
--rw-rw-rw-   0        0        0     1926 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_role.py
--rw-rw-rw-   0        0        0      509 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_send.py
--rw-rw-rw-   0        0        0     3102 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_utils.py
--rw-rw-rw-   0        0        0     1684 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_verify_embed.py
--rw-rw-rw-   0        0        0     1146 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_verify_file.py
--rw-rw-rw-   0        0        0     1675 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_verify_message.py
--rw-rw-rw-   0        0        0      754 2023-05-05 10:24:22.000000 dpytest-0.6.6/tests/test_voice.py
+drwxrwxrwx   0        0        0        0 2023-06-16 12:31:44.834169 dpytest-0.6.7/
+-rw-rw-rw-   0        0        0     2234 2023-06-16 12:29:51.000000 dpytest-0.6.7/HISTORY.md
+-rw-rw-rw-   0        0        0     1102 2023-06-16 08:31:44.000000 dpytest-0.6.7/LICENSE
+-rw-rw-rw-   0        0        0      228 2023-06-16 08:31:44.000000 dpytest-0.6.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     5708 2023-06-16 12:31:44.834169 dpytest-0.6.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1142 2023-06-16 08:31:44.000000 dpytest-0.6.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 12:31:43.813166 dpytest-0.6.7/discord/
+drwxrwxrwx   0        0        0        0 2023-06-16 12:31:43.817169 dpytest-0.6.7/discord/ext/
+drwxrwxrwx   0        0        0        0 2023-06-16 12:31:43.921167 dpytest-0.6.7/discord/ext/test/
+-rw-rw-rw-   0        0        0      586 2023-06-16 12:29:33.000000 dpytest-0.6.7/discord/ext/test/__init__.py
+-rw-rw-rw-   0        0        0      541 2023-06-16 08:31:44.000000 dpytest-0.6.7/discord/ext/test/_types.py
+-rw-rw-rw-   0        0        0    41690 2023-06-16 08:31:44.000000 dpytest-0.6.7/discord/ext/test/backend.py
+-rw-rw-rw-   0        0        0     1992 2023-06-16 08:31:44.000000 dpytest-0.6.7/discord/ext/test/callbacks.py
+-rw-rw-rw-   0        0        0    20502 2023-06-16 08:31:44.000000 dpytest-0.6.7/discord/ext/test/factories.py
+-rw-rw-rw-   0        0        0    14745 2023-06-16 08:31:44.000000 dpytest-0.6.7/discord/ext/test/runner.py
+-rw-rw-rw-   0        0        0     3873 2023-06-16 08:31:44.000000 dpytest-0.6.7/discord/ext/test/state.py
+-rw-rw-rw-   0        0        0     1870 2023-06-16 08:31:44.000000 dpytest-0.6.7/discord/ext/test/utils.py
+-rw-rw-rw-   0        0        0    10242 2023-06-16 08:31:44.000000 dpytest-0.6.7/discord/ext/test/verify.py
+-rw-rw-rw-   0        0        0     1355 2023-06-16 08:31:44.000000 dpytest-0.6.7/discord/ext/test/voice.py
+-rw-rw-rw-   0        0        0     1605 2023-06-16 08:31:44.000000 dpytest-0.6.7/discord/ext/test/websocket.py
+drwxrwxrwx   0        0        0        0 2023-06-16 12:31:43.947165 dpytest-0.6.7/docs/
+-rw-rw-rw-   0        0        0     2957 2023-06-16 12:29:33.000000 dpytest-0.6.7/docs/conf.py
+-rw-rw-rw-   0        0        0      796 2023-06-16 08:31:44.000000 dpytest-0.6.7/docs/index.rst
+drwxrwxrwx   0        0        0        0 2023-06-16 12:31:44.252166 dpytest-0.6.7/docs/modules/
+-rw-rw-rw-   0        0        0       64 2023-06-16 08:31:44.000000 dpytest-0.6.7/docs/modules/backend.rst
+-rw-rw-rw-   0        0        0       70 2023-06-16 08:31:44.000000 dpytest-0.6.7/docs/modules/callbacks.rst
+-rw-rw-rw-   0        0        0       70 2023-06-16 08:31:44.000000 dpytest-0.6.7/docs/modules/factories.rst
+-rw-rw-rw-   0        0        0      171 2023-06-16 08:31:44.000000 dpytest-0.6.7/docs/modules/index.rst
+-rw-rw-rw-   0        0        0       61 2023-06-16 08:31:44.000000 dpytest-0.6.7/docs/modules/runner.rst
+-rw-rw-rw-   0        0        0       58 2023-06-16 08:31:44.000000 dpytest-0.6.7/docs/modules/state.rst
+-rw-rw-rw-   0        0        0       58 2023-06-16 08:31:44.000000 dpytest-0.6.7/docs/modules/utils.rst
+-rw-rw-rw-   0        0        0       61 2023-06-16 08:31:44.000000 dpytest-0.6.7/docs/modules/verify.rst
+-rw-rw-rw-   0        0        0       70 2023-06-16 08:31:44.000000 dpytest-0.6.7/docs/modules/websocket.rst
+drwxrwxrwx   0        0        0        0 2023-06-16 12:31:44.470164 dpytest-0.6.7/docs/tutorials/
+-rw-rw-rw-   0        0        0     1707 2023-06-16 08:31:44.000000 dpytest-0.6.7/docs/tutorials/getting_started.rst
+-rw-rw-rw-   0        0        0      310 2023-06-16 08:31:44.000000 dpytest-0.6.7/docs/tutorials/index.rst
+-rw-rw-rw-   0        0        0     5008 2023-06-16 08:31:44.000000 dpytest-0.6.7/docs/tutorials/using_pytest.rst
+drwxrwxrwx   0        0        0        0 2023-06-16 12:31:44.541165 dpytest-0.6.7/dpytest.egg-info/
+-rw-rw-rw-   0        0        0     5708 2023-06-16 12:31:43.000000 dpytest-0.6.7/dpytest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1527 2023-06-16 12:31:43.000000 dpytest-0.6.7/dpytest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 12:31:43.000000 dpytest-0.6.7/dpytest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      111 2023-06-16 12:31:43.000000 dpytest-0.6.7/dpytest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-16 12:31:43.000000 dpytest-0.6.7/dpytest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1534 2023-06-16 08:31:44.000000 dpytest-0.6.7/pyproject.toml
+-rw-rw-rw-   0        0        0      514 2023-06-16 12:31:44.913168 dpytest-0.6.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 12:31:44.731165 dpytest-0.6.7/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/__init__.py
+-rw-rw-rw-   0        0        0     1377 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-06-16 12:31:44.792193 dpytest-0.6.7/tests/data/
+-rw-rw-rw-   0        0        0     3561 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/data/loremimpsum.txt
+-rw-rw-rw-   0        0        0    48027 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/data/unit-tests.jpg
+drwxrwxrwx   0        0        0        0 2023-06-16 12:31:44.817167 dpytest-0.6.7/tests/internal/
+-rw-rw-rw-   0        0        0        0 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/internal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-16 12:31:44.831166 dpytest-0.6.7/tests/internal/cogs/
+-rw-rw-rw-   0        0        0        0 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/internal/cogs/__init__.py
+-rw-rw-rw-   0        0        0      330 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/internal/cogs/echo.py
+-rw-rw-rw-   0        0        0      352 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/internal/cogs/greeting.py
+-rw-rw-rw-   0        0        0      809 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/test_activity.py
+-rw-rw-rw-   0        0        0      948 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/test_create_channel.py
+-rw-rw-rw-   0        0        0      508 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/test_dmchannel.py
+-rw-rw-rw-   0        0        0      552 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/test_edit.py
+-rw-rw-rw-   0        0        0      442 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/test_fetch_message.py
+-rw-rw-rw-   0        0        0     1800 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/test_get.py
+-rw-rw-rw-   0        0        0      735 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/test_get_channel_history.py
+-rw-rw-rw-   0        0        0      783 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/test_member.py
+-rw-rw-rw-   0        0        0     1386 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/test_mentions.py
+-rw-rw-rw-   0        0        0     1192 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/test_message.py
+-rw-rw-rw-   0        0        0     2333 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/test_permissions.py
+-rw-rw-rw-   0        0        0     1789 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/test_reactions.py
+-rw-rw-rw-   0        0        0     1926 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/test_role.py
+-rw-rw-rw-   0        0        0      509 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/test_send.py
+-rw-rw-rw-   0        0        0     3102 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/test_utils.py
+-rw-rw-rw-   0        0        0     1684 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/test_verify_embed.py
+-rw-rw-rw-   0        0        0     1146 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/test_verify_file.py
+-rw-rw-rw-   0        0        0     1675 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/test_verify_message.py
+-rw-rw-rw-   0        0        0      754 2023-06-16 08:31:44.000000 dpytest-0.6.7/tests/test_voice.py
```

### Comparing `dpytest-0.6.6/HISTORY.md` & `dpytest-0.6.7/HISTORY.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # History
 
+## 0.6.7
+
+Fix bug in channel_history
+
+Fix issue #111
+
 ## 0.6.6
 
 Support asyncio tasks that have no \_\_name\_\_
 
 ## 0.6.5
 
 This release allows testing with Voice Channels.
@@ -13,18 +19,25 @@
 - `FakeVoiceChannel` and `FakeVoiceClient` classes implemetation
 - New tests
 
 Changes :
 
 - `create_channel` method can create voice channel
 
+⚠️ Warning ⚠️:
+
+This can be **breaking** :
+
+the `configure()` function DOESN'T take the keyword parameter `num_channels` anymore, but instead :
+`num_text_channels` and `num_voice_channels`
+
 ## 0.6.4
 
 - Fix: edit message doesn't update message queue
-- Refactor __init__.py import to be explicit exports as per PEP 484
+- Refactor **init**.py import to be explicit exports as per PEP 484
 
 ## 0.6.3
 
 - Update requirements for discord.py 2.2.2
 
 ## 0.6.2
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dpytest-0.6.6/LICENSE` & `dpytest-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/PKG-INFO` & `dpytest-0.6.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpytest
-Version: 0.6.6
+Version: 0.6.7
 Summary: A package that assists in writing tests for discord.py
 Author-email: Rune Tynan <runetynan@gmail.com>
 Maintainer: CraftSpider, Sergeileduc
 License: The MIT License (MIT)
         
         Copyright (c) 2018-2019 CraftSpider
         
@@ -65,14 +65,20 @@
 
 ## Documentation
 
 Documentation can be found at [dpytest.readthedocs.io](https://dpytest.readthedocs.io/en/latest/), including examples and tutorials
 
 # History
 
+## 0.6.7
+
+Fix bug in channel_history
+
+Fix issue #111
+
 ## 0.6.6
 
 Support asyncio tasks that have no \_\_name\_\_
 
 ## 0.6.5
 
 This release allows testing with Voice Channels.
@@ -82,18 +88,25 @@
 - `FakeVoiceChannel` and `FakeVoiceClient` classes implemetation
 - New tests
 
 Changes :
 
 - `create_channel` method can create voice channel
 
+⚠️ Warning ⚠️:
+
+This can be **breaking** :
+
+the `configure()` function DOESN'T take the keyword parameter `num_channels` anymore, but instead :
+`num_text_channels` and `num_voice_channels`
+
 ## 0.6.4
 
 - Fix: edit message doesn't update message queue
-- Refactor __init__.py import to be explicit exports as per PEP 484
+- Refactor **init**.py import to be explicit exports as per PEP 484
 
 ## 0.6.3
 
 - Update requirements for discord.py 2.2.2
 
 ## 0.6.2
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dpytest-0.6.6/README.md` & `dpytest-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/discord/ext/test/__init__.py` & `dpytest-0.6.7/discord/ext/test/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 __title__ = "dpytest"
 __author__ = "Rune Tynan"
 __license__ = "MIT"
 __copyright__ = "Copyright 2018-2019 CraftSpider"
-__version__ = "0.6.6"
+__version__ = "0.6.7"
 
 from . import backend as backend
 
 from .runner import *
 
 from .utils import embed_eq as embed_eq
 from .utils import activity_eq as activity_eq
```

### Comparing `dpytest-0.6.6/discord/ext/test/_types.py` & `dpytest-0.6.7/discord/ext/test/_types.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/discord/ext/test/backend.py` & `dpytest-0.6.7/discord/ext/test/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,16 +282,15 @@
             channel_id: int,
             limit: int,
             before: typing.Optional[int] = None,
             after: typing.Optional[int] = None,
             around: typing.Optional[int] = None
     ) -> typing.List[_types.JsonDict]:
         locs = _get_higher_locs(1)
-        his = locs.get("self", None)
-        channel = his.channel
+        channel = locs.get("self", None)
 
         await callbacks.dispatch_event("logs_from", channel, limit, before=None, after=None, around=None)
 
         messages = _cur_config.messages[channel_id]
         if after is not None:
             start = next(i for i, v in enumerate(messages) if v["id"] == after)
             return messages[start:start + limit]
```

### Comparing `dpytest-0.6.6/discord/ext/test/callbacks.py` & `dpytest-0.6.7/discord/ext/test/callbacks.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/discord/ext/test/factories.py` & `dpytest-0.6.7/discord/ext/test/factories.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/discord/ext/test/runner.py` & `dpytest-0.6.7/discord/ext/test/runner.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/discord/ext/test/state.py` & `dpytest-0.6.7/discord/ext/test/state.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/discord/ext/test/utils.py` & `dpytest-0.6.7/discord/ext/test/utils.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/discord/ext/test/verify.py` & `dpytest-0.6.7/discord/ext/test/verify.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/discord/ext/test/voice.py` & `dpytest-0.6.7/discord/ext/test/voice.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/discord/ext/test/websocket.py` & `dpytest-0.6.7/discord/ext/test/websocket.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/docs/conf.py` & `dpytest-0.6.7/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'dpytest'
 copyright = '2020, CraftSpider'
 author = 'CraftSpider'
 
 # The full version, including alpha/beta/rc tags
-release = '0.6.6'
+release = '0.6.7'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `dpytest-0.6.6/docs/index.rst` & `dpytest-0.6.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/docs/tutorials/getting_started.rst` & `dpytest-0.6.7/docs/tutorials/getting_started.rst`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/docs/tutorials/using_pytest.rst` & `dpytest-0.6.7/docs/tutorials/using_pytest.rst`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/dpytest.egg-info/PKG-INFO` & `dpytest-0.6.7/dpytest.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpytest
-Version: 0.6.6
+Version: 0.6.7
 Summary: A package that assists in writing tests for discord.py
 Author-email: Rune Tynan <runetynan@gmail.com>
 Maintainer: CraftSpider, Sergeileduc
 License: The MIT License (MIT)
         
         Copyright (c) 2018-2019 CraftSpider
         
@@ -65,14 +65,20 @@
 
 ## Documentation
 
 Documentation can be found at [dpytest.readthedocs.io](https://dpytest.readthedocs.io/en/latest/), including examples and tutorials
 
 # History
 
+## 0.6.7
+
+Fix bug in channel_history
+
+Fix issue #111
+
 ## 0.6.6
 
 Support asyncio tasks that have no \_\_name\_\_
 
 ## 0.6.5
 
 This release allows testing with Voice Channels.
@@ -82,18 +88,25 @@
 - `FakeVoiceChannel` and `FakeVoiceClient` classes implemetation
 - New tests
 
 Changes :
 
 - `create_channel` method can create voice channel
 
+⚠️ Warning ⚠️:
+
+This can be **breaking** :
+
+the `configure()` function DOESN'T take the keyword parameter `num_channels` anymore, but instead :
+`num_text_channels` and `num_voice_channels`
+
 ## 0.6.4
 
 - Fix: edit message doesn't update message queue
-- Refactor __init__.py import to be explicit exports as per PEP 484
+- Refactor **init**.py import to be explicit exports as per PEP 484
 
 ## 0.6.3
 
 - Update requirements for discord.py 2.2.2
 
 ## 0.6.2
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dpytest-0.6.6/dpytest.egg-info/SOURCES.txt` & `dpytest-0.6.7/dpytest.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 tests/conftest.py
 tests/test_activity.py
 tests/test_create_channel.py
 tests/test_dmchannel.py
 tests/test_edit.py
 tests/test_fetch_message.py
 tests/test_get.py
+tests/test_get_channel_history.py
 tests/test_member.py
 tests/test_mentions.py
 tests/test_message.py
 tests/test_permissions.py
 tests/test_reactions.py
 tests/test_role.py
 tests/test_send.py
```

### Comparing `dpytest-0.6.6/pyproject.toml` & `dpytest-0.6.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/setup.cfg` & `dpytest-0.6.7/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.6.6
+current_version = 0.6.7
 commit = True
 tag = True
 
 [tool:pytest]
 junit_family = xunit1
 testpaths = tests
 markers =
```

### Comparing `dpytest-0.6.6/tests/conftest.py` & `dpytest-0.6.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/tests/data/loremimpsum.txt` & `dpytest-0.6.7/tests/data/loremimpsum.txt`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/tests/data/unit-tests.jpg` & `dpytest-0.6.7/tests/data/unit-tests.jpg`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/tests/test_activity.py` & `dpytest-0.6.7/tests/test_activity.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/tests/test_create_channel.py` & `dpytest-0.6.7/tests/test_create_channel.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/tests/test_edit.py` & `dpytest-0.6.7/tests/test_edit.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/tests/test_get.py` & `dpytest-0.6.7/tests/test_get.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/tests/test_member.py` & `dpytest-0.6.7/tests/test_member.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/tests/test_mentions.py` & `dpytest-0.6.7/tests/test_mentions.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/tests/test_message.py` & `dpytest-0.6.7/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/tests/test_permissions.py` & `dpytest-0.6.7/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/tests/test_reactions.py` & `dpytest-0.6.7/tests/test_reactions.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/tests/test_role.py` & `dpytest-0.6.7/tests/test_role.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/tests/test_utils.py` & `dpytest-0.6.7/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/tests/test_verify_embed.py` & `dpytest-0.6.7/tests/test_verify_embed.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/tests/test_verify_file.py` & `dpytest-0.6.7/tests/test_verify_file.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/tests/test_verify_message.py` & `dpytest-0.6.7/tests/test_verify_message.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.6/tests/test_voice.py` & `dpytest-0.6.7/tests/test_voice.py`

 * *Files identical despite different names*

