# Comparing `tmp/tbselenium-0.6.2.tar.gz` & `tmp/tbselenium-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tbselenium-0.6.2.tar", last modified: Mon Dec 13 22:28:01 2021, max compression
+gzip compressed data, was "tbselenium-0.6.3.tar", last modified: Tue Sep 20 20:30:39 2022, max compression
```

## Comparing `tbselenium-0.6.2.tar` & `tbselenium-0.6.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 gacar     (1000) gacar     (1000)        0 2021-12-13 22:28:01.657029 tbselenium-0.6.2/
--rw-rw-r--   0 gacar     (1000) gacar     (1000)     8443 2021-12-13 22:28:01.657029 tbselenium-0.6.2/PKG-INFO
--rw-rw-r--   0 gacar     (1000) gacar     (1000)     7015 2021-12-13 21:42:08.000000 tbselenium-0.6.2/README.md
--rw-rw-r--   0 gacar     (1000) gacar     (1000)       79 2021-12-13 22:28:01.657029 tbselenium-0.6.2/setup.cfg
--rw-rw-r--   0 gacar     (1000) gacar     (1000)      521 2021-12-13 21:43:01.000000 tbselenium-0.6.2/setup.py
-drwxrwxr-x   0 gacar     (1000) gacar     (1000)        0 2021-12-13 22:28:01.649029 tbselenium-0.6.2/tbselenium/
--rw-rw-r--   0 gacar     (1000) gacar     (1000)        0 2017-10-04 01:40:34.000000 tbselenium-0.6.2/tbselenium/__init__.py
--rw-rw-r--   0 gacar     (1000) gacar     (1000)     2071 2021-11-24 22:01:11.000000 tbselenium-0.6.2/tbselenium/common.py
--rw-rw-r--   0 gacar     (1000) gacar     (1000)      336 2017-10-04 01:40:34.000000 tbselenium-0.6.2/tbselenium/exceptions.py
--rw-rw-r--   0 gacar     (1000) gacar     (1000)      957 2021-11-23 21:31:02.000000 tbselenium-0.6.2/tbselenium/set_profile.py
--rw-rw-r--   0 gacar     (1000) gacar     (1000)      305 2021-11-23 20:03:26.000000 tbselenium-0.6.2/tbselenium/set_profile_nops.py
--rw-rw-r--   0 gacar     (1000) gacar     (1000)      423 2017-10-20 03:12:07.000000 tbselenium-0.6.2/tbselenium/tbbinary.py
--rw-rw-r--   0 gacar     (1000) gacar     (1000)    15057 2021-12-13 21:40:59.000000 tbselenium-0.6.2/tbselenium/tbdriver.py
-drwxrwxr-x   0 gacar     (1000) gacar     (1000)        0 2021-12-13 22:28:01.657029 tbselenium-0.6.2/tbselenium/test/
--rw-rw-r--   0 gacar     (1000) gacar     (1000)      428 2021-11-21 18:33:07.000000 tbselenium-0.6.2/tbselenium/test/__init__.py
--rw-rw-r--   0 gacar     (1000) gacar     (1000)     1375 2021-11-24 22:01:11.000000 tbselenium-0.6.2/tbselenium/test/conftest.py
--rw-rw-r--   0 gacar     (1000) gacar     (1000)     4509 2021-12-13 22:11:25.000000 tbselenium-0.6.2/tbselenium/test/fixtures.py
--rw-rw-r--   0 gacar     (1000) gacar     (1000)     2213 2021-11-24 22:01:11.000000 tbselenium-0.6.2/tbselenium/test/test_addons.py
--rw-rw-r--   0 gacar     (1000) gacar     (1000)     1548 2021-11-24 22:01:11.000000 tbselenium-0.6.2/tbselenium/test/test_bridge.py
--rw-rw-r--   0 gacar     (1000) gacar     (1000)     2557 2021-11-24 22:01:11.000000 tbselenium-0.6.2/tbselenium/test/test_browser.py
--rw-rw-r--   0 gacar     (1000) gacar     (1000)     1686 2021-11-24 22:01:11.000000 tbselenium-0.6.2/tbselenium/test/test_context_switch.py
--rw-rw-r--   0 gacar     (1000) gacar     (1000)      862 2019-01-28 03:06:32.000000 tbselenium-0.6.2/tbselenium/test/test_disable_javascript.py
--rw-rw-r--   0 gacar     (1000) gacar     (1000)      807 2021-11-24 22:01:11.000000 tbselenium-0.6.2/tbselenium/test/test_env.py
--rw-rw-r--   0 gacar     (1000) gacar     (1000)     4160 2021-11-24 22:01:11.000000 tbselenium-0.6.2/tbselenium/test/test_exceptions.py
--rw-rw-r--   0 gacar     (1000) gacar     (1000)     1369 2017-10-19 13:40:30.000000 tbselenium-0.6.2/tbselenium/test/test_screenshot.py
--rw-rw-r--   0 gacar     (1000) gacar     (1000)     5402 2021-11-24 22:01:11.000000 tbselenium-0.6.2/tbselenium/test/test_set_security_level.py
--rw-rw-r--   0 gacar     (1000) gacar     (1000)     2078 2021-11-24 22:01:11.000000 tbselenium-0.6.2/tbselenium/test/test_stem.py
--rw-rw-r--   0 gacar     (1000) gacar     (1000)     4857 2021-12-13 21:40:59.000000 tbselenium-0.6.2/tbselenium/test/test_tbdriver.py
--rw-rw-r--   0 gacar     (1000) gacar     (1000)      619 2019-01-24 04:43:00.000000 tbselenium-0.6.2/tbselenium/test/test_tor.py
--rw-rw-r--   0 gacar     (1000) gacar     (1000)      889 2017-10-20 05:26:59.000000 tbselenium-0.6.2/tbselenium/test/test_utils.py
--rw-rw-r--   0 gacar     (1000) gacar     (1000)     1521 2021-11-21 11:47:40.000000 tbselenium-0.6.2/tbselenium/unpack_tb.py
--rw-rw-r--   0 gacar     (1000) gacar     (1000)     3546 2021-11-24 17:32:08.000000 tbselenium-0.6.2/tbselenium/utils.py
-drwxrwxr-x   0 gacar     (1000) gacar     (1000)        0 2021-12-13 22:28:01.653029 tbselenium-0.6.2/tbselenium.egg-info/
--rw-rw-r--   0 gacar     (1000) gacar     (1000)     8443 2021-12-13 22:28:01.000000 tbselenium-0.6.2/tbselenium.egg-info/PKG-INFO
--rw-rw-r--   0 gacar     (1000) gacar     (1000)      934 2021-12-13 22:28:01.000000 tbselenium-0.6.2/tbselenium.egg-info/SOURCES.txt
--rw-rw-r--   0 gacar     (1000) gacar     (1000)        1 2021-12-13 22:28:01.000000 tbselenium-0.6.2/tbselenium.egg-info/dependency_links.txt
--rw-rw-r--   0 gacar     (1000) gacar     (1000)       12 2021-12-13 22:28:01.000000 tbselenium-0.6.2/tbselenium.egg-info/requires.txt
--rw-rw-r--   0 gacar     (1000) gacar     (1000)       11 2021-12-13 22:28:01.000000 tbselenium-0.6.2/tbselenium.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-20 20:30:39.541347 tbselenium-0.6.3/
+-rw-r--r--   0 root         (0) root         (0)     8450 2022-09-20 20:30:39.541347 tbselenium-0.6.3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     7022 2022-09-20 06:40:34.000000 tbselenium-0.6.3/README.md
+-rw-rw-r--   0 root         (0) root         (0)       79 2022-09-20 20:30:39.541347 tbselenium-0.6.3/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      521 2022-09-20 20:28:22.000000 tbselenium-0.6.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-20 20:30:39.537347 tbselenium-0.6.3/tbselenium/
+-rw-rw-r--   0 root         (0) root         (0)        0 2017-10-04 01:40:34.000000 tbselenium-0.6.3/tbselenium/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2071 2021-11-24 22:01:11.000000 tbselenium-0.6.3/tbselenium/common.py
+-rw-rw-r--   0 root         (0) root         (0)      336 2017-10-04 01:40:34.000000 tbselenium-0.6.3/tbselenium/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)      957 2021-11-23 21:31:02.000000 tbselenium-0.6.3/tbselenium/set_profile.py
+-rw-rw-r--   0 root         (0) root         (0)      305 2021-11-23 20:03:26.000000 tbselenium-0.6.3/tbselenium/set_profile_nops.py
+-rw-rw-r--   0 root         (0) root         (0)      423 2017-10-20 03:12:07.000000 tbselenium-0.6.3/tbselenium/tbbinary.py
+-rw-rw-r--   0 root         (0) root         (0)    15213 2022-09-20 20:20:22.000000 tbselenium-0.6.3/tbselenium/tbdriver.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-20 20:30:39.541347 tbselenium-0.6.3/tbselenium/test/
+-rw-rw-r--   0 root         (0) root         (0)      428 2021-11-21 18:33:07.000000 tbselenium-0.6.3/tbselenium/test/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1375 2021-11-24 22:01:11.000000 tbselenium-0.6.3/tbselenium/test/conftest.py
+-rw-rw-r--   0 root         (0) root         (0)     4509 2021-12-13 22:11:25.000000 tbselenium-0.6.3/tbselenium/test/fixtures.py
+-rw-rw-r--   0 root         (0) root         (0)     2193 2022-08-03 11:55:54.000000 tbselenium-0.6.3/tbselenium/test/test_addons.py
+-rw-rw-r--   0 root         (0) root         (0)     1548 2021-11-24 22:01:11.000000 tbselenium-0.6.3/tbselenium/test/test_bridge.py
+-rw-rw-r--   0 root         (0) root         (0)     2557 2021-11-24 22:01:11.000000 tbselenium-0.6.3/tbselenium/test/test_browser.py
+-rw-rw-r--   0 root         (0) root         (0)     1686 2021-11-24 22:01:11.000000 tbselenium-0.6.3/tbselenium/test/test_context_switch.py
+-rw-rw-r--   0 root         (0) root         (0)      862 2019-01-28 03:06:32.000000 tbselenium-0.6.3/tbselenium/test/test_disable_javascript.py
+-rw-rw-r--   0 root         (0) root         (0)      807 2021-11-24 22:01:11.000000 tbselenium-0.6.3/tbselenium/test/test_env.py
+-rw-rw-r--   0 root         (0) root         (0)     4160 2021-11-24 22:01:11.000000 tbselenium-0.6.3/tbselenium/test/test_exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)     1369 2017-10-19 13:40:30.000000 tbselenium-0.6.3/tbselenium/test/test_screenshot.py
+-rw-rw-r--   0 root         (0) root         (0)     5402 2021-11-24 22:01:11.000000 tbselenium-0.6.3/tbselenium/test/test_set_security_level.py
+-rw-rw-r--   0 root         (0) root         (0)     2078 2021-11-24 22:01:11.000000 tbselenium-0.6.3/tbselenium/test/test_stem.py
+-rw-rw-r--   0 root         (0) root         (0)     5488 2022-09-20 20:20:22.000000 tbselenium-0.6.3/tbselenium/test/test_tbdriver.py
+-rw-rw-r--   0 root         (0) root         (0)      619 2019-01-24 04:43:00.000000 tbselenium-0.6.3/tbselenium/test/test_tor.py
+-rw-rw-r--   0 root         (0) root         (0)      889 2017-10-20 05:26:59.000000 tbselenium-0.6.3/tbselenium/test/test_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     1521 2021-11-21 11:47:40.000000 tbselenium-0.6.3/tbselenium/unpack_tb.py
+-rw-rw-r--   0 root         (0) root         (0)     3546 2021-12-27 14:34:35.000000 tbselenium-0.6.3/tbselenium/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-20 20:30:39.537347 tbselenium-0.6.3/tbselenium.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     8450 2022-09-20 20:30:39.000000 tbselenium-0.6.3/tbselenium.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      934 2022-09-20 20:30:39.000000 tbselenium-0.6.3/tbselenium.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2022-09-20 20:30:39.000000 tbselenium-0.6.3/tbselenium.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       12 2022-09-20 20:30:39.000000 tbselenium-0.6.3/tbselenium.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       11 2022-09-20 20:30:39.000000 tbselenium-0.6.3/tbselenium.egg-info/top_level.txt
```

### Comparing `tbselenium-0.6.2/PKG-INFO` & `tbselenium-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: tbselenium
-Version: 0.6.2
+Version: 0.6.3
 Summary: Tor Browser automation with Selenium
 Home-page: https://github.com/webfp/tor-browser-selenium
 Author: Gunes Acar
 License: UNKNOWN
-Description: # tor-browser-selenium [![Build Status](https://travis-ci.com/webfp/tor-browser-selenium.svg?branch=main)](https://travis-ci.com/webfp/tor-browser-selenium)
+Description: # tor-browser-selenium [![Build Status](https://app.travis-ci.com/webfp/tor-browser-selenium.svg?branch=main)](https://app.travis-ci.com/webfp/tor-browser-selenium)
         
         
         A Python library to automate Tor Browser with Selenium.
         
         ## Installation
         
         ```
@@ -100,16 +100,16 @@
         * [stem_simple.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/stem_simple.py): Using Stem to start the Tor process
         * [stem_adv.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/stem_adv.py): Using Stem with more advanced configuration
         
         
         ## Compatibility
         [Tested](https://travis-ci.org/webfp/tor-browser-selenium) with the following Tor Browser Bundle versions on Ubuntu:
         
-        * 11.0.2
-        * 11.0a10
+        * 11.5.2
+        * 12.0a2
         
         Warning: **Windows and macOS are not supported.**
         
         ## Troubleshooting
         
         Solutions to potential issues:
```

### Comparing `tbselenium-0.6.2/README.md` & `tbselenium-0.6.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# tor-browser-selenium [![Build Status](https://travis-ci.com/webfp/tor-browser-selenium.svg?branch=main)](https://travis-ci.com/webfp/tor-browser-selenium)
+# tor-browser-selenium [![Build Status](https://app.travis-ci.com/webfp/tor-browser-selenium.svg?branch=main)](https://app.travis-ci.com/webfp/tor-browser-selenium)
 
 
 A Python library to automate Tor Browser with Selenium.
 
 ## Installation
 
 ```
@@ -93,16 +93,16 @@
 * [stem_simple.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/stem_simple.py): Using Stem to start the Tor process
 * [stem_adv.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/stem_adv.py): Using Stem with more advanced configuration
 
 
 ## Compatibility
 [Tested](https://travis-ci.org/webfp/tor-browser-selenium) with the following Tor Browser Bundle versions on Ubuntu:
 
-* 11.0.2
-* 11.0a10
+* 11.5.2
+* 12.0a2
 
 Warning: **Windows and macOS are not supported.**
 
 ## Troubleshooting
 
 Solutions to potential issues:
```

### Comparing `tbselenium-0.6.2/setup.py` & `tbselenium-0.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 setup(
     author='Gunes Acar',
     name="tbselenium",
     description="Tor Browser automation with Selenium",
     keywords=["tor", "selenium", "tor browser"],
-    version="0.6.2",
+    version="0.6.3",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/webfp/tor-browser-selenium',
     packages=["tbselenium", "tbselenium.test"],
     install_requires=[
         "selenium>=4"
     ]
```

### Comparing `tbselenium-0.6.2/tbselenium/common.py` & `tbselenium-0.6.3/tbselenium/common.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.2/tbselenium/set_profile.py` & `tbselenium-0.6.3/tbselenium/set_profile.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.2/tbselenium/tbdriver.py` & `tbselenium-0.6.3/tbselenium/tbdriver.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,16 @@
                  pref_dict={},
                  socks_port=None,
                  control_port=None,
                  extensions=[],
                  default_bridge_type="",
                  headless=False,
                  options=None,
-                 use_custom_profile=False
+                 use_custom_profile=False,
+                 geckodriver_port=0  # by default a random port will be used
                  ):
 
         # use_custom_profile: whether to launch from and *write to* the given
         # profile
         # False: copy the profile to a tempdir; remove the temp folder on quit
         # True: use the given profile without copying. This can be used to keep
         # a stateful profile across different launches of the Tor Browser.
@@ -75,20 +76,22 @@
         self.export_env_vars()
         # TODO:
         # self.binary = self.get_tb_binary(logfile=tbb_logfile_path)
         if use_custom_profile:
             tbb_service = Service(
                 executable_path=executable_path,
                 log_path=tbb_logfile_path,
-                service_args=["--marionette-port", "2828"]
+                service_args=["--marionette-port", "2828"],
+                port=geckodriver_port
                 )
         else:
             tbb_service = Service(
                 executable_path=executable_path,
-                log_path=tbb_logfile_path
+                log_path=tbb_logfile_path,
+                port=geckodriver_port
                 )
         self.options.binary = self.tbb_fx_binary_path
         self.options.add_argument('--class')
         self.options.add_argument('"Tor Browser"')
         if headless:
             self.options.headless = True
```

### Comparing `tbselenium-0.6.2/tbselenium/test/conftest.py` & `tbselenium-0.6.3/tbselenium/test/conftest.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.2/tbselenium/test/fixtures.py` & `tbselenium-0.6.3/tbselenium/test/fixtures.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.2/tbselenium/test/test_addons.py` & `tbselenium-0.6.3/tbselenium/test/test_addons.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             driver.load_url_ensure(self.HE_HTTP_URL)
             WebDriverWait(driver, self.TEST_LONG_WAIT).\
                 until(EC.title_contains("httpbin"))
             self.assertEqual(driver.current_url, self.HE_HTTPS_URL)
 
     def test_builtin_addons_should_come_installed(self):
         """Make sure that the built-in addons come installed."""
-        EXPECTED_ADDONS = set(['HTTPS Everywhere', 'NoScript'])
+        EXPECTED_ADDONS = set(['NoScript'])
         found_addons = []
         with TBDriverFixture(TBB_PATH) as driver:
             found_addons = self.get_list_of_installed_addons(driver)
             assert EXPECTED_ADDONS == set(found_addons)
 
     def test_should_install_custom_extension(self):
         XPI_NAME = "borderify.xpi"  # sample extension based on:
```

### Comparing `tbselenium-0.6.2/tbselenium/test/test_bridge.py` & `tbselenium-0.6.3/tbselenium/test/test_bridge.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.2/tbselenium/test/test_browser.py` & `tbselenium-0.6.3/tbselenium/test/test_browser.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.2/tbselenium/test/test_context_switch.py` & `tbselenium-0.6.3/tbselenium/test/test_context_switch.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.2/tbselenium/test/test_disable_javascript.py` & `tbselenium-0.6.3/tbselenium/test/test_disable_javascript.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.2/tbselenium/test/test_env.py` & `tbselenium-0.6.3/tbselenium/test/test_env.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.2/tbselenium/test/test_exceptions.py` & `tbselenium-0.6.3/tbselenium/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.2/tbselenium/test/test_screenshot.py` & `tbselenium-0.6.3/tbselenium/test/test_screenshot.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.2/tbselenium/test/test_set_security_level.py` & `tbselenium-0.6.3/tbselenium/test/test_set_security_level.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.2/tbselenium/test/test_stem.py` & `tbselenium-0.6.3/tbselenium/test/test_stem.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.2/tbselenium/test/test_tbdriver.py` & `tbselenium-0.6.3/tbselenium/test/test_tbdriver.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from time import time
 
 from selenium.webdriver.common.timeouts import Timeouts
 from selenium.common.exceptions import TimeoutException
 from tbselenium import common as cm
 from tbselenium.test import TBB_PATH
 from tbselenium.test.fixtures import TBDriverFixture
+from selenium.webdriver.common.utils import free_port
+from tbselenium.utils import is_busy
 
 
 class TBDriverTest(unittest.TestCase):
     def setUp(self):
         self.tb_driver = TBDriverFixture(TBB_PATH)
 
     def tearDown(self):
@@ -122,9 +124,21 @@
             assert isdir(tmp_dir)
             assert driver.temp_profile_dir == tmp_dir
             driver.load_url_ensure(cm.CHECK_TPO_URL)
         mod_time_after = getmtime(self.TBB_PROFILE_PATH)
         self.assertEqual(mod_time_before, mod_time_after)
 
 
+class TBDriverCustomGeckoDriverPort(unittest.TestCase):
+
+    def test_should_accept_custom_geckodriver_port(self):
+        """Make sure we accept a custom port number to run geckodriver on."""
+        random_port = free_port()
+        with TBDriverFixture(TBB_PATH, geckodriver_port=random_port) as driver:
+            driver.load_url_ensure(cm.ABOUT_TOR_URL)
+            self.assertTrue(is_busy(random_port))  # check if the port is used
+        # check if the port is closed after we quit
+        self.assertFalse(is_busy(random_port))
+
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `tbselenium-0.6.2/tbselenium/test/test_tor.py` & `tbselenium-0.6.3/tbselenium/test/test_tor.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.2/tbselenium/test/test_utils.py` & `tbselenium-0.6.3/tbselenium/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.2/tbselenium/unpack_tb.py` & `tbselenium-0.6.3/tbselenium/unpack_tb.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.2/tbselenium/utils.py` & `tbselenium-0.6.3/tbselenium/utils.py`

 * *Files identical despite different names*

### Comparing `tbselenium-0.6.2/tbselenium.egg-info/PKG-INFO` & `tbselenium-0.6.3/tbselenium.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: tbselenium
-Version: 0.6.2
+Version: 0.6.3
 Summary: Tor Browser automation with Selenium
 Home-page: https://github.com/webfp/tor-browser-selenium
 Author: Gunes Acar
 License: UNKNOWN
-Description: # tor-browser-selenium [![Build Status](https://travis-ci.com/webfp/tor-browser-selenium.svg?branch=main)](https://travis-ci.com/webfp/tor-browser-selenium)
+Description: # tor-browser-selenium [![Build Status](https://app.travis-ci.com/webfp/tor-browser-selenium.svg?branch=main)](https://app.travis-ci.com/webfp/tor-browser-selenium)
         
         
         A Python library to automate Tor Browser with Selenium.
         
         ## Installation
         
         ```
@@ -100,16 +100,16 @@
         * [stem_simple.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/stem_simple.py): Using Stem to start the Tor process
         * [stem_adv.py](https://github.com/webfp/tor-browser-selenium/tree/master/examples/stem_adv.py): Using Stem with more advanced configuration
         
         
         ## Compatibility
         [Tested](https://travis-ci.org/webfp/tor-browser-selenium) with the following Tor Browser Bundle versions on Ubuntu:
         
-        * 11.0.2
-        * 11.0a10
+        * 11.5.2
+        * 12.0a2
         
         Warning: **Windows and macOS are not supported.**
         
         ## Troubleshooting
         
         Solutions to potential issues:
```

### Comparing `tbselenium-0.6.2/tbselenium.egg-info/SOURCES.txt` & `tbselenium-0.6.3/tbselenium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

