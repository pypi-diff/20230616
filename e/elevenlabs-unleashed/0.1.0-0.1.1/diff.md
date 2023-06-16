# Comparing `tmp/elevenlabs_unleashed-0.1.0.tar.gz` & `tmp/elevenlabs_unleashed-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "elevenlabs_unleashed-0.1.1.tar", last modified: Fri Jun 16 15:08:19 2023, max compression
```

## Comparing `elevenlabs_unleashed-0.1.0.tar` & `elevenlabs_unleashed-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,15 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 elevenlabs_unleashed-0.1.0/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elevenlabs_unleashed-0.1.0/src/elevenlabsunleashed/__init__.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 elevenlabs_unleashed-0.1.0/src/elevenlabsunleashed/account_generator.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 elevenlabs_unleashed-0.1.0/src/elevenlabsunleashed/manager.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 elevenlabs_unleashed-0.1.0/.gitignore
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 elevenlabs_unleashed-0.1.0/README.md
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 elevenlabs_unleashed-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 elevenlabs_unleashed-0.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-16 15:08:19.079715 elevenlabs_unleashed-0.1.1/
+-rw-rw-rw-   0        0        0     3056 2023-06-16 15:08:19.070703 elevenlabs_unleashed-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2514 2023-06-16 14:54:04.000000 elevenlabs_unleashed-0.1.1/README.md
+-rw-rw-rw-   0        0        0      676 2023-06-16 13:33:47.000000 elevenlabs_unleashed-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-16 15:08:19.082687 elevenlabs_unleashed-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 15:08:18.928610 elevenlabs_unleashed-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-16 15:08:18.958693 elevenlabs_unleashed-0.1.1/src/elevenlabs_unleashed/
+-rw-rw-rw-   0        0        0        0 2023-06-16 13:23:29.000000 elevenlabs_unleashed-0.1.1/src/elevenlabs_unleashed/__init__.py
+-rw-rw-rw-   0        0        0     4756 2023-06-16 14:29:49.000000 elevenlabs_unleashed-0.1.1/src/elevenlabs_unleashed/account.py
+-rw-rw-rw-   0        0        0     1453 2023-06-16 14:22:56.000000 elevenlabs_unleashed-0.1.1/src/elevenlabs_unleashed/manager.py
+drwxrwxrwx   0        0        0        0 2023-06-16 15:08:19.058685 elevenlabs_unleashed-0.1.1/src/elevenlabs_unleashed.egg-info/
+-rw-rw-rw-   0        0        0     3056 2023-06-16 15:08:18.000000 elevenlabs_unleashed-0.1.1/src/elevenlabs_unleashed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-06-16 15:08:18.000000 elevenlabs_unleashed-0.1.1/src/elevenlabs_unleashed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 15:08:18.000000 elevenlabs_unleashed-0.1.1/src/elevenlabs_unleashed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-16 15:08:18.000000 elevenlabs_unleashed-0.1.1/src/elevenlabs_unleashed.egg-info/top_level.txt
```

### Comparing `elevenlabs_unleashed-0.1.0/src/elevenlabsunleashed/account_generator.py` & `elevenlabs_unleashed-0.1.1/src/elevenlabs_unleashed/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,13 +120,16 @@
     account_button = WebDriverWait(driver, 10).until(lambda driver: driver.find_element(By.XPATH, "//button[@data-testid='user-menu-button']"))
     account_button.click()
 
     profile_button = WebDriverWait(driver, 10).until(lambda driver: driver.find_element(By.XPATH, "//a[starts-with(@id, 'headlessui-menu-item')]"))
     profile_button.click()
     
     api_key_input = WebDriverWait(driver, 10).until(lambda driver: driver.find_element(By.XPATH, "//input[@type='password']"))
-    sleep(0.5)
-    api_key = api_key_input.get_attribute("value")
+    
+    api_key = ''
+    while api_key == '':
+        api_key = api_key_input.get_attribute("value")
+        sleep(0.1)
 
     driver.quit()
 
     return email, password, api_key
```

### Comparing `elevenlabs_unleashed-0.1.0/src/elevenlabsunleashed/manager.py` & `elevenlabs_unleashed-0.1.1/src/elevenlabs_unleashed/manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 import threading
-from account_generator import create_account
+from elevenlabs_unleashed.account import create_account
 from typing import Callable, Tuple
 
 class ELUAccountManager():
     def __init__(self, set_api_key_callback: Callable[[str], None], nb_accounts: int = 2):
-        self.api_key_callback = set_api_key_callback
-        self.nb_accounts = nb_accounts
+        self.__api_key_callback = set_api_key_callback
+        self.__nb_accounts = nb_accounts
         self.accounts = []
-        self.threads = []
-        self.daemon = True
+        self.__threads = []
 
-    def _create_account(self):
+    def __create_account(self):
         self.accounts.append(create_account())
 
-    def _create_accounts_async(self):
-        self.threads = []
-        for i in range(self.nb_accounts - len(self.accounts)):
-            thread = threading.Thread(target=self._create_account)
+    def __create_accounts_async(self):
+        self.__threads = []
+        for i in range(self.__nb_accounts - len(self.accounts)):
+            thread = threading.Thread(target=self.__create_account)
             thread.start()
-            self.threads.append(thread)
+            self.__threads.append(thread)
 
     def next(self) -> Tuple[str, str, str]:
         """
         Takes the next account from the list and returns the email, password and api key, creating new accounts if needed.
         This function is thread-blocking if no account is available, until a new account is created
         """
         if len(self.accounts) == 0:
-            if len(self.threads) == 0:
-                self._create_accounts_async()
-            for thread in self.threads:
+            if len(self.__threads) == 0:
+                self.__create_accounts_async()
+            for thread in self.__threads:
                 thread.join()
-            self.threads = []
+            self.__threads = []
         account = self.accounts.pop()
-        self.api_key_callback(account['api_key'])
-        self._create_accounts_async()
-        return account['email'], account['password'], account['api_key']
+        self.__api_key_callback(account[2])
+        self.__create_accounts_async()
+        return account[0], account[1], account[2]
```

### Comparing `elevenlabs_unleashed-0.1.0/pyproject.toml` & `elevenlabs_unleashed-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
-name = "elevenlabs-unleashed"
-version = "0.1.0"
+name = "elevenlabs_unleashed"
+version = "0.1.1"
 authors = [
   { name="GaspardCulis", email="gasdev.lp@gmail.com" },
 ]
 description = "Unlimited access to Elevenlabs API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -14,12 +14,12 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/GaspardCulis/elevenlabs-unleashed"
 "Bug Tracker" = "https://github.com/GaspardCulis/elevenlabs-unleashed/issues"
 
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[options]
-packages = "find:"
+requires = [
+    "setuptools >= 65",
+    "wheel >= 0.38",
+]
+build-backend = "setuptools.build_meta"
```

