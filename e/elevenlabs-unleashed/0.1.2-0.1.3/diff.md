# Comparing `tmp/elevenlabs_unleashed-0.1.2.tar.gz` & `tmp/elevenlabs_unleashed-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabs_unleashed-0.1.2.tar", last modified: Fri Jun 16 15:12:44 2023, max compression
+gzip compressed data, was "elevenlabs_unleashed-0.1.3.tar", last modified: Fri Jun 16 15:25:29 2023, max compression
```

## Comparing `elevenlabs_unleashed-0.1.2.tar` & `elevenlabs_unleashed-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 15:12:44.533032 elevenlabs_unleashed-0.1.2/
--rw-rw-rw-   0        0        0     1070 2023-06-16 15:10:34.000000 elevenlabs_unleashed-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     3044 2023-06-16 15:12:44.530024 elevenlabs_unleashed-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2479 2023-06-16 15:10:04.000000 elevenlabs_unleashed-0.1.2/README.md
--rw-rw-rw-   0        0        0      676 2023-06-16 15:12:04.000000 elevenlabs_unleashed-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-16 15:12:44.536048 elevenlabs_unleashed-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-16 15:12:44.378360 elevenlabs_unleashed-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-16 15:12:44.436035 elevenlabs_unleashed-0.1.2/src/elevenlabs_unleashed/
--rw-rw-rw-   0        0        0        0 2023-06-16 13:23:29.000000 elevenlabs_unleashed-0.1.2/src/elevenlabs_unleashed/__init__.py
--rw-rw-rw-   0        0        0     4756 2023-06-16 14:29:49.000000 elevenlabs_unleashed-0.1.2/src/elevenlabs_unleashed/account.py
--rw-rw-rw-   0        0        0     1453 2023-06-16 14:22:56.000000 elevenlabs_unleashed-0.1.2/src/elevenlabs_unleashed/manager.py
-drwxrwxrwx   0        0        0        0 2023-06-16 15:12:44.521024 elevenlabs_unleashed-0.1.2/src/elevenlabs_unleashed.egg-info/
--rw-rw-rw-   0        0        0     3044 2023-06-16 15:12:44.000000 elevenlabs_unleashed-0.1.2/src/elevenlabs_unleashed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-06-16 15:12:44.000000 elevenlabs_unleashed-0.1.2/src/elevenlabs_unleashed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 15:12:44.000000 elevenlabs_unleashed-0.1.2/src/elevenlabs_unleashed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-16 15:12:44.000000 elevenlabs_unleashed-0.1.2/src/elevenlabs_unleashed.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 15:25:29.755212 elevenlabs_unleashed-0.1.3/
+-rw-rw-rw-   0        0        0     1070 2023-06-16 15:10:34.000000 elevenlabs_unleashed-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     3044 2023-06-16 15:25:29.740142 elevenlabs_unleashed-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2479 2023-06-16 15:10:04.000000 elevenlabs_unleashed-0.1.3/README.md
+-rw-rw-rw-   0        0        0      676 2023-06-16 15:24:08.000000 elevenlabs_unleashed-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-16 15:25:29.763140 elevenlabs_unleashed-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 15:25:29.423041 elevenlabs_unleashed-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-16 15:25:29.594077 elevenlabs_unleashed-0.1.3/src/elevenlabs_unleashed/
+-rw-rw-rw-   0        0        0        0 2023-06-16 13:23:29.000000 elevenlabs_unleashed-0.1.3/src/elevenlabs_unleashed/__init__.py
+-rw-rw-rw-   0        0        0     4760 2023-06-16 15:23:03.000000 elevenlabs_unleashed-0.1.3/src/elevenlabs_unleashed/account.py
+-rw-rw-rw-   0        0        0     1453 2023-06-16 14:22:56.000000 elevenlabs_unleashed-0.1.3/src/elevenlabs_unleashed/manager.py
+drwxrwxrwx   0        0        0        0 2023-06-16 15:25:29.734823 elevenlabs_unleashed-0.1.3/src/elevenlabs_unleashed.egg-info/
+-rw-rw-rw-   0        0        0     3044 2023-06-16 15:25:29.000000 elevenlabs_unleashed-0.1.3/src/elevenlabs_unleashed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-06-16 15:25:29.000000 elevenlabs_unleashed-0.1.3/src/elevenlabs_unleashed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 15:25:29.000000 elevenlabs_unleashed-0.1.3/src/elevenlabs_unleashed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-16 15:25:29.000000 elevenlabs_unleashed-0.1.3/src/elevenlabs_unleashed.egg-info/top_level.txt
```

### Comparing `elevenlabs_unleashed-0.1.2/LICENSE` & `elevenlabs_unleashed-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `elevenlabs_unleashed-0.1.2/PKG-INFO` & `elevenlabs_unleashed-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabs_unleashed
-Version: 0.1.2
+Version: 0.1.3
 Summary: Unlimited access to Elevenlabs API
 Author-email: GaspardCulis <gasdev.lp@gmail.com>
 Project-URL: Homepage, https://github.com/GaspardCulis/elevenlabs-unleashed
 Project-URL: Bug Tracker, https://github.com/GaspardCulis/elevenlabs-unleashed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `elevenlabs_unleashed-0.1.2/README.md` & `elevenlabs_unleashed-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `elevenlabs_unleashed-0.1.2/pyproject.toml` & `elevenlabs_unleashed-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "elevenlabs_unleashed"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="GaspardCulis", email="gasdev.lp@gmail.com" },
 ]
 description = "Unlimited access to Elevenlabs API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `elevenlabs_unleashed-0.1.2/src/elevenlabs_unleashed/account.py` & `elevenlabs_unleashed-0.1.3/src/elevenlabs_unleashed/account.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,16 +77,16 @@
     driver = webdriver.Chrome(options=options)
 
     driver.get(SIGNUP_URL)
 
     email = _generate_email()
     password = _generate_password()
 
-    cookie_button = WebDriverWait(driver, 10).until(lambda driver: driver.find_element(By.ID, "CybotCookiebotDialogBodyButtonAccept"))
-    cookie_button.click()
+    # cookie_button = WebDriverWait(driver, 10).until(lambda driver: driver.find_element(By.ID, "CybotCookiebotDialogBodyButtonAccept"))
+    # cookie_button.click()
 
     email_input = WebDriverWait(driver, 10).until(lambda driver: driver.find_element(By.NAME, "email"))
     email_input.send_keys(email)
 
     password_input = driver.find_element(By.NAME, "password")
     password_input.send_keys(password)
```

### Comparing `elevenlabs_unleashed-0.1.2/src/elevenlabs_unleashed/manager.py` & `elevenlabs_unleashed-0.1.3/src/elevenlabs_unleashed/manager.py`

 * *Files identical despite different names*

### Comparing `elevenlabs_unleashed-0.1.2/src/elevenlabs_unleashed.egg-info/PKG-INFO` & `elevenlabs_unleashed-0.1.3/src/elevenlabs_unleashed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabs-unleashed
-Version: 0.1.2
+Version: 0.1.3
 Summary: Unlimited access to Elevenlabs API
 Author-email: GaspardCulis <gasdev.lp@gmail.com>
 Project-URL: Homepage, https://github.com/GaspardCulis/elevenlabs-unleashed
 Project-URL: Bug Tracker, https://github.com/GaspardCulis/elevenlabs-unleashed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

