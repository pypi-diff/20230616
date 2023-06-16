# Comparing `tmp/aiida_nanotech_empa-1.0.0b1.tar.gz` & `tmp/aiida_nanotech_empa-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_nanotech_empa-1.0.0b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiida_nanotech_empa-1.0.0b2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida_nanotech_empa-1.0.0b1.tar` & `aiida_nanotech_empa-1.0.0b2.tar`

### file list

```diff
@@ -1,121 +1,121 @@
--rw-r--r--   0        0        0       13 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/.codecov.yml
--rw-r--r--   0        0        0       33 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/.coveragerc
--rw-r--r--   0        0        0       52 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/.flake8
--rw-r--r--   0        0        0      200 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/.github/install_cp2k.sh
--rw-r--r--   0        0        0      289 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/.github/install_qe.sh
--rw-r--r--   0        0        0     1737 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      795 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      135 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/.gitignore
--rw-r--r--   0        0        0     1628 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1075 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/LICENSE
--rw-r--r--   0        0        0     2277 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/README.md
--rw-r--r--   0        0        0      189 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/__init__.py
--rw-r--r--   0        0        0       51 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/helpers.py
--rw-r--r--   0        0        0      273 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/parsers/__init__.py
--rw-r--r--   0        0        0     9867 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/parsers/cp2k_gw_parser.py
--rw-r--r--   0        0        0     4846 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/parsers/cp2k_neb_parser.py
--rw-r--r--   0        0        0     2542 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/parsers/cubegen_pymol_parser.py
--rw-r--r--   0        0        0     1678 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/parsers/gaussian_casscf_parser.py
--rw-r--r--   0        0        0     1379 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/parsers/pp_parser.py
--rw-r--r--   0        0        0      230 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/plugins/__init__.py
--rw-r--r--   0        0        0     3023 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/plugins/afm.py
--rw-r--r--   0        0        0     2951 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/plugins/hrstm.py
--rw-r--r--   0        0        0     3542 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/plugins/overlap.py
--rw-r--r--   0        0        0     2863 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/plugins/stm.py
--rw-r--r--   0        0        0      168 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/schedulers/__init__.py
--rw-r--r--   0        0        0     1523 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/schedulers/lsf_ethz_euler.py
--rw-r--r--   0        0        0     1599 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/schedulers/slurm_ethz_euler.py
--rw-r--r--   0        0        0        0 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/__init__.py
--rw-r--r--   0        0        0    15829 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/analyze_structure.py
--rw-r--r--   0        0        0     1375 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/common_utils.py
--rw-r--r--   0        0        0     2736 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/cube_utils.py
--rw-r--r--   0        0        0     9994 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/gaussian_wcs_postprocess.py
--rw-r--r--   0        0        0    10034 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/igor.py
--rw-r--r--   0        0        0     5427 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/pymol_render.py
--rw-r--r--   0        0        0     8560 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/stm_tools.py
--rw-r--r--   0        0        0      103 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/version.py
--rw-r--r--   0        0        0        0 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/__init__.py
--rw-r--r--   0        0        0     1147 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/__init__.py
--rw-r--r--   0        0        0    11867 2023-06-08 15:09:59.606987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/adsorbed_gw_ic_workchain.py
--rw-r--r--   0        0        0     6154 2023-06-08 15:09:59.610987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/afm_workchain.py
--rw-r--r--   0        0        0    31717 2023-06-08 15:09:59.610987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/cp2k_utils.py
--rw-r--r--   0        0        0     2627 2023-06-08 15:09:59.610987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/ALL_POTENTIALS
--rw-r--r--   0        0        0     2333 2023-06-08 15:09:59.610987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/BASIS_DEFAULT
--rw-r--r--   0        0        0   135679 2023-06-08 15:09:59.610987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/BASIS_MOLOPT
--rw-r--r--   0        0        0   114564 2023-06-08 15:09:59.610987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/GW_BASIS_SET
--rw-r--r--   0        0        0   172445 2023-06-08 15:09:59.610987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/K_GW_BASIS
--rw-r--r--   0        0        0   135561 2023-06-08 15:09:59.610987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/POTENTIAL
--rw-r--r--   0        0        0      378 2023-06-08 15:09:59.610987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/POTENTIALS_DEFAULT
--rw-r--r--   0        0        0   154582 2023-06-08 15:09:59.614987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/RI_HFX_BASIS_all
--rw-r--r--   0        0        0     8385 2023-06-08 15:09:59.614987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/atomic_kinds.yml
--rw-r--r--   0        0        0    10869 2023-06-08 15:09:59.614987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_2pp.ini
--rw-r--r--   0        0        0    10601 2023-06-08 15:09:59.614987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_pp.ini
--rw-r--r--   0        0        0  1959318 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/dftd3.dat
--rw-r--r--   0        0        0     9698 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/diag_workchain.py
--rw-r--r--   0        0        0    13166 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/fragment_separation.py
--rw-r--r--   0        0        0     7700 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/geo_opt_workchain.py
--rw-r--r--   0        0        0     5666 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/hrstm_workchain.py
--rw-r--r--   0        0        0    11952 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/molecule_gw_workchain.py
--rw-r--r--   0        0        0     6348 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/molecule_opt_gw_workchain.py
--rw-r--r--   0        0        0     9953 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/neb_workchain.py
--rw-r--r--   0        0        0     4169 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/orbitals_workchain.py
--rw-r--r--   0        0        0     6973 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/pdos_workchain.py
--rw-r--r--   0        0        0     5592 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/phonons_workchain.py
--rw-r--r--   0        0        0     1252 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/cell_opt_protocol.yml
--rw-r--r--   0        0        0    12253 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/geo_opt_protocol.yml
--rw-r--r--   0        0        0    11446 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/gw_protocols.yml
--rw-r--r--   0        0        0     7983 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/neb_protocol.yml
--rw-r--r--   0        0        0     9918 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/phonons_protocol.yml
--rw-r--r--   0        0        0     1966 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/scf_diag_protocol.yml
--rw-r--r--   0        0        0     7603 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/scf_ot_protocol.yml
--rw-r--r--   0        0        0    14942 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/replica_workchain.py
--rw-r--r--   0        0        0     4369 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/stm_workchain.py
--rw-r--r--   0        0        0      812 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/__init__.py
--rw-r--r--   0        0        0     9185 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/casscf_series_workchain.py
--rw-r--r--   0        0        0     8919 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/casscf_workchain.py
--rw-r--r--   0        0        0     6083 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/common.py
--rw-r--r--   0        0        0     6708 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/constr_opt_chain_workchain.py
--rw-r--r--   0        0        0     7953 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/delta_scf_workchain.py
--rw-r--r--   0        0        0     5234 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/hf_mp2_workchain.py
--rw-r--r--   0        0        0    11073 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/natorb_workchain.py
--rw-r--r--   0        0        0    12134 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/relax_workchain.py
--rw-r--r--   0        0        0    11760 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/scf_workchain.py
--rw-r--r--   0        0        0    11519 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/spin_workchain.py
--rw-r--r--   0        0        0       80 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/qe/__init__.py
--rw-r--r--   0        0        0    22418 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/qe/nanoribbon.py
--rw-r--r--   0        0        0     3369 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/conftest.py
--rw-r--r--   0        0        0       96 2023-06-08 15:09:59.622987 aiida_nanotech_empa-1.0.0b1/examples/__init__.py
--rw-r--r--   0        0        0   921233 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/data/sssp_minimal/C.upf
--rw-r--r--   0        0        0   366195 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/data/sssp_minimal/H.upf
--rw-r--r--   0        0        0       13 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/.gitignore
--rwxr-xr-x   0        0        0     9833 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/aa
--rw-r--r--   0        0        0      558 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/benzene-diradical.xyz
--rw-r--r--   0        0        0      402 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/c2h2.xyz
--rw-r--r--   0        0        0      422 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/c2h2_no_spin.xyz
--rw-r--r--   0        0        0     2959 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/c2h2_on_au111.xyz
--rw-r--r--   0        0        0      467 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/c2h2_spin.xyz
--rw-r--r--   0        0        0      572 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/c2h4.xyz
--rw-r--r--   0        0        0     2533 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_ads_gw_ic.py
--rw-r--r--   0        0        0     5271 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_afm.py
--rw-r--r--   0        0        0     3527 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_diag.py
--rw-r--r--   0        0        0     3702 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_fragment_separation.py
--rw-r--r--   0        0        0     4654 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_geo_opt.py
--rw-r--r--   0        0        0     3177 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_gw.py
--rw-r--r--   0        0        0     5825 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_hrstm.py
--rw-r--r--   0        0        0     1934 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_mol_opt_gw.py
--rw-r--r--   0        0        0     6194 2023-06-08 15:09:59.630987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_neb.py
--rw-r--r--   0        0        0     3893 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_orb.py
--rw-r--r--   0        0        0     4486 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_pdos.py
--rw-r--r--   0        0        0     3057 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_phonons.py
--rw-r--r--   0        0        0     3163 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_replica_chain.py
--rw-r--r--   0        0        0     3831 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_stm.py
--rw-r--r--   0        0        0     2145 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_gaussian_casscf.py
--rw-r--r--   0        0        0     1393 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_gaussian_spin.py
--rw-r--r--   0        0        0     2776 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/examples/workflows/example_nanoribbon.py
--rw-r--r--   0        0        0      251 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/examples/workflows/h2.xyz
--rw-r--r--   0        0        0     2483 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/examples/workflows/h2_on_au111.xyz
--rw-r--r--   0        0        0     1568 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/examples/workflows/h2_on_hbn.xyz
--rw-r--r--   0        0        0      679 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/examples/workflows/si_bulk.xyz
--rw-r--r--   0        0        0     4743 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0      253 2023-06-08 15:09:59.634987 aiida_nanotech_empa-1.0.0b1/pytest.ini
--rw-r--r--   0        0        0     3610 1970-01-01 00:00:00.000000 aiida_nanotech_empa-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0       13 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/.codecov.yml
+-rw-r--r--   0        0        0       33 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/.coveragerc
+-rw-r--r--   0        0        0       52 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/.flake8
+-rw-r--r--   0        0        0      200 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/.github/install_cp2k.sh
+-rw-r--r--   0        0        0      289 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/.github/install_qe.sh
+-rw-r--r--   0        0        0     1737 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      795 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      135 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/.gitignore
+-rw-r--r--   0        0        0     1628 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1075 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/LICENSE
+-rw-r--r--   0        0        0     2277 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/README.md
+-rw-r--r--   0        0        0      189 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/__init__.py
+-rw-r--r--   0        0        0       51 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/helpers.py
+-rw-r--r--   0        0        0      273 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/parsers/__init__.py
+-rw-r--r--   0        0        0     9867 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/parsers/cp2k_gw_parser.py
+-rw-r--r--   0        0        0     4846 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/parsers/cp2k_neb_parser.py
+-rw-r--r--   0        0        0     2542 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/parsers/cubegen_pymol_parser.py
+-rw-r--r--   0        0        0     1678 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/parsers/gaussian_casscf_parser.py
+-rw-r--r--   0        0        0     1379 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/parsers/pp_parser.py
+-rw-r--r--   0        0        0      230 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/plugins/__init__.py
+-rw-r--r--   0        0        0     3023 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/plugins/afm.py
+-rw-r--r--   0        0        0     2951 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/plugins/hrstm.py
+-rw-r--r--   0        0        0     3542 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/plugins/overlap.py
+-rw-r--r--   0        0        0     2863 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/plugins/stm.py
+-rw-r--r--   0        0        0      168 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/schedulers/__init__.py
+-rw-r--r--   0        0        0     1523 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/schedulers/lsf_ethz_euler.py
+-rw-r--r--   0        0        0     1599 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/schedulers/slurm_ethz_euler.py
+-rw-r--r--   0        0        0        0 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/__init__.py
+-rw-r--r--   0        0        0    15829 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/analyze_structure.py
+-rw-r--r--   0        0        0     1375 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/common_utils.py
+-rw-r--r--   0        0        0     2736 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/cube_utils.py
+-rw-r--r--   0        0        0     9994 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/gaussian_wcs_postprocess.py
+-rw-r--r--   0        0        0    10034 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/igor.py
+-rw-r--r--   0        0        0     5427 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/pymol_render.py
+-rw-r--r--   0        0        0     8561 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/stm_tools.py
+-rw-r--r--   0        0        0      103 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/version.py
+-rw-r--r--   0        0        0        0 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/__init__.py
+-rw-r--r--   0        0        0     1147 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/__init__.py
+-rw-r--r--   0        0        0    11867 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/adsorbed_gw_ic_workchain.py
+-rw-r--r--   0        0        0     6154 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/afm_workchain.py
+-rw-r--r--   0        0        0    31717 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/cp2k_utils.py
+-rw-r--r--   0        0        0     2627 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/ALL_POTENTIALS
+-rw-r--r--   0        0        0     2333 2023-06-16 13:42:28.623693 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/BASIS_DEFAULT
+-rw-r--r--   0        0        0   136047 2023-06-16 13:42:28.627694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/BASIS_MOLOPT
+-rw-r--r--   0        0        0   114564 2023-06-16 13:42:28.627694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/GW_BASIS_SET
+-rw-r--r--   0        0        0   172445 2023-06-16 13:42:28.627694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/K_GW_BASIS
+-rw-r--r--   0        0        0   135825 2023-06-16 13:42:28.627694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/POTENTIAL
+-rw-r--r--   0        0        0      378 2023-06-16 13:42:28.627694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/POTENTIALS_DEFAULT
+-rw-r--r--   0        0        0   154582 2023-06-16 13:42:28.627694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/RI_HFX_BASIS_all
+-rw-r--r--   0        0        0     8000 2023-06-16 13:42:28.627694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/atomic_kinds.yml
+-rw-r--r--   0        0        0    10869 2023-06-16 13:42:28.627694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_2pp.ini
+-rw-r--r--   0        0        0    10601 2023-06-16 13:42:28.627694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_pp.ini
+-rw-r--r--   0        0        0  1959318 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/dftd3.dat
+-rw-r--r--   0        0        0     9698 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/diag_workchain.py
+-rw-r--r--   0        0        0    13166 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/fragment_separation.py
+-rw-r--r--   0        0        0     7700 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/geo_opt_workchain.py
+-rw-r--r--   0        0        0     5666 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/hrstm_workchain.py
+-rw-r--r--   0        0        0    11952 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/molecule_gw_workchain.py
+-rw-r--r--   0        0        0     6348 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/molecule_opt_gw_workchain.py
+-rw-r--r--   0        0        0     9953 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/neb_workchain.py
+-rw-r--r--   0        0        0     4169 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/orbitals_workchain.py
+-rw-r--r--   0        0        0     6973 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/pdos_workchain.py
+-rw-r--r--   0        0        0     5592 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/phonons_workchain.py
+-rw-r--r--   0        0        0     1252 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/cell_opt_protocol.yml
+-rw-r--r--   0        0        0    12253 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/geo_opt_protocol.yml
+-rw-r--r--   0        0        0    11446 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/gw_protocols.yml
+-rw-r--r--   0        0        0     7983 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/neb_protocol.yml
+-rw-r--r--   0        0        0     9918 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/phonons_protocol.yml
+-rw-r--r--   0        0        0     1966 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/scf_diag_protocol.yml
+-rw-r--r--   0        0        0     7603 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/scf_ot_protocol.yml
+-rw-r--r--   0        0        0    14942 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/replica_workchain.py
+-rw-r--r--   0        0        0     4369 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/stm_workchain.py
+-rw-r--r--   0        0        0      812 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/__init__.py
+-rw-r--r--   0        0        0     9185 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/casscf_series_workchain.py
+-rw-r--r--   0        0        0     8919 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/casscf_workchain.py
+-rw-r--r--   0        0        0     6083 2023-06-16 13:42:28.635694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/common.py
+-rw-r--r--   0        0        0     6708 2023-06-16 13:42:28.639694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/constr_opt_chain_workchain.py
+-rw-r--r--   0        0        0     7953 2023-06-16 13:42:28.639694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/delta_scf_workchain.py
+-rw-r--r--   0        0        0     5234 2023-06-16 13:42:28.639694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/hf_mp2_workchain.py
+-rw-r--r--   0        0        0    11073 2023-06-16 13:42:28.639694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/natorb_workchain.py
+-rw-r--r--   0        0        0    12134 2023-06-16 13:42:28.639694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/relax_workchain.py
+-rw-r--r--   0        0        0    11760 2023-06-16 13:42:28.639694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/scf_workchain.py
+-rw-r--r--   0        0        0    11519 2023-06-16 13:42:28.639694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/spin_workchain.py
+-rw-r--r--   0        0        0       80 2023-06-16 13:42:28.639694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/qe/__init__.py
+-rw-r--r--   0        0        0    22418 2023-06-16 13:42:28.639694 aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/qe/nanoribbon.py
+-rw-r--r--   0        0        0     3369 2023-06-16 13:42:28.639694 aiida_nanotech_empa-1.0.0b2/conftest.py
+-rw-r--r--   0        0        0       96 2023-06-16 13:42:28.639694 aiida_nanotech_empa-1.0.0b2/examples/__init__.py
+-rw-r--r--   0        0        0   921233 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/data/sssp_minimal/C.upf
+-rw-r--r--   0        0        0   366195 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/data/sssp_minimal/H.upf
+-rw-r--r--   0        0        0       13 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/.gitignore
+-rwxr-xr-x   0        0        0     9833 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/aa
+-rw-r--r--   0        0        0      558 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/benzene-diradical.xyz
+-rw-r--r--   0        0        0      402 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/c2h2.xyz
+-rw-r--r--   0        0        0      422 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/c2h2_no_spin.xyz
+-rw-r--r--   0        0        0     2959 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/c2h2_on_au111.xyz
+-rw-r--r--   0        0        0      467 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/c2h2_spin.xyz
+-rw-r--r--   0        0        0      572 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/c2h4.xyz
+-rw-r--r--   0        0        0     2533 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_ads_gw_ic.py
+-rw-r--r--   0        0        0     5271 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_afm.py
+-rw-r--r--   0        0        0     3527 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_diag.py
+-rw-r--r--   0        0        0     3702 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_fragment_separation.py
+-rw-r--r--   0        0        0     4654 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_geo_opt.py
+-rw-r--r--   0        0        0     3177 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_gw.py
+-rw-r--r--   0        0        0     5825 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_hrstm.py
+-rw-r--r--   0        0        0     1934 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_mol_opt_gw.py
+-rw-r--r--   0        0        0     6194 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_neb.py
+-rw-r--r--   0        0        0     3893 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_orb.py
+-rw-r--r--   0        0        0     4486 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_pdos.py
+-rw-r--r--   0        0        0     3057 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_phonons.py
+-rw-r--r--   0        0        0     3163 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_replica_chain.py
+-rw-r--r--   0        0        0     3831 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_stm.py
+-rw-r--r--   0        0        0     2145 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_gaussian_casscf.py
+-rw-r--r--   0        0        0     1393 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_gaussian_spin.py
+-rw-r--r--   0        0        0     2776 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/example_nanoribbon.py
+-rw-r--r--   0        0        0      251 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/h2.xyz
+-rw-r--r--   0        0        0     2483 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/h2_on_au111.xyz
+-rw-r--r--   0        0        0     1568 2023-06-16 13:42:28.643694 aiida_nanotech_empa-1.0.0b2/examples/workflows/h2_on_hbn.xyz
+-rw-r--r--   0        0        0      679 2023-06-16 13:42:28.647694 aiida_nanotech_empa-1.0.0b2/examples/workflows/si_bulk.xyz
+-rw-r--r--   0        0        0     4743 2023-06-16 13:42:28.647694 aiida_nanotech_empa-1.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0      253 2023-06-16 13:42:28.647694 aiida_nanotech_empa-1.0.0b2/pytest.ini
+-rw-r--r--   0        0        0     3610 1970-01-01 00:00:00.000000 aiida_nanotech_empa-1.0.0b2/PKG-INFO
```

### Comparing `aiida_nanotech_empa-1.0.0b1/.github/workflows/ci.yml` & `aiida_nanotech_empa-1.0.0b2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/.github/workflows/publish.yml` & `aiida_nanotech_empa-1.0.0b2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/.pre-commit-config.yaml` & `aiida_nanotech_empa-1.0.0b2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/LICENSE` & `aiida_nanotech_empa-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/README.md` & `aiida_nanotech_empa-1.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/parsers/cp2k_gw_parser.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/parsers/cp2k_gw_parser.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/parsers/cp2k_neb_parser.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/parsers/cp2k_neb_parser.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/parsers/cubegen_pymol_parser.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/parsers/cubegen_pymol_parser.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/parsers/gaussian_casscf_parser.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/parsers/gaussian_casscf_parser.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/parsers/pp_parser.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/parsers/pp_parser.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/plugins/afm.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/plugins/afm.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/plugins/hrstm.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/plugins/hrstm.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/plugins/overlap.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/plugins/overlap.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/plugins/stm.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/plugins/stm.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/schedulers/lsf_ethz_euler.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/schedulers/lsf_ethz_euler.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/schedulers/slurm_ethz_euler.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/schedulers/slurm_ethz_euler.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/analyze_structure.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/analyze_structure.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/common_utils.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/cube_utils.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/cube_utils.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/gaussian_wcs_postprocess.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/gaussian_wcs_postprocess.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/igor.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/igor.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/pymol_render.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/pymol_render.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/utils/stm_tools.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/utils/stm_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import matplotlib.pyplot as plt
 import numpy as np
 
+from ..helpers import ANG_TO_BOHR, HART_2_EV
 from . import igor
-from .helpers import ANG_TO_BOHR, HART_2_EV
 
 
 def process_cube_planes_array(cpa):
     x_arr = cpa.get_array("x_arr")
     y_arr = cpa.get_array("y_arr")
     h_arr = cpa.get_array("h_arr")
```

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/__init__.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/adsorbed_gw_ic_workchain.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/adsorbed_gw_ic_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/afm_workchain.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/afm_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/cp2k_utils.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/cp2k_utils.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/ALL_POTENTIALS` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/ALL_POTENTIALS`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/BASIS_DEFAULT` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/BASIS_DEFAULT`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/BASIS_MOLOPT` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/BASIS_MOLOPT`

 * *Files 0% similar despite different names*

```diff
@@ -974,14 +974,20 @@
      23.518800761960  0.037798268053  0.005040470618  0.037779070657 -0.041235150854 -0.005410838671
      11.135656103275  0.180415272016  0.031210048356 -0.119614429319 -0.102704065658 -0.017609338317
       4.647813820246 -0.084235489885 -0.021214584887  0.224302495702 -0.276507156374 -0.043803008653
       1.866708259982 -0.502007239468 -0.088006426680 -0.183779813212 -0.405087985600 -0.067844235623
       0.734683697196 -0.487454712994 -0.241562643580  1.641649867502 -0.345669762598 -0.085057974012
       0.275672995860 -0.088909855778  0.046069503612 -2.281564821968 -0.128294724774  0.159527770719
       0.049895108245 -0.000245624853  1.008694292400  0.801660990981 -0.002074313963  0.982149424568
+Na DZVP-MOLOPT-PBE-GTH-q1 DZVP-MOLOPT-GGA-GTH-q1
+ 1
+ 2 0 1 3 2 1
+         0.55937327280667     4.32698741744364E-01    -3.62793274495803E-01    -9.29686125933925E-02
+         0.08401566905623    -7.04674873494766E-01     4.34900470135887E-01     6.69532915505373E-01
+         0.03702783530289     5.62321190742426E-01     8.24161768742155E-01     7.36941322038149E-01
  Mg SZV-MOLOPT-SR-GTH SZV-MOLOPT-SR-GTH-q10
  1
  2 0 1 7 2 1
      30.653047963189  0.054377184080 -0.008503364657  0.041949376018
      12.924389070531  0.180093043263 -0.033268853396  0.154513485142
       4.968377097667 -0.183378978769  0.039287763681  0.347080006586
       1.851827556019 -0.641604001295  0.169148911336  0.456042413582
```

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/GW_BASIS_SET` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/GW_BASIS_SET`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/K_GW_BASIS` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/K_GW_BASIS`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/POTENTIAL` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/POTENTIAL`

 * *Files 1% similar despite different names*

```diff
@@ -2573,14 +2573,22 @@
 Na GTH-PBE-q9 GTH-PBE
     3    6
      0.23652322    2     0.29510499    -0.91388488
     2
      0.14356046    1    34.60149228
      0.12993224    1   -14.27746168
 #
+Na GTH-PBE-q1 GTH-GGA-q1
+    1    0    0    0
+    0.87948364241558       1   -1.16444467445039
+       2
+    0.67053579706433       2    1.86827773481150   -0.22540116228205
+                       0.63725384210554
+    0.86099184094473       1    0.61384869795326
+#
 Mg GTH-PBE-q10 GTH-PBE
     4    6
      0.19275787    2   -20.57539077     3.04016732
     2
      0.14140682    1    41.04729209
      0.10293187    1    -9.98562566
 #
```

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/RI_HFX_BASIS_all` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/RI_HFX_BASIS_all`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/atomic_kinds.yml` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/atomic_kinds.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,83 +1,82 @@
 initial_magnetization:
-  H:  0
-  Li: 0  # oxidation state +1
-  Be: 0  # oxidation state +2
-  B:  0
-  C:  0
-  N:  0
-  O:  0
-  F:  0
-  Na: 0  # oxidation state +1
-  Mg: 0  # oxidation state +2
-  Al: 0  # oxidation state +3
+  H: 0
+  Li: 0 # oxidation state +1
+  Be: 0 # oxidation state +2
+  B: 0
+  C: 0
+  N: 0
+  O: 0
+  F: 0
+  Na: 0 # oxidation state +1
+  Mg: 0 # oxidation state +2
+  Al: 0 # oxidation state +3
   Si: 0
-  P:  0
-  S:  0
+  P: 0
+  S: 0
   Cl: 0
-  K:  0  # oxidation state +1
-  Ca: 0  # oxidation state +2
-  Sc: 0  # oxidation state +1
-  Ti: 0  # oxidation state +4
-  V:  3  # oxidation state +2 high spin
-  Cr: 4  # oxidation state +2 high spin
-  Mn: 5  # oxidation state +2 high spin
-  Fe: 4  # oxidation state +2 high spin
-  Co: 3  # oxidation state +2 high spin
-  Ni: 2  # oxidation state +2 high spin
-  Cu: 1  # oxidation state +2 high spin
-  Zn: 0  # oxidation state +2
-  Ga: 0  # oxidation state +3
+  K: 0 # oxidation state +1
+  Ca: 0 # oxidation state +2
+  Sc: 0 # oxidation state +1
+  Ti: 0 # oxidation state +4
+  V: 3 # oxidation state +2 high spin
+  Cr: 4 # oxidation state +2 high spin
+  Mn: 5 # oxidation state +2 high spin
+  Fe: 4 # oxidation state +2 high spin
+  Co: 3 # oxidation state +2 high spin
+  Ni: 2 # oxidation state +2 high spin
+  Cu: 1 # oxidation state +2 high spin
+  Zn: 0 # oxidation state +2
+  Ga: 0 # oxidation state +3
   Ge: 0
   As: 0
   Se: 0
   Br: 0
   Sr: 0
   Rb: 0
-  Y:  0
-  Zr: 0  # oxidation state +4
-  Nb: 0  # oxidation state +5 (the most stable one)
-  Mo: 2  # oxidation state +4
-  Tc: 3  # oxidation state +4
-  Ru: 4  # oxidation state +4
-  Rh: 4  # oxidation state +3
-  Pd: 2  # oxidation state +2
-  Ag: 0  # oxidation state +1
-  Cd: 0  # oxidation state +2
-  In: 0  # oxidation state +3
-  Sn: 0  # oxidation state +4
+  Y: 0
+  Zr: 0 # oxidation state +4
+  Nb: 0 # oxidation state +5 (the most stable one)
+  Mo: 2 # oxidation state +4
+  Tc: 3 # oxidation state +4
+  Ru: 4 # oxidation state +4
+  Rh: 4 # oxidation state +3
+  Pd: 2 # oxidation state +2
+  Ag: 0 # oxidation state +1
+  Cd: 0 # oxidation state +2
+  In: 0 # oxidation state +3
+  Sn: 0 # oxidation state +4
   Sb: 0
   Te: 0
-  I:  0
-
+  I: 0
 
 basis_set:
-  H:  TZV2P-MOLOPT-GTH
+  H: TZV2P-MOLOPT-GTH
   He: DZVP-MOLOPT-SR-GTH-q2
   Li: DZVP-MOLOPT-SR-GTH-q3
   Be: DZVP-MOLOPT-SR-GTH-q4
-  B:  DZVP-MOLOPT-SR-GTH-q3
-  C:  TZV2P-MOLOPT-GTH
-  N:  TZV2P-MOLOPT-GTH
-  O:  TZV2P-MOLOPT-GTH
-  F:  DZVP-MOLOPT-SR-GTH-q7
+  B: DZVP-MOLOPT-SR-GTH-q3
+  C: TZV2P-MOLOPT-GTH
+  N: TZV2P-MOLOPT-GTH
+  O: TZV2P-MOLOPT-GTH
+  F: DZVP-MOLOPT-SR-GTH-q7
   Ne: DZVP-MOLOPT-SR-GTH-q8
-  Na: DZVP-MOLOPT-SR-GTH-q9
+  Na: DZVP-MOLOPT-PBE-GTH-q1
   Mg: DZVP-MOLOPT-SR-GTH-q2
   Al: DZVP-MOLOPT-SR-GTH
   Si: DZVP-MOLOPT-SR-GTH-q4
-  P:  DZVP-MOLOPT-SR-GTH-q5
-  S:  TZV2P-MOLOPT-GTH
+  P: DZVP-MOLOPT-SR-GTH-q5
+  S: TZV2P-MOLOPT-GTH
   Cl: TZV2P-MOLOPT-GTH
   Ar: DZVP-MOLOPT-SR-GTH-q8
-  K:  DZVP-MOLOPT-SR-GTH-q9
+  K: DZVP-MOLOPT-SR-GTH-q9
   Ca: DZVP-MOLOPT-SR-GTH-q10
   Sc: DZVP-MOLOPT-SR-GTH-q11
   Ti: DZVP-MOLOPT-SR-GTH-q12
-  V:  DZVP-MOLOPT-SR-GTH-q13
+  V: DZVP-MOLOPT-SR-GTH-q13
   Cr: DZVP-MOLOPT-SR-GTH-q14
   Mn: DZVP-MOLOPT-SR-GTH-q15
   Fe: TZV2P-MOLOPT-SR-GTH-q16
   Co: DZVP-MOLOPT-SR-GTH-q17
   Ni: DZVP-MOLOPT-SR-GTH-q18
   Cu: DZVP-MOLOPT-SR-GTH-q11
   Zn: DZVP-MOLOPT-SR-GTH-q12
@@ -85,29 +84,29 @@
   Ge: DZVP-MOLOPT-SR-GTH-q4
   As: DZVP-MOLOPT-SR-GTH-q5
   Se: DZVP-MOLOPT-SR-GTH-q6
   Br: DZVP-MOLOPT-SR-GTH-q7
   Kr: DZVP-MOLOPT-SR-GTH-q8
   Rb: DZVP-MOLOPT-SR-GTH-q9
   Sr: DZVP-MOLOPT-SR-GTH-q10
-  Y:  DZVP-MOLOPT-SR-GTH-q11
+  Y: DZVP-MOLOPT-SR-GTH-q11
   Zr: DZVP-MOLOPT-SR-GTH-q12
   Nb: DZVP-MOLOPT-SR-GTH-q13
   Mo: DZVP-MOLOPT-SR-GTH-q14
   Tc: DZVP-MOLOPT-SR-GTH-q15
   Ru: DZVP-MOLOPT-SR-GTH-q16
   Rh: DZVP-MOLOPT-SR-GTH-q9
   Pd: DZVP-MOLOPT-SR-GTH-q18
   Ag: DZVP-MOLOPT-SR-GTH-q11
   Cd: DZVP-MOLOPT-SR-GTH-q12
   In: DZVP-MOLOPT-SR-GTH-q13
   Sn: DZVP-MOLOPT-SR-GTH-q4
   Sb: DZVP-MOLOPT-SR-GTH-q5
   Te: DZVP-MOLOPT-SR-GTH-q6
-  I:  DZVP-MOLOPT-SR-GTH-q7
+  I: DZVP-MOLOPT-SR-GTH-q7
   Xe: DZVP-MOLOPT-SR-GTH-q8
   Cs: DZVP-MOLOPT-SR-GTH-q9
   Ba: DZVP-MOLOPT-SR-GTH-q10
   La: DZVP-MOLOPT-SR-GTH-q11
   Ce: DZVP-MOLOPT-SR-GTH-q12
   Pr: DZVP-MOLOPT-SR-GTH-q13
   Nd: DZVP-MOLOPT-SR-GTH-q14
@@ -120,341 +119,340 @@
   Ho: DZVP-MOLOPT-SR-GTH-q21
   Er: DZVP-MOLOPT-SR-GTH-q22
   Tm: DZVP-MOLOPT-SR-GTH-q23
   Yb: DZVP-MOLOPT-SR-GTH-q24
   Lu: DZVP-MOLOPT-SR-GTH-q25
   Hf: DZVP-MOLOPT-SR-GTH-q12
   Ta: DZVP-MOLOPT-SR-GTH-q13
-  W:  DZVP-MOLOPT-SR-GTH-q14
+  W: DZVP-MOLOPT-SR-GTH-q14
   Re: DZVP-MOLOPT-SR-GTH-q15
   Os: DZVP-MOLOPT-SR-GTH-q16
   Ir: DZVP-MOLOPT-SR-GTH-q17
   Pt: DZVP-MOLOPT-SR-GTH-q18
   Au: DZVP-MOLOPT-SR-GTH-q11
   Hg: DZVP-MOLOPT-SR-GTH-q12
   Tl: DZVP-MOLOPT-SR-GTH-q13
   Pb: DZVP-MOLOPT-SR-GTH-q4
   Bi: DZVP-MOLOPT-SR-GTH-q5
   Po: DZVP-MOLOPT-SR-GTH-q6
   At: DZVP-MOLOPT-SR-GTH-q7
   Rn: DZVP-MOLOPT-SR-GTH-q8
 
-
 # -------------------------------------------------------------
 # Basis sets for the GW workchain
 # -------------------------------------------------------------
 gpw_std_gw_basis_set:
-  H:  aug-DZVP-GTH-up-up-up-up
-  B:  K-aug-DZVP-GTH-3
-  C:  aug-DZVP-GTH-up-up-up-up
-  N:  aug-DZVP-GTH
-  O:  aug-DZVP-GTH
+  H: aug-DZVP-GTH-up-up-up-up
+  B: K-aug-DZVP-GTH-3
+  C: aug-DZVP-GTH-up-up-up-up
+  N: aug-DZVP-GTH
+  O: aug-DZVP-GTH
 
 gpw_std_gw_basis_set_aux:
-  H:  RI_aug_DZ
-  B:  K-RI_aug_DZ
-  C:  RI_aug_DZ
-  N:  RI_aug_DZ
-  O:  RI_DZVP-own
+  H: RI_aug_DZ
+  B: K-RI_aug_DZ
+  C: RI_aug_DZ
+  N: RI_aug_DZ
+  O: RI_DZVP-own
 
 gapw_std_gw_basis_set:
-  H:  aug-cc-pVDZ-up
-  B:  aug-cc-pVDZ-up
-  C:  aug-cc-pVDZ-up
-  N:  aug-cc-pVDZ-up
-  O:  aug-cc-pVDZ-up
-  S:  aug-cc-pVDZ-up
+  H: aug-cc-pVDZ-up
+  B: aug-cc-pVDZ-up
+  C: aug-cc-pVDZ-up
+  N: aug-cc-pVDZ-up
+  O: aug-cc-pVDZ-up
+  S: aug-cc-pVDZ-up
   Zn: aug-cc-pVDZ-up
 
 gapw_std_gw_basis_set_aux:
-  H:  aug-cc-pVDZ-RIFIT
-  B:  aug-cc-pVDZ-RIFIT
-  C:  aug-cc-pVDZ-RIFIT
-  N:  aug-cc-pVDZ-RIFIT
-  O:  aug-cc-pVDZ-RIFIT
-  S:  aug-cc-pVDZ-RIFIT
+  H: aug-cc-pVDZ-RIFIT
+  B: aug-cc-pVDZ-RIFIT
+  C: aug-cc-pVDZ-RIFIT
+  N: aug-cc-pVDZ-RIFIT
+  O: aug-cc-pVDZ-RIFIT
+  S: aug-cc-pVDZ-RIFIT
   Zn: aug-cc-pVDZ-RIFIT
 
 gapw_hq_gw_basis_set:
-  H:  aug-cc-pVTZ
-  B:  aug-cc-pVQZ
-  C:  aug-cc-pVTZ
-  N:  aug-cc-pVQZ
-  O:  aug-cc-pVQZ
-  S:  aug-cc-pVQZ
+  H: aug-cc-pVTZ
+  B: aug-cc-pVQZ
+  C: aug-cc-pVTZ
+  N: aug-cc-pVQZ
+  O: aug-cc-pVQZ
+  S: aug-cc-pVQZ
   Zn: aug-cc-pVQZ
 
 gapw_hq_gw_basis_set_aux:
-  H:  aug-cc-pVTZ-RIFIT
-  B:  aug-cc-pVQZ-RIFIT
-  C:  aug-cc-pVTZ-RIFIT
-  N:  aug-cc-pVQZ-RIFIT
-  O:  aug-cc-pVQZ-RIFIT
-  S:  aug-cc-pVQZ-RIFIT
+  H: aug-cc-pVTZ-RIFIT
+  B: aug-cc-pVQZ-RIFIT
+  C: aug-cc-pVTZ-RIFIT
+  N: aug-cc-pVQZ-RIFIT
+  O: aug-cc-pVQZ-RIFIT
+  S: aug-cc-pVQZ-RIFIT
   Zn: aug-cc-pVQZ-RIFIT
 
 # -------------------------------------------------------------
 # Pseudopotentials
 # -------------------------------------------------------------
 pseudopotential:
-   H:  GTH-PBE-q1
-   He: GTH-PBE-q2
-   Li: GTH-PBE-q3
-   Be: GTH-PBE-q4
-   B:  GTH-PBE-q3
-   C:  GTH-PBE-q4
-   N:  GTH-PBE-q5
-   O:  GTH-PBE-q6
-   F:  GTH-PBE-q7
-   Ne: GTH-PBE-q8
-   Na: GTH-PBE-q9
-   Mg: GTH-PBE-q2
-   Al: GTH-PBE-q3
-   Si: GTH-PBE-q4
-   P:  GTH-PBE-q5
-   S:  GTH-PBE-q6
-   Cl: GTH-PBE-q7
-   Ar: GTH-PBE-q8
-   K:  GTH-PBE-q9
-   Ca: GTH-PBE-q10
-   Sc: GTH-PBE-q11
-   Ti: GTH-PBE-q12
-   V:  GTH-PBE-q13
-   Cr: GTH-PBE-q14
-   Mn: GTH-PBE-q15
-   Fe: GTH-PBE-q16
-   Co: GTH-PBE-q17
-   Ni: GTH-PBE-q18
-   Cu: GTH-PBE-q11
-   Zn: GTH-PBE-q12
-   Ga: GTH-PBE-q13
-   Ge: GTH-PBE-q4
-   As: GTH-PBE-q5
-   Se: GTH-PBE-q6
-   Br: GTH-PBE-q7
-   Kr: GTH-PBE-q8
-   Rb: GTH-PBE-q9
-   Sr: GTH-PBE-q10
-   Y:  GTH-PBE-q11
-   Zr: GTH-PBE-q12
-   Nb: GTH-PBE-q13
-   Mo: GTH-PBE-q14
-   Tc: GTH-PBE-q15
-   Ru: GTH-PBE-q16
-   Rh: GTH-PBE-q9
-   Pd: GTH-PBE-q18
-   Ag: GTH-PBE-q11
-   Cd: GTH-PBE-q12
-   In: GTH-PBE-q13
-   Sn: GTH-PBE-q4
-   Sb: GTH-PBE-q5
-   Te: GTH-PBE-q6
-   I:  GTH-PBE-q7
-   Xe: GTH-PBE-q8
-   Cs: GTH-PBE-q9
-   Ba: GTH-PBE-q10
-   La: GTH-PBE-q11
-   Ce: GTH-PBE-q12
-   Pr: GTH-PBE-q13
-   Nd: GTH-PBE-q14
-   Pm: GTH-PBE-q15
-   Sm: GTH-PBE-q16
-   Eu: GTH-PBE-q17
-   Gd: GTH-PBE-q18
-   Tb: GTH-PBE-q19
-   Dy: GTH-PBE-q20
-   Ho: GTH-PBE-q21
-   Er: GTH-PBE-q22
-   Tm: GTH-PBE-q23
-   Yb: GTH-PBE-q24
-   Lu: GTH-PBE-q25
-   Hf: GTH-PBE-q12
-   Ta: GTH-PBE-q13
-   W:  GTH-PBE-q14
-   Re: GTH-PBE-q15
-   Os: GTH-PBE-q16
-   Ir: GTH-PBE-q17
-   Pt: GTH-PBE-q18
-   Au: GTH-PBE-q11
-   Hg: GTH-PBE-q12
-   Tl: GTH-PBE-q13
-   Pb: GTH-PBE-q4
-   Bi: GTH-PBE-q5
-   Po: GTH-PBE-q6
-   At: GTH-PBE-q7
-   Rn: GTH-PBE-q8
+  H: GTH-PBE-q1
+  He: GTH-PBE-q2
+  Li: GTH-PBE-q3
+  Be: GTH-PBE-q4
+  B: GTH-PBE-q3
+  C: GTH-PBE-q4
+  N: GTH-PBE-q5
+  O: GTH-PBE-q6
+  F: GTH-PBE-q7
+  Ne: GTH-PBE-q8
+  Na: GTH-PBE-q1
+  Mg: GTH-PBE-q2
+  Al: GTH-PBE-q3
+  Si: GTH-PBE-q4
+  P: GTH-PBE-q5
+  S: GTH-PBE-q6
+  Cl: GTH-PBE-q7
+  Ar: GTH-PBE-q8
+  K: GTH-PBE-q9
+  Ca: GTH-PBE-q10
+  Sc: GTH-PBE-q11
+  Ti: GTH-PBE-q12
+  V: GTH-PBE-q13
+  Cr: GTH-PBE-q14
+  Mn: GTH-PBE-q15
+  Fe: GTH-PBE-q16
+  Co: GTH-PBE-q17
+  Ni: GTH-PBE-q18
+  Cu: GTH-PBE-q11
+  Zn: GTH-PBE-q12
+  Ga: GTH-PBE-q13
+  Ge: GTH-PBE-q4
+  As: GTH-PBE-q5
+  Se: GTH-PBE-q6
+  Br: GTH-PBE-q7
+  Kr: GTH-PBE-q8
+  Rb: GTH-PBE-q9
+  Sr: GTH-PBE-q10
+  Y: GTH-PBE-q11
+  Zr: GTH-PBE-q12
+  Nb: GTH-PBE-q13
+  Mo: GTH-PBE-q14
+  Tc: GTH-PBE-q15
+  Ru: GTH-PBE-q16
+  Rh: GTH-PBE-q9
+  Pd: GTH-PBE-q18
+  Ag: GTH-PBE-q11
+  Cd: GTH-PBE-q12
+  In: GTH-PBE-q13
+  Sn: GTH-PBE-q4
+  Sb: GTH-PBE-q5
+  Te: GTH-PBE-q6
+  I: GTH-PBE-q7
+  Xe: GTH-PBE-q8
+  Cs: GTH-PBE-q9
+  Ba: GTH-PBE-q10
+  La: GTH-PBE-q11
+  Ce: GTH-PBE-q12
+  Pr: GTH-PBE-q13
+  Nd: GTH-PBE-q14
+  Pm: GTH-PBE-q15
+  Sm: GTH-PBE-q16
+  Eu: GTH-PBE-q17
+  Gd: GTH-PBE-q18
+  Tb: GTH-PBE-q19
+  Dy: GTH-PBE-q20
+  Ho: GTH-PBE-q21
+  Er: GTH-PBE-q22
+  Tm: GTH-PBE-q23
+  Yb: GTH-PBE-q24
+  Lu: GTH-PBE-q25
+  Hf: GTH-PBE-q12
+  Ta: GTH-PBE-q13
+  W: GTH-PBE-q14
+  Re: GTH-PBE-q15
+  Os: GTH-PBE-q16
+  Ir: GTH-PBE-q17
+  Pt: GTH-PBE-q18
+  Au: GTH-PBE-q11
+  Hg: GTH-PBE-q12
+  Tl: GTH-PBE-q13
+  Pb: GTH-PBE-q4
+  Bi: GTH-PBE-q5
+  Po: GTH-PBE-q6
+  At: GTH-PBE-q7
+  Rn: GTH-PBE-q8
 
 all:
-   H:  ALL
-   He: ALL
-   Li: ALL
-   Be: ALL
-   B:  ALL
-   C:  ALL
-   N:  ALL
-   O:  ALL
-   F:  ALL
-   Ne: ALL
-   Na: ALL
-   Mg: ALL
-   Al: ALL
-   Si: ALL
-   P:  ALL
-   S:  ALL
-   Cl: ALL
-   Ar: ALL
-   K:  ALL
-   Ca: ALL
-   Sc: ALL
-   Ti: ALL
-   V:  ALL
-   Cr: ALL
-   Mn: ALL
-   Fe: ALL
-   Co: ALL
-   Ni: ALL
-   Cu: ALL
-   Zn: ALL
-   Ga: ALL
-   Ge: ALL
-   As: ALL
-   Se: ALL
-   Br: ALL
-   Kr: ALL
-   Rb: ALL
-   Sr: ALL
-   Y:  ALL
-   Zr: ALL
-   Nb: ALL
-   Mo: ALL
-   Tc: ALL
-   Ru: ALL
-   Rh: ALL
-   Pd: ALL
-   Ag: ALL
-   Cd: ALL
-   In: ALL
-   Sn: ALL
-   Sb: ALL
-   Te: ALL
-   I:  ALL
-   Xe: ALL
-   Cs: ALL
-   Ba: ALL
-   La: ALL
-   Ce: ALL
-   Pr: ALL
-   Nd: ALL
-   Pm: ALL
-   Sm: ALL
-   Eu: ALL
-   Gd: ALL
-   Tb: ALL
-   Dy: ALL
-   Ho: ALL
-   Er: ALL
-   Tm: ALL
-   Yb: ALL
-   Lu: ALL
-   Hf: ALL
-   Ta: ALL
-   W:  ALL
-   Re: ALL
-   Os: ALL
-   Ir: ALL
-   Pt: ALL
-   Au: ALL
-   Hg: ALL
-   Tl: ALL
-   Pb: ALL
-   Bi: ALL
-   Po: ALL
-   At: ALL
-   Rn: ALL
+  H: ALL
+  He: ALL
+  Li: ALL
+  Be: ALL
+  B: ALL
+  C: ALL
+  N: ALL
+  O: ALL
+  F: ALL
+  Ne: ALL
+  Na: ALL
+  Mg: ALL
+  Al: ALL
+  Si: ALL
+  P: ALL
+  S: ALL
+  Cl: ALL
+  Ar: ALL
+  K: ALL
+  Ca: ALL
+  Sc: ALL
+  Ti: ALL
+  V: ALL
+  Cr: ALL
+  Mn: ALL
+  Fe: ALL
+  Co: ALL
+  Ni: ALL
+  Cu: ALL
+  Zn: ALL
+  Ga: ALL
+  Ge: ALL
+  As: ALL
+  Se: ALL
+  Br: ALL
+  Kr: ALL
+  Rb: ALL
+  Sr: ALL
+  Y: ALL
+  Zr: ALL
+  Nb: ALL
+  Mo: ALL
+  Tc: ALL
+  Ru: ALL
+  Rh: ALL
+  Pd: ALL
+  Ag: ALL
+  Cd: ALL
+  In: ALL
+  Sn: ALL
+  Sb: ALL
+  Te: ALL
+  I: ALL
+  Xe: ALL
+  Cs: ALL
+  Ba: ALL
+  La: ALL
+  Ce: ALL
+  Pr: ALL
+  Nd: ALL
+  Pm: ALL
+  Sm: ALL
+  Eu: ALL
+  Gd: ALL
+  Tb: ALL
+  Dy: ALL
+  Ho: ALL
+  Er: ALL
+  Tm: ALL
+  Yb: ALL
+  Lu: ALL
+  Hf: ALL
+  Ta: ALL
+  W: ALL
+  Re: ALL
+  Os: ALL
+  Ir: ALL
+  Pt: ALL
+  Au: ALL
+  Hg: ALL
+  Tl: ALL
+  Pb: ALL
+  Bi: ALL
+  Po: ALL
+  At: ALL
+  Rn: ALL
 
 cutoff:
-   H:  600
-   He: 600
-   Li: 600
-   Be: 600
-   B:  600
-   C:  600
-   N:  600
-   O:  600
-   F:  600
-   Ne: 600
-   Na: 600
-   Mg: 600
-   Al: 600
-   Si: 600
-   P:  600
-   S:  600
-   Cl: 600
-   Ar: 600
-   K:  600
-   Ca: 600
-   Sc: 600
-   Ti: 600
-   V:  600
-   Cr: 600
-   Mn: 600
-   Fe: 1200
-   Co: 600
-   Ni: 600
-   Cu: 600
-   Zn: 600
-   Ga: 1200
-   Ge: 600
-   As: 600
-   Se: 600
-   Br: 600
-   Kr: 600
-   Rb: 600
-   Sr: 600
-   Y:  600
-   Zr: 600
-   Nb: 600
-   Mo: 600
-   Tc: 600
-   Ru: 600
-   Rh: 600
-   Pd: 1200
-   Ag: 600
-   Cd: 600
-   In: 600
-   Sn: 600
-   Sb: 600
-   Te: 600
-   I:  600
-   Xe: 600
-   Cs: 600
-   Ba: 600
-   La: 600
-   Ce: 600
-   Pr: 600
-   Nd: 600
-   Pm: 600
-   Sm: 600
-   Eu: 600
-   Gd: 600
-   Tb: 600
-   Dy: 600
-   Ho: 600
-   Er: 600
-   Tm: 600
-   Yb: 600
-   Lu: 600
-   Hf: 600
-   Ta: 600
-   W:  600
-   Re: 600
-   Os: 600
-   Ir: 600
-   Pt: 600
-   Au: 600
-   Hg: 600
-   Tl: 600
-   Pb: 600
-   Bi: 600
-   Po: 600
-   At: 600
-   Rn: 600
+  H: 600
+  He: 600
+  Li: 600
+  Be: 600
+  B: 600
+  C: 600
+  N: 600
+  O: 600
+  F: 600
+  Ne: 600
+  Na: 600
+  Mg: 600
+  Al: 600
+  Si: 600
+  P: 600
+  S: 600
+  Cl: 600
+  Ar: 600
+  K: 600
+  Ca: 600
+  Sc: 600
+  Ti: 600
+  V: 600
+  Cr: 600
+  Mn: 600
+  Fe: 1200
+  Co: 600
+  Ni: 600
+  Cu: 600
+  Zn: 600
+  Ga: 1200
+  Ge: 600
+  As: 600
+  Se: 600
+  Br: 600
+  Kr: 600
+  Rb: 600
+  Sr: 600
+  Y: 600
+  Zr: 600
+  Nb: 600
+  Mo: 600
+  Tc: 600
+  Ru: 600
+  Rh: 600
+  Pd: 1200
+  Ag: 600
+  Cd: 600
+  In: 600
+  Sn: 600
+  Sb: 600
+  Te: 600
+  I: 600
+  Xe: 600
+  Cs: 600
+  Ba: 600
+  La: 600
+  Ce: 600
+  Pr: 600
+  Nd: 600
+  Pm: 600
+  Sm: 600
+  Eu: 600
+  Gd: 600
+  Tb: 600
+  Dy: 600
+  Ho: 600
+  Er: 600
+  Tm: 600
+  Yb: 600
+  Lu: 600
+  Hf: 600
+  Ta: 600
+  W: 600
+  Re: 600
+  Os: 600
+  Ir: 600
+  Pt: 600
+  Au: 600
+  Hg: 600
+  Tl: 600
+  Pb: 600
+  Bi: 600
+  Po: 600
+  At: 600
+  Rn: 600
```

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_2pp.ini` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_2pp.ini`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_pp.ini` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/atomtypes_pp.ini`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/data/dftd3.dat` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/data/dftd3.dat`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/diag_workchain.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/diag_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/fragment_separation.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/fragment_separation.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/geo_opt_workchain.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/geo_opt_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/hrstm_workchain.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/hrstm_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/molecule_gw_workchain.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/molecule_gw_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/molecule_opt_gw_workchain.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/molecule_opt_gw_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/neb_workchain.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/neb_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/orbitals_workchain.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/orbitals_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/pdos_workchain.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/pdos_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/phonons_workchain.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/phonons_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/cell_opt_protocol.yml` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/cell_opt_protocol.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/geo_opt_protocol.yml` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/geo_opt_protocol.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/gw_protocols.yml` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/gw_protocols.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/neb_protocol.yml` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/neb_protocol.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/phonons_protocol.yml` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/phonons_protocol.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/scf_diag_protocol.yml` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/scf_diag_protocol.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/protocols/scf_ot_protocol.yml` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/protocols/scf_ot_protocol.yml`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/replica_workchain.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/replica_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/cp2k/stm_workchain.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/cp2k/stm_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/__init__.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/casscf_series_workchain.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/casscf_series_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/casscf_workchain.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/casscf_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/common.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/common.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/constr_opt_chain_workchain.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/constr_opt_chain_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/delta_scf_workchain.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/delta_scf_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/hf_mp2_workchain.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/hf_mp2_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/natorb_workchain.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/natorb_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/relax_workchain.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/relax_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/scf_workchain.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/scf_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/gaussian/spin_workchain.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/gaussian/spin_workchain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/aiida_nanotech_empa/workflows/qe/nanoribbon.py` & `aiida_nanotech_empa-1.0.0b2/aiida_nanotech_empa/workflows/qe/nanoribbon.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/conftest.py` & `aiida_nanotech_empa-1.0.0b2/conftest.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/data/sssp_minimal/C.upf` & `aiida_nanotech_empa-1.0.0b2/examples/data/sssp_minimal/C.upf`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/data/sssp_minimal/H.upf` & `aiida_nanotech_empa-1.0.0b2/examples/data/sssp_minimal/H.upf`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/workflows/aa` & `aiida_nanotech_empa-1.0.0b2/examples/workflows/aa`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/workflows/benzene-diradical.xyz` & `aiida_nanotech_empa-1.0.0b2/examples/workflows/benzene-diradical.xyz`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/workflows/c2h2_on_au111.xyz` & `aiida_nanotech_empa-1.0.0b2/examples/workflows/c2h2_on_au111.xyz`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/workflows/c2h4.xyz` & `aiida_nanotech_empa-1.0.0b2/examples/workflows/c2h4.xyz`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_ads_gw_ic.py` & `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_ads_gw_ic.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_afm.py` & `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_afm.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_diag.py` & `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_diag.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_fragment_separation.py` & `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_fragment_separation.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_geo_opt.py` & `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_geo_opt.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_gw.py` & `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_gw.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_hrstm.py` & `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_hrstm.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_mol_opt_gw.py` & `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_mol_opt_gw.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_neb.py` & `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_neb.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_orb.py` & `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_orb.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_pdos.py` & `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_pdos.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_phonons.py` & `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_phonons.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_replica_chain.py` & `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_replica_chain.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_cp2k_stm.py` & `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_cp2k_stm.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_gaussian_casscf.py` & `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_gaussian_casscf.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_gaussian_spin.py` & `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_gaussian_spin.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/workflows/example_nanoribbon.py` & `aiida_nanotech_empa-1.0.0b2/examples/workflows/example_nanoribbon.py`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/workflows/h2_on_au111.xyz` & `aiida_nanotech_empa-1.0.0b2/examples/workflows/h2_on_au111.xyz`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/workflows/h2_on_hbn.xyz` & `aiida_nanotech_empa-1.0.0b2/examples/workflows/h2_on_hbn.xyz`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/examples/workflows/si_bulk.xyz` & `aiida_nanotech_empa-1.0.0b2/examples/workflows/si_bulk.xyz`

 * *Files identical despite different names*

### Comparing `aiida_nanotech_empa-1.0.0b1/pyproject.toml` & `aiida_nanotech_empa-1.0.0b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 "nanotech_empa.cp2k.phonons" = "aiida_nanotech_empa.workflows.cp2k:Cp2kPhononsWorkChain"
 
 
 [project.entry-points."aiida.schedulers"]
 slurm_ethz_euler = "aiida_nanotech_empa.schedulers:ETHZEulerSlurmScheduler"
 
 [tool.bumpver]
-current_version = "v1.0.0b1"
+current_version = "v1.0.0b2"
 version_pattern = "vMAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Bump version {old_version} -> {new_version}."
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `aiida_nanotech_empa-1.0.0b1/PKG-INFO` & `aiida_nanotech_empa-1.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-nanotech-empa
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: AiiDA plugins and workflows developed at nanotech@surfaces group from Empa.
 Author: nanotech@surfaces
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
 Classifier: Intended Audience :: Science/Research
```

