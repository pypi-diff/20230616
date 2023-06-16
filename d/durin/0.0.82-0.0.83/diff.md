# Comparing `tmp/durin-0.0.82.tar.gz` & `tmp/durin-0.0.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "durin-0.0.82.tar", last modified: Wed Jun 14 13:31:10 2023, max compression
+gzip compressed data, was "durin-0.0.83.tar", last modified: Fri Jun 16 14:08:22 2023, max compression
```

## Comparing `durin-0.0.82.tar` & `durin-0.0.83.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:31:10.546093 durin-0.0.82/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-14 13:31:00.000000 durin-0.0.82/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-14 13:31:10.546093 durin-0.0.82/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2683 2023-06-14 13:31:00.000000 durin-0.0.82/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:31:10.538092 durin-0.0.82/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)       34 2023-06-14 13:31:00.000000 durin-0.0.82/bin/durin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:31:10.542093 durin-0.0.82/durin/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-14 13:31:00.000000 durin-0.0.82/durin/Profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-14 13:31:00.000000 durin-0.0.82/durin/Read_profilers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-06-14 13:31:00.000000 durin-0.0.82/durin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-06-14 13:31:00.000000 durin-0.0.82/durin/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-06-14 13:31:00.000000 durin-0.0.82/durin/actuator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4148 2023-06-14 13:31:00.000000 durin-0.0.82/durin/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:31:10.542093 durin-0.0.82/durin/controller/
--rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-06-14 13:31:00.000000 durin-0.0.82/durin/controller/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-06-14 13:31:00.000000 durin-0.0.82/durin/controller/dvs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4307 2023-06-14 13:31:00.000000 durin-0.0.82/durin/controller/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:31:10.542093 durin-0.0.82/durin/controller/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:31:00.000000 durin-0.0.82/durin/controller/test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      947 2023-06-14 13:31:00.000000 durin-0.0.82/durin/controller/test/test_stream.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4694 2023-06-14 13:31:00.000000 durin-0.0.82/durin/durin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   181742 2023-06-14 13:31:00.000000 durin-0.0.82/durin/durin_birdseye.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)      504 2023-06-14 13:31:00.000000 durin-0.0.82/durin/dvs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:31:10.542093 durin-0.0.82/durin/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-14 13:31:00.000000 durin-0.0.82/durin/examples/CPU_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 13:31:00.000000 durin-0.0.82/durin/examples/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2281 2023-06-14 13:31:00.000000 durin-0.0.82/durin/examples/braitenberg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2631 2023-06-14 13:31:00.000000 durin-0.0.82/durin/examples/commands.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1448 2023-06-14 13:31:00.000000 durin-0.0.82/durin/examples/dashboard.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      923 2023-06-14 13:31:00.000000 durin-0.0.82/durin/examples/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-14 13:31:00.000000 durin-0.0.82/durin/examples/plot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      589 2023-06-14 13:31:00.000000 durin-0.0.82/durin/examples/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-14 13:31:00.000000 durin-0.0.82/durin/examples/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:31:10.546093 durin-0.0.82/durin/io/
--rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-06-14 13:31:00.000000 durin-0.0.82/durin/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-14 13:31:00.000000 durin-0.0.82/durin/io/command.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1418 2023-06-14 13:31:00.000000 durin-0.0.82/durin/io/gamepad.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6181 2023-06-14 13:31:00.000000 durin-0.0.82/durin/io/network.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-06-14 13:31:00.000000 durin-0.0.82/durin/io/ringbuffer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-06-14 13:31:00.000000 durin-0.0.82/durin/io/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-06-14 13:31:00.000000 durin-0.0.82/durin/io/schema.capnp
--rwxr-xr-x   0 runner    (1001) docker     (123)     7102 2023-06-14 13:31:00.000000 durin-0.0.82/durin/sensor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15983 2023-06-14 13:31:00.000000 durin-0.0.82/durin/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 13:31:10.542093 durin-0.0.82/durin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-14 13:31:10.000000 durin-0.0.82/durin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-14 13:31:10.000000 durin-0.0.82/durin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 13:31:10.000000 durin-0.0.82/durin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-14 13:31:10.000000 durin-0.0.82/durin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 13:31:10.000000 durin-0.0.82/durin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 13:31:10.546093 durin-0.0.82/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      663 2023-06-14 13:31:00.000000 durin-0.0.82/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:08:22.716153 durin-0.0.83/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-16 14:08:12.000000 durin-0.0.83/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-16 14:08:22.716153 durin-0.0.83/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2683 2023-06-16 14:08:12.000000 durin-0.0.83/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:08:22.708152 durin-0.0.83/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       34 2023-06-16 14:08:12.000000 durin-0.0.83/bin/durin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:08:22.712152 durin-0.0.83/durin/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-16 14:08:12.000000 durin-0.0.83/durin/Profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-16 14:08:12.000000 durin-0.0.83/durin/Read_profilers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-06-16 14:08:12.000000 durin-0.0.83/durin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-06-16 14:08:12.000000 durin-0.0.83/durin/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-06-16 14:08:12.000000 durin-0.0.83/durin/actuator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4148 2023-06-16 14:08:12.000000 durin-0.0.83/durin/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:08:22.712152 durin-0.0.83/durin/controller/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-06-16 14:08:12.000000 durin-0.0.83/durin/controller/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-06-16 14:08:12.000000 durin-0.0.83/durin/controller/dvs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4307 2023-06-16 14:08:12.000000 durin-0.0.83/durin/controller/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:08:22.712152 durin-0.0.83/durin/controller/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:08:12.000000 durin-0.0.83/durin/controller/test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      947 2023-06-16 14:08:12.000000 durin-0.0.83/durin/controller/test/test_stream.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4694 2023-06-16 14:08:12.000000 durin-0.0.83/durin/durin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   181742 2023-06-16 14:08:12.000000 durin-0.0.83/durin/durin_birdseye.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      504 2023-06-16 14:08:12.000000 durin-0.0.83/durin/dvs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:08:22.712152 durin-0.0.83/durin/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-16 14:08:12.000000 durin-0.0.83/durin/examples/CPU_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:08:12.000000 durin-0.0.83/durin/examples/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2281 2023-06-16 14:08:12.000000 durin-0.0.83/durin/examples/braitenberg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2631 2023-06-16 14:08:12.000000 durin-0.0.83/durin/examples/commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1448 2023-06-16 14:08:12.000000 durin-0.0.83/durin/examples/dashboard.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      923 2023-06-16 14:08:12.000000 durin-0.0.83/durin/examples/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-16 14:08:12.000000 durin-0.0.83/durin/examples/plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      589 2023-06-16 14:08:12.000000 durin-0.0.83/durin/examples/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-16 14:08:12.000000 durin-0.0.83/durin/examples/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:08:22.716153 durin-0.0.83/durin/io/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-06-16 14:08:12.000000 durin-0.0.83/durin/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-16 14:08:12.000000 durin-0.0.83/durin/io/command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1418 2023-06-16 14:08:12.000000 durin-0.0.83/durin/io/gamepad.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6181 2023-06-16 14:08:12.000000 durin-0.0.83/durin/io/network.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-06-16 14:08:12.000000 durin-0.0.83/durin/io/ringbuffer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-06-16 14:08:12.000000 durin-0.0.83/durin/io/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-06-16 14:08:12.000000 durin-0.0.83/durin/io/schema.capnp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7102 2023-06-16 14:08:12.000000 durin-0.0.83/durin/sensor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16014 2023-06-16 14:08:12.000000 durin-0.0.83/durin/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:08:22.712152 durin-0.0.83/durin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-16 14:08:22.000000 durin-0.0.83/durin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-16 14:08:22.000000 durin-0.0.83/durin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 14:08:22.000000 durin-0.0.83/durin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-16 14:08:22.000000 durin-0.0.83/durin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-16 14:08:22.000000 durin-0.0.83/durin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 14:08:22.716153 durin-0.0.83/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      663 2023-06-16 14:08:12.000000 durin-0.0.83/setup.py
```

### Comparing `durin-0.0.82/PKG-INFO` & `durin-0.0.83/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durin
-Version: 0.0.82
+Version: 0.0.83
 Summary: Python control interface for the Durin robot
 Maintainer: Jens E. Pedersen
 Maintainer-email: jeped@kth.se
 License: LGPLv3
 Description-Content-Type: text/markdown
 Provides-Extra: aestream
```

### Comparing `durin-0.0.82/README.md` & `durin-0.0.83/README.md`

 * *Files identical despite different names*

### Comparing `durin-0.0.82/durin/actuator.py` & `durin-0.0.83/durin/actuator.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.82/durin/cli.py` & `durin-0.0.83/durin/cli.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.82/durin/controller/server.py` & `durin-0.0.83/durin/controller/server.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.82/durin/controller/test/test_stream.py` & `durin-0.0.83/durin/controller/test/test_stream.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.82/durin/durin.py` & `durin-0.0.83/durin/durin.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.82/durin/durin_birdseye.jpg` & `durin-0.0.83/durin/durin_birdseye.jpg`

 * *Files identical despite different names*

### Comparing `durin-0.0.82/durin/examples/braitenberg.py` & `durin-0.0.83/durin/examples/braitenberg.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.82/durin/examples/commands.py` & `durin-0.0.83/durin/examples/commands.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.82/durin/examples/dashboard.py` & `durin-0.0.83/durin/examples/dashboard.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.82/durin/examples/main.py` & `durin-0.0.83/durin/examples/main.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.82/durin/examples/plot.py` & `durin-0.0.83/durin/examples/plot.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.82/durin/examples/record.py` & `durin-0.0.83/durin/examples/record.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.82/durin/examples/stats.py` & `durin-0.0.83/durin/examples/stats.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.82/durin/io/__init__.py` & `durin-0.0.83/durin/io/__init__.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.82/durin/io/command.py` & `durin-0.0.83/durin/io/command.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.82/durin/io/gamepad.py` & `durin-0.0.83/durin/io/gamepad.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.82/durin/io/network.py` & `durin-0.0.83/durin/io/network.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.82/durin/io/ringbuffer.py` & `durin-0.0.83/durin/io/ringbuffer.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.82/durin/io/runnable.py` & `durin-0.0.83/durin/io/runnable.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.82/durin/io/schema.capnp` & `durin-0.0.83/durin/io/schema.capnp`

 * *Files identical despite different names*

### Comparing `durin-0.0.82/durin/sensor.py` & `durin-0.0.83/durin/sensor.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.82/durin/ui.py` & `durin-0.0.83/durin/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,26 +83,26 @@
         self.clock = pygame.time.Clock()
 
         # Gamepad
         pygame.joystick.init()
 
         if pygame.joystick.get_count() == 0:
             print("No gamepad found.")
-            return
+            gamepad_found = False
+        else:
+            gamepad_found = True
+            self.gamepad = pygame.joystick.Joystick(0)
+            self.gamepad.init()
+            print("Gamepad found:", self.gamepad.get_name())
 
-        self.gamepad = pygame.joystick.Joystick(0)
-        self.gamepad.init()
-
-        print("Gamepad found:", self.gamepad.get_name())
 
 
         # Set up the display
         info = pygame.display.Info() # Get screen size
         self.screen_width, self.screen_height = info.current_w, info.current_h-50
-        print("WIDTH", self.screen_width)
 
         self.font = pygame.font.SysFont(None, round(self.screen_width/70))
         self.big_font = pygame.font.SysFont(None, 60)
 
 
         self.screen = pygame.display.set_mode((0, 0), pygame.RESIZABLE)
 
@@ -182,19 +182,19 @@
                 if event.key == pygame.K_LEFT or event.key == pygame.K_d or event.key == pygame.K_RIGHT or event.key == pygame.K_a:
                     self.horizontal = 0
                 if event.key == pygame.K_e or event.key == pygame.K_q:
                     self.rot = 0
 
             # Gamepad
             if event.type == pygame.JOYAXISMOTION: 
-                if event.axis == 2:
+                if event.axis == 1:
                     self.vertical = event.value * 500/0.8
-                elif event.axis == 3:
-                    self.horizontal = event.value * 500/0.8
                 elif event.axis == 0:
+                    self.horizontal = event.value * 500/0.8
+                elif event.axis == 3:
                     self.rot = event.value * -500/0.8
 
                 # If the input is close to 0, round to 0. It is very difficult to have the joystick exactly in the middle.
                 self.vertical = 0 if abs(self.vertical) < 50 else self.vertical
                 self.horizontal = 0 if abs(self.horizontal) < 50 else self.horizontal 
                 self.rot = 0 if abs(self.rot) < 50 else self.rot
```

### Comparing `durin-0.0.82/durin.egg-info/PKG-INFO` & `durin-0.0.83/durin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durin
-Version: 0.0.82
+Version: 0.0.83
 Summary: Python control interface for the Durin robot
 Maintainer: Jens E. Pedersen
 Maintainer-email: jeped@kth.se
 License: LGPLv3
 Description-Content-Type: text/markdown
 Provides-Extra: aestream
```

### Comparing `durin-0.0.82/durin.egg-info/SOURCES.txt` & `durin-0.0.83/durin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `durin-0.0.82/setup.py` & `durin-0.0.83/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = fp.read().split("\n")
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
 
 setup(
     name="durin",
-    version="0.0.82",
+    version="0.0.83",
     install_requires=requirements,
     packages=find_packages(),
     license="LGPLv3",
     maintainer="Jens E. Pedersen",
     maintainer_email="jeped@kth.se",
     extras_require={"aestream": ["aestream"]},
     scripts=["bin/durin"],
```

