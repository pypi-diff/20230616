# Comparing `tmp/SGTPy-0.0.8.tar.gz` & `tmp/SGTPy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SGTPy-0.0.8.tar", last modified: Fri Jun  4 15:26:46 2021, max compression
+gzip compressed data, was "dist\SGTPy-0.0.9.tar", last modified: Wed Jun 16 20:56:02 2021, max compression
```

## Comparing `SGTPy-0.0.8.tar` & `SGTPy-0.0.9.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxrwx   0        0        0        0 2021-06-04 15:26:46.840422 SGTPy-0.0.8/
--rw-rw-rw-   0        0        0     1174 2020-08-11 18:01:10.000000 SGTPy-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0      179 2019-11-03 07:46:32.000000 SGTPy-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      967 2021-06-04 15:26:46.837428 SGTPy-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4381 2021-03-20 14:58:37.000000 SGTPy-0.0.8/README.rst
-drwxrwxrwx   0        0        0        0 2021-06-04 15:26:46.085338 SGTPy-0.0.8/SGTPy/
--rw-rw-rw-   0        0        0      260 2020-07-24 13:56:16.000000 SGTPy-0.0.8/SGTPy/__init__.py
--rw-rw-rw-   0        0        0      222 2020-07-23 20:54:44.000000 SGTPy-0.0.8/SGTPy/constants.py
-drwxrwxrwx   0        0        0        0 2021-06-04 15:26:46.353018 SGTPy-0.0.8/SGTPy/equilibrium/
--rw-rw-rw-   0        0        0     1245 2020-07-24 13:38:20.000000 SGTPy-0.0.8/SGTPy/equilibrium/__init__.py
--rw-rw-rw-   0        0        0     9127 2021-04-07 13:13:02.000000 SGTPy-0.0.8/SGTPy/equilibrium/bubble.py
--rw-rw-rw-   0        0        0     8846 2021-04-07 13:14:12.000000 SGTPy-0.0.8/SGTPy/equilibrium/dew.py
--rw-rw-rw-   0        0        0     2916 2021-03-31 13:08:02.000000 SGTPy-0.0.8/SGTPy/equilibrium/ell.py
--rw-rw-rw-   0        0        0      614 2020-06-26 15:31:36.000000 SGTPy-0.0.8/SGTPy/equilibrium/equilibriumresult.py
--rw-rw-rw-   0        0        0     6232 2021-04-07 19:44:50.000000 SGTPy-0.0.8/SGTPy/equilibrium/flash.py
--rw-rw-rw-   0        0        0     4119 2021-04-07 13:10:31.000000 SGTPy-0.0.8/SGTPy/equilibrium/hazb.py
--rw-rw-rw-   0        0        0    12039 2021-04-16 19:33:58.000000 SGTPy-0.0.8/SGTPy/equilibrium/hazt.py
--rw-rw-rw-   0        0        0     7128 2021-04-16 19:55:24.000000 SGTPy-0.0.8/SGTPy/equilibrium/multiflash.py
--rw-rw-rw-   0        0        0     8684 2021-06-04 13:32:53.000000 SGTPy-0.0.8/SGTPy/equilibrium/stability.py
-drwxrwxrwx   0        0        0        0 2021-06-04 15:26:46.412129 SGTPy-0.0.8/SGTPy/fit/
--rw-rw-rw-   0        0        0      181 2020-07-24 18:47:26.000000 SGTPy-0.0.8/SGTPy/fit/__init__.py
--rw-rw-rw-   0        0        0     1374 2021-06-04 13:31:59.000000 SGTPy-0.0.8/SGTPy/fit/fit_beta.py
--rw-rw-rw-   0        0        0     1568 2021-06-04 13:32:10.000000 SGTPy-0.0.8/SGTPy/fit/fit_cii.py
--rw-rw-rw-   0        0        0     4333 2021-06-04 13:32:16.000000 SGTPy-0.0.8/SGTPy/fit/fitbinary.py
--rw-rw-rw-   0        0        0     2565 2020-12-23 14:27:37.000000 SGTPy-0.0.8/SGTPy/fit/fitmulticomponent.py
--rw-rw-rw-   0        0        0     1035 2020-07-24 13:37:02.000000 SGTPy-0.0.8/SGTPy/math.py
--rw-rw-rw-   0        0        0    10549 2020-12-29 14:01:54.000000 SGTPy-0.0.8/SGTPy/mixture.py
-drwxrwxrwx   0        0        0        0 2021-06-04 15:26:46.568625 SGTPy-0.0.8/SGTPy/mixtures/
--rw-rw-rw-   0        0        0     5454 2021-06-04 13:30:36.000000 SGTPy-0.0.8/SGTPy/mixtures/B_monomer.py
--rw-rw-rw-   0        0        0      162 2020-06-29 19:47:54.000000 SGTPy-0.0.8/SGTPy/mixtures/__init__.py
--rw-rw-rw-   0        0        0     1084 2021-06-04 13:29:41.000000 SGTPy-0.0.8/SGTPy/mixtures/a1_monomer.py
--rw-rw-rw-   0        0        0    15344 2021-06-04 13:29:52.000000 SGTPy-0.0.8/SGTPy/mixtures/a1sB_monomer.py
--rw-rw-rw-   0        0        0     6542 2021-06-04 13:29:47.000000 SGTPy-0.0.8/SGTPy/mixtures/a1s_monomer.py
--rw-rw-rw-   0        0        0     2817 2021-06-04 13:29:57.000000 SGTPy-0.0.8/SGTPy/mixtures/a2_monomer.py
--rw-rw-rw-   0        0        0     1724 2021-06-04 13:30:03.000000 SGTPy-0.0.8/SGTPy/mixtures/a2new_chain.py
--rw-rw-rw-   0        0        0     2036 2021-06-04 13:30:09.000000 SGTPy-0.0.8/SGTPy/mixtures/a3_monomer.py
--rw-rw-rw-   0        0        0     3914 2021-06-04 13:30:14.000000 SGTPy-0.0.8/SGTPy/mixtures/ahs_monomer.py
--rw-rw-rw-   0        0        0    32344 2021-06-04 13:30:21.000000 SGTPy-0.0.8/SGTPy/mixtures/ares.py
--rw-rw-rw-   0        0        0     8260 2021-06-04 13:30:26.000000 SGTPy-0.0.8/SGTPy/mixtures/association_aux.py
--rw-rw-rw-   0        0        0     4053 2021-06-04 13:30:41.000000 SGTPy-0.0.8/SGTPy/mixtures/density_solver.py
--rw-rw-rw-   0        0        0     1504 2021-06-04 13:30:47.000000 SGTPy-0.0.8/SGTPy/mixtures/g1sigma_chain.py
--rw-rw-rw-   0        0        0     2288 2021-06-04 13:30:52.000000 SGTPy-0.0.8/SGTPy/mixtures/g2mca_chain.py
--rw-rw-rw-   0        0        0     1780 2021-06-04 13:30:59.000000 SGTPy-0.0.8/SGTPy/mixtures/gammac_chain.py
--rw-rw-rw-   0        0        0     5810 2021-06-04 13:31:05.000000 SGTPy-0.0.8/SGTPy/mixtures/ghs_chain.py
--rw-rw-rw-   0        0        0     1714 2021-06-04 13:31:10.000000 SGTPy-0.0.8/SGTPy/mixtures/ideal.py
--rw-rw-rw-   0        0        0     1754 2021-06-04 13:31:16.000000 SGTPy-0.0.8/SGTPy/mixtures/lngmie_chain.py
--rw-rw-rw-   0        0        0     9453 2021-06-04 13:31:22.000000 SGTPy-0.0.8/SGTPy/mixtures/monomer_aux.py
--rw-rw-rw-   0        0        0     7724 2021-06-04 13:31:27.000000 SGTPy-0.0.8/SGTPy/mixtures/polarGV.py
--rw-rw-rw-   0        0        0    66438 2021-06-04 13:31:33.000000 SGTPy-0.0.8/SGTPy/mixtures/saftvrmiemix.py
-drwxrwxrwx   0        0        0        0 2021-06-04 15:26:46.751546 SGTPy-0.0.8/SGTPy/pure/
--rw-rw-rw-   0        0        0     1801 2021-06-04 13:27:54.000000 SGTPy-0.0.8/SGTPy/pure/B_monomer.py
--rw-rw-rw-   0        0        0      680 2021-06-04 13:28:12.000000 SGTPy-0.0.8/SGTPy/pure/EquilibriumResult.py
--rw-rw-rw-   0        0        0      163 2020-06-29 19:47:54.000000 SGTPy-0.0.8/SGTPy/pure/__init__.py
--rw-rw-rw-   0        0        0     4528 2021-06-04 13:26:26.000000 SGTPy-0.0.8/SGTPy/pure/a1sB_monomer.py
--rw-rw-rw-   0        0        0     2352 2021-06-04 13:26:20.000000 SGTPy-0.0.8/SGTPy/pure/a1s_monomer.py
--rw-rw-rw-   0        0        0     2162 2021-06-04 13:27:01.000000 SGTPy-0.0.8/SGTPy/pure/a2m_monomer.py
--rw-rw-rw-   0        0        0      889 2021-06-04 13:27:21.000000 SGTPy-0.0.8/SGTPy/pure/a3m_monomer.py
--rw-rw-rw-   0        0        0      473 2021-06-04 13:27:10.000000 SGTPy-0.0.8/SGTPy/pure/aHS_monomer.py
--rw-rw-rw-   0        0        0    10514 2021-06-04 13:27:42.000000 SGTPy-0.0.8/SGTPy/pure/ares.py
--rw-rw-rw-   0        0        0     2933 2021-06-04 13:27:47.000000 SGTPy-0.0.8/SGTPy/pure/association_aux.py
--rw-rw-rw-   0        0        0     1871 2021-06-04 13:27:59.000000 SGTPy-0.0.8/SGTPy/pure/critical_pure.py
--rw-rw-rw-   0        0        0     4002 2021-06-04 13:28:07.000000 SGTPy-0.0.8/SGTPy/pure/density_solver.py
--rw-rw-rw-   0        0        0      674 2021-06-04 13:28:18.000000 SGTPy-0.0.8/SGTPy/pure/g1sigma_chain.py
--rw-rw-rw-   0        0        0     2032 2021-06-04 13:28:24.000000 SGTPy-0.0.8/SGTPy/pure/g2sigma_chain.py
--rw-rw-rw-   0        0        0     2691 2021-06-04 13:28:30.000000 SGTPy-0.0.8/SGTPy/pure/gdHS_chain.py
--rw-rw-rw-   0        0        0      677 2021-06-04 13:28:42.000000 SGTPy-0.0.8/SGTPy/pure/ideal.py
--rw-rw-rw-   0        0        0     1042 2021-06-04 13:28:51.000000 SGTPy-0.0.8/SGTPy/pure/lngmie_chain.py
--rw-rw-rw-   0        0        0     2921 2021-06-04 13:28:58.000000 SGTPy-0.0.8/SGTPy/pure/monomer_aux.py
--rw-rw-rw-   0        0        0     3437 2021-06-04 13:29:03.000000 SGTPy-0.0.8/SGTPy/pure/polarGV.py
--rw-rw-rw-   0        0        0     3331 2021-06-04 13:29:09.000000 SGTPy-0.0.8/SGTPy/pure/psat_saft.py
--rw-rw-rw-   0        0        0    48925 2021-06-04 13:29:15.000000 SGTPy-0.0.8/SGTPy/pure/saftvrmie.py
--rw-rw-rw-   0        0        0     1380 2021-06-04 13:29:21.000000 SGTPy-0.0.8/SGTPy/pure/tsat_saft.py
--rw-rw-rw-   0        0        0      606 2020-12-29 15:07:45.000000 SGTPy-0.0.8/SGTPy/saft.py
--rw-rw-rw-   0        0        0     3131 2021-06-04 13:33:24.000000 SGTPy-0.0.8/SGTPy/saft_forcefield.py
-drwxrwxrwx   0        0        0        0 2021-06-04 15:26:46.827424 SGTPy-0.0.8/SGTPy/sgt/
--rw-rw-rw-   0        0        0      398 2020-08-03 01:24:56.000000 SGTPy-0.0.8/SGTPy/sgt/__init__.py
--rw-rw-rw-   0        0        0    13102 2021-03-31 15:13:27.000000 SGTPy-0.0.8/SGTPy/sgt/coloc_z.py
--rw-rw-rw-   0        0        0     8139 2021-03-31 15:10:37.000000 SGTPy-0.0.8/SGTPy/sgt/coloc_z_ds.py
--rw-rw-rw-   0        0        0     6470 2021-03-31 15:12:51.000000 SGTPy-0.0.8/SGTPy/sgt/linear_spot.py
--rw-rw-rw-   0        0        0     3112 2021-03-31 14:50:01.000000 SGTPy-0.0.8/SGTPy/sgt/path_sk.py
--rw-rw-rw-   0        0        0     2678 2021-03-31 14:50:23.000000 SGTPy-0.0.8/SGTPy/sgt/reference_component.py
--rw-rw-rw-   0        0        0     2064 2021-03-31 14:52:52.000000 SGTPy-0.0.8/SGTPy/sgt/sgt_beta0.py
--rw-rw-rw-   0        0        0     2258 2021-03-31 14:54:00.000000 SGTPy-0.0.8/SGTPy/sgt/sgtpuros.py
--rw-rw-rw-   0        0        0      610 2020-06-26 14:53:10.000000 SGTPy-0.0.8/SGTPy/sgt/tensionresult.py
-drwxrwxrwx   0        0        0        0 2021-06-04 15:26:46.184448 SGTPy-0.0.8/SGTPy/src/
--rw-rw-rw-   0        0        0      436 2019-02-18 14:25:54.000000 SGTPy-0.0.8/SGTPy/src/cijmix_cy.pyx
--rw-rw-rw-   0        0        0     4837 2020-03-11 01:03:06.000000 SGTPy-0.0.8/SGTPy/src/coloc_cy.pyx
-drwxrwxrwx   0        0        0        0 2021-06-04 15:26:46.168823 SGTPy-0.0.8/SGTPy.egg-info/
--rw-rw-rw-   0        0        0      967 2021-06-04 15:26:44.000000 SGTPy-0.0.8/SGTPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2243 2021-06-04 15:26:45.000000 SGTPy-0.0.8/SGTPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-04 15:26:44.000000 SGTPy-0.0.8/SGTPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-07-24 15:36:30.000000 SGTPy-0.0.8/SGTPy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       19 2021-06-04 15:26:44.000000 SGTPy-0.0.8/SGTPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2021-06-04 15:26:44.000000 SGTPy-0.0.8/SGTPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      472 2020-08-11 18:02:40.000000 SGTPy-0.0.8/long_description.rst
--rw-rw-rw-   0        0        0       42 2021-06-04 15:26:46.842422 SGTPy-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1686 2021-06-04 15:24:06.000000 SGTPy-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-06-16 20:56:02.670240 SGTPy-0.0.9/
+-rw-rw-rw-   0        0        0     1174 2020-08-11 18:01:10.000000 SGTPy-0.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      179 2019-11-03 07:46:32.000000 SGTPy-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      967 2021-06-16 20:56:02.670240 SGTPy-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4381 2021-03-20 14:58:37.000000 SGTPy-0.0.9/README.rst
+drwxrwxrwx   0        0        0        0 2021-06-16 20:56:02.244251 SGTPy-0.0.9/SGTPy/
+-rw-rw-rw-   0        0        0      260 2020-07-24 13:56:16.000000 SGTPy-0.0.9/SGTPy/__init__.py
+-rw-rw-rw-   0        0        0      222 2020-07-23 20:54:44.000000 SGTPy-0.0.9/SGTPy/constants.py
+drwxrwxrwx   0        0        0        0 2021-06-16 20:56:02.375237 SGTPy-0.0.9/SGTPy/equilibrium/
+-rw-rw-rw-   0        0        0     1245 2021-06-11 19:26:31.000000 SGTPy-0.0.9/SGTPy/equilibrium/__init__.py
+-rw-rw-rw-   0        0        0     9127 2021-04-07 13:13:02.000000 SGTPy-0.0.9/SGTPy/equilibrium/bubble.py
+-rw-rw-rw-   0        0        0     8846 2021-04-07 13:14:12.000000 SGTPy-0.0.9/SGTPy/equilibrium/dew.py
+-rw-rw-rw-   0        0        0      614 2020-06-26 15:31:36.000000 SGTPy-0.0.9/SGTPy/equilibrium/equilibriumresult.py
+-rw-rw-rw-   0        0        0     6232 2021-04-07 19:44:50.000000 SGTPy-0.0.9/SGTPy/equilibrium/flash.py
+-rw-rw-rw-   0        0        0     4119 2021-04-07 13:10:31.000000 SGTPy-0.0.9/SGTPy/equilibrium/hazb.py
+-rw-rw-rw-   0        0        0    12039 2021-04-16 19:33:58.000000 SGTPy-0.0.9/SGTPy/equilibrium/hazt.py
+-rw-rw-rw-   0        0        0     2916 2021-03-31 13:08:02.000000 SGTPy-0.0.9/SGTPy/equilibrium/lle.py
+-rw-rw-rw-   0        0        0     7128 2021-04-16 19:55:24.000000 SGTPy-0.0.9/SGTPy/equilibrium/multiflash.py
+-rw-rw-rw-   0        0        0     8684 2021-06-04 13:32:53.000000 SGTPy-0.0.9/SGTPy/equilibrium/stability.py
+drwxrwxrwx   0        0        0        0 2021-06-16 20:56:02.389246 SGTPy-0.0.9/SGTPy/fit/
+-rw-rw-rw-   0        0        0      181 2020-07-24 18:47:26.000000 SGTPy-0.0.9/SGTPy/fit/__init__.py
+-rw-rw-rw-   0        0        0     1374 2021-06-04 13:31:59.000000 SGTPy-0.0.9/SGTPy/fit/fit_beta.py
+-rw-rw-rw-   0        0        0     1568 2021-06-04 13:32:10.000000 SGTPy-0.0.9/SGTPy/fit/fit_cii.py
+-rw-rw-rw-   0        0        0     7689 2021-06-16 19:55:46.000000 SGTPy-0.0.9/SGTPy/fit/fitbinary.py
+-rw-rw-rw-   0        0        0     2764 2021-06-16 20:54:33.000000 SGTPy-0.0.9/SGTPy/fit/fitmulticomponent.py
+-rw-rw-rw-   0        0        0     1035 2020-07-24 13:37:02.000000 SGTPy-0.0.9/SGTPy/math.py
+-rw-rw-rw-   0        0        0    10549 2020-12-29 14:01:54.000000 SGTPy-0.0.9/SGTPy/mixture.py
+drwxrwxrwx   0        0        0        0 2021-06-16 20:56:02.526240 SGTPy-0.0.9/SGTPy/mixtures/
+-rw-rw-rw-   0        0        0     5454 2021-06-04 13:30:36.000000 SGTPy-0.0.9/SGTPy/mixtures/B_monomer.py
+-rw-rw-rw-   0        0        0      162 2020-06-29 19:47:54.000000 SGTPy-0.0.9/SGTPy/mixtures/__init__.py
+-rw-rw-rw-   0        0        0     1084 2021-06-04 13:29:41.000000 SGTPy-0.0.9/SGTPy/mixtures/a1_monomer.py
+-rw-rw-rw-   0        0        0    15344 2021-06-04 13:29:52.000000 SGTPy-0.0.9/SGTPy/mixtures/a1sB_monomer.py
+-rw-rw-rw-   0        0        0     6542 2021-06-04 13:29:47.000000 SGTPy-0.0.9/SGTPy/mixtures/a1s_monomer.py
+-rw-rw-rw-   0        0        0     2817 2021-06-04 13:29:57.000000 SGTPy-0.0.9/SGTPy/mixtures/a2_monomer.py
+-rw-rw-rw-   0        0        0     1724 2021-06-04 13:30:03.000000 SGTPy-0.0.9/SGTPy/mixtures/a2new_chain.py
+-rw-rw-rw-   0        0        0     2036 2021-06-04 13:30:09.000000 SGTPy-0.0.9/SGTPy/mixtures/a3_monomer.py
+-rw-rw-rw-   0        0        0     3914 2021-06-04 13:30:14.000000 SGTPy-0.0.9/SGTPy/mixtures/ahs_monomer.py
+-rw-rw-rw-   0        0        0    32344 2021-06-04 13:30:21.000000 SGTPy-0.0.9/SGTPy/mixtures/ares.py
+-rw-rw-rw-   0        0        0     8260 2021-06-04 13:30:26.000000 SGTPy-0.0.9/SGTPy/mixtures/association_aux.py
+-rw-rw-rw-   0        0        0     4053 2021-06-04 13:30:41.000000 SGTPy-0.0.9/SGTPy/mixtures/density_solver.py
+-rw-rw-rw-   0        0        0     1504 2021-06-04 13:30:47.000000 SGTPy-0.0.9/SGTPy/mixtures/g1sigma_chain.py
+-rw-rw-rw-   0        0        0     2288 2021-06-04 13:30:52.000000 SGTPy-0.0.9/SGTPy/mixtures/g2mca_chain.py
+-rw-rw-rw-   0        0        0     1780 2021-06-04 13:30:59.000000 SGTPy-0.0.9/SGTPy/mixtures/gammac_chain.py
+-rw-rw-rw-   0        0        0     5810 2021-06-04 13:31:05.000000 SGTPy-0.0.9/SGTPy/mixtures/ghs_chain.py
+-rw-rw-rw-   0        0        0     1714 2021-06-04 13:31:10.000000 SGTPy-0.0.9/SGTPy/mixtures/ideal.py
+-rw-rw-rw-   0        0        0     1754 2021-06-04 13:31:16.000000 SGTPy-0.0.9/SGTPy/mixtures/lngmie_chain.py
+-rw-rw-rw-   0        0        0     9453 2021-06-04 13:31:22.000000 SGTPy-0.0.9/SGTPy/mixtures/monomer_aux.py
+-rw-rw-rw-   0        0        0     7724 2021-06-04 13:31:27.000000 SGTPy-0.0.9/SGTPy/mixtures/polarGV.py
+-rw-rw-rw-   0        0        0    66438 2021-06-04 13:31:33.000000 SGTPy-0.0.9/SGTPy/mixtures/saftvrmiemix.py
+drwxrwxrwx   0        0        0        0 2021-06-16 20:56:02.618240 SGTPy-0.0.9/SGTPy/pure/
+-rw-rw-rw-   0        0        0     1801 2021-06-04 13:27:54.000000 SGTPy-0.0.9/SGTPy/pure/B_monomer.py
+-rw-rw-rw-   0        0        0      680 2021-06-04 13:28:12.000000 SGTPy-0.0.9/SGTPy/pure/EquilibriumResult.py
+-rw-rw-rw-   0        0        0      163 2020-06-29 19:47:54.000000 SGTPy-0.0.9/SGTPy/pure/__init__.py
+-rw-rw-rw-   0        0        0     4528 2021-06-04 13:26:26.000000 SGTPy-0.0.9/SGTPy/pure/a1sB_monomer.py
+-rw-rw-rw-   0        0        0     2352 2021-06-04 13:26:20.000000 SGTPy-0.0.9/SGTPy/pure/a1s_monomer.py
+-rw-rw-rw-   0        0        0     2162 2021-06-04 13:27:01.000000 SGTPy-0.0.9/SGTPy/pure/a2m_monomer.py
+-rw-rw-rw-   0        0        0      889 2021-06-04 13:27:21.000000 SGTPy-0.0.9/SGTPy/pure/a3m_monomer.py
+-rw-rw-rw-   0        0        0      473 2021-06-04 13:27:10.000000 SGTPy-0.0.9/SGTPy/pure/aHS_monomer.py
+-rw-rw-rw-   0        0        0    10514 2021-06-04 13:27:42.000000 SGTPy-0.0.9/SGTPy/pure/ares.py
+-rw-rw-rw-   0        0        0     2933 2021-06-04 13:27:47.000000 SGTPy-0.0.9/SGTPy/pure/association_aux.py
+-rw-rw-rw-   0        0        0     1871 2021-06-04 13:27:59.000000 SGTPy-0.0.9/SGTPy/pure/critical_pure.py
+-rw-rw-rw-   0        0        0     4002 2021-06-04 13:28:07.000000 SGTPy-0.0.9/SGTPy/pure/density_solver.py
+-rw-rw-rw-   0        0        0      674 2021-06-04 13:28:18.000000 SGTPy-0.0.9/SGTPy/pure/g1sigma_chain.py
+-rw-rw-rw-   0        0        0     2032 2021-06-04 13:28:24.000000 SGTPy-0.0.9/SGTPy/pure/g2sigma_chain.py
+-rw-rw-rw-   0        0        0     2691 2021-06-04 13:28:30.000000 SGTPy-0.0.9/SGTPy/pure/gdHS_chain.py
+-rw-rw-rw-   0        0        0      677 2021-06-04 13:28:42.000000 SGTPy-0.0.9/SGTPy/pure/ideal.py
+-rw-rw-rw-   0        0        0     1042 2021-06-04 13:28:51.000000 SGTPy-0.0.9/SGTPy/pure/lngmie_chain.py
+-rw-rw-rw-   0        0        0     2921 2021-06-04 13:28:58.000000 SGTPy-0.0.9/SGTPy/pure/monomer_aux.py
+-rw-rw-rw-   0        0        0     3437 2021-06-04 13:29:03.000000 SGTPy-0.0.9/SGTPy/pure/polarGV.py
+-rw-rw-rw-   0        0        0     3331 2021-06-04 13:29:09.000000 SGTPy-0.0.9/SGTPy/pure/psat_saft.py
+-rw-rw-rw-   0        0        0    48928 2021-06-11 19:13:11.000000 SGTPy-0.0.9/SGTPy/pure/saftvrmie.py
+-rw-rw-rw-   0        0        0     1380 2021-06-04 13:29:21.000000 SGTPy-0.0.9/SGTPy/pure/tsat_saft.py
+-rw-rw-rw-   0        0        0      606 2020-12-29 15:07:45.000000 SGTPy-0.0.9/SGTPy/saft.py
+-rw-rw-rw-   0        0        0     3131 2021-06-04 13:33:24.000000 SGTPy-0.0.9/SGTPy/saft_forcefield.py
+drwxrwxrwx   0        0        0        0 2021-06-16 20:56:02.667239 SGTPy-0.0.9/SGTPy/sgt/
+-rw-rw-rw-   0        0        0      397 2021-06-11 19:09:19.000000 SGTPy-0.0.9/SGTPy/sgt/__init__.py
+-rw-rw-rw-   0        0        0    13102 2021-03-31 15:13:27.000000 SGTPy-0.0.9/SGTPy/sgt/coloc_z.py
+-rw-rw-rw-   0        0        0     8139 2021-03-31 15:10:37.000000 SGTPy-0.0.9/SGTPy/sgt/coloc_z_ds.py
+-rw-rw-rw-   0        0        0     6470 2021-03-31 15:12:51.000000 SGTPy-0.0.9/SGTPy/sgt/linear_spot.py
+-rw-rw-rw-   0        0        0     3112 2021-03-31 14:50:01.000000 SGTPy-0.0.9/SGTPy/sgt/path_sk.py
+-rw-rw-rw-   0        0        0     2678 2021-03-31 14:50:23.000000 SGTPy-0.0.9/SGTPy/sgt/reference_component.py
+-rw-rw-rw-   0        0        0     2064 2021-03-31 14:52:52.000000 SGTPy-0.0.9/SGTPy/sgt/sgt_beta0.py
+-rw-rw-rw-   0        0        0     2266 2021-06-11 19:19:00.000000 SGTPy-0.0.9/SGTPy/sgt/sgtpure.py
+-rw-rw-rw-   0        0        0      610 2020-06-26 14:53:10.000000 SGTPy-0.0.9/SGTPy/sgt/tensionresult.py
+drwxrwxrwx   0        0        0        0 2021-06-16 20:56:02.289237 SGTPy-0.0.9/SGTPy/src/
+-rw-rw-rw-   0        0        0      436 2019-02-18 14:25:54.000000 SGTPy-0.0.9/SGTPy/src/cijmix_cy.pyx
+-rw-rw-rw-   0        0        0     4837 2020-03-11 01:03:06.000000 SGTPy-0.0.9/SGTPy/src/coloc_cy.pyx
+drwxrwxrwx   0        0        0        0 2021-06-16 20:56:02.269255 SGTPy-0.0.9/SGTPy.egg-info/
+-rw-rw-rw-   0        0        0      967 2021-06-16 20:56:01.000000 SGTPy-0.0.9/SGTPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2242 2021-06-16 20:56:01.000000 SGTPy-0.0.9/SGTPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-06-16 20:56:01.000000 SGTPy-0.0.9/SGTPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2020-07-24 15:36:30.000000 SGTPy-0.0.9/SGTPy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       19 2021-06-16 20:56:01.000000 SGTPy-0.0.9/SGTPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2021-06-16 20:56:01.000000 SGTPy-0.0.9/SGTPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      472 2020-08-11 18:02:40.000000 SGTPy-0.0.9/long_description.rst
+-rw-rw-rw-   0        0        0       42 2021-06-16 20:56:02.671239 SGTPy-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1686 2021-06-16 20:54:15.000000 SGTPy-0.0.9/setup.py
```

### Comparing `SGTPy-0.0.8/LICENSE.txt` & `SGTPy-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/PKG-INFO` & `SGTPy-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: SGTPy
-Version: 0.0.8
+Version: 0.0.9
 Summary: SAFT-VR-MIE EOS and SGT
 Home-page: https://github.com/gustavochm/SGTPy
 Author: Gustavo Chaparro Maldonado, Andres Mejia Matallana, Erich A. Muller
 Author-email: gustavochaparro@udec.cl
 License: MIT
 Download-URL: https://github.com/gustavochm/SGTPy.git
 Description: SGTPy is an open-source python package of SAFT-VR-Mie Equation of State (EOS).
```

### Comparing `SGTPy-0.0.8/README.rst` & `SGTPy-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/equilibrium/__init__.py` & `SGTPy-0.0.9/SGTPy/equilibrium/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,8 +30,8 @@
 from .bubble import bubblePy, bubbleTy
 from .dew import dewPx, dewTx
 from .flash import flash
 from .multiflash import multiflash
 from .hazt import haz, vlle
 from .hazb import vlleb
 from .stability import tpd_min, tpd_minimas, lle_init, gmix
-from .ell import lle
+from .lle import lle
```

### Comparing `SGTPy-0.0.8/SGTPy/equilibrium/bubble.py` & `SGTPy-0.0.9/SGTPy/equilibrium/bubble.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/equilibrium/dew.py` & `SGTPy-0.0.9/SGTPy/equilibrium/dew.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/equilibrium/ell.py` & `SGTPy-0.0.9/SGTPy/equilibrium/lle.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/equilibrium/equilibriumresult.py` & `SGTPy-0.0.9/SGTPy/equilibrium/equilibriumresult.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/equilibrium/flash.py` & `SGTPy-0.0.9/SGTPy/equilibrium/flash.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/equilibrium/hazb.py` & `SGTPy-0.0.9/SGTPy/equilibrium/hazb.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/equilibrium/hazt.py` & `SGTPy-0.0.9/SGTPy/equilibrium/hazt.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/equilibrium/multiflash.py` & `SGTPy-0.0.9/SGTPy/equilibrium/multiflash.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/equilibrium/stability.py` & `SGTPy-0.0.9/SGTPy/equilibrium/stability.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/fit/fit_beta.py` & `SGTPy-0.0.9/SGTPy/fit/fit_beta.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/fit/fit_cii.py` & `SGTPy-0.0.9/SGTPy/fit/fit_cii.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/fit/fitmulticomponent.py` & `SGTPy-0.0.9/SGTPy/fit/fitmulticomponent.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import division, print_function, absolute_import
 import numpy as np
 from ..equilibrium import bubblePy, lle, tpd_min, vlleb
 
 
-def fobj_elv(model, Xexp, Yexp, Texp, Pexp):
+def fobj_vle(model, Xexp, Yexp, Texp, Pexp, weights_vle=[1., 1.]):
     """
     Objective function to fit parameters for VLE in multicomponent mixtures
     """
 
     n = Pexp.shape[0]
     n1, n2 = Xexp.shape
     if n2 == n:
@@ -16,21 +16,21 @@
 
     P = np.zeros(n)  # n,
     Y = np.zeros_like(Xexp)  # nc,n
 
     for i in range(n):
         Y[i], P[i] = bubblePy(Yexp[i], Pexp[i], Xexp[i], Texp[i], model)
 
-    error = ((Y-Yexp)**2).sum()
-    error += ((P/Pexp-1)**2).sum()
+    error = weights_vle[0] * np.sum((Y-Yexp)**2)
+    error += weights_vle[1] * np.sum((P/Pexp-1)**2)
     error /= n
     return error
 
 
-def fobj_ell(model, Xexp, Wexp, Texp, Pexp, tpd=True):
+def fobj_lle(model, Xexp, Wexp, Texp, Pexp, tpd=True, weights_lle=[1., 1.]):
     """
     Objective function to fit parameters for LLE in multicomponent mixtures
     """
     n = Pexp.shape[0]
     n1, n2 = Xexp.shape
     if n2 == n:
         Xexp = Xexp.T
@@ -45,21 +45,22 @@
             X0, tpd = tpd_min(Xexp[i], Z[i], Texp[i], Pexp[i], model, 'L', 'L')
             W0, tpd = tpd_min(Wexp[i], Z[i], Texp[i], Pexp[i], model, 'L', 'L')
         else:
             X0 = Xexp[i]
             W0 = Wexp[i]
         X[i], W[i], beta = lle(X0, W0, Z[i], Texp[i], Pexp[i], model)
 
-    error = ((X-Xexp)**2).sum()
-    error += ((W-Wexp)**2).sum()
+    error = weights_lle[0] * np.sum((X-Xexp)**2)
+    error += weights_lle[1] * np.sum((W-Wexp)**2)
     error /= n
     return error
 
 
-def fobj_hazb(model, Xellv, Wellv, Yellv, Tellv, Pellv, info=[1, 1, 1]):
+def fobj_vlleb(model, Xellv, Wellv, Yellv, Tellv, Pellv,
+               weights_vlleb=[1., 1., 1., 1.]):
     """
     Objective function to fit parameters for VLLE in binary mixtures
     """
     n = len(Tellv)
     n1, n2 = Xellv.shape
     if n2 == n:
         Xellv = Xellv.T
@@ -79,14 +80,15 @@
             W0, tpd = tpd_min(Wellv[i], Zll[i], Tellv[i], Pellv[i],
                               model, 'L', 'L')
             X[i], W[i], Y[i], P[i] = vlleb(X0, W0, Yellv[i], Pellv[i],
                                            Tellv[i], 'T', model)
         except:
             pass
 
-    error = info[0]*((X-Xellv)**2).sum()
-    error += info[1]*((W-Wellv)**2).sum()
-    error += info[2]*((Y-Yellv)**2).sum()
-    error += ((P/Pellv-1)**2).sum()
+    error = weights_vlleb[0] * np.sum((X-Xellv)**2)
+    error += weights_vlleb[1] * np.sum((W-Wellv)**2)
+    error += weights_vlleb[2] * np.sum((Y-Yellv)**2)
+    error += weights_vlleb[3] * np.sum((P/Pellv-1)**2)
+
     error /= n
 
     return error
```

### Comparing `SGTPy-0.0.8/SGTPy/math.py` & `SGTPy-0.0.9/SGTPy/math.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/mixture.py` & `SGTPy-0.0.9/SGTPy/mixture.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/mixtures/B_monomer.py` & `SGTPy-0.0.9/SGTPy/mixtures/B_monomer.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/mixtures/a1_monomer.py` & `SGTPy-0.0.9/SGTPy/mixtures/a1_monomer.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/mixtures/a1sB_monomer.py` & `SGTPy-0.0.9/SGTPy/mixtures/a1sB_monomer.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/mixtures/a1s_monomer.py` & `SGTPy-0.0.9/SGTPy/mixtures/a1s_monomer.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/mixtures/a2_monomer.py` & `SGTPy-0.0.9/SGTPy/mixtures/a2_monomer.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/mixtures/a2new_chain.py` & `SGTPy-0.0.9/SGTPy/mixtures/a2new_chain.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/mixtures/a3_monomer.py` & `SGTPy-0.0.9/SGTPy/mixtures/a3_monomer.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/mixtures/ahs_monomer.py` & `SGTPy-0.0.9/SGTPy/mixtures/ahs_monomer.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/mixtures/ares.py` & `SGTPy-0.0.9/SGTPy/mixtures/ares.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/mixtures/association_aux.py` & `SGTPy-0.0.9/SGTPy/mixtures/association_aux.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/mixtures/density_solver.py` & `SGTPy-0.0.9/SGTPy/mixtures/density_solver.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/mixtures/g1sigma_chain.py` & `SGTPy-0.0.9/SGTPy/mixtures/g1sigma_chain.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/mixtures/g2mca_chain.py` & `SGTPy-0.0.9/SGTPy/mixtures/g2mca_chain.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/mixtures/gammac_chain.py` & `SGTPy-0.0.9/SGTPy/mixtures/gammac_chain.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/mixtures/ghs_chain.py` & `SGTPy-0.0.9/SGTPy/mixtures/ghs_chain.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/mixtures/ideal.py` & `SGTPy-0.0.9/SGTPy/mixtures/ideal.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/mixtures/lngmie_chain.py` & `SGTPy-0.0.9/SGTPy/mixtures/lngmie_chain.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/mixtures/monomer_aux.py` & `SGTPy-0.0.9/SGTPy/mixtures/monomer_aux.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/mixtures/polarGV.py` & `SGTPy-0.0.9/SGTPy/mixtures/polarGV.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/mixtures/saftvrmiemix.py` & `SGTPy-0.0.9/SGTPy/mixtures/saftvrmiemix.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/pure/B_monomer.py` & `SGTPy-0.0.9/SGTPy/pure/B_monomer.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/pure/EquilibriumResult.py` & `SGTPy-0.0.9/SGTPy/pure/EquilibriumResult.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/pure/a1sB_monomer.py` & `SGTPy-0.0.9/SGTPy/pure/a1sB_monomer.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/pure/a1s_monomer.py` & `SGTPy-0.0.9/SGTPy/pure/a1s_monomer.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/pure/a2m_monomer.py` & `SGTPy-0.0.9/SGTPy/pure/a2m_monomer.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/pure/a3m_monomer.py` & `SGTPy-0.0.9/SGTPy/pure/a3m_monomer.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/pure/ares.py` & `SGTPy-0.0.9/SGTPy/pure/ares.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/pure/association_aux.py` & `SGTPy-0.0.9/SGTPy/pure/association_aux.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/pure/critical_pure.py` & `SGTPy-0.0.9/SGTPy/pure/critical_pure.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/pure/density_solver.py` & `SGTPy-0.0.9/SGTPy/pure/density_solver.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/pure/g1sigma_chain.py` & `SGTPy-0.0.9/SGTPy/pure/g1sigma_chain.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/pure/g2sigma_chain.py` & `SGTPy-0.0.9/SGTPy/pure/g2sigma_chain.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/pure/gdHS_chain.py` & `SGTPy-0.0.9/SGTPy/pure/gdHS_chain.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/pure/ideal.py` & `SGTPy-0.0.9/SGTPy/pure/ideal.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/pure/lngmie_chain.py` & `SGTPy-0.0.9/SGTPy/pure/lngmie_chain.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/pure/monomer_aux.py` & `SGTPy-0.0.9/SGTPy/pure/monomer_aux.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/pure/polarGV.py` & `SGTPy-0.0.9/SGTPy/pure/polarGV.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/pure/psat_saft.py` & `SGTPy-0.0.9/SGTPy/pure/psat_saft.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/pure/saftvrmie.py` & `SGTPy-0.0.9/SGTPy/pure/saftvrmie.py`

 * *Files 0% similar despite different names*

```diff
@@ -1004,17 +1004,17 @@
             factor to obtain dimentionless density (mol/m3 -> mol/m3)
         tenfactor : float
             factor to obtain dimentionless surface tension (mN/m)
         zfactor : float
             factor to obtain dimentionless distance  (Amstrong -> m)
         '''
 
-        Tfactor = 1
-        Pfactor = 1
-        rofactor = 1
+        Tfactor = 1.
+        Pfactor = 1.
+        rofactor = 1.
         tenfactor = np.sqrt(self.cii) * 1000  # To give tension in mN/m
         zfactor = 10**-10
 
         return Tfactor, Pfactor, rofactor, tenfactor, zfactor
 
     def sgt_adim_fit(self, T):
```

### Comparing `SGTPy-0.0.8/SGTPy/pure/tsat_saft.py` & `SGTPy-0.0.9/SGTPy/pure/tsat_saft.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/saft.py` & `SGTPy-0.0.9/SGTPy/saft.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/saft_forcefield.py` & `SGTPy-0.0.9/SGTPy/saft_forcefield.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/sgt/coloc_z.py` & `SGTPy-0.0.9/SGTPy/sgt/coloc_z.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/sgt/coloc_z_ds.py` & `SGTPy-0.0.9/SGTPy/sgt/coloc_z_ds.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/sgt/linear_spot.py` & `SGTPy-0.0.9/SGTPy/sgt/linear_spot.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/sgt/path_sk.py` & `SGTPy-0.0.9/SGTPy/sgt/path_sk.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/sgt/reference_component.py` & `SGTPy-0.0.9/SGTPy/sgt/reference_component.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/sgt/sgt_beta0.py` & `SGTPy-0.0.9/SGTPy/sgt/sgt_beta0.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/sgt/sgtpuros.py` & `SGTPy-0.0.9/SGTPy/sgt/sgtpure.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,17 +62,17 @@
         dOm[i], Xass = model.dOm_aux(roi[i], temp_aux, mu0, Pad, Xass)
 
     tenint = np.nan_to_num(np.sqrt(2*dOm))
     ten = np.dot(wreal, tenint)
     ten *= tenfactor
 
     if full_output:
-        zint = np.sqrt(1/(2*dOm))
+        zint = np.sqrt(model.cii/(2*dOm))
         z = np.cumsum(wreal*zint)
-        z *= zfactor
+        z /= zfactor
         roi /= rofactor
         dictresult = {'tension': ten, 'rho': roi, 'z': z,
                       'GPT': dOm}
         out = TensionResult(dictresult)
         return out
 
     return ten
```

### Comparing `SGTPy-0.0.8/SGTPy/sgt/tensionresult.py` & `SGTPy-0.0.9/SGTPy/sgt/tensionresult.py`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy/src/coloc_cy.pyx` & `SGTPy-0.0.9/SGTPy/src/coloc_cy.pyx`

 * *Files identical despite different names*

### Comparing `SGTPy-0.0.8/SGTPy.egg-info/PKG-INFO` & `SGTPy-0.0.9/SGTPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: SGTPy
-Version: 0.0.8
+Version: 0.0.9
 Summary: SAFT-VR-MIE EOS and SGT
 Home-page: https://github.com/gustavochm/SGTPy
 Author: Gustavo Chaparro Maldonado, Andres Mejia Matallana, Erich A. Muller
 Author-email: gustavochaparro@udec.cl
 License: MIT
 Download-URL: https://github.com/gustavochm/SGTPy.git
 Description: SGTPy is an open-source python package of SAFT-VR-Mie Equation of State (EOS).
```

### Comparing `SGTPy-0.0.8/SGTPy.egg-info/SOURCES.txt` & `SGTPy-0.0.9/SGTPy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 SGTPy.egg-info/requires.txt
 SGTPy.egg-info/top_level.txt
 SGTPy/src/cijmix_cy.pyx
 SGTPy/src/coloc_cy.pyx
 SGTPy/equilibrium/__init__.py
 SGTPy/equilibrium/bubble.py
 SGTPy/equilibrium/dew.py
-SGTPy/equilibrium/ell.py
 SGTPy/equilibrium/equilibriumresult.py
 SGTPy/equilibrium/flash.py
 SGTPy/equilibrium/hazb.py
 SGTPy/equilibrium/hazt.py
+SGTPy/equilibrium/lle.py
 SGTPy/equilibrium/multiflash.py
 SGTPy/equilibrium/stability.py
 SGTPy/fit/__init__.py
 SGTPy/fit/fit_beta.py
 SGTPy/fit/fit_cii.py
 SGTPy/fit/fitbinary.py
 SGTPy/fit/fitmulticomponent.py
@@ -78,11 +78,11 @@
 SGTPy/sgt/__init__.py
 SGTPy/sgt/coloc_z.py
 SGTPy/sgt/coloc_z_ds.py
 SGTPy/sgt/linear_spot.py
 SGTPy/sgt/path_sk.py
 SGTPy/sgt/reference_component.py
 SGTPy/sgt/sgt_beta0.py
-SGTPy/sgt/sgtpuros.py
+SGTPy/sgt/sgtpure.py
 SGTPy/sgt/tensionresult.py
 SGTPy/src/cijmix_cy.pyx
 SGTPy/src/coloc_cy.pyx
```

### Comparing `SGTPy-0.0.8/setup.py` & `SGTPy-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                           ['SGTPy/src/cijmix_cy.pyx'])]
 cmdclass.update({'build_ext': build_ext})
 """
 
 setup(
   name='SGTPy',
   license='MIT',
-  version='0.0.8',
+  version='0.0.9',
   description='SAFT-VR-MIE EOS and SGT',
   author='Gustavo Chaparro Maldonado, Andres Mejia Matallana, Erich A. Muller',
   author_email='gustavochaparro@udec.cl',
   url='https://github.com/gustavochm/SGTPy',
   download_url='https://github.com/gustavochm/SGTPy.git',
   long_description=open('long_description.rst').read(),
   packages=['SGTPy', 'SGTPy.mixtures',  'SGTPy.pure',   'SGTPy.sgt',
```

