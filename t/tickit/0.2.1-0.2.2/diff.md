# Comparing `tmp/tickit-0.2.1.tar.gz` & `tmp/tickit-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tickit-0.2.1.tar", last modified: Wed Apr 12 12:37:01 2023, max compression
+gzip compressed data, was "tickit-0.2.2.tar", last modified: Fri Jun 16 14:45:39 2023, max compression
```

## Comparing `tickit-0.2.1.tar` & `tickit-0.2.2.tar`

### file list

```diff
@@ -1,247 +1,252 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.553765 tickit-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.517765 tickit-0.2.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-12 12:36:47.000000 tickit-0.2.1/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-12 12:36:47.000000 tickit-0.2.1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-12 12:36:47.000000 tickit-0.2.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.517765 tickit-0.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-12 12:36:47.000000 tickit-0.2.1/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.509765 tickit-0.2.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.517765 tickit-0.2.1/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-12 12:36:47.000000 tickit-0.2.1/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-12 12:36:47.000000 tickit-0.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.517765 tickit-0.2.1/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-12 12:36:47.000000 tickit-0.2.1/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-12 12:36:47.000000 tickit-0.2.1/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.521765 tickit-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-04-12 12:36:47.000000 tickit-0.2.1/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-12 12:36:47.000000 tickit-0.2.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-12 12:36:47.000000 tickit-0.2.1/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-12 12:36:47.000000 tickit-0.2.1/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-12 12:36:47.000000 tickit-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-12 12:36:47.000000 tickit-0.2.1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-12 12:36:47.000000 tickit-0.2.1/.gitremotes
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-12 12:36:47.000000 tickit-0.2.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.521765 tickit-0.2.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-12 12:36:47.000000 tickit-0.2.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-12 12:36:47.000000 tickit-0.2.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-12 12:36:47.000000 tickit-0.2.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-12 12:36:47.000000 tickit-0.2.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-12 12:36:47.000000 tickit-0.2.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-12 12:36:47.000000 tickit-0.2.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 12:36:47.000000 tickit-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18646 2023-04-12 12:37:01.553765 tickit-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-04-12 12:36:47.000000 tickit-0.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 12:36:47.000000 tickit-0.2.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.521765 tickit-0.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.521765 tickit-0.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/_static/theme_overrides.css
--rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.521765 tickit-0.2.1/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.521765 tickit-0.2.1/docs/developer/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.521765 tickit-0.2.1/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/explanations/decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/explanations/framework-details.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/explanations/how-component-updates-are-ordered.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/explanations/why-tickit.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.525765 tickit-0.2.1/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/how-to/pin-requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/how-to/test-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.525765 tickit-0.2.1/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.525765 tickit-0.2.1/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.525765 tickit-0.2.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/images/example-systems.drawio.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/images/tickit-create-device-amplifier.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/images/tickit-device-simulation-cpt.svg
--rw-r--r--   0 runner    (1001) docker     (123)   343434 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/images/tickit-logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/images/tickit-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/images/tickit-overview-full.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/images/tickit-simple-dag.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/images/tickit-simple-overview-with-system-simulation.svg
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/images/tickit-simple-overview.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/images/tickit-simple-simulation.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/images/tickit-system-simulation-cpt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.525765 tickit-0.2.1/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.529765 tickit-0.2.1/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/explanations/adapters.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/explanations/components.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/explanations/devices.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/explanations/framework-summary.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/explanations/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/explanations/wiring.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.529765 tickit-0.2.1/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/how-to/use-command-wrappers.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/how-to/use-epics-adapter.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.529765 tickit-0.2.1/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.529765 tickit-0.2.1/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/tutorials/create-a-device.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/tutorials/creating-a-simulation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/tutorials/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/tutorials/running-a-simulation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-12 12:36:47.000000 tickit-0.2.1/docs/user/tutorials/use-composed-adapter.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.513765 tickit-0.2.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.529765 tickit-0.2.1/examples/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/configs/amplifier.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/configs/counter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/configs/http-device.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/configs/nested.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/configs/shutter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/configs/sunk-tcp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/configs/sunk-trampoline.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.533765 tickit-0.2.1/examples/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/devices/amplifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/devices/counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/devices/http_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/devices/remote_controlled.py
--rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/devices/shutter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-04-12 12:36:47.000000 tickit-0.2.1/examples/devices/trampoline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-12 12:36:47.000000 tickit-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 12:37:01.553765 tickit-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.513765 tickit-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.533765 tickit-0.2.1/src/tickit/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-12 12:37:01.000000 tickit-0.2.1/src/tickit/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.533765 tickit-0.2.1/src/tickit/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/composed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.537765 tickit-0.2.1/src/tickit/adapters/epicsadapter/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/epicsadapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/epicsadapter/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/epicsadapter/ioc_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/httpadapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.537765 tickit-0.2.1/src/tickit/adapters/interpreters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/interpreters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.537765 tickit-0.2.1/src/tickit/adapters/interpreters/command/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/interpreters/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/interpreters/command/command_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/interpreters/command/regex_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.537765 tickit-0.2.1/src/tickit/adapters/interpreters/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/interpreters/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/interpreters/endpoints/http_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/interpreters/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.537765 tickit-0.2.1/src/tickit/adapters/interpreters/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/interpreters/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/interpreters/wrappers/beheading_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/interpreters/wrappers/joining_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/interpreters/wrappers/splitting_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.537765 tickit-0.2.1/src/tickit/adapters/servers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/servers/tcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/adapters/zmqadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.537765 tickit-0.2.1/src/tickit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.541765 tickit-0.2.1/src/tickit/core/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/components/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/components/device_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/components/system_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.541765 tickit-0.2.1/src/tickit/core/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10532 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/management/event_router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.541765 tickit-0.2.1/src/tickit/core/management/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/management/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/management/schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/management/schedulers/master.py
--rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/management/schedulers/slave.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/management/ticker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.541765 tickit-0.2.1/src/tickit/core/state_interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/state_interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/state_interfaces/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/state_interfaces/kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/state_interfaces/state_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/core/typedefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.541765 tickit-0.2.1/src/tickit/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/devices/sink.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/devices/source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.545765 tickit-0.2.1/src/tickit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/utils/byte_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.545765 tickit-0.2.1/src/tickit/utils/compat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/utils/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/utils/compat/functools_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/utils/compat/typing_compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.545765 tickit-0.2.1/src/tickit/utils/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/utils/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/utils/configuration/configurable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/utils/configuration/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/utils/singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-12 12:36:47.000000 tickit-0.2.1/src/tickit/utils/topic_naming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.533765 tickit-0.2.1/src/tickit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18646 2023-04-12 12:37:01.000000 tickit-0.2.1/src/tickit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-04-12 12:37:01.000000 tickit-0.2.1/src/tickit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:37:01.000000 tickit-0.2.1/src/tickit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-12 12:37:01.000000 tickit-0.2.1/src/tickit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-12 12:37:01.000000 tickit-0.2.1/src/tickit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 12:37:01.000000 tickit-0.2.1/src/tickit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.545765 tickit-0.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.545765 tickit-0.2.1/tests/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.545765 tickit-0.2.1/tests/adapters/interpreters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.545765 tickit-0.2.1/tests/adapters/interpreters/command/
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/adapters/interpreters/command/test_command_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/adapters/interpreters/command/test_regex_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.545765 tickit-0.2.1/tests/adapters/interpreters/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/adapters/interpreters/endpoints/test_http_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/adapters/interpreters/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.545765 tickit-0.2.1/tests/adapters/interpreters/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/adapters/interpreters/wrappers/test_beheading_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/adapters/interpreters/wrappers/test_joining_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/adapters/interpreters/wrappers/test_splitting_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.545765 tickit-0.2.1/tests/adapters/servers/
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/adapters/servers/test_tcp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.549765 tickit-0.2.1/tests/adapters/test_epicsadapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/adapters/test_epicsadapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/adapters/test_epicsadapter/test_epics_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/adapters/test_httpadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/adapters/test_zmqadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.549765 tickit-0.2.1/tests/core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.549765 tickit-0.2.1/tests/core/components/
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/components/test_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/components/test_device_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/components/test_system_simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.549765 tickit-0.2.1/tests/core/management/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.549765 tickit-0.2.1/tests/core/management/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/management/schedulers/test_base_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/management/schedulers/test_master_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/management/schedulers/test_slave_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/management/test_event_router.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/management/test_ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.549765 tickit-0.2.1/tests/core/state_interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/state_interfaces/test_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/state_interfaces/test_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/state_interfaces/test_state_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/core/test_typedefs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.549765 tickit-0.2.1/tests/devices/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/devices/test_sink.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/devices/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.553765 tickit-0.2.1/tests/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:37:01.553765 tickit-0.2.1/tests/utils/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/utils/configuration/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/utils/test_byte_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/utils/test_configurable.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/utils/test_singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-12 12:36:47.000000 tickit-0.2.1/tests/utils/test_topic_naming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.059791 tickit-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.035789 tickit-0.2.2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-16 14:45:28.000000 tickit-0.2.2/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-16 14:45:28.000000 tickit-0.2.2/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 14:45:28.000000 tickit-0.2.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.035789 tickit-0.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-16 14:45:28.000000 tickit-0.2.2/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.027789 tickit-0.2.2/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.035789 tickit-0.2.2/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-16 14:45:28.000000 tickit-0.2.2/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-16 14:45:28.000000 tickit-0.2.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.035789 tickit-0.2.2/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-16 14:45:28.000000 tickit-0.2.2/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-06-16 14:45:28.000000 tickit-0.2.2/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.035789 tickit-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-06-16 14:45:28.000000 tickit-0.2.2/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-06-16 14:45:28.000000 tickit-0.2.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-16 14:45:28.000000 tickit-0.2.2/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-16 14:45:28.000000 tickit-0.2.2/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-16 14:45:28.000000 tickit-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-16 14:45:28.000000 tickit-0.2.2/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-16 14:45:28.000000 tickit-0.2.2/.gitremotes
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-16 14:45:28.000000 tickit-0.2.2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.035789 tickit-0.2.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-16 14:45:28.000000 tickit-0.2.2/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-16 14:45:28.000000 tickit-0.2.2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-16 14:45:28.000000 tickit-0.2.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-16 14:45:28.000000 tickit-0.2.2/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-16 14:45:28.000000 tickit-0.2.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-16 14:45:28.000000 tickit-0.2.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-16 14:45:28.000000 tickit-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18638 2023-06-16 14:45:39.059791 tickit-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-06-16 14:45:28.000000 tickit-0.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-16 14:45:28.000000 tickit-0.2.2/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.035789 tickit-0.2.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.035789 tickit-0.2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/_static/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7037 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.035789 tickit-0.2.2/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.035789 tickit-0.2.2/docs/developer/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.035789 tickit-0.2.2/docs/developer/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/developer/explanations/decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/developer/explanations/framework-details.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/developer/explanations/how-component-updates-are-ordered.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/developer/explanations/why-tickit.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.039790 tickit-0.2.2/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/developer/how-to/pin-requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/developer/how-to/test-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.039790 tickit-0.2.2/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.039790 tickit-0.2.2/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.039790 tickit-0.2.2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/images/example-systems.drawio.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/images/tickit-create-device-amplifier.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/images/tickit-device-simulation-cpt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   343434 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/images/tickit-logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/images/tickit-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/images/tickit-overview-full.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12678 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/images/tickit-simple-dag.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/images/tickit-simple-overview-with-system-simulation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/images/tickit-simple-overview.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/images/tickit-simple-simulation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/images/tickit-system-simulation-cpt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.039790 tickit-0.2.2/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.043790 tickit-0.2.2/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/user/explanations/adapters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/user/explanations/components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/user/explanations/devices.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/user/explanations/framework-summary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/user/explanations/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/user/explanations/wiring.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.043790 tickit-0.2.2/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/user/how-to/use-command-wrappers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/user/how-to/use-epics-adapter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.043790 tickit-0.2.2/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.043790 tickit-0.2.2/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/user/tutorials/create-a-device.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/user/tutorials/creating-a-simulation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/user/tutorials/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/user/tutorials/running-a-simulation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-06-16 14:45:28.000000 tickit-0.2.2/docs/user/tutorials/use-composed-adapter.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.027789 tickit-0.2.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.043790 tickit-0.2.2/examples/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-16 14:45:28.000000 tickit-0.2.2/examples/configs/amplifier.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-16 14:45:28.000000 tickit-0.2.2/examples/configs/counter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-16 14:45:28.000000 tickit-0.2.2/examples/configs/http-device.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-16 14:45:28.000000 tickit-0.2.2/examples/configs/isolated-device.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-16 14:45:28.000000 tickit-0.2.2/examples/configs/nested.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-16 14:45:28.000000 tickit-0.2.2/examples/configs/shutter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-16 14:45:28.000000 tickit-0.2.2/examples/configs/sunk-tcp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-16 14:45:28.000000 tickit-0.2.2/examples/configs/sunk-trampoline.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.043790 tickit-0.2.2/examples/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:28.000000 tickit-0.2.2/examples/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-06-16 14:45:28.000000 tickit-0.2.2/examples/devices/amplifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-16 14:45:28.000000 tickit-0.2.2/examples/devices/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-16 14:45:28.000000 tickit-0.2.2/examples/devices/http_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-06-16 14:45:28.000000 tickit-0.2.2/examples/devices/isolated_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 14:45:28.000000 tickit-0.2.2/examples/devices/isolated_record.db
+-rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-06-16 14:45:28.000000 tickit-0.2.2/examples/devices/remote_controlled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-16 14:45:28.000000 tickit-0.2.2/examples/devices/shutter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-06-16 14:45:28.000000 tickit-0.2.2/examples/devices/trampoline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3799 2023-06-16 14:45:28.000000 tickit-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 14:45:39.059791 tickit-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.027789 tickit-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.043790 tickit-0.2.2/src/tickit/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-16 14:45:38.000000 tickit-0.2.2/src/tickit/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.047790 tickit-0.2.2/src/tickit/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/adapters/composed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.047790 tickit-0.2.2/src/tickit/adapters/epicsadapter/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/adapters/epicsadapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/adapters/epicsadapter/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/adapters/epicsadapter/ioc_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/adapters/httpadapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.047790 tickit-0.2.2/src/tickit/adapters/interpreters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/adapters/interpreters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.047790 tickit-0.2.2/src/tickit/adapters/interpreters/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/adapters/interpreters/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/adapters/interpreters/command/command_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/adapters/interpreters/command/regex_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.047790 tickit-0.2.2/src/tickit/adapters/interpreters/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/adapters/interpreters/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/adapters/interpreters/endpoints/http_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/adapters/interpreters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.047790 tickit-0.2.2/src/tickit/adapters/interpreters/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/adapters/interpreters/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/adapters/interpreters/wrappers/beheading_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/adapters/interpreters/wrappers/joining_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/adapters/interpreters/wrappers/splitting_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.047790 tickit-0.2.2/src/tickit/adapters/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/adapters/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/adapters/servers/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/adapters/zmqadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.047790 tickit-0.2.2/src/tickit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/core/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.051790 tickit-0.2.2/src/tickit/core/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/core/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/core/components/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/core/components/device_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/core/components/system_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/core/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.051790 tickit-0.2.2/src/tickit/core/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/core/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/core/management/event_router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.051790 tickit-0.2.2/src/tickit/core/management/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/core/management/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/core/management/schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/core/management/schedulers/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/core/management/schedulers/slave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/core/management/ticker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/core/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.051790 tickit-0.2.2/src/tickit/core/state_interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/core/state_interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/core/state_interfaces/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/core/state_interfaces/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/core/state_interfaces/state_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/core/typedefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.051790 tickit-0.2.2/src/tickit/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/devices/iobox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/devices/sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/devices/source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.051790 tickit-0.2.2/src/tickit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/utils/byte_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.051790 tickit-0.2.2/src/tickit/utils/compat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/utils/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/utils/compat/functools_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/utils/compat/typing_compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.051790 tickit-0.2.2/src/tickit/utils/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/utils/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/utils/configuration/configurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/utils/configuration/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/utils/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-16 14:45:28.000000 tickit-0.2.2/src/tickit/utils/topic_naming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.047790 tickit-0.2.2/src/tickit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18638 2023-06-16 14:45:38.000000 tickit-0.2.2/src/tickit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-06-16 14:45:39.000000 tickit-0.2.2/src/tickit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 14:45:38.000000 tickit-0.2.2/src/tickit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-16 14:45:38.000000 tickit-0.2.2/src/tickit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-16 14:45:38.000000 tickit-0.2.2/src/tickit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 14:45:38.000000 tickit-0.2.2/src/tickit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.051790 tickit-0.2.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.055791 tickit-0.2.2/tests/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.055791 tickit-0.2.2/tests/adapters/interpreters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.055791 tickit-0.2.2/tests/adapters/interpreters/command/
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/adapters/interpreters/command/test_command_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/adapters/interpreters/command/test_regex_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.055791 tickit-0.2.2/tests/adapters/interpreters/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/adapters/interpreters/endpoints/test_http_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/adapters/interpreters/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.055791 tickit-0.2.2/tests/adapters/interpreters/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/adapters/interpreters/wrappers/test_beheading_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/adapters/interpreters/wrappers/test_joining_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/adapters/interpreters/wrappers/test_splitting_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.055791 tickit-0.2.2/tests/adapters/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/adapters/servers/test_tcp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.055791 tickit-0.2.2/tests/adapters/test_epicsadapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/adapters/test_epicsadapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/adapters/test_epicsadapter/test_epics_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/adapters/test_httpadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/adapters/test_zmqadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.055791 tickit-0.2.2/tests/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.055791 tickit-0.2.2/tests/core/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/core/components/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/core/components/test_device_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/core/components/test_system_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.055791 tickit-0.2.2/tests/core/management/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.055791 tickit-0.2.2/tests/core/management/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/core/management/schedulers/test_base_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/core/management/schedulers/test_master_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/core/management/schedulers/test_slave_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/core/management/test_event_router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/core/management/test_ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.055791 tickit-0.2.2/tests/core/state_interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/core/state_interfaces/test_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/core/state_interfaces/test_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/core/state_interfaces/test_state_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/core/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/core/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/core/test_typedefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.055791 tickit-0.2.2/tests/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/devices/test_iobox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/devices/test_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/devices/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.055791 tickit-0.2.2/tests/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:45:39.055791 tickit-0.2.2/tests/utils/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/utils/configuration/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/utils/test_byte_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/utils/test_configurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/utils/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-16 14:45:28.000000 tickit-0.2.2/tests/utils/test_topic_naming.py
```

### Comparing `tickit-0.2.1/.devcontainer/devcontainer.json` & `tickit-0.2.2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/.github/CONTRIBUTING.rst` & `tickit-0.2.2/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/.github/actions/install_requirements/action.yml` & `tickit-0.2.2/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/.github/dependabot.yml` & `tickit-0.2.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/.github/pages/make_switcher.py` & `tickit-0.2.2/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/.github/workflows/code.yml` & `tickit-0.2.2/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/.github/workflows/docs.yml` & `tickit-0.2.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/.github/workflows/docs_clean.yml` & `tickit-0.2.2/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/.github/workflows/linkcheck.yml` & `tickit-0.2.2/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/.gitignore` & `tickit-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/.gitlab-ci.yml` & `tickit-0.2.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/.vscode/launch.json` & `tickit-0.2.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/.vscode/settings.json` & `tickit-0.2.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/CHANGELOG.rst` & `tickit-0.2.2/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/Dockerfile` & `tickit-0.2.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/LICENSE` & `tickit-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/PKG-INFO` & `tickit-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tickit
-Version: 0.2.1
+Version: 0.2.2
 Summary: Event-based device simulation framework
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -301,15 +301,15 @@
         def __init__(self, initial_value: int = 0, callback_period: int = int(1e9)) -> None:
             self._value = initial_value
             self.callback_period = SimTime(callback_period)
             LOGGER.debug(f"Counter initialized with value => {self._value}")
 
         def update(self, time: SimTime, inputs: Inputs) -> DeviceUpdate[Outputs]:
             self._value = self._value + 1
-            LOGGER.debug("Counter incremented to {}".format(self._value))
+            LOGGER.debug(f"Counter incremented to {self._value}")
             return DeviceUpdate(
                 CounterDevice.Outputs(value=self._value),
                 SimTime(time + self.callback_period),
             )
 
 .. |code_ci| image:: https://github.com/dls-controls/tickit/workflows/Code%20CI/badge.svg?branch=master
     :target: https://github.com/dls-controls/tickit/actions?query=workflow%3A%22Code+CI%22
```

### Comparing `tickit-0.2.1/README.rst` & `tickit-0.2.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         def __init__(self, initial_value: int = 0, callback_period: int = int(1e9)) -> None:
             self._value = initial_value
             self.callback_period = SimTime(callback_period)
             LOGGER.debug(f"Counter initialized with value => {self._value}")
 
         def update(self, time: SimTime, inputs: Inputs) -> DeviceUpdate[Outputs]:
             self._value = self._value + 1
-            LOGGER.debug("Counter incremented to {}".format(self._value))
+            LOGGER.debug(f"Counter incremented to {self._value}")
             return DeviceUpdate(
                 CounterDevice.Outputs(value=self._value),
                 SimTime(time + self.callback_period),
             )
 
 .. |code_ci| image:: https://github.com/dls-controls/tickit/workflows/Code%20CI/badge.svg?branch=master
     :target: https://github.com/dls-controls/tickit/actions?query=workflow%3A%22Code+CI%22
```

### Comparing `tickit-0.2.1/docs/_static/theme_overrides.css` & `tickit-0.2.2/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/conf.py` & `tickit-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/developer/explanations/decisions.rst` & `tickit-0.2.2/docs/developer/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/developer/explanations/framework-details.rst` & `tickit-0.2.2/docs/developer/explanations/framework-details.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/developer/explanations/how-component-updates-are-ordered.rst` & `tickit-0.2.2/docs/developer/explanations/how-component-updates-are-ordered.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/developer/explanations/why-tickit.rst` & `tickit-0.2.2/docs/developer/explanations/why-tickit.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/developer/how-to/build-docs.rst` & `tickit-0.2.2/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/developer/how-to/lint.rst` & `tickit-0.2.2/docs/developer/how-to/lint.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/developer/how-to/make-release.rst` & `tickit-0.2.2/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/developer/how-to/pin-requirements.rst` & `tickit-0.2.2/docs/developer/how-to/pin-requirements.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/developer/how-to/test-container.rst` & `tickit-0.2.2/docs/developer/how-to/test-container.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/developer/how-to/update-tools.rst` & `tickit-0.2.2/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/developer/index.rst` & `tickit-0.2.2/docs/developer/index.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/developer/reference/standards.rst` & `tickit-0.2.2/docs/developer/reference/standards.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/developer/tutorials/dev-install.rst` & `tickit-0.2.2/docs/developer/tutorials/dev-install.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/images/example-systems.drawio.svg` & `tickit-0.2.2/docs/images/example-systems.drawio.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/images/tickit-create-device-amplifier.svg` & `tickit-0.2.2/docs/images/tickit-create-device-amplifier.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/images/tickit-device-simulation-cpt.svg` & `tickit-0.2.2/docs/images/tickit-device-simulation-cpt.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/images/tickit-logo.ico` & `tickit-0.2.2/docs/images/tickit-logo.ico`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/images/tickit-logo.svg` & `tickit-0.2.2/docs/images/tickit-logo.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/images/tickit-overview-full.svg` & `tickit-0.2.2/docs/images/tickit-overview-full.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/images/tickit-simple-dag.svg` & `tickit-0.2.2/docs/images/tickit-simple-dag.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/images/tickit-simple-overview-with-system-simulation.svg` & `tickit-0.2.2/docs/images/tickit-simple-overview-with-system-simulation.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/images/tickit-simple-overview.svg` & `tickit-0.2.2/docs/images/tickit-simple-overview.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/images/tickit-simple-simulation.svg` & `tickit-0.2.2/docs/images/tickit-simple-simulation.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/images/tickit-system-simulation-cpt.svg` & `tickit-0.2.2/docs/images/tickit-system-simulation-cpt.svg`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/index.rst` & `tickit-0.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/user/explanations/adapters.rst` & `tickit-0.2.2/docs/user/explanations/adapters.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/user/explanations/components.rst` & `tickit-0.2.2/docs/user/explanations/components.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/user/explanations/devices.rst` & `tickit-0.2.2/docs/user/explanations/devices.rst`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             Returns:
                 DeviceUpdate[Outputs]:
                     The produced update event which contains the value of the random output,
                     and requests a callback after the configured callback period.
             """
             output = randint(0, 255)
             LOGGER.debug(
-                "Boing! (delta: {}, inputs: {}, output: {})".format(time, inputs, output)
+                f"Boing! (delta: {time}, inputs: {inputs}, output: {output})"
             )
             return DeviceUpdate(
                 RandomTrampolineDevice.Outputs(output=output),
                 SimTime(time + self.callback_period),
             )
```

### Comparing `tickit-0.2.1/docs/user/explanations/framework-summary.rst` & `tickit-0.2.2/docs/user/explanations/framework-summary.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/user/explanations/glossary.rst` & `tickit-0.2.2/docs/user/explanations/glossary.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/user/explanations/wiring.rst` & `tickit-0.2.2/docs/user/explanations/wiring.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/user/how-to/use-command-wrappers.rst` & `tickit-0.2.2/docs/user/how-to/use-command-wrappers.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/user/how-to/use-epics-adapter.rst` & `tickit-0.2.2/docs/user/how-to/use-epics-adapter.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/user/index.rst` & `tickit-0.2.2/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/user/reference/api.rst` & `tickit-0.2.2/docs/user/reference/api.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/user/tutorials/create-a-device.rst` & `tickit-0.2.2/docs/user/tutorials/create-a-device.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/user/tutorials/creating-a-simulation.rst` & `tickit-0.2.2/docs/user/tutorials/creating-a-simulation.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/user/tutorials/installation.rst` & `tickit-0.2.2/docs/user/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/user/tutorials/running-a-simulation.rst` & `tickit-0.2.2/docs/user/tutorials/running-a-simulation.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/docs/user/tutorials/use-composed-adapter.rst` & `tickit-0.2.2/docs/user/tutorials/use-composed-adapter.rst`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/examples/configs/nested.yaml` & `tickit-0.2.2/examples/configs/nested.yaml`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/examples/devices/amplifier.py` & `tickit-0.2.2/examples/devices/amplifier.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/examples/devices/counter.py` & `tickit-0.2.2/examples/devices/counter.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,12 +47,12 @@
 
         Returns:
             DeviceUpdate[Outputs]:
                 The produced update event which contains the incremented value, and
                 requests a callback after callback_period.
         """
         self._value = self._value + 1
-        LOGGER.debug("Counter incremented to {}".format(self._value))
+        LOGGER.debug(f"Counter incremented to {self._value}")
         return DeviceUpdate(
             CounterDevice.Outputs(value=self._value),
             SimTime(time + self.callback_period),
         )
```

### Comparing `tickit-0.2.1/examples/devices/http_device.py` & `tickit-0.2.2/examples/devices/http_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         Args:
             request (web.Request): [description]
 
         Returns:
             web.Response: [description]
         """
-        return web.Response(text="Your data: {}".format(request.match_info["data"]))
+        return web.Response(text=f"Your data: {request.match_info['data']}")
 
 
 @dataclass
 class ExampleHTTP(ComponentConfig):
     """Example HTTP device."""
 
     foo: bool = False
```

### Comparing `tickit-0.2.1/examples/devices/remote_controlled.py` & `tickit-0.2.2/examples/devices/remote_controlled.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,16 +43,15 @@
                 Defaults to 3.14.
         """
         self.observed = initial_observed
         self.unobserved = initial_unobserved
         self.hidden = initial_hidden
 
     def update(self, time: SimTime, inputs: Inputs) -> DeviceUpdate[Outputs]:
-        """The update method which produces an output mapping containing the observed
-        value.
+        """Produces an output mapping containing the observed value.
 
         Args:
             time (SimTime): The current simulation time (in nanoseconds).
             inputs (State): A mapping of inputs to the device and their values.
 
         Returns:
             DeviceUpdate[Outputs]:
@@ -82,24 +81,23 @@
         """
         super().__init__(
             server,
             CommandInterpreter(),
         )
 
     async def on_connect(self) -> AsyncIterable[Optional[bytes]]:
-        """An on_connect method which continiously sends the unobserved value to the
-        client.
+        """Continiously sends the unobserved value to the client.
 
         Returns:
             AsyncIterable[bytes]:
                 An asynchronous iterable which regularly outputs the unobserved value.
         """
         while True:
             await asyncio.sleep(5.0)
-            yield "U is {}".format(self.device.unobserved).encode("utf-8")
+            yield f"U is {self.device.unobserved}".encode("utf-8")
 
     @RegexCommand(b"\x01")
     async def get_observed_bytes(self) -> bytes:
         """A regex bytes command which returns the byte encoded value of observed.
 
         Returns:
             bytes: The big endian float encoded value of observed.
@@ -135,15 +133,15 @@
         Args:
             value (int): The new value of observed.
 
         Returns:
             bytes: The utf-8 encoded value of observed.
         """
         self.device.observed = value
-        return "Observed set to {}".format(self.device.observed).encode("utf-8")
+        return f"Observed set to {self.device.observed}".encode("utf-8")
 
     @RegexCommand(b"\x02")
     async def get_unobserved_bytes(self) -> bytes:
         """A regex bytes command which returns the byte encoded value of unobserved.
 
         Returns:
             bytes: The big endian float encoded value of unobserved.
@@ -179,15 +177,15 @@
         Args:
             value (int): The new value of unobserved.
 
         Returns:
             bytes: The utf-8 encoded value of unobserved.
         """
         self.device.unobserved = value
-        return "Unobserved set to {}".format(self.device.unobserved).encode("utf-8")
+        return f"Unobserved set to {self.device.unobserved}".encode("utf-8")
 
     @RegexCommand(chr(0x1F95A), format="utf-8")
     async def misc(self) -> bytes:
         """A regex string command which returns a utf-8 encoded character.
 
         Returns:
             bytes: A utf-8 encoded character.
@@ -197,15 +195,15 @@
     @RegexCommand(r"H=(\d+\.?\d*)", format="utf-8")
     async def set_hidden(self, value: float) -> None:
         """A regex string command which sets the value of hidden.
 
         Args:
             value (float): The new value of hidden.
         """
-        LOGGER.info("Hidden set to {}".format(self.device.hidden))
+        LOGGER.info(f"Hidden set to {self.device.hidden}")
 
     @RegexCommand(r"H", format="utf-8")
     async def get_hidden(self) -> None:
         """A regex string command which returns nothing, hidden cannot be shown."""
         pass
 
     @RegexCommand(r"O\?(\d+)", format="utf-8")
@@ -218,15 +216,15 @@
         Returns:
             AsyncIterable[bytes]:
                 An asynchronous iterable which yields the value of observed the
                 specified number of times with a fixed delay.
         """
         for i in range(1, int(n)):
             await asyncio.sleep(1.0)
-            yield "Observed is {}".format(self.device.observed).encode("utf-8")
+            yield f"Observed is {self.device.observed}".encode("utf-8")
 
 
 @dataclass
 class RemoteControlled(ComponentConfig):
     """Thing you can poke over TCP."""
 
     format: ByteFormat = ByteFormat(b"%b\r\n")
```

### Comparing `tickit-0.2.1/examples/devices/shutter.py` & `tickit-0.2.2/examples/devices/shutter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/examples/devices/trampoline.py` & `tickit-0.2.2/examples/devices/trampoline.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             inputs (State): A mapping of inputs to the device and their values.
 
         Returns:
             DeviceUpdate[Outputs]:
                 The produced update event which never contains any changes, and
                 requests a callback after the configured callback period.
         """
-        LOGGER.debug("Boing! ({}, {})".format(time, inputs))
+        LOGGER.debug(f"Boing! ({time}, {inputs})")
         return DeviceUpdate(
             TrampolineDevice.Outputs(), SimTime(time + self.callback_period)
         )
 
 
 class RandomTrampolineDevice(Device):
     """A trivial toy device which produced a random output and requests a callback."""
@@ -80,17 +80,15 @@
 
         Returns:
             DeviceUpdate[Outputs]:
                 The produced update event which contains the value of the random output,
                 and requests a callback after the configured callback period.
         """
         output = randint(0, 255)
-        LOGGER.debug(
-            "Boing! (delta: {}, inputs: {}, output: {})".format(time, inputs, output)
-        )
+        LOGGER.debug(f"Boing! (delta: {time}, inputs: {inputs}, output: {output})")
         return DeviceUpdate(
             RandomTrampolineDevice.Outputs(output=output),
             SimTime(time + self.callback_period),
         )
 
 
 @dataclass
```

### Comparing `tickit-0.2.1/pyproject.toml` & `tickit-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,15 @@
     "F811", # support typing.overload decorator
     "F722", # allow Annotated[typ, some_func("some string")]
 ]
 max-line-length = 88 # Respect black's line length (default 88),
 exclude = [".tox", "venv"]
 
 [tool.pydocstyle]
+convention = "google"
 add-ignore = [
     "D100", # Ignore missing docstrings in public modules
     "D104", # Ignore missing docstrings in public packages
     "D418", # Ignore missing docstrings in dunder methods; See: https://github.com/PyCQA/pydocstyle/issues/525
 ]
 
 [tool.pytest.ini_options]
```

### Comparing `tickit-0.2.1/src/tickit/adapters/composed.py` & `tickit-0.2.2/src/tickit/adapters/composed.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,26 +16,24 @@
     protocol to a server and message handling to an interpreter.
     """
 
     server: Server
     interpreter: Interpreter
 
     async def on_connect(self) -> AsyncIterable[Optional[T]]:
-        """An overridable asynchronous iterable which yields messages on client
-        connection.
+        """Overridable asynchronous iterable which yields messages on client connection.
 
         Returns:
             AsyncIterable[Optional[T]]: An asynchronous iterable of messages.
         """
         if False:
             yield None
 
     async def handle_message(self, message: T) -> AsyncIterable[Optional[T]]:
-        """Delegates message handling to the interpreter and raises interrupt if
-        requested.
+        """Delegates message handling to the interpreter, raises interrupt if requested.
 
         Args:
             message (T): The message from the server to be handled.
 
         Returns:
             AsyncIterable[Optional[T]]: An asynchronous iterable of reply messages.
         """
```

### Comparing `tickit-0.2.1/src/tickit/adapters/epicsadapter/adapter.py` & `tickit-0.2.2/src/tickit/adapters/epicsadapter/adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         self.interrupt_records[record] = getter
 
     def after_update(self) -> None:
         """Updates IOC records immediately following a device update."""
         for record, getter in self.interrupt_records.items():
             current_value = getter()
             record.set(current_value)
-            print("Record {} updated to : {}".format(record.name, current_value))
+            print(f"Record {record.name} updated to : {current_value}")
 
     @abstractmethod
     def on_db_load(self) -> None:
         """Customises records that have been loaded in to suit the simulation."""
         raise NotImplementedError
 
     def load_records_without_DTYP_fields(self):
```

### Comparing `tickit-0.2.1/src/tickit/adapters/epicsadapter/ioc_manager.py` & `tickit-0.2.2/src/tickit/adapters/epicsadapter/ioc_manager.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/src/tickit/adapters/httpadapter.py` & `tickit-0.2.2/src/tickit/adapters/httpadapter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/src/tickit/adapters/interpreters/command/command_interpreter.py` & `tickit-0.2.2/src/tickit/adapters/interpreters/command/command_interpreter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/src/tickit/adapters/interpreters/command/regex_command.py` & `tickit-0.2.2/src/tickit/adapters/interpreters/command/regex_command.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/src/tickit/adapters/interpreters/endpoints/http_endpoint.py` & `tickit-0.2.2/src/tickit/adapters/interpreters/endpoints/http_endpoint.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/src/tickit/adapters/interpreters/utils.py` & `tickit-0.2.2/src/tickit/adapters/interpreters/utils.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/src/tickit/adapters/interpreters/wrappers/beheading_interpreter.py` & `tickit-0.2.2/src/tickit/adapters/interpreters/wrappers/beheading_interpreter.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,16 +21,15 @@
         super().__init__()
         self.interpreter: Interpreter[AnyStr] = interpreter
         self.header_size: int = header_size
 
     async def handle(
         self, adapter: Adapter, message: AnyStr
     ) -> Tuple[AsyncIterable[AnyStr], bool]:
-        """Removes a header from the start of a message, and passes it on to an
-        interpreter.
+        """Removes a header from a message and passes the message on to an interpreter.
 
         Args:
             adapter (Adapter): The adapter in which the function should be executed
             message: (AnyStr): The handled message, of which the header is removed.
 
         Returns:
             Tuple[AsyncIterable[Union[str, bytes]], bool]:
```

### Comparing `tickit-0.2.1/src/tickit/adapters/interpreters/wrappers/joining_interpreter.py` & `tickit-0.2.2/src/tickit/adapters/interpreters/wrappers/joining_interpreter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/src/tickit/adapters/interpreters/wrappers/splitting_interpreter.py` & `tickit-0.2.2/src/tickit/adapters/interpreters/wrappers/splitting_interpreter.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,15 @@
     """
 
     def __init__(
         self,
         interpreter: Interpreter[AnyStr],
         message_delimiter: AnyStr,
     ) -> None:
-        """A decorator for an interpreter that splits a message into multiple
-        sub-messages.
+        """An interpreter decorator that splits a message into multiple sub-messages.
 
         Args:
             interpreter (Interpreter): The interpreter messages are passed on to.
             message_delimiter (AnyStr): The delimiter by which the message is split up.
                 Can be a regex pattern. Must be of the same type as the message.
         """
         super().__init__()
```

### Comparing `tickit-0.2.1/src/tickit/adapters/servers/tcp.py` & `tickit-0.2.2/src/tickit/adapters/servers/tcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,27 +77,27 @@
         tasks: List[asyncio.Task] = list()
 
         async def handle(reader: StreamReader, writer: StreamWriter) -> None:
             async def reply(replies: AsyncIterable[Optional[bytes]]) -> None:
                 async for reply in replies:
                     if reply is None:
                         continue
-                    LOGGER.debug("Replying with {!r}".format(reply))
+                    LOGGER.debug(f"Replying with {reply!r}")
                     writer.write(self.format % reply)
                     if writer.is_closing():
                         break
                     await writer.drain()
 
             tasks.append(asyncio.create_task(reply(on_connect())))
 
             while True:
                 data: bytes = await reader.read(1024)
                 if data == b"":
                     break
                 addr = writer.get_extra_info("peername")
 
-                LOGGER.debug("Recieved {!r} from {}".format(data, addr))
+                LOGGER.debug(f"Recieved {data!r} from {addr}")
                 tasks.append(asyncio.create_task(reply(await handler(data))))
 
             await asyncio.wait(tasks)
 
         return handle
```

### Comparing `tickit-0.2.1/src/tickit/adapters/zmqadapter.py` & `tickit-0.2.2/src/tickit/adapters/zmqadapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,17 +80,17 @@
         while running:
             message = await self._message_queue.get()
             await self._process_message(message)
             running = self.check_if_running()
 
     async def _process_message(self, message: str) -> None:
         if message is not None:
-            LOGGER.debug("Data from ZMQ stream: {!r}".format(message))
+            LOGGER.debug(f"Data from ZMQ stream: {message!r}")
 
             msg = (b"Data", str(message).encode("utf-8"))
             self._dealer.write(msg)
             data = await self._router.read()
             self._router.write(data)
             answer = await self._dealer.read()
-            LOGGER.debug("Received {!r}".format(answer))
+            LOGGER.debug(f"Received {answer!r}")
         else:
             LOGGER.debug("No message")
```

### Comparing `tickit-0.2.1/src/tickit/cli.py` & `tickit-0.2.2/src/tickit/cli.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/src/tickit/core/adapter.py` & `tickit-0.2.2/src/tickit/core/adapter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/src/tickit/core/components/component.py` & `tickit-0.2.2/src/tickit/core/components/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,38 +119,37 @@
                 requests to be awoken.
         """
         await self.state_producer.produce(
             output_topic(self.name), Output(self.name, time, changes, call_at)
         )
 
     async def raise_interrupt(self) -> None:
-        """Send an Interrupt message to the component output topic.
+        """Sends an Interrupt message to the component output topic.
 
         An asynchronous method whicb constructs an Interrupt message tagged with the
         component name and sends it to the output topic of this component.
         """
         await self.state_producer.produce(output_topic(self.name), Interrupt(self.name))
 
     async def run_forever(
         self, state_consumer: Type[StateConsumer], state_producer: Type[StateProducer]
     ) -> None:
-        """Create and configures a state consumer and state producer.
+        """Creates and configures a state consumer and state producer.
 
         An asynchronous method which creates a state consumer which is subscribed to
         the input topic of the component and calls back to handle_input, and a state
         producer to produce Interrupt, Output or ComponentException messages.
         """
         self.state_consumer = state_consumer(self.handle_input)
         await self.state_consumer.subscribe([input_topic(self.name)])
         self.state_producer = state_producer()
 
     @abstractmethod
     async def on_tick(self, time: SimTime, changes: Changes):
-        """An abstract asynchronous method which implements the core logic of the
-        component.
+        """Abstract asynchronous method which implements core logic of the component.
 
         Args:
             time (SimTime): The current simulation time (in nanoseconds).
             changes (Changes): A mapping of changed component inputs and their new
                 values.
         """
         raise NotImplementedError
```

### Comparing `tickit-0.2.1/src/tickit/core/components/device_simulation.py` & `tickit-0.2.2/src/tickit/core/components/device_simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,10 +82,10 @@
         await self.output(time, out_changes, device_update.call_at)
 
     async def stop_component(self) -> None:
         """Cancel all pending tasks associated with the device component.
 
         Cancels long running adapter tasks associated with the component.
         """
-        LOGGER.debug("Stopping {}".format(self.name))
+        LOGGER.debug(f"Stopping {self.name}")
         for task in self._tasks:
             task.cancel()
```

### Comparing `tickit-0.2.1/src/tickit/core/components/system_simulation.py` & `tickit-0.2.2/src/tickit/core/components/system_simulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,16 +33,15 @@
     expose: Dict[PortID, ComponentPort]
 
     _tasks: List[asyncio.Task] = field(default_factory=list)
 
     async def run_forever(
         self, state_consumer: Type[StateConsumer], state_producer: Type[StateProducer]
     ) -> None:
-        """Sets up state interfaces, the scheduler, and components and blocks until any
-        complete.
+        """Sets up state interfaces, the scheduler, and components to run continuously.
 
         An asynchronous method starts the run_forever method of each component, runs
         the scheduler, and sets up externally facing state interfaces. The method
         blocks until and of the components or the scheduler complete.
         """
         inverse_wiring = InverseWiring.from_component_configs(self.components)
         self.scheduler = SlaveScheduler(
@@ -90,15 +89,15 @@
             await self.output(time, output_changes, call_in)
 
     async def stop_component(self) -> None:
         """Cancel all pending tasks associated with the System Simulation component.
 
         Cancels long running adapter tasks associated with the component.
         """
-        LOGGER.debug("Stopping {}".format(self.name))
+        LOGGER.debug(f"Stopping {self.name}")
         for task in self._tasks:
             task.cancel()
 
 
 @dataclass
 class SystemSimulation(ComponentConfig):
     """Simulation of a nested set of components."""
```

### Comparing `tickit-0.2.1/src/tickit/core/device.py` & `tickit-0.2.2/src/tickit/core/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 @as_tagged_union
 class Device(ABC, Generic[InMap, OutMap]):
     """An interface for types which implement simulated devices."""
 
     @abstractmethod
     def update(self, time: SimTime, inputs: InMap) -> DeviceUpdate[OutMap]:
-        """A method which implements device behaviour according to the time and its
-        inputs.
+        """Implements device behaviour according to the time and its inputs.
 
         A method which implements the (typically physics based) changes which occur
         within the device in response to either the progression of time or the
         alteration of inputs to the device. The method returns the new observable state
         of the device and may optionally include a time in which the method should be
         called again.
```

### Comparing `tickit-0.2.1/src/tickit/core/management/event_router.py` & `tickit-0.2.2/src/tickit/core/management/event_router.py`

 * *Files 3% similar despite different names*

```diff
@@ -165,15 +165,19 @@
     @cached_property
     def components(self) -> Set[ComponentID]:
         """A cached set of all components in the wiring.
 
         Returns:
             Set[ComponentID]: A set of all components in the wiring.
         """
-        return set.union(self.input_components, self.output_components)
+        return set.union(
+            self.input_components,
+            self.output_components,
+            self.isolated_components,
+        )
 
     @cached_property
     def output_components(self) -> Set[ComponentID]:
         """A cached set of components which provide outputs.
 
         Returns:
             Set[ComponentID]: A set of components which provide outputs.
@@ -191,14 +195,26 @@
             dev
             for out in self.wiring.values()
             for port in out.values()
             for dev, _ in port
         )
 
     @cached_property
+    def isolated_components(self) -> Set[ComponentID]:
+        """A cached set of components without inputs or outputs.
+
+        Returns:
+            Set[ComponentID]: A set of components which are isolated
+        """
+        return set.difference(
+            set(self.wiring.keys()),
+            set.union(self.input_components, self.output_components),
+        )
+
+    @cached_property
     def component_tree(self) -> Dict[ComponentID, Set[ComponentID]]:
         """A cached mapping of first order component dependants.
 
         A cached property which returns a mapping of components to the set of
         components which are wired to any of its outputs.
 
         Returns:
@@ -228,15 +244,17 @@
         }
         for dev, deps in self.component_tree.items():
             for dep in deps:
                 inverse_tree[dep].add(dev)
         return inverse_tree
 
     def dependants(self, root: ComponentID) -> Set[ComponentID]:
-        """Finds the set of all components which are recursively dependant on the root
+        """Finds the set of root component dependents .
+
+        Finds the set of all components which are recursively dependant on the root
         component.
 
         Args:
             root (ComponentID): The root component.
 
         Returns:
             Set[ComponentID]:
```

### Comparing `tickit-0.2.1/src/tickit/core/management/schedulers/base.py` & `tickit-0.2.2/src/tickit/core/management/schedulers/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,17 @@
         self._state_producer_cls = state_producer
         self.wakeups: Dict[ComponentID, SimTime] = dict()
 
         self.error = asyncio.Event()
 
     @abstractmethod
     async def schedule_interrupt(self, source: ComponentID) -> None:
-        """An abstract asynchronous method which should schedule an interrupt
+        """An abstract asynchronous method which should schedule an interrupt.
+
+        When implemented in a child this method should schedule an interrupt
         immediately.
 
         Args:
             source (ComponentID): The component which should be updated.
         """
         raise NotImplementedError
 
@@ -76,15 +78,15 @@
         exceptions, a StopComponent message is produced to each component in the system
         to facilitate shut down.
 
         Args:
             message (Union[Interrupt, Output, ComponentException]): An Interrupt,
                 Output or ComponentException recieved by the state consumer.
         """
-        LOGGER.debug("Scheduler ({}) got {}".format(type(self).__name__, message))
+        LOGGER.debug(f"Scheduler ({type(self).__name__}) got {message}")
         if isinstance(message, Output):
             await self.ticker.propagate(message)
             if message.call_at is not None:
                 self.add_wakeup(message.source, message.call_at)
         elif isinstance(message, Interrupt):
             await self.schedule_interrupt(message.source)
         elif isinstance(message, ComponentException):
@@ -111,15 +113,15 @@
     def add_wakeup(self, component: ComponentID, when: SimTime) -> None:
         """Adds a wakeup to the mapping.
 
         Args:
             component (ComponentID): The component which should be updated.
             when (SimTime): The simulation time at which the update should occur.
         """
-        LOGGER.debug("Scheduling {} for wakeup at {}".format(component, when))
+        LOGGER.debug(f"Scheduling {component} for wakeup at {when}")
         self.wakeups[component] = when
 
     def get_first_wakeups(self) -> Tuple[Set[ComponentID], Optional[SimTime]]:
         """Gets the components which are due for update first and the wakeup time.
 
         A method which returns a set of components which are due for update first and
         the simulation time at which the updates are scheduled. Or an empty set and
```

### Comparing `tickit-0.2.1/src/tickit/core/management/schedulers/master.py` & `tickit-0.2.2/src/tickit/core/management/schedulers/master.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,16 +56,15 @@
             component (ComponentID): The component which should be updated.
             when (SimTime): The simulation time at which the update should occur.
         """
         super().add_wakeup(component, when)
         self.new_wakeup.set()
 
     async def run_forever(self) -> None:
-        """Performs an intial tick then continiously schedules ticks according to
-        wakeups.
+        """Perform an intial tick then continiously schedule ticks according to wakeups.
 
         An asynchronous method which initially performs setup and an initial tick in
         which all components are updated, subsequently ticks are performed as requested
         by components of the simulation according to the simulation speed.
         """
         await self.setup()
         await self._do_initial_tick()
```

### Comparing `tickit-0.2.1/src/tickit/core/management/schedulers/slave.py` & `tickit-0.2.2/src/tickit/core/management/schedulers/slave.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,15 @@
         self,
         wiring: Union[Wiring, InverseWiring],
         state_consumer: Type[StateConsumer],
         state_producer: Type[StateProducer],
         expose: Dict[PortID, ComponentPort],
         raise_interrupt: Callable[[], Awaitable[None]],
     ) -> None:
-        """A slave scheduler constructor which adds wiring and saves values for
-        reference.
+        """Slave scheduler constructor which adds wiring and saves values for reference.
 
         Args:
             wiring (Union[Wiring, InverseWiring]): A wiring or inverse wiring object
                 representing the connections between components in the system.
             state_consumer (Type[StateConsumer]): The state consumer class to be used
                 by the component.
             state_producer (Type[StateProducer]): The state producer class to be used
@@ -77,16 +76,15 @@
         """
         if isinstance(wiring, Wiring):
             wiring = InverseWiring.from_wiring(wiring)
         wiring[ComponentID("expose")].update(expose)
         return wiring
 
     async def update_component(self, input: Input) -> None:
-        """Sends an input to the corresponding component. Mocks I/O for "external" or
-        "expose".
+        """Sends an input to the target component. Mocks I/O for "external" or "expose".
 
         For real components the input is sent in a message to their input topic, for
         the mock component named "external", external inputs are injected, whilst for
         the mock component and named "expose" the input is stored for use as the
         scheduler output.
 
         Args:
@@ -103,16 +101,15 @@
             )
         else:
             await super().update_component(input)
 
     async def on_tick(
         self, time: SimTime, changes: Changes
     ) -> Tuple[Changes, Optional[SimTime]]:
-        """Routes inputs, performs a tick and returns output changes and a callback
-        time.
+        """Routes inputs, does a tick and returns output changes and a callback time.
 
         An asyhcnronous method which determines which components within the simulation
         require being woken up, sets the input changes for use by the "external" mock
         component, performs a tick, determines the period in which the slave scheduler
         should next be updated, and returns the changes collated by the "expose" mock
         component.
 
@@ -155,15 +152,15 @@
 
         An asynchronous method which schedules an interrupt immediately by adding it to
         a set of queued interrupts and raising the interrupt to the master scheduler.
 
         Args:
             source (ComponentID): The source component of the interrupt.
         """
-        LOGGER.debug("Adding {} to interrupts".format(source))
+        LOGGER.debug(f"Adding {source} to interrupts")
         self.interrupts.add(source)
         await self.raise_interrupt()
 
     async def handle_component_exception(self, message: ComponentException) -> None:
         """Handle exceptions raised from componenets by shutting down the simulation.
 
         If a component inside a system simulation produces an exception, the slave
```

### Comparing `tickit-0.2.1/src/tickit/core/management/ticker.py` & `tickit-0.2.2/src/tickit/core/management/ticker.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             time (SimTime): The simulation time at which the tick occurs (in
                 nanoseconds).
             update_components (Set[ComponentID]): A set of components which require
                 update.
         """
         self.time = time
         self.roots = update_components
-        LOGGER.debug("Doing tick @ {}".format(self.time))
+        LOGGER.debug(f"Doing tick @ {self.time}")
         self.inputs: DefaultDict[ComponentID, Dict[PortID, Hashable]] = defaultdict(
             dict
         )
         self.to_update = {
             c: None
             for component in self.roots
             for c in self.event_router.dependants(component)
```

### Comparing `tickit-0.2.1/src/tickit/core/runner.py` & `tickit-0.2.2/src/tickit/core/runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     async def run_with_error_handling(awaitable: Awaitable[None]) -> None:
         try:
             await awaitable
         except Exception as e:
             # These are prints rather than logging because we just want the
             # result going directly to stdout.
-            print("Task exception: {}".format(e))
+            print(f"Task exception: {e}")
             print(traceback.format_exc())
 
     return [
         asyncio.create_task(run_with_error_handling(awaitable))
         for awaitable in awaitables
     ]
```

### Comparing `tickit-0.2.1/src/tickit/core/state_interfaces/internal.py` & `tickit-0.2.2/src/tickit/core/state_interfaces/internal.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,15 @@
                 topic.
         """
         self._topics[topic].append(message)
         for subscriber in self._subscribers[topic]:
             await subscriber.add_message(message)
 
     async def subscribe(self, consumer: "InternalStateConsumer", topics: Iterable[str]):
-        """Subscribes the consumer to the given topics, so it is notified a message is
-        added.
+        """Subscribes the consumer to the given topics.
 
         An asynchronous method which adds a consumer to the subscriber list of each
         topic in the topics iterable. On subscription, previous messages on the topic
         are immediately passed to the consumer.
 
         Args:
             consumer (InternalStateConsumer): The consumer which is subscribing to the
@@ -126,15 +125,17 @@
             callback (Callable[[C], Awaitable[None]]): An asynchronous handler function
                 for consumed values.
         """
         self.server = InternalStateServer()
         self.callback = callback
 
     async def subscribe(self, topics: Iterable[str]) -> None:
-        """Subscribes the consumer to the given topics, new messages are passed to the
+        """Subscribes the consumer to the given topics.
+
+        Subscribes the consumer to the given topics, new messages are passed to the
         callback.
 
         Args:
             topics (Iterable[str]): An iterable of topics to subscribe to.
         """
         await self.server.subscribe(self, topics)
```

### Comparing `tickit-0.2.1/src/tickit/core/state_interfaces/kafka.py` & `tickit-0.2.2/src/tickit/core/state_interfaces/kafka.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,17 @@
         """Starts the consumer and waits for messages to arrive."""
         await self.consumer.start()
         while True:
             async for message in self.consumer:
                 await self.callback(message.value)
 
     async def subscribe(self, topics: Iterable[str]):
-        """Subscribes the consumer to the given topics, new messages are passed to the
+        """Subscribes the consumer to the given topics.
+
+        Subscribes the consumer to the given topics, new messages are passed to the
         callback.
 
         Args:
             topics (Iterable[str]): An iterable of topics to subscribe to.
         """
         self.consumer.subscribe(topics)
```

### Comparing `tickit-0.2.1/src/tickit/core/state_interfaces/state_interface.py` & `tickit-0.2.2/src/tickit/core/state_interfaces/state_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,17 +96,15 @@
     def wrap(interface: Type[StateInterface]) -> Type[StateInterface]:
         if isinstance(interface, StateProducer):
             producers[name] = (interface, external)
         elif isinstance(interface, StateConsumer):
             consumers[name] = (interface, external)
         else:
             warn(
-                RuntimeWarning(
-                    "{} is not {} or {}".format(interface, StateConsumer, StateProducer)
-                )
+                RuntimeWarning(f"{interface} is not {StateConsumer} or {StateProducer}")
             )
         return interface
 
     return wrap
 
 
 def interfaces(external: bool = False) -> Set[str]:
```

### Comparing `tickit-0.2.1/src/tickit/core/typedefs.py` & `tickit-0.2.2/src/tickit/core/typedefs.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,26 +29,30 @@
         Returns:
             str: A string representation of the object of format component:port.
         """
         return ":".join((self.component, self.port))
 
     @serializer
     def serialize(self) -> str:
-        """An apischema serialization method which returns a string of component:port.
+        """Returns a string of component:port.
+
+        An apischema serialization method which returns a string of component:port.
 
         Returns:
             str: The serialized ComponentPort, in format component:port.
         """
         return str(self)
 
     @deserializer
     @staticmethod
     def deserialize(data: str) -> "ComponentPort":
-        """An apischema deserialization method which builds a from a string of
-        component:port.
+        """Builds a ComponentPort from a string of component:port.
+
+        An apischema deserialization method which builds a ComponentPort from a string
+        of component:port.
 
         Returns:
             ComponentPort: The deserialized ComponentPort.
         """
         component, port = data.split(":")
         return ComponentPort(ComponentID(component), PortID(port))
```

### Comparing `tickit-0.2.1/src/tickit/devices/sink.py` & `tickit-0.2.2/src/tickit/devices/sink.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,27 +15,26 @@
 
     #: A typed mapping containing the 'input' input value
     Inputs: TypedDict = TypedDict("Inputs", {"input": Any})
     #: An empty typed mapping of device outputs
     Outputs: TypedDict = TypedDict("Outputs", {})
 
     def update(self, time: SimTime, inputs: Inputs) -> DeviceUpdate[Outputs]:
-        """The update method which logs the inputs at debug level and produces no
-        outputs.
+        """The update method which logs the inputs and produces no outputs.
 
         Args:
             time (SimTime): The current simulation time (in nanoseconds).
             inputs (State): A mapping of inputs to the device and their values.
 
         Returns:
             DeviceUpdate[Outputs]:
                 The produced update event which never contains any changes, and never
                 requests a callback.
         """
-        LOGGER.debug("Sunk {}".format({k: v for k, v in inputs.items()}))
+        LOGGER.debug(f"Sunk { {k: v for k, v in inputs.items()} }")
         return DeviceUpdate(SinkDevice.Outputs(), None)
 
 
 class Sink(ComponentConfig):
     """Arbitrary value sink that logs the value."""
 
     def __call__(self) -> Component:  # noqa: D102
```

### Comparing `tickit-0.2.1/src/tickit/devices/source.py` & `tickit-0.2.2/src/tickit/devices/source.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             inputs (State): A mapping of inputs to the device and their values.
 
         Returns:
             DeviceUpdate[Outputs]:
                 The produced update event which contains the pre-configured value, and
                 never requests a callback.
         """
-        LOGGER.debug("Sourced {}".format(self.value))
+        LOGGER.debug(f"Sourced {self.value}")
         return DeviceUpdate(SourceDevice.Outputs(value=self.value), None)
 
 
 @dataclass
 class Source(ComponentConfig):
     """Source of a fixed value."""
```

### Comparing `tickit-0.2.1/src/tickit/utils/byte_format.py` & `tickit-0.2.2/src/tickit/utils/byte_format.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/src/tickit/utils/configuration/configurable.py` & `tickit-0.2.2/src/tickit/utils/configuration/configurable.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,32 +26,32 @@
 
 
 #: Whether the current class is registered as a tagged union
 is_tagged_union: Dict[Type[Any], bool] = DefaultDict(lambda: False)
 
 
 def as_tagged_union(cls: Cls) -> Cls:
-    """A decorator to make a config base class which can deserialize aliased
-    sub-classes.
+    """A decorator to make a config base class that can deserialize aliased sub-classes.
 
     A decorator which makes a config class the root of a tagged union of sub-classes
     allowing for serialization and deserialization of config trees by class alias. The
     function registers both an apischema serialization and an apischema deserialization
     conversion for the base class which perform lookup based on a tagged union of
     aliased sub-classes.
 
     Args:
         cls (Cls): The config base class.
 
     Returns:
         Cls: The modified config base class.
     """
 
-    # This will only be used if we want to generate a json schema (which we will)
-    def deserialization() -> Conversion:
+    def deserialization() -> (
+        Conversion
+    ):  # This will only be used if we want to generate a json schema (which we will)
         annotations: Dict[str, Any] = {}
         deserialization_namespace: Dict[str, Any] = {"__annotations__": annotations}
         for sub in rec_subclasses(cls):
             fullname = sub.__module__ + "." + sub.__name__
             annotations[fullname] = Tagged[sub]  # type: ignore
         deserialization_union = type(
             cls.__name__ + "TaggedUnion",
```

### Comparing `tickit-0.2.1/src/tickit/utils/configuration/loading.py` & `tickit-0.2.2/src/tickit/utils/configuration/loading.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/src/tickit/utils/topic_naming.py` & `tickit-0.2.2/src/tickit/utils/topic_naming.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/src/tickit.egg-info/PKG-INFO` & `tickit-0.2.2/src/tickit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tickit
-Version: 0.2.1
+Version: 0.2.2
 Summary: Event-based device simulation framework
 Author-email: Callum Forrester <callum.forrester@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -301,15 +301,15 @@
         def __init__(self, initial_value: int = 0, callback_period: int = int(1e9)) -> None:
             self._value = initial_value
             self.callback_period = SimTime(callback_period)
             LOGGER.debug(f"Counter initialized with value => {self._value}")
 
         def update(self, time: SimTime, inputs: Inputs) -> DeviceUpdate[Outputs]:
             self._value = self._value + 1
-            LOGGER.debug("Counter incremented to {}".format(self._value))
+            LOGGER.debug(f"Counter incremented to {self._value}")
             return DeviceUpdate(
                 CounterDevice.Outputs(value=self._value),
                 SimTime(time + self.callback_period),
             )
 
 .. |code_ci| image:: https://github.com/dls-controls/tickit/workflows/Code%20CI/badge.svg?branch=master
     :target: https://github.com/dls-controls/tickit/actions?query=workflow%3A%22Code+CI%22
```

### Comparing `tickit-0.2.1/src/tickit.egg-info/SOURCES.txt` & `tickit-0.2.2/src/tickit.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -70,22 +70,25 @@
 docs/user/tutorials/creating-a-simulation.rst
 docs/user/tutorials/installation.rst
 docs/user/tutorials/running-a-simulation.rst
 docs/user/tutorials/use-composed-adapter.rst
 examples/configs/amplifier.yaml
 examples/configs/counter.yaml
 examples/configs/http-device.yaml
+examples/configs/isolated-device.yaml
 examples/configs/nested.yaml
 examples/configs/shutter.yaml
 examples/configs/sunk-tcp.yaml
 examples/configs/sunk-trampoline.yaml
 examples/devices/__init__.py
 examples/devices/amplifier.py
 examples/devices/counter.py
 examples/devices/http_device.py
+examples/devices/isolated_device.py
+examples/devices/isolated_record.db
 examples/devices/remote_controlled.py
 examples/devices/shutter.py
 examples/devices/trampoline.py
 src/tickit/__init__.py
 src/tickit/__main__.py
 src/tickit/_version.py
 src/tickit/cli.py
@@ -132,14 +135,15 @@
 src/tickit/core/management/schedulers/master.py
 src/tickit/core/management/schedulers/slave.py
 src/tickit/core/state_interfaces/__init__.py
 src/tickit/core/state_interfaces/internal.py
 src/tickit/core/state_interfaces/kafka.py
 src/tickit/core/state_interfaces/state_interface.py
 src/tickit/devices/__init__.py
+src/tickit/devices/iobox.py
 src/tickit/devices/sink.py
 src/tickit/devices/source.py
 src/tickit/utils/__init__.py
 src/tickit/utils/byte_format.py
 src/tickit/utils/singleton.py
 src/tickit/utils/topic_naming.py
 src/tickit/utils/compat/__init__.py
@@ -172,14 +176,15 @@
 tests/core/management/test_ticker.py
 tests/core/management/schedulers/test_base_scheduler.py
 tests/core/management/schedulers/test_master_scheduler.py
 tests/core/management/schedulers/test_slave_scheduler.py
 tests/core/state_interfaces/test_internal.py
 tests/core/state_interfaces/test_kafka.py
 tests/core/state_interfaces/test_state_interface.py
+tests/devices/test_iobox.py
 tests/devices/test_sink.py
 tests/devices/test_source.py
 tests/utils/test_byte_format.py
 tests/utils/test_configurable.py
 tests/utils/test_singleton.py
 tests/utils/test_topic_naming.py
 tests/utils/configuration/test_loading.py
```

### Comparing `tickit-0.2.1/tests/adapters/interpreters/command/test_command_interpreter.py` & `tickit-0.2.2/tests/adapters/interpreters/command/test_command_interpreter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/adapters/interpreters/command/test_regex_command.py` & `tickit-0.2.2/tests/adapters/interpreters/command/test_regex_command.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/adapters/interpreters/endpoints/test_http_endpoint.py` & `tickit-0.2.2/tests/adapters/interpreters/endpoints/test_http_endpoint.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/adapters/interpreters/test_utils.py` & `tickit-0.2.2/tests/adapters/interpreters/test_utils.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/adapters/interpreters/wrappers/test_beheading_interpreter.py` & `tickit-0.2.2/tests/adapters/interpreters/wrappers/test_beheading_interpreter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/adapters/interpreters/wrappers/test_joining_interpreter.py` & `tickit-0.2.2/tests/adapters/interpreters/wrappers/test_joining_interpreter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/adapters/interpreters/wrappers/test_splitting_interpreter.py` & `tickit-0.2.2/tests/adapters/interpreters/wrappers/test_splitting_interpreter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/adapters/servers/test_tcp.py` & `tickit-0.2.2/tests/adapters/servers/test_tcp.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/adapters/test_epicsadapter/test_epics_adapter.py` & `tickit-0.2.2/tests/adapters/test_epicsadapter/test_epics_adapter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/adapters/test_httpadapter.py` & `tickit-0.2.2/tests/adapters/test_httpadapter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/adapters/test_zmqadapter.py` & `tickit-0.2.2/tests/adapters/test_zmqadapter.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/conftest.py` & `tickit-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/core/components/test_component.py` & `tickit-0.2.2/tests/core/components/test_component.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/core/components/test_device_simulation.py` & `tickit-0.2.2/tests/core/components/test_device_simulation.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/core/components/test_system_simulation.py` & `tickit-0.2.2/tests/core/components/test_system_simulation.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/core/management/schedulers/test_base_scheduler.py` & `tickit-0.2.2/tests/core/management/schedulers/test_base_scheduler.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/core/management/schedulers/test_master_scheduler.py` & `tickit-0.2.2/tests/core/management/schedulers/test_master_scheduler.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/core/management/schedulers/test_slave_scheduler.py` & `tickit-0.2.2/tests/core/management/schedulers/test_slave_scheduler.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/core/management/test_ticker.py` & `tickit-0.2.2/tests/core/management/test_ticker.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/core/state_interfaces/test_internal.py` & `tickit-0.2.2/tests/core/state_interfaces/test_internal.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/core/state_interfaces/test_kafka.py` & `tickit-0.2.2/tests/core/state_interfaces/test_kafka.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/core/state_interfaces/test_state_interface.py` & `tickit-0.2.2/tests/core/state_interfaces/test_state_interface.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/core/test_typedefs.py` & `tickit-0.2.2/tests/core/test_typedefs.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/devices/test_sink.py` & `tickit-0.2.2/tests/devices/test_sink.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,8 +26,8 @@
     assert device_update.outputs == {}
     assert device_update.call_at is None
 
     assert len(caplog.records) == 1
     record: logging.LogRecord = caplog.records[0]
 
     assert record.levelname == "DEBUG"
-    assert record.message == "Sunk {}".format(inputs)
+    assert record.message == f"Sunk {inputs}"
```

### Comparing `tickit-0.2.1/tests/devices/test_source.py` & `tickit-0.2.2/tests/devices/test_source.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/test_cli.py` & `tickit-0.2.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/utils/configuration/test_loading.py` & `tickit-0.2.2/tests/utils/configuration/test_loading.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/utils/test_byte_format.py` & `tickit-0.2.2/tests/utils/test_byte_format.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/utils/test_configurable.py` & `tickit-0.2.2/tests/utils/test_configurable.py`

 * *Files identical despite different names*

### Comparing `tickit-0.2.1/tests/utils/test_singleton.py` & `tickit-0.2.2/tests/utils/test_singleton.py`

 * *Files identical despite different names*

