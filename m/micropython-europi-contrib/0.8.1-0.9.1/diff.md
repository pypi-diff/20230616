# Comparing `tmp/micropython-europi-contrib-0.8.1.tar.gz` & `tmp/micropython-europi-contrib-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-europi-contrib-0.8.1.tar", last modified: Sat Mar 25 16:17:24 2023, max compression
+gzip compressed data, was "micropython-europi-contrib-0.9.1.tar", last modified: Fri Jun 16 14:15:00 2023, max compression
```

## Comparing `micropython-europi-contrib-0.8.1.tar` & `micropython-europi-contrib-0.9.1.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 16:17:24.401208 micropython-europi-contrib-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      364 2023-03-25 16:17:24.401208 micropython-europi-contrib-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 16:17:24.397209 micropython-europi-contrib-0.8.1/contrib/
--rw-r--r--   0 runner    (1001) docker     (122)     9651 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/bernoulli_gates.py
--rw-r--r--   0 runner    (1001) docker     (122)     4213 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/coin_toss.py
--rw-r--r--   0 runner    (1001) docker     (122)    22729 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/consequencer.py
--rw-r--r--   0 runner    (1001) docker     (122)    19449 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/cvecorder.py
--rw-r--r--   0 runner    (1001) docker     (122)     2784 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/diagnostic.py
--rw-r--r--   0 runner    (1001) docker     (122)    15749 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/euclid.py
--rw-r--r--   0 runner    (1001) docker     (122)    12547 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/hamlet.py
--rw-r--r--   0 runner    (1001) docker     (122)     9665 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/harmonic_lfos.py
--rw-r--r--   0 runner    (1001) docker     (122)     1232 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/hello_world.py
--rw-r--r--   0 runner    (1001) docker     (122)     2407 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/knob_playground.py
--rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/logic.py
--rw-r--r--   0 runner    (1001) docker     (122)    17721 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/master_clock.py
--rw-r--r--   0 runner    (1001) docker     (122)     1529 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/menu.py
--rw-r--r--   0 runner    (1001) docker     (122)     3411 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/noddy_holder.py
--rw-r--r--   0 runner    (1001) docker     (122)     4309 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/piconacci.py
--rw-r--r--   0 runner    (1001) docker     (122)    13936 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/poly_square.py
--rw-r--r--   0 runner    (1001) docker     (122)    12275 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/polyrhythmic_sequencer.py
--rw-r--r--   0 runner    (1001) docker     (122)     8850 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/probapoly.py
--rw-r--r--   0 runner    (1001) docker     (122)    20829 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/quantizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3320 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/radio_scanner.py
--rw-r--r--   0 runner    (1001) docker     (122)     4263 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/scope.py
--rw-r--r--   0 runner    (1001) docker     (122)     8568 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/sequential_switch.py
--rw-r--r--   0 runner    (1001) docker     (122)     8266 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/smooth_random_voltages.py
--rw-r--r--   0 runner    (1001) docker     (122)    13721 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/strange_attractor.py
--rw-r--r--   0 runner    (1001) docker     (122)    13098 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/contrib/turing_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 16:17:24.401208 micropython-europi-contrib-0.8.1/firmware/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/firmware/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-25 16:17:24.401208 micropython-europi-contrib-0.8.1/micropython_europi_contrib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      364 2023-03-25 16:17:24.000000 micropython-europi-contrib-0.8.1/micropython_europi_contrib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-03-25 16:17:24.000000 micropython-europi-contrib-0.8.1/micropython_europi_contrib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-25 16:17:24.000000 micropython-europi-contrib-0.8.1/micropython_europi_contrib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-03-25 16:17:24.000000 micropython-europi-contrib-0.8.1/micropython_europi_contrib.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-03-25 16:17:24.000000 micropython-europi-contrib-0.8.1/micropython_europi_contrib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-25 16:17:24.401208 micropython-europi-contrib-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      578 2023-03-25 16:17:21.000000 micropython-europi-contrib-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:15:00.921386 micropython-europi-contrib-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    11340 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      364 2023-06-16 14:15:00.921386 micropython-europi-contrib-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:15:00.921386 micropython-europi-contrib-0.9.1/contrib/
+-rw-r--r--   0 runner    (1001) docker     (122)     9651 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/bernoulli_gates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4190 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/coin_toss.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23482 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/consequencer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19449 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/cvecorder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2784 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/diagnostic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9791 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/envelope_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12096 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/euclid.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12541 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/hamlet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9665 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/harmonic_lfos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1232 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2407 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/knob_playground.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/logic.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16827 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/master_clock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1613 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/menu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3411 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/noddy_holder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    40591 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/pams.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4303 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/piconacci.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13936 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/poly_square.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12305 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/polyrhythmic_sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8850 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/probapoly.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17687 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3320 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/radio_scanner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4263 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/scope.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8210 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/sequential_switch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8266 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/smooth_random_voltages.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13721 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/strange_attractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13098 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/contrib/turing_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:15:00.921386 micropython-europi-contrib-0.9.1/firmware/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/firmware/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:15:00.921386 micropython-europi-contrib-0.9.1/micropython_europi_contrib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      364 2023-06-16 14:15:00.000000 micropython-europi-contrib-0.9.1/micropython_europi_contrib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      938 2023-06-16 14:15:00.000000 micropython-europi-contrib-0.9.1/micropython_europi_contrib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 14:15:00.000000 micropython-europi-contrib-0.9.1/micropython_europi_contrib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-16 14:15:00.000000 micropython-europi-contrib-0.9.1/micropython_europi_contrib.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-06-16 14:15:00.000000 micropython-europi-contrib-0.9.1/micropython_europi_contrib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 14:15:00.921386 micropython-europi-contrib-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      578 2023-06-16 14:14:58.000000 micropython-europi-contrib-0.9.1/setup.py
```

### Comparing `micropython-europi-contrib-0.8.1/LICENSE` & `micropython-europi-contrib-0.9.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2023 Rory Allen
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `micropython-europi-contrib-0.8.1/README.md` & `micropython-europi-contrib-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `micropython-europi-contrib-0.8.1/contrib/bernoulli_gates.py` & `micropython-europi-contrib-0.9.1/contrib/bernoulli_gates.py`

 * *Files identical despite different names*

### Comparing `micropython-europi-contrib-0.8.1/contrib/coin_toss.py` & `micropython-europi-contrib-0.9.1/contrib/coin_toss.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             """Toggle between internal clock and external clock from digital in."""
             self.internal_clock = not self.internal_clock
 
         @b2.handler
         def toggle_gate():
             """Toggle between gate and trigger mode."""
             self.gate_mode = not self.gate_mode
-            [o.off() for o in cvs]
+            turn_off_all_cvs()
 
     def tempo(self):
         """Read the current tempo set by k1 within set range."""
         return round(k1.read_position(MAX_BPM - MIN_BPM) + MIN_BPM)
 
     def get_next_deadline(self):
         """Get the deadline for next clock tick whole note."""
@@ -50,15 +50,15 @@
                     return
         else:  # External clock
             # Loop until digital in goes high (clock pulse received).
             while not self.internal_clock:
                 if din.value() != self._prev_clock:
                     # We've detected a new clock value.
                     self._prev_clock = 1 if self._prev_clock == 0 else 0
-                    # If the previous value was just set to 1 then we are seeing 
+                    # If the previous value was just set to 1 then we are seeing
                     # a high value for the first time, break wait and return.
                     if self._prev_clock == 1:
                         return
 
     def toss(self, a, b, draw=True):
         """If random value is below trigger a, otherwise trigger b.
 
@@ -69,15 +69,15 @@
         read_sum = k2.percent() + ain.read_voltage()/12
         self.threshold = clamp(read_sum, 0, 1)
         if self.gate_mode:
             a.value(coin < self.threshold)
             b.value(coin > self.threshold)
         else:
             (a if coin < self.threshold else b).on()
-        
+
         if not draw:
             return
 
         # Draw gate/trigger display graphics for coin toss
         h = int(self.threshold * OLED_HEIGHT)
         tick = FRAME_WIDTH if self.gate_mode else 1
         offset = 8  # The amount of negative space before drawing gate.
@@ -96,22 +96,23 @@
             oled.fill_rect(0, 0, FRAME_WIDTH, OLED_HEIGHT, 0)
 
             self.toss(cv1, cv2)
             cv3.on()  # First column clock trigger
             if counter % 4 == 0:
                 self.toss(cv4, cv5, False)
                 cv6.on()  # Second column clock trigger (1/4x speed)
-            
+
             sleep_ms(10)
             if self.gate_mode:
                 # Only turn off clock triggers.
-                [o.off() for o in (cv3, cv6)]
+                cv3.off()
+                cv6.off()
             else:
                 # Turn of all cvs in trigger mode.
-                [o.off() for o in cvs]
+                turn_off_all_cvs()
 
             # Draw threshold line
             oled.hline(0, int(self.threshold * OLED_HEIGHT), FRAME_WIDTH, 1)
             oled.show()
 
             counter += 1
             self.wait()
```

### Comparing `micropython-europi-contrib-0.8.1/contrib/consequencer.py` & `micropython-europi-contrib-0.9.1/contrib/consequencer.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,18 +289,34 @@
         return output
 
     def updateScreen(self):
         # oled.clear() - dont use this, it causes the screen to flicker!
         oled.fill(0)
 
         # Show selected pattern visually
-        lpos = 8-(self.step*8)
-        oled.text(self.visualizePattern(self.BD[self.pattern], self.BdProb[self.pattern]), lpos, 0, 1)
-        oled.text(self.visualizePattern(self.SN[self.pattern], self.SnProb[self.pattern]), lpos, 10, 1)
-        oled.text(self.visualizePattern(self.HH[self.pattern], self.HhProb[self.pattern]), lpos, 20, 1)
+        
+        # Calculate the length of the current pattern
+        current_pattern_length = len(self.BD[self.pattern])
+        
+        # Calculate the width of one full pattern in pixels
+        lpos_offset = current_pattern_length * CHAR_WIDTH
+        
+        # Calculate the x position of the first pattern to be drawn
+        normal_lpos = lpos = 8 - (self.step * 8)
+        
+        # Calculate the number of patterns required to fill the OLED width
+        number_of_offset_patterns = 2 * max(int(OLED_WIDTH / lpos_offset), 1)
+        
+        # Draw as many offset patterns as required to fill the OLED
+        for pattern_offset in range(number_of_offset_patterns):
+            # Draw the current pattern
+            oled.text(self.visualizePattern(self.BD[self.pattern], self.BdProb[self.pattern]), normal_lpos, 0, 1)
+            oled.text(self.visualizePattern(self.SN[self.pattern], self.SnProb[self.pattern]), normal_lpos, 10, 1)
+            oled.text(self.visualizePattern(self.HH[self.pattern], self.HhProb[self.pattern]), normal_lpos, 20, 1)
+            normal_lpos += lpos_offset
 
         # If the random toggle is on, show a rectangle
         if self.random_HH:
             oled.fill_rect(0, 29, 10, 3, 1)
 
         # Show self.output4isClock indicator
         if self.output4isClock:
@@ -682,12 +698,12 @@
     HH.append("111")
     BdProb.append("9")
     SnProb.append("9")
     HhProb.append("9")
 
 if __name__ == '__main__':
     # Reset module display state.
-    [cv.off() for cv in cvs]
+    turn_off_all_cvs()
     dm = Consequencer()
     dm.main()
```

### Comparing `micropython-europi-contrib-0.8.1/contrib/cvecorder.py` & `micropython-europi-contrib-0.9.1/contrib/cvecorder.py`

 * *Files identical despite different names*

### Comparing `micropython-europi-contrib-0.8.1/contrib/diagnostic.py` & `micropython-europi-contrib-0.9.1/contrib/diagnostic.py`

 * *Files identical despite different names*

### Comparing `micropython-europi-contrib-0.8.1/contrib/euclid.py` & `micropython-europi-contrib-0.9.1/contrib/euclid.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,162 +8,83 @@
 This script contains code released under the MIT license, as
 noted below
 """
 
 from europi import *
 from europi_script import EuroPiScript
 
+from experimental.euclid import generate_euclidean_pattern
+from experimental.screensaver import Screensaver
+
 import random
 import time
 
 ## Duration before we blank the screen
 SCREENSAVER_TIMEOUT_MS = 1000 * 60 * 20
 
-def generate_euclidean_pattern(steps, pulses, rot=0):
-    """Generates an array indicating the on/off steps of Euclid(k, n)
-
-    Copied from https://github.com/brianhouse/bjorklund with all due gratitude
-
-    @param steps  The number of steps in the pattern
-    @param pulses The number of ON steps in the pattern (must be <= steps)
-    @param rot    Optional rotation to offset the pattern. Must be in the range [0, steps]
-    
-    @return An int array of length steps consisting of 1 and 0 values only
-    
-    @exception ValueError if pulses or rot is out of range
-    
-    @author Brian House
-    @year 2011
-    @license MIT
-    
-    COPYRIGHT 2011 Brian House
-    
-    Permission is hereby granted, free of charge, to any person obtaining a copy of this
-    software and associated documentation files (the “Software”), to deal in the Software
-    without restriction, including without limitation the rights to use, copy, modify, merge,
-    publish, distribute, sublicense, and/or sell copies of the Software, and to permit
-    persons to whom the Software is furnished to do so, subject to the following conditions:
-
-    The above copyright notice and this permission notice shall be included in all copies or
-    substantial portions of the Software.
-
-    THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
-    INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR
-    PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE
-    FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
-    OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-    DEALINGS IN THE SOFTWARE.
-    """
-    steps = int(steps)
-    pulses = int(pulses)
-    rot = int(rot)
-    if pulses > steps or pulses < 0:
-        raise ValueError
-    if rot > steps or steps < 0:
-        raise ValueError
-    if steps == 0:
-        return []
-    pattern = []    
-    counts = []
-    remainders = []
-    divisor = steps - pulses
-    remainders.append(pulses)
-    level = 0
-    while True:
-        counts.append(divisor // remainders[level])
-        remainders.append(divisor % remainders[level])
-        divisor = remainders[level]
-        level = level + 1
-        if remainders[level] <= 1:
-            break
-    counts.append(divisor)
-    
-    def build(level):
-        if level == -1:
-            pattern.append(0)
-        elif level == -2:
-            pattern.append(1)         
-        else:
-            for i in range(0, counts[level]):
-                build(level - 1)
-            if remainders[level] != 0:
-                build(level - 2)
-    
-    build(level)
-    i = pattern.index(1)
-    pattern = pattern[i:] + pattern[0:i]
-    
-    # rotate the pattern if needed by removing the last item and
-    # adding it to the start
-    if rot != 0:
-        for i in range(rot):
-            x = pattern.pop(-1)
-            pattern.insert(0, x)
-    
-    return pattern
 
 class EuclidGenerator:
     """Generates the euclidean rhythm for a single output
     """
-    
+
     def __init__(self, cv_out, steps=1, pulses=0, rotation=0, skip=0):
         """Create a generator that sends its output to the given CV output
 
         @param cv_out  One of the six output jacks (cv1..cv6)
         @param steps  The initial number of steps (1-32)
         @param pulses  The initial number of pulses (0-32)
         @param rotation  The initial rotation (0-32)
         @param skip  The skip probability (0-1)
         """
-        
+
         ## The CV output this generator controls
         self.cv = cv_out
-        
+
         ## The current position within the pattern
         self.position = 0
-        
+
         ## The number of steps in the pattern
         self.steps = steps
-        
+
         ## The number of triggers in the pattern
         self.pulses = pulses
-        
+
         ## The rotation of the pattern
         self.rotation = rotation
-        
+
         ## The probability that we skip any given step when it triggers
         #
         #  Must be in the range [0, 1], where 0 means never skip and
         #  1 means always skip
         self.skip = skip
-        
+
         ## The on/off pattern we generate
         self.pattern = []
-        
+
         ## Cached copy of the string representation
         #
         #  __str__(self) will do some extra string processing
         #  if this is None; otherwise its value is simply returned
         self.str = None
-        
+
         self.regenerate()
-        
+
     def __str__(self):
         """Return a string representation of the pattern
 
         The string consists of 4 characters:
             - ^ current beat, high
             - v current beat, low
             - | high beat
             - . low beat
-            
+
         e.g. |.|.^|.|.||. is a 7/12 pattern, where the 5th note
         is currently playing
         """
-        
+
         if self.str is None:
             s = ""
             for i in range(len(self.pattern)):
                 if i == self.position:
                     if self.pattern[i] == 0:
                         s = s+"v"
                     else:
@@ -171,120 +92,120 @@
                 else:
                     if self.pattern[i] == 0:
                         s = s+"."
                     else:
                         s = s+"|"
             self.str = s
         return self.str
-        
+
     def regenerate(self):
         """Re-calculate the pattern for this generator
 
         Call this after changing any of steps, pulses, or rotation to apply
         the changes.
-        
+
         Changing the pattern will reset the position to zero
         """
-        
+
         self.position = 0
         self.pattern = generate_euclidean_pattern(self.steps, self.pulses, self.rotation)
-        
+
         # clear the cached string representation
         self.str = None
-        
+
     def advance(self):
         """Advance to the next step in the pattern and set the CV output
         """
-        
+
         # advance the position
         # to ease CPU usage don't do any divisions, just reset to zero
         # if we overflow
         self.position = self.position+1
         if self.position >= len(self.pattern):
             self.position = 0
-            
+
         if self.steps == 0 or self.pattern[self.position] == 0:
             self.cv.off()
         else:
             if self.skip > random.random():
                 self.cv.off()
             else:
                 self.cv.on()
-                
+
         # clear the cached string representation
         self.str = None
-        
+
 
 class ChannelMenu:
     """A menu screen that lets us choose which CV channel to edit
     """
     def __init__(self, script):
         """Create the channel menu
 
         @param script  The EuclideanRhythms script that owns this menu
         """
         self.script = script
-        
+
     def draw(self):
         generator_index = k1.range(len(self.script.generators))
         g = self.script.generators[generator_index]
         pattern_str = str(g)
-        
+
         oled.fill(0)
         oled.text(f"-- CV {generator_index+1} --", 0, 0)
         if len(pattern_str) > 16:
             pattern_row1 = pattern_str[0:16]
             pattern_row2 = pattern_str[16:]
             oled.text(f"{pattern_row1}", 0, 10)
             oled.text(f"{pattern_row2}", 0, 20)
         else:
             oled.text(f"{pattern_str}", 0, 10)
-        
+
         oled.show()
 
 class SettingsMenu:
     """A menu screen for controlling a single setting of the generator
     """
     def __init__(self, script):
         """Create the settings menu for a given generator
 
         @param script  The EuclideanRhythms script that owns this menu
         """
         self.script = script
         self.generator = script.generators[0]
-        
+
         self.MENU_ITEMS_STEPS = 0
         self.MENU_ITEMS_PULSES = 1
         self.MENU_ITEMS_ROTATION = 2
         self.MENU_ITEMS_SKIP = 3
         self.menu_items = [
             "Steps",
             "Pulses",
             "Rot.",
             "Skip %"
         ]
-        
+
     def set_generator(self, g):
         """Configure this menu to control a given EuclideanGenerator
 
         @param g  The EuclideanGenerator to control
         """
         self.generator = g
-        
+
     def read_knobs(self):
         """Returns a tuple with the current options
 
         @return a tuple of the form (menu_item, lower_bound, upper_bound, current_setting, new_setting)
         """
-        
+
         menu_item = k1.range(len(self.menu_items))
         lower_bound = 0
         upper_bound = 0
         current_setting = 0
-        
+
         if menu_item == self.MENU_ITEMS_STEPS:
             lower_bound = 1
             upper_bound = 32
             current_setting = self.generator.steps
         elif menu_item == self.MENU_ITEMS_PULSES:
             lower_bound = 0
             upper_bound = self.generator.steps
@@ -293,190 +214,179 @@
             lower_bound = 0
             upper_bound = self.generator.steps
             current_setting = self.generator.rotation
         elif menu_item == self.MENU_ITEMS_SKIP:
             lower_bound = 0
             upper_bound = 100
             current_setting = int(self.generator.skip * 100)
-            
+
         new_setting = k2.range(upper_bound-lower_bound+1) + lower_bound
-        
+
         return (menu_item, lower_bound, upper_bound, current_setting, new_setting)
-        
+
     def draw(self):
         (menu_item, lower_bound, upper_bound, current_setting, new_setting) = self.read_knobs()
-        
+
         oled.fill(0)
         oled.text(f"-- {self.menu_items[menu_item]} --", 0, 0)
         oled.text(f"{current_setting} <- {new_setting}", 0, 10)
         oled.show()
-        
+
     def apply_setting(self):
         """Apply the current setting
         """
         (menu_item, lower_bound, upper_bound, current_setting, new_setting) = self.read_knobs()
-        
+
         if menu_item == self.MENU_ITEMS_STEPS:
             self.generator.steps = new_setting
             if self.generator.pulses > new_setting:
                 self.generator.pulses = new_setting
             if self.generator.rotation > new_setting:
                 self.generator.rotation = new_setting
         elif menu_item == self.MENU_ITEMS_PULSES:
             self.generator.pulses = new_setting
         elif menu_item == self.MENU_ITEMS_ROTATION:
             self.generator.rotation = new_setting
         elif menu_item == self.MENU_ITEMS_SKIP:
             self.generator.skip = new_setting / 100.0
-            
-        self.generator.regenerate()
-        
 
-class Screensaver:
-    """Blanks the screen to prevent burn-in
-    """
-    def __init__(self):
-        pass
-    
-    def draw(self):
-        oled.fill(0);
-        oled.show()
+        self.generator.regenerate()
 
 class EuclideanRhythms(EuroPiScript):
     """Generates 6 different Euclidean rhythms, one per output
 
     Must be clocked externally into DIN
     """
-    
+
     def __init__(self):
         super().__init__()
-        
+
         ## The euclidean pattern generators for each CV output
         #
         #  We pre-load the defaults with some interesting patterns so the script
         #  does _something_ out of the box
         self.generators = [
             EuclidGenerator(cv1, 8, 5),
             EuclidGenerator(cv2, 16, 7),
             EuclidGenerator(cv3, 16, 11),
             EuclidGenerator(cv4, 32, 9),
             EuclidGenerator(cv5, 32, 15),
             EuclidGenerator(cv6, 32, 19)
         ]
-        
+
         self.load()
-        
+
         self.channel_menu = ChannelMenu(self)
         self.settings_menu = SettingsMenu(self)
         self.screensaver = Screensaver()
-        
+
         self.active_screen = self.channel_menu
-        
+
         self.last_interaction_time = time.ticks_ms()
-        
+
         @din.handler
         def on_rising_clock():
             """Handler for the rising edge of the input clock
 
             Advance all of the rhythms
             """
             for g in self.generators:
                 g.advance()
-                
+
         @din.handler_falling
         def on_falling_clock():
             """Handler for the falling edge of the input clock
 
             Turn off all of the CVs so we don't stay on for adjacent pulses
             """
             for cv in cvs:
                 cv.off()
-            
+
         @b1.handler
         def on_b1_press():
             """Handler for pressing button 1
-            """            
+            """
             self.last_interaction_time = time.ticks_ms()
-            
+
             if self.active_screen == self.screensaver:
                 self.active_screen = self.channel_menu
             elif self.active_screen == self.channel_menu:
                 self.activate_settings_menu()
             else:
                 self.settings_menu.apply_setting()
                 self.save()
-            
+
         @b2.handler
         def on_b2_press():
             """Handler for pressing button 2
-            """            
+            """
             self.last_interaction_time = time.ticks_ms()
-            
+
             if self.active_screen == self.screensaver:
                 self.active_screen = self.channel_menu
             elif self.active_screen == self.channel_menu:
                 self.activate_settings_menu()
             else:
                 self.activate_channel_menu()
-        
+
     @classmethod
     def display_name(cls):
         return "Euclid"
-    
+
     def activate_settings_menu(self):
         """ Change the active screen to the settings menu
         """
         channel_index = k1.range(len(self.generators))
         self.settings_menu.set_generator(self.generators[channel_index])
         self.active_screen = self.settings_menu
-        
+
     def activate_channel_menu(self):
         """Change the active screen to the CV channel menu
         """
         self.active_screen = self.channel_menu
-        
+
     def load(self):
         """Load the previously-saved parameters and restore them
         """
         state = self.load_state_json()
-        
+
         for rhythm in state.get("rhythms", []):
             id = rhythm["id"]
             generator = self.generators[id]
-            
+
             generator.steps = rhythm["steps"]
             generator.pulses = rhythm["pulses"]
             generator.rotation = rhythm["rotation"]
             generator.skip = rhythm["skip"]
-            
+
             generator.regenerate()
-        
+
     def save(self):
         """Write the current settings to the persistent storage
         """
         rhythms = []
         for i in range(len(self.generators)):
             d = {
                 "id": i,
                 "steps": self.generators[i].steps,
                 "pulses": self.generators[i].pulses,
                 "rotation": self.generators[i].rotation,
                 "skip": self.generators[i].skip
             }
             rhythms.append(d)
-            
+
         state = {
             "rhythms": rhythms
         }
         self.save_state_json(state)
-        
+
     def main(self):
         while True:
             # check if we've been idle for long enough to trigger the screensaver
             now = time.ticks_ms()
             if time.ticks_diff(now, self.last_interaction_time) > SCREENSAVER_TIMEOUT_MS:
                 self.active_screen = self.screensaver
-                
+
             self.active_screen.draw()
-    
+
 if __name__=="__main__":
     EuclideanRhythms().main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `micropython-europi-contrib-0.8.1/contrib/hamlet.py` & `micropython-europi-contrib-0.9.1/contrib/hamlet.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,12 +349,12 @@
 
     BD.append("1000100010010010")
     HH.append("0010001000100010")
 
 if __name__ == '__main__':
     # Reset module display state.
     oled.fill(0)
-    [cv.off() for cv in cvs]
+    turn_off_all_cvs()
     hm = Hamlet()
     hm.main()
```

### Comparing `micropython-europi-contrib-0.8.1/contrib/harmonic_lfos.py` & `micropython-europi-contrib-0.9.1/contrib/harmonic_lfos.py`

 * *Files identical despite different names*

### Comparing `micropython-europi-contrib-0.8.1/contrib/hello_world.py` & `micropython-europi-contrib-0.9.1/contrib/hello_world.py`

 * *Files identical despite different names*

### Comparing `micropython-europi-contrib-0.8.1/contrib/knob_playground.py` & `micropython-europi-contrib-0.9.1/contrib/knob_playground.py`

 * *Files identical despite different names*

### Comparing `micropython-europi-contrib-0.8.1/contrib/logic.py` & `micropython-europi-contrib-0.9.1/contrib/logic.py`

 * *Files identical despite different names*

### Comparing `micropython-europi-contrib-0.8.1/contrib/master_clock.py` & `micropython-europi-contrib-0.9.1/contrib/master_clock.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,65 +12,45 @@
 Master Clock
 author: Nik Ansell (github.com/gamecat69)
 date: 2022-08-02
 labels: clock, divider
 
 A master clock and clock divider. Each output sends a +5V trigger/gate at different divisions of the master clock, or randomly if condigured with a division of zero.
 Pulse width (gate/trigger duration) is configurable up to a maximum of 50% of the pulse width of output 1.
-
-All configuration (BPM, Pulse Width, output clock divisions) is automatically saved, then loaded when the module is restarted.
-
-For wonky/more interesting clock patterns try these:
-- Reset to step 1 using a gate into the digital input, or by using an odd value for the maximum division
-- Vary BPM by sending CV into the analog input
-- Set the division to zero for an output, this will cause the output to randomly go from high (+5V) to low (0V)
-
-Demo video: TBC
-
-digital_in: (optional) Reset step count on rising edge
-analog_in: (optional) Adjust BPM
-
-knob_1: Screen 2: Adjust BPM. Screen 3: Select output to edit 
-knob_2: Screen 2: Adjust Pulse width. Screen 3: Adjust division of selected output 
-
-button_1: Short Press (<500ms): Start / Stop. Long Press (>500ms): Select clock source (Internal/External)
-button_2: Short Press (<500ms): Cycle through screens. Long Press (>500ms): Enter config mode
-
-Defaults:
-output_1: clock / 1
-output_2: clock / 2
-output_3: clock / 4
-output_4: clock / 8
-output_5: clock / 16
-output_6: clock / 32
-
-Known Issues:
-- If playback is restarted while screen 2 is in config mode, playback will be slightly irratic, especially when moving knobs
-- BPM occasionally drifts by 1ms - possibly due to asyncio, pico performance limitations, or some other as-yet unknown error
+'''
 
 '''
+Version History (with lots missing from the early days!):
+1.1 - Updates by @awoknak to reduce calls to oled.show() as it causes short hangs causes latency
+1.2 - Updates by @nik:  Fix inability to activate internal/external clock with a long-press of B1
+                        Remove screen1 as it is not as important now an external clock is supported
+                        Fix inability to edit pulse width
+                        Removed some bugs in the notes above
+'''
 
 class MasterClockInner(EuroPiScript):
     def __init__(self):
         # Overclock the Pico for improved performance.
         machine.freq(250_000_000)
         self.step = 1
         self.clockInputNum = 1
         self.completedCycles = 0
         self.running = True
         self.resetTimeout = 2000
         self.previousStepTime = 0
-        self.screen = 2
         self.configMode = False
         self.k2Unlocked = False
         self.previousSelectedDivision = 0
         self.previousActiveOption = ''
         self.previousClockTime = 0
         self.inputClockDiffs = []
         self.clockSelectionScreenActive = False
+        
+        # State flag to determine if UI state has changed and display should update.
+        self._updateUI = True
 
         self.MIN_BPM = 20  # Successfully calibrated to >= 20 and <= 240 BPM
         self.MAX_BPM = 240
         self.MIN_PULSE_WIDTH = 8
         self.MIN_AIN_VOLTAGE = 1.1
         self.MAX_DIVISION = 128
         self.MAX_PW_PERCENTAGE = 80
@@ -130,28 +110,16 @@
                 self.configMode = not self.configMode
                 # This will stop the clock from running in config mode - keep here as it might be needed in the future
                 #self.running = False
                 if not self.configMode:
                     # config mode has just been turned off, save state and lock k2
                     self.saveState()
                     self.k2Unlocked = False
-            else:
-                self.k2Unlocked = False
-                
-                # Turn off config mode to avoid current knob positions messing up other settings on the next screen
-                if self.configMode:
-                    self.configMode = False
-                    self.saveState()
-
-                if self.screen == 1:
-                    self.screen = 2
-                elif self.screen == 2:
-                    self.screen = 1
-                else:
-                    self.screen = 1
+                    # Screen has changed
+                    self._updateUI = True
 
         # Trigger clock if using an external clock, or reset if not
         @din.handler
         def dinTrigger():
             if self.externalClockInput:
                 # Divide input clocks by self.inputClockDivision and trigger the clock
                 if self.clockInputNum % self.inputClockDivision == 0:
@@ -164,115 +132,114 @@
                         else:
                             self.inputClockDiffs.append(250)
                         # Only keep 20 values in the buffer
                         if len(self.inputClockDiffs) == 20:
                             del self.inputClockDiffs[0]
 
                         if self.clockInputNum > 3: # Only calculate is there are > 3 entries
-                            self.bpm = self.calculateBpm(self.inputClockDiffs)
+                            bpm = self.calculateBpm(self.inputClockDiffs)
+                            if bpm != self.bpm:
+                                self.bpm = bpm
+                                self._updateUI = True
                     self.previousClockTime = ticks_ms()
                     
                 self.clockInputNum += 1
             else:
                 self.step = 1
 
     ''' Ask to use internal or external clock'''
     def getClockOption(self):
         self.clockSelectionScreenActive = True
         oled.fill(0)
         oled.text("Clock Source:", 0, 0, 1)
         oled.text("B1: Internal", 0, 9, 1)
         oled.text("B2: External", 0, 17, 1)
-        oled.show()
+        self._updateUI = True
+        self.updateDisplay()
         while True:
             if b1.value() == 1:
                 self.externalClockInput = False
                 self.running = False # Need to do this to keep it running because the b1 handler will reverse the value
                 self.clockSelectionScreenActive = False
                 break
             elif b2.value() == 1:
                 self.externalClockInput = True
                 self.clockSelectionScreenActive = False
                 break
             time.sleep(0.05)
         
         self.saveState()
+        self._updateUI = True
 
     def bpmFromMs(self, ms):
         return int(((1/(ms/1000))*60)/4)
 
     def calculateBpm(self, list):
         self.averageDiff = self.average(list)
         return self.bpmFromMs(self.averageDiff)
 
     def average(self, list):
         return sum(list) / len(list)
 
-    '''Show running status'''
-    def screen1(self):
-        oled.fill(0)
-        oled.text(str(self.completedCycles) + ':' + str(self.step), 0, 0, 1)
-        if not self.running:
-            oled.text('B1:Start', 0, 23, 1)
-        else:
-            oled.text('B1:Stop', 0, 23, 1)
-        oled.show()
-
-    '''config screen'''
-    def screen2(self):
+    '''main screen'''
+    def showScreen(self):
         # k1 adjusts selected option. Remove option 1 (bpm) if using an external clock
         if self.externalClockInput:
             self.activeOption = k1.choice([2, 3, 4, 5, 6, 7, 8])
         else:
             self.activeOption = k1.choice([1, 2, 3, 4, 5, 6, 7, 8])
 
         oled.fill(0)
         if self.configMode and self.activeOption != 3:
             configMarker = '|'
             
             # if active config option changes, lock k2 and save state
             if self.previousActiveOption != self.activeOption:
                 self.k2Unlocked = False
-                self.saveState()
+                #self.saveState()
+                self._updateUI = True
 
             # Prevent the BPM from being configured if using an external clock input
             if self.activeOption == 1 and not self.externalClockInput:
                 # read current knob value
                 newBpm = self.MIN_BPM + k2.read_position(steps=(self.MAX_BPM - self.MIN_BPM + 2))
                 # unlock the knob if it has reached near the same value - avoids messy UX
                 if abs(newBpm - self.state.get('bpm')) <= 10:
                     self.k2Unlocked = True
                 # update config value if k2 is unlocked
                 if self.k2Unlocked:
                     self.bpm = newBpm
                     # calculate the new pulse width in milliseconds based on the new bpm
                     self.calcSleepTime()
                     self.getPulseWidth()
-                    
+                    self._updateUI = True
+                        
             elif self.activeOption == 2:
                 # read current knob value
                 newPw = k2.read_position(steps=self.MAX_PW_PERCENTAGE) + 1
                 # unlock the knob if it has reached near the same value - avoids messy UX
                 if abs(newPw - self.state.get('pulseWidthPercent')) <= 2:
                     self.k2Unlocked = True
                 # update config value if k2 is unlocked
-                if self.k2Unlocked:
+                if self.k2Unlocked and self.pulseWidthPercent != newPw:
                     self.pulseWidthPercent = newPw
                     self.calcSleepTime()
                     self.getPulseWidth()
+                self._updateUI = True
 
             elif self.activeOption > 2:
                 # k2 adjusts clock division
                 selectedDivision = k2.choice(self.clockDivisions)
                 # Only adjust values if k2 has moved. This avoids a potentially annoying UX
                 # self.activeOption != 3 / output 1 is disabled from configuration
                 if self.previousSelectedDivision != selectedDivision and self.activeOption != 3:
                     self.outputDivisions[self.activeOption - 3] = selectedDivision
                 
                 self.previousSelectedDivision = selectedDivision
+                self._updateUI = True
             
             self.previousActiveOption = self.activeOption
                     
         else:
             configMarker = '.'
         
         oled.text(str(self.bpm) + ' bpm', 6, 0, 1)
@@ -280,15 +247,15 @@
         oled.text('/' + str(self.outputDivisions[0]), 6, 12, 1)
         oled.text('/' + str(self.outputDivisions[1]), 45, 12, 1)
         oled.text('/' + str(self.outputDivisions[2]), 85, 12, 1)
         oled.text('/' + str(self.outputDivisions[3]), 6, 24, 1)
         oled.text('/' + str(self.outputDivisions[4]), 45, 24, 1)
         oled.text('/' + str(self.outputDivisions[5]), 85, 24, 1)
         oled.text(configMarker, self.markerPositions[self.activeOption-1][0], self.markerPositions[self.activeOption-1][1], 1)
-        oled.show() 
+        self.updateDisplay() 
 
     ''' Holds given output (cv) high for pulseWidthMs duration '''
     async def outputPulse(self, cv):
         cv.voltage(5)
         await asyncio.sleep_ms(self.pulseWidthMs)
         cv.off()
 
@@ -296,22 +263,24 @@
     def calcSleepTime(self):
         self.mSBetweenClockCycles = int((60000 / self.bpm / self.CLOCKS_PER_QUARTER_NOTE))
     
     def checkForAinBPM(self):
         val = 100 * ain.percent()
         # If there is an analogue input voltage use that for BPM. clamp ensures it is higher than MIN and lower than MAX
         if val > self.MIN_AIN_VOLTAGE:
-            self.bpm = clamp(int((((self.MAX_BPM) / 100) * val) + self.MIN_BPM), self.MIN_BPM, self.MAX_BPM)
-            self.calcSleepTime()
-            self.getPulseWidth()
+            bpm = clamp(int((((self.MAX_BPM) / 100) * val) + self.MIN_BPM), self.MIN_BPM, self.MAX_BPM)
         else:
             # No analog input, revert to last saved state
-            self.bpm = self.state.get("bpm", 100)
+            bpm = self.state.get("bpm", 100)
+        
+        if self.bpm != bpm:
+            self.bpm = bpm
             self.calcSleepTime()
             self.getPulseWidth()
+            self._updateUI = True
 
     def getPulseWidth(self):
         # Set max of self.MAX_PW_PERCENTAGE percent of total cycle time
         self.MAX_PULSE_WIDTH = int(self.mSBetweenClockCycles * self.MAX_PW_PERCENTAGE // 100)
         # Calc pulse width in milliseconds given the desired percentage. clamp ensures it is higher than MIN and lower than MAX
         self.pulseWidthMs = clamp((self.mSBetweenClockCycles * (self.pulseWidthPercent)//100), self.MIN_PULSE_WIDTH, self.MAX_PULSE_WIDTH)
 
@@ -352,21 +321,30 @@
         else:
             self.completedCycles += 1
             self.step = 1
         
         # Get time of last step to use in the auto reset function
         self.previousStepTime = ticks_ms()
 
+        # Display may update on clock trigger.
+        self._updateUI = True
+
         # Debug task output to check for overrunning tasks i.e. memory leaks
         if self.DEBUG:
             for i in self.tasks:
                 if i != 0:
                     print(f'[{i}] done: {str(i.done())}. state: {str(i.state)}. data: {str(i.data)}. coro: {str(i.coro)}')
                 else:
                     print(0)
+    
+    def updateDisplay(self):
+        """Update the display if UI state has changed."""
+        if self._updateUI:
+            oled.show()
+            self._updateUI = False
 
     ''' Save working vars to a save state file'''
     def saveState(self):
         self.state = {
             "bpm": self.bpm,
             "pulseWidthPercent": self.pulseWidthPercent,
             "externalClockInput": self.externalClockInput,
@@ -387,19 +365,15 @@
         self.outputDivisions = self.state.get("outputDivisions", [1,2,4,8,16,32])
 
         self.saveState()
 
     async def main(self):
         while True:
             if not self.clockSelectionScreenActive:
-                # Display selected screen
-                if self.screen == 1:
-                    self.screen1()
-                else:
-                    self.screen2()
+                self.showScreen()
 
             # Auto reset function after resetTimeout
             if self.step != 0 and ticks_diff(ticks_ms(), self.previousStepTime) > self.resetTimeout:
                  self.step = 1
                  self.completedCycles = 0
 
             if not self.configMode and not self.externalClockInput:
@@ -426,8 +400,7 @@
         el.run_forever()
 
 if __name__ == '__main__':
     m = MasterClock()
     m.main()
 
 
-
```

### Comparing `micropython-europi-contrib-0.8.1/contrib/menu.py` & `micropython-europi-contrib-0.9.1/contrib/menu.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,22 +16,24 @@
 # Scripts that are included in the menu
 EUROPI_SCRIPTS = [
     "contrib.bernoulli_gates.BernoulliGates",
     "contrib.coin_toss.CoinToss",
     "contrib.consequencer.Consequencer",
     "contrib.cvecorder.CVecorder",
     "contrib.diagnostic.Diagnostic",
+    "contrib.envelope_generator.EnvelopeGenerator",
     "contrib.euclid.EuclideanRhythms",
     "contrib.hamlet.Hamlet",
     "contrib.harmonic_lfos.HarmonicLFOs",
     "contrib.hello_world.HelloWorld",
     "contrib.knob_playground.KnobPlayground",
     "contrib.logic.Logic",
     "contrib.master_clock.MasterClock",
     "contrib.noddy_holder.NoddyHolder",
+    "contrib.pams.PamsWorkout",
     "contrib.piconacci.Piconacci",
     "contrib.polyrhythmic_sequencer.PolyrhythmSeq",
     "contrib.poly_square.PolySquare",
     "contrib.probapoly.Probapoly",
     "contrib.quantizer.QuantizerScript",
     "contrib.radio_scanner.RadioScanner",
     "contrib.scope.Scope",
```

### Comparing `micropython-europi-contrib-0.8.1/contrib/noddy_holder.py` & `micropython-europi-contrib-0.9.1/contrib/noddy_holder.py`

 * *Files identical despite different names*

### Comparing `micropython-europi-contrib-0.8.1/contrib/piconacci.py` & `micropython-europi-contrib-0.9.1/contrib/piconacci.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
     def value(self, index):
         # Return a value from the series, taking into account offset and rotation
         return self.fib[self.offset : self.offset + 6][(index + self.rotate) % 6]
 
     def main(self):
         # Reset all outputs
-        [cv.off() for cv in cvs]
+        turn_off_all_cvs()
         while True:
             # If the state has changed, update display
             if self.display_update_required:
                 self.updateScreen()
                 self.display_update_required = False
 
     def updateScreen(self):
```

### Comparing `micropython-europi-contrib-0.8.1/contrib/poly_square.py` & `micropython-europi-contrib-0.9.1/contrib/poly_square.py`

 * *Files identical despite different names*

### Comparing `micropython-europi-contrib-0.8.1/contrib/polyrhythmic_sequencer.py` & `micropython-europi-contrib-0.9.1/contrib/polyrhythmic_sequencer.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,15 +208,16 @@
                 self.trigger_xor.on()
 
             self.counter = self.counter + 1
 
         @din.handler_falling
         def triggers_off():
             # Turn off all of the trigger CV outputs.
-            [seq.trigger_cv.off() for seq in self.seqs]
+            for seq in self.seqs:
+                seq.trigger_cv.off()
             self.trigger_and.off()
             self.trigger_xor.off()
 
     def _trigger_seq(self, step: int):
         # Convert poly sequence enablement into binary to determine which
         # sequences are triggered on this step.
         status = f"{self.seq_poly[step]:02b}"
@@ -260,15 +261,16 @@
         self.seq_poly = list(_state.seq_poly)
     
     def reset_check(self):
         """Reset the sequences and triggers when no clock pulse detected for specified time."""
         if self.counter != 0 and ticks_diff(ticks_ms(), din.last_triggered()) > self.reset_timeout:
             self.step = 0
             self.counter = 0
-            [s.reset() for s in self.seqs]
+            for s in self.seqs:
+                s.reset()
             self.trigger_and.off()
             self.trigger_xor.off()
 
     def show_menu_header(self):
         if ticks_diff(ticks_ms(), b1.last_pressed()) < MENU_DURATION:
             oled.fill_rect(0, 0, OLED_WIDTH, CHAR_HEIGHT, 1)
             oled.text(f"{self.pages[self.page]}", 0, 0, 0)
```

### Comparing `micropython-europi-contrib-0.8.1/contrib/probapoly.py` & `micropython-europi-contrib-0.9.1/contrib/probapoly.py`

 * *Files identical despite different names*

### Comparing `micropython-europi-contrib-0.8.1/contrib/quantizer.py` & `micropython-europi-contrib-0.9.1/contrib/quantizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,27 +4,19 @@
 
   @author Chris Iverach-Brereton <ve4cib@gmail.com>
   @date   2023-02-12
 """
 
 from europi import *
 from europi_script import EuroPiScript
-import time
-
-## 1.0V/O is the Eurorack/Moog standard, but Buchla uses 1.2V/O
-#
-#  Just in case someone needs Buchla compatibility, this is defined
-#  but nobody is likely to need this
-VOLTS_PER_OCTAVE = 1.0
 
-## Standard wester music scale has 12 semitones per octave
-SEMITONES_PER_OCTAVE = 12
+from experimental.quantizer import Quantizer, VOLTS_PER_OCTAVE, VOLTS_PER_SEMITONE, SEMITONES_PER_OCTAVE
+from experimental.screensaver import Screensaver
 
-## How many volts per semitone
-VOLTS_PER_SEMITONE = float(VOLTS_PER_OCTAVE) / float(SEMITONES_PER_OCTAVE)
+import time
 
 ## Whe in triggered mode we only quantize when we receive an external clock signal
 MODE_TRIGGERED=0
 
 ## In continuous mode the digital input is ignored and we quantize the input
 #  at the highest rate possible
 MODE_CONTINUOUS=1
@@ -34,40 +26,36 @@
 #  =20 minutes
 SCREENSAVER_TIMEOUT_MS = 1000 * 60 * 20
 
 
 SELECT_OPTION_Y = 16
 HALF_CHAR_WIDTH = int(CHAR_WIDTH / 2)
 
-
-class ScreensaverScreen:
+class ScreensaverScreen(Screensaver):
     """Blank the screen when idle
 
     Eventually it might be neat to have an animation, but that's
     not necessary for now
     """
     def __init__(self, quantizer):
+        super().__init__(self)
         self.quantizer = quantizer
-        
+
     def on_button1(self):
         self.quantizer.active_screen = self.quantizer.kb
-    
-    def draw(self):
-        oled.fill(0)
-        oled.show()
 
 class KeyboardScreen:
     """Draws a pretty keyboard and indicates what notes are enabled
     and what note is being played as the primary output
     """
-    
+
     def __init__(self, quantizer):
         self.quantizer = quantizer
         self.highlight_note = 0
-        
+
         # X, Y, bw
         self.enable_marks = [
             (  8, 2, 0),
             ( 17, 2, 1),
             ( 26, 2, 0),
             ( 35, 2, 1),
             ( 43, 2, 0),
@@ -75,120 +63,120 @@
             ( 69, 2, 1),
             ( 77, 2, 0),
             ( 85, 2, 1),
             ( 94, 2, 0),
             (103, 2, 1),
             (112, 2, 0)
         ]
-        
+
         self.playing_marks = [
             (  8, 20, 0),
             ( 17, 15, 1),
             ( 26, 20, 0),
             ( 35, 15, 1),
             ( 43, 20, 0),
             ( 59, 20, 0),
             ( 69, 15, 1),
             ( 77, 20, 0),
             ( 85, 15, 1),
             ( 94, 20, 0),
             (103, 15, 1),
             (112, 20, 0)
         ]
-        
+
     def draw(self):
         # a 128x32 keyboard image
         # see https://github.com/Allen-Synthesis/EuroPi/blob/main/software/oled_tips.md
         # and https://github.com/novaspirit/img2bytearray
         kb=b'\x07\xff\xc0\x7f\xe0?\xfe\xff\xf8\x0f\xfc\x07\xfe\x03\xff\xe0\x07\xff\xc0\x7f\xe0?\xfe\xff\xf8\x0f\xfc\x07\xfe\x03\xff\xe0\x07\xff\xc0\x7f\xe0?\xfe\xff\xf8\x0f\xfc\x07\xfe\x03\xff\xe0\x07\xff\xc0\x7f\xe0?\xfe\xff\xf8\x0f\xfc\x07\xfe\x03\xff\xe0\x07\xff\xc0\x7f\xe0?\xfe\xff\xf8\x0f\xfc\x07\xfe\x03\xff\xe0\x07\xff\xc0\x7f\xe0?\xfe\xff\xf8\x0f\xfc\x07\xfe\x03\xff\xe0\x07\xff\xc0\x7f\xe0?\xfe\xff\xf8\x0f\xfc\x07\xfe\x03\xff\xe0\x07\xff\xc0\x7f\xe0?\xfe\xff\xf8\x0f\xfc\x07\xfe\x03\xff\xe0\x07\xff\xc0\x7f\xe0?\xfe\xff\xf8\x0f\xfc\x07\xfe\x03\xff\xe0\x07\xff\xc0\x7f\xe0?\xfe\xff\xf8\x0f\xfc\x07\xfe\x03\xff\xe0\x07\xff\xc0\x7f\xe0?\xfe\xff\xf8\x0f\xfc\x07\xfe\x03\xff\xe0\x07\xff\xc0\x7f\xe0?\xfe\xff\xf8\x0f\xfc\x07\xfe\x03\xff\xe0\x07\xff\xc0\x7f\xe0?\xfe\xff\xf8\x0f\xfc\x07\xfe\x03\xff\xe0\x07\xff\xc0\x7f\xe0?\xfe\xff\xf8\x0f\xfc\x07\xfe\x03\xff\xe0\x07\xff\xc0\x7f\xe0?\xfe\xff\xf8\x0f\xfc\x07\xfe\x03\xff\xe0\x07\xff\xc0\x7f\xe0?\xfe\xff\xf8\x0f\xfc\x07\xfe\x03\xff\xe0\x07\xff\xc0\x7f\xe0?\xfe\xff\xf8\x0f\xfc\x07\xfe\x03\xff\xe0\x07\xff\xc0\x7f\xe0?\xfe\xff\xf8\x0f\xfc\x07\xfe\x03\xff\xe0\x07\xff\xc0\x7f\xe0?\xfe\xff\xf8\x0f\xfc\x07\xfe\x03\xff\xe0\x07\xff\xc0\x7f\xe0?\xfe\xff\xf8\x0f\xfc\x07\xfe\x03\xff\xe0\x07\xff\xc0\x7f\xe0?\xfe\xff\xf8\x0f\xfc\x07\xfe\x03\xff\xe0\x07\xff\xc0\x7f\xe0?\xfe\xff\xf8\x0f\xfc\x07\xfe\x03\xff\xe0\x07\xff\xc0\x7f\xe0?\xfe\xff\xf8\x0f\xfc\x07\xfe\x03\xff\xe0\x07\xff\xfb\xff\xfd\xff\xfe\xff\xff\x7f\xff\xbf\xff\xdf\xff\xe0\x07\xff\xfb\xff\xfd\xff\xfe\xff\xff\x7f\xff\xbf\xff\xdf\xff\xe0\x07\xff\xfb\xff\xfd\xff\xfe\xff\xff\x7f\xff\xbf\xff\xdf\xff\xe0\x07\xff\xfb\xff\xfd\xff\xfe\xff\xff\x7f\xff\xbf\xff\xdf\xff\xe0\x07\xff\xfb\xff\xfd\xff\xfe\xff\xff\x7f\xff\xbf\xff\xdf\xff\xe0\x07\xff\xfb\xff\xfd\xff\xfe\xff\xff\x7f\xff\xbf\xff\xdf\xff\xe0\x07\xff\xfb\xff\xfd\xff\xfe\xff\xff\x7f\xff\xbf\xff\xdf\xff\xe0\x07\xff\xfb\xff\xfd\xff\xfe\xff\xff\x7f\xff\xbf\xff\xdf\xff\xe0\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00'
-        
+
         # read the encoder value from knob 1 so we know what key to highlight
         self.highlight_note = k1.range(len(self.quantizer.scale))
-        
+
         # draw the keyboard image to the screen
         img = bytearray(kb)
         imgFB = FrameBuffer(img, 128, 32, MONO_HLSB)
         oled.blit(imgFB,0,0)
-        
+
         # mark the enabled notes with a .
         for i in range(len(self.quantizer.scale)):
             if self.quantizer.scale[i]:
                 oled.text('.', *self.enable_marks[i])
-        
+
         # mark the active note with a +
         k = self.quantizer.current_note
         oled.text('+', self.playing_marks[k][0], self.playing_marks[k][1], self.playing_marks[k][2])
-        
+
         # clear the bottom of the screen and mark the togglable key with a line
         oled.fill_rect(0, 30, 128, 32, 0)
         oled.fill_rect(self.enable_marks[self.highlight_note][0], 31, 7, 1, 1)
-        
+
         oled.show()
-        
+
     def on_button1(self):
         self.quantizer.scale[self.highlight_note] = not self.quantizer.scale[self.highlight_note]
         self.quantizer.save()
 
 class MenuScreen:
     """Advanced menu options screen
     """
-    
+
     def __init__(self, quantizer):
         self.quantizer = quantizer
         self.menu_item = 0
-        
+
         self.menu_items = [
             ModeChooser(quantizer),
             RootChooser(quantizer),
             OctaveChooser(quantizer),
             IntervalChooser(quantizer, 2),
             IntervalChooser(quantizer, 3),
             IntervalChooser(quantizer, 4),
             IntervalChooser(quantizer, 5)
         ]
-        
+
     def draw(self):
         self.menu_item = k1.range(len(self.menu_items))
         self.menu_items[self.menu_item].draw()
-        
+
     def on_button1(self):
         self.menu_items[self.menu_item].on_button1()
 
 class ModeChooser:
     """Used by MenuScreen to choose the operating mode
     """
     def __init__(self, quantizer):
         self.quantizer = quantizer
-        
+
         self.mode_names = [
             "Triggered",
             "Continuous"
         ]
-        
+
     def read_mode(self, mode='integer'):
         if mode == 'string':
             return k2.choice(self.mode_names)
         else:
             return k2.range(len(self.mode_names))
-        
+
     def on_button1(self):
         new_mode = self.read_mode()
         self.quantizer.mode = new_mode
         self.quantizer.save()
-        
+
     def draw(self):
         oled.fill(0)
         oled.text(f"Mode", 0, 0)
-        
+
         current_mode = self.mode_names[self.quantizer.mode]
         new_mode = self.read_mode(mode='string')
         QuantizerScript.choose_option(self, new_mode, current_mode, self.mode_names)
-        
+
         oled.show()
-    
+
 class RootChooser:
     """Used by MenuScreen to choose the transposition offset
     """
     def __init__(self, quantizer):
         self.quantizer = quantizer
         self.root_names = [
             "C ",
@@ -200,69 +188,69 @@
             "F#",
             "G ",
             "G#",
             "A ",
             "A#",
             "B "
         ]
-        
+
     def read_root(self, mode='integer'):
         if mode == 'string':
             return k2.choice(self.root_names)
         else:
             return k2.range(len(self.root_names))
-    
+
     def on_button1(self):
         new_root = self.read_root()
         self.quantizer.root = new_root
         self.quantizer.save()
-        
+
     def draw(self):
         oled.fill(0)
         oled.text(f"Transpose", 0, 0)
-        
+
         new_root = self.read_root(mode='string')
         current_root = self.root_names[self.quantizer.root]
         QuantizerScript.choose_option(self, new_root, current_root, self.root_names)
-        
+
         oled.show()
 
 class OctaveChooser:
     """Used by MenuScreen to choose the octave offset
     """
     def __init__(self, quantizer):
         self.quantizer = quantizer
         self.octave_texts = ['-4', '-3', '-2', '-1', '0', '+1', '+2', '+3', '+4']
         self.octave_text_y = 12
-        
+
     def read_octave(self, mode='integer'):
         if mode == 'string':
             return k2.choice(self.octave_texts)
         else:
             return k2.range(9) - 4  # result should be -1 to +2
-    
+
     def on_button1(self):
         new_octave = self.read_octave()
         self.quantizer.octave = new_octave
         self.quantizer.save()
-        
+
     def draw(self):
         oled.fill(0)
         oled.text(f"Octave", 0, 0)
-        
+
         new_octave = self.read_octave(mode='string')
         current_octave = self.quantizer.octave
-        
+
         if current_octave > 0:
             current_octave = '+' + str(current_octave)
         else:
             current_octave = str(current_octave)
-            
+
         QuantizerScript.choose_option(self, new_octave, current_octave, self.octave_texts)
-            
+
         oled.show()
 
 class IntervalChooser:
     """Used by MenuScreen to choose the interval offset for a given output
     """
     def __init__(self, quantizer, n):
         self.quantizer = quantizer
@@ -271,312 +259,252 @@
             "-Pe 8",
             "-MA 7",
             "-mi 7",
             "-MA 6",
             "-mi 6",
             "-Pe 5",
             "-Di 5",
-            "-Per 4",
+            "-Pe 4",
             "-MA 3",
             "-mi 3",
             "-MA 2",
             "-mi 2",
             "Pe 1",
             "+mi 2",
             "+MA 2",
             "+mi 3",
             "+MA 3",
-            "+Per 4",
+            "+Pe 4",
             "+Di 5",
             "+Pe 5",
             "+mi 6",
             "+MA 6",
             "+mi 7",
             "+MA 7",
             "+Pe 8"
         ]
-        
-        
+
+
     def read_interval(self, mode='integer'):
         if mode == 'string':
             return k2.choice(self.interval_names)
         else:
             return k2.range(len(self.interval_names)) - 12
-    
+
     def on_button1(self):
         new_interval = self.read_interval()
         self.quantizer.intervals[self.n-2] = new_interval
         self.quantizer.save()
-        
+
     def draw(self):
         oled.fill(0)
         oled.text(f"Output {self.n}", 0, 0)
-        
+
         new_interval = self.read_interval(mode='string')
         current_interval = self.interval_names[self.quantizer.intervals[self.n-2]+12]
         QuantizerScript.choose_option(self, new_interval, current_interval, self.interval_names)
-        
-        oled.show()
 
-class Quantizer:
-    """Represents a set of semitones we can quantize input voltages to
-
-    By default this represents a chromatic scale, with all notes enabled.  Notes can be changed
-    by setting scale[n] = True/False, where n is the index of the semitone to toggle
-    """
-    
-    def __init__(self, notes=None):
-        """Constructor; can specify what notes are enabled/disabled
-
-        Undesired results may happen if you use an array that's not of length 12
-
-        @param notes  A boolean array of length 12 indicating what semitones are enabled (True)
-                      or disabled (False)
-        """
-        if notes is None:
-            self.notes = [True]*12
-        else:
-            self.notes = notes
-        
-    def __getitem__(self, n):
-        return self.notes[n]
-    
-    def __setitem__(self, n, value):
-        self.notes[n] = value
-        
-    def __len__(self):
-        return len(self.notes)
-        
-    def quantize(self, analog_in):
-        """Take an analog input voltage and round it to the nearest note on our scale
-
-        @param analog_in  The input voltage to quantize, as a float
-        
-        @return A tuple of the form (voltage, note) where voltage is
-                the raw voltage to output, and note is a value from
-                0-11 indicating the semitone
-        """
-        # first get the closest chromatic voltage to the input
-        nearest_chromatic_volt = round(analog_in / VOLTS_PER_SEMITONE) * VOLTS_PER_SEMITONE
-        
-        # then convert that to a 0-12 value indicating the nearest semitone
-        base_volts = int(nearest_chromatic_volt)
-        nearest_semitone = (nearest_chromatic_volt - base_volts) / VOLTS_PER_SEMITONE
-        
-        # go through our scale and determine the nearest on-scale note
-        nearest_on_scale = 0
-        best_delta = 255
-        for note in range(len(self.notes)):
-            if self.notes[note]:
-                delta = abs(nearest_semitone - note)
-                if delta < best_delta:
-                    nearest_on_scale = note
-                    best_delta = delta
-           
-        volts = base_volts + nearest_on_scale * VOLTS_PER_SEMITONE
-        
-        return (volts, nearest_on_scale)
-    
+        oled.show()
 
 class QuantizerScript(EuroPiScript):
     """The main EuroPi program. Uses Scale to quantize incoming analog voltages
     and round them to the nearest note on the scale.
 
     Primary output is on cv1, with cv2-5 as aux outputs shifted up/down a fixed
     number of semitones.  cv6 outputs a gate/trigger.
     """
     def __init__(self):
         super().__init__()
-        
+
         # keep track of the last time the user interacted with the module
         # if we're idle for too long, start the screensaver
         self.last_interaction_time = time.ticks_ms()
-        
+
         # Continious quantizing, or only on an external trigger?
         self.mode = MODE_TRIGGERED
-        
+
         # What semitone is the root of the scale?
         # 0 = C, 1 = C#/Db, 2 = D, etc...
         # This is used to transpose the output up the given number of semitones
         self.root = 0
-        
+
         # What octave are we outputting?
         self.octave = 0
-        
+
         # Outputs 2-5 output the same note, shifted up or down by
         # a fixed number of semitones
         self.intervals = [0, 0, 0, 0]
         self.aux_outs = [cv2, cv3, cv4, cv5]
-        
+
         # The current scale we're quantizing to
         self.scale = Quantizer()
-        
+
         # The input/output voltages
         self.input_voltage = 0.0
         self.output_voltage = 0.0
-        
+
         # The semitone we're currently outputting on cv1 (0-11)
         self.current_note = 0
-        
+
         # GUI/user interaction
         self.kb = KeyboardScreen(self)
         self.menu = MenuScreen(self)
         self.screensaver = ScreensaverScreen(self)
         self.active_screen = self.kb
-        
+
         self.screen_centre = int(OLED_WIDTH / 2)
-        
+
         self.load()
-        
+
         # connect event handlers for the rising & falling clock edges + button presses
-        
+
         @din.handler
         def on_rising_clock():
             """Handler for the rising edge of the input clock
             """
             if self.mode == MODE_TRIGGERED:
                 self.read_quantize_output()
                 cv6.on()
-            
+
         @din.handler_falling
         def on_falling_clock():
             """Handler for the falling edge of the input clock
             """
             if self.mode == MODE_TRIGGERED:
                 cv6.off()
-            
+
         @b1.handler
         def on_b1_press():
             """Handler for pressing button 1
 
             Button 1 is used for the main interaction and is passed to
             the current display for user interaction
             """
             self.last_interaction_time = time.ticks_ms()
             self.active_screen.on_button1()
-            
+
         @b2.handler
         def on_b2_press():
             """Handler for pressing button 2
 
             Button 2 is used to cycle between screens
             """
             self.last_interaction_time = time.ticks_ms()
-            
+
             if self.active_screen == self.kb:
                 self.active_screen = self.menu
             else:
                 self.active_screen = self.kb
-        
+
     def load(self):
         """Load the persistent settings from storage and apply them
         """
         state = self.load_state_json()
-        
+
         loaded_scale = state.get("scale", [True]*12)  # default to a chromatic scale
         self.scale.notes = loaded_scale
-        
+
         self.root = state.get("root", self.root)
         self.octave = state.get("octave", self.octave)
         self.intervals = state.get("intervals", self.intervals)
         self.mode = state.get("mode", self.mode)
-    
+
     def save(self):
         """Save the current settings to persistent storage
         """
         state = {
             "scale": self.scale.notes,
             "root": self.root,
             "octave": self.octave,
             "intervals": self.intervals,
             "mode": self.mode
         }
         self.save_state_json(state)
-        
+
     @classmethod
     def display_name(cls):
         return "Quantizer"
-       
+
     def quantize(self, analog_in):
         """Take an analog signal and process it
 
         Sets self.current_note and self.output_voltage
         """
-        
+
         (volts, semitone) = self.scale.quantize(analog_in)
-        
+
         # apply our octave & transposition offsets
         volts = volts + self.octave * VOLTS_PER_OCTAVE + self.root * VOLTS_PER_SEMITONE
-        
+
         self.output_voltage = volts
         self.current_note = semitone
-       
+
     def read_quantize_output(self):
         """Read the input signal, quantize it, set outputs 1-5 accordingly
 
         Called by the main loop in continuous mode or the rising clock handler
         in triggered mode
         """
         self.input_voltage = ain.read_voltage(500)   # increase the number of samples to help reduce noise
         self.quantize(self.input_voltage)
-        
+
         cv1.voltage(self.output_voltage)
-        
+
         for i in range(len(self.aux_outs)):
             self.aux_outs[i].voltage(self.output_voltage + self.intervals[i] * VOLTS_PER_SEMITONE)
-    
+
     def choose_option(self, new_item, current_item, all_items):
         item_widths = []
         for item_text in all_items:
             if item_text == new_item:
                 offset = -int(sum(item_widths) + (CHAR_WIDTH * (len(item_widths))) + (CHAR_WIDTH * (len(item_text) / 2)) - (OLED_WIDTH / 2))
             item_widths.append(len(item_text) * CHAR_WIDTH)
-        
+
         x = offset
 
         for index, item_text in enumerate(all_items):
             item_text_width = item_widths[index]
             if item_text == current_item:
                 oled.fill_rect((x - 1), SELECT_OPTION_Y, (item_text_width + 3), (CHAR_HEIGHT + 4), 1)
                 oled.text(item_text, x, (SELECT_OPTION_Y + 2), 0)
             elif item_text == new_item:
                 oled.rect((x - 1), SELECT_OPTION_Y, (item_text_width + 3), (CHAR_HEIGHT + 4), 1)
                 oled.text(item_text, x, (SELECT_OPTION_Y + 2), 1)
             else:
                 oled.text(item_text, x, (SELECT_OPTION_Y + 2), 1)
             x += item_text_width + CHAR_WIDTH
-    
+
     def main(self):
         """The main loop; reads from ain, sets the output voltages
         """
-        
+
         while True:
             # Check if we've been idle for too long; if so, blank the screen
             # to prevent burn-in
             now = time.ticks_ms()
             if time.ticks_diff(now, self.last_interaction_time) > SCREENSAVER_TIMEOUT_MS:
                 self.active_screen = self.screensaver
-            
+
             if self.mode == MODE_CONTINUOUS:
                 # clear the previous trigger
                 cv6.off()
-                
+
                 # Read the new voltage and output it
                 last_output = self.output_voltage
                 self.read_quantize_output()
-                
+
                 if last_output != self.output_voltage:
                     cv6.on()
-                    
+
                 # In continuous mode we fall back to a 100Hz internal clock
                 # that effectively simulates a very high-speed input trigger
                 # Note that this rate has to be long enough for the trigger on
                 # cv6 to be useful to other modules.  A 10ms trigger is a
                 # reasonable compromise between high-speed input signal processing
                 # and keeping the code simple
                 CYCLE_RATE = 0.01
                 time.sleep(CYCLE_RATE)
-            
+
             self.active_screen.draw()
-    
+
 if __name__ == "__main__":
     QuantizerScript().main()
```

### Comparing `micropython-europi-contrib-0.8.1/contrib/radio_scanner.py` & `micropython-europi-contrib-0.9.1/contrib/radio_scanner.py`

 * *Files identical despite different names*

### Comparing `micropython-europi-contrib-0.8.1/contrib/scope.py` & `micropython-europi-contrib-0.9.1/contrib/scope.py`

 * *Files identical despite different names*

### Comparing `micropython-europi-contrib-0.8.1/contrib/sequential_switch.py` & `micropython-europi-contrib-0.9.1/contrib/sequential_switch.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 
     @author Chris Iverach-Brereton <ve4cib@gmail.com>
     @date   2023-02-13
 """
 
 from europi import *
 from europi_script import EuroPiScript
+
+from experimental.screensaver import Screensaver
+
 import time
 import random
 
 ## Move in order 1>2>3>4>5>6>1>2>...
 MODE_SEQUENTIAL=0
 
 ## Move in order 1>6>5>4>3>2>1>6>...
@@ -22,192 +25,189 @@
 MODE_RANDOM=3
 
 ## How many milliseconds of idleness do we need before we trigger the screensaver?
 #
 #  =20 minutes
 SCREENSAVER_TIMEOUT_MS = 1000 * 60 * 20
 
-class ScreensaverScreen:
+class ScreensaverScreen(Screensaver):
     """Blank the screen when idle
     Eventually it might be neat to have an animation, but that's
     not necessary for now
     """
-    
+
     def __init__(self, parent):
+        super().__init__(self)
         self.parent = parent
-        
+
     def on_button1(self):
         self.parent.active_screen = self.parent.switch_screen
         self.parent.on_trigger()
-    
-    def draw(self):
-        oled.fill(0)
-        oled.show()
 
 class SwitchScreen:
     """Default display: shows what output is currently active
     """
-    
+
     def __init__(self, parent):
         self.parent = parent
-        
+
     def on_button1(self):
         # the button can be used to advance the output
         self.parent.on_trigger()
-        
+
     def draw(self):
         oled.fill(0)
-        
+
         # Show all 6 outputs as a string on 2 lines to mirror the panel
         switches = ""
         for i in range(2):
             for j in range(3):
                 out_no = i*3 + j
                 if out_no < self.parent.num_outputs:
                     # output is enabled; is it hot?
                     if self.parent.current_output == out_no:
                         switches = switches + " [*] "
                     else:
                         switches = switches + " [ ] "
                 else:
                     # output is disabled; mark it with .
                     switches = switches + "  .  "
-                    
+
             switches = switches + "\n"
-        
+
         oled.centre_text(switches)
-        
+
         oled.show()
 
 class MenuScreen:
     """Advanced menu options screen
     """
     def __init__(self, parent):
         self.parent = parent
-        
+
         self.menu_items = [
             NumOutsChooser(parent),
             ModeChooser(parent)
         ]
-        
+
     def draw(self):
         self.menu_items[self.parent.menu_item].draw()
-        
+
     def on_button1(self):
         self.menu_items[self.parent.menu_item].on_button1()
 
 class NumOutsChooser:
     """Used by MenuScreen to choose the number of outputs
     """
-    
+
     def __init__(self, parent):
         self.parent = parent
-        
+
     def read_num_outs(self):
         return k2.range(5) + 2 # result should be 2-6
-        
+
     def on_button1(self):
         num_outs = self.read_num_outs()
         self.parent.num_outputs = num_outs
         self.parent.current_output = self.parent.current_output % num_outs
         self.parent.save()
-        
+
     def draw(self):
         num_outs = self.read_num_outs()
         oled.fill(0)
         oled.text(f"-- # Outputs --", 0, 0)
         oled.text(f"{self.parent.num_outputs} <- {num_outs}", 0, 10)
         oled.show()
-    
+
 class ModeChooser:
     """Used by MenuScreen to choose the operating mode
     """
     def __init__(self, parent):
         self.parent = parent
-        
+
         self.mode_names = [
             "Seq.",
             "Rev.",
             "P-P",
             "Rand."
         ]
-        
+
     def read_mode(self):
         return k2.range(len(self.mode_names))
-        
+
     def on_button1(self):
         new_mode = self.read_mode()
         self.parent.mode = new_mode
         self.parent.save()
-        
+
     def draw(self):
         new_mode = self.read_mode()
         oled.fill(0)
         oled.text(f"-- Mode --", 0, 0)
         oled.text(f"{self.mode_names[self.parent.mode]} <- {self.mode_names[new_mode]}", 0, 10)
         oled.show()
 
 class SequentialSwitch(EuroPiScript):
     """The main workhorse of the whole module
 
     Copies the analog input to one of the 6 outputs, cycling which output
     whenever a trigger is received
     """
-    
+
     def __init__(self):
         super().__init__()
-        
+
         # keep track of the last time the user interacted with the module
         # if we're idle for too long, start the screensaver
         self.last_interaction_time = time.ticks_ms()
-        
+
         # How do we advance the output?
         self.mode = MODE_SEQUENTIAL
-        
+
         # Use all 6 outputs by default
         self.num_outputs = 6
-        
+
         # The index of the current outputs
         self.current_output = 0
-        
+
         # For MODE_PINGPONG, this indicates the direction of travel
         # it will always be +1 or -1
         self.direction = 1
-        
+
         # GUI/user interaction
         self.switch_screen = SwitchScreen(self)
         self.menu_screen = MenuScreen(self)
         self.screensaver = ScreensaverScreen(self)
         self.active_screen = self.switch_screen
-        
+
         self.menu_item = 0              # the active item from the advanced menu
-        
+
         self.load()
-       
+
     def load(self):
         """Load the persistent settings from storage and apply them
         """
         state = self.load_state_json()
-        
+
         self.mode = state.get("mode", self.mode)
         self.num_outputs = state.get("num_outputs", self.num_outputs)
-    
+
     def save(self):
         """Save the current settings to persistent storage
         """
         state = {
             "mode": self.mode,
             "num_outputs": self.num_outputs
         }
         self.save_state_json(state)
-        
+
     @classmethod
     def display_name(cls):
         return "Seq. Switch"
-    
+
     def on_trigger(self):
         """Handler for the rising edge of the input clock
 
         Also used for manually advancing the output on a button press
         """
         # to save on clock cycles, don't use modular arithmetic
         # instead just to integer math and handle roll-over manually
@@ -216,71 +216,71 @@
             next_out = next_out + 1
         elif self.mode == MODE_REVERSE:
             next_out = next_out - 1
         elif self.mode == MODE_PINGPONG:
             next_out = next_out + self.direction
         else:
             next_out = random.randint(0, self.num_outputs-1)
-            
+
         if next_out < 0:
             if self.mode == MODE_REVERSE:
                 next_out = self.num_outputs-1
             else:
                 next_out = -next_out
                 self.direction = -self.direction
         elif next_out >= self.num_outputs:
             if self.mode == MODE_SEQUENTIAL:
                 next_out = 0
             else:
                 next_out = self.num_outputs-2
                 self.direction = -self.direction
-                
+
         self.current_output = next_out
-    
+
     def main(self):
         """The main loop
 
         Connects event handlers for clock-in and button presses
         and runs the main loop
         """
-        
+
         @din.handler
         def on_rising_clock():
             self.on_trigger()
-            
+
         @b1.handler
         def on_b1_press():
             self.last_interaction_time = time.ticks_ms()
             self.active_screen.on_button1()
-            
+
         @b2.handler
         def on_b2_press():
             self.last_interaction_time = time.ticks_ms()
-        
+
             if self.active_screen == self.switch_screen:
                 self.active_screen = self.menu_screen
             else:
                 self.active_screen = self.switch_screen
-            
+
         while True:
             # keep the menu items sync'd with the left knob
             self.menu_item = k1.range(len(self.menu_screen.menu_items))
-            
+
             # check if we've been idle for too long; if so, blank the screen
             # to prevent burn-in
             now = time.ticks_ms()
             if time.ticks_diff(now, self.last_interaction_time) > SCREENSAVER_TIMEOUT_MS:
                 self.active_screen = self.screensaver
-            
+
             # read the input and send it to the current output
             # all other outputs should be zero
             input_volts = ain.read_voltage()
             for i in range(len(cvs)):
                 if i == self.current_output:
                     cvs[i].voltage(input_volts)
                 else:
                     cvs[i].voltage(0)
-            
+
             self.active_screen.draw()
-    
+
 if __name__ == "__main__":
     SequentialSwitch().main()
```

### Comparing `micropython-europi-contrib-0.8.1/contrib/smooth_random_voltages.py` & `micropython-europi-contrib-0.9.1/contrib/smooth_random_voltages.py`

 * *Files identical despite different names*

### Comparing `micropython-europi-contrib-0.8.1/contrib/strange_attractor.py` & `micropython-europi-contrib-0.9.1/contrib/strange_attractor.py`

 * *Files identical despite different names*

### Comparing `micropython-europi-contrib-0.8.1/contrib/turing_machine.py` & `micropython-europi-contrib-0.9.1/contrib/turing_machine.py`

 * *Files identical despite different names*

### Comparing `micropython-europi-contrib-0.8.1/micropython_europi_contrib.egg-info/SOURCES.txt` & `micropython-europi-contrib-0.9.1/micropython_europi_contrib.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 README.md
 setup.py
 contrib/bernoulli_gates.py
 contrib/coin_toss.py
 contrib/consequencer.py
 contrib/cvecorder.py
 contrib/diagnostic.py
+contrib/envelope_generator.py
 contrib/euclid.py
 contrib/hamlet.py
 contrib/harmonic_lfos.py
 contrib/hello_world.py
 contrib/knob_playground.py
 contrib/logic.py
 contrib/master_clock.py
 contrib/menu.py
 contrib/noddy_holder.py
+contrib/pams.py
 contrib/piconacci.py
 contrib/poly_square.py
 contrib/polyrhythmic_sequencer.py
 contrib/probapoly.py
 contrib/quantizer.py
 contrib/radio_scanner.py
 contrib/scope.py
```

### Comparing `micropython-europi-contrib-0.8.1/setup.py` & `micropython-europi-contrib-0.9.1/setup.py`

 * *Files identical despite different names*

