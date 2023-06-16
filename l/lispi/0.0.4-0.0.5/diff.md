# Comparing `tmp/lispi-0.0.4.tar.gz` & `tmp/lispi-0.0.5.tar.gz`

## Comparing `lispi-0.0.4.tar` & `lispi-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.4/.DS_Store
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 lispi-0.0.4/MANIFEST.in
--rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 lispi-0.0.4/requirements.txt
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.4/example/.DS_Store
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 lispi-0.0.4/example/original_example.ipynb
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 lispi-0.0.4/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.4/src/lispi/.DS_Store
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 lispi-0.0.4/src/lispi/__init__.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 lispi-0.0.4/src/lispi/__main__.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 lispi-0.0.4/src/lispi/revealjs_template.py
--rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 lispi-0.0.4/src/lispi/slideEdit.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 lispi-0.0.4/src/lispi/text2audio.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.4/tests/test_audioText.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.4/tests/test_nbconvert.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.4/tests/test_pyscript.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 lispi-0.0.4/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 lispi-0.0.4/LICENSE
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 lispi-0.0.4/README.md
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 lispi-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 lispi-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.5/.DS_Store
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 lispi-0.0.5/MANIFEST.in
+-rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 lispi-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 lispi-0.0.5/setup.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.5/example/.DS_Store
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 lispi-0.0.5/example/original_example.ipynb
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.5/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 lispi-0.0.5/src/lispi/.DS_Store
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 lispi-0.0.5/src/lispi/__init__.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 lispi-0.0.5/src/lispi/__main__.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 lispi-0.0.5/src/lispi/lispi.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 lispi-0.0.5/src/lispi/revealjs_template.py
+-rw-r--r--   0        0        0     4422 2020-02-02 00:00:00.000000 lispi-0.0.5/src/lispi/slideEdit.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 lispi-0.0.5/src/lispi/text2audio.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.5/tests/test_audioText.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.5/tests/test_nbconvert.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.5/tests/test_pyscript.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lispi-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 lispi-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3169 2020-02-02 00:00:00.000000 lispi-0.0.5/README.md
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 lispi-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 lispi-0.0.5/PKG-INFO
```

### Comparing `lispi-0.0.4/.DS_Store` & `lispi-0.0.5/.DS_Store`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
 00000010: 0000 1000 0000 040a 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0009  ................
-00000050: 0000 0001 0000 1000 0070 006c 0065 6277  .........p.l.ebw
-00000060: 7370 626c 0000 0000 0000 0000 0000 0000  spbl............
+00000040: 0000 0000 0000 0002 0000 0000 0000 000b  ................
+00000050: 0000 0001 0000 1000 6277 7370 626c 6f62  ........bwspblob
+00000060: 0000 00b8 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -58,74 +58,74 @@
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000400: 0000 0000 0000 0000 0000 0009 0000 0007  ................
-00000410: 0065 0078 0061 006d 0070 006c 0065 6277  .e.x.a.m.p.l.ebw
-00000420: 7370 626c 6f62 0000 00b8 6270 6c69 7374  spblob....bplist
-00000430: 3030 d601 0203 0405 0607 0807 080b 085d  00.............]
-00000440: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
-00000450: 6f77 546f 6f6c 6261 725b 5368 6f77 5461  owToolbar[ShowTa
-00000460: 6256 6965 775f 1014 436f 6e74 6169 6e65  bView_..Containe
-00000470: 7253 686f 7753 6964 6562 6172 5c57 696e  rShowSidebar\Win
-00000480: 646f 7742 6f75 6e64 735b 5368 6f77 5369  dowBounds[ShowSi
-00000490: 6465 6261 7208 0908 095f 1018 7b7b 3335  debar...._..{{35
-000004a0: 372c 2031 3436 7d2c 207b 3932 302c 2034  7, 146}, {920, 4
-000004b0: 3336 7d7d 0908 1523 2f3b 525f 6b6c 6d6e  36}}...#/;R_klmn
-000004c0: 6f8a 0000 0000 0000 0101 0000 0000 0000  o...............
-000004d0: 000d 0000 0000 0000 0000 0000 0000 0000  ................
-000004e0: 008b 0000 0007 0065 0078 0061 006d 0070  .......e.x.a.m.p
-000004f0: 006c 0065 7653 726e 6c6f 6e67 0000 0001  .l.evSrnlong....
-00000500: 0000 0007 004c 0049 0043 0045 004e 0053  .....L.I.C.E.N.S
-00000510: 0045 496c 6f63 626c 6f62 0000 0010 0000  .EIlocblob......
-00000520: 011d 0000 002e ffff ffff ffff 0000 0000  ................
-00000530: 000e 0070 0079 0070 0072 006f 006a 0065  ...p.y.p.r.o.j.e
-00000540: 0063 0074 002e 0074 006f 006d 006c 496c  .c.t...t.o.m.lIl
-00000550: 6f63 626c 6f62 0000 0010 0000 018b 0000  ocblob..........
-00000560: 002e ffff ffff ffff 0000 0000 0009 0052  ...............R
-00000570: 0045 0041 0044 004d 0045 002e 006d 0064  .E.A.D.M.E...m.d
-00000580: 496c 6f63 626c 6f62 0000 0010 0000 01f9  Ilocblob........
-00000590: 0000 002e ffff ffff ffff 0000 0000 0003  ................
-000005a0: 0073 0072 0063 496c 6f63 626c 6f62 0000  .s.r.cIlocblob..
-000005b0: 0010 0000 0041 0000 002e ffff ffff ffff  .....A..........
-000005c0: 0000 0000 0003 0073 0072 0063 6277 7370  .......s.r.cbwsp
-000005d0: 626c 6f62 0000 00b8 6270 6c69 7374 3030  blob....bplist00
-000005e0: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
-000005f0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
-00000600: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
-00000610: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
-00000620: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
-00000630: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-00000640: 6261 7208 0908 095f 1018 7b7b 3131 372c  bar...._..{{117,
-00000650: 2031 3134 7d2c 207b 3932 302c 2034 3336   114}, {920, 436
-00000660: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
-00000670: 0000 0000 0000 0101 0000 0000 0000 000d  ................
-00000680: 0000 0000 0000 0000 0000 0000 0000 008b  ................
-00000690: 0000 0003 0073 0072 0063 7653 726e 6c6f  .....s.r.cvSrnlo
-000006a0: 6e67 0000 0001 0000 0005 0074 0065 0073  ng.........t.e.s
-000006b0: 0074 0073 496c 6f63 626c 6f62 0000 0010  .t.sIlocblob....
-000006c0: 0000 0267 0000 002e ffff ffff ffff 0000  ...g............
-000006d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000730: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000007a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000007b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000400: 0000 0000 0000 0000 0000 000b 0000 0004  ................
+00000410: 002e 0067 0069 0074 6277 7370 626c 6f62  ...g.i.tbwspblob
+00000420: 0000 00b8 6270 6c69 7374 3030 d601 0203  ....bplist00....
+00000430: 0405 0607 0807 080b 085d 5368 6f77 5374  .........]ShowSt
+00000440: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
+00000450: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
+00000460: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
+00000470: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
+00000480: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
+00000490: 0908 095f 1018 7b7b 3335 372c 2031 3436  ..._..{{357, 146
+000004a0: 7d2c 207b 3932 302c 2034 3336 7d7d 0908  }, {920, 436}}..
+000004b0: 1523 2f3b 525f 6b6c 6d6e 6f8a 0000 0000  .#/;R_klmno.....
+000004c0: 0000 0101 0000 0000 0000 000d 0000 0000  ................
+000004d0: 0000 0000 0000 0000 0000 008b 0000 0004  ................
+000004e0: 002e 0067 0069 0074 7653 726e 6c6f 6e67  ...g.i.tvSrnlong
+000004f0: 0000 0001 0000 0007 0065 0078 0061 006d  .........e.x.a.m
+00000500: 0070 006c 0065 6277 7370 626c 6f62 0000  .p.l.ebwspblob..
+00000510: 00b8 6270 6c69 7374 3030 d601 0203 0405  ..bplist00......
+00000520: 0607 0807 080b 085d 5368 6f77 5374 6174  .......]ShowStat
+00000530: 7573 4261 725b 5368 6f77 546f 6f6c 6261  usBar[ShowToolba
+00000540: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
+00000550: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
+00000560: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
+00000570: 735b 5368 6f77 5369 6465 6261 7208 0908  s[ShowSidebar...
+00000580: 095f 1018 7b7b 3335 372c 2031 3436 7d2c  ._..{{357, 146},
+00000590: 207b 3932 302c 2034 3336 7d7d 0908 1523   {920, 436}}...#
+000005a0: 2f3b 525f 6b6c 6d6e 6f8a 0000 0000 0000  /;R_klmno.......
+000005b0: 0101 0000 0000 0000 000d 0000 0000 0000  ................
+000005c0: 0000 0000 0000 0000 008b 0000 0007 0065  ...............e
+000005d0: 0078 0061 006d 0070 006c 0065 7653 726e  .x.a.m.p.l.evSrn
+000005e0: 6c6f 6e67 0000 0001 0000 0007 004c 0049  long.........L.I
+000005f0: 0043 0045 004e 0053 0045 496c 6f63 626c  .C.E.N.S.EIlocbl
+00000600: 6f62 0000 0010 0000 011d 0000 002e ffff  ob..............
+00000610: ffff ffff 0000 0000 000e 0070 0079 0070  ...........p.y.p
+00000620: 0072 006f 006a 0065 0063 0074 002e 0074  .r.o.j.e.c.t...t
+00000630: 006f 006d 006c 496c 6f63 626c 6f62 0000  .o.m.lIlocblob..
+00000640: 0010 0000 018b 0000 002e ffff ffff ffff  ................
+00000650: 0000 0000 0009 0052 0045 0041 0044 004d  .......R.E.A.D.M
+00000660: 0045 002e 006d 0064 496c 6f63 626c 6f62  .E...m.dIlocblob
+00000670: 0000 0010 0000 01f9 0000 002e ffff ffff  ................
+00000680: ffff 0000 0000 0003 0073 0072 0063 496c  .........s.r.cIl
+00000690: 6f63 626c 6f62 0000 0010 0000 0041 0000  ocblob.......A..
+000006a0: 002e ffff ffff ffff 0000 0000 0003 0073  ...............s
+000006b0: 0072 0063 6277 7370 626c 6f62 0000 00b8  .r.cbwspblob....
+000006c0: 6270 6c69 7374 3030 d601 0203 0405 0607  bplist00........
+000006d0: 0807 080b 085d 5368 6f77 5374 6174 7573  .....]ShowStatus
+000006e0: 4261 725b 5368 6f77 546f 6f6c 6261 725b  Bar[ShowToolbar[
+000006f0: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
+00000700: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
+00000710: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
+00000720: 5368 6f77 5369 6465 6261 7208 0908 095f  ShowSidebar...._
+00000730: 1018 7b7b 3131 372c 2031 3134 7d2c 207b  ..{{117, 114}, {
+00000740: 3932 302c 2034 3336 7d7d 0908 1523 2f3b  920, 436}}...#/;
+00000750: 525f 6b6c 6d6e 6f8a 0000 0000 0000 0101  R_klmno.........
+00000760: 0000 0000 0000 000d 0000 0000 0000 0000  ................
+00000770: 0000 0000 0000 008b 0000 0003 0073 0072  .............s.r
+00000780: 0063 7653 726e 6c6f 6e67 0000 0001 0000  .cvSrnlong......
+00000790: 0005 0074 0065 0073 0074 0073 496c 6f63  ...t.e.s.t.sIloc
+000007a0: 626c 6f62 0000 0010 0000 0267 0000 002e  blob.......g....
+000007b0: ffff ffff ffff 0000 0000 0000 0000 0000  ................
 000007c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000800: 0000 0000 0000 0001 0000 0000 0000 080b  ................
 00000810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `lispi-0.0.4/requirements.txt` & `lispi-0.0.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `lispi-0.0.4/example/.DS_Store` & `lispi-0.0.5/example/.DS_Store`

 * *Files identical despite different names*

### Comparing `lispi-0.0.4/example/original_example.ipynb` & `lispi-0.0.5/example/original_example.ipynb`

 * *Files identical despite different names*

### Comparing `lispi-0.0.4/src/lispi/.DS_Store` & `lispi-0.0.5/src/lispi/.DS_Store`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
-00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
+00000010: 0000 1000 0000 0087 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0006  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 0002  ................
 00000050: 0000 0001 0000 1000 0069 006e 005f 005f  .........i.n._._
 00000060: 002e 0070 0000 0000 0000 0000 0000 0000  ...p............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000080: 0000 0000 0000 0000 0000 0002 0000 000b  ................
+00000090: 005f 005f 006d 0061 0069 006e 005f 005f  ._._.m.a.i.n._._
+000000a0: 002e 0070 0079 496c 6f63 626c 6f62 0000  ...p.yIlocblob..
+000000b0: 0010 0000 0041 0000 002e ffff ffff ffff  .....A..........
+000000c0: 0000 0000 000c 0073 006c 0069 0064 0065  .......s.l.i.d.e
+000000d0: 0045 0064 0069 0074 002e 0070 0079 496c  .E.d.i.t...p.yIl
+000000e0: 6f63 626c 6f62 0000 0010 0000 011d 0000  ocblob..........
+000000f0: 002e ffff ffff ffff 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -26,36 +26,36 @@
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0006 0000 000b  ................
-00000210: 005f 005f 006d 0061 0069 006e 005f 005f  ._._.m.a.i.n._._
-00000220: 002e 0070 0079 496c 6f63 626c 6f62 0000  ...p.yIlocblob..
-00000230: 0010 0000 0041 0000 002e ffff ffff ffff  .....A..........
-00000240: 0000 0000 000a 0065 0078 0061 006d 0070  .......e.x.a.m.p
-00000250: 006c 0065 002e 0070 0079 496c 6f63 626c  .l.e...p.yIlocbl
-00000260: 6f62 0000 0010 0000 00af 0000 002e ffff  ob..............
-00000270: ffff ffff 0000 0000 000d 006d 006f 0064  ...........m.o.d
-00000280: 0069 0066 0069 0065 0064 002e 0068 0074  .i.f.i.e.d...h.t
-00000290: 006d 006c 496c 6f63 626c 6f62 0000 0010  .m.lIlocblob....
-000002a0: 0000 018b 0000 002e ffff ffff ffff 0000  ................
-000002b0: 0000 0009 006e 0065 0077 002e 0069 0070  .....n.e.w...i.p
-000002c0: 0079 006e 0062 496c 6f63 626c 6f62 0000  .y.n.bIlocblob..
-000002d0: 0010 0000 01f9 0000 002e ffff ffff ffff  ................
-000002e0: 0000 0000 000f 006e 0065 0077 002e 0073  .......n.e.w...s
-000002f0: 006c 0069 0064 0065 0073 002e 0068 0074  .l.i.d.e.s...h.t
-00000300: 006d 006c 496c 6f63 626c 6f62 0000 0010  .m.lIlocblob....
-00000310: 0000 0267 0000 002e ffff ffff ffff 0000  ...g............
-00000320: 0000 000c 0073 006c 0069 0064 0065 0045  .....s.l.i.d.e.E
-00000330: 0064 0069 0074 002e 0070 0079 496c 6f63  .d.i.t...p.yIloc
-00000340: 626c 6f62 0000 0010 0000 011d 0000 002e  blob............
-00000350: ffff ffff ffff 0000 0000 0000 0000 0000  ................
+00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000002f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -251,15 +251,15 @@
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0003 0000 0000 0000 100b  ................
-00001010: 0000 0045 0000 0209 0000 0000 0000 0000  ...E............
+00001010: 0000 0045 0000 0087 0000 0000 0000 0000  ...E............
 00001020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -318,15 +318,15 @@
 000013d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001400: 0000 0000 0000 0000 0000 0000 0000 0001  ................
 00001410: 0444 5344 4200 0000 0100 0000 0000 0000  .DSDB...........
 00001420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001430: 0200 0000 2000 0000 6000 0000 0000 0000  .... ...`.......
-00001440: 0100 0000 8000 0000 0100 0001 0000 0000  ................
+00001440: 0000 0000 0100 0001 0000 0000 0100 0002  ................
 00001450: 0000 0000 0100 0004 0000 0000 0200 0008  ................
 00001460: 0000 0018 0000 0000 0000 0000 0100 0020  ............... 
 00001470: 0000 0000 0100 0040 0000 0000 0100 0080  .......@........
 00001480: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001490: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 000014a0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 000014b0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
```

### Comparing `lispi-0.0.4/src/lispi/__main__.py` & `lispi-0.0.5/src/lispi/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,33 +3,32 @@
 import jupyter
 import shutil
 import pkg_resources
 import lispi
 from lispi import *
 
 def main():
+    class Showcase:
+        def __init__(self, index):
+            self._name = index
+        def get_file(self):
+            examples_dir = pkg_resources.resource_filename('lispi', '../../example/original_example.ipynb')
+            if not os.path.exists(os.path.join(os.getcwd(), 'output')):
+                os.makedirs(os.path.join(os.getcwd(), 'output'))
+            shutil.copy(examples_dir, os.getcwd())
+            self.examples_dir = os.getcwd()
+            return self.examples_dir
+        
     index = input("Enter the name of the notebook file: \n")
     if os.path.isfile(index+".ipynb"):
         text2audio.text2audio(index+".ipynb")
         revealjs_template.convert('nbconvert')
         subprocess.run(["jupyter", "nbconvert", index+".ipynb", "--to", "slides"])
         slideEdit._ess(index)
     elif index=="original_example":
-        class Showcase:
-            def __init__(self, index):
-                self._name = index
-            def get_file(self):
-                examples_dir = pkg_resources.resource_filename('lispi', '../../example/original_example.ipynb')
-                if not os.path.exists(os.path.join(os.getcwd(), 'output')):
-                    os.makedirs(os.path.join(os.getcwd(), 'output'))
-                shutil.copy(examples_dir, os.getcwd())
-                self.examples_dir = os.getcwd()
-                return self.examples_dir
-        
-        
         examples_dir=Showcase(index).get_file()
         text2audio.text2audio(examples_dir+"/original_example.ipynb")
         revealjs_template.convert('nbconvert')
         subprocess.run(["jupyter", "nbconvert", examples_dir+"/original_example.ipynb", "--to", "slides"])
         slideEdit._ess("original_example")
         source_file = os.path.join(examples_dir, 'original_example_lispi.html')
         destination_folder = "./output"
@@ -39,20 +38,21 @@
             item=os.path.join(destination_folder, f)
             print(item)
             if os.path.isfile(item):
                 os.remove(item)
             elif os.path.isdir(item):
                 shutil.rmtree(item)
                 
-        os.remove("original_example.ipynb")
         os.remove("original_example.slides.html")
         shutil.move(source_file, destination_folder)
+        shutil.move("original_example.ipynb",destination_folder)
         shutil.move(os.path.join(examples_dir, 'slides_audios'), destination_folder)
     else:
         print("\n")
         print(f"\"{index}.ipynb\" not found!")
         print("*********************************************")
         print("Make sure you have the notebook and try again!")
         print("*********************************************")
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `lispi-0.0.4/src/lispi/slideEdit.py` & `lispi-0.0.5/src/lispi/slideEdit.py`

 * *Files identical despite different names*

### Comparing `lispi-0.0.4/src/lispi/text2audio.py` & `lispi-0.0.5/src/lispi/text2audio.py`

 * *Files identical despite different names*

### Comparing `lispi-0.0.4/LICENSE` & `lispi-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lispi-0.0.4/README.md` & `lispi-0.0.5/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -9,42 +9,55 @@
 To install `lispi` package, you can use pip, the Python package installer. Open your terminal and run the following command:
 
 ```
 pip install lispi
 ```
 
 ## Usage
+### Command Line Interface
+To use lispi, in your terminal follow these steps:
+After installing the package, you can use the `lispi` command to convert your Jupyter notebook into interactive slides. In your terminal, navigate to the folder containing the notebooks and run the following command:
 
-To use lispi, follow these steps:
+```lispi```
 
-1. Import the `lispi` class from the package:
+Upon running the command, the package will prompt you to enter the path to your Jupyter notebook file. Enter the name of the file press enter. The package will convert the Jupyter notebook into interactive slides and save the output HTML file in the output folder in the same directory as html file and audio file folder.
+
+### Python
+If you want to use lispi in your Python code, you can import the package and use it as a library. To use lispi, in python follow these steps:
+
+1. Import the `Gen` class from the package:
+
+   ```python
+   import lispi
+   ```
+   or 
 
    ```python
-    import lispi
+    from lispi import *
    ```
 
-2. Create an instance of the `InteractiveSlidesGenerator` class:
+2. Create an instance of the `Interactive Slides Generator` class:
 
    ```python
-   generator = lispi()
+   generator = lispi.Gen
    ```
 
 3. Specify the Jupyter notebook file you want to convert:
 
    ```python
    notebook_file = "path/to/your/notebook.ipynb"
    ```
 
 4. Generate the interactive slides:
 
    ```python
-   generator.generate_slides(notebook_file)
+   generator(notebook_file)
    ```
 
-5. The package will convert the Jupyter notebook into interactive slides and save the output HTML file.
+5. The package will convert the Jupyter notebook into interactive slides and save the output HTML file in the output folder in the same directory as html file and audio file folder.
 
 ## Configuration
 
 Lispi provides several configuration options to customize the output slides. You can pass these options as arguments when creating an instance of the `lispi` class. Here are the available configuration options:
 
 - `audio`: Specify if you wish the output without audio (default: "unmute").
 - `output_file`: Specify the output file path for the generated slides (default: "output.html").
@@ -56,25 +69,25 @@
     audio="unmute",
     output_file="path/to/output/slides.html"
 )
 ```
 
 ## Examples
 
-Here are a few examples demonstrating the usage of `lispi`:
+Here is an example that comes with the package. To run the example, in your terminal or python code provide 'original_example' as the file name.
 
 ```python
-from lispi import lispi
+import lispi
 
 # Create an instance of the lispi class
-generator = lispi()
+generator = lispi.Gen
 
-# Specify the Jupyter notebook file
-notebook_file = "path/to/your/notebook.ipynb"
+# Specify the example notebook file
+notebook_file = "original_example"
 
 # Generate the interactive slides
-generator.generate_slides(notebook_file)
+generator(notebook_file)
 ```
 
 ## Conclusion
 
 Lispi package provides a convenient way to convert Jupyter notebooks into interactive slides. It allows users to create engaging presentations with interactive elements easily. By following the installation and usage instructions outlined in this documentation, you can leverage this package to generate interactive slides from your Jupyter notebooks effortlessly.
```

### Comparing `lispi-0.0.4/pyproject.toml` & `lispi-0.0.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.include]
 include = [".example/**"]
 
 [project]
 name = "lispi"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="B7M", email="ibsnetwork001@gmail.com" },
 ]
 license = { file = "LICENSE" }
 description = "A simple python package for generating live notebooks where you can write code and run it in real time."
 readme = "README.md"
 requires-python = ">=3.7"
@@ -38,22 +38,23 @@
 Homepage = "https://github.com/B7M/lispi"
 
 [project.scripts]
 lispi = "lispi.__main__:main"
 
 
 [tool.bumpver]
-current_version = "0.0.4"
+current_version = "0.0.5"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'version = "{version}"',
 ]
 "README.md" = [
     "{version}",
     "{pep440_version}",
-]
+]
+"src/lispi/__init__.py" = ["{version}"]
```

### Comparing `lispi-0.0.4/PKG-INFO` & `lispi-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lispi
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple python package for generating live notebooks where you can write code and run it in real time.
 Project-URL: Homepage, https://github.com/B7M/lispi
 Author-email: B7M <ibsnetwork001@gmail.com>
 License: Copyright (c) 2023 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -49,42 +49,55 @@
 To install `lispi` package, you can use pip, the Python package installer. Open your terminal and run the following command:
 
 ```
 pip install lispi
 ```
 
 ## Usage
+### Command Line Interface
+To use lispi, in your terminal follow these steps:
+After installing the package, you can use the `lispi` command to convert your Jupyter notebook into interactive slides. In your terminal, navigate to the folder containing the notebooks and run the following command:
 
-To use lispi, follow these steps:
+```lispi```
 
-1. Import the `lispi` class from the package:
+Upon running the command, the package will prompt you to enter the path to your Jupyter notebook file. Enter the name of the file press enter. The package will convert the Jupyter notebook into interactive slides and save the output HTML file in the output folder in the same directory as html file and audio file folder.
+
+### Python
+If you want to use lispi in your Python code, you can import the package and use it as a library. To use lispi, in python follow these steps:
+
+1. Import the `Gen` class from the package:
+
+   ```python
+   import lispi
+   ```
+   or 
 
    ```python
-    import lispi
+    from lispi import *
    ```
 
-2. Create an instance of the `InteractiveSlidesGenerator` class:
+2. Create an instance of the `Interactive Slides Generator` class:
 
    ```python
-   generator = lispi()
+   generator = lispi.Gen
    ```
 
 3. Specify the Jupyter notebook file you want to convert:
 
    ```python
    notebook_file = "path/to/your/notebook.ipynb"
    ```
 
 4. Generate the interactive slides:
 
    ```python
-   generator.generate_slides(notebook_file)
+   generator(notebook_file)
    ```
 
-5. The package will convert the Jupyter notebook into interactive slides and save the output HTML file.
+5. The package will convert the Jupyter notebook into interactive slides and save the output HTML file in the output folder in the same directory as html file and audio file folder.
 
 ## Configuration
 
 Lispi provides several configuration options to customize the output slides. You can pass these options as arguments when creating an instance of the `lispi` class. Here are the available configuration options:
 
 - `audio`: Specify if you wish the output without audio (default: "unmute").
 - `output_file`: Specify the output file path for the generated slides (default: "output.html").
@@ -96,25 +109,25 @@
     audio="unmute",
     output_file="path/to/output/slides.html"
 )
 ```
 
 ## Examples
 
-Here are a few examples demonstrating the usage of `lispi`:
+Here is an example that comes with the package. To run the example, in your terminal or python code provide 'original_example' as the file name.
 
 ```python
-from lispi import lispi
+import lispi
 
 # Create an instance of the lispi class
-generator = lispi()
+generator = lispi.Gen
 
-# Specify the Jupyter notebook file
-notebook_file = "path/to/your/notebook.ipynb"
+# Specify the example notebook file
+notebook_file = "original_example"
 
 # Generate the interactive slides
-generator.generate_slides(notebook_file)
+generator(notebook_file)
 ```
 
 ## Conclusion
 
 Lispi package provides a convenient way to convert Jupyter notebooks into interactive slides. It allows users to create engaging presentations with interactive elements easily. By following the installation and usage instructions outlined in this documentation, you can leverage this package to generate interactive slides from your Jupyter notebooks effortlessly.
```

