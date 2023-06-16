# Comparing `tmp/siriuspy-2.75.0.tar.gz` & `tmp/siriuspy-2.76.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siriuspy-2.75.0.tar", last modified: Tue May 23 19:09:19 2023, max compression
+gzip compressed data, was "siriuspy-2.76.0.tar", last modified: Fri Jun 16 14:01:11 2023, max compression
```

## Comparing `siriuspy-2.75.0.tar` & `siriuspy-2.76.0.tar`

### file list

```diff
@@ -1,389 +1,395 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.874388 siriuspy-2.75.0/
--rw-r--r--   0 runner    (1001) docker     (122)    34494 2023-05-23 19:09:08.000000 siriuspy-2.75.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-05-23 19:09:08.000000 siriuspy-2.75.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-05-23 19:09:19.874388 siriuspy-2.75.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      954 2023-05-23 19:09:08.000000 siriuspy-2.75.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-23 19:09:08.000000 siriuspy-2.75.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-23 19:09:19.874388 siriuspy-2.75.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     1243 2023-05-23 19:09:08.000000 siriuspy-2.75.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.834384 siriuspy-2.75.0/siriuspy/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.834384 siriuspy-2.75.0/siriuspy/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/bsmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15885 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/bsmp/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)     1904 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/bsmp/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    11790 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/bsmp/entities.py
--rw-r--r--   0 runner    (1001) docker     (122)      610 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/bsmp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     8110 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/bsmp/serial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/bsmp/types.py
--rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.834384 siriuspy-2.75.0/siriuspy/clientarch/
--rw-r--r--   0 runner    (1001) docker     (122)      306 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientarch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientarch/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientarch/devices.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientarch/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    20400 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientarch/pvarch.py
--rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientarch/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.838384 siriuspy-2.75.0/siriuspy/clientconfigdb/
--rw-r--r--   0 runner    (1001) docker     (122)      227 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3535 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/_templates.py
--rw-r--r--   0 runner    (1001) docker     (122)     9599 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/configdb_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5448 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/configdb_document.py
--rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/pvsconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.838384 siriuspy-2.75.0/siriuspy/clientconfigdb/types/
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13746 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/as_corrloop_params.py
--rw-r--r--   0 runner    (1001) docker     (122)    57636 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/as_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/as_pwrstate.py
--rw-r--r--   0 runner    (1001) docker     (122)    34247 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/as_rf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     3984 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/bo_normalized.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      700 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/bo_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/bo_ramp.py
--rw-r--r--   0 runner    (1001) docker     (122)      975 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)   123230 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/global_config.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_bbadata.py
--rw-r--r--   0 runner    (1001) docker     (122)    18619 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_bbbproc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_fofb.py
--rw-r--r--   0 runner    (1001) docker     (122)      957 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     3181 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_idff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      701 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py
--rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/tb_normalized.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/tb_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/tb_posang_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py
--rw-r--r--   0 runner    (1001) docker     (122)      693 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/ts_orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     1721 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientconfigdb/types/ts_posang_respm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.842385 siriuspy-2.75.0/siriuspy/clientweb/
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientweb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5896 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/clientweb/implementation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.842385 siriuspy-2.75.0/siriuspy/currinfo/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/currinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9620 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/currinfo/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.842385 siriuspy-2.75.0/siriuspy/currinfo/lifetime/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/currinfo/lifetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12607 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/currinfo/lifetime/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    23275 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/currinfo/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.842385 siriuspy-2.75.0/siriuspy/cycle/
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/cycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   104994 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/cycle/bo_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    31135 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/cycle/conn.py
--rw-r--r--   0 runner    (1001) docker     (122)     9781 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/cycle/fc_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3286 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/cycle/li_cycle_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    38408 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/cycle/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     3567 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/cycle/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.846385 siriuspy-2.75.0/siriuspy/devices/
--rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    48546 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/bbb.py
--rw-r--r--   0 runner    (1001) docker     (122)    41443 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/bpm.py
--rw-r--r--   0 runner    (1001) docker     (122)     7380 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/currinfo.py
--rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/dcct.py
--rw-r--r--   0 runner    (1001) docker     (122)    12731 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (122)    14364 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/dvf.py
--rw-r--r--   0 runner    (1001) docker     (122)    30814 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/egun.py
--rw-r--r--   0 runner    (1001) docker     (122)     1743 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/energy.py
--rw-r--r--   0 runner    (1001) docker     (122)    48527 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/fofb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/ict.py
--rw-r--r--   0 runner    (1001) docker     (122)     9625 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/idff.py
--rw-r--r--   0 runner    (1001) docker     (122)    17596 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/ids.py
--rw-r--r--   0 runner    (1001) docker     (122)    20741 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/injctrl.py
--rw-r--r--   0 runner    (1001) docker     (122)    36024 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/injsys.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/lienergy.py
--rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/lillrf.py
--rw-r--r--   0 runner    (1001) docker     (122)      964 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/machshift.py
--rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/modltr.py
--rw-r--r--   0 runner    (1001) docker     (122)    36060 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/orbit_interlock.py
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/posang.py
--rw-r--r--   0 runner    (1001) docker     (122)     9576 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/psconv.py
--rw-r--r--   0 runner    (1001) docker     (122)    12042 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/pssofb.py
--rw-r--r--   0 runner    (1001) docker     (122)    19964 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/pstesters.py
--rw-r--r--   0 runner    (1001) docker     (122)    29550 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/pwrsupply.py
--rw-r--r--   0 runner    (1001) docker     (122)    35448 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/rf.py
--rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/screen.py
--rw-r--r--   0 runner    (1001) docker     (122)    22629 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/sofb.py
--rw-r--r--   0 runner    (1001) docker     (122)     2606 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/syncd.py
--rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/timing.py
--rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/devices/tune.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.846385 siriuspy-2.75.0/siriuspy/diagbeam/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagbeam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.846385 siriuspy-2.75.0/siriuspy/diagbeam/bpm/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagbeam/bpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24052 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagbeam/bpm/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.846385 siriuspy-2.75.0/siriuspy/diagbeam/dcct/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagbeam/dcct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagbeam/dcct/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.846385 siriuspy-2.75.0/siriuspy/diagbeam/ict/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagbeam/ict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagbeam/ict/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.846385 siriuspy-2.75.0/siriuspy/diagbeam/screen/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagbeam/screen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12756 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagbeam/screen/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.846385 siriuspy-2.75.0/siriuspy/diagbeam/slit/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagbeam/slit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6750 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagbeam/slit/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.846385 siriuspy-2.75.0/siriuspy/diagsys/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.850386 siriuspy-2.75.0/siriuspy/diagsys/lidiag/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/lidiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/lidiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     8168 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/lidiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/lidiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.850386 siriuspy-2.75.0/siriuspy/diagsys/psdiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/psdiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2556 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/psdiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     4299 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/psdiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     6705 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/psdiag/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.850386 siriuspy-2.75.0/siriuspy/diagsys/pudiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/pudiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/pudiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/pudiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/pudiag/pvs.py
--rw-r--r--   0 runner    (1001) docker     (122)     6824 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/pvs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.850386 siriuspy-2.75.0/siriuspy/diagsys/rfdiag/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/rfdiag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/rfdiag/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/rfdiag/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     4891 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/diagsys/rfdiag/pvs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2135 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/envars.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.850386 siriuspy-2.75.0/siriuspy/epics/
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/epics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      624 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/epics/multiproc.py
--rw-r--r--   0 runner    (1001) docker     (122)     9097 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/epics/properties.py
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/epics/pv.py
--rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/epics/pv_fake.py
--rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/epics/pv_time_serie.py
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/epics/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.850386 siriuspy-2.75.0/siriuspy/fofb/
--rw-r--r--   0 runner    (1001) docker     (122)       34 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/fofb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18873 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/fofb/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    80150 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/fofb/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.850386 siriuspy-2.75.0/siriuspy/idff/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/idff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7455 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/idff/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3150 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/idff/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    13821 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/idff/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.854386 siriuspy-2.75.0/siriuspy/injctrl/
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/injctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15244 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/injctrl/bias_feedback.py
--rw-r--r--   0 runner    (1001) docker     (122)    26067 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/injctrl/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    67948 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/injctrl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.854386 siriuspy-2.75.0/siriuspy/machshift/
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/machshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/machshift/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    77640 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/machshift/macreport.py
--rw-r--r--   0 runner    (1001) docker     (122)     8913 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/machshift/macschedule.py
--rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/machshift/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     5429 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/machshift/test_macreport.py
--rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/machshift/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.854386 siriuspy-2.75.0/siriuspy/magnet/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/magnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/magnet/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/magnet/excdata.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/magnet/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)    15453 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/magnet/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/magnet/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.854386 siriuspy-2.75.0/siriuspy/meas/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/meas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11826 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/meas/csdev.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.854386 siriuspy-2.75.0/siriuspy/meas/liemit/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/meas/liemit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/meas/liemit/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    13017 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/meas/liemit/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.854386 siriuspy-2.75.0/siriuspy/meas/lienergy/
--rw-r--r--   0 runner    (1001) docker     (122)       80 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/meas/lienergy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/meas/lienergy/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     8714 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/meas/lienergy/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    25137 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/meas/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.854386 siriuspy-2.75.0/siriuspy/namesys/
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/namesys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/namesys/implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.858386 siriuspy-2.75.0/siriuspy/optics/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/optics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      363 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/optics/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     6906 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/optics/lattice_survey.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.858386 siriuspy-2.75.0/siriuspy/opticscorr/
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/opticscorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    34878 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/opticscorr/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    16096 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/opticscorr/chrom.py
--rw-r--r--   0 runner    (1001) docker     (122)    13454 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/opticscorr/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    18765 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/opticscorr/opticscorr.py
--rw-r--r--   0 runner    (1001) docker     (122)     8006 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/opticscorr/tune.py
--rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/opticscorr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.858386 siriuspy-2.75.0/siriuspy/oscilloscope/
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/oscilloscope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6691 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/oscilloscope/keysight.py
--rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/oscilloscope/scopes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.858386 siriuspy-2.75.0/siriuspy/posang/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/posang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/posang/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    19747 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/posang/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/posang/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.858386 siriuspy-2.75.0/siriuspy/pwrsupply/
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8950 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/beaglebone.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.858386 siriuspy-2.75.0/siriuspy/pwrsupply/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/bsmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    25156 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/bsmp/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)    19464 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/bsmp/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    53763 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/bsmp/entities.py
--rw-r--r--   0 runner    (1001) docker     (122)      850 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/bsmp/factory.py
--rw-r--r--   0 runner    (1001) docker     (122)   150426 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    10620 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.862387 siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/
--rw-r--r--   0 runner    (1001) docker     (122)      841 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/pru.py
--rw-r--r--   0 runner    (1001) docker     (122)    26340 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/prucontroller.py
--rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/prucparms.py
--rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/psdevstate.py
--rw-r--r--   0 runner    (1001) docker     (122)     7712 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/udc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.862387 siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/
--rw-r--r--   0 runner    (1001) docker     (122)      866 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/pscontroller.py
--rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/pscreaders.py
--rw-r--r--   0 runner    (1001) docker     (122)     5502 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/pscstatus.py
--rw-r--r--   0 runner    (1001) docker     (122)    17064 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/pscwriters.py
--rw-r--r--   0 runner    (1001) docker     (122)    42124 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/psmodel.py
--rw-r--r--   0 runner    (1001) docker     (122)    34134 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/pssofb.py
--rw-r--r--   0 runner    (1001) docker     (122)    12500 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/pwrsupply/siggen.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.862387 siriuspy-2.75.0/siriuspy/ramp/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/ramp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28999 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/ramp/conn.py
--rw-r--r--   0 runner    (1001) docker     (122)      346 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/ramp/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3969 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/ramp/magnet.py
--rw-r--r--   0 runner    (1001) docker     (122)    45093 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/ramp/ramp.py
--rw-r--r--   0 runner    (1001) docker     (122)    29333 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/ramp/reconst_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6985 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/ramp/test_reconst_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4158 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/ramp/testwfm.py
--rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/ramp/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    30145 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/ramp/waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.862387 siriuspy-2.75.0/siriuspy/search/
--rw-r--r--   0 runner    (1001) docker     (122)      359 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/search/bpms_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     6612 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/search/hl_time_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     4859 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/search/id_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     4152 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/search/ioc_search.py
--rw-r--r--   0 runner    (1001) docker     (122)    16917 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/search/ll_time_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/search/ma_search.py
--rw-r--r--   0 runner    (1001) docker     (122)    23882 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/search/ps_search.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.866387 siriuspy-2.75.0/siriuspy/simul/
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/simul/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/simul/simfactory.py
--rw-r--r--   0 runner    (1001) docker     (122)     6298 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/simul/simps.py
--rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/simul/simpv.py
--rw-r--r--   0 runner    (1001) docker     (122)     7391 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/simul/simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/simul/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.866387 siriuspy-2.75.0/siriuspy/sofb/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/sofb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4646 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/sofb/base_class.py
--rw-r--r--   0 runner    (1001) docker     (122)    28072 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/sofb/bpms.py
--rw-r--r--   0 runner    (1001) docker     (122)    32149 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/sofb/correctors.py
--rw-r--r--   0 runner    (1001) docker     (122)    47045 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/sofb/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    45797 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/sofb/main.py
--rw-r--r--   0 runner    (1001) docker     (122)    12220 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/sofb/matrix.py
--rw-r--r--   0 runner    (1001) docker     (122)    39936 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/sofb/orbit.py
--rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/sofb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.866387 siriuspy-2.75.0/siriuspy/stabinfo/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/stabinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/stabinfo/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)     7708 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/stabinfo/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     8093 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.866387 siriuspy-2.75.0/siriuspy/timesys/
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/timesys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20220 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/timesys/csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)    12705 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/timesys/hl_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)    33256 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/timesys/ll_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/timesys/plot_network.py
--rw-r--r--   0 runner    (1001) docker     (122)     5957 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/timesys/static_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     8732 2023-05-23 19:09:08.000000 siriuspy-2.75.0/siriuspy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.834384 siriuspy-2.75.0/siriuspy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-05-23 19:09:19.000000 siriuspy-2.75.0/siriuspy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9945 2023-05-23 19:09:19.000000 siriuspy-2.75.0/siriuspy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 19:09:19.000000 siriuspy-2.75.0/siriuspy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 19:09:19.000000 siriuspy-2.75.0/siriuspy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-05-23 19:09:19.000000 siriuspy-2.75.0/siriuspy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-23 19:09:19.000000 siriuspy-2.75.0/siriuspy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.870387 siriuspy-2.75.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.870387 siriuspy-2.75.0/tests/bsmp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/bsmp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5698 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/bsmp/test_bsmp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    14788 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/bsmp/test_commands.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    13382 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/bsmp/test_entities.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7719 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/bsmp/test_serial.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1837 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/bsmp/test_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.870387 siriuspy-2.75.0/tests/clientconfigdb/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/clientconfigdb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2843 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/clientconfigdb/test_configdb_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.870387 siriuspy-2.75.0/tests/clientweb/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/clientweb/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11633 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/clientweb/test_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.870387 siriuspy-2.75.0/tests/currinfo/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/currinfo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.870387 siriuspy-2.75.0/tests/currinfo/lifetime/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/currinfo/lifetime/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1908 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/currinfo/lifetime/test_main.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6495 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/currinfo/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2653 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/currinfo/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.870387 siriuspy-2.75.0/tests/magnet/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/magnet/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2275 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/magnet/test_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2687 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/magnet/tests_normalizer.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3618 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/mock_servweb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.870387 siriuspy-2.75.0/tests/namesys/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/namesys/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4896 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/namesys/test_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.870387 siriuspy-2.75.0/tests/opticscorr/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/opticscorr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5490 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/opticscorr/test_chrom.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4609 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/opticscorr/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    23381 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/opticscorr/test_opticscorr.py
--rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/opticscorr/test_tune.py
--rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/opticscorr/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.870387 siriuspy-2.75.0/tests/posang/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/posang/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2872 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/posang/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3164 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/posang/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.874388 siriuspy-2.75.0/tests/pwrsupply/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/pwrsupply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18979 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/pwrsupply/db.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.874388 siriuspy-2.75.0/tests/pwrsupply/pructrl/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/pwrsupply/pructrl/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2257 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/pwrsupply/pructrl/test_pru.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.874388 siriuspy-2.75.0/tests/pwrsupply/psctrl/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/pwrsupply/psctrl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4853 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/pwrsupply/psctrl/test_pscwriters.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      166 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/pwrsupply/test_beaglebone.py
--rwxr-xr-x   0 runner    (1001) docker     (122)       89 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/pwrsupply/test_bsmp.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6439 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/pwrsupply/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7331 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/pwrsupply/test_data.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2323 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/pwrsupply/test_siggen.py
--rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/pwrsupply/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.874388 siriuspy-2.75.0/tests/ramp/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/ramp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     5699 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/ramp/test_magnet.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7235 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/ramp/test_waveform.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.874388 siriuspy-2.75.0/tests/search/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2412 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/search/test_hl_time_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      559 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/search/test_init.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3831 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/search/test_ll_time_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     6120 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/search/test_ma_search.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    13502 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/search/test_ps_search.py
--rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/test_callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1009 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/test_csdev.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1605 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/test_envars.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11533 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:19.874388 siriuspy-2.75.0/tests/timesys/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/timesys/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4999 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/timesys/test_csdev.py
--rw-r--r--   0 runner    (1001) docker     (122)      978 2023-05-23 19:09:08.000000 siriuspy-2.75.0/tests/timesys/test_plot_network.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.822934 siriuspy-2.76.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    34494 2023-06-16 14:01:00.000000 siriuspy-2.76.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-06-16 14:01:00.000000 siriuspy-2.76.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-06-16 14:01:11.822934 siriuspy-2.76.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      954 2023-06-16 14:01:00.000000 siriuspy-2.76.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-16 14:01:00.000000 siriuspy-2.76.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 14:01:11.822934 siriuspy-2.76.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1243 2023-06-16 14:01:00.000000 siriuspy-2.76.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.786934 siriuspy-2.76.0/siriuspy/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.786934 siriuspy-2.76.0/siriuspy/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/bsmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15885 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/bsmp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1904 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/bsmp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11790 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/bsmp/entities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      610 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/bsmp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8110 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/bsmp/serial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1204 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/bsmp/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2992 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.790934 siriuspy-2.76.0/siriuspy/clientarch/
+-rw-r--r--   0 runner    (1001) docker     (122)      306 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientarch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13813 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientarch/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6392 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientarch/devices.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientarch/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20400 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientarch/pvarch.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5003 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientarch/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.790934 siriuspy-2.76.0/siriuspy/clientconfigdb/
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3345 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/_templates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9599 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/configdb_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5448 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/configdb_document.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4785 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/pvsconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.790934 siriuspy-2.76.0/siriuspy/clientconfigdb/types/
+-rw-r--r--   0 runner    (1001) docker     (122)      286 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13746 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/as_corrloop_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)    57636 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/as_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6681 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/as_pwrstate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34247 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/as_rf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3984 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/bo_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      700 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/bo_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3042 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/bo_ramp.py
+-rw-r--r--   0 runner    (1001) docker     (122)      975 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)   123230 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/global_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_bbadata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18619 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_bbbproc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4741 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_fofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3181 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_idff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      701 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/tb_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/tb_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1651 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/tb_posang_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      969 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/ts_orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1721 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientconfigdb/types/ts_posang_respm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.790934 siriuspy-2.76.0/siriuspy/clientweb/
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientweb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5896 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/clientweb/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2236 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.794934 siriuspy-2.76.0/siriuspy/currinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/currinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9620 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/currinfo/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.794934 siriuspy-2.76.0/siriuspy/currinfo/lifetime/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/currinfo/lifetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12607 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/currinfo/lifetime/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23275 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/currinfo/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.794934 siriuspy-2.76.0/siriuspy/cycle/
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/cycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   104994 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/cycle/bo_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31135 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/cycle/conn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9781 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/cycle/fc_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3286 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/cycle/li_cycle_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38408 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/cycle/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3574 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/cycle/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/devices/
+-rw-r--r--   0 runner    (1001) docker     (122)     1784 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48546 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/bbb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2786 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/blctrl.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41443 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/bpm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7380 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/currinfo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2402 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/dcct.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12885 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16522 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/dvf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30814 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/egun.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1743 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/energy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    51761 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/fofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2121 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/ict.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9798 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/idff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21226 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/ids.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20741 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/injctrl.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36024 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/injsys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/lienergy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6948 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/lillrf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      964 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/machshift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/modltr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36060 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/orbit_interlock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/posang.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9576 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/psconv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12042 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/pssofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20070 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/pstesters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29992 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/pwrsupply.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35448 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/rf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/screen.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22629 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/sofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2606 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/syncd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17907 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/timing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5055 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/devices/tune.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/diagbeam/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagbeam/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/diagbeam/bpm/
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagbeam/bpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24052 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagbeam/bpm/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/diagbeam/dcct/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagbeam/dcct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8215 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagbeam/dcct/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/diagbeam/ict/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagbeam/ict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4878 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagbeam/ict/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/diagbeam/screen/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagbeam/screen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12756 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagbeam/screen/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/diagbeam/slit/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagbeam/slit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6750 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagbeam/slit/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/diagsys/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/diagsys/lidiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/lidiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/lidiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8168 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/lidiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8774 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/lidiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/diagsys/psdiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/psdiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2699 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/psdiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4582 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/psdiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7692 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/psdiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/diagsys/pudiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/pudiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/pudiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2871 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/pudiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4099 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/pudiag/pvs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6824 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/diagsys/rfdiag/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/rfdiag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2409 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/rfdiag/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/rfdiag/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4891 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/diagsys/rfdiag/pvs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/dvfimgproc/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/dvfimgproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7611 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/dvfimgproc/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15404 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/dvfimgproc/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7057 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/dvfimgproc/meas.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2135 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/envars.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.798934 siriuspy-2.76.0/siriuspy/epics/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/epics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      624 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/epics/multiproc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9097 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/epics/properties.py
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/epics/pv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/epics/pv_fake.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9170 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/epics/pv_time_serie.py
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/epics/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.802934 siriuspy-2.76.0/siriuspy/fofb/
+-rw-r--r--   0 runner    (1001) docker     (122)       34 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/fofb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20125 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/fofb/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    79298 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/fofb/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.802934 siriuspy-2.76.0/siriuspy/idff/
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/idff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7475 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/idff/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3408 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/idff/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13812 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/idff/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.802934 siriuspy-2.76.0/siriuspy/injctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/injctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15244 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/injctrl/bias_feedback.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26067 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/injctrl/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    67948 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/injctrl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.802934 siriuspy-2.76.0/siriuspy/machshift/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/machshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1297 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/machshift/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    77640 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/machshift/macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8913 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/machshift/macschedule.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2237 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/machshift/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5429 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/machshift/test_macreport.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/machshift/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.802934 siriuspy-2.76.0/siriuspy/magnet/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/magnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/magnet/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8736 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/magnet/excdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/magnet/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15453 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/magnet/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/magnet/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.802934 siriuspy-2.76.0/siriuspy/meas/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/meas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11826 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/meas/csdev.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.802934 siriuspy-2.76.0/siriuspy/meas/liemit/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/meas/liemit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/meas/liemit/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13017 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/meas/liemit/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.802934 siriuspy-2.76.0/siriuspy/meas/lienergy/
+-rw-r--r--   0 runner    (1001) docker     (122)       80 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/meas/lienergy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2821 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/meas/lienergy/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8714 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/meas/lienergy/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25137 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/meas/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.806934 siriuspy-2.76.0/siriuspy/namesys/
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/namesys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15210 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/namesys/implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.806934 siriuspy-2.76.0/siriuspy/optics/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/optics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      363 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/optics/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8749 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/optics/lattice_survey.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.806934 siriuspy-2.76.0/siriuspy/opticscorr/
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/opticscorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34878 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/opticscorr/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16096 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/opticscorr/chrom.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13454 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/opticscorr/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18765 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/opticscorr/opticscorr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8006 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/opticscorr/tune.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/opticscorr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.806934 siriuspy-2.76.0/siriuspy/oscilloscope/
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/oscilloscope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6691 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/oscilloscope/keysight.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/oscilloscope/scopes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.806934 siriuspy-2.76.0/siriuspy/posang/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/posang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/posang/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19747 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/posang/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1678 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/posang/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.806934 siriuspy-2.76.0/siriuspy/pwrsupply/
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8950 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/beaglebone.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.810934 siriuspy-2.76.0/siriuspy/pwrsupply/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/bsmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25156 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/bsmp/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19464 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/bsmp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53763 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/bsmp/entities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      850 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/bsmp/factory.py
+-rw-r--r--   0 runner    (1001) docker     (122)   150426 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3624 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10620 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.810934 siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3393 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/pru.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26340 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/prucontroller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6133 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/prucparms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/psdevstate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7712 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/udc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.810934 siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7884 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/pscontroller.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/pscreaders.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5502 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/pscstatus.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17064 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/pscwriters.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42124 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/psmodel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34134 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/pssofb.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12500 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/pwrsupply/siggen.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.810934 siriuspy-2.76.0/siriuspy/ramp/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/ramp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28999 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/ramp/conn.py
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/ramp/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3969 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/ramp/magnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45093 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/ramp/ramp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29333 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/ramp/reconst_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6985 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/ramp/test_reconst_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4158 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/ramp/testwfm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/ramp/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30145 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/ramp/waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.814934 siriuspy-2.76.0/siriuspy/search/
+-rw-r--r--   0 runner    (1001) docker     (122)      359 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3537 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/search/bpms_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6612 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/search/hl_time_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5566 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/search/id_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4152 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/search/ioc_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16917 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/search/ll_time_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7219 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/search/ma_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23882 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/search/ps_search.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.814934 siriuspy-2.76.0/siriuspy/simul/
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/simul/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/simul/simfactory.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6298 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/simul/simps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2324 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/simul/simpv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7391 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/simul/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4266 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/simul/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.814934 siriuspy-2.76.0/siriuspy/sofb/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/sofb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4646 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/sofb/base_class.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28072 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/sofb/bpms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32149 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/sofb/correctors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    47045 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/sofb/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    46519 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/sofb/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12220 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/sofb/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39936 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/sofb/orbit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3030 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/sofb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.814934 siriuspy-2.76.0/siriuspy/stabinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/stabinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3558 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/stabinfo/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7708 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/stabinfo/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8093 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.814934 siriuspy-2.76.0/siriuspy/timesys/
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/timesys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20220 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/timesys/csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12705 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/timesys/hl_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33256 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/timesys/ll_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6015 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/timesys/plot_network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5957 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/timesys/static_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8732 2023-06-16 14:01:00.000000 siriuspy-2.76.0/siriuspy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.786934 siriuspy-2.76.0/siriuspy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-06-16 14:01:11.000000 siriuspy-2.76.0/siriuspy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10089 2023-06-16 14:01:11.000000 siriuspy-2.76.0/siriuspy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 14:01:11.000000 siriuspy-2.76.0/siriuspy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-16 14:01:11.000000 siriuspy-2.76.0/siriuspy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-06-16 14:01:11.000000 siriuspy-2.76.0/siriuspy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-16 14:01:11.000000 siriuspy-2.76.0/siriuspy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.814934 siriuspy-2.76.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.818934 siriuspy-2.76.0/tests/bsmp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/bsmp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5698 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/bsmp/test_bsmp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    14788 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/bsmp/test_commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13382 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/bsmp/test_entities.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7719 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/bsmp/test_serial.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1837 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/bsmp/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.818934 siriuspy-2.76.0/tests/clientconfigdb/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/clientconfigdb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2843 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/clientconfigdb/test_configdb_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.818934 siriuspy-2.76.0/tests/clientweb/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/clientweb/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11633 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/clientweb/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.818934 siriuspy-2.76.0/tests/currinfo/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/currinfo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.818934 siriuspy-2.76.0/tests/currinfo/lifetime/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/currinfo/lifetime/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1908 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/currinfo/lifetime/test_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6495 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/currinfo/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2653 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/currinfo/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.818934 siriuspy-2.76.0/tests/magnet/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/magnet/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2275 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/magnet/test_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2687 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/magnet/tests_normalizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3618 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/mock_servweb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.818934 siriuspy-2.76.0/tests/namesys/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/namesys/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4896 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/namesys/test_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.818934 siriuspy-2.76.0/tests/opticscorr/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/opticscorr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5490 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/opticscorr/test_chrom.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4609 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/opticscorr/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    23381 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/opticscorr/test_opticscorr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/opticscorr/test_tune.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1145 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/opticscorr/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.818934 siriuspy-2.76.0/tests/posang/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/posang/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2872 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/posang/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3164 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/posang/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.818934 siriuspy-2.76.0/tests/pwrsupply/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/pwrsupply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18979 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/pwrsupply/db.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.822934 siriuspy-2.76.0/tests/pwrsupply/pructrl/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/pwrsupply/pructrl/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2257 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/pwrsupply/pructrl/test_pru.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.822934 siriuspy-2.76.0/tests/pwrsupply/psctrl/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/pwrsupply/psctrl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4853 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/pwrsupply/psctrl/test_pscwriters.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      166 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/pwrsupply/test_beaglebone.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)       89 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/pwrsupply/test_bsmp.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6439 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/pwrsupply/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7331 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/pwrsupply/test_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2323 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/pwrsupply/test_siggen.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3146 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/pwrsupply/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.822934 siriuspy-2.76.0/tests/ramp/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/ramp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5699 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/ramp/test_magnet.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7235 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/ramp/test_waveform.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.822934 siriuspy-2.76.0/tests/search/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2412 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/search/test_hl_time_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      559 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/search/test_init.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3831 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/search/test_ll_time_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6120 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/search/test_ma_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    13502 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/search/test_ps_search.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/test_callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1009 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/test_csdev.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1605 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/test_envars.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11533 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:11.822934 siriuspy-2.76.0/tests/timesys/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/timesys/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4999 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/timesys/test_csdev.py
+-rw-r--r--   0 runner    (1001) docker     (122)      978 2023-06-16 14:01:00.000000 siriuspy-2.76.0/tests/timesys/test_plot_network.py
```

### Comparing `siriuspy-2.75.0/LICENSE` & `siriuspy-2.76.0/LICENSE`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/PKG-INFO` & `siriuspy-2.76.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siriuspy
-Version: 2.75.0
+Version: 2.76.0
 Summary: Development packages for Sirius
 Home-page: https://github.com/lnls-sirius/dev-packages
 Download-URL: https://github.com/lnls-sirius/dev-packages
 Author: lnls-sirius
 License: GNU GPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `siriuspy-2.75.0/README.md` & `siriuspy-2.76.0/README.md`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/setup.py` & `siriuspy-2.76.0/setup.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/bsmp/commands.py` & `siriuspy-2.76.0/siriuspy/bsmp/commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/bsmp/constants.py` & `siriuspy-2.76.0/siriuspy/bsmp/constants.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/bsmp/entities.py` & `siriuspy-2.76.0/siriuspy/bsmp/entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/bsmp/exceptions.py` & `siriuspy-2.76.0/siriuspy/bsmp/exceptions.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/bsmp/serial.py` & `siriuspy-2.76.0/siriuspy/bsmp/serial.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/bsmp/types.py` & `siriuspy-2.76.0/siriuspy/bsmp/types.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/callbacks.py` & `siriuspy-2.76.0/siriuspy/callbacks.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientarch/client.py` & `siriuspy-2.76.0/siriuspy/clientarch/client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientarch/devices.py` & `siriuspy-2.76.0/siriuspy/clientarch/devices.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientarch/exceptions.py` & `siriuspy-2.76.0/siriuspy/clientarch/exceptions.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientarch/pvarch.py` & `siriuspy-2.76.0/siriuspy/clientarch/pvarch.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientarch/time.py` & `siriuspy-2.76.0/siriuspy/clientarch/time.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/_templates.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/_templates.py`

 * *Files 11% similar despite different names*

```diff
@@ -67,39 +67,32 @@
 
 
 # NOTE: It would be better if this method raised an error with a message
 #       specifying the name of the PV which is incompatible.
 def _recursive_check(ref_value, value, checklength=True):
     tps = {type(ref_value), type(value)}
     if len(tps) > len(tps - _INT_TYPES) > 0:
-        # print('h1')
         return False
     elif len(tps) > len(tps - _FLOAT_TYPES) > 0:
-        # print('h2')
         return False
     elif isinstance(ref_value, dict):
         if checklength and len(value) != len(ref_value):
-            # print('h3')
             return False
         for key, val in value.items():
             if key not in ref_value and checklength:
-                # print('h4')
                 return False
             if key in ref_value:
                 v_ref = ref_value[key]
                 if isinstance(key, str) and key.endswith('*'):
                     checked = _recursive_check(v_ref, val, checklength=False)
                 else:
                     checked = _recursive_check(v_ref, val, checklength)
                 if not checked:
-                    # print('h5')
                     return False
     elif isinstance(ref_value, (list, tuple, _np.ndarray)):
         if checklength and len(ref_value) != len(value):
-            # print('h6')
             return False
         for i in range(min(len(value), len(ref_value))):
             checked = _recursive_check(value[i], ref_value[i], checklength)
             if not checked:
-                # print('h7')
                 return False
     return True
```

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/configdb_client.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/configdb_client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/configdb_document.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/configdb_document.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/pvsconfig.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/pvsconfig.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/as_corrloop_params.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/as_corrloop_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/as_diagnostics.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/as_diagnostics.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/as_pwrstate.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/as_pwrstate.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/as_rf.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/as_rf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/bo_chromcorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/bo_normalized.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/bo_normalized.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/bo_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/bo_orbit.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/bo_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/bo_ramp.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/bo_ramp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/bo_tunecorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/global_config.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/global_config.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_bbadata.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_bbadata.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_bbbproc.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_bbbproc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_chromcorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_fastorbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_fofb.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_fofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_id.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_id.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_idff.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_idff.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_orbit.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/si_tunecorr_params.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/tb_normalized.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/tb_normalized.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/tb_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/tb_orbit.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/tb_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/tb_posang_respm.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/tb_posang_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/ts_orbcorr_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/ts_orbit.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/ts_orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientconfigdb/types/ts_posang_respm.py` & `siriuspy-2.76.0/siriuspy/clientconfigdb/types/ts_posang_respm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/clientweb/implementation.py` & `siriuspy-2.76.0/siriuspy/clientweb/implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/csdev.py` & `siriuspy-2.76.0/siriuspy/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/currinfo/csdev.py` & `siriuspy-2.76.0/siriuspy/currinfo/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/currinfo/lifetime/main.py` & `siriuspy-2.76.0/siriuspy/currinfo/lifetime/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/currinfo/main.py` & `siriuspy-2.76.0/siriuspy/currinfo/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/cycle/__init__.py` & `siriuspy-2.76.0/siriuspy/cycle/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/cycle/bo_cycle_data.py` & `siriuspy-2.76.0/siriuspy/cycle/bo_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/cycle/conn.py` & `siriuspy-2.76.0/siriuspy/cycle/conn.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/cycle/fc_cycle_data.py` & `siriuspy-2.76.0/siriuspy/cycle/fc_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/cycle/li_cycle_data.py` & `siriuspy-2.76.0/siriuspy/cycle/li_cycle_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/cycle/main.py` & `siriuspy-2.76.0/siriuspy/cycle/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/cycle/util.py` & `siriuspy-2.76.0/siriuspy/cycle/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             {'sec': 'SI', 'dis': 'PS', 'dev': 'FC.*'}))
     else:
         names.extend(_PSSearch.get_psnames(
             {'sec': 'SI', 'dis': 'PS', 'dev': '(B|Q.*|S.*|C.*|FC.*)'}))
 
     to_remove = _PSSearch.get_psnames({'sec': 'TS', 'idx': '(0|1E2)'})
     to_remove.extend(_PSSearch.get_psnames(
-        {'sec': 'SI', 'sub': '10SB', 'dev': '(CH|CV|QS)'}))
+        {'sec': 'SI', 'sub': '(10SB|17SA)', 'dev': '(CH|CV|QS)'}))
     to_remove.extend(_PSSearch.get_psnames(
         {'sec': 'SI', 'sub': '(01M1|01M2)', 'dev': '(FCH|FCV)'}))
     for name in to_remove:
         names.remove(name)
     return names
```

### Comparing `siriuspy-2.75.0/siriuspy/devices/__init__.py` & `siriuspy-2.76.0/siriuspy/devices/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from .dcct import DCCT
 from .device import Device, DeviceApp, Devices, DeviceNC
 from .egun import EGBias, EGFilament, EGHVPS, EGTriggerPS, EGPulsePS, EGun
 from .energy import Energy
 from .fofb import FOFBCtrlDCC, BPMDCC, FOFBCtrlRef, FamFOFBControllers, \
     FamFastCorrs, HLFOFB
 from .ict import ICT, TranspEff
-from .ids import APU, WIG, EPU
-from .idff import IDFF, WIGIDFF, EPUIDFF, APUIDFF
+from .ids import APU, WIG, PAPU, EPU
+from .idff import IDFF, WIGIDFF, PAPUIDFF, EPUIDFF, APUIDFF
 from .injctrl import InjCtrl
 from .injsys import ASPUStandbyHandler, BOPSRampStandbyHandler, \
     BORFRampStandbyHandler, InjBOStandbyHandler, InjSysStandbyHandler, \
     LILLRFStandbyHandler, InjSysPUModeHandler
 from .lillrf import LILLRF, DevLILLRF
 from .machshift import MachShift
 from .modltr import LIModltr
@@ -31,13 +31,14 @@
 from .screen import Screen
 from .sofb import SOFB
 from .syncd import DevicesSync
 from .timing import EVG, Event, Trigger, HLTiming
 from .tune import TuneFrac, TuneProc, Tune, TuneCorr
 from .dvf import DVF, DVFImgProc
 from .lienergy import LIEnergy
+from .blctrl import BLPPSCtrl
 
 
 del device, bpm, dcct, egun, ict, lillrf, modltr
 del pwrsupply, posang, psconv, pssofb, rf, injsys, injctrl
 del screen, tune, sofb, timing, syncd, energy
-del ids, currinfo, bbb, machshift, dvf, lienergy
+del ids, currinfo, bbb, machshift, dvf, lienergy, blctrl
```

### Comparing `siriuspy-2.75.0/siriuspy/devices/bbb.py` & `siriuspy-2.76.0/siriuspy/devices/bbb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/devices/bpm.py` & `siriuspy-2.76.0/siriuspy/devices/bpm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/devices/currinfo.py` & `siriuspy-2.76.0/siriuspy/devices/currinfo.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/devices/dcct.py` & `siriuspy-2.76.0/siriuspy/devices/dcct.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/devices/device.py` & `siriuspy-2.76.0/siriuspy/devices/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,17 @@
     def _create_pvs(self, devname):
         if devname:
             devname = _SiriusPVName(devname)
 
         pvs = dict()
         for propty in self._properties:
             pvname = self._get_pvname(devname, propty)
-            auto_monitor = self._auto_mon or not pvname.endswith('-Mon')
+            # avoid keeping auto_monitor enabled for -Mon PVs as they usually
+            # have a high update rate which can generate a lot of CPU load
+            auto_monitor = self._auto_mon and not pvname.endswith('-Mon')
             in_sim = _Simulation.pv_check(pvname)
             pvclass = _PVSim if in_sim else _PV
             pvs[propty] = pvclass(
                 pvname, auto_monitor=auto_monitor,
                 connection_timeout=Device.CONNECTION_TIMEOUT)
         return devname, pvs
```

### Comparing `siriuspy-2.75.0/siriuspy/devices/dvf.py` & `siriuspy-2.76.0/siriuspy/devices/dvf.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,52 +26,57 @@
         'ACQUISITION_TIME_DEFAULT',  # [s]
         'EXPOSURE_TIME_DEFAULT',  # [s]
         'IMAGE_SIZE_Y',  # [pixel]
         'IMAGE_SIZE_X',  # [pixel]
         'IMAGE_PIXEL_SIZE',  # [um]
         'OPTICS_MAGNIFICATION_FACTOR',  # source to image
     )
-    #   DVF device :       ((sizey, sizex), pixel_size_um mag_factor
+
     _dev2params = {
-        DEVICES.CAX_DVF1 :
-            # DVF1 Today: pixel size 4.8 um; magnification factor 0.5
-            _get_namedtuple('DVFParameters',
-            # _dvfparam_fields, (8, 0.5, 0.5, 0.005, 1024, 1280, 4.8, 0.5)),
-            _dvfparam_fields, (8, 0.5, 0.5, 0.005, 2064, 3088, 2.4, 5.0)),
-        DEVICES.CAX_DVF2 :
-            # DVF2 today: pixel size 4.8 um; magnification factor 5.0
-            # DVF2 future hifi: pixel size 2.4 um; magnification factor 5.0
-            _get_namedtuple('DVFParameters',
-            # _dvfparam_fields, (8, 0.5, 0.5, 0.005, 1024, 1280, 4.8, 5.0)),
-            _dvfparam_fields, (8, 0.5, 0.5, 0.005, 2064, 3088, 2.4, 5.0)),
+        DEVICES.CAX_DVF1:
+            _get_namedtuple(
+                'DVFParameters',
+                _dvfparam_fields, (16, 0.5, 0.5, 0.005, 2064, 3088, 2.4, 5.0)),
+        DEVICES.CAX_DVF2:
+            _get_namedtuple(
+                'DVFParameters',
+                _dvfparam_fields, (16, 0.5, 0.5, 0.005, 2064, 3088, 2.4, 5.0)),
         }
 
     _properties = (
+        'cam1:MaxSizeX_RBV', 'cam1:MaxSizeY_RBV',
         'cam1:ArrayCallbacks', 'cam1:ArrayCallbacks_RBV',
         'cam1:AcquireTime', 'cam1:AcquireTime_RBV',
         'cam1:AcquirePeriod', 'cam1:AcquirePeriod_RBV',
         'cam1:Acquire', 'cam1:Acquire_RBV',
         'cam1:ImageMode', 'cam1:ImageMode_RBV',
         'cam1:Gain', 'cam1:Gain_RBV',
         'cam1:GainAuto', 'cam1:GainAuto_RBV',
+        'cam1:DataType', 'cam1:DataType_RBV',
         'cam1:PixelFormat', 'cam1:PixelFormat_RBV',
         'cam1:PixelSize', 'cam1:PixelSize_RBV',
         'cam1:SizeX_RBV', 'cam1:SizeY_RBV',
         'cam1:Temperature',
+        'cam1:FAILURES_RBV', 'cam1:COMPLETED_RBV',
+        'ROI1:NDArrayPort', 'ROI1:NDArrayPort_RBV',
+        'ROI1:EnableCallbacks', 'ROI1:EnableCallbacks_RBV',
+        'ROI1:MinX', 'ROI1:MinX_RBV',
+        'ROI1:MinY', 'ROI1:MinY_RBV',
+        'ROI1:SizeX', 'ROI1:SizeX_RBV',
+        'ROI1:SizeY', 'ROI1:SizeY_RBV',
+        'ROI1:EnableX', 'ROI1:EnableX_RBV',
+        'ROI1:EnableY', 'ROI1:EnableY_RBV',
+        'ROI1:ArrayCallbacks', 'ROI1:ArrayCallbacks_RBV',
+        'image1:NDArrayPort', 'image1:NDArrayPort_RBV',
         'image1:EnableCallbacks', 'image1:EnableCallbacks_RBV',
         'image1:ArraySize0_RBV', 'image1:ArraySize1_RBV',
         'image1:ArrayData',
         'ffmstream1:EnableCallbacks', 'ffmstream1:EnableCallbacks_RBV',
         'Trans1:EnableCallbacks', 'Trans1:EnableCallbacks_RBV',
         'HDF1:EnableCallbacks', 'HDF1:EnableCallbacks_RBV',
-        # 'Over1:EnableCallbacks', 'Over1:EnableCallbacks_RBV',
-        # 'CC1:EnableCallbacks', 'CC1:EnableCallbacks_RBV',
-        # 'CC1:ColorModeOut', 'CC1:ColorModeOut_RBV',
-        # 'CC1:FalseColor', 'CC1:FalseColor_RBV',
-        # 'DimFei1:EnableCallbacks', 'DimFei1:EnableCallbacks_RBV',
         )
 
     def __init__(self, devname, *args, **kwargs):
         """Init."""
         # check if device exists
         if devname not in DVF.DEVICES.ALL:
             raise NotImplementedError(devname)
@@ -82,17 +87,26 @@
     def parameters(self):
         """Return DVF parameters."""
         return DVF._dev2params[self.devname]
 
     @property
     def intensity_saturation_value(self):
         """Image intensity saturation value."""
-        # NOTE: a PV will be added to the IOC to select nr bits of intensity
-        intensity_nr_bits = self.parameters.MAX_INTENSITY_NR_BITS
-        return 2**intensity_nr_bits - 1
+        pixel_format_to_num_bits = {0: 8, 1: 12}  # 0: 'Mono8, 1: 'Mono12
+        data_type_to_num_bits = {0: 8, 1: 16} # 0: 'UInt8', 1: 'UInt16'
+        used_bits = pixel_format_to_num_bits[self.pixel_format]
+        max_bits = data_type_to_num_bits[self.data_type]
+        max_intensity = (1 << used_bits) - 1
+        if used_bits <= max_bits:
+            # Shift intensity to align with most-significant bits
+            max_intensity <<= max_bits - used_bits
+        elif used_bits > max_bits:
+            # Clip to maximum value allowed by the data type
+            max_intensity = (1 << max_bits) - 1
+        return max_intensity
 
     @property
     def exposure_time(self):
         """Camera exposure time [s]."""
         return self['cam1:AcquireTime']
 
     @exposure_time.setter
@@ -115,24 +129,54 @@
 
     @property
     def acquisition_status(self):
         """Return IOC acquisition status."""
         return self['cam1:Acquire']
 
     @property
+    def cam_max_sizex(self):
+        """Camera max second dimension size (pixels)."""
+        return self['cam1:MaxSizeX_RBV']
+
+    @property
+    def cam_max_sizey(self):
+        """Camera max first dimension size (pixels)."""
+        return self['cam1:MaxSizeY_RBV']
+
+    @property
     def cam_sizex(self):
         """Camera second dimension size (pixels)."""
         return self['cam1:SizeX_RBV']
 
     @property
     def cam_sizey(self):
         """Camera first dimension size (pixels)."""
         return self['cam1:SizeY_RBV']
 
     @property
+    def roi_minx(self):
+        """."""
+        return self['ROI1:MinX_RBV']
+
+    @roi_minx.setter
+    def roi_minx(self, value):
+        """."""
+        self['ROI1:MinX'] = int(value)
+
+    @property
+    def roi_miny(self):
+        """."""
+        return self['ROI1:MinY_RBV']
+
+    @roi_miny.setter
+    def roi_miny(self, value):
+        """."""
+        self['ROI1:MinY'] = int(value)
+
+    @property
     def image_sizex(self):
         """Image second dimension size (pixels)."""
         return self['image1:ArraySize0_RBV']
 
     @property
     def image_sizey(self):
         """Image first dimension size (pixels)."""
@@ -193,42 +237,69 @@
 
     @pixel_format.setter
     def pixel_format(self, value):
         """Set camera pixel format."""
         self['cam1:PixelFormat'] = value
 
     @property
+    def data_type(self):
+        """Return camera data type."""
+        return self['cam1:DataType_RBV']
+
+    @data_type.setter
+    def data_type(self, value):
+        """Set camera data type."""
+        self['cam1:DataType'] = value
+
+    @property
     def pixel_size(self):
         """Return camera pixel size."""
         return self['cam1:PixelSize_RBV']
 
     @pixel_size.setter
     def pixel_size(self, value):
         """Set camera pixel size."""
         self['cam1:PixelSize'] = value
 
     @property
     def cam_temperature(self):
         """Return camera temperature"""
         return self['cam1:Temperature']
 
+    @property
+    def cam_frames_completed(self):
+        """Return number of acquisition frames completed."""
+        return self['cam1:COMPLETED_RBV']
+
+    @property
+    def cam_frames_failures(self):
+        """Return number of acquisition frames failures."""
+        return self['cam1:FAILURES_RBV']
+
     def cmd_reset(self, timeout=None):
         """Reset DVF to a standard configuration."""
         props_values = {
-            'cam1:ArrayCallbacks': 1,  # Enable
+            'cam1:ArrayCallbacks': 1,  # Enable passing array
             'cam1:ImageMode': 2,  # Continuous
+            'cam1:PixelFormat': 1,  # Mono12
+            'cam1:DataType': 1,  # UInt16 (maybe unnecessary)
+            'ROI1:NDArrayPort': 'CAMPORT',  # Take img from camport
+            'ROI1:EnableCallbacks': 1,  # Enable getting from NDArrayPort
+            'ROI1:MinX': 0,  # [pixel]
+            'ROI1:MinY': 0,  # [pixel]
+            'ROI1:SizeX': self.cam_max_sizex,  # [pixel]
+            'ROI1:SizeY': self.cam_max_sizey,  # [pixel]
+            'ROI1:EnableX': 1,  # Enable
+            'ROI1:EnableY': 1,  # Enable
+            'ROI1:ArrayCallbacks': 1,  # Enable passing array
+            'image1:NDArrayPort': 'ROI1',  # image1 takes img from ROI1
             'image1:EnableCallbacks': 1,  # Enable
-            'ffmstream1:EnableCallbacks': 1,  # Enable
-            'HDF1:EnableCallbacks': 1,  # Enable
+            'ffmstream1:EnableCallbacks': 0,  # Disable
+            'HDF1:EnableCallbacks': 0,  # Disable
             'Trans1:EnableCallbacks': 0,  # Disable
-            # 'Over1:EnableCallbacks': 0,  # Disable
-            # 'CC1:EnableCallbacks': 0,  # Disable
-            # 'CC1:ColorModeOut': 0,  # Mono
-            # 'CC1:FalseColor': 0,  # None
-            # 'DimFei1:EnableCallbacks': 0,  # Disable
         }
 
         # set properties
         for propty, value in props_values.items():
             self[propty] = value
 
         # check readback values
@@ -246,14 +317,19 @@
         """Tune IOC image acquisition on."""
         return self._set_and_wait('cam1:Acquire', 1, timeout=timeout)
 
     def cmd_acquire_off(self, timeout=None):
         """Tune IOC image acquisition off."""
         return self._set_and_wait('cam1:Acquire', 0, timeout=timeout)
 
+    @staticmethod
+    def conv_devname2parameters(devname):
+        """."""
+        return DVF._dev2params[devname]
+
     def _set_and_wait(self, propty, value, timeout=None):
         """."""
         timeout = timeout or self._default_timeout
         self[propty] = value
         return self._wait(propty + '_RBV', value, timeout=timeout)
```

### Comparing `siriuspy-2.75.0/siriuspy/devices/egun.py` & `siriuspy-2.76.0/siriuspy/devices/egun.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/devices/energy.py` & `siriuspy-2.76.0/siriuspy/devices/energy.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/devices/fofb.py` & `siriuspy-2.76.0/siriuspy/devices/fofb.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,16 @@
         'RefOrbX-SP', 'RefOrbX-RB',
         'RefOrbY-SP', 'RefOrbY-RB',
         'MaxOrbDistortion-SP', 'MaxOrbDistortion-RB',
         'MaxOrbDistortionEnbl-Sel', 'MaxOrbDistortionEnbl-Sts',
         'MinBPMCnt-SP', 'MinBPMCnt-RB',
         'MinBPMCntEnbl-Sel', 'MinBPMCntEnbl-Sts',
         'LoopIntlk-Mon', 'LoopIntlkReset-Cmd',
+        'SYSIDPRBSFOFBAccEn-Sel', 'SYSIDPRBSFOFBAccEn-Sts',
+        'SYSIDPRBSBPMPosEn-Sel', 'SYSIDPRBSBPMPosEn-Sts',
     )
 
     def __init__(self, devname):
         """Init."""
         # check if device exists
         if devname not in self.DEVICES:
             raise NotImplementedError(devname)
@@ -109,14 +111,32 @@
         return self['MinBPMCntEnbl-Sts']
 
     @min_bpm_count_enbl.setter
     def min_bpm_count_enbl(self, value):
         self['MinBPMCntEnbl-Sel'] = value
 
     @property
+    def sysid_fofbacc_exc_state(self):
+        """SYSID core PRBS excitation enable state for correctors."""
+        return self['SYSIDPRBSFOFBAccEn-Sts']
+
+    @sysid_fofbacc_exc_state.setter
+    def sysid_fofbacc_exc_state(self, value):
+        self['SYSIDPRBSFOFBAccEn-Sel'] = value
+
+    @property
+    def sysid_bpm_exc_state(self):
+        """SYSID core PRBS excitation enable state for BPMs."""
+        return self['SYSIDPRBSBPMPosEn-Sts']
+
+    @sysid_bpm_exc_state.setter
+    def sysid_bpm_exc_state(self, value):
+        self['SYSIDPRBSBPMPosEn-Sel'] = value
+
+    @property
     def interlock(self):
         """Interlock status."""
         return self['LoopIntlk-Mon']
 
     def cmd_reset(self):
         """Reset interlocks."""
         self['LoopIntlkReset-Cmd'] = 1
@@ -273,15 +293,19 @@
         self._bpm_dccs, self._bpm_trgs, self._bpm_ids = dict(), dict(), dict()
         for idx, bpm in enumerate(self._bpmnames):
             self._bpm_ids[bpm] = bpmids[idx]
             self._bpm_dccs[bpm] = BPMDCC(bpm)
             for trig in self.BPM_TRIGS_IDS:
                 trigname = bpm + ':TRIGGER' + str(trig)
                 self._bpm_trgs[trigname] = BPMLogicalTrigger(bpm, trig)
-        bpm2dsbl = ['SI-10SB:DI-BPM-1', 'SI-10SB:DI-BPM-2']
+        bpm2dsbl = [
+            'SI-'+sub+':DI-BPM-'+idx
+            for sub in ['06SB', '07SP', '08SB', '09SA', '10SB', '11SP', '12SB']
+            for idx in ['1', '2']
+        ]
         self._bpmdcc2dsbl = dict()
         for bpm in bpm2dsbl:
             self._bpmdcc2dsbl[bpm] = BPMDCC(bpm)
         # fofb event
         self._evt_fofb = Event('FOFBS')
 
         devices = list()
@@ -645,14 +669,37 @@
             return False
         self._set_devices_propty(devs, 'RcvInSel-SP', rins)
         if not self._wait_devices_propty(
                 devs, 'RcvInSel-RB', rins, timeout=timeout/2):
             return False
         return True
 
+    def check_sysid_exc_disabled(self):
+        """Check whether SYSID excitation is disabled."""
+        if not self.connected:
+            return False
+        for ctl in self._ctl_refs.values():
+            if ctl.sysid_fofbacc_exc_state or ctl.sysid_bpm_exc_state:
+                return False
+        return True
+
+    def cmd_dsbl_sysid_exc(self, timeout=DEF_TIMEOUT):
+        """Command to disable SYSID excitation."""
+        devs = list(self._ctl_refs.values())
+        self._set_devices_propty(devs, 'SYSIDPRBSFOFBAccEn-Sel', 0)
+        if not self._wait_devices_propty(
+                devs, 'SYSIDPRBSFOFBAccEn-Sts', 0, timeout=timeout/2):
+            return False
+        self._set_devices_propty(devs, 'SYSIDPRBSBPMPosEn-Sel', 0)
+        if not self._wait_devices_propty(
+                devs, 'SYSIDPRBSBPMPosEn-Sts', 0, timeout=timeout/2):
+            return False
+        self._evt_fofb.cmd_external_trigger()
+        return True
+
 
 class FamFastCorrs(_Devices):
     """Family of FOFB fast correctors."""
 
     DEF_TIMEOUT = 10  # [s]
     OPMODE_SEL = PowerSupplyFC.OPMODE_SEL
     OPMODE_STS = PowerSupplyFC.OPMODE_STS
@@ -768,14 +815,24 @@
             gain (numpy.ndarray, 160):
                 FOFB pre-accumulator minimum saturation current
                 for each power supply.
         """
         return _np.array([p.fofbacc_satmin for p in self._psdevs])
 
     @property
+    def fofbacc_decimation(self):
+        """FOFB pre-accumulator decimation.
+
+        Returns:
+            counts (numpy.ndarray, 160):
+                FOFB pre-accumulator decimation for each power supply.
+        """
+        return _np.array([p.fofbacc_decimation for p in self._psdevs])
+
+    @property
     def curr_gain(self):
         """Current gain.
 
         Returns:
             gain (numpy.ndarray, 160):
                 current gain for each power supply.
         """
@@ -983,14 +1040,37 @@
         impltd = _np.asarray([d.fofbacc_satmin for d in devs])
         if isinstance(values, (int, float, bool)):
             values = len(devs) * [values]
         if _np.allclose(values, impltd, atol=atol):
             return True
         return False
 
+    def set_fofbacc_decimation(self, values, psnames=None, psindices=None):
+        """Set power supply pre-accumulator decimation."""
+        devs = self._get_devices(psnames, psindices)
+        if isinstance(values, (int, float, bool)):
+            values = len(devs) * [values]
+        for i, dev in enumerate(devs):
+            dev.fofbacc_decimation = values[i]
+        return True
+
+    def check_fofbacc_decimation(
+            self, values, psnames=None, psindices=None,
+            atol=DEF_ATOL_CURRENT_MON):
+        """Check whether power supplies have desired decimation value."""
+        if not self.connected:
+            return False
+        devs = self._get_devices(psnames, psindices)
+        impltd = _np.asarray([d.fofbacc_decimation for d in devs])
+        if isinstance(values, (int, float, bool)):
+            values = len(devs) * [values]
+        if _np.allclose(values, impltd, atol=atol):
+            return True
+        return False
+
     def cmd_fofbacc_clear(self, psnames=None, psindices=None):
         """Send clear power supplies pre-accumulator."""
         for dev in self._get_devices(psnames, psindices):
             dev.cmd_fofbacc_clear()
         return True
 
     # ----- private methods -----
@@ -1030,15 +1110,16 @@
         'CHAccSatMax-SP', 'CHAccSatMax-RB',
         'CVAccSatMax-SP', 'CVAccSatMax-RB',
         'CtrlrStatus-Mon', 'CtrlrConfBPMId-Cmd',
         'CtrlrSyncNet-Cmd', 'CtrlrSyncRefOrb-Cmd',
         'CtrlrSyncTFrameLen-Cmd', 'CtrlrConfBPMLogTrg-Cmd',
         'CtrlrSyncMaxOrbDist-Cmd', 'CtrlrSyncPacketLossDetec-Cmd',
         'CtrlrReset-Cmd',
-        'KickBufferSize-SP', 'KickBufferSize-RB', 'KickBufferSize-Mon',
+        'KickCHAcc-Mon', 'KickCVAcc-Mon',
+        'KickCHRef-Mon', 'KickCVRef-Mon',
         'KickCH-Mon', 'KickCV-Mon',
         'RefOrbX-SP', 'RefOrbX-RB', 'RefOrbY-SP', 'RefOrbY-RB',
         'RefOrbHwX-Mon', 'RefOrbHwY-Mon',
         'BPMXEnblList-SP', 'BPMXEnblList-RB',
         'BPMYEnblList-SP', 'BPMYEnblList-RB',
         'CHEnblList-SP', 'CHEnblList-RB',
         'CVEnblList-SP', 'CVEnblList-RB',
@@ -1246,35 +1327,41 @@
 
     def cmd_fofbctrl_reset(self):
         """Command to reset interlocks of all FOFB controllers."""
         self['CtrlrReset-Cmd'] = 1
         return True
 
     @property
-    def kick_buffer_size_mon(self):
-        """Return actual kicks buffer size."""
-        return self['KickBufferSize-Mon']
+    def kickch_acc(self):
+        """Return CH kicks related to FOFBAcc-Mon PVs."""
+        return self['KickCHAcc-Mon']
+
+    @property
+    def kickcv_acc(self):
+        """Return CV kicks related to FOFBAcc-Mon PVs."""
+        return self['KickCVAcc-Mon']
+
+    @property
+    def kickch_ref(self):
+        """Return CH kicks related to CurrentRef-Mon PVs."""
+        return self['KickCHRef-Mon']
 
     @property
-    def kick_buffer_size(self):
-        """Return kicks buffer size."""
-        return self['KickBufferSize-RB']
-
-    @kick_buffer_size.setter
-    def kick_buffer_size(self, value):
-        self['KickBufferSize-SP'] = max(1, int(value))
+    def kickcv_ref(self):
+        """Return CV kicks related to CurrentRef-Mon PVs."""
+        return self['KickCVRef-Mon']
 
     @property
     def kickch(self):
-        """Return average of CH kicks."""
+        """Return CH kicks related to Current-Mon PVs."""
         return self['KickCH-Mon']
 
     @property
     def kickcv(self):
-        """Return average of CV kicks."""
+        """Return CV kicks related to Current-Mon PVs."""
         return self['KickCV-Mon']
 
     @property
     def refx(self):
         """RefOrb X."""
         return self['RefOrbX-RB']
```

### Comparing `siriuspy-2.75.0/siriuspy/devices/ict.py` & `siriuspy-2.76.0/siriuspy/devices/ict.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/devices/idff.py` & `siriuspy-2.76.0/siriuspy/devices/idff.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,27 +2,23 @@
 
 from ..namesys import SiriusPVName as _SiriusPVName
 from ..search import IDSearch as _IDSearch
 from ..idff.config import IDFFConfig as _IDFFConfig
 
 from .device import Device as _Device, Devices as _Devices
 from .pwrsupply import PowerSupplyFBP as _PowerSupplyFBP
-from .ids import WIG as _WIG, APU as _APU, EPU as _EPU
+from .ids import WIG as _WIG, APU as _APU, PAPU as _PAPU, EPU as _EPU
 
 
 class IDFF(_Devices):
     """Insertion Device Feedforward Device."""
 
-    class DEVICES:
+    class DEVICES(_WIG.DEVICES, _PAPU.DEVICES, _EPU.DEVICES):
         """."""
-        EPU50_10SB = 'SI-10SB:ID-EPU50'
-        WIG180_14SB = 'SI-14SB:ID-WIG180'
-        ALL = (
-            EPU50_10SB, WIG180_14SB,
-            )
+        ALL = _WIG.DEVICES.ALL + _PAPU.DEVICES.ALL + _EPU.DEVICES.ALL
 
     def __init__(self, devname):
         """."""
         devname = _SiriusPVName(devname)
 
         # check if device exists
         if devname not in IDFF.DEVICES.ALL:
@@ -257,14 +253,26 @@
 
     @property
     def gap_mon(self):
         """."""
         return self.kparameter_mon
 
 
+class PAPUIDFF(IDFF):
+    """PAPU Feedforward."""
+
+    class DEVICES(_PAPU.DEVICES):
+        """."""
+
+    @property
+    def phase_mon(self):
+        """."""
+        return self.pparameter_mon
+
+
 class EPUIDFF(IDFF):
     """EPU Feedforward."""
 
     class DEVICES(_EPU.DEVICES):
         """."""
 
     @property
```

### Comparing `siriuspy-2.75.0/siriuspy/devices/ids.py` & `siriuspy-2.76.0/siriuspy/devices/ids.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,80 +99,71 @@
     def wait_move(self):
         """Wait for phase movement to complete."""
         _time.sleep(APU._MOVECHECK_SLEEP)
         while self.is_moving:
             _time.sleep(APU._MOVECHECK_SLEEP)
 
 
-class EPU(_Device):
-    """EPU Insertion Device."""
+class PAPU(_Device):
+    """PAPU Insertion Device."""
 
     class DEVICES:
         """."""
 
-        EPU50_10SB = 'SI-10SB:ID-EPU50'
-        ALL = (EPU50_10SB, )
-
-    # NOTE: move this info to IDSearch?
-    _idparam_fields = (
-        'PERIOD',  # [mm]
-        'PHASE_PARK',  # [mm]
-        'GAP_PARK',  # [mm]
-        )
+        PAPU50_17SA = 'SI-17SA:ID-PAPU50'
+        ALL = (PAPU50_17SA, )
 
-    _dev2params = {
-        DEVICES.EPU50_10SB:
-            _get_namedtuple(
-                'IDParameters', _idparam_fields, (50.0, 0, 300.0)),
-        }
+    TOLERANCE_PHASE = 0.01  # [mm]
 
-    _short_shut_eye = 0.1  # [s]
+    _SHORT_SHUT_EYE = 0.1  # [s]
     _default_timeout = 8  # [s]
 
+    _properties_papu = (
+        'Home-Cmd', 'EnblPwrPhase-Cmd', 'ClearErr-Cmd',
+        'BeamLineCtrl-Mon', 'Home-Mon',
+        )
     _properties = (
+        'PeriodLength-Cte',
         'BeamLineCtrlEnbl-Sel', 'BeamLineCtrlEnbl-Sts',
-        'EnblPwrAll-Cmd', 'PwrPhase-Mon', 'PwrGap-Mon',
+        'Moving-Mon',
+        'PwrPhase-Mon',
         'EnblAndReleasePhase-Sel', 'EnblAndReleasePhase-Sts',
         'AllowedToChangePhase-Mon',
-        'EnblAndReleaseGap-Sel', 'EnblAndReleaseGap-Sts',
-        'AllowedToChangeGap-Mon',
+        'ParkedPhase-Cte',
         'Phase-SP', 'Phase-RB', 'Phase-Mon',
         'PhaseSpeed-SP', 'PhaseSpeed-RB', 'PhaseSpeed-Mon',
         'MaxPhaseSpeed-SP', 'MaxPhaseSpeed-RB',
-        'ChangePhase-Cmd',
-        'Gap-SP', 'Gap-RB', 'Gap-Mon',
-        'GapSpeed-SP', 'GapSpeed-RB', 'GapSpeed-Mon',
-        'MaxGapSpeed-SP', 'MaxGapSpeed-RB',
-        'ChangeGap-Cmd',
-        'Stop-Cmd', 'Moving-Mon', 'IsBusy-Mon',
-        'Status-Mon',
+        'StopPhase-Cmd', 'ChangePhase-Cmd',
+        'Log-Mon',
         )
 
-    def __init__(self, devname):
+
+    def __init__(self, devname, properties=None, auto_mon=True):
         """."""
         devname = _SiriusPVName(devname)
 
         # check if device exists
-        if devname not in EPU.DEVICES.ALL:
+        if devname not in self.DEVICES.ALL:
             raise NotImplementedError(devname)
 
         # call base class constructor
-        super().__init__(devname, properties=EPU._properties, auto_mon=True)
+        properties = properties or self._properties + self._properties_papu
+        super().__init__(devname, properties=properties, auto_mon=auto_mon)
 
     @property
-    def parameters(self):
-        """Return EPU parameters."""
-        return EPU._dev2params[self.devname]
+    def period_length(self):
+        """Return ID period length [mm]."""
+        return self['PeriodLength-Cte']
 
     @property
-    def status(self):
-        """EPU status."""
-        return self['Status-Mon']
+    def log_mon(self):
+        """Return ID Log."""
+        return self['Log-Mon']
 
-    # --- speeds ----
+    # --- phase speeds ----
 
     @property
     def phase_speed(self):
         """Return phase speed readback [mm/s]."""
         return self['PhaseSpeed-RB']
 
     @property
@@ -188,331 +179,225 @@
     @property
     def phase_speed_max_lims(self):
         """."""
         ctrl = self.pv_ctrlvars('MaxPhaseSpeed-SP')
         lims = [ctrl['lower_ctrl_limit'], ctrl['upper_ctrl_limit']]
         return lims
 
-    @property
-    def gap_speed(self):
-        """Return gap speed readback [mm/s]."""
-        return self['GapSpeed-RB']
-
-    @property
-    def gap_speed_mon(self):
-        """Return gap speed monitor [mm/s]."""
-        return self['GapSpeed-Mon']
-
-    @property
-    def gap_speed_max(self):
-        """Return max gap speed readback [mm/s]."""
-        return self['MaxGapSpeed-RB']
+    # --- phase ---
 
     @property
-    def gap_speed_max_lims(self):
-        """."""
-        ctrl = self.pv_ctrlvars('MaxGapSpeed-SP')
-        lims = [ctrl['lower_ctrl_limit'], ctrl['upper_ctrl_limit']]
-        return lims
-
-    # --- phase ---
+    def phase_parked(self):
+        """Return ID parked phase value [mm]."""
+        return self['ParkedPhase-Cte']
 
     @property
     def phase(self):
-        """Return EPU phase readback [mm]."""
+        """Return ID phase readback [mm]."""
         return self['Phase-RB']
 
     @property
     def phase_min(self):
-        """Return EPU phase lower control limit [mm]."""
+        """Return ID phase lower control limit [mm]."""
         ctrlvars = self.pv_ctrlvars('Phase-SP')
         return ctrlvars['lower_ctrl_limit']
 
     @property
     def phase_max(self):
-        """Return EPU phase upper control limit [mm]."""
+        """Return ID phase upper control limit [mm]."""
         ctrlvars = self.pv_ctrlvars('Phase-SP')
         return ctrlvars['upper_ctrl_limit']
 
     @property
     def phase_mon(self):
-        """Return EPU phase monitor [mm]."""
+        """Return ID phase monitor [mm]."""
         return self['Phase-Mon']
 
-    # --- gap ---
-
-    @property
-    def gap(self):
-        """Return EPU gap readback [mm]."""
-        return self['Gap-RB']
-
-    @property
-    def gap_min(self):
-        """Return EPU gap lower control limit [mm]."""
-        ctrlvars = self.pv_ctrlvars('Gap-SP')
-        return ctrlvars['lower_ctrl_limit']
-
-    @property
-    def gap_max(self):
-        """Return EPU gap upper control limit [mm]."""
-        ctrlvars = self.pv_ctrlvars('Gap-SP')
-        return ctrlvars['upper_ctrl_limit']
-
-    @property
-    def gap_mon(self):
-        """Return EPU gap monitor [mm]."""
-        return self['Gap-Mon']
-
     # --- drive checks ---
 
     @property
     def is_phase_drive_powered(self):
         """Return phase driver power state on (True|False)."""
         return self['PwrPhase-Mon'] != 0
 
-    @property
-    def is_gap_drive_powered(self):
-        """Return gap driver power state on (True|False)."""
-        return self['PwrGap-Mon'] != 0
-
-    @property
-    def is_drives_powered(self):
-        """Return phase & gap drives powered state on (True|False)."""
-        return self.is_phase_drive_powered and self.is_gap_drive_powered
-
     # --- movement checks ---
 
     @property
     def is_move_phase_enabled(self):
         """Return phase movement enabled state (True|False)."""
         return self['AllowedToChangePhase-Mon'] != 0
 
     @property
-    def is_move_gap_enabled(self):
-        """Return gap movement enabled state (True|False)."""
-        return self['AllowedToChangeGap-Mon'] != 0
-
-    @property
-    def is_move_enabled(self):
-        """Return phase and gap movements enabled state (True|False)."""
-        return self.is_move_phase_enabled and self.is_move_gap_enabled
-
-    @property
     def is_moving(self):
         """Return is moving state (True|False)."""
         return self['Moving-Mon'] != 0
 
-    # --- other checks ---
-
     @property
-    def is_busy(self):
-        """Return is busy state (True|False)."""
-        return self['IsBusy-Mon'] != 0
+    def is_homing(self):
+        """Return whether ID is in homing procedure (True|False)."""
+        return self['Home-Mon'] != 0
 
     @property
     def is_beamline_ctrl_enabled(self):
         """Return beamline control enabled state (True|False)."""
         return self['BeamLineCtrlEnbl-Sts'] != 0
 
-    # --- cmd_wait
-
-    def cmd_wait_while_busy(self, timeout=None):
-        """Command wait within timeout while EPU control is busy."""
-        timeout = timeout or self._default_timeout
-        time_init = _time.time()
-        while self.is_busy:
-            _time.sleep(min(EPU._short_shut_eye, timeout))
-            if _time.time() - time_init > timeout:
-                return False
-        return True
-
     # --- cmd_beamline and cmd_drive
 
     def cmd_drive_turn_power_on(self, timeout=None):
-        """Command turn phase and gap drives on."""
-        if self.is_phase_drive_powered and self.is_gap_drive_powered:
+        """Command turn phase drive on."""
+        if self.is_phase_drive_powered:
             return True
-        self['EnblPwrAll-Cmd'] = 1
-        props_values = {'PwrPhase-Mon': 1, 'PwrGap-Mon': 1}
+        self['EnblPwrPhase-Cmd'] = 1
+        props_values = {'PwrPhase-Mon': 1}
         return self._wait(props_values, timeout=timeout)
 
     def cmd_beamline_ctrl_enable(self, timeout=None):
-        """Command enable bealine EPU control."""
+        """Command enable bealine ID control."""
         return self._write_sp('BeamLineCtrlEnbl-Sel', 1, timeout)
 
     def cmd_beamline_ctrl_disable(self, timeout=None):
-        """Command disable bealine EPU control."""
+        """Command disable bealine ID control."""
         return self._write_sp('BeamLineCtrlEnbl-Sel', 0, timeout)
 
     # --- cmd_set ---
 
     def cmd_set_phase(self, phase, timeout=None):
-        """Command to set EPU target phase for movement [mm]."""
+        """Command to set ID target phase for movement [mm]."""
         return self._write_sp('Phase-SP', phase, timeout)
 
-    def cmd_set_gap(self, gap, timeout=None):
-        """Command to set EPU target gap for movement [mm]."""
-        return self._write_sp('Gap-SP', gap, timeout)
-
     def cmd_set_phase_speed(self, phase_speed, timeout=None):
-        """Command to set EPU cruise phase speed for movement [mm/s]."""
+        """Command to set ID cruise phase speed for movement [mm/s]."""
         return self._write_sp('PhaseSpeed-SP', phase_speed, timeout)
 
-    def cmd_set_gap_speed(self, gap_speed, timeout=None):
-        """Command to set EPU cruise gap speed for movement [mm/s]."""
-        return self._write_sp('GapSpeed-SP', gap_speed, timeout)
-
     def cmd_set_phase_speed_max(self, phase_speed_max, timeout=None):
-        """Command to set EPU max cruise phase speed for movement [mm/s]."""
+        """Command to set ID max cruise phase speed for movement [mm/s]."""
         return self._write_sp('MaxPhaseSpeed-SP', phase_speed_max, timeout)
 
-    def cmd_set_gap_speed_max(self, gap_speed_max, timeout=None):
-        """Command to set EPU max cruise gap speed for movement [mm/s]."""
-        return self._write_sp('MaxGapSpeed-SP', gap_speed_max, timeout)
-
     # --- cmd_move disable/enable ---
 
     def cmd_move_phase_enable(self, timeout=None):
-        """Command to release and enable EPU phase movement."""
-        # self['EnblAndReleasePhase-Sel'] = 1
-        # return True
+        """Command to release and enable ID phase movement."""
         return self._write_sp('EnblAndReleasePhase-Sel', 1, timeout)
 
     def cmd_move_phase_disable(self, timeout=None):
-        """Command to disable and break EPU phase movement."""
-        # self['EnblAndReleasePhase-Sel'] = 0
-        # return True
+        """Command to disable and break ID phase movement."""
         return self._write_sp('EnblAndReleasePhase-Sel', 0, timeout)
 
-    def cmd_move_gap_enable(self, timeout=None):
-        """Command to release and enable EPU gap movement."""
-        # self['EnblAndReleaseGap-Sel'] = 1
-        # return True
-        return self._write_sp('EnblAndReleaseGap-Sel', 1, timeout)
-
-    def cmd_move_gap_disable(self, timeout=None):
-        """Command to disable and break EPU gap movement."""
-        # self['EnblAndReleaseGap-Sel'] = 0
-        # return True
-        return self._write_sp('EnblAndReleaseGap-Sel', 0, timeout)
-
     def cmd_move_enable(self, timeout=None):
-        """Command to release and enable EPU phase and gap movements."""
-        success = True
-        success &= self.cmd_move_phase_enable(timeout=timeout)
-        success &= self.cmd_move_gap_enable(timeout=timeout)
-        return success
+        """Command to release and enable ID phase and gap movements."""
+        return self.cmd_move_phase_enable(timeout=timeout)
 
     def cmd_move_disable(self, timeout=None):
-        """Command to disable and break EPU phase and gap movements."""
-        success = True
-        success &= self.cmd_move_phase_disable(timeout=timeout)
-        success &= self.cmd_move_gap_disable(timeout=timeout)
-        return success
+        """Command to disable and break ID phase and gap movements."""
+        return self.cmd_move_phase_disable(timeout=timeout)
+
+    # --- cmd_wait
+
+    def wait_while_busy(self, timeout=None):
+        """Command wait within timeout while ID control is busy."""
+        return True
+
+    def wait_move_start(self, timeout=None):
+        """Command wait until movement starts or timeout."""
+        time_init = _time.time()
+        while not self.is_moving:
+            if timeout is not None and _time.time() - time_init > timeout:
+                return False
+        return True
 
     # -- cmd_move
 
     def cmd_move_stop(self, timeout=None):
-        """Command to interrupt and then enable phase and gap movements."""
+        """Command to interrupt and then enable phase movements."""
         timeout = timeout or self._default_timeout
 
         # wait for not busy state
-        if not self.cmd_wait_while_busy(timeout=timeout):
+        if not self.wait_while_busy(timeout=timeout):
             return False
 
         # send stop command
         self.cmd_move_disable()
-        # self['Stop-Cmd'] = 1
 
         # check for successful stop
-        if not self.cmd_wait_while_busy(timeout=timeout):
+        if not self.wait_while_busy(timeout=timeout):
             return False
         success = True
         success &= super()._wait('Moving-Mon', 0, timeout=timeout)
-        success &= super()._wait('IsBusy-Mon', 0, timeout=timeout)
         if not success:
             return False
 
         # enable movement again
         return self.cmd_move_enable(timeout=timeout)
 
     def cmd_move_phase_start(self, timeout=None):
         """Command to start phase movement."""
         return self._move_start('ChangePhase-Cmd', timeout=timeout)
 
-    def cmd_move_gap_start(self, timeout=None):
-        """Command to start gap movement."""
-        return self._move_start('ChangeGap-Cmd', timeout=timeout)
-
-    def cmd_move(self, phase, gap, timeout=None):
-        """Command to set and start phase and gap movements."""
+    def cmd_move(self, phase, timeout=None):
+        """Command to set and start phase movements."""
         # calc ETA
-        dtime_phase = abs(phase - self.phase_mon) / self.phase_speed
-        dtime_gap = abs(gap - self.gap_mon) / self.gap_speed
-        dtime_max = max(dtime_phase, dtime_gap)
+        dtime_max = abs(phase - self.phase_mon) / self.phase_speed
 
         # additional percentual in ETA
-        tol_gap = 0.01  # [mm]
-        tol_phase = 0.01  # [mm]
         tol_dtime = 300  # [%]
         tol_factor = (1 + tol_dtime/100)
         tol_total = tol_factor * dtime_max + 5
 
         # set target phase and gap
         if not self.cmd_set_phase(phase=phase, timeout=timeout):
             return False
-        if not self.cmd_set_gap(gap=gap, timeout=timeout):
-            return False
 
         # command move start
         if not self.cmd_move_phase_start(timeout=timeout):
             return False
-        if not self.cmd_move_gap_start(timeout=timeout):
-            return False
 
         # wait for movement within reasonable time
         time_init = _time.time()
         while \
-                abs(self.gap_mon - gap) > tol_gap or \
-                abs(self.phase_mon - phase) > tol_phase or \
+                abs(self.phase_mon - phase) > PAPU.TOLERANCE_PHASE or \
                 self.is_moving:
             if _time.time() - time_init > tol_total:
                 print(f'tol_total: {tol_total:.3f} s')
                 print(f'wait_time: {_time.time() - time_init:.3f} s')
                 print()
                 return False
-            _time.sleep(EPU._short_shut_eye)
+            _time.sleep(self._SHORT_SHUT_EYE)
 
         # successfull movement at this point
         return True
 
     def cmd_move_park(self, timeout=None):
-        """Command to set and start EPU movement to parked config."""
-        params = self.parameters
-        return self.cmd_move(
-            params.PHASE_PARK, params.GAP_PARK, timeout=timeout)
+        """Command to set and start ID movement to parked config."""
+        return self.cmd_move(self.phase_parked, timeout=timeout)
 
     # --- cmd_reset
 
     def cmd_device_reset(self, timeout=None):
-        """Command to reset EPU to a standard movement state."""
+        """Command to reset ID to a standard movement state."""
         success = True
         success &= self.cmd_beamline_ctrl_disable(timeout=timeout)
         success &= self.cmd_drive_turn_power_on(timeout=timeout)
         success &= self.cmd_move_enable(timeout=timeout)
         return success
 
+    # --- other cmds ---
+
+    def cmd_clear_error(self):
+        """."""
+        self['ClearErr-Cmd'] = 1
+
     # --- private methods ---
 
     def _move_start(self, cmd_propty, timeout=None):
         """."""
         timeout = timeout or self._default_timeout
 
         # wait for not busy state
-        if not self.cmd_wait_while_busy(timeout=timeout):
+        if not self.wait_while_busy(timeout=timeout):
             return False
 
         # send move command
         self[cmd_propty] = 1
 
         return True
 
@@ -522,15 +407,15 @@
             propties_sp = (propties_sp, )
             values = (values, )
         success = True
         for propty_sp, value in zip(propties_sp, values):
             propty_rb = propty_sp.replace('-SP', '-RB').replace('-Sel', '-Sts')
             # if self[propty_rb] == value:
             #     continue
-            if not self.cmd_wait_while_busy(timeout=timeout):
+            if not self.wait_while_busy(timeout=timeout):
                 return False
             self[propty_sp] = value
             success &= super()._wait(
                 propty_rb, value, timeout=timeout, comp='eq')
         return success
 
     def _wait(self, props_values, timeout=None, comp='eq'):
@@ -538,14 +423,261 @@
         success = True
         for propty, value in props_values.items():
             success &= super()._wait(
                 propty, value, timeout=timeout, comp=comp)
         return success
 
 
+class EPU(PAPU):
+    """EPU Insertion Device."""
+
+    class DEVICES:
+        """."""
+
+        EPU50_10SB = 'SI-10SB:ID-EPU50'
+        ALL = (EPU50_10SB, )
+
+    _properties = PAPU._properties + (
+        'EnblPwrAll-Cmd',
+        'PwrGap-Mon',
+        'Status-Mon',
+        'EnblAndReleaseGap-Sel', 'EnblAndReleaseGap-Sts',
+        'AllowedToChangeGap-Mon',
+        'ParkedGap-Cte', 'IsBusy-Mon',
+        'Gap-SP', 'Gap-RB', 'Gap-Mon',
+        'GapSpeed-SP', 'GapSpeed-RB', 'GapSpeed-Mon',
+        'MaxGapSpeed-SP', 'MaxGapSpeed-RB',
+        'ChangeGap-Cmd', 'Stop-Cmd',
+        )
+
+    def __init__(self, devname):
+        """."""
+        devname = _SiriusPVName(devname)
+
+        # check if device exists
+        if devname not in EPU.DEVICES.ALL:
+            raise NotImplementedError(devname)
+
+        # call base class constructor
+        super().__init__(devname, properties=self._properties, auto_mon=True)
+
+    @property
+    def status(self):
+        """ID status."""
+        return self['Status-Mon']
+
+    # --- gap speeds ----
+
+    @property
+    def gap_parked(self):
+        """Return ID parked gap value [mm]."""
+        return self['ParkedGap-Cte']
+
+    @property
+    def gap_speed(self):
+        """Return gap speed readback [mm/s]."""
+        return self['GapSpeed-RB']
+
+    @property
+    def gap_speed_mon(self):
+        """Return gap speed monitor [mm/s]."""
+        return self['GapSpeed-Mon']
+
+    @property
+    def gap_speed_max(self):
+        """Return max gap speed readback [mm/s]."""
+        return self['MaxGapSpeed-RB']
+
+    @property
+    def gap_speed_max_lims(self):
+        """."""
+        ctrl = self.pv_ctrlvars('MaxGapSpeed-SP')
+        lims = [ctrl['lower_ctrl_limit'], ctrl['upper_ctrl_limit']]
+        return lims
+
+    # --- gap ---
+
+    @property
+    def gap(self):
+        """Return ID gap readback [mm]."""
+        return self['Gap-RB']
+
+    @property
+    def gap_min(self):
+        """Return ID gap lower control limit [mm]."""
+        ctrlvars = self.pv_ctrlvars('Gap-SP')
+        return ctrlvars['lower_ctrl_limit']
+
+    @property
+    def gap_max(self):
+        """Return ID gap upper control limit [mm]."""
+        ctrlvars = self.pv_ctrlvars('Gap-SP')
+        return ctrlvars['upper_ctrl_limit']
+
+    @property
+    def gap_mon(self):
+        """Return ID gap monitor [mm]."""
+        return self['Gap-Mon']
+
+    # --- drive checks ---
+
+    @property
+    def is_gap_drive_powered(self):
+        """Return gap driver power state on (True|False)."""
+        return self['PwrGap-Mon'] != 0
+
+    @property
+    def is_drives_powered(self):
+        """Return phase & gap drives powered state on (True|False)."""
+        return self.is_phase_drive_powered and self.is_gap_drive_powered
+
+    # --- movement checks ---
+
+    @property
+    def is_move_gap_enabled(self):
+        """Return gap movement enabled state (True|False)."""
+        return self['AllowedToChangeGap-Mon'] != 0
+
+    @property
+    def is_move_enabled(self):
+        """Return phase and gap movements enabled state (True|False)."""
+        return self.is_move_phase_enabled and self.is_move_gap_enabled
+
+    @property
+    def is_homing(self):
+        """Return whether ID is in homing procedure."""
+        return False
+
+    # --- other checks ---
+
+    @property
+    def is_busy(self):
+        """Return is busy state (True|False)."""
+        return self['IsBusy-Mon'] != 0
+
+    # --- cmd_beamline and cmd_drive
+
+    def cmd_drive_turn_power_on(self, timeout=None):
+        """Command turn phase and gap drives on."""
+        if self.is_phase_drive_powered and self.is_gap_drive_powered:
+            return True
+        self['EnblPwrAll-Cmd'] = 1
+        props_values = {'PwrPhase-Mon': 1, 'PwrGap-Mon': 1}
+        return self._wait(props_values, timeout=timeout)
+
+    # --- cmd_set ---
+
+    def cmd_set_gap(self, gap, timeout=None):
+        """Command to set ID target gap for movement [mm]."""
+        return self._write_sp('Gap-SP', gap, timeout)
+
+    def cmd_set_gap_speed(self, gap_speed, timeout=None):
+        """Command to set ID cruise gap speed for movement [mm/s]."""
+        return self._write_sp('GapSpeed-SP', gap_speed, timeout)
+
+    def cmd_set_gap_speed_max(self, gap_speed_max, timeout=None):
+        """Command to set ID max cruise gap speed for movement [mm/s]."""
+        return self._write_sp('MaxGapSpeed-SP', gap_speed_max, timeout)
+
+    # --- cmd_move disable/enable ---
+
+    def cmd_move_gap_enable(self, timeout=None):
+        """Command to release and enable ID gap movement."""
+        return self._write_sp('EnblAndReleaseGap-Sel', 1, timeout)
+
+    def cmd_move_gap_disable(self, timeout=None):
+        """Command to disable and break ID gap movement."""
+        return self._write_sp('EnblAndReleaseGap-Sel', 0, timeout)
+
+    def cmd_move_enable(self, timeout=None):
+        """Command to release and enable ID phase and gap movements."""
+        success = True
+        success &= self.cmd_move_phase_enable(timeout=timeout)
+        success &= self.cmd_move_gap_enable(timeout=timeout)
+        return success
+
+    def cmd_move_disable(self, timeout=None):
+        """Command to disable and break ID phase and gap movements."""
+        success = True
+        success &= self.cmd_move_phase_disable(timeout=timeout)
+        success &= self.cmd_move_gap_disable(timeout=timeout)
+        return success
+
+    # --- cmd_wait
+
+    def wait_while_busy(self, timeout=None):
+        """Command wait within timeout while ID control is busy."""
+        timeout = timeout or self._default_timeout
+        time_init = _time.time()
+        while self.is_busy:
+            _time.sleep(min(self._SHORT_SHUT_EYE, timeout))
+            if _time.time() - time_init > timeout:
+                return False
+        return True
+
+    # -- cmd_move
+
+    def cmd_move_gap_start(self, timeout=None):
+        """Command to start gap movement."""
+        return self._move_start('ChangeGap-Cmd', timeout=timeout)
+
+    def cmd_move(self, phase, gap, timeout=None):
+        """Command to set and start phase and gap movements."""
+        # calc ETA
+        dtime_phase = abs(phase - self.phase_mon) / self.phase_speed
+        dtime_gap = abs(gap - self.gap_mon) / self.gap_speed
+        dtime_max = max(dtime_phase, dtime_gap)
+
+        # additional percentual in ETA
+        tol_gap = 0.01  # [mm]
+        tol_phase = 0.01  # [mm]
+        tol_dtime = 300  # [%]
+        tol_factor = (1 + tol_dtime/100)
+        tol_total = tol_factor * dtime_max + 5
+
+        # set target phase and gap
+        if not self.cmd_set_phase(phase=phase, timeout=timeout):
+            return False
+        if not self.cmd_set_gap(gap=gap, timeout=timeout):
+            return False
+
+        # command move start
+        if not self.cmd_move_phase_start(timeout=timeout):
+            return False
+        if not self.cmd_move_gap_start(timeout=timeout):
+            return False
+
+        # wait for movement within reasonable time
+        time_init = _time.time()
+        while \
+                abs(self.gap_mon - gap) > tol_gap or \
+                abs(self.phase_mon - phase) > tol_phase or \
+                self.is_moving:
+            if _time.time() - time_init > tol_total:
+                print(f'tol_total: {tol_total:.3f} s')
+                print(f'wait_time: {_time.time() - time_init:.3f} s')
+                print()
+                return False
+            _time.sleep(EPU._SHORT_SHUT_EYE)
+
+        # successfull movement at this point
+        return True
+
+    def cmd_move_park(self, timeout=None):
+        """Command to set and start ID movement to parked config."""
+        return self.cmd_move(
+            self.phase_parked, self.gap_parked, timeout=timeout)
+
+    # --- other cmds ---
+
+    def cmd_clear_error(self):
+        """."""
+        pass
+
+
 class WIG(_Device):
     """Wiggler Insertion Device."""
 
     class DEVICES:
         """."""
         WIG180_14SB = 'SI-14SB:ID-WIG180'
         ALL = (WIG180_14SB, )
```

### Comparing `siriuspy-2.75.0/siriuspy/devices/injctrl.py` & `siriuspy-2.76.0/siriuspy/devices/injctrl.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/devices/injsys.py` & `siriuspy-2.76.0/siriuspy/devices/injsys.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/devices/lienergy.py` & `siriuspy-2.76.0/siriuspy/devices/lienergy.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/devices/lillrf.py` & `siriuspy-2.76.0/siriuspy/devices/lillrf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/devices/machshift.py` & `siriuspy-2.76.0/siriuspy/devices/machshift.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/devices/modltr.py` & `siriuspy-2.76.0/siriuspy/devices/modltr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/devices/orbit_interlock.py` & `siriuspy-2.76.0/siriuspy/devices/orbit_interlock.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/devices/posang.py` & `siriuspy-2.76.0/siriuspy/devices/posang.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/devices/psconv.py` & `siriuspy-2.76.0/siriuspy/devices/psconv.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/devices/pssofb.py` & `siriuspy-2.76.0/siriuspy/devices/pssofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/devices/pstesters.py` & `siriuspy-2.76.0/siriuspy/devices/pstesters.py`

 * *Files 4% similar despite different names*

```diff
@@ -428,28 +428,32 @@
         return abs(value - target) < self.test_tol
 
 
 class TesterPSFOFB(_TesterBase):
     """FOFB PS tester."""
 
     _properties = (
-        'AlarmsAmp-Mon',
+        'AlarmsAmp-Mon', 'AlarmsAmpLtcRst-Cmd',
         'PwrState-Sel', 'PwrState-Sts',
         'Current-SP', 'CurrentRef-Mon', 'Current-Mon',
         'OpMode-Sel', 'OpMode-Sts',
     )
 
     def __init__(self, devname):
         """Init."""
         super().__init__(devname, properties=TesterPSFOFB._properties)
 
         splims = _PSSearch.conv_psname_2_splims(devname)
         self.test_current = splims['TSTV']
         self.test_tol = splims['TSTR']
 
+    def reset(self):
+        """Reset."""
+        self['AlarmsAmpLtcRst-Cmd'] = 1
+
     def set_opmode(self, state):
         """Set opmode to 'state'."""
         self['OpMode-Sel'] = state
 
     def check_opmode(self, state):
         """Check whether power supply is in opmode 'state'."""
         if isinstance(state, (list, tuple)):
```

### Comparing `siriuspy-2.75.0/siriuspy/devices/pwrsupply.py` & `siriuspy-2.76.0/siriuspy/devices/pwrsupply.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,16 @@
         'InvRespMatRowX-SP', 'InvRespMatRowX-RB',
         'InvRespMatRowY-SP', 'InvRespMatRowY-RB',
         'FOFBAccGain-SP', 'FOFBAccGain-RB',
         'FOFBAccFreeze-Sel', 'FOFBAccFreeze-Sts',
         'FOFBAccClear-Cmd',
         'FOFBAccSatMax-SP', 'FOFBAccSatMax-RB',
         'FOFBAccSatMin-SP', 'FOFBAccSatMin-RB',
+        'FOFBAcc-Mon',
+        'FOFBAccDecimation-SP', 'FOFBAccDecimation-RB',
     )
     _properties_pulsed = (
         'Voltage-SP', 'Voltage-RB', 'Voltage-Mon',
         'Pulse-Sel', 'Pulse-Sts')
     _properties_pulsed_sept = (
         'Intlk1-Mon', 'Intlk2-Mon', 'Intlk3-Mon', 'Intlk4-Mon',
         'Intlk5-Mon', 'Intlk6-Mon', 'Intlk7-Mon',
@@ -966,14 +968,28 @@
         """FOFB accumulator minimum saturation."""
         return self['FOFBAccSatMin-RB']
 
     @fofbacc_satmin.setter
     def fofbacc_satmin(self, value):
         self['FOFBAccSatMin-SP'] = value
 
+    @property
+    def fofbacc_mon(self):
+        """FOFB accumulator."""
+        return self['FOFBAcc-Mon']
+
+    @property
+    def fofbacc_decimation(self):
+        """FOFB accumulator decimation."""
+        return self['FOFBAccDecimation-RB']
+
+    @fofbacc_decimation.setter
+    def fofbacc_decimation(self, value):
+        self['FOFBAccDecimation-SP'] = value
+
     def cmd_fofbacc_clear(self):
         """Command to clear FOFB accumulator."""
         self['FOFBAccClear-Cmd'] = 1
         return True
 
 
 class PowerSupplyFBP(PowerSupply):
```

### Comparing `siriuspy-2.75.0/siriuspy/devices/rf.py` & `siriuspy-2.76.0/siriuspy/devices/rf.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/devices/screen.py` & `siriuspy-2.76.0/siriuspy/devices/screen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/devices/sofb.py` & `siriuspy-2.76.0/siriuspy/devices/sofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/devices/syncd.py` & `siriuspy-2.76.0/siriuspy/devices/syncd.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/devices/timing.py` & `siriuspy-2.76.0/siriuspy/devices/timing.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/devices/tune.py` & `siriuspy-2.76.0/siriuspy/devices/tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/diagbeam/bpm/csdev.py` & `siriuspy-2.76.0/siriuspy/diagbeam/bpm/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/diagbeam/dcct/csdev.py` & `siriuspy-2.76.0/siriuspy/diagbeam/dcct/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/diagbeam/ict/csdev.py` & `siriuspy-2.76.0/siriuspy/diagbeam/ict/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/diagbeam/screen/csdev.py` & `siriuspy-2.76.0/siriuspy/diagbeam/screen/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/diagbeam/slit/csdev.py` & `siriuspy-2.76.0/siriuspy/diagbeam/slit/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/diagsys/app.py` & `siriuspy-2.76.0/siriuspy/diagsys/app.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/diagsys/lidiag/csdev.py` & `siriuspy-2.76.0/siriuspy/diagsys/lidiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/diagsys/lidiag/main.py` & `siriuspy-2.76.0/siriuspy/diagsys/lidiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/diagsys/lidiag/pvs.py` & `siriuspy-2.76.0/siriuspy/diagsys/lidiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/diagsys/psdiag/csdev.py` & `siriuspy-2.76.0/siriuspy/diagsys/psdiag/csdev.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,42 +11,50 @@
     DIAG_STATUS_LABELS_AS = (
         'PS Disconnected/Comm. Broken',
         'PwrState-Sts Off',
         'Current-(SP|Mon) are different',
         'Interlocks',
         'Alarms',
         'OpMode-(Sel|Sts) are different',
-        'Reserved')
+        'Reserved',
+        'Reserved',
+        )
 
     DIAG_STATUS_LABELS_LI = (
         'PS Disconnected/Comm. Broken',
         'PwrState-Sts Off',
         'Current-(SP|Mon) are different',
         'Interlocks',
         'Reserved',
         'Reserved',
-        'Reserved')
+        'Reserved',
+        'Reserved',
+        )
 
     DIAG_STATUS_LABELS_FC = (
         'PS Disconnected',
         'PwrState-Sts Off',
-        'Current-(SP|RB) are different',
+        'Current-(SP|Ref-Mon|Mon) are different',
         'Reserved',
         'Alarms',
         'OpMode-(Sel|Sts) are different',
-        'Reserved')
+        'Reserved',
+        'Triggered mode enabled',
+        )
 
     DIAG_STATUS_LABELS_BO = (
         'PS Disconnected/Comm. Broken',
         'PwrState-Sts Off',
         'Current-(SP|Mon) are different',
         'Interlocks',
         'Alarms',
         'OpMode-(Sel|Sts) are different',
-        'Wfm error exceeded tolerance')
+        'Wfm error exceeded tolerance',
+        'Reserved',
+        )
 
 
 _et = ETypes  # syntactic sugar
 
 
 def get_ps_diag_status_labels(psname):
     """Return Diag Status Labels enum."""
```

### Comparing `siriuspy-2.75.0/siriuspy/diagsys/psdiag/main.py` & `siriuspy-2.76.0/siriuspy/diagsys/psdiag/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,17 +15,21 @@
 
     def _create_computed_pvs(self, psnames):
         self._psnames = psnames
         for psname in self._psnames:
             devname = SiriusPVName(psname).substitute(prefix=self._prefix)
 
             # DiagCurrentDiff-Mon
-            pvs = [None, None]
+            nrpvs = 4 if devname.sec != 'LI' else 2
+            pvs = [None]*nrpvs
             pvs[_PSDiffPV.CURRT_SP] = devname + ':Current-SP'
             pvs[_PSDiffPV.CURRT_MON] = devname + ':Current-Mon'
+            if devname.sec != 'LI':
+                pvs[_PSDiffPV.CURRT_REF] = devname + ':CurrentRef-Mon'
+                pvs[_PSDiffPV.OPMODESTS] = devname + ':OpMode-Sts'
             pvo = _ComputedPV(
                 psname + ':DiagCurrentDiff-Mon', _PSDiffPV(), self._queue,
                 pvs, monitor=False)
             self.pvs.append(pvo)
 
             # DiagStatus-Mon
             computer = _PSStatusPV()
@@ -38,22 +42,24 @@
                     for aux in ['a', 'b', 'c']:
                         intlk_list.extend(
                             [aux+':'+ilk for ilk in intlks if 'Intlk' in ilk
                              if 'Soft' not in ilk and 'Hard' not in ilk])
                         alarm_list.extend(
                             [aux+':'+alm for alm in intlks if 'Alarm' in alm])
 
-                nbpvs = 4 if psname.dev in ['FCH', 'FCV'] else 5
+                nbpvs = 5
                 pvs = [None]*(nbpvs+len(intlk_list)+len(alarm_list))
                 pvs[_PSStatusPV.PWRSTE_STS] = devname + ':PwrState-Sts'
                 pvs[_PSStatusPV.CURRT_DIFF] = devname + ':DiagCurrentDiff-Mon'
                 pvs[_PSStatusPV.OPMODE_SEL] = devname + ':OpMode-Sel'
                 pvs[_PSStatusPV.OPMODE_STS] = devname + ':OpMode-Sts'
                 if psname.dev not in ['FCH', 'FCV']:
                     pvs[_PSStatusPV.WAVFRM_MON] = devname + ':Wfm-Mon'
+                else:
+                    pvs[_PSStatusPV.TRIGEN_STS] = devname + ':TrigEn-Sts'
 
                 computer.INTLK_PVS = list()
                 for idx, intlk in enumerate(intlk_list):
                     pvidx = idx + nbpvs
                     computer.INTLK_PVS.append(pvidx)
                     pvs[pvidx] = devname + intlk
                 computer.ALARM_PVS = list()
```

### Comparing `siriuspy-2.75.0/siriuspy/diagsys/psdiag/pvs.py` & `siriuspy-2.76.0/siriuspy/diagsys/psdiag/pvs.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,47 +11,62 @@
 
 
 class PSDiffPV:
     """Diff of a PS current setpoint and a readback."""
 
     CURRT_SP = 0
     CURRT_MON = 1
+    CURRT_REF = 2
+    OPMODESTS = 3
 
     def compute_update(self, computed_pv, updated_pv_name, value):
         """Compute difference between SP and Mon current values."""
-        disconnected = \
+        psname = _PVName(computed_pv.pvs[0].pvname).device_name
+        disconn = \
             not computed_pv.pvs[PSDiffPV.CURRT_SP].connected or \
             not computed_pv.pvs[PSDiffPV.CURRT_MON].connected
-        if disconnected:
+        if psname.dev in ['FCH', 'FCV']:
+            disconn |= not computed_pv.pvs[PSDiffPV.CURRT_REF].connected
+            disconn |= not computed_pv.pvs[PSDiffPV.OPMODESTS].connected
+        if disconn:
             return None
+
         value_sp = computed_pv.pvs[PSDiffPV.CURRT_SP].value
         value_mon = computed_pv.pvs[PSDiffPV.CURRT_MON].value
         diff = value_mon - value_sp
+        if psname.dev in ['FCH', 'FCV']:
+            opmode = computed_pv.pvs[PSDiffPV.OPMODESTS].value
+            if opmode == _PSConst.OpModeFOFBSts.fofb:
+                value_ref = computed_pv.pvs[PSDiffPV.CURRT_REF].value
+                diff = value_mon - value_ref
+
         return {'value': diff}
 
 
 class PSStatusPV:
     """Power Supply Status PV."""
 
-    BIT_PSCONNECT = 0b0000001
-    BIT_PWRSTATON = 0b0000010
-    BIT_CURRTDIFF = 0b0000100
-    BIT_INTERLOCK = 0b0001000
-    BIT_ALARMSSET = 0b0010000
-    BIT_OPMODEDIF = 0b0100000
-    BIT_BOWFMDIFF = 0b1000000
+    BIT_PSCONNECT = 0b00000001
+    BIT_PWRSTATON = 0b00000010
+    BIT_CURRTDIFF = 0b00000100
+    BIT_INTERLOCK = 0b00001000
+    BIT_ALARMSSET = 0b00010000
+    BIT_OPMODEDIF = 0b00100000
+    BIT_BOWFMDIFF = 0b01000000
+    BIT_TRIGMDENB = 0b10000000
 
     PWRSTE_STS = 0
     CURRT_DIFF = 1
     INTRLCK_LI = 2
     WARNSTS_LI = 3
     CONNCTD_LI = 4
     OPMODE_SEL = 2
     OPMODE_STS = 3
     WAVFRM_MON = 4
+    TRIGEN_STS = 4
 
     DTOLWFM_DICT = dict()
 
     def __init__(self):
         """Init attributs."""
         self.INTLK_PVS = list()
         self.ALARM_PVS = list()
@@ -95,14 +110,15 @@
             value |= PSStatusPV.BIT_PSCONNECT
             value |= PSStatusPV.BIT_PWRSTATON
             value |= PSStatusPV.BIT_CURRTDIFF
             value |= PSStatusPV.BIT_INTERLOCK
             value |= PSStatusPV.BIT_ALARMSSET
             value |= PSStatusPV.BIT_OPMODEDIF
             value |= PSStatusPV.BIT_BOWFMDIFF
+            value |= PSStatusPV.BIT_TRIGMDENB
             return {'value': value}
 
         # pwrstate?
         pwrsts = computed_pv.pvs[PSStatusPV.PWRSTE_STS].value
         if pwrsts != _PSConst.PwrStateSts.On or pwrsts is None:
             value |= PSStatusPV.BIT_PWRSTATON
 
@@ -110,15 +126,17 @@
             # opmode?
             sel = computed_pv.pvs[PSStatusPV.OPMODE_SEL].value
             sts = computed_pv.pvs[PSStatusPV.OPMODE_STS].value
             if sel is not None and sts is not None:
                 if psname.dev in ['FCH', 'FCV']:
                     opmode_sel = _ETypes.FOFB_OPMODES_SEL[sel]
                     opmode_sts = _ETypes.FOFB_OPMODES_STS[sts]
-                    checkdiff = sts == _PSConst.OpModeFOFBSts.manual
+                    checkdiff = sts in [
+                        _PSConst.OpModeFOFBSts.manual,
+                        _PSConst.OpModeFOFBSts.fofb]
                 else:
                     opmode_sel = _ETypes.OPMODES[sel]
                     opmode_sts = _ETypes.STATES[sts]
                     checkdiff = sts == _PSConst.States.SlowRef
                 if opmode_sel != opmode_sts:
                     value |= PSStatusPV.BIT_OPMODEDIF
                 # current-diff?
@@ -149,14 +167,20 @@
             # alarms?
             for alarm in self.ALARM_PVS:
                 alarmval = computed_pv.pvs[alarm].value
                 if alarmval != 0 or alarmval is None:
                     value |= PSStatusPV.BIT_ALARMSSET
                     break
 
+            # triggered mode enable?
+            if psname.dev in ['FCH', 'FCV']:
+                trigen = computed_pv.pvs[PSStatusPV.TRIGEN_STS].value
+                if trigen or trigen is None:
+                    value |= PSStatusPV.BIT_TRIGMDENB
+
         else:
             # current-diff?
             severity = computed_pv.pvs[PSStatusPV.CURRT_DIFF].severity
             if severity != 0:
                 value |= PSStatusPV.BIT_CURRTDIFF
 
             # interlocks?
```

### Comparing `siriuspy-2.75.0/siriuspy/diagsys/pudiag/csdev.py` & `siriuspy-2.76.0/siriuspy/diagsys/pudiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/diagsys/pudiag/main.py` & `siriuspy-2.76.0/siriuspy/diagsys/pudiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/diagsys/pudiag/pvs.py` & `siriuspy-2.76.0/siriuspy/diagsys/pudiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/diagsys/pvs.py` & `siriuspy-2.76.0/siriuspy/diagsys/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/diagsys/rfdiag/csdev.py` & `siriuspy-2.76.0/siriuspy/diagsys/rfdiag/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/diagsys/rfdiag/main.py` & `siriuspy-2.76.0/siriuspy/diagsys/rfdiag/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/diagsys/rfdiag/pvs.py` & `siriuspy-2.76.0/siriuspy/diagsys/rfdiag/pvs.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/envars.py` & `siriuspy-2.76.0/siriuspy/envars.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/epics/multiproc.py` & `siriuspy-2.76.0/siriuspy/epics/multiproc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/epics/properties.py` & `siriuspy-2.76.0/siriuspy/epics/properties.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/epics/pv_fake.py` & `siriuspy-2.76.0/siriuspy/epics/pv_fake.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/epics/pv_time_serie.py` & `siriuspy-2.76.0/siriuspy/epics/pv_time_serie.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/fofb/csdev.py` & `siriuspy-2.76.0/siriuspy/fofb/csdev.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Define PVs, contants and properties of High Level FOFB."""
 
 import os as _os
+import numpy as _np
 
 from .. import csdev as _csdev
 from ..search import PSSearch as _PSSearch, MASearch as _MASearch, \
     BPMSearch as _BPMSearch
 
 
 NR_BPM = 160
@@ -20,34 +21,36 @@
     GLOB_INDIV = ('Global', 'Individual')
 
     MEAS_RMAT_CMD = ('Start', 'Stop', 'Reset')
     MEAS_RMAT_MON = ('Idle', 'Measuring', 'Completed', 'Aborted')
 
     STS_LBLS_CORR = (
         'Connected', 'PwrStateOn', 'OpModeConfigured', 'AccFreezeConfigured',
-        'InvRespMatRowSynced', 'AccGainSynced', 'AccSatLimsSynced')
+        'InvRespMatRowSynced', 'AccGainSynced', 'AccSatLimsSynced',
+        'AccDecimationSynced')
     STS_LBLS_FOFBCTRL = (
         'Connected', 'BPMIdsConfigured', 'NetSynced', 'LinkPartnerConnected',
         'RefOrbSynced', 'TimeFrameLenSynced', 'BPMLogTrigsConfigured',
         'OrbDistortionDetectionSynced', 'PacketLossDetectionSynced',
-        'LoopInterlockOk')
+        'LoopInterlockOk', 'SYSIDExcitationDisabled')
+
+    DEC_OPT = ('FOFB', 'Monit', 'Custom')
 
 
 _et = ETypes  # syntactic sugar
 
 
 # --- Const class ---
 
 class HLFOFBConst(_csdev.Const):
     """Const class defining High Level FOFB constants."""
 
-    MIN_SING_VAL = 0.2
+    MIN_SING_VAL = 0.1
     TIKHONOV_REG_CONST = 0
     SINGVALHW_THRS = 1e-14
-    DEF_KICK_BUFFER_SIZE = 1
     DEF_MAX_ORB_DISTORTION = 200  # [um]
 
     CONV_UM_2_NM = 1e3
     ACCGAIN_RESO = 2**-12
 
     DEF_TIMEOUT = 10  # [s]
     DEF_TIMESLEEP = 0.1  # [s]
@@ -59,14 +62,15 @@
     CURRZERO_RMP_FREQ = 2  # [steps/s]
 
     LoopState = _csdev.Const.register('LoopState', _et.OPEN_CLOSED)
     GlobIndiv = _csdev.Const.register('GlobIndiv', _et.GLOB_INDIV)
     UseRF = _csdev.Const.register('UseRF', _et.DSBL_ENBL)
     MeasRespMatCmd = _csdev.Const.register('MeasRespMatCmd', _et.MEAS_RMAT_CMD)
     MeasRespMatMon = _csdev.Const.register('MeasRespMatMon', _et.MEAS_RMAT_MON)
+    DecOpt = _csdev.Const.register('DecOpt', _et.DEC_OPT)
 
     def __init__(self):
         """Class constructor."""
 
         # device names and nicknames
         self.bpm_names = _BPMSearch.get_names({'sec': 'SI', 'dev': 'BPM'})
         if NR_BPM != len(self.bpm_names):
@@ -93,22 +97,31 @@
         self.nr_corrs = self.nr_chcv + 1  # include RF
 
         # data folder
         ioc_fol = _os.path.join(
             '/home', 'sirius', 'iocs-log', 'si-ap-fofb', 'data')
         self.reforb_fname = _os.path.join(ioc_fol, 'reforbit.orb')
         self.respmat_fname = _os.path.join(ioc_fol, 'respmat.respmat')
+        self.bpmxenbl_fname = _os.path.join(ioc_fol, 'bpmxenbllist.bpmenbl')
+        self.bpmyenbl_fname = _os.path.join(ioc_fol, 'bpmyenbllist.bpmenbl')
+        self.chenbl_fname = _os.path.join(ioc_fol, 'chenbllist.correnbl')
+        self.cvenbl_fname = _os.path.join(ioc_fol, 'cvenbllist.correnbl')
+        self.rfenbl_fname = _os.path.join(ioc_fol, 'rfenbllist.rfenbl')
 
         # reforb and matrix parameters
         self.reforb_size = self.nr_bpms
         self.matrix_size = self.nr_corrs * (2 * self.nr_bpms)
         self.nr_svals = min(self.nr_corrs, 2 * self.nr_bpms)
         self.corrcoeffs_size = self.nr_chcv * (2 * self.nr_bpms)
         self.corrgains_size = self.nr_chcv
 
+        # dcc minimum enable configuration
+        self.dccenbl_min = _np.array([
+            bpm.sub[2:] in ['M1', 'M2'] for bpm in self.bpm_names])
+
     def get_hlfofb_database(self):
         """Return Soft IOC database."""
         pvs_database = {
             # Global
             'Version-Cte': {'type': 'string', 'value': 'UNDEF'},
             'Log-Mon': {'type': 'string', 'value': 'Starting...'},
 
@@ -168,15 +181,15 @@
                 'value': self.cv_pos},
             'CHNickName-Cte': {
                 'type': 'string', 'unit': 'shortname for the chs.',
                 'count': self.nr_ch, 'value': self.ch_nicknames},
             'CVNickName-Cte': {
                 'type': 'string', 'unit': 'shortname for the cvs.',
                 'count': self.nr_cv, 'value': self.cv_nicknames},
-            'CorrStatus-Mon': {'type': 'int', 'value': 0b1111111},
+            'CorrStatus-Mon': {'type': 'int', 'value': 0b11111111},
             'CorrStatusLabels-Cte': {
                 'type': 'string', 'count': len(_et.STS_LBLS_CORR),
                 'value': _et.STS_LBLS_CORR},
             'CorrConfig-Cmd': {'type': 'int', 'value': 0},
             'CorrSetPwrStateOn-Cmd': {'type': 'int', 'value': 0},
             'CorrSetPwrStateOff-Cmd': {'type': 'int', 'value': 0},
             'CorrSetOpModeManual-Cmd': {'type': 'int', 'value': 0},
@@ -204,15 +217,15 @@
                 'lolim': 0, 'hilim': 0.95},
 
             # FOFB Controllers
             'TimeFrameLen-SP': {
                 'type': 'int', 'value': 2100, 'lolim': 500, 'hilim': 10000},
             'TimeFrameLen-RB': {
                 'type': 'int', 'value': 2100, 'lolim': 500, 'hilim': 10000},
-            'CtrlrStatus-Mon': {'type': 'int', 'value': 0b111111111},
+            'CtrlrStatus-Mon': {'type': 'int', 'value': 0b11111111111},
             'CtrlrStatusLabels-Cte': {
                 'type': 'string', 'count': len(_et.STS_LBLS_FOFBCTRL),
                 'value': _et.STS_LBLS_FOFBCTRL},
             'CtrlrConfBPMId-Cmd': {'type': 'int', 'value': 0},
             'CtrlrSyncNet-Cmd': {'type': 'int', 'value': 0},
             'CtrlrSyncUseEnblList-Sel': {
                 'type': 'enum', 'enums': _et.DSBL_ENBL,
@@ -225,28 +238,41 @@
                 'value': self.nr_bpms*[1], 'unit': 'DCCs used in loop'},
             'CtrlrSyncRefOrb-Cmd': {'type': 'int', 'value': 0},
             'CtrlrSyncTFrameLen-Cmd': {'type': 'int', 'value': 0},
             'CtrlrConfBPMLogTrg-Cmd': {'type': 'int', 'value': 0},
             'CtrlrSyncMaxOrbDist-Cmd': {'type': 'int', 'value': 0},
             'CtrlrSyncPacketLossDetec-Cmd': {'type': 'int', 'value': 0},
             'CtrlrReset-Cmd': {'type': 'int', 'value': 0},
+            'CtrlrDsblSYSIDExc-Cmd': {'type': 'int', 'value': 0},
 
-            # Kicks and Kick buffer configuration
-            'KickBufferSize-SP': {
-                'type': 'float', 'value': self.DEF_KICK_BUFFER_SIZE, 'prec': 0,
-                'lolim': 1, 'hilim': 1000,
-                'unit': 'Size of the buffer to calculate kicks average.'},
-            'KickBufferSize-RB': {
-                'type': 'float', 'value': self.DEF_KICK_BUFFER_SIZE, 'prec': 0,
-                'lolim': 1, 'hilim': 1000,
-                'unit': 'Size of the buffer to calculate kicks average.'},
-            'KickBufferSize-Mon': {
-                'type': 'float', 'value': self.DEF_KICK_BUFFER_SIZE, 'prec': 0,
-                'lolim': 1, 'hilim': 1000,
-                'unit': 'Actual buffer size used to calculate kicks average.'},
+            # Kicks and decimation configuration
+            'FOFBAccDecimation-Sel': {
+                'type': 'enum', 'enums': _et.DEC_OPT,
+                'value': self.DecOpt.FOFB, 'unit': 'FOFB_Monit_Custom'},
+            'FOFBAccDecimation-Sts': {
+                'type': 'enum', 'enums': _et.DEC_OPT,
+                'value': self.DecOpt.FOFB, 'unit': 'FOFB_Monit_Custom'},
+            'FOFBAccDecimation-SP': {
+                'type': 'float', 'value': 1, 'prec': 0, 'lolim': 1,
+                'hilim': 8600, 'unit': 'count'},
+            'FOFBAccDecimation-RB': {
+                'type': 'float', 'value': 1, 'prec': 0, 'lolim': 1,
+                'hilim': 8600, 'unit': 'count'},
+            'KickCHAcc-Mon': {
+                'type': 'float', 'unit': 'urad', 'count': self.nr_ch,
+                'value': self.nr_ch*[0]},
+            'KickCVAcc-Mon': {
+                'type': 'float', 'unit': 'urad', 'count': self.nr_cv,
+                'value': self.nr_cv*[0]},
+            'KickCHRef-Mon': {
+                'type': 'float', 'unit': 'urad', 'count': self.nr_ch,
+                'value': self.nr_ch*[0]},
+            'KickCVRef-Mon': {
+                'type': 'float', 'unit': 'urad', 'count': self.nr_cv,
+                'value': self.nr_cv*[0]},
             'KickCH-Mon': {
                 'type': 'float', 'unit': 'urad', 'count': self.nr_ch,
                 'value': self.nr_ch*[0]},
             'KickCV-Mon': {
                 'type': 'float', 'unit': 'urad', 'count': self.nr_cv,
                 'value': self.nr_cv*[0]},
```

### Comparing `siriuspy-2.75.0/siriuspy/fofb/main.py` & `siriuspy-2.76.0/siriuspy/fofb/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import numpy as _np
 
 from ..util import update_bit as _updt_bit, get_bit as _get_bit
 from ..epics import PV as _PV
 from ..callbacks import Callback as _Callback
 from ..envars import VACA_PREFIX as _vaca_prefix
 from ..namesys import SiriusPVName as _PVName
-from ..devices import FamFOFBControllers as _FamFOFBCtrls, \
+from ..devices import FamFOFBControllers as _FamFOFBCtrls, Device as _Device,\
     FamFastCorrs as _FamFastCorrs, SOFB as _SOFB, RFGen as _RFGen
 
 from .csdev import HLFOFBConst as _Const, ETypes as _ETypes
 
 
 class App(_Callback):
     """High Level FOFB main application."""
@@ -40,38 +40,22 @@
         self._loop_gain_mon_v = 0
         self._thread_loopstate = None
         self._abort_thread = False
         self._loop_max_orb_dist = self._const.DEF_MAX_ORB_DISTORTION
         self._loop_max_orb_dist_enbl = self._const.DsblEnbl.Dsbl
         self._loop_packloss_detec_enbl = self._const.DsblEnbl.Dsbl
         self._corr_status = self._pvs_database['CorrStatus-Mon']['value']
-        self._corr_confall_count = 0
-        self._corr_setpwrstateon_count = 0
-        self._corr_setpwrstateoff_count = 0
-        self._corr_setopmodemanual_count = 0
-        self._corr_setaccfreezeenbl_count = 0
-        self._corr_setaccfreezedsbl_count = 0
-        self._corr_setaccclear_count = 0
-        self._corr_setcurrzero_count = 0
         self._corr_setcurrzero_dur = 5
         self._thread_currzero = None
         self._abort_thread_currzero = False
         self._ch_maxacccurr = self._pvs_database['CHAccSatMax-RB']['value']
         self._cv_maxacccurr = self._pvs_database['CVAccSatMax-RB']['value']
         self._time_frame_len = self._pvs_database['TimeFrameLen-RB']['value']
         self._fofbctrl_status = self._pvs_database['CtrlrStatus-Mon']['value']
-        self._fofbctrl_confbpmid_count = 0
-        self._fofbctrl_syncnet_count = 0
         self._thread_syncnet = None
-        self._fofbctrl_syncref_count = 0
-        self._fofbctrl_synctframelen_count = 0
-        self._fofbctrl_confbpmlogtrg_count = 0
-        self._fofbctrl_syncmaxorbdist_count = 0
-        self._fofbctrl_syncpackloss_count = 0
-        self._fofbctrl_reset_count = 0
         self._thread_reset = None
         self._fofbctrl_syncenbllist = _np.ones(self._const.nr_bpms, dtype=bool)
         self._fofbctrl_syncuseenbllist = self._const.DsblEnbl.Enbl
         self._reforb_x = _np.zeros(self._const.nr_bpms, dtype=float)
         self._reforbhw_x = _np.zeros(self._const.nr_bpms, dtype=float)
         self._reforb_y = _np.zeros(self._const.nr_bpms, dtype=float)
         self._reforbhw_y = _np.zeros(self._const.nr_bpms, dtype=float)
@@ -82,57 +66,52 @@
         self._enable_lists = {
             'bpmx': _np.ones(self._const.nr_bpms, dtype=bool),
             'bpmy': _np.ones(self._const.nr_bpms, dtype=bool),
             'ch': _np.ones(self._const.nr_ch, dtype=bool),
             'cv': _np.ones(self._const.nr_cv, dtype=bool),
             'rf': _np.ones(1, dtype=bool),
         }
+        self._corr_accdec_val = 1
+        self._corr_accdec_enm = self._const.DecOpt.FOFB
         self._thread_enbllist = None
         self._abort_thread_enbllist = False
         self._min_sing_val = self._const.MIN_SING_VAL
         self._tikhonov_reg_const = self._const.TIKHONOV_REG_CONST
         self._invrespmat_normmode = self._const.GlobIndiv.Global
         self._pscoeffs = self._invrespmatconv[:-1].copy()
         self._psgains = _np.ones(self._const.nr_chcv, dtype=float)
-        self._meas_respmat_count = 0
         self._meas_respmat_kick = {
             'ch': 15,  # [urad]
             'cv': 22.5,  # [urad]
             'rf': 75,  # [Hz]
         }
         self._meas_respmat_wait = 1  # [s]
         self._meas_respmat_thread = None
         self._measuring_respmat = False
 
-        # use pyepics recommendations for threading
-        _epics.ca.use_initial_context()
-
         # devices and connections
         self._sisofb_dev = _SOFB(_SOFB.DEVICES.SI)
-        ppties_automon_off = [
-            'MTurnSum-Mon', 'MTurnOrbX-Mon', 'MTurnOrbY-Mon', 'MTurnTime-Mon',
-            'MTurnIdxOrbX-Mon', 'MTurnIdxOrbY-Mon', 'MTurnIdxSum-Mon',
-            'SlowOrbX-Mon', 'SlowOrbY-Mon',
-            'KickCH-Mon', 'KickCV-Mon', 'KickRF-Mon',
-            'DeltaKickCH-Mon', 'DeltaKickCV-Mon', 'DeltaKickRF-Mon',
-        ]
-        for ppty in ppties_automon_off:
-            self._sisofb_dev.set_auto_monitor(ppty, False)
 
         corrnames = self._const.ch_names + self._const.cv_names
         self._corrs_dev = _FamFastCorrs(corrnames)
 
-        self._kick_buffer = []
-        self._kick_buffer_size = self._const.DEF_KICK_BUFFER_SIZE
-        for idx, pso in enumerate(self._corrs_dev.psdevs):
-            pvo = pso.pv_object('CurrentRef-Mon')
-            pvo.auto_monitor = True
-            self._kick_buffer.append([])
-            pvo.add_callback(
-                _part(self._update_kick_buffer, ps_index=idx))
+        self._propty2kickpvs = {
+            'FOFBAcc-Mon': ['KickCHAcc-Mon', 'KickCVAcc-Mon'],
+            'CurrentRef-Mon': ['KickCHRef-Mon', 'KickCVRef-Mon'],
+            'Current-Mon': ['KickCH-Mon', 'KickCV-Mon'],
+        }
+        self._kick_mon = {}
+        size = len(self._corrs_dev.psdevs)
+        for propty in self._propty2kickpvs:
+            self._kick_mon[propty] = _np.zeros(size, dtype=float)
+            for idx, pso in enumerate(self._corrs_dev.psdevs):
+                pvo = pso.pv_object(propty)
+                pvo.auto_monitor = _epics.dbr.DBE_VALUE
+                pvo.add_callback(
+                    _part(self._update_kick_array, ps_index=idx))
 
         self._rf_dev = _RFGen()
 
         self._llfofb_dev = _FamFOFBCtrls()
 
         self._intlk_pvs = list()
         self._intlk_values = dict()
@@ -141,14 +120,19 @@
             self._intlk_values[pvo.pvname] = 0
             pvo.auto_monitor = True
             pvo.add_callback(self._callback_loopintlk)
             self._intlk_pvs.append(pvo)
 
         self._corrs_dev.wait_for_connection(self._const.DEF_TIMEWAIT)
 
+        self._auxbpm = _Device(
+            'SI-01M1:DI-BPM',
+            properties=('INFOFOFBRate-RB', 'INFOMONITRate-RB'),
+            auto_mon=False)
+
         havebeam_pvname = _PVName(
             'SI-Glob:AP-CurrInfo:StoredEBeam-Mon').substitute(
                 prefix=_vaca_prefix)
         self._havebeam_pv = _PV(
             havebeam_pvname, connection_timeout=0.05,
             callback=self._callback_havebeam)
 
@@ -177,15 +161,17 @@
             'CtrlrSyncRefOrb-Cmd': self.cmd_fofbctrl_syncreforb,
             'CtrlrSyncTFrameLen-Cmd': self.cmd_fofbctrl_synctframelen,
             'CtrlrConfBPMLogTrg-Cmd': self.cmd_fofbctrl_confbpmlogtrg,
             'CtrlrSyncUseEnblList-Sel': self.set_fofbctrl_syncuseenablelist,
             'CtrlrSyncMaxOrbDist-Cmd': self.cmd_fofbctrl_syncmaxorbdist,
             'CtrlrSyncPacketLossDetec-Cmd': self.cmd_fofbctrl_syncpacklossdet,
             'CtrlrReset-Cmd': self.cmd_fofbctrl_reset,
-            'KickBufferSize-SP': self.set_kicker_buffer_size,
+            'CtrlrDsblSYSIDExc-Cmd': self.cmd_fofbctrl_dsblsysid,
+            'FOFBAccDecimation-Sel': _part(self.set_corr_accdec, 'enum'),
+            'FOFBAccDecimation-SP': _part(self.set_corr_accdec, 'value'),
             'RefOrbX-SP': _part(self.set_reforbit, 'x'),
             'RefOrbY-SP': _part(self.set_reforbit, 'y'),
             'RespMat-SP': self.set_respmat,
             'BPMXEnblList-SP': _part(self.set_enbllist, 'bpmx'),
             'BPMYEnblList-SP': _part(self.set_enbllist, 'bpmy'),
             'CHEnblList-SP': _part(self.set_enbllist, 'ch'),
             'CVEnblList-SP': _part(self.set_enbllist, 'cv'),
@@ -208,127 +194,114 @@
         self.thread_check_corrs_configs.start()
         self.thread_check_ctrls_configs = _epics.ca.CAThread(
             target=self._check_ctrls_configs, daemon=True)
         self.thread_check_ctrls_configs.start()
 
     def init_database(self):
         """Set initial PV values."""
-        self.run_callbacks('LoopState-Sel', self._loop_state)
-        self.run_callbacks('LoopState-Sts', self._loop_state)
-        self.run_callbacks('LoopGainH-SP', self._loop_gain_h)
-        self.run_callbacks('LoopGainH-RB', self._loop_gain_h)
-        self.run_callbacks('LoopGainH-Mon', self._loop_gain_mon_h)
-        self.run_callbacks('LoopGainV-SP', self._loop_gain_v)
-        self.run_callbacks('LoopGainV-RB', self._loop_gain_v)
-        self.run_callbacks('LoopGainV-Mon', self._loop_gain_mon_v)
-        self.run_callbacks('LoopMaxOrbDistortion-SP', self._loop_max_orb_dist)
-        self.run_callbacks('LoopMaxOrbDistortion-RB', self._loop_max_orb_dist)
-        self.run_callbacks(
-            'LoopMaxOrbDistortionEnbl-Sel', self._loop_max_orb_dist_enbl)
-        self.run_callbacks(
-            'LoopMaxOrbDistortionEnbl-Sts', self._loop_max_orb_dist_enbl)
-        self.run_callbacks(
-            'LoopPacketLossDetecEnbl-Sel', self._loop_packloss_detec_enbl)
-        self.run_callbacks(
-            'LoopPacketLossDetecEnbl-Sts', self._loop_packloss_detec_enbl)
-        self.run_callbacks('CorrStatus-Mon', self._corr_status)
-        self.run_callbacks('CorrConfig-Cmd', self._corr_confall_count)
-        self.run_callbacks(
-            'CorrSetPwrStateOn-Cmd', self._corr_setpwrstateon_count)
-        self.run_callbacks(
-            'CorrSetOpModeManual-Cmd', self._corr_setopmodemanual_count)
-        self.run_callbacks(
-            'CorrSetAccFreezeDsbl-Cmd', self._corr_setaccfreezedsbl_count)
-        self.run_callbacks(
-            'CorrSetAccFreezeEnbl-Cmd', self._corr_setaccfreezeenbl_count)
-        self.run_callbacks(
-            'CorrSetAccClear-Cmd', self._corr_setaccclear_count)
-        self.run_callbacks(
-            'CorrSetCurrZero-Cmd', self._corr_setcurrzero_count)
-        self.run_callbacks(
-            'CorrSetCurrZeroDuration-SP', self._corr_setcurrzero_dur)
-        self.run_callbacks(
-            'CorrSetCurrZeroDuration-RB', self._corr_setcurrzero_dur)
-        self.run_callbacks('CHAccSatMax-SP', self._ch_maxacccurr)
-        self.run_callbacks('CHAccSatMax-RB', self._ch_maxacccurr)
-        self.run_callbacks('CVAccSatMax-SP', self._cv_maxacccurr)
-        self.run_callbacks('CVAccSatMax-RB', self._cv_maxacccurr)
-        self.run_callbacks('TimeFrameLen-SP', self._time_frame_len)
-        self.run_callbacks('TimeFrameLen-RB', self._time_frame_len)
-        self.run_callbacks('CtrlrStatus-Mon', self._fofbctrl_status)
-        self.run_callbacks(
-            'CtrlrConfBPMId-Cmd', self._fofbctrl_confbpmid_count)
-        self.run_callbacks(
-            'CtrlrSyncNet-Cmd', self._fofbctrl_syncnet_count)
-        self.run_callbacks(
-            'CtrlrSyncUseEnblList-Sel', self._fofbctrl_syncuseenbllist)
-        self.run_callbacks(
-            'CtrlrSyncUseEnblList-Sts', self._fofbctrl_syncuseenbllist)
-        self.run_callbacks(
-            'CtrlrSyncEnblList-Mon', self._fofbctrl_syncenbllist)
-        self.run_callbacks(
-            'CtrlrSyncRefOrb-Cmd', self._fofbctrl_syncref_count)
-        self.run_callbacks(
-            'CtrlrSyncTFrameLen-Cmd', self._fofbctrl_synctframelen_count)
-        self.run_callbacks(
-            'CtrlrConfBPMLogTrg-Cmd', self._fofbctrl_confbpmlogtrg_count)
-        self.run_callbacks(
-            'CtrlrSyncMaxOrbDist-Cmd', self._fofbctrl_syncmaxorbdist_count)
-        self.run_callbacks(
-            'CtrlrSyncPacketLossDetec-Cmd', self._fofbctrl_syncpackloss_count)
-        self.run_callbacks('CtrlrReset-Cmd', self._fofbctrl_reset_count)
-        self.run_callbacks('KickBufferSize-SP', self._kick_buffer_size)
-        self.run_callbacks('KickBufferSize-RB', self._kick_buffer_size)
-        self.run_callbacks('KickBufferSize-Mon', self._kick_buffer_size)
-        self.run_callbacks(
-            'KickCH-Mon', _np.zeros(self._const.nr_ch, dtype=float))
-        self.run_callbacks(
-            'KickCV-Mon', _np.zeros(self._const.nr_cv, dtype=float))
-        self.run_callbacks('RefOrbX-SP', self._reforb_x)
-        self.run_callbacks('RefOrbX-RB', self._reforb_x)
-        self.run_callbacks('RefOrbY-SP', self._reforb_y)
-        self.run_callbacks('RefOrbY-RB', self._reforb_y)
-        self.run_callbacks('RefOrbHwX-Mon', self._reforbhw_x)
-        self.run_callbacks('RefOrbHwY-Mon', self._reforbhw_y)
-        self.run_callbacks('BPMXEnblList-SP', self._enable_lists['bpmx'])
-        self.run_callbacks('BPMXEnblList-RB', self._enable_lists['bpmx'])
-        self.run_callbacks('BPMYEnblList-SP', self._enable_lists['bpmy'])
-        self.run_callbacks('BPMYEnblList-RB', self._enable_lists['bpmy'])
-        self.run_callbacks('CHEnblList-SP', self._enable_lists['ch'])
-        self.run_callbacks('CHEnblList-RB', self._enable_lists['ch'])
-        self.run_callbacks('CVEnblList-SP', self._enable_lists['cv'])
-        self.run_callbacks('CVEnblList-RB', self._enable_lists['cv'])
-        self.run_callbacks(
-            'UseRF-Sel', bool(self._enable_lists['rf']))
-        self.run_callbacks(
-            'UseRF-Sts', bool(self._enable_lists['rf']))
-        self.run_callbacks('MinSingValue-SP', self._min_sing_val)
-        self.run_callbacks('MinSingValue-RB', self._min_sing_val)
-        self.run_callbacks('TikhonovRegConst-SP', self._tikhonov_reg_const)
-        self.run_callbacks('TikhonovRegConst-RB', self._tikhonov_reg_const)
-        self.run_callbacks('InvRespMatNormMode-Sel', self._invrespmat_normmode)
-        self.run_callbacks('InvRespMatNormMode-Sts', self._invrespmat_normmode)
-        self._load_respmat()
+        initkickch = _np.zeros(self._const.nr_ch, dtype=float)
+        initkickcv = _np.zeros(self._const.nr_cv, dtype=float)
+        pvn2vals = {
+            'LoopState-Sel': self._loop_state,
+            'LoopState-Sts': self._loop_state,
+            'LoopGainH-SP': self._loop_gain_h,
+            'LoopGainH-RB': self._loop_gain_h,
+            'LoopGainH-Mon': self._loop_gain_mon_h,
+            'LoopGainV-SP': self._loop_gain_v,
+            'LoopGainV-RB': self._loop_gain_v,
+            'LoopGainV-Mon': self._loop_gain_mon_v,
+            'LoopMaxOrbDistortion-SP': self._loop_max_orb_dist,
+            'LoopMaxOrbDistortion-RB': self._loop_max_orb_dist,
+            'LoopMaxOrbDistortionEnbl-Sel': self._loop_max_orb_dist_enbl,
+            'LoopMaxOrbDistortionEnbl-Sts': self._loop_max_orb_dist_enbl,
+            'LoopPacketLossDetecEnbl-Sel': self._loop_packloss_detec_enbl,
+            'LoopPacketLossDetecEnbl-Sts': self._loop_packloss_detec_enbl,
+            'CorrStatus-Mon': self._corr_status,
+            'CorrConfig-Cmd': 0,
+            'CorrSetPwrStateOn-Cmd': 0,
+            'CorrSetOpModeManual-Cmd': 0,
+            'CorrSetAccFreezeDsbl-Cmd': 0,
+            'CorrSetAccFreezeEnbl-Cmd': 0,
+            'CorrSetAccClear-Cmd': 0,
+            'CorrSetCurrZero-Cmd': 0,
+            'CorrSetCurrZeroDuration-SP': self._corr_setcurrzero_dur,
+            'CorrSetCurrZeroDuration-RB': self._corr_setcurrzero_dur,
+            'CHAccSatMax-SP': self._ch_maxacccurr,
+            'CHAccSatMax-RB': self._ch_maxacccurr,
+            'CVAccSatMax-SP': self._cv_maxacccurr,
+            'CVAccSatMax-RB': self._cv_maxacccurr,
+            'TimeFrameLen-SP': self._time_frame_len,
+            'TimeFrameLen-RB': self._time_frame_len,
+            'CtrlrStatus-Mon': self._fofbctrl_status,
+            'CtrlrConfBPMId-Cmd': 0,
+            'CtrlrSyncNet-Cmd': 0,
+            'CtrlrSyncUseEnblList-Sel': self._fofbctrl_syncuseenbllist,
+            'CtrlrSyncUseEnblList-Sts': self._fofbctrl_syncuseenbllist,
+            'CtrlrSyncEnblList-Mon': self._fofbctrl_syncenbllist,
+            'CtrlrSyncRefOrb-Cmd': 0,
+            'CtrlrSyncTFrameLen-Cmd': 0,
+            'CtrlrConfBPMLogTrg-Cmd': 0,
+            'CtrlrSyncMaxOrbDist-Cmd': 0,
+            'CtrlrSyncPacketLossDetec-Cmd': 0,
+            'CtrlrReset-Cmd': 0,
+            'CtrlrDsblSYSIDExc-Cmd': 0,
+            'FOFBAccDecimation-Sel': self._corr_accdec_enm,
+            'FOFBAccDecimation-Sts': self._corr_accdec_enm,
+            'FOFBAccDecimation-SP': self._corr_accdec_val,
+            'FOFBAccDecimation-RB': self._corr_accdec_val,
+            'KickCHAcc-Mon': initkickch,
+            'KickCVAcc-Mon': initkickcv,
+            'KickCHRef-Mon': initkickch,
+            'KickCVRef-Mon': initkickcv,
+            'KickCH-Mon': initkickch,
+            'KickCV-Mon': initkickcv,
+            'MinSingValue-SP': self._min_sing_val,
+            'MinSingValue-RB': self._min_sing_val,
+            'TikhonovRegConst-SP': self._tikhonov_reg_const,
+            'TikhonovRegConst-RB': self._tikhonov_reg_const,
+            'InvRespMatNormMode-Sel': self._invrespmat_normmode,
+            'InvRespMatNormMode-Sts': self._invrespmat_normmode,
+            'MeasRespMat-Cmd': 0,
+            'MeasRespMat-Mon': self._const.MeasRespMatMon.Idle,
+            'MeasRespMatKickCH-SP': self._meas_respmat_kick['ch'],
+            'MeasRespMatKickCH-RB': self._meas_respmat_kick['ch'],
+            'MeasRespMatKickCV-SP': self._meas_respmat_kick['cv'],
+            'MeasRespMatKickCV-RB': self._meas_respmat_kick['cv'],
+            'MeasRespMatKickRF-SP': self._meas_respmat_kick['rf'],
+            'MeasRespMatKickRF-RB': self._meas_respmat_kick['rf'],
+            'MeasRespMatWait-SP': self._meas_respmat_wait,
+            'MeasRespMatWait-RB': self._meas_respmat_wait,
+        }
+        for pvn, val in pvn2vals.items():
+            self.run_callbacks(pvn, val)
+
+        # load autosave data
+        # matrix
+        okm = self._load_respmat()
         self.run_callbacks('RespMat-SP', list(self._respmat.ravel()))
-        self.run_callbacks('MeasRespMat-Cmd', self._meas_respmat_count)
-        self.run_callbacks('MeasRespMat-Mon', self._const.MeasRespMatMon.Idle)
-        self.run_callbacks(
-            'MeasRespMatKickCH-SP', self._meas_respmat_kick['ch'])
-        self.run_callbacks(
-            'MeasRespMatKickCH-RB', self._meas_respmat_kick['ch'])
-        self.run_callbacks(
-            'MeasRespMatKickCV-SP', self._meas_respmat_kick['cv'])
-        self.run_callbacks(
-            'MeasRespMatKickCV-RB', self._meas_respmat_kick['cv'])
-        self.run_callbacks(
-            'MeasRespMatKickRF-SP', self._meas_respmat_kick['rf'])
-        self.run_callbacks(
-            'MeasRespMatKickRF-RB', self._meas_respmat_kick['rf'])
-        self.run_callbacks('MeasRespMatWait-SP', self._meas_respmat_wait)
-        self.run_callbacks('MeasRespMatWait-RB', self._meas_respmat_wait)
+        if not okm:
+            self.run_callbacks('RespMat-RB', list(self._respmat.ravel()))
+        # ref orbits
+        okr = self._load_reforbit()
+        for plan in ['x', 'y']:
+            pvn = f'RefOrb{plan.upper()}-SP'
+            pvv = getattr(self, f'_reforb_{plan}')
+            self.run_callbacks(pvn, pvv)
+            if not okr:
+                self.run_callbacks(pvn.replace('SP', 'RB'), pvv)
+        # enable lists
+        for dev in ['bpmx', 'bpmy', 'ch', 'cv', 'rf']:
+            okl = self._load_enbllist(dev)
+            pvn = f'{dev.upper()}EnblList-SP' if dev != 'rf' else 'UseRF-Sel'
+            enb = self._enable_lists[dev]
+            pvv = enb if dev != 'rf' else bool(enb)
+            self.run_callbacks(pvn, pvv)
+            if not okl:
+                self.run_callbacks(
+                    pvn.replace('SP', 'RB').replace('Sel', 'Sts'), pvv)
         self._update_log('Started.')
         self._init = True
 
     @property
     def pvs_database(self):
         """Return pvs_database."""
         return self._pvs_database
@@ -378,15 +351,15 @@
         """Return if there is stored beam."""
         if self._tests:
             return True
         return self._havebeam_pv.connected and self._havebeam_pv.value
 
     # --- loop control ---
 
-    def set_loop_state(self, value, reset=False, abort=False):
+    def set_loop_state(self, value, abort=False):
         """Set loop state."""
         if not 0 <= value < len(_ETypes.OPEN_CLOSED):
             return False
 
         self._loop_state_lastsp = value
         if value:
             if not self.havebeam:
@@ -401,19 +374,19 @@
                 self._thread_loopstate.is_alive():
             self._update_log('WARN:Interrupting Loop Enable thread...')
             self._abort_thread = True
             self._thread_loopstate.join()
 
         self._thread_loopstate = _epics.ca.CAThread(
             target=self._thread_set_loop_state,
-            args=[value, reset, abort], daemon=True)
+            args=[value, abort], daemon=True)
         self._thread_loopstate.start()
         return True
 
-    def _thread_set_loop_state(self, value, reset, abort):
+    def _thread_set_loop_state(self, value, abort):
         if value:  # closing the loop
             # set gains to zero, recalculate gains and coeffs
             self._update_log('Setting Loop Gain to zero...')
             self._loop_gain_mon_h, self._loop_gain_mon_v = 0, 0
             self._calc_corrs_coeffs(log=False)
             # set and wait corrector gains and coeffs to zero
             if not self._set_corrs_coeffs(log=False):
@@ -453,17 +426,14 @@
                 return
 
             # open the loop
             self._loop_state = value
             self._check_set_corrs_opmode()
             self.run_callbacks('LoopState-Sts', self._loop_state)
 
-        if reset:
-            self._do_fofbctrl_reset()
-
     def _do_loop_gain_ramp(self, ramp='up', abort=False):
         xdata = _np.linspace(0, 1, self._const.LOOPGAIN_RMP_NPTS)
         power = 1
         if ramp == 'up':
             ydata = xdata**power
             ydata_h = ydata * self._loop_gain_h
             ydata_v = ydata * self._loop_gain_v
@@ -624,127 +594,96 @@
         self._check_set_corrs_opmode()
         # fofbacc_freeze
         self._set_corrs_fofbacc_freeze()
         # matrix coefficients
         self._set_corrs_coeffs()
 
         self._update_log('Correctors configuration done!')
-
-        self._corr_confall_count += 1
-        self.run_callbacks('CorrConfig-Cmd', self._corr_confall_count)
-        return False
+        return True
 
     def cmd_corr_pwrstate_on(self, _):
         """Set all corrector pwrstate to on."""
         self._update_log('Received set corrector pwrstate to on...')
         if not self._check_corr_connection():
             return False
 
         self._update_log('Setting all corrector pwrstate to on...')
         self._corrs_dev.set_pwrstate(self._const.OffOn.On)
         self._update_log('...done!')
-
-        self._corr_setpwrstateon_count += 1
-        self.run_callbacks(
-            'CorrSetPwrStateOn-Cmd', self._corr_setpwrstateon_count)
-        return False
+        return True
 
     def cmd_corr_pwrstate_off(self, _):
         """Set all corrector pwrstate to off."""
         self._update_log('Received set corrector pwrstate to off...')
         if not self._check_corr_connection():
             return False
 
         self._update_log('Setting all corrector pwrstate to off...')
         self._corrs_dev.set_pwrstate(self._const.OffOn.Off)
         self._update_log('...done!')
-
-        self._corr_setpwrstateoff_count += 1
-        self.run_callbacks(
-            'CorrSetPwrStateOff-Cmd', self._corr_setpwrstateoff_count)
-        return False
+        return True
 
     def cmd_corr_opmode_manual(self, _):
         """Set all corrector opmode to manual."""
         self._update_log('Received set corrector opmode to manual...')
         if not self._check_corr_connection():
             return False
 
         self._update_log('Setting all corrector opmode to manual...')
         self._corrs_dev.set_opmode(self._corrs_dev.OPMODE_STS.manual)
         self._update_log('...done!')
-
-        self._corr_setopmodemanual_count += 1
-        self.run_callbacks(
-            'CorrSetOpModeManual-Cmd', self._corr_setopmodemanual_count)
-        return False
+        return True
 
     def cmd_corr_accfreeze_dsbl(self, _):
         """Set all corrector accumulator freeze state to Dsbl."""
         self._update_log('Received set corrector AccFreeze to Dsbl...')
         if not self._check_corr_connection():
             return False
 
         self._update_log('Setting AccFreeze to Dsbl...')
         self._corrs_dev.set_fofbacc_freeze(self._const.DsblEnbl.Dsbl)
         self._update_log('...done!')
-
-        self._corr_setaccfreezedsbl_count += 1
-        self.run_callbacks(
-            'CorrSetAccFreezeDsbl-Cmd', self._corr_setaccfreezedsbl_count)
-        return False
+        return True
 
     def cmd_corr_accfreeze_enbl(self, _):
         """Set all corrector accumulator freeze state to Enbl."""
         self._update_log('Received set corrector AccFreeze to Enbl...')
         if not self._check_corr_connection():
             return False
 
         self._update_log('Setting AccFreeze to Enbl...')
         self._corrs_dev.set_fofbacc_freeze(self._const.DsblEnbl.Enbl)
         self._update_log('...done!')
-
-        self._corr_setaccfreezeenbl_count += 1
-        self.run_callbacks(
-            'CorrSetAccFreezeEnbl-Cmd', self._corr_setaccfreezeenbl_count)
-        return False
+        return True
 
     def cmd_corr_accclear(self, _):
         """Clear all corrector accumulator."""
         self._update_log('Received clear all corrector accumulator...')
         if not self._check_corr_connection():
             return False
 
         self._update_log('Sending clear accumulator command...')
         self._corrs_dev.cmd_fofbacc_clear()
         self._update_log('...done!')
-
-        self._corr_setaccclear_count += 1
-        self.run_callbacks(
-            'CorrSetAccClear-Cmd', self._corr_setaccclear_count)
-        return False
+        return True
 
     def cmd_corr_currzero(self, _):
         """Set all corrector current to zero."""
         self._update_log('Received set corrector current to zero...')
         if not self._check_corr_connection():
             return False
         if self._thread_currzero is not None and \
                 self._thread_currzero.is_alive():
             self._update_log('ERR:Current ramp down already in progress.')
             return False
 
         self._thread_currzero = _epics.ca.CAThread(
             target=self._thread_corr_currzero, daemon=True)
         self._thread_currzero.start()
-
-        self._corr_setcurrzero_count += 1
-        self.run_callbacks(
-            'CorrSetCurrZero-Cmd', self._corr_setcurrzero_count)
-        return False
+        return True
 
     def set_corr_currzero_duration(self, value):
         """Set corrector ramp down current duration."""
         if not 0 <= value <= 1000:
             return False
 
         self._corr_setcurrzero_dur = value
@@ -755,14 +694,48 @@
             self._thread_currzero.join()
             self._thread_currzero = _epics.ca.CAThread(
                 target=self._thread_corr_currzero, daemon=True)
             self._thread_currzero.start()
         self.run_callbacks('CorrSetCurrZeroDuration-RB', value)
         return True
 
+    def set_corr_accdec(self, option, value):
+        """Set corrector accumulator decimation."""
+        if self._corr_accdec_enm != self._const.DecOpt.Custom and \
+                option == 'value':
+            return False
+
+        if option == 'enum':
+            if value == self._const.DecOpt.FOFB:
+                dec = 1
+            elif value == self._const.DecOpt.Monit:
+                if self._auxbpm.connected:
+                    monit = self._auxbpm['INFOMONITRate-RB']
+                    fofb = self._auxbpm['INFOFOFBRate-RB']
+                    dec = monit // fofb
+                else:
+                    self._update_log('WARN:Could not read decimation from BPM')
+                    self._update_log('WARN:rates. Using value 4600.')
+                    dec = 4600
+            else:
+                dec = self._corr_accdec_val
+            self._corr_accdec_enm = value
+            self.run_callbacks('FOFBAccDecimation-Sts', value)
+            self.run_callbacks('FOFBAccDecimation-SP', dec)
+        else:
+            dec = value
+        self._corr_accdec_val = dec
+        self.run_callbacks('FOFBAccDecimation-RB', dec)
+
+        self._update_log('Setting FOFB Acc decimation...')
+        self._corrs_dev.set_fofbacc_decimation(dec)
+        self._update_log('...done!')
+
+        return True
+
     def _thread_corr_currzero(self):
         if self._corrs_dev.check_current(0):
             self._update_log('Current of all correctors already zeroed.')
             return
 
         self._update_log('Sending all corrector current to zero...')
 
@@ -834,19 +807,15 @@
             self._update_log('Configuring DCC BPMIds...')
             if self._llfofb_dev.cmd_config_bpm_id():
                 self._update_log('Sent configuration to DCCs.')
             else:
                 self._update_log('ERR:Failed to configure DCCs.')
         else:
             self._update_log('FOFB DCC BPMIds already configured.')
-
-        self._fofbctrl_confbpmid_count += 1
-        self.run_callbacks(
-            'CtrlrConfBPMId-Cmd', self._fofbctrl_confbpmid_count)
-        return False
+        return True
 
     def cmd_fofbctrl_syncnet(self, _):
         """Sync FOFB net command."""
         self._update_log('Received sync FOFB net command...')
         if not self._check_fofbctrl_connection():
             return False
         self._update_log('Checking...')
@@ -855,19 +824,15 @@
                 self._thread_syncnet.is_alive():
             self._update_log('ERR:Net sync already in progress.')
             return False
 
         self._thread_syncnet = _epics.ca.CAThread(
             target=self._thread_fofbctrl_syncnet, daemon=True)
         self._thread_syncnet.start()
-
-        self._fofbctrl_syncnet_count += 1
-        self.run_callbacks(
-            'CtrlrSyncNet-Cmd', self._fofbctrl_syncnet_count)
-        return False
+        return True
 
     def _thread_fofbctrl_syncnet(self):
         steps = [
             self._dsbl_fofbctrl_minbpmcnt_enbl,
             self._do_fofbctrl_syncnet,
             self._wait_fofbctrl_netsync,
             self._conf_fofbctrl_minbpmcnt_enbl,
@@ -886,19 +851,15 @@
                 self._llfofb_dev.check_reforby(self._reforbhw_y):
             self._update_log('Syncing FOFB RefOrb...')
             self._llfofb_dev.set_reforbx(self._reforbhw_x)
             self._llfofb_dev.set_reforby(self._reforbhw_y)
             self._update_log('...done!')
         else:
             self._update_log('FOFB RefOrb already synced.')
-
-        self._fofbctrl_syncref_count += 1
-        self.run_callbacks(
-            'CtrlrSyncRefOrb-Cmd', self._fofbctrl_syncref_count)
-        return False
+        return True
 
     def cmd_fofbctrl_synctframelen(self, _):
         """Sync FOFB controllers TimeFrameLen command."""
         self._update_log('Received configure FOFB controllers')
         self._update_log('TimeFrameLen command... Checking...')
         if not self._check_fofbctrl_connection():
             return False
@@ -907,19 +868,15 @@
             self._update_log('Configuring TimeFrameLen PVs...')
             if self._llfofb_dev.set_time_frame_len(timeframe):
                 self._update_log('...done!')
             else:
                 self._update_log('ERR:Failed to configure TimeFrameLen.')
         else:
             self._update_log('TimeFrameLen PVs already configured.')
-
-        self._fofbctrl_synctframelen_count += 1
-        self.run_callbacks(
-            'CtrlrSyncTFrameLen-Cmd', self._fofbctrl_synctframelen_count)
-        return False
+        return True
 
     def cmd_fofbctrl_confbpmlogtrg(self, _):
         """Configure BPM logical triggers command."""
         self._update_log('Received configure BPM Logical')
         if not self._check_fofbctrl_connection():
             return False
         self._update_log('triggers command... Checking...')
@@ -927,19 +884,15 @@
             self._update_log('Configuring BPM logical triggers...')
             if self._llfofb_dev.cmd_config_bpm_trigs():
                 self._update_log('...done!')
             else:
                 self._update_log('ERR:Failed to configure BPM log.trigs.')
         else:
             self._update_log('BPM logical triggers already configured.')
-
-        self._fofbctrl_confbpmlogtrg_count += 1
-        self.run_callbacks(
-            'CtrlrConfBPMLogTrg-Cmd', self._fofbctrl_confbpmlogtrg_count)
-        return False
+        return True
 
     def set_fofbctrl_syncuseenablelist(self, value):
         """Set whether to use or not BPMEnblList in sync."""
         if not self._check_fofbctrl_connection():
             return False
         if not 0 <= value < len(_ETypes.DSBL_ENBL):
             return False
@@ -979,92 +932,65 @@
             self._update_log('Setting MaxOrbDistortionEnbl PVs...')
             if self._llfofb_dev.set_max_orb_distortion_enbl(sts, timeout=tout):
                 self._update_log('...done!')
             else:
                 self._update_log('ERR:Failed to sync enable status.')
         else:
             self._update_log('MaxOrbDistortionEnbl PVs already configured.')
-
-        self._fofbctrl_syncmaxorbdist_count += 1
-        self.run_callbacks(
-            'CtrlrSyncMaxOrbDist-Cmd', self._fofbctrl_syncmaxorbdist_count)
-        return False
+        return True
 
     def cmd_fofbctrl_syncpacklossdet(self, _):
         """Sync FOFB controllers packet loss detection command."""
         self._update_log('Received sync FOFB controllers packet')
         self._update_log('loss detection command...Checking...')
         if not self._check_fofbctrl_connection():
             return False
-
         self._conf_fofbctrl_packetlossdetec()
-
-        self._fofbctrl_syncpackloss_count += 1
-        self.run_callbacks(
-            'CtrlrSyncPacketLossDetec-Cmd', self._fofbctrl_syncpackloss_count)
-        return False
+        return True
 
     def cmd_fofbctrl_reset(self, _):
         """Reset FOFB controllers interlock command."""
         self._update_log('Received reset FOFB controllers command...')
         if not self._check_fofbctrl_connection():
             return False
-
         self._do_fofbctrl_reset()
+        return True
 
-        self._fofbctrl_reset_count += 1
-        self.run_callbacks('CtrlrReset-Cmd', self._fofbctrl_reset_count)
-        return False
-
-    # --- kicks buffer and kicks update ---
-
-    def set_kicker_buffer_size(self, value: int):
-        """Set size of the kick buffer.
-
-        Args:
-            value (int): New value for the buffer size.
-
-        Returns:
-            bool: Whether property was properly set.
-
-        """
-        self._kick_buffer_size = max(1, int(value))
-        self.run_callbacks('KickBufferSize-RB', self._kick_buffer_size)
+    def cmd_fofbctrl_dsblsysid(self, _):
+        """Disable FOFB controllers system identification excitation."""
+        self._update_log('Received disable FOFB controllers SYSID...')
+        if not self._check_fofbctrl_connection():
+            return False
+        self._update_log('Disabling SYSID excitation...')
+        self._llfofb_dev.cmd_dsbl_sysid_exc()
+        self._update_log('...done!')
         return True
 
-    def _update_kick_buffer(self, pvname, value, ps_index, **kwargs):
-        _ = kwargs, pvname
+    # --- kicks update ---
+
+    def _update_kick_array(self, pvname, value, ps_index, **kwargs):
+        _ = kwargs
         if value is None:
             return
         val = self._corrs_dev.psconvs[ps_index].conv_current_2_strength(value)
         if val is None:
             return
-        self._kick_buffer[ps_index].append(val)
-        del self._kick_buffer[ps_index][:-self._kick_buffer_size]
+        propty = _PVName(pvname).propty
+        self._kick_mon[propty][ps_index] = val
 
     def _update_kicks(self):
-        kickch, kickcv = [], []
-        lenb = self._kick_buffer_size if self._loop_state else 1
+        nrch, nrcv = self._const.nr_ch, self._const.nr_cv
 
-        rlenb = 0
-        for i in range(self._const.nr_ch):
-            buff = self._kick_buffer[i][-lenb:]
-            rlenb = max(rlenb, len(buff))
-            val = _np.mean(buff) if buff else 0.0
-            kickch.append(val)
-
-        for i in range(self._const.nr_ch, self._const.nr_chcv):
-            buff = self._kick_buffer[i][-lenb:]
-            rlenb = max(rlenb, len(buff))
-            val = _np.mean(buff) if buff else 0.0
-            kickcv.append(val)
-
-        self.run_callbacks('KickCH-Mon', kickch)
-        self.run_callbacks('KickCV-Mon', kickcv)
-        self.run_callbacks('KickBufferSize-Mon', rlenb)
+        for propty, kickpvs in self._propty2kickpvs.items():
+            kicks = self._kick_mon[propty]
+            kickch = kicks[:nrch]
+            kickcv = kicks[nrch:nrch+nrcv]
+
+            self.run_callbacks(kickpvs[0], kickch)
+            self.run_callbacks(kickpvs[1], kickcv)
 
     # --- reference orbit ---
 
     def set_reforbit(self, plane, value):
         """Set reference orbit."""
         self._update_log(f'Setting New RefOrb{plane.upper()}...')
 
@@ -1079,24 +1005,55 @@
         setattr(self, '_reforb_' + plane.lower(), ref)
         # hardware units
         refhw = ref * self._const.CONV_UM_2_NM
         refhw = _np.round(refhw)  # round, low level expect it to be int
         refhw = _np.roll(refhw, 1)  # make BPM 01M1 the first element
         setattr(self, '_reforbhw_' + plane.lower(), refhw)
 
-        # set reforb to FOFB controllers
-        func = getattr(self._llfofb_dev, 'set_reforb' + plane.lower())
-        func(refhw)
+        # do not set reforb to controllers and save to file in initialization
+        if self._init:
+            # set reforb to FOFB controllers
+            func = getattr(self._llfofb_dev, 'set_reforb' + plane.lower())
+            func(refhw)
+
+            # save to autosave file
+            self._save_reforbit()
 
         # update readback PV
         self.run_callbacks(f'RefOrb{plane.upper()}-RB', list(ref.ravel()))
         self.run_callbacks(f'RefOrbHw{plane.upper()}-Mon', refhw)
         self._update_log('...done!')
         return True
 
+    def _load_reforbit(self):
+        filename = self._const.reforb_fname
+        if not _os.path.isfile(filename):
+            return False
+        self._update_log('Loading RefOrbits from file...')
+        refx, refy = _np.loadtxt(filename, unpack=True)
+        okx = self.set_reforbit('x', refx)
+        oky = self.set_reforbit('y', refy)
+        if all([okx, oky]):
+            msg = 'Loaded RefOrbits!'
+        else:
+            msg = 'ERR:Problem loading RefOrbits from file.'
+        self._update_log(msg)
+        return 'ERR' not in msg
+
+    def _save_reforbit(self):
+        filename = self._const.reforb_fname
+        refx, refy = self._reforb_x, self._reforb_y
+        orbs = _np.array([refx, refy]).T
+        try:
+            path = _os.path.split(filename)[0]
+            _os.makedirs(path, exist_ok=True)
+            _np.savetxt(filename, orbs)
+        except FileNotFoundError:
+            self._update_log('WARN:Could not save ref.orbit to file.')
+
     # --- matrix manipulation ---
 
     def set_respmat(self, value):
         """Set response matrix."""
         self._update_log('Setting New RespMat...')
 
         # check size
@@ -1116,35 +1073,42 @@
         old_ = self._respmat.copy()
         self._respmat = mat
         if not self._calc_matrices():
             self._respmat = old_
             return False
 
         # if ok, save matrix
-        self._save_respmat(matb)
+        if self._init:
+            self._save_respmat(matb)
 
         # update readback pv
         self.run_callbacks('RespMat-RB', list(self._respmat.ravel()))
 
         return True
 
     def _load_respmat(self):
         filename = self._const.respmat_fname
-        if _os.path.isfile(filename):
-            self._update_log('Loading RespMat from file...')
-            if self.set_respmat(_np.loadtxt(filename)):
-                msg = 'Loaded RespMat!'
-            else:
-                msg = 'ERR:Problem loading RespMat from file.'
-            self._update_log(msg)
+        if not _os.path.isfile(filename):
+            return False
+        self._update_log('Loading RespMat from file...')
+        if self.set_respmat(_np.loadtxt(filename)):
+            msg = 'Loaded RespMat!'
+        else:
+            msg = 'ERR:Problem loading RespMat from file.'
+        self._update_log(msg)
+        return 'ERR' not in msg
 
     def _save_respmat(self, mat):
-        path = _os.path.split(self._const.respmat_fname)[0]
-        _os.makedirs(path, exist_ok=True)
-        _np.savetxt(self._const.respmat_fname, mat)
+        try:
+            filename = self._const.respmat_fname
+            path = _os.path.split(filename)[0]
+            _os.makedirs(path, exist_ok=True)
+            _np.savetxt(filename, mat)
+        except FileNotFoundError:
+            self._update_log('WARN:Could not save matrix to file.')
 
     def set_enbllist(self, device, value):
         """Set enable list for device."""
         if self._loop_state:
             self._update_log('ERR:Open loop before continuing.')
             return False
         if self._thread_enbllist is not None and \
@@ -1163,19 +1127,24 @@
 
         # check if matrix is invertible
         self._enable_lists[device] = new
         if not self._calc_matrices():
             self._enable_lists[device] = bkup
             return False
 
-        # handle devices enable configuration
-        self._thread_enbllist = _epics.ca.CAThread(
-            target=self._handle_devices_enblconfig, args=[device, ],
-            daemon=True)
-        self._thread_enbllist.start()
+        # do not set enable lists and save to file in initialization
+        if self._init:
+            # handle devices enable configuration
+            self._thread_enbllist = _epics.ca.CAThread(
+                target=self._handle_devices_enblconfig, args=[device, ],
+                daemon=True)
+            self._thread_enbllist.start()
+
+            # save to autosave files
+            self._save_enbllist(device, _np.array([value], dtype=bool))
 
         # update readback pv
         if device == 'rf':
             self.run_callbacks('UseRF-Sts', bool(value))
         else:
             self.run_callbacks(device.upper()+'EnblList-RB', new)
 
@@ -1215,14 +1184,36 @@
 
     @property
     def corr_enbllist(self):
         """Corrector enable list."""
         enbl = self._enable_lists
         return _np.hstack([enbl['ch'], enbl['cv'], enbl['rf']])
 
+    def _load_enbllist(self, device):
+        filename = getattr(self._const, device+'enbl_fname')
+        if not _os.path.isfile(filename):
+            return
+        okl = self.set_enbllist(device, _np.loadtxt(filename))
+        if okl:
+            msg = f'Loaded {device} enable list!'
+        else:
+            msg = f'ERR:Problem loading {device} enable list from file.'
+        self._update_log(msg)
+        return okl
+
+    def _save_enbllist(self, device, value):
+        try:
+            filename = getattr(self._const, device+'enbl_fname')
+            path = _os.path.split(filename)[0]
+            _os.makedirs(path, exist_ok=True)
+            _np.savetxt(filename, value)
+        except FileNotFoundError:
+            self._update_log(
+                f'WARN:Could not save {device} enable list to file.')
+
     def set_min_sing_value(self, value):
         """Set minimum singular values."""
         bkup = self._min_sing_val
         self._min_sing_val = float(value)
         if not self._calc_matrices():
             self._min_sing_val = bkup
             return False
@@ -1380,16 +1371,14 @@
         """Set response matrix measure state."""
         if value == self._const.MeasRespMatCmd.Start:
             return self._start_meas_respmat()
         if value == self._const.MeasRespMatCmd.Stop:
             return self._stop_meas_respmat()
         if value == self._const.MeasRespMatCmd.Reset:
             return self._reset_meas_respmat()
-        self._meas_respmat_count += 1
-        self.run_callbacks('MeasRespMat-Cmd', self._meas_respmat_count)
         return True
 
     def set_respmat_meas_kick(self, plane, value):
         """Set response matrix measure kick value for plane [urad]."""
         self._meas_respmat_kick[plane] = value
         self.run_callbacks('MeasRespMatKick'+plane.upper()+'-RB', value)
         return True
@@ -1563,16 +1552,15 @@
                      not self._thread_loopstate.is_alive()) or \
                     (self._thread_loopstate is not None and
                      self._thread_loopstate.is_alive() and
                      self._loop_state_lastsp != self._const.LoopState.Open):
                 self._update_log('FATAL:Opening FOFB loop...')
                 self.run_callbacks('LoopState-Sel', self._const.LoopState.Open)
                 self.run_callbacks('LoopState-Sts', self._const.LoopState.Open)
-                self.set_loop_state(
-                    self._const.LoopState.Open, reset=True, abort=True)
+                self.set_loop_state(self._const.LoopState.Open, abort=True)
 
     # --- auxiliary corrector and fofbcontroller methods ---
 
     def _check_corr_connection(self):
         if self._corrs_dev.connected:
             return True
         self._update_log('ERR:Correctors not connected... aborted.')
@@ -1723,15 +1711,16 @@
         self._update_log('ERR:aborted.')
         return False
 
     def _update_fofbctrl_sync_enbllist(self):
         if self._fofbctrl_syncuseenbllist:
             bpmx = self._enable_lists['bpmx']
             bpmy = self._enable_lists['bpmy']
-            dccenbl = _np.logical_or(bpmx, bpmy)
+            mini = self._const.dccenbl_min
+            dccenbl = _np.logical_or.reduce([bpmx, bpmy, mini])
             bpms = self._llfofb_dev.get_dccfmc_visible_bpms([
                 self._const.bpm_names[i] for i, s in enumerate(dccenbl) if s])
             dccenbl = _np.array([b in bpms for b in self._const.bpm_names])
         else:
             dccenbl = _np.ones(self._const.nr_bpms, dtype=bool)
         self._fofbctrl_syncenbllist = dccenbl
         self.run_callbacks('CtrlrSyncEnblList-Mon', dccenbl)
@@ -1887,16 +1876,20 @@
                 cvn, cvl = self._const.cv_names, self._cv_maxacccurr
                 isok = self._corrs_dev.check_fofbacc_satmax(chl, psnames=chn)
                 isok &= self._corrs_dev.check_fofbacc_satmin(-chl, psnames=chn)
                 isok &= self._corrs_dev.check_fofbacc_satmax(cvl, psnames=cvn)
                 isok &= self._corrs_dev.check_fofbacc_satmin(-cvl, psnames=cvn)
                 if not isok:
                     value = _updt_bit(value, 6, 1)
+                # AccDecimationSynced
+                dec = self._corr_accdec_val
+                if not self._corrs_dev.check_fofbacc_decimation(dec):
+                    value = _updt_bit(value, 7, 1)
             else:
-                value = 0b1111111
+                value = 0b11111111
 
             self._corr_status = value
             self.run_callbacks('CorrStatus-Mon', self._corr_status)
 
             ttook = _time.time() - _t0
             tsleep = tplanned - ttook
             if tsleep > 0:
@@ -1952,16 +1945,19 @@
                 count = int(_np.sum(self._fofbctrl_syncenbllist))
                 count_ok = self._llfofb_dev.min_bpm_count == count
                 if not _np.all(sts_ok) or not _np.all(count_ok):
                     value = _updt_bit(value, 8, 1)
                 # LoopInterlockOk
                 if not self._llfofb_dev.interlock_ok:
                     value = _updt_bit(value, 9, 1)
+                # SYSIDExcitationDisabled
+                if not self._llfofb_dev.check_sysid_exc_disabled():
+                    value = _updt_bit(value, 10, 1)
             else:
-                value = 0b1111111111
+                value = 0b11111111111
 
             self._fofbctrl_status = value
             self.run_callbacks('CtrlrStatus-Mon', self._fofbctrl_status)
 
             ttook = _time.time() - _t0
             tsleep = tplanned - ttook
             if tsleep > 0:
```

### Comparing `siriuspy-2.75.0/siriuspy/idff/config.py` & `siriuspy-2.76.0/siriuspy/idff/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,25 +35,25 @@
     def pparameter_pvname(self):
         """Return ID pparameter pvname."""
         config = self._value
         if config:
             kparm = config['pvnames']['pparameter']
             return kparm
         else:
-            raise ValueError('Configuration not loaded!')
+            raise ValueError('Configuration not defined!')
 
     @property
     def kparameter_pvname(self):
         """Return ID kparameter pvname."""
         config = self._value
         if config:
             kparm = config['pvnames']['kparameter']
             return kparm
         else:
-            raise ValueError('Configuration not loaded!')
+            raise ValueError('Configuration not defined!')
 
     @property
     def ch_pvnames(self):
         """Return CH corrector power supply pvnames."""
         return self._get_corr_pvnames('ch1', 'ch2')
 
     @property
@@ -68,15 +68,15 @@
 
     @property
     def polarizations(self):
         """Return list of light polarizations in the IDFF config."""
         if self._value:
             return list(self._value['polarizations'].keys())
         else:
-            raise ValueError('Configuration not loaded!')
+            raise ValueError('Configuration not defined!')
 
     @property
     def value(self):
         """Get configuration."""
         return _dcopy(self._value)
 
     @value.setter
@@ -100,15 +100,15 @@
                     # linear interpolation
                     setpoint = _np.interp(
                         kparameter_value, kparameter_values, table)
                     corr_pvname = self._value['pvnames'][corrlabel]
                     setpoints[corr_pvname] = setpoint
             return setpoints
         else:
-            raise ValueError('Configuration not loaded!')
+            raise ValueError('Configuration not defined!')
 
     @staticmethod
     def create_template_config(idname):
         """Create a template configuration for a given ID type."""
         idff = _IDSearch.conv_idname_2_idff(idname)
 
         # description
@@ -179,15 +179,15 @@
         KPARAM_TOL = 0.1
         poldefs = self._polarization_definitions
         if poldefs is None:
             raise ValueError('No IDFF configuration defined.')
         for pol, val in poldefs.items():
             if pol == 'none':
                 continue
-            if abs(pparameter - val) < PPARAM_TOL:
+            if val is None or abs(pparameter - val) < PPARAM_TOL:
                 return pol
         if abs(kparameter - poldefs['none']) < KPARAM_TOL:
             return 'none'
         return 'not_defined'
 
     def check_valid_value(self, value):
         """."""
@@ -208,15 +208,15 @@
     def _get_corr_pvnames(self, cname1, cname2):
         """Return corrector power supply pvnames."""
         if self._value:
             pvnames = self._value['pvnames']
             corr1, corr2 = pvnames.get(cname1), pvnames.get(cname2)
             return corr1, corr2
         else:
-            raise ValueError('Configuration not loaded!')
+            raise ValueError('Configuration not defined!')
 
     def _set_value(self, value):
         super()._set_value(value)
         self._calc_polariz_defs()
 
     def _calc_polariz_defs(self):
         """."""
```

### Comparing `siriuspy-2.75.0/siriuspy/idff/csdev.py` & `siriuspy-2.76.0/siriuspy/idff/csdev.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ID feedforward database."""
 
 import os as _os
 
 from .. import csdev as _csdev
 from ..namesys import SiriusPVName as _PVName
+from ..search import IDSearch as _IDSearch
 
 
 # --- Enumeration Types ---
 
 class ETypes(_csdev.ETypes):
     """Local enumerate types."""
 
@@ -36,55 +37,55 @@
         self.idname = _PVName(idname)
         self.idffname = 'SI-' + self.idname.sub + ':AP-IDFF'
         ioc_fol = _os.path.join(
             '/home', 'sirius', 'iocs-log', 'si-ap-idff', 'data')
         fname = '_'.join([self.idname.sec, self.idname.sub, self.idname.dev])
         fname = fname.lower()
         self.autosave_fname = _os.path.join(ioc_fol, fname+'.txt')
+        qsnames = _IDSearch.conv_idname_2_idff_qsnames(idname)
+        self.has_qscorrs = True if qsnames else False
 
     def get_propty_database(self):
         """Return property database."""
         dbase = {
             'Version-Cte': {'type': 'str', 'value': 'UNDEF'},
             'Log-Mon': {'type': 'string', 'value': 'Starting...'},
-
             'LoopState-Sel': {
                 'type': 'enum', 'enums': _et.OPEN_CLOSED,
                 'value': self.LoopState.Open},
             'LoopState-Sts': {
                 'type': 'enum', 'enums': _et.OPEN_CLOSED,
                 'value': self.LoopState.Open},
-
             'LoopFreq-SP': {
                 'type': 'float', 'value': self.DEFAULT_LOOP_FREQ,
                 'unit': 'Hz', 'prec': 3, 'lolim': 1e-3, 'hilim': 60},
             'LoopFreq-RB': {
                 'type': 'float', 'value': self.DEFAULT_LOOP_FREQ,
                 'unit': 'Hz', 'prec': 3, 'lolim': 1e-3, 'hilim': 60},
-
-            'ControlQS-Sel': {
-                'type': 'enum', 'enums': _et.DSBL_ENBL,
-                'value': self.DsblEnbl.Enbl,
-                'unit': 'If QS are included in loop'},
-            'ControlQS-Sts': {
-                'type': 'enum', 'enums': _et.DSBL_ENBL,
-                'value': self.DsblEnbl.Enbl,
-                'unit': 'If QS are included in loop'},
-
             'Polarization-Mon': {'type': 'string', 'value': 'none'},
-
             'ConfigName-SP': {'type': 'string', 'value': ''},
             'ConfigName-RB': {'type': 'string', 'value': ''},
             'SOFBMode-Sel': {
                 'type': 'enum', 'enums': _et.DSBL_ENBL,
                 'value': self.DsblEnbl.Dsbl, 'unit': 'sofbmode'},
             'SOFBMode-Sts': {
                 'type': 'enum', 'enums': _et.DSBL_ENBL,
                 'value': self.DsblEnbl.Dsbl, 'unit': 'sofbmode'},
             'CorrConfig-Cmd': {'type': 'int', 'value': 0},
             'CorrStatus-Mon': {'type': 'int', 'value': 0b1111},
             'CorrStatusLabels-Cte': {
                 'type': 'string', 'count': len(self.StsLblsCorr._fields),
                 'value': self.StsLblsCorr._fields}
         }
+        if self.has_qscorrs:
+            dbase.update({
+                'ControlQS-Sel': {
+                    'type': 'enum', 'enums': _et.DSBL_ENBL,
+                    'value': self.DsblEnbl.Enbl,
+                    'unit': 'If QS are included in loop'},
+                'ControlQS-Sts': {
+                    'type': 'enum', 'enums': _et.DSBL_ENBL,
+                    'value': self.DsblEnbl.Enbl,
+                    'unit': 'If QS are included in loop'},
+            })
         dbase = _csdev.add_pvslist_cte(dbase)
         return dbase
```

### Comparing `siriuspy-2.75.0/siriuspy/idff/main.py` & `siriuspy-2.76.0/siriuspy/idff/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from ..pwrsupply.pssofb import PSConnSOFB as _PSConnSOFB
 from ..pwrsupply.pssofb import PSNamesSOFB as _PSNamesSOFB
 
 from .csdev import IDFFConst as _Const, ETypes as _ETypes
 
 
 class App(_Callback):
-    """Main application for handling machine shift."""
+    """Main application for handling IDFF."""
 
     DEF_PS_TIMEOUT = 5  # [s]
 
     def __init__(self, idname):
         """Class constructor."""
         super().__init__()
         self._const = _Const(idname)
```

### Comparing `siriuspy-2.75.0/siriuspy/injctrl/bias_feedback.py` & `siriuspy-2.76.0/siriuspy/injctrl/bias_feedback.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/injctrl/csdev.py` & `siriuspy-2.76.0/siriuspy/injctrl/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/injctrl/main.py` & `siriuspy-2.76.0/siriuspy/injctrl/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/machshift/csdev.py` & `siriuspy-2.76.0/siriuspy/machshift/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/machshift/macreport.py` & `siriuspy-2.76.0/siriuspy/machshift/macreport.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/machshift/macschedule.py` & `siriuspy-2.76.0/siriuspy/machshift/macschedule.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/machshift/main.py` & `siriuspy-2.76.0/siriuspy/machshift/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/machshift/test_macreport.py` & `siriuspy-2.76.0/siriuspy/machshift/test_macreport.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/machshift/utils.py` & `siriuspy-2.76.0/siriuspy/machshift/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/magnet/data.py` & `siriuspy-2.76.0/siriuspy/magnet/data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/magnet/excdata.py` & `siriuspy-2.76.0/siriuspy/magnet/excdata.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/magnet/factory.py` & `siriuspy-2.76.0/siriuspy/magnet/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/magnet/normalizer.py` & `siriuspy-2.76.0/siriuspy/magnet/normalizer.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/magnet/util.py` & `siriuspy-2.76.0/siriuspy/magnet/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/meas/csdev.py` & `siriuspy-2.76.0/siriuspy/meas/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/meas/liemit/csdev.py` & `siriuspy-2.76.0/siriuspy/meas/liemit/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/meas/liemit/main.py` & `siriuspy-2.76.0/siriuspy/meas/liemit/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/meas/lienergy/csdev.py` & `siriuspy-2.76.0/siriuspy/meas/lienergy/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/meas/lienergy/main.py` & `siriuspy-2.76.0/siriuspy/meas/lienergy/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/meas/util.py` & `siriuspy-2.76.0/siriuspy/meas/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/namesys/implementation.py` & `siriuspy-2.76.0/siriuspy/namesys/implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/optics/lattice_survey.py` & `siriuspy-2.76.0/siriuspy/optics/lattice_survey.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,76 +18,135 @@
         "# This file was generated automatically from the data of the \n"\
         "# models of the accelerators in the pymodels repository by the \n"\
         "# function: \n"\
         "#    siriuspy.optics.lattice_survey.generate_model_static_table.\n"\
         "#\n"\
         "# If any model change, please, run the script\n"\
         "# again and copy the generated file to replace this one.\n"
+
     filename = 'magnets-model-data.txt'
 
     with open(filename, 'w') as f:
         f.write(disclaimer)
         f.write('\n\n#Magnets data \n')
         f.write('#-----------')
 
     model = pymodels.si
     acc = model.create_accelerator()
-    _append_mag_data(filename, model, acc, 'Storage Ring (SR)', 'SI')
+    _append_mag_data(filename, model, acc, 'Storage Ring (SI)', 'SI')
 
     model = pymodels.bo
     acc = model.create_accelerator()
     ind = pyaccel.lattice.find_indices(acc, 'fam_name', 'InjSept')
     acc = pyaccel.lattice.shift(acc, ind[0])
-    _append_mag_data(filename, model, acc, 'Booster', 'BO')
+    _append_mag_data(filename, model, acc, 'Booster (BO)', 'BO')
 
     model = pymodels.tb
-    acc, *_ = model.create_accelerator()
-    _append_mag_data(filename, model, acc, 'Booster Transport Line', 'TB')
+    acc, *_ = model.create_accelerator(add_from_li_triplets=False)
+    _append_mag_data(
+        filename, model, acc, 'Booster Transport Line (TB)', 'TB')
 
     model = pymodels.ts
     acc, *_ = model.create_accelerator()
-    _append_mag_data(filename, model, acc, 'SR Transport Line', 'TS')
+    _append_mag_data(filename, model, acc, 'SR Transport Line (TS)', 'TS')
+
+
+def _conv_dev_inst(section, sub, mag_tp, inst):
+    inst_conv = {
+        # additional correctors were added in TS
+        'TS-01': {
+            'CV': {'2': ('CV', '1E2'), '3': ('CV', '2')},
+            },
+        'TS-02': {
+            'CV': {'1': ('CV', '0'), '2': ('CV', '')},
+            },
+        'TS-04': {
+            'CV': {
+                '1': ('CV', '0'), '2': ('CV', '1'),
+                '3': ('CV', '1E2'), '4': ('CV', '2')},
+            },
+        # TB skew quad in the model converted to ch
+        'TB-04': {
+            'CH': {'1': ('CH', '')},
+            'CH': {'2': ('QS', '')},
+            },
+        'TB-04': {
+            'CH': {'': ('CH', '1')},
+            'QS': {'': ('CH', '2')},
+            },
+        }
+    secsub = section + '-' + sub
+    inst_conv_ = inst_conv
+    if secsub in inst_conv_:
+        inst_conv_ = inst_conv_[secsub]
+        if mag_tp in inst_conv_:
+            inst_conv_ = inst_conv_[mag_tp]
+            if inst in inst_conv_:
+                return inst_conv_[inst]
+    return mag_tp, inst
+
+
+def _conv_id_correctors(mag_tp):
+    if mag_tp in ('IDCH', 'IDCV', 'IDQS'):
+        # NOTE: this would issue wrong instances if there were
+        # other CH or CV magnets in insertion device straights, which
+        # is not the case.
+        mag_tp = mag_tp[2:]
+    return mag_tp
+
+
+def _conv_pulsed_magnets(mag_tp, dis):
+    if 'Inj' in mag_tp or 'Eje' in mag_tp or 'Ping' in mag_tp:
+        dis = 'PM'
+    return dis
 
 
 def _append_mag_data(filename, model, acc, label, section):
     fam_data = model.get_family_data(acc)
     pos = pyaccel.lattice.find_spos(acc)
 
+    args = (acc, ) if model == pymodels.tb else ()
     mag_tps = []
-    mag_tps.extend(model.families.families_dipoles())
-    mag_tps.extend(model.families.families_pulsed_magnets())
-    mag_tps.extend(model.families.families_quadrupoles())
-    mag_tps.extend(model.families.families_horizontal_correctors())
-    mag_tps.extend(model.families.families_vertical_correctors())
-    mag_tps.extend(model.families.families_sextupoles())
-    mag_tps.extend(model.families.families_skew_correctors())
-    if section.lower().startswith('si'):
-        mag_tps.extend(model.families.families_id_correctors())
+    mag_tps.extend(model.families.families_dipoles(*args))
+    mag_tps.extend(model.families.families_pulsed_magnets(*args))
+    mag_tps.extend(model.families.families_quadrupoles(*args))
+    mag_tps.extend(model.families.families_horizontal_correctors(*args))
+    mag_tps.extend(model.families.families_vertical_correctors(*args))
+    mag_tps.extend(model.families.families_sextupoles(*args))
+    mag_tps.extend(model.families.families_skew_correctors(*args))
 
     mag_data = dict()
     for mag_tp in mag_tps:
         inds = fam_data[mag_tp]['index']
         subs = fam_data[mag_tp]['subsection']
         insts = fam_data[mag_tp]['instance']
         for ind, inst, sub in zip(inds, insts, subs):
+            val = (pos[ind[-1]+1] + pos[ind[0]]) / 2  # elem position
+            # special conversions
+            mag_tp_, inst_, dis_ = mag_tp, inst, 'MA'
+            mag_tp_ = _conv_id_correctors(mag_tp_)
+            dis_ = _conv_pulsed_magnets(mag_tp_, dis_)
+            mag_tp_, inst_ = _conv_dev_inst(section, sub, mag_tp_, inst_)
             name = _join_name(
-                sec=section, dis='MA', dev=mag_tp, sub=sub, idx=inst)
-            val = (pos[ind[-1]+1] + pos[ind[0]]) / 2
-            mag_data[name] = {'pos': val}
+                sec=section, dis=dis_, dev=mag_tp_, sub=sub, idx=inst_)
+            mag_data[name] = val
+
+    # order by spos
+    mags = list(mag_data.keys())
+    mpos = list(mag_data.values())
+    mpos, mags = zip(*sorted(zip(mpos, mags)))
 
-    mags = sorted(mag_data.keys())
     with open(filename, 'a') as f:
         f.write('\n\n\n# '+label+'\n')
         f.write('#'+57*'-' + '\n')
         f.write("#{mag:20s} {pos:^20s}\n".format(
             mag='Name', pos='Position @ center [m]'))
         f.write('#'+57*'-' + '\n')
-        for mag in mags:
-            f.write("{mag:20s} {pos:^20.4f}\n".format(
-                mag=mag, **mag_data[mag]))
+        for mag, pos in zip(mags, mpos):
+            f.write(f'{mag:20s} {pos:>20.4f}\n')
 
 
 def generate_bpm_static_table():
     """."""
     disclaimer = \
         "# This file was generated automatically from the data of the files\n"\
         "# in the subfolder Mapeamento_placas_MicroTCA_vs_BPMs and the\n"\
@@ -140,14 +199,15 @@
     bpms, bpos = [], []
     for ind, inst, sub in zip(inds, insts, subs):
         name = _join_name(sec=section, dis='DI', dev='BPM', sub=sub, idx=inst)
         bpms.append(name)
         bpos.append(pos[ind])
     _write_to_file(filename, bpms, bpos, label)
 
+
 def _append_bpm_data_bl(filename, acc, all_bpms, label):
     pos = pyaccel.lattice.find_spos(acc)
 
     mcs = pyaccel.lattice.find_indices(acc, 'fam_name', 'mc')
 
     bpms_bc = [bpm for bpm in all_bpms if bpm.sub.endswith('BCFE')]
     secs = [int(bpm.sub[:2]) for bpm in bpms_bc]
```

### Comparing `siriuspy-2.75.0/siriuspy/opticscorr/base.py` & `siriuspy-2.76.0/siriuspy/opticscorr/base.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/opticscorr/chrom.py` & `siriuspy-2.76.0/siriuspy/opticscorr/chrom.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/opticscorr/csdev.py` & `siriuspy-2.76.0/siriuspy/opticscorr/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/opticscorr/opticscorr.py` & `siriuspy-2.76.0/siriuspy/opticscorr/opticscorr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/opticscorr/tune.py` & `siriuspy-2.76.0/siriuspy/opticscorr/tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/opticscorr/utils.py` & `siriuspy-2.76.0/siriuspy/opticscorr/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/oscilloscope/keysight.py` & `siriuspy-2.76.0/siriuspy/oscilloscope/keysight.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/oscilloscope/scopes.py` & `siriuspy-2.76.0/siriuspy/oscilloscope/scopes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/posang/csdev.py` & `siriuspy-2.76.0/siriuspy/posang/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/posang/main.py` & `siriuspy-2.76.0/siriuspy/posang/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/posang/utils.py` & `siriuspy-2.76.0/siriuspy/posang/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/pwrsupply/beaglebone.py` & `siriuspy-2.76.0/siriuspy/pwrsupply/beaglebone.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/pwrsupply/bsmp/commands.py` & `siriuspy-2.76.0/siriuspy/pwrsupply/bsmp/commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/pwrsupply/bsmp/constants.py` & `siriuspy-2.76.0/siriuspy/pwrsupply/bsmp/constants.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/pwrsupply/bsmp/entities.py` & `siriuspy-2.76.0/siriuspy/pwrsupply/bsmp/entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/pwrsupply/bsmp/factory.py` & `siriuspy-2.76.0/siriuspy/pwrsupply/bsmp/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/pwrsupply/csdev.py` & `siriuspy-2.76.0/siriuspy/pwrsupply/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/pwrsupply/data.py` & `siriuspy-2.76.0/siriuspy/pwrsupply/data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/pwrsupply/factory.py` & `siriuspy-2.76.0/siriuspy/pwrsupply/factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/__init__.py` & `siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/pru.py` & `siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/pru.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/prucontroller.py` & `siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/prucontroller.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/prucparms.py` & `siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/prucparms.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/psdevstate.py` & `siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/psdevstate.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/pwrsupply/pructrl/udc.py` & `siriuspy-2.76.0/siriuspy/pwrsupply/pructrl/udc.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/__init__.py` & `siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/__init__.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/pscontroller.py` & `siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/pscontroller.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/pscreaders.py` & `siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/pscreaders.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/pscstatus.py` & `siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/pscstatus.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/pscwriters.py` & `siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/pscwriters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/pwrsupply/psctrl/psmodel.py` & `siriuspy-2.76.0/siriuspy/pwrsupply/psctrl/psmodel.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/pwrsupply/pssofb.py` & `siriuspy-2.76.0/siriuspy/pwrsupply/pssofb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/pwrsupply/siggen.py` & `siriuspy-2.76.0/siriuspy/pwrsupply/siggen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/ramp/conn.py` & `siriuspy-2.76.0/siriuspy/ramp/conn.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/ramp/magnet.py` & `siriuspy-2.76.0/siriuspy/ramp/magnet.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/ramp/ramp.py` & `siriuspy-2.76.0/siriuspy/ramp/ramp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/ramp/reconst_factory.py` & `siriuspy-2.76.0/siriuspy/ramp/reconst_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/ramp/test_reconst_factory.py` & `siriuspy-2.76.0/siriuspy/ramp/test_reconst_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/ramp/testwfm.py` & `siriuspy-2.76.0/siriuspy/ramp/testwfm.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/ramp/util.py` & `siriuspy-2.76.0/siriuspy/ramp/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/ramp/waveform.py` & `siriuspy-2.76.0/siriuspy/ramp/waveform.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/search/bpms_search.py` & `siriuspy-2.76.0/siriuspy/search/bpms_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/search/hl_time_search.py` & `siriuspy-2.76.0/siriuspy/search/hl_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/search/id_search.py` & `siriuspy-2.76.0/siriuspy/search/id_search.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,21 +10,22 @@
     # NOTE: Maybe we should move these mappings to
     # static tables in our cs-constants server.
 
     # NOTE: see
     # https://wiki-sirius.lnls.br/mediawiki/index.php/Machine:Insertion_Devices
 
     _beamline2idname = {
-        'CARNAUBA': 'SI-06SB:ID-APU22',
-        'CATERETE': 'SI-07SP:ID-APU22',
-        'EMA':      'SI-08SB:ID-APU22',
-        'MANACA':   'SI-09SA:ID-APU22',
-        'SABIA':    'SI-10SB:ID-EPU50',
-        'IPE':      'SI-11SP:ID-APU58',
-        'PAINEIRA': 'SI-14SB:ID-WIG180',
+        'CARNAUBA': 'SI-06SB:ID-APU22',  # titular: VPU19
+        'CATERETE': 'SI-07SP:ID-APU22',  # titular: VPU19
+        'EMA':      'SI-08SB:ID-APU22',  # titular: IVU18
+        'MANACA':   'SI-09SA:ID-APU22',  # titular: 2 x APU22
+        'SABIA':    'SI-10SB:ID-EPU50',  # titular: 2 x DELTA52
+        'IPE':      'SI-11SP:ID-APU58',  # titular: 2 x APPLE-II
+        'PAINEIRA': 'SI-14SB:ID-WIG180',  # titular: IVU18
+        'SAPUCAIA': 'SI-17SA:ID-PAPU50',  # titular: 2 x APU22
     }
 
     _idname2beamline = {v: k for k, v in _beamline2idname.items()}
 
     _idname_2_idff = {
         'SI-06SB:ID-APU22': None,
         'SI-07SP:ID-APU22': None,
@@ -47,14 +48,23 @@
         'SI-14SB:ID-WIG180': {
             'polarizations': ('horizontal', ),
             'pparameter': None,
             'kparameter': 'SI-14SB:ID-WIG180:Gap-Mon',
             'ch1': 'SI-14SB:PS-CH-1:Current-SP',  # upstream
             'ch2': 'SI-14SB:PS-CH-2:Current-SP',  # downstream
         },
+        'SI-17SA:ID-PAPU50': {
+            'polarizations': ('horizontal', ),
+            'pparameter': None,
+            'kparameter': 'SI-17SA:ID-PAPU50:Phase-Mon',
+            'ch1': 'SI-17SA:PS-CH-1:Current-SP',  # upstream
+            'ch2': 'SI-17SA:PS-CH-2:Current-SP',  # downstream
+            'cv1': 'SI-17SA:PS-CV-1:Current-SP',
+            'cv2': 'SI-17SA:PS-CV-2:Current-SP',
+        },
     }
 
     @staticmethod
     def get_idnames(filters=None):
         """Return a sorted and filtered list of all ID names."""
         idnames_list = list(IDSearch._idname2beamline.keys())
         idnames = _Filter.process_filters(idnames_list, filters=filters)
@@ -96,16 +106,20 @@
         """Return the IDFF dictionary for a given ID name."""
         return dict(IDSearch._idname_2_idff[idname])
 
     @staticmethod
     def conv_idname_2_pparameter_propty(idname):
         """."""
         idff = IDSearch.conv_idname_2_idff(idname)
-        pvname = _SiriusPVName(idff['pparameter'])
-        return pvname.propty
+        pparameter = idff['pparameter']
+        if pparameter:
+            pvname = _SiriusPVName(pparameter)
+            return pvname.propty
+        else:
+            return None
 
     @staticmethod
     def conv_idname_2_kparameter_propty(idname):
         """."""
         idff = IDSearch.conv_idname_2_idff(idname)
         pvname = _SiriusPVName(idff['kparameter'])
         return pvname.propty
```

### Comparing `siriuspy-2.75.0/siriuspy/search/ioc_search.py` & `siriuspy-2.76.0/siriuspy/search/ioc_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/search/ll_time_search.py` & `siriuspy-2.76.0/siriuspy/search/ll_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/search/ma_search.py` & `siriuspy-2.76.0/siriuspy/search/ma_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/search/ps_search.py` & `siriuspy-2.76.0/siriuspy/search/ps_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/simul/simfactory.py` & `siriuspy-2.76.0/siriuspy/simul/simfactory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/simul/simps.py` & `siriuspy-2.76.0/siriuspy/simul/simps.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/simul/simpv.py` & `siriuspy-2.76.0/siriuspy/simul/simpv.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/simul/simulation.py` & `siriuspy-2.76.0/siriuspy/simul/simulation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/simul/simulator.py` & `siriuspy-2.76.0/siriuspy/simul/simulator.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/sofb/base_class.py` & `siriuspy-2.76.0/siriuspy/sofb/base_class.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/sofb/bpms.py` & `siriuspy-2.76.0/siriuspy/sofb/bpms.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/sofb/correctors.py` & `siriuspy-2.76.0/siriuspy/sofb/correctors.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/sofb/csdev.py` & `siriuspy-2.76.0/siriuspy/sofb/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/sofb/main.py` & `siriuspy-2.76.0/siriuspy/sofb/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,17 @@
         self._ref_corr_kicks = None
         self._thread = None
         self._havebeam_pv = _PV('SI-Glob:AP-CurrInfo:StoredEBeam-Mon')
 
         self.orbit = orbit
         self.correctors = correctors
         self.matrix = matrix
+        self._amcs = [
+            _PV(f'IA-{i:02d}RaBPM:TI-AMCFPGAEVR:RefClkLocked-Mon')
+            for i in range(1, 21)]
 
     def get_map2write(self):
         """Get the database of the class."""
         dbase = {
             'LoopState-Sel': self.set_auto_corr,
             'LoopFreq-SP': self.set_auto_corr_frequency,
             'LoopPrintEveryNumIters-SP': self.set_print_every_num_iters,
@@ -179,14 +182,30 @@
     @property
     def havebeam(self):
         """."""
         if self._tests or self.acc != 'SI':
             return True
         return self._havebeam_pv.connected and self._havebeam_pv.value
 
+    @property
+    def is_amc_connected(self):
+        """."""
+        for amc in self._amcs:
+            if not amc.connected:
+                return False
+        return True
+
+    @property
+    def is_amc_locked(self):
+        """."""
+        for amc in self._amcs:
+            if not amc.connected or not amc.value:
+                return False
+        return True
+
     def process(self):
         """Run continuously in the main thread."""
         time0 = _time()
         self.status
         tfin = _time()
         dtime = INTERVAL - (tfin-time0)
         if dtime > 0:
@@ -734,15 +753,15 @@
             'MeasRespMat-Mon', self._csorb.MeasRespMatMon.Completed)
         self._measuring_respmat = False
         msg = 'RespMat Measurement Completed!'
         self._update_log(msg)
         _log.info(msg)
 
     def _do_drive(self):
-        self.run_callbacks('DriveState-Sts', 1)
+        self.run_callbacks('DriveState-Sts', self._csorb.DriveState.Closed)
 
         freqdiv = self._drive_divisor
         nrcycles = self._drive_nrcycles
         ampl = self._drive_amplitude
         phase = self._drive_phase / 180 * _np.pi
         corridx = self._drive_corr_index
         bpmidx = self._drive_bpm_index
@@ -795,18 +814,18 @@
         ret = self.correctors.apply_kicks(refkicks)
         if len(data) < 6:
             data.extend((6-len(data)) * [0.0])
         self.run_callbacks('DriveData-Mon', data)
         msg = 'Drive Loop opened!'
         self._update_log(msg)
         _log.info(msg)
-        self.run_callbacks('DriveState-Sts', 0)
+        self.run_callbacks('DriveState-Sts', self._csorb.DriveState.Open)
 
     def _do_auto_corr(self):
-        self.run_callbacks('LoopState-Sts', 1)
+        self.run_callbacks('LoopState-Sts', self._csorb.LoopState.Closed)
         times, rets = [], []
         tim0 = _time()
         bpmsfreq = self._csorb.BPMsFreq
         zer = _np.zeros(self._csorb.nr_corrs, dtype=float)
         self._pid_errs = [zer, zer.copy(), zer.copy()]
         fofb = self.fofb
         refx0 = refy0 = None
@@ -832,17 +851,27 @@
                 msg = 'Trigger ready!'
                 self._update_log(msg)
                 _log.info(msg)
 
         tims = []
         while self._loop_state == self._csorb.LoopState.Closed:
             if not self.havebeam:
-                msg = 'ERR: Cannot Correct, We do not have stored beam!'
+                msg = 'ERR: We do not have stored beam!'
                 self._update_log(msg)
-                _log.info(msg)
+                _log.error(msg[5:])
+                break
+            if not self.is_amc_connected:
+                msg = 'ERR: At least one AMC is not connected!'
+                self._update_log(msg)
+                _log.error(msg[5:])
+                break
+            if not self.is_amc_locked:
+                msg = 'ERR: At least one AMC is not locked!'
+                self._update_log(msg)
+                _log.error(msg[5:])
                 break
             itern = len(times)
             self.run_callbacks('LoopNumIters-Mon', itern)
             if itern >= self._loop_print_every_num_iter:
                 _Thread(
                     target=self._print_auto_corr_info,
                     args=(times, rets, _time()-tim0), daemon=True).start()
@@ -883,44 +912,36 @@
 
             orb = self._interact_with_fofb_in_calc_kicks(orb)
 
             dkicks = self.matrix.calc_kicks(orb)
             tims.append(_time())
 
             if not self._check_valid_orbit(orb):
-                self._loop_state = self._csorb.LoopState.Open
-                self.run_callbacks('LoopState-Sel', 0)
                 break
 
             dkicks = self._process_pid(dkicks, interval)
 
             kicks, dkicks = self._process_kicks(
                 self._ref_corr_kicks, dkicks, apply_gain=False)
             if kicks is None:
-                self._loop_state = self._csorb.LoopState.Open
-                self.run_callbacks('LoopState-Sel', 0)
                 break
 
             kicks = self._interact_with_fofb_in_apply_kicks(
                 kicks, dkicks, refx0, refy0)
             if kicks is None:
-                self._loop_state = self._csorb.LoopState.Open
-                self.run_callbacks('LoopState-Sel', 0)
                 break
             tims.append(_time())
 
             ret = self.correctors.apply_kicks(kicks)
             rets.append(ret)
             tims.append(_time())
             tims.append(tims[1])  # to compute total time - get_orbit
             times.append(tims)
             # if ret == -2:
             if ret < 0:  # change here for debug
-                self._loop_state = self._csorb.LoopState.Open
-                self.run_callbacks('LoopState-Sel', 0)
                 break
             elif ret == -1:
                 # means that correctors are not ready yet
                 # skip this iteration
                 continue
 
         if self._loop_use_pssofb:
@@ -938,18 +959,22 @@
                 _log.info(msg)
                 self.run_callbacks('CorrSync-Sts', self._csorb.CorrSync.Event)
                 self.correctors.set_corrs_mode(self._csorb.CorrSync.Event)
                 msg = 'Trigger ready!'
                 self._update_log(msg)
                 _log.info(msg)
 
+        if self._loop_state == self._csorb.LoopState.Closed:
+            self._loop_state = self._csorb.LoopState.Open
+            self.run_callbacks('LoopState-Sel', self._csorb.LoopState.Open)
+
         msg = 'Loop opened!'
         self._update_log(msg)
         _log.info(msg)
-        self.run_callbacks('LoopState-Sts', 0)
+        self.run_callbacks('LoopState-Sts', self._csorb.LoopState.Open)
 
     def _process_pid(self, dkicks, interval):
         """Velocity algorithm of PID."""
         if dkicks is None:
             return None
 
         self._pid_errs.append(dkicks.copy())
@@ -1081,16 +1106,16 @@
             # But it seems this may also be a possibility:
             # fofb.refx = refx - dorb[:dorb.size//2]
             # fofb.refy = refy - dorb[dorb.size//2:]
             fofb.cmd_fofbctrl_syncreforb()
 
         if self._download_fofb_kicks and fofb.loop_state:
             # NOTE: Do not download kicks from correctors not in the loop:
-            kickch = fofb.kickch.copy()
-            kickcv = fofb.kickcv.copy()
+            kickch = fofb.kickch_acc.copy()
+            kickcv = fofb.kickcv_acc.copy()
             kickch[~fofb.chenbl] = 0
             kickcv[~fofb.cvenbl] = 0
 
             kicks_fofb = _np.r_[kickch, kickcv, 0]
             dorb = _np.dot(fofb.respmat, kicks_fofb)
             # NOTE: calc_kicks return the kicks to correct dorb, which means
             # that a minus sign is already applied by this method. To negate
```

### Comparing `siriuspy-2.75.0/siriuspy/sofb/matrix.py` & `siriuspy-2.76.0/siriuspy/sofb/matrix.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/sofb/orbit.py` & `siriuspy-2.76.0/siriuspy/sofb/orbit.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/sofb/utils.py` & `siriuspy-2.76.0/siriuspy/sofb/utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/stabinfo/csdev.py` & `siriuspy-2.76.0/siriuspy/stabinfo/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/stabinfo/main.py` & `siriuspy-2.76.0/siriuspy/stabinfo/main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/thread.py` & `siriuspy-2.76.0/siriuspy/thread.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/timesys/csdev.py` & `siriuspy-2.76.0/siriuspy/timesys/csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/timesys/hl_classes.py` & `siriuspy-2.76.0/siriuspy/timesys/hl_classes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/timesys/ll_classes.py` & `siriuspy-2.76.0/siriuspy/timesys/ll_classes.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/timesys/plot_network.py` & `siriuspy-2.76.0/siriuspy/timesys/plot_network.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/timesys/static_table.py` & `siriuspy-2.76.0/siriuspy/timesys/static_table.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy/util.py` & `siriuspy-2.76.0/siriuspy/util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/siriuspy.egg-info/PKG-INFO` & `siriuspy-2.76.0/siriuspy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siriuspy
-Version: 2.75.0
+Version: 2.76.0
 Summary: Development packages for Sirius
 Home-page: https://github.com/lnls-sirius/dev-packages
 Download-URL: https://github.com/lnls-sirius/dev-packages
 Author: lnls-sirius
 License: GNU GPLv3
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
```

### Comparing `siriuspy-2.75.0/siriuspy.egg-info/SOURCES.txt` & `siriuspy-2.76.0/siriuspy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 siriuspy/cycle/conn.py
 siriuspy/cycle/fc_cycle_data.py
 siriuspy/cycle/li_cycle_data.py
 siriuspy/cycle/main.py
 siriuspy/cycle/util.py
 siriuspy/devices/__init__.py
 siriuspy/devices/bbb.py
+siriuspy/devices/blctrl.py
 siriuspy/devices/bpm.py
 siriuspy/devices/currinfo.py
 siriuspy/devices/dcct.py
 siriuspy/devices/device.py
 siriuspy/devices/dvf.py
 siriuspy/devices/egun.py
 siriuspy/devices/energy.py
@@ -136,14 +137,18 @@
 siriuspy/diagsys/pudiag/csdev.py
 siriuspy/diagsys/pudiag/main.py
 siriuspy/diagsys/pudiag/pvs.py
 siriuspy/diagsys/rfdiag/__init__.py
 siriuspy/diagsys/rfdiag/csdev.py
 siriuspy/diagsys/rfdiag/main.py
 siriuspy/diagsys/rfdiag/pvs.py
+siriuspy/dvfimgproc/__init__.py
+siriuspy/dvfimgproc/csdev.py
+siriuspy/dvfimgproc/main.py
+siriuspy/dvfimgproc/meas.py
 siriuspy/epics/__init__.py
 siriuspy/epics/multiproc.py
 siriuspy/epics/properties.py
 siriuspy/epics/pv.py
 siriuspy/epics/pv_fake.py
 siriuspy/epics/pv_time_serie.py
 siriuspy/epics/threading.py
```

### Comparing `siriuspy-2.75.0/tests/bsmp/test_bsmp.py` & `siriuspy-2.76.0/tests/bsmp/test_bsmp.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/bsmp/test_commands.py` & `siriuspy-2.76.0/tests/bsmp/test_commands.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/bsmp/test_entities.py` & `siriuspy-2.76.0/tests/bsmp/test_entities.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/bsmp/test_serial.py` & `siriuspy-2.76.0/tests/bsmp/test_serial.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/bsmp/test_types.py` & `siriuspy-2.76.0/tests/bsmp/test_types.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/clientconfigdb/test_configdb_client.py` & `siriuspy-2.76.0/tests/clientconfigdb/test_configdb_client.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/clientweb/test_implementation.py` & `siriuspy-2.76.0/tests/clientweb/test_implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/currinfo/lifetime/test_main.py` & `siriuspy-2.76.0/tests/currinfo/lifetime/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/currinfo/test_csdev.py` & `siriuspy-2.76.0/tests/currinfo/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/currinfo/test_main.py` & `siriuspy-2.76.0/tests/currinfo/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/magnet/test_factory.py` & `siriuspy-2.76.0/tests/magnet/test_factory.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/magnet/tests_normalizer.py` & `siriuspy-2.76.0/tests/magnet/tests_normalizer.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/mock_servweb.py` & `siriuspy-2.76.0/tests/mock_servweb.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/namesys/test_implementation.py` & `siriuspy-2.76.0/tests/namesys/test_implementation.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/opticscorr/test_chrom.py` & `siriuspy-2.76.0/tests/opticscorr/test_chrom.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/opticscorr/test_csdev.py` & `siriuspy-2.76.0/tests/opticscorr/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/opticscorr/test_opticscorr.py` & `siriuspy-2.76.0/tests/opticscorr/test_opticscorr.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/opticscorr/test_tune.py` & `siriuspy-2.76.0/tests/opticscorr/test_tune.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/opticscorr/test_utils.py` & `siriuspy-2.76.0/tests/opticscorr/test_utils.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/posang/test_csdev.py` & `siriuspy-2.76.0/tests/posang/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/posang/test_main.py` & `siriuspy-2.76.0/tests/posang/test_main.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/pwrsupply/db.py` & `siriuspy-2.76.0/tests/pwrsupply/db.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/pwrsupply/pructrl/test_pru.py` & `siriuspy-2.76.0/tests/pwrsupply/pructrl/test_pru.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/pwrsupply/psctrl/test_pscwriters.py` & `siriuspy-2.76.0/tests/pwrsupply/psctrl/test_pscwriters.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/pwrsupply/test_csdev.py` & `siriuspy-2.76.0/tests/pwrsupply/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/pwrsupply/test_data.py` & `siriuspy-2.76.0/tests/pwrsupply/test_data.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/pwrsupply/test_siggen.py` & `siriuspy-2.76.0/tests/pwrsupply/test_siggen.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/pwrsupply/variables.py` & `siriuspy-2.76.0/tests/pwrsupply/variables.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/ramp/test_magnet.py` & `siriuspy-2.76.0/tests/ramp/test_magnet.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/ramp/test_waveform.py` & `siriuspy-2.76.0/tests/ramp/test_waveform.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/search/test_hl_time_search.py` & `siriuspy-2.76.0/tests/search/test_hl_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/search/test_init.py` & `siriuspy-2.76.0/tests/search/test_init.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/search/test_ll_time_search.py` & `siriuspy-2.76.0/tests/search/test_ll_time_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/search/test_ma_search.py` & `siriuspy-2.76.0/tests/search/test_ma_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/search/test_ps_search.py` & `siriuspy-2.76.0/tests/search/test_ps_search.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/test_callbacks.py` & `siriuspy-2.76.0/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/test_csdev.py` & `siriuspy-2.76.0/tests/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/test_envars.py` & `siriuspy-2.76.0/tests/test_envars.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/test_util.py` & `siriuspy-2.76.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/timesys/test_csdev.py` & `siriuspy-2.76.0/tests/timesys/test_csdev.py`

 * *Files identical despite different names*

### Comparing `siriuspy-2.75.0/tests/timesys/test_plot_network.py` & `siriuspy-2.76.0/tests/timesys/test_plot_network.py`

 * *Files identical despite different names*

