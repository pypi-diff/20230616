# Comparing `tmp/PyTransit-2.5.8-py3-none-any.whl.zip` & `tmp/PyTransit-2.5.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 948679 bytes, number of entries: 101
+Zip file size: 948684 bytes, number of entries: 101
 -rw-r--r--  2.0 unx     3823 b- defN 21-May-19 16:26 pytransit/__init__.py
 -rw-r--r--  2.0 unx     3538 b- defN 20-Jan-13 23:32 pytransit/limb_darkening.py
--rw-r--r--  2.0 unx      829 b- defN 21-Jun-08 10:50 pytransit/version.py
+-rw-r--r--  2.0 unx      829 b- defN 21-Jun-08 11:05 pytransit/version.py
 -rw-r--r--  2.0 unx     1603 b- defN 21-May-19 16:26 pytransit/contamination/__init__.py
 -rw-r--r--  2.0 unx    14927 b- defN 21-May-19 16:26 pytransit/contamination/contamination.py
 -rw-r--r--  2.0 unx     4082 b- defN 21-May-19 16:26 pytransit/contamination/filter.py
 -rw-r--r--  2.0 unx     1644 b- defN 21-May-19 16:26 pytransit/contamination/instrument.py
 -rw-r--r--  2.0 unx     5964 b- defN 20-Mar-16 23:34 pytransit/contamination/plotting.py
 -rw-r--r--  2.0 unx   421592 b- defN 20-Jan-13 23:32 pytransit/contamination/data/spectra.h5
 -rw-r--r--  2.0 unx   454764 b- defN 20-Jan-13 23:32 pytransit/contamination/data/transmission.nc
@@ -91,13 +91,13 @@
 -rw-r--r--  2.0 unx     2343 b- defN 20-Apr-08 17:00 pytransit/utils/mdwarfs.py
 -rw-r--r--  2.0 unx     2640 b- defN 21-Jun-08 10:50 pytransit/utils/misc.py
 -rw-r--r--  2.0 unx     3647 b- defN 21-Feb-23 17:25 pytransit/utils/octasphere.py
 -rw-r--r--  2.0 unx    10041 b- defN 20-Sep-16 10:12 pytransit/utils/phasecurves.py
 -rw-r--r--  2.0 unx     1642 b- defN 20-Jun-03 18:30 pytransit/utils/physics.py
 -rw-r--r--  2.0 unx     2570 b- defN 20-May-09 18:55 pytransit/utils/rv.py
 -rw-r--r--  2.0 unx     2331 b- defN 21-Jun-08 10:50 pytransit/utils/tess.py
--rw-r--r--  2.0 unx    18045 b- defN 21-Jun-08 10:59 PyTransit-2.5.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     1028 b- defN 21-Jun-08 10:59 PyTransit-2.5.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Jun-08 10:59 PyTransit-2.5.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 21-Jun-08 10:59 PyTransit-2.5.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     8938 b- defN 21-Jun-08 10:59 PyTransit-2.5.8.dist-info/RECORD
-101 files, 1531690 bytes uncompressed, 934535 bytes compressed:  39.0%
+-rw-r--r--  2.0 unx    18045 b- defN 21-Jun-08 11:06 PyTransit-2.5.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1051 b- defN 21-Jun-08 11:06 PyTransit-2.5.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Jun-08 11:06 PyTransit-2.5.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 21-Jun-08 11:06 PyTransit-2.5.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     8938 b- defN 21-Jun-08 11:06 PyTransit-2.5.9.dist-info/RECORD
+101 files, 1531713 bytes uncompressed, 934540 bytes compressed:  39.0%
```

## zipnote {}

```diff
@@ -282,23 +282,23 @@
 
 Filename: pytransit/utils/rv.py
 Comment: 
 
 Filename: pytransit/utils/tess.py
 Comment: 
 
-Filename: PyTransit-2.5.8.dist-info/LICENSE
+Filename: PyTransit-2.5.9.dist-info/LICENSE
 Comment: 
 
-Filename: PyTransit-2.5.8.dist-info/METADATA
+Filename: PyTransit-2.5.9.dist-info/METADATA
 Comment: 
 
-Filename: PyTransit-2.5.8.dist-info/WHEEL
+Filename: PyTransit-2.5.9.dist-info/WHEEL
 Comment: 
 
-Filename: PyTransit-2.5.8.dist-info/top_level.txt
+Filename: PyTransit-2.5.9.dist-info/top_level.txt
 Comment: 
 
-Filename: PyTransit-2.5.8.dist-info/RECORD
+Filename: PyTransit-2.5.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytransit/version.py

```diff
@@ -12,8 +12,8 @@
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 from semantic_version import Version
 
-__version__ = Version('2.5.8')
+__version__ = Version('2.5.9')
```

## Comparing `PyTransit-2.5.8.dist-info/LICENSE` & `PyTransit-2.5.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `PyTransit-2.5.8.dist-info/METADATA` & `PyTransit-2.5.9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTransit
-Version: 2.5.8
+Version: 2.5.9
 Summary: Fast and painless exoplanet transit light curve modelling.
 Home-page: https://github.com/hpparvi/PyTransit
 Author: Hannu Parviainen
 Author-email: hpparvi@gmail.com
 License: GPLv2
 Keywords: astronomy astrophysics exoplanets
 Platform: UNKNOWN
@@ -21,14 +21,15 @@
 Requires-Dist: pandas
 Requires-Dist: xarray
 Requires-Dist: tables
 Requires-Dist: semantic-version
 Requires-Dist: deprecated
 Requires-Dist: uncertainties
 Requires-Dist: pyrr
+Requires-Dist: seaborn
 Provides-Extra: celerite
 Requires-Dist: celerite ; extra == 'celerite'
 Requires-Dist: pybind11 ; extra == 'celerite'
 
 UNKNOWN
```

## Comparing `PyTransit-2.5.8.dist-info/RECORD` & `PyTransit-2.5.9.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pytransit/__init__.py,sha256=55tq8nBollEWoX-uI-uSVrOUX4SmRhQL-uBExvusJ00,3823
 pytransit/limb_darkening.py,sha256=OeBPhUWXGKe_QFWcuSMv0b1sR6HbCdrYtTlYhPX-L_c,3538
-pytransit/version.py,sha256=EczyZT1K_Ujgjy70Hx2uy31rSFDg4uG-6_KdwWLHcik,829
+pytransit/version.py,sha256=0XG87_V-PYhq0VZbrbzyQd83opJVIKubzzA9qOGHHqs,829
 pytransit/contamination/__init__.py,sha256=l2TQSaQSc5S0-6YVB_VXu1ddr4_H8GAw4ypNBV2lgNY,1603
 pytransit/contamination/contamination.py,sha256=xMLneKPd22ZQ3pBED9qWgNCDlJcdXazjwrYzTWf4E6Y,14927
 pytransit/contamination/filter.py,sha256=XYyt55GSZ-NKbSfV3GygHsbltWkCb0gz3biFT7v1GOs,4082
 pytransit/contamination/instrument.py,sha256=FYxkR_vgqB5Pn0au32OhPtCIR6xU8JYOO_FfFz4yWu0,1644
 pytransit/contamination/plotting.py,sha256=anyl11vxyGat3X1SiKMfExcTxFqJyrW7u9MVnluROyc,5964
 pytransit/contamination/data/spectra.h5,sha256=vKmCJhla9QLEKWMAUjDvPTX---rLFqELWi8mrgRr2iw,421592
 pytransit/contamination/data/transmission.nc,sha256=C5VJo-3YdU0ivmqhLeTQ0_cV_m75WfIVOkdKfowprrs,454764
@@ -90,12 +90,12 @@
 pytransit/utils/mdwarfs.py,sha256=qTS7H3cyo3LkoO5BjSTIOFWB08m9WxjEnqLhVmtkHxk,2343
 pytransit/utils/misc.py,sha256=nJVBYIxEFfkeVQB7FZ5P350CLH5YvUxWEpjWVvsZn48,2640
 pytransit/utils/octasphere.py,sha256=Iwd4Y4t7NFNC46VffKJfvVUeD4aztt-7iGISzfYz0T8,3647
 pytransit/utils/phasecurves.py,sha256=YvtCOrM_jVtYHj4N5BAzx39TMuKYiLbxd1YReXtdE_k,10041
 pytransit/utils/physics.py,sha256=HtOiDfk_PRMdOdk05rty877iRXpWuV89QwbQwAO9ySI,1642
 pytransit/utils/rv.py,sha256=jNf-79080K4sST0Z0ot75h-ewCBSOLYgANVRb9knUNI,2570
 pytransit/utils/tess.py,sha256=YEDU-pbNTm6KVrnyNg0bu9F_madD3pGHp95sf6g-_Zo,2331
-PyTransit-2.5.8.dist-info/LICENSE,sha256=s6DMeIC72jjJFdFX2MTU3lCz_4UCUQAcCMtxAqYBiv0,18045
-PyTransit-2.5.8.dist-info/METADATA,sha256=IG3P6CUTdF5PF8b5o0w9WEUdPj7AilWPCZWtOG-s4AA,1028
-PyTransit-2.5.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-PyTransit-2.5.8.dist-info/top_level.txt,sha256=Y4wC10N9yBBNslkDDVW6JTmTjMRD5GPgu992lWf6rwk,10
-PyTransit-2.5.8.dist-info/RECORD,,
+PyTransit-2.5.9.dist-info/LICENSE,sha256=s6DMeIC72jjJFdFX2MTU3lCz_4UCUQAcCMtxAqYBiv0,18045
+PyTransit-2.5.9.dist-info/METADATA,sha256=ktpQ5MIK6kcA8iJmAD9b-WzSboTY5rZEpn7oV1AOLlk,1051
+PyTransit-2.5.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+PyTransit-2.5.9.dist-info/top_level.txt,sha256=Y4wC10N9yBBNslkDDVW6JTmTjMRD5GPgu992lWf6rwk,10
+PyTransit-2.5.9.dist-info/RECORD,,
```

