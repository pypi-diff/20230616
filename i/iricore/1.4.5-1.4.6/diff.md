# Comparing `tmp/iricore-1.4.5.tar.gz` & `tmp/iricore-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iricore-1.4.5.tar", max compression
+gzip compressed data, was "iricore-1.4.6.tar", max compression
```

## Comparing `iricore-1.4.5.tar` & `iricore-1.4.6.tar`

### file list

```diff
@@ -1,142 +1,141 @@
--rwxr-xr-x   0        0        0     1276 2022-05-03 16:22:41.008931 iricore-1.4.5/LICENSE
--rwxr-xr-x   0        0        0     1254 2023-03-28 01:11:06.672275 iricore-1.4.5/README.md
--rwxr-xr-x   0        0        0      463 2022-11-10 03:07:50.807105 iricore-1.4.5/build.py
--rwxr-xr-x   0        0        0      641 2023-06-12 19:51:37.147261 iricore-1.4.5/pyproject.toml
--rwxr-xr-x   0        0        0      431 2023-05-26 16:38:21.723202 iricore-1.4.5/src/iricore/CMakeLists.txt
--rwxr-xr-x   0        0        0      112 2023-05-05 20:40:56.755640 iricore-1.4.5/src/iricore/__init__.py
--rw-r--r--   0        0        0       44 2023-05-05 22:32:51.315676 iricore-1.4.5/src/iricore/config.py
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.5/src/iricore/data/data16/ccir/ccir11.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.5/src/iricore/data/data16/ccir/ccir12.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.5/src/iricore/data/data16/ccir/ccir13.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.5/src/iricore/data/data16/ccir/ccir14.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.5/src/iricore/data/data16/ccir/ccir15.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.5/src/iricore/data/data16/ccir/ccir16.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.5/src/iricore/data/data16/ccir/ccir17.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.5/src/iricore/data/data16/ccir/ccir18.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.5/src/iricore/data/data16/ccir/ccir19.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.5/src/iricore/data/data16/ccir/ccir20.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.5/src/iricore/data/data16/ccir/ccir21.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.5/src/iricore/data/data16/ccir/ccir22.asc
--rw-r--r--   0        0        0      443 2016-02-04 05:04:35.000000 iricore-1.4.5/src/iricore/data/data16/igrf/dgrf1945.dat
--rw-r--r--   0        0        0      445 2016-02-04 05:04:44.000000 iricore-1.4.5/src/iricore/data/data16/igrf/dgrf1950.dat
--rw-r--r--   0        0        0      437 2016-02-04 05:04:50.000000 iricore-1.4.5/src/iricore/data/data16/igrf/dgrf1955.dat
--rw-r--r--   0        0        0      431 2016-02-04 05:04:58.000000 iricore-1.4.5/src/iricore/data/data16/igrf/dgrf1960.dat
--rw-r--r--   0        0        0      435 2016-02-04 05:05:13.000000 iricore-1.4.5/src/iricore/data/data16/igrf/dgrf1965.dat
--rw-r--r--   0        0        0      435 2016-02-04 05:05:18.000000 iricore-1.4.5/src/iricore/data/data16/igrf/dgrf1970.dat
--rw-r--r--   0        0        0      439 2016-02-04 05:05:25.000000 iricore-1.4.5/src/iricore/data/data16/igrf/dgrf1975.dat
--rw-r--r--   0        0        0      436 2016-02-04 05:05:31.000000 iricore-1.4.5/src/iricore/data/data16/igrf/dgrf1980.dat
--rw-r--r--   0        0        0      433 2016-02-04 05:05:40.000000 iricore-1.4.5/src/iricore/data/data16/igrf/dgrf1985.dat
--rw-r--r--   0        0        0      434 2016-02-04 05:05:58.000000 iricore-1.4.5/src/iricore/data/data16/igrf/dgrf1990.dat
--rw-r--r--   0        0        0      438 2016-02-04 05:06:08.000000 iricore-1.4.5/src/iricore/data/data16/igrf/dgrf1995.dat
--rw-r--r--   0        0        0     1015 2016-02-04 05:06:15.000000 iricore-1.4.5/src/iricore/data/data16/igrf/dgrf2000.dat
--rw-r--r--   0        0        0     1219 2016-02-04 05:06:22.000000 iricore-1.4.5/src/iricore/data/data16/igrf/dgrf2005.dat
--rw-r--r--   0        0        0     1218 2016-02-04 05:06:32.000000 iricore-1.4.5/src/iricore/data/data16/igrf/dgrf2010.dat
--rw-r--r--   0        0        0     1188 2020-04-06 19:51:12.000000 iricore-1.4.5/src/iricore/data/data16/igrf/dgrf2015.dat
--rw-r--r--   0        0        0     1018 2021-09-21 01:36:47.000000 iricore-1.4.5/src/iricore/data/data16/igrf/igrf2020.dat
--rw-r--r--   0        0        0      598 2021-09-21 01:37:16.000000 iricore-1.4.5/src/iricore/data/data16/igrf/igrf2020s.dat
--rwxr-xr-x   0        0        0  1312575 2023-05-05 22:25:06.976848 iricore-1.4.5/src/iricore/data/data16/index/apf107.dat
--rwxr-xr-x   0        0        0     9681 2023-05-05 22:25:07.132847 iricore-1.4.5/src/iricore/data/data16/index/ig_rz.dat
--rw-r--r--   0        0        0    88224 2016-02-04 04:59:17.000000 iricore-1.4.5/src/iricore/data/data16/mcsat/mcsat11.dat
--rw-r--r--   0        0        0    88224 2016-02-04 04:59:21.000000 iricore-1.4.5/src/iricore/data/data16/mcsat/mcsat12.dat
--rw-r--r--   0        0        0    88224 2016-02-04 04:59:26.000000 iricore-1.4.5/src/iricore/data/data16/mcsat/mcsat13.dat
--rw-r--r--   0        0        0    88224 2016-02-04 04:59:31.000000 iricore-1.4.5/src/iricore/data/data16/mcsat/mcsat14.dat
--rw-r--r--   0        0        0    88224 2016-02-04 04:59:35.000000 iricore-1.4.5/src/iricore/data/data16/mcsat/mcsat15.dat
--rw-r--r--   0        0        0    88224 2016-02-04 04:59:47.000000 iricore-1.4.5/src/iricore/data/data16/mcsat/mcsat16.dat
--rw-r--r--   0        0        0    88224 2016-02-04 04:59:56.000000 iricore-1.4.5/src/iricore/data/data16/mcsat/mcsat17.dat
--rw-r--r--   0        0        0    88224 2016-02-04 05:00:05.000000 iricore-1.4.5/src/iricore/data/data16/mcsat/mcsat18.dat
--rw-r--r--   0        0        0    88224 2016-02-04 05:00:12.000000 iricore-1.4.5/src/iricore/data/data16/mcsat/mcsat19.dat
--rw-r--r--   0        0        0    88224 2016-02-04 05:00:19.000000 iricore-1.4.5/src/iricore/data/data16/mcsat/mcsat20.dat
--rw-r--r--   0        0        0    88224 2016-02-04 05:00:27.000000 iricore-1.4.5/src/iricore/data/data16/mcsat/mcsat21.dat
--rw-r--r--   0        0        0    88224 2016-02-04 05:00:33.000000 iricore-1.4.5/src/iricore/data/data16/mcsat/mcsat22.dat
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.5/src/iricore/data/data16/ursi/ursi11.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.5/src/iricore/data/data16/ursi/ursi12.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.5/src/iricore/data/data16/ursi/ursi13.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.5/src/iricore/data/data16/ursi/ursi14.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.5/src/iricore/data/data16/ursi/ursi15.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.5/src/iricore/data/data16/ursi/ursi16.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.5/src/iricore/data/data16/ursi/ursi17.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.5/src/iricore/data/data16/ursi/ursi18.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.5/src/iricore/data/data16/ursi/ursi19.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.5/src/iricore/data/data16/ursi/ursi20.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.5/src/iricore/data/data16/ursi/ursi21.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.5/src/iricore/data/data16/ursi/ursi22.asc
--rw-r--r--   0        0        0    44300 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/ccir/ccir11.asc
--rw-r--r--   0        0        0    44300 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/ccir/ccir12.asc
--rw-r--r--   0        0        0    44300 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/ccir/ccir13.asc
--rw-r--r--   0        0        0    44300 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/ccir/ccir14.asc
--rw-r--r--   0        0        0    44300 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/ccir/ccir15.asc
--rw-r--r--   0        0        0    44300 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/ccir/ccir16.asc
--rw-r--r--   0        0        0    44300 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/ccir/ccir17.asc
--rw-r--r--   0        0        0    44300 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/ccir/ccir18.asc
--rw-r--r--   0        0        0    44300 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/ccir/ccir19.asc
--rw-r--r--   0        0        0    44300 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/ccir/ccir20.asc
--rw-r--r--   0        0        0    44300 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/ccir/ccir21.asc
--rw-r--r--   0        0        0    44300 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/ccir/ccir22.asc
--rw-r--r--   0        0        0      443 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/igrf/dgrf1945.dat
--rw-r--r--   0        0        0      445 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/igrf/dgrf1950.dat
--rw-r--r--   0        0        0      437 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/igrf/dgrf1955.dat
--rw-r--r--   0        0        0      431 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/igrf/dgrf1960.dat
--rw-r--r--   0        0        0      435 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/igrf/dgrf1965.dat
--rw-r--r--   0        0        0      435 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/igrf/dgrf1970.dat
--rw-r--r--   0        0        0      439 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/igrf/dgrf1975.dat
--rw-r--r--   0        0        0      436 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/igrf/dgrf1980.dat
--rw-r--r--   0        0        0      433 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/igrf/dgrf1985.dat
--rw-r--r--   0        0        0      434 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/igrf/dgrf1990.dat
--rw-r--r--   0        0        0      438 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/igrf/dgrf1995.dat
--rw-r--r--   0        0        0     1015 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/igrf/dgrf2000.dat
--rw-r--r--   0        0        0     1219 2011-12-16 23:39:00.000000 iricore-1.4.5/src/iricore/data/data20/igrf/dgrf2005.dat
--rw-r--r--   0        0        0     1218 2015-02-11 20:37:48.000000 iricore-1.4.5/src/iricore/data/data20/igrf/dgrf2010.dat
--rw-r--r--   0        0        0     1188 2022-09-06 07:12:00.000000 iricore-1.4.5/src/iricore/data/data20/igrf/dgrf2015.dat
--rw-r--r--   0        0        0     1018 2022-10-02 13:54:08.000000 iricore-1.4.5/src/iricore/data/data20/igrf/igrf2020.dat
--rw-r--r--   0        0        0      598 2022-09-06 07:12:00.000000 iricore-1.4.5/src/iricore/data/data20/igrf/igrf2020s.dat
--rw-r--r--   0        0        0  1324624 2022-10-07 03:31:18.000000 iricore-1.4.5/src/iricore/data/data20/index/apf107.dat
--rw-r--r--   0        0        0     9823 2022-10-07 03:33:30.000000 iricore-1.4.5/src/iricore/data/data20/index/ig_rz.dat
--rw-r--r--   0        0        0    88224 2022-09-06 07:12:00.000000 iricore-1.4.5/src/iricore/data/data20/mcsat/mcsat11.dat
--rw-r--r--   0        0        0    88224 2022-09-06 07:12:00.000000 iricore-1.4.5/src/iricore/data/data20/mcsat/mcsat12.dat
--rw-r--r--   0        0        0    88224 2022-09-06 07:12:00.000000 iricore-1.4.5/src/iricore/data/data20/mcsat/mcsat13.dat
--rw-r--r--   0        0        0    88224 2022-09-06 07:12:00.000000 iricore-1.4.5/src/iricore/data/data20/mcsat/mcsat14.dat
--rw-r--r--   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.4.5/src/iricore/data/data20/mcsat/mcsat15.dat
--rw-r--r--   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.4.5/src/iricore/data/data20/mcsat/mcsat16.dat
--rw-r--r--   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.4.5/src/iricore/data/data20/mcsat/mcsat17.dat
--rw-r--r--   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.4.5/src/iricore/data/data20/mcsat/mcsat18.dat
--rw-r--r--   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.4.5/src/iricore/data/data20/mcsat/mcsat19.dat
--rw-r--r--   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.4.5/src/iricore/data/data20/mcsat/mcsat20.dat
--rw-r--r--   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.4.5/src/iricore/data/data20/mcsat/mcsat21.dat
--rw-r--r--   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.4.5/src/iricore/data/data20/mcsat/mcsat22.dat
--rw-r--r--   0        0        0    30628 2004-11-05 00:40:00.000000 iricore-1.4.5/src/iricore/data/data20/ursi/ursi11.asc
--rw-r--r--   0        0        0    30628 2004-11-05 00:40:00.000000 iricore-1.4.5/src/iricore/data/data20/ursi/ursi12.asc
--rw-r--r--   0        0        0    30628 2004-11-05 00:40:00.000000 iricore-1.4.5/src/iricore/data/data20/ursi/ursi13.asc
--rw-r--r--   0        0        0    30628 2004-11-05 00:40:00.000000 iricore-1.4.5/src/iricore/data/data20/ursi/ursi14.asc
--rw-r--r--   0        0        0    30628 2004-11-05 00:40:00.000000 iricore-1.4.5/src/iricore/data/data20/ursi/ursi15.asc
--rw-r--r--   0        0        0    30628 2004-11-05 00:40:00.000000 iricore-1.4.5/src/iricore/data/data20/ursi/ursi16.asc
--rw-r--r--   0        0        0    30628 2004-11-05 00:40:00.000000 iricore-1.4.5/src/iricore/data/data20/ursi/ursi17.asc
--rw-r--r--   0        0        0    30628 2004-11-05 00:40:00.000000 iricore-1.4.5/src/iricore/data/data20/ursi/ursi18.asc
--rw-r--r--   0        0        0    30628 2004-11-05 00:40:00.000000 iricore-1.4.5/src/iricore/data/data20/ursi/ursi19.asc
--rw-r--r--   0        0        0    30628 2004-11-05 00:40:00.000000 iricore-1.4.5/src/iricore/data/data20/ursi/ursi20.asc
--rw-r--r--   0        0        0    30628 2004-11-05 00:40:00.000000 iricore-1.4.5/src/iricore/data/data20/ursi/ursi21.asc
--rw-r--r--   0        0        0    30628 2004-11-05 00:40:00.000000 iricore-1.4.5/src/iricore/data/data20/ursi/ursi22.asc
--rwxr-xr-x   0        0        0      725 2022-11-10 03:07:50.835105 iricore-1.4.5/src/iricore/data_update.py
--rwxr-xr-x   0        0        0     9308 2023-05-10 18:13:43.181093 iricore-1.4.5/src/iricore/iri.py
--rwxr-xr-x   0        0        0   112771 2022-11-10 03:07:50.835105 iricore-1.4.5/src/iricore/iri2016/cira.for
--rwxr-xr-x   0        0        0   161141 2022-11-10 03:07:50.835105 iricore-1.4.5/src/iricore/iri2016/igrf.for
--rwxr-xr-x   0        0        0  1409825 2022-11-10 03:07:50.839105 iricore-1.4.5/src/iricore/iri2016/iridreg.for
--rwxr-xr-x   0        0        0    87973 2022-11-10 03:07:50.839105 iricore-1.4.5/src/iricore/iri2016/iriflip.for
--rwxr-xr-x   0        0        0   485167 2023-06-12 18:38:06.344577 iricore-1.4.5/src/iricore/iri2016/irifun.for
--rwxr-xr-x   0        0        0     6147 2022-12-13 16:30:02.547302 iricore-1.4.5/src/iricore/iri2016/irirtam.for
--rwxr-xr-x   0        0        0    82092 2022-12-13 16:30:02.539301 iricore-1.4.5/src/iricore/iri2016/irisub.for
--rwxr-xr-x   0        0        0     9441 2022-11-10 03:07:50.843105 iricore-1.4.5/src/iricore/iri2016/iritec.for
--rwxr-xr-x   0        0        0      787 2022-10-05 19:17:08.132334 iricore-1.4.5/src/iricore/iri2016/test.f90
--rw-r--r--   0        0        0   112771 2022-09-06 07:12:00.000000 iricore-1.4.5/src/iricore/iri2020/cira.for
--rw-r--r--   0        0        0   161131 2023-06-12 18:46:31.728823 iricore-1.4.5/src/iricore/iri2020/igrf.for
--rw-r--r--   0        0        0  1315925 2022-09-06 07:12:00.000000 iricore-1.4.5/src/iricore/iri2020/iridreg.for
--rw-r--r--   0        0        0    87909 2022-09-06 07:12:00.000000 iricore-1.4.5/src/iricore/iri2020/iriflip.for
--rw-r--r--   0        0        0   580220 2023-06-12 18:49:14.319628 iricore-1.4.5/src/iricore/iri2020/irifun.for
--rw-r--r--   0        0        0     6147 2023-06-12 18:52:43.590118 iricore-1.4.5/src/iricore/iri2020/irirtam.for
--rw-r--r--   0        0        0    88920 2023-06-12 18:52:43.622117 iricore-1.4.5/src/iricore/iri2020/irisub.for
--rw-r--r--   0        0        0   623932 2023-03-19 02:54:42.000000 iricore-1.4.5/src/iricore/iri2020/rocdrift.for
--rw-r--r--   0        0        0      652 2023-05-05 20:54:12.161524 iricore-1.4.5/src/iricore/modules.py
--rwxr-xr-x   0        0        0     1260 2023-03-30 01:44:21.528128 iricore-1.4.5/src/iricore/python_interface.f90
--rw-r--r--   0        0        0     1194 2023-03-30 01:44:21.552128 iricore-1.4.5/src/iricore/python_stec.f90
--rw-r--r--   0        0        0     1020 2023-05-05 22:34:39.878513 iricore-1.4.5/src/iricore/read_iri_data.py
--rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 iricore-1.4.5/setup.py
--rw-r--r--   0        0        0     1814 1970-01-01 00:00:00.000000 iricore-1.4.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1276 2022-05-03 16:22:41.008931 iricore-1.4.6/LICENSE
+-rwxr-xr-x   0        0        0     1254 2023-03-28 01:11:06.672275 iricore-1.4.6/README.md
+-rwxr-xr-x   0        0        0      463 2022-11-10 03:07:50.807105 iricore-1.4.6/build.py
+-rwxr-xr-x   0        0        0      641 2023-06-16 02:20:34.377596 iricore-1.4.6/pyproject.toml
+-rwxr-xr-x   0        0        0      431 2023-06-16 02:04:11.203309 iricore-1.4.6/src/iricore/CMakeLists.txt
+-rwxr-xr-x   0        0        0      112 2023-05-05 20:40:56.755640 iricore-1.4.6/src/iricore/__init__.py
+-rw-r--r--   0        0        0       44 2023-05-05 22:32:51.315676 iricore-1.4.6/src/iricore/config.py
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ccir/ccir11.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ccir/ccir12.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ccir/ccir13.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ccir/ccir14.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ccir/ccir15.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ccir/ccir16.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ccir/ccir17.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ccir/ccir18.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ccir/ccir19.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ccir/ccir20.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ccir/ccir21.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ccir/ccir22.asc
+-rw-r--r--   0        0        0      443 2016-02-04 05:04:35.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf1945.dat
+-rw-r--r--   0        0        0      445 2016-02-04 05:04:44.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf1950.dat
+-rw-r--r--   0        0        0      437 2016-02-04 05:04:50.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf1955.dat
+-rw-r--r--   0        0        0      431 2016-02-04 05:04:58.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf1960.dat
+-rw-r--r--   0        0        0      435 2016-02-04 05:05:13.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf1965.dat
+-rw-r--r--   0        0        0      435 2016-02-04 05:05:18.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf1970.dat
+-rw-r--r--   0        0        0      439 2016-02-04 05:05:25.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf1975.dat
+-rw-r--r--   0        0        0      436 2016-02-04 05:05:31.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf1980.dat
+-rw-r--r--   0        0        0      433 2016-02-04 05:05:40.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf1985.dat
+-rw-r--r--   0        0        0      434 2016-02-04 05:05:58.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf1990.dat
+-rw-r--r--   0        0        0      438 2016-02-04 05:06:08.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf1995.dat
+-rw-r--r--   0        0        0     1015 2016-02-04 05:06:15.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf2000.dat
+-rw-r--r--   0        0        0     1219 2016-02-04 05:06:22.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf2005.dat
+-rw-r--r--   0        0        0     1218 2016-02-04 05:06:32.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf2010.dat
+-rw-r--r--   0        0        0     1188 2020-04-06 19:51:12.000000 iricore-1.4.6/src/iricore/data/data16/igrf/dgrf2015.dat
+-rw-r--r--   0        0        0     1018 2021-09-21 01:36:47.000000 iricore-1.4.6/src/iricore/data/data16/igrf/igrf2020.dat
+-rw-r--r--   0        0        0      598 2021-09-21 01:37:16.000000 iricore-1.4.6/src/iricore/data/data16/igrf/igrf2020s.dat
+-rwxr-xr-x   0        0        0  1312575 2023-05-05 22:25:06.976848 iricore-1.4.6/src/iricore/data/data16/index/apf107.dat
+-rwxr-xr-x   0        0        0     9681 2023-05-05 22:25:07.132847 iricore-1.4.6/src/iricore/data/data16/index/ig_rz.dat
+-rw-r--r--   0        0        0    88224 2016-02-04 04:59:17.000000 iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat11.dat
+-rw-r--r--   0        0        0    88224 2016-02-04 04:59:21.000000 iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat12.dat
+-rw-r--r--   0        0        0    88224 2016-02-04 04:59:26.000000 iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat13.dat
+-rw-r--r--   0        0        0    88224 2016-02-04 04:59:31.000000 iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat14.dat
+-rw-r--r--   0        0        0    88224 2016-02-04 04:59:35.000000 iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat15.dat
+-rw-r--r--   0        0        0    88224 2016-02-04 04:59:47.000000 iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat16.dat
+-rw-r--r--   0        0        0    88224 2016-02-04 04:59:56.000000 iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat17.dat
+-rw-r--r--   0        0        0    88224 2016-02-04 05:00:05.000000 iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat18.dat
+-rw-r--r--   0        0        0    88224 2016-02-04 05:00:12.000000 iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat19.dat
+-rw-r--r--   0        0        0    88224 2016-02-04 05:00:19.000000 iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat20.dat
+-rw-r--r--   0        0        0    88224 2016-02-04 05:00:27.000000 iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat21.dat
+-rw-r--r--   0        0        0    88224 2016-02-04 05:00:33.000000 iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat22.dat
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ursi/ursi11.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ursi/ursi12.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ursi/ursi13.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ursi/ursi14.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ursi/ursi15.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ursi/ursi16.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ursi/ursi17.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ursi/ursi18.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ursi/ursi19.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ursi/ursi20.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ursi/ursi21.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data16/ursi/ursi22.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ccir/ccir11.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ccir/ccir12.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ccir/ccir13.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ccir/ccir14.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ccir/ccir15.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ccir/ccir16.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ccir/ccir17.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ccir/ccir18.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ccir/ccir19.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ccir/ccir20.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ccir/ccir21.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ccir/ccir22.asc
+-rw-r--r--   0        0        0      443 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf1945.dat
+-rw-r--r--   0        0        0      445 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf1950.dat
+-rw-r--r--   0        0        0      437 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf1955.dat
+-rw-r--r--   0        0        0      431 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf1960.dat
+-rw-r--r--   0        0        0      435 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf1965.dat
+-rw-r--r--   0        0        0      435 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf1970.dat
+-rw-r--r--   0        0        0      439 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf1975.dat
+-rw-r--r--   0        0        0      436 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf1980.dat
+-rw-r--r--   0        0        0      433 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf1985.dat
+-rw-r--r--   0        0        0      434 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf1990.dat
+-rw-r--r--   0        0        0      438 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf1995.dat
+-rw-r--r--   0        0        0     1015 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf2000.dat
+-rw-r--r--   0        0        0     1219 2011-12-16 23:39:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf2005.dat
+-rw-r--r--   0        0        0     1218 2015-02-11 20:37:48.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf2010.dat
+-rw-r--r--   0        0        0     1188 2022-09-06 07:12:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/dgrf2015.dat
+-rw-r--r--   0        0        0     1018 2022-10-02 13:54:08.000000 iricore-1.4.6/src/iricore/data/data20/igrf/igrf2020.dat
+-rw-r--r--   0        0        0      598 2022-09-06 07:12:00.000000 iricore-1.4.6/src/iricore/data/data20/igrf/igrf2020s.dat
+-rw-r--r--   0        0        0  1324624 2022-10-07 03:31:18.000000 iricore-1.4.6/src/iricore/data/data20/index/apf107.dat
+-rw-r--r--   0        0        0     9823 2022-10-07 03:33:30.000000 iricore-1.4.6/src/iricore/data/data20/index/ig_rz.dat
+-rw-r--r--   0        0        0    88224 2022-09-06 07:12:00.000000 iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat11.dat
+-rw-r--r--   0        0        0    88224 2022-09-06 07:12:00.000000 iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat12.dat
+-rw-r--r--   0        0        0    88224 2022-09-06 07:12:00.000000 iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat13.dat
+-rw-r--r--   0        0        0    88224 2022-09-06 07:12:00.000000 iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat14.dat
+-rw-r--r--   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat15.dat
+-rw-r--r--   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat16.dat
+-rw-r--r--   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat17.dat
+-rw-r--r--   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat18.dat
+-rw-r--r--   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat19.dat
+-rw-r--r--   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat20.dat
+-rw-r--r--   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat21.dat
+-rw-r--r--   0        0        0    88224 2022-09-06 07:12:02.000000 iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat22.dat
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ursi/ursi11.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ursi/ursi12.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ursi/ursi13.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ursi/ursi14.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ursi/ursi15.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ursi/ursi16.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ursi/ursi17.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ursi/ursi18.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ursi/ursi19.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ursi/ursi20.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ursi/ursi21.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.6/src/iricore/data/data20/ursi/ursi22.asc
+-rwxr-xr-x   0        0        0      725 2022-11-10 03:07:50.835105 iricore-1.4.6/src/iricore/data_update.py
+-rwxr-xr-x   0        0        0     9332 2023-06-16 02:19:12.764327 iricore-1.4.6/src/iricore/iri.py
+-rwxr-xr-x   0        0        0   112771 2022-11-10 03:07:50.835105 iricore-1.4.6/src/iricore/iri2016/cira.for
+-rwxr-xr-x   0        0        0   161141 2022-11-10 03:07:50.835105 iricore-1.4.6/src/iricore/iri2016/igrf.for
+-rwxr-xr-x   0        0        0  1409825 2022-11-10 03:07:50.839105 iricore-1.4.6/src/iricore/iri2016/iridreg.for
+-rwxr-xr-x   0        0        0    87973 2022-11-10 03:07:50.839105 iricore-1.4.6/src/iricore/iri2016/iriflip.for
+-rwxr-xr-x   0        0        0   485167 2023-06-12 18:38:06.344577 iricore-1.4.6/src/iricore/iri2016/irifun.for
+-rwxr-xr-x   0        0        0     6147 2022-12-13 16:30:02.547302 iricore-1.4.6/src/iricore/iri2016/irirtam.for
+-rwxr-xr-x   0        0        0    82092 2022-12-13 16:30:02.539301 iricore-1.4.6/src/iricore/iri2016/irisub.for
+-rwxr-xr-x   0        0        0     9441 2022-11-10 03:07:50.843105 iricore-1.4.6/src/iricore/iri2016/iritec.for
+-rw-r--r--   0        0        0   112771 2022-09-06 07:12:00.000000 iricore-1.4.6/src/iricore/iri2020/cira.for
+-rw-r--r--   0        0        0   161131 2023-06-12 18:46:31.728823 iricore-1.4.6/src/iricore/iri2020/igrf.for
+-rw-r--r--   0        0        0  1315925 2022-09-06 07:12:00.000000 iricore-1.4.6/src/iricore/iri2020/iridreg.for
+-rw-r--r--   0        0        0    87909 2022-09-06 07:12:00.000000 iricore-1.4.6/src/iricore/iri2020/iriflip.for
+-rw-r--r--   0        0        0   580220 2023-06-12 18:49:14.319628 iricore-1.4.6/src/iricore/iri2020/irifun.for
+-rw-r--r--   0        0        0     6147 2023-06-12 18:52:43.590118 iricore-1.4.6/src/iricore/iri2020/irirtam.for
+-rw-r--r--   0        0        0    88920 2023-06-12 18:52:43.622117 iricore-1.4.6/src/iricore/iri2020/irisub.for
+-rw-r--r--   0        0        0   623932 2023-03-19 02:54:42.000000 iricore-1.4.6/src/iricore/iri2020/rocdrift.for
+-rw-r--r--   0        0        0      652 2023-05-05 20:54:12.161524 iricore-1.4.6/src/iricore/modules.py
+-rwxr-xr-x   0        0        0     1317 2023-06-16 02:18:13.523470 iricore-1.4.6/src/iricore/python_interface.f90
+-rw-r--r--   0        0        0     1194 2023-03-30 01:44:21.552128 iricore-1.4.6/src/iricore/python_stec.f90
+-rw-r--r--   0        0        0     1020 2023-05-05 22:34:39.878513 iricore-1.4.6/src/iricore/read_iri_data.py
+-rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 iricore-1.4.6/setup.py
+-rw-r--r--   0        0        0     1814 1970-01-01 00:00:00.000000 iricore-1.4.6/PKG-INFO
```

### Comparing `iricore-1.4.5/LICENSE` & `iricore-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/README.md` & `iricore-1.4.6/README.md`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/pyproject.toml` & `iricore-1.4.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iricore"
-version = "1.4.5"
+version = "1.4.6"
 description = ""
 authors = ["Vadym Bidula <vadym.bidula@gmail.com>"]
 readme = "README.md"
 build = "build.py"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <4.0"
```

### Comparing `iricore-1.4.5/src/iricore/data/data16/ccir/ccir11.asc` & `iricore-1.4.6/src/iricore/data/data16/ccir/ccir11.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/ccir/ccir12.asc` & `iricore-1.4.6/src/iricore/data/data16/ccir/ccir12.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/ccir/ccir13.asc` & `iricore-1.4.6/src/iricore/data/data16/ccir/ccir13.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/ccir/ccir14.asc` & `iricore-1.4.6/src/iricore/data/data16/ccir/ccir14.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/ccir/ccir15.asc` & `iricore-1.4.6/src/iricore/data/data16/ccir/ccir15.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/ccir/ccir16.asc` & `iricore-1.4.6/src/iricore/data/data16/ccir/ccir16.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/ccir/ccir17.asc` & `iricore-1.4.6/src/iricore/data/data16/ccir/ccir17.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/ccir/ccir18.asc` & `iricore-1.4.6/src/iricore/data/data16/ccir/ccir18.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/ccir/ccir19.asc` & `iricore-1.4.6/src/iricore/data/data16/ccir/ccir19.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/ccir/ccir20.asc` & `iricore-1.4.6/src/iricore/data/data16/ccir/ccir20.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/ccir/ccir21.asc` & `iricore-1.4.6/src/iricore/data/data16/ccir/ccir21.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/ccir/ccir22.asc` & `iricore-1.4.6/src/iricore/data/data16/ccir/ccir22.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/igrf/dgrf2000.dat` & `iricore-1.4.6/src/iricore/data/data16/igrf/dgrf2000.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/igrf/dgrf2005.dat` & `iricore-1.4.6/src/iricore/data/data16/igrf/dgrf2005.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/igrf/dgrf2010.dat` & `iricore-1.4.6/src/iricore/data/data16/igrf/dgrf2010.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/igrf/dgrf2015.dat` & `iricore-1.4.6/src/iricore/data/data16/igrf/dgrf2015.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/igrf/igrf2020.dat` & `iricore-1.4.6/src/iricore/data/data16/igrf/igrf2020.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/igrf/igrf2020s.dat` & `iricore-1.4.6/src/iricore/data/data16/igrf/igrf2020s.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/index/apf107.dat` & `iricore-1.4.6/src/iricore/data/data16/index/apf107.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/index/ig_rz.dat` & `iricore-1.4.6/src/iricore/data/data16/index/ig_rz.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/mcsat/mcsat11.dat` & `iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat11.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/mcsat/mcsat12.dat` & `iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat12.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/mcsat/mcsat13.dat` & `iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat13.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/mcsat/mcsat14.dat` & `iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat14.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/mcsat/mcsat15.dat` & `iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat15.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/mcsat/mcsat16.dat` & `iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat16.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/mcsat/mcsat17.dat` & `iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat17.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/mcsat/mcsat18.dat` & `iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat18.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/mcsat/mcsat19.dat` & `iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat19.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/mcsat/mcsat20.dat` & `iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat20.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/mcsat/mcsat21.dat` & `iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat21.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/mcsat/mcsat22.dat` & `iricore-1.4.6/src/iricore/data/data16/mcsat/mcsat22.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/ursi/ursi11.asc` & `iricore-1.4.6/src/iricore/data/data16/ursi/ursi11.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/ursi/ursi12.asc` & `iricore-1.4.6/src/iricore/data/data16/ursi/ursi12.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/ursi/ursi13.asc` & `iricore-1.4.6/src/iricore/data/data16/ursi/ursi13.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/ursi/ursi14.asc` & `iricore-1.4.6/src/iricore/data/data16/ursi/ursi14.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/ursi/ursi15.asc` & `iricore-1.4.6/src/iricore/data/data16/ursi/ursi15.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/ursi/ursi16.asc` & `iricore-1.4.6/src/iricore/data/data16/ursi/ursi16.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/ursi/ursi17.asc` & `iricore-1.4.6/src/iricore/data/data16/ursi/ursi17.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/ursi/ursi18.asc` & `iricore-1.4.6/src/iricore/data/data16/ursi/ursi18.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/ursi/ursi19.asc` & `iricore-1.4.6/src/iricore/data/data16/ursi/ursi19.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/ursi/ursi20.asc` & `iricore-1.4.6/src/iricore/data/data16/ursi/ursi20.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/ursi/ursi21.asc` & `iricore-1.4.6/src/iricore/data/data16/ursi/ursi21.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data16/ursi/ursi22.asc` & `iricore-1.4.6/src/iricore/data/data16/ursi/ursi22.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/ccir/ccir11.asc` & `iricore-1.4.6/src/iricore/data/data20/ccir/ccir11.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/ccir/ccir12.asc` & `iricore-1.4.6/src/iricore/data/data20/ccir/ccir12.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/ccir/ccir13.asc` & `iricore-1.4.6/src/iricore/data/data20/ccir/ccir13.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/ccir/ccir14.asc` & `iricore-1.4.6/src/iricore/data/data20/ccir/ccir14.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/ccir/ccir15.asc` & `iricore-1.4.6/src/iricore/data/data20/ccir/ccir15.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/ccir/ccir16.asc` & `iricore-1.4.6/src/iricore/data/data20/ccir/ccir16.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/ccir/ccir17.asc` & `iricore-1.4.6/src/iricore/data/data20/ccir/ccir17.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/ccir/ccir18.asc` & `iricore-1.4.6/src/iricore/data/data20/ccir/ccir18.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/ccir/ccir19.asc` & `iricore-1.4.6/src/iricore/data/data20/ccir/ccir19.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/ccir/ccir20.asc` & `iricore-1.4.6/src/iricore/data/data20/ccir/ccir20.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/ccir/ccir21.asc` & `iricore-1.4.6/src/iricore/data/data20/ccir/ccir21.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/ccir/ccir22.asc` & `iricore-1.4.6/src/iricore/data/data20/ccir/ccir22.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/igrf/dgrf2000.dat` & `iricore-1.4.6/src/iricore/data/data20/igrf/dgrf2000.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/igrf/dgrf2005.dat` & `iricore-1.4.6/src/iricore/data/data20/igrf/dgrf2005.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/igrf/dgrf2010.dat` & `iricore-1.4.6/src/iricore/data/data20/igrf/dgrf2010.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/igrf/dgrf2015.dat` & `iricore-1.4.6/src/iricore/data/data20/igrf/dgrf2015.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/igrf/igrf2020.dat` & `iricore-1.4.6/src/iricore/data/data20/igrf/igrf2020.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/igrf/igrf2020s.dat` & `iricore-1.4.6/src/iricore/data/data20/igrf/igrf2020s.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/index/apf107.dat` & `iricore-1.4.6/src/iricore/data/data20/index/apf107.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/index/ig_rz.dat` & `iricore-1.4.6/src/iricore/data/data20/index/ig_rz.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/mcsat/mcsat11.dat` & `iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat11.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/mcsat/mcsat12.dat` & `iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat12.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/mcsat/mcsat13.dat` & `iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat13.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/mcsat/mcsat14.dat` & `iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat14.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/mcsat/mcsat15.dat` & `iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat15.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/mcsat/mcsat16.dat` & `iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat16.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/mcsat/mcsat17.dat` & `iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat17.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/mcsat/mcsat18.dat` & `iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat18.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/mcsat/mcsat19.dat` & `iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat19.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/mcsat/mcsat20.dat` & `iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat20.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/mcsat/mcsat21.dat` & `iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat21.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/mcsat/mcsat22.dat` & `iricore-1.4.6/src/iricore/data/data20/mcsat/mcsat22.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/ursi/ursi11.asc` & `iricore-1.4.6/src/iricore/data/data20/ursi/ursi11.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/ursi/ursi12.asc` & `iricore-1.4.6/src/iricore/data/data20/ursi/ursi12.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/ursi/ursi13.asc` & `iricore-1.4.6/src/iricore/data/data20/ursi/ursi13.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/ursi/ursi14.asc` & `iricore-1.4.6/src/iricore/data/data20/ursi/ursi14.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/ursi/ursi15.asc` & `iricore-1.4.6/src/iricore/data/data20/ursi/ursi15.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/ursi/ursi16.asc` & `iricore-1.4.6/src/iricore/data/data20/ursi/ursi16.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/ursi/ursi17.asc` & `iricore-1.4.6/src/iricore/data/data20/ursi/ursi17.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/ursi/ursi18.asc` & `iricore-1.4.6/src/iricore/data/data20/ursi/ursi18.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/ursi/ursi19.asc` & `iricore-1.4.6/src/iricore/data/data20/ursi/ursi19.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/ursi/ursi20.asc` & `iricore-1.4.6/src/iricore/data/data20/ursi/ursi20.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/ursi/ursi21.asc` & `iricore-1.4.6/src/iricore/data/data20/ursi/ursi21.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data/data20/ursi/ursi22.asc` & `iricore-1.4.6/src/iricore/data/data20/ursi/ursi22.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/data_update.py` & `iricore-1.4.6/src/iricore/data_update.py`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/iri.py` & `iricore-1.4.6/src/iricore/iri.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from .config import IRI_VERSIONS, DEFAULT_VERSION
 from .modules import srange, R_EARTH
 from .read_iri_data import readapf107
 
 _iri_cfd = os.path.dirname(os.path.abspath(__file__))
 
+# TODO: Fix data reading from Python
 IRI_DATA = readapf107(20)
 
 
 def _import_libs():
     iri2016 = np.ctypeslib.load_library("libiri2016", _iri_cfd)
     iri2020 = np.ctypeslib.load_library("libiri2020", _iri_cfd)
     return iri2016, iri2020
@@ -134,15 +135,15 @@
 
 
 def IRI(dt: datetime, alt_range: [float, float, float], lats: Sequence[float], lons: Sequence[float],
         replace_missing: float = np.nan, version: Literal[16, 20] = DEFAULT_VERSION, calc_ions: bool = False,
         jf: Sequence[bool] = None) -> dict:
     if jf is None:
         jf = np.ones(50, dtype=np.int32, order="F")
-        jf[[2, 3, 4, 5, 11, 20, 21, 22, 23, 25, 27, 28, 29, 33, 34, 35, 36, 46]] = 0
+        jf[[2, 3, 4, 5, 11, 20, 21, 22, 25, 27, 28, 29, 33, 34, 35, 36, 46]] = 0
         if calc_ions:
             jf[[1, 2]] = 1
     else:
         jf = np.asarray(jf, dtype=np.int32, order="F")
         if jf.size != 50:
             raise ValueError("Length of jf array must be 50")
     iri_res = _call_iri_sub(dt, alt_range, lats, lons, jf, version)
@@ -151,22 +152,21 @@
     te = _extract_data(iri_res, 3, len(lats), alt_range, replace_missing)
     o = _extract_data(iri_res, 4, len(lats), alt_range, replace_missing)
     h = _extract_data(iri_res, 5, len(lats), alt_range, replace_missing)
     he = _extract_data(iri_res, 6, len(lats), alt_range, replace_missing)
     o2 = _extract_data(iri_res, 7, len(lats), alt_range, replace_missing)
     no = _extract_data(iri_res, 8, len(lats), alt_range, replace_missing)
     n = _extract_data(iri_res, 10, len(lats), alt_range, replace_missing)
-
     return dict(ne=ne, te=te, o=o, h=h, he=he, o2=o2, no=no, n=n)
 
 
 def IRI_etemp_only(dt: datetime, alt_range: [float, float, float], lats: Sequence[float], lons: Sequence[float],
                    replace_missing: float = np.nan, version: Literal[16, 20] = DEFAULT_VERSION) -> dict:
     jf = np.ones(50, dtype=np.int32, order="F")
-    jf[[0, 2, 3, 4, 5, 11, 20, 21, 22, 23, 25, 27, 28, 29, 33, 34, 35, 36, 46]] = 0
+    jf[[0, 2, 3, 4, 5, 11, 20, 21, 22, 25, 27, 28, 29, 33, 34, 35, 36, 46]] = 0
     iri_res = _call_iri_sub(dt, alt_range, lats, lons, jf, version)
     te = _extract_data(iri_res, 3, len(lats), alt_range, replace_missing)
     return {'te': te}
 
 
 def stec(alt: float, az: float, dt: datetime, position: Sequence[float, float, float], hbot: float = 90,
          htop: float = 2000, npoints: int = 500,
@@ -189,15 +189,15 @@
     heights = np.linspace(hbot, htop, npoints)
     rslant = srange(np.deg2rad(90 - alt), heights * 1e3)
     ell = pm.Ellipsoid(R_EARTH, R_EARTH)
     slat, slon, _ = pm.aer2geodetic(az, alt, rslant, *position, ell=ell)
 
     # IRI call and data extraction
     jf = np.ones(50, dtype=np.int32, order="F")
-    jf[[1, 2, 3, 4, 5, 11, 20, 21, 22, 23, 25, 27, 28, 29, 33, 34, 35, 36, 46]] = 0
+    jf[[1, 2, 3, 4, 5, 11, 20, 21, 22, 25, 27, 28, 29, 33, 34, 35, 36, 46]] = 0
     iri_res = _call_stec(dt, heights, slat, slon, jf, version)
     ne = iri_res[0].transpose()
     ne = ne.reshape((len(heights), -1))[:, 0]
 
     # Data postprocessing (fixing non-physical IRI output)
     ne_debug = ne.copy()
     if np.any(np.isnan(ne)) or np.any(np.isinf(ne)):
```

### Comparing `iricore-1.4.5/src/iricore/iri2016/cira.for` & `iricore-1.4.6/src/iricore/iri2016/cira.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/iri2016/igrf.for` & `iricore-1.4.6/src/iricore/iri2016/igrf.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/iri2016/iridreg.for` & `iricore-1.4.6/src/iricore/iri2016/iridreg.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/iri2016/iriflip.for` & `iricore-1.4.6/src/iricore/iri2016/iriflip.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/iri2016/irifun.for` & `iricore-1.4.6/src/iricore/iri2016/irifun.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/iri2016/irirtam.for` & `iricore-1.4.6/src/iricore/iri2016/irirtam.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/iri2016/irisub.for` & `iricore-1.4.6/src/iricore/iri2016/irisub.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/iri2016/iritec.for` & `iricore-1.4.6/src/iricore/iri2016/iritec.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/iri2020/cira.for` & `iricore-1.4.6/src/iricore/iri2020/cira.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/iri2020/igrf.for` & `iricore-1.4.6/src/iricore/iri2020/igrf.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/iri2020/iridreg.for` & `iricore-1.4.6/src/iricore/iri2020/iridreg.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/iri2020/iriflip.for` & `iricore-1.4.6/src/iricore/iri2020/iriflip.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/iri2020/irifun.for` & `iricore-1.4.6/src/iricore/iri2020/irifun.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/iri2020/irirtam.for` & `iricore-1.4.6/src/iricore/iri2020/irirtam.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/iri2020/irisub.for` & `iricore-1.4.6/src/iricore/iri2020/irisub.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/iri2020/rocdrift.for` & `iricore-1.4.6/src/iricore/iri2020/rocdrift.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/modules.py` & `iricore-1.4.6/src/iricore/modules.py`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/python_interface.f90` & `iricore-1.4.6/src/iricore/python_interface.f90`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,16 @@
   integer :: NITER
 
   aap = aap_
   af107 = af107_
   n = n_
   datadir1 = datadir
   call read_ig_rz
-!  call readapf107
+  ! TODO: Remove next line later (after applying the fix)
+  call readapf107
   NITER = SIZE(glat)
 
 
   do i = 1, NITER
       call IRI_SUB(jf, jmag, glat(i), glon(i), iyyyy, mmdd, dhour, heibeg, heiend, heistp, outf, oarr, datadir)
       do j = 1, 20
         do k = 1, 1000
```

### Comparing `iricore-1.4.5/src/iricore/python_stec.f90` & `iricore-1.4.6/src/iricore/python_stec.f90`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/src/iricore/read_iri_data.py` & `iricore-1.4.6/src/iricore/read_iri_data.py`

 * *Files identical despite different names*

### Comparing `iricore-1.4.5/setup.py` & `iricore-1.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
              'iri2020/*']}
 
 install_requires = \
 ['fortranformat>=1.2.2,<2.0.0', 'numpy>=1.22,<2.0', 'pymap3d>=3.0.1,<4.0.0']
 
 setup_kwargs = {
     'name': 'iricore',
-    'version': '1.4.5',
+    'version': '1.4.6',
     'description': '',
     'long_description': '# iricore\nA Python interface to IRI-2016 and IRI-2020 using `ctypes` communication.\n\n**Important!** Because this package is mainly used for the [MIST experiment](http://www.physics.mcgill.ca/mist/), \nthe `iricore` cuts off calculation of unnecessary atmospheric parameters available in IRI-2016, leaving only electron density\nand electron temperature. All other parameters can be restored on demand (please contact me).\n\n## Installation\n\nThis package proved to work under Linux only (due to compilation difficulties in Windows). \nIf you are using Windows - consider installing [WSL](https://docs.microsoft.com/en-us/windows/wsl/install).\n\n### Prerequisites\n- CMAKE\n```\nsudo apt instal cmake\n```\n\n- Fortran compiler, e.g. `gfortran`\n```\nsudo apt isntall gfortran\n```\n\n### Installing package\nNow you can simply install it via `pip`:\n\n```\npython3 -m pip install iricore\n```\n\n## Data files\n`IRI2016` model depends on [data files](http://irimodel.org/indices/) which are regularly updated.\n`iricore` does not autoupdate those, but provides tool for quick update. You can run from terminal\n```\npython3 -c "import iricore; iricore.update()"\n```\n\nor add\n\n```\nimport iricore\niricore.update()\n```\nto any Python script.\n\n## Usage\nFor usage examples see `examples/`.',
     'author': 'Vadym Bidula',
     'author_email': 'vadym.bidula@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `iricore-1.4.5/PKG-INFO` & `iricore-1.4.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iricore
-Version: 1.4.5
+Version: 1.4.6
 Summary: 
 Author: Vadym Bidula
 Author-email: vadym.bidula@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

