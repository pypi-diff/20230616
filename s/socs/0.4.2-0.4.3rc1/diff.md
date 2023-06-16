# Comparing `tmp/socs-0.4.2.tar.gz` & `tmp/socs-0.4.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socs-0.4.2.tar", last modified: Wed Apr 19 16:58:31 2023, max compression
+gzip compressed data, was "socs-0.4.3rc1.tar", last modified: Fri Jun 16 18:58:01 2023, max compression
```

## Comparing `socs-0.4.2.tar` & `socs-0.4.3rc1.tar`

### file list

```diff
@@ -1,190 +1,200 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.646277 socs-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-19 16:58:14.000000 socs-0.4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-19 16:58:14.000000 socs-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-04-19 16:58:31.646277 socs-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-19 16:58:14.000000 socs-0.4.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-19 16:58:14.000000 socs-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-19 16:58:31.646277 socs-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-19 16:58:14.000000 socs-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.646277 socs-0.4.2/socs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.622276 socs-0.4.2/socs/Lakeshore/
--rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-04-19 16:58:14.000000 socs-0.4.2/socs/Lakeshore/Lakeshore240.py
--rw-r--r--   0 runner    (1001) docker     (123)    40327 2023-04-19 16:58:14.000000 socs-0.4.2/socs/Lakeshore/Lakeshore336.py
--rw-r--r--   0 runner    (1001) docker     (123)    56866 2023-04-19 16:58:14.000000 socs-0.4.2/socs/Lakeshore/Lakeshore370.py
--rw-r--r--   0 runner    (1001) docker     (123)    57733 2023-04-19 16:58:14.000000 socs-0.4.2/socs/Lakeshore/Lakeshore372.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1444 2023-04-19 16:58:14.000000 socs-0.4.2/socs/Lakeshore/Lakeshore425.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/Lakeshore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-19 16:58:14.000000 socs-0.4.2/socs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-19 16:58:31.646277 socs-0.4.2/socs/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.622276 socs-0.4.2/socs/agents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.622276 socs-0.4.2/socs/agents/acu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/acu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60407 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/acu/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    19641 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/acu/drivers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.622276 socs-0.4.2/socs/agents/bluefors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/bluefors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19253 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/bluefors/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.622276 socs-0.4.2/socs/agents/cryomech_cpa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/cryomech_cpa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/cryomech_cpa/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.622276 socs-0.4.2/socs/agents/fts_aerotech/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/fts_aerotech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12424 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/fts_aerotech/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.622276 socs-0.4.2/socs/agents/holo_fpga/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/holo_fpga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/holo_fpga/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.622276 socs-0.4.2/socs/agents/holo_synth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/holo_synth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/holo_synth/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.622276 socs-0.4.2/socs/agents/hwp_encoder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/hwp_encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29096 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/hwp_encoder/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.626276 socs-0.4.2/socs/agents/hwp_picoscope/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/hwp_picoscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/hwp_picoscope/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.626276 socs-0.4.2/socs/agents/hwp_picoscope/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/hwp_picoscope/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21269 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/hwp_picoscope/drivers/class_ps3000a.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.626276 socs-0.4.2/socs/agents/hwp_rotation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/hwp_rotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18596 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/hwp_rotation/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.626276 socs-0.4.2/socs/agents/hwp_rotation/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/hwp_rotation/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/hwp_rotation/drivers/pid_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.626276 socs-0.4.2/socs/agents/ibootbar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/ibootbar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15136 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/ibootbar/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.626276 socs-0.4.2/socs/agents/labjack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/labjack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20201 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/labjack/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.626276 socs-0.4.2/socs/agents/labjack/cal_curves/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/labjack/cal_curves/GA10K4D25_cal_curve.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.626276 socs-0.4.2/socs/agents/lakeshore240/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/lakeshore240/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/lakeshore240/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.626276 socs-0.4.2/socs/agents/lakeshore336/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/lakeshore336/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48306 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/lakeshore336/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.626276 socs-0.4.2/socs/agents/lakeshore370/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/lakeshore370/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36049 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/lakeshore370/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.630276 socs-0.4.2/socs/agents/lakeshore372/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/lakeshore372/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64295 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/lakeshore372/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.630276 socs-0.4.2/socs/agents/lakeshore425/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/lakeshore425/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9229 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/lakeshore425/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.630276 socs-0.4.2/socs/agents/magpie/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/magpie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37829 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/magpie/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.630276 socs-0.4.2/socs/agents/meinberg_m1000/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/meinberg_m1000/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17785 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/meinberg_m1000/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/ocs_plugin_so.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.630276 socs-0.4.2/socs/agents/pfeiffer_tc400/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/pfeiffer_tc400/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/pfeiffer_tc400/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/pfeiffer_tc400/drivers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.630276 socs-0.4.2/socs/agents/pfeiffer_tpg366/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/pfeiffer_tpg366/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/pfeiffer_tpg366/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.630276 socs-0.4.2/socs/agents/pysmurf_controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/pysmurf_controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35232 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/pysmurf_controller/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.634276 socs-0.4.2/socs/agents/pysmurf_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/pysmurf_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/pysmurf_monitor/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.634276 socs-0.4.2/socs/agents/scpi_psu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/scpi_psu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/scpi_psu/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/scpi_psu/drivers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.634276 socs-0.4.2/socs/agents/smurf_crate_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/smurf_crate_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/smurf_crate_monitor/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.634276 socs-0.4.2/socs/agents/smurf_file_emulator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/smurf_file_emulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25842 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/smurf_file_emulator/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)   105526 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/smurf_file_emulator/status_sample.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.634276 socs-0.4.2/socs/agents/smurf_stream_simulator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/smurf_stream_simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/smurf_stream_simulator/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.634276 socs-0.4.2/socs/agents/smurf_timing_card/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/smurf_timing_card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/smurf_timing_card/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.634276 socs-0.4.2/socs/agents/suprsync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/suprsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/suprsync/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.638277 socs-0.4.2/socs/agents/synacc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/synacc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/synacc/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.638277 socs-0.4.2/socs/agents/tektronix3021c/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/tektronix3021c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/tektronix3021c/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/tektronix3021c/drivers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.638277 socs-0.4.2/socs/agents/thorlabs_mc2000b/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/thorlabs_mc2000b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/thorlabs_mc2000b/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.638277 socs-0.4.2/socs/agents/ups/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/ups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14781 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/ups/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.638277 socs-0.4.2/socs/agents/vantagepro2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/vantagepro2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/vantagepro2/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/vantagepro2/drivers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.638277 socs-0.4.2/socs/agents/wiregrid_actuator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_actuator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34937 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_actuator/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.638277 socs-0.4.2/socs/agents/wiregrid_actuator/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)    14540 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_actuator/drivers/Actuator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7945 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_actuator/drivers/DigitalIO.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_actuator/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_actuator/limitswitch_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_actuator/stopper_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.642277 socs-0.4.2/socs/agents/wiregrid_encoder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_encoder/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_encoder/drivers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.642277 socs-0.4.2/socs/agents/wiregrid_kikusui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_kikusui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24161 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_kikusui/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.642277 socs-0.4.2/socs/agents/wiregrid_kikusui/drivers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_kikusui/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/wiregrid_kikusui/drivers/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.642277 socs-0.4.2/socs/agents/xy_stage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/xy_stage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-04-19 16:58:14.000000 socs-0.4.2/socs/agents/xy_stage/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.642277 socs-0.4.2/socs/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-04-19 16:58:14.000000 socs-0.4.2/socs/common/moxa_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-04-19 16:58:14.000000 socs-0.4.2/socs/common/pmx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-19 16:58:14.000000 socs-0.4.2/socs/common/prologix_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.642277 socs-0.4.2/socs/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16265 2023-04-19 16:58:14.000000 socs-0.4.2/socs/db/suprsync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.646277 socs-0.4.2/socs/mibs/
--rw-r--r--   0 runner    (1001) docker     (123)    17434 2023-04-19 16:58:14.000000 socs-0.4.2/socs/mibs/IBOOTPDU-MIB.py
--rw-r--r--   0 runner    (1001) docker     (123)   143372 2023-04-19 16:58:14.000000 socs-0.4.2/socs/mibs/MBG-SNMP-LTNG-MIB.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-19 16:58:14.000000 socs-0.4.2/socs/mibs/MBG-SNMP-ROOT-MIB.py
--rw-r--r--   0 runner    (1001) docker     (123)    16838 2023-04-19 16:58:14.000000 socs-0.4.2/socs/mibs/SNMPv2-MIB.py
--rw-r--r--   0 runner    (1001) docker     (123)    38813 2023-04-19 16:58:14.000000 socs-0.4.2/socs/mibs/UPS-MIB.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/mibs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-04-19 16:58:14.000000 socs-0.4.2/socs/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-04-19 16:58:14.000000 socs-0.4.2/socs/snmp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.646277 socs-0.4.2/socs/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:14.000000 socs-0.4.2/socs/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-04-19 16:58:14.000000 socs-0.4.2/socs/testing/device_emulator.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-19 16:58:14.000000 socs-0.4.2/socs/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.618276 socs-0.4.2/socs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-04-19 16:58:31.000000 socs-0.4.2/socs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-19 16:58:31.000000 socs-0.4.2/socs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:58:31.000000 socs-0.4.2/socs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-19 16:58:31.000000 socs-0.4.2/socs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-19 16:58:31.000000 socs-0.4.2/socs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 16:58:31.000000 socs-0.4.2/socs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:58:31.646277 socs-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-19 16:58:14.000000 socs-0.4.2/tests/test_device_emulator.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-19 16:58:14.000000 socs-0.4.2/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-19 16:58:14.000000 socs-0.4.2/tests/test_snmp.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-19 16:58:14.000000 socs-0.4.2/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    69022 2023-04-19 16:58:14.000000 socs-0.4.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.935317 socs-0.4.3rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-16 18:57:47.000000 socs-0.4.3rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-16 18:57:47.000000 socs-0.4.3rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-06-16 18:58:01.935317 socs-0.4.3rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-06-16 18:57:47.000000 socs-0.4.3rc1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-16 18:57:47.000000 socs-0.4.3rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-16 18:58:01.939317 socs-0.4.3rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-06-16 18:57:47.000000 socs-0.4.3rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.939317 socs-0.4.3rc1/socs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.923317 socs-0.4.3rc1/socs/Lakeshore/
+-rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/Lakeshore/Lakeshore240.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40327 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/Lakeshore/Lakeshore336.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56866 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/Lakeshore/Lakeshore370.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57733 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/Lakeshore/Lakeshore372.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1444 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/Lakeshore/Lakeshore425.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/Lakeshore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-16 18:58:01.939317 socs-0.4.3rc1/socs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.923317 socs-0.4.3rc1/socs/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.923317 socs-0.4.3rc1/socs/agents/acu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/acu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67412 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/acu/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19641 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/acu/drivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/acu/exercisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.923317 socs-0.4.3rc1/socs/agents/bluefors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/bluefors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19253 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/bluefors/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.923317 socs-0.4.3rc1/socs/agents/cryomech_cpa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/cryomech_cpa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/cryomech_cpa/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.923317 socs-0.4.3rc1/socs/agents/fts_aerotech/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/fts_aerotech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12424 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/fts_aerotech/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.923317 socs-0.4.3rc1/socs/agents/holo_fpga/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/holo_fpga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/holo_fpga/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.923317 socs-0.4.3rc1/socs/agents/holo_synth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/holo_synth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/holo_synth/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.923317 socs-0.4.3rc1/socs/agents/hwp_encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/hwp_encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29096 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/hwp_encoder/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.923317 socs-0.4.3rc1/socs/agents/hwp_picoscope/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/hwp_picoscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/hwp_picoscope/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.923317 socs-0.4.3rc1/socs/agents/hwp_picoscope/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/hwp_picoscope/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21269 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/hwp_picoscope/drivers/class_ps3000a.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.923317 socs-0.4.3rc1/socs/agents/hwp_pid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/hwp_pid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13653 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/hwp_pid/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.923317 socs-0.4.3rc1/socs/agents/hwp_pid/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/hwp_pid/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/hwp_pid/drivers/pid_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.923317 socs-0.4.3rc1/socs/agents/hwp_pmx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/hwp_pmx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11478 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/hwp_pmx/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.927317 socs-0.4.3rc1/socs/agents/hwp_pmx/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/hwp_pmx/drivers/PMX_ethernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/hwp_pmx/drivers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.927317 socs-0.4.3rc1/socs/agents/ibootbar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/ibootbar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/ibootbar/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.927317 socs-0.4.3rc1/socs/agents/ifm_sbn246_flowmeter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/ifm_sbn246_flowmeter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/ifm_sbn246_flowmeter/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.927317 socs-0.4.3rc1/socs/agents/labjack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/labjack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20308 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/labjack/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.927317 socs-0.4.3rc1/socs/agents/labjack/cal_curves/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/labjack/cal_curves/GA10K4D25_cal_curve.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.927317 socs-0.4.3rc1/socs/agents/lakeshore240/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/lakeshore240/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12026 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/lakeshore240/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.927317 socs-0.4.3rc1/socs/agents/lakeshore336/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/lakeshore336/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48306 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/lakeshore336/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.927317 socs-0.4.3rc1/socs/agents/lakeshore370/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/lakeshore370/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36049 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/lakeshore370/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.927317 socs-0.4.3rc1/socs/agents/lakeshore372/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/lakeshore372/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64295 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/lakeshore372/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.927317 socs-0.4.3rc1/socs/agents/lakeshore425/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/lakeshore425/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9229 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/lakeshore425/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.927317 socs-0.4.3rc1/socs/agents/magpie/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/magpie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37829 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/magpie/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.927317 socs-0.4.3rc1/socs/agents/meinberg_m1000/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/meinberg_m1000/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17785 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/meinberg_m1000/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/ocs_plugin_so.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.927317 socs-0.4.3rc1/socs/agents/pfeiffer_tc400/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/pfeiffer_tc400/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/pfeiffer_tc400/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/pfeiffer_tc400/drivers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.927317 socs-0.4.3rc1/socs/agents/pfeiffer_tpg366/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/pfeiffer_tpg366/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/pfeiffer_tpg366/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.927317 socs-0.4.3rc1/socs/agents/pysmurf_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/pysmurf_controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37315 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/pysmurf_controller/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.927317 socs-0.4.3rc1/socs/agents/pysmurf_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/pysmurf_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/pysmurf_monitor/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.931317 socs-0.4.3rc1/socs/agents/scpi_psu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/scpi_psu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/scpi_psu/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/scpi_psu/drivers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.931317 socs-0.4.3rc1/socs/agents/smurf_crate_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/smurf_crate_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/smurf_crate_monitor/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.931317 socs-0.4.3rc1/socs/agents/smurf_file_emulator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/smurf_file_emulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26124 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/smurf_file_emulator/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105526 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/smurf_file_emulator/status_sample.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.931317 socs-0.4.3rc1/socs/agents/smurf_stream_simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/smurf_stream_simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/smurf_stream_simulator/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.931317 socs-0.4.3rc1/socs/agents/smurf_timing_card/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/smurf_timing_card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/smurf_timing_card/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.931317 socs-0.4.3rc1/socs/agents/suprsync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/suprsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/suprsync/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.931317 socs-0.4.3rc1/socs/agents/synacc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/synacc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/synacc/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.931317 socs-0.4.3rc1/socs/agents/tektronix3021c/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/tektronix3021c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/tektronix3021c/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/tektronix3021c/drivers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.931317 socs-0.4.3rc1/socs/agents/thorlabs_mc2000b/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/thorlabs_mc2000b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/thorlabs_mc2000b/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.931317 socs-0.4.3rc1/socs/agents/ups/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/ups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14932 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/ups/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.931317 socs-0.4.3rc1/socs/agents/vantagepro2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/vantagepro2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/vantagepro2/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/vantagepro2/drivers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.931317 socs-0.4.3rc1/socs/agents/wiregrid_actuator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/wiregrid_actuator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34937 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/wiregrid_actuator/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.931317 socs-0.4.3rc1/socs/agents/wiregrid_actuator/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)    14540 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/wiregrid_actuator/drivers/Actuator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7945 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/wiregrid_actuator/drivers/DigitalIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/wiregrid_actuator/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/wiregrid_actuator/limitswitch_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/wiregrid_actuator/stopper_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.931317 socs-0.4.3rc1/socs/agents/wiregrid_encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/wiregrid_encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/wiregrid_encoder/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/wiregrid_encoder/drivers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.935317 socs-0.4.3rc1/socs/agents/wiregrid_kikusui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/wiregrid_kikusui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24161 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/wiregrid_kikusui/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.935317 socs-0.4.3rc1/socs/agents/wiregrid_kikusui/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/wiregrid_kikusui/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/wiregrid_kikusui/drivers/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.935317 socs-0.4.3rc1/socs/agents/xy_stage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/xy_stage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/agents/xy_stage/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.935317 socs-0.4.3rc1/socs/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6763 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/common/moxa_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/common/pmx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/common/prologix_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.935317 socs-0.4.3rc1/socs/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16265 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/db/suprsync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.935317 socs-0.4.3rc1/socs/mibs/
+-rw-r--r--   0 runner    (1001) docker     (123)    17434 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/mibs/IBOOTPDU-MIB.py
+-rw-r--r--   0 runner    (1001) docker     (123)   143372 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/mibs/MBG-SNMP-LTNG-MIB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/mibs/MBG-SNMP-ROOT-MIB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16838 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/mibs/SNMPv2-MIB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38813 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/mibs/UPS-MIB.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/mibs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/snmp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.935317 socs-0.4.3rc1/socs/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/testing/device_emulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-16 18:57:47.000000 socs-0.4.3rc1/socs/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.919317 socs-0.4.3rc1/socs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-06-16 18:58:01.000000 socs-0.4.3rc1/socs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-06-16 18:58:01.000000 socs-0.4.3rc1/socs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:58:01.000000 socs-0.4.3rc1/socs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-16 18:58:01.000000 socs-0.4.3rc1/socs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-16 18:58:01.000000 socs-0.4.3rc1/socs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-16 18:58:01.000000 socs-0.4.3rc1/socs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:58:01.935317 socs-0.4.3rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-16 18:57:47.000000 socs-0.4.3rc1/tests/test_device_emulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-16 18:57:47.000000 socs-0.4.3rc1/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-16 18:57:47.000000 socs-0.4.3rc1/tests/test_snmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-16 18:57:47.000000 socs-0.4.3rc1/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69022 2023-06-16 18:57:47.000000 socs-0.4.3rc1/versioneer.py
```

### Comparing `socs-0.4.2/LICENSE.txt` & `socs-0.4.3rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/PKG-INFO` & `socs-0.4.3rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socs
-Version: 0.4.2
+Version: 0.4.3rc1
 Summary: Simons Observatory Control System
 Home-page: https://github.com/simonsobs/socs
 Project-URL: Source Code, https://github.com/simonsobs/ocs
 Project-URL: Documentation, https://ocs.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/simonsobs/ocs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `socs-0.4.2/README.rst` & `socs-0.4.3rc1/README.rst`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/setup.py` & `socs-0.4.3rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,19 +93,20 @@
     ],
     python_requires=">=3.7",
     install_requires=[
         'autobahn[serialization]',
         'numpy',
         'ocs',
         'pyserial',
-        'pysnmp',
+        'pysnmp-lextudio',
         'pysmi',
         'pyyaml',
         'sqlalchemy>=1.4',
         'twisted',
+        'pyasn1==0.4.8',
     ],
     extras_require={
         'all': all_deps,
         # 'acu': acu_deps,
         # 'holography': holography_deps,
         'labjack': labjack_deps,
         'magpie': magpie_deps,
```

### Comparing `socs-0.4.2/socs/Lakeshore/Lakeshore240.py` & `socs-0.4.3rc1/socs/Lakeshore/Lakeshore240.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/Lakeshore/Lakeshore336.py` & `socs-0.4.3rc1/socs/Lakeshore/Lakeshore336.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/Lakeshore/Lakeshore370.py` & `socs-0.4.3rc1/socs/Lakeshore/Lakeshore370.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/Lakeshore/Lakeshore372.py` & `socs-0.4.3rc1/socs/Lakeshore/Lakeshore372.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/Lakeshore/Lakeshore425.py` & `socs-0.4.3rc1/socs/Lakeshore/Lakeshore425.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/acu/agent.py` & `socs-0.4.3rc1/socs/agents/acu/agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,68 @@
 import argparse
+import random
 import struct
 import time
 from enum import Enum
 
 import numpy as np
 import soaculib as aculib
 import soaculib.status_keys as status_keys
 import twisted.web.client as tclient
+import yaml
 from autobahn.twisted.util import sleep as dsleep
 from ocs import ocs_agent, site_config
 from ocs.ocs_twisted import TimeoutLock
 from soaculib.twisted_backend import TwistedHttpBackend
 from twisted.internet import protocol, reactor
 from twisted.internet.defer import DeferredList, inlineCallbacks
 
-import socs.agents.acu.drivers as sh
+from socs.agents.acu import drivers as sh
+from socs.agents.acu import exercisor
 
 #: The number of free ProgramTrack positions, when stack is empty.
 FULL_STACK = 10000
 
 
 class ACUAgent:
     """
     Agent to acquire data from an ACU and control telescope pointing with the
     ACU.
 
     Parameters:
         acu_config (str):
             The configuration for the ACU, as referenced in aculib.configs.
             Default value is 'guess'.
-
+        exercise_plan (str):
+            The full path to a scan config file describing motions to cycle
+            through on the ACU.  If this is None, the associated process and
+            feed will not be registered.
     """
 
-    def __init__(self, agent, acu_config='guess'):
+    def __init__(self, agent, acu_config='guess', exercise_plan=None):
         # Separate locks for exclusive access to az/el, and boresight motions.
         self.azel_lock = TimeoutLock()
         self.boresight_lock = TimeoutLock()
 
+        self.acu_config_name = acu_config
         self.acu_config = aculib.guess_config(acu_config)
         self.sleeptime = self.acu_config['motion_waittime']
         self.udp = self.acu_config['streams']['main']
         self.udp_schema = aculib.get_stream_schema(self.udp['schema'])
         self.udp_ext = self.acu_config['streams']['ext']
         self.acu8100 = self.acu_config['status']['status_name']
 
         # There may or may not be a special 3rd axis dataset that
         # needs to be probed.
         self.acu3rdaxis = self.acu_config['status'].get('3rdaxis_name')
         self.monitor_fields = status_keys.status_fields[self.acu_config['platform']]['status_fields']
         self.motion_limits = self.acu_config['motion_limits']
 
+        self.exercise_plan = exercise_plan
+
         self.log = agent.log
 
         # self.data provides a place to reference data from the monitors.
         # 'status' is populated by the monitor operation
         # 'broadcast' is populated by the udp_monitor operation
 
         self.data = {'status': {'summary': {},
@@ -156,14 +165,26 @@
         agent.register_task('stop_and_clear',
                             self.stop_and_clear,
                             blocking=False)
         agent.register_task('clear_faults',
                             self.clear_faults,
                             blocking=False)
 
+        # Automatic exercise program...
+        if exercise_plan:
+            agent.register_process(
+                'exercise', self.exercise, self._simple_process_stop)
+            # Use longer default frame length ... very low volume feed.
+            self.agent.register_feed('activity',
+                                     record=True,
+                                     buffer_time=0,
+                                     agg_params={
+                                         'frame_length': 600,
+                                     })
+
     @inlineCallbacks
     def _simple_task_abort(self, session, params):
         # Trigger a task abort by updating state to "stopping"
         yield session.set_status('stopping')
 
     @inlineCallbacks
     def _simple_process_stop(self, session, params):
@@ -221,34 +242,49 @@
               "3rd axis Mode": "Stop",
               "3rd axis commanded position": 77,
               "3rd axis current position": 77,
               "3rd axis computer disabled": "No Fault",
               ...
             },
             "StatusResponseRate": 19.237531827325963,
-            "PlatformType": "satp"
+            "PlatformType": "satp",
+            "connected": True,
           }
 
         In the case of an SATP, the Status3rdAxis is not populated
         (the Boresight info can be found in StatusDetailed).  In the
         case of the LAT, the corotator info is queried separately and
         stored under Status3rdAxis.
 
         """
 
         session.set_status('running')
-        version = yield self.acu_read.http.Version()
-        self.log.info(version)
 
         # Note that session.data will get scanned, to assign data to
         # feed blocks.  Items in session.data that are themselves
         # dicts will parsed; but items (such as PlatformType and
         # StatusResponseRate) which are simple strings or floats will
         # be ignored for feed assignment.
-        session.data = {'PlatformType': self.acu_config['platform']}
+        session.data = {'PlatformType': self.acu_config['platform'],
+                        'connected': False}
+
+        last_complaint = 0
+        while True:
+            try:
+                version = yield self.acu_read.http.Version()
+                break
+            except Exception as e:
+                if time.time() - last_complaint > 3600:
+                    errormsg = {'aculib_error_message': str(e)}
+                    self.log.error(str(e))
+                    self.log.error('monitor process failed to query version! Will keep trying.')
+                    last_complaint = time.time()
+                yield dsleep(10)
+        self.log.info(version)
+        session.data['connected'] = True
 
         # Numbering as per ICD.
         mode_key = {
             'Stop': 0,
             'Preset': 1,
             'ProgramTrack': 2,
             'Rate': 3,
@@ -343,25 +379,29 @@
 
             try:
                 j = yield self.acu_read.http.Values(self.acu8100)
                 if self.acu3rdaxis:
                     j2 = yield self.acu_read.http.Values(self.acu3rdaxis)
                 else:
                     j2 = {}
-                session.data.update({'StatusDetailed': j, 'Status3rdAxis': j2})
+                session.data.update({'StatusDetailed': j, 'Status3rdAxis': j2,
+                                     'connected': True})
                 n_ok += 1
+                last_complaint = 0
             except Exception as e:
-                # Need more error handling here...
-                errormsg = {'aculib_error_message': str(e)}
-                self.log.error(str(e))
-                acu_error = {'timestamp': time.time(),
-                             'block_name': 'ACU_error',
-                             'data': errormsg
-                             }
-                self.agent.publish_to_feed('acu_error', acu_error)
+                if now - last_complaint > 3600:
+                    errormsg = {'aculib_error_message': str(e)}
+                    self.log.error(str(e))
+                    acu_error = {'timestamp': time.time(),
+                                 'block_name': 'ACU_error',
+                                 'data': errormsg
+                                 }
+                    self.agent.publish_to_feed('acu_error', acu_error)
+                    last_complaint = time.time()
+                    session.data['connected'] = False
                 yield dsleep(1)
                 continue
             for k, v in session.data.items():
                 if isinstance(v, dict):
                     for (key, value) in v.items():
                         for category in self.monitor_fields:
                             if key in self.monitor_fields[category]:
@@ -501,58 +541,68 @@
             prev_checkdata = {'ctime': self.data['status']['summary']['ctime'],
                               'Azimuth_mode': self.data['status']['summary']['Azimuth_mode'],
                               'Elevation_mode': self.data['status']['summary']['Elevation_mode'],
                               'Boresight_mode': self.data['status']['summary']['Boresight_mode'],
                               }
         return True, 'Acquisition exited cleanly.'
 
+    @ocs_agent.param('auto_enable', type=bool, default=True)
     @inlineCallbacks
     def broadcast(self, session, params):
-        """broadcast()
+        """broadcast(auto_enable=True)
 
         **Process** - Read UDP data from the port specified by
         self.acu_config, decode it, and publish to HK feeds.  Full
         resolution (200 Hz) data are written to feed "acu_udp_stream"
         while 1 Hz decimated are written to "acu_broadcast_influx".
         The 1 Hz decimated output are also stored in session.data.
 
-        The session.data looks like this (this is for a SATP running
-        with servo details in the UDP output)::
+        Args:
+          auto_enable (bool): If True, the Process will try to
+            configure and (re-)enable the UDP stream if at any point
+            the stream seems to drop out.
 
-          {
-            "Time": 1679499948.8234625,
-            "Corrected_Azimuth": -20.00112176010607,
-            "Corrected_Elevation": 50.011521050839434,
-            "Corrected_Boresight": 29.998428712246067,
-            "Raw_Azimuth": -20.00112176010607,
-            "Raw_Elevation": 50.011521050839434,
-            "Raw_Boresight": 29.998428712246067,
-            "Azimuth_Current_1": -0.000384521484375,
-            "Azimuth_Current_2": -0.0008331298828125,
-            "Elevation_Current_1": 0.003397979736328125,
-            "Boresight_Current_1": -0.000483856201171875,
-            "Boresight_Current_2": -0.000105743408203125,
-            "Azimuth_Vel_1": -0.000002288818359375,
-            "Azimuth_Vel_2": 0,
-            "Az_Vel_Act": -0.0000011444091796875,
-            "Az_Vel_Des": 0,
-            "Az_Vffw": 0,
-            "Az_Pos_Des": -20.00112176010607,
-            "Az_Pos_Err": 0
-          }
+        Notes:
+          The session.data looks like this (this is for a SATP running
+          with servo details in the UDP output)::
+
+            {
+              "Time": 1679499948.8234625,
+              "Corrected_Azimuth": -20.00112176010607,
+              "Corrected_Elevation": 50.011521050839434,
+              "Corrected_Boresight": 29.998428712246067,
+              "Raw_Azimuth": -20.00112176010607,
+              "Raw_Elevation": 50.011521050839434,
+              "Raw_Boresight": 29.998428712246067,
+              "Azimuth_Current_1": -0.000384521484375,
+              "Azimuth_Current_2": -0.0008331298828125,
+              "Elevation_Current_1": 0.003397979736328125,
+              "Boresight_Current_1": -0.000483856201171875,
+              "Boresight_Current_2": -0.000105743408203125,
+              "Azimuth_Vel_1": -0.000002288818359375,
+              "Azimuth_Vel_2": 0,
+              "Az_Vel_Act": -0.0000011444091796875,
+              "Az_Vel_Des": 0,
+              "Az_Vffw": 0,
+              "Az_Pos_Des": -20.00112176010607,
+              "Az_Pos_Err": 0
+            }
 
         """
         session.set_status('running')
         FMT = self.udp_schema['format']
         FMT_LEN = struct.calcsize(FMT)
         UDP_PORT = self.udp['port']
         udp_data = []
         fields = self.udp_schema['fields']
         session.data = {}
 
+        # BroadcastStreamControl instance.
+        stream = self.acu_control.streams['main']
+
         class MonitorUDP(protocol.DatagramProtocol):
             def datagramReceived(self, data, src_addr):
                 host, port = src_addr
                 offset = 0
                 while len(data) - offset >= FMT_LEN:
                     d = struct.unpack(FMT, data[offset:offset + FMT_LEN])
                     udp_data.append(d)
@@ -600,18 +650,28 @@
                                         }
                 self.agent.publish_to_feed('acu_broadcast_influx', acu_broadcast_influx, from_reactor=True)
                 sd = {}
                 for ky in influx_means:
                     sd[ky.split('_bcast_influx')[0]] = influx_means[ky]
                 session.data.update(sd)
             else:
+                # Consider logging an outage, attempting reconfig.
                 if active and now - last_packet_time > 3:
                     self.log.info('No UDP packets are being received.')
                     active = False
+                    next_reconfig = time.time()
+                if not active and params['auto_enable'] and next_reconfig <= time.time():
+                    self.log.info('Requesting UDP stream enable.')
+                    try:
+                        cfg, raw = yield stream.safe_enable()
+                    except Exception as err:
+                        self.log.info('Exception while trying to enable stream: {err}', err=err)
+                    next_reconfig += 60
                 yield dsleep(1)
+
             yield dsleep(0.005)
 
         handler.stopListening()
         return True, 'Acquisition exited cleanly.'
 
     @inlineCallbacks
     def _check_daq_streams(self, stream):
@@ -1355,29 +1415,152 @@
             # Yes, sometimes you have to wait a very long time ...
             yield dsleep(10)
             yield self.acu_control.http.Command('DataSets.CmdTimePositionTransfer',
                                                 'Clear Stack')
 
         return True, 'Track ended cleanly'
 
+    @ocs_agent.param('starting_index', type=int, default=0)
+    def exercise(self, session, params):
+        """exercise(starting_index=0)
+
+        **Process** - Run telescope platform through some pre-defined motions.
+
+        For historical reasons, this does not command agent functions
+        internally, but rather instantiates a *client* and calls the
+        agent as though it were an external entity.
+
+        """
+        # Load the exercise plan.
+        plans = yaml.safe_load(open(self.exercise_plan, 'rb'))
+        super_plan = exercisor.get_plan(plans[self.acu_config_name])
+
+        session.data = {
+            'timestamp': time.time(),
+            'iterations': 0,
+            'attempts': 0,
+            'errors': 0,
+        }
+        session.set_status('running')
+
+        def _publish_activity(activity):
+            msg = {
+                'block_name': 'A',
+                'timestamp': time.time(),
+                'data': {'activity': activity},
+            }
+            self.agent.publish_to_feed('activity', msg)
+
+        def _publish_error(delta_error=1):
+            session.data['errors'] += delta_error
+            msg = {
+                'block_name': 'B',
+                'timestamp': time.time(),
+                'data': {'error_count': session.data['errors']}
+            }
+            self.agent.publish_to_feed('activity', msg)
+
+        def _exit_now(ok, msg):
+            _publish_activity('idle')
+            self.agent.feeds['activity'].flush_buffer()
+            return ok, msg
+
+        _publish_activity('idle')
+        _publish_error(0)
+
+        target_instance_id = self.agent.agent_address.split('.')[-1]
+        exercisor.set_client(target_instance_id)
+        settings = super_plan.get('settings', {})
+
+        plan_idx = 0
+        plan_t = None
+
+        for plan in super_plan['steps']:
+            plan['iter'] = iter(plan['driver'])
+
+        while session.status in ['running']:
+            time.sleep(1)
+            session.data['timestamp'] = time.time()
+            session.data['iterations'] += 1
+
+            # Fault maintenance
+            faults = exercisor.get_faults()
+            if faults['safe_lock']:
+                self.log.info('SAFE lock detected, exiting')
+                return _exit_now(False, 'Exiting on SAFE lock.')
+
+            if faults['local_mode']:
+                self.log.info('LOCAL mode detected, exiting')
+                return _exit_now(False, 'Exiting on LOCAL mode.')
+
+            if faults['az_summary']:
+                if session.data['attempts'] > 5:
+                    self.log.info('Too many az summary faults, exiting.')
+                    return _exit_now(False, 'Too many az summary faults.')
+                session.data['attempts'] += 1
+                self.log.info('az summary fault -- trying to clear.')
+                exercisor.clear_faults()
+                time.sleep(10)
+                continue
+
+            session.data['attempts'] = 0
+
+            # Plan execution
+            active_plan = super_plan['steps'][plan_idx]
+            if plan_t is None:
+                plan_t = time.time()
+
+            now = time.time()
+            if now - plan_t > active_plan['duration']:
+                plan_idx = (plan_idx + 1) % len(super_plan['steps'])
+                plan_t = None
+                continue
+
+            if settings.get('use_boresight'):
+                bore_target = random.choice(settings['boresight_opts'])
+                self.log.info(f'Setting boresight={bore_target}...')
+                _publish_activity('boresight')
+                exercisor.set_boresight(bore_target)
+
+            plan, info = next(active_plan['iter'])
+
+            self.log.info(f'Launching next scan. plan={plan}')
+
+            _publish_activity(active_plan['driver'].code)
+            ok = None
+            if 'targets' in plan:
+                exercisor.steps(**plan)
+            else:
+                exercisor.scan(**plan)
+            _publish_activity('idle')
+
+            if ok is None:
+                self.log.info('Scan completed without error.')
+            else:
+                self.log.info(f'Scan exited with error: {ok}')
+                _publish_error()
+
+        return _exit_now(True, "Stopped run process")
+
 
 def add_agent_args(parser_in=None):
     if parser_in is None:
         parser_in = argparse.ArgumentParser()
     pgroup = parser_in.add_argument_group('Agent Options')
-    pgroup.add_argument("--acu_config")
+    pgroup.add_argument("--acu-config")
+    pgroup.add_argument("--exercise-plan")
     return parser_in
 
 
 def main(args=None):
     parser = add_agent_args()
     args = site_config.parse_args(agent_class='ACUAgent',
                                   parser=parser,
                                   args=args)
     agent, runner = ocs_agent.init_site_agent(args)
-    _ = ACUAgent(agent, args.acu_config)
+    _ = ACUAgent(agent, args.acu_config, args.exercise_plan)
 
     runner.run(agent, auto_reconnect=True)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `socs-0.4.2/socs/agents/acu/drivers.py` & `socs-0.4.3rc1/socs/agents/acu/drivers.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/bluefors/agent.py` & `socs-0.4.3rc1/socs/agents/bluefors/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/cryomech_cpa/agent.py` & `socs-0.4.3rc1/socs/agents/cryomech_cpa/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/fts_aerotech/agent.py` & `socs-0.4.3rc1/socs/agents/fts_aerotech/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/holo_fpga/agent.py` & `socs-0.4.3rc1/socs/agents/holo_fpga/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/holo_synth/agent.py` & `socs-0.4.3rc1/socs/agents/holo_synth/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/hwp_encoder/agent.py` & `socs-0.4.3rc1/socs/agents/hwp_encoder/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/hwp_picoscope/agent.py` & `socs-0.4.3rc1/socs/agents/hwp_picoscope/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/hwp_picoscope/drivers/class_ps3000a.py` & `socs-0.4.3rc1/socs/agents/hwp_picoscope/drivers/class_ps3000a.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/hwp_rotation/agent.py` & `socs-0.4.3rc1/socs/agents/hwp_pid/agent.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,47 @@
 import argparse
 import time
 
 from ocs import ocs_agent, site_config
 from ocs.ocs_twisted import TimeoutLock
 from twisted.internet import reactor
 
-import socs.agents.hwp_rotation.drivers.pid_controller as pd
-from socs.common.pmx import PMX, Command
+import socs.agents.hwp_pid.drivers.pid_controller as pd
 
 
-class RotationAgent:
-    """Agent to control the rotation speed of the CHWP
+class HWPPIDAgent:
+    """Agent to PID control the rotation speed of the CHWP
 
     Args:
-        kikusui_ip (str): IP address for the Kikusui power supply
-        kikusui_port (str): Port for the Kikusui power supply
-        pid_ip (str): IP address for the PID controller
-        pid_port (str): Port for the PID controller
-        pid_verbosity (str): Verbosity of PID controller output
+        ip (str): IP address for the PID controller
+        port (str): Port for the PID controller
+        verbosity (str): Verbosity of PID controller output
 
     """
 
-    def __init__(self, agent, kikusui_ip, kikusui_port, pid_ip, pid_port, pid_verbosity):
+    def __init__(self, agent, ip, port, verbosity):
         self.agent = agent
         self.log = agent.log
         self.lock = TimeoutLock()
         self._initialized = False
         self.take_data = False
-        self.kikusui_ip = kikusui_ip
-        self.kikusui_port = int(kikusui_port)
-        self.pid_ip = pid_ip
-        self.pid_port = pid_port
-        self._pid_verbosity = pid_verbosity > 0
-        self.cmd = None  # Command object for PSU commanding
-        self.pid = None  # PID object for pid controller commanding
+        self.ip = ip
+        self.port = port
+        self._verbosity = verbosity > 0
 
         agg_params = {'frame_length': 60}
         self.agent.register_feed(
-            'hwprotation', record=True, agg_params=agg_params)
+            'hwppid', record=True, agg_params=agg_params)
 
     @ocs_agent.param('auto_acquire', default=False, type=bool)
     @ocs_agent.param('force', default=False, type=bool)
     def init_connection(self, session, params):
         """init_connection(auto_acquire=False, force=False)
 
-        **Task** - Initialize connection to Kikusui Power Supply and PID
+        **Task** - Initialize connection to PID
         Controller.
 
         Parameters:
             auto_acquire (bool, optional): Default is False. Starts data
                 acquisition after initialization if True.
             force (bool, optional): Force initialization, even if already
                 initialized. Defaults to False.
@@ -61,39 +54,29 @@
         with self.lock.acquire_timeout(0, job='init_connection') as acquired:
             if not acquired:
                 self.log.warn(
                     'Could not run init_connection because {} is already running'.format(self.lock.job))
                 return False, 'Could not acquire lock'
 
             try:
-                pmx = PMX(tcp_ip=self.kikusui_ip,
-                          tcp_port=self.kikusui_port, timeout=0.5)
-                self.cmd = Command(pmx)
-                self.log.info('Connected to Kikusui power supply')
-            except ConnectionRefusedError:
-                self.log.error('Could not establish connection to Kikusui power supply')
-                reactor.callFromThread(reactor.stop)
-                return False, 'Unable to connect to Kikusui PSU'
-
-            try:
-                self.pid = pd.PID(pid_ip=self.pid_ip, pid_port=self.pid_port,
-                                  verb=self._pid_verbosity)
+                self.pid = pd.PID(ip=self.ip, port=self.port,
+                                  verb=self._verbosity)
                 self.log.info('Connected to PID controller')
             except BrokenPipeError:
                 self.log.error('Could not establish connection to PID controller')
                 reactor.callFromThread(reactor.stop)
                 return False, 'Unable to connect to PID controller'
 
         self._initialized = True
 
-        # Start 'iv_acq' Process if requested
+        # Start 'acq' Process if requested
         if params['auto_acquire']:
-            self.agent.start('iv_acq')
+            self.agent.start('acq')
 
-        return True, 'Connection to PSU and PID controller established'
+        return True, 'Connection to PID controller established'
 
     def tune_stop(self, session, params):
         """tune_stop()
 
         **Task** - Reverse the drive direction of the PID controller and
         optimize the PID parameters for deceleration.
 
@@ -186,14 +169,31 @@
                     'Could not get freq because {} is already running'.format(self.lock.job))
                 return False, 'Could not acquire lock'
 
             freq = self.pid.get_freq()
 
         return True, 'Current frequency = {}'.format(freq)
 
+    def get_target(self, session, params):
+        """get_target()
+
+        **Task** - Return the target HWP frequency of the PID
+        controller.
+
+        """
+        with self.lock.acquire_timeout(3, job='get_target') as acquired:
+            if not acquired:
+                self.log.warn(
+                    'Could not get freq because {} is already running'.format(self.lock.job))
+                return False, 'Could not acquire lock'
+
+            freq = self.pid.get_target()
+
+        return True, 'Target frequency = {}'.format(freq)
+
     def get_direction(self, session, params):
         """get_direction()
 
         **Task** - Return the current HWP tune direction as seen by the PID
         controller.
 
         """
@@ -201,15 +201,15 @@
             if not acquired:
                 self.log.warn(
                     'Could not get freq because {} is already running'.format(self.lock.job))
                 return False, 'Could not acquire lock'
 
             direction = self.pid.get_direction()
 
-        return True, 'Current Direction = {}'.format(['Forward', 'Reverse'][direction])
+        return True, 'Current direction = {}'.format(['Forward', 'Reverse'][direction])
 
     @ocs_agent.param('direction', type=str, default='0', choices=['0', '1'])
     def set_direction(self, session, params):
         """set_direction(direction='0')
 
         **Task** - Set the HWP rotation direction.
 
@@ -248,148 +248,31 @@
                     'Could not set scale because {} is already running'.format(self.lock.job))
                 return False, 'Could not acquire lock'
 
             self.pid.set_scale(params['slope'], params['offset'])
 
         return True, 'Set scale'
 
-    def set_on(self, session, params):
-        """set_on()
-
-        **Task** - Turn on the Kikusui drive voltage.
-
-        """
-        with self.lock.acquire_timeout(3, job='set_on') as acquired:
-            if not acquired:
-                self.log.warn(
-                    'Could not set on because {} is already running'.format(self.lock.job))
-                return False, 'Could not acquire lock'
-
-            time.sleep(1)
-            self.cmd.user_input('on')
-
-        return True, 'Set Kikusui on'
-
-    def set_off(self, session, params):
-        """set_off()
-
-        **Task** - Turn off the Kikusui drive voltage.
-
-        """
-        with self.lock.acquire_timeout(3, job='set_off') as acquired:
-            if not acquired:
-                self.log.warn(
-                    'Could not set off because {} is already running'.format(self.lock.job))
-                return False, 'Could not acquire lock'
+    def acq(self, session, params):
+        """acq()
 
-            time.sleep(1)
-            self.cmd.user_input('off')
-
-        return True, 'Set Kikusui off'
-
-    @ocs_agent.param('volt', default=0, type=float, check=lambda x: 0 <= x <= 35)
-    def set_v(self, session, params):
-        """set_v(volt=0)
-
-        **Task** - Set the Kikusui drive voltage.
-
-        Parameters:
-            volt (float): Kikusui set voltage
-
-        """
-        with self.lock.acquire_timeout(3, job='set_v') as acquired:
-            if not acquired:
-                self.log.warn(
-                    'Could not set v because {} is already running'.format(self.lock.job))
-                return False, 'Could not acquire lock'
-
-            time.sleep(1)
-            self.cmd.user_input('V {}'.format(params['volt']))
-
-        return True, 'Set Kikusui voltage to {} V'.format(params['volt'])
-
-    @ocs_agent.param('volt', default=32., type=float, check=lambda x: 0. <= x <= 35.)
-    def set_v_lim(self, session, params):
-        """set_v_lim(volt=32)
-
-        **Task** - Set the Kikusui drive voltage limit.
-
-        Parameters:
-            volt (float): Kikusui limit voltage
-
-        """
-        with self.lock.acquire_timeout(3, job='set_v_lim') as acquired:
-            if not acquired:
-                self.log.warn(
-                    'Could not set v lim because {} is already running'.format(self.lock.job))
-                return False, 'Could not acquire lock'
-
-            time.sleep(1)
-            print(params['volt'])
-            self.cmd.user_input('VL {}'.format(params['volt']))
-
-        return True, 'Set Kikusui voltage limit to {} V'.format(params['volt'])
-
-    def use_ext(self, session, params):
-        """use_ext()
-
-        **Task** - Set the Kikusui to use an external voltage control. Doing so
-        enables PID control.
-
-        """
-        with self.lock.acquire_timeout(3, job='use_ext') as acquired:
-            if not acquired:
-                self.log.warn(
-                    'Could not use external voltage because {} is already running'.format(self.lock.job))
-                return False, 'Could not acquire lock'
-
-            time.sleep(1)
-            self.cmd.user_input('U')
-
-        return True, 'Set Kikusui voltage to PID control'
-
-    def ign_ext(self, session, params):
-        """ign_ext()
-
-        **Task** - Set the Kiksui to ignore external voltage control. Doing so
-        disables the PID and switches to direct control.
-
-        """
-        with self.lock.acquire_timeout(3, job='ign_ext') as acquired:
-            if not acquired:
-                self.log.warn(
-                    'Could not ignore external voltage because {} is already running'.format(self.lock.job))
-                return False, 'Could not acquire lock'
-
-            time.sleep(1)
-            self.cmd.user_input('I')
-
-        return True, 'Set Kikusui voltage to direct control'
-
-    @ocs_agent.param('test_mode', default=False, type=bool)
-    def iv_acq(self, session, params):
-        """iv_acq(test_mode=False)
-
-        **Process** - Start Kikusui data acquisition.
-
-        Parameters:
-            test_mode (bool, optional): Run the Process loop only once.
-                This is meant only for testing. Default is False.
+        **Process** - Start PID data acquisition.
 
         Notes:
             The most recent data collected is stored in the session data in the
             structure::
 
                 >>> response.session['data']
-                {'kikusui_volt': 0,
-                 'kikusui_curr': 0,
+                {'current_freq': 0,
+                 'target_freq': 0,
+                 'direction': 1,
                  'last_updated': 1649085992.719602}
 
         """
-        with self.lock.acquire_timeout(timeout=0, job='iv_acq') as acquired:
+        with self.lock.acquire_timeout(timeout=0, job='acq') as acquired:
             if not acquired:
                 self.log.warn('Could not start iv acq because {} is already running'
                               .format(self.lock.job))
                 return False, 'Could not acquire lock'
 
             session.set_status('running')
             last_release = time.time()
@@ -401,39 +284,39 @@
                     last_release = time.time()
                     if not self.lock.release_and_acquire(timeout=10):
                         self.log.warn(f"Failed to re-acquire sampling lock, "
                                       f"currently held by {self.lock.job}.")
                         continue
 
                 data = {'timestamp': time.time(),
-                        'block_name': 'HWPKikusui_IV', 'data': {}}
+                        'block_name': 'HWPPID', 'data': {}}
 
-                v_msg, v_val = self.cmd.user_input('V?')
-                i_msg, i_val = self.cmd.user_input('C?')
+                current_freq = self.pid.get_freq()
+                target_freq = self.pid.get_target()
+                direction = self.pid.get_direction()
 
-                data['data']['kikusui_volt'] = v_val
-                data['data']['kikusui_curr'] = i_val
+                data['data']['current_freq'] = current_freq
+                data['data']['target_freq'] = target_freq
+                data['data']['direction'] = direction
 
-                self.agent.publish_to_feed('hwprotation', data)
+                self.agent.publish_to_feed('hwppid', data)
 
-                session.data = {'kikusui_volt': v_val,
-                                'kikusui_curr': i_val,
+                session.data = {'current_freq': current_freq,
+                                'target_freq': target_freq,
+                                'direction': direction,
                                 'last_updated': time.time()}
 
                 time.sleep(1)
 
-                if params['test_mode']:
-                    break
-
-        self.agent.feeds['hwprotation'].flush_buffer()
+        self.agent.feeds['hwppid'].flush_buffer()
         return True, 'Acqusition exited cleanly'
 
-    def _stop_iv_acq(self, session, params):
+    def _stop_acq(self, session, params):
         """
-        Stop iv_acq process.
+        Stop acq process.
         """
         if self.take_data:
             self.take_data = False
             return True, 'requested to stop taking data'
 
         return False, 'acq is not currently running'
 
@@ -444,61 +327,52 @@
     baised on this function
     """
     if parser is None:
         parser = argparse.ArgumentParser()
 
     # Add options specific to this agent
     pgroup = parser.add_argument_group('Agent Options')
-    pgroup.add_argument('--kikusui-ip')
-    pgroup.add_argument('--kikusui-port')
-    pgroup.add_argument('--pid-ip')
-    pgroup.add_argument('--pid-port')
+    pgroup.add_argument('--ip')
+    pgroup.add_argument('--port')
     pgroup.add_argument('--verbose', '-v', action='count', default=0,
                         help='PID Controller verbosity level.')
-    pgroup.add_argument('--mode', type=str, default='iv_acq',
-                        choices=['idle', 'init', 'iv_acq'],
+    pgroup.add_argument('--mode', type=str, default='acq',
+                        choices=['init', 'acq'],
                         help="Starting operation for the Agent.")
     return parser
 
 
 def main(args=None):
     parser = make_parser()
-    args = site_config.parse_args(agent_class='RotationAgent',
+    args = site_config.parse_args(agent_class='HWPPIDAgent',
                                   parser=parser,
                                   args=args)
 
     init_params = False
     if args.mode == 'init':
         init_params = {'auto_acquire': False}
-    elif args.mode == 'iv_acq':
+    elif args.mode == 'acq':
         init_params = {'auto_acquire': True}
 
     agent, runner = ocs_agent.init_site_agent(args)
-    rotation_agent = RotationAgent(agent, kikusui_ip=args.kikusui_ip,
-                                   kikusui_port=args.kikusui_port,
-                                   pid_ip=args.pid_ip,
-                                   pid_port=args.pid_port,
-                                   pid_verbosity=args.verbose)
-    agent.register_process('iv_acq', rotation_agent.iv_acq,
-                           rotation_agent._stop_iv_acq)
-    agent.register_task('init_connection', rotation_agent.init_connection,
+    hwppid_agent = HWPPIDAgent(agent, ip=args.ip,
+                               port=args.port,
+                               verbosity=args.verbose)
+    agent.register_task('init_connection', hwppid_agent.init_connection,
                         startup=init_params)
-    agent.register_task('tune_stop', rotation_agent.tune_stop)
-    agent.register_task('tune_freq', rotation_agent.tune_freq)
-    agent.register_task('declare_freq', rotation_agent.declare_freq)
-    agent.register_task('set_pid', rotation_agent.set_pid)
-    agent.register_task('get_freq', rotation_agent.get_freq)
-    agent.register_task('get_direction', rotation_agent.get_direction)
-    agent.register_task('set_direction', rotation_agent.set_direction)
-    agent.register_task('set_scale', rotation_agent.set_scale)
-    agent.register_task('set_on', rotation_agent.set_on)
-    agent.register_task('set_off', rotation_agent.set_off)
-    agent.register_task('set_v', rotation_agent.set_v)
-    agent.register_task('set_v_lim', rotation_agent.set_v_lim)
-    agent.register_task('use_ext', rotation_agent.use_ext)
-    agent.register_task('ign_ext', rotation_agent.ign_ext)
+    agent.register_process('acq', hwppid_agent.acq,
+                           hwppid_agent._stop_acq)
+    agent.register_task('tune_stop', hwppid_agent.tune_stop)
+    agent.register_task('tune_freq', hwppid_agent.tune_freq)
+    agent.register_task('declare_freq', hwppid_agent.declare_freq)
+    agent.register_task('set_pid', hwppid_agent.set_pid)
+    agent.register_task('get_freq', hwppid_agent.get_freq)
+    agent.register_task('get_target', hwppid_agent.get_target)
+    agent.register_task('get_direction', hwppid_agent.get_direction)
+    agent.register_task('set_direction', hwppid_agent.set_direction)
+    agent.register_task('set_scale', hwppid_agent.set_scale)
 
     runner.run(agent, auto_reconnect=True)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `socs-0.4.2/socs/agents/hwp_rotation/drivers/pid_controller.py` & `socs-0.4.3rc1/socs/agents/hwp_pid/drivers/pid_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,34 +2,35 @@
 import time
 
 
 class PID:
     """Class to communicate with the Omega CNi16D54-EIT PID controller.
 
     Args:
-        pid_ip (str): IP address for the controller.
-        pid_port (int): Port number for the socket connection.
+        ip (str): IP address for the controller.
+        port (int): Port number for the socket connection.
         verb (bool): Verbose output setting. Defaults to False.
 
     Attributes:
         verb (bool): Verbose output setting.
         hex_freq (str): Currently declared rotation frequency in hexadecimal.
         direction (int): Current direction of the HWP. 0 for forward and 1 for
             backwards.
         conn (socket.socket): Socket object with open connection to the PID
             controller.
 
     """
 
-    def __init__(self, pid_ip, pid_port, verb=False):
+    def __init__(self, ip, port, verb=False):
         self.verb = verb
         self.hex_freq = '00000'
         self.direction = None
+        self.target = 0
         # Need to setup connection before setting direction
-        self.conn = self._establish_connection(pid_ip, int(pid_port))
+        self.conn = self._establish_connection(ip, int(port))
         self.set_direction('0')
 
     @staticmethod
     def _establish_connection(ip, port, timeout=5):
         """Connect to PID controller.
 
         Args:
@@ -128,17 +129,18 @@
             print('Starting Stop')
 
         responses = []
         responses.append(self.send_message("*W0C83"))
         responses.append(self.send_message("*W01400000"))
         responses.append(self.send_message("*R01"))
         responses.append(self.send_message("*Z02"))
+        messages = self.return_messages(responses)
         if self.verb:
             print(responses)
-            print(self.return_messages(responses))
+            print(messages)
 
         stop_params = [0.2, 0, 0]
         self.set_pid(stop_params)
 
     def tune_freq(self):
         """Set the setpoint to currently declared frequency.
 
@@ -149,17 +151,18 @@
             print('Starting Tune')
 
         responses = []
         responses.append(self.send_message("*W0C81"))
         responses.append(self.send_message(f"*W014{self.hex_freq}"))
         responses.append(self.send_message("*R01"))
         responses.append(self.send_message("*Z02"))
+        messages = self.return_messages(responses)
         if self.verb:
             print(responses)
-            print(self.return_messages(responses))
+            print(messages)
 
         tune_params = [0.2, 63, 0]
         self.set_pid(tune_params)
 
     def get_freq(self):
         """Returns the current frequency of the CHWP."""
         if self.verb:
@@ -169,33 +172,46 @@
         responses.append(self.send_message("*X01"))
         if self.verb:
             print(responses)
 
         freq = self.return_messages(responses)[0]
         return freq
 
+    def get_target(self):
+        """Returns the target frequency of the CHWP."""
+        if self.verb:
+            print('Finding target CHWP Frequency')
+
+        responses = []
+        responses.append(self.send_message("*R01"))
+        target = self.return_messages(responses)[0]
+        if self.verb:
+            print(responses)
+            print('Setpoint = ' + str(target))
+
+        return target
+
     def get_direction(self):
         """Get the current rotation direction.
 
         Returns:
             int: 0 for forward and 1 for backwards
 
         """
         if self.verb:
             print('Finding CHWP Direction')
 
         responses = []
         responses.append(self.send_message("*R02"))
-
         direction = self.return_messages(responses)[0]
-        if direction == 1:
-            print('Direction = Reverse')
-        elif direction == 0:
-            print('Direction = Forward')
-        self.direction = direction
+        if self.verb:
+            if direction == 1:
+                print('Direction = Reverse')
+            elif direction == 0:
+                print('Direction = Forward')
 
         return direction
 
     def set_pid(self, params):
         """Sets the PID parameters of the controller."""
         if self.verb:
             print('Setting PID Params')
@@ -296,23 +312,23 @@
                 pass
 
         return output_array
 
     @staticmethod
     def _decode_read(string):
         read_type = string[1:3]
+        # Decode target
         if read_type == '01':
-            return 'Setpoint = ' + str(int(string[4:], 16) / 1000.)
+            target = float(int(string[4:], 16) / 1000.)
+            return target
         # Decode direction
         if read_type == '02':
             if int(string[4:], 16) / 1000. > 2.5:
-                print('Direction = Reverse')
                 return 1
             else:
-                print('Direction = Forward')
                 return 0
         else:
             return 'Unrecognized Read'
 
     @staticmethod
     def _decode_write(string):
         write_type = string[1:]
```

### Comparing `socs-0.4.2/socs/agents/ibootbar/agent.py` & `socs-0.4.3rc1/socs/agents/ups/agent.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,24 +33,24 @@
     ----------
     get_result : pysnmp.smi.rfc1902.ObjectType
         Result from a pysnmp GET command.
 
     Returns
     -------
     field_name : str
-        Field name for an OID, i.e. 'outletStatus_1'
+        Field name for an OID, i.e. 'upsIdentModel'
     oid_value : int or str
         Associated value for the OID. Returns None if not an int or str
     oid_description : str
         String description of the OID value.
     """
     # OID from SNMP GET
     oid = get_result[0].prettyPrint()
-    # Makes something like 'IBOOTPDU-MIB::outletStatus.1'
-    # look like 'outletStatus_1'
+    # Makes something like 'UPS-MIB::upsIdentModel.0'
+    # look like 'upsIdentModel_0'
     field_name = oid.split("::")[1].replace('.', '_')
 
     # Grab OID value, mostly these are integers
     oid_value = get_result[1]._value
     oid_description = get_result[1].prettyPrint()
 
     # Decode string values
@@ -60,377 +60,393 @@
     # I don't expect any other types at the moment, but just in case.
     if not isinstance(oid_value, (int, bytes, str)):
         oid_value = None
 
     return field_name, oid_value, oid_description
 
 
-def _build_message(get_result, names, time):
+def _build_message(get_result, time):
     """Build the message for publication on an OCS Feed.
 
     Parameters
     ----------
     get_result : pysnmp.smi.rfc1902.ObjectType
         Result from a pysnmp GET command.
-    names : list
-        List of strings for outlet names
     time : float
         Timestamp for when the SNMP GET was issued.
 
     Returns
     -------
     message : dict
         OCS Feed formatted message for publishing
     """
     message = {
-        'block_name': 'ibootbar',
+        'block_name': 'ups',
         'timestamp': time,
         'data': {}
     }
 
     for item in get_result:
         field_name, oid_value, oid_description = _extract_oid_field_and_value(item)
 
         if oid_value is None:
             continue
 
         message['data'][field_name] = oid_value
-        message['data'][field_name + "_name"] = names[int(field_name[-1])]
         message['data'][field_name + "_description"] = oid_description
 
     return message
 
 
-def update_cache(get_result, names, timestamp):
+def update_cache(get_result, timestamp):
     """Update the OID Value Cache.
 
     The OID Value Cache is used to store each unique OID and will be passed to
     session.data
 
     The cache consists of a dictionary, with the unique OIDs as keys, and
-    another dictionary as the value. Each of these nested dictionaries contains
-    the OID values, name, and description (decoded string). An example for a
-    single OID, with connection status and timestamp information::
-
-        {"outletStatus_0": {"status": 1,
-                            "name": Outlet-1,
-                            "description": "on"},
-         "ibootbar_connection": {"last_attempt": 1598543359.6326838,
-                                 "connected": True},
-         "timestamp": 1656085022.680916}
+    another dictionary as the value. Each of these nested dictionaries contains the
+    OID values, name, and description (decoded string). An example for a single OID::
+
+        {"upsBatteryStatus":
+            {"status": 2,
+                "description": "batteryNormal"}}
+
+    Additionally there is connection status and timestamp information under::
+
+        {"ups_connection":
+            {"last_attempt": 1598543359.6326838,
+            "connected": True}
+        {"timestamp": 1656085022.680916}
 
     Parameters
     ----------
     get_result : pysnmp.smi.rfc1902.ObjectType
         Result from a pysnmp GET command.
-    names : list
-        List of strings for outlet names
     timestamp : float
         Timestamp for when the SNMP GET was issued.
     """
     oid_cache = {}
-    try:
-        for item in get_result:
-            field_name, oid_value, oid_description = _extract_oid_field_and_value(item)
-            if oid_value is None:
-                continue
+    # Return disconnected if SNMP response is empty
+    if get_result is None:
+        oid_cache['ups_connection'] = {'last_attempt': time.time(),
+                                       'connected': False}
+        return oid_cache
 
-            # Update OID Cache for session.data
-            oid_cache[field_name] = {"status": oid_value}
-            oid_cache[field_name]["name"] = names[int(field_name[-1])]
-            oid_cache[field_name]["description"] = oid_description
-            oid_cache['ibootbar_connection'] = {'last_attempt': time.time(),
-                                                'connected': True}
-            oid_cache['timestamp'] = timestamp
-    # This is a TypeError due to nothing coming back from the yield,
-    # so get_result is None here and can't be iterated.
-    except TypeError:
-        oid_cache['ibootbar_connection'] = {'last_attempt': time.time(),
-                                            'connected': False}
-        raise ConnectionError('No SNMP response. Check your connection.')
+    for item in get_result:
+        field_name, oid_value, oid_description = _extract_oid_field_and_value(item)
+        if oid_value is None:
+            continue
+
+        # Update OID Cache for session.data
+        oid_cache[field_name] = {"status": oid_value}
+        oid_cache[field_name]["description"] = oid_description
+        oid_cache['ups_connection'] = {'last_attempt': time.time(),
+                                       'connected': True}
+        oid_cache['timestamp'] = timestamp
 
     return oid_cache
 
 
-class ibootbarAgent:
-    """Monitor the ibootbar system via SNMP.
+class UPSAgent:
+    """Monitor the UPS system via SNMP.
 
     Parameters
     ----------
     agent : OCSAgent
         OCSAgent object which forms this Agent
     address : str
-        Address of the ibootbar.
+        Address of the UPS.
     port : int
         SNMP port to issue GETs to, default to 161.
     version : int
-        SNMP version for communication (1, 2, or 3), defaults to 2.
+        SNMP version for communication (1, 2, or 3), defaults to 3.
 
     Attributes
     ----------
     agent : OCSAgent
         OCSAgent object which forms this Agent
     is_streaming : bool
         Tracks whether or not the agent is actively issuing SNMP GET commands
-        to the ibootbar. Setting to false stops sending commands.
+        to the UPS. Setting to false stops sending commands.
     log : txaio.tx.Logger
         txaio logger object, created by the OCSAgent
     """
 
-    def __init__(self, agent, address, port=161, version=2):
+    def __init__(self, agent, address, port=161, version=1):
         self.agent = agent
         self.is_streaming = False
         self.log = self.agent.log
         self.lock = TimeoutLock()
 
         self.log.info(f'Using SNMP version {version}.')
         self.version = version
         self.snmp = SNMPTwister(address, port)
 
         self.lastGet = 0
 
         agg_params = {
             'frame_length': 10 * 60  # [sec]
         }
-        self.agent.register_feed('ibootbar',
+        self.agent.register_feed('ups',
                                  record=True,
                                  agg_params=agg_params,
                                  buffer_time=0)
 
     @ocs_agent.param('test_mode', default=False, type=bool)
     @inlineCallbacks
     def acq(self, session, params=None):
         """acq()
 
-        **Process** - Fetch values from the ibootbar via SNMP.
+        **Process** - Fetch values from the UPS via SNMP.
+
+        Parameters
+        ----------
+        test_mode : bool, optional
+            Run the Process loop only once. Meant only for testing.
+            Default is False.
 
         Notes
         -----
         The most recent data collected is stored in session.data in the
         structure::
 
             >>> response.session['data']
-            {'outletStatus_0':
-                {'status': 1,
-                 'name': 'Outlet-1',
-                 'description': 'on'},
-             'outletStatus_1':
+            {'upsIdentManufacturer':
+                {'description': 'Falcon'},
+            'upsIdentModel':
+                {'description': 'SSG3KRM-2'},
+            'upsBatteryStatus':
+                {'status': 2,
+                 'description': 'batteryNormal'},
+            'upsSecondsOnBattery':
                 {'status': 0,
-                 'name': 'Outlet-2',
-                 'description': 'off'},
-             ...
-             'ibootbar_connection':
+                 'description': 0},
+            'upsEstimatedMinutesRemaining':
+                {'status': 60,
+                 'description': 60},
+            'upsEstimatedChargeRemaining':
+                {'status': 100,
+                 'description': 100},
+            'upsBatteryVoltage':
+                {'status': 120,
+                 'description': 120},
+            'upsBatteryCurrent':
+                {'status': 10,
+                 'description': 10},
+            'upsBatteryTemperature':
+                {'status': 30,
+                 'description': 30},
+            'upsOutputSource':
+                {'status': 3,
+                 'description': normal},
+            'upsOutputVoltage':
+                {'status': 120,
+                 'description': 120},
+            'upsOutputCurrent':
+                {'status': 10,
+                 'description': 10},
+            'upsOutputPower':
+                {'status': 120,
+                 'description': 120},
+            'upsOutputPercentLoad':
+                {'status': 25,
+                 'description': 25}
+            'upsInputVoltage':
+                {'status': 120,
+                 'description': 120},
+            'upsInputCurrent':
+                {'status': 10,
+                 'description': 10},
+            'upsInputTruePower':
+                {'status': 120,
+                 'description': 120},
+            'ups_connection':
                 {'last_attempt': 1656085022.680916,
                  'connected': True},
-             'timestamp': 1656085022.680916}
+            'timestamp': 1656085022.680916}
+
+        Some relevant options and units for the above OIDs::
+
+            upsBatteryStatus::
+                Options:: unknown(1),
+                          batteryNormal(2),
+                          batteryLow(3),
+                          batteryDepleted(4)
+            upsSecondsOnBattery::
+                Note:: Zero shall be returned if the unit is not on
+                       battery power.
+            upsEstimatedChargeRemaining::
+                Units:: percentage
+            upsBatteryVoltage::
+                Units:: 0.1 Volt DC
+            upsBatteryCurrent::
+                Units:: 0.1 Amp DC
+            upsBatteryTemperature::
+                Units:: degrees Centigrade
+            upsOutputSource::
+                Options:: other(1),
+                          none(2),
+                          normal(3),
+                          bypass(4),
+                          battery(5),
+                          booster(6),
+                          reducer(7)
+            upsOutputVoltage::
+                Units:: RMS Volts
+            upsOutputCurrent::
+                Units:: 0.1 RMS Amp
+            upsOutputPower::
+                Units:: Watts
+            upsInputVoltage::
+                Units:: RMS Volts
+            upsInputCurrent::
+                Units:: 0.1 RMS Amp
+            upsInputTruePower::
+                Units:: Watts
         """
-        # Set initial default outlet names
-        names = ['Outlet-1', 'Outlet-2', 'Outlet-3', 'Outlet-4',
-                 'Outlet-5', 'Outlet-6', 'Outlet-7', 'Outlet-8']
 
+        session.set_status('running')
         self.is_streaming = True
         while self.is_streaming:
             yield dsleep(1)
             read_time = time.time()
 
             # Check if 60 seconds has passed before getting status
             if (read_time - self.lastGet) < 60:
                 continue
 
             get_list = []
-            name_list = []
-            names = []
 
-            # Create the lists of OIDs to send get commands
-            for i in range(8):
-                get_list.append(('IBOOTPDU-MIB', 'outletStatus', i))
-                name_list.append(('IBOOTPDU-MIB', 'outletName', i))
+            # Create the list of OIDs to send get commands
+            oids = ['upsIdentManufacturer',
+                    'upsIdentModel',
+                    'upsBatteryStatus',
+                    'upsSecondsOnBattery',
+                    'upsEstimatedMinutesRemaining',
+                    'upsEstimatedChargeRemaining',
+                    'upsBatteryVoltage',
+                    'upsBatteryCurrent',
+                    'upsBatteryTemperature',
+                    'upsOutputSource']
+
+            for oid in oids:
+                get_list.append(('UPS-MIB', oid, 0))
+
+            # Append input OIDs to GET list
+            input_oids = ['upsInputVoltage',
+                          'upsInputCurrent',
+                          'upsInputTruePower']
+
+            # Use number of input lines used to append correct number of input OIDs
+            num_lines = [('UPS-MIB', 'upsInputNumLines', 0)]
+            num_res = yield self.snmp.get(num_lines, self.version)
+            if num_res is not None:
+                inputs = num_res[0][1]._value
+                for i in range(inputs):
+                    for oid in input_oids:
+                        get_list.append(('UPS-MIB', oid, i + 1))
+
+            # Append output OIDs to GET list
+            output_oids = ['upsOutputVoltage',
+                           'upsOutputCurrent',
+                           'upsOutputPower',
+                           'upsOutputPercentLoad']
+
+            # Use number of output lines used to append correct number of output OIDs
+            num_lines = [('UPS-MIB', 'upsOutputNumLines', 0)]
+            num_res = yield self.snmp.get(num_lines, self.version)
+            if num_res is not None:
+                outputs = num_res[0][1]._value
+                for i in range(outputs):
+                    for oid in output_oids:
+                        get_list.append(('UPS-MIB', oid, i + 1))
 
             # Issue SNMP GET command
             get_result = yield self.snmp.get(get_list, self.version)
-            name_result = yield self.snmp.get(name_list, self.version)
-
-            # If device gets disconnected, name_result is None
-            if name_result is not None:
-                for item in name_result:
-                    names.append(item[1].prettyPrint())
 
-            # Do not publish if ibootbar connection has dropped
+            # Do not publish if UPS connection has dropped
             try:
                 # Update session.data
-                oid_cache = update_cache(get_result, names, read_time)
-                session.data = oid_cache
+                session.data = update_cache(get_result, read_time)
                 self.log.debug("{data}", data=session.data)
-                self.lastGet = time.time()
 
+                if get_result is None:
+                    raise ConnectionError('No SNMP response. Check your connection.')
+
+                self.lastGet = time.time()
                 # Publish to feed
-                message = _build_message(get_result, names, read_time)
+                message = _build_message(get_result, read_time)
                 self.log.debug("{msg}", msg=message)
-                session.app.publish_to_feed('ibootbar', message)
+                session.app.publish_to_feed('ups', message)
             except ConnectionError as e:
                 self.log.error(f'{e}')
                 yield dsleep(1)
                 self.log.info('Trying to reconnect.')
 
             if params['test_mode']:
                 break
 
         return True, "Finished Recording"
 
     def _stop_acq(self, session, params=None):
         """_stop_acq()
         **Task** - Stop task associated with acq process.
         """
-        self.is_streaming = False
-        return True, "Stopping Recording"
-
-    @ocs_agent.param('outlet', choices=[1, 2, 3, 4, 5, 6, 7, 8])
-    @ocs_agent.param('state', choices=['on', 'off'])
-    @inlineCallbacks
-    def set_outlet(self, session, params=None):
-        """set_outlet(outlet, state)
-
-        **Task** - Set a particular outlet to on/off.
-
-        Parameters
-        ----------
-        outlet : int
-            Index of outlet to set
-        state : str
-            State to set outlet to
-        """
-        with self.lock.acquire_timeout(3, job='set_outlet') as acquired:
-            if not acquired:
-                return False, "Could not acquire lock"
-            # Convert given state parameter to integer
-            if params['state'] == 'on':
-                state = 1
-            else:
-                state = 0
-
-            # Issue SNMP SET command to given outlet
-            outlet = [('IBOOTPDU-MIB', 'outletControl', params['outlet'] - 1)]
-            setcmd = yield self.snmp.set(outlet, self.version, state)
-            self.log.info('{}'.format(setcmd))
-
-        # Force SNMP GET status commands by rewinding the lastGet time by 60 seconds
-        self.lastGet = self.lastGet - 60
-
-        return True, 'Set outlet {} to {}'.\
-            format(params['outlet'] - 1, params['state'])
-
-    @ocs_agent.param('outlet', choices=[1, 2, 3, 4, 5, 6, 7, 8])
-    @ocs_agent.param('cycle_time', default=10, type=int)
-    @inlineCallbacks
-    def cycle_outlet(self, session, params=None):
-        """cycle_outlet(outlet, cycle_time=10)
-
-        **Task** - Cycle a particular outlet for given amount of seconds.
-
-        Parameters
-        ----------
-        outlet : int
-            Index of outlet to cycle
-        cycle_time : int
-            The amount of seconds to cycle an outlet. Default is 10 seconds.
-        """
-        with self.lock.acquire_timeout(3, job='cycle_outlet') as acquired:
-            if not acquired:
-                return False, "Could not acquire lock"
-            # Issue SNMP SET command for cycle time
-            set_cycle = [('IBOOTPDU-MIB', 'outletCycleTime', params['outlet'] - 1)]
-            setcmd1 = yield self.snmp.set(set_cycle, self.version, params['cycle_time'])
-            self.log.info('{}'.format(setcmd1))
-
-            # Issue SNMP SET command to given outlet
-            outlet = [('IBOOTPDU-MIB', 'outletControl', params['outlet'] - 1)]
-            setcmd2 = yield self.snmp.set(outlet, self.version, 2)
-            self.log.info('{}'.format(setcmd2))
-            self.log.info('Cycling outlet {} for {} seconds'.
-                          format(params['outlet'] - 1, params['cycle_time']))
-
-        # Force SNMP GET status commands throughout the cycle time
-        for i in range(params['cycle_time'] + 1):
-            self.lastGet = self.lastGet - 60
-            yield dsleep(1)
-
-        return True, 'Cycled outlet {} for {} seconds'.\
-            format(params['outlet'] - 1, params['cycle_time'])
-
-    @ocs_agent.param('_')
-    @inlineCallbacks
-    def set_initial_state(self, session, params=None):
-        """set_initial_state()
-
-        **Task** - Set outlets to their initial states.
-
-        Performs a software reboot. The outlets are then set to their
-        respective initial states. This takes about 30 seconds.
-        """
-        with self.lock.acquire_timeout(3, job='reboot') as acquired:
-            if not acquired:
-                return False, "Could not acquire lock"
-            # Send SNMP SET command to set rebootSystem to True
-            reboot = [('IBOOTPDU-MIB', 'rebootSystem', 0)]
-            setcmd = yield self.snmp.set(reboot, self.version, 1)
-            self.log.info('{}'.format(setcmd))
-
-        # Force SNMP GET status commands
-        self.lastGet = self.lastGet - 60
-
-        return True, 'Rebooting. Outlets will be set to their initial states.'
+        if self.is_streaming:
+            session.set_status('stopping')
+            self.is_streaming = False
+            return True, "Stopping Recording"
+        else:
+            return False, "Acq is not currently running"
 
 
 def add_agent_args(parser=None):
     """
     Build the argument parser for the Agent. Allows sphinx to automatically
     build documentation based on this function.
     """
     if parser is None:
         parser = argparse.ArgumentParser()
 
     pgroup = parser.add_argument_group("Agent Options")
     pgroup.add_argument("--address", help="Address to listen to.")
     pgroup.add_argument("--port", default=161,
                         help="Port to listen on.")
-    pgroup.add_argument("--snmp-version", default='2', choices=['1', '2', '3'],
+    pgroup.add_argument("--snmp-version", default='1', choices=['1', '2', '3'],
                         help="SNMP version for communication. Must match "
-                             + "configuration on the ibootbar.")
+                             + "configuration on the UPS.")
     pgroup.add_argument("--mode", choices=['acq', 'test'])
 
     return parser
 
 
 def main(args=None):
     # Start logging
     txaio.start_logging(level=os.environ.get("LOGLEVEL", "info"))
 
     parser = add_agent_args()
-    args = site_config.parse_args(agent_class='ibootbarAgent',
+    args = site_config.parse_args(agent_class='UPSAgent',
                                   parser=parser,
                                   args=args)
 
     if args.mode == 'acq':
         init_params = True
     elif args.mode == 'test':
         init_params = False
 
     agent, runner = ocs_agent.init_site_agent(args)
-    p = ibootbarAgent(agent,
-                      address=args.address,
-                      port=int(args.port),
-                      version=int(args.snmp_version))
+    p = UPSAgent(agent,
+                 address=args.address,
+                 port=int(args.port),
+                 version=int(args.snmp_version))
 
     agent.register_process("acq",
                            p.acq,
                            p._stop_acq,
                            startup=init_params, blocking=False)
 
-    agent.register_task("set_outlet", p.set_outlet, blocking=False)
-    agent.register_task("cycle_outlet", p.cycle_outlet, blocking=False)
-    agent.register_task("set_initial_state", p.set_initial_state, blocking=False)
-
     runner.run(agent, auto_reconnect=True)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `socs-0.4.2/socs/agents/labjack/agent.py` & `socs-0.4.3rc1/socs/agents/labjack/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,17 @@
         for the thermistor model, serial number 10K4D25.
         """
         # LJTick voltage to resistance conversion
         R = (2.5 - v_array) * 10000 / v_array
 
         # Import the Ohms to Celsius cal curve and apply cubic
         # interpolation to find the temperature
-        reader = csv.reader(open('cal_curves/GA10K4D25_cal_curve.txt'),
+        cal_curves = os.path.join(os.path.dirname(__file__),
+                                  'cal_curves/GA10K4D25_cal_curve.txt')
+        reader = csv.reader(open(cal_curves),
                             delimiter=' ')
         lists = [el for el in [row for row in reader]]
         T_cal = np.array([float(RT[0]) for RT in lists[1:]])
         R_cal = np.array([float(RT[1]) for RT in lists[1:]])
         T_cal = np.flip(T_cal)
         R_cal = np.flip(R_cal)
         try:
```

### Comparing `socs-0.4.2/socs/agents/labjack/cal_curves/GA10K4D25_cal_curve.txt` & `socs-0.4.3rc1/socs/agents/labjack/cal_curves/GA10K4D25_cal_curve.txt`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/lakeshore240/agent.py` & `socs-0.4.3rc1/socs/agents/lakeshore240/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/lakeshore336/agent.py` & `socs-0.4.3rc1/socs/agents/lakeshore336/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/lakeshore370/agent.py` & `socs-0.4.3rc1/socs/agents/lakeshore370/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/lakeshore372/agent.py` & `socs-0.4.3rc1/socs/agents/lakeshore372/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/lakeshore425/agent.py` & `socs-0.4.3rc1/socs/agents/lakeshore425/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/magpie/agent.py` & `socs-0.4.3rc1/socs/agents/magpie/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/meinberg_m1000/agent.py` & `socs-0.4.3rc1/socs/agents/meinberg_m1000/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/ocs_plugin_so.py` & `socs-0.4.3rc1/socs/agents/ocs_plugin_so.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,33 +11,35 @@
 root = os.path.abspath(os.path.split(__file__)[0])
 
 for n, f in [
         ('ACUAgent', 'acu/agent.py'),
         ('BlueforsAgent', 'bluefors/agent.py'),
         ('CrateAgent', 'smurf_crate_monitor/agent.py'),
         ('CryomechCPAAgent', 'cryomech_cpa/agent.py'),
+        ('FlowmeterAgent', 'ifm_sbn246_flowmeter/agent.py'),
         ('FPGAAgent', 'holo_fpga/agent.py'),
         ('FTSAerotechAgent', 'fts_aerotech/agent.py'),
         ('HWPBBBAgent', 'hwp_encoder/agent.py'),
         ('HWPPicoscopeAgent', 'hwp_picoscope/agent.py'),
+        ('HWPPIDAgent', 'hwp_pid/agent.py'),
+        ('HWPPMXAgent', 'hwp_pmx/agent.py'),
         ('ibootbarAgent', 'ibootbar/agent.py'),
         ('LabJackAgent', 'labjack/agent.py'),
         ('Lakeshore240Agent', 'lakeshore240/agent.py'),
         ('Lakeshore336Agent', 'lakeshore336/agent.py'),
         ('Lakeshore370Agent', 'lakeshore370/agent.py'),
         ('Lakeshore372Agent', 'lakeshore372/agent.py'),
         ('Lakeshore425Agent', 'lakeshore425/agent.py'),
         ('LATRtXYStageAgent', 'xy_stage/agent.py'),
         ('MagpieAgent', 'magpie/agent.py'),
         ('MeinbergM1000Agent', 'meinberg_m1000/agent.py'),
         ('PfeifferAgent', 'pfeiffer_tpg366/agent.py'),
         ('PfeifferTC400Agent', 'pfeiffer_tc400/agent.py'),
         ('PysmurfController', 'pysmurf_controller/agent.py'),
         ('PysmurfMonitor', 'pysmurf_monitor/agent.py'),
-        ('RotationAgent', 'hwp_rotation/agent.py'),
         ('ScpiPsuAgent', 'scpi_psu/agent.py'),
         ('SmurfFileEmulator', 'smurf_file_emulator/agent.py'),
         ('SmurfStreamSimulator', 'smurf_stream_simulator/agent.py'),
         ('SmurfTimingCardAgent', 'smurf_timing_card/agent.py'),
         ('SupRsync', 'suprsync/agent.py'),
         ('SynaccessAgent', 'synacc/agent.py'),
         ('SynthAgent', 'holo_synth/agent.py'),
```

### Comparing `socs-0.4.2/socs/agents/pfeiffer_tc400/agent.py` & `socs-0.4.3rc1/socs/agents/pfeiffer_tc400/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/pfeiffer_tc400/drivers.py` & `socs-0.4.3rc1/socs/agents/pfeiffer_tc400/drivers.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/pfeiffer_tpg366/agent.py` & `socs-0.4.3rc1/socs/agents/pfeiffer_tpg366/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/pysmurf_controller/agent.py` & `socs-0.4.3rc1/socs/agents/pysmurf_controller/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -327,14 +327,17 @@
     def _stop_check_state(self, session, params):
         """Stopper for check state process"""
         session.set_status('stopping')
 
     @ocs_agent.param("duration", default=None, type=float)
     @ocs_agent.param('kwargs', default=None)
     @ocs_agent.param('load_tune', default=True, type=bool)
+    @ocs_agent.param('stream_type', default='obs', choices=['obs', 'oper'])
+    @ocs_agent.param('subtype', default=None)
+    @ocs_agent.param('tag', default=None)
     @ocs_agent.param('test_mode', default=False, type=bool)
     def stream(self, session, params):
         """stream(duration=None)
 
         **Process** - Stream smurf data. If a duration is specified, stream
         will end after that amount of time. If unspecified, the stream will run
         until the stop function is called.
@@ -346,28 +349,44 @@
             will leave stream open until stop function is called.
         kwargs : dict
             A dictionary containing additional keyword arguments to pass
             to sodetlib's ``stream_g3_on`` function
         load_tune : bool
             If true, will load a tune-file to the pysmurf object on
             instantiation.
+        stream_type : string, optional
+            Stream type. This can be either 'obs' or 'oper', and will be 'obs'
+            by default. The tags attached to the stream will be
+            ``<stream_type>,<subtype>,<tag>``.
+        subtype : string, optional
+            Operation subtype used tot tag the stream.
+        tag : string, optional
+            Tag (or comma-separated list of tags) to attach to the G3 stream.
+            This has precedence over the `tag` key in the kwargs dict.
 
         Notes
         ------
         The following data will be written to the session.data object::
 
             >> response.session['data']
             {
                 'stream_id': Stream-id for the slot,
                 'sid': Session-id for the streaming session,
             }
         """
         if params['kwargs'] is None:
             params['kwargs'] = {}
 
+        if params['stream_type']:
+            params['kwargs']['tag'] = params['stream_type']
+        if params['subtype'] is not None:
+            params['kwargs']['subtype'] = params['subtype']
+        if params['tag'] is not None:
+            params['kwargs']['tag'] = params['tag']
+
         with self.lock.acquire_timeout(0, job='stream') as acquired:
             if not acquired:
                 return False, f"Operation failed: {self.lock.job} is running."
 
             S, cfg = self._get_smurf_control(session=session,
                                              load_tune=params['load_tune'])
 
@@ -529,14 +548,15 @@
             success, summary = uxm_relock.uxm_relock(
                 S, cfg, bands=params['bands'], **params['kwargs']
             )
             return success, "Finished UXM Relock"
 
     @ocs_agent.param('duration', default=30., type=float)
     @ocs_agent.param('kwargs', default=None)
+    @ocs_agent.param('tag', default=None)
     def take_noise(self, session, params):
         """take_noise(duration=30., kwargs=None)
 
         **Task** - Takes a short timestream and calculates noise statistics.
         Median white noise level for each band will be stored in the session
         data. See the `sodetlib noise docs
         <https://simons1.princeton.edu/docs/sodetlib/noise.html>`_ for more
@@ -545,14 +565,18 @@
         Args
         -----
         duration : float
             Duration of timestream to take for noise calculation.
         kwargs : dict
             Dict containing additional keyword args to pass to the take_noise
             function.
+        tag : string, optional
+            Tag (or comma-separated list of tags) to attach to the G3 stream.
+            This has precedence over the `tag` key in the kwargs dict.
+
 
         Notes
         -------
         Median white noise levels for each band will be stored in the
         session.data object, for example::
 
             >> response.session['data']
@@ -561,38 +585,45 @@
                    'band_medians': List of median white noise for each band
                 }
             }
         """
         if params['kwargs'] is None:
             params['kwargs'] = {}
 
+        if params['tag'] is not None:
+            params['kwargs']['g3_tag'] = params['tag']
+
         with self.lock.acquire_timeout(0, job='take_noise') as acquired:
             if not acquired:
                 return False, f"Operation failed: {self.lock.job} is running."
 
             session.set_status('running')
             S, cfg = self._get_smurf_control(session=session)
             sdl.noise.take_noise(S, cfg, params['duration'], **params['kwargs'])
             return True, "Finished taking noise"
 
     @ocs_agent.param('kwargs', default=None)
+    @ocs_agent.param('tag', default=None)
     def take_bgmap(self, session, params):
         """take_bgmap(kwargs=None)
 
         **Task** - Takes a bias-group map. This will calculate the number of
         channels assigned to each bias group and put that into the session data
         object along with the filepath to the analyzed bias-step output. See
         the `bias steps docs page <https://simons1.princeton.edu/docs/sodetlib/operations/bias_steps.html>`_
         for more information on what additional keyword arguments can be
         passed.
 
         Args
         ----
         kwargs : dict
             Additional kwargs to pass to take_bgmap function.
+        tag : Optional[str]
+            String containing a tag or comma-separated list of tags to attach
+            to the g3 stream.
 
         Notes
         ------
         The filepath of the BiasStepAnalysis object and the number of channels
         assigned to each bias group will be written to the session.data
         object::
 
@@ -602,14 +633,17 @@
                 'filepath': /path/to/bias_step_file/on/smurf_server.npy,
             }
 
         """
         if params['kwargs'] is None:
             params['kwargs'] = {}
 
+        if params['tag'] is not None:
+            params['kwargs']['g3_tag'] = params['tag']
+
         with self.lock.acquire_timeout(0, job='take_bgmap') as acquired:
             if not acquired:
                 return False, f"Operation failed: {self.lock.job} is running."
 
             session.set_status('running')
             S, cfg = self._get_smurf_control(session=session)
 
@@ -626,28 +660,32 @@
             session.data = {
                 'nchans_per_bg': nchans_per_bg,
                 'filepath': bsa.filepath,
             }
             return True, "Finished taking bgmap"
 
     @ocs_agent.param('kwargs', default=None)
+    @ocs_agent.param('tag', default=None)
     def take_iv(self, session, params):
         """take_iv(kwargs=None)
 
         **Task** - Takes an IV. This will add the normal resistance array and
         channel info to the session data object along with the analyzed IV
         filepath. See the `sodetlib IV docs page
         <https://simons1.princeton.edu/docs/sodetlib/operations/iv.html>`_
         for more information on what additional keyword arguments can be passed
         in.
 
         Args
         ----
         kwargs : dict
             Additional kwargs to pass to the ``take_iv`` function.
+        tag : Optional[str]
+            String containing a tag or comma-separated list of tags to attach
+            to the g3 stream.
 
         Notes
         ------
         The following data will be written to the session.data object::
 
             >> response.session['data']
             {
@@ -657,14 +695,17 @@
                 'R_n': Normal resistance for each resonator
                 'filepath': Filepath of saved IVAnalysis object
             }
         """
         if params['kwargs'] is None:
             params['kwargs'] = {}
 
+        if params['tag'] is not None:
+            params['kwargs']['g3_tag'] = params['tag']
+
         with self.lock.acquire_timeout(0, job='take_iv') as acquired:
             if not acquired:
                 return False, f"Operation failed: {self.lock.job} is running."
 
             session.set_status('starting')
             S, cfg = self._get_smurf_control(session=session)
             iva = iv.take_iv(S, cfg, **params['kwargs'])
@@ -675,14 +716,15 @@
                 'R_n': iva.R_n.tolist(),
                 'filepath': iva.filepath,
             }
             return True, "Finished taking IV"
 
     @ocs_agent.param('kwargs', default=None)
     @ocs_agent.param('rfrac_range', default=(0.2, 0.9))
+    @ocs_agent.param('tag', default=None)
     def take_bias_steps(self, session, params):
         """take_bias_steps(kwargs=None, rfrac_range=(0.2, 0.9))
 
         **Task** - Takes bias_steps and saves the output filepath to the
         session data object. See the `sodetlib bias step docs page
         <https://simons1.princeton.edu/docs/sodetlib/operations/bias_steps.html>`_
         for more information on bias steps and what kwargs can be passed in.
@@ -690,14 +732,17 @@
         Args
         ----
         kwargs : dict
             Additional kwargs to pass to ``take_bais_steps`` function.
         rfrac_range : tuple
             Range of valid rfracs to check against when determining the number
             of good detectors.
+        tag : Optional[str]
+            String containing a tag or comma-separated list of tags to attach
+            to the g3 stream.
 
         Notes
         ------
         The following data will be written to the session.data object::
 
             >> response.session['data']
             {
@@ -714,14 +759,17 @@
 
             }
         """
 
         if params['kwargs'] is None:
             params['kwargs'] = {}
 
+        if params['tag'] is not None:
+            params['kwargs']['g3_tag'] = params['tag']
+
         with self.lock.acquire_timeout(0, job='bias_steps') as acquired:
             if not acquired:
                 return False, f"Operation failed: {self.lock.job} is running."
 
             session.set_status('starting')
             S, cfg = self._get_smurf_control(session=session)
             bsa = bias_steps.take_bias_steps(
```

### Comparing `socs-0.4.2/socs/agents/pysmurf_monitor/agent.py` & `socs-0.4.3rc1/socs/agents/pysmurf_monitor/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/scpi_psu/agent.py` & `socs-0.4.3rc1/socs/agents/scpi_psu/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/scpi_psu/drivers.py` & `socs-0.4.3rc1/socs/agents/scpi_psu/drivers.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/smurf_crate_monitor/agent.py` & `socs-0.4.3rc1/socs/agents/smurf_crate_monitor/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/smurf_file_emulator/agent.py` & `socs-0.4.3rc1/socs/agents/smurf_file_emulator/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -485,15 +485,16 @@
 
         # tracking setup
         action_time = time.time()
         fname = f"{int(time.time())}.dat"
         self._write_smurf_file(fname, action, action_time=action_time, prepend_ctime=False)
 
         # Short g3 stream
-        streamer = self._new_streamer(action=action, action_time=action_time)
+        streamer = self._new_streamer(action=action, action_time=action_time,
+                                      tag='oper,noise')
         now = time.time()
         streamer.stream_between(now, now + 30, wait=False)
         if session is not None:
             session.data['noise_file'] = streamer.file_list[0]
 
     @ocs_agent.param('sleep', default=True)
     def uxm_setup(self, session, params):
@@ -524,15 +525,16 @@
         """take_noise()
 
         **Task** - Takes a short noise timestream
         """
         action = 'take_noise'
         action_time = time.time()
 
-        streamer = self._new_streamer(action=action, action_time=action_time)
+        streamer = self._new_streamer(action=action, action_time=action_time,
+                                      tag='oper,noise')
         now = time.time()
         streamer.stream_between(now, now + 30, wait=False)
         session.data['noise_file'] = streamer.file_list[0]
         time.sleep(1)
         return True, "Took noise data"
 
     def uxm_relock(self, session, params=None):
@@ -552,15 +554,16 @@
 
         **Task** - Creates files generated associated with iv taking / analysis
         """
         action = 'take_iv'
         action_time = time.time()
         files = ['iv_analyze.npy', 'iv_bias_all.npy', 'iv_info.npy']
 
-        streamer = self._new_streamer(action=action, action_time=action_time)
+        streamer = self._new_streamer(action=action, action_time=action_time,
+                                      tag='oper,iv')
         now = time.time()
         streamer.stream_between(now, now + 5, wait=params['wait'])
 
         for f in files:
             self._write_smurf_file(f, action, action_time=action_time)
 
         return True, "Wrote IV files"
@@ -571,15 +574,16 @@
 
         **Task** - Creates files associated with taking bias steps
         """
         action = 'take_bias_steps'
         action_time = time.time()
         files = ['bias_step_analysis.npy']
 
-        streamer = self._new_streamer(action=action, action_time=action_time)
+        streamer = self._new_streamer(action=action, action_time=action_time,
+                                      tag='oper,bias_steps')
         now = time.time()
         streamer.stream_between(now, now + 5, wait=params['wait'])
 
         for f in files:
             self._write_smurf_file(f, action, action_time=action_time)
 
         return True, "Wrote Bias Step Files"
@@ -589,15 +593,16 @@
         """take_bgmap()
 
         **Task** - Creates files associated with taking a bias group mapping.
         """
         action = 'take_bgmap'
         action_time = time.time()
 
-        streamer = self._new_streamer(action=action, action_time=action_time)
+        streamer = self._new_streamer(action=action, action_time=action_time,
+                                      tag='oper,bgmap')
         now = time.time()
         streamer.stream_between(now, now + 5, wait=params['wait'])
 
         files = ['bg_map.npy', 'bias_step_analysis.npy']
         for f in files:
             self._write_smurf_file(f, action, action_time=action_time)
```

### Comparing `socs-0.4.2/socs/agents/smurf_file_emulator/status_sample.yaml` & `socs-0.4.3rc1/socs/agents/smurf_file_emulator/status_sample.yaml`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/smurf_stream_simulator/agent.py` & `socs-0.4.3rc1/socs/agents/smurf_stream_simulator/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/smurf_timing_card/agent.py` & `socs-0.4.3rc1/socs/agents/smurf_timing_card/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/suprsync/agent.py` & `socs-0.4.3rc1/socs/agents/suprsync/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/synacc/agent.py` & `socs-0.4.3rc1/socs/agents/synacc/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/tektronix3021c/agent.py` & `socs-0.4.3rc1/socs/agents/tektronix3021c/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/thorlabs_mc2000b/agent.py` & `socs-0.4.3rc1/socs/agents/thorlabs_mc2000b/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/ups/agent.py` & `socs-0.4.3rc1/socs/agents/ibootbar/agent.py`

 * *Files 27% similar despite different names*

```diff
@@ -33,24 +33,24 @@
     ----------
     get_result : pysnmp.smi.rfc1902.ObjectType
         Result from a pysnmp GET command.
 
     Returns
     -------
     field_name : str
-        Field name for an OID, i.e. 'upsIdentModel'
+        Field name for an OID, i.e. 'outletStatus_1'
     oid_value : int or str
         Associated value for the OID. Returns None if not an int or str
     oid_description : str
         String description of the OID value.
     """
     # OID from SNMP GET
     oid = get_result[0].prettyPrint()
-    # Makes something like 'UPS-MIB::upsIdentModel.0'
-    # look like 'upsIdentModel_0'
+    # Makes something like 'IBOOTPDU-MIB::outletStatus.1'
+    # look like 'outletStatus_1'
     field_name = oid.split("::")[1].replace('.', '_')
 
     # Grab OID value, mostly these are integers
     oid_value = get_result[1]._value
     oid_description = get_result[1].prettyPrint()
 
     # Decode string values
@@ -60,386 +60,447 @@
     # I don't expect any other types at the moment, but just in case.
     if not isinstance(oid_value, (int, bytes, str)):
         oid_value = None
 
     return field_name, oid_value, oid_description
 
 
-def _build_message(get_result, time):
+def _build_message(get_result, names, time):
     """Build the message for publication on an OCS Feed.
 
     Parameters
     ----------
     get_result : pysnmp.smi.rfc1902.ObjectType
         Result from a pysnmp GET command.
+    names : list
+        List of strings for outlet names
     time : float
         Timestamp for when the SNMP GET was issued.
 
     Returns
     -------
     message : dict
         OCS Feed formatted message for publishing
     """
     message = {
-        'block_name': 'ups',
+        'block_name': 'ibootbar',
         'timestamp': time,
         'data': {}
     }
 
     for item in get_result:
         field_name, oid_value, oid_description = _extract_oid_field_and_value(item)
 
         if oid_value is None:
             continue
 
         message['data'][field_name] = oid_value
+        message['data'][field_name + "_name"] = names[int(field_name[-1])]
         message['data'][field_name + "_description"] = oid_description
 
     return message
 
 
-def update_cache(get_result, timestamp):
+def update_cache(get_result, names, outlet_locked, timestamp):
     """Update the OID Value Cache.
 
     The OID Value Cache is used to store each unique OID and will be passed to
     session.data
 
     The cache consists of a dictionary, with the unique OIDs as keys, and
-    another dictionary as the value. Each of these nested dictionaries contains the
-    OID values, name, and description (decoded string). An example for a single OID::
-
-        {"upsBatteryStatus":
-            {"status": 2,
-                "description": "batteryNormal"}}
-
-    Additionally there is connection status and timestamp information under::
-
-        {"ups_connection":
-            {"last_attempt": 1598543359.6326838,
-            "connected": True}
-        {"timestamp": 1656085022.680916}
+    another dictionary as the value. Each of these nested dictionaries contains
+    the OID values, name, and description (decoded string). An example for a
+    single OID, with connection status and timestamp information::
+
+        {"outletStatus_0": {"status": 1,
+                            "name": Outlet-1,
+                            "description": "on"},
+         "ibootbar_connection": {"last_attempt": 1598543359.6326838,
+                                 "connected": True},
+         "timestamp": 1656085022.680916}
 
     Parameters
     ----------
     get_result : pysnmp.smi.rfc1902.ObjectType
         Result from a pysnmp GET command.
+    names : list
+        List of strings for outlet names
+    outlet_locked : list of bool
+        List of bool for outlets (1-8) that are locked
     timestamp : float
         Timestamp for when the SNMP GET was issued.
     """
     oid_cache = {}
-    try:
-        for item in get_result:
-            field_name, oid_value, oid_description = _extract_oid_field_and_value(item)
-            if oid_value is None:
-                continue
+    # Return disconnected if SNMP response is empty
+    if get_result is None:
+        oid_cache['ibootbar_connection'] = {'last_attempt': time.time(),
+                                            'connected': False}
+        return oid_cache
+
+    for item in get_result:
+        field_name, oid_value, oid_description = _extract_oid_field_and_value(item)
+        if oid_value is None:
+            continue
 
-            # Update OID Cache for session.data
-            oid_cache[field_name] = {"status": oid_value}
-            oid_cache[field_name]["description"] = oid_description
-            oid_cache['ups_connection'] = {'last_attempt': time.time(),
-                                           'connected': True}
-            oid_cache['timestamp'] = timestamp
-    # This is a TypeError due to nothing coming back from the yield,
-    # so get_result is None here and can't be iterated.
-    except TypeError:
-        oid_cache['ups_connection'] = {'last_attempt': time.time(),
-                                       'connected': False}
-        raise ConnectionError('No SNMP response. Check your connection.')
+        # Update OID Cache for session.data
+        oid_cache[field_name] = {"status": oid_value}
+        oid_cache[field_name]["name"] = names[int(field_name[-1])]
+        oid_cache[field_name]["locked"] = outlet_locked[int(field_name[-1])]
+        oid_cache[field_name]["description"] = oid_description
+        oid_cache['ibootbar_connection'] = {'last_attempt': time.time(),
+                                            'connected': True}
+        oid_cache['timestamp'] = timestamp
 
     return oid_cache
 
 
-class UPSAgent:
-    """Monitor the UPS system via SNMP.
+class ibootbarAgent:
+    """Monitor the ibootbar system via SNMP.
 
     Parameters
     ----------
     agent : OCSAgent
         OCSAgent object which forms this Agent
     address : str
-        Address of the UPS.
+        Address of the ibootbar.
     port : int
         SNMP port to issue GETs to, default to 161.
     version : int
-        SNMP version for communication (1, 2, or 3), defaults to 3.
+        SNMP version for communication (1, 2, or 3), defaults to 2.
+    lock_outlet : list of ints
+        List of outlets to lock on agent startup. Outlets are numbered 1-8.
 
     Attributes
     ----------
     agent : OCSAgent
         OCSAgent object which forms this Agent
     is_streaming : bool
         Tracks whether or not the agent is actively issuing SNMP GET commands
-        to the UPS. Setting to false stops sending commands.
+        to the ibootbar. Setting to false stops sending commands.
     log : txaio.tx.Logger
         txaio logger object, created by the OCSAgent
     """
 
-    def __init__(self, agent, address, port=161, version=1):
+    def __init__(self, agent, address, port=161, version=2, lock_outlet=None):
         self.agent = agent
         self.is_streaming = False
         self.log = self.agent.log
         self.lock = TimeoutLock()
 
+        # Initialize with locked outlets if given in args
+        self.outlet_locked = [False for i in range(8)]
+        if lock_outlet is not None:
+            for i in range(8):
+                if i + 1 in lock_outlet:
+                    self.outlet_locked[i] = True
+                else:
+                    self.outlet_locked[i] = False
+
         self.log.info(f'Using SNMP version {version}.')
         self.version = version
+        self.address = address
         self.snmp = SNMPTwister(address, port)
 
         self.lastGet = 0
+        self.sample_period = 60
 
         agg_params = {
             'frame_length': 10 * 60  # [sec]
         }
-        self.agent.register_feed('ups',
+        self.agent.register_feed('ibootbar',
                                  record=True,
                                  agg_params=agg_params,
                                  buffer_time=0)
 
     @ocs_agent.param('test_mode', default=False, type=bool)
     @inlineCallbacks
     def acq(self, session, params=None):
         """acq()
 
-        **Process** - Fetch values from the UPS via SNMP.
-
-        Parameters
-        ----------
-        test_mode : bool, optional
-            Run the Process loop only once. Meant only for testing.
-            Default is False.
+        **Process** - Fetch values from the ibootbar via SNMP.
 
         Notes
         -----
         The most recent data collected is stored in session.data in the
         structure::
 
             >>> response.session['data']
-            {'upsIdentManufacturer':
-                {'description': 'Falcon'},
-            'upsIdentModel':
-                {'description': 'SSG3KRM-2'},
-            'upsBatteryStatus':
-                {'status': 2,
-                 'description': 'batteryNormal'},
-            'upsSecondsOnBattery':
+            {'outletStatus_0':
+                {'status': 1,
+                 'name': 'Outlet-1',
+                 'description': 'on'},
+             'outletStatus_1':
                 {'status': 0,
-                 'description': 0},
-            'upsEstimatedMinutesRemaining':
-                {'status': 60,
-                 'description': 60},
-            'upsEstimatedChargeRemaining':
-                {'status': 100,
-                 'description': 100},
-            'upsBatteryVoltage':
-                {'status': 120,
-                 'description': 120},
-            'upsBatteryCurrent':
-                {'status': 10,
-                 'description': 10},
-            'upsBatteryTemperature':
-                {'status': 30,
-                 'description': 30},
-            'upsOutputSource':
-                {'status': 3,
-                 'description': normal},
-            'upsOutputVoltage':
-                {'status': 120,
-                 'description': 120},
-            'upsOutputCurrent':
-                {'status': 10,
-                 'description': 10},
-            'upsOutputPower':
-                {'status': 120,
-                 'description': 120},
-            'upsOutputPercentLoad':
-                {'status': 25,
-                 'description': 25}
-            'upsInputVoltage':
-                {'status': 120,
-                 'description': 120},
-            'upsInputCurrent':
-                {'status': 10,
-                 'description': 10},
-            'upsInputTruePower':
-                {'status': 120,
-                 'description': 120},
-            'ups_connection':
+                 'name': 'Outlet-2',
+                 'description': 'off'},
+             ...
+             'ibootbar_connection':
                 {'last_attempt': 1656085022.680916,
                  'connected': True},
-            'timestamp': 1656085022.680916}
-
-        Some relevant options and units for the above OIDs::
-
-            upsBatteryStatus::
-                Options:: unknown(1),
-                          batteryNormal(2),
-                          batteryLow(3),
-                          batteryDepleted(4)
-            upsSecondsOnBattery::
-                Note:: Zero shall be returned if the unit is not on
-                       battery power.
-            upsEstimatedChargeRemaining::
-                Units:: percentage
-            upsBatteryVoltage::
-                Units:: 0.1 Volt DC
-            upsBatteryCurrent::
-                Units:: 0.1 Amp DC
-            upsBatteryTemperature::
-                Units:: degrees Centigrade
-            upsOutputSource::
-                Options:: other(1),
-                          none(2),
-                          normal(3),
-                          bypass(4),
-                          battery(5),
-                          booster(6),
-                          reducer(7)
-            upsOutputVoltage::
-                Units:: RMS Volts
-            upsOutputCurrent::
-                Units:: 0.1 RMS Amp
-            upsOutputPower::
-                Units:: Watts
-            upsInputVoltage::
-                Units:: RMS Volts
-            upsInputCurrent::
-                Units:: 0.1 RMS Amp
-            upsInputTruePower::
-                Units:: Watts
+             'timestamp': 1656085022.680916,
+             'address': '10.10.10.50'}
         """
+        # Set initial default outlet names
+        # Note outlets are numbered 1-8 physically on ibootbars, OIDs are numbered 0-7
+        names = ['Outlet-1', 'Outlet-2', 'Outlet-3', 'Outlet-4',
+                 'Outlet-5', 'Outlet-6', 'Outlet-7', 'Outlet-8']
 
+        session.set_status('running')
         self.is_streaming = True
         while self.is_streaming:
             yield dsleep(1)
             read_time = time.time()
 
-            # Check if 60 seconds has passed before getting status
-            if (read_time - self.lastGet) < 60:
+            # Check if sample period has passed before getting status
+            if (read_time - self.lastGet) < self.sample_period:
                 continue
 
             get_list = []
+            name_list = []
+            names = []
 
-            # Create the list of OIDs to send get commands
-            oids = ['upsIdentManufacturer',
-                    'upsIdentModel',
-                    'upsBatteryStatus',
-                    'upsSecondsOnBattery',
-                    'upsEstimatedMinutesRemaining',
-                    'upsEstimatedChargeRemaining',
-                    'upsBatteryVoltage',
-                    'upsBatteryCurrent',
-                    'upsBatteryTemperature',
-                    'upsOutputSource']
-
-            for oid in oids:
-                get_list.append(('UPS-MIB', oid, 0))
-
-            # Append input OIDs to GET list
-            input_oids = ['upsInputVoltage',
-                          'upsInputCurrent',
-                          'upsInputTruePower']
-
-            # Use number of input lines used to append correct number of input OIDs
-            num_lines = [('UPS-MIB', 'upsInputNumLines', 0)]
-            num_res = yield self.snmp.get(num_lines, self.version)
-            if num_res is not None:
-                inputs = num_res[0][1]._value
-                for i in range(inputs):
-                    for oid in input_oids:
-                        get_list.append(('UPS-MIB', oid, i + 1))
-
-            # Append output OIDs to GET list
-            output_oids = ['upsOutputVoltage',
-                           'upsOutputCurrent',
-                           'upsOutputPower',
-                           'upsOutputPercentLoad']
-
-            # Use number of output lines used to append correct number of output OIDs
-            num_lines = [('UPS-MIB', 'upsOutputNumLines', 0)]
-            num_res = yield self.snmp.get(num_lines, self.version)
-            if num_res is not None:
-                outputs = num_res[0][1]._value
-                for i in range(outputs):
-                    for oid in output_oids:
-                        get_list.append(('UPS-MIB', oid, i + 1))
+            # Create the lists of OIDs to send get commands
+            for i in range(8):
+                get_list.append(('IBOOTPDU-MIB', 'outletStatus', i))
+                name_list.append(('IBOOTPDU-MIB', 'outletName', i))
 
             # Issue SNMP GET command
             get_result = yield self.snmp.get(get_list, self.version)
+            name_result = yield self.snmp.get(name_list, self.version)
+
+            # If device gets disconnected, name_result is None
+            if name_result is not None:
+                for item in name_result:
+                    names.append(item[1].prettyPrint())
 
-            # Do not publish if UPS connection has dropped
+            # Do not publish if ibootbar connection has dropped
             try:
                 # Update session.data
-                session.data = update_cache(get_result, read_time)
+                oid_cache = update_cache(get_result, names, self.outlet_locked, read_time)
+                oid_cache['address'] = self.address
+                session.data = oid_cache
                 self.log.debug("{data}", data=session.data)
-                self.lastGet = time.time()
 
+                if get_result is None:
+                    raise ConnectionError('No SNMP response. Check your connection.')
+
+                self.lastGet = time.time()
                 # Publish to feed
-                message = _build_message(get_result, read_time)
+                message = _build_message(get_result, names, read_time)
                 self.log.debug("{msg}", msg=message)
-                session.app.publish_to_feed('ups', message)
+                session.app.publish_to_feed('ibootbar', message)
             except ConnectionError as e:
                 self.log.error(f'{e}')
                 yield dsleep(1)
                 self.log.info('Trying to reconnect.')
 
             if params['test_mode']:
                 break
 
         return True, "Finished Recording"
 
     def _stop_acq(self, session, params=None):
         """_stop_acq()
         **Task** - Stop task associated with acq process.
         """
-        self.is_streaming = False
-        return True, "Stopping Recording"
+        if self.is_streaming:
+            session.set_status('stopping')
+            self.is_streaming = False
+            return True, "Stopping Recording"
+        else:
+            return False, "Acq is not currently running"
+
+    @ocs_agent.param('outlet', choices=[1, 2, 3, 4, 5, 6, 7, 8])
+    @ocs_agent.param('state', choices=['on', 'off'])
+    @inlineCallbacks
+    def set_outlet(self, session, params=None):
+        """set_outlet(outlet, state)
+
+        **Task** - Set a particular outlet to on/off.
+
+        Parameters
+        ----------
+        outlet : int
+            Outlet number to set. Choices are 1-8 (physical outlets).
+        state : str
+            State to set outlet to, which may be 'on' or 'off'
+        """
+        with self.lock.acquire_timeout(3, job='set_outlet') as acquired:
+            if not acquired:
+                return False, "Could not acquire lock"
+
+            # Check if outlet is locked
+            outlet_id = params['outlet'] - 1
+            if self.outlet_locked[outlet_id]:
+                return False, 'Outlet {} is locked. Cannot turn outlet on/off.'.format(params['outlet'])
+
+            # Convert given state parameter to integer
+            if params['state'] == 'on':
+                state = 1
+            else:
+                state = 0
+
+            # Issue SNMP SET command to given outlet
+            outlet = [('IBOOTPDU-MIB', 'outletControl', outlet_id)]
+            setcmd = yield self.snmp.set(outlet, self.version, state)
+            self.log.info('{}'.format(setcmd))
+
+        # Force SNMP GET status commands by rewinding the lastGet time by sample period
+        self.lastGet = self.lastGet - self.sample_period
+
+        return True, 'Set outlet {} to {}'.\
+            format(params['outlet'], params['state'])
+
+    @ocs_agent.param('outlet', choices=[1, 2, 3, 4, 5, 6, 7, 8])
+    @ocs_agent.param('cycle_time', default=10, type=int)
+    @inlineCallbacks
+    def cycle_outlet(self, session, params=None):
+        """cycle_outlet(outlet, cycle_time=10)
+
+        **Task** - Cycle a particular outlet for given amount of seconds.
+
+        Parameters
+        ----------
+        outlet : int
+            Outlet number to cycle. Choices are 1-8 (physical outlets).
+        cycle_time : int
+            The amount of seconds to cycle an outlet. Default is 10 seconds.
+        """
+        with self.lock.acquire_timeout(3, job='cycle_outlet') as acquired:
+            if not acquired:
+                return False, "Could not acquire lock"
+
+            # Check if outlet is locked
+            outlet_id = params['outlet'] - 1
+            if self.outlet_locked[outlet_id]:
+                return False, 'Outlet {} is locked. Cannot cycle outlet.'.format(params['outlet'])
+
+            # Issue SNMP SET command for cycle time
+            set_cycle = [('IBOOTPDU-MIB', 'outletCycleTime', outlet_id)]
+            setcmd1 = yield self.snmp.set(set_cycle, self.version, params['cycle_time'])
+            self.log.info('{}'.format(setcmd1))
+
+            # Issue SNMP SET command to given outlet
+            outlet = [('IBOOTPDU-MIB', 'outletControl', outlet_id)]
+            setcmd2 = yield self.snmp.set(outlet, self.version, 2)
+            self.log.info('{}'.format(setcmd2))
+            self.log.info('Cycling outlet {} for {} seconds'.
+                          format(outlet_id, params['cycle_time']))
+
+        # Force SNMP GET status commands throughout the cycle time
+        for i in range(params['cycle_time'] + 1):
+            self.lastGet = self.lastGet - self.sample_period
+            yield dsleep(1)
+
+        return True, 'Cycled outlet {} for {} seconds'.\
+            format(params['outlet'], params['cycle_time'])
+
+    @ocs_agent.param('_')
+    @inlineCallbacks
+    def set_initial_state(self, session, params=None):
+        """set_initial_state()
+
+        **Task** - Set outlets to their initial states.
+
+        Performs a software reboot. The outlets are then set to their
+        respective initial states. This takes about 30 seconds.
+        """
+        with self.lock.acquire_timeout(3, job='reboot') as acquired:
+            if not acquired:
+                return False, "Could not acquire lock"
+
+            # Send SNMP SET command to set rebootSystem to True
+            reboot = [('IBOOTPDU-MIB', 'rebootSystem', 0)]
+            setcmd = yield self.snmp.set(reboot, self.version, 1)
+            self.log.info('{}'.format(setcmd))
+
+        # Force SNMP GET status commands
+        self.lastGet = self.lastGet - self.sample_period
+
+        return True, 'Rebooting. Outlets will be set to their initial states.'
+
+    @ocs_agent.param('outlet', choices=[1, 2, 3, 4, 5, 6, 7, 8])
+    @ocs_agent.param('lock', choices=[True, False])
+    def lock_outlet(self, session, params=None):
+        """lock_outlet(outlet, lock)
+
+        **Task** - Lock/unlocks a particular outlet, preventing change of state.
+
+        Parameters
+        ----------
+        outlet : int
+            Outlet number to lock/unlock. Choices are 1-8 (physical outlets).
+        lock : bool
+            Set to true to lock, set to false to unlock
+        """
+        with self.lock.acquire_timeout(3, job='lock_outlet') as acquired:
+            if not acquired:
+                return False, "Could not acquire lock"
+            # Lock/unlock specific outlet
+            outlet = params['outlet'] - 1
+            if params['lock']:
+                self.outlet_locked[outlet] = True
+            elif not params['lock']:
+                self.outlet_locked[outlet] = False
+
+        return True, 'Set outlet {} lock to {}'.\
+            format(params['outlet'], params['lock'])
 
 
 def add_agent_args(parser=None):
     """
     Build the argument parser for the Agent. Allows sphinx to automatically
     build documentation based on this function.
     """
     if parser is None:
         parser = argparse.ArgumentParser()
 
     pgroup = parser.add_argument_group("Agent Options")
     pgroup.add_argument("--address", help="Address to listen to.")
     pgroup.add_argument("--port", default=161,
                         help="Port to listen on.")
-    pgroup.add_argument("--snmp-version", default='1', choices=['1', '2', '3'],
+    pgroup.add_argument("--snmp-version", default='2', choices=['1', '2', '3'],
                         help="SNMP version for communication. Must match "
-                             + "configuration on the UPS.")
-    pgroup.add_argument("--mode", choices=['acq', 'test'])
+                             + "configuration on the ibootbar.")
+    pgroup.add_argument("--mode", default='acq', choices=['acq', 'test'])
+    pgroup.add_argument("--lock-outlet", nargs='+', type=int,
+                        help="List of outlets to lock on startup.")
 
     return parser
 
 
 def main(args=None):
     # Start logging
     txaio.start_logging(level=os.environ.get("LOGLEVEL", "info"))
 
     parser = add_agent_args()
-    args = site_config.parse_args(agent_class='UPSAgent',
+    args = site_config.parse_args(agent_class='ibootbarAgent',
                                   parser=parser,
                                   args=args)
 
     if args.mode == 'acq':
         init_params = True
     elif args.mode == 'test':
         init_params = False
 
     agent, runner = ocs_agent.init_site_agent(args)
-    p = UPSAgent(agent,
-                 address=args.address,
-                 port=int(args.port),
-                 version=int(args.snmp_version))
+    p = ibootbarAgent(agent,
+                      address=args.address,
+                      port=int(args.port),
+                      version=int(args.snmp_version),
+                      lock_outlet=args.lock_outlet)
 
     agent.register_process("acq",
                            p.acq,
                            p._stop_acq,
                            startup=init_params, blocking=False)
 
+    agent.register_task("set_outlet", p.set_outlet, blocking=False)
+    agent.register_task("cycle_outlet", p.cycle_outlet, blocking=False)
+    agent.register_task("set_initial_state", p.set_initial_state, blocking=False)
+    agent.register_task("lock_outlet", p.lock_outlet, blocking=False)
+
     runner.run(agent, auto_reconnect=True)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `socs-0.4.2/socs/agents/vantagepro2/agent.py` & `socs-0.4.3rc1/socs/agents/vantagepro2/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/vantagepro2/drivers.py` & `socs-0.4.3rc1/socs/agents/vantagepro2/drivers.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/wiregrid_actuator/agent.py` & `socs-0.4.3rc1/socs/agents/wiregrid_actuator/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/wiregrid_actuator/drivers/Actuator.py` & `socs-0.4.3rc1/socs/agents/wiregrid_actuator/drivers/Actuator.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/wiregrid_actuator/drivers/DigitalIO.py` & `socs-0.4.3rc1/socs/agents/wiregrid_actuator/drivers/DigitalIO.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/wiregrid_actuator/limitswitch_config.py` & `socs-0.4.3rc1/socs/agents/wiregrid_actuator/limitswitch_config.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/wiregrid_encoder/agent.py` & `socs-0.4.3rc1/socs/agents/wiregrid_encoder/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/wiregrid_encoder/drivers.py` & `socs-0.4.3rc1/socs/agents/wiregrid_encoder/drivers.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/wiregrid_kikusui/agent.py` & `socs-0.4.3rc1/socs/agents/wiregrid_kikusui/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/wiregrid_kikusui/drivers/common.py` & `socs-0.4.3rc1/socs/agents/wiregrid_kikusui/drivers/common.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/agents/xy_stage/agent.py` & `socs-0.4.3rc1/socs/agents/xy_stage/agent.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/common/moxa_serial.py` & `socs-0.4.3rc1/socs/common/moxa_serial.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/common/pmx.py` & `socs-0.4.3rc1/socs/common/pmx.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/common/prologix_interface.py` & `socs-0.4.3rc1/socs/common/prologix_interface.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/db/suprsync.py` & `socs-0.4.3rc1/socs/db/suprsync.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/mibs/IBOOTPDU-MIB.py` & `socs-0.4.3rc1/socs/mibs/IBOOTPDU-MIB.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/mibs/MBG-SNMP-LTNG-MIB.py` & `socs-0.4.3rc1/socs/mibs/MBG-SNMP-LTNG-MIB.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/mibs/MBG-SNMP-ROOT-MIB.py` & `socs-0.4.3rc1/socs/mibs/MBG-SNMP-ROOT-MIB.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/mibs/SNMPv2-MIB.py` & `socs-0.4.3rc1/socs/mibs/SNMPv2-MIB.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/mibs/UPS-MIB.py` & `socs-0.4.3rc1/socs/mibs/UPS-MIB.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/plugin.py` & `socs-0.4.3rc1/socs/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 package_name = 'socs'
 agents = {
     'ACUAgent': {'module': 'socs.agents.acu.agent', 'entry_point': 'main'},
     'BlueforsAgent': {'module': 'socs.agents.bluefors.agent', 'entry_point': 'main'},
     'CrateAgent': {'module': 'socs.agents.smurf_crate_monitor.agent', 'entry_point': 'main'},
     'CryomechCPAAgent': {'module': 'socs.agents.cryomech_cpa.agent', 'entry_point': 'main'},
     'FPGAAgent': {'module': 'socs.agents.holo_fpga.agent', 'entry_point': 'main'},
+    'FlowmeterAgent': {'module': 'socs.agents.ifm_sbn246_flowmeter.agent', 'entry_point': 'main'},
     'FTSAerotechAgent': {'module': 'socs.agents.fts_aerotech.agent', 'entry_point': 'main'},
     'HWPBBBAgent': {'module': 'socs.agents.hwp_encoder.agent', 'entry_point': 'main'},
     'HWPPicoscopeAgent': {'module': 'socs.agents.hwp_picoscope.agent', 'entry_point': 'main'},
+    'HWPPIDAgent': {'module': 'socs.agents.hwp_pid.agent', 'entry_point': 'main'},
+    'HWPPMXAgent': {'module': 'socs.agents.hwp_pmx.agent', 'entry_point': 'main'},
     'ibootbarAgent': {'module': 'socs.agents.ibootbar.agent', 'entry_point': 'main'},
     'LabJackAgent': {'module': 'socs.agents.labjack.agent', 'entry_point': 'main'},
     'Lakeshore240Agent': {'module': 'socs.agents.lakeshore240.agent', 'entry_point': 'main'},
     'Lakeshore336Agent': {'module': 'socs.agents.lakeshore336.agent', 'entry_point': 'main'},
     'Lakeshore370Agent': {'module': 'socs.agents.lakeshore370.agent', 'entry_point': 'main'},
     'Lakeshore372Agent': {'module': 'socs.agents.lakeshore372.agent', 'entry_point': 'main'},
     'Lakeshore425Agent': {'module': 'socs.agents.lakeshore425.agent', 'entry_point': 'main'},
     'LATRtXYStageAgent': {'module': 'socs.agents.xy_stage.agent', 'entry_point': 'main'},
     'MagpieAgent': {'module': 'socs.agents.magpie.agent', 'entry_point': 'main'},
     'MeinbergM1000Agent': {'module': 'socs.agents.meinberg_m1000.agent', 'entry_point': 'main'},
     'PfeifferAgent': {'module': 'socs.agents.pfeiffer_tpg366.agent', 'entry_point': 'main'},
     'PfeifferTC400Agent': {'module': 'socs.agents.pfeiffer_tc400.agent', 'entry_point': 'main'},
     'PysmurfController': {'module': 'socs.agents.pysmurf_controller.agent', 'entry_point': 'main'},
     'PysmurfMonitor': {'module': 'socs.agents.pysmurf_monitor.agent', 'entry_point': 'main'},
-    'RotationAgent': {'module': 'socs.agents.hwp_rotation.agent', 'entry_point': 'main'},
     'ScpiPsuAgent': {'module': 'socs.agents.scpi_psu.agent', 'entry_point': 'main'},
     'SmurfFileEmulator': {'module': 'socs.agents.smurf_file_emulator.agent', 'entry_point': 'main'},
     'SmurfStreamSimulator': {'module': 'socs.agents.smurf_stream_simulator.agent', 'entry_point': 'main'},
     'SmurfTimingCardAgent': {'module': 'socs.agents.smurf_timing_card.agent', 'entry_point': 'main'},
     'SupRsync': {'module': 'socs.agents.suprsync.agent', 'entry_point': 'main'},
     'SynaccessAgent': {'module': 'socs.agents.synacc.agent', 'entry_point': 'main'},
     'SynthAgent': {'module': 'socs.agents.holo_synth.agent', 'entry_point': 'main'},
```

### Comparing `socs-0.4.2/socs/snmp.py` & `socs-0.4.3rc1/socs/snmp.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs/testing/device_emulator.py` & `socs-0.4.3rc1/socs/testing/device_emulator.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/socs.egg-info/PKG-INFO` & `socs-0.4.3rc1/socs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socs
-Version: 0.4.2
+Version: 0.4.3rc1
 Summary: Simons Observatory Control System
 Home-page: https://github.com/simonsobs/socs
 Project-URL: Source Code, https://github.com/simonsobs/ocs
 Project-URL: Documentation, https://ocs.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/simonsobs/ocs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `socs-0.4.2/socs.egg-info/SOURCES.txt` & `socs-0.4.3rc1/socs.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 socs/Lakeshore/Lakeshore425.py
 socs/Lakeshore/__init__.py
 socs/agents/__init__.py
 socs/agents/ocs_plugin_so.py
 socs/agents/acu/__init__.py
 socs/agents/acu/agent.py
 socs/agents/acu/drivers.py
+socs/agents/acu/exercisor.py
 socs/agents/bluefors/__init__.py
 socs/agents/bluefors/agent.py
 socs/agents/cryomech_cpa/__init__.py
 socs/agents/cryomech_cpa/agent.py
 socs/agents/fts_aerotech/__init__.py
 socs/agents/fts_aerotech/agent.py
 socs/agents/holo_fpga/__init__.py
@@ -39,20 +40,26 @@
 socs/agents/holo_synth/agent.py
 socs/agents/hwp_encoder/__init__.py
 socs/agents/hwp_encoder/agent.py
 socs/agents/hwp_picoscope/__init__.py
 socs/agents/hwp_picoscope/agent.py
 socs/agents/hwp_picoscope/drivers/__init__.py
 socs/agents/hwp_picoscope/drivers/class_ps3000a.py
-socs/agents/hwp_rotation/__init__.py
-socs/agents/hwp_rotation/agent.py
-socs/agents/hwp_rotation/drivers/__init__.py
-socs/agents/hwp_rotation/drivers/pid_controller.py
+socs/agents/hwp_pid/__init__.py
+socs/agents/hwp_pid/agent.py
+socs/agents/hwp_pid/drivers/__init__.py
+socs/agents/hwp_pid/drivers/pid_controller.py
+socs/agents/hwp_pmx/__init__.py
+socs/agents/hwp_pmx/agent.py
+socs/agents/hwp_pmx/drivers/PMX_ethernet.py
+socs/agents/hwp_pmx/drivers/__init__.py
 socs/agents/ibootbar/__init__.py
 socs/agents/ibootbar/agent.py
+socs/agents/ifm_sbn246_flowmeter/__init__.py
+socs/agents/ifm_sbn246_flowmeter/agent.py
 socs/agents/labjack/__init__.py
 socs/agents/labjack/agent.py
 socs/agents/labjack/cal_curves/GA10K4D25_cal_curve.txt
 socs/agents/lakeshore240/__init__.py
 socs/agents/lakeshore240/agent.py
 socs/agents/lakeshore336/__init__.py
 socs/agents/lakeshore336/agent.py
```

### Comparing `socs-0.4.2/tests/test_device_emulator.py` & `socs-0.4.3rc1/tests/test_device_emulator.py`

 * *Files identical despite different names*

### Comparing `socs-0.4.2/versioneer.py` & `socs-0.4.3rc1/versioneer.py`

 * *Files identical despite different names*

