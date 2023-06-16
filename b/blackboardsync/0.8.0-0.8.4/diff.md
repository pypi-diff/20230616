# Comparing `tmp/blackboardsync-0.8.0.tar.gz` & `tmp/blackboardsync-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackboardsync-0.8.0.tar", last modified: Fri Jun 16 09:06:09 2023, max compression
+gzip compressed data, was "blackboardsync-0.8.4.tar", last modified: Fri Jun 16 11:57:03 2023, max compression
```

## Comparing `blackboardsync-0.8.0.tar` & `blackboardsync-0.8.4.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:06:09.805889 blackboardsync-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:06:09.797888 blackboardsync-0.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:06:09.797888 blackboardsync-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-16 09:06:09.805889 blackboardsync-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    99257 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/UNIVERSITIES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:06:09.801888 blackboardsync-0.8.0/blackboard_sync/
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:06:09.801888 blackboardsync-0.8.0/blackboard_sync/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/assets/alert.png
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/assets/alert.svg
--rw-r--r--   0 runner    (1001) docker     (123)   110234 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/assets/logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/assets/watermark.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:06:09.801888 blackboardsync-0.8.0/blackboard_sync/blackboard/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/blackboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/blackboard/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/blackboard/blackboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/institutions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:06:09.801888 blackboardsync-0.8.0/blackboard_sync/qt/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/qt/LoginWebView.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/qt/PersistenceWarning.ui
--rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/qt/SettingsWindow.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/qt/SetupWizard.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/qt/UniNotSupportedDialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20622 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/qt/qt_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/sync_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/universities.json
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/blackboard_sync/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:06:09.801888 blackboardsync-0.8.0/blackboardsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-16 09:06:09.000000 blackboardsync-0.8.0/blackboardsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-16 09:06:09.000000 blackboardsync-0.8.0/blackboardsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 09:06:09.000000 blackboardsync-0.8.0/blackboardsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-16 09:06:09.000000 blackboardsync-0.8.0/blackboardsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 09:06:09.000000 blackboardsync-0.8.0/blackboardsync.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:06:09.805889 blackboardsync-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:06:09.805889 blackboardsync-0.8.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:06:09.805889 blackboardsync-0.8.0/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/docs/dev/bb_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/docs/dev/qt_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/docs/dev/sync_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:06:09.805889 blackboardsync-0.8.0/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/packaging/pkg_macos.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/packaging/pkg_win.nsi
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/packaging/pyinst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-16 09:06:09.805889 blackboardsync-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 09:06:09.805889 blackboardsync-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/tests/test_blackboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/tests/test_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-16 09:05:28.000000 blackboardsync-0.8.0/tests/test_sync_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:57:03.689205 blackboardsync-0.8.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:57:03.681205 blackboardsync-0.8.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:57:03.681205 blackboardsync-0.8.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-16 11:57:03.689205 blackboardsync-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    99257 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/UNIVERSITIES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:57:03.685205 blackboardsync-0.8.4/blackboard_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:57:03.685205 blackboardsync-0.8.4/blackboard_sync/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/assets/alert.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/assets/alert.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   110234 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/assets/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/assets/watermark.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:57:03.685205 blackboardsync-0.8.4/blackboard_sync/blackboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/blackboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/blackboard/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/blackboard/blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/institutions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:57:03.685205 blackboardsync-0.8.4/blackboard_sync/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/qt/LoginWebView.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/qt/PersistenceWarning.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/qt/SettingsWindow.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/qt/SetupWizard.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/qt/UniNotSupportedDialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20622 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/qt/qt_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/sync_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/universities.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/blackboard_sync/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:57:03.685205 blackboardsync-0.8.4/blackboardsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-16 11:57:03.000000 blackboardsync-0.8.4/blackboardsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-16 11:57:03.000000 blackboardsync-0.8.4/blackboardsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 11:57:03.000000 blackboardsync-0.8.4/blackboardsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-16 11:57:03.000000 blackboardsync-0.8.4/blackboardsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 11:57:03.000000 blackboardsync-0.8.4/blackboardsync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:57:03.685205 blackboardsync-0.8.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:57:03.685205 blackboardsync-0.8.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:57:03.689205 blackboardsync-0.8.4/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/docs/dev/bb_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/docs/dev/qt_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/docs/dev/sync_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:57:03.689205 blackboardsync-0.8.4/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/packaging/pkg_macos.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/packaging/pkg_win.nsi
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/packaging/pyinst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-16 11:57:03.689205 blackboardsync-0.8.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 11:57:03.689205 blackboardsync-0.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/tests/test_blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/tests/test_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-16 11:56:23.000000 blackboardsync-0.8.4/tests/test_sync_config.py
```

### Comparing `blackboardsync-0.8.0/.github/workflows/build.yml` & `blackboardsync-0.8.4/.github/workflows/build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,18 @@
           TWINE_USERNAME: ${{ secrets.TWINE_USERNAME }}
           TWINE_PASSWORD: ${{ secrets.TWINE_PASSWORD }}
         run: |
           python -m build
           twine upload dist/*
 
   pyinstaller:
-    runs-on: [ windows-latest, macos-latest ]
+    runs-on: ${{ matrix.os }}
+    strategy:
+      matrix:
+        os: [macos-latest, windows-latest]
     if: startsWith(github.ref, 'refs/tags/')
     needs: [ test, version-check ]
     steps:
       - name: Checkout repository
         uses: actions/checkout@v3
 
       - name: Set up Python
```

### Comparing `blackboardsync-0.8.0/.gitignore` & `blackboardsync-0.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/CHANGELOG.md` & `blackboardsync-0.8.4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/CONTRIBUTING.md` & `blackboardsync-0.8.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/LICENSE` & `blackboardsync-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/PKG-INFO` & `blackboardsync-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.8.0
+Version: 0.8.4
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `blackboardsync-0.8.0/Pipfile` & `blackboardsync-0.8.4/Pipfile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/Pipfile.lock` & `blackboardsync-0.8.4/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/README.md` & `blackboardsync-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/UNIVERSITIES.md` & `blackboardsync-0.8.4/UNIVERSITIES.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/blackboard_sync/__about__.py` & `blackboardsync-0.8.4/blackboard_sync/__about__.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,14 @@
     "__copyright__",
 ]
 
 __title__ = "BlackboardSync"
 __summary__ = "Automatic Syncing Of Your Blackboard Content"
 __uri__ = "https://github.com/jacobszpz/BlackboardSync"
 
-__version__ = "0.8.3-5"
+__version__ = "0.8.4"
 
 __author__ = "Jacob Sánchez"
 __email__ = "jacobszpz@protonmail.com"
 
 __license__ = "GNU General Public License v2"
 __copyright__ = f"2023, {__author__}"
```

### Comparing `blackboardsync-0.8.0/blackboard_sync/__main__.py` & `blackboardsync-0.8.4/blackboard_sync/__main__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/blackboard_sync/assets/alert.png` & `blackboardsync-0.8.4/blackboard_sync/assets/alert.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/blackboard_sync/assets/alert.svg` & `blackboardsync-0.8.4/blackboard_sync/assets/alert.svg`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/blackboard_sync/assets/logo.ico` & `blackboardsync-0.8.4/blackboard_sync/assets/logo.ico`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/blackboard_sync/assets/logo.png` & `blackboardsync-0.8.4/blackboard_sync/assets/logo.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/blackboard_sync/assets/watermark.png` & `blackboardsync-0.8.4/blackboard_sync/assets/watermark.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/blackboard_sync/blackboard/__init__.py` & `blackboardsync-0.8.4/blackboard_sync/blackboard/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/blackboard_sync/blackboard/api.py` & `blackboardsync-0.8.4/blackboard_sync/blackboard/api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/blackboard_sync/blackboard/blackboard.py` & `blackboardsync-0.8.4/blackboard_sync/blackboard/blackboard.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/blackboard_sync/config.py` & `blackboardsync-0.8.4/blackboard_sync/config.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/blackboard_sync/download.py` & `blackboardsync-0.8.4/blackboard_sync/download.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/blackboard_sync/institutions.py` & `blackboardsync-0.8.4/blackboard_sync/institutions.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/blackboard_sync/qt/LoginWebView.ui` & `blackboardsync-0.8.4/blackboard_sync/qt/LoginWebView.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/blackboard_sync/qt/PersistenceWarning.ui` & `blackboardsync-0.8.4/blackboard_sync/qt/PersistenceWarning.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/blackboard_sync/qt/SettingsWindow.ui` & `blackboardsync-0.8.4/blackboard_sync/qt/SettingsWindow.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/blackboard_sync/qt/SetupWizard.ui` & `blackboardsync-0.8.4/blackboard_sync/qt/SetupWizard.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/blackboard_sync/qt/UniNotSupportedDialog.ui` & `blackboardsync-0.8.4/blackboard_sync/qt/UniNotSupportedDialog.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/blackboard_sync/qt/__init__.py` & `blackboardsync-0.8.4/blackboard_sync/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/blackboard_sync/qt/qt_elements.py` & `blackboardsync-0.8.4/blackboard_sync/qt/qt_elements.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/blackboard_sync/sync.py` & `blackboardsync-0.8.4/blackboard_sync/sync.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/blackboard_sync/sync_controller.py` & `blackboardsync-0.8.4/blackboard_sync/sync_controller.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/blackboard_sync/updates.py` & `blackboardsync-0.8.4/blackboard_sync/updates.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/blackboard_sync/webdav.py` & `blackboardsync-0.8.4/blackboard_sync/webdav.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/blackboardsync.egg-info/PKG-INFO` & `blackboardsync-0.8.4/blackboardsync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.8.0
+Version: 0.8.4
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `blackboardsync-0.8.0/blackboardsync.egg-info/SOURCES.txt` & `blackboardsync-0.8.4/blackboardsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/docs/Makefile` & `blackboardsync-0.8.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/docs/conf.py` & `blackboardsync-0.8.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/docs/index.rst` & `blackboardsync-0.8.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/docs/make.bat` & `blackboardsync-0.8.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/main.py` & `blackboardsync-0.8.4/main.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/packaging/pkg_macos.sh` & `blackboardsync-0.8.4/packaging/pkg_macos.sh`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/packaging/pkg_win.nsi` & `blackboardsync-0.8.4/packaging/pkg_win.nsi`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/packaging/pyinst.py` & `blackboardsync-0.8.4/packaging/pyinst.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/pyproject.toml` & `blackboardsync-0.8.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "blackboardsync"
-version = "0.8.0"
+dynamic = ["version"]
 authors = [
   { name="Jacob Sánchez", email="jacobszpz@protonmail.com" },
 ]
 description = "Sync your blackboard content to your device"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -25,14 +25,17 @@
     "python-dateutil",
     "appdirs",
     "lxml",
     "requests",
     "packaging"
 ]
 
+[tool.setuptools.dynamic]
+version = {attr = "blackboard_sync.__version__"}
+
 [project.optional-dependencies]
 test = ["pytest", "hypothesis", "coverage", "pytest-qt", "pytest-mock"]
 package = ["pyinstaller", "build", "twine"]
 
 [project.urls]
 "Homepage" = "https://bbsync.app"
 "Repository" = "https://github.com/jacobszpz/BlackboardSync"
```

### Comparing `blackboardsync-0.8.0/tests/strategies.py` & `blackboardsync-0.8.4/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/tests/test_api.py` & `blackboardsync-0.8.4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/tests/test_blackboard.py` & `blackboardsync-0.8.4/tests/test_blackboard.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/tests/test_download.py` & `blackboardsync-0.8.4/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/tests/test_qt.py` & `blackboardsync-0.8.4/tests/test_qt.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.0/tests/test_sync_config.py` & `blackboardsync-0.8.4/tests/test_sync_config.py`

 * *Files identical despite different names*

