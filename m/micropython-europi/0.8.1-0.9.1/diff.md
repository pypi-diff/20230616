# Comparing `tmp/micropython-europi-0.8.1.tar.gz` & `tmp/micropython-europi-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-europi-0.8.1.tar", last modified: Sat Mar 25 16:17:24 2023, max compression
+gzip compressed data, was "micropython-europi-0.9.1.tar", last modified: Fri Jun 16 14:15:00 2023, max compression
```

## Comparing `micropython-europi-0.8.1.tar` & `micropython-europi-0.9.1.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 16:17:24.181214 micropython-europi-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (122)      464 2023-03-25 16:17:24.181214 micropython-europi-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-03-25 16:17:21.000000 micropython-europi-0.8.1/bootloader.py
--rw-r--r--   0 runner    (1001) docker     (122)     3867 2023-03-25 16:17:21.000000 micropython-europi-0.8.1/calibrate.py
--rw-r--r--   0 runner    (1001) docker     (122)     7634 2023-03-25 16:17:21.000000 micropython-europi-0.8.1/configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)    24109 2023-03-25 16:17:21.000000 micropython-europi-0.8.1/europi.py
--rw-r--r--   0 runner    (1001) docker     (122)      785 2023-03-25 16:17:21.000000 micropython-europi-0.8.1/europi_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    11470 2023-03-25 16:17:21.000000 micropython-europi-0.8.1/europi_script.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 16:17:24.181214 micropython-europi-0.8.1/experimental/
--rw-r--r--   0 runner    (1001) docker     (122)      578 2023-03-25 16:17:21.000000 micropython-europi-0.8.1/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13067 2023-03-25 16:17:21.000000 micropython-europi-0.8.1/experimental/knobs.py
--rw-r--r--   0 runner    (1001) docker     (122)      711 2023-03-25 16:17:21.000000 micropython-europi-0.8.1/file_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 16:17:24.181214 micropython-europi-0.8.1/micropython_europi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      464 2023-03-25 16:17:23.000000 micropython-europi-0.8.1/micropython_europi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      342 2023-03-25 16:17:24.000000 micropython-europi-0.8.1/micropython_europi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-25 16:17:23.000000 micropython-europi-0.8.1/micropython_europi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      105 2023-03-25 16:17:23.000000 micropython-europi-0.8.1/micropython_europi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-25 16:17:24.181214 micropython-europi-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-03-25 16:17:21.000000 micropython-europi-0.8.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     2092 2023-03-25 16:17:21.000000 micropython-europi-0.8.1/ui.py
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-03-25 16:17:21.000000 micropython-europi-0.8.1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:15:00.685384 micropython-europi-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      464 2023-06-16 14:15:00.685384 micropython-europi-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4784 2023-06-16 14:14:58.000000 micropython-europi-0.9.1/bootloader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3867 2023-06-16 14:14:58.000000 micropython-europi-0.9.1/calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7634 2023-06-16 14:14:58.000000 micropython-europi-0.9.1/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24542 2023-06-16 14:14:58.000000 micropython-europi-0.9.1/europi.py
+-rw-r--r--   0 runner    (1001) docker     (122)      785 2023-06-16 14:14:58.000000 micropython-europi-0.9.1/europi_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11470 2023-06-16 14:14:58.000000 micropython-europi-0.9.1/europi_script.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:15:00.685384 micropython-europi-0.9.1/experimental/
+-rw-r--r--   0 runner    (1001) docker     (122)      578 2023-06-16 14:14:58.000000 micropython-europi-0.9.1/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3011 2023-06-16 14:14:58.000000 micropython-europi-0.9.1/experimental/euclid.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13067 2023-06-16 14:14:58.000000 micropython-europi-0.9.1/experimental/knobs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6725 2023-06-16 14:14:58.000000 micropython-europi-0.9.1/experimental/quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1569 2023-06-16 14:14:58.000000 micropython-europi-0.9.1/experimental/screensaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-06-16 14:14:58.000000 micropython-europi-0.9.1/file_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:15:00.685384 micropython-europi-0.9.1/micropython_europi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      464 2023-06-16 14:15:00.000000 micropython-europi-0.9.1/micropython_europi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      419 2023-06-16 14:15:00.000000 micropython-europi-0.9.1/micropython_europi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 14:15:00.000000 micropython-europi-0.9.1/micropython_europi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2023-06-16 14:15:00.000000 micropython-europi-0.9.1/micropython_europi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 14:15:00.685384 micropython-europi-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-06-16 14:14:58.000000 micropython-europi-0.9.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2092 2023-06-16 14:14:58.000000 micropython-europi-0.9.1/ui.py
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-16 14:14:58.000000 micropython-europi-0.9.1/version.py
```

### Comparing `micropython-europi-0.8.1/bootloader.py` & `micropython-europi-0.9.1/bootloader.py`

 * *Files identical despite different names*

### Comparing `micropython-europi-0.8.1/calibrate.py` & `micropython-europi-0.9.1/calibrate.py`

 * *Files identical despite different names*

### Comparing `micropython-europi-0.8.1/configuration.py` & `micropython-europi-0.9.1/configuration.py`

 * *Files identical despite different names*

### Comparing `micropython-europi-0.8.1/europi.py` & `micropython-europi-0.9.1/europi.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,20 +88,29 @@
 
 
 def clamp(value, low, high):
     """Returns a value that is no lower than 'low' and no higher than 'high'."""
     return max(min(value, high), low)
 
 
+def turn_off_all_cvs():
+    """Calls cv.off() for every cv in cvs. This is done commonly enough in
+    contrib scripts that a function seems useful.
+    """
+    for cv in cvs:
+        cv.off()
+
+
 def reset_state():
     """Return device to initial state with all components off and handlers reset."""
     if not TEST_ENV:
         oled.fill(0)
-    [cv.off() for cv in cvs]
-    [d.reset_handler() for d in (b1, b2, din)]
+    turn_off_all_cvs()
+    for d in (b1, b2, din):
+        d.reset_handler()
 
 
 def bootsplash():
     """Display the EuroPi version when booting."""
     image = b"\x00\x00\x00\x01\xf0\x00\x00\x00\x00\x00\x00\x00\x03\x00\x00\x00\x00\x00\x00\x02\x08\x00\x00\x00\x00\x00\x00\x00\x03\x00\x00\x00\x00\x00\x00\x04\x04\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x03\xc4\x04\x00\x18\x00\x00\x00p\x07\x00\x00\x00\x00\x00\x00\x0c$\x02\x00~\x0c\x18\xb9\x8c8\xc3\x00\x00\x00\x00\x00\x10\x14\x01\x00\xc3\x0c\x18\xc3\x060c\x00\x00\x00\x00\x00\x10\x0b\xc0\x80\x81\x8c\x18\xc2\x020#\x00\x00\x00\x00\x00 \x04\x00\x81\x81\x8c\x18\x82\x02 #\x00\x00\x00\x00\x00A\x8a|\x81\xff\x0c\x18\x82\x02 #\x00\x00\x00\x00\x00FJC\xc1\x80\x0c\x18\x82\x02 #\x00\x00\x00\x00\x00H\x898\x00\x80\x0c\x18\x83\x060c\x00\x00\x00\x00\x00S\x08\x87\x00\xc3\x060\x81\x8c8\xc3\x00\x00\x00\x00\x00d\x08\x00\xc0<\x01\xc0\x80p7\x03\x00\x00\x00\x00\x00X\x08p \x00\x00\x00\x00\x000\x00\x00\x00\x00\x00\x00#\x88H \x00\x00\x00\x00\x000\x00\x00\x00\x00\x00\x00L\xb8& \x00\x00\x00\x00\x000\x00\x00\x00\x00\x00\x00\x91P\x11 \x00\x00\x00\x00\x000\x00\x00\x00\x00\x00\x00\xa6\x91\x08\xa0\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\xc9\x12\x84`\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x12\x12C\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00$\x11 \x80\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00H\x0c\x90\x80\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00@\x12\x88\x80\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00 \x12F\x80\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x10\x10A\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x10  \x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x08  \x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x04@@\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x02\x00\x80\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x01\x01\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\xc6\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x008\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00"
     TH = bytearray(image)
     fb = FrameBuffer(TH, 128, 32, MONO_HLSB)
@@ -189,14 +198,18 @@
     The functions all take an optional parameter of ``samples``, which will
     oversample the ADC and then take an average, which will take more time per
     reading, but will give you a statistically more accurate result. The
     default is 32, provides a balance of performance vs accuracy, but if you
     want to process at the maximum speed you can use as little as 1, and the
     processor won't bog down until you get way up into the thousands if you
     wan't incredibly accurate (but quite slow) readings.
+
+    The percent function takes an optional parameter ``deadzone``. However this
+    parameter is ignored and just present to be compatible with the percent
+    function of the AnalogueReader and Knob classes
     """
 
     def __init__(self, pin, min_voltage=MIN_INPUT_VOLTAGE, max_voltage=MAX_INPUT_VOLTAGE):
         super().__init__(pin)
         self.MIN_VOLTAGE = min_voltage
         self.MAX_VOLTAGE = max_voltage
         self._gradients = []
@@ -205,15 +218,15 @@
                 self._gradients.append(1 / (INPUT_CALIBRATION_VALUES[index + 1] - value))
             except ZeroDivisionError:
                 raise Exception(
                     "The input calibration process did not complete properly. Please complete again with rack power turned on"
                 )
         self._gradients.append(self._gradients[-1])
 
-    def percent(self, samples=None):
+    def percent(self, samples=None, deadzone=None):
         """Current voltage as a relative percentage of the component's range."""
         # Determine the percent value from the max calibration value.
         reading = self._sample_adc(samples) - INPUT_CALIBRATION_VALUES[0]
         max_value = max(
             reading,
             INPUT_CALIBRATION_VALUES[-1] - INPUT_CALIBRATION_VALUES[0],
         )
```

### Comparing `micropython-europi-0.8.1/europi_config.py` & `micropython-europi-0.9.1/europi_config.py`

 * *Files identical despite different names*

### Comparing `micropython-europi-0.8.1/europi_script.py` & `micropython-europi-0.9.1/europi_script.py`

 * *Files identical despite different names*

### Comparing `micropython-europi-0.8.1/experimental/__init__.py` & `micropython-europi-0.9.1/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `micropython-europi-0.8.1/experimental/knobs.py` & `micropython-europi-0.9.1/experimental/knobs.py`

 * *Files identical despite different names*

### Comparing `micropython-europi-0.8.1/file_utils.py` & `micropython-europi-0.9.1/file_utils.py`

 * *Files identical despite different names*

### Comparing `micropython-europi-0.8.1/setup.py` & `micropython-europi-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `micropython-europi-0.8.1/ui.py` & `micropython-europi-0.9.1/ui.py`

 * *Files identical despite different names*

