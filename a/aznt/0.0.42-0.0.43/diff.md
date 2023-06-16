# Comparing `tmp/aznt-0.0.42.tar.gz` & `tmp/aznt-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aznt-0.0.42.tar", last modified: Wed Jun 14 07:49:58 2023, max compression
+gzip compressed data, was "aznt-0.0.43.tar", last modified: Fri Jun 16 08:21:20 2023, max compression
```

## Comparing `aznt-0.0.42.tar` & `aznt-0.0.43.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 07:49:58.451474 aznt-0.0.42/
--rw-rw-rw-   0        0        0     1090 2023-01-31 07:03:04.000000 aznt-0.0.42/LICENCE.txt
--rw-rw-rw-   0        0        0       76 2023-03-22 18:32:20.000000 aznt-0.0.42/MANIFEST.in
--rw-rw-rw-   0        0        0    17530 2023-06-14 07:49:58.451474 aznt-0.0.42/PKG-INFO
--rw-rw-rw-   0        0        0    16451 2023-06-14 07:46:49.000000 aznt-0.0.42/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 07:49:58.420199 aznt-0.0.42/aznt/
--rw-rw-rw-   0        0        0        1 2023-01-31 07:04:46.000000 aznt-0.0.42/aznt/__init__.py
--rw-rw-rw-   0        0        0     9463 2023-06-14 07:27:03.000000 aznt-0.0.42/aznt/azntnumbers.py
--rw-rw-rw-   0        0        0     3360 2023-03-21 16:09:46.000000 aznt-0.0.42/aznt/azntplots.py
--rw-rw-rw-   0        0        0     1180 2023-03-21 16:09:56.000000 aznt-0.0.42/aznt/azntprimality.py
-drwxrwxrwx   0        0        0        0 2023-06-14 07:49:58.451474 aznt-0.0.42/aznt.egg-info/
--rw-rw-rw-   0        0        0    17530 2023-06-14 07:49:58.000000 aznt-0.0.42/aznt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-06-14 07:49:58.000000 aznt-0.0.42/aznt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 07:49:58.000000 aznt-0.0.42/aznt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-14 07:49:58.000000 aznt-0.0.42/aznt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-14 07:49:58.000000 aznt-0.0.42/aznt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1119 2023-06-14 07:49:27.000000 aznt-0.0.42/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 07:49:58.451474 aznt-0.0.42/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-16 08:21:20.900669 aznt-0.0.43/
+-rw-rw-rw-   0        0        0     1090 2023-06-14 06:07:32.000000 aznt-0.0.43/LICENCE.txt
+-rw-rw-rw-   0        0        0       76 2023-06-14 06:07:32.000000 aznt-0.0.43/MANIFEST.in
+-rw-rw-rw-   0        0        0    18044 2023-06-16 08:21:20.900669 aznt-0.0.43/PKG-INFO
+-rw-rw-rw-   0        0        0    16965 2023-06-16 08:20:34.000000 aznt-0.0.43/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 08:21:20.885049 aznt-0.0.43/aznt/
+-rw-rw-rw-   0        0        0        1 2023-06-14 06:07:34.000000 aznt-0.0.43/aznt/__init__.py
+-rw-rw-rw-   0        0        0     9463 2023-06-14 06:07:34.000000 aznt-0.0.43/aznt/azntnumbers.py
+-rw-rw-rw-   0        0        0     3360 2023-06-14 06:07:34.000000 aznt-0.0.43/aznt/azntplots.py
+-rw-rw-rw-   0        0        0     1765 2023-06-16 08:14:00.000000 aznt-0.0.43/aznt/azntprimality.py
+drwxrwxrwx   0        0        0        0 2023-06-16 08:21:20.900669 aznt-0.0.43/aznt.egg-info/
+-rw-rw-rw-   0        0        0    18044 2023-06-16 08:21:20.000000 aznt-0.0.43/aznt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-06-16 08:21:20.000000 aznt-0.0.43/aznt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 08:21:20.000000 aznt-0.0.43/aznt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-16 08:21:20.000000 aznt-0.0.43/aznt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-16 08:21:20.000000 aznt-0.0.43/aznt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1119 2023-06-16 08:20:41.000000 aznt-0.0.43/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-16 08:21:20.900669 aznt-0.0.43/setup.cfg
```

### Comparing `aznt-0.0.42/LICENCE.txt` & `aznt-0.0.43/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `aznt-0.0.42/PKG-INFO` & `aznt-0.0.43/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aznt
-Version: 0.0.42
+Version: 0.0.43
 Summary: From A to Z Number Theory
 Author-email: "Adrian Zapała, MSc" <adrian.zapala@outlook.com>
 Keywords: aznt,numbers,number theory,primes,prime numbers,math
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
@@ -19,15 +19,15 @@
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 ![Python Version](https://img.shields.io/badge/python-3.11-blue/)
-![aznt version](https://img.shields.io/badge/aznt-0.0.42-green)
+![aznt version](https://img.shields.io/badge/aznt-0.0.43-green)
 ![Beta version](https://img.shields.io/badge/beta-ver.-green)
 
 # `aznt` - From A to Z Number Theory
 
 * Number Theory library for Python with prime numbers.
 * **Important:** requires Python >= 3.11.
 * You can pass to author's GitHub at
@@ -506,14 +506,27 @@
 Time complexity: `O(n log n)`.<br>
 **<span style="color: coral">Examples</span>**
 ```python
 >>> eratosthenes_sieve(100)
 [2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47, 53, 59, 61, 67, 71, 73, 79, 83, 89, 97]
 ```
 
+## `is_probably_prime(n)`
+Fermat's Little Theorem to check if number is a probable prime. If so, return string and boolean `True` value, `False` otherwise. So it's recommended to check for a given number multiple times in a loop. <br>
+Time complexity: `O(1)`.<br>
+**<span style="color: coral">Examples</span>**
+```python
+>>> is_probably_prime(5)
+5: probably prime
+>>> is_probably_prime(561)
+561: not prime
+>>> is_probably_prime(561)
+561: probably prime  # False result, 561 is a composite number
+```
+
 # Usage: `azntplots` module functions
 
 ## `critical_strip()`
 
 Return a plot presenting critical strip and critical line of Riemann zeta.<br>
 
 ## `riemann_zeta()`
```

### Comparing `aznt-0.0.42/README.md` & `aznt-0.0.43/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ![Python Version](https://img.shields.io/badge/python-3.11-blue/)
-![aznt version](https://img.shields.io/badge/aznt-0.0.42-green)
+![aznt version](https://img.shields.io/badge/aznt-0.0.43-green)
 ![Beta version](https://img.shields.io/badge/beta-ver.-green)
 
 # `aznt` - From A to Z Number Theory
 
 * Number Theory library for Python with prime numbers.
 * **Important:** requires Python >= 3.11.
 * You can pass to author's GitHub at
@@ -482,14 +482,27 @@
 Time complexity: `O(n log n)`.<br>
 **<span style="color: coral">Examples</span>**
 ```python
 >>> eratosthenes_sieve(100)
 [2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47, 53, 59, 61, 67, 71, 73, 79, 83, 89, 97]
 ```
 
+## `is_probably_prime(n)`
+Fermat's Little Theorem to check if number is a probable prime. If so, return string and boolean `True` value, `False` otherwise. So it's recommended to check for a given number multiple times in a loop. <br>
+Time complexity: `O(1)`.<br>
+**<span style="color: coral">Examples</span>**
+```python
+>>> is_probably_prime(5)
+5: probably prime
+>>> is_probably_prime(561)
+561: not prime
+>>> is_probably_prime(561)
+561: probably prime  # False result, 561 is a composite number
+```
+
 # Usage: `azntplots` module functions
 
 ## `critical_strip()`
 
 Return a plot presenting critical strip and critical line of Riemann zeta.<br>
 
 ## `riemann_zeta()`
```

### Comparing `aznt-0.0.42/aznt/azntnumbers.py` & `aznt-0.0.43/aznt/azntnumbers.py`

 * *Files identical despite different names*

### Comparing `aznt-0.0.42/aznt/azntplots.py` & `aznt-0.0.43/aznt/azntplots.py`

 * *Files identical despite different names*

### Comparing `aznt-0.0.42/aznt/azntprimality.py` & `aznt-0.0.43/aznt/azntprimality.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """
 aznt - From A to Z Number Theory
 Author: Adrian Zapała, Msc, adrian.zapala@outlook.com, All rights reserved
 Licence: MIT
 """
 
+from random import randint
+from azntnumbers import gcd_mod
+
 
 def is_prime_naive1(n):
     if n <= 1:
         return False
     for i in range(2, n):
         if n % i == 0:
             return False
@@ -38,18 +41,40 @@
     if n <= 1 or n % 2 == 0:
         return False
     for i in range(3, int(n ** 0.5) + 1, 2):
         if n % i == 0:
             return False
     return True
 
+
 def eratosthenes_sieve(n):
     nums = [True if i >= 2 else False for i in range(n + 1)]
 
     for i in range(2, int(n ** 0.5) + 1):
         j = i
         while j <= n:
             if j > i:
                 nums[j] = False
             j += i
 
     return [i for i in range(len(nums)) if nums[i]]
+
+
+def is_probably_prime(p):
+    """Fermat's Little Theorem to check if number is a prime"""
+    a = 1 if p < 5 else randint(2, p - 2)
+    if gcd_mod(a, p) == 1:
+        if (a ** (p - 1) - 1) % p == 0:
+            print(f"{p}: probably prime")
+            return True
+
+    print(f"{p}: not prime")
+    return False
+
+
+if __name__ == "__main__":
+    is_probably_prime(2)
+    is_probably_prime(3)
+    is_probably_prime(5)
+    is_probably_prime(101)
+    is_probably_prime(552)
+    is_probably_prime(561)
```

### Comparing `aznt-0.0.42/aznt.egg-info/PKG-INFO` & `aznt-0.0.43/aznt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aznt
-Version: 0.0.42
+Version: 0.0.43
 Summary: From A to Z Number Theory
 Author-email: "Adrian Zapała, MSc" <adrian.zapala@outlook.com>
 Keywords: aznt,numbers,number theory,primes,prime numbers,math
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
@@ -19,15 +19,15 @@
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 ![Python Version](https://img.shields.io/badge/python-3.11-blue/)
-![aznt version](https://img.shields.io/badge/aznt-0.0.42-green)
+![aznt version](https://img.shields.io/badge/aznt-0.0.43-green)
 ![Beta version](https://img.shields.io/badge/beta-ver.-green)
 
 # `aznt` - From A to Z Number Theory
 
 * Number Theory library for Python with prime numbers.
 * **Important:** requires Python >= 3.11.
 * You can pass to author's GitHub at
@@ -506,14 +506,27 @@
 Time complexity: `O(n log n)`.<br>
 **<span style="color: coral">Examples</span>**
 ```python
 >>> eratosthenes_sieve(100)
 [2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47, 53, 59, 61, 67, 71, 73, 79, 83, 89, 97]
 ```
 
+## `is_probably_prime(n)`
+Fermat's Little Theorem to check if number is a probable prime. If so, return string and boolean `True` value, `False` otherwise. So it's recommended to check for a given number multiple times in a loop. <br>
+Time complexity: `O(1)`.<br>
+**<span style="color: coral">Examples</span>**
+```python
+>>> is_probably_prime(5)
+5: probably prime
+>>> is_probably_prime(561)
+561: not prime
+>>> is_probably_prime(561)
+561: probably prime  # False result, 561 is a composite number
+```
+
 # Usage: `azntplots` module functions
 
 ## `critical_strip()`
 
 Return a plot presenting critical strip and critical line of Riemann zeta.<br>
 
 ## `riemann_zeta()`
```

### Comparing `aznt-0.0.42/pyproject.toml` & `aznt-0.0.43/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aznt"
-version = "0.0.42"
+version = "0.0.43"
 description = "From A to Z Number Theory"
 keywords = ["aznt", "numbers", "number theory", "primes", "prime numbers", "math"]
 authors = [
     {name = "Adrian Zapała, MSc", email = "adrian.zapala@outlook.com"},
 ]
 license = {file = "LICENSE.txt"}
 readme = "README.md"
```

