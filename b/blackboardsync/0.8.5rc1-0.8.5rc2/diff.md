# Comparing `tmp/blackboardsync-0.8.5rc1.tar.gz` & `tmp/blackboardsync-0.8.5rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackboardsync-0.8.5rc1.tar", last modified: Fri Jun 16 20:32:44 2023, max compression
+gzip compressed data, was "blackboardsync-0.8.5rc2.tar", last modified: Fri Jun 16 20:45:54 2023, max compression
```

## Comparing `blackboardsync-0.8.5rc1.tar` & `blackboardsync-0.8.5rc2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:32:44.117443 blackboardsync-0.8.5rc1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:32:44.113443 blackboardsync-0.8.5rc1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:32:44.113443 blackboardsync-0.8.5rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-06-16 20:32:44.117443 blackboardsync-0.8.5rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    99257 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/UNIVERSITIES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:32:44.113443 blackboardsync-0.8.5rc1/blackboard_sync/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:32:44.113443 blackboardsync-0.8.5rc1/blackboard_sync/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/assets/alert.png
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/assets/alert.svg
--rw-r--r--   0 runner    (1001) docker     (123)   110234 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/assets/logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/assets/watermark.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:32:44.117443 blackboardsync-0.8.5rc1/blackboard_sync/blackboard/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/blackboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/blackboard/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/blackboard/blackboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/institutions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:32:44.117443 blackboardsync-0.8.5rc1/blackboard_sync/qt/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/qt/LoginWebView.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/qt/PersistenceWarning.ui
--rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/qt/SettingsWindow.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/qt/SetupWizard.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/qt/UniNotSupportedDialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20622 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/qt/qt_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/sync_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/universities.json
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/blackboard_sync/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:32:44.117443 blackboardsync-0.8.5rc1/blackboardsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-06-16 20:32:44.000000 blackboardsync-0.8.5rc1/blackboardsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-16 20:32:44.000000 blackboardsync-0.8.5rc1/blackboardsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:32:44.000000 blackboardsync-0.8.5rc1/blackboardsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-16 20:32:44.000000 blackboardsync-0.8.5rc1/blackboardsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 20:32:44.000000 blackboardsync-0.8.5rc1/blackboardsync.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:32:44.117443 blackboardsync-0.8.5rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:32:44.117443 blackboardsync-0.8.5rc1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:32:44.117443 blackboardsync-0.8.5rc1/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/docs/dev/bb_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/docs/dev/qt_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/docs/dev/sync_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:32:44.117443 blackboardsync-0.8.5rc1/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/packaging/pkg_macos.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/packaging/pkg_win.nsi
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/packaging/pyinst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-16 20:32:44.121443 blackboardsync-0.8.5rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:32:44.117443 blackboardsync-0.8.5rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/tests/test_blackboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/tests/test_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-16 20:32:01.000000 blackboardsync-0.8.5rc1/tests/test_sync_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:45:54.257110 blackboardsync-0.8.5rc2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:45:54.245111 blackboardsync-0.8.5rc2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:45:54.245111 blackboardsync-0.8.5rc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-06-16 20:45:54.257110 blackboardsync-0.8.5rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    99257 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/UNIVERSITIES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:45:54.249111 blackboardsync-0.8.5rc2/blackboard_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:45:54.249111 blackboardsync-0.8.5rc2/blackboard_sync/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/assets/alert.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/assets/alert.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   110234 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/assets/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/assets/watermark.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:45:54.249111 blackboardsync-0.8.5rc2/blackboard_sync/blackboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/blackboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/blackboard/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/blackboard/blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/institutions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:45:54.249111 blackboardsync-0.8.5rc2/blackboard_sync/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/qt/LoginWebView.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/qt/PersistenceWarning.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/qt/SettingsWindow.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/qt/SetupWizard.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/qt/UniNotSupportedDialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20622 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/qt/qt_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/sync_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/universities.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/blackboard_sync/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:45:54.253111 blackboardsync-0.8.5rc2/blackboardsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-06-16 20:45:54.000000 blackboardsync-0.8.5rc2/blackboardsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-16 20:45:54.000000 blackboardsync-0.8.5rc2/blackboardsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:45:54.000000 blackboardsync-0.8.5rc2/blackboardsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-16 20:45:54.000000 blackboardsync-0.8.5rc2/blackboardsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-16 20:45:54.000000 blackboardsync-0.8.5rc2/blackboardsync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:45:54.253111 blackboardsync-0.8.5rc2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:45:54.253111 blackboardsync-0.8.5rc2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:45:54.253111 blackboardsync-0.8.5rc2/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/docs/dev/bb_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/docs/dev/qt_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/docs/dev/sync_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:45:54.253111 blackboardsync-0.8.5rc2/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/packaging/pkg_macos.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/packaging/pkg_win.nsi
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/packaging/pyinst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-16 20:45:54.257110 blackboardsync-0.8.5rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:45:54.257110 blackboardsync-0.8.5rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/tests/test_blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/tests/test_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-16 20:45:06.000000 blackboardsync-0.8.5rc2/tests/test_sync_config.py
```

### Comparing `blackboardsync-0.8.5rc1/.github/workflows/build.yml` & `blackboardsync-0.8.5rc2/.github/workflows/build.yml`

 * *Files 0% similar despite different names*

```diff
@@ -131,9 +131,9 @@
 
       # Save Packages
 
       - name: Upload as release - only tagged commits
         uses: softprops/action-gh-release@v1
         with:
           files: |
-            'dist/*.exe'
-            'dist/*.dmg'
+            dist/*.exe
+            dist/*.dmg
```

### Comparing `blackboardsync-0.8.5rc1/.gitignore` & `blackboardsync-0.8.5rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/CHANGELOG.md` & `blackboardsync-0.8.5rc2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/CONTRIBUTING.md` & `blackboardsync-0.8.5rc2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/LICENSE` & `blackboardsync-0.8.5rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/PKG-INFO` & `blackboardsync-0.8.5rc2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.8.5rc1
+Version: 0.8.5rc2
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -204,15 +204,15 @@
 
 
 
 <!-- SHIELDS -->
 
 [version-shield]: https://img.shields.io/pypi/v/BlackboardSync
 [license-shield]: https://img.shields.io/github/license/jacobszpz/BlackboardSync
-[build-shield]: https://img.shields.io/github/actions/workflow/status/jacobszpz/BlackboardSync/release.yml?branch=main
+[build-shield]: https://img.shields.io/github/actions/workflow/status/jacobszpz/BlackboardSync/build.yml?branch=main
 [kofi-shield]: https://ko-fi.com/img/githubbutton_sm.svg
 [lp-shield]: https://img.shields.io/liberapay/receives/BlackboardSync.svg?logo=liberapay
 
 
 
 <!-- SHIELD LINKS -->
```

### Comparing `blackboardsync-0.8.5rc1/Pipfile` & `blackboardsync-0.8.5rc2/Pipfile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/Pipfile.lock` & `blackboardsync-0.8.5rc2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/README.md` & `blackboardsync-0.8.5rc2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
 
 
 
 <!-- SHIELDS -->
 
 [version-shield]: https://img.shields.io/pypi/v/BlackboardSync
 [license-shield]: https://img.shields.io/github/license/jacobszpz/BlackboardSync
-[build-shield]: https://img.shields.io/github/actions/workflow/status/jacobszpz/BlackboardSync/release.yml?branch=main
+[build-shield]: https://img.shields.io/github/actions/workflow/status/jacobszpz/BlackboardSync/build.yml?branch=main
 [kofi-shield]: https://ko-fi.com/img/githubbutton_sm.svg
 [lp-shield]: https://img.shields.io/liberapay/receives/BlackboardSync.svg?logo=liberapay
 
 
 
 <!-- SHIELD LINKS -->
```

### Comparing `blackboardsync-0.8.5rc1/UNIVERSITIES.md` & `blackboardsync-0.8.5rc2/UNIVERSITIES.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/__about__.py` & `blackboardsync-0.8.5rc2/blackboard_sync/__about__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,14 @@
     "__copyright__",
 ]
 
 __title__ = "BlackboardSync"
 __summary__ = "Automatic Syncing Of Your Blackboard Content"
 __uri__ = "https://github.com/jacobszpz/BlackboardSync"
 
-__version__ = "0.8.5-rc.1"
+__version__ = "0.8.5-rc.2"
 
 __author__ = "Jacob Sánchez"
 __email__ = "jacobszpz@protonmail.com"
 
 __license__ = "GNU General Public License v2"
 __copyright__ = f"2023, {__author__}"
```

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/__init__.py` & `blackboardsync-0.8.5rc2/blackboard_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/__main__.py` & `blackboardsync-0.8.5rc2/blackboard_sync/__main__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/assets/alert.png` & `blackboardsync-0.8.5rc2/blackboard_sync/assets/alert.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/assets/alert.svg` & `blackboardsync-0.8.5rc2/blackboard_sync/assets/alert.svg`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/assets/logo.ico` & `blackboardsync-0.8.5rc2/blackboard_sync/assets/logo.ico`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/assets/logo.png` & `blackboardsync-0.8.5rc2/blackboard_sync/assets/logo.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/assets/watermark.png` & `blackboardsync-0.8.5rc2/blackboard_sync/assets/watermark.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/blackboard/__init__.py` & `blackboardsync-0.8.5rc2/blackboard_sync/blackboard/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/blackboard/api.py` & `blackboardsync-0.8.5rc2/blackboard_sync/blackboard/api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/blackboard/blackboard.py` & `blackboardsync-0.8.5rc2/blackboard_sync/blackboard/blackboard.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/config.py` & `blackboardsync-0.8.5rc2/blackboard_sync/config.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/download.py` & `blackboardsync-0.8.5rc2/blackboard_sync/download.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/institutions.py` & `blackboardsync-0.8.5rc2/blackboard_sync/institutions.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/qt/LoginWebView.ui` & `blackboardsync-0.8.5rc2/blackboard_sync/qt/LoginWebView.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/qt/PersistenceWarning.ui` & `blackboardsync-0.8.5rc2/blackboard_sync/qt/PersistenceWarning.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/qt/SettingsWindow.ui` & `blackboardsync-0.8.5rc2/blackboard_sync/qt/SettingsWindow.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/qt/SetupWizard.ui` & `blackboardsync-0.8.5rc2/blackboard_sync/qt/SetupWizard.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/qt/UniNotSupportedDialog.ui` & `blackboardsync-0.8.5rc2/blackboard_sync/qt/UniNotSupportedDialog.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/qt/__init__.py` & `blackboardsync-0.8.5rc2/blackboard_sync/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/qt/qt_elements.py` & `blackboardsync-0.8.5rc2/blackboard_sync/qt/qt_elements.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/sync.py` & `blackboardsync-0.8.5rc2/blackboard_sync/sync.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/sync_controller.py` & `blackboardsync-0.8.5rc2/blackboard_sync/sync_controller.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/updates.py` & `blackboardsync-0.8.5rc2/blackboard_sync/updates.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboard_sync/webdav.py` & `blackboardsync-0.8.5rc2/blackboard_sync/webdav.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/blackboardsync.egg-info/PKG-INFO` & `blackboardsync-0.8.5rc2/blackboardsync.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.8.5rc1
+Version: 0.8.5rc2
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -204,15 +204,15 @@
 
 
 
 <!-- SHIELDS -->
 
 [version-shield]: https://img.shields.io/pypi/v/BlackboardSync
 [license-shield]: https://img.shields.io/github/license/jacobszpz/BlackboardSync
-[build-shield]: https://img.shields.io/github/actions/workflow/status/jacobszpz/BlackboardSync/release.yml?branch=main
+[build-shield]: https://img.shields.io/github/actions/workflow/status/jacobszpz/BlackboardSync/build.yml?branch=main
 [kofi-shield]: https://ko-fi.com/img/githubbutton_sm.svg
 [lp-shield]: https://img.shields.io/liberapay/receives/BlackboardSync.svg?logo=liberapay
 
 
 
 <!-- SHIELD LINKS -->
```

### Comparing `blackboardsync-0.8.5rc1/blackboardsync.egg-info/SOURCES.txt` & `blackboardsync-0.8.5rc2/blackboardsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/docs/Makefile` & `blackboardsync-0.8.5rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/docs/conf.py` & `blackboardsync-0.8.5rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/docs/index.rst` & `blackboardsync-0.8.5rc2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/docs/make.bat` & `blackboardsync-0.8.5rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/main.py` & `blackboardsync-0.8.5rc2/main.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/packaging/pkg_macos.sh` & `blackboardsync-0.8.5rc2/packaging/pkg_macos.sh`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/packaging/pkg_win.nsi` & `blackboardsync-0.8.5rc2/packaging/pkg_win.nsi`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/packaging/pyinst.py` & `blackboardsync-0.8.5rc2/packaging/pyinst.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/pyproject.toml` & `blackboardsync-0.8.5rc2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/tests/strategies.py` & `blackboardsync-0.8.5rc2/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/tests/test_api.py` & `blackboardsync-0.8.5rc2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/tests/test_blackboard.py` & `blackboardsync-0.8.5rc2/tests/test_blackboard.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/tests/test_download.py` & `blackboardsync-0.8.5rc2/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/tests/test_qt.py` & `blackboardsync-0.8.5rc2/tests/test_qt.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.8.5rc1/tests/test_sync_config.py` & `blackboardsync-0.8.5rc2/tests/test_sync_config.py`

 * *Files identical despite different names*

