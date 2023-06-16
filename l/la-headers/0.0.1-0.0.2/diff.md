# Comparing `tmp/la-headers-0.0.1.tar.gz` & `tmp/la-headers-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "la-headers-0.0.1.tar", last modified: Sat Sep 10 11:25:40 2022, max compression
+gzip compressed data, was "la-headers-0.0.2.tar", last modified: Fri Jun 16 04:58:03 2023, max compression
```

## Comparing `la-headers-0.0.1.tar` & `la-headers-0.0.2.tar`

### file list

```diff
@@ -1,50 +1,60 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-09-10 11:25:29.024775 la-headers-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-09-10 11:25:29.024775 la-headers-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     2928 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/accept/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      908 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/accept/chrome.py
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/accept/firefox.py
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/accept_encondig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/accept_encondig/chrome.py
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/accept_encondig/firefox.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/accept_language/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/accept_language/chrome.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/accept_language/firefox.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4851 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/browser/chrome.py
--rw-r--r--   0 runner    (1001) docker     (121)     7637 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/browser/firefox.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/operating_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/operating_system/android.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/operating_system/linux.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/operating_system/mac.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/operating_system/windows.py
--rw-r--r--   0 runner    (1001) docker     (121)     1897 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/prefabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/sec_ch_ua/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/sec_ch_ua/chromie.py
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/sec_ch_ua/firefox.py
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/sec_ch_ua_mobile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/sec_ch_ua_mobile/chromie.py
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/sec_ch_ua_mobile/firefox.py
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/sec_ch_ua_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      487 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/sec_ch_ua_platform/chromie.py
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/sec_ch_ua_platform/firefox.py
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/system/android.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/system/linux.py
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/system/mac.py
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/system/windows.py
--rw-r--r--   0 runner    (1001) docker     (121)      807 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/upgrade_insecure_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       77 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/upgrade_insecure_requests/chrome.py
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/upgrade_insecure_requests/firefox.py
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/upgrade_insecure_requests/safari.py
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/user_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-09-10 11:25:29.024775 la-headers-0.0.1/la_headers/user_agent/chrome.py
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-09-10 11:25:29.028775 la-headers-0.0.1/la_headers/user_agent/firefox.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-09-10 11:25:29.028775 la-headers-0.0.1/la_headers/user_agent/safari.py
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-09-10 11:25:29.028775 la-headers-0.0.1/la_headers/utility.py
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-09-10 11:25:29.028775 la-headers-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-10 11:25:29.028775 la-headers-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-09-10 11:25:29.028775 la-headers-0.0.1/tests/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-09-10 11:25:29.028775 la-headers-0.0.1/tests/test_random_headers.py
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-09-10 11:25:29.028775 la-headers-0.0.1/tests/test_system.py
--rw-------   0 runner    (1001) docker     (121)      569 2022-09-10 11:25:40.177117 la-headers-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-06-14 13:33:02.341257 la-headers-0.0.2/LICENSE
+-rw-r--r--   0        0        0       77 2023-06-14 13:33:02.341257 la-headers-0.0.2/README.md
+-rw-r--r--   0        0        0     2970 2023-06-16 04:23:03.544579 la-headers-0.0.2/la_headers/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-15 05:31:03.980785 la-headers-0.0.2/la_headers/gen/__init__.py
+-rw-r--r--   0        0        0      828 2023-06-16 03:57:13.897238 la-headers-0.0.2/la_headers/gen/accept/__init__.py
+-rw-r--r--   0        0        0      686 2023-06-15 15:37:06.116517 la-headers-0.0.2/la_headers/gen/accept/brave.py
+-rw-r--r--   0        0        0     1063 2023-06-15 15:29:06.448909 la-headers-0.0.2/la_headers/gen/accept/chrome.py
+-rw-r--r--   0        0        0     1278 2023-06-15 15:31:46.443401 la-headers-0.0.2/la_headers/gen/accept/firefox.py
+-rw-r--r--   0        0        0      765 2023-06-16 03:57:10.445182 la-headers-0.0.2/la_headers/gen/accept_encondig/__init__.py
+-rw-r--r--   0        0        0       83 2023-06-16 03:39:27.281854 la-headers-0.0.2/la_headers/gen/accept_encondig/brave.py
+-rw-r--r--   0        0        0       84 2023-06-14 13:33:02.345257 la-headers-0.0.2/la_headers/gen/accept_encondig/chrome.py
+-rw-r--r--   0        0        0       85 2023-06-14 13:33:02.345257 la-headers-0.0.2/la_headers/gen/accept_encondig/firefox.py
+-rw-r--r--   0        0        0        0 2023-06-14 13:33:02.345257 la-headers-0.0.2/la_headers/gen/accept_language/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 13:33:02.345257 la-headers-0.0.2/la_headers/gen/accept_language/chrome.py
+-rw-r--r--   0        0        0        0 2023-06-14 13:33:02.345257 la-headers-0.0.2/la_headers/gen/accept_language/firefox.py
+-rw-r--r--   0        0        0      684 2023-06-16 04:33:14.276821 la-headers-0.0.2/la_headers/gen/sec_ch_ua/__init__.py
+-rw-r--r--   0        0        0      270 2023-06-16 04:34:32.313942 la-headers-0.0.2/la_headers/gen/sec_ch_ua/brave.py
+-rw-r--r--   0        0        0     1071 2023-06-16 04:34:51.346221 la-headers-0.0.2/la_headers/gen/sec_ch_ua/chromie.py
+-rw-r--r--   0        0        0      219 2023-06-16 04:35:08.074467 la-headers-0.0.2/la_headers/gen/sec_ch_ua/firefox.py
+-rw-r--r--   0        0        0      623 2023-06-16 03:57:01.393036 la-headers-0.0.2/la_headers/gen/sec_ch_ua_mobile/__init__.py
+-rw-r--r--   0        0        0      253 2023-06-16 03:45:49.565451 la-headers-0.0.2/la_headers/gen/sec_ch_ua_mobile/brave.py
+-rw-r--r--   0        0        0      258 2023-06-14 13:33:02.345257 la-headers-0.0.2/la_headers/gen/sec_ch_ua_mobile/chromie.py
+-rw-r--r--   0        0        0      207 2023-06-14 13:33:02.345257 la-headers-0.0.2/la_headers/gen/sec_ch_ua_mobile/firefox.py
+-rw-r--r--   0        0        0      639 2023-06-16 03:56:56.676959 la-headers-0.0.2/la_headers/gen/sec_ch_ua_platform/__init__.py
+-rw-r--r--   0        0        0      675 2023-06-16 03:55:26.439517 la-headers-0.0.2/la_headers/gen/sec_ch_ua_platform/brave.py
+-rw-r--r--   0        0        0      685 2023-06-16 03:54:13.402380 la-headers-0.0.2/la_headers/gen/sec_ch_ua_platform/chromie.py
+-rw-r--r--   0        0        0      362 2023-06-15 05:15:53.739305 la-headers-0.0.2/la_headers/gen/sec_ch_ua_platform/firefox.py
+-rw-r--r--   0        0        0     1382 2023-06-15 05:58:46.755583 la-headers-0.0.2/la_headers/gen/system/__init__.py
+-rw-r--r--   0        0        0      349 2023-06-14 14:44:58.215932 la-headers-0.0.2/la_headers/gen/system/android.py
+-rw-r--r--   0        0        0      271 2023-06-14 14:44:55.471869 la-headers-0.0.2/la_headers/gen/system/linux.py
+-rw-r--r--   0        0        0      299 2023-06-14 14:44:53.143815 la-headers-0.0.2/la_headers/gen/system/mac.py
+-rw-r--r--   0        0        0      384 2023-06-14 14:45:00.911994 la-headers-0.0.2/la_headers/gen/system/ubuntu.py
+-rw-r--r--   0        0        0      364 2023-06-14 14:44:48.223702 la-headers-0.0.2/la_headers/gen/system/windows.py
+-rw-r--r--   0        0        0      973 2023-06-16 03:57:50.053828 la-headers-0.0.2/la_headers/gen/upgrade_insecure_requests/__init__.py
+-rw-r--r--   0        0        0       77 2023-06-16 03:57:27.945467 la-headers-0.0.2/la_headers/gen/upgrade_insecure_requests/brave.py
+-rw-r--r--   0        0        0       78 2023-06-14 13:33:02.349257 la-headers-0.0.2/la_headers/gen/upgrade_insecure_requests/chrome.py
+-rw-r--r--   0        0        0       79 2023-06-14 13:33:02.349257 la-headers-0.0.2/la_headers/gen/upgrade_insecure_requests/firefox.py
+-rw-r--r--   0        0        0       79 2023-06-14 13:33:02.349257 la-headers-0.0.2/la_headers/gen/upgrade_insecure_requests/safari.py
+-rw-r--r--   0        0        0      785 2023-06-16 04:00:54.640909 la-headers-0.0.2/la_headers/gen/user_agent/__init__.py
+-rw-r--r--   0        0        0      410 2023-06-16 04:00:16.348261 la-headers-0.0.2/la_headers/gen/user_agent/brave.py
+-rw-r--r--   0        0        0      415 2023-06-15 15:31:41.467323 la-headers-0.0.2/la_headers/gen/user_agent/chrome.py
+-rw-r--r--   0        0        0      536 2023-06-15 15:33:20.840896 la-headers-0.0.2/la_headers/gen/user_agent/firefox.py
+-rw-r--r--   0        0        0      427 2023-06-14 13:33:02.349257 la-headers-0.0.2/la_headers/gen/user_agent/safari.py
+-rw-r--r--   0        0        0        0 2023-06-15 05:49:50.361193 la-headers-0.0.2/la_headers/options/__init__.py
+-rw-r--r--   0        0        0      124 2023-06-15 05:49:37.313038 la-headers-0.0.2/la_headers/options/browser/__init__.py
+-rw-r--r--   0        0        0       38 2023-06-16 04:01:35.917611 la-headers-0.0.2/la_headers/options/browser/brave.py
+-rw-r--r--   0        0        0     4868 2023-06-15 15:22:42.391255 la-headers-0.0.2/la_headers/options/browser/chrome.py
+-rw-r--r--   0        0        0     7650 2023-06-15 15:22:54.663426 la-headers-0.0.2/la_headers/options/browser/firefox.py
+-rw-r--r--   0        0        0       72 2023-06-15 05:49:45.697138 la-headers-0.0.2/la_headers/options/operating_system/__init__.py
+-rw-r--r--   0        0        0      545 2023-06-14 13:33:02.345257 la-headers-0.0.2/la_headers/options/operating_system/android.py
+-rw-r--r--   0        0        0        0 2023-06-14 13:33:02.345257 la-headers-0.0.2/la_headers/options/operating_system/linux.py
+-rw-r--r--   0        0        0        0 2023-06-14 13:33:02.345257 la-headers-0.0.2/la_headers/options/operating_system/mac.py
+-rw-r--r--   0        0        0        0 2023-06-14 13:33:02.345257 la-headers-0.0.2/la_headers/options/operating_system/windows.py
+-rw-r--r--   0        0        0     1921 2023-06-16 04:04:39.980788 la-headers-0.0.2/la_headers/prefabs/__init__.py
+-rw-r--r--   0        0        0      420 2023-06-15 05:38:31.485260 la-headers-0.0.2/la_headers/utility.py
+-rw-r--r--   0        0        0      888 2023-06-16 04:58:00.917006 la-headers-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-14 13:33:02.349257 la-headers-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      390 2023-06-16 04:35:34.078853 la-headers-0.0.2/tests/test_random_headers.py
+-rw-r--r--   0        0        0      527 2023-06-15 05:40:31.778627 la-headers-0.0.2/tests/test_system.py
+-rw-r--r--   0        0        0      532 1970-01-01 00:00:00.000000 la-headers-0.0.2/PKG-INFO
```

### Comparing `la-headers-0.0.1/LICENSE` & `la-headers-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `la-headers-0.0.1/la_headers/__init__.py` & `la-headers-0.0.2/la_headers/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from random import choice
 
-from la_headers.accept import generate_accept
-from la_headers.accept_encondig import generate_accept_encoding
+from la_headers.gen.accept import generate_accept
+from la_headers.gen.accept_encondig import generate_accept_encoding
+from la_headers.gen.sec_ch_ua import generate_sec_ch_ua
+from la_headers.gen.sec_ch_ua_mobile import generate_sec_ch_ua_mobile
+from la_headers.gen.sec_ch_ua_platform import generate_sec_ch_ua_platform
+from la_headers.gen.system import generate_system
+from la_headers.gen.upgrade_insecure_requests import generate_upgrade_insecure_requests
+from la_headers.gen.user_agent import generate_user_agent
 from la_headers.prefabs import get_prefabs
-from la_headers.sec_ch_ua import generate_sec_ch_ua
-from la_headers.sec_ch_ua_mobile import generate_sec_ch_ua_mobile
-from la_headers.sec_ch_ua_platform import generate_sec_ch_ua_platform
-from la_headers.system import generate_system
-from la_headers.upgrade_insecure_requests import \
-    generate_upgrade_insecure_requests
-from la_headers.user_agent import generate_user_agent
 
 
 def generate_headers(
     os: str,
     os_version: str,
     browser: str,
     version: str,
     device: str = "desktop",
     context: str = "default",
 ) -> dict:
     """
     Generate a specific headers.
 
     os:
-        windows
-        linux
         android
+        linux
         mac
+        ubuntu
+        windows
 
     os_version:
         major.minor.patch
-    
+
     browser options:
         chrome
         firefox
 
     version:
         major.minor.patch
 
@@ -48,56 +48,56 @@
         image
         video
         audio
         script
         css
     """
 
-    system = generate_system(os, os_version)
+    system = generate_system(os, os_version, browser)
 
     headers = {
         "Accept": generate_accept(browser, version, context),
         "Accept-Encoding": generate_accept_encoding(browser, version),
         "Accept-Language": None,
         "Connection": None,
-        "Sec-Ch-Ua": generate_sec_ch_ua(browser, version),
+        "Sec-Ch-Ua": generate_sec_ch_ua(browser, version, os),
         "Sec-Ch-Ua-Mobile": generate_sec_ch_ua_mobile(browser, version, device),
         "Sec-Ch-Ua-Platform": generate_sec_ch_ua_platform(browser, version, os),
         "Upgrade-Insecure-Requests": generate_upgrade_insecure_requests(
             browser, version
         ),
         "User-Agent": generate_user_agent(browser, version, system, device),
     }
 
     # Remove fields with None
-    return {k:v for k, v in headers.items() if v is not None}
+    return {k: v for k, v in headers.items() if v is not None}
 
 
 def generate_random_headers(
     os: list[str] = [],
     os_version: list[str] = [],
     browser: list[str] = [],
     version: list[str] = [],
     device: list[str] = [],
     context: list[str] = [],
 ) -> dict:
     """
-    Generate a random headers.  
+    Generate a random headers.
     All paramaters are a list of possibilities but
     empty list means that you accept any possibility in the field.
 
     os:
         windows
         linux
         android
         mac
 
     os_version:
         major.minor.patch
-    
+
     browser options:
         chrome
         firefox
 
     version:
         major.minor.patch
 
@@ -123,9 +123,9 @@
         context=context,
     )
 
     prefab = choice(prefabs)
 
     for k in prefab:
         prefab[k] = choice(prefab[k])
-    
-    return generate_headers(**prefab)
+
+    return generate_headers(**prefab)
```

### Comparing `la-headers-0.0.1/la_headers/accept/__init__.py` & `la-headers-0.0.2/la_headers/gen/accept/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Accept
 # https://developer.mozilla.org/en-US/docs/Web/HTTP/Content_negotiation/List_of_default_Accept_values
 
 
-from la_headers.accept.chrome import CHROME_ACCEPT
-from la_headers.accept.firefox import FIREFOX_ACCEPT
+from la_headers.gen.accept.brave import BRAVE_ACCEPT
+from la_headers.gen.accept.chrome import CHROME_ACCEPT
+from la_headers.gen.accept.firefox import FIREFOX_ACCEPT
 from la_headers.utility import find_best_option
 
 _accept = {
+    "brave": BRAVE_ACCEPT,
     "chrome": CHROME_ACCEPT,
     "firefox": FIREFOX_ACCEPT,
 }
 
 
 def generate_accept(browser: str, version: str, context: str) -> str:
     context_options = _accept[browser][context]
```

### Comparing `la-headers-0.0.1/la_headers/accept/chrome.py` & `la-headers-0.0.2/la_headers/gen/accept/chrome.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # fmt: off
 CHROME_DEFAULT_ACCEPT = (
+    ("114.0", "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7"),
     ("97.0", "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9"),
     ("0.0", "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8"),
 )
 
 CHROME_IMAGE_ACCEPT = (
     ("97.0", "image/avif,image/webp,image/apng,image/svg+xml,image/*,*/*;q=0.8"),
     ("0.0", "image/avif,image/webp,image/apng,image/*,*/*;q=0.8"),
@@ -29,8 +30,8 @@
     "default": CHROME_DEFAULT_ACCEPT,
     "image": CHROME_IMAGE_ACCEPT,
     "video": CHROME_VIDEO_ACCEPT,
     "audio": CHROME_AUDIO_ACCEPT,
     "script": CHROME_SCRIPT_ACCEPT,
     "css": CHROME_CSS_ACCEPT,
 }
-# fmt: on
+# fmt: on
```

### Comparing `la-headers-0.0.1/la_headers/accept/firefox.py` & `la-headers-0.0.2/la_headers/gen/accept/firefox.py`

 * *Files identical despite different names*

### Comparing `la-headers-0.0.1/la_headers/accept_encondig/__init__.py` & `la-headers-0.0.2/la_headers/gen/accept_encondig/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Accept-Encoding
 # https://www.iana.org/assignments/http-parameters/http-parameters.xml#http-parameters-1
 
 
-from la_headers.accept_encondig.chrome import CHROME_ACCEPT_ENCODING
-from la_headers.accept_encondig.firefox import FIREFOX_ACCEPT_ENCODING
+from la_headers.gen.accept_encondig.brave import BRAVE_ACCEPT_ENCODING
+from la_headers.gen.accept_encondig.chrome import CHROME_ACCEPT_ENCODING
+from la_headers.gen.accept_encondig.firefox import FIREFOX_ACCEPT_ENCODING
 from la_headers.utility import find_best_option
 
 _accept_encoding = {
+    "brave": BRAVE_ACCEPT_ENCODING,
     "chrome": CHROME_ACCEPT_ENCODING,
     "firefox": FIREFOX_ACCEPT_ENCODING,
 }
 
 
 def generate_accept_encoding(browser: str, version: str) -> str:
     options = _accept_encoding[browser]
```

### Comparing `la-headers-0.0.1/la_headers/browser/chrome.py` & `la-headers-0.0.2/la_headers/options/browser/chrome.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 CHROME_VERSION = [
+    "114.0.0.0",
     "98.0.4758.66",
     "98.0.4758.54",
     "98.0.4758.48",
     "97.0.4692.99",
     "97.0.4692.98",
     "97.0.4692.87",
     "97.0.4692.84",
```

### Comparing `la-headers-0.0.1/la_headers/browser/firefox.py` & `la-headers-0.0.2/la_headers/options/browser/firefox.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 FIREFOX_VERSION = [
+    "114.0",
     "98.0a1",
     "97.0b6",
     "97.0b5",
     "97.0b4",
     "97.0b3",
     "97.0b2",
     "97.0b1",
```

### Comparing `la-headers-0.0.1/la_headers/operating_system/android.py` & `la-headers-0.0.2/la_headers/options/operating_system/android.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -40,8 +40,8 @@
     "2.1",
     "2.0.1",
     "2.0",
     "1.6",
     "1.5",
     "1.0",
     "1.0",
-)
+)
```

### Comparing `la-headers-0.0.1/la_headers/prefabs/__init__.py` & `la-headers-0.0.2/la_headers/prefabs/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from copy import deepcopy
 
-from la_headers.browser.chrome import CHROME_VERSION
-from la_headers.browser.firefox import FIREFOX_VERSION
-from la_headers.operating_system.android import ANDROID_VERSION
+from la_headers.options.browser.chrome import CHROME_VERSION
+from la_headers.options.browser.firefox import FIREFOX_VERSION
+from la_headers.options.operating_system.android import ANDROID_VERSION
 
 _prefabs: list[dict] = [
     {
         "os": ["linux"],
-        "os_version": ["22.04", "21.10", "21.04"],
+        "os_version": ["23.04", "22.10", "22.04"],
         "browser": ["chrome"],
         "version": CHROME_VERSION[:10],
         "device": ["desktop"],
         "context": ["default"],
     },
     {
         "os": ["linux"],
-        "os_version": ["22.04", "21.10", "21.04"],
+        "os_version": ["23.04", "22.10", "22.04"],
         "browser": ["firefox"],
         "version": FIREFOX_VERSION[:10],
         "device": ["desktop"],
         "context": ["default"],
     },
     {
         "os": ["windows"],
```

### Comparing `la-headers-0.0.1/la_headers/sec_ch_ua/__init__.py` & `la-headers-0.0.2/la_headers/gen/sec_ch_ua/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from packaging.version import Version
 
-from la_headers.sec_ch_ua.chromie import CHROME_SEC_CH_UA
-from la_headers.sec_ch_ua.firefox import FIREFOX_SEC_CH_UA
+from la_headers.gen.sec_ch_ua.brave import BRAVE_SEC_CH_UA
+from la_headers.gen.sec_ch_ua.chromie import CHROME_SEC_CH_UA
+from la_headers.gen.sec_ch_ua.firefox import FIREFOX_SEC_CH_UA
 from la_headers.utility import find_best_option
 
 _sec_ch_ua = {
+    "brave": BRAVE_SEC_CH_UA,
     "chrome": CHROME_SEC_CH_UA,
     "firefox": FIREFOX_SEC_CH_UA,
 }
 
 
-def generate_sec_ch_ua(browser: str, version: str) -> str:
-    options = _sec_ch_ua[browser]
+def generate_sec_ch_ua(browser: str, version: str, os: str) -> str:
+    options = _sec_ch_ua[browser][os]
     best_option = find_best_option(version, options)
 
     if best_option:
         major = Version(version).major
         best_option = best_option.format(major=major)
 
     return best_option
```

### Comparing `la-headers-0.0.1/la_headers/sec_ch_ua_platform/__init__.py` & `la-headers-0.0.2/la_headers/gen/sec_ch_ua_platform/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from packaging.version import Version
-
-from la_headers.sec_ch_ua_platform.chromie import CHROME_SEC_CH_UA_PLATFORM
-from la_headers.sec_ch_ua_platform.firefox import FIREFOX_SEC_CH_UA_PLATFORM
+from la_headers.gen.sec_ch_ua_platform.brave import BRAVE_SEC_CH_UA_PLATFORM
+from la_headers.gen.sec_ch_ua_platform.chromie import CHROME_SEC_CH_UA_PLATFORM
+from la_headers.gen.sec_ch_ua_platform.firefox import FIREFOX_SEC_CH_UA_PLATFORM
 from la_headers.utility import find_best_option
 
 _sec_ch_ua_platform = {
+    "brave": BRAVE_SEC_CH_UA_PLATFORM,
     "chrome": CHROME_SEC_CH_UA_PLATFORM,
     "firefox": FIREFOX_SEC_CH_UA_PLATFORM,
 }
 
 
 def generate_sec_ch_ua_platform(browser: str, version: str, os: str) -> str:
     options = _sec_ch_ua_platform[browser][os]
```

### Comparing `la-headers-0.0.1/pyproject.toml` & `la-headers-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "la-headers"
-version = "0.0.1"
+version = "0.0.2"
 description = "Headers generator"
 authors = [
     { name = "thiagola92", email = "thiagola92@gmail.com" },
 ]
 dependencies = [
     "packaging==21.3",
 ]
@@ -30,15 +30,19 @@
 [build-system]
 requires = [
     "pdm-pep517>=1.0.0",
 ]
 build-backend = "pdm.pep517.api"
 
 [tool.pdm.scripts]
-tests = "python -m unittest discover -v -f -s tests"
-sort = "python -m isort -v --ac ."
+unittest = "python -m unittest discover -v -f -s tests"
+black = "python -m black ."
+isort = "python -m isort -v --ac ."
 
 [tool.pdm.dev-dependencies]
 lint = [
     "black",
     "isort",
 ]
+
+[tool.isort]
+profile = "black"
```

### Comparing `la-headers-0.0.1/PKG-INFO` & `la-headers-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: la-headers
-Version: 0.0.1
+Version: 0.0.2
 Summary: Headers generator
 License: MIT
 Keywords: headers,request,browser
 Author-email: thiagola92 <thiagola92@gmail.com>
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,8 +12,9 @@
 Project-URL: Homepage, https://github.com/thiagola92/la-headers
 Description-Content-Type: text/markdown
 
 # la-headers
 A dumb headers generator.  
 
 # install
-`pip install git+https://github.com/thiagola92/la-headers.git`
+`pip install la-headers`
+
```

