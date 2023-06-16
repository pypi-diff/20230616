# Comparing `tmp/cloud_tts_tool-0.0.74.tar.gz` & `tmp/cloud_tts_tool-0.0.75.tar.gz`

## Comparing `cloud_tts_tool-0.0.74.tar` & `cloud_tts_tool-0.0.75.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.74/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.74/src/.DS_Store
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.74/src/cloud_tts_tool/__init__.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.74/src/cloud_tts_tool/aws_cloud.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.74/src/cloud_tts_tool/azure_cloud.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.74/src/cloud_tts_tool/google_cloud.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.74/src/cloud_tts_tool/main.py
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.74/src/cloud_tts_tool/text_blocks.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.74/.gitignore
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.74/LICENSE
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.74/README.md
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.74/pyproject.toml
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.74/PKG-INFO
+-rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.75/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.75/src/.DS_Store
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.75/src/cloud_tts_tool/__init__.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.75/src/cloud_tts_tool/aws_cloud.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.75/src/cloud_tts_tool/azure_cloud.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.75/src/cloud_tts_tool/google_cloud.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.75/src/cloud_tts_tool/main.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.75/src/cloud_tts_tool/text_blocks.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.75/.gitignore
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.75/LICENSE
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.75/README.md
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.75/pyproject.toml
+-rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 cloud_tts_tool-0.0.75/PKG-INFO
```

### Comparing `cloud_tts_tool-0.0.74/.DS_Store` & `cloud_tts_tool-0.0.75/.DS_Store`

 * *Files 25% similar despite different names*

```diff
@@ -282,125 +282,125 @@
 00001190: 3231 362c 2033 397d 2c20 7b39 3230 2c20  216, 39}, {920, 
 000011a0: 3436 347d 7d09 0815 232f 3b52 5f6b 6c6d  464}}...#/;R_klm
 000011b0: 6e6f 8900 0000 0000 0001 0100 0000 0000  no..............
 000011c0: 0000 0d00 0000 0000 0000 0000 0000 0000  ................
 000011d0: 0000 8a00 0000 0400 6400 6900 7300 746c  ........d.i.s.tl
 000011e0: 6731 5363 6f6d 7000 0000 0000 0050 8f00  g1Scomp......P..
 000011f0: 0000 0400 6400 6900 7300 746c 7376 4362  ....d.i.s.tlsvCb
-00001200: 6c6f 6200 0003 0a62 706c 6973 7430 30d8  lob....bplist00.
-00001210: 0102 0304 0506 0708 090a 0b1b 5758 0a5a  ............WX.Z
-00001220: 5869 636f 6e53 697a 655f 100f 7368 6f77  XiconSize_..show
-00001230: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
-00001240: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
-00001250: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
-00001260: 5a73 6f72 7443 6f6c 756d 6e5f 1010 7573  ZsortColumn_..us
-00001270: 6552 656c 6174 6976 6544 6174 6573 5f10  eRelativeDates_.
-00001280: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
-00001290: 696f 6e23 4030 0000 0000 0000 09ae 0c15  ion#@0..........
-000012a0: 1d22 272c 3136 3b40 4549 4e52 d40d 0e0f  ."',16;@EINR....
-000012b0: 1011 120a 0a5a 6964 656e 7469 6669 6572  .....Zidentifier
-000012c0: 5577 6964 7468 5961 7363 656e 6469 6e67  UwidthYascending
-000012d0: 5776 6973 6962 6c65 546e 616d 6510 f209  WvisibleTname...
-000012e0: 09d4 0d16 1718 191a 1b1b 5577 6964 7468  ..........Uwidth
-000012f0: 5961 7363 656e 6469 6e67 5776 6973 6962  YascendingWvisib
-00001300: 6c65 5875 6269 7175 6974 7910 2308 08d4  leXubiquity.#...
-00001310: 0d0e 0f10 1e1f 1b0a 5c64 6174 654d 6f64  ........\dateMod
-00001320: 6966 6965 6410 7008 09d4 100e 0f0d 1b24  ified.p........$
-00001330: 1b26 0810 b508 5b64 6174 6543 7265 6174  .&....[dateCreat
-00001340: 6564 d410 0e0f 0d0a 291b 2b09 1061 0854  ed......).+..a.T
-00001350: 7369 7a65 d410 0e0f 0d0a 2e0a 3009 1073  size........0..s
-00001360: 0954 6b69 6e64 d410 0e0f 0d1b 330a 3508  .Tkind......3.5.
-00001370: 1064 0955 6c61 6265 6cd4 100e 0f0d 1b38  .d.Ulabel......8
-00001380: 0a3a 0810 4b09 5776 6572 7369 6f6e d410  .:..K.Wversion..
-00001390: 0e0f 0d1b 3d0a 3f08 1101 2c09 5863 6f6d  ....=.?...,.Xcom
-000013a0: 6d65 6e74 73d4 100e 0f0d 1b42 1b44 0810  ments......B.D..
-000013b0: c808 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
-000013c0: 64d4 0d16 1718 4624 1b1b 5964 6174 6541  d.....F$..YdateA
-000013d0: 6464 6564 0808 d418 1617 0d1b 4b1b 4d08  dded........K.M.
-000013e0: 10d2 085a 7368 6172 654f 776e 6572 d418  ...ZshareOwner..
-000013f0: 1617 0d1b 4b1b 5108 085f 100f 7368 6172  ....K.Q.._..shar
-00001400: 654c 6173 7445 6469 746f 72d4 1816 170d  eLastEditor.....
-00001410: 1b4b 1b55 0808 5f10 1069 6e76 6974 6174  .K.U.._..invitat
-00001420: 696f 6e53 7461 7475 7308 2340 2800 0000  ionStatus.#@(...
-00001430: 0000 0054 6e61 6d65 0910 0100 0800 1900  ...Tname........
-00001440: 2200 3400 3c00 5000 5900 6400 7700 8c00  ".4.<.P.Y.d.w...
-00001450: 9500 9600 a500 ae00 b900 bf00 c900 d100  ................
-00001460: d600 d800 d900 da00 e300 e900 f300 fb01  ................
-00001470: 0401 0601 0701 0801 1101 1e01 2001 2101  ............ .!.
-00001480: 2201 2b01 2c01 2e01 2f01 3b01 4401 4501  ".+.,.../.;.D.E.
-00001490: 4701 4801 4d01 5601 5701 5901 5a01 5f01  G.H.M.V.W.Y.Z._.
-000014a0: 6801 6901 6b01 6c01 7201 7b01 7c01 7e01  h.i.k.l.r.{.|.~.
-000014b0: 7f01 8701 9001 9101 9401 9501 9e01 a701  ................
-000014c0: a801 aa01 ab01 ba01 c301 cd01 ce01 cf01  ................
-000014d0: d801 d901 db01 dc01 e701 f001 f101 f202  ................
-000014e0: 0402 0d02 0e02 0f02 2202 2302 2c02 3102  ........".#.,.1.
-000014f0: 3200 0000 0000 0002 0100 0000 0000 0000  2...............
-00001500: 5b00 0000 0000 0000 0000 0000 0000 0002  [...............
-00001510: 3400 0000 0400 6400 6900 7300 746c 7376  4.....d.i.s.tlsv
-00001520: 7062 6c6f 6200 0002 6162 706c 6973 7430  pblob...abplist0
-00001530: 30d8 0102 0304 0506 0708 090a 0b1d 4748  0.............GH
-00001540: 0a36 5869 636f 6e53 697a 655f 100f 7368  .6XiconSize_..sh
-00001550: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
-00001560: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
-00001570: 6541 6c6c 5369 7a65 7358 7465 7874 5369  eAllSizesXtextSi
-00001580: 7a65 5a73 6f72 7443 6f6c 756d 6e5f 1010  zeZsortColumn_..
-00001590: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-000015a0: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
-000015b0: 7273 696f 6e23 4030 0000 0000 0000 09d9  rsion#@0........
-000015c0: 0c0d 0e0f 1011 1213 1415 1e23 282d 3237  ...........#(-27
-000015d0: 3c41 5863 6f6d 6d65 6e74 7355 6c61 6265  <AXcommentsUlabe
-000015e0: 6c57 7665 7273 696f 6e5b 6461 7465 4372  lWversion[dateCr
-000015f0: 6561 7465 6454 7369 7a65 5c64 6174 654d  eatedTsize\dateM
-00001600: 6f64 6966 6965 6454 6b69 6e64 546e 616d  odifiedTkindTnam
-00001610: 655e 6461 7465 4c61 7374 4f70 656e 6564  e^dateLastOpened
-00001620: d416 1718 191a 1b0a 1d55 696e 6465 7855  .........UindexU
-00001630: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
-00001640: 7669 7369 626c 6510 0711 012c 0908 d416  visible....,....
-00001650: 1718 191f 200a 1d10 0510 6409 08d4 1617  .... .....d.....
-00001660: 1819 2425 0a1d 1006 104b 0908 d416 1718  ..$%.....K......
-00001670: 1929 2a1d 1d10 0210 b508 08d4 1617 1819  .)*.............
-00001680: 2e2f 1d0a 1003 1061 0809 d419 1718 160a  ./.....a........
-00001690: 341d 3609 1070 0810 01d4 1617 1819 3839  4.6..p........89
-000016a0: 0a0a 1004 1073 0909 d419 1718 160a 3e0a  .....s........>.
-000016b0: 4009 10f2 0910 00d4 1617 1819 4243 1d1d  @...........BC..
-000016c0: 1008 10c8 0808 0823 4028 0000 0000 0000  .......#@(......
-000016d0: 546e 616d 6509 0008 0019 0022 0034 003c  Tname......".4.<
-000016e0: 0050 0059 0064 0077 008c 0095 0096 00a9  .P.Y.d.w........
-000016f0: 00b2 00b8 00c0 00cc 00d1 00de 00e3 00e8  ................
-00001700: 00f7 0100 0106 010c 0116 011e 0120 0123  ............. .#
-00001710: 0124 0125 012e 0130 0132 0133 0134 013d  .$.%...0.2.3.4.=
-00001720: 013f 0141 0142 0143 014c 014e 0150 0151  .?.A.B.C.L.N.P.Q
-00001730: 0152 015b 015d 015f 0160 0161 016a 016b  .R.[.]._.`.a.j.k
-00001740: 016d 016e 0170 0179 017b 017d 017e 017f  .m.n.p.y.{.}.~..
-00001750: 0188 0189 018b 018c 018e 0197 0199 019b  ................
-00001760: 019c 019d 019e 01a7 01ac 0000 0000 0000  ................
-00001770: 0201 0000 0000 0000 004a 0000 0000 0000  .........J......
-00001780: 0000 0000 0000 0000 01ad 0000 0004 0064  ...............d
-00001790: 0069 0073 0074 6d6f 4444 626c 6f62 0000  .i.s.tmoDDblob..
-000017a0: 0008 f014 b9c0 4e1b c541 0000 0004 0064  ......N..A.....d
-000017b0: 0069 0073 0074 6d6f 6444 626c 6f62 0000  .i.s.tmodDblob..
-000017c0: 0008 f014 b9c0 4e1b c541 0000 0004 0064  ......N..A.....d
-000017d0: 0069 0073 0074 7068 3153 636f 6d70 0000  .i.s.tph1Scomp..
-000017e0: 0000 0000 6000 0000 0004 0064 0069 0073  ....`......d.i.s
-000017f0: 0074 7653 726e 6c6f 6e67 0000 0001 0000  .tvSrnlong......
-00001800: 0003 0073 0072 0063 6c67 3153 636f 6d70  ...s.r.clg1Scomp
-00001810: 0000 0000 0000 5ed0 0000 0003 0073 0072  ......^......s.r
-00001820: 0063 6d6f 4444 626c 6f62 0000 0008 d4d9  .cmoDDblob......
-00001830: 785e a91a c541 0000 0003 0073 0072 0063  x^...A.....s.r.c
-00001840: 6d6f 6444 626c 6f62 0000 0008 d4d9 785e  modDblob......x^
-00001850: a91a c541 0000 0003 0073 0072 0063 7068  ...A.....s.r.cph
-00001860: 3153 636f 6d70 0000 0000 0000 e000 0000  1Scomp..........
-00001870: 0005 0074 0065 0073 0074 0073 6c67 3153  ...t.e.s.t.slg1S
-00001880: 636f 6d70 0000 0000 0000 0000 0000 0005  comp............
-00001890: 0074 0065 0073 0074 0073 6d6f 4444 626c  .t.e.s.t.smoDDbl
+00001200: 6c6f 6200 0002 e862 706c 6973 7430 30d8  lob....bplist00.
+00001210: 0102 0304 0506 0708 090a 0b16 5354 550a  ............STU.
+00001220: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
+00001230: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
+00001240: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
+00001250: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
+00001260: 7a65 7358 7465 7874 5369 7a65 5a73 6f72  zesXtextSizeZsor
+00001270: 7443 6f6c 756d 6e58 6963 6f6e 5369 7a65  tColumnXiconSize
+00001280: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+00001290: 7465 7310 0109 ae0c 151a 1f24 292e 3338  tes........$).38
+000012a0: 3d42 464a 4ed4 0d0e 0f10 0a12 0a14 5776  =BFJN.........Wv
+000012b0: 6973 6962 6c65 5577 6964 7468 5961 7363  isibleUwidthYasc
+000012c0: 656e 6469 6e67 5a69 6465 6e74 6966 6965  endingZidentifie
+000012d0: 7209 10d2 0954 6e61 6d65 d40d 0e0f 1016  r....Tname......
+000012e0: 1716 1908 1023 0858 7562 6971 7569 7479  .....#.Xubiquity
+000012f0: d40d 0e0f 100a 1c16 1e09 1070 085c 6461  ...........p.\da
+00001300: 7465 4d6f 6469 6669 6564 d410 0e0f 0d20  teModified..... 
+00001310: 2116 165b 6461 7465 4372 6561 7465 6410  !..[dateCreated.
+00001320: b508 08d4 100e 0f0d 2526 160a 5473 697a  ........%&..Tsiz
+00001330: 6510 6108 09d4 100e 0f0d 2a2b 0a0a 546b  e.a.......*+..Tk
+00001340: 696e 6410 7309 09d4 100e 0f0d 2f30 0a16  ind.s......./0..
+00001350: 556c 6162 656c 1064 0908 d410 0e0f 0d34  Ulabel.d.......4
+00001360: 350a 1657 7665 7273 696f 6e10 4b09 08d4  5..Wversion.K...
+00001370: 100e 0f0d 393a 0a16 5863 6f6d 6d65 6e74  ....9:..Xcomment
+00001380: 7311 012c 0908 d410 0e0f 0d3e 3f16 165e  s..,.......>?..^
+00001390: 6461 7465 4c61 7374 4f70 656e 6564 10c8  dateLastOpened..
+000013a0: 0808 d40d 0e0f 1016 2116 4508 0859 6461  ........!.E..Yda
+000013b0: 7465 4164 6465 64d4 100e 0f0d 4712 1616  teAdded.....G...
+000013c0: 5a73 6861 7265 4f77 6e65 7208 08d4 100e  ZshareOwner.....
+000013d0: 0f0d 4b12 1616 5f10 0f73 6861 7265 4c61  ..K..._..shareLa
+000013e0: 7374 4564 6974 6f72 0808 d410 0e0f 0d4f  stEditor.......O
+000013f0: 1216 165f 1010 696e 7669 7461 7469 6f6e  ..._..invitation
+00001400: 5374 6174 7573 0808 0823 4028 0000 0000  Status...#@(....
+00001410: 0000 546e 616d 6523 4030 0000 0000 0000  ..Tname#@0......
+00001420: 0900 0800 1900 2e00 4000 4800 5c00 6500  ........@.H.\.e.
+00001430: 7000 7900 8c00 8e00 8f00 9e00 a700 af00  p.y.............
+00001440: b500 bf00 ca00 cb00 cd00 ce00 d300 dc00  ................
+00001450: dd00 df00 e000 e900 f200 f300 f500 f601  ................
+00001460: 0301 0c01 1801 1a01 1b01 1c01 2501 2a01  ............%.*.
+00001470: 2c01 2d01 2e01 3701 3c01 3e01 3f01 4001  ,.-...7.<.>.?.@.
+00001480: 4901 4f01 5101 5201 5301 5c01 6401 6601  I.O.Q.R.S.\.d.f.
+00001490: 6701 6801 7101 7a01 7d01 7e01 7f01 8801  g.h.q.z.}.~.....
+000014a0: 9701 9901 9a01 9b01 a401 a501 a601 b001  ................
+000014b0: b901 c401 c501 c601 cf01 e101 e201 e301  ................
+000014c0: ec01 ff02 0002 0102 0202 0b02 1002 1900  ................
+000014d0: 0000 0000 0002 0100 0000 0000 0000 5700  ..............W.
+000014e0: 0000 0000 0000 0000 0000 0000 0002 1a00  ................
+000014f0: 0000 0400 6400 6900 7300 746c 7376 7062  ....d.i.s.tlsvpb
+00001500: 6c6f 6200 0002 6162 706c 6973 7430 30d8  lob...abplist00.
+00001510: 0102 0304 0506 0708 090a 0b1a 4647 480a  ............FGH.
+00001520: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
+00001530: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
+00001540: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
+00001550: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
+00001560: 7a65 7358 7465 7874 5369 7a65 5a73 6f72  zesXtextSizeZsor
+00001570: 7443 6f6c 756d 6e58 6963 6f6e 5369 7a65  tColumnXiconSize
+00001580: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+00001590: 7465 7310 0109 d90c 0d0e 0f10 1112 1314  tes.............
+000015a0: 151e 2328 2d32 363b 4058 636f 6d6d 656e  ..#(-26;@Xcommen
+000015b0: 7473 556c 6162 656c 5776 6572 7369 6f6e  tsUlabelWversion
+000015c0: 5b64 6174 6543 7265 6174 6564 5473 697a  [dateCreatedTsiz
+000015d0: 655c 6461 7465 4d6f 6469 6669 6564 546b  e\dateModifiedTk
+000015e0: 696e 6454 6e61 6d65 5e64 6174 654c 6173  indTname^dateLas
+000015f0: 744f 7065 6e65 64d4 1617 1819 1a1b 0a1d  tOpened.........
+00001600: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
+00001610: 7363 656e 6469 6e67 5569 6e64 6578 0811  scendingUindex..
+00001620: 012c 0910 07d4 1617 1819 1a20 0a22 0810  .,......... ."..
+00001630: 6409 1005 d416 1718 191a 250a 2708 104b  d.........%.'..K
+00001640: 0910 06d4 1617 1819 1a2a 1a2c 0810 b508  .........*.,....
+00001650: 1002 d416 1718 190a 2f1a 3109 1061 0810  ......../.1..a..
+00001660: 03d4 1917 1816 0933 1a0a 1070 0809 d416  .......3...p....
+00001670: 1718 190a 380a 3a09 1073 0910 04d4 1917  ....8.:..s......
+00001680: 1816 3c3d 0a0a 1000 10d2 0909 d416 1718  ..<=............
+00001690: 191a 421a 4408 10c8 0810 0808 2340 2800  ..B.D.......#@(.
+000016a0: 0000 0000 0054 6e61 6d65 2340 3000 0000  .....Tname#@0...
+000016b0: 0000 0009 0008 0019 002e 0040 0048 005c  ...........@.H.\
+000016c0: 0065 0070 0079 008c 008e 008f 00a2 00ab  .e.p.y..........
+000016d0: 00b1 00b9 00c5 00ca 00d7 00dc 00e1 00f0  ................
+000016e0: 00f9 0101 0107 0111 0117 0118 011b 011c  ................
+000016f0: 011e 0127 0128 012a 012b 012d 0136 0137  ...'.(.*.+.-.6.7
+00001700: 0139 013a 013c 0145 0146 0148 0149 014b  .9.:.<.E.F.H.I.K
+00001710: 0154 0155 0157 0158 015a 0163 0165 0166  .T.U.W.X.Z.c.e.f
+00001720: 0167 0170 0171 0173 0174 0176 017f 0181  .g.p.q.s.t.v....
+00001730: 0183 0184 0185 018e 018f 0191 0192 0194  ................
+00001740: 0195 019e 01a3 01ac 0000 0000 0000 0201  ................
+00001750: 0000 0000 0000 004a 0000 0000 0000 0000  .......J........
+00001760: 0000 0000 0000 01ad 0000 0004 0064 0069  .............d.i
+00001770: 0073 0074 6d6f 4444 626c 6f62 0000 0008  .s.tmoDDblob....
+00001780: f014 b9c0 4e1b c541 0000 0004 0064 0069  ....N..A.....d.i
+00001790: 0073 0074 6d6f 6444 626c 6f62 0000 0008  .s.tmodDblob....
+000017a0: f014 b9c0 4e1b c541 0000 0004 0064 0069  ....N..A.....d.i
+000017b0: 0073 0074 7068 3153 636f 6d70 0000 0000  .s.tph1Scomp....
+000017c0: 0000 6000 0000 0004 0064 0069 0073 0074  ..`......d.i.s.t
+000017d0: 7653 726e 6c6f 6e67 0000 0001 0000 0003  vSrnlong........
+000017e0: 0073 0072 0063 6c67 3153 636f 6d70 0000  .s.r.clg1Scomp..
+000017f0: 0000 0000 5ed0 0000 0003 0073 0072 0063  ....^......s.r.c
+00001800: 6d6f 4444 626c 6f62 0000 0008 d4d9 785e  moDDblob......x^
+00001810: a91a c541 0000 0003 0073 0072 0063 6d6f  ...A.....s.r.cmo
+00001820: 6444 626c 6f62 0000 0008 d4d9 785e a91a  dDblob......x^..
+00001830: c541 0000 0003 0073 0072 0063 7068 3153  .A.....s.r.cph1S
+00001840: 636f 6d70 0000 0000 0000 e000 0000 0005  comp............
+00001850: 0074 0065 0073 0074 0073 6c67 3153 636f  .t.e.s.t.slg1Sco
+00001860: 6d70 0000 0000 0000 0000 0000 0005 0074  mp.............t
+00001870: 0065 0073 0074 0073 6d6f 4444 626c 6f62  .e.s.t.smoDDblob
+00001880: 0000 0008 82d9 b31f 831a c541 0000 0005  ...........A....
+00001890: 0074 0065 0073 0074 0073 6d6f 6444 626c  .t.e.s.t.smodDbl
 000018a0: 6f62 0000 0008 82d9 b31f 831a c541 0000  ob...........A..
-000018b0: 0005 0074 0065 0073 0074 0073 6d6f 6444  ...t.e.s.t.smodD
-000018c0: 626c 6f62 0000 0008 82d9 b31f 831a c541  blob...........A
-000018d0: 0000 0005 0074 0065 0073 0074 0073 7068  .....t.e.s.t.sph
-000018e0: 3153 636f 6d70 0000 0000 0000 0000 0000  1Scomp..........
+000018b0: 0005 0074 0065 0073 0074 0073 7068 3153  ...t.e.s.t.sph1S
+000018c0: 636f 6d70 0000 0000 0000 0000 0000 0000  comp............
+000018d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000018e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000018f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001900: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001910: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001920: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001930: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -586,56 +586,56 @@
 00002490: 0100 0200 0000 0000 0100 0400 0000 0000  ................
 000024a0: 0100 0800 0000 0000 0100 1000 0000 0000  ................
 000024b0: 0100 2000 0000 0000 0100 4000 0000 0000  .. .......@.....
 000024c0: 0100 8000 0000 0000 0101 0000 0000 0000  ................
 000024d0: 0102 0000 0000 0000 0104 0000 0000 0000  ................
 000024e0: 0108 0000 0000 0000 0110 0000 0000 0000  ................
 000024f0: 0120 0000 0000 0000 0140 0000 0000 0000  . .......@......
-00002500: 0000 0000 0000 0000 0000 0000 0000 0002  ................
-00002510: 3400 0000 0400 6400 6900 7300 746c 7376  4.....d.i.s.tlsv
-00002520: 7062 6c6f 6200 0002 6162 706c 6973 7430  pblob...abplist0
-00002530: 30d8 0102 0304 0506 0708 090a 0b1d 4748  0.............GH
-00002540: 0a36 5869 636f 6e53 697a 655f 100f 7368  .6XiconSize_..sh
-00002550: 6f77 4963 6f6e 5072 6576 6965 7757 636f  owIconPreviewWco
-00002560: 6c75 6d6e 735f 1011 6361 6c63 756c 6174  lumns_..calculat
-00002570: 6541 6c6c 5369 7a65 7358 7465 7874 5369  eAllSizesXtextSi
-00002580: 7a65 5a73 6f72 7443 6f6c 756d 6e5f 1010  zeZsortColumn_..
-00002590: 7573 6552 656c 6174 6976 6544 6174 6573  useRelativeDates
-000025a0: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
-000025b0: 7273 696f 6e23 4030 0000 0000 0000 09d9  rsion#@0........
-000025c0: 0c0d 0e0f 1011 1213 1415 1e23 282d 3237  ...........#(-27
-000025d0: 3c41 5863 6f6d 6d65 6e74 7355 6c61 6265  <AXcommentsUlabe
-000025e0: 6c57 7665 7273 696f 6e5b 6461 7465 4372  lWversion[dateCr
-000025f0: 6561 7465 6454 7369 7a65 5c64 6174 654d  eatedTsize\dateM
-00002600: 6f64 6966 6965 6454 6b69 6e64 546e 616d  odifiedTkindTnam
-00002610: 655e 6461 7465 4c61 7374 4f70 656e 6564  e^dateLastOpened
-00002620: d416 1718 191a 1b0a 1d55 696e 6465 7855  .........UindexU
-00002630: 7769 6474 6859 6173 6365 6e64 696e 6757  widthYascendingW
-00002640: 7669 7369 626c 6510 0711 012c 0908 d416  visible....,....
-00002650: 1718 191f 200a 1d10 0510 6409 08d4 1617  .... .....d.....
-00002660: 1819 2425 0a1d 1006 104b 0908 d416 1718  ..$%.....K......
-00002670: 1929 2a1d 1d10 0210 b508 08d4 1617 1819  .)*.............
-00002680: 2e2f 1d0a 1003 1061 0809 d419 1718 160a  ./.....a........
-00002690: 341d 3609 1070 0810 01d4 1617 1819 3839  4.6..p........89
-000026a0: 0a0a 1004 1073 0909 d419 1718 160a 3e0a  .....s........>.
-000026b0: 4009 10f2 0910 00d4 1617 1819 4243 1d1d  @...........BC..
-000026c0: 1008 10c8 0808 0823 4028 0000 0000 0000  .......#@(......
-000026d0: 546e 616d 6509 0008 0019 0022 0034 003c  Tname......".4.<
-000026e0: 0050 0059 0064 0077 008c 0095 0096 00a9  .P.Y.d.w........
-000026f0: 00b2 00b8 00c0 00cc 00d1 00de 00e3 00e8  ................
-00002700: 00f7 0100 0106 010c 0116 011e 0120 0123  ............. .#
-00002710: 0124 0125 012e 0130 0132 0133 0134 013d  .$.%...0.2.3.4.=
-00002720: 013f 0141 0142 0143 014c 014e 0150 0151  .?.A.B.C.L.N.P.Q
-00002730: 0152 015b 015d 015f 0160 0161 016a 016b  .R.[.]._.`.a.j.k
-00002740: 016d 016e 0170 0179 017b 017d 017e 017f  .m.n.p.y.{.}.~..
-00002750: 0188 0189 018b 018c 018e 0197 0199 019b  ................
-00002760: 019c 019d 019e 01a7 01ac 0000 0000 0000  ................
-00002770: 0201 0000 0000 0000 004a 0000 0000 0000  .........J......
-00002780: 0000 0000 0000 0000 01ad 0000 0004 0064  ...............d
-00002790: 0069 0073 0074 6d6f 4444 626c 6f62 0000  .i.s.tmoDDblob..
-000027a0: 0008 f014 b9c0 4e1b c541 0000 0004 0064  ......N..A.....d
-000027b0: 0069 0073 0074 6d6f 6444 626c 6f62 0000  .i.s.tmodDblob..
-000027c0: 0008 f014 b9c0 4e1b c541 0000 0004 0064  ......N..A.....d
-000027d0: 0069 0073 0074 7068 3153 636f 6d70 0000  .i.s.tph1Scomp..
-000027e0: 0000 0000 6000 0000 0004 0064 0069 0073  ....`......d.i.s
-000027f0: 0074 7653 726e 6c6f 6e67 0000 0001 0000  .tvSrnlong......
-00002800: 0003 0073                                ...s
+00002500: 006f 6200 0002 6162 706c 6973 7430 30d8  .ob...abplist00.
+00002510: 0102 0304 0506 0708 090a 0b1a 4647 480a  ............FGH.
+00002520: 5f10 1276 6965 774f 7074 696f 6e73 5665  _..viewOptionsVe
+00002530: 7273 696f 6e5f 100f 7368 6f77 4963 6f6e  rsion_..showIcon
+00002540: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
+00002550: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
+00002560: 7a65 7358 7465 7874 5369 7a65 5a73 6f72  zesXtextSizeZsor
+00002570: 7443 6f6c 756d 6e58 6963 6f6e 5369 7a65  tColumnXiconSize
+00002580: 5f10 1075 7365 5265 6c61 7469 7665 4461  _..useRelativeDa
+00002590: 7465 7310 0109 d90c 0d0e 0f10 1112 1314  tes.............
+000025a0: 151e 2328 2d32 363b 4058 636f 6d6d 656e  ..#(-26;@Xcommen
+000025b0: 7473 556c 6162 656c 5776 6572 7369 6f6e  tsUlabelWversion
+000025c0: 5b64 6174 6543 7265 6174 6564 5473 697a  [dateCreatedTsiz
+000025d0: 655c 6461 7465 4d6f 6469 6669 6564 546b  e\dateModifiedTk
+000025e0: 696e 6454 6e61 6d65 5e64 6174 654c 6173  indTname^dateLas
+000025f0: 744f 7065 6e65 64d4 1617 1819 1a1b 0a1d  tOpened.........
+00002600: 5776 6973 6962 6c65 5577 6964 7468 5961  WvisibleUwidthYa
+00002610: 7363 656e 6469 6e67 5569 6e64 6578 0811  scendingUindex..
+00002620: 012c 0910 07d4 1617 1819 1a20 0a22 0810  .,......... ."..
+00002630: 6409 1005 d416 1718 191a 250a 2708 104b  d.........%.'..K
+00002640: 0910 06d4 1617 1819 1a2a 1a2c 0810 b508  .........*.,....
+00002650: 1002 d416 1718 190a 2f1a 3109 1061 0810  ......../.1..a..
+00002660: 03d4 1917 1816 0933 1a0a 1070 0809 d416  .......3...p....
+00002670: 1718 190a 380a 3a09 1073 0910 04d4 1917  ....8.:..s......
+00002680: 1816 3c3d 0a0a 1000 10d2 0909 d416 1718  ..<=............
+00002690: 191a 421a 4408 10c8 0810 0808 2340 2800  ..B.D.......#@(.
+000026a0: 0000 0000 0054 6e61 6d65 2340 3000 0000  .....Tname#@0...
+000026b0: 0000 0009 0008 0019 002e 0040 0048 005c  ...........@.H.\
+000026c0: 0065 0070 0079 008c 008e 008f 00a2 00ab  .e.p.y..........
+000026d0: 00b1 00b9 00c5 00ca 00d7 00dc 00e1 00f0  ................
+000026e0: 00f9 0101 0107 0111 0117 0118 011b 011c  ................
+000026f0: 011e 0127 0128 012a 012b 012d 0136 0137  ...'.(.*.+.-.6.7
+00002700: 0139 013a 013c 0145 0146 0148 0149 014b  .9.:.<.E.F.H.I.K
+00002710: 0154 0155 0157 0158 015a 0163 0165 0166  .T.U.W.X.Z.c.e.f
+00002720: 0167 0170 0171 0173 0174 0176 017f 0181  .g.p.q.s.t.v....
+00002730: 0183 0184 0185 018e 018f 0191 0192 0194  ................
+00002740: 0195 019e 01a3 01ac 0000 0000 0000 0201  ................
+00002750: 0000 0000 0000 004a 0000 0000 0000 0000  .......J........
+00002760: 0000 0000 0000 01ad 0000 0004 0064 0069  .............d.i
+00002770: 0073 0074 6d6f 4444 626c 6f62 0000 0008  .s.tmoDDblob....
+00002780: f014 b9c0 4e1b c541 0000 0004 0064 0069  ....N..A.....d.i
+00002790: 0073 0074 6d6f 6444 626c 6f62 0000 0008  .s.tmodDblob....
+000027a0: f014 b9c0 4e1b c541 0000 0004 0064 0069  ....N..A.....d.i
+000027b0: 0073 0074 7068 3153 636f 6d70 0000 0000  .s.tph1Scomp....
+000027c0: 0000 6000 0000 0004 0064 0069 0073 0074  ..`......d.i.s.t
+000027d0: 7653 726e 6c6f 6e67 0000 0001 0000 0003  vSrnlong........
+000027e0: 0073 0072 0063 6c67 3153 636f 6d70 0000  .s.r.clg1Scomp..
+000027f0: 0000 0000 5ed0 0000 0003 0073 0072 0063  ....^......s.r.c
+00002800: 6d6f 4444                                moDD
```

### Comparing `cloud_tts_tool-0.0.74/src/.DS_Store` & `cloud_tts_tool-0.0.75/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `cloud_tts_tool-0.0.74/src/cloud_tts_tool/aws_cloud.py` & `cloud_tts_tool-0.0.75/src/cloud_tts_tool/aws_cloud.py`

 * *Files identical despite different names*

### Comparing `cloud_tts_tool-0.0.74/src/cloud_tts_tool/azure_cloud.py` & `cloud_tts_tool-0.0.75/src/cloud_tts_tool/azure_cloud.py`

 * *Files identical despite different names*

### Comparing `cloud_tts_tool-0.0.74/src/cloud_tts_tool/google_cloud.py` & `cloud_tts_tool-0.0.75/src/cloud_tts_tool/google_cloud.py`

 * *Files identical despite different names*

### Comparing `cloud_tts_tool-0.0.74/src/cloud_tts_tool/main.py` & `cloud_tts_tool-0.0.75/src/cloud_tts_tool/main.py`

 * *Files identical despite different names*

### Comparing `cloud_tts_tool-0.0.74/src/cloud_tts_tool/text_blocks.py` & `cloud_tts_tool-0.0.75/src/cloud_tts_tool/text_blocks.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,29 +16,30 @@
     text_blocks = []
     intro_ssml = f'''
                     <speak xmlns="http://www.w3.org/2001/10/synthesis" 
                         xmlns:mstts="http://www.w3.org/2001/mstts" 
                         xmlns:emo="http://www.w3.org/2009/10/emotionml" version="1.0" xml:lang="en-US">
                     {voice_tag}
                         <prosody rate="medium">
-                            {style}'''
+                            {style}
+                            '''
     ending_ssml = f'''
                 {end_style}
             </prosody>
         {end_voice_tag}
     </speak>
                 '''
     while (len(rest) > 3000):
         begin = 0
         end = rest.rfind("</p>", 0, 3000)  # rfind looks for the last case of the search term.
         if (end == -1):
             end = rest.rfind(". ", 0, 3000)
             text_block = rest[begin:end + 1]
             rest = rest[end + 1:]
-            text_blocks.append(intro_ssml + text_block + "</p>" + ending_ssml)
+            text_blocks.append(intro_ssml + "<p>" + text_block + "</p>" + ending_ssml)
             rest = "<p>" + rest
         else:
             text_block = rest[begin:end + 4]
             rest = rest[ end + 4:]
             text_blocks.append(intro_ssml + text_block + ending_ssml)
     text_blocks.append( intro_ssml + rest + ending_ssml)
     return text_blocks
```

### Comparing `cloud_tts_tool-0.0.74/LICENSE` & `cloud_tts_tool-0.0.75/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud_tts_tool-0.0.74/README.md` & `cloud_tts_tool-0.0.75/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 Please set keyring items:
 
 Google Cloud:
 https://cloud.google.com/iam/docs/service-accounts-create
 ```python
 #python console
 import keyring
-keyring.set_password("cloud_tts", "google_private_key_id", "<GOOGLE_PRIVATE_KEY_ID_FROM_JSON>")
-keyring.set_password("cloud_tts", "google_private_key", "<GOOGLE_PRIVATE_KEY_FROM_JSON>")
-keyring.set_password("cloud_tts", "google_client_email", "<GOOGLE_CLIENT_EMAIL>")
+keyring.set_password("google_tts", "google_private_key_id", "<GOOGLE_PRIVATE_KEY_ID_FROM_JSON>")
+keyring.set_password("google_tts", "google_private_key", "<GOOGLE_PRIVATE_KEY_FROM_JSON>")
+keyring.set_password("google_tts", "google_client_email", "<GOOGLE_CLIENT_EMAIL>")
 ```
 The other items don't appear to matter.
 
 #AWS Polly:
 in console, IAM, Users, Add user,
 choose a username 
 Attatch Policies Directly
```

### Comparing `cloud_tts_tool-0.0.74/pyproject.toml` & `cloud_tts_tool-0.0.75/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cloud_tts_tool"
-version = "0.0.74"
+version = "0.0.75"
 authors = [
     { name="Ben Brenner", email="ben.brenner@gmail.com" },
     ]
 description = "A tool for requesting text to speech from a variety of cloud APIs."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `cloud_tts_tool-0.0.74/PKG-INFO` & `cloud_tts_tool-0.0.75/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud_tts_tool
-Version: 0.0.74
+Version: 0.0.75
 Summary: A tool for requesting text to speech from a variety of cloud APIs.
 Project-URL: Homepage, https://github.com/cobiadigital/cloud_tts_tools
 Project-URL: Bug Tracker, https://github.com/cobiadigital/cloud_tts_tools/issues
 Author-email: Ben Brenner <ben.brenner@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,17 +23,17 @@
 Please set keyring items:
 
 Google Cloud:
 https://cloud.google.com/iam/docs/service-accounts-create
 ```python
 #python console
 import keyring
-keyring.set_password("cloud_tts", "google_private_key_id", "<GOOGLE_PRIVATE_KEY_ID_FROM_JSON>")
-keyring.set_password("cloud_tts", "google_private_key", "<GOOGLE_PRIVATE_KEY_FROM_JSON>")
-keyring.set_password("cloud_tts", "google_client_email", "<GOOGLE_CLIENT_EMAIL>")
+keyring.set_password("google_tts", "google_private_key_id", "<GOOGLE_PRIVATE_KEY_ID_FROM_JSON>")
+keyring.set_password("google_tts", "google_private_key", "<GOOGLE_PRIVATE_KEY_FROM_JSON>")
+keyring.set_password("google_tts", "google_client_email", "<GOOGLE_CLIENT_EMAIL>")
 ```
 The other items don't appear to matter.
 
 #AWS Polly:
 in console, IAM, Users, Add user,
 choose a username 
 Attatch Policies Directly
```

