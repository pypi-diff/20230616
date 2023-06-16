# Comparing `tmp/decoratory-0.1.0.3.tar.gz` & `tmp/decoratory-0.1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoratory-0.1.0.3.tar", last modified: Thu Jun 15 16:36:26 2023, max compression
+gzip compressed data, was "decoratory-0.1.1.3.tar", last modified: Fri Jun 16 18:02:15 2023, max compression
```

## Comparing `decoratory-0.1.0.3.tar` & `decoratory-0.1.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 16:36:26.159623 decoratory-0.1.0.3/
--rw-rw-rw-   0        0        0     2550 2023-06-02 20:50:35.000000 decoratory-0.1.0.3/License.txt
--rw-rw-rw-   0        0        0    22392 2023-06-15 16:36:26.159623 decoratory-0.1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    20767 2023-06-15 16:35:28.000000 decoratory-0.1.0.3/Readme.rst
--rw-rw-rw-   0        0        0        0 2023-06-10 04:00:34.000000 decoratory-0.1.0.3/Requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-15 16:36:26.112747 decoratory-0.1.0.3/Sources/
-drwxrwxrwx   0        0        0        0 2023-06-15 16:36:26.143999 decoratory-0.1.0.3/Sources/decoratory/
--rw-rw-rw-   0        0        0      249 2023-06-07 18:32:49.000000 decoratory-0.1.0.3/Sources/decoratory/__init__.py
--rw-rw-rw-   0        0        0     4621 2023-06-15 16:35:51.000000 decoratory-0.1.0.3/Sources/decoratory/__main__.py
--rw-rw-rw-   0        0        0     4855 2023-06-13 16:03:52.000000 decoratory-0.1.0.3/Sources/decoratory/banner.py
--rw-rw-rw-   0        0        0    14152 2023-06-14 15:11:14.000000 decoratory-0.1.0.3/Sources/decoratory/basic.py
--rw-rw-rw-   0        0        0    15763 2023-06-15 16:24:13.000000 decoratory-0.1.0.3/Sources/decoratory/multiton.py
--rw-rw-rw-   0        0        0    38553 2023-06-12 12:49:52.000000 decoratory-0.1.0.3/Sources/decoratory/observer.py
--rw-rw-rw-   0        0        0     9089 2023-06-15 16:24:13.000000 decoratory-0.1.0.3/Sources/decoratory/singleton.py
--rw-rw-rw-   0        0        0    13845 2023-06-15 16:24:13.000000 decoratory-0.1.0.3/Sources/decoratory/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-15 16:36:26.143999 decoratory-0.1.0.3/Sources/decoratory.egg-info/
--rw-rw-rw-   0        0        0    22392 2023-06-15 16:36:26.000000 decoratory-0.1.0.3/Sources/decoratory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-06-15 16:36:26.000000 decoratory-0.1.0.3/Sources/decoratory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 16:36:26.000000 decoratory-0.1.0.3/Sources/decoratory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-15 16:36:26.000000 decoratory-0.1.0.3/Sources/decoratory.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-15 16:36:26.159623 decoratory-0.1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     4017 2023-06-15 16:35:51.000000 decoratory-0.1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:02:15.974894 decoratory-0.1.1.3/
+-rw-rw-rw-   0        0        0     2550 2023-06-02 20:50:35.000000 decoratory-0.1.1.3/License.txt
+-rw-rw-rw-   0        0        0    39099 2023-06-16 18:02:15.974894 decoratory-0.1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    37474 2023-06-16 17:55:52.000000 decoratory-0.1.1.3/Readme.rst
+-rw-rw-rw-   0        0        0        0 2023-06-10 04:00:34.000000 decoratory-0.1.1.3/Requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 18:02:15.924897 decoratory-0.1.1.3/Sources/
+drwxrwxrwx   0        0        0        0 2023-06-16 18:02:15.964893 decoratory-0.1.1.3/Sources/decoratory/
+-rw-rw-rw-   0        0        0      249 2023-06-07 18:32:49.000000 decoratory-0.1.1.3/Sources/decoratory/__init__.py
+-rw-rw-rw-   0        0        0     4621 2023-06-16 18:01:41.000000 decoratory-0.1.1.3/Sources/decoratory/__main__.py
+-rw-rw-rw-   0        0        0     4855 2023-06-16 07:40:57.000000 decoratory-0.1.1.3/Sources/decoratory/banner.py
+-rw-rw-rw-   0        0        0    14152 2023-06-16 07:40:57.000000 decoratory-0.1.1.3/Sources/decoratory/basic.py
+-rw-rw-rw-   0        0        0    16033 2023-06-16 07:40:57.000000 decoratory-0.1.1.3/Sources/decoratory/multiton.py
+-rw-rw-rw-   0        0        0    40070 2023-06-16 17:56:14.000000 decoratory-0.1.1.3/Sources/decoratory/observer.py
+-rw-rw-rw-   0        0        0     9128 2023-06-16 07:40:57.000000 decoratory-0.1.1.3/Sources/decoratory/singleton.py
+-rw-rw-rw-   0        0        0    13933 2023-06-16 07:40:57.000000 decoratory-0.1.1.3/Sources/decoratory/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-06-16 18:02:15.964893 decoratory-0.1.1.3/Sources/decoratory.egg-info/
+-rw-rw-rw-   0        0        0    39099 2023-06-16 18:02:15.000000 decoratory-0.1.1.3/Sources/decoratory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      459 2023-06-16 18:02:15.000000 decoratory-0.1.1.3/Sources/decoratory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 18:02:15.000000 decoratory-0.1.1.3/Sources/decoratory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-16 18:02:15.000000 decoratory-0.1.1.3/Sources/decoratory.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-16 18:02:15.974894 decoratory-0.1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     4017 2023-06-16 18:01:41.000000 decoratory-0.1.1.3/setup.py
```

### Comparing `decoratory-0.1.0.3/License.txt` & `decoratory-0.1.1.3/License.txt`

 * *Files identical despite different names*

### Comparing `decoratory-0.1.0.3/Sources/decoratory/__main__.py` & `decoratory-0.1.1.3/Sources/decoratory/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.0.3"
-__date__ = "2023-06-15"
-__time__ = "18:35:51"
+__version__ = "0.1.1.3"
+__date__ = "2023-06-16"
+__time__ = "20:01:41"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = []
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.1.0.3/Sources/decoratory/banner.py` & `decoratory-0.1.1.3/Sources/decoratory/banner.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.0.3"
-__date__ = "2023-06-13"
-__time__ = "18:03:50"
+__version__ = "0.1.1.1"
+__date__ = "2023-06-16"
+__time__ = "09:40:57"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["__banner"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.1.0.3/Sources/decoratory/basic.py` & `decoratory-0.1.1.3/Sources/decoratory/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,17 +37,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.0.3"
-__date__ = "2023-06-14"
-__time__ = "17:11:10"
+__version__ = "0.1.1.1"
+__date__ = "2023-06-16"
+__time__ = "09:40:57"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Activation", "Parser", "F", "X"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
```

### Comparing `decoratory-0.1.0.3/Sources/decoratory/multiton.py` & `decoratory-0.1.1.3/Sources/decoratory/multiton.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     unseal(self):
         Unseal multiton.
 
     issealed(self):
         Multiton sealing state
 
     get_instance():
-        Return the singleton instantce. (if accessible=True)
+        Return the singleton instance.  (if accessible=True)
 
     reset():
         Resets the singleton instance.  (if resettable=True)
 
     Example
     -------
 
@@ -43,103 +43,103 @@
             self.spec = spec
             self.name = name
 
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.spec}', '{self.name}')"
 
     # Create instances
-    a = Animal('dog', name='Bello')
-    b = Animal('cat', name='Mausi')
-    c = Animal('dog', name='Tessa')
+    a = Animal('dog', name='Teddy')
+    b = Animal('cat', name='Molly')
+    c = Animal('dog', name='Roxie')
 
     # Case 0: decoration @Multiton or @Multiton() or @Multiton(key=17) or ...
     #    ---> With no or fixed key the Multiton acts like a Singleton
-    print(a)                        # Animal('dog', 'Bello')
-    print(b)                        # Animal('dog', 'Bello')
-    print(c)                        # Animal('dog', 'Bello')
+    print(a)                        # Animal('dog', 'Teddy')
+    print(b)                        # Animal('dog', 'Teddy')
+    print(c)                        # Animal('dog', 'Teddy')
 
     # Case 1: decoration @Multiton(key=lambda spec, name: name)
     #    ---> key is a function evaluating the attribute name from __init__(..)
-    print(a)                        # Animal('dog', 'Bello')
-    print(b)                        # Animal('cat', 'Mausi')
-    print(c)                        # Animal('dog', 'Tessa')
+    print(a)                        # Animal('dog', 'Teddy')
+    print(b)                        # Animal('cat', 'Molly')
+    print(c)                        # Animal('dog', 'Roxie')
 
     # Case 2: decoration @Multiton(key=lambda spec, name: 'a' in name)
     #    ---> key is a function evaluating the attribute name from __init__(..)
-    print(a)                        # Animal('dog', 'Bello')
-    print(b)                        # Animal('cat', 'Mausi')
-    print(c)                        # Animal('cat', 'Mausi')
+    print(a)                        # Animal('dog', 'Teddy')
+    print(b)                        # Animal('cat', 'Molly')
+    print(c)                        # Animal('cat', 'Molly')
 
     # Case 3: decoration @Multiton(key="{0}".format)
     #    ---> Parameter spec is referenced as args[0] (positional)
-    print(a)                        # Animal('dog', 'Bello')
-    print(b)                        # Animal('cat', 'Mausi')
-    print(c)                        # Animal('dog', 'Bello')
+    print(a)                        # Animal('dog', 'Teddy')
+    print(b)                        # Animal('cat', 'Molly')
+    print(c)                        # Animal('dog', 'Teddy')
 
     # Case 4: decoration @Multiton(key="{name}".format)
     #    ---> Parameter name is referenced as kwargs['name'] (keyword)
-    print(a)                        # Animal('dog', 'Bello')
-    print(b)                        # Animal('cat', 'Mausi')
-    print(c)                        # Animal('dog', 'Tessa')
+    print(a)                        # Animal('dog', 'Teddy')
+    print(b)                        # Animal('cat', 'Molly')
+    print(c)                        # Animal('dog', 'Roxie')
 
     # Case 5: decoration @Multiton(key=lambda spec, name: (spec, name))
     #    ---> One unique instance for all init values, i.e. no duplicates
-    print(a)                        # Animal('dog', 'Bello')
-    print(b)                        # Animal('cat', 'Mausi')
-    print(c)                        # Animal('dog', 'Tessa')
+    print(a)                        # Animal('dog', 'Teddy')
+    print(b)                        # Animal('cat', 'Molly')
+    print(c)                        # Animal('dog', 'Roxie')
 
     # Case 6: decoration @Multiton(key=F("my_key"))
     #    ---> Late binding with F(classmethod_string)
     #         One unique instance from a @staticmethod or @classmethod
     class Animal:
         ...
         @classmethod
         def my_key(cls, spec, name):
             return 'a' in name
-    print(a)                        # Animal('dog', 'Bello')
-    print(b)                        # Animal('cat', 'Mausi')
-    print(c)                        # Animal('cat', 'Mausi')
+    print(a)                        # Animal('dog', 'Teddy')
+    print(b)                        # Animal('cat', 'Molly')
+    print(c)                        # Animal('cat', 'Molly')
 
     # Case 7: decoration @Multiton(key=lambda spec, name: name,
     #                              accessible=True, resettable=True)
-    #    ---> Seal after Bello
+    #    ---> Seal after Teddy
     Animal.reset()                  # Reset/Clear the instance dictionary
     print(Animal.get_instances())   # {}
     print(Animal.issealed())        # False
-    a = Animal('dog', name='Bello') # Animal('dog', 'Bello')
+    a = Animal('dog', name='Teddy') # Animal('dog', 'Teddy')
     Animal.seal()                   # Seal it!
     print(Animal.issealed())        # True
-    b = Animal('dog', name='Bello') # Returns primary instance
+    b = Animal('dog', name='Teddy') # Returns primary instance
     print(a is b)                   # True
     try:
-        c = Animal('dog', name='Tessa')
+        c = Animal('dog', name='Roxie')
     except KeyError as ex:          # KeyError, Animal is sealed!
         print(f"For '{ex.args[1]}' {ex.args[0]}")
-    print(Animal.get_instances())   # {'Bello': Animal('dog', 'Bello')}
+    print(Animal.get_instances())   # {'Teddy': Animal('dog', 'Teddy')}
     Animal.unseal()                 # Unseal it!
-    c = Animal('dog', name='Tessa') # Animal('dog', 'Bello') now it's ok!
-    print(Animal.get_instances())   # {'Bello': Animal('dog', 'Bello'),
-                                    #  'Tessa': Animal('dog', 'Tessa')}
+    c = Animal('dog', name='Roxie') # Animal('dog', 'Teddy') now it's ok!
+    print(Animal.get_instances())   # {'Teddy': Animal('dog', 'Teddy'),
+                                    #  'Roxie': Animal('dog', 'Roxie')}
 """
 
 # -----------------------------------------------------------------------------
 # Module Level Dunders
 __title__ = "Multiton"
 __module__ = "multiton.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.0.5"
-__date__ = "2023-06-15"
-__time__ = "18:24:13"
+__version__ = "0.1.1.1"
+__date__ = "2023-06-16"
+__time__ = "09:40:57"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Multiton"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
@@ -191,86 +191,86 @@
             self.spec = spec
             self.name = name
 
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.spec}', '{self.name}')"
 
     # Create instances
-    a = Animal('dog', name='Bello')
-    b = Animal('cat', name='Mausi')
-    c = Animal('dog', name='Tessa')
+    a = Animal('dog', name='Teddy')
+    b = Animal('cat', name='Molly')
+    c = Animal('dog', name='Roxie')
 
     # Case 0: decoration @Multiton or @Multiton() or @Multiton(key=17) or ...
     #    ---> With no or fixed key the Multiton acts like a Singleton
-    print(a)                        # Animal('dog', 'Bello')
-    print(b)                        # Animal('dog', 'Bello')
-    print(c)                        # Animal('dog', 'Bello')
+    print(a)                        # Animal('dog', 'Teddy')
+    print(b)                        # Animal('dog', 'Teddy')
+    print(c)                        # Animal('dog', 'Teddy')
 
     # Case 1: decoration @Multiton(key=lambda spec, name: name)
     #    ---> key is a function evaluating the attribute name from __init__(..)
-    print(a)                        # Animal('dog', 'Bello')
-    print(b)                        # Animal('cat', 'Mausi')
-    print(c)                        # Animal('dog', 'Tessa')
+    print(a)                        # Animal('dog', 'Teddy')
+    print(b)                        # Animal('cat', 'Molly')
+    print(c)                        # Animal('dog', 'Roxie')
 
     # Case 2: decoration @Multiton(key=lambda spec, name: 'a' in name)
     #    ---> key is a function evaluating the attribute name from __init__(..)
-    print(a)                        # Animal('dog', 'Bello')
-    print(b)                        # Animal('cat', 'Mausi')
-    print(c)                        # Animal('cat', 'Mausi')
+    print(a)                        # Animal('dog', 'Teddy')
+    print(b)                        # Animal('cat', 'Molly')
+    print(c)                        # Animal('cat', 'Molly')
 
     # Case 3: decoration @Multiton(key="{0}".format)
     #    ---> Parameter spec is referenced as args[0] (positional)
-    print(a)                        # Animal('dog', 'Bello')
-    print(b)                        # Animal('cat', 'Mausi')
-    print(c)                        # Animal('dog', 'Bello')
+    print(a)                        # Animal('dog', 'Teddy')
+    print(b)                        # Animal('cat', 'Molly')
+    print(c)                        # Animal('dog', 'Teddy')
 
     # Case 4: decoration @Multiton(key="{name}".format)
     #    ---> Parameter name is referenced as kwargs['name'] (keyword)
-    print(a)                        # Animal('dog', 'Bello')
-    print(b)                        # Animal('cat', 'Mausi')
-    print(c)                        # Animal('dog', 'Tessa')
+    print(a)                        # Animal('dog', 'Teddy')
+    print(b)                        # Animal('cat', 'Molly')
+    print(c)                        # Animal('dog', 'Roxie')
 
     # Case 5: decoration @Multiton(key=lambda spec, name: (spec, name))
     #    ---> One unique instance for all init values, i.e. no duplicates
-    print(a)                        # Animal('dog', 'Bello')
-    print(b)                        # Animal('cat', 'Mausi')
-    print(c)                        # Animal('dog', 'Tessa')
+    print(a)                        # Animal('dog', 'Teddy')
+    print(b)                        # Animal('cat', 'Molly')
+    print(c)                        # Animal('dog', 'Roxie')
 
     # Case 6: decoration @Multiton(key=F("my_key"))
     #    ---> Late binding with F(classmethod_string)
     #         One unique instance from a @staticmethod or @classmethod
     class Animal:
         ...
         @classmethod
         def my_key(cls, spec, name):
             return 'a' in name
-    print(a)                        # Animal('dog', 'Bello')
-    print(b)                        # Animal('cat', 'Mausi')
-    print(c)                        # Animal('cat', 'Mausi')
+    print(a)                        # Animal('dog', 'Teddy')
+    print(b)                        # Animal('cat', 'Molly')
+    print(c)                        # Animal('cat', 'Molly')
 
     # Case 7: decoration @Multiton(key=lambda spec, name: name,
     #                              accessible=True, resettable=True)
-    #    ---> Seal after Bello
+    #    ---> Seal after Teddy
     Animal.reset()                  # Reset/Clear the instance dictionary
     print(Animal.get_instances())   # {}
     print(Animal.issealed())        # False
-    a = Animal('dog', name='Bello') # Animal('dog', 'Bello')
+    a = Animal('dog', name='Teddy') # Animal('dog', 'Teddy')
     Animal.seal()                   # Seal it!
     print(Animal.issealed())        # True
-    b = Animal('dog', name='Bello') # Returns primary instance
+    b = Animal('dog', name='Teddy') # Returns primary instance
     print(a is b)                   # True
     try:
-        c = Animal('dog', name='Tessa')
+        c = Animal('dog', name='Roxie')
     except KeyError as ex:          # KeyError, Animal is sealed!
         print(f"For '{ex.args[1]}' {ex.args[0]}")
-    print(Animal.get_instances())   # {'Bello': Animal('dog', 'Bello')}
+    print(Animal.get_instances())   # {'Teddy': Animal('dog', 'Teddy')}
     Animal.unseal()                 # Unseal it!
-    c = Animal('dog', name='Tessa') # Animal('dog', 'Bello') now it's ok!
-    print(Animal.get_instances())   # {'Bello': Animal('dog', 'Bello'),
-                                    #  'Tessa': Animal('dog', 'Tessa')}
+    c = Animal('dog', name='Roxie') # Animal('dog', 'Teddy') now it's ok!
+    print(Animal.get_instances())   # {'Teddy': Animal('dog', 'Teddy'),
+                                    #  'Roxie': Animal('dog', 'Roxie')}
     """
 
     def __init__(self,
                  substitute: type = None,
                  *args: object,
                  key: Union[F, callable, object, None] = None,
                  accessible: bool = False,
@@ -311,40 +311,45 @@
                 """Define reset method"""
                 s.__instances.clear()
 
             # Add the reset method
             setattr(self, 'reset', reset)
 
         # --- Decorator Arguments Pattern (1/2)
-        if self.__substitute is not None:
+        if self.__get__substitute() is not None:
             # Decoration without parameter(s)
-            self.__set__substitute(F(self.__substitute, *args, **kwargs))
+            self.__set__substitute(
+                F(self.__get__substitute(), *args, **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
 
     def __call__(self, *args, **kwargs):
         """Apply the decorator"""
         # --- Decorator Arguments Pattern (2/2)
-        if self.__substitute is None:
+        if self.__get__substitute() is None:
             # Decoration with parameter(s)
             self.__set__substitute(F(args[0], *args[1:], **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
             return self
         else:  # *** Wrapper ***
             # If no current values, take defaults
             if args or kwargs:
                 subst = F(self.__get__substitute().callee, *args, **kwargs)
             else:
                 subst = self.__get__substitute()
 
             # Calculate key from callable or read key from arguments
             try:
                 if isinstance(self.__key, F):  # classmethod or staticmethod
-                    d_key = F(
-                        getattr(self.substitute.callee, self.__key.callee),
-                        *subst.callee_args, **subst.callee_kwargs).eval()
+                    if callable(self.__key.callee):
+                        d_key = F(self.__key.callee, *subst.callee_args,
+                                  **subst.callee_kwargs).eval()
+                    else:
+                        d_key = F(
+                            getattr(self.substitute.callee, self.__key.callee),
+                            *subst.callee_args, **subst.callee_kwargs).eval()
                 elif callable(self.__key):  # function
                     d_key = F(self.__key, *subst.callee_args,
                               **subst.callee_kwargs).eval()
                 else:  # Value
                     d_key = self.__key
                 instance = self.__instances.get(d_key, None)
             except (TypeError, Exception):  # Default is None
```

### Comparing `decoratory-0.1.0.3/Sources/decoratory/observer.py` & `decoratory-0.1.1.3/Sources/decoratory/observer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,302 +1,345 @@
 #!/usr/bin/env python
 # -*- coding=UTF-8 -*-
 # vim: fileencoding=UTF-8 tabstop=8 expandtab shiftwidth=4 softtabstop=4
 # -----------------------------------------------------------------------------
 # Document Description
 """**Observer Pattern**
 
-The observer pattern is generally used to inform one or more registered
-objects (observers, subscribers, objects) about a specific action of a given
-observed object (observable, publisher, subject).
-
-This implementation offers different possibilities to decorate a function/class
-as an observable resp. observer.
-
--------------------------------------------------------------------------------
-A) Observable decoration
-
-The simplest as well as most pythonic version for decoration is to decorate
-only the observable elements. This is possible, because all observer pattern
-functionalities are located in the BaseClass (=BaseObservable) of the
-Observable decorator while the BaseClass (=BaseObserver) of the Observer
-decorator is empty, here. From both BaseClasses can be inherited to extend
-their functionalities.
+    The observer pattern is generally used to inform one or more registered
+    objects (observers, subscribers, objects) about selected actions of an
+    observed object (observable, publisher, subject).
 
-Example:
+    This implementation provides several ways to decorate a function or class
+    as an Observable or Observer.
+
+    Attributes
+    ----------
+        None.
+
+    Methods
+    -------
+    seal(self):
+        Seal multiton.
+
+    unseal(self):
+        Unseal multiton.
+
+    issealed(self):
+        Multiton sealing state
+
+    get_instance():
+        Return the singleton instance.  (if accessible=True)
+
+    reset():
+        Resets the singleton instance.  (if resettable=True)
+
+    Example
+    -------
+
+    A) Observable Decoration
+
+    The simplest and at the same time the most Pythonic variant of decoration
+    is to decorate only the *observed* entities. This is possible because all
+    observer pattern functionalities are concentrated in the BaseClass
+    (=BaseObservable) of the observable decorator, while the BaseClass
+    (=BaseObserver) of the observer decorator remains empty here. If
+    necessary, it is possible to inherit from both BaseClasses to extend
+    their functionalities.
+
+    from decoratory.observer import Observable
 
     def person(say: str = "Hello?"):
         print(f"{person.__name__} says '{say}'")
 
     @Observable(observers=F(person, 'Hey, dog!'))
     def dog(act: str = "Woof!"):
         print(f"{dog.__name__} acts '{act}'")
 
-This results in:
-
-    1. Calling person() prints:
-        person says 'Hello?'            # person is acting
+    # Case 1: Observable decoration
+    #    ---> Person as an observer to dog
+    person()                        # person says 'Hello?'
+    dog()                           # dog acts 'Woof!'        (dog acting)
+                                    # person says 'Hey, dog!' (observer to dog)
+
+    Obviously, the addressed observer, the person, must be specified before
+    the observed, the dog. To make the observers more visible in the code, an
+    (optional) observer decoration is supported, i.e.
 
-    2. Calling dog() prints:
-        dog acts 'Woof!'                # dog is acting, default dog
-        person says 'Hey, dog!'         # person is a custom. observer to dog
-
-Obviously, the addressed observer, the person, must be declared before the
-observed, the dog. In order to make the observers more visible in the code, an
-(optional) Observer decoration is supported, i.e.
-
-    @Observer
+    @Observer                       # Just for the clarity of the code!
     def person(say: str = "Hello?"):
         print(f"{person.__name__} says '{say}'")
 
-making person to an Observer, but here, with the same result as above.
-
-Because of hierarchies in stacked observer patterns a more detailed managing
-of the observed observable objects can be necessary.
+    This makes person an observer, but here with the same result as above.
 
-Example:
+    Due to hierarchies in stacked observer patterns, a more detailed management
+    of the observed objects may be necessary.
 
     def person(say: str = "Hello?"):
         print(f"{person.__name__} says '{say}'")
 
     @Observable(observers=F(person, 'Hey, cat!'))
     def cat(act: str = "Meow!"):
         print(f"{cat.__name__} acts '{act}'")
 
     @Observable(observers=[F(cat, 'Roar!'), F(person, 'Hey, dog!')])
     def dog(act: str = "Woof!"):
         print(f"{dog.__name__} acts '{act}'")
 
-This results in:
+    # Case 2: Stacked observable decoration
+    #    ---> Cat observes dog, person observes cat and dog
+    person()                        # person says 'Hello?'    (person acting)
+
+    cat()                           # cat acts 'Meow!'        (cat acting)
+                                    # person says 'Hey, cat!' (observer to cat)
+
+    dog()                           # dog acts 'Woof!'        (dog acting)
+                                    # cat acts 'Roar!'        (observer to dog)
+                                    # person says 'Hey, cat!' (observer to cat)
+                                    # person says 'Hey, dog!' (observer to dog)
 
-    1. Calling person() prints:
-        person says 'Hello?'            # person is acting
-
-    2. Calling cat() prints:
-        cat acts 'Meow!'                # cat    is acting
-        person says 'Hey, cat!'         # person is an observer to cat
-
-    3. Calling dog() prints:
-        dog acts 'Woof!'                # dog    is acting
-        cat acts 'Roar!'                # cat    is an observer to dog
-        person says 'Hey, cat!'         # person is an observer to cat
-        person says 'Hey, dog!'         # person is an observer to dog
-
-The order of the reactions comes from the list order where cat observes dog
-prior to person. Switching this order to
+    The order of reactions is determined by the order in the list in which
+    the cat observes the dog prior to the person. If this order is reversed:
 
     @Observable(observers=[F(person, 'Hey, dog!'), F(cat, 'Roar!')])
     def dog(act: str = "Woof!"):
         print(f"{dog.__name__} acts '{act}'")
 
-results in
-
-    3. Calling dog() prints:
-        dog acts 'Woof!'                # dog    is acting
-        person says 'Hey, dog!'         # person is an observer to dog
-        cat acts 'Roar!'                # cat    is an observer to dog
-        person says 'Hey, cat!'         # person is an observer to cat
-
-Calling dog() results in three observer calls because dog() addresses the
-'observed cat' informing person about its own action. If this behavior is not
-desired, dog can address the 'native cat' using cat's substitute instead, i.e.
+    # Case 3: Stacked observable decoration
+    #    ---> Cat observes dog, person observes dog and cat
+    dog()                           # dog acts 'Woof!'        (dog acting)
+                                    # person says 'Hey, dog!' (observer to dog)
+                                    # cat acts 'Roar!'        (observer to dog)
+                                    # person says 'Hey, cat!' (observer to cat)
+
+    Calling dog() results in three activities at the observers, because dog()
+    observes the 'observed cat', which informs the person about its own action.
+    If this behavior is not desired, dog() can instead address the
+    'original cat' using the cat substitute, i.e.
 
     @Observable(observers=[F(cat.substitute.callee, 'Roar!'),
                            F(person, 'Hey, dog!')])
     def dog(act: str = "Woof!"):
         print(f"{dog.__name__} acts '{act}'")
 
-results in
+    # Case 4: Stacked observable decoration
+    #    ---> Original cat observes dog, person observes dog and cat
+    dog()                           # dog acts 'Woof!'        (dog acting)
+                                    # cat acts 'Roar!'        (observer to dog)
+                                    # person says 'Hey, dog!' (observer to dog)
 
-    3. Calling dog() prints:
-        dog acts 'Woof!'                # dog    is acting
-        cat acts 'Roar!'                # cat    is an observer to dog
-        person says 'Hey, dog!'         # person is an observer to dog
+    And again, cat acts before person because of the order of the observer
+    list.
 
-And again, cat acts before person because of the order of the observer list.
 
--------------------------------------------------------------------------------
-B) Observer decoration
+    B) Observer Decoration
 
-In this reversed decoration the Observer decorator defines its observable.
-Because an observer decoration makes use of observable methods the
-observable(s) always has to be declared before any of its observer(s)!
+    In this reverse decoration, the observer decorator defines its observables.
+    Because an observer decoration uses observable methods, all observable(s)
+    must always be declared before their observer(s).
 
-    1) Rule: Declare Observables before Observers
+    1. Rule: Declare Observables before Observers
 
-For multiple decoration the **order of decoration** matters. At the end it has
-to be an observable for following observers
+    Thus, the initial example Case 1 from above is as follows:
 
-    2) Rule: Decorate @Observer before @Observable
-
-Example:
+    from decoratory.observer import Observer, Observable
+    from decoratory.basic import X
 
     @Observable
-    def dog(act: str = "Woof!"):
+    def dog(act: str = "Woof!"):    # 1. Rule: declare dog before person!
         print(f"{dog.__name__} acts '{act}'")
 
-    @Observable                             # 2) Rule: cat before person
-    @Observer(observables=X(dog, 'Roar!'))  # 1) Rule: dog before cat
-    def cat(act: str = "Meow!"):
-        print(f"{cat.__name__} acts '{act}'")
-
-    @Observer(observables=[X(dog, 'Hey, dog!'), X(cat, say='Hey, cat!')])
+    @Observer(observables=X(dog, 'Hey, dog!'))
     def person(say: str = "Hello?"):
         print(f"{person.__name__} says '{say}'")
 
-This results in:
+    # Case 1: Observer decoration
+    #    ---> Person as an observer to dog
+    person()                        # person says 'Hello?'
+    dog()                           # dog acts 'Woof!'        (dog acting)
+                                    # person says 'Hey, dog!' (observer to dog)
+
+    The use of the semantic X instead of F indicates that dog is the
+    observable, but the X arguments are for person.
+
+    For multiple decorations, the order of decoration is relevant. Each
+    observable must be decorated before it is used by the observer.
 
-    1. Calling person() prints:
-        person says 'Hello?'            # person is acting
+    2. Rule: Decorate @Observer before @Observable
 
-    2. Calling cat() prints:
-        cat acts 'Meow!'                # cat    is acting
-        person says 'Hey, cat!'         # person is an observer to cat
-
-    3. Calling dog() prints:
-        dog acts 'Woof!'                # dog    is acting
-        cat acts 'Roar!'                # cat    is an observer to dog
-        person says 'Hey, dog!'         # person is an observer to dog
-
-Again, the 'observable cat' person observes is not the 'native cat' observing
-dog, thus, person reacts only to dog but not to the induced cat by dog. If
-desired, that person reacts to the dog induced cat also, simply switch the
-decoration order and address the substitute of the 'observer cat':
+    The above situation with person, dog and cat would then look like this:
+
+    @Observable                     # 2. Rule: dog before cat, person
+    def dog(act: str = "Woof!"):    # 1. Rule: dog before cat, person
+        print(f"{dog.__name__} acts '{act}'")
 
     @Observer(observables=X(dog, 'Roar!'))
-    @Observable
-    def cat(act: str = "Meow!"):
+    @Observable                     # 2. Rule: cat before person
+    def cat(act: str = "Meow!"):    # 1. Rule: cat before person
         print(f"{cat.__name__} acts '{act}'")
 
     @Observer(observables=[X(dog, 'Hey, dog!'),
                            X(cat.substitute.callee, say='Hey, cat!')])
     def person(say: str = "Hello?"):
         print(f"{person.__name__} says '{say}'")
 
-Then, in 3. the result will be:
+    # Case 2: Stacked observer decoration
+    #    ---> Cat observes dog, person observes cat and dog
+    person()                        # person says 'Hello?'    (person acting)
+
+    cat()                           # cat acts 'Meow!'        (cat acting)
+                                    # person says 'Hey, cat!' (observer to cat)
+
+    dog()                           # dog acts 'Woof!'        (dog acting)
+                                    # cat acts 'Roar!'        (observer to dog)
+                                    # person says 'Hey, cat!' (observer to cat)
+                                    # person says 'Hey, dog!' (observer to dog)
+
+    Here, the observed cat observes the dog, reacts and triggers the person
+    observing the orignal cat. This situation reflects the Case 2 from above.
+
+    To reproduce Case 3 above, simply swap the order of the decorations at the
+    cat and the person then looks at the observed cat.
+
+    @Observable                     # 2. Rule: dog before cat, person
+    def dog(act: str = "Woof!"):    # 1. Rule: dog before cat, person
+        print(f"{dog.__name__} acts '{act}'")
+
+    @Observable                     # 2. Rule: cat before person
+    @Observer(observables=X(dog, 'Roar!'))
+    def cat(act: str = "Meow!"):    # 1. Rule: cat before person
+        print(f"{cat.__name__} acts '{act}'")
+
+    @Observer(observables=[X(dog, 'Hey, dog!'), X(cat, say='Hey, cat!')])
+    def person(say: str = "Hello?"):        # 1) Rule: dog, cat before person
+        print(f"{person.__name__} says '{say}'")
+
+    # Case 3: Stacked observer decoration
+    #    ---> Cat observes dog, person observes cat and dog
+    person()                        # person says 'Hello?'    (person acting)
+
+    cat()                           # cat acts 'Meow!'        (cat acting)
+                                    # person says 'Hey, cat!' (observer to cat)
+
+    dog()                           # dog acts 'Woof!'        (dog acting)
+                                    # cat acts 'Roar!'        (observer to dog)
+                                    # person says 'Hey, dog!' (observer to dog)
+
+    Note the difference: in Case 2, the cat ends up as an Observer, not as an
+    Observable. So the person observes the original cat. Whereas in case 3,
+    the cat actually ends up as an Observable and person can observe the
+    observed cat.
 
-    3. Calling dog() prints:
-        dog acts 'Woof!'                # dog    is acting
-        cat acts 'Roar!'                # cat    is an observer to dog
-        person says 'Hey, cat!'         # person is an observer to cat
-        person says 'Hey, dog!'         # person is an observer to dog
 
--------------------------------------------------------------------------------
-C) Static decoration
+    C) Static Class Decoration
 
-Both techniques, A) and B), are static, in the sense, decorations are done in
-pie notation evaluated at compile time. They are applied to (static) functions.
+    Both techniques, observable and observer decoration, are static, in the
+    sense, decorations are done in @-notation evaluated at compile time. They
+    are applied to *static functions*.
 
-Decoration of a class by default addresses decoration of the class constructor:
+    Decoration of a class by default addresses decoration of the class
+    constructor, this means
 
     @Observable
     class Dog:
         def __init__(self):
-            pass
+            pass                    # Some code ...
 
-should be understood as
+    should be understood as
 
     class Dog:
         @Observable
         def __init__(self):
-            pass
+            pass                    # Some code ...
 
-ATTENTION:  Calling __init__ results in a new instance! This means calling the
-            observable induces instantiation of a new observer object, surely
-            in not any case this is the desired action - so, be careful here!
-
-To address other methods, both decorators, Observable and Observer, support the
-methods parameter for a single or even a list of methods by name strings. In
-these cases the class itself remains undecorated but the listed method(s) are
-decorated.
-
-    @Observable(methods=['meth1', F('meth2', 13, key='number')])
-    class A:
-        def meth1(self, val=0):
-            pass
-        def meth2(self, val=0, key='decimal'):
-            pass
+    But this behavior is insidious.
 
-should be understood as
-
-    class A:
-        @Observable
-        def meth1(self, val=0):                 # Using declaration defaults!
-            pass
-        @Observable
-        def meth2(self, val=13, key='number'):  # Using decoration defaults!
-            pass
-
-Clearly, these techniques allow to address static methods and class methods
-being declared at compile time. For instance methods things are different,
-because instances are not available at compile time. They are generated within
-the init constructor. Therefore, instance methods are decorated best in the
-object constructor.
-
-Example:
+    WARNING: Calling __init__() results in a new instance! This means calling
+             the observable induces instantiation of a new observer object,
+             surely in not any case this is the desired action...
+
+    These previous two techniques can be used to decorate @staticmethod and
+    @classmethod that are declared and available at compile time. Things are
+    different for instance methods, because instances are not available at
+    compile time. They are not available until class instantiation. Therefore,
+    instance methods are best decorated dynamically in the class constructor.
 
     class Agent:
         @classmethod
         def inform(cls, value):
             print(f"Informed value is: {value}")
 
         def report(self, value):
             print(f"Reported value is: {value}")
 
     class Actor:
         def __init__(self):
-            self.a = 1
+            self.a = 1              # Dynamic decoration, static data
             print(f"Initialization: a = {self.a}")
             self.modify = Observable(observers=[
                 F(Agent.inform, 'unknown'),
-                F(Agent().report, 'undef')])(self.modify)
+                F(Agent().report, 'undefined')])(self.modify)
 
         def modify(self, value=1):
             self.a += value
             print(f"Modification  : a = {self.a}")
 
-Every Actor instance defines its modify method as an observable reporting every
-modification of self.a to the class method Agent.inform as well as to an
-instance method Agent().report. But at init no value data is available, so only
-a static reporting will be feasible this way. Running
+    Each Actor instance defines its modify method as an observable, which
+    informs about each change of self.a both the class method Agent.inform
+    and the Agent().report instance method. But at the time of execution of
+    __init__ no (current) values or data are available yet, so only static
+    reporting is possible in this way.
+
+    # Case 1: Dynamic decoration, static data
+    a = Actor()                     # Initialization: a = 1
+    a.modify(13)                    # Modification  : a = 14
+                                    # Informed value is: unknown
+                                    # Reported value is: undefined
+
+    However, the problem can be tackled i.e. adding the attribute
+    activate=Activation.NONE to the Observable definition in __init__ to
+    switch off default Activation.AFTER and add an individualized dispatch
+    within the modify method
 
-    a = Actor()
-    a.modify(13)
-
-will generate the messages:
-
-    Initialization: a = 1
-    Modification  : a = 14
-    Informed value is: unknown
-    Reported value is: undef
-
-But this problem can be solved i.e. adding the attribute
-
-    activate=Activation.NONE
+    class Actor:
+        def __init__(self):
+            self.a = 1
+            print(f"Initialization: a = {self.a}")
+            self.modify = Observable(observers=[
+                F(Agent.inform, 'unknown'),
+                F(Agent().report, 'undefined')],
+            # (1) Switch off default activation
+                activate=Activation.NONE)(self.modify)
 
-to the Observable definition in init to switch off default Activation.AFTER
-and add an individualized dispatch within the modify method
+        def modify(self, value=1):
+            self.a += value
+            print(f"Modification  : a = {self.a}")
+            # (2) Add individual dispatch
+            self.modify.observable.dispatch(value=self.a)
 
-    self.modify.observable.dispatch(None, value)        or
-    self.modify.observable.dispatch(value=value)
+    # Case 2: Dynamic decoration, dynamic data
+    a = Actor()                     # Initialization: a = 1
+    a.modify(13)                    # Modification  : a = 14
+                                    # Informed value is: 14
+                                    # Reported value is: 14
 
-and the prints look like
 
-    Initialization: a = 1
-    Modification  : a = 14
-    Reported value is: 13
-    Informed value is: 13
+    D) Dynamic Class Decoration
 
--------------------------------------------------------------------------------
-D) Dynamic decoration
+    The classic way to exchange information between objects with the observer
+    pattern is through the active use of the register, dispatch, and unregister
+    methods that an observable exports. This way, information can be given to
+    the right recipients at the right places in the code. For this, the
+    classes are not decorated. The dynamic decoration comes into play.
 
-Decoration, registration etc. can also be done outside the class(es).
-Observers can be registered and unregistered on demand in the program.
+    For this, the classes remain undecorated. Dynamic decoration is used,
+    often also in connection with getter/setter/property constructions, since
+    data changes take place meaningfully over these methods.
 
-Example:
+    Let’s start with the simple classes:
 
     class Note:                             # Observer without decoration!
         def info(self, thing):
             print(f"Note.info: val = {thing.a}")
 
     class Thing:                            # Observable without decoration!
         def __init__(self, a=0):
@@ -305,57 +348,62 @@
             self._a += 1
         def get_a(self):
             return self._a
         def set_a(self, value):
             self._a = value
         a = property(get_a, set_a)
 
-Some typical actions could be:
+    Well, some typical actions might be:
 
-    # Preparation
-    nti = Note()                            # Note instance
-    thg = Thing()                           # Thing instance
+    # (1) Setup instances
+    nti = Note()                    # Note instance
+    thg = Thing()                   # Thing instance
 
+    # (2) Dynamic decoration of some methods: Late binding
     thg.inc = Observable(thg.inc)           # Late method decoration
     Thing.set_a = Observable(Thing.set_a)   # Late property decoration
     Thing.a = property(Thing.get_a, Thing.set_a)
 
+    # (3) Register the observer (Note) with the observable (Thing)
     thg.inc.observable.register(F(nti.info, thg))
     thg.set_a.observable.register(F(nti.info, thing=thg))
 
-    # Usage
-    thg.inc()                               # Method   observers dispatched
-    thg.a = 2                               # Property observers dispatched
+    # Case 1: Change self.a = 0 using inc()
+    thg.inc()                       # Note.info: val = 1
 
+    # Case 2: Change self.a = 1 using setter via property
+    thg.a = 2                       # Note.info: val = 2
+
+    # Case 3: Notification from inc() to nti.info() about Thing(3)
     thg.inc.observable.dispatch(nti.info, Thing(3))
-    thg.set_a.observable.dispatch(nti.info, Thing(4))
+                                    # Note.info: val = 3
 
-This will print:
+    # Case 4: Notification from set_a() to nti.info() about Thing(4)
+    thg.set_a.observable.dispatch(nti.info, Thing(4))
+                                    # Note.info: val = 4
 
-    Note.info: val = 1                      # from observing thg.inc()
-    Note.info: val = 2                      # from observing thg.a = 2
-    Note.info: val = 3                      # by thg.inc.observable
-    Note.info: val = 4                      # by thg.set_a.observable
+    # Case 5: Print the current value of thg.a
+    print(f"a = {thg.a}")           # a = 2     (no changes by notifications)
 """
 
 # -----------------------------------------------------------------------------
 # Module Level Dunders
 __title__ = "Observer"
 __module__ = "observer.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.0.1"
-__date__ = "2023-06-12"
-__time__ = "14:49:52"
+__version__ = "0.1.1.2"
+__date__ = "2023-06-16"
+__time__ = "19:56:14"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Observer", "BaseObserver", "Observable", "BaseObservable"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
@@ -385,78 +433,83 @@
     method of class A or an instance a = A():
      - Registration call:   F(a.method, *args, **kwargs).eval()         or
                             F('method', a, *args, **kwargs).eval()      but not
      - Dynamic call:        F('method', *args, **kwargs).eval(obj=a)
     """
 
     def __init__(self, *args, **kwargs) -> None:
-        # Python 3.7ff.: Dictionary order is guaranteed to be insertion order.
-        self.__observers = dict()  # dict of F-type observers: callee is key!
-
-        # if args or kwargs:
-        #     raise NotImplementedError(
-        #     f"Abstract class {self.__class__.__name__} has no arguments.")
         self.args = args
         self.kwargs = kwargs
 
+        self.__observers = dict()  # dict of F-type observers: callee is key!
+
     # Methods of the Observer Pattern
     def register(self,
                  observer: Union[F, callable, str],
                  *observer_args,
                  **observer_kwargs) -> None:
-        """**Register a function (callable) or method (str) for callback**
+        """Register a function (callable) or method (str) for callback.
+
+        Parameters:
+            observer (F|callable|str): Callback function|method of the observer
+            observer_args (object): Callback (default) positional arguments
+            observer_kwargs (object): Callback (default) keyword arguments
 
-        @param observer:        Callback function or method str of the observer
-        @param observer_args:   The (default) positional arguments for callback
-        @param observer_kwargs: The (default) keyword    arguments for callback
-        @rtype:                 NoneType
+        Returns:
+            None.
         """
         if isinstance(observer, F):
             if observer_args or observer_kwargs:
                 observer.callee_args = observer_args
                 observer.callee_kwargs = observer_kwargs
             self.__observers[observer.callee] = observer  # Override mode
         elif callable(observer) or isinstance(observer, str):
             obs = F(observer, *observer_args, **observer_kwargs)
             self.__observers[observer] = obs
         else:
             raise TypeError(f"'{observer}' cannot be registered.")
 
     def unregister(self,
                    observer: Union[F, callable, str, None] = None) -> None:
-        """**Unregister an observer**
+        """Unregister an observer.
 
         If the observer parameter is omitted (None), all registered observers
         will be unregistered.
 
-        @param observer: The (optional) observer callable to be unregistered
-        @rtype:          NoneType
+        Parameters:
+            observer (F|callable|str|None): Callback to be unregistered
+
+        Returns:
+            None.
         """
         if observer is None:
             self.__observers.clear()
         elif isinstance(observer, F):
             self.__observers.pop(observer.callee, None)  # Quiet mode
         elif callable(observer) or isinstance(observer, str):
             self.__observers.pop(observer, None)  # Quiet mode
         else:
             raise TypeError(f"'{observer}' cannot be unregistered.")
 
     def dispatch(self,
                  observer: Union[F, callable, str, None] = None,
                  *observer_args,
                  **observer_kwargs) -> None:
-        """**Dispatch an observer**
+        """Dispatch an observer.
 
         If the observer parameter is omitted (None), all registered observers
         will be dispatched.
 
-        @param observer:        The observer's callable to be dispatched
-        @param observer_args:   The (default) positional arguments for dispatch
-        @param observer_kwargs: The (default) keyword    arguments for dispatch
-        @rtype:                 NoneType
+        Parameters:
+            observer (F|callable|str|None): Callback to be dispatched
+            observer_args (object): Callback (default) positional arguments
+            observer_kwargs (object): Callback (default) keyword arguments
+
+        Returns:
+            None.
         """
         if observer is None:
             # Registration call using default arguments, no extra eval obj!
             if observer_args or observer_kwargs:
                 for obs in self.__observers.values():
                     F(obs.callee, *observer_args, **observer_kwargs).eval()
             else:
@@ -467,32 +520,37 @@
             if observer_args or observer_kwargs:
                 F(observer.callee, *observer_args, **observer_kwargs).eval()
             else:
                 observer.eval()
         elif callable(observer):
             # Dynamic call using current arguments, no extra eval obj!
             F(observer, *observer_args, **observer_kwargs).eval()
+        elif isinstance(observer, str):
+            pass  # todo: str???
         else:
             raise TypeError(f"'{observer}' cannot be dispatched.")
 
     def observers(self, classbased=False) -> dict:
-        """**Listing of all observers**
+        """Listing of all observers.
 
         Observers are collected in a dict, which is returned by default with
         classbased=False. Calling with classbased=True returns a dictionary
         with key-value-pair syntax {classname: list(methods)}.
 
-        @param classbased: A boolean switch for returned data structure
-        @return:           Dictionary of all observers
+        Parameters:
+            classbased (bool): A boolean switch for returned data structure
+
+        Returns:
+            observers (dict): Dictionary of all observers
         """
         if bool(classbased):
             result = dict()
             for obs in self.__observers.values():
                 *skip, cls, mtd = obs.callee.__qualname__.split(".")
-                result.setdefault(cls, []).append(repr(obs))
+                result.setdefault(cls, []).append(obs)
             return result
         else:
             return self.__observers  # Has to be the default (without params)!
 
 
 class Observable:
     """**Observable** (Publisher, Subject)
@@ -510,102 +568,106 @@
     def __init__(self,
                  substitute: Union[callable, type] = None,
                  *args: object,
                  observers: Union[list, F, callable, str] = None,
                  methods: Union[list, F, callable, str] = None,
                  activate: Activation = Activation.AFTER,
                  **kwargs: object) -> None:
-        """**Observable** (Publisher, Subject)
+        """Observable (Publisher, Subject).
 
-        @param substitute: The callable or type to be made an observable
-        @param observers: (List of) callable(s) of observers
-        @param methods: (List of) callable(s) of method strings
-        @param activate: Dispatch activation point of time
-        @rtype: NoneType
+        Parameters:
+            substitute (callable|type: Callable|Type to be made an observable
+            observers (list|F|callable|str): (List of) callable(s) of observers
+            methods (list|F|callable|str): (List of) callable(s) of as strings
+            activate (Activation): Dispatch activation point in time
+
+        Returns:
+            None.
         """
         self.__set__substitute(substitute)
         self.__set__observers(observers)
         self.__set__methods(methods)
-        self.activate = activate
+        self.__set__activate(activate)
 
-        # Decorator Arguments Pattern
-        if self.__substitute is not None:
+        # --- Decorator Arguments Pattern (1/2)
+        if self.__get__substitute() is not None:
             # Decoration without parameter(s)
-            self.__set__substitute(F(self.__substitute, *args, **kwargs))
+            self.__set__substitute(
+                F(self.__get__substitute(), *args, **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
 
             # Instance of BaseObservable
             self.__set__observable(Observable.BaseClass())
         else:
             # Decoration with parameter(s)
             self.__set__decorator_args(args)
             self.__set__decorator_kwargs(kwargs)
 
             # Instance of BaseObservable
             self.__set__observable(Observable.BaseClass(
-                *self.__decorator_args, **self.__decorator_kwargs))
+                *self.__get__decorator_args(),
+                **self.__get__decorator_kwargs()))
 
     def __call__(self, *args, **kwargs):
-        # Decorator Arguments Pattern
-        if self.__substitute is None:
+        # --- Decorator Arguments Pattern (2/2)
+        if self.__get__substitute() is None:
             # Decoration with parameter(s)
             self.__set__substitute(F(args[0], *args[1:], **kwargs))
 
             # Decoration of a type means decoration of *all* submitted methods
-            if self.__methods:
+            if self.__get__methods():
                 # Resolve list of methods:
                 subst = self.__get__substitute().callee
-                for mtd, mtd_args, mtd_kwargs in self.__methods:
+                for mtd, mtd_args, mtd_kwargs in self.__get__methods():
                     if isinstance(mtd, str) and hasattr(subst, mtd):
                         mtds = mtd
                         mtd0 = getattr(subst, mtds)
                     elif callable(mtd):
                         mtds = mtd.__name__
                         mtd0 = mtd
                     else:
                         raise TypeError(f"{mtd} is nor a string nor callable.")
                     # noinspection PyArgumentEqualDefault
                     mtd1 = Observable(
                         None,  # Call with deco arguments (substitute is None)
-                        *self.__decorator_args,
-                        observers=self.__observers,
+                        *self.__get__decorator_args(),
+                        observers=self.__get__observers(),
                         methods=None,  # Resolved, call to else part below!
-                        activate=self.activate,
-                        **self.__decorator_kwargs)(mtd0,
-                                                   *mtd_args,
-                                                   **mtd_kwargs)
+                        activate=self.__get__activate(),
+                        **self.__get__decorator_kwargs())(
+                        mtd0, *mtd_args, **mtd_kwargs)
                     setattr(subst, mtds, mtd1)
 
                 # Return the undecorated original class
                 return subst
             else:
                 # Setup observers
-                if self.__observers:
-                    for observer in self.__observers:
-                        self.__observable.register(observer)
+                if self.__get__observers():
+                    for observer in self.__get__observers():
+                        self.__get__observable().register(observer)
 
                 # Complete wrapper and return observable
                 update_wrapper(self, self.__get__substitute().callee,
                                updated=())
                 return self
         else:  # *** Wrapper ***
             # Dispatch BEFORE
-            if self.activate & Activation.BEFORE:
-                self.__observable.dispatch()
+            if self.__get__activate() & Activation.BEFORE:
+                self.__get__observable().dispatch()
 
             # Delegation: apply the substitute, current before default values
             if args or kwargs:
                 result = F(self.__get__substitute().callee, *args,
                            **kwargs).eval()
             else:
                 result = self.__get__substitute().eval()
 
             # Dispatch AFTER
-            if self.activate & Activation.AFTER:
-                self.__observable.dispatch()
+            if self.__get__activate() & Activation.AFTER:
+                self.__get__observable().dispatch()
 
             return result
 
     # Getter, Setter, Properties
     def __get__substitute(self):
         return self.__substitute
 
@@ -653,17 +715,17 @@
         self.__observable = value
 
     observable = property(__get__observable)
 
     def __get__activate(self):
         return self.__activate
 
-    def __set__activate(self, value):
-        self.__activate = value if isinstance(
-            value, Activation) else Activation.NONE
+    def __set__activate(self, activate):
+        self.__activate = activate if isinstance(
+            activate, Activation) else Activation.NONE
 
     activate = property(__get__activate, __set__activate)
 
 
 class BaseObserver:
     """**Observer Base Class**
 
@@ -673,17 +735,14 @@
     callable as an observer is optional. If BaseObserver is overwritten and
     assigned to the observers BaseClass attribute all non captured decorator
     args & kwargs will be submitted to be used in customized class
     functionalities.
     """
 
     def __init__(self, *args, **kwargs):
-        # if args or kwargs:
-        #     raise NotImplementedError(
-        #     f"Abstract class {self.__class__.__name__} has no arguments.")
         self.args = args
         self.kwargs = kwargs
 
 
 class Observer:
     """**Observer** (Subscriber, Object)
 
@@ -707,71 +766,72 @@
         @param methods: (List of) callable(s) of method strings
         @rtype: NoneType
             """
         self.__set__substitute(substitute)
         self.__set__observables(observables)
         self.__set__methods(methods)
 
-        # Decorator Arguments Pattern
-        if self.__substitute is not None:
+        # --- Decorator Arguments Pattern (1/2)
+        if self.__get__substitute() is not None:
             # Decoration without parameter(s)
-            self.__set__substitute(F(self.__substitute, *args, **kwargs))
+            self.__set__substitute(
+                F(self.__get__substitute(), *args, **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
 
             # Instance of BaseObserver
             self.__set__observer(Observer.BaseClass())
         else:
             # Decoration with parameter(s)
             self.__set__decorator_args(args)
             self.__set__decorator_kwargs(kwargs)
 
             # Instance of BaseObserver
             self.__set__observer(Observer.BaseClass(
-                *self.__decorator_args, **self.__decorator_kwargs))
+                *self.__get__decorator_args(),
+                **self.__get__decorator_kwargs()))
 
     def __call__(self, *args, **kwargs):
-        # Decorator Arguments Pattern
-        if self.__substitute is None:
+        # --- Decorator Arguments Pattern (2/2)
+        if self.__get__substitute() is None:
             # Decoration with parameter(s)
             self.__set__substitute(F(args[0], *args[1:], **kwargs))
 
             # Decoration of a type means decoration of *all* submitted methods
-            if self.__methods:
+            if self.__get__methods():
                 # Resolve list of methods:
                 subst = self.__get__substitute().callee
-                for mtd, mtd_args, mtd_kwargs in self.__methods:
+                for mtd, mtd_args, mtd_kwargs in self.__get__methods():
                     if isinstance(mtd, str) and hasattr(subst, mtd):
                         mtds = mtd
                         mtd0 = getattr(subst, mtds)
                     elif callable(mtd):
                         mtds = mtd.__name__
                         mtd0 = mtd
                     else:
                         raise TypeError(f"{mtd} is nor a string nor callable.")
                     # noinspection PyArgumentEqualDefault
                     mtd1 = Observer(
                         None,  # Call with deco arguments (substitute is None)
-                        *self.__decorator_args,
-                        observables=self.__observables,
+                        *self.__get__decorator_args(),
+                        observables=self.__get__observables(),
                         methods=None,  # Resolved, call to else part below!
-                        **self.__decorator_kwargs)(mtd0,
-                                                   *mtd_args,
-                                                   **mtd_kwargs)
+                        **self.__get__decorator_kwargs())(
+                        mtd0, *mtd_args, **mtd_kwargs)
                     setattr(subst, mtds, mtd1)
 
                 # Return the undecorated original class
                 return subst
             else:
                 # Register self as a callable object for callback
                 # CAUTION: observables is a list of X-objects with semantics
                 #     obs = X(observABLE, observER_args, observER_kwargs)
                 # The arguments belong to the observer (self) but not to the
                 # observable from the observables list!
-                if self.__observables:
-                    for observable in self.__observables:
+                if self.__get__observables():
+                    for observable in self.__get__observables():
                         if isinstance(observable.callee, Observable):
                             observable.callee.observable.register(
                                 self, *observable.callee_args,
                                 **observable.callee_kwargs)
                         else:
                             raise TypeError(
                                 f"{observable.callee} is not an observable.")
@@ -853,80 +913,15 @@
            company=__company__,
            email=__email__,
            url=__url__,
            copyright=__copyright__,
            state=__state__,
            license=__license__)
 
-    # def __test01():
-    #     # ---------------------------------------------------------------------
-    #     # Function decoration
-    #     @Observable
-    #     def dog(act: str = "Woof!"):
-    #         """A dog function"""
-    #         print(f"{dog.__name__} acts '{act}'")
-    #
-    #     @Observer(observables=X(dog, 'Roar!'))
-    #     @Observable
-    #     def cat(act: str = "Meow!"):
-    #         """A cat function"""
-    #         print(f"{cat.__name__} acts '{act}'")
-    #
-    #     @Observer(observables=[X(dog, 'Hey, dog!'),
-    #                            X(cat.substitute.callee, say='Hey, cat!')])
-    #     def person(say: str = "Hello?"):
-    #         """A person function"""
-    #         print(f"{person.__name__} says '{say}'")
-    #
-    #     # Some Actions
-    #     print("Calling person:")
-    #     person()
-    #     print("\nCalling cat:")
-    #     cat()
-    #     print("\nCalling dog:")
-    #     dog()
-    #
-    #
-    # def __test02():
-    #     # ---------------------------------------------------------------------
-    #     # Class decoration (static)
-    #     class Agent:
-    #         """An agent"""
-    #
-    #         @classmethod
-    #         def inform(cls, value):
-    #             """Informer"""
-    #             print(f"Informed value is: {value}")
-    #
-    #         # noinspection PyMethodMayBeStatic
-    #         def report(self, value):
-    #             """Reporter"""
-    #             print(f"Reported value is: {value}")
-    #
-    #     class Actor:
-    #         """An actor"""
-    #
-    #         def __init__(self):
-    #             self.a = 1
-    #             print(f"Initialization: a = {self.a}")
-    #             self.modify = Observable(observers=[
-    #                 F(Agent.inform, 'unknown'),
-    #                 F(Agent().report, 'undef')],
-    #                 activate=Activation.NONE)(self.modify)
-    #
-    #         def modify(self, value=1):
-    #             """Modification"""
-    #             self.a += value
-    #             print(f"Modification  : a = {self.a}")
-    #             self.modify.observable.dispatch(value=value)
-    #
-    #     # Some Actions
-    #     a = Actor()
-    #     a.modify(13)
-    #
+
     #
     # def __test03():
     #     # ---------------------------------------------------------------------
     #     # Class decoration (dynamic)
     #     class DftFormatter:
     #         """Default Formatter"""
     #
@@ -1014,12 +1009,14 @@
     #     print(df.set_data.observable.observers())
     #
     #
     # # -------------------------------------------------------------------------
     # # Apply tests
     # print("----------")
     # __test01()
+
     # print("----------")
     # __test02()
     # print("----------")
     # __test03()
     # print("----------")
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `decoratory-0.1.0.3/Sources/decoratory/singleton.py` & `decoratory-0.1.1.3/Sources/decoratory/singleton.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     Attributes
     ----------
         None.
 
     Methods
     -------
     get_instance():
-        Return the singleton instantce. (if accessible=True)
+        Return the singleton instance.  (if accessible=True)
 
     reset():
         Resets the singleton instance.  (if resettable=True)
 
     Example
     -------
 
@@ -32,60 +32,60 @@
         def __init__(self, name):
             self.name = name
 
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.name}')"
 
     # Create Instances
-    a = Animal(name='Bello')        # Creates Bello
-    b = Animal(name='Tessa')        # Returns Bello
+    a = Animal(name='Teddy')        # Creates Teddy
+    b = Animal(name='Roxie')        # Returns Teddy
 
     # Case 1: Static decoration using @Singleton or @Singleton()
     #    ---> One single object instance fits all.
-    print(f"a = {a}")               # a = Animal('Bello')
-    print(f"b = {b}")               # b = Animal('Bello')
+    print(f"a = {a}")               # a = Animal('Teddy')
+    print(f"b = {b}")               # b = Animal('Teddy')
     print(f"a is b: {a is b}")      # a is b: True
     print(f"a == b: {a == b}")      # a == b: True
 
     # Case 2: Dynamic decoration providing extra initial default values
     #    ---> Initial default values provided via the decorator
-    Animal = Singleton(Animal, 'Bello')
-    Animal()                        # Using the decorator's default 'Bello'
-    a = Animal(name='Tessa')        # Returns Bello
-    print(a)                        # Animal('Bello')
+    Animal = Singleton(Animal, 'Teddy')
+    Animal()                        # Using the decorator's default 'Teddy'
+    a = Animal(name='Roxie')        # Returns Teddy
+    print(a)                        # Animal('Teddy')
 
     # Case 3: Decoration using @Singleton(resettable=True)
-    print(Animal(name='Bello'))     # Animal('Bello')
-    print(Animal(name='Tessa'))     # Animal('Bello')   (=primary instance)
+    print(Animal(name='Teddy'))     # Animal('Teddy')
+    print(Animal(name='Roxie'))     # Animal('Teddy')   (=primary instance)
     Animal.reset()                  # Reset the singleton
-    print(Animal(name='Tessa'))     # Animal('Tessa')
-    print(Animal(name='Bello'))     # Animal('Tessa')   (=primary instance)
+    print(Animal(name='Roxie'))     # Animal('Roxie')
+    print(Animal(name='Teddy'))     # Animal('Roxie')   (=primary instance)
 
     # Case 4: Decoration using @Singleton(accessible=True)
-    a = Animal(name='Bello')        # Animal('Bello')
-    b = Animal.get_instance()       # Animal('Bello')   (=primary instance)
-    print(a)                        # Animal('Bello')
-    print(b)                        # Animal('Bello')
+    a = Animal(name='Teddy')        # Animal('Teddy')
+    b = Animal.get_instance()       # Animal('Teddy')   (=primary instance)
+    print(a)                        # Animal('Teddy')
+    print(b)                        # Animal('Teddy')
 """
 
 # -----------------------------------------------------------------------------
 # Module Level Dunders
 __title__ = "Singleton"
 __module__ = "singleton.py"
 __author__ = "Martin Abel"
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.0.4"
-__date__ = "2023-06-15"
-__time__ = "18:24:13"
+__version__ = "0.1.1.1"
+__date__ = "2023-06-16"
+__time__ = "09:40:57"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Singleton"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
@@ -105,15 +105,15 @@
 
     Attributes
     ----------
         None.
 
     Methods
     -------
-        get_instance(): Return the singleton instantce, (if accessible=True)
+        get_instance(): Return the singleton instance.  (if accessible=True)
         reset(): Resets the singleton instance.         (if resettable=True)
 
     Example
     -------
 
     from decoratory.singleton import Singleton
 
@@ -122,43 +122,43 @@
         def __init__(self, name):
             self.name = name
 
         def __repr__(self):
             return f"{self.__class__.__name__}('{self.name}')"
 
     # Create Instances
-    a = Animal(name='Bello')        # Creates Bello
-    b = Animal(name='Tessa')        # Returns Bello
+    a = Animal(name='Teddy')        # Creates Teddy
+    b = Animal(name='Roxie')        # Returns Teddy
 
     # Case 1: Static decoration using @Singleton or @Singleton()
     #    ---> One single object instance fits all.
-    print(f"a = {a}")               # a = Animal('Bello')
-    print(f"b = {b}")               # b = Animal('Bello')
+    print(f"a = {a}")               # a = Animal('Teddy')
+    print(f"b = {b}")               # b = Animal('Teddy')
     print(f"a is b: {a is b}")      # a is b: True
     print(f"a == b: {a == b}")      # a == b: True
 
     # Case 2: Dynamic decoration providing extra initial default values
     #    ---> Initial default values provided via the decorator
-    Animal = Singleton(Animal, 'Bello')
-    Animal()                        # Using the decorator's default 'Bello'
-    a = Animal(name='Tessa')        # Returns Bello
-    print(a)                        # Animal('Bello')
+    Animal = Singleton(Animal, 'Teddy')
+    Animal()                        # Using the decorator's default 'Teddy'
+    a = Animal(name='Roxie')        # Returns Teddy
+    print(a)                        # Animal('Teddy')
 
     # Case 3: Decoration using @Singleton(resettable=True)
-    print(Animal(name='Bello'))     # Animal('Bello')
-    print(Animal(name='Tessa'))     # Animal('Bello')   (=primary instance)
+    print(Animal(name='Teddy'))     # Animal('Teddy')
+    print(Animal(name='Roxie'))     # Animal('Teddy')   (=primary instance)
     Animal.reset()                  # Reset the singleton
-    print(Animal(name='Tessa'))     # Animal('Tessa')
-    print(Animal(name='Bello'))     # Animal('Tessa')   (=primary instance)
+    print(Animal(name='Roxie'))     # Animal('Roxie')
+    print(Animal(name='Teddy'))     # Animal('Roxie')   (=primary instance)
 
     # Case 4: Decoration using @Singleton(accessible=True)
-    a = Animal(name='Bello')        # Animal('Bello')
-    b = Animal.get_instance()       # Animal('Bello')   (=primary instance)
-    print(a)                        # Animal('Bello')
-    print(b)                        # Animal('Bello')
+    a = Animal(name='Teddy')        # Animal('Teddy')
+    b = Animal.get_instance()       # Animal('Teddy')   (=primary instance)
+    print(a)                        # Animal('Teddy')
+    print(b)                        # Animal('Teddy')
     """
 
     def __init__(self,
                  substitute: object = None,
                  *args: object,
                  accessible: bool = False,
                  resettable: bool = False,
@@ -193,24 +193,25 @@
                 """Define reset method"""
                 s.__instance = None
 
             # Add the reset method
             setattr(self, 'reset', reset)
 
         # --- Decorator Arguments Pattern (1/2)
-        if self.__substitute is not None:
+        if self.__get__substitute() is not None:
             # Decoration without parameter(s)
-            self.__set__substitute(F(self.__substitute, *args, **kwargs))
+            self.__set__substitute(
+                F(self.__get__substitute(), *args, **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
 
     def __call__(self, *args, **kwargs):
         """Apply the decorator."""
 
         # --- Decorator Arguments Pattern (2/2)
-        if self.__substitute is None:
+        if self.__get__substitute() is None:
             # Decoration with parameter(s)
             self.__set__substitute(F(args[0], *args[1:], **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
             return self
         else:  # *** Wrapper ***
             # Create and store new or return existing instance
             if self.__instance is None:
```

### Comparing `decoratory-0.1.0.3/Sources/decoratory/wrapper.py` & `decoratory-0.1.1.3/Sources/decoratory/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     # Case 4: Decoration of a class always refers to __init__
     @Wrapper(before=F(print, "BEFORE init"), after=F(print, "AFTER init"))
     class Animal:
         def __init__(self, name):
             self.name = name
             print("RUNNING init")
 
-    a = Animal(name='Bello')        # BEFORE init
+    a = Animal(name='Teddy')        # BEFORE init
                                     # RUNNING init
                                     # AFTER init
 
     # Case 5: Define a private wrapper library
     before_wrapper = Wrapper(before=F(print, "BEFORE"))
     after_wrapper = Wrapper(after=F(print, "AFTER"))
 
@@ -125,17 +125,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.0.3"
-__date__ = "2023-06-15"
-__time__ = "18:24:13"
+__version__ = "0.1.1.1"
+__date__ = "2023-06-16"
+__time__ = "09:40:57"
 __state__ = "Beta"
 __license__ = "PSF"
 
 __all__ = ["Wrapper"]
 
 # -----------------------------------------------------------------------------
 # Libraries & Modules
@@ -237,15 +237,15 @@
     # Case 4: Decoration of a class always refers to __init__
     @Wrapper(before=F(print, "BEFORE init"), after=F(print, "AFTER init"))
     class Animal:
         def __init__(self, name):
             self.name = name
             print("RUNNING init")
 
-    a = Animal(name='Bello')        # BEFORE init
+    a = Animal(name='Teddy')        # BEFORE init
                                     # RUNNING init
                                     # AFTER init
 
     # Case 5: Define a private wrapper library
     before_wrapper = Wrapper(before=F(print, "BEFORE"))
     after_wrapper = Wrapper(after=F(print, "AFTER"))
 
@@ -280,59 +280,60 @@
         """
         self.__set__substitute(substitute)
         self.__set__before(before)
         self.__set__replace(replace)
         self.__set__after(after)
 
         # --- Decorator Arguments Pattern (1/2)
-        if self.__substitute is not None:
+        if self.__get__substitute() is not None:
             # Decoration without parameter(s)
-            self.__set__substitute(F(self.__substitute, *args, **kwargs))
+            self.__set__substitute(
+                F(self.__get__substitute(), *args, **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
 
     def __call__(self, *args, **kwargs):
         # --- Decorator Arguments Pattern (2/2)
-        if self.__substitute is None:
+        if self.__get__substitute() is None:
             # Decoration with parameter(s)
             self.__set__substitute(F(args[0], *args[1:], **kwargs))
             update_wrapper(self, self.__get__substitute().callee, updated=())
             return self
         else:  # *** Wrapper ***
             # Action BEFORE
-            if self.__before:
-                for before in self.__before:
+            if self.__get__before():
+                for before in self.__get__before():
                     before.eval()
 
             # Delegation vs. REPLACE
-            if self.__replace:
+            if self.__get__replace():
                 # Replacement
                 result = None
                 if args or kwargs:
-                    for replace in self.__replace:
+                    for replace in self.__get__replace():
                         d = replace.callee.__kwdefaults__
                         if d and 'result' in d:
                             d['result'] = result
                         result = F(replace.callee, *args, **kwargs).eval()
                 else:
-                    for replace in self.__replace:
+                    for replace in self.__get__replace():
                         d = replace.callee.__kwdefaults__
                         if d and 'result' in d:
                             d['result'] = result
                         result = replace.eval()
             else:
                 # Delegation
                 if args or kwargs:
                     result = F(self.__get__substitute().callee, *args,
                                **kwargs).eval()
                 else:
                     result = self.__get__substitute().eval()
 
             # Action AFTER
-            if self.__after:
-                for after in self.__after:
+            if self.__get__after():
+                for after in self.__get__after():
                     after.eval()
 
             return result
 
     # Getter, Setter, Properties
     def __get__substitute(self):
         return self.__substitute
```

### Comparing `decoratory-0.1.0.3/setup.py` & `decoratory-0.1.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 __maintainer__ = "Martin Abel"
 __credits__ = ["Martin Abel"]
 __company__ = "eVation"
 __email__ = "python@evation.eu"
 __url__ = "http://evation.eu"
 __copyright__ = f"(c) copyright 2020-2023, {__company__}"
 __created__ = "2020-01-01"
-__version__ = "0.1.0.3"
-__date__ = "2023-06-15"
-__time__ = "18:35:51"
+__version__ = "0.1.1.3"
+__date__ = "2023-06-16"
+__time__ = "20:01:41"
 __state__ = "Beta"
 __license__ = "PSF"
 
 # -----------------------------------------------------------------------------
 # Libraries
 from os.path import join
 from setuptools import setup, find_packages
```

