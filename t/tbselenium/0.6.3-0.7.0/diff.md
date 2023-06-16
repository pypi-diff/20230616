# Comparing `tmp/tbselenium-0.6.3.tar.gz` & `tmp/tbselenium-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tbselenium-0.6.3.tar", last modified: Tue Sep 20 20:30:39 2022, max compression
+gzip compressed data, was "tbselenium-0.7.0.tar", last modified: Fri Jun 16 20:08:03 2023, max compression
```

## Comparing `tbselenium-0.6.3.tar` & `tbselenium-0.7.0.tar`

### file list

```diff
@@ -1,38 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-20 20:30:39.541347 tbselenium-0.6.3/
--rw-r--r--   0 root         (0) root         (0)     8450 2022-09-20 20:30:39.541347 tbselenium-0.6.3/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     7022 2022-09-20 06:40:34.000000 tbselenium-0.6.3/README.md
--rw-rw-r--   0 root         (0) root         (0)       79 2022-09-20 20:30:39.541347 tbselenium-0.6.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      521 2022-09-20 20:28:22.000000 tbselenium-0.6.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-20 20:30:39.537347 tbselenium-0.6.3/tbselenium/
--rw-rw-r--   0 root         (0) root         (0)        0 2017-10-04 01:40:34.000000 tbselenium-0.6.3/tbselenium/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2071 2021-11-24 22:01:11.000000 tbselenium-0.6.3/tbselenium/common.py
--rw-rw-r--   0 root         (0) root         (0)      336 2017-10-04 01:40:34.000000 tbselenium-0.6.3/tbselenium/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)      957 2021-11-23 21:31:02.000000 tbselenium-0.6.3/tbselenium/set_profile.py
--rw-rw-r--   0 root         (0) root         (0)      305 2021-11-23 20:03:26.000000 tbselenium-0.6.3/tbselenium/set_profile_nops.py
--rw-rw-r--   0 root         (0) root         (0)      423 2017-10-20 03:12:07.000000 tbselenium-0.6.3/tbselenium/tbbinary.py
--rw-rw-r--   0 root         (0) root         (0)    15213 2022-09-20 20:20:22.000000 tbselenium-0.6.3/tbselenium/tbdriver.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-20 20:30:39.541347 tbselenium-0.6.3/tbselenium/test/
--rw-rw-r--   0 root         (0) root         (0)      428 2021-11-21 18:33:07.000000 tbselenium-0.6.3/tbselenium/test/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1375 2021-11-24 22:01:11.000000 tbselenium-0.6.3/tbselenium/test/conftest.py
--rw-rw-r--   0 root         (0) root         (0)     4509 2021-12-13 22:11:25.000000 tbselenium-0.6.3/tbselenium/test/fixtures.py
--rw-rw-r--   0 root         (0) root         (0)     2193 2022-08-03 11:55:54.000000 tbselenium-0.6.3/tbselenium/test/test_addons.py
--rw-rw-r--   0 root         (0) root         (0)     1548 2021-11-24 22:01:11.000000 tbselenium-0.6.3/tbselenium/test/test_bridge.py
--rw-rw-r--   0 root         (0) root         (0)     2557 2021-11-24 22:01:11.000000 tbselenium-0.6.3/tbselenium/test/test_browser.py
--rw-rw-r--   0 root         (0) root         (0)     1686 2021-11-24 22:01:11.000000 tbselenium-0.6.3/tbselenium/test/test_context_switch.py
--rw-rw-r--   0 root         (0) root         (0)      862 2019-01-28 03:06:32.000000 tbselenium-0.6.3/tbselenium/test/test_disable_javascript.py
--rw-rw-r--   0 root         (0) root         (0)      807 2021-11-24 22:01:11.000000 tbselenium-0.6.3/tbselenium/test/test_env.py
--rw-rw-r--   0 root         (0) root         (0)     4160 2021-11-24 22:01:11.000000 tbselenium-0.6.3/tbselenium/test/test_exceptions.py
--rw-rw-r--   0 root         (0) root         (0)     1369 2017-10-19 13:40:30.000000 tbselenium-0.6.3/tbselenium/test/test_screenshot.py
--rw-rw-r--   0 root         (0) root         (0)     5402 2021-11-24 22:01:11.000000 tbselenium-0.6.3/tbselenium/test/test_set_security_level.py
--rw-rw-r--   0 root         (0) root         (0)     2078 2021-11-24 22:01:11.000000 tbselenium-0.6.3/tbselenium/test/test_stem.py
--rw-rw-r--   0 root         (0) root         (0)     5488 2022-09-20 20:20:22.000000 tbselenium-0.6.3/tbselenium/test/test_tbdriver.py
--rw-rw-r--   0 root         (0) root         (0)      619 2019-01-24 04:43:00.000000 tbselenium-0.6.3/tbselenium/test/test_tor.py
--rw-rw-r--   0 root         (0) root         (0)      889 2017-10-20 05:26:59.000000 tbselenium-0.6.3/tbselenium/test/test_utils.py
--rw-rw-r--   0 root         (0) root         (0)     1521 2021-11-21 11:47:40.000000 tbselenium-0.6.3/tbselenium/unpack_tb.py
--rw-rw-r--   0 root         (0) root         (0)     3546 2021-12-27 14:34:35.000000 tbselenium-0.6.3/tbselenium/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-20 20:30:39.537347 tbselenium-0.6.3/tbselenium.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     8450 2022-09-20 20:30:39.000000 tbselenium-0.6.3/tbselenium.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      934 2022-09-20 20:30:39.000000 tbselenium-0.6.3/tbselenium.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2022-09-20 20:30:39.000000 tbselenium-0.6.3/tbselenium.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       12 2022-09-20 20:30:39.000000 tbselenium-0.6.3/tbselenium.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       11 2022-09-20 20:30:39.000000 tbselenium-0.6.3/tbselenium.egg-info/top_level.txt
+drwxrwxr-x   0 gacar     (1000) gacar     (1000)        0 2023-06-16 20:08:03.877579 tbselenium-0.7.0/
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)     1121 2023-05-13 20:09:27.000000 tbselenium-0.7.0/LICENSE
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)     7227 2023-06-16 20:08:03.877579 tbselenium-0.7.0/PKG-INFO
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)     6953 2023-06-11 23:26:11.000000 tbselenium-0.7.0/README.md
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)       79 2023-06-16 20:08:03.877579 tbselenium-0.7.0/setup.cfg
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)      521 2023-06-16 20:00:22.000000 tbselenium-0.7.0/setup.py
+drwxrwxr-x   0 gacar     (1000) gacar     (1000)        0 2023-06-16 20:08:03.873579 tbselenium-0.7.0/tbselenium/
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)        0 2023-05-13 20:09:27.000000 tbselenium-0.7.0/tbselenium/__init__.py
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)     2332 2023-06-11 16:36:29.000000 tbselenium-0.7.0/tbselenium/common.py
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)      336 2023-05-13 20:09:27.000000 tbselenium-0.7.0/tbselenium/exceptions.py
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)      423 2023-05-13 20:09:27.000000 tbselenium-0.7.0/tbselenium/tbbinary.py
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)    15746 2023-06-10 14:06:55.000000 tbselenium-0.7.0/tbselenium/tbdriver.py
+drwxrwxr-x   0 gacar     (1000) gacar     (1000)        0 2023-06-16 20:08:03.877579 tbselenium-0.7.0/tbselenium/test/
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)      428 2023-05-13 20:09:27.000000 tbselenium-0.7.0/tbselenium/test/__init__.py
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)     1375 2023-05-13 20:09:27.000000 tbselenium-0.7.0/tbselenium/test/conftest.py
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)     4539 2023-06-10 14:47:35.000000 tbselenium-0.7.0/tbselenium/test/fixtures.py
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)     2174 2023-06-10 12:46:21.000000 tbselenium-0.7.0/tbselenium/test/test_addons.py
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)     1548 2023-05-13 20:09:27.000000 tbselenium-0.7.0/tbselenium/test/test_bridge.py
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)     3326 2023-06-10 13:30:55.000000 tbselenium-0.7.0/tbselenium/test/test_browser.py
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)     1686 2023-05-13 20:09:27.000000 tbselenium-0.7.0/tbselenium/test/test_context_switch.py
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)     1588 2023-06-11 16:47:58.000000 tbselenium-0.7.0/tbselenium/test/test_disable_features.py
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)     1028 2023-06-10 12:55:22.000000 tbselenium-0.7.0/tbselenium/test/test_env.py
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)     4160 2023-05-13 20:09:27.000000 tbselenium-0.7.0/tbselenium/test/test_exceptions.py
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)     1369 2023-05-13 20:09:27.000000 tbselenium-0.7.0/tbselenium/test/test_screenshot.py
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)     4365 2023-06-11 15:58:04.000000 tbselenium-0.7.0/tbselenium/test/test_set_security_level.py
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)     2078 2023-05-13 20:09:27.000000 tbselenium-0.7.0/tbselenium/test/test_stem.py
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)     5565 2023-06-11 17:38:00.000000 tbselenium-0.7.0/tbselenium/test/test_tbdriver.py
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)      619 2023-05-13 20:09:27.000000 tbselenium-0.7.0/tbselenium/test/test_tor.py
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)      889 2023-05-13 20:09:27.000000 tbselenium-0.7.0/tbselenium/test/test_utils.py
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)     6654 2023-06-11 16:50:56.000000 tbselenium-0.7.0/tbselenium/utils.py
+drwxrwxr-x   0 gacar     (1000) gacar     (1000)        0 2023-06-16 20:08:03.873579 tbselenium-0.7.0/tbselenium.egg-info/
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)     7227 2023-06-16 20:08:03.000000 tbselenium-0.7.0/tbselenium.egg-info/PKG-INFO
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)      859 2023-06-16 20:08:03.000000 tbselenium-0.7.0/tbselenium.egg-info/SOURCES.txt
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)        1 2023-06-16 20:08:03.000000 tbselenium-0.7.0/tbselenium.egg-info/dependency_links.txt
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)       12 2023-06-16 20:08:03.000000 tbselenium-0.7.0/tbselenium.egg-info/requires.txt
+-rw-rw-r--   0 gacar     (1000) gacar     (1000)       11 2023-06-16 20:08:03.000000 tbselenium-0.7.0/tbselenium.egg-info/top_level.txt
```

### Comparing `tbselenium-0.6.3/PKG-INFO` & `tbselenium-0.7.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,152 +1,143 @@
-Metadata-Version: 2.1
-Name: tbselenium
-Version: 0.6.3
-Summary: Tor Browser automation with Selenium
-Home-page: https://github.com/webfp/tor-browser-selenium
-Author: Gunes Acar
-License: UNKNOWN
-Description: # tor-browser-selenium [![Build Status](https://app.travis-ci.com/webfp/tor-browser-selenium.svg?branch=main)](https://app.travis-ci.com/webfp/tor-browser-selenium)
-        
-        
-        A Python library to automate Tor Browser with Selenium.
-        
-        ## Installation
-        
-        ```
-        pip install tbselenium
-        ```
-        
-        Install `geckodriver` from the [geckodriver releases page](https://github.com/mozilla/geckodriver/releases/). Make sure you install version v0.23.0 version or newer; older versions may not be compatible with the current Tor Browser series.
-        
-        
-        ## Basic usage
-        ### Using with system `tor`
-        
-        `tor` needs to be installed (`apt install tor`) and running on port 9050.
-        
-        ```python
-        from tbselenium.tbdriver import TorBrowserDriver
-        with TorBrowserDriver("/path/to/TorBrowserBundle/") as driver:
-            driver.get('https://check.torproject.org')
-        ```
-        
-        ### Using with `Stem`
-        First, make sure you have `Stem` installed (`pip install stem`).
-        The following will start a new `tor` process using `Stem`. It will not use the `tor` installed on your system.
-        
-        ```python
-        import tbselenium.common as cm
-        from tbselenium.tbdriver import TorBrowserDriver
-        from tbselenium.utils import launch_tbb_tor_with_stem
-        
-        tbb_dir = "/path/to/TorBrowserBundle/"
-        tor_process = launch_tbb_tor_with_stem(tbb_path=tbb_dir)
-        with TorBrowserDriver(tbb_dir, tor_cfg=cm.USE_STEM) as driver:
-            driver.load_url("https://check.torproject.org")
-        
-        tor_process.kill()
-        ```
-        
-        TorBrowserDriver does not download Tor Browser Bundle (TBB) for you. You should [download](https://www.torproject.org/projects/torbrowser.html.en), extract TBB and provide its path when you initialize `TorBrowserDriver`.
-        
-        ### Setting `geckodriver`'s location without using PATH
-        If `geckodriver` is not on the system PATH, the binary location can be set programmatically:
-        
-        ```python
-        TorBrowserDriver(executable_path="/path/to/geckodriver")
-        ```
-        
-        ## Test and development
-        Install the Python packages that are needed for development and testing:
-        
-        `pip install -r requirements-dev.txt`
-        
-        Install `xvfb` package by running `apt-get install xvfb` or using your distro's package manager.
-        
-        Run the following to launch the tests:
-        
-        `./run_tests.py /path/to/TorBrowserBundle/`
-        
-        By default, tests will be run using `Xvfb`, so the browser will not be visible.
-        You may disable `Xvfb` by exporting the following environment variable:
-        
-        `export NO_XVFB=1`
-        
-        
-        
-        ### Running individual tests
-        First, export a `TBB_PATH` environment variable that points to the TBB version you want to use:
-        
-        `export TBB_PATH=/path/to/tbb/tor-browser_en-US/`
-        
-        Then, use `py.test` to launch the tests you want, e.g.:
-        
-        * `py.test tbselenium/test/test_tbdriver.py`
-        * `py.test tbselenium/test/test_tbdriver.py::TBDriverTest::test_should_load_check_tpo`
-        
-        ### Disabling console logs
-        You can redirect the logs to `/dev/null` by passing the `tbb_logfile_path` initialization parameter:
-        ```python
-        TorBrowserDriver(..., tbb_logfile_path='/dev/null')
-        ```
-        
-        ## Examples
-        Check the [examples](https://github.com/webfp/tor-browser-selenium/tree/master/examples) to discover different ways to use TorBrowserDriver
-        * [check_tpo.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/check_tpo.py): Visit check.torproject.org website and print the network status message
-        * [headless.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/headless.py): Headless visit and screenshot of check.torproject.org using XVFB
-        * [hidden_service.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/hidden_service.py): Search using DuckDuckGo's hidden service
-        * [parallel.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/parallel.py): Visit check.torproject.org with 3 browsers running in parallel
-        * [screenshot.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/screenshot.py): Take a screenshot
-        * [stem_simple.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/stem_simple.py): Using Stem to start the Tor process
-        * [stem_adv.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/stem_adv.py): Using Stem with more advanced configuration
-        
-        
-        ## Compatibility
-        [Tested](https://travis-ci.org/webfp/tor-browser-selenium) with the following Tor Browser Bundle versions on Ubuntu:
-        
-        * 11.5.2
-        * 12.0a2
-        
-        Warning: **Windows and macOS are not supported.**
-        
-        ## Troubleshooting
-        
-        Solutions to potential issues:
-        
-        * Make sure you can run Firefox on the same system. This may help discover issues such as missing libraries, displays etc..
-        * Outdated (or incompatible) Python `selenium` package: This is the source of various obscure errors. Make sure you have an up-to-date `selenium` package installed.
-        * No display: When running on a cloud machine, follow the [headless.py example](https://github.com/webfp/tor-browser-selenium/blob/master/examples/headless.py#L10) to start a virtual display.
-        * Outdated Tor Browser Bundle: Download and use a more recent TBB version.
-        * Make sure you install the latest `geckodriver` version.
-        * Port conflict with other (`Tor`) process: Pick a different SOCKS and controller port using `socks_port` argument.
-        * Use `tbb_logfile_path` argument of TorBrowserDriver to debug obscure errors. This can help with problems due to missing display, missing libraries (e.g. when the LD_LIBRARY_PATH is not set correctly) or other errors that Tor Browser logs to standard output/error.
-        * When you use `LAUNCH_NEW_TBB_TOR` option and get the following [error message](https://github.com/webfp/tor-browser-selenium/issues/62) during the initialization, it's likely that Tor failed to bootstrap (due to network etc.):
-        
-         ```
-         Can't load the profile. Profile Dir: /tmp/tmpO7i1lL/webdriver-py-profilecopy If you specified a log_file in the FirefoxBinary constructor, check it for details
-         ```
-        * `driver.get_cookies()` returns an empty list. This is due to Private Browsing Mode (PBM), which Selenium uses under the hood. See [#79](https://github.com/webfp/tor-browser-selenium/issues/79) for a possible solution.
-        * WebGL is not supported in the headless mode started with `headless=True` due to Firefox bug [#1375585](https://bugzilla.mozilla.org/show_bug.cgi?id=1375585). To enable WebGL in a headless setting, use `pyvirtualdisplay` following the [headless.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/headless.py) example.
-        
-        ## Reference
-        Please consider citing this repository if you use `tor-browser-selenium` in your academic publications.
-        
-        ```
-        @misc{tor-browser-selenium,
-          author = {Gunes Acar and Marc Juarez and individual contributors},
-          title = {tor-browser-selenium - Tor Browser automation with Selenium},
-          year = {2020},
-          publisher = {GitHub},
-          journal = {GitHub repository},
-          howpublished = {\url{https://github.com/webfp/tor-browser-selenium}}
-        }
-        ```
-        
-        ## Credits
-        We greatly benefited from the following two projects:
-        * [tor-browser-selenium](https://github.com/isislovecruft/tor-browser-selenium) by @isislovecruft.
-        * [tor-browser-bundle-testsuite](https://gitweb.torproject.org/boklm/tor-browser-bundle-testsuite.git/) by @boklm.
-        
-Keywords: tor,selenium,tor browser
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# tor-browser-selenium [![Build Status](https://app.travis-ci.com/webfp/tor-browser-selenium.svg?branch=main)](https://app.travis-ci.com/webfp/tor-browser-selenium)
+
+
+A Python library to automate Tor Browser with Selenium WebDriver.
+
+## 📦 Installation
+
+```
+pip install tbselenium
+```
+
+Download `geckodriver` v0.31.0 from the [geckodriver releases page](https://github.com/mozilla/geckodriver/releases/) and add it to PATH.
+
+## 🚀 Usage
+
+Download and extract [Tor Browser](https://www.torproject.org/projects/torbrowser.html.en), and pass its path when you initialize `TorBrowserDriver`.
+
+
+### Using with system `tor`
+
+`tor` needs to be installed (`apt install tor`) and running on port 9050.
+
+```python
+from tbselenium.tbdriver import TorBrowserDriver
+with TorBrowserDriver("/path/to/tor-browser/") as driver:
+    driver.get('https://check.torproject.org')
+```
+
+### Using with `Stem`
+You can use `Stem` to start a new tor process programmatically, and connect to it from `tor-browser-selenium`. Make sure you have `Stem` installed: `pip install stem`:
+
+
+```python
+import tbselenium.common as cm
+from tbselenium.tbdriver import TorBrowserDriver
+from tbselenium.utils import launch_tbb_tor_with_stem
+
+tbb_dir = "/path/to/tor-browser/"
+tor_process = launch_tbb_tor_with_stem(tbb_path=tbb_dir)
+with TorBrowserDriver(tbb_dir, tor_cfg=cm.USE_STEM) as driver:
+    driver.load_url("https://check.torproject.org")
+
+tor_process.kill()
+```
+
+
+## 💡 Examples
+Check the [examples](https://github.com/webfp/tor-browser-selenium/tree/master/examples) to discover different ways to use `tor-browser-selenium`
+* [check_tpo.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/check_tpo.py): Visit the `check.torproject.org` website and print the network status message
+* [headless.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/headless.py): Headless visit and screenshot of check.torproject.org using [PyVirtualDisplay](https://pypi.org/project/PyVirtualDisplay/)
+* [onion_service.py](https://github.com/webfp/tor-browser-selenium/blob/main/examples/onion_service.py): Search using DuckDuckGo's Onion service
+* [parallel.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/parallel.py): Visit `check.torproject.org`` with 3 browsers running in parallel
+* [screenshot.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/screenshot.py): Take a screenshot
+* [stem_simple.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/stem_simple.py): Use Stem to start a `tor` process
+* [stem_adv.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/stem_adv.py): Use Stem to launch `tor` with more advanced configuration
+
+
+
+## 🛠️ Test and development
+
+* Browse the [existing tests](https://github.com/webfp/tor-browser-selenium/tree/main/tbselenium/test) to find out about different ways you can use `tor-browser-selenium`.
+
+* For development and testing first install the necessary Python packages:
+  `pip install -r requirements-dev.txt`
+
+* Install the `xvfb` package by running `apt-get install xvfb` or using your distro's package manager.
+
+* Run the following to launch the tests:
+
+  `./run_tests.py /path/to/tor-browser/`
+
+* By default, tests will be run using `Xvfb`, so the browser window will not be visible.
+You may disable `Xvfb` by setting the `NO_XVFB` environment variable:
+
+  `export NO_XVFB=1`
+
+
+### Running individual tests
+* First, export the path to Tor Browser folder in the `TBB_PATH` environment variable.
+
+`export TBB_PATH=/path/to/tbb/tor-browser/`
+
+* Then, use `py.test` to launch the tests you want, e.g.:
+
+* `py.test tbselenium/test/test_tbdriver.py`
+* `py.test tbselenium/test/test_tbdriver.py::TBDriverTest::test_should_load_check_tpo`
+
+
+### Using a custom `geckodriver`
+A custom `geckodriver` binary can be set via the `executable_path` argument:
+
+```python
+TorBrowserDriver(executable_path="/path/to/geckodriver")
+```
+
+### Disabling console logs
+You can redirect the logs to `/dev/null` by passing the `tbb_logfile_path` initialization parameter:
+```python
+TorBrowserDriver(..., tbb_logfile_path='/dev/null')
+```
+
+## ⚙️ Compatibility
+
+Warning: **Windows and macOS are not supported.**
+
+[Tested](https://travis-ci.org/webfp/tor-browser-selenium) with the following Tor Browser versions on Ubuntu:
+
+* **Stable**: 12.0.7
+* **Alpha**: 12.5a7
+
+If you need to use a different version of Tor Browser, [view the past test runs](https://travis-ci.org/webfp/tor-browser-selenium) to find out the compatible `selenium` and `geckodriver` versions.
+
+## 🔧 Troubleshooting
+
+Solutions to potential issues:
+
+* Make sure you have compatible dependencies. While older or newer versions may work, they may cause issues.
+  - [Tor Browser](https://www.torproject.org/download/) needs to be downloaded and extracted.
+  - Python [`selenium`](https://www.selenium.dev/) (`pip install -U selenium`).
+  - `geckodriver` [version 0.31.0](https://github.com/mozilla/geckodriver/releases/tag/v0.31.0).
+
+* Running Firefox on the same system may help diagnose issues such as missing libraries and displays.
+* `Process unexpectedly closed with status 1`: If you encounter this on a remote machine you connect via SSH, you may need to enable the [headless mode](https://github.com/webfp/tor-browser-selenium/blob/master/examples/headless.py).
+* Port conflict with other (`Tor`) process: Pick a different SOCKS and controller port using the `socks_port` argument.
+* Use `tbb_logfile_path` argument of TorBrowserDriver to debug obscure errors. This can help with problems due to missing display, missing libraries (e.g. when the LD_LIBRARY_PATH is not set correctly) or other errors that Tor Browser logs to standard output/error.
+* `driver.get_cookies()` returns an empty list. This is due to Private Browsing Mode (PBM), which Selenium uses under the hood. See [#79](https://github.com/webfp/tor-browser-selenium/issues/79) for a possible solution.
+* WebGL is not supported in the headless mode started with `headless=True` due to a Firefox bug ([#1375585](https://bugzilla.mozilla.org/show_bug.cgi?id=1375585)). To enable WebGL in a headless setting, use `pyvirtualdisplay` following the [headless.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/headless.py) example.
+
+## 📚 Reference
+Please use the following reference if you use `tor-browser-selenium` in your academic publications.
+
+```
+@misc{tor-browser-selenium,
+  author = {Gunes Acar and Marc Juarez and individual contributors},
+  title = {tor-browser-selenium - Tor Browser automation with Selenium},
+  year = {2023},
+  publisher = {GitHub},
+  howpublished = {\url{https://github.com/webfp/tor-browser-selenium}}
+}
+```
+
+## 🙌 Credits
+We greatly benefited from the [tor-browser-bundle-testsuite](https://gitlab.torproject.org/tpo/applications/tor-browser-bundle-testsuite) and [tor-browser-selenium](https://github.com/isislovecruft/tor-browser-selenium) projects.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tbselenium-0.6.3/README.md` & `tbselenium-0.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,141 +1,153 @@
+Metadata-Version: 2.1
+Name: tbselenium
+Version: 0.7.0
+Summary: Tor Browser automation with Selenium
+Home-page: https://github.com/webfp/tor-browser-selenium
+Author: Gunes Acar
+Keywords: tor,selenium,tor browser
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # tor-browser-selenium [![Build Status](https://app.travis-ci.com/webfp/tor-browser-selenium.svg?branch=main)](https://app.travis-ci.com/webfp/tor-browser-selenium)
 
 
-A Python library to automate Tor Browser with Selenium.
+A Python library to automate Tor Browser with Selenium WebDriver.
 
-## Installation
+## 📦 Installation
 
 ```
 pip install tbselenium
 ```
 
-Install `geckodriver` from the [geckodriver releases page](https://github.com/mozilla/geckodriver/releases/). Make sure you install version v0.23.0 version or newer; older versions may not be compatible with the current Tor Browser series.
+Download `geckodriver` v0.31.0 from the [geckodriver releases page](https://github.com/mozilla/geckodriver/releases/) and add it to PATH.
+
+## 🚀 Usage
+
+Download and extract [Tor Browser](https://www.torproject.org/projects/torbrowser.html.en), and pass its path when you initialize `TorBrowserDriver`.
 
 
-## Basic usage
 ### Using with system `tor`
 
 `tor` needs to be installed (`apt install tor`) and running on port 9050.
 
 ```python
 from tbselenium.tbdriver import TorBrowserDriver
-with TorBrowserDriver("/path/to/TorBrowserBundle/") as driver:
+with TorBrowserDriver("/path/to/tor-browser/") as driver:
     driver.get('https://check.torproject.org')
 ```
 
 ### Using with `Stem`
-First, make sure you have `Stem` installed (`pip install stem`).
-The following will start a new `tor` process using `Stem`. It will not use the `tor` installed on your system.
+You can use `Stem` to start a new tor process programmatically, and connect to it from `tor-browser-selenium`. Make sure you have `Stem` installed: `pip install stem`:
+
 
 ```python
 import tbselenium.common as cm
 from tbselenium.tbdriver import TorBrowserDriver
 from tbselenium.utils import launch_tbb_tor_with_stem
 
-tbb_dir = "/path/to/TorBrowserBundle/"
+tbb_dir = "/path/to/tor-browser/"
 tor_process = launch_tbb_tor_with_stem(tbb_path=tbb_dir)
 with TorBrowserDriver(tbb_dir, tor_cfg=cm.USE_STEM) as driver:
     driver.load_url("https://check.torproject.org")
 
 tor_process.kill()
 ```
 
-TorBrowserDriver does not download Tor Browser Bundle (TBB) for you. You should [download](https://www.torproject.org/projects/torbrowser.html.en), extract TBB and provide its path when you initialize `TorBrowserDriver`.
 
-### Setting `geckodriver`'s location without using PATH
-If `geckodriver` is not on the system PATH, the binary location can be set programmatically:
+## 💡 Examples
+Check the [examples](https://github.com/webfp/tor-browser-selenium/tree/master/examples) to discover different ways to use `tor-browser-selenium`
+* [check_tpo.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/check_tpo.py): Visit the `check.torproject.org` website and print the network status message
+* [headless.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/headless.py): Headless visit and screenshot of check.torproject.org using [PyVirtualDisplay](https://pypi.org/project/PyVirtualDisplay/)
+* [onion_service.py](https://github.com/webfp/tor-browser-selenium/blob/main/examples/onion_service.py): Search using DuckDuckGo's Onion service
+* [parallel.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/parallel.py): Visit `check.torproject.org`` with 3 browsers running in parallel
+* [screenshot.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/screenshot.py): Take a screenshot
+* [stem_simple.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/stem_simple.py): Use Stem to start a `tor` process
+* [stem_adv.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/stem_adv.py): Use Stem to launch `tor` with more advanced configuration
+
 
-```python
-TorBrowserDriver(executable_path="/path/to/geckodriver")
-```
 
-## Test and development
-Install the Python packages that are needed for development and testing:
+## 🛠️ Test and development
 
-`pip install -r requirements-dev.txt`
+* Browse the [existing tests](https://github.com/webfp/tor-browser-selenium/tree/main/tbselenium/test) to find out about different ways you can use `tor-browser-selenium`.
 
-Install `xvfb` package by running `apt-get install xvfb` or using your distro's package manager.
+* For development and testing first install the necessary Python packages:
+  `pip install -r requirements-dev.txt`
 
-Run the following to launch the tests:
+* Install the `xvfb` package by running `apt-get install xvfb` or using your distro's package manager.
 
-`./run_tests.py /path/to/TorBrowserBundle/`
+* Run the following to launch the tests:
 
-By default, tests will be run using `Xvfb`, so the browser will not be visible.
-You may disable `Xvfb` by exporting the following environment variable:
+  `./run_tests.py /path/to/tor-browser/`
 
-`export NO_XVFB=1`
+* By default, tests will be run using `Xvfb`, so the browser window will not be visible.
+You may disable `Xvfb` by setting the `NO_XVFB` environment variable:
 
+  `export NO_XVFB=1`
 
 
 ### Running individual tests
-First, export a `TBB_PATH` environment variable that points to the TBB version you want to use:
+* First, export the path to Tor Browser folder in the `TBB_PATH` environment variable.
 
-`export TBB_PATH=/path/to/tbb/tor-browser_en-US/`
+`export TBB_PATH=/path/to/tbb/tor-browser/`
 
-Then, use `py.test` to launch the tests you want, e.g.:
+* Then, use `py.test` to launch the tests you want, e.g.:
 
 * `py.test tbselenium/test/test_tbdriver.py`
 * `py.test tbselenium/test/test_tbdriver.py::TBDriverTest::test_should_load_check_tpo`
 
+
+### Using a custom `geckodriver`
+A custom `geckodriver` binary can be set via the `executable_path` argument:
+
+```python
+TorBrowserDriver(executable_path="/path/to/geckodriver")
+```
+
 ### Disabling console logs
 You can redirect the logs to `/dev/null` by passing the `tbb_logfile_path` initialization parameter:
 ```python
 TorBrowserDriver(..., tbb_logfile_path='/dev/null')
 ```
 
-## Examples
-Check the [examples](https://github.com/webfp/tor-browser-selenium/tree/master/examples) to discover different ways to use TorBrowserDriver
-* [check_tpo.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/check_tpo.py): Visit check.torproject.org website and print the network status message
-* [headless.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/headless.py): Headless visit and screenshot of check.torproject.org using XVFB
-* [hidden_service.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/hidden_service.py): Search using DuckDuckGo's hidden service
-* [parallel.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/parallel.py): Visit check.torproject.org with 3 browsers running in parallel
-* [screenshot.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/screenshot.py): Take a screenshot
-* [stem_simple.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/stem_simple.py): Using Stem to start the Tor process
-* [stem_adv.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/stem_adv.py): Using Stem with more advanced configuration
+## ⚙️ Compatibility
 
+Warning: **Windows and macOS are not supported.**
 
-## Compatibility
-[Tested](https://travis-ci.org/webfp/tor-browser-selenium) with the following Tor Browser Bundle versions on Ubuntu:
+[Tested](https://travis-ci.org/webfp/tor-browser-selenium) with the following Tor Browser versions on Ubuntu:
 
-* 11.5.2
-* 12.0a2
+* **Stable**: 12.0.7
+* **Alpha**: 12.5a7
 
-Warning: **Windows and macOS are not supported.**
+If you need to use a different version of Tor Browser, [view the past test runs](https://travis-ci.org/webfp/tor-browser-selenium) to find out the compatible `selenium` and `geckodriver` versions.
 
-## Troubleshooting
+## 🔧 Troubleshooting
 
 Solutions to potential issues:
 
-* Make sure you can run Firefox on the same system. This may help discover issues such as missing libraries, displays etc..
-* Outdated (or incompatible) Python `selenium` package: This is the source of various obscure errors. Make sure you have an up-to-date `selenium` package installed.
-* No display: When running on a cloud machine, follow the [headless.py example](https://github.com/webfp/tor-browser-selenium/blob/master/examples/headless.py#L10) to start a virtual display.
-* Outdated Tor Browser Bundle: Download and use a more recent TBB version.
-* Make sure you install the latest `geckodriver` version.
-* Port conflict with other (`Tor`) process: Pick a different SOCKS and controller port using `socks_port` argument.
+* Make sure you have compatible dependencies. While older or newer versions may work, they may cause issues.
+  - [Tor Browser](https://www.torproject.org/download/) needs to be downloaded and extracted.
+  - Python [`selenium`](https://www.selenium.dev/) (`pip install -U selenium`).
+  - `geckodriver` [version 0.31.0](https://github.com/mozilla/geckodriver/releases/tag/v0.31.0).
+
+* Running Firefox on the same system may help diagnose issues such as missing libraries and displays.
+* `Process unexpectedly closed with status 1`: If you encounter this on a remote machine you connect via SSH, you may need to enable the [headless mode](https://github.com/webfp/tor-browser-selenium/blob/master/examples/headless.py).
+* Port conflict with other (`Tor`) process: Pick a different SOCKS and controller port using the `socks_port` argument.
 * Use `tbb_logfile_path` argument of TorBrowserDriver to debug obscure errors. This can help with problems due to missing display, missing libraries (e.g. when the LD_LIBRARY_PATH is not set correctly) or other errors that Tor Browser logs to standard output/error.
-* When you use `LAUNCH_NEW_TBB_TOR` option and get the following [error message](https://github.com/webfp/tor-browser-selenium/issues/62) during the initialization, it's likely that Tor failed to bootstrap (due to network etc.):
-
- ```
- Can't load the profile. Profile Dir: /tmp/tmpO7i1lL/webdriver-py-profilecopy If you specified a log_file in the FirefoxBinary constructor, check it for details
- ```
 * `driver.get_cookies()` returns an empty list. This is due to Private Browsing Mode (PBM), which Selenium uses under the hood. See [#79](https://github.com/webfp/tor-browser-selenium/issues/79) for a possible solution.
-* WebGL is not supported in the headless mode started with `headless=True` due to Firefox bug [#1375585](https://bugzilla.mozilla.org/show_bug.cgi?id=1375585). To enable WebGL in a headless setting, use `pyvirtualdisplay` following the [headless.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/headless.py) example.
+* WebGL is not supported in the headless mode started with `headless=True` due to a Firefox bug ([#1375585](https://bugzilla.mozilla.org/show_bug.cgi?id=1375585)). To enable WebGL in a headless setting, use `pyvirtualdisplay` following the [headless.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/headless.py) example.
 
-## Reference
-Please consider citing this repository if you use `tor-browser-selenium` in your academic publications.
+## 📚 Reference
+Please use the following reference if you use `tor-browser-selenium` in your academic publications.
 
 ```
 @misc{tor-browser-selenium,
   author = {Gunes Acar and Marc Juarez and individual contributors},
   title = {tor-browser-selenium - Tor Browser automation with Selenium},
-  year = {2020},
+  year = {2023},
   publisher = {GitHub},
-  journal = {GitHub repository},
   howpublished = {\url{https://github.com/webfp/tor-browser-selenium}}
 }
 ```
 
-## Credits
-We greatly benefited from the following two projects:
-* [tor-browser-selenium](https://github.com/isislovecruft/tor-browser-selenium) by @isislovecruft.
-* [tor-browser-bundle-testsuite](https://gitweb.torproject.org/boklm/tor-browser-bundle-testsuite.git/) by @boklm.
+## 🙌 Credits
+We greatly benefited from the [tor-browser-bundle-testsuite](https://gitlab.torproject.org/tpo/applications/tor-browser-bundle-testsuite) and [tor-browser-selenium](https://github.com/isislovecruft/tor-browser-selenium) projects.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tbselenium-0.6.3/setup.py` & `tbselenium-0.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 setup(
     author='Gunes Acar',
     name="tbselenium",
     description="Tor Browser automation with Selenium",
     keywords=["tor", "selenium", "tor browser"],
-    version="0.6.3",
+    version="0.7.0",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/webfp/tor-browser-selenium',
     packages=["tbselenium", "tbselenium.test"],
     install_requires=[
         "selenium>=4"
     ]
```

### Comparing `tbselenium-0.6.3/tbselenium/tbdriver.py` & `tbselenium-0.7.0/tbselenium/tbdriver.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,35 +73,39 @@
 
         self.init_ports(tor_cfg, socks_port, control_port)
         self.init_prefs(pref_dict, default_bridge_type)
         self.export_env_vars()
         # TODO:
         # self.binary = self.get_tb_binary(logfile=tbb_logfile_path)
         if use_custom_profile:
+            print(f'Using custom profile: {self.tbb_profile_path}')
             tbb_service = Service(
                 executable_path=executable_path,
-                log_path=tbb_logfile_path,
+                log_path=tbb_logfile_path,  # TODO: deprecated, use log_output
                 service_args=["--marionette-port", "2828"],
                 port=geckodriver_port
                 )
         else:
             tbb_service = Service(
                 executable_path=executable_path,
                 log_path=tbb_logfile_path,
                 port=geckodriver_port
                 )
+        # options.binary is path to the Firefox binary and it can be a string
+        # or a FirefoxBinary object. If it's a string, it will be converted to
+        # a FirefoxBinary object.
+        # https://github.com/SeleniumHQ/selenium/blob/7cfd137085fcde932cd71af78642a15fd56fe1f1/py/selenium/webdriver/firefox/options.py#L54
         self.options.binary = self.tbb_fx_binary_path
         self.options.add_argument('--class')
         self.options.add_argument('"Tor Browser"')
         if headless:
             self.options.headless = True
 
         super(TorBrowserDriver, self).__init__(
             service=tbb_service,
-            executable_path=executable_path,
             options=self.options,
             )
         self.is_running = True
         self.install_extensions(extensions, install_noscript)
         self.temp_profile_dir = self.capabilities["moz:profile"]
         sleep(1)
 
@@ -274,14 +278,16 @@
         if default_bridge_type:
             # to use a non-default bridge, overwrite the relevant pref, e.g.:
             # extensions.torlauncher.default_bridge.meek-azure.1 = meek 0.0....
             set_pref('extensions.torlauncher.default_bridge_type',
                      default_bridge_type)
 
         set_pref('extensions.torbutton.prompted_language', True)
+        # https://gitlab.torproject.org/tpo/applications/tor-browser/-/issues/41378
+        set_pref('intl.language_notification.shown', True)
         # Configure Firefox to use Tor SOCKS proxy
         set_pref('network.proxy.socks_port', self.socks_port)
         set_pref('extensions.torbutton.socks_port', self.socks_port)
         set_pref('extensions.torlauncher.control_port', self.control_port)
         self.set_tb_prefs_for_using_system_tor(self.control_port)
         # pref_dict overwrites above preferences
         for pref_name, pref_val in pref_dict.items():
```

### Comparing `tbselenium-0.6.3/tbselenium/test/conftest.py` & `tbselenium-0.7.0/tbselenium/test/conftest.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.3/tbselenium/test/fixtures.py` & `tbselenium-0.7.0/tbselenium/test/fixtures.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         try:
             raise last_err
         except Exception:
             raise TorBrowserDriverInitError("Cannot initialize")
 
     def __del__(self):
         # remove the temp log file if we created
-        if FORCE_TB_LOGS_DURING_TESTS and os.path.isfile(self.log_file):
+        if FORCE_TB_LOGS_DURING_TESTS and hasattr(self, "log_file") and os.path.isfile(self.log_file):
             os.remove(self.log_file)
 
     def change_default_tor_cfg(self, kwargs):
         """Use the Tor process that we started with at the beginning of the
         tests if the caller doesn't want to launch a new TBB Tor.
 
         This makes tests faster and more robust against network
```

### Comparing `tbselenium-0.6.3/tbselenium/test/test_addons.py` & `tbselenium-0.7.0/tbselenium/test/test_addons.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,33 +9,30 @@
 from tbselenium import common as cm
 from tbselenium.test import TBB_PATH
 from tbselenium.test.fixtures import TBDriverFixture
 
 
 class TBAddonsTest(unittest.TestCase):
 
-    # Test idea is taken from the TBB test suite
-    # https://gitweb.torproject.org/boklm/tor-browser-bundle-testsuite.git/tree/marionette/tor_browser_tests/test_https-everywhere.py#n18
-    HE_HTTP_URL = "http://httpbin.org/"
-    HE_HTTPS_URL = "https://httpbin.org/"
+    # Based on https://gitlab.torproject.org/tpo/applications/tor-browser-bundle-testsuite/-/blob/2190cfc87657cc64b0b48ec8577617a961d68462/marionette/tor_browser_tests/test_https-everywhere.py#L13
+    HE_HTTP_URL = "http://https-everywhere.badssl.com/redirect-test/status.svg"
+    HE_HTTPS_URL = "https://https-everywhere.badssl.com/redirect-test/status.svg"
     TEST_LONG_WAIT = 60
 
     def get_list_of_installed_addons(self, driver):
         found_addons = []
         driver.load_url_ensure("about:addons")
         addons = driver.find_elements(By.CLASS_NAME, "addon-name")
         for addon in addons:
             found_addons.append(addon.text)
         return found_addons
 
     def test_https_everywhere_redirection(self):
         with TBDriverFixture(TBB_PATH) as driver:
             driver.load_url_ensure(self.HE_HTTP_URL)
-            WebDriverWait(driver, self.TEST_LONG_WAIT).\
-                until(EC.title_contains("httpbin"))
             self.assertEqual(driver.current_url, self.HE_HTTPS_URL)
 
     def test_builtin_addons_should_come_installed(self):
         """Make sure that the built-in addons come installed."""
         EXPECTED_ADDONS = set(['NoScript'])
         found_addons = []
         with TBDriverFixture(TBB_PATH) as driver:
```

### Comparing `tbselenium-0.6.3/tbselenium/test/test_bridge.py` & `tbselenium-0.7.0/tbselenium/test/test_bridge.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.3/tbselenium/test/test_browser.py` & `tbselenium-0.7.0/tbselenium/test/test_browser.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,17 +23,25 @@
     def tearDownClass(cls):
         if cls.driver:
             cls.driver.quit()
         if exists(cls.log_file):
             remove(cls.log_file)
 
     def test_correct_firefox_binary(self):
-        self.assertTrue(self.driver.binary.which('firefox').
-                        startswith(TBB_PATH))
+        """Make sure we use the Firefox binary from the TBB directory."""
+        try:
+            # driver.binary was removed in selenium-4.10.0
+            # https://github.com/SeleniumHQ/selenium/pull/12030/files#diff-89ba579445647535b74423c7bf4b8be79ef1ce33847a2768e623c3083a33545dL127
+            tbbinary = self.driver.options.binary
+        except AttributeError:
+            tbbinary = self.driver.binary
+        self.assertTrue(tbbinary.which('firefox').startswith(TBB_PATH))
 
+    # TODO: log output is always empty
+    @pytest.mark.xfail
     def test_tbb_logfile(self):
         log_txt = read_file(self.log_file)
         self.assertIn("Torbutton INFO", log_txt)
 
     @pytest.mark.skipif(sys.platform != 'linux', reason='Requires Linux')
     def test_should_load_tbb_firefox_libs(self):
         """Make sure we load the Firefox libraries from the TBB directories.
@@ -42,15 +50,21 @@
         The memory map of the TB process is used to find loaded libraries.
         http://man7.org/linux/man-pages/man5/proc.5.html
         """
         FF_BINARY_SUFFIX = '.real'
         driver = self.driver
         geckodriver_pid = driver.service.process.pid
         process = psutil.Process(geckodriver_pid)
-        tbbinary_path = self.driver.binary.which('firefox') + FF_BINARY_SUFFIX
+        try:
+            # driver.binary was removed in selenium-4.10.0
+            # https://github.com/SeleniumHQ/selenium/pull/12030/files#diff-89ba579445647535b74423c7bf4b8be79ef1ce33847a2768e623c3083a33545dL127
+            tbbinary = self.driver.options.binary
+        except AttributeError:
+            tbbinary = self.driver.binary
+        tbbinary_path = tbbinary.which('firefox') + FF_BINARY_SUFFIX
         for child in process.children():
             if tbbinary_path == child.exe():
                 tb_pid = child.pid
                 break
         else:
             self.fail("Cannot find the firefox process")
         xul_lib_path = join(driver.tbb_browser_dir, "libxul.so")
```

### Comparing `tbselenium-0.6.3/tbselenium/test/test_context_switch.py` & `tbselenium-0.7.0/tbselenium/test/test_context_switch.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.3/tbselenium/test/test_env.py` & `tbselenium-0.7.0/tbselenium/test/test_env.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,14 +12,17 @@
     def test_selenium_version(self):
         import selenium
         pkg_ver = selenium.__version__
         self.assertGreaterEqual(LooseVersion(pkg_ver), LooseVersion(MINIMUM_SELENIUM_VERSION))
 
     def test_geckodriver_version(self):
         """Make sure that the right geckodriver version is installed."""
-        GECKODRIVER_VERSION_STR = "geckodriver 0.30.0"
+        # we use 0.31.0 to be able to interact with chrome content (e.g. about: pages)
+        # until the next ESR release (>102)
+        # See, https://github.com/mozilla/geckodriver/issues/2060#issuecomment-1298313743
+        GECKODRIVER_VERSION_STR = "geckodriver 0.31.0"
         gd_v_out = check_output(["geckodriver", "-V"]).decode("utf-8")
         self.assertIn(GECKODRIVER_VERSION_STR, gd_v_out.split("\n")[0])
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `tbselenium-0.6.3/tbselenium/test/test_exceptions.py` & `tbselenium-0.7.0/tbselenium/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.3/tbselenium/test/test_screenshot.py` & `tbselenium-0.7.0/tbselenium/test/test_screenshot.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.3/tbselenium/test/test_stem.py` & `tbselenium-0.7.0/tbselenium/test/test_stem.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.3/tbselenium/test/test_tbdriver.py` & `tbselenium-0.7.0/tbselenium/test/test_tbdriver.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,16 +24,17 @@
     def test_should_load_check_tpo(self):
         congrats = "Congratulations. This browser is configured to use Tor."
         self.tb_driver.load_url_ensure(cm.CHECK_TPO_URL)
         status = self.tb_driver.find_element_by("h1.on")
         self.assertEqual(status.text, congrats)
 
     def test_should_load_hidden_service(self):
-        TPO_ONION_URL = "http://2gzyxa5ihm7nsggfxnu52rck2vv4rvmdlkiu3zzui5du4xyclen53wid.onion/index.html"  # noqa
-        self.tb_driver.load_url_ensure(TPO_ONION_URL, wait_for_page_body=True)
+        # https://support.torproject.org/onionservices/v2-deprecation/index.html
+        TPO_V3_ONION_URL = "http://2gzyxa5ihm7nsggfxnu52rck2vv4rvmdlkiu3zzui5du4xyclen53wid.onion/"  # noqa
+        self.tb_driver.load_url_ensure(TPO_V3_ONION_URL, wait_for_page_body=True)
         self.assertEqual(
             'Tor Project | Anonymity Online',
             self.tb_driver.title)
 
     def test_should_check_environ_in_prepend(self):
         self.tb_driver.quit()
         self.tb_driver = TBDriverFixture(TBB_PATH)
```

### Comparing `tbselenium-0.6.3/tbselenium/test/test_tor.py` & `tbselenium-0.7.0/tbselenium/test/test_tor.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.3/tbselenium/test/test_utils.py` & `tbselenium-0.7.0/tbselenium/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.3/tbselenium.egg-info/PKG-INFO` & `tbselenium-0.7.0/tbselenium.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,152 +1,153 @@
 Metadata-Version: 2.1
 Name: tbselenium
-Version: 0.6.3
+Version: 0.7.0
 Summary: Tor Browser automation with Selenium
 Home-page: https://github.com/webfp/tor-browser-selenium
 Author: Gunes Acar
-License: UNKNOWN
-Description: # tor-browser-selenium [![Build Status](https://app.travis-ci.com/webfp/tor-browser-selenium.svg?branch=main)](https://app.travis-ci.com/webfp/tor-browser-selenium)
-        
-        
-        A Python library to automate Tor Browser with Selenium.
-        
-        ## Installation
-        
-        ```
-        pip install tbselenium
-        ```
-        
-        Install `geckodriver` from the [geckodriver releases page](https://github.com/mozilla/geckodriver/releases/). Make sure you install version v0.23.0 version or newer; older versions may not be compatible with the current Tor Browser series.
-        
-        
-        ## Basic usage
-        ### Using with system `tor`
-        
-        `tor` needs to be installed (`apt install tor`) and running on port 9050.
-        
-        ```python
-        from tbselenium.tbdriver import TorBrowserDriver
-        with TorBrowserDriver("/path/to/TorBrowserBundle/") as driver:
-            driver.get('https://check.torproject.org')
-        ```
-        
-        ### Using with `Stem`
-        First, make sure you have `Stem` installed (`pip install stem`).
-        The following will start a new `tor` process using `Stem`. It will not use the `tor` installed on your system.
-        
-        ```python
-        import tbselenium.common as cm
-        from tbselenium.tbdriver import TorBrowserDriver
-        from tbselenium.utils import launch_tbb_tor_with_stem
-        
-        tbb_dir = "/path/to/TorBrowserBundle/"
-        tor_process = launch_tbb_tor_with_stem(tbb_path=tbb_dir)
-        with TorBrowserDriver(tbb_dir, tor_cfg=cm.USE_STEM) as driver:
-            driver.load_url("https://check.torproject.org")
-        
-        tor_process.kill()
-        ```
-        
-        TorBrowserDriver does not download Tor Browser Bundle (TBB) for you. You should [download](https://www.torproject.org/projects/torbrowser.html.en), extract TBB and provide its path when you initialize `TorBrowserDriver`.
-        
-        ### Setting `geckodriver`'s location without using PATH
-        If `geckodriver` is not on the system PATH, the binary location can be set programmatically:
-        
-        ```python
-        TorBrowserDriver(executable_path="/path/to/geckodriver")
-        ```
-        
-        ## Test and development
-        Install the Python packages that are needed for development and testing:
-        
-        `pip install -r requirements-dev.txt`
-        
-        Install `xvfb` package by running `apt-get install xvfb` or using your distro's package manager.
-        
-        Run the following to launch the tests:
-        
-        `./run_tests.py /path/to/TorBrowserBundle/`
-        
-        By default, tests will be run using `Xvfb`, so the browser will not be visible.
-        You may disable `Xvfb` by exporting the following environment variable:
-        
-        `export NO_XVFB=1`
-        
-        
-        
-        ### Running individual tests
-        First, export a `TBB_PATH` environment variable that points to the TBB version you want to use:
-        
-        `export TBB_PATH=/path/to/tbb/tor-browser_en-US/`
-        
-        Then, use `py.test` to launch the tests you want, e.g.:
-        
-        * `py.test tbselenium/test/test_tbdriver.py`
-        * `py.test tbselenium/test/test_tbdriver.py::TBDriverTest::test_should_load_check_tpo`
-        
-        ### Disabling console logs
-        You can redirect the logs to `/dev/null` by passing the `tbb_logfile_path` initialization parameter:
-        ```python
-        TorBrowserDriver(..., tbb_logfile_path='/dev/null')
-        ```
-        
-        ## Examples
-        Check the [examples](https://github.com/webfp/tor-browser-selenium/tree/master/examples) to discover different ways to use TorBrowserDriver
-        * [check_tpo.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/check_tpo.py): Visit check.torproject.org website and print the network status message
-        * [headless.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/headless.py): Headless visit and screenshot of check.torproject.org using XVFB
-        * [hidden_service.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/hidden_service.py): Search using DuckDuckGo's hidden service
-        * [parallel.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/parallel.py): Visit check.torproject.org with 3 browsers running in parallel
-        * [screenshot.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/screenshot.py): Take a screenshot
-        * [stem_simple.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/stem_simple.py): Using Stem to start the Tor process
-        * [stem_adv.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/stem_adv.py): Using Stem with more advanced configuration
-        
-        
-        ## Compatibility
-        [Tested](https://travis-ci.org/webfp/tor-browser-selenium) with the following Tor Browser Bundle versions on Ubuntu:
-        
-        * 11.5.2
-        * 12.0a2
-        
-        Warning: **Windows and macOS are not supported.**
-        
-        ## Troubleshooting
-        
-        Solutions to potential issues:
-        
-        * Make sure you can run Firefox on the same system. This may help discover issues such as missing libraries, displays etc..
-        * Outdated (or incompatible) Python `selenium` package: This is the source of various obscure errors. Make sure you have an up-to-date `selenium` package installed.
-        * No display: When running on a cloud machine, follow the [headless.py example](https://github.com/webfp/tor-browser-selenium/blob/master/examples/headless.py#L10) to start a virtual display.
-        * Outdated Tor Browser Bundle: Download and use a more recent TBB version.
-        * Make sure you install the latest `geckodriver` version.
-        * Port conflict with other (`Tor`) process: Pick a different SOCKS and controller port using `socks_port` argument.
-        * Use `tbb_logfile_path` argument of TorBrowserDriver to debug obscure errors. This can help with problems due to missing display, missing libraries (e.g. when the LD_LIBRARY_PATH is not set correctly) or other errors that Tor Browser logs to standard output/error.
-        * When you use `LAUNCH_NEW_TBB_TOR` option and get the following [error message](https://github.com/webfp/tor-browser-selenium/issues/62) during the initialization, it's likely that Tor failed to bootstrap (due to network etc.):
-        
-         ```
-         Can't load the profile. Profile Dir: /tmp/tmpO7i1lL/webdriver-py-profilecopy If you specified a log_file in the FirefoxBinary constructor, check it for details
-         ```
-        * `driver.get_cookies()` returns an empty list. This is due to Private Browsing Mode (PBM), which Selenium uses under the hood. See [#79](https://github.com/webfp/tor-browser-selenium/issues/79) for a possible solution.
-        * WebGL is not supported in the headless mode started with `headless=True` due to Firefox bug [#1375585](https://bugzilla.mozilla.org/show_bug.cgi?id=1375585). To enable WebGL in a headless setting, use `pyvirtualdisplay` following the [headless.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/headless.py) example.
-        
-        ## Reference
-        Please consider citing this repository if you use `tor-browser-selenium` in your academic publications.
-        
-        ```
-        @misc{tor-browser-selenium,
-          author = {Gunes Acar and Marc Juarez and individual contributors},
-          title = {tor-browser-selenium - Tor Browser automation with Selenium},
-          year = {2020},
-          publisher = {GitHub},
-          journal = {GitHub repository},
-          howpublished = {\url{https://github.com/webfp/tor-browser-selenium}}
-        }
-        ```
-        
-        ## Credits
-        We greatly benefited from the following two projects:
-        * [tor-browser-selenium](https://github.com/isislovecruft/tor-browser-selenium) by @isislovecruft.
-        * [tor-browser-bundle-testsuite](https://gitweb.torproject.org/boklm/tor-browser-bundle-testsuite.git/) by @boklm.
-        
 Keywords: tor,selenium,tor browser
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# tor-browser-selenium [![Build Status](https://app.travis-ci.com/webfp/tor-browser-selenium.svg?branch=main)](https://app.travis-ci.com/webfp/tor-browser-selenium)
+
+
+A Python library to automate Tor Browser with Selenium WebDriver.
+
+## 📦 Installation
+
+```
+pip install tbselenium
+```
+
+Download `geckodriver` v0.31.0 from the [geckodriver releases page](https://github.com/mozilla/geckodriver/releases/) and add it to PATH.
+
+## 🚀 Usage
+
+Download and extract [Tor Browser](https://www.torproject.org/projects/torbrowser.html.en), and pass its path when you initialize `TorBrowserDriver`.
+
+
+### Using with system `tor`
+
+`tor` needs to be installed (`apt install tor`) and running on port 9050.
+
+```python
+from tbselenium.tbdriver import TorBrowserDriver
+with TorBrowserDriver("/path/to/tor-browser/") as driver:
+    driver.get('https://check.torproject.org')
+```
+
+### Using with `Stem`
+You can use `Stem` to start a new tor process programmatically, and connect to it from `tor-browser-selenium`. Make sure you have `Stem` installed: `pip install stem`:
+
+
+```python
+import tbselenium.common as cm
+from tbselenium.tbdriver import TorBrowserDriver
+from tbselenium.utils import launch_tbb_tor_with_stem
+
+tbb_dir = "/path/to/tor-browser/"
+tor_process = launch_tbb_tor_with_stem(tbb_path=tbb_dir)
+with TorBrowserDriver(tbb_dir, tor_cfg=cm.USE_STEM) as driver:
+    driver.load_url("https://check.torproject.org")
+
+tor_process.kill()
+```
+
+
+## 💡 Examples
+Check the [examples](https://github.com/webfp/tor-browser-selenium/tree/master/examples) to discover different ways to use `tor-browser-selenium`
+* [check_tpo.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/check_tpo.py): Visit the `check.torproject.org` website and print the network status message
+* [headless.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/headless.py): Headless visit and screenshot of check.torproject.org using [PyVirtualDisplay](https://pypi.org/project/PyVirtualDisplay/)
+* [onion_service.py](https://github.com/webfp/tor-browser-selenium/blob/main/examples/onion_service.py): Search using DuckDuckGo's Onion service
+* [parallel.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/parallel.py): Visit `check.torproject.org`` with 3 browsers running in parallel
+* [screenshot.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/screenshot.py): Take a screenshot
+* [stem_simple.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/stem_simple.py): Use Stem to start a `tor` process
+* [stem_adv.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/stem_adv.py): Use Stem to launch `tor` with more advanced configuration
+
+
+
+## 🛠️ Test and development
+
+* Browse the [existing tests](https://github.com/webfp/tor-browser-selenium/tree/main/tbselenium/test) to find out about different ways you can use `tor-browser-selenium`.
+
+* For development and testing first install the necessary Python packages:
+  `pip install -r requirements-dev.txt`
+
+* Install the `xvfb` package by running `apt-get install xvfb` or using your distro's package manager.
+
+* Run the following to launch the tests:
+
+  `./run_tests.py /path/to/tor-browser/`
+
+* By default, tests will be run using `Xvfb`, so the browser window will not be visible.
+You may disable `Xvfb` by setting the `NO_XVFB` environment variable:
+
+  `export NO_XVFB=1`
+
+
+### Running individual tests
+* First, export the path to Tor Browser folder in the `TBB_PATH` environment variable.
+
+`export TBB_PATH=/path/to/tbb/tor-browser/`
+
+* Then, use `py.test` to launch the tests you want, e.g.:
+
+* `py.test tbselenium/test/test_tbdriver.py`
+* `py.test tbselenium/test/test_tbdriver.py::TBDriverTest::test_should_load_check_tpo`
+
+
+### Using a custom `geckodriver`
+A custom `geckodriver` binary can be set via the `executable_path` argument:
+
+```python
+TorBrowserDriver(executable_path="/path/to/geckodriver")
+```
+
+### Disabling console logs
+You can redirect the logs to `/dev/null` by passing the `tbb_logfile_path` initialization parameter:
+```python
+TorBrowserDriver(..., tbb_logfile_path='/dev/null')
+```
+
+## ⚙️ Compatibility
+
+Warning: **Windows and macOS are not supported.**
+
+[Tested](https://travis-ci.org/webfp/tor-browser-selenium) with the following Tor Browser versions on Ubuntu:
+
+* **Stable**: 12.0.7
+* **Alpha**: 12.5a7
+
+If you need to use a different version of Tor Browser, [view the past test runs](https://travis-ci.org/webfp/tor-browser-selenium) to find out the compatible `selenium` and `geckodriver` versions.
+
+## 🔧 Troubleshooting
+
+Solutions to potential issues:
+
+* Make sure you have compatible dependencies. While older or newer versions may work, they may cause issues.
+  - [Tor Browser](https://www.torproject.org/download/) needs to be downloaded and extracted.
+  - Python [`selenium`](https://www.selenium.dev/) (`pip install -U selenium`).
+  - `geckodriver` [version 0.31.0](https://github.com/mozilla/geckodriver/releases/tag/v0.31.0).
+
+* Running Firefox on the same system may help diagnose issues such as missing libraries and displays.
+* `Process unexpectedly closed with status 1`: If you encounter this on a remote machine you connect via SSH, you may need to enable the [headless mode](https://github.com/webfp/tor-browser-selenium/blob/master/examples/headless.py).
+* Port conflict with other (`Tor`) process: Pick a different SOCKS and controller port using the `socks_port` argument.
+* Use `tbb_logfile_path` argument of TorBrowserDriver to debug obscure errors. This can help with problems due to missing display, missing libraries (e.g. when the LD_LIBRARY_PATH is not set correctly) or other errors that Tor Browser logs to standard output/error.
+* `driver.get_cookies()` returns an empty list. This is due to Private Browsing Mode (PBM), which Selenium uses under the hood. See [#79](https://github.com/webfp/tor-browser-selenium/issues/79) for a possible solution.
+* WebGL is not supported in the headless mode started with `headless=True` due to a Firefox bug ([#1375585](https://bugzilla.mozilla.org/show_bug.cgi?id=1375585)). To enable WebGL in a headless setting, use `pyvirtualdisplay` following the [headless.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/headless.py) example.
+
+## 📚 Reference
+Please use the following reference if you use `tor-browser-selenium` in your academic publications.
+
+```
+@misc{tor-browser-selenium,
+  author = {Gunes Acar and Marc Juarez and individual contributors},
+  title = {tor-browser-selenium - Tor Browser automation with Selenium},
+  year = {2023},
+  publisher = {GitHub},
+  howpublished = {\url{https://github.com/webfp/tor-browser-selenium}}
+}
+```
+
+## 🙌 Credits
+We greatly benefited from the [tor-browser-bundle-testsuite](https://gitlab.torproject.org/tpo/applications/tor-browser-bundle-testsuite) and [tor-browser-selenium](https://github.com/isislovecruft/tor-browser-selenium) projects.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tbselenium-0.6.3/tbselenium.egg-info/SOURCES.txt` & `tbselenium-0.7.0/tbselenium.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,30 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 tbselenium/__init__.py
 tbselenium/common.py
 tbselenium/exceptions.py
-tbselenium/set_profile.py
-tbselenium/set_profile_nops.py
 tbselenium/tbbinary.py
 tbselenium/tbdriver.py
-tbselenium/unpack_tb.py
 tbselenium/utils.py
 tbselenium.egg-info/PKG-INFO
 tbselenium.egg-info/SOURCES.txt
 tbselenium.egg-info/dependency_links.txt
 tbselenium.egg-info/requires.txt
 tbselenium.egg-info/top_level.txt
 tbselenium/test/__init__.py
 tbselenium/test/conftest.py
 tbselenium/test/fixtures.py
 tbselenium/test/test_addons.py
 tbselenium/test/test_bridge.py
 tbselenium/test/test_browser.py
 tbselenium/test/test_context_switch.py
-tbselenium/test/test_disable_javascript.py
+tbselenium/test/test_disable_features.py
 tbselenium/test/test_env.py
 tbselenium/test/test_exceptions.py
 tbselenium/test/test_screenshot.py
 tbselenium/test/test_set_security_level.py
 tbselenium/test/test_stem.py
 tbselenium/test/test_tbdriver.py
 tbselenium/test/test_tor.py
```

