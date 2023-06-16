# Comparing `tmp/pyrfu-2.4.1.tar.gz` & `tmp/pyrfu-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrfu-2.4.1.tar", last modified: Sat Jun 10 20:06:20 2023, max compression
+gzip compressed data, was "pyrfu-2.4.3.tar", last modified: Fri Jun 16 10:56:01 2023, max compression
```

## Comparing `pyrfu-2.4.1.tar` & `pyrfu-2.4.3.tar`

### file list

```diff
@@ -1,348 +1,348 @@
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:20.189452 pyrfu-2.4.1/
--rw-r--r--   0 louisr     (501) staff       (20)       69 2023-04-21 10:39:09.000000 pyrfu-2.4.1/.flake8
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:18.952866 pyrfu-2.4.1/.github/
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.801874 pyrfu-2.4.1/.github/workflows/
--rw-r--r--   0 louisr     (501) staff       (20)      570 2023-04-20 14:38:38.000000 pyrfu-2.4.1/.github/workflows/flake8.yml
--rw-r--r--   0 louisr     (501) staff       (20)      823 2023-05-14 19:49:15.000000 pyrfu-2.4.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 louisr     (501) staff       (20)      588 2023-06-09 14:46:12.000000 pyrfu-2.4.1/.github/workflows/pylint.yml
--rw-r--r--   0 louisr     (501) staff       (20)      289 2023-06-09 14:44:34.000000 pyrfu-2.4.1/.gitignore
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.809442 pyrfu-2.4.1/.idea/
--rw-r--r--   0 louisr     (501) staff       (20)      294 2023-06-09 19:35:51.000000 pyrfu-2.4.1/.idea/aws.xml
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.812557 pyrfu-2.4.1/.idea/codeStyles/
--rw-r--r--   0 louisr     (501) staff       (20)      153 2023-04-20 14:38:38.000000 pyrfu-2.4.1/.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.816298 pyrfu-2.4.1/.idea/inspectionProfiles/
--rw-r--r--   0 louisr     (501) staff       (20)      803 2023-04-20 14:38:38.000000 pyrfu-2.4.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 louisr     (501) staff       (20)      174 2023-04-20 14:38:38.000000 pyrfu-2.4.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 louisr     (501) staff       (20)      185 2023-04-20 14:38:38.000000 pyrfu-2.4.1/.idea/vcs (LAPTOP-E2ISLACJ's conflicted copy 2022-09-29).xml
--rw-r--r--   0 louisr     (501) staff       (20)      185 2023-04-20 14:38:38.000000 pyrfu-2.4.1/.idea/vcs.xml
--rw-r--r--   0 louisr     (501) staff       (20)    17383 2023-04-20 14:38:38.000000 pyrfu-2.4.1/.idea/workspace (LAPTOP-E2ISLACJ's conflicted copy 2022-10-01).xml
--rw-r--r--   0 louisr     (501) staff       (20)     1499 2023-06-09 14:43:25.000000 pyrfu-2.4.1/.pre-commit-config.yaml
--rwxr-xr-x   0 louisr     (501) staff       (20)       83 2023-04-20 14:38:38.000000 pyrfu-2.4.1/.readthedocs.yml
--rw-r--r--   0 louisr     (501) staff       (20)     2972 2023-04-20 14:38:38.000000 pyrfu-2.4.1/CONTRIBUTING.rst
--rw-r--r--   0 louisr     (501) staff       (20)     1067 2023-04-20 14:38:38.000000 pyrfu-2.4.1/LICENSE.txt
--rw-r--r--   0 louisr     (501) staff       (20)      438 2023-04-20 14:38:38.000000 pyrfu-2.4.1/MANIFEST.in
--rw-r--r--   0 louisr     (501) staff       (20)     8862 2023-06-10 20:06:20.188637 pyrfu-2.4.1/PKG-INFO
--rw-r--r--   0 louisr     (501) staff       (20)     6490 2023-06-09 10:13:58.000000 pyrfu-2.4.1/README.rst
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.821843 pyrfu-2.4.1/docs/
--rw-r--r--   0 louisr     (501) staff       (20)      640 2023-04-20 14:38:38.000000 pyrfu-2.4.1/docs/Makefile
--rw-r--r--   0 louisr     (501) staff       (20)      341 2023-04-21 12:45:20.000000 pyrfu-2.4.1/docs/environment.yml
--rw-r--r--   0 louisr     (501) staff       (20)      785 2023-04-20 14:38:38.000000 pyrfu-2.4.1/docs/make.bat
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.855506 pyrfu-2.4.1/docs/source/
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.857951 pyrfu-2.4.1/docs/source/_static/
--rw-r--r--   0 louisr     (501) staff       (20)    18615 2023-04-20 14:38:38.000000 pyrfu-2.4.1/docs/source/_static/logo-pyrfu.png
--rw-r--r--   0 louisr     (501) staff       (20)     2011 2023-04-20 14:38:38.000000 pyrfu-2.4.1/docs/source/_static/logo-pyrfu.svg
--rw-r--r--   0 louisr     (501) staff       (20)     8992 2023-06-09 14:50:39.000000 pyrfu-2.4.1/docs/source/conf.py
--rw-r--r--   0 louisr     (501) staff       (20)      372 2023-04-20 14:38:38.000000 pyrfu-2.4.1/docs/source/contributing.rst
--rw-r--r--   0 louisr     (501) staff       (20)     1044 2023-06-09 09:58:31.000000 pyrfu-2.4.1/docs/source/examples.rst
--rw-r--r--   0 louisr     (501) staff       (20)      192 2023-04-20 14:38:38.000000 pyrfu-2.4.1/docs/source/getting_started.rst
--rw-r--r--   0 louisr     (501) staff       (20)      618 2023-04-21 13:33:36.000000 pyrfu-2.4.1/docs/source/index.rst
--rw-r--r--   0 louisr     (501) staff       (20)       72 2023-04-20 14:38:38.000000 pyrfu-2.4.1/docs/source/modules.rst
--rw-r--r--   0 louisr     (501) staff       (20)     1283 2023-04-20 14:38:38.000000 pyrfu-2.4.1/docs/source/quick-overview.rst
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:18.955589 pyrfu-2.4.1/examples/
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.859208 pyrfu-2.4.1/examples/00_overview/
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.864806 pyrfu-2.4.1/examples/00_overview/.ipynb_checkpoints/
--rw-r--r--   0 louisr     (501) staff       (20)   520481 2023-06-09 11:41:54.000000 pyrfu-2.4.1/examples/00_overview/.ipynb_checkpoints/quick-overview-checkpoint.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   520481 2023-06-09 11:41:54.000000 pyrfu-2.4.1/examples/00_overview/quick-overview.ipynb
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.936951 pyrfu-2.4.1/examples/01_mms/
--rw-r--r--   0 louisr     (501) staff       (20)   281483 2023-06-08 15:46:40.000000 pyrfu-2.4.1/examples/01_mms/example_mms_b_e_j.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   564517 2023-06-09 09:46:23.000000 pyrfu-2.4.1/examples/01_mms/example_mms_ebfields.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   371521 2023-06-08 15:46:40.000000 pyrfu-2.4.1/examples/01_mms/example_mms_edr_signatures.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   411079 2023-06-08 15:46:40.000000 pyrfu-2.4.1/examples/01_mms/example_mms_eis.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   108423 2023-06-08 16:35:41.000000 pyrfu-2.4.1/examples/01_mms/example_mms_electron_psd.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   432503 2023-06-09 14:51:47.000000 pyrfu-2.4.1/examples/01_mms/example_mms_feeps.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   184196 2023-06-08 15:51:52.000000 pyrfu-2.4.1/examples/01_mms/example_mms_hpca.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   279733 2023-06-08 16:35:41.000000 pyrfu-2.4.1/examples/01_mms/example_mms_ohmslaw.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   353737 2023-06-08 16:40:22.000000 pyrfu-2.4.1/examples/01_mms/example_mms_particle_deflux.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   450116 2023-06-09 09:46:14.000000 pyrfu-2.4.1/examples/01_mms/example_mms_particle_distributions.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   634316 2023-06-09 09:42:51.000000 pyrfu-2.4.1/examples/01_mms/example_mms_particle_pad.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   445067 2023-06-08 15:50:47.000000 pyrfu-2.4.1/examples/01_mms/example_mms_polarizationanalysis.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   242849 2023-06-09 07:50:56.000000 pyrfu-2.4.1/examples/01_mms/example_mms_reduced_electron_dist.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   424890 2023-06-09 09:16:19.000000 pyrfu-2.4.1/examples/01_mms/example_mms_reduced_ion_dist.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)   205591 2023-06-09 11:46:23.000000 pyrfu-2.4.1/examples/01_mms/example_mms_walen_test.ipynb
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:20.004226 pyrfu-2.4.1/examples/02_dispersion/
--rw-r--r--   0 louisr     (501) staff       (20)    51819 2023-06-09 11:47:26.000000 pyrfu-2.4.1/examples/02_dispersion/example_dispersion_one_fluid.ipynb
--rw-r--r--   0 louisr     (501) staff       (20)     3050 2023-06-10 20:05:29.000000 pyrfu-2.4.1/pyproject.toml
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:18.966591 pyrfu-2.4.1/pyrfu/
--rw-r--r--   0 louisr     (501) staff       (20)      334 2023-06-10 20:05:29.000000 pyrfu-2.4.1/pyrfu/__init__.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:20.034939 pyrfu-2.4.1/pyrfu/__pycache__/
--rw-r--r--   0 louisr     (501) staff       (20)      521 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:18.968998 pyrfu-2.4.1/pyrfu/dispersion/
--rw-r--r--   0 louisr     (501) staff       (20)      381 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/dispersion/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)    10002 2023-04-21 10:37:39.000000 pyrfu-2.4.1/pyrfu/dispersion/disp_surf_calc.py
--rw-r--r--   0 louisr     (501) staff       (20)     3488 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/dispersion/one_fluid_dispersion.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:18.973018 pyrfu-2.4.1/pyrfu/lp/
--rw-r--r--   0 louisr     (501) staff       (20)     5325 2023-05-15 11:18:18.000000 pyrfu-2.4.1/pyrfu/lp/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)     3604 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/lp/photo_current.py
--rw-r--r--   0 louisr     (501) staff       (20)     3295 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/lp/thermal_current.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:20.091387 pyrfu-2.4.1/pyrfu/mms/
--rw-r--r--   0 louisr     (501) staff       (20)     6238 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)      726 2023-05-15 20:42:04.000000 pyrfu-2.4.1/pyrfu/mms/ancillary.json
--rw-r--r--   0 louisr     (501) staff       (20)     4954 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/calculate_epsilon.py
--rw-r--r--   0 louisr     (501) staff       (20)       35 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/config.json
--rw-r--r--   0 louisr     (501) staff       (20)     2281 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/copy_files.py
--rw-r--r--   0 louisr     (501) staff       (20)     2196 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/copy_files_ancillary.py
--rw-r--r--   0 louisr     (501) staff       (20)     2914 2023-05-15 20:29:49.000000 pyrfu-2.4.1/pyrfu/mms/correct_edp_probe_timing.py
--rw-r--r--   0 louisr     (501) staff       (20)     1759 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/db_get_ts.py
--rw-r--r--   0 louisr     (501) staff       (20)     1574 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/db_get_variable.py
--rw-r--r--   0 louisr     (501) staff       (20)     1094 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/db_init.py
--rw-r--r--   0 louisr     (501) staff       (20)     2658 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/def2psd.py
--rw-r--r--   0 louisr     (501) staff       (20)     1701 2023-04-21 08:58:14.000000 pyrfu-2.4.1/pyrfu/mms/dft_time_shift.py
--rw-r--r--   0 louisr     (501) staff       (20)     5504 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/download_ancillary.py
--rw-r--r--   0 louisr     (501) staff       (20)     7729 2023-06-10 20:03:44.000000 pyrfu-2.4.1/pyrfu/mms/download_data.py
--rw-r--r--   0 louisr     (501) staff       (20)     2533 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/dpf2psd.py
--rw-r--r--   0 louisr     (501) staff       (20)     3291 2023-04-21 09:02:25.000000 pyrfu-2.4.1/pyrfu/mms/dsl2gse.py
--rw-r--r--   0 louisr     (501) staff       (20)     3158 2023-04-21 09:02:47.000000 pyrfu-2.4.1/pyrfu/mms/dsl2gsm.py
--rw-r--r--   0 louisr     (501) staff       (20)     6423 2023-05-15 11:04:37.000000 pyrfu-2.4.1/pyrfu/mms/eis_ang_ang.py
--rw-r--r--   0 louisr     (501) staff       (20)     5431 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/eis_combine_proton_pad.py
--rw-r--r--   0 louisr     (501) staff       (20)     1502 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/eis_combine_proton_skymap.py
--rw-r--r--   0 louisr     (501) staff       (20)    10923 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/eis_combine_proton_spec.py
--rw-r--r--   0 louisr     (501) staff       (20)     4645 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/eis_moments.py
--rw-r--r--   0 louisr     (501) staff       (20)     1782 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/eis_omni.py
--rw-r--r--   0 louisr     (501) staff       (20)     3768 2023-04-21 20:23:25.000000 pyrfu-2.4.1/pyrfu/mms/eis_pad.py
--rw-r--r--   0 louisr     (501) staff       (20)     1996 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/eis_pad_combine_sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     1486 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/eis_pad_spinavg.py
--rw-r--r--   0 louisr     (501) staff       (20)     3297 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/eis_proton_correction.py
--rw-r--r--   0 louisr     (501) staff       (20)     2154 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/eis_skymap.py
--rw-r--r--   0 louisr     (501) staff       (20)     4747 2023-05-14 17:25:56.000000 pyrfu-2.4.1/pyrfu/mms/eis_skymap_combine_sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     3515 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/eis_spec_combine_sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     3390 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/eis_spin_avg.py
--rw-r--r--   0 louisr     (501) staff       (20)     2983 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/estimate_phase_speed.py
--rw-r--r--   0 louisr     (501) staff       (20)     4386 2023-05-15 20:31:04.000000 pyrfu-2.4.1/pyrfu/mms/feeps_active_eyes.py
--rw-r--r--   0 louisr     (501) staff       (20)     3968 2023-05-15 20:42:14.000000 pyrfu-2.4.1/pyrfu/mms/feeps_bad_data.json
--rw-r--r--   0 louisr     (501) staff       (20)     1757 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/feeps_correct_energies.py
--rw-r--r--   0 louisr     (501) staff       (20)     3354 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/feeps_energy_table.py
--rw-r--r--   0 louisr     (501) staff       (20)     1991 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/feeps_flat_field_corrections.py
--rw-r--r--   0 louisr     (501) staff       (20)     2982 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/feeps_omni.py
--rw-r--r--   0 louisr     (501) staff       (20)     6204 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/feeps_pad.py
--rw-r--r--   0 louisr     (501) staff       (20)     2520 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/feeps_pad_spinavg.py
--rw-r--r--   0 louisr     (501) staff       (20)     4567 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/feeps_pitch_angles.py
--rw-r--r--   0 louisr     (501) staff       (20)     5604 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/feeps_remove_bad_data.py
--rw-r--r--   0 louisr     (501) staff       (20)     2003 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/feeps_remove_sun.py
--rw-r--r--   0 louisr     (501) staff       (20)     1810 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/feeps_sector_spec.py
--rw-r--r--   0 louisr     (501) staff       (20)     1435 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/feeps_spin_avg.py
--rw-r--r--   0 louisr     (501) staff       (20)     1292 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/feeps_split_integral_ch.py
--rw-r--r--   0 louisr     (501) staff       (20)     2797 2023-04-21 10:10:19.000000 pyrfu-2.4.1/pyrfu/mms/fft_bandpass.py
--rw-r--r--   0 louisr     (501) staff       (20)    12130 2023-05-16 12:07:24.000000 pyrfu-2.4.1/pyrfu/mms/fk_power_spectrum_4sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     3062 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/get_data.py
--rw-r--r--   0 louisr     (501) staff       (20)     9383 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/get_dist.py
--rw-r--r--   0 louisr     (501) staff       (20)     4902 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/get_eis_allt.py
--rw-r--r--   0 louisr     (501) staff       (20)     4690 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/get_feeps_alleyes.py
--rw-r--r--   0 louisr     (501) staff       (20)     2525 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/get_feeps_omni.py
--rw-r--r--   0 louisr     (501) staff       (20)     6173 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/get_hpca_dist.py
--rw-r--r--   0 louisr     (501) staff       (20)     7052 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/get_pitch_angle_dist.py
--rw-r--r--   0 louisr     (501) staff       (20)    11547 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/get_ts.py
--rw-r--r--   0 louisr     (501) staff       (20)      926 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/get_variable.py
--rw-r--r--   0 louisr     (501) staff       (20)     1771 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/hpca_calc_anodes.py
--rw-r--r--   0 louisr     (501) staff       (20)     1395 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/hpca_energies.py
--rw-r--r--   0 louisr     (501) staff       (20)     5854 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/hpca_pad.py
--rw-r--r--   0 louisr     (501) staff       (20)     1621 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/hpca_spin_sum.py
--rw-r--r--   0 louisr     (501) staff       (20)     5642 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/lh_wave_analysis.py
--rw-r--r--   0 louisr     (501) staff       (20)     6790 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/list_files.py
--rw-r--r--   0 louisr     (501) staff       (20)     4366 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/list_files_ancillary.py
--rw-r--r--   0 louisr     (501) staff       (20)     2882 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/load_ancillary.py
--rw-r--r--   0 louisr     (501) staff       (20)     2861 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/load_brst_segments.py
--rw-r--r--   0 louisr     (501) staff       (20)     4016 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/make_model_kappa.py
--rw-r--r--   0 louisr     (501) staff       (20)     7023 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/make_model_rq.py
--rw-r--r--   0 louisr     (501) staff       (20)     7030 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/make_model_vdf.py
--rw-r--r--   0 louisr     (501) staff       (20)    25074 2023-05-15 20:42:21.000000 pyrfu-2.4.1/pyrfu/mms/mms_keys.json
--rw-r--r--   0 louisr     (501) staff       (20)     6101 2023-04-21 10:35:28.000000 pyrfu-2.4.1/pyrfu/mms/probe_align_times.py
--rw-r--r--   0 louisr     (501) staff       (20)     2782 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/psd2def.py
--rw-r--r--   0 louisr     (501) staff       (20)     2796 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/psd2dpf.py
--rw-r--r--   0 louisr     (501) staff       (20)    18467 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/psd_moments.py
--rw-r--r--   0 louisr     (501) staff       (20)     3307 2023-04-21 09:53:59.000000 pyrfu-2.4.1/pyrfu/mms/psd_rebin.py
--rw-r--r--   0 louisr     (501) staff       (20)     2610 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/read_feeps_sector_masks_csv.py
--rw-r--r--   0 louisr     (501) staff       (20)     9191 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/reduce.py
--rw-r--r--   0 louisr     (501) staff       (20)     5568 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/remove_edist_background.py
--rw-r--r--   0 louisr     (501) staff       (20)     2099 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/remove_idist_background.py
--rw-r--r--   0 louisr     (501) staff       (20)     3224 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/remove_imoms_background.py
--rw-r--r--   0 louisr     (501) staff       (20)     7295 2023-04-21 10:35:32.000000 pyrfu-2.4.1/pyrfu/mms/rotate_tensor.py
--rw-r--r--   0 louisr     (501) staff       (20)     4320 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/scpot2ne.py
--rw-r--r--   0 louisr     (501) staff       (20)      945 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/spectr_to_dataset.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:20.163973 pyrfu-2.4.1/pyrfu/mms/sun/
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20151111.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20160709.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20161028.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20170531.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20171003.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20181005.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20151111.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20160709.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20161028.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20170531.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20171003.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20181005.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20151111.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20160709.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20161028.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3134 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20170531.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20171003.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20181005.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20151111.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20160709.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20161028.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20170531.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20171003.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20181005.csv
--rw-r--r--   0 louisr     (501) staff       (20)     3854 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/tokenize.py
--rw-r--r--   0 louisr     (501) staff       (20)     3363 2023-06-09 09:40:21.000000 pyrfu-2.4.1/pyrfu/mms/vdf_elim.py
--rw-r--r--   0 louisr     (501) staff       (20)     1946 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/mms/vdf_omni.py
--rw-r--r--   0 louisr     (501) staff       (20)    11804 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/vdf_projection.py
--rw-r--r--   0 louisr     (501) staff       (20)     8578 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/vdf_reduce.py
--rw-r--r--   0 louisr     (501) staff       (20)     2488 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/vdf_to_e64.py
--rw-r--r--   0 louisr     (501) staff       (20)     2337 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/mms/whistler_b2e.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:20.165571 pyrfu-2.4.1/pyrfu/models/
--rw-r--r--   0 louisr     (501) staff       (20)      689 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/models/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)     2741 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/models/igrf.py
--rw-r--r--   0 louisr     (501) staff       (20)    26798 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/models/igrf13coeffs.csv
--rw-r--r--   0 louisr     (501) staff       (20)     6278 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/models/magnetopause_normal.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.429523 pyrfu-2.4.1/pyrfu/plot/
--rw-r--r--   0 louisr     (501) staff       (20)     1645 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)     1725 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/add_position.py
--rw-r--r--   0 louisr     (501) staff       (20)     2366 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/annotate_heatmap.py
--rw-r--r--   0 louisr     (501) staff       (20)      935 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/plot/colorbar.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:20.170127 pyrfu-2.4.1/pyrfu/plot/logo/
--rw-r--r--   0 louisr     (501) staff       (20)    43962 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/plot/logo/IRF_logo_blue_on_white.jpg
--rw-r--r--   0 louisr     (501) staff       (20)     1160 2023-05-16 12:44:48.000000 pyrfu-2.4.1/pyrfu/plot/make_labels.py
--rw-r--r--   0 louisr     (501) staff       (20)     3808 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/mms_pl_config.py
--rw-r--r--   0 louisr     (501) staff       (20)     2856 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/pl_scatter_matrix.py
--rw-r--r--   0 louisr     (501) staff       (20)     1539 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/pl_tx.py
--rw-r--r--   0 louisr     (501) staff       (20)     3832 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/plot_ang_ang.py
--rw-r--r--   0 louisr     (501) staff       (20)     1764 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/plot_clines.py
--rw-r--r--   0 louisr     (501) staff       (20)     2446 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/plot_heatmap.py
--rw-r--r--   0 louisr     (501) staff       (20)     1495 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/plot_line.py
--rw-r--r--   0 louisr     (501) staff       (20)     3809 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/plot_magnetosphere.py
--rw-r--r--   0 louisr     (501) staff       (20)     2212 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/plot_projection.py
--rw-r--r--   0 louisr     (501) staff       (20)     1946 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/plot_reduced_2d.py
--rw-r--r--   0 louisr     (501) staff       (20)    11634 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/plot_sitl_overview.py
--rw-r--r--   0 louisr     (501) staff       (20)     4628 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/plot_spectr.py
--rw-r--r--   0 louisr     (501) staff       (20)     2423 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/plot_surf.py
--rw-r--r--   0 louisr     (501) staff       (20)     1511 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/plot/span_tint.py
--rw-r--r--   0 louisr     (501) staff       (20)     2455 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/plot/zoom.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:20.183483 pyrfu-2.4.1/pyrfu/pyrf/
--rw-r--r--   0 louisr     (501) staff       (20)     5735 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)     1964 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/autocorr.py
--rw-r--r--   0 louisr     (501) staff       (20)     2743 2023-04-21 10:37:39.000000 pyrfu-2.4.1/pyrfu/pyrf/average_vdf.py
--rw-r--r--   0 louisr     (501) staff       (20)     1156 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/avg_4sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     5023 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/c_4_grad.py
--rw-r--r--   0 louisr     (501) staff       (20)     4189 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/c_4_j.py
--rw-r--r--   0 louisr     (501) staff       (20)     1315 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/c_4_k.py
--rw-r--r--   0 louisr     (501) staff       (20)     2633 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/c_4_v.py
--rw-r--r--   0 louisr     (501) staff       (20)     2080 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/calc_ag.py
--rw-r--r--   0 louisr     (501) staff       (20)     1422 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/calc_agyro.py
--rw-r--r--   0 louisr     (501) staff       (20)     1850 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/calc_dng.py
--rw-r--r--   0 louisr     (501) staff       (20)      623 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/calc_dt.py
--rw-r--r--   0 louisr     (501) staff       (20)      646 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/calc_fs.py
--rw-r--r--   0 louisr     (501) staff       (20)     1809 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/calc_sqrtq.py
--rw-r--r--   0 louisr     (501) staff       (20)     1223 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/cart2sph.py
--rw-r--r--   0 louisr     (501) staff       (20)     1997 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/cart2sph_ts.py
--rw-r--r--   0 louisr     (501) staff       (20)     1654 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/cdfepoch2datetime64.py
--rw-r--r--   0 louisr     (501) staff       (20)     1582 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/compress_cwt.py
--rw-r--r--   0 louisr     (501) staff       (20)     3430 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/convert_fac.py
--rw-r--r--   0 louisr     (501) staff       (20)     6686 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/corr_deriv.py
--rw-r--r--   0 louisr     (501) staff       (20)    10734 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/cotrans.py
--rw-r--r--   0 louisr     (501) staff       (20)     1430 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/cross.py
--rw-r--r--   0 louisr     (501) staff       (20)     1486 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/date_str.py
--rw-r--r--   0 louisr     (501) staff       (20)      821 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/datetime2iso8601.py
--rw-r--r--   0 louisr     (501) staff       (20)      842 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/datetime642iso8601.py
--rw-r--r--   0 louisr     (501) staff       (20)      870 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/datetime642ttns.py
--rw-r--r--   0 louisr     (501) staff       (20)      694 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/datetime642unix.py
--rw-r--r--   0 louisr     (501) staff       (20)     2570 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/dec_par_perp.py
--rw-r--r--   0 louisr     (501) staff       (20)     2992 2023-05-09 14:12:30.000000 pyrfu-2.4.1/pyrfu/pyrf/dist_append.py
--rw-r--r--   0 louisr     (501) staff       (20)     1715 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/dot.py
--rw-r--r--   0 louisr     (501) staff       (20)     1594 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/dynamic_press.py
--rw-r--r--   0 louisr     (501) staff       (20)     2283 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/e_vxb.py
--rw-r--r--   0 louisr     (501) staff       (20)     1910 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/eb_nrf.py
--rw-r--r--   0 louisr     (501) staff       (20)    37491 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/ebsp.py
--rw-r--r--   0 louisr     (501) staff       (20)     3678 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/edb.py
--rw-r--r--   0 louisr     (501) staff       (20)      625 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/end.py
--rw-r--r--   0 louisr     (501) staff       (20)     3113 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/estimate.py
--rw-r--r--   0 louisr     (501) staff       (20)     1880 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/extend_tint.py
--rw-r--r--   0 louisr     (501) staff       (20)     3882 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/filt.py
--rw-r--r--   0 louisr     (501) staff       (20)     1971 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/find_closest.py
--rw-r--r--   0 louisr     (501) staff       (20)     3978 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/get_omni_data.py
--rw-r--r--   0 louisr     (501) staff       (20)     1298 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/gradient.py
--rw-r--r--   0 louisr     (501) staff       (20)      987 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/gse2gsm.py
--rw-r--r--   0 louisr     (501) staff       (20)     2402 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/histogram.py
--rw-r--r--   0 louisr     (501) staff       (20)     3160 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/histogram2d.py
--rw-r--r--   0 louisr     (501) staff       (20)     1684 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/increments.py
--rw-r--r--   0 louisr     (501) staff       (20)    18801 2023-06-10 20:04:38.000000 pyrfu-2.4.1/pyrfu/pyrf/int_sph_dist.py
--rw-r--r--   0 louisr     (501) staff       (20)     2106 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/integrate.py
--rw-r--r--   0 louisr     (501) staff       (20)     6075 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/iplasma_calc.py
--rw-r--r--   0 louisr     (501) staff       (20)      585 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/iso2unix.py
--rw-r--r--   0 louisr     (501) staff       (20)      875 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/iso86012datetime.py
--rw-r--r--   0 louisr     (501) staff       (20)      626 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/iso86012datetime64.py
--rw-r--r--   0 louisr     (501) staff       (20)     1060 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/iso86012timevec.py
--rw-r--r--   0 louisr     (501) staff       (20)      999 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/l_shell.py
--rw-r--r--   0 louisr     (501) staff       (20)     1281 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/lowpass.py
--rw-r--r--   0 louisr     (501) staff       (20)     2438 2023-04-21 10:37:39.000000 pyrfu-2.4.1/pyrfu/pyrf/magnetosphere.py
--rw-r--r--   0 louisr     (501) staff       (20)     4500 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/match_phibe_dir.py
--rw-r--r--   0 louisr     (501) staff       (20)     1794 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/match_phibe_v.py
--rw-r--r--   0 louisr     (501) staff       (20)     2154 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/mean.py
--rw-r--r--   0 louisr     (501) staff       (20)     2391 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/mean_bins.py
--rw-r--r--   0 louisr     (501) staff       (20)     1220 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/mean_field.py
--rw-r--r--   0 louisr     (501) staff       (20)     2336 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/medfilt.py
--rw-r--r--   0 louisr     (501) staff       (20)     2362 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/median_bins.py
--rw-r--r--   0 louisr     (501) staff       (20)     1836 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/movmean.py
--rw-r--r--   0 louisr     (501) staff       (20)     4827 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/mva.py
--rw-r--r--   0 louisr     (501) staff       (20)     1473 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/new_xyz.py
--rw-r--r--   0 louisr     (501) staff       (20)      957 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/norm.py
--rw-r--r--   0 louisr     (501) staff       (20)      957 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/normalize.py
--rw-r--r--   0 louisr     (501) staff       (20)     2046 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/optimize_nbins_1d.py
--rw-r--r--   0 louisr     (501) staff       (20)     2746 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/optimize_nbins_2d.py
--rw-r--r--   0 louisr     (501) staff       (20)     3719 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/pid_4sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     1219 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/plasma_beta.py
--rw-r--r--   0 louisr     (501) staff       (20)     7424 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/plasma_calc.py
--rw-r--r--   0 louisr     (501) staff       (20)     2766 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/poynting_flux.py
--rw-r--r--   0 louisr     (501) staff       (20)     1897 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/pres_anis.py
--rw-r--r--   0 louisr     (501) staff       (20)     3060 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/psd.py
--rw-r--r--   0 louisr     (501) staff       (20)     1293 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/pvi.py
--rw-r--r--   0 louisr     (501) staff       (20)     2494 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/pvi_4sc.py
--rw-r--r--   0 louisr     (501) staff       (20)     1277 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/read_cdf.py
--rw-r--r--   0 louisr     (501) staff       (20)     2094 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/remove_repeated_points.py
--rw-r--r--   0 louisr     (501) staff       (20)     9204 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/resample.py
--rw-r--r--   0 louisr     (501) staff       (20)      697 2023-06-07 15:24:32.000000 pyrfu-2.4.1/pyrfu/pyrf/shock_models_parameters.json
--rw-r--r--   0 louisr     (501) staff       (20)    15260 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/shock_normal.py
--rw-r--r--   0 louisr     (501) staff       (20)     9265 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/shock_parameters.py
--rw-r--r--   0 louisr     (501) staff       (20)     1646 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/solid_angle.py
--rw-r--r--   0 louisr     (501) staff       (20)      905 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/sph2cart.py
--rw-r--r--   0 louisr     (501) staff       (20)     2961 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/st_diff.py
--rw-r--r--   0 louisr     (501) staff       (20)      600 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/start.py
--rw-r--r--   0 louisr     (501) staff       (20)     1936 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/struct_func.py
--rw-r--r--   0 louisr     (501) staff       (20)     1146 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/t_eval.py
--rw-r--r--   0 louisr     (501) staff       (20)     3837 2023-04-21 10:37:39.000000 pyrfu-2.4.1/pyrfu/pyrf/time_clip.py
--rw-r--r--   0 louisr     (501) staff       (20)     1212 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/timevec2iso8601.py
--rw-r--r--   0 louisr     (501) staff       (20)     1501 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/trace.py
--rw-r--r--   0 louisr     (501) staff       (20)      688 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/transformation_indices.json
--rw-r--r--   0 louisr     (501) staff       (20)     2422 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/ts_append.py
--rw-r--r--   0 louisr     (501) staff       (20)      956 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/ts_scalar.py
--rw-r--r--   0 louisr     (501) staff       (20)     3150 2023-05-09 14:12:22.000000 pyrfu-2.4.1/pyrfu/pyrf/ts_skymap.py
--rw-r--r--   0 louisr     (501) staff       (20)     1060 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/ts_tensor_xyz.py
--rw-r--r--   0 louisr     (501) staff       (20)      672 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/ts_time.py
--rw-r--r--   0 louisr     (501) staff       (20)     1022 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/ts_vec_xyz.py
--rw-r--r--   0 louisr     (501) staff       (20)      928 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/ttns2datetime64.py
--rw-r--r--   0 louisr     (501) staff       (20)      718 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/unix2datetime64.py
--rw-r--r--   0 louisr     (501) staff       (20)     3658 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/vht.py
--rw-r--r--   0 louisr     (501) staff       (20)     1749 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/wave_fft.py
--rw-r--r--   0 louisr     (501) staff       (20)     6512 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/wavelet.py
--rw-r--r--   0 louisr     (501) staff       (20)    14548 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/pyrf/wavepolarize_means.py
--rw-r--r--   0 louisr     (501) staff       (20)     2375 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/pyrf/waverage.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:20.186141 pyrfu-2.4.1/pyrfu/solo/
--rw-r--r--   0 louisr     (501) staff       (20)      384 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/solo/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)       48 2023-04-20 14:38:39.000000 pyrfu-2.4.1/pyrfu/solo/config.json
--rw-r--r--   0 louisr     (501) staff       (20)     1148 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/solo/db_init.py
--rw-r--r--   0 louisr     (501) staff       (20)     4781 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/solo/read_lfr_density.py
--rw-r--r--   0 louisr     (501) staff       (20)     8500 2023-06-09 14:49:17.000000 pyrfu-2.4.1/pyrfu/solo/read_tnr.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.794898 pyrfu-2.4.1/pyrfu/tests/
--rw-r--r--   0 louisr     (501) staff       (20)      206 2023-04-21 10:37:39.000000 pyrfu-2.4.1/pyrfu/tests/__init__.py
--rw-r--r--   0 louisr     (501) staff       (20)     1553 2023-04-21 10:37:39.000000 pyrfu-2.4.1/pyrfu/tests/test_pyrf.py
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:20.033744 pyrfu-2.4.1/pyrfu.egg-info/
--rw-r--r--   0 louisr     (501) staff       (20)     8862 2023-06-10 20:06:18.000000 pyrfu-2.4.1/pyrfu.egg-info/PKG-INFO
--rw-r--r--   0 louisr     (501) staff       (20)    16027 2023-06-10 20:06:18.000000 pyrfu-2.4.1/pyrfu.egg-info/SOURCES.txt
--rw-r--r--   0 louisr     (501) staff       (20)        1 2023-06-10 20:06:18.000000 pyrfu-2.4.1/pyrfu.egg-info/dependency_links.txt
--rw-r--r--   0 louisr     (501) staff       (20)      235 2023-06-10 20:06:18.000000 pyrfu-2.4.1/pyrfu.egg-info/requires.txt
--rw-r--r--   0 louisr     (501) staff       (20)       36 2023-06-10 20:06:18.000000 pyrfu-2.4.1/pyrfu.egg-info/top_level.txt
--rw-r--r--   0 louisr     (501) staff       (20)     2691 2023-06-09 14:45:06.000000 pyrfu-2.4.1/requirements.txt
--rw-r--r--   0 louisr     (501) staff       (20)       38 2023-06-10 20:06:20.189599 pyrfu-2.4.1/setup.cfg
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:18.952182 pyrfu-2.4.1/venv/
-drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-10 20:06:19.796417 pyrfu-2.4.1/venv/bin/
--rw-r--r--   0 louisr     (501) staff       (20)     1175 2023-06-09 14:34:14.000000 pyrfu-2.4.1/venv/bin/activate_this.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:01.228027 pyrfu-2.4.3/
+-rw-r--r--   0 louisr     (501) staff       (20)       69 2023-04-21 10:39:09.000000 pyrfu-2.4.3/.flake8
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.459838 pyrfu-2.4.3/.github/
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.507865 pyrfu-2.4.3/.github/workflows/
+-rw-r--r--   0 louisr     (501) staff       (20)      570 2023-04-20 14:38:38.000000 pyrfu-2.4.3/.github/workflows/flake8.yml
+-rw-r--r--   0 louisr     (501) staff       (20)      823 2023-05-14 19:49:15.000000 pyrfu-2.4.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 louisr     (501) staff       (20)      588 2023-06-09 14:46:12.000000 pyrfu-2.4.3/.github/workflows/pylint.yml
+-rw-r--r--   0 louisr     (501) staff       (20)      289 2023-06-09 14:44:34.000000 pyrfu-2.4.3/.gitignore
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.517289 pyrfu-2.4.3/.idea/
+-rw-r--r--   0 louisr     (501) staff       (20)      294 2023-06-14 09:44:52.000000 pyrfu-2.4.3/.idea/aws.xml
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.518921 pyrfu-2.4.3/.idea/codeStyles/
+-rw-r--r--   0 louisr     (501) staff       (20)      153 2023-04-20 14:38:38.000000 pyrfu-2.4.3/.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.521263 pyrfu-2.4.3/.idea/inspectionProfiles/
+-rw-r--r--   0 louisr     (501) staff       (20)      803 2023-04-20 14:38:38.000000 pyrfu-2.4.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 louisr     (501) staff       (20)      174 2023-04-20 14:38:38.000000 pyrfu-2.4.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 louisr     (501) staff       (20)      185 2023-04-20 14:38:38.000000 pyrfu-2.4.3/.idea/vcs (LAPTOP-E2ISLACJ's conflicted copy 2022-09-29).xml
+-rw-r--r--   0 louisr     (501) staff       (20)      185 2023-04-20 14:38:38.000000 pyrfu-2.4.3/.idea/vcs.xml
+-rw-r--r--   0 louisr     (501) staff       (20)    17383 2023-04-20 14:38:38.000000 pyrfu-2.4.3/.idea/workspace (LAPTOP-E2ISLACJ's conflicted copy 2022-10-01).xml
+-rw-r--r--   0 louisr     (501) staff       (20)     1499 2023-06-09 14:43:25.000000 pyrfu-2.4.3/.pre-commit-config.yaml
+-rwxr-xr-x   0 louisr     (501) staff       (20)       83 2023-04-20 14:38:38.000000 pyrfu-2.4.3/.readthedocs.yml
+-rw-r--r--   0 louisr     (501) staff       (20)     2972 2023-04-20 14:38:38.000000 pyrfu-2.4.3/CONTRIBUTING.rst
+-rw-r--r--   0 louisr     (501) staff       (20)     1067 2023-04-20 14:38:38.000000 pyrfu-2.4.3/LICENSE.txt
+-rw-r--r--   0 louisr     (501) staff       (20)      438 2023-04-20 14:38:38.000000 pyrfu-2.4.3/MANIFEST.in
+-rw-r--r--   0 louisr     (501) staff       (20)     8862 2023-06-16 10:56:01.227157 pyrfu-2.4.3/PKG-INFO
+-rw-r--r--   0 louisr     (501) staff       (20)     6490 2023-06-09 10:13:58.000000 pyrfu-2.4.3/README.rst
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.546892 pyrfu-2.4.3/docs/
+-rw-r--r--   0 louisr     (501) staff       (20)      640 2023-04-20 14:38:38.000000 pyrfu-2.4.3/docs/Makefile
+-rw-r--r--   0 louisr     (501) staff       (20)      341 2023-04-21 12:45:20.000000 pyrfu-2.4.3/docs/environment.yml
+-rw-r--r--   0 louisr     (501) staff       (20)      785 2023-04-20 14:38:38.000000 pyrfu-2.4.3/docs/make.bat
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.569847 pyrfu-2.4.3/docs/source/
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.572840 pyrfu-2.4.3/docs/source/_static/
+-rw-r--r--   0 louisr     (501) staff       (20)    18615 2023-04-20 14:38:38.000000 pyrfu-2.4.3/docs/source/_static/logo-pyrfu.png
+-rw-r--r--   0 louisr     (501) staff       (20)     2011 2023-04-20 14:38:38.000000 pyrfu-2.4.3/docs/source/_static/logo-pyrfu.svg
+-rw-r--r--   0 louisr     (501) staff       (20)     8992 2023-06-09 14:50:39.000000 pyrfu-2.4.3/docs/source/conf.py
+-rw-r--r--   0 louisr     (501) staff       (20)      372 2023-04-20 14:38:38.000000 pyrfu-2.4.3/docs/source/contributing.rst
+-rw-r--r--   0 louisr     (501) staff       (20)     1091 2023-06-14 09:19:39.000000 pyrfu-2.4.3/docs/source/examples.rst
+-rw-r--r--   0 louisr     (501) staff       (20)      192 2023-04-20 14:38:38.000000 pyrfu-2.4.3/docs/source/getting_started.rst
+-rw-r--r--   0 louisr     (501) staff       (20)      618 2023-04-21 13:33:36.000000 pyrfu-2.4.3/docs/source/index.rst
+-rw-r--r--   0 louisr     (501) staff       (20)       72 2023-04-20 14:38:38.000000 pyrfu-2.4.3/docs/source/modules.rst
+-rw-r--r--   0 louisr     (501) staff       (20)     1283 2023-04-20 14:38:38.000000 pyrfu-2.4.3/docs/source/quick-overview.rst
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.468931 pyrfu-2.4.3/examples/
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.574300 pyrfu-2.4.3/examples/00_overview/
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.586051 pyrfu-2.4.3/examples/00_overview/.ipynb_checkpoints/
+-rw-r--r--   0 louisr     (501) staff       (20)   520481 2023-06-09 11:41:54.000000 pyrfu-2.4.3/examples/00_overview/.ipynb_checkpoints/quick-overview-checkpoint.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   520481 2023-06-09 11:41:54.000000 pyrfu-2.4.3/examples/00_overview/quick-overview.ipynb
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.662376 pyrfu-2.4.3/examples/01_mms/
+-rw-r--r--   0 louisr     (501) staff       (20)   281483 2023-06-08 15:46:40.000000 pyrfu-2.4.3/examples/01_mms/example_mms_b_e_j.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   564517 2023-06-09 09:46:23.000000 pyrfu-2.4.3/examples/01_mms/example_mms_ebfields.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   371521 2023-06-08 15:46:40.000000 pyrfu-2.4.3/examples/01_mms/example_mms_edr_signatures.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   411079 2023-06-08 15:46:40.000000 pyrfu-2.4.3/examples/01_mms/example_mms_eis.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   108423 2023-06-08 16:35:41.000000 pyrfu-2.4.3/examples/01_mms/example_mms_electron_psd.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   432503 2023-06-09 14:51:47.000000 pyrfu-2.4.3/examples/01_mms/example_mms_feeps.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   184196 2023-06-08 15:51:52.000000 pyrfu-2.4.3/examples/01_mms/example_mms_hpca.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   279733 2023-06-08 16:35:41.000000 pyrfu-2.4.3/examples/01_mms/example_mms_ohmslaw.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   353737 2023-06-08 16:40:22.000000 pyrfu-2.4.3/examples/01_mms/example_mms_particle_deflux.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   450116 2023-06-09 09:46:14.000000 pyrfu-2.4.3/examples/01_mms/example_mms_particle_distributions.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   634316 2023-06-09 09:42:51.000000 pyrfu-2.4.3/examples/01_mms/example_mms_particle_pad.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   445067 2023-06-08 15:50:47.000000 pyrfu-2.4.3/examples/01_mms/example_mms_polarizationanalysis.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   242849 2023-06-09 07:50:56.000000 pyrfu-2.4.3/examples/01_mms/example_mms_reduced_electron_dist.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   424890 2023-06-09 09:16:19.000000 pyrfu-2.4.3/examples/01_mms/example_mms_reduced_ion_dist.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)   205591 2023-06-09 11:46:23.000000 pyrfu-2.4.3/examples/01_mms/example_mms_walen_test.ipynb
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.666315 pyrfu-2.4.3/examples/02_dispersion/
+-rw-r--r--   0 louisr     (501) staff       (20)    51819 2023-06-09 11:47:26.000000 pyrfu-2.4.3/examples/02_dispersion/example_dispersion_one_fluid.ipynb
+-rw-r--r--   0 louisr     (501) staff       (20)     3072 2023-06-16 10:53:10.000000 pyrfu-2.4.3/pyproject.toml
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.668295 pyrfu-2.4.3/pyrfu/
+-rw-r--r--   0 louisr     (501) staff       (20)      334 2023-06-16 10:53:10.000000 pyrfu-2.4.3/pyrfu/__init__.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.689255 pyrfu-2.4.3/pyrfu/__pycache__/
+-rw-r--r--   0 louisr     (501) staff       (20)      521 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.695429 pyrfu-2.4.3/pyrfu/dispersion/
+-rw-r--r--   0 louisr     (501) staff       (20)      381 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/dispersion/__init__.py
+-rw-r--r--   0 louisr     (501) staff       (20)    10001 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/dispersion/disp_surf_calc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3487 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/dispersion/one_fluid_dispersion.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.700442 pyrfu-2.4.3/pyrfu/lp/
+-rw-r--r--   0 louisr     (501) staff       (20)     5325 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/lp/__init__.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3604 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/lp/photo_current.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3295 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/lp/thermal_current.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.894309 pyrfu-2.4.3/pyrfu/mms/
+-rw-r--r--   0 louisr     (501) staff       (20)     6045 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/__init__.py
+-rw-r--r--   0 louisr     (501) staff       (20)      726 2023-05-15 20:42:04.000000 pyrfu-2.4.3/pyrfu/mms/ancillary.json
+-rw-r--r--   0 louisr     (501) staff       (20)     4954 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/calculate_epsilon.py
+-rw-r--r--   0 louisr     (501) staff       (20)       35 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/config.json
+-rw-r--r--   0 louisr     (501) staff       (20)     2280 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/copy_files.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2195 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/copy_files_ancillary.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2914 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/correct_edp_probe_timing.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1759 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/db_get_ts.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1574 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/db_get_variable.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1093 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/db_init.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2558 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/def2psd.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1631 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/dft_time_shift.py
+-rw-r--r--   0 louisr     (501) staff       (20)     5503 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/download_ancillary.py
+-rw-r--r--   0 louisr     (501) staff       (20)     7477 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/download_data.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2533 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/dpf2psd.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3166 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/dsl2gse.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3041 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/dsl2gsm.py
+-rw-r--r--   0 louisr     (501) staff       (20)     6423 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_ang_ang.py
+-rw-r--r--   0 louisr     (501) staff       (20)     5431 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_combine_proton_pad.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1502 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_combine_proton_skymap.py
+-rw-r--r--   0 louisr     (501) staff       (20)    10923 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_combine_proton_spec.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4645 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_moments.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1782 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_omni.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3768 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_pad.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1996 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_pad_combine_sc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1486 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_pad_spinavg.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3297 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_proton_correction.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2154 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_skymap.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4590 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_skymap_combine_sc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3515 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_spec_combine_sc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3390 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/eis_spin_avg.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2983 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/estimate_phase_speed.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4386 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_active_eyes.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3968 2023-05-15 20:42:14.000000 pyrfu-2.4.3/pyrfu/mms/feeps_bad_data.json
+-rw-r--r--   0 louisr     (501) staff       (20)     1697 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_correct_energies.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3354 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_energy_table.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1991 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_flat_field_corrections.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2982 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_omni.py
+-rw-r--r--   0 louisr     (501) staff       (20)     6204 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_pad.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2520 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_pad_spinavg.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4567 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_pitch_angles.py
+-rw-r--r--   0 louisr     (501) staff       (20)     5604 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_remove_bad_data.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2003 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_remove_sun.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1810 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_sector_spec.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1435 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_spin_avg.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1292 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/feeps_split_integral_ch.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2797 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/fft_bandpass.py
+-rw-r--r--   0 louisr     (501) staff       (20)    11773 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/fk_power_spectrum_4sc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3062 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/get_data.py
+-rw-r--r--   0 louisr     (501) staff       (20)     9081 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/get_dist.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4726 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/get_eis_allt.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4496 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/get_feeps_alleyes.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2525 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/get_feeps_omni.py
+-rw-r--r--   0 louisr     (501) staff       (20)     6173 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/get_hpca_dist.py
+-rw-r--r--   0 louisr     (501) staff       (20)     7052 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/get_pitch_angle_dist.py
+-rw-r--r--   0 louisr     (501) staff       (20)    11195 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/get_ts.py
+-rw-r--r--   0 louisr     (501) staff       (20)      926 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/get_variable.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1771 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/hpca_calc_anodes.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1395 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/hpca_energies.py
+-rw-r--r--   0 louisr     (501) staff       (20)     5663 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/hpca_pad.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1620 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/hpca_spin_sum.py
+-rw-r--r--   0 louisr     (501) staff       (20)     5642 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/lh_wave_analysis.py
+-rw-r--r--   0 louisr     (501) staff       (20)     6789 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/list_files.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4230 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/list_files_ancillary.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2770 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/load_ancillary.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2860 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/load_brst_segments.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4016 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/make_model_kappa.py
+-rw-r--r--   0 louisr     (501) staff       (20)     7022 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/make_model_rq.py
+-rw-r--r--   0 louisr     (501) staff       (20)     7043 2023-06-16 10:48:31.000000 pyrfu-2.4.3/pyrfu/mms/make_model_vdf.py
+-rw-r--r--   0 louisr     (501) staff       (20)    25074 2023-05-15 20:42:21.000000 pyrfu-2.4.3/pyrfu/mms/mms_keys.json
+-rw-r--r--   0 louisr     (501) staff       (20)     6101 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/probe_align_times.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2782 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/psd2def.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2796 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/psd2dpf.py
+-rw-r--r--   0 louisr     (501) staff       (20)    18467 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/psd_moments.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3307 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/psd_rebin.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2610 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/read_feeps_sector_masks_csv.py
+-rw-r--r--   0 louisr     (501) staff       (20)     8942 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/reduce.py
+-rw-r--r--   0 louisr     (501) staff       (20)     5397 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/remove_edist_background.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2034 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/remove_idist_background.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3131 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/remove_imoms_background.py
+-rw-r--r--   0 louisr     (501) staff       (20)     7075 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/rotate_tensor.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4320 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/scpot2ne.py
+-rw-r--r--   0 louisr     (501) staff       (20)      945 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/spectr_to_dataset.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.939657 pyrfu-2.4.3/pyrfu/mms/sun/
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20151111.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20160709.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20161028.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20170531.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20171003.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS1_FEEPS_ContaminatedSectors_20181005.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20151111.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20160709.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20161028.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20170531.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20171003.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS2_FEEPS_ContaminatedSectors_20181005.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20151111.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20160709.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20161028.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3134 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20170531.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20171003.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS3_FEEPS_ContaminatedSectors_20181005.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20151111.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20160709.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20161028.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20170531.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20171003.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3136 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/mms/sun/MMS4_FEEPS_ContaminatedSectors_20181005.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     3854 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/tokenize.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3248 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/vdf_elim.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1946 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/vdf_omni.py
+-rw-r--r--   0 louisr     (501) staff       (20)    11440 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/vdf_projection.py
+-rw-r--r--   0 louisr     (501) staff       (20)     8287 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/vdf_reduce.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2487 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/vdf_to_e64.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2337 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/mms/whistler_b2e.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.946049 pyrfu-2.4.3/pyrfu/models/
+-rw-r--r--   0 louisr     (501) staff       (20)      347 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/models/__init__.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2810 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/models/igrf.py
+-rw-r--r--   0 louisr     (501) staff       (20)    26798 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/models/igrf13coeffs.csv
+-rw-r--r--   0 louisr     (501) staff       (20)     6085 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/models/magnetopause_normal.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.988558 pyrfu-2.4.3/pyrfu/plot/
+-rw-r--r--   0 louisr     (501) staff       (20)     1582 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/__init__.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1725 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/add_position.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2366 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/annotate_heatmap.py
+-rw-r--r--   0 louisr     (501) staff       (20)      935 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/colorbar.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.989836 pyrfu-2.4.3/pyrfu/plot/logo/
+-rw-r--r--   0 louisr     (501) staff       (20)    43962 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/plot/logo/IRF_logo_blue_on_white.jpg
+-rw-r--r--   0 louisr     (501) staff       (20)     1108 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/make_labels.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3808 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/mms_pl_config.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2856 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/pl_scatter_matrix.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1539 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/pl_tx.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3832 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/plot_ang_ang.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1764 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/plot_clines.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2446 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/plot_heatmap.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1431 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/plot_line.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3646 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/plot_magnetosphere.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2212 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/plot_projection.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1946 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/plot_reduced_2d.py
+-rw-r--r--   0 louisr     (501) staff       (20)    11634 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/plot_sitl_overview.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4627 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/plot_spectr.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2423 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/plot_surf.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1511 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/span_tint.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2455 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/plot/zoom.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:01.210364 pyrfu-2.4.3/pyrfu/pyrf/
+-rw-r--r--   0 louisr     (501) staff       (20)     5552 2023-06-10 21:31:59.000000 pyrfu-2.4.3/pyrfu/pyrf/__init__.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1963 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/autocorr.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2651 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/average_vdf.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1156 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/avg_4sc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     5023 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/c_4_grad.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4188 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/c_4_j.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1315 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/c_4_k.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2633 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/c_4_v.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2080 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/calc_ag.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1422 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/calc_agyro.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1850 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/calc_dng.py
+-rw-r--r--   0 louisr     (501) staff       (20)      591 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/calc_dt.py
+-rw-r--r--   0 louisr     (501) staff       (20)      614 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/calc_fs.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1809 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/calc_sqrtq.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1223 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/cart2sph.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1929 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/cart2sph_ts.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1570 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/cdfepoch2datetime64.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1746 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/compress_cwt.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3430 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/convert_fac.py
+-rw-r--r--   0 louisr     (501) staff       (20)     6502 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/corr_deriv.py
+-rw-r--r--   0 louisr     (501) staff       (20)    10401 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/cotrans.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1430 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/cross.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1486 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/date_str.py
+-rw-r--r--   0 louisr     (501) staff       (20)      821 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/datetime2iso8601.py
+-rw-r--r--   0 louisr     (501) staff       (20)      842 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/datetime642iso8601.py
+-rw-r--r--   0 louisr     (501) staff       (20)      870 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/datetime642ttns.py
+-rw-r--r--   0 louisr     (501) staff       (20)      694 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/datetime642unix.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2570 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/dec_par_perp.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2871 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/dist_append.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1715 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/dot.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1594 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/dynamic_press.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2283 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/e_vxb.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1910 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/eb_nrf.py
+-rw-r--r--   0 louisr     (501) staff       (20)    36446 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/ebsp.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3678 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/edb.py
+-rw-r--r--   0 louisr     (501) staff       (20)      593 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/end.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3009 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/estimate.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1880 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/extend_tint.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3736 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/filt.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1971 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/find_closest.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3795 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/get_omni_data.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1298 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/gradient.py
+-rw-r--r--   0 louisr     (501) staff       (20)      987 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/gse2gsm.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2401 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/histogram.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3159 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/histogram2d.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1684 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/increments.py
+-rw-r--r--   0 louisr     (501) staff       (20)    18234 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/int_sph_dist.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2024 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/integrate.py
+-rw-r--r--   0 louisr     (501) staff       (20)     6075 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/iplasma_calc.py
+-rw-r--r--   0 louisr     (501) staff       (20)      585 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/iso2unix.py
+-rw-r--r--   0 louisr     (501) staff       (20)      875 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/iso86012datetime.py
+-rw-r--r--   0 louisr     (501) staff       (20)      626 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/iso86012datetime64.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1060 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/iso86012timevec.py
+-rw-r--r--   0 louisr     (501) staff       (20)      999 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/l_shell.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1281 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/lowpass.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2438 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/magnetosphere.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4500 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/match_phibe_dir.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1794 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/match_phibe_v.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2153 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/mean.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2391 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/mean_bins.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1220 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/mean_field.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2231 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/medfilt.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2362 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/median_bins.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1757 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/movmean.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4661 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/mva.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1473 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/new_xyz.py
+-rw-r--r--   0 louisr     (501) staff       (20)      957 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/norm.py
+-rw-r--r--   0 louisr     (501) staff       (20)      957 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/normalize.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2046 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/optimize_nbins_1d.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2746 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/optimize_nbins_2d.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3593 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/pid_4sc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1219 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/plasma_beta.py
+-rw-r--r--   0 louisr     (501) staff       (20)     7424 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/plasma_calc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2766 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/poynting_flux.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1897 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/pres_anis.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2958 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/psd.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1293 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/pvi.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2494 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/pvi_4sc.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1223 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/read_cdf.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2017 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/remove_repeated_points.py
+-rw-r--r--   0 louisr     (501) staff       (20)     8891 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/resample.py
+-rw-r--r--   0 louisr     (501) staff       (20)      697 2023-06-07 15:24:32.000000 pyrfu-2.4.3/pyrfu/pyrf/shock_models_parameters.json
+-rw-r--r--   0 louisr     (501) staff       (20)    15259 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/shock_normal.py
+-rw-r--r--   0 louisr     (501) staff       (20)     9264 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/shock_parameters.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1651 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/solid_angle.py
+-rw-r--r--   0 louisr     (501) staff       (20)      910 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/sph2cart.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2961 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/st_diff.py
+-rw-r--r--   0 louisr     (501) staff       (20)      568 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/start.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1857 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/struct_func.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1094 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/t_eval.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3716 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/time_clip.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1163 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/timevec2iso8601.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1501 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/trace.py
+-rw-r--r--   0 louisr     (501) staff       (20)      688 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/pyrf/transformation_indices.json
+-rw-r--r--   0 louisr     (501) staff       (20)     2422 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/ts_append.py
+-rw-r--r--   0 louisr     (501) staff       (20)      956 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/ts_scalar.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3043 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/ts_skymap.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1060 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/ts_tensor_xyz.py
+-rw-r--r--   0 louisr     (501) staff       (20)      672 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/ts_time.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1022 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/ts_vec_xyz.py
+-rw-r--r--   0 louisr     (501) staff       (20)      928 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/ttns2datetime64.py
+-rw-r--r--   0 louisr     (501) staff       (20)      718 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/unix2datetime64.py
+-rw-r--r--   0 louisr     (501) staff       (20)     3658 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/vht.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1683 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/wave_fft.py
+-rw-r--r--   0 louisr     (501) staff       (20)     6301 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/wavelet.py
+-rw-r--r--   0 louisr     (501) staff       (20)    14548 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/wavepolarize_means.py
+-rw-r--r--   0 louisr     (501) staff       (20)     2375 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/pyrf/waverage.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:01.218252 pyrfu-2.4.3/pyrfu/solo/
+-rw-r--r--   0 louisr     (501) staff       (20)      373 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/solo/__init__.py
+-rw-r--r--   0 louisr     (501) staff       (20)       48 2023-04-20 14:38:39.000000 pyrfu-2.4.3/pyrfu/solo/config.json
+-rw-r--r--   0 louisr     (501) staff       (20)     1109 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/solo/db_init.py
+-rw-r--r--   0 louisr     (501) staff       (20)     4619 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/solo/read_lfr_density.py
+-rw-r--r--   0 louisr     (501) staff       (20)     8224 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/solo/read_tnr.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:01.221674 pyrfu-2.4.3/pyrfu/tests/
+-rw-r--r--   0 louisr     (501) staff       (20)      210 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/tests/__init__.py
+-rw-r--r--   0 louisr     (501) staff       (20)     1553 2023-06-10 21:13:04.000000 pyrfu-2.4.3/pyrfu/tests/test_pyrf.py
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.688013 pyrfu-2.4.3/pyrfu.egg-info/
+-rw-r--r--   0 louisr     (501) staff       (20)     8862 2023-06-16 10:56:00.000000 pyrfu-2.4.3/pyrfu.egg-info/PKG-INFO
+-rw-r--r--   0 louisr     (501) staff       (20)     9550 2023-06-16 10:56:00.000000 pyrfu-2.4.3/pyrfu.egg-info/SOURCES.txt
+-rw-r--r--   0 louisr     (501) staff       (20)        1 2023-06-16 10:56:00.000000 pyrfu-2.4.3/pyrfu.egg-info/dependency_links.txt
+-rw-r--r--   0 louisr     (501) staff       (20)      235 2023-06-16 10:56:00.000000 pyrfu-2.4.3/pyrfu.egg-info/requires.txt
+-rw-r--r--   0 louisr     (501) staff       (20)       30 2023-06-16 10:56:00.000000 pyrfu-2.4.3/pyrfu.egg-info/top_level.txt
+-rw-r--r--   0 louisr     (501) staff       (20)     2691 2023-06-09 14:45:06.000000 pyrfu-2.4.3/requirements.txt
+-rw-r--r--   0 louisr     (501) staff       (20)       38 2023-06-16 10:56:01.228197 pyrfu-2.4.3/setup.cfg
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:00.479079 pyrfu-2.4.3/venv/
+drwxr-xr-x   0 louisr     (501) staff       (20)        0 2023-06-16 10:56:01.223550 pyrfu-2.4.3/venv/bin/
+-rw-r--r--   0 louisr     (501) staff       (20)     1175 2023-06-09 14:34:14.000000 pyrfu-2.4.3/venv/bin/activate_this.py
```

### Comparing `pyrfu-2.4.1/.github/workflows/flake8.yml` & `pyrfu-2.4.3/.github/workflows/flake8.yml`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/.github/workflows/publish-to-pypi.yml` & `pyrfu-2.4.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/.github/workflows/pylint.yml` & `pyrfu-2.4.3/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/.idea/inspectionProfiles/Project_Default.xml` & `pyrfu-2.4.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/.idea/workspace (LAPTOP-E2ISLACJ's conflicted copy 2022-10-01).xml` & `pyrfu-2.4.3/.idea/workspace (LAPTOP-E2ISLACJ's conflicted copy 2022-10-01).xml`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/.pre-commit-config.yaml` & `pyrfu-2.4.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/CONTRIBUTING.rst` & `pyrfu-2.4.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/LICENSE.txt` & `pyrfu-2.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/PKG-INFO` & `pyrfu-2.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrfu
-Version: 2.4.1
+Version: 2.4.3
 Summary: Python Space Physics (RymdFysik) Utilities
 Author-email: Louis RICHARD <louir@irfu.se>
 License: 
         MIT License
         
         Copyright (c) 2020 L. RICHARD
```

### Comparing `pyrfu-2.4.1/README.rst` & `pyrfu-2.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/docs/Makefile` & `pyrfu-2.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/docs/make.bat` & `pyrfu-2.4.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/docs/source/_static/logo-pyrfu.png` & `pyrfu-2.4.3/docs/source/_static/logo-pyrfu.png`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/docs/source/_static/logo-pyrfu.svg` & `pyrfu-2.4.3/docs/source/_static/logo-pyrfu.svg`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/docs/source/conf.py` & `pyrfu-2.4.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/docs/source/examples.rst` & `pyrfu-2.4.3/docs/source/examples.rst`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     examples/01_mms/example_mms_b_e_j.ipynb
     examples/01_mms/example_mms_ebfields.ipynb
     examples/01_mms/example_mms_edr_signatures.ipynb
     examples/01_mms/example_mms_eis.ipynb
     examples/01_mms/example_mms_electron_psd.ipynb
     examples/01_mms/example_mms_feeps.ipynb
     examples/01_mms/example_mms_hpca.ipynb
+    examples/01_mms/example_mms_ipshocks.ipynb
     examples/01_mms/example_mms_ohmslaw.ipynb
     examples/01_mms/example_mms_particle_deflux.ipynb
     examples/01_mms/example_mms_particle_distributions.ipynb
     examples/01_mms/example_mms_particle_pad.ipynb
     examples/01_mms/example_mms_reduced_ion_dist.ipynb
     examples/01_mms/example_mms_reduced_electron_dist.ipynb
     examples/01_mms/example_mms_polarizationanalysis.ipynb
```

### Comparing `pyrfu-2.4.1/docs/source/index.rst` & `pyrfu-2.4.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/docs/source/quick-overview.rst` & `pyrfu-2.4.3/docs/source/quick-overview.rst`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/examples/00_overview/.ipynb_checkpoints/quick-overview-checkpoint.ipynb` & `pyrfu-2.4.3/examples/00_overview/.ipynb_checkpoints/quick-overview-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/examples/00_overview/quick-overview.ipynb` & `pyrfu-2.4.3/examples/00_overview/quick-overview.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/examples/01_mms/example_mms_b_e_j.ipynb` & `pyrfu-2.4.3/examples/01_mms/example_mms_b_e_j.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/examples/01_mms/example_mms_ebfields.ipynb` & `pyrfu-2.4.3/examples/01_mms/example_mms_ebfields.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/examples/01_mms/example_mms_edr_signatures.ipynb` & `pyrfu-2.4.3/examples/01_mms/example_mms_edr_signatures.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/examples/01_mms/example_mms_eis.ipynb` & `pyrfu-2.4.3/examples/01_mms/example_mms_eis.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/examples/01_mms/example_mms_electron_psd.ipynb` & `pyrfu-2.4.3/examples/01_mms/example_mms_electron_psd.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/examples/01_mms/example_mms_feeps.ipynb` & `pyrfu-2.4.3/examples/01_mms/example_mms_feeps.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/examples/01_mms/example_mms_hpca.ipynb` & `pyrfu-2.4.3/examples/01_mms/example_mms_hpca.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/examples/01_mms/example_mms_ohmslaw.ipynb` & `pyrfu-2.4.3/examples/01_mms/example_mms_ohmslaw.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/examples/01_mms/example_mms_particle_deflux.ipynb` & `pyrfu-2.4.3/examples/01_mms/example_mms_particle_deflux.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/examples/01_mms/example_mms_particle_distributions.ipynb` & `pyrfu-2.4.3/examples/01_mms/example_mms_particle_distributions.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/examples/01_mms/example_mms_particle_pad.ipynb` & `pyrfu-2.4.3/examples/01_mms/example_mms_particle_pad.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/examples/01_mms/example_mms_polarizationanalysis.ipynb` & `pyrfu-2.4.3/examples/01_mms/example_mms_polarizationanalysis.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/examples/01_mms/example_mms_reduced_electron_dist.ipynb` & `pyrfu-2.4.3/examples/01_mms/example_mms_reduced_electron_dist.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/examples/01_mms/example_mms_reduced_ion_dist.ipynb` & `pyrfu-2.4.3/examples/01_mms/example_mms_reduced_ion_dist.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/examples/01_mms/example_mms_walen_test.ipynb` & `pyrfu-2.4.3/examples/01_mms/example_mms_walen_test.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/examples/02_dispersion/example_dispersion_one_fluid.ipynb` & `pyrfu-2.4.3/examples/02_dispersion/example_dispersion_one_fluid.ipynb`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/pyproject.toml` & `pyrfu-2.4.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel==0.38.1",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyrfu"
-version = "2.4.1"
+version = "2.4.3"
 description = "Python Space Physics (RymdFysik) Utilities"
 readme = "README.rst"
 authors = [{ name = "Louis RICHARD", email = "louir@irfu.se" }]
 license = { file = "LICENSE.txt" }
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Environment :: Other Environment",
@@ -112,17 +112,17 @@
     igrf13coeffs.csv,
     mms_keys.json,
     transformation_indices.json
 """
 ignored-modules = "scipy,cdflib"
 
 [tool.bumpver]
-current_version = "2.4.1"
+current_version = "2.4.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
-"pyrfu/__init__.py" = ["{version}"]
+"pyrfu/__init__.py" = ["{version}", "Copyright 2020-YYYY"]
```

### Comparing `pyrfu-2.4.1/pyrfu/__pycache__/__init__.cpython-38.pyc` & `pyrfu-2.4.3/pyrfu/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/pyrfu/dispersion/disp_surf_calc.py` & `pyrfu-2.4.3/pyrfu/dispersion/disp_surf_calc.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import itertools
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.11"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def _calc_diel(kc_, w_final, theta_, wp_e, wp_i, wc_i):
     # The elements of the dielectric tensor, using Swansons notation
     diel_s = 1 - wp_e**2 / (w_final**2 - 1) - wp_i**2 / (w_final**2 - wc_i**2)
     diel_d = -(wp_e**2) / (w_final * (w_final**2 - 1))
```

### Comparing `pyrfu-2.4.1/pyrfu/dispersion/one_fluid_dispersion.py` & `pyrfu-2.4.3/pyrfu/dispersion/one_fluid_dispersion.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 # 3rd party imports
 import numpy as np
 import xarray as xr
 from scipy import constants, optimize
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.11"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def _disprel(w, *args):
     assert len(args) == 6, "not enougth arguments"
     k, theta, v_a, c_s, wc_e, wc_p = args
```

### Comparing `pyrfu-2.4.1/pyrfu/lp/__init__.py` & `pyrfu-2.4.3/pyrfu/lp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 # Local imports
 from ..pyrf import estimate
 from .photo_current import photo_current
 from .thermal_current import thermal_current
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 __all__ = ["LangmuirProbe", "photo_current", "thermal_current"]
 
 
 class LangmuirProbe:
     r"""Defines either spherical, cylindrical, conical or spherical +
```

### Comparing `pyrfu-2.4.1/pyrfu/lp/photo_current.py` & `pyrfu-2.4.3/pyrfu/lp/photo_current.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 # 3rd party imports
 import numpy as np
 from scipy import interpolate
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 logging.captureWarnings(True)
 logging.basicConfig(
     format="[%(asctime)s] %(levelname)s: %(message)s",
     datefmt="%d-%b-%y %H:%M:%S",
     level=logging.INFO,
```

### Comparing `pyrfu-2.4.1/pyrfu/lp/thermal_current.py` & `pyrfu-2.4.3/pyrfu/lp/thermal_current.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 # 3rd party imports
 import numpy as np
 from scipy import constants, special
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def _spherical_body(z, u, x, i_p):
     j_thermal = np.zeros(u.shape)
 
     if z > 0:
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/__init__.py` & `pyrfu-2.4.3/pyrfu/mms/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,192 +1,192 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-from .calculate_epsilon import calculate_epsilon
-from .copy_files import copy_files
-from .copy_files_ancillary import copy_files_ancillary
-from .correct_edp_probe_timing import correct_edp_probe_timing
-from .db_get_ts import db_get_ts
-from .db_get_variable import db_get_variable
-from .db_init import db_init
-from .def2psd import def2psd
-from .dft_time_shift import dft_time_shift
-from .download_ancillary import download_ancillary
-from .download_data import download_data
-from .dpf2psd import dpf2psd
-from .dsl2gse import dsl2gse
-from .dsl2gsm import dsl2gsm
-
-# Energetic Ion Spectrometer (EIS)
-from .eis_ang_ang import eis_ang_ang
-from .eis_combine_proton_pad import eis_combine_proton_pad
-from .eis_combine_proton_skymap import eis_combine_proton_skymap
-from .eis_combine_proton_spec import eis_combine_proton_spec
-
-# from .eis_correlation import eis_correlation
-from .eis_moments import eis_moments
-from .eis_omni import eis_omni
-from .eis_pad import eis_pad
-from .eis_pad_combine_sc import eis_pad_combine_sc
-from .eis_pad_spinavg import eis_pad_spinavg
-from .eis_proton_correction import eis_proton_correction
-from .eis_skymap import eis_skymap
-from .eis_skymap_combine_sc import eis_skymap_combine_sc
-from .eis_spec_combine_sc import eis_spec_combine_sc
-from .eis_spin_avg import eis_spin_avg
-from .estimate_phase_speed import estimate_phase_speed
-
-# Fly’s Eye Energetic Particle Spectrometer (FEEPS)
-from .feeps_active_eyes import feeps_active_eyes
-from .feeps_correct_energies import feeps_correct_energies
-from .feeps_energy_table import feeps_energy_table
-from .feeps_flat_field_corrections import feeps_flat_field_corrections
-from .feeps_omni import feeps_omni
-from .feeps_pad import feeps_pad
-from .feeps_pad_spinavg import feeps_pad_spinavg
-from .feeps_pitch_angles import feeps_pitch_angles
-from .feeps_remove_bad_data import feeps_remove_bad_data
-from .feeps_remove_sun import feeps_remove_sun
-from .feeps_sector_spec import feeps_sector_spec
-from .feeps_spin_avg import feeps_spin_avg
-from .feeps_split_integral_ch import feeps_split_integral_ch
-from .fft_bandpass import fft_bandpass
-from .fk_power_spectrum_4sc import fk_power_spectrum_4sc
-from .get_data import get_data
-from .get_dist import get_dist
-from .get_eis_allt import get_eis_allt
-from .get_feeps_alleyes import get_feeps_alleyes
-from .get_feeps_omni import get_feeps_omni
-
-# Hot Plasma Composition Analyser (HPCA)
-from .get_hpca_dist import get_hpca_dist
-from .get_pitch_angle_dist import get_pitch_angle_dist
-from .get_ts import get_ts
-from .get_variable import get_variable
-from .hpca_calc_anodes import hpca_calc_anodes
-from .hpca_energies import hpca_energies
-from .hpca_pad import hpca_pad
-from .hpca_spin_sum import hpca_spin_sum
-from .lh_wave_analysis import lh_wave_analysis
-from .list_files import list_files
-from .list_files_ancillary import list_files_ancillary
-from .load_ancillary import load_ancillary
-from .load_brst_segments import load_brst_segments
-from .make_model_kappa import make_model_kappa
-from .make_model_vdf import make_model_vdf
-from .probe_align_times import probe_align_times
-from .psd2def import psd2def
-from .psd2dpf import psd2dpf
-from .psd_moments import psd_moments
-from .psd_rebin import psd_rebin
-from .read_feeps_sector_masks_csv import read_feeps_sector_masks_csv
-from .reduce import reduce
-from .remove_edist_background import remove_edist_background
-from .remove_idist_background import remove_idist_background
-from .remove_imoms_background import remove_imoms_background
-from .rotate_tensor import rotate_tensor
-from .scpot2ne import scpot2ne
-from .spectr_to_dataset import spectr_to_dataset
-
-# @Louis Richard
-from .tokenize import tokenize
-from .vdf_elim import vdf_elim
-from .vdf_omni import vdf_omni
-from .vdf_projection import vdf_projection
-from .vdf_reduce import vdf_frame_transformation, vdf_reduce
-from .vdf_to_e64 import vdf_to_e64
-from .whistler_b2e import whistler_b2e
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.22"
-__status__ = "Prototype"
-
-__all__ = [
-    "calculate_epsilon",
-    "copy_files",
-    "copy_files_ancillary",
-    "correct_edp_probe_timing",
-    "db_get_ts",
-    "db_get_variable",
-    "db_init",
-    "def2psd",
-    "dft_time_shift",
-    "download_ancillary",
-    "download_data",
-    "dpf2psd",
-    "dsl2gse",
-    "dsl2gsm",
-    "eis_ang_ang",
-    "eis_combine_proton_pad",
-    "eis_combine_proton_skymap",
-    "eis_combine_proton_spec",
-    "eis_moments",
-    "eis_omni",
-    "eis_pad",
-    "eis_pad_combine_sc",
-    "eis_pad_spinavg",
-    "eis_proton_correction",
-    "eis_skymap",
-    "eis_skymap_combine_sc",
-    "eis_spec_combine_sc",
-    "eis_spin_avg",
-    "estimate_phase_speed",
-    "feeps_active_eyes",
-    "feeps_correct_energies",
-    "feeps_energy_table",
-    "feeps_flat_field_corrections",
-    "feeps_omni",
-    "feeps_pad",
-    "feeps_pad_spinavg",
-    "feeps_pitch_angles",
-    "feeps_remove_bad_data",
-    "feeps_remove_sun",
-    "feeps_sector_spec",
-    "feeps_spin_avg",
-    "feeps_split_integral_ch",
-    "fft_bandpass",
-    "fk_power_spectrum_4sc",
-    "get_data",
-    "get_dist",
-    "get_eis_allt",
-    "get_feeps_alleyes",
-    "get_feeps_omni",
-    "get_hpca_dist",
-    "get_pitch_angle_dist",
-    "get_ts",
-    "get_variable",
-    "hpca_calc_anodes",
-    "hpca_energies",
-    "hpca_pad",
-    "hpca_spin_sum",
-    "lh_wave_analysis",
-    "list_files",
-    "list_files_ancillary",
-    "load_ancillary",
-    "load_brst_segments",
-    "make_model_kappa",
-    "make_model_vdf",
-    "probe_align_times",
-    "psd2def",
-    "psd2dpf",
-    "psd_moments",
-    "psd_rebin",
-    "read_feeps_sector_masks_csv",
-    "reduce",
-    "remove_edist_background",
-    "remove_idist_background",
-    "remove_imoms_background",
-    "rotate_tensor",
-    "scpot2ne",
-    "spectr_to_dataset",
-    "tokenize",
-    "vdf_elim",
-    "vdf_frame_transformation",
-    "vdf_omni",
-    "vdf_projection",
-    "vdf_reduce",
-    "vdf_to_e64",
-    "whistler_b2e",
-]
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+from .calculate_epsilon import calculate_epsilon
+from .copy_files import copy_files
+from .copy_files_ancillary import copy_files_ancillary
+from .correct_edp_probe_timing import correct_edp_probe_timing
+from .db_get_ts import db_get_ts
+from .db_get_variable import db_get_variable
+from .db_init import db_init
+from .def2psd import def2psd
+from .dft_time_shift import dft_time_shift
+from .download_ancillary import download_ancillary
+from .download_data import download_data
+from .dpf2psd import dpf2psd
+from .dsl2gse import dsl2gse
+from .dsl2gsm import dsl2gsm
+
+# Energetic Ion Spectrometer (EIS)
+from .eis_ang_ang import eis_ang_ang
+from .eis_combine_proton_pad import eis_combine_proton_pad
+from .eis_combine_proton_skymap import eis_combine_proton_skymap
+from .eis_combine_proton_spec import eis_combine_proton_spec
+
+# from .eis_correlation import eis_correlation
+from .eis_moments import eis_moments
+from .eis_omni import eis_omni
+from .eis_pad import eis_pad
+from .eis_pad_combine_sc import eis_pad_combine_sc
+from .eis_pad_spinavg import eis_pad_spinavg
+from .eis_proton_correction import eis_proton_correction
+from .eis_skymap import eis_skymap
+from .eis_skymap_combine_sc import eis_skymap_combine_sc
+from .eis_spec_combine_sc import eis_spec_combine_sc
+from .eis_spin_avg import eis_spin_avg
+from .estimate_phase_speed import estimate_phase_speed
+
+# Fly’s Eye Energetic Particle Spectrometer (FEEPS)
+from .feeps_active_eyes import feeps_active_eyes
+from .feeps_correct_energies import feeps_correct_energies
+from .feeps_energy_table import feeps_energy_table
+from .feeps_flat_field_corrections import feeps_flat_field_corrections
+from .feeps_omni import feeps_omni
+from .feeps_pad import feeps_pad
+from .feeps_pad_spinavg import feeps_pad_spinavg
+from .feeps_pitch_angles import feeps_pitch_angles
+from .feeps_remove_bad_data import feeps_remove_bad_data
+from .feeps_remove_sun import feeps_remove_sun
+from .feeps_sector_spec import feeps_sector_spec
+from .feeps_spin_avg import feeps_spin_avg
+from .feeps_split_integral_ch import feeps_split_integral_ch
+from .fft_bandpass import fft_bandpass
+from .fk_power_spectrum_4sc import fk_power_spectrum_4sc
+from .get_data import get_data
+from .get_dist import get_dist
+from .get_eis_allt import get_eis_allt
+from .get_feeps_alleyes import get_feeps_alleyes
+from .get_feeps_omni import get_feeps_omni
+
+# Hot Plasma Composition Analyser (HPCA)
+from .get_hpca_dist import get_hpca_dist
+from .get_pitch_angle_dist import get_pitch_angle_dist
+from .get_ts import get_ts
+from .get_variable import get_variable
+from .hpca_calc_anodes import hpca_calc_anodes
+from .hpca_energies import hpca_energies
+from .hpca_pad import hpca_pad
+from .hpca_spin_sum import hpca_spin_sum
+from .lh_wave_analysis import lh_wave_analysis
+from .list_files import list_files
+from .list_files_ancillary import list_files_ancillary
+from .load_ancillary import load_ancillary
+from .load_brst_segments import load_brst_segments
+from .make_model_kappa import make_model_kappa
+from .make_model_vdf import make_model_vdf
+from .probe_align_times import probe_align_times
+from .psd2def import psd2def
+from .psd2dpf import psd2dpf
+from .psd_moments import psd_moments
+from .psd_rebin import psd_rebin
+from .read_feeps_sector_masks_csv import read_feeps_sector_masks_csv
+from .reduce import reduce
+from .remove_edist_background import remove_edist_background
+from .remove_idist_background import remove_idist_background
+from .remove_imoms_background import remove_imoms_background
+from .rotate_tensor import rotate_tensor
+from .scpot2ne import scpot2ne
+from .spectr_to_dataset import spectr_to_dataset
+
+# @Louis Richard
+from .tokenize import tokenize
+from .vdf_elim import vdf_elim
+from .vdf_omni import vdf_omni
+from .vdf_projection import vdf_projection
+from .vdf_reduce import vdf_frame_transformation, vdf_reduce
+from .vdf_to_e64 import vdf_to_e64
+from .whistler_b2e import whistler_b2e
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+__all__ = [
+    "calculate_epsilon",
+    "copy_files",
+    "copy_files_ancillary",
+    "correct_edp_probe_timing",
+    "db_get_ts",
+    "db_get_variable",
+    "db_init",
+    "def2psd",
+    "dft_time_shift",
+    "download_ancillary",
+    "download_data",
+    "dpf2psd",
+    "dsl2gse",
+    "dsl2gsm",
+    "eis_ang_ang",
+    "eis_combine_proton_pad",
+    "eis_combine_proton_skymap",
+    "eis_combine_proton_spec",
+    "eis_moments",
+    "eis_omni",
+    "eis_pad",
+    "eis_pad_combine_sc",
+    "eis_pad_spinavg",
+    "eis_proton_correction",
+    "eis_skymap",
+    "eis_skymap_combine_sc",
+    "eis_spec_combine_sc",
+    "eis_spin_avg",
+    "estimate_phase_speed",
+    "feeps_active_eyes",
+    "feeps_correct_energies",
+    "feeps_energy_table",
+    "feeps_flat_field_corrections",
+    "feeps_omni",
+    "feeps_pad",
+    "feeps_pad_spinavg",
+    "feeps_pitch_angles",
+    "feeps_remove_bad_data",
+    "feeps_remove_sun",
+    "feeps_sector_spec",
+    "feeps_spin_avg",
+    "feeps_split_integral_ch",
+    "fft_bandpass",
+    "fk_power_spectrum_4sc",
+    "get_data",
+    "get_dist",
+    "get_eis_allt",
+    "get_feeps_alleyes",
+    "get_feeps_omni",
+    "get_hpca_dist",
+    "get_pitch_angle_dist",
+    "get_ts",
+    "get_variable",
+    "hpca_calc_anodes",
+    "hpca_energies",
+    "hpca_pad",
+    "hpca_spin_sum",
+    "lh_wave_analysis",
+    "list_files",
+    "list_files_ancillary",
+    "load_ancillary",
+    "load_brst_segments",
+    "make_model_kappa",
+    "make_model_vdf",
+    "probe_align_times",
+    "psd2def",
+    "psd2dpf",
+    "psd_moments",
+    "psd_rebin",
+    "read_feeps_sector_masks_csv",
+    "reduce",
+    "remove_edist_background",
+    "remove_idist_background",
+    "remove_imoms_background",
+    "rotate_tensor",
+    "scpot2ne",
+    "spectr_to_dataset",
+    "tokenize",
+    "vdf_elim",
+    "vdf_frame_transformation",
+    "vdf_omni",
+    "vdf_projection",
+    "vdf_reduce",
+    "vdf_to_e64",
+    "whistler_b2e",
+]
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/ancillary.json` & `pyrfu-2.4.3/pyrfu/mms/ancillary.json`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/pyrfu/mms/calculate_epsilon.py` & `pyrfu-2.4.3/pyrfu/mms/calculate_epsilon.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 # Local imports
 from ..pyrf.resample import resample
 from ..pyrf.ts_scalar import ts_scalar
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 q_e = constants.elementary_charge
 
 
 def calculate_epsilon(vdf, model_vdf, n_s, sc_pot, **kwargs):
     r"""Calculates epsilon parameter using model distribution.
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/copy_files.py` & `pyrfu-2.4.3/pyrfu/mms/copy_files.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 import subprocess
 
 # Local imports
 from .list_files import list_files
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.11"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def copy_files(var, tint, mms_id, tar_path: str = "./data/"):
     r"""Copy files from local_data_dir as defined in config.json to the target
     path.
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/copy_files_ancillary.py` & `pyrfu-2.4.3/pyrfu/mms/copy_files_ancillary.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 import subprocess
 
 # Local imports
 from .list_files_ancillary import list_files_ancillary
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2022"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.22"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def copy_files_ancillary(product, tint, mms_id, tar_path: str = "./data/"):
     r"""Copy ancillary files from local_data_dir as defined in config.json to
     the target path.
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/correct_edp_probe_timing.py` & `pyrfu-2.4.3/pyrfu/mms/correct_edp_probe_timing.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 # Local imports
 from ..pyrf.resample import resample
 from ..pyrf.ts_scalar import ts_scalar
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def correct_edp_probe_timing(sc_pot):
     r"""Corrects for the channel delays not accounted for in the MMS EDP
     processing. As described in the MMS EDP data products guide.
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/db_get_ts.py` & `pyrfu-2.4.3/pyrfu/mms/db_get_ts.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from .get_ts import get_ts
 
 # Local imports
 from .list_files import list_files
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 logging.captureWarnings(True)
 logging.basicConfig(
     format="[%(asctime)s] %(levelname)s: %(message)s",
     datefmt="%d-%b-%y %H:%M:%S",
     level=logging.INFO,
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/db_get_variable.py` & `pyrfu-2.4.3/pyrfu/mms/db_get_variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from .get_variable import get_variable
 
 # Local imports
 from .list_files import list_files
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 logging.captureWarnings(True)
 logging.basicConfig(
     format="[%(asctime)s] %(levelname)s: %(message)s",
     datefmt="%d-%b-%y %H:%M:%S",
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/db_init.py` & `pyrfu-2.4.3/pyrfu/solo/db_init.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,33 +4,35 @@
 import json
 
 # Built-in imports
 import os
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.11"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def db_init(local_data_dir):
-    r"""Setup the default path of MMS data.
+    r"""Setup the default path of SolO data.
 
     Parameters
     ----------
     local_data_dir : str
         Path to the data.
 
     """
 
     # Normalize the path and make sure that it exists
     local_data_dir = os.path.normpath(local_data_dir)
-    assert os.path.exists(local_data_dir), f"{local_data_dir} doesn't exists!!"
+    assert os.path.exists(
+        local_data_dir,
+    ), f"{local_data_dir} doesn't exists!!"
 
     # Path to the configuration file.
     pkg_path = os.path.dirname(os.path.abspath(__file__))
 
     # Read the current version of the configuration
     with open(os.path.join(pkg_path, "config.json"), "r", encoding="utf-8") as fs:
         config = json.load(fs)
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/def2psd.py` & `pyrfu-2.4.3/pyrfu/mms/dpf2psd.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# 3rd party imports
-import numpy as np
-import xarray as xr
-from scipy import constants
-
-# Local imports
-from .spectr_to_dataset import spectr_to_dataset
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.22"
-__status__ = "Prototype"
-
-
-def _mass_ratio(inp):
-    if inp.attrs["species"] in ["ions", "ion", "protons", "proton"]:
-        mass_ratio = 1
-    elif inp.attrs["species"] in ["alphas", "alpha", "helium"]:
-        mass_ratio = 4
-    elif inp.attrs["species"] in ["electrons", "e"]:
-        mass_ratio = constants.electron_mass / constants.proton_mass
-    else:
-        raise ValueError("Invalid specie")
-
-    return mass_ratio
-
-
-def _convert(inp, mass_ratio):
-    if inp.attrs["UNITS"] == "keV/(cm^2 s sr keV)":
-        tmp_data = inp.data.data / 1e12 * 0.53707 * mass_ratio**2
-    else:
-        raise ValueError("Invalid unit")
-
-    return tmp_data
-
-
-def def2psd(inp):
-    r"""Computes phase space density from differential energy flux as:
-
-    .. math:
-
-        f(E) = m^2 \frac{DEF}{E^2} * 0.53707,
-
-    where :math:`m` is the particle mass in atomic mass unit, :math:`DEF` is
-    the differential energy flux in 1/(cm sr s) and :math:`E` is the energy
-    in eV.
-
-    Parameters
-    ----------
-    inp : xarray.Dataset or xarray.DataArray
-        Time series of the differential energy flux in [(cm^{2} s sr)^{-1}].
-
-    Returns
-    -------
-    psd : xarray.Dataset
-        Time series of the phase space density in [s^{3} m^{-6}]
-
-    """
-
-    if isinstance(inp, xr.DataArray):
-        inp = spectr_to_dataset(inp)
-
-    tmp_data = _convert(inp, _mass_ratio(inp))
-
-    energy = inp.energy.data.copy()
-
-    if tmp_data.ndim == 2:
-        tmp_data = tmp_data[:, :, None, None]
-
-    data_r = np.reshape(
-        tmp_data,
-        (tmp_data.shape[0], tmp_data.shape[1], np.prod(tmp_data.shape[2:])),
-    )
-
-    if energy.ndim == 1:
-        energy_mat = np.tile(
-            energy,
-            (len(inp.time), np.prod(tmp_data.shape[2:]), 1),
-        )
-        energy_mat = np.transpose(energy_mat, [0, 2, 1])
-    elif energy.ndim == 2:
-        energy_mat = np.tile(energy, (np.prod(tmp_data.shape[2:]), 1, 1))
-        energy_mat = np.transpose(energy_mat, [1, 2, 0])
-    else:
-        raise ValueError("Invalid energy shape")
-
-    data_r /= energy_mat**2
-    tmp_data = np.reshape(data_r, tmp_data.shape)
-
-    psd = inp.copy()
-    psd.data.data = np.squeeze(tmp_data)
-    psd.attrs["UNITS"] = "s^3/m^6"
-
-    return psd
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# 3rd party imports
+import numpy as np
+import xarray as xr
+from scipy import constants
+
+# Local imports
+from .spectr_to_dataset import spectr_to_dataset
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def _mass_ratio(inp):
+    if inp.attrs["species"] in ["ions", "ion", "protons", "proton"]:
+        mass_ratio = 1
+    elif inp.attrs["species"] in ["alphas", "alpha", "helium"]:
+        mass_ratio = 4
+    elif inp.attrs["species"] in ["electrons", "e"]:
+        mass_ratio = constants.electron_mass / constants.proton_mass
+    else:
+        raise ValueError("Invalid specie")
+
+    return mass_ratio
+
+
+def _convert(inp, mass_ratio):
+    if isinstance(inp, xr.Dataset):
+        units = inp.data.attrs["UNITS"]
+    elif isinstance(inp, xr.DataArray):
+        units = inp.attrs["UNITS"]
+    else:
+        raise TypeError("Invalid input!!")
+
+    if units == "1/(cm^2 s sr keV)":
+        tmp_data = inp.data.data * 1e-3 / 1e12 * 0.53707 * mass_ratio**2
+    else:
+        raise ValueError("Invalid unit")
+
+    return tmp_data
+
+
+def dpf2psd(inp):
+    r"""Computes phase space density from differential particle flux.
+
+    Parameters
+    ----------
+    inp : xarray.Dataset or xarray.DataArray
+        Time series of the differential particle flux in
+        [(cm^{2} s sr keV)^{-1}].
+
+    Returns
+    -------
+    psd : xarray.Dataset
+        Time series of the phase space density in [s^{3} m^{-6}].
+
+    """
+
+    if isinstance(inp, xr.DataArray):
+        inp = spectr_to_dataset(inp)
+
+    tmp_data = _convert(inp, _mass_ratio(inp))
+
+    energy = inp.energy.data
+
+    if tmp_data.ndim == 2:
+        tmp_data = tmp_data[:, :, None, None]
+
+    data_r = np.reshape(
+        tmp_data,
+        (tmp_data.shape[0], tmp_data.shape[1], np.prod(tmp_data.shape[2:])),
+    )
+
+    if energy.ndim == 1:
+        energy_mat = np.tile(
+            energy,
+            (len(inp.time), np.prod(tmp_data.shape[2:]), 1),
+        )
+        energy_mat = np.transpose(energy_mat, [0, 2, 1])
+    elif energy.ndim == 2:
+        energy_mat = np.tile(energy, (np.prod(tmp_data.shape[2:]), 1, 1))
+        energy_mat = np.transpose(energy_mat, [1, 2, 0])
+    else:
+        raise ValueError("Invalid energy shape")
+
+    data_r /= energy_mat
+    tmp_data = np.reshape(data_r, tmp_data.shape)
+
+    psd = inp.copy()
+    psd.data.data = np.squeeze(tmp_data)
+    psd.attrs["UNITS"] = "s^3/m^6"
+
+    return psd
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/dft_time_shift.py` & `pyrfu-2.4.3/pyrfu/mms/dft_time_shift.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# 3rd party imports
-import numpy as np
-
-# Local imports
-from ..pyrf.calc_fs import calc_fs
-from ..pyrf.ts_scalar import ts_scalar
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.22"
-__status__ = "Prototype"
-
-
-def dft_time_shift(inp, tau):
-    r"""Shifts the input signal ``inp`` by ``tau`` seconds using discrete
-    fourier transform (DFT). Particularly useful when calculating the
-    frequency-wavenumber spectrum of the mms' spin-plane or axial probes.
-
-    Parameters
-    ----------
-    inp : xarray.DataArray
-        Time series to be shifted (Note : Only tensor order 1).
-    tau : float
-        Applied shift in seconds.
-
-    Returns
-    -------
-    out : xarray.DataArray
-        Time series of the shifted input.
-
-    See also
-    --------
-    pyrfu.mms.fk_power_spectrum : Calculates the frequency-wave number
-    power spectrum.
-
-    """
-
-    time, sig = [inp.time.data, inp.data]
-
-    # Sampling frequency
-    f_sampling = calc_fs(inp)
-
-    # Applied delay in samples.
-    delay = np.floor(tau * f_sampling)
-
-    # Forward FFT
-    sig_fft = np.fft.fft(sig)
-    n_p = len(sig)
-
-    # Disregard Nyquist frequency for even-sized dft
-    if not n_p % 2:
-        sig_fft[int(n_p / 2 + 1)] = 0
-
-    freq = (np.arange(n_p) + np.floor(n_p / 2)) % n_p - np.floor(n_p / 2)
-    freq /= n_p
-
-    # Backward FFT
-    out_data = np.fft.ifft(sig_fft * np.exp(-2j * np.pi * delay * freq))
-
-    out_time = time + int(tau * 1e9)
-
-    out = ts_scalar(out_time, out_data, attrs=inp.attrs)
-
-    return out
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# 3rd party imports
+import numpy as np
+
+# Local imports
+from ..pyrf.calc_fs import calc_fs
+from ..pyrf.ts_scalar import ts_scalar
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def dft_time_shift(inp, tau):
+    r"""Shifts the input signal ``inp`` by ``tau`` seconds using discrete
+    fourier transform (DFT). Particularly useful when calculating the
+    frequency-wavenumber spectrum of the mms' spin-plane or axial probes.
+
+    Parameters
+    ----------
+    inp : xarray.DataArray
+        Time series to be shifted (Note : Only tensor order 1).
+    tau : float
+        Applied shift in seconds.
+
+    Returns
+    -------
+    out : xarray.DataArray
+        Time series of the shifted input.
+
+    See also
+    --------
+    pyrfu.mms.fk_power_spectrum : Calculates the frequency-wave number
+    power spectrum.
+
+    """
+
+    time, sig = [inp.time.data, inp.data]
+
+    # Sampling frequency
+    f_sampling = calc_fs(inp)
+
+    # Applied delay in samples.
+    delay = np.floor(tau * f_sampling)
+
+    # Forward FFT
+    sig_fft = np.fft.fft(sig)
+    n_p = len(sig)
+
+    # Disregard Nyquist frequency for even-sized dft
+    if not n_p % 2:
+        sig_fft[int(n_p / 2 + 1)] = 0
+
+    freq = (np.arange(n_p) + np.floor(n_p / 2)) % n_p - np.floor(n_p / 2)
+    freq /= n_p
+
+    # Backward FFT
+    out_data = np.fft.ifft(sig_fft * np.exp(-2j * np.pi * delay * freq))
+
+    out_time = time + int(tau * 1e9)
+
+    out = ts_scalar(out_time, out_data, attrs=inp.attrs)
+
+    return out
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/download_ancillary.py` & `pyrfu-2.4.3/pyrfu/mms/download_ancillary.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 import numpy as np
 import pkg_resources
 import requests
 import tqdm
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2022"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.22"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 logging.captureWarnings(True)
 logging.basicConfig(
     format="[%(asctime)s] %(levelname)s: %(message)s",
     datefmt="%d-%b-%y %H:%M:%S",
     level=logging.INFO,
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/download_data.py` & `pyrfu-2.4.3/pyrfu/mms/download_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,251 +1,251 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Built-in imports
-import json
-import logging
-import os
-import re
-import warnings
-from bisect import bisect_left
-from datetime import datetime, timedelta
-from shutil import copy, copyfileobj
-from tempfile import NamedTemporaryFile
-
-# 3rd party imports
-import numpy as np
-import pkg_resources
-import requests
-import tqdm
-from dateutil.parser import parse
-
-# Local imports
-from .tokenize import tokenize
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2022"
-__license__ = "MIT"
-__version__ = "2.3.13"
-__status__ = "Prototype"
-
-logging.captureWarnings(True)
-logging.basicConfig(
-    format="[%(asctime)s] %(levelname)s: %(message)s",
-    datefmt="%d-%b-%y %H:%M:%S",
-    level=logging.INFO,
-)
-
-LASP_PUBL = "https://lasp.colorado.edu/mms/sdc/public/files/api/v1/"
-LASP_SITL = "https://lasp.colorado.edu/mms/sdc/sitl/files/api/v1/"
-
-
-def _login_lasp(user: str, password: str, lasp_url: str):
-    r"""Login to LASP colorado."""
-
-    session = requests.Session()
-    session.auth = (user, password)
-
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore", category=ResourceWarning)
-        _ = session.post("https://lasp.colorado.edu", verify=True, timeout=5)
-        testget = session.get(lasp_url, verify=True, timeout=5)
-
-    assert testget != "401", "Login failed!!"
-
-    return session, user
-
-
-def _construct_url(tint, mms_id, var, lasp_url):
-    r"""Construct the url that return a json-formatted string of science
-    filenames that are available for download according to:
-    https://lasp.colorado.edu/mms/sdc/team/about/how-to/
-    """
-
-    tint = np.array(tint).astype("<M8[ns]").astype(str)
-    tint = [datetime.strptime(t_[:-3], "%Y-%m-%dT%H:%M:%S.%f") for t_ in tint]
-    start_date = tint[0].strftime("%Y-%m-%d")
-    end_date = (tint[1] - timedelta(seconds=1)).strftime("%Y-%m-%d-%H-%M-%S")
-
-    url = f"{lasp_url}/file_info/science"
-    url = f"{url}?start_date={start_date}&end_date={end_date}&sc_id=mms{mms_id}"
-
-    url = f"{url}&instrument_id={var['inst']}"
-    url = f"{url}&data_rate_mode={var['tmmode']}"
-    url = f"{url}&data_level={var['lev']}"
-
-    if var["dtype"]:
-        url = f"{url}&descriptor={var['dtype']}"
-
-    return url
-
-
-def _files_in_interval(in_files, trange):
-    r"""Filters the file list returned by the SDC to the requested time
-    range. This filter is purposefully liberal, it regularly grabs an extra
-    file due to special cases
-    """
-
-    file_name = r"mms.*_([0-9]{8,14})_v(\d+).(\d+).(\d+).cdf"
-
-    file_times = []
-
-    regex = re.compile(file_name)
-
-    for file in in_files:
-        matches = regex.match(file["file_name"])
-        if matches:
-            file_times.append(
-                (
-                    file["file_name"],
-                    parse(matches.groups()[0]).timestamp(),
-                    file["timetag"],
-                    file["file_size"],
-                ),
-            )
-
-    # sort in time
-    sorted_files = sorted(file_times, key=lambda x: x[1])
-
-    times = [t[1] for t in sorted_files]
-
-    idx_min = bisect_left(times, parse(trange[0]).timestamp())
-
-    def mkout(f):
-        return {"file_name": f[0], "timetag": f[2], "size": f[3]}
-
-    if idx_min == 0:
-        files = list(map(mkout, sorted_files[idx_min:]))
-    else:
-        files = list(map(mkout, sorted_files[idx_min - 1 :]))
-
-    return files
-
-
-def _make_path(file, var, mms_id, lasp_url, data_path: str = ""):
-    r"""Construct path of the data file using the standard convention."""
-
-    file_date = parse(file["timetag"])
-
-    if not data_path:
-        pkg_path = os.path.dirname(os.path.abspath(__file__))
-
-        # Read the current version of the MMS configuration file
-        with open(os.path.join(pkg_path, "config.json"), "r", encoding="utf-8") as fs:
-            config = json.load(fs)
-
-        data_path = os.path.normpath(config["local_data_dir"])
-    else:
-        data_path = os.path.normpath(data_path)
-
-    assert os.path.exists(data_path), "local data directory doesn't exist!"
-
-    path_list = [
-        data_path,
-        f"mms{mms_id}",
-        var["inst"],
-        var["tmmode"],
-        var["lev"],
-        var["dtype"],
-        *file_date.strftime("%Y-%m").split("-"),
-    ]
-
-    if var["tmmode"].lower() == "brst":
-        path_list.append(file_date.strftime("%d"))
-
-    out_path = os.path.join(*path_list)
-    out_file = os.path.join(*path_list, file["file_name"])
-
-    download_url = f"{lasp_url}download/science?file={file['file_name']}"
-
-    return out_path, out_file, download_url
-
-
-def download_data(
-    var_str, tint, mms_id, login: str = "", password: str = "", data_path: str = ""
-):
-    r"""Downloads files containing field `var_str` over the time interval
-    `tint` for the spacecraft `mms_id`. The files are saved to `data_path`.
-
-    Parameters
-    ----------
-    var_str : str
-        Input key of variable.
-    tint : list of str
-        Time interval.
-    mms_id : str or int
-        Index of the target spacecraft.
-    login : str, Optional
-        Login to LASP MMS SITL. Default downloads from
-        https://lasp.colorado.edu/mms/sdc/public/
-    password : str, Optional
-        Password to LASP MMS SITL. Default downloads from
-        https://lasp.colorado.edu/mms/sdc/public/
-    data_path : str, Optional
-        Path of MMS data. If None use `pyrfu/mms/config.json`
-
-    """
-
-    if not login:
-        lasp_url = LASP_PUBL
-    else:
-        lasp_url = LASP_SITL
-
-    sdc_session, _ = _login_lasp(login, password, lasp_url)
-
-    headers = {}
-    try:
-        release_version = pkg_resources.get_distribution("pyrfu").version
-    except pkg_resources.DistributionNotFound:
-        release_version = "bleeding edge"
-
-    headers["User-Agent"] = f"pyrfu {release_version}"
-
-    var = tokenize(var_str)
-
-    root_path = os.path.dirname(os.path.abspath(__file__))
-
-    with open(
-        os.sep.join([root_path, "mms_keys.json"]), "r", encoding="utf-8"
-    ) as json_file:
-        keys_ = json.load(json_file)
-
-    var["dtype"] = keys_[var["inst"]][var_str.lower()]["dtype"]
-
-    url = _construct_url(tint, mms_id, var, lasp_url)
-
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore", category=ResourceWarning)
-        http_json = sdc_session.get(url, verify=True, headers=headers).json()
-
-    files_in_interval = _files_in_interval(http_json["files"], tint)
-
-    for file in files_in_interval:
-        out_path, out_file, dwl_url = _make_path(file, var, mms_id, lasp_url, data_path)
-
-        logging.info("Downloading %s from %s...", os.path.basename(out_file), dwl_url)
-
-        with warnings.catch_warnings():
-            warnings.simplefilter("ignore", category=ResourceWarning)
-            with sdc_session.get(
-                dwl_url,
-                stream=True,
-                verify=True,
-                headers=headers,
-            ) as fsrc:
-                with NamedTemporaryFile(delete=False) as ftmp:
-                    with tqdm.tqdm.wrapattr(
-                        fsrc.raw,
-                        "read",
-                        total=file["size"],
-                        ncols=60,
-                    ) as fsrc_raw:
-                        with open(ftmp.name, "wb") as fs:
-                            copyfileobj(fsrc_raw, fs)
-
-                os.makedirs(out_path, exist_ok=True)
-
-                # if the download was successful, copy to data directory
-                copy(ftmp.name, out_file)
-
-    sdc_session.close()
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# Built-in imports
+import json
+import logging
+import os
+import re
+import warnings
+from bisect import bisect_left
+from datetime import datetime, timedelta
+from shutil import copy, copyfileobj
+from tempfile import NamedTemporaryFile
+
+# 3rd party imports
+import numpy as np
+import pkg_resources
+import requests
+import tqdm
+from dateutil.parser import parse
+
+# Local imports
+from .tokenize import tokenize
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+logging.captureWarnings(True)
+logging.basicConfig(
+    format="[%(asctime)s] %(levelname)s: %(message)s",
+    datefmt="%d-%b-%y %H:%M:%S",
+    level=logging.INFO,
+)
+
+LASP_PUBL = "https://lasp.colorado.edu/mms/sdc/public/files/api/v1/"
+LASP_SITL = "https://lasp.colorado.edu/mms/sdc/sitl/files/api/v1/"
+
+
+def _login_lasp(user: str, password: str, lasp_url: str):
+    r"""Login to LASP colorado."""
+
+    session = requests.Session()
+    session.auth = (user, password)
+
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore", category=ResourceWarning)
+        _ = session.post("https://lasp.colorado.edu", verify=True, timeout=5)
+        testget = session.get(lasp_url, verify=True, timeout=5)
+
+    assert testget != "401", "Login failed!!"
+
+    return session, user
+
+
+def _construct_url(tint, mms_id, var, lasp_url):
+    r"""Construct the url that return a json-formatted string of science
+    filenames that are available for download according to:
+    https://lasp.colorado.edu/mms/sdc/team/about/how-to/
+    """
+
+    tint = np.array(tint).astype("<M8[ns]").astype(str)
+    tint = [datetime.strptime(t_[:-3], "%Y-%m-%dT%H:%M:%S.%f") for t_ in tint]
+    start_date = tint[0].strftime("%Y-%m-%d")
+    end_date = (tint[1] - timedelta(seconds=1)).strftime("%Y-%m-%d-%H-%M-%S")
+
+    url = f"{lasp_url}/file_info/science"
+    url = f"{url}?start_date={start_date}&end_date={end_date}&sc_id=mms{mms_id}"
+
+    url = f"{url}&instrument_id={var['inst']}"
+    url = f"{url}&data_rate_mode={var['tmmode']}"
+    url = f"{url}&data_level={var['lev']}"
+
+    if var["dtype"]:
+        url = f"{url}&descriptor={var['dtype']}"
+
+    return url
+
+
+def _files_in_interval(in_files, trange):
+    r"""Filters the file list returned by the SDC to the requested time
+    range. This filter is purposefully liberal, it regularly grabs an extra
+    file due to special cases
+    """
+
+    file_name = r"mms.*_([0-9]{8,14})_v(\d+).(\d+).(\d+).cdf"
+
+    file_times = []
+
+    regex = re.compile(file_name)
+
+    for file in in_files:
+        matches = regex.match(file["file_name"])
+        if matches:
+            file_times.append(
+                (
+                    file["file_name"],
+                    parse(matches.groups()[0]).timestamp(),
+                    file["timetag"],
+                    file["file_size"],
+                ),
+            )
+
+    # sort in time
+    sorted_files = sorted(file_times, key=lambda x: x[1])
+
+    times = [t[1] for t in sorted_files]
+
+    idx_min = bisect_left(times, parse(trange[0]).timestamp())
+
+    def mkout(f):
+        return {"file_name": f[0], "timetag": f[2], "size": f[3]}
+
+    if idx_min == 0:
+        files = list(map(mkout, sorted_files[idx_min:]))
+    else:
+        files = list(map(mkout, sorted_files[idx_min - 1 :]))
+
+    return files
+
+
+def _make_path(file, var, mms_id, lasp_url, data_path: str = ""):
+    r"""Construct path of the data file using the standard convention."""
+
+    file_date = parse(file["timetag"])
+
+    if not data_path:
+        pkg_path = os.path.dirname(os.path.abspath(__file__))
+
+        # Read the current version of the MMS configuration file
+        with open(os.path.join(pkg_path, "config.json"), "r", encoding="utf-8") as fs:
+            config = json.load(fs)
+
+        data_path = os.path.normpath(config["local_data_dir"])
+    else:
+        data_path = os.path.normpath(data_path)
+
+    assert os.path.exists(data_path), "local data directory doesn't exist!"
+
+    path_list = [
+        data_path,
+        f"mms{mms_id}",
+        var["inst"],
+        var["tmmode"],
+        var["lev"],
+        var["dtype"],
+        *file_date.strftime("%Y-%m").split("-"),
+    ]
+
+    if var["tmmode"].lower() == "brst":
+        path_list.append(file_date.strftime("%d"))
+
+    out_path = os.path.join(*path_list)
+    out_file = os.path.join(*path_list, file["file_name"])
+
+    download_url = f"{lasp_url}download/science?file={file['file_name']}"
+
+    return out_path, out_file, download_url
+
+
+def download_data(
+    var_str, tint, mms_id, login: str = "", password: str = "", data_path: str = ""
+):
+    r"""Downloads files containing field `var_str` over the time interval
+    `tint` for the spacecraft `mms_id`. The files are saved to `data_path`.
+
+    Parameters
+    ----------
+    var_str : str
+        Input key of variable.
+    tint : list of str
+        Time interval.
+    mms_id : str or int
+        Index of the target spacecraft.
+    login : str, Optional
+        Login to LASP MMS SITL. Default downloads from
+        https://lasp.colorado.edu/mms/sdc/public/
+    password : str, Optional
+        Password to LASP MMS SITL. Default downloads from
+        https://lasp.colorado.edu/mms/sdc/public/
+    data_path : str, Optional
+        Path of MMS data. If None use `pyrfu/mms/config.json`
+
+    """
+
+    if not login:
+        lasp_url = LASP_PUBL
+    else:
+        lasp_url = LASP_SITL
+
+    sdc_session, _ = _login_lasp(login, password, lasp_url)
+
+    headers = {}
+    try:
+        release_version = pkg_resources.get_distribution("pyrfu").version
+    except pkg_resources.DistributionNotFound:
+        release_version = "bleeding edge"
+
+    headers["User-Agent"] = f"pyrfu {release_version}"
+
+    var = tokenize(var_str)
+
+    root_path = os.path.dirname(os.path.abspath(__file__))
+
+    with open(
+        os.sep.join([root_path, "mms_keys.json"]), "r", encoding="utf-8"
+    ) as json_file:
+        keys_ = json.load(json_file)
+
+    var["dtype"] = keys_[var["inst"]][var_str.lower()]["dtype"]
+
+    url = _construct_url(tint, mms_id, var, lasp_url)
+
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore", category=ResourceWarning)
+        http_json = sdc_session.get(url, verify=True, headers=headers).json()
+
+    files_in_interval = _files_in_interval(http_json["files"], tint)
+
+    for file in files_in_interval:
+        out_path, out_file, dwl_url = _make_path(file, var, mms_id, lasp_url, data_path)
+
+        logging.info("Downloading %s from %s...", os.path.basename(out_file), dwl_url)
+
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore", category=ResourceWarning)
+            with sdc_session.get(
+                dwl_url,
+                stream=True,
+                verify=True,
+                headers=headers,
+            ) as fsrc:
+                with NamedTemporaryFile(delete=False) as ftmp:
+                    with tqdm.tqdm.wrapattr(
+                        fsrc.raw,
+                        "read",
+                        total=file["size"],
+                        ncols=60,
+                    ) as fsrc_raw:
+                        with open(ftmp.name, "wb") as fs:
+                            copyfileobj(fsrc_raw, fs)
+
+                os.makedirs(out_path, exist_ok=True)
+
+                # if the download was successful, copy to data directory
+                copy(ftmp.name, out_file)
+
+    sdc_session.close()
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/dpf2psd.py` & `pyrfu-2.4.3/pyrfu/mms/def2psd.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from scipy import constants
 
 # Local imports
 from .spectr_to_dataset import spectr_to_dataset
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def _mass_ratio(inp):
     if inp.attrs["species"] in ["ions", "ion", "protons", "proton"]:
         mass_ratio = 1
     elif inp.attrs["species"] in ["alphas", "alpha", "helium"]:
@@ -27,51 +27,51 @@
     else:
         raise ValueError("Invalid specie")
 
     return mass_ratio
 
 
 def _convert(inp, mass_ratio):
-    if isinstance(inp, xr.Dataset):
-        units = inp.data.attrs["UNITS"]
-    elif isinstance(inp, xr.DataArray):
-        units = inp.attrs["UNITS"]
-    else:
-        raise TypeError("Invalid input!!")
-
-    if units == "1/(cm^2 s sr keV)":
-        tmp_data = inp.data.data * 1e-3 / 1e12 * 0.53707 * mass_ratio**2
+    if inp.attrs["UNITS"] == "keV/(cm^2 s sr keV)":
+        tmp_data = inp.data.data / 1e12 * 0.53707 * mass_ratio**2
     else:
         raise ValueError("Invalid unit")
 
     return tmp_data
 
 
-def dpf2psd(inp):
-    r"""Computes phase space density from differential particle flux.
+def def2psd(inp):
+    r"""Computes phase space density from differential energy flux as:
+
+    .. math:
+
+        f(E) = m^2 \frac{DEF}{E^2} * 0.53707,
+
+    where :math:`m` is the particle mass in atomic mass unit, :math:`DEF` is
+    the differential energy flux in 1/(cm sr s) and :math:`E` is the energy
+    in eV.
 
     Parameters
     ----------
     inp : xarray.Dataset or xarray.DataArray
-        Time series of the differential particle flux in
-        [(cm^{2} s sr keV)^{-1}].
+        Time series of the differential energy flux in [(cm^{2} s sr)^{-1}].
 
     Returns
     -------
     psd : xarray.Dataset
-        Time series of the phase space density in [s^{3} m^{-6}].
+        Time series of the phase space density in [s^{3} m^{-6}]
 
     """
 
     if isinstance(inp, xr.DataArray):
         inp = spectr_to_dataset(inp)
 
     tmp_data = _convert(inp, _mass_ratio(inp))
 
-    energy = inp.energy.data
+    energy = inp.energy.data.copy()
 
     if tmp_data.ndim == 2:
         tmp_data = tmp_data[:, :, None, None]
 
     data_r = np.reshape(
         tmp_data,
         (tmp_data.shape[0], tmp_data.shape[1], np.prod(tmp_data.shape[2:])),
@@ -85,15 +85,15 @@
         energy_mat = np.transpose(energy_mat, [0, 2, 1])
     elif energy.ndim == 2:
         energy_mat = np.tile(energy, (np.prod(tmp_data.shape[2:]), 1, 1))
         energy_mat = np.transpose(energy_mat, [1, 2, 0])
     else:
         raise ValueError("Invalid energy shape")
 
-    data_r /= energy_mat
+    data_r /= energy_mat**2
     tmp_data = np.reshape(data_r, tmp_data.shape)
 
     psd = inp.copy()
     psd.data.data = np.squeeze(tmp_data)
     psd.attrs["UNITS"] = "s^3/m^6"
 
     return psd
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/dsl2gse.py` & `pyrfu-2.4.3/pyrfu/mms/dsl2gse.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# 3rd party imports
-import numpy as np
-import xarray as xr
-
-# Local imports
-from ..pyrf.calc_fs import calc_fs
-from ..pyrf.cotrans import cotrans
-from ..pyrf.resample import resample
-from ..pyrf.ts_vec_xyz import ts_vec_xyz
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2023"
-__license__ = "MIT"
-__version__ = "2.3.26"
-__status__ = "Prototype"
-
-
-def _transformation_matrix(spin_axis, direction):
-    r_x, r_y, r_z = [spin_axis[:, i] for i in range(3)]
-
-    fact = 1.0 / np.sqrt(r_y**2 + r_z**2)
-    out = np.zeros((len(fact), 3, 3))
-    out[:, 0, :] = np.transpose(
-        np.stack(
-            [
-                fact * (r_y**2 + r_z**2),
-                -fact * r_x * r_y,
-                -fact * r_x * r_z,
-            ],
-        ),
-    )
-
-    out[:, 1, :] = np.transpose(
-        np.stack([0.0 * fact, fact * r_z, -fact * r_y]),
-    )
-
-    out[:, 2, :] = np.transpose(np.stack([r_x, r_y, r_z]))
-
-    if direction == 1:
-        out = np.transpose(out, [0, 2, 1])
-
-    return out
-
-
-def dsl2gse(inp, defatt, direction: int = 1):
-    r"""Transform time series from MMS's DSL to GSE.
-
-    Parameters
-    ----------
-    inp : xarray.DataArray
-        Input time series to convert.
-    defatt : xarray.Dataset or array_like
-        Spacecraft attitude.
-    direction : {1, -1}, Optional
-        Direction of transformation. +1 DSL -> GSE, -1 GSE -> DSL.
-        Default is 1.
-
-    Returns
-    -------
-    out : xarray.DataArray
-        Time series of the input field in the new coordinates systems.
-
-    Examples
-    --------
-    >>> from pyrfu.mms import get_data, load_ancillary, dsl2gse
-
-    Define time interval
-
-    >>> tint = ["2015-05-09T14:00:000", "2015-05-09T17:59:590"]
-
-    Load magnetic field in spacecraft coordinates
-
-    >>> b_xyz = get_data("b_dmpa_fgm_brst_l2", tint, 1)
-
-    Load spacecraft attitude
-
-    >>> defatt = load_ancillary("defatt", tint, 1)
-
-    Transform magnetic field to GSE
-
-    >>> b_gse = dsl2gse(b_xyz, defatt)
-
-    """
-
-    if isinstance(defatt, xr.Dataset):
-        x = np.cos(np.deg2rad(defatt.z_dec)) * np.cos(
-            np.deg2rad(defatt.z_ra.data),
-        )
-        y = np.cos(np.deg2rad(defatt.z_dec)) * np.sin(
-            np.deg2rad(defatt.z_ra.data),
-        )
-        z = np.sin(np.deg2rad(defatt.z_dec))
-        sax_gei = np.transpose(
-            np.vstack([defatt.time.data.astype("int") / 1e9, x, y, z]),
-        )
-        sax_gse = cotrans(sax_gei, "gei>gse")
-        sax_gse = ts_vec_xyz(
-            (sax_gse[:, 0] * 1e9).astype("datetime64[ns]"),
-            sax_gse[:, 1:],
-        )
-
-        spin_ax_gse = resample(sax_gse, inp, f_s=calc_fs(inp))
-        spin_axis = spin_ax_gse.data
-
-    elif isinstance(defatt, (np.ndarray, list)) and len(defatt) == 3:
-        spin_axis = defatt
-
-    else:
-        raise ValueError("unrecognized DEFATT/SAX input")
-
-    # Compute transformation natrix
-    transf_mat = _transformation_matrix(spin_axis, direction)
-
-    out_data = np.einsum("kji,ki->kj", transf_mat, inp.data)
-
-    out = inp.copy()
-    out.data = out_data
-    out.attrs["COORDINATE_SYSTEM"] = "GSE"
-
-    return out
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# 3rd party imports
+import numpy as np
+import xarray as xr
+
+# Local imports
+from ..pyrf.calc_fs import calc_fs
+from ..pyrf.cotrans import cotrans
+from ..pyrf.resample import resample
+from ..pyrf.ts_vec_xyz import ts_vec_xyz
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def _transformation_matrix(spin_axis, direction):
+    r_x, r_y, r_z = [spin_axis[:, i] for i in range(3)]
+
+    fact = 1.0 / np.sqrt(r_y**2 + r_z**2)
+    out = np.zeros((len(fact), 3, 3))
+    out[:, 0, :] = np.transpose(
+        np.stack(
+            [
+                fact * (r_y**2 + r_z**2),
+                -fact * r_x * r_y,
+                -fact * r_x * r_z,
+            ],
+        ),
+    )
+
+    out[:, 1, :] = np.transpose(
+        np.stack([0.0 * fact, fact * r_z, -fact * r_y]),
+    )
+
+    out[:, 2, :] = np.transpose(np.stack([r_x, r_y, r_z]))
+
+    if direction == 1:
+        out = np.transpose(out, [0, 2, 1])
+
+    return out
+
+
+def dsl2gse(inp, defatt, direction: int = 1):
+    r"""Transform time series from MMS's DSL to GSE.
+
+    Parameters
+    ----------
+    inp : xarray.DataArray
+        Input time series to convert.
+    defatt : xarray.Dataset or array_like
+        Spacecraft attitude.
+    direction : {1, -1}, Optional
+        Direction of transformation. +1 DSL -> GSE, -1 GSE -> DSL.
+        Default is 1.
+
+    Returns
+    -------
+    out : xarray.DataArray
+        Time series of the input field in the new coordinates systems.
+
+    Examples
+    --------
+    >>> from pyrfu.mms import get_data, load_ancillary, dsl2gse
+
+    Define time interval
+
+    >>> tint = ["2015-05-09T14:00:000", "2015-05-09T17:59:590"]
+
+    Load magnetic field in spacecraft coordinates
+
+    >>> b_xyz = get_data("b_dmpa_fgm_brst_l2", tint, 1)
+
+    Load spacecraft attitude
+
+    >>> defatt = load_ancillary("defatt", tint, 1)
+
+    Transform magnetic field to GSE
+
+    >>> b_gse = dsl2gse(b_xyz, defatt)
+
+    """
+
+    if isinstance(defatt, xr.Dataset):
+        x = np.cos(np.deg2rad(defatt.z_dec)) * np.cos(
+            np.deg2rad(defatt.z_ra.data),
+        )
+        y = np.cos(np.deg2rad(defatt.z_dec)) * np.sin(
+            np.deg2rad(defatt.z_ra.data),
+        )
+        z = np.sin(np.deg2rad(defatt.z_dec))
+        sax_gei = np.transpose(
+            np.vstack([defatt.time.data.astype("int") / 1e9, x, y, z]),
+        )
+        sax_gse = cotrans(sax_gei, "gei>gse")
+        sax_gse = ts_vec_xyz(
+            (sax_gse[:, 0] * 1e9).astype("datetime64[ns]"),
+            sax_gse[:, 1:],
+        )
+
+        spin_ax_gse = resample(sax_gse, inp, f_s=calc_fs(inp))
+        spin_axis = spin_ax_gse.data
+
+    elif isinstance(defatt, (np.ndarray, list)) and len(defatt) == 3:
+        spin_axis = defatt
+
+    else:
+        raise ValueError("unrecognized DEFATT/SAX input")
+
+    # Compute transformation natrix
+    transf_mat = _transformation_matrix(spin_axis, direction)
+
+    out_data = np.einsum("kji,ki->kj", transf_mat, inp.data)
+
+    out = inp.copy()
+    out.data = out_data
+    out.attrs["COORDINATE_SYSTEM"] = "GSE"
+
+    return out
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/dsl2gsm.py` & `pyrfu-2.4.3/pyrfu/mms/dsl2gsm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# 3rd party imports
-import numpy as np
-import xarray as xr
-
-# Local imports
-from ..pyrf.calc_fs import calc_fs
-from ..pyrf.cotrans import cotrans
-from ..pyrf.resample import resample
-from ..pyrf.ts_vec_xyz import ts_vec_xyz
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2023"
-__license__ = "MIT"
-__version__ = "2.3.26"
-__status__ = "Prototype"
-
-
-def _transformation_matrix(spin_axis, direction):
-    r_x, r_y, r_z = [spin_axis[:, i] for i in range(3)]
-
-    a = 1.0 / np.sqrt(r_y**2 + r_z**2)
-    out = np.zeros((len(a), 3, 3))
-    out[:, 0, :] = np.transpose(
-        np.stack([a * (r_y**2 + r_z**2), -a * r_x * r_y, -a * r_x * r_z]),
-    )
-
-    out[:, 1, :] = np.transpose(np.stack([0.0 * a, a * r_z, -a * r_y]))
-
-    out[:, 2, :] = np.transpose(np.stack([r_x, r_y, r_z]))
-
-    if direction == 1:
-        out = np.transpose(out, [0, 2, 1])
-
-    return out
-
-
-def dsl2gsm(inp, defatt, direction: int = 1):
-    r"""Transform time series from MMS's DSL to GSM.
-
-    Parameters
-    ----------
-    inp : xarray.DataArray
-        Input time series to convert.
-    defatt : xarray.Dataset or array_like
-        Spacecraft attitude.
-    direction : {1, -1}, optional
-        Direction of transformation. +1 DSL -> GSE, -1 GSE -> DSL.
-        Default is 1.
-
-    Returns
-    -------
-    out : xarray.DataArray
-        Time series of the input field in the new coordinates systems.
-
-    Examples
-    --------
-    >>> from pyrfu.mms import get_data, load_ancillary, dsl2gse
-
-    Define time interval
-
-    >>> tint = ["2015-05-09T14:00:000", "2015-05-09T17:59:590"]
-
-    Load magnetic field in spacecraft coordinates
-
-    >>> b_xyz = get_data("b_dmpa_fgm_brst_l2", tint, 1)
-
-    Load spacecraft attitude
-
-    >>> defatt = load_ancillary("defatt", tint, 1)
-
-    Transform magnetic field to GSE
-
-    >>> b_gse = dsl2gse(b_xyz, defatt)
-
-    """
-
-    if isinstance(defatt, xr.Dataset):
-        x = np.cos(np.deg2rad(defatt.z_dec)) * np.cos(
-            np.deg2rad(defatt.z_ra.data),
-        )
-        y = np.cos(np.deg2rad(defatt.z_dec)) * np.sin(
-            np.deg2rad(defatt.z_ra.data),
-        )
-        z = np.sin(np.deg2rad(defatt.z_dec))
-        sax_gei = np.transpose(
-            np.vstack([defatt.time.data.astype("int") / 1e9, x, y, z]),
-        )
-        sax_gsm = cotrans(sax_gei, "gei>gsm")
-        sax_gsm = ts_vec_xyz(
-            (sax_gsm[:, 0] * 1e9).astype("datetime64[ns]"),
-            sax_gsm[:, 1:],
-        )
-
-        spin_ax_gsm = resample(sax_gsm, inp, f_s=calc_fs(inp))
-        spin_axis = spin_ax_gsm.data
-
-    elif isinstance(defatt, (np.ndarray, list)) and len(defatt) == 3:
-        spin_axis = defatt
-
-    else:
-        raise ValueError("unrecognized DEFATT/SAX input")
-
-    # Compute transformation matrix
-    transf_mat = _transformation_matrix(spin_axis, direction)
-
-    out_data = np.einsum("kji,ki->kj", transf_mat, inp.data)
-
-    out = inp.copy()
-    out.data = out_data
-    out.attrs["COORDINATE_SYSTEM"] = "GSM"
-
-    return out
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# 3rd party imports
+import numpy as np
+import xarray as xr
+
+# Local imports
+from ..pyrf.calc_fs import calc_fs
+from ..pyrf.cotrans import cotrans
+from ..pyrf.resample import resample
+from ..pyrf.ts_vec_xyz import ts_vec_xyz
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def _transformation_matrix(spin_axis, direction):
+    r_x, r_y, r_z = [spin_axis[:, i] for i in range(3)]
+
+    a = 1.0 / np.sqrt(r_y**2 + r_z**2)
+    out = np.zeros((len(a), 3, 3))
+    out[:, 0, :] = np.transpose(
+        np.stack([a * (r_y**2 + r_z**2), -a * r_x * r_y, -a * r_x * r_z]),
+    )
+
+    out[:, 1, :] = np.transpose(np.stack([0.0 * a, a * r_z, -a * r_y]))
+
+    out[:, 2, :] = np.transpose(np.stack([r_x, r_y, r_z]))
+
+    if direction == 1:
+        out = np.transpose(out, [0, 2, 1])
+
+    return out
+
+
+def dsl2gsm(inp, defatt, direction: int = 1):
+    r"""Transform time series from MMS's DSL to GSM.
+
+    Parameters
+    ----------
+    inp : xarray.DataArray
+        Input time series to convert.
+    defatt : xarray.Dataset or array_like
+        Spacecraft attitude.
+    direction : {1, -1}, optional
+        Direction of transformation. +1 DSL -> GSE, -1 GSE -> DSL.
+        Default is 1.
+
+    Returns
+    -------
+    out : xarray.DataArray
+        Time series of the input field in the new coordinates systems.
+
+    Examples
+    --------
+    >>> from pyrfu.mms import get_data, load_ancillary, dsl2gse
+
+    Define time interval
+
+    >>> tint = ["2015-05-09T14:00:000", "2015-05-09T17:59:590"]
+
+    Load magnetic field in spacecraft coordinates
+
+    >>> b_xyz = get_data("b_dmpa_fgm_brst_l2", tint, 1)
+
+    Load spacecraft attitude
+
+    >>> defatt = load_ancillary("defatt", tint, 1)
+
+    Transform magnetic field to GSE
+
+    >>> b_gse = dsl2gse(b_xyz, defatt)
+
+    """
+
+    if isinstance(defatt, xr.Dataset):
+        x = np.cos(np.deg2rad(defatt.z_dec)) * np.cos(
+            np.deg2rad(defatt.z_ra.data),
+        )
+        y = np.cos(np.deg2rad(defatt.z_dec)) * np.sin(
+            np.deg2rad(defatt.z_ra.data),
+        )
+        z = np.sin(np.deg2rad(defatt.z_dec))
+        sax_gei = np.transpose(
+            np.vstack([defatt.time.data.astype("int") / 1e9, x, y, z]),
+        )
+        sax_gsm = cotrans(sax_gei, "gei>gsm")
+        sax_gsm = ts_vec_xyz(
+            (sax_gsm[:, 0] * 1e9).astype("datetime64[ns]"),
+            sax_gsm[:, 1:],
+        )
+
+        spin_ax_gsm = resample(sax_gsm, inp, f_s=calc_fs(inp))
+        spin_axis = spin_ax_gsm.data
+
+    elif isinstance(defatt, (np.ndarray, list)) and len(defatt) == 3:
+        spin_axis = defatt
+
+    else:
+        raise ValueError("unrecognized DEFATT/SAX input")
+
+    # Compute transformation matrix
+    transf_mat = _transformation_matrix(spin_axis, direction)
+
+    out_data = np.einsum("kji,ki->kj", transf_mat, inp.data)
+
+    out = inp.copy()
+    out.data = out_data
+    out.attrs["COORDINATE_SYSTEM"] = "GSM"
+
+    return out
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/eis_ang_ang.py` & `pyrfu-2.4.3/pyrfu/mms/eis_ang_ang.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 import xarray as xr
 
 # Local imports
 from .dsl2gse import dsl2gse
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def _check_spin(spin):
     _, spin_inds = np.unique(spin, return_index=True)
 
     len_spin = np.max(np.diff(spin_inds))
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/eis_combine_proton_pad.py` & `pyrfu-2.4.3/pyrfu/mms/eis_combine_proton_pad.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 from .eis_omni import eis_omni
 
 # Local imports
 from .eis_pad import eis_pad
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def _despin(inp, spin_nums):
     spin_starts = np.where(spin_nums[1:] > spin_nums[:-1])[0]
     time_rec = inp.time.data[spin_starts]
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/eis_combine_proton_skymap.py` & `pyrfu-2.4.3/pyrfu/mms/eis_combine_proton_skymap.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 # Local imports
 from .eis_combine_proton_spec import eis_combine_proton_spec
 from .eis_skymap import eis_skymap
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def eis_combine_proton_skymap(
     phxtof_allt,
     extof_allt,
     en_chan: list = None,
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/eis_combine_proton_spec.py` & `pyrfu-2.4.3/pyrfu/mms/eis_combine_proton_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from ..pyrf.datetime642iso8601 import datetime642iso8601
 
 # Local imports
 from .list_files import list_files
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def _check_time(proton_phxtof, proton_extof):
     data_size = [len(proton_phxtof), len(proton_extof)]
 
     if data_size[0] == data_size[1]:
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/eis_moments.py` & `pyrfu-2.4.3/pyrfu/mms/eis_moments.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 # Local imports
 from ..pyrf.resample import resample
 from ..pyrf.ts_scalar import ts_scalar
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def eis_moments(
     inp,
     specie: str = "proton",
     n_bg: xr.DataArray = None,
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/eis_omni.py` & `pyrfu-2.4.3/pyrfu/mms/eis_omni.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def eis_omni(eis_allt, method: str = "mean"):
     r"""Calculates the omni-directional flux for all 6 telescopes.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/eis_pad.py` & `pyrfu-2.4.3/pyrfu/mms/eis_pad.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 # Local imports
 from ..pyrf.normalize import normalize
 from ..pyrf.resample import resample
 from ..pyrf.ts_vec_xyz import ts_vec_xyz
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def _calc_angle(look_, vec):
     vec_hat = normalize(vec)
     theta_ = np.rad2deg(
         np.pi - np.arccos(np.sum(vec_hat.data * look_.data, axis=1)),
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/eis_pad_combine_sc.py` & `pyrfu-2.4.3/pyrfu/mms/eis_pad_combine_sc.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def eis_pad_combine_sc(pads):
     r"""Generate composite Pitch Angle Distributions (PAD) from the EIS
     sensors across the MMS spacecraft.
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/eis_pad_spinavg.py` & `pyrfu-2.4.3/pyrfu/mms/eis_pad_spinavg.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def eis_pad_spinavg(inp, spin_nums):
     r"""Calculates spin-averaged Pitch-Angle Distribution (PAD) for the EIS
     instrument.
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/eis_proton_correction.py` & `pyrfu-2.4.3/pyrfu/mms/eis_proton_correction.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def _phxtof_calibration(energy, alpha, beta, gamma):
     r"""Pulse Height x Time Of Flight correction model from EPD Data Product
     Guide"""
     return 1 / (0.5 * (1 + alpha * (np.tanh((energy - beta) / gamma) + 1)))
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/eis_skymap.py` & `pyrfu-2.4.3/pyrfu/mms/eis_skymap.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from ..pyrf.ts_skymap import ts_skymap
 
 # Local imports
 from .dpf2psd import dpf2psd
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def eis_skymap(inp_ang_ang, to_psd: bool = True):
     r"""Construct skymap distribution from angle-angle distribution.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/eis_skymap_combine_sc.py` & `pyrfu-2.4.3/pyrfu/mms/eis_skymap_combine_sc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# 3rd party imports
-import numpy as np
-
-from ..pyrf.ts_skymap import ts_skymap
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.7"
-__status__ = "Prototype"
-
-
-def _idx_closest(lst0, lst1):
-    return [(np.abs(np.asarray(lst0) - k)).argmin() for k in lst1]
-
-
-def _combine_attrs(skymaps_attrs):
-    attrs = {}
-    filtered_attrs = [
-        "delta_energy_plus",
-        "delta_energy_minus",
-        "esteptable",
-        "energy0",
-        "energy1",
-    ]
-
-    attrs_keys = list(
-        filter(lambda k: k not in filtered_attrs, skymaps_attrs[0]),
-    )
-
-    for k in attrs_keys:
-        sms_attrs = [skymaps_attr[k] for skymaps_attr in skymaps_attrs]
-
-        is_same = [sms_attr == sms_attrs[0] for sms_attr in sms_attrs[1:]]
-
-        try:
-            if all(is_same):
-                attrs[k] = sms_attrs[0]
-            else:
-                continue
-        except ValueError:
-            continue
-
-    return attrs
-
-
-def eis_skymap_combine_sc(skymaps, method: str = "mean"):
-    r"""Generate composite skymap from the EIS sensors across the MMS
-    spacecraft.
-
-    Parameters
-    ----------
-    skymaps : list of xarray.Dataset
-        Skymap distribution for all spacecraft.
-    method : str, Optional
-        Method to combine spectra, "mean" or "sum"
-
-    Returns
-    -------
-    out : xarray.Dataset
-        Composite skymap distribution
-
-    See Also
-    --------
-    pyrfu.mms.get_eis_allt, pyrfu.mms.eis_pad,
-    pyrfu.mms.eis_spec_combine_sc, pyrfu.mms.eis_spec_combine_sc
-
-    """
-    assert method.lower() in ["mean", "sum"]
-
-    # Determine spacecraft with smallest number of time steps to use as
-    # reference spacecraft
-    time_size = [len(probe.time.data) for probe in skymaps]
-    ref_sc_time_size, ref_sc_loc = [np.min(time_size), np.argmin(time_size)]
-    ref_probe = skymaps[ref_sc_loc]
-
-    # Define common energy grid across EIS instruments
-    n_en_chans = [probe.energy.shape[1] for probe in skymaps]
-    size_en, loc_ref_en = [np.min(n_en_chans), np.argmin(n_en_chans)]
-    ref_energy = skymaps[loc_ref_en].energy.data[0, :]
-
-    energy_data, e_plus, e_minu = [[], [], []]
-    for probe in skymaps:
-        idx = _idx_closest(probe.energy.data[0, :], ref_energy)
-        energy_data.append(probe.energy.data[0, idx])
-        e_minu.append(probe.attrs["delta_energy_minus"][idx])
-        e_plus.append(probe.attrs["delta_energy_plus"][idx])
-
-    energy_data = np.stack(energy_data)
-    common_energy = np.nanmean(energy_data, axis=0)
-    common_energy = np.tile(common_energy, (ref_sc_time_size, 1))
-
-    #
-    e_minu = np.stack(e_minu)
-    e_plus = np.stack(e_plus)
-    common_minu = np.nanmean(e_minu, axis=0)
-    common_plus = np.nanmean(e_plus, axis=0)
-
-    # Use azimuthal and elevation angle from reference spacecraft (in
-    # practice they are the same for all spacecraft)
-    phi = ref_probe.phi.data
-    theta = ref_probe.theta.data
-
-    allmms_skymap = np.zeros(
-        [ref_sc_time_size, size_en, phi.shape[1], len(theta), len(skymaps)],
-    )
-
-    for i_s, skymap in enumerate(skymaps):
-        idx_en = _idx_closest(skymap.energy.data[0, :], common_energy[0, :])
-        allmms_skymap[..., i_s] = skymap.data[:ref_sc_time_size, idx_en, ...]
-
-    if method.lower() == "mean":
-        # Average the four spacecraft
-        allmms_skymap_avg = np.nanmean(allmms_skymap, axis=-1)
-    else:
-        # Sum the four spacecraft
-        allmms_skymap_avg = np.nansum(allmms_skymap, axis=-1)
-
-    # Combine attributes
-    # Combine global attributes
-    glob_attrs = _combine_attrs([s.attrs for s in skymaps])
-    glob_attrs = {
-        "delta_energy_plus": np.tile(common_plus, (ref_sc_time_size)),
-        "delta_energy_minus": np.tile(common_minu, (ref_sc_time_size)),
-        **glob_attrs,
-    }
-
-    # Combine coordinates attributes
-    coords_attrs = {}
-    for coor in ["time", "energy", "phi", "theta"]:
-        coords_attrs[coor] = _combine_attrs(
-            [skymap[coor].attrs for skymap in skymaps],
-        )
-
-    # Combine data attributes
-    attrs = _combine_attrs([skymap.data.attrs for skymap in skymaps])
-
-    # Create combined skymap
-    out = ts_skymap(
-        ref_probe.time.data,
-        allmms_skymap_avg,
-        common_energy,
-        phi,
-        theta,
-        energy0=common_energy[0, :],
-        energy1=common_energy[1, :],
-        esteptable=np.zeros(len(ref_probe.time.data)),
-        attrs=attrs,
-        coords_attrs=coords_attrs,
-        glob_attrs=glob_attrs,
-    )
-
-    return out
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# 3rd party imports
+import numpy as np
+
+from ..pyrf.ts_skymap import ts_skymap
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def _idx_closest(lst0, lst1):
+    return [(np.abs(np.asarray(lst0) - k)).argmin() for k in lst1]
+
+
+def _combine_attrs(skymaps_attrs):
+    attrs = {}
+    filtered_attrs = [
+        "delta_energy_plus",
+        "delta_energy_minus",
+        "esteptable",
+        "energy0",
+        "energy1",
+    ]
+
+    attrs_keys = list(
+        filter(lambda k: k not in filtered_attrs, skymaps_attrs[0]),
+    )
+
+    for k in attrs_keys:
+        sms_attrs = [skymaps_attr[k] for skymaps_attr in skymaps_attrs]
+
+        is_same = [sms_attr == sms_attrs[0] for sms_attr in sms_attrs[1:]]
+
+        try:
+            if all(is_same):
+                attrs[k] = sms_attrs[0]
+            else:
+                continue
+        except ValueError:
+            continue
+
+    return attrs
+
+
+def eis_skymap_combine_sc(skymaps, method: str = "mean"):
+    r"""Generate composite skymap from the EIS sensors across the MMS
+    spacecraft.
+
+    Parameters
+    ----------
+    skymaps : list of xarray.Dataset
+        Skymap distribution for all spacecraft.
+    method : str, Optional
+        Method to combine spectra, "mean" or "sum"
+
+    Returns
+    -------
+    out : xarray.Dataset
+        Composite skymap distribution
+
+    See Also
+    --------
+    pyrfu.mms.get_eis_allt, pyrfu.mms.eis_pad,
+    pyrfu.mms.eis_spec_combine_sc, pyrfu.mms.eis_spec_combine_sc
+
+    """
+    assert method.lower() in ["mean", "sum"]
+
+    # Determine spacecraft with smallest number of time steps to use as
+    # reference spacecraft
+    time_size = [len(probe.time.data) for probe in skymaps]
+    ref_sc_time_size, ref_sc_loc = [np.min(time_size), np.argmin(time_size)]
+    ref_probe = skymaps[ref_sc_loc]
+
+    # Define common energy grid across EIS instruments
+    n_en_chans = [probe.energy.shape[1] for probe in skymaps]
+    size_en, loc_ref_en = [np.min(n_en_chans), np.argmin(n_en_chans)]
+    ref_energy = skymaps[loc_ref_en].energy.data[0, :]
+
+    energy_data, e_plus, e_minu = [[], [], []]
+    for probe in skymaps:
+        idx = _idx_closest(probe.energy.data[0, :], ref_energy)
+        energy_data.append(probe.energy.data[0, idx])
+        e_minu.append(probe.attrs["delta_energy_minus"][idx])
+        e_plus.append(probe.attrs["delta_energy_plus"][idx])
+
+    energy_data = np.stack(energy_data)
+    common_energy = np.nanmean(energy_data, axis=0)
+    common_energy = np.tile(common_energy, (ref_sc_time_size, 1))
+
+    #
+    e_minu = np.stack(e_minu)
+    e_plus = np.stack(e_plus)
+    common_minu = np.nanmean(e_minu, axis=0)
+    common_plus = np.nanmean(e_plus, axis=0)
+
+    # Use azimuthal and elevation angle from reference spacecraft (in
+    # practice they are the same for all spacecraft)
+    phi = ref_probe.phi.data
+    theta = ref_probe.theta.data
+
+    allmms_skymap = np.zeros(
+        [ref_sc_time_size, size_en, phi.shape[1], len(theta), len(skymaps)],
+    )
+
+    for i_s, skymap in enumerate(skymaps):
+        idx_en = _idx_closest(skymap.energy.data[0, :], common_energy[0, :])
+        allmms_skymap[..., i_s] = skymap.data[:ref_sc_time_size, idx_en, ...]
+
+    if method.lower() == "mean":
+        # Average the four spacecraft
+        allmms_skymap_avg = np.nanmean(allmms_skymap, axis=-1)
+    else:
+        # Sum the four spacecraft
+        allmms_skymap_avg = np.nansum(allmms_skymap, axis=-1)
+
+    # Combine attributes
+    # Combine global attributes
+    glob_attrs = _combine_attrs([s.attrs for s in skymaps])
+    glob_attrs = {
+        "delta_energy_plus": np.tile(common_plus, (ref_sc_time_size)),
+        "delta_energy_minus": np.tile(common_minu, (ref_sc_time_size)),
+        **glob_attrs,
+    }
+
+    # Combine coordinates attributes
+    coords_attrs = {}
+    for coor in ["time", "energy", "phi", "theta"]:
+        coords_attrs[coor] = _combine_attrs(
+            [skymap[coor].attrs for skymap in skymaps],
+        )
+
+    # Combine data attributes
+    attrs = _combine_attrs([skymap.data.attrs for skymap in skymaps])
+
+    # Create combined skymap
+    out = ts_skymap(
+        ref_probe.time.data,
+        allmms_skymap_avg,
+        common_energy,
+        phi,
+        theta,
+        energy0=common_energy[0, :],
+        energy1=common_energy[1, :],
+        esteptable=np.zeros(len(ref_probe.time.data)),
+        attrs=attrs,
+        coords_attrs=coords_attrs,
+        glob_attrs=glob_attrs,
+    )
+
+    return out
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/eis_spec_combine_sc.py` & `pyrfu-2.4.3/pyrfu/mms/eis_spec_combine_sc.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def _idx_closest(lst0, lst1):
     return [(np.abs(np.asarray(lst0) - k)).argmin() for k in lst1]
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/eis_spin_avg.py` & `pyrfu-2.4.3/pyrfu/mms/eis_spin_avg.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def _check_spin(spin):
     _, spin_inds = np.unique(spin, return_index=True)
 
     len_spin = np.max(np.diff(spin_inds))
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/estimate_phase_speed.py` & `pyrfu-2.4.3/pyrfu/mms/estimate_phase_speed.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # 3rd party imports
 import numpy as np
 from scipy.optimize import curve_fit
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def estimate_phase_speed(f_k_power, freq, k, f_min: float = 100.0):
     r"""Simple function to estimate the phase speed from the frequency
     wave number power spectrum. Fits :math:`f = v k/ 2 \\pi` to the
     power spectrum.
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/feeps_active_eyes.py` & `pyrfu-2.4.3/pyrfu/mms/feeps_active_eyes.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def feeps_active_eyes(var, tint, mms_id):
     r"""This function returns the FEEPS active eyes,
     based on date/mms_id/species/rate.
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/feeps_bad_data.json` & `pyrfu-2.4.3/pyrfu/mms/feeps_bad_data.json`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/pyrfu/mms/feeps_correct_energies.py` & `pyrfu-2.4.3/pyrfu/mms/feeps_correct_energies.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# 3rd party imports
-import xarray as xr
-
-# Local imports
-from .feeps_energy_table import feeps_energy_table
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.7"
-__status__ = "Prototype"
-
-
-def feeps_correct_energies(feeps_alle):
-    r"""Modifies the energy table in FEEPS spectra (intensity, count_rate,
-    counts) using the function: mms_feeps_energy_table (which is s/c, sensor
-    head and sensor ID dependent)
-
-    Parameters
-    ----------
-    feeps_alle : xarray.Dataset
-        Dataset containing the energy spectrum of the available eyes of the
-        Fly's Eye Energetic Particle Spectrometer (FEEPS).
-
-    Returns
-    -------
-    out : xarray.Dataset
-        Dataset containing the energy spectrum of the available eyes of the
-        Fly's Eye Energetic Particle Spectrometer (FEEPS) with corrected
-        energy table.
-
-    """
-
-    mms_id = feeps_alle.attrs["mmsId"]
-
-    sensors_eyes = list(filter(lambda x: x[:3] in ["top", "bot"], feeps_alle))
-
-    out_dict = {k: feeps_alle[k] for k in feeps_alle if k not in sensors_eyes}
-
-    for sensors_eye in sensors_eyes:
-        sensor, eye = sensors_eye.split("-")
-
-        new_energy = feeps_energy_table(mms_id, sensor, int(eye))
-
-        dim = feeps_alle[sensors_eye].dims[1]
-        out_dict[sensors_eye] = feeps_alle[sensors_eye].assign_coords(
-            {dim: new_energy},
-        )
-        out_dict[sensors_eye] = out_dict[sensors_eye].rename(
-            {"time": "time", dim: f"energy-{sensors_eye}"},
-        )
-
-    out = xr.Dataset(out_dict)
-    out.attrs = feeps_alle.attrs
-
-    return out
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# 3rd party imports
+import xarray as xr
+
+# Local imports
+from .feeps_energy_table import feeps_energy_table
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def feeps_correct_energies(feeps_alle):
+    r"""Modifies the energy table in FEEPS spectra (intensity, count_rate,
+    counts) using the function: mms_feeps_energy_table (which is s/c, sensor
+    head and sensor ID dependent)
+
+    Parameters
+    ----------
+    feeps_alle : xarray.Dataset
+        Dataset containing the energy spectrum of the available eyes of the
+        Fly's Eye Energetic Particle Spectrometer (FEEPS).
+
+    Returns
+    -------
+    out : xarray.Dataset
+        Dataset containing the energy spectrum of the available eyes of the
+        Fly's Eye Energetic Particle Spectrometer (FEEPS) with corrected
+        energy table.
+
+    """
+
+    mms_id = feeps_alle.attrs["mmsId"]
+
+    sensors_eyes = list(filter(lambda x: x[:3] in ["top", "bot"], feeps_alle))
+
+    out_dict = {k: feeps_alle[k] for k in feeps_alle if k not in sensors_eyes}
+
+    for sensors_eye in sensors_eyes:
+        sensor, eye = sensors_eye.split("-")
+
+        new_energy = feeps_energy_table(mms_id, sensor, int(eye))
+
+        dim = feeps_alle[sensors_eye].dims[1]
+        out_dict[sensors_eye] = feeps_alle[sensors_eye].assign_coords(
+            {dim: new_energy},
+        )
+        out_dict[sensors_eye] = out_dict[sensors_eye].rename(
+            {"time": "time", dim: f"energy-{sensors_eye}"},
+        )
+
+    out = xr.Dataset(out_dict)
+    out.attrs = feeps_alle.attrs
+
+    return out
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/feeps_energy_table.py` & `pyrfu-2.4.3/pyrfu/mms/feeps_energy_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 table = {
     "mms1-top": [
         14.0,
         7.0,
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/feeps_flat_field_corrections.py` & `pyrfu-2.4.3/pyrfu/mms/feeps_flat_field_corrections.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 g_corr = {
     "mms1-top6": 0.7,
     "mms1-top7": 2.5,
     "mms1-top8": 1.5,
     "mms1-bot5": 1.2,
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/feeps_omni.py` & `pyrfu-2.4.3/pyrfu/mms/feeps_omni.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 energies_ = {
     "electron": np.array(
         [
             33.2,
             51.90,
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/feeps_pad.py` & `pyrfu-2.4.3/pyrfu/mms/feeps_pad.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 from .feeps_active_eyes import feeps_active_eyes
 
 # Local imports
 from .feeps_pitch_angles import feeps_pitch_angles
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 # Angular response (finite field of view) of instruments electrons can use
 # +/- 21.4 deg on each pitch angle as average response angle; ions can start
 # with +/-10 deg, but both need to be further refined
 angular_repsonse = {"electron": 21.4, "ion": 10}
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/feeps_pad_spinavg.py` & `pyrfu-2.4.3/pyrfu/mms/feeps_pad_spinavg.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 # #rd party imports
 import numpy as np
 import xarray as xr
 from scipy import interpolate
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def feeps_pad_spinavg(pad, spin_sectors, bin_size: float = 16.3636):
     r"""Spin-average the FEEPS pitch angle distributions.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/feeps_pitch_angles.py` & `pyrfu-2.4.3/pyrfu/mms/feeps_pitch_angles.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from ..pyrf.resample import resample
 
 # Local imports
 from .feeps_active_eyes import feeps_active_eyes
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 # Rotation matrices for FEEPS coord system (FCS) into body coordinate system
 # (BCS):
 t_top = np.array(
     [
         [1.0 / np.sqrt(2.0), -1.0 / np.sqrt(2.0), 0],
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/feeps_remove_bad_data.py` & `pyrfu-2.4.3/pyrfu/mms/feeps_remove_bad_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 # Local imports
 from ..pyrf.datetime642iso8601 import datetime642iso8601
 from ..pyrf.iso86012datetime import iso86012datetime
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def _bad_vars(bad_data):
     bad_vars_top = list(filter(lambda x: x not in [6, 7, 8], bad_data["top"]))
     bad_vars_bot = list(
         filter(lambda x: x not in [6, 7, 8], bad_data["bottom"]),
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/feeps_remove_sun.py` & `pyrfu-2.4.3/pyrfu/mms/feeps_remove_sun.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import xarray as xr
 
 # Local imports
 from .read_feeps_sector_masks_csv import read_feeps_sector_masks_csv
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def feeps_remove_sun(inp_dataset):
     r"""Removes the sunlight contamination from FEEPS data.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/feeps_sector_spec.py` & `pyrfu-2.4.3/pyrfu/mms/feeps_sector_spec.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def feeps_sector_spec(inp_alle):
     r"""Creates sector-spectrograms with FEEPS data (particle data organized
     by time and sector number)
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/feeps_spin_avg.py` & `pyrfu-2.4.3/pyrfu/mms/feeps_spin_avg.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def feeps_spin_avg(flux_omni, spin_sectors):
     r"""spin-average the omni-directional FEEPS energy spectra
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/feeps_split_integral_ch.py` & `pyrfu-2.4.3/pyrfu/mms/feeps_split_integral_ch.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def feeps_split_integral_ch(inp_dataset):
     r"""This function splits the last integral channel from the FEEPS spectra,
     creating 2 new DataArrays
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/fft_bandpass.py` & `pyrfu-2.4.3/pyrfu/mms/fft_bandpass.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 # Local imports
 from ..pyrf.calc_fs import calc_fs
 from ..pyrf.ts_scalar import ts_scalar
 from ..pyrf.ts_vec_xyz import ts_vec_xyz
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def fft_bandpass(inp, f_min, f_max):
     r"""Perform simple bandpass using FFT - returns fields between with
     ``f_min`` < f < ``f_max``.
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/fk_power_spectrum_4sc.py` & `pyrfu-2.4.3/pyrfu/mms/fk_power_spectrum_4sc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,361 +1,361 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Built-in imports
-import bisect
-import logging
-
-# 3rd party imports
-import numpy as np
-import xarray as xr
-
-# Local imports
-from ..pyrf.avg_4sc import avg_4sc
-from ..pyrf.resample import resample
-from ..pyrf.time_clip import time_clip
-from ..pyrf.wavelet import wavelet
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2022"
-__license__ = "MIT"
-__version__ = "2.3.22"
-__status__ = "Prototype"
-
-logging.captureWarnings(True)
-logging.basicConfig(
-    format="[%(asctime)s] %(levelname)s: %(message)s",
-    datefmt="%d-%b-%y %H:%M:%S",
-    level=logging.INFO,
-)
-
-
-def fk_power_spectrum_4sc(
-    e,
-    r,
-    b,
-    tints,
-    cav: int = 8,
-    num_k: int = 500,
-    num_f: int = 200,
-    df: float = None,
-    w_width: int = 1,
-    f_range: list = None,
-):
-    r"""Calculates the frequency-wave number power spectrum using the four
-    MMS spacecraft. Uses a generalization of mms.fk_powerspectrum. Wavelet
-    based cross-spectral analysis is used to calculate the phase difference
-    each spacecraft pair and determine 3D wave vector. A generalization of
-    the method used in mms.fk_powerspectrum to four point measurements.
-
-    Parameters
-    ----------
-    e : list of xarray.DataArray
-        Fields to apply 4SC cross-spectral analysis to. e.g., e or b fields
-        (if multiple components only the first is used).
-    r : list of xarray.DataArray
-        Positions of the four spacecraft.
-    b : list of xarray.DataArray
-        background magnetic field in the same coordinates as r. Used to
-        determine the parallel and perpendicular wave numbers using 4SC
-        average.
-    tints : list of str
-        Time interval over which the power spectrum is calculated. To avoid
-        boundary effects use a longer time interval for e and b.
-    cav : int, Optional
-        Number of points in time series used to estimate phase.
-        Default ``cav`` = 8.
-    num_k : int, Optional
-        Number of wave numbers used in spectrogram. Default ``num_k`` = 500.
-    df : float, Optional
-        Linear spacing of frequencies. Default ``df`` = None (log spacing).
-    num_f : int, Optional
-        Number of frequencies used in spectrogram. Default ``num_f`` = 200.
-    w_width : float, Optional
-        Multiplier for Morlet wavelet width. Default ``w_width`` = 1.
-    f_range : list of float, Optional
-        Frequency range for k-k plots. [minf maxf].
-
-    Returns
-    -------
-    out : xarray.Dataset
-        Dataset of array of powers as a function of frequency and
-        wavenumber. Power is normalized to the maximum value.
-
-    Notes
-    -----
-    Wavelength must be larger than twice the spacecraft separations,
-    otherwise spatial aliasing will occur.
-
-    Examples
-    --------
-    >>> from pyrfu.mms import get_data, fk_power_spectrum_4sc
-    >>> from pyrfu.pyrf import extend_tint, convert_fac
-
-    Load data
-
-    >>> tint = ["2015-10-16T13:05:24.00", "2015-10-16T13:05:50.000"]
-    >>> ic = range(1, 5)
-    >>> b_fgm = [get_data("b_gse_fgm_brst_l2", tint, i) for i in ic]
-    >>> b_scm = [get_data("b_gse_scm_brst_l2", tint, i) for i in ic]
-
-    Load spacecraft position
-
-    >>> tint_long = extend_tint(tint, [-60, 60])
-    >>> r_gse_mms = [get_data("r_gse", tint_long, i) for i in range(1, 5)]
-
-    Convert magnetic field fluctuations to field aligned coordinates
-
-    >>> b_fac = [convert_fac(b_s, b_f) for b_s, b_f in zip(b_scm, b_fgm)]
-    >>> b_par = [b_s[:, 0] for b_s in b_fac]
-
-    Compute dispersion relation
-
-    >>> tint = ["2015-10-16T13:05:26.500", "2015-10-16T13:05:27.000"]
-    >>> pwer = fk_power_spectrum_4sc(b_par, r_gse, b_fgm, tint, 4, 500, 2,
-    ... 10, 2)
-
-    """
-
-    ic = np.arange(1, 5)
-
-    e = [resample(e[i - 1], e[0]) for i in ic]
-    r = [resample(r[i - 1], e[0]) for i in ic]
-    b = [resample(b[i - 1], e[0]) for i in ic]
-
-    b_avg = avg_4sc(b)
-
-    times = e[0].time
-    use_linear = df is not None
-
-    idx = time_clip(e[0].time, list(tints))
-
-    # If odd, remove last data point (as is done in irf_wavelet)
-    if len(idx) % 2:
-        idx = idx[:-1]
-
-    if use_linear:
-        cwt_options = {
-            "linear": df,
-            "return_power": False,
-            "wavelet_width": 5.36 * w_width,
-            "cut_edge": False,
-        }
-    else:
-        cwt_options = {
-            "nf": num_f,
-            "return_power": False,
-            "wavelet_width": 5.36 * w_width,
-            "cut_edge": False,
-        }
-
-    w = [wavelet(e[i], **cwt_options) for i in range(4)]
-
-    num_f = len(w[0].frequency)
-
-    times = time_clip(times, tints)
-    nt = len(times)
-
-    w = [time_clip(w[i], tints) for i in range(4)]
-
-    fk_power = 0
-    for i in range(4):
-        fk_power += (w[i].data * np.conj(w[i].data) / 4).astype(np.float64)
-
-    n = int(np.floor(nt / cav) - 1)
-    pos_av = cav / 2 + np.arange(n + 1) * cav
-    av_times = times[pos_av.astype(np.int64)]
-
-    b_avg = resample(b_avg, av_times)
-
-    r = [resample(r[i], av_times) for i in range(4)]
-
-    cx12, cx13, cx14 = [np.zeros((n + 1, num_f), dtype="complex128") for _ in range(3)]
-    cx23, cx24, cx34 = [np.zeros((n + 1, num_f), dtype="complex128") for _ in range(3)]
-
-    power_avg = np.zeros((n + 1, num_f), dtype="complex128")
-
-    for m, pos_avm in enumerate(pos_av):
-        lb, ub = [int(pos_avm - cav / 2), int(pos_avm + cav / 2)]
-
-        cx12[m, :] = np.nanmean(
-            w[0].data[lb:ub, :] * np.conj(w[1].data[lb:ub, :]),
-            axis=0,
-        )
-        cx13[m, :] = np.nanmean(
-            w[0].data[lb:ub, :] * np.conj(w[2].data[lb:ub, :]),
-            axis=0,
-        )
-        cx14[m, :] = np.nanmean(
-            w[0].data[lb:ub, :] * np.conj(w[3].data[lb:ub, :]),
-            axis=0,
-        )
-        cx23[m, :] = np.nanmean(
-            w[1].data[lb:ub, :] * np.conj(w[2].data[lb:ub, :]),
-            axis=0,
-        )
-        cx24[m, :] = np.nanmean(
-            w[1].data[lb:ub, :] * np.conj(w[3].data[lb:ub, :]),
-            axis=0,
-        )
-        cx34[m, :] = np.nanmean(
-            w[2].data[lb:ub, :] * np.conj(w[3].data[lb:ub, :]),
-            axis=0,
-        )
-
-        power_avg[m, :] = np.nanmean(fk_power[lb:ub, :], axis=0)
-
-    # Compute phase differences between each spacecraft pair
-    th12 = np.arctan2(np.imag(cx12), np.real(cx12))
-    th13 = np.arctan2(np.imag(cx13), np.real(cx13))
-    th14 = np.arctan2(np.imag(cx14), np.real(cx14))
-    th23 = np.arctan2(np.imag(cx23), np.real(cx23))
-    th24 = np.arctan2(np.imag(cx24), np.real(cx24))
-    th34 = np.arctan2(np.imag(cx34), np.real(cx34))
-
-    w_mat = 2 * np.pi * np.tile(w[0].frequency.data, (n + 1, 1))
-
-    # Convert phase difference to time delay
-    dt12, dt13, dt14, dt23, dt24, dt34 = [
-        th / w_mat for th in [th12, th13, th14, th23, th24, th34]
-    ]
-
-    # Weighted averaged time delay using all spacecraft pairs
-    dt2 = (
-        0.5 * dt12
-        + 0.2 * (dt13 - dt23)
-        + 0.2 * (dt14 - dt24)
-        + 0.1 * (dt14 - dt34 - dt23)
-    )
-    dt3 = (
-        0.5 * dt13
-        + 0.2 * (dt12 + dt23)
-        + 0.2 * (dt14 - dt34)
-        + 0.1 * (dt12 + dt24 - dt34)
-    )
-    dt4 = (
-        0.5 * dt14
-        + 0.2 * (dt12 + dt24)
-        + 0.2 * (dt13 + dt34)
-        + 0.1 * (dt12 + dt23 + dt34)
-    )
-
-    # Compute phase speeds
-    r = [r[i].data for i in range(4)]
-
-    k_x, k_y, k_z = [np.zeros((n + 1, num_f)) for _ in range(3)]
-
-    for ii in range(n + 1):
-        dr = np.array(
-            [
-                r[1][ii, :] - r[0][ii, :],
-                r[2][ii, :] - r[0][ii, :],
-                r[3][ii, :] - r[0][ii, :],
-            ],
-        )
-        for jj in range(num_f):
-            m = np.linalg.solve(dr, [dt2[ii, jj], dt3[ii, jj], dt4[ii, jj]])
-            k_x[ii, jj] = 2 * np.pi * w[0].frequency[jj].data * m[0]
-            k_y[ii, jj] = 2 * np.pi * w[0].frequency[jj].data * m[1]
-            k_z[ii, jj] = 2 * np.pi * w[0].frequency[jj].data * m[2]
-
-    k_x, k_y, k_z = [k / 1e3 for k in [k_x, k_y, k_z]]
-
-    k_mag = np.linalg.norm(np.array([k_x, k_y, k_z]), axis=0)
-
-    b_avg_x_mat = np.tile(b_avg.data[:, 0], (num_f, 1)).T
-    b_avg_y_mat = np.tile(b_avg.data[:, 1], (num_f, 1)).T
-    b_avg_z_mat = np.tile(b_avg.data[:, 2], (num_f, 1)).T
-
-    b_avg_abs = np.linalg.norm(b_avg, axis=1)
-    b_avg_abs_mat = np.tile(b_avg_abs, (num_f, 1)).T
-
-    k_par = (k_x * b_avg_x_mat + k_y * b_avg_y_mat + k_z * b_avg_z_mat) / b_avg_abs_mat
-    k_perp = np.sqrt(k_mag**2 - k_par**2)
-
-    k_max = np.max(k_mag) * 1.1
-    k_min = -k_max
-    k_vec = np.linspace(-k_max, k_max, num_k)
-    k_mag_vec = np.linspace(0, k_max, num_k)
-
-    dk_mag = k_max / num_k
-    dk = 2 * k_max / num_k
-
-    # Sort power into frequency and wave vector
-    logging.info("Computing power versus kx,f; ky,f, kz,f")
-    power_k_x_f, power_k_y_f, power_k_z_f = [np.zeros((num_f, num_k)) for _ in range(3)]
-    power_k_mag_f = np.zeros((num_f, num_k))
-
-    for nn in range(num_f):
-        k_x_number = np.floor((k_x[:, nn] - k_min) / dk).astype(np.int64)
-        k_y_number = np.floor((k_y[:, nn] - k_min) / dk).astype(np.int64)
-        k_z_number = np.floor((k_z[:, nn] - k_min) / dk).astype(np.int64)
-        k_number = np.floor((k_mag[:, nn]) / dk_mag).astype(np.int64)
-
-        power_k_x_f[nn, k_x_number] += np.real(power_avg[:, nn])
-        power_k_y_f[nn, k_y_number] += np.real(power_avg[:, nn])
-        power_k_z_f[nn, k_z_number] += np.real(power_avg[:, nn])
-
-        power_k_mag_f[nn, k_number] += np.real(power_avg[:, nn])
-
-    power_k_x_f /= np.max(power_k_x_f)
-    power_k_y_f /= np.max(power_k_y_f)
-    power_k_z_f /= np.max(power_k_z_f)
-    power_k_mag_f /= np.max(power_k_mag_f)
-
-    frequencies = w[0].frequency.data
-    idx_f = np.arange(num_f)
-
-    if f_range is not None:
-        idx_min_freq = bisect.bisect_left(frequencies, np.min(f_range))
-        idx_max_freq = bisect.bisect_left(frequencies, np.max(f_range))
-        idx_f = idx_f[idx_min_freq:idx_max_freq]
-
-    logging.info("Computing power versus kx,ky; kx,kz; ky,kz")
-    power_k_x_k_y = np.zeros((num_k, num_k))
-    power_k_x_k_z = np.zeros((num_k, num_k))
-    power_k_y_k_z = np.zeros((num_k, num_k))
-    power_k_perp_k_par = np.zeros((num_k, num_k))
-
-    for nn in idx_f:
-        k_x_number = np.floor((k_x[:, nn] - k_min) / dk).astype(np.int64)
-        k_y_number = np.floor((k_y[:, nn] - k_min) / dk).astype(np.int64)
-        k_z_number = np.floor((k_z[:, nn] - k_min) / dk).astype(np.int64)
-
-        k_par_number = np.floor((k_par[:, nn] - k_min) / dk).astype(np.int64)
-        k_perp_number = np.floor((k_perp[:, nn]) / dk_mag).astype(np.int64)
-
-        power_k_x_k_y[k_y_number, k_x_number] += np.real(power_avg[:, nn])
-        power_k_x_k_z[k_z_number, k_x_number] += np.real(power_avg[:, nn])
-        power_k_y_k_z[k_z_number, k_y_number] += np.real(power_avg[:, nn])
-
-        power_k_perp_k_par[k_par_number, k_perp_number] += np.real(
-            power_avg[:, nn],
-        )
-
-    power_k_x_k_y /= np.max(power_k_x_k_y)
-    power_k_x_k_z /= np.max(power_k_x_k_z)
-    power_k_y_k_z /= np.max(power_k_y_k_z)
-    power_k_perp_k_par /= np.max(power_k_perp_k_par)
-
-    out_dict = {
-        "k_x_f": (["k_x", "f"], power_k_x_f.T),
-        "k_y_f": (["k_x", "f"], power_k_y_f.T),
-        "k_z_f": (["k_x", "f"], power_k_z_f.T),
-        "k_mag_f": (["k_mag", "f"], power_k_mag_f.T),
-        "k_x_k_y": (["k_x", "k_y"], power_k_x_k_y.T),
-        "k_x_k_z": (["kx", "kz"], power_k_x_k_z.T),
-        "k_y_k_z": (["k_y", "k_z"], power_k_y_k_z.T),
-        "k_perp_k_par": (["k_perp", "k_par"], power_k_perp_k_par.T),
-        "k_x": k_vec,
-        "k_y": k_vec,
-        "k_z": k_vec,
-        "k_mag": k_mag_vec,
-        "k_perp": k_mag_vec,
-        "k_par": k_vec,
-        "f": frequencies,
-    }
-
-    out = xr.Dataset(out_dict)
-
-    return out
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# Built-in imports
+import bisect
+import logging
+
+# 3rd party imports
+import numpy as np
+import xarray as xr
+
+# Local imports
+from ..pyrf.avg_4sc import avg_4sc
+from ..pyrf.resample import resample
+from ..pyrf.time_clip import time_clip
+from ..pyrf.wavelet import wavelet
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+logging.captureWarnings(True)
+logging.basicConfig(
+    format="[%(asctime)s] %(levelname)s: %(message)s",
+    datefmt="%d-%b-%y %H:%M:%S",
+    level=logging.INFO,
+)
+
+
+def fk_power_spectrum_4sc(
+    e,
+    r,
+    b,
+    tints,
+    cav: int = 8,
+    num_k: int = 500,
+    num_f: int = 200,
+    df: float = None,
+    w_width: int = 1,
+    f_range: list = None,
+):
+    r"""Calculates the frequency-wave number power spectrum using the four
+    MMS spacecraft. Uses a generalization of mms.fk_powerspectrum. Wavelet
+    based cross-spectral analysis is used to calculate the phase difference
+    each spacecraft pair and determine 3D wave vector. A generalization of
+    the method used in mms.fk_powerspectrum to four point measurements.
+
+    Parameters
+    ----------
+    e : list of xarray.DataArray
+        Fields to apply 4SC cross-spectral analysis to. e.g., e or b fields
+        (if multiple components only the first is used).
+    r : list of xarray.DataArray
+        Positions of the four spacecraft.
+    b : list of xarray.DataArray
+        background magnetic field in the same coordinates as r. Used to
+        determine the parallel and perpendicular wave numbers using 4SC
+        average.
+    tints : list of str
+        Time interval over which the power spectrum is calculated. To avoid
+        boundary effects use a longer time interval for e and b.
+    cav : int, Optional
+        Number of points in time series used to estimate phase.
+        Default ``cav`` = 8.
+    num_k : int, Optional
+        Number of wave numbers used in spectrogram. Default ``num_k`` = 500.
+    df : float, Optional
+        Linear spacing of frequencies. Default ``df`` = None (log spacing).
+    num_f : int, Optional
+        Number of frequencies used in spectrogram. Default ``num_f`` = 200.
+    w_width : float, Optional
+        Multiplier for Morlet wavelet width. Default ``w_width`` = 1.
+    f_range : list of float, Optional
+        Frequency range for k-k plots. [minf maxf].
+
+    Returns
+    -------
+    out : xarray.Dataset
+        Dataset of array of powers as a function of frequency and
+        wavenumber. Power is normalized to the maximum value.
+
+    Notes
+    -----
+    Wavelength must be larger than twice the spacecraft separations,
+    otherwise spatial aliasing will occur.
+
+    Examples
+    --------
+    >>> from pyrfu.mms import get_data, fk_power_spectrum_4sc
+    >>> from pyrfu.pyrf import extend_tint, convert_fac
+
+    Load data
+
+    >>> tint = ["2015-10-16T13:05:24.00", "2015-10-16T13:05:50.000"]
+    >>> ic = range(1, 5)
+    >>> b_fgm = [get_data("b_gse_fgm_brst_l2", tint, i) for i in ic]
+    >>> b_scm = [get_data("b_gse_scm_brst_l2", tint, i) for i in ic]
+
+    Load spacecraft position
+
+    >>> tint_long = extend_tint(tint, [-60, 60])
+    >>> r_gse_mms = [get_data("r_gse", tint_long, i) for i in range(1, 5)]
+
+    Convert magnetic field fluctuations to field aligned coordinates
+
+    >>> b_fac = [convert_fac(b_s, b_f) for b_s, b_f in zip(b_scm, b_fgm)]
+    >>> b_par = [b_s[:, 0] for b_s in b_fac]
+
+    Compute dispersion relation
+
+    >>> tint = ["2015-10-16T13:05:26.500", "2015-10-16T13:05:27.000"]
+    >>> pwer = fk_power_spectrum_4sc(b_par, r_gse, b_fgm, tint, 4, 500, 2,
+    ... 10, 2)
+
+    """
+
+    ic = np.arange(1, 5)
+
+    e = [resample(e[i - 1], e[0]) for i in ic]
+    r = [resample(r[i - 1], e[0]) for i in ic]
+    b = [resample(b[i - 1], e[0]) for i in ic]
+
+    b_avg = avg_4sc(b)
+
+    times = e[0].time
+    use_linear = df is not None
+
+    idx = time_clip(e[0].time, list(tints))
+
+    # If odd, remove last data point (as is done in irf_wavelet)
+    if len(idx) % 2:
+        idx = idx[:-1]
+
+    if use_linear:
+        cwt_options = {
+            "linear": df,
+            "return_power": False,
+            "wavelet_width": 5.36 * w_width,
+            "cut_edge": False,
+        }
+    else:
+        cwt_options = {
+            "nf": num_f,
+            "return_power": False,
+            "wavelet_width": 5.36 * w_width,
+            "cut_edge": False,
+        }
+
+    w = [wavelet(e[i], **cwt_options) for i in range(4)]
+
+    num_f = len(w[0].frequency)
+
+    times = time_clip(times, tints)
+    nt = len(times)
+
+    w = [time_clip(w[i], tints) for i in range(4)]
+
+    fk_power = 0
+    for i in range(4):
+        fk_power += (w[i].data * np.conj(w[i].data) / 4).astype(np.float64)
+
+    n = int(np.floor(nt / cav) - 1)
+    pos_av = cav / 2 + np.arange(n + 1) * cav
+    av_times = times[pos_av.astype(np.int64)]
+
+    b_avg = resample(b_avg, av_times)
+
+    r = [resample(r[i], av_times) for i in range(4)]
+
+    cx12, cx13, cx14 = [np.zeros((n + 1, num_f), dtype="complex128") for _ in range(3)]
+    cx23, cx24, cx34 = [np.zeros((n + 1, num_f), dtype="complex128") for _ in range(3)]
+
+    power_avg = np.zeros((n + 1, num_f), dtype="complex128")
+
+    for m, pos_avm in enumerate(pos_av):
+        lb, ub = [int(pos_avm - cav / 2), int(pos_avm + cav / 2)]
+
+        cx12[m, :] = np.nanmean(
+            w[0].data[lb:ub, :] * np.conj(w[1].data[lb:ub, :]),
+            axis=0,
+        )
+        cx13[m, :] = np.nanmean(
+            w[0].data[lb:ub, :] * np.conj(w[2].data[lb:ub, :]),
+            axis=0,
+        )
+        cx14[m, :] = np.nanmean(
+            w[0].data[lb:ub, :] * np.conj(w[3].data[lb:ub, :]),
+            axis=0,
+        )
+        cx23[m, :] = np.nanmean(
+            w[1].data[lb:ub, :] * np.conj(w[2].data[lb:ub, :]),
+            axis=0,
+        )
+        cx24[m, :] = np.nanmean(
+            w[1].data[lb:ub, :] * np.conj(w[3].data[lb:ub, :]),
+            axis=0,
+        )
+        cx34[m, :] = np.nanmean(
+            w[2].data[lb:ub, :] * np.conj(w[3].data[lb:ub, :]),
+            axis=0,
+        )
+
+        power_avg[m, :] = np.nanmean(fk_power[lb:ub, :], axis=0)
+
+    # Compute phase differences between each spacecraft pair
+    th12 = np.arctan2(np.imag(cx12), np.real(cx12))
+    th13 = np.arctan2(np.imag(cx13), np.real(cx13))
+    th14 = np.arctan2(np.imag(cx14), np.real(cx14))
+    th23 = np.arctan2(np.imag(cx23), np.real(cx23))
+    th24 = np.arctan2(np.imag(cx24), np.real(cx24))
+    th34 = np.arctan2(np.imag(cx34), np.real(cx34))
+
+    w_mat = 2 * np.pi * np.tile(w[0].frequency.data, (n + 1, 1))
+
+    # Convert phase difference to time delay
+    dt12, dt13, dt14, dt23, dt24, dt34 = [
+        th / w_mat for th in [th12, th13, th14, th23, th24, th34]
+    ]
+
+    # Weighted averaged time delay using all spacecraft pairs
+    dt2 = (
+        0.5 * dt12
+        + 0.2 * (dt13 - dt23)
+        + 0.2 * (dt14 - dt24)
+        + 0.1 * (dt14 - dt34 - dt23)
+    )
+    dt3 = (
+        0.5 * dt13
+        + 0.2 * (dt12 + dt23)
+        + 0.2 * (dt14 - dt34)
+        + 0.1 * (dt12 + dt24 - dt34)
+    )
+    dt4 = (
+        0.5 * dt14
+        + 0.2 * (dt12 + dt24)
+        + 0.2 * (dt13 + dt34)
+        + 0.1 * (dt12 + dt23 + dt34)
+    )
+
+    # Compute phase speeds
+    r = [r[i].data for i in range(4)]
+
+    k_x, k_y, k_z = [np.zeros((n + 1, num_f)) for _ in range(3)]
+
+    for ii in range(n + 1):
+        dr = np.array(
+            [
+                r[1][ii, :] - r[0][ii, :],
+                r[2][ii, :] - r[0][ii, :],
+                r[3][ii, :] - r[0][ii, :],
+            ],
+        )
+        for jj in range(num_f):
+            m = np.linalg.solve(dr, [dt2[ii, jj], dt3[ii, jj], dt4[ii, jj]])
+            k_x[ii, jj] = 2 * np.pi * w[0].frequency[jj].data * m[0]
+            k_y[ii, jj] = 2 * np.pi * w[0].frequency[jj].data * m[1]
+            k_z[ii, jj] = 2 * np.pi * w[0].frequency[jj].data * m[2]
+
+    k_x, k_y, k_z = [k / 1e3 for k in [k_x, k_y, k_z]]
+
+    k_mag = np.linalg.norm(np.array([k_x, k_y, k_z]), axis=0)
+
+    b_avg_x_mat = np.tile(b_avg.data[:, 0], (num_f, 1)).T
+    b_avg_y_mat = np.tile(b_avg.data[:, 1], (num_f, 1)).T
+    b_avg_z_mat = np.tile(b_avg.data[:, 2], (num_f, 1)).T
+
+    b_avg_abs = np.linalg.norm(b_avg, axis=1)
+    b_avg_abs_mat = np.tile(b_avg_abs, (num_f, 1)).T
+
+    k_par = (k_x * b_avg_x_mat + k_y * b_avg_y_mat + k_z * b_avg_z_mat) / b_avg_abs_mat
+    k_perp = np.sqrt(k_mag**2 - k_par**2)
+
+    k_max = np.max(k_mag) * 1.1
+    k_min = -k_max
+    k_vec = np.linspace(-k_max, k_max, num_k)
+    k_mag_vec = np.linspace(0, k_max, num_k)
+
+    dk_mag = k_max / num_k
+    dk = 2 * k_max / num_k
+
+    # Sort power into frequency and wave vector
+    logging.info("Computing power versus kx,f; ky,f, kz,f")
+    power_k_x_f, power_k_y_f, power_k_z_f = [np.zeros((num_f, num_k)) for _ in range(3)]
+    power_k_mag_f = np.zeros((num_f, num_k))
+
+    for nn in range(num_f):
+        k_x_number = np.floor((k_x[:, nn] - k_min) / dk).astype(np.int64)
+        k_y_number = np.floor((k_y[:, nn] - k_min) / dk).astype(np.int64)
+        k_z_number = np.floor((k_z[:, nn] - k_min) / dk).astype(np.int64)
+        k_number = np.floor((k_mag[:, nn]) / dk_mag).astype(np.int64)
+
+        power_k_x_f[nn, k_x_number] += np.real(power_avg[:, nn])
+        power_k_y_f[nn, k_y_number] += np.real(power_avg[:, nn])
+        power_k_z_f[nn, k_z_number] += np.real(power_avg[:, nn])
+
+        power_k_mag_f[nn, k_number] += np.real(power_avg[:, nn])
+
+    power_k_x_f /= np.max(power_k_x_f)
+    power_k_y_f /= np.max(power_k_y_f)
+    power_k_z_f /= np.max(power_k_z_f)
+    power_k_mag_f /= np.max(power_k_mag_f)
+
+    frequencies = w[0].frequency.data
+    idx_f = np.arange(num_f)
+
+    if f_range is not None:
+        idx_min_freq = bisect.bisect_left(frequencies, np.min(f_range))
+        idx_max_freq = bisect.bisect_left(frequencies, np.max(f_range))
+        idx_f = idx_f[idx_min_freq:idx_max_freq]
+
+    logging.info("Computing power versus kx,ky; kx,kz; ky,kz")
+    power_k_x_k_y = np.zeros((num_k, num_k))
+    power_k_x_k_z = np.zeros((num_k, num_k))
+    power_k_y_k_z = np.zeros((num_k, num_k))
+    power_k_perp_k_par = np.zeros((num_k, num_k))
+
+    for nn in idx_f:
+        k_x_number = np.floor((k_x[:, nn] - k_min) / dk).astype(np.int64)
+        k_y_number = np.floor((k_y[:, nn] - k_min) / dk).astype(np.int64)
+        k_z_number = np.floor((k_z[:, nn] - k_min) / dk).astype(np.int64)
+
+        k_par_number = np.floor((k_par[:, nn] - k_min) / dk).astype(np.int64)
+        k_perp_number = np.floor((k_perp[:, nn]) / dk_mag).astype(np.int64)
+
+        power_k_x_k_y[k_y_number, k_x_number] += np.real(power_avg[:, nn])
+        power_k_x_k_z[k_z_number, k_x_number] += np.real(power_avg[:, nn])
+        power_k_y_k_z[k_z_number, k_y_number] += np.real(power_avg[:, nn])
+
+        power_k_perp_k_par[k_par_number, k_perp_number] += np.real(
+            power_avg[:, nn],
+        )
+
+    power_k_x_k_y /= np.max(power_k_x_k_y)
+    power_k_x_k_z /= np.max(power_k_x_k_z)
+    power_k_y_k_z /= np.max(power_k_y_k_z)
+    power_k_perp_k_par /= np.max(power_k_perp_k_par)
+
+    out_dict = {
+        "k_x_f": (["k_x", "f"], power_k_x_f.T),
+        "k_y_f": (["k_x", "f"], power_k_y_f.T),
+        "k_z_f": (["k_x", "f"], power_k_z_f.T),
+        "k_mag_f": (["k_mag", "f"], power_k_mag_f.T),
+        "k_x_k_y": (["k_x", "k_y"], power_k_x_k_y.T),
+        "k_x_k_z": (["kx", "kz"], power_k_x_k_z.T),
+        "k_y_k_z": (["k_y", "k_z"], power_k_y_k_z.T),
+        "k_perp_k_par": (["k_perp", "k_par"], power_k_perp_k_par.T),
+        "k_x": k_vec,
+        "k_y": k_vec,
+        "k_z": k_vec,
+        "k_mag": k_mag_vec,
+        "k_perp": k_mag_vec,
+        "k_par": k_vec,
+        "f": frequencies,
+    }
+
+    out = xr.Dataset(out_dict)
+
+    return out
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/get_data.py` & `pyrfu-2.4.3/pyrfu/mms/get_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 from .list_files import list_files
 
 # Local imports
 from .tokenize import tokenize
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 logging.captureWarnings(True)
 logging.basicConfig(
     format="[%(asctime)s] %(levelname)s: %(message)s",
     datefmt="%d-%b-%y %H:%M:%S",
     level=logging.INFO,
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/get_feeps_omni.py` & `pyrfu-2.4.3/pyrfu/mms/get_feeps_omni.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from .feeps_split_integral_ch import feeps_split_integral_ch
 
 # Local imports
 from .get_feeps_alleyes import get_feeps_alleyes
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def get_feeps_omni(
     tar_var,
     tint,
     mms_id,
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/get_hpca_dist.py` & `pyrfu-2.4.3/pyrfu/mms/get_hpca_dist.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 mass_and_charge = {
     "hydrogen+": [1.04535e-2, 1],
     "helium+": [4.18138e-2, 1],
     "helium++": [4.18138e-2, 2],
     "oxygen+": [0.167255, 1],
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/get_pitch_angle_dist.py` & `pyrfu-2.4.3/pyrfu/mms/get_pitch_angle_dist.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # Local imports
 from ..pyrf.normalize import normalize
 from ..pyrf.resample import resample
 from ..pyrf.time_clip import time_clip
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 logging.captureWarnings(True)
 logging.basicConfig(
     format="[%(asctime)s] %(levelname)s: %(message)s",
     datefmt="%d-%b-%y %H:%M:%S",
     level=logging.INFO,
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/get_ts.py` & `pyrfu-2.4.3/pyrfu/mms/get_ts.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,351 +1,351 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Built-in import
-import re
-import warnings
-
-# 3rd party imports
-import numpy as np
-import xarray as xr
-from cdflib import CDF, cdfepoch
-
-from ..pyrf.cdfepoch2datetime64 import cdfepoch2datetime64
-
-# Local imports
-from ..pyrf.datetime642iso8601 import datetime642iso8601
-from ..pyrf.extend_tint import extend_tint
-from ..pyrf.iso86012datetime64 import iso86012datetime64
-from ..pyrf.time_clip import time_clip
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2023"
-__license__ = "MIT"
-__version__ = "2.3.26"
-__status__ = "Prototype"
-
-
-def _shift_epochs(file, epoch):
-    r"""Shift times for particles."""
-
-    epoch_shifted = epoch["data"].copy()
-
-    try:
-        delta_minus_var = {
-            "data": file.varget(epoch["attrs"]["DELTA_MINUS_VAR"]),
-            "attrs": file.varget(epoch["attrs"]["DELTA_MINUS_VAR"]),
-        }
-        delta_plus_var = {
-            "data": file.varget(epoch["attrs"]["DELTA_PLUS_VAR"]),
-            "attrs": file.varget(epoch["attrs"]["DELTA_PLUS_VAR"]),
-        }
-
-        delta_vars = [delta_minus_var, delta_plus_var]
-        flags_vars = [1e3, 1e3]  # Time scaling conversion flags
-
-        for i, delta_var in enumerate(delta_vars):
-            if isinstance(delta_var["attrs"], dict) and "UNITS" in delta_var["attrs"]:
-                if delta_var["attrs"]["UNITS"].lower() == "s":
-                    flags_vars[i] = 1e3
-                elif delta_var["attrs"]["UNITS"].lower() == "ms":
-                    flags_vars[i] = 1e0
-                else:
-                    message = " units are not clear, assume s"
-                    warnings.warn(message)
-            else:
-                message = "Epoch_plus_var/Epoch_minus_var units are not clear, assume s"
-                warnings.warn(message)
-
-        flag_minus, flag_plus = flags_vars
-        t_offset = (
-            delta_plus_var["data"] * flag_plus - delta_minus_var["data"] * flag_minus
-        )
-        t_offset = np.timedelta64(int(np.round(t_offset, 1) * 1e6 / 2), "ns")
-        t_diff = (
-            delta_plus_var["data"] * flag_plus - delta_minus_var["data"] * flag_minus
-        )
-        t_diff = np.timedelta64(int(np.round(t_diff, 1) * 1e6 / 2), "ns")
-        t_diff_data = np.median(np.diff(epoch["data"])) / 2
-
-        if t_diff_data != np.mean(t_diff):
-            t_offset = t_diff_data
-
-        epoch_shifted += t_offset
-
-        return {"data": epoch_shifted, "attrs": epoch["attrs"]}
-
-    except KeyError:
-        return {"data": epoch_shifted, "attrs": epoch["attrs"]}
-
-
-def _get_epochs(file, cdf_name, tint):
-    r"""Get epochs form cdf and shift if needed."""
-
-    depend0_key = file.varattsget(cdf_name)["DEPEND_0"]
-
-    out = {
-        "data": file.varget(depend0_key, starttime=tint[0], endtime=tint[1]),
-    }
-
-    if file.varinq(depend0_key).Data_Type_Description == "CDF_TIME_TT2000":
-        try:
-            out["data"] = cdfepoch2datetime64(out["data"])
-
-            # Get epoch attributes
-            out["attrs"] = file.varattsget(depend0_key)
-
-            # Shift times if particle data
-            is_part = re.search(
-                "^mms[1-4]_d[ei]s_",
-                cdf_name,
-            )  # Is it FPI data?
-            is_part = is_part or re.search(
-                "^mms[1-4]_hpca_",
-                cdf_name,
-            )  # Is it HPCA data?
-
-            if is_part:
-                out = _shift_epochs(file, out)
-
-        except TypeError:
-            pass
-
-    return out
-
-
-def _get_depend_attributes(file, depend_key):
-    attributes = file.varattsget(depend_key)
-
-    # Remove spaces in label
-    try:
-        attributes["LABLAXIS"] = attributes["LABLAXIS"].replace(" ", "_")
-
-        if attributes["LABLAXIS"] == "Diffential_energy_channels":
-            attributes["LABLAXIS"] = "Differential_energy_channels"
-
-    except (KeyError, AttributeError):
-        attributes["LABLAXIS"] = "comp"
-
-    return attributes
-
-
-def _get_depend(file, cdf_name, tint, dep_num=1):
-    out = {}
-
-    try:
-        depend_key = file.varattsget(cdf_name)[f"DEPEND_{dep_num:d}"]
-    except KeyError:
-        depend_key = file.varattsget(cdf_name)[f"REPRESENTATION_{dep_num:d}"]
-
-    if depend_key == "x,y,z":
-        out["data"] = np.array(depend_key.split(","))
-
-        out["attrs"] = {"LABLAXIS": "comp"}
-    else:
-        try:
-            out["data"] = file.varget(
-                depend_key,
-                starttime=tint[0],
-                endtime=tint[1],
-            )
-        except IndexError:
-            out["data"] = file.varget(depend_key)
-
-        out["data"] = file.varget(depend_key)
-
-        if len(out["data"]) == 1:
-            out["data"] = out["data"][0]
-
-        if len(out["data"]) == 4 and all(out["data"] == ["x", "y", "z", "r"]):
-            out["data"] = out["data"][:-1]
-
-        elif out["data"].ndim == 2:
-            if len(out["data"].flatten()) == 3:
-                out["data"] = out["data"].flatten()
-            else:
-                try:
-                    out["data"] = out["data"][0, :]
-                except IndexError:
-                    pass
-
-        out["attrs"] = _get_depend_attributes(file, depend_key)
-
-    return out
-
-
-def get_ts(file_path, cdf_name, tint):
-    r"""Reads field named cdf_name in file and convert to time series.
-
-    Parameters
-    ----------
-    file_path : str
-        Path of the cdf file.
-    cdf_name : str
-        Name of the target variable in the cdf file.
-    tint : list of str
-        Time interval.
-
-    Returns
-    -------
-    out : xarray.DataArray
-        Time series of the target variable in the selected time interval.
-
-    """
-
-    # Check time interval type
-    # Check time interval
-    if isinstance(tint, (np.ndarray, list)):
-        if isinstance(tint[0], np.datetime64):
-            tint = datetime642iso8601(np.array(tint))
-        elif isinstance(tint[0], str):
-            tint = iso86012datetime64(
-                np.array(tint),
-            )  # to make sure it is ISO8601 ok!!
-            tint = datetime642iso8601(np.array(tint))
-        else:
-            raise TypeError("Values must be in datetime64, or str!!")
-    else:
-        raise TypeError("tint must be array_like!!")
-
-    # Extend time interval by 1s and convert time interval to epochs
-    tint_org = tint.copy()
-    tint = extend_tint(tint, [-1.0, 1.0])
-    tint = list(datetime642iso8601(iso86012datetime64(np.array(tint))))
-    tint = np.stack(list(map(cdfepoch.parse, tint)))
-
-    out_dict = {}
-    time, depend_1, depend_2, depend_3 = [{}, {}, {}, {}]
-
-    with CDF(file_path) as file:
-        var_attrs = file.varattsget(cdf_name)
-        glb_attrs = file.globalattsget()
-        out_dict["attrs"] = {"GLOBAL": glb_attrs, **var_attrs}
-        out_dict["attrs"] = {k: out_dict["attrs"][k] for k in sorted(out_dict["attrs"])}
-
-        assert "DEPEND_0" in var_attrs and "epoch" in var_attrs["DEPEND_0"].lower()
-
-        time = _get_epochs(file, cdf_name, tint)
-
-        if time["data"] is None:
-            return None
-
-        if "DEPEND_1" in var_attrs or "REPRESENTATION_1" in var_attrs:
-            depend_1 = _get_depend(file, cdf_name, tint, 1)
-
-        elif "afg" in cdf_name or "dfg" in cdf_name:
-            depend_1 = {
-                "data": ["x", "y", "z"],
-                "attrs": {"LABLAXIS": "comp"},
-            }
-
-        if "DEPEND_2" in var_attrs or "REPRESENTATION_2" in var_attrs:
-            depend_2 = _get_depend(file, cdf_name, tint, 2)
-
-            if depend_2["attrs"]["LABLAXIS"] == depend_1["attrs"]["LABLAXIS"]:
-                depend_1["attrs"]["LABLAXIS"] = "rcomp"
-                depend_2["attrs"]["LABLAXIS"] = "ccomp"
-
-        if "DEPEND_3" in var_attrs or "REPRESENTATION_3" in var_attrs:
-            if "REPRESENTATION_3" in var_attrs:
-                assert out_dict["attrs"]["REPRESENTATION_3"] != "x,y,z"
-
-            depend_3 = _get_depend(file, cdf_name, tint, 3)
-
-            if depend_3["attrs"]["LABLAXIS"] == depend_2["attrs"]["LABLAXIS"]:
-                depend_2["attrs"]["LABLAXIS"] = "rcomp"
-                depend_3["attrs"]["LABLAXIS"] = "ccomp"
-
-        if "sector_mask" in cdf_name:
-            cdf_name_mask = cdf_name.replace("sector_mask", "intensity")
-            depend_1_key = file.varattsget(cdf_name_mask)["DEPEND_1"]
-
-            depend_1["data"] = file.varget(depend_1_key)
-            depend_1["attrs"] = file.varattsget(depend_1_key)
-
-            depend_1["attrs"]["LABLAXIS"] = depend_1["attrs"]["LABLAXIS"].replace(
-                " ", "_"
-            )
-
-        if "edp_dce_sensor" in cdf_name:
-            depend_1["data"] = ["x", "y", "z"]
-            depend_1["attrs"] = {"LABLAXIS": "comp"}
-
-        out_dict["data"] = file.varget(
-            cdf_name,
-            starttime=tint[0],
-            endtime=tint[1],
-        )
-
-        if out_dict["data"].ndim == 2 and out_dict["data"].shape[1] == 4:
-            out_dict["data"] = out_dict["data"][:, :-1]
-
-    if out_dict["data"].ndim == 2 and not depend_1:
-        depend_1["data"] = np.arange(out_dict["data"].shape[1])
-        depend_1["attrs"] = {"LABLAXIS": "idx"}
-
-    if time and not depend_1 and not depend_2 and not depend_3:
-        dims = ["time"]
-        coords_data = [time["data"]]
-        coords_attrs = [time["attrs"]]
-
-    elif time and depend_1 and not depend_2 and not depend_3:
-        dims = ["time", depend_1["attrs"]["LABLAXIS"]]
-        coords_data = [time["data"], depend_1["data"]]
-        coords_attrs = [time["attrs"], depend_1["attrs"]]
-
-    elif time and depend_1 and depend_2 and not depend_3:
-        if depend_1["attrs"]["LABLAXIS"] == depend_2["attrs"]["LABLAXIS"]:
-            depend_1["attrs"]["LABLAXIS"] = "rcomp"
-            depend_2["attrs"]["LABLAXIS"] = "ccomp"
-
-        dims = [
-            "time",
-            depend_1["attrs"]["LABLAXIS"],
-            depend_2["attrs"]["LABLAXIS"],
-        ]
-        coords_data = [time["data"], depend_1["data"], depend_2["data"]]
-        coords_attrs = [time["attrs"], depend_1["attrs"], depend_2["attrs"]]
-
-    elif time and depend_1 and depend_2 and depend_3:
-        if depend_2["attrs"]["LABLAXIS"] == depend_3["attrs"]["LABLAXIS"]:
-            depend_2["attrs"]["LABLAXIS"] = "rcomp"
-            depend_3["attrs"]["LABLAXIS"] = "ccomp"
-
-        dims = [
-            "time",
-            depend_1["attrs"]["LABLAXIS"],
-            depend_2["attrs"]["LABLAXIS"],
-            depend_3["attrs"]["LABLAXIS"],
-        ]
-        coords_data = [
-            time["data"],
-            depend_1["data"],
-            depend_2["data"],
-            depend_3["data"],
-        ]
-        coords_attrs = [
-            time["attrs"],
-            depend_1["attrs"],
-            depend_2["attrs"],
-            depend_3["attrs"],
-        ]
-
-    else:
-        raise NotImplementedError
-
-    out = xr.DataArray(
-        out_dict["data"],
-        coords=coords_data,
-        dims=dims,
-        attrs=out_dict["attrs"],
-    )
-
-    for dim, coord_attrs in zip(dims, coords_attrs):
-        # Sort attributes and set to coordinates attribute
-        out[dim].attrs = {k: coord_attrs[k] for k in sorted(coord_attrs)}
-
-    # Time clip to original time interval
-    out = time_clip(out, tint_org)
-
-    return out
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# Built-in import
+import re
+import warnings
+
+# 3rd party imports
+import numpy as np
+import xarray as xr
+from cdflib import CDF, cdfepoch
+
+from ..pyrf.cdfepoch2datetime64 import cdfepoch2datetime64
+
+# Local imports
+from ..pyrf.datetime642iso8601 import datetime642iso8601
+from ..pyrf.extend_tint import extend_tint
+from ..pyrf.iso86012datetime64 import iso86012datetime64
+from ..pyrf.time_clip import time_clip
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def _shift_epochs(file, epoch):
+    r"""Shift times for particles."""
+
+    epoch_shifted = epoch["data"].copy()
+
+    try:
+        delta_minus_var = {
+            "data": file.varget(epoch["attrs"]["DELTA_MINUS_VAR"]),
+            "attrs": file.varget(epoch["attrs"]["DELTA_MINUS_VAR"]),
+        }
+        delta_plus_var = {
+            "data": file.varget(epoch["attrs"]["DELTA_PLUS_VAR"]),
+            "attrs": file.varget(epoch["attrs"]["DELTA_PLUS_VAR"]),
+        }
+
+        delta_vars = [delta_minus_var, delta_plus_var]
+        flags_vars = [1e3, 1e3]  # Time scaling conversion flags
+
+        for i, delta_var in enumerate(delta_vars):
+            if isinstance(delta_var["attrs"], dict) and "UNITS" in delta_var["attrs"]:
+                if delta_var["attrs"]["UNITS"].lower() == "s":
+                    flags_vars[i] = 1e3
+                elif delta_var["attrs"]["UNITS"].lower() == "ms":
+                    flags_vars[i] = 1e0
+                else:
+                    message = " units are not clear, assume s"
+                    warnings.warn(message)
+            else:
+                message = "Epoch_plus_var/Epoch_minus_var units are not clear, assume s"
+                warnings.warn(message)
+
+        flag_minus, flag_plus = flags_vars
+        t_offset = (
+            delta_plus_var["data"] * flag_plus - delta_minus_var["data"] * flag_minus
+        )
+        t_offset = np.timedelta64(int(np.round(t_offset, 1) * 1e6 / 2), "ns")
+        t_diff = (
+            delta_plus_var["data"] * flag_plus - delta_minus_var["data"] * flag_minus
+        )
+        t_diff = np.timedelta64(int(np.round(t_diff, 1) * 1e6 / 2), "ns")
+        t_diff_data = np.median(np.diff(epoch["data"])) / 2
+
+        if t_diff_data != np.mean(t_diff):
+            t_offset = t_diff_data
+
+        epoch_shifted += t_offset
+
+        return {"data": epoch_shifted, "attrs": epoch["attrs"]}
+
+    except KeyError:
+        return {"data": epoch_shifted, "attrs": epoch["attrs"]}
+
+
+def _get_epochs(file, cdf_name, tint):
+    r"""Get epochs form cdf and shift if needed."""
+
+    depend0_key = file.varattsget(cdf_name)["DEPEND_0"]
+
+    out = {
+        "data": file.varget(depend0_key, starttime=tint[0], endtime=tint[1]),
+    }
+
+    if file.varinq(depend0_key).Data_Type_Description == "CDF_TIME_TT2000":
+        try:
+            out["data"] = cdfepoch2datetime64(out["data"])
+
+            # Get epoch attributes
+            out["attrs"] = file.varattsget(depend0_key)
+
+            # Shift times if particle data
+            is_part = re.search(
+                "^mms[1-4]_d[ei]s_",
+                cdf_name,
+            )  # Is it FPI data?
+            is_part = is_part or re.search(
+                "^mms[1-4]_hpca_",
+                cdf_name,
+            )  # Is it HPCA data?
+
+            if is_part:
+                out = _shift_epochs(file, out)
+
+        except TypeError:
+            pass
+
+    return out
+
+
+def _get_depend_attributes(file, depend_key):
+    attributes = file.varattsget(depend_key)
+
+    # Remove spaces in label
+    try:
+        attributes["LABLAXIS"] = attributes["LABLAXIS"].replace(" ", "_")
+
+        if attributes["LABLAXIS"] == "Diffential_energy_channels":
+            attributes["LABLAXIS"] = "Differential_energy_channels"
+
+    except (KeyError, AttributeError):
+        attributes["LABLAXIS"] = "comp"
+
+    return attributes
+
+
+def _get_depend(file, cdf_name, tint, dep_num=1):
+    out = {}
+
+    try:
+        depend_key = file.varattsget(cdf_name)[f"DEPEND_{dep_num:d}"]
+    except KeyError:
+        depend_key = file.varattsget(cdf_name)[f"REPRESENTATION_{dep_num:d}"]
+
+    if depend_key == "x,y,z":
+        out["data"] = np.array(depend_key.split(","))
+
+        out["attrs"] = {"LABLAXIS": "comp"}
+    else:
+        try:
+            out["data"] = file.varget(
+                depend_key,
+                starttime=tint[0],
+                endtime=tint[1],
+            )
+        except IndexError:
+            out["data"] = file.varget(depend_key)
+
+        out["data"] = file.varget(depend_key)
+
+        if len(out["data"]) == 1:
+            out["data"] = out["data"][0]
+
+        if len(out["data"]) == 4 and all(out["data"] == ["x", "y", "z", "r"]):
+            out["data"] = out["data"][:-1]
+
+        elif out["data"].ndim == 2:
+            if len(out["data"].flatten()) == 3:
+                out["data"] = out["data"].flatten()
+            else:
+                try:
+                    out["data"] = out["data"][0, :]
+                except IndexError:
+                    pass
+
+        out["attrs"] = _get_depend_attributes(file, depend_key)
+
+    return out
+
+
+def get_ts(file_path, cdf_name, tint):
+    r"""Reads field named cdf_name in file and convert to time series.
+
+    Parameters
+    ----------
+    file_path : str
+        Path of the cdf file.
+    cdf_name : str
+        Name of the target variable in the cdf file.
+    tint : list of str
+        Time interval.
+
+    Returns
+    -------
+    out : xarray.DataArray
+        Time series of the target variable in the selected time interval.
+
+    """
+
+    # Check time interval type
+    # Check time interval
+    if isinstance(tint, (np.ndarray, list)):
+        if isinstance(tint[0], np.datetime64):
+            tint = datetime642iso8601(np.array(tint))
+        elif isinstance(tint[0], str):
+            tint = iso86012datetime64(
+                np.array(tint),
+            )  # to make sure it is ISO8601 ok!!
+            tint = datetime642iso8601(np.array(tint))
+        else:
+            raise TypeError("Values must be in datetime64, or str!!")
+    else:
+        raise TypeError("tint must be array_like!!")
+
+    # Extend time interval by 1s and convert time interval to epochs
+    tint_org = tint.copy()
+    tint = extend_tint(tint, [-1.0, 1.0])
+    tint = list(datetime642iso8601(iso86012datetime64(np.array(tint))))
+    tint = np.stack(list(map(cdfepoch.parse, tint)))
+
+    out_dict = {}
+    time, depend_1, depend_2, depend_3 = [{}, {}, {}, {}]
+
+    with CDF(file_path) as file:
+        var_attrs = file.varattsget(cdf_name)
+        glb_attrs = file.globalattsget()
+        out_dict["attrs"] = {"GLOBAL": glb_attrs, **var_attrs}
+        out_dict["attrs"] = {k: out_dict["attrs"][k] for k in sorted(out_dict["attrs"])}
+
+        assert "DEPEND_0" in var_attrs and "epoch" in var_attrs["DEPEND_0"].lower()
+
+        time = _get_epochs(file, cdf_name, tint)
+
+        if time["data"] is None:
+            return None
+
+        if "DEPEND_1" in var_attrs or "REPRESENTATION_1" in var_attrs:
+            depend_1 = _get_depend(file, cdf_name, tint, 1)
+
+        elif "afg" in cdf_name or "dfg" in cdf_name:
+            depend_1 = {
+                "data": ["x", "y", "z"],
+                "attrs": {"LABLAXIS": "comp"},
+            }
+
+        if "DEPEND_2" in var_attrs or "REPRESENTATION_2" in var_attrs:
+            depend_2 = _get_depend(file, cdf_name, tint, 2)
+
+            if depend_2["attrs"]["LABLAXIS"] == depend_1["attrs"]["LABLAXIS"]:
+                depend_1["attrs"]["LABLAXIS"] = "rcomp"
+                depend_2["attrs"]["LABLAXIS"] = "ccomp"
+
+        if "DEPEND_3" in var_attrs or "REPRESENTATION_3" in var_attrs:
+            if "REPRESENTATION_3" in var_attrs:
+                assert out_dict["attrs"]["REPRESENTATION_3"] != "x,y,z"
+
+            depend_3 = _get_depend(file, cdf_name, tint, 3)
+
+            if depend_3["attrs"]["LABLAXIS"] == depend_2["attrs"]["LABLAXIS"]:
+                depend_2["attrs"]["LABLAXIS"] = "rcomp"
+                depend_3["attrs"]["LABLAXIS"] = "ccomp"
+
+        if "sector_mask" in cdf_name:
+            cdf_name_mask = cdf_name.replace("sector_mask", "intensity")
+            depend_1_key = file.varattsget(cdf_name_mask)["DEPEND_1"]
+
+            depend_1["data"] = file.varget(depend_1_key)
+            depend_1["attrs"] = file.varattsget(depend_1_key)
+
+            depend_1["attrs"]["LABLAXIS"] = depend_1["attrs"]["LABLAXIS"].replace(
+                " ", "_"
+            )
+
+        if "edp_dce_sensor" in cdf_name:
+            depend_1["data"] = ["x", "y", "z"]
+            depend_1["attrs"] = {"LABLAXIS": "comp"}
+
+        out_dict["data"] = file.varget(
+            cdf_name,
+            starttime=tint[0],
+            endtime=tint[1],
+        )
+
+        if out_dict["data"].ndim == 2 and out_dict["data"].shape[1] == 4:
+            out_dict["data"] = out_dict["data"][:, :-1]
+
+    if out_dict["data"].ndim == 2 and not depend_1:
+        depend_1["data"] = np.arange(out_dict["data"].shape[1])
+        depend_1["attrs"] = {"LABLAXIS": "idx"}
+
+    if time and not depend_1 and not depend_2 and not depend_3:
+        dims = ["time"]
+        coords_data = [time["data"]]
+        coords_attrs = [time["attrs"]]
+
+    elif time and depend_1 and not depend_2 and not depend_3:
+        dims = ["time", depend_1["attrs"]["LABLAXIS"]]
+        coords_data = [time["data"], depend_1["data"]]
+        coords_attrs = [time["attrs"], depend_1["attrs"]]
+
+    elif time and depend_1 and depend_2 and not depend_3:
+        if depend_1["attrs"]["LABLAXIS"] == depend_2["attrs"]["LABLAXIS"]:
+            depend_1["attrs"]["LABLAXIS"] = "rcomp"
+            depend_2["attrs"]["LABLAXIS"] = "ccomp"
+
+        dims = [
+            "time",
+            depend_1["attrs"]["LABLAXIS"],
+            depend_2["attrs"]["LABLAXIS"],
+        ]
+        coords_data = [time["data"], depend_1["data"], depend_2["data"]]
+        coords_attrs = [time["attrs"], depend_1["attrs"], depend_2["attrs"]]
+
+    elif time and depend_1 and depend_2 and depend_3:
+        if depend_2["attrs"]["LABLAXIS"] == depend_3["attrs"]["LABLAXIS"]:
+            depend_2["attrs"]["LABLAXIS"] = "rcomp"
+            depend_3["attrs"]["LABLAXIS"] = "ccomp"
+
+        dims = [
+            "time",
+            depend_1["attrs"]["LABLAXIS"],
+            depend_2["attrs"]["LABLAXIS"],
+            depend_3["attrs"]["LABLAXIS"],
+        ]
+        coords_data = [
+            time["data"],
+            depend_1["data"],
+            depend_2["data"],
+            depend_3["data"],
+        ]
+        coords_attrs = [
+            time["attrs"],
+            depend_1["attrs"],
+            depend_2["attrs"],
+            depend_3["attrs"],
+        ]
+
+    else:
+        raise NotImplementedError
+
+    out = xr.DataArray(
+        out_dict["data"],
+        coords=coords_data,
+        dims=dims,
+        attrs=out_dict["attrs"],
+    )
+
+    for dim, coord_attrs in zip(dims, coords_attrs):
+        # Sort attributes and set to coordinates attribute
+        out[dim].attrs = {k: coord_attrs[k] for k in sorted(coord_attrs)}
+
+    # Time clip to original time interval
+    out = time_clip(out, tint_org)
+
+    return out
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/get_variable.py` & `pyrfu-2.4.3/pyrfu/mms/get_variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 # 3rd party imports
 import numpy as np
 import xarray as xr
 from cdflib import cdfread
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def get_variable(file_path, cdf_name):
     r"""Reads field named cdf_name in file and convert to DataArray.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/hpca_calc_anodes.py` & `pyrfu-2.4.3/pyrfu/mms/hpca_calc_anodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 anodes_theta = np.array(
     [
         123.75000,
         101.25000,
         78.750000,
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/hpca_energies.py` & `pyrfu-2.4.3/pyrfu/mms/hpca_energies.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def hpca_energies():
     r"""Construct Hot Plasma Composition Analyser (HPCA) energy bins"""
     return [
         1.35500,
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/hpca_pad.py` & `pyrfu-2.4.3/pyrfu/mms/hpca_pad.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,191 +1,191 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Built-in imports
-import warnings
-
-# 3rd party imports
-import numpy as np
-import xarray as xr
-from scipy import interpolate
-
-# Local imports
-from ..pyrf.normalize import normalize
-from ..pyrf.resample import resample
-from ..pyrf.time_clip import time_clip
-from ..pyrf.ts_scalar import ts_scalar
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.7"
-__status__ = "Prototype"
-
-
-def _hpca_elevations():
-    anode_theta = [
-        123.75000,
-        101.25000,
-        78.750000,
-        56.250000,
-        33.750000,
-        11.250000,
-        11.250000,
-        33.750000,
-        56.250000,
-        78.750000,
-        101.25000,
-        123.75000,
-        146.25000,
-        168.75000,
-        168.75000,
-        146.25000,
-    ]
-
-    anode_theta[6:14] = [anode_val + 180.0 for anode_val in anode_theta[6:14]]
-
-    return anode_theta
-
-
-def hpca_pad(vdf, saz, aze, b_xyz, elim=None):
-    r"""Computes HPCA pitch angle distribution.
-
-    Parameters
-    ----------
-    vdf : xarray.DataArray
-        Ion PSD or flux; [nt, npo16, ner63], looking direction
-    saz : xarray.DataArray
-        Start index of azimuthal angle; [nt, 1], (0 - 15)
-    aze : xarray.DataArray
-        Azimuthal angle per energy; [nT, naz16, npo16, ner63]
-    b_xyz : xarray.DataArray
-        B in dmpa coordinate
-    elim : list, Optional
-        [emin, emax], energy range for PAD
-
-    Returns
-    -------
-    pad_spec : xarray.DataArray
-        PAD spectrum
-
-    Examples
-    --------
-    >>> pad_ = hpca_pad(vdf, saz, aze, elev, ien, b_xyz, elim=[500, 3000])
-
-    """
-
-    # 1. get data
-    ien = vdf.ccomp
-    elev = _hpca_elevations()
-
-    if elim is None:
-        elim = [ien.data[0], ien.data[-1]]
-
-    # azimuthal angle #
-    n_az = 16
-
-    # 2. set tint and TLIM(dist & startaz)
-    n_start_az = np.where(saz.data == 0)[0][0]
-    start_time_match = aze.time.data[0].view("i8")
-    start_time_match -= vdf.time.data[n_start_az].view("i8")
-
-    if start_time_match < 1e6:
-        warnings.warn("start times of aze and vdf match.", UserWarning)
-    else:
-        raise ValueError("start times of aze and vdf don't match!")
-
-    n_stop_az = np.where(saz.data == 15)[0][-1]
-
-    if (n_stop_az - n_start_az + 1) // n_az == len(aze):
-        warnings.warn("stop times of aze and vdf match.", UserWarning)
-    else:
-        raise ValueError("stop times of aze and vdf don't match!")
-
-    tint_ = [saz.time.data[n_start_az], saz.time.data[n_stop_az]]
-    tint_ = [np.datetime_as_string(time, "ns") for time in tint_]
-
-    vdf = time_clip(vdf, tint_)
-
-    # 3. compute PAD
-    # 3.1. pitchangle
-    # Default pitch angles. 15 degree angle widths
-    angle_vec = np.linspace(15, 180, 12)
-
-    d_angle = np.median(np.diff(angle_vec)) * np.ones(len(angle_vec))
-    pitch_a = angle_vec - d_angle / 2
-
-    # 3.2.data dimension
-    n_po, n_en, n_ta, n_ti = len(elev), len(ien), len(aze), len(vdf)
-
-    assert n_ti == n_ta * n_az, "aze and vdf don't match!"
-
-    tt_ = vdf.time.data
-
-    # 3.3.reshape aze to aze_mat
-    aze_mat = np.transpose(aze.data, [1, 0, 2, 3])  # [nt, npo, ner]
-    aze_mat = np.reshape(aze_mat, [n_ti, n_po, n_en])
-
-    elev_mat = np.tile(elev, (n_ti, n_en, 1))  # [nt, npo, ner]
-    elev_mat = np.transpose(elev_mat, [0, 2, 1])
-    xx_ = np.sin(np.deg2rad(elev_mat)) * np.cos(np.deg2rad(aze_mat))
-    yy_ = np.sin(np.deg2rad(elev_mat)) * np.sin(np.deg2rad(aze_mat))
-    zz_ = np.cos(np.deg2rad(elev_mat))
-
-    t0_ = vdf.time.data.astype(np.int64)
-    t0_start = t0_[0]
-    t0_ -= t0_start
-    tck_ = interpolate.interp1d(
-        np.arange(0, n_en * len(t0_), n_en),
-        t0_,
-        fill_value="extrapolate",
-    )
-    t1_tt = tck_(np.arange(0, n_en * len(t0_))) + t0_start
-    t1_tt = t1_tt.astype("datetime64[ns]")
-    b_xyz_r = resample(b_xyz, ts_scalar(t1_tt, np.zeros(len(t1_tt))))
-    b_xyz_r = normalize(b_xyz_r)
-
-    b_x = np.transpose(np.reshape(b_xyz_r.data[:, 0], [n_en, n_ti]))
-    b_x = np.transpose(np.tile(b_x, [n_po, 1, 1]), [1, 0, 2])  # [nt, npo, ner]
-
-    b_y = np.transpose(np.reshape(b_xyz_r.data[:, 1], [n_en, n_ti]))
-    b_y = np.transpose(np.tile(b_y, [n_po, 1, 1]), [1, 0, 2])  # [nt, npo, ner]
-
-    b_z = np.transpose(np.reshape(b_xyz_r.data[:, 2], [n_en, n_ti]))
-    b_z = np.transpose(np.tile(b_z, [n_po, 1, 1]), [1, 0, 2])  # [nt, npo, ner]
-
-    theta_b = np.arccos(xx_ * b_x + yy_ * b_y + zz_ * b_z)
-    theta_b = np.rad2deg(theta_b)
-
-    # 3.5.select dist for PAD
-    vdfs_ = [vdf.data.copy() for _ in range(len(angle_vec))]
-
-    vdfs_[0][theta_b > angle_vec[0]] = np.nan
-
-    for i, vdf_ in enumerate(vdfs_):
-        vdf_[theta_b < (angle_vec[i] - d_angle[i])] = np.nan
-        vdf_[theta_b > angle_vec[i]] = np.nan
-
-    vdfs_[-1][theta_b < (angle_vec[-1] - d_angle[len(angle_vec) - 1])] = np.nan
-
-    # [n_ti, n_po, n_en] --> [n_ti, n_en]
-    vdfs_ = [np.squeeze(np.nanmean(vdf_, axis=1)) for vdf_ in vdfs_]
-
-    # average among energy dimension
-    i_elim = np.argmin(abs(ien.data - elim[0]))
-    e_min = ien.data[i_elim]
-    j_elim = np.argmin(abs(ien.data - elim[1]))
-    e_max = ien.data[j_elim]
-    messsage = f"PSD/pflux pitch angle dist. from {e_min} [eV] to {e_max} [eV]"
-    warnings.warn(messsage, UserWarning)
-
-    vdfs_ = [np.nanmean(vdf_[:, i_elim:j_elim], axis=1) for vdf_ in vdfs_]
-    vdfs_ = [np.squeeze(vdf_) for vdf_ in vdfs_]  # [n_ti, n_en] --> [n_ti]
-    padd_ = np.transpose(np.stack(vdfs_))  # [nt, ner, npitcha12]
-
-    # 3.6.make spectrum
-    coords = [tt_, pitch_a]
-    dims = ["time", "theta"]
-    pad_spec = xr.DataArray(padd_, coords=coords, dims=dims)
-
-    return pad_spec
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# Built-in imports
+import warnings
+
+# 3rd party imports
+import numpy as np
+import xarray as xr
+from scipy import interpolate
+
+# Local imports
+from ..pyrf.normalize import normalize
+from ..pyrf.resample import resample
+from ..pyrf.time_clip import time_clip
+from ..pyrf.ts_scalar import ts_scalar
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def _hpca_elevations():
+    anode_theta = [
+        123.75000,
+        101.25000,
+        78.750000,
+        56.250000,
+        33.750000,
+        11.250000,
+        11.250000,
+        33.750000,
+        56.250000,
+        78.750000,
+        101.25000,
+        123.75000,
+        146.25000,
+        168.75000,
+        168.75000,
+        146.25000,
+    ]
+
+    anode_theta[6:14] = [anode_val + 180.0 for anode_val in anode_theta[6:14]]
+
+    return anode_theta
+
+
+def hpca_pad(vdf, saz, aze, b_xyz, elim=None):
+    r"""Computes HPCA pitch angle distribution.
+
+    Parameters
+    ----------
+    vdf : xarray.DataArray
+        Ion PSD or flux; [nt, npo16, ner63], looking direction
+    saz : xarray.DataArray
+        Start index of azimuthal angle; [nt, 1], (0 - 15)
+    aze : xarray.DataArray
+        Azimuthal angle per energy; [nT, naz16, npo16, ner63]
+    b_xyz : xarray.DataArray
+        B in dmpa coordinate
+    elim : list, Optional
+        [emin, emax], energy range for PAD
+
+    Returns
+    -------
+    pad_spec : xarray.DataArray
+        PAD spectrum
+
+    Examples
+    --------
+    >>> pad_ = hpca_pad(vdf, saz, aze, elev, ien, b_xyz, elim=[500, 3000])
+
+    """
+
+    # 1. get data
+    ien = vdf.ccomp
+    elev = _hpca_elevations()
+
+    if elim is None:
+        elim = [ien.data[0], ien.data[-1]]
+
+    # azimuthal angle #
+    n_az = 16
+
+    # 2. set tint and TLIM(dist & startaz)
+    n_start_az = np.where(saz.data == 0)[0][0]
+    start_time_match = aze.time.data[0].view("i8")
+    start_time_match -= vdf.time.data[n_start_az].view("i8")
+
+    if start_time_match < 1e6:
+        warnings.warn("start times of aze and vdf match.", UserWarning)
+    else:
+        raise ValueError("start times of aze and vdf don't match!")
+
+    n_stop_az = np.where(saz.data == 15)[0][-1]
+
+    if (n_stop_az - n_start_az + 1) // n_az == len(aze):
+        warnings.warn("stop times of aze and vdf match.", UserWarning)
+    else:
+        raise ValueError("stop times of aze and vdf don't match!")
+
+    tint_ = [saz.time.data[n_start_az], saz.time.data[n_stop_az]]
+    tint_ = [np.datetime_as_string(time, "ns") for time in tint_]
+
+    vdf = time_clip(vdf, tint_)
+
+    # 3. compute PAD
+    # 3.1. pitchangle
+    # Default pitch angles. 15 degree angle widths
+    angle_vec = np.linspace(15, 180, 12)
+
+    d_angle = np.median(np.diff(angle_vec)) * np.ones(len(angle_vec))
+    pitch_a = angle_vec - d_angle / 2
+
+    # 3.2.data dimension
+    n_po, n_en, n_ta, n_ti = len(elev), len(ien), len(aze), len(vdf)
+
+    assert n_ti == n_ta * n_az, "aze and vdf don't match!"
+
+    tt_ = vdf.time.data
+
+    # 3.3.reshape aze to aze_mat
+    aze_mat = np.transpose(aze.data, [1, 0, 2, 3])  # [nt, npo, ner]
+    aze_mat = np.reshape(aze_mat, [n_ti, n_po, n_en])
+
+    elev_mat = np.tile(elev, (n_ti, n_en, 1))  # [nt, npo, ner]
+    elev_mat = np.transpose(elev_mat, [0, 2, 1])
+    xx_ = np.sin(np.deg2rad(elev_mat)) * np.cos(np.deg2rad(aze_mat))
+    yy_ = np.sin(np.deg2rad(elev_mat)) * np.sin(np.deg2rad(aze_mat))
+    zz_ = np.cos(np.deg2rad(elev_mat))
+
+    t0_ = vdf.time.data.astype(np.int64)
+    t0_start = t0_[0]
+    t0_ -= t0_start
+    tck_ = interpolate.interp1d(
+        np.arange(0, n_en * len(t0_), n_en),
+        t0_,
+        fill_value="extrapolate",
+    )
+    t1_tt = tck_(np.arange(0, n_en * len(t0_))) + t0_start
+    t1_tt = t1_tt.astype("datetime64[ns]")
+    b_xyz_r = resample(b_xyz, ts_scalar(t1_tt, np.zeros(len(t1_tt))))
+    b_xyz_r = normalize(b_xyz_r)
+
+    b_x = np.transpose(np.reshape(b_xyz_r.data[:, 0], [n_en, n_ti]))
+    b_x = np.transpose(np.tile(b_x, [n_po, 1, 1]), [1, 0, 2])  # [nt, npo, ner]
+
+    b_y = np.transpose(np.reshape(b_xyz_r.data[:, 1], [n_en, n_ti]))
+    b_y = np.transpose(np.tile(b_y, [n_po, 1, 1]), [1, 0, 2])  # [nt, npo, ner]
+
+    b_z = np.transpose(np.reshape(b_xyz_r.data[:, 2], [n_en, n_ti]))
+    b_z = np.transpose(np.tile(b_z, [n_po, 1, 1]), [1, 0, 2])  # [nt, npo, ner]
+
+    theta_b = np.arccos(xx_ * b_x + yy_ * b_y + zz_ * b_z)
+    theta_b = np.rad2deg(theta_b)
+
+    # 3.5.select dist for PAD
+    vdfs_ = [vdf.data.copy() for _ in range(len(angle_vec))]
+
+    vdfs_[0][theta_b > angle_vec[0]] = np.nan
+
+    for i, vdf_ in enumerate(vdfs_):
+        vdf_[theta_b < (angle_vec[i] - d_angle[i])] = np.nan
+        vdf_[theta_b > angle_vec[i]] = np.nan
+
+    vdfs_[-1][theta_b < (angle_vec[-1] - d_angle[len(angle_vec) - 1])] = np.nan
+
+    # [n_ti, n_po, n_en] --> [n_ti, n_en]
+    vdfs_ = [np.squeeze(np.nanmean(vdf_, axis=1)) for vdf_ in vdfs_]
+
+    # average among energy dimension
+    i_elim = np.argmin(abs(ien.data - elim[0]))
+    e_min = ien.data[i_elim]
+    j_elim = np.argmin(abs(ien.data - elim[1]))
+    e_max = ien.data[j_elim]
+    messsage = f"PSD/pflux pitch angle dist. from {e_min} [eV] to {e_max} [eV]"
+    warnings.warn(messsage, UserWarning)
+
+    vdfs_ = [np.nanmean(vdf_[:, i_elim:j_elim], axis=1) for vdf_ in vdfs_]
+    vdfs_ = [np.squeeze(vdf_) for vdf_ in vdfs_]  # [n_ti, n_en] --> [n_ti]
+    padd_ = np.transpose(np.stack(vdfs_))  # [nt, ner, npitcha12]
+
+    # 3.6.make spectrum
+    coords = [tt_, pitch_a]
+    dims = ["time", "theta"]
+    pad_spec = xr.DataArray(padd_, coords=coords, dims=dims)
+
+    return pad_spec
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/hpca_spin_sum.py` & `pyrfu-2.4.3/pyrfu/mms/hpca_spin_sum.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.12"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def hpca_spin_sum(inp, saz, method: str = "mean"):
     r"""Sum or average teh Hot Plasma Composition Analyser (HPCA) data over
     each spin.
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/lh_wave_analysis.py` & `pyrfu-2.4.3/pyrfu/mms/lh_wave_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from ..pyrf.resample import resample
 from ..pyrf.time_clip import time_clip
 from ..pyrf.ts_scalar import ts_scalar
 from ..pyrf.ts_vec_xyz import ts_vec_xyz
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def lh_wave_analysis(
     tints,
     e_xyz,
     b_scm,
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/list_files.py` & `pyrfu-2.4.3/pyrfu/mms/list_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 
 # Local imports
 from ..pyrf.datetime642iso8601 import datetime642iso8601
 from ..pyrf.iso86012datetime64 import iso86012datetime64
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2022"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.11"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def list_files(tint, mms_id, var, data_path: str = ""):
     """Find files in the data directories of the target instrument, data type,
     data rate, mms_id and level during the target time interval.
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/list_files_ancillary.py` & `pyrfu-2.4.3/pyrfu/mms/list_files_ancillary.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-import datetime
-import fnmatch
-import glob
-import json
-
-# Built-in imports
-import os
-import re
-
-# 3rd party imports
-import numpy as np
-import pandas as pd
-
-# Local imports
-from ..pyrf.datetime642iso8601 import datetime642iso8601
-from ..pyrf.iso86012datetime import iso86012datetime
-from ..pyrf.iso86012datetime64 import iso86012datetime64
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2023"
-__license__ = "MIT"
-__version__ = "2.3.26"
-__status__ = "Prototype"
-
-
-def list_files_ancillary(tint, mms_id, product, data_path: str = ""):
-    r"""Loads ancillary data.
-
-    Parameters
-    ----------
-    tint : list of str
-        Time interval
-    mms_id : str or int
-        Spacecraft index
-    product : {"predatt", "predeph", "defatt", "defeph"}
-        Ancillary type.
-    data_path : str, Optional
-        Path of MMS data. If None use `pyrfu.mms.mms_config.py`
-
-    Returns
-    -------
-    files_names : list
-        Ancillary files in interval.
-
-    """
-    # Check path
-    if not data_path:
-        pkg_path = os.path.dirname(os.path.abspath(__file__))
-
-        # Read the current version of the MMS configuration file
-        with open(os.path.join(pkg_path, "config.json"), "r", encoding="utf-8") as fs:
-            config = json.load(fs)
-
-        data_path = os.path.normpath(config["local_data_dir"])
-    else:
-        data_path = os.path.normpath(data_path)
-
-    # Make sure that the data path exists
-    assert os.path.exists(data_path), f"{data_path} doesn't exist!!"
-
-    if isinstance(mms_id, int):
-        mms_id = str(mms_id)
-
-    # Check time interval type
-    if isinstance(tint, (np.ndarray, list)):
-        if isinstance(tint[0], np.datetime64):
-            tint = datetime642iso8601(tint)
-            tint = iso86012datetime(tint)
-        elif isinstance(tint[0], str):
-            tint = iso86012datetime64(
-                np.array(tint),
-            )  # to make sure it is ISO8601 ok!
-            tint = datetime642iso8601(tint)
-            tint = iso86012datetime(tint)
-        elif isinstance(tint[0], datetime.datetime):
-            pass
-        else:
-            raise TypeError("Values must be in datetime, datetime64, or str!!")
-    else:
-        raise TypeError("tint must be a DataArray or array_like!!")
-
-    # directory and file name search patterns
-    # For now
-    # -all ancillary data is in one directory:
-    #       mms\ancillary
-    # -assume file names are of the form:
-    #   SPACECRAFT_FILETYPE_startDate_endDate.version
-    #   where SPACECRAFT is [MMS1, MMS2, MMS3, MMS4] in uppercase
-    #   and FILETYPE is either DEFATT, PREDATT, DEFEPH, PREDEPH in uppercase
-    #   and start/endDate is YYYYDOY
-    #   and version is Vnn (.V00, .V01, etc..)
-    dir_pattern = os.sep.join([data_path, "ancillary", f"mms{mms_id}", product])
-    file_pattern = "_".join([f"MMS{mms_id}", product.upper(), "???????_???????.V??"])
-
-    files_in_tint = []
-    out_files = []
-
-    files = glob.glob(os.sep.join([dir_pattern, file_pattern]))
-
-    # find the files within the time interval
-    fname_fmt = f"MMS{mms_id}_{product.upper()}_([0-9]{{7}})_([0-9]{{7}}).V[0-9]{{2}}"
-
-    if os.name == "nt":
-        full_path = os.sep.join([re.escape(dir_pattern) + os.sep, fname_fmt])
-    else:
-        full_path = os.sep.join([re.escape(dir_pattern), fname_fmt])
-
-    file_regex = re.compile(full_path)
-
-    for file in files:
-        time_match = file_regex.match(file)
-        if time_match is not None:
-            start_time = pd.to_datetime(time_match.group(1), format="%Y%j")
-            end_time = pd.to_datetime(time_match.group(2), format="%Y%j")
-            if start_time < tint[1] and end_time >= tint[0]:
-                files_in_tint.append(file)
-
-    # ensure only the latest version of each file is loaded
-    for file in files_in_tint:
-        this_file = file[0:-3] + "V??"
-        versions = fnmatch.filter(files_in_tint, this_file)
-        if len(versions) > 1:
-            # only grab the latest version
-            out_files.append(sorted(versions)[-1])
-        else:
-            out_files.append(versions[0])
-
-    files_names = list(set(out_files))
-    files_names.sort()
-
-    return files_names
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+import datetime
+import fnmatch
+import glob
+import json
+
+# Built-in imports
+import os
+import re
+
+# 3rd party imports
+import numpy as np
+import pandas as pd
+
+# Local imports
+from ..pyrf.datetime642iso8601 import datetime642iso8601
+from ..pyrf.iso86012datetime import iso86012datetime
+from ..pyrf.iso86012datetime64 import iso86012datetime64
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def list_files_ancillary(tint, mms_id, product, data_path: str = ""):
+    r"""Loads ancillary data.
+
+    Parameters
+    ----------
+    tint : list of str
+        Time interval
+    mms_id : str or int
+        Spacecraft index
+    product : {"predatt", "predeph", "defatt", "defeph"}
+        Ancillary type.
+    data_path : str, Optional
+        Path of MMS data. If None use `pyrfu.mms.mms_config.py`
+
+    Returns
+    -------
+    files_names : list
+        Ancillary files in interval.
+
+    """
+    # Check path
+    if not data_path:
+        pkg_path = os.path.dirname(os.path.abspath(__file__))
+
+        # Read the current version of the MMS configuration file
+        with open(os.path.join(pkg_path, "config.json"), "r", encoding="utf-8") as fs:
+            config = json.load(fs)
+
+        data_path = os.path.normpath(config["local_data_dir"])
+    else:
+        data_path = os.path.normpath(data_path)
+
+    # Make sure that the data path exists
+    assert os.path.exists(data_path), f"{data_path} doesn't exist!!"
+
+    if isinstance(mms_id, int):
+        mms_id = str(mms_id)
+
+    # Check time interval type
+    if isinstance(tint, (np.ndarray, list)):
+        if isinstance(tint[0], np.datetime64):
+            tint = datetime642iso8601(tint)
+            tint = iso86012datetime(tint)
+        elif isinstance(tint[0], str):
+            tint = iso86012datetime64(
+                np.array(tint),
+            )  # to make sure it is ISO8601 ok!
+            tint = datetime642iso8601(tint)
+            tint = iso86012datetime(tint)
+        elif isinstance(tint[0], datetime.datetime):
+            pass
+        else:
+            raise TypeError("Values must be in datetime, datetime64, or str!!")
+    else:
+        raise TypeError("tint must be a DataArray or array_like!!")
+
+    # directory and file name search patterns
+    # For now
+    # -all ancillary data is in one directory:
+    #       mms\ancillary
+    # -assume file names are of the form:
+    #   SPACECRAFT_FILETYPE_startDate_endDate.version
+    #   where SPACECRAFT is [MMS1, MMS2, MMS3, MMS4] in uppercase
+    #   and FILETYPE is either DEFATT, PREDATT, DEFEPH, PREDEPH in uppercase
+    #   and start/endDate is YYYYDOY
+    #   and version is Vnn (.V00, .V01, etc..)
+    dir_pattern = os.sep.join([data_path, "ancillary", f"mms{mms_id}", product])
+    file_pattern = "_".join([f"MMS{mms_id}", product.upper(), "???????_???????.V??"])
+
+    files_in_tint = []
+    out_files = []
+
+    files = glob.glob(os.sep.join([dir_pattern, file_pattern]))
+
+    # find the files within the time interval
+    fname_fmt = f"MMS{mms_id}_{product.upper()}_([0-9]{{7}})_([0-9]{{7}}).V[0-9]{{2}}"
+
+    if os.name == "nt":
+        full_path = os.sep.join([re.escape(dir_pattern) + os.sep, fname_fmt])
+    else:
+        full_path = os.sep.join([re.escape(dir_pattern), fname_fmt])
+
+    file_regex = re.compile(full_path)
+
+    for file in files:
+        time_match = file_regex.match(file)
+        if time_match is not None:
+            start_time = pd.to_datetime(time_match.group(1), format="%Y%j")
+            end_time = pd.to_datetime(time_match.group(2), format="%Y%j")
+            if start_time < tint[1] and end_time >= tint[0]:
+                files_in_tint.append(file)
+
+    # ensure only the latest version of each file is loaded
+    for file in files_in_tint:
+        this_file = file[0:-3] + "V??"
+        versions = fnmatch.filter(files_in_tint, this_file)
+        if len(versions) > 1:
+            # only grab the latest version
+            out_files.append(sorted(versions)[-1])
+        else:
+            out_files.append(versions[0])
+
+    files_names = list(set(out_files))
+    files_names.sort()
+
+    return files_names
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/load_ancillary.py` & `pyrfu-2.4.3/pyrfu/mms/load_ancillary.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-import bisect
-import json
-import logging
-
-# Built-in imports
-import os
-
-# 3rd party imports
-import pandas as pd
-
-from ..pyrf.extend_tint import extend_tint
-from ..pyrf.iso86012datetime import iso86012datetime
-
-# Local imports
-from .list_files_ancillary import list_files_ancillary
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.11"
-__status__ = "Prototype"
-
-logging.captureWarnings(True)
-logging.basicConfig(
-    format="[%(asctime)s] %(levelname)s: %(message)s",
-    datefmt="%d-%b-%y %H:%M:%S",
-    level=logging.INFO,
-)
-
-
-def load_ancillary(
-    product,
-    tint,
-    mms_id,
-    verbose: bool = True,
-    data_path: str = "",
-):
-    r"""Loads ancillary data.
-
-    Parameters
-    ----------
-    product : {"predatt", "predeph", "defatt", "defeph"}
-        Ancillary type.
-    tint : list of str
-        Time interval
-    mms_id : str or int
-        Spacecraft index
-    verbose : bool, Optional
-        Set to True to follow the loading. Default is True
-    data_path : str, Optional
-        Path of MMS data. If None use `pyrfu.mms.mms_config.py`
-
-    Returns
-    -------
-    out : xarray.Dataset
-        Time series of the ancillary data
-
-    """
-
-    # Get path of files in interval
-    tint_long = extend_tint(tint, [-86400, 86400])
-    files_names = list_files_ancillary(tint_long, mms_id, product, data_path)
-
-    # Convert time interval to datetime
-    tint = iso86012datetime(tint)
-
-    # Read length of header and columns names from .json file
-    # Root path
-    pkg_path = os.path.dirname(os.path.abspath(__file__))
-
-    with open(os.sep.join([pkg_path, "ancillary.json"]), "r", encoding="utf-8") as file:
-        anc_dict = json.load(file)
-
-    if verbose:
-        logging.info("Loading ancillary %s files...", product)
-
-    data_frame_dict = {}
-
-    for i, file in enumerate(files_names):
-        rows = pd.read_csv(
-            file,
-            delim_whitespace=True,
-            header=None,
-            skiprows=anc_dict[product]["header"],
-        )
-
-        # Remove footer
-        rows = rows[:][:-1]
-
-        # Convert time
-        fmt = anc_dict[product]["time_format"]
-        rows[0] = pd.to_datetime(rows[0], format=fmt)
-
-        start_idx = bisect.bisect_left(rows[0][:], tint[0])
-        end_idx = bisect.bisect_left(rows[0][:], tint[1])
-        rows.columns = anc_dict[product]["columns_names"]
-
-        data_frame_dict[i] = rows[:][start_idx:end_idx]
-
-    data_frame = data_frame_dict[0]
-
-    for k in list(data_frame_dict.keys())[1:]:
-        data_frame = data_frame.append(data_frame_dict[k])
-
-    data_frame = data_frame.sort_values(by="time").set_index(["time"])
-
-    return data_frame.to_xarray()
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+import bisect
+import json
+import logging
+
+# Built-in imports
+import os
+
+# 3rd party imports
+import pandas as pd
+
+from ..pyrf.extend_tint import extend_tint
+from ..pyrf.iso86012datetime import iso86012datetime
+
+# Local imports
+from .list_files_ancillary import list_files_ancillary
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+logging.captureWarnings(True)
+logging.basicConfig(
+    format="[%(asctime)s] %(levelname)s: %(message)s",
+    datefmt="%d-%b-%y %H:%M:%S",
+    level=logging.INFO,
+)
+
+
+def load_ancillary(
+    product,
+    tint,
+    mms_id,
+    verbose: bool = True,
+    data_path: str = "",
+):
+    r"""Loads ancillary data.
+
+    Parameters
+    ----------
+    product : {"predatt", "predeph", "defatt", "defeph"}
+        Ancillary type.
+    tint : list of str
+        Time interval
+    mms_id : str or int
+        Spacecraft index
+    verbose : bool, Optional
+        Set to True to follow the loading. Default is True
+    data_path : str, Optional
+        Path of MMS data. If None use `pyrfu.mms.mms_config.py`
+
+    Returns
+    -------
+    out : xarray.Dataset
+        Time series of the ancillary data
+
+    """
+
+    # Get path of files in interval
+    tint_long = extend_tint(tint, [-86400, 86400])
+    files_names = list_files_ancillary(tint_long, mms_id, product, data_path)
+
+    # Convert time interval to datetime
+    tint = iso86012datetime(tint)
+
+    # Read length of header and columns names from .json file
+    # Root path
+    pkg_path = os.path.dirname(os.path.abspath(__file__))
+
+    with open(os.sep.join([pkg_path, "ancillary.json"]), "r", encoding="utf-8") as file:
+        anc_dict = json.load(file)
+
+    if verbose:
+        logging.info("Loading ancillary %s files...", product)
+
+    data_frame_dict = {}
+
+    for i, file in enumerate(files_names):
+        rows = pd.read_csv(
+            file,
+            delim_whitespace=True,
+            header=None,
+            skiprows=anc_dict[product]["header"],
+        )
+
+        # Remove footer
+        rows = rows[:][:-1]
+
+        # Convert time
+        fmt = anc_dict[product]["time_format"]
+        rows[0] = pd.to_datetime(rows[0], format=fmt)
+
+        start_idx = bisect.bisect_left(rows[0][:], tint[0])
+        end_idx = bisect.bisect_left(rows[0][:], tint[1])
+        rows.columns = anc_dict[product]["columns_names"]
+
+        data_frame_dict[i] = rows[:][start_idx:end_idx]
+
+    data_frame = data_frame_dict[0]
+
+    for k in list(data_frame_dict.keys())[1:]:
+        data_frame = data_frame.append(data_frame_dict[k])
+
+    data_frame = data_frame.sort_values(by="time").set_index(["time"])
+
+    return data_frame.to_xarray()
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/load_brst_segments.py` & `pyrfu-2.4.3/pyrfu/mms/load_brst_segments.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from ..pyrf.datetime642iso8601 import datetime642iso8601
 from ..pyrf.extend_tint import extend_tint
 from ..pyrf.time_clip import time_clip
 from ..pyrf.ts_time import ts_time
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.17"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 URL = "http://www.spedas.org/mms/mms_brst_intervals.sav"
 
 
 def load_brst_segments(tint, data_path: str = None, download: bool = True):
     r"""Load burst segment time intervals associated with the input time
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/make_model_kappa.py` & `pyrfu-2.4.3/pyrfu/mms/make_model_kappa.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from scipy import constants, special
 
 # Local imports
 from ..pyrf.resample import resample
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def _thermal_velocity(energy, specie):
     if specie.lower() == "ions":
         mass = constants.proton_mass
     elif specie.lower() == "electrons":
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/make_model_rq.py` & `pyrfu-2.4.3/pyrfu/mms/make_model_rq.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Local imports
 from . import rotate_tensor
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.33"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def make_model_rq(
     vdf,
     b_xyz,
     sc_pot,
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/make_model_vdf.py` & `pyrfu-2.4.3/pyrfu/mms/make_model_vdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 from ..pyrf.dec_par_perp import dec_par_perp
 from ..pyrf.norm import norm
 from ..pyrf.resample import resample
 from ..pyrf.trace import trace
 from ..pyrf.ts_scalar import ts_scalar
 
 # Local imports
-from . import rotate_tensor
+from .rotate_tensor import rotate_tensor
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def make_model_vdf(
     vdf,
     b_xyz,
     sc_pot,
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/mms_keys.json` & `pyrfu-2.4.3/pyrfu/mms/mms_keys.json`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/pyrfu/mms/probe_align_times.py` & `pyrfu-2.4.3/pyrfu/mms/probe_align_times.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from ..pyrf.extend_tint import extend_tint
 from ..pyrf.resample import resample
 from ..pyrf.time_clip import time_clip
 from ..pyrf.ts_scalar import ts_scalar
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def probe_align_times(e_xyz, b_xyz, sc_pot, z_phase):
     r"""Returns times when field-aligned electrostatic waves can be
     characterized using interferometry techniques. The same alignment
     conditions as Graham et al., JGR, 2015 are used. Optional figure produced
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/psd2def.py` & `pyrfu-2.4.3/pyrfu/mms/psd2def.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # 3rd party imports
 import numpy as np
 from scipy import constants
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def _mass_ratio(inp):
     if inp.attrs["species"] in ["ions", "ion", "protons", "proton"]:
         mass_ratio = 1
     elif inp.attrs["species"] in ["alphas", "alpha", "helium"]:
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/psd2dpf.py` & `pyrfu-2.4.3/pyrfu/mms/psd2dpf.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # 3rd party imports
 import numpy as np
 from scipy import constants
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def _mass_ratio(inp):
     if inp.attrs["species"] in ["ions", "ion", "protons", "proton"]:
         mass_ratio = 1
     elif inp.attrs["species"] in ["alphas", "alpha", "helium"]:
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/psd_moments.py` & `pyrfu-2.4.3/pyrfu/mms/psd_moments.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from ..pyrf.resample import resample
 from ..pyrf.ts_scalar import ts_scalar
 from ..pyrf.ts_tensor_xyz import ts_tensor_xyz
 from ..pyrf.ts_vec_xyz import ts_vec_xyz
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 logging.captureWarnings(True)
 logging.basicConfig(
     format="[%(asctime)s] %(levelname)s: %(message)s",
     datefmt="%d-%b-%y %H:%M:%S",
     level=logging.INFO,
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/psd_rebin.py` & `pyrfu-2.4.3/pyrfu/mms/psd_rebin.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import xarray as xr
 
 # Local imports
 from ..pyrf.calc_dt import calc_dt
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def psd_rebin(vdf, phi, energy0, energy1, step_table):
     r"""Converts burst mode distribution into 64 energy channel distribution.
     Functions takes the burst mode distribution sampled in two energy tables
     and converts to a single energy table with 64 energy channels. Time
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/read_feeps_sector_masks_csv.py` & `pyrfu-2.4.3/pyrfu/mms/read_feeps_sector_masks_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # Local imports
 from ..pyrf.datetime642unix import datetime642unix
 from ..pyrf.iso86012datetime64 import iso86012datetime64
 from ..pyrf.unix2datetime64 import unix2datetime64
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def read_feeps_sector_masks_csv(tint):
     r"""Reads the FEEPS sectors to mask due to sunlight contamination from
     csv files.x
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/reduce.py` & `pyrfu-2.4.3/pyrfu/mms/reduce.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,248 +1,248 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Third party imports
-import numpy as np
-
-# Built-in imports
-import tqdm
-import xarray as xr
-from scipy.constants import electron_mass, electron_volt, proton_mass, speed_of_light
-
-# Local imports
-from ..pyrf.datetime642iso8601 import datetime642iso8601
-from ..pyrf.int_sph_dist import int_sph_dist
-from ..pyrf.resample import resample
-from ..pyrf.time_clip import time_clip
-from ..pyrf.ts_scalar import ts_scalar
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2023"
-__license__ = "MIT"
-__version__ = "2.3.33"
-__status__ = "Prototype"
-
-
-def reduce(vdf, xyz, dim: str = "1d", base: str = "pol", **kwargs):
-    r"""Reduces (integrates) 3D distribution to 1D (line) or 2D (plane).
-    Draft do not use!!
-
-    Parameters
-    ----------
-    vdf : xarray.Dataset
-        3D skymap velocity distribution function.
-    xyz : xarray.DataArray or numpy.ndarray
-        Transformation matrix from instrument frame to desired frame.
-    base : str, Optional
-        Base for the 2D projection either cartesian 'cart' (default) or
-        polar 'pol'.
-    **kwargs
-        Keyword arguments
-
-    Returns
-    -------
-    out : xarray.DataArray
-        Time series of reduced velocity distribution function.
-
-    """
-
-    # Make sure the projection dimension amd base are correct
-    assert dim.lower() in ["1d", "2d", "3d"], "Invalid projection dimension!!"
-    assert base.lower() in ["cart", "pol"], "Invalid projection base!!"
-
-    # Lower energy bound of instrument bins
-    delta_energy_minu = xr.DataArray(
-        vdf.attrs["delta_energy_minus"],
-        coords=[vdf.time.data, vdf.idx0.data],
-        dims=["time", "idx0"],
-    )
-
-    # Clip the distribution. If no time interval provided use the entire
-    # time series.
-    vdf_time = vdf.time.copy()
-    tint = kwargs.get("tint", list(datetime642iso8601(vdf_time[[0, -1]])))
-    vdf_time = time_clip(vdf_time, tint).copy()
-    vdf_energy = time_clip(vdf.energy, tint).copy()
-    delta_energy_minu = time_clip(delta_energy_minu, tint)
-    vdf_phi = time_clip(vdf.phi, tint).copy()
-    vdf_theta = vdf.theta.copy()
-    vdf_data = time_clip(vdf.data, tint).copy()
-
-    # make input distribution to SI units, s^3/m^6
-    if vdf.data.attrs["UNITS"].lower() == "s^3/cm^6":
-        vdf_data *= 1e12
-    elif vdf.data.attrs["UNITS"].lower() == "s^3/m^6":
-        vdf_data *= 1e0
-    elif vdf.data.attrs["UNITS"].lower() == "s^3/km^6":
-        vdf_data *= 1e-18
-    else:
-        raise ValueError("Invalid units!!")
-
-    # Get VDF dimension (time, energy, phi, theta)
-    # n_t, _, n_ph, _ = vdf_data.shape
-    n_t, _, _, _ = vdf_data.shape
-
-    # Construct or resample the time series of transformation matrix
-    if isinstance(xyz, xr.DataArray):
-        # If time series, clip to time interval and resample to VDF's time line
-        xyz = time_clip(xyz, tint)
-        xyz = resample(xyz, vdf_time).data
-    elif isinstance(xyz, np.ndarray) and xyz.ndim == 2:
-        assert xyz.shape == (3, 3), "xyz must be a transformation matrix!!"
-        # If matrix, tile to VDF timeline
-        xyz = np.tile(xyz, (n_t, 1, 1))
-    else:
-        raise TypeError("Invalid type for xyz")
-
-    # Check that the transformation matrices are orthonormal direct
-    x_phat_ts, y_phat_ts, z_phat_ts = [xyz[:, :, i] for i in range(3)]
-    x_phat_ts /= np.linalg.norm(x_phat_ts, axis=1, keepdims=True)
-    y_phat_ts /= np.linalg.norm(y_phat_ts, axis=1, keepdims=True)
-    z_phat_ts = np.cross(x_phat_ts, y_phat_ts)
-    z_phat_ts /= np.linalg.norm(z_phat_ts, axis=1, keepdims=True)
-    y_phat_ts = np.cross(z_phat_ts, x_phat_ts)
-
-    # Construct the time series of transformation matrix
-    xyz_ts = np.transpose(
-        np.stack([x_phat_ts, y_phat_ts, z_phat_ts]),
-        [1, 2, 0],
-    )
-
-    # Set azimuthal angle projection grid
-    # d_phi = kwargs.get("d_phi", 2 * np.pi / n_ph)
-    # phi_grid = np.linspace(0, 2 * np.pi, n_ph) + d_phi / 2  # centers
-
-    # Number of Monte Carlo iterations and weights
-    n_mc = kwargs.get("n_mc", 100)
-    weight = kwargs.get("weight", None)
-
-    v_lim = kwargs.get("v_lim", [-np.inf, np.inf])  # Velocity grid limits
-    a_lim = kwargs.get("a_lim", [-180.0, 180.0])  # Azimuthal angle limits
-
-    # Spacecraft potential to account for photoelectrons. If not provided set
-    # to 0 V.
-    sc_pot = kwargs.get("sc_pot", ts_scalar(vdf_time.data, np.zeros(n_t)))
-    sc_pot = resample(sc_pot, vdf_time).data
-
-    # Threshold energy (e.g., to remove background noise). If not provided set
-    # to 0 eV.
-    lower_e_lim = kwargs.get("lower_e_lim", 0.0)
-
-    if isinstance(lower_e_lim, xr.DataArray):
-        # If time series, clip to time interval and resample to VDF's time line
-        lower_e_lim = resample(lower_e_lim, vdf_time).data
-    elif isinstance(lower_e_lim, float):
-        # If float, tile to VDF's timeline
-        lower_e_lim = np.tile(lower_e_lim, n_t)
-    else:
-        raise TypeError("Invalid lower_e_lim!!")
-
-    # Set particle specie mass from VDF's attribute "species"
-    if vdf.species.lower() == "electrons":
-        m_p = electron_mass
-    elif vdf.species.lower() == "ions":
-        m_p = proton_mass
-    else:
-        raise ValueError("Invalid species!!")
-
-    # Convert maximum energy from instrument to velocity (relativistically
-    # correct)
-    e_max = vdf_energy.data[0, -1] + vdf.attrs["delta_energy_plus"][0, -1]
-    gamma_max = 1 + electron_volt * e_max / (m_p * speed_of_light**2)
-    v_max = speed_of_light * np.sqrt(1 - 1 / gamma_max**2)  # m/s
-
-    speed_grid_cart = np.linspace(-v_max, v_max, endpoint=True)
-
-    speed_grid = kwargs.get("vg", None)  # TODO : check that for no input!!
-    speed_grid_edges = kwargs.get("vg_edges", None)
-
-    # initiate projected f
-    n_vg = len(speed_grid)
-    n_pr = int(dim[0])
-    f_g = np.zeros([n_t, *[n_vg] * n_pr])
-    all_v = {f"v{chr(120 + i)}": np.zeros((n_t, n_vg)) for i in range(n_pr)}
-
-    for i_t in tqdm.tqdm(range(n_t), ncols=60):  # display progress
-        # 3d data matrix for time index
-        f_3d = np.squeeze(vdf_data.data[i_t, ...])  # s^3/m^6
-        f_3d = f_3d.astype(
-            np.float64,
-        ).copy()  # convert to C contiguous float64
-
-        # Energies
-        energy = vdf_energy.data[i_t, :]
-        energy = energy.astype(np.float64)  # Convert to float64
-
-        # Assign zeros to phase-space density values corresponding to energies
-        # below the threshold energy or below the spacecraft potential if
-        # provided.
-        thresh_e = np.max([lower_e_lim[i_t], sc_pot[i_t]])
-        e_min_idx = np.where(energy - delta_energy_minu[i_t, :] > thresh_e)[0][0]
-        f_3d[:e_min_idx] = 0.0
-
-        # Correct energy shift due to spacecraft potential
-        energy -= sc_pot[i_t]
-        energy[energy < 0] = 0.0
-
-        # Convert energy to velocity (relativistically correct)
-        gamma = 1 + electron_volt * energy / (m_p * speed_of_light**2)
-        speed = speed_of_light * np.sqrt(1 - 1 / gamma**2)  # m/s
-
-        # azimuthal angle
-        phi = vdf_phi.data[i_t, :].astype(np.float64)  # in degrees
-        phi = np.deg2rad(phi - 180.0)  # in radians
-
-        # elevation angle
-        theta = vdf_theta.data.astype(np.float64)  # in degrees
-        theta = np.deg2rad(theta - 90.0)  # in radians
-
-        # Set velocity projection grid.
-        if speed_grid_edges is not None:
-            speed_grid = speed_grid_edges[:-1] + 0.5 * np.diff(
-                speed_grid_edges,
-            )
-        elif speed_grid is None:
-            if base == "pol":
-                if dim == "1d":
-                    speed_grid = np.hstack((-np.flip(speed), speed))
-                elif dim in ["2d", "3d"]:
-                    speed_grid = speed
-                else:
-                    raise ValueError("Invalid projection dimension!!")
-            elif base == "cart":
-                speed_grid = speed_grid_cart
-            else:
-                raise ValueError("Invalid base!!")
-        else:
-            pass
-
-        options = {
-            "xyz": xyz_ts[i_t, ...],
-            "n_mc": n_mc,
-            "weight": weight,
-            "v_lim": v_lim,
-            "a_lim": a_lim,
-            "projection_dim": dim,
-            "projection_base": base,
-            "speed_grid_edges": speed_grid_edges,
-        }
-
-        tmpst = int_sph_dist(f_3d, speed, phi, theta, speed_grid, **options)
-
-        f_g[i_t, ...] = tmpst["f"]
-
-        for i in range(n_pr):
-            all_v[f"v{chr(120 + i)}"][i_t, :] = tmpst[f"v{chr(120 + i)}"] / 1e3  # km/s
-
-    # Build output as a time series with dimensions:
-    #   - (time x vx) for 1D reduced distribution
-    #   - (time x vx x vy) for 2D reduced distribution
-    coords = [
-        vdf_time.data,
-        *[all_v[f"v{chr(120 + i)}"][0, :] for i in range(n_pr)],
-    ]
-    dims = ["time", *[f"v{chr(120 + i)}" for i in range(n_pr)]]
-    out = xr.DataArray(f_g, coords=coords, dims=dims)
-
-    return out
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# Third party imports
+import numpy as np
+
+# Built-in imports
+import tqdm
+import xarray as xr
+from scipy.constants import electron_mass, electron_volt, proton_mass, speed_of_light
+
+# Local imports
+from ..pyrf.datetime642iso8601 import datetime642iso8601
+from ..pyrf.int_sph_dist import int_sph_dist
+from ..pyrf.resample import resample
+from ..pyrf.time_clip import time_clip
+from ..pyrf.ts_scalar import ts_scalar
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def reduce(vdf, xyz, dim: str = "1d", base: str = "pol", **kwargs):
+    r"""Reduces (integrates) 3D distribution to 1D (line) or 2D (plane).
+    Draft do not use!!
+
+    Parameters
+    ----------
+    vdf : xarray.Dataset
+        3D skymap velocity distribution function.
+    xyz : xarray.DataArray or numpy.ndarray
+        Transformation matrix from instrument frame to desired frame.
+    base : str, Optional
+        Base for the 2D projection either cartesian 'cart' (default) or
+        polar 'pol'.
+    **kwargs
+        Keyword arguments
+
+    Returns
+    -------
+    out : xarray.DataArray
+        Time series of reduced velocity distribution function.
+
+    """
+
+    # Make sure the projection dimension amd base are correct
+    assert dim.lower() in ["1d", "2d", "3d"], "Invalid projection dimension!!"
+    assert base.lower() in ["cart", "pol"], "Invalid projection base!!"
+
+    # Lower energy bound of instrument bins
+    delta_energy_minu = xr.DataArray(
+        vdf.attrs["delta_energy_minus"],
+        coords=[vdf.time.data, vdf.idx0.data],
+        dims=["time", "idx0"],
+    )
+
+    # Clip the distribution. If no time interval provided use the entire
+    # time series.
+    vdf_time = vdf.time.copy()
+    tint = kwargs.get("tint", list(datetime642iso8601(vdf_time[[0, -1]])))
+    vdf_time = time_clip(vdf_time, tint).copy()
+    vdf_energy = time_clip(vdf.energy, tint).copy()
+    delta_energy_minu = time_clip(delta_energy_minu, tint)
+    vdf_phi = time_clip(vdf.phi, tint).copy()
+    vdf_theta = vdf.theta.copy()
+    vdf_data = time_clip(vdf.data, tint).copy()
+
+    # make input distribution to SI units, s^3/m^6
+    if vdf.data.attrs["UNITS"].lower() == "s^3/cm^6":
+        vdf_data *= 1e12
+    elif vdf.data.attrs["UNITS"].lower() == "s^3/m^6":
+        vdf_data *= 1e0
+    elif vdf.data.attrs["UNITS"].lower() == "s^3/km^6":
+        vdf_data *= 1e-18
+    else:
+        raise ValueError("Invalid units!!")
+
+    # Get VDF dimension (time, energy, phi, theta)
+    # n_t, _, n_ph, _ = vdf_data.shape
+    n_t, _, _, _ = vdf_data.shape
+
+    # Construct or resample the time series of transformation matrix
+    if isinstance(xyz, xr.DataArray):
+        # If time series, clip to time interval and resample to VDF's time line
+        xyz = time_clip(xyz, tint)
+        xyz = resample(xyz, vdf_time).data
+    elif isinstance(xyz, np.ndarray) and xyz.ndim == 2:
+        assert xyz.shape == (3, 3), "xyz must be a transformation matrix!!"
+        # If matrix, tile to VDF timeline
+        xyz = np.tile(xyz, (n_t, 1, 1))
+    else:
+        raise TypeError("Invalid type for xyz")
+
+    # Check that the transformation matrices are orthonormal direct
+    x_phat_ts, y_phat_ts, z_phat_ts = [xyz[:, :, i] for i in range(3)]
+    x_phat_ts /= np.linalg.norm(x_phat_ts, axis=1, keepdims=True)
+    y_phat_ts /= np.linalg.norm(y_phat_ts, axis=1, keepdims=True)
+    z_phat_ts = np.cross(x_phat_ts, y_phat_ts)
+    z_phat_ts /= np.linalg.norm(z_phat_ts, axis=1, keepdims=True)
+    y_phat_ts = np.cross(z_phat_ts, x_phat_ts)
+
+    # Construct the time series of transformation matrix
+    xyz_ts = np.transpose(
+        np.stack([x_phat_ts, y_phat_ts, z_phat_ts]),
+        [1, 2, 0],
+    )
+
+    # Set azimuthal angle projection grid
+    # d_phi = kwargs.get("d_phi", 2 * np.pi / n_ph)
+    # phi_grid = np.linspace(0, 2 * np.pi, n_ph) + d_phi / 2  # centers
+
+    # Number of Monte Carlo iterations and weights
+    n_mc = kwargs.get("n_mc", 100)
+    weight = kwargs.get("weight", None)
+
+    v_lim = kwargs.get("v_lim", [-np.inf, np.inf])  # Velocity grid limits
+    a_lim = kwargs.get("a_lim", [-180.0, 180.0])  # Azimuthal angle limits
+
+    # Spacecraft potential to account for photoelectrons. If not provided set
+    # to 0 V.
+    sc_pot = kwargs.get("sc_pot", ts_scalar(vdf_time.data, np.zeros(n_t)))
+    sc_pot = resample(sc_pot, vdf_time).data
+
+    # Threshold energy (e.g., to remove background noise). If not provided set
+    # to 0 eV.
+    lower_e_lim = kwargs.get("lower_e_lim", 0.0)
+
+    if isinstance(lower_e_lim, xr.DataArray):
+        # If time series, clip to time interval and resample to VDF's time line
+        lower_e_lim = resample(lower_e_lim, vdf_time).data
+    elif isinstance(lower_e_lim, float):
+        # If float, tile to VDF's timeline
+        lower_e_lim = np.tile(lower_e_lim, n_t)
+    else:
+        raise TypeError("Invalid lower_e_lim!!")
+
+    # Set particle specie mass from VDF's attribute "species"
+    if vdf.species.lower() == "electrons":
+        m_p = electron_mass
+    elif vdf.species.lower() == "ions":
+        m_p = proton_mass
+    else:
+        raise ValueError("Invalid species!!")
+
+    # Convert maximum energy from instrument to velocity (relativistically
+    # correct)
+    e_max = vdf_energy.data[0, -1] + vdf.attrs["delta_energy_plus"][0, -1]
+    gamma_max = 1 + electron_volt * e_max / (m_p * speed_of_light**2)
+    v_max = speed_of_light * np.sqrt(1 - 1 / gamma_max**2)  # m/s
+
+    speed_grid_cart = np.linspace(-v_max, v_max, endpoint=True)
+
+    speed_grid = kwargs.get("vg", None)  # TODO : check that for no input!!
+    speed_grid_edges = kwargs.get("vg_edges", None)
+
+    # initiate projected f
+    n_vg = len(speed_grid)
+    n_pr = int(dim[0])
+    f_g = np.zeros([n_t, *[n_vg] * n_pr])
+    all_v = {f"v{chr(120 + i)}": np.zeros((n_t, n_vg)) for i in range(n_pr)}
+
+    for i_t in tqdm.tqdm(range(n_t), ncols=60):  # display progress
+        # 3d data matrix for time index
+        f_3d = np.squeeze(vdf_data.data[i_t, ...])  # s^3/m^6
+        f_3d = f_3d.astype(
+            np.float64,
+        ).copy()  # convert to C contiguous float64
+
+        # Energies
+        energy = vdf_energy.data[i_t, :]
+        energy = energy.astype(np.float64)  # Convert to float64
+
+        # Assign zeros to phase-space density values corresponding to energies
+        # below the threshold energy or below the spacecraft potential if
+        # provided.
+        thresh_e = np.max([lower_e_lim[i_t], sc_pot[i_t]])
+        e_min_idx = np.where(energy - delta_energy_minu[i_t, :] > thresh_e)[0][0]
+        f_3d[:e_min_idx] = 0.0
+
+        # Correct energy shift due to spacecraft potential
+        energy -= sc_pot[i_t]
+        energy[energy < 0] = 0.0
+
+        # Convert energy to velocity (relativistically correct)
+        gamma = 1 + electron_volt * energy / (m_p * speed_of_light**2)
+        speed = speed_of_light * np.sqrt(1 - 1 / gamma**2)  # m/s
+
+        # azimuthal angle
+        phi = vdf_phi.data[i_t, :].astype(np.float64)  # in degrees
+        phi = np.deg2rad(phi - 180.0)  # in radians
+
+        # elevation angle
+        theta = vdf_theta.data.astype(np.float64)  # in degrees
+        theta = np.deg2rad(theta - 90.0)  # in radians
+
+        # Set velocity projection grid.
+        if speed_grid_edges is not None:
+            speed_grid = speed_grid_edges[:-1] + 0.5 * np.diff(
+                speed_grid_edges,
+            )
+        elif speed_grid is None:
+            if base == "pol":
+                if dim == "1d":
+                    speed_grid = np.hstack((-np.flip(speed), speed))
+                elif dim in ["2d", "3d"]:
+                    speed_grid = speed
+                else:
+                    raise ValueError("Invalid projection dimension!!")
+            elif base == "cart":
+                speed_grid = speed_grid_cart
+            else:
+                raise ValueError("Invalid base!!")
+        else:
+            pass
+
+        options = {
+            "xyz": xyz_ts[i_t, ...],
+            "n_mc": n_mc,
+            "weight": weight,
+            "v_lim": v_lim,
+            "a_lim": a_lim,
+            "projection_dim": dim,
+            "projection_base": base,
+            "speed_grid_edges": speed_grid_edges,
+        }
+
+        tmpst = int_sph_dist(f_3d, speed, phi, theta, speed_grid, **options)
+
+        f_g[i_t, ...] = tmpst["f"]
+
+        for i in range(n_pr):
+            all_v[f"v{chr(120 + i)}"][i_t, :] = tmpst[f"v{chr(120 + i)}"] / 1e3  # km/s
+
+    # Build output as a time series with dimensions:
+    #   - (time x vx) for 1D reduced distribution
+    #   - (time x vx x vy) for 2D reduced distribution
+    coords = [
+        vdf_time.data,
+        *[all_v[f"v{chr(120 + i)}"][0, :] for i in range(n_pr)],
+    ]
+    dims = ["time", *[f"v{chr(120 + i)}" for i in range(n_pr)]]
+    out = xr.DataArray(f_g, coords=coords, dims=dims)
+
+    return out
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/remove_edist_background.py` & `pyrfu-2.4.3/pyrfu/mms/remove_edist_background.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,170 +1,170 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Built-in imports
-import json
-import os
-
-# 3rd party imports
-import numpy as np
-from cdflib import cdfread
-
-from ..pyrf.datetime642iso8601 import datetime642iso8601
-from ..pyrf.time_clip import time_clip
-from ..pyrf.ts_skymap import ts_skymap
-
-# Local imports
-from .db_get_ts import db_get_ts
-from .get_data import get_data
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2023"
-__license__ = "MIT"
-__version__ = "2.3.26"
-__status__ = "Prototype"
-
-
-def remove_edist_background(vdf, n_sec: float = 0.0, n_art: float = -1.0):
-    r"""Remove secondary photoelectrons from electron distribution function
-    according to [1]_.
-
-    Parameters
-    ----------
-    vdf : xarray.Dataset
-        Measured electron velocity distribution function.
-    n_sec : float, Optional
-        Artificial secondary electron density (isotropic). Default is 0.
-    n_art : float, Optional
-        Artificial photoelectron density (sun-angle dependant),
-        Default is ephoto_scale from des-emoms GlobalAttributes.
-
-    Returns
-    -------
-    vdf_new : xarray.Dataset
-        Electron VDF with photoelectrons removed.
-    vdf_bkg : xarray.Dataset
-        Photoelectron VDF.
-    photoe_scle : float
-        Artificial photoelectron and secondary electron density
-
-    References
-    ----------
-    .. [1]  Gershman, D. J., Avanov, L. A., Boardsen,S. A., Dorelli, J. C.,
-            Gliese, U., Barrie, A. C.,... Pollock, C. J. (2017). Spacecraft
-            and instrument photoelectrons measured by the dual electron
-            spectrometers on MMS. Journal of Geophysical Research:Space
-            Physics,122, 11,548–11,558. https://doi.org/10.1002/2017JA024518
-
-    """
-
-    # Time interval of VDF
-    tint = list(datetime642iso8601(vdf.time.data[[0, -1]]))
-
-    # Get spacecraft index from VDF metadata
-    mms_id = vdf.attrs["CATDESC"].split(" ")[0].lower()
-    mms_id = int(mms_id[-1])
-
-    vdf_tmp = time_clip(vdf, tint)
-    vdf_new = np.zeros_like(vdf_tmp.data.data)
-    vdf_bkg = np.zeros_like(vdf_tmp.data.data)
-
-    dataset_name = f"mms{mms_id}_fpi_brst_l2_des-dist"
-    startdelphi_count = db_get_ts(
-        dataset_name,
-        f"mms{mms_id}_des_startdelphi_count_brst",
-        tint,
-        verbose=False,
-    )
-
-    # Load the elctron number density to get the name of the photoelectron
-    # model file, and the photoelectron scaling factor
-    n_e = get_data("ne_fpi_brst_l2", tint, mms_id, verbose=False)
-
-    photoe_scle = n_e.attrs["Photoelectron_model_scaling_factor"]
-    photoe_scle = float(photoe_scle)
-
-    # Load the model internal photoelectrons
-    bkg_fname = n_e.attrs["Photoelectron_model_filenames"]
-
-    # Check path
-    # Guess data path from CDF attributes
-    data_path = str(vdf.attrs["CDF"]).split(f"mms{mms_id}/fpi", maxsplit=1)[0]
-
-    # Check if path exists if not use the default
-    if not os.path.exists(data_path):
-        pkg_path = os.path.dirname(os.path.abspath(__file__))
-
-        # Read the current version of the MMS configuration file
-        with open(os.path.join(pkg_path, "config.json"), "r", encoding="utf-8") as fs:
-            config = json.load(fs)
-
-        data_path = os.path.normpath(config["local_data_dir"])
-    else:
-        data_path = os.path.normpath(data_path)
-
-    bkg_fname = os.path.join(data_path, "models", "fpi", bkg_fname)
-
-    vdf_bkg01 = [None, None]
-    with cdfread.CDF(bkg_fname) as f:
-        vdf_bkg01[0] = f.varget("mms_des_bgdist_p0_brst")
-        vdf_bkg01[0] = np.transpose(vdf_bkg01[0], [0, 3, 1, 2])
-        vdf_bkg01[1] = f.varget("mms_des_bgdist_p1_brst")
-        vdf_bkg01[1] = np.transpose(vdf_bkg01[1], [0, 3, 1, 2])
-
-    # Overwrite fraction of photoelectron if provided by user.
-    if n_art > 0:
-        n_photo = n_art
-    else:
-        n_photo = photoe_scle
-
-    for i, _ in enumerate(vdf.time.data):
-        istartdelphi_count = startdelphi_count.data[i]
-        iebgdist = int(np.fix(istartdelphi_count / 16))
-
-        esteptable_idx = int(vdf.attrs["esteptable"][i])
-        vdf_bkg_tmp_data = vdf_bkg01[esteptable_idx][iebgdist, ...]
-        vdf_bkg_tmp = n_photo * vdf_bkg_tmp_data
-
-        if n_sec > 0:
-            vdf_bkg_av = np.nanmean(vdf_bkg_tmp_data, axis=2)
-            vdf_bkg_av = np.tile(vdf_bkg_av, (vdf_bkg_tmp_data.shape[2], 1, 1))
-            vdf_bkg_av = np.transpose(vdf_bkg_av, [1, 2, 0])
-
-            vdf_bkg_tmp += n_sec * vdf_bkg_av
-
-        vdf_new_tmp = vdf.data.data[i, ...] - vdf_bkg_tmp
-        vdf_new_tmp[vdf_new_tmp < 0] = 0.0
-        vdf_bkg_tmp[vdf_bkg_tmp < 0] = 0.0
-        vdf_new[i, ...] = vdf_new_tmp
-        vdf_bkg[i, ...] = vdf_bkg_tmp
-
-    # Construct the new VDFs
-    glob_attrs = vdf.attrs
-    vdf_attrs = vdf.data.attrs
-    coords_attrs = {k: vdf[k].attrs for k in ["time", "energy", "phi", "theta"]}
-
-    vdf_new = ts_skymap(
-        vdf.time.data,
-        vdf_new,
-        vdf.energy.data,
-        vdf.phi.data,
-        vdf.theta.data,
-        attrs=vdf_attrs,
-        coords_attrs=coords_attrs,
-        glob_attrs=glob_attrs,
-    )
-    vdf_new.attrs = vdf.attrs
-    vdf_bkg = ts_skymap(
-        vdf.time.data,
-        vdf_bkg,
-        vdf.energy.data,
-        vdf.phi.data,
-        vdf.theta.data,
-        attrs=vdf_attrs,
-        coords_attrs=coords_attrs,
-        glob_attrs=glob_attrs,
-    )
-    vdf_bkg.attrs = vdf.attrs
-
-    return vdf_new, vdf_bkg, photoe_scle
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# Built-in imports
+import json
+import os
+
+# 3rd party imports
+import numpy as np
+from cdflib import cdfread
+
+from ..pyrf.datetime642iso8601 import datetime642iso8601
+from ..pyrf.time_clip import time_clip
+from ..pyrf.ts_skymap import ts_skymap
+
+# Local imports
+from .db_get_ts import db_get_ts
+from .get_data import get_data
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def remove_edist_background(vdf, n_sec: float = 0.0, n_art: float = -1.0):
+    r"""Remove secondary photoelectrons from electron distribution function
+    according to [1]_.
+
+    Parameters
+    ----------
+    vdf : xarray.Dataset
+        Measured electron velocity distribution function.
+    n_sec : float, Optional
+        Artificial secondary electron density (isotropic). Default is 0.
+    n_art : float, Optional
+        Artificial photoelectron density (sun-angle dependant),
+        Default is ephoto_scale from des-emoms GlobalAttributes.
+
+    Returns
+    -------
+    vdf_new : xarray.Dataset
+        Electron VDF with photoelectrons removed.
+    vdf_bkg : xarray.Dataset
+        Photoelectron VDF.
+    photoe_scle : float
+        Artificial photoelectron and secondary electron density
+
+    References
+    ----------
+    .. [1]  Gershman, D. J., Avanov, L. A., Boardsen,S. A., Dorelli, J. C.,
+            Gliese, U., Barrie, A. C.,... Pollock, C. J. (2017). Spacecraft
+            and instrument photoelectrons measured by the dual electron
+            spectrometers on MMS. Journal of Geophysical Research:Space
+            Physics,122, 11,548–11,558. https://doi.org/10.1002/2017JA024518
+
+    """
+
+    # Time interval of VDF
+    tint = list(datetime642iso8601(vdf.time.data[[0, -1]]))
+
+    # Get spacecraft index from VDF metadata
+    mms_id = vdf.attrs["CATDESC"].split(" ")[0].lower()
+    mms_id = int(mms_id[-1])
+
+    vdf_tmp = time_clip(vdf, tint)
+    vdf_new = np.zeros_like(vdf_tmp.data.data)
+    vdf_bkg = np.zeros_like(vdf_tmp.data.data)
+
+    dataset_name = f"mms{mms_id}_fpi_brst_l2_des-dist"
+    startdelphi_count = db_get_ts(
+        dataset_name,
+        f"mms{mms_id}_des_startdelphi_count_brst",
+        tint,
+        verbose=False,
+    )
+
+    # Load the elctron number density to get the name of the photoelectron
+    # model file, and the photoelectron scaling factor
+    n_e = get_data("ne_fpi_brst_l2", tint, mms_id, verbose=False)
+
+    photoe_scle = n_e.attrs["Photoelectron_model_scaling_factor"]
+    photoe_scle = float(photoe_scle)
+
+    # Load the model internal photoelectrons
+    bkg_fname = n_e.attrs["Photoelectron_model_filenames"]
+
+    # Check path
+    # Guess data path from CDF attributes
+    data_path = str(vdf.attrs["CDF"]).split(f"mms{mms_id}/fpi", maxsplit=1)[0]
+
+    # Check if path exists if not use the default
+    if not os.path.exists(data_path):
+        pkg_path = os.path.dirname(os.path.abspath(__file__))
+
+        # Read the current version of the MMS configuration file
+        with open(os.path.join(pkg_path, "config.json"), "r", encoding="utf-8") as fs:
+            config = json.load(fs)
+
+        data_path = os.path.normpath(config["local_data_dir"])
+    else:
+        data_path = os.path.normpath(data_path)
+
+    bkg_fname = os.path.join(data_path, "models", "fpi", bkg_fname)
+
+    vdf_bkg01 = [None, None]
+    with cdfread.CDF(bkg_fname) as f:
+        vdf_bkg01[0] = f.varget("mms_des_bgdist_p0_brst")
+        vdf_bkg01[0] = np.transpose(vdf_bkg01[0], [0, 3, 1, 2])
+        vdf_bkg01[1] = f.varget("mms_des_bgdist_p1_brst")
+        vdf_bkg01[1] = np.transpose(vdf_bkg01[1], [0, 3, 1, 2])
+
+    # Overwrite fraction of photoelectron if provided by user.
+    if n_art > 0:
+        n_photo = n_art
+    else:
+        n_photo = photoe_scle
+
+    for i, _ in enumerate(vdf.time.data):
+        istartdelphi_count = startdelphi_count.data[i]
+        iebgdist = int(np.fix(istartdelphi_count / 16))
+
+        esteptable_idx = int(vdf.attrs["esteptable"][i])
+        vdf_bkg_tmp_data = vdf_bkg01[esteptable_idx][iebgdist, ...]
+        vdf_bkg_tmp = n_photo * vdf_bkg_tmp_data
+
+        if n_sec > 0:
+            vdf_bkg_av = np.nanmean(vdf_bkg_tmp_data, axis=2)
+            vdf_bkg_av = np.tile(vdf_bkg_av, (vdf_bkg_tmp_data.shape[2], 1, 1))
+            vdf_bkg_av = np.transpose(vdf_bkg_av, [1, 2, 0])
+
+            vdf_bkg_tmp += n_sec * vdf_bkg_av
+
+        vdf_new_tmp = vdf.data.data[i, ...] - vdf_bkg_tmp
+        vdf_new_tmp[vdf_new_tmp < 0] = 0.0
+        vdf_bkg_tmp[vdf_bkg_tmp < 0] = 0.0
+        vdf_new[i, ...] = vdf_new_tmp
+        vdf_bkg[i, ...] = vdf_bkg_tmp
+
+    # Construct the new VDFs
+    glob_attrs = vdf.attrs
+    vdf_attrs = vdf.data.attrs
+    coords_attrs = {k: vdf[k].attrs for k in ["time", "energy", "phi", "theta"]}
+
+    vdf_new = ts_skymap(
+        vdf.time.data,
+        vdf_new,
+        vdf.energy.data,
+        vdf.phi.data,
+        vdf.theta.data,
+        attrs=vdf_attrs,
+        coords_attrs=coords_attrs,
+        glob_attrs=glob_attrs,
+    )
+    vdf_new.attrs = vdf.attrs
+    vdf_bkg = ts_skymap(
+        vdf.time.data,
+        vdf_bkg,
+        vdf.energy.data,
+        vdf.phi.data,
+        vdf.theta.data,
+        attrs=vdf_attrs,
+        coords_attrs=coords_attrs,
+        glob_attrs=glob_attrs,
+    )
+    vdf_bkg.attrs = vdf.attrs
+
+    return vdf_new, vdf_bkg, photoe_scle
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/remove_idist_background.py` & `pyrfu-2.4.3/pyrfu/mms/remove_idist_background.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# 3rd party imports
-import numpy as np
-from scipy import constants
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2023"
-__license__ = "MIT"
-__version__ = "2.3.26"
-__status__ = "Prototype"
-
-
-def remove_idist_background(vdf, def_bg):
-    r"""Remove the mode background population due to penetrating radiation
-    `def_bg` from the ion velocity distribution function `vdf` using the
-    method from [1]_.
-
-    Parameters
-    ----------
-    vdf : xarray.Dataset
-        Ion velocity distribution function.
-    def_bg : xarray.DataArray
-        Omni-directional ion differential energy flux.
-
-    Returns
-    -------
-    vdf_new : xarray.Dataset
-        Ion velocity distribution function cleaned.
-
-    References
-    ----------
-    .. [1]  Gershman, D. J., Dorelli, J. C., Avanov,L. A., Gliese, U.,
-            Barrie, A., Schiff, C.,et al. (2019). Systematic uncertainties
-            in plasma parameters reported by the fast plasma investigation on
-            NASA's magnetospheric multiscale mission. Journal of Geophysical
-            Research: Space Physics, 124, https://doi.org/10.1029/2019JA026980
-
-    """
-
-    # Tile background flux to number of energy channels of the
-    # FPI-DIS instrument
-    def_bg_tmp = np.tile(def_bg.data[:, np.newaxis], (1, vdf.energy.shape[1]))
-
-    # Convert differential energy flux (cm^2 s sr)^{-1} of the background
-    # population (penetrating radiations) to phase-space density (s^3 m^{-6})
-    coeff = constants.proton_mass / (constants.elementary_charge * vdf.energy.data)
-    vdf_bg = def_bg_tmp.copy() * 1e4 / 2
-    vdf_bg *= coeff**2
-    vdf_bg /= 1e12
-
-    # Tile the background phase-space density to number of azimuthal
-    # and elevation angles channels of the FPI-DIS instrument
-    vdf_bg = np.tile(
-        vdf_bg[:, :, np.newaxis, np.newaxis],
-        (1, 1, vdf.phi.shape[1], vdf.theta.shape[0]),
-    )
-
-    vdf_new = vdf.copy()
-    vdf_new.data.data -= vdf_bg.data
-
-    return vdf_new
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# 3rd party imports
+import numpy as np
+from scipy import constants
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def remove_idist_background(vdf, def_bg):
+    r"""Remove the mode background population due to penetrating radiation
+    `def_bg` from the ion velocity distribution function `vdf` using the
+    method from [1]_.
+
+    Parameters
+    ----------
+    vdf : xarray.Dataset
+        Ion velocity distribution function.
+    def_bg : xarray.DataArray
+        Omni-directional ion differential energy flux.
+
+    Returns
+    -------
+    vdf_new : xarray.Dataset
+        Ion velocity distribution function cleaned.
+
+    References
+    ----------
+    .. [1]  Gershman, D. J., Dorelli, J. C., Avanov,L. A., Gliese, U.,
+            Barrie, A., Schiff, C.,et al. (2019). Systematic uncertainties
+            in plasma parameters reported by the fast plasma investigation on
+            NASA's magnetospheric multiscale mission. Journal of Geophysical
+            Research: Space Physics, 124, https://doi.org/10.1029/2019JA026980
+
+    """
+
+    # Tile background flux to number of energy channels of the
+    # FPI-DIS instrument
+    def_bg_tmp = np.tile(def_bg.data[:, np.newaxis], (1, vdf.energy.shape[1]))
+
+    # Convert differential energy flux (cm^2 s sr)^{-1} of the background
+    # population (penetrating radiations) to phase-space density (s^3 m^{-6})
+    coeff = constants.proton_mass / (constants.elementary_charge * vdf.energy.data)
+    vdf_bg = def_bg_tmp.copy() * 1e4 / 2
+    vdf_bg *= coeff**2
+    vdf_bg /= 1e12
+
+    # Tile the background phase-space density to number of azimuthal
+    # and elevation angles channels of the FPI-DIS instrument
+    vdf_bg = np.tile(
+        vdf_bg[:, :, np.newaxis, np.newaxis],
+        (1, 1, vdf.phi.shape[1], vdf.theta.shape[0]),
+    )
+
+    vdf_new = vdf.copy()
+    vdf_new.data.data -= vdf_bg.data
+
+    return vdf_new
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/scpot2ne.py` & `pyrfu-2.4.3/pyrfu/mms/scpot2ne.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from ..pyrf.resample import resample
 from ..pyrf.trace import trace
 from ..pyrf.ts_scalar import ts_scalar
 from ..pyrf.ts_tensor_xyz import ts_tensor_xyz
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def _f_one_pop(x, *args):
     i_e, i_aspoc, sc_pot_r = args
     return np.nansum(
         np.abs(
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/spectr_to_dataset.py` & `pyrfu-2.4.3/pyrfu/mms/spectr_to_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def spectr_to_dataset(spectr):
     r"""Convert energy spectrum (DataArray) to Dataset.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/tokenize.py` & `pyrfu-2.4.3/pyrfu/mms/tokenize.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # Built-in imports
 import warnings
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 all_params_scalars = [
     "ni",
     "nbgi",
     "pbgi",
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/vdf_elim.py` & `pyrfu-2.4.3/pyrfu/mms/vdf_elim.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Built-in imports
-import logging
-
-# 3rd party imports
-import numpy as np
-
-# Local imports
-from ..pyrf.ts_skymap import ts_skymap
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.33"
-__status__ = "Prototype"
-
-logging.captureWarnings(True)
-logging.basicConfig(
-    format="[%(asctime)s] %(levelname)s: %(message)s",
-    datefmt="%d-%b-%y %H:%M:%S",
-    level=logging.INFO,
-)
-
-
-def vdf_elim(vdf, e_int):
-    r"""Limits the skymap distribution to the selected energy range.
-
-    Parameters
-    ----------
-    vdf : xarray.Dataset
-        Skymap velocity distribution to clip.
-    e_int : list or float
-        Energy interval boundaries (list) or energy to slice.
-
-    Returns
-    -------
-    vdf_e_clipped : xarray.Dataset
-        Skymap of the clipped velocity distribution.
-
-    """
-
-    energy = vdf.energy
-    unique_etables = np.unique(vdf.energy, axis=0)
-    # n_etables = 2 for older dta and 1 for newer data
-    n_etables = unique_etables.shape[0]
-
-    e_int = list(np.atleast_1d(e_int))
-
-    # energy interval
-    if len(e_int) == 2:
-        e_levels = []
-
-        for i_etable in range(n_etables):
-            # loop over 1 or 2 and saves all the unique indices, i.e. max range
-            lower_ = e_int[0] < unique_etables[i_etable, :]
-            upper_ = unique_etables[i_etable, :] < e_int[1]
-            tmp_elevels = np.where(np.logical_and(lower_, upper_))[0]
-            e_levels = np.unique(np.hstack([e_levels, tmp_elevels]))
-
-        e_levels = list(e_levels.astype(np.int64))
-        e_min = np.min(energy.data[:, e_levels])
-        e_max = np.max(energy.data[:, e_levels])
-        logging.info(
-            "Effective eint = [%(e_min)5.2f, %(e_max)5.2f]",
-            {"e_min": e_min, "e_max": e_max},
-        )
-
-    else:
-        # pick closest energy level
-        e_diff0 = np.abs(energy[0, :] - e_int)
-        e_diff1 = np.abs(energy[1, :] - e_int)
-        if np.min(e_diff0) < np.min(e_diff1):
-            e_diff = e_diff0
-        else:
-            e_diff = e_diff1
-
-        e_levels = int(np.where(e_diff == np.min(e_diff))[0][0])
-        logging.info(
-            "Effective energies alternate in time between %(e0)5.2f and %(e1)5.2f",
-            {"e0": energy.data[0, e_levels], "e1": energy.data[1, e_levels]},
-        )
-
-    # Data attributes
-    data_attrs = vdf.data.attrs
-
-    # Coordinates attributes
-    coords_attrs = {k: vdf[k].attrs for k in ["time", "energy", "phi", "theta"]}
-
-    # Global attributes
-    glob_attrs = vdf.attrs
-
-    # Get energies levels
-    energy_0 = glob_attrs.get("energy0", unique_etables[0, :])[e_levels]
-    energy_1 = glob_attrs.get("energy1", unique_etables[0, :])[e_levels]
-    esteptable = glob_attrs.get("esteptable", np.zeros(len(vdf.time)))
-
-    vdf_e_clipped = ts_skymap(
-        vdf.time.data,
-        vdf.data.data[:, e_levels, ...],
-        energy=energy.data[:, e_levels],
-        phi=vdf.phi.data,
-        theta=vdf.theta.data,
-        energy0=energy_0,
-        energy1=energy_1,
-        esteptable=esteptable,
-        attrs=data_attrs,
-        coords_attrs=coords_attrs,
-        glob_attrs=glob_attrs,
-    )
-
-    return vdf_e_clipped
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# Built-in imports
+import logging
+
+# 3rd party imports
+import numpy as np
+
+# Local imports
+from ..pyrf.ts_skymap import ts_skymap
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+logging.captureWarnings(True)
+logging.basicConfig(
+    format="[%(asctime)s] %(levelname)s: %(message)s",
+    datefmt="%d-%b-%y %H:%M:%S",
+    level=logging.INFO,
+)
+
+
+def vdf_elim(vdf, e_int):
+    r"""Limits the skymap distribution to the selected energy range.
+
+    Parameters
+    ----------
+    vdf : xarray.Dataset
+        Skymap velocity distribution to clip.
+    e_int : list or float
+        Energy interval boundaries (list) or energy to slice.
+
+    Returns
+    -------
+    vdf_e_clipped : xarray.Dataset
+        Skymap of the clipped velocity distribution.
+
+    """
+
+    energy = vdf.energy
+    unique_etables = np.unique(vdf.energy, axis=0)
+    # n_etables = 2 for older dta and 1 for newer data
+    n_etables = unique_etables.shape[0]
+
+    e_int = list(np.atleast_1d(e_int))
+
+    # energy interval
+    if len(e_int) == 2:
+        e_levels = []
+
+        for i_etable in range(n_etables):
+            # loop over 1 or 2 and saves all the unique indices, i.e. max range
+            lower_ = e_int[0] < unique_etables[i_etable, :]
+            upper_ = unique_etables[i_etable, :] < e_int[1]
+            tmp_elevels = np.where(np.logical_and(lower_, upper_))[0]
+            e_levels = np.unique(np.hstack([e_levels, tmp_elevels]))
+
+        e_levels = list(e_levels.astype(np.int64))
+        e_min = np.min(energy.data[:, e_levels])
+        e_max = np.max(energy.data[:, e_levels])
+        logging.info(
+            "Effective eint = [%(e_min)5.2f, %(e_max)5.2f]",
+            {"e_min": e_min, "e_max": e_max},
+        )
+
+    else:
+        # pick closest energy level
+        e_diff0 = np.abs(energy[0, :] - e_int)
+        e_diff1 = np.abs(energy[1, :] - e_int)
+        if np.min(e_diff0) < np.min(e_diff1):
+            e_diff = e_diff0
+        else:
+            e_diff = e_diff1
+
+        e_levels = int(np.where(e_diff == np.min(e_diff))[0][0])
+        logging.info(
+            "Effective energies alternate in time between %(e0)5.2f and %(e1)5.2f",
+            {"e0": energy.data[0, e_levels], "e1": energy.data[1, e_levels]},
+        )
+
+    # Data attributes
+    data_attrs = vdf.data.attrs
+
+    # Coordinates attributes
+    coords_attrs = {k: vdf[k].attrs for k in ["time", "energy", "phi", "theta"]}
+
+    # Global attributes
+    glob_attrs = vdf.attrs
+
+    # Get energies levels
+    energy_0 = glob_attrs.get("energy0", unique_etables[0, :])[e_levels]
+    energy_1 = glob_attrs.get("energy1", unique_etables[0, :])[e_levels]
+    esteptable = glob_attrs.get("esteptable", np.zeros(len(vdf.time)))
+
+    vdf_e_clipped = ts_skymap(
+        vdf.time.data,
+        vdf.data.data[:, e_levels, ...],
+        energy=energy.data[:, e_levels],
+        phi=vdf.phi.data,
+        theta=vdf.theta.data,
+        energy0=energy_0,
+        energy1=energy_1,
+        esteptable=esteptable,
+        attrs=data_attrs,
+        coords_attrs=coords_attrs,
+        glob_attrs=glob_attrs,
+    )
+
+    return vdf_e_clipped
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/vdf_omni.py` & `pyrfu-2.4.3/pyrfu/mms/vdf_omni.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def vdf_omni(vdf, method: str = "mean"):
     r"""Computes omni-directional distribution, without changing the units.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/vdf_reduce.py` & `pyrfu-2.4.3/pyrfu/mms/vdf_reduce.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,290 +1,290 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# 3rd party imports
-import numpy as np
-import xarray as xr
-from scipy import constants, interpolate
-
-# Local imports
-from pyrfu.pyrf import cart2sph, resample, sph2cart, time_clip
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2022"
-__license__ = "MIT"
-__version__ = "2.3.12"
-__status__ = "Prototype"
-
-__all__ = ["vdf_frame_transformation", "vdf_reduce"]
-
-
-def _interp_skymap_sphe(vdf, energy, phi, theta, grid_sphe):
-    r"""Interpolate the skymap distribution defined on the grid (`energy`,
-    `phi`, `theta`) onto the spherical grid `grid_sphe`.
-
-    Parameters
-    ----------
-    vdf : numpy.ndarray
-        Values of the skymap distribution.
-    energy : numpy.ndarray
-        Energy level of skymap sampling.
-    phi : numpy.ndarray
-        Azimuthal angle of skymap sampling.
-    theta : numpy.ndarray
-        Elevation angle of skymap sampling.
-    grid_sphe : numpy.ndarray
-        Spherical velocity grid to interpolate on (3xlxmxn).
-
-    Returns
-    -------
-    out_data : numpy.ndarray
-        Values of the distribution interpolated onto `grdi_sphe`.
-
-    Notes
-    -----
-    The values corresponding to energy levels below the instrument range are
-    discarded.
-
-    """
-
-    phi_period = np.zeros(len(phi) + 2)
-    phi_period[1:-1] = phi
-    phi_period[0] = phi[-1] - 2 * 180.0
-    phi_period[-1] = phi[0] + 2 * 180.0
-
-    theta_period = np.zeros(len(theta) + 2)
-    theta_period[1:-1] = theta
-    theta_period[0] = theta[-1] - 180.0
-    theta_period[-1] = theta[0] + 180.0
-
-    vdf_period = np.zeros((len(energy), len(phi) + 2, len(theta) + 2))
-    vdf_period[:, 1:-1, 1:-1] = vdf
-    vdf_period[:, 1:-1, 0] = vdf[:, :, -1]
-    vdf_period[:, 1:-1, -1] = vdf[:, :, 0]
-    vdf_period[:, 0] = vdf_period[:, 1]
-    vdf_period[:, -1] = vdf_period[:, -2]
-
-    vdf_interp = interpolate.RegularGridInterpolator(
-        (energy, phi_period, theta_period),
-        vdf_period,
-        method="linear",
-        bounds_error=False,
-        fill_value=None,
-    )
-
-    out_data = vdf_interp(grid_sphe)
-
-    return out_data
-
-
-def _interp_skymap_cart(vdf, energy, phi, theta, grid_cart):
-    r"""Interpolate the skymap distribution defined on the grid (`energy`,
-    `phi`, `theta`) onto the cartesian grid `grid_cart`.
-
-    Parameters
-    ----------
-    vdf : numpy.ndarray
-        Values of the skymap distribution.
-    energy : numpy.ndarray
-        Energy level of skymap sampling.
-    phi : numpy.ndarray
-        Azimuthal angle of skymap sampling.
-    theta : numpy.ndarray
-        Elevation angle of skymap sampling.
-    grid_cart : numpy.ndarray
-        Cartesian velocity grid to interpolate on (3xlxmxn).
-
-    Returns
-    -------
-    out_data : numpy.ndarray
-        Values of the distribution interpolated onto `grid_cart`.
-
-    Notes
-    -----
-    The values corresponding to energy levels below the instrument range are
-    discarded.
-
-    See Also
-    --------
-    _inter_skymap_sphe.py
-    """
-
-    # Unpack cartesian grid
-    v_x, v_y, v_z = grid_cart
-
-    # Transform cartesian velocity grid to spherical velocity grid
-    phi_grid, theta_grid, speed_grid = cart2sph(v_x, v_y, v_z)
-    energy_grid = (
-        0.5 * constants.proton_mass * speed_grid**2 / constants.elementary_charge
-    )
-    phi_grid = np.rad2deg(phi_grid) + 180.0
-    theta_grid = np.rad2deg(theta_grid)
-
-    grid_sphe = np.transpose(
-        np.stack([energy_grid, phi_grid, theta_grid]),
-        [1, 2, 3, 0],
-    )
-
-    # Interpolate the skymap distribution onto the spherical grid
-    out_data = _interp_skymap_sphe(vdf, energy, phi, theta, grid_sphe)
-
-    # Discard points with energy below the instrument energy range.
-    v_min_2 = 2 * energy[0] * constants.electron_volt / constants.proton_mass
-    out_data[v_x**2 + v_y**2 + v_z**2 < v_min_2] = np.nan
-
-    return out_data
-
-
-def vdf_frame_transformation(vdf, v_gse):
-    r"""Move the skymap into the desired frame associated with the bulk
-    velocity `v_gse`.
-
-    Parameters
-    ----------
-    vdf : xarray.Dataset
-        Skymap distribution in the initial frame.
-    v_gse : xarray.DataArray
-        Time series of the bulk velocity to shift.
-
-    Returns
-    -------
-    out : xarray.Dataset
-        Skymap distribution into the new frame.
-
-    Notes
-    -----
-    The new skymap grid is identical to the original one. The bulk velocity
-    must be in the same coordinates system as the skymap (i.e spacecraft for
-    FPI and GSE for EIS)
-
-    See Also
-    --------
-    _interp_skymap_cart.py, _interp_skymap_sphe.py
-
-    """
-
-    v_gse = resample(v_gse, vdf.time)
-    theta = vdf.theta.data
-
-    out_data = np.zeros_like(vdf.data.data)
-
-    for i in range(len(vdf.time.data)):
-        vdf_data = vdf.data.data[i, :]
-        energy = vdf.energy.data[i, :]
-        phi = vdf.phi.data[i, :]
-
-        phi_mat, en_mat, theta_mat = np.meshgrid(phi, energy, theta)
-        v_mat = np.sqrt(
-            2 * en_mat * constants.electron_volt / constants.proton_mass,
-        )
-        v_xyz = sph2cart(np.deg2rad(phi_mat), np.deg2rad(theta_mat), v_mat)
-
-        grid_cart = np.stack(
-            [
-                v_xyz[0] - v_gse.data[i, 0, None, None, None],
-                v_xyz[1] - v_gse.data[i, 1, None, None, None],
-                v_xyz[2] - v_gse.data[i, 2, None, None, None],
-            ],
-        )
-
-        out_data[i, ...] = _interp_skymap_cart(
-            vdf_data,
-            energy,
-            phi,
-            theta,
-            grid_cart,
-        )
-
-    out = vdf.copy()
-    out.data.data = out_data
-
-    return out
-
-
-def vdf_reduce(
-    vdf,
-    tint,
-    dim,
-    x_vec,
-    z_vec: list = None,
-    v_int: list = None,
-    n_vpt: int = 100,
-):
-    r"""Interpolate the skymap distribution onto the velocity grid defined
-    by the velocity interval `v_int` along the axes `x_vec` and `z_vec`,
-    and reduce (integrate) it along 1 (if `dim` is "2d") or 2 (if `dim` is
-    "1d").
-
-    Parameters
-    ----------
-    vdf : xarray.Dataset
-        Skymap distribution to reduce.
-    tint : list of strs
-        Time interval over which the time series of the skymap distribution
-        is averaged.
-    dim : {"1d", "2d"}
-        Dimension of the output reduced distribution.
-    x_vec : array_like
-        X axis. For the "1d" case, it is the axis on which the skymap is
-        plotted. For the "2d" case, it is the first of the two axes on which
-        the skymap is plotted.
-    z_vec : array_like, Optional
-        Axis along which the skymap is integrated. Needed only for the "2d"
-        case.
-    v_int : array_like, Optional
-        Velocity interval.
-    n_vpt : int, Optional
-        Number of points along the plot direction(s).
-
-    Returns
-    -------
-    out : xarray.DataArray
-        Reduced distribution.
-
-    """
-
-    if v_int is None:
-        v_int = [-1e6, 1e6]
-    if z_vec is None:
-        z_vec = [0, 0, 1]
-
-    x_vec = x_vec / np.linalg.norm(x_vec, keepdims=True)
-    y_vec = np.cross(z_vec, x_vec)
-    y_vec = y_vec / np.linalg.norm(y_vec, keepdims=True)
-    z_vec = np.cross(x_vec, y_vec)
-    z_vec = z_vec / np.linalg.norm(z_vec, keepdims=True)
-
-    v_x, v_y, v_z = [np.linspace(v_int[0], v_int[1], n_vpt) for _ in range(3)]
-
-    m_vec = np.transpose([x_vec, y_vec, z_vec])
-    v_x, v_y, v_z = np.matmul(np.linalg.inv(m_vec), np.array([v_x, v_y, v_z]))
-    v_x_mat, v_y_mat, v_z_mat = np.meshgrid(v_x, v_y, v_z)
-    grid_cart = np.stack([v_x_mat, v_y_mat, v_z_mat])
-
-    vdf = time_clip(vdf, tint)
-
-    vdf_data = np.mean(vdf.data.data, axis=0)
-    energy = np.mean(np.atleast_2d(vdf.energy.data), axis=0)
-    phi = np.mean(np.atleast_2d(vdf.phi.data), axis=0)
-    theta = vdf.theta.data
-
-    interp_vdf = _interp_skymap_cart(vdf_data, energy, phi, theta, grid_cart)
-
-    if dim.lower() == "2d":
-        dv_ = np.abs(np.diff(v_z)[0])
-        red_vdf = np.nansum(interp_vdf, axis=-1) * dv_
-        out = xr.DataArray(
-            red_vdf,
-            coords=[v_x / 1e6, v_y / 1e6],
-            dims=["vx", "vy"],
-        )
-    elif dim.lower() == "1d":
-        dv_ = np.abs(np.diff(v_y)[0] * np.diff(v_z)[0])
-        red_vdf = np.nansum(np.sum(interp_vdf, axis=-1), axis=-1) * dv_
-        out = xr.DataArray(red_vdf, coords=[v_x / 1e6], dims=["vx"])
-
-    else:
-        raise ValueError
-
-    return out
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# 3rd party imports
+import numpy as np
+import xarray as xr
+from scipy import constants, interpolate
+
+# Local imports
+from pyrfu.pyrf import cart2sph, resample, sph2cart, time_clip
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+__all__ = ["vdf_frame_transformation", "vdf_reduce"]
+
+
+def _interp_skymap_sphe(vdf, energy, phi, theta, grid_sphe):
+    r"""Interpolate the skymap distribution defined on the grid (`energy`,
+    `phi`, `theta`) onto the spherical grid `grid_sphe`.
+
+    Parameters
+    ----------
+    vdf : numpy.ndarray
+        Values of the skymap distribution.
+    energy : numpy.ndarray
+        Energy level of skymap sampling.
+    phi : numpy.ndarray
+        Azimuthal angle of skymap sampling.
+    theta : numpy.ndarray
+        Elevation angle of skymap sampling.
+    grid_sphe : numpy.ndarray
+        Spherical velocity grid to interpolate on (3xlxmxn).
+
+    Returns
+    -------
+    out_data : numpy.ndarray
+        Values of the distribution interpolated onto `grdi_sphe`.
+
+    Notes
+    -----
+    The values corresponding to energy levels below the instrument range are
+    discarded.
+
+    """
+
+    phi_period = np.zeros(len(phi) + 2)
+    phi_period[1:-1] = phi
+    phi_period[0] = phi[-1] - 2 * 180.0
+    phi_period[-1] = phi[0] + 2 * 180.0
+
+    theta_period = np.zeros(len(theta) + 2)
+    theta_period[1:-1] = theta
+    theta_period[0] = theta[-1] - 180.0
+    theta_period[-1] = theta[0] + 180.0
+
+    vdf_period = np.zeros((len(energy), len(phi) + 2, len(theta) + 2))
+    vdf_period[:, 1:-1, 1:-1] = vdf
+    vdf_period[:, 1:-1, 0] = vdf[:, :, -1]
+    vdf_period[:, 1:-1, -1] = vdf[:, :, 0]
+    vdf_period[:, 0] = vdf_period[:, 1]
+    vdf_period[:, -1] = vdf_period[:, -2]
+
+    vdf_interp = interpolate.RegularGridInterpolator(
+        (energy, phi_period, theta_period),
+        vdf_period,
+        method="linear",
+        bounds_error=False,
+        fill_value=None,
+    )
+
+    out_data = vdf_interp(grid_sphe)
+
+    return out_data
+
+
+def _interp_skymap_cart(vdf, energy, phi, theta, grid_cart):
+    r"""Interpolate the skymap distribution defined on the grid (`energy`,
+    `phi`, `theta`) onto the cartesian grid `grid_cart`.
+
+    Parameters
+    ----------
+    vdf : numpy.ndarray
+        Values of the skymap distribution.
+    energy : numpy.ndarray
+        Energy level of skymap sampling.
+    phi : numpy.ndarray
+        Azimuthal angle of skymap sampling.
+    theta : numpy.ndarray
+        Elevation angle of skymap sampling.
+    grid_cart : numpy.ndarray
+        Cartesian velocity grid to interpolate on (3xlxmxn).
+
+    Returns
+    -------
+    out_data : numpy.ndarray
+        Values of the distribution interpolated onto `grid_cart`.
+
+    Notes
+    -----
+    The values corresponding to energy levels below the instrument range are
+    discarded.
+
+    See Also
+    --------
+    _inter_skymap_sphe.py
+    """
+
+    # Unpack cartesian grid
+    v_x, v_y, v_z = grid_cart
+
+    # Transform cartesian velocity grid to spherical velocity grid
+    phi_grid, theta_grid, speed_grid = cart2sph(v_x, v_y, v_z)
+    energy_grid = (
+        0.5 * constants.proton_mass * speed_grid**2 / constants.elementary_charge
+    )
+    phi_grid = np.rad2deg(phi_grid) + 180.0
+    theta_grid = np.rad2deg(theta_grid)
+
+    grid_sphe = np.transpose(
+        np.stack([energy_grid, phi_grid, theta_grid]),
+        [1, 2, 3, 0],
+    )
+
+    # Interpolate the skymap distribution onto the spherical grid
+    out_data = _interp_skymap_sphe(vdf, energy, phi, theta, grid_sphe)
+
+    # Discard points with energy below the instrument energy range.
+    v_min_2 = 2 * energy[0] * constants.electron_volt / constants.proton_mass
+    out_data[v_x**2 + v_y**2 + v_z**2 < v_min_2] = np.nan
+
+    return out_data
+
+
+def vdf_frame_transformation(vdf, v_gse):
+    r"""Move the skymap into the desired frame associated with the bulk
+    velocity `v_gse`.
+
+    Parameters
+    ----------
+    vdf : xarray.Dataset
+        Skymap distribution in the initial frame.
+    v_gse : xarray.DataArray
+        Time series of the bulk velocity to shift.
+
+    Returns
+    -------
+    out : xarray.Dataset
+        Skymap distribution into the new frame.
+
+    Notes
+    -----
+    The new skymap grid is identical to the original one. The bulk velocity
+    must be in the same coordinates system as the skymap (i.e spacecraft for
+    FPI and GSE for EIS)
+
+    See Also
+    --------
+    _interp_skymap_cart.py, _interp_skymap_sphe.py
+
+    """
+
+    v_gse = resample(v_gse, vdf.time)
+    theta = vdf.theta.data
+
+    out_data = np.zeros_like(vdf.data.data)
+
+    for i in range(len(vdf.time.data)):
+        vdf_data = vdf.data.data[i, :]
+        energy = vdf.energy.data[i, :]
+        phi = vdf.phi.data[i, :]
+
+        phi_mat, en_mat, theta_mat = np.meshgrid(phi, energy, theta)
+        v_mat = np.sqrt(
+            2 * en_mat * constants.electron_volt / constants.proton_mass,
+        )
+        v_xyz = sph2cart(np.deg2rad(phi_mat), np.deg2rad(theta_mat), v_mat)
+
+        grid_cart = np.stack(
+            [
+                v_xyz[0] - v_gse.data[i, 0, None, None, None],
+                v_xyz[1] - v_gse.data[i, 1, None, None, None],
+                v_xyz[2] - v_gse.data[i, 2, None, None, None],
+            ],
+        )
+
+        out_data[i, ...] = _interp_skymap_cart(
+            vdf_data,
+            energy,
+            phi,
+            theta,
+            grid_cart,
+        )
+
+    out = vdf.copy()
+    out.data.data = out_data
+
+    return out
+
+
+def vdf_reduce(
+    vdf,
+    tint,
+    dim,
+    x_vec,
+    z_vec: list = None,
+    v_int: list = None,
+    n_vpt: int = 100,
+):
+    r"""Interpolate the skymap distribution onto the velocity grid defined
+    by the velocity interval `v_int` along the axes `x_vec` and `z_vec`,
+    and reduce (integrate) it along 1 (if `dim` is "2d") or 2 (if `dim` is
+    "1d").
+
+    Parameters
+    ----------
+    vdf : xarray.Dataset
+        Skymap distribution to reduce.
+    tint : list of strs
+        Time interval over which the time series of the skymap distribution
+        is averaged.
+    dim : {"1d", "2d"}
+        Dimension of the output reduced distribution.
+    x_vec : array_like
+        X axis. For the "1d" case, it is the axis on which the skymap is
+        plotted. For the "2d" case, it is the first of the two axes on which
+        the skymap is plotted.
+    z_vec : array_like, Optional
+        Axis along which the skymap is integrated. Needed only for the "2d"
+        case.
+    v_int : array_like, Optional
+        Velocity interval.
+    n_vpt : int, Optional
+        Number of points along the plot direction(s).
+
+    Returns
+    -------
+    out : xarray.DataArray
+        Reduced distribution.
+
+    """
+
+    if v_int is None:
+        v_int = [-1e6, 1e6]
+    if z_vec is None:
+        z_vec = [0, 0, 1]
+
+    x_vec = x_vec / np.linalg.norm(x_vec, keepdims=True)
+    y_vec = np.cross(z_vec, x_vec)
+    y_vec = y_vec / np.linalg.norm(y_vec, keepdims=True)
+    z_vec = np.cross(x_vec, y_vec)
+    z_vec = z_vec / np.linalg.norm(z_vec, keepdims=True)
+
+    v_x, v_y, v_z = [np.linspace(v_int[0], v_int[1], n_vpt) for _ in range(3)]
+
+    m_vec = np.transpose([x_vec, y_vec, z_vec])
+    v_x, v_y, v_z = np.matmul(np.linalg.inv(m_vec), np.array([v_x, v_y, v_z]))
+    v_x_mat, v_y_mat, v_z_mat = np.meshgrid(v_x, v_y, v_z)
+    grid_cart = np.stack([v_x_mat, v_y_mat, v_z_mat])
+
+    vdf = time_clip(vdf, tint)
+
+    vdf_data = np.mean(vdf.data.data, axis=0)
+    energy = np.mean(np.atleast_2d(vdf.energy.data), axis=0)
+    phi = np.mean(np.atleast_2d(vdf.phi.data), axis=0)
+    theta = vdf.theta.data
+
+    interp_vdf = _interp_skymap_cart(vdf_data, energy, phi, theta, grid_cart)
+
+    if dim.lower() == "2d":
+        dv_ = np.abs(np.diff(v_z)[0])
+        red_vdf = np.nansum(interp_vdf, axis=-1) * dv_
+        out = xr.DataArray(
+            red_vdf,
+            coords=[v_x / 1e6, v_y / 1e6],
+            dims=["vx", "vy"],
+        )
+    elif dim.lower() == "1d":
+        dv_ = np.abs(np.diff(v_y)[0] * np.diff(v_z)[0])
+        red_vdf = np.nansum(np.sum(interp_vdf, axis=-1), axis=-1) * dv_
+        out = xr.DataArray(red_vdf, coords=[v_x / 1e6], dims=["vx"])
+
+    else:
+        raise ValueError
+
+    return out
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/vdf_to_e64.py` & `pyrfu-2.4.3/pyrfu/mms/vdf_to_e64.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from ..pyrf.ts_skymap import ts_skymap
 
 # Local imports
 from .psd_rebin import psd_rebin
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.33"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def vdf_to_e64(vdf_e32):
     r"""Recompile data into 64 energy channels. Time resolution is halved.
     Only applies to skymap.
```

### Comparing `pyrfu-2.4.1/pyrfu/mms/whistler_b2e.py` & `pyrfu-2.4.3/pyrfu/mms/whistler_b2e.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from scipy import constants
 
 # Local imports
 from ..pyrf.plasma_calc import plasma_calc
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def whistler_b2e(b2, freq, theta_k, b_mag, n_e):
     r"""Computes electric field power as a function of frequency for whistler
     waves using magnetic field power and cold plasma theory.
```

### Comparing `pyrfu-2.4.1/pyrfu/models/igrf13coeffs.csv` & `pyrfu-2.4.3/pyrfu/models/igrf13coeffs.csv`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/pyrfu/models/magnetopause_normal.py` & `pyrfu-2.4.3/pyrfu/models/magnetopause_normal.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,197 +1,197 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Built-in imports
-import warnings
-
-# 3rd party imports
-import numpy as np
-from scipy.optimize import fminbound
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2022"
-__license__ = "MIT"
-__version__ = "2.3.22"
-__status__ = "Prototype"
-
-
-def _magnetopause(theta, *args):
-    r0, alpha, x0, y0 = args
-    out = (
-        r0**2 * (2.0 / (1 + np.cos(theta))) ** (2 * alpha)
-        - 2
-        * r0
-        * (2.0 / (1 + np.cos(theta))) ** alpha
-        * (x0 * np.cos(theta) + y0 * np.sin(theta))
-        + x0**2
-        + y0**2
-    )
-
-    return out
-
-
-def _bow_shock(r_xy, *args):
-    x, y = r_xy
-    x0, y0 = args
-    out = (x - x0) ** 2 + (y - y0) ** 2
-    return out
-
-
-def magnetopause_normal(
-    r_gsm,
-    b_z_imf,
-    p_sw,
-    model: str = "mp_shue1997",
-    m_alfven: float = 4.0,
-):
-    r"""Computes the distance and normal vector to the magnetopause for
-    Shue et al., 1997 or Shue et al., 1998 model. Or bow shock for
-    Farris & Russell 1994 model.
-
-    Parameters
-    ----------
-    r_gsm : array_like
-        GSM position in Re (if more than 3 values assumes that 1st is time).
-    b_z_imf : float
-        IMF Bz in nT.
-    p_sw : float
-        Solar wind dynamic pressure in nPa.
-    model : {"mp_shue1997", "mp_shue1998", "bs97", "bs98"}, Optional
-        Name of model :
-            * 'mp_shue1997' : Shue et al., 1997 (Default)
-            * 'mp_shue1998' : Shue et al., 1998
-            * 'bs97'        : Bow shock, Farris & Russell 1994
-            * 'bs98'        : Bow shock, Farris & Russell 1994
-    m_alfven : float, Optional
-        Alfvenic Mach number, only needed if bow shock model is used.
-
-    Returns
-    -------
-    mindist : float
-        Minimum distance to the magnetopause, in Re. Positive value if
-        spacecraft is inside the magnetopause, negative if outside the
-        magnetopause.
-    n_vec : numpy.ndarray
-        Normal vector to the magnetopause (pointing away from Earth).
-
-
-    References
-    ----------
-    .. [1]  J.-H. Shue, J. K. Chao, H. C. Fu, C. T. Russell, P. Song,
-            K. K. Khurana, and H. J. Singer (1997), A new functional form to
-            study the solar wind control of the magnetopause size and shape,
-            J. Geophys. Res., 102, 9497, doi: https://doi.org/10.1029/97JA00196
-
-    .. [2]  J.-H. Shue, P. Song, C. T. Russell, J. T. Steinberg, J. K. Chao,
-            G. Zastenker, O. L. Vaisber, S. Kokubun, H. J. Singer,
-            T. R. Detman and H. Kawano (1998), Magnetopause location under
-            extreme solar wind conditions, J. Geophys. Res., 103(A8), 17,
-            691–17,700, doi: https://doi.org/10.1029/98JA01103
-
-    .. [3]  M. H. Farris and C. T. Russell (1994), Determining the standoff
-            distance of the bow shock: Mach number dependence and use of
-            models, J. Geophys. Res., 99, 17681.
-            doi: https://doi.org/10.1029/94JA01020
-
-    """
-
-    if model in ["mp_shue1998", "bs98"]:
-        alpha = (0.58 - 0.007 * b_z_imf) * (1.0 + 0.024 * np.log(p_sw))
-        r0 = 10.22 + 1.29 * np.tanh(0.184 * (b_z_imf + 8.14))
-        r0 *= p_sw ** (-1.0 / 6.6)
-        warnings.warn("Shue et al., 1998 model used.", UserWarning)
-    else:
-        alpha = (0.58 - 0.01 * b_z_imf) * (1.0 + 0.01 * p_sw)
-
-        if b_z_imf >= 0:
-            r0 = (11.4 + 0.013 * b_z_imf) * p_sw ** (-1.0 / 6.6)
-        else:
-            r0 = (11.4 + 0.140 * b_z_imf) * p_sw ** (-1.0 / 6.6)
-
-        warnings.warn("Shue et al., 1997 model used.", UserWarning)
-
-    # Spacecraft position
-    r1_x, r1_y, r1_z = r_gsm
-    r0_x, r0_y = [r1_x, np.sqrt(r1_y**2 + r1_z**2)]
-
-    if model[:2].lower() == "mp":
-        # Magnetopause
-
-        theta_min, min_val, _, _ = fminbound(
-            _magnetopause,
-            x1=-np.pi / 2,
-            x2=np.pi / 2,
-            args=(r0, alpha, r0_x, r1_y),
-            full_output=True,
-        )
-
-        min_dist = np.sqrt(min_val)
-
-        # calculate the direction to the spacecraft normal to the magnetopause
-        x_n = r0 * (2 / (1 + np.cos(theta_min))) ** alpha * np.cos(theta_min) - r1_x
-        phi = np.arctan2(r1_z, r1_y)
-        y_n = (
-            np.cos(phi)
-            * (r0 * (2 / (1 + np.cos(theta_min))) ** alpha * np.sin(theta_min))
-            - r1_y
-        )
-        z_n = (
-            np.sin(phi)
-            * (r0 * (2 / (1 + np.cos(theta_min))) ** alpha * np.sin(theta_min))
-            - r1_z
-        )
-
-        n_vec = np.stack([x_n, y_n, z_n]) / min_dist
-
-        # if statement to ensure normal is pointing away from Earth
-        if np.sqrt(r0_x**2 + r0_y**2) > r0 * (2 / (1 + np.cos(theta_min))) ** alpha:
-            n_vec *= -1
-            min_dist *= -1
-
-    else:
-        # Bow shock
-        warnings.warn(
-            "Farris & Russell 1994 bow shock model used.",
-            UserWarning,
-        )
-
-        gamma = 5 / 3
-        mach = m_alfven
-
-        # Bow shock standoff distance
-        rbs = r0 * (
-            1 + 1.1 * ((gamma - 1) * mach**2 + 2) / ((gamma + 1) * (mach**2 - 1))
-        )
-
-        # y ^ 2 = 0 - Ax + Bx ^ 2
-        coeffs = [0, 45.3, 0.04]
-        x = np.linspace(rbs, -100, int((rbs + 100) * 1e3) + 1)
-        y = np.sqrt(-coeffs[1] * (x - rbs) + coeffs[2] * (x - rbs) ** 2)
-        x = np.hstack([np.flip(x), x])
-        y = np.hstack([-np.flip(y), y])
-
-        r_xy = np.transpose(np.stack([x, y]))
-        args_bow_shock = (r0_x, r0_y)
-
-        min_val = np.min(_bow_shock(r_xy, *args_bow_shock))
-        min_pos = np.argmin(_bow_shock(r_xy, *args_bow_shock))
-
-        d_vec = np.stack([x - r0_x, y - r0_y])
-        d_min = d_vec[min_pos, :]
-
-        x_n = d_min[0] / np.linalg.norm(d_min)
-        min_dist = np.sqrt(min_val)
-
-        qyz = r1_y / r1_z
-        z_n = np.sign(r1_z) * np.sign(x_n) * np.sqrt((1 - x_n**2) / (1 + qyz**2))
-        y_n = z_n * qyz
-
-        n_vec = np.stack([x_n, y_n, z_n])
-
-        # if statement to ensure normal is pointing away from Earth
-        if n_vec[0] < 0:
-            n_vec *= -1
-            min_dist *= -1
-
-    return min_dist, n_vec
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# Built-in imports
+import warnings
+
+# 3rd party imports
+import numpy as np
+from scipy.optimize import fminbound
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def _magnetopause(theta, *args):
+    r0, alpha, x0, y0 = args
+    out = (
+        r0**2 * (2.0 / (1 + np.cos(theta))) ** (2 * alpha)
+        - 2
+        * r0
+        * (2.0 / (1 + np.cos(theta))) ** alpha
+        * (x0 * np.cos(theta) + y0 * np.sin(theta))
+        + x0**2
+        + y0**2
+    )
+
+    return out
+
+
+def _bow_shock(r_xy, *args):
+    x, y = r_xy
+    x0, y0 = args
+    out = (x - x0) ** 2 + (y - y0) ** 2
+    return out
+
+
+def magnetopause_normal(
+    r_gsm,
+    b_z_imf,
+    p_sw,
+    model: str = "mp_shue1997",
+    m_alfven: float = 4.0,
+):
+    r"""Computes the distance and normal vector to the magnetopause for
+    Shue et al., 1997 or Shue et al., 1998 model. Or bow shock for
+    Farris & Russell 1994 model.
+
+    Parameters
+    ----------
+    r_gsm : array_like
+        GSM position in Re (if more than 3 values assumes that 1st is time).
+    b_z_imf : float
+        IMF Bz in nT.
+    p_sw : float
+        Solar wind dynamic pressure in nPa.
+    model : {"mp_shue1997", "mp_shue1998", "bs97", "bs98"}, Optional
+        Name of model :
+            * 'mp_shue1997' : Shue et al., 1997 (Default)
+            * 'mp_shue1998' : Shue et al., 1998
+            * 'bs97'        : Bow shock, Farris & Russell 1994
+            * 'bs98'        : Bow shock, Farris & Russell 1994
+    m_alfven : float, Optional
+        Alfvenic Mach number, only needed if bow shock model is used.
+
+    Returns
+    -------
+    mindist : float
+        Minimum distance to the magnetopause, in Re. Positive value if
+        spacecraft is inside the magnetopause, negative if outside the
+        magnetopause.
+    n_vec : numpy.ndarray
+        Normal vector to the magnetopause (pointing away from Earth).
+
+
+    References
+    ----------
+    .. [1]  J.-H. Shue, J. K. Chao, H. C. Fu, C. T. Russell, P. Song,
+            K. K. Khurana, and H. J. Singer (1997), A new functional form to
+            study the solar wind control of the magnetopause size and shape,
+            J. Geophys. Res., 102, 9497, doi: https://doi.org/10.1029/97JA00196
+
+    .. [2]  J.-H. Shue, P. Song, C. T. Russell, J. T. Steinberg, J. K. Chao,
+            G. Zastenker, O. L. Vaisber, S. Kokubun, H. J. Singer,
+            T. R. Detman and H. Kawano (1998), Magnetopause location under
+            extreme solar wind conditions, J. Geophys. Res., 103(A8), 17,
+            691–17,700, doi: https://doi.org/10.1029/98JA01103
+
+    .. [3]  M. H. Farris and C. T. Russell (1994), Determining the standoff
+            distance of the bow shock: Mach number dependence and use of
+            models, J. Geophys. Res., 99, 17681.
+            doi: https://doi.org/10.1029/94JA01020
+
+    """
+
+    if model in ["mp_shue1998", "bs98"]:
+        alpha = (0.58 - 0.007 * b_z_imf) * (1.0 + 0.024 * np.log(p_sw))
+        r0 = 10.22 + 1.29 * np.tanh(0.184 * (b_z_imf + 8.14))
+        r0 *= p_sw ** (-1.0 / 6.6)
+        warnings.warn("Shue et al., 1998 model used.", UserWarning)
+    else:
+        alpha = (0.58 - 0.01 * b_z_imf) * (1.0 + 0.01 * p_sw)
+
+        if b_z_imf >= 0:
+            r0 = (11.4 + 0.013 * b_z_imf) * p_sw ** (-1.0 / 6.6)
+        else:
+            r0 = (11.4 + 0.140 * b_z_imf) * p_sw ** (-1.0 / 6.6)
+
+        warnings.warn("Shue et al., 1997 model used.", UserWarning)
+
+    # Spacecraft position
+    r1_x, r1_y, r1_z = r_gsm
+    r0_x, r0_y = [r1_x, np.sqrt(r1_y**2 + r1_z**2)]
+
+    if model[:2].lower() == "mp":
+        # Magnetopause
+
+        theta_min, min_val, _, _ = fminbound(
+            _magnetopause,
+            x1=-np.pi / 2,
+            x2=np.pi / 2,
+            args=(r0, alpha, r0_x, r1_y),
+            full_output=True,
+        )
+
+        min_dist = np.sqrt(min_val)
+
+        # calculate the direction to the spacecraft normal to the magnetopause
+        x_n = r0 * (2 / (1 + np.cos(theta_min))) ** alpha * np.cos(theta_min) - r1_x
+        phi = np.arctan2(r1_z, r1_y)
+        y_n = (
+            np.cos(phi)
+            * (r0 * (2 / (1 + np.cos(theta_min))) ** alpha * np.sin(theta_min))
+            - r1_y
+        )
+        z_n = (
+            np.sin(phi)
+            * (r0 * (2 / (1 + np.cos(theta_min))) ** alpha * np.sin(theta_min))
+            - r1_z
+        )
+
+        n_vec = np.stack([x_n, y_n, z_n]) / min_dist
+
+        # if statement to ensure normal is pointing away from Earth
+        if np.sqrt(r0_x**2 + r0_y**2) > r0 * (2 / (1 + np.cos(theta_min))) ** alpha:
+            n_vec *= -1
+            min_dist *= -1
+
+    else:
+        # Bow shock
+        warnings.warn(
+            "Farris & Russell 1994 bow shock model used.",
+            UserWarning,
+        )
+
+        gamma = 5 / 3
+        mach = m_alfven
+
+        # Bow shock standoff distance
+        rbs = r0 * (
+            1 + 1.1 * ((gamma - 1) * mach**2 + 2) / ((gamma + 1) * (mach**2 - 1))
+        )
+
+        # y ^ 2 = 0 - Ax + Bx ^ 2
+        coeffs = [0, 45.3, 0.04]
+        x = np.linspace(rbs, -100, int((rbs + 100) * 1e3) + 1)
+        y = np.sqrt(-coeffs[1] * (x - rbs) + coeffs[2] * (x - rbs) ** 2)
+        x = np.hstack([np.flip(x), x])
+        y = np.hstack([-np.flip(y), y])
+
+        r_xy = np.transpose(np.stack([x, y]))
+        args_bow_shock = (r0_x, r0_y)
+
+        min_val = np.min(_bow_shock(r_xy, *args_bow_shock))
+        min_pos = np.argmin(_bow_shock(r_xy, *args_bow_shock))
+
+        d_vec = np.stack([x - r0_x, y - r0_y])
+        d_min = d_vec[min_pos, :]
+
+        x_n = d_min[0] / np.linalg.norm(d_min)
+        min_dist = np.sqrt(min_val)
+
+        qyz = r1_y / r1_z
+        z_n = np.sign(r1_z) * np.sign(x_n) * np.sqrt((1 - x_n**2) / (1 + qyz**2))
+        y_n = z_n * qyz
+
+        n_vec = np.stack([x_n, y_n, z_n])
+
+        # if statement to ensure normal is pointing away from Earth
+        if n_vec[0] < 0:
+            n_vec *= -1
+            min_dist *= -1
+
+    return min_dist, n_vec
```

### Comparing `pyrfu-2.4.1/pyrfu/plot/__init__.py` & `pyrfu-2.4.3/pyrfu/plot/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# 3rd party imports
-import matplotlib.pyplot as plt
-
-from .add_position import add_position
-from .annotate_heatmap import annotate_heatmap
-from .colorbar import colorbar
-from .make_labels import make_labels
-from .mms_pl_config import mms_pl_config
-from .pl_scatter_matrix import pl_scatter_matrix
-from .pl_tx import pl_tx
-from .plot_ang_ang import plot_ang_ang
-from .plot_clines import plot_clines
-from .plot_heatmap import plot_heatmap
-
-# Local imports
-from .plot_line import plot_line
-from .plot_magnetosphere import plot_magnetosphere
-from .plot_projection import plot_projection
-from .plot_reduced_2d import plot_reduced_2d
-from .plot_sitl_overview import plot_sitl_overview
-from .plot_spectr import plot_spectr
-from .plot_surf import plot_surf
-from .span_tint import span_tint
-from .zoom import zoom
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.7"
-__status__ = "Prototype"
-
-
-# Setup plotting style
-plt.style.use("classic")
-plt.rcParams["figure.facecolor"] = "1"
-plt.rcParams["mathtext.sf"] = "sans"
-plt.rcParams["mathtext.fontset"] = "dejavusans"
-
-__all__ = [
-    "add_position",
-    "annotate_heatmap",
-    "colorbar",
-    "make_labels",
-    "mms_pl_config",
-    "pl_scatter_matrix",
-    "pl_tx",
-    "plot_ang_ang",
-    "plot_clines",
-    "plot_heatmap",
-    "plot_line",
-    "plot_magnetosphere",
-    "plot_projection",
-    "plot_reduced_2d",
-    "plot_sitl_overview",
-    "plot_spectr",
-    "plot_surf",
-    "span_tint",
-    "zoom",
-]
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# 3rd party imports
+import matplotlib.pyplot as plt
+
+from .add_position import add_position
+from .annotate_heatmap import annotate_heatmap
+from .colorbar import colorbar
+from .make_labels import make_labels
+from .mms_pl_config import mms_pl_config
+from .pl_scatter_matrix import pl_scatter_matrix
+from .pl_tx import pl_tx
+from .plot_ang_ang import plot_ang_ang
+from .plot_clines import plot_clines
+from .plot_heatmap import plot_heatmap
+
+# Local imports
+from .plot_line import plot_line
+from .plot_magnetosphere import plot_magnetosphere
+from .plot_projection import plot_projection
+from .plot_reduced_2d import plot_reduced_2d
+from .plot_sitl_overview import plot_sitl_overview
+from .plot_spectr import plot_spectr
+from .plot_surf import plot_surf
+from .span_tint import span_tint
+from .zoom import zoom
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+# Setup plotting style
+plt.style.use("classic")
+plt.rcParams["figure.facecolor"] = "1"
+plt.rcParams["mathtext.sf"] = "sans"
+plt.rcParams["mathtext.fontset"] = "dejavusans"
+
+__all__ = [
+    "add_position",
+    "annotate_heatmap",
+    "colorbar",
+    "make_labels",
+    "mms_pl_config",
+    "pl_scatter_matrix",
+    "pl_tx",
+    "plot_ang_ang",
+    "plot_clines",
+    "plot_heatmap",
+    "plot_line",
+    "plot_magnetosphere",
+    "plot_projection",
+    "plot_reduced_2d",
+    "plot_sitl_overview",
+    "plot_spectr",
+    "plot_surf",
+    "span_tint",
+    "zoom",
+]
```

### Comparing `pyrfu-2.4.1/pyrfu/plot/add_position.py` & `pyrfu-2.4.3/pyrfu/plot/add_position.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from matplotlib.dates import num2date
 
 # Local imports
 from ..pyrf import t_eval
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def add_position(
     ax,
     r_xyz,
     spine: float = 20,
```

### Comparing `pyrfu-2.4.1/pyrfu/plot/annotate_heatmap.py` & `pyrfu-2.4.3/pyrfu/plot/annotate_heatmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 # 3rd party imports
 import numpy as np
 from matplotlib import ticker
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def annotate_heatmap(
     im,
     data: np.ndarray = None,
     valfmt: str = "{x:.2f}",
```

### Comparing `pyrfu-2.4.1/pyrfu/plot/colorbar.py` & `pyrfu-2.4.3/pyrfu/plot/colorbar.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import matplotlib.pyplot as plt
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def colorbar(mappable, axis, pad: float = 0.01):
     r"""Add colorbar to ax corresponding to im.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/plot/logo/IRF_logo_blue_on_white.jpg` & `pyrfu-2.4.3/pyrfu/plot/logo/IRF_logo_blue_on_white.jpg`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/pyrfu/plot/mms_pl_config.py` & `pyrfu-2.4.3/pyrfu/plot/mms_pl_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import matplotlib.pyplot as plt
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 plt.style.use("seaborn-ticks")
 colors = ["tab:blue", "tab:green", "tab:red", "k"]
 markers = ["s", "d", "o", "^"]
```

### Comparing `pyrfu-2.4.1/pyrfu/plot/pl_scatter_matrix.py` & `pyrfu-2.4.3/pyrfu/plot/pl_scatter_matrix.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 # Local imports
 from ..pyrf import histogram2d
 from . import plot_spectr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def pl_scatter_matrix(
     inp1,
     inp2: xr.DataArray = None,
     pdf: bool = False,
```

### Comparing `pyrfu-2.4.1/pyrfu/plot/pl_tx.py` & `pyrfu-2.4.3/pyrfu/plot/pl_tx.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import matplotlib.pyplot as plt
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def pl_tx(axis, inp_list, comp, **kwargs):
     r"""Line plot of 4 spacecraft time series.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/plot/plot_ang_ang.py` & `pyrfu-2.4.3/pyrfu/plot/plot_ang_ang.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 
 # Local imports
 from ..pyrf import datetime642iso8601, time_clip
 from .plot_spectr import plot_spectr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def _time_avg(vdf, tint):
     if not tint:
         tint = list(datetime642iso8601(vdf.time.data[[0, -1]]))
         warnings.warn("Averages the entire time series", UserWarning)
```

### Comparing `pyrfu-2.4.1/pyrfu/plot/plot_clines.py` & `pyrfu-2.4.3/pyrfu/plot/plot_clines.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from matplotlib.colors import LogNorm
 
 # Local imports
 from .plot_line import plot_line
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def plot_clines(axis, inp, yscale="log", cscale="log", cmap="jet", **kwargs):
     r"""Plot lines with color associated to the level.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/plot/plot_heatmap.py` & `pyrfu-2.4.3/pyrfu/plot/plot_heatmap.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # 3rd party imports
 import numpy as np
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def plot_heatmap(
     ax,
     data,
     row_labels,
```

### Comparing `pyrfu-2.4.1/pyrfu/plot/plot_line.py` & `pyrfu-2.4.3/pyrfu/plot/plot_line.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-import matplotlib.dates as mdates
-import matplotlib.pyplot as plt
-import matplotlib.ticker as mticker
-
-# 3rd party imports
-import numpy as np
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.7"
-__status__ = "Prototype"
-
-
-def plot_line(axis, inp, **kwargs):
-    r"""Line plot of time series.
-
-    Parameters
-    ----------
-    axis : matplotlib.pyplot.subplotsaxes
-        Axis
-    inp : xarray.DataArray
-        Time series to plot
-
-    Other Parameters
-    ----------------
-    **kwargs
-        Keyword arguments control the Line2D properties.
-
-    Returns
-    -------
-    axs :
-        Axes.
-
-    """
-
-    if axis is None:
-        _, axis = plt.subplots(1)
-
-    if len(inp.shape) == 3:
-        data = np.reshape(
-            inp.data,
-            (inp.shape[0], inp.shape[1] * inp.shape[2]),
-        )
-    else:
-        data = inp.data
-
-    time = inp.time
-    axis.plot(time, data, **kwargs)
-
-    if time.dtype == "<M8[ns]":
-        locator = mdates.AutoDateLocator(minticks=3, maxticks=7)
-        formatter = mdates.ConciseDateFormatter(locator)
-        axis.xaxis.set_major_locator(locator)
-        axis.xaxis.set_major_formatter(formatter)
-
-    axis.grid(True, which="major", linestyle="-", linewidth="0.2", c="0.5")
-    axis.yaxis.set_major_locator(mticker.MaxNLocator(4))
-
-    return axis
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+import matplotlib.dates as mdates
+import matplotlib.pyplot as plt
+import matplotlib.ticker as mticker
+
+# 3rd party imports
+import numpy as np
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def plot_line(axis, inp, **kwargs):
+    r"""Line plot of time series.
+
+    Parameters
+    ----------
+    axis : matplotlib.pyplot.subplotsaxes
+        Axis
+    inp : xarray.DataArray
+        Time series to plot
+
+    Other Parameters
+    ----------------
+    **kwargs
+        Keyword arguments control the Line2D properties.
+
+    Returns
+    -------
+    axs :
+        Axes.
+
+    """
+
+    if axis is None:
+        _, axis = plt.subplots(1)
+
+    if len(inp.shape) == 3:
+        data = np.reshape(
+            inp.data,
+            (inp.shape[0], inp.shape[1] * inp.shape[2]),
+        )
+    else:
+        data = inp.data
+
+    time = inp.time
+    axis.plot(time, data, **kwargs)
+
+    if time.dtype == "<M8[ns]":
+        locator = mdates.AutoDateLocator(minticks=3, maxticks=7)
+        formatter = mdates.ConciseDateFormatter(locator)
+        axis.xaxis.set_major_locator(locator)
+        axis.xaxis.set_major_formatter(formatter)
+
+    axis.grid(True, which="major", linestyle="-", linewidth="0.2", c="0.5")
+    axis.yaxis.set_major_locator(mticker.MaxNLocator(4))
+
+    return axis
```

### Comparing `pyrfu-2.4.1/pyrfu/plot/plot_magnetosphere.py` & `pyrfu-2.4.3/pyrfu/plot/plot_magnetosphere.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Built-in imports
-import logging
-
-# 3rd party imports
-import numpy as np
-from geopack import geopack
-from matplotlib.patches import Wedge
-
-# Local imports
-from ..pyrf import datetime642unix, iso86012datetime64, magnetosphere
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.7"
-__status__ = "Prototype"
-
-logging.captureWarnings(True)
-logging.basicConfig(
-    format="[%(asctime)s] %(levelname)s: %(message)s",
-    datefmt="%d-%b-%y %H:%M:%S",
-    level=logging.INFO,
-)
-
-
-def _add_earth(ax=None, **kwargs):
-    theta1, theta2 = 90.0, 270.0
-    nightside_ = Wedge(
-        (0.0, 0.0),
-        1.0,
-        theta1,
-        theta2,
-        fc="k",
-        ec="k",
-        **kwargs,
-    )
-    dayside_ = Wedge(
-        (0.0, 0.0),
-        1.0,
-        theta2,
-        theta1,
-        fc="w",
-        ec="k",
-        **kwargs,
-    )
-    for wedge in [nightside_, dayside_]:
-        ax.add_artist(wedge)
-
-    return [nightside_, dayside_]
-
-
-def _add_field_lines(ax, tint):
-    # Get dipole axis at begin of the time interval
-    ut = datetime642unix(iso86012datetime64(np.array(tint)))[0]
-    _ = geopack.recalc(ut)
-
-    x_lines_m, z_lines_m = [[], []]
-    x_lines_p, z_lines_p = [[], []]
-
-    xx_gsm, zz_gsm = np.meshgrid(
-        np.linspace(-30, 6, 19),
-        np.linspace(-5, 5, 10),
-    )
-    xx_gsm = np.reshape(xx_gsm, (xx_gsm.size,))
-    zz_gsm = np.reshape(zz_gsm, (zz_gsm.size,))
-
-    for x_gsm, z_gsm in zip(xx_gsm, zz_gsm):
-        y_gsm = 0
-        _, _, _, xx, _, zz = geopack.trace(
-            x_gsm,
-            y_gsm,
-            z_gsm,
-            dir=-1,
-            rlim=100,
-            r0=0.99999,
-            parmod=2,
-            exname="t89",
-            inname="igrf",
-            maxloop=10000,
-        )
-        x_lines_m.append(xx)
-        z_lines_m.append(zz)
-
-        _, _, _, xx, _, zz = geopack.trace(
-            x_gsm,
-            y_gsm,
-            z_gsm,
-            dir=1,
-            rlim=100,
-            r0=0.99999,
-            parmod=2,
-            exname="t89",
-            inname="igrf",
-            maxloop=10000,
-        )
-        x_lines_p.append(xx)
-        z_lines_p.append(zz)
-
-    for xx, zz in zip(x_lines_m, z_lines_m):
-        ax.plot(xx, zz, color="k", linewidth=0.2)
-
-    for xx, zz in zip(x_lines_p, z_lines_p):
-        ax.plot(xx, zz, color="k", linewidth=0.2)
-
-
-def plot_magnetosphere(
-    ax,
-    tint,
-    colors: list = None,
-    field_lines: bool = True,
-):
-    r"""Plot magnetopause, bow shock and earth.
-
-    Parameters
-    ----------
-    ax : matplotlib.pyplot.subplotsaxes
-        Axis to plot.
-    tint : list of str
-        Time interval.
-    colors : list, Optional
-        Colors of the magnetopause and the bow show.
-        Default use ["tab:blue", "tab:red"]
-
-    Returns
-    -------
-    ax : matplotlib.pyplot.subplotsaxes
-        Axis.
-
-    """
-
-    # Compute Magnetopause
-    if colors is None:
-        colors = ["tab:blue", "tab:green"]
-
-    x_mp, y_mp = magnetosphere("mp_shue1998", tint)
-
-    # Compute bow show
-    x_bs, y_bs = magnetosphere("bs", tint)
-
-    # Plot
-    ax.plot(
-        np.hstack([x_mp, np.flip(x_mp)]),
-        np.hstack([y_mp, np.flip(-y_mp)]),
-        color=colors[0],
-        label="Magnetopause",
-    )
-    ax.plot(
-        np.hstack([x_bs, np.flip(x_bs)]),
-        np.hstack([y_bs, np.flip(-y_bs)]),
-        color=colors[1],
-        label="Bow Shock",
-    )
-    _add_earth(ax)
-
-    if field_lines:
-        logging.info("Computing field lines using T89 model...")
-        _add_field_lines(ax, tint)
-
-    return ax
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# Built-in imports
+import logging
+
+# 3rd party imports
+import numpy as np
+from geopack import geopack
+from matplotlib.patches import Wedge
+
+# Local imports
+from ..pyrf import datetime642unix, iso86012datetime64, magnetosphere
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+logging.captureWarnings(True)
+logging.basicConfig(
+    format="[%(asctime)s] %(levelname)s: %(message)s",
+    datefmt="%d-%b-%y %H:%M:%S",
+    level=logging.INFO,
+)
+
+
+def _add_earth(ax=None, **kwargs):
+    theta1, theta2 = 90.0, 270.0
+    nightside_ = Wedge(
+        (0.0, 0.0),
+        1.0,
+        theta1,
+        theta2,
+        fc="k",
+        ec="k",
+        **kwargs,
+    )
+    dayside_ = Wedge(
+        (0.0, 0.0),
+        1.0,
+        theta2,
+        theta1,
+        fc="w",
+        ec="k",
+        **kwargs,
+    )
+    for wedge in [nightside_, dayside_]:
+        ax.add_artist(wedge)
+
+    return [nightside_, dayside_]
+
+
+def _add_field_lines(ax, tint):
+    # Get dipole axis at begin of the time interval
+    ut = datetime642unix(iso86012datetime64(np.array(tint)))[0]
+    _ = geopack.recalc(ut)
+
+    x_lines_m, z_lines_m = [[], []]
+    x_lines_p, z_lines_p = [[], []]
+
+    xx_gsm, zz_gsm = np.meshgrid(
+        np.linspace(-30, 6, 19),
+        np.linspace(-5, 5, 10),
+    )
+    xx_gsm = np.reshape(xx_gsm, (xx_gsm.size,))
+    zz_gsm = np.reshape(zz_gsm, (zz_gsm.size,))
+
+    for x_gsm, z_gsm in zip(xx_gsm, zz_gsm):
+        y_gsm = 0
+        _, _, _, xx, _, zz = geopack.trace(
+            x_gsm,
+            y_gsm,
+            z_gsm,
+            dir=-1,
+            rlim=100,
+            r0=0.99999,
+            parmod=2,
+            exname="t89",
+            inname="igrf",
+            maxloop=10000,
+        )
+        x_lines_m.append(xx)
+        z_lines_m.append(zz)
+
+        _, _, _, xx, _, zz = geopack.trace(
+            x_gsm,
+            y_gsm,
+            z_gsm,
+            dir=1,
+            rlim=100,
+            r0=0.99999,
+            parmod=2,
+            exname="t89",
+            inname="igrf",
+            maxloop=10000,
+        )
+        x_lines_p.append(xx)
+        z_lines_p.append(zz)
+
+    for xx, zz in zip(x_lines_m, z_lines_m):
+        ax.plot(xx, zz, color="k", linewidth=0.2)
+
+    for xx, zz in zip(x_lines_p, z_lines_p):
+        ax.plot(xx, zz, color="k", linewidth=0.2)
+
+
+def plot_magnetosphere(
+    ax,
+    tint,
+    colors: list = None,
+    field_lines: bool = True,
+):
+    r"""Plot magnetopause, bow shock and earth.
+
+    Parameters
+    ----------
+    ax : matplotlib.pyplot.subplotsaxes
+        Axis to plot.
+    tint : list of str
+        Time interval.
+    colors : list, Optional
+        Colors of the magnetopause and the bow show.
+        Default use ["tab:blue", "tab:red"]
+
+    Returns
+    -------
+    ax : matplotlib.pyplot.subplotsaxes
+        Axis.
+
+    """
+
+    # Compute Magnetopause
+    if colors is None:
+        colors = ["tab:blue", "tab:green"]
+
+    x_mp, y_mp = magnetosphere("mp_shue1998", tint)
+
+    # Compute bow show
+    x_bs, y_bs = magnetosphere("bs", tint)
+
+    # Plot
+    ax.plot(
+        np.hstack([x_mp, np.flip(x_mp)]),
+        np.hstack([y_mp, np.flip(-y_mp)]),
+        color=colors[0],
+        label="Magnetopause",
+    )
+    ax.plot(
+        np.hstack([x_bs, np.flip(x_bs)]),
+        np.hstack([y_bs, np.flip(-y_bs)]),
+        color=colors[1],
+        label="Bow Shock",
+    )
+    _add_earth(ax)
+
+    if field_lines:
+        logging.info("Computing field lines using T89 model...")
+        _add_field_lines(ax, tint)
+
+    return ax
```

### Comparing `pyrfu-2.4.1/pyrfu/plot/plot_projection.py` & `pyrfu-2.4.3/pyrfu/plot/plot_projection.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import matplotlib.pyplot as plt
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def plot_projection(
     axis,
     v_x,
     v_y,
```

### Comparing `pyrfu-2.4.1/pyrfu/plot/plot_reduced_2d.py` & `pyrfu-2.4.3/pyrfu/plot/plot_reduced_2d.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 # 3rd party imports
 import numpy as np
 from matplotlib import colors
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def plot_reduced_2d(ax, f2d, clim: list = None):
     r"""Plot the 2D recuded distribution `f2d` onto the axis `ax`.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/plot/plot_sitl_overview.py` & `pyrfu-2.4.3/pyrfu/plot/plot_sitl_overview.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 from .plot_line import plot_line
 from .plot_magnetosphere import plot_magnetosphere
 from .plot_spectr import plot_spectr
 from .span_tint import span_tint
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def _tcut_edges(tint):
     tint = iso86012datetime64(np.array(tint))
     tint[0] += np.timedelta64(1, "s")
     tint[1] -= np.timedelta64(1, "s")
```

### Comparing `pyrfu-2.4.1/pyrfu/plot/plot_spectr.py` & `pyrfu-2.4.3/pyrfu/plot/plot_spectr.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 # 3rd party imports
 import matplotlib.pyplot as plt
 import matplotlib.ticker as mticker
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.11"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 plt.style.use("seaborn-ticks")
 
 
 def plot_spectr(
     axis,
```

### Comparing `pyrfu-2.4.1/pyrfu/plot/plot_surf.py` & `pyrfu-2.4.3/pyrfu/plot/plot_surf.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import matplotlib.pyplot as plt
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def plot_surf(axis, x, y, z, c, cmap, norm, cax_pos: str = "bottom"):
     r"""Plots surface.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/plot/span_tint.py` & `pyrfu-2.4.3/pyrfu/plot/span_tint.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 from matplotlib import dates
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def span_tint(axs, tint, ymin: float = 0, ymax: float = 1, **kwargs):
     r"""Add a vertical span (rectangle) across the time Axes.
 
     The rectangle spans from tint[0] to tint[1] horizontally, and, by default,
```

### Comparing `pyrfu-2.4.1/pyrfu/plot/zoom.py` & `pyrfu-2.4.3/pyrfu/plot/zoom.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
     BboxConnector,
     BboxConnectorPatch,
     BboxPatch,
 )
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def _connect_bbox(
     bbox1,
     bbox2,
     loc1a,
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/__init__.py` & `pyrfu-2.4.3/pyrfu/pyrf/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,220 +1,221 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-from .autocorr import autocorr
-from .avg_4sc import avg_4sc
-from .c_4_grad import c_4_grad
-from .c_4_j import c_4_j
-from .c_4_k import c_4_k
-from .c_4_v import c_4_v
-from .calc_ag import calc_ag
-from .calc_agyro import calc_agyro
-from .calc_dng import calc_dng
-from .calc_dt import calc_dt
-from .calc_fs import calc_fs
-from .calc_sqrtq import calc_sqrtq
-from .cart2sph import cart2sph
-from .cart2sph_ts import cart2sph_ts
-from .cdfepoch2datetime64 import cdfepoch2datetime64
-from .compress_cwt import compress_cwt
-from .convert_fac import convert_fac
-from .corr_deriv import corr_deriv
-from .cotrans import cotrans
-from .cross import cross
-from .date_str import date_str
-from .datetime2iso8601 import datetime2iso8601
-from .datetime642iso8601 import datetime642iso8601
-from .datetime642ttns import datetime642ttns
-from .datetime642unix import datetime642unix
-from .dec_par_perp import dec_par_perp
-from .dist_append import dist_append
-from .dot import dot
-from .dynamic_press import dynamic_press
-from .e_vxb import e_vxb
-from .eb_nrf import eb_nrf
-from .ebsp import ebsp
-from .edb import edb
-from .end import end
-from .estimate import estimate
-from .extend_tint import extend_tint
-from .filt import filt
-from .find_closest import find_closest
-from .get_omni_data import get_omni_data
-from .gradient import gradient
-from .gse2gsm import gse2gsm
-from .histogram import histogram
-from .histogram2d import histogram2d
-from .increments import increments
-from .int_sph_dist import int_sph_dist
-from .integrate import integrate
-from .iplasma_calc import iplasma_calc
-from .iso2unix import iso2unix
-from .iso86012datetime import iso86012datetime
-from .iso86012datetime64 import iso86012datetime64
-from .iso86012timevec import iso86012timevec
-from .l_shell import l_shell
-from .lowpass import lowpass
-from .magnetosphere import magnetosphere
-from .match_phibe_dir import match_phibe_dir
-from .match_phibe_v import match_phibe_v
-from .mean import mean
-from .mean_bins import mean_bins
-from .mean_field import mean_field
-from .medfilt import medfilt
-from .median_bins import median_bins
-from .movmean import movmean
-from .mva import mva
-from .new_xyz import new_xyz
-from .norm import norm
-from .normalize import normalize
-from .optimize_nbins_1d import optimize_nbins_1d
-from .optimize_nbins_2d import optimize_nbins_2d
-from .pid_4sc import pid_4sc
-from .plasma_calc import plasma_calc
-from .poynting_flux import poynting_flux
-from .pres_anis import pres_anis
-from .psd import psd
-from .pvi import pvi
-from .pvi_4sc import pvi_4sc
-
-# @Louis Richard
-from .read_cdf import read_cdf
-from .remove_repeated_points import remove_repeated_points
-from .resample import resample
-from .shock_normal import shock_normal
-from .shock_parameters import shock_parameters
-from .solid_angle import solid_angle
-from .sph2cart import sph2cart
-from .start import start
-from .struct_func import struct_func
-from .t_eval import t_eval
-from .time_clip import time_clip
-from .timevec2iso8601 import timevec2iso8601
-from .trace import trace
-from .ts_append import ts_append
-from .ts_scalar import ts_scalar
-from .ts_skymap import ts_skymap
-from .ts_tensor_xyz import ts_tensor_xyz
-from .ts_time import ts_time
-from .ts_vec_xyz import ts_vec_xyz
-from .ttns2datetime64 import ttns2datetime64
-from .unix2datetime64 import unix2datetime64
-from .vht import vht
-from .wave_fft import wave_fft
-from .wavelet import wavelet
-from .wavepolarize_means import wavepolarize_means
-from .waverage import waverage
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.7"
-__status__ = "Prototype"
-
-__all__ = [
-    "autocorr",
-    "average_vdf",
-    "avg_4sc",
-    "c_4_grad",
-    "c_4_j",
-    "c_4_k",
-    "c_4_v",
-    "calc_ag",
-    "calc_agyro",
-    "calc_dng",
-    "calc_dt",
-    "calc_fs",
-    "calc_sqrtq",
-    "cart2sph",
-    "cart2sph_ts",
-    "cdfepoch2datetime64",
-    "compress_cwt",
-    "convert_fac",
-    "corr_deriv",
-    "cotrans",
-    "cross",
-    "date_str",
-    "datetime2iso8601",
-    "datetime642iso8601",
-    "datetime642ttns",
-    "datetime642unix",
-    "dec_par_perp",
-    "dist_append",
-    "dot",
-    "dynamic_press",
-    "e_vxb",
-    "eb_nrf",
-    "ebsp",
-    "edb",
-    "end",
-    "estimate",
-    "extend_tint",
-    "filt",
-    "find_closest",
-    "get_omni_data",
-    "gradient",
-    "gse2gsm",
-    "histogram",
-    "histogram2d",
-    "increments",
-    "int_sph_dist",
-    "integrate",
-    "iplasma_calc",
-    "iso2unix",
-    "iso86012datetime",
-    "iso86012datetime64",
-    "iso86012timevec",
-    "l_shell",
-    "lowpass",
-    "magnetosphere",
-    "match_phibe_dir",
-    "match_phibe_v",
-    "mean",
-    "mean_bins",
-    "mean_field",
-    "medfilt",
-    "median_bins",
-    "movmean",
-    "mva",
-    "new_xyz",
-    "norm",
-    "normalize",
-    "optimize_nbins_1d",
-    "optimize_nbins_2d",
-    "pid_4sc",
-    "plasma_beta",
-    "plasma_calc",
-    "poynting_flux",
-    "pres_anis",
-    "psd",
-    "pvi",
-    "pvi_4sc",
-    "read_cdf",
-    "remove_repeated_points",
-    "resample",
-    "shock_normal",
-    "shock_parameters",
-    "solid_angle",
-    "sph2cart",
-    "st_diff",
-    "start",
-    "struct_func",
-    "t_eval",
-    "time_clip",
-    "timevec2iso8601",
-    "trace",
-    "ts_append",
-    "ts_scalar",
-    "ts_skymap",
-    "ts_tensor_xyz",
-    "ts_time",
-    "ts_vec_xyz",
-    "ttns2datetime64",
-    "unix2datetime64",
-    "vht",
-    "wave_fft",
-    "wavelet",
-    "wavepolarize_means",
-    "waverage",
-]
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+from .autocorr import autocorr
+from .average_vdf import average_vdf
+from .avg_4sc import avg_4sc
+from .c_4_grad import c_4_grad
+from .c_4_j import c_4_j
+from .c_4_k import c_4_k
+from .c_4_v import c_4_v
+from .calc_ag import calc_ag
+from .calc_agyro import calc_agyro
+from .calc_dng import calc_dng
+from .calc_dt import calc_dt
+from .calc_fs import calc_fs
+from .calc_sqrtq import calc_sqrtq
+from .cart2sph import cart2sph
+from .cart2sph_ts import cart2sph_ts
+from .cdfepoch2datetime64 import cdfepoch2datetime64
+from .compress_cwt import compress_cwt
+from .convert_fac import convert_fac
+from .corr_deriv import corr_deriv
+from .cotrans import cotrans
+from .cross import cross
+from .date_str import date_str
+from .datetime2iso8601 import datetime2iso8601
+from .datetime642iso8601 import datetime642iso8601
+from .datetime642ttns import datetime642ttns
+from .datetime642unix import datetime642unix
+from .dec_par_perp import dec_par_perp
+from .dist_append import dist_append
+from .dot import dot
+from .dynamic_press import dynamic_press
+from .e_vxb import e_vxb
+from .eb_nrf import eb_nrf
+from .ebsp import ebsp
+from .edb import edb
+from .end import end
+from .estimate import estimate
+from .extend_tint import extend_tint
+from .filt import filt
+from .find_closest import find_closest
+from .get_omni_data import get_omni_data
+from .gradient import gradient
+from .gse2gsm import gse2gsm
+from .histogram import histogram
+from .histogram2d import histogram2d
+from .increments import increments
+from .int_sph_dist import int_sph_dist
+from .integrate import integrate
+from .iplasma_calc import iplasma_calc
+from .iso2unix import iso2unix
+from .iso86012datetime import iso86012datetime
+from .iso86012datetime64 import iso86012datetime64
+from .iso86012timevec import iso86012timevec
+from .l_shell import l_shell
+from .lowpass import lowpass
+from .magnetosphere import magnetosphere
+from .match_phibe_dir import match_phibe_dir
+from .match_phibe_v import match_phibe_v
+from .mean import mean
+from .mean_bins import mean_bins
+from .mean_field import mean_field
+from .medfilt import medfilt
+from .median_bins import median_bins
+from .movmean import movmean
+from .mva import mva
+from .new_xyz import new_xyz
+from .norm import norm
+from .normalize import normalize
+from .optimize_nbins_1d import optimize_nbins_1d
+from .optimize_nbins_2d import optimize_nbins_2d
+from .pid_4sc import pid_4sc
+from .plasma_calc import plasma_calc
+from .poynting_flux import poynting_flux
+from .pres_anis import pres_anis
+from .psd import psd
+from .pvi import pvi
+from .pvi_4sc import pvi_4sc
+
+# @Louis Richard
+from .read_cdf import read_cdf
+from .remove_repeated_points import remove_repeated_points
+from .resample import resample
+from .shock_normal import shock_normal
+from .shock_parameters import shock_parameters
+from .solid_angle import solid_angle
+from .sph2cart import sph2cart
+from .start import start
+from .struct_func import struct_func
+from .t_eval import t_eval
+from .time_clip import time_clip
+from .timevec2iso8601 import timevec2iso8601
+from .trace import trace
+from .ts_append import ts_append
+from .ts_scalar import ts_scalar
+from .ts_skymap import ts_skymap
+from .ts_tensor_xyz import ts_tensor_xyz
+from .ts_time import ts_time
+from .ts_vec_xyz import ts_vec_xyz
+from .ttns2datetime64 import ttns2datetime64
+from .unix2datetime64 import unix2datetime64
+from .vht import vht
+from .wave_fft import wave_fft
+from .wavelet import wavelet
+from .wavepolarize_means import wavepolarize_means
+from .waverage import waverage
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+__all__ = [
+    "autocorr",
+    "average_vdf",
+    "avg_4sc",
+    "c_4_grad",
+    "c_4_j",
+    "c_4_k",
+    "c_4_v",
+    "calc_ag",
+    "calc_agyro",
+    "calc_dng",
+    "calc_dt",
+    "calc_fs",
+    "calc_sqrtq",
+    "cart2sph",
+    "cart2sph_ts",
+    "cdfepoch2datetime64",
+    "compress_cwt",
+    "convert_fac",
+    "corr_deriv",
+    "cotrans",
+    "cross",
+    "date_str",
+    "datetime2iso8601",
+    "datetime642iso8601",
+    "datetime642ttns",
+    "datetime642unix",
+    "dec_par_perp",
+    "dist_append",
+    "dot",
+    "dynamic_press",
+    "e_vxb",
+    "eb_nrf",
+    "ebsp",
+    "edb",
+    "end",
+    "estimate",
+    "extend_tint",
+    "filt",
+    "find_closest",
+    "get_omni_data",
+    "gradient",
+    "gse2gsm",
+    "histogram",
+    "histogram2d",
+    "increments",
+    "int_sph_dist",
+    "integrate",
+    "iplasma_calc",
+    "iso2unix",
+    "iso86012datetime",
+    "iso86012datetime64",
+    "iso86012timevec",
+    "l_shell",
+    "lowpass",
+    "magnetosphere",
+    "match_phibe_dir",
+    "match_phibe_v",
+    "mean",
+    "mean_bins",
+    "mean_field",
+    "medfilt",
+    "median_bins",
+    "movmean",
+    "mva",
+    "new_xyz",
+    "norm",
+    "normalize",
+    "optimize_nbins_1d",
+    "optimize_nbins_2d",
+    "pid_4sc",
+    "plasma_beta",
+    "plasma_calc",
+    "poynting_flux",
+    "pres_anis",
+    "psd",
+    "pvi",
+    "pvi_4sc",
+    "read_cdf",
+    "remove_repeated_points",
+    "resample",
+    "shock_normal",
+    "shock_parameters",
+    "solid_angle",
+    "sph2cart",
+    "st_diff",
+    "start",
+    "struct_func",
+    "t_eval",
+    "time_clip",
+    "timevec2iso8601",
+    "trace",
+    "ts_append",
+    "ts_scalar",
+    "ts_skymap",
+    "ts_tensor_xyz",
+    "ts_time",
+    "ts_vec_xyz",
+    "ttns2datetime64",
+    "unix2datetime64",
+    "vht",
+    "wave_fft",
+    "wavelet",
+    "wavepolarize_means",
+    "waverage",
+]
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/autocorr.py` & `pyrfu-2.4.3/pyrfu/pyrf/autocorr.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import xarray as xr
 
 # Local imports
 from .calc_dt import calc_dt
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2022"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.12"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def autocorr(inp, maxlags: int = None, normed: bool = True):
     r"""Compute the autocorrelation function
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/average_vdf.py` & `pyrfu-2.4.3/pyrfu/pyrf/average_vdf.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# 3rd party imports
-import numpy as np
-
-# Local imports
-from .ts_skymap import ts_skymap
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2023"
-__license__ = "MIT"
-__version__ = "2.3.26"
-__status__ = "Prototype"
-
-
-def average_vdf(vdf, n_pts):
-    r"""Time averages the velocity distribution functions over `n_pts` in time.
-
-    Parameters
-    ----------
-    vdf : xarray.DataArray
-        Time series of the velocity distribution function.
-    n_pts : int
-        Number of points (samples) of the averaging window.
-
-    Returns
-    -------
-    vdf_avg : xarray.DataArray
-        Time series of the time averaged velocity distribution function.
-
-    """
-
-    assert n_pts % 2 != 0, "The number of distributions to be averaged must be an odd"
-
-    assert np.median(vdf.energy.data[0, :] - vdf.energy.data[0, :]) == 0
-
-    n_vdf = len(vdf.time.data)
-    times = vdf.time.data
-
-    pad_value = np.floor(n_pts / 2)
-    avg_inds = np.arange(pad_value, n_vdf - pad_value, n_pts, dtype=int)
-    time_avg = times[avg_inds]
-
-    energy_avg = np.zeros((len(avg_inds), vdf.data.shape[1]))
-    phi_avg = np.zeros((len(avg_inds), vdf.data.shape[2]))
-    vdf_avg = np.zeros((len(avg_inds), *vdf.data.shape[1:]))
-
-    for i, avg_ind in enumerate(avg_inds):
-        l_bound = int(avg_ind - pad_value)
-        r_bound = int(avg_ind + pad_value)
-        vdf_avg[i, ...] = np.nanmean(
-            vdf.data.data[l_bound:r_bound, ...],
-            axis=0,
-        )
-        energy_avg[i, ...] = np.nanmean(
-            vdf.energy.data[l_bound:r_bound, ...],
-            axis=0,
-        )
-        phi_avg[i, ...] = np.nanmean(
-            vdf.phi.data[l_bound:r_bound, ...],
-            axis=0,
-        )
-
-    # Attributes
-    glob_attrs = vdf.attrs  # Global attributes
-    vdf_attrs = vdf.data.attrs  # VDF attributes
-    coords_attrs = {k: vdf[k].attrs for k in ["time", "energy", "phi", "theta"]}
-
-    # Get delta energy in global attributes for selected timestamps
-    glob_attrs["delta_energy_minus"] = glob_attrs["delta_energy_minus"][avg_inds]
-    glob_attrs["delta_energy_plus"] = glob_attrs["delta_energy_plus"][avg_inds]
-
-    glob_attrs["esteptable"] = glob_attrs["esteptable"][: len(avg_inds)]
-
-    vdf_avg = ts_skymap(
-        time_avg,
-        vdf_avg,
-        energy_avg,
-        phi_avg,
-        vdf.theta.data,
-        energy0=glob_attrs["energy0"],
-        energy1=glob_attrs["energy1"],
-        esteptable=glob_attrs["esteptable"][: len(avg_inds)],
-        attrs=vdf_attrs,
-        coords_attrs=coords_attrs,
-        glob_attrs=glob_attrs,
-    )
-
-    return vdf_avg
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# 3rd party imports
+import numpy as np
+
+# Local imports
+from .ts_skymap import ts_skymap
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def average_vdf(vdf, n_pts):
+    r"""Time averages the velocity distribution functions over `n_pts` in time.
+
+    Parameters
+    ----------
+    vdf : xarray.DataArray
+        Time series of the velocity distribution function.
+    n_pts : int
+        Number of points (samples) of the averaging window.
+
+    Returns
+    -------
+    vdf_avg : xarray.DataArray
+        Time series of the time averaged velocity distribution function.
+
+    """
+
+    assert n_pts % 2 != 0, "The number of distributions to be averaged must be an odd"
+
+    assert np.median(vdf.energy.data[0, :] - vdf.energy.data[0, :]) == 0
+
+    n_vdf = len(vdf.time.data)
+    times = vdf.time.data
+
+    pad_value = np.floor(n_pts / 2)
+    avg_inds = np.arange(pad_value, n_vdf - pad_value, n_pts, dtype=int)
+    time_avg = times[avg_inds]
+
+    energy_avg = np.zeros((len(avg_inds), vdf.data.shape[1]))
+    phi_avg = np.zeros((len(avg_inds), vdf.data.shape[2]))
+    vdf_avg = np.zeros((len(avg_inds), *vdf.data.shape[1:]))
+
+    for i, avg_ind in enumerate(avg_inds):
+        l_bound = int(avg_ind - pad_value)
+        r_bound = int(avg_ind + pad_value)
+        vdf_avg[i, ...] = np.nanmean(
+            vdf.data.data[l_bound:r_bound, ...],
+            axis=0,
+        )
+        energy_avg[i, ...] = np.nanmean(
+            vdf.energy.data[l_bound:r_bound, ...],
+            axis=0,
+        )
+        phi_avg[i, ...] = np.nanmean(
+            vdf.phi.data[l_bound:r_bound, ...],
+            axis=0,
+        )
+
+    # Attributes
+    glob_attrs = vdf.attrs  # Global attributes
+    vdf_attrs = vdf.data.attrs  # VDF attributes
+    coords_attrs = {k: vdf[k].attrs for k in ["time", "energy", "phi", "theta"]}
+
+    # Get delta energy in global attributes for selected timestamps
+    glob_attrs["delta_energy_minus"] = glob_attrs["delta_energy_minus"][avg_inds]
+    glob_attrs["delta_energy_plus"] = glob_attrs["delta_energy_plus"][avg_inds]
+
+    glob_attrs["esteptable"] = glob_attrs["esteptable"][: len(avg_inds)]
+
+    vdf_avg = ts_skymap(
+        time_avg,
+        vdf_avg,
+        energy_avg,
+        phi_avg,
+        vdf.theta.data,
+        energy0=glob_attrs["energy0"],
+        energy1=glob_attrs["energy1"],
+        esteptable=glob_attrs["esteptable"][: len(avg_inds)],
+        attrs=vdf_attrs,
+        coords_attrs=coords_attrs,
+        glob_attrs=glob_attrs,
+    )
+
+    return vdf_avg
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/avg_4sc.py` & `pyrfu-2.4.3/pyrfu/pyrf/avg_4sc.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # Local imports
 from .calc_fs import calc_fs
 from .resample import resample
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def avg_4sc(b_list):
     r"""Computes the input quantity at the center of mass of the MMS
     tetrahedron.
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/c_4_grad.py` & `pyrfu-2.4.3/pyrfu/pyrf/c_4_grad.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 from .normalize import normalize
 
 # Local imports
 from .resample import resample
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def _to_ts(out_data, b_dict):
     if len(out_data.shape) == 1:
         out = xr.DataArray(out_data, coords=[b_dict["1"].time], dims=["time"])
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/c_4_j.py` & `pyrfu-2.4.3/pyrfu/pyrf/c_4_j.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 # Local imports
 from .avg_4sc import avg_4sc
 from .c_4_grad import c_4_grad
 from .cross import cross
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.10"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def c_4_j(r_list, b_list):
     r"""Calculate current density :math:`J` from using 4
     spacecraft technique [4]_, the divergence of the magnetic field
     :math:`\nabla . B`, magnetic field at the center of
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/c_4_k.py` & `pyrfu-2.4.3/pyrfu/pyrf/c_4_k.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 # Local imports
 from .cross import cross
 from .dot import dot
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def c_4_k(r_list):
     r"""Calculates reciprocal vectors in barycentric coordinates.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/c_4_v.py` & `pyrfu-2.4.3/pyrfu/pyrf/c_4_v.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # 3rd party imports
 import numpy as np
 from scipy import interpolate
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def _get_vol_ten(r_xyz, time):
     if len(time) == 1:
         time = np.array([time, time, time, time])
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/calc_ag.py` & `pyrfu-2.4.3/pyrfu/pyrf/calc_ag.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def calc_ag(p_xyz):
     r"""Computes agyrotropy coefficient as in [16]_
 
     .. math::
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/calc_agyro.py` & `pyrfu-2.4.3/pyrfu/pyrf/calc_agyro.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def calc_agyro(p_xyz):
     r"""Computes agyrotropy coefficient as
 
     .. math::
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/calc_dng.py` & `pyrfu-2.4.3/pyrfu/pyrf/calc_dng.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def calc_dng(p_xyz):
     r"""Computes agyrotropy coefficient as in [15]_
 
     .. math::
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/calc_dt.py` & `pyrfu-2.4.3/pyrfu/pyrf/calc_dt.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# 3rd party imports
-import numpy as np
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.7"
-__status__ = "Prototype"
-
-
-def calc_dt(inp):
-    r"""Computes time step of the input time series.
-
-    Parameters
-    ----------
-    inp : xarray.DataArray
-        Time series of the input variable.
-
-    Returns
-    -------
-    out : float
-        Time step in seconds.
-
-    """
-
-    out = np.median(np.diff(inp.time.data)).astype(np.float64) * 1e-9
-
-    return out
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# 3rd party imports
+import numpy as np
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def calc_dt(inp):
+    r"""Computes time step of the input time series.
+
+    Parameters
+    ----------
+    inp : xarray.DataArray
+        Time series of the input variable.
+
+    Returns
+    -------
+    out : float
+        Time step in seconds.
+
+    """
+
+    out = np.median(np.diff(inp.time.data)).astype(np.float64) * 1e-9
+
+    return out
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/calc_sqrtq.py` & `pyrfu-2.4.3/pyrfu/pyrf/calc_sqrtq.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def calc_sqrtq(p_xyz):
     r"""Computes agyrotropy coefficient as in [1]_
 
     .. math::
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/cart2sph.py` & `pyrfu-2.4.3/pyrfu/pyrf/cart2sph.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def cart2sph(x, y, z):
     r"""Cartesian to spherical coordinate transform.
 
     .. math::
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/cart2sph_ts.py` & `pyrfu-2.4.3/pyrfu/pyrf/cart2sph_ts.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# 3rd party imports
-import numpy as np
-
-# Local imports
-from .ts_vec_xyz import ts_vec_xyz
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.7"
-__status__ = "Prototype"
-
-
-def cart2sph_ts(inp, direction_flag: int = 1):
-    r"""Computes magnitude, theta and phi angle from column vector xyz
-    (first column is x ....) theta is 0 at equator.
-    direction_flag = -1  -> to make transformation in opposite direction
-
-    Parameters
-    ----------
-    inp : xarray.DataArray
-        Time series to convert.
-
-    direction_flag : {1, -1}, Optional
-        Set to 1 (default) to transform from cartesian to spherical
-        coordinates. Set to -1 to transform from spherical to cartesian
-        coordinates.
-
-    Returns
-    -------
-    out : xarray.DataArray
-        Input field in spherical/cartesian coordinate system.
-
-    """
-
-    if inp.attrs["TENSOR_ORDER"] != 1 or inp.data.ndim != 2:
-        raise TypeError("Input must be vector field")
-
-    if direction_flag == -1:
-        r_data = inp.data[:, 0]
-
-        sin_the = np.sin(np.deg2rad(inp.data[:, 1]))
-        cos_the = np.cos(np.deg2rad(inp.data[:, 1]))
-        sin_phi = np.sin(np.deg2rad(inp.data[:, 2]))
-        cos_phi = np.cos(np.deg2rad(inp.data[:, 2]))
-
-        z_data = r_data * sin_the
-        x_data = r_data * cos_the * cos_phi
-        y_data = r_data * cos_the * sin_phi
-
-        out_data = np.hstack([x_data, y_data, z_data])
-
-    else:
-        xy2 = inp.data[:, 0] ** 2 + inp.data[:, 1] ** 2
-
-        r_data = np.sqrt(xy2 + inp.data[:, 2] ** 2)
-        theta = np.rad2deg(np.arctan2(inp.data[:, 2], np.sqrt(xy2)))
-        phi = np.rad2deg(np.arctan2(inp.data[:, 1], inp.data[:, 0]))
-
-        out_data = np.transpose(np.vstack([r_data, theta, phi]))
-
-    out = ts_vec_xyz(inp.time.data, out_data, inp.attrs)
-
-    return out
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# 3rd party imports
+import numpy as np
+
+# Local imports
+from .ts_vec_xyz import ts_vec_xyz
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def cart2sph_ts(inp, direction_flag: int = 1):
+    r"""Computes magnitude, theta and phi angle from column vector xyz
+    (first column is x ....) theta is 0 at equator.
+    direction_flag = -1  -> to make transformation in opposite direction
+
+    Parameters
+    ----------
+    inp : xarray.DataArray
+        Time series to convert.
+
+    direction_flag : {1, -1}, Optional
+        Set to 1 (default) to transform from cartesian to spherical
+        coordinates. Set to -1 to transform from spherical to cartesian
+        coordinates.
+
+    Returns
+    -------
+    out : xarray.DataArray
+        Input field in spherical/cartesian coordinate system.
+
+    """
+
+    if inp.attrs["TENSOR_ORDER"] != 1 or inp.data.ndim != 2:
+        raise TypeError("Input must be vector field")
+
+    if direction_flag == -1:
+        r_data = inp.data[:, 0]
+
+        sin_the = np.sin(np.deg2rad(inp.data[:, 1]))
+        cos_the = np.cos(np.deg2rad(inp.data[:, 1]))
+        sin_phi = np.sin(np.deg2rad(inp.data[:, 2]))
+        cos_phi = np.cos(np.deg2rad(inp.data[:, 2]))
+
+        z_data = r_data * sin_the
+        x_data = r_data * cos_the * cos_phi
+        y_data = r_data * cos_the * sin_phi
+
+        out_data = np.hstack([x_data, y_data, z_data])
+
+    else:
+        xy2 = inp.data[:, 0] ** 2 + inp.data[:, 1] ** 2
+
+        r_data = np.sqrt(xy2 + inp.data[:, 2] ** 2)
+        theta = np.rad2deg(np.arctan2(inp.data[:, 2], np.sqrt(xy2)))
+        phi = np.rad2deg(np.arctan2(inp.data[:, 1], inp.data[:, 0]))
+
+        out_data = np.transpose(np.vstack([r_data, theta, phi]))
+
+    out = ts_vec_xyz(inp.time.data, out_data, inp.attrs)
+
+    return out
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/cdfepoch2datetime64.py` & `pyrfu-2.4.3/pyrfu/pyrf/cdfepoch2datetime64.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# 3rd party imports
-import numpy as np
-from cdflib import cdfepoch
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2023"
-__license__ = "MIT"
-__version__ = "2.3.26"
-__status__ = "Prototype"
-
-
-def _compose_date(
-    years,
-    months,
-    days,
-    hours=None,
-    minutes=None,
-    seconds=None,
-    milliseconds=None,
-    microseconds=None,
-    nanoseconds=None,
-):
-    years = np.asarray(years) - 1970
-    months = np.asarray(months) - 1
-    days = np.asarray(days) - 1
-    types = [
-        "<M8[Y]",
-        "<m8[M]",
-        "<m8[D]",
-        "<m8[h]",
-        "<m8[m]",
-        "<m8[s]",
-        "<m8[ms]",
-        "<m8[us]",
-        "<m8[ns]",
-    ]
-    vals = [
-        years,
-        months,
-        days,
-        hours,
-        minutes,
-        seconds,
-        milliseconds,
-        microseconds,
-        nanoseconds,
-    ]
-
-    dates_list = []
-    for t, v in zip(types, vals):
-        if v is not None:
-            dates_list.append(np.asarray(v, dtype=t))
-
-    dates = sum(dates_list)
-
-    return dates
-
-
-def cdfepoch2datetime64(epochs):
-    r"""Converts CDF epochs to numpy.datetime64 with nanosecond precision.
-
-    Parameters
-    ----------
-    epochs : array_like
-        CDF epochs to convert.
-
-    Returns
-    -------
-    times : numpy.ndarray
-        Array of times in datetime64([ns]).
-
-    """
-
-    times = cdfepoch.breakdown(epochs)
-    times = np.transpose(np.atleast_2d(times))
-
-    times = _compose_date(*times).astype("datetime64[ns]")
-
-    return times
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# 3rd party imports
+import numpy as np
+from cdflib import cdfepoch
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def _compose_date(
+    years,
+    months,
+    days,
+    hours=None,
+    minutes=None,
+    seconds=None,
+    milliseconds=None,
+    microseconds=None,
+    nanoseconds=None,
+):
+    years = np.asarray(years) - 1970
+    months = np.asarray(months) - 1
+    days = np.asarray(days) - 1
+    types = [
+        "<M8[Y]",
+        "<m8[M]",
+        "<m8[D]",
+        "<m8[h]",
+        "<m8[m]",
+        "<m8[s]",
+        "<m8[ms]",
+        "<m8[us]",
+        "<m8[ns]",
+    ]
+    vals = [
+        years,
+        months,
+        days,
+        hours,
+        minutes,
+        seconds,
+        milliseconds,
+        microseconds,
+        nanoseconds,
+    ]
+
+    dates_list = []
+    for t, v in zip(types, vals):
+        if v is not None:
+            dates_list.append(np.asarray(v, dtype=t))
+
+    dates = sum(dates_list)
+
+    return dates
+
+
+def cdfepoch2datetime64(epochs):
+    r"""Converts CDF epochs to numpy.datetime64 with nanosecond precision.
+
+    Parameters
+    ----------
+    epochs : array_like
+        CDF epochs to convert.
+
+    Returns
+    -------
+    times : numpy.ndarray
+        Array of times in datetime64([ns]).
+
+    """
+
+    times = cdfepoch.breakdown(epochs)
+    times = np.transpose(np.atleast_2d(times))
+
+    times = _compose_date(*times).astype("datetime64[ns]")
+
+    return times
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/compress_cwt.py` & `pyrfu-2.4.3/pyrfu/pyrf/compress_cwt.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # 3rd party import
 import numba
 import numpy as np
 
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
 
 @numba.jit(nopython=True, parallel=True)
 def _compress_cwt_1d(cwt, nc: int = 100):
     nf = cwt.shape[1]
     idxs = np.arange(
         start=int(nc / 2),
         stop=len(cwt) - int(nc / 2),
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/convert_fac.py` & `pyrfu-2.4.3/pyrfu/pyrf/convert_fac.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 
 # Local imports
 from .resample import resample
 from .ts_vec_xyz import ts_vec_xyz
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def convert_fac(inp, b_bgd, r_xyz: list = None):
     r"""Transforms to a field-aligned coordinate (FAC) system defined as :
         * R_parallel_z aligned with the background magnetic field
         * R_perp_y defined by R_parallel cross the position vector of the
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/cotrans.py` & `pyrfu-2.4.3/pyrfu/pyrf/cotrans.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,333 +1,333 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-import json
-
-# Built-in imports
-import os
-
-# 3rd party imports
-import numpy as np
-import xarray as xr
-
-# Local imports
-from ..models import igrf
-from .ts_vec_xyz import ts_vec_xyz
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.7"
-__status__ = "Prototype"
-
-
-def _triang(angle, axis):
-    cos_angle = np.cos(np.deg2rad(angle))
-    sin_angle = np.sin(np.deg2rad(angle))
-
-    axes = list(filter(lambda x: x != axis, np.arange(3)))
-
-    transf_mat = np.zeros((len(angle), 3, 3))
-    transf_mat[:, axes[0], axes[0]] = cos_angle
-    transf_mat[:, axes[1], axes[1]] = cos_angle
-    transf_mat[:, axis, axis] = 1
-    transf_mat[:, axes[0], axes[1]] = sin_angle
-    transf_mat[:, axes[1], axes[0]] = -sin_angle
-
-    return transf_mat
-
-
-def _dipole_direction_gse(time, flag: str = "dipole"):
-    lambda_, phi = igrf(time, flag)
-
-    cos_phi = np.cos(np.deg2rad(phi))
-    dipole_direction_geo_ = np.stack(
-        [
-            cos_phi * np.cos(np.deg2rad(lambda_)),
-            cos_phi * np.sin(np.deg2rad(lambda_)),
-            np.sin(np.deg2rad(phi)),
-        ],
-    ).T
-
-    dipole_direction_gse_ = cotrans(
-        np.hstack([time[:, None], dipole_direction_geo_]),
-        "geo>gse",
-    )
-
-    return dipole_direction_gse_
-
-
-def _transformation_matrix(t, tind, hapgood, *args):
-    t_zero, ut, d0_j2000, d_j2000, h_j2000, t_j2000 = args
-
-    transf_mat_out = np.zeros((len(t), 3, 3))
-    transf_mat_out[:, 0, 0] = np.ones(len(t))
-    transf_mat_out[:, 1, 1] = np.ones(len(t))
-    transf_mat_out[:, 2, 2] = np.ones(len(t))
-
-    for j, t_num in enumerate(tind[::-1]):
-        if t_num in [-1, 1]:
-            if hapgood:
-                theta = 100.461 + 36000.770 * t_zero + 15.04107 * ut
-
-            else:
-                # Source: United States Naval Observatory, Astronomical
-                # Applications Dept. http: // aa.usno.navy.mil / faq / docs
-                # / GAST.php Last modified: 2011/06/14T14:04
-                gmst = 6.697374558
-                gmst += 0.06570982441908 * d0_j2000
-                gmst += 1.00273790935 * h_j2000
-                gmst += 0.000026 * t_j2000**2
-
-                gmst = gmst % 24  # Interval 0->24 hours
-                theta = (360 / 24) * gmst  # Convert to degree.
-
-            # invert if tInd = -1
-            transf_mat = _triang(theta * np.sign(t_num), 2)
-
-        elif t_num in [-2, 2]:
-            if hapgood:
-                eps = 23.439 - 0.013 * t_zero
-                # Suns mean anomaly
-                m_anom = 357.528 + 35999.050 * t_zero + 0.04107 * ut
-                # Suns mean longitude
-                m_long = 280.460 + 36000.772 * t_zero + 0.04107 * ut
-                l_sun = m_long
-                l_sun += (1.915 - 0.0048 * t_zero) * np.sin(
-                    np.deg2rad(m_anom),
-                )
-                l_sun += 0.020 * np.sin(np.deg2rad(2 * m_anom))
-            else:
-                # Source: United States Naval Observatory, Astronomical
-                # Applications Dept.
-                # http://aa.usno.navy.mil/faq/docsSunApprox.php.
-                # Last modified: 2012/11/06T14:12
-                eps = 23.439 - 0.00000036 * d_j2000
-                m_anom = 357.529 + 0.98560028 * d_j2000
-                m_long = 280.459 + 0.98564736 * d_j2000
-                l_sun = m_long
-                l_sun += 1.915 * np.sin(np.deg2rad(m_anom))
-                l_sun += 0.020 * np.sin(np.deg2rad(2 * m_anom))
-
-            transf_mat = np.matmul(_triang(l_sun, 2), _triang(eps, 0))
-            if t_num == -2:
-                transf_mat = np.transpose(transf_mat, [0, 2, 1])
-
-        elif t_num in [-3, 3]:
-            dipole_direction_gse_ = _dipole_direction_gse(t, "dipole")
-            y_e = dipole_direction_gse_[:, 2]  # 1st col is time
-            z_e = dipole_direction_gse_[:, 3]
-            psi = np.rad2deg(np.arctan(y_e / z_e))
-
-            transf_mat = _triang(-psi * np.sign(t_num), 0)  # inverse if -3
-
-        elif t_num in [-4, 4]:
-            dipole_direction_gse_ = _dipole_direction_gse(t, "dipole")
-
-            mu = np.arctan(
-                dipole_direction_gse_[:, 1]
-                / np.sqrt(np.sum(dipole_direction_gse_[:, 2:] ** 2, axis=1)),
-            )
-            mu = np.rad2deg(mu)
-
-            transf_mat = _triang(-mu * np.sign(t_num), 1)
-
-        elif t_num in [-5, 5]:
-            lambda_, phi = igrf(t, "dipole")
-
-            transf_mat = np.matmul(_triang(phi - 90, 1), _triang(lambda_, 2))
-            if t_num == -5:
-                transf_mat = np.transpose(transf_mat, [0, 2, 1])
-
-        else:
-            raise ValueError
-
-        if j == len(tind):
-            transf_mat_out = transf_mat
-        else:
-            transf_mat_out = np.matmul(transf_mat, transf_mat_out)
-
-    return transf_mat_out
-
-
-def cotrans(inp, flag, hapgood: bool = True):
-    r"""Coordinate transformation GE0/GEI/GSE/GSM/SM/MAG
-
-    Parameters
-    ----------
-    inp : xarray.DataArray or ndarray
-        Time series of the input field.
-    flag : str
-        Coordinates transformation "{coord1}>{coord2}", where coord1 and
-        coord2 can be geo/gei/gse/gsm/sm/mag.
-    hapgood : bool, Optional
-        Indicator if original Hapgood sources should be used for angle
-        computations or if updated USNO-AA sources should be used.
-        Default = true, meaning original Hapgood sources.
-
-
-    Examples
-    --------
-    >>> from pyrfu.mms import get_data
-    >>> from pyrfu.pyrf import cotrans
-
-    Time interval
-
-    >>> tint = ["2019-09-14T07:54:00.000", "2019-09-14T08:11:00.000"]
-
-    Spacecraft index
-
-    >>> mms_id = 1
-
-    Load magnetic field in GSE coordinates
-
-    >>> b_gse = get_data("b_gse_fgm_srvy_l2", tint, mms_id)
-
-    Transform to GSM assuming that the original coordinates system is part
-    of the inp metadata
-
-    >>> b_gsm = cotrans(b_gse, 'GSM')
-
-    If the original coordinates is not in the meta
-
-    >>> b_gsm = cotrans(b_gse, 'GSE>GSM')
-
-    Compute the dipole direction in GSE
-
-    >>> dipole = cotrans(b_gse.time,
-    'dipoledirectiongse')
-
-
-    References
-    ----------
-    .. [17]     Hapgood 1997 (corrected version of Hapgood 1992) Planet.Space
-                Sci..Vol. 40, No. 5. pp. 71l - 717, 1992
-
-    .. [18]     USNO - AA 2011 & 2012
-
-    """
-
-    if ">" in flag:
-        ref_syst_in, ref_syst_out = flag.split(">")
-    else:
-        ref_syst_in, ref_syst_out = [None, flag.lower()]
-
-    if isinstance(inp, xr.DataArray):
-        if "COORDINATE_SYSTEM" in inp.attrs:
-            ref_syst_internal = inp.attrs["COORDINATE_SYSTEM"].lower()
-            ref_syst_internal = ref_syst_internal.split(">")[0]
-        else:
-            ref_syst_internal = None
-
-        if ref_syst_in is not None and ref_syst_internal is not None:
-            message = "input ref. frame in variable and input flag differs"
-            assert ref_syst_internal == ref_syst_in, message
-        elif ref_syst_in is None and ref_syst_internal is not None:
-            ref_syst_in = ref_syst_internal.lower()
-        elif ref_syst_in is None and ref_syst_internal is None:
-            raise ValueError("input reference frame undefined")
-
-        flag = f"{ref_syst_in}>{ref_syst_out}"
-
-    if ref_syst_in == ref_syst_out:
-        return inp
-
-    # J2000 reference time
-    j2000 = 946727930.8160001
-    # j2000 = Time("J2000", format="jyear_str").unix
-
-    if isinstance(inp, xr.DataArray):
-        time = inp.time.data
-        t = time.view("i8") * 1e-9
-
-        #  Terrestial Time (seconds since J2000)
-        tts = t - j2000
-        inp_ts = inp
-        inp = inp.data
-
-    elif isinstance(inp, np.ndarray):
-        time = (inp[:, 0] * 1e9).astype("datetime64[ns]")
-        t = inp[:, 0]
-        #  Terrestial Time (seconds since J2000)
-        tts = t - j2000
-        inp_ts = None
-        inp = inp[:, 1:]
-    else:
-        raise TypeError("invalid inpu")
-
-    if hapgood:
-        day_start_epoch = time.astype("datetime64[D]")
-        day_start_epoch = day_start_epoch.astype("datetime64[ns]")
-        day_start_epoch = day_start_epoch.astype(np.int64) / 1e9
-        mjd_ref_epoch = np.datetime64("2000-01-01T12:00:00", "ns")
-        mjd_ref_epoch = mjd_ref_epoch.astype(np.int64) / 1e9
-
-        # t_zero is time measured in Julian centuries from 2000-01-0112:00 UT
-        # to the previous midnight
-        t_zero = day_start_epoch - mjd_ref_epoch
-        t_zero /= 3600 * 24 * 36525.0
-
-        hours = (time.astype("datetime64[h]") - time.astype("datetime64[D]")).astype(
-            float
-        )
-        minutes = (time.astype("datetime64[m]") - time.astype("datetime64[h]")).astype(
-            float
-        )
-        seconds = 1e-9 * (
-            time.astype("datetime64[ns]") - time.astype("datetime64[m]")
-        ).astype(np.float64)
-        ut = hours + minutes / 60 + seconds / 3600
-
-        args_trans_mat = (t_zero, ut, None, None, None, None)
-
-    else:
-        # Julian date(of req.time) from J2000
-        d_j2000 = tts / 86400
-
-        # Julian date(of preceeding midnight of req.time) from J2000
-        d0_j2000 = np.floor(tts / 86400) - 0.5
-
-        # Julian centuries(of req.time) since J2000
-        t_j2000 = d_j2000 / 36525
-
-        # Hours in the of req.time(since midnight).
-        h_j2000 = 24 * (d_j2000 - d0_j2000)
-
-        args_trans_mat = (None, None, d0_j2000, d_j2000, h_j2000, t_j2000)
-
-    if ">" in flag:
-        root_path = os.path.dirname(os.path.abspath(__file__))
-        file_name = "transformation_indices.json"
-
-        with open(os.sep.join([root_path, file_name]), "r", encoding="utf-8") as file:
-            transformation_dict = json.load(file)
-
-        tind = transformation_dict[flag]
-
-    elif flag == "dipoledirectiongse":
-        out_data = _dipole_direction_gse(t)
-        return ts_vec_xyz(inp.time.data, out_data)
-
-    else:
-        raise ValueError(f"Transformation {flag} is unknown!")
-
-    transf_mat = _transformation_matrix(t, tind, hapgood, *args_trans_mat)
-
-    if inp.ndim == 2:
-        out = np.einsum("kji,ki->kj", transf_mat, inp)
-    elif inp.ndim == 1:
-        out = transf_mat
-    else:
-        raise ValueError
-
-    if inp_ts is not None:
-        out_data = out
-        out = inp_ts.copy()
-        out.data = out_data
-        out.attrs["COORDINATE_SYSTEM"] = ref_syst_out.upper()
-
-    else:
-        out = np.hstack([t[:, None], out])
-
-    return out
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+import json
+
+# Built-in imports
+import os
+
+# 3rd party imports
+import numpy as np
+import xarray as xr
+
+# Local imports
+from ..models import igrf
+from .ts_vec_xyz import ts_vec_xyz
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def _triang(angle, axis):
+    cos_angle = np.cos(np.deg2rad(angle))
+    sin_angle = np.sin(np.deg2rad(angle))
+
+    axes = list(filter(lambda x: x != axis, np.arange(3)))
+
+    transf_mat = np.zeros((len(angle), 3, 3))
+    transf_mat[:, axes[0], axes[0]] = cos_angle
+    transf_mat[:, axes[1], axes[1]] = cos_angle
+    transf_mat[:, axis, axis] = 1
+    transf_mat[:, axes[0], axes[1]] = sin_angle
+    transf_mat[:, axes[1], axes[0]] = -sin_angle
+
+    return transf_mat
+
+
+def _dipole_direction_gse(time, flag: str = "dipole"):
+    lambda_, phi = igrf(time, flag)
+
+    cos_phi = np.cos(np.deg2rad(phi))
+    dipole_direction_geo_ = np.stack(
+        [
+            cos_phi * np.cos(np.deg2rad(lambda_)),
+            cos_phi * np.sin(np.deg2rad(lambda_)),
+            np.sin(np.deg2rad(phi)),
+        ],
+    ).T
+
+    dipole_direction_gse_ = cotrans(
+        np.hstack([time[:, None], dipole_direction_geo_]),
+        "geo>gse",
+    )
+
+    return dipole_direction_gse_
+
+
+def _transformation_matrix(t, tind, hapgood, *args):
+    t_zero, ut, d0_j2000, d_j2000, h_j2000, t_j2000 = args
+
+    transf_mat_out = np.zeros((len(t), 3, 3))
+    transf_mat_out[:, 0, 0] = np.ones(len(t))
+    transf_mat_out[:, 1, 1] = np.ones(len(t))
+    transf_mat_out[:, 2, 2] = np.ones(len(t))
+
+    for j, t_num in enumerate(tind[::-1]):
+        if t_num in [-1, 1]:
+            if hapgood:
+                theta = 100.461 + 36000.770 * t_zero + 15.04107 * ut
+
+            else:
+                # Source: United States Naval Observatory, Astronomical
+                # Applications Dept. http: // aa.usno.navy.mil / faq / docs
+                # / GAST.php Last modified: 2011/06/14T14:04
+                gmst = 6.697374558
+                gmst += 0.06570982441908 * d0_j2000
+                gmst += 1.00273790935 * h_j2000
+                gmst += 0.000026 * t_j2000**2
+
+                gmst = gmst % 24  # Interval 0->24 hours
+                theta = (360 / 24) * gmst  # Convert to degree.
+
+            # invert if tInd = -1
+            transf_mat = _triang(theta * np.sign(t_num), 2)
+
+        elif t_num in [-2, 2]:
+            if hapgood:
+                eps = 23.439 - 0.013 * t_zero
+                # Suns mean anomaly
+                m_anom = 357.528 + 35999.050 * t_zero + 0.04107 * ut
+                # Suns mean longitude
+                m_long = 280.460 + 36000.772 * t_zero + 0.04107 * ut
+                l_sun = m_long
+                l_sun += (1.915 - 0.0048 * t_zero) * np.sin(
+                    np.deg2rad(m_anom),
+                )
+                l_sun += 0.020 * np.sin(np.deg2rad(2 * m_anom))
+            else:
+                # Source: United States Naval Observatory, Astronomical
+                # Applications Dept.
+                # http://aa.usno.navy.mil/faq/docsSunApprox.php.
+                # Last modified: 2012/11/06T14:12
+                eps = 23.439 - 0.00000036 * d_j2000
+                m_anom = 357.529 + 0.98560028 * d_j2000
+                m_long = 280.459 + 0.98564736 * d_j2000
+                l_sun = m_long
+                l_sun += 1.915 * np.sin(np.deg2rad(m_anom))
+                l_sun += 0.020 * np.sin(np.deg2rad(2 * m_anom))
+
+            transf_mat = np.matmul(_triang(l_sun, 2), _triang(eps, 0))
+            if t_num == -2:
+                transf_mat = np.transpose(transf_mat, [0, 2, 1])
+
+        elif t_num in [-3, 3]:
+            dipole_direction_gse_ = _dipole_direction_gse(t, "dipole")
+            y_e = dipole_direction_gse_[:, 2]  # 1st col is time
+            z_e = dipole_direction_gse_[:, 3]
+            psi = np.rad2deg(np.arctan(y_e / z_e))
+
+            transf_mat = _triang(-psi * np.sign(t_num), 0)  # inverse if -3
+
+        elif t_num in [-4, 4]:
+            dipole_direction_gse_ = _dipole_direction_gse(t, "dipole")
+
+            mu = np.arctan(
+                dipole_direction_gse_[:, 1]
+                / np.sqrt(np.sum(dipole_direction_gse_[:, 2:] ** 2, axis=1)),
+            )
+            mu = np.rad2deg(mu)
+
+            transf_mat = _triang(-mu * np.sign(t_num), 1)
+
+        elif t_num in [-5, 5]:
+            lambda_, phi = igrf(t, "dipole")
+
+            transf_mat = np.matmul(_triang(phi - 90, 1), _triang(lambda_, 2))
+            if t_num == -5:
+                transf_mat = np.transpose(transf_mat, [0, 2, 1])
+
+        else:
+            raise ValueError
+
+        if j == len(tind):
+            transf_mat_out = transf_mat
+        else:
+            transf_mat_out = np.matmul(transf_mat, transf_mat_out)
+
+    return transf_mat_out
+
+
+def cotrans(inp, flag, hapgood: bool = True):
+    r"""Coordinate transformation GE0/GEI/GSE/GSM/SM/MAG
+
+    Parameters
+    ----------
+    inp : xarray.DataArray or ndarray
+        Time series of the input field.
+    flag : str
+        Coordinates transformation "{coord1}>{coord2}", where coord1 and
+        coord2 can be geo/gei/gse/gsm/sm/mag.
+    hapgood : bool, Optional
+        Indicator if original Hapgood sources should be used for angle
+        computations or if updated USNO-AA sources should be used.
+        Default = true, meaning original Hapgood sources.
+
+
+    Examples
+    --------
+    >>> from pyrfu.mms import get_data
+    >>> from pyrfu.pyrf import cotrans
+
+    Time interval
+
+    >>> tint = ["2019-09-14T07:54:00.000", "2019-09-14T08:11:00.000"]
+
+    Spacecraft index
+
+    >>> mms_id = 1
+
+    Load magnetic field in GSE coordinates
+
+    >>> b_gse = get_data("b_gse_fgm_srvy_l2", tint, mms_id)
+
+    Transform to GSM assuming that the original coordinates system is part
+    of the inp metadata
+
+    >>> b_gsm = cotrans(b_gse, 'GSM')
+
+    If the original coordinates is not in the meta
+
+    >>> b_gsm = cotrans(b_gse, 'GSE>GSM')
+
+    Compute the dipole direction in GSE
+
+    >>> dipole = cotrans(b_gse.time,
+    'dipoledirectiongse')
+
+
+    References
+    ----------
+    .. [17]     Hapgood 1997 (corrected version of Hapgood 1992) Planet.Space
+                Sci..Vol. 40, No. 5. pp. 71l - 717, 1992
+
+    .. [18]     USNO - AA 2011 & 2012
+
+    """
+
+    if ">" in flag:
+        ref_syst_in, ref_syst_out = flag.split(">")
+    else:
+        ref_syst_in, ref_syst_out = [None, flag.lower()]
+
+    if isinstance(inp, xr.DataArray):
+        if "COORDINATE_SYSTEM" in inp.attrs:
+            ref_syst_internal = inp.attrs["COORDINATE_SYSTEM"].lower()
+            ref_syst_internal = ref_syst_internal.split(">")[0]
+        else:
+            ref_syst_internal = None
+
+        if ref_syst_in is not None and ref_syst_internal is not None:
+            message = "input ref. frame in variable and input flag differs"
+            assert ref_syst_internal == ref_syst_in, message
+        elif ref_syst_in is None and ref_syst_internal is not None:
+            ref_syst_in = ref_syst_internal.lower()
+        elif ref_syst_in is None and ref_syst_internal is None:
+            raise ValueError("input reference frame undefined")
+
+        flag = f"{ref_syst_in}>{ref_syst_out}"
+
+    if ref_syst_in == ref_syst_out:
+        return inp
+
+    # J2000 reference time
+    j2000 = 946727930.8160001
+    # j2000 = Time("J2000", format="jyear_str").unix
+
+    if isinstance(inp, xr.DataArray):
+        time = inp.time.data
+        t = time.view("i8") * 1e-9
+
+        #  Terrestial Time (seconds since J2000)
+        tts = t - j2000
+        inp_ts = inp
+        inp = inp.data
+
+    elif isinstance(inp, np.ndarray):
+        time = (inp[:, 0] * 1e9).astype("datetime64[ns]")
+        t = inp[:, 0]
+        #  Terrestial Time (seconds since J2000)
+        tts = t - j2000
+        inp_ts = None
+        inp = inp[:, 1:]
+    else:
+        raise TypeError("invalid inpu")
+
+    if hapgood:
+        day_start_epoch = time.astype("datetime64[D]")
+        day_start_epoch = day_start_epoch.astype("datetime64[ns]")
+        day_start_epoch = day_start_epoch.astype(np.int64) / 1e9
+        mjd_ref_epoch = np.datetime64("2000-01-01T12:00:00", "ns")
+        mjd_ref_epoch = mjd_ref_epoch.astype(np.int64) / 1e9
+
+        # t_zero is time measured in Julian centuries from 2000-01-0112:00 UT
+        # to the previous midnight
+        t_zero = day_start_epoch - mjd_ref_epoch
+        t_zero /= 3600 * 24 * 36525.0
+
+        hours = (time.astype("datetime64[h]") - time.astype("datetime64[D]")).astype(
+            float
+        )
+        minutes = (time.astype("datetime64[m]") - time.astype("datetime64[h]")).astype(
+            float
+        )
+        seconds = 1e-9 * (
+            time.astype("datetime64[ns]") - time.astype("datetime64[m]")
+        ).astype(np.float64)
+        ut = hours + minutes / 60 + seconds / 3600
+
+        args_trans_mat = (t_zero, ut, None, None, None, None)
+
+    else:
+        # Julian date(of req.time) from J2000
+        d_j2000 = tts / 86400
+
+        # Julian date(of preceeding midnight of req.time) from J2000
+        d0_j2000 = np.floor(tts / 86400) - 0.5
+
+        # Julian centuries(of req.time) since J2000
+        t_j2000 = d_j2000 / 36525
+
+        # Hours in the of req.time(since midnight).
+        h_j2000 = 24 * (d_j2000 - d0_j2000)
+
+        args_trans_mat = (None, None, d0_j2000, d_j2000, h_j2000, t_j2000)
+
+    if ">" in flag:
+        root_path = os.path.dirname(os.path.abspath(__file__))
+        file_name = "transformation_indices.json"
+
+        with open(os.sep.join([root_path, file_name]), "r", encoding="utf-8") as file:
+            transformation_dict = json.load(file)
+
+        tind = transformation_dict[flag]
+
+    elif flag == "dipoledirectiongse":
+        out_data = _dipole_direction_gse(t)
+        return ts_vec_xyz(inp.time.data, out_data)
+
+    else:
+        raise ValueError(f"Transformation {flag} is unknown!")
+
+    transf_mat = _transformation_matrix(t, tind, hapgood, *args_trans_mat)
+
+    if inp.ndim == 2:
+        out = np.einsum("kji,ki->kj", transf_mat, inp)
+    elif inp.ndim == 1:
+        out = transf_mat
+    else:
+        raise ValueError
+
+    if inp_ts is not None:
+        out_data = out
+        out = inp_ts.copy()
+        out.data = out_data
+        out.attrs["COORDINATE_SYSTEM"] = ref_syst_out.upper()
+
+    else:
+        out = np.hstack([t[:, None], out])
+
+    return out
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/cross.py` & `pyrfu-2.4.3/pyrfu/pyrf/cross.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 # Local imports
 from .resample import resample
 from .ts_vec_xyz import ts_vec_xyz
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def cross(inp1, inp2):
     r"""Computes cross product of two fields.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/date_str.py` & `pyrfu-2.4.3/pyrfu/pyrf/date_str.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # Built-in imports
 from datetime import datetime
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def date_str(tint, fmt: int = 1):
     r"""Creates a string corresponding to time interval for output plot naming.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/datetime2iso8601.py` & `pyrfu-2.4.3/pyrfu/pyrf/datetime2iso8601.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import pandas as pd
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def datetime2iso8601(time):
     r"""Transforms datetime to TT2000 string format.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/datetime642iso8601.py` & `pyrfu-2.4.3/pyrfu/pyrf/datetime642iso8601.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def datetime642iso8601(time):
     r"""Convert datetime64 in ns units to ISO 8601 time format .
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/datetime642ttns.py` & `pyrfu-2.4.3/pyrfu/pyrf/datetime642ttns.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from cdflib import cdfepoch
 
 # local imports
 from .datetime642iso8601 import datetime642iso8601
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def datetime642ttns(time):
     r"""Converts datetime64 in ns units to epoch_tt2000
     (nanoseconds since J2000).
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/datetime642unix.py` & `pyrfu-2.4.3/pyrfu/pyrf/datetime642unix.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def datetime642unix(time):
     r"""Converts datetime64 in ns units to unix time.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/dec_par_perp.py` & `pyrfu-2.4.3/pyrfu/pyrf/dec_par_perp.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from .dot import dot
 
 # Local imports
 from .resample import resample
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def dec_par_perp(inp, b_bgd, flag_spin_plane: bool = False):
     r"""Decomposes a vector into par/perp to B components. If flagspinplane
     decomposes components to the projection of ``b0`` into the XY plane.
     ``alpha`` gives the angle between ``b0`` and the XY. plane.
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/dot.py` & `pyrfu-2.4.3/pyrfu/pyrf/dot.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 # Local imports
 from .resample import resample
 from .ts_scalar import ts_scalar
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def dot(inp1, inp2):
     r"""Computes dot product of two fields.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/dynamic_press.py` & `pyrfu-2.4.3/pyrfu/pyrf/dynamic_press.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # 3rd party imports
 import numpy as np
 from scipy import constants
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def dynamic_press(n_s, v_xyz, specie: str = "i"):
     r"""Computes dynamic pressure.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/e_vxb.py` & `pyrfu-2.4.3/pyrfu/pyrf/e_vxb.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 # Local imports
 from .resample import resample
 from .ts_vec_xyz import ts_vec_xyz
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def e_vxb(v_xyz, b_xyz, flag: str = "vxb"):
     r"""Computes the convection electric field :math:`V\times B` (default)
     or the :math:`E\times B/|B|^{2}` drift velocity (flag="exb").
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/eb_nrf.py` & `pyrfu-2.4.3/pyrfu/pyrf/eb_nrf.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from .normalize import normalize
 
 # Local imports
 from .resample import resample
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def eb_nrf(e_xyz, b_xyz, v_xyz, flag=0):
     """Find E and B in MP system given B and MP normal vector.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/ebsp.py` & `pyrfu-2.4.3/pyrfu/pyrf/ebsp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1044 +1,1044 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Built-in imports
-import logging
-import os
-import warnings
-
-# 3rd party imports
-import numba
-import numpy as np
-import xarray as xr
-from scipy import fft
-
-from .calc_fs import calc_fs
-from .cart2sph import cart2sph
-from .convert_fac import convert_fac
-from .datetime642iso8601 import datetime642iso8601
-from .iso2unix import iso2unix
-from .resample import resample
-
-# Local imports
-from .ts_time import ts_time
-from .ts_vec_xyz import ts_vec_xyz
-from .unix2datetime64 import unix2datetime64
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2023"
-__license__ = "MIT"
-__version__ = "2.3.29"
-__status__ = "Prototype"
-
-logging.captureWarnings(True)
-logging.basicConfig(
-    format="[%(asctime)s] %(levelname)s: %(message)s",
-    datefmt="%d-%b-%y %H:%M:%S",
-    level=logging.INFO,
-)
-
-
-def _checksampling(e_xyz, db_xyz, b_xyz, b_bgd, flag_no_resamp):
-    assert e_xyz is not None
-
-    fs_e, fs_b = [calc_fs(e_xyz), calc_fs(db_xyz)]
-
-    resample_b_options = {"f_s": fs_b}
-
-    if flag_no_resamp:
-        assert fs_e == fs_b
-        fs_ = fs_e
-    else:
-        if fs_b > 1.5 * fs_e:
-            e_xyz = resample(e_xyz, db_xyz, **resample_b_options)
-            b_bgd = resample(b_bgd, db_xyz, **resample_b_options)
-
-            fs_ = fs_b
-            logging.info("Interpolating e to b")
-        elif fs_e > 1.5 * fs_b:
-            db_xyz = resample(db_xyz, e_xyz)
-            b_bgd = resample(b_bgd, e_xyz)
-
-            fs_ = fs_e
-            logging.info("Interpolating b to e")
-        elif fs_e == fs_b and len(e_xyz) == len(db_xyz):
-            fs_ = fs_e
-        else:
-            fs_ = 2 * fs_e
-            start_time = np.max(
-                [
-                    e_xyz.time.data[0].astype(int) / 1e9,
-                    db_xyz.time.data[0].astype(int) / 1e9,
-                ]
-            )
-            end_time = np.min(
-                [
-                    e_xyz.time.data[-1].astype(int) / 1e9,
-                    db_xyz.time.data[-1].astype(int) / 1e9,
-                ]
-            )
-
-            nt = int((end_time - start_time) * fs_)
-
-            t = np.linspace(start_time, end_time, nt)
-
-            t = ts_time(t)
-
-            e_xyz = resample(e_xyz, t)
-            b_bgd = resample(b_bgd, t)
-            b_xyz = resample(b_xyz, t)
-            db_xyz = resample(db_xyz, t)
-
-            logging.info("Interpolating b and e to 2x e sampling")
-
-    return e_xyz, db_xyz, b_xyz, b_bgd, fs_
-
-
-def _b_elevation(b_x, b_y, b_z, angle_b_elevation_max):
-    # Remove the last sample if the total number of samples is odd
-    b_x = b_x[: int(2 * (len(b_x) // 2)), :]
-    b_y = b_y[: int(2 * (len(b_y) // 2)), :]
-    b_z = b_z[: int(2 * (len(b_z) // 2)), :]
-
-    angle_b_elevation = np.arctan(b_z / np.sqrt(b_x**2 + b_y**2))
-    angle_b_elevation = np.rad2deg(angle_b_elevation)
-    idx_b_par_spin_plane = np.abs(angle_b_elevation) < angle_b_elevation_max
-
-    return angle_b_elevation, idx_b_par_spin_plane
-
-
-def _freq_int(freq_int, delta_b):
-    start_time = delta_b.time.data[0].astype(int) / 1e9
-    end_time = delta_b.time.data[-1].astype(int) / 1e9
-
-    pc12_range, pc35_range, other_range = [False, False, False]
-
-    if isinstance(freq_int, str):
-        if freq_int.lower() == "pc12":
-            pc12_range = True
-
-            freq_int = [0.1, 5]
-
-            delta_t = 1  # local
-
-            tint = np.round([start_time, end_time])
-            tint = list(datetime642iso8601(unix2datetime64(tint)))
-
-        elif freq_int.lower() == "pc35":
-            pc35_range = True
-
-            freq_int = [0.002, 0.1]
-
-            delta_t = 60  # local
-
-            tint = 60 * np.array([np.round(start_time / 60), np.round(end_time / 60)])
-            tint = datetime642iso8601(unix2datetime64(tint))
-
-        else:
-            raise ValueError("Invalid format of interval")
-
-        fs_out = 1 / delta_t
-
-        nt = np.round((iso2unix(tint[1]) - iso2unix(tint[0])) / delta_t)
-        nt = nt.astype(int)  # local
-
-        out_time = np.linspace(iso2unix(tint[0]), iso2unix(tint[1]), nt)
-        out_time += delta_t / 2
-        out_time = out_time[:-1]
-    else:
-        if freq_int[1] >= freq_int[0]:
-            other_range = True
-
-            fs_out = freq_int[1] / 5
-
-            delta_t = 1 / fs_out  # local
-
-            nt = np.round((end_time - start_time) / delta_t).astype(int)
-
-            out_time = np.linspace(start_time, end_time, nt)
-            out_time += delta_t / 2
-            out_time = out_time[:-1]
-        else:
-            raise ValueError("FREQ_INT must be [f_min f_max], f_min<f_max")
-
-    any_range = [pc12_range, pc35_range, other_range]
-
-    return any_range, freq_int, fs_out, out_time
-
-
-@numba.jit(cache=True, nogil=True, parallel=True, nopython=True, fastmath=True)
-def _average_data(data=None, x=None, y=None, av_window=None):
-    # average data with time x to time y using window
-
-    dtx, dty = [np.median(np.diff(x)), np.median(np.diff(y))]
-
-    if av_window is None:
-        av_window = dty
-
-    dt2 = av_window / 2
-
-    n_data_out = len(y)
-
-    # Pad data with NaNs from each side
-    n_point_to_add = int(np.ceil(dt2 / dtx))
-    pad_nan = np.ones((n_point_to_add, data.shape[1]), dtype="complex128") * np.nan
-    data_padded = np.vstack((pad_nan, data, pad_nan))
-
-    x_pad_pref = np.linspace(x[0] - dtx * (n_point_to_add - 1), x[0], n_point_to_add)
-    x_pad_suff = np.linspace(x[-1], x[-1] + dtx * (n_point_to_add - 1), n_point_to_add)
-    x_padded = np.hstack((x_pad_pref, x, x_pad_suff))
-
-    out = np.zeros((n_data_out, data.shape[1]), dtype="complex128")
-
-    il = np.digitize(y - dt2, x_padded)
-    ir = np.digitize(y + dt2, x_padded)
-
-    for i in numba.prange(len(y)):
-        for j in range(data.shape[1]):
-            out[i, j] = np.nanmean(data_padded[il[i] : ir[i], j])
-
-    return out
-
-
-def _bb_xxyyzzss(power_bx_plot, power_by_plot, power_bz_plot, power_2b_plot):
-    bb_xxyyzzss = np.tile(power_bx_plot[:, :, np.newaxis], (1, 1, 4))
-    bb_xxyyzzss[:, :, 1] = power_by_plot
-    bb_xxyyzzss[:, :, 2] = power_bz_plot
-    bb_xxyyzzss[:, :, 3] = power_2b_plot
-    return np.real(bb_xxyyzzss)
-
-
-def _ee_xxyyzzss(power_ex_plot, power_ey_plot, power_ez_plot, power_2e_plot):
-    ee_xxyyzzss = np.tile(power_ex_plot[..., np.newaxis], (1, 1, 4))
-    ee_xxyyzzss[:, :, 1] = power_ey_plot
-    ee_xxyyzzss[:, :, 2] = power_ez_plot
-    ee_xxyyzzss[:, :, 3] = power_2e_plot
-    return np.real(ee_xxyyzzss)
-
-
-@numba.jit(cache=True, nogil=True, parallel=True, nopython=True, fastmath=True)
-def _censure_plot(inp, idx_nan, censure, n_data, a_):
-    out = inp.copy()
-
-    for i in numba.prange(len(idx_nan) - 1):
-        for j in range(len(a_)):
-            if idx_nan[i] < idx_nan[i + 1]:
-                out[int(max([i - censure[j], 0])) : i, j] = np.nan
-
-            if idx_nan[i] > idx_nan[i + 1]:
-                out[i : int(min([i + censure[j], n_data])), j] = np.nan
-
-    return out
-
-
-def ebsp(e_xyz, db_xyz, b_xyz, b_bgd, xyz, freq_int, **kwargs):
-    """Calculates wavelet spectra of E&B and Poynting flux using wavelets
-    (Morlet wavelet). Also computes polarization parameters of B using SVD
-    [7]_. SVD is performed on spectral matrices computed from the time series
-    of B using wavelets and then averaged over a number of wave periods.
-
-    Parameters
-    ----------
-    e_xyz : xarray.DataArray
-        Time series of the wave electric field.
-    db_xyz : xarray.DataArray
-        Time series of the wave magnetic field.
-    b_xyz : xarray.DataArray
-        Time series of the high resolution background magnetic field used
-        for E.B=0.
-    b_bgd : xarray.DataArray
-        Time series of the background magnetic field used for field aligned
-        coordinates.
-    xyz : xarray.DataArray
-        Time series of the position time series of spacecraft used for field
-        aligned coordinates.
-    freq_int : str or array_like
-        Frequency interval :
-            * "pc12" : [0.1, 5.0]
-            * "pc35" : [2e-3, 0.1]
-            * [fmin, fmax] : arbitrary interval [fmin,fmax]
-
-    Returns
-    -------
-    res : xarray.Dataset
-        Dataset with :
-            * t : xarray.DataArray
-                Time.
-            * f : xarray.DataArray
-                Frequencies.
-            * bb_xxyyzzss : xarray.DataArray
-                delta_b power spectrum with :
-                    * [...,0] : x
-                    * [...,1] : y
-                    * [...,2] : z
-                    * [...,3] : sum
-            * ee_xxyyzzss : xarray.DataArray
-                E power spectrum with :
-                    * [...,0] : x
-                    * [...,1] : y
-                    * [...,2] : z
-                    * [...,3] : sum
-            * ee_ss : xarray.DataArray
-                E power spectrum (xx+yy spacecraft coordinates, e.g. ISR2).
-            * pf_xyz : xarray.DataArray
-                Poynting flux (xyz).
-            * pf_rtp : xarray.DataArray
-                Poynting flux (r, theta, phi) [angles in degrees].
-            * dop : xarray.DataArray
-                3D degree of polarization.
-            * dop2d : xarray.DataArray
-                2D degree of polarization in the polarization plane.
-            * planarity : xarray.DataArray
-                Planarity of polarization.
-            * ellipticity : xarray.DataArray
-                Ellipticity of polarization ellipse.
-            * k : xarray.DataArray
-                k-vector (theta, phi FAC) [angles in degrees].
-
-    Other Parameters
-    ----------------
-    polarization : bool
-        Computes polarization parameters. Default False.
-    noresamp : bool
-        No resampling, E and delta_b are given at the same time line.
-        Default False.
-    fac : bool
-        Uses FAC coordinate system (defined by b0 and optionally xyz),
-        otherwise no coordinate system transformation is performed. Default
-        False.
-    de_dot_b0 : bool
-        Computes dEz from delta_b dot B = 0, uses full_b. Default False.
-    full_b_db : bool
-        delta_b contains DC field. Default False.
-    nav : int
-        Number of wave periods to average Default 8.
-    fac_matrix : numpy.ndarray
-        Specify rotation matrix to FAC system Default None.
-    m_width_coeff : int or float
-        Specify coefficient to multiple Morlet wavelet width by. Default 1.
-
-    See also
-    --------
-    pyrfu.plot.pl_ebsp : to fill.
-    pyrfu.pyrf.convert_fac : Transforms to a field-aligned coordinate.
-
-    Notes
-    -----
-    This software was developed as part of the MAARBLE (Monitoring, Analyzing
-    and Assessing Radiation Belt Energization and Loss) collaborative
-    research project which has received funding from the European
-    Community's Seventh Framework Programme (FP7-SPACE-2011-1) under grant
-    agreement n. 284520.
-
-    References
-    ----------
-    .. [7] 	Santolík, O., Parrot. M., and  Lefeuvre. F. (2003) Singular value
-            decomposition methods for wave propagation analysis,Radio Sci.,
-            38(1), 1010, doi : https://doi.org/10.1029/2000RS002523 .
-
-    Examples
-    --------
-    >>> from pyrfu import mms, pyrf
-    >>> # Time interval
-    >>> tint_brst = ["2015-10-30T05:15:42.000", "2015-10-30T05:15:54.000"]
-    >>> # Spacecraft index
-    >>> mms_id = 3
-    >>> # Load spacecraft position
-    >>> tint_long = pyrf.extend_tint(tint_brst, [-100, 100])
-    >>> r_xyz = mms.get_data("R_gse", tint_long, mms_id)
-    >>> # Load background magnetic field, electric field and magnetic field
-    fluctuations
-    >>> b_xyz = mms.get_data("B_gse_fgm_brst_l2", tint_brst, mms_id)
-    >>> e_xyz = mms.get_data("E_gse_edp_brst_l2", tint_brst, mms_id)
-    >>> b_scm = mms.get_data("B_gse_scm_brst_l2", tint_brst, mms_id)
-    >>> # Polarization analysis
-    >>> options = dict(polarization=True, fac=True)
-    >>> polarization = pyrf.ebsp(e_xyz, b_scm, b_xyz, b_xyz, r_xyz,
-    >>>                          freq_int=[10, 4000], **options)
-
-    """
-
-    assert isinstance(db_xyz, xr.DataArray), "delta_b must be a DataArray"
-    assert isinstance(b_xyz, xr.DataArray), "full_b must be a DataArray"
-    assert isinstance(b_bgd, xr.DataArray), "b0 must be a DataArray"
-    assert isinstance(xyz, xr.DataArray), "xyz must be a DataArray"
-
-    # Compute magnetic field fluctuations sampling frequency
-    fs_b = calc_fs(db_xyz)
-
-    # Below which we cannot apply E*B=0
-    angle_b_elevation_max = 15.0
-
-    want_ee = e_xyz is not None
-
-    res = {
-        "t": None,
-        "f": None,
-        "flagFac": 0,
-        "bb_xxyyzzss": None,
-        "ee_xxyyzzss": None,
-        "ee_ss": None,
-        "pf_xyz": None,
-        "pf_rtp": None,
-        "dop": None,
-        "dop2d": None,
-        "planarity": None,
-        "ellipticity": None,
-        "k_tp": None,
-        "full_b": b_xyz,
-        "b0": b_bgd,
-        "r": xyz,
-    }
-
-    want_polarization = kwargs.get("polarization", False)
-
-    flag_no_resample = kwargs.get("no_resample", False)
-    flag_want_fac = kwargs.get("fac", False)
-    flag_de_dot_b0 = kwargs.get("de_dot_b0", False)
-    flag_full_b_db = kwargs.get("full_b_db", False)
-
-    m_width_coeff = kwargs.get("m_width_coeff", 1.0)
-
-    # Number of wave periods to average
-    n_wave_period_to_average = kwargs.get("nav", 8)
-
-    # matrix for rotation to FAC
-    fac_matrix = kwargs.get("fac_matrix", None)
-
-    if flag_want_fac and fac_matrix is None:
-        if b_bgd is None:
-            raise ValueError("ebsp(): at least b0 should be given for option FAC")
-
-        if xyz is None:
-            logging.info(
-                "convert_fac : assuming s/c position [1 0 0] for estimating FAC"
-            )
-            xyz = [1, 0, 0]
-            xyz = ts_vec_xyz(db_xyz.time.data, np.tile(xyz, (len(db_xyz), 1)))
-
-        xyz = resample(xyz, db_xyz, **{"f_s": fs_b})
-
-    b_bgd = resample(b_bgd, db_xyz, **{"f_s": fs_b})
-
-    if flag_full_b_db:
-        b_xyz = db_xyz
-        res["full_b"] = b_xyz
-        db_xyz = db_xyz - b_bgd
-
-    if flag_de_dot_b0 and b_xyz is None:
-        raise ValueError("full_b must be given for option de_dot_b0=0")
-
-    any_range, freq_int, out_sampling, out_time = _freq_int(freq_int, db_xyz)
-    pc12_range, pc35_range, other_range = any_range
-
-    if want_ee:
-        # Check the sampling rate
-        temp_ = _checksampling(e_xyz, db_xyz, b_xyz, b_bgd, flag_no_resample)
-        e_xyz, db_xyz, b_xyz, b_bgd, in_sampling = temp_
-
-    else:
-        in_sampling = calc_fs(db_xyz)
-
-        e_xyz = None
-
-    if in_sampling / 2 < freq_int[1]:
-        raise ValueError("F_MAX must be lower than the Nyquist frequency")
-
-    if want_ee and e_xyz.shape[1] < 3 and not flag_de_dot_b0:
-        raise ValueError(
-            "E must have all 3 components or flag de_dot_db=0 must be given"
-        )
-
-    if len(db_xyz) % 2:
-        db_xyz = db_xyz[:-1, :]
-        b_bgd = b_bgd[:-1, :]
-
-        if fac_matrix is None:
-            xyz = xyz[:-1, :]
-        else:
-            fac_matrix["t"] = fac_matrix["t"][:-1, :]
-
-            fac_matrix["rotMatrix"] = fac_matrix["rotMatrix"][:-1, :, :]
-
-        if want_ee:
-            e_xyz = e_xyz[:-1, :]
-
-    in_time = db_xyz.time.data.astype("int64") / 1e9
-
-    b_x, b_y, b_z = [None, None, None]
-
-    idx_b_par_spin_plane = None
-
-    if flag_de_dot_b0:
-        b_x, b_y, b_z = [b_xyz[:, i].data for i in range(3)]
-
-        # Remove the last sample if the total number of samples is odd
-        # temp_ = _b_elevation(b_x, b_y, b_z, angle_b_elevation_max)
-        # angle_b_elevation, idx_b_par_spin_plane = temp_
-        _, idx_b_par_spin_plane = _b_elevation(b_x, b_y, b_z, angle_b_elevation_max)
-
-    # If E has all three components, transform E and B waveforms to a magnetic
-    # field aligned coordinate (FAC) and save eisr for computation of e_sum.
-    # Otherwise we compute Ez within the main loop and do the transformation
-    # to FAC there.
-
-    time_b0 = 0
-    if flag_want_fac:
-        res["flagFac"] = True
-
-        time_b0 = b_bgd.time.data.astype("int64") / 1e9
-
-        if want_ee and not flag_de_dot_b0:
-            eisr2 = e_xyz[:, :2]
-            idx_nan_e = np.isnan(e_xyz.data)
-            idx_nan_eisr2 = np.isnan(eisr2.data)
-
-            if e_xyz.shape[1] < 3:
-                raise TypeError("E must be a 3D vector to be rotated to FAC")
-
-            if fac_matrix is None:
-                e_xyz = convert_fac(e_xyz, b_bgd, xyz)
-            else:
-                e_xyz = convert_fac(e_xyz, fac_matrix)
-
-        else:
-            idx_nan_e = None
-            eisr2 = None
-            idx_nan_eisr2 = None
-
-        if fac_matrix is None:
-            db_xyz = convert_fac(db_xyz, b_bgd, xyz)
-        else:
-            db_xyz = convert_fac(db_xyz, fac_matrix)
-    else:
-        idx_nan_e = None
-        eisr2 = None
-        idx_nan_eisr2 = None
-
-    # Find the frequencies for an FFT of all data and set important parameters
-    nd2 = len(in_time) / 2
-
-    freq = in_sampling * np.arange(nd2) / nd2 * 0.5
-
-    # The frequencies corresponding to FFT
-    w_ = np.hstack([0, freq, -np.flip(freq[:-1])])
-
-    morlet_width = 5.36 * m_width_coeff
-
-    # to get proper overlap for Morlet
-    freq_number = np.ceil(
-        (np.log10(freq_int[1]) - np.log10(freq_int[0])) * 12 * m_width_coeff
-    )
-
-    a_min, a_max = [
-        np.log10(0.5 * in_sampling / freq_int[1]),
-        np.log10(0.5 * in_sampling / freq_int[0]),
-    ]
-
-    a_number = freq_number
-    a_ = np.logspace(a_min, a_max, int(a_number))
-
-    # Maximum frequency
-    w_0 = in_sampling / 2
-
-    # Width of the Morlet wavelet
-    sigma = morlet_width / w_0
-
-    # Make the FFT of all data
-    idx_nan_b = np.isnan(db_xyz.data)
-
-    db_xyz.data[idx_nan_b] = 0
-
-    swb = fft.fft(db_xyz.data, axis=0, workers=os.cpu_count())
-
-    sw_e, sw_eisr2 = [None, None]
-
-    if want_ee:
-        logging.info("ebsp ... calculate E and B wavelet transform ... ")
-        e_xyz.data[idx_nan_e] = 0.0
-
-        sw_e = fft.fft(e_xyz.data, axis=0, workers=os.cpu_count())
-
-        if flag_want_fac and not flag_de_dot_b0:
-            eisr2.data[idx_nan_eisr2] = 0.0
-
-            sw_eisr2 = fft.fft(eisr2.data, axis=0, workers=os.cpu_count())
-    else:
-        logging.info("ebsp ... calculate B wavelet transform ....")
-
-    # Loop through all frequencies
-    n_data, n_freq, n_data_out = [len(in_time), len(a_), len(out_time)]
-
-    #
-    power_ex_plot = np.zeros((n_data, n_freq), dtype="complex128")
-    power_ey_plot = np.zeros((n_data, n_freq), dtype="complex128")
-    power_ez_plot = np.zeros((n_data, n_freq), dtype="complex128")
-    power_2e_plot = np.zeros((n_data, n_freq), dtype="complex128")
-    power_2e_isr2_plot = np.zeros((n_data, n_freq), dtype="complex128")
-
-    power_bx_plot = np.zeros((n_data, n_freq), dtype="complex128")
-    power_by_plot = np.zeros((n_data, n_freq), dtype="complex128")
-    power_bz_plot = np.zeros((n_data, n_freq), dtype="complex128")
-    power_2b_plot = np.zeros((n_data, n_freq), dtype="complex128")
-
-    s_plot_x = np.zeros((n_data, n_freq))
-    s_plot_y = np.zeros((n_data, n_freq))
-    s_plot_z = np.zeros((n_data, n_freq))
-
-    planarity, ellipticity = [np.zeros((n_data_out, n_freq)) for _ in range(2)]
-    dop_3d = np.zeros((n_data_out, n_freq), dtype="complex128")
-    dop_2d = np.zeros((n_data_out, n_freq), dtype="complex128")
-
-    the_svd_fac = np.zeros((n_data_out, n_freq))
-    phi_svd_fac = np.zeros((n_data_out, n_freq))
-
-    # Get the correct frequencies for the wavelet transform
-    frequency_vec = w_0 / a_
-
-    censure = np.floor(2 * a_ * out_sampling / in_sampling * n_wave_period_to_average)
-
-    for ind_a, a_0 in enumerate(a_):
-        new_freq_mat = w_0 / a_0
-
-        # resample to 1 second sampling for Pc1-2 or 1 minute sampling for
-        # Pc3-5 average top frequencies to 1 second/1 minute below will be
-        # an average over 8 wave periods. first find where one sample is less
-        # than eight wave periods
-
-        if frequency_vec[ind_a] / n_wave_period_to_average > out_sampling:
-            av_window = 1 / out_sampling
-        else:
-            av_window = n_wave_period_to_average / frequency_vec[ind_a]
-
-        # Get the wavelet transform by backward FFT
-        w_exp_mat = np.exp(-sigma * sigma * ((a_0 * w_ - w_0) ** 2) / 2)
-        w_exp_mat2 = np.tile(w_exp_mat[:, np.newaxis], (1, 2))
-        w_exp_mat = np.tile(w_exp_mat[:, np.newaxis], (1, 3))
-
-        wb = fft.ifft(np.sqrt(1) * swb * w_exp_mat, axis=0, workers=os.cpu_count())
-        wb = np.array(wb)  # Make sure it's an array (scipy.fft.ifft returns Any type)
-        wb[idx_nan_b] = np.nan
-
-        we, w_eisr2 = [None, None]
-
-        if want_ee:
-            we = fft.ifft(np.sqrt(1) * sw_e * w_exp_mat, axis=0, workers=os.cpu_count())
-            we = np.array(we)
-            we[idx_nan_e] = np.nan
-
-            if flag_want_fac and not flag_de_dot_b0:
-                w_eisr2 = fft.ifft(
-                    np.sqrt(1) * sw_eisr2 * w_exp_mat2, axis=0, workers=os.cpu_count()
-                )
-                w_eisr2 = np.array(w_eisr2)
-                w_eisr2[idx_nan_eisr2] = np.nan
-
-                # Power spectrum of E, power = (2*pi)*conj(W).*W./new_freq_mat
-                power_2e_isr2_plot[:, ind_a] = np.sum(
-                    2 * np.pi * (w_eisr2 * np.conj(w_eisr2)) / new_freq_mat, axis=1
-                )
-            else:
-                # Power spectrum of E, power = (2*pi)*conj(W).*W./new_freq_mat
-                power_2e_isr2_plot[:, ind_a] = np.sum(
-                    2 * np.pi * (we * np.conj(we)) / new_freq_mat, axis=1
-                )
-
-            # Compute Ez from dE * B = 0
-            if flag_de_dot_b0:
-                we_re, we_im = [np.real(we), np.imag(we)]
-
-                we_z = (
-                    -(we_re[:, 0] * b_x + we_re[:, 1] * b_y) / b_z
-                    - 1j * (we_im[:, 0] * b_x + we_im[:, 1] * b_y) / b_z
-                )
-                we_z[idx_b_par_spin_plane] = np.nan
-
-                if flag_want_fac:
-                    if fac_matrix is None:
-                        arg_ = ts_vec_xyz(time_b0, np.hstack([we[:, :2], we_z]))
-                        we = convert_fac(arg_, b_bgd, xyz)
-                    else:
-                        arg_ = ts_vec_xyz(time_b0, np.hstack([we[:, :2], we_z]))
-                        we = convert_fac(arg_, fac_matrix)
-
-                    we = we[:, 1:]
-                else:
-                    we = np.hstack([we[:, :2], we_z])
-
-            power_e = 2 * np.pi * (we * np.conj(we)) / new_freq_mat
-            power_e = np.vstack([power_e.T, np.sum(power_e, axis=1)]).T
-
-            power_ex_plot[:, ind_a] = power_e[:, 0]
-            power_ey_plot[:, ind_a] = power_e[:, 1]
-            power_ez_plot[:, ind_a] = power_e[:, 2]
-            power_2e_plot[:, ind_a] = power_e[:, 3]
-
-            # Poynting flux calculations, assume E and b units mV/m and nT,
-            # get  S in uW/m^2 4pi from wavelets, see A. Tjulins power
-            # estimates
-            coeff_poynting = 10 / 4 / np.pi * (1 / 4) * (4 * np.pi)
-
-            s = np.zeros((n_data, 3))
-
-            we_x, we_y, we_z = [we[:, i] for i in range(3)]
-            wb_x, wb_y, wb_z = [wb[:, i] for i in range(3)]
-
-            s[:, 0] = (
-                coeff_poynting
-                * np.real(
-                    we_y * np.conj(wb_z)
-                    + np.conj(we_y) * wb_z
-                    - we_z * np.conj(wb_y)
-                    - np.conj(we_z) * wb_y
-                )
-                / new_freq_mat
-            )
-            s[:, 1] = (
-                coeff_poynting
-                * np.real(
-                    we_z * np.conj(wb_x)
-                    + np.conj(we_z) * wb_x
-                    - we_x * np.conj(wb_z)
-                    - np.conj(we_x) * wb_z
-                )
-                / new_freq_mat
-            )
-            s[:, 2] = (
-                coeff_poynting
-                * np.real(
-                    we_x * np.conj(wb_y)
-                    + np.conj(we_x) * wb_y
-                    - we_y * np.conj(wb_x)
-                    - np.conj(we_y) * wb_x
-                )
-                / new_freq_mat
-            )
-
-            s_plot_x[:, ind_a] = s[:, 0]
-            s_plot_y[:, ind_a] = s[:, 1]
-            s_plot_z[:, ind_a] = s[:, 2]
-
-        # Power spectrum of B
-        power_b = 2 * np.pi * (wb * np.conj(wb)) / new_freq_mat
-        power_b = np.vstack([power_b.T, np.sum(power_b, axis=1)]).T
-
-        power_bx_plot[:, ind_a] = power_b[:, 0]
-        power_by_plot[:, ind_a] = power_b[:, 1]
-        power_bz_plot[:, ind_a] = power_b[:, 2]
-        power_2b_plot[:, ind_a] = power_b[:, 3]
-
-        # Polarization parameters
-        if want_polarization:
-            # Construct spectral matrix and average it
-            s_mat = np.zeros((n_data, 3, 3), dtype="complex128")
-
-            for i in range(3):
-                for j in range(3):
-                    s_mat[:, i, j] = (
-                        2 * np.pi * (wb[:, i] * np.conj(wb[:, j])) / new_freq_mat
-                    )
-
-            # Averaged s_mat
-            s_mat_avg = np.zeros((n_data_out, 3, 3), dtype="complex128")
-
-            for comp in range(3):
-                s_mat_avg[..., comp] = _average_data(
-                    s_mat[..., comp], in_time, out_time, av_window
-                )
-
-            # Remove data possibly influenced by edge effects
-            censure_idx = np.hstack(
-                [
-                    np.arange(np.min([censure[ind_a], len(out_time)])),
-                    np.arange(
-                        np.max([0, len(out_time) - censure[ind_a] - 1]), len(out_time)
-                    ),
-                ]
-            ).astype(int)
-
-            s_mat_avg[censure_idx, ...] = np.nan
-
-            # compute singular value decomposition
-            # real matrix which is superposition of real part of spectral
-            # matrix over imaginary part
-            a_mat, u_mat = [np.zeros((6, 3, n_data_out)) for _ in range(2)]
-            w_mat, v_mat = [np.zeros((3, 3, n_data_out)) for _ in range(2)]
-
-            # wSingularValues = zeros(3,n_data2);
-            # R = zeros(3,3,n_data2); #spectral matrix in coordinate defined
-            # by V axes
-            a_mat[:3, ...] = np.real(np.transpose(s_mat_avg, [1, 2, 0]))
-            a_mat[3:6, ...] = -np.imag(np.transpose(s_mat_avg, [1, 2, 0]))
-
-            for i in range(n_data_out):
-                if np.sum(np.isnan(a_mat[..., i])) != 0:
-                    u_mat[..., i] = np.nan
-                    w_mat[..., i] = np.nan
-                    v_mat[..., i] = np.nan
-                else:
-                    uu_, ww_, vv_ = np.linalg.svd(a_mat[..., i], full_matrices=False)
-                    u_mat[..., i] = uu_
-                    w_mat[..., i] = ww_
-                    v_mat[..., i] = vv_
-
-            # compute direction of propagation
-            sign_kz = np.sign(v_mat[2, 2, :])
-            v_mat[2, 2, :] = v_mat[2, 2, :] * sign_kz
-            v_mat[1, 2, :] = v_mat[1, 2, :] * sign_kz
-            v_mat[0, 2, :] = v_mat[0, 2, :] * sign_kz
-
-            the_svd_fac[:, ind_a] = np.abs(
-                np.squeeze(
-                    np.arctan(
-                        np.sqrt(v_mat[0, 2, :] ** 2 + v_mat[1, 2, :] ** 2)
-                        / v_mat[2, 2, :]
-                    )
-                )
-            )
-            phi_svd_fac[:, ind_a] = np.squeeze(
-                np.arctan2(v_mat[1, 2, :], v_mat[0, 2, :])
-            )
-
-            # Calculate polarization parameters
-            planarity_local = np.squeeze(1 - np.sqrt(w_mat[2, 2, :] / w_mat[0, 0, :]))
-            planarity_local[censure_idx] = np.nan
-
-            planarity[:, ind_a] = planarity_local
-
-            # ellipticity: ratio of axes of polarization ellipse axes*sign of
-            # polarization
-
-            ellipticity_local = np.squeeze(w_mat[1, 1, :] / w_mat[0, 0, :]) * np.sign(
-                np.imag(s_mat_avg[:, 0, 1])
-            )
-            ellipticity_local[censure_idx] = np.nan
-
-            ellipticity[:, ind_a] = ellipticity_local
-
-            # DOP = sqrt[(3/2.*trace(SM^2)./(trace(SM))^2 - 1/2)]; Samson, 1973, JGR
-            dop = np.sqrt(
-                (3 / 2)
-                * (
-                    np.trace(np.matmul(s_mat_avg, s_mat_avg), axis1=1, axis2=2)
-                    / np.trace(s_mat_avg, axis1=1, axis2=2) ** 2
-                )
-                - 1 / 2
-            )
-
-            dop[censure_idx] = np.nan
-            dop_3d[:, ind_a] = dop
-
-            # DOP in 2D = sqrt[2*trace(rA^2)/trace(rA)^2 - 1)]; Ulrich
-            v_mat_new = np.transpose(v_mat, [2, 0, 1])
-
-            s_mat_avg2dim = np.matmul(
-                v_mat_new, np.matmul(s_mat_avg, np.transpose(v_mat_new, [0, 2, 1]))
-            )
-            s_mat_avg2dim = s_mat_avg2dim[:, :2, :2]
-            s_mat_avg = s_mat_avg2dim
-
-            dop2dim = np.sqrt(
-                2
-                * (
-                    np.trace(np.matmul(s_mat_avg, s_mat_avg), axis1=1, axis2=2)
-                    / np.trace(s_mat_avg, axis1=1, axis2=2) ** 2
-                )
-                - 1
-            )
-            dop2dim[censure_idx] = np.nan
-            dop_2d[:, ind_a] = dop
-
-    # set data gaps to NaN and remove edge effects
-    censure = np.floor(2 * a_)
-
-    for ind_a in range(len(a_)):
-        censure_idx = np.hstack(
-            [
-                np.arange(np.min([censure[ind_a], len(in_time)])),
-                np.arange(np.max([1, len(in_time) - censure[ind_a]]), len(in_time)),
-            ]
-        )
-
-        censure_idx = censure_idx.astype(int)
-
-        power_bx_plot[censure_idx, ind_a] = np.nan
-        power_by_plot[censure_idx, ind_a] = np.nan
-        power_bz_plot[censure_idx, ind_a] = np.nan
-        power_2b_plot[censure_idx, ind_a] = np.nan
-
-        if want_ee:
-            power_ex_plot[censure_idx, ind_a] = np.nan
-            power_ey_plot[censure_idx, ind_a] = np.nan
-            power_ez_plot[censure_idx, ind_a] = np.nan
-            power_2e_plot[censure_idx, ind_a] = np.nan
-
-            power_2e_isr2_plot[censure_idx, ind_a] = np.nan
-
-            s_plot_x[censure_idx, ind_a] = np.nan
-            s_plot_y[censure_idx, ind_a] = np.nan
-            s_plot_z[censure_idx, ind_a] = np.nan
-
-    # remove edge effects from data gaps
-    idx_nan_e = np.sum(idx_nan_e, axis=1) > 0
-    idx_nan_b = np.sum(idx_nan_b, axis=1) > 0
-    idx_nan_eisr2 = np.sum(idx_nan_eisr2, axis=1) > 0
-
-    n_power_b = len(power_2b_plot)
-
-    if pc12_range or other_range:
-        censure3 = np.floor(1.8 * a_)
-    elif pc35_range:
-        censure3 = np.floor(0.4 * a_)
-    else:
-        raise ValueError("Invalid range")
-
-    # Censure magnetic fied
-    power_bx_plot = _censure_plot(power_bx_plot, idx_nan_b, censure3, n_power_b, a_)
-    power_by_plot = _censure_plot(power_by_plot, idx_nan_b, censure3, n_power_b, a_)
-    power_bz_plot = _censure_plot(power_bz_plot, idx_nan_b, censure3, n_power_b, a_)
-    power_2b_plot = _censure_plot(power_2b_plot, idx_nan_b, censure3, n_power_b, a_)
-
-    # Censure electric field
-    n_power_e = len(power_2e_plot)
-    power_ex_plot = _censure_plot(power_ex_plot, idx_nan_e, censure3, n_power_e, a_)
-    power_ey_plot = _censure_plot(power_ey_plot, idx_nan_e, censure3, n_power_e, a_)
-    power_ez_plot = _censure_plot(power_ez_plot, idx_nan_e, censure3, n_power_e, a_)
-    power_2e_plot = _censure_plot(power_2e_plot, idx_nan_e, censure3, n_power_e, a_)
-
-    power_2e_isr2_plot = _censure_plot(
-        power_2e_isr2_plot, idx_nan_e, censure3, n_power_e, a_
-    )
-
-    # Censure poynting flux
-    s_plot_x = _censure_plot(s_plot_x, idx_nan_b, censure3, n_power_b, a_)
-    s_plot_x = _censure_plot(s_plot_x, idx_nan_e, censure3, n_power_e, a_)
-    s_plot_y = _censure_plot(s_plot_y, idx_nan_b, censure3, n_power_b, a_)
-    s_plot_y = _censure_plot(s_plot_y, idx_nan_e, censure3, n_power_e, a_)
-    s_plot_z = _censure_plot(s_plot_z, idx_nan_b, censure3, n_power_b, a_)
-    s_plot_z = _censure_plot(s_plot_z, idx_nan_e, censure3, n_power_e, a_)
-
-    n_power_2e_isr2 = len(power_2e_isr2_plot)
-    power_2e_isr2_plot = _censure_plot(
-        power_2e_isr2_plot, idx_nan_eisr2, censure3, n_power_2e_isr2, a_
-    )
-
-    power_bx_plot = _average_data(power_bx_plot, in_time, out_time)
-    power_by_plot = _average_data(power_by_plot, in_time, out_time)
-    power_bz_plot = _average_data(power_bz_plot, in_time, out_time)
-    power_2b_plot = _average_data(power_2b_plot, in_time, out_time)
-
-    bb_xxyyzzss = _bb_xxyyzzss(
-        power_bx_plot, power_by_plot, power_bz_plot, power_2b_plot
-    )
-
-    # Output
-    res["t"] = unix2datetime64(out_time)
-    res["f"] = frequency_vec[::-1]
-    res["bb_xxyyzzss"] = xr.DataArray(
-        bb_xxyyzzss[:, ::-1, ...],
-        coords=[res["t"], res["f"], ["xx", "yy", "zz", "ss"]],
-        dims=["time", "frequency", "comp"],
-    )
-
-    if want_ee:
-        power_ex_plot = _average_data(power_ex_plot, in_time, out_time)
-        power_ey_plot = _average_data(power_ey_plot, in_time, out_time)
-        power_ez_plot = _average_data(power_ez_plot, in_time, out_time)
-        power_2e_plot = _average_data(power_2e_plot, in_time, out_time)
-
-        power_2e_isr2_plot = _average_data(power_2e_isr2_plot, in_time, out_time)
-        power_2e_isr2_plot = np.real(power_2e_isr2_plot)
-
-        s_plot_x = np.real(_average_data(s_plot_x, in_time, out_time))
-        s_plot_y = np.real(_average_data(s_plot_y, in_time, out_time))
-        s_plot_z = np.real(_average_data(s_plot_z, in_time, out_time))
-
-        # TODO: check that it's correct (MATLAB weird stuff)
-        s_azimuth, s_elevation, s_r = cart2sph(s_plot_x, s_plot_y, s_plot_z)
-
-        ee_xxyyzzss = _ee_xxyyzzss(
-            power_ex_plot, power_ey_plot, power_ez_plot, power_2e_plot
-        )
-
-        poynting_xyz = np.tile(s_plot_x, (3, 1, 1))
-        poynting_xyz = np.transpose(poynting_xyz, [1, 2, 0])
-        poynting_xyz[:, :, 1] = s_plot_y
-        poynting_xyz[:, :, 2] = s_plot_z
-        poynting_xyz = poynting_xyz.astype(float)
-
-        poynting_r_th_ph = np.tile(s_r, (3, 1, 1))
-        poynting_r_th_ph = np.transpose(poynting_r_th_ph, [1, 2, 0])
-        poynting_r_th_ph[..., 1] = np.pi / 2 - s_elevation
-        poynting_r_th_ph[..., 2] = s_azimuth
-        poynting_r_th_ph[..., 1:] = poynting_r_th_ph[..., 1:] * 180 / np.pi
-        poynting_r_th_ph = poynting_r_th_ph.astype(float)
-
-        # Output
-        res["ee_ss"] = power_2e_isr2_plot.astype(float)
-
-        res["ee_xxyyzzss"] = xr.DataArray(
-            ee_xxyyzzss[:, ::-1, ...],
-            coords=[res["t"], res["f"], ["xx", "yy", "zz", "ss"]],
-            dims=["time", "frequency", "comp"],
-        )
-
-        res["pf_xyz"] = xr.DataArray(
-            poynting_xyz[:, ::-1, ...],
-            coords=[res["t"], res["f"], ["x", "y", "z"]],
-            dims=["time", "frequency", "comp"],
-        )
-
-        res["pf_rtp"] = xr.DataArray(
-            poynting_r_th_ph[:, ::-1, ...],
-            coords=[res["t"], res["f"], ["rho", "theta", "phi"]],
-            dims=["time", "frequency", "comp"],
-        )
-
-    if want_polarization:
-        # Define parameters for which we cannot compute the wave vector
-        with warnings.catch_warnings():
-            warnings.simplefilter(action="ignore", category=RuntimeWarning)
-            ind_low_planarity = planarity < 0.5
-            ind_low_ellipticity = np.abs(ellipticity) < 0.2
-
-        the_svd_fac[ind_low_planarity] = np.nan
-        phi_svd_fac[ind_low_planarity] = np.nan
-
-        the_svd_fac[ind_low_ellipticity] = np.nan
-        phi_svd_fac[ind_low_ellipticity] = np.nan
-
-        k_th_ph_svd_fac = np.zeros((the_svd_fac.shape[0], the_svd_fac.shape[1], 2))
-        k_th_ph_svd_fac[..., 0] = the_svd_fac
-        k_th_ph_svd_fac[..., 1] = phi_svd_fac
-
-        # Output
-        res["dop"] = xr.DataArray(
-            np.real(dop_3d[:, ::-1]),
-            coords=[res["t"], res["f"]],
-            dims=["time", "frequency"],
-        )
-
-        res["dop2d"] = xr.DataArray(
-            np.real(dop_2d[:, ::-1]),
-            coords=[res["t"], res["f"]],
-            dims=["time", "frequency"],
-        )
-
-        res["planarity"] = xr.DataArray(
-            planarity[:, ::-1], coords=[res["t"], res["f"]], dims=["time", "frequency"]
-        )
-
-        res["ellipticity"] = xr.DataArray(
-            ellipticity[:, ::-1],
-            coords=[res["t"], res["f"]],
-            dims=["time", "frequency"],
-        )
-
-        res["k_tp"] = xr.DataArray(
-            k_th_ph_svd_fac[:, ::-1, ...],
-            coords=[res["t"], res["f"], ["theta", "phi"]],
-            dims=["time", "frequency", "comp"],
-        )
-
-    return res
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# Built-in imports
+import logging
+import os
+import warnings
+
+# 3rd party imports
+import numba
+import numpy as np
+import xarray as xr
+from scipy import fft
+
+from .calc_fs import calc_fs
+from .cart2sph import cart2sph
+from .convert_fac import convert_fac
+from .datetime642iso8601 import datetime642iso8601
+from .iso2unix import iso2unix
+from .resample import resample
+
+# Local imports
+from .ts_time import ts_time
+from .ts_vec_xyz import ts_vec_xyz
+from .unix2datetime64 import unix2datetime64
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+logging.captureWarnings(True)
+logging.basicConfig(
+    format="[%(asctime)s] %(levelname)s: %(message)s",
+    datefmt="%d-%b-%y %H:%M:%S",
+    level=logging.INFO,
+)
+
+
+def _checksampling(e_xyz, db_xyz, b_xyz, b_bgd, flag_no_resamp):
+    assert e_xyz is not None
+
+    fs_e, fs_b = [calc_fs(e_xyz), calc_fs(db_xyz)]
+
+    resample_b_options = {"f_s": fs_b}
+
+    if flag_no_resamp:
+        assert fs_e == fs_b
+        fs_ = fs_e
+    else:
+        if fs_b > 1.5 * fs_e:
+            e_xyz = resample(e_xyz, db_xyz, **resample_b_options)
+            b_bgd = resample(b_bgd, db_xyz, **resample_b_options)
+
+            fs_ = fs_b
+            logging.info("Interpolating e to b")
+        elif fs_e > 1.5 * fs_b:
+            db_xyz = resample(db_xyz, e_xyz)
+            b_bgd = resample(b_bgd, e_xyz)
+
+            fs_ = fs_e
+            logging.info("Interpolating b to e")
+        elif fs_e == fs_b and len(e_xyz) == len(db_xyz):
+            fs_ = fs_e
+        else:
+            fs_ = 2 * fs_e
+            start_time = np.max(
+                [
+                    e_xyz.time.data[0].astype(int) / 1e9,
+                    db_xyz.time.data[0].astype(int) / 1e9,
+                ]
+            )
+            end_time = np.min(
+                [
+                    e_xyz.time.data[-1].astype(int) / 1e9,
+                    db_xyz.time.data[-1].astype(int) / 1e9,
+                ]
+            )
+
+            nt = int((end_time - start_time) * fs_)
+
+            t = np.linspace(start_time, end_time, nt)
+
+            t = ts_time(t)
+
+            e_xyz = resample(e_xyz, t)
+            b_bgd = resample(b_bgd, t)
+            b_xyz = resample(b_xyz, t)
+            db_xyz = resample(db_xyz, t)
+
+            logging.info("Interpolating b and e to 2x e sampling")
+
+    return e_xyz, db_xyz, b_xyz, b_bgd, fs_
+
+
+def _b_elevation(b_x, b_y, b_z, angle_b_elevation_max):
+    # Remove the last sample if the total number of samples is odd
+    b_x = b_x[: int(2 * (len(b_x) // 2)), :]
+    b_y = b_y[: int(2 * (len(b_y) // 2)), :]
+    b_z = b_z[: int(2 * (len(b_z) // 2)), :]
+
+    angle_b_elevation = np.arctan(b_z / np.sqrt(b_x**2 + b_y**2))
+    angle_b_elevation = np.rad2deg(angle_b_elevation)
+    idx_b_par_spin_plane = np.abs(angle_b_elevation) < angle_b_elevation_max
+
+    return angle_b_elevation, idx_b_par_spin_plane
+
+
+def _freq_int(freq_int, delta_b):
+    start_time = delta_b.time.data[0].astype(int) / 1e9
+    end_time = delta_b.time.data[-1].astype(int) / 1e9
+
+    pc12_range, pc35_range, other_range = [False, False, False]
+
+    if isinstance(freq_int, str):
+        if freq_int.lower() == "pc12":
+            pc12_range = True
+
+            freq_int = [0.1, 5]
+
+            delta_t = 1  # local
+
+            tint = np.round([start_time, end_time])
+            tint = list(datetime642iso8601(unix2datetime64(tint)))
+
+        elif freq_int.lower() == "pc35":
+            pc35_range = True
+
+            freq_int = [0.002, 0.1]
+
+            delta_t = 60  # local
+
+            tint = 60 * np.array([np.round(start_time / 60), np.round(end_time / 60)])
+            tint = datetime642iso8601(unix2datetime64(tint))
+
+        else:
+            raise ValueError("Invalid format of interval")
+
+        fs_out = 1 / delta_t
+
+        nt = np.round((iso2unix(tint[1]) - iso2unix(tint[0])) / delta_t)
+        nt = nt.astype(int)  # local
+
+        out_time = np.linspace(iso2unix(tint[0]), iso2unix(tint[1]), nt)
+        out_time += delta_t / 2
+        out_time = out_time[:-1]
+    else:
+        if freq_int[1] >= freq_int[0]:
+            other_range = True
+
+            fs_out = freq_int[1] / 5
+
+            delta_t = 1 / fs_out  # local
+
+            nt = np.round((end_time - start_time) / delta_t).astype(int)
+
+            out_time = np.linspace(start_time, end_time, nt)
+            out_time += delta_t / 2
+            out_time = out_time[:-1]
+        else:
+            raise ValueError("FREQ_INT must be [f_min f_max], f_min<f_max")
+
+    any_range = [pc12_range, pc35_range, other_range]
+
+    return any_range, freq_int, fs_out, out_time
+
+
+@numba.jit(cache=True, nogil=True, parallel=True, nopython=True, fastmath=True)
+def _average_data(data=None, x=None, y=None, av_window=None):
+    # average data with time x to time y using window
+
+    dtx, dty = [np.median(np.diff(x)), np.median(np.diff(y))]
+
+    if av_window is None:
+        av_window = dty
+
+    dt2 = av_window / 2
+
+    n_data_out = len(y)
+
+    # Pad data with NaNs from each side
+    n_point_to_add = int(np.ceil(dt2 / dtx))
+    pad_nan = np.ones((n_point_to_add, data.shape[1]), dtype="complex128") * np.nan
+    data_padded = np.vstack((pad_nan, data, pad_nan))
+
+    x_pad_pref = np.linspace(x[0] - dtx * (n_point_to_add - 1), x[0], n_point_to_add)
+    x_pad_suff = np.linspace(x[-1], x[-1] + dtx * (n_point_to_add - 1), n_point_to_add)
+    x_padded = np.hstack((x_pad_pref, x, x_pad_suff))
+
+    out = np.zeros((n_data_out, data.shape[1]), dtype="complex128")
+
+    il = np.digitize(y - dt2, x_padded)
+    ir = np.digitize(y + dt2, x_padded)
+
+    for i in numba.prange(len(y)):
+        for j in range(data.shape[1]):
+            out[i, j] = np.nanmean(data_padded[il[i] : ir[i], j])
+
+    return out
+
+
+def _bb_xxyyzzss(power_bx_plot, power_by_plot, power_bz_plot, power_2b_plot):
+    bb_xxyyzzss = np.tile(power_bx_plot[:, :, np.newaxis], (1, 1, 4))
+    bb_xxyyzzss[:, :, 1] = power_by_plot
+    bb_xxyyzzss[:, :, 2] = power_bz_plot
+    bb_xxyyzzss[:, :, 3] = power_2b_plot
+    return np.real(bb_xxyyzzss)
+
+
+def _ee_xxyyzzss(power_ex_plot, power_ey_plot, power_ez_plot, power_2e_plot):
+    ee_xxyyzzss = np.tile(power_ex_plot[..., np.newaxis], (1, 1, 4))
+    ee_xxyyzzss[:, :, 1] = power_ey_plot
+    ee_xxyyzzss[:, :, 2] = power_ez_plot
+    ee_xxyyzzss[:, :, 3] = power_2e_plot
+    return np.real(ee_xxyyzzss)
+
+
+@numba.jit(cache=True, nogil=True, parallel=True, nopython=True, fastmath=True)
+def _censure_plot(inp, idx_nan, censure, n_data, a_):
+    out = inp.copy()
+
+    for i in numba.prange(len(idx_nan) - 1):
+        for j in range(len(a_)):
+            if idx_nan[i] < idx_nan[i + 1]:
+                out[int(max([i - censure[j], 0])) : i, j] = np.nan
+
+            if idx_nan[i] > idx_nan[i + 1]:
+                out[i : int(min([i + censure[j], n_data])), j] = np.nan
+
+    return out
+
+
+def ebsp(e_xyz, db_xyz, b_xyz, b_bgd, xyz, freq_int, **kwargs):
+    """Calculates wavelet spectra of E&B and Poynting flux using wavelets
+    (Morlet wavelet). Also computes polarization parameters of B using SVD
+    [7]_. SVD is performed on spectral matrices computed from the time series
+    of B using wavelets and then averaged over a number of wave periods.
+
+    Parameters
+    ----------
+    e_xyz : xarray.DataArray
+        Time series of the wave electric field.
+    db_xyz : xarray.DataArray
+        Time series of the wave magnetic field.
+    b_xyz : xarray.DataArray
+        Time series of the high resolution background magnetic field used
+        for E.B=0.
+    b_bgd : xarray.DataArray
+        Time series of the background magnetic field used for field aligned
+        coordinates.
+    xyz : xarray.DataArray
+        Time series of the position time series of spacecraft used for field
+        aligned coordinates.
+    freq_int : str or array_like
+        Frequency interval :
+            * "pc12" : [0.1, 5.0]
+            * "pc35" : [2e-3, 0.1]
+            * [fmin, fmax] : arbitrary interval [fmin,fmax]
+
+    Returns
+    -------
+    res : xarray.Dataset
+        Dataset with :
+            * t : xarray.DataArray
+                Time.
+            * f : xarray.DataArray
+                Frequencies.
+            * bb_xxyyzzss : xarray.DataArray
+                delta_b power spectrum with :
+                    * [...,0] : x
+                    * [...,1] : y
+                    * [...,2] : z
+                    * [...,3] : sum
+            * ee_xxyyzzss : xarray.DataArray
+                E power spectrum with :
+                    * [...,0] : x
+                    * [...,1] : y
+                    * [...,2] : z
+                    * [...,3] : sum
+            * ee_ss : xarray.DataArray
+                E power spectrum (xx+yy spacecraft coordinates, e.g. ISR2).
+            * pf_xyz : xarray.DataArray
+                Poynting flux (xyz).
+            * pf_rtp : xarray.DataArray
+                Poynting flux (r, theta, phi) [angles in degrees].
+            * dop : xarray.DataArray
+                3D degree of polarization.
+            * dop2d : xarray.DataArray
+                2D degree of polarization in the polarization plane.
+            * planarity : xarray.DataArray
+                Planarity of polarization.
+            * ellipticity : xarray.DataArray
+                Ellipticity of polarization ellipse.
+            * k : xarray.DataArray
+                k-vector (theta, phi FAC) [angles in degrees].
+
+    Other Parameters
+    ----------------
+    polarization : bool
+        Computes polarization parameters. Default False.
+    noresamp : bool
+        No resampling, E and delta_b are given at the same time line.
+        Default False.
+    fac : bool
+        Uses FAC coordinate system (defined by b0 and optionally xyz),
+        otherwise no coordinate system transformation is performed. Default
+        False.
+    de_dot_b0 : bool
+        Computes dEz from delta_b dot B = 0, uses full_b. Default False.
+    full_b_db : bool
+        delta_b contains DC field. Default False.
+    nav : int
+        Number of wave periods to average Default 8.
+    fac_matrix : numpy.ndarray
+        Specify rotation matrix to FAC system Default None.
+    m_width_coeff : int or float
+        Specify coefficient to multiple Morlet wavelet width by. Default 1.
+
+    See also
+    --------
+    pyrfu.plot.pl_ebsp : to fill.
+    pyrfu.pyrf.convert_fac : Transforms to a field-aligned coordinate.
+
+    Notes
+    -----
+    This software was developed as part of the MAARBLE (Monitoring, Analyzing
+    and Assessing Radiation Belt Energization and Loss) collaborative
+    research project which has received funding from the European
+    Community's Seventh Framework Programme (FP7-SPACE-2011-1) under grant
+    agreement n. 284520.
+
+    References
+    ----------
+    .. [7] 	Santolík, O., Parrot. M., and  Lefeuvre. F. (2003) Singular value
+            decomposition methods for wave propagation analysis,Radio Sci.,
+            38(1), 1010, doi : https://doi.org/10.1029/2000RS002523 .
+
+    Examples
+    --------
+    >>> from pyrfu import mms, pyrf
+    >>> # Time interval
+    >>> tint_brst = ["2015-10-30T05:15:42.000", "2015-10-30T05:15:54.000"]
+    >>> # Spacecraft index
+    >>> mms_id = 3
+    >>> # Load spacecraft position
+    >>> tint_long = pyrf.extend_tint(tint_brst, [-100, 100])
+    >>> r_xyz = mms.get_data("R_gse", tint_long, mms_id)
+    >>> # Load background magnetic field, electric field and magnetic field
+    fluctuations
+    >>> b_xyz = mms.get_data("B_gse_fgm_brst_l2", tint_brst, mms_id)
+    >>> e_xyz = mms.get_data("E_gse_edp_brst_l2", tint_brst, mms_id)
+    >>> b_scm = mms.get_data("B_gse_scm_brst_l2", tint_brst, mms_id)
+    >>> # Polarization analysis
+    >>> options = dict(polarization=True, fac=True)
+    >>> polarization = pyrf.ebsp(e_xyz, b_scm, b_xyz, b_xyz, r_xyz,
+    >>>                          freq_int=[10, 4000], **options)
+
+    """
+
+    assert isinstance(db_xyz, xr.DataArray), "delta_b must be a DataArray"
+    assert isinstance(b_xyz, xr.DataArray), "full_b must be a DataArray"
+    assert isinstance(b_bgd, xr.DataArray), "b0 must be a DataArray"
+    assert isinstance(xyz, xr.DataArray), "xyz must be a DataArray"
+
+    # Compute magnetic field fluctuations sampling frequency
+    fs_b = calc_fs(db_xyz)
+
+    # Below which we cannot apply E*B=0
+    angle_b_elevation_max = 15.0
+
+    want_ee = e_xyz is not None
+
+    res = {
+        "t": None,
+        "f": None,
+        "flagFac": 0,
+        "bb_xxyyzzss": None,
+        "ee_xxyyzzss": None,
+        "ee_ss": None,
+        "pf_xyz": None,
+        "pf_rtp": None,
+        "dop": None,
+        "dop2d": None,
+        "planarity": None,
+        "ellipticity": None,
+        "k_tp": None,
+        "full_b": b_xyz,
+        "b0": b_bgd,
+        "r": xyz,
+    }
+
+    want_polarization = kwargs.get("polarization", False)
+
+    flag_no_resample = kwargs.get("no_resample", False)
+    flag_want_fac = kwargs.get("fac", False)
+    flag_de_dot_b0 = kwargs.get("de_dot_b0", False)
+    flag_full_b_db = kwargs.get("full_b_db", False)
+
+    m_width_coeff = kwargs.get("m_width_coeff", 1.0)
+
+    # Number of wave periods to average
+    n_wave_period_to_average = kwargs.get("nav", 8)
+
+    # matrix for rotation to FAC
+    fac_matrix = kwargs.get("fac_matrix", None)
+
+    if flag_want_fac and fac_matrix is None:
+        if b_bgd is None:
+            raise ValueError("ebsp(): at least b0 should be given for option FAC")
+
+        if xyz is None:
+            logging.info(
+                "convert_fac : assuming s/c position [1 0 0] for estimating FAC"
+            )
+            xyz = [1, 0, 0]
+            xyz = ts_vec_xyz(db_xyz.time.data, np.tile(xyz, (len(db_xyz), 1)))
+
+        xyz = resample(xyz, db_xyz, **{"f_s": fs_b})
+
+    b_bgd = resample(b_bgd, db_xyz, **{"f_s": fs_b})
+
+    if flag_full_b_db:
+        b_xyz = db_xyz
+        res["full_b"] = b_xyz
+        db_xyz = db_xyz - b_bgd
+
+    if flag_de_dot_b0 and b_xyz is None:
+        raise ValueError("full_b must be given for option de_dot_b0=0")
+
+    any_range, freq_int, out_sampling, out_time = _freq_int(freq_int, db_xyz)
+    pc12_range, pc35_range, other_range = any_range
+
+    if want_ee:
+        # Check the sampling rate
+        temp_ = _checksampling(e_xyz, db_xyz, b_xyz, b_bgd, flag_no_resample)
+        e_xyz, db_xyz, b_xyz, b_bgd, in_sampling = temp_
+
+    else:
+        in_sampling = calc_fs(db_xyz)
+
+        e_xyz = None
+
+    if in_sampling / 2 < freq_int[1]:
+        raise ValueError("F_MAX must be lower than the Nyquist frequency")
+
+    if want_ee and e_xyz.shape[1] < 3 and not flag_de_dot_b0:
+        raise ValueError(
+            "E must have all 3 components or flag de_dot_db=0 must be given"
+        )
+
+    if len(db_xyz) % 2:
+        db_xyz = db_xyz[:-1, :]
+        b_bgd = b_bgd[:-1, :]
+
+        if fac_matrix is None:
+            xyz = xyz[:-1, :]
+        else:
+            fac_matrix["t"] = fac_matrix["t"][:-1, :]
+
+            fac_matrix["rotMatrix"] = fac_matrix["rotMatrix"][:-1, :, :]
+
+        if want_ee:
+            e_xyz = e_xyz[:-1, :]
+
+    in_time = db_xyz.time.data.astype("int64") / 1e9
+
+    b_x, b_y, b_z = [None, None, None]
+
+    idx_b_par_spin_plane = None
+
+    if flag_de_dot_b0:
+        b_x, b_y, b_z = [b_xyz[:, i].data for i in range(3)]
+
+        # Remove the last sample if the total number of samples is odd
+        # temp_ = _b_elevation(b_x, b_y, b_z, angle_b_elevation_max)
+        # angle_b_elevation, idx_b_par_spin_plane = temp_
+        _, idx_b_par_spin_plane = _b_elevation(b_x, b_y, b_z, angle_b_elevation_max)
+
+    # If E has all three components, transform E and B waveforms to a magnetic
+    # field aligned coordinate (FAC) and save eisr for computation of e_sum.
+    # Otherwise we compute Ez within the main loop and do the transformation
+    # to FAC there.
+
+    time_b0 = 0
+    if flag_want_fac:
+        res["flagFac"] = True
+
+        time_b0 = b_bgd.time.data.astype("int64") / 1e9
+
+        if want_ee and not flag_de_dot_b0:
+            eisr2 = e_xyz[:, :2]
+            idx_nan_e = np.isnan(e_xyz.data)
+            idx_nan_eisr2 = np.isnan(eisr2.data)
+
+            if e_xyz.shape[1] < 3:
+                raise TypeError("E must be a 3D vector to be rotated to FAC")
+
+            if fac_matrix is None:
+                e_xyz = convert_fac(e_xyz, b_bgd, xyz)
+            else:
+                e_xyz = convert_fac(e_xyz, fac_matrix)
+
+        else:
+            idx_nan_e = None
+            eisr2 = None
+            idx_nan_eisr2 = None
+
+        if fac_matrix is None:
+            db_xyz = convert_fac(db_xyz, b_bgd, xyz)
+        else:
+            db_xyz = convert_fac(db_xyz, fac_matrix)
+    else:
+        idx_nan_e = None
+        eisr2 = None
+        idx_nan_eisr2 = None
+
+    # Find the frequencies for an FFT of all data and set important parameters
+    nd2 = len(in_time) / 2
+
+    freq = in_sampling * np.arange(nd2) / nd2 * 0.5
+
+    # The frequencies corresponding to FFT
+    w_ = np.hstack([0, freq, -np.flip(freq[:-1])])
+
+    morlet_width = 5.36 * m_width_coeff
+
+    # to get proper overlap for Morlet
+    freq_number = np.ceil(
+        (np.log10(freq_int[1]) - np.log10(freq_int[0])) * 12 * m_width_coeff
+    )
+
+    a_min, a_max = [
+        np.log10(0.5 * in_sampling / freq_int[1]),
+        np.log10(0.5 * in_sampling / freq_int[0]),
+    ]
+
+    a_number = freq_number
+    a_ = np.logspace(a_min, a_max, int(a_number))
+
+    # Maximum frequency
+    w_0 = in_sampling / 2
+
+    # Width of the Morlet wavelet
+    sigma = morlet_width / w_0
+
+    # Make the FFT of all data
+    idx_nan_b = np.isnan(db_xyz.data)
+
+    db_xyz.data[idx_nan_b] = 0
+
+    swb = fft.fft(db_xyz.data, axis=0, workers=os.cpu_count())
+
+    sw_e, sw_eisr2 = [None, None]
+
+    if want_ee:
+        logging.info("ebsp ... calculate E and B wavelet transform ... ")
+        e_xyz.data[idx_nan_e] = 0.0
+
+        sw_e = fft.fft(e_xyz.data, axis=0, workers=os.cpu_count())
+
+        if flag_want_fac and not flag_de_dot_b0:
+            eisr2.data[idx_nan_eisr2] = 0.0
+
+            sw_eisr2 = fft.fft(eisr2.data, axis=0, workers=os.cpu_count())
+    else:
+        logging.info("ebsp ... calculate B wavelet transform ....")
+
+    # Loop through all frequencies
+    n_data, n_freq, n_data_out = [len(in_time), len(a_), len(out_time)]
+
+    #
+    power_ex_plot = np.zeros((n_data, n_freq), dtype="complex128")
+    power_ey_plot = np.zeros((n_data, n_freq), dtype="complex128")
+    power_ez_plot = np.zeros((n_data, n_freq), dtype="complex128")
+    power_2e_plot = np.zeros((n_data, n_freq), dtype="complex128")
+    power_2e_isr2_plot = np.zeros((n_data, n_freq), dtype="complex128")
+
+    power_bx_plot = np.zeros((n_data, n_freq), dtype="complex128")
+    power_by_plot = np.zeros((n_data, n_freq), dtype="complex128")
+    power_bz_plot = np.zeros((n_data, n_freq), dtype="complex128")
+    power_2b_plot = np.zeros((n_data, n_freq), dtype="complex128")
+
+    s_plot_x = np.zeros((n_data, n_freq))
+    s_plot_y = np.zeros((n_data, n_freq))
+    s_plot_z = np.zeros((n_data, n_freq))
+
+    planarity, ellipticity = [np.zeros((n_data_out, n_freq)) for _ in range(2)]
+    dop_3d = np.zeros((n_data_out, n_freq), dtype="complex128")
+    dop_2d = np.zeros((n_data_out, n_freq), dtype="complex128")
+
+    the_svd_fac = np.zeros((n_data_out, n_freq))
+    phi_svd_fac = np.zeros((n_data_out, n_freq))
+
+    # Get the correct frequencies for the wavelet transform
+    frequency_vec = w_0 / a_
+
+    censure = np.floor(2 * a_ * out_sampling / in_sampling * n_wave_period_to_average)
+
+    for ind_a, a_0 in enumerate(a_):
+        new_freq_mat = w_0 / a_0
+
+        # resample to 1 second sampling for Pc1-2 or 1 minute sampling for
+        # Pc3-5 average top frequencies to 1 second/1 minute below will be
+        # an average over 8 wave periods. first find where one sample is less
+        # than eight wave periods
+
+        if frequency_vec[ind_a] / n_wave_period_to_average > out_sampling:
+            av_window = 1 / out_sampling
+        else:
+            av_window = n_wave_period_to_average / frequency_vec[ind_a]
+
+        # Get the wavelet transform by backward FFT
+        w_exp_mat = np.exp(-sigma * sigma * ((a_0 * w_ - w_0) ** 2) / 2)
+        w_exp_mat2 = np.tile(w_exp_mat[:, np.newaxis], (1, 2))
+        w_exp_mat = np.tile(w_exp_mat[:, np.newaxis], (1, 3))
+
+        wb = fft.ifft(np.sqrt(1) * swb * w_exp_mat, axis=0, workers=os.cpu_count())
+        wb = np.array(wb)  # Make sure it's an array (scipy.fft.ifft returns Any type)
+        wb[idx_nan_b] = np.nan
+
+        we, w_eisr2 = [None, None]
+
+        if want_ee:
+            we = fft.ifft(np.sqrt(1) * sw_e * w_exp_mat, axis=0, workers=os.cpu_count())
+            we = np.array(we)
+            we[idx_nan_e] = np.nan
+
+            if flag_want_fac and not flag_de_dot_b0:
+                w_eisr2 = fft.ifft(
+                    np.sqrt(1) * sw_eisr2 * w_exp_mat2, axis=0, workers=os.cpu_count()
+                )
+                w_eisr2 = np.array(w_eisr2)
+                w_eisr2[idx_nan_eisr2] = np.nan
+
+                # Power spectrum of E, power = (2*pi)*conj(W).*W./new_freq_mat
+                power_2e_isr2_plot[:, ind_a] = np.sum(
+                    2 * np.pi * (w_eisr2 * np.conj(w_eisr2)) / new_freq_mat, axis=1
+                )
+            else:
+                # Power spectrum of E, power = (2*pi)*conj(W).*W./new_freq_mat
+                power_2e_isr2_plot[:, ind_a] = np.sum(
+                    2 * np.pi * (we * np.conj(we)) / new_freq_mat, axis=1
+                )
+
+            # Compute Ez from dE * B = 0
+            if flag_de_dot_b0:
+                we_re, we_im = [np.real(we), np.imag(we)]
+
+                we_z = (
+                    -(we_re[:, 0] * b_x + we_re[:, 1] * b_y) / b_z
+                    - 1j * (we_im[:, 0] * b_x + we_im[:, 1] * b_y) / b_z
+                )
+                we_z[idx_b_par_spin_plane] = np.nan
+
+                if flag_want_fac:
+                    if fac_matrix is None:
+                        arg_ = ts_vec_xyz(time_b0, np.hstack([we[:, :2], we_z]))
+                        we = convert_fac(arg_, b_bgd, xyz)
+                    else:
+                        arg_ = ts_vec_xyz(time_b0, np.hstack([we[:, :2], we_z]))
+                        we = convert_fac(arg_, fac_matrix)
+
+                    we = we[:, 1:]
+                else:
+                    we = np.hstack([we[:, :2], we_z])
+
+            power_e = 2 * np.pi * (we * np.conj(we)) / new_freq_mat
+            power_e = np.vstack([power_e.T, np.sum(power_e, axis=1)]).T
+
+            power_ex_plot[:, ind_a] = power_e[:, 0]
+            power_ey_plot[:, ind_a] = power_e[:, 1]
+            power_ez_plot[:, ind_a] = power_e[:, 2]
+            power_2e_plot[:, ind_a] = power_e[:, 3]
+
+            # Poynting flux calculations, assume E and b units mV/m and nT,
+            # get  S in uW/m^2 4pi from wavelets, see A. Tjulins power
+            # estimates
+            coeff_poynting = 10 / 4 / np.pi * (1 / 4) * (4 * np.pi)
+
+            s = np.zeros((n_data, 3))
+
+            we_x, we_y, we_z = [we[:, i] for i in range(3)]
+            wb_x, wb_y, wb_z = [wb[:, i] for i in range(3)]
+
+            s[:, 0] = (
+                coeff_poynting
+                * np.real(
+                    we_y * np.conj(wb_z)
+                    + np.conj(we_y) * wb_z
+                    - we_z * np.conj(wb_y)
+                    - np.conj(we_z) * wb_y
+                )
+                / new_freq_mat
+            )
+            s[:, 1] = (
+                coeff_poynting
+                * np.real(
+                    we_z * np.conj(wb_x)
+                    + np.conj(we_z) * wb_x
+                    - we_x * np.conj(wb_z)
+                    - np.conj(we_x) * wb_z
+                )
+                / new_freq_mat
+            )
+            s[:, 2] = (
+                coeff_poynting
+                * np.real(
+                    we_x * np.conj(wb_y)
+                    + np.conj(we_x) * wb_y
+                    - we_y * np.conj(wb_x)
+                    - np.conj(we_y) * wb_x
+                )
+                / new_freq_mat
+            )
+
+            s_plot_x[:, ind_a] = s[:, 0]
+            s_plot_y[:, ind_a] = s[:, 1]
+            s_plot_z[:, ind_a] = s[:, 2]
+
+        # Power spectrum of B
+        power_b = 2 * np.pi * (wb * np.conj(wb)) / new_freq_mat
+        power_b = np.vstack([power_b.T, np.sum(power_b, axis=1)]).T
+
+        power_bx_plot[:, ind_a] = power_b[:, 0]
+        power_by_plot[:, ind_a] = power_b[:, 1]
+        power_bz_plot[:, ind_a] = power_b[:, 2]
+        power_2b_plot[:, ind_a] = power_b[:, 3]
+
+        # Polarization parameters
+        if want_polarization:
+            # Construct spectral matrix and average it
+            s_mat = np.zeros((n_data, 3, 3), dtype="complex128")
+
+            for i in range(3):
+                for j in range(3):
+                    s_mat[:, i, j] = (
+                        2 * np.pi * (wb[:, i] * np.conj(wb[:, j])) / new_freq_mat
+                    )
+
+            # Averaged s_mat
+            s_mat_avg = np.zeros((n_data_out, 3, 3), dtype="complex128")
+
+            for comp in range(3):
+                s_mat_avg[..., comp] = _average_data(
+                    s_mat[..., comp], in_time, out_time, av_window
+                )
+
+            # Remove data possibly influenced by edge effects
+            censure_idx = np.hstack(
+                [
+                    np.arange(np.min([censure[ind_a], len(out_time)])),
+                    np.arange(
+                        np.max([0, len(out_time) - censure[ind_a] - 1]), len(out_time)
+                    ),
+                ]
+            ).astype(int)
+
+            s_mat_avg[censure_idx, ...] = np.nan
+
+            # compute singular value decomposition
+            # real matrix which is superposition of real part of spectral
+            # matrix over imaginary part
+            a_mat, u_mat = [np.zeros((6, 3, n_data_out)) for _ in range(2)]
+            w_mat, v_mat = [np.zeros((3, 3, n_data_out)) for _ in range(2)]
+
+            # wSingularValues = zeros(3,n_data2);
+            # R = zeros(3,3,n_data2); #spectral matrix in coordinate defined
+            # by V axes
+            a_mat[:3, ...] = np.real(np.transpose(s_mat_avg, [1, 2, 0]))
+            a_mat[3:6, ...] = -np.imag(np.transpose(s_mat_avg, [1, 2, 0]))
+
+            for i in range(n_data_out):
+                if np.sum(np.isnan(a_mat[..., i])) != 0:
+                    u_mat[..., i] = np.nan
+                    w_mat[..., i] = np.nan
+                    v_mat[..., i] = np.nan
+                else:
+                    uu_, ww_, vv_ = np.linalg.svd(a_mat[..., i], full_matrices=False)
+                    u_mat[..., i] = uu_
+                    w_mat[..., i] = ww_
+                    v_mat[..., i] = vv_
+
+            # compute direction of propagation
+            sign_kz = np.sign(v_mat[2, 2, :])
+            v_mat[2, 2, :] = v_mat[2, 2, :] * sign_kz
+            v_mat[1, 2, :] = v_mat[1, 2, :] * sign_kz
+            v_mat[0, 2, :] = v_mat[0, 2, :] * sign_kz
+
+            the_svd_fac[:, ind_a] = np.abs(
+                np.squeeze(
+                    np.arctan(
+                        np.sqrt(v_mat[0, 2, :] ** 2 + v_mat[1, 2, :] ** 2)
+                        / v_mat[2, 2, :]
+                    )
+                )
+            )
+            phi_svd_fac[:, ind_a] = np.squeeze(
+                np.arctan2(v_mat[1, 2, :], v_mat[0, 2, :])
+            )
+
+            # Calculate polarization parameters
+            planarity_local = np.squeeze(1 - np.sqrt(w_mat[2, 2, :] / w_mat[0, 0, :]))
+            planarity_local[censure_idx] = np.nan
+
+            planarity[:, ind_a] = planarity_local
+
+            # ellipticity: ratio of axes of polarization ellipse axes*sign of
+            # polarization
+
+            ellipticity_local = np.squeeze(w_mat[1, 1, :] / w_mat[0, 0, :]) * np.sign(
+                np.imag(s_mat_avg[:, 0, 1])
+            )
+            ellipticity_local[censure_idx] = np.nan
+
+            ellipticity[:, ind_a] = ellipticity_local
+
+            # DOP = sqrt[(3/2.*trace(SM^2)./(trace(SM))^2 - 1/2)]; Samson, 1973, JGR
+            dop = np.sqrt(
+                (3 / 2)
+                * (
+                    np.trace(np.matmul(s_mat_avg, s_mat_avg), axis1=1, axis2=2)
+                    / np.trace(s_mat_avg, axis1=1, axis2=2) ** 2
+                )
+                - 1 / 2
+            )
+
+            dop[censure_idx] = np.nan
+            dop_3d[:, ind_a] = dop
+
+            # DOP in 2D = sqrt[2*trace(rA^2)/trace(rA)^2 - 1)]; Ulrich
+            v_mat_new = np.transpose(v_mat, [2, 0, 1])
+
+            s_mat_avg2dim = np.matmul(
+                v_mat_new, np.matmul(s_mat_avg, np.transpose(v_mat_new, [0, 2, 1]))
+            )
+            s_mat_avg2dim = s_mat_avg2dim[:, :2, :2]
+            s_mat_avg = s_mat_avg2dim
+
+            dop2dim = np.sqrt(
+                2
+                * (
+                    np.trace(np.matmul(s_mat_avg, s_mat_avg), axis1=1, axis2=2)
+                    / np.trace(s_mat_avg, axis1=1, axis2=2) ** 2
+                )
+                - 1
+            )
+            dop2dim[censure_idx] = np.nan
+            dop_2d[:, ind_a] = dop
+
+    # set data gaps to NaN and remove edge effects
+    censure = np.floor(2 * a_)
+
+    for ind_a in range(len(a_)):
+        censure_idx = np.hstack(
+            [
+                np.arange(np.min([censure[ind_a], len(in_time)])),
+                np.arange(np.max([1, len(in_time) - censure[ind_a]]), len(in_time)),
+            ]
+        )
+
+        censure_idx = censure_idx.astype(int)
+
+        power_bx_plot[censure_idx, ind_a] = np.nan
+        power_by_plot[censure_idx, ind_a] = np.nan
+        power_bz_plot[censure_idx, ind_a] = np.nan
+        power_2b_plot[censure_idx, ind_a] = np.nan
+
+        if want_ee:
+            power_ex_plot[censure_idx, ind_a] = np.nan
+            power_ey_plot[censure_idx, ind_a] = np.nan
+            power_ez_plot[censure_idx, ind_a] = np.nan
+            power_2e_plot[censure_idx, ind_a] = np.nan
+
+            power_2e_isr2_plot[censure_idx, ind_a] = np.nan
+
+            s_plot_x[censure_idx, ind_a] = np.nan
+            s_plot_y[censure_idx, ind_a] = np.nan
+            s_plot_z[censure_idx, ind_a] = np.nan
+
+    # remove edge effects from data gaps
+    idx_nan_e = np.sum(idx_nan_e, axis=1) > 0
+    idx_nan_b = np.sum(idx_nan_b, axis=1) > 0
+    idx_nan_eisr2 = np.sum(idx_nan_eisr2, axis=1) > 0
+
+    n_power_b = len(power_2b_plot)
+
+    if pc12_range or other_range:
+        censure3 = np.floor(1.8 * a_)
+    elif pc35_range:
+        censure3 = np.floor(0.4 * a_)
+    else:
+        raise ValueError("Invalid range")
+
+    # Censure magnetic fied
+    power_bx_plot = _censure_plot(power_bx_plot, idx_nan_b, censure3, n_power_b, a_)
+    power_by_plot = _censure_plot(power_by_plot, idx_nan_b, censure3, n_power_b, a_)
+    power_bz_plot = _censure_plot(power_bz_plot, idx_nan_b, censure3, n_power_b, a_)
+    power_2b_plot = _censure_plot(power_2b_plot, idx_nan_b, censure3, n_power_b, a_)
+
+    # Censure electric field
+    n_power_e = len(power_2e_plot)
+    power_ex_plot = _censure_plot(power_ex_plot, idx_nan_e, censure3, n_power_e, a_)
+    power_ey_plot = _censure_plot(power_ey_plot, idx_nan_e, censure3, n_power_e, a_)
+    power_ez_plot = _censure_plot(power_ez_plot, idx_nan_e, censure3, n_power_e, a_)
+    power_2e_plot = _censure_plot(power_2e_plot, idx_nan_e, censure3, n_power_e, a_)
+
+    power_2e_isr2_plot = _censure_plot(
+        power_2e_isr2_plot, idx_nan_e, censure3, n_power_e, a_
+    )
+
+    # Censure poynting flux
+    s_plot_x = _censure_plot(s_plot_x, idx_nan_b, censure3, n_power_b, a_)
+    s_plot_x = _censure_plot(s_plot_x, idx_nan_e, censure3, n_power_e, a_)
+    s_plot_y = _censure_plot(s_plot_y, idx_nan_b, censure3, n_power_b, a_)
+    s_plot_y = _censure_plot(s_plot_y, idx_nan_e, censure3, n_power_e, a_)
+    s_plot_z = _censure_plot(s_plot_z, idx_nan_b, censure3, n_power_b, a_)
+    s_plot_z = _censure_plot(s_plot_z, idx_nan_e, censure3, n_power_e, a_)
+
+    n_power_2e_isr2 = len(power_2e_isr2_plot)
+    power_2e_isr2_plot = _censure_plot(
+        power_2e_isr2_plot, idx_nan_eisr2, censure3, n_power_2e_isr2, a_
+    )
+
+    power_bx_plot = _average_data(power_bx_plot, in_time, out_time)
+    power_by_plot = _average_data(power_by_plot, in_time, out_time)
+    power_bz_plot = _average_data(power_bz_plot, in_time, out_time)
+    power_2b_plot = _average_data(power_2b_plot, in_time, out_time)
+
+    bb_xxyyzzss = _bb_xxyyzzss(
+        power_bx_plot, power_by_plot, power_bz_plot, power_2b_plot
+    )
+
+    # Output
+    res["t"] = unix2datetime64(out_time)
+    res["f"] = frequency_vec[::-1]
+    res["bb_xxyyzzss"] = xr.DataArray(
+        bb_xxyyzzss[:, ::-1, ...],
+        coords=[res["t"], res["f"], ["xx", "yy", "zz", "ss"]],
+        dims=["time", "frequency", "comp"],
+    )
+
+    if want_ee:
+        power_ex_plot = _average_data(power_ex_plot, in_time, out_time)
+        power_ey_plot = _average_data(power_ey_plot, in_time, out_time)
+        power_ez_plot = _average_data(power_ez_plot, in_time, out_time)
+        power_2e_plot = _average_data(power_2e_plot, in_time, out_time)
+
+        power_2e_isr2_plot = _average_data(power_2e_isr2_plot, in_time, out_time)
+        power_2e_isr2_plot = np.real(power_2e_isr2_plot)
+
+        s_plot_x = np.real(_average_data(s_plot_x, in_time, out_time))
+        s_plot_y = np.real(_average_data(s_plot_y, in_time, out_time))
+        s_plot_z = np.real(_average_data(s_plot_z, in_time, out_time))
+
+        # TODO: check that it's correct (MATLAB weird stuff)
+        s_azimuth, s_elevation, s_r = cart2sph(s_plot_x, s_plot_y, s_plot_z)
+
+        ee_xxyyzzss = _ee_xxyyzzss(
+            power_ex_plot, power_ey_plot, power_ez_plot, power_2e_plot
+        )
+
+        poynting_xyz = np.tile(s_plot_x, (3, 1, 1))
+        poynting_xyz = np.transpose(poynting_xyz, [1, 2, 0])
+        poynting_xyz[:, :, 1] = s_plot_y
+        poynting_xyz[:, :, 2] = s_plot_z
+        poynting_xyz = poynting_xyz.astype(float)
+
+        poynting_r_th_ph = np.tile(s_r, (3, 1, 1))
+        poynting_r_th_ph = np.transpose(poynting_r_th_ph, [1, 2, 0])
+        poynting_r_th_ph[..., 1] = np.pi / 2 - s_elevation
+        poynting_r_th_ph[..., 2] = s_azimuth
+        poynting_r_th_ph[..., 1:] = poynting_r_th_ph[..., 1:] * 180 / np.pi
+        poynting_r_th_ph = poynting_r_th_ph.astype(float)
+
+        # Output
+        res["ee_ss"] = power_2e_isr2_plot.astype(float)
+
+        res["ee_xxyyzzss"] = xr.DataArray(
+            ee_xxyyzzss[:, ::-1, ...],
+            coords=[res["t"], res["f"], ["xx", "yy", "zz", "ss"]],
+            dims=["time", "frequency", "comp"],
+        )
+
+        res["pf_xyz"] = xr.DataArray(
+            poynting_xyz[:, ::-1, ...],
+            coords=[res["t"], res["f"], ["x", "y", "z"]],
+            dims=["time", "frequency", "comp"],
+        )
+
+        res["pf_rtp"] = xr.DataArray(
+            poynting_r_th_ph[:, ::-1, ...],
+            coords=[res["t"], res["f"], ["rho", "theta", "phi"]],
+            dims=["time", "frequency", "comp"],
+        )
+
+    if want_polarization:
+        # Define parameters for which we cannot compute the wave vector
+        with warnings.catch_warnings():
+            warnings.simplefilter(action="ignore", category=RuntimeWarning)
+            ind_low_planarity = planarity < 0.5
+            ind_low_ellipticity = np.abs(ellipticity) < 0.2
+
+        the_svd_fac[ind_low_planarity] = np.nan
+        phi_svd_fac[ind_low_planarity] = np.nan
+
+        the_svd_fac[ind_low_ellipticity] = np.nan
+        phi_svd_fac[ind_low_ellipticity] = np.nan
+
+        k_th_ph_svd_fac = np.zeros((the_svd_fac.shape[0], the_svd_fac.shape[1], 2))
+        k_th_ph_svd_fac[..., 0] = the_svd_fac
+        k_th_ph_svd_fac[..., 1] = phi_svd_fac
+
+        # Output
+        res["dop"] = xr.DataArray(
+            np.real(dop_3d[:, ::-1]),
+            coords=[res["t"], res["f"]],
+            dims=["time", "frequency"],
+        )
+
+        res["dop2d"] = xr.DataArray(
+            np.real(dop_2d[:, ::-1]),
+            coords=[res["t"], res["f"]],
+            dims=["time", "frequency"],
+        )
+
+        res["planarity"] = xr.DataArray(
+            planarity[:, ::-1], coords=[res["t"], res["f"]], dims=["time", "frequency"]
+        )
+
+        res["ellipticity"] = xr.DataArray(
+            ellipticity[:, ::-1],
+            coords=[res["t"], res["f"]],
+            dims=["time", "frequency"],
+        )
+
+        res["k_tp"] = xr.DataArray(
+            k_th_ph_svd_fac[:, ::-1, ...],
+            coords=[res["t"], res["f"], ["theta", "phi"]],
+            dims=["time", "frequency", "comp"],
+        )
+
+    return res
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/edb.py` & `pyrfu-2.4.3/pyrfu/pyrf/edb.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 # Local imports
 from .resample import resample
 from .ts_scalar import ts_scalar
 from .ts_vec_xyz import ts_vec_xyz
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def _check_method(flag_method):
     default_value = 0
     if flag_method.lower() == "e_perp+nan":
         default_value = np.nan
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/end.py` & `pyrfu-2.4.3/pyrfu/pyrf/end.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# 3rd party import
-import numpy as np
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.7"
-__status__ = "Prototype"
-
-
-def end(inp):
-    """Gives the last time of the time series in unix format.
-
-    Parameters
-    ----------
-    inp : xarray.DataArray
-        Time series of the input variable.
-
-    Returns
-    -------
-    out : float
-        Value of the last time in unix format.
-
-    """
-
-    out = inp.time.data[-1].astype(np.int64) / 1e9
-
-    return out
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# 3rd party import
+import numpy as np
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def end(inp):
+    """Gives the last time of the time series in unix format.
+
+    Parameters
+    ----------
+    inp : xarray.DataArray
+        Time series of the input variable.
+
+    Returns
+    -------
+    out : float
+        Value of the last time in unix format.
+
+    """
+
+    out = inp.time.data[-1].astype(np.int64) / 1e9
+
+    return out
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/estimate.py` & `pyrfu-2.4.3/pyrfu/pyrf/estimate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# 3rd party imports
-import numpy as np
-from scipy import constants
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.7"
-__status__ = "Prototype"
-
-
-def _estimate_capa_disk(radius):
-    return 8 * constants.epsilon_0 * radius
-
-
-def _estimate_capa_sphe(radius):
-    return 4 * np.pi * constants.epsilon_0 * radius
-
-
-def _estimate_capa_wire(radius, length):
-    if not radius or radius == 0 or not length:
-        out = None
-    elif length and radius and length >= 10 * radius:
-        l_ = np.log(length / radius)
-        out = length / l_ * (1 + 1 / l_ * (1 - np.log(2)))
-        out *= 2 * np.pi * constants.epsilon_0
-    else:
-        raise ValueError(
-            "capacitance_wire requires length at least 10 times the radius!",
-        )
-    return out
-
-
-def _estimate_capa_cyli(a, h):
-    coef = 4 * np.pi**2 * a * constants.epsilon_0
-
-    if 0.5 < h / a < 4:
-        c_1 = h / (2.0 * a * (np.log(16 * h / a) ** 2 + np.pi**2 / 12))
-        out = coef * np.pi * c_1
-    elif h / a >= 4:
-        o_m = 2 * (np.log(4 * h / a) - 1)
-        c_1 = 2 * h / (np.pi * a) * (1.0 / o_m + (4 - np.pi**2) / o_m**3)
-        out = coef * c_1
-    else:
-        raise ValueError("length less than diameter, do not have formula yet")
-
-    return out
-
-
-def estimate(what_to_estimate: str, radius: float, length: float = None):
-    r"""Estimate values for some everyday stuff.
-
-    Parameters
-    ----------
-    what_to_estimate : str
-        Value to estimate:
-            * "capacitance_disk" estimates the capacitance of a disk
-            (requires radius of the disk).
-            * "capacitance_sphere" estimates of a sphere
-            (requires radius of the sphere).
-            * "capacitance_wire" estimates the capacitance of a wire
-            (requires radius and length of the wire).
-            * "capacitance_cylinder" estimates the capacitance of a cylinder
-            (requires radius and half length of the cylinder).
-    radius :  float
-        Radius of the disk, sphere, wire or cylinder
-    length : float, Optional
-        Length of the wire or half lenght of the cylinder.
-
-    Returns
-    -------
-    out : float
-        Estimated value.
-
-    Examples
-    --------
-    >>> from pyrfu import pyrf
-
-    Define radius of the sphere in SI units
-
-    >>> r_sphere = 20e-2
-
-    Computes the capacitance of the sphere
-
-    >>> c_sphere = pyrf.estimate("capacitance_sphere", r_sphere)
-
-
-    """
-    if what_to_estimate.lower() == "capacitance_disk":
-        out = _estimate_capa_disk(radius)
-    elif what_to_estimate.lower() == "capacitance_sphere":
-        out = _estimate_capa_sphe(radius)
-    elif what_to_estimate.lower() == "capacitance_wire":
-        out = _estimate_capa_wire(radius, length)
-    elif what_to_estimate.lower() == "capacitance_cylinder":
-        out = _estimate_capa_cyli(radius, length)
-    else:
-        raise NotImplementedError
-
-    return out
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# 3rd party imports
+import numpy as np
+from scipy import constants
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def _estimate_capa_disk(radius):
+    return 8 * constants.epsilon_0 * radius
+
+
+def _estimate_capa_sphe(radius):
+    return 4 * np.pi * constants.epsilon_0 * radius
+
+
+def _estimate_capa_wire(radius, length):
+    if not radius or radius == 0 or not length:
+        out = None
+    elif length and radius and length >= 10 * radius:
+        l_ = np.log(length / radius)
+        out = length / l_ * (1 + 1 / l_ * (1 - np.log(2)))
+        out *= 2 * np.pi * constants.epsilon_0
+    else:
+        raise ValueError(
+            "capacitance_wire requires length at least 10 times the radius!",
+        )
+    return out
+
+
+def _estimate_capa_cyli(a, h):
+    coef = 4 * np.pi**2 * a * constants.epsilon_0
+
+    if 0.5 < h / a < 4:
+        c_1 = h / (2.0 * a * (np.log(16 * h / a) ** 2 + np.pi**2 / 12))
+        out = coef * np.pi * c_1
+    elif h / a >= 4:
+        o_m = 2 * (np.log(4 * h / a) - 1)
+        c_1 = 2 * h / (np.pi * a) * (1.0 / o_m + (4 - np.pi**2) / o_m**3)
+        out = coef * c_1
+    else:
+        raise ValueError("length less than diameter, do not have formula yet")
+
+    return out
+
+
+def estimate(what_to_estimate: str, radius: float, length: float = None):
+    r"""Estimate values for some everyday stuff.
+
+    Parameters
+    ----------
+    what_to_estimate : str
+        Value to estimate:
+            * "capacitance_disk" estimates the capacitance of a disk
+            (requires radius of the disk).
+            * "capacitance_sphere" estimates of a sphere
+            (requires radius of the sphere).
+            * "capacitance_wire" estimates the capacitance of a wire
+            (requires radius and length of the wire).
+            * "capacitance_cylinder" estimates the capacitance of a cylinder
+            (requires radius and half length of the cylinder).
+    radius :  float
+        Radius of the disk, sphere, wire or cylinder
+    length : float, Optional
+        Length of the wire or half lenght of the cylinder.
+
+    Returns
+    -------
+    out : float
+        Estimated value.
+
+    Examples
+    --------
+    >>> from pyrfu import pyrf
+
+    Define radius of the sphere in SI units
+
+    >>> r_sphere = 20e-2
+
+    Computes the capacitance of the sphere
+
+    >>> c_sphere = pyrf.estimate("capacitance_sphere", r_sphere)
+
+
+    """
+    if what_to_estimate.lower() == "capacitance_disk":
+        out = _estimate_capa_disk(radius)
+    elif what_to_estimate.lower() == "capacitance_sphere":
+        out = _estimate_capa_sphe(radius)
+    elif what_to_estimate.lower() == "capacitance_wire":
+        out = _estimate_capa_wire(radius, length)
+    elif what_to_estimate.lower() == "capacitance_cylinder":
+        out = _estimate_capa_cyli(radius, length)
+    else:
+        raise NotImplementedError
+
+    return out
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/extend_tint.py` & `pyrfu-2.4.3/pyrfu/pyrf/extend_tint.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from .datetime642iso8601 import datetime642iso8601
 
 # Local imports
 from .iso86012datetime64 import iso86012datetime64
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def extend_tint(tint, ext: list = None):
     r"""Extends time interval.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/filt.py` & `pyrfu-2.4.3/pyrfu/pyrf/filt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# 3rd party imports
-import numpy as np
-import xarray as xr
-from scipy import signal
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.7"
-__status__ = "Prototype"
-
-
-# noinspection PyTupleAssignmentBalance
-def _ellip_coefficients(f_min, f_max, order):
-    num1, den1, num2, den2 = [None] * 4
-
-    if f_min == 0:
-        if order == -1:
-            order, f_max = signal.ellipord(
-                f_max,
-                np.min([f_max * 1.1, 0.9999]),
-                0.5,
-                60,
-            )
-
-        num1, den1 = signal.ellip(order, 0.5, 60, f_max, btype="lowpass")
-    elif f_max == 0:
-        if order == -1:
-            order, f_min = signal.ellipord(
-                f_min,
-                np.min([f_min * 1.1, 0.9999]),
-                0.5,
-                60,
-            )
-
-        num1, den1 = signal.ellip(order, 0.5, 60, f_min, btype="highpass")
-    else:
-        if order == -1:
-            order, f_max = signal.ellipord(
-                f_max,
-                np.min([f_max * 1.3, 0.9999]),
-                0.5,
-                60,
-            )
-
-        num1, den1 = signal.ellip(order, 0.5, 60, f_max)
-
-        if order == -1:
-            order, f_min = signal.ellipord(f_min, f_min * 0.75, 0.5, 60)
-
-        num2, den2 = signal.ellip(order, 0.5, 60, f_min)
-
-    return num1, den1, num2, den2
-
-
-def filt(inp, f_min: float = 0.0, f_max: float = 1.0, order: int = -1):
-    r"""Filters input quantity.
-
-    Parameters
-    ----------
-    inp : xarray.DataArray
-        Time series of the variable to filter.
-    f_min : float, Optional
-        Lower limit of the frequency range. Default is 0. (Highpass filter).
-    f_max : float, Optional
-        Upper limit of the frequency range. Default is 1. (Highpass filter).
-    order : int, Optional
-        Order of the elliptic filter. Default is -1.
-
-    Returns
-    -------
-    out : xarray.DataArray
-        Time series of the filtered signal.
-
-    Examples
-    --------
-    >>> from pyrfu import mms, pyrf
-
-    Time interval
-
-    >>> tint = ["2017-07-18T13:03:34.000", "2017-07-18T13:07:00.000"]
-
-    Spacecraft index
-
-    >>> mms_id = 1
-
-    Load magnetic and electric fields
-
-    >>> b_xyz = mms.get_data("B_gse_fgm_brst_l2", tint, mms_id)
-    >>> e_xyz = mms.get_data("E_gse_edp_brst_l2", tint, mms_id)
-
-    Convert E to field aligned coordinates
-
-    >>> e_xyzfac = pyrf.convert_fac(e_xyz, b_xyz, [1,0,0])
-
-    Bandpass filter E waveform
-
-    >>> e_xyzfac_hf = pyrf.filt(e_xyzfac, 4, 0, 3)
-    >>> e_xyzfac_lf = pyrf.filt(e_xyzfac, 0, 4, 3)
-
-    """
-
-    f_samp = 1 / (np.median(np.diff(inp.time)).astype(np.int64) * 1e-9)
-
-    # Data of the input
-    inp_data = inp.data
-
-    f_min, f_max = [f_min / (f_samp / 2), f_max / (f_samp / 2)]
-
-    f_max = np.min([f_max, 1.0])
-
-    # Parameters of the elliptic filter. fact defines the width between
-    # stopband and passband
-    # r_pass, r_stop, fact = [0.5, 60, 1.1]
-
-    num1, den1, num2, den2 = _ellip_coefficients(f_min, f_max, order)
-
-    if len(inp_data.shape) == 1:
-        inp_data = inp_data[:, np.newaxis]
-
-    out_data = np.zeros(inp_data.shape)
-
-    for i_col in range(inp_data.shape[1]):
-        out_data[:, i_col] = signal.filtfilt(num1, den1, inp_data[:, i_col])
-
-        if num2 is not None and den2 is not None:
-            out_data[:, i_col] = signal.filtfilt(
-                num2,
-                den2,
-                out_data[:, i_col],
-            )
-    if inp_data.shape[1] == 1:
-        out_data = out_data[:, 0]
-
-    out = xr.DataArray(
-        out_data,
-        coords=inp.coords,
-        dims=inp.dims,
-        attrs=inp.attrs,
-    )
-
-    return out
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# 3rd party imports
+import numpy as np
+import xarray as xr
+from scipy import signal
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+# noinspection PyTupleAssignmentBalance
+def _ellip_coefficients(f_min, f_max, order):
+    num1, den1, num2, den2 = [None] * 4
+
+    if f_min == 0:
+        if order == -1:
+            order, f_max = signal.ellipord(
+                f_max,
+                np.min([f_max * 1.1, 0.9999]),
+                0.5,
+                60,
+            )
+
+        num1, den1 = signal.ellip(order, 0.5, 60, f_max, btype="lowpass")
+    elif f_max == 0:
+        if order == -1:
+            order, f_min = signal.ellipord(
+                f_min,
+                np.min([f_min * 1.1, 0.9999]),
+                0.5,
+                60,
+            )
+
+        num1, den1 = signal.ellip(order, 0.5, 60, f_min, btype="highpass")
+    else:
+        if order == -1:
+            order, f_max = signal.ellipord(
+                f_max,
+                np.min([f_max * 1.3, 0.9999]),
+                0.5,
+                60,
+            )
+
+        num1, den1 = signal.ellip(order, 0.5, 60, f_max)
+
+        if order == -1:
+            order, f_min = signal.ellipord(f_min, f_min * 0.75, 0.5, 60)
+
+        num2, den2 = signal.ellip(order, 0.5, 60, f_min)
+
+    return num1, den1, num2, den2
+
+
+def filt(inp, f_min: float = 0.0, f_max: float = 1.0, order: int = -1):
+    r"""Filters input quantity.
+
+    Parameters
+    ----------
+    inp : xarray.DataArray
+        Time series of the variable to filter.
+    f_min : float, Optional
+        Lower limit of the frequency range. Default is 0. (Highpass filter).
+    f_max : float, Optional
+        Upper limit of the frequency range. Default is 1. (Highpass filter).
+    order : int, Optional
+        Order of the elliptic filter. Default is -1.
+
+    Returns
+    -------
+    out : xarray.DataArray
+        Time series of the filtered signal.
+
+    Examples
+    --------
+    >>> from pyrfu import mms, pyrf
+
+    Time interval
+
+    >>> tint = ["2017-07-18T13:03:34.000", "2017-07-18T13:07:00.000"]
+
+    Spacecraft index
+
+    >>> mms_id = 1
+
+    Load magnetic and electric fields
+
+    >>> b_xyz = mms.get_data("B_gse_fgm_brst_l2", tint, mms_id)
+    >>> e_xyz = mms.get_data("E_gse_edp_brst_l2", tint, mms_id)
+
+    Convert E to field aligned coordinates
+
+    >>> e_xyzfac = pyrf.convert_fac(e_xyz, b_xyz, [1,0,0])
+
+    Bandpass filter E waveform
+
+    >>> e_xyzfac_hf = pyrf.filt(e_xyzfac, 4, 0, 3)
+    >>> e_xyzfac_lf = pyrf.filt(e_xyzfac, 0, 4, 3)
+
+    """
+
+    f_samp = 1 / (np.median(np.diff(inp.time)).astype(np.int64) * 1e-9)
+
+    # Data of the input
+    inp_data = inp.data
+
+    f_min, f_max = [f_min / (f_samp / 2), f_max / (f_samp / 2)]
+
+    f_max = np.min([f_max, 1.0])
+
+    # Parameters of the elliptic filter. fact defines the width between
+    # stopband and passband
+    # r_pass, r_stop, fact = [0.5, 60, 1.1]
+
+    num1, den1, num2, den2 = _ellip_coefficients(f_min, f_max, order)
+
+    if len(inp_data.shape) == 1:
+        inp_data = inp_data[:, np.newaxis]
+
+    out_data = np.zeros(inp_data.shape)
+
+    for i_col in range(inp_data.shape[1]):
+        out_data[:, i_col] = signal.filtfilt(num1, den1, inp_data[:, i_col])
+
+        if num2 is not None and den2 is not None:
+            out_data[:, i_col] = signal.filtfilt(
+                num2,
+                den2,
+                out_data[:, i_col],
+            )
+    if inp_data.shape[1] == 1:
+        out_data = out_data[:, 0]
+
+    out = xr.DataArray(
+        out_data,
+        coords=inp.coords,
+        dims=inp.dims,
+        attrs=inp.attrs,
+    )
+
+    return out
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/find_closest.py` & `pyrfu-2.4.3/pyrfu/pyrf/find_closest.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # 3rd party imports
 import numpy as np
 from scipy import interpolate
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def find_closest(inp1, inp2):
     r"""Finds pairs that are closest to each other in two time series.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/get_omni_data.py` & `pyrfu-2.4.3/pyrfu/pyrf/get_omni_data.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,183 +1,183 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-import datetime
-
-# Built-in imports
-import urllib
-
-# 3rd party imports
-import numpy as np
-import pandas as pd
-
-# Local imports
-from .iso86012datetime64 import iso86012datetime64
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.7"
-__status__ = "Prototype"
-
-
-var_omni_1 = {
-    "b": 13,
-    "avgb": -1,
-    "blat": -1,
-    "blong": -1,
-    "bx": 14,
-    "bxgse": 14,
-    "bxgsm": 14,
-    "by": 15,
-    "bygse": 15,
-    "bz": 16,
-    "bzgse": 16,
-    "bygsm": 17,
-    "bzgsm": 18,
-    "t": 26,
-    "n": 25,
-    "nanp": -1,
-    "v": 21,
-    "vx": 22,
-    "vy": 23,
-    "vz": 24,
-    "vlon": -1,
-    "vlat": -1,
-    "p": 27,
-    "e": 28,
-    "beta": 29,
-    "ma": 30,
-    "bsnx": 34,
-    "bsny": 35,
-    "bsnz": 36,
-    "ms": 45,
-    "ssn": -1,
-    "dst": -1,
-    "ae": 37,
-    "al": 38,
-    "au": 39,
-    "kp": -1,
-    "pc": 44,
-    "f10.7": -1,
-    "imfid": 4,
-    "swid": 5,
-    "ts": 9,
-    "rmsts": 10,
-}
-
-var_omni_2 = {
-    "b": 8,
-    "avgb": 9,
-    "blat": 10,
-    "blong": 11,
-    "bx": 12,
-    "bxgse": 12,
-    "bxgsm": 12,
-    "by": 13,
-    "bygse": 13,
-    "bz": 14,
-    "bzgse": 14,
-    "bygsm": 15,
-    "bzgsm": 16,
-    "t": 22,
-    "n": 23,
-    "nanp": 27,
-    "v": 24,
-    "vx": -1,
-    "vy": -1,
-    "vz": -1,
-    "vlon": 25,
-    "vlat": 26,
-    "p": 28,
-    "e": 35,
-    "beta": 36,
-    "ma": 37,
-    "bsnx": -1,
-    "bsny": -1,
-    "bsnz": -1,
-    "ms": 56,
-    "ssn": 39,
-    "dst": 40,
-    "ae": 41,
-    "al": 52,
-    "au": 53,
-    "kp": 38,
-    "pc": 51,
-    "f10.7": 50,
-    "imfid": -1,
-    "swid": -1,
-    "ts": -1,
-    "rmsts": -1,
-}
-
-
-def _omni_url(tint, omni_database):
-    if omni_database == "omni_hour":
-        data_source = "omni2"
-        date_format = "%Y%m%d"
-        delta_t_min = 24 * 3600
-    elif omni_database == "omni_min":
-        data_source = "omni_min"
-        date_format = "%Y%m%d%H"
-        delta_t_min = 3600
-    else:
-        raise ValueError("Invalid database")
-
-    url_ = "omniweb.gsfc.nasa.gov/cgi/nx1.cgi?activity=retrieve&spacecraft="
-    url_ = f"https://{url_}{data_source}"
-
-    tint[0] += np.timedelta64(0, "[s]")
-    tint[1] += np.timedelta64(delta_t_min, "[s]")
-    tint = [t_.astype(datetime.datetime) for t_ in tint]
-    start_date, end_date = [t_.strftime(date_format) for t_ in tint]
-
-    url_ = f"{url_}&start_date={start_date}&end_date={end_date}"
-
-    return url_
-
-
-def get_omni_data(variables, tint, database: str = "omni_hour"):
-    r"""Downloads OMNI data.
-
-    Parameters
-    ----------
-    variables : list
-        Keys of the variables to download.
-    tint : list
-        Time interval.
-    database : {"omni_hour", "omni_min"}, Optional
-        OMNI data resolution. Default is database = "omni_hour".
-
-    Returns
-    -------
-    data : xarray.Dataset
-        OMNI data.
-
-    """
-
-    tint = iso86012datetime64(np.array(tint)).astype("<M8[s]")
-
-    url_ = _omni_url(tint, database)
-
-    vars_ = ""
-    for variable in variables:
-        vars_ = f"{vars_}&vars={var_omni_2[variable]:d}"
-
-    with urllib.request.urlopen(f"{url_}{vars_}") as file:
-        out = str(file.read())
-
-    idx_start, idx_end = [out.find("YEAR"), out.find("</pre>")]
-
-    lines = out[idx_start:idx_end].split("\\n")[:-1]
-    lines = [list(filter(lambda x: x != "", l_.split(" "))) for l_ in lines]
-    lines = [[f"{l_[0]}-{l_[1]}/{l_[2]}", *l_[3:]] for l_ in lines[1:]]
-    data = pd.DataFrame(lines, columns=["time", *variables])
-    data["time"] = pd.to_datetime(data["time"], format="%Y-%j/%H")
-
-    data = data.set_index("time").astype(np.float64)
-    fmt_ = f"<M8[{database[5].lower()}]"
-    data = data.loc[data.index.isin(tint.astype(fmt_).astype("<M8[ns]"))]
-    data = data.to_xarray()
-
-    return data
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+import datetime
+
+# Built-in imports
+import urllib
+
+# 3rd party imports
+import numpy as np
+import pandas as pd
+
+# Local imports
+from .iso86012datetime64 import iso86012datetime64
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+var_omni_1 = {
+    "b": 13,
+    "avgb": -1,
+    "blat": -1,
+    "blong": -1,
+    "bx": 14,
+    "bxgse": 14,
+    "bxgsm": 14,
+    "by": 15,
+    "bygse": 15,
+    "bz": 16,
+    "bzgse": 16,
+    "bygsm": 17,
+    "bzgsm": 18,
+    "t": 26,
+    "n": 25,
+    "nanp": -1,
+    "v": 21,
+    "vx": 22,
+    "vy": 23,
+    "vz": 24,
+    "vlon": -1,
+    "vlat": -1,
+    "p": 27,
+    "e": 28,
+    "beta": 29,
+    "ma": 30,
+    "bsnx": 34,
+    "bsny": 35,
+    "bsnz": 36,
+    "ms": 45,
+    "ssn": -1,
+    "dst": -1,
+    "ae": 37,
+    "al": 38,
+    "au": 39,
+    "kp": -1,
+    "pc": 44,
+    "f10.7": -1,
+    "imfid": 4,
+    "swid": 5,
+    "ts": 9,
+    "rmsts": 10,
+}
+
+var_omni_2 = {
+    "b": 8,
+    "avgb": 9,
+    "blat": 10,
+    "blong": 11,
+    "bx": 12,
+    "bxgse": 12,
+    "bxgsm": 12,
+    "by": 13,
+    "bygse": 13,
+    "bz": 14,
+    "bzgse": 14,
+    "bygsm": 15,
+    "bzgsm": 16,
+    "t": 22,
+    "n": 23,
+    "nanp": 27,
+    "v": 24,
+    "vx": -1,
+    "vy": -1,
+    "vz": -1,
+    "vlon": 25,
+    "vlat": 26,
+    "p": 28,
+    "e": 35,
+    "beta": 36,
+    "ma": 37,
+    "bsnx": -1,
+    "bsny": -1,
+    "bsnz": -1,
+    "ms": 56,
+    "ssn": 39,
+    "dst": 40,
+    "ae": 41,
+    "al": 52,
+    "au": 53,
+    "kp": 38,
+    "pc": 51,
+    "f10.7": 50,
+    "imfid": -1,
+    "swid": -1,
+    "ts": -1,
+    "rmsts": -1,
+}
+
+
+def _omni_url(tint, omni_database):
+    if omni_database == "omni_hour":
+        data_source = "omni2"
+        date_format = "%Y%m%d"
+        delta_t_min = 24 * 3600
+    elif omni_database == "omni_min":
+        data_source = "omni_min"
+        date_format = "%Y%m%d%H"
+        delta_t_min = 3600
+    else:
+        raise ValueError("Invalid database")
+
+    url_ = "omniweb.gsfc.nasa.gov/cgi/nx1.cgi?activity=retrieve&spacecraft="
+    url_ = f"https://{url_}{data_source}"
+
+    tint[0] += np.timedelta64(0, "[s]")
+    tint[1] += np.timedelta64(delta_t_min, "[s]")
+    tint = [t_.astype(datetime.datetime) for t_ in tint]
+    start_date, end_date = [t_.strftime(date_format) for t_ in tint]
+
+    url_ = f"{url_}&start_date={start_date}&end_date={end_date}"
+
+    return url_
+
+
+def get_omni_data(variables, tint, database: str = "omni_hour"):
+    r"""Downloads OMNI data.
+
+    Parameters
+    ----------
+    variables : list
+        Keys of the variables to download.
+    tint : list
+        Time interval.
+    database : {"omni_hour", "omni_min"}, Optional
+        OMNI data resolution. Default is database = "omni_hour".
+
+    Returns
+    -------
+    data : xarray.Dataset
+        OMNI data.
+
+    """
+
+    tint = iso86012datetime64(np.array(tint)).astype("<M8[s]")
+
+    url_ = _omni_url(tint, database)
+
+    vars_ = ""
+    for variable in variables:
+        vars_ = f"{vars_}&vars={var_omni_2[variable]:d}"
+
+    with urllib.request.urlopen(f"{url_}{vars_}") as file:
+        out = str(file.read())
+
+    idx_start, idx_end = [out.find("YEAR"), out.find("</pre>")]
+
+    lines = out[idx_start:idx_end].split("\\n")[:-1]
+    lines = [list(filter(lambda x: x != "", l_.split(" "))) for l_ in lines]
+    lines = [[f"{l_[0]}-{l_[1]}/{l_[2]}", *l_[3:]] for l_ in lines[1:]]
+    data = pd.DataFrame(lines, columns=["time", *variables])
+    data["time"] = pd.to_datetime(data["time"], format="%Y-%j/%H")
+
+    data = data.set_index("time").astype(np.float64)
+    fmt_ = f"<M8[{database[5].lower()}]"
+    data = data.loc[data.index.isin(tint.astype(fmt_).astype("<M8[ns]"))]
+    data = data.to_xarray()
+
+    return data
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/gradient.py` & `pyrfu-2.4.3/pyrfu/pyrf/gradient.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 import xarray as xr
 
 # Local imports
 from .calc_dt import calc_dt
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def gradient(inp):
     r"""Computes time derivative of the input variable.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/gse2gsm.py` & `pyrfu-2.4.3/pyrfu/pyrf/gse2gsm.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # Local imports
 from .cotrans import cotrans
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def gse2gsm(inp, flag: str = "gse>gsm"):
     r"""Converts GSE to GSM.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/histogram.py` & `pyrfu-2.4.3/pyrfu/pyrf/histogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.14"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def histogram(
     inp,
     bins: Union[str, int, np.ndarray, list] = 100,
     y_range: tuple = None,
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/histogram2d.py` & `pyrfu-2.4.3/pyrfu/pyrf/histogram2d.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 import xarray as xr
 
 # Local imports
 from .resample import resample
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.14"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def histogram2d(
     inp1,
     inp2,
     bins: Union[str, int, tuple] = 100,
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/increments.py` & `pyrfu-2.4.3/pyrfu/pyrf/increments.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 # 3rd party imports
 import numpy as np
 import xarray as xr
 from scipy.stats import kurtosis
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def increments(inp, scale: int = 10):
     r"""Returns the increments of a time series.
 
     .. math:: y = |x_i - x_{i+s}|
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/integrate.py` & `pyrfu-2.4.3/pyrfu/pyrf/integrate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# 3rd party imports
-import numpy as np
-import xarray as xr
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.7"
-__status__ = "Prototype"
-
-
-def integrate(inp, time_step: float = None):
-    r"""Integrate time series.
-
-    Parameters
-    ----------
-    inp : xarray.DataArray
-        Time series of the variable to integrate.
-
-    time_step : float, Optional
-        Time steps threshold. All time_steps larger than 3*time_step
-        are assumed data gaps, default is that time_step is the
-        smallest value of all time_steps of the time series.
-
-    Returns
-    -------
-    out : xarray.DataArray
-        Time series of the time integrated input.
-
-    Examples
-    --------
-    >>> from pyrfu import mms, pyrf
-
-    Time interval
-
-    >>> tint = ["2015-12-14T01:17:40.200", "2015-12-14T01:17:41.500"]
-
-    Spacecraft index
-
-    >>> mms_id = 1
-
-    Load magnetic field and electric field
-
-    >>> b_xyz = mms.get_data("B_gse_fgm_brst_l2", tint, mms_id)
-    >>> e_xyz = mms.get_data("E_gse_edp_brst_l2", tint, mms_id)
-
-    Convert electric field to field aligned coordinates
-
-    >>> e_xyzfac = pyrf.convert_fac(e_xyz, b_xyz, [1, 0, 0])
-
-    """
-
-    time_tmp = inp.time.data.astype(np.int64) * 1e-9
-    data_tmp = inp.data
-    unit_tmp = inp.attrs["UNITS"]
-
-    data = np.hstack([time_tmp, data_tmp])
-
-    delta_t = np.hstack([0, np.diff(data[:, 0])])
-
-    if time_step is None:
-        time_steps = np.diff(data[:, 0])
-
-        # remove the smallest time step in case some problems
-        time_step = np.min(np.delete(time_steps, np.argmin(time_steps)))
-
-    delta_t[delta_t > 3 * time_step] = 0
-
-    x_int = data
-    for j in range(1, x_int.shape[1]):
-        j_ok = ~np.isnan(x_int[:, j])
-
-        x_int[j_ok, j] = np.cumsum(data[j_ok, j] * delta_t[j_ok])
-
-    out = xr.DataArray(data[:, 1:], coords=inp.coords, dims=inp.dims)
-    out.attrs["UNITS"] = unit_tmp + "*s"
-
-    return out
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# 3rd party imports
+import numpy as np
+import xarray as xr
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def integrate(inp, time_step: float = None):
+    r"""Integrate time series.
+
+    Parameters
+    ----------
+    inp : xarray.DataArray
+        Time series of the variable to integrate.
+
+    time_step : float, Optional
+        Time steps threshold. All time_steps larger than 3*time_step
+        are assumed data gaps, default is that time_step is the
+        smallest value of all time_steps of the time series.
+
+    Returns
+    -------
+    out : xarray.DataArray
+        Time series of the time integrated input.
+
+    Examples
+    --------
+    >>> from pyrfu import mms, pyrf
+
+    Time interval
+
+    >>> tint = ["2015-12-14T01:17:40.200", "2015-12-14T01:17:41.500"]
+
+    Spacecraft index
+
+    >>> mms_id = 1
+
+    Load magnetic field and electric field
+
+    >>> b_xyz = mms.get_data("B_gse_fgm_brst_l2", tint, mms_id)
+    >>> e_xyz = mms.get_data("E_gse_edp_brst_l2", tint, mms_id)
+
+    Convert electric field to field aligned coordinates
+
+    >>> e_xyzfac = pyrf.convert_fac(e_xyz, b_xyz, [1, 0, 0])
+
+    """
+
+    time_tmp = inp.time.data.astype(np.int64) * 1e-9
+    data_tmp = inp.data
+    unit_tmp = inp.attrs["UNITS"]
+
+    data = np.hstack([time_tmp, data_tmp])
+
+    delta_t = np.hstack([0, np.diff(data[:, 0])])
+
+    if time_step is None:
+        time_steps = np.diff(data[:, 0])
+
+        # remove the smallest time step in case some problems
+        time_step = np.min(np.delete(time_steps, np.argmin(time_steps)))
+
+    delta_t[delta_t > 3 * time_step] = 0
+
+    x_int = data
+    for j in range(1, x_int.shape[1]):
+        j_ok = ~np.isnan(x_int[:, j])
+
+        x_int[j_ok, j] = np.cumsum(data[j_ok, j] * delta_t[j_ok])
+
+    out = xr.DataArray(data[:, 1:], coords=inp.coords, dims=inp.dims)
+    out.attrs["UNITS"] = unit_tmp + "*s"
+
+    return out
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/iplasma_calc.py` & `pyrfu-2.4.3/pyrfu/pyrf/iplasma_calc.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # 3rd party imports
 import numpy as np
 from scipy import constants
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def _print_header():
     print("=" * 70)
     print("IRFU plasma calculator, relativistic effects not fully included")
     print("velocities, gyroradia are relativistically correct")
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/iso2unix.py` & `pyrfu-2.4.3/pyrfu/pyrf/iso2unix.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def iso2unix(time):
     r"""Converts time in iso format to unix
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/iso86012datetime.py` & `pyrfu-2.4.3/pyrfu/pyrf/iso86012datetime.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import datetime
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def iso86012datetime(time):
     r"""Converts ISO 8601 time to datetime
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/iso86012datetime64.py` & `pyrfu-2.4.3/pyrfu/pyrf/iso86012datetime64.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def iso86012datetime64(time):
     r"""Convert ISO8601 time format to datetime64 in ns units.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/iso86012timevec.py` & `pyrfu-2.4.3/pyrfu/pyrf/iso86012timevec.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import re
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def iso86012timevec(time):
     r"""Convert ISO 8601 time string into time vector.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/l_shell.py` & `pyrfu-2.4.3/pyrfu/pyrf/l_shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import numpy as np
 
 # Local imports
 from .cotrans import cotrans
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def l_shell(r_xyz):
     r"""Compute spacecraft position L Shell for a dipole magnetic field
     according to IRGF.
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/lowpass.py` & `pyrfu-2.4.3/pyrfu/pyrf/lowpass.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # 3rd party imports
 import xarray as xr
 from scipy import signal
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def lowpass(inp, f_cut, fhz):
     r"""Filter the data through low or highpass filter with max
     frequency f_cut and subtract from the original.
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/magnetosphere.py` & `pyrfu-2.4.3/pyrfu/pyrf/magnetosphere.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import numpy as np
 
 # Local imports
 from .get_omni_data import get_omni_data
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def _rzero(d_p, b_z):
     return (10.22 + 1.29 * np.tanh(0.184 * (b_z + 8.14))) * d_p ** (-1 / 6.6)
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/match_phibe_dir.py` & `pyrfu-2.4.3/pyrfu/pyrf/match_phibe_dir.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 # Local imports
 from .resample import resample
 from .ts_scalar import ts_scalar
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def match_phibe_dir(b_xyz, e_xyz, angles: np.ndarray = None, f: float = None):
     r"""Get propagation direction by matching dBpar and "phi". Tries different
     propagation directions and finds the direction perpendicular to the
     magnetic field that gives the best correlation between the electrostatic
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/match_phibe_v.py` & `pyrfu-2.4.3/pyrfu/pyrf/match_phibe_v.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 # 3rd party imports
 import numpy as np
 from scipy import constants
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def match_phibe_v(b_0, b_z, int_e_dt, n, v):
     r"""Get propagation velocity by matching dBpar and phi. Used together with
     irf_match_phibe_dir.m.Finds best match in amplitude given, B0, dB_par,
     phi, propagation direction implied, for specified n and v given as
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/mean.py` & `pyrfu-2.4.3/pyrfu/pyrf/mean.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 # Local imports
 from .resample import resample
 from .ts_vec_xyz import ts_vec_xyz
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2022"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.13"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def mean(inp, r_xyz, b_xyz, dipole_axis):
     r"""Put inp into mean field coordinates defined by position vector r and
     magnetic field b if earth magnetic dipole axis z is given then  uses
     another algorithm (good for auroral passages)
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/mean_bins.py` & `pyrfu-2.4.3/pyrfu/pyrf/mean_bins.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def mean_bins(inp0, inp1, bins: int = 10):
     r"""Computes mean of values of y corresponding to bins of x.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/mean_field.py` & `pyrfu-2.4.3/pyrfu/pyrf/mean_field.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def mean_field(inp, deg):
     r"""Estimates mean field xm and wave field xw using polynomial fit of order
     `deg` for the number of columns larger than 3 assume that first column
     is time.
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/medfilt.py` & `pyrfu-2.4.3/pyrfu/pyrf/medfilt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-import numpy as np
-
-# 3rd party imports
-import xarray as xr
-from scipy import signal
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.7"
-__status__ = "Prototype"
-
-
-def medfilt(inp, n_pts: int = 11):
-    r"""Applies a median filter over npts points to inp.
-
-    Parameters
-    ----------
-    inp : xarray.DataArray
-        Time series of the input variable.
-    n_pts : int, Optional
-        Number of points of median filter.
-
-    Returns
-    -------
-    out : xarray.DataArray
-        Time series of the median filtered input variable.
-
-    Examples
-    --------
-    >>> import numpy
-    >>> from pyrfu import mms, pyrf
-
-    Time interval
-
-    >>> tint = ["2019-09-14T07:54:00.000", "2019-09-14T08:11:00.000"]
-
-    Spacecraft indices
-
-    >>> mms_list = numpy.arange(1,5)
-
-    Load magnetic field and electric field
-
-    >>> r_mms, b_mms = [[] * 4 for _ in range(2)]
-    >>> for mms_id in range(1, 5):
-    >>> 	r_mms.append(mms.get_data("R_gse", tint, mms_id))
-    >>> 	b_mms.append(mms.get_data("B_gse_fgm_srvy_l2", tint, mms_id))
-    >>>
-
-    Compute current density, etc
-
-    >>> j_xyz, _, b_xyz, _, _, _ = pyrf.c_4_j(r_mms, b_mms)
-
-    Get J sampling frequency
-
-    >>> fs = pyrf.calc_fs(j_xyz)
-
-    Median filter over 1s
-
-    >>> j_xyz = pyrf.medfilt(j_xyz,fs)
-
-    """
-
-    if isinstance(n_pts, float):
-        n_pts = np.floor(n_pts).astype(np.int64)
-
-    if n_pts % 2 == 0:
-        n_pts += 1
-
-    n_times = len(inp)
-
-    if inp.ndim == 3:
-        inp_data = np.reshape(inp.data, [n_times, 9])
-    else:
-        inp_data = inp.data
-
-    try:
-        n_comp = inp_data.shape[1]
-    except IndexError:
-        n_comp = 1
-
-        inp_data = inp_data[..., None]
-
-    out_data = np.zeros(inp_data.shape)
-
-    if not n_pts % 2:
-        n_pts += 1
-
-    for i in range(n_comp):
-        out_data[:, i] = signal.medfilt(inp_data[:, i], n_pts)
-
-    if n_comp == 9:
-        out_data = np.reshape(out_data, [n_times, 3, 3])
-
-    if out_data.shape[1] == 1:
-        out_data = out_data[:, 0]
-
-    out = xr.DataArray(out_data, coords=inp.coords, dims=inp.dims)
-    out.attrs = inp.attrs
-
-    return out
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+import numpy as np
+
+# 3rd party imports
+import xarray as xr
+from scipy import signal
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def medfilt(inp, n_pts: int = 11):
+    r"""Applies a median filter over npts points to inp.
+
+    Parameters
+    ----------
+    inp : xarray.DataArray
+        Time series of the input variable.
+    n_pts : int, Optional
+        Number of points of median filter.
+
+    Returns
+    -------
+    out : xarray.DataArray
+        Time series of the median filtered input variable.
+
+    Examples
+    --------
+    >>> import numpy
+    >>> from pyrfu import mms, pyrf
+
+    Time interval
+
+    >>> tint = ["2019-09-14T07:54:00.000", "2019-09-14T08:11:00.000"]
+
+    Spacecraft indices
+
+    >>> mms_list = numpy.arange(1,5)
+
+    Load magnetic field and electric field
+
+    >>> r_mms, b_mms = [[] * 4 for _ in range(2)]
+    >>> for mms_id in range(1, 5):
+    >>> 	r_mms.append(mms.get_data("R_gse", tint, mms_id))
+    >>> 	b_mms.append(mms.get_data("B_gse_fgm_srvy_l2", tint, mms_id))
+    >>>
+
+    Compute current density, etc
+
+    >>> j_xyz, _, b_xyz, _, _, _ = pyrf.c_4_j(r_mms, b_mms)
+
+    Get J sampling frequency
+
+    >>> fs = pyrf.calc_fs(j_xyz)
+
+    Median filter over 1s
+
+    >>> j_xyz = pyrf.medfilt(j_xyz,fs)
+
+    """
+
+    if isinstance(n_pts, float):
+        n_pts = np.floor(n_pts).astype(np.int64)
+
+    if n_pts % 2 == 0:
+        n_pts += 1
+
+    n_times = len(inp)
+
+    if inp.ndim == 3:
+        inp_data = np.reshape(inp.data, [n_times, 9])
+    else:
+        inp_data = inp.data
+
+    try:
+        n_comp = inp_data.shape[1]
+    except IndexError:
+        n_comp = 1
+
+        inp_data = inp_data[..., None]
+
+    out_data = np.zeros(inp_data.shape)
+
+    if not n_pts % 2:
+        n_pts += 1
+
+    for i in range(n_comp):
+        out_data[:, i] = signal.medfilt(inp_data[:, i], n_pts)
+
+    if n_comp == 9:
+        out_data = np.reshape(out_data, [n_times, 3, 3])
+
+    if out_data.shape[1] == 1:
+        out_data = out_data[:, 0]
+
+    out = xr.DataArray(out_data, coords=inp.coords, dims=inp.dims)
+    out.attrs = inp.attrs
+
+    return out
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/median_bins.py` & `pyrfu-2.4.3/pyrfu/pyrf/median_bins.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def median_bins(inp0, inp1, bins: int = 10):
     r"""Computes median of values of y corresponding to bins of x
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/mva.py` & `pyrfu-2.4.3/pyrfu/pyrf/mva.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,166 +1,166 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# 3rd party imports
-import numpy as np
-import xarray as xr
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.7"
-__status__ = "Prototype"
-
-
-def mva(inp, flag: str = "mvar"):
-    r"""Compute the minimum variance frame.
-
-    Parameters
-    ----------
-    inp : xarray.DataArray
-        Time series of the quantity to find minimum variance frame.
-    flag : {"mvar", "<bn>=0", "td"}, Optional
-        Constrain. Default is "mvar".
-
-    Returns
-    -------
-    out : xarray.DataArray
-        Time series of the input quantity in LMN coordinates.
-    l : numpy.ndarray
-        Eigenvalues l[0] > l[1] > l[2].
-    lmn : numpy.ndarray
-        Eigenvectors LMN coordinates.
-
-    See also
-    --------
-    pyrfu.pyrf.new_xyz
-
-    Examples
-    --------
-    >>> from pyrfu import mms, pyrf
-
-    Time interval
-
-    >>> tint = ["2019-09-14T07:54:00.000", "2019-09-14T08:11:00.000"]
-
-    Spacecraft index
-
-    >>> mms_id = 1
-
-    Load magnetic field
-
-    >>> b_xyz = mms.get_data("B_gse_fgm_srvy_l2", tint, mms_id)
-
-    Compute MVA frame
-
-    >>> b_lmn, lamb, frame = pyrf.mva(b_xyz)
-
-    """
-
-    inp_data = inp.data
-    n_t = inp_data.shape[0]
-
-    idx_1, idx_2 = [[0, 1, 2, 0, 0, 1], [0, 1, 2, 1, 2, 2]]
-
-    if flag in ["mvar", "<bn>=0"]:
-        m_mu_nu_m = np.mean(inp_data[:, idx_1] * inp_data[:, idx_2], 0)
-        m_mu_nu_m -= np.mean(inp_data, 0)[idx_1] * np.mean(inp_data, 0)[idx_2]
-
-    elif flag.lower() == "td":
-        m_mu_nu_m = np.mean(inp_data[:, idx_1] * inp_data[:, idx_2], 0)
-
-    else:
-        raise ValueError("invalid flag")
-
-    m_mu_nu = np.array(
-        [m_mu_nu_m[[0, 3, 4]], m_mu_nu_m[[3, 1, 5]], m_mu_nu_m[[4, 5, 2]]],
-    )
-
-    # Compute eigenvalues and eigenvectors
-    [lamb, lmn] = np.linalg.eig(m_mu_nu)
-
-    # Sort eigenvalues
-    lamb, lmn = [lamb[lamb.argsort()[::-1]], lmn[:, lamb.argsort()[::-1]]]
-
-    # ensure that the frame is right handed
-    lmn[:, 2] = np.cross(lmn[:, 0], lmn[:, 1])
-
-    if flag.lower() == "<bn>=0":
-        inp_mvar_mean = np.mean(
-            np.sum(
-                np.tile(inp_data, (3, 1, 1))
-                * np.transpose(np.tile(lmn, (n_t, 1, 1)), (2, 0, 1)),
-                1,
-            ),
-            1,
-        )
-
-        coeffs = np.zeros(3)
-        coeffs[0] = np.sum(inp_mvar_mean**2)
-
-        coeffs[1] = -(lamb[1] + lamb[2]) * inp_mvar_mean[0] ** 2
-        coeffs[1] -= (lamb[0] + lamb[2]) * inp_mvar_mean[1] ** 2
-        coeffs[1] -= (lamb[0] + lamb[1]) * inp_mvar_mean[2] ** 2
-
-        coeffs[2] = lamb[1] * lamb[2] * inp_mvar_mean[0] ** 2
-        coeffs[2] += lamb[0] * lamb[2] * inp_mvar_mean[1] ** 2
-        coeffs[2] += lamb[0] * lamb[1] * inp_mvar_mean[2] ** 2
-
-        roots = np.roots(coeffs)
-
-        l_min = np.min(roots)
-
-        n_vec = inp_mvar_mean / (lamb - l_min)
-        n_vec /= np.linalg.norm(n_vec, keepdims=True)
-        n_vec = np.matmul(lmn, n_vec)
-
-        b_vec = np.sum(inp_data * np.tile(n_vec, (n_t, 1)), axis=1)
-
-        inp_data_2 = inp_data.copy()
-        inp_data_2 -= np.tile(b_vec, (3, 1)).T * np.tile(n_vec, (n_t, 1))
-
-        inp_data_2_m = np.mean(inp_data_2, 0)
-
-        m_mu_nu_m = np.mean(inp_data_2[:, idx_1] * inp_data_2[:, idx_2], 0)
-        m_mu_nu_m -= inp_data_2_m[idx_1] * inp_data_2_m[idx_2]
-
-        m_mu_nu = np.array(
-            [m_mu_nu_m[[0, 3, 4]], m_mu_nu_m[[3, 1, 5]], m_mu_nu_m[[4, 5, 2]]],
-        )
-
-        lamb, lmn = np.linalg.eig(m_mu_nu)
-
-        lamb, lmn = [lamb[lamb.argsort()[::-1]], lmn[:, lamb.argsort()[::-1]]]
-
-        # Force the maximum variance direction to be positive
-        # lmn[:, 0] *= np.sign(lmn[np.argmax(lmn[:, 0]), 0])
-        # lamb[2], lmn[:, 2] = [l_min, np.cross(lmn[:, 0], lmn[:, 1])]
-
-    elif flag.lower() == "td":
-        l_min = lamb[2]
-        b_vec = np.sum(inp_data * np.tile(lmn[:, 2], (n_t, 1)), axis=1)
-
-        inp_data_2 = inp_data.copy()
-        inp_data_2 -= np.tile(b_vec, (3, 1)).T * np.tile(lmn[:, 2], (n_t, 1))
-
-        inp_data_2_m = np.mean(inp_data_2, 0)
-
-        m_mu_nu_m = np.mean(inp_data_2[:, idx_1] * inp_data_2[:, idx_2], 0)
-        m_mu_nu_m -= inp_data_2_m[idx_1] * inp_data_2_m[idx_2]
-
-        m_mu_nu = np.array(
-            [m_mu_nu_m[[0, 3, 4]], m_mu_nu_m[[3, 1, 5]], m_mu_nu_m[[4, 5, 2]]],
-        )
-
-        lamb, lmn = np.linalg.eig(m_mu_nu)
-
-        lamb, lmn = [lamb[lamb.argsort()[::-1]], lmn[:, lamb.argsort()[::-1]]]
-
-        lamb[2], lmn[:, 2] = [l_min, np.cross(lmn[:, 0], lmn[:, 1])]
-
-    out_data = (lmn.T @ inp_data.T).T
-
-    out = xr.DataArray(out_data, coords=inp.coords, dims=inp.dims)
-
-    return out, lamb, lmn
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# 3rd party imports
+import numpy as np
+import xarray as xr
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def mva(inp, flag: str = "mvar"):
+    r"""Compute the minimum variance frame.
+
+    Parameters
+    ----------
+    inp : xarray.DataArray
+        Time series of the quantity to find minimum variance frame.
+    flag : {"mvar", "<bn>=0", "td"}, Optional
+        Constrain. Default is "mvar".
+
+    Returns
+    -------
+    out : xarray.DataArray
+        Time series of the input quantity in LMN coordinates.
+    l : numpy.ndarray
+        Eigenvalues l[0] > l[1] > l[2].
+    lmn : numpy.ndarray
+        Eigenvectors LMN coordinates.
+
+    See also
+    --------
+    pyrfu.pyrf.new_xyz
+
+    Examples
+    --------
+    >>> from pyrfu import mms, pyrf
+
+    Time interval
+
+    >>> tint = ["2019-09-14T07:54:00.000", "2019-09-14T08:11:00.000"]
+
+    Spacecraft index
+
+    >>> mms_id = 1
+
+    Load magnetic field
+
+    >>> b_xyz = mms.get_data("B_gse_fgm_srvy_l2", tint, mms_id)
+
+    Compute MVA frame
+
+    >>> b_lmn, lamb, frame = pyrf.mva(b_xyz)
+
+    """
+
+    inp_data = inp.data
+    n_t = inp_data.shape[0]
+
+    idx_1, idx_2 = [[0, 1, 2, 0, 0, 1], [0, 1, 2, 1, 2, 2]]
+
+    if flag in ["mvar", "<bn>=0"]:
+        m_mu_nu_m = np.mean(inp_data[:, idx_1] * inp_data[:, idx_2], 0)
+        m_mu_nu_m -= np.mean(inp_data, 0)[idx_1] * np.mean(inp_data, 0)[idx_2]
+
+    elif flag.lower() == "td":
+        m_mu_nu_m = np.mean(inp_data[:, idx_1] * inp_data[:, idx_2], 0)
+
+    else:
+        raise ValueError("invalid flag")
+
+    m_mu_nu = np.array(
+        [m_mu_nu_m[[0, 3, 4]], m_mu_nu_m[[3, 1, 5]], m_mu_nu_m[[4, 5, 2]]],
+    )
+
+    # Compute eigenvalues and eigenvectors
+    [lamb, lmn] = np.linalg.eig(m_mu_nu)
+
+    # Sort eigenvalues
+    lamb, lmn = [lamb[lamb.argsort()[::-1]], lmn[:, lamb.argsort()[::-1]]]
+
+    # ensure that the frame is right handed
+    lmn[:, 2] = np.cross(lmn[:, 0], lmn[:, 1])
+
+    if flag.lower() == "<bn>=0":
+        inp_mvar_mean = np.mean(
+            np.sum(
+                np.tile(inp_data, (3, 1, 1))
+                * np.transpose(np.tile(lmn, (n_t, 1, 1)), (2, 0, 1)),
+                1,
+            ),
+            1,
+        )
+
+        coeffs = np.zeros(3)
+        coeffs[0] = np.sum(inp_mvar_mean**2)
+
+        coeffs[1] = -(lamb[1] + lamb[2]) * inp_mvar_mean[0] ** 2
+        coeffs[1] -= (lamb[0] + lamb[2]) * inp_mvar_mean[1] ** 2
+        coeffs[1] -= (lamb[0] + lamb[1]) * inp_mvar_mean[2] ** 2
+
+        coeffs[2] = lamb[1] * lamb[2] * inp_mvar_mean[0] ** 2
+        coeffs[2] += lamb[0] * lamb[2] * inp_mvar_mean[1] ** 2
+        coeffs[2] += lamb[0] * lamb[1] * inp_mvar_mean[2] ** 2
+
+        roots = np.roots(coeffs)
+
+        l_min = np.min(roots)
+
+        n_vec = inp_mvar_mean / (lamb - l_min)
+        n_vec /= np.linalg.norm(n_vec, keepdims=True)
+        n_vec = np.matmul(lmn, n_vec)
+
+        b_vec = np.sum(inp_data * np.tile(n_vec, (n_t, 1)), axis=1)
+
+        inp_data_2 = inp_data.copy()
+        inp_data_2 -= np.tile(b_vec, (3, 1)).T * np.tile(n_vec, (n_t, 1))
+
+        inp_data_2_m = np.mean(inp_data_2, 0)
+
+        m_mu_nu_m = np.mean(inp_data_2[:, idx_1] * inp_data_2[:, idx_2], 0)
+        m_mu_nu_m -= inp_data_2_m[idx_1] * inp_data_2_m[idx_2]
+
+        m_mu_nu = np.array(
+            [m_mu_nu_m[[0, 3, 4]], m_mu_nu_m[[3, 1, 5]], m_mu_nu_m[[4, 5, 2]]],
+        )
+
+        lamb, lmn = np.linalg.eig(m_mu_nu)
+
+        lamb, lmn = [lamb[lamb.argsort()[::-1]], lmn[:, lamb.argsort()[::-1]]]
+
+        # Force the maximum variance direction to be positive
+        # lmn[:, 0] *= np.sign(lmn[np.argmax(lmn[:, 0]), 0])
+        # lamb[2], lmn[:, 2] = [l_min, np.cross(lmn[:, 0], lmn[:, 1])]
+
+    elif flag.lower() == "td":
+        l_min = lamb[2]
+        b_vec = np.sum(inp_data * np.tile(lmn[:, 2], (n_t, 1)), axis=1)
+
+        inp_data_2 = inp_data.copy()
+        inp_data_2 -= np.tile(b_vec, (3, 1)).T * np.tile(lmn[:, 2], (n_t, 1))
+
+        inp_data_2_m = np.mean(inp_data_2, 0)
+
+        m_mu_nu_m = np.mean(inp_data_2[:, idx_1] * inp_data_2[:, idx_2], 0)
+        m_mu_nu_m -= inp_data_2_m[idx_1] * inp_data_2_m[idx_2]
+
+        m_mu_nu = np.array(
+            [m_mu_nu_m[[0, 3, 4]], m_mu_nu_m[[3, 1, 5]], m_mu_nu_m[[4, 5, 2]]],
+        )
+
+        lamb, lmn = np.linalg.eig(m_mu_nu)
+
+        lamb, lmn = [lamb[lamb.argsort()[::-1]], lmn[:, lamb.argsort()[::-1]]]
+
+        lamb[2], lmn[:, 2] = [l_min, np.cross(lmn[:, 0], lmn[:, 1])]
+
+    out_data = (lmn.T @ inp_data.T).T
+
+    out = xr.DataArray(out_data, coords=inp.coords, dims=inp.dims)
+
+    return out, lamb, lmn
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/new_xyz.py` & `pyrfu-2.4.3/pyrfu/pyrf/new_xyz.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def new_xyz(inp, trans_mat):
     r"""Transform the input field to the new frame.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/norm.py` & `pyrfu-2.4.3/pyrfu/pyrf/norm.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def norm(inp):
     r"""Computes the magnitude of the input field.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/normalize.py` & `pyrfu-2.4.3/pyrfu/pyrf/normalize.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def normalize(inp):
     r"""Normalizes the input field.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/optimize_nbins_1d.py` & `pyrfu-2.4.3/pyrfu/pyrf/optimize_nbins_1d.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def optimize_nbins_1d(x, n_min: int = 1, n_max: int = 100):
     r"""Estimates the number of bins for 1d histogram that minimizes the
     risk function in [1]_ , obtained by direct decomposition of the MISE
     following the method described in [2]_ .
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/optimize_nbins_2d.py` & `pyrfu-2.4.3/pyrfu/pyrf/optimize_nbins_2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import itertools
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def optimize_nbins_2d(x, y, n_min: list = None, n_max: list = None):
     r"""Estimates the number of bins for 2d histogram that minimizes
     the risk function in [1]_ , obtained by direct decomposition of the
     MISE following the method described in [2]_ .
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/pid_4sc.py` & `pyrfu-2.4.3/pyrfu/pyrf/pid_4sc.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# 3rd party imports
-import numpy as np
-import xarray as xr
-
-# Local imports
-from ..mms.rotate_tensor import rotate_tensor
-from .avg_4sc import avg_4sc
-from .c_4_grad import c_4_grad
-from .trace import trace
-from .ts_scalar import ts_scalar
-from .ts_tensor_xyz import ts_tensor_xyz
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2023"
-__license__ = "MIT"
-__version__ = "2.3.26"
-__status__ = "Prototype"
-
-
-def pid_4sc(r_mms, v_mms, p_mms, b_mms):
-    r"""Compute Pi-D term using definition of [1]_ as :
-
-    .. math::
-
-        Pi-D = - \Pi_{ij}D_{ij}
-
-    with :math:`\Pi_{ij}` the deviatoric part of the pressure
-    tensor :
-
-    .. math::
-
-        \Pi_{ij} = P_{ij} - p\delta_{ij}
-
-        p = \frac{1}{3}P_{ii}
-
-
-    and :math:`D_{ij}` the deviatoric part of the strain tensor :
-
-    .. math::
-
-        D_{ij} = \frac{1}{2}\left ( \partial_i u_j + \partial_j u_i \right )
-        - \frac{1}{3}\theta\delta_{ij}
-
-        \theta = \nabla . u
-
-
-    Parameters
-    ----------
-    r_mms : list of xarray.DataArray
-        Time series of the position of the 4 spacecraft.
-    v_mms : list of xarray.DataArray
-        Time series of the bulk velocities of the 4 spacecraft.
-    p_mms : list of xarray.DataArray
-        Time series of the pressure tensor of the 4 spacecraft.
-    b_mms : list of xarray.DataArray
-        Time series of the background magnetic field of the 4 spacecraft.
-
-    Returns
-    -------
-    pid : xarray.DataArray
-        Time series of the Pi-D.
-
-    References
-    ----------
-    .. [1]  Yang, Y., Matthaeus, W. H., Parashar, T. N., Wu, P., Wan, M.,
-            Shi, Y., et al. (2017). Energy transfer channels and turbulence
-            cascade in Vlasov-Maxwell turbulence. Physical Review E, 95,
-            061201. doi : https://doi.org/10.1103/PhysRevE.95.061201
-
-    """
-
-    # Compute pressure tensor and background magnetic field at the center of
-    # mass of the tetrahedron
-    p_xyz = avg_4sc(p_mms)
-    b_xyz = avg_4sc(b_mms)
-
-    # Compute divergence and gradient tensor of the bulk velocity. Yang's
-    # notation
-    theta = c_4_grad(r_mms, v_mms, "div")
-    grad_u = c_4_grad(r_mms, v_mms, "grad")
-
-    # Define identity tensor
-    identity_3d = np.zeros((len(grad_u), 3, 3))
-    np.einsum("jii->ji", identity_3d)[:] = 1
-
-    # strain tensor
-    eps_xyz = (grad_u.data + np.transpose(grad_u.data, [0, 2, 1])) / 2
-
-    # Deviatoric part of the strain tensor
-    d_xyz = eps_xyz - theta.data[:, np.newaxis, np.newaxis] * identity_3d / 2
-    d_xyz = ts_tensor_xyz(v_mms[0].time.data, d_xyz)
-
-    # Convert tensors to field aligned coordinates
-    d_fac = rotate_tensor(d_xyz, "fac", b_xyz, "pp")
-    p_fac = rotate_tensor(p_xyz, "fac", b_xyz, "pp")
-
-    # Isotropic scalar pressure
-    press = trace(p_fac) / 3
-
-    # Deviatoric part of the pressure tensor
-    pi_fac = p_fac.data - press.data[:, np.newaxis, np.newaxis] * identity_3d
-    pi_fac = ts_tensor_xyz(v_mms[0].time.data, pi_fac)
-
-    # Compute Pi-D
-    pid = np.sum(np.sum(pi_fac.data * d_fac.data, axis=1), axis=1)
-    pid = ts_scalar(v_mms[0].time.data, pid)
-
-    # Flatten tensors
-    d_flat = np.reshape(d_fac.data, [len(d_fac), 9])
-    pi_flat = np.reshape(pi_fac.data, [len(pi_fac), 9])
-    d_flat = d_flat[:, [0, 4, -1, 1, 2, 5]]
-    pi_flat = pi_flat[:, [0, 4, -1, 1, 2, 5]]
-
-    # Compute components of the double contraction sum
-    d_coeff = xr.DataArray(
-        d_flat * pi_flat,
-        coords=[p_xyz.time.data, np.arange(1, 7)],
-        dims=["time", "index"],
-    )
-
-    return pid, d_coeff
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# 3rd party imports
+import numpy as np
+import xarray as xr
+
+# Local imports
+from ..mms.rotate_tensor import rotate_tensor
+from .avg_4sc import avg_4sc
+from .c_4_grad import c_4_grad
+from .trace import trace
+from .ts_scalar import ts_scalar
+from .ts_tensor_xyz import ts_tensor_xyz
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def pid_4sc(r_mms, v_mms, p_mms, b_mms):
+    r"""Compute Pi-D term using definition of [1]_ as :
+
+    .. math::
+
+        Pi-D = - \Pi_{ij}D_{ij}
+
+    with :math:`\Pi_{ij}` the deviatoric part of the pressure
+    tensor :
+
+    .. math::
+
+        \Pi_{ij} = P_{ij} - p\delta_{ij}
+
+        p = \frac{1}{3}P_{ii}
+
+
+    and :math:`D_{ij}` the deviatoric part of the strain tensor :
+
+    .. math::
+
+        D_{ij} = \frac{1}{2}\left ( \partial_i u_j + \partial_j u_i \right )
+        - \frac{1}{3}\theta\delta_{ij}
+
+        \theta = \nabla . u
+
+
+    Parameters
+    ----------
+    r_mms : list of xarray.DataArray
+        Time series of the position of the 4 spacecraft.
+    v_mms : list of xarray.DataArray
+        Time series of the bulk velocities of the 4 spacecraft.
+    p_mms : list of xarray.DataArray
+        Time series of the pressure tensor of the 4 spacecraft.
+    b_mms : list of xarray.DataArray
+        Time series of the background magnetic field of the 4 spacecraft.
+
+    Returns
+    -------
+    pid : xarray.DataArray
+        Time series of the Pi-D.
+
+    References
+    ----------
+    .. [1]  Yang, Y., Matthaeus, W. H., Parashar, T. N., Wu, P., Wan, M.,
+            Shi, Y., et al. (2017). Energy transfer channels and turbulence
+            cascade in Vlasov-Maxwell turbulence. Physical Review E, 95,
+            061201. doi : https://doi.org/10.1103/PhysRevE.95.061201
+
+    """
+
+    # Compute pressure tensor and background magnetic field at the center of
+    # mass of the tetrahedron
+    p_xyz = avg_4sc(p_mms)
+    b_xyz = avg_4sc(b_mms)
+
+    # Compute divergence and gradient tensor of the bulk velocity. Yang's
+    # notation
+    theta = c_4_grad(r_mms, v_mms, "div")
+    grad_u = c_4_grad(r_mms, v_mms, "grad")
+
+    # Define identity tensor
+    identity_3d = np.zeros((len(grad_u), 3, 3))
+    np.einsum("jii->ji", identity_3d)[:] = 1
+
+    # strain tensor
+    eps_xyz = (grad_u.data + np.transpose(grad_u.data, [0, 2, 1])) / 2
+
+    # Deviatoric part of the strain tensor
+    d_xyz = eps_xyz - theta.data[:, np.newaxis, np.newaxis] * identity_3d / 2
+    d_xyz = ts_tensor_xyz(v_mms[0].time.data, d_xyz)
+
+    # Convert tensors to field aligned coordinates
+    d_fac = rotate_tensor(d_xyz, "fac", b_xyz, "pp")
+    p_fac = rotate_tensor(p_xyz, "fac", b_xyz, "pp")
+
+    # Isotropic scalar pressure
+    press = trace(p_fac) / 3
+
+    # Deviatoric part of the pressure tensor
+    pi_fac = p_fac.data - press.data[:, np.newaxis, np.newaxis] * identity_3d
+    pi_fac = ts_tensor_xyz(v_mms[0].time.data, pi_fac)
+
+    # Compute Pi-D
+    pid = np.sum(np.sum(pi_fac.data * d_fac.data, axis=1), axis=1)
+    pid = ts_scalar(v_mms[0].time.data, pid)
+
+    # Flatten tensors
+    d_flat = np.reshape(d_fac.data, [len(d_fac), 9])
+    pi_flat = np.reshape(pi_fac.data, [len(pi_fac), 9])
+    d_flat = d_flat[:, [0, 4, -1, 1, 2, 5]]
+    pi_flat = pi_flat[:, [0, 4, -1, 1, 2, 5]]
+
+    # Compute components of the double contraction sum
+    d_coeff = xr.DataArray(
+        d_flat * pi_flat,
+        coords=[p_xyz.time.data, np.arange(1, 7)],
+        dims=["time", "index"],
+    )
+
+    return pid, d_coeff
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/plasma_beta.py` & `pyrfu-2.4.3/pyrfu/pyrf/plasma_beta.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from ..mms import rotate_tensor
 from .norm import norm
 from .resample import resample
 from .ts_scalar import ts_scalar
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def plasma_beta(b_xyz, p_xyz):
     """Computes plasma beta at magnetic field sampling
 
     .. math::
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/plasma_calc.py` & `pyrfu-2.4.3/pyrfu/pyrf/plasma_calc.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from scipy import constants
 
 # Local imports
 from .resample import resample
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def plasma_calc(b_xyz, t_i, t_e, n_i, n_e):
     """Computes plasma parameters including characteristic length and time
     scales.
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/poynting_flux.py` & `pyrfu-2.4.3/pyrfu/pyrf/poynting_flux.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from .dot import dot
 from .normalize import normalize
 from .resample import resample
 from .time_clip import time_clip
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def poynting_flux(e_xyz, b_xyz, b_hat):
     r"""Estimates Poynting flux at electric field sampling as
 
     .. math::
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/pres_anis.py` & `pyrfu-2.4.3/pyrfu/pyrf/pres_anis.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from scipy import constants
 
 # Local imports
 from .resample import resample
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def pres_anis(p_fac, b_xyz):
     r"""Compute pressure anisotropy factor:
 
     .. math::
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/pvi.py` & `pyrfu-2.4.3/pyrfu/pyrf/pvi.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def pvi(inp, scale: int = 10):
     r"""Returns the PVI of a time series.
 
     .. math::
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/pvi_4sc.py` & `pyrfu-2.4.3/pyrfu/pyrf/pvi_4sc.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from .norm import norm
 
 # Local imports
 from .resample import resample
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def pvi_4sc(b_mms):
     r"""Compute the Partial Variance of Increments (PVI) using the
     definition in [1]_ as
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/read_cdf.py` & `pyrfu-2.4.3/pyrfu/pyrf/read_cdf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# 3rd party imports
-import numpy as np
-import xarray as xr
-from cdflib import cdfepoch, cdfread
-from dateutil import parser
-
-# Local imports
-from .datetime2iso8601 import datetime2iso8601
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2023"
-__license__ = "MIT"
-__version__ = "2.3.26"
-__status__ = "Prototype"
-
-
-def read_cdf(path, tint):
-    r"""Reads CDF files.
-
-    Parameters
-    ----------
-    path : str
-        String of the filename in .cdf containing the L2 data
-    tint : list
-        Time interval
-
-    Returns
-    -------
-    out_dict : dict
-        Hash table with fields contained in the .cdf file.
-
-    """
-
-    tint = list(map(parser.parse, tint))
-    tint = list(map(datetime2iso8601, tint))
-    tint = list(map(cdfepoch.parse, tint))
-
-    out_dict = {}
-
-    with cdfread.CDF(path) as file:
-        keys_ = file.cdf_info()["zVariables"]
-        for k_ in keys_:
-            temp_ = file.varget(k_, starttime=tint[0], endtime=tint[1])
-            shape_ = temp_.shape
-            coords = [np.arange(lim_) for lim_ in shape_]
-
-            out_dict[k_.lower()] = xr.DataArray(temp_, coords=coords)
-
-    return out_dict
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# 3rd party imports
+import numpy as np
+import xarray as xr
+from cdflib import cdfepoch, cdfread
+from dateutil import parser
+
+# Local imports
+from .datetime2iso8601 import datetime2iso8601
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def read_cdf(path, tint):
+    r"""Reads CDF files.
+
+    Parameters
+    ----------
+    path : str
+        String of the filename in .cdf containing the L2 data
+    tint : list
+        Time interval
+
+    Returns
+    -------
+    out_dict : dict
+        Hash table with fields contained in the .cdf file.
+
+    """
+
+    tint = list(map(parser.parse, tint))
+    tint = list(map(datetime2iso8601, tint))
+    tint = list(map(cdfepoch.parse, tint))
+
+    out_dict = {}
+
+    with cdfread.CDF(path) as file:
+        keys_ = file.cdf_info()["zVariables"]
+        for k_ in keys_:
+            temp_ = file.varget(k_, starttime=tint[0], endtime=tint[1])
+            shape_ = temp_.shape
+            coords = [np.arange(lim_) for lim_ in shape_]
+
+            out_dict[k_.lower()] = xr.DataArray(temp_, coords=coords)
+
+    return out_dict
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/resample.py` & `pyrfu-2.4.3/pyrfu/pyrf/resample.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,313 +1,313 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Built-in imports
-import bisect
-import logging
-
-# 3rd party imports
-import numpy as np
-import xarray as xr
-from scipy import interpolate
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.7"
-__status__ = "Prototype"
-
-logging.captureWarnings(True)
-logging.basicConfig(
-    format="[%(asctime)s] %(levelname)s: %(message)s",
-    datefmt="%d-%b-%y %H:%M:%S",
-    level=logging.INFO,
-)
-
-
-def _guess_sampling_frequency(ref_time):
-    r"""Compute sampling frequency of the time line."""
-
-    n_data = len(ref_time)
-
-    sfy1 = 1 / (ref_time[1] - ref_time[0])
-    sfy = None
-    not_found = True
-
-    if n_data == 2:
-        sfy = sfy1
-        not_found = False
-
-    cur, max_try = [2, 10]
-
-    while not_found and cur < n_data and cur - 3 < max_try:
-        sfy = 1 / (ref_time[cur] - ref_time[cur - 1])
-
-        if np.absolute(sfy - sfy1) < sfy * 0.001:
-            not_found = False
-
-            sfy = (sfy + sfy1) / 2
-            break
-
-        sfy = sfy1
-        cur += 1
-
-    if not_found:
-        raise RuntimeError(f"Cannot guess sampling frequency. Tried {max_try:d} times")
-
-    return sfy
-
-
-def _average(inp_time, inp_data, ref_time, thresh, dt2):
-    r"""Resample inp_data to timeline of ref_time, using half-window of dt2.
-    Points above std*tresh are excluded. thresh=0 turns off this option.
-    """
-
-    try:
-        out_data = np.zeros([len(ref_time), *inp_data.shape[1:]])
-    except IndexError:
-        inp_data = inp_data[:, None]
-        out_data = np.zeros((len(ref_time), inp_data.shape[1]))
-
-    for i, ref_t in enumerate(ref_time):
-        idx_l = bisect.bisect_left(inp_time, ref_t - dt2)
-        idx_r = bisect.bisect_right(inp_time, ref_t + dt2)
-
-        idx = np.arange(idx_l, idx_r)
-
-        if idx.size == 0:
-            out_data[i, ...] = np.nan
-        else:
-            if thresh:
-                std_ = np.std(inp_data[idx, ...], axis=0)
-                mean_ = np.mean(inp_data[idx, ...], axis=0)
-
-                assert any(np.isnan(std_))
-
-                for j, stdd in enumerate(std_):
-                    if not np.isnan(stdd):
-                        idx_r = bisect.bisect_right(
-                            inp_data[idx, j + 1] - mean_[j],
-                            thresh * stdd,
-                        )
-                        if idx_r:
-                            out_data[i, j + 1] = np.mean(
-                                inp_data[idx[idx_r], j + 1],
-                                axis=0,
-                            )
-                        else:
-                            out_data[i, j + 1] = np.nan
-                    else:
-                        out_data[i, ...] = np.nan
-
-            else:
-                out_data[i, ...] = np.mean(inp_data[idx, ...], axis=0)
-
-    if out_data.ndim > 1 and out_data.shape[1] == 1:
-        out_data = out_data[:, 0]
-
-    return out_data
-
-
-def _resample_dataarray(inp, ref, method, f_s, window, thresh):
-    r"""Resample for time series (xarray.DataArray)"""
-
-    flag_do = "check"
-
-    if method:
-        flag_do = "interpolation"
-
-    if f_s is not None:
-        sfy = f_s
-    elif window is not None:
-        sfy = 1 / window
-    else:
-        sfy = None
-
-    inp_time = inp.time.data.view("i8") * 1e-9
-    ref_time = ref.time.data.view("i8") * 1e-9
-
-    if flag_do == "check":
-        if len(ref_time) > 1:
-            if not sfy:
-                sfy = _guess_sampling_frequency(ref_time)
-
-            if len(inp_time) / (inp_time[-1] - inp_time[0]) > 2 * sfy:
-                flag_do = "average"
-                logging.info("Using averages in resample")
-            else:
-                flag_do = "interpolation"
-        else:
-            flag_do = "interpolation"
-
-    assert flag_do in ["average", "interpolation"]
-
-    if flag_do == "average":
-        assert not method, "cannot mix interpolation and averaging flags"
-
-        if not sfy:
-            sfy = _guess_sampling_frequency(ref_time)
-
-        out_data = _average(inp_time, inp.data, ref_time, thresh, 0.5 / sfy)
-
-    else:
-        if not method:
-            method = "linear"
-
-        # If time series agree, no interpolation is necessary.
-        if len(inp_time) == len(ref_time) and all(inp_time == ref_time):
-            out_data = inp.data.copy()
-            coord = [ref.coords["time"].data]
-
-            if len(inp.coords) > 1:
-                for k in list(inp.dims)[1:]:
-                    coord.append(inp.coords[k].data)
-
-            out = xr.DataArray(
-                out_data,
-                coords=coord,
-                dims=inp.dims,
-                attrs=inp.attrs,
-            )
-
-            return out
-
-        tck = interpolate.interp1d(
-            inp_time,
-            inp.data,
-            kind=method,
-            axis=0,
-            fill_value="extrapolate",
-        )
-        out_data = tck(ref_time)
-
-    coord = [ref.coords["time"]]
-
-    if len(inp.coords) > 1:
-        for k in list(inp.dims)[1:]:
-            coord.append(inp.coords[k].data)
-
-    out = xr.DataArray(out_data, coords=coord, dims=inp.dims, attrs=inp.attrs)
-
-    return out
-
-
-def _resample_dataset(inp, ref, **kwargs):
-    r"""Resample for VDFs (xarray.Dataset)"""
-    # Find time dependent zVariables and resample
-    tdepnd_zvars = list(filter(lambda x: "time" in inp[x].dims, inp))
-    out_dict = {k: _resample_dataarray(inp[k], ref, **kwargs) for k in tdepnd_zvars}
-
-    # Complete the dictionary with non-time dependent zVaraiables
-    ndepnd_zvars = list(filter(lambda x: x not in tdepnd_zvars, inp))
-    out_dict = {**out_dict, **{k: inp[k] for k in ndepnd_zvars}}
-
-    # Find array_like attributes
-    arr_attrs = filter(
-        lambda x: isinstance(inp.attrs[x], np.ndarray),
-        inp.attrs,
-    )
-    arr_attrs = list(arr_attrs)
-
-    # Initialize attributes dictionary with non array_like attributes
-    gen_attrs = filter(lambda x: x not in arr_attrs, inp.attrs)
-    out_attrs = {k: inp.attrs[k] for k in list(gen_attrs)}
-
-    for k in arr_attrs:
-        attr = inp.attrs[k]
-
-        # If array_like attributes have one dimension equal to time length
-        # assume time dependent. One option would be move the time dependent
-        # array_like attributes to time series to zVaraibles to avoid
-        # confusion
-        if attr.shape[0] == len(inp.time.data):
-            coords = [np.arange(attr.shape[i + 1]) for i in range(attr.ndim - 1)]
-            dims = [f"idx{i:d}" for i in range(attr.ndim - 1)]
-            attr_ts = xr.DataArray(
-                attr,
-                coords=[inp.time.data, *coords],
-                dims=["time", *dims],
-            )
-            out_attrs[k] = _resample_dataarray(attr_ts, ref, **kwargs).data
-        else:
-            out_attrs[k] = attr
-
-    out_attrs = {k: out_attrs[k] for k in sorted(out_attrs)}
-
-    # Make output Dataset
-    out = xr.Dataset(out_dict, attrs=out_attrs)
-
-    return out
-
-
-def resample(
-    inp,
-    ref,
-    method: str = "",
-    f_s: float = None,
-    window: int = None,
-    thresh: float = 0,
-):
-    r"""Resample inp to the time line of ref. If sampling of X is more than two
-    times higher than Y, we average X, otherwise we interpolate X.
-
-    Parameters
-    ----------
-    inp : xarray.DataArray or xarray.Dataset
-        Time series to resample.
-    ref : xarray.DataArray
-        Reference time line.
-    method : str, Optional
-        Method of interpolation "spline", "linear" etc.
-        (default "linear") if method is given then interpolate
-        independent of sampling.
-    f_s : float, Optional
-        Sampling frequency of the Y signal, 1/window.
-    window : int or float or ndarray, Optional
-        Length of the averaging window, 1/fsample.
-    thresh : float, Optional
-        Points above STD*THRESH are disregarded for averaging
-
-    Returns
-    -------
-    out : xarray.DataArray
-        Resampled input to the reference time line using the selected method.
-
-    TODO
-    ----
-    Make the resampling VDF (xarray.Dataset) compliant.
-
-
-    Examples
-    --------
-    >>> from pyrfu import mms, pyrf
-
-    Time interval
-
-    >>> tint = ["2015-10-30T05:15:20.000", "2015-10-30T05:16:20.000"]
-
-    Spacecraft index
-
-    >>> mms_id = 1
-
-    Load magnetic field and electric field
-
-    >>> b_xyz = mms.get_data("B_gse_fgm_srvy_l2", tint, mms_id)
-    >>> e_xyz = mms.get_data("E_gse_edp_fast_l2", tint, mms_id)
-
-    Resample magnetic field to electric field sampling
-
-    >>> b_xyz = pyrf.resample(b_xyz, e_xyz)
-
-    """
-
-    options = {"method": method, "f_s": f_s, "window": window, "thresh": thresh}
-
-    if isinstance(inp, xr.DataArray):
-        out = _resample_dataarray(inp, ref, **options)
-    elif isinstance(inp, xr.Dataset):
-        out = _resample_dataset(inp, ref, **options)
-    else:
-        raise TypeError("Invalid input type. Input must be a xarray!!")
-
-    return out
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# Built-in imports
+import bisect
+import logging
+
+# 3rd party imports
+import numpy as np
+import xarray as xr
+from scipy import interpolate
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+logging.captureWarnings(True)
+logging.basicConfig(
+    format="[%(asctime)s] %(levelname)s: %(message)s",
+    datefmt="%d-%b-%y %H:%M:%S",
+    level=logging.INFO,
+)
+
+
+def _guess_sampling_frequency(ref_time):
+    r"""Compute sampling frequency of the time line."""
+
+    n_data = len(ref_time)
+
+    sfy1 = 1 / (ref_time[1] - ref_time[0])
+    sfy = None
+    not_found = True
+
+    if n_data == 2:
+        sfy = sfy1
+        not_found = False
+
+    cur, max_try = [2, 10]
+
+    while not_found and cur < n_data and cur - 3 < max_try:
+        sfy = 1 / (ref_time[cur] - ref_time[cur - 1])
+
+        if np.absolute(sfy - sfy1) < sfy * 0.001:
+            not_found = False
+
+            sfy = (sfy + sfy1) / 2
+            break
+
+        sfy = sfy1
+        cur += 1
+
+    if not_found:
+        raise RuntimeError(f"Cannot guess sampling frequency. Tried {max_try:d} times")
+
+    return sfy
+
+
+def _average(inp_time, inp_data, ref_time, thresh, dt2):
+    r"""Resample inp_data to timeline of ref_time, using half-window of dt2.
+    Points above std*tresh are excluded. thresh=0 turns off this option.
+    """
+
+    try:
+        out_data = np.zeros([len(ref_time), *inp_data.shape[1:]])
+    except IndexError:
+        inp_data = inp_data[:, None]
+        out_data = np.zeros((len(ref_time), inp_data.shape[1]))
+
+    for i, ref_t in enumerate(ref_time):
+        idx_l = bisect.bisect_left(inp_time, ref_t - dt2)
+        idx_r = bisect.bisect_right(inp_time, ref_t + dt2)
+
+        idx = np.arange(idx_l, idx_r)
+
+        if idx.size == 0:
+            out_data[i, ...] = np.nan
+        else:
+            if thresh:
+                std_ = np.std(inp_data[idx, ...], axis=0)
+                mean_ = np.mean(inp_data[idx, ...], axis=0)
+
+                assert any(np.isnan(std_))
+
+                for j, stdd in enumerate(std_):
+                    if not np.isnan(stdd):
+                        idx_r = bisect.bisect_right(
+                            inp_data[idx, j + 1] - mean_[j],
+                            thresh * stdd,
+                        )
+                        if idx_r:
+                            out_data[i, j + 1] = np.mean(
+                                inp_data[idx[idx_r], j + 1],
+                                axis=0,
+                            )
+                        else:
+                            out_data[i, j + 1] = np.nan
+                    else:
+                        out_data[i, ...] = np.nan
+
+            else:
+                out_data[i, ...] = np.mean(inp_data[idx, ...], axis=0)
+
+    if out_data.ndim > 1 and out_data.shape[1] == 1:
+        out_data = out_data[:, 0]
+
+    return out_data
+
+
+def _resample_dataarray(inp, ref, method, f_s, window, thresh):
+    r"""Resample for time series (xarray.DataArray)"""
+
+    flag_do = "check"
+
+    if method:
+        flag_do = "interpolation"
+
+    if f_s is not None:
+        sfy = f_s
+    elif window is not None:
+        sfy = 1 / window
+    else:
+        sfy = None
+
+    inp_time = inp.time.data.view("i8") * 1e-9
+    ref_time = ref.time.data.view("i8") * 1e-9
+
+    if flag_do == "check":
+        if len(ref_time) > 1:
+            if not sfy:
+                sfy = _guess_sampling_frequency(ref_time)
+
+            if len(inp_time) / (inp_time[-1] - inp_time[0]) > 2 * sfy:
+                flag_do = "average"
+                logging.info("Using averages in resample")
+            else:
+                flag_do = "interpolation"
+        else:
+            flag_do = "interpolation"
+
+    assert flag_do in ["average", "interpolation"]
+
+    if flag_do == "average":
+        assert not method, "cannot mix interpolation and averaging flags"
+
+        if not sfy:
+            sfy = _guess_sampling_frequency(ref_time)
+
+        out_data = _average(inp_time, inp.data, ref_time, thresh, 0.5 / sfy)
+
+    else:
+        if not method:
+            method = "linear"
+
+        # If time series agree, no interpolation is necessary.
+        if len(inp_time) == len(ref_time) and all(inp_time == ref_time):
+            out_data = inp.data.copy()
+            coord = [ref.coords["time"].data]
+
+            if len(inp.coords) > 1:
+                for k in list(inp.dims)[1:]:
+                    coord.append(inp.coords[k].data)
+
+            out = xr.DataArray(
+                out_data,
+                coords=coord,
+                dims=inp.dims,
+                attrs=inp.attrs,
+            )
+
+            return out
+
+        tck = interpolate.interp1d(
+            inp_time,
+            inp.data,
+            kind=method,
+            axis=0,
+            fill_value="extrapolate",
+        )
+        out_data = tck(ref_time)
+
+    coord = [ref.coords["time"]]
+
+    if len(inp.coords) > 1:
+        for k in list(inp.dims)[1:]:
+            coord.append(inp.coords[k].data)
+
+    out = xr.DataArray(out_data, coords=coord, dims=inp.dims, attrs=inp.attrs)
+
+    return out
+
+
+def _resample_dataset(inp, ref, **kwargs):
+    r"""Resample for VDFs (xarray.Dataset)"""
+    # Find time dependent zVariables and resample
+    tdepnd_zvars = list(filter(lambda x: "time" in inp[x].dims, inp))
+    out_dict = {k: _resample_dataarray(inp[k], ref, **kwargs) for k in tdepnd_zvars}
+
+    # Complete the dictionary with non-time dependent zVaraiables
+    ndepnd_zvars = list(filter(lambda x: x not in tdepnd_zvars, inp))
+    out_dict = {**out_dict, **{k: inp[k] for k in ndepnd_zvars}}
+
+    # Find array_like attributes
+    arr_attrs = filter(
+        lambda x: isinstance(inp.attrs[x], np.ndarray),
+        inp.attrs,
+    )
+    arr_attrs = list(arr_attrs)
+
+    # Initialize attributes dictionary with non array_like attributes
+    gen_attrs = filter(lambda x: x not in arr_attrs, inp.attrs)
+    out_attrs = {k: inp.attrs[k] for k in list(gen_attrs)}
+
+    for k in arr_attrs:
+        attr = inp.attrs[k]
+
+        # If array_like attributes have one dimension equal to time length
+        # assume time dependent. One option would be move the time dependent
+        # array_like attributes to time series to zVaraibles to avoid
+        # confusion
+        if attr.shape[0] == len(inp.time.data):
+            coords = [np.arange(attr.shape[i + 1]) for i in range(attr.ndim - 1)]
+            dims = [f"idx{i:d}" for i in range(attr.ndim - 1)]
+            attr_ts = xr.DataArray(
+                attr,
+                coords=[inp.time.data, *coords],
+                dims=["time", *dims],
+            )
+            out_attrs[k] = _resample_dataarray(attr_ts, ref, **kwargs).data
+        else:
+            out_attrs[k] = attr
+
+    out_attrs = {k: out_attrs[k] for k in sorted(out_attrs)}
+
+    # Make output Dataset
+    out = xr.Dataset(out_dict, attrs=out_attrs)
+
+    return out
+
+
+def resample(
+    inp,
+    ref,
+    method: str = "",
+    f_s: float = None,
+    window: int = None,
+    thresh: float = 0,
+):
+    r"""Resample inp to the time line of ref. If sampling of X is more than two
+    times higher than Y, we average X, otherwise we interpolate X.
+
+    Parameters
+    ----------
+    inp : xarray.DataArray or xarray.Dataset
+        Time series to resample.
+    ref : xarray.DataArray
+        Reference time line.
+    method : str, Optional
+        Method of interpolation "spline", "linear" etc.
+        (default "linear") if method is given then interpolate
+        independent of sampling.
+    f_s : float, Optional
+        Sampling frequency of the Y signal, 1/window.
+    window : int or float or ndarray, Optional
+        Length of the averaging window, 1/fsample.
+    thresh : float, Optional
+        Points above STD*THRESH are disregarded for averaging
+
+    Returns
+    -------
+    out : xarray.DataArray
+        Resampled input to the reference time line using the selected method.
+
+    TODO
+    ----
+    Make the resampling VDF (xarray.Dataset) compliant.
+
+
+    Examples
+    --------
+    >>> from pyrfu import mms, pyrf
+
+    Time interval
+
+    >>> tint = ["2015-10-30T05:15:20.000", "2015-10-30T05:16:20.000"]
+
+    Spacecraft index
+
+    >>> mms_id = 1
+
+    Load magnetic field and electric field
+
+    >>> b_xyz = mms.get_data("B_gse_fgm_srvy_l2", tint, mms_id)
+    >>> e_xyz = mms.get_data("E_gse_edp_fast_l2", tint, mms_id)
+
+    Resample magnetic field to electric field sampling
+
+    >>> b_xyz = pyrf.resample(b_xyz, e_xyz)
+
+    """
+
+    options = {"method": method, "f_s": f_s, "window": window, "thresh": thresh}
+
+    if isinstance(inp, xr.DataArray):
+        out = _resample_dataarray(inp, ref, **options)
+    elif isinstance(inp, xr.Dataset):
+        out = _resample_dataset(inp, ref, **options)
+    else:
+        raise TypeError("Invalid input type. Input must be a xarray!!")
+
+    return out
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/shock_models_parameters.json` & `pyrfu-2.4.3/pyrfu/pyrf/shock_models_parameters.json`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/shock_normal.py` & `pyrfu-2.4.3/pyrfu/pyrf/shock_normal.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from scipy import constants, interpolate, optimize
 from scipy.spatial.transform import Rotation as R
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.29"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 __all__ = ["shock_normal"]
 
 
 def shock_normal(spec, leq90: bool = True):
     r"""Calculates shock normals with different methods. Normal vectors are calculated
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/shock_parameters.py` & `pyrfu-2.4.3/pyrfu/pyrf/shock_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import numpy as np
 from scipy import constants
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
 __copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.29"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 __all__ = ["shock_parameters"]
 
 logging.captureWarnings(True)
 logging.basicConfig(
     format="[%(asctime)s] %(levelname)s: %(message)s",
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/solid_angle.py` & `pyrfu-2.4.3/pyrfu/pyrf/solid_angle.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def solid_angle(inp0, inp1, inp2):
     r"""Calculates the solid angle of three vectors making up a triangle
     in a unit sphere with the sign taken into account.
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/sph2cart.py` & `pyrfu-2.4.3/pyrfu/pyrf/sph2cart.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def sph2cart(azimuth, elevation, r):
     r"""Transform spherical to cartesian coordinates
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/st_diff.py` & `pyrfu-2.4.3/pyrfu/pyrf/st_diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 # Local imports
 from .c_4_grad import c_4_grad
 from .gradient import gradient
 from .ts_vec_xyz import ts_vec_xyz
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def st_diff(r_mms, b_mms, lmn):
     r"""Computes velocity of the structure using spatio-temporal
     derivative method [13]_ [14]_ as
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/struct_func.py` & `pyrfu-2.4.3/pyrfu/pyrf/struct_func.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# 3rd party imports
-import numpy as np
-import xarray as xr
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2022"
-__license__ = "MIT"
-__version__ = "2.3.23"
-__status__ = "Prototype"
-
-
-def struct_func(inp, scales, order):
-    r"""Returns the structure function of a time series
-
-    .. math::
-
-       y= \frac{1}{N-s}\sum_{i=1}^{N-s}(x_i - x_{i+s})^o
-
-    where :math:`s` is the scale, and :math:`o` is the order.
-
-    Parameters
-    ----------
-    inp : xarray.DataArray
-        Input time series.
-    scales : array_like
-        A list or an array containing the scales to calculate.
-    order : int
-        Order of the exponential of the structure function.
-
-    Returns
-    -------
-    values : xarray.DataArray
-        An xarray containing the structure functions, one per product in
-        the original time series. The index coordinate contains the scale
-        value, and the attribute 'order' keeps a record on the order used
-        for its calculation.
-
-    """
-
-    if scales is None:
-        scales = [1]
-
-    data = inp.data
-
-    if data.ndim == 1:
-        data = np.transpose(np.atleast_2d(data))
-
-    result = []
-    for scale in scales:
-        result.append(
-            np.nanmean(
-                np.abs(data[scale:, :] - data[:-scale, :]) ** order,
-                axis=0,
-            ),
-        )
-
-    if inp.data.ndim == 1:
-        result = xr.DataArray(
-            np.squeeze(result),
-            coords=[scales],
-            dims=["scale"],
-            attrs=inp.attrs,
-        )
-    else:
-        result = xr.DataArray(
-            np.squeeze(result),
-            coords=[scales, inp.coords[inp.dims[1]]],
-            dims=["scale", inp.dims[1]],
-            attrs=inp.attrs,
-        )
-
-    result.attrs["order"] = order
-
-    return result
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# 3rd party imports
+import numpy as np
+import xarray as xr
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def struct_func(inp, scales, order):
+    r"""Returns the structure function of a time series
+
+    .. math::
+
+       y= \frac{1}{N-s}\sum_{i=1}^{N-s}(x_i - x_{i+s})^o
+
+    where :math:`s` is the scale, and :math:`o` is the order.
+
+    Parameters
+    ----------
+    inp : xarray.DataArray
+        Input time series.
+    scales : array_like
+        A list or an array containing the scales to calculate.
+    order : int
+        Order of the exponential of the structure function.
+
+    Returns
+    -------
+    values : xarray.DataArray
+        An xarray containing the structure functions, one per product in
+        the original time series. The index coordinate contains the scale
+        value, and the attribute 'order' keeps a record on the order used
+        for its calculation.
+
+    """
+
+    if scales is None:
+        scales = [1]
+
+    data = inp.data
+
+    if data.ndim == 1:
+        data = np.transpose(np.atleast_2d(data))
+
+    result = []
+    for scale in scales:
+        result.append(
+            np.nanmean(
+                np.abs(data[scale:, :] - data[:-scale, :]) ** order,
+                axis=0,
+            ),
+        )
+
+    if inp.data.ndim == 1:
+        result = xr.DataArray(
+            np.squeeze(result),
+            coords=[scales],
+            dims=["scale"],
+            attrs=inp.attrs,
+        )
+    else:
+        result = xr.DataArray(
+            np.squeeze(result),
+            coords=[scales, inp.coords[inp.dims[1]]],
+            dims=["scale", inp.dims[1]],
+            attrs=inp.attrs,
+        )
+
+    result.attrs["order"] = order
+
+    return result
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/trace.py` & `pyrfu-2.4.3/pyrfu/pyrf/trace.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def trace(inp):
     r"""Computes trace of the time series of 2nd order tensors.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/transformation_indices.json` & `pyrfu-2.4.3/pyrfu/pyrf/transformation_indices.json`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/ts_append.py` & `pyrfu-2.4.3/pyrfu/pyrf/ts_append.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def ts_append(inp1, inp2):
     r"""Concatenate two time series along the time axis.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/ts_scalar.py` & `pyrfu-2.4.3/pyrfu/pyrf/ts_scalar.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def ts_scalar(time, data, attrs: dict = None):
     r"""Create a time series containing a 0th order tensor
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/ts_skymap.py` & `pyrfu-2.4.3/pyrfu/pyrf/ts_skymap.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# 3rd party imports
-import numpy as np
-import xarray as xr
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2023"
-__license__ = "MIT"
-__version__ = "2.3.26"
-__status__ = "Prototype"
-
-
-def ts_skymap(time, data, energy, phi, theta, **kwargs):
-    r"""Creates a skymap of the distribution function.
-
-    Parameters
-    ----------
-    time : array_like
-        List of times.
-    data : array_like
-        Values of the distribution function.
-    energy : array_like
-        Energy levels.
-    phi : array_like
-        Azimuthal angles.
-    theta : array_like
-        Elevation angles.
-
-    Other Parameters
-    ---------------
-    **kwargs
-        Hash table of keyword arguments with :
-            * energy0 : array_like
-                Energy table 0 (odd time indices).
-            * energy1 : array_like
-                Energy table 1 (even time indices).
-            * esteptable : array_like
-                Time series of the stepping table between energies (burst).
-
-    Returns
-    -------
-    out : xarray.Dataset
-        Skymap of the distribution function.
-
-    """
-
-    # Check if even (odd) time step energy channels energy1 (energy0), and
-    # energy step table are provided.
-    energy0 = kwargs.get("energy0", None)
-    energy1 = kwargs.get("energy1", None)
-    esteptable = kwargs.get("esteptable", None)
-    attrs = kwargs.get("attrs", {})
-    coords_attrs = kwargs.get("coords_attrs", {})
-    glob_attrs = kwargs.get("glob_attrs", {})
-
-    if energy is None:
-        assert energy0 is not None and energy1 is not None and esteptable is not None
-
-        energy = np.tile(energy0, (len(esteptable), 1))
-
-        energy[esteptable == 1] = np.tile(
-            energy1,
-            (int(np.sum(esteptable)), 1),
-        )
-
-    if phi.ndim == 1:
-        phi = np.tile(phi, (len(time), 1))
-
-    out_dict = {
-        "data": (["time", "idx0", "idx1", "idx2"], data),
-        "phi": (["time", "idx1"], phi),
-        "theta": (["idx2"], theta),
-        "energy": (["time", "idx0"], energy),
-        "time": time,
-        "idx0": np.arange(energy.shape[1]),
-        "idx1": np.arange(phi.shape[1]),
-        "idx2": np.arange(len(theta)),
-    }
-
-    # Construct global attributes and sort them
-    # remove energy0, energy1, and esteptable from global attrs to overwrite
-    overwrite_keys = ["energy0", "energy1", "esteptable"]
-    glob_attrs = {k: glob_attrs[k] for k in glob_attrs if k not in overwrite_keys}
-    glob_attrs = {
-        "energy0": energy0,
-        "energy1": energy1,
-        "esteptable": esteptable,
-        **glob_attrs,
-    }
-
-    glob_attrs = {k: glob_attrs[k] for k in sorted(glob_attrs)}
-
-    # Create Dataset
-    out = xr.Dataset(out_dict, attrs=glob_attrs)
-
-    # Sort and fill coordinates attributes
-    for k in coords_attrs:
-        out[k].attrs = {m: coords_attrs[k][m] for m in sorted(coords_attrs[k])}
-
-    # Sort and fill data attributes
-    out.data.attrs = {k: attrs[k] for k in sorted(attrs)}
-
-    return out
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# 3rd party imports
+import numpy as np
+import xarray as xr
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def ts_skymap(time, data, energy, phi, theta, **kwargs):
+    r"""Creates a skymap of the distribution function.
+
+    Parameters
+    ----------
+    time : array_like
+        List of times.
+    data : array_like
+        Values of the distribution function.
+    energy : array_like
+        Energy levels.
+    phi : array_like
+        Azimuthal angles.
+    theta : array_like
+        Elevation angles.
+
+    Other Parameters
+    ---------------
+    **kwargs
+        Hash table of keyword arguments with :
+            * energy0 : array_like
+                Energy table 0 (odd time indices).
+            * energy1 : array_like
+                Energy table 1 (even time indices).
+            * esteptable : array_like
+                Time series of the stepping table between energies (burst).
+
+    Returns
+    -------
+    out : xarray.Dataset
+        Skymap of the distribution function.
+
+    """
+
+    # Check if even (odd) time step energy channels energy1 (energy0), and
+    # energy step table are provided.
+    energy0 = kwargs.get("energy0", None)
+    energy1 = kwargs.get("energy1", None)
+    esteptable = kwargs.get("esteptable", None)
+    attrs = kwargs.get("attrs", {})
+    coords_attrs = kwargs.get("coords_attrs", {})
+    glob_attrs = kwargs.get("glob_attrs", {})
+
+    if energy is None:
+        assert energy0 is not None and energy1 is not None and esteptable is not None
+
+        energy = np.tile(energy0, (len(esteptable), 1))
+
+        energy[esteptable == 1] = np.tile(
+            energy1,
+            (int(np.sum(esteptable)), 1),
+        )
+
+    if phi.ndim == 1:
+        phi = np.tile(phi, (len(time), 1))
+
+    out_dict = {
+        "data": (["time", "idx0", "idx1", "idx2"], data),
+        "phi": (["time", "idx1"], phi),
+        "theta": (["idx2"], theta),
+        "energy": (["time", "idx0"], energy),
+        "time": time,
+        "idx0": np.arange(energy.shape[1]),
+        "idx1": np.arange(phi.shape[1]),
+        "idx2": np.arange(len(theta)),
+    }
+
+    # Construct global attributes and sort them
+    # remove energy0, energy1, and esteptable from global attrs to overwrite
+    overwrite_keys = ["energy0", "energy1", "esteptable"]
+    glob_attrs = {k: glob_attrs[k] for k in glob_attrs if k not in overwrite_keys}
+    glob_attrs = {
+        "energy0": energy0,
+        "energy1": energy1,
+        "esteptable": esteptable,
+        **glob_attrs,
+    }
+
+    glob_attrs = {k: glob_attrs[k] for k in sorted(glob_attrs)}
+
+    # Create Dataset
+    out = xr.Dataset(out_dict, attrs=glob_attrs)
+
+    # Sort and fill coordinates attributes
+    for k in coords_attrs:
+        out[k].attrs = {m: coords_attrs[k][m] for m in sorted(coords_attrs[k])}
+
+    # Sort and fill data attributes
+    out.data.attrs = {k: attrs[k] for k in sorted(attrs)}
+
+    return out
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/ts_tensor_xyz.py` & `pyrfu-2.4.3/pyrfu/pyrf/ts_tensor_xyz.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def ts_tensor_xyz(time, data, attrs: dict = None):
     r"""Create a time series containing a 2nd order tensor.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/ts_time.py` & `pyrfu-2.4.3/pyrfu/pyrf/ts_time.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # 3rd party imports
 import numpy as np
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def ts_time(time):
     r"""Creates time line in DataArray.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/ts_vec_xyz.py` & `pyrfu-2.4.3/pyrfu/pyrf/ts_vec_xyz.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import xarray as xr
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def ts_vec_xyz(time, data, attrs: dict = None):
     r"""Create a time series containing a 1st order tensor.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/ttns2datetime64.py` & `pyrfu-2.4.3/pyrfu/pyrf/ttns2datetime64.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from cdflib import cdfepoch
 
 # Local imports
 from .timevec2iso8601 import timevec2iso8601
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def ttns2datetime64(time):
     r"""Convert time in epoch_tt2000 (nanosedconds since J2000) to datetime64
     in ns units.
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/unix2datetime64.py` & `pyrfu-2.4.3/pyrfu/pyrf/unix2datetime64.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def unix2datetime64(time):
     r"""Converts unix time to datetime64 in ns units.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/vht.py` & `pyrfu-2.4.3/pyrfu/pyrf/vht.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from .e_vxb import e_vxb
 
 # Local imports
 from .resample import resample
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def vht(e, b, flag: int = 1):
     r"""Estimate velocity of the De Hoffman-Teller frame from the velocity
     estimate the electric field eht=-vht x b
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/wave_fft.py` & `pyrfu-2.4.3/pyrfu/pyrf/wave_fft.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# 3rd party imports
-import numpy as np
-from scipy import signal
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.7"
-__status__ = "Prototype"
-
-
-def wave_fft(
-    inp,
-    window,
-    frame_overlap: float = 10.0,
-    frame_length: float = 20.0,
-    f_sampling: float = None,
-):
-    r"""Short-Time Fourier Transform.
-
-    Parameters
-    ----------
-    inp : xarray.DataArray
-        Time series of the one dimension data.
-    window : str
-        Window function such as rectwin, hamming (default).
-    frame_overlap : float, Optional
-        Length of each frame overlaps in second.
-    frame_length : float, Optional
-        Length of each frame in second.
-    f_sampling : float, Optional
-        Sampling frequency.
-
-    Returns
-    -------
-    spectrogram : ndarray
-        Spectrogram of x.
-    time : ndarray
-        Value corresponds to the center of each frame (x-axis) in sec.
-    frequencies : ndarray
-        Vector of frequencies (y-axis) in Hz.
-
-    """
-
-    if f_sampling is None:
-        delta_t = np.median(np.diff(inp.time.data).astype(np.float64)) * 1e-9
-        f_sampling = 1 / delta_t
-
-    # convert ms to points
-    n_per_seg = np.round(frame_length * f_sampling).astype(np.int64)
-    n_overlap = np.round(frame_overlap * f_sampling).astype(np.int64)
-
-    options = {
-        "fs": f_sampling,
-        "window": window,
-        "nperseg": n_per_seg,
-        "noverlap": n_overlap,
-        "mode": "complex",
-    }
-    frequencies, time, spectrogram = signal.spectrogram(inp, **options)
-
-    return frequencies, time, spectrogram
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# 3rd party imports
+import numpy as np
+from scipy import signal
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def wave_fft(
+    inp,
+    window,
+    frame_overlap: float = 10.0,
+    frame_length: float = 20.0,
+    f_sampling: float = None,
+):
+    r"""Short-Time Fourier Transform.
+
+    Parameters
+    ----------
+    inp : xarray.DataArray
+        Time series of the one dimension data.
+    window : str
+        Window function such as rectwin, hamming (default).
+    frame_overlap : float, Optional
+        Length of each frame overlaps in second.
+    frame_length : float, Optional
+        Length of each frame in second.
+    f_sampling : float, Optional
+        Sampling frequency.
+
+    Returns
+    -------
+    spectrogram : ndarray
+        Spectrogram of x.
+    time : ndarray
+        Value corresponds to the center of each frame (x-axis) in sec.
+    frequencies : ndarray
+        Vector of frequencies (y-axis) in Hz.
+
+    """
+
+    if f_sampling is None:
+        delta_t = np.median(np.diff(inp.time.data).astype(np.float64)) * 1e-9
+        f_sampling = 1 / delta_t
+
+    # convert ms to points
+    n_per_seg = np.round(frame_length * f_sampling).astype(np.int64)
+    n_overlap = np.round(frame_overlap * f_sampling).astype(np.int64)
+
+    options = {
+        "fs": f_sampling,
+        "window": window,
+        "nperseg": n_per_seg,
+        "noverlap": n_overlap,
+        "mode": "complex",
+    }
+    frequencies, time, spectrogram = signal.spectrogram(inp, **options)
+
+    return frequencies, time, spectrogram
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/wavelet.py` & `pyrfu-2.4.3/pyrfu/pyrf/wavelet.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,211 +1,211 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-import logging
-
-# Built-in imports
-import os
-
-# 3rd party imports
-import numba
-import numpy as np
-import xarray as xr
-from scipy import fft
-
-# Local imports
-from .calc_fs import calc_fs
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
-__license__ = "MIT"
-__version__ = "2.3.7"
-__status__ = "Prototype"
-
-logging.captureWarnings(True)
-logging.basicConfig(
-    format="[%(asctime)s] %(levelname)s: %(message)s",
-    datefmt="%d-%b-%y %H:%M:%S",
-    level=logging.INFO,
-)
-
-
-@numba.jit(nopython=True, fastmath=True)
-def _ww(s_ww, scales_mat, sigma, frequencies_mat, f_nyq):
-    # TODO : use nested for loop and math instead of numpy and test speed!!
-    w_w = s_ww * np.exp(
-        -sigma * sigma * ((scales_mat * frequencies_mat - f_nyq) ** 2) / 2,
-    )
-    w_w = w_w * np.sqrt(1)
-    return w_w
-
-
-@numba.jit(nopython=True, parallel=True, fastmath=True)
-def _power_r(power, new_freq_mat):
-    power2 = np.absolute((2 * np.pi) * np.conj(power) * power / new_freq_mat)
-    return power2
-
-
-@numba.jit(nopython=True, parallel=True, fastmath=True)
-def _power_c(power, new_freq_mat):
-    power2 = np.sqrt(np.absolute((2 * np.pi) / new_freq_mat)) * power
-    return power2
-
-
-def wavelet(inp, **kwargs):
-    """Computes wavelet spectrogram based on fast FFT algorithm.
-    Parameters
-    ----------
-    inp : xarray.DataArray
-        Input quantity.
-    **kwargs : dict
-        Hash table of keyword arguments with :
-            * fs : int or float
-                Sampling frequency of the input time series.
-            * f : list or ndarray
-                Vector [f_min f_max], calculate spectra between frequencies
-                f_min and f_max.
-            * nf : int or float
-                Number of frequency bins.
-            * wavelet_width : int or float
-                Width of the Morlet wavelet. Default 5.36.
-            * linear : float
-                Linear spacing between frequencies of df.
-            * return_power : bool
-                Set to True to return the power, False for complex wavelet
-                transform. Default True.
-            * cut_edge : bool
-                Set to True to set points affected by edge effects to NaN,
-                False to keep edge affect points. Default True
-    Returns
-    -------
-    out : xarray.DataArray or xarray.Dataset
-        Wavelet transform of the input.
-    """
-
-    # Unpack time and data
-    data = inp.data
-
-    f_s = kwargs.get("fs", calc_fs(inp))
-    n_freqs = kwargs.get("nf", 200)
-    wavelet_width = kwargs.get("wavelet_width", 5.36)
-    cut_edge = kwargs.get("cut_edge", True)
-    return_power = kwargs.get("return_power", True)
-
-    if kwargs.get("linear"):
-        linear_df = True
-        if isinstance(kwargs["linear"], (int, float)):
-            delta_f = kwargs["linear"]
-        else:
-            delta_f = 100
-            logging.warning("Unknown input for linear delta_f set to 100")
-    else:
-        delta_f = 100
-        linear_df = False
-
-    scale_min, scale_max = [0.01, 2]
-
-    f_min, f_max = kwargs.get(
-        "f",
-        [0.5 * f_s / 10**scale_max, 0.5 * f_s / 10**scale_min],
-    )
-
-    f_nyq, scale_number, sigma = [f_s / 2, n_freqs, wavelet_width / (f_s / 2)]
-
-    if linear_df:
-        scale_number = np.floor(f_nyq / delta_f).astype(np.int64)
-
-        f_min, f_max = [delta_f, scale_number * delta_f]
-
-        scales = f_nyq / (np.linspace(f_max, f_min, scale_number))
-    else:
-        scale_min = np.log10(0.5 * f_s / f_max)
-        scale_max = np.log10(0.5 * f_s / f_min)
-        scales = np.logspace(scale_min, scale_max, scale_number)
-
-    # Remove the last sample if the total number of samples is odd
-    if len(data) / 2 != np.floor(len(data) / 2):
-        time = inp.time.data[:-1]
-        data = data[:-1, ...]
-    else:
-        time = inp.time.data
-
-    # Check for NaNs
-    scales[np.isnan(scales)] = 0
-
-    # Find the frequencies for an FFT of all data
-    freq = f_s * 0.5 * np.arange(1, 1 + len(data) / 2) / (len(data) / 2)
-
-    # The frequencies corresponding to FFT
-    frequencies = np.hstack([0, freq, -np.flip(freq[:-1])])
-
-    # Get the correct frequencies for the wavelet transform
-    new_freq = f_nyq / scales
-
-    if len(inp.shape) == 1:
-        out_dict, power2 = [None, np.zeros((len(inp.data), n_freqs))]
-    elif len(inp.shape) == 2:
-        out_dict, power2 = [{}, None]
-    else:
-        raise TypeError("Invalid shape of the inp")
-
-    new_freq_mat, _ = np.meshgrid(new_freq, frequencies, sparse=True)
-
-    _, frequencies_mat = np.meshgrid(scales, frequencies, sparse=True)
-
-    # if scalar add virtual axis
-    if len(inp.shape) == 1:
-        data = data[:, np.newaxis]
-
-    # go through all the data columns
-    for i in range(data.shape[1]):
-        # Make the FFT of all data
-        data_col = data[:, i]
-
-        # Wavelet transform of the data
-        # Forward FFT
-        s_w = fft.fft(data_col, workers=os.cpu_count())
-
-        scales_mat, s_w_mat = np.meshgrid(scales, s_w, sparse=True)
-
-        # Calculate the FFT of the wavelet transform
-        w_w = _ww(s_w_mat, scales_mat, sigma, frequencies_mat, f_nyq)
-
-        # Backward FFT
-        power = fft.ifft(w_w, axis=0, workers=os.cpu_count())
-
-        # Calculate the power spectrum
-        if return_power:
-            power2 = _power_r(power, np.tile(new_freq_mat, (len(power), 1)))
-        else:
-            power2 = _power_c(power, np.tile(new_freq_mat, (len(power), 1)))
-
-        if cut_edge:
-            censure = np.floor(2 * scales).astype(int)
-
-            for j in range(scale_number):
-                power2[: censure[j], j] = np.nan
-
-                power2[len(data_col) - censure[j] : len(data_col), j] = np.nan
-
-        if len(inp.shape) == 2:
-            out_dict[inp.comp.data[i]] = (
-                ["time", "frequency"],
-                np.fliplr(power2),
-            )
-
-    if len(inp.shape) == 1:
-        out = xr.DataArray(
-            np.fliplr(power2),
-            coords=[time, np.flip(new_freq)],
-            dims=["time", "frequency"],
-        )
-    elif len(inp.shape) == 2:
-        out = xr.Dataset(
-            out_dict,
-            coords={"time": time, "frequency": np.flip(new_freq)},
-        )
-    else:
-        raise TypeError("Invalid shape")
-
-    return out
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+import logging
+
+# Built-in imports
+import os
+
+# 3rd party imports
+import numba
+import numpy as np
+import xarray as xr
+from scipy import fft
+
+# Local imports
+from .calc_fs import calc_fs
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+logging.captureWarnings(True)
+logging.basicConfig(
+    format="[%(asctime)s] %(levelname)s: %(message)s",
+    datefmt="%d-%b-%y %H:%M:%S",
+    level=logging.INFO,
+)
+
+
+@numba.jit(nopython=True, fastmath=True)
+def _ww(s_ww, scales_mat, sigma, frequencies_mat, f_nyq):
+    # TODO : use nested for loop and math instead of numpy and test speed!!
+    w_w = s_ww * np.exp(
+        -sigma * sigma * ((scales_mat * frequencies_mat - f_nyq) ** 2) / 2,
+    )
+    w_w = w_w * np.sqrt(1)
+    return w_w
+
+
+@numba.jit(nopython=True, parallel=True, fastmath=True)
+def _power_r(power, new_freq_mat):
+    power2 = np.absolute((2 * np.pi) * np.conj(power) * power / new_freq_mat)
+    return power2
+
+
+@numba.jit(nopython=True, parallel=True, fastmath=True)
+def _power_c(power, new_freq_mat):
+    power2 = np.sqrt(np.absolute((2 * np.pi) / new_freq_mat)) * power
+    return power2
+
+
+def wavelet(inp, **kwargs):
+    """Computes wavelet spectrogram based on fast FFT algorithm.
+    Parameters
+    ----------
+    inp : xarray.DataArray
+        Input quantity.
+    **kwargs : dict
+        Hash table of keyword arguments with :
+            * fs : int or float
+                Sampling frequency of the input time series.
+            * f : list or ndarray
+                Vector [f_min f_max], calculate spectra between frequencies
+                f_min and f_max.
+            * nf : int or float
+                Number of frequency bins.
+            * wavelet_width : int or float
+                Width of the Morlet wavelet. Default 5.36.
+            * linear : float
+                Linear spacing between frequencies of df.
+            * return_power : bool
+                Set to True to return the power, False for complex wavelet
+                transform. Default True.
+            * cut_edge : bool
+                Set to True to set points affected by edge effects to NaN,
+                False to keep edge affect points. Default True
+    Returns
+    -------
+    out : xarray.DataArray or xarray.Dataset
+        Wavelet transform of the input.
+    """
+
+    # Unpack time and data
+    data = inp.data
+
+    f_s = kwargs.get("fs", calc_fs(inp))
+    n_freqs = kwargs.get("nf", 200)
+    wavelet_width = kwargs.get("wavelet_width", 5.36)
+    cut_edge = kwargs.get("cut_edge", True)
+    return_power = kwargs.get("return_power", True)
+
+    if kwargs.get("linear"):
+        linear_df = True
+        if isinstance(kwargs["linear"], (int, float)):
+            delta_f = kwargs["linear"]
+        else:
+            delta_f = 100
+            logging.warning("Unknown input for linear delta_f set to 100")
+    else:
+        delta_f = 100
+        linear_df = False
+
+    scale_min, scale_max = [0.01, 2]
+
+    f_min, f_max = kwargs.get(
+        "f",
+        [0.5 * f_s / 10**scale_max, 0.5 * f_s / 10**scale_min],
+    )
+
+    f_nyq, scale_number, sigma = [f_s / 2, n_freqs, wavelet_width / (f_s / 2)]
+
+    if linear_df:
+        scale_number = np.floor(f_nyq / delta_f).astype(np.int64)
+
+        f_min, f_max = [delta_f, scale_number * delta_f]
+
+        scales = f_nyq / (np.linspace(f_max, f_min, scale_number))
+    else:
+        scale_min = np.log10(0.5 * f_s / f_max)
+        scale_max = np.log10(0.5 * f_s / f_min)
+        scales = np.logspace(scale_min, scale_max, scale_number)
+
+    # Remove the last sample if the total number of samples is odd
+    if len(data) / 2 != np.floor(len(data) / 2):
+        time = inp.time.data[:-1]
+        data = data[:-1, ...]
+    else:
+        time = inp.time.data
+
+    # Check for NaNs
+    scales[np.isnan(scales)] = 0
+
+    # Find the frequencies for an FFT of all data
+    freq = f_s * 0.5 * np.arange(1, 1 + len(data) / 2) / (len(data) / 2)
+
+    # The frequencies corresponding to FFT
+    frequencies = np.hstack([0, freq, -np.flip(freq[:-1])])
+
+    # Get the correct frequencies for the wavelet transform
+    new_freq = f_nyq / scales
+
+    if len(inp.shape) == 1:
+        out_dict, power2 = [None, np.zeros((len(inp.data), n_freqs))]
+    elif len(inp.shape) == 2:
+        out_dict, power2 = [{}, None]
+    else:
+        raise TypeError("Invalid shape of the inp")
+
+    new_freq_mat, _ = np.meshgrid(new_freq, frequencies, sparse=True)
+
+    _, frequencies_mat = np.meshgrid(scales, frequencies, sparse=True)
+
+    # if scalar add virtual axis
+    if len(inp.shape) == 1:
+        data = data[:, np.newaxis]
+
+    # go through all the data columns
+    for i in range(data.shape[1]):
+        # Make the FFT of all data
+        data_col = data[:, i]
+
+        # Wavelet transform of the data
+        # Forward FFT
+        s_w = fft.fft(data_col, workers=os.cpu_count())
+
+        scales_mat, s_w_mat = np.meshgrid(scales, s_w, sparse=True)
+
+        # Calculate the FFT of the wavelet transform
+        w_w = _ww(s_w_mat, scales_mat, sigma, frequencies_mat, f_nyq)
+
+        # Backward FFT
+        power = fft.ifft(w_w, axis=0, workers=os.cpu_count())
+
+        # Calculate the power spectrum
+        if return_power:
+            power2 = _power_r(power, np.tile(new_freq_mat, (len(power), 1)))
+        else:
+            power2 = _power_c(power, np.tile(new_freq_mat, (len(power), 1)))
+
+        if cut_edge:
+            censure = np.floor(2 * scales).astype(int)
+
+            for j in range(scale_number):
+                power2[: censure[j], j] = np.nan
+
+                power2[len(data_col) - censure[j] : len(data_col), j] = np.nan
+
+        if len(inp.shape) == 2:
+            out_dict[inp.comp.data[i]] = (
+                ["time", "frequency"],
+                np.fliplr(power2),
+            )
+
+    if len(inp.shape) == 1:
+        out = xr.DataArray(
+            np.fliplr(power2),
+            coords=[time, np.flip(new_freq)],
+            dims=["time", "frequency"],
+        )
+    elif len(inp.shape) == 2:
+        out = xr.Dataset(
+            out_dict,
+            coords={"time": time, "frequency": np.flip(new_freq)},
+        )
+    else:
+        raise TypeError("Invalid shape")
+
+    return out
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/wavepolarize_means.py` & `pyrfu-2.4.3/pyrfu/pyrf/wavepolarize_means.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 from .datetime642unix import datetime642unix
 
 # Local imports
 from .resample import resample
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 logging.captureWarnings(True)
 logging.basicConfig(
     format="[%(asctime)s] %(levelname)s: %(message)s",
     datefmt="%d-%b-%y %H:%M:%S",
     level=logging.INFO,
```

### Comparing `pyrfu-2.4.1/pyrfu/pyrf/waverage.py` & `pyrfu-2.4.3/pyrfu/pyrf/waverage.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 # -*- coding: utf-8 -*-
 
 # 3rd party imports
 import numpy as np
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 def waverage(inp, f_sampl: float = None, n_pts: int = 7):
     r"""Computes weighted average.
 
     Parameters
```

### Comparing `pyrfu-2.4.1/pyrfu/solo/db_init.py` & `pyrfu-2.4.3/pyrfu/mms/db_init.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,41 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-import json
-
-# Built-in imports
-import os
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2022"
-__license__ = "MIT"
-__version__ = "2.3.22"
-__status__ = "Prototype"
-
-
-def db_init(local_data_dir):
-    r"""Setup the default path of SolO data.
-
-    Parameters
-    ----------
-    local_data_dir : str
-        Path to the data.
-
-    """
-
-    # Normalize the path and make sure that it exists
-    local_data_dir = os.path.normpath(local_data_dir)
-    assert os.path.exists(
-        local_data_dir,
-    ), f"{local_data_dir} doesn't exists!!"
-
-    # Path to the configuration file.
-    pkg_path = os.path.dirname(os.path.abspath(__file__))
-
-    # Read the current version of the configuration
-    with open(os.path.join(pkg_path, "config.json"), "r", encoding="utf-8") as fs:
-        config = json.load(fs)
-
-    # Overwrite the configuration file with the new path
-    with open(os.path.join(pkg_path, "config.json"), "w", encoding="utf-8") as fs:
-        config["local_data_dir"] = local_data_dir
-        json.dump(config, fs)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+import json
+
+# Built-in imports
+import os
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+
+def db_init(local_data_dir):
+    r"""Setup the default path of MMS data.
+
+    Parameters
+    ----------
+    local_data_dir : str
+        Path to the data.
+
+    """
+
+    # Normalize the path and make sure that it exists
+    local_data_dir = os.path.normpath(local_data_dir)
+    assert os.path.exists(local_data_dir), f"{local_data_dir} doesn't exists!!"
+
+    # Path to the configuration file.
+    pkg_path = os.path.dirname(os.path.abspath(__file__))
+
+    # Read the current version of the configuration
+    with open(os.path.join(pkg_path, "config.json"), "r", encoding="utf-8") as fs:
+        config = json.load(fs)
+
+    # Overwrite the configuration file with the new path
+    with open(os.path.join(pkg_path, "config.json"), "w", encoding="utf-8") as fs:
+        config["local_data_dir"] = local_data_dir
+        json.dump(config, fs)
```

### Comparing `pyrfu-2.4.1/pyrfu/solo/read_lfr_density.py` & `pyrfu-2.4.3/pyrfu/solo/read_lfr_density.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,166 +1,166 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Built-in imports
-import datetime
-import json
-import logging
-import os
-import re
-
-# 3rd party imports
-import numpy as np
-from cdflib import cdfepoch
-from dateutil import parser
-from dateutil.rrule import DAILY, rrule
-
-from ..pyrf import read_cdf, ts_append, ts_scalar
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2022"
-__license__ = "MIT"
-__version__ = "2.3.22"
-__status__ = "Prototype"
-
-logging.captureWarnings(True)
-logging.basicConfig(
-    format="[%(asctime)s] %(levelname)s: %(message)s",
-    datefmt="%d-%b-%y %H:%M:%S",
-    level=logging.INFO,
-)
-
-
-def _list_files_lfr_density_l3(tint, data_path: str = "", tree: bool = False):
-    """Find files in the L2 data repo corresponding to the target time
-    interval.
-
-    Parameters
-    ----------
-    tint : list
-        Time interval
-    data_path : str, Optional
-        Path of MMS data. Default uses `pyrfu.solo.config.json`
-    tree : bool, Optional
-        Flag for tree structured data repos. Default is False.
-
-    Returns
-    -------
-    files : list
-        List of files corresponding to the parameters in the selected time
-        interval
-
-    """
-
-    # Check path
-    if not data_path:
-        # pkg_path = os.path.dirname(os.path.abspath(__file__))
-        pkg_path = os.path.dirname(os.path.abspath(__file__))
-
-        # Read the current version of the MMS configuration file
-        with open(os.path.join(pkg_path, "config.json"), "r", encoding="utf-8") as fs:
-            config = json.load(fs)
-
-        data_path = os.path.normpath(config["local_data_dir"])
-    else:
-        data_path = os.path.normpath(data_path)
-
-    # Make sure that the data path exists
-    assert os.path.exists(data_path), f"{data_path} doesn't exist!!"
-
-    files_out = []
-
-    # directory and file name search patterns:
-    # - assume directories are of the form: [path]/L3/lfr_density/year/month/
-    # - assume file names are of the form:
-    #   solo_L3_rpw-bia-density-cdag_YYYYMMDD_version.cdf
-
-    file_name = r"solo_L3_rpw-bia-density.*_([0-9]{8})_V[0-9]{2}.cdf"
-
-    d_start = parser.parse(parser.parse(tint[0]).strftime("%Y-%m-%d"))
-    until_ = parser.parse(tint[1]) - datetime.timedelta(seconds=1)
-    days = rrule(DAILY, dtstart=d_start, until=until_)
-
-    for date in days:
-        if tree:
-            local_dir = os.sep.join(
-                [
-                    data_path,
-                    "L3",
-                    "lfr_density",
-                    date.strftime("%Y"),
-                    date.strftime("%m"),
-                ],
-            )
-        else:
-            local_dir = data_path
-
-        if os.name == "nt":
-            full_path = os.sep.join(
-                [re.escape(local_dir) + os.sep, file_name],
-            )
-        else:
-            full_path = os.sep.join([re.escape(local_dir), file_name])
-
-        regex = re.compile(full_path)
-
-        for root, _, files in os.walk(local_dir):
-            for file in files:
-                this_file = os.sep.join([root, file])
-
-                matches = regex.match(this_file)
-                if matches:
-                    this_time = parser.parse(matches.groups()[0])
-                    if d_start <= this_time <= until_:
-                        if this_file not in files_out:
-                            files_out.append(os.sep.join([local_dir, file]))
-
-    # sort in time
-    if len(files_out) > 1:
-        files_out = sorted(files_out)
-
-    return files_out
-
-
-def read_lfr_density(tint, data_path: str = "", tree: bool = False):
-    r"""Read L3 density data from LFR
-
-    Parameters
-    ----------
-    tint : list
-        Time interval
-    data_path : str, Optional
-        Path of MMS data. Default uses `pyrfu.solo.config.json`
-    tree : bool, Optional
-        Flag for tree structured data repos. Default is False.
-
-    Returns
-    -------
-    out : xarray.DataArray
-        Time series of the density.
-
-    """
-
-    # List LFR density files in the data path.
-    files = _list_files_lfr_density_l3(tint, data_path, tree)
-
-    # Initialize spectrum output to None
-    out = None
-
-    for file in files:
-        # Notify user
-        logging.info("Loading %s...", os.path.split(file)[-1])
-
-        # Read file content
-        data_l3 = read_cdf(file, tint)
-
-        # Get time from Epoch
-        epoch = data_l3["epoch"].data
-        time = cdfepoch.to_datetime(epoch)
-
-        # Get density data and contruct time series.
-        density = data_l3["density"].data
-        density[density == -1e31] = np.nan
-        out = ts_append(out, ts_scalar(time, density))
-
-    return out
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# Built-in imports
+import datetime
+import json
+import logging
+import os
+import re
+
+# 3rd party imports
+import numpy as np
+from cdflib import cdfepoch
+from dateutil import parser
+from dateutil.rrule import DAILY, rrule
+
+from ..pyrf import read_cdf, ts_append, ts_scalar
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+logging.captureWarnings(True)
+logging.basicConfig(
+    format="[%(asctime)s] %(levelname)s: %(message)s",
+    datefmt="%d-%b-%y %H:%M:%S",
+    level=logging.INFO,
+)
+
+
+def _list_files_lfr_density_l3(tint, data_path: str = "", tree: bool = False):
+    """Find files in the L2 data repo corresponding to the target time
+    interval.
+
+    Parameters
+    ----------
+    tint : list
+        Time interval
+    data_path : str, Optional
+        Path of MMS data. Default uses `pyrfu.solo.config.json`
+    tree : bool, Optional
+        Flag for tree structured data repos. Default is False.
+
+    Returns
+    -------
+    files : list
+        List of files corresponding to the parameters in the selected time
+        interval
+
+    """
+
+    # Check path
+    if not data_path:
+        # pkg_path = os.path.dirname(os.path.abspath(__file__))
+        pkg_path = os.path.dirname(os.path.abspath(__file__))
+
+        # Read the current version of the MMS configuration file
+        with open(os.path.join(pkg_path, "config.json"), "r", encoding="utf-8") as fs:
+            config = json.load(fs)
+
+        data_path = os.path.normpath(config["local_data_dir"])
+    else:
+        data_path = os.path.normpath(data_path)
+
+    # Make sure that the data path exists
+    assert os.path.exists(data_path), f"{data_path} doesn't exist!!"
+
+    files_out = []
+
+    # directory and file name search patterns:
+    # - assume directories are of the form: [path]/L3/lfr_density/year/month/
+    # - assume file names are of the form:
+    #   solo_L3_rpw-bia-density-cdag_YYYYMMDD_version.cdf
+
+    file_name = r"solo_L3_rpw-bia-density.*_([0-9]{8})_V[0-9]{2}.cdf"
+
+    d_start = parser.parse(parser.parse(tint[0]).strftime("%Y-%m-%d"))
+    until_ = parser.parse(tint[1]) - datetime.timedelta(seconds=1)
+    days = rrule(DAILY, dtstart=d_start, until=until_)
+
+    for date in days:
+        if tree:
+            local_dir = os.sep.join(
+                [
+                    data_path,
+                    "L3",
+                    "lfr_density",
+                    date.strftime("%Y"),
+                    date.strftime("%m"),
+                ],
+            )
+        else:
+            local_dir = data_path
+
+        if os.name == "nt":
+            full_path = os.sep.join(
+                [re.escape(local_dir) + os.sep, file_name],
+            )
+        else:
+            full_path = os.sep.join([re.escape(local_dir), file_name])
+
+        regex = re.compile(full_path)
+
+        for root, _, files in os.walk(local_dir):
+            for file in files:
+                this_file = os.sep.join([root, file])
+
+                matches = regex.match(this_file)
+                if matches:
+                    this_time = parser.parse(matches.groups()[0])
+                    if d_start <= this_time <= until_:
+                        if this_file not in files_out:
+                            files_out.append(os.sep.join([local_dir, file]))
+
+    # sort in time
+    if len(files_out) > 1:
+        files_out = sorted(files_out)
+
+    return files_out
+
+
+def read_lfr_density(tint, data_path: str = "", tree: bool = False):
+    r"""Read L3 density data from LFR
+
+    Parameters
+    ----------
+    tint : list
+        Time interval
+    data_path : str, Optional
+        Path of MMS data. Default uses `pyrfu.solo.config.json`
+    tree : bool, Optional
+        Flag for tree structured data repos. Default is False.
+
+    Returns
+    -------
+    out : xarray.DataArray
+        Time series of the density.
+
+    """
+
+    # List LFR density files in the data path.
+    files = _list_files_lfr_density_l3(tint, data_path, tree)
+
+    # Initialize spectrum output to None
+    out = None
+
+    for file in files:
+        # Notify user
+        logging.info("Loading %s...", os.path.split(file)[-1])
+
+        # Read file content
+        data_l3 = read_cdf(file, tint)
+
+        # Get time from Epoch
+        epoch = data_l3["epoch"].data
+        time = cdfepoch.to_datetime(epoch)
+
+        # Get density data and contruct time series.
+        density = data_l3["density"].data
+        density[density == -1e31] = np.nan
+        out = ts_append(out, ts_scalar(time, density))
+
+    return out
```

### Comparing `pyrfu-2.4.1/pyrfu/solo/read_tnr.py` & `pyrfu-2.4.3/pyrfu/solo/read_tnr.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,280 +1,280 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Built-in imports
-import datetime
-import json
-import logging
-import os
-import re
-
-# 3rd party imports
-import numpy as np
-import xarray as xr
-from cdflib import cdfepoch
-from dateutil import parser
-from dateutil.rrule import DAILY, rrule
-from scipy import integrate
-
-from ..pyrf import read_cdf, ts_append
-
-__author__ = "Louis Richard"
-__email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2022"
-__license__ = "MIT"
-__version__ = "2.3.22"
-__status__ = "Prototype"
-
-logging.captureWarnings(True)
-logging.basicConfig(
-    format="[%(asctime)s] %(levelname)s: %(message)s",
-    datefmt="%d-%b-%y %H:%M:%S",
-    level=logging.INFO,
-)
-
-
-def _list_files_tnr_l2(tint, data_path: str = "", tree: bool = False):
-    """Find files in the L2 data repo corresponding to the target time
-    interval.
-
-    Parameters
-    ----------
-    tint : list
-        Time interval
-    data_path : str, Optional
-        Path of MMS data. Default uses `pyrfu.solo.config.json`
-    tree : bool, Optional
-        Flag for tree structured data repos. Default is False.
-
-    Returns
-    -------
-    files : list
-        List of files corresponding to the parameters in the selected time
-        interval
-
-    """
-
-    # Check path
-    if not data_path:
-        pkg_path = os.path.dirname(os.path.abspath(__file__))
-
-        # Read the current version of the MMS configuration file
-        with open(os.path.join(pkg_path, "config.json"), "r", encoding="utf-8") as fs:
-            config = json.load(fs)
-
-        data_path = os.path.normpath(config["local_data_dir"])
-    else:
-        data_path = os.path.normpath(data_path)
-
-    # Make sure that the data path exists
-    assert os.path.exists(data_path), f"{data_path} doesn't exist!!"
-
-    files_out = []
-
-    # directory and file name search patterns:
-    # - assume directories are of the form: [data_path]/L2/thr/year/month/
-    # - assume file names are of the form:
-    #   solo_L2_rpw-tnr-surv-cdag_YYYYMMDD_version.cdf
-
-    file_name = r"solo_L2_rpw-tnr-surv.*_([0-9]{8})_V[0-9]{2}.cdf"
-
-    d_start = parser.parse(parser.parse(tint[0]).strftime("%Y-%m-%d"))
-    until_ = parser.parse(tint[1]) - datetime.timedelta(seconds=1)
-    days = rrule(DAILY, dtstart=d_start, until=until_)
-
-    for date in days:
-        if tree:
-            local_dir = os.sep.join(
-                [
-                    data_path,
-                    "L2",
-                    "thr",
-                    date.strftime("%Y"),
-                    date.strftime("%m"),
-                ],
-            )
-        else:
-            local_dir = data_path
-
-        if os.name == "nt":
-            full_path = os.sep.join(
-                [re.escape(local_dir) + os.sep, file_name],
-            )
-        else:
-            full_path = os.sep.join([re.escape(local_dir), file_name])
-
-        regex = re.compile(full_path)
-
-        for root, _, files in os.walk(local_dir):
-            for file in files:
-                this_file = os.sep.join([root, file])
-
-                matches = regex.match(this_file)
-                if matches:
-                    this_time = parser.parse(matches.groups()[0])
-                    if d_start <= this_time <= until_:
-                        if this_file not in files_out:
-                            files_out.append(os.sep.join([local_dir, file]))
-
-    # sort in time
-    if len(files_out) > 1:
-        files_out = sorted(files_out)
-
-    return files_out
-
-
-def read_tnr(tint, sensor: int = 4, data_path: str = "", tree: bool = False):
-    r"""Read L2 data from TNR
-
-    Parameters
-    ----------
-    tint : list
-        Time interval
-    sensor : int, Optional
-        TNR sensor to be read:
-            * 1: V1
-            * 2: V2
-            * 3: V3
-            * 4: V1 - V2 (default)
-            * 5: V2 - V3
-            * 6: V3 - V1
-            * 7: B
-    data_path : str, Optional
-        Path of MMS data. Default uses `pyrfu.solo.config.json`
-    tree : bool, Optional
-        Flag for tree structured data repos. Default is False.
-
-    Returns
-    -------
-    out : xarray.DataArray
-        Spectrum of the measured signals.
-
-    Notes
-    -----
-    The script check if there are data from the two channel and put them
-    together.
-
-    """
-
-    files = _list_files_tnr_l2(tint, data_path, tree)
-
-    assert files, "No files found. Make sure that the data_path is correct"
-
-    # Initialize spectrum output to None
-    out = None
-
-    for file in files:
-        # Notify user
-        logging.info("Loading %s...", os.path.split(file)[-1])
-
-        data_l2 = read_cdf(file, tint)
-
-        n_freqs = 4 * data_l2["tnr_band_freq"].shape[1]
-        freq_tnr = np.reshape(data_l2["tnr_band_freq"].data, n_freqs) / 1000
-
-        epoch_ = data_l2["epoch"].data
-        auto1_ = data_l2["auto1"].data
-        auto2_ = data_l2["auto2"].data
-        sweep_ = data_l2["sweep_num"].data
-        bande_ = data_l2["tnr_band"].data
-        confg_ = data_l2["sensor_config"].data
-
-        if sensor == 7:
-            auto1_ = data_l2["magnetic_spectral_power1"].data
-            auto2_ = data_l2["magnetic_spectral_power2"].data
-
-        puntical = np.where(data_l2["front_end"].data == 1)[0]
-
-        epoch_ = epoch_[puntical]
-        confg_ = confg_[puntical, :]
-        auto1_ = auto1_[puntical, :]
-        auto2_ = auto2_[puntical, :]
-        sweep_ = sweep_[puntical]
-        bande_ = bande_[puntical]
-
-        sweep_num = sweep_
-
-        delta_sw = np.abs(sweep_[1:] - sweep_[:-1])
-
-        xdelta_sw = np.where(delta_sw > 100)[0]
-        if xdelta_sw.size:
-            xdelta_sw = np.hstack([xdelta_sw, len(sweep_) - 1])
-            nxdelta_sw = len(xdelta_sw)
-            for inswn in range(nxdelta_sw - 1):
-                idx_l, idx_r = [xdelta_sw[inswn] + 1, xdelta_sw[inswn + 1]]
-                sweep_num[idx_l:idx_r] += sweep_num[xdelta_sw[inswn]]
-
-        timet_ = cdfepoch.to_datetime(epoch_)
-
-        sens0_, sens1_ = [np.where(confg_[:, i] == sensor)[0] for i in range(2)]
-
-        if sens0_.size and sens1_.size:
-            auto_calib = np.vstack([auto1_[sens0_, :], auto2_[sens1_, :]])
-            sens_ = np.hstack([sens0_, sens1_])
-            timet_ici = np.hstack([timet_[sens0_], timet_[sens1_]])
-        elif sens0_.size:
-            auto_calib = auto1_[sens0_, :]
-            sens_ = sens0_
-            timet_ici = timet_[sens0_]
-        elif sens1_.size:
-            auto_calib = auto2_[sens1_, :]
-            sens_ = sens1_
-            timet_ici = timet_[sens1_]
-
-        else:
-            raise ValueError("no data at all ?!?")
-
-        ord_time = np.argsort(timet_ici)
-        time_rr = timet_ici[ord_time]
-        sens_ = sens_[ord_time]
-        auto_calib = auto_calib[ord_time, :]
-
-        bande_e = bande_[sens_]
-        max_sweep = np.max(sweep_num[sens_])
-        min_sweep = np.min(sweep_num[sens_])
-        sweep_num = sweep_num[sens_]
-
-        v_, time, sweepn_tnr = [[], [], []]
-
-        for ind_sweep in range(min_sweep, max_sweep):
-            v1_ = np.zeros(128)
-            p_punt = np.where(sweep_num == ind_sweep)[0]
-            if p_punt.size:
-                for indband in range(p_punt.size):
-                    idx_l = 32 * bande_e[p_punt[indband]]
-                    idx_r = 32 * (bande_e[p_punt[indband]] + 1)
-                    v1_[idx_l:idx_r] = auto_calib[p_punt[indband], :]
-
-                if np.sum(v1_) > 0.0:
-                    punt0_ = np.where(v1_ == 0.0)[0]
-                    if punt0_.size:
-                        v1_[punt0_] = np.nan
-                    v_.append(v1_)
-                    sweepn_tnr.append(sweep_num[p_punt[0]])
-
-            if p_punt.size:
-                time.append(time_rr[np.min(p_punt)])
-
-        time = time[1:]
-        v_ = np.stack(v_)
-
-        # select frequencies lower than 100 kHz
-        freq_tnr = freq_tnr[freq_tnr < 1e2]
-        vp = v_[1:, : len(freq_tnr)]
-
-        # Integration
-        itg = integrate.trapz(vp, axis=1) / vp.shape[0]
-        vp = vp - itg[:, None]
-
-        out = ts_append(
-            out,
-            xr.DataArray(
-                vp,
-                coords=[np.stack(time), freq_tnr],
-                dims=["time", "frequency"],
-            ),
-        )
-
-    out = out[np.argsort(out.time.data)]
-
-    return out
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# Built-in imports
+import datetime
+import json
+import logging
+import os
+import re
+
+# 3rd party imports
+import numpy as np
+import xarray as xr
+from cdflib import cdfepoch
+from dateutil import parser
+from dateutil.rrule import DAILY, rrule
+from scipy import integrate
+
+from ..pyrf import read_cdf, ts_append
+
+__author__ = "Louis Richard"
+__email__ = "louisr@irfu.se"
+__copyright__ = "Copyright 2020-2023"
+__license__ = "MIT"
+__version__ = "2.4.2"
+__status__ = "Prototype"
+
+logging.captureWarnings(True)
+logging.basicConfig(
+    format="[%(asctime)s] %(levelname)s: %(message)s",
+    datefmt="%d-%b-%y %H:%M:%S",
+    level=logging.INFO,
+)
+
+
+def _list_files_tnr_l2(tint, data_path: str = "", tree: bool = False):
+    """Find files in the L2 data repo corresponding to the target time
+    interval.
+
+    Parameters
+    ----------
+    tint : list
+        Time interval
+    data_path : str, Optional
+        Path of MMS data. Default uses `pyrfu.solo.config.json`
+    tree : bool, Optional
+        Flag for tree structured data repos. Default is False.
+
+    Returns
+    -------
+    files : list
+        List of files corresponding to the parameters in the selected time
+        interval
+
+    """
+
+    # Check path
+    if not data_path:
+        pkg_path = os.path.dirname(os.path.abspath(__file__))
+
+        # Read the current version of the MMS configuration file
+        with open(os.path.join(pkg_path, "config.json"), "r", encoding="utf-8") as fs:
+            config = json.load(fs)
+
+        data_path = os.path.normpath(config["local_data_dir"])
+    else:
+        data_path = os.path.normpath(data_path)
+
+    # Make sure that the data path exists
+    assert os.path.exists(data_path), f"{data_path} doesn't exist!!"
+
+    files_out = []
+
+    # directory and file name search patterns:
+    # - assume directories are of the form: [data_path]/L2/thr/year/month/
+    # - assume file names are of the form:
+    #   solo_L2_rpw-tnr-surv-cdag_YYYYMMDD_version.cdf
+
+    file_name = r"solo_L2_rpw-tnr-surv.*_([0-9]{8})_V[0-9]{2}.cdf"
+
+    d_start = parser.parse(parser.parse(tint[0]).strftime("%Y-%m-%d"))
+    until_ = parser.parse(tint[1]) - datetime.timedelta(seconds=1)
+    days = rrule(DAILY, dtstart=d_start, until=until_)
+
+    for date in days:
+        if tree:
+            local_dir = os.sep.join(
+                [
+                    data_path,
+                    "L2",
+                    "thr",
+                    date.strftime("%Y"),
+                    date.strftime("%m"),
+                ],
+            )
+        else:
+            local_dir = data_path
+
+        if os.name == "nt":
+            full_path = os.sep.join(
+                [re.escape(local_dir) + os.sep, file_name],
+            )
+        else:
+            full_path = os.sep.join([re.escape(local_dir), file_name])
+
+        regex = re.compile(full_path)
+
+        for root, _, files in os.walk(local_dir):
+            for file in files:
+                this_file = os.sep.join([root, file])
+
+                matches = regex.match(this_file)
+                if matches:
+                    this_time = parser.parse(matches.groups()[0])
+                    if d_start <= this_time <= until_:
+                        if this_file not in files_out:
+                            files_out.append(os.sep.join([local_dir, file]))
+
+    # sort in time
+    if len(files_out) > 1:
+        files_out = sorted(files_out)
+
+    return files_out
+
+
+def read_tnr(tint, sensor: int = 4, data_path: str = "", tree: bool = False):
+    r"""Read L2 data from TNR
+
+    Parameters
+    ----------
+    tint : list
+        Time interval
+    sensor : int, Optional
+        TNR sensor to be read:
+            * 1: V1
+            * 2: V2
+            * 3: V3
+            * 4: V1 - V2 (default)
+            * 5: V2 - V3
+            * 6: V3 - V1
+            * 7: B
+    data_path : str, Optional
+        Path of MMS data. Default uses `pyrfu.solo.config.json`
+    tree : bool, Optional
+        Flag for tree structured data repos. Default is False.
+
+    Returns
+    -------
+    out : xarray.DataArray
+        Spectrum of the measured signals.
+
+    Notes
+    -----
+    The script check if there are data from the two channel and put them
+    together.
+
+    """
+
+    files = _list_files_tnr_l2(tint, data_path, tree)
+
+    assert files, "No files found. Make sure that the data_path is correct"
+
+    # Initialize spectrum output to None
+    out = None
+
+    for file in files:
+        # Notify user
+        logging.info("Loading %s...", os.path.split(file)[-1])
+
+        data_l2 = read_cdf(file, tint)
+
+        n_freqs = 4 * data_l2["tnr_band_freq"].shape[1]
+        freq_tnr = np.reshape(data_l2["tnr_band_freq"].data, n_freqs) / 1000
+
+        epoch_ = data_l2["epoch"].data
+        auto1_ = data_l2["auto1"].data
+        auto2_ = data_l2["auto2"].data
+        sweep_ = data_l2["sweep_num"].data
+        bande_ = data_l2["tnr_band"].data
+        confg_ = data_l2["sensor_config"].data
+
+        if sensor == 7:
+            auto1_ = data_l2["magnetic_spectral_power1"].data
+            auto2_ = data_l2["magnetic_spectral_power2"].data
+
+        puntical = np.where(data_l2["front_end"].data == 1)[0]
+
+        epoch_ = epoch_[puntical]
+        confg_ = confg_[puntical, :]
+        auto1_ = auto1_[puntical, :]
+        auto2_ = auto2_[puntical, :]
+        sweep_ = sweep_[puntical]
+        bande_ = bande_[puntical]
+
+        sweep_num = sweep_
+
+        delta_sw = np.abs(sweep_[1:] - sweep_[:-1])
+
+        xdelta_sw = np.where(delta_sw > 100)[0]
+        if xdelta_sw.size:
+            xdelta_sw = np.hstack([xdelta_sw, len(sweep_) - 1])
+            nxdelta_sw = len(xdelta_sw)
+            for inswn in range(nxdelta_sw - 1):
+                idx_l, idx_r = [xdelta_sw[inswn] + 1, xdelta_sw[inswn + 1]]
+                sweep_num[idx_l:idx_r] += sweep_num[xdelta_sw[inswn]]
+
+        timet_ = cdfepoch.to_datetime(epoch_)
+
+        sens0_, sens1_ = [np.where(confg_[:, i] == sensor)[0] for i in range(2)]
+
+        if sens0_.size and sens1_.size:
+            auto_calib = np.vstack([auto1_[sens0_, :], auto2_[sens1_, :]])
+            sens_ = np.hstack([sens0_, sens1_])
+            timet_ici = np.hstack([timet_[sens0_], timet_[sens1_]])
+        elif sens0_.size:
+            auto_calib = auto1_[sens0_, :]
+            sens_ = sens0_
+            timet_ici = timet_[sens0_]
+        elif sens1_.size:
+            auto_calib = auto2_[sens1_, :]
+            sens_ = sens1_
+            timet_ici = timet_[sens1_]
+
+        else:
+            raise ValueError("no data at all ?!?")
+
+        ord_time = np.argsort(timet_ici)
+        time_rr = timet_ici[ord_time]
+        sens_ = sens_[ord_time]
+        auto_calib = auto_calib[ord_time, :]
+
+        bande_e = bande_[sens_]
+        max_sweep = np.max(sweep_num[sens_])
+        min_sweep = np.min(sweep_num[sens_])
+        sweep_num = sweep_num[sens_]
+
+        v_, time, sweepn_tnr = [[], [], []]
+
+        for ind_sweep in range(min_sweep, max_sweep):
+            v1_ = np.zeros(128)
+            p_punt = np.where(sweep_num == ind_sweep)[0]
+            if p_punt.size:
+                for indband in range(p_punt.size):
+                    idx_l = 32 * bande_e[p_punt[indband]]
+                    idx_r = 32 * (bande_e[p_punt[indband]] + 1)
+                    v1_[idx_l:idx_r] = auto_calib[p_punt[indband], :]
+
+                if np.sum(v1_) > 0.0:
+                    punt0_ = np.where(v1_ == 0.0)[0]
+                    if punt0_.size:
+                        v1_[punt0_] = np.nan
+                    v_.append(v1_)
+                    sweepn_tnr.append(sweep_num[p_punt[0]])
+
+            if p_punt.size:
+                time.append(time_rr[np.min(p_punt)])
+
+        time = time[1:]
+        v_ = np.stack(v_)
+
+        # select frequencies lower than 100 kHz
+        freq_tnr = freq_tnr[freq_tnr < 1e2]
+        vp = v_[1:, : len(freq_tnr)]
+
+        # Integration
+        itg = integrate.trapz(vp, axis=1) / vp.shape[0]
+        vp = vp - itg[:, None]
+
+        out = ts_append(
+            out,
+            xr.DataArray(
+                vp,
+                coords=[np.stack(time), freq_tnr],
+                dims=["time", "frequency"],
+            ),
+        )
+
+    out = out[np.argsort(out.time.data)]
+
+    return out
```

### Comparing `pyrfu-2.4.1/pyrfu/tests/test_pyrf.py` & `pyrfu-2.4.3/pyrfu/tests/test_pyrf.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 # 3rd party imports
 import numpy as np
 
 from pyrfu import mms, pyrf
 
 __author__ = "Louis Richard"
 __email__ = "louisr@irfu.se"
-__copyright__ = "Copyright 2020-2021"
+__copyright__ = "Copyright 2020-2023"
 __license__ = "MIT"
-__version__ = "2.3.7"
+__version__ = "2.4.2"
 __status__ = "Prototype"
 
 
 class TestPyrf(unittest.TestCase):
     r"""Library test class"""
 
     def setUp(self):
```

### Comparing `pyrfu-2.4.1/pyrfu.egg-info/PKG-INFO` & `pyrfu-2.4.3/pyrfu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrfu
-Version: 2.4.1
+Version: 2.4.3
 Summary: Python Space Physics (RymdFysik) Utilities
 Author-email: Louis RICHARD <louir@irfu.se>
 License: 
         MIT License
         
         Copyright (c) 2020 L. RICHARD
```

### Comparing `pyrfu-2.4.1/requirements.txt` & `pyrfu-2.4.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyrfu-2.4.1/venv/bin/activate_this.py` & `pyrfu-2.4.3/venv/bin/activate_this.py`

 * *Files identical despite different names*

