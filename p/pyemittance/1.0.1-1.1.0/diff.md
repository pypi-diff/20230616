# Comparing `tmp/pyemittance-1.0.1.tar.gz` & `tmp/pyemittance-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/PyEmittance/PyEmittance/dist/.tmp-g_s2po_i/pyemittance-1.0.1.tar", last modified: Fri Jan  6 19:02:08 2023, max compression
+gzip compressed data, was "/home/runner/work/PyEmittance/PyEmittance/dist/.tmp-wjghqk1s/pyemittance-1.1.0.tar", last modified: Fri Jun 16 16:04:02 2023, max compression
```

## Comparing `pyemittance-1.0.1.tar` & `pyemittance-1.1.0.tar`

### file list

```diff
@@ -1,98 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 19:02:08.000000 pyemittance-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-01-06 19:01:50.000000 pyemittance-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-06 19:01:50.000000 pyemittance-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-01-06 19:02:08.000000 pyemittance-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-01-06 19:01:50.000000 pyemittance-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 19:02:08.000000 pyemittance-1.0.1/pyemittance/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-06 19:02:08.000000 pyemittance-1.0.1/pyemittance/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/bs_fitting_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 19:02:08.000000 pyemittance-1.0.1/pyemittance/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 19:02:08.000000 pyemittance-1.0.1/pyemittance/configs/FACET_nominal/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/FACET_nominal/beamline_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/FACET_nominal/img_proc.json
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/FACET_nominal/meas_pv_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/FACET_nominal/opt_pv_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/FACET_nominal/save_scalar_pvs.json
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/FACET_nominal/savepaths.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 19:02:08.000000 pyemittance-1.0.1/pyemittance/configs/LCLS2_OTR0H04/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS2_OTR0H04/beamline_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS2_OTR0H04/img_proc.json
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS2_OTR0H04/meas_pv_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS2_OTR0H04/opt_pv_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS2_OTR0H04/save_scalar_pvs.json
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS2_OTR0H04/savepaths.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 19:02:08.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_OTR1/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_OTR1/beamline_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_OTR1/img_proc.json
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_OTR1/meas_pv_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_OTR1/opt_pv_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_OTR1/save_scalar_pvs.json
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_OTR1/savepaths.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 19:02:08.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_OTR2/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_OTR2/beamline_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_OTR2/img_proc.json
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_OTR2/meas_pv_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_OTR2/opt_pv_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_OTR2/save_scalar_pvs.json
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_OTR2/savepaths.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 19:02:08.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_OTR3/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_OTR3/beamline_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_OTR3/img_proc.json
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_OTR3/meas_pv_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_OTR3/opt_pv_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_OTR3/save_scalar_pvs.json
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_OTR3/savepaths.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 19:02:08.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_WS02/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_WS02/beamline_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_WS02/img_proc.json
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_WS02/meas_pv_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_WS02/opt_pv_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_WS02/save_scalar_pvs.json
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_WS02/savepaths.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 19:02:08.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_nominal/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_nominal/beamline_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_nominal/img_proc.json
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_nominal/meas_pv_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_nominal/opt_pv_info.json
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_nominal/pv_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/LCLS_nominal/savepaths.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 19:02:08.000000 pyemittance-1.0.1/pyemittance/configs/latest_facet/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/latest_facet/beamline_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/latest_facet/img_proc.json
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/latest_facet/meas_pv_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/latest_facet/opt_pv_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/latest_facet/save_scalar_pvs.json
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/latest_facet/savepaths.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 19:02:08.000000 pyemittance-1.0.1/pyemittance/configs/sim/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/sim/beamline_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/sim/img_proc.json
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/sim/meas_pv_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/sim/opt_pv_info.json
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/sim/save_scalar_pvs.json
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/configs/sim/savepaths.json
--rw-r--r--   0 runner    (1001) docker     (123)    12426 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/data_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/emittance_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/load_json_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/machine_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/machine_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/optics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/otrs_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/pyemittance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/saving_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/simulation_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-01-06 19:01:50.000000 pyemittance-1.0.1/pyemittance/wire_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 19:02:08.000000 pyemittance-1.0.1/pyemittance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-01-06 19:02:08.000000 pyemittance-1.0.1/pyemittance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-01-06 19:02:08.000000 pyemittance-1.0.1/pyemittance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 19:02:08.000000 pyemittance-1.0.1/pyemittance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-01-06 19:02:08.000000 pyemittance-1.0.1/pyemittance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-06 19:02:08.000000 pyemittance-1.0.1/pyemittance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-06 19:01:50.000000 pyemittance-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-01-06 19:02:08.000000 pyemittance-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-01-06 19:01:50.000000 pyemittance-1.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83426 2023-01-06 19:01:50.000000 pyemittance-1.0.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:04:02.000000 pyemittance-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-16 16:03:52.000000 pyemittance-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-16 16:03:52.000000 pyemittance-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-16 16:04:02.000000 pyemittance-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-16 16:03:52.000000 pyemittance-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:04:02.000000 pyemittance-1.1.0/pyemittance/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-16 16:04:02.000000 pyemittance-1.1.0/pyemittance/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/bs_fitting_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:04:02.000000 pyemittance-1.1.0/pyemittance/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:04:02.000000 pyemittance-1.1.0/pyemittance/configs/FACET_nominal/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/FACET_nominal/beamline_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/FACET_nominal/img_proc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/FACET_nominal/meas_pv_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/FACET_nominal/opt_pv_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/FACET_nominal/save_scalar_pvs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/FACET_nominal/savepaths.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:04:02.000000 pyemittance-1.1.0/pyemittance/configs/LCLS2_OTR0H04/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS2_OTR0H04/beamline_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS2_OTR0H04/img_proc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS2_OTR0H04/meas_pv_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS2_OTR0H04/savepaths.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:04:02.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_OTR1/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_OTR1/beamline_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_OTR1/img_proc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_OTR1/meas_pv_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_OTR1/opt_pv_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_OTR1/save_scalar_pvs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_OTR1/savepaths.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:04:02.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_OTR2/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_OTR2/beamline_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_OTR2/img_proc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_OTR2/meas_pv_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_OTR2/opt_pv_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_OTR2/save_scalar_pvs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_OTR2/savepaths.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:04:02.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_OTR3/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_OTR3/beamline_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_OTR3/img_proc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_OTR3/meas_pv_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_OTR3/opt_pv_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_OTR3/save_scalar_pvs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_OTR3/savepaths.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:04:02.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_WS02/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_WS02/beamline_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_WS02/img_proc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_WS02/meas_pv_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_WS02/opt_pv_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_WS02/save_scalar_pvs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_WS02/savepaths.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:04:02.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_nominal/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_nominal/beamline_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_nominal/img_proc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_nominal/meas_pv_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_nominal/opt_pv_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_nominal/pv_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/LCLS_nominal/savepaths.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:04:02.000000 pyemittance-1.1.0/pyemittance/configs/latest_facet/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/latest_facet/beamline_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/latest_facet/img_proc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/latest_facet/meas_pv_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/latest_facet/opt_pv_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/latest_facet/save_scalar_pvs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/latest_facet/savepaths.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:04:02.000000 pyemittance-1.1.0/pyemittance/configs/sim/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/sim/beamline_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/sim/img_proc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/sim/meas_pv_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/sim/opt_pv_info.json
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/sim/save_scalar_pvs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/configs/sim/savepaths.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/emittance_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/load_json_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/machine_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/machine_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/optics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/otrs_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/pyemittance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/saving_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/simulation_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-16 16:03:52.000000 pyemittance-1.1.0/pyemittance/wire_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:04:02.000000 pyemittance-1.1.0/pyemittance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-06-16 16:04:02.000000 pyemittance-1.1.0/pyemittance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-16 16:04:02.000000 pyemittance-1.1.0/pyemittance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 16:04:02.000000 pyemittance-1.1.0/pyemittance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-16 16:04:02.000000 pyemittance-1.1.0/pyemittance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-16 16:04:02.000000 pyemittance-1.1.0/pyemittance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-16 16:03:52.000000 pyemittance-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-16 16:04:02.000000 pyemittance-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-16 16:03:52.000000 pyemittance-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 16:04:02.000000 pyemittance-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-16 16:03:52.000000 pyemittance-1.1.0/tests/test_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-16 16:03:52.000000 pyemittance-1.1.0/tests/test_online.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83426 2023-06-16 16:03:52.000000 pyemittance-1.1.0/versioneer.py
```

### Comparing `pyemittance-1.0.1/LICENSE` & `pyemittance-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyemittance-1.0.1/PKG-INFO` & `pyemittance-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyemittance
-Version: 1.0.1
+Version: 1.1.0
 Home-page: https://github.com/slaclab/PyEmittance
 Author: Sara Miskovich
 Author-email: smiskov@slac.stanford.edu
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyemittance-1.0.1/README.md` & `pyemittance-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pyemittance-1.0.1/pyemittance/bs_fitting_methods.py` & `pyemittance-1.1.0/pyemittance/bs_fitting_methods.py`

 * *Files identical despite different names*

### Comparing `pyemittance-1.0.1/pyemittance/configs/FACET_nominal/meas_pv_info.json` & `pyemittance-1.1.0/pyemittance/configs/FACET_nominal/meas_pv_info.json`

 * *Files identical despite different names*

### Comparing `pyemittance-1.0.1/pyemittance/configs/FACET_nominal/save_scalar_pvs.json` & `pyemittance-1.1.0/pyemittance/configs/FACET_nominal/save_scalar_pvs.json`

 * *Files identical despite different names*

### Comparing `pyemittance-1.0.1/pyemittance/configs/LCLS2_OTR0H04/save_scalar_pvs.json` & `pyemittance-1.1.0/pyemittance/configs/LCLS_OTR3/save_scalar_pvs.json`

 * *Files identical despite different names*

### Comparing `pyemittance-1.0.1/pyemittance/configs/LCLS2_OTR0H04/savepaths.json` & `pyemittance-1.1.0/pyemittance/configs/LCLS2_OTR0H04/savepaths.json`

 * *Files identical despite different names*

### Comparing `pyemittance-1.0.1/pyemittance/configs/LCLS_OTR1/meas_pv_info.json` & `pyemittance-1.1.0/pyemittance/configs/LCLS_OTR1/meas_pv_info.json`

 * *Files identical despite different names*

### Comparing `pyemittance-1.0.1/pyemittance/configs/LCLS_OTR1/save_scalar_pvs.json` & `pyemittance-1.1.0/pyemittance/configs/LCLS_OTR1/save_scalar_pvs.json`

 * *Files identical despite different names*

### Comparing `pyemittance-1.0.1/pyemittance/configs/LCLS_OTR2/meas_pv_info.json` & `pyemittance-1.1.0/pyemittance/configs/LCLS_OTR2/meas_pv_info.json`

 * *Files identical despite different names*

### Comparing `pyemittance-1.0.1/pyemittance/configs/LCLS_OTR2/save_scalar_pvs.json` & `pyemittance-1.1.0/pyemittance/configs/LCLS_OTR2/save_scalar_pvs.json`

 * *Files identical despite different names*

### Comparing `pyemittance-1.0.1/pyemittance/configs/LCLS_OTR3/meas_pv_info.json` & `pyemittance-1.1.0/pyemittance/configs/LCLS_OTR3/meas_pv_info.json`

 * *Files identical despite different names*

### Comparing `pyemittance-1.0.1/pyemittance/configs/LCLS_OTR3/save_scalar_pvs.json` & `pyemittance-1.1.0/pyemittance/configs/sim/save_scalar_pvs.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8214285714285714%*

 * *Differences: {"'scalars'": "{insert: [(18, 'OTRS:IN20:541:XRMS'), (19, 'OTRS:IN20:541:YRMS'), (20, "*

 * *              "'OTRS:IN20:541:X'), (21, 'OTRS:IN20:541:Y'), (22, 'OTRS:IN20:541:RESOLUTION')], "*

 * *              'delete: [22, 21, 20, 19, 18]}'}*

```diff
@@ -14,14 +14,14 @@
         "QUAD:IN20:122:BCTRL",
         "QUAD:IN20:361:BCTRL",
         "QUAD:IN20:371:BCTRL",
         "QUAD:IN20:425:BCTRL",
         "QUAD:IN20:441:BCTRL",
         "QUAD:IN20:511:BCTRL",
         "QUAD:IN20:525:BCTRL",
-        "OTRS:IN20:621:XRMS",
-        "OTRS:IN20:621:YRMS",
-        "OTRS:IN20:621:X",
-        "OTRS:IN20:621:Y",
-        "OTRS:IN20:621:RESOLUTION"
+        "OTRS:IN20:541:XRMS",
+        "OTRS:IN20:541:YRMS",
+        "OTRS:IN20:541:X",
+        "OTRS:IN20:541:Y",
+        "OTRS:IN20:541:RESOLUTION"
     ]
 }
```

### Comparing `pyemittance-1.0.1/pyemittance/configs/LCLS_WS02/meas_pv_info.json` & `pyemittance-1.1.0/pyemittance/configs/LCLS_WS02/meas_pv_info.json`

 * *Files identical despite different names*

### Comparing `pyemittance-1.0.1/pyemittance/configs/LCLS_nominal/pv_info.json` & `pyemittance-1.1.0/pyemittance/configs/LCLS_nominal/pv_info.json`

 * *Files identical despite different names*

### Comparing `pyemittance-1.0.1/pyemittance/configs/latest_facet/meas_pv_info.json` & `pyemittance-1.1.0/pyemittance/configs/latest_facet/meas_pv_info.json`

 * *Files identical despite different names*

### Comparing `pyemittance-1.0.1/pyemittance/configs/latest_facet/save_scalar_pvs.json` & `pyemittance-1.1.0/pyemittance/configs/latest_facet/save_scalar_pvs.json`

 * *Files identical despite different names*

### Comparing `pyemittance-1.0.1/pyemittance/data_handler.py` & `pyemittance-1.1.0/pyemittance/data_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 def adapt_range(
     x, 
     y,
     axis,
     w=None,
     cutoff_percent=0.3,
     num_points=5,
+    bounds = None
 ):
     """
     Returns new scan quad values AS LIST
     
     Parameters
     ----------
     x : list
@@ -24,14 +25,17 @@
         beamsize values
     axis : str
         "x" or "y"
     w : list, optional
         weights for beamsize values, by default None
     num_points : int, optional
         number of points to add, by default 5
+    bounds: tuple or None
+        Bounds of (min, max) to be honored.
+        If given, will clip the output to be within these bounds.
         
     Returns 
     -------
     list
         new quad values
     
     """
@@ -79,18 +83,22 @@
     fit_coefs, fit_cov = curve_fit(func, x, y_squared)
 
     # space over which to fit
     x_fit = np.linspace(min_x, max_x, 25)
 
     # no more restrictions on quad vals, just staying within
     # the region already scanned (can increase this if need be)
-    min_x_range, max_x_range = np.min([min_x, x[np.argmin(y)] - 2.5]), np.max(
-        [max_x, x[np.argmin(y)] + 2.5]
-    )
-
+    
+    min_x_range = np.min([min_x, x[np.argmin(y)] - 2.5]) # TODO: where does 2.5 come from?
+    max_x_range =  np.max([max_x, x[np.argmin(y)] + 2.5])
+    # Restrict to be within bounds
+    if bounds is not None:
+        min_x_range = max(min_x_range, bounds[0])
+        max_x_range = min(max_x_range, bounds[1])
+        
     c2, c1, c0 = fit_coefs
 
     if c2 < 0:  # same if s11q is negative
         logger.debug("Adjusting concave poly.")
         # go to lower side of concave polynomials
         # (assuming it is closer to the local minimum)
         x_min_concave = x[np.argmin(y)]
@@ -134,56 +142,57 @@
 
     x_fine_fit = np.linspace(roots.min(), roots.max(), num_points)
 
     # return the new quad measurement range for this axis (machine units)
     return list(x_fine_fit)
 
 
-def check_symmetry(x, y, y_err, axis, bs_fn=None, add_meas=False):
+def check_symmetry(x, y, y_err, axis, bs_fn=None, add_meas=False, bounds=None):
     """Check symmetry of quad scan around min of scan
     and find side (left or right) and num of beamsize
     points to add to get a full curve"""
 
     if len(y) != len(x):
         raise Exception("Array lengths do not match!")
 
     # get number of points on left and right side
     left_side = np.argmin(y)
     right_side = len(x) - left_side - 1
     stepsize = abs((x[0] - x[-1]) / len(x))
 
     if left_side == right_side:
         return None
-
     elif left_side > right_side:
         add_to_side = "right"
         diff = left_side - right_side
         # add points to right_side
         xmin = x[-1] + stepsize
         xmax = xmin + diff * stepsize
-        x_add = np.linspace(xmin, xmax, diff)
-
     elif right_side > left_side:
         add_to_side = "left"
         diff = right_side - left_side
         # add points to left_side
         xmin = x[0] - diff * stepsize
         xmax = x[0] - stepsize
-        x_add = np.linspace(xmin, xmax, diff)
+    x_add = np.linspace(xmin, xmax, diff)
+    
+    # Restrict to be within bounds
+    if bounds is not None:
+        x_add = np.clip(x_add, bounds[0], bounds[1])
 
     if add_meas:
         return add_measurements(add_to_side, x_add, x, y, y_err, axis, bs_fn)
     else:
         return add_to_side, x_add
 
 
 def add_measurements(add_to_side, x_add, x, y, y_err, axis, bs_fn):
     """Add beamsize measurements on left or right side based on
     symmetry of scan curve.
-    x_add are the quad scan values k in units of 1/m^2"""
+    x_add are the quad scan values k in units of 1/m^2""" # TODO: this is wrong
 
     # get new data points
     idx_size = 1 if axis == "y" else 0
     idx_err = 3 if axis == "y" else 2
     new_data = bs_fn(x_add)
     y_add, y_err_add = new_data[idx_size], new_data[idx_err]
```

### Comparing `pyemittance-1.0.1/pyemittance/emittance_calc.py` & `pyemittance-1.1.0/pyemittance/emittance_calc.py`

 * *Files identical despite different names*

### Comparing `pyemittance-1.0.1/pyemittance/image.py` & `pyemittance-1.1.0/pyemittance/image.py`

 * *Files identical despite different names*

### Comparing `pyemittance-1.0.1/pyemittance/load_json_configs.py` & `pyemittance-1.1.0/pyemittance/load_json_configs.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 CONFIG_PATH = os.path.join(this_dir, "configs")
 
 # default jsons that include the configurations for the emittance scan
 json_namelist = [
     "beamline_info",
     "img_proc",
     "meas_pv_info",
-    "opt_pv_info",
-    "save_scalar_pvs",
+  #   "opt_pv_info",
+  #  "save_scalar_pvs",
     "savepaths",
 ]
 
 
 def load_configs(dir_name="LCLS2_OTR0H04"):
     all_data = {}
     for i in range(len(json_namelist)):
```

### Comparing `pyemittance-1.0.1/pyemittance/machine_io.py` & `pyemittance-1.1.0/pyemittance/machine_io.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,61 +12,80 @@
 class MachineIO:
     """Class for handling all machine I/O"""
 
     def __init__(self, config_name="LCLS_OTR2", config_dict=None, meas_type="OTRS"):
         # specify OTRS or WIRE scans
         self.meas_type = meas_type
         self.online = False
-        self.settle_time = 0.1  # sleep time in seconds
+
 
         # Set configs for measurement
         # if config is not provided, use LCLS OTR2 as default
         if config_dict is None and config_name is None:
             logger.info("No configuration specified. Taking default LCLS-OTR2 configs.")
             self.config_name = "LCLS_OTR2"
             self.config_dict = self.load_config()
         else:
             self.config_name = config_name
             self.config_dict = config_dict if config_dict else self.load_config()
 
         self.meas_pv_info = self.config_dict["meas_pv_info"]
 
+        meas_device = self.meas_pv_info["meas_device"]
+        if "settle_time" in meas_device:
+            self.settle_time = meas_device["settle_time"]
+        else:
+            self.settle_time = 0
+            logger.warning("No settle_time found in in meas_device, setting to zero")
+
+        
+        if "bounds" in meas_device:
+            self.bounds = meas_device["bounds"]
+        else:
+            self.bounds = None
+
         # Connect to PVs 
         self.meas_read_pv = PV(self.meas_pv_info["meas_device"]["pv"]["read"])
         self.meas_cntrl_pv = PV(self.meas_pv_info["meas_device"]["pv"]["cntrl"])
 
-        # load info about settings to optimize
-        self.opt_pv_info = self.config_dict["opt_pv_info"]
-        self.opt_pvs = self.opt_pv_info["opt_vars"]
-
     def load_config(self):
         # if path exists, load from path
         if self.config_name is not None:
             self.config_dict = load_configs(self.config_name)
         return self.config_dict
 
     def get_beamsizes_machine(self, quad_val):
         """Fn that pyemittance.observer calls
         Takes quad value as input,
         Returns xrms, yrms, xrms_err, yrms_err
         """
         if self.online and quad_val is not None:
             self.setquad(quad_val)
-            time.sleep(self.settle_time)
+            if self.settle_time > 0:  
+                logger.info(f"Settling for {self.settle_time} s...")
+                time.sleep(self.settle_time)
         
         if self.meas_type == "OTRS" and self.online:
             return get_beamsizes_otrs(self.config_dict)
         elif self.meas_type == "WIRE" and self.online:
             logger.info("Running wire scanner")
             return get_beamsizes_wire(self.online, self.config_dict)
         elif not self.online:
             return np.random.uniform(0.5e-4, 5e-4), np.random.uniform(1e-4, 6e-4), 0, 0
         else:
             raise NotImplementedError("No valid measurement type defined.")
     def setquad(self, value):
         """Sets quad to new scan value"""
+
+        if self.bounds is not None:
+            lower, upper = self.bounds
+            if value < lower:
+                raise ValueError(f'Quad set point value {value} < {lower} lower limit')
+            if value > upper:
+                raise ValueError(f'Quad set point value {value} > {upper} upper limit')                
+        
         if self.online:
             logger.info(f'EPICS put {self.meas_cntrl_pv.pvname} = {value}')
             self.meas_cntrl_pv.put(value)
         else:
             logger.info("Not setting quad online values.")
             pass
```

### Comparing `pyemittance-1.0.1/pyemittance/machine_settings.py` & `pyemittance-1.1.0/pyemittance/machine_settings.py`

 * *Files identical despite different names*

### Comparing `pyemittance-1.0.1/pyemittance/observer.py` & `pyemittance-1.1.0/pyemittance/observer.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,20 +14,14 @@
     def __init__(self, quad_meas, beam_meas, beam_meas_err):
         self.quad_meas = quad_meas
         self.beam_meas = beam_meas
         self.beam_meas_err = beam_meas_err
         self.use_prev_meas = False
         self.tolerance = 0.1
 
-        self.inj_config = None  # injector configuration settings for SOL, CQ, SQ
-        self.use_model = True
-        # if using the surrogate model
-        self.get_beamsizes_model = None
-        self.noise_red = 100000
-
         # if using machine
         self.online = False
         self.config_name = "sim"
         self.config_dict = None
         self.meas_type = "OTRS"
 
 
@@ -114,21 +108,10 @@
                     yrms.append(self.beam_meas["y"][use_loc])
                     xrms_err.append(self.beam_meas_err["x"][use_loc])
                     yrms_err.append(self.beam_meas_err["y"][use_loc])
 
         return xrms, yrms, xrms_err, yrms_err
 
     def get_beamsizes(self, val):
-        """Define where the beamsizes are acquired from"""
-        if self.use_model:
-            if len(np.asarray(self.inj_config).shape) == 2:
-                # temp workaround for testing
-                out = self.get_beamsizes_model(self.inj_config[0] + [val])
-                return np.array([out["sigma_x"][0], out["sigma_y"][0], 0.0, 0.0])
-
-            return self.get_beamsizes_model(self.inj_config, val)
-
-        else:
-            io = MachineIO(self.config_name, self.config_dict, self.meas_type)
-            io.online = self.online
-            # note we are not setting the injector on the machine here
-            return io.get_beamsizes_machine(val)
+        io = MachineIO(self.config_name, self.config_dict, self.meas_type)
+        io.online = self.online
+        return io.get_beamsizes_machine(val)
```

### Comparing `pyemittance-1.0.1/pyemittance/optics.py` & `pyemittance-1.1.0/pyemittance/optics.py`

 * *Files identical despite different names*

### Comparing `pyemittance-1.0.1/pyemittance/otrs_io.py` & `pyemittance-1.1.0/pyemittance/otrs_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import datetime
 from epics import caget, PV
 from pyemittance.image import Image
-from pyemittance.saving_io import save_image, numpy_save, save_config
+from pyemittance.saving_io import save_image, save_config
 import os
 
 import logging
 logger = logging.getLogger(__name__)
 
 def get_beamsizes_otrs(config_dict):
     """Main function imported by machine_io
@@ -24,20 +24,17 @@
     config_dict, reject_bad_beam=True, save_summary=False,
 ):
     """Data acquisition from OTRS
     Additional option to reject bad beams
     Returns xrms, yrms, xrms_err, yrms_err
     """
     # Saving configs
-    opt_pv_info = config_dict["opt_pv_info"]
     meas_pv_info = config_dict["meas_pv_info"]
     meas_read_pv = meas_pv_info["meas_device"]["pv"]["read"]
-    opt_pvs = opt_pv_info["opt_vars"]
     savepaths = config_dict["savepaths"]
-    pv_savelist = config_dict["save_scalar_pvs"]
     # Load image processing setting info
     im_proc = config_dict["img_proc"]
     amp_threshold_x = im_proc["amp_threshold"]
     amp_threshold_y = im_proc["amp_threshold"]
     max_samples = im_proc["max_samples"]
 
     # Measurement PVs
@@ -119,27 +116,17 @@
         save_config(
             xrms,
             yrms,
             xrms_err,
             yrms_err,
             timestamp,
             meas_read_pv,
-            opt_pvs,
             configpath=savepaths["summaries"],
             impath=savepaths["images"],
         )
-        numpy_save(
-            xrms,
-            yrms,
-            xrms_err,
-            yrms_err,
-            timestamp,
-            savelist=pv_savelist["scalars"],
-            path=savepaths["raw_saves"],
-        )
 
     return xrms, yrms, xrms_err, yrms_err
 
 
 def getbeamsizes_from_img(config_dict):
     """Returns xrms, yrms, xrms_err, yrms_err for multiple sampled images;
     can optionally average multiple images
```

### Comparing `pyemittance-1.0.1/pyemittance/pyemittance.py` & `pyemittance-1.1.0/pyemittance/pyemittance.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import numpy as np
 from pyemittance.observer import Observer
 from pyemittance.data_handler import (
     adapt_range,
     check_symmetry,
     find_inflection_pnt,
     add_measurements_btwn_pnts,
 )
@@ -29,43 +30,69 @@
 
         self.meas_type = meas_type
         # if running on machine, use_model=False
         self.use_model = use_model
         # only True if setting PVs
         self.online = online
 
-        # injector settings (SOL, CQ, SQ) if optimizing
-        self.inj_config = None
         # initial rough quad scan
-        self.quad_init = [-6, -4, -2, 0]
+        self._quad_init = [-6, -4, -2, 0]
 
         # pyemittance method options
         self.adapt_ranges = True
+        self.settle_time = 0
         self.num_points = 7
-        self.check_sym = True
-        self.infl_check = True
-        self.add_pnts = True
+        self.check_sym = True  # check_sym will add more points to fill out a parabola
+        self.infl_check = True # truncates data outside inflection point
+        self.add_pnts = True   # ensures there are .num_points by adding points in between previous
         self.show_plots = False
         self.use_prev_meas = True
         self.quad_tol = 0.05
         self.save_runs = False
         self.calc_bmag = False
 
         # simulation/model options
         # beamsize function from model
         self.get_bs_model = None
 
         # to save total number of points queried
         self.return_num_points = False
 
+    @property
+    def quad_bounds(self):
+        """
+        Returns a tuple of floats: (lower, upper) limit for quad bounds.
+        """
+        if "bounds" not in self.config_dict["meas_pv_info"]["meas_device"]:
+            bounds =  min(self.quad_init), max(self.quad_init)
+        else:
+            bounds = self.config_dict["meas_pv_info"]["meas_device"]["bounds"]
+            if bounds is None:
+                bounds = min(self.quad_init), max(self.quad_init)
+        return bounds
+            
+    @quad_bounds.setter
+    def quad_bounds(self, value):
+        self.config_dict["meas_pv_info"]["meas_device"]["bounds"] = value
+
+    @property 
+    def quad_init(self):
+        return self._quad_init
+    @quad_init.setter
+    def quad_init(self, values):
+        self._quad_init = list(values)
+    def clip_quad_values(self, values):
+        lower, upper = self.quad_bounds
+        return list(np.clip(values, lower, upper))
+        
+
     def measure_emittance(self):
         # get initial points from the observer
         o = Observer([], {"x": [], "y": []}, {"x": [], "y": []})
         o.use_model = self.use_model
-        o.inj_config = self.inj_config
         o.online = self.online
         o.meas_type = self.meas_type
         o.use_prev_meas = self.use_prev_meas
         o.tolerance = self.quad_tol
 
         # logger.info warning
         if self.online:
@@ -88,63 +115,72 @@
             self.quad_init
         )
 
         quad_range_x = self.quad_init
         quad_range_y = self.quad_init
 
         if self.adapt_ranges:
+            logger.info('Adapting ranges')
             quad_range_x = adapt_range(
                 quad_range_x,
                 bs_x_list,
                 "x",
                 w=bs_x_list_err,
                 num_points=self.num_points,
+                bounds = self.quad_bounds,
             )
             quad_range_y = adapt_range(
                 quad_range_y,
                 bs_y_list,
                 "y",
                 w=bs_y_list_err,
                 num_points=self.num_points,
+                bounds = self.quad_bounds,
             )
-
+            logger.info(f"Adapting ranges for x beam size measurement: {quad_range_x}")
             new_beamsize_x = o.measure_beam(quad_range_x)
             bs_x_list, bs_x_list_err = new_beamsize_x[0], new_beamsize_x[2]
+
+            logger.info(f"Adapting ranges for y beam size measurement: {quad_range_y}")
             new_beamsize_y = o.measure_beam(quad_range_y)
             bs_y_list, bs_y_list_err = new_beamsize_y[1], new_beamsize_y[3]
 
         if self.check_sym:
+            logger.info('Checking symmetry')
             add_points_x = check_symmetry(
                 quad_range_x,
                 bs_x_list,
                 bs_x_list_err,
                 "x",
                 bs_fn=o.measure_beam,
                 add_meas=True,
+                bounds = self.quad_bounds,
             )
             add_points_y = check_symmetry(
                 quad_range_y,
                 bs_y_list,
                 bs_y_list_err,
                 "y",
                 bs_fn=o.measure_beam,
                 add_meas=True,
+                bounds = self.quad_bounds,
             )
 
             if add_points_x is not None:
                 quad_range_x = add_points_x[0]
                 bs_x_list = add_points_x[1]
                 bs_x_list_err = add_points_x[2]
 
             if add_points_y is not None:
                 quad_range_y = add_points_y[0]
                 bs_y_list = add_points_y[1]
                 bs_y_list_err = add_points_y[2]
 
         if self.infl_check:
+            logger.info('Checking inflection')
             left_x, right_x = find_inflection_pnt(
                 quad_range_x, bs_x_list, show_plots=self.show_plots
             )
             left_y, right_y = find_inflection_pnt(
                 quad_range_y, bs_y_list, show_plots=self.show_plots
             )
 
@@ -154,14 +190,15 @@
             bs_x_list_err = bs_x_list_err[left_x:right_x]
 
             quad_range_y = quad_range_y[left_y:right_y]
             bs_y_list = bs_y_list[left_y:right_y]
             bs_y_list_err = bs_y_list_err[left_y:right_y]
 
         if self.add_pnts:
+            logger.info('Adding points')
             quad_range_x, bs_x_list, bs_x_list_err = add_measurements_btwn_pnts(
                 quad_range_x,
                 bs_x_list,
                 bs_x_list_err,
                 self.num_points,
                 "x",
                 bs_fn=o.measure_beam,
@@ -171,14 +208,15 @@
                 bs_y_list,
                 bs_y_list_err,
                 self.num_points,
                 "y",
                 bs_fn=o.measure_beam,
             )
 
+        logger.info(f"Emmitance calc for {len(quad_range_x)} x points, {len(quad_range_x)} y points" )
         # finally get emittance
         ef = EmitCalc(
             {"x": quad_range_x, "y": quad_range_y},
             {"x": bs_x_list, "y": bs_y_list},
             {"x": bs_x_list_err, "y": bs_y_list_err},
             config_dict=o.config_dict,
         )
```

### Comparing `pyemittance-1.0.1/pyemittance/saving_io.py` & `pyemittance-1.1.0/pyemittance/saving_io.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,51 +18,33 @@
     else:
 
         np.save(str(impath) + f"img_{timestamp}.npy", im)
         np.save(str(impath) + f"ncol_{timestamp}.npy", ncol)
         np.save(str(impath) + f"nrow_{timestamp}.npy", nrow)
 
 
-def numpy_save(xrms, yrms, xrms_err, yrms_err, timestamp=False, savelist="", path=""):
-    ts = isotime()
-    x = caget_many(savelist)
-    if timestamp:
-        x.append(timestamp)
-    else:
-        x.append(ts)
-    x.append(xrms)
-    x.append(yrms)
-    x.append(xrms_err)
-    x.append(yrms_err)
-
-    np.save(path + ts + "_pv_bs_data_.npy", np.array(x))
-
-
 def save_config(
     xrms,
     yrms,
     xrms_err,
     yrms_err,
     timestamp,
     meas_read_pv,
-    opt_pvs,
     im=None,
     configpath="",
     impath="",
 ):
     if timestamp is None:
         f = open(configpath + "bax_beamsize_config_info.csv", "a+")
         timestamp = isotime()
     else:
         f = open(configpath + "beamsize_config_info.csv", "a+")
 
     # todo make more general, pandas etc
-    varx_cur = caget(opt_pvs[0])
-    vary_cur = caget(opt_pvs[1])
-    varz_cur = caget(opt_pvs[2])
+
     bact_cur = caget(meas_read_pv)
     f.write(
         f"{timestamp},{varx_cur},{vary_cur},{varz_cur},"
         f"{bact_cur},{xrms},{yrms},{xrms_err},{yrms_err}\n"
     )
 
     f.close()
```

### Comparing `pyemittance-1.0.1/pyemittance/simulation.py` & `pyemittance-1.1.0/pyemittance/simulation.py`

 * *Files identical despite different names*

### Comparing `pyemittance-1.0.1/pyemittance/simulation_server.py` & `pyemittance-1.1.0/pyemittance/simulation_server.py`

 * *Files identical despite different names*

### Comparing `pyemittance-1.0.1/pyemittance/tools.py` & `pyemittance-1.1.0/pyemittance/tools.py`

 * *Files identical despite different names*

### Comparing `pyemittance-1.0.1/pyemittance/wire_io.py` & `pyemittance-1.1.0/pyemittance/wire_io.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import time
 import datetime
 from epics import PV
-from pyemittance.saving_io import numpy_save, save_config
+from pyemittance.saving_io import save_config
 
 import logging
 logger = logging.getLogger(__name__)
 
 def get_beamsizes_wire(online=False, config_dict=None, save_summary=False):
     """Main function imported by machine_io
     Returns xrms, yrms, xrms_err, yrms_err
     """
     # Saving configs
-    opt_pv_info = config_dict["opt_pv_info"]
     meas_pv_info = config_dict["meas_pv_info"]
     meas_read_pv = meas_pv_info["meas_device"]["pv"]["read"]
-    opt_pvs = opt_pv_info["opt_vars"]
     savepaths = config_dict["savepaths"]
     pv_savelist = config_dict["save_scalar_pvs"]
     # Measurement PVs
     meas_pv_info = config_dict["meas_pv_info"]
     # BS in meters for emittance calc
     scan_pv = PV(meas_pv_info["diagnostic"]["pv"]["scan"])
     x_size_pv = PV(meas_pv_info["diagnostic"]["pv"]["xsize"])
@@ -39,27 +37,17 @@
         save_config(
             xrms,
             yrms,
             xrms_err,
             yrms_err,
             timestamp,
             meas_read_pv,
-            opt_pvs,
             configpath=savepaths["summaries"],
             impath=savepaths["images"],
         )
-        numpy_save(
-            xrms,
-            yrms,
-            xrms_err,
-            yrms_err,
-            timestamp,
-            savelist=pv_savelist["scalars"],
-            path=savepaths["raw_saves"],
-        )
 
     return xrms, yrms, xrms_err, yrms_err
 
 
 def get_beamsize(online, scan_pv):
     if online:
         scan_pv.put(1)
```

### Comparing `pyemittance-1.0.1/pyemittance.egg-info/PKG-INFO` & `pyemittance-1.1.0/pyemittance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyemittance
-Version: 1.0.1
+Version: 1.1.0
 Home-page: https://github.com/slaclab/PyEmittance
 Author: Sara Miskovich
 Author-email: smiskov@slac.stanford.edu
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyemittance-1.0.1/pyemittance.egg-info/SOURCES.txt` & `pyemittance-1.1.0/pyemittance.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -33,16 +33,14 @@
 pyemittance/configs/FACET_nominal/meas_pv_info.json
 pyemittance/configs/FACET_nominal/opt_pv_info.json
 pyemittance/configs/FACET_nominal/save_scalar_pvs.json
 pyemittance/configs/FACET_nominal/savepaths.json
 pyemittance/configs/LCLS2_OTR0H04/beamline_info.json
 pyemittance/configs/LCLS2_OTR0H04/img_proc.json
 pyemittance/configs/LCLS2_OTR0H04/meas_pv_info.json
-pyemittance/configs/LCLS2_OTR0H04/opt_pv_info.json
-pyemittance/configs/LCLS2_OTR0H04/save_scalar_pvs.json
 pyemittance/configs/LCLS2_OTR0H04/savepaths.json
 pyemittance/configs/LCLS_OTR1/beamline_info.json
 pyemittance/configs/LCLS_OTR1/img_proc.json
 pyemittance/configs/LCLS_OTR1/meas_pv_info.json
 pyemittance/configs/LCLS_OTR1/opt_pv_info.json
 pyemittance/configs/LCLS_OTR1/save_scalar_pvs.json
 pyemittance/configs/LCLS_OTR1/savepaths.json
@@ -77,8 +75,10 @@
 pyemittance/configs/latest_facet/save_scalar_pvs.json
 pyemittance/configs/latest_facet/savepaths.json
 pyemittance/configs/sim/beamline_info.json
 pyemittance/configs/sim/img_proc.json
 pyemittance/configs/sim/meas_pv_info.json
 pyemittance/configs/sim/opt_pv_info.json
 pyemittance/configs/sim/save_scalar_pvs.json
-pyemittance/configs/sim/savepaths.json
+pyemittance/configs/sim/savepaths.json
+tests/test_measurement.py
+tests/test_online.py
```

### Comparing `pyemittance-1.0.1/setup.py` & `pyemittance-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `pyemittance-1.0.1/versioneer.py` & `pyemittance-1.1.0/versioneer.py`

 * *Files identical despite different names*

